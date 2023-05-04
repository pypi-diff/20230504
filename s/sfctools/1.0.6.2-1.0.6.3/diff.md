# Comparing `tmp/sfctools-1.0.6.2.tar.gz` & `tmp/sfctools-1.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.6.2.tar", max compression
+gzip compressed data, was "sfctools-1.0.6.3.tar", max compression
```

## Comparing `sfctools-1.0.6.2.tar` & `sfctools-1.0.6.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.2/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-04 18:18:23.188486 sfctools-1.0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.2/README.md
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.2/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.2/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.2/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.2/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.2/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.2/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.2/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.2/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.2/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.2/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.2/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.2/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.2/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.2/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.2/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.2/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.6.2/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.2/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.2/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.2/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.2/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.2/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.2/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.2/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.2/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.2/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.2/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.2/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.2/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.2/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.2/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.2/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.2/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.2/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.2/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-04 16:23:20.302674 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      414 2023-05-04 16:23:20.370337 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      416 2023-05-04 16:23:20.426339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      410 2023-05-04 16:23:20.481339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      410 2023-05-04 16:23:20.538339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      413 2023-05-04 16:23:20.597341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      410 2023-05-04 16:23:20.653341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      414 2023-05-04 16:23:20.708341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      415 2023-05-04 16:23:20.764341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      406 2023-05-04 16:23:20.820343 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      410 2023-05-04 16:23:20.877974 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-05-04 16:23:20.878347 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-04 16:23:20.878347 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.2/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.2/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.2/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.2/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.2/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.2/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.2/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.2/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.2/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.2/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.2/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.2/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.2/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.2/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.2/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.2/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.2/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.2/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.2/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-04 16:23:22.655503 sfctools-1.0.6.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.2/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.2/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.2/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.2/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.2/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.2/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.2/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.2/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.2/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.2/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-04 18:18:04.506385 sfctools-1.0.6.2/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.2/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.2/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.2/setup.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.3/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 18:41:55.106218 sfctools-1.0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.3/README.md
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.3/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.3/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.3/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.3/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.3/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.3/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.3/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.3/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.3/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.3/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.3/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.3/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.3/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.3/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.3/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.3/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15252 2023-05-04 18:38:24.098165 sfctools-1.0.6.3/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.3/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.3/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.3/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.3/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.3/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.3/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.3/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.3/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.3/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.3/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.3/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.3/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.3/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.3/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.3/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.3/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.3/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.3/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 18:39:36.198530 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      416 2023-05-04 18:39:36.258191 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.317192 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      417 2023-05-04 18:39:36.376193 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.434194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      413 2023-05-04 18:39:36.491194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      413 2023-05-04 18:39:36.550194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.605194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      410 2023-05-04 18:39:36.663195 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      411 2023-05-04 18:39:36.726197 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      418 2023-05-04 18:39:36.783222 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-05-04 18:39:36.784197 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 18:39:36.784722 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.3/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.3/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.3/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.3/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.3/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.3/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.3/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.3/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.3/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.3/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.3/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.3/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.3/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.3/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.3/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.3/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.3/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.3/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.3/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 18:39:38.676454 sfctools-1.0.6.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.3/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.3/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.3/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.3/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.3/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.3/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.3/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.3/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.3/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.3/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    21989 2023-05-04 18:34:38.291617 sfctools-1.0.6.3/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.3/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.3/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.3/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.3/PKG-INFO
```

### Comparing `sfctools-1.0.6.2/LICENSE` & `sfctools-1.0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/pyproject.toml` & `sfctools-1.0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.6.2"
+version = "1.0.6.3"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.6.2/README.md` & `sfctools-1.0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/__init__.py` & `sfctools-1.0.6.3/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/__main__.py` & `sfctools-1.0.6.3/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/automation/calibration.py` & `sfctools-1.0.6.3/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/automation/cgesolver.py` & `sfctools-1.0.6.3/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/automation/runner.py` & `sfctools-1.0.6.3/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/bottomup/matching.py` & `sfctools-1.0.6.3/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/bottomup/productiontree.py` & `sfctools-1.0.6.3/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.6.3/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/bottomup/treestruct.py` & `sfctools-1.0.6.3/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/core/agent.py` & `sfctools-1.0.6.3/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/core/clock.py` & `sfctools-1.0.6.3/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/core/flow_matrix.py` & `sfctools-1.0.6.3/sfctools/core/flow_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -358,29 +358,31 @@
         my_sankey_sink =  pd.DataFrame({"to":source2,
                                   "from":target2,
                                   "color_id":types2,
                                   "value":value2}).round(2)
 
         return my_sankey_source, my_sankey_sink
 
-    def plot_sankey(self,show_values=True, show_plot=True,colors=None):
+    def plot_sankey(self,show_values=True, show_plot=True,colors=None,label_rot=0.0,filling_fraction=0.85):
         """
         plots a sankey diagram of the flow matrix
 
         :param show_values: boolean switch to plot the values of the edge weights
         :param show_plot: show the plot as window? default True. If False, figure is returned instead.
         :param colors: (optional) a list of colors (if None, default colors are chosen)
+        :param label_rot: rotation of the labels 
+        :param filling_fraction: controls the 'thickness' of the Sankey bands
 
         :return fig: figure object
         """
         import matplotlib.pyplot as plt
         from ..misc.mpl_plotting import plot_sankey as sankey
 
         my_sankey_source,my_sankey_sink = self.convert_sankey_df()
-        fig = sankey([my_sankey_source,my_sankey_sink],show_values=show_values,show_plot=show_plot,colors=colors)
+        fig = sankey([my_sankey_source,my_sankey_sink],show_values=show_values,show_plot=show_plot,colors=colors,label_rot=label_rot,filling_fraction=filling_fraction)
         return fig
 
 
     @property
     def capital_flow_data(self):
         """'shortcut' property. only returns the data from the capital account"""
         return self._flow_data[Accounts.KA]
```

### Comparing `sfctools-1.0.6.2/sfctools/core/settings.py` & `sfctools-1.0.6.3/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/core/singleton.py` & `sfctools-1.0.6.3/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/core/world.py` & `sfctools-1.0.6.3/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/balance.py` & `sfctools-1.0.6.3/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.6.3/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.6.3/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/collection.py` & `sfctools-1.0.6.3/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/income_statement.py` & `sfctools-1.0.6.3/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/inventory.py` & `sfctools-1.0.6.3/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/market_registry.py` & `sfctools-1.0.6.3/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/signalslot.py` & `sfctools-1.0.6.3/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.6.3/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/__init__.py` & `sfctools-1.0.6.3/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/balance.py` & `sfctools-1.0.6.3/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.6.3/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/clock.py` & `sfctools-1.0.6.3/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/example_wrapper.py` & `sfctools-1.0.6.3/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.6.3/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/flowmatrix.py` & `sfctools-1.0.6.3/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/hello_agent.py` & `sfctools-1.0.6.3/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/inventory.py` & `sfctools-1.0.6.3/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/market_example/market.py` & `sfctools-1.0.6.3/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/market_example/market2.py` & `sfctools-1.0.6.3/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.6.3/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/order_book.py` & `sfctools-1.0.6.3/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/examples/signal_slot.py` & `sfctools-1.0.6.3/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.6.3/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/draw_widget.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.6.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.6.3/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/CLA.pdf` & `sfctools-1.0.6.3/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.6.3/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/LICENSE` & `sfctools-1.0.6.3/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/gui/README.md` & `sfctools-1.0.6.3/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.6.3/sfctools/misc/mpl_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,15 +421,16 @@
                 fontsize=10,
                 separation=0.8,
                 norm_factor=1.5,
                 min_width=0.1,
                 dy=10,
                 dx=55,
                 dx_space=8.5,
-                alpha=0.5):
+                alpha=0.5,
+                filling_fraction = 0.85):
     """
     plots a sankey diagram from data
 
     :param data: list of pandas dataframes, of the following format. length at least two.
     :param title: title of the plot
     :param show_plot: boolean switch to show plot window (default True). If False, figure is returned
     :param show_values: boolean switch to print numerical values of data as text label (default True)
@@ -438,14 +439,15 @@
     :param fontsize: size of label font
     :param separation: separation point of the label along the bands, between 0 and 1,
     :param norm_factor: normalization factor for width 
     :param min_width: minimum width of bands
     :param dy: vertical distance of bands
     :param dx: horizontal distance of bands
     :param dx_space: space between layers
+    :param filling_fraction: fraction by which the bands align (scaling with dy)
 
     :return fig: None or matplotlib figure
 
     Example: 
 
     +----------+----------+----------+-------------+
     |  from    |   to     |  value   | color_id    |
@@ -612,15 +614,15 @@
 
         for idx, row in layer.iterrows():
 
             fromnode = my_points[row["from"]]
             tonode = my_points[row["to"]]
             color_idx = row["color_id"]
 
-            my_band = Band(fromnode, tonode, w = float(row["value"])*norm_factor * dy * 0.2, color = colors[color_idx%len(colors)])
+            my_band = Band(fromnode, tonode, w = float(row["value"])*norm_factor * dy * (1-filling_fraction), color = colors[color_idx%len(colors)])
             
             bands[fromnode].append(my_band)
             bands[tonode].append(my_band)
 
         i += dx
 
         #for name,point in my_points.items():
```

### Comparing `sfctools-1.0.6.2/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.6.3/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/sfctools/misc/timeseries.py` & `sfctools-1.0.6.3/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.2/setup.py` & `sfctools-1.0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.6.2',
+    'version': '1.0.6.3',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.6.2/PKG-INFO` & `sfctools-1.0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.6.2
+Version: 1.0.6.3
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

