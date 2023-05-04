# Comparing `tmp/sfctools-1.0.5.8.tar.gz` & `tmp/sfctools-1.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.5.8.tar", max compression
+gzip compressed data, was "sfctools-1.0.5.9.tar", max compression
```

## Comparing `sfctools-1.0.5.8.tar` & `sfctools-1.0.5.9.tar`

### file list

```diff
@@ -1,121 +1,215 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.5.8/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-04 11:03:59.435555 sfctools-1.0.5.8/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.5.8/README.md
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.5.8/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.5.8/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.5.8/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.5.8/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.5.8/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.5.8/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.5.8/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.5.8/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.5.8/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.5.8/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.5.8/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.5.8/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.5.8/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.5.8/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.5.8/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.5.8/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.5.8/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.5.8/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.5.8/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.5.8/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.5.8/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.5.8/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.5.8/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.5.8/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.5.8/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.5.8/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.5.8/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.5.8/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.5.8/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.5.8/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.5.8/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.5.8/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.5.8/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.5.8/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.5.8/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.5.8/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.5.8/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.5.8/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.5.8/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.5.8/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.5.8/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.5.8/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.5.8/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.5.8/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    72504 2023-05-04 10:46:26.158680 sfctools-1.0.5.8/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.5.8/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.5.8/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.5.8/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.5.8/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.5.8/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.5.8/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.5.8/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.5.8/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.5.8/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-04 11:01:36.149057 sfctools-1.0.5.8/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.5.8/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.5.8/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.5.8/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.5.8/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.5.8/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.5.8/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.5.8/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.5.8/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.5.8/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.5.8/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    18645 2023-03-21 16:33:08.131566 sfctools-1.0.5.8/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.5.8/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.5.8/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.5.8/setup.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.5.9/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 12:04:03.789783 sfctools-1.0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.5.9/README.md
+-rw-r--r--   0        0        0       39 2023-01-26 10:19:31.537790 sfctools-1.0.5.9/sfctools/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-01-26 10:19:31.537845 sfctools-1.0.5.9/sfctools/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-01-26 10:19:31.536780 sfctools-1.0.5.9/sfctools/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-01-26 10:19:31.537845 sfctools-1.0.5.9/sfctools/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-01-26 10:19:31.539052 sfctools-1.0.5.9/sfctools/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.5.9/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.5.9/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.5.9/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0      177 2023-01-25 08:23:20.053567 sfctools-1.0.5.9/sfctools/automation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2023-01-19 21:54:26.523852 sfctools-1.0.5.9/sfctools/automation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8273 2023-01-25 08:23:20.054862 sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-311.pyc
+-rw-r--r--   0        0        0     4139 2023-01-19 21:54:26.530954 sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-38.pyc
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.5.9/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.5.9/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.5.9/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.5.9/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.5.9/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0      175 2023-01-25 08:23:19.248631 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      157 2023-01-19 21:54:25.705346 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13061 2023-01-25 08:23:19.475949 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-311.pyc
+-rw-r--r--   0        0        0     8647 2023-02-06 10:24:45.316244 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-38.pyc
+-rw-r--r--   0        0        0    11948 2023-01-25 08:16:32.088889 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc
+-rw-r--r--   0        0        0     8339 2023-01-25 08:23:19.250795 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     5937 2023-01-19 21:54:25.707915 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc
+-rw-r--r--   0        0        0     2863 2023-01-25 08:16:32.090879 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.5.9/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.5.9/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.5.9/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.5.9/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.5.9/sfctools/core/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-25 08:23:16.612109 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      153 2023-01-19 21:54:24.854116 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      153 2022-12-22 08:43:56.478191 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10127 2023-01-25 08:23:16.614415 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-311.pyc
+-rw-r--r--   0        0        0     7106 2023-01-19 21:54:24.857704 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-38.pyc
+-rw-r--r--   0        0        0     7096 2022-12-22 08:43:56.499523 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     3200 2023-01-25 08:23:17.901786 sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-311.pyc
+-rw-r--r--   0        0        0     2503 2023-01-19 21:54:25.148426 sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-38.pyc
+-rw-r--r--   0        0        0      856 2023-01-25 08:23:17.915777 sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc
+-rw-r--r--   0        0        0      677 2023-04-04 07:45:29.386549 sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc
+-rw-r--r--   0        0        0    19394 2023-01-25 08:23:19.254129 sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc
+-rw-r--r--   0        0        0    12090 2023-04-04 07:45:29.716546 sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc
+-rw-r--r--   0        0        0    13234 2023-01-25 08:23:19.211702 sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     8933 2023-04-04 07:45:29.692870 sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0        0        0     1482 2023-01-25 08:23:17.905919 sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-311.pyc
+-rw-r--r--   0        0        0     1091 2023-01-19 21:54:25.153899 sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-38.pyc
+-rw-r--r--   0        0        0     8862 2023-01-25 08:23:16.616906 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-311.pyc
+-rw-r--r--   0        0        0     5654 2023-02-06 10:24:44.695973 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-38.pyc
+-rw-r--r--   0        0        0     5547 2022-12-22 08:43:56.518896 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-39.pyc
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.5.9/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.5.9/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.5.9/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.5.9/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.5.9/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.5.9/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.5.9/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.5.9/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0      178 2023-01-25 08:23:16.618054 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      160 2023-01-19 21:54:24.869946 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      160 2022-12-22 08:43:56.522922 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    36033 2023-01-25 08:23:19.209700 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-311.pyc
+-rw-r--r--   0        0        0    22057 2023-04-04 07:45:29.687338 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-38.pyc
+-rw-r--r--   0        0        0    19951 2023-01-25 08:23:19.473688 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc
+-rw-r--r--   0        0        0    13962 2023-02-06 10:24:45.311852 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc
+-rw-r--r--   0        0        0     8905 2023-01-25 08:23:19.468631 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc
+-rw-r--r--   0        0        0     6617 2023-04-04 07:45:29.894931 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc
+-rw-r--r--   0        0        0     6937 2023-01-25 08:23:16.619099 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-311.pyc
+-rw-r--r--   0        0        0     4736 2023-01-19 21:54:24.876121 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-38.pyc
+-rw-r--r--   0        0        0     4718 2022-12-22 08:43:56.543068 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-39.pyc
+-rw-r--r--   0        0        0    18687 2023-01-25 08:23:19.466630 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc
+-rw-r--r--   0        0        0    13398 2023-01-19 21:54:25.920678 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc
+-rw-r--r--   0        0        0     8382 2023-01-25 08:23:20.048441 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc
+-rw-r--r--   0        0        0     5672 2023-01-19 21:54:26.507228 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc
+-rw-r--r--   0        0        0     6583 2023-01-25 08:23:20.050844 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc
+-rw-r--r--   0        0        0     5167 2023-01-19 21:54:26.513706 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc
+-rw-r--r--   0        0        0     8490 2023-01-25 08:23:19.471344 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc
+-rw-r--r--   0        0        0     6018 2023-01-19 21:54:25.936504 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc
+-rw-r--r--   0        0        0     5219 2023-01-25 08:23:20.052395 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc
+-rw-r--r--   0        0        0     3653 2023-01-19 21:54:26.519688 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.5.9/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.5.9/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.5.9/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.5.9/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.5.9/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.5.9/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.5.9/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.5.9/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.5.9/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.5.9/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.5.9/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.5.9/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.5.9/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.5.9/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.5.9/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.5.9/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.5.9/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.5.9/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0      269 2023-01-25 08:23:20.061472 sfctools-1.0.5.9/sfctools/gui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      221 2023-01-25 08:17:49.221422 sfctools-1.0.5.9/sfctools/gui/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2791 2023-01-25 08:23:20.063473 sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-311.pyc
+-rw-r--r--   0        0        0      835 2023-04-04 07:45:30.299298 sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-38.pyc
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.5.9/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.5.9/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0      177 2022-12-22 08:51:44.532604 sfctools-1.0.5.9/sfctools/gui/attune/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2022-11-23 08:49:18.431057 sfctools-1.0.5.9/sfctools/gui/attune/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.5.9/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0      181 2022-12-22 08:51:44.534815 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      163 2022-11-23 08:49:18.433350 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    50257 2023-01-25 08:23:24.448393 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc
+-rw-r--r--   0        0        0    20359 2023-04-04 07:45:31.111570 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    70418 2023-01-25 08:50:00.544297 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc
+-rw-r--r--   0        0        0    35485 2023-05-04 12:02:59.036460 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    16034 2023-01-25 08:23:21.221015 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc
+-rw-r--r--   0        0        0    10518 2023-05-04 09:43:05.888334 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    10890 2023-01-25 08:23:21.216723 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc
+-rw-r--r--   0        0        0     4813 2023-02-06 10:17:36.928510 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc
+-rw-r--r--   0        0        0    32862 2023-01-25 08:23:21.227665 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc
+-rw-r--r--   0        0        0    12521 2023-04-04 07:45:30.873144 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc
+-rw-r--r--   0        0        0     2435 2023-01-25 08:23:21.211969 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2023-04-04 07:45:30.862180 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc
+-rw-r--r--   0        0        0   152005 2023-01-25 08:47:50.827103 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc
+-rw-r--r--   0        0        0    69406 2023-05-04 09:43:04.168970 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc
+-rw-r--r--   0        0        0     7007 2023-01-25 08:23:24.383425 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc
+-rw-r--r--   0        0        0     6499 2022-11-23 08:49:30.377800 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc
+-rw-r--r--   0        0        0    10255 2023-01-25 08:23:24.459690 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     5060 2023-05-04 09:43:06.152185 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc
+-rw-r--r--   0        0        0    14167 2023-01-25 08:23:24.456539 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc
+-rw-r--r--   0        0        0     9595 2023-05-04 09:43:06.142977 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.5.9/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.5.9/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    74357 2023-05-04 12:03:31.938961 sfctools-1.0.5.9/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.5.9/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.5.9/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.5.9/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.5.9/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.5.9/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.5.9/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.5.9/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.5.9/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.5.9/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 12:02:59.053599 sfctools-1.0.5.9/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.5.9/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.5.9/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.5.9/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.5.9/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.5.9/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.5.9/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.5.9/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.5.9/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.5.9/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0     4765 2022-11-23 09:50:36.467143 sfctools-1.0.5.9/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.5.9/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-25 08:23:20.056190 sfctools-1.0.5.9/sfctools/misc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      153 2023-01-19 21:54:26.534886 sfctools-1.0.5.9/sfctools/misc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13145 2023-02-06 10:24:45.828385 sfctools-1.0.5.9/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc
+-rw-r--r--   0        0        0    10106 2023-01-25 08:23:20.059255 sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc
+-rw-r--r--   0        0        0     7616 2023-04-04 07:45:30.288586 sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc
+-rw-r--r--   0        0        0    12006 2023-01-25 08:23:21.230666 sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-311.pyc
+-rw-r--r--   0        0        0     6420 2023-01-25 08:17:49.793565 sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-38.pyc
+-rw-r--r--   0        0        0    18645 2023-03-21 16:33:08.131566 sfctools-1.0.5.9/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.5.9/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.5.9/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 sfctools-1.0.5.9/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.5.9/PKG-INFO
```

### Comparing `sfctools-1.0.5.8/LICENSE` & `sfctools-1.0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/pyproject.toml` & `sfctools-1.0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.5.8"
+version = "1.0.5.9"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.5.8/README.md` & `sfctools-1.0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/__init__.py` & `sfctools-1.0.5.9/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/__main__.py` & `sfctools-1.0.5.9/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/automation/calibration.py` & `sfctools-1.0.5.9/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/automation/cgesolver.py` & `sfctools-1.0.5.9/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/automation/runner.py` & `sfctools-1.0.5.9/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/bottomup/matching.py` & `sfctools-1.0.5.9/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/bottomup/productiontree.py` & `sfctools-1.0.5.9/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.5.9/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/bottomup/treestruct.py` & `sfctools-1.0.5.9/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/agent.py` & `sfctools-1.0.5.9/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/clock.py` & `sfctools-1.0.5.9/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/flow_matrix.py` & `sfctools-1.0.5.9/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/settings.py` & `sfctools-1.0.5.9/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/singleton.py` & `sfctools-1.0.5.9/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/core/world.py` & `sfctools-1.0.5.9/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/balance.py` & `sfctools-1.0.5.9/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.5.9/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.5.9/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/collection.py` & `sfctools-1.0.5.9/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/income_statement.py` & `sfctools-1.0.5.9/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/inventory.py` & `sfctools-1.0.5.9/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/market_registry.py` & `sfctools-1.0.5.9/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/signalslot.py` & `sfctools-1.0.5.9/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.5.9/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/__init__.py` & `sfctools-1.0.5.9/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/balance.py` & `sfctools-1.0.5.9/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.5.9/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/clock.py` & `sfctools-1.0.5.9/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/example_wrapper.py` & `sfctools-1.0.5.9/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.5.9/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/flowmatrix.py` & `sfctools-1.0.5.9/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/hello_agent.py` & `sfctools-1.0.5.9/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/inventory.py` & `sfctools-1.0.5.9/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/market_example/market.py` & `sfctools-1.0.5.9/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/market_example/market2.py` & `sfctools-1.0.5.9/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.5.9/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/order_book.py` & `sfctools-1.0.5.9/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/examples/signal_slot.py` & `sfctools-1.0.5.9/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.5.9/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/draw_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,24 +124,22 @@
         self.ishelper = ishelper
         self.is_support = is_support
         self.parent = parent
         self.n_connections = 0
 
         self.parent_widget = parent_widget
 
-
     @property
     def name(self):
         return self._name
     @name.setter
     def name(self,val):
         self._name = val
         self.label.name = val
 
-
     @property
     def x(self):
         return self._x
 
     @property
     def y(self):
         return self._y
@@ -402,15 +400,15 @@
         self.mousey = 0
 
         self.interpol_method = "quadratic"
         self.mode = "select"
 
         self.zoom_factor = 1.0
 
-        self.raster_size = 0.9
+        self.raster_size = 3.0 # 0.9
         self.show_raster = False
 
         self.show()
 
 
     def update_raster(self):
         # updates the raster settings
@@ -813,20 +811,20 @@
             x = -np.pi/2.0
 
         elif -np.pi <= x < -np.pi/2:
             x = -np.pi 
         
         return x         
 
-    def draw_arrow_at(self, qp, interpolated_points, md,offset_text=15, reverse = False, dashed=False):
+    def draw_arrow_at(self, qp, interpolated_points, md,offset_text=15, reverse = False, dashed=False,dd=5):
 
         mid_point = interpolated_points[md]
-        mid_point2 = interpolated_points[md+5]
+        mid_point2 = interpolated_points[md+dd]
         mid_points3 = interpolated_points[md-offset_text+1]
-        mid_points4 = interpolated_points[md-offset_text+1+10]
+        mid_points4 = interpolated_points[md-offset_text+1+2*dd]
 
         dy = mid_point[1] - mid_point2[1]
         dx = mid_point[0] - mid_point2[0]
 
         if reverse:
             dx = -dx 
             dy = -dy 
@@ -1062,62 +1060,104 @@
                 pass
             else:
                 points.append(points2[i])
 
         points = np.array(points)
         points = [(self.raster(t[0]), self.raster(t[1])) for t in points]
 
+        xt,yt = 0,0
         # Linear length along the line:
         try:
             distance = np.cumsum( np.sqrt(np.sum( np.diff(points, axis=0)**2, axis=1 )) )
             distance = np.insert(distance, 0, 0)/distance[-1]
 
             # Interpolation for different methods:
             #interpolations_methods = ['slinear', 'quadratic', 'cubic']
 
             if not self.show_raster:
-                if end_is_start:
+                if not end_is_start:
                     # method = "quadratic"
                     method  = self.interpol_method
                     alpha = np.linspace(0, 1, 40) # np.linspace(0, 1, 50)
+
+                    #for method in interpolations_methods:
+                    interpolator =  interp1d(distance, points, kind=method, axis=0)
+                    interpolated_points= interpolator(alpha)
+
                 else:
-                    method  = self.interpol_method
-                    alpha = np.linspace(0, 1, 60) #np.linspace(0, 1, 80)
+                    # method  = self.interpol_method
+                    # alpha = np.linspace(0, 1, 60) #np.linspace(0, 1, 80)
 
-                #for method in interpolations_methods:
-                interpolator =  interp1d(distance, points, kind=method, axis=0)
-                interpolated_points= interpolator(alpha)
+                    c0x = 0.5*(xi-x0)
+                    c0y = 0.5*(yi-y0) 
 
+                    r = 0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) 
+                    
+                    t0 = np.arctan2((yi-y0) ,(xi-x0))
+
+                    t = t0 + np.linspace(0,2*np.pi, 100)
+                    rx = r 
+                    ry = 0.7*r 
+
+                    x_coords = [rx * np.cos(ti) * np.cos(t0) - ry * np.sin(ti) * np.sin(t0) + c0x + x0 for ti in t]
+                    y_coords = [rx * np.cos(ti) * np.sin(t0) + ry* np.sin(ti) * np.cos(t0) + c0y + y0 for ti in t] 
+                    
+                    interpolated_points = list(zip(x_coords,y_coords))
+
+                
             else:
                 method = "linear"
                 alpha = np.linspace(0, 1, 5) # np.linspace(0, 1, 50)
                 #for method in interpolations_methods:
 
                 #for method in interpolations_methods:
                 interpolator =  interp1d(distance, points, kind=method, axis=0)
                 ip = interpolator(alpha)
 
                 x0 = points[0][0]
                 y0 = points[0][1]
                 xf = points[-1][0]
                 yf = points[-1][1]
 
-                xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,111)
-                xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,111)
-                xc3, yc3 = self.manhattan_lines(xd,yd,xf,yf,111) # 
+                # start_is_end = abs(x0 - xf) < 1e-6 and abs(y0 - yf) < 1e-6
 
-                x_coords = xc1 + xc2 + xc3
-                y_coords = yc1 + yc2 + yc3
+                if not end_is_start:
+                    # construct a line 
+                    xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,111)
+                    xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,111)
+
+                    xc3, yc3 = self.manhattan_lines(xd,yd,xf,yf,111) # 
+
+                    x_coords = xc1 + xc2 + xc3
+                    y_coords = yc1 + yc2 + yc3
+                else:
+                    # construct a circle with center point x0, y0 
+                    # through xi,yi 
+
+                    c0x = 0.5*(xi-x0)
+                    c0y = 0.5*(yi-y0) 
+
+                    r = 0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) 
+                    
+                    t0 = np.arctan2((yi-y0) ,(xi-x0))
+
+                    t = t0 + np.linspace(0,2*np.pi, 100)
+                    rx = r 
+                    ry = 0.7*r 
+
+                    x_coords = [rx * np.cos(ti) * np.cos(t0) - ry * np.sin(ti) * np.sin(t0) + c0x + x0 for ti in t]
+                    y_coords = [rx * np.cos(ti) * np.sin(t0) + ry* np.sin(ti) * np.cos(t0) + c0y + y0 for ti in t] 
+                    
+                    
+                    
                 interpolated_points = list(zip(x_coords,y_coords))
 
             # draw connector line as path
             n = len(interpolated_points)
 
-            interpolated_points = [(self.raster(t[0]), self.raster(t[1])) for t in interpolated_points]
-
             # print("interpolated_poitns",interpolated_points)
             # draw curved line
             offset_text = 20
 
             qp.setRenderHint(QPainter.Antialiasing)
 
             connPath = QPainterPath()
@@ -1137,29 +1177,33 @@
                 connPath.lineTo(self.zoom_factor*(interpolated_points[i][0]),self.zoom_factor*(interpolated_points[i][1]))
 
             connPath.moveTo(startx,starty)
 
             connPath.closeSubpath()
             qp.drawPath(connPath)
 
+            # interpolated_points = [(self.raster(t[0]), self.raster(t[1])) for t in interpolated_points]
+
             # draw arrow at midpoint
 
             md = int(n/2.)
             
             # interpolated_points = [(self.raster(p[0],50),self.raster(p[1],50)) for p in interpolated_points]
+            draw_reverse = False 
 
-            xt,yt = self.draw_arrow_at(qp,interpolated_points,md,dashed=dashed)
+            if not end_is_start:
+                xt, yt = self.draw_arrow_at(qp,interpolated_points,md,dashed=dashed)
             
-
             if not is_unidir: # double arrow for non-unidirectional
                 if not end_is_start and self.main_widget.checkBox.isChecked():
-                    
-                    md = int(n/2. - 40)
-                    
-                    xt,yt = self.draw_arrow_at(qp,interpolated_points,md, reverse=True,dashed=dashed)
+                    if not draw_reverse:
+                        md = int(n/2. - 40)                
+                        xt, yt = self.draw_arrow_at(qp,interpolated_points,md, reverse=True,dashed=dashed)
+
+                
 
                     
         except Exception as e:
             print("Error in Line Interpolation:",str(e))
             xt = 0
             yt = 0
 
@@ -2054,15 +2098,15 @@
         self.go_startx = self.gox
         self.go_starty = self.goy
 
         if self.mode == "drag_label":
 
             if self.selected is not None:
                 self.selected.x += self.selected.offx
-                self.selected.y += self.selected.offy
+                self.selected.y += self.selected.offy 
 
                 self.selected.offx = 0
                 self.selected.offy = 0
 
 
         if self.mode == "drag":
             x, y = event.pos().x(), event.pos().y()
@@ -2072,16 +2116,16 @@
             y = self.raster(int(y/self.zoom_factor),m)
 
             self.mousex = x
             self.mousey = y
 
             if self.selected is not None:
 
-                self.selected.x = self.mousex + self.offx # np.clip(self.mousex + self.offx,1-self.gox,2*self.maxx-self.gox)
-                self.selected.y = self.mousey + self.offy # np.clip(self.mousey + self.offy, 1-self.goy,2*self.maxy-self.goy)
+                self.selected.x = self.raster(self.mousex + self.offx ) # np.clip(self.mousex + self.offx,1-self.gox,2*self.maxx-self.gox)
+                self.selected.y = self.raster(self.mousey + self.offy ) # np.clip(self.mousey + self.offy, 1-self.goy,2*self.maxy-self.goy)
                 self.selected.x0 = self.selected.x
                 self.selected.y0 = self.selected.y
 
                 self.selected = None
             self.update()
 
         self.mode = "select"
```

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.5.9/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.5.9/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/CLA.pdf` & `sfctools-1.0.5.9/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.5.9/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/LICENSE` & `sfctools-1.0.5.9/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/gui/README.md` & `sfctools-1.0.5.9/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.5.9/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.5.9/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/sfctools/misc/timeseries.py` & `sfctools-1.0.5.9/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.8/setup.py` & `sfctools-1.0.5.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  'sfctools.gui',
  'sfctools.gui.attune',
  'sfctools.gui.attune.src',
  'sfctools.misc']
 
 package_data = \
 {'': ['*'],
+ 'sfctools': ['.pytest_cache/*', '.pytest_cache/v/cache/*'],
  'sfctools.examples': ['exampleabm/data/processed/*',
                        'exampleabm/data/raw/*',
                        'exampleabm/figures/*',
                        'monte_carlo/result/*'],
  'sfctools.gui': ['attune/src/styles/bright/*', 'attune/src/styles/dark/*']}
 
 install_requires = \
@@ -43,15 +44,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.5.8',
+    'version': '1.0.5.9',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.5.8/PKG-INFO` & `sfctools-1.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.5.8
+Version: 1.0.5.9
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

