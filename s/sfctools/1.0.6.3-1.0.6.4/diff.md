# Comparing `tmp/sfctools-1.0.6.3.tar.gz` & `tmp/sfctools-1.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.6.3.tar", max compression
+gzip compressed data, was "sfctools-1.0.6.4.tar", max compression
```

## Comparing `sfctools-1.0.6.3.tar` & `sfctools-1.0.6.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.3/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-04 18:41:55.106218 sfctools-1.0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.3/README.md
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.3/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.3/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.3/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.3/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.3/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.3/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.3/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.3/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.3/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.3/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.3/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.3/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.3/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.3/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.3/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.3/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15252 2023-05-04 18:38:24.098165 sfctools-1.0.6.3/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.3/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.3/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.3/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.3/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.3/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.3/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.3/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.3/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.3/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.3/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.3/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.3/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.3/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.3/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.3/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.3/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.3/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.3/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.3/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.3/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.3/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-04 18:39:36.198530 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      416 2023-05-04 18:39:36.258191 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      412 2023-05-04 18:39:36.317192 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      417 2023-05-04 18:39:36.376193 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      412 2023-05-04 18:39:36.434194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      413 2023-05-04 18:39:36.491194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      413 2023-05-04 18:39:36.550194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      412 2023-05-04 18:39:36.605194 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      410 2023-05-04 18:39:36.663195 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      411 2023-05-04 18:39:36.726197 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      418 2023-05-04 18:39:36.783222 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-05-04 18:39:36.784197 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-04 18:39:36.784722 sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.3/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.3/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.3/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.3/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.3/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.3/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.3/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.3/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.3/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.3/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.3/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.3/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.3/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.3/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.3/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.3/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.3/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.3/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.3/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.3/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.3/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-04 18:39:38.676454 sfctools-1.0.6.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.3/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.3/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.3/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.3/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.3/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.3/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.3/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.3/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.3/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.3/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    21989 2023-05-04 18:34:38.291617 sfctools-1.0.6.3/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.3/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.3/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.3/setup.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.4/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 19:46:48.508957 sfctools-1.0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.4/README.md
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.4/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.4/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.4/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.4/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.4/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.4/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.4/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.4/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.4/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.4/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.4/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.4/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.4/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.4/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.4/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.4/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15252 2023-05-04 18:38:24.098165 sfctools-1.0.6.4/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.4/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.4/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.4/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.4/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.4/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.4/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.4/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.4/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.4/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.4/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.4/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.4/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.4/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.4/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.4/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.4/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.4/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.4/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.4/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.4/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.4/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.4/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.4/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.4/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.4/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.4/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.4/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.4/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.4/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.4/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.4/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 18:39:36.198530 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      416 2023-05-04 18:39:36.258191 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.317192 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      417 2023-05-04 18:39:36.376193 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.434194 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      413 2023-05-04 18:39:36.491194 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      413 2023-05-04 18:39:36.550194 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      412 2023-05-04 18:39:36.605194 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      410 2023-05-04 18:39:36.663195 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      411 2023-05-04 18:39:36.726197 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      418 2023-05-04 18:39:36.783222 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-05-04 18:39:36.784197 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 18:39:36.784722 sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.4/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.4/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.4/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.4/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.4/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.4/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.4/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.4/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.4/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.4/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.4/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.4/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.4/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.4/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.4/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.4/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.4/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.4/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.4/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.4/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136652 2023-05-04 19:45:36.979343 sfctools-1.0.6.4/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.4/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.4/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.4/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.4/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.4/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.4/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.4/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 18:39:38.676454 sfctools-1.0.6.4/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.4/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.4/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.4/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.4/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.4/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.4/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.4/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.4/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.4/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.4/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    21989 2023-05-04 18:34:38.291617 sfctools-1.0.6.4/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.4/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.4/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.6.4/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.4/PKG-INFO
```

### Comparing `sfctools-1.0.6.3/LICENSE` & `sfctools-1.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/pyproject.toml` & `sfctools-1.0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.6.3"
+version = "1.0.6.4"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.6.3/README.md` & `sfctools-1.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/__init__.py` & `sfctools-1.0.6.4/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/__main__.py` & `sfctools-1.0.6.4/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/automation/calibration.py` & `sfctools-1.0.6.4/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/automation/cgesolver.py` & `sfctools-1.0.6.4/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/automation/runner.py` & `sfctools-1.0.6.4/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/bottomup/matching.py` & `sfctools-1.0.6.4/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/bottomup/productiontree.py` & `sfctools-1.0.6.4/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.6.4/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/bottomup/treestruct.py` & `sfctools-1.0.6.4/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/agent.py` & `sfctools-1.0.6.4/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/clock.py` & `sfctools-1.0.6.4/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/flow_matrix.py` & `sfctools-1.0.6.4/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/settings.py` & `sfctools-1.0.6.4/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/singleton.py` & `sfctools-1.0.6.4/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/core/world.py` & `sfctools-1.0.6.4/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/balance.py` & `sfctools-1.0.6.4/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.6.4/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.6.4/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/collection.py` & `sfctools-1.0.6.4/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/income_statement.py` & `sfctools-1.0.6.4/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/inventory.py` & `sfctools-1.0.6.4/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/market_registry.py` & `sfctools-1.0.6.4/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/signalslot.py` & `sfctools-1.0.6.4/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.6.4/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/__init__.py` & `sfctools-1.0.6.4/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/balance.py` & `sfctools-1.0.6.4/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.6.4/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/clock.py` & `sfctools-1.0.6.4/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/example_wrapper.py` & `sfctools-1.0.6.4/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.6.4/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/flowmatrix.py` & `sfctools-1.0.6.4/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/hello_agent.py` & `sfctools-1.0.6.4/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/inventory.py` & `sfctools-1.0.6.4/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/market_example/market.py` & `sfctools-1.0.6.4/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/market_example/market2.py` & `sfctools-1.0.6.4/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.6.4/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.6.4/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/order_book.py` & `sfctools-1.0.6.4/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/examples/signal_slot.py` & `sfctools-1.0.6.4/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.6.4/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/draw_widget.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/qtattune.py`

 * *Files 0% similar despite different names*

```diff
@@ -3147,5390 +3147,5395 @@
 0000c4a0: 2020 2020 2020 666f 7220 626f 7820 696e        for box in
 0000c4b0: 2073 656c 662e 6472 6177 6361 6e76 6173   self.drawcanvas
 0000c4c0: 2e62 6f78 6573 3a0d 0a20 2020 2020 2020  .boxes:..       
 0000c4d0: 2020 2020 2062 6f78 2e65 6469 745f 6167       box.edit_ag
 0000c4e0: 656e 7428 290d 0a0d 0a20 2020 2020 2020  ent()....       
 0000c4f0: 2023 2075 7064 6174 6520 6469 7370 6c61   # update displa
 0000c500: 7920 6f70 7469 6f6e 730d 0a20 2020 2020  y options..     
-0000c510: 2020 2069 6620 226f 7074 696f 6e73 2220     if "options" 
-0000c520: 696e 2074 7261 6e73 6163 7469 6f6e 5f64  in transaction_d
-0000c530: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
-0000c540: 2020 6966 2074 7261 6e73 6163 7469 6f6e    if transaction
-0000c550: 5f64 6174 615b 226f 7074 696f 6e73 225d  _data["options"]
-0000c560: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c580: 656c 662e 7365 745f 6f70 7469 6f6e 7328  elf.set_options(
-0000c590: 7472 616e 7361 6374 696f 6e5f 6461 7461  transaction_data
-0000c5a0: 5b22 6f70 7469 6f6e 7322 5d29 0d0a 2020  ["options"])..  
-0000c5b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000c5c0: 2020 6465 6620 656e 7472 795f 746f 5f76    def entry_to_v
-0000c5d0: 616c 7328 7365 6c66 2c65 6e74 7279 2c20  als(self,entry, 
-0000c5e0: 6167 656e 742c 7768 6963 6829 3a0d 0a0d  agent,which):...
-0000c5f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000c600: 626f 6f6c 2872 6567 6578 2e66 696e 6461  bool(regex.finda
-0000c610: 6c6c 2822 285b 2b2d 5d2b 2922 2c20 656e  ll("([+-]+)", en
-0000c620: 7472 7929 293a 0d0a 2020 2020 2020 2020  try)):..        
-0000c630: 2020 2020 7365 6c66 2e6e 6f74 6966 7928      self.notify(
-0000c640: 6d65 7373 6167 653d 2253 6967 6e20 636f  message="Sign co
-0000c650: 7272 7570 7465 6420 696e 2065 6e74 7279  rrupted in entry
-0000c660: 2025 7320 2825 7320 6f66 2025 7329 2225   %s (%s of %s)"%
-0000c670: 2865 6e74 7279 2c77 6869 6368 2c61 6765  (entry,which,age
-0000c680: 6e74 292c 7469 746c 653d 2245 7272 6f72  nt),title="Error
-0000c690: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000c6a0: 7265 7475 726e 204e 6f6e 652c 204e 6f6e  return None, Non
-0000c6b0: 652c 204e 6f6e 650d 0a0d 0a20 2020 2020  e, None....     
-0000c6c0: 2020 2069 6620 7265 6765 782e 6669 6e64     if regex.find
-0000c6d0: 616c 6c28 2228 5b2b 2d5d 2b29 222c 2065  all("([+-]+)", e
-0000c6e0: 6e74 7279 295b 305d 203d 3d20 222d 223a  ntry)[0] == "-":
-0000c6f0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
-0000c700: 676e 203d 2022 2d22 0d0a 2020 2020 2020  gn = "-"..      
-0000c710: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000c720: 2020 2020 2073 6967 6e20 3d20 222b 220d       sign = "+".
-0000c730: 0a0d 0a20 2020 2020 2020 2077 6f72 6473  ...        words
-0000c740: 203d 2072 6567 6578 2e66 696e 6461 6c6c   = regex.findall
-0000c750: 2822 285b 5c77 5c73 5d2b 2922 2c20 656e  ("([\w\s]+)", en
-0000c760: 7472 7929 0d0a 0d0a 2020 2020 2020 2020  try)....        
-0000c770: 6974 656d 203d 2022 220d 0a20 2020 2020  item = ""..     
-0000c780: 2020 2073 696c 656e 7420 3d20 4661 6c73     silent = Fals
-0000c790: 650d 0a20 2020 2020 2020 2066 6f72 2077  e..        for w
-0000c7a0: 6f72 6420 696e 2077 6f72 6473 3a0d 0a20  ord in words:.. 
-0000c7b0: 2020 2020 2020 2020 2020 2069 6620 776f             if wo
-0000c7c0: 7264 2021 3d20 2273 223a 0d0a 2020 2020  rd != "s":..    
-0000c7d0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-0000c7e0: 202b 3d20 776f 7264 2e73 7472 6970 2829   += word.strip()
-0000c7f0: 202b 2022 2022 0d0a 2020 2020 2020 2020   + " "..        
-0000c800: 2020 2020 656c 6966 2077 6f72 6420 3d3d      elif word ==
-0000c810: 2022 7322 3a0d 0a20 2020 2020 2020 2020   "s":..         
-0000c820: 2020 2020 2020 2073 696c 656e 7420 3d20         silent = 
-0000c830: 5472 7565 0d0a 0d0a 2020 2020 2020 2020  True....        
-0000c840: 6974 656d 203d 2069 7465 6d2e 7374 7269  item = item.stri
-0000c850: 7028 290d 0a0d 0a20 2020 2020 2020 2072  p()....        r
-0000c860: 6574 7572 6e20 7369 676e 2c20 6974 656d  eturn sign, item
-0000c870: 2c20 7369 6c65 6e74 0d0a 0d0a 0d0a 2020  , silent......  
-0000c880: 2020 6465 6620 7570 6461 7465 5f74 6162    def update_tab
-0000c890: 6c65 2873 656c 6629 3a0d 0a20 2020 2020  le(self):..     
-0000c8a0: 2020 2023 7365 6c66 2e73 656c 6563 7469     #self.selecti
-0000c8b0: 6f6e 5f69 6478 203d 204e 6f6e 650d 0a20  on_idx = None.. 
-0000c8c0: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
-0000c8d0: 7361 6374 696f 6e56 6965 772e 7365 7452  sactionView.setR
-0000c8e0: 6f77 436f 756e 7428 3029 0d0a 0d0a 2020  owCount(0)....  
-0000c8f0: 2020 2020 2020 2320 7365 6c66 2e74 7261        # self.tra
-0000c900: 6e73 6163 7469 6f6e 5669 6577 2e6d 6f64  nsactionView.mod
-0000c910: 656c 2829 2e73 6574 546f 7269 7a6f 6e74  el().setTorizont
-0000c920: 616c 4865 6164 6572 4974 656d 2820 302c  alHeaderItem( 0,
-0000c930: 2051 5461 626c 6557 6964 6765 7449 7465   QTableWidgetIte
-0000c940: 6d28 224e 616d 6522 2929 0d0a 2020 2020  m("Name"))..    
-0000c950: 2020 2020 2320 7365 6c66 2e74 7261 6e73      # self.trans
-0000c960: 6163 7469 6f6e 5669 6577 2e6d 6f64 656c  actionView.model
-0000c970: 2829 2e73 6574 546f 7269 7a6f 6e74 616c  ().setTorizontal
-0000c980: 4865 6164 6572 4974 656d 2820 312c 2051  HeaderItem( 1, Q
-0000c990: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-0000c9a0: 2253 686f 7274 204e 616d 6522 2929 0d0a  "Short Name"))..
-0000c9b0: 2020 2020 2020 2020 2320 7365 6c66 2e74          # self.t
-0000c9c0: 7261 6e73 6163 7469 6f6e 5669 6577 2e6d  ransactionView.m
-0000c9d0: 6f64 656c 2829 2e73 6574 546f 7269 7a6f  odel().setTorizo
-0000c9e0: 6e74 616c 4865 6164 6572 4974 656d 2820  ntalHeaderItem( 
-0000c9f0: 322c 2051 5461 626c 6557 6964 6765 7449  2, QTableWidgetI
-0000ca00: 7465 6d28 2255 6e69 6469 7265 6374 696f  tem("Unidirectio
-0000ca10: 6e61 6c22 2929 0d0a 2020 2020 2020 2020  nal"))..        
-0000ca20: 2320 7365 6c66 2e74 7261 6e73 6163 7469  # self.transacti
-0000ca30: 6f6e 5669 6577 2e6d 6f64 656c 2829 2e73  onView.model().s
-0000ca40: 6574 546f 7269 7a6f 6e74 616c 4865 6164  etTorizontalHead
-0000ca50: 6572 4974 656d 2820 332c 2051 5461 626c  erItem( 3, QTabl
-0000ca60: 6557 6964 6765 7449 7465 6d28 2246 6c6f  eWidgetItem("Flo
-0000ca70: 7722 2929 0d0a 0d0a 2020 2020 2020 2020  w"))....        
-0000ca80: 2320 696e 7365 7274 206e 6577 2072 6f77  # insert new row
-0000ca90: 7320 6966 206e 6565 6465 640d 0a20 2020  s if needed..   
-0000caa0: 2020 2020 2072 6f77 5f63 6f75 6e74 203d       row_count =
-0000cab0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
-0000cac0: 6e56 6965 772e 726f 7743 6f75 6e74 2829  nView.rowCount()
-0000cad0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
-0000cae0: 656c 662e 656e 7472 795f 6461 7461 2069  elf.entry_data i
-0000caf0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-0000cb00: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
-0000cb10: 2822 4461 7461 2069 7320 656d 7074 7920  ("Data is empty 
-0000cb20: 6f72 2063 6f72 7275 7074 6564 2e20 536f  or corrupted. So
-0000cb30: 6d65 7468 696e 6720 7765 6e74 2077 726f  mething went wro
-0000cb40: 6e67 222c 2074 6974 6c65 3d22 4661 7461  ng", title="Fata
-0000cb50: 6c20 4572 726f 7222 290d 0a20 2020 2020  l Error")..     
-0000cb60: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
-0000cb70: 0a20 2020 2020 2020 2069 6620 726f 775f  .        if row_
-0000cb80: 636f 756e 7420 3c20 6c65 6e28 7365 6c66  count < len(self
-0000cb90: 2e65 6e74 7279 5f64 6174 6129 3a0d 0a20  .entry_data):.. 
-0000cba0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000cbb0: 2069 6e20 7261 6e67 6528 6c65 6e28 7365   in range(len(se
-0000cbc0: 6c66 2e65 6e74 7279 5f64 6174 6129 2d72  lf.entry_data)-r
-0000cbd0: 6f77 5f63 6f75 6e74 293a 0d0a 2020 2020  ow_count):..    
-0000cbe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cbf0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000cc00: 2e69 6e73 6572 7452 6f77 2872 6f77 5f63  .insertRow(row_c
-0000cc10: 6f75 6e74 290d 0a0d 0a20 2020 2020 2020  ount)....       
-0000cc20: 2073 656c 662e 6472 6177 6361 6e76 6173   self.drawcanvas
-0000cc30: 2e63 6c65 6172 2829 0d0a 2020 2020 2020  .clear()..      
-0000cc40: 2020 7365 6c66 2e66 696c 7465 7243 6f6d    self.filterCom
-0000cc50: 626f 2e63 6c65 6172 2829 0d0a 2020 2020  bo.clear()..    
-0000cc60: 2020 2020 7365 6c66 2e66 696c 7465 725f      self.filter_
-0000cc70: 656e 7472 6965 7320 3d20 5b5d 0d0a 0d0a  entries = []....
-0000cc80: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-0000cc90: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-0000cca0: 2064 6174 6120 696e 2065 6e75 6d65 7261   data in enumera
-0000ccb0: 7465 2873 656c 662e 656e 7472 795f 6461  te(self.entry_da
-0000ccc0: 7461 293a 0d0a 2020 2020 2020 2020 2020  ta):..          
-0000ccd0: 2020 2020 2020 2320 6578 6973 7473 3120        # exists1 
-0000cce0: 3d20 7365 6c66 2e64 7261 7763 616e 7661  = self.drawcanva
-0000ccf0: 732e 6368 6563 6b5f 6578 6973 7428 6461  s.check_exist(da
-0000cd00: 7461 5b22 6167 656e 7431 225d 2e63 6170  ta["agent1"].cap
-0000cd10: 6974 616c 697a 6528 2929 0d0a 2020 2020  italize())..    
-0000cd20: 2020 2020 2020 2020 2020 2020 2320 6578              # ex
-0000cd30: 6973 7473 3220 3d20 7365 6c66 2e64 7261  ists2 = self.dra
-0000cd40: 7763 616e 7661 732e 6368 6563 6b5f 6578  wcanvas.check_ex
-0000cd50: 6973 7428 6461 7461 5b22 6167 656e 7432  ist(data["agent2
-0000cd60: 225d 2e63 6170 6974 616c 697a 6528 2929  "].capitalize())
-0000cd70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000cd80: 2020 2020 2020 2020 6e65 775f 6167 656e          new_agen
-0000cd90: 7431 203d 2063 616d 656c 2864 6174 615b  t1 = camel(data[
-0000cda0: 2261 6765 6e74 3122 5d29 0d0a 2020 2020  "agent1"])..    
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 6e65 775f 6167 656e 7432 203d 2063 616d  new_agent2 = cam
-0000cdd0: 656c 2864 6174 615b 2261 6765 6e74 3222  el(data["agent2"
-0000cde0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0000cdf0: 2020 2020 2020 2020 626f 7831 203d 2073          box1 = s
-0000ce00: 656c 662e 6472 6177 6361 6e76 6173 2e61  elf.drawcanvas.a
-0000ce10: 6464 5f61 6765 6e74 286e 6577 5f61 6765  dd_agent(new_age
-0000ce20: 6e74 3129 2023 202e 6361 7069 7461 6c69  nt1) # .capitali
-0000ce30: 7a65 2829 290d 0a20 2020 2020 2020 2020  ze())..         
-0000ce40: 2020 2020 2020 2020 2020 2062 6f78 3220             box2 
-0000ce50: 3d20 7365 6c66 2e64 7261 7763 616e 7661  = self.drawcanva
-0000ce60: 732e 6164 645f 6167 656e 7428 6e65 775f  s.add_agent(new_
-0000ce70: 6167 656e 7432 2920 232e 6361 7069 7461  agent2) #.capita
-0000ce80: 6c69 7a65 2829 290d 0a0d 0a20 2020 2020  lize())....     
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000cea0: 2063 6f72 7265 6374 206e 756d 6265 7220   correct number 
-0000ceb0: 6f66 2063 6f6e 6e65 6374 696f 6e73 2066  of connections f
-0000cec0: 6f72 2065 7869 7374 696e 6720 6167 656e  or existing agen
-0000ced0: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-0000cee0: 2020 2020 2020 2020 626f 7831 2e6e 5f63          box1.n_c
-0000cef0: 6f6e 6e65 6374 696f 6e73 203d 2030 0d0a  onnections = 0..
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 626f 7832 2e6e 5f63 6f6e 6e65      box2.n_conne
-0000cf20: 6374 696f 6e73 203d 2030 0d0a 0d0a 0d0a  ctions = 0......
-0000cf30: 2020 2020 2020 2020 2020 2020 2320 7570              # up
-0000cf40: 6461 7465 2074 6865 2064 6174 610d 0a20  date the data.. 
-0000cf50: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000cf60: 2c20 6461 7461 2069 6e20 656e 756d 6572  , data in enumer
-0000cf70: 6174 6528 7365 6c66 2e65 6e74 7279 5f64  ate(self.entry_d
-0000cf80: 6174 6129 3a0d 0a20 2020 2020 2020 2020  ata):..         
-0000cf90: 2020 2020 2020 2070 7269 6e74 2864 6174         print(dat
-0000cfa0: 6129 0d0a 0d0a 2020 2020 2020 2020 2020  a)....          
-0000cfb0: 2020 2020 2020 7365 6c66 2e74 7261 6e73        self.trans
-0000cfc0: 6163 7469 6f6e 5669 6577 2e73 6574 4974  actionView.setIt
-0000cfd0: 656d 2869 2c20 302c 2051 5461 626c 6557  em(i, 0, QTableW
-0000cfe0: 6964 6765 7449 7465 6d28 6461 7461 5b22  idgetItem(data["
-0000cff0: 7375 626a 6563 7422 5d29 290d 0a20 2020  subject"]))..   
-0000d000: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d010: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
-0000d020: 772e 7365 7449 7465 6d28 692c 2031 2c20  w.setItem(i, 1, 
-0000d030: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
-0000d040: 2863 616d 656c 2864 6174 615b 2261 6765  (camel(data["age
-0000d050: 6e74 3122 5d29 2929 2023 202e 6361 7069  nt1"]))) # .capi
-0000d060: 7461 6c69 7a65 2829 2929 0d0a 2020 2020  talize()))..    
-0000d070: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d080: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000d090: 2e73 6574 4974 656d 2869 2c20 322c 2051  .setItem(i, 2, Q
-0000d0a0: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-0000d0b0: 6361 6d65 6c28 6461 7461 5b22 6167 656e  camel(data["agen
-0000d0c0: 7432 225d 2929 2920 2320 2e63 6170 6974  t2"]))) # .capit
-0000d0d0: 616c 697a 6528 2929 290d 0a20 2020 2020  alize()))..     
-0000d0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d0f0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-0000d100: 7365 7449 7465 6d28 692c 2033 2c20 5154  setItem(i, 3, QT
-0000d110: 6162 6c65 5769 6467 6574 4974 656d 2864  ableWidgetItem(d
-0000d120: 6174 615b 2273 686f 7274 6e61 6d65 225d  ata["shortname"]
-0000d130: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000d140: 2020 2020 7365 6c66 2e74 7261 6e73 6163      self.transac
-0000d150: 7469 6f6e 5669 6577 2e73 6574 4974 656d  tionView.setItem
-0000d160: 2869 2c20 342c 2051 5461 626c 6557 6964  (i, 4, QTableWid
-0000d170: 6765 7449 7465 6d28 6461 7461 5b22 6b69  getItem(data["ki
-0000d180: 6e64 225d 2929 0d0a 2020 2020 2020 2020  nd"]))..        
-0000d190: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000d1a0: 6e73 6163 7469 6f6e 5669 6577 2e73 6574  nsactionView.set
-0000d1b0: 4974 656d 2869 2c20 352c 2051 5461 626c  Item(i, 5, QTabl
-0000d1c0: 6557 6964 6765 7449 7465 6d28 7374 7228  eWidgetItem(str(
-0000d1d0: 6461 7461 5b22 756e 692d 6469 7265 6374  data["uni-direct
-0000d1e0: 696f 6e61 6c22 5d29 2929 0d0a 2020 2020  ional"])))..    
-0000d1f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d200: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000d210: 2e73 6574 4974 656d 2869 2c20 362c 2051  .setItem(i, 6, Q
-0000d220: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-0000d230: 7374 7228 6461 7461 5b22 7175 616e 7469  str(data["quanti
-0000d240: 7479 225d 2929 290d 0a20 2020 2020 2020  ty"])))..       
-0000d250: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-0000d260: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-0000d270: 7365 6c65 6374 696f 6e4d 6f64 656c 2829  selectionModel()
-0000d280: 2e73 656c 6563 7465 6452 6f77 7328 290d  .selectedRows().
-0000d290: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000d2a0: 2020 2062 6f78 3120 3d20 7365 6c66 2e64     box1 = self.d
-0000d2b0: 7261 7763 616e 7661 732e 6164 645f 6167  rawcanvas.add_ag
-0000d2c0: 656e 7428 6361 6d65 6c28 6461 7461 5b22  ent(camel(data["
-0000d2d0: 6167 656e 7431 225d 2929 2023 2e63 6170  agent1"])) #.cap
-0000d2e0: 6974 616c 697a 6528 2929 0d0a 2020 2020  italize())..    
-0000d2f0: 2020 2020 2020 2020 2020 2020 626f 7832              box2
-0000d300: 203d 2073 656c 662e 6472 6177 6361 6e76   = self.drawcanv
-0000d310: 6173 2e61 6464 5f61 6765 6e74 2863 616d  as.add_agent(cam
-0000d320: 656c 2864 6174 615b 2261 6765 6e74 3222  el(data["agent2"
-0000d330: 5d29 2920 232e 6361 7069 7461 6c69 7a65  ])) #.capitalize
-0000d340: 2829 290d 0a0d 0a20 2020 2020 2020 2020  ())....         
-0000d350: 2020 2020 2020 206d 795f 6974 656d 7320         my_items 
-0000d360: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-0000d370: 2020 2020 2020 2020 616c 6c65 6e74 7269          allentri
-0000d380: 6573 203d 2022 5c6e 222e 6a6f 696e 285b  es = "\n".join([
-0000d390: 6461 7461 5b22 6c31 225d 2c20 6461 7461  data["l1"], data
-0000d3a0: 5b22 6131 225d 2c20 6461 7461 5b22 6531  ["a1"], data["e1
-0000d3b0: 225d 2c20 6461 7461 5b22 6c32 225d 2c20  "], data["l2"], 
-0000d3c0: 6461 7461 5b22 6132 225d 2c20 6461 7461  data["a2"], data
-0000d3d0: 5b22 6532 225d 5d29 0d0a 2020 2020 2020  ["e2"]])..      
-0000d3e0: 2020 2020 2020 2020 2020 666f 7220 7375            for su
-0000d3f0: 625f 6974 656d 2069 6e20 616c 6c65 6e74  b_item in allent
-0000d400: 7269 6573 2e73 706c 6974 2822 5c6e 2229  ries.split("\n")
-0000d410: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d420: 2020 2020 2020 2066 6f72 2073 7562 5f65         for sub_e
-0000d430: 6e74 7279 2069 6e20 7375 625f 6974 656d  ntry in sub_item
-0000d440: 2e73 706c 6974 2822 5c6e 2229 3a0d 0a20  .split("\n"):.. 
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 2020 2020 2020 2065 6e74 7279 203d 2073         entry = s
-0000d470: 7562 5f65 6e74 7279 2e72 6570 6c61 6365  ub_entry.replace
-0000d480: 2822 2d22 2c22 2229 2e72 6570 6c61 6365  ("-","").replace
-0000d490: 2822 2b22 2c22 2229 2e73 7472 6970 2829  ("+","").strip()
-0000d4a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d4b0: 2020 2020 2020 2020 2020 6966 2065 6e74            if ent
-0000d4c0: 7279 2021 3d20 2022 223a 0d0a 2020 2020  ry !=  "":..    
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2020 2020 2020 2020 6d79 5f69 7465 6d73          my_items
-0000d4f0: 2e61 7070 656e 6428 656e 7472 7929 0d0a  .append(entry)..
-0000d500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d510: 2020 7365 6c66 2e64 7261 7763 616e 7661    self.drawcanva
-0000d520: 732e 6164 645f 636f 6e6e 6563 7469 6f6e  s.add_connection
-0000d530: 2862 6f78 312c 2062 6f78 322c 206e 616d  (box1, box2, nam
-0000d540: 653d 2064 6174 615b 2273 686f 7274 6e61  e= data["shortna
-0000d550: 6d65 225d 2c73 7562 6a65 6374 3d64 6174  me"],subject=dat
-0000d560: 615b 2273 7562 6a65 6374 225d 2c69 7465  a["subject"],ite
-0000d570: 6d73 3d6d 795f 6974 656d 7329 0d0a 0d0a  ms=my_items)....
-0000d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d590: 2320 7570 6461 7465 2074 6865 2066 696c  # update the fil
-0000d5a0: 7465 7220 7661 6c75 6573 0d0a 2020 2020  ter values..    
-0000d5b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d5c0: 656e 7472 7920 696e 206d 795f 6974 656d  entry in my_item
-0000d5d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-0000d5e0: 2020 2020 2020 2020 6966 2065 6e74 7279          if entry
-0000d5f0: 206e 6f74 2069 6e20 7365 6c66 2e66 696c   not in self.fil
-0000d600: 7465 725f 656e 7472 6965 733a 0d0a 2020  ter_entries:..  
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 2020 7365 6c66 2e66 696c 7465        self.filte
-0000d630: 725f 656e 7472 6965 732e 6170 7065 6e64  r_entries.append
-0000d640: 2865 6e74 7279 290d 0a0d 0a20 2020 2020  (entry)....     
-0000d650: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000d660: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0000d670: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
-0000d680: 6679 2873 7472 2865 292b 225c 6e22 202b  fy(str(e)+"\n" +
-0000d690: 2073 7472 2864 6174 6129 2c74 6974 6c65   str(data),title
-0000d6a0: 3d22 4572 726f 7222 290d 0a0d 0a20 2020  ="Error")....   
-0000d6b0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-0000d6c0: 2020 2020 2020 2023 2073 6561 7263 6820         # search 
-0000d6d0: 666f 7220 6120 6d61 7463 6820 696e 2074  for a match in t
-0000d6e0: 6865 2066 696c 7465 720d 0a0d 0a20 2020  he filter....   
-0000d6f0: 2020 2020 2020 2020 2066 6f75 6e64 5f69           found_i
-0000d700: 6478 7320 3d20 5b5d 0d0a 2020 2020 2020  dxs = []..      
-0000d710: 2020 2020 2020 7365 6172 6368 5f73 7472        search_str
-0000d720: 203d 2073 656c 662e 4669 6c74 6572 6c69   = self.Filterli
-0000d730: 6e65 4564 6974 2e74 6578 7428 290d 0a0d  neEdit.text()...
-0000d740: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d750: 7365 6172 6368 5f73 7472 2021 3d20 2222  search_str != ""
-0000d760: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000d770: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-0000d780: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000d790: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-0000d7a0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000d7b0: 2e72 6f77 436f 756e 7428 2929 3a0d 0a0d  .rowCount()):...
-0000d7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d7d0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0000d7e0: 6e20 7261 6e67 6528 7365 6c66 2e74 7261  n range(self.tra
-0000d7f0: 6e73 6163 7469 6f6e 5669 6577 2e63 6f6c  nsactionView.col
-0000d800: 756d 6e43 6f75 6e74 2829 293a 0d0a 0d0a  umnCount()):....
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-0000d830: 795f 7374 7220 3d20 7365 6c66 2e74 7261  y_str = self.tra
-0000d840: 6e73 6163 7469 6f6e 5669 6577 2e69 7465  nsactionView.ite
-0000d850: 6d28 692c 6a29 2e74 6578 7428 290d 0a0d  m(i,j).text()...
-0000d860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d880: 656e 7472 795f 7374 722e 6669 6e64 2873  entry_str.find(s
-0000d890: 6561 7263 685f 7374 7229 203e 202d 313a  earch_str) > -1:
-0000d8a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 666f 756e 645f 6964 7873 2e61      found_idxs.a
-0000d8d0: 7070 656e 6428 6929 0d0a 2020 2020 2020  ppend(i)..      
-0000d8e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000d8f0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-0000d900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d910: 2020 2020 2020 7072 696e 7428 2245 7863        print("Exc
-0000d920: 6570 7469 6f6e 3a22 2c20 7374 7228 6529  eption:", str(e)
-0000d930: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000d940: 2066 6f72 2066 6f75 6e64 5f69 6478 2069   for found_idx i
-0000d950: 6e20 666f 756e 645f 6964 7873 3a0d 0a20  n found_idxs:.. 
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000d970: 2068 6967 686c 6967 6874 206f 6363 7572   highlight occur
-0000d980: 616e 6365 730d 0a20 2020 2020 2020 2020  ances..         
-0000d990: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0000d9a0: 7261 6e67 6528 7365 6c66 2e74 7261 6e73  range(self.trans
-0000d9b0: 6163 7469 6f6e 5669 6577 2e63 6f6c 756d  actionView.colum
-0000d9c0: 6e43 6f75 6e74 2829 293a 0d0a 2020 2020  nCount()):..    
-0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9e0: 7472 793a 0d0a 0d0a 2020 2020 2020 2020  try:....        
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 6966 2073 656c 662e 7468 656d 655f 6d61  if self.theme_ma
-0000da10: 6e61 6765 722e 7468 656d 6520 3d3d 2022  nager.theme == "
-0000da20: 6272 6967 6874 223a 0d0a 0d0a 2020 2020  bright":....    
-0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da40: 2020 2020 2020 2020 2320 6c69 6768 7420          # light 
-0000da50: 6d6f 6465 0d0a 2020 2020 2020 2020 2020  mode..          
-0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da70: 2020 7365 6c66 2e74 7261 6e73 6163 7469    self.transacti
-0000da80: 6f6e 5669 6577 2e69 7465 6d28 666f 756e  onView.item(foun
-0000da90: 645f 6964 782c 206a 292e 7365 7442 6163  d_idx, j).setBac
-0000daa0: 6b67 726f 756e 6428 5174 4775 692e 5143  kground(QtGui.QC
-0000dab0: 6f6c 6f72 2832 3237 2c20 3136 362c 2031  olor(227, 166, 1
-0000dac0: 3636 2929 0d0a 2020 2020 2020 2020 2020  66))..          
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2020 7365 6c66 2e74 7261 6e73 6163 7469    self.transacti
-0000daf0: 6f6e 5669 6577 2e69 7465 6d28 666f 756e  onView.item(foun
-0000db00: 645f 6964 782c 206a 292e 7365 7446 6f72  d_idx, j).setFor
-0000db10: 6567 726f 756e 6428 5174 4775 692e 5143  eground(QtGui.QC
-0000db20: 6f6c 6f72 2831 3830 2c20 3138 2c20 3138  olor(180, 18, 18
-0000db30: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0000db40: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000db50: 7365 3a0d 0a0d 0a20 2020 2020 2020 2020  se:....         
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2023 2064 6172 6b20 6d6f 6465 0d0a     # dark mode..
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dba0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000dbb0: 2e69 7465 6d28 666f 756e 645f 6964 782c  .item(found_idx,
-0000dbc0: 206a 292e 7365 7442 6163 6b67 726f 756e   j).setBackgroun
-0000dbd0: 6428 5174 4775 692e 5143 6f6c 6f72 2831  d(QtGui.QColor(1
-0000dbe0: 3230 2c20 3132 302c 2031 3230 2929 0d0a  20, 120, 120))..
-0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dc10: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000dc20: 2e69 7465 6d28 666f 756e 645f 6964 782c  .item(found_idx,
-0000dc30: 206a 292e 7365 7446 6f72 6567 726f 756e   j).setForegroun
-0000dc40: 6428 5174 4775 692e 5143 6f6c 6f72 2835  d(QtGui.QColor(5
-0000dc50: 302c 2035 302c 2035 3029 290d 0a0d 0a20  0, 50, 50)).... 
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2020 2065 7863 6570 743a 0d0a 2020 2020     except:..    
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 2020 2320 6176 6f69 6473 204e 6f6e 6520    # avoids None 
-0000dcc0: 706f 696e 7465 7220 7768 656e 2061 2074  pointer when a t
-0000dcd0: 7261 6e73 6163 7469 6f6e 2069 7320 6465  ransaction is de
-0000dce0: 6c65 7465 640d 0a20 2020 2020 2020 2065  leted..        e
-0000dcf0: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-0000dd00: 2020 2020 7061 7373 0d0a 0d0a 0d0a 2020      pass......  
-0000dd10: 2020 2020 2020 666f 7220 656e 7472 7920        for entry 
-0000dd20: 696e 2073 656c 662e 6669 6c74 6572 5f65  in self.filter_e
-0000dd30: 6e74 7269 6573 3a0d 0a20 2020 2020 2020  ntries:..       
-0000dd40: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
-0000dd50: 436f 6d62 6f2e 6164 6449 7465 6d28 656e  Combo.addItem(en
-0000dd60: 7472 7929 0d0a 0d0a 2020 2020 2020 2020  try)....        
-0000dd70: 7365 6c66 2e64 7261 7763 616e 7661 732e  self.drawcanvas.
-0000dd80: 7265 706f 7369 7469 6f6e 2829 0d0a 2020  reposition()..  
-0000dd90: 2020 2020 2020 7365 6c66 2e64 7261 7763        self.drawc
-0000dda0: 616e 7661 732e 7265 706f 7369 7469 6f6e  anvas.reposition
-0000ddb0: 5f6c 6162 656c 7328 290d 0a0d 0a20 2020  _labels()....   
+0000c510: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+0000c520: 2020 2020 2069 6620 226f 7074 696f 6e73       if "options
+0000c530: 2220 696e 2074 7261 6e73 6163 7469 6f6e  " in transaction
+0000c540: 5f64 6174 613a 0d0a 2020 2020 2020 2020  _data:..        
+0000c550: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+0000c560: 6163 7469 6f6e 5f64 6174 615b 226f 7074  action_data["opt
+0000c570: 696f 6e73 225d 2069 7320 6e6f 7420 4e6f  ions"] is not No
+0000c580: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000c590: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000c5a0: 745f 6f70 7469 6f6e 7328 7472 616e 7361  t_options(transa
+0000c5b0: 6374 696f 6e5f 6461 7461 5b22 6f70 7469  ction_data["opti
+0000c5c0: 6f6e 7322 5d29 0d0a 2020 2020 2020 2020  ons"])..        
+0000c5d0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0000c5e0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+0000c5f0: 2020 2020 7072 696e 7428 7374 7228 6529      print(str(e)
+0000c600: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+0000c610: 0a0d 0a20 2020 2064 6566 2065 6e74 7279  ...    def entry
+0000c620: 5f74 6f5f 7661 6c73 2873 656c 662c 656e  _to_vals(self,en
+0000c630: 7472 792c 2061 6765 6e74 2c77 6869 6368  try, agent,which
+0000c640: 293a 0d0a 0d0a 2020 2020 2020 2020 6966  ):....        if
+0000c650: 206e 6f74 2062 6f6f 6c28 7265 6765 782e   not bool(regex.
+0000c660: 6669 6e64 616c 6c28 2228 5b2b 2d5d 2b29  findall("([+-]+)
+0000c670: 222c 2065 6e74 7279 2929 3a0d 0a20 2020  ", entry)):..   
+0000c680: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+0000c690: 7469 6679 286d 6573 7361 6765 3d22 5369  tify(message="Si
+0000c6a0: 676e 2063 6f72 7275 7074 6564 2069 6e20  gn corrupted in 
+0000c6b0: 656e 7472 7920 2573 2028 2573 206f 6620  entry %s (%s of 
+0000c6c0: 2573 2922 2528 656e 7472 792c 7768 6963  %s)"%(entry,whic
+0000c6d0: 682c 6167 656e 7429 2c74 6974 6c65 3d22  h,agent),title="
+0000c6e0: 4572 726f 7222 290d 0a20 2020 2020 2020  Error")..       
+0000c6f0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000c700: 2c20 4e6f 6e65 2c20 4e6f 6e65 0d0a 0d0a  , None, None....
+0000c710: 2020 2020 2020 2020 6966 2072 6567 6578          if regex
+0000c720: 2e66 696e 6461 6c6c 2822 285b 2b2d 5d2b  .findall("([+-]+
+0000c730: 2922 2c20 656e 7472 7929 5b30 5d20 3d3d  )", entry)[0] ==
+0000c740: 2022 2d22 3a0d 0a20 2020 2020 2020 2020   "-":..         
+0000c750: 2020 2073 6967 6e20 3d20 222d 220d 0a20     sign = "-".. 
+0000c760: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000c770: 2020 2020 2020 2020 2020 7369 676e 203d            sign =
+0000c780: 2022 2b22 0d0a 0d0a 2020 2020 2020 2020   "+"....        
+0000c790: 776f 7264 7320 3d20 7265 6765 782e 6669  words = regex.fi
+0000c7a0: 6e64 616c 6c28 2228 5b5c 775c 735d 2b29  ndall("([\w\s]+)
+0000c7b0: 222c 2065 6e74 7279 290d 0a0d 0a20 2020  ", entry)....   
+0000c7c0: 2020 2020 2069 7465 6d20 3d20 2222 0d0a       item = ""..
+0000c7d0: 2020 2020 2020 2020 7369 6c65 6e74 203d          silent =
+0000c7e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0000c7f0: 666f 7220 776f 7264 2069 6e20 776f 7264  for word in word
+0000c800: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0000c810: 6966 2077 6f72 6420 213d 2022 7322 3a0d  if word != "s":.
+0000c820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c830: 2069 7465 6d20 2b3d 2077 6f72 642e 7374   item += word.st
+0000c840: 7269 7028 2920 2b20 2220 220d 0a20 2020  rip() + " "..   
+0000c850: 2020 2020 2020 2020 2065 6c69 6620 776f           elif wo
+0000c860: 7264 203d 3d20 2273 223a 0d0a 2020 2020  rd == "s":..    
+0000c870: 2020 2020 2020 2020 2020 2020 7369 6c65              sile
+0000c880: 6e74 203d 2054 7275 650d 0a0d 0a20 2020  nt = True....   
+0000c890: 2020 2020 2069 7465 6d20 3d20 6974 656d       item = item
+0000c8a0: 2e73 7472 6970 2829 0d0a 0d0a 2020 2020  .strip()....    
+0000c8b0: 2020 2020 7265 7475 726e 2073 6967 6e2c      return sign,
+0000c8c0: 2069 7465 6d2c 2073 696c 656e 740d 0a0d   item, silent...
+0000c8d0: 0a0d 0a20 2020 2064 6566 2075 7064 6174  ...    def updat
+0000c8e0: 655f 7461 626c 6528 7365 6c66 293a 0d0a  e_table(self):..
+0000c8f0: 2020 2020 2020 2020 2373 656c 662e 7365          #self.se
+0000c900: 6c65 6374 696f 6e5f 6964 7820 3d20 4e6f  lection_idx = No
+0000c910: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
+0000c920: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
+0000c930: 2e73 6574 526f 7743 6f75 6e74 2830 290d  .setRowCount(0).
+0000c940: 0a0d 0a20 2020 2020 2020 2023 2073 656c  ...        # sel
+0000c950: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+0000c960: 772e 6d6f 6465 6c28 292e 7365 7454 6f72  w.model().setTor
+0000c970: 697a 6f6e 7461 6c48 6561 6465 7249 7465  izontalHeaderIte
+0000c980: 6d28 2030 2c20 5154 6162 6c65 5769 6467  m( 0, QTableWidg
+0000c990: 6574 4974 656d 2822 4e61 6d65 2229 290d  etItem("Name")).
+0000c9a0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000c9b0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+0000c9c0: 6d6f 6465 6c28 292e 7365 7454 6f72 697a  model().setToriz
+0000c9d0: 6f6e 7461 6c48 6561 6465 7249 7465 6d28  ontalHeaderItem(
+0000c9e0: 2031 2c20 5154 6162 6c65 5769 6467 6574   1, QTableWidget
+0000c9f0: 4974 656d 2822 5368 6f72 7420 4e61 6d65  Item("Short Name
+0000ca00: 2229 290d 0a20 2020 2020 2020 2023 2073  "))..        # s
+0000ca10: 656c 662e 7472 616e 7361 6374 696f 6e56  elf.transactionV
+0000ca20: 6965 772e 6d6f 6465 6c28 292e 7365 7454  iew.model().setT
+0000ca30: 6f72 697a 6f6e 7461 6c48 6561 6465 7249  orizontalHeaderI
+0000ca40: 7465 6d28 2032 2c20 5154 6162 6c65 5769  tem( 2, QTableWi
+0000ca50: 6467 6574 4974 656d 2822 556e 6964 6972  dgetItem("Unidir
+0000ca60: 6563 7469 6f6e 616c 2229 290d 0a20 2020  ectional"))..   
+0000ca70: 2020 2020 2023 2073 656c 662e 7472 616e       # self.tran
+0000ca80: 7361 6374 696f 6e56 6965 772e 6d6f 6465  sactionView.mode
+0000ca90: 6c28 292e 7365 7454 6f72 697a 6f6e 7461  l().setTorizonta
+0000caa0: 6c48 6561 6465 7249 7465 6d28 2033 2c20  lHeaderItem( 3, 
+0000cab0: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+0000cac0: 2822 466c 6f77 2229 290d 0a0d 0a20 2020  ("Flow"))....   
+0000cad0: 2020 2020 2023 2069 6e73 6572 7420 6e65       # insert ne
+0000cae0: 7720 726f 7773 2069 6620 6e65 6564 6564  w rows if needed
+0000caf0: 0d0a 2020 2020 2020 2020 726f 775f 636f  ..        row_co
+0000cb00: 756e 7420 3d20 7365 6c66 2e74 7261 6e73  unt = self.trans
+0000cb10: 6163 7469 6f6e 5669 6577 2e72 6f77 436f  actionView.rowCo
+0000cb20: 756e 7428 290d 0a0d 0a20 2020 2020 2020  unt()....       
+0000cb30: 2069 6620 7365 6c66 2e65 6e74 7279 5f64   if self.entry_d
+0000cb40: 6174 6120 6973 204e 6f6e 653a 0d0a 2020  ata is None:..  
+0000cb50: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000cb60: 6f74 6966 7928 2244 6174 6120 6973 2065  otify("Data is e
+0000cb70: 6d70 7479 206f 7220 636f 7272 7570 7465  mpty or corrupte
+0000cb80: 642e 2053 6f6d 6574 6869 6e67 2077 656e  d. Something wen
+0000cb90: 7420 7772 6f6e 6722 2c20 7469 746c 653d  t wrong", title=
+0000cba0: 2246 6174 616c 2045 7272 6f72 2229 0d0a  "Fatal Error")..
+0000cbb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000cbc0: 726e 0d0a 0d0a 2020 2020 2020 2020 6966  rn....        if
+0000cbd0: 2072 6f77 5f63 6f75 6e74 203c 206c 656e   row_count < len
+0000cbe0: 2873 656c 662e 656e 7472 795f 6461 7461  (self.entry_data
+0000cbf0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000cc00: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+0000cc10: 656e 2873 656c 662e 656e 7472 795f 6461  en(self.entry_da
+0000cc20: 7461 292d 726f 775f 636f 756e 7429 3a0d  ta)-row_count):.
+0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc40: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000cc50: 6e56 6965 772e 696e 7365 7274 526f 7728  nView.insertRow(
+0000cc60: 726f 775f 636f 756e 7429 0d0a 0d0a 2020  row_count)....  
+0000cc70: 2020 2020 2020 7365 6c66 2e64 7261 7763        self.drawc
+0000cc80: 616e 7661 732e 636c 6561 7228 290d 0a20  anvas.clear().. 
+0000cc90: 2020 2020 2020 2073 656c 662e 6669 6c74         self.filt
+0000cca0: 6572 436f 6d62 6f2e 636c 6561 7228 290d  erCombo.clear().
+0000ccb0: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+0000ccc0: 6c74 6572 5f65 6e74 7269 6573 203d 205b  lter_entries = [
+0000ccd0: 5d0d 0a0d 0a20 2020 2020 2020 2074 7279  ]....        try
+0000cce0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000ccf0: 6f72 2069 2c20 6461 7461 2069 6e20 656e  or i, data in en
+0000cd00: 756d 6572 6174 6528 7365 6c66 2e65 6e74  umerate(self.ent
+0000cd10: 7279 5f64 6174 6129 3a0d 0a20 2020 2020  ry_data):..     
+0000cd20: 2020 2020 2020 2020 2020 2023 2065 7869             # exi
+0000cd30: 7374 7331 203d 2073 656c 662e 6472 6177  sts1 = self.draw
+0000cd40: 6361 6e76 6173 2e63 6865 636b 5f65 7869  canvas.check_exi
+0000cd50: 7374 2864 6174 615b 2261 6765 6e74 3122  st(data["agent1"
+0000cd60: 5d2e 6361 7069 7461 6c69 7a65 2829 290d  ].capitalize()).
+0000cd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd80: 2023 2065 7869 7374 7332 203d 2073 656c   # exists2 = sel
+0000cd90: 662e 6472 6177 6361 6e76 6173 2e63 6865  f.drawcanvas.che
+0000cda0: 636b 5f65 7869 7374 2864 6174 615b 2261  ck_exist(data["a
+0000cdb0: 6765 6e74 3222 5d2e 6361 7069 7461 6c69  gent2"].capitali
+0000cdc0: 7a65 2829 290d 0a0d 0a20 2020 2020 2020  ze())....       
+0000cdd0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000cde0: 5f61 6765 6e74 3120 3d20 6361 6d65 6c28  _agent1 = camel(
+0000cdf0: 6461 7461 5b22 6167 656e 7431 225d 290d  data["agent1"]).
+0000ce00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce10: 2020 2020 206e 6577 5f61 6765 6e74 3220       new_agent2 
+0000ce20: 3d20 6361 6d65 6c28 6461 7461 5b22 6167  = camel(data["ag
+0000ce30: 656e 7432 225d 290d 0a20 2020 2020 2020  ent2"])..       
+0000ce40: 2020 2020 2020 2020 2020 2020 2062 6f78               box
+0000ce50: 3120 3d20 7365 6c66 2e64 7261 7763 616e  1 = self.drawcan
+0000ce60: 7661 732e 6164 645f 6167 656e 7428 6e65  vas.add_agent(ne
+0000ce70: 775f 6167 656e 7431 2920 2320 2e63 6170  w_agent1) # .cap
+0000ce80: 6974 616c 697a 6528 2929 0d0a 2020 2020  italize())..    
+0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cea0: 626f 7832 203d 2073 656c 662e 6472 6177  box2 = self.draw
+0000ceb0: 6361 6e76 6173 2e61 6464 5f61 6765 6e74  canvas.add_agent
+0000cec0: 286e 6577 5f61 6765 6e74 3229 2023 2e63  (new_agent2) #.c
+0000ced0: 6170 6974 616c 697a 6528 2929 0d0a 0d0a  apitalize())....
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 2020 2020 2320 636f 7272 6563 7420 6e75      # correct nu
+0000cf00: 6d62 6572 206f 6620 636f 6e6e 6563 7469  mber of connecti
+0000cf10: 6f6e 7320 666f 7220 6578 6973 7469 6e67  ons for existing
+0000cf20: 2061 6765 6e74 730d 0a20 2020 2020 2020   agents..       
+0000cf30: 2020 2020 2020 2020 2020 2020 2062 6f78               box
+0000cf40: 312e 6e5f 636f 6e6e 6563 7469 6f6e 7320  1.n_connections 
+0000cf50: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000cf60: 2020 2020 2020 2020 2062 6f78 322e 6e5f           box2.n_
+0000cf70: 636f 6e6e 6563 7469 6f6e 7320 3d20 300d  connections = 0.
+0000cf80: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+0000cf90: 2023 2075 7064 6174 6520 7468 6520 6461   # update the da
+0000cfa0: 7461 0d0a 2020 2020 2020 2020 2020 2020  ta..            
+0000cfb0: 666f 7220 692c 2064 6174 6120 696e 2065  for i, data in e
+0000cfc0: 6e75 6d65 7261 7465 2873 656c 662e 656e  numerate(self.en
+0000cfd0: 7472 795f 6461 7461 293a 0d0a 2020 2020  try_data):..    
+0000cfe0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000cff0: 7428 6461 7461 290d 0a0d 0a20 2020 2020  t(data)....     
+0000d000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d010: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+0000d020: 7365 7449 7465 6d28 692c 2030 2c20 5154  setItem(i, 0, QT
+0000d030: 6162 6c65 5769 6467 6574 4974 656d 2864  ableWidgetItem(d
+0000d040: 6174 615b 2273 7562 6a65 6374 225d 2929  ata["subject"]))
+0000d050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d060: 2020 7365 6c66 2e74 7261 6e73 6163 7469    self.transacti
+0000d070: 6f6e 5669 6577 2e73 6574 4974 656d 2869  onView.setItem(i
+0000d080: 2c20 312c 2051 5461 626c 6557 6964 6765  , 1, QTableWidge
+0000d090: 7449 7465 6d28 6361 6d65 6c28 6461 7461  tItem(camel(data
+0000d0a0: 5b22 6167 656e 7431 225d 2929 2920 2320  ["agent1"]))) # 
+0000d0b0: 2e63 6170 6974 616c 697a 6528 2929 290d  .capitalize())).
+0000d0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d0d0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000d0e0: 6e56 6965 772e 7365 7449 7465 6d28 692c  nView.setItem(i,
+0000d0f0: 2032 2c20 5154 6162 6c65 5769 6467 6574   2, QTableWidget
+0000d100: 4974 656d 2863 616d 656c 2864 6174 615b  Item(camel(data[
+0000d110: 2261 6765 6e74 3222 5d29 2929 2023 202e  "agent2"]))) # .
+0000d120: 6361 7069 7461 6c69 7a65 2829 2929 0d0a  capitalize()))..
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+0000d150: 5669 6577 2e73 6574 4974 656d 2869 2c20  View.setItem(i, 
+0000d160: 332c 2051 5461 626c 6557 6964 6765 7449  3, QTableWidgetI
+0000d170: 7465 6d28 6461 7461 5b22 7368 6f72 746e  tem(data["shortn
+0000d180: 616d 6522 5d29 290d 0a20 2020 2020 2020  ame"]))..       
+0000d190: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000d1a0: 616e 7361 6374 696f 6e56 6965 772e 7365  ansactionView.se
+0000d1b0: 7449 7465 6d28 692c 2034 2c20 5154 6162  tItem(i, 4, QTab
+0000d1c0: 6c65 5769 6467 6574 4974 656d 2864 6174  leWidgetItem(dat
+0000d1d0: 615b 226b 696e 6422 5d29 290d 0a20 2020  a["kind"]))..   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d1f0: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+0000d200: 772e 7365 7449 7465 6d28 692c 2035 2c20  w.setItem(i, 5, 
+0000d210: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+0000d220: 2873 7472 2864 6174 615b 2275 6e69 2d64  (str(data["uni-d
+0000d230: 6972 6563 7469 6f6e 616c 225d 2929 290d  irectional"]))).
+0000d240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d250: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000d260: 6e56 6965 772e 7365 7449 7465 6d28 692c  nView.setItem(i,
+0000d270: 2036 2c20 5154 6162 6c65 5769 6467 6574   6, QTableWidget
+0000d280: 4974 656d 2873 7472 2864 6174 615b 2271  Item(str(data["q
+0000d290: 7561 6e74 6974 7922 5d29 2929 0d0a 2020  uantity"])))..  
+0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000d2b0: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+0000d2c0: 5669 6577 2e73 656c 6563 7469 6f6e 4d6f  View.selectionMo
+0000d2d0: 6465 6c28 292e 7365 6c65 6374 6564 526f  del().selectedRo
+0000d2e0: 7773 2829 0d0a 0d0a 2020 2020 2020 2020  ws()....        
+0000d2f0: 2020 2020 2020 2020 626f 7831 203d 2073          box1 = s
+0000d300: 656c 662e 6472 6177 6361 6e76 6173 2e61  elf.drawcanvas.a
+0000d310: 6464 5f61 6765 6e74 2863 616d 656c 2864  dd_agent(camel(d
+0000d320: 6174 615b 2261 6765 6e74 3122 5d29 2920  ata["agent1"])) 
+0000d330: 232e 6361 7069 7461 6c69 7a65 2829 290d  #.capitalize()).
+0000d340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d350: 2062 6f78 3220 3d20 7365 6c66 2e64 7261   box2 = self.dra
+0000d360: 7763 616e 7661 732e 6164 645f 6167 656e  wcanvas.add_agen
+0000d370: 7428 6361 6d65 6c28 6461 7461 5b22 6167  t(camel(data["ag
+0000d380: 656e 7432 225d 2929 2023 2e63 6170 6974  ent2"])) #.capit
+0000d390: 616c 697a 6528 2929 0d0a 0d0a 2020 2020  alize())....    
+0000d3a0: 2020 2020 2020 2020 2020 2020 6d79 5f69              my_i
+0000d3b0: 7465 6d73 203d 205b 5d0d 0a0d 0a20 2020  tems = []....   
+0000d3c0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+0000d3d0: 656e 7472 6965 7320 3d20 225c 6e22 2e6a  entries = "\n".j
+0000d3e0: 6f69 6e28 5b64 6174 615b 226c 3122 5d2c  oin([data["l1"],
+0000d3f0: 2064 6174 615b 2261 3122 5d2c 2064 6174   data["a1"], dat
+0000d400: 615b 2265 3122 5d2c 2064 6174 615b 226c  a["e1"], data["l
+0000d410: 3222 5d2c 2064 6174 615b 2261 3222 5d2c  2"], data["a2"],
+0000d420: 2064 6174 615b 2265 3222 5d5d 290d 0a20   data["e2"]]).. 
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d440: 6f72 2073 7562 5f69 7465 6d20 696e 2061  or sub_item in a
+0000d450: 6c6c 656e 7472 6965 732e 7370 6c69 7428  llentries.split(
+0000d460: 225c 6e22 293a 0d0a 2020 2020 2020 2020  "\n"):..        
+0000d470: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d480: 7375 625f 656e 7472 7920 696e 2073 7562  sub_entry in sub
+0000d490: 5f69 7465 6d2e 7370 6c69 7428 225c 6e22  _item.split("\n"
+0000d4a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000d4b0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
+0000d4c0: 7920 3d20 7375 625f 656e 7472 792e 7265  y = sub_entry.re
+0000d4d0: 706c 6163 6528 222d 222c 2222 292e 7265  place("-","").re
+0000d4e0: 706c 6163 6528 222b 222c 2222 292e 7374  place("+","").st
+0000d4f0: 7269 7028 290d 0a20 2020 2020 2020 2020  rip()..         
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d510: 6620 656e 7472 7920 213d 2020 2222 3a0d  f entry !=  "":.
+0000d520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d530: 2020 2020 2020 2020 2020 2020 206d 795f               my_
+0000d540: 6974 656d 732e 6170 7065 6e64 2865 6e74  items.append(ent
+0000d550: 7279 290d 0a0d 0a20 2020 2020 2020 2020  ry)....         
+0000d560: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
+0000d570: 6361 6e76 6173 2e61 6464 5f63 6f6e 6e65  canvas.add_conne
+0000d580: 6374 696f 6e28 626f 7831 2c20 626f 7832  ction(box1, box2
+0000d590: 2c20 6e61 6d65 3d20 6461 7461 5b22 7368  , name= data["sh
+0000d5a0: 6f72 746e 616d 6522 5d2c 7375 626a 6563  ortname"],subjec
+0000d5b0: 743d 6461 7461 5b22 7375 626a 6563 7422  t=data["subject"
+0000d5c0: 5d2c 6974 656d 733d 6d79 5f69 7465 6d73  ],items=my_items
+0000d5d0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000d5e0: 2020 2020 2023 2075 7064 6174 6520 7468       # update th
+0000d5f0: 6520 6669 6c74 6572 2076 616c 7565 730d  e filter values.
+0000d600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d610: 2066 6f72 2065 6e74 7279 2069 6e20 6d79   for entry in my
+0000d620: 5f69 7465 6d73 3a0d 0a20 2020 2020 2020  _items:..       
+0000d630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d640: 656e 7472 7920 6e6f 7420 696e 2073 656c  entry not in sel
+0000d650: 662e 6669 6c74 6572 5f65 6e74 7269 6573  f.filter_entries
+0000d660: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d680: 6669 6c74 6572 5f65 6e74 7269 6573 2e61  filter_entries.a
+0000d690: 7070 656e 6428 656e 7472 7929 0d0a 0d0a  ppend(entry)....
+0000d6a0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0000d6b0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0000d6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d6d0: 2e6e 6f74 6966 7928 7374 7228 6529 2b22  .notify(str(e)+"
+0000d6e0: 5c6e 2220 2b20 7374 7228 6461 7461 292c  \n" + str(data),
+0000d6f0: 7469 746c 653d 2245 7272 6f72 2229 0d0a  title="Error")..
+0000d700: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+0000d710: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0000d720: 6172 6368 2066 6f72 2061 206d 6174 6368  arch for a match
+0000d730: 2069 6e20 7468 6520 6669 6c74 6572 0d0a   in the filter..
+0000d740: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000d750: 756e 645f 6964 7873 203d 205b 5d0d 0a20  und_idxs = [].. 
+0000d760: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+0000d770: 685f 7374 7220 3d20 7365 6c66 2e46 696c  h_str = self.Fil
+0000d780: 7465 726c 696e 6545 6469 742e 7465 7874  terlineEdit.text
+0000d790: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+0000d7a0: 2020 6966 2073 6561 7263 685f 7374 7220    if search_str 
+0000d7b0: 213d 2022 223a 0d0a 2020 2020 2020 2020  != "":..        
+0000d7c0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000d7f0: 2873 656c 662e 7472 616e 7361 6374 696f  (self.transactio
+0000d800: 6e56 6965 772e 726f 7743 6f75 6e74 2829  nView.rowCount()
+0000d810: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0000d820: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000d830: 7220 6a20 696e 2072 616e 6765 2873 656c  r j in range(sel
+0000d840: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+0000d850: 772e 636f 6c75 6d6e 436f 756e 7428 2929  w.columnCount())
+0000d860: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d880: 2065 6e74 7279 5f73 7472 203d 2073 656c   entry_str = sel
+0000d890: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+0000d8a0: 772e 6974 656d 2869 2c6a 292e 7465 7874  w.item(i,j).text
+0000d8b0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8d0: 2020 6966 2065 6e74 7279 5f73 7472 2e66    if entry_str.f
+0000d8e0: 696e 6428 7365 6172 6368 5f73 7472 2920  ind(search_str) 
+0000d8f0: 3e20 2d31 3a0d 0a0d 0a20 2020 2020 2020  > -1:....       
+0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d910: 2020 2020 2020 2020 2066 6f75 6e64 5f69           found_i
+0000d920: 6478 732e 6170 7065 6e64 2869 290d 0a20  dxs.append(i).. 
+0000d930: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d940: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000d950: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+0000d960: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000d970: 2822 4578 6365 7074 696f 6e3a 222c 2073  ("Exception:", s
+0000d980: 7472 2865 2929 0d0a 0d0a 2020 2020 2020  tr(e))....      
+0000d990: 2020 2020 2020 666f 7220 666f 756e 645f        for found_
+0000d9a0: 6964 7820 696e 2066 6f75 6e64 5f69 6478  idx in found_idx
+0000d9b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0000d9c0: 2020 2020 2320 6869 6768 6c69 6768 7420      # highlight 
+0000d9d0: 6f63 6375 7261 6e63 6573 0d0a 2020 2020  occurances..    
+0000d9e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d9f0: 6a20 696e 2072 616e 6765 2873 656c 662e  j in range(self.
+0000da00: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+0000da10: 636f 6c75 6d6e 436f 756e 7428 2929 3a0d  columnCount()):.
+0000da20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da30: 2020 2020 2074 7279 3a0d 0a0d 0a20 2020       try:....   
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2020 2069 6620 7365 6c66 2e74 6865       if self.the
+0000da60: 6d65 5f6d 616e 6167 6572 2e74 6865 6d65  me_manager.theme
+0000da70: 203d 3d20 2262 7269 6768 7422 3a0d 0a0d   == "bright":...
+0000da80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da90: 2020 2020 2020 2020 2020 2020 2023 206c               # l
+0000daa0: 6967 6874 206d 6f64 650d 0a20 2020 2020  ight mode..     
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
+0000dad0: 7361 6374 696f 6e56 6965 772e 6974 656d  sactionView.item
+0000dae0: 2866 6f75 6e64 5f69 6478 2c20 6a29 2e73  (found_idx, j).s
+0000daf0: 6574 4261 636b 6772 6f75 6e64 2851 7447  etBackground(QtG
+0000db00: 7569 2e51 436f 6c6f 7228 3232 372c 2031  ui.QColor(227, 1
+0000db10: 3636 2c20 3136 3629 290d 0a20 2020 2020  66, 166))..     
+0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db30: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
+0000db40: 7361 6374 696f 6e56 6965 772e 6974 656d  sactionView.item
+0000db50: 2866 6f75 6e64 5f69 6478 2c20 6a29 2e73  (found_idx, j).s
+0000db60: 6574 466f 7265 6772 6f75 6e64 2851 7447  etForeground(QtG
+0000db70: 7569 2e51 436f 6c6f 7228 3138 302c 2031  ui.QColor(180, 1
+0000db80: 382c 2031 3829 290d 0a0d 0a20 2020 2020  8, 18))....     
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 2020 2065 6c73 653a 0d0a 0d0a 2020 2020     else:....    
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 2020 2020 2020 2020 2320 6461 726b 206d          # dark m
+0000dbd0: 6f64 650d 0a20 2020 2020 2020 2020 2020  ode..           
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000dc00: 6e56 6965 772e 6974 656d 2866 6f75 6e64  nView.item(found
+0000dc10: 5f69 6478 2c20 6a29 2e73 6574 4261 636b  _idx, j).setBack
+0000dc20: 6772 6f75 6e64 2851 7447 7569 2e51 436f  ground(QtGui.QCo
+0000dc30: 6c6f 7228 3132 302c 2031 3230 2c20 3132  lor(120, 120, 12
+0000dc40: 3029 290d 0a20 2020 2020 2020 2020 2020  0))..           
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000dc70: 6e56 6965 772e 6974 656d 2866 6f75 6e64  nView.item(found
+0000dc80: 5f69 6478 2c20 6a29 2e73 6574 466f 7265  _idx, j).setFore
+0000dc90: 6772 6f75 6e64 2851 7447 7569 2e51 436f  ground(QtGui.QCo
+0000dca0: 6c6f 7228 3530 2c20 3530 2c20 3530 2929  lor(50, 50, 50))
+0000dcb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000dcc0: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
+0000dcd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dce0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 2020 2020 2020 2023 2061 766f 6964 7320         # avoids 
+0000dd10: 4e6f 6e65 2070 6f69 6e74 6572 2077 6865  None pointer whe
+0000dd20: 6e20 6120 7472 616e 7361 6374 696f 6e20  n a transaction 
+0000dd30: 6973 2064 656c 6574 6564 0d0a 2020 2020  is deleted..    
+0000dd40: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+0000dd50: 2020 2020 2020 2020 2070 6173 730d 0a0d           pass...
+0000dd60: 0a0d 0a20 2020 2020 2020 2066 6f72 2065  ...        for e
+0000dd70: 6e74 7279 2069 6e20 7365 6c66 2e66 696c  ntry in self.fil
+0000dd80: 7465 725f 656e 7472 6965 733a 0d0a 2020  ter_entries:..  
+0000dd90: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000dda0: 696c 7465 7243 6f6d 626f 2e61 6464 4974  ilterCombo.addIt
+0000ddb0: 656d 2865 6e74 7279 290d 0a0d 0a20 2020  em(entry)....   
 0000ddc0: 2020 2020 2073 656c 662e 6472 6177 6361       self.drawca
-0000ddd0: 6e76 6173 2e75 7064 6174 6528 290d 0a20  nvas.update().. 
-0000dde0: 2020 2020 2020 2073 656c 662e 6d61 6465         self.made
-0000ddf0: 5f63 6861 6e67 6573 203d 2046 616c 7365  _changes = False
-0000de00: 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020 6465  ..........    de
-0000de10: 6620 6d6f 7665 5f64 6f77 6e28 7365 6c66  f move_down(self
-0000de20: 293a 0d0a 2020 2020 2020 2020 2320 6d6f  ):..        # mo
-0000de30: 7665 2073 656c 6563 7465 6420 7472 616e  ve selected tran
-0000de40: 7361 6374 696f 6e20 7570 2069 6e20 7461  saction up in ta
-0000de50: 626c 650d 0a20 2020 2020 2020 2073 656c  ble..        sel
-0000de60: 6563 7465 645f 726f 7773 203d 2073 6f72  ected_rows = sor
-0000de70: 7465 6428 7365 7428 696e 6465 782e 726f  ted(set(index.ro
-0000de80: 7728 2920 666f 7220 696e 6465 7820 696e  w() for index in
-0000de90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000deb0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000dec0: 2e73 656c 6563 7465 6449 6e64 6578 6573  .selectedIndexes
-0000ded0: 2829 2929 0d0a 0d0a 2020 2020 2020 2020  ()))....        
-0000dee0: 6966 206c 656e 2873 656c 6563 7465 645f  if len(selected_
-0000def0: 726f 7773 2920 3d3d 2030 3a0d 0a20 2020  rows) == 0:..   
-0000df00: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000df10: 6e6f 2073 656c 6563 7465 6420 726f 7773  no selected rows
-0000df20: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000df30: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
-0000df40: 2020 7365 6c65 6374 696f 6e20 3d20 7365    selection = se
-0000df50: 6c65 6374 6564 5f72 6f77 735b 305d 0d0a  lected_rows[0]..
-0000df60: 0d0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
-0000df70: 5f6f 665f 6974 656d 7320 3d20 7365 6c66  _of_items = self
-0000df80: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000df90: 2e72 6f77 436f 756e 7428 290d 0a20 2020  .rowCount()..   
-0000dfa0: 2020 2020 206e 756d 6265 725f 6f66 5f63       number_of_c
-0000dfb0: 6f6c 756d 6e73 203d 2073 656c 662e 7472  olumns = self.tr
-0000dfc0: 616e 7361 6374 696f 6e56 6965 772e 636f  ansactionView.co
-0000dfd0: 6c75 6d6e 436f 756e 7428 290d 0a0d 0a20  lumnCount().... 
-0000dfe0: 2020 2020 2020 2074 7279 3a0d 0a0d 0a20         try:.... 
-0000dff0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e000: 6c65 6374 696f 6e20 3c20 6e75 6d62 6572  lection < number
-0000e010: 5f6f 665f 6974 656d 732d 313a 0d0a 2020  _of_items-1:..  
-0000e020: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000e030: 7272 656e 7452 6f77 203d 2073 656c 662e  rrentRow = self.
-0000e040: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-0000e050: 6375 7272 656e 7452 6f77 2829 0d0a 0d0a  currentRow()....
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 666f 7220 6a20 696e 2072 616e 6765 286e  for j in range(n
-0000e080: 756d 6265 725f 6f66 5f63 6f6c 756d 6e73  umber_of_columns
-0000e090: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000e0a0: 2020 2020 2020 2020 6375 7272 656e 7449          currentI
-0000e0b0: 7465 6d20 3d20 7365 6c66 2e74 7261 6e73  tem = self.trans
-0000e0c0: 6163 7469 6f6e 5669 6577 2e74 616b 6549  actionView.takeI
-0000e0d0: 7465 6d28 6375 7272 656e 7452 6f77 2c6a  tem(currentRow,j
-0000e0e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e0f0: 2020 2020 2020 2073 7769 7463 6849 7465         switchIte
-0000e100: 6d20 3d20 7365 6c66 2e74 7261 6e73 6163  m = self.transac
-0000e110: 7469 6f6e 5669 6577 2e74 616b 6549 7465  tionView.takeIte
-0000e120: 6d28 6375 7272 656e 7452 6f77 2b31 2c6a  m(currentRow+1,j
-0000e130: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000e140: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-0000e150: 616e 7361 6374 696f 6e56 6965 772e 7365  ansactionView.se
-0000e160: 7449 7465 6d28 6375 7272 656e 7452 6f77  tItem(currentRow
-0000e170: 202b 2031 2c20 6a2c 2063 7572 7265 6e74   + 1, j, current
-0000e180: 4974 656d 290d 0a20 2020 2020 2020 2020  Item)..         
-0000e190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e1a0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-0000e1b0: 7365 7449 7465 6d28 6375 7272 656e 7452  setItem(currentR
-0000e1c0: 6f77 2c20 6a2c 2073 7769 7463 6849 7465  ow, j, switchIte
-0000e1d0: 6d29 0d0a 0d0a 2020 2020 2020 2020 2020  m)....          
-0000e1e0: 2020 2020 2020 2020 2020 7377 6974 6368            switch
-0000e1f0: 5f65 6e74 7279 203d 2073 656c 662e 656e  _entry = self.en
-0000e200: 7472 795f 6461 7461 5b63 7572 7265 6e74  try_data[current
-0000e210: 526f 772b 315d 0d0a 2020 2020 2020 2020  Row+1]..        
-0000e220: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-0000e230: 656e 745f 656e 7472 7920 3d20 7365 6c66  ent_entry = self
-0000e240: 2e65 6e74 7279 5f64 6174 615b 6375 7272  .entry_data[curr
-0000e250: 656e 7452 6f77 5d0d 0a0d 0a20 2020 2020  entRow]....     
-0000e260: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e270: 656c 662e 656e 7472 795f 6461 7461 5b63  elf.entry_data[c
-0000e280: 7572 7265 6e74 526f 775d 203d 2073 7769  urrentRow] = swi
-0000e290: 7463 685f 656e 7472 790d 0a20 2020 2020  tch_entry..     
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e2b0: 656c 662e 656e 7472 795f 6461 7461 5b63  elf.entry_data[c
-0000e2c0: 7572 7265 6e74 526f 772b 315d 203d 2063  urrentRow+1] = c
-0000e2d0: 7572 7265 6e74 5f65 6e74 7279 0d0a 0d0a  urrent_entry....
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
-0000e300: 5669 6577 2e63 6c65 6172 5365 6c65 6374  View.clearSelect
-0000e310: 696f 6e28 290d 0a20 2020 2020 2020 2020  ion()..         
-0000e320: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
-0000e330: 7361 6374 696f 6e56 6965 772e 7365 7443  sactionView.setC
-0000e340: 7572 7265 6e74 4365 6c6c 2863 7572 7265  urrentCell(curre
-0000e350: 6e74 526f 772b 312c 3029 0d0a 0d0a 2020  ntRow+1,0)....  
-0000e360: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0000e370: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-0000e380: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000e390: 6f74 6966 7928 2265 7272 6f72 3a20 222b  otify("error: "+
-0000e3a0: 7374 7228 6529 2c20 7469 746c 653d 2245  str(e), title="E
-0000e3b0: 7272 6f72 2229 0d0a 0d0a 0d0a 2020 2020  rror")......    
-0000e3c0: 6465 6620 6d6f 7665 5f75 7028 7365 6c66  def move_up(self
-0000e3d0: 293a 0d0a 2020 2020 2020 2020 2320 6d6f  ):..        # mo
-0000e3e0: 7665 2073 656c 6563 7465 6420 7472 616e  ve selected tran
-0000e3f0: 7361 6374 696f 6e20 7570 2069 6e20 7461  saction up in ta
-0000e400: 626c 650d 0a20 2020 2020 2020 2073 656c  ble..        sel
-0000e410: 6563 7465 645f 726f 7773 203d 2073 6f72  ected_rows = sor
-0000e420: 7465 6428 7365 7428 696e 6465 782e 726f  ted(set(index.ro
-0000e430: 7728 2920 666f 7220 696e 6465 7820 696e  w() for index in
-0000e440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e460: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000e470: 2e73 656c 6563 7465 6449 6e64 6578 6573  .selectedIndexes
-0000e480: 2829 2929 0d0a 0d0a 2020 2020 2020 2020  ()))....        
-0000e490: 6966 206c 656e 2873 656c 6563 7465 645f  if len(selected_
-0000e4a0: 726f 7773 2920 3d3d 2030 3a0d 0a20 2020  rows) == 0:..   
-0000e4b0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000e4c0: 6e6f 2073 656c 6563 7465 6420 726f 7773  no selected rows
-0000e4d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000e4e0: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
-0000e4f0: 2020 7365 6c65 6374 696f 6e20 3d20 7365    selection = se
-0000e500: 6c65 6374 6564 5f72 6f77 735b 305d 0d0a  lected_rows[0]..
-0000e510: 0d0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
-0000e520: 5f6f 665f 6974 656d 7320 3d20 7365 6c66  _of_items = self
-0000e530: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000e540: 2e72 6f77 436f 756e 7428 290d 0a20 2020  .rowCount()..   
-0000e550: 2020 2020 206e 756d 6265 725f 6f66 5f63       number_of_c
-0000e560: 6f6c 756d 6e73 203d 2073 656c 662e 7472  olumns = self.tr
-0000e570: 616e 7361 6374 696f 6e56 6965 772e 636f  ansactionView.co
-0000e580: 6c75 6d6e 436f 756e 7428 290d 0a0d 0a20  lumnCount().... 
-0000e590: 2020 2020 2020 2074 7279 3a0d 0a0d 0a20         try:.... 
-0000e5a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e5b0: 6c65 6374 696f 6e20 3e3d 2031 3a0d 0a20  lection >= 1:.. 
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000e5d0: 7572 7265 6e74 526f 7720 3d20 7365 6c66  urrentRow = self
-0000e5e0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000e5f0: 2e63 7572 7265 6e74 526f 7728 290d 0a0d  .currentRow()...
-0000e600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e610: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0000e620: 6e75 6d62 6572 5f6f 665f 636f 6c75 6d6e  number_of_column
-0000e630: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-0000e640: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000e650: 4974 656d 203d 2073 656c 662e 7472 616e  Item = self.tran
-0000e660: 7361 6374 696f 6e56 6965 772e 7461 6b65  sactionView.take
-0000e670: 4974 656d 2863 7572 7265 6e74 526f 772c  Item(currentRow,
-0000e680: 6a29 0d0a 2020 2020 2020 2020 2020 2020  j)..            
-0000e690: 2020 2020 2020 2020 7377 6974 6368 4974          switchIt
-0000e6a0: 656d 203d 2073 656c 662e 7472 616e 7361  em = self.transa
-0000e6b0: 6374 696f 6e56 6965 772e 7461 6b65 4974  ctionView.takeIt
-0000e6c0: 656d 2863 7572 7265 6e74 526f 772d 312c  em(currentRow-1,
-0000e6d0: 6a29 0d0a 0d0a 2020 2020 2020 2020 2020  j)....          
-0000e6e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000e6f0: 7261 6e73 6163 7469 6f6e 5669 6577 2e73  ransactionView.s
-0000e700: 6574 4974 656d 2863 7572 7265 6e74 526f  etItem(currentRo
-0000e710: 7720 2d20 312c 206a 2c20 6375 7272 656e  w - 1, j, curren
-0000e720: 7449 7465 6d29 0d0a 2020 2020 2020 2020  tItem)..        
-0000e730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e740: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000e750: 2e73 6574 4974 656d 2863 7572 7265 6e74  .setItem(current
-0000e760: 526f 772c 206a 2c20 7377 6974 6368 4974  Row, j, switchIt
-0000e770: 656d 290d 0a0d 0a20 2020 2020 2020 2020  em)....         
-0000e780: 2020 2020 2020 2020 2020 2073 7769 7463             switc
-0000e790: 685f 656e 7472 7920 3d20 7365 6c66 2e65  h_entry = self.e
-0000e7a0: 6e74 7279 5f64 6174 615b 6375 7272 656e  ntry_data[curren
-0000e7b0: 7452 6f77 2d31 5d0d 0a20 2020 2020 2020  tRow-1]..       
-0000e7c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0000e7d0: 7265 6e74 5f65 6e74 7279 203d 2073 656c  rent_entry = sel
-0000e7e0: 662e 656e 7472 795f 6461 7461 5b63 7572  f.entry_data[cur
-0000e7f0: 7265 6e74 526f 775d 0d0a 0d0a 2020 2020  rentRow]....    
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
-0000e820: 6375 7272 656e 7452 6f77 5d20 3d20 7377  currentRow] = sw
-0000e830: 6974 6368 5f65 6e74 7279 0d0a 2020 2020  itch_entry..    
-0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e850: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
-0000e860: 6375 7272 656e 7452 6f77 2d31 5d20 3d20  currentRow-1] = 
-0000e870: 6375 7272 656e 745f 656e 7472 790d 0a0d  current_entry...
-0000e880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e890: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
-0000e8a0: 6e56 6965 772e 636c 6561 7253 656c 6563  nView.clearSelec
-0000e8b0: 7469 6f6e 2829 0d0a 2020 2020 2020 2020  tion()..        
-0000e8c0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000e8d0: 6e73 6163 7469 6f6e 5669 6577 2e73 6574  nsactionView.set
-0000e8e0: 4375 7272 656e 7443 656c 6c28 6375 7272  CurrentCell(curr
-0000e8f0: 656e 7452 6f77 2d31 2c30 290d 0a0d 0a20  entRow-1,0).... 
-0000e900: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-0000e910: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-0000e920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e930: 6e6f 7469 6679 2822 6572 726f 723a 2022  notify("error: "
-0000e940: 2b73 7472 2865 292c 2074 6974 6c65 3d22  +str(e), title="
-0000e950: 4572 726f 7222 290d 0a0d 0a20 2020 2064  Error")....    d
-0000e960: 6566 2064 6174 615f 7365 6c65 6374 2873  ef data_select(s
-0000e970: 656c 6629 3a0d 0a0d 0a20 2020 2020 2020  elf):....       
-0000e980: 2023 7365 6c65 6374 6564 5f72 6f77 7320   #selected_rows 
-0000e990: 3d20 7365 6c66 2e74 7261 6e73 6163 7469  = self.transacti
-0000e9a0: 6f6e 5669 6577 2e73 656c 6563 7469 6f6e  onView.selection
-0000e9b0: 4d6f 6465 6c28 292e 7365 6c65 6374 6564  Model().selected
-0000e9c0: 526f 7773 2829 0d0a 2020 2020 2020 2020  Rows()..        
-0000e9d0: 7365 6c65 6374 6564 5f72 6f77 7320 3d20  selected_rows = 
-0000e9e0: 736f 7274 6564 2873 6574 2869 6e64 6578  sorted(set(index
-0000e9f0: 2e72 6f77 2829 2066 6f72 2069 6e64 6578  .row() for index
-0000ea00: 2069 6e0d 0a20 2020 2020 2020 2020 2020   in..           
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ea20: 656c 662e 7472 616e 7361 6374 696f 6e56  elf.transactionV
-0000ea30: 6965 772e 7365 6c65 6374 6564 496e 6465  iew.selectedInde
-0000ea40: 7865 7328 2929 290d 0a0d 0a20 2020 2020  xes()))....     
-0000ea50: 2020 2069 6620 6c65 6e28 7365 6c65 6374     if len(select
-0000ea60: 6564 5f72 6f77 7329 203d 3d20 303a 0d0a  ed_rows) == 0:..
-0000ea70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000ea80: 7428 226e 6f20 7365 6c65 6374 6564 2072  t("no selected r
-0000ea90: 6f77 7322 290d 0a20 2020 2020 2020 2020  ows")..         
-0000eaa0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-0000eab0: 2020 2020 2073 656c 6563 7469 6f6e 203d       selection =
-0000eac0: 2073 656c 6563 7465 645f 726f 7773 5b30   selected_rows[0
-0000ead0: 5d0d 0a0d 0a20 2020 2020 2020 2073 656c  ]....        sel
-0000eae0: 662e 726f 775f 7365 6c65 6374 2873 656c  f.row_select(sel
-0000eaf0: 6563 7469 6f6e 290d 0a20 2020 2020 2020  ection)..       
-0000eb00: 2073 656c 662e 6d61 6465 5f63 6861 6e67   self.made_chang
-0000eb10: 6573 203d 2046 616c 7365 0d0a 0d0a 0d0a  es = False......
-0000eb20: 2020 2020 6465 6620 6461 7461 5f73 656c      def data_sel
-0000eb30: 6563 745f 7768 6572 6528 7365 6c66 2c65  ect_where(self,e
-0000eb40: 7870 7229 3a0d 0a20 2020 2020 2020 2070  xpr):..        p
-0000eb50: 7269 6e74 2822 6461 7461 2073 656c 6563  rint("data selec
-0000eb60: 7420 7768 6572 6522 2c65 7870 7229 0d0a  t where",expr)..
-0000eb70: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-0000eb80: 696e 2072 616e 6765 2873 656c 662e 7472  in range(self.tr
-0000eb90: 616e 7361 6374 696f 6e56 6965 772e 726f  ansactionView.ro
-0000eba0: 7743 6f75 6e74 2829 293a 0d0a 2020 2020  wCount()):..    
-0000ebb0: 2020 2020 2020 2020 2020 2020 6d79 5f65              my_e
-0000ebc0: 6e74 7279 203d 2073 656c 662e 7472 616e  ntry = self.tran
-0000ebd0: 7361 6374 696f 6e56 6965 772e 6974 656d  sactionView.item
-0000ebe0: 2869 2c20 3329 2e74 6578 7428 290d 0a0d  (i, 3).text()...
-0000ebf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec00: 2070 7269 6e74 2822 2e2e 2e22 2c69 2c6d   print("...",i,m
-0000ec10: 795f 656e 7472 7929 0d0a 2020 2020 2020  y_entry)..      
-0000ec20: 2020 2020 2020 2020 2020 6966 206d 795f            if my_
-0000ec30: 656e 7472 7920 3d3d 2065 7870 7220 6f72  entry == expr or
-0000ec40: 206d 795f 656e 7472 792e 6c6f 7765 7228   my_entry.lower(
-0000ec50: 2920 3d3d 2065 7870 722e 6c6f 7765 7228  ) == expr.lower(
-0000ec60: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0000ec70: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000ec80: 6f77 5f73 656c 6563 7428 6929 0d0a 2020  ow_select(i)..  
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-0000ecb0: 6465 6620 726f 775f 7365 6c65 6374 2873  def row_select(s
-0000ecc0: 656c 662c 7365 6c65 6374 696f 6e29 3a0d  elf,selection):.
-0000ecd0: 0a0d 0a20 2020 2020 2020 2023 2063 6f6c  ...        # col
-0000ece0: 6f72 2074 6865 2073 656c 6563 7465 6420  or the selected 
-0000ecf0: 726f 770d 0a20 2020 2020 2020 2023 2067  row..        # g
-0000ed00: 6228 3233 332c 2032 3334 2c20 3232 3729  b(233, 234, 227)
-0000ed10: 3b0d 0a0d 0a20 2020 2020 2020 2073 656c  ;....        sel
-0000ed20: 662e 7365 6c65 6374 696f 6e5f 6964 7820  f.selection_idx 
-0000ed30: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 2020  = None....      
-0000ed40: 2020 6966 2073 656c 662e 6d61 6465 5f63    if self.made_c
-0000ed50: 6861 6e67 6573 3a0d 0a20 2020 2020 2020  hanges:..       
-0000ed60: 2020 2020 2079 6573 203d 2073 656c 662e       yes = self.
-0000ed70: 6173 6b5f 7175 6573 7469 6f6e 2822 5761  ask_question("Wa
-0000ed80: 726e 696e 6722 2c20 2259 6f75 2061 7265  rning", "You are
-0000ed90: 2061 626f 7574 2074 6f20 6368 616e 6765   about to change
-0000eda0: 2074 6f20 616e 6f74 6865 7220 7472 616e   to another tran
-0000edb0: 7361 6374 696f 6e20 616e 6420 7769 7468  saction and with
-0000edc0: 6472 6177 2074 6865 2063 6861 6e67 6573  draw the changes
-0000edd0: 2079 6f75 206d 6164 652e 2043 6f6e 7469   you made. Conti
-0000ede0: 6e75 653f 2229 0d0a 2020 2020 2020 2020  nue?")..        
-0000edf0: 2020 2020 6966 206e 6f74 2079 6573 3a0d      if not yes:.
-0000ee00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ee10: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-0000ee20: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-0000ee30: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000ee40: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-0000ee50: 6c65 6374 696f 6e5f 6964 7820 6973 206e  lection_idx is n
-0000ee60: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000ee70: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-0000ee80: 696e 2072 616e 6765 2873 656c 662e 7472  in range(self.tr
-0000ee90: 616e 7361 6374 696f 6e56 6965 772e 636f  ansactionView.co
-0000eea0: 6c75 6d6e 436f 756e 7428 2929 3a0d 0a20  lumnCount()):.. 
-0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eec0: 2020 2073 656c 662e 7472 616e 7361 6374     self.transact
-0000eed0: 696f 6e56 6965 772e 6974 656d 2873 656c  ionView.item(sel
-0000eee0: 662e 7365 6c65 6374 696f 6e5f 6964 782c  f.selection_idx,
-0000eef0: 2069 292e 7365 7442 6163 6b67 726f 756e   i).setBackgroun
-0000ef00: 6428 5174 4775 692e 5143 6f6c 6f72 2832  d(QtGui.QColor(2
-0000ef10: 3333 2c20 3233 342c 2032 3237 2929 0d0a  33, 234, 227))..
-0000ef20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef30: 2020 2020 7365 6c66 2e74 7261 6e73 6163      self.transac
-0000ef40: 7469 6f6e 5669 6577 2e73 6372 6f6c 6c54  tionView.scrollT
-0000ef50: 6f49 7465 6d28 7365 6c66 2e74 7261 6e73  oItem(self.trans
-0000ef60: 6163 7469 6f6e 5669 6577 2e69 7465 6d28  actionView.item(
-0000ef70: 7365 6c65 6374 696f 6e2c 2069 2929 0d0a  selection, i))..
-0000ef80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ef90: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-0000efa0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-0000efb0: 636f 6c75 6d6e 436f 756e 7428 2929 3a0d  columnCount()):.
-0000efc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000efd0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
-0000efe0: 6e56 6965 772e 6974 656d 2873 656c 6563  nView.item(selec
-0000eff0: 7469 6f6e 2c20 6929 2e73 6574 4261 636b  tion, i).setBack
-0000f000: 6772 6f75 6e64 2851 7447 7569 2e51 436f  ground(QtGui.QCo
-0000f010: 6c6f 7228 3539 2c20 3539 2c20 3135 3929  lor(59, 59, 159)
-0000f020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f030: 2020 2073 656c 662e 7472 616e 7361 6374     self.transact
-0000f040: 696f 6e56 6965 772e 7363 726f 6c6c 546f  ionView.scrollTo
-0000f050: 4974 656d 2873 656c 662e 7472 616e 7361  Item(self.transa
-0000f060: 6374 696f 6e56 6965 772e 6974 656d 2873  ctionView.item(s
-0000f070: 656c 6563 7469 6f6e 2c20 6929 290d 0a20  election, i)).. 
-0000f080: 2020 2020 2020 2020 2020 2022 2222 0d0a             """..
-0000f090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f0a0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
-0000f0b0: 2e63 6c65 6172 5365 6c65 6374 696f 6e28  .clearSelection(
-0000f0c0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000f0d0: 656c 662e 7472 616e 7361 6374 696f 6e56  elf.transactionV
-0000f0e0: 6965 772e 7365 7443 7572 7265 6e74 4365  iew.setCurrentCe
-0000f0f0: 6c6c 2873 656c 6563 7469 6f6e 2c33 290d  ll(selection,3).
-0000f100: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2065  .......        e
-0000f110: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-0000f120: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-0000f130: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000f140: 2020 2020 2020 7365 6c66 2e73 656c 6563        self.selec
-0000f150: 7469 6f6e 5f69 6478 203d 2073 656c 6563  tion_idx = selec
-0000f160: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-0000f170: 2020 7072 696e 7428 2273 656c 6563 7469    print("selecti
-0000f180: 6f6e 222c 7365 6c65 6374 696f 6e29 0d0a  on",selection)..
-0000f190: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-0000f1a0: 7461 203d 2073 656c 662e 656e 7472 795f  ta = self.entry_
-0000f1b0: 6461 7461 5b73 656c 6563 7469 6f6e 5d0d  data[selection].
-0000f1c0: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-0000f1d0: 7269 6e74 2822 6461 7461 222c 2064 6174  rint("data", dat
-0000f1e0: 6129 0d0a 0d0a 2020 2020 2020 2020 2020  a)....          
-0000f1f0: 2020 7365 6c66 2e41 7373 6574 4c69 7374    self.AssetList
-0000f200: 4c65 6674 2e63 6c65 6172 2829 0d0a 2020  Left.clear()..  
-0000f210: 2020 2020 2020 2020 2020 7365 6c66 2e4c            self.L
-0000f220: 6961 6269 6c69 7479 4c69 7374 4c65 6674  iabilityListLeft
-0000f230: 2e63 6c65 6172 2829 0d0a 2020 2020 2020  .clear()..      
-0000f240: 2020 2020 2020 7365 6c66 2e4c 6961 6269        self.Liabi
-0000f250: 6c69 7479 4c69 7374 5269 6768 742e 636c  lityListRight.cl
-0000f260: 6561 7228 290d 0a20 2020 2020 2020 2020  ear()..         
-0000f270: 2020 2073 656c 662e 4173 7365 744c 6973     self.AssetLis
-0000f280: 7452 6967 6874 2e63 6c65 6172 2829 0d0a  tRight.clear()..
-0000f290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f2a0: 2e45 7175 6974 794c 6973 744c 6566 742e  .EquityListLeft.
-0000f2b0: 636c 6561 7228 290d 0a20 2020 2020 2020  clear()..       
-0000f2c0: 2020 2020 2073 656c 662e 4571 7569 7479       self.Equity
-0000f2d0: 4c69 7374 5269 6768 742e 636c 6561 7228  ListRight.clear(
-0000f2e0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000f2f0: 2073 656c 662e 4173 7365 744c 6973 744c   self.AssetListL
-0000f300: 6566 742e 7365 7450 6c61 696e 5465 7874  eft.setPlainText
-0000f310: 2864 6174 615b 2261 3122 5d29 0d0a 2020  (data["a1"])..  
-0000f320: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000f330: 7373 6574 4c69 7374 5269 6768 742e 7365  ssetListRight.se
-0000f340: 7450 6c61 696e 5465 7874 2864 6174 615b  tPlainText(data[
-0000f350: 2261 3222 5d29 0d0a 2020 2020 2020 2020  "a2"])..        
-0000f360: 2020 2020 7365 6c66 2e4c 6961 6269 6c69      self.Liabili
-0000f370: 7479 4c69 7374 4c65 6674 2e73 6574 506c  tyListLeft.setPl
-0000f380: 6169 6e54 6578 7428 6461 7461 5b22 6c31  ainText(data["l1
-0000f390: 225d 2920 2023 202b 6461 7461 5b22 6531  "])  # +data["e1
-0000f3a0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
-0000f3b0: 2073 656c 662e 4c69 6162 696c 6974 794c   self.LiabilityL
-0000f3c0: 6973 7452 6967 6874 2e73 6574 506c 6169  istRight.setPlai
-0000f3d0: 6e54 6578 7428 6461 7461 5b22 6c32 225d  nText(data["l2"]
-0000f3e0: 2920 2320 2b64 6174 615b 2265 3222 5d29  ) # +data["e2"])
-0000f3f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000f400: 6c66 2e45 7175 6974 794c 6973 744c 6566  lf.EquityListLef
-0000f410: 742e 7365 7450 6c61 696e 5465 7874 2864  t.setPlainText(d
-0000f420: 6174 615b 2265 3122 5d29 0d0a 2020 2020  ata["e1"])..    
-0000f430: 2020 2020 2020 2020 7365 6c66 2e45 7175          self.Equ
-0000f440: 6974 794c 6973 7452 6967 6874 2e73 6574  ityListRight.set
-0000f450: 506c 6169 6e54 6578 7428 6461 7461 5b22  PlainText(data["
-0000f460: 6532 225d 290d 0a0d 0a20 2020 2020 2020  e2"])....       
-0000f470: 2020 2020 2073 656c 662e 6167 656e 7431       self.agent1
-0000f480: 4564 6974 2e73 6574 5465 7874 2863 616d  Edit.setText(cam
-0000f490: 656c 2864 6174 615b 2261 6765 6e74 3122  el(data["agent1"
-0000f4a0: 5d29 2920 232e 6361 7069 7461 6c69 7a65  ])) #.capitalize
-0000f4b0: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
-0000f4c0: 2073 656c 662e 6167 656e 7432 4564 6974   self.agent2Edit
-0000f4d0: 2e73 6574 5465 7874 2863 616d 656c 2864  .setText(camel(d
-0000f4e0: 6174 615b 2261 6765 6e74 3222 5d29 2920  ata["agent2"])) 
-0000f4f0: 2320 2e63 6170 6974 616c 697a 6528 2929  # .capitalize())
-0000f500: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f510: 7365 6c66 2e72 6567 6973 7465 7246 6c6f  self.registerFlo
-0000f520: 7742 6f78 2e73 6574 4375 7272 656e 7449  wBox.setCurrentI
-0000f530: 6e64 6578 2873 656c 662e 7265 6769 7374  ndex(self.regist
-0000f540: 6572 466c 6f77 426f 782e 6669 6e64 5465  erFlowBox.findTe
-0000f550: 7874 2873 7472 2864 6174 615b 226c 6f67  xt(str(data["log
-0000f560: 2074 7261 6e73 6163 7469 6f6e 225d 2929   transaction"]))
-0000f570: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000f580: 2063 6173 6866 6c6f 7731 203d 2064 6174   cashflow1 = dat
-0000f590: 615b 2263 6173 6866 6c6f 7731 225d 206f  a["cashflow1"] o
-0000f5a0: 7220 224e 6f6e 6522 0d0a 2020 2020 2020  r "None"..      
-0000f5b0: 2020 2020 2020 6361 7368 666c 6f77 3220        cashflow2 
-0000f5c0: 3d20 6461 7461 5b22 6361 7368 666c 6f77  = data["cashflow
-0000f5d0: 3222 5d20 6f72 2022 4e6f 6e65 220d 0a20  2"] or "None".. 
-0000f5e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f5f0: 636f 6d62 6f43 6173 684c 6566 742e 7365  comboCashLeft.se
-0000f600: 7443 7572 7265 6e74 496e 6465 7828 7365  tCurrentIndex(se
-0000f610: 6c66 2e63 6f6d 626f 4361 7368 4c65 6674  lf.comboCashLeft
-0000f620: 2e66 696e 6454 6578 7428 7374 7228 6361  .findText(str(ca
-0000f630: 7368 666c 6f77 3129 2929 0d0a 2020 2020  shflow1)))..    
-0000f640: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-0000f650: 626f 4361 7368 5269 6768 742e 7365 7443  boCashRight.setC
-0000f660: 7572 7265 6e74 496e 6465 7828 7365 6c66  urrentIndex(self
-0000f670: 2e63 6f6d 626f 4361 7368 5269 6768 742e  .comboCashRight.
-0000f680: 6669 6e64 5465 7874 2873 7472 2863 6173  findText(str(cas
-0000f690: 6866 6c6f 7732 2929 290d 0a0d 0a20 2020  hflow2)))....   
-0000f6a0: 2020 2020 2020 2020 2074 7274 7970 6520           trtype 
-0000f6b0: 3d20 6461 7461 5b22 6b69 6e64 225d 206f  = data["kind"] o
-0000f6c0: 7220 224b 412d 3e4b 4122 0d0a 2020 2020  r "KA->KA"..    
-0000f6d0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000f6e0: 7454 7970 652e 7365 7443 7572 7265 6e74  tType.setCurrent
-0000f6f0: 496e 6465 7828 7365 6c66 2e65 6469 7454  Index(self.editT
-0000f700: 7970 652e 6669 6e64 5465 7874 2873 7472  ype.findText(str
-0000f710: 2874 7274 7970 6529 2929 0d0a 0d0a 2020  (trtype)))....  
-0000f720: 2020 2020 2020 2020 2020 6963 7331 203d            ics1 =
-0000f730: 2064 6174 615b 2269 6e63 6f6d 6531 225d   data["income1"]
-0000f740: 206f 7220 224e 6f6e 6522 0d0a 2020 2020   or "None"..    
-0000f750: 2020 2020 2020 2020 6963 7332 203d 2064          ics2 = d
-0000f760: 6174 615b 2269 6e63 6f6d 6532 225d 206f  ata["income2"] o
-0000f770: 7220 224e 6f6e 6522 0d0a 2020 2020 2020  r "None"..      
-0000f780: 2020 2020 2020 7365 6c66 2e63 6f6d 626f        self.combo
-0000f790: 496e 636f 6d65 4c65 6674 2e73 6574 4375  IncomeLeft.setCu
-0000f7a0: 7272 656e 7449 6e64 6578 2873 656c 662e  rrentIndex(self.
-0000f7b0: 636f 6d62 6f49 6e63 6f6d 654c 6566 742e  comboIncomeLeft.
-0000f7c0: 6669 6e64 5465 7874 2869 6373 3129 290d  findText(ics1)).
-0000f7d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f7e0: 662e 636f 6d62 6f49 6e63 6f6d 6552 6967  f.comboIncomeRig
-0000f7f0: 6874 2e73 6574 4375 7272 656e 7449 6e64  ht.setCurrentInd
-0000f800: 6578 2873 656c 662e 636f 6d62 6f49 6e63  ex(self.comboInc
-0000f810: 6f6d 6552 6967 6874 2e66 696e 6454 6578  omeRight.findTex
-0000f820: 7428 6963 7332 2929 0d0a 0d0a 2020 2020  t(ics2))....    
-0000f830: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000f840: 7451 7561 6e74 6974 792e 7365 7454 6578  tQuantity.setTex
-0000f850: 7428 6461 7461 5b22 7175 616e 7469 7479  t(data["quantity
-0000f860: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
-0000f870: 2073 656c 662e 6564 6974 5375 626a 6563   self.editSubjec
-0000f880: 742e 7365 7454 6578 7428 6461 7461 5b22  t.setText(data["
-0000f890: 7375 626a 6563 7422 5d29 0d0a 0d0a 2020  subject"])....  
-0000f8a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000f8b0: 7261 7763 616e 7661 732e 6869 6768 6c69  rawcanvas.highli
-0000f8c0: 6768 745f 636f 6e6e 6563 746f 7228 6461  ght_connector(da
-0000f8d0: 7461 5b22 7368 6f72 746e 616d 6522 5d29  ta["shortname"])
-0000f8e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f8f0: 6966 2022 6465 7363 7269 7074 696f 6e22  if "description"
-0000f900: 2069 6e20 6461 7461 3a0d 0a20 2020 2020   in data:..     
-0000f910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f920: 6564 6974 4465 7363 7269 7074 696f 6e2e  editDescription.
-0000f930: 7365 7454 6578 7428 6461 7461 5b22 6465  setText(data["de
-0000f940: 7363 7269 7074 696f 6e22 5d29 0d0a 2020  scription"])..  
-0000f950: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0000f960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f970: 2073 656c 662e 6564 6974 4465 7363 7269   self.editDescri
-0000f980: 7074 696f 6e2e 7365 7454 6578 7428 2222  ption.setText(""
-0000f990: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000f9a0: 656c 662e 6564 6974 5368 6f72 746e 616d  elf.editShortnam
-0000f9b0: 652e 7365 7454 6578 7428 6461 7461 5b22  e.setText(data["
-0000f9c0: 7368 6f72 746e 616d 6522 5d29 0d0a 0d0a  shortname"])....
-0000f9d0: 2020 2020 2020 2020 2020 2020 756e 6964              unid
-0000f9e0: 6972 203d 2073 7472 2864 6174 615b 2275  ir = str(data["u
-0000f9f0: 6e69 2d64 6972 6563 7469 6f6e 616c 225d  ni-directional"]
-0000fa00: 2920 6f72 2022 4e6f 6e65 220d 0a20 2020  ) or "None"..   
-0000fa10: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000fa20: 6d62 6f55 6e69 6469 722e 7365 7443 7572  mboUnidir.setCur
-0000fa30: 7265 6e74 496e 6465 7828 7365 6c66 2e63  rentIndex(self.c
-0000fa40: 6f6d 626f 556e 6964 6972 2e66 696e 6454  omboUnidir.findT
-0000fa50: 6578 7428 756e 6964 6972 2929 0d0a 0d0a  ext(unidir))....
-0000fa60: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-0000fa70: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-0000fa80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fa90: 2e6e 6f74 6966 7928 7374 7228 6529 2c74  .notify(str(e),t
-0000faa0: 6974 6c65 3d22 4572 726f 7222 290d 0a0d  itle="Error")...
-0000fab0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-0000fac0: 6465 5f63 6861 6e67 6573 203d 2046 616c  de_changes = Fal
-0000fad0: 7365 0d0a 0d0a 2020 2020 6465 6620 7570  se....    def up
-0000fae0: 6461 7465 5f64 6174 6128 7365 6c66 293a  date_data(self):
-0000faf0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-0000fb00: 662e 7365 6c65 6374 696f 6e5f 6964 7820  f.selection_idx 
-0000fb10: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-0000fb20: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-0000fb30: 2020 2020 2020 2020 7365 6c66 2e65 6e74          self.ent
-0000fb40: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
-0000fb50: 6563 7469 6f6e 5f69 6478 5d5b 2261 3122  ection_idx]["a1"
-0000fb60: 5d20 3d20 7365 6c66 2e41 7373 6574 4c69  ] = self.AssetLi
-0000fb70: 7374 4c65 6674 2e74 6f50 6c61 696e 5465  stLeft.toPlainTe
-0000fb80: 7874 2829 0d0a 2020 2020 2020 2020 7365  xt()..        se
-0000fb90: 6c66 2e65 6e74 7279 5f64 6174 615b 7365  lf.entry_data[se
-0000fba0: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
-0000fbb0: 5d5b 2261 3222 5d20 3d20 7365 6c66 2e41  ]["a2"] = self.A
-0000fbc0: 7373 6574 4c69 7374 5269 6768 742e 746f  ssetListRight.to
-0000fbd0: 506c 6169 6e54 6578 7428 290d 0a20 2020  PlainText()..   
-0000fbe0: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
-0000fbf0: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
-0000fc00: 696f 6e5f 6964 785d 5b22 6c31 225d 203d  ion_idx]["l1"] =
-0000fc10: 2073 656c 662e 4c69 6162 696c 6974 794c   self.LiabilityL
-0000fc20: 6973 744c 6566 742e 746f 506c 6169 6e54  istLeft.toPlainT
-0000fc30: 6578 7428 290d 0a20 2020 2020 2020 2073  ext()..        s
-0000fc40: 656c 662e 656e 7472 795f 6461 7461 5b73  elf.entry_data[s
-0000fc50: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
-0000fc60: 785d 5b22 6c32 225d 203d 2073 656c 662e  x]["l2"] = self.
-0000fc70: 4c69 6162 696c 6974 794c 6973 7452 6967  LiabilityListRig
-0000fc80: 6874 2e74 6f50 6c61 696e 5465 7874 2829  ht.toPlainText()
-0000fc90: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-0000fca0: 6e74 7279 5f64 6174 615b 7365 6c66 2e73  ntry_data[self.s
-0000fcb0: 656c 6563 7469 6f6e 5f69 6478 5d5b 2265  election_idx]["e
-0000fcc0: 3122 5d20 3d20 7365 6c66 2e45 7175 6974  1"] = self.Equit
-0000fcd0: 794c 6973 744c 6566 742e 746f 506c 6169  yListLeft.toPlai
-0000fce0: 6e54 6578 7428 290d 0a20 2020 2020 2020  nText()..       
-0000fcf0: 2073 656c 662e 656e 7472 795f 6461 7461   self.entry_data
-0000fd00: 5b73 656c 662e 7365 6c65 6374 696f 6e5f  [self.selection_
-0000fd10: 6964 785d 5b22 6532 225d 203d 2073 656c  idx]["e2"] = sel
-0000fd20: 662e 4571 7569 7479 4c69 7374 5269 6768  f.EquityListRigh
-0000fd30: 742e 746f 506c 6169 6e54 6578 7428 290d  t.toPlainText().
-0000fd40: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-0000fd50: 656e 7472 795f 6461 7461 5b73 656c 662e  entry_data[self.
-0000fd60: 7365 6c65 6374 696f 6e5f 6964 785d 5b22  selection_idx]["
-0000fd70: 6131 225d 2020 3d20 7365 6c66 2e41 7373  a1"]  = self.Ass
-0000fd80: 6574 4c69 7374 4c65 6674 2e74 6f50 6c61  etListLeft.toPla
-0000fd90: 696e 5465 7874 2829 0d0a 2020 2020 2020  inText()..      
-0000fda0: 2020 7365 6c66 2e65 6e74 7279 5f64 6174    self.entry_dat
-0000fdb0: 615b 7365 6c66 2e73 656c 6563 7469 6f6e  a[self.selection
-0000fdc0: 5f69 6478 5d5b 2261 3222 5d20 3d20 7365  _idx]["a2"] = se
-0000fdd0: 6c66 2e41 7373 6574 4c69 7374 5269 6768  lf.AssetListRigh
-0000fde0: 742e 746f 506c 6169 6e54 6578 7428 290d  t.toPlainText().
-0000fdf0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-0000fe00: 7472 795f 6461 7461 5b73 656c 662e 7365  try_data[self.se
-0000fe10: 6c65 6374 696f 6e5f 6964 785d 5b22 6c31  lection_idx]["l1
-0000fe20: 225d 2020 3d20 7365 6c66 2e4c 6961 6269  "]  = self.Liabi
-0000fe30: 6c69 7479 4c69 7374 4c65 6674 2e74 6f50  lityListLeft.toP
-0000fe40: 6c61 696e 5465 7874 2829 0d0a 2020 2020  lainText()..    
-0000fe50: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
-0000fe60: 6174 615b 7365 6c66 2e73 656c 6563 7469  ata[self.selecti
-0000fe70: 6f6e 5f69 6478 5d5b 226c 3222 5d20 203d  on_idx]["l2"]  =
-0000fe80: 2073 656c 662e 4c69 6162 696c 6974 794c   self.LiabilityL
-0000fe90: 6973 7452 6967 6874 2e74 6f50 6c61 696e  istRight.toPlain
-0000fea0: 5465 7874 2829 0d0a 2020 2020 2020 2020  Text()..        
-0000feb0: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
-0000fec0: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
-0000fed0: 6478 5d5b 2265 3122 5d20 203d 2073 656c  dx]["e1"]  = sel
-0000fee0: 662e 4571 7569 7479 4c69 7374 4c65 6674  f.EquityListLeft
-0000fef0: 2e74 6f50 6c61 696e 5465 7874 2829 0d0a  .toPlainText()..
-0000ff00: 2020 2020 2020 2020 7365 6c66 2e65 6e74          self.ent
-0000ff10: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
-0000ff20: 6563 7469 6f6e 5f69 6478 5d5b 2265 3222  ection_idx]["e2"
-0000ff30: 5d20 203d 2073 656c 662e 4571 7569 7479  ]  = self.Equity
-0000ff40: 4c69 7374 5269 6768 742e 746f 506c 6169  ListRight.toPlai
-0000ff50: 6e54 6578 7428 290d 0a0d 0a20 2020 2020  nText()....     
-0000ff60: 2020 206f 6e6c 795f 7265 6e61 6d65 203d     only_rename =
-0000ff70: 2054 7275 650d 0a20 2020 2020 2020 2069   True..        i
-0000ff80: 6620 7365 6c66 2e65 6e74 7279 5f64 6174  f self.entry_dat
-0000ff90: 615b 7365 6c66 2e73 656c 6563 7469 6f6e  a[self.selection
-0000ffa0: 5f69 6478 5d5b 2261 6765 6e74 3122 5d20  _idx]["agent1"] 
-0000ffb0: 2021 3d20 7365 6c66 2e61 6765 6e74 3145   != self.agent1E
-0000ffc0: 6469 742e 7465 7874 2829 3a0d 0a20 2020  dit.text():..   
-0000ffd0: 2020 2020 2020 2020 206f 6e6c 795f 7265           only_re
-0000ffe0: 6e61 6d65 203d 2046 616c 7365 0d0a 2020  name = False..  
-0000fff0: 2020 2020 2020 6966 2073 656c 662e 656e        if self.en
-00010000: 7472 795f 6461 7461 5b73 656c 662e 7365  try_data[self.se
-00010010: 6c65 6374 696f 6e5f 6964 785d 5b22 6167  lection_idx]["ag
-00010020: 656e 7432 225d 2020 213d 7365 6c66 2e61  ent2"]  !=self.a
-00010030: 6765 6e74 3245 6469 742e 7465 7874 2829  gent2Edit.text()
-00010040: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
-00010050: 6e6c 795f 7265 6e61 6d65 203d 2046 616c  nly_rename = Fal
-00010060: 7365 0d0a 0d0a 0d0a 2020 2020 2020 2020  se......        
-00010070: 6966 206e 6f74 2073 656c 662e 6472 6177  if not self.draw
-00010080: 6361 6e76 6173 2e63 6865 636b 5f65 7869  canvas.check_exi
-00010090: 7374 2873 656c 662e 6167 656e 7431 4564  st(self.agent1Ed
-000100a0: 6974 2e74 6578 7428 2929 3a0d 0a20 2020  it.text()):..   
-000100b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000100c0: 2e61 6765 6e74 3145 6469 742e 7465 7874  .agent1Edit.text
-000100d0: 2829 2e73 7472 6970 2829 2021 3d20 2222  ().strip() != ""
-000100e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000100f0: 2020 2079 6573 203d 2073 656c 662e 6173     yes = self.as
-00010100: 6b5f 7175 6573 7469 6f6e 2827 272c 2254  k_question('',"T
-00010110: 6865 2061 6765 6e74 2025 7320 646f 6573  he agent %s does
-00010120: 206e 6f74 2065 7869 7374 2e5c 6e44 6f20   not exist.\nDo 
-00010130: 796f 7520 7769 7368 2074 6f20 636f 6e74  you wish to cont
-00010140: 696e 7565 2061 6e64 2061 7574 6f6d 6174  inue and automat
-00010150: 6963 616c 6c79 2063 7265 6174 6520 6120  ically create a 
-00010160: 6e65 7720 6167 656e 743f 2225 7365 6c66  new agent?"%self
-00010170: 2e61 6765 6e74 3145 6469 742e 7465 7874  .agent1Edit.text
-00010180: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
-00010190: 2020 2020 2069 6620 6e6f 7420 7965 733a       if not yes:
-000101a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000101b0: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-000101c0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000101d0: 656c 662e 6472 6177 6361 6e76 6173 2e63  elf.drawcanvas.c
-000101e0: 6865 636b 5f65 7869 7374 2873 656c 662e  heck_exist(self.
-000101f0: 6167 656e 7432 4564 6974 2e74 6578 7428  agent2Edit.text(
-00010200: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00010210: 2069 6620 7365 6c66 2e61 6765 6e74 3245   if self.agent2E
-00010220: 6469 742e 7465 7874 2829 2e73 7472 6970  dit.text().strip
-00010230: 2829 2021 3d20 2222 3a0d 0a20 2020 2020  () != "":..     
-00010240: 2020 2020 2020 2020 2020 2079 6573 203d             yes =
-00010250: 2073 656c 662e 6173 6b5f 7175 6573 7469   self.ask_questi
-00010260: 6f6e 2827 272c 2254 6865 2061 6765 6e74  on('',"The agent
-00010270: 2025 7320 646f 6573 206e 6f74 2065 7869   %s does not exi
-00010280: 7374 2e5c 6e44 6f20 796f 7520 7769 7368  st.\nDo you wish
-00010290: 2074 6f20 636f 6e74 696e 7565 2061 6e64   to continue and
-000102a0: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
-000102b0: 7265 6174 6520 6120 6e65 7720 6167 656e  reate a new agen
-000102c0: 743f 2225 7365 6c66 2e61 6765 6e74 3245  t?"%self.agent2E
-000102d0: 6469 742e 7465 7874 2829 290d 0a20 2020  dit.text())..   
-000102e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000102f0: 6e6f 7420 7965 733a 0d0a 2020 2020 2020  not yes:..      
-00010300: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00010310: 7475 726e 0d0a 0d0a 2020 2020 2020 2020  turn....        
-00010320: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
-00010330: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
-00010340: 6478 5d5b 2261 6765 6e74 3122 5d20 203d  dx]["agent1"]  =
-00010350: 2063 616d 656c 2873 656c 662e 6167 656e   camel(self.agen
-00010360: 7431 4564 6974 2e74 6578 7428 2929 2023  t1Edit.text()) #
-00010370: 2e63 6170 6974 616c 697a 6528 2920 2320  .capitalize() # 
-00010380: 7570 7065 7220 6265 6361 7573 6520 6167  upper because ag
-00010390: 656e 7473 2061 7265 2061 6c77 6179 7320  ents are always 
-000103a0: 7570 7065 7263 6173 650d 0a20 2020 2020  uppercase..     
-000103b0: 2020 2073 656c 662e 656e 7472 795f 6461     self.entry_da
-000103c0: 7461 5b73 656c 662e 7365 6c65 6374 696f  ta[self.selectio
-000103d0: 6e5f 6964 785d 5b22 6167 656e 7432 225d  n_idx]["agent2"]
-000103e0: 2020 3d20 6361 6d65 6c28 7365 6c66 2e61    = camel(self.a
-000103f0: 6765 6e74 3245 6469 742e 7465 7874 2829  gent2Edit.text()
-00010400: 2920 232e 6361 7069 7461 6c69 7a65 2829  ) #.capitalize()
-00010410: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00010420: 2e61 6765 6e74 3145 6469 742e 7365 7454  .agent1Edit.setT
-00010430: 6578 7428 6361 6d65 6c28 7365 6c66 2e61  ext(camel(self.a
-00010440: 6765 6e74 3145 6469 742e 7465 7874 2829  gent1Edit.text()
-00010450: 2929 2023 2e63 6170 6974 616c 697a 6528  )) #.capitalize(
-00010460: 2929 0d0a 2020 2020 2020 2020 7365 6c66  ))..        self
-00010470: 2e61 6765 6e74 3245 6469 742e 7365 7454  .agent2Edit.setT
-00010480: 6578 7428 6361 6d65 6c28 7365 6c66 2e61  ext(camel(self.a
-00010490: 6765 6e74 3245 6469 742e 7465 7874 2829  gent2Edit.text()
-000104a0: 2929 2023 2e63 6170 6974 616c 697a 6528  )) #.capitalize(
-000104b0: 2929 0d0a 0d0a 2020 2020 2020 2020 7365  ))....        se
-000104c0: 6c66 2e65 6e74 7279 5f64 6174 615b 7365  lf.entry_data[se
-000104d0: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
-000104e0: 5d5b 2275 6e69 2d64 6972 6563 7469 6f6e  ]["uni-direction
-000104f0: 616c 225d 203d 205c 0d0a 2020 2020 2020  al"] = \..      
-00010500: 2020 2020 2020 7374 7228 7365 6c66 2e63        str(self.c
-00010510: 6f6d 626f 556e 6964 6972 2e63 7572 7265  omboUnidir.curre
-00010520: 6e74 5465 7874 2829 290d 0a0d 0a20 2020  ntText())....   
-00010530: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
-00010540: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
-00010550: 696f 6e5f 6964 785d 5b22 6c6f 6720 7472  ion_idx]["log tr
-00010560: 616e 7361 6374 696f 6e22 5d20 3d5c 0d0a  ansaction"] =\..
-00010570: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00010580: 7365 6c66 2e72 6567 6973 7465 7246 6c6f  self.registerFlo
-00010590: 7742 6f78 2e63 7572 7265 6e74 5465 7874  wBox.currentText
-000105a0: 2829 290d 0a0d 0a20 2020 2020 2020 2073  ())....        s
-000105b0: 656c 662e 656e 7472 795f 6461 7461 5b73  elf.entry_data[s
-000105c0: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
-000105d0: 785d 5b22 6361 7368 666c 6f77 3122 5d20  x]["cashflow1"] 
-000105e0: 3d20 5c0d 0a20 2020 2020 2020 2020 2020  = \..           
-000105f0: 2073 7472 2873 656c 662e 636f 6d62 6f43   str(self.comboC
-00010600: 6173 684c 6566 742e 6375 7272 656e 7454  ashLeft.currentT
-00010610: 6578 7428 2929 0d0a 2020 2020 2020 2020  ext())..        
-00010620: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
-00010630: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
-00010640: 6478 5d5b 2263 6173 6866 6c6f 7732 225d  dx]["cashflow2"]
-00010650: 203d 205c 0d0a 2020 2020 2020 2020 2020   = \..          
-00010660: 2020 7374 7228 7365 6c66 2e63 6f6d 626f    str(self.combo
-00010670: 4361 7368 5269 6768 742e 6375 7272 656e  CashRight.curren
-00010680: 7454 6578 7428 2929 0d0a 0d0a 2020 2020  tText())....    
-00010690: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
-000106a0: 6174 615b 7365 6c66 2e73 656c 6563 7469  ata[self.selecti
-000106b0: 6f6e 5f69 6478 5d5b 226b 696e 6422 5d20  on_idx]["kind"] 
-000106c0: 3d20 5c0d 0a20 2020 2020 2020 2020 2020  = \..           
-000106d0: 2073 7472 2873 656c 662e 6564 6974 5479   str(self.editTy
-000106e0: 7065 2e63 7572 7265 6e74 5465 7874 2829  pe.currentText()
-000106f0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-00010700: 662e 656e 7472 795f 6461 7461 5b73 656c  f.entry_data[sel
-00010710: 662e 7365 6c65 6374 696f 6e5f 6964 785d  f.selection_idx]
-00010720: 5b22 696e 636f 6d65 3122 5d20 3d20 5c0d  ["income1"] = \.
-00010730: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00010740: 2873 656c 662e 636f 6d62 6f49 6e63 6f6d  (self.comboIncom
-00010750: 654c 6566 742e 6375 7272 656e 7454 6578  eLeft.currentTex
-00010760: 7428 2929 0d0a 2020 2020 2020 2020 7365  t())..        se
-00010770: 6c66 2e65 6e74 7279 5f64 6174 615b 7365  lf.entry_data[se
-00010780: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
-00010790: 5d5b 2269 6e63 6f6d 6532 225d 203d 205c  ]["income2"] = \
-000107a0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000107b0: 7228 7365 6c66 2e63 6f6d 626f 496e 636f  r(self.comboInco
-000107c0: 6d65 5269 6768 742e 6375 7272 656e 7454  meRight.currentT
-000107d0: 6578 7428 2929 0d0a 0d0a 0d0a 2020 2020  ext())......    
-000107e0: 2020 2020 6966 206f 6e6c 795f 7265 6e61      if only_rena
-000107f0: 6d65 3a0d 0a0d 0a20 2020 2020 2020 2020  me:....         
-00010800: 2020 2073 656c 662e 6472 6177 6361 6e76     self.drawcanv
-00010810: 6173 2e72 656e 616d 655f 636f 6e6e 6563  as.rename_connec
-00010820: 7469 6f6e 2873 656c 662e 656e 7472 795f  tion(self.entry_
-00010830: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
-00010840: 696f 6e5f 6964 785d 5b22 7368 6f72 746e  ion_idx]["shortn
-00010850: 616d 6522 5d20 2c20 7374 7228 7365 6c66  ame"] , str(self
-00010860: 2e65 6469 7453 686f 7274 6e61 6d65 2e74  .editShortname.t
-00010870: 6578 7428 2929 290d 0a0d 0a20 2020 2020  ext()))....     
-00010880: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00010890: 2020 2020 2020 7365 6c66 2e64 7261 7763        self.drawc
-000108a0: 616e 7661 732e 7265 6d6f 7665 5f63 6f6e  anvas.remove_con
-000108b0: 6e65 6374 696f 6e28 7365 6c66 2e65 6e74  nection(self.ent
-000108c0: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
-000108d0: 6563 7469 6f6e 5f69 6478 5d5b 2273 686f  ection_idx]["sho
-000108e0: 7274 6e61 6d65 225d 2920 232c 2073 7472  rtname"]) #, str
-000108f0: 2873 656c 662e 6564 6974 5375 626a 6563  (self.editSubjec
-00010900: 742e 7465 7874 2829 2929 0d0a 0d0a 2020  t.text()))....  
-00010910: 2020 2020 2020 2020 2020 626f 7831 203d            box1 =
-00010920: 2073 656c 662e 6472 6177 6361 6e76 6173   self.drawcanvas
-00010930: 2e61 6464 5f61 6765 6e74 2873 656c 662e  .add_agent(self.
-00010940: 656e 7472 795f 6461 7461 5b73 656c 662e  entry_data[self.
-00010950: 7365 6c65 6374 696f 6e5f 6964 785d 5b22  selection_idx]["
-00010960: 6167 656e 7431 225d 290d 0a20 2020 2020  agent1"])..     
-00010970: 2020 2020 2020 2062 6f78 3220 3d20 7365         box2 = se
-00010980: 6c66 2e64 7261 7763 616e 7661 732e 6164  lf.drawcanvas.ad
-00010990: 645f 6167 656e 7428 7365 6c66 2e65 6e74  d_agent(self.ent
-000109a0: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
-000109b0: 6563 7469 6f6e 5f69 6478 5d5b 2261 6765  ection_idx]["age
-000109c0: 6e74 3222 5d29 0d0a 0d0a 0d0a 2020 2020  nt2"])......    
-000109d0: 2020 2020 2020 2020 6d79 5f69 7465 6d73          my_items
-000109e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000109f0: 2020 2064 6174 6120 3d20 7365 6c66 2e65     data = self.e
-00010a00: 6e74 7279 5f64 6174 615b 7365 6c66 2e73  ntry_data[self.s
-00010a10: 656c 6563 7469 6f6e 5f69 6478 5d0d 0a0d  election_idx]...
-00010a20: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-00010a30: 656e 7472 6965 7320 3d20 225c 6e22 2e6a  entries = "\n".j
-00010a40: 6f69 6e28 5b64 6174 615b 226c 3122 5d2c  oin([data["l1"],
-00010a50: 2064 6174 615b 2261 3122 5d2c 2064 6174   data["a1"], dat
-00010a60: 615b 2265 3122 5d2c 2064 6174 615b 226c  a["e1"], data["l
-00010a70: 3222 5d2c 2064 6174 615b 2261 3222 5d2c  2"], data["a2"],
-00010a80: 2064 6174 615b 2265 3222 5d5d 290d 0a20   data["e2"]]).. 
-00010a90: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00010aa0: 7562 5f69 7465 6d20 696e 2061 6c6c 656e  ub_item in allen
-00010ab0: 7472 6965 732e 7370 6c69 7428 225c 6e22  tries.split("\n"
-00010ac0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00010ad0: 2020 2020 666f 7220 7375 625f 656e 7472      for sub_entr
-00010ae0: 7920 696e 2073 7562 5f69 7465 6d2e 7370  y in sub_item.sp
-00010af0: 6c69 7428 225c 6e22 293a 0d0a 2020 2020  lit("\n"):..    
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 656e 7472 7920 3d20 7375 625f 656e 7472  entry = sub_entr
-00010b20: 792e 7265 706c 6163 6528 222d 222c 2222  y.replace("-",""
-00010b30: 292e 7265 706c 6163 6528 222b 222c 2222  ).replace("+",""
-00010b40: 292e 7374 7269 7028 290d 0a20 2020 2020  ).strip()..     
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010b60: 6620 656e 7472 7920 213d 2020 2222 3a0d  f entry !=  "":.
-00010b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b80: 2020 2020 2020 2020 206d 795f 6974 656d           my_item
-00010b90: 732e 6170 7065 6e64 2865 6e74 7279 290d  s.append(entry).
-00010ba0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00010bb0: 2073 656c 662e 6472 6177 6361 6e76 6173   self.drawcanvas
-00010bc0: 2e61 6464 5f63 6f6e 6e65 6374 696f 6e28  .add_connection(
-00010bd0: 626f 7831 2c62 6f78 322c 2073 7472 2873  box1,box2, str(s
-00010be0: 656c 662e 6564 6974 5368 6f72 746e 616d  elf.editShortnam
-00010bf0: 652e 7465 7874 2829 292c 7375 626a 6563  e.text()),subjec
-00010c00: 743d 7365 6c66 2e65 6469 7453 7562 6a65  t=self.editSubje
-00010c10: 6374 2e74 6578 7428 292c 6974 656d 733d  ct.text(),items=
-00010c20: 6d79 5f69 7465 6d73 290d 0a0d 0a0d 0a20  my_items)...... 
-00010c30: 2020 2020 2020 2073 656c 662e 656e 7472         self.entr
-00010c40: 795f 6461 7461 5b73 656c 662e 7365 6c65  y_data[self.sele
-00010c50: 6374 696f 6e5f 6964 785d 5b22 7175 616e  ction_idx]["quan
-00010c60: 7469 7479 225d 203d 205c 0d0a 2020 2020  tity"] = \..    
-00010c70: 2020 2020 2020 2020 7374 7228 7365 6c66          str(self
-00010c80: 2e65 6469 7451 7561 6e74 6974 792e 7465  .editQuantity.te
-00010c90: 7874 2829 290d 0a0d 0a0d 0a20 2020 2020  xt())......     
-00010ca0: 2020 2073 656c 662e 656e 7472 795f 6461     self.entry_da
-00010cb0: 7461 5b73 656c 662e 7365 6c65 6374 696f  ta[self.selectio
-00010cc0: 6e5f 6964 785d 5b22 7375 626a 6563 7422  n_idx]["subject"
-00010cd0: 5d20 3d20 5c0d 0a20 2020 2020 2020 2020  ] = \..         
-00010ce0: 2020 2073 7472 2873 656c 662e 6564 6974     str(self.edit
-00010cf0: 5375 626a 6563 742e 7465 7874 2829 290d  Subject.text()).
-00010d00: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00010d10: 656e 7472 795f 6461 7461 5b73 656c 662e  entry_data[self.
-00010d20: 7365 6c65 6374 696f 6e5f 6964 785d 5b22  selection_idx]["
-00010d30: 7368 6f72 746e 616d 6522 5d20 3d20 5c0d  shortname"] = \.
-00010d40: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00010d50: 2873 656c 662e 6564 6974 5368 6f72 746e  (self.editShortn
-00010d60: 616d 652e 7465 7874 2829 290d 0a0d 0a20  ame.text()).... 
-00010d70: 2020 2020 2020 2073 656c 662e 656e 7472         self.entr
-00010d80: 795f 6461 7461 5b73 656c 662e 7365 6c65  y_data[self.sele
-00010d90: 6374 696f 6e5f 6964 785d 5b22 6465 7363  ction_idx]["desc
-00010da0: 7269 7074 696f 6e22 5d20 3d20 5c0d 0a20  ription"] = \.. 
-00010db0: 2020 2020 2020 2020 2020 2073 7472 2873             str(s
-00010dc0: 656c 662e 6564 6974 4465 7363 7269 7074  elf.editDescript
-00010dd0: 696f 6e2e 7465 7874 2829 290d 0a0d 0a20  ion.text()).... 
-00010de0: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00010df0: 7465 5f74 6162 6c65 2829 0d0a 0d0a 2020  te_table()....  
-00010e00: 2020 2020 2020 7072 696e 7428 2264 6174        print("dat
-00010e10: 6120 6368 616e 6765 642e 2229 0d0a 0d0a  a changed.")....
-00010e20: 2020 2020 2020 2020 7365 6c66 2e6d 6164          self.mad
-00010e30: 655f 6368 616e 6765 7320 3d20 4661 6c73  e_changes = Fals
-00010e40: 650d 0a0d 0a20 2020 2020 2020 2073 656c  e....        sel
-00010e50: 662e 726f 775f 7365 6c65 6374 2873 656c  f.row_select(sel
-00010e60: 662e 7365 6c65 6374 696f 6e5f 6964 7829  f.selection_idx)
-00010e70: 0d0a 0d0a 2020 2020 2020 2020 2320 7365  ....        # se
-00010e80: 6c66 2e75 6470 6174 6542 7574 746f 6e2e  lf.udpateButton.
-00010e90: 7365 7454 6578 7428 2255 7064 6174 6520  setText("Update 
-00010ea0: 5661 6c75 6573 2229 0d0a 0d0a 2020 2020  Values")....    
-00010eb0: 6465 6620 7361 7665 2873 656c 6629 3a0d  def save(self):.
-00010ec0: 0a0d 0a20 2020 2020 2020 2074 7279 3a0d  ...        try:.
-00010ed0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00010ee0: 2066 696c 656e 616d 6520 3d20 7365 6c66   filename = self
-00010ef0: 2e63 7572 7265 6e74 5f66 696c 6520 2320  .current_file # 
-00010f00: 7374 6174 7573 4261 7228 292e 6375 7272  statusBar().curr
-00010f10: 656e 744d 6573 7361 6765 2829 0d0a 2020  entMessage()..  
-00010f20: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00010f30: 6162 656c 5f66 6e61 6d65 2e73 6574 5465  abel_fname.setTe
-00010f40: 7874 2866 696c 656e 616d 6529 0d0a 0d0a  xt(filename)....
-00010f50: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00010f60: 696c 656e 616d 6520 6973 206e 6f74 204e  ilename is not N
-00010f70: 6f6e 653a 0d0a 0d0a 2020 2020 2020 2020  one:....        
-00010f80: 2020 2020 2020 2020 7365 6c66 2e73 6176          self.sav
-00010f90: 6561 7328 6669 6c65 6e61 6d65 290d 0a0d  eas(filename)...
-00010fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010fb0: 2023 2054 4f44 4f20 6d61 7962 6520 6261   # TODO maybe ba
-00010fc0: 636b 7570 283f 290d 0a20 2020 2020 2020  ckup(?)..       
-00010fd0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00010fe0: 6e6f 7469 6679 2822 4669 6c65 2073 6176  notify("File sav
-00010ff0: 6564 2075 6e64 6572 2025 7322 2025 2066  ed under %s" % f
-00011000: 696c 656e 616d 652c 7469 746c 653d 224f  ilename,title="O
-00011010: 6b22 290d 0a20 2020 2020 2020 2020 2020  k")..           
-00011020: 2020 2020 2070 7269 6e74 2822 4649 4c45       print("FILE
-00011030: 2053 4156 4544 2122 290d 0a20 2020 2020   SAVED!")..     
-00011040: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00011050: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011060: 6c66 2e73 6176 655f 646c 6728 290d 0a0d  lf.save_dlg()...
-00011070: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00011080: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00011090: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000110a0: 6669 6c65 6e61 6d65 2021 3d20 2222 3a0d  filename != "":.
-000110b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110c0: 2073 656c 662e 6e6f 7469 6679 2873 7472   self.notify(str
-000110d0: 2865 292c 7469 746c 653d 2245 7272 6f72  (e),title="Error
-000110e0: 2229 0d0a 0d0a 0d0a 0d0a 2020 2020 6465  ")........    de
-000110f0: 6620 7361 7665 5f64 6c67 2873 656c 6629  f save_dlg(self)
-00011100: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
-00011110: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-00011120: 696c 656e 616d 6520 3d20 5146 696c 6544  ilename = QFileD
-00011130: 6961 6c6f 672e 6765 7453 6176 6546 696c  ialog.getSaveFil
-00011140: 654e 616d 6528 7365 6c66 2c20 2753 6176  eName(self, 'Sav
-00011150: 6520 6669 6c65 272c 0d0a 2020 2020 2020  e file',..      
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 206f 732e 6765 7463           os.getc
-00011190: 7764 2829 2c20 2261 7474 756e 6520 4669  wd(), "attune Fi
-000111a0: 6c65 7320 282a 2e73 6663 746c 2922 295b  les (*.sfctl)")[
-000111b0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-000111c0: 7365 6c66 2e73 7461 7475 7342 6172 2829  self.statusBar()
-000111d0: 2e73 686f 774d 6573 7361 6765 2822 5361  .showMessage("Sa
-000111e0: 7665 6420 6669 6c65 2022 202b 2066 696c  ved file " + fil
-000111f0: 656e 616d 6529 0d0a 0d0a 2020 2020 2020  ename)....      
-00011200: 2020 2020 2020 6375 7272 656e 745f 6669        current_fi
-00011210: 6c65 5f62 6163 6b75 7020 3d20 7365 6c66  le_backup = self
-00011220: 2e63 7572 7265 6e74 5f66 696c 650d 0a0d  .current_file...
-00011230: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011240: 6669 6c65 6e61 6d65 2069 7320 6e6f 7420  filename is not 
-00011250: 4e6f 6e65 2061 6e64 2066 696c 656e 616d  None and filenam
-00011260: 6520 213d 2022 223a 0d0a 2020 2020 2020  e != "":..      
-00011270: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00011280: 6162 656c 5f66 6e61 6d65 2e73 6574 5465  abel_fname.setTe
-00011290: 7874 2866 696c 656e 616d 6529 0d0a 0d0a  xt(filename)....
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 7365 6c66 2e63 7572 7265 6e74 5f66 696c  self.current_fil
-000112c0: 6520 3d20 6669 6c65 6e61 6d65 0d0a 2020  e = filename..  
-000112d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000112e0: 6c66 2e73 6176 6561 7328 6669 6c65 6e61  lf.saveas(filena
-000112f0: 6d65 290d 0a0d 0a20 2020 2020 2020 2020  me)....         
-00011300: 2020 2023 2054 4f44 4f20 6d61 7962 6520     # TODO maybe 
-00011310: 6261 636b 7570 283f 290d 0a0d 0a20 2020  backup(?)....   
-00011320: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00011330: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00011340: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00011350: 7469 6679 2822 436f 756c 6420 6e6f 7420  tify("Could not 
-00011360: 7361 7665 2070 726f 6a65 6374 2e22 2c74  save project.",t
-00011370: 6974 6c65 3d22 4572 726f 7222 290d 0a20  itle="Error").. 
-00011380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011390: 6375 7272 656e 745f 6669 6c65 203d 2063  current_file = c
-000113a0: 7572 7265 6e74 5f66 696c 655f 6261 636b  urrent_file_back
-000113b0: 7570 0d0a 0d0a 0d0a 2020 2020 6465 6620  up......    def 
-000113c0: 6765 745f 6f70 7469 6f6e 7328 7365 6c66  get_options(self
-000113d0: 293a 0d0a 2020 2020 2020 2020 6f31 203d  ):..        o1 =
-000113e0: 2073 7472 2873 656c 662e 6368 6563 6b42   str(self.checkB
-000113f0: 6f78 5f32 2e69 7343 6865 636b 6564 2829  ox_2.isChecked()
-00011400: 290d 0a20 2020 2020 2020 206f 3220 3d20  )..        o2 = 
-00011410: 7374 7228 7365 6c66 2e63 6865 636b 426f  str(self.checkBo
-00011420: 782e 6973 4368 6563 6b65 6428 2929 0d0a  x.isChecked())..
-00011430: 2020 2020 2020 2020 6f33 203d 2073 7472          o3 = str
-00011440: 2873 656c 662e 6368 6563 6b42 6f78 5f34  (self.checkBox_4
-00011450: 2e69 7343 6865 636b 6564 2829 290d 0a20  .isChecked()).. 
-00011460: 2020 2020 2020 206f 3420 3d20 7374 7228         o4 = str(
-00011470: 7365 6c66 2e63 6865 636b 426f 785f 352e  self.checkBox_5.
-00011480: 6973 4368 6563 6b65 6428 2929 0d0a 2020  isChecked())..  
-00011490: 2020 2020 2020 6f35 203d 2073 7472 2873        o5 = str(s
-000114a0: 656c 662e 6368 6563 6b42 6f78 5f33 2e69  elf.checkBox_3.i
-000114b0: 7343 6865 636b 6564 2829 290d 0a20 2020  sChecked())..   
-000114c0: 2020 2020 206f 3620 3d20 7374 7228 7365       o6 = str(se
-000114d0: 6c66 2e63 6865 636b 426f 785f 362e 6973  lf.checkBox_6.is
-000114e0: 4368 6563 6b65 6428 2929 0d0a 2020 2020  Checked())..    
-000114f0: 2020 2020 6f37 203d 2073 7472 2873 656c      o7 = str(sel
-00011500: 662e 6368 6563 6b42 6f78 5f38 2e69 7343  f.checkBox_8.isC
-00011510: 6865 636b 6564 2829 290d 0a20 2020 2020  hecked())..     
-00011520: 2020 206f 3820 3d20 7374 7228 7365 6c66     o8 = str(self
-00011530: 2e63 6865 636b 426f 785f 392e 6973 4368  .checkBox_9.isCh
-00011540: 6563 6b65 6428 2929 0d0a 2020 2020 2020  ecked())..      
-00011550: 2020 6f39 203d 2073 7472 2873 656c 662e    o9 = str(self.
-00011560: 6368 6563 6b42 6f78 5f72 6173 7465 722e  checkBox_raster.
-00011570: 6973 4368 6563 6b65 6428 2929 0d0a 0d0a  isChecked())....
-00011580: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00011590: 6f31 2c6f 322c 6f33 2c6f 342c 6f35 2c6f  o1,o2,o3,o4,o5,o
-000115a0: 362c 6f37 2c6f 382c 6f39 5d0d 0a0d 0a20  6,o7,o8,o9].... 
-000115b0: 2020 2064 6566 2073 6574 5f6f 7074 696f     def set_optio
-000115c0: 6e73 2873 656c 662c 6e65 775f 6f70 7469  ns(self,new_opti
-000115d0: 6f6e 7329 3a0d 0a20 2020 2020 2020 2023  ons):..        #
-000115e0: 2073 6574 2064 6973 706c 6179 206f 7074   set display opt
-000115f0: 696f 6e73 0d0a 2020 2020 2020 2020 6966  ions..        if
-00011600: 206e 6577 5f6f 7074 696f 6e73 2069 7320   new_options is 
-00011610: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00011620: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-00011630: 2020 2020 206f 312c 6f32 2c6f 332c 6f34       o1,o2,o3,o4
-00011640: 2c6f 352c 6f36 2c6f 372c 6f38 2c6f 3920  ,o5,o6,o7,o8,o9 
-00011650: 3d20 6e65 775f 6f70 7469 6f6e 730d 0a0d  = new_options...
-00011660: 0a20 2020 2020 2020 2064 6566 2073 7472  .        def str
-00011670: 5f74 6f5f 626f 6f6c 2878 293a 0d0a 2020  _to_bool(x):..  
-00011680: 2020 2020 2020 2020 2020 6966 2078 203d            if x =
-00011690: 3d20 2254 7275 6522 3a0d 0a20 2020 2020  = "True":..     
-000116a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000116b0: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-000116c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000116d0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000116e0: 2e63 6865 636b 426f 785f 322e 7365 7443  .checkBox_2.setC
-000116f0: 6865 636b 6564 2873 7472 5f74 6f5f 626f  hecked(str_to_bo
-00011700: 6f6c 286f 3129 290d 0a20 2020 2020 2020  ol(o1))..       
-00011710: 2073 656c 662e 6368 6563 6b42 6f78 2e73   self.checkBox.s
-00011720: 6574 4368 6563 6b65 6428 7374 725f 746f  etChecked(str_to
-00011730: 5f62 6f6f 6c28 6f32 2929 0d0a 2020 2020  _bool(o2))..    
-00011740: 2020 2020 7365 6c66 2e63 6865 636b 426f      self.checkBo
-00011750: 785f 342e 7365 7443 6865 636b 6564 2873  x_4.setChecked(s
-00011760: 7472 5f74 6f5f 626f 6f6c 286f 3329 290d  tr_to_bool(o3)).
-00011770: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
-00011780: 6563 6b42 6f78 5f35 2e73 6574 4368 6563  eckBox_5.setChec
-00011790: 6b65 6428 7374 725f 746f 5f62 6f6f 6c28  ked(str_to_bool(
-000117a0: 6f34 2929 0d0a 2020 2020 2020 2020 7365  o4))..        se
-000117b0: 6c66 2e63 6865 636b 426f 785f 332e 7365  lf.checkBox_3.se
-000117c0: 7443 6865 636b 6564 2873 7472 5f74 6f5f  tChecked(str_to_
-000117d0: 626f 6f6c 286f 3529 290d 0a20 2020 2020  bool(o5))..     
-000117e0: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
-000117f0: 5f36 2e73 6574 4368 6563 6b65 6428 7374  _6.setChecked(st
-00011800: 725f 746f 5f62 6f6f 6c28 6f36 2929 0d0a  r_to_bool(o6))..
-00011810: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
-00011820: 636b 426f 785f 382e 7365 7443 6865 636b  ckBox_8.setCheck
-00011830: 6564 2873 7472 5f74 6f5f 626f 6f6c 286f  ed(str_to_bool(o
-00011840: 3729 290d 0a20 2020 2020 2020 2073 656c  7))..        sel
-00011850: 662e 6368 6563 6b42 6f78 5f39 2e73 6574  f.checkBox_9.set
-00011860: 4368 6563 6b65 6428 7374 725f 746f 5f62  Checked(str_to_b
-00011870: 6f6f 6c28 6f38 2929 0d0a 2020 2020 2020  ool(o8))..      
-00011880: 2020 7365 6c66 2e63 6865 636b 426f 785f    self.checkBox_
-00011890: 7261 7374 6572 2e73 6574 4368 6563 6b65  raster.setChecke
-000118a0: 6428 7374 725f 746f 5f62 6f6f 6c28 6f39  d(str_to_bool(o9
-000118b0: 2929 0d0a 0d0a 0d0a 2020 2020 6465 6620  ))......    def 
-000118c0: 7361 7665 6173 2873 656c 662c 6669 6c65  saveas(self,file
-000118d0: 6e61 6d65 293a 0d0a 0d0a 2020 2020 2020  name):....      
-000118e0: 2020 6674 6865 6d65 203d 204e 6f6e 650d    ftheme = None.
-000118f0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00011900: 2020 2020 2020 2020 2020 2066 7468 656d             fthem
-00011910: 6520 3d20 6669 6c65 6e61 6d65 5b3a 2d35  e = filename[:-5
-00011920: 5d2b 2273 6663 7468 656d 6522 2023 2061  ]+"sfctheme" # a
-00011930: 6273 6f6c 7574 6520 6669 6c65 2070 6174  bsolute file pat
-00011940: 680d 0a20 2020 2020 2020 2020 2020 2066  h..            f
-00011950: 6f6c 6465 722c 6674 6865 6d65 203d 206f  older,ftheme = o
-00011960: 732e 7061 7468 2e73 706c 6974 2866 7468  s.path.split(fth
-00011970: 656d 6529 2023 2063 6f6e 7665 7274 2074  eme) # convert t
-00011980: 6f20 7265 6c61 7469 7665 2066 696c 6520  o relative file 
-00011990: 7061 7468 0d0a 2020 2020 2020 2020 2020  path..          
-000119a0: 2020 7365 6c66 2e74 6865 6d65 5f6d 616e    self.theme_man
-000119b0: 6167 6572 2e73 6176 655f 636f 6c6f 7273  ager.save_colors
-000119c0: 2866 7468 656d 6529 0d0a 2020 2020 2020  (ftheme)..      
-000119d0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-000119e0: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
-000119f0: 6679 2822 436f 756c 6420 6e6f 7420 7361  fy("Could not sa
-00011a00: 7665 2063 6f6c 6f72 2074 6865 6d65 2e20  ve color theme. 
-00011a10: 7072 6f63 6565 6469 6e67 2077 6974 686f  proceeding witho
-00011a20: 7574 222c 7469 746c 653d 2245 7272 6f72  ut",title="Error
-00011a30: 2229 0d0a 0d0a 0d0a 2020 2020 2020 2020  ")......        
-00011a40: 2320 6472 6177 6361 6e76 6173 2063 6f64  # drawcanvas cod
-00011a50: 655f 6461 7461 0d0a 2020 2020 2020 2020  e_data..        
-00011a60: 636f 6465 5f64 6174 6120 3d20 7b7d 0d0a  code_data = {}..
-00011a70: 2020 2020 2020 2020 666f 7220 6b2c 7620          for k,v 
-00011a80: 696e 2073 656c 662e 6472 6177 6361 6e76  in self.drawcanv
-00011a90: 6173 2e63 6f64 655f 6461 7461 2e69 7465  as.code_data.ite
-00011aa0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00011ab0: 2020 2063 6f64 655f 6461 7461 5b6b 5d20     code_data[k] 
-00011ac0: 3d20 7374 7228 762e 656e 636f 6465 2822  = str(v.encode("
-00011ad0: 7574 662d 3822 292e 6465 636f 6465 2827  utf-8").decode('
-00011ae0: 6370 3132 3532 2729 290d 0a20 2020 2020  cp1252'))..     
-00011af0: 2020 2020 2020 2023 2066 6978 2073 6f6d         # fix som
-00011b00: 6520 706f 7465 6e74 6961 6c20 656e 636f  e potential enco
-00011b10: 6469 6e67 2065 7272 6f72 730d 0a0d 0a20  ding errors.... 
-00011b20: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00011b30: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00011b40: 4649 4c45 4e41 4d45 222c 2066 696c 656e  FILENAME", filen
-00011b50: 616d 6529 0d0a 0d0a 2020 2020 2020 2020  ame)....        
-00011b60: 2020 2020 2320 6c6f 6164 2065 6e74 7269      # load entri
-00011b70: 6573 2069 6e74 6f20 7468 6520 6c69 7374  es into the list
-00011b80: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00011b90: 7468 206f 7065 6e28 6669 6c65 6e61 6d65  th open(filename
-00011ba0: 2c20 2777 2729 2061 7320 7374 7265 616d  , 'w') as stream
-00011bb0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00011bc0: 2020 2020 2064 6174 6120 3d20 7b22 7472       data = {"tr
-00011bd0: 616e 7361 6374 696f 6e73 223a 2073 656c  ansactions": sel
-00011be0: 662e 656e 7472 795f 6461 7461 2c0d 0a20  f.entry_data,.. 
-00011bf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011c00: 6167 656e 7473 223a 2063 6f64 655f 6461  agents": code_da
-00011c10: 7461 2c0d 0a20 2020 2020 2020 2020 2020  ta,..           
-00011c20: 2020 2020 2022 626f 785f 706f 7369 7469       "box_positi
-00011c30: 6f6e 7322 3a20 7365 6c66 2e64 7261 7763  ons": self.drawc
-00011c40: 616e 7661 732e 626f 785f 706f 7369 7469  anvas.box_positi
-00011c50: 6f6e 7328 292c 0d0a 2020 2020 2020 2020  ons(),..        
-00011c60: 2020 2020 2020 2020 226c 6162 656c 5f70          "label_p
-00011c70: 6f73 6974 696f 6e73 223a 2073 656c 662e  ositions": self.
-00011c80: 6472 6177 6361 6e76 6173 2e6c 6162 656c  drawcanvas.label
-00011c90: 5f70 6f73 6974 696f 6e73 2829 2c0d 0a20  _positions(),.. 
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011cb0: 7365 7474 696e 6773 223a 2073 656c 662e  settings": self.
-00011cc0: 7365 7474 696e 6773 5f73 7472 2c0d 0a20  settings_str,.. 
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011ce0: 6d61 696e 6c6f 6f70 223a 2073 656c 662e  mainloop": self.
-00011cf0: 6d61 696e 6c6f 6f70 5f73 7472 2c0d 0a20  mainloop_str,.. 
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011d10: 7468 656d 6522 3a20 7b22 676c 6f62 616c  theme": {"global
-00011d20: 7468 656d 6522 3a20 7365 6c66 2e74 6865  theme": self.the
-00011d30: 6d65 5f6d 616e 6167 6572 2e74 6865 6d65  me_manager.theme
-00011d40: 2c20 2263 6f6c 6f72 7322 3a66 7468 656d  , "colors":fthem
-00011d50: 657d 2c0d 0a20 2020 2020 2020 2020 2020  e},..           
-00011d60: 2020 2020 2022 6e6f 7465 7322 3a20 7365       "notes": se
-00011d70: 6c66 2e6e 6f74 6573 4564 6974 2e74 6f50  lf.notesEdit.toP
-00011d80: 6c61 696e 5465 7874 2829 2c0d 0a20 2020  lainText(),..   
-00011d90: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
-00011da0: 7469 6f6e 7322 3a20 7365 6c66 2e67 6574  tions": self.get
-00011db0: 5f6f 7074 696f 6e73 2829 2c0d 0a20 2020  _options(),..   
-00011dc0: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-00011dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011de0: 2020 7961 6d6c 2e64 756d 7028 6461 7461    yaml.dump(data
-00011df0: 2c73 7472 6561 6d29 0d0a 0d0a 2020 2020  ,stream)....    
-00011e00: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00011e10: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-00011e20: 2020 2020 2020 2020 7365 6c66 2e6e 6f74          self.not
-00011e30: 6966 7928 6d65 7373 6167 653d 7374 7228  ify(message=str(
-00011e40: 6529 2c20 7469 746c 653d 2245 7272 6f72  e), title="Error
-00011e50: 2229 0d0a 0d0a 0d0a 2020 2020 6465 6620  ")......    def 
-00011e60: 7472 795f 6765 6e5f 6d61 7472 6978 2873  try_gen_matrix(s
-00011e70: 656c 6629 3a0d 0a20 2020 2020 2020 2074  elf):..        t
-00011e80: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00011e90: 2073 656c 662e 6765 6e5f 6d61 7472 6978   self.gen_matrix
-00011ea0: 2829 0d0a 2020 2020 2020 2020 6578 6365  ()..        exce
-00011eb0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00011ec0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00011ed0: 7365 6c66 2e6e 6f74 6966 7928 2245 7272  self.notify("Err
-00011ee0: 6f72 222c 7374 7228 6529 290d 0a0d 0a20  or",str(e)).... 
-00011ef0: 2020 2064 6566 2067 656e 5f6d 6174 7269     def gen_matri
-00011f00: 7828 7365 6c66 2c6d 6f64 653d 2273 7461  x(self,mode="sta
-00011f10: 6e64 6172 6422 293a 0d0a 2020 2020 2020  ndard"):..      
-00011f20: 2020 2222 220d 0a20 2020 2020 2020 2067    """..        g
-00011f30: 656e 6572 6174 6520 666c 6f77 206d 6174  enerate flow mat
-00011f40: 7269 783a 0d0a 0d0a 2020 2020 2020 2020  rix:....        
-00011f50: 3a70 6172 616d 206d 6f64 653a 2073 7461  :param mode: sta
-00011f60: 6e64 6172 642c 6578 6365 6c2c 6c61 7465  ndard,excel,late
-00011f70: 780d 0a0d 0a20 2020 2020 2020 2073 7461  x....        sta
-00011f80: 6e64 6172 643a 2073 686f 7773 206d 6174  ndard: shows mat
-00011f90: 7269 7820 6772 6170 6869 6361 6c6c 790d  rix graphically.
-00011fa0: 0a20 2020 2020 2020 2065 7863 656c 3a20  .        excel: 
-00011fb0: 6578 706f 7274 7320 616e 2065 7863 656c  exports an excel
-00011fc0: 2066 696c 650d 0a20 2020 2020 2020 206c   file..        l
-00011fd0: 6174 6578 3a20 6e6f 7420 7965 7420 7375  atex: not yet su
-00011fe0: 7070 6f72 7465 6420 4e4f 5420 4156 4149  pported NOT AVAI
-00011ff0: 4c41 424c 4520 464f 5220 4e4f 570d 0a20  LABLE FOR NOW.. 
-00012000: 2020 2020 2020 2068 746d 6c3a 204e 4f54         html: NOT
-00012010: 2041 5641 494c 4142 4c45 2046 4f52 204e   AVAILABLE FOR N
-00012020: 4f57 0d0a 2020 2020 2020 2020 2222 220d  OW..        """.
-00012030: 0a0d 0a20 2020 2020 2020 2066 6c6f 775f  ...        flow_
-00012040: 6461 7461 203d 207b 7d0d 0a0d 0a20 2020  data = {}....   
-00012050: 2020 2020 2066 6c6f 775f 6461 7461 5b22       flow_data["
-00012060: 4341 225d 203d 2064 6566 6175 6c74 6469  CA"] = defaultdi
-00012070: 6374 286c 616d 6264 613a 2064 6566 6175  ct(lambda: defau
-00012080: 6c74 6469 6374 286c 6973 7429 2920 2023  ltdict(list))  #
-00012090: 2063 7572 7265 6e74 2061 6363 6f75 6e74   current account
+0000ddd0: 6e76 6173 2e72 6570 6f73 6974 696f 6e28  nvas.reposition(
+0000dde0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000ddf0: 6472 6177 6361 6e76 6173 2e72 6570 6f73  drawcanvas.repos
+0000de00: 6974 696f 6e5f 6c61 6265 6c73 2829 0d0a  ition_labels()..
+0000de10: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+0000de20: 7261 7763 616e 7661 732e 7570 6461 7465  rawcanvas.update
+0000de30: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0000de40: 2e6d 6164 655f 6368 616e 6765 7320 3d20  .made_changes = 
+0000de50: 4661 6c73 650d 0a0d 0a0d 0a0d 0a0d 0a20  False.......... 
+0000de60: 2020 2064 6566 206d 6f76 655f 646f 776e     def move_down
+0000de70: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+0000de80: 2023 206d 6f76 6520 7365 6c65 6374 6564   # move selected
+0000de90: 2074 7261 6e73 6163 7469 6f6e 2075 7020   transaction up 
+0000dea0: 696e 2074 6162 6c65 0d0a 2020 2020 2020  in table..      
+0000deb0: 2020 7365 6c65 6374 6564 5f72 6f77 7320    selected_rows 
+0000dec0: 3d20 736f 7274 6564 2873 6574 2869 6e64  = sorted(set(ind
+0000ded0: 6578 2e72 6f77 2829 2066 6f72 2069 6e64  ex.row() for ind
+0000dee0: 6578 2069 6e0d 0a20 2020 2020 2020 2020  ex in..         
+0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df00: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000df10: 6e56 6965 772e 7365 6c65 6374 6564 496e  nView.selectedIn
+0000df20: 6465 7865 7328 2929 290d 0a0d 0a20 2020  dexes()))....   
+0000df30: 2020 2020 2069 6620 6c65 6e28 7365 6c65       if len(sele
+0000df40: 6374 6564 5f72 6f77 7329 203d 3d20 303a  cted_rows) == 0:
+0000df50: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000df60: 696e 7428 226e 6f20 7365 6c65 6374 6564  int("no selected
+0000df70: 2072 6f77 7322 290d 0a20 2020 2020 2020   rows")..       
+0000df80: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+0000df90: 2020 2020 2020 2073 656c 6563 7469 6f6e         selection
+0000dfa0: 203d 2073 656c 6563 7465 645f 726f 7773   = selected_rows
+0000dfb0: 5b30 5d0d 0a0d 0a20 2020 2020 2020 206e  [0]....        n
+0000dfc0: 756d 6265 725f 6f66 5f69 7465 6d73 203d  umber_of_items =
+0000dfd0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000dfe0: 6e56 6965 772e 726f 7743 6f75 6e74 2829  nView.rowCount()
+0000dff0: 0d0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
+0000e000: 5f6f 665f 636f 6c75 6d6e 7320 3d20 7365  _of_columns = se
+0000e010: 6c66 2e74 7261 6e73 6163 7469 6f6e 5669  lf.transactionVi
+0000e020: 6577 2e63 6f6c 756d 6e43 6f75 6e74 2829  ew.columnCount()
+0000e030: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
+0000e040: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000e050: 6966 2073 656c 6563 7469 6f6e 203c 206e  if selection < n
+0000e060: 756d 6265 725f 6f66 5f69 7465 6d73 2d31  umber_of_items-1
+0000e070: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e080: 2020 2063 7572 7265 6e74 526f 7720 3d20     currentRow = 
+0000e090: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+0000e0a0: 5669 6577 2e63 7572 7265 6e74 526f 7728  View.currentRow(
+0000e0b0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000e0c0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0000e0d0: 6e67 6528 6e75 6d62 6572 5f6f 665f 636f  nge(number_of_co
+0000e0e0: 6c75 6d6e 7329 3a0d 0a20 2020 2020 2020  lumns):..       
+0000e0f0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0000e100: 7265 6e74 4974 656d 203d 2073 656c 662e  rentItem = self.
+0000e110: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+0000e120: 7461 6b65 4974 656d 2863 7572 7265 6e74  takeItem(current
+0000e130: 526f 772c 6a29 0d0a 2020 2020 2020 2020  Row,j)..        
+0000e140: 2020 2020 2020 2020 2020 2020 7377 6974              swit
+0000e150: 6368 4974 656d 203d 2073 656c 662e 7472  chItem = self.tr
+0000e160: 616e 7361 6374 696f 6e56 6965 772e 7461  ansactionView.ta
+0000e170: 6b65 4974 656d 2863 7572 7265 6e74 526f  keItem(currentRo
+0000e180: 772b 312c 6a29 0d0a 0d0a 2020 2020 2020  w+1,j)....      
+0000e190: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e1a0: 6c66 2e74 7261 6e73 6163 7469 6f6e 5669  lf.transactionVi
+0000e1b0: 6577 2e73 6574 4974 656d 2863 7572 7265  ew.setItem(curre
+0000e1c0: 6e74 526f 7720 2b20 312c 206a 2c20 6375  ntRow + 1, j, cu
+0000e1d0: 7272 656e 7449 7465 6d29 0d0a 2020 2020  rrentItem)..    
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+0000e200: 5669 6577 2e73 6574 4974 656d 2863 7572  View.setItem(cur
+0000e210: 7265 6e74 526f 772c 206a 2c20 7377 6974  rentRow, j, swit
+0000e220: 6368 4974 656d 290d 0a0d 0a20 2020 2020  chItem)....     
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e240: 7769 7463 685f 656e 7472 7920 3d20 7365  witch_entry = se
+0000e250: 6c66 2e65 6e74 7279 5f64 6174 615b 6375  lf.entry_data[cu
+0000e260: 7272 656e 7452 6f77 2b31 5d0d 0a20 2020  rrentRow+1]..   
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2063 7572 7265 6e74 5f65 6e74 7279 203d   current_entry =
+0000e290: 2073 656c 662e 656e 7472 795f 6461 7461   self.entry_data
+0000e2a0: 5b63 7572 7265 6e74 526f 775d 0d0a 0d0a  [currentRow]....
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2c0: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
+0000e2d0: 6174 615b 6375 7272 656e 7452 6f77 5d20  ata[currentRow] 
+0000e2e0: 3d20 7377 6974 6368 5f65 6e74 7279 0d0a  = switch_entry..
+0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e300: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
+0000e310: 6174 615b 6375 7272 656e 7452 6f77 2b31  ata[currentRow+1
+0000e320: 5d20 3d20 6375 7272 656e 745f 656e 7472  ] = current_entr
+0000e330: 790d 0a0d 0a20 2020 2020 2020 2020 2020  y....           
+0000e340: 2020 2020 2073 656c 662e 7472 616e 7361       self.transa
+0000e350: 6374 696f 6e56 6965 772e 636c 6561 7253  ctionView.clearS
+0000e360: 656c 6563 7469 6f6e 2829 0d0a 2020 2020  election()..    
+0000e370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e380: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
+0000e390: 2e73 6574 4375 7272 656e 7443 656c 6c28  .setCurrentCell(
+0000e3a0: 6375 7272 656e 7452 6f77 2b31 2c30 290d  currentRow+1,0).
+0000e3b0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
+0000e3c0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000e3d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0000e3e0: 656c 662e 6e6f 7469 6679 2822 6572 726f  elf.notify("erro
+0000e3f0: 723a 2022 2b73 7472 2865 292c 2074 6974  r: "+str(e), tit
+0000e400: 6c65 3d22 4572 726f 7222 290d 0a0d 0a0d  le="Error").....
+0000e410: 0a20 2020 2064 6566 206d 6f76 655f 7570  .    def move_up
+0000e420: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+0000e430: 2023 206d 6f76 6520 7365 6c65 6374 6564   # move selected
+0000e440: 2074 7261 6e73 6163 7469 6f6e 2075 7020   transaction up 
+0000e450: 696e 2074 6162 6c65 0d0a 2020 2020 2020  in table..      
+0000e460: 2020 7365 6c65 6374 6564 5f72 6f77 7320    selected_rows 
+0000e470: 3d20 736f 7274 6564 2873 6574 2869 6e64  = sorted(set(ind
+0000e480: 6578 2e72 6f77 2829 2066 6f72 2069 6e64  ex.row() for ind
+0000e490: 6578 2069 6e0d 0a20 2020 2020 2020 2020  ex in..         
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000e4c0: 6e56 6965 772e 7365 6c65 6374 6564 496e  nView.selectedIn
+0000e4d0: 6465 7865 7328 2929 290d 0a0d 0a20 2020  dexes()))....   
+0000e4e0: 2020 2020 2069 6620 6c65 6e28 7365 6c65       if len(sele
+0000e4f0: 6374 6564 5f72 6f77 7329 203d 3d20 303a  cted_rows) == 0:
+0000e500: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000e510: 696e 7428 226e 6f20 7365 6c65 6374 6564  int("no selected
+0000e520: 2072 6f77 7322 290d 0a20 2020 2020 2020   rows")..       
+0000e530: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+0000e540: 2020 2020 2020 2073 656c 6563 7469 6f6e         selection
+0000e550: 203d 2073 656c 6563 7465 645f 726f 7773   = selected_rows
+0000e560: 5b30 5d0d 0a0d 0a20 2020 2020 2020 206e  [0]....        n
+0000e570: 756d 6265 725f 6f66 5f69 7465 6d73 203d  umber_of_items =
+0000e580: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000e590: 6e56 6965 772e 726f 7743 6f75 6e74 2829  nView.rowCount()
+0000e5a0: 0d0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
+0000e5b0: 5f6f 665f 636f 6c75 6d6e 7320 3d20 7365  _of_columns = se
+0000e5c0: 6c66 2e74 7261 6e73 6163 7469 6f6e 5669  lf.transactionVi
+0000e5d0: 6577 2e63 6f6c 756d 6e43 6f75 6e74 2829  ew.columnCount()
+0000e5e0: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
+0000e5f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000e600: 6966 2073 656c 6563 7469 6f6e 203e 3d20  if selection >= 
+0000e610: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0000e620: 2020 2020 6375 7272 656e 7452 6f77 203d      currentRow =
+0000e630: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000e640: 6e56 6965 772e 6375 7272 656e 7452 6f77  nView.currentRow
+0000e650: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+0000e660: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+0000e670: 616e 6765 286e 756d 6265 725f 6f66 5f63  ange(number_of_c
+0000e680: 6f6c 756d 6e73 293a 0d0a 2020 2020 2020  olumns):..      
+0000e690: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000e6a0: 7272 656e 7449 7465 6d20 3d20 7365 6c66  rrentItem = self
+0000e6b0: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
+0000e6c0: 2e74 616b 6549 7465 6d28 6375 7272 656e  .takeItem(curren
+0000e6d0: 7452 6f77 2c6a 290d 0a20 2020 2020 2020  tRow,j)..       
+0000e6e0: 2020 2020 2020 2020 2020 2020 2073 7769               swi
+0000e6f0: 7463 6849 7465 6d20 3d20 7365 6c66 2e74  tchItem = self.t
+0000e700: 7261 6e73 6163 7469 6f6e 5669 6577 2e74  ransactionView.t
+0000e710: 616b 6549 7465 6d28 6375 7272 656e 7452  akeItem(currentR
+0000e720: 6f77 2d31 2c6a 290d 0a0d 0a20 2020 2020  ow-1,j)....     
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e740: 656c 662e 7472 616e 7361 6374 696f 6e56  elf.transactionV
+0000e750: 6965 772e 7365 7449 7465 6d28 6375 7272  iew.setItem(curr
+0000e760: 656e 7452 6f77 202d 2031 2c20 6a2c 2063  entRow - 1, j, c
+0000e770: 7572 7265 6e74 4974 656d 290d 0a20 2020  urrentItem)..   
+0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e790: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000e7a0: 6e56 6965 772e 7365 7449 7465 6d28 6375  nView.setItem(cu
+0000e7b0: 7272 656e 7452 6f77 2c20 6a2c 2073 7769  rrentRow, j, swi
+0000e7c0: 7463 6849 7465 6d29 0d0a 0d0a 2020 2020  tchItem)....    
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7e0: 7377 6974 6368 5f65 6e74 7279 203d 2073  switch_entry = s
+0000e7f0: 656c 662e 656e 7472 795f 6461 7461 5b63  elf.entry_data[c
+0000e800: 7572 7265 6e74 526f 772d 315d 0d0a 2020  urrentRow-1]..  
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 6375 7272 656e 745f 656e 7472 7920    current_entry 
+0000e830: 3d20 7365 6c66 2e65 6e74 7279 5f64 6174  = self.entry_dat
+0000e840: 615b 6375 7272 656e 7452 6f77 5d0d 0a0d  a[currentRow]...
+0000e850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e860: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
+0000e870: 6461 7461 5b63 7572 7265 6e74 526f 775d  data[currentRow]
+0000e880: 203d 2073 7769 7463 685f 656e 7472 790d   = switch_entry.
+0000e890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e8a0: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
+0000e8b0: 6461 7461 5b63 7572 7265 6e74 526f 772d  data[currentRow-
+0000e8c0: 315d 203d 2063 7572 7265 6e74 5f65 6e74  1] = current_ent
+0000e8d0: 7279 0d0a 0d0a 2020 2020 2020 2020 2020  ry....          
+0000e8e0: 2020 2020 2020 7365 6c66 2e74 7261 6e73        self.trans
+0000e8f0: 6163 7469 6f6e 5669 6577 2e63 6c65 6172  actionView.clear
+0000e900: 5365 6c65 6374 696f 6e28 290d 0a20 2020  Selection()..   
+0000e910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e920: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+0000e930: 772e 7365 7443 7572 7265 6e74 4365 6c6c  w.setCurrentCell
+0000e940: 2863 7572 7265 6e74 526f 772d 312c 3029  (currentRow-1,0)
+0000e950: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0000e960: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+0000e970: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e980: 7365 6c66 2e6e 6f74 6966 7928 2265 7272  self.notify("err
+0000e990: 6f72 3a20 222b 7374 7228 6529 2c20 7469  or: "+str(e), ti
+0000e9a0: 746c 653d 2245 7272 6f72 2229 0d0a 0d0a  tle="Error")....
+0000e9b0: 2020 2020 6465 6620 6461 7461 5f73 656c      def data_sel
+0000e9c0: 6563 7428 7365 6c66 293a 0d0a 0d0a 2020  ect(self):....  
+0000e9d0: 2020 2020 2020 2373 656c 6563 7465 645f        #selected_
+0000e9e0: 726f 7773 203d 2073 656c 662e 7472 616e  rows = self.tran
+0000e9f0: 7361 6374 696f 6e56 6965 772e 7365 6c65  sactionView.sele
+0000ea00: 6374 696f 6e4d 6f64 656c 2829 2e73 656c  ctionModel().sel
+0000ea10: 6563 7465 6452 6f77 7328 290d 0a20 2020  ectedRows()..   
+0000ea20: 2020 2020 2073 656c 6563 7465 645f 726f       selected_ro
+0000ea30: 7773 203d 2073 6f72 7465 6428 7365 7428  ws = sorted(set(
+0000ea40: 696e 6465 782e 726f 7728 2920 666f 7220  index.row() for 
+0000ea50: 696e 6465 7820 696e 0d0a 2020 2020 2020  index in..      
+0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea70: 2020 2020 7365 6c66 2e74 7261 6e73 6163      self.transac
+0000ea80: 7469 6f6e 5669 6577 2e73 656c 6563 7465  tionView.selecte
+0000ea90: 6449 6e64 6578 6573 2829 2929 0d0a 0d0a  dIndexes()))....
+0000eaa0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+0000eab0: 656c 6563 7465 645f 726f 7773 2920 3d3d  elected_rows) ==
+0000eac0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0000ead0: 2070 7269 6e74 2822 6e6f 2073 656c 6563   print("no selec
+0000eae0: 7465 6420 726f 7773 2229 0d0a 2020 2020  ted rows")..    
+0000eaf0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+0000eb00: 0d0a 2020 2020 2020 2020 7365 6c65 6374  ..        select
+0000eb10: 696f 6e20 3d20 7365 6c65 6374 6564 5f72  ion = selected_r
+0000eb20: 6f77 735b 305d 0d0a 0d0a 2020 2020 2020  ows[0]....      
+0000eb30: 2020 7365 6c66 2e72 6f77 5f73 656c 6563    self.row_selec
+0000eb40: 7428 7365 6c65 6374 696f 6e29 0d0a 2020  t(selection)..  
+0000eb50: 2020 2020 2020 7365 6c66 2e6d 6164 655f        self.made_
+0000eb60: 6368 616e 6765 7320 3d20 4661 6c73 650d  changes = False.
+0000eb70: 0a0d 0a0d 0a20 2020 2064 6566 2064 6174  .....    def dat
+0000eb80: 615f 7365 6c65 6374 5f77 6865 7265 2873  a_select_where(s
+0000eb90: 656c 662c 6578 7072 293a 0d0a 2020 2020  elf,expr):..    
+0000eba0: 2020 2020 7072 696e 7428 2264 6174 6120      print("data 
+0000ebb0: 7365 6c65 6374 2077 6865 7265 222c 6578  select where",ex
+0000ebc0: 7072 290d 0a0d 0a20 2020 2020 2020 2066  pr)....        f
+0000ebd0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+0000ebe0: 6c66 2e74 7261 6e73 6163 7469 6f6e 5669  lf.transactionVi
+0000ebf0: 6577 2e72 6f77 436f 756e 7428 2929 3a0d  ew.rowCount()):.
+0000ec00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec10: 206d 795f 656e 7472 7920 3d20 7365 6c66   my_entry = self
+0000ec20: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
+0000ec30: 2e69 7465 6d28 692c 2033 292e 7465 7874  .item(i, 3).text
+0000ec40: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+0000ec50: 2020 2020 2020 7072 696e 7428 222e 2e2e        print("...
+0000ec60: 222c 692c 6d79 5f65 6e74 7279 290d 0a20  ",i,my_entry).. 
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000ec80: 6620 6d79 5f65 6e74 7279 203d 3d20 6578  f my_entry == ex
+0000ec90: 7072 206f 7220 6d79 5f65 6e74 7279 2e6c  pr or my_entry.l
+0000eca0: 6f77 6572 2829 203d 3d20 6578 7072 2e6c  ower() == expr.l
+0000ecb0: 6f77 6572 2829 3a0d 0a0d 0a20 2020 2020  ower():....     
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ecd0: 656c 662e 726f 775f 7365 6c65 6374 2869  elf.row_select(i
+0000ece0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ecf0: 2020 2020 2020 2072 6574 7572 6e0d 0a0d         return...
+0000ed00: 0a20 2020 2064 6566 2072 6f77 5f73 656c  .    def row_sel
+0000ed10: 6563 7428 7365 6c66 2c73 656c 6563 7469  ect(self,selecti
+0000ed20: 6f6e 293a 0d0a 0d0a 2020 2020 2020 2020  on):....        
+0000ed30: 2320 636f 6c6f 7220 7468 6520 7365 6c65  # color the sele
+0000ed40: 6374 6564 2072 6f77 0d0a 2020 2020 2020  cted row..      
+0000ed50: 2020 2320 6762 2832 3333 2c20 3233 342c    # gb(233, 234,
+0000ed60: 2032 3237 293b 0d0a 0d0a 2020 2020 2020   227);....      
+0000ed70: 2020 7365 6c66 2e73 656c 6563 7469 6f6e    self.selection
+0000ed80: 5f69 6478 203d 204e 6f6e 650d 0a0d 0a20  _idx = None.... 
+0000ed90: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+0000eda0: 6164 655f 6368 616e 6765 733a 0d0a 2020  ade_changes:..  
+0000edb0: 2020 2020 2020 2020 2020 7965 7320 3d20            yes = 
+0000edc0: 7365 6c66 2e61 736b 5f71 7565 7374 696f  self.ask_questio
+0000edd0: 6e28 2257 6172 6e69 6e67 222c 2022 596f  n("Warning", "Yo
+0000ede0: 7520 6172 6520 6162 6f75 7420 746f 2063  u are about to c
+0000edf0: 6861 6e67 6520 746f 2061 6e6f 7468 6572  hange to another
+0000ee00: 2074 7261 6e73 6163 7469 6f6e 2061 6e64   transaction and
+0000ee10: 2077 6974 6864 7261 7720 7468 6520 6368   withdraw the ch
+0000ee20: 616e 6765 7320 796f 7520 6d61 6465 2e20  anges you made. 
+0000ee30: 436f 6e74 696e 7565 3f22 290d 0a20 2020  Continue?")..   
+0000ee40: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000ee50: 7965 733a 0d0a 2020 2020 2020 2020 2020  yes:..          
+0000ee60: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
+0000ee70: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000ee80: 2020 2020 2020 2020 2020 2222 220d 0a20            """.. 
+0000ee90: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000eea0: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
+0000eeb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000eed0: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+0000eee0: 6c66 2e74 7261 6e73 6163 7469 6f6e 5669  lf.transactionVi
+0000eef0: 6577 2e63 6f6c 756d 6e43 6f75 6e74 2829  ew.columnCount()
+0000ef00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000ef10: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000ef20: 6e73 6163 7469 6f6e 5669 6577 2e69 7465  nsactionView.ite
+0000ef30: 6d28 7365 6c66 2e73 656c 6563 7469 6f6e  m(self.selection
+0000ef40: 5f69 6478 2c20 6929 2e73 6574 4261 636b  _idx, i).setBack
+0000ef50: 6772 6f75 6e64 2851 7447 7569 2e51 436f  ground(QtGui.QCo
+0000ef60: 6c6f 7228 3233 332c 2032 3334 2c20 3232  lor(233, 234, 22
+0000ef70: 3729 290d 0a20 2020 2020 2020 2020 2020  7))..           
+0000ef80: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000ef90: 616e 7361 6374 696f 6e56 6965 772e 7363  ansactionView.sc
+0000efa0: 726f 6c6c 546f 4974 656d 2873 656c 662e  rollToItem(self.
+0000efb0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+0000efc0: 6974 656d 2873 656c 6563 7469 6f6e 2c20  item(selection, 
+0000efd0: 6929 290d 0a20 2020 2020 2020 2020 2020  i))..           
+0000efe0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000eff0: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+0000f000: 5669 6577 2e63 6f6c 756d 6e43 6f75 6e74  View.columnCount
+0000f010: 2829 293a 0d0a 2020 2020 2020 2020 2020  ()):..          
+0000f020: 2020 2020 2020 7365 6c66 2e74 7261 6e73        self.trans
+0000f030: 6163 7469 6f6e 5669 6577 2e69 7465 6d28  actionView.item(
+0000f040: 7365 6c65 6374 696f 6e2c 2069 292e 7365  selection, i).se
+0000f050: 7442 6163 6b67 726f 756e 6428 5174 4775  tBackground(QtGu
+0000f060: 692e 5143 6f6c 6f72 2835 392c 2035 392c  i.QColor(59, 59,
+0000f070: 2031 3539 2929 0d0a 2020 2020 2020 2020   159))..        
+0000f080: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000f090: 6e73 6163 7469 6f6e 5669 6577 2e73 6372  nsactionView.scr
+0000f0a0: 6f6c 6c54 6f49 7465 6d28 7365 6c66 2e74  ollToItem(self.t
+0000f0b0: 7261 6e73 6163 7469 6f6e 5669 6577 2e69  ransactionView.i
+0000f0c0: 7465 6d28 7365 6c65 6374 696f 6e2c 2069  tem(selection, i
+0000f0d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000f0e0: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+0000f0f0: 2073 656c 662e 7472 616e 7361 6374 696f   self.transactio
+0000f100: 6e56 6965 772e 636c 6561 7253 656c 6563  nView.clearSelec
+0000f110: 7469 6f6e 2829 0d0a 2020 2020 2020 2020  tion()..        
+0000f120: 2020 2020 7365 6c66 2e74 7261 6e73 6163      self.transac
+0000f130: 7469 6f6e 5669 6577 2e73 6574 4375 7272  tionView.setCurr
+0000f140: 656e 7443 656c 6c28 7365 6c65 6374 696f  entCell(selectio
+0000f150: 6e2c 3329 0d0a 0d0a 0d0a 0d0a 2020 2020  n,3)........    
+0000f160: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+0000f170: 2020 2020 2020 2020 2070 6173 730d 0a0d           pass...
+0000f180: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+0000f190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f1a0: 7365 6c65 6374 696f 6e5f 6964 7820 3d20  selection_idx = 
+0000f1b0: 7365 6c65 6374 696f 6e0d 0a20 2020 2020  selection..     
+0000f1c0: 2020 2020 2020 2070 7269 6e74 2822 7365         print("se
+0000f1d0: 6c65 6374 696f 6e22 2c73 656c 6563 7469  lection",selecti
+0000f1e0: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
+0000f1f0: 2020 2064 6174 6120 3d20 7365 6c66 2e65     data = self.e
+0000f200: 6e74 7279 5f64 6174 615b 7365 6c65 6374  ntry_data[select
+0000f210: 696f 6e5d 0d0a 0d0a 2020 2020 2020 2020  ion]....        
+0000f220: 2020 2020 7072 696e 7428 2264 6174 6122      print("data"
+0000f230: 2c20 6461 7461 290d 0a0d 0a20 2020 2020  , data)....     
+0000f240: 2020 2020 2020 2073 656c 662e 4173 7365         self.Asse
+0000f250: 744c 6973 744c 6566 742e 636c 6561 7228  tListLeft.clear(
+0000f260: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000f270: 656c 662e 4c69 6162 696c 6974 794c 6973  elf.LiabilityLis
+0000f280: 744c 6566 742e 636c 6561 7228 290d 0a20  tLeft.clear().. 
+0000f290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f2a0: 4c69 6162 696c 6974 794c 6973 7452 6967  LiabilityListRig
+0000f2b0: 6874 2e63 6c65 6172 2829 0d0a 2020 2020  ht.clear()..    
+0000f2c0: 2020 2020 2020 2020 7365 6c66 2e41 7373          self.Ass
+0000f2d0: 6574 4c69 7374 5269 6768 742e 636c 6561  etListRight.clea
+0000f2e0: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+0000f2f0: 2073 656c 662e 4571 7569 7479 4c69 7374   self.EquityList
+0000f300: 4c65 6674 2e63 6c65 6172 2829 0d0a 2020  Left.clear()..  
+0000f310: 2020 2020 2020 2020 2020 7365 6c66 2e45            self.E
+0000f320: 7175 6974 794c 6973 7452 6967 6874 2e63  quityListRight.c
+0000f330: 6c65 6172 2829 0d0a 0d0a 2020 2020 2020  lear()....      
+0000f340: 2020 2020 2020 7365 6c66 2e41 7373 6574        self.Asset
+0000f350: 4c69 7374 4c65 6674 2e73 6574 506c 6169  ListLeft.setPlai
+0000f360: 6e54 6578 7428 6461 7461 5b22 6131 225d  nText(data["a1"]
+0000f370: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000f380: 656c 662e 4173 7365 744c 6973 7452 6967  elf.AssetListRig
+0000f390: 6874 2e73 6574 506c 6169 6e54 6578 7428  ht.setPlainText(
+0000f3a0: 6461 7461 5b22 6132 225d 290d 0a20 2020  data["a2"])..   
+0000f3b0: 2020 2020 2020 2020 2073 656c 662e 4c69           self.Li
+0000f3c0: 6162 696c 6974 794c 6973 744c 6566 742e  abilityListLeft.
+0000f3d0: 7365 7450 6c61 696e 5465 7874 2864 6174  setPlainText(dat
+0000f3e0: 615b 226c 3122 5d29 2020 2320 2b64 6174  a["l1"])  # +dat
+0000f3f0: 615b 2265 3122 5d29 0d0a 2020 2020 2020  a["e1"])..      
+0000f400: 2020 2020 2020 7365 6c66 2e4c 6961 6269        self.Liabi
+0000f410: 6c69 7479 4c69 7374 5269 6768 742e 7365  lityListRight.se
+0000f420: 7450 6c61 696e 5465 7874 2864 6174 615b  tPlainText(data[
+0000f430: 226c 3222 5d29 2023 202b 6461 7461 5b22  "l2"]) # +data["
+0000f440: 6532 225d 290d 0a20 2020 2020 2020 2020  e2"])..         
+0000f450: 2020 2073 656c 662e 4571 7569 7479 4c69     self.EquityLi
+0000f460: 7374 4c65 6674 2e73 6574 506c 6169 6e54  stLeft.setPlainT
+0000f470: 6578 7428 6461 7461 5b22 6531 225d 290d  ext(data["e1"]).
+0000f480: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f490: 662e 4571 7569 7479 4c69 7374 5269 6768  f.EquityListRigh
+0000f4a0: 742e 7365 7450 6c61 696e 5465 7874 2864  t.setPlainText(d
+0000f4b0: 6174 615b 2265 3222 5d29 0d0a 0d0a 2020  ata["e2"])....  
+0000f4c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000f4d0: 6765 6e74 3145 6469 742e 7365 7454 6578  gent1Edit.setTex
+0000f4e0: 7428 6361 6d65 6c28 6461 7461 5b22 6167  t(camel(data["ag
+0000f4f0: 656e 7431 225d 2929 2023 2e63 6170 6974  ent1"])) #.capit
+0000f500: 616c 697a 6528 2929 0d0a 2020 2020 2020  alize())..      
+0000f510: 2020 2020 2020 7365 6c66 2e61 6765 6e74        self.agent
+0000f520: 3245 6469 742e 7365 7454 6578 7428 6361  2Edit.setText(ca
+0000f530: 6d65 6c28 6461 7461 5b22 6167 656e 7432  mel(data["agent2
+0000f540: 225d 2929 2023 202e 6361 7069 7461 6c69  "])) # .capitali
+0000f550: 7a65 2829 290d 0a0d 0a20 2020 2020 2020  ze())....       
+0000f560: 2020 2020 2073 656c 662e 7265 6769 7374       self.regist
+0000f570: 6572 466c 6f77 426f 782e 7365 7443 7572  erFlowBox.setCur
+0000f580: 7265 6e74 496e 6465 7828 7365 6c66 2e72  rentIndex(self.r
+0000f590: 6567 6973 7465 7246 6c6f 7742 6f78 2e66  egisterFlowBox.f
+0000f5a0: 696e 6454 6578 7428 7374 7228 6461 7461  indText(str(data
+0000f5b0: 5b22 6c6f 6720 7472 616e 7361 6374 696f  ["log transactio
+0000f5c0: 6e22 5d29 2929 0d0a 0d0a 2020 2020 2020  n"])))....      
+0000f5d0: 2020 2020 2020 6361 7368 666c 6f77 3120        cashflow1 
+0000f5e0: 3d20 6461 7461 5b22 6361 7368 666c 6f77  = data["cashflow
+0000f5f0: 3122 5d20 6f72 2022 4e6f 6e65 220d 0a20  1"] or "None".. 
+0000f600: 2020 2020 2020 2020 2020 2063 6173 6866             cashf
+0000f610: 6c6f 7732 203d 2064 6174 615b 2263 6173  low2 = data["cas
+0000f620: 6866 6c6f 7732 225d 206f 7220 224e 6f6e  hflow2"] or "Non
+0000f630: 6522 0d0a 2020 2020 2020 2020 2020 2020  e"..            
+0000f640: 7365 6c66 2e63 6f6d 626f 4361 7368 4c65  self.comboCashLe
+0000f650: 6674 2e73 6574 4375 7272 656e 7449 6e64  ft.setCurrentInd
+0000f660: 6578 2873 656c 662e 636f 6d62 6f43 6173  ex(self.comboCas
+0000f670: 684c 6566 742e 6669 6e64 5465 7874 2873  hLeft.findText(s
+0000f680: 7472 2863 6173 6866 6c6f 7731 2929 290d  tr(cashflow1))).
+0000f690: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f6a0: 662e 636f 6d62 6f43 6173 6852 6967 6874  f.comboCashRight
+0000f6b0: 2e73 6574 4375 7272 656e 7449 6e64 6578  .setCurrentIndex
+0000f6c0: 2873 656c 662e 636f 6d62 6f43 6173 6852  (self.comboCashR
+0000f6d0: 6967 6874 2e66 696e 6454 6578 7428 7374  ight.findText(st
+0000f6e0: 7228 6361 7368 666c 6f77 3229 2929 0d0a  r(cashflow2)))..
+0000f6f0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0000f700: 7479 7065 203d 2064 6174 615b 226b 696e  type = data["kin
+0000f710: 6422 5d20 6f72 2022 4b41 2d3e 4b41 220d  d"] or "KA->KA".
+0000f720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f730: 662e 6564 6974 5479 7065 2e73 6574 4375  f.editType.setCu
+0000f740: 7272 656e 7449 6e64 6578 2873 656c 662e  rrentIndex(self.
+0000f750: 6564 6974 5479 7065 2e66 696e 6454 6578  editType.findTex
+0000f760: 7428 7374 7228 7472 7479 7065 2929 290d  t(str(trtype))).
+0000f770: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0000f780: 6373 3120 3d20 6461 7461 5b22 696e 636f  cs1 = data["inco
+0000f790: 6d65 3122 5d20 6f72 2022 4e6f 6e65 220d  me1"] or "None".
+0000f7a0: 0a20 2020 2020 2020 2020 2020 2069 6373  .            ics
+0000f7b0: 3220 3d20 6461 7461 5b22 696e 636f 6d65  2 = data["income
+0000f7c0: 3222 5d20 6f72 2022 4e6f 6e65 220d 0a20  2"] or "None".. 
+0000f7d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f7e0: 636f 6d62 6f49 6e63 6f6d 654c 6566 742e  comboIncomeLeft.
+0000f7f0: 7365 7443 7572 7265 6e74 496e 6465 7828  setCurrentIndex(
+0000f800: 7365 6c66 2e63 6f6d 626f 496e 636f 6d65  self.comboIncome
+0000f810: 4c65 6674 2e66 696e 6454 6578 7428 6963  Left.findText(ic
+0000f820: 7331 2929 0d0a 2020 2020 2020 2020 2020  s1))..          
+0000f830: 2020 7365 6c66 2e63 6f6d 626f 496e 636f    self.comboInco
+0000f840: 6d65 5269 6768 742e 7365 7443 7572 7265  meRight.setCurre
+0000f850: 6e74 496e 6465 7828 7365 6c66 2e63 6f6d  ntIndex(self.com
+0000f860: 626f 496e 636f 6d65 5269 6768 742e 6669  boIncomeRight.fi
+0000f870: 6e64 5465 7874 2869 6373 3229 290d 0a0d  ndText(ics2))...
+0000f880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f890: 662e 6564 6974 5175 616e 7469 7479 2e73  f.editQuantity.s
+0000f8a0: 6574 5465 7874 2864 6174 615b 2271 7561  etText(data["qua
+0000f8b0: 6e74 6974 7922 5d29 0d0a 2020 2020 2020  ntity"])..      
+0000f8c0: 2020 2020 2020 7365 6c66 2e65 6469 7453        self.editS
+0000f8d0: 7562 6a65 6374 2e73 6574 5465 7874 2864  ubject.setText(d
+0000f8e0: 6174 615b 2273 7562 6a65 6374 225d 290d  ata["subject"]).
+0000f8f0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+0000f900: 656c 662e 6472 6177 6361 6e76 6173 2e68  elf.drawcanvas.h
+0000f910: 6967 686c 6967 6874 5f63 6f6e 6e65 6374  ighlight_connect
+0000f920: 6f72 2864 6174 615b 2273 686f 7274 6e61  or(data["shortna
+0000f930: 6d65 225d 290d 0a0d 0a20 2020 2020 2020  me"])....       
+0000f940: 2020 2020 2069 6620 2264 6573 6372 6970       if "descrip
+0000f950: 7469 6f6e 2220 696e 2064 6174 613a 0d0a  tion" in data:..
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 7365 6c66 2e65 6469 7444 6573 6372 6970  self.editDescrip
+0000f980: 7469 6f6e 2e73 6574 5465 7874 2864 6174  tion.setText(dat
+0000f990: 615b 2264 6573 6372 6970 7469 6f6e 225d  a["description"]
+0000f9a0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000f9b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000f9c0: 2020 2020 2020 7365 6c66 2e65 6469 7444        self.editD
+0000f9d0: 6573 6372 6970 7469 6f6e 2e73 6574 5465  escription.setTe
+0000f9e0: 7874 2822 2229 0d0a 2020 2020 2020 2020  xt("")..        
+0000f9f0: 2020 2020 7365 6c66 2e65 6469 7453 686f      self.editSho
+0000fa00: 7274 6e61 6d65 2e73 6574 5465 7874 2864  rtname.setText(d
+0000fa10: 6174 615b 2273 686f 7274 6e61 6d65 225d  ata["shortname"]
+0000fa20: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000fa30: 2075 6e69 6469 7220 3d20 7374 7228 6461   unidir = str(da
+0000fa40: 7461 5b22 756e 692d 6469 7265 6374 696f  ta["uni-directio
+0000fa50: 6e61 6c22 5d29 206f 7220 224e 6f6e 6522  nal"]) or "None"
+0000fa60: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000fa70: 6c66 2e63 6f6d 626f 556e 6964 6972 2e73  lf.comboUnidir.s
+0000fa80: 6574 4375 7272 656e 7449 6e64 6578 2873  etCurrentIndex(s
+0000fa90: 656c 662e 636f 6d62 6f55 6e69 6469 722e  elf.comboUnidir.
+0000faa0: 6669 6e64 5465 7874 2875 6e69 6469 7229  findText(unidir)
+0000fab0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
+0000fac0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+0000fad0: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
+0000fae0: 2073 656c 662e 6e6f 7469 6679 2873 7472   self.notify(str
+0000faf0: 2865 292c 7469 746c 653d 2245 7272 6f72  (e),title="Error
+0000fb00: 2229 0d0a 0d0a 2020 2020 2020 2020 7365  ")....        se
+0000fb10: 6c66 2e6d 6164 655f 6368 616e 6765 7320  lf.made_changes 
+0000fb20: 3d20 4661 6c73 650d 0a0d 0a20 2020 2064  = False....    d
+0000fb30: 6566 2075 7064 6174 655f 6461 7461 2873  ef update_data(s
+0000fb40: 656c 6629 3a0d 0a20 2020 2020 2020 2069  elf):..        i
+0000fb50: 6620 7365 6c66 2e73 656c 6563 7469 6f6e  f self.selection
+0000fb60: 5f69 6478 2069 7320 4e6f 6e65 3a0d 0a20  _idx is None:.. 
+0000fb70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fb80: 6e0d 0a0d 0a20 2020 2020 2020 2073 656c  n....        sel
+0000fb90: 662e 656e 7472 795f 6461 7461 5b73 656c  f.entry_data[sel
+0000fba0: 662e 7365 6c65 6374 696f 6e5f 6964 785d  f.selection_idx]
+0000fbb0: 5b22 6131 225d 203d 2073 656c 662e 4173  ["a1"] = self.As
+0000fbc0: 7365 744c 6973 744c 6566 742e 746f 506c  setListLeft.toPl
+0000fbd0: 6169 6e54 6578 7428 290d 0a20 2020 2020  ainText()..     
+0000fbe0: 2020 2073 656c 662e 656e 7472 795f 6461     self.entry_da
+0000fbf0: 7461 5b73 656c 662e 7365 6c65 6374 696f  ta[self.selectio
+0000fc00: 6e5f 6964 785d 5b22 6132 225d 203d 2073  n_idx]["a2"] = s
+0000fc10: 656c 662e 4173 7365 744c 6973 7452 6967  elf.AssetListRig
+0000fc20: 6874 2e74 6f50 6c61 696e 5465 7874 2829  ht.toPlainText()
+0000fc30: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+0000fc40: 6e74 7279 5f64 6174 615b 7365 6c66 2e73  ntry_data[self.s
+0000fc50: 656c 6563 7469 6f6e 5f69 6478 5d5b 226c  election_idx]["l
+0000fc60: 3122 5d20 3d20 7365 6c66 2e4c 6961 6269  1"] = self.Liabi
+0000fc70: 6c69 7479 4c69 7374 4c65 6674 2e74 6f50  lityListLeft.toP
+0000fc80: 6c61 696e 5465 7874 2829 0d0a 2020 2020  lainText()..    
+0000fc90: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
+0000fca0: 6174 615b 7365 6c66 2e73 656c 6563 7469  ata[self.selecti
+0000fcb0: 6f6e 5f69 6478 5d5b 226c 3222 5d20 3d20  on_idx]["l2"] = 
+0000fcc0: 7365 6c66 2e4c 6961 6269 6c69 7479 4c69  self.LiabilityLi
+0000fcd0: 7374 5269 6768 742e 746f 506c 6169 6e54  stRight.toPlainT
+0000fce0: 6578 7428 290d 0a20 2020 2020 2020 2073  ext()..        s
+0000fcf0: 656c 662e 656e 7472 795f 6461 7461 5b73  elf.entry_data[s
+0000fd00: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
+0000fd10: 785d 5b22 6531 225d 203d 2073 656c 662e  x]["e1"] = self.
+0000fd20: 4571 7569 7479 4c69 7374 4c65 6674 2e74  EquityListLeft.t
+0000fd30: 6f50 6c61 696e 5465 7874 2829 0d0a 2020  oPlainText()..  
+0000fd40: 2020 2020 2020 7365 6c66 2e65 6e74 7279        self.entry
+0000fd50: 5f64 6174 615b 7365 6c66 2e73 656c 6563  _data[self.selec
+0000fd60: 7469 6f6e 5f69 6478 5d5b 2265 3222 5d20  tion_idx]["e2"] 
+0000fd70: 3d20 7365 6c66 2e45 7175 6974 794c 6973  = self.EquityLis
+0000fd80: 7452 6967 6874 2e74 6f50 6c61 696e 5465  tRight.toPlainTe
+0000fd90: 7874 2829 0d0a 0d0a 2020 2020 2020 2020  xt()....        
+0000fda0: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
+0000fdb0: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
+0000fdc0: 6478 5d5b 2261 3122 5d20 203d 2073 656c  dx]["a1"]  = sel
+0000fdd0: 662e 4173 7365 744c 6973 744c 6566 742e  f.AssetListLeft.
+0000fde0: 746f 506c 6169 6e54 6578 7428 290d 0a20  toPlainText().. 
+0000fdf0: 2020 2020 2020 2073 656c 662e 656e 7472         self.entr
+0000fe00: 795f 6461 7461 5b73 656c 662e 7365 6c65  y_data[self.sele
+0000fe10: 6374 696f 6e5f 6964 785d 5b22 6132 225d  ction_idx]["a2"]
+0000fe20: 203d 2073 656c 662e 4173 7365 744c 6973   = self.AssetLis
+0000fe30: 7452 6967 6874 2e74 6f50 6c61 696e 5465  tRight.toPlainTe
+0000fe40: 7874 2829 0d0a 2020 2020 2020 2020 7365  xt()..        se
+0000fe50: 6c66 2e65 6e74 7279 5f64 6174 615b 7365  lf.entry_data[se
+0000fe60: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
+0000fe70: 5d5b 226c 3122 5d20 203d 2073 656c 662e  ]["l1"]  = self.
+0000fe80: 4c69 6162 696c 6974 794c 6973 744c 6566  LiabilityListLef
+0000fe90: 742e 746f 506c 6169 6e54 6578 7428 290d  t.toPlainText().
+0000fea0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+0000feb0: 7472 795f 6461 7461 5b73 656c 662e 7365  try_data[self.se
+0000fec0: 6c65 6374 696f 6e5f 6964 785d 5b22 6c32  lection_idx]["l2
+0000fed0: 225d 2020 3d20 7365 6c66 2e4c 6961 6269  "]  = self.Liabi
+0000fee0: 6c69 7479 4c69 7374 5269 6768 742e 746f  lityListRight.to
+0000fef0: 506c 6169 6e54 6578 7428 290d 0a20 2020  PlainText()..   
+0000ff00: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
+0000ff10: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
+0000ff20: 696f 6e5f 6964 785d 5b22 6531 225d 2020  ion_idx]["e1"]  
+0000ff30: 3d20 7365 6c66 2e45 7175 6974 794c 6973  = self.EquityLis
+0000ff40: 744c 6566 742e 746f 506c 6169 6e54 6578  tLeft.toPlainTex
+0000ff50: 7428 290d 0a20 2020 2020 2020 2073 656c  t()..        sel
+0000ff60: 662e 656e 7472 795f 6461 7461 5b73 656c  f.entry_data[sel
+0000ff70: 662e 7365 6c65 6374 696f 6e5f 6964 785d  f.selection_idx]
+0000ff80: 5b22 6532 225d 2020 3d20 7365 6c66 2e45  ["e2"]  = self.E
+0000ff90: 7175 6974 794c 6973 7452 6967 6874 2e74  quityListRight.t
+0000ffa0: 6f50 6c61 696e 5465 7874 2829 0d0a 0d0a  oPlainText()....
+0000ffb0: 2020 2020 2020 2020 6f6e 6c79 5f72 656e          only_ren
+0000ffc0: 616d 6520 3d20 5472 7565 0d0a 2020 2020  ame = True..    
+0000ffd0: 2020 2020 6966 2073 656c 662e 656e 7472      if self.entr
+0000ffe0: 795f 6461 7461 5b73 656c 662e 7365 6c65  y_data[self.sele
+0000fff0: 6374 696f 6e5f 6964 785d 5b22 6167 656e  ction_idx]["agen
+00010000: 7431 225d 2020 213d 2073 656c 662e 6167  t1"]  != self.ag
+00010010: 656e 7431 4564 6974 2e74 6578 7428 293a  ent1Edit.text():
+00010020: 0d0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
+00010030: 6c79 5f72 656e 616d 6520 3d20 4661 6c73  ly_rename = Fals
+00010040: 650d 0a20 2020 2020 2020 2069 6620 7365  e..        if se
+00010050: 6c66 2e65 6e74 7279 5f64 6174 615b 7365  lf.entry_data[se
+00010060: 6c66 2e73 656c 6563 7469 6f6e 5f69 6478  lf.selection_idx
+00010070: 5d5b 2261 6765 6e74 3222 5d20 2021 3d73  ]["agent2"]  !=s
+00010080: 656c 662e 6167 656e 7432 4564 6974 2e74  elf.agent2Edit.t
+00010090: 6578 7428 293a 0d0a 2020 2020 2020 2020  ext():..        
+000100a0: 2020 2020 6f6e 6c79 5f72 656e 616d 6520      only_rename 
+000100b0: 3d20 4661 6c73 650d 0a0d 0a0d 0a20 2020  = False......   
+000100c0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+000100d0: 2e64 7261 7763 616e 7661 732e 6368 6563  .drawcanvas.chec
+000100e0: 6b5f 6578 6973 7428 7365 6c66 2e61 6765  k_exist(self.age
+000100f0: 6e74 3145 6469 742e 7465 7874 2829 293a  nt1Edit.text()):
+00010100: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00010110: 2073 656c 662e 6167 656e 7431 4564 6974   self.agent1Edit
+00010120: 2e74 6578 7428 292e 7374 7269 7028 2920  .text().strip() 
+00010130: 213d 2022 223a 0d0a 2020 2020 2020 2020  != "":..        
+00010140: 2020 2020 2020 2020 7965 7320 3d20 7365          yes = se
+00010150: 6c66 2e61 736b 5f71 7565 7374 696f 6e28  lf.ask_question(
+00010160: 2727 2c22 5468 6520 6167 656e 7420 2573  '',"The agent %s
+00010170: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
+00010180: 5c6e 446f 2079 6f75 2077 6973 6820 746f  \nDo you wish to
+00010190: 2063 6f6e 7469 6e75 6520 616e 6420 6175   continue and au
+000101a0: 746f 6d61 7469 6361 6c6c 7920 6372 6561  tomatically crea
+000101b0: 7465 2061 206e 6577 2061 6765 6e74 3f22  te a new agent?"
+000101c0: 2573 656c 662e 6167 656e 7431 4564 6974  %self.agent1Edit
+000101d0: 2e74 6578 7428 2929 0d0a 2020 2020 2020  .text())..      
+000101e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000101f0: 2079 6573 3a0d 0a20 2020 2020 2020 2020   yes:..         
+00010200: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010210: 6e0d 0a0d 0a20 2020 2020 2020 2069 6620  n....        if 
+00010220: 6e6f 7420 7365 6c66 2e64 7261 7763 616e  not self.drawcan
+00010230: 7661 732e 6368 6563 6b5f 6578 6973 7428  vas.check_exist(
+00010240: 7365 6c66 2e61 6765 6e74 3245 6469 742e  self.agent2Edit.
+00010250: 7465 7874 2829 293a 0d0a 2020 2020 2020  text()):..      
+00010260: 2020 2020 2020 6966 2073 656c 662e 6167        if self.ag
+00010270: 656e 7432 4564 6974 2e74 6578 7428 292e  ent2Edit.text().
+00010280: 7374 7269 7028 2920 213d 2022 223a 0d0a  strip() != "":..
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 7965 7320 3d20 7365 6c66 2e61 736b 5f71  yes = self.ask_q
+000102b0: 7565 7374 696f 6e28 2727 2c22 5468 6520  uestion('',"The 
+000102c0: 6167 656e 7420 2573 2064 6f65 7320 6e6f  agent %s does no
+000102d0: 7420 6578 6973 742e 5c6e 446f 2079 6f75  t exist.\nDo you
+000102e0: 2077 6973 6820 746f 2063 6f6e 7469 6e75   wish to continu
+000102f0: 6520 616e 6420 6175 746f 6d61 7469 6361  e and automatica
+00010300: 6c6c 7920 6372 6561 7465 2061 206e 6577  lly create a new
+00010310: 2061 6765 6e74 3f22 2573 656c 662e 6167   agent?"%self.ag
+00010320: 656e 7432 4564 6974 2e74 6578 7428 2929  ent2Edit.text())
+00010330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010340: 2020 6966 206e 6f74 2079 6573 3a0d 0a20    if not yes:.. 
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+00010370: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
+00010380: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
+00010390: 696f 6e5f 6964 785d 5b22 6167 656e 7431  ion_idx]["agent1
+000103a0: 225d 2020 3d20 6361 6d65 6c28 7365 6c66  "]  = camel(self
+000103b0: 2e61 6765 6e74 3145 6469 742e 7465 7874  .agent1Edit.text
+000103c0: 2829 2920 232e 6361 7069 7461 6c69 7a65  ()) #.capitalize
+000103d0: 2829 2023 2075 7070 6572 2062 6563 6175  () # upper becau
+000103e0: 7365 2061 6765 6e74 7320 6172 6520 616c  se agents are al
+000103f0: 7761 7973 2075 7070 6572 6361 7365 0d0a  ways uppercase..
+00010400: 2020 2020 2020 2020 7365 6c66 2e65 6e74          self.ent
+00010410: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
+00010420: 6563 7469 6f6e 5f69 6478 5d5b 2261 6765  ection_idx]["age
+00010430: 6e74 3222 5d20 203d 2063 616d 656c 2873  nt2"]  = camel(s
+00010440: 656c 662e 6167 656e 7432 4564 6974 2e74  elf.agent2Edit.t
+00010450: 6578 7428 2929 2023 2e63 6170 6974 616c  ext()) #.capital
+00010460: 697a 6528 290d 0a0d 0a20 2020 2020 2020  ize()....       
+00010470: 2073 656c 662e 6167 656e 7431 4564 6974   self.agent1Edit
+00010480: 2e73 6574 5465 7874 2863 616d 656c 2873  .setText(camel(s
+00010490: 656c 662e 6167 656e 7431 4564 6974 2e74  elf.agent1Edit.t
+000104a0: 6578 7428 2929 2920 232e 6361 7069 7461  ext())) #.capita
+000104b0: 6c69 7a65 2829 290d 0a20 2020 2020 2020  lize())..       
+000104c0: 2073 656c 662e 6167 656e 7432 4564 6974   self.agent2Edit
+000104d0: 2e73 6574 5465 7874 2863 616d 656c 2873  .setText(camel(s
+000104e0: 656c 662e 6167 656e 7432 4564 6974 2e74  elf.agent2Edit.t
+000104f0: 6578 7428 2929 2920 232e 6361 7069 7461  ext())) #.capita
+00010500: 6c69 7a65 2829 290d 0a0d 0a20 2020 2020  lize())....     
+00010510: 2020 2073 656c 662e 656e 7472 795f 6461     self.entry_da
+00010520: 7461 5b73 656c 662e 7365 6c65 6374 696f  ta[self.selectio
+00010530: 6e5f 6964 785d 5b22 756e 692d 6469 7265  n_idx]["uni-dire
+00010540: 6374 696f 6e61 6c22 5d20 3d20 5c0d 0a20  ctional"] = \.. 
+00010550: 2020 2020 2020 2020 2020 2073 7472 2873             str(s
+00010560: 656c 662e 636f 6d62 6f55 6e69 6469 722e  elf.comboUnidir.
+00010570: 6375 7272 656e 7454 6578 7428 2929 0d0a  currentText())..
+00010580: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
+00010590: 6e74 7279 5f64 6174 615b 7365 6c66 2e73  ntry_data[self.s
+000105a0: 656c 6563 7469 6f6e 5f69 6478 5d5b 226c  election_idx]["l
+000105b0: 6f67 2074 7261 6e73 6163 7469 6f6e 225d  og transaction"]
+000105c0: 203d 5c0d 0a20 2020 2020 2020 2020 2020   =\..           
+000105d0: 2073 7472 2873 656c 662e 7265 6769 7374   str(self.regist
+000105e0: 6572 466c 6f77 426f 782e 6375 7272 656e  erFlowBox.curren
+000105f0: 7454 6578 7428 2929 0d0a 0d0a 2020 2020  tText())....    
+00010600: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
+00010610: 6174 615b 7365 6c66 2e73 656c 6563 7469  ata[self.selecti
+00010620: 6f6e 5f69 6478 5d5b 2263 6173 6866 6c6f  on_idx]["cashflo
+00010630: 7731 225d 203d 205c 0d0a 2020 2020 2020  w1"] = \..      
+00010640: 2020 2020 2020 7374 7228 7365 6c66 2e63        str(self.c
+00010650: 6f6d 626f 4361 7368 4c65 6674 2e63 7572  omboCashLeft.cur
+00010660: 7265 6e74 5465 7874 2829 290d 0a20 2020  rentText())..   
+00010670: 2020 2020 2073 656c 662e 656e 7472 795f       self.entry_
+00010680: 6461 7461 5b73 656c 662e 7365 6c65 6374  data[self.select
+00010690: 696f 6e5f 6964 785d 5b22 6361 7368 666c  ion_idx]["cashfl
+000106a0: 6f77 3222 5d20 3d20 5c0d 0a20 2020 2020  ow2"] = \..     
+000106b0: 2020 2020 2020 2073 7472 2873 656c 662e         str(self.
+000106c0: 636f 6d62 6f43 6173 6852 6967 6874 2e63  comboCashRight.c
+000106d0: 7572 7265 6e74 5465 7874 2829 290d 0a0d  urrentText())...
+000106e0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+000106f0: 7472 795f 6461 7461 5b73 656c 662e 7365  try_data[self.se
+00010700: 6c65 6374 696f 6e5f 6964 785d 5b22 6b69  lection_idx]["ki
+00010710: 6e64 225d 203d 205c 0d0a 2020 2020 2020  nd"] = \..      
+00010720: 2020 2020 2020 7374 7228 7365 6c66 2e65        str(self.e
+00010730: 6469 7454 7970 652e 6375 7272 656e 7454  ditType.currentT
+00010740: 6578 7428 2929 0d0a 0d0a 2020 2020 2020  ext())....      
+00010750: 2020 7365 6c66 2e65 6e74 7279 5f64 6174    self.entry_dat
+00010760: 615b 7365 6c66 2e73 656c 6563 7469 6f6e  a[self.selection
+00010770: 5f69 6478 5d5b 2269 6e63 6f6d 6531 225d  _idx]["income1"]
+00010780: 203d 205c 0d0a 2020 2020 2020 2020 2020   = \..          
+00010790: 2020 7374 7228 7365 6c66 2e63 6f6d 626f    str(self.combo
+000107a0: 496e 636f 6d65 4c65 6674 2e63 7572 7265  IncomeLeft.curre
+000107b0: 6e74 5465 7874 2829 290d 0a20 2020 2020  ntText())..     
+000107c0: 2020 2073 656c 662e 656e 7472 795f 6461     self.entry_da
+000107d0: 7461 5b73 656c 662e 7365 6c65 6374 696f  ta[self.selectio
+000107e0: 6e5f 6964 785d 5b22 696e 636f 6d65 3222  n_idx]["income2"
+000107f0: 5d20 3d20 5c0d 0a20 2020 2020 2020 2020  ] = \..         
+00010800: 2020 2073 7472 2873 656c 662e 636f 6d62     str(self.comb
+00010810: 6f49 6e63 6f6d 6552 6967 6874 2e63 7572  oIncomeRight.cur
+00010820: 7265 6e74 5465 7874 2829 290d 0a0d 0a0d  rentText()).....
+00010830: 0a20 2020 2020 2020 2069 6620 6f6e 6c79  .        if only
+00010840: 5f72 656e 616d 653a 0d0a 0d0a 2020 2020  _rename:....    
+00010850: 2020 2020 2020 2020 7365 6c66 2e64 7261          self.dra
+00010860: 7763 616e 7661 732e 7265 6e61 6d65 5f63  wcanvas.rename_c
+00010870: 6f6e 6e65 6374 696f 6e28 7365 6c66 2e65  onnection(self.e
+00010880: 6e74 7279 5f64 6174 615b 7365 6c66 2e73  ntry_data[self.s
+00010890: 656c 6563 7469 6f6e 5f69 6478 5d5b 2273  election_idx]["s
+000108a0: 686f 7274 6e61 6d65 225d 202c 2073 7472  hortname"] , str
+000108b0: 2873 656c 662e 6564 6974 5368 6f72 746e  (self.editShortn
+000108c0: 616d 652e 7465 7874 2829 2929 0d0a 0d0a  ame.text()))....
+000108d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000108e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000108f0: 6472 6177 6361 6e76 6173 2e72 656d 6f76  drawcanvas.remov
+00010900: 655f 636f 6e6e 6563 7469 6f6e 2873 656c  e_connection(sel
+00010910: 662e 656e 7472 795f 6461 7461 5b73 656c  f.entry_data[sel
+00010920: 662e 7365 6c65 6374 696f 6e5f 6964 785d  f.selection_idx]
+00010930: 5b22 7368 6f72 746e 616d 6522 5d29 2023  ["shortname"]) #
+00010940: 2c20 7374 7228 7365 6c66 2e65 6469 7453  , str(self.editS
+00010950: 7562 6a65 6374 2e74 6578 7428 2929 290d  ubject.text())).
+00010960: 0a0d 0a20 2020 2020 2020 2020 2020 2062  ...            b
+00010970: 6f78 3120 3d20 7365 6c66 2e64 7261 7763  ox1 = self.drawc
+00010980: 616e 7661 732e 6164 645f 6167 656e 7428  anvas.add_agent(
+00010990: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
+000109a0: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
+000109b0: 6478 5d5b 2261 6765 6e74 3122 5d29 0d0a  dx]["agent1"])..
+000109c0: 2020 2020 2020 2020 2020 2020 626f 7832              box2
+000109d0: 203d 2073 656c 662e 6472 6177 6361 6e76   = self.drawcanv
+000109e0: 6173 2e61 6464 5f61 6765 6e74 2873 656c  as.add_agent(sel
+000109f0: 662e 656e 7472 795f 6461 7461 5b73 656c  f.entry_data[sel
+00010a00: 662e 7365 6c65 6374 696f 6e5f 6964 785d  f.selection_idx]
+00010a10: 5b22 6167 656e 7432 225d 290d 0a0d 0a0d  ["agent2"]).....
+00010a20: 0a20 2020 2020 2020 2020 2020 206d 795f  .            my_
+00010a30: 6974 656d 7320 3d20 5b5d 0d0a 2020 2020  items = []..    
+00010a40: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
+00010a50: 656c 662e 656e 7472 795f 6461 7461 5b73  elf.entry_data[s
+00010a60: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
+00010a70: 785d 0d0a 0d0a 2020 2020 2020 2020 2020  x]....          
+00010a80: 2020 616c 6c65 6e74 7269 6573 203d 2022    allentries = "
+00010a90: 5c6e 222e 6a6f 696e 285b 6461 7461 5b22  \n".join([data["
+00010aa0: 6c31 225d 2c20 6461 7461 5b22 6131 225d  l1"], data["a1"]
+00010ab0: 2c20 6461 7461 5b22 6531 225d 2c20 6461  , data["e1"], da
+00010ac0: 7461 5b22 6c32 225d 2c20 6461 7461 5b22  ta["l2"], data["
+00010ad0: 6132 225d 2c20 6461 7461 5b22 6532 225d  a2"], data["e2"]
+00010ae0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00010af0: 666f 7220 7375 625f 6974 656d 2069 6e20  for sub_item in 
+00010b00: 616c 6c65 6e74 7269 6573 2e73 706c 6974  allentries.split
+00010b10: 2822 5c6e 2229 3a0d 0a20 2020 2020 2020  ("\n"):..       
+00010b20: 2020 2020 2020 2020 2066 6f72 2073 7562           for sub
+00010b30: 5f65 6e74 7279 2069 6e20 7375 625f 6974  _entry in sub_it
+00010b40: 656d 2e73 706c 6974 2822 5c6e 2229 3a0d  em.split("\n"):.
+00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b60: 2020 2020 2065 6e74 7279 203d 2073 7562       entry = sub
+00010b70: 5f65 6e74 7279 2e72 6570 6c61 6365 2822  _entry.replace("
+00010b80: 2d22 2c22 2229 2e72 6570 6c61 6365 2822  -","").replace("
+00010b90: 2b22 2c22 2229 2e73 7472 6970 2829 0d0a  +","").strip()..
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bb0: 2020 2020 6966 2065 6e74 7279 2021 3d20      if entry != 
+00010bc0: 2022 223a 0d0a 2020 2020 2020 2020 2020   "":..          
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 6d79                my
+00010be0: 5f69 7465 6d73 2e61 7070 656e 6428 656e  _items.append(en
+00010bf0: 7472 7929 0d0a 0d0a 0d0a 2020 2020 2020  try)......      
+00010c00: 2020 2020 2020 7365 6c66 2e64 7261 7763        self.drawc
+00010c10: 616e 7661 732e 6164 645f 636f 6e6e 6563  anvas.add_connec
+00010c20: 7469 6f6e 2862 6f78 312c 626f 7832 2c20  tion(box1,box2, 
+00010c30: 7374 7228 7365 6c66 2e65 6469 7453 686f  str(self.editSho
+00010c40: 7274 6e61 6d65 2e74 6578 7428 2929 2c73  rtname.text()),s
+00010c50: 7562 6a65 6374 3d73 656c 662e 6564 6974  ubject=self.edit
+00010c60: 5375 626a 6563 742e 7465 7874 2829 2c69  Subject.text(),i
+00010c70: 7465 6d73 3d6d 795f 6974 656d 7329 0d0a  tems=my_items)..
+00010c80: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00010c90: 2e65 6e74 7279 5f64 6174 615b 7365 6c66  .entry_data[self
+00010ca0: 2e73 656c 6563 7469 6f6e 5f69 6478 5d5b  .selection_idx][
+00010cb0: 2271 7561 6e74 6974 7922 5d20 3d20 5c0d  "quantity"] = \.
+00010cc0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00010cd0: 2873 656c 662e 6564 6974 5175 616e 7469  (self.editQuanti
+00010ce0: 7479 2e74 6578 7428 2929 0d0a 0d0a 0d0a  ty.text())......
+00010cf0: 2020 2020 2020 2020 7365 6c66 2e65 6e74          self.ent
+00010d00: 7279 5f64 6174 615b 7365 6c66 2e73 656c  ry_data[self.sel
+00010d10: 6563 7469 6f6e 5f69 6478 5d5b 2273 7562  ection_idx]["sub
+00010d20: 6a65 6374 225d 203d 205c 0d0a 2020 2020  ject"] = \..    
+00010d30: 2020 2020 2020 2020 7374 7228 7365 6c66          str(self
+00010d40: 2e65 6469 7453 7562 6a65 6374 2e74 6578  .editSubject.tex
+00010d50: 7428 2929 0d0a 0d0a 2020 2020 2020 2020  t())....        
+00010d60: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
+00010d70: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
+00010d80: 6478 5d5b 2273 686f 7274 6e61 6d65 225d  dx]["shortname"]
+00010d90: 203d 205c 0d0a 2020 2020 2020 2020 2020   = \..          
+00010da0: 2020 7374 7228 7365 6c66 2e65 6469 7453    str(self.editS
+00010db0: 686f 7274 6e61 6d65 2e74 6578 7428 2929  hortname.text())
+00010dc0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00010dd0: 2e65 6e74 7279 5f64 6174 615b 7365 6c66  .entry_data[self
+00010de0: 2e73 656c 6563 7469 6f6e 5f69 6478 5d5b  .selection_idx][
+00010df0: 2264 6573 6372 6970 7469 6f6e 225d 203d  "description"] =
+00010e00: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00010e10: 7374 7228 7365 6c66 2e65 6469 7444 6573  str(self.editDes
+00010e20: 6372 6970 7469 6f6e 2e74 6578 7428 2929  cription.text())
+00010e30: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00010e40: 2e75 7064 6174 655f 7461 626c 6528 290d  .update_table().
+00010e50: 0a0d 0a20 2020 2020 2020 2070 7269 6e74  ...        print
+00010e60: 2822 6461 7461 2063 6861 6e67 6564 2e22  ("data changed."
+00010e70: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+00010e80: 662e 6d61 6465 5f63 6861 6e67 6573 203d  f.made_changes =
+00010e90: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
+00010ea0: 2020 7365 6c66 2e72 6f77 5f73 656c 6563    self.row_selec
+00010eb0: 7428 7365 6c66 2e73 656c 6563 7469 6f6e  t(self.selection
+00010ec0: 5f69 6478 290d 0a0d 0a20 2020 2020 2020  _idx)....       
+00010ed0: 2023 2073 656c 662e 7564 7061 7465 4275   # self.udpateBu
+00010ee0: 7474 6f6e 2e73 6574 5465 7874 2822 5570  tton.setText("Up
+00010ef0: 6461 7465 2056 616c 7565 7322 290d 0a0d  date Values")...
+00010f00: 0a20 2020 2064 6566 2073 6176 6528 7365  .    def save(se
+00010f10: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
+00010f20: 7472 793a 0d0a 0d0a 0d0a 2020 2020 2020  try:......      
+00010f30: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
+00010f40: 2073 656c 662e 6375 7272 656e 745f 6669   self.current_fi
+00010f50: 6c65 2023 2073 7461 7475 7342 6172 2829  le # statusBar()
+00010f60: 2e63 7572 7265 6e74 4d65 7373 6167 6528  .currentMessage(
+00010f70: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00010f80: 656c 662e 6c61 6265 6c5f 666e 616d 652e  elf.label_fname.
+00010f90: 7365 7454 6578 7428 6669 6c65 6e61 6d65  setText(filename
+00010fa0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00010fb0: 2069 6620 6669 6c65 6e61 6d65 2069 7320   if filename is 
+00010fc0: 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20 2020  not None:....   
+00010fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010fe0: 662e 7361 7665 6173 2866 696c 656e 616d  f.saveas(filenam
+00010ff0: 6529 0d0a 0d0a 2020 2020 2020 2020 2020  e)....          
+00011000: 2020 2020 2020 2320 544f 444f 206d 6179        # TODO may
+00011010: 6265 2062 6163 6b75 7028 3f29 0d0a 2020  be backup(?)..  
+00011020: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011030: 7365 6c66 2e6e 6f74 6966 7928 2246 696c  self.notify("Fil
+00011040: 6520 7361 7665 6420 756e 6465 7220 2573  e saved under %s
+00011050: 2220 2520 6669 6c65 6e61 6d65 2c74 6974  " % filename,tit
+00011060: 6c65 3d22 4f6b 2229 0d0a 2020 2020 2020  le="Ok")..      
+00011070: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00011080: 2246 494c 4520 5341 5645 4421 2229 0d0a  "FILE SAVED!")..
+00011090: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000110a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000110b0: 2020 2073 656c 662e 7361 7665 5f64 6c67     self.save_dlg
+000110c0: 2829 0d0a 0d0a 2020 2020 2020 2020 6578  ()....        ex
+000110d0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+000110e0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+000110f0: 2020 6966 2066 696c 656e 616d 6520 213d    if filename !=
+00011100: 2022 223a 0d0a 2020 2020 2020 2020 2020   "":..          
+00011110: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+00011120: 7928 7374 7228 6529 2c74 6974 6c65 3d22  y(str(e),title="
+00011130: 4572 726f 7222 290d 0a0d 0a0d 0a0d 0a20  Error")........ 
+00011140: 2020 2064 6566 2073 6176 655f 646c 6728     def save_dlg(
+00011150: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00011160: 7472 793a 0d0a 0d0a 2020 2020 2020 2020  try:....        
+00011170: 2020 2020 6669 6c65 6e61 6d65 203d 2051      filename = Q
+00011180: 4669 6c65 4469 616c 6f67 2e67 6574 5361  FileDialog.getSa
+00011190: 7665 4669 6c65 4e61 6d65 2873 656c 662c  veFileName(self,
+000111a0: 2027 5361 7665 2066 696c 6527 2c0d 0a20   'Save file',.. 
+000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+000111e0: 2e67 6574 6377 6428 292c 2022 6174 7475  .getcwd(), "attu
+000111f0: 6e65 2046 696c 6573 2028 2a2e 7366 6374  ne Files (*.sfct
+00011200: 6c29 2229 5b30 5d0d 0a20 2020 2020 2020  l)")[0]..       
+00011210: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00011220: 4261 7228 292e 7368 6f77 4d65 7373 6167  Bar().showMessag
+00011230: 6528 2253 6176 6564 2066 696c 6520 2220  e("Saved file " 
+00011240: 2b20 6669 6c65 6e61 6d65 290d 0a0d 0a20  + filename).... 
+00011250: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00011260: 6e74 5f66 696c 655f 6261 636b 7570 203d  nt_file_backup =
+00011270: 2073 656c 662e 6375 7272 656e 745f 6669   self.current_fi
+00011280: 6c65 0d0a 0d0a 2020 2020 2020 2020 2020  le....          
+00011290: 2020 6966 2066 696c 656e 616d 6520 6973    if filename is
+000112a0: 206e 6f74 204e 6f6e 6520 616e 6420 6669   not None and fi
+000112b0: 6c65 6e61 6d65 2021 3d20 2222 3a0d 0a20  lename != "":.. 
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000112d0: 656c 662e 6c61 6265 6c5f 666e 616d 652e  elf.label_fname.
+000112e0: 7365 7454 6578 7428 6669 6c65 6e61 6d65  setText(filename
+000112f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00011300: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
+00011310: 745f 6669 6c65 203d 2066 696c 656e 616d  t_file = filenam
+00011320: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00011330: 2020 2073 656c 662e 7361 7665 6173 2866     self.saveas(f
+00011340: 696c 656e 616d 6529 0d0a 0d0a 2020 2020  ilename)....    
+00011350: 2020 2020 2020 2020 2320 544f 444f 206d          # TODO m
+00011360: 6179 6265 2062 6163 6b75 7028 3f29 0d0a  aybe backup(?)..
+00011370: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00011380: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00011390: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000113a0: 6c66 2e6e 6f74 6966 7928 2243 6f75 6c64  lf.notify("Could
+000113b0: 206e 6f74 2073 6176 6520 7072 6f6a 6563   not save projec
+000113c0: 742e 222c 7469 746c 653d 2245 7272 6f72  t.",title="Error
+000113d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000113e0: 7365 6c66 2e63 7572 7265 6e74 5f66 696c  self.current_fil
+000113f0: 6520 3d20 6375 7272 656e 745f 6669 6c65  e = current_file
+00011400: 5f62 6163 6b75 700d 0a0d 0a0d 0a20 2020  _backup......   
+00011410: 2064 6566 2067 6574 5f6f 7074 696f 6e73   def get_options
+00011420: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00011430: 206f 3120 3d20 7374 7228 7365 6c66 2e63   o1 = str(self.c
+00011440: 6865 636b 426f 785f 322e 6973 4368 6563  heckBox_2.isChec
+00011450: 6b65 6428 2929 0d0a 2020 2020 2020 2020  ked())..        
+00011460: 6f32 203d 2073 7472 2873 656c 662e 6368  o2 = str(self.ch
+00011470: 6563 6b42 6f78 2e69 7343 6865 636b 6564  eckBox.isChecked
+00011480: 2829 290d 0a20 2020 2020 2020 206f 3320  ())..        o3 
+00011490: 3d20 7374 7228 7365 6c66 2e63 6865 636b  = str(self.check
+000114a0: 426f 785f 342e 6973 4368 6563 6b65 6428  Box_4.isChecked(
+000114b0: 2929 0d0a 2020 2020 2020 2020 6f34 203d  ))..        o4 =
+000114c0: 2073 7472 2873 656c 662e 6368 6563 6b42   str(self.checkB
+000114d0: 6f78 5f35 2e69 7343 6865 636b 6564 2829  ox_5.isChecked()
+000114e0: 290d 0a20 2020 2020 2020 206f 3520 3d20  )..        o5 = 
+000114f0: 7374 7228 7365 6c66 2e63 6865 636b 426f  str(self.checkBo
+00011500: 785f 332e 6973 4368 6563 6b65 6428 2929  x_3.isChecked())
+00011510: 0d0a 2020 2020 2020 2020 6f36 203d 2073  ..        o6 = s
+00011520: 7472 2873 656c 662e 6368 6563 6b42 6f78  tr(self.checkBox
+00011530: 5f36 2e69 7343 6865 636b 6564 2829 290d  _6.isChecked()).
+00011540: 0a20 2020 2020 2020 206f 3720 3d20 7374  .        o7 = st
+00011550: 7228 7365 6c66 2e63 6865 636b 426f 785f  r(self.checkBox_
+00011560: 382e 6973 4368 6563 6b65 6428 2929 0d0a  8.isChecked())..
+00011570: 2020 2020 2020 2020 6f38 203d 2073 7472          o8 = str
+00011580: 2873 656c 662e 6368 6563 6b42 6f78 5f39  (self.checkBox_9
+00011590: 2e69 7343 6865 636b 6564 2829 290d 0a20  .isChecked()).. 
+000115a0: 2020 2020 2020 206f 3920 3d20 7374 7228         o9 = str(
+000115b0: 7365 6c66 2e63 6865 636b 426f 785f 7261  self.checkBox_ra
+000115c0: 7374 6572 2e69 7343 6865 636b 6564 2829  ster.isChecked()
+000115d0: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
+000115e0: 7572 6e20 5b6f 312c 6f32 2c6f 332c 6f34  urn [o1,o2,o3,o4
+000115f0: 2c6f 352c 6f36 2c6f 372c 6f38 2c6f 395d  ,o5,o6,o7,o8,o9]
+00011600: 0d0a 0d0a 2020 2020 6465 6620 7365 745f  ....    def set_
+00011610: 6f70 7469 6f6e 7328 7365 6c66 2c6e 6577  options(self,new
+00011620: 5f6f 7074 696f 6e73 293a 0d0a 2020 2020  _options):..    
+00011630: 2020 2020 2320 7365 7420 6469 7370 6c61      # set displa
+00011640: 7920 6f70 7469 6f6e 730d 0a20 2020 2020  y options..     
+00011650: 2020 2069 6620 6e65 775f 6f70 7469 6f6e     if new_option
+00011660: 7320 6973 204e 6f6e 653a 0d0a 2020 2020  s is None:..    
+00011670: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00011680: 0d0a 2020 2020 2020 2020 6f31 2c6f 322c  ..        o1,o2,
+00011690: 6f33 2c6f 342c 6f35 2c6f 362c 6f37 2c6f  o3,o4,o5,o6,o7,o
+000116a0: 382c 6f39 203d 206e 6577 5f6f 7074 696f  8,o9 = new_optio
+000116b0: 6e73 0d0a 0d0a 2020 2020 2020 2020 6465  ns....        de
+000116c0: 6620 7374 725f 746f 5f62 6f6f 6c28 7829  f str_to_bool(x)
+000116d0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+000116e0: 6620 7820 3d3d 2022 5472 7565 223a 0d0a  f x == "True":..
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00011710: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011720: 4661 6c73 650d 0a0d 0a20 2020 2020 2020  False....       
+00011730: 2073 656c 662e 6368 6563 6b42 6f78 5f32   self.checkBox_2
+00011740: 2e73 6574 4368 6563 6b65 6428 7374 725f  .setChecked(str_
+00011750: 746f 5f62 6f6f 6c28 6f31 2929 0d0a 2020  to_bool(o1))..  
+00011760: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00011770: 426f 782e 7365 7443 6865 636b 6564 2873  Box.setChecked(s
+00011780: 7472 5f74 6f5f 626f 6f6c 286f 3229 290d  tr_to_bool(o2)).
+00011790: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+000117a0: 6563 6b42 6f78 5f34 2e73 6574 4368 6563  eckBox_4.setChec
+000117b0: 6b65 6428 7374 725f 746f 5f62 6f6f 6c28  ked(str_to_bool(
+000117c0: 6f33 2929 0d0a 2020 2020 2020 2020 7365  o3))..        se
+000117d0: 6c66 2e63 6865 636b 426f 785f 352e 7365  lf.checkBox_5.se
+000117e0: 7443 6865 636b 6564 2873 7472 5f74 6f5f  tChecked(str_to_
+000117f0: 626f 6f6c 286f 3429 290d 0a20 2020 2020  bool(o4))..     
+00011800: 2020 2073 656c 662e 6368 6563 6b42 6f78     self.checkBox
+00011810: 5f33 2e73 6574 4368 6563 6b65 6428 7374  _3.setChecked(st
+00011820: 725f 746f 5f62 6f6f 6c28 6f35 2929 0d0a  r_to_bool(o5))..
+00011830: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+00011840: 636b 426f 785f 362e 7365 7443 6865 636b  ckBox_6.setCheck
+00011850: 6564 2873 7472 5f74 6f5f 626f 6f6c 286f  ed(str_to_bool(o
+00011860: 3629 290d 0a20 2020 2020 2020 2073 656c  6))..        sel
+00011870: 662e 6368 6563 6b42 6f78 5f38 2e73 6574  f.checkBox_8.set
+00011880: 4368 6563 6b65 6428 7374 725f 746f 5f62  Checked(str_to_b
+00011890: 6f6f 6c28 6f37 2929 0d0a 2020 2020 2020  ool(o7))..      
+000118a0: 2020 7365 6c66 2e63 6865 636b 426f 785f    self.checkBox_
+000118b0: 392e 7365 7443 6865 636b 6564 2873 7472  9.setChecked(str
+000118c0: 5f74 6f5f 626f 6f6c 286f 3829 290d 0a20  _to_bool(o8)).. 
+000118d0: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+000118e0: 6b42 6f78 5f72 6173 7465 722e 7365 7443  kBox_raster.setC
+000118f0: 6865 636b 6564 2873 7472 5f74 6f5f 626f  hecked(str_to_bo
+00011900: 6f6c 286f 3929 290d 0a0d 0a0d 0a20 2020  ol(o9))......   
+00011910: 2064 6566 2073 6176 6561 7328 7365 6c66   def saveas(self
+00011920: 2c66 696c 656e 616d 6529 3a0d 0a0d 0a20  ,filename):.... 
+00011930: 2020 2020 2020 2066 7468 656d 6520 3d20         ftheme = 
+00011940: 4e6f 6e65 0d0a 2020 2020 2020 2020 7472  None..        tr
+00011950: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00011960: 6674 6865 6d65 203d 2066 696c 656e 616d  ftheme = filenam
+00011970: 655b 3a2d 355d 2b22 7366 6374 6865 6d65  e[:-5]+"sfctheme
+00011980: 2220 2320 6162 736f 6c75 7465 2066 696c  " # absolute fil
+00011990: 6520 7061 7468 0d0a 2020 2020 2020 2020  e path..        
+000119a0: 2020 2020 666f 6c64 6572 2c66 7468 656d      folder,fthem
+000119b0: 6520 3d20 6f73 2e70 6174 682e 7370 6c69  e = os.path.spli
+000119c0: 7428 6674 6865 6d65 2920 2320 636f 6e76  t(ftheme) # conv
+000119d0: 6572 7420 746f 2072 656c 6174 6976 6520  ert to relative 
+000119e0: 6669 6c65 2070 6174 680d 0a20 2020 2020  file path..     
+000119f0: 2020 2020 2020 2073 656c 662e 7468 656d         self.them
+00011a00: 655f 6d61 6e61 6765 722e 7361 7665 5f63  e_manager.save_c
+00011a10: 6f6c 6f72 7328 6674 6865 6d65 290d 0a20  olors(ftheme).. 
+00011a20: 2020 2020 2020 2065 7863 6570 743a 0d0a         except:..
+00011a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011a40: 2e6e 6f74 6966 7928 2243 6f75 6c64 206e  .notify("Could n
+00011a50: 6f74 2073 6176 6520 636f 6c6f 7220 7468  ot save color th
+00011a60: 656d 652e 2070 726f 6365 6564 696e 6720  eme. proceeding 
+00011a70: 7769 7468 6f75 7422 2c74 6974 6c65 3d22  without",title="
+00011a80: 4572 726f 7222 290d 0a0d 0a0d 0a20 2020  Error")......   
+00011a90: 2020 2020 2023 2064 7261 7763 616e 7661       # drawcanva
+00011aa0: 7320 636f 6465 5f64 6174 610d 0a20 2020  s code_data..   
+00011ab0: 2020 2020 2063 6f64 655f 6461 7461 203d       code_data =
+00011ac0: 207b 7d0d 0a20 2020 2020 2020 2066 6f72   {}..        for
+00011ad0: 206b 2c76 2069 6e20 7365 6c66 2e64 7261   k,v in self.dra
+00011ae0: 7763 616e 7661 732e 636f 6465 5f64 6174  wcanvas.code_dat
+00011af0: 612e 6974 656d 7328 293a 0d0a 2020 2020  a.items():..    
+00011b00: 2020 2020 2020 2020 636f 6465 5f64 6174          code_dat
+00011b10: 615b 6b5d 203d 2073 7472 2876 2e65 6e63  a[k] = str(v.enc
+00011b20: 6f64 6528 2275 7466 2d38 2229 2e64 6563  ode("utf-8").dec
+00011b30: 6f64 6528 2763 7031 3235 3227 2929 0d0a  ode('cp1252'))..
+00011b40: 2020 2020 2020 2020 2020 2020 2320 6669              # fi
+00011b50: 7820 736f 6d65 2070 6f74 656e 7469 616c  x some potential
+00011b60: 2065 6e63 6f64 696e 6720 6572 726f 7273   encoding errors
+00011b70: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
+00011b80: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00011b90: 696e 7428 2246 494c 454e 414d 4522 2c20  int("FILENAME", 
+00011ba0: 6669 6c65 6e61 6d65 290d 0a0d 0a20 2020  filename)....   
+00011bb0: 2020 2020 2020 2020 2023 206c 6f61 6420           # load 
+00011bc0: 656e 7472 6965 7320 696e 746f 2074 6865  entries into the
+00011bd0: 206c 6973 740d 0a20 2020 2020 2020 2020   list..         
+00011be0: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
+00011bf0: 656e 616d 652c 2027 7727 2920 6173 2073  ename, 'w') as s
+00011c00: 7472 6561 6d3a 0d0a 0d0a 2020 2020 2020  tream:....      
+00011c10: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00011c20: 207b 2274 7261 6e73 6163 7469 6f6e 7322   {"transactions"
+00011c30: 3a20 7365 6c66 2e65 6e74 7279 5f64 6174  : self.entry_dat
+00011c40: 612c 0d0a 2020 2020 2020 2020 2020 2020  a,..            
+00011c50: 2020 2020 2261 6765 6e74 7322 3a20 636f      "agents": co
+00011c60: 6465 5f64 6174 612c 0d0a 2020 2020 2020  de_data,..      
+00011c70: 2020 2020 2020 2020 2020 2262 6f78 5f70            "box_p
+00011c80: 6f73 6974 696f 6e73 223a 2073 656c 662e  ositions": self.
+00011c90: 6472 6177 6361 6e76 6173 2e62 6f78 5f70  drawcanvas.box_p
+00011ca0: 6f73 6974 696f 6e73 2829 2c0d 0a20 2020  ositions(),..   
+00011cb0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+00011cc0: 6265 6c5f 706f 7369 7469 6f6e 7322 3a20  bel_positions": 
+00011cd0: 7365 6c66 2e64 7261 7763 616e 7661 732e  self.drawcanvas.
+00011ce0: 6c61 6265 6c5f 706f 7369 7469 6f6e 7328  label_positions(
+00011cf0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00011d00: 2020 2020 2273 6574 7469 6e67 7322 3a20      "settings": 
+00011d10: 7365 6c66 2e73 6574 7469 6e67 735f 7374  self.settings_st
+00011d20: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00011d30: 2020 2020 226d 6169 6e6c 6f6f 7022 3a20      "mainloop": 
+00011d40: 7365 6c66 2e6d 6169 6e6c 6f6f 705f 7374  self.mainloop_st
+00011d50: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00011d60: 2020 2020 2274 6865 6d65 223a 207b 2267      "theme": {"g
+00011d70: 6c6f 6261 6c74 6865 6d65 223a 2073 656c  lobaltheme": sel
+00011d80: 662e 7468 656d 655f 6d61 6e61 6765 722e  f.theme_manager.
+00011d90: 7468 656d 652c 2022 636f 6c6f 7273 223a  theme, "colors":
+00011da0: 6674 6865 6d65 7d2c 0d0a 2020 2020 2020  ftheme},..      
+00011db0: 2020 2020 2020 2020 2020 226e 6f74 6573            "notes
+00011dc0: 223a 2073 656c 662e 6e6f 7465 7345 6469  ": self.notesEdi
+00011dd0: 742e 746f 506c 6169 6e54 6578 7428 292c  t.toPlainText(),
+00011de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011df0: 2020 226f 7074 696f 6e73 223a 2073 656c    "options": sel
+00011e00: 662e 6765 745f 6f70 7469 6f6e 7328 292c  f.get_options(),
+00011e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011e20: 2020 7d0d 0a0d 0a20 2020 2020 2020 2020    }....         
+00011e30: 2020 2020 2020 2079 616d 6c2e 6475 6d70         yaml.dump
+00011e40: 2864 6174 612c 7374 7265 616d 290d 0a0d  (data,stream)...
+00011e50: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00011e60: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+00011e70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011e80: 662e 6e6f 7469 6679 286d 6573 7361 6765  f.notify(message
+00011e90: 3d73 7472 2865 292c 2074 6974 6c65 3d22  =str(e), title="
+00011ea0: 4572 726f 7222 290d 0a0d 0a0d 0a20 2020  Error")......   
+00011eb0: 2064 6566 2074 7279 5f67 656e 5f6d 6174   def try_gen_mat
+00011ec0: 7269 7828 7365 6c66 293a 0d0a 2020 2020  rix(self):..    
+00011ed0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00011ee0: 2020 2020 2020 7365 6c66 2e67 656e 5f6d        self.gen_m
+00011ef0: 6174 7269 7828 290d 0a20 2020 2020 2020  atrix()..       
+00011f00: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00011f10: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+00011f20: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
+00011f30: 2822 4572 726f 7222 2c73 7472 2865 2929  ("Error",str(e))
+00011f40: 0d0a 0d0a 2020 2020 6465 6620 6765 6e5f  ....    def gen_
+00011f50: 6d61 7472 6978 2873 656c 662c 6d6f 6465  matrix(self,mode
+00011f60: 3d22 7374 616e 6461 7264 2229 3a0d 0a20  ="standard"):.. 
+00011f70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00011f80: 2020 2020 6765 6e65 7261 7465 2066 6c6f      generate flo
+00011f90: 7720 6d61 7472 6978 3a0d 0a0d 0a20 2020  w matrix:....   
+00011fa0: 2020 2020 203a 7061 7261 6d20 6d6f 6465       :param mode
+00011fb0: 3a20 7374 616e 6461 7264 2c65 7863 656c  : standard,excel
+00011fc0: 2c6c 6174 6578 0d0a 0d0a 2020 2020 2020  ,latex....      
+00011fd0: 2020 7374 616e 6461 7264 3a20 7368 6f77    standard: show
+00011fe0: 7320 6d61 7472 6978 2067 7261 7068 6963  s matrix graphic
+00011ff0: 616c 6c79 0d0a 2020 2020 2020 2020 6578  ally..        ex
+00012000: 6365 6c3a 2065 7870 6f72 7473 2061 6e20  cel: exports an 
+00012010: 6578 6365 6c20 6669 6c65 0d0a 2020 2020  excel file..    
+00012020: 2020 2020 6c61 7465 783a 206e 6f74 2079      latex: not y
+00012030: 6574 2073 7570 706f 7274 6564 204e 4f54  et supported NOT
+00012040: 2041 5641 494c 4142 4c45 2046 4f52 204e   AVAILABLE FOR N
+00012050: 4f57 0d0a 2020 2020 2020 2020 6874 6d6c  OW..        html
+00012060: 3a20 4e4f 5420 4156 4149 4c41 424c 4520  : NOT AVAILABLE 
+00012070: 464f 5220 4e4f 570d 0a20 2020 2020 2020  FOR NOW..       
+00012080: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00012090: 666c 6f77 5f64 6174 6120 3d20 7b7d 0d0a  flow_data = {}..
 000120a0: 0d0a 2020 2020 2020 2020 666c 6f77 5f64  ..        flow_d
-000120b0: 6174 615b 224b 4122 5d20 3d20 6465 6661  ata["KA"] = defa
+000120b0: 6174 615b 2243 4122 5d20 3d20 6465 6661  ata["CA"] = defa
 000120c0: 756c 7464 6963 7428 6c61 6d62 6461 3a20  ultdict(lambda: 
 000120d0: 6465 6661 756c 7464 6963 7428 6c69 7374  defaultdict(list
-000120e0: 2929 2020 2320 6361 7069 7461 6c20 6163  ))  # capital ac
-000120f0: 636f 756e 740d 0a0d 0a20 2020 2020 2020  count....       
-00012100: 2023 2066 6c6f 775f 6461 7461 5b4b 4120   # flow_data[KA 
-00012110: 6f72 2043 415d 5b73 7562 6a65 6374 5d5b  or CA][subject][
-00012120: 6167 656e 745d 0d0a 2020 2020 2020 2020  agent]..        
-00012130: 6966 206c 656e 2873 656c 662e 656e 7472  if len(self.entr
-00012140: 795f 6461 7461 2920 3d3d 2030 3a0d 0a20  y_data) == 0:.. 
-00012150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012160: 6e6f 7469 6679 286d 6573 7361 6765 3d22  notify(message="
-00012170: 4361 6e6e 6f74 2067 656e 6572 6174 6520  Cannot generate 
-00012180: 4d61 7472 6978 2e20 4861 7665 2079 6f75  Matrix. Have you
-00012190: 2073 6574 2075 7020 616e 7920 7472 616e   set up any tran
-000121a0: 7361 6374 696f 6e73 2079 6574 3f22 2c74  sactions yet?",t
-000121b0: 6974 6c65 3d22 4572 726f 7222 290d 0a20  itle="Error").. 
-000121c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000121d0: 6e0d 0a0d 0a20 2020 2020 2020 2074 7279  n....        try
-000121e0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-000121f0: 6f72 2066 696c 6564 6174 6120 696e 2073  or filedata in s
-00012200: 656c 662e 656e 7472 795f 6461 7461 3a0d  elf.entry_data:.
-00012210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 2022 2222 0d0a 2020 2020 2020 2020 2020   """..          
-00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012250: 2020 2020 2020 6576 616c 7561 7465 2074        evaluate t
-00012260: 7261 6e73 6163 7469 6f6e 2065 6e74 7269  ransaction entri
-00012270: 6573 2077 6974 6820 7468 6520 666c 6f77  es with the flow
-00012280: 206c 6f67 6765 720d 0a20 2020 2020 2020   logger..       
+000120e0: 2929 2020 2320 6375 7272 656e 7420 6163  ))  # current ac
+000120f0: 636f 756e 740d 0a20 2020 2020 2020 2066  count..        f
+00012100: 6c6f 775f 6461 7461 5b22 4b41 225d 203d  low_data["KA"] =
+00012110: 2064 6566 6175 6c74 6469 6374 286c 616d   defaultdict(lam
+00012120: 6264 613a 2064 6566 6175 6c74 6469 6374  bda: defaultdict
+00012130: 286c 6973 7429 2920 2023 2063 6170 6974  (list))  # capit
+00012140: 616c 2061 6363 6f75 6e74 0d0a 0d0a 2020  al account....  
+00012150: 2020 2020 2020 2320 666c 6f77 5f64 6174        # flow_dat
+00012160: 615b 4b41 206f 7220 4341 5d5b 7375 626a  a[KA or CA][subj
+00012170: 6563 745d 5b61 6765 6e74 5d0d 0a20 2020  ect][agent]..   
+00012180: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
+00012190: 2e65 6e74 7279 5f64 6174 6129 203d 3d20  .entry_data) == 
+000121a0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000121b0: 7365 6c66 2e6e 6f74 6966 7928 6d65 7373  self.notify(mess
+000121c0: 6167 653d 2243 616e 6e6f 7420 6765 6e65  age="Cannot gene
+000121d0: 7261 7465 204d 6174 7269 782e 2048 6176  rate Matrix. Hav
+000121e0: 6520 796f 7520 7365 7420 7570 2061 6e79  e you set up any
+000121f0: 2074 7261 6e73 6163 7469 6f6e 7320 7965   transactions ye
+00012200: 743f 222c 7469 746c 653d 2245 7272 6f72  t?",title="Error
+00012210: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00012220: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
+00012230: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00012240: 2020 2020 666f 7220 6669 6c65 6461 7461      for filedata
+00012250: 2069 6e20 7365 6c66 2e65 6e74 7279 5f64   in self.entry_d
+00012260: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
+00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012280: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
 00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 2020 2020 2020 2020 2022 2222 0d0a 2020           """..  
-000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000122d0: 626a 6563 7420 3d20 6669 6c65 6461 7461  bject = filedata
-000122e0: 5b22 7375 626a 6563 7422 5d2e 7265 706c  ["subject"].repl
-000122f0: 6163 6528 225f 222c 2022 2022 292e 7469  ace("_", " ").ti
-00012300: 746c 6528 290d 0a20 2020 2020 2020 2020  tle()..         
+000122a0: 2020 2020 2020 2020 2020 2065 7661 6c75             evalu
+000122b0: 6174 6520 7472 616e 7361 6374 696f 6e20  ate transaction 
+000122c0: 656e 7472 6965 7320 7769 7468 2074 6865  entries with the
+000122d0: 2066 6c6f 7720 6c6f 6767 6572 0d0a 2020   flow logger..  
+000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
+00012300: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
 00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012320: 2020 2020 2020 206b 696e 6420 3d20 6669         kind = fi
-00012330: 6c65 6461 7461 5b22 6b69 6e64 225d 0d0a  ledata["kind"]..
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012360: 6c6f 675f 666c 6f77 203d 2054 7275 650d  log_flow = True.
-00012370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2069 6620 6669 6c65 6461 7461 5b22 6c6f   if filedata["lo
-000123a0: 6720 7472 616e 7361 6374 696f 6e22 5d20  g transaction"] 
-000123b0: 3d3d 2022 4661 6c73 6522 3a0d 0a20 2020  == "False":..   
-000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012320: 2020 2073 7562 6a65 6374 203d 2066 696c     subject = fil
+00012330: 6564 6174 615b 2273 7562 6a65 6374 225d  edata["subject"]
+00012340: 2e72 6570 6c61 6365 2822 5f22 2c20 2220  .replace("_", " 
+00012350: 2229 2e74 6974 6c65 2829 0d0a 2020 2020  ").title()..    
+00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012370: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
+00012380: 203d 2066 696c 6564 6174 615b 226b 696e   = filedata["kin
+00012390: 6422 5d0d 0a20 2020 2020 2020 2020 2020  d"]..           
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 2020 2020 206c 6f67 5f66 6c6f 7720 3d20       log_flow = 
+000123c0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
 000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123e0: 206c 6f67 5f66 6c6f 773d 2046 616c 7365   log_flow= False
-000123f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012410: 2020 2320 2020 6c6f 675f 666c 6f77 203d    #   log_flow =
-00012420: 2062 6f6f 6c28 6669 6c65 6461 7461 5b22   bool(filedata["
-00012430: 6c6f 6720 7472 616e 7361 6374 696f 6e22  log transaction"
-00012440: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000123e0: 2020 2020 2020 6966 2066 696c 6564 6174        if filedat
+000123f0: 615b 226c 6f67 2074 7261 6e73 6163 7469  a["log transacti
+00012400: 6f6e 225d 203d 3d20 2246 616c 7365 223a  on"] == "False":
+00012410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012430: 2020 2020 2020 6c6f 675f 666c 6f77 3d20        log_flow= 
+00012440: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
 00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012460: 2020 2020 7072 696e 7428 224c 4f47 2046      print("LOG F
-00012470: 4c4f 5722 2c6c 6f67 5f66 6c6f 772c 2272  LOW",log_flow,"r
-00012480: 6177 222c 6669 6c65 6461 7461 5b22 6c6f  aw",filedata["lo
-00012490: 6720 7472 616e 7361 6374 696f 6e22 5d29  g transaction"])
-000124a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 7175 616e 7469 7479 203d 2066 696c    quantity = fil
-000124d0: 6564 6174 615b 2271 7561 6e74 6974 7922  edata["quantity"
-000124e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 2020 2061 6765 6e74 3120 3d20 6669 6c65     agent1 = file
-00012510: 6461 7461 5b22 6167 656e 7431 225d 2e72  data["agent1"].r
-00012520: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
-00012530: 2e74 6974 6c65 2829 0d0a 2020 2020 2020  .title()..      
+00012460: 2020 2020 2020 2023 2020 206c 6f67 5f66         #   log_f
+00012470: 6c6f 7720 3d20 626f 6f6c 2866 696c 6564  low = bool(filed
+00012480: 6174 615b 226c 6f67 2074 7261 6e73 6163  ata["log transac
+00012490: 7469 6f6e 225d 290d 0a20 2020 2020 2020  tion"])..       
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124b0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+000124c0: 4c4f 4720 464c 4f57 222c 6c6f 675f 666c  LOG FLOW",log_fl
+000124d0: 6f77 2c22 7261 7722 2c66 696c 6564 6174  ow,"raw",filedat
+000124e0: 615b 226c 6f67 2074 7261 6e73 6163 7469  a["log transacti
+000124f0: 6f6e 225d 290d 0a20 2020 2020 2020 2020  on"])..         
+00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012510: 2020 2020 2020 2071 7561 6e74 6974 7920         quantity 
+00012520: 3d20 6669 6c65 6461 7461 5b22 7175 616e  = filedata["quan
+00012530: 7469 7479 225d 0d0a 2020 2020 2020 2020  tity"]..        
 00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012550: 2020 2020 2020 2020 2020 6167 656e 7432            agent2
-00012560: 203d 2066 696c 6564 6174 615b 2261 6765   = filedata["age
-00012570: 6e74 3222 5d2e 7265 706c 6163 6528 225f  nt2"].replace("_
-00012580: 222c 2022 2022 292e 7469 746c 6528 290d  ", " ").title().
-00012590: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 2023 2075 7070 6572 2070 6172 7420     # upper part 
-000125c0: 6f66 206d 6174 7269 780d 0a20 2020 2020  of matrix..     
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-000125f0: 675f 666c 6f77 3a0d 0a20 2020 2020 2020  g_flow:..       
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-00012620: 6f75 6e74 5f66 726f 6d20 3d20 6b69 6e64  ount_from = kind
-00012630: 2e73 706c 6974 2822 2d3e 2229 5b30 5d0d  .split("->")[0].
-00012640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012550: 2020 2020 2020 2020 6167 656e 7431 203d          agent1 =
+00012560: 2066 696c 6564 6174 615b 2261 6765 6e74   filedata["agent
+00012570: 3122 5d2e 7265 706c 6163 6528 225f 222c  1"].replace("_",
+00012580: 2022 2022 292e 7469 746c 6528 290d 0a20   " ").title().. 
+00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000125b0: 6765 6e74 3220 3d20 6669 6c65 6461 7461  gent2 = filedata
+000125c0: 5b22 6167 656e 7432 225d 2e72 6570 6c61  ["agent2"].repla
+000125d0: 6365 2822 5f22 2c20 2220 2229 2e74 6974  ce("_", " ").tit
+000125e0: 6c65 2829 0d0a 0d0a 2020 2020 2020 2020  le()....        
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 2020 2020 2020 2320 7570 7065 7220          # upper 
+00012610: 7061 7274 206f 6620 6d61 7472 6978 0d0a  part of matrix..
+00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 6966 206c 6f67 5f66 6c6f 773a 0d0a 2020  if log_flow:..  
 00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012660: 2020 2020 2061 6363 6f75 6e74 5f74 6f20       account_to 
-00012670: 3d20 6b69 6e64 2e73 706c 6974 2822 2d3e  = kind.split("->
-00012680: 2229 5b31 5d0d 0a0d 0a20 2020 2020 2020  ")[1]....       
-00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126a0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-000126b0: 775f 6461 7461 5b61 6363 6f75 6e74 5f66  w_data[account_f
-000126c0: 726f 6d5d 5b73 7562 6a65 6374 5d5b 6167  rom][subject][ag
-000126d0: 656e 7431 5d2e 6170 7065 6e64 2822 2d22  ent1].append("-"
-000126e0: 202b 2073 7472 2871 7561 6e74 6974 7929   + str(quantity)
-000126f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2020 2020 2066 6c6f 775f 6461 7461         flow_data
-00012720: 5b61 6363 6f75 6e74 5f74 6f5d 5b73 7562  [account_to][sub
-00012730: 6a65 6374 5d5b 6167 656e 7432 5d2e 6170  ject][agent2].ap
-00012740: 7065 6e64 2873 7472 2871 7561 6e74 6974  pend(str(quantit
-00012750: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
-00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2020 2020 2020 2023 206c 6f77 6572 2070         # lower p
-00012780: 6172 7420 6f66 206d 6174 7269 7820 3d20  art of matrix = 
-00012790: 6368 616e 6765 7320 696e 2061 7373 6574  changes in asset
-000127a0: 7320 616e 7320 6c69 6162 696c 6974 6965  s ans liabilitie
-000127b0: 730d 0a0d 0a20 2020 2020 2020 2020 2020  s....           
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 2020 2020 2061 3120 3d20 6669 6c65 6461       a1 = fileda
-000127e0: 7461 5b22 6131 225d 2020 2320 2b20 225c  ta["a1"]  # + "\
-000127f0: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2020 2020 6531 203d 2066 696c 6564 6174      e1 = filedat
-00012820: 615b 2265 3122 5d20 2023 202b 2022 5c6e  a["e1"]  # + "\n
-00012830: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 206c 3120 3d20 6669 6c65 6461 7461     l1 = filedata
-00012860: 5b22 6c31 225d 2020 2320 2b20 225c 6e22  ["l1"]  # + "\n"
-00012870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012890: 2020 6132 203d 2066 696c 6564 6174 615b    a2 = filedata[
-000128a0: 2261 3222 5d20 2023 202b 2022 5c6e 220d  "a2"]  # + "\n".
-000128b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 2065 3220 3d20 6669 6c65 6461 7461 5b22   e2 = filedata["
-000128e0: 6532 225d 2020 2320 2b20 225c 6e22 0d0a  e2"]  # + "\n"..
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 6c32 203d 2066 696c 6564 6174 615b 226c  l2 = filedata["l
-00012920: 3222 5d20 2023 202b 2022 5c6e 220d 0a0d  2"]  # + "\n"...
-00012930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2023 2061 7373 6574 730d 0a20 2020 2020   # assets..     
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00012980: 7465 6d5f 6e61 6d65 2069 6e20 6131 2e73  tem_name in a1.s
-00012990: 706c 6974 2822 5c6e 2229 3a20 2023 202b  plit("\n"):  # +
-000129a0: 2065 312e 7370 6c69 7428 225c 6e22 293a   e1.split("\n"):
-000129b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012670: 2020 6163 636f 756e 745f 6672 6f6d 203d    account_from =
+00012680: 206b 696e 642e 7370 6c69 7428 222d 3e22   kind.split("->"
+00012690: 295b 305d 0d0a 2020 2020 2020 2020 2020  )[0]..          
+000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126b0: 2020 2020 2020 2020 2020 6163 636f 756e            accoun
+000126c0: 745f 746f 203d 206b 696e 642e 7370 6c69  t_to = kind.spli
+000126d0: 7428 222d 3e22 295b 315d 0d0a 0d0a 2020  t("->")[1]....  
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012700: 2020 666c 6f77 5f64 6174 615b 6163 636f    flow_data[acco
+00012710: 756e 745f 6672 6f6d 5d5b 7375 626a 6563  unt_from][subjec
+00012720: 745d 5b61 6765 6e74 315d 2e61 7070 656e  t][agent1].appen
+00012730: 6428 222d 2220 2b20 7374 7228 7175 616e  d("-" + str(quan
+00012740: 7469 7479 2929 0d0a 2020 2020 2020 2020  tity))..        
+00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012760: 2020 2020 2020 2020 2020 2020 666c 6f77              flow
+00012770: 5f64 6174 615b 6163 636f 756e 745f 746f  _data[account_to
+00012780: 5d5b 7375 626a 6563 745d 5b61 6765 6e74  ][subject][agent
+00012790: 325d 2e61 7070 656e 6428 7374 7228 7175  2].append(str(qu
+000127a0: 616e 7469 7479 2929 0d0a 0d0a 2020 2020  antity))....    
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
+000127d0: 7765 7220 7061 7274 206f 6620 6d61 7472  wer part of matr
+000127e0: 6978 203d 2063 6861 6e67 6573 2069 6e20  ix = changes in 
+000127f0: 6173 7365 7473 2061 6e73 206c 6961 6269  assets ans liabi
+00012800: 6c69 7469 6573 0d0a 0d0a 2020 2020 2020  lities....      
+00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012820: 2020 2020 2020 2020 2020 6131 203d 2066            a1 = f
+00012830: 696c 6564 6174 615b 2261 3122 5d20 2023  iledata["a1"]  #
+00012840: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
+00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012860: 2020 2020 2020 2020 2065 3120 3d20 6669           e1 = fi
+00012870: 6c65 6461 7461 5b22 6531 225d 2020 2320  ledata["e1"]  # 
+00012880: 2b20 225c 6e22 0d0a 2020 2020 2020 2020  + "\n"..        
+00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128a0: 2020 2020 2020 2020 6c31 203d 2066 696c          l1 = fil
+000128b0: 6564 6174 615b 226c 3122 5d20 2023 202b  edata["l1"]  # +
+000128c0: 2022 5c6e 220d 0a20 2020 2020 2020 2020   "\n"..         
+000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128e0: 2020 2020 2020 2061 3220 3d20 6669 6c65         a2 = file
+000128f0: 6461 7461 5b22 6132 225d 2020 2320 2b20  data["a2"]  # + 
+00012900: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
+00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012920: 2020 2020 2020 6532 203d 2066 696c 6564        e2 = filed
+00012930: 6174 615b 2265 3222 5d20 2023 202b 2022  ata["e2"]  # + "
+00012940: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
+00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012960: 2020 2020 206c 3220 3d20 6669 6c65 6461       l2 = fileda
+00012970: 7461 5b22 6c32 225d 2020 2320 2b20 225c  ta["l2"]  # + "\
+00012980: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 2020 2020 2020 2320 6173 7365 7473 0d0a        # assets..
+000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 2020 2020 6966 2069 7465 6d5f 6e61        if item_na
-000129e0: 6d65 2021 3d20 2222 3a0d 0a20 2020 2020  me != "":..     
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a10: 2020 206e 616d 6520 3d20 6974 656d 5f6e     name = item_n
-00012a20: 616d 655b 313a 5d2e 7374 7269 7028 290d  ame[1:].strip().
-00012a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129d0: 666f 7220 6974 656d 5f6e 616d 6520 696e  for item_name in
+000129e0: 2061 312e 7370 6c69 7428 225c 6e22 293a   a1.split("\n"):
+000129f0: 2020 2320 2b20 6531 2e73 706c 6974 2822    # + e1.split("
+00012a00: 5c6e 2229 3a0d 0a20 2020 2020 2020 2020  \n"):..         
+00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a20: 2020 2020 2020 2020 2020 2069 6620 6974             if it
+00012a30: 656d 5f6e 616d 6520 213d 2022 223a 0d0a  em_name != "":..
 00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 2020 2020 2020 2020 2073 6967 6e20 3d20           sign = 
-00012a60: 6974 656d 5f6e 616d 655b 305d 0d0a 0d0a  item_name[0]....
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2020 2020 2020 6966 2073 6967 6e20          if sign 
-00012aa0: 3d3d 2022 2b22 3a0d 0a20 2020 2020 2020  == "+":..       
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2020 2020 2066 6c69 7070 6564 5f73 6967       flipped_sig
-00012ae0: 6e20 3d20 222d 220d 0a20 2020 2020 2020  n = "-"..       
-00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a60: 2020 2020 2020 2020 6e61 6d65 203d 2069          name = i
+00012a70: 7465 6d5f 6e61 6d65 5b31 3a5d 2e73 7472  tem_name[1:].str
+00012a80: 6970 2829 0d0a 2020 2020 2020 2020 2020  ip()..          
+00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012aa0: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00012ab0: 676e 203d 2069 7465 6d5f 6e61 6d65 5b30  gn = item_name[0
+00012ac0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00012af0: 7369 676e 203d 3d20 222b 223a 0d0a 2020  sign == "+":..  
 00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 2020 666c 6970 7065 645f 7369 676e      flipped_sign
-00012b50: 203d 2022 2b22 0d0a 0d0a 2020 2020 2020   = "+"....      
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b20: 2020 2020 2020 2020 2020 666c 6970 7065            flippe
+00012b30: 645f 7369 676e 203d 2022 2d22 0d0a 2020  d_sign = "-"..  
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
 00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b80: 2020 6966 206e 6f74 2022 2873 2922 2069    if not "(s)" i
-00012b90: 6e20 6e61 6d65 3a0d 0a20 2020 2020 2020  n name:..       
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2020 2020 2020 2020 2066 6c69 7070 6564           flipped
+00012ba0: 5f73 6967 6e20 3d20 222b 220d 0a0d 0a20  _sign = "+".... 
 00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 2066 6c6f 775f 6461 7461 5b22       flow_data["
-00012bd0: 4b41 225d 5b22 ce94 2025 7322 2025 206e  KA"][".. %s" % n
-00012be0: 616d 655d 5b61 6765 6e74 315d 2e61 7070  ame][agent1].app
-00012bf0: 656e 6428 0d0a 2020 2020 2020 2020 2020  end(..          
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 2020 2020 2069 6620 6e6f 7420 2228         if not "(
+00012be0: 7329 2220 696e 206e 616d 653a 0d0a 2020  s)" in name:..  
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2020 2020 2020 2228 2220 2b20 666c 6970        "(" + flip
-00012c30: 7065 645f 7369 676e 202b 2071 7561 6e74  ped_sign + quant
-00012c40: 6974 7920 2b20 2229 2229 0d0a 0d0a 2020  ity + ")")....  
+00012c10: 2020 2020 2020 2020 2020 666c 6f77 5f64            flow_d
+00012c20: 6174 615b 224b 4122 5d5b 22ce 9420 2573  ata["KA"][".. %s
+00012c30: 2220 2520 6e61 6d65 5d5b 6167 656e 7431  " % name][agent1
+00012c40: 5d2e 6170 7065 6e64 280d 0a20 2020 2020  ].append(..     
 00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c60: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012c70: 7220 6974 656d 5f6e 616d 6520 696e 2061  r item_name in a
-00012c80: 322e 7370 6c69 7428 225c 6e22 293a 2020  2.split("\n"):  
-00012c90: 2320 2b20 6532 2e73 706c 6974 2822 5c6e  # + e2.split("\n
-00012ca0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c70: 2020 2020 2020 2020 2020 2022 2822 202b             "(" +
+00012c80: 2066 6c69 7070 6564 5f73 6967 6e20 2b20   flipped_sign + 
+00012c90: 7175 616e 7469 7479 202b 2022 2922 290d  quantity + ")").
+00012ca0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00012cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cc0: 2020 2020 2020 2020 2069 6620 6974 656d           if item
-00012cd0: 5f6e 616d 6520 213d 2022 223a 0d0a 2020  _name != "":..  
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2020 2020 6e61 6d65 203d 2069 7465        name = ite
-00012d10: 6d5f 6e61 6d65 5b31 3a5d 2e73 7472 6970  m_name[1:].strip
-00012d20: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 2020 2020 2020 2020 7369 676e              sign
-00012d50: 203d 2069 7465 6d5f 6e61 6d65 5b30 5d0d   = item_name[0].
-00012d60: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 2020 2020 2020 2020 2069 6620 7369             if si
-00012d90: 676e 203d 3d20 222b 223a 0d0a 2020 2020  gn == "+":..    
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dc0: 2020 2020 2020 2020 666c 6970 7065 645f          flipped_
-00012dd0: 7369 676e 203d 2022 2d22 0d0a 2020 2020  sign = "-"..    
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e00: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2066 6c69 7070 6564 5f73         flipped_s
-00012e40: 6967 6e20 3d20 222b 220d 0a0d 0a20 2020  ign = "+"....   
-00012e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cc0: 2020 2066 6f72 2069 7465 6d5f 6e61 6d65     for item_name
+00012cd0: 2069 6e20 6132 2e73 706c 6974 2822 5c6e   in a2.split("\n
+00012ce0: 2229 3a20 2023 202b 2065 322e 7370 6c69  "):  # + e2.spli
+00012cf0: 7428 225c 6e22 293a 0d0a 2020 2020 2020  t("\n"):..      
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012d20: 2069 7465 6d5f 6e61 6d65 2021 3d20 2222   item_name != ""
+00012d30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d50: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+00012d60: 3d20 6974 656d 5f6e 616d 655b 313a 5d2e  = item_name[1:].
+00012d70: 7374 7269 7028 290d 0a20 2020 2020 2020  strip()..       
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2073 6967 6e20 3d20 6974 656d 5f6e 616d   sign = item_nam
+00012db0: 655b 305d 0d0a 0d0a 2020 2020 2020 2020  e[0]....        
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012de0: 6966 2073 6967 6e20 3d3d 2022 2b22 3a0d  if sign == "+":.
+00012df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 2020 2020 2020 2020 2066 6c69               fli
+00012e20: 7070 6564 5f73 6967 6e20 3d20 222d 220d  pped_sign = "-".
+00012e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2069 6620 6e6f 7420 2228 7329       if not "(s)
-00012e80: 2220 696e 206e 616d 653a 0d0a 2020 2020  " in name:..    
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2020 2020 2020 2020 666c 6f77 5f64 6174          flow_dat
-00012ec0: 615b 224b 4122 5d5b 22ce 9420 2573 2220  a["KA"][".. %s" 
-00012ed0: 2520 6e61 6d65 5d5b 6167 656e 7432 5d2e  % name][agent2].
-00012ee0: 6170 7065 6e64 280d 0a20 2020 2020 2020  append(..       
+00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e80: 2020 2020 2020 2020 2020 2020 666c 6970              flip
+00012e90: 7065 645f 7369 676e 203d 2022 2b22 0d0a  ped_sign = "+"..
+00012ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00012ed0: 2022 2873 2922 2069 6e20 6e61 6d65 3a0d   "(s)" in name:.
+00012ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2020 2020 2022 2822 202b 2066           "(" + f
-00012f20: 6c69 7070 6564 5f73 6967 6e20 2b20 7175  lipped_sign + qu
-00012f30: 616e 7469 7479 202b 2022 2922 290d 0a0d  antity + ")")...
-00012f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f00: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00012f10: 775f 6461 7461 5b22 4b41 225d 5b22 ce94  w_data["KA"]["..
+00012f20: 2025 7322 2025 206e 616d 655d 5b61 6765   %s" % name][age
+00012f30: 6e74 325d 2e61 7070 656e 6428 0d0a 2020  nt2].append(..  
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f60: 2023 206c 6961 6269 6c69 7469 6573 0d0a   # liabilities..
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f90: 666f 7220 6974 656d 5f6e 616d 6520 696e  for item_name in
-00012fa0: 206c 312e 7370 6c69 7428 225c 6e22 293a   l1.split("\n"):
-00012fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fd0: 2020 2020 2020 6966 2069 7465 6d5f 6e61        if item_na
-00012fe0: 6d65 2021 3d20 2222 3a0d 0a20 2020 2020  me != "":..     
-00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 2020 206e 616d 6520 3d20 6974 656d 5f6e     name = item_n
-00013020: 616d 655b 313a 5d2e 7374 7269 7028 290d  ame[1:].strip().
-00013030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f60: 2020 2020 2020 2020 2020 2020 2020 2228                "(
+00012f70: 2220 2b20 666c 6970 7065 645f 7369 676e  " + flipped_sign
+00012f80: 202b 2071 7561 6e74 6974 7920 2b20 2229   + quantity + ")
+00012f90: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2020 2320 6c69 6162 696c 6974        # liabilit
+00012fc0: 6965 730d 0a20 2020 2020 2020 2020 2020  ies..           
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2020 2020 2066 6f72 2069 7465 6d5f 6e61       for item_na
+00012ff0: 6d65 2069 6e20 6c31 2e73 706c 6974 2822  me in l1.split("
+00013000: 5c6e 2229 3a0d 0a20 2020 2020 2020 2020  \n"):..         
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 2020 2020 2020 2020 2069 6620 6974             if it
+00013030: 656d 5f6e 616d 6520 213d 2022 223a 0d0a  em_name != "":..
 00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2020 2020 2020 2020 2073 6967 6e20 3d20           sign = 
-00013060: 6974 656d 5f6e 616d 655b 305d 0d0a 0d0a  item_name[0]....
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013090: 2020 2020 2020 2020 6966 206e 6f74 2022          if not "
-000130a0: 2873 2922 2069 6e20 6e61 6d65 3a0d 0a20  (s)" in name:.. 
-000130b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 2020 2020 2020 2066 6c6f 775f             flow_
-000130e0: 6461 7461 5b22 4b41 225d 5b22 ce94 2025  data["KA"][".. %
-000130f0: 7322 2025 206e 616d 655d 5b61 6765 6e74  s" % name][agent
-00013100: 315d 2e61 7070 656e 6428 0d0a 2020 2020  1].append(..    
+00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013060: 2020 2020 2020 2020 6e61 6d65 203d 2069          name = i
+00013070: 7465 6d5f 6e61 6d65 5b31 3a5d 2e73 7472  tem_name[1:].str
+00013080: 6970 2829 0d0a 2020 2020 2020 2020 2020  ip()..          
+00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130a0: 2020 2020 2020 2020 2020 2020 2020 7369                si
+000130b0: 676e 203d 2069 7465 6d5f 6e61 6d65 5b30  gn = item_name[0
+000130c0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000130f0: 6e6f 7420 2228 7329 2220 696e 206e 616d  not "(s)" in nam
+00013100: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 2020 2020 2020 2020 2020 2020 2228 2220              "(" 
-00013140: 2b20 7369 676e 202b 2071 7561 6e74 6974  + sign + quantit
-00013150: 7920 2b20 2229 2229 0d0a 0d0a 2020 2020  y + ")")....    
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00013180: 6974 656d 5f6e 616d 6520 696e 206c 322e  item_name in l2.
-00013190: 7370 6c69 7428 225c 6e22 293a 0d0a 2020  split("\n"):..  
-000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 2020 6966 2069 7465 6d5f 6e61 6d65 2021    if item_name !
-000131d0: 3d20 2222 3a0d 0a20 2020 2020 2020 2020  = "":..         
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00013200: 616d 6520 3d20 6974 656d 5f6e 616d 655b  ame = item_name[
-00013210: 313a 5d2e 7374 7269 7028 290d 0a20 2020  1:].strip()..   
-00013220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013130: 666c 6f77 5f64 6174 615b 224b 4122 5d5b  flow_data["KA"][
+00013140: 22ce 9420 2573 2220 2520 6e61 6d65 5d5b  ".. %s" % name][
+00013150: 6167 656e 7431 5d2e 6170 7065 6e64 280d  agent1].append(.
+00013160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013190: 2022 2822 202b 2073 6967 6e20 2b20 7175   "(" + sign + qu
+000131a0: 616e 7469 7479 202b 2022 2922 290d 0a0d  antity + ")")...
+000131b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131d0: 2066 6f72 2069 7465 6d5f 6e61 6d65 2069   for item_name i
+000131e0: 6e20 6c32 2e73 706c 6974 2822 5c6e 2229  n l2.split("\n")
+000131f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013210: 2020 2020 2020 2069 6620 6974 656d 5f6e         if item_n
+00013220: 616d 6520 213d 2022 223a 0d0a 2020 2020  ame != "":..    
 00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013240: 2020 2020 2073 6967 6e20 3d20 6974 656d       sign = item
-00013250: 5f6e 616d 655b 305d 0d0a 0d0a 2020 2020  _name[0]....    
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 2020 2020 6966 206e 6f74 2022 2873 2922      if not "(s)"
-00013290: 2069 6e20 6e61 6d65 3a0d 0a20 2020 2020   in name:..     
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132c0: 2020 2020 2020 2066 6c6f 775f 6461 7461         flow_data
-000132d0: 5b22 4b41 225d 5b22 ce94 2025 7322 2025  ["KA"][".. %s" %
-000132e0: 206e 616d 655d 5b61 6765 6e74 325d 2e61   name][agent2].a
-000132f0: 7070 656e 6428 0d0a 2020 2020 2020 2020  ppend(..        
+00013240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013250: 2020 2020 6e61 6d65 203d 2069 7465 6d5f      name = item_
+00013260: 6e61 6d65 5b31 3a5d 2e73 7472 6970 2829  name[1:].strip()
+00013270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 2020 2020 2020 2020 2020 7369 676e 203d            sign =
+000132a0: 2069 7465 6d5f 6e61 6d65 5b30 5d0d 0a0d   item_name[0]...
+000132b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000132e0: 2228 7329 2220 696e 206e 616d 653a 0d0a  "(s)" in name:..
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 2020 2020 2228 2220 2b20 7369          "(" + si
-00013330: 676e 202b 2071 7561 6e74 6974 7920 2b20  gn + quantity + 
-00013340: 2229 2229 0d0a 0d0a 2020 2020 2020 2020  ")")....        
-00013350: 2020 2020 2320 7072 696e 7428 666c 6f77      # print(flow
-00013360: 5f64 6174 6129 0d0a 2020 2020 2020 2020  _data)..        
-00013370: 2020 2020 6466 5f63 7265 6469 7420 3d20      df_credit = 
-00013380: 7064 2e44 6174 6146 7261 6d65 2866 6c6f  pd.DataFrame(flo
-00013390: 775f 6461 7461 5b22 4341 225d 292e 540d  w_data["CA"]).T.
-000133a0: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-000133b0: 6361 7069 7461 6c20 3d20 7064 2e44 6174  capital = pd.Dat
-000133c0: 6146 7261 6d65 2866 6c6f 775f 6461 7461  aFrame(flow_data
-000133d0: 5b22 4b41 225d 292e 540d 0a0d 0a20 2020  ["KA"]).T....   
-000133e0: 2020 2020 2020 2020 2064 665f 6d65 7267           df_merg
-000133f0: 6520 3d20 7064 2e63 6f6e 6361 7428 5b64  e = pd.concat([d
-00013400: 665f 6372 6564 6974 2c20 6466 5f63 6170  f_credit, df_cap
-00013410: 6974 616c 5d2c 2061 7869 733d 312c 206b  ital], axis=1, k
-00013420: 6579 733d 5b27 4341 272c 2027 4b41 275d  eys=['CA', 'KA']
-00013430: 292e 7377 6170 6c65 7665 6c28 302c 2031  ).swaplevel(0, 1
-00013440: 2c61 7869 733d 3129 2e73 6f72 745f 696e  ,axis=1).sort_in
-00013450: 6465 7828 6178 6973 3d31 290d 0a0d 0a0d  dex(axis=1).....
-00013460: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-00013470: 7070 656e 6420 6e65 7720 636f 6c75 6d6e  ppend new column
-00013480: 730d 0a20 2020 2020 2020 2020 2020 2063  s..            c
-00013490: 6f6c 5f64 6963 745f 6361 203d 207b 7d0d  ol_dict_ca = {}.
-000134a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000134b0: 2063 6f6c 2069 6e20 6466 5f63 7265 6469   col in df_credi
-000134c0: 742e 636f 6c75 6d6e 733a 0d0a 2020 2020  t.columns:..    
-000134d0: 2020 2020 2020 2020 2020 2020 636f 6c5f              col_
-000134e0: 6469 6374 5f63 615b 636f 6c5d 203d 2063  dict_ca[col] = c
-000134f0: 6f6c 202b 2022 2028 4341 2922 0d0a 0d0a  ol + " (CA)"....
-00013500: 2020 2020 2020 2020 2020 2020 636f 6c5f              col_
-00013510: 6469 6374 5f6b 6120 3d20 7b7d 0d0a 2020  dict_ka = {}..  
-00013520: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-00013530: 6c20 696e 2064 665f 6361 7069 7461 6c2e  l in df_capital.
-00013540: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
-00013550: 2020 2020 2020 2020 2020 636f 6c5f 6469            col_di
-00013560: 6374 5f6b 615b 636f 6c5d 203d 2063 6f6c  ct_ka[col] = col
-00013570: 202b 2022 2028 4b41 2922 0d0a 0d0a 2020   + " (KA)"....  
-00013580: 2020 2020 2020 2020 2020 6466 5f63 7265            df_cre
-00013590: 6469 7420 3d20 6466 5f63 7265 6469 742e  dit = df_credit.
-000135a0: 7265 6e61 6d65 2863 6f6c 756d 6e73 203d  rename(columns =
-000135b0: 2063 6f6c 5f64 6963 745f 6361 290d 0a20   col_dict_ca).. 
-000135c0: 2020 2020 2020 2020 2020 2064 665f 6361             df_ca
-000135d0: 7069 7461 6c20 3d20 6466 5f63 6170 6974  pital = df_capit
-000135e0: 616c 2e72 656e 616d 6528 636f 6c75 6d6e  al.rename(column
-000135f0: 733d 636f 6c5f 6469 6374 5f6b 6129 0d0a  s=col_dict_ka)..
-00013600: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00013610: 5f6d 6572 6765 3220 3d20 7064 2e63 6f6e  _merge2 = pd.con
-00013620: 6361 7428 5b64 665f 6372 6564 6974 2c20  cat([df_credit, 
-00013630: 6466 5f63 6170 6974 616c 5d2c 2061 7869  df_capital], axi
-00013640: 733d 3129 0d0a 0d0a 2020 2020 2020 2020  s=1)....        
-00013650: 2020 2020 6466 5f6d 6572 6765 3220 3d20      df_merge2 = 
-00013660: 6466 5f6d 6572 6765 322e 7265 696e 6465  df_merge2.reinde
-00013670: 7828 736f 7274 6564 2864 665f 6d65 7267  x(sorted(df_merg
-00013680: 6532 2e63 6f6c 756d 6e73 292c 2061 7869  e2.columns), axi
-00013690: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
-000136a0: 2020 6466 5f6d 6572 6765 3220 3d20 6466    df_merge2 = df
-000136b0: 5f6d 6572 6765 322e 7265 696e 6465 7828  _merge2.reindex(
-000136c0: 736f 7274 6564 2864 665f 6d65 7267 6532  sorted(df_merge2
-000136d0: 2e69 6e64 6578 292c 2061 7869 733d 3029  .index), axis=0)
-000136e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000136f0: 6466 203d 2064 665f 6d65 7267 652e 6669  df = df_merge.fi
-00013700: 6c6c 6e61 2830 2e30 292e 736f 7274 5f69  llna(0.0).sort_i
-00013710: 6e64 6578 2829 0d0a 0d0a 0d0a 2020 2020  ndex()......    
-00013720: 2020 2020 2020 2020 6465 6620 6a6f 696e          def join
-00013730: 5f65 6c65 6d65 6e74 7328 6d79 5f69 7465  _elements(my_ite
-00013740: 6d29 3a0d 0a20 2020 2020 2020 2020 2020  m):..           
-00013750: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00013760: 6365 286d 795f 6974 656d 2c20 6c69 7374  ce(my_item, list
-00013770: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00013780: 2020 2020 2020 2020 6d79 5f6c 6973 7420          my_list 
-00013790: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000137a0: 2020 2020 2020 2020 2020 666f 7220 7375            for su
-000137b0: 6269 7465 6d20 696e 206d 795f 6974 656d  bitem in my_item
-000137c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000137d0: 2020 2020 2020 2020 2020 2069 6620 7375             if su
-000137e0: 6269 7465 6d20 213d 2022 3022 3a0d 0a20  bitem != "0":.. 
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 2020 2020 2020 2020 206d 795f 6c69             my_li
-00013810: 7374 2e61 7070 656e 6428 7375 6269 7465  st.append(subite
-00013820: 6d29 0d0a 0d0a 2020 2020 2020 2020 2020  m)....          
-00013830: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013840: 2022 2b22 2e6a 6f69 6e28 6d79 5f6c 6973   "+".join(my_lis
-00013850: 7429 0d0a 0d0a 2020 2020 2020 2020 2020  t)....          
-00013860: 2020 2020 2020 656c 6966 206d 795f 6974        elif my_it
-00013870: 656d 203d 3d20 302e 303a 0d0a 2020 2020  em == 0.0:..    
-00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013890: 7265 7475 726e 2022 3022 0d0a 2020 2020  return "0"..    
-000138a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000138b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000138c0: 2020 2020 2020 2072 6574 7572 6e20 6d79         return my
-000138d0: 5f69 7465 6d0d 0a0d 0a20 2020 2020 2020  _item....       
-000138e0: 2020 2020 2064 6620 3d20 6466 2e61 7070       df = df.app
-000138f0: 6c79 6d61 7028 6a6f 696e 5f65 6c65 6d65  lymap(join_eleme
-00013900: 6e74 7329 0d0a 0d0a 0d0a 0d0a 2020 2020  nts)........    
-00013910: 2020 2020 2020 2020 2320 7375 6d20 6f76          # sum ov
-00013920: 6572 2074 6865 2063 6f6c 756d 6e73 0d0a  er the columns..
-00013930: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
-00013940: 6620 6576 616c 5f73 756d 2863 6f6c 756d  f eval_sum(colum
-00013950: 6e29 3a0d 0a20 2020 2020 2020 2020 2020  n):..           
-00013960: 2020 2020 2063 6f6c 756d 6e20 3d20 5b73       column = [s
-00013970: 7472 2863 292e 7265 706c 6163 6528 225e  tr(c).replace("^
-00013980: 222c 2022 2a2a 2229 2066 6f72 2063 2069  ", "**") for c i
-00013990: 6e20 636f 6c75 6d6e 5d0d 0a20 2020 2020  n column]..     
-000139a0: 2020 2020 2020 2020 2020 206d 795f 6578             my_ex
-000139b0: 7072 203d 2022 2b22 2e6a 6f69 6e28 636f  pr = "+".join(co
-000139c0: 6c75 6d6e 290d 0a20 2020 2020 2020 2020  lumn)..         
-000139d0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000139e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139f0: 2072 6574 7572 6e20 7061 7273 655f 6578   return parse_ex
-00013a00: 7072 286d 795f 6578 7072 290d 0a20 2020  pr(my_expr)..   
-00013a10: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00013a20: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
-00013a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013a40: 206d 795f 6578 7072 0d0a 0d0a 0d0a 0d0a   my_expr........
-00013a50: 2020 2020 2020 2020 2020 2020 6466 5b22              df["
-00013a60: 546f 7461 6c22 5d20 3d20 6466 2e54 2e61  Total"] = df.T.a
-00013a70: 6767 2865 7661 6c5f 7375 6d29 2020 2320  gg(eval_sum)  # 
-00013a80: 6466 2e54 2e73 756d 2829 0d0a 2020 2020  df.T.sum()..    
-00013a90: 2020 2020 2020 2020 6466 2e6c 6f63 5b22          df.loc["
-00013aa0: 546f 7461 6c22 5d20 3d20 6466 2e61 6767  Total"] = df.agg
-00013ab0: 2865 7661 6c5f 7375 6d29 0d0a 2020 2020  (eval_sum)..    
-00013ac0: 2020 2020 2020 2020 7072 696e 7428 2254          print("T
-00013ad0: 4f54 414c 222c 6466 2e6c 6f63 5b22 546f  OTAL",df.loc["To
-00013ae0: 7461 6c22 5d29 0d0a 2020 2020 2020 2020  tal"])..        
-00013af0: 2020 2020 6466 5f6d 6572 6765 325b 2254      df_merge2["T
-00013b00: 6f74 616c 225d 203d 2064 665b 2254 6f74  otal"] = df["Tot
-00013b10: 616c 225d 0d0a 0d0a 2020 2020 2020 2020  al"]....        
-00013b20: 2020 2020 2320 6765 7420 7468 6520 6e65      # get the ne
-00013b30: 7720 636f 6c75 6d6e 730d 0a0d 0a20 2020  w columns....   
-00013b40: 2020 2020 2020 2020 2023 2069 7465 7261           # itera
-00013b50: 7465 2074 6872 6f75 6768 2074 6865 2063  te through the c
-00013b60: 6f6c 756d 6e73 0d0a 2020 2020 2020 2020  olumns..        
-00013b70: 2020 2020 7072 696e 7428 6466 2e63 6f6c      print(df.col
-00013b80: 756d 6e73 290d 0a0d 0a0d 0a20 2020 2020  umns)......     
-00013b90: 2020 2020 2020 2066 6f72 2063 6f6c 756d         for colum
-00013ba0: 6e20 696e 2064 662e 636f 6c75 6d6e 733a  n in df.columns:
-00013bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013bc0: 2020 6966 2063 6f6c 756d 6e5b 305d 2021    if column[0] !
-00013bd0: 3d20 2254 6f74 616c 223a 0d0a 2020 2020  = "Total":..    
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 7072 696e 7428 636f 6c75 6d6e 5b30 5d20  print(column[0] 
-00013c00: 2b20 2220 2220 202b 2022 2825 7329 2220  + " "  + "(%s)" 
-00013c10: 2520 636f 6c75 6d6e 5b31 5d2c 6466 2e6c  % column[1],df.l
-00013c20: 6f63 5b22 546f 7461 6c22 5d5b 636f 6c75  oc["Total"][colu
-00013c30: 6d6e 5d29 0d0a 2020 2020 2020 2020 2020  mn])..          
-00013c40: 2020 2020 2020 2020 2020 6466 5f6d 6572            df_mer
-00013c50: 6765 322e 6c6f 635b 2254 6f74 616c 222c  ge2.loc["Total",
-00013c60: 636f 6c75 6d6e 5b30 5d20 2b20 2220 2220  column[0] + " " 
-00013c70: 202b 2022 2825 7329 2220 2520 636f 6c75   + "(%s)" % colu
-00013c80: 6d6e 5b31 5d5d 203d 2064 662e 6c6f 635b  mn[1]] = df.loc[
-00013c90: 2254 6f74 616c 225d 5b63 6f6c 756d 6e5d  "Total"][column]
-00013ca0: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
-00013cb0: 2020 2020 6465 6620 7369 6d70 6c69 6679      def simplify
-00013cc0: 5f65 7870 7228 6d79 5f69 7465 6d29 3a0d  _expr(my_item):.
-00013cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ce0: 2072 6574 7572 6e20 7369 6d70 6c69 6679   return simplify
-00013cf0: 286d 795f 6974 656d 290d 0a0d 0a20 2020  (my_item)....   
-00013d00: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
-00013d10: 2e61 7070 6c79 6d61 7028 7369 6d70 6c69  .applymap(simpli
-00013d20: 6679 5f65 7870 7229 0d0a 0d0a 2020 2020  fy_expr)....    
-00013d30: 2020 2020 2020 2020 6466 5f66 6f72 5f65          df_for_e
-00013d40: 7863 656c 203d 2064 662e 636f 7079 2829  xcel = df.copy()
-00013d50: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
-00013d60: 2020 2020 6465 6620 6162 6272 6576 6961      def abbrevia
-00013d70: 7465 5f7a 6572 6f73 5f6c 6174 6578 286d  te_zeros_latex(m
-00013d80: 795f 6974 656d 293a 0d0a 2020 2020 2020  y_item):..      
-00013d90: 2020 2020 2020 2020 2020 6966 206d 795f            if my_
-00013da0: 6974 656d 203d 3d20 2230 2220 6f72 206d  item == "0" or m
-00013db0: 795f 6974 656d 203d 3d20 303a 0d0a 2020  y_item == 0:..  
-00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 7265 7475 726e 2022 202e 2d20 2220    return " .- " 
-00013de0: 2023 202e 2d20 220d 0a20 2020 2020 2020   # .- "..       
-00013df0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00013e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e10: 2020 2020 7320 3d20 7072 696e 7469 6e67      s = printing
-00013e20: 2e6c 6174 6578 286d 795f 6974 656d 202c  .latex(my_item ,
-00013e30: 6d6f 6465 3d22 696e 6c69 6e65 2229 2023  mode="inline") #
-00013e40: 2020 6d6f 6465 3d22 696e 6c69 6e65 2229    mode="inline")
-00013e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013e60: 2020 2020 2020 7072 696e 7428 7329 0d0a        print(s)..
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 2020 2020 7265 7475 726e 2073 0d0a 0d0a      return s....
-00013e90: 2020 2020 2020 2020 2020 2020 2364 665f              #df_
-00013ea0: 6261 636b 7570 203d 2064 662e 636f 7079  backup = df.copy
-00013eb0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00013ec0: 6466 203d 2064 662e 6170 706c 796d 6170  df = df.applymap
-00013ed0: 2861 6262 7265 7669 6174 655f 7a65 726f  (abbreviate_zero
-00013ee0: 735f 6c61 7465 7829 0d0a 0d0a 0d0a 0d0a  s_latex)........
-00013ef0: 2020 2020 2020 2020 2020 2020 6466 5f6d              df_m
-00013f00: 6572 6765 3220 3d20 6466 5f6d 6572 6765  erge2 = df_merge
-00013f10: 322e 7265 706c 6163 6528 6e70 2e6e 616e  2.replace(np.nan
-00013f20: 2c20 2727 2c20 7265 6765 783d 5472 7565  , '', regex=True
-00013f30: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00013f40: 665f 6d65 7267 6532 203d 2064 665f 6d65  f_merge2 = df_me
-00013f50: 7267 6532 2e72 6570 6c61 6365 2822 3022  rge2.replace("0"
-00013f60: 2c20 2727 2c20 7265 6765 783d 5472 7565  , '', regex=True
-00013f70: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00013f80: 665f 6d65 7267 6532 203d 2064 665f 6d65  f_merge2 = df_me
-00013f90: 7267 6532 2e72 6570 6c61 6365 2830 2c20  rge2.replace(0, 
-00013fa0: 2727 2c20 7265 6765 783d 5472 7565 290d  '', regex=True).
-00013fb0: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-00013fc0: 6d65 7267 6532 203d 2064 665f 6d65 7267  merge2 = df_merg
-00013fd0: 6532 2e72 6570 6c61 6365 2830 2e30 2c20  e2.replace(0.0, 
-00013fe0: 2727 2c20 7265 6765 783d 5472 7565 290d  '', regex=True).
-00013ff0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00014000: 2070 7269 6e74 2864 662e 746f 5f73 7472   print(df.to_str
-00014010: 696e 6728 2929 0d0a 2020 2020 2020 2020  ing())..        
-00014020: 2020 2020 2320 6466 2e69 6c6f 635b 302c      # df.iloc[0,
-00014030: 305d 203d 2022 245c 5c61 6c70 6861 2422  0] = "$\\alpha$"
-00014040: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014050: 7064 2e6f 7074 696f 6e73 2e64 6973 706c  pd.options.displ
-00014060: 6179 2e6d 6178 5f63 6f6c 7769 6474 6820  ay.max_colwidth 
-00014070: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 2020  = None....      
-00014080: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-00014090: 2022 6874 6d6c 223a 2023 203c 204e 4f54   "html": # < NOT
-000140a0: 2059 4554 2053 5550 504f 5254 4544 0d0a   YET SUPPORTED..
-000140b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000140c0: 2020 6466 5f68 746d 6c20 3d20 2222 220d    df_html = """.
-000140d0: 0a20 2020 2020 2020 203c 6874 6d6c 3e0d  .        <html>.
-000140e0: 0a20 2020 2020 2020 203c 6865 6164 3e0d  .        <head>.
-000140f0: 0a20 2020 2020 2020 203c 7469 746c 653e  .        <title>
-00014100: 4d61 7468 6564 656d 6f3c 2f74 6974 6c65  Mathedemo</title
-00014110: 3e0d 0a20 2020 2020 2020 203c 7363 7269  >..        <scri
-00014120: 7074 2074 7970 653d 2274 6578 742f 782d  pt type="text/x-
-00014130: 6d61 7468 6a61 782d 636f 6e66 6967 223e  mathjax-config">
-00014140: 0d0a 2020 2020 2020 2020 2020 4d61 7468  ..          Math
-00014150: 4a61 782e 4875 622e 436f 6e66 6967 287b  Jax.Hub.Config({
-00014160: 7465 7832 6a61 783a 207b 696e 6c69 6e65  tex2jax: {inline
-00014170: 4d61 7468 3a20 5b5b 2724 272c 2724 275d  Math: [['$','$']
-00014180: 2c20 5b27 5c5c 2827 2c27 5c5c 2927 5d5d  , ['\\(','\\)']]
-00014190: 7d7d 293b 0d0a 2020 2020 2020 2020 3c2f  }});..        </
-000141a0: 7363 7269 7074 3e0d 0a20 2020 2020 2020  script>..       
-000141b0: 203c 7363 7269 7074 2074 7970 653d 2274   <script type="t
-000141c0: 6578 742f 6a61 7661 7363 7269 7074 220d  ext/javascript".
-000141d0: 0a20 2020 2020 2020 2020 2073 7263 3d22  .          src="
-000141e0: 6874 7470 3a2f 2f63 646e 6a73 2e63 6c6f  http://cdnjs.clo
-000141f0: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
-00014200: 2f6c 6962 732f 6d61 7468 6a61 782f 322e  /libs/mathjax/2.
-00014210: 372e 312f 4d61 7468 4a61 782e 6a73 3f63  7.1/MathJax.js?c
-00014220: 6f6e 6669 673d 5465 582d 414d 532d 4d4d  onfig=TeX-AMS-MM
-00014230: 4c5f 4854 4d4c 6f72 4d4d 4c22 3e0d 0a20  L_HTMLorMML">.. 
-00014240: 2020 2020 2020 203c 2f73 6372 6970 743e         </script>
-00014250: 0d0a 2020 2020 2020 2020 3c6c 696e 6b20  ..        <link 
-00014260: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
-00014270: 2068 7265 663d 226d 7973 7479 6c65 2e63   href="mystyle.c
-00014280: 7373 223e 0d0a 2020 2020 2020 2020 3c2f  ss">..        </
-00014290: 6865 6164 3e0d 0a0d 0a20 2020 2020 2020  head>....       
-000142a0: 203c 626f 6479 3e0d 0a20 2020 2020 2020   <body>..       
-000142b0: 2025 730d 0a20 2020 2020 2020 203c 2f62   %s..        </b
-000142c0: 6f64 793e 0d0a 2020 2020 2020 2020 3c2f  ody>..        </
-000142d0: 6874 6d6c 3e0d 0a20 2020 2020 2020 2022  html>..        "
-000142e0: 2222 2520 2064 662e 746f 5f68 746d 6c28  ""%  df.to_html(
-000142f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00014300: 2020 2020 2070 6167 6553 6f75 7263 6520       pageSource 
-00014310: 3d20 2222 220d 0a20 2020 2020 2020 2020  = """..         
-00014320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014330: 2020 2020 3c68 746d 6c3e 3c68 6561 643e      <html><head>
-00014340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014350: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00014360: 2f68 6561 643e 0d0a 2020 2020 2020 2020  /head>..        
+00013310: 2020 2020 2020 2020 2020 2020 666c 6f77              flow
+00013320: 5f64 6174 615b 224b 4122 5d5b 22ce 9420  _data["KA"][".. 
+00013330: 2573 2220 2520 6e61 6d65 5d5b 6167 656e  %s" % name][agen
+00013340: 7432 5d2e 6170 7065 6e64 280d 0a20 2020  t2].append(..   
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 2020 2020 2020 2020 2020 2020 2022 2822               "("
+00013380: 202b 2073 6967 6e20 2b20 7175 616e 7469   + sign + quanti
+00013390: 7479 202b 2022 2922 290d 0a0d 0a20 2020  ty + ")")....   
+000133a0: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
+000133b0: 2866 6c6f 775f 6461 7461 290d 0a20 2020  (flow_data)..   
+000133c0: 2020 2020 2020 2020 2064 665f 6372 6564           df_cred
+000133d0: 6974 203d 2070 642e 4461 7461 4672 616d  it = pd.DataFram
+000133e0: 6528 666c 6f77 5f64 6174 615b 2243 4122  e(flow_data["CA"
+000133f0: 5d29 2e54 0d0a 2020 2020 2020 2020 2020  ]).T..          
+00013400: 2020 6466 5f63 6170 6974 616c 203d 2070    df_capital = p
+00013410: 642e 4461 7461 4672 616d 6528 666c 6f77  d.DataFrame(flow
+00013420: 5f64 6174 615b 224b 4122 5d29 2e54 0d0a  _data["KA"]).T..
+00013430: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00013440: 5f6d 6572 6765 203d 2070 642e 636f 6e63  _merge = pd.conc
+00013450: 6174 285b 6466 5f63 7265 6469 742c 2064  at([df_credit, d
+00013460: 665f 6361 7069 7461 6c5d 2c20 6178 6973  f_capital], axis
+00013470: 3d31 2c20 6b65 7973 3d5b 2743 4127 2c20  =1, keys=['CA', 
+00013480: 274b 4127 5d29 2e73 7761 706c 6576 656c  'KA']).swaplevel
+00013490: 2830 2c20 312c 6178 6973 3d31 292e 736f  (0, 1,axis=1).so
+000134a0: 7274 5f69 6e64 6578 2861 7869 733d 3129  rt_index(axis=1)
+000134b0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+000134c0: 2020 2320 6170 7065 6e64 206e 6577 2063    # append new c
+000134d0: 6f6c 756d 6e73 0d0a 2020 2020 2020 2020  olumns..        
+000134e0: 2020 2020 636f 6c5f 6469 6374 5f63 6120      col_dict_ca 
+000134f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00013500: 2020 666f 7220 636f 6c20 696e 2064 665f    for col in df_
+00013510: 6372 6564 6974 2e63 6f6c 756d 6e73 3a0d  credit.columns:.
+00013520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013530: 2063 6f6c 5f64 6963 745f 6361 5b63 6f6c   col_dict_ca[col
+00013540: 5d20 3d20 636f 6c20 2b20 2220 2843 4129  ] = col + " (CA)
+00013550: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
+00013560: 2063 6f6c 5f64 6963 745f 6b61 203d 207b   col_dict_ka = {
+00013570: 7d0d 0a20 2020 2020 2020 2020 2020 2066  }..            f
+00013580: 6f72 2063 6f6c 2069 6e20 6466 5f63 6170  or col in df_cap
+00013590: 6974 616c 2e63 6f6c 756d 6e73 3a0d 0a20  ital.columns:.. 
+000135a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135b0: 6f6c 5f64 6963 745f 6b61 5b63 6f6c 5d20  ol_dict_ka[col] 
+000135c0: 3d20 636f 6c20 2b20 2220 284b 4129 220d  = col + " (KA)".
+000135d0: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
+000135e0: 665f 6372 6564 6974 203d 2064 665f 6372  f_credit = df_cr
+000135f0: 6564 6974 2e72 656e 616d 6528 636f 6c75  edit.rename(colu
+00013600: 6d6e 7320 3d20 636f 6c5f 6469 6374 5f63  mns = col_dict_c
+00013610: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
+00013620: 6466 5f63 6170 6974 616c 203d 2064 665f  df_capital = df_
+00013630: 6361 7069 7461 6c2e 7265 6e61 6d65 2863  capital.rename(c
+00013640: 6f6c 756d 6e73 3d63 6f6c 5f64 6963 745f  olumns=col_dict_
+00013650: 6b61 290d 0a0d 0a20 2020 2020 2020 2020  ka)....         
+00013660: 2020 2064 665f 6d65 7267 6532 203d 2070     df_merge2 = p
+00013670: 642e 636f 6e63 6174 285b 6466 5f63 7265  d.concat([df_cre
+00013680: 6469 742c 2064 665f 6361 7069 7461 6c5d  dit, df_capital]
+00013690: 2c20 6178 6973 3d31 290d 0a0d 0a20 2020  , axis=1)....   
+000136a0: 2020 2020 2020 2020 2064 665f 6d65 7267           df_merg
+000136b0: 6532 203d 2064 665f 6d65 7267 6532 2e72  e2 = df_merge2.r
+000136c0: 6569 6e64 6578 2873 6f72 7465 6428 6466  eindex(sorted(df
+000136d0: 5f6d 6572 6765 322e 636f 6c75 6d6e 7329  _merge2.columns)
+000136e0: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
+000136f0: 2020 2020 2020 2064 665f 6d65 7267 6532         df_merge2
+00013700: 203d 2064 665f 6d65 7267 6532 2e72 6569   = df_merge2.rei
+00013710: 6e64 6578 2873 6f72 7465 6428 6466 5f6d  ndex(sorted(df_m
+00013720: 6572 6765 322e 696e 6465 7829 2c20 6178  erge2.index), ax
+00013730: 6973 3d30 290d 0a0d 0a20 2020 2020 2020  is=0)....       
+00013740: 2020 2020 2064 6620 3d20 6466 5f6d 6572       df = df_mer
+00013750: 6765 2e66 696c 6c6e 6128 302e 3029 2e73  ge.fillna(0.0).s
+00013760: 6f72 745f 696e 6465 7828 290d 0a0d 0a0d  ort_index().....
+00013770: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00013780: 206a 6f69 6e5f 656c 656d 656e 7473 286d   join_elements(m
+00013790: 795f 6974 656d 293a 0d0a 2020 2020 2020  y_item):..      
+000137a0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000137b0: 6e73 7461 6e63 6528 6d79 5f69 7465 6d2c  nstance(my_item,
+000137c0: 206c 6973 7429 3a0d 0a20 2020 2020 2020   list):..       
+000137d0: 2020 2020 2020 2020 2020 2020 206d 795f               my_
+000137e0: 6c69 7374 203d 205b 5d0d 0a20 2020 2020  list = []..     
+000137f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013800: 6f72 2073 7562 6974 656d 2069 6e20 6d79  or subitem in my
+00013810: 5f69 7465 6d3a 0d0a 2020 2020 2020 2020  _item:..        
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013830: 6966 2073 7562 6974 656d 2021 3d20 2230  if subitem != "0
+00013840: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 6d79 5f6c 6973 742e 6170 7065 6e64 2873  my_list.append(s
+00013870: 7562 6974 656d 290d 0a0d 0a20 2020 2020  ubitem)....     
+00013880: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00013890: 6574 7572 6e20 222b 222e 6a6f 696e 286d  eturn "+".join(m
+000138a0: 795f 6c69 7374 290d 0a0d 0a20 2020 2020  y_list)....     
+000138b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000138c0: 6d79 5f69 7465 6d20 3d3d 2030 2e30 3a0d  my_item == 0.0:.
+000138d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138e0: 2020 2020 2072 6574 7572 6e20 2230 220d       return "0".
+000138f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013900: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00013910: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013920: 726e 206d 795f 6974 656d 0d0a 0d0a 2020  rn my_item....  
+00013930: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
+00013940: 662e 6170 706c 796d 6170 286a 6f69 6e5f  f.applymap(join_
+00013950: 656c 656d 656e 7473 290d 0a0d 0a0d 0a0d  elements).......
+00013960: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00013970: 756d 206f 7665 7220 7468 6520 636f 6c75  um over the colu
+00013980: 6d6e 730d 0a0d 0a20 2020 2020 2020 2020  mns....         
+00013990: 2020 2064 6566 2065 7661 6c5f 7375 6d28     def eval_sum(
+000139a0: 636f 6c75 6d6e 293a 0d0a 2020 2020 2020  column):..      
+000139b0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+000139c0: 203d 205b 7374 7228 6329 2e72 6570 6c61   = [str(c).repla
+000139d0: 6365 2822 5e22 2c20 222a 2a22 2920 666f  ce("^", "**") fo
+000139e0: 7220 6320 696e 2063 6f6c 756d 6e5d 0d0a  r c in column]..
+000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a00: 6d79 5f65 7870 7220 3d20 222b 222e 6a6f  my_expr = "+".jo
+00013a10: 696e 2863 6f6c 756d 6e29 0d0a 2020 2020  in(column)..    
+00013a20: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00013a30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013a40: 2020 2020 2020 7265 7475 726e 2070 6172        return par
+00013a50: 7365 5f65 7870 7228 6d79 5f65 7870 7229  se_expr(my_expr)
+00013a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013a70: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00013a90: 6574 7572 6e20 6d79 5f65 7870 720d 0a0d  eturn my_expr...
+00013aa0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00013ab0: 2064 665b 2254 6f74 616c 225d 203d 2064   df["Total"] = d
+00013ac0: 662e 542e 6167 6728 6576 616c 5f73 756d  f.T.agg(eval_sum
+00013ad0: 2920 2023 2064 662e 542e 7375 6d28 290d  )  # df.T.sum().
+00013ae0: 0a20 2020 2020 2020 2020 2020 2064 662e  .            df.
+00013af0: 6c6f 635b 2254 6f74 616c 225d 203d 2064  loc["Total"] = d
+00013b00: 662e 6167 6728 6576 616c 5f73 756d 290d  f.agg(eval_sum).
+00013b10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00013b20: 6e74 2822 544f 5441 4c22 2c64 662e 6c6f  nt("TOTAL",df.lo
+00013b30: 635b 2254 6f74 616c 225d 290d 0a20 2020  c["Total"])..   
+00013b40: 2020 2020 2020 2020 2064 665f 6d65 7267           df_merg
+00013b50: 6532 5b22 546f 7461 6c22 5d20 3d20 6466  e2["Total"] = df
+00013b60: 5b22 546f 7461 6c22 5d0d 0a0d 0a20 2020  ["Total"]....   
+00013b70: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
+00013b80: 6865 206e 6577 2063 6f6c 756d 6e73 0d0a  he new columns..
+00013b90: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00013ba0: 6974 6572 6174 6520 7468 726f 7567 6820  iterate through 
+00013bb0: 7468 6520 636f 6c75 6d6e 730d 0a20 2020  the columns..   
+00013bc0: 2020 2020 2020 2020 2070 7269 6e74 2864           print(d
+00013bd0: 662e 636f 6c75 6d6e 7329 0d0a 0d0a 0d0a  f.columns)......
+00013be0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00013bf0: 636f 6c75 6d6e 2069 6e20 6466 2e63 6f6c  column in df.col
+00013c00: 756d 6e73 3a0d 0a20 2020 2020 2020 2020  umns:..         
+00013c10: 2020 2020 2020 2069 6620 636f 6c75 6d6e         if column
+00013c20: 5b30 5d20 213d 2022 546f 7461 6c22 3a0d  [0] != "Total":.
+00013c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c40: 2020 2020 2070 7269 6e74 2863 6f6c 756d       print(colum
+00013c50: 6e5b 305d 202b 2022 2022 2020 2b20 2228  n[0] + " "  + "(
+00013c60: 2573 2922 2025 2063 6f6c 756d 6e5b 315d  %s)" % column[1]
+00013c70: 2c64 662e 6c6f 635b 2254 6f74 616c 225d  ,df.loc["Total"]
+00013c80: 5b63 6f6c 756d 6e5d 290d 0a20 2020 2020  [column])..     
+00013c90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00013ca0: 665f 6d65 7267 6532 2e6c 6f63 5b22 546f  f_merge2.loc["To
+00013cb0: 7461 6c22 2c63 6f6c 756d 6e5b 305d 202b  tal",column[0] +
+00013cc0: 2022 2022 2020 2b20 2228 2573 2922 2025   " "  + "(%s)" %
+00013cd0: 2063 6f6c 756d 6e5b 315d 5d20 3d20 6466   column[1]] = df
+00013ce0: 2e6c 6f63 5b22 546f 7461 6c22 5d5b 636f  .loc["Total"][co
+00013cf0: 6c75 6d6e 5d0d 0a0d 0a0d 0a0d 0a20 2020  lumn]........   
+00013d00: 2020 2020 2020 2020 2064 6566 2073 696d           def sim
+00013d10: 706c 6966 795f 6578 7072 286d 795f 6974  plify_expr(my_it
+00013d20: 656d 293a 0d0a 2020 2020 2020 2020 2020  em):..          
+00013d30: 2020 2020 2020 7265 7475 726e 2073 696d        return sim
+00013d40: 706c 6966 7928 6d79 5f69 7465 6d29 0d0a  plify(my_item)..
+00013d50: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00013d60: 203d 2064 662e 6170 706c 796d 6170 2873   = df.applymap(s
+00013d70: 696d 706c 6966 795f 6578 7072 290d 0a0d  implify_expr)...
+00013d80: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00013d90: 666f 725f 6578 6365 6c20 3d20 6466 2e63  for_excel = df.c
+00013da0: 6f70 7928 290d 0a0d 0a0d 0a0d 0a20 2020  opy()........   
+00013db0: 2020 2020 2020 2020 2064 6566 2061 6262           def abb
+00013dc0: 7265 7669 6174 655f 7a65 726f 735f 6c61  reviate_zeros_la
+00013dd0: 7465 7828 6d79 5f69 7465 6d29 3a0d 0a20  tex(my_item):.. 
+00013de0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00013df0: 6620 6d79 5f69 7465 6d20 3d3d 2022 3022  f my_item == "0"
+00013e00: 206f 7220 6d79 5f69 7465 6d20 3d3d 2030   or my_item == 0
+00013e10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00013e20: 2020 2020 2020 2072 6574 7572 6e20 2220         return " 
+00013e30: 2e2d 2022 2020 2320 2e2d 2022 0d0a 2020  .- "  # .- "..  
+00013e40: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00013e50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00013e60: 2020 2020 2020 2020 2073 203d 2070 7269           s = pri
+00013e70: 6e74 696e 672e 6c61 7465 7828 6d79 5f69  nting.latex(my_i
+00013e80: 7465 6d20 2c6d 6f64 653d 2269 6e6c 696e  tem ,mode="inlin
+00013e90: 6522 2920 2320 206d 6f64 653d 2269 6e6c  e") #  mode="inl
+00013ea0: 696e 6522 290d 0a20 2020 2020 2020 2020  ine")..         
+00013eb0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00013ec0: 2873 290d 0a20 2020 2020 2020 2020 2020  (s)..           
+00013ed0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013ee0: 730d 0a0d 0a20 2020 2020 2020 2020 2020  s....           
+00013ef0: 2023 6466 5f62 6163 6b75 7020 3d20 6466   #df_backup = df
+00013f00: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00013f10: 2020 2020 2064 6620 3d20 6466 2e61 7070       df = df.app
+00013f20: 6c79 6d61 7028 6162 6272 6576 6961 7465  lymap(abbreviate
+00013f30: 5f7a 6572 6f73 5f6c 6174 6578 290d 0a0d  _zeros_latex)...
+00013f40: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00013f50: 2064 665f 6d65 7267 6532 203d 2064 665f   df_merge2 = df_
+00013f60: 6d65 7267 6532 2e72 6570 6c61 6365 286e  merge2.replace(n
+00013f70: 702e 6e61 6e2c 2027 272c 2072 6567 6578  p.nan, '', regex
+00013f80: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00013f90: 2020 2020 6466 5f6d 6572 6765 3220 3d20      df_merge2 = 
+00013fa0: 6466 5f6d 6572 6765 322e 7265 706c 6163  df_merge2.replac
+00013fb0: 6528 2230 222c 2027 272c 2072 6567 6578  e("0", '', regex
+00013fc0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00013fd0: 2020 2020 6466 5f6d 6572 6765 3220 3d20      df_merge2 = 
+00013fe0: 6466 5f6d 6572 6765 322e 7265 706c 6163  df_merge2.replac
+00013ff0: 6528 302c 2027 272c 2072 6567 6578 3d54  e(0, '', regex=T
+00014000: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00014010: 2020 6466 5f6d 6572 6765 3220 3d20 6466    df_merge2 = df
+00014020: 5f6d 6572 6765 322e 7265 706c 6163 6528  _merge2.replace(
+00014030: 302e 302c 2027 272c 2072 6567 6578 3d54  0.0, '', regex=T
+00014040: 7275 6529 0d0a 0d0a 2020 2020 2020 2020  rue)....        
+00014050: 2020 2020 2320 7072 696e 7428 6466 2e74      # print(df.t
+00014060: 6f5f 7374 7269 6e67 2829 290d 0a20 2020  o_string())..   
+00014070: 2020 2020 2020 2020 2023 2064 662e 696c           # df.il
+00014080: 6f63 5b30 2c30 5d20 3d20 2224 5c5c 616c  oc[0,0] = "$\\al
+00014090: 7068 6124 220d 0a0d 0a20 2020 2020 2020  pha$"....       
+000140a0: 2020 2020 2070 642e 6f70 7469 6f6e 732e       pd.options.
+000140b0: 6469 7370 6c61 792e 6d61 785f 636f 6c77  display.max_colw
+000140c0: 6964 7468 203d 204e 6f6e 650d 0a0d 0a20  idth = None.... 
+000140d0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+000140e0: 6465 203d 3d20 2268 746d 6c22 3a20 2320  de == "html": # 
+000140f0: 3c20 4e4f 5420 5945 5420 5355 5050 4f52  < NOT YET SUPPOR
+00014100: 5445 440d 0a0d 0a20 2020 2020 2020 2020  TED....         
+00014110: 2020 2020 2020 2064 665f 6874 6d6c 203d         df_html =
+00014120: 2022 2222 0d0a 2020 2020 2020 2020 3c68   """..        <h
+00014130: 746d 6c3e 0d0a 2020 2020 2020 2020 3c68  tml>..        <h
+00014140: 6561 643e 0d0a 2020 2020 2020 2020 3c74  ead>..        <t
+00014150: 6974 6c65 3e4d 6174 6865 6465 6d6f 3c2f  itle>Mathedemo</
+00014160: 7469 746c 653e 0d0a 2020 2020 2020 2020  title>..        
+00014170: 3c73 6372 6970 7420 7479 7065 3d22 7465  <script type="te
+00014180: 7874 2f78 2d6d 6174 686a 6178 2d63 6f6e  xt/x-mathjax-con
+00014190: 6669 6722 3e0d 0a20 2020 2020 2020 2020  fig">..         
+000141a0: 204d 6174 684a 6178 2e48 7562 2e43 6f6e   MathJax.Hub.Con
+000141b0: 6669 6728 7b74 6578 326a 6178 3a20 7b69  fig({tex2jax: {i
+000141c0: 6e6c 696e 654d 6174 683a 205b 5b27 2427  nlineMath: [['$'
+000141d0: 2c27 2427 5d2c 205b 275c 5c28 272c 275c  ,'$'], ['\\(','\
+000141e0: 5c29 275d 5d7d 7d29 3b0d 0a20 2020 2020  \)']]}});..     
+000141f0: 2020 203c 2f73 6372 6970 743e 0d0a 2020     </script>..  
+00014200: 2020 2020 2020 3c73 6372 6970 7420 7479        <script ty
+00014210: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00014220: 6970 7422 0d0a 2020 2020 2020 2020 2020  ipt"..          
+00014230: 7372 633d 2268 7474 703a 2f2f 6364 6e6a  src="http://cdnj
+00014240: 732e 636c 6f75 6466 6c61 7265 2e63 6f6d  s.cloudflare.com
+00014250: 2f61 6a61 782f 6c69 6273 2f6d 6174 686a  /ajax/libs/mathj
+00014260: 6178 2f32 2e37 2e31 2f4d 6174 684a 6178  ax/2.7.1/MathJax
+00014270: 2e6a 733f 636f 6e66 6967 3d54 6558 2d41  .js?config=TeX-A
+00014280: 4d53 2d4d 4d4c 5f48 544d 4c6f 724d 4d4c  MS-MML_HTMLorMML
+00014290: 223e 0d0a 2020 2020 2020 2020 3c2f 7363  ">..        </sc
+000142a0: 7269 7074 3e0d 0a20 2020 2020 2020 203c  ript>..        <
+000142b0: 6c69 6e6b 2072 656c 3d22 7374 796c 6573  link rel="styles
+000142c0: 6865 6574 2220 6872 6566 3d22 6d79 7374  heet" href="myst
+000142d0: 796c 652e 6373 7322 3e0d 0a20 2020 2020  yle.css">..     
+000142e0: 2020 203c 2f68 6561 643e 0d0a 0d0a 2020     </head>....  
+000142f0: 2020 2020 2020 3c62 6f64 793e 0d0a 2020        <body>..  
+00014300: 2020 2020 2020 2573 0d0a 2020 2020 2020        %s..      
+00014310: 2020 3c2f 626f 6479 3e0d 0a20 2020 2020    </body>..     
+00014320: 2020 203c 2f68 746d 6c3e 0d0a 2020 2020     </html>..    
+00014330: 2020 2020 2222 2225 2020 6466 2e74 6f5f      """%  df.to_
+00014340: 6874 6d6c 2829 0d0a 0d0a 2020 2020 2020  html()....      
+00014350: 2020 2020 2020 2020 2020 7061 6765 536f            pageSo
+00014360: 7572 6365 203d 2022 2222 0d0a 2020 2020  urce = """..    
 00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014380: 2020 2020 203c 626f 6479 3e0d 0a20 2020       <body>..   
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 2020 2020 2020 2020 2020 3c70 3e61 7364            <p>asd
-000143b0: 663c 2f70 3e0d 0a20 2020 2020 2020 2020  f</p>..         
+00014380: 2020 2020 2020 2020 203c 6874 6d6c 3e3c           <html><
+00014390: 6865 6164 3e0d 0a20 2020 2020 2020 2020  head>..         
+000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143b0: 2020 2020 3c2f 6865 6164 3e0d 0a20 2020      </head>..   
 000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143d0: 2020 2020 3c2f 626f 6479 3e3c 2f68 746d      </body></htm
-000143e0: 6c3e 0d0a 2020 2020 2020 2020 2020 2020  l>..            
-000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00014410: 2020 2020 2020 2020 2320 424c 410d 0a0d          # BLA...
-00014420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014430: 2023 2077 7269 7465 2070 6167 6520 736f   # write page so
-00014440: 7572 6365 2074 6f20 6874 6d6c 0d0a 2020  urce to html..  
-00014450: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014460: 2046 616c 7365 3a0d 0a20 2020 2020 2020   False:..       
-00014470: 2020 2020 2020 2020 2020 2020 2023 2044               # D
-00014480: 4550 5245 4349 4154 4544 0d0a 2020 2020  EPRECIATED..    
-00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144a0: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
-000144b0: 6972 6e61 6d65 286f 732e 7061 7468 2e61  irname(os.path.a
-000144c0: 6273 7061 7468 285f 5f66 696c 655f 5f29  bspath(__file__)
-000144d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000144e0: 2020 2020 2020 2066 696c 6520 3d20 6f70         file = op
-000144f0: 656e 286f 732e 7061 7468 2e6a 6f69 6e28  en(os.path.join(
-00014500: 7061 7468 2c22 6669 6c65 732f 6d79 6d61  path,"files/myma
-00014510: 7472 6978 2e68 746d 6c22 292c 2277 222c  trix.html"),"w",
-00014520: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-00014530: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014540: 2020 2020 2020 2066 696c 652e 7772 6974         file.writ
-00014550: 6528 6466 5f68 746d 6c29 0d0a 2020 2020  e(df_html)..    
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 6669 6c65 2e63 6c6f 7365 2829 0d0a 0d0a  file.close()....
-00014580: 2020 2020 2020 2020 2020 2020 2320 5144              # QD
-00014590: 6573 6b74 6f70 5365 7276 6963 6573 2e6f  esktopServices.o
-000145a0: 7065 6e55 726c 2851 5572 6c28 222e 2f66  penUrl(QUrl("./f
-000145b0: 696c 6573 2f6d 6174 7269 782e 6874 6d6c  iles/matrix.html
-000145c0: 2229 290d 0a0d 0a20 2020 2020 2020 2020  "))....         
-000145d0: 2020 2069 6620 6d6f 6465 203d 3d20 2273     if mode == "s
-000145e0: 7461 6e64 6172 6422 3a0d 0a20 2020 2020  tandard":..     
-000145f0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00014600: 203d 2050 616e 6461 734d 6f64 656c 2864   = PandasModel(d
-00014610: 665f 6d65 7267 6532 290d 0a20 2020 2020  f_merge2)..     
-00014620: 2020 2020 2020 2020 2020 206d 7669 6577             mview
-00014630: 203d 204d 6174 7269 7856 6965 7765 7228   = MatrixViewer(
-00014640: 6d6f 6465 6c2c 7061 7265 6e74 3d73 656c  model,parent=sel
-00014650: 6629 0d0a 0d0a 2020 2020 2020 2020 2020  f)....          
-00014660: 2020 2020 2020 2320 6d76 6965 772e 7765        # mview.we
-00014670: 6256 6965 772e 7365 7448 746d 6c28 6466  bView.setHtml(df
-00014680: 5f68 746d 6c29 0d0a 2020 2020 2020 2020  _html)..        
-00014690: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000146a0: 656c 662e 7465 7374 5f6d 6f64 653a 0d0a  elf.test_mode:..
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 2020 2020 6d76 6965 772e 7368 6f77 2829      mview.show()
-000146d0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-000146e0: 2020 6966 206d 6f64 6520 3d3d 2022 6c61    if mode == "la
-000146f0: 7465 7822 3a20 2320 3c20 4e4f 5420 5945  tex": # < NOT YE
-00014700: 5420 5355 5050 4f52 5445 440d 0a20 2020  T SUPPORTED..   
-00014710: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00014720: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00014730: 2020 2020 2020 2073 656c 662e 636f 6e76         self.conv
-00014740: 6572 745f 6466 5f74 6f5f 7465 7828 6466  ert_df_to_tex(df
-00014750: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014760: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00014770: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00014780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014790: 656c 662e 6e6f 7469 6679 2873 7472 2865  elf.notify(str(e
-000147a0: 292c 7469 746c 653d 2245 7272 6f72 2064  ),title="Error d
-000147b0: 7572 696e 6720 5465 7820 436f 6e76 6572  uring Tex Conver
-000147c0: 7369 6f6e 2229 0d0a 0d0a 2020 2020 2020  sion")....      
-000147d0: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
-000147e0: 7428 2256 4945 5722 290d 0a20 2020 2020  t("VIEW")..     
-000147f0: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
-00014800: 6e74 2864 665f 6874 6d6c 290d 0a0d 0a20  nt(df_html).... 
-00014810: 2020 2020 2020 2020 2020 2064 6566 2063             def c
-00014820: 6f6e 7665 7274 5f65 7863 656c 286d 795f  onvert_excel(my_
-00014830: 6974 656d 293a 0d0a 2020 2020 2020 2020  item):..        
-00014840: 2020 2020 2020 2020 6966 206d 795f 6974          if my_it
-00014850: 656d 203d 3d20 2230 2220 6f72 206d 795f  em == "0" or my_
-00014860: 6974 656d 203d 3d20 303a 0d0a 2020 2020  item == 0:..    
-00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014880: 7265 7475 726e 2022 202e 2d20 2220 2023  return " .- "  #
-00014890: 202e 2d20 220d 0a20 2020 2020 2020 2020   .- "..         
-000148a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2020 7320 3d20 7072 6574 7479 286d 795f    s = pretty(my_
-000148d0: 6974 656d 2920 2320 7072 696e 7469 6e67  item) # printing
-000148e0: 2e6c 6174 6578 286d 795f 6974 656d 2920  .latex(my_item) 
-000148f0: 2320 2c6d 6f64 653d 2269 6e6c 696e 6522  # ,mode="inline"
-00014900: 2920 2320 206d 6f64 653d 2269 6e6c 696e  ) #  mode="inlin
-00014910: 6522 290d 0a20 2020 2020 2020 2020 2020  e")..           
-00014920: 2020 2020 2020 2020 2070 7269 6e74 2873           print(s
-00014930: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014940: 2020 2020 2020 2072 6574 7572 6e20 730d         return s.
-00014950: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00014960: 6620 6d6f 6465 203d 3d20 2265 7863 656c  f mode == "excel
-00014970: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00014980: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00014990: 2020 2020 2020 2020 2020 2020 2020 6566                ef
-000149a0: 696c 656e 616d 6520 3d20 5146 696c 6544  ilename = QFileD
-000149b0: 6961 6c6f 672e 6765 7453 6176 6546 696c  ialog.getSaveFil
-000149c0: 654e 616d 6528 7365 6c66 2c20 2753 6176  eName(self, 'Sav
-000149d0: 6520 6669 6c65 272c 206f 732e 6765 7463  e file', os.getc
-000149e0: 7764 2829 2c20 2245 7863 656c 2046 696c  wd(), "Excel Fil
-000149f0: 6573 2028 2a2e 786c 7378 2922 295b 305d  es (*.xlsx)")[0]
-00014a00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014a10: 2020 2020 2020 2020 6966 2065 6669 6c65          if efile
-00014a20: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-00014a30: 2061 6e64 2065 6669 6c65 6e61 6d65 2021   and efilename !
-00014a40: 3d20 2222 3a0d 0a20 2020 2020 2020 2020  = "":..         
-00014a50: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00014a60: 665f 666f 725f 6578 6365 6c20 3d20 6466  f_for_excel = df
-00014a70: 5f66 6f72 5f65 7863 656c 2e61 7070 6c79  _for_excel.apply
-00014a80: 6d61 7028 636f 6e76 6572 745f 6578 6365  map(convert_exce
-00014a90: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
-00014aa0: 2020 2020 2020 2020 2020 2020 2320 7061              # pa
-00014ab0: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
-00014ac0: 6e61 6d65 286f 732e 7061 7468 2e61 6273  name(os.path.abs
-00014ad0: 7061 7468 285f 5f66 696c 655f 5f29 290d  path(__file__)).
-00014ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014af0: 2020 2020 2020 2020 2064 665f 666f 725f           df_for_
-00014b00: 6578 6365 6c2e 746f 5f65 7863 656c 2865  excel.to_excel(e
-00014b10: 6669 6c65 6e61 6d65 2920 2320 2266 696c  filename) # "fil
-00014b20: 6573 2f46 6c6f 774d 6174 7269 785f 666f  es/FlowMatrix_fo
-00014b30: 726d 6174 7465 642e 786c 7378 2229 290d  rmatted.xlsx")).
-00014b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b50: 2020 2020 2020 2020 2023 2064 665f 6d65           # df_me
-00014b60: 7267 6532 2e74 6f5f 6578 6365 6c28 6f73  rge2.to_excel(os
-00014b70: 2e70 6174 682e 6a6f 696e 2870 6174 682c  .path.join(path,
-00014b80: 6566 696c 656e 616d 6529 2920 2020 2023  efilename))    #
-00014b90: 2022 6669 6c65 732f 466c 6f77 4d61 7472   "files/FlowMatr
-00014ba0: 6978 2e78 6c73 7822 2929 0d0a 0d0a 2020  ix.xlsx"))....  
-00014bb0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00014bc0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00014bd0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-00014be0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00014bf0: 6f74 6966 7928 7374 7228 6529 2c20 7469  otify(str(e), ti
-00014c00: 746c 653d 2245 7272 6f72 2064 7572 696e  tle="Error durin
-00014c10: 6720 4578 6365 6c20 636f 6e76 6572 7369  g Excel conversi
-00014c20: 6f6e 2229 0d0a 0d0a 2020 2020 2020 2020  on")....        
-00014c30: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00014c40: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00014c50: 2020 2020 7365 6c66 2e6e 6f74 6966 7928      self.notify(
-00014c60: 7374 7228 6529 2c20 7469 746c 653d 2245  str(e), title="E
-00014c70: 7272 6f72 2064 7572 696e 6720 6d61 7472  rror during matr
-00014c80: 6978 2067 656e 6572 6174 696f 6e22 290d  ix generation").
-00014c90: 0a0d 0a20 2020 2064 6566 2072 656d 6f76  ...    def remov
-00014ca0: 655f 6974 656d 2873 656c 6629 3a0d 0a0d  e_item(self):...
-00014cb0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00014cc0: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00014cd0: 7465 645f 726f 7773 203d 2073 6f72 7465  ted_rows = sorte
-00014ce0: 6428 7365 7428 696e 6465 782e 726f 7728  d(set(index.row(
-00014cf0: 2920 666f 7220 696e 6465 7820 696e 0d0a  ) for index in..
-00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d20: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
-00014d30: 7361 6374 696f 6e56 6965 772e 7365 6c65  sactionView.sele
-00014d40: 6374 6564 496e 6465 7865 7328 2929 290d  ctedIndexes())).
-00014d50: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00014d60: 6620 6c65 6e28 7365 6c65 6374 6564 5f72  f len(selected_r
-00014d70: 6f77 7329 203d 3d20 303a 0d0a 2020 2020  ows) == 0:..    
-00014d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014d90: 2e6e 6f74 6966 7928 226e 6f20 7365 6c65  .notify("no sele
-00014da0: 6374 6564 2072 6f77 7322 2c74 6974 6c65  cted rows",title
-00014db0: 3d22 4572 726f 7222 290d 0a20 2020 2020  ="Error")..     
-00014dc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014dd0: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
-00014de0: 2073 656c 6563 7469 6f6e 203d 2073 656c   selection = sel
-00014df0: 6563 7465 645f 726f 7773 5b30 5d0d 0a0d  ected_rows[0]...
-00014e00: 0a20 2020 2020 2020 2020 2020 2079 6573  .            yes
-00014e10: 203d 2020 7365 6c66 2e61 736b 5f71 7565   =  self.ask_que
-00014e20: 7374 696f 6e28 2727 2c22 4172 6520 796f  stion('',"Are yo
-00014e30: 7520 7375 7265 2079 6f75 2077 616e 7420  u sure you want 
-00014e40: 746f 2072 656d 6f76 6520 7468 6520 656e  to remove the en
-00014e50: 7472 7920 2725 7327 3f22 2573 656c 662e  try '%s'?"%self.
-00014e60: 656e 7472 795f 6461 7461 5b73 656c 6563  entry_data[selec
-00014e70: 7469 6f6e 5d5b 2273 7562 6a65 6374 225d  tion]["subject"]
-00014e80: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00014e90: 6620 7965 733a 0d0a 0d0a 2020 2020 2020  f yes:....      
-00014ea0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00014eb0: 7261 7763 616e 7661 732e 7265 6d6f 7665  rawcanvas.remove
-00014ec0: 5f63 6f6e 6e65 6374 696f 6e28 7365 6c66  _connection(self
-00014ed0: 2e65 6e74 7279 5f64 6174 615b 7365 6c65  .entry_data[sele
-00014ee0: 6374 696f 6e5d 5b22 7368 6f72 746e 616d  ction]["shortnam
-00014ef0: 6522 5d29 0d0a 0d0a 2020 2020 2020 2020  e"])....        
-00014f00: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00014f10: 6e73 6163 7469 6f6e 5669 6577 2e72 656d  nsactionView.rem
-00014f20: 6f76 6552 6f77 2873 656c 6563 7469 6f6e  oveRow(selection
-00014f30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014f40: 2020 2064 656c 2073 656c 662e 656e 7472     del self.entr
-00014f50: 795f 6461 7461 5b73 656c 6563 7469 6f6e  y_data[selection
-00014f60: 5d0d 0a0d 0a20 2020 2020 2020 2065 7863  ]....        exc
-00014f70: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00014f80: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
-00014f90: 2073 656c 662e 6e6f 7469 6679 2873 7472   self.notify(str
-00014fa0: 2865 292c 2074 6974 6c65 3d22 4572 726f  (e), title="Erro
-00014fb0: 7222 290d 0a0d 0a20 2020 2020 2020 2074  r")....        t
-00014fc0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00014fd0: 2073 656c 662e 7570 6461 7465 5f74 6162   self.update_tab
-00014fe0: 6c65 2829 0d0a 0d0a 2020 2020 2020 2020  le()....        
-00014ff0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00015000: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00015010: 2020 2020 7365 6c66 2e6e 6f74 6966 7928      self.notify(
-00015020: 7374 7228 6529 2c20 7469 746c 653d 2245  str(e), title="E
-00015030: 7272 6f72 2229 0d0a 0d0a 0d0a 2020 2020  rror")......    
-00015040: 6465 6620 636f 6e76 6572 745f 6466 5f74  def convert_df_t
-00015050: 6f5f 7465 7828 7365 6c66 2c64 6629 3a0d  o_tex(self,df):.
-00015060: 0a0d 0a20 2020 2020 2020 2064 6566 2077  ...        def w
-00015070: 7261 7073 7472 696e 6728 7329 3a0d 0a20  rapstring(s):.. 
-00015080: 2020 2020 2020 2020 2020 2023 2077 7261             # wra
-00015090: 7073 2073 7472 696e 670d 0a20 2020 2020  ps string..     
-000150a0: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
-000150b0: 7874 7772 6170 2e77 7261 7028 732c 2077  xtwrap.wrap(s, w
-000150c0: 6964 7468 3d31 3029 0d0a 0d0a 2020 2020  idth=10)....    
-000150d0: 2020 2020 6465 6620 6162 6272 6576 6961      def abbrevia
-000150e0: 7465 5f7a 6572 6f73 286d 795f 6974 656d  te_zeros(my_item
-000150f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00015100: 6966 206d 795f 6974 656d 203d 3d20 2230  if my_item == "0
-00015110: 2220 6f72 206d 795f 6974 656d 203d 3d20  " or my_item == 
-00015120: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00015130: 2020 2020 7265 7475 726e 2022 202e 2d20      return " .- 
-00015140: 2220 2023 202e 2d20 220d 0a20 2020 2020  "  # .- "..     
-00015150: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00015160: 2020 2020 2020 2020 2020 2020 2020 6d79                my
-00015170: 5f69 7465 6d20 3d20 7374 7228 6d79 5f69  _item = str(my_i
-00015180: 7465 6d29 0d0a 2020 2020 2020 2020 2020  tem)..          
-00015190: 2020 2020 2020 6d61 785f 6c65 6e20 3d20        max_len = 
-000151a0: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
-000151b0: 2020 2020 6966 206c 656e 286d 795f 6974      if len(my_it
-000151c0: 656d 2920 3e20 6d61 785f 6c65 6e3a 0d0a  em) > max_len:..
-000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151e0: 2020 2020 7265 7475 726e 206d 795f 6974      return my_it
-000151f0: 656d 5b3a 6d61 785f 6c65 6e5d 202b 2022  em[:max_len] + "
-00015200: 2e2e 2e22 0d0a 2020 2020 2020 2020 2020  ..."..          
-00015210: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015230: 2072 6574 7572 6e20 6d79 5f69 7465 6d0d   return my_item.
-00015240: 0a0d 0a20 2020 2020 2020 2064 665f 6261  ...        df_ba
-00015250: 636b 7570 203d 2064 662e 636f 7079 2829  ckup = df.copy()
-00015260: 0d0a 0d0a 2020 2020 2020 2020 6466 5f6c  ....        df_l
-00015270: 6174 6578 203d 2064 662e 746f 5f6c 6174  atex = df.to_lat
-00015280: 6578 286c 6f6e 6774 6162 6c65 3d46 616c  ex(longtable=Fal
-00015290: 7365 2c20 6573 6361 7065 3d46 616c 7365  se, escape=False
-000152a0: 292e 7265 706c 6163 6528 22ce 9422 2c20  ).replace("..", 
-000152b0: 2224 5c44 656c 7461 2422 290d 0a0d 0a20  "$\Delta$").... 
-000152c0: 2020 2020 2020 2064 665f 6c61 7465 7820         df_latex 
-000152d0: 3d20 6466 5f6c 6174 6578 2e72 6570 6c61  = df_latex.repla
-000152e0: 6365 2822 5c5c 6265 6769 6e7b 7461 6275  ce("\\begin{tabu
-000152f0: 6c61 727d 222c 2022 5c5c 6265 6769 6e7b  lar}", "\\begin{
-00015300: 7461 6275 6c61 7278 7d7b 5c5c 7465 7874  tabularx}{\\text
-00015310: 7769 6474 687d 2229 0d0a 2020 2020 2020  width}")..      
-00015320: 2020 6466 5f6c 6174 6578 203d 2064 665f    df_latex = df_
-00015330: 6c61 7465 782e 7265 706c 6163 6528 225c  latex.replace("\
-00015340: 5c65 6e64 7b74 6162 756c 6172 7d22 2c20  \end{tabular}", 
-00015350: 225c 5c65 6e64 7b74 6162 756c 6172 787d  "\\end{tabularx}
-00015360: 2229 0d0a 2020 2020 2020 2020 6466 5f6c  ")..        df_l
-00015370: 6174 6578 203d 2022 5c5c 6265 6769 6e7b  atex = "\\begin{
-00015380: 736d 616c 6c7d 5c6e 2220 2b20 6466 5f6c  small}\n" + df_l
-00015390: 6174 6578 202b 2022 5c6e 5c65 6e64 7b73  atex + "\n\end{s
-000153a0: 6d61 6c6c 7d22 0d0a 0d0a 2020 2020 2020  mall}"....      
-000153b0: 2020 6466 5f6c 6174 6578 203d 2064 665f    df_latex = df_
-000153c0: 6c61 7465 782e 7265 706c 6163 6528 225c  latex.replace("\
-000153d0: 5c6c 6566 7428 222c 2022 2822 290d 0a20  \left(", "(").. 
-000153e0: 2020 2020 2020 2064 665f 6c61 7465 7820         df_latex 
-000153f0: 3d20 6466 5f6c 6174 6578 2e72 6570 6c61  = df_latex.repla
-00015400: 6365 2822 5c5c 7269 6768 7429 222c 2022  ce("\\right)", "
-00015410: 2922 290d 0a0d 0a20 2020 2020 2020 2064  )")....        d
-00015420: 665f 6c61 7465 7820 3d20 6466 5f6c 6174  f_latex = df_lat
-00015430: 6578 2e72 6570 6c61 6365 2822 7b6c 222c  ex.replace("{l",
-00015440: 2022 7b4c 7b33 636d 7d22 290d 0a0d 0a20   "{L{3cm}").... 
-00015450: 2020 2020 2020 2064 665f 6c61 7465 7820         df_latex 
-00015460: 3d20 2222 220d 0a5c 5c64 6f63 756d 656e  = """..\\documen
-00015470: 7463 6c61 7373 5b61 3370 6170 6572 2c6c  tclass[a3paper,l
-00015480: 616e 6473 6361 7065 5d7b 6172 7469 636c  andscape]{articl
-00015490: 657d 0d0a 5c5c 7573 6570 6163 6b61 6765  e}..\\usepackage
-000154a0: 7b62 6f6f 6b74 6162 737d 0d0a 5c5c 7573  {booktabs}..\\us
-000154b0: 6570 6163 6b61 6765 7b61 646a 7573 7462  epackage{adjustb
-000154c0: 6f78 7d0d 0a5c 5c75 7365 7061 636b 6167  ox}..\\usepackag
-000154d0: 655b 7461 626c 655d 7b78 636f 6c6f 727d  e[table]{xcolor}
-000154e0: 0d0a 5c5c 7573 6570 6163 6b61 6765 7b6c  ..\\usepackage{l
-000154f0: 6f6e 6774 6162 6c65 7d0d 0a5c 5c75 7365  ongtable}..\\use
-00015500: 7061 636b 6167 657b 7461 6275 6c61 7278  package{tabularx
-00015510: 2c72 6167 6765 6432 657d 0d0a 5c5c 6465  ,ragged2e}..\\de
-00015520: 6669 6e65 636f 6c6f 727b 4772 6179 7d7b  finecolor{Gray}{
-00015530: 6772 6179 7d7b 302e 3930 7d0d 0a5c 5c64  gray}{0.90}..\\d
-00015540: 6566 696e 6563 6f6c 6f72 7b4c 6967 6874  efinecolor{Light
-00015550: 4772 6179 7d7b 6772 6179 7d7b 302e 3935  Gray}{gray}{0.95
-00015560: 7d0d 0a5c 5c64 6566 696e 6563 6f6c 6f72  }..\\definecolor
-00015570: 7b57 6869 7465 7d7b 7267 627d 7b31 2c31  {White}{rgb}{1,1
-00015580: 2c31 7d0d 0a0d 0a5c 5c6e 6577 636f 6c75  ,1}....\\newcolu
-00015590: 6d6e 7479 7065 7b67 7d7b 3e7b 5c5c 636f  mntype{g}{>{\\co
-000155a0: 6c75 6d6e 636f 6c6f 727b 5768 6974 657d  lumncolor{White}
-000155b0: 5c5c 6172 7261 7962 6163 6b73 6c61 7368  \\arraybackslash
-000155c0: 7d4c 7d20 250d 0a5c 5c6e 6577 636f 6c75  }L} %..\\newcolu
-000155d0: 6d6e 7479 7065 7b6c 7d7b 3e7b 5c5c 636f  mntype{l}{>{\\co
-000155e0: 6c75 6d6e 636f 6c6f 727b 5768 6974 657d  lumncolor{White}
-000155f0: 5c5c 6172 7261 7962 6163 6b73 6c61 7368  \\arraybackslash
-00015600: 7d70 7b33 636d 7d7d 2025 6365 6e74 6572  }p{3cm}} %center
-00015610: 6564 2022 5822 2063 6f6c 756d 6e0d 0a5c  ed "X" column..\
-00015620: 5c6e 6577 636f 6c75 6d6e 7479 7065 7b4c  \newcolumntype{L
-00015630: 7d5b 315d 7b3e 7b5c 5c72 6167 6765 6472  }[1]{>{\\raggedr
-00015640: 6967 6874 5c5c 6172 7261 7962 6163 6b73  ight\\arraybacks
-00015650: 6c61 7368 7d70 7b5c 5c64 696d 6578 7072  lash}p{\\dimexpr
-00015660: 2331 2d32 5c5c 7461 6263 6f6c 7365 702d  #1-2\\tabcolsep-
-00015670: 325c 5c61 7272 6179 7275 6c65 7769 6474  2\\arrayrulewidt
-00015680: 682b 2e32 3170 747d 7d0d 0a0d 0a5c 5c75  h+.21pt}}....\\u
-00015690: 7365 7061 636b 6167 655b 6c65 6674 3d31  sepackage[left=1
-000156a0: 636d 2c72 6967 6874 3d31 2e35 636d 5d7b  cm,right=1.5cm]{
-000156b0: 6765 6f6d 6574 7279 7d0d 0a0d 0a5c 5c62  geometry}....\\b
-000156c0: 6567 696e 7b64 6f63 756d 656e 747d 5c6e  egin{document}\n
-000156d0: 2222 2220 2b20 6466 5f6c 6174 6578 2020  """ + df_latex  
-000156e0: 202b 2022 5c6e 5c5c 656e 647b 646f 6375   + "\n\\end{docu
-000156f0: 6d65 6e74 7d22 0d0a 0d0a 2020 2020 2020  ment}"....      
-00015700: 2020 7079 7065 7263 6c69 702e 636f 7079    pyperclip.copy
-00015710: 2864 665f 6c61 7465 7829 0d0a 2020 2020  (df_latex)..    
-00015720: 2020 2020 2373 656c 662e 6e6f 7469 6679      #self.notify
-00015730: 286d 6573 7361 6765 3d22 4c61 5465 5820  (message="LaTeX 
-00015740: 636f 6465 2063 6f70 6965 6420 746f 2063  code copied to c
-00015750: 6c69 7062 6f61 7264 2e20 4861 7665 2066  lipboard. Have f
-00015760: 756e 2122 2c20 7469 746c 653d 2248 6176  un!", title="Hav
-00015770: 6520 6675 6e22 290d 0a20 2020 2020 2020  e fun")..       
-00015780: 2073 656c 662e 7374 6174 7573 4261 7228   self.statusBar(
-00015790: 292e 7368 6f77 4d65 7373 6167 6528 224c  ).showMessage("L
-000157a0: 6154 6558 2063 6f64 6520 636f 7069 6564  aTeX code copied
-000157b0: 2074 6f20 636c 6970 626f 6172 642e 2048   to clipboard. H
-000157c0: 6176 6520 6675 6e21 2229 0d0a 0d0a 0d0a  ave fun!")......
-000157d0: 2020 2020 2020 2020 2320 2d2d 2d2d 2d2d          # ------
-000157e0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-000157f0: 2069 6620 4661 6c73 653a 2023 2044 4550   if False: # DEP
-00015800: 5249 4341 5445 440d 0a20 2020 2020 2020  RICATED..       
-00015810: 2020 2020 2074 7279 3a0d 0a0d 0a20 2020       try:....   
-00015820: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-00015830: 6d20 7064 666c 6174 6578 2069 6d70 6f72  m pdflatex impor
-00015840: 7420 5044 464c 6154 6558 0d0a 2020 2020  t PDFLaTeX..    
-00015850: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00015860: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00015870: 6d65 286f 732e 7061 7468 2e61 6273 7061  me(os.path.abspa
-00015880: 7468 285f 5f66 696c 655f 5f29 290d 0a20  th(__file__)).. 
-00015890: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000158a0: 795f 6669 6c65 203d 206f 732e 7061 7468  y_file = os.path
-000158b0: 2e6a 6f69 6e28 7061 7468 2c22 6d79 6d61  .join(path,"myma
-000158c0: 7472 6978 2229 0d0a 0d0a 2020 2020 2020  trix")....      
-000158d0: 2020 2020 2020 2020 2020 6669 6c65 203d            file =
-000158e0: 206f 7065 6e28 6d79 5f66 696c 652c 2022   open(my_file, "
-000158f0: 7722 290d 0a20 2020 2020 2020 2020 2020  w")..           
-00015900: 2020 2020 2066 696c 652e 7772 6974 6528       file.write(
-00015910: 2222 220d 0a20 2020 2020 2020 205c 5c64  """..        \\d
-00015920: 6f63 756d 656e 7463 6c61 7373 5b61 3370  ocumentclass[a3p
-00015930: 6170 6572 2c6c 616e 6473 6361 7065 5d7b  aper,landscape]{
-00015940: 6172 7469 636c 657d 0d0a 2020 2020 2020  article}..      
-00015950: 2020 5c5c 7573 6570 6163 6b61 6765 7b62    \\usepackage{b
-00015960: 6f6f 6b74 6162 737d 0d0a 2020 2020 2020  ooktabs}..      
-00015970: 2020 5c5c 7573 6570 6163 6b61 6765 7b61    \\usepackage{a
-00015980: 646a 7573 7462 6f78 7d0d 0a20 2020 2020  djustbox}..     
-00015990: 2020 205c 5c75 7365 7061 636b 6167 655b     \\usepackage[
-000159a0: 7461 626c 655d 7b78 636f 6c6f 727d 0d0a  table]{xcolor}..
-000159b0: 2020 2020 2020 2020 5c5c 7573 6570 6163          \\usepac
-000159c0: 6b61 6765 7b6c 6f6e 6774 6162 6c65 7d0d  kage{longtable}.
-000159d0: 0a20 2020 2020 2020 205c 5c75 7365 7061  .        \\usepa
-000159e0: 636b 6167 657b 7461 6275 6c61 7278 2c72  ckage{tabularx,r
-000159f0: 6167 6765 6432 657d 0d0a 2020 2020 2020  agged2e}..      
-00015a00: 2020 5c5c 6465 6669 6e65 636f 6c6f 727b    \\definecolor{
-00015a10: 4772 6179 7d7b 6772 6179 7d7b 302e 3930  Gray}{gray}{0.90
-00015a20: 7d0d 0a20 2020 2020 2020 205c 5c64 6566  }..        \\def
-00015a30: 696e 6563 6f6c 6f72 7b4c 6967 6874 4772  inecolor{LightGr
-00015a40: 6179 7d7b 6772 6179 7d7b 302e 3935 7d0d  ay}{gray}{0.95}.
-00015a50: 0a20 2020 2020 2020 205c 5c64 6566 696e  .        \\defin
-00015a60: 6563 6f6c 6f72 7b57 6869 7465 7d7b 7267  ecolor{White}{rg
-00015a70: 627d 7b31 2c31 2c31 7d0d 0a0d 0a20 2020  b}{1,1,1}....   
-00015a80: 2020 2020 205c 5c6e 6577 636f 6c75 6d6e       \\newcolumn
-00015a90: 7479 7065 7b67 7d7b 3e7b 5c5c 636f 6c75  type{g}{>{\\colu
-00015aa0: 6d6e 636f 6c6f 727b 5768 6974 657d 5c5c  mncolor{White}\\
-00015ab0: 6172 7261 7962 6163 6b73 6c61 7368 7d4c  arraybackslash}L
-00015ac0: 7d20 250d 0a20 2020 2020 2020 205c 5c6e  } %..        \\n
-00015ad0: 6577 636f 6c75 6d6e 7479 7065 7b6c 7d7b  ewcolumntype{l}{
-00015ae0: 3e7b 5c5c 636f 6c75 6d6e 636f 6c6f 727b  >{\\columncolor{
-00015af0: 5768 6974 657d 5c5c 6172 7261 7962 6163  White}\\arraybac
-00015b00: 6b73 6c61 7368 7d70 7b33 636d 7d7d 2025  kslash}p{3cm}} %
-00015b10: 6365 6e74 6572 6564 2022 5822 2063 6f6c  centered "X" col
-00015b20: 756d 6e0d 0a20 2020 2020 2020 205c 5c6e  umn..        \\n
-00015b30: 6577 636f 6c75 6d6e 7479 7065 7b4c 7d5b  ewcolumntype{L}[
-00015b40: 315d 7b3e 7b5c 5c72 6167 6765 6472 6967  1]{>{\\raggedrig
-00015b50: 6874 5c5c 6172 7261 7962 6163 6b73 6c61  ht\\arraybacksla
-00015b60: 7368 7d70 7b5c 5c64 696d 6578 7072 2331  sh}p{\\dimexpr#1
-00015b70: 2d32 5c5c 7461 6263 6f6c 7365 702d 325c  -2\\tabcolsep-2\
-00015b80: 5c61 7272 6179 7275 6c65 7769 6474 682b  \arrayrulewidth+
-00015b90: 2e32 3170 747d 7d0d 0a0d 0a20 2020 2020  .21pt}}....     
-00015ba0: 2020 205c 5c75 7365 7061 636b 6167 655b     \\usepackage[
-00015bb0: 6c65 6674 3d31 636d 2c72 6967 6874 3d31  left=1cm,right=1
-00015bc0: 2e35 636d 5d7b 6765 6f6d 6574 7279 7d0d  .5cm]{geometry}.
-00015bd0: 0a0d 0a20 2020 2020 2020 205c 5c62 6567  ...        \\beg
-00015be0: 696e 7b64 6f63 756d 656e 747d 2222 2229  in{document}""")
-00015bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015c00: 2020 6669 6c65 2e77 7269 7465 2864 665f    file.write(df_
-00015c10: 6c61 7465 7829 0d0a 2020 2020 2020 2020  latex)..        
-00015c20: 2020 2020 2020 2020 6669 6c65 2e77 7269          file.wri
-00015c30: 7465 2822 2222 0d0a 2020 2020 2020 2020  te("""..        
-00015c40: 5c5c 656e 647b 646f 6375 6d65 6e74 7d22  \\end{document}"
-00015c50: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
-00015c60: 2020 2020 2066 696c 652e 636c 6f73 6528       file.close(
-00015c70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015c80: 2020 2023 2070 6466 6c20 3d20 5044 464c     # pdfl = PDFL
-00015c90: 6154 6558 2e66 726f 6d5f 7465 7866 696c  aTeX.from_texfil
-00015ca0: 6528 276d 795f 7465 7866 696c 652e 7465  e('my_texfile.te
-00015cb0: 7827 290d 0a20 2020 2020 2020 2020 2020  x')..           
-00015cc0: 2020 2020 2023 2070 6466 2c20 6c6f 672c       # pdf, log,
-00015cd0: 2063 6f6d 706c 6574 6564 5f70 726f 6365   completed_proce
-00015ce0: 7373 203d 2070 6466 6c2e 6372 6561 7465  ss = pdfl.create
-00015cf0: 5f70 6466 286b 6565 705f 7064 665f 6669  _pdf(keep_pdf_fi
-00015d00: 6c65 3d54 7275 652c 206b 6565 705f 6c6f  le=True, keep_lo
-00015d10: 675f 6669 6c65 3d54 7275 6529 0d0a 2020  g_file=True)..  
-00015d20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00015d30: 6f73 2e70 6f70 656e 2822 7064 666c 6174  os.popen("pdflat
-00015d40: 6578 2025 7322 2025 2028 6f73 2e67 6574  ex %s" % (os.get
-00015d50: 6377 6428 292b 222f 6d79 5f74 6578 6669  cwd()+"/my_texfi
-00015d60: 6c65 2e74 6578 2229 290d 0a20 2020 2020  le.tex"))..     
-00015d70: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
-00015d80: 7420 7375 6270 726f 6365 7373 0d0a 2020  t subprocess..  
-00015d90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00015da0: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
-00015db0: 6e61 6d65 286f 732e 7061 7468 2e61 6273  name(os.path.abs
-00015dc0: 7061 7468 285f 5f66 696c 655f 5f29 290d  path(__file__)).
-00015dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015de0: 2073 7562 7072 6f63 6573 732e 7275 6e28   subprocess.run(
-00015df0: 2270 6466 6c61 7465 7820 2573 2220 2520  "pdflatex %s" % 
-00015e00: 286f 732e 7061 7468 2e6a 6f69 6e28 7061  (os.path.join(pa
-00015e10: 7468 2c22 6d79 6d61 7472 6978 2e74 6578  th,"mymatrix.tex
-00015e20: 2229 2929 2e63 6865 636b 5f72 6574 7572  "))).check_retur
-00015e30: 6e63 6f64 6528 290d 0a0d 0a20 2020 2020  ncode()....     
-00015e40: 2020 2020 2020 2020 2020 2023 6f73 2e73             #os.s
-00015e50: 7461 7274 6669 6c65 286f 732e 6765 7463  tartfile(os.getc
-00015e60: 7764 2829 202b 2022 5c5c 6d79 6d61 7472  wd() + "\\mymatr
-00015e70: 6978 2e70 6466 2229 0d0a 2020 2020 2020  ix.pdf")..      
-00015e80: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+000143d0: 2020 2020 2020 2020 2020 3c62 6f64 793e            <body>
+000143e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000143f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00014400: 703e 6173 6466 3c2f 703e 0d0a 2020 2020  p>asdf</p>..    
+00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014420: 2020 2020 2020 2020 203c 2f62 6f64 793e           </body>
+00014430: 3c2f 6874 6d6c 3e0d 0a20 2020 2020 2020  </html>..       
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
+00014460: 2020 2020 2020 2020 2020 2020 2023 2042               # B
+00014470: 4c41 0d0a 0d0a 2020 2020 2020 2020 2020  LA....          
+00014480: 2020 2020 2020 2320 7772 6974 6520 7061        # write pa
+00014490: 6765 2073 6f75 7263 6520 746f 2068 746d  ge source to htm
+000144a0: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
+000144b0: 2020 2069 6620 4661 6c73 653a 0d0a 2020     if False:..  
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144d0: 2020 2320 4445 5052 4543 4941 5445 440d    # DEPRECIATED.
+000144e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000144f0: 2020 2020 2070 6174 6820 3d20 6f73 2e70       path = os.p
+00014500: 6174 682e 6469 726e 616d 6528 6f73 2e70  ath.dirname(os.p
+00014510: 6174 682e 6162 7370 6174 6828 5f5f 6669  ath.abspath(__fi
+00014520: 6c65 5f5f 2929 0d0a 2020 2020 2020 2020  le__))..        
+00014530: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00014540: 203d 206f 7065 6e28 6f73 2e70 6174 682e   = open(os.path.
+00014550: 6a6f 696e 2870 6174 682c 2266 696c 6573  join(path,"files
+00014560: 2f6d 796d 6174 7269 782e 6874 6d6c 2229  /mymatrix.html")
+00014570: 2c22 7722 2c65 6e63 6f64 696e 673d 2775  ,"w",encoding='u
+00014580: 7466 2d38 2729 0d0a 2020 2020 2020 2020  tf-8')..        
+00014590: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+000145a0: 2e77 7269 7465 2864 665f 6874 6d6c 290d  .write(df_html).
+000145b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145c0: 2020 2020 2066 696c 652e 636c 6f73 6528       file.close(
+000145d0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000145e0: 2023 2051 4465 736b 746f 7053 6572 7669   # QDesktopServi
+000145f0: 6365 732e 6f70 656e 5572 6c28 5155 726c  ces.openUrl(QUrl
+00014600: 2822 2e2f 6669 6c65 732f 6d61 7472 6978  ("./files/matrix
+00014610: 2e68 746d 6c22 2929 0d0a 0d0a 2020 2020  .html"))....    
+00014620: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00014630: 3d3d 2022 7374 616e 6461 7264 223a 0d0a  == "standard":..
+00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014650: 6d6f 6465 6c20 3d20 5061 6e64 6173 4d6f  model = PandasMo
+00014660: 6465 6c28 6466 5f6d 6572 6765 3229 0d0a  del(df_merge2)..
+00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014680: 6d76 6965 7720 3d20 4d61 7472 6978 5669  mview = MatrixVi
+00014690: 6577 6572 286d 6f64 656c 2c70 6172 656e  ewer(model,paren
+000146a0: 743d 7365 6c66 290d 0a0d 0a20 2020 2020  t=self)....     
+000146b0: 2020 2020 2020 2020 2020 2023 206d 7669             # mvi
+000146c0: 6577 2e77 6562 5669 6577 2e73 6574 4874  ew.webView.setHt
+000146d0: 6d6c 2864 665f 6874 6d6c 290d 0a20 2020  ml(df_html)..   
+000146e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000146f0: 6e6f 7420 7365 6c66 2e74 6573 745f 6d6f  not self.test_mo
+00014700: 6465 3a0d 0a20 2020 2020 2020 2020 2020  de:..           
+00014710: 2020 2020 2020 2020 206d 7669 6577 2e73           mview.s
+00014720: 686f 7728 290d 0a0d 0a0d 0a20 2020 2020  how()......     
+00014730: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+00014740: 3d20 226c 6174 6578 223a 2023 203c 204e  = "latex": # < N
+00014750: 4f54 2059 4554 2053 5550 504f 5254 4544  OT YET SUPPORTED
+00014760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014770: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00014780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014790: 2e63 6f6e 7665 7274 5f64 665f 746f 5f74  .convert_df_to_t
+000147a0: 6578 2864 6629 0d0a 2020 2020 2020 2020  ex(df)..        
+000147b0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+000147c0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147e0: 2020 2020 7365 6c66 2e6e 6f74 6966 7928      self.notify(
+000147f0: 7374 7228 6529 2c74 6974 6c65 3d22 4572  str(e),title="Er
+00014800: 726f 7220 6475 7269 6e67 2054 6578 2043  ror during Tex C
+00014810: 6f6e 7665 7273 696f 6e22 290d 0a0d 0a20  onversion").... 
+00014820: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00014830: 2070 7269 6e74 2822 5649 4557 2229 0d0a   print("VIEW")..
+00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014850: 2320 7072 696e 7428 6466 5f68 746d 6c29  # print(df_html)
+00014860: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014870: 6465 6620 636f 6e76 6572 745f 6578 6365  def convert_exce
+00014880: 6c28 6d79 5f69 7465 6d29 3a0d 0a20 2020  l(my_item):..   
+00014890: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000148a0: 6d79 5f69 7465 6d20 3d3d 2022 3022 206f  my_item == "0" o
+000148b0: 7220 6d79 5f69 7465 6d20 3d3d 2030 3a0d  r my_item == 0:.
+000148c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000148d0: 2020 2020 2072 6574 7572 6e20 2220 2e2d       return " .-
+000148e0: 2022 2020 2320 2e2d 2022 0d0a 2020 2020   "  # .- "..    
+000148f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00014900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014910: 2020 2020 2020 2073 203d 2070 7265 7474         s = prett
+00014920: 7928 6d79 5f69 7465 6d29 2023 2070 7269  y(my_item) # pri
+00014930: 6e74 696e 672e 6c61 7465 7828 6d79 5f69  nting.latex(my_i
+00014940: 7465 6d29 2023 202c 6d6f 6465 3d22 696e  tem) # ,mode="in
+00014950: 6c69 6e65 2229 2023 2020 6d6f 6465 3d22  line") #  mode="
+00014960: 696e 6c69 6e65 2229 0d0a 2020 2020 2020  inline")..      
+00014970: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00014980: 696e 7428 7329 0d0a 2020 2020 2020 2020  int(s)..        
+00014990: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000149a0: 726e 2073 0d0a 0d0a 2020 2020 2020 2020  rn s....        
+000149b0: 2020 2020 6966 206d 6f64 6520 3d3d 2022      if mode == "
+000149c0: 6578 6365 6c22 3a0d 0a20 2020 2020 2020  excel":..       
+000149d0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149f0: 2020 2065 6669 6c65 6e61 6d65 203d 2051     efilename = Q
+00014a00: 4669 6c65 4469 616c 6f67 2e67 6574 5361  FileDialog.getSa
+00014a10: 7665 4669 6c65 4e61 6d65 2873 656c 662c  veFileName(self,
+00014a20: 2027 5361 7665 2066 696c 6527 2c20 6f73   'Save file', os
+00014a30: 2e67 6574 6377 6428 292c 2022 4578 6365  .getcwd(), "Exce
+00014a40: 6c20 4669 6c65 7320 282a 2e78 6c73 7829  l Files (*.xlsx)
+00014a50: 2229 5b30 5d0d 0a0d 0a20 2020 2020 2020  ")[0]....       
+00014a60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014a70: 6566 696c 656e 616d 6520 6973 206e 6f74  efilename is not
+00014a80: 204e 6f6e 6520 616e 6420 6566 696c 656e   None and efilen
+00014a90: 616d 6520 213d 2022 223a 0d0a 2020 2020  ame != "":..    
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ab0: 2020 2020 6466 5f66 6f72 5f65 7863 656c      df_for_excel
+00014ac0: 203d 2064 665f 666f 725f 6578 6365 6c2e   = df_for_excel.
+00014ad0: 6170 706c 796d 6170 2863 6f6e 7665 7274  applymap(convert
+00014ae0: 5f65 7863 656c 290d 0a20 2020 2020 2020  _excel)..       
+00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b00: 2023 2070 6174 6820 3d20 6f73 2e70 6174   # path = os.pat
+00014b10: 682e 6469 726e 616d 6528 6f73 2e70 6174  h.dirname(os.pat
+00014b20: 682e 6162 7370 6174 6828 5f5f 6669 6c65  h.abspath(__file
+00014b30: 5f5f 2929 0d0a 2020 2020 2020 2020 2020  __))..          
+00014b40: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00014b50: 5f66 6f72 5f65 7863 656c 2e74 6f5f 6578  _for_excel.to_ex
+00014b60: 6365 6c28 6566 696c 656e 616d 6529 2023  cel(efilename) #
+00014b70: 2022 6669 6c65 732f 466c 6f77 4d61 7472   "files/FlowMatr
+00014b80: 6978 5f66 6f72 6d61 7474 6564 2e78 6c73  ix_formatted.xls
+00014b90: 7822 2929 0d0a 2020 2020 2020 2020 2020  x"))..          
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00014bb0: 6466 5f6d 6572 6765 322e 746f 5f65 7863  df_merge2.to_exc
+00014bc0: 656c 286f 732e 7061 7468 2e6a 6f69 6e28  el(os.path.join(
+00014bd0: 7061 7468 2c65 6669 6c65 6e61 6d65 2929  path,efilename))
+00014be0: 2020 2020 2320 2266 696c 6573 2f46 6c6f      # "files/Flo
+00014bf0: 774d 6174 7269 782e 786c 7378 2229 290d  wMatrix.xlsx")).
+00014c00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00014c10: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00014c20: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014c40: 656c 662e 6e6f 7469 6679 2873 7472 2865  elf.notify(str(e
+00014c50: 292c 2074 6974 6c65 3d22 4572 726f 7220  ), title="Error 
+00014c60: 6475 7269 6e67 2045 7863 656c 2063 6f6e  during Excel con
+00014c70: 7665 7273 696f 6e22 290d 0a0d 0a20 2020  version")....   
+00014c80: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00014c90: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+00014ca0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00014cb0: 7469 6679 2873 7472 2865 292c 2074 6974  tify(str(e), tit
+00014cc0: 6c65 3d22 4572 726f 7220 6475 7269 6e67  le="Error during
+00014cd0: 206d 6174 7269 7820 6765 6e65 7261 7469   matrix generati
+00014ce0: 6f6e 2229 0d0a 0d0a 2020 2020 6465 6620  on")....    def 
+00014cf0: 7265 6d6f 7665 5f69 7465 6d28 7365 6c66  remove_item(self
+00014d00: 293a 0d0a 0d0a 2020 2020 2020 2020 7472  ):....        tr
+00014d10: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00014d20: 7365 6c65 6374 6564 5f72 6f77 7320 3d20  selected_rows = 
+00014d30: 736f 7274 6564 2873 6574 2869 6e64 6578  sorted(set(index
+00014d40: 2e72 6f77 2829 2066 6f72 2069 6e64 6578  .row() for index
+00014d50: 2069 6e0d 0a20 2020 2020 2020 2020 2020   in..           
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014d80: 2e74 7261 6e73 6163 7469 6f6e 5669 6577  .transactionView
+00014d90: 2e73 656c 6563 7465 6449 6e64 6578 6573  .selectedIndexes
+00014da0: 2829 2929 0d0a 0d0a 2020 2020 2020 2020  ()))....        
+00014db0: 2020 2020 6966 206c 656e 2873 656c 6563      if len(selec
+00014dc0: 7465 645f 726f 7773 2920 3d3d 2030 3a0d  ted_rows) == 0:.
+00014dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014de0: 2073 656c 662e 6e6f 7469 6679 2822 6e6f   self.notify("no
+00014df0: 2073 656c 6563 7465 6420 726f 7773 222c   selected rows",
+00014e00: 7469 746c 653d 2245 7272 6f72 2229 0d0a  title="Error")..
+00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e20: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
+00014e30: 2020 2020 2020 7365 6c65 6374 696f 6e20        selection 
+00014e40: 3d20 7365 6c65 6374 6564 5f72 6f77 735b  = selected_rows[
+00014e50: 305d 0d0a 0d0a 2020 2020 2020 2020 2020  0]....          
+00014e60: 2020 7965 7320 3d20 2073 656c 662e 6173    yes =  self.as
+00014e70: 6b5f 7175 6573 7469 6f6e 2827 272c 2241  k_question('',"A
+00014e80: 7265 2079 6f75 2073 7572 6520 796f 7520  re you sure you 
+00014e90: 7761 6e74 2074 6f20 7265 6d6f 7665 2074  want to remove t
+00014ea0: 6865 2065 6e74 7279 2027 2573 273f 2225  he entry '%s'?"%
+00014eb0: 7365 6c66 2e65 6e74 7279 5f64 6174 615b  self.entry_data[
+00014ec0: 7365 6c65 6374 696f 6e5d 5b22 7375 626a  selection]["subj
+00014ed0: 6563 7422 5d29 0d0a 2020 2020 2020 2020  ect"])..        
+00014ee0: 2020 2020 6966 2079 6573 3a0d 0a0d 0a20      if yes:.... 
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014f00: 656c 662e 6472 6177 6361 6e76 6173 2e72  elf.drawcanvas.r
+00014f10: 656d 6f76 655f 636f 6e6e 6563 7469 6f6e  emove_connection
+00014f20: 2873 656c 662e 656e 7472 795f 6461 7461  (self.entry_data
+00014f30: 5b73 656c 6563 7469 6f6e 5d5b 2273 686f  [selection]["sho
+00014f40: 7274 6e61 6d65 225d 290d 0a0d 0a20 2020  rtname"])....   
+00014f50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014f60: 662e 7472 616e 7361 6374 696f 6e56 6965  f.transactionVie
+00014f70: 772e 7265 6d6f 7665 526f 7728 7365 6c65  w.removeRow(sele
+00014f80: 6374 696f 6e29 0d0a 2020 2020 2020 2020  ction)..        
+00014f90: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
+00014fa0: 2e65 6e74 7279 5f64 6174 615b 7365 6c65  .entry_data[sele
+00014fb0: 6374 696f 6e5d 0d0a 0d0a 2020 2020 2020  ction]....      
+00014fc0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00014fd0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+00014fe0: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+00014ff0: 7928 7374 7228 6529 2c20 7469 746c 653d  y(str(e), title=
+00015000: 2245 7272 6f72 2229 0d0a 0d0a 2020 2020  "Error")....    
+00015010: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00015020: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+00015030: 655f 7461 626c 6528 290d 0a0d 0a20 2020  e_table()....   
+00015040: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00015050: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+00015060: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015070: 7469 6679 2873 7472 2865 292c 2074 6974  tify(str(e), tit
+00015080: 6c65 3d22 4572 726f 7222 290d 0a0d 0a0d  le="Error").....
+00015090: 0a20 2020 2064 6566 2063 6f6e 7665 7274  .    def convert
+000150a0: 5f64 665f 746f 5f74 6578 2873 656c 662c  _df_to_tex(self,
+000150b0: 6466 293a 0d0a 0d0a 2020 2020 2020 2020  df):....        
+000150c0: 6465 6620 7772 6170 7374 7269 6e67 2873  def wrapstring(s
+000150d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000150e0: 2320 7772 6170 7320 7374 7269 6e67 0d0a  # wraps string..
+000150f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015100: 726e 2074 6578 7477 7261 702e 7772 6170  rn textwrap.wrap
+00015110: 2873 2c20 7769 6474 683d 3130 290d 0a0d  (s, width=10)...
+00015120: 0a20 2020 2020 2020 2064 6566 2061 6262  .        def abb
+00015130: 7265 7669 6174 655f 7a65 726f 7328 6d79  reviate_zeros(my
+00015140: 5f69 7465 6d29 3a0d 0a20 2020 2020 2020  _item):..       
+00015150: 2020 2020 2069 6620 6d79 5f69 7465 6d20       if my_item 
+00015160: 3d3d 2022 3022 206f 7220 6d79 5f69 7465  == "0" or my_ite
+00015170: 6d20 3d3d 2030 3a0d 0a20 2020 2020 2020  m == 0:..       
+00015180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015190: 2220 2e2d 2022 2020 2320 2e2d 2022 0d0a  " .- "  # .- "..
+000151a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000151b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000151c0: 2020 206d 795f 6974 656d 203d 2073 7472     my_item = str
+000151d0: 286d 795f 6974 656d 290d 0a20 2020 2020  (my_item)..     
+000151e0: 2020 2020 2020 2020 2020 206d 6178 5f6c             max_l
+000151f0: 656e 203d 2031 300d 0a20 2020 2020 2020  en = 10..       
+00015200: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00015210: 6d79 5f69 7465 6d29 203e 206d 6178 5f6c  my_item) > max_l
+00015220: 656e 3a0d 0a20 2020 2020 2020 2020 2020  en:..           
+00015230: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015240: 6d79 5f69 7465 6d5b 3a6d 6178 5f6c 656e  my_item[:max_len
+00015250: 5d20 2b20 222e 2e2e 220d 0a20 2020 2020  ] + "..."..     
+00015260: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00015270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015280: 2020 2020 2020 7265 7475 726e 206d 795f        return my_
+00015290: 6974 656d 0d0a 0d0a 2020 2020 2020 2020  item....        
+000152a0: 6466 5f62 6163 6b75 7020 3d20 6466 2e63  df_backup = df.c
+000152b0: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
+000152c0: 2064 665f 6c61 7465 7820 3d20 6466 2e74   df_latex = df.t
+000152d0: 6f5f 6c61 7465 7828 6c6f 6e67 7461 626c  o_latex(longtabl
+000152e0: 653d 4661 6c73 652c 2065 7363 6170 653d  e=False, escape=
+000152f0: 4661 6c73 6529 2e72 6570 6c61 6365 2822  False).replace("
+00015300: ce94 222c 2022 245c 4465 6c74 6124 2229  ..", "$\Delta$")
+00015310: 0d0a 0d0a 2020 2020 2020 2020 6466 5f6c  ....        df_l
+00015320: 6174 6578 203d 2064 665f 6c61 7465 782e  atex = df_latex.
+00015330: 7265 706c 6163 6528 225c 5c62 6567 696e  replace("\\begin
+00015340: 7b74 6162 756c 6172 7d22 2c20 225c 5c62  {tabular}", "\\b
+00015350: 6567 696e 7b74 6162 756c 6172 787d 7b5c  egin{tabularx}{\
+00015360: 5c74 6578 7477 6964 7468 7d22 290d 0a20  \textwidth}").. 
+00015370: 2020 2020 2020 2064 665f 6c61 7465 7820         df_latex 
+00015380: 3d20 6466 5f6c 6174 6578 2e72 6570 6c61  = df_latex.repla
+00015390: 6365 2822 5c5c 656e 647b 7461 6275 6c61  ce("\\end{tabula
+000153a0: 727d 222c 2022 5c5c 656e 647b 7461 6275  r}", "\\end{tabu
+000153b0: 6c61 7278 7d22 290d 0a20 2020 2020 2020  larx}")..       
+000153c0: 2064 665f 6c61 7465 7820 3d20 225c 5c62   df_latex = "\\b
+000153d0: 6567 696e 7b73 6d61 6c6c 7d5c 6e22 202b  egin{small}\n" +
+000153e0: 2064 665f 6c61 7465 7820 2b20 225c 6e5c   df_latex + "\n\
+000153f0: 656e 647b 736d 616c 6c7d 220d 0a0d 0a20  end{small}".... 
+00015400: 2020 2020 2020 2064 665f 6c61 7465 7820         df_latex 
+00015410: 3d20 6466 5f6c 6174 6578 2e72 6570 6c61  = df_latex.repla
+00015420: 6365 2822 5c5c 6c65 6674 2822 2c20 2228  ce("\\left(", "(
+00015430: 2229 0d0a 2020 2020 2020 2020 6466 5f6c  ")..        df_l
+00015440: 6174 6578 203d 2064 665f 6c61 7465 782e  atex = df_latex.
+00015450: 7265 706c 6163 6528 225c 5c72 6967 6874  replace("\\right
+00015460: 2922 2c20 2229 2229 0d0a 0d0a 2020 2020  )", ")")....    
+00015470: 2020 2020 6466 5f6c 6174 6578 203d 2064      df_latex = d
+00015480: 665f 6c61 7465 782e 7265 706c 6163 6528  f_latex.replace(
+00015490: 227b 6c22 2c20 227b 4c7b 3363 6d7d 2229  "{l", "{L{3cm}")
+000154a0: 0d0a 0d0a 2020 2020 2020 2020 6466 5f6c  ....        df_l
+000154b0: 6174 6578 203d 2022 2222 0d0a 5c5c 646f  atex = """..\\do
+000154c0: 6375 6d65 6e74 636c 6173 735b 6133 7061  cumentclass[a3pa
+000154d0: 7065 722c 6c61 6e64 7363 6170 655d 7b61  per,landscape]{a
+000154e0: 7274 6963 6c65 7d0d 0a5c 5c75 7365 7061  rticle}..\\usepa
+000154f0: 636b 6167 657b 626f 6f6b 7461 6273 7d0d  ckage{booktabs}.
+00015500: 0a5c 5c75 7365 7061 636b 6167 657b 6164  .\\usepackage{ad
+00015510: 6a75 7374 626f 787d 0d0a 5c5c 7573 6570  justbox}..\\usep
+00015520: 6163 6b61 6765 5b74 6162 6c65 5d7b 7863  ackage[table]{xc
+00015530: 6f6c 6f72 7d0d 0a5c 5c75 7365 7061 636b  olor}..\\usepack
+00015540: 6167 657b 6c6f 6e67 7461 626c 657d 0d0a  age{longtable}..
+00015550: 5c5c 7573 6570 6163 6b61 6765 7b74 6162  \\usepackage{tab
+00015560: 756c 6172 782c 7261 6767 6564 3265 7d0d  ularx,ragged2e}.
+00015570: 0a5c 5c64 6566 696e 6563 6f6c 6f72 7b47  .\\definecolor{G
+00015580: 7261 797d 7b67 7261 797d 7b30 2e39 307d  ray}{gray}{0.90}
+00015590: 0d0a 5c5c 6465 6669 6e65 636f 6c6f 727b  ..\\definecolor{
+000155a0: 4c69 6768 7447 7261 797d 7b67 7261 797d  LightGray}{gray}
+000155b0: 7b30 2e39 357d 0d0a 5c5c 6465 6669 6e65  {0.95}..\\define
+000155c0: 636f 6c6f 727b 5768 6974 657d 7b72 6762  color{White}{rgb
+000155d0: 7d7b 312c 312c 317d 0d0a 0d0a 5c5c 6e65  }{1,1,1}....\\ne
+000155e0: 7763 6f6c 756d 6e74 7970 657b 677d 7b3e  wcolumntype{g}{>
+000155f0: 7b5c 5c63 6f6c 756d 6e63 6f6c 6f72 7b57  {\\columncolor{W
+00015600: 6869 7465 7d5c 5c61 7272 6179 6261 636b  hite}\\arrayback
+00015610: 736c 6173 687d 4c7d 2025 0d0a 5c5c 6e65  slash}L} %..\\ne
+00015620: 7763 6f6c 756d 6e74 7970 657b 6c7d 7b3e  wcolumntype{l}{>
+00015630: 7b5c 5c63 6f6c 756d 6e63 6f6c 6f72 7b57  {\\columncolor{W
+00015640: 6869 7465 7d5c 5c61 7272 6179 6261 636b  hite}\\arrayback
+00015650: 736c 6173 687d 707b 3363 6d7d 7d20 2563  slash}p{3cm}} %c
+00015660: 656e 7465 7265 6420 2258 2220 636f 6c75  entered "X" colu
+00015670: 6d6e 0d0a 5c5c 6e65 7763 6f6c 756d 6e74  mn..\\newcolumnt
+00015680: 7970 657b 4c7d 5b31 5d7b 3e7b 5c5c 7261  ype{L}[1]{>{\\ra
+00015690: 6767 6564 7269 6768 745c 5c61 7272 6179  ggedright\\array
+000156a0: 6261 636b 736c 6173 687d 707b 5c5c 6469  backslash}p{\\di
+000156b0: 6d65 7870 7223 312d 325c 5c74 6162 636f  mexpr#1-2\\tabco
+000156c0: 6c73 6570 2d32 5c5c 6172 7261 7972 756c  lsep-2\\arrayrul
+000156d0: 6577 6964 7468 2b2e 3231 7074 7d7d 0d0a  ewidth+.21pt}}..
+000156e0: 0d0a 5c5c 7573 6570 6163 6b61 6765 5b6c  ..\\usepackage[l
+000156f0: 6566 743d 3163 6d2c 7269 6768 743d 312e  eft=1cm,right=1.
+00015700: 3563 6d5d 7b67 656f 6d65 7472 797d 0d0a  5cm]{geometry}..
+00015710: 0d0a 5c5c 6265 6769 6e7b 646f 6375 6d65  ..\\begin{docume
+00015720: 6e74 7d5c 6e22 2222 202b 2064 665f 6c61  nt}\n""" + df_la
+00015730: 7465 7820 2020 2b20 225c 6e5c 5c65 6e64  tex   + "\n\\end
+00015740: 7b64 6f63 756d 656e 747d 220d 0a0d 0a20  {document}".... 
+00015750: 2020 2020 2020 2070 7970 6572 636c 6970         pyperclip
+00015760: 2e63 6f70 7928 6466 5f6c 6174 6578 290d  .copy(df_latex).
+00015770: 0a20 2020 2020 2020 2023 7365 6c66 2e6e  .        #self.n
+00015780: 6f74 6966 7928 6d65 7373 6167 653d 224c  otify(message="L
+00015790: 6154 6558 2063 6f64 6520 636f 7069 6564  aTeX code copied
+000157a0: 2074 6f20 636c 6970 626f 6172 642e 2048   to clipboard. H
+000157b0: 6176 6520 6675 6e21 222c 2074 6974 6c65  ave fun!", title
+000157c0: 3d22 4861 7665 2066 756e 2229 0d0a 2020  ="Have fun")..  
+000157d0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+000157e0: 7342 6172 2829 2e73 686f 774d 6573 7361  sBar().showMessa
+000157f0: 6765 2822 4c61 5465 5820 636f 6465 2063  ge("LaTeX code c
+00015800: 6f70 6965 6420 746f 2063 6c69 7062 6f61  opied to clipboa
+00015810: 7264 2e20 4861 7665 2066 756e 2122 290d  rd. Have fun!").
+00015820: 0a0d 0a0d 0a20 2020 2020 2020 2023 202d  .....        # -
+00015830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020  ------------..  
+00015840: 2020 2020 2020 6966 2046 616c 7365 3a20        if False: 
+00015850: 2320 4445 5052 4943 4154 4544 0d0a 2020  # DEPRICATED..  
+00015860: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00015870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015880: 2020 6672 6f6d 2070 6466 6c61 7465 7820    from pdflatex 
+00015890: 696d 706f 7274 2050 4446 4c61 5465 580d  import PDFLaTeX.
+000158a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158b0: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
+000158c0: 6469 726e 616d 6528 6f73 2e70 6174 682e  dirname(os.path.
+000158d0: 6162 7370 6174 6828 5f5f 6669 6c65 5f5f  abspath(__file__
+000158e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000158f0: 2020 2020 6d79 5f66 696c 6520 3d20 6f73      my_file = os
+00015900: 2e70 6174 682e 6a6f 696e 2870 6174 682c  .path.join(path,
+00015910: 226d 796d 6174 7269 7822 290d 0a0d 0a20  "mymatrix").... 
+00015920: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015930: 696c 6520 3d20 6f70 656e 286d 795f 6669  ile = open(my_fi
+00015940: 6c65 2c20 2277 2229 0d0a 2020 2020 2020  le, "w")..      
+00015950: 2020 2020 2020 2020 2020 6669 6c65 2e77            file.w
+00015960: 7269 7465 2822 2222 0d0a 2020 2020 2020  rite("""..      
+00015970: 2020 5c5c 646f 6375 6d65 6e74 636c 6173    \\documentclas
+00015980: 735b 6133 7061 7065 722c 6c61 6e64 7363  s[a3paper,landsc
+00015990: 6170 655d 7b61 7274 6963 6c65 7d0d 0a20  ape]{article}.. 
+000159a0: 2020 2020 2020 205c 5c75 7365 7061 636b         \\usepack
+000159b0: 6167 657b 626f 6f6b 7461 6273 7d0d 0a20  age{booktabs}.. 
+000159c0: 2020 2020 2020 205c 5c75 7365 7061 636b         \\usepack
+000159d0: 6167 657b 6164 6a75 7374 626f 787d 0d0a  age{adjustbox}..
+000159e0: 2020 2020 2020 2020 5c5c 7573 6570 6163          \\usepac
+000159f0: 6b61 6765 5b74 6162 6c65 5d7b 7863 6f6c  kage[table]{xcol
+00015a00: 6f72 7d0d 0a20 2020 2020 2020 205c 5c75  or}..        \\u
+00015a10: 7365 7061 636b 6167 657b 6c6f 6e67 7461  sepackage{longta
+00015a20: 626c 657d 0d0a 2020 2020 2020 2020 5c5c  ble}..        \\
+00015a30: 7573 6570 6163 6b61 6765 7b74 6162 756c  usepackage{tabul
+00015a40: 6172 782c 7261 6767 6564 3265 7d0d 0a20  arx,ragged2e}.. 
+00015a50: 2020 2020 2020 205c 5c64 6566 696e 6563         \\definec
+00015a60: 6f6c 6f72 7b47 7261 797d 7b67 7261 797d  olor{Gray}{gray}
+00015a70: 7b30 2e39 307d 0d0a 2020 2020 2020 2020  {0.90}..        
+00015a80: 5c5c 6465 6669 6e65 636f 6c6f 727b 4c69  \\definecolor{Li
+00015a90: 6768 7447 7261 797d 7b67 7261 797d 7b30  ghtGray}{gray}{0
+00015aa0: 2e39 357d 0d0a 2020 2020 2020 2020 5c5c  .95}..        \\
+00015ab0: 6465 6669 6e65 636f 6c6f 727b 5768 6974  definecolor{Whit
+00015ac0: 657d 7b72 6762 7d7b 312c 312c 317d 0d0a  e}{rgb}{1,1,1}..
+00015ad0: 0d0a 2020 2020 2020 2020 5c5c 6e65 7763  ..        \\newc
+00015ae0: 6f6c 756d 6e74 7970 657b 677d 7b3e 7b5c  olumntype{g}{>{\
+00015af0: 5c63 6f6c 756d 6e63 6f6c 6f72 7b57 6869  \columncolor{Whi
+00015b00: 7465 7d5c 5c61 7272 6179 6261 636b 736c  te}\\arraybacksl
+00015b10: 6173 687d 4c7d 2025 0d0a 2020 2020 2020  ash}L} %..      
+00015b20: 2020 5c5c 6e65 7763 6f6c 756d 6e74 7970    \\newcolumntyp
+00015b30: 657b 6c7d 7b3e 7b5c 5c63 6f6c 756d 6e63  e{l}{>{\\columnc
+00015b40: 6f6c 6f72 7b57 6869 7465 7d5c 5c61 7272  olor{White}\\arr
+00015b50: 6179 6261 636b 736c 6173 687d 707b 3363  aybackslash}p{3c
+00015b60: 6d7d 7d20 2563 656e 7465 7265 6420 2258  m}} %centered "X
+00015b70: 2220 636f 6c75 6d6e 0d0a 2020 2020 2020  " column..      
+00015b80: 2020 5c5c 6e65 7763 6f6c 756d 6e74 7970    \\newcolumntyp
+00015b90: 657b 4c7d 5b31 5d7b 3e7b 5c5c 7261 6767  e{L}[1]{>{\\ragg
+00015ba0: 6564 7269 6768 745c 5c61 7272 6179 6261  edright\\arrayba
+00015bb0: 636b 736c 6173 687d 707b 5c5c 6469 6d65  ckslash}p{\\dime
+00015bc0: 7870 7223 312d 325c 5c74 6162 636f 6c73  xpr#1-2\\tabcols
+00015bd0: 6570 2d32 5c5c 6172 7261 7972 756c 6577  ep-2\\arrayrulew
+00015be0: 6964 7468 2b2e 3231 7074 7d7d 0d0a 0d0a  idth+.21pt}}....
+00015bf0: 2020 2020 2020 2020 5c5c 7573 6570 6163          \\usepac
+00015c00: 6b61 6765 5b6c 6566 743d 3163 6d2c 7269  kage[left=1cm,ri
+00015c10: 6768 743d 312e 3563 6d5d 7b67 656f 6d65  ght=1.5cm]{geome
+00015c20: 7472 797d 0d0a 0d0a 2020 2020 2020 2020  try}....        
+00015c30: 5c5c 6265 6769 6e7b 646f 6375 6d65 6e74  \\begin{document
+00015c40: 7d22 2222 290d 0a20 2020 2020 2020 2020  }""")..         
+00015c50: 2020 2020 2020 2066 696c 652e 7772 6974         file.writ
+00015c60: 6528 6466 5f6c 6174 6578 290d 0a20 2020  e(df_latex)..   
+00015c70: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00015c80: 652e 7772 6974 6528 2222 220d 0a20 2020  e.write("""..   
+00015c90: 2020 2020 205c 5c65 6e64 7b64 6f63 756d       \\end{docum
+00015ca0: 656e 747d 2222 2229 0d0a 2020 2020 2020  ent}""")..      
+00015cb0: 2020 2020 2020 2020 2020 6669 6c65 2e63            file.c
+00015cc0: 6c6f 7365 2829 0d0a 2020 2020 2020 2020  lose()..        
+00015cd0: 2020 2020 2020 2020 2320 7064 666c 203d          # pdfl =
+00015ce0: 2050 4446 4c61 5465 582e 6672 6f6d 5f74   PDFLaTeX.from_t
+00015cf0: 6578 6669 6c65 2827 6d79 5f74 6578 6669  exfile('my_texfi
+00015d00: 6c65 2e74 6578 2729 0d0a 2020 2020 2020  le.tex')..      
+00015d10: 2020 2020 2020 2020 2020 2320 7064 662c            # pdf,
+00015d20: 206c 6f67 2c20 636f 6d70 6c65 7465 645f   log, completed_
+00015d30: 7072 6f63 6573 7320 3d20 7064 666c 2e63  process = pdfl.c
+00015d40: 7265 6174 655f 7064 6628 6b65 6570 5f70  reate_pdf(keep_p
+00015d50: 6466 5f66 696c 653d 5472 7565 2c20 6b65  df_file=True, ke
+00015d60: 6570 5f6c 6f67 5f66 696c 653d 5472 7565  ep_log_file=True
+00015d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015d80: 2020 2023 206f 732e 706f 7065 6e28 2270     # os.popen("p
+00015d90: 6466 6c61 7465 7820 2573 2220 2520 286f  dflatex %s" % (o
+00015da0: 732e 6765 7463 7764 2829 2b22 2f6d 795f  s.getcwd()+"/my_
+00015db0: 7465 7866 696c 652e 7465 7822 2929 0d0a  texfile.tex"))..
+00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015dd0: 696d 706f 7274 2073 7562 7072 6f63 6573  import subproces
+00015de0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00015df0: 2020 2070 6174 6820 3d20 6f73 2e70 6174     path = os.pat
+00015e00: 682e 6469 726e 616d 6528 6f73 2e70 6174  h.dirname(os.pat
+00015e10: 682e 6162 7370 6174 6828 5f5f 6669 6c65  h.abspath(__file
+00015e20: 5f5f 2929 0d0a 2020 2020 2020 2020 2020  __))..          
+00015e30: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+00015e40: 2e72 756e 2822 7064 666c 6174 6578 2025  .run("pdflatex %
+00015e50: 7322 2025 2028 6f73 2e70 6174 682e 6a6f  s" % (os.path.jo
+00015e60: 696e 2870 6174 682c 226d 796d 6174 7269  in(path,"mymatri
+00015e70: 782e 7465 7822 2929 292e 6368 6563 6b5f  x.tex"))).check_
+00015e80: 7265 7475 726e 636f 6465 2829 0d0a 0d0a  returncode()....
 00015e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ea0: 2020 2020 2320 7368 7574 696c 2e72 6d74      # shutil.rmt
-00015eb0: 7265 6528 6f73 2e67 6574 6377 6428 292b  ree(os.getcwd()+
-00015ec0: 225c 5c66 696c 6573 2229 0d0a 2020 2020  "\\files")..    
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 2320 6f73 2e6d 6b64 6972 286f 732e 6765  # os.mkdir(os.ge
-00015ef0: 7463 7764 2829 2b22 5c5c 6669 6c65 7322  tcwd()+"\\files"
-00015f00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00015f10: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-00015f20: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00015f30: 6f73 2e70 6174 682e 6162 7370 6174 6828  os.path.abspath(
-00015f40: 5f5f 6669 6c65 5f5f 2929 0d0a 2020 2020  __file__))..    
-00015f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f60: 7368 7574 696c 2e6d 6f76 6528 7061 7468  shutil.move(path
-00015f70: 2b22 5c5c 6d79 6d61 7472 6978 2e74 6578  +"\\mymatrix.tex
-00015f80: 2220 2c20 7061 7468 2b20 225c 5c66 696c  " , path+ "\\fil
-00015f90: 6573 5c5c 6d79 6d61 7472 6978 2e74 6578  es\\mymatrix.tex
-00015fa0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00015fb0: 2020 2020 2020 2020 7368 7574 696c 2e6d          shutil.m
-00015fc0: 6f76 6528 7061 7468 202b 2022 5c5c 6d79  ove(path + "\\my
-00015fd0: 6d61 7472 6978 2e6c 6f67 222c 2070 6174  matrix.log", pat
-00015fe0: 6820 2b20 225c 5c66 696c 6573 5c5c 6d79  h + "\\files\\my
-00015ff0: 6d61 7472 6978 2e6c 6f67 2229 0d0a 2020  matrix.log")..  
-00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016010: 2020 7368 7574 696c 2e6d 6f76 6528 7061    shutil.move(pa
-00016020: 7468 202b 2022 5c5c 6d79 6d61 7472 6978  th + "\\mymatrix
-00016030: 2e61 7578 222c 2070 6174 6820 2b20 225c  .aux", path + "\
-00016040: 5c66 696c 6573 5c5c 5c6d 796d 6174 7269  \files\\\mymatri
-00016050: 782e 6175 7822 290d 0a20 2020 2020 2020  x.aux")..       
-00016060: 2020 2020 2020 2020 2020 2020 2073 6875               shu
-00016070: 7469 6c2e 6d6f 7665 2870 6174 6820 2b20  til.move(path + 
-00016080: 225c 5c6d 796d 6174 7269 782e 7064 6622  "\\mymatrix.pdf"
-00016090: 2c20 7061 7468 202b 2022 5c5c 6669 6c65  , path + "\\file
-000160a0: 735c 5c6d 796d 6174 7269 782e 7064 6622  s\\mymatrix.pdf"
-000160b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000160c0: 2020 2020 2020 2023 7368 7574 696c 2e63         #shutil.c
-000160d0: 6f70 7928 6f73 2e67 6574 6377 6428 2920  opy(os.getcwd() 
-000160e0: 2b20 225c 5c66 696c 6573 5c5c 6d79 6d61  + "\\files\\myma
-000160f0: 7472 6978 2e68 746d 6c22 2c6f 732e 6765  trix.html",os.ge
-00016100: 7463 7764 2829 202b 2022 5c5c 6669 6c65  tcwd() + "\\file
-00016110: 735c 5c6d 796d 6174 7269 782e 6874 6d6c  s\\mymatrix.html
-00016120: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00016130: 2020 2020 2020 2020 2373 6875 7469 6c2e          #shutil.
-00016140: 636f 7079 286f 732e 6765 7463 7764 2829  copy(os.getcwd()
-00016150: 202b 2022 5c5c 6669 6c65 735c 5c6d 7973   + "\\files\\mys
-00016160: 7479 6c65 2e63 7373 222c 206f 732e 6765  tyle.css", os.ge
-00016170: 7463 7764 2829 202b 2022 5c5c 6669 6c65  tcwd() + "\\file
-00016180: 735c 5c6d 7973 7479 6c65 2e63 7373 2229  s\\mystyle.css")
-00016190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000161a0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000161b0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-000161c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000161d0: 6c66 2e6e 6f74 6966 7928 6d65 7373 6167  lf.notify(messag
-000161e0: 653d 7374 7228 6529 2c74 6974 6c65 3d22  e=str(e),title="
-000161f0: 416e 2045 7272 6f72 206f 6363 7572 7265  An Error occurre
-00016200: 642e 2e2e 2849 4420 3133 3038 2922 290d  d...(ID 1308)").
-00016210: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
-00016220: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00016230: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-00016240: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
-00016250: 6679 286d 6573 7361 6765 3d73 7472 2865  fy(message=str(e
-00016260: 292c 7469 746c 653d 2241 6e20 4572 726f  ),title="An Erro
-00016270: 7220 6f63 6375 7272 6564 2e2e 2e28 4944  r occurred...(ID
-00016280: 2031 3331 3129 2229 0d0a 2020 2020 2020   1311)")..      
-00016290: 2020 2020 2020 2320 2d2d 2d2d 2d2d 2d2d        # --------
-000162a0: 2d2d 2d2d 2d0d 0a0d 0a20 2020 2020 2020  -----....       
-000162b0: 2020 2020 2070 642e 6f70 7469 6f6e 732e       pd.options.
-000162c0: 6469 7370 6c61 792e 6d61 785f 636f 6c77  display.max_colw
-000162d0: 6964 7468 203d 2032 0d0a 0d0a 2020 2020  idth = 2....    
-000162e0: 2020 2020 2020 2020 6466 5f64 6973 706c          df_displ
-000162f0: 6179 203d 2064 665f 6261 636b 7570 2e61  ay = df_backup.a
-00016300: 7070 6c79 6d61 7028 6162 6272 6576 6961  pplymap(abbrevia
-00016310: 7465 5f7a 6572 6f73 292e 746f 5f73 7472  te_zeros).to_str
-00016320: 696e 6728 6c69 6e65 5f77 6964 7468 3d4e  ing(line_width=N
-00016330: 6f6e 6529 2e72 6570 6c61 6365 2822 5c5f  one).replace("\_
-00016340: 222c 2022 5f22 290d 0a0d 0a20 2020 2020  ", "_")....     
-00016350: 2020 2020 2020 2023 2073 656c 662e 7061         # self.pa
-00016360: 7265 6e74 2e70 6172 656e 7441 7070 2e67  rent.parentApp.g
-00016370: 6574 466f 726d 2822 4147 4752 5f46 4c4f  etForm("AGGR_FLO
-00016380: 5722 292e 6461 7461 5f62 6f78 2e76 616c  W").data_box.val
-00016390: 7565 7320 3d20 6466 5f64 6973 706c 6179  ues = df_display
-000163a0: 2e73 706c 6974 2822 5c6e 2229 0d0a 2020  .split("\n")..  
-000163b0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-000163c0: 2e70 6172 656e 742e 7061 7265 6e74 4170  .parent.parentAp
-000163d0: 702e 7377 6974 6368 466f 726d 2822 4147  p.switchForm("AG
-000163e0: 4752 5f46 4c4f 5722 290d 0a0d 0a0d 0a20  GR_FLOW")...... 
-000163f0: 2020 2064 6566 2067 656e 5f63 6f64 6528     def gen_code(
-00016400: 7365 6c66 2c73 686f 775f 6e6f 7469 6669  self,show_notifi
-00016410: 6361 7469 6f6e 3d46 616c 7365 293a 0d0a  cation=False):..
-00016420: 0d0a 2020 2020 2020 2020 636f 6465 203d  ..        code =
-00016430: 2022 220d 0a20 2020 2020 2020 2063 6f64   ""..        cod
-00016440: 6520 2b3d 2022 6672 6f6d 2073 6663 746f  e += "from sfcto
-00016450: 6f6c 7320 696d 706f 7274 2046 6c6f 774d  ols import FlowM
-00016460: 6174 7269 7820 5c6e 696d 706f 7274 206e  atrix \nimport n
-00016470: 756d 7079 2061 7320 6e70 5c6e 220d 0a20  umpy as np\n".. 
-00016480: 2020 2020 2020 2063 6f64 6520 2b3d 2022         code += "
-00016490: 6672 6f6d 2073 6663 746f 6f6c 7320 696d  from sfctools im
-000164a0: 706f 7274 2042 616c 616e 6365 456e 7472  port BalanceEntr
-000164b0: 792c 4163 636f 756e 7473 5c6e 220d 0a20  y,Accounts\n".. 
-000164c0: 2020 2020 2020 2063 6f64 6520 2b3d 2022         code += "
-000164d0: 6672 6f6d 2073 6663 746f 6f6c 7320 696d  from sfctools im
-000164e0: 706f 7274 2043 6173 6846 6c6f 7745 6e74  port CashFlowEnt
-000164f0: 7279 5c6e 220d 0a20 2020 2020 2020 2063  ry\n"..        c
-00016500: 6f64 6520 2b3d 2022 6672 6f6d 2073 6663  ode += "from sfc
-00016510: 746f 6f6c 7320 696d 706f 7274 2049 4353  tools import ICS
-00016520: 456e 7472 795c 6e22 0d0a 2020 2020 2020  Entry\n"..      
-00016530: 2020 636f 6465 202b 3d20 2243 4120 3d20    code += "CA = 
-00016540: 4163 636f 756e 7473 2e43 415c 6e4b 4120  Accounts.CA\nKA 
-00016550: 3d20 4163 636f 756e 7473 2e4b 415c 6e5c  = Accounts.KA\n\
-00016560: 6e22 0d0a 0d0a 2020 2020 2020 2020 7375  n"....        su
-00016570: 626a 6563 7473 5f63 6f75 6e74 203d 2064  bjects_count = d
-00016580: 6566 6175 6c74 6469 6374 286c 616d 6264  efaultdict(lambd
-00016590: 613a 2030 2e30 290d 0a0d 0a20 2020 2020  a: 0.0)....     
-000165a0: 2020 2066 6f72 2066 696c 6564 6174 6120     for filedata 
-000165b0: 696e 2073 656c 662e 656e 7472 795f 6461  in self.entry_da
-000165c0: 7461 3a0d 0a20 2020 2020 2020 2020 2020  ta:..           
-000165d0: 2061 6765 6e74 3120 3d20 6669 6c65 6461   agent1 = fileda
-000165e0: 7461 5b22 6167 656e 7431 225d 0d0a 2020  ta["agent1"]..  
-000165f0: 2020 2020 2020 2020 2020 6167 656e 7432            agent2
-00016600: 203d 2066 696c 6564 6174 615b 2261 6765   = filedata["age
-00016610: 6e74 3222 5d0d 0a0d 0a20 2020 2020 2020  nt2"]....       
-00016620: 2020 2020 2069 6620 6167 656e 7431 203d       if agent1 =
-00016630: 3d20 6167 656e 7432 3a0d 0a20 2020 2020  = agent2:..     
-00016640: 2020 2020 2020 2020 2020 2061 6765 6e74             agent
-00016650: 3220 3d20 226f 7468 6572 5f22 202b 2061  2 = "other_" + a
-00016660: 6765 6e74 320d 0a0d 0a20 2020 2020 2020  gent2....       
-00016670: 2020 2020 2061 3120 3d20 6669 6c65 6461       a1 = fileda
-00016680: 7461 5b22 6131 225d 2020 2320 2b20 225c  ta["a1"]  # + "\
-00016690: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
-000166a0: 6531 203d 2066 696c 6564 6174 615b 2265  e1 = filedata["e
-000166b0: 3122 5d20 2023 202b 2022 5c6e 220d 0a20  1"]  # + "\n".. 
-000166c0: 2020 2020 2020 2020 2020 206c 3120 3d20             l1 = 
-000166d0: 6669 6c65 6461 7461 5b22 6c31 225d 2020  filedata["l1"]  
-000166e0: 2320 2b20 225c 6e22 0d0a 2020 2020 2020  # + "\n"..      
-000166f0: 2020 2020 2020 6132 203d 2066 696c 6564        a2 = filed
-00016700: 6174 615b 2261 3222 5d20 2023 202b 2022  ata["a2"]  # + "
-00016710: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
-00016720: 2065 3220 3d20 6669 6c65 6461 7461 5b22   e2 = filedata["
-00016730: 6532 225d 2020 2320 2b20 225c 6e22 0d0a  e2"]  # + "\n"..
-00016740: 2020 2020 2020 2020 2020 2020 6c32 203d              l2 =
-00016750: 2066 696c 6564 6174 615b 226c 3222 5d20   filedata["l2"] 
-00016760: 2023 202b 2022 5c6e 220d 0a0d 0a20 2020   # + "\n"....   
-00016770: 2020 2020 2020 2020 2066 6c6f 775f 6368           flow_ch
-00016780: 6563 6b20 3d20 5472 7565 0d0a 2020 2020  eck = True..    
-00016790: 2020 2020 2020 2020 7072 696e 7428 2246          print("F
-000167a0: 4c4f 5720 4348 4543 4b22 2c20 6669 6c65  LOW CHECK", file
-000167b0: 6461 7461 5b22 7368 6f72 746e 616d 6522  data["shortname"
-000167c0: 5d2c 6669 6c65 6461 7461 5b22 6c6f 6720  ],filedata["log 
-000167d0: 7472 616e 7361 6374 696f 6e22 5d29 0d0a  transaction"])..
-000167e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000167f0: 7369 6e73 7461 6e63 6528 6669 6c65 6461  sinstance(fileda
-00016800: 7461 5b22 6c6f 6720 7472 616e 7361 6374  ta["log transact
-00016810: 696f 6e22 5d2c 7374 7229 2061 6e64 2066  ion"],str) and f
-00016820: 696c 6564 6174 615b 226c 6f67 2074 7261  iledata["log tra
-00016830: 6e73 6163 7469 6f6e 225d 2e73 7472 6970  nsaction"].strip
-00016840: 2829 203d 3d20 2254 7275 6522 3a0d 0a20  () == "True":.. 
-00016850: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00016860: 2062 6f6f 6c28 6669 6c65 6461 7461 5b22   bool(filedata["
-00016870: 6c6f 6720 7472 616e 7361 6374 696f 6e22  log transaction"
-00016880: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00016890: 2020 2020 666c 6f77 5f63 6865 636b 203d      flow_check =
-000168a0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-000168b0: 2020 2020 2020 2070 7269 6e74 2866 6c6f         print(flo
-000168c0: 775f 6368 6563 6b29 0d0a 2020 2020 2020  w_check)..      
-000168d0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000168e0: 7461 6e63 6528 6669 6c65 6461 7461 5b22  tance(filedata["
-000168f0: 6c6f 6720 7472 616e 7361 6374 696f 6e22  log transaction"
-00016900: 5d2c 7374 7229 2061 6e64 2066 696c 6564  ],str) and filed
-00016910: 6174 615b 226c 6f67 2074 7261 6e73 6163  ata["log transac
-00016920: 7469 6f6e 225d 2e73 7472 6970 2829 203d  tion"].strip() =
-00016930: 3d20 2246 616c 7365 223a 0d0a 2020 2020  = "False":..    
-00016940: 2020 2020 2020 2020 2020 2020 2320 626f              # bo
-00016950: 6f6c 2866 696c 6564 6174 615b 226c 6f67  ol(filedata["log
-00016960: 2074 7261 6e73 6163 7469 6f6e 225d 290d   transaction"]).
-00016970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016980: 2066 6c6f 775f 6368 6563 6b20 3d20 4661   flow_check = Fa
-00016990: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-000169a0: 2020 2020 2070 7269 6e74 2866 6c6f 775f       print(flow_
-000169b0: 6368 6563 6b29 0d0a 2020 2020 2020 2020  check)..        
-000169c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000169d0: 2020 2020 2020 2020 2020 2066 6c6f 775f             flow_
-000169e0: 6368 6563 6b20 3d20 6669 6c65 6461 7461  check = filedata
-000169f0: 5b22 6c6f 6720 7472 616e 7361 6374 696f  ["log transactio
-00016a00: 6e22 5d0d 0a20 2020 2020 2020 2020 2020  n"]..           
-00016a10: 2020 2020 2070 7269 6e74 2866 6c6f 775f       print(flow_
-00016a20: 6368 6563 6b29 0d0a 2020 2020 2020 2020  check)..        
-00016a30: 2020 2020 2370 7269 6e74 2822 464c 4f57      #print("FLOW
-00016a40: 2043 4845 434b 222c 2066 696c 656e 616d   CHECK", filenam
-00016a50: 652c 2066 6c6f 775f 6368 6563 6b29 0d0a  e, flow_check)..
-00016a60: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016a70: 7428 2274 7970 6522 2c20 7479 7065 2866  t("type", type(f
-00016a80: 6c6f 775f 6368 6563 6b29 290d 0a0d 0a20  low_check)).... 
-00016a90: 2020 2020 2020 2020 2020 206b 696e 6420             kind 
-00016aa0: 3d20 6669 6c65 6461 7461 5b22 6b69 6e64  = filedata["kind
-00016ab0: 225d 0d0a 0d0a 2020 2020 2020 2020 2020  "]....          
-00016ac0: 2020 2373 7562 6a65 6374 203d 2020 6669    #subject =  fi
-00016ad0: 6c65 6461 7461 5b22 7375 626a 6563 7422  ledata["subject"
-00016ae0: 5d2e 7265 706c 6163 6528 2220 222c 225f  ].replace(" ","_
-00016af0: 2229 202b 2022 5f22 202b 2066 696c 6564  ") + "_" + filed
-00016b00: 6174 615b 2273 686f 7274 6e61 6d65 222e  ata["shortname".
-00016b10: 7265 706c 6163 6528 2220 222c 225f 2229  replace(" ","_")
-00016b20: 5d2e 6c6f 7765 7228 290d 0a20 2020 2020  ].lower()..     
-00016b30: 2020 2020 2020 2073 7562 6a65 6374 203d         subject =
-00016b40: 2020 6669 6c65 6461 7461 5b22 7368 6f72    filedata["shor
-00016b50: 746e 616d 6522 2e72 6570 6c61 6365 2822  tname".replace("
-00016b60: 2022 2c22 5f22 295d 2e72 6570 6c61 6365   ","_")].replace
-00016b70: 2822 2822 2c22 5f22 292e 7265 706c 6163  ("(","_").replac
-00016b80: 6528 2229 222c 2222 292e 6c6f 7765 7228  e(")","").lower(
-00016b90: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00016ba0: 7562 6a65 6374 5f73 7472 203d 2020 6669  ubject_str =  fi
-00016bb0: 6c65 6461 7461 5b22 7375 626a 6563 7422  ledata["subject"
-00016bc0: 2e72 6570 6c61 6365 2822 2022 2c22 5f22  .replace(" ","_"
-00016bd0: 295d 2e6c 6f77 6572 2829 2e63 6170 6974  )].lower().capit
-00016be0: 616c 697a 6528 292e 7265 706c 6163 6528  alize().replace(
-00016bf0: 225f 222c 2022 2022 290d 0a0d 0a20 2020  "_", " ")....   
-00016c00: 2020 2020 2020 2020 2073 7562 6a65 6374           subject
-00016c10: 735f 636f 756e 745b 7375 626a 6563 745d  s_count[subject]
-00016c20: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-00016c30: 2020 2069 6620 7375 626a 6563 7473 5f63     if subjects_c
-00016c40: 6f75 6e74 5b73 7562 6a65 6374 5d20 3e20  ount[subject] > 
-00016c50: 313a 2023 2073 7566 6669 7820 666f 7220  1: # suffix for 
-00016c60: 7361 6d65 206e 616d 6573 0d0a 2020 2020  same names..    
-00016c70: 2020 2020 2020 2020 2020 2020 7375 626a              subj
-00016c80: 6563 7420 2b3d 2022 5f25 6922 2025 2069  ect += "_%i" % i
-00016c90: 6e74 2873 7562 6a65 6374 735f 636f 756e  nt(subjects_coun
-00016ca0: 745b 7375 626a 6563 745d 290d 0a0d 0a0d  t[subject]).....
-00016cb0: 0a20 2020 2020 2020 2020 2020 2071 7561  .            qua
-00016cc0: 6e74 6974 7920 3d20 2271 2220 2320 6669  ntity = "q" # fi
-00016cd0: 6c65 6461 7461 5b22 7175 616e 7469 7479  ledata["quantity
-00016ce0: 225d 0d0a 0d0a 2020 2020 2020 2020 2020  "]....          
-00016cf0: 2020 636f 6d6d 616e 6473 203d 205b 5d0d    commands = [].
-00016d00: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00016d10: 6620 2275 6e69 2d64 6972 6563 7469 6f6e  f "uni-direction
-00016d20: 616c 2220 696e 2066 696c 6564 6174 613a  al" in filedata:
-00016d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016d40: 2020 756e 6964 6972 203d 2066 696c 6564    unidir = filed
-00016d50: 6174 615b 2275 6e69 2d64 6972 6563 7469  ata["uni-directi
-00016d60: 6f6e 616c 225d 0d0a 0d0a 2020 2020 2020  onal"]....      
-00016d70: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-00016d80: 6473 2e61 7070 656e 6428 2263 6f6e 6420  ds.append("cond 
-00016d90: 3d20 2869 7369 6e73 7461 6e63 6528 712c  = (isinstance(q,
-00016da0: 666c 6f61 7429 206f 7220 6973 696e 7374  float) or isinst
-00016db0: 616e 6365 2871 2c69 6e74 2929 2229 0d0a  ance(q,int))")..
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 636f 6d6d 616e 6473 2e61 7070 656e 6428  commands.append(
-00016de0: 2269 6620 636f 6e64 3a20 6173 7365 7274  "if cond: assert
-00016df0: 206e 6f74 206e 702e 6973 6e61 6e28 7129   not np.isnan(q)
-00016e00: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00016e10: 2020 2020 2320 5e20 7769 6c6c 2061 6c73      # ^ will als
-00016e20: 6f20 7061 7373 2066 6f72 206e 702e 666c  o pass for np.fl
-00016e30: 6f61 7436 340d 0a20 2020 2020 2020 2020  oat64..         
-00016e40: 2020 2020 2020 2063 6f6d 6d61 6e64 732e         commands.
-00016e50: 6170 7065 6e64 2822 6966 2063 6f6e 643a  append("if cond:
-00016e60: 2061 7373 6572 7420 7120 3c20 2b6e 702e   assert q < +np.
-00016e70: 696e 6622 290d 0a20 2020 2020 2020 2020  inf")..         
-00016e80: 2020 2020 2020 2063 6f6d 6d61 6e64 732e         commands.
-00016e90: 6170 7065 6e64 2822 6966 2063 6f6e 643a  append("if cond:
-00016ea0: 2061 7373 6572 7420 7120 3e20 2d6e 702e   assert q > -np.
-00016eb0: 696e 6622 290d 0a0d 0a20 2020 2020 2020  inf")....       
-00016ec0: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
-00016ed0: 2275 6e69 2d64 6972 6563 7469 6f6e 616c  "uni-directional
-00016ee0: 222c 756e 6964 6972 290d 0a20 2020 2020  ",unidir)..     
-00016ef0: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00016f00: 7228 756e 6964 6972 2920 3d3d 2022 5472  r(unidir) == "Tr
-00016f10: 7565 223a 2023 2064 6f20 6e6f 7420 646f  ue": # do not do
-00016f20: 2062 6f6f 6c28 756e 6964 6972 290d 0a20   bool(unidir).. 
-00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f40: 2020 2023 6e61 6d61 6161 203d 2066 696c     #namaaa = fil
-00016f50: 6564 6174 615b 2273 686f 7274 6e61 6d65  edata["shortname
-00016f60: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00016f70: 2020 2020 2020 2020 2373 656c 662e 6e6f          #self.no
-00016f80: 7469 6679 2820 286e 616d 6161 612b 2073  tify( (namaaa+ s
-00016f90: 7472 2875 6e69 6469 7229 2b20 223d 222b  tr(unidir)+ "="+
-00016fa0: 2873 7472 2862 6f6f 6c28 756e 6964 6972  (str(bool(unidir
-00016fb0: 2929 2929 2c74 6974 6c65 3d22 6368 6563  )))),title="chec
-00016fc0: 6b22 290d 0a20 2020 2020 2020 2020 2020  k")..           
-00016fd0: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-00016fe0: 732e 6170 7065 6e64 2822 6966 2063 6f6e  s.append("if con
-00016ff0: 643a 2061 7373 6572 7420 7120 3e3d 2030  d: assert q >= 0
-00017000: 2c20 2768 6176 6520 746f 2070 6173 7320  , 'have to pass 
-00017010: 706f 7369 7469 7665 2071 7561 6e74 6974  positive quantit
-00017020: 793a 2075 6e69 6469 7265 6374 696f 6e61  y: unidirectiona
-00017030: 6c20 7472 616e 7361 6374 696f 6e27 2229  l transaction'")
-00017040: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017050: 636f 6d6d 616e 6473 203d 2063 6f6d 6d61  commands = comma
-00017060: 6e64 7320 2b20 5b22 2573 2e62 616c 616e  nds + ["%s.balan
-00017070: 6365 5f73 6865 6574 2e64 6973 656e 6761  ce_sheet.disenga
-00017080: 6765 2829 2220 2520 6167 656e 7431 5d0d  ge()" % agent1].
-00017090: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000170a0: 5472 7565 3a20 2320 6167 656e 7431 2021  True: # agent1 !
-000170b0: 3d20 6167 656e 7432 3a0d 0a20 2020 2020  = agent2:..     
-000170c0: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-000170d0: 6e64 732b 3d20 5b22 2573 2e62 616c 616e  nds+= ["%s.balan
-000170e0: 6365 5f73 6865 6574 2e64 6973 656e 6761  ce_sheet.disenga
-000170f0: 6765 2829 2220 2520 6167 656e 7432 5d0d  ge()" % agent2].
-00017100: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-00017110: 6f72 2065 6e74 7279 2069 6e20 6531 2e73  or entry in e1.s
-00017120: 706c 6974 2822 5c6e 2229 3a0d 0a20 2020  plit("\n"):..   
-00017130: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017140: 656e 7472 7920 213d 2022 2220 616e 6420  entry != "" and 
-00017150: 656e 7472 7920 213d 2022 5c6e 223a 0d0a  entry != "\n":..
-00017160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017170: 2020 2020 7369 676e 2c20 6974 656d 2c20      sign, item, 
-00017180: 7369 6c65 6e74 203d 2073 656c 662e 656e  silent = self.en
-00017190: 7472 795f 746f 5f76 616c 7328 656e 7472  try_to_vals(entr
-000171a0: 792c 2061 6765 6e74 312c 2022 4571 7569  y, agent1, "Equi
-000171b0: 7479 2229 0d0a 2020 2020 2020 2020 2020  ty")..          
-000171c0: 2020 2020 2020 2020 2020 6966 2073 6967            if sig
-000171d0: 6e20 6973 206e 6f74 204e 6f6e 653a 0d0a  n is not None:..
-000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171f0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-00017200: 2e61 7070 656e 6428 2225 732e 6261 6c61  .append("%s.bala
-00017210: 6e63 655f 7368 6565 742e 6368 616e 6765  nce_sheet.change
-00017220: 5f69 7465 6d28 2725 7327 2c20 2573 2c20  _item('%s', %s, 
-00017230: 2573 2c20 7375 7070 7265 7373 5f73 746f  %s, suppress_sto
-00017240: 636b 3d25 7329 2220 2520 280d 0a20 2020  ck=%s)" % (..   
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 2020 2061 6765 6e74 312c 2069 7465       agent1, ite
-00017270: 6d2c 2022 4261 6c61 6e63 6545 6e74 7279  m, "BalanceEntry
-00017280: 2e45 5155 4954 5922 2c20 7369 676e 202b  .EQUITY", sign +
-00017290: 2071 7561 6e74 6974 792c 2073 696c 656e   quantity, silen
-000172a0: 7429 290d 0a20 2020 2020 2020 2020 2020  t))..           
-000172b0: 2066 6f72 2065 6e74 7279 2069 6e20 6131   for entry in a1
-000172c0: 2e73 706c 6974 2822 5c6e 2229 3a0d 0a20  .split("\n"):.. 
-000172d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000172e0: 6620 656e 7472 7920 213d 2022 2220 616e  f entry != "" an
-000172f0: 6420 656e 7472 7920 213d 2022 5c6e 223a  d entry != "\n":
-00017300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017310: 2020 2020 2020 7369 676e 2c20 6974 656d        sign, item
-00017320: 2c20 7369 6c65 6e74 203d 2073 656c 662e  , silent = self.
-00017330: 656e 7472 795f 746f 5f76 616c 7328 656e  entry_to_vals(en
-00017340: 7472 792c 2061 6765 6e74 312c 2022 4173  try, agent1, "As
-00017350: 7365 7473 2229 0d0a 2020 2020 2020 2020  sets")..        
-00017360: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017370: 6967 6e20 6973 206e 6f74 204e 6f6e 653a  ign is not None:
-00017380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017390: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-000173a0: 6473 2e61 7070 656e 6428 2225 732e 6261  ds.append("%s.ba
-000173b0: 6c61 6e63 655f 7368 6565 742e 6368 616e  lance_sheet.chan
-000173c0: 6765 5f69 7465 6d28 2725 7327 2c20 2573  ge_item('%s', %s
-000173d0: 2c20 2573 2c20 7375 7070 7265 7373 5f73  , %s, suppress_s
-000173e0: 746f 636b 3d25 7329 2220 2520 280d 0a20  tock=%s)" % (.. 
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 2020 2020 2061 6765 6e74 312c 2069         agent1, i
-00017410: 7465 6d2c 2022 4261 6c61 6e63 6545 6e74  tem, "BalanceEnt
-00017420: 7279 2e41 5353 4554 5322 2c20 7369 676e  ry.ASSETS", sign
-00017430: 202b 2071 7561 6e74 6974 792c 2073 696c   + quantity, sil
-00017440: 656e 7429 290d 0a20 2020 2020 2020 2020  ent))..         
-00017450: 2020 2066 6f72 2065 6e74 7279 2069 6e20     for entry in 
-00017460: 6c31 2e73 706c 6974 2822 5c6e 2229 3a0d  l1.split("\n"):.
-00017470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017480: 2069 6620 656e 7472 7920 213d 2022 2220   if entry != "" 
-00017490: 616e 6420 656e 7472 7920 213d 2022 5c6e  and entry != "\n
-000174a0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000174b0: 2020 2020 2020 2020 7369 676e 2c20 6974          sign, it
-000174c0: 656d 2c20 7369 6c65 6e74 203d 2073 656c  em, silent = sel
-000174d0: 662e 656e 7472 795f 746f 5f76 616c 7328  f.entry_to_vals(
-000174e0: 656e 7472 792c 2061 6765 6e74 312c 2022  entry, agent1, "
-000174f0: 4c69 6162 696c 6974 6965 7322 290d 0a20  Liabilities").. 
-00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017510: 2020 2069 6620 7369 676e 2069 7320 6e6f     if sign is no
-00017520: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 2063 6f6d 6d61 6e64 732e 6170 7065 6e64   commands.append
-00017550: 2822 2573 2e62 616c 616e 6365 5f73 6865  ("%s.balance_she
-00017560: 6574 2e63 6861 6e67 655f 6974 656d 2827  et.change_item('
-00017570: 2573 272c 2025 732c 2025 732c 2073 7570  %s', %s, %s, sup
-00017580: 7072 6573 735f 7374 6f63 6b3d 2573 2922  press_stock=%s)"
-00017590: 2025 2028 0d0a 2020 2020 2020 2020 2020   % (..          
-000175a0: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-000175b0: 656e 7431 2c20 6974 656d 2c20 2242 616c  ent1, item, "Bal
-000175c0: 616e 6365 456e 7472 792e 4c49 4142 494c  anceEntry.LIABIL
-000175d0: 4954 4945 5322 2c20 7369 676e 202b 2071  ITIES", sign + q
-000175e0: 7561 6e74 6974 792c 2073 696c 656e 7429  uantity, silent)
-000175f0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00017600: 6f72 2065 6e74 7279 2069 6e20 6532 2e73  or entry in e2.s
-00017610: 706c 6974 2822 5c6e 2229 3a0d 0a20 2020  plit("\n"):..   
-00017620: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017630: 656e 7472 7920 213d 2022 2220 616e 6420  entry != "" and 
-00017640: 656e 7472 7920 213d 2022 5c6e 223a 0d0a  entry != "\n":..
-00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2020 2020 7369 676e 2c20 6974 656d 2c20      sign, item, 
-00017670: 7369 6c65 6e74 203d 2073 656c 662e 656e  silent = self.en
-00017680: 7472 795f 746f 5f76 616c 7328 656e 7472  try_to_vals(entr
-00017690: 792c 2061 6765 6e74 322c 2022 4571 7569  y, agent2, "Equi
-000176a0: 7479 2229 0d0a 2020 2020 2020 2020 2020  ty")..          
-000176b0: 2020 2020 2020 2020 2020 6966 2073 6967            if sig
-000176c0: 6e20 6973 206e 6f74 204e 6f6e 653a 0d0a  n is not None:..
-000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176e0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-000176f0: 2e61 7070 656e 6428 2225 732e 6261 6c61  .append("%s.bala
-00017700: 6e63 655f 7368 6565 742e 6368 616e 6765  nce_sheet.change
-00017710: 5f69 7465 6d28 2725 7327 2c20 2573 2c20  _item('%s', %s, 
-00017720: 2573 2c20 7375 7070 7265 7373 5f73 746f  %s, suppress_sto
-00017730: 636b 3d25 7329 2220 2520 280d 0a20 2020  ck=%s)" % (..   
-00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017750: 2020 2020 2061 6765 6e74 322c 2069 7465       agent2, ite
-00017760: 6d2c 2022 4261 6c61 6e63 6545 6e74 7279  m, "BalanceEntry
-00017770: 2e45 5155 4954 5922 2c20 7369 676e 202b  .EQUITY", sign +
-00017780: 2071 7561 6e74 6974 792c 2073 696c 656e   quantity, silen
-00017790: 7429 290d 0a20 2020 2020 2020 2020 2020  t))..           
-000177a0: 2066 6f72 2065 6e74 7279 2069 6e20 6132   for entry in a2
-000177b0: 2e73 706c 6974 2822 5c6e 2229 3a0d 0a20  .split("\n"):.. 
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000177d0: 6620 656e 7472 7920 213d 2022 2220 616e  f entry != "" an
-000177e0: 6420 656e 7472 7920 213d 2022 5c6e 223a  d entry != "\n":
-000177f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017800: 2020 2020 2020 7369 676e 2c20 6974 656d        sign, item
-00017810: 2c20 7369 6c65 6e74 203d 2073 656c 662e  , silent = self.
-00017820: 656e 7472 795f 746f 5f76 616c 7328 656e  entry_to_vals(en
-00017830: 7472 792c 2061 6765 6e74 322c 2022 4173  try, agent2, "As
-00017840: 7365 7473 2229 0d0a 2020 2020 2020 2020  sets")..        
-00017850: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017860: 6967 6e20 6973 206e 6f74 204e 6f6e 653a  ign is not None:
-00017870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017880: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-00017890: 6473 2e61 7070 656e 6428 2225 732e 6261  ds.append("%s.ba
-000178a0: 6c61 6e63 655f 7368 6565 742e 6368 616e  lance_sheet.chan
-000178b0: 6765 5f69 7465 6d28 2725 7327 2c20 2573  ge_item('%s', %s
-000178c0: 2c20 2573 2c20 7375 7070 7265 7373 5f73  , %s, suppress_s
-000178d0: 746f 636b 3d25 7329 2220 2520 280d 0a20  tock=%s)" % (.. 
-000178e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178f0: 2020 2020 2020 2061 6765 6e74 322c 2069         agent2, i
-00017900: 7465 6d2c 2022 4261 6c61 6e63 6545 6e74  tem, "BalanceEnt
-00017910: 7279 2e41 5353 4554 5322 2c20 7369 676e  ry.ASSETS", sign
-00017920: 202b 2071 7561 6e74 6974 792c 2073 696c   + quantity, sil
-00017930: 656e 7429 290d 0a20 2020 2020 2020 2020  ent))..         
-00017940: 2020 2066 6f72 2065 6e74 7279 2069 6e20     for entry in 
-00017950: 6c32 2e73 706c 6974 2822 5c6e 2229 3a0d  l2.split("\n"):.
-00017960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017970: 2069 6620 656e 7472 7920 213d 2022 2220   if entry != "" 
-00017980: 616e 6420 656e 7472 7920 213d 2022 5c6e  and entry != "\n
-00017990: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000179a0: 2020 2020 2020 2020 7369 676e 2c20 6974          sign, it
-000179b0: 656d 2c20 7369 6c65 6e74 203d 2073 656c  em, silent = sel
-000179c0: 662e 656e 7472 795f 746f 5f76 616c 7328  f.entry_to_vals(
-000179d0: 656e 7472 792c 2061 6765 6e74 322c 2022  entry, agent2, "
-000179e0: 4c69 6162 696c 6974 6965 7322 290d 0a20  Liabilities").. 
-000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a00: 2020 2069 6620 7369 676e 2069 7320 6e6f     if sign is no
-00017a10: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a30: 2063 6f6d 6d61 6e64 732e 6170 7065 6e64   commands.append
-00017a40: 2822 2573 2e62 616c 616e 6365 5f73 6865  ("%s.balance_she
-00017a50: 6574 2e63 6861 6e67 655f 6974 656d 2827  et.change_item('
-00017a60: 2573 272c 2025 732c 2025 732c 2073 7570  %s', %s, %s, sup
-00017a70: 7072 6573 735f 7374 6f63 6b3d 2573 2922  press_stock=%s)"
-00017a80: 2025 2028 0d0a 2020 2020 2020 2020 2020   % (..          
-00017a90: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-00017aa0: 656e 7432 2c20 6974 656d 2c20 2242 616c  ent2, item, "Bal
-00017ab0: 616e 6365 456e 7472 792e 4c49 4142 494c  anceEntry.LIABIL
-00017ac0: 4954 4945 5322 2c20 7369 676e 202b 2071  ITIES", sign + q
-00017ad0: 7561 6e74 6974 792c 2073 696c 656e 7429  uantity, silent)
-00017ae0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017af0: 2063 6f6d 6d61 6e64 732e 6170 7065 6e64   commands.append
-00017b00: 2822 2573 2e62 616c 616e 6365 5f73 6865  ("%s.balance_she
-00017b10: 6574 2e65 6e67 6167 6528 2922 2025 2061  et.engage()" % a
-00017b20: 6765 6e74 3129 0d0a 2020 2020 2020 2020  gent1)..        
-00017b30: 2020 2020 6966 2054 7275 653a 2023 2061      if True: # a
-00017b40: 6765 6e74 3121 3d61 6765 6e74 323a 0d0a  gent1!=agent2:..
-00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b60: 636f 6d6d 616e 6473 2e61 7070 656e 6428  commands.append(
-00017b70: 2225 732e 6261 6c61 6e63 655f 7368 6565  "%s.balance_shee
-00017b80: 742e 656e 6761 6765 2829 2220 2520 6167  t.engage()" % ag
-00017b90: 656e 7432 290d 0a0d 0a20 2020 2020 2020  ent2)....       
-00017ba0: 2020 2020 2061 6464 5f66 6c6f 7720 3d20       add_flow = 
-00017bb0: 666c 6f77 5f63 6865 636b 0d0a 2020 2020  flow_check..    
-00017bc0: 2020 2020 2020 2020 6966 2061 6464 5f66          if add_f
-00017bd0: 6c6f 773a 0d0a 2020 2020 2020 2020 2020  low:..          
-00017be0: 2020 2020 2020 7072 696e 7428 7375 626a        print(subj
-00017bf0: 6563 745f 7374 722c 2266 6c6f 7720 6368  ect_str,"flow ch
-00017c00: 6563 6b22 2c66 6c6f 775f 6368 6563 6b29  eck",flow_check)
-00017c10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017c20: 2020 2020 6b69 6e64 5f65 6e75 6d20 3d20      kind_enum = 
-00017c30: 2228 2573 2c25 7329 2220 2520 286b 696e  "(%s,%s)" % (kin
-00017c40: 642e 7370 6c69 7428 222d 3e22 295b 305d  d.split("->")[0]
-00017c50: 2e73 7472 6970 2829 2c6b 696e 642e 7370  .strip(),kind.sp
-00017c60: 6c69 7428 222d 3e22 295b 315d 2e73 7472  lit("->")[1].str
-00017c70: 6970 2829 290d 0a0d 0a20 2020 2020 2020  ip())....       
-00017c80: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-00017c90: 732e 6170 7065 6e64 2822 466c 6f77 4d61  s.append("FlowMa
-00017ca0: 7472 6978 2829 2e6c 6f67 5f66 6c6f 7728  trix().log_flow(
-00017cb0: 2573 2c20 2573 2c20 2573 2c20 2573 2c20  %s, %s, %s, %s, 
-00017cc0: 7375 626a 6563 743d 2725 7327 2922 2025  subject='%s')" %
-00017cd0: 2028 6b69 6e64 5f65 6e75 6d2c 2071 7561   (kind_enum, qua
-00017ce0: 6e74 6974 792c 2061 6765 6e74 312c 2061  ntity, agent1, a
-00017cf0: 6765 6e74 322c 2073 7562 6a65 6374 5f73  gent2, subject_s
-00017d00: 7472 2929 0d0a 0d0a 2020 2020 2020 2020  tr))....        
-00017d10: 2020 2020 2320 6170 7065 6e64 2069 6e73      # append ins
-00017d20: 6572 745f 6c69 6e6b 2063 6f6d 6d61 6e64  ert_link command
-00017d30: 2074 6f20 636f 6465 0d0a 0d0a 0d0a 2020   to code......  
-00017d40: 2020 2020 2020 2020 2020 6d79 5f69 6e63            my_inc
-00017d50: 6f6d 655f 6469 6374 203d 207b 2023 2023  ome_dict = { # #
-00017d60: 7472 616e 736c 6174 6573 2073 7472 696e  translates strin
-00017d70: 6720 696e 746f 2049 4353 456e 7472 7920  g into ICSEntry 
-00017d80: 2866 6f72 2062 6574 7465 7220 6566 6669  (for better effi
-00017d90: 6369 656e 6379 290d 0a20 2020 2020 2020  ciency)..       
-00017da0: 2020 2020 2020 2020 2022 5265 7665 6e75           "Revenu
-00017db0: 6522 3a20 2249 4353 456e 7472 792e 5245  e": "ICSEntry.RE
-00017dc0: 5645 4e55 4553 222c 0d0a 2020 2020 2020  VENUES",..      
-00017dd0: 2020 2020 2020 2020 2020 224e 6f6e 2d4f            "Non-O
-00017de0: 702e 2049 6e63 6f6d 6522 3a20 2249 4353  p. Income": "ICS
-00017df0: 456e 7472 792e 4e4f 4922 2c0d 0a20 2020  Entry.NOI",..   
-00017e00: 2020 2020 2020 2020 2020 2020 2022 4578               "Ex
-00017e10: 7065 6e73 6522 3a20 2249 4353 456e 7472  pense": "ICSEntr
-00017e20: 792e 4558 5045 4e53 4553 222c 0d0a 2020  y.EXPENSES",..  
-00017e30: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-00017e40: 6178 223a 2022 4943 5345 6e74 7279 2e54  ax": "ICSEntry.T
-00017e50: 4158 4553 222c 0d0a 2020 2020 2020 2020  AXES",..        
-00017e60: 2020 2020 2020 2020 2249 6e74 6572 6573          "Interes
-00017e70: 7422 3a20 2249 4353 456e 7472 792e 494e  t": "ICSEntry.IN
-00017e80: 5445 5245 5354 222c 0d0a 2020 2020 2020  TEREST",..      
-00017e90: 2020 2020 2020 2020 2020 2247 6169 6e22            "Gain"
-00017ea0: 3a20 2249 4353 456e 7472 792e 4741 494e  : "ICSEntry.GAIN
-00017eb0: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
-00017ec0: 2020 2020 2022 4e6f 6e74 6178 2e50 726f       "Nontax.Pro
-00017ed0: 6669 7422 3a20 2249 4353 456e 7472 792e  fit": "ICSEntry.
-00017ee0: 4e4f 4e54 4158 5f50 524f 4649 5453 222c  NONTAX_PROFITS",
-00017ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017f00: 2020 224e 6f6e 7461 782e 2050 726f 6669    "Nontax. Profi
-00017f10: 7422 3a20 2249 4353 456e 7472 792e 4e4f  t": "ICSEntry.NO
-00017f20: 4e54 4158 5f50 524f 4649 5453 222c 2023  NTAX_PROFITS", #
-00017f30: 2071 7569 636b 2061 6e64 2064 6972 7479   quick and dirty
-00017f40: 2062 7567 6669 780d 0a20 2020 2020 2020   bugfix..       
-00017f50: 2020 2020 2020 2020 2022 4e6f 6e74 6178           "Nontax
-00017f60: 2e20 4c6f 7373 223a 2020 2249 4353 456e  . Loss":  "ICSEn
-00017f70: 7472 792e 4e4f 4e54 4158 5f4c 4f53 5345  try.NONTAX_LOSSE
-00017f80: 5322 2c0d 0a20 2020 2020 2020 2020 2020  S",..           
-00017f90: 2020 2020 2022 4c6f 7373 223a 2020 2249       "Loss":  "I
-00017fa0: 4353 456e 7472 792e 4c4f 5353 4553 220d  CSEntry.LOSSES".
-00017fb0: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00017fc0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00017fd0: 696e 636f 6d65 2073 7461 7465 6d65 6e74  income statement
-00017fe0: 3f0d 0a20 2020 2020 2020 2020 2020 2069  ?..            i
-00017ff0: 6620 2269 6e63 6f6d 6531 2220 696e 2066  f "income1" in f
-00018000: 696c 6564 6174 613a 0d0a 2020 2020 2020  iledata:..      
-00018010: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-00018020: 2866 696c 6564 6174 615b 2269 6e63 6f6d  (filedata["incom
-00018030: 6531 225d 2920 213d 2027 4e6f 6e65 273a  e1"]) != 'None':
-00018040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018050: 2020 2020 2020 636f 6d6d 616e 6473 2e61        commands.a
-00018060: 7070 656e 6428 2225 732e 696e 636f 6d65  ppend("%s.income
-00018070: 5f73 7461 7465 6d65 6e74 2e6e 6577 5f65  _statement.new_e
-00018080: 6e74 7279 2825 732c 2725 7327 2c25 7329  ntry(%s,'%s',%s)
-00018090: 2220 2520 2861 6765 6e74 312c 6d79 5f69  " % (agent1,my_i
-000180a0: 6e63 6f6d 655f 6469 6374 5b66 696c 6564  ncome_dict[filed
-000180b0: 6174 615b 2269 6e63 6f6d 6531 225d 5d2c  ata["income1"]],
-000180c0: 7375 626a 6563 742c 7175 616e 7469 7479  subject,quantity
-000180d0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000180e0: 2020 6966 2022 696e 636f 6d65 3222 2069    if "income2" i
-000180f0: 6e20 6669 6c65 6461 7461 3a0d 0a20 2020  n filedata:..   
-00018100: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018110: 7374 7228 6669 6c65 6461 7461 5b22 696e  str(filedata["in
-00018120: 636f 6d65 3222 5d29 2021 3d20 274e 6f6e  come2"]) != 'Non
-00018130: 6527 3a0d 0a20 2020 2020 2020 2020 2020  e':..           
-00018140: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-00018150: 732e 6170 7065 6e64 2822 2573 2e69 6e63  s.append("%s.inc
-00018160: 6f6d 655f 7374 6174 656d 656e 742e 6e65  ome_statement.ne
-00018170: 775f 656e 7472 7928 2573 2c27 2573 272c  w_entry(%s,'%s',
-00018180: 2573 2922 2025 2028 6167 656e 7432 2c20  %s)" % (agent2, 
-00018190: 6d79 5f69 6e63 6f6d 655f 6469 6374 5b66  my_income_dict[f
-000181a0: 696c 6564 6174 615b 2269 6e63 6f6d 6532  iledata["income2
-000181b0: 225d 5d2c 2073 7562 6a65 6374 2c20 7175  "]], subject, qu
-000181c0: 616e 7469 7479 2929 0d0a 0d0a 2020 2020  antity))....    
-000181d0: 2020 2020 2020 2020 2320 6361 7368 2066          # cash f
-000181e0: 6c6f 7720 7374 6174 656d 656e 740d 0a20  low statement.. 
-000181f0: 2020 2020 2020 2020 2020 2069 6620 2263             if "c
-00018200: 6173 6866 6c6f 7731 2220 696e 2066 696c  ashflow1" in fil
-00018210: 6564 6174 613a 0d0a 2020 2020 2020 2020  edata:..        
-00018220: 2020 2020 2020 2020 6966 2073 7472 2866          if str(f
-00018230: 696c 6564 6174 615b 2263 6173 6866 6c6f  iledata["cashflo
-00018240: 7731 225d 2920 213d 2027 4e6f 6e65 273a  w1"]) != 'None':
-00018250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018260: 2020 2020 2020 636f 6d6d 616e 6473 2e61        commands.a
-00018270: 7070 656e 6428 2225 732e 6361 7368 5f66  ppend("%s.cash_f
-00018280: 6c6f 775f 7374 6174 656d 656e 742e 6e65  low_statement.ne
-00018290: 775f 656e 7472 7928 2573 2c27 2573 272c  w_entry(%s,'%s',
-000182a0: 2d25 7329 2220 2520 2861 6765 6e74 312c  -%s)" % (agent1,
-000182b0: 2243 6173 6846 6c6f 7745 6e74 7279 2e22  "CashFlowEntry."
-000182c0: 202b 2066 696c 6564 6174 615b 2263 6173   + filedata["cas
-000182d0: 6866 6c6f 7731 225d 2e75 7070 6572 2829  hflow1"].upper()
-000182e0: 2c73 7562 6a65 6374 2c71 7561 6e74 6974  ,subject,quantit
-000182f0: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
-00018300: 2020 2069 6620 2263 6173 6866 6c6f 7732     if "cashflow2
-00018310: 2220 696e 2066 696c 6564 6174 613a 0d0a  " in filedata:..
-00018320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018330: 6966 2073 7472 2866 696c 6564 6174 615b  if str(filedata[
-00018340: 2263 6173 6866 6c6f 7732 225d 2920 213d  "cashflow2"]) !=
-00018350: 2027 4e6f 6e65 273a 0d0a 2020 2020 2020   'None':..      
-00018360: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00018370: 6d6d 616e 6473 2e61 7070 656e 6428 2225  mmands.append("%
-00018380: 732e 6361 7368 5f66 6c6f 775f 7374 6174  s.cash_flow_stat
-00018390: 656d 656e 742e 6e65 775f 656e 7472 7928  ement.new_entry(
-000183a0: 2573 2c27 2573 272c 2573 2922 2025 2028  %s,'%s',%s)" % (
-000183b0: 6167 656e 7432 2c22 4361 7368 466c 6f77  agent2,"CashFlow
-000183c0: 456e 7472 792e 2220 2b20 6669 6c65 6461  Entry." + fileda
-000183d0: 7461 5b22 6361 7368 666c 6f77 3222 5d2e  ta["cashflow2"].
-000183e0: 7570 7065 7228 292c 7375 626a 6563 742c  upper(),subject,
-000183f0: 7175 616e 7469 7479 2929 0d0a 0d0a 2020  quantity))....  
-00018400: 2020 2020 2020 2020 2020 6966 2054 7275            if Tru
-00018410: 653a 2023 2061 6765 6e74 3120 213d 2061  e: # agent1 != a
-00018420: 6765 6e74 323a 0d0a 2020 2020 2020 2020  gent2:..        
-00018430: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
-00018440: 2022 6465 6620 2573 2825 732c 2025 732c   "def %s(%s, %s,
-00018450: 2025 7329 3a5c 6e22 2025 2028 7375 626a   %s):\n" % (subj
-00018460: 6563 742c 6167 656e 7431 2c61 6765 6e74  ect,agent1,agent
-00018470: 322c 7175 616e 7469 7479 290d 0a20 2020  2,quantity)..   
-00018480: 2020 2020 2020 2020 2023 656c 7365 3a0d           #else:.
-00018490: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-000184a0: 2020 6d65 7468 6f64 203d 2022 6465 6620    method = "def 
-000184b0: 2573 2825 732c 2025 7329 3a5c 6e22 2025  %s(%s, %s):\n" %
-000184c0: 2028 7375 626a 6563 742c 2061 6765 6e74   (subject, agent
-000184d0: 312c 2071 7561 6e74 6974 7929 0d0a 0d0a  1, quantity)....
-000184e0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-000184f0: 6465 7363 7269 7074 696f 6e22 2069 6e20  description" in 
-00018500: 6669 6c65 6461 7461 3a20 2320 6164 6420  filedata: # add 
-00018510: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-00018520: 696e 2074 6865 2064 6f63 7374 7269 6e67  in the docstring
-00018530: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-00018540: 2064 6566 696e 6974 696f 6e0d 0a20 2020   definition..   
-00018550: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00018560: 686f 6420 2b3d 2022 2020 2020 2322 202b  hod += "    #" +
-00018570: 2066 696c 6564 6174 615b 2264 6573 6372   filedata["descr
-00018580: 6970 7469 6f6e 225d 202b 2022 5c6e 220d  iption"] + "\n".
-00018590: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-000185a0: 6f72 2063 6f6d 6d61 6e64 2069 6e20 636f  or command in co
-000185b0: 6d6d 616e 6473 3a0d 0a20 2020 2020 2020  mmands:..       
-000185c0: 2020 2020 2020 2020 206d 6574 686f 6420           method 
-000185d0: 2b3d 2022 2020 2020 2220 2b20 636f 6d6d  += "    " + comm
-000185e0: 616e 6420 2b20 225c 6e22 0d0a 0d0a 2020  and + "\n"....  
-000185f0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-00018600: 202b 3d20 225c 6e5c 6e22 0d0a 2020 2020   += "\n\n"..    
-00018610: 2020 2020 2020 2020 636f 6465 202b 3d20          code += 
-00018620: 6d65 7468 6f64 0d0a 0d0a 2020 2020 2020  method....      
-00018630: 2020 666f 6c64 6572 203d 206f 732e 7061    folder = os.pa
-00018640: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
-00018650: 6375 7272 656e 745f 6669 6c65 2920 2320  current_file) # 
-00018660: 7374 6174 7573 4261 7228 292e 6375 7272  statusBar().curr
-00018670: 656e 744d 6573 7361 6765 2829 290d 0a20  entMessage()).. 
-00018680: 2020 2020 2020 2066 6e61 6d65 203d 2020         fname =  
-00018690: 666f 6c64 6572 202b 2022 2f70 7974 686f  folder + "/pytho
-000186a0: 6e5f 636f 6465 2f74 7261 6e73 6163 7469  n_code/transacti
-000186b0: 6f6e 732e 7079 220d 0a0d 0a20 2020 2020  ons.py"....     
-000186c0: 2020 2077 6974 6820 6f70 656e 2866 6e61     with open(fna
-000186d0: 6d65 2c22 7722 2c65 6e63 6f64 696e 673d  me,"w",encoding=
-000186e0: 2275 7466 2d38 2229 2061 7320 6669 6c65  "utf-8") as file
-000186f0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00018700: 696c 652e 7772 6974 6528 636f 6465 290d  ile.write(code).
-00018710: 0a0d 0a20 2020 2020 2020 2069 6620 7368  ...        if sh
-00018720: 6f77 5f6e 6f74 6966 6963 6174 696f 6e3a  ow_notification:
-00018730: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00018740: 6c66 2e6e 6f74 6966 7928 6d65 7373 6167  lf.notify(messag
-00018750: 653d 2243 6f64 6520 6578 706f 7274 6564  e="Code exported
-00018760: 2074 6f20 2573 2220 2520 2866 6e61 6d65   to %s" % (fname
-00018770: 292c 7469 746c 653d 2253 7563 6365 7373  ),title="Success
-00018780: 2229 0d0a 0d0a 0d0a 2020 2020 6465 6620  ")......    def 
-00018790: 6765 6e5f 6963 735f 7369 6e67 6c65 2873  gen_ics_single(s
-000187a0: 656c 6629 3a0d 0a20 2020 2020 2020 2069  elf):..        i
-000187b0: 6620 7365 6c66 2e64 7261 7763 616e 7661  f self.drawcanva
-000187c0: 732e 6869 6768 6c69 6768 7465 6420 6973  s.highlighted is
-000187d0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000187e0: 2020 2020 7365 6c66 2e6e 6f74 6966 7928      self.notify(
-000187f0: 7469 746c 653d 224e 6f20 6167 656e 7420  title="No agent 
-00018800: 7365 6c65 6374 6564 222c 206d 6573 7361  selected", messa
-00018810: 6765 3d22 4e6f 2061 6765 6e74 2073 656c  ge="No agent sel
-00018820: 6563 7465 642e 2050 6c65 6173 6520 7365  ected. Please se
-00018830: 6c65 6374 206f 6e65 2066 6972 7374 2e22  lect one first."
-00018840: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00018850: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
-00018860: 6620 7365 6c66 2e64 7261 7763 616e 7661  f self.drawcanva
-00018870: 732e 6869 6768 6c69 6768 7465 642e 6973  s.highlighted.is
-00018880: 6865 6c70 6572 3a0d 0a20 2020 2020 2020  helper:..       
-00018890: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
-000188a0: 2874 6974 6c65 3d22 4e6f 2061 6765 6e74  (title="No agent
-000188b0: 2073 656c 6563 7465 6422 2c20 6d65 7373   selected", mess
-000188c0: 6167 653d 224e 6f20 7661 6c69 6420 626f  age="No valid bo
-000188d0: 7820 7365 6c65 6374 6564 2e20 506c 6561  x selected. Plea
-000188e0: 7365 2073 656c 6563 7420 616e 2061 6765  se select an age
-000188f0: 6e74 2e22 290d 0a20 2020 2020 2020 2020  nt.")..         
-00018900: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00018910: 2020 206d 795f 6167 656e 7420 3d20 7365     my_agent = se
-00018920: 6c66 2e64 7261 7763 616e 7661 732e 6869  lf.drawcanvas.hi
-00018930: 6768 6c69 6768 7465 642e 6e61 6d65 0d0a  ghlighted.name..
-00018940: 0d0a 2020 2020 2020 2020 636f 6d62 696e  ..        combin
-00018950: 6564 5f69 6e63 6f6d 6520 3d20 207b 2253  ed_income =  {"S
-00018960: 7562 6a65 6374 223a 5b5d 2c22 5368 6f72  ubject":[],"Shor
-00018970: 7420 4e61 6d65 223a 205b 5d2c 2251 7561  t Name": [],"Qua
-00018980: 6e74 6974 7922 3a5b 5d2c 2022 5479 7065  ntity":[], "Type
-00018990: 223a 5b5d 2c20 2252 616e 6b69 6e67 223a  ":[], "Ranking":
-000189a0: 5b5d 7d20 2320 7261 6e6b 696e 6720 7769  []} # ranking wi
-000189b0: 6c6c 2062 6520 7265 6d6f 7665 6420 6c61  ll be removed la
-000189c0: 7465 720d 0a20 2020 2020 2020 2022 2222  ter..        """
-000189d0: 0d0a 2020 2020 2020 2020 2247 6169 6e73  ..        "Gains
-000189e0: 223a 205b 5d2c 2022 4c6f 7373 6573 223a  ": [], "Losses":
-000189f0: 205b 5d2c 2022 5265 7665 6e75 6573 223a   [], "Revenues":
-00018a00: 205b 5d2c 2022 5461 7865 7322 3a20 5b5d   [], "Taxes": []
-00018a10: 2c20 2245 7870 656e 7365 7322 3a20 5b5d  , "Expenses": []
-00018a20: 2c0d 0a20 2020 2020 2020 2020 224e 6f6e  ,..         "Non
-00018a30: 7461 7861 626c 6520 4c6f 7373 6573 223a  taxable Losses":
-00018a40: 205b 5d2c 2022 4e6f 6e74 6178 6162 6c65   [], "Nontaxable
-00018a50: 2050 726f 6669 7473 223a 205b 5d2c 0d0a   Profits": [],..
-00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00018a80: 4e6f 6e2d 4f70 6572 6174 696f 6e61 6c20  Non-Operational 
-00018a90: 496e 636f 6d65 223a 205b 5d2c 0d0a 2020  Income": [],..  
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ac0: 2020 2020 2020 2020 2020 2020 2022 496e               "In
-00018ad0: 7465 7265 7374 2050 6179 6d65 6e74 7322  terest Payments"
-00018ae0: 3a20 5b5d 0d0a 2020 2020 2020 2020 2020  : []..          
-00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ea0: 236f 732e 7374 6172 7466 696c 6528 6f73  #os.startfile(os
+00015eb0: 2e67 6574 6377 6428 2920 2b20 225c 5c6d  .getcwd() + "\\m
+00015ec0: 796d 6174 7269 782e 7064 6622 290d 0a20  ymatrix.pdf").. 
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00015ee0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00015ef0: 2020 2020 2020 2020 2023 2073 6875 7469           # shuti
+00015f00: 6c2e 726d 7472 6565 286f 732e 6765 7463  l.rmtree(os.getc
+00015f10: 7764 2829 2b22 5c5c 6669 6c65 7322 290d  wd()+"\\files").
+00015f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f30: 2020 2020 2023 206f 732e 6d6b 6469 7228       # os.mkdir(
+00015f40: 6f73 2e67 6574 6377 6428 292b 225c 5c66  os.getcwd()+"\\f
+00015f50: 696c 6573 2229 0d0a 0d0a 2020 2020 2020  iles")....      
+00015f60: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00015f70: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+00015f80: 6e61 6d65 286f 732e 7061 7468 2e61 6273  name(os.path.abs
+00015f90: 7061 7468 285f 5f66 696c 655f 5f29 290d  path(__file__)).
+00015fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015fb0: 2020 2020 2073 6875 7469 6c2e 6d6f 7665       shutil.move
+00015fc0: 2870 6174 682b 225c 5c6d 796d 6174 7269  (path+"\\mymatri
+00015fd0: 782e 7465 7822 202c 2070 6174 682b 2022  x.tex" , path+ "
+00015fe0: 5c5c 6669 6c65 735c 5c6d 796d 6174 7269  \\files\\mymatri
+00015ff0: 782e 7465 7822 290d 0a20 2020 2020 2020  x.tex")..       
+00016000: 2020 2020 2020 2020 2020 2020 2073 6875               shu
+00016010: 7469 6c2e 6d6f 7665 2870 6174 6820 2b20  til.move(path + 
+00016020: 225c 5c6d 796d 6174 7269 782e 6c6f 6722  "\\mymatrix.log"
+00016030: 2c20 7061 7468 202b 2022 5c5c 6669 6c65  , path + "\\file
+00016040: 735c 5c6d 796d 6174 7269 782e 6c6f 6722  s\\mymatrix.log"
+00016050: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016060: 2020 2020 2020 2073 6875 7469 6c2e 6d6f         shutil.mo
+00016070: 7665 2870 6174 6820 2b20 225c 5c6d 796d  ve(path + "\\mym
+00016080: 6174 7269 782e 6175 7822 2c20 7061 7468  atrix.aux", path
+00016090: 202b 2022 5c5c 6669 6c65 735c 5c5c 6d79   + "\\files\\\my
+000160a0: 6d61 7472 6978 2e61 7578 2229 0d0a 2020  matrix.aux")..  
+000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160c0: 2020 7368 7574 696c 2e6d 6f76 6528 7061    shutil.move(pa
+000160d0: 7468 202b 2022 5c5c 6d79 6d61 7472 6978  th + "\\mymatrix
+000160e0: 2e70 6466 222c 2070 6174 6820 2b20 225c  .pdf", path + "\
+000160f0: 5c66 696c 6573 5c5c 6d79 6d61 7472 6978  \files\\mymatrix
+00016100: 2e70 6466 2229 0d0a 2020 2020 2020 2020  .pdf")..        
+00016110: 2020 2020 2020 2020 2020 2020 2373 6875              #shu
+00016120: 7469 6c2e 636f 7079 286f 732e 6765 7463  til.copy(os.getc
+00016130: 7764 2829 202b 2022 5c5c 6669 6c65 735c  wd() + "\\files\
+00016140: 5c6d 796d 6174 7269 782e 6874 6d6c 222c  \mymatrix.html",
+00016150: 6f73 2e67 6574 6377 6428 2920 2b20 225c  os.getcwd() + "\
+00016160: 5c66 696c 6573 5c5c 6d79 6d61 7472 6978  \files\\mymatrix
+00016170: 2e68 746d 6c22 290d 0a20 2020 2020 2020  .html")..       
+00016180: 2020 2020 2020 2020 2020 2020 2023 7368               #sh
+00016190: 7574 696c 2e63 6f70 7928 6f73 2e67 6574  util.copy(os.get
+000161a0: 6377 6428 2920 2b20 225c 5c66 696c 6573  cwd() + "\\files
+000161b0: 5c5c 6d79 7374 796c 652e 6373 7322 2c20  \\mystyle.css", 
+000161c0: 6f73 2e67 6574 6377 6428 2920 2b20 225c  os.getcwd() + "\
+000161d0: 5c66 696c 6573 5c5c 6d79 7374 796c 652e  \files\\mystyle.
+000161e0: 6373 7322 290d 0a20 2020 2020 2020 2020  css")..         
+000161f0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00016200: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016220: 2020 2073 656c 662e 6e6f 7469 6679 286d     self.notify(m
+00016230: 6573 7361 6765 3d73 7472 2865 292c 7469  essage=str(e),ti
+00016240: 746c 653d 2241 6e20 4572 726f 7220 6f63  tle="An Error oc
+00016250: 6375 7272 6564 2e2e 2e28 4944 2031 3330  curred...(ID 130
+00016260: 3829 2229 0d0a 0d0a 2020 2020 2020 2020  8)")....        
+00016270: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00016280: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+00016290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000162a0: 2e6e 6f74 6966 7928 6d65 7373 6167 653d  .notify(message=
+000162b0: 7374 7228 6529 2c74 6974 6c65 3d22 416e  str(e),title="An
+000162c0: 2045 7272 6f72 206f 6363 7572 7265 642e   Error occurred.
+000162d0: 2e2e 2849 4420 3133 3131 2922 290d 0a20  ..(ID 1311)").. 
+000162e0: 2020 2020 2020 2020 2020 2023 202d 2d2d             # ---
+000162f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 2020  ----------....  
+00016300: 2020 2020 2020 2020 2020 7064 2e6f 7074            pd.opt
+00016310: 696f 6e73 2e64 6973 706c 6179 2e6d 6178  ions.display.max
+00016320: 5f63 6f6c 7769 6474 6820 3d20 320d 0a0d  _colwidth = 2...
+00016330: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
+00016340: 6469 7370 6c61 7920 3d20 6466 5f62 6163  display = df_bac
+00016350: 6b75 702e 6170 706c 796d 6170 2861 6262  kup.applymap(abb
+00016360: 7265 7669 6174 655f 7a65 726f 7329 2e74  reviate_zeros).t
+00016370: 6f5f 7374 7269 6e67 286c 696e 655f 7769  o_string(line_wi
+00016380: 6474 683d 4e6f 6e65 292e 7265 706c 6163  dth=None).replac
+00016390: 6528 225c 5f22 2c20 225f 2229 0d0a 0d0a  e("\_", "_")....
+000163a0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+000163b0: 6c66 2e70 6172 656e 742e 7061 7265 6e74  lf.parent.parent
+000163c0: 4170 702e 6765 7446 6f72 6d28 2241 4747  App.getForm("AGG
+000163d0: 525f 464c 4f57 2229 2e64 6174 615f 626f  R_FLOW").data_bo
+000163e0: 782e 7661 6c75 6573 203d 2064 665f 6469  x.values = df_di
+000163f0: 7370 6c61 792e 7370 6c69 7428 225c 6e22  splay.split("\n"
+00016400: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00016410: 2073 656c 662e 7061 7265 6e74 2e70 6172   self.parent.par
+00016420: 656e 7441 7070 2e73 7769 7463 6846 6f72  entApp.switchFor
+00016430: 6d28 2241 4747 525f 464c 4f57 2229 0d0a  m("AGGR_FLOW")..
+00016440: 0d0a 0d0a 2020 2020 6465 6620 6765 6e5f  ....    def gen_
+00016450: 636f 6465 2873 656c 662c 7368 6f77 5f6e  code(self,show_n
+00016460: 6f74 6966 6963 6174 696f 6e3d 4661 6c73  otification=Fals
+00016470: 6529 3a0d 0a0d 0a20 2020 2020 2020 2063  e):....        c
+00016480: 6f64 6520 3d20 2222 0d0a 2020 2020 2020  ode = ""..      
+00016490: 2020 636f 6465 202b 3d20 2266 726f 6d20    code += "from 
+000164a0: 7366 6374 6f6f 6c73 2069 6d70 6f72 7420  sfctools import 
+000164b0: 466c 6f77 4d61 7472 6978 205c 6e69 6d70  FlowMatrix \nimp
+000164c0: 6f72 7420 6e75 6d70 7920 6173 206e 705c  ort numpy as np\
+000164d0: 6e22 0d0a 2020 2020 2020 2020 636f 6465  n"..        code
+000164e0: 202b 3d20 2266 726f 6d20 7366 6374 6f6f   += "from sfctoo
+000164f0: 6c73 2069 6d70 6f72 7420 4261 6c61 6e63  ls import Balanc
+00016500: 6545 6e74 7279 2c41 6363 6f75 6e74 735c  eEntry,Accounts\
+00016510: 6e22 0d0a 2020 2020 2020 2020 636f 6465  n"..        code
+00016520: 202b 3d20 2266 726f 6d20 7366 6374 6f6f   += "from sfctoo
+00016530: 6c73 2069 6d70 6f72 7420 4361 7368 466c  ls import CashFl
+00016540: 6f77 456e 7472 795c 6e22 0d0a 2020 2020  owEntry\n"..    
+00016550: 2020 2020 636f 6465 202b 3d20 2266 726f      code += "fro
+00016560: 6d20 7366 6374 6f6f 6c73 2069 6d70 6f72  m sfctools impor
+00016570: 7420 4943 5345 6e74 7279 5c6e 220d 0a20  t ICSEntry\n".. 
+00016580: 2020 2020 2020 2063 6f64 6520 2b3d 2022         code += "
+00016590: 4341 203d 2041 6363 6f75 6e74 732e 4341  CA = Accounts.CA
+000165a0: 5c6e 4b41 203d 2041 6363 6f75 6e74 732e  \nKA = Accounts.
+000165b0: 4b41 5c6e 5c6e 220d 0a0d 0a20 2020 2020  KA\n\n"....     
+000165c0: 2020 2073 7562 6a65 6374 735f 636f 756e     subjects_coun
+000165d0: 7420 3d20 6465 6661 756c 7464 6963 7428  t = defaultdict(
+000165e0: 6c61 6d62 6461 3a20 302e 3029 0d0a 0d0a  lambda: 0.0)....
+000165f0: 2020 2020 2020 2020 666f 7220 6669 6c65          for file
+00016600: 6461 7461 2069 6e20 7365 6c66 2e65 6e74  data in self.ent
+00016610: 7279 5f64 6174 613a 0d0a 2020 2020 2020  ry_data:..      
+00016620: 2020 2020 2020 6167 656e 7431 203d 2066        agent1 = f
+00016630: 696c 6564 6174 615b 2261 6765 6e74 3122  iledata["agent1"
+00016640: 5d0d 0a20 2020 2020 2020 2020 2020 2061  ]..            a
+00016650: 6765 6e74 3220 3d20 6669 6c65 6461 7461  gent2 = filedata
+00016660: 5b22 6167 656e 7432 225d 0d0a 0d0a 2020  ["agent2"]....  
+00016670: 2020 2020 2020 2020 2020 6966 2061 6765            if age
+00016680: 6e74 3120 3d3d 2061 6765 6e74 323a 0d0a  nt1 == agent2:..
+00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166a0: 6167 656e 7432 203d 2022 6f74 6865 725f  agent2 = "other_
+000166b0: 2220 2b20 6167 656e 7432 0d0a 0d0a 2020  " + agent2....  
+000166c0: 2020 2020 2020 2020 2020 6131 203d 2066            a1 = f
+000166d0: 696c 6564 6174 615b 2261 3122 5d20 2023  iledata["a1"]  #
+000166e0: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
+000166f0: 2020 2020 2065 3120 3d20 6669 6c65 6461       e1 = fileda
+00016700: 7461 5b22 6531 225d 2020 2320 2b20 225c  ta["e1"]  # + "\
+00016710: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
+00016720: 6c31 203d 2066 696c 6564 6174 615b 226c  l1 = filedata["l
+00016730: 3122 5d20 2023 202b 2022 5c6e 220d 0a20  1"]  # + "\n".. 
+00016740: 2020 2020 2020 2020 2020 2061 3220 3d20             a2 = 
+00016750: 6669 6c65 6461 7461 5b22 6132 225d 2020  filedata["a2"]  
+00016760: 2320 2b20 225c 6e22 0d0a 2020 2020 2020  # + "\n"..      
+00016770: 2020 2020 2020 6532 203d 2066 696c 6564        e2 = filed
+00016780: 6174 615b 2265 3222 5d20 2023 202b 2022  ata["e2"]  # + "
+00016790: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
+000167a0: 206c 3220 3d20 6669 6c65 6461 7461 5b22   l2 = filedata["
+000167b0: 6c32 225d 2020 2320 2b20 225c 6e22 0d0a  l2"]  # + "\n"..
+000167c0: 0d0a 2020 2020 2020 2020 2020 2020 666c  ..            fl
+000167d0: 6f77 5f63 6865 636b 203d 2054 7275 650d  ow_check = True.
+000167e0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000167f0: 6e74 2822 464c 4f57 2043 4845 434b 222c  nt("FLOW CHECK",
+00016800: 2066 696c 6564 6174 615b 2273 686f 7274   filedata["short
+00016810: 6e61 6d65 225d 2c66 696c 6564 6174 615b  name"],filedata[
+00016820: 226c 6f67 2074 7261 6e73 6163 7469 6f6e  "log transaction
+00016830: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+00016840: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
+00016850: 696c 6564 6174 615b 226c 6f67 2074 7261  iledata["log tra
+00016860: 6e73 6163 7469 6f6e 225d 2c73 7472 2920  nsaction"],str) 
+00016870: 616e 6420 6669 6c65 6461 7461 5b22 6c6f  and filedata["lo
+00016880: 6720 7472 616e 7361 6374 696f 6e22 5d2e  g transaction"].
+00016890: 7374 7269 7028 2920 3d3d 2022 5472 7565  strip() == "True
+000168a0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+000168b0: 2020 2020 2320 626f 6f6c 2866 696c 6564      # bool(filed
+000168c0: 6174 615b 226c 6f67 2074 7261 6e73 6163  ata["log transac
+000168d0: 7469 6f6e 225d 290d 0a20 2020 2020 2020  tion"])..       
+000168e0: 2020 2020 2020 2020 2066 6c6f 775f 6368           flow_ch
+000168f0: 6563 6b20 3d20 5472 7565 0d0a 2020 2020  eck = True..    
+00016900: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00016910: 7428 666c 6f77 5f63 6865 636b 290d 0a20  t(flow_check).. 
+00016920: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00016930: 6973 696e 7374 616e 6365 2866 696c 6564  isinstance(filed
+00016940: 6174 615b 226c 6f67 2074 7261 6e73 6163  ata["log transac
+00016950: 7469 6f6e 225d 2c73 7472 2920 616e 6420  tion"],str) and 
+00016960: 6669 6c65 6461 7461 5b22 6c6f 6720 7472  filedata["log tr
+00016970: 616e 7361 6374 696f 6e22 5d2e 7374 7269  ansaction"].stri
+00016980: 7028 2920 3d3d 2022 4661 6c73 6522 3a0d  p() == "False":.
+00016990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000169a0: 2023 2062 6f6f 6c28 6669 6c65 6461 7461   # bool(filedata
+000169b0: 5b22 6c6f 6720 7472 616e 7361 6374 696f  ["log transactio
+000169c0: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
+000169d0: 2020 2020 2020 666c 6f77 5f63 6865 636b        flow_check
+000169e0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+000169f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00016a00: 666c 6f77 5f63 6865 636b 290d 0a20 2020  flow_check)..   
+00016a10: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a30: 666c 6f77 5f63 6865 636b 203d 2066 696c  flow_check = fil
+00016a40: 6564 6174 615b 226c 6f67 2074 7261 6e73  edata["log trans
+00016a50: 6163 7469 6f6e 225d 0d0a 2020 2020 2020  action"]..      
+00016a60: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00016a70: 666c 6f77 5f63 6865 636b 290d 0a20 2020  flow_check)..   
+00016a80: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
+00016a90: 2246 4c4f 5720 4348 4543 4b22 2c20 6669  "FLOW CHECK", fi
+00016aa0: 6c65 6e61 6d65 2c20 666c 6f77 5f63 6865  lename, flow_che
+00016ab0: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+00016ac0: 2070 7269 6e74 2822 7479 7065 222c 2074   print("type", t
+00016ad0: 7970 6528 666c 6f77 5f63 6865 636b 2929  ype(flow_check))
+00016ae0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016af0: 6b69 6e64 203d 2066 696c 6564 6174 615b  kind = filedata[
+00016b00: 226b 696e 6422 5d0d 0a0d 0a20 2020 2020  "kind"]....     
+00016b10: 2020 2020 2020 2023 7375 626a 6563 7420         #subject 
+00016b20: 3d20 2066 696c 6564 6174 615b 2273 7562  =  filedata["sub
+00016b30: 6a65 6374 225d 2e72 6570 6c61 6365 2822  ject"].replace("
+00016b40: 2022 2c22 5f22 2920 2b20 225f 2220 2b20   ","_") + "_" + 
+00016b50: 6669 6c65 6461 7461 5b22 7368 6f72 746e  filedata["shortn
+00016b60: 616d 6522 2e72 6570 6c61 6365 2822 2022  ame".replace(" "
+00016b70: 2c22 5f22 295d 2e6c 6f77 6572 2829 0d0a  ,"_")].lower()..
+00016b80: 2020 2020 2020 2020 2020 2020 7375 626a              subj
+00016b90: 6563 7420 3d20 2066 696c 6564 6174 615b  ect =  filedata[
+00016ba0: 2273 686f 7274 6e61 6d65 222e 7265 706c  "shortname".repl
+00016bb0: 6163 6528 2220 222c 225f 2229 5d2e 7265  ace(" ","_")].re
+00016bc0: 706c 6163 6528 2228 222c 225f 2229 2e72  place("(","_").r
+00016bd0: 6570 6c61 6365 2822 2922 2c22 2229 2e6c  eplace(")","").l
+00016be0: 6f77 6572 2829 0d0a 2020 2020 2020 2020  ower()..        
+00016bf0: 2020 2020 7375 626a 6563 745f 7374 7220      subject_str 
+00016c00: 3d20 2066 696c 6564 6174 615b 2273 7562  =  filedata["sub
+00016c10: 6a65 6374 222e 7265 706c 6163 6528 2220  ject".replace(" 
+00016c20: 222c 225f 2229 5d2e 6c6f 7765 7228 292e  ","_")].lower().
+00016c30: 6361 7069 7461 6c69 7a65 2829 2e72 6570  capitalize().rep
+00016c40: 6c61 6365 2822 5f22 2c20 2220 2229 0d0a  lace("_", " ")..
+00016c50: 0d0a 2020 2020 2020 2020 2020 2020 7375  ..            su
+00016c60: 626a 6563 7473 5f63 6f75 6e74 5b73 7562  bjects_count[sub
+00016c70: 6a65 6374 5d20 2b3d 2031 0d0a 2020 2020  ject] += 1..    
+00016c80: 2020 2020 2020 2020 6966 2073 7562 6a65          if subje
+00016c90: 6374 735f 636f 756e 745b 7375 626a 6563  cts_count[subjec
+00016ca0: 745d 203e 2031 3a20 2320 7375 6666 6978  t] > 1: # suffix
+00016cb0: 2066 6f72 2073 616d 6520 6e61 6d65 730d   for same names.
+00016cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016cd0: 2073 7562 6a65 6374 202b 3d20 225f 2569   subject += "_%i
+00016ce0: 2220 2520 696e 7428 7375 626a 6563 7473  " % int(subjects
+00016cf0: 5f63 6f75 6e74 5b73 7562 6a65 6374 5d29  _count[subject])
+00016d00: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00016d10: 2020 7175 616e 7469 7479 203d 2022 7122    quantity = "q"
+00016d20: 2023 2066 696c 6564 6174 615b 2271 7561   # filedata["qua
+00016d30: 6e74 6974 7922 5d0d 0a0d 0a20 2020 2020  ntity"]....     
+00016d40: 2020 2020 2020 2063 6f6d 6d61 6e64 7320         commands 
+00016d50: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016d60: 2020 2020 6966 2022 756e 692d 6469 7265      if "uni-dire
+00016d70: 6374 696f 6e61 6c22 2069 6e20 6669 6c65  ctional" in file
+00016d80: 6461 7461 3a0d 0a20 2020 2020 2020 2020  data:..         
+00016d90: 2020 2020 2020 2075 6e69 6469 7220 3d20         unidir = 
+00016da0: 6669 6c65 6461 7461 5b22 756e 692d 6469  filedata["uni-di
+00016db0: 7265 6374 696f 6e61 6c22 5d0d 0a0d 0a20  rectional"].... 
+00016dc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00016dd0: 6f6d 6d61 6e64 732e 6170 7065 6e64 2822  ommands.append("
+00016de0: 636f 6e64 203d 2028 6973 696e 7374 616e  cond = (isinstan
+00016df0: 6365 2871 2c66 6c6f 6174 2920 6f72 2069  ce(q,float) or i
+00016e00: 7369 6e73 7461 6e63 6528 712c 696e 7429  sinstance(q,int)
+00016e10: 2922 290d 0a20 2020 2020 2020 2020 2020  )")..           
+00016e20: 2020 2020 2063 6f6d 6d61 6e64 732e 6170       commands.ap
+00016e30: 7065 6e64 2822 6966 2063 6f6e 643a 2061  pend("if cond: a
+00016e40: 7373 6572 7420 6e6f 7420 6e70 2e69 736e  ssert not np.isn
+00016e50: 616e 2871 2922 290d 0a20 2020 2020 2020  an(q)")..       
+00016e60: 2020 2020 2020 2020 2023 205e 2077 696c           # ^ wil
+00016e70: 6c20 616c 736f 2070 6173 7320 666f 7220  l also pass for 
+00016e80: 6e70 2e66 6c6f 6174 3634 0d0a 2020 2020  np.float64..    
+00016e90: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+00016ea0: 616e 6473 2e61 7070 656e 6428 2269 6620  ands.append("if 
+00016eb0: 636f 6e64 3a20 6173 7365 7274 2071 203c  cond: assert q <
+00016ec0: 202b 6e70 2e69 6e66 2229 0d0a 2020 2020   +np.inf")..    
+00016ed0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+00016ee0: 616e 6473 2e61 7070 656e 6428 2269 6620  ands.append("if 
+00016ef0: 636f 6e64 3a20 6173 7365 7274 2071 203e  cond: assert q >
+00016f00: 202d 6e70 2e69 6e66 2229 0d0a 0d0a 2020   -np.inf")....  
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2370                #p
+00016f20: 7269 6e74 2822 756e 692d 6469 7265 6374  rint("uni-direct
+00016f30: 696f 6e61 6c22 2c75 6e69 6469 7229 0d0a  ional",unidir)..
+00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f50: 6966 2073 7472 2875 6e69 6469 7229 203d  if str(unidir) =
+00016f60: 3d20 2254 7275 6522 3a20 2320 646f 206e  = "True": # do n
+00016f70: 6f74 2064 6f20 626f 6f6c 2875 6e69 6469  ot do bool(unidi
+00016f80: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+00016f90: 2020 2020 2020 2020 236e 616d 6161 6120          #namaaa 
+00016fa0: 3d20 6669 6c65 6461 7461 5b22 7368 6f72  = filedata["shor
+00016fb0: 746e 616d 6522 5d0d 0a20 2020 2020 2020  tname"]..       
+00016fc0: 2020 2020 2020 2020 2020 2020 2023 7365               #se
+00016fd0: 6c66 2e6e 6f74 6966 7928 2028 6e61 6d61  lf.notify( (nama
+00016fe0: 6161 2b20 7374 7228 756e 6964 6972 292b  aa+ str(unidir)+
+00016ff0: 2022 3d22 2b28 7374 7228 626f 6f6c 2875   "="+(str(bool(u
+00017000: 6e69 6469 7229 2929 292c 7469 746c 653d  nidir)))),title=
+00017010: 2263 6865 636b 2229 0d0a 2020 2020 2020  "check")..      
+00017020: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00017030: 6d6d 616e 6473 2e61 7070 656e 6428 2269  mmands.append("i
+00017040: 6620 636f 6e64 3a20 6173 7365 7274 2071  f cond: assert q
+00017050: 203e 3d20 302c 2027 6861 7665 2074 6f20   >= 0, 'have to 
+00017060: 7061 7373 2070 6f73 6974 6976 6520 7175  pass positive qu
+00017070: 616e 7469 7479 3a20 756e 6964 6972 6563  antity: unidirec
+00017080: 7469 6f6e 616c 2074 7261 6e73 6163 7469  tional transacti
+00017090: 6f6e 2722 290d 0a0d 0a20 2020 2020 2020  on'")....       
+000170a0: 2020 2020 2063 6f6d 6d61 6e64 7320 3d20       commands = 
+000170b0: 636f 6d6d 616e 6473 202b 205b 2225 732e  commands + ["%s.
+000170c0: 6261 6c61 6e63 655f 7368 6565 742e 6469  balance_sheet.di
+000170d0: 7365 6e67 6167 6528 2922 2025 2061 6765  sengage()" % age
+000170e0: 6e74 315d 0d0a 2020 2020 2020 2020 2020  nt1]..          
+000170f0: 2020 6966 2054 7275 653a 2023 2061 6765    if True: # age
+00017100: 6e74 3120 213d 2061 6765 6e74 323a 0d0a  nt1 != agent2:..
+00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017120: 636f 6d6d 616e 6473 2b3d 205b 2225 732e  commands+= ["%s.
+00017130: 6261 6c61 6e63 655f 7368 6565 742e 6469  balance_sheet.di
+00017140: 7365 6e67 6167 6528 2922 2025 2061 6765  sengage()" % age
+00017150: 6e74 325d 0d0a 0d0a 2020 2020 2020 2020  nt2]....        
+00017160: 2020 2020 666f 7220 656e 7472 7920 696e      for entry in
+00017170: 2065 312e 7370 6c69 7428 225c 6e22 293a   e1.split("\n"):
+00017180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017190: 2020 6966 2065 6e74 7279 2021 3d20 2222    if entry != ""
+000171a0: 2061 6e64 2065 6e74 7279 2021 3d20 225c   and entry != "\
+000171b0: 6e22 3a0d 0a20 2020 2020 2020 2020 2020  n":..           
+000171c0: 2020 2020 2020 2020 2073 6967 6e2c 2069           sign, i
+000171d0: 7465 6d2c 2073 696c 656e 7420 3d20 7365  tem, silent = se
+000171e0: 6c66 2e65 6e74 7279 5f74 6f5f 7661 6c73  lf.entry_to_vals
+000171f0: 2865 6e74 7279 2c20 6167 656e 7431 2c20  (entry, agent1, 
+00017200: 2245 7175 6974 7922 290d 0a20 2020 2020  "Equity")..     
+00017210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017220: 6620 7369 676e 2069 7320 6e6f 7420 4e6f  f sign is not No
+00017230: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00017240: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00017250: 6d61 6e64 732e 6170 7065 6e64 2822 2573  mands.append("%s
+00017260: 2e62 616c 616e 6365 5f73 6865 6574 2e63  .balance_sheet.c
+00017270: 6861 6e67 655f 6974 656d 2827 2573 272c  hange_item('%s',
+00017280: 2025 732c 2025 732c 2073 7570 7072 6573   %s, %s, suppres
+00017290: 735f 7374 6f63 6b3d 2573 2922 2025 2028  s_stock=%s)" % (
+000172a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000172b0: 2020 2020 2020 2020 2020 6167 656e 7431            agent1
+000172c0: 2c20 6974 656d 2c20 2242 616c 616e 6365  , item, "Balance
+000172d0: 456e 7472 792e 4551 5549 5459 222c 2073  Entry.EQUITY", s
+000172e0: 6967 6e20 2b20 7175 616e 7469 7479 2c20  ign + quantity, 
+000172f0: 7369 6c65 6e74 2929 0d0a 2020 2020 2020  silent))..      
+00017300: 2020 2020 2020 666f 7220 656e 7472 7920        for entry 
+00017310: 696e 2061 312e 7370 6c69 7428 225c 6e22  in a1.split("\n"
+00017320: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00017330: 2020 2020 6966 2065 6e74 7279 2021 3d20      if entry != 
+00017340: 2222 2061 6e64 2065 6e74 7279 2021 3d20  "" and entry != 
+00017350: 225c 6e22 3a0d 0a20 2020 2020 2020 2020  "\n":..         
+00017360: 2020 2020 2020 2020 2020 2073 6967 6e2c             sign,
+00017370: 2069 7465 6d2c 2073 696c 656e 7420 3d20   item, silent = 
+00017380: 7365 6c66 2e65 6e74 7279 5f74 6f5f 7661  self.entry_to_va
+00017390: 6c73 2865 6e74 7279 2c20 6167 656e 7431  ls(entry, agent1
+000173a0: 2c20 2241 7373 6574 7322 290d 0a20 2020  , "Assets")..   
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 2069 6620 7369 676e 2069 7320 6e6f 7420   if sign is not 
+000173d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000173e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000173f0: 6f6d 6d61 6e64 732e 6170 7065 6e64 2822  ommands.append("
+00017400: 2573 2e62 616c 616e 6365 5f73 6865 6574  %s.balance_sheet
+00017410: 2e63 6861 6e67 655f 6974 656d 2827 2573  .change_item('%s
+00017420: 272c 2025 732c 2025 732c 2073 7570 7072  ', %s, %s, suppr
+00017430: 6573 735f 7374 6f63 6b3d 2573 2922 2025  ess_stock=%s)" %
+00017440: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00017450: 2020 2020 2020 2020 2020 2020 6167 656e              agen
+00017460: 7431 2c20 6974 656d 2c20 2242 616c 616e  t1, item, "Balan
+00017470: 6365 456e 7472 792e 4153 5345 5453 222c  ceEntry.ASSETS",
+00017480: 2073 6967 6e20 2b20 7175 616e 7469 7479   sign + quantity
+00017490: 2c20 7369 6c65 6e74 2929 0d0a 2020 2020  , silent))..    
+000174a0: 2020 2020 2020 2020 666f 7220 656e 7472          for entr
+000174b0: 7920 696e 206c 312e 7370 6c69 7428 225c  y in l1.split("\
+000174c0: 6e22 293a 0d0a 2020 2020 2020 2020 2020  n"):..          
+000174d0: 2020 2020 2020 6966 2065 6e74 7279 2021        if entry !
+000174e0: 3d20 2222 2061 6e64 2065 6e74 7279 2021  = "" and entry !
+000174f0: 3d20 225c 6e22 3a0d 0a20 2020 2020 2020  = "\n":..       
+00017500: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+00017510: 6e2c 2069 7465 6d2c 2073 696c 656e 7420  n, item, silent 
+00017520: 3d20 7365 6c66 2e65 6e74 7279 5f74 6f5f  = self.entry_to_
+00017530: 7661 6c73 2865 6e74 7279 2c20 6167 656e  vals(entry, agen
+00017540: 7431 2c20 224c 6961 6269 6c69 7469 6573  t1, "Liabilities
+00017550: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00017560: 2020 2020 2020 2020 6966 2073 6967 6e20          if sign 
+00017570: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 2020 2020 2020 636f 6d6d 616e 6473 2e61        commands.a
+000175a0: 7070 656e 6428 2225 732e 6261 6c61 6e63  ppend("%s.balanc
+000175b0: 655f 7368 6565 742e 6368 616e 6765 5f69  e_sheet.change_i
+000175c0: 7465 6d28 2725 7327 2c20 2573 2c20 2573  tem('%s', %s, %s
+000175d0: 2c20 7375 7070 7265 7373 5f73 746f 636b  , suppress_stock
+000175e0: 3d25 7329 2220 2520 280d 0a20 2020 2020  =%s)" % (..     
+000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017600: 2020 2061 6765 6e74 312c 2069 7465 6d2c     agent1, item,
+00017610: 2022 4261 6c61 6e63 6545 6e74 7279 2e4c   "BalanceEntry.L
+00017620: 4941 4249 4c49 5449 4553 222c 2073 6967  IABILITIES", sig
+00017630: 6e20 2b20 7175 616e 7469 7479 2c20 7369  n + quantity, si
+00017640: 6c65 6e74 2929 0d0a 2020 2020 2020 2020  lent))..        
+00017650: 2020 2020 666f 7220 656e 7472 7920 696e      for entry in
+00017660: 2065 322e 7370 6c69 7428 225c 6e22 293a   e2.split("\n"):
+00017670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017680: 2020 6966 2065 6e74 7279 2021 3d20 2222    if entry != ""
+00017690: 2061 6e64 2065 6e74 7279 2021 3d20 225c   and entry != "\
+000176a0: 6e22 3a0d 0a20 2020 2020 2020 2020 2020  n":..           
+000176b0: 2020 2020 2020 2020 2073 6967 6e2c 2069           sign, i
+000176c0: 7465 6d2c 2073 696c 656e 7420 3d20 7365  tem, silent = se
+000176d0: 6c66 2e65 6e74 7279 5f74 6f5f 7661 6c73  lf.entry_to_vals
+000176e0: 2865 6e74 7279 2c20 6167 656e 7432 2c20  (entry, agent2, 
+000176f0: 2245 7175 6974 7922 290d 0a20 2020 2020  "Equity")..     
+00017700: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017710: 6620 7369 676e 2069 7320 6e6f 7420 4e6f  f sign is not No
+00017720: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00017730: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00017740: 6d61 6e64 732e 6170 7065 6e64 2822 2573  mands.append("%s
+00017750: 2e62 616c 616e 6365 5f73 6865 6574 2e63  .balance_sheet.c
+00017760: 6861 6e67 655f 6974 656d 2827 2573 272c  hange_item('%s',
+00017770: 2025 732c 2025 732c 2073 7570 7072 6573   %s, %s, suppres
+00017780: 735f 7374 6f63 6b3d 2573 2922 2025 2028  s_stock=%s)" % (
+00017790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000177a0: 2020 2020 2020 2020 2020 6167 656e 7432            agent2
+000177b0: 2c20 6974 656d 2c20 2242 616c 616e 6365  , item, "Balance
+000177c0: 456e 7472 792e 4551 5549 5459 222c 2073  Entry.EQUITY", s
+000177d0: 6967 6e20 2b20 7175 616e 7469 7479 2c20  ign + quantity, 
+000177e0: 7369 6c65 6e74 2929 0d0a 2020 2020 2020  silent))..      
+000177f0: 2020 2020 2020 666f 7220 656e 7472 7920        for entry 
+00017800: 696e 2061 322e 7370 6c69 7428 225c 6e22  in a2.split("\n"
+00017810: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00017820: 2020 2020 6966 2065 6e74 7279 2021 3d20      if entry != 
+00017830: 2222 2061 6e64 2065 6e74 7279 2021 3d20  "" and entry != 
+00017840: 225c 6e22 3a0d 0a20 2020 2020 2020 2020  "\n":..         
+00017850: 2020 2020 2020 2020 2020 2073 6967 6e2c             sign,
+00017860: 2069 7465 6d2c 2073 696c 656e 7420 3d20   item, silent = 
+00017870: 7365 6c66 2e65 6e74 7279 5f74 6f5f 7661  self.entry_to_va
+00017880: 6c73 2865 6e74 7279 2c20 6167 656e 7432  ls(entry, agent2
+00017890: 2c20 2241 7373 6574 7322 290d 0a20 2020  , "Assets")..   
+000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178b0: 2069 6620 7369 676e 2069 7320 6e6f 7420   if sign is not 
+000178c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000178e0: 6f6d 6d61 6e64 732e 6170 7065 6e64 2822  ommands.append("
+000178f0: 2573 2e62 616c 616e 6365 5f73 6865 6574  %s.balance_sheet
+00017900: 2e63 6861 6e67 655f 6974 656d 2827 2573  .change_item('%s
+00017910: 272c 2025 732c 2025 732c 2073 7570 7072  ', %s, %s, suppr
+00017920: 6573 735f 7374 6f63 6b3d 2573 2922 2025  ess_stock=%s)" %
+00017930: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00017940: 2020 2020 2020 2020 2020 2020 6167 656e              agen
+00017950: 7432 2c20 6974 656d 2c20 2242 616c 616e  t2, item, "Balan
+00017960: 6365 456e 7472 792e 4153 5345 5453 222c  ceEntry.ASSETS",
+00017970: 2073 6967 6e20 2b20 7175 616e 7469 7479   sign + quantity
+00017980: 2c20 7369 6c65 6e74 2929 0d0a 2020 2020  , silent))..    
+00017990: 2020 2020 2020 2020 666f 7220 656e 7472          for entr
+000179a0: 7920 696e 206c 322e 7370 6c69 7428 225c  y in l2.split("\
+000179b0: 6e22 293a 0d0a 2020 2020 2020 2020 2020  n"):..          
+000179c0: 2020 2020 2020 6966 2065 6e74 7279 2021        if entry !
+000179d0: 3d20 2222 2061 6e64 2065 6e74 7279 2021  = "" and entry !
+000179e0: 3d20 225c 6e22 3a0d 0a20 2020 2020 2020  = "\n":..       
+000179f0: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+00017a00: 6e2c 2069 7465 6d2c 2073 696c 656e 7420  n, item, silent 
+00017a10: 3d20 7365 6c66 2e65 6e74 7279 5f74 6f5f  = self.entry_to_
+00017a20: 7661 6c73 2865 6e74 7279 2c20 6167 656e  vals(entry, agen
+00017a30: 7432 2c20 224c 6961 6269 6c69 7469 6573  t2, "Liabilities
+00017a40: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00017a50: 2020 2020 2020 2020 6966 2073 6967 6e20          if sign 
+00017a60: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a80: 2020 2020 2020 636f 6d6d 616e 6473 2e61        commands.a
+00017a90: 7070 656e 6428 2225 732e 6261 6c61 6e63  ppend("%s.balanc
+00017aa0: 655f 7368 6565 742e 6368 616e 6765 5f69  e_sheet.change_i
+00017ab0: 7465 6d28 2725 7327 2c20 2573 2c20 2573  tem('%s', %s, %s
+00017ac0: 2c20 7375 7070 7265 7373 5f73 746f 636b  , suppress_stock
+00017ad0: 3d25 7329 2220 2520 280d 0a20 2020 2020  =%s)" % (..     
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017af0: 2020 2061 6765 6e74 322c 2069 7465 6d2c     agent2, item,
+00017b00: 2022 4261 6c61 6e63 6545 6e74 7279 2e4c   "BalanceEntry.L
+00017b10: 4941 4249 4c49 5449 4553 222c 2073 6967  IABILITIES", sig
+00017b20: 6e20 2b20 7175 616e 7469 7479 2c20 7369  n + quantity, si
+00017b30: 6c65 6e74 2929 0d0a 0d0a 2020 2020 2020  lent))....      
+00017b40: 2020 2020 2020 636f 6d6d 616e 6473 2e61        commands.a
+00017b50: 7070 656e 6428 2225 732e 6261 6c61 6e63  ppend("%s.balanc
+00017b60: 655f 7368 6565 742e 656e 6761 6765 2829  e_sheet.engage()
+00017b70: 2220 2520 6167 656e 7431 290d 0a20 2020  " % agent1)..   
+00017b80: 2020 2020 2020 2020 2069 6620 5472 7565           if True
+00017b90: 3a20 2320 6167 656e 7431 213d 6167 656e  : # agent1!=agen
+00017ba0: 7432 3a0d 0a20 2020 2020 2020 2020 2020  t2:..           
+00017bb0: 2020 2020 2063 6f6d 6d61 6e64 732e 6170       commands.ap
+00017bc0: 7065 6e64 2822 2573 2e62 616c 616e 6365  pend("%s.balance
+00017bd0: 5f73 6865 6574 2e65 6e67 6167 6528 2922  _sheet.engage()"
+00017be0: 2025 2061 6765 6e74 3229 0d0a 0d0a 2020   % agent2)....  
+00017bf0: 2020 2020 2020 2020 2020 6164 645f 666c            add_fl
+00017c00: 6f77 203d 2066 6c6f 775f 6368 6563 6b0d  ow = flow_check.
+00017c10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017c20: 6164 645f 666c 6f77 3a0d 0a20 2020 2020  add_flow:..     
+00017c30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00017c40: 2873 7562 6a65 6374 5f73 7472 2c22 666c  (subject_str,"fl
+00017c50: 6f77 2063 6865 636b 222c 666c 6f77 5f63  ow check",flow_c
+00017c60: 6865 636b 290d 0a0d 0a20 2020 2020 2020  heck)....       
+00017c70: 2020 2020 2020 2020 206b 696e 645f 656e           kind_en
+00017c80: 756d 203d 2022 2825 732c 2573 2922 2025  um = "(%s,%s)" %
+00017c90: 2028 6b69 6e64 2e73 706c 6974 2822 2d3e   (kind.split("->
+00017ca0: 2229 5b30 5d2e 7374 7269 7028 292c 6b69  ")[0].strip(),ki
+00017cb0: 6e64 2e73 706c 6974 2822 2d3e 2229 5b31  nd.split("->")[1
+00017cc0: 5d2e 7374 7269 7028 2929 0d0a 0d0a 2020  ].strip())....  
+00017cd0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00017ce0: 6d6d 616e 6473 2e61 7070 656e 6428 2246  mmands.append("F
+00017cf0: 6c6f 774d 6174 7269 7828 292e 6c6f 675f  lowMatrix().log_
+00017d00: 666c 6f77 2825 732c 2025 732c 2025 732c  flow(%s, %s, %s,
+00017d10: 2025 732c 2073 7562 6a65 6374 3d27 2573   %s, subject='%s
+00017d20: 2729 2220 2520 286b 696e 645f 656e 756d  ')" % (kind_enum
+00017d30: 2c20 7175 616e 7469 7479 2c20 6167 656e  , quantity, agen
+00017d40: 7431 2c20 6167 656e 7432 2c20 7375 626a  t1, agent2, subj
+00017d50: 6563 745f 7374 7229 290d 0a0d 0a20 2020  ect_str))....   
+00017d60: 2020 2020 2020 2020 2023 2061 7070 656e           # appen
+00017d70: 6420 696e 7365 7274 5f6c 696e 6b20 636f  d insert_link co
+00017d80: 6d6d 616e 6420 746f 2063 6f64 650d 0a0d  mmand to code...
+00017d90: 0a0d 0a20 2020 2020 2020 2020 2020 206d  ...            m
+00017da0: 795f 696e 636f 6d65 5f64 6963 7420 3d20  y_income_dict = 
+00017db0: 7b20 2320 2374 7261 6e73 6c61 7465 7320  { # #translates 
+00017dc0: 7374 7269 6e67 2069 6e74 6f20 4943 5345  string into ICSE
+00017dd0: 6e74 7279 2028 666f 7220 6265 7474 6572  ntry (for better
+00017de0: 2065 6666 6963 6965 6e63 7929 0d0a 2020   efficiency)..  
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2252                "R
+00017e00: 6576 656e 7565 223a 2022 4943 5345 6e74  evenue": "ICSEnt
+00017e10: 7279 2e52 4556 454e 5545 5322 2c0d 0a20  ry.REVENUES",.. 
+00017e20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017e30: 4e6f 6e2d 4f70 2e20 496e 636f 6d65 223a  Non-Op. Income":
+00017e40: 2022 4943 5345 6e74 7279 2e4e 4f49 222c   "ICSEntry.NOI",
+00017e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017e60: 2020 2245 7870 656e 7365 223a 2022 4943    "Expense": "IC
+00017e70: 5345 6e74 7279 2e45 5850 454e 5345 5322  SEntry.EXPENSES"
+00017e80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00017e90: 2020 2022 5461 7822 3a20 2249 4353 456e     "Tax": "ICSEn
+00017ea0: 7472 792e 5441 5845 5322 2c0d 0a20 2020  try.TAXES",..   
+00017eb0: 2020 2020 2020 2020 2020 2020 2022 496e               "In
+00017ec0: 7465 7265 7374 223a 2022 4943 5345 6e74  terest": "ICSEnt
+00017ed0: 7279 2e49 4e54 4552 4553 5422 2c0d 0a20  ry.INTEREST",.. 
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017ef0: 4761 696e 223a 2022 4943 5345 6e74 7279  Gain": "ICSEntry
+00017f00: 2e47 4149 4e53 222c 0d0a 2020 2020 2020  .GAINS",..      
+00017f10: 2020 2020 2020 2020 2020 224e 6f6e 7461            "Nonta
+00017f20: 782e 5072 6f66 6974 223a 2022 4943 5345  x.Profit": "ICSE
+00017f30: 6e74 7279 2e4e 4f4e 5441 585f 5052 4f46  ntry.NONTAX_PROF
+00017f40: 4954 5322 2c0d 0a20 2020 2020 2020 2020  ITS",..         
+00017f50: 2020 2020 2020 2022 4e6f 6e74 6178 2e20         "Nontax. 
+00017f60: 5072 6f66 6974 223a 2022 4943 5345 6e74  Profit": "ICSEnt
+00017f70: 7279 2e4e 4f4e 5441 585f 5052 4f46 4954  ry.NONTAX_PROFIT
+00017f80: 5322 2c20 2320 7175 6963 6b20 616e 6420  S", # quick and 
+00017f90: 6469 7274 7920 6275 6766 6978 0d0a 2020  dirty bugfix..  
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 224e                "N
+00017fb0: 6f6e 7461 782e 204c 6f73 7322 3a20 2022  ontax. Loss":  "
+00017fc0: 4943 5345 6e74 7279 2e4e 4f4e 5441 585f  ICSEntry.NONTAX_
+00017fd0: 4c4f 5353 4553 222c 0d0a 2020 2020 2020  LOSSES",..      
+00017fe0: 2020 2020 2020 2020 2020 224c 6f73 7322            "Loss"
+00017ff0: 3a20 2022 4943 5345 6e74 7279 2e4c 4f53  :  "ICSEntry.LOS
+00018000: 5345 5322 0d0a 2020 2020 2020 2020 2020  SES"..          
+00018010: 2020 7d0d 0a0d 0a20 2020 2020 2020 2020    }....         
+00018020: 2020 2023 2069 6e63 6f6d 6520 7374 6174     # income stat
+00018030: 656d 656e 743f 0d0a 2020 2020 2020 2020  ement?..        
+00018040: 2020 2020 6966 2022 696e 636f 6d65 3122      if "income1"
+00018050: 2069 6e20 6669 6c65 6461 7461 3a0d 0a20   in filedata:.. 
+00018060: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018070: 6620 7374 7228 6669 6c65 6461 7461 5b22  f str(filedata["
+00018080: 696e 636f 6d65 3122 5d29 2021 3d20 274e  income1"]) != 'N
+00018090: 6f6e 6527 3a0d 0a20 2020 2020 2020 2020  one':..         
+000180a0: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
+000180b0: 6e64 732e 6170 7065 6e64 2822 2573 2e69  nds.append("%s.i
+000180c0: 6e63 6f6d 655f 7374 6174 656d 656e 742e  ncome_statement.
+000180d0: 6e65 775f 656e 7472 7928 2573 2c27 2573  new_entry(%s,'%s
+000180e0: 272c 2573 2922 2025 2028 6167 656e 7431  ',%s)" % (agent1
+000180f0: 2c6d 795f 696e 636f 6d65 5f64 6963 745b  ,my_income_dict[
+00018100: 6669 6c65 6461 7461 5b22 696e 636f 6d65  filedata["income
+00018110: 3122 5d5d 2c73 7562 6a65 6374 2c71 7561  1"]],subject,qua
+00018120: 6e74 6974 7929 290d 0a0d 0a20 2020 2020  ntity))....     
+00018130: 2020 2020 2020 2069 6620 2269 6e63 6f6d         if "incom
+00018140: 6532 2220 696e 2066 696c 6564 6174 613a  e2" in filedata:
+00018150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018160: 2020 6966 2073 7472 2866 696c 6564 6174    if str(filedat
+00018170: 615b 2269 6e63 6f6d 6532 225d 2920 213d  a["income2"]) !=
+00018180: 2027 4e6f 6e65 273a 0d0a 2020 2020 2020   'None':..      
+00018190: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000181a0: 6d6d 616e 6473 2e61 7070 656e 6428 2225  mmands.append("%
+000181b0: 732e 696e 636f 6d65 5f73 7461 7465 6d65  s.income_stateme
+000181c0: 6e74 2e6e 6577 5f65 6e74 7279 2825 732c  nt.new_entry(%s,
+000181d0: 2725 7327 2c25 7329 2220 2520 2861 6765  '%s',%s)" % (age
+000181e0: 6e74 322c 206d 795f 696e 636f 6d65 5f64  nt2, my_income_d
+000181f0: 6963 745b 6669 6c65 6461 7461 5b22 696e  ict[filedata["in
+00018200: 636f 6d65 3222 5d5d 2c20 7375 626a 6563  come2"]], subjec
+00018210: 742c 2071 7561 6e74 6974 7929 290d 0a0d  t, quantity))...
+00018220: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00018230: 6173 6820 666c 6f77 2073 7461 7465 6d65  ash flow stateme
+00018240: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00018250: 6966 2022 6361 7368 666c 6f77 3122 2069  if "cashflow1" i
+00018260: 6e20 6669 6c65 6461 7461 3a0d 0a20 2020  n filedata:..   
+00018270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018280: 7374 7228 6669 6c65 6461 7461 5b22 6361  str(filedata["ca
+00018290: 7368 666c 6f77 3122 5d29 2021 3d20 274e  shflow1"]) != 'N
+000182a0: 6f6e 6527 3a0d 0a20 2020 2020 2020 2020  one':..         
+000182b0: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
+000182c0: 6e64 732e 6170 7065 6e64 2822 2573 2e63  nds.append("%s.c
+000182d0: 6173 685f 666c 6f77 5f73 7461 7465 6d65  ash_flow_stateme
+000182e0: 6e74 2e6e 6577 5f65 6e74 7279 2825 732c  nt.new_entry(%s,
+000182f0: 2725 7327 2c2d 2573 2922 2025 2028 6167  '%s',-%s)" % (ag
+00018300: 656e 7431 2c22 4361 7368 466c 6f77 456e  ent1,"CashFlowEn
+00018310: 7472 792e 2220 2b20 6669 6c65 6461 7461  try." + filedata
+00018320: 5b22 6361 7368 666c 6f77 3122 5d2e 7570  ["cashflow1"].up
+00018330: 7065 7228 292c 7375 626a 6563 742c 7175  per(),subject,qu
+00018340: 616e 7469 7479 2929 0d0a 0d0a 2020 2020  antity))....    
+00018350: 2020 2020 2020 2020 6966 2022 6361 7368          if "cash
+00018360: 666c 6f77 3222 2069 6e20 6669 6c65 6461  flow2" in fileda
+00018370: 7461 3a0d 0a20 2020 2020 2020 2020 2020  ta:..           
+00018380: 2020 2020 2069 6620 7374 7228 6669 6c65       if str(file
+00018390: 6461 7461 5b22 6361 7368 666c 6f77 3222  data["cashflow2"
+000183a0: 5d29 2021 3d20 274e 6f6e 6527 3a0d 0a20  ]) != 'None':.. 
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183c0: 2020 2063 6f6d 6d61 6e64 732e 6170 7065     commands.appe
+000183d0: 6e64 2822 2573 2e63 6173 685f 666c 6f77  nd("%s.cash_flow
+000183e0: 5f73 7461 7465 6d65 6e74 2e6e 6577 5f65  _statement.new_e
+000183f0: 6e74 7279 2825 732c 2725 7327 2c25 7329  ntry(%s,'%s',%s)
+00018400: 2220 2520 2861 6765 6e74 322c 2243 6173  " % (agent2,"Cas
+00018410: 6846 6c6f 7745 6e74 7279 2e22 202b 2066  hFlowEntry." + f
+00018420: 696c 6564 6174 615b 2263 6173 6866 6c6f  iledata["cashflo
+00018430: 7732 225d 2e75 7070 6572 2829 2c73 7562  w2"].upper(),sub
+00018440: 6a65 6374 2c71 7561 6e74 6974 7929 290d  ject,quantity)).
+00018450: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00018460: 6620 5472 7565 3a20 2320 6167 656e 7431  f True: # agent1
+00018470: 2021 3d20 6167 656e 7432 3a0d 0a20 2020   != agent2:..   
+00018480: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00018490: 686f 6420 3d20 2264 6566 2025 7328 2573  hod = "def %s(%s
+000184a0: 2c20 2573 2c20 2573 293a 5c6e 2220 2520  , %s, %s):\n" % 
+000184b0: 2873 7562 6a65 6374 2c61 6765 6e74 312c  (subject,agent1,
+000184c0: 6167 656e 7432 2c71 7561 6e74 6974 7929  agent2,quantity)
+000184d0: 0d0a 2020 2020 2020 2020 2020 2020 2365  ..            #e
+000184e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000184f0: 2020 2320 2020 206d 6574 686f 6420 3d20    #    method = 
+00018500: 2264 6566 2025 7328 2573 2c20 2573 293a  "def %s(%s, %s):
+00018510: 5c6e 2220 2520 2873 7562 6a65 6374 2c20  \n" % (subject, 
+00018520: 6167 656e 7431 2c20 7175 616e 7469 7479  agent1, quantity
+00018530: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00018540: 2069 6620 2264 6573 6372 6970 7469 6f6e   if "description
+00018550: 2220 696e 2066 696c 6564 6174 613a 2023  " in filedata: #
+00018560: 2061 6464 2074 6865 2064 6573 6372 6970   add the descrip
+00018570: 7469 6f6e 2069 6e20 7468 6520 646f 6373  tion in the docs
+00018580: 7472 696e 6720 6f66 2074 6865 2066 756e  tring of the fun
+00018590: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
+000185a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000185b0: 2020 6d65 7468 6f64 202b 3d20 2220 2020    method += "   
+000185c0: 2023 2220 2b20 6669 6c65 6461 7461 5b22   #" + filedata["
+000185d0: 6465 7363 7269 7074 696f 6e22 5d20 2b20  description"] + 
+000185e0: 225c 6e22 0d0a 0d0a 2020 2020 2020 2020  "\n"....        
+000185f0: 2020 2020 666f 7220 636f 6d6d 616e 6420      for command 
+00018600: 696e 2063 6f6d 6d61 6e64 733a 0d0a 2020  in commands:..  
+00018610: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00018620: 7468 6f64 202b 3d20 2220 2020 2022 202b  thod += "    " +
+00018630: 2063 6f6d 6d61 6e64 202b 2022 5c6e 220d   command + "\n".
+00018640: 0a0d 0a20 2020 2020 2020 2020 2020 206d  ...            m
+00018650: 6574 686f 6420 2b3d 2022 5c6e 5c6e 220d  ethod += "\n\n".
+00018660: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
+00018670: 6520 2b3d 206d 6574 686f 640d 0a0d 0a20  e += method.... 
+00018680: 2020 2020 2020 2066 6f6c 6465 7220 3d20         folder = 
+00018690: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+000186a0: 7365 6c66 2e63 7572 7265 6e74 5f66 696c  self.current_fil
+000186b0: 6529 2023 2073 7461 7475 7342 6172 2829  e) # statusBar()
+000186c0: 2e63 7572 7265 6e74 4d65 7373 6167 6528  .currentMessage(
+000186d0: 2929 0d0a 2020 2020 2020 2020 666e 616d  ))..        fnam
+000186e0: 6520 3d20 2066 6f6c 6465 7220 2b20 222f  e =  folder + "/
+000186f0: 7079 7468 6f6e 5f63 6f64 652f 7472 616e  python_code/tran
+00018700: 7361 6374 696f 6e73 2e70 7922 0d0a 0d0a  sactions.py"....
+00018710: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00018720: 6e28 666e 616d 652c 2277 222c 656e 636f  n(fname,"w",enco
+00018730: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+00018740: 2066 696c 653a 0d0a 2020 2020 2020 2020   file:..        
+00018750: 2020 2020 6669 6c65 2e77 7269 7465 2863      file.write(c
+00018760: 6f64 6529 0d0a 0d0a 2020 2020 2020 2020  ode)....        
+00018770: 6966 2073 686f 775f 6e6f 7469 6669 6361  if show_notifica
+00018780: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
+00018790: 2020 2073 656c 662e 6e6f 7469 6679 286d     self.notify(m
+000187a0: 6573 7361 6765 3d22 436f 6465 2065 7870  essage="Code exp
+000187b0: 6f72 7465 6420 746f 2025 7322 2025 2028  orted to %s" % (
+000187c0: 666e 616d 6529 2c74 6974 6c65 3d22 5375  fname),title="Su
+000187d0: 6363 6573 7322 290d 0a0d 0a0d 0a20 2020  ccess")......   
+000187e0: 2064 6566 2067 656e 5f69 6373 5f73 696e   def gen_ics_sin
+000187f0: 676c 6528 7365 6c66 293a 0d0a 2020 2020  gle(self):..    
+00018800: 2020 2020 6966 2073 656c 662e 6472 6177      if self.draw
+00018810: 6361 6e76 6173 2e68 6967 686c 6967 6874  canvas.highlight
+00018820: 6564 2069 7320 4e6f 6e65 3a0d 0a20 2020  ed is None:..   
+00018830: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018840: 7469 6679 2874 6974 6c65 3d22 4e6f 2061  tify(title="No a
+00018850: 6765 6e74 2073 656c 6563 7465 6422 2c20  gent selected", 
+00018860: 6d65 7373 6167 653d 224e 6f20 6167 656e  message="No agen
+00018870: 7420 7365 6c65 6374 6564 2e20 506c 6561  t selected. Plea
+00018880: 7365 2073 656c 6563 7420 6f6e 6520 6669  se select one fi
+00018890: 7273 742e 2229 0d0a 2020 2020 2020 2020  rst.")..        
+000188a0: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+000188b0: 2020 2020 6966 2073 656c 662e 6472 6177      if self.draw
+000188c0: 6361 6e76 6173 2e68 6967 686c 6967 6874  canvas.highlight
+000188d0: 6564 2e69 7368 656c 7065 723a 0d0a 2020  ed.ishelper:..  
+000188e0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000188f0: 6f74 6966 7928 7469 746c 653d 224e 6f20  otify(title="No 
+00018900: 6167 656e 7420 7365 6c65 6374 6564 222c  agent selected",
+00018910: 206d 6573 7361 6765 3d22 4e6f 2076 616c   message="No val
+00018920: 6964 2062 6f78 2073 656c 6563 7465 642e  id box selected.
+00018930: 2050 6c65 6173 6520 7365 6c65 6374 2061   Please select a
+00018940: 6e20 6167 656e 742e 2229 0d0a 2020 2020  n agent.")..    
+00018950: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00018960: 2020 2020 2020 2020 6d79 5f61 6765 6e74          my_agent
+00018970: 203d 2073 656c 662e 6472 6177 6361 6e76   = self.drawcanv
+00018980: 6173 2e68 6967 686c 6967 6874 6564 2e6e  as.highlighted.n
+00018990: 616d 650d 0a0d 0a20 2020 2020 2020 2063  ame....        c
+000189a0: 6f6d 6269 6e65 645f 696e 636f 6d65 203d  ombined_income =
+000189b0: 2020 7b22 5375 626a 6563 7422 3a5b 5d2c    {"Subject":[],
+000189c0: 2253 686f 7274 204e 616d 6522 3a20 5b5d  "Short Name": []
+000189d0: 2c22 5175 616e 7469 7479 223a 5b5d 2c20  ,"Quantity":[], 
+000189e0: 2254 7970 6522 3a5b 5d2c 2022 5261 6e6b  "Type":[], "Rank
+000189f0: 696e 6722 3a5b 5d7d 2023 2072 616e 6b69  ing":[]} # ranki
+00018a00: 6e67 2077 696c 6c20 6265 2072 656d 6f76  ng will be remov
+00018a10: 6564 206c 6174 6572 0d0a 2020 2020 2020  ed later..      
+00018a20: 2020 2222 220d 0a20 2020 2020 2020 2022    """..        "
+00018a30: 4761 696e 7322 3a20 5b5d 2c20 224c 6f73  Gains": [], "Los
+00018a40: 7365 7322 3a20 5b5d 2c20 2252 6576 656e  ses": [], "Reven
+00018a50: 7565 7322 3a20 5b5d 2c20 2254 6178 6573  ues": [], "Taxes
+00018a60: 223a 205b 5d2c 2022 4578 7065 6e73 6573  ": [], "Expenses
+00018a70: 223a 205b 5d2c 0d0a 2020 2020 2020 2020  ": [],..        
+00018a80: 2022 4e6f 6e74 6178 6162 6c65 204c 6f73   "Nontaxable Los
+00018a90: 7365 7322 3a20 5b5d 2c20 224e 6f6e 7461  ses": [], "Nonta
+00018aa0: 7861 626c 6520 5072 6f66 6974 7322 3a20  xable Profits": 
+00018ab0: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
+00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ad0: 2020 2020 224e 6f6e 2d4f 7065 7261 7469      "Non-Operati
+00018ae0: 6f6e 616c 2049 6e63 6f6d 6522 3a20 5b5d  onal Income": []
+00018af0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 00018b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b10: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00018b20: 2222 220d 0a20 2020 2020 2020 206b 203d  """..        k =
-00018b30: 2030 0d0a 2020 2020 2020 2020 7472 793a   0..        try:
-00018b40: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00018b50: 7220 6669 6c65 6461 7461 2069 6e20 7365  r filedata in se
-00018b60: 6c66 2e65 6e74 7279 5f64 6174 613a 0d0a  lf.entry_data:..
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b80: 6167 656e 7431 203d 2066 696c 6564 6174  agent1 = filedat
-00018b90: 615b 2261 6765 6e74 3122 5d2e 7374 7269  a["agent1"].stri
-00018ba0: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
-00018bb0: 2020 2020 2061 6765 6e74 3220 3d20 6669       agent2 = fi
-00018bc0: 6c65 6461 7461 5b22 6167 656e 7432 225d  ledata["agent2"]
-00018bd0: 2e73 7472 6970 2829 0d0a 0d0a 2020 2020  .strip()....    
-00018be0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00018bf0: 7428 2261 6765 6e74 3122 2c61 6765 6e74  t("agent1",agent
-00018c00: 312c 2261 6765 6e74 3222 2c61 6765 6e74  1,"agent2",agent
-00018c10: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00018c20: 2020 2020 6966 2061 6765 6e74 3120 3d3d      if agent1 ==
-00018c30: 206d 795f 6167 656e 743a 0d0a 2020 2020   my_agent:..    
-00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c50: 7265 665f 6167 656e 7420 3d20 2261 6765  ref_agent = "age
-00018c60: 6e74 3122 0d0a 2020 2020 2020 2020 2020  nt1"..          
-00018c70: 2020 2020 2020 2020 2020 7265 665f 696e            ref_in
-00018c80: 636f 6d65 203d 2022 696e 636f 6d65 3122  come = "income1"
-00018c90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018ca0: 2020 2020 656c 6966 2061 6765 6e74 3220      elif agent2 
-00018cb0: 3d3d 206d 795f 6167 656e 743a 0d0a 2020  == my_agent:..  
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cd0: 2020 7265 665f 6167 656e 7420 3d20 2261    ref_agent = "a
-00018ce0: 6765 6e74 3222 0d0a 2020 2020 2020 2020  gent2"..        
-00018cf0: 2020 2020 2020 2020 2020 2020 7265 665f              ref_
-00018d00: 696e 636f 6d65 203d 2022 696e 636f 6d65  income = "income
-00018d10: 3222 0d0a 2020 2020 2020 2020 2020 2020  2"..            
-00018d20: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00018d40: 6173 730d 0a0d 0a20 2020 2020 2020 2020  ass....         
-00018d50: 2020 2020 2020 2023 6173 7365 7473 3120         #assets1 
-00018d60: 3d20 6669 6c65 6461 7461 5b22 6131 225d  = filedata["a1"]
-00018d70: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
-00018d80: 2020 2020 2020 2020 2023 6c69 6162 7331           #liabs1
-00018d90: 203d 2066 696c 6564 6174 615b 226c 3122   = filedata["l1"
-00018da0: 5d20 2b20 225c 6e22 202b 2066 696c 6564  ] + "\n" + filed
-00018db0: 6174 615b 2265 3122 5d20 2b20 225c 6e22  ata["e1"] + "\n"
-00018dc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018dd0: 2020 2020 2361 7373 6574 7332 203d 2066      #assets2 = f
-00018de0: 696c 6564 6174 615b 2261 3222 5d20 2b20  iledata["a2"] + 
-00018df0: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
-00018e00: 2020 2020 2020 236c 6961 6273 3220 3d20        #liabs2 = 
-00018e10: 6669 6c65 6461 7461 5b22 6c32 225d 202b  filedata["l2"] +
-00018e20: 2022 5c6e 2220 2b20 6669 6c65 6461 7461   "\n" + filedata
-00018e30: 5b22 6532 225d 202b 2022 5c6e 220d 0a0d  ["e2"] + "\n"...
-00018e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e50: 2069 6620 2861 6765 6e74 3120 3d3d 206d   if (agent1 == m
-00018e60: 795f 6167 656e 7420 6f72 2061 6765 6e74  y_agent or agent
-00018e70: 3220 3d3d 206d 795f 6167 656e 7429 2061  2 == my_agent) a
-00018e80: 6e64 2073 7472 2866 696c 6564 6174 615b  nd str(filedata[
-00018e90: 7265 665f 696e 636f 6d65 5d29 2021 3d20  ref_income]) != 
-00018ea0: 274e 6f6e 6527 3a0d 0a20 2020 2020 2020  'None':..       
-00018eb0: 2020 2020 2020 2020 2020 2020 206d 7964               myd
-00018ec0: 6963 7420 3d20 7b22 4761 696e 223a 2022  ict = {"Gain": "
-00018ed0: 4761 696e 7322 2c0d 0a20 2020 2020 2020  Gains",..       
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 2020 2020 2020 2022 4c6f 7373 223a 2022         "Loss": "
-00018f00: 4c6f 7373 6573 222c 0d0a 2020 2020 2020  Losses",..      
-00018f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f20: 2020 2020 2020 2020 2245 7870 656e 7365          "Expense
-00018f30: 223a 2022 4578 7065 6e73 6573 222c 0d0a  ": "Expenses",..
-00018f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f50: 2020 2020 2020 2020 2020 2020 2020 2252                "R
-00018f60: 6576 656e 7565 223a 2022 5265 7665 6e75  evenue": "Revenu
-00018f70: 6573 222c 0d0a 2020 2020 2020 2020 2020  es",..          
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f90: 2020 2020 2254 6178 223a 2022 5461 7865      "Tax": "Taxe
-00018fa0: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fc0: 2020 2022 4e6f 6e74 6178 2e20 5072 6f66     "Nontax. Prof
-00018fd0: 6974 223a 2022 4e6f 6e74 6178 6162 6c65  it": "Nontaxable
-00018fe0: 2050 726f 6669 7473 222c 0d0a 2020 2020   Profits",..    
-00018ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019000: 2020 2020 2020 2020 2020 224e 6f6e 7461            "Nonta
-00019010: 782e 204c 6f73 7322 3a20 224e 6f6e 7461  x. Loss": "Nonta
-00019020: 7861 626c 6520 4c6f 7373 6573 222c 0d0a  xable Losses",..
-00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019040: 2020 2020 2020 2020 2020 2020 2020 224e                "N
-00019050: 6f6e 2d4f 702e 2049 6e63 6f6d 6522 3a20  on-Op. Income": 
-00019060: 224e 6f6e 2d4f 7065 7261 7469 6f6e 616c  "Non-Operational
-00019070: 2049 6e63 6f6d 6522 2c0d 0a20 2020 2020   Income",..     
-00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019090: 2020 2020 2020 2020 2022 496e 7465 7265           "Intere
-000190a0: 7374 223a 2022 496e 7465 7265 7374 2050  st": "Interest P
-000190b0: 6179 6d65 6e74 7322 7d0d 0a0d 0a20 2020  ayments"}....   
-000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190d0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000190f0: 6620 6167 656e 7431 203d 3d20 6d79 5f61  f agent1 == my_a
-00019100: 6765 6e74 3a0d 0a20 2020 2020 2020 2020  gent:..         
-00019110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019120: 2020 2073 6967 6e20 3d20 222d 220d 0a20     sign = "-".. 
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 2020 2249 6e74 6572 6573 7420 5061 796d    "Interest Paym
+00018b30: 656e 7473 223a 205b 5d0d 0a20 2020 2020  ents": []..     
+00018b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b60: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+00018b70: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00018b80: 2020 6b20 3d20 300d 0a20 2020 2020 2020    k = 0..       
+00018b90: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00018ba0: 2020 2066 6f72 2066 696c 6564 6174 6120     for filedata 
+00018bb0: 696e 2073 656c 662e 656e 7472 795f 6461  in self.entry_da
+00018bc0: 7461 3a0d 0a20 2020 2020 2020 2020 2020  ta:..           
+00018bd0: 2020 2020 2061 6765 6e74 3120 3d20 6669       agent1 = fi
+00018be0: 6c65 6461 7461 5b22 6167 656e 7431 225d  ledata["agent1"]
+00018bf0: 2e73 7472 6970 2829 0d0a 2020 2020 2020  .strip()..      
+00018c00: 2020 2020 2020 2020 2020 6167 656e 7432            agent2
+00018c10: 203d 2066 696c 6564 6174 615b 2261 6765   = filedata["age
+00018c20: 6e74 3222 5d2e 7374 7269 7028 290d 0a0d  nt2"].strip()...
+00018c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c40: 2070 7269 6e74 2822 6167 656e 7431 222c   print("agent1",
+00018c50: 6167 656e 7431 2c22 6167 656e 7432 222c  agent1,"agent2",
+00018c60: 6167 656e 7432 290d 0a20 2020 2020 2020  agent2)..       
+00018c70: 2020 2020 2020 2020 2069 6620 6167 656e           if agen
+00018c80: 7431 203d 3d20 6d79 5f61 6765 6e74 3a0d  t1 == my_agent:.
+00018c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ca0: 2020 2020 2072 6566 5f61 6765 6e74 203d       ref_agent =
+00018cb0: 2022 6167 656e 7431 220d 0a20 2020 2020   "agent1"..     
+00018cc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018cd0: 6566 5f69 6e63 6f6d 6520 3d20 2269 6e63  ef_income = "inc
+00018ce0: 6f6d 6531 220d 0a0d 0a20 2020 2020 2020  ome1"....       
+00018cf0: 2020 2020 2020 2020 2065 6c69 6620 6167           elif ag
+00018d00: 656e 7432 203d 3d20 6d79 5f61 6765 6e74  ent2 == my_agent
+00018d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018d20: 2020 2020 2020 2072 6566 5f61 6765 6e74         ref_agent
+00018d30: 203d 2022 6167 656e 7432 220d 0a20 2020   = "agent2"..   
+00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d50: 2072 6566 5f69 6e63 6f6d 6520 3d20 2269   ref_income = "i
+00018d60: 6e63 6f6d 6532 220d 0a20 2020 2020 2020  ncome2"..       
+00018d70: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d90: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
+00018da0: 2020 2020 2020 2020 2020 2020 2361 7373              #ass
+00018db0: 6574 7331 203d 2066 696c 6564 6174 615b  ets1 = filedata[
+00018dc0: 2261 3122 5d20 2b20 225c 6e22 0d0a 2020  "a1"] + "\n"..  
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 236c                #l
+00018de0: 6961 6273 3120 3d20 6669 6c65 6461 7461  iabs1 = filedata
+00018df0: 5b22 6c31 225d 202b 2022 5c6e 2220 2b20  ["l1"] + "\n" + 
+00018e00: 6669 6c65 6461 7461 5b22 6531 225d 202b  filedata["e1"] +
+00018e10: 2022 5c6e 220d 0a0d 0a20 2020 2020 2020   "\n"....       
+00018e20: 2020 2020 2020 2020 2023 6173 7365 7473           #assets
+00018e30: 3220 3d20 6669 6c65 6461 7461 5b22 6132  2 = filedata["a2
+00018e40: 225d 202b 2022 5c6e 220d 0a20 2020 2020  "] + "\n"..     
+00018e50: 2020 2020 2020 2020 2020 2023 6c69 6162             #liab
+00018e60: 7332 203d 2066 696c 6564 6174 615b 226c  s2 = filedata["l
+00018e70: 3222 5d20 2b20 225c 6e22 202b 2066 696c  2"] + "\n" + fil
+00018e80: 6564 6174 615b 2265 3222 5d20 2b20 225c  edata["e2"] + "\
+00018e90: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
+00018ea0: 2020 2020 2020 6966 2028 6167 656e 7431        if (agent1
+00018eb0: 203d 3d20 6d79 5f61 6765 6e74 206f 7220   == my_agent or 
+00018ec0: 6167 656e 7432 203d 3d20 6d79 5f61 6765  agent2 == my_age
+00018ed0: 6e74 2920 616e 6420 7374 7228 6669 6c65  nt) and str(file
+00018ee0: 6461 7461 5b72 6566 5f69 6e63 6f6d 655d  data[ref_income]
+00018ef0: 2920 213d 2027 4e6f 6e65 273a 0d0a 2020  ) != 'None':..  
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 6d79 6469 6374 203d 207b 2247 6169    mydict = {"Gai
+00018f20: 6e22 3a20 2247 6169 6e73 222c 0d0a 2020  n": "Gains",..  
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 2020 2020 2020 2020 2020 2020 224c 6f73              "Los
+00018f50: 7322 3a20 224c 6f73 7365 7322 2c0d 0a20  s": "Losses",.. 
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f70: 2020 2020 2020 2020 2020 2020 2022 4578               "Ex
+00018f80: 7065 6e73 6522 3a20 2245 7870 656e 7365  pense": "Expense
+00018f90: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 2020 2022 5265 7665 6e75 6522 3a20 2252     "Revenue": "R
+00018fc0: 6576 656e 7565 7322 2c0d 0a20 2020 2020  evenues",..     
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fe0: 2020 2020 2020 2020 2022 5461 7822 3a20           "Tax": 
+00018ff0: 2254 6178 6573 222c 0d0a 2020 2020 2020  "Taxes",..      
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 2020 2020 2020 2020 224e 6f6e 7461 782e          "Nontax.
+00019020: 2050 726f 6669 7422 3a20 224e 6f6e 7461   Profit": "Nonta
+00019030: 7861 626c 6520 5072 6f66 6974 7322 2c0d  xable Profits",.
+00019040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019050: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019060: 4e6f 6e74 6178 2e20 4c6f 7373 223a 2022  Nontax. Loss": "
+00019070: 4e6f 6e74 6178 6162 6c65 204c 6f73 7365  Nontaxable Losse
+00019080: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2020 2022 4e6f 6e2d 4f70 2e20 496e 636f     "Non-Op. Inco
+000190b0: 6d65 223a 2022 4e6f 6e2d 4f70 6572 6174  me": "Non-Operat
+000190c0: 696f 6e61 6c20 496e 636f 6d65 222c 0d0a  ional Income",..
+000190d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190e0: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+000190f0: 6e74 6572 6573 7422 3a20 2249 6e74 6572  nterest": "Inter
+00019100: 6573 7420 5061 796d 656e 7473 227d 0d0a  est Payments"}..
+00019110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019120: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
 00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019140: 2020 2020 2020 2069 6620 6167 656e 7432         if agent2
-00019150: 203d 3d20 6d79 5f61 6765 6e74 3a0d 0a20   == my_agent:.. 
+00019140: 2020 2020 6966 2061 6765 6e74 3120 3d3d      if agent1 ==
+00019150: 206d 795f 6167 656e 743a 0d0a 2020 2020   my_agent:..    
 00019160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019170: 2020 2020 2020 2020 2020 2073 6967 6e20             sign 
-00019180: 3d20 222b 220d 0a0d 0a20 2020 2020 2020  = "+"....       
-00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191a0: 2071 203d 2073 796d 7079 2e6c 6174 6578   q = sympy.latex
-000191b0: 2873 796d 7079 2e73 696d 706c 6966 7928  (sympy.simplify(
-000191c0: 7369 676e 202b 2066 696c 6564 6174 615b  sign + filedata[
-000191d0: 2271 7561 6e74 6974 7922 5d29 2c20 6d6f  "quantity"]), mo
-000191e0: 6465 3d22 706c 6169 6e22 290d 0a20 2020  de="plain")..   
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 2020 2073 7562 6a65 6374 203d 2066       subject = f
-00019210: 696c 6564 6174 615b 2273 7562 6a65 6374  iledata["subject
-00019220: 225d 2e72 6570 6c61 6365 2822 5f22 2c20  "].replace("_", 
-00019230: 2220 2229 2e63 6170 6974 616c 697a 6528  " ").capitalize(
-00019240: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019250: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00019260: 2822 2020 2020 2020 666f 756e 6422 2c71  ("      found",q
-00019270: 2c73 7562 6a65 6374 290d 0a20 2020 2020  ,subject)..     
-00019280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019290: 2020 2074 7065 203d 206d 7964 6963 745b     tpe = mydict[
-000192a0: 6669 6c65 6461 7461 5b72 6566 5f69 6e63  filedata[ref_inc
-000192b0: 6f6d 655d 5d0d 0a20 2020 2020 2020 2020  ome]]..         
-000192c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000192d0: 6f6d 6269 6e65 645f 696e 636f 6d65 5b22  ombined_income["
-000192e0: 5479 7065 225d 2e61 7070 656e 6428 7470  Type"].append(tp
-000192f0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00019300: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-00019310: 696e 6564 5f69 6e63 6f6d 655b 2253 7562  ined_income["Sub
-00019320: 6a65 6374 225d 2e61 7070 656e 6428 7375  ject"].append(su
-00019330: 626a 6563 7429 0d0a 2020 2020 2020 2020  bject)..        
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 636f 6d62 696e 6564 5f69 6e63 6f6d 655b  combined_income[
-00019360: 2251 7561 6e74 6974 7922 5d2e 6170 7065  "Quantity"].appe
-00019370: 6e64 2873 7472 2871 2929 0d0a 2020 2020  nd(str(q))..    
-00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019390: 2020 2020 636f 6d62 696e 6564 5f69 6e63      combined_inc
-000193a0: 6f6d 655b 2253 686f 7274 204e 616d 6522  ome["Short Name"
-000193b0: 5d2e 6170 7065 6e64 2866 696c 6564 6174  ].append(filedat
-000193c0: 615b 2273 686f 7274 6e61 6d65 225d 2e73  a["shortname"].s
-000193d0: 7472 6970 2829 290d 0a0d 0a20 2020 2020  trip())....     
-000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193f0: 2020 2069 6620 7470 6520 696e 205b 2247     if tpe in ["G
-00019400: 6169 6e73 222c 224c 6f73 7365 7322 2c22  ains","Losses","
-00019410: 4578 7065 6e73 6573 222c 2252 6576 656e  Expenses","Reven
-00019420: 7565 7322 5d3a 0d0a 2020 2020 2020 2020  ues"]:..        
+00019170: 2020 2020 2020 2020 7369 676e 203d 2022          sign = "
+00019180: 2d22 0d0a 2020 2020 2020 2020 2020 2020  -"..            
+00019190: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000191a0: 6765 6e74 3220 3d3d 206d 795f 6167 656e  gent2 == my_agen
+000191b0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191d0: 7369 676e 203d 2022 2b22 0d0a 0d0a 2020  sign = "+"....  
+000191e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191f0: 2020 2020 2020 7120 3d20 7379 6d70 792e        q = sympy.
+00019200: 6c61 7465 7828 7379 6d70 792e 7369 6d70  latex(sympy.simp
+00019210: 6c69 6679 2873 6967 6e20 2b20 6669 6c65  lify(sign + file
+00019220: 6461 7461 5b22 7175 616e 7469 7479 225d  data["quantity"]
+00019230: 292c 206d 6f64 653d 2270 6c61 696e 2229  ), mode="plain")
+00019240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019250: 2020 2020 2020 2020 2020 7375 626a 6563            subjec
+00019260: 7420 3d20 6669 6c65 6461 7461 5b22 7375  t = filedata["su
+00019270: 626a 6563 7422 5d2e 7265 706c 6163 6528  bject"].replace(
+00019280: 225f 222c 2022 2022 292e 6361 7069 7461  "_", " ").capita
+00019290: 6c69 7a65 2829 0d0a 2020 2020 2020 2020  lize()..        
+000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192b0: 7072 696e 7428 2220 2020 2020 2066 6f75  print("      fou
+000192c0: 6e64 222c 712c 7375 626a 6563 7429 0d0a  nd",q,subject)..
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2020 2020 2020 7470 6520 3d20 6d79          tpe = my
+000192f0: 6469 6374 5b66 696c 6564 6174 615b 7265  dict[filedata[re
+00019300: 665f 696e 636f 6d65 5d5d 0d0a 2020 2020  f_income]]..    
+00019310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019320: 2020 2020 636f 6d62 696e 6564 5f69 6e63      combined_inc
+00019330: 6f6d 655b 2254 7970 6522 5d2e 6170 7065  ome["Type"].appe
+00019340: 6e64 2874 7065 290d 0a20 2020 2020 2020  nd(tpe)..       
+00019350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019360: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
+00019370: 5b22 5375 626a 6563 7422 5d2e 6170 7065  ["Subject"].appe
+00019380: 6e64 2873 7562 6a65 6374 290d 0a20 2020  nd(subject)..   
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 2020 2020 2063 6f6d 6269 6e65 645f 696e       combined_in
+000193b0: 636f 6d65 5b22 5175 616e 7469 7479 225d  come["Quantity"]
+000193c0: 2e61 7070 656e 6428 7374 7228 7129 290d  .append(str(q)).
+000193d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000193e0: 2020 2020 2020 2020 2063 6f6d 6269 6e65           combine
+000193f0: 645f 696e 636f 6d65 5b22 5368 6f72 7420  d_income["Short 
+00019400: 4e61 6d65 225d 2e61 7070 656e 6428 6669  Name"].append(fi
+00019410: 6c65 6461 7461 5b22 7368 6f72 746e 616d  ledata["shortnam
+00019420: 6522 5d2e 7374 7269 7028 2929 0d0a 0d0a  e"].strip())....
 00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2020 636f 6d62 696e 6564 5f69 6e63      combined_inc
-00019450: 6f6d 655b 2252 616e 6b69 6e67 225d 2e61  ome["Ranking"].a
-00019460: 7070 656e 6428 3029 0d0a 2020 2020 2020  ppend(0)..      
-00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019480: 2020 656c 6966 2074 7065 2069 6e20 5b22    elif tpe in ["
-00019490: 4e6f 6e2d 4f70 6572 6174 696f 6e61 6c20  Non-Operational 
-000194a0: 496e 636f 6d65 222c 2249 6e74 6572 6573  Income","Interes
-000194b0: 7420 5061 796d 656e 7473 225d 3a0d 0a20  t Payments"]:.. 
+00019440: 2020 2020 2020 2020 6966 2074 7065 2069          if tpe i
+00019450: 6e20 5b22 4761 696e 7322 2c22 4c6f 7373  n ["Gains","Loss
+00019460: 6573 222c 2245 7870 656e 7365 7322 2c22  es","Expenses","
+00019470: 5265 7665 6e75 6573 225d 3a0d 0a20 2020  Revenues"]:..   
+00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019490: 2020 2020 2020 2020 2063 6f6d 6269 6e65           combine
+000194a0: 645f 696e 636f 6d65 5b22 5261 6e6b 696e  d_income["Rankin
+000194b0: 6722 5d2e 6170 7065 6e64 2830 290d 0a20  g"].append(0).. 
 000194c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194d0: 2020 2020 2020 2020 2020 2063 6f6d 6269             combi
-000194e0: 6e65 645f 696e 636f 6d65 5b22 5261 6e6b  ned_income["Rank
-000194f0: 696e 6722 5d2e 6170 7065 6e64 2831 290d  ing"].append(1).
-00019500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019510: 2020 2020 2020 2020 2065 6c69 6620 7470           elif tp
-00019520: 6520 696e 205b 2254 6178 6573 225d 3a0d  e in ["Taxes"]:.
-00019530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019540: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-00019550: 6269 6e65 645f 696e 636f 6d65 5b22 5261  bined_income["Ra
-00019560: 6e6b 696e 6722 5d2e 6170 7065 6e64 2832  nking"].append(2
-00019570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019580: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00019590: 7470 6520 696e 205b 224e 6f6e 7461 7861  tpe in ["Nontaxa
-000195a0: 626c 6520 5072 6f66 6974 7322 2c20 224e  ble Profits", "N
-000195b0: 6f6e 7461 7861 626c 6520 4c6f 7373 6573  ontaxable Losses
-000195c0: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
+000194d0: 2020 2020 2020 2065 6c69 6620 7470 6520         elif tpe 
+000194e0: 696e 205b 224e 6f6e 2d4f 7065 7261 7469  in ["Non-Operati
+000194f0: 6f6e 616c 2049 6e63 6f6d 6522 2c22 496e  onal Income","In
+00019500: 7465 7265 7374 2050 6179 6d65 6e74 7322  terest Payments"
+00019510: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019530: 636f 6d62 696e 6564 5f69 6e63 6f6d 655b  combined_income[
+00019540: 2252 616e 6b69 6e67 225d 2e61 7070 656e  "Ranking"].appen
+00019550: 6428 3129 0d0a 2020 2020 2020 2020 2020  d(1)..          
+00019560: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00019570: 6966 2074 7065 2069 6e20 5b22 5461 7865  if tpe in ["Taxe
+00019580: 7322 5d3a 0d0a 2020 2020 2020 2020 2020  s"]:..          
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2020 636f 6d62 696e 6564 5f69 6e63 6f6d    combined_incom
+000195b0: 655b 2252 616e 6b69 6e67 225d 2e61 7070  e["Ranking"].app
+000195c0: 656e 6428 3229 0d0a 2020 2020 2020 2020  end(2)..        
 000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195e0: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
-000195f0: 5b22 5261 6e6b 696e 6722 5d2e 6170 7065  ["Ranking"].appe
-00019600: 6e64 2833 290d 0a20 2020 2020 2020 2020  nd(3)..         
-00019610: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019620: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019640: 2020 636f 6d62 696e 6564 5f69 6e63 6f6d    combined_incom
-00019650: 655b 2252 616e 6b69 6e67 225d 2e61 7070  e["Ranking"].app
-00019660: 656e 6428 3429 0d0a 0d0a 0d0a 2020 2020  end(4)......    
-00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019680: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00019690: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 7365 6c66 2e6e 6f74 6966 7928 0d0a 2020  self.notify(..  
-000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196d0: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
-000196e0: 7420 6861 6e64 6c65 2074 6865 2073 796d  t handle the sym
-000196f0: 626f 6c69 6320 6578 7072 6573 7369 6f6e  bolic expression
-00019700: 2025 7322 2025 2073 6967 6e20 2b20 6669   %s" % sign + fi
-00019710: 6c65 6461 7461 5b22 7175 616e 7469 7479  ledata["quantity
-00019720: 225d 2c74 6974 6c65 3d22 4572 726f 7222  "],title="Error"
-00019730: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
-00019740: 6570 743a 0d0a 2020 2020 2020 2020 2020  ept:..          
-00019750: 2020 7365 6c66 2e6e 6f74 6966 7928 7469    self.notify(ti
-00019760: 746c 653d 2245 7272 6f72 222c 206d 6573  tle="Error", mes
-00019770: 7361 6765 3d22 416e 2065 7272 6f72 206f  sage="An error o
-00019780: 6363 7572 7265 642e 2229 0d0a 0d0a 2020  ccurred.")....  
-00019790: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000197a0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000197b0: 2070 642e 4461 7461 4672 616d 6528 636f   pd.DataFrame(co
-000197c0: 6d62 696e 6564 5f69 6e63 6f6d 6529 2e73  mbined_income).s
-000197d0: 6574 5f69 6e64 6578 2822 5375 626a 6563  et_index("Subjec
-000197e0: 7422 290d 0a0d 0a0d 0a20 2020 2020 2020  t")......       
-000197f0: 2020 2020 2023 2073 6f72 7420 6166 7465       # sort afte
-00019800: 7220 7261 6e6b 696e 670d 0a20 2020 2020  r ranking..     
-00019810: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00019820: 7265 7375 6c74 2e73 6f72 745f 7661 6c75  result.sort_valu
-00019830: 6573 2827 5261 6e6b 696e 6727 290d 0a0d  es('Ranking')...
-00019840: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00019850: 656d 6f76 6520 7261 6e6b 696e 670d 0a20  emove ranking.. 
-00019860: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00019870: 7420 3d20 7265 7375 6c74 2e64 726f 7028  t = result.drop(
-00019880: 636f 6c75 6d6e 733d 2022 5261 6e6b 696e  columns= "Rankin
-00019890: 6722 290d 0a0d 0a20 2020 2020 2020 2020  g")....         
-000198a0: 2020 206d 6f64 656c 203d 2050 616e 6461     model = Panda
-000198b0: 734d 6f64 656c 2872 6573 756c 7429 0d0a  sModel(result)..
-000198c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000198d0: 206d 795f 6167 656e 7420 6e6f 7420 696e   my_agent not in
-000198e0: 2049 6e63 6f6d 6556 6965 7765 722e 696e   IncomeViewer.in
-000198f0: 7374 616e 6365 733a 0d0a 2020 2020 2020  stances:..      
-00019900: 2020 2020 2020 2020 2020 6d79 7669 6577            myview
-00019910: 203d 2049 6e63 6f6d 6556 6965 7765 7228   = IncomeViewer(
-00019920: 7365 6c66 2c6e 616d 653d 6d79 5f61 6765  self,name=my_age
-00019930: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00019940: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00019950: 2020 2020 2020 2020 6d79 7669 6577 203d          myview =
-00019960: 2049 6e63 6f6d 6556 6965 7765 722e 696e   IncomeViewer.in
-00019970: 7374 616e 6365 735b 6d79 5f61 6765 6e74  stances[my_agent
-00019980: 5d0d 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-00019990: 206d 7669 6577 2e73 6574 4765 6f6d 6574   mview.setGeomet
-000199a0: 7279 2831 3030 2c35 3030 290d 0a20 2020  ry(100,500)..   
-000199b0: 2020 2020 2020 2020 206d 7976 6965 772e           myview.
-000199c0: 7365 745f 6d6f 6465 6c28 6d6f 6465 6c29  set_model(model)
-000199d0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000199e0: 6d76 6965 772e 7765 6256 6965 772e 7365  mview.webView.se
-000199f0: 7448 746d 6c28 6466 5f68 746d 6c29 0d0a  tHtml(df_html)..
-00019a00: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00019a10: 206e 6f74 2073 656c 662e 7465 7374 5f6d   not self.test_m
-00019a20: 6f64 653a 0d0a 2020 2020 2020 2020 2020  ode:..          
-00019a30: 2020 2020 2020 6d79 7669 6577 2e73 686f        myview.sho
-00019a40: 7728 290d 0a0d 0a20 2020 2020 2020 2065  w()....        e
-00019a50: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00019a60: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-00019a70: 2020 2073 656c 662e 6e6f 7469 6679 2874     self.notify(t
-00019a80: 6974 6c65 3d22 4572 726f 7222 2c20 6d65  itle="Error", me
-00019a90: 7373 6167 653d 2241 6e20 6572 726f 7220  ssage="An error 
-00019aa0: 6f63 6375 7272 6564 2e22 202b 2073 7472  occurred." + str
-00019ab0: 2865 2929 0d0a 0d0a 0d0a 2020 2020 6465  (e))......    de
-00019ac0: 6620 6765 6e5f 6361 7368 666c 6f77 5f73  f gen_cashflow_s
-00019ad0: 696e 676c 6528 7365 6c66 293a 0d0a 2020  ingle(self):..  
-00019ae0: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
-00019af0: 6177 6361 6e76 6173 2e68 6967 686c 6967  awcanvas.highlig
-00019b00: 6874 6564 2069 7320 4e6f 6e65 3a0d 0a20  hted is None:.. 
-00019b10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019b20: 6e6f 7469 6679 2874 6974 6c65 3d22 4e6f  notify(title="No
-00019b30: 2061 6765 6e74 2073 656c 6563 7465 6422   agent selected"
-00019b40: 2c20 6d65 7373 6167 653d 224e 6f20 6167  , message="No ag
-00019b50: 656e 7420 7365 6c65 6374 6564 2e20 506c  ent selected. Pl
-00019b60: 6561 7365 2073 656c 6563 7420 6f6e 6520  ease select one 
-00019b70: 6669 7273 742e 2229 0d0a 2020 2020 2020  first.")..      
-00019b80: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00019b90: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
-00019ba0: 6177 6361 6e76 6173 2e68 6967 686c 6967  awcanvas.highlig
-00019bb0: 6874 6564 2e69 7368 656c 7065 723a 0d0a  hted.ishelper:..
-00019bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019bd0: 2e6e 6f74 6966 7928 7469 746c 653d 224e  .notify(title="N
-00019be0: 6f20 6167 656e 7420 7365 6c65 6374 6564  o agent selected
-00019bf0: 222c 206d 6573 7361 6765 3d22 4e6f 2076  ", message="No v
-00019c00: 616c 6964 2062 6f78 2073 656c 6563 7465  alid box selecte
-00019c10: 642e 2050 6c65 6173 6520 7365 6c65 6374  d. Please select
-00019c20: 2061 6e20 6167 656e 742e 2229 0d0a 2020   an agent.")..  
-00019c30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00019c40: 0d0a 2020 2020 2020 2020 6d79 5f61 6765  ..        my_age
-00019c50: 6e74 203d 2073 656c 662e 6472 6177 6361  nt = self.drawca
-00019c60: 6e76 6173 2e68 6967 686c 6967 6874 6564  nvas.highlighted
-00019c70: 2e6e 616d 650d 0a0d 0a20 2020 2020 2020  .name....       
-00019c80: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
-00019c90: 203d 2020 7b22 5375 626a 6563 7422 3a5b   =  {"Subject":[
-00019ca0: 5d2c 2253 686f 7274 204e 616d 6522 3a20  ],"Short Name": 
-00019cb0: 5b5d 2c22 5175 616e 7469 7479 223a 5b5d  [],"Quantity":[]
-00019cc0: 2c20 2254 7970 6522 3a5b 5d2c 2022 5261  , "Type":[], "Ra
-00019cd0: 6e6b 696e 6722 3a5b 5d7d 2023 2072 616e  nking":[]} # ran
-00019ce0: 6b69 6e67 2077 696c 6c20 6265 2072 656d  king will be rem
-00019cf0: 6f76 6564 206c 6174 6572 0d0a 2020 2020  oved later..    
-00019d00: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00019d10: 2022 2222 0d0a 2020 2020 2020 2020 6b20   """..        k 
-00019d20: 3d20 300d 0a20 2020 2020 2020 2074 7279  = 0..        try
-00019d30: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00019d40: 6f72 2066 696c 6564 6174 6120 696e 2073  or filedata in s
-00019d50: 656c 662e 656e 7472 795f 6461 7461 3a0d  elf.entry_data:.
-00019d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d70: 2061 6765 6e74 3120 3d20 6669 6c65 6461   agent1 = fileda
-00019d80: 7461 5b22 6167 656e 7431 225d 2e73 7472  ta["agent1"].str
-00019d90: 6970 2829 0d0a 2020 2020 2020 2020 2020  ip()..          
-00019da0: 2020 2020 2020 6167 656e 7432 203d 2066        agent2 = f
-00019db0: 696c 6564 6174 615b 2261 6765 6e74 3222  iledata["agent2"
-00019dc0: 5d2e 7374 7269 7028 290d 0a0d 0a20 2020  ].strip()....   
-00019dd0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00019de0: 6e74 2822 6167 656e 7431 222c 6167 656e  nt("agent1",agen
-00019df0: 7431 2c22 6167 656e 7432 222c 6167 656e  t1,"agent2",agen
-00019e00: 7432 290d 0a20 2020 2020 2020 2020 2020  t2)..           
-00019e10: 2020 2020 2069 6620 6167 656e 7431 203d       if agent1 =
-00019e20: 3d20 6d79 5f61 6765 6e74 3a0d 0a20 2020  = my_agent:..   
-00019e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e40: 2072 6566 5f61 6765 6e74 203d 2022 6167   ref_agent = "ag
-00019e50: 656e 7431 220d 0a20 2020 2020 2020 2020  ent1"..         
-00019e60: 2020 2020 2020 2020 2020 2072 6566 5f69             ref_i
-00019e70: 6e63 6f6d 6520 3d20 2263 6173 6866 6c6f  ncome = "cashflo
-00019e80: 7731 220d 0a0d 0a20 2020 2020 2020 2020  w1"....         
-00019e90: 2020 2020 2020 2065 6c69 6620 6167 656e         elif agen
-00019ea0: 7432 203d 3d20 6d79 5f61 6765 6e74 3a0d  t2 == my_agent:.
-00019eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ec0: 2020 2020 2072 6566 5f61 6765 6e74 203d       ref_agent =
-00019ed0: 2022 6167 656e 7432 220d 0a20 2020 2020   "agent2"..     
-00019ee0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019ef0: 6566 5f69 6e63 6f6d 6520 3d20 2263 6173  ef_income = "cas
-00019f00: 6866 6c6f 7732 220d 0a20 2020 2020 2020  hflow2"..       
-00019f10: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00019f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f30: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
-00019f40: 2020 2020 2020 2020 2020 2020 2361 7373              #ass
-00019f50: 6574 7331 203d 2066 696c 6564 6174 615b  ets1 = filedata[
-00019f60: 2261 3122 5d20 2b20 225c 6e22 0d0a 2020  "a1"] + "\n"..  
-00019f70: 2020 2020 2020 2020 2020 2020 2020 236c                #l
-00019f80: 6961 6273 3120 3d20 6669 6c65 6461 7461  iabs1 = filedata
-00019f90: 5b22 6c31 225d 202b 2022 5c6e 2220 2b20  ["l1"] + "\n" + 
-00019fa0: 6669 6c65 6461 7461 5b22 6531 225d 202b  filedata["e1"] +
-00019fb0: 2022 5c6e 220d 0a0d 0a20 2020 2020 2020   "\n"....       
-00019fc0: 2020 2020 2020 2020 2023 6173 7365 7473           #assets
-00019fd0: 3220 3d20 6669 6c65 6461 7461 5b22 6132  2 = filedata["a2
-00019fe0: 225d 202b 2022 5c6e 220d 0a20 2020 2020  "] + "\n"..     
-00019ff0: 2020 2020 2020 2020 2020 2023 6c69 6162             #liab
-0001a000: 7332 203d 2066 696c 6564 6174 615b 226c  s2 = filedata["l
-0001a010: 3222 5d20 2b20 225c 6e22 202b 2066 696c  2"] + "\n" + fil
-0001a020: 6564 6174 615b 2265 3222 5d20 2b20 225c  edata["e2"] + "\
-0001a030: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
-0001a040: 2020 2020 2020 6966 2028 6167 656e 7431        if (agent1
-0001a050: 203d 3d20 6d79 5f61 6765 6e74 206f 7220   == my_agent or 
-0001a060: 6167 656e 7432 203d 3d20 6d79 5f61 6765  agent2 == my_age
-0001a070: 6e74 2920 616e 6420 7374 7228 6669 6c65  nt) and str(file
-0001a080: 6461 7461 5b72 6566 5f69 6e63 6f6d 655d  data[ref_income]
-0001a090: 2920 213d 2027 4e6f 6e65 273a 0d0a 2020  ) != 'None':..  
-0001a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0b0: 2020 6d79 6469 6374 203d 207b 2247 6169    mydict = {"Gai
-0001a0c0: 6e22 3a20 2247 6169 6e73 222c 0d0a 2020  n": "Gains",..  
-0001a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0e0: 2020 2020 2020 2020 2020 2020 224c 6f73              "Los
-0001a0f0: 7322 3a20 224c 6f73 7365 7322 2c0d 0a20  s": "Losses",.. 
-0001a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a110: 2020 2020 2020 2020 2020 2020 2022 4578               "Ex
-0001a120: 7065 6e73 6522 3a20 2245 7870 656e 7365  pense": "Expense
-0001a130: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-0001a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a150: 2020 2022 5265 7665 6e75 6522 3a20 2252     "Revenue": "R
-0001a160: 6576 656e 7565 7322 2c0d 0a20 2020 2020  evenues",..     
-0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a180: 2020 2020 2020 2020 2022 5461 7822 3a20           "Tax": 
-0001a190: 2254 6178 6573 222c 0d0a 2020 2020 2020  "Taxes",..      
-0001a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1b0: 2020 2020 2020 2020 224e 6f6e 7461 782e          "Nontax.
-0001a1c0: 2050 726f 6669 7422 3a20 224e 6f6e 7461   Profit": "Nonta
-0001a1d0: 7861 626c 6520 5072 6f66 6974 7322 2c0d  xable Profits",.
-0001a1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001a200: 4e6f 6e74 6178 2e20 4c6f 7373 223a 2022  Nontax. Loss": "
-0001a210: 4e6f 6e74 6178 6162 6c65 204c 6f73 7365  Nontaxable Losse
-0001a220: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-0001a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a240: 2020 2022 4e6f 6e2d 4f70 2e20 496e 636f     "Non-Op. Inco
-0001a250: 6d65 223a 2022 4e6f 6e2d 4f70 6572 6174  me": "Non-Operat
-0001a260: 696f 6e61 6c20 496e 636f 6d65 222c 0d0a  ional Income",..
-0001a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a280: 2020 2020 2020 2020 2020 2020 2020 2249                "I
-0001a290: 6e74 6572 6573 7422 3a20 2249 6e74 6572  nterest": "Inter
-0001a2a0: 6573 7420 5061 796d 656e 7473 227d 0d0a  est Payments"}..
-0001a2b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a2c0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+000195e0: 656c 6966 2074 7065 2069 6e20 5b22 4e6f  elif tpe in ["No
+000195f0: 6e74 6178 6162 6c65 2050 726f 6669 7473  ntaxable Profits
+00019600: 222c 2022 4e6f 6e74 6178 6162 6c65 204c  ", "Nontaxable L
+00019610: 6f73 7365 7322 5d3a 0d0a 2020 2020 2020  osses"]:..      
+00019620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019630: 2020 2020 2020 636f 6d62 696e 6564 5f69        combined_i
+00019640: 6e63 6f6d 655b 2252 616e 6b69 6e67 225d  ncome["Ranking"]
+00019650: 2e61 7070 656e 6428 3329 0d0a 2020 2020  .append(3)..    
+00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019670: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019690: 2020 2020 2020 2063 6f6d 6269 6e65 645f         combined_
+000196a0: 696e 636f 6d65 5b22 5261 6e6b 696e 6722  income["Ranking"
+000196b0: 5d2e 6170 7065 6e64 2834 290d 0a0d 0a0d  ].append(4).....
+000196c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000196d0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000196e0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019700: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
+00019710: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00019720: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019730: 4361 6e6e 6f74 2068 616e 646c 6520 7468  Cannot handle th
+00019740: 6520 7379 6d62 6f6c 6963 2065 7870 7265  e symbolic expre
+00019750: 7373 696f 6e20 2573 2220 2520 7369 676e  ssion %s" % sign
+00019760: 202b 2066 696c 6564 6174 615b 2271 7561   + filedata["qua
+00019770: 6e74 6974 7922 5d2c 7469 746c 653d 2245  ntity"],title="E
+00019780: 7272 6f72 2229 0d0a 0d0a 2020 2020 2020  rror")....      
+00019790: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
+000197a0: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
+000197b0: 6679 2874 6974 6c65 3d22 4572 726f 7222  fy(title="Error"
+000197c0: 2c20 6d65 7373 6167 653d 2241 6e20 6572  , message="An er
+000197d0: 726f 7220 6f63 6375 7272 6564 2e22 290d  ror occurred.").
+000197e0: 0a0d 0a20 2020 2020 2020 2074 7279 3a0d  ...        try:.
+000197f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00019800: 756c 7420 3d20 7064 2e44 6174 6146 7261  ult = pd.DataFra
+00019810: 6d65 2863 6f6d 6269 6e65 645f 696e 636f  me(combined_inco
+00019820: 6d65 292e 7365 745f 696e 6465 7828 2253  me).set_index("S
+00019830: 7562 6a65 6374 2229 0d0a 0d0a 0d0a 2020  ubject")......  
+00019840: 2020 2020 2020 2020 2020 2320 736f 7274            # sort
+00019850: 2061 6674 6572 2072 616e 6b69 6e67 0d0a   after ranking..
+00019860: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00019870: 6c74 203d 2072 6573 756c 742e 736f 7274  lt = result.sort
+00019880: 5f76 616c 7565 7328 2752 616e 6b69 6e67  _values('Ranking
+00019890: 2729 0d0a 0d0a 2020 2020 2020 2020 2020  ')....          
+000198a0: 2020 2320 7265 6d6f 7665 2072 616e 6b69    # remove ranki
+000198b0: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
+000198c0: 7265 7375 6c74 203d 2072 6573 756c 742e  result = result.
+000198d0: 6472 6f70 2863 6f6c 756d 6e73 3d20 2252  drop(columns= "R
+000198e0: 616e 6b69 6e67 2229 0d0a 0d0a 2020 2020  anking")....    
+000198f0: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
+00019900: 5061 6e64 6173 4d6f 6465 6c28 7265 7375  PandasModel(resu
+00019910: 6c74 290d 0a0d 0a20 2020 2020 2020 2020  lt)....         
+00019920: 2020 2069 6620 6d79 5f61 6765 6e74 206e     if my_agent n
+00019930: 6f74 2069 6e20 496e 636f 6d65 5669 6577  ot in IncomeView
+00019940: 6572 2e69 6e73 7461 6e63 6573 3a0d 0a20  er.instances:.. 
+00019950: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00019960: 7976 6965 7720 3d20 496e 636f 6d65 5669  yview = IncomeVi
+00019970: 6577 6572 2873 656c 662c 6e61 6d65 3d6d  ewer(self,name=m
+00019980: 795f 6167 656e 7429 0d0a 2020 2020 2020  y_agent)..      
+00019990: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000199a0: 2020 2020 2020 2020 2020 2020 206d 7976               myv
+000199b0: 6965 7720 3d20 496e 636f 6d65 5669 6577  iew = IncomeView
+000199c0: 6572 2e69 6e73 7461 6e63 6573 5b6d 795f  er.instances[my_
+000199d0: 6167 656e 745d 0d0a 2020 2020 2020 2020  agent]..        
+000199e0: 2020 2020 2320 6d76 6965 772e 7365 7447      # mview.setG
+000199f0: 656f 6d65 7472 7928 3130 302c 3530 3029  eometry(100,500)
+00019a00: 0d0a 2020 2020 2020 2020 2020 2020 6d79  ..            my
+00019a10: 7669 6577 2e73 6574 5f6d 6f64 656c 286d  view.set_model(m
+00019a20: 6f64 656c 290d 0a20 2020 2020 2020 2020  odel)..         
+00019a30: 2020 2023 206d 7669 6577 2e77 6562 5669     # mview.webVi
+00019a40: 6577 2e73 6574 4874 6d6c 2864 665f 6874  ew.setHtml(df_ht
+00019a50: 6d6c 290d 0a0d 0a20 2020 2020 2020 2020  ml)....         
+00019a60: 2020 2069 6620 6e6f 7420 7365 6c66 2e74     if not self.t
+00019a70: 6573 745f 6d6f 6465 3a0d 0a20 2020 2020  est_mode:..     
+00019a80: 2020 2020 2020 2020 2020 206d 7976 6965             myvie
+00019a90: 772e 7368 6f77 2829 0d0a 0d0a 2020 2020  w.show()....    
+00019aa0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00019ab0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+00019ac0: 2020 2020 2020 2020 7365 6c66 2e6e 6f74          self.not
+00019ad0: 6966 7928 7469 746c 653d 2245 7272 6f72  ify(title="Error
+00019ae0: 222c 206d 6573 7361 6765 3d22 416e 2065  ", message="An e
+00019af0: 7272 6f72 206f 6363 7572 7265 642e 2220  rror occurred." 
+00019b00: 2b20 7374 7228 6529 290d 0a0d 0a0d 0a20  + str(e))...... 
+00019b10: 2020 2064 6566 2067 656e 5f63 6173 6866     def gen_cashf
+00019b20: 6c6f 775f 7369 6e67 6c65 2873 656c 6629  low_single(self)
+00019b30: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
+00019b40: 6c66 2e64 7261 7763 616e 7661 732e 6869  lf.drawcanvas.hi
+00019b50: 6768 6c69 6768 7465 6420 6973 204e 6f6e  ghlighted is Non
+00019b60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00019b70: 7365 6c66 2e6e 6f74 6966 7928 7469 746c  self.notify(titl
+00019b80: 653d 224e 6f20 6167 656e 7420 7365 6c65  e="No agent sele
+00019b90: 6374 6564 222c 206d 6573 7361 6765 3d22  cted", message="
+00019ba0: 4e6f 2061 6765 6e74 2073 656c 6563 7465  No agent selecte
+00019bb0: 642e 2050 6c65 6173 6520 7365 6c65 6374  d. Please select
+00019bc0: 206f 6e65 2066 6972 7374 2e22 290d 0a20   one first.").. 
+00019bd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00019be0: 6e0d 0a20 2020 2020 2020 2069 6620 7365  n..        if se
+00019bf0: 6c66 2e64 7261 7763 616e 7661 732e 6869  lf.drawcanvas.hi
+00019c00: 6768 6c69 6768 7465 642e 6973 6865 6c70  ghlighted.ishelp
+00019c10: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
+00019c20: 2073 656c 662e 6e6f 7469 6679 2874 6974   self.notify(tit
+00019c30: 6c65 3d22 4e6f 2061 6765 6e74 2073 656c  le="No agent sel
+00019c40: 6563 7465 6422 2c20 6d65 7373 6167 653d  ected", message=
+00019c50: 224e 6f20 7661 6c69 6420 626f 7820 7365  "No valid box se
+00019c60: 6c65 6374 6564 2e20 506c 6561 7365 2073  lected. Please s
+00019c70: 656c 6563 7420 616e 2061 6765 6e74 2e22  elect an agent."
+00019c80: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00019c90: 6574 7572 6e0d 0a20 2020 2020 2020 206d  eturn..        m
+00019ca0: 795f 6167 656e 7420 3d20 7365 6c66 2e64  y_agent = self.d
+00019cb0: 7261 7763 616e 7661 732e 6869 6768 6c69  rawcanvas.highli
+00019cc0: 6768 7465 642e 6e61 6d65 0d0a 0d0a 2020  ghted.name....  
+00019cd0: 2020 2020 2020 636f 6d62 696e 6564 5f69        combined_i
+00019ce0: 6e63 6f6d 6520 3d20 207b 2253 7562 6a65  ncome =  {"Subje
+00019cf0: 6374 223a 5b5d 2c22 5368 6f72 7420 4e61  ct":[],"Short Na
+00019d00: 6d65 223a 205b 5d2c 2251 7561 6e74 6974  me": [],"Quantit
+00019d10: 7922 3a5b 5d2c 2022 5479 7065 223a 5b5d  y":[], "Type":[]
+00019d20: 2c20 2252 616e 6b69 6e67 223a 5b5d 7d20  , "Ranking":[]} 
+00019d30: 2320 7261 6e6b 696e 6720 7769 6c6c 2062  # ranking will b
+00019d40: 6520 7265 6d6f 7665 6420 6c61 7465 720d  e removed later.
+00019d50: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00019d60: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00019d70: 2020 206b 203d 2030 0d0a 2020 2020 2020     k = 0..      
+00019d80: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00019d90: 2020 2020 666f 7220 6669 6c65 6461 7461      for filedata
+00019da0: 2069 6e20 7365 6c66 2e65 6e74 7279 5f64   in self.entry_d
+00019db0: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
+00019dc0: 2020 2020 2020 6167 656e 7431 203d 2066        agent1 = f
+00019dd0: 696c 6564 6174 615b 2261 6765 6e74 3122  iledata["agent1"
+00019de0: 5d2e 7374 7269 7028 290d 0a20 2020 2020  ].strip()..     
+00019df0: 2020 2020 2020 2020 2020 2061 6765 6e74             agent
+00019e00: 3220 3d20 6669 6c65 6461 7461 5b22 6167  2 = filedata["ag
+00019e10: 656e 7432 225d 2e73 7472 6970 2829 0d0a  ent2"].strip()..
+00019e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019e30: 2020 7072 696e 7428 2261 6765 6e74 3122    print("agent1"
+00019e40: 2c61 6765 6e74 312c 2261 6765 6e74 3222  ,agent1,"agent2"
+00019e50: 2c61 6765 6e74 3229 0d0a 2020 2020 2020  ,agent2)..      
+00019e60: 2020 2020 2020 2020 2020 6966 2061 6765            if age
+00019e70: 6e74 3120 3d3d 206d 795f 6167 656e 743a  nt1 == my_agent:
+00019e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019e90: 2020 2020 2020 7265 665f 6167 656e 7420        ref_agent 
+00019ea0: 3d20 2261 6765 6e74 3122 0d0a 2020 2020  = "agent1"..    
+00019eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ec0: 7265 665f 696e 636f 6d65 203d 2022 6361  ref_income = "ca
+00019ed0: 7368 666c 6f77 3122 0d0a 0d0a 2020 2020  shflow1"....    
+00019ee0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00019ef0: 2061 6765 6e74 3220 3d3d 206d 795f 6167   agent2 == my_ag
+00019f00: 656e 743a 0d0a 2020 2020 2020 2020 2020  ent:..          
+00019f10: 2020 2020 2020 2020 2020 7265 665f 6167            ref_ag
+00019f20: 656e 7420 3d20 2261 6765 6e74 3222 0d0a  ent = "agent2"..
+00019f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f40: 2020 2020 7265 665f 696e 636f 6d65 203d      ref_income =
+00019f50: 2022 6361 7368 666c 6f77 3222 0d0a 2020   "cashflow2"..  
+00019f60: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00019f70: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00019f80: 2020 2020 2020 2020 2070 6173 730d 0a0d           pass...
+00019f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019fa0: 2023 6173 7365 7473 3120 3d20 6669 6c65   #assets1 = file
+00019fb0: 6461 7461 5b22 6131 225d 202b 2022 5c6e  data["a1"] + "\n
+00019fc0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00019fd0: 2020 2023 6c69 6162 7331 203d 2066 696c     #liabs1 = fil
+00019fe0: 6564 6174 615b 226c 3122 5d20 2b20 225c  edata["l1"] + "\
+00019ff0: 6e22 202b 2066 696c 6564 6174 615b 2265  n" + filedata["e
+0001a000: 3122 5d20 2b20 225c 6e22 0d0a 0d0a 2020  1"] + "\n"....  
+0001a010: 2020 2020 2020 2020 2020 2020 2020 2361                #a
+0001a020: 7373 6574 7332 203d 2066 696c 6564 6174  ssets2 = filedat
+0001a030: 615b 2261 3222 5d20 2b20 225c 6e22 0d0a  a["a2"] + "\n"..
+0001a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a050: 236c 6961 6273 3220 3d20 6669 6c65 6461  #liabs2 = fileda
+0001a060: 7461 5b22 6c32 225d 202b 2022 5c6e 2220  ta["l2"] + "\n" 
+0001a070: 2b20 6669 6c65 6461 7461 5b22 6532 225d  + filedata["e2"]
+0001a080: 202b 2022 5c6e 220d 0a0d 0a20 2020 2020   + "\n"....     
+0001a090: 2020 2020 2020 2020 2020 2069 6620 2861             if (a
+0001a0a0: 6765 6e74 3120 3d3d 206d 795f 6167 656e  gent1 == my_agen
+0001a0b0: 7420 6f72 2061 6765 6e74 3220 3d3d 206d  t or agent2 == m
+0001a0c0: 795f 6167 656e 7429 2061 6e64 2073 7472  y_agent) and str
+0001a0d0: 2866 696c 6564 6174 615b 7265 665f 696e  (filedata[ref_in
+0001a0e0: 636f 6d65 5d29 2021 3d20 274e 6f6e 6527  come]) != 'None'
+0001a0f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a100: 2020 2020 2020 206d 7964 6963 7420 3d20         mydict = 
+0001a110: 7b22 4761 696e 223a 2022 4761 696e 7322  {"Gain": "Gains"
+0001a120: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a140: 2022 4c6f 7373 223a 2022 4c6f 7373 6573   "Loss": "Losses
+0001a150: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a170: 2020 2245 7870 656e 7365 223a 2022 4578    "Expense": "Ex
+0001a180: 7065 6e73 6573 222c 0d0a 2020 2020 2020  penses",..      
+0001a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1a0: 2020 2020 2020 2020 2252 6576 656e 7565          "Revenue
+0001a1b0: 223a 2022 5265 7665 6e75 6573 222c 0d0a  ": "Revenues",..
+0001a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+0001a1e0: 6178 223a 2022 5461 7865 7322 2c0d 0a20  ax": "Taxes",.. 
+0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a200: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
+0001a210: 6e74 6178 2e20 5072 6f66 6974 223a 2022  ntax. Profit": "
+0001a220: 4e6f 6e74 6178 6162 6c65 2050 726f 6669  Nontaxable Profi
+0001a230: 7473 222c 0d0a 2020 2020 2020 2020 2020  ts",..          
+0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a250: 2020 2020 224e 6f6e 7461 782e 204c 6f73      "Nontax. Los
+0001a260: 7322 3a20 224e 6f6e 7461 7861 626c 6520  s": "Nontaxable 
+0001a270: 4c6f 7373 6573 222c 0d0a 2020 2020 2020  Losses",..      
+0001a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a290: 2020 2020 2020 2020 224e 6f6e 2d4f 702e          "Non-Op.
+0001a2a0: 2049 6e63 6f6d 6522 3a20 224e 6f6e 2d4f   Income": "Non-O
+0001a2b0: 7065 7261 7469 6f6e 616c 2049 6e63 6f6d  perational Incom
+0001a2c0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
 0001a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2e0: 2020 2020 6966 2061 6765 6e74 3120 3d3d      if agent1 ==
-0001a2f0: 206d 795f 6167 656e 743a 0d0a 2020 2020   my_agent:..    
-0001a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a310: 2020 2020 2020 2020 7369 676e 203d 2022          sign = "
-0001a320: 2d22 0d0a 2020 2020 2020 2020 2020 2020  -"..            
-0001a330: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0001a340: 6765 6e74 3220 3d3d 206d 795f 6167 656e  gent2 == my_agen
-0001a350: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-0001a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a370: 7369 676e 203d 2022 2b22 0d0a 0d0a 2020  sign = "+"....  
+0001a2e0: 2020 2022 496e 7465 7265 7374 223a 2022     "Interest": "
+0001a2f0: 496e 7465 7265 7374 2050 6179 6d65 6e74  Interest Payment
+0001a300: 7322 7d0d 0a0d 0a20 2020 2020 2020 2020  s"}....         
+0001a310: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+0001a320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a330: 2020 2020 2020 2020 2069 6620 6167 656e           if agen
+0001a340: 7431 203d 3d20 6d79 5f61 6765 6e74 3a0d  t1 == my_agent:.
+0001a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a360: 2020 2020 2020 2020 2020 2020 2073 6967               sig
+0001a370: 6e20 3d20 222d 220d 0a20 2020 2020 2020  n = "-"..       
 0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 2020 2020 2020 7120 3d20 7379 6d70 792e        q = sympy.
-0001a3a0: 6c61 7465 7828 7379 6d70 792e 7369 6d70  latex(sympy.simp
-0001a3b0: 6c69 6679 2873 6967 6e20 2b20 6669 6c65  lify(sign + file
-0001a3c0: 6461 7461 5b22 7175 616e 7469 7479 225d  data["quantity"]
-0001a3d0: 292c 206d 6f64 653d 2270 6c61 696e 2229  ), mode="plain")
-0001a3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a3f0: 2020 2020 2020 2020 2020 7375 626a 6563            subjec
-0001a400: 7420 3d20 6669 6c65 6461 7461 5b22 7375  t = filedata["su
-0001a410: 626a 6563 7422 5d2e 7265 706c 6163 6528  bject"].replace(
-0001a420: 225f 222c 2022 2022 292e 6361 7069 7461  "_", " ").capita
-0001a430: 6c69 7a65 2829 0d0a 2020 2020 2020 2020  lize()..        
-0001a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a450: 7072 696e 7428 2220 2020 2020 2066 6f75  print("      fou
-0001a460: 6e64 222c 712c 7375 626a 6563 7429 0d0a  nd",q,subject)..
-0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a480: 2020 2020 2020 2020 7470 6520 3d20 6669          tpe = fi
-0001a490: 6c65 6461 7461 5b72 6566 5f69 6e63 6f6d  ledata[ref_incom
-0001a4a0: 655d 0d0a 2020 2020 2020 2020 2020 2020  e]..            
-0001a4b0: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-0001a4c0: 696e 6564 5f69 6e63 6f6d 655b 2254 7970  ined_income["Typ
-0001a4d0: 6522 5d2e 6170 7065 6e64 2874 7065 290d  e"].append(tpe).
-0001a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a4f0: 2020 2020 2020 2020 2063 6f6d 6269 6e65           combine
-0001a500: 645f 696e 636f 6d65 5b22 5375 626a 6563  d_income["Subjec
-0001a510: 7422 5d2e 6170 7065 6e64 2873 7562 6a65  t"].append(subje
-0001a520: 6374 290d 0a20 2020 2020 2020 2020 2020  ct)..           
-0001a530: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-0001a540: 6269 6e65 645f 696e 636f 6d65 5b22 5175  bined_income["Qu
-0001a550: 616e 7469 7479 225d 2e61 7070 656e 6428  antity"].append(
-0001a560: 7374 7228 7129 290d 0a20 2020 2020 2020  str(q))..       
-0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a580: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
-0001a590: 5b22 5368 6f72 7420 4e61 6d65 225d 2e61  ["Short Name"].a
-0001a5a0: 7070 656e 6428 6669 6c65 6461 7461 5b22  ppend(filedata["
-0001a5b0: 7368 6f72 746e 616d 6522 5d2e 7374 7269  shortname"].stri
-0001a5c0: 7028 2929 0d0a 2020 2020 2020 2020 2020  p())..          
-0001a5d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001a5e0: 6d62 696e 6564 5f69 6e63 6f6d 655b 2252  mbined_income["R
-0001a5f0: 616e 6b69 6e67 225d 2e61 7070 656e 6428  anking"].append(
-0001a600: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-0001a610: 2020 2020 2020 2020 2020 2020 2222 220d              """.
-0001a620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a630: 2020 2020 2020 2020 2069 6620 7470 6520           if tpe 
-0001a640: 696e 205b 2247 6169 6e73 222c 224c 6f73  in ["Gains","Los
-0001a650: 7365 7322 2c22 4578 7065 6e73 6573 222c  ses","Expenses",
-0001a660: 2252 6576 656e 7565 7322 5d3a 0d0a 2020  "Revenues"]:..  
-0001a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a680: 2020 2020 2020 2020 2020 636f 6d62 696e            combin
-0001a690: 6564 5f69 6e63 6f6d 655b 2252 616e 6b69  ed_income["Ranki
-0001a6a0: 6e67 225d 2e61 7070 656e 6428 3029 0d0a  ng"].append(0)..
-0001a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6c0: 2020 2020 2020 2020 656c 6966 2074 7065          elif tpe
-0001a6d0: 2069 6e20 5b22 4e6f 6e2d 4f70 6572 6174   in ["Non-Operat
-0001a6e0: 696f 6e61 6c20 496e 636f 6d65 222c 2249  ional Income","I
-0001a6f0: 6e74 6572 6573 7420 5061 796d 656e 7473  nterest Payments
-0001a700: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
-0001a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a720: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
-0001a730: 5b22 5261 6e6b 696e 6722 5d2e 6170 7065  ["Ranking"].appe
-0001a740: 6e64 2831 290d 0a20 2020 2020 2020 2020  nd(1)..         
-0001a750: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001a760: 6c69 6620 7470 6520 696e 205b 2254 6178  lif tpe in ["Tax
-0001a770: 6573 225d 3a0d 0a20 2020 2020 2020 2020  es"]:..         
-0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a790: 2020 2063 6f6d 6269 6e65 645f 696e 636f     combined_inco
-0001a7a0: 6d65 5b22 5261 6e6b 696e 6722 5d2e 6170  me["Ranking"].ap
-0001a7b0: 7065 6e64 2832 290d 0a20 2020 2020 2020  pend(2)..       
-0001a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7d0: 2065 6c69 6620 7470 6520 696e 205b 224e   elif tpe in ["N
-0001a7e0: 6f6e 7461 7861 626c 6520 5072 6f66 6974  ontaxable Profit
-0001a7f0: 7322 2c20 224e 6f6e 7461 7861 626c 6520  s", "Nontaxable 
-0001a800: 4c6f 7373 6573 225d 3a0d 0a20 2020 2020  Losses"]:..     
+0001a390: 2069 6620 6167 656e 7432 203d 3d20 6d79   if agent2 == my
+0001a3a0: 5f61 6765 6e74 3a0d 0a20 2020 2020 2020  _agent:..       
+0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3c0: 2020 2020 2073 6967 6e20 3d20 222b 220d       sign = "+".
+0001a3d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a3e0: 2020 2020 2020 2020 2020 2071 203d 2073             q = s
+0001a3f0: 796d 7079 2e6c 6174 6578 2873 796d 7079  ympy.latex(sympy
+0001a400: 2e73 696d 706c 6966 7928 7369 676e 202b  .simplify(sign +
+0001a410: 2066 696c 6564 6174 615b 2271 7561 6e74   filedata["quant
+0001a420: 6974 7922 5d29 2c20 6d6f 6465 3d22 706c  ity"]), mode="pl
+0001a430: 6169 6e22 290d 0a20 2020 2020 2020 2020  ain")..         
+0001a440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a450: 7562 6a65 6374 203d 2066 696c 6564 6174  ubject = filedat
+0001a460: 615b 2273 7562 6a65 6374 225d 2e72 6570  a["subject"].rep
+0001a470: 6c61 6365 2822 5f22 2c20 2220 2229 2e63  lace("_", " ").c
+0001a480: 6170 6974 616c 697a 6528 290d 0a20 2020  apitalize()..   
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2020 2020 2070 7269 6e74 2822 2020 2020       print("    
+0001a4b0: 2020 666f 756e 6422 2c71 2c73 7562 6a65    found",q,subje
+0001a4c0: 6374 290d 0a20 2020 2020 2020 2020 2020  ct)..           
+0001a4d0: 2020 2020 2020 2020 2020 2020 2074 7065               tpe
+0001a4e0: 203d 2066 696c 6564 6174 615b 7265 665f   = filedata[ref_
+0001a4f0: 696e 636f 6d65 5d0d 0a20 2020 2020 2020  income]..       
+0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a510: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
+0001a520: 5b22 5479 7065 225d 2e61 7070 656e 6428  ["Type"].append(
+0001a530: 7470 6529 0d0a 2020 2020 2020 2020 2020  tpe)..          
+0001a540: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0001a550: 6d62 696e 6564 5f69 6e63 6f6d 655b 2253  mbined_income["S
+0001a560: 7562 6a65 6374 225d 2e61 7070 656e 6428  ubject"].append(
+0001a570: 7375 626a 6563 7429 0d0a 2020 2020 2020  subject)..      
+0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a590: 2020 636f 6d62 696e 6564 5f69 6e63 6f6d    combined_incom
+0001a5a0: 655b 2251 7561 6e74 6974 7922 5d2e 6170  e["Quantity"].ap
+0001a5b0: 7065 6e64 2873 7472 2871 2929 0d0a 2020  pend(str(q))..  
+0001a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5d0: 2020 2020 2020 636f 6d62 696e 6564 5f69        combined_i
+0001a5e0: 6e63 6f6d 655b 2253 686f 7274 204e 616d  ncome["Short Nam
+0001a5f0: 6522 5d2e 6170 7065 6e64 2866 696c 6564  e"].append(filed
+0001a600: 6174 615b 2273 686f 7274 6e61 6d65 225d  ata["shortname"]
+0001a610: 2e73 7472 6970 2829 290d 0a20 2020 2020  .strip())..     
+0001a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a630: 2020 2063 6f6d 6269 6e65 645f 696e 636f     combined_inco
+0001a640: 6d65 5b22 5261 6e6b 696e 6722 5d2e 6170  me["Ranking"].ap
+0001a650: 7065 6e64 2830 290d 0a20 2020 2020 2020  pend(0)..       
+0001a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a670: 2022 2222 0d0a 2020 2020 2020 2020 2020   """..          
+0001a680: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001a690: 2074 7065 2069 6e20 5b22 4761 696e 7322   tpe in ["Gains"
+0001a6a0: 2c22 4c6f 7373 6573 222c 2245 7870 656e  ,"Losses","Expen
+0001a6b0: 7365 7322 2c22 5265 7665 6e75 6573 225d  ses","Revenues"]
+0001a6c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a6d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001a6e0: 6f6d 6269 6e65 645f 696e 636f 6d65 5b22  ombined_income["
+0001a6f0: 5261 6e6b 696e 6722 5d2e 6170 7065 6e64  Ranking"].append
+0001a700: 2830 290d 0a20 2020 2020 2020 2020 2020  (0)..           
+0001a710: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0001a720: 6620 7470 6520 696e 205b 224e 6f6e 2d4f  f tpe in ["Non-O
+0001a730: 7065 7261 7469 6f6e 616c 2049 6e63 6f6d  perational Incom
+0001a740: 6522 2c22 496e 7465 7265 7374 2050 6179  e","Interest Pay
+0001a750: 6d65 6e74 7322 5d3a 0d0a 2020 2020 2020  ments"]:..      
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a770: 2020 2020 2020 636f 6d62 696e 6564 5f69        combined_i
+0001a780: 6e63 6f6d 655b 2252 616e 6b69 6e67 225d  ncome["Ranking"]
+0001a790: 2e61 7070 656e 6428 3129 0d0a 2020 2020  .append(1)..    
+0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7b0: 2020 2020 656c 6966 2074 7065 2069 6e20      elif tpe in 
+0001a7c0: 5b22 5461 7865 7322 5d3a 0d0a 2020 2020  ["Taxes"]:..    
+0001a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7e0: 2020 2020 2020 2020 636f 6d62 696e 6564          combined
+0001a7f0: 5f69 6e63 6f6d 655b 2252 616e 6b69 6e67  _income["Ranking
+0001a800: 225d 2e61 7070 656e 6428 3229 0d0a 2020  "].append(2)..  
 0001a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a820: 2020 2020 2020 2063 6f6d 6269 6e65 645f         combined_
-0001a830: 696e 636f 6d65 5b22 5261 6e6b 696e 6722  income["Ranking"
-0001a840: 5d2e 6170 7065 6e64 2833 290d 0a20 2020  ].append(3)..   
-0001a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a860: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0001a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a880: 2020 2020 2020 2020 636f 6d62 696e 6564          combined
-0001a890: 5f69 6e63 6f6d 655b 2252 616e 6b69 6e67  _income["Ranking
-0001a8a0: 225d 2e61 7070 656e 6428 3429 0d0a 2020  "].append(4)..  
-0001a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8c0: 2020 2020 2020 2222 220d 0a0d 0a20 2020        """....   
-0001a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8e0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0001a8f0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-0001a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a910: 2073 656c 662e 6e6f 7469 6679 280d 0a20   self.notify(.. 
-0001a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a930: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
-0001a940: 6f74 2068 616e 646c 6520 7468 6520 7379  ot handle the sy
-0001a950: 6d62 6f6c 6963 2065 7870 7265 7373 696f  mbolic expressio
-0001a960: 6e20 2573 2220 2520 7369 676e 202b 2066  n %s" % sign + f
-0001a970: 696c 6564 6174 615b 2271 7561 6e74 6974  iledata["quantit
-0001a980: 7922 5d20 2b20 7374 7228 6529 2c74 6974  y"] + str(e),tit
-0001a990: 6c65 3d22 4572 726f 7222 290d 0a0d 0a20  le="Error").... 
-0001a9a0: 2020 2020 2020 2065 7863 6570 743a 0d0a         except:..
-0001a9b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001a9c0: 2e6e 6f74 6966 7928 7469 746c 653d 2245  .notify(title="E
-0001a9d0: 7272 6f72 222c 206d 6573 7361 6765 3d22  rror", message="
-0001a9e0: 416e 2065 7272 6f72 206f 6363 7572 7265  An error occurre
-0001a9f0: 642e 2229 0d0a 0d0a 2020 2020 2020 2020  d.")....        
-0001aa00: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0001aa10: 2020 7265 7375 6c74 203d 2070 642e 4461    result = pd.Da
-0001aa20: 7461 4672 616d 6528 636f 6d62 696e 6564  taFrame(combined
-0001aa30: 5f69 6e63 6f6d 6529 2e73 6574 5f69 6e64  _income).set_ind
-0001aa40: 6578 2822 5375 626a 6563 7422 290d 0a0d  ex("Subject")...
-0001aa50: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-0001aa60: 2073 6f72 7420 6166 7465 7220 7261 6e6b   sort after rank
-0001aa70: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
-0001aa80: 2072 6573 756c 7420 3d20 7265 7375 6c74   result = result
-0001aa90: 2e73 6f72 745f 7661 6c75 6573 2827 5261  .sort_values('Ra
-0001aaa0: 6e6b 696e 6727 290d 0a0d 0a20 2020 2020  nking')....     
-0001aab0: 2020 2020 2020 2023 2072 656d 6f76 6520         # remove 
-0001aac0: 7261 6e6b 696e 670d 0a20 2020 2020 2020  ranking..       
-0001aad0: 2020 2020 2072 6573 756c 7420 3d20 7265       result = re
-0001aae0: 7375 6c74 2e64 726f 7028 636f 6c75 6d6e  sult.drop(column
-0001aaf0: 733d 2022 5261 6e6b 696e 6722 290d 0a0d  s= "Ranking")...
-0001ab00: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-0001ab10: 656c 203d 2050 616e 6461 734d 6f64 656c  el = PandasModel
-0001ab20: 2872 6573 756c 7429 0d0a 0d0a 2020 2020  (result)....    
-0001ab30: 2020 2020 2020 2020 6966 206d 795f 6167          if my_ag
-0001ab40: 656e 7420 6e6f 7420 696e 2043 6173 6846  ent not in CashF
-0001ab50: 6c6f 7756 6965 7765 722e 696e 7374 616e  lowViewer.instan
-0001ab60: 6365 733a 0d0a 2020 2020 2020 2020 2020  ces:..          
-0001ab70: 2020 2020 2020 6d79 7669 6577 203d 2043        myview = C
-0001ab80: 6173 6846 6c6f 7756 6965 7765 7228 7365  ashFlowViewer(se
-0001ab90: 6c66 2c6e 616d 653d 6d79 5f61 6765 6e74  lf,name=my_agent
-0001aba0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0001abb0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0001abc0: 2020 2020 2020 6d79 7669 6577 203d 2043        myview = C
-0001abd0: 6173 6846 6c6f 7756 6965 7765 722e 696e  ashFlowViewer.in
-0001abe0: 7374 616e 6365 735b 6d79 5f61 6765 6e74  stances[my_agent
-0001abf0: 5d0d 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-0001ac00: 206d 7669 6577 2e73 6574 4765 6f6d 6574   mview.setGeomet
-0001ac10: 7279 2831 3030 2c35 3030 290d 0a20 2020  ry(100,500)..   
-0001ac20: 2020 2020 2020 2020 206d 7976 6965 772e           myview.
-0001ac30: 7365 745f 6d6f 6465 6c28 6d6f 6465 6c29  set_model(model)
-0001ac40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001ac50: 6d76 6965 772e 7765 6256 6965 772e 7365  mview.webView.se
-0001ac60: 7448 746d 6c28 6466 5f68 746d 6c29 0d0a  tHtml(df_html)..
-0001ac70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001ac80: 6f74 2073 656c 662e 7465 7374 5f6d 6f64  ot self.test_mod
-0001ac90: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001aca0: 2020 2020 6d79 7669 6577 2e73 686f 7728      myview.show(
-0001acb0: 290d 0a0d 0a20 2020 2020 2020 2065 7863  )....        exc
-0001acc0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0001acd0: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
-0001ace0: 2073 656c 662e 6e6f 7469 6679 2874 6974   self.notify(tit
-0001acf0: 6c65 3d22 4572 726f 7222 2c20 6d65 7373  le="Error", mess
-0001ad00: 6167 653d 2241 6e20 6572 726f 7220 6f63  age="An error oc
-0001ad10: 6375 7272 6564 2e22 202b 2073 7472 2865  curred." + str(e
-0001ad20: 2929 0d0a 0d0a 0d0a 2020 2020 6465 6620  ))......    def 
-0001ad30: 6765 6e5f 7465 785f 6963 7328 7365 6c66  gen_tex_ics(self
-0001ad40: 293a 0d0a 2020 2020 2020 2020 636f 6d62  ):..        comb
-0001ad50: 696e 6564 5f73 6865 6574 7320 3d20 7b7d  ined_sheets = {}
-0001ad60: 0d0a 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
-0001ad70: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-0001ad80: 2020 2020 6167 656e 745f 6e61 6d65 3a20      agent_name: 
-0001ad90: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-0001ada0: 2020 2020 2020 2022 4173 7365 7473 223a         "Assets":
-0001adb0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-0001adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001add0: 2020 2020 6173 7365 745f 6e61 6d65 203a      asset_name :
-0001ade0: 205b 656e 7472 6965 735d 2c0d 0a20 2020   [entries],..   
-0001adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae00: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-0001ae10: 7d2c 0d0a 0d0a 2020 2020 2020 2020 2020  },....          
-0001ae20: 2020 2020 2020 2020 2020 224c 6961 6269            "Liabi
-0001ae30: 6c69 7469 6573 2061 6e64 2045 7175 6974  lities and Equit
-0001ae40: 7922 3a20 7b0d 0a20 2020 2020 2020 2020  y": {..         
+0001a820: 2020 2020 2020 656c 6966 2074 7065 2069        elif tpe i
+0001a830: 6e20 5b22 4e6f 6e74 6178 6162 6c65 2050  n ["Nontaxable P
+0001a840: 726f 6669 7473 222c 2022 4e6f 6e74 6178  rofits", "Nontax
+0001a850: 6162 6c65 204c 6f73 7365 7322 5d3a 0d0a  able Losses"]:..
+0001a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a870: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
+0001a880: 696e 6564 5f69 6e63 6f6d 655b 2252 616e  ined_income["Ran
+0001a890: 6b69 6e67 225d 2e61 7070 656e 6428 3329  king"].append(3)
+0001a8a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a8b0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0001a8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a8d0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0001a8e0: 6269 6e65 645f 696e 636f 6d65 5b22 5261  bined_income["Ra
+0001a8f0: 6e6b 696e 6722 5d2e 6170 7065 6e64 2834  nking"].append(4
+0001a900: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a910: 2020 2020 2020 2020 2020 2022 2222 0d0a             """..
+0001a920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a930: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001a940: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+0001a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a960: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+0001a970: 7928 0d0a 2020 2020 2020 2020 2020 2020  y(..            
+0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a990: 2243 616e 6e6f 7420 6861 6e64 6c65 2074  "Cannot handle t
+0001a9a0: 6865 2073 796d 626f 6c69 6320 6578 7072  he symbolic expr
+0001a9b0: 6573 7369 6f6e 2025 7322 2025 2073 6967  ession %s" % sig
+0001a9c0: 6e20 2b20 6669 6c65 6461 7461 5b22 7175  n + filedata["qu
+0001a9d0: 616e 7469 7479 225d 202b 2073 7472 2865  antity"] + str(e
+0001a9e0: 292c 7469 746c 653d 2245 7272 6f72 2229  ),title="Error")
+0001a9f0: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
+0001aa00: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
+0001aa10: 2073 656c 662e 6e6f 7469 6679 2874 6974   self.notify(tit
+0001aa20: 6c65 3d22 4572 726f 7222 2c20 6d65 7373  le="Error", mess
+0001aa30: 6167 653d 2241 6e20 6572 726f 7220 6f63  age="An error oc
+0001aa40: 6375 7272 6564 2e22 290d 0a0d 0a20 2020  curred.")....   
+0001aa50: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+0001aa60: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0001aa70: 7064 2e44 6174 6146 7261 6d65 2863 6f6d  pd.DataFrame(com
+0001aa80: 6269 6e65 645f 696e 636f 6d65 292e 7365  bined_income).se
+0001aa90: 745f 696e 6465 7828 2253 7562 6a65 6374  t_index("Subject
+0001aaa0: 2229 0d0a 0d0a 0d0a 2020 2020 2020 2020  ")......        
+0001aab0: 2020 2020 2320 736f 7274 2061 6674 6572      # sort after
+0001aac0: 2072 616e 6b69 6e67 0d0a 2020 2020 2020   ranking..      
+0001aad0: 2020 2020 2020 7265 7375 6c74 203d 2072        result = r
+0001aae0: 6573 756c 742e 736f 7274 5f76 616c 7565  esult.sort_value
+0001aaf0: 7328 2752 616e 6b69 6e67 2729 0d0a 0d0a  s('Ranking')....
+0001ab00: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+0001ab10: 6d6f 7665 2072 616e 6b69 6e67 0d0a 2020  move ranking..  
+0001ab20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0001ab30: 203d 2072 6573 756c 742e 6472 6f70 2863   = result.drop(c
+0001ab40: 6f6c 756d 6e73 3d20 2252 616e 6b69 6e67  olumns= "Ranking
+0001ab50: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
+0001ab60: 2020 6d6f 6465 6c20 3d20 5061 6e64 6173    model = Pandas
+0001ab70: 4d6f 6465 6c28 7265 7375 6c74 290d 0a0d  Model(result)...
+0001ab80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001ab90: 6d79 5f61 6765 6e74 206e 6f74 2069 6e20  my_agent not in 
+0001aba0: 4361 7368 466c 6f77 5669 6577 6572 2e69  CashFlowViewer.i
+0001abb0: 6e73 7461 6e63 6573 3a0d 0a20 2020 2020  nstances:..     
+0001abc0: 2020 2020 2020 2020 2020 206d 7976 6965             myvie
+0001abd0: 7720 3d20 4361 7368 466c 6f77 5669 6577  w = CashFlowView
+0001abe0: 6572 2873 656c 662c 6e61 6d65 3d6d 795f  er(self,name=my_
+0001abf0: 6167 656e 7429 0d0a 2020 2020 2020 2020  agent)..        
+0001ac00: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001ac10: 2020 2020 2020 2020 2020 206d 7976 6965             myvie
+0001ac20: 7720 3d20 4361 7368 466c 6f77 5669 6577  w = CashFlowView
+0001ac30: 6572 2e69 6e73 7461 6e63 6573 5b6d 795f  er.instances[my_
+0001ac40: 6167 656e 745d 0d0a 2020 2020 2020 2020  agent]..        
+0001ac50: 2020 2020 2320 6d76 6965 772e 7365 7447      # mview.setG
+0001ac60: 656f 6d65 7472 7928 3130 302c 3530 3029  eometry(100,500)
+0001ac70: 0d0a 2020 2020 2020 2020 2020 2020 6d79  ..            my
+0001ac80: 7669 6577 2e73 6574 5f6d 6f64 656c 286d  view.set_model(m
+0001ac90: 6f64 656c 290d 0a20 2020 2020 2020 2020  odel)..         
+0001aca0: 2020 2023 206d 7669 6577 2e77 6562 5669     # mview.webVi
+0001acb0: 6577 2e73 6574 4874 6d6c 2864 665f 6874  ew.setHtml(df_ht
+0001acc0: 6d6c 290d 0a20 2020 2020 2020 2020 2020  ml)..           
+0001acd0: 2069 6620 6e6f 7420 7365 6c66 2e74 6573   if not self.tes
+0001ace0: 745f 6d6f 6465 3a0d 0a20 2020 2020 2020  t_mode:..       
+0001acf0: 2020 2020 2020 2020 206d 7976 6965 772e           myview.
+0001ad00: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
+0001ad10: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0001ad20: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+0001ad30: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+0001ad40: 7928 7469 746c 653d 2245 7272 6f72 222c  y(title="Error",
+0001ad50: 206d 6573 7361 6765 3d22 416e 2065 7272   message="An err
+0001ad60: 6f72 206f 6363 7572 7265 642e 2220 2b20  or occurred." + 
+0001ad70: 7374 7228 6529 290d 0a0d 0a0d 0a20 2020  str(e))......   
+0001ad80: 2064 6566 2067 656e 5f74 6578 5f69 6373   def gen_tex_ics
+0001ad90: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+0001ada0: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001adb0: 203d 207b 7d0d 0a0d 0a20 2020 2020 2020   = {}....       
+0001adc0: 2022 2222 0d0a 2020 2020 2020 2020 7b0d   """..        {.
+0001add0: 0a20 2020 2020 2020 2061 6765 6e74 5f6e  .        agent_n
+0001ade0: 616d 653a 207b 0d0a 2020 2020 2020 2020  ame: {..        
+0001adf0: 2020 2020 2020 2020 2020 2020 2241 7373              "Ass
+0001ae00: 6574 7322 3a20 7b0d 0a20 2020 2020 2020  ets": {..       
+0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae20: 2020 2020 2020 2020 2061 7373 6574 5f6e           asset_n
+0001ae30: 616d 6520 3a20 5b65 6e74 7269 6573 5d2c  ame : [entries],
+0001ae40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae60: 2020 2020 2020 206e 616d 6520 3a20 5b65         name : [e
-0001ae70: 6e74 7269 6573 5d2c 0d0a 2020 2020 2020  ntries],..      
-0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae90: 2020 2020 2020 2020 2020 2e2e 2e7d 2c0d            ...},.
-0001aea0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001aeb0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-0001aec0: 2020 7d0d 0a20 2020 2020 2020 2022 2222    }..        """
-0001aed0: 0d0a 0d0a 2020 2020 2020 2020 636f 6d62  ....        comb
-0001aee0: 696e 6564 5f69 6e63 6f6d 6520 3d20 6465  ined_income = de
-0001aef0: 6661 756c 7464 6963 7428 6c61 6d62 6461  faultdict(lambda
-0001af00: 3a20 7b22 4761 696e 7322 3a20 5b5d 2c20  : {"Gains": [], 
-0001af10: 224c 6f73 7365 7322 3a20 5b5d 2c20 2252  "Losses": [], "R
-0001af20: 6576 656e 7565 7322 3a20 5b5d 2c20 2254  evenues": [], "T
-0001af30: 6178 6573 223a 205b 5d2c 2022 4578 7065  axes": [], "Expe
-0001af40: 6e73 6573 223a 205b 5d2c 0d0a 2020 2020  nses": [],..    
-0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af70: 2020 2020 2020 2020 2020 2022 4e6f 6e74             "Nont
-0001af80: 6178 6162 6c65 204c 6f73 7365 7322 3a20  axable Losses": 
-0001af90: 5b5d 2c20 224e 6f6e 7461 7861 626c 6520  [], "Nontaxable 
-0001afa0: 5072 6f66 6974 7322 3a20 5b5d 2c0d 0a20  Profits": [],.. 
+0001ae60: 2020 2e2e 2e7d 2c0d 0a0d 0a20 2020 2020    ...},....     
+0001ae70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001ae80: 4c69 6162 696c 6974 6965 7320 616e 6420  Liabilities and 
+0001ae90: 4571 7569 7479 223a 207b 0d0a 2020 2020  Equity": {..    
+0001aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aeb0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0001aec0: 203a 205b 656e 7472 6965 735d 2c0d 0a20   : [entries],.. 
+0001aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aee0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+0001aef0: 2e2e 7d2c 0d0a 0d0a 2020 2020 2020 2020  ..},....        
+0001af00: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+0001af10: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+0001af20: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+0001af30: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
+0001af40: 203d 2064 6566 6175 6c74 6469 6374 286c   = defaultdict(l
+0001af50: 616d 6264 613a 207b 2247 6169 6e73 223a  ambda: {"Gains":
+0001af60: 205b 5d2c 2022 4c6f 7373 6573 223a 205b   [], "Losses": [
+0001af70: 5d2c 2022 5265 7665 6e75 6573 223a 205b  ], "Revenues": [
+0001af80: 5d2c 2022 5461 7865 7322 3a20 5b5d 2c20  ], "Taxes": [], 
+0001af90: 2245 7870 656e 7365 7322 3a20 5b5d 2c0d  "Expenses": [],.
+0001afa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 224e                "N
-0001afe0: 6f6e 2d4f 7065 7261 7469 6f6e 616c 2049  on-Operational I
-0001aff0: 6e63 6f6d 6522 3a20 5b5d 2c0d 0a20 2020  ncome": [],..   
-0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afd0: 224e 6f6e 7461 7861 626c 6520 4c6f 7373  "Nontaxable Loss
+0001afe0: 6573 223a 205b 5d2c 2022 4e6f 6e74 6178  es": [], "Nontax
+0001aff0: 6162 6c65 2050 726f 6669 7473 223a 205b  able Profits": [
+0001b000: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
 0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b020: 2020 2020 2020 2020 2020 2020 2249 6e74              "Int
-0001b030: 6572 6573 7420 5061 796d 656e 7473 223a  erest Payments":
-0001b040: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0001b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b030: 2020 2022 4e6f 6e2d 4f70 6572 6174 696f     "Non-Operatio
+0001b040: 6e61 6c20 496e 636f 6d65 223a 205b 5d2c  nal Income": [],
+0001b050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b070: 2020 2020 7d29 0d0a 0d0a 2020 2020 2020      })....      
-0001b080: 2020 2222 220d 0a20 2020 2020 2020 207b    """..        {
-0001b090: 0d0a 2020 2020 2020 2020 6167 656e 745f  ..        agent_
-0001b0a0: 6e61 6d65 3a20 7b0d 0a20 2020 2020 2020  name: {..       
-0001b0b0: 2020 2020 2020 2020 2022 4761 696e 7322           "Gains"
-0001b0c0: 3a20 205b 656e 7472 6965 735d 2c0d 0a20  :  [entries],.. 
-0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001b0e0: 4c6f 7373 6573 223a 5b65 6e74 7269 6573  Losses":[entries
-0001b0f0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001b100: 2020 2020 2245 7870 656e 6469 7475 7265      "Expenditure
-0001b110: 7322 3a5b 656e 7472 6965 735d 2c0d 0a20  s":[entries],.. 
-0001b120: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001b130: 5265 7665 6e75 6573 223a 205b 656e 7472  Revenues": [entr
-0001b140: 6965 735d 2c0d 0a20 2020 2020 2020 2020  ies],..         
-0001b150: 2020 2020 2020 2022 5461 7865 7322 3a5b         "Taxes":[
-0001b160: 656e 7472 6965 735d 0d0a 2020 2020 2020  entries]..      
-0001b170: 2020 7d0d 0a20 2020 2020 2020 2022 2222    }..        """
-0001b180: 0d0a 0d0a 2020 2020 2020 2020 6b20 3d20  ....        k = 
-0001b190: 300d 0a20 2020 2020 2020 2074 6578 7374  0..        texst
-0001b1a0: 7220 3d20 2222 0d0a 0d0a 2020 2020 2020  r = ""....      
-0001b1b0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-0001b1c0: 2020 2020 666f 7220 6669 6c65 6461 7461      for filedata
-0001b1d0: 2069 6e20 7365 6c66 2e65 6e74 7279 5f64   in self.entry_d
-0001b1e0: 6174 613a 0d0a 2020 2020 2020 2020 2020  ata:..          
-0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b200: 2020 2320 2020 7365 6c66 2e70 6172 656e    #   self.paren
-0001b210: 742e 6167 656e 7431 2e76 616c 7565 203d  t.agent1.value =
-0001b220: 2066 696c 6564 6174 615b 2261 6765 6e74   filedata["agent
-0001b230: 3122 5d0d 0a20 2020 2020 2020 2020 2020  1"]..           
+0001b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b080: 2022 496e 7465 7265 7374 2050 6179 6d65   "Interest Payme
+0001b090: 6e74 7322 3a20 5b5d 0d0a 2020 2020 2020  nts": []..      
+0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0c0: 2020 2020 2020 2020 207d 290d 0a0d 0a20           }).... 
+0001b0d0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0001b0e0: 2020 2020 7b0d 0a20 2020 2020 2020 2061      {..        a
+0001b0f0: 6765 6e74 5f6e 616d 653a 207b 0d0a 2020  gent_name: {..  
+0001b100: 2020 2020 2020 2020 2020 2020 2020 2247                "G
+0001b110: 6169 6e73 223a 2020 5b65 6e74 7269 6573  ains":  [entries
+0001b120: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001b130: 2020 2020 224c 6f73 7365 7322 3a5b 656e      "Losses":[en
+0001b140: 7472 6965 735d 2c0d 0a20 2020 2020 2020  tries],..       
+0001b150: 2020 2020 2020 2020 2022 4578 7065 6e64           "Expend
+0001b160: 6974 7572 6573 223a 5b65 6e74 7269 6573  itures":[entries
+0001b170: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001b180: 2020 2020 2252 6576 656e 7565 7322 3a20      "Revenues": 
+0001b190: 5b65 6e74 7269 6573 5d2c 0d0a 2020 2020  [entries],..    
+0001b1a0: 2020 2020 2020 2020 2020 2020 2254 6178              "Tax
+0001b1b0: 6573 223a 5b65 6e74 7269 6573 5d0d 0a20  es":[entries].. 
+0001b1c0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+0001b1d0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+0001b1e0: 206b 203d 2030 0d0a 2020 2020 2020 2020   k = 0..        
+0001b1f0: 7465 7873 7472 203d 2022 220d 0a0d 0a20  texstr = "".... 
+0001b200: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+0001b210: 2020 2020 2020 2020 2066 6f72 2066 696c           for fil
+0001b220: 6564 6174 6120 696e 2073 656c 662e 656e  edata in self.en
+0001b230: 7472 795f 6461 7461 3a0d 0a20 2020 2020  try_data:..     
 0001b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b250: 2023 2073 656c 662e 7061 7265 6e74 2e61   # self.parent.a
-0001b260: 6765 6e74 322e 7661 6c75 6520 3d20 6669  gent2.value = fi
-0001b270: 6c65 6461 7461 5b22 6167 656e 7432 225d  ledata["agent2"]
-0001b280: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001b250: 2020 2020 2020 2023 2020 2073 656c 662e         #   self.
+0001b260: 7061 7265 6e74 2e61 6765 6e74 312e 7661  parent.agent1.va
+0001b270: 6c75 6520 3d20 6669 6c65 6461 7461 5b22  lue = filedata["
+0001b280: 6167 656e 7431 225d 0d0a 2020 2020 2020  agent1"]..      
 0001b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2a0: 2320 7365 6c66 2e70 6172 656e 742e 666c  # self.parent.fl
-0001b2b0: 6f77 5f63 6865 636b 2e76 616c 7565 203d  ow_check.value =
-0001b2c0: 2073 7472 2862 6f6f 6c28 6669 6c65 6461   str(bool(fileda
-0001b2d0: 7461 5b22 6c6f 6720 7472 616e 7361 6374  ta["log transact
-0001b2e0: 696f 6e22 5d29 290d 0a20 2020 2020 2020  ion"]))..       
-0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b300: 2020 2020 2023 2073 656c 662e 7061 7265       # self.pare
-0001b310: 6e74 2e6b 696e 642e 7661 6c75 6520 3d20  nt.kind.value = 
-0001b320: 6669 6c65 6461 7461 5b22 6b69 6e64 225d  filedata["kind"]
-0001b330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b340: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001b350: 7365 6c66 2e70 6172 656e 742e 7375 626a  self.parent.subj
-0001b360: 6563 742e 7661 6c75 6520 3d20 6669 6c65  ect.value = file
-0001b370: 6461 7461 5b22 7375 626a 6563 7422 5d0d  data["subject"].
-0001b380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b390: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0001b3a0: 656c 662e 7061 7265 6e74 2e71 7561 6e74  elf.parent.quant
-0001b3b0: 6974 792e 7661 6c75 6520 3d20 6669 6c65  ity.value = file
-0001b3c0: 6461 7461 5b22 7175 616e 7469 7479 225d  data["quantity"]
-0001b3d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001b2a0: 2020 2020 2020 2320 7365 6c66 2e70 6172        # self.par
+0001b2b0: 656e 742e 6167 656e 7432 2e76 616c 7565  ent.agent2.value
+0001b2c0: 203d 2066 696c 6564 6174 615b 2261 6765   = filedata["age
+0001b2d0: 6e74 3222 5d0d 0a0d 0a20 2020 2020 2020  nt2"]....       
+0001b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b2f0: 2020 2020 2023 2073 656c 662e 7061 7265       # self.pare
+0001b300: 6e74 2e66 6c6f 775f 6368 6563 6b2e 7661  nt.flow_check.va
+0001b310: 6c75 6520 3d20 7374 7228 626f 6f6c 2866  lue = str(bool(f
+0001b320: 696c 6564 6174 615b 226c 6f67 2074 7261  iledata["log tra
+0001b330: 6e73 6163 7469 6f6e 225d 2929 0d0a 2020  nsaction"]))..  
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0001b360: 2e70 6172 656e 742e 6b69 6e64 2e76 616c  .parent.kind.val
+0001b370: 7565 203d 2066 696c 6564 6174 615b 226b  ue = filedata["k
+0001b380: 696e 6422 5d0d 0a20 2020 2020 2020 2020  ind"]..         
+0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3a0: 2020 2023 2073 656c 662e 7061 7265 6e74     # self.parent
+0001b3b0: 2e73 7562 6a65 6374 2e76 616c 7565 203d  .subject.value =
+0001b3c0: 2066 696c 6564 6174 615b 2273 7562 6a65   filedata["subje
+0001b3d0: 6374 225d 0d0a 2020 2020 2020 2020 2020  ct"]..          
 0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3f0: 6167 656e 7431 203d 2066 696c 6564 6174  agent1 = filedat
-0001b400: 615b 2261 6765 6e74 3122 5d0d 0a20 2020  a["agent1"]..   
-0001b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b420: 2020 2020 2020 2020 2061 6765 6e74 3220           agent2 
-0001b430: 3d20 6669 6c65 6461 7461 5b22 6167 656e  = filedata["agen
-0001b440: 7432 225d 0d0a 0d0a 2020 2020 2020 2020  t2"]....        
-0001b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b460: 2020 2020 6173 7365 7473 3120 3d20 6669      assets1 = fi
-0001b470: 6c65 6461 7461 5b22 6131 225d 202b 2022  ledata["a1"] + "
-0001b480: 5c6e 220d 0a20 2020 2020 2020 2020 2020  \n"..           
-0001b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4a0: 206c 6961 6273 3120 3d20 6669 6c65 6461   liabs1 = fileda
-0001b4b0: 7461 5b22 6c31 225d 202b 2022 5c6e 2220  ta["l1"] + "\n" 
-0001b4c0: 2b20 6669 6c65 6461 7461 5b22 6531 225d  + filedata["e1"]
-0001b4d0: 202b 2022 5c6e 220d 0a0d 0a20 2020 2020   + "\n"....     
+0001b3f0: 2020 2320 7365 6c66 2e70 6172 656e 742e    # self.parent.
+0001b400: 7175 616e 7469 7479 2e76 616c 7565 203d  quantity.value =
+0001b410: 2066 696c 6564 6174 615b 2271 7561 6e74   filedata["quant
+0001b420: 6974 7922 5d0d 0a0d 0a20 2020 2020 2020  ity"]....       
+0001b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b440: 2020 2020 2061 6765 6e74 3120 3d20 6669       agent1 = fi
+0001b450: 6c65 6461 7461 5b22 6167 656e 7431 225d  ledata["agent1"]
+0001b460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b470: 2020 2020 2020 2020 2020 2020 2020 6167                ag
+0001b480: 656e 7432 203d 2066 696c 6564 6174 615b  ent2 = filedata[
+0001b490: 2261 6765 6e74 3222 5d0d 0a0d 0a20 2020  "agent2"]....   
+0001b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4b0: 2020 2020 2020 2020 2061 7373 6574 7331           assets1
+0001b4c0: 203d 2066 696c 6564 6174 615b 2261 3122   = filedata["a1"
+0001b4d0: 5d20 2b20 225c 6e22 0d0a 2020 2020 2020  ] + "\n"..      
 0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4f0: 2020 2020 2020 2061 7373 6574 7332 203d         assets2 =
-0001b500: 2066 696c 6564 6174 615b 2261 3222 5d20   filedata["a2"] 
-0001b510: 2b20 225c 6e22 0d0a 2020 2020 2020 2020  + "\n"..        
-0001b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b530: 2020 2020 6c69 6162 7332 203d 2066 696c      liabs2 = fil
-0001b540: 6564 6174 615b 226c 3222 5d20 2b20 225c  edata["l2"] + "\
-0001b550: 6e22 202b 2066 696c 6564 6174 615b 2265  n" + filedata["e
-0001b560: 3222 5d20 2b20 225c 6e22 0d0a 0d0a 2020  2"] + "\n"....  
+0001b4f0: 2020 2020 2020 6c69 6162 7331 203d 2066        liabs1 = f
+0001b500: 696c 6564 6174 615b 226c 3122 5d20 2b20  iledata["l1"] + 
+0001b510: 225c 6e22 202b 2066 696c 6564 6174 615b  "\n" + filedata[
+0001b520: 2265 3122 5d20 2b20 225c 6e22 0d0a 0d0a  "e1"] + "\n"....
+0001b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b540: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0001b550: 7473 3220 3d20 6669 6c65 6461 7461 5b22  ts2 = filedata["
+0001b560: 6132 225d 202b 2022 5c6e 220d 0a20 2020  a2"] + "\n"..   
 0001b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b580: 2020 2020 2020 2020 2020 6d79 5f74 6162            my_tab
-0001b590: 6c65 203d 2070 642e 4461 7461 4672 616d  le = pd.DataFram
-0001b5a0: 652e 6672 6f6d 5f64 6963 7428 0d0a 2020  e.from_dict(..  
-0001b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b5c0: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
-0001b5d0: 4173 7365 7473 223a 2061 7373 6574 7331  Assets": assets1
-0001b5e0: 2e73 706c 6974 2822 5c6e 2229 2c20 224c  .split("\n"), "L
-0001b5f0: 6961 6269 6c69 7469 6573 2061 6e64 2045  iabilities and E
-0001b600: 7175 6974 7922 3a20 6c69 6162 7331 2e73  quity": liabs1.s
-0001b610: 706c 6974 2822 5c6e 2229 7d2c 0d0a 2020  plit("\n")},..  
-0001b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b630: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-0001b640: 6965 6e74 3d27 696e 6465 7827 292e 540d  ient='index').T.
-0001b650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b660: 2020 2020 2020 2020 2020 2020 206d 795f               my_
-0001b670: 7461 626c 6532 203d 2070 642e 4461 7461  table2 = pd.Data
-0001b680: 4672 616d 652e 6672 6f6d 5f64 6963 7428  Frame.from_dict(
-0001b690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b6b0: 2020 7b22 4173 7365 7473 223a 2061 7373    {"Assets": ass
-0001b6c0: 6574 7332 2e73 706c 6974 2822 5c6e 2229  ets2.split("\n")
-0001b6d0: 2c20 224c 6961 6269 6c69 7469 6573 2061  , "Liabilities a
-0001b6e0: 6e64 2045 7175 6974 7922 3a20 6c69 6162  nd Equity": liab
-0001b6f0: 7332 2e73 706c 6974 2822 5c6e 2229 7d2c  s2.split("\n")},
-0001b700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b720: 2020 6f72 6965 6e74 3d27 696e 6465 7827    orient='index'
-0001b730: 292e 540d 0a0d 0a20 2020 2020 2020 2020  ).T....         
-0001b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b750: 2020 2074 6578 5f74 6162 6c65 3120 3d20     tex_table1 = 
-0001b760: 6d79 5f74 6162 6c65 2e74 6f5f 6c61 7465  my_table.to_late
-0001b770: 7828 696e 6465 785f 6e61 6d65 733d 4661  x(index_names=Fa
-0001b780: 6c73 652c 2069 6e64 6578 3d46 616c 7365  lse, index=False
-0001b790: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001b7a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001b7b0: 6578 5f74 6162 6c65 3220 3d20 6d79 5f74  ex_table2 = my_t
-0001b7c0: 6162 6c65 322e 746f 5f6c 6174 6578 2869  able2.to_latex(i
-0001b7d0: 6e64 6578 5f6e 616d 6573 3d46 616c 7365  ndex_names=False
-0001b7e0: 2c20 696e 6465 783d 4661 6c73 6529 0d0a  , index=False)..
-0001b7f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b800: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001b810: 6d65 7267 655f 7461 626c 6520 3d20 7064  merge_table = pd
-0001b820: 2e63 6f6e 6361 7428 7465 785f 7461 626c  .concat(tex_tabl
-0001b830: 6531 2c74 6578 5f74 6162 6c65 3229 0d0a  e1,tex_table2)..
-0001b840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b850: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001b860: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001b870: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 206d 6f64  ============ mod
-0001b880: 6966 7920 636f 6d62 696e 6564 2073 6865  ify combined she
-0001b890: 6574 0d0a 0d0a 2020 2020 2020 2020 2020  et....          
+0001b580: 2020 2020 2020 2020 206c 6961 6273 3220           liabs2 
+0001b590: 3d20 6669 6c65 6461 7461 5b22 6c32 225d  = filedata["l2"]
+0001b5a0: 202b 2022 5c6e 2220 2b20 6669 6c65 6461   + "\n" + fileda
+0001b5b0: 7461 5b22 6532 225d 202b 2022 5c6e 220d  ta["e2"] + "\n".
+0001b5c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b5d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001b5e0: 795f 7461 626c 6520 3d20 7064 2e44 6174  y_table = pd.Dat
+0001b5f0: 6146 7261 6d65 2e66 726f 6d5f 6469 6374  aFrame.from_dict
+0001b600: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b620: 2020 207b 2241 7373 6574 7322 3a20 6173     {"Assets": as
+0001b630: 7365 7473 312e 7370 6c69 7428 225c 6e22  sets1.split("\n"
+0001b640: 292c 2022 4c69 6162 696c 6974 6965 7320  ), "Liabilities 
+0001b650: 616e 6420 4571 7569 7479 223a 206c 6961  and Equity": lia
+0001b660: 6273 312e 7370 6c69 7428 225c 6e22 297d  bs1.split("\n")}
+0001b670: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b690: 2020 206f 7269 656e 743d 2769 6e64 6578     orient='index
+0001b6a0: 2729 2e54 0d0a 2020 2020 2020 2020 2020  ').T..          
+0001b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b6c0: 2020 6d79 5f74 6162 6c65 3220 3d20 7064    my_table2 = pd
+0001b6d0: 2e44 6174 6146 7261 6d65 2e66 726f 6d5f  .DataFrame.from_
+0001b6e0: 6469 6374 280d 0a20 2020 2020 2020 2020  dict(..         
+0001b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b700: 2020 2020 2020 207b 2241 7373 6574 7322         {"Assets"
+0001b710: 3a20 6173 7365 7473 322e 7370 6c69 7428  : assets2.split(
+0001b720: 225c 6e22 292c 2022 4c69 6162 696c 6974  "\n"), "Liabilit
+0001b730: 6965 7320 616e 6420 4571 7569 7479 223a  ies and Equity":
+0001b740: 206c 6961 6273 322e 7370 6c69 7428 225c   liabs2.split("\
+0001b750: 6e22 297d 2c0d 0a20 2020 2020 2020 2020  n")},..         
+0001b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b770: 2020 2020 2020 206f 7269 656e 743d 2769         orient='i
+0001b780: 6e64 6578 2729 2e54 0d0a 0d0a 2020 2020  ndex').T....    
+0001b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7a0: 2020 2020 2020 2020 7465 785f 7461 626c          tex_tabl
+0001b7b0: 6531 203d 206d 795f 7461 626c 652e 746f  e1 = my_table.to
+0001b7c0: 5f6c 6174 6578 2869 6e64 6578 5f6e 616d  _latex(index_nam
+0001b7d0: 6573 3d46 616c 7365 2c20 696e 6465 783d  es=False, index=
+0001b7e0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+0001b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b800: 2020 2020 7465 785f 7461 626c 6532 203d      tex_table2 =
+0001b810: 206d 795f 7461 626c 6532 2e74 6f5f 6c61   my_table2.to_la
+0001b820: 7465 7828 696e 6465 785f 6e61 6d65 733d  tex(index_names=
+0001b830: 4661 6c73 652c 2069 6e64 6578 3d46 616c  False, index=Fal
+0001b840: 7365 290d 0a0d 0a20 2020 2020 2020 2020  se)....         
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b860: 2020 2023 206d 6572 6765 5f74 6162 6c65     # merge_table
+0001b870: 203d 2070 642e 636f 6e63 6174 2874 6578   = pd.concat(tex
+0001b880: 5f74 6162 6c65 312c 7465 785f 7461 626c  _table1,tex_tabl
+0001b890: 6532 290d 0a0d 0a20 2020 2020 2020 2020  e2)....         
 0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8b0: 2020 230d 0a20 2020 2020 2020 2020 2020    #..           
-0001b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8d0: 2023 2041 4745 4e54 2031 0d0a 2020 2020   # AGENT 1..    
-0001b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8f0: 2020 2020 2020 2020 230d 0a0d 0a20 2020          #....   
-0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 2020 2069 6620 6167 656e           if agen
-0001b920: 7431 206e 6f74 2069 6e20 636f 6d62 696e  t1 not in combin
-0001b930: 6564 5f73 6865 6574 733a 0d0a 2020 2020  ed_sheets:..    
-0001b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b950: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-0001b960: 696e 6564 5f73 6865 6574 735b 6167 656e  ined_sheets[agen
-0001b970: 7431 5d20 3d20 7b7d 0d0a 0d0a 2020 2020  t1] = {}....    
-0001b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b990: 2020 2020 2020 2020 6966 2022 4173 7365          if "Asse
-0001b9a0: 7473 2220 6e6f 7420 696e 2063 6f6d 6269  ts" not in combi
-0001b9b0: 6e65 645f 7368 6565 7473 5b61 6765 6e74  ned_sheets[agent
-0001b9c0: 315d 3a0d 0a20 2020 2020 2020 2020 2020  1]:..           
-0001b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9e0: 2020 2020 2063 6f6d 6269 6e65 645f 7368       combined_sh
-0001b9f0: 6565 7473 5b61 6765 6e74 315d 5b22 4173  eets[agent1]["As
-0001ba00: 7365 7473 225d 203d 207b 7d0d 0a20 2020  sets"] = {}..   
-0001ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba20: 2020 2020 2020 2020 2069 6620 224c 6961           if "Lia
-0001ba30: 6269 6c69 7469 6573 2061 6e64 2045 7175  bilities and Equ
-0001ba40: 6974 7922 206e 6f74 2069 6e20 636f 6d62  ity" not in comb
-0001ba50: 696e 6564 5f73 6865 6574 735b 6167 656e  ined_sheets[agen
-0001ba60: 7431 5d3a 0d0a 2020 2020 2020 2020 2020  t1]:..          
-0001ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba80: 2020 2020 2020 636f 6d62 696e 6564 5f73        combined_s
-0001ba90: 6865 6574 735b 6167 656e 7431 5d5b 224c  heets[agent1]["L
-0001baa0: 6961 6269 6c69 7469 6573 2061 6e64 2045  iabilities and E
-0001bab0: 7175 6974 7922 5d20 3d20 7b7d 0d0a 0d0a  quity"] = {}....
+0001b8b0: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
+0001b8c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001b8d0: 3d20 6d6f 6469 6679 2063 6f6d 6269 6e65  = modify combine
+0001b8e0: 6420 7368 6565 740d 0a0d 0a20 2020 2020  d sheet....     
+0001b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b900: 2020 2020 2020 2023 0d0a 2020 2020 2020         #..      
+0001b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b920: 2020 2020 2020 2320 4147 454e 5420 310d        # AGENT 1.
+0001b930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b940: 2020 2020 2020 2020 2020 2020 2023 0d0a               #..
+0001b950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b960: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b970: 2061 6765 6e74 3120 6e6f 7420 696e 2063   agent1 not in c
+0001b980: 6f6d 6269 6e65 645f 7368 6565 7473 3a0d  ombined_sheets:.
+0001b990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9b0: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001b9c0: 5b61 6765 6e74 315d 203d 207b 7d0d 0a0d  [agent1] = {}...
+0001b9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b9e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001b9f0: 2241 7373 6574 7322 206e 6f74 2069 6e20  "Assets" not in 
+0001ba00: 636f 6d62 696e 6564 5f73 6865 6574 735b  combined_sheets[
+0001ba10: 6167 656e 7431 5d3a 0d0a 2020 2020 2020  agent1]:..      
+0001ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba30: 2020 2020 2020 2020 2020 636f 6d62 696e            combin
+0001ba40: 6564 5f73 6865 6574 735b 6167 656e 7431  ed_sheets[agent1
+0001ba50: 5d5b 2241 7373 6574 7322 5d20 3d20 7b7d  ]["Assets"] = {}
+0001ba60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ba70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001ba80: 2022 4c69 6162 696c 6974 6965 7320 616e   "Liabilities an
+0001ba90: 6420 4571 7569 7479 2220 6e6f 7420 696e  d Equity" not in
+0001baa0: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001bab0: 5b61 6765 6e74 315d 3a0d 0a20 2020 2020  [agent1]:..     
 0001bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bad0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001bae0: 6368 616e 6765 2069 6e20 6173 7365 7473  change in assets
-0001baf0: 312e 7370 6c69 7428 225c 6e22 293a 0d0a  1.split("\n"):..
-0001bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb20: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0001bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb40: 2020 2020 2020 2020 2020 7369 676e 203d            sign =
-0001bb50: 2063 6861 6e67 655b 305d 2020 2320 6669   change[0]  # fi
-0001bb60: 7273 7420 6c65 7474 6572 2069 7320 7369  rst letter is si
-0001bb70: 676e 202b 206f 7220 2d0d 0a0d 0a20 2020  gn + or -....   
+0001bad0: 2020 2020 2020 2020 2020 2063 6f6d 6269             combi
+0001bae0: 6e65 645f 7368 6565 7473 5b61 6765 6e74  ned_sheets[agent
+0001baf0: 315d 5b22 4c69 6162 696c 6974 6965 7320  1]["Liabilities 
+0001bb00: 616e 6420 4571 7569 7479 225d 203d 207b  and Equity"] = {
+0001bb10: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
+0001bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb30: 2066 6f72 2063 6861 6e67 6520 696e 2061   for change in a
+0001bb40: 7373 6574 7331 2e73 706c 6974 2822 5c6e  ssets1.split("\n
+0001bb50: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+0001bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb70: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
 0001bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bba0: 206e 616d 6520 3d20 6368 616e 6765 5b31   name = change[1
-0001bbb0: 3a5d 2e73 7472 6970 2829 0d0a 2020 2020  :].strip()..    
-0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbe0: 7120 3d20 7379 6d70 792e 6c61 7465 7828  q = sympy.latex(
-0001bbf0: 7379 6d70 792e 7369 6d70 6c69 6679 2873  sympy.simplify(s
-0001bc00: 6967 6e20 2b20 6669 6c65 6461 7461 5b22  ign + filedata["
-0001bc10: 7175 616e 7469 7479 225d 292c 206d 6f64  quantity"]), mod
-0001bc20: 653d 2269 6e6c 696e 6522 290d 0a20 2020  e="inline")..   
-0001bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc50: 2073 7562 6a65 6374 203d 2022 2020 2028   subject = "   (
-0001bc60: 2220 2b20 6669 6c65 6461 7461 5b22 7375  " + filedata["su
-0001bc70: 626a 6563 7422 5d2e 7265 706c 6163 6528  bject"].replace(
-0001bc80: 225f 222c 2022 2022 2920 2b20 2229 220d  "_", " ") + ")".
-0001bc90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcb0: 2020 2020 2020 2023 7072 696e 7428 226e         #print("n
-0001bcc0: 616d 6522 2c20 6e61 6d65 290d 0a20 2020  ame", name)..   
-0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcf0: 2023 7072 696e 7428 2263 6f6d 6269 6e65   #print("combine
-0001bd00: 645f 7368 6565 7473 5b61 6765 6e74 315d  d_sheets[agent1]
-0001bd10: 222c 2063 6f6d 6269 6e65 645f 7368 6565  ", combined_shee
-0001bd20: 7473 5b61 6765 6e74 315d 290d 0a20 2020  ts[agent1])..   
+0001bb90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001bba0: 6967 6e20 3d20 6368 616e 6765 5b30 5d20  ign = change[0] 
+0001bbb0: 2023 2066 6972 7374 206c 6574 7465 7220   # first letter 
+0001bbc0: 6973 2073 6967 6e20 2b20 6f72 202d 0d0a  is sign + or -..
+0001bbd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbf0: 2020 2020 2020 6e61 6d65 203d 2063 6861        name = cha
+0001bc00: 6e67 655b 313a 5d2e 7374 7269 7028 290d  nge[1:].strip().
+0001bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc30: 2020 2020 2071 203d 2073 796d 7079 2e6c       q = sympy.l
+0001bc40: 6174 6578 2873 796d 7079 2e73 696d 706c  atex(sympy.simpl
+0001bc50: 6966 7928 7369 676e 202b 2066 696c 6564  ify(sign + filed
+0001bc60: 6174 615b 2271 7561 6e74 6974 7922 5d29  ata["quantity"])
+0001bc70: 2c20 6d6f 6465 3d22 696e 6c69 6e65 2229  , mode="inline")
+0001bc80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bca0: 2020 2020 2020 7375 626a 6563 7420 3d20        subject = 
+0001bcb0: 2220 2020 2822 202b 2066 696c 6564 6174  "   (" + filedat
+0001bcc0: 615b 2273 7562 6a65 6374 225d 2e72 6570  a["subject"].rep
+0001bcd0: 6c61 6365 2822 5f22 2c20 2220 2229 202b  lace("_", " ") +
+0001bce0: 2022 2922 0d0a 0d0a 2020 2020 2020 2020   ")"....        
+0001bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd00: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+0001bd10: 6e74 2822 6e61 6d65 222c 206e 616d 6529  nt("name", name)
+0001bd20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0001bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd50: 2069 6620 6e61 6d65 206e 6f74 2069 6e20   if name not in 
-0001bd60: 636f 6d62 696e 6564 5f73 6865 6574 735b  combined_sheets[
-0001bd70: 6167 656e 7431 5d5b 2241 7373 6574 7322  agent1]["Assets"
-0001bd80: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+0001bd40: 2020 2020 2020 2370 7269 6e74 2822 636f        #print("co
+0001bd50: 6d62 696e 6564 5f73 6865 6574 735b 6167  mbined_sheets[ag
+0001bd60: 656e 7431 5d22 2c20 636f 6d62 696e 6564  ent1]", combined
+0001bd70: 5f73 6865 6574 735b 6167 656e 7431 5d29  _sheets[agent1])
+0001bd80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bda0: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-0001bdb0: 696e 6564 5f73 6865 6574 735b 6167 656e  ined_sheets[agen
-0001bdc0: 7431 5d5b 2241 7373 6574 7322 5d5b 6e61  t1]["Assets"][na
-0001bdd0: 6d65 5d20 3d20 2222 0d0a 0d0a 2020 2020  me] = ""....    
+0001bda0: 2020 2020 2020 6966 206e 616d 6520 6e6f        if name no
+0001bdb0: 7420 696e 2063 6f6d 6269 6e65 645f 7368  t in combined_sh
+0001bdc0: 6565 7473 5b61 6765 6e74 315d 5b22 4173  eets[agent1]["As
+0001bdd0: 7365 7473 225d 3a0d 0a20 2020 2020 2020  sets"]:..       
 0001bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be00: 636f 6d62 696e 6564 5f73 6865 6574 735b  combined_sheets[
-0001be10: 6167 656e 7431 5d5b 2241 7373 6574 7322  agent1]["Assets"
-0001be20: 5d5b 6e61 6d65 5d20 2b3d 2071 202b 2073  ][name] += q + s
-0001be30: 7562 6a65 6374 202b 2022 5c6e 220d 0a20  ubject + "\n".. 
+0001be00: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001be10: 5b61 6765 6e74 315d 5b22 4173 7365 7473  [agent1]["Assets
+0001be20: 225d 5b6e 616d 655d 203d 2022 220d 0a0d  "][name] = ""...
+0001be30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001be60: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be80: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0001be90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bea0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0001beb0: 7220 6368 616e 6765 2069 6e20 6c69 6162  r change in liab
-0001bec0: 7331 2e73 706c 6974 2822 5c6e 2229 3a0d  s1.split("\n"):.
-0001bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bef0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0001bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf10: 2020 2020 2020 2020 2020 2073 6967 6e20             sign 
-0001bf20: 3d20 6368 616e 6765 5b30 5d20 2023 2066  = change[0]  # f
-0001bf30: 6972 7374 206c 6574 7465 7220 6973 2073  irst letter is s
-0001bf40: 6967 6e20 2b20 6f72 202d 0d0a 0d0a 2020  ign + or -....  
+0001be50: 2020 2020 2063 6f6d 6269 6e65 645f 7368       combined_sh
+0001be60: 6565 7473 5b61 6765 6e74 315d 5b22 4173  eets[agent1]["As
+0001be70: 7365 7473 225d 5b6e 616d 655d 202b 3d20  sets"][name] += 
+0001be80: 7120 2b20 7375 626a 6563 7420 2b20 225c  q + subject + "\
+0001be90: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
+0001bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001beb0: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+0001bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bee0: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf00: 2020 2066 6f72 2063 6861 6e67 6520 696e     for change in
+0001bf10: 206c 6961 6273 312e 7370 6c69 7428 225c   liabs1.split("\
+0001bf20: 6e22 293a 0d0a 2020 2020 2020 2020 2020  n"):..          
+0001bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf40: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
 0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf70: 2020 6e61 6d65 203d 2063 6861 6e67 655b    name = change[
-0001bf80: 313a 5d2e 7374 7269 7028 290d 0a20 2020  1:].strip()..   
-0001bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0001bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfd0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-0001bfe0: 203d 2073 796d 7079 2e6c 6174 6578 2873   = sympy.latex(s
-0001bff0: 796d 7079 2e73 696d 706c 6966 7928 7369  ympy.simplify(si
-0001c000: 676e 202b 2066 696c 6564 6174 615b 2271  gn + filedata["q
-0001c010: 7561 6e74 6974 7922 5d29 2c20 6d6f 6465  uantity"]), mode
-0001c020: 3d22 696e 6c69 6e65 2229 0d0a 2020 2020  ="inline")..    
-0001c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c050: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0001c060: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c090: 7365 6c66 2e6e 6f74 6966 7928 0d0a 2020  self.notify(..  
-0001c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0c0: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
-0001c0d0: 7420 6861 6e64 6c65 2074 6865 2073 796d  t handle the sym
-0001c0e0: 626f 6c69 6320 6578 7072 6573 7369 6f6e  bolic expression
-0001c0f0: 2025 7322 2025 2073 6967 6e20 2b20 6669   %s" % sign + fi
-0001c100: 6c65 6461 7461 5b0d 0a20 2020 2020 2020  ledata[..       
-0001c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c130: 2020 2020 2020 2020 2022 7175 616e 7469           "quanti
-0001c140: 7479 225d 2c74 6974 6c65 3d22 4572 726f  ty"],title="Erro
-0001c150: 7222 290d 0a0d 0a20 2020 2020 2020 2020  r")....         
+0001bf70: 7369 676e 203d 2063 6861 6e67 655b 305d  sign = change[0]
+0001bf80: 2020 2320 6669 7273 7420 6c65 7474 6572    # first letter
+0001bf90: 2069 7320 7369 676e 202b 206f 7220 2d0d   is sign + or -.
+0001bfa0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bfc0: 2020 2020 2020 206e 616d 6520 3d20 6368         name = ch
+0001bfd0: 616e 6765 5b31 3a5d 2e73 7472 6970 2829  ange[1:].strip()
+0001bfe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c000: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c030: 2020 2020 7120 3d20 7379 6d70 792e 6c61      q = sympy.la
+0001c040: 7465 7828 7379 6d70 792e 7369 6d70 6c69  tex(sympy.simpli
+0001c050: 6679 2873 6967 6e20 2b20 6669 6c65 6461  fy(sign + fileda
+0001c060: 7461 5b22 7175 616e 7469 7479 225d 292c  ta["quantity"]),
+0001c070: 206d 6f64 653d 2269 6e6c 696e 6522 290d   mode="inline").
+0001c080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0a0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0001c0b0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0e0: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
+0001c0f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c110: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c120: 4361 6e6e 6f74 2068 616e 646c 6520 7468  Cannot handle th
+0001c130: 6520 7379 6d62 6f6c 6963 2065 7870 7265  e symbolic expre
+0001c140: 7373 696f 6e20 2573 2220 2520 7369 676e  ssion %s" % sign
+0001c150: 202b 2066 696c 6564 6174 615b 0d0a 2020   + filedata[..  
 0001c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c170: 2020 2020 2020 2020 2020 2073 7562 6a65             subje
-0001c180: 6374 203d 2022 2020 2028 2220 2b20 6669  ct = "   (" + fi
-0001c190: 6c65 6461 7461 5b22 7375 626a 6563 7422  ledata["subject"
-0001c1a0: 5d2e 7265 706c 6163 6528 225f 222c 2022  ].replace("_", "
-0001c1b0: 2022 2920 2b20 2229 220d 0a0d 0a20 2020   ") + ")"....   
+0001c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c180: 2020 2020 2020 2020 2020 2020 2020 2271                "q
+0001c190: 7561 6e74 6974 7922 5d2c 7469 746c 653d  uantity"],title=
+0001c1a0: 2245 7272 6f72 2229 0d0a 0d0a 2020 2020  "Error")....    
+0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1e0: 2069 6620 6e61 6d65 206e 6f74 2069 6e20   if name not in 
-0001c1f0: 636f 6d62 696e 6564 5f73 6865 6574 735b  combined_sheets[
-0001c200: 6167 656e 7431 5d5b 224c 6961 6269 6c69  agent1]["Liabili
-0001c210: 7469 6573 2061 6e64 2045 7175 6974 7922  ties and Equity"
-0001c220: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-0001c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c240: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-0001c250: 696e 6564 5f73 6865 6574 735b 6167 656e  ined_sheets[agen
-0001c260: 7431 5d5b 224c 6961 6269 6c69 7469 6573  t1]["Liabilities
-0001c270: 2061 6e64 2045 7175 6974 7922 5d5b 6e61   and Equity"][na
-0001c280: 6d65 5d20 3d20 2222 0d0a 0d0a 2020 2020  me] = ""....    
+0001c1d0: 7375 626a 6563 7420 3d20 2220 2020 2822  subject = "   ("
+0001c1e0: 202b 2066 696c 6564 6174 615b 2273 7562   + filedata["sub
+0001c1f0: 6a65 6374 225d 2e72 6570 6c61 6365 2822  ject"].replace("
+0001c200: 5f22 2c20 2220 2229 202b 2022 2922 0d0a  _", " ") + ")"..
+0001c210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c230: 2020 2020 2020 6966 206e 616d 6520 6e6f        if name no
+0001c240: 7420 696e 2063 6f6d 6269 6e65 645f 7368  t in combined_sh
+0001c250: 6565 7473 5b61 6765 6e74 315d 5b22 4c69  eets[agent1]["Li
+0001c260: 6162 696c 6974 6965 7320 616e 6420 4571  abilities and Eq
+0001c270: 7569 7479 225d 3a0d 0a20 2020 2020 2020  uity"]:..       
+0001c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c2b0: 636f 6d62 696e 6564 5f73 6865 6574 735b  combined_sheets[
-0001c2c0: 6167 656e 7431 5d5b 224c 6961 6269 6c69  agent1]["Liabili
-0001c2d0: 7469 6573 2061 6e64 2045 7175 6974 7922  ties and Equity"
-0001c2e0: 5d5b 6e61 6d65 5d20 2b3d 2071 202b 2073  ][name] += q + s
-0001c2f0: 7562 6a65 6374 202b 2022 5c6e 220d 0a20  ubject + "\n".. 
-0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c310: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001c320: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-0001c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c340: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0001c350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001c2a0: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001c2b0: 5b61 6765 6e74 315d 5b22 4c69 6162 696c  [agent1]["Liabil
+0001c2c0: 6974 6965 7320 616e 6420 4571 7569 7479  ities and Equity
+0001c2d0: 225d 5b6e 616d 655d 203d 2022 220d 0a0d  "][name] = ""...
+0001c2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c300: 2020 2020 2063 6f6d 6269 6e65 645f 7368       combined_sh
+0001c310: 6565 7473 5b61 6765 6e74 315d 5b22 4c69  eets[agent1]["Li
+0001c320: 6162 696c 6974 6965 7320 616e 6420 4571  abilities and Eq
+0001c330: 7569 7479 225d 5b6e 616d 655d 202b 3d20  uity"][name] += 
+0001c340: 7120 2b20 7375 626a 6563 7420 2b20 225c  q + subject + "\
+0001c350: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
 0001c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c370: 6966 2073 7472 2866 696c 6564 6174 615b  if str(filedata[
-0001c380: 2269 6e63 6f6d 6531 225d 2920 213d 2027  "income1"]) != '
-0001c390: 4e6f 6e65 273a 0d0a 2020 2020 2020 2020  None':..        
-0001c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3b0: 2020 2020 2020 2020 6d79 6469 6374 203d          mydict =
-0001c3c0: 207b 2247 6169 6e22 3a20 2247 6169 6e73   {"Gain": "Gains
-0001c3d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3f0: 2020 2020 2020 2020 2020 2020 2020 224c                "L
-0001c400: 6f73 7322 3a20 224c 6f73 7365 7322 2c0d  oss": "Losses",.
-0001c410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c430: 2020 2020 2020 2020 2020 2022 4578 7065             "Expe
-0001c440: 6e73 6522 3a20 2245 7870 656e 7365 7322  nse": "Expenses"
-0001c450: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c470: 2020 2020 2020 2020 2020 2020 2022 5265               "Re
-0001c480: 7665 6e75 6522 3a20 2252 6576 656e 7565  venue": "Revenue
-0001c490: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c4c0: 5461 7822 3a20 2254 6178 6573 222c 0d0a  Tax": "Taxes",..
-0001c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4f0: 2020 2020 2020 2020 2020 224e 6f6e 7461            "Nonta
-0001c500: 782e 2050 726f 6669 7422 3a20 224e 6f6e  x. Profit": "Non
-0001c510: 7461 7861 626c 6520 5072 6f66 6974 7322  taxable Profits"
-0001c520: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001c370: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+0001c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3a0: 2070 6173 730d 0a0d 0a20 2020 2020 2020   pass....       
+0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3c0: 2020 2020 2069 6620 7374 7228 6669 6c65       if str(file
+0001c3d0: 6461 7461 5b22 696e 636f 6d65 3122 5d29  data["income1"])
+0001c3e0: 2021 3d20 274e 6f6e 6527 3a0d 0a20 2020   != 'None':..   
+0001c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c400: 2020 2020 2020 2020 2020 2020 206d 7964               myd
+0001c410: 6963 7420 3d20 7b22 4761 696e 223a 2022  ict = {"Gain": "
+0001c420: 4761 696e 7322 2c0d 0a20 2020 2020 2020  Gains",..       
+0001c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c450: 2020 2022 4c6f 7373 223a 2022 4c6f 7373     "Loss": "Loss
+0001c460: 6573 222c 0d0a 2020 2020 2020 2020 2020  es",..          
+0001c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c490: 2245 7870 656e 7365 223a 2022 4578 7065  "Expense": "Expe
+0001c4a0: 6e73 6573 222c 0d0a 2020 2020 2020 2020  nses",..        
+0001c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4d0: 2020 2252 6576 656e 7565 223a 2022 5265    "Revenue": "Re
+0001c4e0: 7665 6e75 6573 222c 0d0a 2020 2020 2020  venues",..      
+0001c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c510: 2020 2020 2254 6178 223a 2022 5461 7865      "Tax": "Taxe
+0001c520: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
 0001c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c540: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
-0001c550: 6e74 6178 2e20 4c6f 7373 223a 2022 4e6f  ntax. Loss": "No
-0001c560: 6e74 6178 6162 6c65 204c 6f73 7365 7322  ntaxable Losses"
-0001c570: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001c540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001c550: 4e6f 6e74 6178 2e20 5072 6f66 6974 223a  Nontax. Profit":
+0001c560: 2022 4e6f 6e74 6178 6162 6c65 2050 726f   "Nontaxable Pro
+0001c570: 6669 7473 222c 0d0a 2020 2020 2020 2020  fits",..        
 0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c590: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
-0001c5a0: 6e2d 4f70 2e20 496e 636f 6d65 223a 2022  n-Op. Income": "
-0001c5b0: 4e6f 6e2d 4f70 6572 6174 696f 6e61 6c20  Non-Operational 
-0001c5c0: 496e 636f 6d65 222c 0d0a 2020 2020 2020  Income",..      
+0001c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c5a0: 2020 224e 6f6e 7461 782e 204c 6f73 7322    "Nontax. Loss"
+0001c5b0: 3a20 224e 6f6e 7461 7861 626c 6520 4c6f  : "Nontaxable Lo
+0001c5c0: 7373 6573 222c 0d0a 2020 2020 2020 2020  sses",..        
 0001c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5f0: 2020 2020 2249 6e74 6572 6573 7422 3a20      "Interest": 
-0001c600: 2249 6e74 6572 6573 7420 5061 796d 656e  "Interest Paymen
-0001c610: 7473 227d 0d0a 0d0a 2020 2020 2020 2020  ts"}....        
+0001c5f0: 2020 224e 6f6e 2d4f 702e 2049 6e63 6f6d    "Non-Op. Incom
+0001c600: 6522 3a20 224e 6f6e 2d4f 7065 7261 7469  e": "Non-Operati
+0001c610: 6f6e 616c 2049 6e63 6f6d 6522 2c0d 0a20  onal Income",.. 
 0001c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c630: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c660: 2020 7120 3d20 7379 6d70 792e 6c61 7465    q = sympy.late
-0001c670: 7828 7379 6d70 792e 7369 6d70 6c69 6679  x(sympy.simplify
-0001c680: 2873 6967 6e20 2b20 6669 6c65 6461 7461  (sign + filedata
-0001c690: 5b22 7175 616e 7469 7479 225d 292c 206d  ["quantity"]), m
-0001c6a0: 6f64 653d 2269 6e6c 696e 6522 290d 0a20  ode="inline").. 
-0001c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6d0: 2020 2073 7562 6a65 6374 203d 2022 2020     subject = "  
-0001c6e0: 2028 2220 2b20 6669 6c65 6461 7461 5b22   (" + filedata["
-0001c6f0: 7375 626a 6563 7422 5d2e 7265 706c 6163  subject"].replac
-0001c700: 6528 225f 222c 2022 2022 2920 2b20 2229  e("_", " ") + ")
-0001c710: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0001c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c730: 2020 2020 2020 2063 6f6d 6269 6e65 645f         combined_
-0001c740: 696e 636f 6d65 5b61 6765 6e74 315d 5b6d  income[agent1][m
-0001c750: 7964 6963 745b 6669 6c65 6461 7461 5b22  ydict[filedata["
-0001c760: 696e 636f 6d65 3122 5d5d 5d2e 6170 7065  income1"]]].appe
-0001c770: 6e64 2828 7374 7228 7129 2c20 7375 626a  nd((str(q), subj
-0001c780: 6563 7429 290d 0a0d 0a20 2020 2020 2020  ect))....       
-0001c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7a0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0001c7b0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-0001c7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7e0: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
-0001c7f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c810: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
-0001c820: 6f74 2068 616e 646c 6520 7468 6520 7379  ot handle the sy
-0001c830: 6d62 6f6c 6963 2065 7870 7265 7373 696f  mbolic expressio
-0001c840: 6e20 2573 2220 2520 7369 676e 202b 2066  n %s" % sign + f
-0001c850: 696c 6564 6174 615b 2271 7561 6e74 6974  iledata["quantit
-0001c860: 7922 5d2c 7469 746c 653d 2245 7272 6f72  y"],title="Error
-0001c870: 2229 0d0a 0d0a 0d0a 2020 2020 2020 2020  ")......        
-0001c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c890: 2020 2020 230d 0a20 2020 2020 2020 2020      #..         
-0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8b0: 2020 2023 2041 4745 4e54 2032 0d0a 2020     # AGENT 2..  
-0001c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8d0: 2020 2020 2020 2020 2020 230d 0a0d 0a20            #.... 
-0001c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8f0: 2020 2020 2020 2020 2020 2069 6620 6167             if ag
-0001c900: 656e 7432 206e 6f74 2069 6e20 636f 6d62  ent2 not in comb
-0001c910: 696e 6564 5f73 6865 6574 733a 0d0a 2020  ined_sheets:..  
-0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c930: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0001c940: 6d62 696e 6564 5f73 6865 6574 735b 6167  mbined_sheets[ag
-0001c950: 656e 7432 5d20 3d20 7b7d 0d0a 0d0a 2020  ent2] = {}....  
-0001c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c970: 2020 2020 2020 2020 2020 6966 2022 4173            if "As
-0001c980: 7365 7473 2220 6e6f 7420 696e 2063 6f6d  sets" not in com
-0001c990: 6269 6e65 645f 7368 6565 7473 5b61 6765  bined_sheets[age
-0001c9a0: 6e74 325d 3a0d 0a20 2020 2020 2020 2020  nt2]:..         
-0001c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9c0: 2020 2020 2020 2063 6f6d 6269 6e65 645f         combined_
-0001c9d0: 7368 6565 7473 5b61 6765 6e74 325d 5b22  sheets[agent2]["
-0001c9e0: 4173 7365 7473 225d 203d 207b 7d0d 0a20  Assets"] = {}.. 
-0001c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca00: 2020 2020 2020 2020 2020 2069 6620 224c             if "L
-0001ca10: 6961 6269 6c69 7469 6573 2061 6e64 2045  iabilities and E
-0001ca20: 7175 6974 7922 206e 6f74 2069 6e20 636f  quity" not in co
-0001ca30: 6d62 696e 6564 5f73 6865 6574 735b 6167  mbined_sheets[ag
-0001ca40: 656e 7432 5d3a 0d0a 2020 2020 2020 2020  ent2]:..        
+0001c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c640: 2020 2020 2020 2020 2022 496e 7465 7265           "Intere
+0001c650: 7374 223a 2022 496e 7465 7265 7374 2050  st": "Interest P
+0001c660: 6179 6d65 6e74 7322 7d0d 0a0d 0a20 2020  ayments"}....   
+0001c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c680: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0001c690: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c6b0: 2020 2020 2020 2071 203d 2073 796d 7079         q = sympy
+0001c6c0: 2e6c 6174 6578 2873 796d 7079 2e73 696d  .latex(sympy.sim
+0001c6d0: 706c 6966 7928 7369 676e 202b 2066 696c  plify(sign + fil
+0001c6e0: 6564 6174 615b 2271 7561 6e74 6974 7922  edata["quantity"
+0001c6f0: 5d29 2c20 6d6f 6465 3d22 696e 6c69 6e65  ]), mode="inline
+0001c700: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0001c710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c720: 2020 2020 2020 2020 7375 626a 6563 7420          subject 
+0001c730: 3d20 2220 2020 2822 202b 2066 696c 6564  = "   (" + filed
+0001c740: 6174 615b 2273 7562 6a65 6374 225d 2e72  ata["subject"].r
+0001c750: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
+0001c760: 202b 2022 2922 0d0a 2020 2020 2020 2020   + ")"..        
+0001c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c780: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
+0001c790: 696e 6564 5f69 6e63 6f6d 655b 6167 656e  ined_income[agen
+0001c7a0: 7431 5d5b 6d79 6469 6374 5b66 696c 6564  t1][mydict[filed
+0001c7b0: 6174 615b 2269 6e63 6f6d 6531 225d 5d5d  ata["income1"]]]
+0001c7c0: 2e61 7070 656e 6428 2873 7472 2871 292c  .append((str(q),
+0001c7d0: 2073 7562 6a65 6374 2929 0d0a 0d0a 2020   subject))....  
+0001c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7f0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0001c800: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0001c810: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+0001c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c830: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001c840: 6f74 6966 7928 0d0a 2020 2020 2020 2020  otify(..        
+0001c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c870: 2243 616e 6e6f 7420 6861 6e64 6c65 2074  "Cannot handle t
+0001c880: 6865 2073 796d 626f 6c69 6320 6578 7072  he symbolic expr
+0001c890: 6573 7369 6f6e 2025 7322 2025 2073 6967  ession %s" % sig
+0001c8a0: 6e20 2b20 6669 6c65 6461 7461 5b22 7175  n + filedata["qu
+0001c8b0: 616e 7469 7479 225d 2c74 6974 6c65 3d22  antity"],title="
+0001c8c0: 4572 726f 7222 290d 0a0d 0a0d 0a20 2020  Error")......   
+0001c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8e0: 2020 2020 2020 2020 2023 0d0a 2020 2020           #..    
+0001c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c900: 2020 2020 2020 2020 2320 4147 454e 5420          # AGENT 
+0001c910: 320d 0a20 2020 2020 2020 2020 2020 2020  2..             
+0001c920: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001c930: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c950: 6966 2061 6765 6e74 3220 6e6f 7420 696e  if agent2 not in
+0001c960: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
+0001c970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c990: 2020 2063 6f6d 6269 6e65 645f 7368 6565     combined_shee
+0001c9a0: 7473 5b61 6765 6e74 325d 203d 207b 7d0d  ts[agent2] = {}.
+0001c9b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001c9c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001c9d0: 6620 2241 7373 6574 7322 206e 6f74 2069  f "Assets" not i
+0001c9e0: 6e20 636f 6d62 696e 6564 5f73 6865 6574  n combined_sheet
+0001c9f0: 735b 6167 656e 7432 5d3a 0d0a 2020 2020  s[agent2]:..    
+0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca10: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
+0001ca20: 696e 6564 5f73 6865 6574 735b 6167 656e  ined_sheets[agen
+0001ca30: 7432 5d5b 2241 7373 6574 7322 5d20 3d20  t2]["Assets"] = 
+0001ca40: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
 0001ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca60: 2020 2020 2020 2020 636f 6d62 696e 6564          combined
-0001ca70: 5f73 6865 6574 735b 6167 656e 7432 5d5b  _sheets[agent2][
-0001ca80: 224c 6961 6269 6c69 7469 6573 2061 6e64  "Liabilities and
-0001ca90: 2045 7175 6974 7922 5d20 3d20 7b7d 0d0a   Equity"] = {}..
-0001caa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001cab0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0001cac0: 7220 6368 616e 6765 2069 6e20 6173 7365  r change in asse
-0001cad0: 7473 322e 7370 6c69 7428 225c 6e22 293a  ts2.split("\n"):
-0001cae0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb00: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0001cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb20: 2020 2020 2020 2020 2020 2020 2020 7369                si
-0001cb30: 676e 203d 2063 6861 6e67 655b 305d 2020  gn = change[0]  
-0001cb40: 2320 6669 7273 7420 6c65 7474 6572 2069  # first letter i
-0001cb50: 7320 7369 676e 202b 206f 7220 2d0d 0a0d  s sign + or -...
-0001cb60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ca60: 6966 2022 4c69 6162 696c 6974 6965 7320  if "Liabilities 
+0001ca70: 616e 6420 4571 7569 7479 2220 6e6f 7420  and Equity" not 
+0001ca80: 696e 2063 6f6d 6269 6e65 645f 7368 6565  in combined_shee
+0001ca90: 7473 5b61 6765 6e74 325d 3a0d 0a20 2020  ts[agent2]:..   
+0001caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cab0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0001cac0: 6269 6e65 645f 7368 6565 7473 5b61 6765  bined_sheets[age
+0001cad0: 6e74 325d 5b22 4c69 6162 696c 6974 6965  nt2]["Liabilitie
+0001cae0: 7320 616e 6420 4571 7569 7479 225d 203d  s and Equity"] =
+0001caf0: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
+0001cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb10: 2020 2066 6f72 2063 6861 6e67 6520 696e     for change in
+0001cb20: 2061 7373 6574 7332 2e73 706c 6974 2822   assets2.split("
+0001cb30: 5c6e 2229 3a0d 0a0d 0a20 2020 2020 2020  \n"):....       
+0001cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb50: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+0001cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb80: 2020 2020 206e 616d 6520 3d20 6368 616e       name = chan
-0001cb90: 6765 5b31 3a5d 2e73 7472 6970 2829 0d0a  ge[1:].strip()..
-0001cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbc0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0001cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbf0: 2020 7120 3d20 7379 6d70 792e 6c61 7465    q = sympy.late
-0001cc00: 7828 7379 6d70 792e 7369 6d70 6c69 6679  x(sympy.simplify
-0001cc10: 2873 6967 6e20 2b20 6669 6c65 6461 7461  (sign + filedata
-0001cc20: 5b22 7175 616e 7469 7479 225d 292c 206d  ["quantity"]), m
-0001cc30: 6f64 653d 2269 6e6c 696e 6522 290d 0a20  ode="inline").. 
-0001cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc60: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0001cc70: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0001cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cca0: 2020 2073 656c 662e 6e6f 7469 6679 280d     self.notify(.
-0001ccb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ccd0: 2020 2020 2020 2020 2020 2020 2022 4361               "Ca
-0001cce0: 6e6e 6f74 2068 616e 646c 6520 7468 6520  nnot handle the 
-0001ccf0: 7379 6d62 6f6c 6963 2065 7870 7265 7373  symbolic express
-0001cd00: 696f 6e20 2573 2220 2520 7369 676e 202b  ion %s" % sign +
-0001cd10: 2066 696c 6564 6174 615b 0d0a 2020 2020   filedata[..    
+0001cb80: 2020 2073 6967 6e20 3d20 6368 616e 6765     sign = change
+0001cb90: 5b30 5d20 2023 2066 6972 7374 206c 6574  [0]  # first let
+0001cba0: 7465 7220 6973 2073 6967 6e20 2b20 6f72  ter is sign + or
+0001cbb0: 202d 0d0a 0d0a 2020 2020 2020 2020 2020   -....          
+0001cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbd0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+0001cbe0: 2063 6861 6e67 655b 313a 5d2e 7374 7269   change[1:].stri
+0001cbf0: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
+0001cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc10: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+0001cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc40: 2020 2020 2020 2071 203d 2073 796d 7079         q = sympy
+0001cc50: 2e6c 6174 6578 2873 796d 7079 2e73 696d  .latex(sympy.sim
+0001cc60: 706c 6966 7928 7369 676e 202b 2066 696c  plify(sign + fil
+0001cc70: 6564 6174 615b 2271 7561 6e74 6974 7922  edata["quantity"
+0001cc80: 5d29 2c20 6d6f 6465 3d22 696e 6c69 6e65  ]), mode="inline
+0001cc90: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0001cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0001ccc0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0001ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ccf0: 2020 2020 2020 2020 7365 6c66 2e6e 6f74          self.not
+0001cd00: 6966 7928 0d0a 2020 2020 2020 2020 2020  ify(..          
+0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd40: 2020 2020 2020 2020 2020 2020 2271 7561              "qua
-0001cd50: 6e74 6974 7922 5d2c 7469 746c 653d 2245  ntity"],title="E
-0001cd60: 7272 6f72 2229 0d0a 0d0a 2020 2020 2020  rror")....      
-0001cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd80: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0001cd90: 626a 6563 7420 3d20 2220 2020 2822 202b  bject = "   (" +
-0001cda0: 2066 696c 6564 6174 615b 2273 7562 6a65   filedata["subje
-0001cdb0: 6374 225d 2e72 6570 6c61 6365 2822 5f22  ct"].replace("_"
-0001cdc0: 2c20 2220 2229 202b 2022 2922 0d0a 0d0a  , " ") + ")"....
+0001cd30: 2020 2243 616e 6e6f 7420 6861 6e64 6c65    "Cannot handle
+0001cd40: 2074 6865 2073 796d 626f 6c69 6320 6578   the symbolic ex
+0001cd50: 7072 6573 7369 6f6e 2025 7322 2025 2073  pression %s" % s
+0001cd60: 6967 6e20 2b20 6669 6c65 6461 7461 5b0d  ign + filedata[.
+0001cd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cda0: 2022 7175 616e 7469 7479 225d 2c74 6974   "quantity"],tit
+0001cdb0: 6c65 3d22 4572 726f 7222 290d 0a0d 0a20  le="Error").... 
+0001cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cdf0: 2020 2020 6966 206e 616d 6520 6e6f 7420      if name not 
-0001ce00: 696e 2063 6f6d 6269 6e65 645f 7368 6565  in combined_shee
-0001ce10: 7473 5b61 6765 6e74 325d 5b22 4173 7365  ts[agent2]["Asse
-0001ce20: 7473 225d 3a0d 0a20 2020 2020 2020 2020  ts"]:..         
+0001cde0: 2020 2073 7562 6a65 6374 203d 2022 2020     subject = "  
+0001cdf0: 2028 2220 2b20 6669 6c65 6461 7461 5b22   (" + filedata["
+0001ce00: 7375 626a 6563 7422 5d2e 7265 706c 6163  subject"].replac
+0001ce10: 6528 225f 222c 2022 2022 2920 2b20 2229  e("_", " ") + ")
+0001ce20: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
 0001ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001ce50: 6f6d 6269 6e65 645f 7368 6565 7473 5b61  ombined_sheets[a
-0001ce60: 6765 6e74 325d 5b22 4173 7365 7473 225d  gent2]["Assets"]
-0001ce70: 5b6e 616d 655d 203d 2022 220d 0a0d 0a20  [name] = "".... 
+0001ce40: 2020 2020 2020 2020 2069 6620 6e61 6d65           if name
+0001ce50: 206e 6f74 2069 6e20 636f 6d62 696e 6564   not in combined
+0001ce60: 5f73 6865 6574 735b 6167 656e 7432 5d5b  _sheets[agent2][
+0001ce70: 2241 7373 6574 7322 5d3a 0d0a 2020 2020  "Assets"]:..    
 0001ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cea0: 2020 2063 6f6d 6269 6e65 645f 7368 6565     combined_shee
-0001ceb0: 7473 5b61 6765 6e74 325d 5b22 4173 7365  ts[agent2]["Asse
-0001cec0: 7473 225d 5b6e 616d 655d 202b 3d20 7120  ts"][name] += q 
-0001ced0: 2b20 7375 626a 6563 7420 2b20 225c 6e22  + subject + "\n"
-0001cee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf00: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-0001cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001cf30: 6173 730d 0a0d 0a20 2020 2020 2020 2020  ass....         
+0001cea0: 2020 2020 636f 6d62 696e 6564 5f73 6865      combined_she
+0001ceb0: 6574 735b 6167 656e 7432 5d5b 2241 7373  ets[agent2]["Ass
+0001cec0: 6574 7322 5d5b 6e61 6d65 5d20 3d20 2222  ets"][name] = ""
+0001ced0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cef0: 2020 2020 2020 2020 636f 6d62 696e 6564          combined
+0001cf00: 5f73 6865 6574 735b 6167 656e 7432 5d5b  _sheets[agent2][
+0001cf10: 2241 7373 6574 7322 5d5b 6e61 6d65 5d20  "Assets"][name] 
+0001cf20: 2b3d 2071 202b 2073 7562 6a65 6374 202b  += q + subject +
+0001cf30: 2022 5c6e 220d 0a20 2020 2020 2020 2020   "\n"..         
 0001cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf50: 2020 2066 6f72 2063 6861 6e67 6520 696e     for change in
-0001cf60: 206c 6961 6273 322e 7370 6c69 7428 225c   liabs2.split("\
-0001cf70: 6e22 293a 0d0a 2020 2020 2020 2020 2020  n"):..          
-0001cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf90: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0001cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cfc0: 7369 676e 203d 2063 6861 6e67 655b 305d  sign = change[0]
-0001cfd0: 2020 2320 6669 7273 7420 6c65 7474 6572    # first letter
-0001cfe0: 2069 7320 7369 676e 202b 206f 7220 2d0d   is sign + or -.
-0001cff0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001cf50: 2020 2020 2020 2065 7863 6570 743a 0d0a         except:..
+0001cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf80: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
+0001cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cfa0: 2020 2020 2020 2020 666f 7220 6368 616e          for chan
+0001cfb0: 6765 2069 6e20 6c69 6162 7332 2e73 706c  ge in liabs2.spl
+0001cfc0: 6974 2822 5c6e 2229 3a0d 0a20 2020 2020  it("\n"):..     
+0001cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cfe0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+0001cff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0001d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d010: 2020 2020 2020 206e 616d 6520 3d20 6368         name = ch
-0001d020: 616e 6765 5b31 3a5d 2e73 7472 6970 2829  ange[1:].strip()
-0001d030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d050: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-0001d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d080: 2020 2020 7120 3d20 7379 6d70 792e 6c61      q = sympy.la
-0001d090: 7465 7828 7379 6d70 792e 7369 6d70 6c69  tex(sympy.simpli
-0001d0a0: 6679 2873 6967 6e20 2b20 6669 6c65 6461  fy(sign + fileda
-0001d0b0: 7461 5b22 7175 616e 7469 7479 225d 292c  ta["quantity"]),
-0001d0c0: 206d 6f64 653d 2269 6e6c 696e 6522 290d   mode="inline").
-0001d0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0f0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0001d100: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d130: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
-0001d140: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d160: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001d170: 4361 6e6e 6f74 2068 616e 646c 6520 7468  Cannot handle th
-0001d180: 6520 7379 6d62 6f6c 6963 2065 7870 7265  e symbolic expre
-0001d190: 7373 696f 6e20 2573 2220 2520 7369 676e  ssion %s" % sign
-0001d1a0: 202b 2066 696c 6564 6174 615b 0d0a 2020   + filedata[..  
+0001d010: 2020 2020 2073 6967 6e20 3d20 6368 616e       sign = chan
+0001d020: 6765 5b30 5d20 2023 2066 6972 7374 206c  ge[0]  # first l
+0001d030: 6574 7465 7220 6973 2073 6967 6e20 2b20  etter is sign + 
+0001d040: 6f72 202d 0d0a 0d0a 2020 2020 2020 2020  or -....        
+0001d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d060: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0001d070: 203d 2063 6861 6e67 655b 313a 5d2e 7374   = change[1:].st
+0001d080: 7269 7028 290d 0a20 2020 2020 2020 2020  rip()..         
+0001d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0a0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+0001d0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0d0: 2020 2020 2020 2020 2071 203d 2073 796d           q = sym
+0001d0e0: 7079 2e6c 6174 6578 2873 796d 7079 2e73  py.latex(sympy.s
+0001d0f0: 696d 706c 6966 7928 7369 676e 202b 2066  implify(sign + f
+0001d100: 696c 6564 6174 615b 2271 7561 6e74 6974  iledata["quantit
+0001d110: 7922 5d29 2c20 6d6f 6465 3d22 696e 6c69  y"]), mode="inli
+0001d120: 6e65 2229 0d0a 2020 2020 2020 2020 2020  ne")..          
+0001d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d140: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0001d150: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+0001d160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d180: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001d190: 6f74 6966 7928 0d0a 2020 2020 2020 2020  otify(..        
+0001d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1d0: 2020 2020 2020 2020 2020 2020 2020 2271                "q
-0001d1e0: 7561 6e74 6974 7922 5d2c 7469 746c 653d  uantity"],title=
-0001d1f0: 2245 7272 6f72 2229 0d0a 0d0a 2020 2020  "Error")....    
-0001d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d1c0: 2020 2020 2243 616e 6e6f 7420 6861 6e64      "Cannot hand
+0001d1d0: 6c65 2074 6865 2073 796d 626f 6c69 6320  le the symbolic 
+0001d1e0: 6578 7072 6573 7369 6f6e 2025 7322 2025  expression %s" %
+0001d1f0: 2073 6967 6e20 2b20 6669 6c65 6461 7461   sign + filedata
+0001d200: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
 0001d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d220: 7375 626a 6563 7420 3d20 2220 2020 2822  subject = "   ("
-0001d230: 202b 2066 696c 6564 6174 615b 2273 7562   + filedata["sub
-0001d240: 6a65 6374 225d 2e72 6570 6c61 6365 2822  ject"].replace("
-0001d250: 5f22 2c20 2220 2229 202b 2022 2922 0d0a  _", " ") + ")"..
-0001d260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d280: 2020 2020 2020 6966 206e 616d 6520 6e6f        if name no
-0001d290: 7420 696e 2063 6f6d 6269 6e65 645f 7368  t in combined_sh
-0001d2a0: 6565 7473 5b61 6765 6e74 325d 5b22 4c69  eets[agent2]["Li
-0001d2b0: 6162 696c 6974 6965 7320 616e 6420 4571  abilities and Eq
-0001d2c0: 7569 7479 225d 3a0d 0a20 2020 2020 2020  uity"]:..       
-0001d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2f0: 2063 6f6d 6269 6e65 645f 7368 6565 7473   combined_sheets
-0001d300: 5b61 6765 6e74 325d 5b22 4c69 6162 696c  [agent2]["Liabil
-0001d310: 6974 6965 7320 616e 6420 4571 7569 7479  ities and Equity
-0001d320: 225d 5b6e 616d 655d 203d 2022 220d 0a0d  "][name] = ""...
-0001d330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d350: 2020 2020 2063 6f6d 6269 6e65 645f 7368       combined_sh
-0001d360: 6565 7473 5b61 6765 6e74 325d 5b22 4c69  eets[agent2]["Li
-0001d370: 6162 696c 6974 6965 7320 616e 6420 4571  abilities and Eq
-0001d380: 7569 7479 225d 5b6e 616d 655d 202b 3d20  uity"][name] += 
-0001d390: 7120 2b20 7375 626a 6563 7420 2b20 225c  q + subject + "\
-0001d3a0: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
-0001d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3c0: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
-0001d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3f0: 2070 6173 730d 0a0d 0a20 2020 2020 2020   pass....       
+0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d230: 2020 2022 7175 616e 7469 7479 225d 2c74     "quantity"],t
+0001d240: 6974 6c65 3d22 4572 726f 7222 290d 0a0d  itle="Error")...
+0001d250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d270: 2020 2020 2073 7562 6a65 6374 203d 2022       subject = "
+0001d280: 2020 2028 2220 2b20 6669 6c65 6461 7461     (" + filedata
+0001d290: 5b22 7375 626a 6563 7422 5d2e 7265 706c  ["subject"].repl
+0001d2a0: 6163 6528 225f 222c 2022 2022 2920 2b20  ace("_", " ") + 
+0001d2b0: 2229 220d 0a0d 0a20 2020 2020 2020 2020  ")"....         
+0001d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d2d0: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
+0001d2e0: 6d65 206e 6f74 2069 6e20 636f 6d62 696e  me not in combin
+0001d2f0: 6564 5f73 6865 6574 735b 6167 656e 7432  ed_sheets[agent2
+0001d300: 5d5b 224c 6961 6269 6c69 7469 6573 2061  ]["Liabilities a
+0001d310: 6e64 2045 7175 6974 7922 5d3a 0d0a 2020  nd Equity"]:..  
+0001d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d340: 2020 2020 2020 636f 6d62 696e 6564 5f73        combined_s
+0001d350: 6865 6574 735b 6167 656e 7432 5d5b 224c  heets[agent2]["L
+0001d360: 6961 6269 6c69 7469 6573 2061 6e64 2045  iabilities and E
+0001d370: 7175 6974 7922 5d5b 6e61 6d65 5d20 3d20  quity"][name] = 
+0001d380: 2222 0d0a 0d0a 2020 2020 2020 2020 2020  ""....          
+0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3a0: 2020 2020 2020 2020 2020 636f 6d62 696e            combin
+0001d3b0: 6564 5f73 6865 6574 735b 6167 656e 7432  ed_sheets[agent2
+0001d3c0: 5d5b 224c 6961 6269 6c69 7469 6573 2061  ]["Liabilities a
+0001d3d0: 6e64 2045 7175 6974 7922 5d5b 6e61 6d65  nd Equity"][name
+0001d3e0: 5d20 2b3d 2071 202b 2073 7562 6a65 6374  ] += q + subject
+0001d3f0: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
 0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d410: 2020 2020 2069 6620 7374 7228 6669 6c65       if str(file
-0001d420: 6461 7461 5b22 696e 636f 6d65 3222 5d29  data["income2"])
-0001d430: 2021 3d20 274e 6f6e 6527 3a0d 0a20 2020   != 'None':..   
-0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d450: 2020 2020 2020 2020 2020 2020 206d 7964               myd
-0001d460: 6963 7420 3d20 7b22 4761 696e 223a 2022  ict = {"Gain": "
-0001d470: 4761 696e 7322 2c0d 0a20 2020 2020 2020  Gains",..       
-0001d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4a0: 2020 2022 4c6f 7373 223a 2022 4c6f 7373     "Loss": "Loss
-0001d4b0: 6573 222c 0d0a 2020 2020 2020 2020 2020  es",..          
-0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d410: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+0001d420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d440: 2020 2020 2020 7061 7373 0d0a 0d0a 2020        pass....  
+0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d460: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+0001d470: 2866 696c 6564 6174 615b 2269 6e63 6f6d  (filedata["incom
+0001d480: 6532 225d 2920 213d 2027 4e6f 6e65 273a  e2"]) != 'None':
+0001d490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4b0: 2020 6d79 6469 6374 203d 207b 2247 6169    mydict = {"Gai
+0001d4c0: 6e22 3a20 2247 6169 6e73 222c 0d0a 2020  n": "Gains",..  
 0001d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4e0: 2245 7870 656e 7365 223a 2022 4578 7065  "Expense": "Expe
-0001d4f0: 6e73 6573 222c 0d0a 2020 2020 2020 2020  nses",..        
-0001d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4f0: 2020 2020 2020 2020 224c 6f73 7322 3a20          "Loss": 
+0001d500: 224c 6f73 7365 7322 2c0d 0a20 2020 2020  "Losses",..     
 0001d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d520: 2020 2252 6576 656e 7565 223a 2022 5265    "Revenue": "Re
-0001d530: 7665 6e75 6573 222c 0d0a 2020 2020 2020  venues",..      
-0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d530: 2020 2020 2022 4578 7065 6e73 6522 3a20       "Expense": 
+0001d540: 2245 7870 656e 7365 7322 2c0d 0a20 2020  "Expenses",..   
 0001d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d560: 2020 2020 2254 6178 223a 2022 5461 7865      "Tax": "Taxe
-0001d570: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
-0001d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d590: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001d5a0: 4e6f 6e74 6178 2e20 5072 6f66 6974 223a  Nontax. Profit":
-0001d5b0: 2022 4e6f 6e74 6178 6162 6c65 2050 726f   "Nontaxable Pro
-0001d5c0: 6669 7473 222c 0d0a 2020 2020 2020 2020  fits",..        
+0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d570: 2020 2020 2020 2022 5265 7665 6e75 6522         "Revenue"
+0001d580: 3a20 2252 6576 656e 7565 7322 2c0d 0a20  : "Revenues",.. 
+0001d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5b0: 2020 2020 2020 2020 2022 5461 7822 3a20           "Tax": 
+0001d5c0: 2254 6178 6573 222c 0d0a 2020 2020 2020  "Taxes",..      
 0001d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5f0: 2020 224e 6f6e 7461 782e 204c 6f73 7322    "Nontax. Loss"
-0001d600: 3a20 224e 6f6e 7461 7861 626c 6520 4c6f  : "Nontaxable Lo
-0001d610: 7373 6573 222c 0d0a 2020 2020 2020 2020  sses",..        
+0001d5f0: 2020 2020 224e 6f6e 7461 782e 2050 726f      "Nontax. Pro
+0001d600: 6669 7422 3a20 224e 6f6e 7461 7861 626c  fit": "Nontaxabl
+0001d610: 6520 5072 6f66 6974 7322 2c0d 0a20 2020  e Profits",..   
 0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d640: 2020 224e 6f6e 2d4f 702e 2049 6e63 6f6d    "Non-Op. Incom
-0001d650: 6522 3a20 224e 6f6e 2d4f 7065 7261 7469  e": "Non-Operati
-0001d660: 6f6e 616c 2049 6e63 6f6d 6522 2c0d 0a20  onal Income",.. 
+0001d640: 2020 2020 2020 2022 4e6f 6e74 6178 2e20         "Nontax. 
+0001d650: 4c6f 7373 223a 2022 4e6f 6e74 6178 6162  Loss": "Nontaxab
+0001d660: 6c65 204c 6f73 7365 7322 2c0d 0a20 2020  le Losses",..   
 0001d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d690: 2020 2020 2020 2020 2022 496e 7465 7265           "Intere
-0001d6a0: 7374 223a 2022 496e 7465 7265 7374 2050  st": "Interest P
-0001d6b0: 6179 6d65 6e74 7322 7d0d 0a20 2020 2020  ayments"}..     
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 2020 2020 2020 2071 203d 2073             q = s
-0001d6e0: 796d 7079 2e6c 6174 6578 2873 796d 7079  ympy.latex(sympy
-0001d6f0: 2e73 696d 706c 6966 7928 7369 676e 202b  .simplify(sign +
-0001d700: 2066 696c 6564 6174 615b 2271 7561 6e74   filedata["quant
-0001d710: 6974 7922 5d29 2c20 6d6f 6465 3d22 696e  ity"]), mode="in
-0001d720: 6c69 6e65 2229 0d0a 2020 2020 2020 2020  line")..        
-0001d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d740: 2020 2020 2020 2020 7375 626a 6563 7420          subject 
-0001d750: 3d20 2220 2020 2822 202b 2066 696c 6564  = "   (" + filed
-0001d760: 6174 615b 2273 7562 6a65 6374 225d 2e72  ata["subject"].r
-0001d770: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
-0001d780: 202b 2022 2922 0d0a 2020 2020 2020 2020   + ")"..        
-0001d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7a0: 2020 2020 2020 2020 636f 6d62 696e 6564          combined
-0001d7b0: 5f69 6e63 6f6d 655b 6167 656e 7432 5d5b  _income[agent2][
-0001d7c0: 6d79 6469 6374 5b66 696c 6564 6174 615b  mydict[filedata[
-0001d7d0: 2269 6e63 6f6d 6532 225d 5d5d 2e61 7070  "income2"]]].app
-0001d7e0: 656e 6428 2873 7472 2871 292c 2073 7562  end((str(q), sub
-0001d7f0: 6a65 6374 2929 0d0a 0d0a 2020 2020 2020  ject))....      
-0001d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d810: 2020 2020 2020 2020 2020 2320 3d3d 3d3d            # ====
-0001d820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d830: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 2020 2020  ========....    
-0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d850: 2020 2020 2020 2020 7472 616e 7366 6572          transfer
-0001d860: 5f73 7472 203d 2022 220d 0a0d 0a20 2020  _str = ""....   
-0001d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d880: 2020 2020 2020 2020 2069 6620 636f 6e76           if conv
-0001d890: 6572 745f 626f 6f6c 2866 696c 6564 6174  ert_bool(filedat
-0001d8a0: 615b 226c 6f67 2074 7261 6e73 6163 7469  a["log transacti
-0001d8b0: 6f6e 225d 293a 0d0a 2020 2020 2020 2020  on"]):..        
-0001d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8d0: 2020 2020 2020 2020 7472 616e 7366 6572          transfer
-0001d8e0: 5f73 7472 203d 2022 5c6e 466c 6f77 3a7e  _str = "\nFlow:~
-0001d8f0: 2220 2b20 6669 6c65 6461 7461 5b22 6b69  " + filedata["ki
-0001d900: 6e64 225d 2e73 7472 6970 2829 2e72 6570  nd"].strip().rep
-0001d910: 6c61 6365 2822 2d3e 222c 0d0a 2020 2020  lace("->",..    
-0001d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d970: 2020 2020 2020 2020 2022 245c 5c72 6967           "$\\rig
-0001d980: 6874 6172 726f 7724 2229 202b 2022 267e  htarrow$") + "&~
-0001d990: 5c5c 5c5c 2220 2b20 225c 6e22 0d0a 2020  \\\\" + "\n"..  
+0001d690: 2020 2020 2020 2022 4e6f 6e2d 4f70 2e20         "Non-Op. 
+0001d6a0: 496e 636f 6d65 223a 2022 4e6f 6e2d 4f70  Income": "Non-Op
+0001d6b0: 6572 6174 696f 6e61 6c20 496e 636f 6d65  erational Income
+0001d6c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+0001d6f0: 6e74 6572 6573 7422 3a20 2249 6e74 6572  nterest": "Inter
+0001d700: 6573 7420 5061 796d 656e 7473 227d 0d0a  est Payments"}..
+0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d730: 7120 3d20 7379 6d70 792e 6c61 7465 7828  q = sympy.latex(
+0001d740: 7379 6d70 792e 7369 6d70 6c69 6679 2873  sympy.simplify(s
+0001d750: 6967 6e20 2b20 6669 6c65 6461 7461 5b22  ign + filedata["
+0001d760: 7175 616e 7469 7479 225d 292c 206d 6f64  quantity"]), mod
+0001d770: 653d 2269 6e6c 696e 6522 290d 0a20 2020  e="inline")..   
+0001d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d790: 2020 2020 2020 2020 2020 2020 2073 7562               sub
+0001d7a0: 6a65 6374 203d 2022 2020 2028 2220 2b20  ject = "   (" + 
+0001d7b0: 6669 6c65 6461 7461 5b22 7375 626a 6563  filedata["subjec
+0001d7c0: 7422 5d2e 7265 706c 6163 6528 225f 222c  t"].replace("_",
+0001d7d0: 2022 2022 2920 2b20 2229 220d 0a20 2020   " ") + ")"..   
+0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7f0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+0001d800: 6269 6e65 645f 696e 636f 6d65 5b61 6765  bined_income[age
+0001d810: 6e74 325d 5b6d 7964 6963 745b 6669 6c65  nt2][mydict[file
+0001d820: 6461 7461 5b22 696e 636f 6d65 3222 5d5d  data["income2"]]
+0001d830: 5d2e 6170 7065 6e64 2828 7374 7228 7129  ].append((str(q)
+0001d840: 2c20 7375 626a 6563 7429 290d 0a0d 0a20  , subject)).... 
+0001d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001d870: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+0001d880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d  =============...
+0001d890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d8a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0001d8b0: 6e73 6665 725f 7374 7220 3d20 2222 0d0a  nsfer_str = ""..
+0001d8c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d8d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d8e0: 2063 6f6e 7665 7274 5f62 6f6f 6c28 6669   convert_bool(fi
+0001d8f0: 6c65 6461 7461 5b22 6c6f 6720 7472 616e  ledata["log tran
+0001d900: 7361 6374 696f 6e22 5d29 3a0d 0a20 2020  saction"]):..   
+0001d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d920: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0001d930: 6e73 6665 725f 7374 7220 3d20 225c 6e46  nsfer_str = "\nF
+0001d940: 6c6f 773a 7e22 202b 2066 696c 6564 6174  low:~" + filedat
+0001d950: 615b 226b 696e 6422 5d2e 7374 7269 7028  a["kind"].strip(
+0001d960: 292e 7265 706c 6163 6528 222d 3e22 2c0d  ).replace("->",.
+0001d970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0001d9c0: 616e 7366 6572 5f73 7472 202b 3d20 2253  ansfer_str += "S
-0001d9d0: 7562 6a65 6374 3a7e 2220 2b20 6669 6c65  ubject:~" + file
-0001d9e0: 6461 7461 5b22 7375 626a 6563 7422 5d2e  data["subject"].
-0001d9f0: 7374 7269 7028 292e 7469 746c 6528 2920  strip().title() 
-0001da00: 2b20 2226 7e5c 5c5c 5c22 202b 2022 5c6e  + "&~\\\\" + "\n
-0001da10: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da30: 2020 2023 2074 7261 6e73 6665 725f 7374     # transfer_st
-0001da40: 7220 2b3d 2022 5175 616e 7469 7479 3a7e  r += "Quantity:~
-0001da50: 2220 2b20 6669 6c65 6461 7461 5b22 7175  " + filedata["qu
-0001da60: 616e 7469 7479 225d 2e73 7472 6970 2829  antity"].strip()
-0001da70: 202b 2022 267e 5c5c 5c5c 222b 2022 5c6e   + "&~\\\\"+ "\n
-0001da80: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
-0001da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001daa0: 2074 6162 6c65 5f73 7472 203d 2022 2222   table_str = """
-0001dab0: 5c5c 6265 6769 6e7b 7461 6275 6c61 727d  \\begin{tabular}
-0001dac0: 7b6c 6c7d 0d0a 0d0a 2020 2020 2020 2020  {ll}....        
-0001dad0: 2020 2020 2020 2020 2573 2026 2025 7320          %s & %s 
-0001dae0: 5c5c 5c5c 0d0a 2020 2020 2020 2020 2020  \\\\..          
-0001daf0: 2020 2020 2020 7e20 2620 7e20 5c5c 5c5c        ~ & ~ \\\\
-0001db00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001db10: 2020 2222 2220 2520 2866 696c 6564 6174    """ % (filedat
-0001db20: 615b 2261 6765 6e74 3122 5d2c 2066 696c  a["agent1"], fil
-0001db30: 6564 6174 615b 2261 6765 6e74 3222 5d29  edata["agent2"])
-0001db40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001db50: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0001db60: 626c 655f 7374 7220 2b3d 2074 6578 5f74  ble_str += tex_t
-0001db70: 6162 6c65 3120 2b20 2226 2220 2b20 7465  able1 + "&" + te
-0001db80: 785f 7461 626c 6532 202b 2022 5c5c 5c5c  x_table2 + "\\\\
-0001db90: 5c5c 5c5c 2220 2b20 7472 616e 7366 6572  \\\\" + transfer
-0001dba0: 5f73 7472 0d0a 0d0a 2020 2020 2020 2020  _str....        
-0001dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbc0: 2020 2020 7461 626c 655f 7374 7220 2b3d      table_str +=
-0001dbd0: 2022 5c6e 5c6e 5c5c 656e 647b 7461 6275   "\n\n\\end{tabu
-0001dbe0: 6c61 727d 220d 0a20 2020 2020 2020 2020  lar}"..         
-0001dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc00: 2020 2074 6578 7374 7220 2b3d 2022 2222     texstr += """
-0001dc10: 5c5c 6265 6769 6e7b 7461 626c 657d 5b48  \\begin{table}[H
-0001dc20: 5d5c 6e22 2222 0d0a 2020 2020 2020 2020  ]\n"""..        
-0001dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc40: 2020 2020 7465 7873 7472 202b 3d20 7461      texstr += ta
-0001dc50: 626c 655f 7374 720d 0a20 2020 2020 2020  ble_str..       
-0001dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc70: 2020 2020 2074 6578 7374 7220 2b3d 2022       texstr += "
-0001dc80: 2222 5c63 6170 7469 6f6e 7b25 737d 5c6e  ""\caption{%s}\n
-0001dc90: 5c65 6e64 7b74 6162 6c65 7d22 2222 2025  \end{table}""" %
-0001dca0: 2028 6669 6c65 6461 7461 5b22 7375 626a   (filedata["subj
-0001dcb0: 6563 7422 5d20 2b20 2228 2573 2922 2566  ect"] + "(%s)"%f
-0001dcc0: 696c 6564 6174 615b 2273 686f 7274 6e61  iledata["shortna
-0001dcd0: 6d65 225d 290d 0a0d 0a20 2020 2020 2020  me"])....       
-0001dce0: 2020 2020 2074 6578 7374 7220 3d20 7465       texstr = te
-0001dcf0: 7873 7472 2e72 6570 6c61 6365 2822 5f22  xstr.replace("_"
-0001dd00: 2c20 2220 2229 0d0a 2020 2020 2020 2020  , " ")..        
-0001dd10: 2020 2020 7465 7873 7472 203d 2074 6578      texstr = tex
-0001dd20: 7374 722e 7265 706c 6163 6528 224e 6f6e  str.replace("Non
-0001dd30: 6522 2c20 2222 290d 0a0d 0a20 2020 2020  e", "")....     
-0001dd40: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-0001dd50: 3d3d 3d3d 3d20 6164 6420 636f 6d62 696e  ===== add combin
-0001dd60: 6564 2073 6865 6574 7320 3d3d 3d3d 3d3d  ed sheets ======
-0001dd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001dd80: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0001dd90: 696e 7428 636f 6d62 696e 6564 5f73 6865  int(combined_she
-0001dda0: 6574 7329 0d0a 0d0a 2020 2020 2020 2020  ets)....        
-0001ddb0: 2020 2020 2320 7064 2e44 6174 6146 7261      # pd.DataFra
-0001ddc0: 6d65 2863 6f6d 6269 6e65 645f 7368 6565  me(combined_shee
-0001ddd0: 7473 292e 746f 5f65 7863 656c 2822 7465  ts).to_excel("te
-0001dde0: 7374 2e78 6c73 7822 2920 3c2d 2066 6f72  st.xlsx") <- for
-0001ddf0: 206d 616e 7561 6c20 7465 7374 696e 670d   manual testing.
-0001de00: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-0001de10: 2063 6f6e 7665 7274 2074 6865 2063 6f6d   convert the com
-0001de20: 6269 6e65 6420 7368 6565 7473 2074 6f20  bined sheets to 
-0001de30: 7465 780d 0a20 2020 2020 2020 2020 2020  tex..           
-0001de40: 2074 6578 7374 725f 636f 6d62 696e 6564   texstr_combined
-0001de50: 203d 2022 220d 0a20 2020 2020 2020 2020   = ""..         
-0001de60: 2020 2066 6f72 2061 6765 6e74 2c20 6461     for agent, da
-0001de70: 7461 2069 6e20 636f 6d62 696e 6564 5f73  ta in combined_s
-0001de80: 6865 6574 732e 6974 656d 7328 293a 0d0a  heets.items():..
-0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dea0: 6167 656e 745f 7469 746c 6564 203d 2061  agent_titled = a
-0001deb0: 6765 6e74 2e72 6570 6c61 6365 2822 5f22  gent.replace("_"
-0001dec0: 2c20 2220 2229 2e74 6974 6c65 2829 0d0a  , " ").title()..
-0001ded0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dee0: 2020 6173 7365 7473 203d 2064 6174 615b    assets = data[
-0001def0: 2241 7373 6574 7322 5d0d 0a20 2020 2020  "Assets"]..     
-0001df00: 2020 2020 2020 2020 2020 206c 6961 6273             liabs
-0001df10: 203d 2064 6174 615b 224c 6961 6269 6c69   = data["Liabili
-0001df20: 7469 6573 2061 6e64 2045 7175 6974 7922  ties and Equity"
-0001df30: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0001df40: 2020 2020 206d 7973 203d 2022 2222 0d0a       mys = """..
-0001df50: 2020 2020 2020 2020 2020 2020 5c5c 6265              \\be
-0001df60: 6769 6e7b 7461 626c 657d 5b48 5d0d 0a20  gin{table}[H].. 
-0001df70: 2020 2020 2020 2020 2020 205c 5c63 656e             \\cen
-0001df80: 7465 7269 6e67 0d0a 2020 2020 2020 2020  tering..        
-0001df90: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0001dfa0: 2020 2020 2020 2020 206d 7973 202b 3d20           mys += 
-0001dfb0: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
-0001dfc0: 205c 5c62 6567 696e 7b74 6162 756c 6172   \\begin{tabular
-0001dfd0: 7d7b 7c6c 7c6c 7c7d 0d0a 2020 2020 2020  }{|l|l|}..      
-0001dfe0: 2020 2020 2020 5c68 6c69 6e65 0d0a 2020        \hline..  
-0001dff0: 2020 2020 2020 2020 2020 7e26 7e5c 5c5c            ~&~\\\
-0001e000: 5c0d 0a20 2020 2020 2020 2020 2020 205c  \..            \
-0001e010: 5c74 6578 7462 667b 4173 7365 7473 7d20  \textbf{Assets} 
-0001e020: 2620 5c5c 7465 7874 6266 7b4c 6961 6269  & \\textbf{Liabi
-0001e030: 6c69 7469 6573 2061 6e64 2045 7175 6974  lities and Equit
-0001e040: 797d 5c5c 5c5c 0d0a 2020 2020 2020 2020  y}\\\\..        
-0001e050: 2020 2020 7e26 7e5c 5c5c 5c0d 0a0d 0a20      ~&~\\\\.... 
-0001e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e070: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-0001e080: 2020 2020 2020 2020 2020 2020 2020 6d79                my
-0001e090: 7320 2b3d 2022 2222 0d0a 2020 2020 2020  s += """..      
-0001e0a0: 2020 2020 2020 5c5c 6265 6769 6e7b 7461        \\begin{ta
-0001e0b0: 6275 6c61 727d 7b6c 6c7d 0d0a 2020 2020  bular}{ll}..    
-0001e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0d0: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
-0001e0e0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0001e0f0: 7465 6d2c 2065 6e74 7279 2069 6e20 6173  tem, entry in as
-0001e100: 7365 7473 2e69 7465 6d73 2829 3a0d 0a0d  sets.items():...
+0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9c0: 2020 2020 2020 2020 2020 2020 2020 2224                "$
+0001d9d0: 5c5c 7269 6768 7461 7272 6f77 2422 2920  \\rightarrow$") 
+0001d9e0: 2b20 2226 7e5c 5c5c 5c22 202b 2022 5c6e  + "&~\\\\" + "\n
+0001d9f0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da10: 2020 2074 7261 6e73 6665 725f 7374 7220     transfer_str 
+0001da20: 2b3d 2022 5375 626a 6563 743a 7e22 202b  += "Subject:~" +
+0001da30: 2066 696c 6564 6174 615b 2273 7562 6a65   filedata["subje
+0001da40: 6374 225d 2e73 7472 6970 2829 2e74 6974  ct"].strip().tit
+0001da50: 6c65 2829 202b 2022 267e 5c5c 5c5c 2220  le() + "&~\\\\" 
+0001da60: 2b20 225c 6e22 0d0a 2020 2020 2020 2020  + "\n"..        
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da80: 2020 2020 2020 2020 2320 7472 616e 7366          # transf
+0001da90: 6572 5f73 7472 202b 3d20 2251 7561 6e74  er_str += "Quant
+0001daa0: 6974 793a 7e22 202b 2066 696c 6564 6174  ity:~" + filedat
+0001dab0: 615b 2271 7561 6e74 6974 7922 5d2e 7374  a["quantity"].st
+0001dac0: 7269 7028 2920 2b20 2226 7e5c 5c5c 5c22  rip() + "&~\\\\"
+0001dad0: 2b20 225c 6e22 0d0a 0d0a 2020 2020 2020  + "\n"....      
+0001dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daf0: 2020 2020 2020 7461 626c 655f 7374 7220        table_str 
+0001db00: 3d20 2222 225c 5c62 6567 696e 7b74 6162  = """\\begin{tab
+0001db10: 756c 6172 7d7b 6c6c 7d0d 0a0d 0a20 2020  ular}{ll}....   
+0001db20: 2020 2020 2020 2020 2020 2020 2025 7320               %s 
+0001db30: 2620 2573 205c 5c5c 5c0d 0a20 2020 2020  & %s \\\\..     
+0001db40: 2020 2020 2020 2020 2020 207e 2026 207e             ~ & ~
+0001db50: 205c 5c5c 5c0d 0a20 2020 2020 2020 2020   \\\\..         
+0001db60: 2020 2020 2020 2022 2222 2025 2028 6669         """ % (fi
+0001db70: 6c65 6461 7461 5b22 6167 656e 7431 225d  ledata["agent1"]
+0001db80: 2c20 6669 6c65 6461 7461 5b22 6167 656e  , filedata["agen
+0001db90: 7432 225d 290d 0a20 2020 2020 2020 2020  t2"])..         
+0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbb0: 2020 2074 6162 6c65 5f73 7472 202b 3d20     table_str += 
+0001dbc0: 7465 785f 7461 626c 6531 202b 2022 2622  tex_table1 + "&"
+0001dbd0: 202b 2074 6578 5f74 6162 6c65 3220 2b20   + tex_table2 + 
+0001dbe0: 225c 5c5c 5c5c 5c5c 5c22 202b 2074 7261  "\\\\\\\\" + tra
+0001dbf0: 6e73 6665 725f 7374 720d 0a0d 0a20 2020  nsfer_str....   
+0001dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc10: 2020 2020 2020 2020 2074 6162 6c65 5f73           table_s
+0001dc20: 7472 202b 3d20 225c 6e5c 6e5c 5c65 6e64  tr += "\n\n\\end
+0001dc30: 7b74 6162 756c 6172 7d22 0d0a 2020 2020  {tabular}"..    
+0001dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc50: 2020 2020 2020 2020 7465 7873 7472 202b          texstr +
+0001dc60: 3d20 2222 225c 5c62 6567 696e 7b74 6162  = """\\begin{tab
+0001dc70: 6c65 7d5b 485d 5c6e 2222 220d 0a20 2020  le}[H]\n"""..   
+0001dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc90: 2020 2020 2020 2020 2074 6578 7374 7220           texstr 
+0001dca0: 2b3d 2074 6162 6c65 5f73 7472 0d0a 2020  += table_str..  
+0001dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dcc0: 2020 2020 2020 2020 2020 7465 7873 7472            texstr
+0001dcd0: 202b 3d20 2222 225c 6361 7074 696f 6e7b   += """\caption{
+0001dce0: 2573 7d5c 6e5c 656e 647b 7461 626c 657d  %s}\n\end{table}
+0001dcf0: 2222 2220 2520 2866 696c 6564 6174 615b  """ % (filedata[
+0001dd00: 2273 7562 6a65 6374 225d 202b 2022 2825  "subject"] + "(%
+0001dd10: 7329 2225 6669 6c65 6461 7461 5b22 7368  s)"%filedata["sh
+0001dd20: 6f72 746e 616d 6522 5d29 0d0a 0d0a 2020  ortname"])....  
+0001dd30: 2020 2020 2020 2020 2020 7465 7873 7472            texstr
+0001dd40: 203d 2074 6578 7374 722e 7265 706c 6163   = texstr.replac
+0001dd50: 6528 225f 222c 2022 2022 290d 0a20 2020  e("_", " ")..   
+0001dd60: 2020 2020 2020 2020 2074 6578 7374 7220           texstr 
+0001dd70: 3d20 7465 7873 7472 2e72 6570 6c61 6365  = texstr.replace
+0001dd80: 2822 4e6f 6e65 222c 2022 2229 0d0a 0d0a  ("None", "")....
+0001dd90: 2020 2020 2020 2020 2020 2020 2320 3d3d              # ==
+0001dda0: 3d3d 3d3d 3d3d 3d3d 3d3d 2061 6464 2063  ========== add c
+0001ddb0: 6f6d 6269 6e65 6420 7368 6565 7473 203d  ombined sheets =
+0001ddc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ddd0: 3d3d 3d3d 3d0d 0a20 2020 2020 2020 2020  =====..         
+0001dde0: 2020 2070 7269 6e74 2863 6f6d 6269 6e65     print(combine
+0001ddf0: 645f 7368 6565 7473 290d 0a0d 0a20 2020  d_sheets)....   
+0001de00: 2020 2020 2020 2020 2023 2070 642e 4461           # pd.Da
+0001de10: 7461 4672 616d 6528 636f 6d62 696e 6564  taFrame(combined
+0001de20: 5f73 6865 6574 7329 2e74 6f5f 6578 6365  _sheets).to_exce
+0001de30: 6c28 2274 6573 742e 786c 7378 2229 203c  l("test.xlsx") <
+0001de40: 2d20 666f 7220 6d61 6e75 616c 2074 6573  - for manual tes
+0001de50: 7469 6e67 0d0a 0d0a 2020 2020 2020 2020  ting....        
+0001de60: 2020 2020 2320 636f 6e76 6572 7420 7468      # convert th
+0001de70: 6520 636f 6d62 696e 6564 2073 6865 6574  e combined sheet
+0001de80: 7320 746f 2074 6578 0d0a 2020 2020 2020  s to tex..      
+0001de90: 2020 2020 2020 7465 7873 7472 5f63 6f6d        texstr_com
+0001dea0: 6269 6e65 6420 3d20 2222 0d0a 2020 2020  bined = ""..    
+0001deb0: 2020 2020 2020 2020 666f 7220 6167 656e          for agen
+0001dec0: 742c 2064 6174 6120 696e 2063 6f6d 6269  t, data in combi
+0001ded0: 6e65 645f 7368 6565 7473 2e69 7465 6d73  ned_sheets.items
+0001dee0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0001def0: 2020 2020 2061 6765 6e74 5f74 6974 6c65       agent_title
+0001df00: 6420 3d20 6167 656e 742e 7265 706c 6163  d = agent.replac
+0001df10: 6528 225f 222c 2022 2022 292e 7469 746c  e("_", " ").titl
+0001df20: 6528 290d 0a0d 0a20 2020 2020 2020 2020  e()....         
+0001df30: 2020 2020 2020 2061 7373 6574 7320 3d20         assets = 
+0001df40: 6461 7461 5b22 4173 7365 7473 225d 0d0a  data["Assets"]..
+0001df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df60: 6c69 6162 7320 3d20 6461 7461 5b22 4c69  liabs = data["Li
+0001df70: 6162 696c 6974 6965 7320 616e 6420 4571  abilities and Eq
+0001df80: 7569 7479 225d 0d0a 0d0a 2020 2020 2020  uity"]....      
+0001df90: 2020 2020 2020 2020 2020 6d79 7320 3d20            mys = 
+0001dfa0: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+0001dfb0: 205c 5c62 6567 696e 7b74 6162 6c65 7d5b   \\begin{table}[
+0001dfc0: 485d 0d0a 2020 2020 2020 2020 2020 2020  H]..            
+0001dfd0: 5c5c 6365 6e74 6572 696e 670d 0a20 2020  \\centering..   
+0001dfe0: 2020 2020 2020 2020 2022 2222 0d0a 2020           """..  
+0001dff0: 2020 2020 2020 2020 2020 2020 2020 6d79                my
+0001e000: 7320 2b3d 2022 2222 0d0a 2020 2020 2020  s += """..      
+0001e010: 2020 2020 2020 5c5c 6265 6769 6e7b 7461        \\begin{ta
+0001e020: 6275 6c61 727d 7b7c 6c7c 6c7c 7d0d 0a20  bular}{|l|l|}.. 
+0001e030: 2020 2020 2020 2020 2020 205c 686c 696e             \hlin
+0001e040: 650d 0a20 2020 2020 2020 2020 2020 207e  e..            ~
+0001e050: 267e 5c5c 5c5c 0d0a 2020 2020 2020 2020  &~\\\\..        
+0001e060: 2020 2020 5c5c 7465 7874 6266 7b41 7373      \\textbf{Ass
+0001e070: 6574 737d 2026 205c 5c74 6578 7462 667b  ets} & \\textbf{
+0001e080: 4c69 6162 696c 6974 6965 7320 616e 6420  Liabilities and 
+0001e090: 4571 7569 7479 7d5c 5c5c 5c0d 0a20 2020  Equity}\\\\..   
+0001e0a0: 2020 2020 2020 2020 207e 267e 5c5c 5c5c           ~&~\\\\
+0001e0b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001e0c0: 2020 2020 2020 2020 2020 2020 2222 220d              """.
+0001e0d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001e0e0: 2020 206d 7973 202b 3d20 2222 220d 0a20     mys += """.. 
+0001e0f0: 2020 2020 2020 2020 2020 205c 5c62 6567             \\beg
+0001e100: 696e 7b74 6162 756c 6172 7d7b 6c6c 7d0d  in{tabular}{ll}.
 0001e110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e120: 2020 2020 206d 7973 202b 3d20 6974 656d       mys += item
-0001e130: 202b 2022 267e 205c 5c5c 5c5c 686c 696e   + "&~ \\\\\hlin
-0001e140: 657e 267e 5c5c 5c5c 5c6e 220d 0a0d 0a20  e~&~\\\\\n".... 
-0001e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e160: 2020 2066 6f72 2073 7562 5f65 6e74 7279     for sub_entry
-0001e170: 2069 6e20 656e 7472 792e 7370 6c69 7428   in entry.split(
-0001e180: 225c 6e22 293a 0d0a 2020 2020 2020 2020  "\n"):..        
-0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1a0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0001e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1c0: 2020 6c74 5f73 7562 656e 7472 7920 3d20    lt_subentry = 
-0001e1d0: 7375 625f 656e 7472 790d 0a20 2020 2020  sub_entry..     
+0001e120: 2020 2020 2020 2020 2022 2222 0d0a 0d0a           """....
+0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e140: 666f 7220 6974 656d 2c20 656e 7472 7920  for item, entry 
+0001e150: 696e 2061 7373 6574 732e 6974 656d 7328  in assets.items(
+0001e160: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001e170: 2020 2020 2020 2020 2020 6d79 7320 2b3d            mys +=
+0001e180: 2069 7465 6d20 2b20 2226 7e20 5c5c 5c5c   item + "&~ \\\\
+0001e190: 5c68 6c69 6e65 7e26 7e5c 5c5c 5c5c 6e22  \hline~&~\\\\\n"
+0001e1a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001e1b0: 2020 2020 2020 2020 666f 7220 7375 625f          for sub_
+0001e1c0: 656e 7472 7920 696e 2065 6e74 7279 2e73  entry in entry.s
+0001e1d0: 706c 6974 2822 5c6e 2229 3a0d 0a20 2020  plit("\n"):..   
 0001e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1f0: 2020 2020 2020 206d 7973 202b 3d20 227e         mys += "~
-0001e200: 2622 202b 206c 745f 7375 6265 6e74 7279  &" + lt_subentry
-0001e210: 202b 2022 5c5c 5c5c 2220 2b20 225c 6e22   + "\\\\" + "\n"
-0001e220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e230: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0001e240: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001e250: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001e260: 6173 730d 0a0d 0a20 2020 2020 2020 2020  ass....         
-0001e270: 2020 2020 2020 206d 7973 202b 3d20 2222         mys += ""
-0001e280: 220d 0a20 2020 2020 2020 2020 2020 205c  "..            \
-0001e290: 656e 647b 7461 6275 6c61 727d 2026 205c  end{tabular} & \
-0001e2a0: 5c62 6567 696e 7b74 6162 756c 6172 7d7b  \begin{tabular}{
-0001e2b0: 6c6c 7d22 2222 202b 2022 5c6e 220d 0a0d  ll}""" + "\n"...
-0001e2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e2d0: 2066 6f72 2069 7465 6d2c 2065 6e74 7279   for item, entry
-0001e2e0: 2069 6e20 6c69 6162 732e 6974 656d 7328   in liabs.items(
-0001e2f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001e300: 2020 2020 2020 2020 6966 2069 7465 6d20          if item 
-0001e310: 213d 2022 4571 7569 7479 223a 0d0a 2020  != "Equity":..  
-0001e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e330: 2020 2020 2020 6d79 7320 2b3d 2069 7465        mys += ite
-0001e340: 6d20 2b20 2226 7e20 5c5c 5c5c 5c68 6c69  m + "&~ \\\\\hli
-0001e350: 6e65 7e26 7e5c 5c5c 5c5c 6e22 0d0a 0d0a  ne~&~\\\\\n"....
-0001e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e370: 2020 2020 2020 2020 666f 7220 7375 625f          for sub_
-0001e380: 656e 7472 7920 696e 2065 6e74 7279 2e73  entry in entry.s
-0001e390: 706c 6974 2822 5c6e 2229 3a0d 0a20 2020  plit("\n"):..   
-0001e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3b0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-0001e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001e3e0: 745f 7375 6265 6e74 7279 203d 2073 7562  t_subentry = sub
-0001e3f0: 5f65 6e74 7279 0d0a 2020 2020 2020 2020  _entry..        
-0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e410: 2020 2020 2020 2020 6d79 7320 2b3d 2022          mys += "
-0001e420: 7e26 2220 2b20 6c74 5f73 7562 656e 7472  ~&" + lt_subentr
-0001e430: 7920 2b20 225c 5c5c 5c22 202b 2022 5c6e  y + "\\\\" + "\n
-0001e440: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0001e450: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001e460: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
-0001e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e480: 2020 2020 2020 2020 7061 7373 0d0a 0d0a          pass....
-0001e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4a0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0001e4b0: 2020 2020 2020 2020 2020 6974 656d 203d            item =
-0001e4c0: 2022 4571 7569 7479 220d 0a20 2020 2020   "Equity"..     
-0001e4d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001e4e0: 6e74 7279 203d 206c 6961 6273 5b22 4571  ntry = liabs["Eq
-0001e4f0: 7569 7479 225d 0d0a 2020 2020 2020 2020  uity"]..        
-0001e500: 2020 2020 2020 2020 2020 2020 6d79 7320              mys 
-0001e510: 2b3d 2069 7465 6d20 2b20 2226 7e20 5c5c  += item + "&~ \\
-0001e520: 5c5c 5c68 6c69 6e65 7e26 7e5c 5c5c 5c5c  \\\hline~&~\\\\\
-0001e530: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
-0001e540: 2020 2020 2020 2020 2020 666f 7220 7375            for su
-0001e550: 625f 656e 7472 7920 696e 2065 6e74 7279  b_entry in entry
-0001e560: 2e73 706c 6974 2822 5c6e 2229 3a0d 0a20  .split("\n"):.. 
-0001e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e580: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-0001e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5a0: 2020 2020 2020 2020 206c 745f 7375 6265           lt_sube
-0001e5b0: 6e74 7279 203d 2073 7562 5f65 6e74 7279  ntry = sub_entry
-0001e5c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e5d0: 2020 2020 2020 2020 2020 2020 2020 6d79                my
-0001e5e0: 7320 2b3d 2022 7e26 2220 2b20 6c74 5f73  s += "~&" + lt_s
-0001e5f0: 7562 656e 7472 7920 2b20 225c 5c5c 5c22  ubentry + "\\\\"
-0001e600: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
-0001e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e620: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
-0001e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e640: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-0001e650: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0001e660: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-0001e670: 2020 2020 2020 2020 2070 6173 730d 0a0d           pass...
-0001e680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e690: 206d 7973 202b 3d20 2222 220d 0a20 2020   mys += """..   
-0001e6a0: 2020 2020 2020 2020 205c 5c65 6e64 7b74           \\end{t
-0001e6b0: 6162 756c 6172 7d0d 0a20 2020 2020 2020  abular}..       
-0001e6c0: 2020 2020 205c 5c5c 5c7e 267e 0d0a 2020       \\\\~&~..  
-0001e6d0: 2020 2020 2020 2020 2020 5c5c 5c5c 5c68            \\\\\h
-0001e6e0: 6c69 6e65 2222 220d 0a20 2020 2020 2020  line"""..       
-0001e6f0: 2020 2020 2020 2020 206d 7973 202b 3d20           mys += 
-0001e700: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
-0001e710: 205c 5c65 6e64 7b74 6162 756c 6172 7d22   \\end{tabular}"
-0001e720: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
-0001e730: 2020 2020 6d79 7320 2b3d 2022 2222 0d0a      mys += """..
-0001e740: 2020 2020 2020 2020 2020 2020 5c5c 6361              \\ca
-0001e750: 7074 696f 6e7b 4261 6c61 6e63 6520 5368  ption{Balance Sh
-0001e760: 6565 7420 6f66 2025 737d 2222 2220 2520  eet of %s}""" % 
-0001e770: 6167 656e 745f 7469 746c 6564 202b 2022  agent_titled + "
-0001e780: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
-0001e790: 5c5c 656e 647b 7461 626c 657d 0d0a 2020  \\end{table}..  
-0001e7a0: 2020 2020 2020 2020 2020 2222 220d 0a20            """.. 
-0001e7b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001e7c0: 6578 7374 725f 636f 6d62 696e 6564 202b  exstr_combined +
-0001e7d0: 3d20 6d79 730d 0a0d 0a20 2020 2020 2020  = mys....       
-0001e7e0: 2020 2020 2020 2020 2023 203d 3d3d 3d3d           # =====
-0001e7f0: 3d3d 3d3d 3d3d 2061 6464 2069 6e63 6f6d  ====== add incom
-0001e800: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-0001e810: 2020 2020 2069 6620 6167 656e 7420 696e       if agent in
-0001e820: 2063 6f6d 6269 6e65 645f 696e 636f 6d65   combined_income
-0001e830: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001e840: 2020 2020 2020 2069 6e63 6f6d 655f 6461         income_da
-0001e850: 7461 203d 2063 6f6d 6269 6e65 645f 696e  ta = combined_in
-0001e860: 636f 6d65 5b61 6765 6e74 5d0d 0a20 2020  come[agent]..   
-0001e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e880: 2069 6e63 6f6d 655f 7374 7220 3d20 2222   income_str = ""
-0001e890: 220d 0a20 2020 2020 2020 2020 2020 205c  "..            \
-0001e8a0: 5c62 6567 696e 7b74 6162 6c65 7d5b 485d  \begin{table}[H]
-0001e8b0: 5c6e 5c63 656e 7465 7269 6e67 5c6e 0d0a  \n\centering\n..
-0001e8c0: 2020 2020 2020 2020 2020 2020 5c5c 6265              \\be
-0001e8d0: 6769 6e7b 7461 6275 6c61 727d 7b7c 6c6c  gin{tabular}{|ll
-0001e8e0: 7c7d 5c6e 5c68 6c69 6e65 2222 220d 0a0d  |}\n\hline"""...
-0001e8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e900: 2020 2020 2066 6f72 206b 2069 6e20 2252       for k in "R
-0001e910: 6576 656e 7565 7322 2c20 2247 6169 6e73  evenues", "Gains
-0001e920: 222c 2022 4578 7065 6e73 6573 222c 2022  ", "Expenses", "
-0001e930: 4c6f 7373 6573 222c 205c 0d0a 2020 2020  Losses", \..    
-0001e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e950: 2020 2020 2020 2020 2022 496e 7465 7265           "Intere
-0001e960: 7374 2050 6179 6d65 6e74 7322 2c20 224e  st Payments", "N
-0001e970: 6f6e 2d4f 7065 7261 7469 6f6e 616c 2049  on-Operational I
-0001e980: 6e63 6f6d 6522 2c20 2254 6178 6573 222c  ncome", "Taxes",
-0001e990: 2022 4e6f 6e74 6178 6162 6c65 2050 726f   "Nontaxable Pro
-0001e9a0: 6669 7473 222c 2022 4e6f 6e74 6178 6162  fits", "Nontaxab
-0001e9b0: 6c65 204c 6f73 7365 7322 3a0d 0a20 2020  le Losses":..   
-0001e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9d0: 2020 2020 2076 203d 2069 6e63 6f6d 655f       v = income_
-0001e9e0: 6461 7461 5b6b 5d0d 0a0d 0a20 2020 2020  data[k]....     
-0001e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea00: 2020 2069 6e63 6f6d 655f 7374 7220 2b3d     income_str +=
-0001ea10: 2022 7e26 7e5c 5c5c 5c22 0d0a 2020 2020   "~&~\\\\"..    
-0001ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea30: 2020 2020 696e 636f 6d65 5f73 7472 202b      income_str +
-0001ea40: 3d20 225c 7422 202b 206b 202b 2022 267e  = "\t" + k + "&~
-0001ea50: 5c5c 5c5c 5c6e 220d 0a0d 0a20 2020 2020  \\\\\n"....     
-0001ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea70: 2020 2066 6f72 2073 7562 5f76 616c 7565     for sub_value
-0001ea80: 2069 6e20 763a 0d0a 2020 2020 2020 2020   in v:..        
-0001ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eaa0: 2020 2020 696e 636f 6d65 5f73 7472 202b      income_str +
-0001eab0: 3d20 225c 7422 202b 2022 7e26 2220 2b20  = "\t" + "~&" + 
-0001eac0: 7375 625f 7661 6c75 655b 305d 202b 2073  sub_value[0] + s
-0001ead0: 7562 5f76 616c 7565 5b31 5d20 2b20 225c  ub_value[1] + "\
-0001eae0: 5c5c 5c5c 6e22 0d0a 2020 2020 2020 2020  \\\\n"..        
-0001eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb00: 6966 206c 656e 2876 2920 3d3d 2030 3a0d  if len(v) == 0:.
-0001eb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001eb20: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
-0001eb30: 6f6d 655f 7374 7220 2b3d 2022 5c74 2220  ome_str += "\t" 
-0001eb40: 2b20 227e 2622 202b 2022 2e2d 2220 2b20  + "~&" + ".-" + 
-0001eb50: 225c 5c5c 5c5c 6e22 0d0a 0d0a 2020 2020  "\\\\\n"....    
-0001eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb70: 2020 2020 6966 206b 2021 3d20 224e 6f6e      if k != "Non
-0001eb80: 7461 7861 626c 6520 4c6f 7373 6573 223a  taxable Losses":
-0001eb90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001eba0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0001ebb0: 636f 6d65 5f73 7472 202b 3d20 227e 267e  come_str += "~&~
-0001ebc0: 5c5c 5c5c 5c68 6c69 6e65 5c6e 220d 0a0d  \\\\\hline\n"...
-0001ebd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ebe0: 2020 2020 2069 6e63 6f6d 655f 7374 7220       income_str 
-0001ebf0: 2b3d 2022 2222 5c6e 0d0a 2020 2020 2020  += """\n..      
-0001ec00: 2020 2020 2020 7e26 7e5c 5c5c 5c5c 686c        ~&~\\\\\hl
-0001ec10: 696e 655c 6e5c 5c65 6e64 7b74 6162 756c  ine\n\\end{tabul
-0001ec20: 6172 7d22 2222 0d0a 2020 2020 2020 2020  ar}"""..        
-0001ec30: 2020 2020 2020 2020 2020 2020 696e 636f              inco
-0001ec40: 6d65 5f73 7472 202b 3d20 2222 225c 6e0d  me_str += """\n.
-0001ec50: 0a20 2020 2020 2020 2020 2020 205c 5c63  .            \\c
-0001ec60: 6170 7469 6f6e 7b49 6e63 6f6d 6520 5374  aption{Income St
-0001ec70: 6174 656d 656e 7420 6f66 2025 737d 2222  atement of %s}""
-0001ec80: 2220 2520 6167 656e 745f 7469 746c 6564  " % agent_titled
-0001ec90: 202b 2022 2222 0d0a 2020 2020 2020 2020   + """..        
-0001eca0: 2020 2020 5c5c 656e 647b 7461 626c 657d      \\end{table}
-0001ecb0: 2222 220d 0a0d 0a20 2020 2020 2020 2020  """....         
-0001ecc0: 2020 2020 2020 2020 2020 2074 6578 7374             texst
-0001ecd0: 725f 636f 6d62 696e 6564 202b 3d20 696e  r_combined += in
-0001ece0: 636f 6d65 5f73 7472 0d0a 0d0a 2020 2020  come_str....    
-0001ecf0: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
-0001ed00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ed10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ed20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ed30: 3d0d 0a20 2020 2020 2020 2020 2020 2070  =..            p
-0001ed40: 7970 6572 636c 6970 2e63 6f70 7928 7465  yperclip.copy(te
-0001ed50: 7873 7472 5f63 6f6d 6269 6e65 6429 0d0a  xstr_combined)..
-0001ed60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001ed70: 2e6e 6f74 6966 7928 6d65 7373 6167 653d  .notify(message=
-0001ed80: 224c 6154 6558 2063 6f64 6520 636f 7069  "LaTeX code copi
-0001ed90: 6564 2074 6f20 636c 6970 626f 6172 642e  ed to clipboard.
-0001eda0: 2048 6176 6520 6675 6e21 222c 2074 6974   Have fun!", tit
-0001edb0: 6c65 3d22 4861 7665 2066 756e 2229 0d0a  le="Have fun")..
-0001edc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001edd0: 2046 616c 7365 3a20 2320 6465 7072 6563   False: # deprec
-0001ede0: 6961 7465 640d 0a0d 0a20 2020 2020 2020  iated....       
-0001edf0: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
-0001ee00: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0001ee10: 6f73 2e70 6174 682e 6162 7370 6174 6828  os.path.abspath(
-0001ee20: 5f5f 6669 6c65 5f5f 2929 0d0a 2020 2020  __file__))..    
-0001ee30: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0001ee40: 206f 7065 6e28 6f73 2e70 6174 682e 6a6f   open(os.path.jo
-0001ee50: 696e 2870 6174 6820 2c20 2266 696c 6573  in(path , "files
-0001ee60: 2f69 6e63 6f6d 655f 7374 6174 6d65 6e74  /income_statment
-0001ee70: 732e 7465 7822 292c 2022 7722 2920 6173  s.tex"), "w") as
-0001ee80: 2066 696c 653a 0d0a 2020 2020 2020 2020   file:..        
-0001ee90: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-0001eea0: 2e77 7269 7465 2822 2222 0d0a 2020 2020  .write("""..    
-0001eeb0: 5c64 6f63 756d 656e 7463 6c61 7373 7b61  \documentclass{a
-0001eec0: 7274 6963 6c65 7d0d 0a20 2020 205c 5c75  rticle}..    \\u
-0001eed0: 7365 7061 636b 6167 657b 7461 6275 6c61  sepackage{tabula
-0001eee0: 7278 7d0d 0a20 2020 205c 5c75 7365 7061  rx}..    \\usepa
-0001eef0: 636b 6167 657b 616d 736d 6174 687d 0d0a  ckage{amsmath}..
-0001ef00: 2020 2020 5c5c 7573 6570 6163 6b61 6765      \\usepackage
-0001ef10: 7b66 6c6f 6174 7d0d 0a0d 0a20 2020 205c  {float}....    \
-0001ef20: 5c62 6567 696e 7b64 6f63 756d 656e 747d  \begin{document}
-0001ef30: 0d0a 0d0a 2020 2020 2222 2229 0d0a 2020  ....    """)..  
-0001ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef50: 2020 6669 6c65 2e77 7269 7465 2874 6578    file.write(tex
-0001ef60: 7374 725f 636f 6d62 696e 6564 290d 0a20  str_combined).. 
-0001ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef80: 2020 2066 696c 652e 7772 6974 6528 2222     file.write(""
-0001ef90: 220d 0a20 2020 205c 5c65 6e64 7b64 6f63  "..    \\end{doc
-0001efa0: 756d 656e 747d 0d0a 2020 2020 2222 2229  ument}..    """)
-0001efb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001efc0: 2020 2020 696d 706f 7274 2073 7562 7072      import subpr
-0001efd0: 6f63 6573 730d 0a20 2020 2020 2020 2020  ocess..         
-0001efe0: 2020 2020 2020 2074 7279 3a0d 0a0d 0a20         try:.... 
-0001eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f000: 2020 2070 6174 6820 3d20 6f73 2e70 6174     path = os.pat
-0001f010: 682e 6469 726e 616d 6528 6f73 2e70 6174  h.dirname(os.pat
-0001f020: 682e 6162 7370 6174 6828 5f5f 6669 6c65  h.abspath(__file
-0001f030: 5f5f 2929 0d0a 2020 2020 2020 2020 2020  __))..          
-0001f040: 2020 2020 2020 2020 2020 7375 6270 726f            subpro
-0001f050: 6365 7373 2e72 756e 2822 7064 666c 6174  cess.run("pdflat
-0001f060: 6578 2025 7322 2025 2028 6f73 2e70 6174  ex %s" % (os.pat
-0001f070: 682e 6a6f 696e 2870 6174 682c 2022 6669  h.join(path, "fi
-0001f080: 6c65 732f 696e 636f 6d65 5f73 7461 746d  les/income_statm
-0001f090: 656e 7473 2e74 6578 2229 2929 2e63 6865  ents.tex"))).che
-0001f0a0: 636b 5f72 6574 7572 6e63 6f64 6528 290d  ck_returncode().
-0001f0b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001f0c0: 2020 2020 2020 2073 6875 7469 6c2e 6d6f         shutil.mo
-0001f0d0: 7665 2870 6174 6820 2b20 2269 6e63 6f6d  ve(path + "incom
-0001f0e0: 655f 7374 6174 6d65 6e74 732e 7465 7822  e_statments.tex"
-0001f0f0: 2c20 7061 7468 202b 2022 6669 6c65 735c  , path + "files\
-0001f100: 5c69 6e63 6f6d 655f 7374 6174 6d65 6e74  \income_statment
-0001f110: 732e 7465 7822 290d 0a20 2020 2020 2020  s.tex")..       
-0001f120: 2020 2020 2020 2020 2020 2020 2073 6875               shu
-0001f130: 7469 6c2e 6d6f 7665 2870 6174 6820 2b20  til.move(path + 
-0001f140: 2269 6e63 6f6d 655f 7374 6174 6d65 6e74  "income_statment
-0001f150: 732e 6c6f 6722 2c20 7061 7468 202b 2022  s.log", path + "
-0001f160: 6669 6c65 735c 5c69 6e63 6f6d 655f 7374  files\\income_st
-0001f170: 6174 6d65 6e74 732e 6c6f 6722 290d 0a20  atments.log").. 
-0001f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f190: 2020 2073 6875 7469 6c2e 6d6f 7665 2870     shutil.move(p
-0001f1a0: 6174 6820 2b20 2269 6e63 6f6d 655f 7374  ath + "income_st
-0001f1b0: 6174 6d65 6e74 732e 6175 7822 2c20 7061  atments.aux", pa
-0001f1c0: 7468 202b 2022 6669 6c65 735c 5c5c 6d69  th + "files\\\mi
-0001f1d0: 6e63 6f6d 655f 7374 6174 6d65 6e74 732e  ncome_statments.
-0001f1e0: 6175 7822 290d 0a20 2020 2020 2020 2020  aux")..         
-0001f1f0: 2020 2020 2020 2020 2020 2073 6875 7469             shuti
-0001f200: 6c2e 6d6f 7665 2870 6174 6820 2b20 2269  l.move(path + "i
-0001f210: 6e63 6f6d 655f 7374 6174 6d65 6e74 732e  ncome_statments.
-0001f220: 7064 6622 2c20 7061 7468 202b 2022 6669  pdf", path + "fi
-0001f230: 6c65 735c 5c69 6e63 6f6d 655f 7374 6174  les\\income_stat
-0001f240: 6d65 6e74 732e 7064 6622 290d 0a20 2020  ments.pdf")..   
-0001f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f260: 2073 656c 662e 6e6f 7469 6679 286d 6573   self.notify(mes
-0001f270: 7361 6765 3d22 5465 5820 4669 6c65 2063  sage="TeX File c
-0001f280: 7265 6174 6564 2069 6e20 2573 2220 2520  reated in %s" % 
-0001f290: 7061 7468 202b 2022 5c5c 6669 6c65 7322  path + "\\files"
-0001f2a0: 202c 7469 746c 653d 2253 7563 6365 7373   ,title="Success
-0001f2b0: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
-0001f2c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0001f2d0: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-0001f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f2f0: 2020 7365 6c66 2e6e 6f74 6966 7928 6d65    self.notify(me
-0001f300: 7373 6167 653d 7374 7228 652e 5f5f 636f  ssage=str(e.__co
-0001f310: 6e74 6578 745f 5f29 202b 2022 5c6e 2220  ntext__) + "\n" 
-0001f320: 2b20 7374 7228 6529 2c20 7469 746c 653d  + str(e), title=
-0001f330: 652e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  e.__class__.__na
-0001f340: 6d65 5f5f 290d 0a0d 0a0d 0a20 2020 2020  me__)......     
-0001f350: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0001f360: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-0001f370: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
-0001f380: 6679 286d 6573 7361 6765 3d73 7472 2865  fy(message=str(e
-0001f390: 2e5f 5f63 6f6e 7465 7874 5f5f 2920 2b20  .__context__) + 
-0001f3a0: 225c 6e22 202b 2073 7472 2865 292c 2074  "\n" + str(e), t
-0001f3b0: 6974 6c65 3d65 2e5f 5f63 6c61 7373 5f5f  itle=e.__class__
-0001f3c0: 2e5f 5f6e 616d 655f 5f29 0d0a 0d0a 2020  .__name__)....  
-0001f3d0: 2020 6465 6620 6164 645f 6865 6c70 6572    def add_helper
-0001f3e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-0001f3f0: 206e 6577 5f6e 616d 6520 3d20 7365 6c66   new_name = self
-0001f400: 2e48 656c 7065 724e 616d 6545 6469 742e  .HelperNameEdit.
-0001f410: 7465 7874 2829 0d0a 2020 2020 2020 2020  text()..        
-0001f420: 2320 544f 444f 2061 6464 2073 6563 7572  # TODO add secur
-0001f430: 6974 7920 6d65 6368 616e 6973 6d20 746f  ity mechanism to
-0001f440: 2061 766f 6964 206f 7665 7277 7269 7469   avoid overwriti
-0001f450: 6e67 2061 6e20 6167 656e 740d 0a20 2020  ng an agent..   
-0001f460: 2020 2020 2069 6620 6e65 775f 6e61 6d65       if new_name
-0001f470: 203d 3d20 2222 3a0d 0a20 2020 2020 2020   == "":..       
-0001f480: 2020 2020 2073 656c 662e 6e6f 7469 6679       self.notify
-0001f490: 2822 506c 6561 7365 2065 6e74 6572 2061  ("Please enter a
-0001f4a0: 2076 616c 6964 206e 616d 6522 2c20 7469   valid name", ti
-0001f4b0: 746c 653d 2249 424d 2045 7272 6f72 2229  tle="IBM Error")
-0001f4c0: 0d0a 2020 2020 2020 2020 656c 6966 206e  ..        elif n
-0001f4d0: 6f74 206e 6577 5f6e 616d 655b 305d 2e69  ot new_name[0].i
-0001f4e0: 7375 7070 6572 2829 3a0d 0a20 2020 2020  supper():..     
-0001f4f0: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
-0001f500: 6679 2822 506c 6561 7365 2065 6e74 6572  fy("Please enter
-0001f510: 2061 2076 616c 6964 206e 616d 6520 7769   a valid name wi
-0001f520: 7468 5c6e 7570 7065 7263 6173 6520 6669  th\nuppercase fi
-0001f530: 7273 7420 6c65 7474 6572 206f 7220 6361  rst letter or ca
-0001f540: 6d65 6c63 6173 652c 2065 2e67 2e20 274d  melcase, e.g. 'M
-0001f550: 7941 6765 6e74 2722 2c20 7469 746c 653d  yAgent'", title=
-0001f560: 2249 424d 2045 7272 6f72 2229 0d0a 2020  "IBM Error")..  
-0001f570: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0001f580: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
-0001f590: 6177 6361 6e76 6173 2e61 6464 5f61 6765  awcanvas.add_age
-0001f5a0: 6e74 286e 6577 5f6e 616d 6529 0d0a 0d0a  nt(new_name)....
-0001f5b0: 2020 2020 6465 6620 7265 6d6f 7665 5f68      def remove_h
-0001f5c0: 656c 7065 7228 7365 6c66 293a 0d0a 2020  elper(self):..  
-0001f5d0: 2020 2020 2020 7365 6c66 2e64 7261 7763        self.drawc
-0001f5e0: 616e 7661 732e 7265 6d6f 7665 5f61 6765  anvas.remove_age
-0001f5f0: 6e74 2829 0d0a 0d0a 2020 2020 6465 6620  nt()....    def 
-0001f600: 6164 645f 6e65 7728 7365 6c66 293a 0d0a  add_new(self):..
-0001f610: 0d0a 2020 2020 2020 2020 2320 544f 444f  ..        # TODO
-0001f620: 2061 7373 6572 7420 7468 6174 2071 7561   assert that qua
-0001f630: 6e74 6974 7920 6973 206e 6f74 2079 6574  ntity is not yet
-0001f640: 2069 6e20 616e 7920 6f74 6865 7220 7472   in any other tr
-0001f650: 616e 7361 6374 696f 6e0d 0a20 2020 2020  ansaction..     
-0001f660: 2020 2073 656c 662e 6d61 6465 5f63 6861     self.made_cha
-0001f670: 6e67 6573 203d 2046 616c 7365 0d0a 0d0a  nges = False....
-0001f680: 0d0a 2020 2020 2020 2020 6e65 775f 656e  ..        new_en
-0001f690: 7472 7920 3d20 7b7d 0d0a 0d0a 2020 2020  try = {}....    
-0001f6a0: 2020 2020 6e65 775f 656e 7472 795b 2261      new_entry["a
-0001f6b0: 3122 5d20 3d20 7365 6c66 2e41 7373 6574  1"] = self.Asset
-0001f6c0: 4c69 7374 4c65 6674 2e74 6f50 6c61 696e  ListLeft.toPlain
-0001f6d0: 5465 7874 2829 0d0a 2020 2020 2020 2020  Text()..        
-0001f6e0: 6e65 775f 656e 7472 795b 2261 3222 5d20  new_entry["a2"] 
-0001f6f0: 3d20 7365 6c66 2e41 7373 6574 4c69 7374  = self.AssetList
-0001f700: 5269 6768 742e 746f 506c 6169 6e54 6578  Right.toPlainTex
-0001f710: 7428 290d 0a20 2020 2020 2020 206e 6577  t()..        new
-0001f720: 5f65 6e74 7279 5b22 6c31 225d 203d 2073  _entry["l1"] = s
-0001f730: 656c 662e 4c69 6162 696c 6974 794c 6973  elf.LiabilityLis
-0001f740: 744c 6566 742e 746f 506c 6169 6e54 6578  tLeft.toPlainTex
-0001f750: 7428 290d 0a20 2020 2020 2020 206e 6577  t()..        new
-0001f760: 5f65 6e74 7279 5b22 6c32 225d 203d 2073  _entry["l2"] = s
-0001f770: 656c 662e 4c69 6162 696c 6974 794c 6973  elf.LiabilityLis
-0001f780: 7452 6967 6874 2e74 6f50 6c61 696e 5465  tRight.toPlainTe
-0001f790: 7874 2829 0d0a 2020 2020 2020 2020 6e65  xt()..        ne
-0001f7a0: 775f 656e 7472 795b 2265 3122 5d20 3d20  w_entry["e1"] = 
-0001f7b0: 7365 6c66 2e45 7175 6974 794c 6973 744c  self.EquityListL
-0001f7c0: 6566 742e 746f 506c 6169 6e54 6578 7428  eft.toPlainText(
-0001f7d0: 290d 0a20 2020 2020 2020 206e 6577 5f65  )..        new_e
-0001f7e0: 6e74 7279 5b22 6532 225d 203d 2073 656c  ntry["e2"] = sel
-0001f7f0: 662e 4571 7569 7479 4c69 7374 5269 6768  f.EquityListRigh
-0001f800: 742e 746f 506c 6169 6e54 6578 7428 290d  t.toPlainText().
-0001f810: 0a0d 0a20 2020 2020 2020 2023 206e 6577  ...        # new
-0001f820: 5f65 6e74 7279 5b22 6131 225d 203d 2073  _entry["a1"] = s
-0001f830: 656c 662e 4173 7365 744c 6973 744c 6566  elf.AssetListLef
-0001f840: 742e 746f 506c 6169 6e54 6578 7428 290d  t.toPlainText().
-0001f850: 0a20 2020 2020 2020 2023 206e 6577 5f65  .        # new_e
-0001f860: 6e74 7279 5b22 6c31 225d 203d 2073 656c  ntry["l1"] = sel
-0001f870: 662e 4c69 6162 696c 6974 794c 6973 744c  f.LiabilityListL
-0001f880: 6566 742e 746f 506c 6169 6e54 6578 7428  eft.toPlainText(
-0001f890: 290d 0a20 2020 2020 2020 2023 206e 6577  )..        # new
-0001f8a0: 5f65 6e74 7279 5b22 6132 225d 203d 2073  _entry["a2"] = s
-0001f8b0: 656c 662e 4c69 6162 696c 6974 794c 6973  elf.LiabilityLis
-0001f8c0: 7452 6967 6874 2e74 6f50 6c61 696e 5465  tRight.toPlainTe
-0001f8d0: 7874 2829 0d0a 2020 2020 2020 2020 2320  xt()..        # 
-0001f8e0: 6e65 775f 656e 7472 795b 226c 3222 5d20  new_entry["l2"] 
-0001f8f0: 3d20 7365 6c66 2e41 7373 6574 4c69 7374  = self.AssetList
-0001f900: 5269 6768 742e 746f 506c 6169 6e54 6578  Right.toPlainTex
-0001f910: 7428 290d 0a20 2020 2020 2020 2023 206e  t()..        # n
-0001f920: 6577 5f65 6e74 7279 5b22 6531 225d 203d  ew_entry["e1"] =
-0001f930: 2073 656c 662e 4571 7569 7479 4c69 7374   self.EquityList
-0001f940: 4c65 6674 2e74 6f50 6c61 696e 5465 7874  Left.toPlainText
-0001f950: 2829 0d0a 2020 2020 2020 2020 2320 6e65  ()..        # ne
-0001f960: 775f 656e 7472 795b 2265 3222 5d20 3d20  w_entry["e2"] = 
-0001f970: 7365 6c66 2e45 7175 6974 794c 6973 7452  self.EquityListR
-0001f980: 6967 6874 2e74 6f50 6c61 696e 5465 7874  ight.toPlainText
-0001f990: 2829 0d0a 0d0a 2020 2020 2020 2020 6e65  ()....        ne
-0001f9a0: 775f 656e 7472 795b 2261 6765 6e74 3122  w_entry["agent1"
-0001f9b0: 5d20 3d20 6361 6d65 6c28 7365 6c66 2e61  ] = camel(self.a
-0001f9c0: 6765 6e74 3145 6469 742e 7465 7874 2829  gent1Edit.text()
-0001f9d0: 2920 232e 6361 7069 7461 6c69 7a65 2829  ) #.capitalize()
-0001f9e0: 0d0a 2020 2020 2020 2020 6e65 775f 656e  ..        new_en
-0001f9f0: 7472 795b 2261 6765 6e74 3222 5d20 3d20  try["agent2"] = 
-0001fa00: 6361 6d65 6c28 7365 6c66 2e61 6765 6e74  camel(self.agent
-0001fa10: 3245 6469 742e 7465 7874 2829 2920 232e  2Edit.text()) #.
-0001fa20: 6361 7069 7461 6c69 7a65 2829 0d0a 0d0a  capitalize()....
-0001fa30: 2020 2020 2020 2020 7365 6c66 2e61 6765          self.age
-0001fa40: 6e74 3145 6469 742e 7365 7454 6578 7428  nt1Edit.setText(
-0001fa50: 6361 6d65 6c28 7365 6c66 2e61 6765 6e74  camel(self.agent
-0001fa60: 3145 6469 742e 7465 7874 2829 2929 2023  1Edit.text())) #
-0001fa70: 202e 6361 7069 7461 6c69 7a65 2829 290d   .capitalize()).
-0001fa80: 0a20 2020 2020 2020 2073 656c 662e 6167  .        self.ag
-0001fa90: 656e 7432 4564 6974 2e73 6574 5465 7874  ent2Edit.setText
-0001faa0: 2863 616d 656c 2873 656c 662e 6167 656e  (camel(self.agen
-0001fab0: 7432 4564 6974 2e74 6578 7428 2929 2920  t2Edit.text())) 
-0001fac0: 232e 6361 7069 7461 6c69 7a65 2829 290d  #.capitalize()).
-0001fad0: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
-0001fae0: 7420 7365 6c66 2e64 7261 7763 616e 7661  t self.drawcanva
-0001faf0: 732e 6368 6563 6b5f 6578 6973 7428 6e65  s.check_exist(ne
-0001fb00: 775f 656e 7472 795b 2261 6765 6e74 3122  w_entry["agent1"
-0001fb10: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-0001fb20: 2069 6620 6e65 775f 656e 7472 795b 2261   if new_entry["a
-0001fb30: 6765 6e74 3122 5d20 213d 2022 223a 0d0a  gent1"] != "":..
-0001fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb50: 7965 7320 3d20 2073 656c 662e 6173 6b5f  yes =  self.ask_
-0001fb60: 7175 6573 7469 6f6e 2827 272c 2254 6865  question('',"The
-0001fb70: 2061 6765 6e74 2025 7320 646f 6573 206e   agent %s does n
-0001fb80: 6f74 2065 7869 7374 2e5c 6e44 6f20 796f  ot exist.\nDo yo
-0001fb90: 7520 7769 7368 2074 6f20 636f 6e74 696e  u wish to contin
-0001fba0: 7565 2061 6e64 2061 7574 6f6d 6174 6963  ue and automatic
-0001fbb0: 616c 6c79 2063 7265 6174 6520 6120 6e65  ally create a ne
-0001fbc0: 7720 6167 656e 743f 2225 6e65 775f 656e  w agent?"%new_en
-0001fbd0: 7472 795b 2261 6765 6e74 3122 5d29 0d0a  try["agent1"])..
-0001fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fbf0: 6966 206e 6f74 2079 6573 3a0d 0a20 2020  if not yes:..   
-0001fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc10: 2072 6574 7572 6e0d 0a0d 0a20 2020 2020   return....     
-0001fc20: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
-0001fc30: 7261 7763 616e 7661 732e 6368 6563 6b5f  rawcanvas.check_
-0001fc40: 6578 6973 7428 6e65 775f 656e 7472 795b  exist(new_entry[
-0001fc50: 2261 6765 6e74 3222 5d29 3a0d 0a20 2020  "agent2"]):..   
-0001fc60: 2020 2020 2020 2020 2069 6620 6e65 775f           if new_
-0001fc70: 656e 7472 795b 2261 6765 6e74 3222 5d20  entry["agent2"] 
-0001fc80: 213d 2022 223a 0d0a 2020 2020 2020 2020  != "":..        
-0001fc90: 2020 2020 2020 2020 7965 7320 3d20 2073          yes =  s
-0001fca0: 656c 662e 6173 6b5f 7175 6573 7469 6f6e  elf.ask_question
-0001fcb0: 2827 272c 2022 5468 6520 6167 656e 7420  ('', "The agent 
-0001fcc0: 2573 2064 6f65 7320 6e6f 7420 6578 6973  %s does not exis
-0001fcd0: 742e 5c6e 446f 2079 6f75 2077 6973 6820  t.\nDo you wish 
-0001fce0: 746f 2063 6f6e 7469 6e75 6520 616e 6420  to continue and 
-0001fcf0: 6175 746f 6d61 7469 6361 6c6c 7920 6372  automatically cr
-0001fd00: 6561 7465 2061 206e 6577 2061 6765 6e74  eate a new agent
-0001fd10: 3f22 256e 6577 5f65 6e74 7279 5b22 6167  ?"%new_entry["ag
-0001fd20: 656e 7432 225d 290d 0a20 2020 2020 2020  ent2"])..       
-0001fd30: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001fd40: 7965 733a 0d0a 2020 2020 2020 2020 2020  yes:..          
-0001fd50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001fd60: 0d0a 0d0a 0d0a 2020 2020 2020 2020 626f  ......        bo
-0001fd70: 7831 203d 2073 656c 662e 6472 6177 6361  x1 = self.drawca
-0001fd80: 6e76 6173 2e61 6464 5f61 6765 6e74 286e  nvas.add_agent(n
-0001fd90: 6577 5f65 6e74 7279 5b22 6167 656e 7431  ew_entry["agent1
-0001fda0: 225d 290d 0a20 2020 2020 2020 2062 6f78  "])..        box
-0001fdb0: 3220 3d20 7365 6c66 2e64 7261 7763 616e  2 = self.drawcan
-0001fdc0: 7661 732e 6164 645f 6167 656e 7428 6e65  vas.add_agent(ne
-0001fdd0: 775f 656e 7472 795b 2261 6765 6e74 3222  w_entry["agent2"
-0001fde0: 5d29 0d0a 0d0a 2020 2020 2020 2020 6d79  ])....        my
-0001fdf0: 5f69 7465 6d73 203d 205b 5d0d 0a20 2020  _items = []..   
-0001fe00: 2020 2020 2064 6174 6120 3d20 6e65 775f       data = new_
-0001fe10: 656e 7472 790d 0a20 2020 2020 2020 2061  entry..        a
-0001fe20: 6c6c 656e 7472 6965 7320 3d20 225c 6e22  llentries = "\n"
-0001fe30: 2e6a 6f69 6e28 5b64 6174 615b 226c 3122  .join([data["l1"
-0001fe40: 5d2c 2064 6174 615b 2261 3122 5d2c 2064  ], data["a1"], d
-0001fe50: 6174 615b 2265 3122 5d2c 2064 6174 615b  ata["e1"], data[
-0001fe60: 226c 3222 5d2c 2064 6174 615b 2261 3222  "l2"], data["a2"
-0001fe70: 5d2c 2064 6174 615b 2265 3222 5d5d 290d  ], data["e2"]]).
-0001fe80: 0a20 2020 2020 2020 2066 6f72 2073 7562  .        for sub
-0001fe90: 5f69 7465 6d20 696e 2061 6c6c 656e 7472  _item in allentr
-0001fea0: 6965 732e 7370 6c69 7428 225c 6e22 293a  ies.split("\n"):
-0001feb0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0001fec0: 7220 7375 625f 656e 7472 7920 696e 2073  r sub_entry in s
-0001fed0: 7562 5f69 7465 6d2e 7370 6c69 7428 225c  ub_item.split("\
-0001fee0: 6e22 293a 0d0a 2020 2020 2020 2020 2020  n"):..          
-0001fef0: 2020 2020 2020 656e 7472 7920 3d20 7375        entry = su
-0001ff00: 625f 656e 7472 792e 7265 706c 6163 6528  b_entry.replace(
-0001ff10: 222d 222c 2222 292e 7265 706c 6163 6528  "-","").replace(
-0001ff20: 222b 222c 2222 292e 7374 7269 7028 290d  "+","").strip().
-0001ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff40: 2069 6620 656e 7472 7920 213d 2020 2222   if entry !=  ""
-0001ff50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001ff60: 2020 2020 2020 206d 795f 6974 656d 732e         my_items.
-0001ff70: 6170 7065 6e64 2865 6e74 7279 290d 0a0d  append(entry)...
-0001ff80: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
-0001ff90: 6177 6361 6e76 6173 2e61 6464 5f63 6f6e  awcanvas.add_con
-0001ffa0: 6e65 6374 696f 6e28 626f 7831 2c20 626f  nection(box1, bo
-0001ffb0: 7832 2c20 6e61 6d65 3d20 7374 7228 7365  x2, name= str(se
-0001ffc0: 6c66 2e65 6469 7453 686f 7274 6e61 6d65  lf.editShortname
-0001ffd0: 2e74 6578 7428 2929 2c73 7562 6a65 6374  .text()),subject
-0001ffe0: 3d73 656c 662e 6564 6974 5375 626a 6563  =self.editSubjec
-0001fff0: 742e 7465 7874 2829 2c69 7465 6d73 3d6d  t.text(),items=m
-00020000: 795f 6974 656d 7329 0d0a 0d0a 2020 2020  y_items)....    
-00020010: 2020 2020 6e65 775f 656e 7472 795b 2275      new_entry["u
-00020020: 6e69 2d64 6972 6563 7469 6f6e 616c 225d  ni-directional"]
-00020030: 203d 205c 0d0a 2020 2020 2020 2020 2020   = \..          
-00020040: 2020 7374 7228 7365 6c66 2e63 6f6d 626f    str(self.combo
-00020050: 556e 6964 6972 2e63 7572 7265 6e74 5465  Unidir.currentTe
-00020060: 7874 2829 290d 0a0d 0a20 2020 2020 2020  xt())....       
-00020070: 206e 6577 5f65 6e74 7279 5b22 6c6f 6720   new_entry["log 
-00020080: 7472 616e 7361 6374 696f 6e22 5d20 3d20  transaction"] = 
-00020090: 5c0d 0a20 2020 2020 2020 2020 2020 2073  \..            s
-000200a0: 656c 662e 7265 6769 7374 6572 466c 6f77  elf.registerFlow
-000200b0: 426f 782e 6375 7272 656e 7454 6578 7428  Box.currentText(
-000200c0: 290d 0a0d 0a20 2020 2020 2020 206e 6577  )....        new
-000200d0: 5f65 6e74 7279 5b22 6361 7368 666c 6f77  _entry["cashflow
-000200e0: 3122 5d20 3d20 5c0d 0a20 2020 2020 2020  1"] = \..       
-000200f0: 2020 2020 2073 7472 2873 656c 662e 636f       str(self.co
-00020100: 6d62 6f43 6173 684c 6566 742e 6375 7272  mboCashLeft.curr
-00020110: 656e 7454 6578 7428 2929 0d0a 2020 2020  entText())..    
-00020120: 2020 2020 6e65 775f 656e 7472 795b 2263      new_entry["c
-00020130: 6173 6866 6c6f 7732 225d 203d 205c 0d0a  ashflow2"] = \..
-00020140: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00020150: 7365 6c66 2e63 6f6d 626f 4361 7368 5269  self.comboCashRi
-00020160: 6768 742e 6375 7272 656e 7454 6578 7428  ght.currentText(
-00020170: 2929 0d0a 0d0a 2020 2020 2020 2020 6e65  ))....        ne
-00020180: 775f 656e 7472 795b 226b 696e 6422 5d20  w_entry["kind"] 
+0001e1f0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+0001e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e210: 2020 2020 2020 206c 745f 7375 6265 6e74         lt_subent
+0001e220: 7279 203d 2073 7562 5f65 6e74 7279 0d0a  ry = sub_entry..
+0001e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e240: 2020 2020 2020 2020 2020 2020 6d79 7320              mys 
+0001e250: 2b3d 2022 7e26 2220 2b20 6c74 5f73 7562  += "~&" + lt_sub
+0001e260: 656e 7472 7920 2b20 225c 5c5c 5c22 202b  entry + "\\\\" +
+0001e270: 2022 5c6e 220d 0a20 2020 2020 2020 2020   "\n"..         
+0001e280: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001e290: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
+0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2b0: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
+0001e2c0: 2020 2020 2020 2020 2020 2020 6d79 7320              mys 
+0001e2d0: 2b3d 2022 2222 0d0a 2020 2020 2020 2020  += """..        
+0001e2e0: 2020 2020 5c65 6e64 7b74 6162 756c 6172      \end{tabular
+0001e2f0: 7d20 2620 5c5c 6265 6769 6e7b 7461 6275  } & \\begin{tabu
+0001e300: 6c61 727d 7b6c 6c7d 2222 2220 2b20 225c  lar}{ll}""" + "\
+0001e310: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
+0001e320: 2020 2020 2020 666f 7220 6974 656d 2c20        for item, 
+0001e330: 656e 7472 7920 696e 206c 6961 6273 2e69  entry in liabs.i
+0001e340: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+0001e350: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001e360: 6974 656d 2021 3d20 2245 7175 6974 7922  item != "Equity"
+0001e370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001e380: 2020 2020 2020 2020 2020 206d 7973 202b             mys +
+0001e390: 3d20 6974 656d 202b 2022 267e 205c 5c5c  = item + "&~ \\\
+0001e3a0: 5c5c 686c 696e 657e 267e 5c5c 5c5c 5c6e  \\hline~&~\\\\\n
+0001e3b0: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
+0001e3c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001e3d0: 2073 7562 5f65 6e74 7279 2069 6e20 656e   sub_entry in en
+0001e3e0: 7472 792e 7370 6c69 7428 225c 6e22 293a  try.split("\n"):
+0001e3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e400: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0001e410: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 2020 6c74 5f73 7562 656e 7472 7920      lt_subentry 
+0001e440: 3d20 7375 625f 656e 7472 790d 0a20 2020  = sub_entry..   
+0001e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e460: 2020 2020 2020 2020 2020 2020 206d 7973               mys
+0001e470: 202b 3d20 227e 2622 202b 206c 745f 7375   += "~&" + lt_su
+0001e480: 6265 6e74 7279 202b 2022 5c5c 5c5c 2220  bentry + "\\\\" 
+0001e490: 2b20 225c 6e22 0d0a 2020 2020 2020 2020  + "\n"..        
+0001e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4b0: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
+0001e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4d0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+0001e4e0: 730d 0a0d 0a20 2020 2020 2020 2020 2020  s....           
+0001e4f0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+0001e500: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001e510: 7465 6d20 3d20 2245 7175 6974 7922 0d0a  tem = "Equity"..
+0001e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e530: 2020 2020 656e 7472 7920 3d20 6c69 6162      entry = liab
+0001e540: 735b 2245 7175 6974 7922 5d0d 0a20 2020  s["Equity"]..   
+0001e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e560: 206d 7973 202b 3d20 6974 656d 202b 2022   mys += item + "
+0001e570: 267e 205c 5c5c 5c5c 686c 696e 657e 267e  &~ \\\\\hline~&~
+0001e580: 5c5c 5c5c 5c6e 220d 0a0d 0a20 2020 2020  \\\\\n"....     
+0001e590: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001e5a0: 6f72 2073 7562 5f65 6e74 7279 2069 6e20  or sub_entry in 
+0001e5b0: 656e 7472 792e 7370 6c69 7428 225c 6e22  entry.split("\n"
+0001e5c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001e5d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0001e5e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e5f0: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
+0001e600: 5f73 7562 656e 7472 7920 3d20 7375 625f  _subentry = sub_
+0001e610: 656e 7472 790d 0a20 2020 2020 2020 2020  entry..         
+0001e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e630: 2020 206d 7973 202b 3d20 227e 2622 202b     mys += "~&" +
+0001e640: 206c 745f 7375 6265 6e74 7279 202b 2022   lt_subentry + "
+0001e650: 5c5c 5c5c 2220 2b20 225c 6e22 0d0a 2020  \\\\" + "\n"..  
+0001e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e670: 2020 2020 2020 6578 6365 7074 3a0d 0a20        except:.. 
+0001e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e690: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+0001e6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e6b0: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
+0001e6c0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0001e6d0: 7373 0d0a 0d0a 2020 2020 2020 2020 2020  ss....          
+0001e6e0: 2020 2020 2020 6d79 7320 2b3d 2022 2222        mys += """
+0001e6f0: 0d0a 2020 2020 2020 2020 2020 2020 5c5c  ..            \\
+0001e700: 656e 647b 7461 6275 6c61 727d 0d0a 2020  end{tabular}..  
+0001e710: 2020 2020 2020 2020 2020 5c5c 5c5c 7e26            \\\\~&
+0001e720: 7e0d 0a20 2020 2020 2020 2020 2020 205c  ~..            \
+0001e730: 5c5c 5c5c 686c 696e 6522 2222 0d0a 2020  \\\\hline"""..  
+0001e740: 2020 2020 2020 2020 2020 2020 2020 6d79                my
+0001e750: 7320 2b3d 2022 2222 0d0a 2020 2020 2020  s += """..      
+0001e760: 2020 2020 2020 5c5c 656e 647b 7461 6275        \\end{tabu
+0001e770: 6c61 727d 2222 220d 0a20 2020 2020 2020  lar}"""..       
+0001e780: 2020 2020 2020 2020 206d 7973 202b 3d20           mys += 
+0001e790: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+0001e7a0: 205c 5c63 6170 7469 6f6e 7b42 616c 616e   \\caption{Balan
+0001e7b0: 6365 2053 6865 6574 206f 6620 2573 7d22  ce Sheet of %s}"
+0001e7c0: 2222 2025 2061 6765 6e74 5f74 6974 6c65  "" % agent_title
+0001e7d0: 6420 2b20 2222 220d 0a20 2020 2020 2020  d + """..       
+0001e7e0: 2020 2020 205c 5c65 6e64 7b74 6162 6c65       \\end{table
+0001e7f0: 7d0d 0a20 2020 2020 2020 2020 2020 2022  }..            "
+0001e800: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
+0001e810: 2020 2020 7465 7873 7472 5f63 6f6d 6269      texstr_combi
+0001e820: 6e65 6420 2b3d 206d 7973 0d0a 0d0a 2020  ned += mys....  
+0001e830: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001e840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 6164 6420  =========== add 
+0001e850: 696e 636f 6d65 0d0a 0d0a 2020 2020 2020  income....      
+0001e860: 2020 2020 2020 2020 2020 6966 2061 6765            if age
+0001e870: 6e74 2069 6e20 636f 6d62 696e 6564 5f69  nt in combined_i
+0001e880: 6e63 6f6d 653a 0d0a 2020 2020 2020 2020  ncome:..        
+0001e890: 2020 2020 2020 2020 2020 2020 696e 636f              inco
+0001e8a0: 6d65 5f64 6174 6120 3d20 636f 6d62 696e  me_data = combin
+0001e8b0: 6564 5f69 6e63 6f6d 655b 6167 656e 745d  ed_income[agent]
+0001e8c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e8d0: 2020 2020 2020 696e 636f 6d65 5f73 7472        income_str
+0001e8e0: 203d 2022 2222 0d0a 2020 2020 2020 2020   = """..        
+0001e8f0: 2020 2020 5c5c 6265 6769 6e7b 7461 626c      \\begin{tabl
+0001e900: 657d 5b48 5d5c 6e5c 6365 6e74 6572 696e  e}[H]\n\centerin
+0001e910: 675c 6e0d 0a20 2020 2020 2020 2020 2020  g\n..           
+0001e920: 205c 5c62 6567 696e 7b74 6162 756c 6172   \\begin{tabular
+0001e930: 7d7b 7c6c 6c7c 7d5c 6e5c 686c 696e 6522  }{|ll|}\n\hline"
+0001e940: 2222 0d0a 0d0a 2020 2020 2020 2020 2020  ""....          
+0001e950: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+0001e960: 696e 2022 5265 7665 6e75 6573 222c 2022  in "Revenues", "
+0001e970: 4761 696e 7322 2c20 2245 7870 656e 7365  Gains", "Expense
+0001e980: 7322 2c20 224c 6f73 7365 7322 2c20 5c0d  s", "Losses", \.
+0001e990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e9a0: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+0001e9b0: 6e74 6572 6573 7420 5061 796d 656e 7473  nterest Payments
+0001e9c0: 222c 2022 4e6f 6e2d 4f70 6572 6174 696f  ", "Non-Operatio
+0001e9d0: 6e61 6c20 496e 636f 6d65 222c 2022 5461  nal Income", "Ta
+0001e9e0: 7865 7322 2c20 224e 6f6e 7461 7861 626c  xes", "Nontaxabl
+0001e9f0: 6520 5072 6f66 6974 7322 2c20 224e 6f6e  e Profits", "Non
+0001ea00: 7461 7861 626c 6520 4c6f 7373 6573 223a  taxable Losses":
+0001ea10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ea20: 2020 2020 2020 2020 2020 7620 3d20 696e            v = in
+0001ea30: 636f 6d65 5f64 6174 615b 6b5d 0d0a 0d0a  come_data[k]....
+0001ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea50: 2020 2020 2020 2020 696e 636f 6d65 5f73          income_s
+0001ea60: 7472 202b 3d20 227e 267e 5c5c 5c5c 220d  tr += "~&~\\\\".
+0001ea70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ea80: 2020 2020 2020 2020 2069 6e63 6f6d 655f           income_
+0001ea90: 7374 7220 2b3d 2022 5c74 2220 2b20 6b20  str += "\t" + k 
+0001eaa0: 2b20 2226 7e5c 5c5c 5c5c 6e22 0d0a 0d0a  + "&~\\\\\n"....
+0001eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eac0: 2020 2020 2020 2020 666f 7220 7375 625f          for sub_
+0001ead0: 7661 6c75 6520 696e 2076 3a0d 0a20 2020  value in v:..   
+0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eaf0: 2020 2020 2020 2020 2069 6e63 6f6d 655f           income_
+0001eb00: 7374 7220 2b3d 2022 5c74 2220 2b20 227e  str += "\t" + "~
+0001eb10: 2622 202b 2073 7562 5f76 616c 7565 5b30  &" + sub_value[0
+0001eb20: 5d20 2b20 7375 625f 7661 6c75 655b 315d  ] + sub_value[1]
+0001eb30: 202b 2022 5c5c 5c5c 5c6e 220d 0a20 2020   + "\\\\\n"..   
+0001eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb50: 2020 2020 2069 6620 6c65 6e28 7629 203d       if len(v) =
+0001eb60: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+0001eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb80: 2020 696e 636f 6d65 5f73 7472 202b 3d20    income_str += 
+0001eb90: 225c 7422 202b 2022 7e26 2220 2b20 222e  "\t" + "~&" + ".
+0001eba0: 2d22 202b 2022 5c5c 5c5c 5c6e 220d 0a0d  -" + "\\\\\n"...
+0001ebb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ebc0: 2020 2020 2020 2020 2069 6620 6b20 213d           if k !=
+0001ebd0: 2022 4e6f 6e74 6178 6162 6c65 204c 6f73   "Nontaxable Los
+0001ebe0: 7365 7322 3a0d 0a20 2020 2020 2020 2020  ses":..         
+0001ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec00: 2020 2069 6e63 6f6d 655f 7374 7220 2b3d     income_str +=
+0001ec10: 2022 7e26 7e5c 5c5c 5c5c 686c 696e 655c   "~&~\\\\\hline\
+0001ec20: 6e22 0d0a 0d0a 2020 2020 2020 2020 2020  n"....          
+0001ec30: 2020 2020 2020 2020 2020 696e 636f 6d65            income
+0001ec40: 5f73 7472 202b 3d20 2222 225c 6e0d 0a20  _str += """\n.. 
+0001ec50: 2020 2020 2020 2020 2020 207e 267e 5c5c             ~&~\\
+0001ec60: 5c5c 5c68 6c69 6e65 5c6e 5c5c 656e 647b  \\\hline\n\\end{
+0001ec70: 7461 6275 6c61 727d 2222 220d 0a20 2020  tabular}"""..   
+0001ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec90: 2069 6e63 6f6d 655f 7374 7220 2b3d 2022   income_str += "
+0001eca0: 2222 5c6e 0d0a 2020 2020 2020 2020 2020  ""\n..          
+0001ecb0: 2020 5c5c 6361 7074 696f 6e7b 496e 636f    \\caption{Inco
+0001ecc0: 6d65 2053 7461 7465 6d65 6e74 206f 6620  me Statement of 
+0001ecd0: 2573 7d22 2222 2025 2061 6765 6e74 5f74  %s}""" % agent_t
+0001ece0: 6974 6c65 6420 2b20 2222 220d 0a20 2020  itled + """..   
+0001ecf0: 2020 2020 2020 2020 205c 5c65 6e64 7b74           \\end{t
+0001ed00: 6162 6c65 7d22 2222 0d0a 0d0a 2020 2020  able}"""....    
+0001ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed20: 7465 7873 7472 5f63 6f6d 6269 6e65 6420  texstr_combined 
+0001ed30: 2b3d 2069 6e63 6f6d 655f 7374 720d 0a0d  += income_str...
+0001ed40: 0a20 2020 2020 2020 2020 2020 2023 203d  .            # =
+0001ed50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ed60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ed70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ed80: 3d3d 3d3d 3d3d 0d0a 2020 2020 2020 2020  ======..        
+0001ed90: 2020 2020 7079 7065 7263 6c69 702e 636f      pyperclip.co
+0001eda0: 7079 2874 6578 7374 725f 636f 6d62 696e  py(texstr_combin
+0001edb0: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
+0001edc0: 2073 656c 662e 6e6f 7469 6679 286d 6573   self.notify(mes
+0001edd0: 7361 6765 3d22 4c61 5465 5820 636f 6465  sage="LaTeX code
+0001ede0: 2063 6f70 6965 6420 746f 2063 6c69 7062   copied to clipb
+0001edf0: 6f61 7264 2e20 4861 7665 2066 756e 2122  oard. Have fun!"
+0001ee00: 2c20 7469 746c 653d 2248 6176 6520 6675  , title="Have fu
+0001ee10: 6e22 290d 0a0d 0a20 2020 2020 2020 2020  n")....         
+0001ee20: 2020 2069 6620 4661 6c73 653a 2023 2064     if False: # d
+0001ee30: 6570 7265 6369 6174 6564 0d0a 0d0a 2020  epreciated....  
+0001ee40: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0001ee50: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+0001ee60: 6e61 6d65 286f 732e 7061 7468 2e61 6273  name(os.path.abs
+0001ee70: 7061 7468 285f 5f66 696c 655f 5f29 290d  path(__file__)).
+0001ee80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ee90: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
+0001eea0: 7468 2e6a 6f69 6e28 7061 7468 202c 2022  th.join(path , "
+0001eeb0: 6669 6c65 732f 696e 636f 6d65 5f73 7461  files/income_sta
+0001eec0: 746d 656e 7473 2e74 6578 2229 2c20 2277  tments.tex"), "w
+0001eed0: 2229 2061 7320 6669 6c65 3a0d 0a20 2020  ") as file:..   
+0001eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eef0: 2066 696c 652e 7772 6974 6528 2222 220d   file.write(""".
+0001ef00: 0a20 2020 205c 646f 6375 6d65 6e74 636c  .    \documentcl
+0001ef10: 6173 737b 6172 7469 636c 657d 0d0a 2020  ass{article}..  
+0001ef20: 2020 5c5c 7573 6570 6163 6b61 6765 7b74    \\usepackage{t
+0001ef30: 6162 756c 6172 787d 0d0a 2020 2020 5c5c  abularx}..    \\
+0001ef40: 7573 6570 6163 6b61 6765 7b61 6d73 6d61  usepackage{amsma
+0001ef50: 7468 7d0d 0a20 2020 205c 5c75 7365 7061  th}..    \\usepa
+0001ef60: 636b 6167 657b 666c 6f61 747d 0d0a 0d0a  ckage{float}....
+0001ef70: 2020 2020 5c5c 6265 6769 6e7b 646f 6375      \\begin{docu
+0001ef80: 6d65 6e74 7d0d 0a0d 0a20 2020 2022 2222  ment}....    """
+0001ef90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001efa0: 2020 2020 2020 2066 696c 652e 7772 6974         file.writ
+0001efb0: 6528 7465 7873 7472 5f63 6f6d 6269 6e65  e(texstr_combine
+0001efc0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+0001efd0: 2020 2020 2020 2020 6669 6c65 2e77 7269          file.wri
+0001efe0: 7465 2822 2222 0d0a 2020 2020 5c5c 656e  te("""..    \\en
+0001eff0: 647b 646f 6375 6d65 6e74 7d0d 0a20 2020  d{document}..   
+0001f000: 2022 2222 290d 0a0d 0a20 2020 2020 2020   """)....       
+0001f010: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
+0001f020: 7375 6270 726f 6365 7373 0d0a 2020 2020  subprocess..    
+0001f030: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0001f040: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001f050: 2020 2020 2020 2020 7061 7468 203d 206f          path = o
+0001f060: 732e 7061 7468 2e64 6972 6e61 6d65 286f  s.path.dirname(o
+0001f070: 732e 7061 7468 2e61 6273 7061 7468 285f  s.path.abspath(_
+0001f080: 5f66 696c 655f 5f29 290d 0a20 2020 2020  _file__))..     
+0001f090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f0a0: 7562 7072 6f63 6573 732e 7275 6e28 2270  ubprocess.run("p
+0001f0b0: 6466 6c61 7465 7820 2573 2220 2520 286f  dflatex %s" % (o
+0001f0c0: 732e 7061 7468 2e6a 6f69 6e28 7061 7468  s.path.join(path
+0001f0d0: 2c20 2266 696c 6573 2f69 6e63 6f6d 655f  , "files/income_
+0001f0e0: 7374 6174 6d65 6e74 732e 7465 7822 2929  statments.tex"))
+0001f0f0: 292e 6368 6563 6b5f 7265 7475 726e 636f  ).check_returnco
+0001f100: 6465 2829 0d0a 0d0a 2020 2020 2020 2020  de()....        
+0001f110: 2020 2020 2020 2020 2020 2020 7368 7574              shut
+0001f120: 696c 2e6d 6f76 6528 7061 7468 202b 2022  il.move(path + "
+0001f130: 696e 636f 6d65 5f73 7461 746d 656e 7473  income_statments
+0001f140: 2e74 6578 222c 2070 6174 6820 2b20 2266  .tex", path + "f
+0001f150: 696c 6573 5c5c 696e 636f 6d65 5f73 7461  iles\\income_sta
+0001f160: 746d 656e 7473 2e74 6578 2229 0d0a 2020  tments.tex")..  
+0001f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f180: 2020 7368 7574 696c 2e6d 6f76 6528 7061    shutil.move(pa
+0001f190: 7468 202b 2022 696e 636f 6d65 5f73 7461  th + "income_sta
+0001f1a0: 746d 656e 7473 2e6c 6f67 222c 2070 6174  tments.log", pat
+0001f1b0: 6820 2b20 2266 696c 6573 5c5c 696e 636f  h + "files\\inco
+0001f1c0: 6d65 5f73 7461 746d 656e 7473 2e6c 6f67  me_statments.log
+0001f1d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0001f1e0: 2020 2020 2020 2020 7368 7574 696c 2e6d          shutil.m
+0001f1f0: 6f76 6528 7061 7468 202b 2022 696e 636f  ove(path + "inco
+0001f200: 6d65 5f73 7461 746d 656e 7473 2e61 7578  me_statments.aux
+0001f210: 222c 2070 6174 6820 2b20 2266 696c 6573  ", path + "files
+0001f220: 5c5c 5c6d 696e 636f 6d65 5f73 7461 746d  \\\mincome_statm
+0001f230: 656e 7473 2e61 7578 2229 0d0a 2020 2020  ents.aux")..    
+0001f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f250: 7368 7574 696c 2e6d 6f76 6528 7061 7468  shutil.move(path
+0001f260: 202b 2022 696e 636f 6d65 5f73 7461 746d   + "income_statm
+0001f270: 656e 7473 2e70 6466 222c 2070 6174 6820  ents.pdf", path 
+0001f280: 2b20 2266 696c 6573 5c5c 696e 636f 6d65  + "files\\income
+0001f290: 5f73 7461 746d 656e 7473 2e70 6466 2229  _statments.pdf")
+0001f2a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f2b0: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+0001f2c0: 7928 6d65 7373 6167 653d 2254 6558 2046  y(message="TeX F
+0001f2d0: 696c 6520 6372 6561 7465 6420 696e 2025  ile created in %
+0001f2e0: 7322 2025 2070 6174 6820 2b20 225c 5c66  s" % path + "\\f
+0001f2f0: 696c 6573 2220 2c74 6974 6c65 3d22 5375  iles" ,title="Su
+0001f300: 6363 6573 7322 290d 0a0d 0a20 2020 2020  ccess")....     
+0001f310: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001f320: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0001f330: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001f340: 2020 2020 2020 2073 656c 662e 6e6f 7469         self.noti
+0001f350: 6679 286d 6573 7361 6765 3d73 7472 2865  fy(message=str(e
+0001f360: 2e5f 5f63 6f6e 7465 7874 5f5f 2920 2b20  .__context__) + 
+0001f370: 225c 6e22 202b 2073 7472 2865 292c 2074  "\n" + str(e), t
+0001f380: 6974 6c65 3d65 2e5f 5f63 6c61 7373 5f5f  itle=e.__class__
+0001f390: 2e5f 5f6e 616d 655f 5f29 0d0a 0d0a 0d0a  .__name__)......
+0001f3a0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0001f3b0: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+0001f3c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001f3d0: 2e6e 6f74 6966 7928 6d65 7373 6167 653d  .notify(message=
+0001f3e0: 7374 7228 652e 5f5f 636f 6e74 6578 745f  str(e.__context_
+0001f3f0: 5f29 202b 2022 5c6e 2220 2b20 7374 7228  _) + "\n" + str(
+0001f400: 6529 2c20 7469 746c 653d 652e 5f5f 636c  e), title=e.__cl
+0001f410: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 290d  ass__.__name__).
+0001f420: 0a0d 0a20 2020 2064 6566 2061 6464 5f68  ...    def add_h
+0001f430: 656c 7065 7228 7365 6c66 293a 0d0a 2020  elper(self):..  
+0001f440: 2020 2020 2020 6e65 775f 6e61 6d65 203d        new_name =
+0001f450: 2073 656c 662e 4865 6c70 6572 4e61 6d65   self.HelperName
+0001f460: 4564 6974 2e74 6578 7428 290d 0a20 2020  Edit.text()..   
+0001f470: 2020 2020 2023 2054 4f44 4f20 6164 6420       # TODO add 
+0001f480: 7365 6375 7269 7479 206d 6563 6861 6e69  security mechani
+0001f490: 736d 2074 6f20 6176 6f69 6420 6f76 6572  sm to avoid over
+0001f4a0: 7772 6974 696e 6720 616e 2061 6765 6e74  writing an agent
+0001f4b0: 0d0a 2020 2020 2020 2020 6966 206e 6577  ..        if new
+0001f4c0: 5f6e 616d 6520 3d3d 2022 223a 0d0a 2020  _name == "":..  
+0001f4d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001f4e0: 6f74 6966 7928 2250 6c65 6173 6520 656e  otify("Please en
+0001f4f0: 7465 7220 6120 7661 6c69 6420 6e61 6d65  ter a valid name
+0001f500: 222c 2074 6974 6c65 3d22 4942 4d20 4572  ", title="IBM Er
+0001f510: 726f 7222 290d 0a20 2020 2020 2020 2065  ror")..        e
+0001f520: 6c69 6620 6e6f 7420 6e65 775f 6e61 6d65  lif not new_name
+0001f530: 5b30 5d2e 6973 7570 7065 7228 293a 0d0a  [0].isupper():..
+0001f540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001f550: 2e6e 6f74 6966 7928 2250 6c65 6173 6520  .notify("Please 
+0001f560: 656e 7465 7220 6120 7661 6c69 6420 6e61  enter a valid na
+0001f570: 6d65 2077 6974 685c 6e75 7070 6572 6361  me with\nupperca
+0001f580: 7365 2066 6972 7374 206c 6574 7465 7220  se first letter 
+0001f590: 6f72 2063 616d 656c 6361 7365 2c20 652e  or camelcase, e.
+0001f5a0: 672e 2027 4d79 4167 656e 7427 222c 2074  g. 'MyAgent'", t
+0001f5b0: 6974 6c65 3d22 4942 4d20 4572 726f 7222  itle="IBM Error"
+0001f5c0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+0001f5d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0001f5e0: 6c66 2e64 7261 7763 616e 7661 732e 6164  lf.drawcanvas.ad
+0001f5f0: 645f 6167 656e 7428 6e65 775f 6e61 6d65  d_agent(new_name
+0001f600: 290d 0a0d 0a20 2020 2064 6566 2072 656d  )....    def rem
+0001f610: 6f76 655f 6865 6c70 6572 2873 656c 6629  ove_helper(self)
+0001f620: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+0001f630: 6472 6177 6361 6e76 6173 2e72 656d 6f76  drawcanvas.remov
+0001f640: 655f 6167 656e 7428 290d 0a0d 0a20 2020  e_agent()....   
+0001f650: 2064 6566 2061 6464 5f6e 6577 2873 656c   def add_new(sel
+0001f660: 6629 3a0d 0a0d 0a20 2020 2020 2020 2023  f):....        #
+0001f670: 2054 4f44 4f20 6173 7365 7274 2074 6861   TODO assert tha
+0001f680: 7420 7175 616e 7469 7479 2069 7320 6e6f  t quantity is no
+0001f690: 7420 7965 7420 696e 2061 6e79 206f 7468  t yet in any oth
+0001f6a0: 6572 2074 7261 6e73 6163 7469 6f6e 0d0a  er transaction..
+0001f6b0: 2020 2020 2020 2020 7365 6c66 2e6d 6164          self.mad
+0001f6c0: 655f 6368 616e 6765 7320 3d20 4661 6c73  e_changes = Fals
+0001f6d0: 650d 0a0d 0a0d 0a20 2020 2020 2020 206e  e......        n
+0001f6e0: 6577 5f65 6e74 7279 203d 207b 7d0d 0a0d  ew_entry = {}...
+0001f6f0: 0a20 2020 2020 2020 206e 6577 5f65 6e74  .        new_ent
+0001f700: 7279 5b22 6131 225d 203d 2073 656c 662e  ry["a1"] = self.
+0001f710: 4173 7365 744c 6973 744c 6566 742e 746f  AssetListLeft.to
+0001f720: 506c 6169 6e54 6578 7428 290d 0a20 2020  PlainText()..   
+0001f730: 2020 2020 206e 6577 5f65 6e74 7279 5b22       new_entry["
+0001f740: 6132 225d 203d 2073 656c 662e 4173 7365  a2"] = self.Asse
+0001f750: 744c 6973 7452 6967 6874 2e74 6f50 6c61  tListRight.toPla
+0001f760: 696e 5465 7874 2829 0d0a 2020 2020 2020  inText()..      
+0001f770: 2020 6e65 775f 656e 7472 795b 226c 3122    new_entry["l1"
+0001f780: 5d20 3d20 7365 6c66 2e4c 6961 6269 6c69  ] = self.Liabili
+0001f790: 7479 4c69 7374 4c65 6674 2e74 6f50 6c61  tyListLeft.toPla
+0001f7a0: 696e 5465 7874 2829 0d0a 2020 2020 2020  inText()..      
+0001f7b0: 2020 6e65 775f 656e 7472 795b 226c 3222    new_entry["l2"
+0001f7c0: 5d20 3d20 7365 6c66 2e4c 6961 6269 6c69  ] = self.Liabili
+0001f7d0: 7479 4c69 7374 5269 6768 742e 746f 506c  tyListRight.toPl
+0001f7e0: 6169 6e54 6578 7428 290d 0a20 2020 2020  ainText()..     
+0001f7f0: 2020 206e 6577 5f65 6e74 7279 5b22 6531     new_entry["e1
+0001f800: 225d 203d 2073 656c 662e 4571 7569 7479  "] = self.Equity
+0001f810: 4c69 7374 4c65 6674 2e74 6f50 6c61 696e  ListLeft.toPlain
+0001f820: 5465 7874 2829 0d0a 2020 2020 2020 2020  Text()..        
+0001f830: 6e65 775f 656e 7472 795b 2265 3222 5d20  new_entry["e2"] 
+0001f840: 3d20 7365 6c66 2e45 7175 6974 794c 6973  = self.EquityLis
+0001f850: 7452 6967 6874 2e74 6f50 6c61 696e 5465  tRight.toPlainTe
+0001f860: 7874 2829 0d0a 0d0a 2020 2020 2020 2020  xt()....        
+0001f870: 2320 6e65 775f 656e 7472 795b 2261 3122  # new_entry["a1"
+0001f880: 5d20 3d20 7365 6c66 2e41 7373 6574 4c69  ] = self.AssetLi
+0001f890: 7374 4c65 6674 2e74 6f50 6c61 696e 5465  stLeft.toPlainTe
+0001f8a0: 7874 2829 0d0a 2020 2020 2020 2020 2320  xt()..        # 
+0001f8b0: 6e65 775f 656e 7472 795b 226c 3122 5d20  new_entry["l1"] 
+0001f8c0: 3d20 7365 6c66 2e4c 6961 6269 6c69 7479  = self.Liability
+0001f8d0: 4c69 7374 4c65 6674 2e74 6f50 6c61 696e  ListLeft.toPlain
+0001f8e0: 5465 7874 2829 0d0a 2020 2020 2020 2020  Text()..        
+0001f8f0: 2320 6e65 775f 656e 7472 795b 2261 3222  # new_entry["a2"
+0001f900: 5d20 3d20 7365 6c66 2e4c 6961 6269 6c69  ] = self.Liabili
+0001f910: 7479 4c69 7374 5269 6768 742e 746f 506c  tyListRight.toPl
+0001f920: 6169 6e54 6578 7428 290d 0a20 2020 2020  ainText()..     
+0001f930: 2020 2023 206e 6577 5f65 6e74 7279 5b22     # new_entry["
+0001f940: 6c32 225d 203d 2073 656c 662e 4173 7365  l2"] = self.Asse
+0001f950: 744c 6973 7452 6967 6874 2e74 6f50 6c61  tListRight.toPla
+0001f960: 696e 5465 7874 2829 0d0a 2020 2020 2020  inText()..      
+0001f970: 2020 2320 6e65 775f 656e 7472 795b 2265    # new_entry["e
+0001f980: 3122 5d20 3d20 7365 6c66 2e45 7175 6974  1"] = self.Equit
+0001f990: 794c 6973 744c 6566 742e 746f 506c 6169  yListLeft.toPlai
+0001f9a0: 6e54 6578 7428 290d 0a20 2020 2020 2020  nText()..       
+0001f9b0: 2023 206e 6577 5f65 6e74 7279 5b22 6532   # new_entry["e2
+0001f9c0: 225d 203d 2073 656c 662e 4571 7569 7479  "] = self.Equity
+0001f9d0: 4c69 7374 5269 6768 742e 746f 506c 6169  ListRight.toPlai
+0001f9e0: 6e54 6578 7428 290d 0a0d 0a20 2020 2020  nText()....     
+0001f9f0: 2020 206e 6577 5f65 6e74 7279 5b22 6167     new_entry["ag
+0001fa00: 656e 7431 225d 203d 2063 616d 656c 2873  ent1"] = camel(s
+0001fa10: 656c 662e 6167 656e 7431 4564 6974 2e74  elf.agent1Edit.t
+0001fa20: 6578 7428 2929 2023 2e63 6170 6974 616c  ext()) #.capital
+0001fa30: 697a 6528 290d 0a20 2020 2020 2020 206e  ize()..        n
+0001fa40: 6577 5f65 6e74 7279 5b22 6167 656e 7432  ew_entry["agent2
+0001fa50: 225d 203d 2063 616d 656c 2873 656c 662e  "] = camel(self.
+0001fa60: 6167 656e 7432 4564 6974 2e74 6578 7428  agent2Edit.text(
+0001fa70: 2929 2023 2e63 6170 6974 616c 697a 6528  )) #.capitalize(
+0001fa80: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+0001fa90: 662e 6167 656e 7431 4564 6974 2e73 6574  f.agent1Edit.set
+0001faa0: 5465 7874 2863 616d 656c 2873 656c 662e  Text(camel(self.
+0001fab0: 6167 656e 7431 4564 6974 2e74 6578 7428  agent1Edit.text(
+0001fac0: 2929 2920 2320 2e63 6170 6974 616c 697a  ))) # .capitaliz
+0001fad0: 6528 2929 0d0a 2020 2020 2020 2020 7365  e())..        se
+0001fae0: 6c66 2e61 6765 6e74 3245 6469 742e 7365  lf.agent2Edit.se
+0001faf0: 7454 6578 7428 6361 6d65 6c28 7365 6c66  tText(camel(self
+0001fb00: 2e61 6765 6e74 3245 6469 742e 7465 7874  .agent2Edit.text
+0001fb10: 2829 2929 2023 2e63 6170 6974 616c 697a  ())) #.capitaliz
+0001fb20: 6528 2929 0d0a 0d0a 2020 2020 2020 2020  e())....        
+0001fb30: 6966 206e 6f74 2073 656c 662e 6472 6177  if not self.draw
+0001fb40: 6361 6e76 6173 2e63 6865 636b 5f65 7869  canvas.check_exi
+0001fb50: 7374 286e 6577 5f65 6e74 7279 5b22 6167  st(new_entry["ag
+0001fb60: 656e 7431 225d 293a 0d0a 2020 2020 2020  ent1"]):..      
+0001fb70: 2020 2020 2020 6966 206e 6577 5f65 6e74        if new_ent
+0001fb80: 7279 5b22 6167 656e 7431 225d 2021 3d20  ry["agent1"] != 
+0001fb90: 2222 3a0d 0a20 2020 2020 2020 2020 2020  "":..           
+0001fba0: 2020 2020 2079 6573 203d 2020 7365 6c66       yes =  self
+0001fbb0: 2e61 736b 5f71 7565 7374 696f 6e28 2727  .ask_question(''
+0001fbc0: 2c22 5468 6520 6167 656e 7420 2573 2064  ,"The agent %s d
+0001fbd0: 6f65 7320 6e6f 7420 6578 6973 742e 5c6e  oes not exist.\n
+0001fbe0: 446f 2079 6f75 2077 6973 6820 746f 2063  Do you wish to c
+0001fbf0: 6f6e 7469 6e75 6520 616e 6420 6175 746f  ontinue and auto
+0001fc00: 6d61 7469 6361 6c6c 7920 6372 6561 7465  matically create
+0001fc10: 2061 206e 6577 2061 6765 6e74 3f22 256e   a new agent?"%n
+0001fc20: 6577 5f65 6e74 7279 5b22 6167 656e 7431  ew_entry["agent1
+0001fc30: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+0001fc40: 2020 2020 2069 6620 6e6f 7420 7965 733a       if not yes:
+0001fc50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001fc60: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
+0001fc70: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0001fc80: 656c 662e 6472 6177 6361 6e76 6173 2e63  elf.drawcanvas.c
+0001fc90: 6865 636b 5f65 7869 7374 286e 6577 5f65  heck_exist(new_e
+0001fca0: 6e74 7279 5b22 6167 656e 7432 225d 293a  ntry["agent2"]):
+0001fcb0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001fcc0: 206e 6577 5f65 6e74 7279 5b22 6167 656e   new_entry["agen
+0001fcd0: 7432 225d 2021 3d20 2222 3a0d 0a20 2020  t2"] != "":..   
+0001fce0: 2020 2020 2020 2020 2020 2020 2079 6573               yes
+0001fcf0: 203d 2020 7365 6c66 2e61 736b 5f71 7565   =  self.ask_que
+0001fd00: 7374 696f 6e28 2727 2c20 2254 6865 2061  stion('', "The a
+0001fd10: 6765 6e74 2025 7320 646f 6573 206e 6f74  gent %s does not
+0001fd20: 2065 7869 7374 2e5c 6e44 6f20 796f 7520   exist.\nDo you 
+0001fd30: 7769 7368 2074 6f20 636f 6e74 696e 7565  wish to continue
+0001fd40: 2061 6e64 2061 7574 6f6d 6174 6963 616c   and automatical
+0001fd50: 6c79 2063 7265 6174 6520 6120 6e65 7720  ly create a new 
+0001fd60: 6167 656e 743f 2225 6e65 775f 656e 7472  agent?"%new_entr
+0001fd70: 795b 2261 6765 6e74 3222 5d29 0d0a 2020  y["agent2"])..  
+0001fd80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001fd90: 206e 6f74 2079 6573 3a0d 0a20 2020 2020   not yes:..     
+0001fda0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001fdb0: 6574 7572 6e0d 0a0d 0a0d 0a20 2020 2020  eturn......     
+0001fdc0: 2020 2062 6f78 3120 3d20 7365 6c66 2e64     box1 = self.d
+0001fdd0: 7261 7763 616e 7661 732e 6164 645f 6167  rawcanvas.add_ag
+0001fde0: 656e 7428 6e65 775f 656e 7472 795b 2261  ent(new_entry["a
+0001fdf0: 6765 6e74 3122 5d29 0d0a 2020 2020 2020  gent1"])..      
+0001fe00: 2020 626f 7832 203d 2073 656c 662e 6472    box2 = self.dr
+0001fe10: 6177 6361 6e76 6173 2e61 6464 5f61 6765  awcanvas.add_age
+0001fe20: 6e74 286e 6577 5f65 6e74 7279 5b22 6167  nt(new_entry["ag
+0001fe30: 656e 7432 225d 290d 0a0d 0a20 2020 2020  ent2"])....     
+0001fe40: 2020 206d 795f 6974 656d 7320 3d20 5b5d     my_items = []
+0001fe50: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001fe60: 206e 6577 5f65 6e74 7279 0d0a 2020 2020   new_entry..    
+0001fe70: 2020 2020 616c 6c65 6e74 7269 6573 203d      allentries =
+0001fe80: 2022 5c6e 222e 6a6f 696e 285b 6461 7461   "\n".join([data
+0001fe90: 5b22 6c31 225d 2c20 6461 7461 5b22 6131  ["l1"], data["a1
+0001fea0: 225d 2c20 6461 7461 5b22 6531 225d 2c20  "], data["e1"], 
+0001feb0: 6461 7461 5b22 6c32 225d 2c20 6461 7461  data["l2"], data
+0001fec0: 5b22 6132 225d 2c20 6461 7461 5b22 6532  ["a2"], data["e2
+0001fed0: 225d 5d29 0d0a 2020 2020 2020 2020 666f  "]])..        fo
+0001fee0: 7220 7375 625f 6974 656d 2069 6e20 616c  r sub_item in al
+0001fef0: 6c65 6e74 7269 6573 2e73 706c 6974 2822  lentries.split("
+0001ff00: 5c6e 2229 3a0d 0a20 2020 2020 2020 2020  \n"):..         
+0001ff10: 2020 2066 6f72 2073 7562 5f65 6e74 7279     for sub_entry
+0001ff20: 2069 6e20 7375 625f 6974 656d 2e73 706c   in sub_item.spl
+0001ff30: 6974 2822 5c6e 2229 3a0d 0a20 2020 2020  it("\n"):..     
+0001ff40: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+0001ff50: 203d 2073 7562 5f65 6e74 7279 2e72 6570   = sub_entry.rep
+0001ff60: 6c61 6365 2822 2d22 2c22 2229 2e72 6570  lace("-","").rep
+0001ff70: 6c61 6365 2822 2b22 2c22 2229 2e73 7472  lace("+","").str
+0001ff80: 6970 2829 0d0a 2020 2020 2020 2020 2020  ip()..          
+0001ff90: 2020 2020 2020 6966 2065 6e74 7279 2021        if entry !
+0001ffa0: 3d20 2022 223a 0d0a 2020 2020 2020 2020  =  "":..        
+0001ffb0: 2020 2020 2020 2020 2020 2020 6d79 5f69              my_i
+0001ffc0: 7465 6d73 2e61 7070 656e 6428 656e 7472  tems.append(entr
+0001ffd0: 7929 0d0a 0d0a 2020 2020 2020 2020 7365  y)....        se
+0001ffe0: 6c66 2e64 7261 7763 616e 7661 732e 6164  lf.drawcanvas.ad
+0001fff0: 645f 636f 6e6e 6563 7469 6f6e 2862 6f78  d_connection(box
+00020000: 312c 2062 6f78 322c 206e 616d 653d 2073  1, box2, name= s
+00020010: 7472 2873 656c 662e 6564 6974 5368 6f72  tr(self.editShor
+00020020: 746e 616d 652e 7465 7874 2829 292c 7375  tname.text()),su
+00020030: 626a 6563 743d 7365 6c66 2e65 6469 7453  bject=self.editS
+00020040: 7562 6a65 6374 2e74 6578 7428 292c 6974  ubject.text(),it
+00020050: 656d 733d 6d79 5f69 7465 6d73 290d 0a0d  ems=my_items)...
+00020060: 0a20 2020 2020 2020 206e 6577 5f65 6e74  .        new_ent
+00020070: 7279 5b22 756e 692d 6469 7265 6374 696f  ry["uni-directio
+00020080: 6e61 6c22 5d20 3d20 5c0d 0a20 2020 2020  nal"] = \..     
+00020090: 2020 2020 2020 2073 7472 2873 656c 662e         str(self.
+000200a0: 636f 6d62 6f55 6e69 6469 722e 6375 7272  comboUnidir.curr
+000200b0: 656e 7454 6578 7428 2929 0d0a 0d0a 2020  entText())....  
+000200c0: 2020 2020 2020 6e65 775f 656e 7472 795b        new_entry[
+000200d0: 226c 6f67 2074 7261 6e73 6163 7469 6f6e  "log transaction
+000200e0: 225d 203d 205c 0d0a 2020 2020 2020 2020  "] = \..        
+000200f0: 2020 2020 7365 6c66 2e72 6567 6973 7465      self.registe
+00020100: 7246 6c6f 7742 6f78 2e63 7572 7265 6e74  rFlowBox.current
+00020110: 5465 7874 2829 0d0a 0d0a 2020 2020 2020  Text()....      
+00020120: 2020 6e65 775f 656e 7472 795b 2263 6173    new_entry["cas
+00020130: 6866 6c6f 7731 225d 203d 205c 0d0a 2020  hflow1"] = \..  
+00020140: 2020 2020 2020 2020 2020 7374 7228 7365            str(se
+00020150: 6c66 2e63 6f6d 626f 4361 7368 4c65 6674  lf.comboCashLeft
+00020160: 2e63 7572 7265 6e74 5465 7874 2829 290d  .currentText()).
+00020170: 0a20 2020 2020 2020 206e 6577 5f65 6e74  .        new_ent
+00020180: 7279 5b22 6361 7368 666c 6f77 3222 5d20  ry["cashflow2"] 
 00020190: 3d20 5c0d 0a20 2020 2020 2020 2020 2020  = \..           
-000201a0: 2073 7472 2873 656c 662e 6564 6974 5479   str(self.editTy
-000201b0: 7065 2e63 7572 7265 6e74 5465 7874 2829  pe.currentText()
-000201c0: 290d 0a0d 0a20 2020 2020 2020 206e 6577  )....        new
-000201d0: 5f65 6e74 7279 5b22 696e 636f 6d65 3122  _entry["income1"
-000201e0: 5d20 3d20 5c0d 0a20 2020 2020 2020 2020  ] = \..         
-000201f0: 2020 2073 7472 2873 656c 662e 636f 6d62     str(self.comb
-00020200: 6f49 6e63 6f6d 654c 6566 742e 6375 7272  oIncomeLeft.curr
-00020210: 656e 7454 6578 7428 2929 0d0a 2020 2020  entText())..    
-00020220: 2020 2020 6e65 775f 656e 7472 795b 2269      new_entry["i
-00020230: 6e63 6f6d 6532 225d 203d 205c 0d0a 2020  ncome2"] = \..  
-00020240: 2020 2020 2020 2020 2020 7374 7228 7365            str(se
-00020250: 6c66 2e63 6f6d 626f 496e 636f 6d65 5269  lf.comboIncomeRi
-00020260: 6768 742e 6375 7272 656e 7454 6578 7428  ght.currentText(
-00020270: 2929 0d0a 0d0a 2020 2020 2020 2020 6e65  ))....        ne
-00020280: 775f 656e 7472 795b 2271 7561 6e74 6974  w_entry["quantit
-00020290: 7922 5d20 3d20 5c0d 0a20 2020 2020 2020  y"] = \..       
-000202a0: 2020 2020 2073 7472 2873 656c 662e 6564       str(self.ed
-000202b0: 6974 5175 616e 7469 7479 2e74 6578 7428  itQuantity.text(
-000202c0: 2929 0d0a 0d0a 2020 2020 2020 2020 6e65  ))....        ne
-000202d0: 775f 656e 7472 795b 2273 7562 6a65 6374  w_entry["subject
-000202e0: 225d 203d 205c 0d0a 2020 2020 2020 2020  "] = \..        
-000202f0: 2020 2020 7374 7228 7365 6c66 2e65 6469      str(self.edi
-00020300: 7453 7562 6a65 6374 2e74 6578 7428 2929  tSubject.text())
-00020310: 0d0a 0d0a 2020 2020 2020 2020 6e65 775f  ....        new_
-00020320: 656e 7472 795b 2273 686f 7274 6e61 6d65  entry["shortname
-00020330: 225d 203d 205c 0d0a 2020 2020 2020 2020  "] = \..        
-00020340: 2020 2020 7374 7228 7365 6c66 2e65 6469      str(self.edi
-00020350: 7453 686f 7274 6e61 6d65 2e74 6578 7428  tShortname.text(
-00020360: 2929 0d0a 0d0a 2020 2020 2020 2020 6e65  ))....        ne
-00020370: 775f 656e 7472 795b 2264 6573 6372 6970  w_entry["descrip
-00020380: 7469 6f6e 225d 203d 205c 0d0a 2020 2020  tion"] = \..    
-00020390: 2020 2020 2020 2020 7374 7228 7365 6c66          str(self
-000203a0: 2e65 6469 7444 6573 6372 6970 7469 6f6e  .editDescription
-000203b0: 2e74 6578 7428 2929 0d0a 0d0a 2020 2020  .text())....    
-000203c0: 2020 2020 7365 6c66 2e65 6e74 7279 5f64      self.entry_d
-000203d0: 6174 612e 6170 7065 6e64 286e 6577 5f65  ata.append(new_e
-000203e0: 6e74 7279 290d 0a20 2020 2020 2020 2073  ntry)..        s
-000203f0: 656c 662e 7570 6461 7465 5f74 6162 6c65  elf.update_table
-00020400: 2829 0d0a 0d0a 0d0a 0d0a 2020 2020 2020  ()........      
-00020410: 2020 6461 726b 4d6f 6465 203d 2054 7275    darkMode = Tru
-00020420: 650d 0a20 2020 2020 2020 2074 7279 3a0d  e..        try:.
-00020430: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00020440: 7365 6c66 2e74 6865 6d65 5f6d 616e 6167  self.theme_manag
-00020450: 6572 2e74 6865 6d65 203d 3d20 2262 7269  er.theme == "bri
-00020460: 6768 7422 3a0d 0a20 2020 2020 2020 2020  ght":..         
-00020470: 2020 2020 2020 2064 6172 6b4d 6f64 6520         darkMode 
-00020480: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00020490: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
-000204a0: 2020 2020 2020 7061 7373 0d0a 0d0a 2020        pass....  
-000204b0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000204c0: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
-000204d0: 6563 7469 6f6e 5f69 6478 203d 206c 656e  ection_idx = len
-000204e0: 2873 656c 662e 656e 7472 795f 6461 7461  (self.entry_data
-000204f0: 292d 310d 0a20 2020 2020 2020 2020 2020  )-1..           
-00020500: 2073 656c 662e 726f 775f 7365 6c65 6374   self.row_select
-00020510: 2873 656c 662e 7365 6c65 6374 696f 6e5f  (self.selection_
-00020520: 6964 7829 0d0a 2020 2020 2020 2020 6578  idx)..        ex
-00020530: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00020540: 7320 6520 3a0d 0a20 2020 2020 2020 2020  s e :..         
-00020550: 2020 2073 656c 662e 6e6f 7469 6679 2822     self.notify("
-00020560: 4552 524f 523a 2220 2b20 7472 2865 292c  ERROR:" + tr(e),
-00020570: 7469 746c 653d 2245 7272 6f72 2229 0d0a  title="Error")..
-00020580: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00020590: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000205a0: 656c 6563 7469 6f6e 5f69 6478 2069 7320  election_idx is 
-000205b0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-000205c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000205d0: 7261 6e67 6528 7365 6c66 2e74 7261 6e73  range(self.trans
-000205e0: 6163 7469 6f6e 5669 6577 2e63 6f6c 756d  actionView.colum
-000205f0: 6e43 6f75 6e74 2829 293a 0d0a 0d0a 2020  nCount()):....  
-00020600: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00020610: 2064 6172 6b4d 6f64 653a 0d0a 2020 2020   darkMode:..    
-00020620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020630: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
-00020640: 5669 6577 2e69 7465 6d28 7365 6c66 2e73  View.item(self.s
-00020650: 656c 6563 7469 6f6e 5f69 6478 2c20 6929  election_idx, i)
-00020660: 2e73 6574 4261 636b 6772 6f75 6e64 2851  .setBackground(Q
-00020670: 7447 7569 2e51 436f 6c6f 7228 3231 2c20  tGui.QColor(21, 
-00020680: 3231 2c20 3231 2929 0d0a 2020 2020 2020  21, 21))..      
-00020690: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-000206a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000206b0: 2020 2020 2073 656c 662e 7472 616e 7361       self.transa
-000206c0: 6374 696f 6e56 6965 772e 6974 656d 2873  ctionView.item(s
-000206d0: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
-000206e0: 782c 2069 292e 7365 7442 6163 6b67 726f  x, i).setBackgro
-000206f0: 756e 6428 5174 4775 692e 5143 6f6c 6f72  und(QtGui.QColor
-00020700: 2832 3333 2c20 3233 342c 2032 3237 2929  (233, 234, 227))
-00020710: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00020720: 7365 6c66 2e73 656c 6563 7469 6f6e 5f69  self.selection_i
-00020730: 6478 203d 2073 656c 662e 7472 616e 7361  dx = self.transa
-00020740: 6374 696f 6e56 6965 772e 726f 7743 6f75  ctionView.rowCou
-00020750: 6e74 2829 2d31 0d0a 2020 2020 2020 2020  nt()-1..        
-00020760: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00020770: 6765 2873 656c 662e 7472 616e 7361 6374  ge(self.transact
-00020780: 696f 6e56 6965 772e 636f 6c75 6d6e 436f  ionView.columnCo
-00020790: 756e 7428 2929 3a0d 0a20 2020 2020 2020  unt()):..       
-000207a0: 2020 2020 2020 2020 2069 6620 6461 726b           if dark
-000207b0: 4d6f 6465 3a0d 0a20 2020 2020 2020 2020  Mode:..         
-000207c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000207d0: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
-000207e0: 6974 656d 2873 656c 662e 7365 6c65 6374  item(self.select
-000207f0: 696f 6e5f 6964 782c 2069 292e 7365 7442  ion_idx, i).setB
-00020800: 6163 6b67 726f 756e 6428 5174 4775 692e  ackground(QtGui.
-00020810: 5143 6f6c 6f72 2831 382c 2031 382c 2031  QColor(18, 18, 1
-00020820: 3829 290d 0a20 2020 2020 2020 2020 2020  8))..           
-00020830: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00020840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020850: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
-00020860: 5669 6577 2e69 7465 6d28 7365 6c66 2e73  View.item(self.s
-00020870: 656c 6563 7469 6f6e 5f69 6478 2c20 6929  election_idx, i)
-00020880: 2e73 6574 4261 636b 6772 6f75 6e64 2851  .setBackground(Q
-00020890: 7447 7569 2e51 436f 6c6f 7228 3135 392c  tGui.QColor(159,
-000208a0: 2031 3539 2c20 3135 3929 290d 0a20 2020   159, 159))..   
-000208b0: 2020 2020 2022 2222 0d0a 0d0a 0d0a 0d0a       """........
-000208c0: 0d0a 2020 2020 6465 6620 676f 746f 5f6e  ..    def goto_n
-000208d0: 6578 7428 7365 6c66 293a 0d0a 2020 2020  ext(self):..    
-000208e0: 2020 2020 7061 7373 0d0a 0d0a 0d0a 2020      pass......  
-000208f0: 2020 6465 6620 7564 7061 7465 5f64 6973    def udpate_dis
-00020900: 706c 6179 2873 656c 6629 3a0d 0a20 2020  play(self):..   
-00020910: 2020 2020 2074 7279 3a0d 0a0d 0a20 2020       try:....   
-00020920: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-00020930: 6520 3d20 7365 6c66 2e66 696c 656e 616d  e = self.filenam
-00020940: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00020950: 2077 6974 6820 6f70 656e 2866 696c 656e   with open(filen
-00020960: 616d 652c 2027 7227 2920 6173 2073 7472  ame, 'r') as str
-00020970: 6561 6d3a 0d0a 2020 2020 2020 2020 2020  eam:..          
-00020980: 2020 2020 2020 6669 6c65 6461 7461 203d        filedata =
-00020990: 2079 616d 6c2e 7361 6665 5f6c 6f61 6428   yaml.safe_load(
-000209a0: 7374 7265 616d 290d 0a20 2020 2020 2020  stream)..       
-000209b0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-000209c0: 696c 6564 6174 6129 0d0a 0d0a 2020 2020  iledata)....    
-000209d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000209e0: 2e61 6765 6e74 314c 6162 656c 2e74 6578  .agent1Label.tex
-000209f0: 7420 3d20 6669 6c65 6461 7461 5b22 6167  t = filedata["ag
-00020a00: 656e 7431 225d 0d0a 2020 2020 2020 2020  ent1"]..        
-00020a10: 2020 2020 2020 2020 7365 6c66 2e61 6765          self.age
-00020a20: 6e74 324c 6162 656c 2e74 6578 7420 3d20  nt2Label.text = 
-00020a30: 6669 6c65 6461 7461 5b22 6167 656e 7432  filedata["agent2
-00020a40: 225d 0d0a 0d0a 2020 2020 2020 2020 2020  "]....          
-00020a50: 2020 2020 2020 2320 7365 6c66 2e61 312e        # self.a1.
-00020a60: 7661 6c75 6520 3d20 6669 6c65 6461 7461  value = filedata
-00020a70: 5b22 6131 225d 2020 2320 2b20 225c 6e22  ["a1"]  # + "\n"
-00020a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020a90: 2020 2320 7365 6c66 2e65 312e 7661 6c75    # self.e1.valu
-00020aa0: 6520 3d20 6669 6c65 6461 7461 5b22 6531  e = filedata["e1
-00020ab0: 225d 2020 2320 2b20 225c 6e22 0d0a 2020  "]  # + "\n"..  
-00020ac0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020ad0: 7365 6c66 2e6c 312e 7661 6c75 6520 3d20  self.l1.value = 
-00020ae0: 6669 6c65 6461 7461 5b22 6c31 225d 2020  filedata["l1"]  
-00020af0: 2320 2b20 225c 6e22 0d0a 2020 2020 2020  # + "\n"..      
-00020b00: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00020b10: 2e61 322e 7661 6c75 6520 3d20 6669 6c65  .a2.value = file
-00020b20: 6461 7461 5b22 6132 225d 2020 2320 2b20  data["a2"]  # + 
-00020b30: 225c 6e22 0d0a 2020 2020 2020 2020 2020  "\n"..          
-00020b40: 2020 2020 2020 2320 7365 6c66 2e65 322e        # self.e2.
-00020b50: 7661 6c75 6520 3d20 6669 6c65 6461 7461  value = filedata
-00020b60: 5b22 6532 225d 2020 2320 2b20 225c 6e22  ["e2"]  # + "\n"
-00020b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020b80: 2020 2320 7365 6c66 2e6c 322e 7661 6c75    # self.l2.valu
-00020b90: 6520 3d20 6669 6c65 6461 7461 5b22 6c32  e = filedata["l2
-00020ba0: 225d 2020 2320 2b20 225c 6e22 0d0a 0d0a  "]  # + "\n"....
-00020bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bc0: 2320 6966 2022 7368 6f72 746e 616d 6522  # if "shortname"
-00020bd0: 2069 6e20 6669 6c65 6461 7461 3a0d 0a20   in filedata:.. 
-00020be0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00020bf0: 2020 2020 7365 6c66 2e70 6172 656e 742e      self.parent.
-00020c00: 7368 6f72 746e 616d 652e 7661 6c75 6520  shortname.value 
-00020c10: 3d20 6669 6c65 6461 7461 5b22 7368 6f72  = filedata["shor
-00020c20: 746e 616d 6522 5d0d 0a0d 0a20 2020 2020  tname"]....     
-00020c30: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00020c40: 2275 6e69 2d64 6972 6563 7469 6f6e 616c  "uni-directional
-00020c50: 2220 696e 2066 696c 6564 6174 613a 0d0a  " in filedata:..
-00020c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c70: 2320 2020 2073 656c 662e 7061 7265 6e74  #    self.parent
-00020c80: 2e64 6972 6563 7469 6f6e 5f63 6865 636b  .direction_check
-00020c90: 2e76 616c 7565 203d 2062 6f6f 6c28 7374  .value = bool(st
-00020ca0: 7228 6669 6c65 6461 7461 5b22 756e 692d  r(filedata["uni-
-00020cb0: 6469 7265 6374 696f 6e61 6c22 5d29 290d  directional"])).
-00020cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020cd0: 2023 2065 6c73 653a 0d0a 2020 2020 2020   # else:..      
-00020ce0: 2020 2020 2020 2020 2020 2320 2020 2073            #    s
-00020cf0: 656c 662e 7061 7265 6e74 2e64 6972 6563  elf.parent.direc
-00020d00: 7469 6f6e 5f63 6865 636b 2e76 616c 7565  tion_check.value
-00020d10: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
-00020d20: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00020d30: 2022 6465 7363 7269 7074 696f 6e22 2069   "description" i
-00020d40: 6e20 6669 6c65 6461 7461 3a0d 0a20 2020  n filedata:..   
-00020d50: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00020d60: 2020 7365 6c66 2e70 6172 656e 742e 6465    self.parent.de
-00020d70: 7363 7269 7074 696f 6e2e 7661 6c75 6520  scription.value 
-00020d80: 3d20 6669 6c65 6461 7461 5b22 6465 7363  = filedata["desc
-00020d90: 7269 7074 696f 6e22 5d0d 0a0d 0a20 2020  ription"]....   
-00020da0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00020db0: 656c 662e 7061 7265 6e74 2e66 6c6f 775f  elf.parent.flow_
-00020dc0: 6368 6563 6b2e 7661 6c75 6520 3d20 6669  check.value = fi
-00020dd0: 6c65 6461 7461 5b22 6c6f 6720 7472 616e  ledata["log tran
-00020de0: 7361 6374 696f 6e22 5d0d 0a20 2020 2020  saction"]..     
-00020df0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00020e00: 662e 7061 7265 6e74 2e6b 696e 642e 7661  f.parent.kind.va
-00020e10: 6c75 6520 3d20 6669 6c65 6461 7461 5b22  lue = filedata["
-00020e20: 6b69 6e64 225d 0d0a 2020 2020 2020 2020  kind"]..        
-00020e30: 2020 2020 2020 2020 2320 7365 6c66 2e70          # self.p
-00020e40: 6172 656e 742e 7375 626a 6563 742e 7661  arent.subject.va
-00020e50: 6c75 6520 3d20 6669 6c65 6461 7461 5b22  lue = filedata["
-00020e60: 7375 626a 6563 7422 5d0d 0a20 2020 2020  subject"]..     
-00020e70: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00020e80: 662e 7061 7265 6e74 2e71 7561 6e74 6974  f.parent.quantit
-00020e90: 792e 7661 6c75 6520 3d20 6669 6c65 6461  y.value = fileda
-00020ea0: 7461 5b22 7175 616e 7469 7479 225d 0d0a  ta["quantity"]..
-00020eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020ec0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00020ed0: 2020 2020 2020 2020 2020 2020 2320 5b22              # ["
-00020ee0: 4e6f 6e65 222c 2252 6576 656e 7565 222c  None","Revenue",
-00020ef0: 2245 7870 656e 7365 222c 2247 6169 6e22  "Expense","Gain"
-00020f00: 2c22 4c6f 7373 222c 2254 6178 225d 0d0a  ,"Loss","Tax"]..
-00020f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00020f20: 2020 2020 2020 6d79 5f64 6963 7420 3d20        my_dict = 
-00020f30: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00020f40: 2020 2020 2020 2020 2020 2022 4e6f 6e65             "None
-00020f50: 223a 2030 2c0d 0a20 2020 2020 2020 2020  ": 0,..         
-00020f60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00020f70: 5265 7665 6e75 6522 3a20 312c 0d0a 2020  Revenue": 1,..  
-00020f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f90: 2020 2020 2020 2245 7870 656e 7365 223a        "Expense":
-00020fa0: 2032 2c0d 0a20 2020 2020 2020 2020 2020   2,..           
-00020fb0: 2020 2020 2020 2020 2020 2020 2022 4761               "Ga
-00020fc0: 696e 223a 2033 2c0d 0a20 2020 2020 2020  in": 3,..       
-00020fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fe0: 2022 4c6f 7373 223a 2034 2c0d 0a20 2020   "Loss": 4,..   
-00020ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021000: 2020 2020 2022 496e 7465 7265 7374 223a       "Interest":
-00021010: 2035 2c0d 0a20 2020 2020 2020 2020 2020   5,..           
-00021020: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
-00021030: 6e2d 4f70 2e20 496e 636f 6d65 223a 2036  n-Op. Income": 6
-00021040: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00021050: 2020 2020 2020 2020 2020 2022 5461 7822             "Tax"
-00021060: 3a20 372c 0d0a 2020 2020 2020 2020 2020  : 7,..          
-00021070: 2020 2020 2020 2020 2020 2020 2020 224e                "N
-00021080: 6f6e 7461 782e 2050 726f 6669 7422 3a20  ontax. Profit": 
-00021090: 382c 0d0a 2020 2020 2020 2020 2020 2020  8,..            
-000210a0: 2020 2020 2020 2020 2020 2020 224e 6f6e              "Non
-000210b0: 7461 782e 204c 6f73 7322 3a20 390d 0a20  tax. Loss": 9.. 
+000201a0: 2073 7472 2873 656c 662e 636f 6d62 6f43   str(self.comboC
+000201b0: 6173 6852 6967 6874 2e63 7572 7265 6e74  ashRight.current
+000201c0: 5465 7874 2829 290d 0a0d 0a20 2020 2020  Text())....     
+000201d0: 2020 206e 6577 5f65 6e74 7279 5b22 6b69     new_entry["ki
+000201e0: 6e64 225d 203d 205c 0d0a 2020 2020 2020  nd"] = \..      
+000201f0: 2020 2020 2020 7374 7228 7365 6c66 2e65        str(self.e
+00020200: 6469 7454 7970 652e 6375 7272 656e 7454  ditType.currentT
+00020210: 6578 7428 2929 0d0a 0d0a 2020 2020 2020  ext())....      
+00020220: 2020 6e65 775f 656e 7472 795b 2269 6e63    new_entry["inc
+00020230: 6f6d 6531 225d 203d 205c 0d0a 2020 2020  ome1"] = \..    
+00020240: 2020 2020 2020 2020 7374 7228 7365 6c66          str(self
+00020250: 2e63 6f6d 626f 496e 636f 6d65 4c65 6674  .comboIncomeLeft
+00020260: 2e63 7572 7265 6e74 5465 7874 2829 290d  .currentText()).
+00020270: 0a20 2020 2020 2020 206e 6577 5f65 6e74  .        new_ent
+00020280: 7279 5b22 696e 636f 6d65 3222 5d20 3d20  ry["income2"] = 
+00020290: 5c0d 0a20 2020 2020 2020 2020 2020 2073  \..            s
+000202a0: 7472 2873 656c 662e 636f 6d62 6f49 6e63  tr(self.comboInc
+000202b0: 6f6d 6552 6967 6874 2e63 7572 7265 6e74  omeRight.current
+000202c0: 5465 7874 2829 290d 0a0d 0a20 2020 2020  Text())....     
+000202d0: 2020 206e 6577 5f65 6e74 7279 5b22 7175     new_entry["qu
+000202e0: 616e 7469 7479 225d 203d 205c 0d0a 2020  antity"] = \..  
+000202f0: 2020 2020 2020 2020 2020 7374 7228 7365            str(se
+00020300: 6c66 2e65 6469 7451 7561 6e74 6974 792e  lf.editQuantity.
+00020310: 7465 7874 2829 290d 0a0d 0a20 2020 2020  text())....     
+00020320: 2020 206e 6577 5f65 6e74 7279 5b22 7375     new_entry["su
+00020330: 626a 6563 7422 5d20 3d20 5c0d 0a20 2020  bject"] = \..   
+00020340: 2020 2020 2020 2020 2073 7472 2873 656c           str(sel
+00020350: 662e 6564 6974 5375 626a 6563 742e 7465  f.editSubject.te
+00020360: 7874 2829 290d 0a0d 0a20 2020 2020 2020  xt())....       
+00020370: 206e 6577 5f65 6e74 7279 5b22 7368 6f72   new_entry["shor
+00020380: 746e 616d 6522 5d20 3d20 5c0d 0a20 2020  tname"] = \..   
+00020390: 2020 2020 2020 2020 2073 7472 2873 656c           str(sel
+000203a0: 662e 6564 6974 5368 6f72 746e 616d 652e  f.editShortname.
+000203b0: 7465 7874 2829 290d 0a0d 0a20 2020 2020  text())....     
+000203c0: 2020 206e 6577 5f65 6e74 7279 5b22 6465     new_entry["de
+000203d0: 7363 7269 7074 696f 6e22 5d20 3d20 5c0d  scription"] = \.
+000203e0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+000203f0: 2873 656c 662e 6564 6974 4465 7363 7269  (self.editDescri
+00020400: 7074 696f 6e2e 7465 7874 2829 290d 0a0d  ption.text())...
+00020410: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+00020420: 7472 795f 6461 7461 2e61 7070 656e 6428  try_data.append(
+00020430: 6e65 775f 656e 7472 7929 0d0a 2020 2020  new_entry)..    
+00020440: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+00020450: 7461 626c 6528 290d 0a0d 0a0d 0a0d 0a20  table()........ 
+00020460: 2020 2020 2020 2064 6172 6b4d 6f64 6520         darkMode 
+00020470: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+00020480: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00020490: 2020 6966 2073 656c 662e 7468 656d 655f    if self.theme_
+000204a0: 6d61 6e61 6765 722e 7468 656d 6520 3d3d  manager.theme ==
+000204b0: 2022 6272 6967 6874 223a 0d0a 2020 2020   "bright":..    
+000204c0: 2020 2020 2020 2020 2020 2020 6461 726b              dark
+000204d0: 4d6f 6465 203d 2046 616c 7365 0d0a 2020  Mode = False..  
+000204e0: 2020 2020 2020 6578 6365 7074 3a0d 0a20        except:.. 
+000204f0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00020500: 0a0d 0a20 2020 2020 2020 2074 7279 3a0d  ...        try:.
+00020510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00020520: 662e 7365 6c65 6374 696f 6e5f 6964 7820  f.selection_idx 
+00020530: 3d20 6c65 6e28 7365 6c66 2e65 6e74 7279  = len(self.entry
+00020540: 5f64 6174 6129 2d31 0d0a 2020 2020 2020  _data)-1..      
+00020550: 2020 2020 2020 7365 6c66 2e72 6f77 5f73        self.row_s
+00020560: 656c 6563 7428 7365 6c66 2e73 656c 6563  elect(self.selec
+00020570: 7469 6f6e 5f69 6478 290d 0a20 2020 2020  tion_idx)..     
+00020580: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00020590: 696f 6e20 6173 2065 203a 0d0a 2020 2020  ion as e :..    
+000205a0: 2020 2020 2020 2020 7365 6c66 2e6e 6f74          self.not
+000205b0: 6966 7928 2245 5252 4f52 3a22 202b 2074  ify("ERROR:" + t
+000205c0: 7228 6529 2c74 6974 6c65 3d22 4572 726f  r(e),title="Erro
+000205d0: 7222 290d 0a0d 0a20 2020 2020 2020 2022  r")....        "
+000205e0: 2222 0d0a 2020 2020 2020 2020 6966 2073  ""..        if s
+000205f0: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
+00020600: 7820 6973 206e 6f74 204e 6f6e 653a 0d0a  x is not None:..
+00020610: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00020620: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
+00020630: 7472 616e 7361 6374 696f 6e56 6965 772e  transactionView.
+00020640: 636f 6c75 6d6e 436f 756e 7428 2929 3a0d  columnCount()):.
+00020650: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00020660: 2020 2069 6620 6461 726b 4d6f 6465 3a0d     if darkMode:.
+00020670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020680: 2020 2020 2073 656c 662e 7472 616e 7361       self.transa
+00020690: 6374 696f 6e56 6965 772e 6974 656d 2873  ctionView.item(s
+000206a0: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
+000206b0: 782c 2069 292e 7365 7442 6163 6b67 726f  x, i).setBackgro
+000206c0: 756e 6428 5174 4775 692e 5143 6f6c 6f72  und(QtGui.QColor
+000206d0: 2832 312c 2032 312c 2032 3129 290d 0a20  (21, 21, 21)).. 
+000206e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000206f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00020700: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00020710: 7261 6e73 6163 7469 6f6e 5669 6577 2e69  ransactionView.i
+00020720: 7465 6d28 7365 6c66 2e73 656c 6563 7469  tem(self.selecti
+00020730: 6f6e 5f69 6478 2c20 6929 2e73 6574 4261  on_idx, i).setBa
+00020740: 636b 6772 6f75 6e64 2851 7447 7569 2e51  ckground(QtGui.Q
+00020750: 436f 6c6f 7228 3233 332c 2032 3334 2c20  Color(233, 234, 
+00020760: 3232 3729 290d 0a0d 0a20 2020 2020 2020  227))....       
+00020770: 2020 2020 2073 656c 662e 7365 6c65 6374       self.select
+00020780: 696f 6e5f 6964 7820 3d20 7365 6c66 2e74  ion_idx = self.t
+00020790: 7261 6e73 6163 7469 6f6e 5669 6577 2e72  ransactionView.r
+000207a0: 6f77 436f 756e 7428 292d 310d 0a20 2020  owCount()-1..   
+000207b0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000207c0: 6e20 7261 6e67 6528 7365 6c66 2e74 7261  n range(self.tra
+000207d0: 6e73 6163 7469 6f6e 5669 6577 2e63 6f6c  nsactionView.col
+000207e0: 756d 6e43 6f75 6e74 2829 293a 0d0a 2020  umnCount()):..  
+000207f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00020800: 2064 6172 6b4d 6f64 653a 0d0a 2020 2020   darkMode:..    
+00020810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020820: 7365 6c66 2e74 7261 6e73 6163 7469 6f6e  self.transaction
+00020830: 5669 6577 2e69 7465 6d28 7365 6c66 2e73  View.item(self.s
+00020840: 656c 6563 7469 6f6e 5f69 6478 2c20 6929  election_idx, i)
+00020850: 2e73 6574 4261 636b 6772 6f75 6e64 2851  .setBackground(Q
+00020860: 7447 7569 2e51 436f 6c6f 7228 3138 2c20  tGui.QColor(18, 
+00020870: 3138 2c20 3138 2929 0d0a 2020 2020 2020  18, 18))..      
+00020880: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00020890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000208a0: 2020 2020 2073 656c 662e 7472 616e 7361       self.transa
+000208b0: 6374 696f 6e56 6965 772e 6974 656d 2873  ctionView.item(s
+000208c0: 656c 662e 7365 6c65 6374 696f 6e5f 6964  elf.selection_id
+000208d0: 782c 2069 292e 7365 7442 6163 6b67 726f  x, i).setBackgro
+000208e0: 756e 6428 5174 4775 692e 5143 6f6c 6f72  und(QtGui.QColor
+000208f0: 2831 3539 2c20 3135 392c 2031 3539 2929  (159, 159, 159))
+00020900: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
+00020910: 0a0d 0a0d 0a0d 0a20 2020 2064 6566 2067  .......    def g
+00020920: 6f74 6f5f 6e65 7874 2873 656c 6629 3a0d  oto_next(self):.
+00020930: 0a20 2020 2020 2020 2070 6173 730d 0a0d  .        pass...
+00020940: 0a0d 0a20 2020 2064 6566 2075 6470 6174  ...    def udpat
+00020950: 655f 6469 7370 6c61 7928 7365 6c66 293a  e_display(self):
+00020960: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00020970: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+00020980: 6c65 6e61 6d65 203d 2073 656c 662e 6669  lename = self.fi
+00020990: 6c65 6e61 6d65 0d0a 0d0a 2020 2020 2020  lename....      
+000209a0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+000209b0: 6669 6c65 6e61 6d65 2c20 2772 2729 2061  filename, 'r') a
+000209c0: 7320 7374 7265 616d 3a0d 0a20 2020 2020  s stream:..     
+000209d0: 2020 2020 2020 2020 2020 2066 696c 6564             filed
+000209e0: 6174 6120 3d20 7961 6d6c 2e73 6166 655f  ata = yaml.safe_
+000209f0: 6c6f 6164 2873 7472 6561 6d29 0d0a 2020  load(stream)..  
+00020a00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00020a10: 696e 7428 6669 6c65 6461 7461 290d 0a0d  int(filedata)...
+00020a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020a30: 2073 656c 662e 6167 656e 7431 4c61 6265   self.agent1Labe
+00020a40: 6c2e 7465 7874 203d 2066 696c 6564 6174  l.text = filedat
+00020a50: 615b 2261 6765 6e74 3122 5d0d 0a20 2020  a["agent1"]..   
+00020a60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00020a70: 662e 6167 656e 7432 4c61 6265 6c2e 7465  f.agent2Label.te
+00020a80: 7874 203d 2066 696c 6564 6174 615b 2261  xt = filedata["a
+00020a90: 6765 6e74 3222 5d0d 0a0d 0a20 2020 2020  gent2"]....     
+00020aa0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00020ab0: 662e 6131 2e76 616c 7565 203d 2066 696c  f.a1.value = fil
+00020ac0: 6564 6174 615b 2261 3122 5d20 2023 202b  edata["a1"]  # +
+00020ad0: 2022 5c6e 220d 0a20 2020 2020 2020 2020   "\n"..         
+00020ae0: 2020 2020 2020 2023 2073 656c 662e 6531         # self.e1
+00020af0: 2e76 616c 7565 203d 2066 696c 6564 6174  .value = filedat
+00020b00: 615b 2265 3122 5d20 2023 202b 2022 5c6e  a["e1"]  # + "\n
+00020b10: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00020b20: 2020 2023 2073 656c 662e 6c31 2e76 616c     # self.l1.val
+00020b30: 7565 203d 2066 696c 6564 6174 615b 226c  ue = filedata["l
+00020b40: 3122 5d20 2023 202b 2022 5c6e 220d 0a20  1"]  # + "\n".. 
+00020b50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00020b60: 2073 656c 662e 6132 2e76 616c 7565 203d   self.a2.value =
+00020b70: 2066 696c 6564 6174 615b 2261 3222 5d20   filedata["a2"] 
+00020b80: 2023 202b 2022 5c6e 220d 0a20 2020 2020   # + "\n"..     
+00020b90: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00020ba0: 662e 6532 2e76 616c 7565 203d 2066 696c  f.e2.value = fil
+00020bb0: 6564 6174 615b 2265 3222 5d20 2023 202b  edata["e2"]  # +
+00020bc0: 2022 5c6e 220d 0a20 2020 2020 2020 2020   "\n"..         
+00020bd0: 2020 2020 2020 2023 2073 656c 662e 6c32         # self.l2
+00020be0: 2e76 616c 7565 203d 2066 696c 6564 6174  .value = filedat
+00020bf0: 615b 226c 3222 5d20 2023 202b 2022 5c6e  a["l2"]  # + "\n
+00020c00: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
+00020c10: 2020 2020 2023 2069 6620 2273 686f 7274       # if "short
+00020c20: 6e61 6d65 2220 696e 2066 696c 6564 6174  name" in filedat
+00020c30: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
+00020c40: 2020 2020 2320 2020 2073 656c 662e 7061      #    self.pa
+00020c50: 7265 6e74 2e73 686f 7274 6e61 6d65 2e76  rent.shortname.v
+00020c60: 616c 7565 203d 2066 696c 6564 6174 615b  alue = filedata[
+00020c70: 2273 686f 7274 6e61 6d65 225d 0d0a 0d0a  "shortname"]....
+00020c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c90: 2320 6966 2022 756e 692d 6469 7265 6374  # if "uni-direct
+00020ca0: 696f 6e61 6c22 2069 6e20 6669 6c65 6461  ional" in fileda
+00020cb0: 7461 3a0d 0a20 2020 2020 2020 2020 2020  ta:..           
+00020cc0: 2020 2020 2023 2020 2020 7365 6c66 2e70       #    self.p
+00020cd0: 6172 656e 742e 6469 7265 6374 696f 6e5f  arent.direction_
+00020ce0: 6368 6563 6b2e 7661 6c75 6520 3d20 626f  check.value = bo
+00020cf0: 6f6c 2873 7472 2866 696c 6564 6174 615b  ol(str(filedata[
+00020d00: 2275 6e69 2d64 6972 6563 7469 6f6e 616c  "uni-directional
+00020d10: 225d 2929 0d0a 2020 2020 2020 2020 2020  "]))..          
+00020d20: 2020 2020 2020 2320 656c 7365 3a0d 0a20        # else:.. 
+00020d30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00020d40: 2020 2020 7365 6c66 2e70 6172 656e 742e      self.parent.
+00020d50: 6469 7265 6374 696f 6e5f 6368 6563 6b2e  direction_check.
+00020d60: 7661 6c75 6520 3d20 4661 6c73 650d 0a0d  value = False...
+00020d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020d80: 2023 2069 6620 2264 6573 6372 6970 7469   # if "descripti
+00020d90: 6f6e 2220 696e 2066 696c 6564 6174 613a  on" in filedata:
+00020da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020db0: 2020 2320 2020 2073 656c 662e 7061 7265    #    self.pare
+00020dc0: 6e74 2e64 6573 6372 6970 7469 6f6e 2e76  nt.description.v
+00020dd0: 616c 7565 203d 2066 696c 6564 6174 615b  alue = filedata[
+00020de0: 2264 6573 6372 6970 7469 6f6e 225d 0d0a  "description"]..
+00020df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020e00: 2020 2320 7365 6c66 2e70 6172 656e 742e    # self.parent.
+00020e10: 666c 6f77 5f63 6865 636b 2e76 616c 7565  flow_check.value
+00020e20: 203d 2066 696c 6564 6174 615b 226c 6f67   = filedata["log
+00020e30: 2074 7261 6e73 6163 7469 6f6e 225d 0d0a   transaction"]..
+00020e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e50: 2320 7365 6c66 2e70 6172 656e 742e 6b69  # self.parent.ki
+00020e60: 6e64 2e76 616c 7565 203d 2066 696c 6564  nd.value = filed
+00020e70: 6174 615b 226b 696e 6422 5d0d 0a20 2020  ata["kind"]..   
+00020e80: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00020e90: 656c 662e 7061 7265 6e74 2e73 7562 6a65  elf.parent.subje
+00020ea0: 6374 2e76 616c 7565 203d 2066 696c 6564  ct.value = filed
+00020eb0: 6174 615b 2273 7562 6a65 6374 225d 0d0a  ata["subject"]..
+00020ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ed0: 2320 7365 6c66 2e70 6172 656e 742e 7175  # self.parent.qu
+00020ee0: 616e 7469 7479 2e76 616c 7565 203d 2066  antity.value = f
+00020ef0: 696c 6564 6174 615b 2271 7561 6e74 6974  iledata["quantit
+00020f00: 7922 5d0d 0a0d 0a20 2020 2020 2020 2020  y"]....         
+00020f10: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00020f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f30: 2023 205b 224e 6f6e 6522 2c22 5265 7665   # ["None","Reve
+00020f40: 6e75 6522 2c22 4578 7065 6e73 6522 2c22  nue","Expense","
+00020f50: 4761 696e 222c 224c 6f73 7322 2c22 5461  Gain","Loss","Ta
+00020f60: 7822 5d0d 0a0d 0a20 2020 2020 2020 2020  x"]....         
+00020f70: 2020 2020 2020 2020 2020 206d 795f 6469             my_di
+00020f80: 6374 203d 207b 0d0a 2020 2020 2020 2020  ct = {..        
+00020f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fa0: 224e 6f6e 6522 3a20 302c 0d0a 2020 2020  "None": 0,..    
+00020fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fc0: 2020 2020 2252 6576 656e 7565 223a 2031      "Revenue": 1
+00020fd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00020fe0: 2020 2020 2020 2020 2020 2022 4578 7065             "Expe
+00020ff0: 6e73 6522 3a20 322c 0d0a 2020 2020 2020  nse": 2,..      
+00021000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021010: 2020 2247 6169 6e22 3a20 332c 0d0a 2020    "Gain": 3,..  
+00021020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021030: 2020 2020 2020 224c 6f73 7322 3a20 342c        "Loss": 4,
+00021040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021050: 2020 2020 2020 2020 2020 2249 6e74 6572            "Inter
+00021060: 6573 7422 3a20 352c 0d0a 2020 2020 2020  est": 5,..      
+00021070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021080: 2020 224e 6f6e 2d4f 702e 2049 6e63 6f6d    "Non-Op. Incom
+00021090: 6522 3a20 362c 0d0a 2020 2020 2020 2020  e": 6,..        
+000210a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210b0: 2254 6178 223a 2037 2c0d 0a20 2020 2020  "Tax": 7,..     
 000210c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210d0: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-000210e0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-000210f0: 6c66 2e70 6172 656e 742e 696e 636f 6d65  lf.parent.income
-00021100: 312e 7661 6c75 6520 3d20 5b6d 795f 6469  1.value = [my_di
-00021110: 6374 5b66 696c 6564 6174 615b 2269 6e63  ct[filedata["inc
-00021120: 6f6d 6531 225d 5d5d 0d0a 2020 2020 2020  ome1"]]]..      
-00021130: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00021140: 7365 6c66 2e70 6172 656e 742e 696e 636f  self.parent.inco
-00021150: 6d65 322e 7661 6c75 6520 3d20 5b6d 795f  me2.value = [my_
-00021160: 6469 6374 5b66 696c 6564 6174 615b 2269  dict[filedata["i
-00021170: 6e63 6f6d 6532 225d 5d5d 0d0a 0d0a 2020  ncome2"]]]....  
+000210d0: 2020 2022 4e6f 6e74 6178 2e20 5072 6f66     "Nontax. Prof
+000210e0: 6974 223a 2038 2c0d 0a20 2020 2020 2020  it": 8,..       
+000210f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021100: 2022 4e6f 6e74 6178 2e20 4c6f 7373 223a   "Nontax. Loss":
+00021110: 2039 0d0a 2020 2020 2020 2020 2020 2020   9..            
+00021120: 2020 2020 2020 2020 7d0d 0a0d 0a20 2020          }....   
+00021130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021140: 2023 2073 656c 662e 7061 7265 6e74 2e69   # self.parent.i
+00021150: 6e63 6f6d 6531 2e76 616c 7565 203d 205b  ncome1.value = [
+00021160: 6d79 5f64 6963 745b 6669 6c65 6461 7461  my_dict[filedata
+00021170: 5b22 696e 636f 6d65 3122 5d5d 5d0d 0a20  ["income1"]]].. 
 00021180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021190: 2020 2320 7365 6c66 2e70 6172 656e 742e    # self.parent.
-000211a0: 6361 7368 666c 6f77 312e 7661 6c75 6520  cashflow1.value 
-000211b0: 3d20 5b66 696c 6564 6174 615b 2263 6173  = [filedata["cas
-000211c0: 6866 6c6f 7731 225d 5d0d 0a20 2020 2020  hflow1"]]..     
-000211d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000211e0: 2073 656c 662e 7061 7265 6e74 2e63 6173   self.parent.cas
-000211f0: 6866 6c6f 7732 2e76 616c 7565 203d 205b  hflow2.value = [
-00021200: 6669 6c65 6461 7461 5b22 6361 7368 666c  filedata["cashfl
-00021210: 6f77 3222 5d5d 0d0a 0d0a 2020 2020 2020  ow2"]]....      
-00021220: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00021230: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00021240: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
-00021250: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00021260: 7365 6c66 2e70 6172 656e 742e 6469 7370  self.parent.disp
-00021270: 6c61 7928 290d 0a0d 0a20 2020 2020 2020  lay()....       
-00021280: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00021290: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-000212a0: 2020 2020 2070 7269 6e74 2873 7472 2865       print(str(e
-000212b0: 2929 2023 2073 656c 662e 6e6f 7469 6679  )) # self.notify
-000212c0: 2873 7472 2865 292c 2245 7863 6570 7469  (str(e),"Excepti
-000212d0: 6f6e 2229 203c 2074 6869 7320 7368 6f75  on") < this shou
-000212e0: 6c64 206e 6f74 2074 6872 6f77 2061 6e20  ld not throw an 
-000212f0: 6578 6365 7074 696f 6e0d 0a0d 0a0d 0a0d  exception.......
-00021300: 0a64 6566 2072 756e 5f61 7070 2829 3a0d  .def run_app():.
-00021310: 0a20 2020 2023 2072 756e 7320 7468 6520  .    # runs the 
-00021320: 6d61 696e 2061 7070 6c69 6361 7469 6f6e  main application
-00021330: 2077 696e 646f 770d 0a0d 0a20 2020 2061   window....    a
-00021340: 7070 203d 2051 7457 6964 6765 7473 2e51  pp = QtWidgets.Q
-00021350: 4170 706c 6963 6174 696f 6e28 7379 732e  Application(sys.
-00021360: 6172 6776 290d 0a0d 0a20 2020 2023 2070  argv)....    # p
-00021370: 6978 6d61 7020 3d20 5150 6978 6d61 7028  ixmap = QPixmap(
-00021380: 222e 2f73 706c 6173 682e 706e 6722 290d  "./splash.png").
-00021390: 0a20 2020 2023 2073 706c 6173 6820 3d20  .    # splash = 
-000213a0: 5153 706c 6173 6853 6372 6565 6e28 7069  QSplashScreen(pi
-000213b0: 786d 6170 290d 0a20 2020 2023 2073 706c  xmap)..    # spl
-000213c0: 6173 682e 7368 6f77 2829 0d0a 0d0a 2020  ash.show()....  
-000213d0: 2020 2320 6170 702e 7365 7453 7479 6c65    # app.setStyle
-000213e0: 2827 4675 7369 6f6e 2729 0d0a 0d0a 2020  ('Fusion')....  
-000213f0: 2020 7769 6e64 6f77 203d 2054 7261 6e73    window = Trans
-00021400: 6163 7469 6f6e 4465 7369 676e 6572 2829  actionDesigner()
-00021410: 0d0a 2020 2020 2320 7370 6c61 7368 2e66  ..    # splash.f
-00021420: 696e 6973 6828 7769 6e64 6f77 290d 0a0d  inish(window)...
-00021430: 0a20 2020 2023 2073 6574 7570 2073 7479  .    # setup sty
-00021440: 6c65 7368 6565 740d 0a20 2020 2023 2061  lesheet..    # a
-00021450: 7070 6c79 5f73 7479 6c65 7368 6565 7428  pply_stylesheet(
-00021460: 6170 702c 2074 6865 6d65 3d27 6461 726b  app, theme='dark
-00021470: 5f74 6561 6c2e 786d 6c27 2c20 696e 7665  _teal.xml', inve
-00021480: 7274 5f73 6563 6f6e 6461 7279 3d54 7275  rt_secondary=Tru
-00021490: 6529 0d0a 2020 2020 2320 6170 706c 795f  e)..    # apply_
-000214a0: 7374 796c 6573 6865 6574 2877 696e 646f  stylesheet(windo
-000214b0: 772c 2074 6865 6d65 3d27 6461 726b 5f74  w, theme='dark_t
-000214c0: 6561 6c2e 786d 6c27 2c20 696e 7665 7274  eal.xml', invert
-000214d0: 5f73 6563 6f6e 6461 7279 3d54 7275 6529  _secondary=True)
-000214e0: 0d0a 0d0a 2020 2020 7769 6e64 6f77 2e73  ....    window.s
-000214f0: 686f 7728 290d 0a20 2020 2077 696e 646f  how()..    windo
-00021500: 772e 7377 6974 6368 5f74 6865 6d65 2829  w.switch_theme()
-00021510: 0d0a 2020 2020 7769 6e64 6f77 2e73 7769  ..    window.swi
-00021520: 7463 685f 7468 656d 6528 290d 0a0d 0a20  tch_theme().... 
-00021530: 2020 2061 7070 2e65 7865 635f 2829 0d0a     app.exec_()..
-00021540: 0d0a 0d0a 0d0a 0d0a 0d0a 6966 205f 5f6e  ..........if __n
-00021550: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
-00021560: 5f5f 223a 0d0a 0d0a 2020 2020 7275 6e5f  __":....    run_
-00021570: 6170 7028 290d 0a                        app()..
+00021190: 2020 2023 2073 656c 662e 7061 7265 6e74     # self.parent
+000211a0: 2e69 6e63 6f6d 6532 2e76 616c 7565 203d  .income2.value =
+000211b0: 205b 6d79 5f64 6963 745b 6669 6c65 6461   [my_dict[fileda
+000211c0: 7461 5b22 696e 636f 6d65 3222 5d5d 5d0d  ta["income2"]]].
+000211d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000211e0: 2020 2020 2020 2023 2073 656c 662e 7061         # self.pa
+000211f0: 7265 6e74 2e63 6173 6866 6c6f 7731 2e76  rent.cashflow1.v
+00021200: 616c 7565 203d 205b 6669 6c65 6461 7461  alue = [filedata
+00021210: 5b22 6361 7368 666c 6f77 3122 5d5d 0d0a  ["cashflow1"]]..
+00021220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021230: 2020 2020 2320 7365 6c66 2e70 6172 656e      # self.paren
+00021240: 742e 6361 7368 666c 6f77 322e 7661 6c75  t.cashflow2.valu
+00021250: 6520 3d20 5b66 696c 6564 6174 615b 2263  e = [filedata["c
+00021260: 6173 6866 6c6f 7732 225d 5d0d 0a0d 0a20  ashflow2"]].... 
+00021270: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00021280: 7863 6570 743a 0d0a 2020 2020 2020 2020  xcept:..        
+00021290: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+000212a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000212b0: 2020 2020 2373 656c 662e 7061 7265 6e74      #self.parent
+000212c0: 2e64 6973 706c 6179 2829 0d0a 0d0a 2020  .display()....  
+000212d0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000212e0: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+000212f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00021300: 7374 7228 6529 2920 2320 7365 6c66 2e6e  str(e)) # self.n
+00021310: 6f74 6966 7928 7374 7228 6529 2c22 4578  otify(str(e),"Ex
+00021320: 6365 7074 696f 6e22 2920 3c20 7468 6973  ception") < this
+00021330: 2073 686f 756c 6420 6e6f 7420 7468 726f   should not thro
+00021340: 7720 616e 2065 7863 6570 7469 6f6e 0d0a  w an exception..
+00021350: 0d0a 0d0a 0d0a 6465 6620 7275 6e5f 6170  ......def run_ap
+00021360: 7028 293a 0d0a 2020 2020 2320 7275 6e73  p():..    # runs
+00021370: 2074 6865 206d 6169 6e20 6170 706c 6963   the main applic
+00021380: 6174 696f 6e20 7769 6e64 6f77 0d0a 0d0a  ation window....
+00021390: 2020 2020 6170 7020 3d20 5174 5769 6467      app = QtWidg
+000213a0: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
+000213b0: 2873 7973 2e61 7267 7629 0d0a 0d0a 2020  (sys.argv)....  
+000213c0: 2020 2320 7069 786d 6170 203d 2051 5069    # pixmap = QPi
+000213d0: 786d 6170 2822 2e2f 7370 6c61 7368 2e70  xmap("./splash.p
+000213e0: 6e67 2229 0d0a 2020 2020 2320 7370 6c61  ng")..    # spla
+000213f0: 7368 203d 2051 5370 6c61 7368 5363 7265  sh = QSplashScre
+00021400: 656e 2870 6978 6d61 7029 0d0a 2020 2020  en(pixmap)..    
+00021410: 2320 7370 6c61 7368 2e73 686f 7728 290d  # splash.show().
+00021420: 0a0d 0a20 2020 2023 2061 7070 2e73 6574  ...    # app.set
+00021430: 5374 796c 6528 2746 7573 696f 6e27 290d  Style('Fusion').
+00021440: 0a0d 0a20 2020 2077 696e 646f 7720 3d20  ...    window = 
+00021450: 5472 616e 7361 6374 696f 6e44 6573 6967  TransactionDesig
+00021460: 6e65 7228 290d 0a20 2020 2023 2073 706c  ner()..    # spl
+00021470: 6173 682e 6669 6e69 7368 2877 696e 646f  ash.finish(windo
+00021480: 7729 0d0a 0d0a 2020 2020 2320 7365 7475  w)....    # setu
+00021490: 7020 7374 796c 6573 6865 6574 0d0a 2020  p stylesheet..  
+000214a0: 2020 2320 6170 706c 795f 7374 796c 6573    # apply_styles
+000214b0: 6865 6574 2861 7070 2c20 7468 656d 653d  heet(app, theme=
+000214c0: 2764 6172 6b5f 7465 616c 2e78 6d6c 272c  'dark_teal.xml',
+000214d0: 2069 6e76 6572 745f 7365 636f 6e64 6172   invert_secondar
+000214e0: 793d 5472 7565 290d 0a20 2020 2023 2061  y=True)..    # a
+000214f0: 7070 6c79 5f73 7479 6c65 7368 6565 7428  pply_stylesheet(
+00021500: 7769 6e64 6f77 2c20 7468 656d 653d 2764  window, theme='d
+00021510: 6172 6b5f 7465 616c 2e78 6d6c 272c 2069  ark_teal.xml', i
+00021520: 6e76 6572 745f 7365 636f 6e64 6172 793d  nvert_secondary=
+00021530: 5472 7565 290d 0a0d 0a20 2020 2077 696e  True)....    win
+00021540: 646f 772e 7368 6f77 2829 0d0a 2020 2020  dow.show()..    
+00021550: 7769 6e64 6f77 2e73 7769 7463 685f 7468  window.switch_th
+00021560: 656d 6528 290d 0a20 2020 2077 696e 646f  eme()..    windo
+00021570: 772e 7377 6974 6368 5f74 6865 6d65 2829  w.switch_theme()
+00021580: 0d0a 0d0a 2020 2020 6170 702e 6578 6563  ....    app.exec
+00021590: 5f28 290d 0a0d 0a0d 0a0d 0a0d 0a0d 0a69  _()............i
+000215a0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+000215b0: 5f6d 6169 6e5f 5f22 3a0d 0a0d 0a20 2020  _main__":....   
+000215c0: 2072 756e 5f61 7070 2829 0d0a             run_app()..
```

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.6.4/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.6.4/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.6.4/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.6.4/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.6.4/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/CLA.pdf` & `sfctools-1.0.6.4/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.6.4/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/LICENSE` & `sfctools-1.0.6.4/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/gui/README.md` & `sfctools-1.0.6.4/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.6.4/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.6.4/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/sfctools/misc/timeseries.py` & `sfctools-1.0.6.4/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.6.3/setup.py` & `sfctools-1.0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.6.3',
+    'version': '1.0.6.4',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.6.3/PKG-INFO` & `sfctools-1.0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.6.3
+Version: 1.0.6.4
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

