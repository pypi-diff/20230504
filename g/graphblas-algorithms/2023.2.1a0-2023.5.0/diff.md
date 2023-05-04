# Comparing `tmp/graphblas-algorithms-2023.2.1a0.tar.gz` & `tmp/graphblas-algorithms-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphblas-algorithms-2023.2.1a0.tar", last modified: Mon Feb 27 17:51:13 2023, max compression
+gzip compressed data, was "graphblas-algorithms-2023.5.0.tar", last modified: Thu May  4 18:02:33 2023, max compression
```

## Comparing `graphblas-algorithms-2023.2.1a0.tar` & `graphblas-algorithms-2023.5.0.tar`

### file list

```diff
@@ -1,111 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.427921 graphblas-algorithms-2023.2.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-02-27 17:51:13.427921 graphblas-algorithms-2023.2.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.415921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.415921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/degree_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/eigenvector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/katz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/community/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/community/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/dominating.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/isolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/link_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/link_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/reciprocity.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/regular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/simple_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/smetric.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/structuralholes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tournament.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/triads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.419921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/digraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/nodemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/nodeset.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/degree_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/eigenvector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/katz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/community/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/community/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/dominating.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/isolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/reciprocity.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/regular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/simple_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/smetric.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/structuralholes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tournament.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/triads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.423921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/tests/test_match_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.427921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:51:13.415921 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19508 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 17:51:13.000000 graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 17:51:13.427921 graphblas-algorithms-2023.2.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 17:50:55.000000 graphblas-algorithms-2023.2.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.925000 graphblas-algorithms-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.909000 graphblas-algorithms-2023.5.0/graphblas_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_bfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/degree_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/eigenvector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/katz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/weakly_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/dominating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/reciprocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/regular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/simple_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/smetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/structuralholes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tournament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/breadth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/triads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/digraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/ego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/degree_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/eigenvector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/katz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/weakly_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dominating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/ego.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/reciprocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/regular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/simple_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/smetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/structuralholes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tournament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/breadth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/triads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_match_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.909000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:02:33.925000 graphblas-algorithms-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/setup.py
```

### Comparing `graphblas-algorithms-2023.2.1a0/LICENSE` & `graphblas-algorithms-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/PKG-INFO` & `graphblas-algorithms-2023.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: graphblas-algorithms
-Version: 2023.2.1a0
+Version: 2023.5.0
 Summary: Graph algorithms written in GraphBLAS and backend for NetworkX
-Author: Erik Welch, Jim Kitchen
+Author: Jim Kitchen, Graphblas-algorithms contributors
+Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -206,52 +207,67 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/python-graphblas/graphblas-algorithms
 Project-URL: repository, https://github.com/python-graphblas/graphblas-algorithms
 Project-URL: changelog, https://github.com/python-graphblas/graphblas-algorithms/releases
 Keywords: graphblas,graph,sparse,matrix,lagraph,suitesparse,Networks,Graph Theory,Mathematics,network,discrete mathematics,math
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: complete
+Provides-Extra: all
 License-File: LICENSE
 
-# **GraphBLAS Algorithms**
-
+![GraphBLAS Algorithms](https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/logo-name-medium.svg)
+<br>
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/graphblas-algorithms.svg)](https://anaconda.org/conda-forge/graphblas-algorithms)
 [![pypi](https://img.shields.io/pypi/v/graphblas-algorithms.svg)](https://pypi.python.org/pypi/graphblas-algorithms/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphblas-algorithms)](https://pypi.python.org/pypi/graphblas-algorithms/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/graphblas-algorithms/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/graphblas-algorithms/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/graphblas-algorithms/actions)
 [![Coverage](https://codecov.io/gh/python-graphblas/graphblas-algorithms/branch/main/graph/badge.svg)](https://codecov.io/gh/python-graphblas/graphblas-algorithms)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7329185.svg)](https://doi.org/10.5281/zenodo.7329185)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 <!--- [![Docs](https://readthedocs.org/projects/graphblas-algorithms/badge/?version=latest)](https://graphblas-algorithms.readthedocs.io/en/latest/) --->
 
-GraphBLAS algorithms written in Python with [Python-graphblas](https://python-graphblas.readthedocs.io/en/latest/).  We are trying to target the NetworkX API algorithms where possible.
+`graphblas-algorithms` is a collection of GraphBLAS algorithms written using
+[`python-graphblas`](https://python-graphblas.readthedocs.io/en/latest/).
+It may be used directly or as an experimental
+[backend to NetworkX](https://networkx.org/documentation/stable/reference/classes/index.html#backends).
+
+Why use GraphBLAS Algorithms? Because it is *fast*, *flexible*, and *familiar* by using the NetworkX API.
+
+Are we missing any [algorithms](#Plugin-Algorithms) that you want?
+[Please let us know!](https://github.com/python-graphblas/graphblas-algorithms/issues)
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-networkx.png" alt="GraphBLAS vs NetworkX" title="Even faster than scipy.sparse!" width="640" />
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-igraph.png" alt="GraphBLAS vs igraph" title="igraph may use different algorithms for PageRank" width="600" />
 
 ### Installation
 ```
 conda install -c conda-forge graphblas-algorithms
 ```
 ```
 pip install graphblas-algorithms
@@ -351,14 +367,18 @@
   - generalized_degree
   - square_clustering
   - transitivity
   - triangles
 - Community
   - inter_community_edges
   - intra_community_edges
+- Components
+  - is_connected
+  - is_weakly_connected
+  - node_connected_component
 - Core
   - k_truss
 - Cuts
   - boundary_expansion
   - conductance
   - cut_size
   - edge_expansion
@@ -367,38 +387,58 @@
   - normalized_cut_size
   - volume
 - DAG
   - ancestors
   - descendants
 - Dominating
   - is_dominating_set
+- Generators
+  - ego_graph
 - Isolate
   - is_isolate
   - isolates
   - number_of_isolates
 - Link Analysis
+  - google_matrix
   - hits
   - pagerank
+- Operators
+  - compose
+  - difference
+  - disjoint_union
+  - full_join
+  - intersection
+  - symmetric_difference
+  - union
 - Reciprocity
   - overall_reciprocity
   - reciprocity
 - Regular
   - is_k_regular
   - is_regular
 - Shortest Paths
+  - all_pairs_bellman_ford_path_length
+  - all_pairs_shortest_path_length
+  - bellman_ford_path
   - floyd_warshall
+  - floyd_warshall_numpy
   - floyd_warshall_predecessor_and_distance
-  - single_source_bellman_ford_path_length
-  - all_pairs_bellman_ford_path_length
   - has_path
+  - negative_edge_cycle
+  - single_source_bellman_ford_path_length
+  - single_source_shortest_path_length
+  - single_target_shortest_path_length
 - Simple Paths
   - is_simple_path
 - S Metric
   - s_metric
 - Structural Holes
   - mutual_weight
 - Tournament
   - is_tournament
   - score_sequence
   - tournament_matrix
+- Traversal
+  - bfs_layers
+  - descendants_at_distance
 - Triads
   - is_triad
```

### Comparing `graphblas-algorithms-2023.2.1a0/README.md` & `graphblas-algorithms-2023.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-# **GraphBLAS Algorithms**
-
+![GraphBLAS Algorithms](https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/logo-name-medium.svg)
+<br>
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/graphblas-algorithms.svg)](https://anaconda.org/conda-forge/graphblas-algorithms)
 [![pypi](https://img.shields.io/pypi/v/graphblas-algorithms.svg)](https://pypi.python.org/pypi/graphblas-algorithms/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphblas-algorithms)](https://pypi.python.org/pypi/graphblas-algorithms/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/graphblas-algorithms/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/graphblas-algorithms/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/graphblas-algorithms/actions)
 [![Coverage](https://codecov.io/gh/python-graphblas/graphblas-algorithms/branch/main/graph/badge.svg)](https://codecov.io/gh/python-graphblas/graphblas-algorithms)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7329185.svg)](https://doi.org/10.5281/zenodo.7329185)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 <!--- [![Docs](https://readthedocs.org/projects/graphblas-algorithms/badge/?version=latest)](https://graphblas-algorithms.readthedocs.io/en/latest/) --->
 
-GraphBLAS algorithms written in Python with [Python-graphblas](https://python-graphblas.readthedocs.io/en/latest/).  We are trying to target the NetworkX API algorithms where possible.
+`graphblas-algorithms` is a collection of GraphBLAS algorithms written using
+[`python-graphblas`](https://python-graphblas.readthedocs.io/en/latest/).
+It may be used directly or as an experimental
+[backend to NetworkX](https://networkx.org/documentation/stable/reference/classes/index.html#backends).
+
+Why use GraphBLAS Algorithms? Because it is *fast*, *flexible*, and *familiar* by using the NetworkX API.
+
+Are we missing any [algorithms](#Plugin-Algorithms) that you want?
+[Please let us know!](https://github.com/python-graphblas/graphblas-algorithms/issues)
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-networkx.png" alt="GraphBLAS vs NetworkX" title="Even faster than scipy.sparse!" width="640" />
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-igraph.png" alt="GraphBLAS vs igraph" title="igraph may use different algorithms for PageRank" width="600" />
 
 ### Installation
 ```
 conda install -c conda-forge graphblas-algorithms
 ```
 ```
 pip install graphblas-algorithms
@@ -113,14 +127,18 @@
   - generalized_degree
   - square_clustering
   - transitivity
   - triangles
 - Community
   - inter_community_edges
   - intra_community_edges
+- Components
+  - is_connected
+  - is_weakly_connected
+  - node_connected_component
 - Core
   - k_truss
 - Cuts
   - boundary_expansion
   - conductance
   - cut_size
   - edge_expansion
@@ -129,38 +147,58 @@
   - normalized_cut_size
   - volume
 - DAG
   - ancestors
   - descendants
 - Dominating
   - is_dominating_set
+- Generators
+  - ego_graph
 - Isolate
   - is_isolate
   - isolates
   - number_of_isolates
 - Link Analysis
+  - google_matrix
   - hits
   - pagerank
+- Operators
+  - compose
+  - difference
+  - disjoint_union
+  - full_join
+  - intersection
+  - symmetric_difference
+  - union
 - Reciprocity
   - overall_reciprocity
   - reciprocity
 - Regular
   - is_k_regular
   - is_regular
 - Shortest Paths
+  - all_pairs_bellman_ford_path_length
+  - all_pairs_shortest_path_length
+  - bellman_ford_path
   - floyd_warshall
+  - floyd_warshall_numpy
   - floyd_warshall_predecessor_and_distance
-  - single_source_bellman_ford_path_length
-  - all_pairs_bellman_ford_path_length
   - has_path
+  - negative_edge_cycle
+  - single_source_bellman_ford_path_length
+  - single_source_shortest_path_length
+  - single_target_shortest_path_length
 - Simple Paths
   - is_simple_path
 - S Metric
   - s_metric
 - Structural Holes
   - mutual_weight
 - Tournament
   - is_tournament
   - score_sequence
   - tournament_matrix
+- Traversal
+  - bfs_layers
+  - descendants_at_distance
 - Triads
   - is_triad
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/__init__.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib.metadata
 
 from .classes import *
 
 from .algorithms import *  # isort:skip
+from .generators import *  # isort:skip
 
 try:
     __version__ = importlib.metadata.version("graphblas-algorithms")
 except Exception as exc:  # pragma: no cover (safety)
     raise AttributeError(
         "`graphblas_algorithms.__version__` not available. This may mean "
         "graphblas-algorithms was incorrectly installed or not installed at all. "
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/_helpers.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_helpers.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/boundary.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/boundary.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/degree_alg.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/eigenvector.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/eigenvector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from graphblas import Vector
 
-from graphblas_algorithms.algorithms._helpers import is_converged, normalize
-from graphblas_algorithms.algorithms.exceptions import (
-    ConvergenceFailure,
-    GraphBlasAlgorithmException,
-    PointlessConcept,
-)
+from .._helpers import is_converged, normalize
+from ..exceptions import ConvergenceFailure, GraphBlasAlgorithmException, PointlessConcept
 
 __all__ = ["eigenvector_centrality"]
 
 
 def eigenvector_centrality(G, max_iter=100, tol=1.0e-6, nstart=None, name="eigenvector_centrality"):
     N = len(G)
     if N == 0:
@@ -23,15 +19,15 @@
         if denom == 0:
             raise GraphBlasAlgorithmException("initial vector cannot have all zero values")
         x *= 1.0 / denom
 
     # Power iteration: make up to max_iter iterations
     A = G._A
     xprev = Vector(float, N, name="x_prev")
-    for _ in range(max_iter):
+    for _i in range(max_iter):
         xprev << x
         x += x @ A
         normalize(x, "L2")
         if is_converged(xprev, x, tol):  # sum(abs(xprev - x)) < N * tol
             x.name = name
             return x
     raise ConvergenceFailure(max_iter)
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/centrality/katz.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/katz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from graphblas import Scalar, Vector
 from graphblas.core.utils import output_type
 from graphblas.semiring import plus_first, plus_times
 
-from graphblas_algorithms.algorithms._helpers import is_converged, normalize
-from graphblas_algorithms.algorithms.exceptions import (
-    ConvergenceFailure,
-    GraphBlasAlgorithmException,
-)
+from .._helpers import is_converged, normalize
+from ..exceptions import ConvergenceFailure, GraphBlasAlgorithmException
 
 __all__ = ["katz_centrality"]
 
 
 def katz_centrality(
     G,
     alpha=0.1,
@@ -40,15 +37,15 @@
         alpha *= iso_value.get(1.0)
         semiring = plus_first[float]
     else:
         semiring = plus_times[float]
 
     # Power iteration: make up to max_iter iterations
     xprev = Vector(float, N, name="x_prev")
-    for _ in range(max_iter):
+    for _i in range(max_iter):
         xprev, x = x, xprev
         # x << alpha * semiring(xprev @ A) + beta
         x << semiring(xprev @ A)
         x *= alpha
         x += b
         if is_converged(xprev, x, tol):  # sum(abs(xprev - x)) < N * tol
             x.name = name
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/cluster.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/community/quality.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/quality.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/core.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from graphblas import Matrix, monoid, replace, select, semiring
 
-from graphblas_algorithms.classes.graph import Graph
+from graphblas_algorithms import Graph
 
 __all__ = ["k_truss"]
 
 
 def k_truss(G: Graph, k) -> Graph:
+    # TODO: should we have an option to keep the output matrix the same size?
     # Ignore self-edges
     S = G.get_property("offdiag")
 
     if k < 3:
         # Most implementations consider k < 3 invalid,
         # but networkx leaves the graph unchanged
         C = S
@@ -28,10 +29,9 @@
             S = C
 
     # Remove isolate nodes
     indices, _ = C.reduce_rowwise(monoid.any).to_coo(values=False)
     Ktruss = C[indices, indices].new()
 
     # Convert back to networkx graph with correct node ids
-    keys = G.list_to_keys(indices)
-    key_to_id = dict(zip(keys, range(len(indices))))
+    key_to_id = G.renumber_key_to_id(indices.tolist())
     return Graph(Ktruss, key_to_id=key_to_id)
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/cuts.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cuts.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/dag.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/dag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from graphblas import Vector, replace
-from graphblas.semiring import lor_pair
+from graphblas.semiring import any_pair
 
 __all__ = ["descendants", "ancestors"]
 
 
 # Push-pull optimization is possible, but annoying to implement
 def descendants(G, source):
     if source not in G._key_to_id:
         raise KeyError(f"The node {source} is not in the graph")
     index = G._key_to_id[source]
     A = G.get_property("offdiag")
-    q = Vector.from_coo(index, True, size=A.nrows, name="q")
+    q = Vector(bool, size=A.nrows, name="q")
+    q[index] = True
     rv = q.dup(name="descendants")
-    for _ in range(A.nrows):
-        q(~rv.S, replace) << lor_pair(q @ A)
+    any_pair_bool = any_pair[bool]
+    for _i in range(A.nrows):
+        q(~rv.S, replace) << any_pair_bool(q @ A)
         if q.nvals == 0:
             break
         rv(q.S) << True
     del rv[index]
     return rv
 
 
 def ancestors(G, source):
     if source not in G._key_to_id:
         raise KeyError(f"The node {source} is not in the graph")
     index = G._key_to_id[source]
     A = G.get_property("offdiag")
-    q = Vector.from_coo(index, True, size=A.nrows, name="q")
+    q = Vector(bool, size=A.nrows, name="q")
+    q[index] = True
     rv = q.dup(name="descendants")
-    for _ in range(A.nrows):
-        q(~rv.S, replace) << lor_pair(A @ q)
+    any_pair_bool = any_pair[bool]
+    for _i in range(A.nrows):
+        q(~rv.S, replace) << any_pair_bool(A @ q)
         if q.nvals == 0:
             break
         rv(q.S) << True
     del rv[index]
     return rv
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/isolate.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/isolate.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from graphblas import Vector
 
-from graphblas_algorithms.algorithms._helpers import is_converged, normalize
-from graphblas_algorithms.algorithms.exceptions import ConvergenceFailure
+from .._helpers import is_converged, normalize
+from ..exceptions import ConvergenceFailure
 
 __all__ = ["hits"]
 
 
 def hits(G, max_iter=100, tol=1.0e-8, nstart=None, normalized=True, *, with_authority=False):
     """HITS algorithms with additional parameter `with_authority`.
 
@@ -26,26 +26,26 @@
 
     # Power iteration: make up to max_iter iterations
     A = G._A
     if with_authority:
         a, h = h, a
         ATA = (A.T @ A).new(name="ATA")  # Authority matrix
         aprev = Vector(float, N, name="a_prev")
-        for _ in range(max_iter):
+        for _i in range(max_iter):
             aprev, a = a, aprev
             a << ATA @ aprev
             normalize(a, "Linf")
             if is_converged(aprev, a, tol):
                 h << A @ a
                 break
         else:
             raise ConvergenceFailure(max_iter)
     else:
         hprev = Vector(float, N, name="h_prev")
-        for _ in range(max_iter):
+        for _i in range(max_iter):
             hprev, h = h, hprev
             a << hprev @ A
             h << A @ a
             normalize(h, "Linf")
             if is_converged(hprev, h, tol):
                 break
         else:
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/reciprocity.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/reciprocity.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/regular.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/regular.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/dense.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/dense.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from graphblas import Matrix, Vector, binary, indexunary, replace, select
 from graphblas.semiring import any_plus, any_second
 
+from ..exceptions import GraphBlasAlgorithmException
+
 __all__ = ["floyd_warshall", "floyd_warshall_predecessor_and_distance"]
 
 
 def floyd_warshall(G, is_weighted=False):
     return floyd_warshall_predecessor_and_distance(G, is_weighted, compute_predecessors=False)[1]
 
 
-def floyd_warshall_predecessor_and_distance(G, is_weighted=False, *, compute_predecessors=True):
+def floyd_warshall_predecessor_and_distance(
+    G, is_weighted=False, *, compute_predecessors=True, permutation=None
+):
     # By using `offdiag` instead of `G._A`, we ensure that D will not become dense.
     # Dense D may be better at times, but not including the diagonal will result in less work.
     # Typically, Floyd-Warshall algorithms sets the diagonal of D to 0 at the beginning.
     # This is unnecessary with sparse matrices, and we set the diagonal to 0 at the end.
     # We also don't iterate over index `i` if either row i or column i are empty.
     if is_directed := G.is_directed():
         A, row_degrees, column_degrees = G.get_properties("offdiag row_degrees- column_degrees-")
         nonempty_nodes = binary.pair(row_degrees & column_degrees).new(name="nonempty_nodes")
     else:
         A, nonempty_nodes = G.get_properties("U- degrees-")
+    if permutation is not None:
+        if len(permutation) != nonempty_nodes.size:
+            raise GraphBlasAlgorithmException(
+                "permutation must contain every node in G with no repeats."
+            )
+        A = A[permutation, permutation].new()
+        nonempty_nodes = nonempty_nodes[permutation].new(name="nonempty_nodes")
 
     if A.dtype == bool or not is_weighted:
         dtype = int
     else:
         dtype = A.dtype
     n = A.nrows
     D = Matrix(dtype, nrows=n, ncols=n, name="floyd_warshall_dist")
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/shortest_paths/generic.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from graphblas import Vector, replace
-from graphblas.semiring import lor_pair
+from graphblas.semiring import any_pair
 
 __all__ = ["has_path"]
 
 
 def has_path(G, source, target):
     # Perform bidirectional BFS from source to target and target to source
     src = G._key_to_id[source]
     dst = G._key_to_id[target]
     if src == dst:
         return True
     A = G.get_property("offdiag")
-    q_src = Vector.from_coo(src, True, size=A.nrows, name="q_src")
+    q_src = Vector(bool, size=A.nrows, name="q_src")
+    q_src[src] = True
     seen_src = q_src.dup(name="seen_src")
-    q_dst = Vector.from_coo(dst, True, size=A.nrows, name="q_dst")
-    seen_dst = q_dst.dup(name="seen_dst")
-    for _ in range(A.nrows // 2):
-        q_src(~seen_src.S, replace) << lor_pair(q_src @ A)
+    q_dst = Vector(bool, size=A.nrows, name="q_dst")
+    q_dst[dst] = True
+    seen_dst = q_dst.dup(name="seen_dst", clear=True)
+    any_pair_bool = any_pair[bool]
+    for _i in range(A.nrows // 2):
+        q_src(~seen_src.S, replace) << any_pair_bool(q_src @ A)
         if q_src.nvals == 0:
             return False
-        if lor_pair(q_src @ q_dst):
+        if any_pair_bool(q_src @ q_dst):
             return True
 
-        q_dst(~seen_dst.S, replace) << lor_pair(A @ q_dst)
+        seen_dst(q_dst.S) << True
+        q_dst(~seen_dst.S, replace) << any_pair_bool(A @ q_dst)
         if q_dst.nvals == 0:
             return False
-        if lor_pair(q_src @ q_dst):
+        if any_pair_bool(q_src @ q_dst):
             return True
 
         seen_src(q_src.S) << True
-        seen_dst(q_dst.S) << True
     return False
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/simple_paths.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/simple_paths.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tests/test_cluster.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/algorithms/tournament.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tournament.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/_caching.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_caching.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/_utils.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,24 @@
             v(mask, binary.first) << fill_value
     elif fill_value is not None and v.nvals < v.size:
         v(mask=~v.S) << fill_value
     id_to_key = self.id_to_key
     return {id_to_key[index]: value for index, value in zip(*v.to_coo(sort=False))}
 
 
+def vector_to_list(self, v, *, values_are_keys=False):
+    id_to_key = self.id_to_key
+    return [
+        id_to_key[idx]
+        for idx in v.to_coo(indices=not values_are_keys, values=values_are_keys, sort=True)[
+            bool(values_are_keys)
+        ].tolist()
+    ]
+
+
 def vector_to_nodemap(self, v, *, mask=None, fill_value=None, values_are_keys=False):
     from .nodemap import NodeMap
 
     if mask is not None:
         if fill_value is not None and v.nvals < mask.parent.nvals:
             v(mask, binary.first) << fill_value
         fill_value = None
@@ -236,7 +246,16 @@
     return G
 
 
 def _cacheit(self, key, func, *args, **kwargs):
     if key not in self._cache:
         self._cache[key] = func(*args, **kwargs)
     return self._cache[key]
+
+
+def renumber_key_to_id(self, indices):
+    """Create `key_to_id` for e.g. a subgraph with node ids from `indices`"""
+    id_to_key = self.id_to_key
+    return {id_to_key[index]: i for i, index in enumerate(indices)}
+    # Alternative (about the same performance)
+    # keys = self.list_to_keys(indices)
+    # return dict(zip(keys, range(len(indices))))
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/digraph.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/digraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,18 +544,20 @@
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     matrix_to_nodenodemap = _utils.matrix_to_nodenodemap
     matrix_to_vectornodemap = _utils.matrix_to_vectornodemap
     set_to_vector = _utils.set_to_vector
     to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     _cacheit = _utils._cacheit
+    renumber_key_to_id = _utils.renumber_key_to_id
 
     # NetworkX methods
     def to_directed_class(self):
         return DiGraph
 
     def to_undirected_class(self):
         return ga.Graph
@@ -593,14 +595,24 @@
 
     def is_multigraph(self):
         return False
 
     def is_directed(self):
         return True
 
+    def to_undirected(self, reciprocal=False, as_view=False, *, name=None):
+        if as_view:
+            raise NotImplementedError("`as_vew=True` is not implemented in `G.to_undirected`")
+        A = self._A
+        if reciprocal:
+            B = binary.any(A & A.T).new(name=name)
+        else:
+            B = binary.any(A | A.T).new(name=name)
+        return Graph(B, key_to_id=self._key_to_id)
+
 
 class MultiDiGraph(DiGraph):
     def is_multigraph(self):
         return True
 
 
 __all__ = ["DiGraph", "MultiDiGraph"]
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/graph.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,23 +233,23 @@
     if "iso_value" not in cache:
         if "is_iso" in cache:
             if cache["is_iso"]:
                 # SuiteSparse:GraphBLAS
                 cache["iso_value"] = A.ss.iso_value
             else:
                 cache["iso_value"]
+
+        # min_val, max_val = G.get_properties('min_element+ max_element+')
+        # SuiteSparse:GraphBLAS
+        elif A.ss.is_iso:
+            cache["iso_value"] = A.ss.iso_value
+            cache["is_iso"] = True
         else:
-            # min_val, max_val = G.get_properties('min_element+ max_element+')
-            # SuiteSparse:GraphBLAS
-            if A.ss.is_iso:
-                cache["iso_value"] = A.ss.iso_value
-                cache["is_iso"] = True
-            else:
-                cache["iso_value"] = None
-                cache["is_iso"] = False
+            cache["iso_value"] = None
+            cache["is_iso"] = False
     return cache["iso_value"]
 
 
 def to_undirected_graph(G, weight=None, dtype=None):
     # We should do some sanity checks here to ensure we're returning a valid undirected graph
     if isinstance(G, Graph):
         return G
@@ -392,18 +392,20 @@
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     matrix_to_nodenodemap = _utils.matrix_to_nodenodemap
     matrix_to_vectornodemap = _utils.matrix_to_vectornodemap
     set_to_vector = _utils.set_to_vector
     to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     _cacheit = _utils._cacheit
+    renumber_key_to_id = _utils.renumber_key_to_id
 
     # NetworkX methods
     def to_directed_class(self):
         return ga.DiGraph
 
     def to_undirected_class(self):
         return Graph
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/nodemap.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     list_to_mask = _utils.list_to_mask
     list_to_ids = _utils.list_to_ids
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     set_to_vector = _utils.set_to_vector
     # to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     # _cacheit = _utils._cacheit
 
     # Requirements for MutableMapping
     def __delitem__(self, key):
@@ -91,14 +92,15 @@
         rv = self.vector.get(idx)
         if rv is None:
             if self._fill_value is not None:
                 return self._fill_value
             return default
         if self._values_are_keys:
             return self.id_to_key[rv]
+        return rv
 
     # items
     # keys
     # pop
 
     def popitem(self):
         v = self.vector
@@ -216,14 +218,15 @@
     list_to_mask = _utils.list_to_mask
     list_to_ids = _utils.list_to_ids
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     set_to_vector = _utils.set_to_vector
     # to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     # _cacheit = _utils._cacheit
 
     # Requirements for MutableMapping
     def __delitem__(self, key):
@@ -331,14 +334,15 @@
     list_to_mask = _utils.list_to_mask
     list_to_ids = _utils.list_to_ids
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     set_to_vector = _utils.set_to_vector
     # to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     # _cacheit = _utils._cacheit
 
     # Requirements for MutableMapping
     def __delitem__(self, key):
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/classes/nodeset.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodeset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import MutableSet
 
-from graphblas.semiring import lor_pair, plus_pair
+from graphblas.semiring import any_pair, plus_pair
 
 from . import _utils
 
 
 class NodeSet(MutableSet):
     def __init__(self, v, *, key_to_id=None):
         self.vector = v
@@ -22,14 +22,15 @@
     list_to_mask = _utils.list_to_mask
     list_to_ids = _utils.list_to_ids
     list_to_keys = _utils.list_to_keys
     matrix_to_dicts = _utils.matrix_to_dicts
     set_to_vector = _utils.set_to_vector
     # to_networkx = _utils.to_networkx
     vector_to_dict = _utils.vector_to_dict
+    vector_to_list = _utils.vector_to_list
     vector_to_nodemap = _utils.vector_to_nodemap
     vector_to_nodeset = _utils.vector_to_nodeset
     vector_to_set = _utils.vector_to_set
     # _cacheit = _utils._cacheit
 
     # Requirements for MutableSet
     def __contains__(self, x):
@@ -72,15 +73,15 @@
     # __xor__
 
     def clear(self):
         self.vector.clear()
 
     def isdisjoin(self, other):
         if isinstance(other, NodeSet):
-            return not lor_pair(self.vector @ other.vector)
+            return not any_pair[bool](self.vector @ other.vector)
         return super().isdisjoint(other)
 
     def pop(self):
         try:
             idx = next(self.vector.ss.iterkeys())
         except StopIteration:
             raise KeyError from None
@@ -100,7 +101,12 @@
         rv._id_to_key = self._id_to_key
         rv.vector = rv.set_to_vector(it, size=self.vector.size)
         return rv
 
     # Add more set methods (as needed)
     def union(self, *args):
         return set(self).union(*args)  # TODO: can we make this better?
+
+    def copy(self):
+        rv = type(self)(self.vector.dup(), key_to_id=self._key_to_id)
+        rv._id_to_key = self._id_to_key
+        return rv
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/__init__.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from .boundary import *
 from .centrality import *
 from .cluster import *
 from .community import *
+from .components import *
 from .core import *
 from .cuts import *
 from .dag import *
 from .dominating import *
+from .generators import *
 from .isolate import *
 from .link_analysis import *
+from .operators import *
 from .reciprocity import *
 from .regular import *
 from .shortest_paths import *
 from .simple_paths import *
 from .smetric import *
 from .structuralholes import *
+from .traversal import *
 from .triads import *
 
 from . import centrality
 from . import cluster
 from . import community
+from . import components
+from . import generators
 from . import link_analysis
+from . import operators
 from . import shortest_paths
 from . import tournament
+from . import traversal
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/_utils.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     if chunksize <= 0 or chunksize >= N:
         yield L
         return
     if chunksize == 1:
         yield from L
         return
     if evenly:
-        k = ceil(L / chunksize)
+        k = ceil(len(L) / chunksize)
         if k * chunksize != N:
             yield from split_evenly(k, L)
             return
     for start, stop in pairwise(range(0, N + chunksize, chunksize)):
         yield L[start:stop]
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/boundary.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/boundary.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/degree_alg.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/eigenvector.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/eigenvector.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/centrality/katz.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/katz.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/cluster.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,27 +74,14 @@
             G,
             weighted=weighted,
             count_zeros=count_zeros,
         )
     return func(G, weighted=weighted, count_zeros=count_zeros, mask=mask)
 
 
-def _split(L, k):
-    """Split a list into approximately-equal parts"""
-    N = len(L)
-    start = 0
-    for i in range(1, k):
-        stop = (N * i + k - 1) // k
-        if stop != start:
-            yield L[start:stop]
-            start = stop
-    if stop != N:
-        yield L[stop:]
-
-
 # TODO: should this move into algorithms?
 def _square_clustering_split(G, node_ids=None, *, chunksize):
     if node_ids is None:
         node_ids, _ = G._A.reduce_rowwise(monoid.any).to_coo(values=False)
     result = None
     for chunk_ids in partition(chunksize, node_ids):
         res = algorithms.square_clustering(G, chunk_ids)
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/community/quality.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/quality.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/cuts.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cuts.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/dag.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dag.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/exception.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/exception.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from graphblas_algorithms import algorithms
 from graphblas_algorithms.classes.digraph import to_graph
 
 from ..exception import PowerIterationFailedConvergence
 
-_all = ["pagerank"]
+_all = ["pagerank", "google_matrix"]
 
 
 def pagerank(
     G,
     alpha=0.85,
     personalization=None,
     max_iter=100,
@@ -39,7 +39,25 @@
             dangling=dangling_weights,
             row_degrees=row_degrees,
         )
     except algorithms.exceptions.ConvergenceFailure as e:
         raise PowerIterationFailedConvergence(*e.args) from e
     else:
         return G.vector_to_nodemap(result, fill_value=0.0)
+
+
+def google_matrix(
+    G, alpha=0.85, personalization=None, nodelist=None, weight="weight", dangling=None
+):
+    G = to_graph(G, weight=weight, dtype=float)
+    p = G.dict_to_vector(personalization, dtype=float, name="personalization")
+    if dangling is not None and G.get_property("row_degrees+").nvals < len(G):
+        dangling_weights = G.dict_to_vector(dangling, dtype=float, name="dangling")
+    else:
+        dangling_weights = None
+    return algorithms.google_matrix(
+        G,
+        alpha=alpha,
+        personalization=p,
+        nodelist=nodelist,
+        dangling=dangling_weights,
+    )
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/reciprocity.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/reciprocity.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/shortest_paths/weighted.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from graphblas_algorithms.classes.digraph import to_graph
 
 from .._utils import normalize_chunksize, partition
 from ..exception import NetworkXUnbounded, NodeNotFound
 
 __all__ = [
     "all_pairs_bellman_ford_path_length",
+    "bellman_ford_path",
+    "negative_edge_cycle",
     "single_source_bellman_ford_path_length",
 ]
 
 
 def all_pairs_bellman_ford_path_length(G, weight="weight", *, chunksize="10 MiB"):
     # Larger chunksize offers more parallelism, but uses more memory.
     # Chunksize indicates for how many source nodes to compute at one time.
@@ -48,7 +50,23 @@
     try:
         d = algorithms.single_source_bellman_ford_path_length(G, source)
     except algorithms.exceptions.Unbounded as e:
         raise NetworkXUnbounded(*e.args) from e
     except KeyError as e:
         raise NodeNotFound(*e.args) from e
     return G.vector_to_nodemap(d)
+
+
+def bellman_ford_path(G, source, target, weight="weight"):
+    # TODO: what if weight is a function?
+    G = to_graph(G, weight=weight)
+    try:
+        return algorithms.bellman_ford_path(G, source, target)
+    except KeyError as e:
+        raise NodeNotFound(*e.args) from e
+
+
+def negative_edge_cycle(G, weight="weight", heuristic=True):
+    # TODO: what if weight is a function?
+    # TODO: use a heuristic to try to stop early
+    G = to_graph(G, weight=weight)
+    return algorithms.negative_edge_cycle(G)
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/test_cluster.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tests/test_utils.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/nxapi/tournament.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tournament.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms/tests/test_core.py` & `graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,8 +29,10 @@
     pkgs.append("graphblas_algorithms")
     pkgs.sort()
     pyproject = path.parent / "pyproject.toml"
     if not pyproject.exists():
         pytest.skip("Did not find pyproject.toml")
     with pyproject.open("rb") as f:
         pkgs2 = sorted(tomli.load(f)["tool"]["setuptools"]["packages"])
-    assert pkgs == pkgs2
+    assert (
+        pkgs == pkgs2
+    ), "If there are extra items on the left, add them to pyproject.toml:tool.setuptools.packages"
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/PKG-INFO` & `graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: graphblas-algorithms
-Version: 2023.2.1a0
+Version: 2023.5.0
 Summary: Graph algorithms written in GraphBLAS and backend for NetworkX
-Author: Erik Welch, Jim Kitchen
+Author: Jim Kitchen, Graphblas-algorithms contributors
+Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -206,52 +207,67 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: homepage, https://github.com/python-graphblas/graphblas-algorithms
 Project-URL: repository, https://github.com/python-graphblas/graphblas-algorithms
 Project-URL: changelog, https://github.com/python-graphblas/graphblas-algorithms/releases
 Keywords: graphblas,graph,sparse,matrix,lagraph,suitesparse,Networks,Graph Theory,Mathematics,network,discrete mathematics,math
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: complete
+Provides-Extra: all
 License-File: LICENSE
 
-# **GraphBLAS Algorithms**
-
+![GraphBLAS Algorithms](https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/logo-name-medium.svg)
+<br>
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/graphblas-algorithms.svg)](https://anaconda.org/conda-forge/graphblas-algorithms)
 [![pypi](https://img.shields.io/pypi/v/graphblas-algorithms.svg)](https://pypi.python.org/pypi/graphblas-algorithms/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphblas-algorithms)](https://pypi.python.org/pypi/graphblas-algorithms/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/python-graphblas/graphblas-algorithms/blob/main/LICENSE)
+<br>
 [![Tests](https://github.com/python-graphblas/graphblas-algorithms/workflows/Tests/badge.svg?branch=main)](https://github.com/python-graphblas/graphblas-algorithms/actions)
 [![Coverage](https://codecov.io/gh/python-graphblas/graphblas-algorithms/branch/main/graph/badge.svg)](https://codecov.io/gh/python-graphblas/graphblas-algorithms)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7329185.svg)](https://doi.org/10.5281/zenodo.7329185)
 [![Discord](https://img.shields.io/badge/Chat-Discord-blue)](https://discord.com/invite/vur45CbwMz)
 <!--- [![Docs](https://readthedocs.org/projects/graphblas-algorithms/badge/?version=latest)](https://graphblas-algorithms.readthedocs.io/en/latest/) --->
 
-GraphBLAS algorithms written in Python with [Python-graphblas](https://python-graphblas.readthedocs.io/en/latest/).  We are trying to target the NetworkX API algorithms where possible.
+`graphblas-algorithms` is a collection of GraphBLAS algorithms written using
+[`python-graphblas`](https://python-graphblas.readthedocs.io/en/latest/).
+It may be used directly or as an experimental
+[backend to NetworkX](https://networkx.org/documentation/stable/reference/classes/index.html#backends).
+
+Why use GraphBLAS Algorithms? Because it is *fast*, *flexible*, and *familiar* by using the NetworkX API.
+
+Are we missing any [algorithms](#Plugin-Algorithms) that you want?
+[Please let us know!](https://github.com/python-graphblas/graphblas-algorithms/issues)
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-networkx.png" alt="GraphBLAS vs NetworkX" title="Even faster than scipy.sparse!" width="640" />
+<br>
+<img src="https://raw.githubusercontent.com/python-graphblas/graphblas-algorithms/main/docs/_static/img/graphblas-vs-igraph.png" alt="GraphBLAS vs igraph" title="igraph may use different algorithms for PageRank" width="600" />
 
 ### Installation
 ```
 conda install -c conda-forge graphblas-algorithms
 ```
 ```
 pip install graphblas-algorithms
@@ -351,14 +367,18 @@
   - generalized_degree
   - square_clustering
   - transitivity
   - triangles
 - Community
   - inter_community_edges
   - intra_community_edges
+- Components
+  - is_connected
+  - is_weakly_connected
+  - node_connected_component
 - Core
   - k_truss
 - Cuts
   - boundary_expansion
   - conductance
   - cut_size
   - edge_expansion
@@ -367,38 +387,58 @@
   - normalized_cut_size
   - volume
 - DAG
   - ancestors
   - descendants
 - Dominating
   - is_dominating_set
+- Generators
+  - ego_graph
 - Isolate
   - is_isolate
   - isolates
   - number_of_isolates
 - Link Analysis
+  - google_matrix
   - hits
   - pagerank
+- Operators
+  - compose
+  - difference
+  - disjoint_union
+  - full_join
+  - intersection
+  - symmetric_difference
+  - union
 - Reciprocity
   - overall_reciprocity
   - reciprocity
 - Regular
   - is_k_regular
   - is_regular
 - Shortest Paths
+  - all_pairs_bellman_ford_path_length
+  - all_pairs_shortest_path_length
+  - bellman_ford_path
   - floyd_warshall
+  - floyd_warshall_numpy
   - floyd_warshall_predecessor_and_distance
-  - single_source_bellman_ford_path_length
-  - all_pairs_bellman_ford_path_length
   - has_path
+  - negative_edge_cycle
+  - single_source_bellman_ford_path_length
+  - single_source_shortest_path_length
+  - single_target_shortest_path_length
 - Simple Paths
   - is_simple_path
 - S Metric
   - s_metric
 - Structural Holes
   - mutual_weight
 - Tournament
   - is_tournament
   - score_sequence
   - tournament_matrix
+- Traversal
+  - bfs_layers
+  - descendants_at_distance
 - Triads
   - is_triad
```

### Comparing `graphblas-algorithms-2023.2.1a0/graphblas_algorithms.egg-info/SOURCES.txt` & `graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 graphblas_algorithms.egg-info/PKG-INFO
 graphblas_algorithms.egg-info/SOURCES.txt
 graphblas_algorithms.egg-info/dependency_links.txt
 graphblas_algorithms.egg-info/entry_points.txt
 graphblas_algorithms.egg-info/requires.txt
 graphblas_algorithms.egg-info/top_level.txt
 graphblas_algorithms/algorithms/__init__.py
+graphblas_algorithms/algorithms/_bfs.py
 graphblas_algorithms/algorithms/_helpers.py
 graphblas_algorithms/algorithms/boundary.py
 graphblas_algorithms/algorithms/cluster.py
 graphblas_algorithms/algorithms/core.py
 graphblas_algorithms/algorithms/cuts.py
 graphblas_algorithms/algorithms/dag.py
 graphblas_algorithms/algorithms/dominating.py
@@ -31,30 +32,40 @@
 graphblas_algorithms/algorithms/triads.py
 graphblas_algorithms/algorithms/centrality/__init__.py
 graphblas_algorithms/algorithms/centrality/degree_alg.py
 graphblas_algorithms/algorithms/centrality/eigenvector.py
 graphblas_algorithms/algorithms/centrality/katz.py
 graphblas_algorithms/algorithms/community/__init__.py
 graphblas_algorithms/algorithms/community/quality.py
+graphblas_algorithms/algorithms/components/__init__.py
+graphblas_algorithms/algorithms/components/connected.py
+graphblas_algorithms/algorithms/components/weakly_connected.py
 graphblas_algorithms/algorithms/link_analysis/__init__.py
 graphblas_algorithms/algorithms/link_analysis/hits_alg.py
 graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
+graphblas_algorithms/algorithms/operators/__init__.py
+graphblas_algorithms/algorithms/operators/binary.py
 graphblas_algorithms/algorithms/shortest_paths/__init__.py
 graphblas_algorithms/algorithms/shortest_paths/dense.py
 graphblas_algorithms/algorithms/shortest_paths/generic.py
+graphblas_algorithms/algorithms/shortest_paths/unweighted.py
 graphblas_algorithms/algorithms/shortest_paths/weighted.py
 graphblas_algorithms/algorithms/tests/__init__.py
 graphblas_algorithms/algorithms/tests/test_cluster.py
+graphblas_algorithms/algorithms/traversal/__init__.py
+graphblas_algorithms/algorithms/traversal/breadth_first_search.py
 graphblas_algorithms/classes/__init__.py
 graphblas_algorithms/classes/_caching.py
 graphblas_algorithms/classes/_utils.py
 graphblas_algorithms/classes/digraph.py
 graphblas_algorithms/classes/graph.py
 graphblas_algorithms/classes/nodemap.py
 graphblas_algorithms/classes/nodeset.py
+graphblas_algorithms/generators/__init__.py
+graphblas_algorithms/generators/ego.py
 graphblas_algorithms/nxapi/__init__.py
 graphblas_algorithms/nxapi/_utils.py
 graphblas_algorithms/nxapi/boundary.py
 graphblas_algorithms/nxapi/cluster.py
 graphblas_algorithms/nxapi/core.py
 graphblas_algorithms/nxapi/cuts.py
 graphblas_algorithms/nxapi/dag.py
@@ -70,22 +81,32 @@
 graphblas_algorithms/nxapi/triads.py
 graphblas_algorithms/nxapi/centrality/__init__.py
 graphblas_algorithms/nxapi/centrality/degree_alg.py
 graphblas_algorithms/nxapi/centrality/eigenvector.py
 graphblas_algorithms/nxapi/centrality/katz.py
 graphblas_algorithms/nxapi/community/__init__.py
 graphblas_algorithms/nxapi/community/quality.py
+graphblas_algorithms/nxapi/components/__init__.py
+graphblas_algorithms/nxapi/components/connected.py
+graphblas_algorithms/nxapi/components/weakly_connected.py
+graphblas_algorithms/nxapi/generators/__init__.py
+graphblas_algorithms/nxapi/generators/ego.py
 graphblas_algorithms/nxapi/link_analysis/__init__.py
 graphblas_algorithms/nxapi/link_analysis/hits_alg.py
 graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
+graphblas_algorithms/nxapi/operators/__init__.py
+graphblas_algorithms/nxapi/operators/binary.py
 graphblas_algorithms/nxapi/shortest_paths/__init__.py
 graphblas_algorithms/nxapi/shortest_paths/dense.py
 graphblas_algorithms/nxapi/shortest_paths/generic.py
+graphblas_algorithms/nxapi/shortest_paths/unweighted.py
 graphblas_algorithms/nxapi/shortest_paths/weighted.py
 graphblas_algorithms/nxapi/tests/__init__.py
 graphblas_algorithms/nxapi/tests/test_cluster.py
 graphblas_algorithms/nxapi/tests/test_utils.py
+graphblas_algorithms/nxapi/traversal/__init__.py
+graphblas_algorithms/nxapi/traversal/breadth_first_search.py
 graphblas_algorithms/tests/__init__.py
 graphblas_algorithms/tests/test_core.py
 graphblas_algorithms/tests/test_match_nx.py
 graphblas_algorithms/utils/__init__.py
 graphblas_algorithms/utils/decorators.py
```

### Comparing `graphblas-algorithms-2023.2.1a0/pyproject.toml` & `graphblas-algorithms-2023.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 name = "graphblas-algorithms"
 dynamic = ["version"]
 description = "Graph algorithms written in GraphBLAS and backend for NetworkX"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
-    {name = "Erik Welch"},
+    {name = "Erik Welch", email = "erik.n.welch@gmail.com"},
     {name = "Jim Kitchen"},
+    {name = "Graphblas-algorithms contributors"},
 ]
 maintainers = [
     {name = "Erik Welch", email = "erik.n.welch@gmail.com"},
     {name = "Jim Kitchen", email = "jim22k@gmail.com"},
 ]
 keywords = [
     "graphblas",
@@ -31,24 +32,25 @@
     "Graph Theory",
     "Mathematics",
     "network",
     "discrete mathematics",
     "math",
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Information Analysis",
@@ -73,42 +75,47 @@
 test = [
     "pytest",
     "networkx >=3.0",
     "scipy >=1.8",
     "setuptools",
     "tomli",
 ]
-complete = [
-    "pytest",
-    "networkx >=3.0",
-    "scipy >=1.8",
-    "setuptools",
-    "tomli",
+all = [
+    "graphblas-algorithms[test]",
 ]
 
 [tool.setuptools]
 # Let's be explicit (we test this too)
+# TODO: it would be nice if setuptools (or our build backend) could handle this automatically and reliably.
 # $ python -c 'from setuptools import find_packages ; [print(x) for x in sorted(find_packages())]'
 # $ find graphblas_algorithms/ -name __init__.py -print | sort | sed -e 's/\/__init__.py//g' -e 's/\//./g'
 # $ python -c 'import tomli ; [print(x) for x in sorted(tomli.load(open("pyproject.toml", "rb"))["tool"]["setuptools"]["packages"])]'
 packages = [
     "graphblas_algorithms",
     "graphblas_algorithms.algorithms",
     "graphblas_algorithms.algorithms.centrality",
     "graphblas_algorithms.algorithms.community",
+    "graphblas_algorithms.algorithms.components",
     "graphblas_algorithms.algorithms.link_analysis",
+    "graphblas_algorithms.algorithms.operators",
     "graphblas_algorithms.algorithms.shortest_paths",
     "graphblas_algorithms.algorithms.tests",
+    "graphblas_algorithms.algorithms.traversal",
     "graphblas_algorithms.classes",
+    "graphblas_algorithms.generators",
     "graphblas_algorithms.nxapi",
     "graphblas_algorithms.nxapi.centrality",
     "graphblas_algorithms.nxapi.community",
+    "graphblas_algorithms.nxapi.components",
+    "graphblas_algorithms.nxapi.generators",
     "graphblas_algorithms.nxapi.link_analysis",
+    "graphblas_algorithms.nxapi.operators",
     "graphblas_algorithms.nxapi.shortest_paths",
     "graphblas_algorithms.nxapi.tests",
+    "graphblas_algorithms.nxapi.traversal",
     "graphblas_algorithms.tests",
     "graphblas_algorithms.utils",
 ]
 
 [tool.setuptools-git-versioning]
 enabled = true
 dev_template = "{tag}+{ccount}.g{sha}"
```

