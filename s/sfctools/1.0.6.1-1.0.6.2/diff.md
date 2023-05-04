# Comparing `tmp/sfctools-1.0.6.1.tar.gz` & `tmp/sfctools-1.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.6.1.tar", max compression
+gzip compressed data, was "sfctools-1.0.6.2.tar", max compression
```

## Comparing `sfctools-1.0.6.1.tar` & `sfctools-1.0.6.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.1/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-04 16:22:46.302449 sfctools-1.0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.1/README.md
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.1/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.1/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.1/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.1/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.1/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.1/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.1/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.1/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.1/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.1/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.1/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.1/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.1/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.1/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.1/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.1/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.6.1/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.1/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.1/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.1/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.1/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.1/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.1/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.1/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.1/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.1/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.1/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.1/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.1/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.1/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.1/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.1/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.1/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.1/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.1/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.1/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.1/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.1/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.1/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.1/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.1/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.1/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.1/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.1/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.1/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.1/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.1/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.1/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.1/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.1/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.1/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.1/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.1/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.1/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.1/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.1/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.1/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.1/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.1/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.1/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.1/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.1/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.1/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.1/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.1/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.1/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.1/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.1/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.1/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.1/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.1/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.1/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.1/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.1/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.1/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.1/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-04 12:11:57.367531 sfctools-1.0.6.1/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.1/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.1/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.1/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.1/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.1/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.1/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.1/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.1/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.1/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.1/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    19072 2023-05-04 16:21:50.341351 sfctools-1.0.6.1/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.1/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.1/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.1/setup.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.2/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 18:18:23.188486 sfctools-1.0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.2/README.md
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.2/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.2/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.2/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.2/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.2/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.2/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.2/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.2/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.2/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.2/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.2/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.2/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.2/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.2/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.2/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.2/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.6.2/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.2/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.2/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.2/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.2/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.2/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.2/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.2/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.2/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.2/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.2/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.2/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.2/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.2/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.2/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.2/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.2/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.2/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.2/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.2/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.2/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.2/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 16:23:20.302674 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      414 2023-05-04 16:23:20.370337 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      416 2023-05-04 16:23:20.426339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      410 2023-05-04 16:23:20.481339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      410 2023-05-04 16:23:20.538339 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      413 2023-05-04 16:23:20.597341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      410 2023-05-04 16:23:20.653341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      414 2023-05-04 16:23:20.708341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      415 2023-05-04 16:23:20.764341 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      406 2023-05-04 16:23:20.820343 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      410 2023-05-04 16:23:20.877974 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-05-04 16:23:20.878347 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 16:23:20.878347 sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.2/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.2/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.2/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.2/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.2/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.2/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.2/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.2/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.2/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.2/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.2/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.2/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.2/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.2/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.2/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.2/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.2/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.2/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.2/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.2/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.2/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 16:23:22.655503 sfctools-1.0.6.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.2/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.2/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.2/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.2/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.2/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.2/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.2/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.2/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.2/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.2/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    21848 2023-05-04 18:18:04.506385 sfctools-1.0.6.2/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.2/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.2/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.2/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.2/PKG-INFO
```

### Comparing `sfctools-1.0.6.1/LICENSE` & `sfctools-1.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/pyproject.toml` & `sfctools-1.0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.6.1"
+version = "1.0.6.2"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.6.1/README.md` & `sfctools-1.0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/__init__.py` & `sfctools-1.0.6.2/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/__main__.py` & `sfctools-1.0.6.2/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/automation/calibration.py` & `sfctools-1.0.6.2/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/automation/cgesolver.py` & `sfctools-1.0.6.2/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/automation/runner.py` & `sfctools-1.0.6.2/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/bottomup/matching.py` & `sfctools-1.0.6.2/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/bottomup/productiontree.py` & `sfctools-1.0.6.2/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.6.2/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/bottomup/treestruct.py` & `sfctools-1.0.6.2/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/agent.py` & `sfctools-1.0.6.2/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/clock.py` & `sfctools-1.0.6.2/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/flow_matrix.py` & `sfctools-1.0.6.2/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/settings.py` & `sfctools-1.0.6.2/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/singleton.py` & `sfctools-1.0.6.2/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/core/world.py` & `sfctools-1.0.6.2/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/balance.py` & `sfctools-1.0.6.2/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.6.2/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.6.2/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/collection.py` & `sfctools-1.0.6.2/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/income_statement.py` & `sfctools-1.0.6.2/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/inventory.py` & `sfctools-1.0.6.2/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/market_registry.py` & `sfctools-1.0.6.2/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/signalslot.py` & `sfctools-1.0.6.2/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.6.2/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/__init__.py` & `sfctools-1.0.6.2/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/balance.py` & `sfctools-1.0.6.2/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.6.2/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/clock.py` & `sfctools-1.0.6.2/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/example_wrapper.py` & `sfctools-1.0.6.2/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.6.2/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/flowmatrix.py` & `sfctools-1.0.6.2/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/hello_agent.py` & `sfctools-1.0.6.2/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/inventory.py` & `sfctools-1.0.6.2/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/market_example/market.py` & `sfctools-1.0.6.2/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/market_example/market2.py` & `sfctools-1.0.6.2/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.6.2/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.6.2/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/order_book.py` & `sfctools-1.0.6.2/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/examples/signal_slot.py` & `sfctools-1.0.6.2/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.6.2/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/draw_widget.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.6.2/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.6.2/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.6.2/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/CLA.pdf` & `sfctools-1.0.6.2/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.6.2/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/LICENSE` & `sfctools-1.0.6.2/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/gui/README.md` & `sfctools-1.0.6.2/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.6.2/sfctools/misc/mpl_plotting.py`

 * *Files 11% similar despite different names*

```diff
@@ -320,15 +320,15 @@
     spline = partial(casteljau,b0=b0,b1=b1,b2=b2,b3=b3)
 
     b = np.array([spline(t) for t in tarr])
 
     return b[:,0],b[:,1]
 
 
-def band(pstart: Point, pend: Point, npoints=100,curv=None, weight=2):
+def plot_band(pstart: Point, pend: Point, npoints=100,curv=None, weight=2):
     """
     computes a band of two bezier curves
 
     :param pstart: starting point of the bezier curve
     :param pend: end point of the bezier curve
     :param npoints: number of discrete points to retrun
     :param curv: optionally you can give a curvature parameter here (float) default None
@@ -337,26 +337,26 @@
     :return: x,y1,y2 coordinate 3-tuple of the band
     """
 
     w = weight # width of the band
     d = 0 # horizontal shift of the bands realtive to each other
     e = 0 # distance of  '<' and '>' arc
 
-    qstart1 = Point(pstart.x-d,pstart.y+1)
-    qstart2 = Point(pstart.x-d,pstart.y-1)
+    qstart1 = Point(pstart.x-d,pstart.y)
+    qstart2 = Point(pstart.x-d,pstart.y)
 
     qend  = Point(pend.x-d,pend.y)
     qend1  = Point(pend.x-d,pend.y)
     qend2  = Point(pend.x-d,pend.y)
 
-    pstart1 = Point(pstart.x-d+.2*e,pstart.y+w)
-    pend1 = Point(pend.x-d-e,pend.y+w)
+    pstart1 = Point(pstart.x-d+.2*e,pstart.y)
+    pend1 = Point(pend.x-d-e,pend.y)
 
-    pstart2 = Point(pstart.x+d+.2*e,pstart.y-w)
-    pend2 = Point(pend.x+d-e,pend.y-w)
+    pstart2 = Point(pstart.x+d+.2*e,pstart.y+w)
+    pend2 = Point(pend.x+d-e,pend.y+w)
 
     bezier_start1 = bezier(qstart1,pstart1)
     bezier_start2 = bezier(qstart2,pstart2)
 
     bezier_end1 = bezier(pend1,pend1)
     bezier_end2 = bezier(pend2,pend2)
 
@@ -378,51 +378,58 @@
 def draw_band(fig,pstart:Point, pend:Point, color="blue",alpha=.9,weight=2,norm=1.0,show_label=True,label=None,dv=0.6,rotation=0):
     """
     draw a band graphically
 
     """
     x,y1,y2 = band(pstart,pend,weight=weight)
     plt.fill_between(x,y1,y2,color=color,figure=fig,alpha=alpha)
+    
+    my_bez_x, my_bez_y = bezier(Point(pstart.x, pstart.y), Point(pend.x, pend.y))
+    
+    plt.plot(my_bez_x, my_bez_y, color="black",alpha=.7) # "black")
 
     if show_label and label is not None:
         # draw bezier
-        my_bez_x, my_bez_y = bezier(Point(pstart.x, pstart.y), Point(pend.x, pend.y))
+        
         # dv = 0.6
         bx = my_bez_x[int(dv*len(my_bez_x))]
         by = my_bez_y[int(dv*len(my_bez_y))]
 
-        # plt.plot(my_bez_x, my_bez_y, color="black")
-
+        
         #bx2,by2 = casteljau(t=0.55,b0=np.array([pstart.x,pstart.y]),b1=b1,b2=b2,b3=np.array([pend.x,pend.y]))
         #bx3,by3 = casteljau(t=0.66,b0=np.array([pstart.x,pstart.y]),b1=b1,b2=b2,b3=np.array([pend.x,pend.y]))
         #rot = (90-.5*np.arctan2((bx3-bx2),(by3-by2))*180.0/np.pi)%360.0 # compute slope at point
         #rot = 0
 
         bbox = {'pad': 2, 'facecolor': color,'edgecolor':color,'linewidth':.0}
         props = {'ha': 'center', 'va': 'center', 'bbox': bbox}
 
         if label is not None:
             plt.gca().text(bx,by - .0, label, props, rotation=rotation,color="white", alpha=alpha)
         else:
             plt.gca().text(bx,by , "%.2f" %(weight/norm), props, rotation=rotation,color="black",alpha=alpha)
+
+        
         # plt.annotate(str(weight),(bx,by),color="gray",alpha=alpha)
 
     pend.offset_y += 1.5*weight
     pstart.offset_y += 1.5*weight
 
 def plot_sankey(data,title="",show_plot=True,
                 show_values=True,
                 colors=None,
                 label_rot=65,
                 fontsize=10,
                 separation=0.8,
                 norm_factor=1.5,
                 min_width=0.1,
                 dy=10,
-                dx=55):
+                dx=55,
+                dx_space=8.5,
+                alpha=0.5):
     """
     plots a sankey diagram from data
 
     :param data: list of pandas dataframes, of the following format. length at least two.
     :param title: title of the plot
     :param show_plot: boolean switch to show plot window (default True). If False, figure is returned
     :param show_values: boolean switch to print numerical values of data as text label (default True)
@@ -430,14 +437,15 @@
     :param label_rot: rotation of the labels (default 65 degrees)
     :param fontsize: size of label font
     :param separation: separation point of the label along the bands, between 0 and 1,
     :param norm_factor: normalization factor for width 
     :param min_width: minimum width of bands
     :param dy: vertical distance of bands
     :param dx: horizontal distance of bands
+    :param dx_space: space between layers
 
     :return fig: None or matplotlib figure
 
     Example: 
 
     +----------+----------+----------+-------------+
     |  from    |   to     |  value   | color_id    |
@@ -465,18 +473,18 @@
 
     if not isinstance(data,list):
         data = [data] # convert to list
 
     if colors is None:
         colors = [
             "lightgray",
-            "royalblue",
-            "tomato",
-            "limegreen",
-            "indigo",
+            "skyblue",
+            "wheat",
+            "lightgreen",
+            "lavender",
         ]
     
     # 1. normalize the values to reasonable width of bands
 
     # norm_factor = 1.5 #normalization factor for width
 
     maxval = 0.0
@@ -500,76 +508,166 @@
 
     i = 10  #
     j0 = 6 # < starting position (i,j)
 
     # dy = 10 # 8  # vertical distance of bands
     # dx = 55 #   # horizontal distance of layers
 
-    dx_space = 2.5 # white space between layers
+    # dx_space = 2.5 # white space between layers
 
     # define some points for the unique nodes
     my_points = {} # keys will be names, value will be Points
     my_labels = {} # keys will be names, value will be Labels
     my_values = {} # labels for values
 
     last_j = j0
 
     # iterate through the dataframes
-    for indx,layer in enumerate(data):
+    # heights = defaultdict(lambda: 0 )
+
+    
+    class Band:
+    
 
-        j = last_j
+            instances = [] 
+            def __init__(self,n_from,n_to,w,color="steelblue"):
+                self.n_from = n_from 
+                self.n_to = n_to 
+                self.shift_y =0.0 
+                self.width =  2* w
+                self.osy1 = 0.0
+                self.osy2 = 0.0
+                self.color = color
+                self.__class__.instances.append(self) 
+
+            def plot(self):
+                fromnode = self.n_from 
+                tonode = self.n_to
+                w = self.width
+                osy1 = self.osy1
+                osy2 = self.osy2
+                
+                #vals_lower = [fromnode.y+osy1,tonode.y+osy2]
+                #vals_upper = [fromnode.y+osy1 + w,tonode.y+osy2 + w]
+
+                point_lower1 = Point(fromnode.x,fromnode.y+osy1)
+                point_lower2  = Point(tonode.x, tonode.y + osy2)
+                # point_lower2 = Point(fromnode.x,fromnode.y+osy1+w)
+
+                # make the curves more smooth 
+                x, vals_lower, vals_upper = plot_band(point_lower1, point_lower2,weight=w)
+                plt.fill_between(x, vals_lower, vals_upper,color=self.color)
+                
+                
+            def maxy(self):
+                w = 2 * self.width 
+                return max([self.n_from.y+ self.osy1 + w, self.n_to.y+ self.osy2 + w])
+            
+
+   
+
+    from collections import defaultdict
+    bands = defaultdict(lambda: [])
+
+    
+    for indx, layer in enumerate(data):
+
+        j =  j0 
+
+        k = 0
         for name in layer["from"].unique():
 
             if name not in my_points:
                 new_point = Point(i+dx_space,j)
                 my_points[name] = new_point
 
+                j += dy
+
             if name not in my_labels:
                 my_labels[name] = Label(new_point.x-5.2,new_point.y-.2,name) # plt.annotate(name,(new_point.x-1.8, new_point.y-.1))
             else:
 
                 my_labels[name].shift_up()
 
-            j+= dy
+            k+=1
 
         j = j0
+
+        k = 0
         for name in layer["to"].unique():
 
             if name not in my_points:
                 new_point = Point(i+dx,j)
                 my_points[name] = new_point #Point(i+dx,j)
 
+                j += dy 
+
             if name not in my_labels:
                 my_labels[name] = Label(new_point.x+.5*dx_space,new_point.y-.2,name) # plt.annotate(name,(new_point.x+.5*dx_space,new_point.y-.1))
             else:
                 my_labels[name].shift_up()
-            #else:
-                #if indx != len(data)-1:
-                #    my_labels[name].shift_up()
-
-            j+= dy
+            
+            k += 1
 
         last_j = j - dy
 
+        for idx, row in layer.iterrows():
+
+            fromnode = my_points[row["from"]]
+            tonode = my_points[row["to"]]
+            color_idx = row["color_id"]
+
+            my_band = Band(fromnode, tonode, w = float(row["value"])*norm_factor * dy * 0.2, color = colors[color_idx%len(colors)])
+            
+            bands[fromnode].append(my_band)
+            bands[tonode].append(my_band)
+
         i += dx
 
-        for name,point in my_points.items():
-            point.offset_y = 0
+        #for name,point in my_points.items():
+        #    point.offset_y = 0
 
         # iterate through the dataframe rows
-        for idx,row in layer.iterrows():
+
+
+        for point, b in bands.items():
+             
+            offset1 = 0.0 
+            offset2 = 0.0 
+
+            for bi in b:
+
+                if point == bi.n_from:
+                    bi.osy1 = offset1
+                    offset1 += bi.width 
+
+                elif point == bi.n_to:
+                    bi.osy2 = offset2
+                    offset2 += bi.width 
+          
+
+        # plot all bands 
+        for band in Band.instances:
+            band.plot()
+
+        """
+        for idx, row in layer.iterrows():
 
             color_idx = int(row["color_id"]) # index for color map
 
             fromnode = my_points[row["from"]]
             tonode = my_points[row["to"]]
-            weight = max(min_width,float(row["value"])*norm_factor) # <- make bars thicker
+            weight = float(row["value"])*norm_factor # 8.5e-2 #  max(min_width,float(row["value"])*norm_factor) # <- make bars thicker
 
             draw_band(fig,fromnode,tonode,colors[color_idx%len(colors)],weight=weight,norm=norm_factor,show_label=show_values,rotation=0,dv=separation,label=str(row["value"]))
 
+            # update weight for next layer
+        """
+
+
     for label in my_labels.values(): # draw the labels here...
         if len(label.text) <= 2:
             plt.annotate(label.text.replace("$[source]","").replace("$[sink]",""),(label.x,label.y))
         else: # rotate label for better visibility
             plt.gca().text(label.x,label.y, label.text.replace("$[source]","").replace("$[sink]",""), rotation=label_rot,fontsize=fontsize)
 
     # 3. return the figure or show window
@@ -583,16 +681,17 @@
         max_x = max(max_x,point.x)
         max_y = max(max_y,point.y)
 
     for label in my_labels.values():
         max_x = max(max_x,label.x)
         max_y = max(max_y,label.y)
 
+    maxy = max([b.maxy() for b in Band.instances])
     plt.xlim([3,max_x+5])
-    plt.ylim([3,max_y+3])
+    plt.ylim([3,maxy+3])
 
     #plt.autoscale()
 
     plt.tight_layout()
 
     plt.title(title)
```

### Comparing `sfctools-1.0.6.1/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.6.2/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/sfctools/misc/timeseries.py` & `sfctools-1.0.6.2/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.1/setup.py` & `sfctools-1.0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.6.1',
+    'version': '1.0.6.2',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.6.1/PKG-INFO` & `sfctools-1.0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.6.1
+Version: 1.0.6.2
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

