# Comparing `tmp/sfctools-1.0.5.7.tar.gz` & `tmp/sfctools-1.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.5.7.tar", max compression
+gzip compressed data, was "sfctools-1.0.5.8.tar", max compression
```

## Comparing `sfctools-1.0.5.7.tar` & `sfctools-1.0.5.8.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1157 2022-07-11 05:48:16.488771 sfctools-1.0.5.7/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-02 14:48:01.301162 sfctools-1.0.5.7/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-20 13:09:06.583059 sfctools-1.0.5.7/README.md
--rw-r--r--   0        0        0     1938 2022-09-30 18:37:37.788985 sfctools-1.0.5.7/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-03-20 13:09:02.730363 sfctools-1.0.5.7/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:24.669104 sfctools-1.0.5.7/sfctools/automation/__init__.py
--rw-r--r--   0        0        0    10574 2023-03-20 13:09:06.605805 sfctools-1.0.5.7/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-20 13:09:06.606808 sfctools-1.0.5.7/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-09-30 16:39:54.806932 sfctools-1.0.5.7/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:24.973114 sfctools-1.0.5.7/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0     8900 2023-03-20 13:09:02.731669 sfctools-1.0.5.7/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-20 13:09:06.607816 sfctools-1.0.5.7/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-07-11 05:48:25.096539 sfctools-1.0.5.7/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-07-11 05:48:25.136548 sfctools-1.0.5.7/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-09-30 17:46:40.211773 sfctools-1.0.5.7/sfctools/core/__init__.py
--rw-r--r--   0        0        0     7572 2022-09-30 18:03:18.887479 sfctools-1.0.5.7/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-10-06 06:50:49.792046 sfctools-1.0.5.7/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-20 13:09:06.608843 sfctools-1.0.5.7/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-20 13:09:06.609847 sfctools-1.0.5.7/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-20 13:09:06.609847 sfctools-1.0.5.7/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-10-06 06:49:21.703590 sfctools-1.0.5.7/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-03-20 13:09:02.733973 sfctools-1.0.5.7/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-07-11 05:48:26.022730 sfctools-1.0.5.7/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0    32494 2023-03-20 13:09:06.610850 sfctools-1.0.5.7/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-03-20 13:09:02.735065 sfctools-1.0.5.7/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-20 13:09:06.611852 sfctools-1.0.5.7/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-07-11 05:48:26.175050 sfctools-1.0.5.7/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-12-30 14:49:34.085439 sfctools-1.0.5.7/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-07-11 05:48:26.251065 sfctools-1.0.5.7/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-07-11 05:48:26.289074 sfctools-1.0.5.7/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-07-11 05:48:26.401099 sfctools-1.0.5.7/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-10-05 17:45:14.259714 sfctools-1.0.5.7/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-20 13:09:06.612897 sfctools-1.0.5.7/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-20 13:09:06.614389 sfctools-1.0.5.7/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-20 13:09:06.615392 sfctools-1.0.5.7/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-20 13:09:06.615392 sfctools-1.0.5.7/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-20 13:09:06.616409 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-20 13:09:06.617415 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-20 13:09:06.617415 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-20 13:09:06.618422 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-20 13:09:06.619427 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-20 13:09:06.619427 sfctools-1.0.5.7/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-20 13:09:06.621437 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-20 13:09:06.622441 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-20 13:09:06.623445 sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-20 13:09:06.623445 sfctools-1.0.5.7/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-20 13:09:06.624450 sfctools-1.0.5.7/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-20 13:09:06.624450 sfctools-1.0.5.7/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-20 13:09:06.625458 sfctools-1.0.5.7/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-20 13:09:06.625458 sfctools-1.0.5.7/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-20 13:09:06.626464 sfctools-1.0.5.7/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-20 13:09:06.626464 sfctools-1.0.5.7/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-20 13:09:06.627470 sfctools-1.0.5.7/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-20 13:09:06.628492 sfctools-1.0.5.7/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-02 14:41:04.722520 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      415 2023-05-02 14:41:04.789151 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      417 2023-05-02 14:41:04.848249 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      413 2023-05-02 14:41:04.910757 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      413 2023-05-02 14:41:04.969838 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      410 2023-05-02 14:41:05.033208 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      415 2023-05-02 14:41:05.092742 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      413 2023-05-02 14:41:05.152384 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      416 2023-05-02 14:41:05.213119 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      413 2023-05-02 14:41:05.272879 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      412 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-02 14:41:05.333495 sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-20 13:09:06.634587 sfctools-1.0.5.7/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-20 13:09:06.635591 sfctools-1.0.5.7/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-20 13:09:06.635591 sfctools-1.0.5.7/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-20 13:09:06.636593 sfctools-1.0.5.7/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/__init__.py
--rw-r--r--   0        0        0       41 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0        0 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0    34561 2023-03-20 13:09:06.637593 sfctools-1.0.5.7/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-04-27 13:29:45.411196 sfctools-1.0.5.7/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    72949 2023-05-02 14:50:59.910575 sfctools-1.0.5.7/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-03-20 13:09:02.740428 sfctools-1.0.5.7/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-02 06:24:19.629663 sfctools-1.0.5.7/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-03-20 13:09:02.741615 sfctools-1.0.5.7/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-20 13:09:06.640594 sfctools-1.0.5.7/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-20 13:09:06.641594 sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-27 08:43:06.249807 sfctools-1.0.5.7/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-02 14:36:23.559376 sfctools-1.0.5.7/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-08-09 15:11:37.968071 sfctools-1.0.5.7/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-04-27 13:07:33.967008 sfctools-1.0.5.7/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-20 13:09:06.643594 sfctools-1.0.5.7/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-20 13:09:06.644595 sfctools-1.0.5.7/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-03-20 13:09:02.744421 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-20 13:09:06.645595 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-03-20 13:09:02.745871 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-03-20 13:09:02.746872 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-20 13:09:06.646595 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-03-20 13:09:02.748074 sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-04-27 16:25:31.372347 sfctools-1.0.5.7/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-02 14:49:34.488744 sfctools-1.0.5.7/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-02 06:27:52.607491 sfctools-1.0.5.7/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-20 13:09:06.647595 sfctools-1.0.5.7/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-20 13:09:06.648596 sfctools-1.0.5.7/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-08-09 15:11:37.952444 sfctools-1.0.5.7/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-03-20 13:09:02.736482 sfctools-1.0.5.7/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2023-03-20 12:39:06.880624 sfctools-1.0.5.7/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-04-27 11:35:47.715548 sfctools-1.0.5.7/sfctools/gui/sfctheme
--rw-r--r--   0        0        0        0 2022-07-11 05:48:26.867204 sfctools-1.0.5.7/sfctools/misc/__init__.py
--rw-r--r--   0        0        0    18645 2023-03-20 13:09:06.649596 sfctools-1.0.5.7/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-20 13:09:06.650596 sfctools-1.0.5.7/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-07-11 05:48:26.971227 sfctools-1.0.5.7/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.5.7/setup.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 sfctools-1.0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.5.8/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 11:03:59.435555 sfctools-1.0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.5.8/README.md
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.5.8/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.5.8/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.5.8/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.5.8/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.5.8/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.5.8/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.5.8/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.5.8/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.5.8/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.5.8/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.5.8/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.5.8/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.5.8/sfctools/core/__init__.py
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.5.8/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.5.8/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.5.8/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.5.8/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.5.8/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.5.8/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.5.8/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.5.8/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.5.8/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.5.8/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.5.8/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.5.8/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.5.8/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.5.8/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.5.8/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.5.8/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.5.8/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.5.8/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.5.8/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.5.8/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.5.8/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.5.8/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.5.8/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.5.8/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.5.8/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.5.8/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.5.8/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.5.8/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.5.8/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.5.8/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.5.8/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.5.8/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.5.8/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.5.8/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.5.8/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.5.8/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    72504 2023-05-04 10:46:26.158680 sfctools-1.0.5.8/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.5.8/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.5.8/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.5.8/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.5.8/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.5.8/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.5.8/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.5.8/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.5.8/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.5.8/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.5.8/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 11:01:36.149057 sfctools-1.0.5.8/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.5.8/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.5.8/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.5.8/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.5.8/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.5.8/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.5.8/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.5.8/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.5.8/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.5.8/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.5.8/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0    18645 2023-03-21 16:33:08.131566 sfctools-1.0.5.8/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.5.8/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.5.8/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 sfctools-1.0.5.8/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.5.8/PKG-INFO
```

### Comparing `sfctools-1.0.5.7/LICENSE` & `sfctools-1.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/pyproject.toml` & `sfctools-1.0.5.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.5.7"
+version = "1.0.5.8"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.5.7/README.md` & `sfctools-1.0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/__init__.py` & `sfctools-1.0.5.8/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/__main__.py` & `sfctools-1.0.5.8/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/automation/calibration.py` & `sfctools-1.0.5.8/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/automation/cgesolver.py` & `sfctools-1.0.5.8/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/automation/runner.py` & `sfctools-1.0.5.8/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/bottomup/matching.py` & `sfctools-1.0.5.8/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/bottomup/productiontree.py` & `sfctools-1.0.5.8/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.5.8/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/bottomup/treestruct.py` & `sfctools-1.0.5.8/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/agent.py` & `sfctools-1.0.5.8/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/clock.py` & `sfctools-1.0.5.8/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/flow_matrix.py` & `sfctools-1.0.5.8/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/settings.py` & `sfctools-1.0.5.8/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/singleton.py` & `sfctools-1.0.5.8/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/core/world.py` & `sfctools-1.0.5.8/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/balance.py` & `sfctools-1.0.5.8/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.5.8/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.5.8/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/collection.py` & `sfctools-1.0.5.8/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/income_statement.py` & `sfctools-1.0.5.8/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/inventory.py` & `sfctools-1.0.5.8/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/market_registry.py` & `sfctools-1.0.5.8/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/signalslot.py` & `sfctools-1.0.5.8/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.5.8/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/__init__.py` & `sfctools-1.0.5.8/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/balance.py` & `sfctools-1.0.5.8/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.5.8/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/clock.py` & `sfctools-1.0.5.8/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/example_wrapper.py` & `sfctools-1.0.5.8/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.5.8/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/flowmatrix.py` & `sfctools-1.0.5.8/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/hello_agent.py` & `sfctools-1.0.5.8/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/inventory.py` & `sfctools-1.0.5.8/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/market_example/market.py` & `sfctools-1.0.5.8/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/market_example/market2.py` & `sfctools-1.0.5.8/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.5.8/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.5.8/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/order_book.py` & `sfctools-1.0.5.8/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/examples/signal_slot.py` & `sfctools-1.0.5.8/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.5.8/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/draw_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             y2 = zf*(dw.goy +y2)
 
             # rect with rounded corners
             round_w = 4
 
             # draw boxes
 
-            path.addRoundedRect(QtCore.QRectF(x1,y1,w,w), zf*round_w, zf*round_w)
+            path.addRoundedRect(QtCore.QRectF(x1,y1,zf*w,zf*w), zf*round_w, zf*round_w)
             qp.fillPath(path,brush.color())
 
 
     def edit_agent(self):
         if not self.ishelper:
             print("EDIT AGENT CODE", self.name)
             print("INSTANCES",CodeEditor.instances,"\n\n")
@@ -402,15 +402,15 @@
         self.mousey = 0
 
         self.interpol_method = "quadratic"
         self.mode = "select"
 
         self.zoom_factor = 1.0
 
-        self.raster_size = 5.0
+        self.raster_size = 0.9
         self.show_raster = False
 
         self.show()
 
 
     def update_raster(self):
         # updates the raster settings
@@ -767,15 +767,15 @@
                 self.old_positions[box.name] = (box.x, box.y)
                 self.old_positions[box.parent.a.name] = (box.parent.a.x,box.parent.a.y)
                 self.old_positions[box.parent.b.name] = (box.parent.b.x,box.parent.b.y)
 
                 self.update()
                 return
 
-    def manhattan_lines(self,x0, y0, xf, yf,n=100):
+    def manhattan_lines(self,x0, y0, xf, yf, n=50):
 
         wx = abs(xf - x0) # abs(ip[-1][0] - ip[0][0])
         wy = abs(yf - y0) #  abs(ip[-1][1] - ip[0][1])
 
         interpolated_points = []
 
         len1 = int(0.75*n)
@@ -796,22 +796,138 @@
         #    x_coords = [x_coords[n-i-1] for i in range(n)]
 
         #if yf - y0 < 0:
         #    y_coords = [y_coords[n-i-1] for i in range(n)]
 
         return x_coords, y_coords
 
+    def crop_angle(self,x):
+        x = x % np.pi 
+
+        if 0 <= x < np.pi/2:
+            x = 0.0 
+
+        elif np.pi/2 <= x < np.pi: 
+            x = np.pi/2
+
+        elif -np.pi/2 <= x < 0 :
+            x = -np.pi/2.0
+
+        elif -np.pi <= x < -np.pi/2:
+            x = -np.pi 
+        
+        return x         
+
+    def draw_arrow_at(self, qp, interpolated_points, md,offset_text=15, reverse = False, dashed=False):
+
+        mid_point = interpolated_points[md]
+        mid_point2 = interpolated_points[md+5]
+        mid_points3 = interpolated_points[md-offset_text+1]
+        mid_points4 = interpolated_points[md-offset_text+1+10]
+
+        dy = mid_point[1] - mid_point2[1]
+        dx = mid_point[0] - mid_point2[0]
+
+        if reverse:
+            dx = -dx 
+            dy = -dy 
+
+        alfa = np.arctan2(dy,dx)
+
+        
+        if abs(dy) == 0.0 and abs(dx) >= 0:
+            alfa = 0.0
+
+        elif abs(dy) == 0.0 and abs(dx) < 0:
+            alfa = np.pi
+
+        elif abs(dx) == 0.0 and abs(dy) >= 0:
+            alfa = -np.pi/2.
+
+        elif abs(dx) == 0.0 and abs(dy) < 0:
+            alfa = np.pi/2.
+
+        if self.show_raster:
+            alfa = self.crop_angle(alfa)
+
+        beta1 = alfa + np.pi/4
+        beta2 = alfa - np.pi/4
+
+        if abs(dy) > abs(dy):
+            beta3 = alfa - np.pi/3
+        else:
+            beta3 = alfa - np.pi/3 + np.pi/2
+        
+        x2 = mid_point2[0]
+        y2 = mid_point2[1]
+
+        d = 10 # arrow width
+        x3 = np.cos(beta1)*d + x2
+        y3 = np.sin(beta1)*d + y2
+
+        x4 = np.cos(beta2)*d + x2
+        y4 = np.sin(beta2)*d + y2
+
+        xt = np.cos(beta3)*3 + mid_points3[0]
+        yt = np.sin(beta3)*3 + mid_points3[1]
+
+        if self.show_raster:
+             
+            darr = 10 # arrow width
+            if abs(dy) == 0.0 and (dx) <= 0:
+                x3 = x2 - d
+                y3 = y2 + darr
+
+                x4 = x2 - d
+                y4 = y2 - darr
+
+            elif abs(dy)  == 0.0  and (dx) > 0:
+                x3 = x2 + d
+                y3 = y2 + darr
+
+                x4 = x2 + d
+                y4 = y2 - darr
+
+
+            elif abs(dx)  == 0.0  and (dy) >= 0:
+                x3 = x2 - darr
+                y3 = y2 + d
+
+                x4 = x2 + darr
+                y4 = y2 + d
+
+
+            elif abs(dx)  == 0.0  and (dy) < 0:
+                x3 = x2  - darr
+                y3 = y2 - d
+
+                x4 = x2 + darr
+                y4 = y2 - d
+
+
+        # draw arrow
+        # if is_flow: # TODO think about behavior for non-flows
+        if not dashed:
+            if self.main_widget.checkBox.isChecked(): # not end_is_start and  ...
+                # left side
+                qp.drawLine(int(self.zoom_factor*(x2)),int(self.zoom_factor*(y2)), int(self.zoom_factor*(x3)), int(self.zoom_factor*(y3)))
+
+                # right side
+                qp.drawLine(int(self.zoom_factor*(x2)), int(self.zoom_factor*(y2)), int(self.zoom_factor*(x4)), int(self.zoom_factor*(y4)))
+
+        return xt, yt 
+
 
     def curved_connector(self,qp,x0,y0,xf,yf,xi,yi,xd,yd,dashed=False,is_flow=True,is_unidir=True):
         """
         draws a curved connector
         """
 
-        # if dashed:
-        #    return 0,0 # TODO maybe add another checkbox to configure behavior for non-active connectors
+        #if dashed:
+        #   return 0,0 # TODO maybe add another checkbox to configure behavior for non-active connectors
 
         # x0 += 12.5
         # y0 += 12.5
 
         # construct helper box_positions
         xi2 = 0.5*(xi-x0) + x0
         xi3 = 0.5*(xf-xi) + xi
@@ -981,17 +1097,17 @@
                 ip = interpolator(alpha)
 
                 x0 = points[0][0]
                 y0 = points[0][1]
                 xf = points[-1][0]
                 yf = points[-1][1]
 
-                xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,30)
-                xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,30)
-                xc3, yc3 = self.manhattan_lines(xd,yd,xf,yf,100)
+                xc1, yc1 = self.manhattan_lines(x0,y0,xi,yi,111)
+                xc2, yc2 = self.manhattan_lines(xi,yi,xd,yd,111)
+                xc3, yc3 = self.manhattan_lines(xd,yd,xf,yf,111) # 
 
                 x_coords = xc1 + xc2 + xc3
                 y_coords = yc1 + yc2 + yc3
                 interpolated_points = list(zip(x_coords,y_coords))
 
             # draw connector line as path
             n = len(interpolated_points)
@@ -1023,144 +1139,29 @@
             connPath.moveTo(startx,starty)
 
             connPath.closeSubpath()
             qp.drawPath(connPath)
 
             # draw arrow at midpoint
 
-            if not self.show_raster:
-                md = int(n/2.)
-            else:
-                md = 25
-                offset_text = 5
-
-            mid_point = interpolated_points[md]
-            mid_point2 = interpolated_points[md+1]
-            mid_points3 = interpolated_points[md-offset_text+1]
-            mid_points4 = interpolated_points[md-offset_text+1+7]
-
-            dy = mid_point[1] - mid_point2[1]
-            dx = mid_point[0] - mid_point2[0]
-
-            alfa = np.arctan2(dy,dx)
-
-            eps = 1e-8
-            if abs(dy) < eps and abs(dx) >= 0:
-                alfa = 0.0
-
-            elif abs(dy) < eps and abs(dx) < 0:
-                alfa = np.pi
-
-            elif abs(dx) < eps and abs(dy) >= 0:
-                alfa = -np.pi/2.
-
-            elif abs(dx) < eps and abs(dy) > 0:
-                alfa = np.pi/2.
-
-            beta1 = alfa + np.pi/4
-            beta2 = alfa - np.pi/4
-
-            if abs(dy) > abs(dy):
-                beta3 = alfa - np.pi/3
-            else:
-                beta3 = alfa - np.pi/3 + np.pi/2
-
-            x2 = mid_point2[0]
-            y2 = mid_point2[1]
-
-            d = 10
-            x3 = np.cos(beta1)*d + x2
-            y3 = np.sin(beta1)*d + y2
-
-            x4 = np.cos(beta2)*d + x2
-            y4 = np.sin(beta2)*d + y2
-
-            xt = np.cos(beta3)*3 + mid_points3[0]
-            yt = np.sin(beta3)*3 + mid_points3[1]
-
-
-            if self.show_raster:
-
-                darr = 10
-                if abs(dy) < eps and (dx) <= 0:
-                    x3 = x2 - d
-                    y3 = y2 + darr
-
-                    x4 = x2 - d
-                    y4 = y2 - darr
-
-                elif abs(dy) < eps and (dx) > 0:
-                    x3 = x2 + d
-                    y3 = y2 + darr
-
-                    x4 = x2 + d
-                    y4 = y2 - darr
-
-
-                elif abs(dx) < eps and (dy) >= 0:
-                    x3 = x2 - darr
-                    y3 = y2 + d
-
-                    x4 = x2 + darr
-                    y4 = y2 + d
-
-
-                elif abs(dx) < eps and (dy) > 0:
-                    x3 = x2  - darr
-                    y3 = y2 - d
-
-                    x4 = x2 + darr
-                    y4 = y2 - d
-
-
-            # draw arrow
-            # if is_flow: # TODO think about behavior for non-flows
-            if not dashed:
-                if not end_is_start and self.main_widget.checkBox.isChecked():
-                    # left side
-                    qp.drawLine(int(self.zoom_factor*(x2)),int(self.zoom_factor*(y2)), int(self.zoom_factor*(x3)), int(self.zoom_factor*(y3)))
-
-                    # right side
-                    qp.drawLine(int(self.zoom_factor*(x2)), int(self.zoom_factor*(y2)), int(self.zoom_factor*(x4)), int(self.zoom_factor*(y4)))
+            md = int(n/2.)
+            
+            # interpolated_points = [(self.raster(p[0],50),self.raster(p[1],50)) for p in interpolated_points]
 
+            xt,yt = self.draw_arrow_at(qp,interpolated_points,md,dashed=dashed)
+            
 
             if not is_unidir: # double arrow for non-unidirectional
                 if not end_is_start and self.main_widget.checkBox.isChecked():
+                    
+                    md = int(n/2. - 40)
+                    
+                    xt,yt = self.draw_arrow_at(qp,interpolated_points,md, reverse=True,dashed=dashed)
 
-                    mid_point = interpolated_points[int(n/2)-4]
-                    mid_point4 = interpolated_points[int(n/2)-4-1]
-
-                    dy = mid_point[1] - mid_point4[1]
-                    dx = mid_point[0] - mid_point4[0]
-
-                    alfa = np.arctan2(dy,dx)
-                    beta1 = alfa + np.pi/4
-                    beta2 = alfa - np.pi/4
-
-                    if abs(dy) > abs(dy):
-                        beta3 = alfa - np.pi/3 + np.pi/2
-                    else:
-                        beta3 = alfa - np.pi/3
-
-                    x2 = mid_point4[0]
-                    y2 = mid_point4[1]
-
-                    d = 10
-                    x3 = np.cos(beta1)*d + x2
-                    y3 = np.sin(beta1)*d + y2
-
-                    x4 = np.cos(beta2)*d + x2
-                    y4 = np.sin(beta2)*d + y2
-
-                    # left side
-                    qp.drawLine(int(self.zoom_factor*(x2)), int(self.zoom_factor*(y2)), int(self.zoom_factor*(x4)), int(self.zoom_factor*(y4)))
-
-                    # right side
-                    qp.drawLine(int(self.zoom_factor*(x2)), int(self.zoom_factor*(y2)), int(self.zoom_factor*(x3)), int(self.zoom_factor*(y3)))
-
+                    
         except Exception as e:
             print("Error in Line Interpolation:",str(e))
             xt = 0
             yt = 0
 
         """
         if self.darkMode:
@@ -1305,18 +1306,18 @@
         # dy = 5
         # ox_transformed = move_x + self.W-w_frame+ox-2
         # oy_transformed = move_y + self.H-h_frame+oy-2
 
         # qp.drawLine(ox_transformed-dx,oy_transformed,ox_transformed+dx,oy_transformed)
         # qp.drawLine(ox_transformed,oy_transformed-dy,ox_transformed,oy_transformed+dy)
 
-    def raster(self,x,n=5):
+    def raster(self, x, n=5):
         if self.show_raster: # show rasterized
             # x_rastered = np.round(x,int(-np.log10(self.raster_size)))
-            m = max(n,self.raster_size)
+            m = min(n,self.raster_size)
             x_rastered = (int(x/m))*m  # np.round(x,int(-np.log10(self.raster_size)))
             return int(x_rastered)
         return int(x)
 
     def paint(self,reference,ratio=1):
 
         qp = QtGui.QPainter(reference)
@@ -2016,16 +2017,16 @@
             x = x
             y = y
 
             dx = x  - self.go_startx
             dy = y - self.go_starty
             # print("move", dx,dy)
 
-            self.gox = self.gox_start + dx
-            self.goy = self.goy_start + dy
+            self.gox = self.raster(self.gox_start + dx)
+            self.goy = self.raster(self.goy_start + dy)
 
         # print("move",x,y)
         else:
 
             hovering = False
             for box in self.boxes:
                 if box.ishelper:
```

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.5.8/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.5.8/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.5.8/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/CLA.pdf` & `sfctools-1.0.5.8/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.5.8/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/LICENSE` & `sfctools-1.0.5.8/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/gui/README.md` & `sfctools-1.0.5.8/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.5.8/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.5.8/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/sfctools/misc/timeseries.py` & `sfctools-1.0.5.8/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.7/setup.py` & `sfctools-1.0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.5.7',
+    'version': '1.0.5.8',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.5.7/PKG-INFO` & `sfctools-1.0.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.5.7
+Version: 1.0.5.8
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyQt5 (>=5.9)
 Requires-Dist: attrs
 Requires-Dist: graphviz
 Requires-Dist: matplotlib (>=2.0.0)
 Requires-Dist: networkx (>=2.2)
 Requires-Dist: numpy
 Requires-Dist: openpyxl
```

