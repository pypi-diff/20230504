# Comparing `tmp/datumaro-1.2.0rc3.tar.gz` & `tmp/datumaro-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.2.0rc3.tar", last modified: Wed Apr 19 00:50:44 2023, max compression
+gzip compressed data, was "datumaro-1.2.1.tar", last modified: Thu May  4 07:27:27 2023, max compression
```

## Comparing `datumaro-1.2.0rc3.tar` & `datumaro-1.2.1.tar`

### file list

```diff
@@ -1,312 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/commands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.169725 datumaro-1.2.0rc3/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.181725 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.185725 datumaro-1.2.0rc3/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89324 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.189725 datumaro-1.2.0rc3/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.189725 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.193724 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.197724 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.201725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/synthia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.205725 datumaro-1.2.0rc3/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    41240 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:50:44.165725 datumaro-1.2.0rc3/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 00:50:44.000000 datumaro-1.2.0rc3/datumaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:50:44.209725 datumaro-1.2.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-19 00:50:30.000000 datumaro-1.2.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.874663 datumaro-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   373252 2023-05-04 07:27:17.000000 datumaro-1.2.1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 07:27:17.000000 datumaro-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 07:27:17.000000 datumaro-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 07:27:17.000000 datumaro-1.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 07:27:27.874663 datumaro-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 07:27:17.000000 datumaro-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.826663 datumaro-1.2.1/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.826663 datumaro-1.2.1/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89332 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/synthia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.862663 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.862663 datumaro-1.2.1/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41240 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.874663 datumaro-1.2.1/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-04 07:27:17.000000 datumaro-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 07:27:17.000000 datumaro-1.2.1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-04 07:27:17.000000 datumaro-1.2.1/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:27:27.874663 datumaro-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-04 07:27:17.000000 datumaro-1.2.1/setup.py
```

### Comparing `datumaro-1.2.0rc3/3rd-party.txt` & `datumaro-1.2.1/3rd-party.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5782,14 +5782,15 @@
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
 
 -------------------------------------------------------------
+
 shapely
 
 BSD 3-Clause License
 
 Copyright (c) 2007, Sean C. Gillies. 2019, Casper van der Wel. 2007-2022, Shapely Contributors.
 All rights reserved.
 
@@ -6730,8 +6731,214 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 -------------------------------------------------------------
+
+pyarrow
+
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+-------------------------------------------------------------
+
 * Other names and brands may be claimed as the property of others.
```

### Comparing `datumaro-1.2.0rc3/LICENSE` & `datumaro-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/PKG-INFO` & `datumaro-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc3
+Version: 1.2.1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc3/README.md` & `datumaro-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/__init__.py` & `datumaro-1.2.1/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/capi/pybind.cpp` & `datumaro-1.2.1/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/__main__.py` & `datumaro-1.2.1/datumaro/cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         # Force-overwrite the log level and formatter
         log.root.setLevel(args.loglevel)
         for h in log.root.handlers:
             h.setFormatter(log.Formatter(log_format))
 
         # Suppress own deprecation warnings
         warnings.filterwarnings("ignore", category=DeprecationWarning, module=r"datumaro\..*")
+        # We don't use sklearn directly, but it yells out too much about its deprecations.
+        warnings.filterwarnings("ignore", category=DeprecationWarning, module=r"sklearn\..*")
 
     @staticmethod
     def _define_loglevel_option(parser):
         parser.add_argument(
             "--loglevel",
             type=loglevel,
             default="info",
@@ -110,15 +112,15 @@
     subcommands_desc = ""
     if known_contexts:
         subcommands_desc += "Contexts:\n"
         subcommands_desc += make_subcommands_help(known_contexts, help_line_start)
     if known_commands:
         if subcommands_desc:
             subcommands_desc += "\n"
-        subcommands_desc += "Basic Commands:\n"
+        subcommands_desc += "Context-free Commands:\n"
         subcommands_desc += make_subcommands_help(known_commands, help_line_start)
     if subcommands_desc:
         subcommands_desc += (
             "\nRun '%s COMMAND --help' for more information on a command." % parser.prog
         )
 
     subcommands = parser.add_subparsers(
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/__init__.py` & `datumaro-1.2.1/datumaro/cli/commands/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,47 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=redefined-builtin
 
-from . import convert, detect_format, download, explain, filter, generate, merge, patch, search
+from . import (
+    convert,
+    detect_format,
+    diff,
+    download,
+    explain,
+    explore,
+    filter,
+    generate,
+    info,
+    merge,
+    patch,
+    stats,
+    transform,
+    validate,
+)
 from .require_project import get_project_commands
 
 __all__ = [
     "get_non_project_commands",
     "get_project_commands",
 ]
 
 
 def get_non_project_commands():
     return [
         ("convert", convert, "Convert dataset between formats"),
-        ("detect-format", detect_format, "Detect the format of a dataset"),
+        ("detect", detect_format, "Detect the format of a dataset"),
+        ("diff", diff, "Compare datasets"),
+        ("dinfo", info, "Print dataset info"),
         ("download", download, "Download a publicly available dataset"),
         ("explain", explain, "Run Explainable AI algorithm for model"),
         ("filter", filter, "Filter dataset items"),
         ("generate", generate, "Generate synthetic dataset"),
         ("merge", merge, "Merge datasets"),
         ("patch", patch, "Update dataset from another one"),
-        ("search", search, "Search similar datasetitems of query"),
+        ("explore", explore, "Explore similar datasetitems of query"),
+        ("stats", stats, "Compute dataset statistics"),
+        ("transform", transform, "Modify dataset items"),
+        ("validate", validate, "Validate dataset"),
     ]
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/convert.py` & `datumaro-1.2.1/datumaro/cli/commands/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,15 +122,19 @@
                 "Multiple formats match the dataset: %s. "
                 "Try to specify format with '-if/--input-format' parameter.",
                 ", ".join(matches),
             )
             return 2
 
         fmt = matches[0]
-        log.info("Source dataset format detected as '%s'", args.input_format)
+        log.info(f"Source dataset format detected as {fmt}")
+
+    if fmt == args.output_format:
+        log.error("The source data format and the output data format is same as {fmt}.")
+        return 3
 
     source = osp.abspath(args.source)
 
     dst_dir = args.dst_dir
     if dst_dir:
         if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
             raise CliException(
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/detect_format.py` & `datumaro-1.2.1/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/download.py` & `datumaro-1.2.1/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/explain.py` & `datumaro-1.2.1/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/filter.py` & `datumaro-1.2.1/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/generate.py` & `datumaro-1.2.1/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/merge.py` & `datumaro-1.2.1/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/patch.py` & `datumaro-1.2.1/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/diff.py` & `datumaro-1.2.1/datumaro/cli/commands/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.operations import DistanceComparator, ExactComparator
 from datumaro.util import dump_json_file
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
-from ....util import MultilineFormatter
-from ....util.diff import DiffVisualizer
-from ....util.errors import CliException
-from ....util.project import generate_next_file_name, load_project, parse_full_revpath
+from ..util import MultilineFormatter
+from ..util.diff import DiffVisualizer
+from ..util.errors import CliException
+from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 class ComparisonMethod(Enum):
     equality = auto()
     distance = auto()
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/export.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/info.py` & `datumaro-1.2.1/datumaro/cli/commands/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import argparse
 
 from datumaro.components.annotation import AnnotationType
 from datumaro.components.errors import DatasetMergeError, MissingObjectError, ProjectNotFoundError
 from datumaro.util.scope import scope_add, scoped
 
-from ....util import MultilineFormatter
-from ....util.project import load_project, parse_full_revpath
+from ..util import MultilineFormatter
+from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Prints dataset overview",
         description="""
         Prints info about the dataset at <revpath>, or about the current
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/stats.py` & `datumaro-1.2.1/datumaro/cli/commands/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging as log
 
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.operations import compute_ann_statistics, compute_image_statistics
 from datumaro.util import dump_json_file, str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
-from ....util import MultilineFormatter
-from ....util.project import generate_next_file_name, load_project, parse_full_revpath
+from ..util import MultilineFormatter
+from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 __all__ = [
     "build_parser",
     "get_sensitive_args",
 ]
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/transform.py` & `datumaro-1.2.1/datumaro/cli/commands/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 from datumaro.components.environment import Environment
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.project import ProjectBuildTargets
 from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
-from ....util import MultilineFormatter
-from ....util.errors import CliException
-from ....util.project import load_project, parse_full_revpath
+from ..util import MultilineFormatter
+from ..util.errors import CliException
+from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     builtins = sorted(Environment().transforms)
 
     parser = parser_ctor(
         help="Transform project",
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/dataset_operations/validate.py` & `datumaro-1.2.1/datumaro/cli/commands/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from datumaro.components.environment import Environment
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.validator import TaskType
 from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
-from ....util import MultilineFormatter
-from ....util.errors import CliException
-from ....util.project import generate_next_file_name, load_project, parse_full_revpath
+from ..util import MultilineFormatter
+from ..util.errors import CliException
+from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Validate project",
         description="""
         Validates a dataset according to the task type and
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/commands/search.py` & `datumaro-1.2.1/datumaro/cli/commands/explore.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,107 +5,105 @@
 import argparse
 import logging as log
 import os.path as osp
 
 import numpy as np
 
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.components.searcher import Searcher
+from datumaro.components.explorer import Explorer
 from datumaro.components.visualizer import Visualizer
 from datumaro.util.image import save_image
-from datumaro.util.scope import scope_add
+from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
-        help="Search similar data of query in dataset",
+        help="Explore similar data of query in dataset",
         description="""
         Applies data exploration to a dataset for image/text query.
         The command can be useful if you have to find similar data in dataset.
         |n
         The current project (-p/--project) is used as a context for plugins
         and models. It is used when there is a dataset path in target.
         When not specified, the current project's working tree is used.|n
         |n
         Examples:|n
-        - Search top50 similar images of image query in COCO dataset:|n
+        - Explore top50 similar images of image query in COCO dataset:|n
         |s|s%(prog)s -q path/to/image.jpg -topk 50|n
-        - Search top50 similar images of text query, elephant, in COCO dataset:|n
+        - Explore top50 similar images of text query, elephant, in COCO dataset:|n
         |s|s%(prog)s -q elephant -topk 50|n
-        - Search top50 similar images of image query list in COCO dataset:|n
+        - Explore top50 similar images of image query list in COCO dataset:|n
         |s|s%(prog)s -q path/to/image1.jpg/ path/to/image2.jpg/ path/to/image3.jpg/ -topk 50|n
-        - Search top50 similar images of text query list in COCO dataset:|n
-        |s|s%(prog)s -q motorcycle/ bus/ train/ -topk 50|n
+        - Explore top50 similar images of text query list in COCO dataset:|n
+        |s|s%(prog)s -q motorcycle/ bus/ train/ -topk 50
         """,
         formatter_class=MultilineFormatter,
     )
 
     parser.add_argument(
         "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
     )  # workaround for -- eaten by positionals
-    parser.add_argument("target", nargs="?", default="project", help="Target dataset")
+    parser.add_argument("target", nargs="+", default="project", help="Target dataset")
     parser.add_argument(
         "-q",
         "--query",
         dest="query",
         required=True,
-        help="Image path or id of query to search similar data",
+        help="Image path or id of query to explore similar data",
     )
     parser.add_argument("-topk", type=int, dest="topk", help="Number of similar results")
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
         help="Directory of the project to operate on (default: current dir)",
     )
     parser.add_argument(
-        "-s", "--save", dest="save", default=True, help="Save searcher result as png"
+        "-s", "--save", dest="save", default=True, help="Save explorer result as png"
     )
 
-    parser.set_defaults(command=search_command)
+    parser.set_defaults(command=explore_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        search_command: [
+        explore_command: [
             "target",
             "query",
             "topk",
-            "project_dir",
             "save",
         ]
     }
 
 
-def search_command(args):
+@scoped
+def explore_command(args):
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
         if args.project_dir:
-            log.info(
-                f"Wrong argument: project_dir, {args.project_dir}, should be a path to project dir"
-            )
             raise
-    dataset, _ = parse_full_revpath(args.target, project)
 
-    searcher = Searcher(dataset)
+    dataset, _ = parse_full_revpath(args.target[0], project)
+
+    explorer = Explorer(dataset)
 
     # Get query datasetitem through query path
     if osp.exists(args.query):
         query_datasetitem = dataset.get_datasetitem_by_path(args.query)
     else:
         query_datasetitem = args.query
 
-    results = searcher.search_topk(query_datasetitem, args.topk)
+    results = explorer.explore_topk(query_datasetitem, args.topk)
 
     subset_list = []
     id_list = []
     result_path_list = []
     log.info("Most similar {} results of query in dataset".format(args.topk))
     for result in results:
         subset_list.append(result.subset)
@@ -117,10 +115,10 @@
     visualizer = Visualizer(dataset, figsize=(20, 20), alpha=0)
     fig = visualizer.vis_gallery(id_list, subset_list)
 
     if args.save:
         fig.canvas.draw()
         data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
         data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
-        save_image(osp.join("./searcher.png"), data, create_dir=True)
+        save_image(osp.join("./explorer.png"), data, create_dir=True)
 
     return 0
```

### Comparing `datumaro-1.2.0rc3/datumaro/cli/contexts/model.py` & `datumaro-1.2.1/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.2.1/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/contexts/source.py` & `datumaro-1.2.1/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/contexts/util.py` & `datumaro-1.2.1/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/util/__init__.py` & `datumaro-1.2.1/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/util/diff.py` & `datumaro-1.2.1/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/cli/util/project.py` & `datumaro-1.2.1/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/abstracts/merger.py` & `datumaro-1.2.1/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/algorithms/rise.py` & `datumaro-1.2.1/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/annotation.py` & `datumaro-1.2.1/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/annotations/matcher.py` & `datumaro-1.2.1/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/annotations/merger.py` & `datumaro-1.2.1/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/cli_plugin.py` & `datumaro-1.2.1/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/config.py` & `datumaro-1.2.1/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/config_model.py` & `datumaro-1.2.1/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/crypter.py` & `datumaro-1.2.1/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/dataset.py` & `datumaro-1.2.1/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/dataset_base.py` & `datumaro-1.2.1/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/dataset_item_storage.py` & `datumaro-1.2.1/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/environment.py` & `datumaro-1.2.1/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/errors.py` & `datumaro-1.2.1/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/exporter.py` & `datumaro-1.2.1/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/extractor_tfds.py` & `datumaro-1.2.1/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/filter.py` & `datumaro-1.2.1/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/format_detection.py` & `datumaro-1.2.1/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/generator.py` & `datumaro-1.2.1/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/hl_ops/__init__.py` & `datumaro-1.2.1/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/importer.py` & `datumaro-1.2.1/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/launcher.py` & `datumaro-1.2.1/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/media.py` & `datumaro-1.2.1/datumaro/components/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,17 +180,15 @@
         if callable(self._data):
             return self._data()
         return self._data
 
     @property
     def bytes(self) -> Optional[bytes]:
         if self.has_data:
-            if callable(self._data):
-                _bytes = self._data()
-            _bytes = self._data
+            _bytes = self._data() if callable(self._data) else self._data
             if isinstance(_bytes, bytes):
                 return _bytes
         return None
 
     @property
     def has_data(self) -> bool:
         return self._data is not None
```

### Comparing `datumaro-1.2.0rc3/datumaro/components/media_manager.py` & `datumaro-1.2.1/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/merge/__init__.py` & `datumaro-1.2.1/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/merge/base.py` & `datumaro-1.2.1/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/merge/exact_merge.py` & `datumaro-1.2.1/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/merge/intersect_merge.py` & `datumaro-1.2.1/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/merge/union_merge.py` & `datumaro-1.2.1/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/operations.py` & `datumaro-1.2.1/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/progress_reporting.py` & `datumaro-1.2.1/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/project.py` & `datumaro-1.2.1/datumaro/components/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1666,15 +1666,15 @@
                 except Exception as e:
                     if not skip_import_errors:
                         raise MigrationError(f"Failed to migrate the source '{name}'") from e
                     else:
                         log.warning(
                             f"Failed to migrate the source '{name}'. "
                             "Try to add this source manually with "
-                            "'datum import', once migration is finished. The "
+                            "'datum project import', once migration is finished. The "
                             "reason is: %s",
                             e,
                         )
                         new_project.remove_source(name, force=True, keep_data=False)
 
         old_dataset_dir = osp.join(src_dir, "dataset")
         if osp.isdir(old_dataset_dir):
```

### Comparing `datumaro-1.2.0rc3/datumaro/components/searcher.py` & `datumaro-1.2.1/datumaro/components/explorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,46 +7,46 @@
 import numpy as np
 
 from datumaro.components.annotation import HashKey
 from datumaro.components.dataset import IDataset
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.media import Image
-from datumaro.plugins.searcher import SearcherLauncher
+from datumaro.plugins.explorer import ExplorerLauncher
 
 
 def calculate_hamming(B1, B2):
     """
     :param B1:  vector [n]
     :param B2:  vector [r*n]
     :return: hamming distance [r]
     """
     q = B2.shape[1]  # max inner product value
     distH = 0.5 * (q - B1 @ B2.transpose())
     return distH
 
 
-class Searcher:
+class Explorer:
     def __init__(
         self,
         dataset: IDataset,
         topk: int = 10,
     ) -> None:
         """
-        Searcher for Datumaro dataitems
+        Explorer for Datumaro dataitems
 
         Parameters
         ----------
         dataset:
-            Datumaro dataset to search similar dataitem.
+            Datumaro dataset to explore similar dataitem.
         topk:
             Number of images.
         """
-        self._model = SearcherLauncher(model_name="clip_visual_ViT-B_32")
-        self._text_model = SearcherLauncher(model_name="clip_text_ViT-B_32")
+        self._model = ExplorerLauncher(model_name="clip_visual_ViT-B_32")
+        self._text_model = ExplorerLauncher(model_name="clip_text_ViT-B_32")
         inference = dataset.run_model(self._model, append_annotation=True)
         self._topk = topk
 
         database_keys = []
         item_list = []
 
         for item in inference:
@@ -59,21 +59,21 @@
                         item_list.append(item)
                     except Exception:
                         hash_key = None
 
         self._database_keys = database_keys
         self._item_list = item_list
 
-    def search_topk(
+    def explore_topk(
         self,
         query: Union[DatasetItem, str, List[DatasetItem], List[str]],
         topk: Optional[int] = None,
     ):
         """
-        Search topk similar results based on hamming distance for query DatasetItem
+        Explore topk similar results based on hamming distance for query DatasetItem
         """
         if not topk:
             topk = self._topk
 
         if all(i is None for i in self._database_keys):
             # media.data is None case
             raise ValueError("Database should have hash_key")
```

### Comparing `datumaro-1.2.0rc3/datumaro/components/shift_analyzer.py` & `datumaro-1.2.1/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/transformer.py` & `datumaro-1.2.1/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/validator.py` & `datumaro-1.2.1/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/components/visualizer.py` & `datumaro-1.2.1/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,29 +184,24 @@
         paths = pa_batches_decoder(batches, f"{parent}.path" if parent else "path")
         attributes_ = pa_batches_decoder(
             batches, f"{parent}.attributes" if parent else "attributes"
         )
         attributes_ = [DictMapper.backward(attributes)[0] for attributes in attributes_]
 
         images = []
-
-        def data_loader(path, idx):
-            options = {
-                "path": path if os.path.exists(path) else None,
-                "data": pa_batches_decoder(batches, f"{parent}.bytes" if parent else "bytes")[idx],
-            }
-            return cls.decode(**options)
-
         for idx, (path, attributes) in enumerate(zip(paths, attributes_)):
             if os.path.exists(path):
                 images.append(Image.from_file(path=path, size=attributes["size"]))
             else:
                 images.append(
                     Image.from_bytes(
-                        data=partial(data_loader, idx=idx, path=path), size=attributes["size"]
+                        data=lambda: pa_batches_decoder(
+                            batches, f"{parent}.bytes" if parent else "bytes"
+                        )[idx],
+                        size=attributes["size"],
                     )
                 )
         return images
 
 
 # TODO: share binary for extra images
 class PointCloudMapper(MediaElementMapper):
@@ -218,15 +213,15 @@
         cls, obj: PointCloud, encoder: Union[str, Callable[[PointCloud], bytes]] = "PNG"
     ) -> Dict[str, Any]:
         out = super().forward(obj)
 
         _bytes = None
         if isinstance(encoder, Callable):
             _bytes = encoder(obj)
-        else:
+        elif encoder != "NONE":
             _bytes = obj.data
         out["bytes"] = _bytes
 
         bytes_arr = bytearray()
         bytes_arr.extend(struct.pack("<I", len(obj.extra_images)))
         for img in obj.extra_images:
             bytes_arr.extend(
@@ -265,18 +260,14 @@
     def backward_from_batches(
         cls,
         batches: List[pa.lib.RecordBatch],
         parent: Optional[str] = None,
     ) -> List[PointCloud]:
         paths = pa_batches_decoder(batches, f"{parent}.path" if parent else "path")
 
-        def data_loader(idx):
-            data = pa_batches_decoder(batches, f"{parent}.bytes" if parent else "bytes")[idx]
-            return data
-
         def extra_images(idx):
             offset = 0
             attributes = pa_batches_decoder(
                 batches, f"{parent}.attributes" if parent else "attributes"
             )[idx]
             (len_extra_images,) = struct.unpack_from("<I", attributes, offset)
             offset += 4
@@ -294,12 +285,14 @@
                         path=path,
                         extra_images=partial(extra_images, idx=idx),
                     )
                 )
             else:
                 point_clouds.append(
                     PointCloud.from_bytes(
-                        data=partial(data_loader, idx=idx),
+                        data=lambda: pa_batches_decoder(
+                            batches, f"{parent}.bytes" if parent else "bytes"
+                        )[idx],
                         extra_images=partial(extra_images, idx=idx),
                     )
                 )
         return point_clouds
```

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -310,24 +310,36 @@
         group = ann.get("group")
         attributes = ann.get("attributes")
         return Label(label_id, attributes=attributes, group=group)
 
     def _load_items(self, parsed):
         for frame_id, item_desc in parsed.items():
             name = item_desc.get("name", "frame_%06d.png" % int(frame_id))
-            image = osp.join(self._images_dir, name)
+
+            image_path_opt_1 = osp.join(self._images_dir, name)
+            image_path_opt_2 = (
+                osp.join(self._images_dir, self._subset, name) if self._subset is not None else None
+            )
+            if osp.exists(image_path_opt_1):
+                image = image_path_opt_1
+            elif image_path_opt_2 and osp.exists(image_path_opt_2):
+                image = image_path_opt_2
+            elif "name" not in item_desc:
+                # If --use-track flag is on
+                # TODO: Revisit all the CVAT import/export parts.
+                image = image_path_opt_1
+            else:
+                raise DatasetImportError(f"Cannot find an image which has name={name}.")
+
             image_size = (item_desc.get("height"), item_desc.get("width"))
             if all(image_size):
                 image = Image.from_file(path=image, size=tuple(map(int, image_size)))
             else:
                 image = Image.from_file(path=image)
 
-            subset = item_desc.get("subset")
-            if subset is not None and subset != self._subset:
-                continue
             parsed[frame_id] = DatasetItem(
                 id=osp.splitext(name)[0],
                 subset=self._subset,
                 media=image,
                 annotations=item_desc.get("annotations"),
                 attributes={"frame": int(frame_id)},
             )
```

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mars.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mot.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mots.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/synthia.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/synthia.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/video.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/ndr.py` & `datumaro-1.2.1/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.2.1/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.2.1/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.2.1/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/searcher.py` & `datumaro-1.2.1/datumaro/plugins/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from tokenizers import Tokenizer
 
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.media import Image
 from datumaro.plugins.openvino_plugin.launcher import OpenvinoLauncher
 
 
-class SearcherLauncher(OpenvinoLauncher):
+class ExplorerLauncher(OpenvinoLauncher):
     def __init__(
         self,
         description=None,
         weights=None,
         interpreter=None,
         model_dir=None,
         model_name=None,
```

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/shift_analyzer.py` & `datumaro-1.2.1/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/splitter.py` & `datumaro-1.2.1/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.2.1/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.2.1/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.2.1/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.2.1/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/tiling/tile.py` & `datumaro-1.2.1/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/tiling/util.py` & `datumaro-1.2.1/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/transforms.py` & `datumaro-1.2.1/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/plugins/validators.py` & `datumaro-1.2.1/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/__init__.py` & `datumaro-1.2.1/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/annotation_util.py` & `datumaro-1.2.1/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/attrs_util.py` & `datumaro-1.2.1/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/file_utils.py` & `datumaro-1.2.1/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/image.py` & `datumaro-1.2.1/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/image_cache.py` & `datumaro-1.2.1/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/log_utils.py` & `datumaro-1.2.1/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/mask_tools.py` & `datumaro-1.2.1/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/meta_file_util.py` & `datumaro-1.2.1/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/os_util.py` & `datumaro-1.2.1/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/pickle_util.py` & `datumaro-1.2.1/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/scope.py` & `datumaro-1.2.1/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/telemetry_stub.py` & `datumaro-1.2.1/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro/util/telemetry_utils.py` & `datumaro-1.2.1/datumaro/util/telemetry_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 NO_TELEMETRY_KEY = "DATUMARO_NO_OV_TELEMETRY"
 
 
 def _get_action_name(command):
     # TODO: We should clean these nonsense if-else branches.
     if command is commands.require_project.versioning.info.info_command:
         return "project_info_result"
-    elif command is commands.require_project.dataset_operations.stats.stats_command:
+    elif command is commands.stats.stats_command:
         return "project_stats_result"
     elif command is contexts.project.migrate_command:
         return "project_migrate_result"
-    elif command is commands.require_project.dataset_operations.export.export_command:
+    elif command is commands.require_project.modification.export.export_command:
         return "project_export_result"
-    elif command is commands.require_project.dataset_operations.validate.validate_command:
+    elif command is commands.validate.validate_command:
         return "project_validate_result"
     elif command is commands.filter.filter_command:
         return "project_filter_result"
-    elif command is commands.require_project.dataset_operations.transform.transform_command:
+    elif command is commands.transform.transform_command:
         return "project_transform_result"
     elif command is commands.require_project.modification.import_.import_command:
         return "source_add_result"
     elif command is commands.require_project.modification.remove.remove_command:
         return "source_remove_result"
     elif command is contexts.source.info_command:
         return "source_info_result"
@@ -55,21 +55,21 @@
         return "checkout_result"
     elif command is commands.require_project.versioning.commit.commit_command:
         return "commit_result"
     elif command is commands.convert.convert_command:
         return "convert_result"
     elif command is commands.require_project.modification.create.create_command:
         return "create_result"
-    elif command is commands.require_project.dataset_operations.diff.diff_command:
+    elif command is commands.diff.diff_command:
         return "diff_result"
     elif command is commands.explain.explain_command:
         return "explain_result"
     elif command is commands.generate.generate_command:
         return "generate_result"
-    elif command is commands.require_project.dataset_operations.info.info_command:
+    elif command is commands.info.info_command:
         return "info_result"
     elif command is commands.require_project.versioning.log.log_command:
         return "log_result"
     elif command is commands.merge.merge_command:
         return "merge_result"
     elif command is commands.patch.patch_command:
         return "patch_result"
```

### Comparing `datumaro-1.2.0rc3/datumaro/util/tf_util.py` & `datumaro-1.2.1/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/datumaro.egg-info/PKG-INFO` & `datumaro-1.2.1/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc3
+Version: 1.2.1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc3/datumaro.egg-info/SOURCES.txt` & `datumaro-1.2.1/datumaro.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,32 +21,31 @@
 datumaro.egg-info/top_level.txt
 datumaro/capi/pybind.cpp
 datumaro/cli/__init__.py
 datumaro/cli/__main__.py
 datumaro/cli/commands/__init__.py
 datumaro/cli/commands/convert.py
 datumaro/cli/commands/detect_format.py
+datumaro/cli/commands/diff.py
 datumaro/cli/commands/download.py
 datumaro/cli/commands/explain.py
+datumaro/cli/commands/explore.py
 datumaro/cli/commands/filter.py
 datumaro/cli/commands/generate.py
+datumaro/cli/commands/info.py
 datumaro/cli/commands/merge.py
 datumaro/cli/commands/patch.py
-datumaro/cli/commands/search.py
+datumaro/cli/commands/stats.py
+datumaro/cli/commands/transform.py
+datumaro/cli/commands/validate.py
 datumaro/cli/commands/require_project/__init__.py
-datumaro/cli/commands/require_project/dataset_operations/__init__.py
-datumaro/cli/commands/require_project/dataset_operations/diff.py
-datumaro/cli/commands/require_project/dataset_operations/export.py
-datumaro/cli/commands/require_project/dataset_operations/info.py
-datumaro/cli/commands/require_project/dataset_operations/stats.py
-datumaro/cli/commands/require_project/dataset_operations/transform.py
-datumaro/cli/commands/require_project/dataset_operations/validate.py
 datumaro/cli/commands/require_project/modification/__init__.py
 datumaro/cli/commands/require_project/modification/add.py
 datumaro/cli/commands/require_project/modification/create.py
+datumaro/cli/commands/require_project/modification/export.py
 datumaro/cli/commands/require_project/modification/import_.py
 datumaro/cli/commands/require_project/modification/remove.py
 datumaro/cli/commands/require_project/versioning/__init__.py
 datumaro/cli/commands/require_project/versioning/checkout.py
 datumaro/cli/commands/require_project/versioning/commit.py
 datumaro/cli/commands/require_project/versioning/info.py
 datumaro/cli/commands/require_project/versioning/log.py
@@ -67,27 +66,27 @@
 datumaro/components/config_model.py
 datumaro/components/crypter.py
 datumaro/components/dataset.py
 datumaro/components/dataset_base.py
 datumaro/components/dataset_item_storage.py
 datumaro/components/environment.py
 datumaro/components/errors.py
+datumaro/components/explorer.py
 datumaro/components/exporter.py
 datumaro/components/extractor_tfds.py
 datumaro/components/filter.py
 datumaro/components/format_detection.py
 datumaro/components/generator.py
 datumaro/components/importer.py
 datumaro/components/launcher.py
 datumaro/components/media.py
 datumaro/components/media_manager.py
 datumaro/components/operations.py
 datumaro/components/progress_reporting.py
 datumaro/components/project.py
-datumaro/components/searcher.py
 datumaro/components/shift_analyzer.py
 datumaro/components/transformer.py
 datumaro/components/validator.py
 datumaro/components/visualizer.py
 datumaro/components/abstracts/__init__.py
 datumaro/components/abstracts/merger.py
 datumaro/components/algorithms/__init__.py
@@ -100,16 +99,16 @@
 datumaro/components/hl_ops/__init__.py
 datumaro/components/merge/__init__.py
 datumaro/components/merge/base.py
 datumaro/components/merge/exact_merge.py
 datumaro/components/merge/intersect_merge.py
 datumaro/components/merge/union_merge.py
 datumaro/plugins/__init__.py
+datumaro/plugins/explorer.py
 datumaro/plugins/ndr.py
-datumaro/plugins/searcher.py
 datumaro/plugins/shift_analyzer.py
 datumaro/plugins/splitter.py
 datumaro/plugins/transforms.py
 datumaro/plugins/validators.py
 datumaro/plugins/accuracy_checker_plugin/__init__.py
 datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
 datumaro/plugins/accuracy_checker_plugin/details/__init__.py
@@ -228,14 +227,24 @@
 datumaro/plugins/data_formats/yolo/__init__.py
 datumaro/plugins/data_formats/yolo/base.py
 datumaro/plugins/data_formats/yolo/exporter.py
 datumaro/plugins/data_formats/yolo/format.py
 datumaro/plugins/data_formats/yolo/importer.py
 datumaro/plugins/openvino_plugin/__init__.py
 datumaro/plugins/openvino_plugin/launcher.py
+datumaro/plugins/openvino_plugin/samples/__init__.py
+datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
 datumaro/plugins/sampler/__init__.py
 datumaro/plugins/sampler/random_sampler.py
 datumaro/plugins/sampler/relevancy_sampler.py
 datumaro/plugins/synthetic_data/__init__.py
 datumaro/plugins/synthetic_data/background_colors.txt
 datumaro/plugins/synthetic_data/image_generator.py
 datumaro/plugins/synthetic_data/utils.py
```

### Comparing `datumaro-1.2.0rc3/datumaro.egg-info/requires.txt` & `datumaro-1.2.1/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/pyproject.toml` & `datumaro-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/requirements-core.txt` & `datumaro-1.2.1/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc3/setup.py` & `datumaro-1.2.1/setup.py`

 * *Files identical despite different names*

