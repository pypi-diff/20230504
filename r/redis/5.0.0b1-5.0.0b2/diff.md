# Comparing `tmp/redis-5.0.0b1.tar.gz` & `tmp/redis-5.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.0.0b1.tar", last modified: Thu Mar 23 14:48:31 2023, max compression
+gzip compressed data, was "redis-5.0.0b2.tar", last modified: Mon Apr 24 15:08:06 2023, max compression
```

## Comparing `redis-5.0.0b1.tar` & `redis-5.0.0b2.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.909164 redis-5.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-23 14:48:15.000000 redis-5.0.0b1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-23 14:48:15.000000 redis-5.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-23 14:48:15.000000 redis-5.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-03-23 14:48:31.909164 redis-5.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-23 14:48:15.000000 redis-5.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.889163 redis-5.0.0b1/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.889163 redis-5.0.0b1/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54795 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    50565 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    79359 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    86601 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   216287 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.893164 redis-5.0.0b1/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    46268 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/ocsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.897163 redis-5.0.0b1/redis/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/parsers/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-23 14:48:15.000000 redis-5.0.0b1/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.889163 redis-5.0.0b1/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-03-23 14:48:31.000000 redis-5.0.0b1/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-03-23 14:48:31.000000 redis-5.0.0b1/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:48:31.000000 redis-5.0.0b1/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-23 14:48:31.000000 redis-5.0.0b1/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-23 14:48:31.000000 redis-5.0.0b1/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 14:48:31.909164 redis-5.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-23 14:48:15.000000 redis-5.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.897163 redis-5.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/asynctests
--rw-r--r--   0 runner    (1001) docker     (123)    15584 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/synctests
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.901163 redis-5.0.0b1/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    37469 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.901163 redis-5.0.0b1/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.905164 redis-5.0.0b1/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28059 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:48:31.905164 redis-5.0.0b1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-03-23 14:48:15.000000 redis-5.0.0b1/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.278016 redis-5.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 15:07:50.000000 redis-5.0.0b2/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 15:07:50.000000 redis-5.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 15:07:50.000000 redis-5.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-24 15:08:06.278016 redis-5.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-24 15:07:50.000000 redis-5.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.258016 redis-5.0.0b2/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55388 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79861 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86601 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216287 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/ocsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:08:06.278016 redis-5.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-24 15:07:50.000000 redis-5.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.270016 redis-5.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/asynctests
+-rw-r--r--   0 runner    (1001) docker     (123)    15584 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/synctests
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38371 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.278016 redis-5.0.0b2/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.0.0b1/LICENSE` & `redis-5.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/PKG-INFO` & `redis-5.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b1/README.md` & `redis-5.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/__init__.py` & `redis-5.0.0b2/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/__init__.py` & `redis-5.0.0b2/redis/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/client.py` & `redis-5.0.0b2/redis/asyncio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     PubSubError,
     RedisError,
     ResponseError,
     TimeoutError,
     WatchError,
 )
 from redis.typing import ChannelT, EncodableT, KeyT
-from redis.utils import safe_str, str_if_bytes
+from redis.utils import HIREDIS_AVAILABLE, _set_info_logger, safe_str, str_if_bytes
 
 PubSubHandler = Callable[[Dict[str, str]], Awaitable[None]]
 _KeyT = TypeVar("_KeyT", bound=KeyT)
 _ArgT = TypeVar("_ArgT", KeyT, EncodableT)
 _RedisT = TypeVar("_RedisT", bound="Redis")
 _NormalizeKeysT = TypeVar("_NormalizeKeysT", bound=Mapping[ChannelT, object])
 if TYPE_CHECKING:
@@ -654,34 +654,38 @@
 
     def __init__(
         self,
         connection_pool: ConnectionPool,
         shard_hint: Optional[str] = None,
         ignore_subscribe_messages: bool = False,
         encoder=None,
+        push_handler_func: Optional[Callable] = None,
     ):
         self.connection_pool = connection_pool
         self.shard_hint = shard_hint
         self.ignore_subscribe_messages = ignore_subscribe_messages
         self.connection = None
         # we need to know the encoding options for this connection in order
         # to lookup channel and pattern names for callback handlers.
         self.encoder = encoder
+        self.push_handler_func = push_handler_func
         if self.encoder is None:
             self.encoder = self.connection_pool.get_encoder()
         if self.encoder.decode_responses:
             self.health_check_response: Iterable[Union[str, bytes]] = [
                 "pong",
                 self.HEALTH_CHECK_MESSAGE,
             ]
         else:
             self.health_check_response = [
                 b"pong",
                 self.encoder.encode(self.HEALTH_CHECK_MESSAGE),
             ]
+        if self.push_handler_func is None:
+            _set_info_logger()
         self.channels = {}
         self.pending_unsubscribe_channels = set()
         self.patterns = {}
         self.pending_unsubscribe_patterns = set()
         self._lock = asyncio.Lock()
 
     async def __aenter__(self):
@@ -753,14 +757,16 @@
                 "pubsub", self.shard_hint
             )
             # register a callback that re-subscribes to any channels we
             # were listening to when we were disconnected
             self.connection.register_connect_callback(self.on_connect)
         else:
             await self.connection.connect()
+        if self.push_handler_func is not None and not HIREDIS_AVAILABLE:
+            self.connection._parser.set_push_handler(self.push_handler_func)
 
     async def _disconnect_raise_connect(self, conn, error):
         """
         Close the connection and raise an exception
         if retry_on_timeout is not set or the error
         is not a TimeoutError. Otherwise, try to reconnect
         """
@@ -793,15 +799,17 @@
 
         await self.check_health()
 
         if not conn.is_connected:
             await conn.connect()
 
         read_timeout = None if block else timeout
-        response = await self._execute(conn, conn.read_response, timeout=read_timeout)
+        response = await self._execute(
+            conn, conn.read_response, timeout=read_timeout, push_request=True
+        )
 
         if conn.health_check_interval and response == self.health_check_response:
             # ignore the health check message as user might not expect it
             return None
         return response
 
     async def check_health(self):
@@ -923,23 +931,27 @@
             return await self.handle_message(response, ignore_subscribe_messages)
         return None
 
     def ping(self, message=None) -> Awaitable:
         """
         Ping the Redis server
         """
-        message = "" if message is None else message
-        return self.execute_command("PING", message)
+        args = ["PING", message] if message is not None else ["PING"]
+        return self.execute_command(*args)
 
     async def handle_message(self, response, ignore_subscribe_messages=False):
         """
         Parses a pub/sub message. If the channel or pattern was subscribed to
         with a message handler, the handler is invoked instead of a parsed
         message being returned.
         """
+        if response is None:
+            return None
+        if isinstance(response, bytes):
+            response = [b"pong", response] if response != b"PONG" else [b"pong", b""]
         message_type = str_if_bytes(response[0])
         if message_type == "pmessage":
             message = {
                 "type": message_type,
                 "pattern": response[1],
                 "channel": response[2],
                 "data": response[3],
```

### Comparing `redis-5.0.0b1/redis/asyncio/cluster.py` & `redis-5.0.0b2/redis/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/connection.py` & `redis-5.0.0b2/redis/asyncio/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,23 +481,37 @@
                 f"Error while reading from {self.host}:{self.port}: {e.args}"
             )
 
     async def read_response(
         self,
         disable_decoding: bool = False,
         timeout: Optional[float] = None,
+        push_request: Optional[bool] = False,
     ):
         """Read the response from a previously sent command"""
         read_timeout = timeout if timeout is not None else self.socket_timeout
         try:
-            if read_timeout is not None:
+            if (
+                read_timeout is not None
+                and self.protocol == "3"
+                and not HIREDIS_AVAILABLE
+            ):
+                async with async_timeout(read_timeout):
+                    response = await self._parser.read_response(
+                        disable_decoding=disable_decoding, push_request=push_request
+                    )
+            elif read_timeout is not None:
                 async with async_timeout(read_timeout):
                     response = await self._parser.read_response(
                         disable_decoding=disable_decoding
                     )
+            elif self.protocol == "3" and not HIREDIS_AVAILABLE:
+                response = await self._parser.read_response(
+                    disable_decoding=disable_decoding, push_request=push_request
+                )
             else:
                 response = await self._parser.read_response(
                     disable_decoding=disable_decoding
                 )
         except asyncio.TimeoutError:
             if timeout is not None:
                 # user requested timeout, return None
```

### Comparing `redis-5.0.0b1/redis/asyncio/lock.py` & `redis-5.0.0b2/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/retry.py` & `redis-5.0.0b2/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/sentinel.py` & `redis-5.0.0b2/redis/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/asyncio/utils.py` & `redis-5.0.0b2/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/backoff.py` & `redis-5.0.0b2/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/client.py` & `redis-5.0.0b2/redis/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     RedisError,
     ResponseError,
     TimeoutError,
     WatchError,
 )
 from redis.lock import Lock
 from redis.retry import Retry
-from redis.utils import safe_str, str_if_bytes
+from redis.utils import HIREDIS_AVAILABLE, _set_info_logger, safe_str, str_if_bytes
 
 SYM_EMPTY = b""
 EMPTY_RESPONSE = "EMPTY_RESPONSE"
 
 # some responses (ie. dump) are binary, and just meant to never be decoded
 NEVER_DECODE = "NEVER_DECODE"
 
@@ -1425,30 +1425,34 @@
 
     def __init__(
         self,
         connection_pool,
         shard_hint=None,
         ignore_subscribe_messages=False,
         encoder=None,
+        push_handler_func=None,
     ):
         self.connection_pool = connection_pool
         self.shard_hint = shard_hint
         self.ignore_subscribe_messages = ignore_subscribe_messages
         self.connection = None
         self.subscribed_event = threading.Event()
         # we need to know the encoding options for this connection in order
         # to lookup channel and pattern names for callback handlers.
         self.encoder = encoder
+        self.push_handler_func = push_handler_func
         if self.encoder is None:
             self.encoder = self.connection_pool.get_encoder()
         self.health_check_response_b = self.encoder.encode(self.HEALTH_CHECK_MESSAGE)
         if self.encoder.decode_responses:
             self.health_check_response = ["pong", self.HEALTH_CHECK_MESSAGE]
         else:
             self.health_check_response = [b"pong", self.health_check_response_b]
+        if self.push_handler_func is None:
+            _set_info_logger()
         self.reset()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.reset()
@@ -1511,14 +1515,16 @@
         if self.connection is None:
             self.connection = self.connection_pool.get_connection(
                 "pubsub", self.shard_hint
             )
             # register a callback that re-subscribes to any channels we
             # were listening to when we were disconnected
             self.connection.register_connect_callback(self.on_connect)
+            if self.push_handler_func is not None and not HIREDIS_AVAILABLE:
+                self.connection._parser.set_push_handler(self.push_handler_func)
         connection = self.connection
         kwargs = {"check_health": not self.subscribed}
         if not self.subscribed:
             self.clean_health_check_responses()
         self._execute(connection, connection.send_command, *args, **kwargs)
 
     def clean_health_check_responses(self):
@@ -1576,15 +1582,15 @@
 
         def try_read():
             if not block:
                 if not conn.can_read(timeout=timeout):
                     return None
             else:
                 conn.connect()
-            return conn.read_response()
+            return conn.read_response(push_request=True)
 
         response = self._execute(conn, try_read)
 
         if self.is_health_check_response(response):
             # ignore the health check message as user might not expect it
             self.health_check_response_counter -= 1
             return None
@@ -1735,25 +1741,27 @@
             return self.handle_message(response, ignore_subscribe_messages)
         return None
 
     def ping(self, message=None):
         """
         Ping the Redis server
         """
-        message = "" if message is None else message
-        return self.execute_command("PING", message)
+        args = ["PING", message] if message is not None else ["PING"]
+        return self.execute_command(*args)
 
     def handle_message(self, response, ignore_subscribe_messages=False):
         """
         Parses a pub/sub message. If the channel or pattern was subscribed to
         with a message handler, the handler is invoked instead of a parsed
         message being returned.
         """
         if response is None:
             return None
+        if isinstance(response, bytes):
+            response = [b"pong", response] if response != b"PONG" else [b"pong", b""]
         message_type = str_if_bytes(response[0])
         if message_type == "pmessage":
             message = {
                 "type": message_type,
                 "pattern": response[1],
                 "channel": response[2],
                 "data": response[3],
```

### Comparing `redis-5.0.0b1/redis/cluster.py` & `redis-5.0.0b2/redis/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/__init__.py` & `redis-5.0.0b2/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/bf/__init__.py` & `redis-5.0.0b2/redis/commands/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/bf/commands.py` & `redis-5.0.0b2/redis/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/bf/info.py` & `redis-5.0.0b2/redis/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/cluster.py` & `redis-5.0.0b2/redis/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/core.py` & `redis-5.0.0b2/redis/commands/core.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/__init__.py` & `redis-5.0.0b2/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/commands.py` & `redis-5.0.0b2/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/edge.py` & `redis-5.0.0b2/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/execution_plan.py` & `redis-5.0.0b2/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/node.py` & `redis-5.0.0b2/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/path.py` & `redis-5.0.0b2/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/graph/query_result.py` & `redis-5.0.0b2/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/helpers.py` & `redis-5.0.0b2/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/json/__init__.py` & `redis-5.0.0b2/redis/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/json/commands.py` & `redis-5.0.0b2/redis/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/json/decoders.py` & `redis-5.0.0b2/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/redismodules.py` & `redis-5.0.0b2/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/__init__.py` & `redis-5.0.0b2/redis/commands/search/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/aggregation.py` & `redis-5.0.0b2/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/commands.py` & `redis-5.0.0b2/redis/commands/search/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/field.py` & `redis-5.0.0b2/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/indexDefinition.py` & `redis-5.0.0b2/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/query.py` & `redis-5.0.0b2/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/querystring.py` & `redis-5.0.0b2/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/reducers.py` & `redis-5.0.0b2/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/result.py` & `redis-5.0.0b2/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/search/suggestion.py` & `redis-5.0.0b2/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/sentinel.py` & `redis-5.0.0b2/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/timeseries/__init__.py` & `redis-5.0.0b2/redis/commands/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/timeseries/commands.py` & `redis-5.0.0b2/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/timeseries/info.py` & `redis-5.0.0b2/redis/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/commands/timeseries/utils.py` & `redis-5.0.0b2/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/connection.py` & `redis-5.0.0b2/redis/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,21 +402,26 @@
 
         try:
             return self._parser.can_read(timeout)
         except OSError as e:
             self.disconnect()
             raise ConnectionError(f"Error while reading from {host_error}: {e.args}")
 
-    def read_response(self, disable_decoding=False):
+    def read_response(self, disable_decoding=False, push_request=False):
         """Read the response from a previously sent command"""
 
         host_error = self._host_error()
 
         try:
-            response = self._parser.read_response(disable_decoding=disable_decoding)
+            if self.protocol == "3" and not HIREDIS_AVAILABLE:
+                response = self._parser.read_response(
+                    disable_decoding=disable_decoding, push_request=push_request
+                )
+            else:
+                response = self._parser.read_response(disable_decoding=disable_decoding)
         except socket.timeout:
             self.disconnect()
             raise TimeoutError(f"Timeout reading from {host_error}")
         except OSError as e:
             self.disconnect()
             raise ConnectionError(
                 f"Error while reading from {host_error}" f" : {e.args}"
@@ -701,16 +706,17 @@
                 raise ConnectionError("ocsp validation error")
         return sslsock
 
 
 class UnixDomainSocketConnection(AbstractConnection):
     "Manages UDS communication to and from a Redis server"
 
-    def __init__(self, path="", **kwargs):
+    def __init__(self, path="", socket_timeout=None, **kwargs):
         self.path = path
+        self.socket_timeout = socket_timeout
         super().__init__(**kwargs)
 
     def repr_pieces(self):
         pieces = [("path", self.path), ("db", self.db)]
         if self.client_name:
             pieces.append(("client_name", self.client_name))
         return pieces
```

### Comparing `redis-5.0.0b1/redis/crc.py` & `redis-5.0.0b2/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/credentials.py` & `redis-5.0.0b2/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/exceptions.py` & `redis-5.0.0b2/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/lock.py` & `redis-5.0.0b2/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/ocsp.py` & `redis-5.0.0b2/redis/ocsp.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/__init__.py` & `redis-5.0.0b2/redis/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/base.py` & `redis-5.0.0b2/redis/parsers/base.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/commands.py` & `redis-5.0.0b2/redis/parsers/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/encoders.py` & `redis-5.0.0b2/redis/parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/hiredis.py` & `redis-5.0.0b2/redis/parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/resp2.py` & `redis-5.0.0b2/redis/parsers/resp2.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/parsers/socket.py` & `redis-5.0.0b2/redis/parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/retry.py` & `redis-5.0.0b2/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/sentinel.py` & `redis-5.0.0b2/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/typing.py` & `redis-5.0.0b2/redis/typing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/redis/utils.py` & `redis-5.0.0b2/redis/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from contextlib import contextmanager
 from functools import wraps
 from typing import Any, Dict, Mapping, Union
 
 try:
     import hiredis  # noqa
 
@@ -113,7 +114,20 @@
         def wrapper(*args, **kwargs):
             warn_deprecated(name or func.__name__, reason, version, stacklevel=3)
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
+
+
+def _set_info_logger():
+    """
+    Set up a logger that log info logs to stdout.
+    (This is used by the default push response handler)
+    """
+    if "push_response" not in logging.root.manager.loggerDict.keys():
+        logger = logging.getLogger("push_response")
+        logger.setLevel(logging.INFO)
+        handler = logging.StreamHandler()
+        handler.setLevel(logging.INFO)
+        logger.addHandler(handler)
```

### Comparing `redis-5.0.0b1/redis.egg-info/PKG-INFO` & `redis-5.0.0b2/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b1/redis.egg-info/SOURCES.txt` & `redis-5.0.0b2/redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/setup.py` & `redis-5.0.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.0.0b1",
+    version="5.0.0b2",
     packages=find_packages(
         include=[
             "redis",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
             "redis.commands.json",
```

### Comparing `redis-5.0.0b1/tests/asynctests` & `redis-5.0.0b2/tests/asynctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/conftest.py` & `redis-5.0.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/mocks.py` & `redis-5.0.0b2/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/synctests` & `redis-5.0.0b2/tests/synctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/conftest.py` & `redis-5.0.0b2/tests/test_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/mocks.py` & `redis-5.0.0b2/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_bloom.py` & `redis-5.0.0b2/tests/test_asyncio/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_cluster.py` & `redis-5.0.0b2/tests/test_asyncio/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_commands.py` & `redis-5.0.0b2/tests/test_asyncio/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_connection.py` & `redis-5.0.0b2/tests/test_asyncio/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_connection_pool.py` & `redis-5.0.0b2/tests/test_asyncio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_credentials.py` & `redis-5.0.0b2/tests/test_asyncio/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_encoding.py` & `redis-5.0.0b2/tests/test_asyncio/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_graph.py` & `redis-5.0.0b2/tests/test_asyncio/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_json.py` & `redis-5.0.0b2/tests/test_asyncio/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_lock.py` & `redis-5.0.0b2/tests/test_asyncio/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_monitor.py` & `redis-5.0.0b2/tests/test_asyncio/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_pipeline.py` & `redis-5.0.0b2/tests/test_asyncio/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_pubsub.py` & `redis-5.0.0b2/tests/test_asyncio/test_pubsub.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 
 import pytest
 import pytest_asyncio
 
 import redis.asyncio as redis
 from redis.exceptions import ConnectionError
 from redis.typing import EncodableT
+from redis.utils import HIREDIS_AVAILABLE
 from tests.conftest import skip_if_server_version_lt
 
 from .compat import create_task, mock
+from .conftest import get_protocol_version
 
 
 def with_timeout(t):
     def wrapper(corofunc):
         @functools.wraps(corofunc)
         async def run(*args, **kwargs):
             async with async_timeout(t):
@@ -416,14 +418,31 @@
             await p.get_message()
         expect = (
             "connection not set: did you forget to call subscribe() or psubscribe()?"
         )
         assert expect in info.exconly()
 
 
+class TestPubSubRESP3Handler:
+    def my_handler(self, message):
+        self.message = ["my handler", message]
+
+    @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
+    async def test_push_handler(self, r):
+        if get_protocol_version(r) in [2, "2", None]:
+            return
+        p = r.pubsub(push_handler_func=self.my_handler)
+        await p.subscribe("foo")
+        assert await wait_for_message(p) is None
+        assert self.message == ["my handler", [b"subscribe", b"foo", 1]]
+        assert await r.publish("foo", "test message") == 1
+        assert await wait_for_message(p) is None
+        assert self.message == ["my handler", [b"message", b"foo", b"test message"]]
+
+
 @pytest.mark.onlynoncluster
 class TestPubSubAutoDecoding:
     """These tests only validate that we get unicode values back"""
 
     channel = "uni" + chr(4456) + "code"
     pattern = "uni" + chr(4456) + "*"
     data = "abc" + chr(4458) + "123"
@@ -991,17 +1010,19 @@
                     return message
 
         # get subscribe message
         msg = await get_msg()
         assert msg is not None
         # timeout waiting for another message which never arrives
         assert pubsub.connection.is_connected
-        with patch("redis.parsers._AsyncRESP2Parser.read_response") as mock1:
+        with patch("redis.parsers._AsyncRESP2Parser.read_response") as mock1, patch(
+            "redis.parsers._AsyncHiredisParser.read_response"
+        ) as mock2, patch("redis.parsers._AsyncRESP3Parser.read_response") as mock3:
             mock1.side_effect = BaseException("boom")
-            with patch("redis.parsers._AsyncHiredisParser.read_response") as mock2:
-                mock2.side_effect = BaseException("boom")
+            mock2.side_effect = BaseException("boom")
+            mock3.side_effect = BaseException("boom")
 
-                with pytest.raises(BaseException):
-                    await get_msg()
+            with pytest.raises(BaseException):
+                await get_msg()
 
         # the timeout on the read should not cause disconnect
         assert pubsub.connection.is_connected
```

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_retry.py` & `redis-5.0.0b2/tests/test_asyncio/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_scripting.py` & `redis-5.0.0b2/tests/test_asyncio/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_search.py` & `redis-5.0.0b2/tests/test_asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_sentinel.py` & `redis-5.0.0b2/tests/test_asyncio/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.0.0b2/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/test_timeseries.py` & `redis-5.0.0b2/tests/test_asyncio/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.0.0b2/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/testdata/titles.csv` & `redis-5.0.0b2/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.0.0b2/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_bloom.py` & `redis-5.0.0b2/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_cluster.py` & `redis-5.0.0b2/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_command_parser.py` & `redis-5.0.0b2/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_commands.py` & `redis-5.0.0b2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_connection.py` & `redis-5.0.0b2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_connection_pool.py` & `redis-5.0.0b2/tests/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_credentials.py` & `redis-5.0.0b2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_encoding.py` & `redis-5.0.0b2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_function.py` & `redis-5.0.0b2/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_graph.py` & `redis-5.0.0b2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_graph_utils/test_edge.py` & `redis-5.0.0b2/tests/test_graph_utils/test_edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_graph_utils/test_node.py` & `redis-5.0.0b2/tests/test_graph_utils/test_node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_graph_utils/test_path.py` & `redis-5.0.0b2/tests/test_graph_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_helpers.py` & `redis-5.0.0b2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_json.py` & `redis-5.0.0b2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_lock.py` & `redis-5.0.0b2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_monitor.py` & `redis-5.0.0b2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_multiprocessing.py` & `redis-5.0.0b2/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_pipeline.py` & `redis-5.0.0b2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_pubsub.py` & `redis-5.0.0b2/tests/test_pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
 
 import redis
 from redis.exceptions import ConnectionError
+from redis.utils import HIREDIS_AVAILABLE
 
-from .conftest import _get_client, skip_if_redis_enterprise, skip_if_server_version_lt
+from .conftest import (
+    _get_client,
+    is_resp2_connection,
+    skip_if_redis_enterprise,
+    skip_if_server_version_lt,
+)
 
 
 def wait_for_message(pubsub, timeout=0.5, ignore_subscribe_messages=False):
     now = time.time()
     timeout = now + timeout
     while now < timeout:
         message = pubsub.get_message(
@@ -348,14 +354,31 @@
         assert r.publish(channel, "test message") == 1
         assert wait_for_message(p) is None
         assert self.message == make_message(
             "pmessage", channel, "test message", pattern=pattern
         )
 
 
+class TestPubSubRESP3Handler:
+    def my_handler(self, message):
+        self.message = ["my handler", message]
+
+    @pytest.mark.skipif(HIREDIS_AVAILABLE, reason="PythonParser only")
+    def test_push_handler(self, r):
+        if is_resp2_connection(r):
+            return
+        p = r.pubsub(push_handler_func=self.my_handler)
+        p.subscribe("foo")
+        assert wait_for_message(p) is None
+        assert self.message == ["my handler", [b"subscribe", b"foo", 1]]
+        assert r.publish("foo", "test message") == 1
+        assert wait_for_message(p) is None
+        assert self.message == ["my handler", [b"message", b"foo", b"test message"]]
+
+
 class TestPubSubAutoDecoding:
     "These tests only validate that we get unicode values back"
 
     channel = "uni" + chr(4456) + "code"
     pattern = "uni" + chr(4456) + "*"
     data = "abc" + chr(4458) + "123"
 
@@ -763,17 +786,19 @@
                     return message
 
         # get subscribe message
         msg = get_msg()
         assert msg is not None
         # timeout waiting for another message which never arrives
         assert is_connected()
-        with patch("redis.parsers._RESP2Parser.read_response") as mock1:
+        with patch("redis.parsers._RESP2Parser.read_response") as mock1, patch(
+            "redis.parsers._HiredisParser.read_response"
+        ) as mock2, patch("redis.parsers._RESP3Parser.read_response") as mock3:
             mock1.side_effect = BaseException("boom")
-            with patch("redis.parsers._HiredisParser.read_response") as mock2:
-                mock2.side_effect = BaseException("boom")
+            mock2.side_effect = BaseException("boom")
+            mock3.side_effect = BaseException("boom")
 
-                with pytest.raises(BaseException):
-                    get_msg()
+            with pytest.raises(BaseException):
+                get_msg()
 
         # the timeout on the read should not cause disconnect
         assert is_connected()
```

### Comparing `redis-5.0.0b1/tests/test_retry.py` & `redis-5.0.0b2/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_scripting.py` & `redis-5.0.0b2/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_search.py` & `redis-5.0.0b2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_sentinel.py` & `redis-5.0.0b2/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_ssl.py` & `redis-5.0.0b2/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/test_timeseries.py` & `redis-5.0.0b2/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/testdata/jsontestdata.py` & `redis-5.0.0b2/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/testdata/titles.csv` & `redis-5.0.0b2/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b1/tests/testdata/will_play_text.csv.bz2` & `redis-5.0.0b2/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

