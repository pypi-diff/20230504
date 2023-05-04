# Comparing `tmp/sfctools-1.0.5.9.tar.gz` & `tmp/sfctools-1.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfctools-1.0.5.9.tar", max compression
+gzip compressed data, was "sfctools-1.0.6.0.tar", max compression
```

## Comparing `sfctools-1.0.5.9.tar` & `sfctools-1.0.6.0.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.5.9/LICENSE
--rw-r--r--   0        0        0     1620 2023-05-04 12:04:03.789783 sfctools-1.0.5.9/pyproject.toml
--rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.5.9/README.md
--rw-r--r--   0        0        0       39 2023-01-26 10:19:31.537790 sfctools-1.0.5.9/sfctools/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-01-26 10:19:31.537845 sfctools-1.0.5.9/sfctools/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-01-26 10:19:31.536780 sfctools-1.0.5.9/sfctools/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-01-26 10:19:31.537845 sfctools-1.0.5.9/sfctools/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-01-26 10:19:31.539052 sfctools-1.0.5.9/sfctools/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.5.9/sfctools/__init__.py
--rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.5.9/sfctools/__main__.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.5.9/sfctools/automation/__init__.py
--rw-r--r--   0        0        0      177 2023-01-25 08:23:20.053567 sfctools-1.0.5.9/sfctools/automation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      159 2023-01-19 21:54:26.523852 sfctools-1.0.5.9/sfctools/automation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8273 2023-01-25 08:23:20.054862 sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-311.pyc
--rw-r--r--   0        0        0     4139 2023-01-19 21:54:26.530954 sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-38.pyc
--rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.5.9/sfctools/automation/calibration.py
--rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.5.9/sfctools/automation/cgesolver.py
--rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.5.9/sfctools/automation/README.md
--rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.5.9/sfctools/automation/runner.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.5.9/sfctools/bottomup/__init__.py
--rw-r--r--   0        0        0      175 2023-01-25 08:23:19.248631 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      157 2023-01-19 21:54:25.705346 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13061 2023-01-25 08:23:19.475949 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-311.pyc
--rw-r--r--   0        0        0     8647 2023-02-06 10:24:45.316244 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-38.pyc
--rw-r--r--   0        0        0    11948 2023-01-25 08:16:32.088889 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc
--rw-r--r--   0        0        0     8339 2023-01-25 08:23:19.250795 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc
--rw-r--r--   0        0        0     5937 2023-01-19 21:54:25.707915 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc
--rw-r--r--   0        0        0     2863 2023-01-25 08:16:32.090879 sfctools-1.0.5.9/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc
--rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.5.9/sfctools/bottomup/matching.py
--rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.5.9/sfctools/bottomup/productiontree.py
--rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.5.9/sfctools/bottomup/stock_manager.py
--rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.5.9/sfctools/bottomup/treestruct.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.5.9/sfctools/core/__init__.py
--rw-r--r--   0        0        0      171 2023-01-25 08:23:16.612109 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      153 2023-01-19 21:54:24.854116 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      153 2022-12-22 08:43:56.478191 sfctools-1.0.5.9/sfctools/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10127 2023-01-25 08:23:16.614415 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-311.pyc
--rw-r--r--   0        0        0     7106 2023-01-19 21:54:24.857704 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-38.pyc
--rw-r--r--   0        0        0     7096 2022-12-22 08:43:56.499523 sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     3200 2023-01-25 08:23:17.901786 sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-311.pyc
--rw-r--r--   0        0        0     2503 2023-01-19 21:54:25.148426 sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-38.pyc
--rw-r--r--   0        0        0      856 2023-01-25 08:23:17.915777 sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc
--rw-r--r--   0        0        0      677 2023-04-04 07:45:29.386549 sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc
--rw-r--r--   0        0        0    19394 2023-01-25 08:23:19.254129 sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc
--rw-r--r--   0        0        0    12090 2023-04-04 07:45:29.716546 sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc
--rw-r--r--   0        0        0    13234 2023-01-25 08:23:19.211702 sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     8933 2023-04-04 07:45:29.692870 sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0        0        0     1482 2023-01-25 08:23:17.905919 sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-311.pyc
--rw-r--r--   0        0        0     1091 2023-01-19 21:54:25.153899 sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-38.pyc
--rw-r--r--   0        0        0     8862 2023-01-25 08:23:16.616906 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-311.pyc
--rw-r--r--   0        0        0     5654 2023-02-06 10:24:44.695973 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-38.pyc
--rw-r--r--   0        0        0     5547 2022-12-22 08:43:56.518896 sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-39.pyc
--rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.5.9/sfctools/core/agent.py
--rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.5.9/sfctools/core/clock.py
--rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.5.9/sfctools/core/custom_warnings.py
--rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.5.9/sfctools/core/flow_matrix.py
--rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.5.9/sfctools/core/settings.py
--rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.5.9/sfctools/core/singleton.py
--rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.5.9/sfctools/core/world.py
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.5.9/sfctools/datastructs/__init__.py
--rw-r--r--   0        0        0      178 2023-01-25 08:23:16.618054 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      160 2023-01-19 21:54:24.869946 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      160 2022-12-22 08:43:56.522922 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    36033 2023-01-25 08:23:19.209700 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-311.pyc
--rw-r--r--   0        0        0    22057 2023-04-04 07:45:29.687338 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-38.pyc
--rw-r--r--   0        0        0    19951 2023-01-25 08:23:19.473688 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc
--rw-r--r--   0        0        0    13962 2023-02-06 10:24:45.311852 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc
--rw-r--r--   0        0        0     8905 2023-01-25 08:23:19.468631 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc
--rw-r--r--   0        0        0     6617 2023-04-04 07:45:29.894931 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc
--rw-r--r--   0        0        0     6937 2023-01-25 08:23:16.619099 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-311.pyc
--rw-r--r--   0        0        0     4736 2023-01-19 21:54:24.876121 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-38.pyc
--rw-r--r--   0        0        0     4718 2022-12-22 08:43:56.543068 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-39.pyc
--rw-r--r--   0        0        0    18687 2023-01-25 08:23:19.466630 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc
--rw-r--r--   0        0        0    13398 2023-01-19 21:54:25.920678 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc
--rw-r--r--   0        0        0     8382 2023-01-25 08:23:20.048441 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc
--rw-r--r--   0        0        0     5672 2023-01-19 21:54:26.507228 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc
--rw-r--r--   0        0        0     6583 2023-01-25 08:23:20.050844 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc
--rw-r--r--   0        0        0     5167 2023-01-19 21:54:26.513706 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc
--rw-r--r--   0        0        0     8490 2023-01-25 08:23:19.471344 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc
--rw-r--r--   0        0        0     6018 2023-01-19 21:54:25.936504 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc
--rw-r--r--   0        0        0     5219 2023-01-25 08:23:20.052395 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc
--rw-r--r--   0        0        0     3653 2023-01-19 21:54:26.519688 sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc
--rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.5.9/sfctools/datastructs/balance.py
--rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.5.9/sfctools/datastructs/bank_order_book.py
--rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.5.9/sfctools/datastructs/cash_flow_statement.py
--rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.5.9/sfctools/datastructs/collection.py
--rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.5.9/sfctools/datastructs/income_statement.py
--rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.5.9/sfctools/datastructs/inventory.py
--rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.5.9/sfctools/datastructs/market_registry.py
--rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.5.9/sfctools/datastructs/signalslot.py
--rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.5.9/sfctools/datastructs/worker_registry.py
--rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.5.9/sfctools/examples/__init__.py
--rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.5.9/sfctools/examples/balance.py
--rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/basic_example/basic_example.py
--rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/basic_example/my_settings.yml
--rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.5.9/sfctools/examples/clock.py
--rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/example_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/__init__.py
--rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/government.py
--rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/household.py
--rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/production.py
--rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/transactions.py
--rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/preprocess.py
--rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
--rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.5.9/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
--rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/matrix.png
--rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/outputs.png
--rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/sankey.png
--rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.5.9/sfctools/examples/exampleabm/info.md
--rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/exampleabm/model.py
--rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/exampleabm/settings.yml
--rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.5.9/sfctools/examples/flowmatrix.py
--rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.5.9/sfctools/examples/hello_agent.py
--rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.5.9/sfctools/examples/inventory.py
--rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/market_example/market.py
--rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/market_example/market2.py
--rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.5.9/sfctools/examples/monte_carlo/monte_carlo.py
--rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/errors.txt
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.0
--rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.1
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.2
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.3
--rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.4
--rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.5
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.6
--rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.7
--rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.8
--rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.9
--rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.txt
--rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/progress.txt
--rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/monte_carlo/testsettings.yml
--rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/order_book.py
--rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.5.9/sfctools/examples/paper_example.py
--rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.5.9/sfctools/examples/signal_slot.py
--rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.5.9/sfctools/gui/.gitignore
--rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.5.9/sfctools/gui/.gitlab-ci.yml
--rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.5.9/sfctools/gui/__init__.py
--rw-r--r--   0        0        0      269 2023-01-25 08:23:20.061472 sfctools-1.0.5.9/sfctools/gui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      221 2023-01-25 08:17:49.221422 sfctools-1.0.5.9/sfctools/gui/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2791 2023-01-25 08:23:20.063473 sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-311.pyc
--rw-r--r--   0        0        0      835 2023-04-04 07:45:30.299298 sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-38.pyc
--rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.5.9/sfctools/gui/attune/.gitignore
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.5.9/sfctools/gui/attune/__init__.py
--rw-r--r--   0        0        0      177 2022-12-22 08:51:44.532604 sfctools-1.0.5.9/sfctools/gui/attune/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      159 2022-11-23 08:49:18.431057 sfctools-1.0.5.9/sfctools/gui/attune/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.5.9/sfctools/gui/attune/src/__init__.py
--rw-r--r--   0        0        0      181 2022-12-22 08:51:44.534815 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      163 2022-11-23 08:49:18.433350 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    50257 2023-01-25 08:23:24.448393 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc
--rw-r--r--   0        0        0    20359 2023-04-04 07:45:31.111570 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc
--rw-r--r--   0        0        0    70418 2023-01-25 08:50:00.544297 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc
--rw-r--r--   0        0        0    35485 2023-05-04 12:02:59.036460 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc
--rw-r--r--   0        0        0    16034 2023-01-25 08:23:21.221015 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc
--rw-r--r--   0        0        0    10518 2023-05-04 09:43:05.888334 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc
--rw-r--r--   0        0        0    10890 2023-01-25 08:23:21.216723 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc
--rw-r--r--   0        0        0     4813 2023-02-06 10:17:36.928510 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc
--rw-r--r--   0        0        0    32862 2023-01-25 08:23:21.227665 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc
--rw-r--r--   0        0        0    12521 2023-04-04 07:45:30.873144 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc
--rw-r--r--   0        0        0     2435 2023-01-25 08:23:21.211969 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2023-04-04 07:45:30.862180 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc
--rw-r--r--   0        0        0   152005 2023-01-25 08:47:50.827103 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc
--rw-r--r--   0        0        0    69406 2023-05-04 09:43:04.168970 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc
--rw-r--r--   0        0        0     7007 2023-01-25 08:23:24.383425 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc
--rw-r--r--   0        0        0     6499 2022-11-23 08:49:30.377800 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc
--rw-r--r--   0        0        0    10255 2023-01-25 08:23:24.459690 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc
--rw-r--r--   0        0        0     5060 2023-05-04 09:43:06.152185 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc
--rw-r--r--   0        0        0    14167 2023-01-25 08:23:24.456539 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc
--rw-r--r--   0        0        0     9595 2023-05-04 09:43:06.142977 sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc
--rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.5.9/sfctools/gui/attune/src/agent_editor.py
--rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.5.9/sfctools/gui/attune/src/code_editor.ui
--rw-r--r--   0        0        0    74357 2023-05-04 12:03:31.938961 sfctools-1.0.5.9/sfctools/gui/attune/src/draw_widget.py
--rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.5.9/sfctools/gui/attune/src/income_viewer.ui
--rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.5.9/sfctools/gui/attune/src/mainloop_editor.py
--rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.5.9/sfctools/gui/attune/src/mamba_interpreter2.py
--rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.5.9/sfctools/gui/attune/src/matrix_viewer.ui
--rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.py
--rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.ui
--rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.5.9/sfctools/gui/attune/src/pandasmodel.py
--rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/qtattune.py
--rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.5.9/sfctools/gui/attune/src/resources.py
--rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.5.9/sfctools/gui/attune/src/resources.qrc
--rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/search_dialog.ui
--rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.5.9/sfctools/gui/attune/src/settings_edit.ui
--rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.5.9/sfctools/gui/attune/src/simulation_edit.ui
--rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/background.txt
--rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/main.txt
--rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/tables.txt
--rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/background.txt
--rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/main.txt
--rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/tables.txt
--rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.5.9/sfctools/gui/attune/src/theme_manager.py
--rw-r--r--   0        0        0    85086 2023-05-04 12:02:59.053599 sfctools-1.0.5.9/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
--rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.5.9/sfctools/gui/attune/src/yaml_editor.py
--rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.5.9/sfctools/gui/attune_main.py
--rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.5.9/sfctools/gui/attune_starter.py
--rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.5.9/sfctools/gui/CLA.pdf
--rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.5.9/sfctools/gui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.5.9/sfctools/gui/LICENSE
--rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.5.9/sfctools/gui/README.md
--rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.5.9/sfctools/gui/runner.py
--rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.5.9/sfctools/gui/sfctheme
--rw-r--r--   0        0        0     4765 2022-11-23 09:50:36.467143 sfctools-1.0.5.9/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc
--rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.5.9/sfctools/misc/__init__.py
--rw-r--r--   0        0        0      171 2023-01-25 08:23:20.056190 sfctools-1.0.5.9/sfctools/misc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      153 2023-01-19 21:54:26.534886 sfctools-1.0.5.9/sfctools/misc/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13145 2023-02-06 10:24:45.828385 sfctools-1.0.5.9/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc
--rw-r--r--   0        0        0    10106 2023-01-25 08:23:20.059255 sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc
--rw-r--r--   0        0        0     7616 2023-04-04 07:45:30.288586 sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc
--rw-r--r--   0        0        0    12006 2023-01-25 08:23:21.230666 sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-311.pyc
--rw-r--r--   0        0        0     6420 2023-01-25 08:17:49.793565 sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-38.pyc
--rw-r--r--   0        0        0    18645 2023-03-21 16:33:08.131566 sfctools-1.0.5.9/sfctools/misc/mpl_plotting.py
--rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.5.9/sfctools/misc/reporting_sheet.py
--rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.5.9/sfctools/misc/timeseries.py
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 sfctools-1.0.5.9/setup.py
--rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.643840 sfctools-1.0.6.0/LICENSE
+-rw-r--r--   0        0        0     1620 2023-05-04 12:06:43.150435 sfctools-1.0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1308 2023-03-21 16:33:08.082866 sfctools-1.0.6.0/README.md
+-rw-r--r--   0        0        0       39 2023-01-26 10:19:31.537790 sfctools-1.0.6.0/sfctools/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-01-26 10:19:31.537845 sfctools-1.0.6.0/sfctools/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-01-26 10:19:31.536780 sfctools-1.0.6.0/sfctools/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-01-26 10:19:31.537845 sfctools-1.0.6.0/sfctools/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-01-26 10:19:31.539052 sfctools-1.0.6.0/sfctools/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1938 2022-11-23 08:34:47.783372 sfctools-1.0.6.0/sfctools/__init__.py
+-rw-r--r--   0        0        0     2655 2023-01-26 10:34:36.652567 sfctools-1.0.6.0/sfctools/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.785439 sfctools-1.0.6.0/sfctools/automation/__init__.py
+-rw-r--r--   0        0        0      177 2023-01-25 08:23:20.053567 sfctools-1.0.6.0/sfctools/automation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2023-01-19 21:54:26.523852 sfctools-1.0.6.0/sfctools/automation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8273 2023-01-25 08:23:20.054862 sfctools-1.0.6.0/sfctools/automation/__pycache__/runner.cpython-311.pyc
+-rw-r--r--   0        0        0     4139 2023-01-19 21:54:26.530954 sfctools-1.0.6.0/sfctools/automation/__pycache__/runner.cpython-38.pyc
+-rw-r--r--   0        0        0    10574 2023-03-21 16:33:08.099326 sfctools-1.0.6.0/sfctools/automation/calibration.py
+-rw-r--r--   0        0        0    14589 2023-03-21 16:33:08.100325 sfctools-1.0.6.0/sfctools/automation/cgesolver.py
+-rw-r--r--   0        0        0       75 2022-11-23 08:34:47.785439 sfctools-1.0.6.0/sfctools/automation/README.md
+-rw-r--r--   0        0        0     5077 2022-11-23 08:34:47.790242 sfctools-1.0.6.0/sfctools/automation/runner.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.791250 sfctools-1.0.6.0/sfctools/bottomup/__init__.py
+-rw-r--r--   0        0        0      175 2023-01-25 08:23:19.248631 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      157 2023-01-19 21:54:25.705346 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13061 2023-01-25 08:23:19.475949 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/matching.cpython-311.pyc
+-rw-r--r--   0        0        0     8647 2023-02-06 10:24:45.316244 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/matching.cpython-38.pyc
+-rw-r--r--   0        0        0    11948 2023-01-25 08:16:32.088889 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc
+-rw-r--r--   0        0        0     8339 2023-01-25 08:23:19.250795 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     5937 2023-01-19 21:54:25.707915 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc
+-rw-r--r--   0        0        0     2863 2023-01-25 08:16:32.090879 sfctools-1.0.6.0/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc
+-rw-r--r--   0        0        0     8900 2023-01-26 10:34:36.653567 sfctools-1.0.6.0/sfctools/bottomup/matching.py
+-rw-r--r--   0        0        0    17465 2023-03-21 16:33:08.101324 sfctools-1.0.6.0/sfctools/bottomup/productiontree.py
+-rw-r--r--   0        0        0     6904 2022-11-23 08:34:47.794005 sfctools-1.0.6.0/sfctools/bottomup/stock_manager.py
+-rw-r--r--   0        0        0     2737 2022-11-23 08:34:47.795896 sfctools-1.0.6.0/sfctools/bottomup/treestruct.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.796902 sfctools-1.0.6.0/sfctools/core/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-25 08:23:16.612109 sfctools-1.0.6.0/sfctools/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      153 2023-01-19 21:54:24.854116 sfctools-1.0.6.0/sfctools/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      153 2022-12-22 08:43:56.478191 sfctools-1.0.6.0/sfctools/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10127 2023-01-25 08:23:16.614415 sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-311.pyc
+-rw-r--r--   0        0        0     7106 2023-01-19 21:54:24.857704 sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-38.pyc
+-rw-r--r--   0        0        0     7096 2022-12-22 08:43:56.499523 sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     3200 2023-01-25 08:23:17.901786 sfctools-1.0.6.0/sfctools/core/__pycache__/clock.cpython-311.pyc
+-rw-r--r--   0        0        0     2503 2023-01-19 21:54:25.148426 sfctools-1.0.6.0/sfctools/core/__pycache__/clock.cpython-38.pyc
+-rw-r--r--   0        0        0      856 2023-01-25 08:23:17.915777 sfctools-1.0.6.0/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc
+-rw-r--r--   0        0        0      677 2023-04-04 07:45:29.386549 sfctools-1.0.6.0/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc
+-rw-r--r--   0        0        0    19394 2023-01-25 08:23:19.254129 sfctools-1.0.6.0/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc
+-rw-r--r--   0        0        0    12090 2023-04-04 07:45:29.716546 sfctools-1.0.6.0/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc
+-rw-r--r--   0        0        0    13234 2023-01-25 08:23:19.211702 sfctools-1.0.6.0/sfctools/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     8933 2023-04-04 07:45:29.692870 sfctools-1.0.6.0/sfctools/core/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0        0        0     1482 2023-01-25 08:23:17.905919 sfctools-1.0.6.0/sfctools/core/__pycache__/singleton.cpython-311.pyc
+-rw-r--r--   0        0        0     1091 2023-01-19 21:54:25.153899 sfctools-1.0.6.0/sfctools/core/__pycache__/singleton.cpython-38.pyc
+-rw-r--r--   0        0        0     8862 2023-01-25 08:23:16.616906 sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-311.pyc
+-rw-r--r--   0        0        0     5654 2023-02-06 10:24:44.695973 sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-38.pyc
+-rw-r--r--   0        0        0     5547 2022-12-22 08:43:56.518896 sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-39.pyc
+-rw-r--r--   0        0        0     7572 2022-11-23 08:34:47.797213 sfctools-1.0.6.0/sfctools/core/agent.py
+-rw-r--r--   0        0        0     2249 2022-11-23 08:34:47.798441 sfctools-1.0.6.0/sfctools/core/clock.py
+-rw-r--r--   0        0        0      495 2023-03-21 16:33:08.101324 sfctools-1.0.6.0/sfctools/core/custom_warnings.py
+-rw-r--r--   0        0        0    15032 2023-03-21 16:33:08.102324 sfctools-1.0.6.0/sfctools/core/flow_matrix.py
+-rw-r--r--   0        0        0    11632 2023-03-21 16:33:08.102324 sfctools-1.0.6.0/sfctools/core/settings.py
+-rw-r--r--   0        0        0      661 2022-11-23 08:34:47.802978 sfctools-1.0.6.0/sfctools/core/singleton.py
+-rw-r--r--   0        0        0     7304 2023-01-26 10:34:36.655075 sfctools-1.0.6.0/sfctools/core/world.py
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.805666 sfctools-1.0.6.0/sfctools/datastructs/__init__.py
+-rw-r--r--   0        0        0      178 2023-01-25 08:23:16.618054 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      160 2023-01-19 21:54:24.869946 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      160 2022-12-22 08:43:56.522922 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    36033 2023-01-25 08:23:19.209700 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/balance.cpython-311.pyc
+-rw-r--r--   0        0        0    22057 2023-04-04 07:45:29.687338 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/balance.cpython-38.pyc
+-rw-r--r--   0        0        0    19951 2023-01-25 08:23:19.473688 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc
+-rw-r--r--   0        0        0    13962 2023-02-06 10:24:45.311852 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc
+-rw-r--r--   0        0        0     8905 2023-01-25 08:23:19.468631 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc
+-rw-r--r--   0        0        0     6617 2023-04-04 07:45:29.894931 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc
+-rw-r--r--   0        0        0     6937 2023-01-25 08:23:16.619099 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-311.pyc
+-rw-r--r--   0        0        0     4736 2023-01-19 21:54:24.876121 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-38.pyc
+-rw-r--r--   0        0        0     4718 2022-12-22 08:43:56.543068 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-39.pyc
+-rw-r--r--   0        0        0    18687 2023-01-25 08:23:19.466630 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc
+-rw-r--r--   0        0        0    13398 2023-01-19 21:54:25.920678 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc
+-rw-r--r--   0        0        0     8382 2023-01-25 08:23:20.048441 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc
+-rw-r--r--   0        0        0     5672 2023-01-19 21:54:26.507228 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc
+-rw-r--r--   0        0        0     6583 2023-01-25 08:23:20.050844 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc
+-rw-r--r--   0        0        0     5167 2023-01-19 21:54:26.513706 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc
+-rw-r--r--   0        0        0     8490 2023-01-25 08:23:19.471344 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc
+-rw-r--r--   0        0        0     6018 2023-01-19 21:54:25.936504 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc
+-rw-r--r--   0        0        0     5219 2023-01-25 08:23:20.052395 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc
+-rw-r--r--   0        0        0     3653 2023-01-19 21:54:26.519688 sfctools-1.0.6.0/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc
+-rw-r--r--   0        0        0    32494 2023-03-21 16:33:08.103324 sfctools-1.0.6.0/sfctools/datastructs/balance.py
+-rw-r--r--   0        0        0    17441 2023-01-26 10:34:36.656502 sfctools-1.0.6.0/sfctools/datastructs/bank_order_book.py
+-rw-r--r--   0        0        0     6175 2023-03-21 16:33:08.104324 sfctools-1.0.6.0/sfctools/datastructs/cash_flow_statement.py
+-rw-r--r--   0        0        0     4900 2022-11-23 08:34:47.810921 sfctools-1.0.6.0/sfctools/datastructs/collection.py
+-rw-r--r--   0        0        0    14241 2022-11-23 08:34:47.811957 sfctools-1.0.6.0/sfctools/datastructs/income_statement.py
+-rw-r--r--   0        0        0     6043 2022-11-23 08:34:47.812908 sfctools-1.0.6.0/sfctools/datastructs/inventory.py
+-rw-r--r--   0        0        0     4272 2022-11-23 08:34:47.813916 sfctools-1.0.6.0/sfctools/datastructs/market_registry.py
+-rw-r--r--   0        0        0     5313 2022-11-23 08:34:47.815910 sfctools-1.0.6.0/sfctools/datastructs/signalslot.py
+-rw-r--r--   0        0        0     2961 2022-11-23 08:34:47.816910 sfctools-1.0.6.0/sfctools/datastructs/worker_registry.py
+-rw-r--r--   0        0        0      550 2023-03-21 16:33:08.105387 sfctools-1.0.6.0/sfctools/examples/__init__.py
+-rw-r--r--   0        0        0     2491 2023-03-21 16:33:08.105387 sfctools-1.0.6.0/sfctools/examples/balance.py
+-rw-r--r--   0        0        0     1701 2023-03-21 16:33:08.106499 sfctools-1.0.6.0/sfctools/examples/basic_example/basic_example.py
+-rw-r--r--   0        0        0      202 2023-03-21 16:33:08.106499 sfctools-1.0.6.0/sfctools/examples/basic_example/my_settings.yml
+-rw-r--r--   0        0        0     1087 2023-03-21 16:33:08.106499 sfctools-1.0.6.0/sfctools/examples/clock.py
+-rw-r--r--   0        0        0     1378 2023-03-21 16:33:08.107730 sfctools-1.0.6.0/sfctools/examples/example_wrapper.py
+-rw-r--r--   0        0        0        0 2023-03-21 16:33:08.107730 sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/__init__.py
+-rw-r--r--   0        0        0     1845 2023-03-21 16:33:08.107730 sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/government.py
+-rw-r--r--   0        0        0     2370 2023-03-21 16:33:08.108754 sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/household.py
+-rw-r--r--   0        0        0     2198 2023-03-21 16:33:08.108754 sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/production.py
+-rw-r--r--   0        0        0     4365 2023-03-21 16:33:08.108754 sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/transactions.py
+-rw-r--r--   0        0        0      910 2023-03-21 16:33:08.109754 sfctools-1.0.6.0/sfctools/examples/exampleabm/data/preprocess.py
+-rw-r--r--   0        0        0    13152 2023-03-21 16:33:08.109754 sfctools-1.0.6.0/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt
+-rw-r--r--   0        0        0      818 2023-03-21 16:33:08.110388 sfctools-1.0.6.0/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv
+-rw-r--r--   0        0        0    31241 2023-03-21 16:33:08.111510 sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/matrix.png
+-rw-r--r--   0        0        0    42423 2023-03-21 16:33:08.111510 sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/outputs.png
+-rw-r--r--   0        0        0    43865 2023-03-21 16:33:08.112510 sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/sankey.png
+-rw-r--r--   0        0        0     1264 2023-03-21 16:33:08.112510 sfctools-1.0.6.0/sfctools/examples/exampleabm/info.md
+-rw-r--r--   0        0        0     3730 2023-03-21 16:33:08.113510 sfctools-1.0.6.0/sfctools/examples/exampleabm/model.py
+-rw-r--r--   0        0        0     1148 2023-03-21 16:33:08.113510 sfctools-1.0.6.0/sfctools/examples/exampleabm/settings.yml
+-rw-r--r--   0        0        0     2805 2023-03-21 16:33:08.113510 sfctools-1.0.6.0/sfctools/examples/flowmatrix.py
+-rw-r--r--   0        0        0      813 2023-03-21 16:33:08.114513 sfctools-1.0.6.0/sfctools/examples/hello_agent.py
+-rw-r--r--   0        0        0     1168 2023-03-21 16:33:08.114513 sfctools-1.0.6.0/sfctools/examples/inventory.py
+-rw-r--r--   0        0        0     1783 2023-03-21 16:33:08.115240 sfctools-1.0.6.0/sfctools/examples/market_example/market.py
+-rw-r--r--   0        0        0     2735 2023-03-21 16:33:08.115240 sfctools-1.0.6.0/sfctools/examples/market_example/market2.py
+-rw-r--r--   0        0        0      999 2023-03-21 16:33:08.115240 sfctools-1.0.6.0/sfctools/examples/monte_carlo/monte_carlo.py
+-rw-r--r--   0        0        0       28 2023-05-04 09:42:20.692720 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/errors.txt
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.692720 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.0
+-rw-r--r--   0        0        0      417 2023-05-04 09:42:20.693746 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.1
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.2
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.693746 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.3
+-rw-r--r--   0        0        0      410 2023-05-04 09:42:20.694720 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.4
+-rw-r--r--   0        0        0      415 2023-05-04 09:42:20.694778 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.5
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.694778 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.6
+-rw-r--r--   0        0        0      416 2023-05-04 09:42:20.694778 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.7
+-rw-r--r--   0        0        0      413 2023-05-04 09:42:20.695959 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.8
+-rw-r--r--   0        0        0      412 2023-05-04 09:42:20.695959 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.9
+-rw-r--r--   0        0        0      527 2023-03-21 16:33:08.119298 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.txt
+-rw-r--r--   0        0        0      258 2023-05-04 09:42:20.695959 sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/progress.txt
+-rw-r--r--   0        0        0      184 2023-03-21 16:33:08.119972 sfctools-1.0.6.0/sfctools/examples/monte_carlo/testsettings.yml
+-rw-r--r--   0        0        0     3411 2023-03-21 16:33:08.119972 sfctools-1.0.6.0/sfctools/examples/order_book.py
+-rw-r--r--   0        0        0      124 2023-03-21 16:33:08.119972 sfctools-1.0.6.0/sfctools/examples/paper_example.py
+-rw-r--r--   0        0        0     1471 2023-03-21 16:33:08.121051 sfctools-1.0.6.0/sfctools/examples/signal_slot.py
+-rw-r--r--   0        0        0       27 2022-11-23 08:34:47.817910 sfctools-1.0.6.0/sfctools/gui/.gitignore
+-rw-r--r--   0        0        0      854 2022-11-23 08:34:47.818915 sfctools-1.0.6.0/sfctools/gui/.gitlab-ci.yml
+-rw-r--r--   0        0        0       64 2022-11-23 08:34:47.822910 sfctools-1.0.6.0/sfctools/gui/__init__.py
+-rw-r--r--   0        0        0      269 2023-01-25 08:23:20.061472 sfctools-1.0.6.0/sfctools/gui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      221 2023-01-25 08:17:49.221422 sfctools-1.0.6.0/sfctools/gui/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2791 2023-01-25 08:23:20.063473 sfctools-1.0.6.0/sfctools/gui/__pycache__/attune_main.cpython-311.pyc
+-rw-r--r--   0        0        0      835 2023-04-04 07:45:30.299298 sfctools-1.0.6.0/sfctools/gui/__pycache__/attune_main.cpython-38.pyc
+-rw-r--r--   0        0        0       41 2022-11-23 08:34:47.824049 sfctools-1.0.6.0/sfctools/gui/attune/.gitignore
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.824049 sfctools-1.0.6.0/sfctools/gui/attune/__init__.py
+-rw-r--r--   0        0        0      177 2022-12-22 08:51:44.532604 sfctools-1.0.6.0/sfctools/gui/attune/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      159 2022-11-23 08:49:18.431057 sfctools-1.0.6.0/sfctools/gui/attune/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.825207 sfctools-1.0.6.0/sfctools/gui/attune/src/__init__.py
+-rw-r--r--   0        0        0      181 2022-12-22 08:51:44.534815 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      163 2022-11-23 08:49:18.433350 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    50257 2023-01-25 08:23:24.448393 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc
+-rw-r--r--   0        0        0    20359 2023-04-04 07:45:31.111570 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    70418 2023-01-25 08:50:00.544297 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc
+-rw-r--r--   0        0        0    35547 2023-05-04 12:10:55.425301 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    16034 2023-01-25 08:23:21.221015 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc
+-rw-r--r--   0        0        0    10518 2023-05-04 09:43:05.888334 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    10890 2023-01-25 08:23:21.216723 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc
+-rw-r--r--   0        0        0     4813 2023-02-06 10:17:36.928510 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc
+-rw-r--r--   0        0        0    32862 2023-01-25 08:23:21.227665 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc
+-rw-r--r--   0        0        0    12521 2023-04-04 07:45:30.873144 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc
+-rw-r--r--   0        0        0     2435 2023-01-25 08:23:21.211969 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2023-04-04 07:45:30.862180 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc
+-rw-r--r--   0        0        0   152005 2023-01-25 08:47:50.827103 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc
+-rw-r--r--   0        0        0    69406 2023-05-04 09:43:04.168970 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc
+-rw-r--r--   0        0        0     7007 2023-01-25 08:23:24.383425 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc
+-rw-r--r--   0        0        0     6499 2022-11-23 08:49:30.377800 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc
+-rw-r--r--   0        0        0    10255 2023-01-25 08:23:24.459690 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     5060 2023-05-04 09:43:06.152185 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc
+-rw-r--r--   0        0        0    14167 2023-01-25 08:23:24.456539 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc
+-rw-r--r--   0        0        0     9595 2023-05-04 09:43:06.142977 sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc
+-rw-r--r--   0        0        0    34561 2023-03-21 16:33:08.121051 sfctools-1.0.6.0/sfctools/gui/attune/src/agent_editor.py
+-rw-r--r--   0        0        0     6944 2023-05-04 09:42:20.696719 sfctools-1.0.6.0/sfctools/gui/attune/src/code_editor.ui
+-rw-r--r--   0        0        0    74439 2023-05-04 12:10:37.548919 sfctools-1.0.6.0/sfctools/gui/attune/src/draw_widget.py
+-rw-r--r--   0        0        0     1645 2023-01-26 10:34:36.660166 sfctools-1.0.6.0/sfctools/gui/attune/src/income_viewer.ui
+-rw-r--r--   0        0        0    13476 2023-05-04 09:42:20.697720 sfctools-1.0.6.0/sfctools/gui/attune/src/mainloop_editor.py
+-rw-r--r--   0        0        0     8176 2023-01-26 10:34:36.661270 sfctools-1.0.6.0/sfctools/gui/attune/src/mamba_interpreter2.py
+-rw-r--r--   0        0        0     1334 2023-03-21 16:33:08.123171 sfctools-1.0.6.0/sfctools/gui/attune/src/matrix_viewer.ui
+-rw-r--r--   0        0        0    19411 2023-03-21 16:33:08.124171 sfctools-1.0.6.0/sfctools/gui/attune/src/output_display.py
+-rw-r--r--   0        0        0    11200 2022-11-23 08:34:47.835944 sfctools-1.0.6.0/sfctools/gui/attune/src/output_display.ui
+-rw-r--r--   0        0        0     1066 2023-04-04 07:33:37.003243 sfctools-1.0.6.0/sfctools/gui/attune/src/pandasmodel.py
+-rw-r--r--   0        0        0   136567 2023-05-04 09:42:20.699719 sfctools-1.0.6.0/sfctools/gui/attune/src/qtattune.py
+-rw-r--r--   0        0        0    24104 2022-11-23 08:34:47.840835 sfctools-1.0.6.0/sfctools/gui/attune/src/resources.py
+-rw-r--r--   0        0        0      107 2022-11-23 08:34:47.840835 sfctools-1.0.6.0/sfctools/gui/attune/src/resources.qrc
+-rw-r--r--   0        0        0     1259 2023-05-04 09:42:20.699719 sfctools-1.0.6.0/sfctools/gui/attune/src/search_dialog.ui
+-rw-r--r--   0        0        0     5927 2023-03-21 16:33:08.126466 sfctools-1.0.6.0/sfctools/gui/attune/src/settings_edit.ui
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:08.127467 sfctools-1.0.6.0/sfctools/gui/attune/src/simulation_edit.ui
+-rw-r--r--   0        0        0      216 2023-01-26 10:34:36.664276 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/bright/background.txt
+-rw-r--r--   0        0        0     4020 2023-03-21 16:33:08.127467 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/bright/main.txt
+-rw-r--r--   0        0        0       62 2023-01-26 10:34:36.665242 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/bright/tables.txt
+-rw-r--r--   0        0        0      727 2023-01-26 10:34:36.665497 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/dark/background.txt
+-rw-r--r--   0        0        0     4228 2023-03-21 16:33:08.128524 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/dark/main.txt
+-rw-r--r--   0        0        0       37 2023-01-26 10:34:36.666498 sfctools-1.0.6.0/sfctools/gui/attune/src/styles/dark/tables.txt
+-rw-r--r--   0        0        0     6964 2023-05-04 09:42:20.699719 sfctools-1.0.6.0/sfctools/gui/attune/src/theme_manager.py
+-rw-r--r--   0        0        0    85086 2023-05-04 12:11:57.367531 sfctools-1.0.6.0/sfctools/gui/attune/src/transaction_designer_mainwindow.ui
+-rw-r--r--   0        0        0    11636 2023-05-04 09:42:20.700719 sfctools-1.0.6.0/sfctools/gui/attune/src/yaml_editor.py
+-rw-r--r--   0        0        0      357 2023-03-21 16:33:08.130565 sfctools-1.0.6.0/sfctools/gui/attune_main.py
+-rw-r--r--   0        0        0      389 2023-03-21 16:33:08.130565 sfctools-1.0.6.0/sfctools/gui/attune_starter.py
+-rw-r--r--   0        0        0    27804 2022-11-23 08:34:47.819952 sfctools-1.0.6.0/sfctools/gui/CLA.pdf
+-rw-r--r--   0        0        0     1434 2022-11-23 08:34:47.820915 sfctools-1.0.6.0/sfctools/gui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1157 2022-11-23 08:34:47.821917 sfctools-1.0.6.0/sfctools/gui/LICENSE
+-rw-r--r--   0        0        0      819 2023-01-26 10:34:36.656502 sfctools-1.0.6.0/sfctools/gui/README.md
+-rw-r--r--   0        0        0       47 2022-12-22 09:03:58.496002 sfctools-1.0.6.0/sfctools/gui/runner.py
+-rw-r--r--   0        0        0      275 2023-05-04 09:42:20.701720 sfctools-1.0.6.0/sfctools/gui/sfctheme
+-rw-r--r--   0        0        0     4765 2022-11-23 09:50:36.467143 sfctools-1.0.6.0/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2022-11-23 08:34:47.855670 sfctools-1.0.6.0/sfctools/misc/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-25 08:23:20.056190 sfctools-1.0.6.0/sfctools/misc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      153 2023-01-19 21:54:26.534886 sfctools-1.0.6.0/sfctools/misc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13145 2023-02-06 10:24:45.828385 sfctools-1.0.6.0/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc
+-rw-r--r--   0        0        0    10106 2023-01-25 08:23:20.059255 sfctools-1.0.6.0/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc
+-rw-r--r--   0        0        0     7616 2023-04-04 07:45:30.288586 sfctools-1.0.6.0/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc
+-rw-r--r--   0        0        0    12006 2023-01-25 08:23:21.230666 sfctools-1.0.6.0/sfctools/misc/__pycache__/timeseries.cpython-311.pyc
+-rw-r--r--   0        0        0     6420 2023-01-25 08:17:49.793565 sfctools-1.0.6.0/sfctools/misc/__pycache__/timeseries.cpython-38.pyc
+-rw-r--r--   0        0        0    18645 2023-03-21 16:33:08.131566 sfctools-1.0.6.0/sfctools/misc/mpl_plotting.py
+-rw-r--r--   0        0        0     7795 2023-03-21 16:33:08.131566 sfctools-1.0.6.0/sfctools/misc/reporting_sheet.py
+-rw-r--r--   0        0        0     7074 2022-11-23 08:34:47.858698 sfctools-1.0.6.0/sfctools/misc/timeseries.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 sfctools-1.0.6.0/setup.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 sfctools-1.0.6.0/PKG-INFO
```

### Comparing `sfctools-1.0.5.9/LICENSE` & `sfctools-1.0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/pyproject.toml` & `sfctools-1.0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sfctools"
-version = "1.0.5.9"
+version = "1.0.6.0"
 description = "Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields."
 
 authors = ["Thomas Baldauf <thomas.baldauf@dlr.de>"]
 license = "MIT"
 maintainers = ["Thomas Baldauf, Benjamin Fuchs <thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de>"]
 homepage = 'https://gitlab.com/dlr-ve/esy/sfctools/framework'
 documentation = 'https://sfctools-framework.readthedocs.io/en/latest/'
```

### Comparing `sfctools-1.0.5.9/README.md` & `sfctools-1.0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/__init__.py` & `sfctools-1.0.6.0/sfctools/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/__main__.py` & `sfctools-1.0.6.0/sfctools/__main__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/automation/__pycache__/runner.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/automation/__pycache__/runner.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/automation/__pycache__/runner.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/automation/calibration.py` & `sfctools-1.0.6.0/sfctools/automation/calibration.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/automation/cgesolver.py` & `sfctools-1.0.6.0/sfctools/automation/cgesolver.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/automation/runner.py` & `sfctools-1.0.6.0/sfctools/automation/runner.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/matching.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/matching.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/productiontree.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/stock_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/stock_manager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/bottomup/__pycache__/treestruct.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/matching.py` & `sfctools-1.0.6.0/sfctools/bottomup/matching.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/productiontree.py` & `sfctools-1.0.6.0/sfctools/bottomup/productiontree.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/stock_manager.py` & `sfctools-1.0.6.0/sfctools/bottomup/stock_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/bottomup/treestruct.py` & `sfctools-1.0.6.0/sfctools/bottomup/treestruct.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/agent.cpython-39.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/clock.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/clock.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/clock.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/custom_warnings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/custom_warnings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/flow_matrix.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/flow_matrix.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/settings.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/singleton.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/singleton.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/singleton.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/__pycache__/world.cpython-39.pyc` & `sfctools-1.0.6.0/sfctools/core/__pycache__/world.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/agent.py` & `sfctools-1.0.6.0/sfctools/core/agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/clock.py` & `sfctools-1.0.6.0/sfctools/core/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/flow_matrix.py` & `sfctools-1.0.6.0/sfctools/core/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/settings.py` & `sfctools-1.0.6.0/sfctools/core/settings.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/singleton.py` & `sfctools-1.0.6.0/sfctools/core/singleton.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/core/world.py` & `sfctools-1.0.6.0/sfctools/core/world.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/balance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/balance.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/balance.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/bank_order_book.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/bank_order_book.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/cash_flow_statement.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/collection.cpython-39.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/collection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/income_statement.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/income_statement.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/inventory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/inventory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/market_registry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/market_registry.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/signalslot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/signalslot.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/worker_registry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/datastructs/__pycache__/worker_registry.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/balance.py` & `sfctools-1.0.6.0/sfctools/datastructs/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/bank_order_book.py` & `sfctools-1.0.6.0/sfctools/datastructs/bank_order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/cash_flow_statement.py` & `sfctools-1.0.6.0/sfctools/datastructs/cash_flow_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/collection.py` & `sfctools-1.0.6.0/sfctools/datastructs/collection.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/income_statement.py` & `sfctools-1.0.6.0/sfctools/datastructs/income_statement.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/inventory.py` & `sfctools-1.0.6.0/sfctools/datastructs/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/market_registry.py` & `sfctools-1.0.6.0/sfctools/datastructs/market_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/signalslot.py` & `sfctools-1.0.6.0/sfctools/datastructs/signalslot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/datastructs/worker_registry.py` & `sfctools-1.0.6.0/sfctools/datastructs/worker_registry.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/__init__.py` & `sfctools-1.0.6.0/sfctools/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/balance.py` & `sfctools-1.0.6.0/sfctools/examples/balance.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/basic_example/basic_example.py` & `sfctools-1.0.6.0/sfctools/examples/basic_example/basic_example.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/clock.py` & `sfctools-1.0.6.0/sfctools/examples/clock.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/example_wrapper.py` & `sfctools-1.0.6.0/sfctools/examples/example_wrapper.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/government.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/government.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/household.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/household.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/production.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/production.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/agents/transactions.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/agents/transactions.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/preprocess.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/data/processed/tipsau20_gdp_processed.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/data/raw/tipsau20_gdp.csv`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/matrix.png` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/matrix.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/outputs.png` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/outputs.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/figures/sankey.png` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/figures/sankey.png`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/info.md` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/info.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/model.py` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/model.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/exampleabm/settings.yml` & `sfctools-1.0.6.0/sfctools/examples/exampleabm/settings.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/flowmatrix.py` & `sfctools-1.0.6.0/sfctools/examples/flowmatrix.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/hello_agent.py` & `sfctools-1.0.6.0/sfctools/examples/hello_agent.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/inventory.py` & `sfctools-1.0.6.0/sfctools/examples/inventory.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/market_example/market.py` & `sfctools-1.0.6.0/sfctools/examples/market_example/market.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/market_example/market2.py` & `sfctools-1.0.6.0/sfctools/examples/market_example/market2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/monte_carlo/monte_carlo.py` & `sfctools-1.0.6.0/sfctools/examples/monte_carlo/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/monte_carlo/result/output.txt` & `sfctools-1.0.6.0/sfctools/examples/monte_carlo/result/output.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/order_book.py` & `sfctools-1.0.6.0/sfctools/examples/order_book.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/examples/signal_slot.py` & `sfctools-1.0.6.0/sfctools/examples/signal_slot.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/.gitlab-ci.yml` & `sfctools-1.0.6.0/sfctools/gui/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/__pycache__/attune_main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/__pycache__/attune_main.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/__pycache__/attune_main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/agent_editor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/draw_widget.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May  4 12:02:56 2023 UTC, .py size: 74357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 f09e 5364 7522 0100  U.........Sdu"..
+00000000: 550d 0d0a 0000 0000 bda0 5364 c722 0100  U.........Sd."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c01 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -1188,16 +1188,16 @@
 00004a30: 0212 0110 0218 0208 0108 0204 0112 0112  ................
 00004a40: 0212 0112 0216 0116 0208 0204 0118 0108  ................
 00004a50: 0108 0208 010a 0218 0108 0108 0208 010a  ................
 00004a60: 0318 0108 0108 0208 010a 0318 0108 0108  ................
 00004a70: 0208 0108 0506 010e 0238 0338 027a 1a4d  .........8.8.z.M
 00004a80: 7944 7261 7757 6964 6765 742e 6472 6177  yDrawWidget.draw
 00004a90: 5f61 7272 6f77 5f61 7454 630d 0000 0000  _arrow_atTc.....
-00004aa0: 0000 0000 0000 003c 0000 000a 0000 0003  .......<........
-00004ab0: 0000 0073 be07 0000 6401 7c06 8806 1800  ...s....d.|.....
+00004aa0: 0000 0000 0000 003b 0000 000a 0000 0003  .......;........
+00004ab0: 0000 0073 0208 0000 6401 7c06 8806 1800  ...s....d.|.....
 00004ac0: 1400 8806 1700 7d0d 6401 7c04 7c06 1800  ......}.d.|.|...
 00004ad0: 1400 7c06 1700 7d0e 6401 7c07 8807 1800  ..|...}.d.|.....
 00004ae0: 1400 8807 1700 7d0f 6401 7c05 7c07 1800  ......}.d.|.|...
 00004af0: 1400 7c07 1700 7d10 6402 7d11 7c06 7d12  ..|...}.d.}.|.}.
 00004b00: 7c07 7d13 7c04 7d14 7c05 7d15 7c04 7c06  |.}.|.}.|.}.|.|.
 00004b10: 6b05 728c 7c05 7c07 6b05 728c 7400 7c06  k.r.|.|.k.r.t.|.
 00004b20: 7c04 1800 8301 7c11 6b04 728c 7c06 7c11  |.....|.k.r.|.|.
@@ -1243,976 +1243,980 @@
 00004da0: 6700 7d20 7c20 a004 7c1f 6406 1900 a101  g.} | ..|.d.....
 00004db0: 0100 7405 6407 7406 7c1f 8301 8302 4400  ..t.d.t.|.....D.
 00004dc0: 5d34 7d21 7c1f 7c21 6408 1800 1900 6406  ]4}!|.|!d.....d.
 00004dd0: 1900 7c1f 7c21 1900 6406 1900 6b02 9003  ..|.|!..d...k...
 00004de0: 722c 6e0e 7c20 a004 7c1f 7c21 1900 a101  r,n.| ..|.|!....
 00004df0: 0100 9003 7108 7401 a002 7c20 a101 7d20  ....q.t...| ..} 
 00004e00: 8704 6601 6409 640a 8408 7c20 4400 8301  ..f.d.d...| D...
-00004e10: 7d20 640b 5c02 7d22 7d23 9004 7a16 7401  } d.\.}"}#..z.t.
+00004e10: 7d20 640b 5c02 7d22 7d23 9004 7a5a 7401  } d.\.}"}#..zZt.
 00004e20: a007 7401 a008 7401 6a09 7401 6a0a 7c20  ..t...t.j.t.j.| 
 00004e30: 6406 640c 8d02 6407 1300 6408 640c 8d02  d.d...d...d.d...
 00004e40: a101 a101 7d24 7401 a00b 7c24 6406 6406  ....}$t...|$d.d.
 00004e50: a103 7c24 640d 1900 1b00 7d24 8804 6a0c  ..|$d.....}$..j.
-00004e60: 9004 7398 7c1e 9003 73e0 8804 6a0d 7d25  ..s.|...s...j.}%
+00004e60: 9004 73ba 7c1e 9003 73e0 8804 6a0d 7d25  ..s.|...s...j.}%
 00004e70: 7401 a00e 6406 6408 640e a103 7d26 740f  t...d.d.d...}&t.
 00004e80: 7c24 7c20 7c25 6406 640f 8d04 7d27 7c27  |$| |%d.d...}'|'
-00004e90: 7c26 8301 7d28 6eb4 6401 7c06 8806 1800  |&..}(n.d.|.....
+00004e90: 7c26 8301 7d28 6ed6 6401 7c06 8806 1800  |&..}(n.d.|.....
 00004ea0: 1400 8900 6401 7c07 8807 1800 1400 8901  ....d.|.........
-00004eb0: 6401 7401 a008 8806 7c06 1800 6407 1300  d.t.....|...d...
-00004ec0: 8807 7c07 1800 6407 1300 1700 a101 1400  ..|...d.........
-00004ed0: 7d29 7401 a010 7c07 8807 1800 7c06 8806  })t...|.....|...
-00004ee0: 1800 a102 8905 8805 7401 a00e 6406 6407  ........t...d.d.
-00004ef0: 7401 6a11 1400 6410 a103 1700 7d2a 7c29  t.j...d.....}*|)
-00004f00: 8902 6411 7c29 1400 8903 8700 8702 8703  ..d.|)..........
-00004f10: 8705 8706 6605 6412 640a 8408 7c2a 4400  ....f.d.d...|*D.
-00004f20: 8301 7d2b 8701 8702 8703 8705 8707 6605  ..}+..........f.
-00004f30: 6413 640a 8408 7c2a 4400 8301 7d2c 7412  d.d...|*D...},t.
-00004f40: 7413 7c2b 7c2c 8302 8301 7d28 9001 6e70  t.|+|,....}(..np
-00004f50: 6414 7d25 7401 a00e 6406 6408 6415 a103  d.}%t...d.d.d...
-00004f60: 7d26 740f 7c24 7c20 7c25 6406 640f 8d04  }&t.|$| |%d.d...
-00004f70: 7d27 7c27 7c26 8301 7d2d 7c20 6406 1900  }'|'|&..}-| d...
-00004f80: 6406 1900 8906 7c20 6406 1900 6408 1900  d.....| d...d...
-00004f90: 8907 7c20 640d 1900 6406 1900 7d04 7c20  ..| d...d...}.| 
-00004fa0: 640d 1900 6408 1900 7d05 7c1e 9005 7354  d...d...}.|...sT
-00004fb0: 8804 a014 8806 8807 7c06 7c07 6416 a105  ........|.|.d...
-00004fc0: 5c02 7d2e 7d2f 8804 a014 7c06 7c07 7c08  \.}.}/....|.|.|.
-00004fd0: 7c09 6416 a105 5c02 7d30 7d31 8804 a014  |.d...\.}0}1....
-00004fe0: 7c08 7c09 7c04 7c05 6416 a105 5c02 7d32  |.|.|.|.d...\.}2
-00004ff0: 7d33 7c2e 7c30 1700 7c32 1700 7d2b 7c2f  }3|.|0..|2..}+|/
-00005000: 7c31 1700 7c33 1700 7d2c 6ea6 6401 7c06  |1..|3..},n.d.|.
-00005010: 8806 1800 1400 8900 6401 7c07 8807 1800  ........d.|.....
-00005020: 1400 8901 6401 7401 a008 8806 7c06 1800  ....d.t.....|...
-00005030: 6407 1300 8807 7c07 1800 6407 1300 1700  d.....|...d.....
-00005040: a101 1400 7d29 7401 a010 7c07 8807 1800  ....})t...|.....
-00005050: 7c06 8806 1800 a102 8905 8805 7401 a00e  |...........t...
-00005060: 6406 6407 7401 6a11 1400 6410 a103 1700  d.d.t.j...d.....
-00005070: 7d2a 7c29 8902 6411 7c29 1400 8903 8700  }*|)..d.|)......
-00005080: 8702 8703 8705 8706 6605 6417 640a 8408  ........f.d.d...
-00005090: 7c2a 4400 8301 7d2b 8701 8702 8703 8705  |*D...}+........
-000050a0: 8707 6605 6418 640a 8408 7c2a 4400 8301  ..f.d.d...|*D...
-000050b0: 7d2c 7412 7413 7c2b 7c2c 8302 8301 7d28  },t.t.|+|,....}(
-000050c0: 7406 7c28 8301 7d34 6419 7d35 7c01 a015  t.|(..}4d.}5|...
-000050d0: 7416 6a17 a101 0100 7418 8300 7d36 8804  t.j.....t...}6..
-000050e0: 6a19 7c28 6406 1900 6406 1900 1400 7d37  j.|(d...d.....}7
-000050f0: 8804 6a19 7c28 6406 1900 6408 1900 1400  ..j.|(d...d.....
-00005100: 7d38 7c36 a01a 7c37 7c38 a102 0100 7405  }8|6..|7|8....t.
-00005110: 6408 741b 7c34 6407 1b00 8301 7c35 1800  d.t.|4d.....|5..
-00005120: 8302 4400 5d2e 7d21 7c36 a01c 8804 6a19  ..D.].}!|6....j.
-00005130: 7c28 7c21 1900 6406 1900 1400 8804 6a19  |(|!..d.......j.
-00005140: 7c28 7c21 1900 6408 1900 1400 a102 0100  |(|!..d.........
-00005150: 9006 716c 7405 741b 7c34 6407 1b00 8301  ..qlt.t.|4d.....
-00005160: 7c35 1800 7406 7c28 8301 8302 4400 5d2e  |5..t.|(....D.].
-00005170: 7d21 7c36 a01c 8804 6a19 7c28 7c21 1900  }!|6....j.|(|!..
-00005180: 6406 1900 1400 8804 6a19 7c28 7c21 1900  d.......j.|(|!..
-00005190: 6408 1900 1400 a102 0100 9006 71b6 7c36  d...........q.|6
-000051a0: a01a 7c37 7c38 a102 0100 7c36 a01d a100  ..|7|8....|6....
-000051b0: 0100 7c01 a01e 7c36 a101 0100 741b 7c34  ..|...|6....t.|4
-000051c0: 641a 1b00 8301 7d39 6403 7d3a 7c1e 9007  d.....}9d.}:|...
-000051d0: 7330 8804 6a1f 7c01 7c28 7c39 7c0a 641b  s0..j.|.|(|9|.d.
-000051e0: 8d04 5c02 7d22 7d23 7c0c 9007 7378 7c1e  ..\.}"}#|...sx|.
-000051f0: 9007 7378 8804 6a20 6a21 a022 a100 9007  ..sx..j j!."....
-00005200: 7278 7c3a 9007 7378 741b 7c34 641a 1b00  rx|:..sxt.|4d...
-00005210: 640e 1800 8301 7d39 8804 6a1f 7c01 7c28  d.....}9..j.|.|(
-00005220: 7c39 6405 7c0a 641c 8d05 5c02 7d22 7d23  |9d.|.d...\.}"}#
-00005230: 5700 6e3a 0400 7423 6b0a 9007 72b4 0100  W.n:..t#k...r...
-00005240: 7d3b 0100 7a1a 7424 641d 7425 7c3b 8301  };..z.t$d.t%|;..
-00005250: 8302 0100 6406 7d22 6406 7d23 5700 3500  ....d.}"d.}#W.5.
-00005260: 641e 7d3b 7e3b 5800 5900 6e02 5800 7c22  d.};~;X.Y.n.X.|"
-00005270: 7c23 6602 5300 291f 7a2a 0a20 2020 2020  |#f.S.).z*.     
-00005280: 2020 2064 7261 7773 2061 2063 7572 7665     draws a curve
-00005290: 6420 636f 6e6e 6563 746f 720a 2020 2020  d connector.    
-000052a0: 2020 2020 72a5 0000 00e9 1900 0000 4667      r.........Fg
-000052b0: 7b14 ae47 e17a 943f 5472 0100 0000 7230  {..G.z.?Tr....r0
-000052c0: 0000 0072 1200 0000 6301 0000 0000 0000  ...r....c.......
-000052d0: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-000052e0: 0073 2800 0000 6700 7c00 5d20 7d01 8800  .s(...g.|.] }...
-000052f0: a000 7c01 6400 1900 a101 8800 a000 7c01  ..|.d.........|.
-00005300: 6401 1900 a101 6602 9102 7104 5300 2902  d.....f...q.S.).
-00005310: 7201 0000 0072 1200 0000 2901 723f 0000  r....r....).r?..
-00005320: 0029 0272 0d01 0000 da01 7472 2b00 0000  .).r......tr+...
-00005330: 7221 0000 0072 2200 0000 720e 0100 0029  r!...r"...r....)
-00005340: 0400 0073 0400 0000 0600 0200 7a31 4d79  ...s........z1My
-00005350: 4472 6177 5769 6467 6574 2e63 7572 7665  DrawWidget.curve
-00005360: 645f 636f 6e6e 6563 746f 722e 3c6c 6f63  d_connector.<loc
-00005370: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
-00005380: 0272 0100 0000 7201 0000 0029 01da 0461  .r....r....)...a
-00005390: 7869 7372 a400 0000 7204 0100 0029 02da  xisr....r....)..
-000053a0: 046b 696e 6472 3f01 0000 7299 0000 0067  .kindr?...r....g
-000053b0: 9a99 9999 9999 e93f 6301 0000 0000 0000  .......?c.......
-000053c0: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-000053d0: 0073 4400 0000 6700 7c00 5d3c 7d01 8801  .sD...g.|.]<}...
-000053e0: 7400 a001 7c01 a101 1400 7400 a001 8803  t...|.....t.....
-000053f0: a101 1400 8802 7400 a002 7c01 a101 1400  ......t...|.....
-00005400: 7400 a002 8803 a101 1400 1800 8800 1700  t...............
-00005410: 8804 1700 9102 7104 5300 7221 0000 00a9  ......q.S.r!....
-00005420: 0372 9a00 0000 722a 0100 0072 2b01 0000  .r....r*...r+...
-00005430: a902 720d 0100 00da 0274 69a9 05da 0363  ..r......ti....c
-00005440: 3078 da02 7278 da02 7279 da02 7430 725e  0x..rx..ry..t0r^
-00005450: 0000 0072 2100 0000 7222 0000 0072 0e01  ...r!...r"...r..
-00005460: 0000 4d04 0000 7304 0000 0006 0002 0063  ..M...s........c
-00005470: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00005480: 0700 0000 1300 0000 7344 0000 0067 007c  ........sD...g.|
-00005490: 005d 3c7d 0188 0174 00a0 017c 01a1 0114  .]<}...t...|....
-000054a0: 0074 00a0 0288 03a1 0114 0088 0274 00a0  .t...........t..
-000054b0: 027c 01a1 0114 0074 00a0 0188 03a1 0114  .|.....t........
-000054c0: 0017 0088 0017 0088 0417 0091 0271 0453  .............q.S
-000054d0: 0072 2100 0000 7241 0100 0072 4201 0000  .r!...rA...rB...
-000054e0: a905 da03 6330 7972 4601 0000 7247 0100  ....c0yrF...rG..
-000054f0: 0072 4801 0000 725f 0000 0072 2100 0000  .rH...r_...r!...
-00005500: 7222 0000 0072 0e01 0000 4e04 0000 7304  r"...r....N...s.
-00005510: 0000 0006 0002 00da 066c 696e 6561 7272  .........linearr
-00005520: 6800 0000 e96f 0000 0063 0100 0000 0000  h....o...c......
-00005530: 0000 0000 0000 0200 0000 0700 0000 1300  ................
-00005540: 0000 7344 0000 0067 007c 005d 3c7d 0188  ..sD...g.|.]<}..
-00005550: 0174 00a0 017c 01a1 0114 0074 00a0 0188  .t...|.....t....
-00005560: 03a1 0114 0088 0274 00a0 027c 01a1 0114  .......t...|....
-00005570: 0074 00a0 0288 03a1 0114 0018 0088 0017  .t..............
-00005580: 0088 0417 0091 0271 0453 0072 2100 0000  .......q.S.r!...
-00005590: 7241 0100 0072 4201 0000 7244 0100 0072  rA...rB...rD...r
-000055a0: 2100 0000 7222 0000 0072 0e01 0000 7b04  !...r"...r....{.
-000055b0: 0000 7304 0000 0006 0002 0063 0100 0000  ..s........c....
-000055c0: 0000 0000 0000 0000 0200 0000 0700 0000  ................
-000055d0: 1300 0000 7344 0000 0067 007c 005d 3c7d  ....sD...g.|.]<}
-000055e0: 0188 0174 00a0 017c 01a1 0114 0074 00a0  ...t...|.....t..
-000055f0: 0288 03a1 0114 0088 0274 00a0 027c 01a1  .........t...|..
-00005600: 0114 0074 00a0 0188 03a1 0114 0017 0088  ...t............
-00005610: 0017 0088 0417 0091 0271 0453 0072 2100  .........q.S.r!.
-00005620: 0000 7241 0100 0072 4201 0000 7249 0100  ..rA...rB...rI..
-00005630: 0072 2100 0000 7222 0000 0072 0e01 0000  .r!...r"...r....
-00005640: 7c04 0000 7304 0000 0006 0002 00e9 1400  |...s...........
-00005650: 0000 7225 0100 0029 0172 3101 0000 2902  ..r%...).r1...).
-00005660: 7230 0100 0072 3101 0000 7a1c 4572 726f  r0...r1...z.Erro
-00005670: 7220 696e 204c 696e 6520 496e 7465 7270  r in Line Interp
-00005680: 6f6c 6174 696f 6e3a 4e29 2672 1601 0000  olation:N)&r....
-00005690: 729a 0000 00da 0561 7272 6179 da01 5472  r......array..Tr
-000056a0: 0501 0000 da05 7261 6e67 6572 0f01 0000  ......ranger....
-000056b0: da06 6375 6d73 756d da04 7371 7274 da03  ..cumsum..sqrt..
-000056c0: 7375 6dda 0464 6966 66da 0669 6e73 6572  sum..diff..inser
-000056d0: 7472 cf00 0000 72cc 0000 0072 1801 0000  tr....r....r....
-000056e0: 7209 0000 0072 2901 0000 7226 0100 0072  r....r)...r&...r
-000056f0: 1701 0000 da03 7a69 7072 2301 0000 da0d  ......zipr#.....
-00005700: 7365 7452 656e 6465 7248 696e 7472 0400  setRenderHintr..
-00005710: 0000 5a0c 416e 7469 616c 6961 7369 6e67  ..Z.Antialiasing
-00005720: 7205 0000 0072 3400 0000 5a06 6d6f 7665  r....r4...Z.move
-00005730: 546f 7240 0000 005a 066c 696e 6554 6f5a  Tor@...Z.lineToZ
-00005740: 0c63 6c6f 7365 5375 6270 6174 685a 0864  .closeSubpathZ.d
-00005750: 7261 7750 6174 6872 3c01 0000 7235 0000  rawPathr<...r5..
-00005760: 0072 2c01 0000 7237 0000 0072 e800 0000  .r,...r7...r....
-00005770: 7215 0000 0072 e900 0000 293c 7227 0000  r....r....)<r'..
-00005780: 0072 4500 0000 725e 0000 0072 5f00 0000  .rE...r^...r_...
-00005790: 7219 0100 0072 1a01 0000 da02 7869 da02  r....r......xi..
-000057a0: 7969 da02 7864 da02 7964 7231 0100 00da  yi..xd..ydr1....
-000057b0: 0769 735f 666c 6f77 da09 6973 5f75 6e69  .is_flow..is_uni
-000057c0: 6469 72da 0378 6932 5a03 7869 335a 0379  dir..xi2Z.xi3Z.y
-000057d0: 6932 5a03 7969 3372 9e00 0000 5a03 7869  i2Z.yi3r....Z.xi
-000057e0: 345a 0379 6934 5a03 7869 355a 0379 6935  4Z.yi4Z.xi5Z.yi5
-000057f0: 5a03 7869 365a 0379 6936 5a03 7869 375a  Z.xi6Z.yi6Z.xi7Z
-00005800: 0379 6937 5a04 7869 3632 5a04 7969 3632  .yi7Z.xi62Z.yi62
-00005810: 5a04 7869 3335 5a04 7969 3335 5a0c 656e  Z.xi35Z.yi35Z.en
-00005820: 645f 6973 5f73 7461 7274 5a07 706f 696e  d_is_startZ.poin
-00005830: 7473 32da 0670 6f69 6e74 73da 0169 7239  ts2..points..ir9
-00005840: 0100 0072 3a01 0000 da08 6469 7374 616e  ...r:.....distan
-00005850: 6365 da06 6d65 7468 6f64 da05 616c 7068  ce..method..alph
-00005860: 61da 0c69 6e74 6572 706f 6c61 746f 7272  a..interpolatorr
-00005870: 1e01 0000 da01 7272 3e01 0000 7221 0100  ......rr>...r!..
-00005880: 0072 2201 0000 da02 6970 5a03 7863 315a  .r".....ipZ.xc1Z
-00005890: 0379 6331 da03 7863 32da 0379 6332 da03  .yc1..xc2..yc2..
-000058a0: 7863 33da 0379 6333 721b 0100 0072 2f01  xc3..yc3r....r/.
-000058b0: 0000 5a08 636f 6e6e 5061 7468 da06 7374  ..Z.connPath..st
-000058c0: 6172 7478 da06 7374 6172 7479 722e 0100  artx..startyr...
-000058d0: 005a 0c64 7261 775f 7265 7665 7273 6572  .Z.draw_reverser
-000058e0: 9700 0000 7221 0000 0029 0872 4501 0000  ....r!...).rE...
-000058f0: 724a 0100 0072 4601 0000 7247 0100 0072  rJ...rF...rG...r
-00005900: 2700 0000 7248 0100 0072 5e00 0000 725f  '...rH...r^...r_
-00005910: 0000 0072 2200 0000 da10 6375 7276 6564  ...r".....curved
-00005920: 5f63 6f6e 6e65 6374 6f72 9603 0000 7324  _connector....s$
-00005930: 0100 0000 0c10 0110 0110 0110 0404 0204  ................
-00005940: 0104 0104 0104 0320 0108 0104 0108 0104  ....... ........
-00005950: 0320 0108 0104 0108 0104 0320 0108 0104  . ......... ....
-00005960: 0108 0104 0326 0108 0104 0108 0104 0204  .....&..........
-00005970: 0104 0104 0104 0326 0108 0104 0108 0104  .......&........
-00005980: 0326 0108 0104 0108 0104 0326 0108 0104  .&.........&....
-00005990: 0108 0104 0326 0108 0104 0108 0104 070c  .....&..........
-000059a0: 010c 0b0c 010c 1104 0124 0104 0110 010c  .........$......
-000059b0: ff0a 0910 010c ff08 0304 010e 0212 011e  ................
-000059c0: 0102 0212 020a 0112 0208 0204 0128 0116  .............(..
-000059d0: 0508 0106 0206 010e 0310 010a 060c 010c  ................
-000059e0: 0222 0214 0218 0104 0108 021a 011a 0212  ."..............
-000059f0: 0404 010e 0410 0108 020c 010c 010c 010c  ................
-00005a00: 0406 0216 0116 0216 020c 010e 050c 010c  ................
-00005a10: 0222 0214 0218 0104 0108 021a 011a 040e  ."..............
-00005a20: 0308 0404 020c 0206 0112 0112 020c 021a  ................
-00005a30: 032c 021e 032c 020c 0208 010a 060c 0304  .,...,..........
-00005a40: 0206 0116 0206 0114 0106 0110 011c 0512  ................
-00005a50: 010e 0104 0116 1b7a 1d4d 7944 7261 7757  .......z.MyDrawW
-00005a60: 6964 6765 742e 6375 7276 6564 5f63 6f6e  idget.curved_con
-00005a70: 6e65 6374 6f72 6302 0000 0000 0000 0000  nectorc.........
-00005a80: 0000 0011 0000 0009 0000 0003 0000 0073  ...............s
-00005a90: ee03 0000 8808 6a00 6a01 a002 a100 7310  ......j.j.....s.
-00005aa0: 6400 5300 7403 a004 8808 6a00 6a05 a006  d.S.t.....j.j...
-00005ab0: 6401 a101 6402 a102 7d02 7c01 a007 7c02  d...d...}.|...|.
-00005ac0: a101 0100 6403 8909 6403 8903 6404 8900  ....d...d...d...
-00005ad0: 6405 8904 6405 8905 7403 a008 7403 a009  d...d...t...t...
-00005ae0: 6403 6403 6403 6406 a104 6402 a102 7d03  d.d.d.d...d...}.
-00005af0: 7c01 a00a 740b a00c 8804 6407 1800 8805  |...t.....d.....
-00005b00: 6407 1800 8809 6405 1700 8803 6405 1700  d.....d.....d...
-00005b10: a104 7c03 a102 0100 740d 8808 6a0e 8301  ..|.....t...j...
-00005b20: 6408 6b02 7296 6400 5300 740f 6408 8808  d.k.r.d.S.t.d...
-00005b30: 6a10 0b00 8302 7d04 7411 8808 6a12 8808  j.....}.t...j...
-00005b40: 6a12 8808 6a10 1800 8302 7d05 740f 6408  j...j.....}.t.d.
-00005b50: 8808 6a13 0b00 8302 7d06 7411 8808 6a14  ..j.....}.t...j.
-00005b60: 8808 6a14 8808 6a13 1800 8302 7d07 6700  ..j...j.....}.g.
-00005b70: 7d08 6700 7d09 8808 6a0e 4400 5d1c 7d0a  }.g.}...j.D.].}.
-00005b80: 7c08 a015 7c0a 6a16 a101 0100 7c09 a015  |...|.j.....|...
-00005b90: 7c0a 6a17 a101 0100 71e8 7411 7418 a011  |.j.....q.t.t...
-00005ba0: 7c08 a101 8808 6a10 0b00 8302 7d05 7411  |.....j.....}.t.
-00005bb0: 7418 a011 7c09 a101 8808 6a13 0b00 8302  t...|.....j.....
-00005bc0: 7d07 740f 7418 a00f 7c08 a101 8808 6a10  }.t.t...|.....j.
-00005bd0: 0b00 8302 7d04 740f 7418 a00f 7c09 a101  ....}.t.t...|...
-00005be0: 8808 6a13 0b00 8302 7d06 7c05 7c04 6b02  ..j.....}.|.|.k.
-00005bf0: 9001 7268 7c04 6405 1700 7d05 7c07 7c06  ..rh|.d...}.|.|.
-00005c00: 6b02 9001 727a 7c06 6405 1700 7d07 7c05  k...rz|.d...}.|.
-00005c10: 8808 6a12 6b00 9001 728c 8808 6a12 7d05  ..j.k...r...j.}.
-00005c20: 7c07 8808 6a14 6b00 9001 729e 8808 6a14  |...j.k...r...j.
-00005c30: 7d07 8708 6601 6409 640a 8408 7c08 4400  }...f.d.d...|.D.
-00005c40: 8301 7d08 8708 6601 640b 640a 8408 7c09  ..}...f.d.d...|.
-00005c50: 4400 8301 7d09 7c08 a015 8808 6a19 6405  D...}.|.....j.d.
-00005c60: 1b00 8808 6a10 640c 8808 6a12 1400 1700  ....j.d...j.....
-00005c70: 1400 a101 0100 7c09 a015 8808 6a19 6405  ......|.....j.d.
-00005c80: 1b00 8808 6a13 640c 8808 6a14 1400 1700  ....j.d...j.....
-00005c90: 1400 a101 0100 7c08 a015 640d 640c 8808  ......|...d.d...
-00005ca0: 6a12 1400 1400 a101 0100 7c09 a015 640d  j.........|...d.
-00005cb0: 640c 8808 6a14 1400 1400 a101 0100 7418  d...j.........t.
-00005cc0: a01a 7c08 a101 8906 7418 a01a 7c09 a101  ..|.....t...|...
-00005cd0: 8907 8706 6601 640e 640a 8408 7c08 4400  ....f.d.d...|.D.
-00005ce0: 8301 7d08 8707 6601 640f 640a 8408 7c09  ..}...f.d.d...|.
-00005cf0: 4400 8301 7d09 7411 7418 a00f 7c08 a101  D...}.t.t...|...
-00005d00: 0b00 7418 a011 7c08 a101 8302 8901 7411  ..t...|.......t.
-00005d10: 7418 a00f 7c09 a101 0b00 7418 a011 7c09  t...|.....t...|.
-00005d20: a101 8302 8902 8701 8709 6602 6410 640a  ..........f.d.d.
-00005d30: 8408 7c08 4400 8301 7d08 8702 8703 6602  ..|.D...}.....f.
-00005d40: 6411 640a 8408 7c09 4400 8301 7d09 8709  d.d...|.D...}...
-00005d50: 6601 6412 640a 8408 7c08 4400 8301 7d08  f.d.d...|.D...}.
-00005d60: 8703 6601 6413 640a 8408 7c09 4400 8301  ..f.d.d...|.D...
-00005d70: 7d09 8700 8704 6602 6414 640a 8408 7c08  }.....f.d.d...|.
-00005d80: 4400 8301 7d08 8700 8705 6602 6415 640a  D...}.....f.d.d.
-00005d90: 8408 7c09 4400 8301 7d09 741b 740d 7c08  ..|.D...}.t.t.|.
-00005da0: 8301 6401 1800 8301 4400 5d46 7d0b 7c08  ..d.....D.]F}.|.
-00005db0: 7c0b 1900 7d0c 7c09 7c0b 1900 7d0d 8808  |...}.|.|...}...
-00005dc0: 6a0e 7c0b 1900 6a1c 9003 724a 7c01 a01d  j.|...j...rJ|...
-00005dd0: 7c0c 7c0d 6402 6402 a104 0100 6e10 7c01  |.|.d.d.....n.|.
-00005de0: a01d 7c0c 7c0d 6416 6416 a104 0100 9003  ..|.|.d.d.......
-00005df0: 7116 7c08 6417 1900 7d0c 7c09 6417 1900  q.|.d...}.|.d...
-00005e00: 7d0d 7403 a004 8808 6a00 6a05 a006 6416  }.t.....j.j...d.
-00005e10: a101 6402 a102 7d02 7c01 a007 7c02 a101  ..d...}.|...|...
-00005e20: 0100 7c0c 7d0e 7c0d 7d0f 6407 7d10 7c01  ..|.}.|.}.d.}.|.
-00005e30: a01e 741f 7c0e 7c10 1800 8301 741f 7c0f  ..t.|.|.....t.|.
-00005e40: 8301 741f 7c0e 7c10 1700 8301 741f 7c0f  ..t.|.|.....t.|.
-00005e50: 8301 a104 0100 7c01 a01e 741f 7c0e 8301  ......|...t.|...
-00005e60: 741f 7c0f 7c10 1800 8301 741f 7c0e 8301  t.|.|.....t.|...
-00005e70: 741f 7c0f 7c10 1700 8301 a104 0100 6400  t.|.|.........d.
-00005e80: 5300 2918 4e72 3000 0000 7212 0000 00e9  S.).Nr0...r.....
-00005e90: 5000 0000 723d 0100 0072 dd00 0000 7299  P...r=...r....r.
-00005ea0: 0000 0072 6800 0000 7201 0000 0063 0100  ...rh...r....c..
-00005eb0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00005ec0: 0000 1300 0000 7320 0000 0067 007c 005d  ......s ...g.|.]
-00005ed0: 187d 0188 006a 007c 0188 006a 0117 0014  .}...j.|...j....
-00005ee0: 0064 001b 0091 0271 0453 00a9 0172 dd00  .d.....q.S...r..
-00005ef0: 0000 2902 7234 0000 0072 3c00 0000 2902  ..).r4...r<...).
-00005f00: 720d 0100 0072 5801 0000 722b 0000 0072  r....rX...r+...r
-00005f10: 2100 0000 7222 0000 0072 0e01 0000 0905  !...r"...r......
-00005f20: 0000 7304 0000 0006 0002 007a 2b4d 7944  ..s........z+MyD
-00005f30: 7261 7757 6964 6765 742e 6461 7750 7265  rawWidget.dawPre
-00005f40: 7669 6577 2e3c 6c6f 6361 6c73 3e2e 3c6c  view.<locals>.<l
-00005f50: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
-00005f60: 0000 0000 0002 0000 0005 0000 0013 0000  ................
-00005f70: 0073 2000 0000 6700 7c00 5d18 7d01 8800  .s ...g.|.].}...
-00005f80: 6a00 7c01 8800 6a01 1700 1400 6400 1b00  j.|...j.....d...
-00005f90: 9102 7104 5300 726f 0100 0029 0272 3400  ..q.S.ro...).r4.
-00005fa0: 0000 723d 0000 0029 0272 0d01 0000 7259  ..r=...).r....rY
-00005fb0: 0100 0072 2b00 0000 7221 0000 0072 2200  ...r+...r!...r".
-00005fc0: 0000 720e 0100 000a 0500 0073 0400 0000  ..r........s....
-00005fd0: 0600 0200 72a5 0000 0072 3100 0000 6301  ....r....r1...c.
-00005fe0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00005ff0: 0000 0013 0000 0073 1400 0000 6700 7c00  .......s....g.|.
-00006000: 5d0c 7d01 7c01 8800 1800 9102 7104 5300  ].}.|.......q.S.
-00006010: 7221 0000 0072 2100 0000 a902 720d 0100  r!...r!.....r...
-00006020: 0072 1a00 0000 2901 da02 6d78 7221 0000  .r....)...mxr!..
-00006030: 0072 2200 0000 720e 0100 0017 0500 0073  .r"...r........s
-00006040: 0400 0000 0600 0200 6301 0000 0000 0000  ........c.......
-00006050: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00006060: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
-00006070: 8800 1800 9102 7104 5300 7221 0000 0072  ......q.S.r!...r
-00006080: 2100 0000 a902 720d 0100 0072 1b00 0000  !.....r....r....
-00006090: 2901 da02 6d79 7221 0000 0072 2200 0000  )...myr!...r"...
-000060a0: 720e 0100 0018 0500 0073 0400 0000 0600  r........s......
-000060b0: 0200 6301 0000 0000 0000 0000 0000 0002  ..c.............
-000060c0: 0000 0004 0000 0013 0000 0073 1c00 0000  ...........s....
-000060d0: 6700 7c00 5d14 7d01 6400 8801 1400 7c01  g.|.].}.d.....|.
-000060e0: 1400 8800 1b00 9102 7104 5300 a901 72a5  ........q.S...r.
-000060f0: 0000 0072 2100 0000 7270 0100 0029 0272  ...r!...rp...).r
-00006100: 6600 0000 da07 775f 6672 616d 6572 2100  f.....w_framer!.
-00006110: 0000 7222 0000 0072 0e01 0000 1d05 0000  ..r"...r........
-00006120: 7304 0000 0006 0002 0063 0100 0000 0000  s........c......
-00006130: 0000 0000 0000 0200 0000 0400 0000 1300  ................
-00006140: 0000 731c 0000 0067 007c 005d 147d 0164  ..s....g.|.].}.d
-00006150: 0088 0114 007c 0114 0088 001b 0091 0271  .....|.........q
-00006160: 0453 0072 7401 0000 7221 0000 0072 7201  .S.rt...r!...rr.
-00006170: 0000 2902 7267 0000 00da 0768 5f66 7261  ..).rg.....h_fra
-00006180: 6d65 7221 0000 0072 2200 0000 720e 0100  mer!...r"...r...
-00006190: 001e 0500 0073 0400 0000 0600 0200 6301  .....s........c.
-000061a0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000061b0: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
-000061c0: 5d10 7d01 7c01 6400 8800 1400 1700 9102  ].}.|.d.........
-000061d0: 7104 5300 7274 0100 0072 2100 0000 7270  q.S.rt...r!...rp
-000061e0: 0100 0029 0172 7501 0000 7221 0000 0072  ...).ru...r!...r
-000061f0: 2200 0000 720e 0100 0020 0500 0073 0400  "...r.... ...s..
-00006200: 0000 0600 0200 6301 0000 0000 0000 0000  ......c.........
-00006210: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-00006220: 1800 0000 6700 7c00 5d10 7d01 7c01 6400  ....g.|.].}.|.d.
-00006230: 8800 1400 1700 9102 7104 5300 7274 0100  ........q.S.rt..
-00006240: 0072 2100 0000 7272 0100 0029 0172 7601  .r!...rr...).rv.
-00006250: 0000 7221 0000 0072 2200 0000 720e 0100  ..r!...r"...r...
-00006260: 0021 0500 0073 0400 0000 0600 0200 6301  .!...s........c.
-00006270: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00006280: 0000 0013 0000 0073 2800 0000 6700 7c00  .......s(...g.|.
-00006290: 5d20 7d01 8801 7400 8800 6400 1b00 8301  ] }...t...d.....
-000062a0: 1700 7c01 1700 6400 1800 6401 1800 9102  ..|...d...d.....
-000062b0: 7104 5300 a902 7230 0000 0072 dd00 0000  q.S...r0...r....
-000062c0: a901 7240 0000 0072 7001 0000 2902 7261  ..r@...rp...).ra
-000062d0: 0100 00da 066d 6f76 655f 7872 2100 0000  .....move_xr!...
-000062e0: 7222 0000 0072 0e01 0000 2305 0000 7304  r"...r....#...s.
-000062f0: 0000 0006 0002 0063 0100 0000 0000 0000  .......c........
-00006300: 0000 0000 0200 0000 0600 0000 1300 0000  ................
-00006310: 7328 0000 0067 007c 005d 207d 0188 0174  s(...g.|.] }...t
-00006320: 0088 0064 001b 0083 0117 007c 0117 0064  ...d.......|...d
-00006330: 0018 0064 0118 0091 0271 0453 0072 7701  ...d.....q.S.rw.
-00006340: 0000 7278 0100 0072 7201 0000 2902 7261  ..rx...rr...).ra
-00006350: 0100 00da 066d 6f76 655f 7972 2100 0000  .....move_yr!...
-00006360: 7222 0000 0072 0e01 0000 2405 0000 7304  r"...r....$...s.
-00006370: 0000 0006 0002 0072 6900 0000 72a4 0000  .......ri...r...
-00006380: 0029 2072 3500 0000 da0a 6368 6563 6b42  .) r5.....checkB
-00006390: 6f78 5f39 7237 0000 0072 0600 0000 da04  ox_9r7...r......
-000063a0: 5150 656e 7288 0000 00da 0967 6574 5f63  QPenr......get_c
-000063b0: 6f6c 6f72 da06 7365 7450 656e da06 5142  olor..setPen..QB
-000063c0: 7275 7368 da06 5143 6f6c 6f72 7243 0000  rush..QColorrC..
-000063d0: 0072 0300 0000 7241 0000 0072 0f01 0000  .r....rA...r....
-000063e0: 7296 0000 00da 036d 696e 723c 0000 0072  r......minr<...r
-000063f0: c200 0000 729e 0000 0072 3d00 0000 729f  ....r....r=...r.
-00006400: 0000 0072 0501 0000 721a 0000 0072 1b00  ...r....r....r..
-00006410: 0000 729a 0000 0072 3400 0000 da04 6d65  ..r....r4.....me
-00006420: 616e 7250 0100 0072 6100 0000 da08 6472  anrP...ra.....dr
-00006430: 6177 5265 6374 722d 0100 0072 4000 0000  awRectr-...r@...
-00006440: 2911 7227 0000 0072 4500 0000 da03 7065  ).r'...rE.....pe
-00006450: 6e72 4600 0000 da05 785f 6d69 6eda 0578  nrF.....x_min..x
-00006460: 5f6d 6178 da05 795f 6d69 6eda 0579 5f6d  _max..y_min..y_m
-00006470: 6178 5a06 785f 7661 6c73 5a06 795f 7661  axZ.x_valsZ.y_va
-00006480: 6c73 7223 0000 0072 6001 0000 721a 0000  lsr#...r`...r...
-00006490: 0072 1b00 0000 da02 6f78 da02 6f79 72aa  .r......ox..oyr.
-000064a0: 0000 0072 2100 0000 290a 7261 0100 0072  ...r!...).ra...r
-000064b0: 6600 0000 7267 0000 0072 7601 0000 7279  f...rg...rv...ry
-000064c0: 0100 0072 7a01 0000 7271 0100 0072 7301  ...rz...rq...rs.
-000064d0: 0000 7227 0000 0072 7501 0000 7222 0000  ..r'...ru...r"..
-000064e0: 00da 0a64 6177 5072 6576 6965 77d5 0400  ...dawPreview...
-000064f0: 0073 8600 0000 0003 0c01 0402 1601 0a06  .s..............
-00006500: 0401 0401 0401 0401 0402 1801 2802 0e01  ............(...
-00006510: 0402 0e01 1401 0e01 1401 0401 0402 0a01  ................
-00006520: 0c01 0e03 1401 1401 1401 1402 0a01 0801  ................
-00006530: 0a01 0802 0c01 0601 0c01 0602 1201 1203  ................
-00006540: 2001 2003 1401 1402 0a01 0a02 1201 1202   . .............
-00006550: 1801 1802 1401 1402 1201 1202 1401 1404  ................
-00006560: 1401 0801 0801 0e01 1209 1403 0801 0801  ................
-00006570: 1601 0a01 0401 0401 0401 2801 7a17 4d79  ..........(.z.My
-00006580: 4472 6177 5769 6467 6574 2e64 6177 5072  DrawWidget.dawPr
-00006590: 6576 6965 7763 0300 0000 0000 0000 0000  eviewc..........
-000065a0: 0000 0500 0000 0300 0000 4300 0000 7332  ..........C...s2
-000065b0: 0000 007c 006a 0072 2a74 017c 027c 006a  ...|.j.r*t.|.|.j
-000065c0: 0283 027d 0374 037c 017c 031b 0083 017c  ...}.t.|.|.....|
-000065d0: 0314 007d 0474 037c 0483 0153 0074 037c  ...}.t.|...S.t.|
-000065e0: 0183 0153 0072 2900 0000 2904 72cf 0000  ...S.r)...).r...
-000065f0: 0072 8101 0000 72ce 0000 0072 4000 0000  .r....r....r@...
-00006600: 2905 7227 0000 0072 1a00 0000 721b 0100  ).r'...r....r...
-00006610: 00da 016d 5a0a 785f 7261 7374 6572 6564  ...mZ.x_rastered
-00006620: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00006630: 3f00 0000 4d05 0000 730a 0000 0000 0106  ?...M...s.......
-00006640: 020c 0110 0108 017a 134d 7944 7261 7757  .......z.MyDrawW
-00006650: 6964 6765 742e 7261 7374 6572 7212 0000  idget.rasterr...
-00006660: 0063 0300 0000 0000 0000 0000 0000 2300  .c............#.
-00006670: 0000 0e00 0000 4300 0000 736c 0b00 0074  ......C...sl...t
-00006680: 00a0 017c 01a1 017d 037c 03a0 027c 027c  ...|...}.|...|.|
-00006690: 02a1 0201 007c 03a0 0374 006a 016a 04a1  .....|...t.j.j..
-000066a0: 0101 007c 03a0 0374 006a 016a 05a1 0101  ...|...t.j.j....
-000066b0: 0074 00a0 067c 006a 076a 08a0 0964 01a1  .t...|.j.j...d..
-000066c0: 0164 02a1 027d 047c 03a0 0a7c 04a1 0101  .d...}.|...|....
-000066d0: 007c 006a 076a 0ba0 0ca1 0072 d474 00a0  .|.j.j.....r.t..
-000066e0: 0d74 00a0 0e64 0364 0364 0364 03a1 0464  .t...d.d.d.d...d
-000066f0: 02a1 027d 057c 03a0 0f74 10a0 1174 10a0  ...}.|...t...t..
-00006700: 1264 0464 04a1 0274 10a0 1274 137c 006a  .d.d...t...t.|.j
-00006710: 1464 0118 0083 0174 137c 006a 1564 0118  .d.....t.|.j.d..
-00006720: 0083 01a1 02a1 027c 05a1 0201 007c 017c  .......|.....|.|
-00006730: 006b 0272 f87c 03a0 1664 0464 047c 006a  .k.r.|...d.d.|.j
-00006740: 1464 0118 007c 006a 1564 0518 00a1 0401  .d...|.j.d......
-00006750: 006e 247c 017c 006b 0272 f87c 03a0 1664  .n$|.|.k.r.|...d
-00006760: 0464 047c 006a 1464 0118 007c 006a 1564  .d.|.j.d...|.j.d
-00006770: 0518 00a1 0401 007c 03a0 0a7c 04a1 0101  .......|...|....
-00006780: 0074 1764 0664 0784 007c 006a 076a 18a0  .t.d.d...|.j.j..
-00006790: 19a1 0044 0083 0183 017d 0667 007d 0767  ...D.....}.g.}.g
-000067a0: 007d 087c 006a 1a44 005d 9c7d 0974 1b7c  .}.|.j.D.].}.t.|
-000067b0: 0683 0164 046b 027d 0a74 1b7c 0683 0164  ...d.k.}.t.|...d
-000067c0: 046b 0390 016f 6074 1b74 1c74 177c 096a  .k...o`t.t.t.|.j
-000067d0: 1d83 017c 0640 0083 0183 0164 046b 047d  ...|.@.....d.k.}
-000067e0: 0b7c 0a90 0173 6e7c 0b90 0172 2a7c 097c  .|...sn|...r*|.|
-000067f0: 086b 0790 0172 2a7c 006a 1e64 006b 0890  .k...r*|.j.d.k..
-00006800: 0172 907c 08a0 1f7c 09a1 0101 006e 347c  .r.|...|.....n4|
-00006810: 096a 207c 006a 1e6b 0290 0173 ba7c 096a  .j |.j.k...s.|.j
-00006820: 217c 006a 1e6b 0290 0173 ba7c 096a 227c  !|.j.k...s.|.j"|
-00006830: 006a 1e6b 0290 0172 2a7c 08a0 1f7c 09a1  .j.k...r*|...|..
-00006840: 0101 0090 0171 2a7c 006a 1a44 0090 055d  .....q*|.j.D...]
-00006850: f07d 0964 087d 0c64 097d 0d7c 096a 227c  .}.d.}.d.}.|.j"|
-00006860: 006a 1e6b 0290 0272 4c74 00a0 067c 006a  .j.k...rLt...|.j
-00006870: 076a 08a0 0964 05a1 0164 0aa1 027d 0464  .j...d...d...}.d
-00006880: 087d 0c74 237c 006a 076a 2483 0144 005d  .}.t#|.j.j$..D.]
-00006890: 385c 027d 0e7d 0f7c 0f64 0b19 007c 096a  8\.}.}.|.d...|.j
-000068a0: 226a 256b 0290 0272 1074 267c 0f64 0c19  "j%k...r.t&|.d..
-000068b0: 0083 0164 0d6b 0290 0272 4064 097d 0c01  ...d.k...r@d.}..
-000068c0: 0090 0371 4890 0271 106e fc74 00a0 067c  ...qH..q.n.t...|
-000068d0: 006a 076a 08a0 0964 01a1 0164 0ea1 027d  .j.j...d...d...}
-000068e0: 047c 097c 086b 0690 0372 1c64 097d 0d64  .|.|.k...r.d.}.d
-000068f0: 087d 0c74 237c 006a 076a 2483 0144 005d  .}.t#|.j.j$..D.]
-00006900: 4e5c 027d 0e7d 0f7c 0f64 0b19 007c 096a  N\.}.}.|.d...|.j
-00006910: 226a 256b 0290 0272 8074 267c 0f64 0f19  "j%k...r.t&|.d..
-00006920: 0083 0164 106b 0290 0272 b064 087d 0d74  ...d.k...r.d.}.t
-00006930: 267c 0f64 0c19 0083 0164 0d6b 0290 0272  &|.d.....d.k...r
-00006940: c664 097d 0c01 0090 0271 d090 0271 807c  .d.}.....q...q.|
-00006950: 0d90 0272 ee74 00a0 067c 006a 076a 08a0  ...r.t...|.j.j..
-00006960: 0964 01a1 0164 0ea1 027d 046e 1674 00a0  .d...d...}.n.t..
-00006970: 067c 006a 076a 08a0 0964 05a1 0164 0ea1  .|.j.j...d...d..
-00006980: 027d 047c 04a0 2774 286a 29a1 0101 007c  .}.|..'t(j)....|
-00006990: 04a0 2a64 0ea1 0101 006e 2c7c 04a0 2774  ..*d.....n,|..'t
-000069a0: 286a 2ba1 0101 007c 04a0 2c64 0264 0567  (j+....|..,d.d.g
-000069b0: 02a1 0101 007c 04a0 2a64 11a1 0101 0064  .....|..*d.....d
-000069c0: 097d 0d64 087d 0c7c 03a0 0a7c 04a1 0101  .}.d.}.|...|....
-000069d0: 0064 087d 1064 127d 117c 097c 086b 0690  .d.}.d.}.|.|.k..
-000069e0: 0772 0a7c 006a 2d7c 037c 006a 2e74 137c  .r.|.j-|.|.j.t.|
-000069f0: 096a 206a 2f7c 1117 0083 0117 007c 006a  .j j/|.......|.j
-00006a00: 3074 137c 096a 206a 317c 1117 0083 0117  0t.|.j j1|......
-00006a10: 007c 006a 2e74 137c 096a 216a 2f7c 1117  .|.j.t.|.j!j/|..
-00006a20: 0083 0117 007c 006a 3074 137c 096a 216a  .....|.j0t.|.j!j
-00006a30: 317c 1117 0083 0117 007c 006a 2e74 137c  1|.......|.j.t.|
-00006a40: 096a 226a 2f64 1317 0083 0117 007c 006a  .j"j/d.......|.j
-00006a50: 3074 137c 096a 226a 3164 1317 0083 0117  0t.|.j"j1d......
-00006a60: 007c 006a 2e74 137c 096a 326a 2f64 1317  .|.j.t.|.j2j/d..
-00006a70: 0083 0117 007c 006a 3074 137c 096a 326a  .....|.j0t.|.j2j
-00006a80: 3164 1317 0083 0117 007c 0d7c 0c64 148d  1d.......|.|.d..
-00006a90: 0b5c 027d 127d 137c 096a 207c 076b 0790  .\.}.}.|.j |.k..
-00006aa0: 0472 307c 07a0 1f7c 096a 20a1 0101 007c  .r0|...|.j ....|
-00006ab0: 096a 217c 076b 0790 0472 487c 07a0 1f7c  .j!|.k...rH|...|
-00006ac0: 096a 21a1 0101 007c 096a 227c 076b 0790  .j!....|.j"|.k..
-00006ad0: 0472 607c 07a0 1f7c 096a 22a1 0101 007c  .r`|...|.j"....|
-00006ae0: 096a 327c 076b 0790 0472 787c 07a0 1f7c  .j2|.k...rx|...|
-00006af0: 096a 32a1 0101 007c 096a 227c 006a 1e6b  .j2....|.j"|.j.k
-00006b00: 0290 0472 a874 00a0 067c 006a 076a 08a0  ...r.t...|.j.j..
-00006b10: 0964 15a1 0164 0ea1 027d 047c 03a0 0a7c  .d...d...}.|...|
-00006b20: 04a1 0101 006e 2074 00a0 067c 006a 076a  .....n t...|.j.j
-00006b30: 08a0 0964 02a1 0164 0ea1 027d 047c 03a0  ...d...d...}.|..
-00006b40: 0a7c 04a1 0101 007c 006a 076a 33a0 0ca1  .|.....|.j.j3...
-00006b50: 0090 0572 8e7c 006a 076a 34a0 0ca1 0090  ...r.|.j.j4.....
-00006b60: 0772 087c 006a 1e7c 096a 226b 0290 0572  .r.|.j.|.j"k...r
-00006b70: 0a74 00a0 0d7c 006a 076a 08a0 0964 05a1  .t...|.j.j...d..
-00006b80: 0164 02a1 027d 146e 1674 00a0 0d7c 006a  .d...}.n.t...|.j
-00006b90: 076a 08a0 0964 16a1 0164 02a1 027d 1464  .j...d...d...}.d
-00006ba0: 177d 157a 2474 137c 006a 076a 35a0 36a1  .}.z$t.|.j.j5.6.
-00006bb0: 0083 017d 157c 03a0 3774 3864 187c 1583  ...}.|..7t8d.|..
-00006bc0: 02a1 0101 0057 006e 3004 0074 396b 0a90  .....W.n0..t9k..
-00006bd0: 0572 7801 007d 1601 007a 1074 3a74 267c  .rx..}...z.t:t&|
-00006be0: 1683 0183 0101 0057 0035 0064 007d 167e  .......W.5.d.}.~
-00006bf0: 1658 0059 006e 0258 007c 096a 226a 3ba0  .X.Y.n.X.|.j"j;.
-00006c00: 3c7c 037c 14a1 0201 0090 0771 be7c 006a  <|.|.......q.|.j
-00006c10: 076a 34a0 0ca1 0090 0772 be7c 006a 1e7c  .j4......r.|.j.|
-00006c20: 096a 226b 0290 0572 c274 00a0 0d7c 006a  .j"k...r.t...|.j
-00006c30: 076a 08a0 0964 05a1 0164 02a1 027d 146e  .j...d...d...}.n
-00006c40: 1674 00a0 0d7c 006a 076a 08a0 0964 16a1  .t...|.j.j...d..
-00006c50: 0164 02a1 027d 147c 096a 206a 2f7c 096a  .d...}.|.j j/|.j
-00006c60: 216a 2f6b 0390 0672 2e7c 096a 206a 317c  !j/k...r.|.j j1|
-00006c70: 096a 216a 316b 0390 0672 2e7c 006a 3d7c  .j!j1k...r.|.j=|
-00006c80: 1214 007d 177c 006a 3d7c 1314 007d 187c  ...}.|.j=|...}.|
-00006c90: 006a 3d7c 1264 1317 0014 007d 197c 006a  .j=|.d.....}.|.j
-00006ca0: 3d7c 1364 1317 0014 007d 1a6e 687c 006a  =|.d.....}.nh|.j
-00006cb0: 3d7c 006a 2e7c 096a 226a 2f17 0014 007d  =|.j.|.j"j/....}
-00006cc0: 177c 006a 3d7c 006a 307c 096a 226a 3117  .|.j=|.j0|.j"j1.
-00006cd0: 0014 007d 187c 006a 3d7c 006a 2e7c 096a  ...}.|.j=|.j.|.j
-00006ce0: 326a 3b6a 2f17 007c 096a 326a 3b6a 3e17  2j;j/..|.j2j;j>.
-00006cf0: 0014 007d 197c 006a 3d7c 006a 307c 096a  ...}.|.j=|.j0|.j
-00006d00: 326a 3b6a 3117 007c 096a 326a 3b6a 3f17  2j;j1..|.j2j;j?.
-00006d10: 0014 007d 1a64 177d 157a 2474 137c 006a  ...}.d.}.z$t.|.j
-00006d20: 076a 35a0 36a1 0083 017d 157c 03a0 3774  .j5.6....}.|..7t
-00006d30: 3864 187c 1583 02a1 0101 0057 006e 3004  8d.|.......W.n0.
-00006d40: 0074 396b 0a90 0672 ee01 007d 1601 007a  .t9k...r...}...z
-00006d50: 1074 3a74 267c 1683 0183 0101 0057 0035  .t:t&|.......W.5
-00006d60: 0064 007d 167e 1658 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
-00006d70: 096a 226a 3b6a 3c7c 037c 147c 197c 1a66  .j"j;j<|.|.|.|.f
-00006d80: 0264 198d 0301 006e b47c 006a 2d7c 037c  .d.....n.|.j-|.|
-00006d90: 006a 2e74 137c 096a 206a 2f7c 1117 0083  .j.t.|.j j/|....
-00006da0: 0117 007c 006a 3074 137c 096a 206a 317c  ...|.j0t.|.j j1|
-00006db0: 1117 0083 0117 007c 006a 2e74 137c 096a  .......|.j.t.|.j
-00006dc0: 216a 2f7c 1117 0083 0117 007c 006a 3074  !j/|.......|.j0t
-00006dd0: 137c 096a 216a 317c 1117 0083 0117 007c  .|.j!j1|.......|
-00006de0: 006a 2e74 137c 096a 226a 2f64 1317 0083  .j.t.|.j"j/d....
-00006df0: 0117 007c 006a 3074 137c 096a 226a 3164  ...|.j0t.|.j"j1d
-00006e00: 1317 0083 0117 007c 006a 2e74 137c 096a  .......|.j.t.|.j
-00006e10: 326a 2f64 1317 0083 0117 007c 006a 3074  2j/d.......|.j0t
-00006e20: 137c 096a 326a 3164 1317 0083 0117 007c  .|.j2j1d.......|
-00006e30: 0d7c 0c64 148d 0b5c 027d 127d 1390 0171  .|.d...\.}.}...q
-00006e40: ce74 00a0 067c 006a 076a 08a0 0964 01a1  .t...|.j.j...d..
-00006e50: 0164 02a1 027d 047c 04a0 2774 286a 29a1  .d...}.|..'t(j).
-00006e60: 0101 007c 03a0 0a7c 04a1 0101 007c 006a  ...|...|.....|.j
-00006e70: 4044 0090 035d 667d 1b7c 1b7c 006a 416b  @D...]f}.|.|.jAk
-00006e80: 0390 0872 147c 1b6a 2f7d 1c7c 1b6a 317d  ...r.|.j/}.|.j1}
-00006e90: 1d6e 307c 1b7c 006a 416b 0290 0872 447c  .n0|.|.jAk...rD|
-00006ea0: 006a 427c 006a 3e17 007d 1c7c 006a 437c  .jB|.j>..}.|.jC|
-00006eb0: 006a 3f17 007d 1d7c 1c7c 1b5f 2f7c 1d7c  .j?..}.|.|._/|.|
-00006ec0: 1b5f 317c 1b7c 006a 416b 0290 0872 6874  ._1|.|.jAk...rht
-00006ed0: 00a0 0d74 00a0 0e64 1a64 1a64 1b64 03a1  ...t...d.d.d.d..
-00006ee0: 04a1 017d 1e6e 887c 1b7c 006a 446b 0290  ...}.n.|.|.jDk..
-00006ef0: 0872 8c74 00a0 0d74 00a0 0e64 1c64 1d64  .r.t...t...d.d.d
-00006f00: 1d64 03a1 04a1 017d 1e6e 647c 1b6a 4590  .d.....}.nd|.jE.
-00006f10: 0872 b87c 1b7c 006a 1e6b 0390 0872 b874  .r.|.|.j.k...r.t
-00006f20: 00a0 0d7c 006a 076a 08a0 0964 04a1 0164  ...|.j.j...d...d
-00006f30: 02a1 027d 1e6e 387c 1b7c 006a 1e6b 0290  ...}.n8|.|.j.k..
-00006f40: 0872 da74 00a0 0d7c 006a 076a 08a0 0964  .r.t...|.j.j...d
-00006f50: 13a1 01a1 017d 1e6e 1674 00a0 0d7c 006a  .....}.n.t...|.j
-00006f60: 076a 08a0 0964 04a1 0164 02a1 027d 1e74  .j...d...d...}.t
-00006f70: 137c 1c83 017d 1c74 137c 1d83 017d 1d7c  .|...}.t.|...}.|
-00006f80: 1b6a 4590 0972 6074 00a0 067c 006a 076a  .jE..r`t...|.j.j
-00006f90: 08a0 0964 15a1 0164 02a1 027d 047c 1b6a  ...d...d...}.|.j
-00006fa0: 4690 0972 3e74 00a0 0d7c 006a 076a 08a0  F..r>t...|.j.j..
-00006fb0: 0964 1ea1 0164 02a1 027d 1e6e 1674 00a0  .d...d...}.n.t..
-00006fc0: 0d7c 006a 076a 08a0 0964 02a1 0164 02a1  .|.j.j...d...d..
-00006fd0: 027d 1e7c 03a0 0a7c 04a1 0101 006e d67c  .}.|...|.....n.|
-00006fe0: 006a 3d7c 1c7c 006a 2e17 0014 007d 177c  .j=|.|.j.....}.|
-00006ff0: 006a 3d7c 1d64 1f18 007c 006a 3017 0014  .j=|.d...|.j0...
-00007000: 007d 1874 00a0 067c 006a 076a 08a0 0964  .}.t...|.j.j...d
-00007010: 15a1 0164 02a1 027d 047c 03a0 0a7c 04a1  ...d...}.|...|..
-00007020: 0101 0064 207d 157a 2474 137c 006a 076a  ...d }.z$t.|.j.j
-00007030: 47a0 36a1 0083 017d 157c 03a0 3774 3864  G.6....}.|..7t8d
-00007040: 187c 1583 02a1 0101 0057 006e 3004 0074  .|.......W.n0..t
-00007050: 396b 0a90 0972 fc01 007d 1601 007a 1074  9k...r...}...z.t
-00007060: 3a74 267c 1683 0183 0101 0057 0035 0064  :t&|.......W.5.d
-00007070: 007d 167e 1658 0059 006e 0258 007c 006a  .}.~.X.Y.n.X.|.j
-00007080: 076a 48a0 0ca1 0090 0a72 2474 00a0 0d7c  .jH......r$t...|
-00007090: 006a 076a 08a0 0964 16a1 0164 02a1 027d  .j.j...d...d...}
-000070a0: 1f6e 0464 007d 1f7c 1b6a 3ba0 3c7c 037c  .n.d.}.|.j;.<|.|
-000070b0: 1fa1 0201 007c 03a0 497c 1ea1 0101 007c  .....|..I|.....|
-000070c0: 1b6a 4590 0a72 ec7c 1c64 1517 007d 207c  .jE..r.|.d...} |
-000070d0: 1d64 1517 007d 2174 00a0 0674 00a0 0e64  .d...}!t...t...d
-000070e0: 0464 0464 0464 04a1 0464 04a1 027d 047c  .d.d.d...d...}.|
-000070f0: 03a0 0a7c 04a1 0101 007c 1b6a 4690 0a72  ...|.....|.jF..r
-00007100: 907c 006a 076a 4aa0 0ca1 007d 226e 0c7c  .|.j.jJ....}"n.|
-00007110: 006a 076a 4ba0 0ca1 007d 227c 2290 0a72  .j.jK....}"|"..r
-00007120: ca7c 1b7c 076b 0690 0a72 bc7c 1b6a 3c7c  .|.|.k...r.|.j<|
-00007130: 0364 0864 218d 0201 006e 0e7c 1b6a 3c7c  .d.d!....n.|.j<|
-00007140: 0364 0964 218d 0201 0074 00a0 067c 006a  .d.d!....t...|.j
-00007150: 076a 08a0 0964 01a1 0164 02a1 027d 047c  .j...d...d...}.|
-00007160: 03a0 0a7c 04a1 0101 006e 6e74 00a0 0674  ...|.....nnt...t
-00007170: 00a0 0e64 0464 0464 1c64 04a1 0464 04a1  ...d.d.d.d...d..
-00007180: 027d 047c 03a0 0a7c 04a1 0101 007c 1b7c  .}.|...|.....|.|
-00007190: 076b 0690 0b72 2a7c 1b6a 3c7c 037c 1e64  .k...r*|.j<|.|.d
-000071a0: 0864 228d 0301 006e 107c 1b6a 3c7c 037c  .d"....n.|.j<|.|
-000071b0: 1e64 0964 228d 0301 0074 00a0 067c 006a  .d.d"....t...|.j
-000071c0: 076a 08a0 0964 16a1 0164 02a1 027d 047c  .j...d...d...}.|
-000071d0: 03a0 0a7c 04a1 0101 0090 0771 f47c 00a0  ...|.......q.|..
-000071e0: 4c7c 03a1 0101 007c 0353 0029 234e 7230  L|.....|.S.)#Nr0
-000071f0: 0000 0072 1200 0000 e9ff 0000 0072 0100  ...r.........r..
-00007200: 0000 7269 0000 0063 0100 0000 0000 0000  ..ri...c........
-00007210: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00007220: 7314 0000 0067 007c 005d 0c7d 017c 01a0  s....g.|.].}.|..
-00007230: 00a1 0091 0271 0453 0072 2100 0000 2901  .....q.S.r!...).
-00007240: da04 7465 7874 2902 720d 0100 00da 0469  ..text).r......i
-00007250: 7465 6d72 2100 0000 7221 0000 0072 2200  temr!...r!...r".
-00007260: 0000 720e 0100 0077 0500 0073 0400 0000  ..r....w...s....
-00007270: 0600 0200 7a26 4d79 4472 6177 5769 6467  ....z&MyDrawWidg
-00007280: 6574 2e70 6169 6e74 2e3c 6c6f 6361 6c73  et.paint.<locals
-00007290: 3e2e 3c6c 6973 7463 6f6d 703e 5446 7225  >.<listcomp>TFr%
-000072a0: 0100 00da 0973 686f 7274 6e61 6d65 7a0f  .....shortnamez.
-000072b0: 756e 692d 6469 7265 6374 696f 6e61 6cda  uni-directional.
-000072c0: 0546 616c 7365 6700 0000 0000 00f8 3f7a  .Falseg.......?z
-000072d0: 0f6c 6f67 2074 7261 6e73 6163 7469 6f6e  .log transaction
-000072e0: da04 5472 7565 72e0 0000 0072 3d01 0000  ..Truer....r=...
-000072f0: 7268 0000 0029 0272 5c01 0000 725d 0100  rh...).r\...r]..
-00007300: 00e9 0600 0000 7228 0100 0072 9500 0000  ......r(...r....
-00007310: 5a05 4172 6961 6c29 0172 4700 0000 e922  Z.Arial).rG...."
-00007320: 0000 00e9 e600 0000 7299 0000 0072 dd00  ........r....r..
-00007330: 0000 725b 0000 00e9 0b00 0000 e90c 0000  ..r[............
-00007340: 0029 0172 6c00 0000 2902 7246 0000 0072  .).rl...).rF...r
-00007350: 6c00 0000 294d 7206 0000 0072 0400 0000  l...)Mr....r....
-00007360: da05 7363 616c 6572 5701 0000 5a17 4869  ..scalerW...Z.Hi
-00007370: 6768 5175 616c 6974 7941 6e74 6961 6c69  ghQualityAntiali
-00007380: 6173 696e 675a 1054 6578 7441 6e74 6961  asingZ.TextAntia
-00007390: 6c69 6173 696e 6772 7c01 0000 7235 0000  liasingr|...r5..
-000073a0: 0072 8800 0000 727d 0100 0072 7e01 0000  .r....r}...r~...
-000073b0: da0a 6368 6563 6b42 6f78 5f37 7237 0000  ..checkBox_7r7..
-000073c0: 0072 7f01 0000 7280 0100 0072 4300 0000  .r....r....rC...
-000073d0: 7203 0000 0072 4100 0000 7242 0000 0072  r....rA...rB...r
-000073e0: 4000 0000 729e 0000 0072 9f00 0000 7283  @...r....r....r.
-000073f0: 0100 00da 0373 6574 da0b 6669 6c74 6572  .....set..filter
-00007400: 436f 6d62 6f5a 0d73 656c 6563 7465 6449  ComboZ.selectedI
-00007410: 7465 6d73 72b3 0000 0072 0f01 0000 7217  temsr....r....r.
-00007420: 0100 0072 a800 0000 72f2 0000 0072 0501  ...r....r....r..
-00007430: 0000 724b 0000 0072 4c00 0000 72a9 0000  ..rK...rL...r...
-00007440: 00da 0965 6e75 6d65 7261 7465 da0a 656e  ...enumerate..en
-00007450: 7472 795f 6461 7461 721c 0000 0072 e900  try_datar....r..
-00007460: 0000 da08 7365 7453 7479 6c65 7207 0000  ....setStyler...
-00007470: 00da 0953 6f6c 6964 4c69 6e65 5a09 7365  ...SolidLineZ.se
-00007480: 7457 6964 7468 46da 0844 6173 684c 696e  tWidthF..DashLin
-00007490: 655a 0e73 6574 4461 7368 5061 7474 6572  eZ.setDashPatter
-000074a0: 6e72 6d01 0000 723c 0000 0072 1a00 0000  nrm...r<...r....
-000074b0: 723d 0000 0072 1b00 0000 72aa 0000 00da  r=...r....r.....
-000074c0: 0a63 6865 636b 426f 785f 35da 0a63 6865  .checkBox_5..che
-000074d0: 636b 426f 785f 32da 1173 7069 6e42 6f78  ckBox_2..spinBox
-000074e0: 466f 6e74 5369 7a65 5f32 da05 7661 6c75  FontSize_2..valu
-000074f0: 65da 0773 6574 466f 6e74 7210 0000 0072  e..setFontr....r
-00007500: e800 0000 7215 0000 0072 6000 0000 7252  ....r....r`...rR
-00007510: 0000 0072 3400 0000 7225 0000 0072 2600  ...r4...r%...r&.
-00007520: 0000 7296 0000 0072 b700 0000 72ca 0000  ..r....r....r...
-00007530: 0072 cb00 0000 72b8 0000 0072 6100 0000  .r....r....ra...
-00007540: 7262 0000 00da 0f73 7069 6e42 6f78 466f  rb.....spinBoxFo
-00007550: 6e74 5369 7a65 723e 0000 00da 0873 6574  ntSizer>.....set
-00007560: 4272 7573 68da 0a63 6865 636b 426f 785f  Brush..checkBox_
-00007570: 36da 0a63 6865 636b 426f 785f 3372 8b01  6..checkBox_3r..
-00007580: 0000 2923 7227 0000 0072 e100 0000 72e2  ..)#r'...r....r.
-00007590: 0000 0072 4500 0000 7284 0100 005a 0862  ...rE...r....Z.b
-000075a0: 725f 7768 6974 655a 0b66 696c 7465 725f  r_whiteZ.filter_
-000075b0: 7661 6c73 5a0c 6163 7469 7665 5f62 6f78  valsZ.active_box
-000075c0: 6573 5a11 6163 7469 7665 5f63 6f6e 6e65  esZ.active_conne
-000075d0: 6374 6f72 73da 0463 6f6e 6e5a 0c6e 6f5f  ctors..connZ.no_
-000075e0: 7365 6c65 6374 696f 6e5a 0b69 735f 7365  selectionZ.is_se
-000075f0: 6c65 6374 6564 725d 0100 0072 5c01 0000  lectedr]...r\...
-00007600: 7260 0100 00da 0464 6174 6172 d000 0000  r`.....datar....
-00007610: 5a0a 6f66 6673 6574 5f62 6f78 da02 7478  Z.offset_box..tx
-00007620: da02 7479 7246 0000 00da 0866 6f6e 7473  ..tyrF.....fonts
-00007630: 697a 6572 9700 0000 724b 0000 0072 4c00  izer....rK...rL.
-00007640: 0000 da02 6132 da02 6232 7223 0000 0072  ....a2..b2r#...r
-00007650: 1a00 0000 721b 0000 00da 0262 725a 0862  ....r......brZ.b
-00007660: 725f 6c61 6265 6c72 6f00 0000 7270 0000  r_labelro...rp..
-00007670: 005a 0873 686f 775f 626f 7872 2100 0000  .Z.show_boxr!...
-00007680: 7221 0000 0072 2200 0000 72ec 0000 0055  r!...r"...r....U
-00007690: 0500 0073 8c01 0000 0002 0a01 0c02 0e01  ...s............
-000076a0: 0e09 1601 0a03 0c01 1801 3801 0801 1e02  ..........8.....
-000076b0: 0801 1c06 0a02 1a01 0401 0402 0a01 0c01  ................
-000076c0: 2801 0c01 0a02 0c01 0c02 2a01 0e03 0c02  (.........*.....
-000076d0: 0401 0402 0e02 1602 0401 1401 1202 1201  ................
-000076e0: 0402 0c0b 1602 0a03 0401 0402 1401 1202  ................
-000076f0: 1201 0402 1201 0402 0a02 0601 1802 1602  ................
-00007700: 0c01 0c03 0c02 0e01 0a02 0401 0403 0a07  ................
-00007710: 0401 0402 0a03 1a01 1401 1401 1401 1400  ................
-00007720: 1401 1400 1401 0201 02f9 0a0c 0c01 0c01  ................
-00007730: 0c01 0c01 0c01 0c01 0c01 0c02 0e01 1601  ................
-00007740: 0c02 1601 0a03 0e01 0e03 0e01 1802 1602  ................
-00007750: 0402 0201 1001 1402 1201 1e02 1002 0419  ................
-00007760: 0e01 0e01 1802 1603 2403 0a01 0a02 0e01  ........$.......
-00007770: 1004 1401 1402 2001 2003 0402 0201 1001  ...... . .......
-00007780: 1402 1201 1e02 1802 0225 1a01 1401 1401  .........%......
-00007790: 1401 1400 1401 1400 1401 0201 02f9 0e11  ................
-000077a0: 1601 0c03 0a11 0c02 0c02 0601 0802 0c02  ................
-000077b0: 0c01 0c02 0601 060a 0c01 1801 0c01 1801  ................
-000077c0: 1408 1803 0c01 1608 1602 0801 0802 0801  ................
-000077d0: 1602 0801 1802 1602 0c0b 1001 1403 1601  ................
-000077e0: 0a04 0402 0201 1001 1402 1201 1e04 0e02  ................
-000077f0: 1802 040d 0e03 0a02 0802 0801 0802 1801  ................
-00007800: 0a03 0801 0e02 0c02 0601 0a08 100a 0e08  ................
-00007810: 1601 0c09 1802 0a11 0a01 1202 100c 1601  ................
-00007820: 0e01 0a05 7a12 4d79 4472 6177 5769 6467  ....z.MyDrawWidg
-00007830: 6574 2e70 6169 6e74 6302 0000 0000 0000  et.paintc.......
-00007840: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00007850: 0073 0e00 0000 7c00 a000 7c00 a101 0100  .s....|...|.....
-00007860: 6400 5300 7229 0000 0029 0172 ec00 0000  d.S.r)...).r....
-00007870: 72d4 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
-00007880: 2200 0000 da0a 7061 696e 7445 7665 6e74  ".....paintEvent
-00007890: 5d07 0000 7302 0000 0000 017a 174d 7944  ]...s......z.MyD
-000078a0: 7261 7757 6964 6765 742e 7061 696e 7445  rawWidget.paintE
-000078b0: 7665 6e74 6307 0000 0000 0000 0000 0000  ventc...........
-000078c0: 0009 0000 0004 0000 0043 0000 0073 7c00  .........C...s|.
-000078d0: 0000 7c00 6a00 7c03 7c00 6a01 1700 1400  ..|.j.|.|.j.....
-000078e0: 7c01 7c00 6a00 1400 0400 0300 6b00 6f34  |.|.j.......k.o4
-000078f0: 7c00 6a00 7c03 7c00 6a01 1700 7c05 1700  |.j.|.|.j...|...
-00007900: 1400 6b00 6e04 0200 0100 7d07 7c00 6a00  ..k.n.....}.|.j.
-00007910: 7c04 7c00 6a02 1700 1400 7c02 7c00 6a00  |.|.j.....|.|.j.
-00007920: 1400 0400 0300 6b00 6f6e 7c00 6a00 7c04  ......k.on|.j.|.
-00007930: 7c06 1700 7c00 6a02 1700 1400 6b00 6e04  |...|.j.....k.n.
-00007940: 0200 0100 7d08 7c07 6f7a 7c08 5300 2901  ....}.|.oz|.S.).
-00007950: 7a6e 0a20 2020 2020 2020 2063 6865 636b  zn.        check
-00007960: 2069 6620 2878 2c79 2920 6c69 6573 2077   if (x,y) lies w
-00007970: 6974 6869 6e20 7468 6520 7265 6374 616e  ithin the rectan
-00007980: 676c 650a 2020 2020 2020 2020 2878 622c  gle.        (xb,
-00007990: 2079 6229 2c20 2878 622c 2079 622b 7779   yb), (xb, yb+wy
-000079a0: 292c 202e 2e2e 2e2c 2028 7862 2b77 782c  ), ...., (xb+wx,
-000079b0: 2079 622b 7779 290a 2020 2020 2020 2020   yb+wy).        
-000079c0: 2903 7234 0000 0072 3c00 0000 723d 0000  ).r4...r<...r=..
-000079d0: 0029 0972 2700 0000 721a 0000 0072 1b00  .).r'...r....r..
-000079e0: 0000 da02 7862 da02 7962 721c 0100 0072  ....xb..ybr....r
-000079f0: 1d01 0000 da05 636f 6e64 31da 0563 6f6e  ......cond1..con
-00007a00: 6432 7221 0000 0072 2100 0000 7222 0000  d2r!...r!...r"..
-00007a10: 00da 0768 6974 5f62 6f78 6107 0000 7306  ...hit_boxa...s.
-00007a20: 0000 0000 063a 013a 017a 144d 7944 7261  .....:.:.z.MyDra
-00007a30: 7757 6964 6765 742e 6869 745f 626f 7863  wWidget.hit_boxc
-00007a40: 0200 0000 0000 0000 0000 0000 0b00 0000  ................
-00007a50: 0900 0000 4300 0000 734c 0400 0074 0064  ....C...sL...t.d
-00007a60: 0183 0101 007c 006a 01a0 027c 006a 037c  .....|.j...|.j.|
-00007a70: 006a 04a1 0201 0074 05a0 05a1 007c 006a  .j.....t.....|.j
-00007a80: 0618 007d 0274 05a0 05a1 007c 005f 067c  ...}.t.....|._.|
-00007a90: 01a0 07a1 0074 086a 096a 0a40 0072 4a64  .....t.j.j.@.rJd
-00007aa0: 027c 005f 0b6e 167c 01a0 07a1 0074 086a  .|._.n.|.....t.j
-00007ab0: 096a 0c40 0072 6064 037c 005f 0b7c 01a0  .j.@.r`d.|._.|..
-00007ac0: 0da1 00a0 0ea1 007c 01a0 0da1 00a0 0fa1  .......|........
-00007ad0: 0002 007d 037d 0474 107c 037c 006a 111b  ...}.}.t.|.|.j..
-00007ae0: 0083 017d 0374 107c 047c 006a 111b 0083  ...}.t.|.|.j....
-00007af0: 017d 047c 037c 005f 127c 047c 005f 137c  .}.|.|._.|.|._.|
-00007b00: 006a 147c 005f 157c 006a 167c 005f 1764  .j.|._.|.j.|._.d
-00007b10: 047d 0564 007c 005f 187c 006a 0344 005d  .}.d.|._.|.j.D.]
-00007b20: 587d 067c 006a 0b64 056b 0372 c27c 00a0  X}.|.j.d.k.r.|..
-00007b30: 197c 037c 047c 066a 1a6a 0e7c 066a 1a6a  .|.|.|.j.j.|.j.j
-00007b40: 1b17 007c 066a 1a6a 0f7c 066a 1a6a 1c17  ...|.j.j.|.j.j..
-00007b50: 0064 0618 0064 0764 08a1 0672 c264 097c  .d...d.d...r.d.|
-00007b60: 005f 0b7c 066a 1a7c 005f 1874 0064 0a7c  ._.|.j.|._.t.d.|
-00007b70: 066a 1d83 0201 0071 c27c 006a 0344 0090  .j.....q.|.j.D..
-00007b80: 035d 047d 067c 066a 1e90 0172 3664 0b7d  .].}.|.j...r6d.}
-00007b90: 076e 0464 0c7d 077c 006a 0b64 056b 0390  .n.d.}.|.j.d.k..
-00007ba0: 0172 227c 00a0 197c 037c 047c 066a 0e7c  .r"|...|.|.|.j.|
-00007bb0: 066a 0f7c 077c 07a1 0690 0172 2274 0064  .j.|.|.....r"t.d
-00007bc0: 0d7c 066a 1d83 0201 0064 0e7d 057c 006a  .|.j.....d.}.|.j
-00007bd0: 0b64 026b 0290 0172 9e7c 067c 005f 187c  .d.k...r.|.|._.|
-00007be0: 066a 0e7c 0318 007c 005f 1b7c 066a 0f7c  .j.|...|._.|.j.|
-00007bf0: 0418 007c 005f 1c90 0171 227c 006a 0b64  ...|._...q"|.j.d
-00007c00: 036b 0290 0272 3e7c 0264 0f6b 0090 0172  .k...r>|.d.k...r
-00007c10: da7c 006a 1f64 006b 0890 0172 c67c 067c  .|.j.d.k...r.|.|
-00007c20: 005f 1f7c 00a0 20a1 0001 0064 007c 005f  ._.|.. ....d.|._
-00007c30: 1f01 0064 0053 007c 006a 1f7c 066b 0290  ...d.S.|.j.|.k..
-00007c40: 0272 0064 007c 005f 1f74 0064 107c 0683  .r.d.|._.t.d.|..
-00007c50: 0201 007c 00a0 21a1 0001 006e 1074 0064  ...|..!....n.t.d
-00007c60: 117c 0683 0201 007c 067c 005f 1f7c 066a  .|.....|.|._.|.j
-00007c70: 1e90 0272 327c 006a 1f7c 066b 0290 0272  ...r2|.j.|.k...r
-00007c80: 327c 006a 01a0 227c 066a 1da1 0101 007c  2|.j.."|.j.....|
-00007c90: 00a0 21a1 0001 0090 0171 227c 006a 0b64  ..!......q"|.j.d
-00007ca0: 126b 0290 0272 8c74 0064 137c 0683 0201  .k...r.t.d.|....
-00007cb0: 007c 066a 1e90 0272 7074 0064 1483 0101  .|.j...rpt.d....
-00007cc0: 0074 237c 007c 0683 027d 086e 1274 0064  .t#|.|...}.n.t.d
-00007cd0: 1583 0101 0074 247c 007c 0683 027d 0864  .....t$|.|...}.d
-00007ce0: 037c 005f 0b90 0171 227c 006a 0b64 166b  .|._...q"|.j.d.k
-00007cf0: 0290 0372 9674 2564 1783 0182 0164 007c  ...r.t%d.....d.|
-00007d00: 005f 1864 007c 005f 2664 007c 005f 277c  ._.d.|._&d.|._'|
-00007d10: 066a 1e90 0372 047c 066a 2864 006b 0990  .j...r.|.j(d.k..
-00007d20: 0372 047c 006a 03a0 297c 066a 286a 2aa1  .r.|.j..)|.j(j*.
-00007d30: 0101 007c 006a 03a0 297c 066a 286a 2ba1  ...|.j..)|.j(j+.
-00007d40: 0101 007c 006a 04a0 297c 066a 28a1 0101  ...|.j..)|.j(...
-00007d50: 007c 00a0 21a1 0001 0064 027c 005f 0b6e  .|..!....d.|._.n
-00007d60: 907c 006a 0444 005d 627d 097c 096a 2c7c  .|.j.D.]b}.|.j,|
-00007d70: 066b 0290 0373 267c 096a 2d7c 066b 0290  .k...s&|.j-|.k..
-00007d80: 0372 0a7c 006a 04a0 297c 09a1 0101 007c  .r.|.j..)|.....|
-00007d90: 006a 03a0 297c 096a 2ca1 0101 007c 006a  .j..)|.j,....|.j
-00007da0: 03a0 297c 096a 2da1 0101 007c 006a 03a0  ..)|.j-....|.j..
-00007db0: 297c 096a 2aa1 0101 007c 006a 03a0 297c  )|.j*....|.j..)|
-00007dc0: 096a 2ba1 0101 0090 0371 0a7c 067c 006a  .j+......q.|.|.j
-00007dd0: 036b 0690 0372 867c 006a 03a0 297c 06a1  .k...r.|.j..)|..
-00007de0: 0101 007c 00a0 21a1 0001 0064 027c 005f  ...|..!....d.|._
-00007df0: 0b6e 907c 006a 0b64 186b 0290 0172 2264  .n.|.j.d.k...r"d
-00007e00: 007c 005f 187c 006a 2664 006b 0890 0372  .|._.|.j&d.k...r
-00007e10: c47c 067c 005f 267c 00a0 21a1 0001 006e  .|.|._&|..!....n
-00007e20: 627c 006a 2764 006b 0890 0172 227c 066a  b|.j'd.k...r"|.j
-00007e30: 1e90 0173 227c 067c 005f 2774 2e7c 006a  ...s"|.|._'t.|.j
-00007e40: 267c 006a 2783 027d 0a7c 006a 04a0 2f7c  &|.j'..}.|.j../|
-00007e50: 0aa1 0101 007c 006a 03a0 2f7c 0a6a 2aa1  .....|.j../|.j*.
-00007e60: 0101 007c 006a 03a0 2f7c 0a6a 2ba1 0101  ...|.j../|.j+...
-00007e70: 0064 007c 005f 2664 007c 005f 2764 027c  .d.|._&d.|._'d.|
-00007e80: 005f 0b90 0171 227c 0590 0473 487c 01a0  ._...q"|...sH|..
-00007e90: 07a1 0074 086a 096a 0c40 0090 0472 4864  ...t.j.j.@...rHd
-00007ea0: 057c 005f 0b64 0053 0029 194e 7a17 4d4f  .|._.d.S.).Nz.MO
-00007eb0: 5553 4520 5052 4553 5320 4452 4157 2057  USE PRESS DRAW W
-00007ec0: 4944 4745 54da 0464 7261 6772 b000 0000  IDGET..dragr....
-00007ed0: 4672 b200 0000 7296 0100 0072 3d01 0000  Fr....r....r=...
-00007ee0: 72d9 0000 00da 0a64 7261 675f 6c61 6265  r......drag_labe
-00007ef0: 6c72 b700 0000 72dd 0000 0072 ae00 0000  lr....r....r....
-00007f00: 7a07 626f 7820 6869 7454 679a 9999 9999  z.box hitTg.....
-00007f10: 99c9 3f5a 0b75 6e68 6967 686c 6967 6874  ..?Z.unhighlight
-00007f20: 5a09 6869 6768 6c69 6768 745a 0465 6469  Z.highlightZ.edi
-00007f30: 745a 0445 4449 547a 0e45 4449 5420 434f  tZ.EDITz.EDIT CO
-00007f40: 4e4e 4543 544f 527a 0a45 4449 5420 4147  NNECTORz.EDIT AG
-00007f50: 454e 54da 0664 656c 6574 657a 1944 656c  ENT..deletez.Del
-00007f60: 6574 6520 6d6f 6465 206e 6f74 2073 7570  ete mode not sup
-00007f70: 706f 7274 6564 728c 0000 0029 3072 1500  portedr....)0r..
-00007f80: 0000 7235 0000 00da 1475 7064 6174 655f  ..r5.....update_
-00007f90: 6772 6170 6869 6373 5f64 6174 6172 9600  graphics_datar..
-00007fa0: 0000 72b3 0000 0072 bb00 0000 72bc 0000  ..r....r....r...
-00007fb0: 00da 0762 7574 746f 6e73 7203 0000 0072  ...buttonsr....r
-00007fc0: 0700 0000 da0b 5269 6768 7442 7574 746f  ......RightButto
-00007fd0: 6e72 cd00 0000 da0a 4c65 6674 4275 7474  nr......LeftButt
-00007fe0: 6f6e 727c 0000 0072 1a00 0000 721b 0000  onr|...r....r...
-00007ff0: 0072 4000 0000 7234 0000 0072 c400 0000  .r@...r4...r....
-00008000: 72c5 0000 0072 3c00 0000 72c6 0000 0072  r....r<...r....r
-00008010: 3d00 0000 72c7 0000 0072 b700 0000 72b7  =...r....r....r.
-00008020: 0100 0072 6000 0000 7225 0000 0072 2600  ...r`...r%...r&.
-00008030: 0000 721c 0000 0072 6100 0000 72f2 0000  ..r....ra...r...
-00008040: 0072 9400 0000 72d2 0000 00da 1164 6174  .r....r......dat
-00008050: 615f 7365 6c65 6374 5f77 6865 7265 5a11  a_select_whereZ.
-00008060: 5472 616e 7361 6374 696f 6e45 6469 746f  TransactionEdito
-00008070: 725a 0b41 6765 6e74 4564 6974 6f72 da0c  rZ.AgentEditor..
-00008080: 5275 6e74 696d 6545 7272 6f72 72b8 0000  RuntimeErrorr...
-00008090: 0072 b900 0000 7263 0000 0072 ff00 0000  .r....rc...r....
-000080a0: 72a9 0000 0072 aa00 0000 724b 0000 0072  r....r....rK...r
-000080b0: 4c00 0000 72a2 0000 0072 0501 0000 290b  L...r....r....).
-000080c0: 7227 0000 0072 d500 0000 5a0a 7469 6d65  r'...r....Z.time
-000080d0: 5f64 656c 6179 721a 0000 0072 1b00 0000  _delayr....r....
-000080e0: 5a07 626f 785f 6869 7472 2300 0000 726e  Z.box_hitr#...rn
-000080f0: 0000 005a 0a6e 6577 5f65 6469 746f 7272  ...Z.new_editorr
-00008100: aa01 0000 da03 636f 6e72 2100 0000 7221  ......conr!...r!
-00008110: 0000 0072 2200 0000 da0f 6d6f 7573 6550  ...r".....mouseP
-00008120: 7265 7373 4576 656e 746b 0700 0073 be00  ressEventk...s..
-00008130: 0000 0001 0802 1202 0e01 0a03 1001 0802  ................
-00008140: 1001 0602 1a02 0e01 0e02 0601 0601 0801  ................
-00008150: 0803 0401 0603 0a02 3a01 0601 0801 0e03  ........:.......
-00008160: 0c01 0801 0602 0402 2601 0c03 0401 0c01  ........&.......
-00008170: 0601 0c01 1002 0c01 0a01 0c01 0601 0801  ................
-00008180: 0601 0602 0c01 0601 0a01 0a02 0a01 0604  ................
-00008190: 1401 0e02 0c02 0c01 0a02 0801 0801 0c03  ................
-000081a0: 0801 0a02 0a02 0c01 0801 0601 0601 0602  ................
-000081b0: 1401 1001 1001 0e01 0801 0804 0a01 1801  ................
-000081c0: 0c01 0e01 0e01 0e01 1202 0c01 0c02 0801  ................
-000081d0: 0803 0c01 0602 0c01 0601 0a02 1401 0602  ................
-000081e0: 0e01 0c01 0e01 0e02 0601 0601 0a02 1802  ................
-000081f0: 7a1c 4d79 4472 6177 5769 6467 6574 2e6d  z.MyDrawWidget.m
-00008200: 6f75 7365 5072 6573 7345 7665 6e74 6302  ousePressEventc.
-00008210: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-00008220: 0000 0043 0000 0073 b001 0000 7c01 a000  ...C...s....|...
-00008230: a100 a001 a100 7c01 a000 a100 a002 a100  ......|.........
-00008240: 0200 7d02 7d03 7403 7c02 7c00 6a04 1b00  ..}.}.t.|.|.j...
-00008250: 8301 7d02 7403 7c03 7c00 6a04 1b00 8301  ..}.t.|.|.j.....
-00008260: 7d03 7c02 7c00 5f05 7c03 7c00 5f06 7c00  }.|.|._.|.|._.|.
-00008270: 6a07 6401 6b02 7274 7c02 7c00 6a08 1800  j.d.k.rt|.|.j...
-00008280: 7d04 7c03 7c00 6a09 1800 7d05 7c04 7c00  }.|.|.j...}.|.|.
-00008290: 6a0a 5f0b 7c05 7c00 6a0a 5f0c 9001 6e30  j._.|.|.j._...n0
-000082a0: 7c00 6a07 6402 6b02 72c0 7c02 7d02 7c03  |.j.d.k.r.|.}.|.
-000082b0: 7d03 7c02 7c00 6a08 1800 7d04 7c03 7c00  }.|.|.j...}.|.|.
-000082c0: 6a09 1800 7d05 7c00 a00d 7c00 6a0e 7c04  j...}.|...|.j.|.
-000082d0: 1700 a101 7c00 5f0f 7c00 a00d 7c00 6a10  ....|._.|...|.j.
-000082e0: 7c05 1700 a101 7c00 5f11 6ee4 6403 7d06  |.....|._.n.d.}.
-000082f0: 7c00 6a12 4400 5dc6 7d07 7c07 6a13 72da  |.j.D.].}.|.j.r.
-00008300: 6404 7d08 6e04 6405 7d08 7c00 6a07 6402  d.}.n.d.}.|.j.d.
-00008310: 6b03 72ca 7c00 6a04 7c07 6a01 7c00 6a0f  k.r.|.j.|.j.|.j.
-00008320: 1700 1400 7c02 7c00 6a04 1400 0400 0300  ....|.|.j.......
-00008330: 6b00 9001 7224 7c00 6a04 7c07 6a01 7c00  k...r$|.j.|.j.|.
-00008340: 6a0f 1700 7c08 1700 1400 6b00 72ca 6e04  j...|.....k.r.n.
-00008350: 0100 71ca 7c00 6a04 7c07 6a02 7c00 6a11  ..q.|.j.|.j.|.j.
-00008360: 1700 1400 7c03 7c00 6a04 1400 0400 0300  ....|.|.j.......
-00008370: 6b00 9001 7264 7c00 6a04 7c07 6a02 7c08  k...rd|.j.|.j.|.
-00008380: 1700 7c00 6a11 1700 1400 6b00 72ca 6e04  ..|.j.....k.r.n.
-00008390: 0100 71ca 7c01 a014 a100 7415 6a16 6a17  ..q.|.....t.j.j.
-000083a0: 4000 9001 7280 6406 7c00 5f07 7c00 a018  @...r.d.|._.|...
-000083b0: 7416 6a19 a101 0100 6407 7d06 71ca 7c06  t.j.....d.}.q.|.
-000083c0: 9001 73a4 7c00 a018 7416 6a1a a101 0100  ..s.|...t.j.....
-000083d0: 7c00 a01b a100 0100 6400 5300 2908 4e72  |.......d.S.).Nr
-000083e0: b901 0000 72b2 0000 0046 72dd 0000 0072  ....r....Fr....r
-000083f0: ae00 0000 72b8 0100 0054 291c 727c 0000  ....r....T).r|..
-00008400: 0072 1a00 0000 721b 0000 0072 4000 0000  .r....r....r@...
-00008410: 7234 0000 0072 ca00 0000 72cb 0000 0072  r4...r....r....r
-00008420: cd00 0000 72c4 0000 0072 c500 0000 72b7  ....r....r....r.
-00008430: 0000 0072 2500 0000 7226 0000 0072 3f00  ...r%...r&...r?.
-00008440: 0000 72c6 0000 0072 3c00 0000 72c7 0000  ..r....r<...r...
-00008450: 0072 3d00 0000 7296 0000 0072 6100 0000  .r=...r....ra...
-00008460: 72bc 0100 0072 0300 0000 7207 0000 0072  r....r....r....r
-00008470: bd01 0000 da09 7365 7443 7572 736f 72da  ......setCursor.
-00008480: 0e4f 7065 6e48 616e 6443 7572 736f 72da  .OpenHandCursor.
-00008490: 0b41 7272 6f77 4375 7273 6f72 72d2 0000  .ArrowCursorr...
-000084a0: 0029 0972 2700 0000 72d5 0000 0072 1a00  .).r'...r....r..
-000084b0: 0000 721b 0000 0072 6600 0000 7267 0000  ..r....rf...rg..
-000084c0: 005a 0868 6f76 6572 696e 6772 2300 0000  .Z.hoveringr#...
-000084d0: 726e 0000 0072 2100 0000 7221 0000 0072  rn...r!...r!...r
-000084e0: 2200 0000 da0e 6d6f 7573 654d 6f76 6545  ".....mouseMoveE
-000084f0: 7665 6e74 fa07 0000 733c 0000 0000 021a  vent....s<......
-00008500: 020e 010e 0206 0106 020a 020a 010a 0208  ................
-00008510: 010c 020a 0104 0104 020a 010a 0312 0114  ................
-00008520: 0504 010a 0106 0106 0204 018a 0212 0106  ................
-00008530: 020c 0106 0206 010c 037a 1b4d 7944 7261  .........z.MyDra
-00008540: 7757 6964 6765 742e 6d6f 7573 654d 6f76  wWidget.mouseMov
-00008550: 6545 7665 6e74 6302 0000 0000 0000 0000  eEventc.........
-00008560: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-00008570: 3801 0000 7c00 6a00 7c00 5f01 7c00 6a02  8...|.j.|._.|.j.
-00008580: 7c00 5f03 7c00 6a00 7c00 5f04 7c00 6a02  |._.|.j.|._.|.j.
-00008590: 7c00 5f05 7c00 6a06 6401 6b02 726c 7c00  |._.|.j.d.k.rl|.
-000085a0: 6a07 6400 6b09 726c 7c00 6a07 0400 6a08  j.d.k.rl|.j...j.
-000085b0: 7c00 6a07 6a09 3700 0200 5f08 7c00 6a07  |.j.j.7..._.|.j.
-000085c0: 0400 6a0a 7c00 6a07 6a0b 3700 0200 5f0a  ..j.|.j.j.7..._.
-000085d0: 6402 7c00 6a07 5f09 6402 7c00 6a07 5f0b  d.|.j._.d.|.j._.
-000085e0: 7c00 6a06 6403 6b02 9001 722e 7c01 a00c  |.j.d.k...r.|...
-000085f0: a100 a008 a100 7c01 a00c a100 a00a a100  ......|.........
-00008600: 0200 7d02 7d03 7c00 6a0d 7d04 7c00 a00e  ..}.}.|.j.}.|...
-00008610: 740f 7c02 7c00 6a10 1b00 8301 7c04 a102  t.|.|.j.....|...
-00008620: 7d02 7c00 a00e 740f 7c03 7c00 6a10 1b00  }.|...t.|.|.j...
-00008630: 8301 7c04 a102 7d03 7c02 7c00 5f11 7c03  ..|...}.|.|._.|.
-00008640: 7c00 5f12 7c00 6a07 6400 6b09 9001 7226  |._.|.j.d.k...r&
-00008650: 7c00 a00e 7c00 6a11 7c00 6a09 1700 a101  |...|.j.|.j.....
-00008660: 7c00 6a07 5f08 7c00 a00e 7c00 6a12 7c00  |.j._.|...|.j.|.
-00008670: 6a0b 1700 a101 7c00 6a07 5f0a 7c00 6a07  j.....|.j._.|.j.
-00008680: 6a08 7c00 6a07 5f13 7c00 6a07 6a0a 7c00  j.|.j._.|.j.j.|.
-00008690: 6a07 5f14 6400 7c00 5f07 7c00 a015 a100  j._.d.|._.|.....
-000086a0: 0100 6404 7c00 5f06 6400 5300 2905 4e72  ..d.|._.d.S.).Nr
-000086b0: b901 0000 7201 0000 0072 b801 0000 72b0  ....r....r....r.
-000086c0: 0000 0029 1672 3c00 0000 72c6 0000 0072  ...).r<...r....r
-000086d0: 3d00 0000 72c7 0000 0072 c400 0000 72c5  =...r....r....r.
-000086e0: 0000 0072 cd00 0000 72b7 0000 0072 1a00  ...r....r....r..
-000086f0: 0000 7225 0000 0072 1b00 0000 7226 0000  ..r%...r....r&..
-00008700: 0072 7c00 0000 72ce 0000 0072 3f00 0000  .r|...r....r?...
-00008710: 7240 0000 0072 3400 0000 72ca 0000 0072  r@...r4...r....r
-00008720: cb00 0000 725e 0000 0072 5f00 0000 72d2  ....r^...r_...r.
-00008730: 0000 0029 0572 2700 0000 72d5 0000 0072  ...).r'...r....r
-00008740: 1a00 0000 721b 0000 0072 8c01 0000 7221  ....r....r....r!
-00008750: 0000 0072 2100 0000 7222 0000 00da 116d  ...r!...r".....m
-00008760: 6f75 7365 5265 6c65 6173 6545 7665 6e74  ouseReleaseEvent
-00008770: 2e08 0000 7332 0000 0000 0208 0108 0108  ....s2..........
-00008780: 0108 020a 020a 0114 0114 0208 0108 030c  ................
-00008790: 011a 0206 0116 0116 0206 0106 020c 0216  ................
-000087a0: 0116 010c 010c 0206 0108 027a 1e4d 7944  ...........z.MyD
-000087b0: 7261 7757 6964 6765 742e 6d6f 7573 6552  rawWidget.mouseR
-000087c0: 656c 6561 7365 4576 656e 7429 0172 a300  eleaseEvent).r..
-000087d0: 0000 2901 4629 0172 ae00 0000 2904 72d9  ..).F).r....).r.
-000087e0: 0000 0046 4672 6800 0000 2903 4654 5429  ...FFrh...).FTT)
-000087f0: 0172 6800 0000 2901 7212 0000 0029 2b72  .rh...).r....)+r
-00008800: 5300 0000 7254 0000 0072 5500 0000 7233  S...rT...rU...r3
-00008810: 0000 0072 2800 0000 72d3 0000 0072 8d00  ...r(...r....r..
-00008820: 0000 72d8 0000 0072 db00 0000 72bf 0000  ..r....r....r...
-00008830: 0072 be00 0000 728f 0000 0072 f100 0000  .r....r....r....
-00008840: 7257 0000 0072 f200 0000 7258 0000 0072  rW...r....rX...r
-00008850: f800 0000 72f9 0000 0072 fb00 0000 72fe  ....r....r....r.
-00008860: 0000 0072 9400 0000 7201 0100 0072 0301  ...r....r....r..
-00008870: 0000 7206 0100 0072 0701 0000 7208 0100  ..r....r....r...
-00008880: 0072 0b01 0000 7212 0100 0072 1401 0000  .r....r....r....
-00008890: 7215 0100 0072 2301 0000 7227 0100 0072  r....r#...r'...r
-000088a0: 3c01 0000 726d 0100 0072 8b01 0000 723f  <...rm...r....r?
-000088b0: 0000 0072 ec00 0000 72b2 0100 0072 b701  ...r....r....r..
-000088c0: 0000 72c2 0100 0072 c601 0000 72c7 0100  ..r....r....r...
-000088d0: 0072 5900 0000 7221 0000 0072 2100 0000  .rY...r!...r!...
-000088e0: 721f 0000 0072 2200 0000 7232 0000 0054  r....r"...r2...T
-000088f0: 0100 0073 5e00 0000 0802 0402 0c45 080a  ...s^........E..
-00008900: 0804 0809 080a 0809 0809 080d 0820 0201  ............. ..
-00008910: 0a03 0401 0a18 0808 0810 080d 0821 0804  .............!..
-00008920: 0812 080a 0814 0806 0807 0a1e 0a11 080e  ................
-00008930: 0826 0a1d 0811 0a64 0a7f 007f 0041 0878  .&.....d.....A.x
-00008940: 0a08 0a7f 007f 007f 007f 000c 0804 080a  ................
-00008950: 087f 0010 0834 7232 0000 0029 22da 0373  .....4r2...)"..s
-00008960: 7973 da05 5079 5174 3572 0200 0000 7203  ys..PyQt5r....r.
-00008970: 0000 00da 0b50 7951 7435 2e51 7447 7569  .....PyQt5.QtGui
-00008980: 7204 0000 0072 0500 0000 7206 0000 00da  r....r....r.....
-00008990: 0c50 7951 7435 2e51 7443 6f72 6572 0700  .PyQt5.QtCorer..
-000089a0: 0000 7208 0000 00da 1173 6369 7079 2e69  ..r......scipy.i
-000089b0: 6e74 6572 706f 6c61 7465 7209 0000 0072  nterpolater....r
-000089c0: bb00 0000 da0f 5079 5174 352e 5174 5769  ......PyQt5.QtWi
-000089d0: 6467 6574 7372 0a00 0000 720b 0000 0072  dgetsr....r....r
-000089e0: 0c00 0000 720d 0000 005a 1450 7951 7435  ....r....Z.PyQt5
-000089f0: 2e51 7450 7269 6e74 5375 7070 6f72 7472  .QtPrintSupportr
-00008a00: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-00008a10: 0000 0072 e400 0000 da05 6e75 6d70 7972  ...r......numpyr
-00008a20: 9a00 0000 da0c 6167 656e 745f 6564 6974  ......agent_edit
-00008a30: 6f72 7213 0000 0072 1400 0000 725a 0000  orr....r....rZ..
-00008a40: 0072 a200 0000 727e 0000 0072 3200 0000  .r....r~...r2...
-00008a50: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
-00008a60: 2200 0000 da08 3c6d 6f64 756c 653e 0100  ".....<module>..
-00008a70: 0000 7326 0000 0008 0110 0110 010c 0110  ..s&............
-00008a80: 010c 0108 0110 010c 010c 0110 0110 0208  ................
-00008a90: 0108 040c 030e 560e 7f00 3b0e 2e         ......V...;..
+00004eb0: 7410 6410 6401 7401 a008 8806 7c06 1800  t.d.d.t.....|...
+00004ec0: 6407 1300 8807 7c07 1800 6407 1300 1700  d.....|...d.....
+00004ed0: a101 1400 8302 8902 7410 6410 6401 7401  ........t.d.d.t.
+00004ee0: a008 7c06 7c08 1800 6407 1300 7c07 7c09  ..|.|...d...|.|.
+00004ef0: 1800 6407 1300 1700 a101 1400 8302 8903  ..d.............
+00004f00: 7401 a011 7c07 8807 1800 7c06 8806 1800  t...|.....|.....
+00004f10: a102 8905 8805 7401 a00e 6406 6407 7401  ......t...d.d.t.
+00004f20: 6a12 1400 6411 a103 1700 7d29 8700 8702  j...d.....})....
+00004f30: 8703 8705 8706 6605 6412 640a 8408 7c29  ......f.d.d...|)
+00004f40: 4400 8301 7d2a 8701 8702 8703 8705 8707  D...}*..........
+00004f50: 6605 6413 640a 8408 7c29 4400 8301 7d2b  f.d.d...|)D...}+
+00004f60: 7413 7414 7c2a 7c2b 8302 8301 7d28 9001  t.t.|*|+....}(..
+00004f70: 6e92 6414 7d25 7401 a00e 6406 6408 6415  n.d.}%t...d.d.d.
+00004f80: a103 7d26 740f 7c24 7c20 7c25 6406 640f  ..}&t.|$| |%d.d.
+00004f90: 8d04 7d27 7c27 7c26 8301 7d2c 7c20 6406  ..}'|'|&..},| d.
+00004fa0: 1900 6406 1900 8906 7c20 6406 1900 6408  ..d.....| d...d.
+00004fb0: 1900 8907 7c20 640d 1900 6406 1900 7d04  ....| d...d...}.
+00004fc0: 7c20 640d 1900 6408 1900 7d05 7c1e 9005  | d...d...}.|...
+00004fd0: 7376 8804 a015 8806 8807 7c06 7c07 6416  sv........|.|.d.
+00004fe0: a105 5c02 7d2d 7d2e 8804 a015 7c06 7c07  ..\.}-}.....|.|.
+00004ff0: 7c08 7c09 6416 a105 5c02 7d2f 7d30 8804  |.|.d...\.}/}0..
+00005000: a015 7c08 7c09 7c04 7c05 6416 a105 5c02  ..|.|.|.|.d...\.
+00005010: 7d31 7d32 7c2d 7c2f 1700 7c31 1700 7d2a  }1}2|-|/..|1..}*
+00005020: 7c2e 7c30 1700 7c32 1700 7d2b 6ec8 6401  |.|0..|2..}+n.d.
+00005030: 7c06 8806 1800 1400 8900 6401 7c07 8807  |.........d.|...
+00005040: 1800 1400 8901 7410 6410 6401 7401 a008  ......t.d.d.t...
+00005050: 8806 7c06 1800 6407 1300 8807 7c07 1800  ..|...d.....|...
+00005060: 6407 1300 1700 a101 1400 8302 8902 7410  d.............t.
+00005070: 6410 6401 7401 a008 7c06 7c08 1800 6407  d.d.t...|.|...d.
+00005080: 1300 7c07 7c09 1800 6407 1300 1700 a101  ..|.|...d.......
+00005090: 1400 8302 8903 7401 a011 7c07 8807 1800  ......t...|.....
+000050a0: 7c06 8806 1800 a102 8905 8805 7401 a00e  |...........t...
+000050b0: 6406 6407 7401 6a12 1400 6411 a103 1700  d.d.t.j...d.....
+000050c0: 7d29 8700 8702 8703 8705 8706 6605 6417  })..........f.d.
+000050d0: 640a 8408 7c29 4400 8301 7d2a 8701 8702  d...|)D...}*....
+000050e0: 8703 8705 8707 6605 6418 640a 8408 7c29  ......f.d.d...|)
+000050f0: 4400 8301 7d2b 7413 7414 7c2a 7c2b 8302  D...}+t.t.|*|+..
+00005100: 8301 7d28 7406 7c28 8301 7d33 6419 7d34  ..}(t.|(..}3d.}4
+00005110: 7c01 a016 7417 6a18 a101 0100 7419 8300  |...t.j.....t...
+00005120: 7d35 8804 6a1a 7c28 6406 1900 6406 1900  }5..j.|(d...d...
+00005130: 1400 7d36 8804 6a1a 7c28 6406 1900 6408  ..}6..j.|(d...d.
+00005140: 1900 1400 7d37 7c35 a01b 7c36 7c37 a102  ....}7|5..|6|7..
+00005150: 0100 7405 6408 741c 7c33 6407 1b00 8301  ..t.d.t.|3d.....
+00005160: 7c34 1800 8302 4400 5d2e 7d21 7c35 a01d  |4....D.].}!|5..
+00005170: 8804 6a1a 7c28 7c21 1900 6406 1900 1400  ..j.|(|!..d.....
+00005180: 8804 6a1a 7c28 7c21 1900 6408 1900 1400  ..j.|(|!..d.....
+00005190: a102 0100 9006 71b0 7405 741c 7c33 6407  ......q.t.t.|3d.
+000051a0: 1b00 8301 7c34 1800 7406 7c28 8301 8302  ....|4..t.|(....
+000051b0: 4400 5d2e 7d21 7c35 a01d 8804 6a1a 7c28  D.].}!|5....j.|(
+000051c0: 7c21 1900 6406 1900 1400 8804 6a1a 7c28  |!..d.......j.|(
+000051d0: 7c21 1900 6408 1900 1400 a102 0100 9006  |!..d...........
+000051e0: 71fa 7c35 a01b 7c36 7c37 a102 0100 7c35  q.|5..|6|7....|5
+000051f0: a01e a100 0100 7c01 a01f 7c35 a101 0100  ......|...|5....
+00005200: 741c 7c33 641a 1b00 8301 7d38 6403 7d39  t.|3d.....}8d.}9
+00005210: 7c1e 9007 7374 8804 6a20 7c01 7c28 7c38  |...st..j |.|(|8
+00005220: 7c0a 641b 8d04 5c02 7d22 7d23 7c0c 9007  |.d...\.}"}#|...
+00005230: 73bc 7c1e 9007 73bc 8804 6a21 6a22 a023  s.|...s...j!j".#
+00005240: a100 9007 72bc 7c39 9007 73bc 741c 7c33  ....r.|9..s.t.|3
+00005250: 641a 1b00 640e 1800 8301 7d38 8804 6a20  d...d.....}8..j 
+00005260: 7c01 7c28 7c38 6405 7c0a 641c 8d05 5c02  |.|(|8d.|.d...\.
+00005270: 7d22 7d23 5700 6e3a 0400 7424 6b0a 9007  }"}#W.n:..t$k...
+00005280: 72f8 0100 7d3a 0100 7a1a 7425 641d 7426  r...}:..z.t%d.t&
+00005290: 7c3a 8301 8302 0100 6406 7d22 6406 7d23  |:......d.}"d.}#
+000052a0: 5700 3500 641e 7d3a 7e3a 5800 5900 6e02  W.5.d.}:~:X.Y.n.
+000052b0: 5800 7c22 7c23 6602 5300 291f 7a2a 0a20  X.|"|#f.S.).z*. 
+000052c0: 2020 2020 2020 2064 7261 7773 2061 2063         draws a c
+000052d0: 7572 7665 6420 636f 6e6e 6563 746f 720a  urved connector.
+000052e0: 2020 2020 2020 2020 72a5 0000 00e9 1900          r.......
+000052f0: 0000 4667 7b14 ae47 e17a 943f 5472 0100  ..Fg{..G.z.?Tr..
+00005300: 0000 7230 0000 0072 1200 0000 6301 0000  ..r0...r....c...
+00005310: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00005320: 0013 0000 0073 2800 0000 6700 7c00 5d20  .....s(...g.|.] 
+00005330: 7d01 8800 a000 7c01 6400 1900 a101 8800  }.....|.d.......
+00005340: a000 7c01 6401 1900 a101 6602 9102 7104  ..|.d.....f...q.
+00005350: 5300 2902 7201 0000 0072 1200 0000 2901  S.).r....r....).
+00005360: 723f 0000 0029 0272 0d01 0000 da01 7472  r?...).r......tr
+00005370: 2b00 0000 7221 0000 0072 2200 0000 720e  +...r!...r"...r.
+00005380: 0100 0029 0400 0073 0400 0000 0600 0200  ...)...s........
+00005390: 7a31 4d79 4472 6177 5769 6467 6574 2e63  z1MyDrawWidget.c
+000053a0: 7572 7665 645f 636f 6e6e 6563 746f 722e  urved_connector.
+000053b0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000053c0: 6d70 3e29 0272 0100 0000 7201 0000 0029  mp>).r....r....)
+000053d0: 01da 0461 7869 7372 a400 0000 7204 0100  ...axisr....r...
+000053e0: 0029 02da 046b 696e 6472 3f01 0000 7228  .)...kindr?...r(
+000053f0: 0100 0072 9900 0000 6301 0000 0000 0000  ...r....c.......
+00005400: 0000 0000 0002 0000 0007 0000 0013 0000  ................
+00005410: 0073 4400 0000 6700 7c00 5d3c 7d01 8801  .sD...g.|.]<}...
+00005420: 7400 a001 7c01 a101 1400 7400 a001 8803  t...|.....t.....
+00005430: a101 1400 8802 7400 a002 7c01 a101 1400  ......t...|.....
+00005440: 7400 a002 8803 a101 1400 1800 8800 1700  t...............
+00005450: 8804 1700 9102 7104 5300 7221 0000 00a9  ......q.S.r!....
+00005460: 0372 9a00 0000 722a 0100 0072 2b01 0000  .r....r*...r+...
+00005470: a902 720d 0100 00da 0274 69a9 05da 0363  ..r......ti....c
+00005480: 3078 da02 7278 da02 7279 da02 7430 725e  0x..rx..ry..t0r^
+00005490: 0000 0072 2100 0000 7222 0000 0072 0e01  ...r!...r"...r..
+000054a0: 0000 4d04 0000 7304 0000 0006 0002 0063  ..M...s........c
+000054b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000054c0: 0700 0000 1300 0000 7344 0000 0067 007c  ........sD...g.|
+000054d0: 005d 3c7d 0188 0174 00a0 017c 01a1 0114  .]<}...t...|....
+000054e0: 0074 00a0 0288 03a1 0114 0088 0274 00a0  .t...........t..
+000054f0: 027c 01a1 0114 0074 00a0 0188 03a1 0114  .|.....t........
+00005500: 0017 0088 0017 0088 0417 0091 0271 0453  .............q.S
+00005510: 0072 2100 0000 7241 0100 0072 4201 0000  .r!...rA...rB...
+00005520: a905 da03 6330 7972 4601 0000 7247 0100  ....c0yrF...rG..
+00005530: 0072 4801 0000 725f 0000 0072 2100 0000  .rH...r_...r!...
+00005540: 7222 0000 0072 0e01 0000 4e04 0000 7304  r"...r....N...s.
+00005550: 0000 0006 0002 00da 066c 696e 6561 7272  .........linearr
+00005560: 6800 0000 e96f 0000 0063 0100 0000 0000  h....o...c......
+00005570: 0000 0000 0000 0200 0000 0700 0000 1300  ................
+00005580: 0000 7344 0000 0067 007c 005d 3c7d 0188  ..sD...g.|.]<}..
+00005590: 0174 00a0 017c 01a1 0114 0074 00a0 0188  .t...|.....t....
+000055a0: 03a1 0114 0088 0274 00a0 027c 01a1 0114  .......t...|....
+000055b0: 0074 00a0 0288 03a1 0114 0018 0088 0017  .t..............
+000055c0: 0088 0417 0091 0271 0453 0072 2100 0000  .......q.S.r!...
+000055d0: 7241 0100 0072 4201 0000 7244 0100 0072  rA...rB...rD...r
+000055e0: 2100 0000 7222 0000 0072 0e01 0000 7b04  !...r"...r....{.
+000055f0: 0000 7304 0000 0006 0002 0063 0100 0000  ..s........c....
+00005600: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00005610: 1300 0000 7344 0000 0067 007c 005d 3c7d  ....sD...g.|.]<}
+00005620: 0188 0174 00a0 017c 01a1 0114 0074 00a0  ...t...|.....t..
+00005630: 0288 03a1 0114 0088 0274 00a0 027c 01a1  .........t...|..
+00005640: 0114 0074 00a0 0188 03a1 0114 0017 0088  ...t............
+00005650: 0017 0088 0417 0091 0271 0453 0072 2100  .........q.S.r!.
+00005660: 0000 7241 0100 0072 4201 0000 7249 0100  ..rA...rB...rI..
+00005670: 0072 2100 0000 7222 0000 0072 0e01 0000  .r!...r"...r....
+00005680: 7c04 0000 7304 0000 0006 0002 00e9 1400  |...s...........
+00005690: 0000 7225 0100 0029 0172 3101 0000 2902  ..r%...).r1...).
+000056a0: 7230 0100 0072 3101 0000 7a1c 4572 726f  r0...r1...z.Erro
+000056b0: 7220 696e 204c 696e 6520 496e 7465 7270  r in Line Interp
+000056c0: 6f6c 6174 696f 6e3a 4e29 2772 1601 0000  olation:N)'r....
+000056d0: 729a 0000 00da 0561 7272 6179 da01 5472  r......array..Tr
+000056e0: 0501 0000 da05 7261 6e67 6572 0f01 0000  ......ranger....
+000056f0: da06 6375 6d73 756d da04 7371 7274 da03  ..cumsum..sqrt..
+00005700: 7375 6dda 0464 6966 66da 0669 6e73 6572  sum..diff..inser
+00005710: 7472 cf00 0000 72cc 0000 0072 1801 0000  tr....r....r....
+00005720: 7209 0000 0072 c200 0000 7229 0100 0072  r....r....r)...r
+00005730: 2601 0000 7217 0100 00da 037a 6970 7223  &...r......zipr#
+00005740: 0100 00da 0d73 6574 5265 6e64 6572 4869  .....setRenderHi
+00005750: 6e74 7204 0000 005a 0c41 6e74 6961 6c69  ntr....Z.Antiali
+00005760: 6173 696e 6772 0500 0000 7234 0000 005a  asingr....r4...Z
+00005770: 066d 6f76 6554 6f72 4000 0000 5a06 6c69  .moveTor@...Z.li
+00005780: 6e65 546f 5a0c 636c 6f73 6553 7562 7061  neToZ.closeSubpa
+00005790: 7468 5a08 6472 6177 5061 7468 723c 0100  thZ.drawPathr<..
+000057a0: 0072 3500 0000 722c 0100 0072 3700 0000  .r5...r,...r7...
+000057b0: 72e8 0000 0072 1500 0000 72e9 0000 0029  r....r....r....)
+000057c0: 3b72 2700 0000 7245 0000 0072 5e00 0000  ;r'...rE...r^...
+000057d0: 725f 0000 0072 1901 0000 721a 0100 00da  r_...r....r.....
+000057e0: 0278 69da 0279 69da 0278 64da 0279 6472  .xi..yi..xd..ydr
+000057f0: 3101 0000 da07 6973 5f66 6c6f 77da 0969  1.....is_flow..i
+00005800: 735f 756e 6964 6972 da03 7869 325a 0378  s_unidir..xi2Z.x
+00005810: 6933 5a03 7969 325a 0379 6933 729e 0000  i3Z.yi2Z.yi3r...
+00005820: 005a 0378 6934 5a03 7969 345a 0378 6935  .Z.xi4Z.yi4Z.xi5
+00005830: 5a03 7969 355a 0378 6936 5a03 7969 365a  Z.yi5Z.xi6Z.yi6Z
+00005840: 0378 6937 5a03 7969 375a 0478 6936 325a  .xi7Z.yi7Z.xi62Z
+00005850: 0479 6936 325a 0478 6933 355a 0479 6933  .yi62Z.xi35Z.yi3
+00005860: 355a 0c65 6e64 5f69 735f 7374 6172 745a  5Z.end_is_startZ
+00005870: 0770 6f69 6e74 7332 da06 706f 696e 7473  .points2..points
+00005880: da01 6972 3901 0000 723a 0100 00da 0864  ..ir9...r:.....d
+00005890: 6973 7461 6e63 65da 066d 6574 686f 64da  istance..method.
+000058a0: 0561 6c70 6861 da0c 696e 7465 7270 6f6c  .alpha..interpol
+000058b0: 6174 6f72 721e 0100 0072 3e01 0000 7221  atorr....r>...r!
+000058c0: 0100 0072 2201 0000 da02 6970 5a03 7863  ...r".....ipZ.xc
+000058d0: 315a 0379 6331 da03 7863 32da 0379 6332  1Z.yc1..xc2..yc2
+000058e0: da03 7863 33da 0379 6333 721b 0100 0072  ..xc3..yc3r....r
+000058f0: 2f01 0000 5a08 636f 6e6e 5061 7468 da06  /...Z.connPath..
+00005900: 7374 6172 7478 da06 7374 6172 7479 722e  startx..startyr.
+00005910: 0100 005a 0c64 7261 775f 7265 7665 7273  ...Z.draw_revers
+00005920: 6572 9700 0000 7221 0000 0029 0872 4501  er....r!...).rE.
+00005930: 0000 724a 0100 0072 4601 0000 7247 0100  ..rJ...rF...rG..
+00005940: 0072 2700 0000 7248 0100 0072 5e00 0000  .r'...rH...r^...
+00005950: 725f 0000 0072 2200 0000 da10 6375 7276  r_...r".....curv
+00005960: 6564 5f63 6f6e 6e65 6374 6f72 9603 0000  ed_connector....
+00005970: 7320 0100 0000 0c10 0110 0110 0110 0404  s ..............
+00005980: 0204 0104 0104 0104 0320 0108 0104 0108  ......... ......
+00005990: 0104 0320 0108 0104 0108 0104 0320 0108  ... ......... ..
+000059a0: 0104 0108 0104 0326 0108 0104 0108 0104  .......&........
+000059b0: 0204 0104 0104 0104 0326 0108 0104 0108  .........&......
+000059c0: 0104 0326 0108 0104 0108 0104 0326 0108  ...&.........&..
+000059d0: 0104 0108 0104 0326 0108 0104 0108 0104  .......&........
+000059e0: 070c 010c 0b0c 010c 1104 0124 0104 0110  ...........$....
+000059f0: 010c ff0a 0910 010c ff08 0304 010e 0212  ................
+00005a00: 011e 0102 0212 020a 0112 0208 0204 0128  ...............(
+00005a10: 0116 0508 0106 0206 010e 0310 010a 060c  ................
+00005a20: 010c 0228 0128 0214 0218 031a 011a 0212  ...(.(..........
+00005a30: 0404 010e 0410 0108 020c 010c 010c 010c  ................
+00005a40: 0406 0216 0116 0216 020c 010e 050c 010c  ................
+00005a50: 0228 0128 0214 0218 031a 011a 040e 0308  .(.(............
+00005a60: 0404 020c 0206 0112 0112 020c 021a 032c  ...............,
+00005a70: 021e 032c 020c 0208 010a 060c 0304 0206  ...,............
+00005a80: 0116 0206 0114 0106 0110 011c 0512 010e  ................
+00005a90: 0104 0116 1b7a 1d4d 7944 7261 7757 6964  .....z.MyDrawWid
+00005aa0: 6765 742e 6375 7276 6564 5f63 6f6e 6e65  get.curved_conne
+00005ab0: 6374 6f72 6302 0000 0000 0000 0000 0000  ctorc...........
+00005ac0: 0011 0000 0009 0000 0003 0000 0073 ee03  .............s..
+00005ad0: 0000 8808 6a00 6a01 a002 a100 7310 6400  ....j.j.....s.d.
+00005ae0: 5300 7403 a004 8808 6a00 6a05 a006 6401  S.t.....j.j...d.
+00005af0: a101 6402 a102 7d02 7c01 a007 7c02 a101  ..d...}.|...|...
+00005b00: 0100 6403 8909 6403 8903 6404 8900 6405  ..d...d...d...d.
+00005b10: 8904 6405 8905 7403 a008 7403 a009 6403  ..d...t...t...d.
+00005b20: 6403 6403 6406 a104 6402 a102 7d03 7c01  d.d.d...d...}.|.
+00005b30: a00a 740b a00c 8804 6407 1800 8805 6407  ..t.....d.....d.
+00005b40: 1800 8809 6405 1700 8803 6405 1700 a104  ....d.....d.....
+00005b50: 7c03 a102 0100 740d 8808 6a0e 8301 6408  |.....t...j...d.
+00005b60: 6b02 7296 6400 5300 740f 6408 8808 6a10  k.r.d.S.t.d...j.
+00005b70: 0b00 8302 7d04 7411 8808 6a12 8808 6a12  ....}.t...j...j.
+00005b80: 8808 6a10 1800 8302 7d05 740f 6408 8808  ..j.....}.t.d...
+00005b90: 6a13 0b00 8302 7d06 7411 8808 6a14 8808  j.....}.t...j...
+00005ba0: 6a14 8808 6a13 1800 8302 7d07 6700 7d08  j...j.....}.g.}.
+00005bb0: 6700 7d09 8808 6a0e 4400 5d1c 7d0a 7c08  g.}...j.D.].}.|.
+00005bc0: a015 7c0a 6a16 a101 0100 7c09 a015 7c0a  ..|.j.....|...|.
+00005bd0: 6a17 a101 0100 71e8 7411 7418 a011 7c08  j.....q.t.t...|.
+00005be0: a101 8808 6a10 0b00 8302 7d05 7411 7418  ....j.....}.t.t.
+00005bf0: a011 7c09 a101 8808 6a13 0b00 8302 7d07  ..|.....j.....}.
+00005c00: 740f 7418 a00f 7c08 a101 8808 6a10 0b00  t.t...|.....j...
+00005c10: 8302 7d04 740f 7418 a00f 7c09 a101 8808  ..}.t.t...|.....
+00005c20: 6a13 0b00 8302 7d06 7c05 7c04 6b02 9001  j.....}.|.|.k...
+00005c30: 7268 7c04 6405 1700 7d05 7c07 7c06 6b02  rh|.d...}.|.|.k.
+00005c40: 9001 727a 7c06 6405 1700 7d07 7c05 8808  ..rz|.d...}.|...
+00005c50: 6a12 6b00 9001 728c 8808 6a12 7d05 7c07  j.k...r...j.}.|.
+00005c60: 8808 6a14 6b00 9001 729e 8808 6a14 7d07  ..j.k...r...j.}.
+00005c70: 8708 6601 6409 640a 8408 7c08 4400 8301  ..f.d.d...|.D...
+00005c80: 7d08 8708 6601 640b 640a 8408 7c09 4400  }...f.d.d...|.D.
+00005c90: 8301 7d09 7c08 a015 8808 6a19 6405 1b00  ..}.|.....j.d...
+00005ca0: 8808 6a10 640c 8808 6a12 1400 1700 1400  ..j.d...j.......
+00005cb0: a101 0100 7c09 a015 8808 6a19 6405 1b00  ....|.....j.d...
+00005cc0: 8808 6a13 640c 8808 6a14 1400 1700 1400  ..j.d...j.......
+00005cd0: a101 0100 7c08 a015 640d 640c 8808 6a12  ....|...d.d...j.
+00005ce0: 1400 1400 a101 0100 7c09 a015 640d 640c  ........|...d.d.
+00005cf0: 8808 6a14 1400 1400 a101 0100 7418 a01a  ..j.........t...
+00005d00: 7c08 a101 8906 7418 a01a 7c09 a101 8907  |.....t...|.....
+00005d10: 8706 6601 640e 640a 8408 7c08 4400 8301  ..f.d.d...|.D...
+00005d20: 7d08 8707 6601 640f 640a 8408 7c09 4400  }...f.d.d...|.D.
+00005d30: 8301 7d09 7411 7418 a00f 7c08 a101 0b00  ..}.t.t...|.....
+00005d40: 7418 a011 7c08 a101 8302 8901 7411 7418  t...|.......t.t.
+00005d50: a00f 7c09 a101 0b00 7418 a011 7c09 a101  ..|.....t...|...
+00005d60: 8302 8902 8701 8709 6602 6410 640a 8408  ........f.d.d...
+00005d70: 7c08 4400 8301 7d08 8702 8703 6602 6411  |.D...}.....f.d.
+00005d80: 640a 8408 7c09 4400 8301 7d09 8709 6601  d...|.D...}...f.
+00005d90: 6412 640a 8408 7c08 4400 8301 7d08 8703  d.d...|.D...}...
+00005da0: 6601 6413 640a 8408 7c09 4400 8301 7d09  f.d.d...|.D...}.
+00005db0: 8700 8704 6602 6414 640a 8408 7c08 4400  ....f.d.d...|.D.
+00005dc0: 8301 7d08 8700 8705 6602 6415 640a 8408  ..}.....f.d.d...
+00005dd0: 7c09 4400 8301 7d09 741b 740d 7c08 8301  |.D...}.t.t.|...
+00005de0: 6401 1800 8301 4400 5d46 7d0b 7c08 7c0b  d.....D.]F}.|.|.
+00005df0: 1900 7d0c 7c09 7c0b 1900 7d0d 8808 6a0e  ..}.|.|...}...j.
+00005e00: 7c0b 1900 6a1c 9003 724a 7c01 a01d 7c0c  |...j...rJ|...|.
+00005e10: 7c0d 6402 6402 a104 0100 6e10 7c01 a01d  |.d.d.....n.|...
+00005e20: 7c0c 7c0d 6416 6416 a104 0100 9003 7116  |.|.d.d.......q.
+00005e30: 7c08 6417 1900 7d0c 7c09 6417 1900 7d0d  |.d...}.|.d...}.
+00005e40: 7403 a004 8808 6a00 6a05 a006 6416 a101  t.....j.j...d...
+00005e50: 6402 a102 7d02 7c01 a007 7c02 a101 0100  d...}.|...|.....
+00005e60: 7c0c 7d0e 7c0d 7d0f 6407 7d10 7c01 a01e  |.}.|.}.d.}.|...
+00005e70: 741f 7c0e 7c10 1800 8301 741f 7c0f 8301  t.|.|.....t.|...
+00005e80: 741f 7c0e 7c10 1700 8301 741f 7c0f 8301  t.|.|.....t.|...
+00005e90: a104 0100 7c01 a01e 741f 7c0e 8301 741f  ....|...t.|...t.
+00005ea0: 7c0f 7c10 1800 8301 741f 7c0e 8301 741f  |.|.....t.|...t.
+00005eb0: 7c0f 7c10 1700 8301 a104 0100 6400 5300  |.|.........d.S.
+00005ec0: 2918 4e72 3000 0000 7212 0000 00e9 5000  ).Nr0...r.....P.
+00005ed0: 0000 723d 0100 0072 dd00 0000 7299 0000  ..r=...r....r...
+00005ee0: 0072 6800 0000 7201 0000 0063 0100 0000  .rh...r....c....
+00005ef0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00005f00: 1300 0000 7320 0000 0067 007c 005d 187d  ....s ...g.|.].}
+00005f10: 0188 006a 007c 0188 006a 0117 0014 0064  ...j.|...j.....d
+00005f20: 001b 0091 0271 0453 00a9 0172 dd00 0000  .....q.S...r....
+00005f30: 2902 7234 0000 0072 3c00 0000 2902 720d  ).r4...r<...).r.
+00005f40: 0100 0072 5801 0000 722b 0000 0072 2100  ...rX...r+...r!.
+00005f50: 0000 7222 0000 0072 0e01 0000 0905 0000  ..r"...r........
+00005f60: 7304 0000 0006 0002 007a 2b4d 7944 7261  s........z+MyDra
+00005f70: 7757 6964 6765 742e 6461 7750 7265 7669  wWidget.dawPrevi
+00005f80: 6577 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ew.<locals>.<lis
+00005f90: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+00005fa0: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
+00005fb0: 2000 0000 6700 7c00 5d18 7d01 8800 6a00   ...g.|.].}...j.
+00005fc0: 7c01 8800 6a01 1700 1400 6400 1b00 9102  |...j.....d.....
+00005fd0: 7104 5300 726e 0100 0029 0272 3400 0000  q.S.rn...).r4...
+00005fe0: 723d 0000 0029 0272 0d01 0000 7259 0100  r=...).r....rY..
+00005ff0: 0072 2b00 0000 7221 0000 0072 2200 0000  .r+...r!...r"...
+00006000: 720e 0100 000a 0500 0073 0400 0000 0600  r........s......
+00006010: 0200 72a5 0000 0072 3100 0000 6301 0000  ..r....r1...c...
+00006020: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00006030: 0013 0000 0073 1400 0000 6700 7c00 5d0c  .....s....g.|.].
+00006040: 7d01 7c01 8800 1800 9102 7104 5300 7221  }.|.......q.S.r!
+00006050: 0000 0072 2100 0000 a902 720d 0100 0072  ...r!.....r....r
+00006060: 1a00 0000 2901 da02 6d78 7221 0000 0072  ....)...mxr!...r
+00006070: 2200 0000 720e 0100 0017 0500 0073 0400  "...r........s..
+00006080: 0000 0600 0200 6301 0000 0000 0000 0000  ......c.........
+00006090: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
+000060a0: 1400 0000 6700 7c00 5d0c 7d01 7c01 8800  ....g.|.].}.|...
+000060b0: 1800 9102 7104 5300 7221 0000 0072 2100  ....q.S.r!...r!.
+000060c0: 0000 a902 720d 0100 0072 1b00 0000 2901  ....r....r....).
+000060d0: da02 6d79 7221 0000 0072 2200 0000 720e  ..myr!...r"...r.
+000060e0: 0100 0018 0500 0073 0400 0000 0600 0200  .......s........
+000060f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00006100: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
+00006110: 7c00 5d14 7d01 6400 8801 1400 7c01 1400  |.].}.d.....|...
+00006120: 8800 1b00 9102 7104 5300 a901 72a5 0000  ......q.S...r...
+00006130: 0072 2100 0000 726f 0100 0029 0272 6600  .r!...ro...).rf.
+00006140: 0000 da07 775f 6672 616d 6572 2100 0000  ....w_framer!...
+00006150: 7222 0000 0072 0e01 0000 1d05 0000 7304  r"...r........s.
+00006160: 0000 0006 0002 0063 0100 0000 0000 0000  .......c........
+00006170: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00006180: 731c 0000 0067 007c 005d 147d 0164 0088  s....g.|.].}.d..
+00006190: 0114 007c 0114 0088 001b 0091 0271 0453  ...|.........q.S
+000061a0: 0072 7301 0000 7221 0000 0072 7101 0000  .rs...r!...rq...
+000061b0: 2902 7267 0000 00da 0768 5f66 7261 6d65  ).rg.....h_frame
+000061c0: 7221 0000 0072 2200 0000 720e 0100 001e  r!...r"...r.....
+000061d0: 0500 0073 0400 0000 0600 0200 6301 0000  ...s........c...
+000061e0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000061f0: 0013 0000 0073 1800 0000 6700 7c00 5d10  .....s....g.|.].
+00006200: 7d01 7c01 6400 8800 1400 1700 9102 7104  }.|.d.........q.
+00006210: 5300 7273 0100 0072 2100 0000 726f 0100  S.rs...r!...ro..
+00006220: 0029 0172 7401 0000 7221 0000 0072 2200  .).rt...r!...r".
+00006230: 0000 720e 0100 0020 0500 0073 0400 0000  ..r.... ...s....
+00006240: 0600 0200 6301 0000 0000 0000 0000 0000  ....c...........
+00006250: 0002 0000 0005 0000 0013 0000 0073 1800  .............s..
+00006260: 0000 6700 7c00 5d10 7d01 7c01 6400 8800  ..g.|.].}.|.d...
+00006270: 1400 1700 9102 7104 5300 7273 0100 0072  ......q.S.rs...r
+00006280: 2100 0000 7271 0100 0029 0172 7501 0000  !...rq...).ru...
+00006290: 7221 0000 0072 2200 0000 720e 0100 0021  r!...r"...r....!
+000062a0: 0500 0073 0400 0000 0600 0200 6301 0000  ...s........c...
+000062b0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+000062c0: 0013 0000 0073 2800 0000 6700 7c00 5d20  .....s(...g.|.] 
+000062d0: 7d01 8801 7400 8800 6400 1b00 8301 1700  }...t...d.......
+000062e0: 7c01 1700 6400 1800 6401 1800 9102 7104  |...d...d.....q.
+000062f0: 5300 a902 7230 0000 0072 dd00 0000 a901  S...r0...r......
+00006300: 7240 0000 0072 6f01 0000 2902 7261 0100  r@...ro...).ra..
+00006310: 00da 066d 6f76 655f 7872 2100 0000 7222  ...move_xr!...r"
+00006320: 0000 0072 0e01 0000 2305 0000 7304 0000  ...r....#...s...
+00006330: 0006 0002 0063 0100 0000 0000 0000 0000  .....c..........
+00006340: 0000 0200 0000 0600 0000 1300 0000 7328  ..............s(
+00006350: 0000 0067 007c 005d 207d 0188 0174 0088  ...g.|.] }...t..
+00006360: 0064 001b 0083 0117 007c 0117 0064 0018  .d.......|...d..
+00006370: 0064 0118 0091 0271 0453 0072 7601 0000  .d.....q.S.rv...
+00006380: 7277 0100 0072 7101 0000 2902 7261 0100  rw...rq...).ra..
+00006390: 00da 066d 6f76 655f 7972 2100 0000 7222  ...move_yr!...r"
+000063a0: 0000 0072 0e01 0000 2405 0000 7304 0000  ...r....$...s...
+000063b0: 0006 0002 0072 6900 0000 72a4 0000 0029  .....ri...r....)
+000063c0: 2072 3500 0000 da0a 6368 6563 6b42 6f78   r5.....checkBox
+000063d0: 5f39 7237 0000 0072 0600 0000 da04 5150  _9r7...r......QP
+000063e0: 656e 7288 0000 00da 0967 6574 5f63 6f6c  enr......get_col
+000063f0: 6f72 da06 7365 7450 656e da06 5142 7275  or..setPen..QBru
+00006400: 7368 da06 5143 6f6c 6f72 7243 0000 0072  sh..QColorrC...r
+00006410: 0300 0000 7241 0000 0072 0f01 0000 7296  ....rA...r....r.
+00006420: 0000 00da 036d 696e 723c 0000 0072 c200  .....minr<...r..
+00006430: 0000 729e 0000 0072 3d00 0000 729f 0000  ..r....r=...r...
+00006440: 0072 0501 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00006450: 729a 0000 0072 3400 0000 da04 6d65 616e  r....r4.....mean
+00006460: 7250 0100 0072 6100 0000 da08 6472 6177  rP...ra.....draw
+00006470: 5265 6374 722d 0100 0072 4000 0000 2911  Rectr-...r@...).
+00006480: 7227 0000 0072 4500 0000 da03 7065 6e72  r'...rE.....penr
+00006490: 4600 0000 da05 785f 6d69 6eda 0578 5f6d  F.....x_min..x_m
+000064a0: 6178 da05 795f 6d69 6eda 0579 5f6d 6178  ax..y_min..y_max
+000064b0: 5a06 785f 7661 6c73 5a06 795f 7661 6c73  Z.x_valsZ.y_vals
+000064c0: 7223 0000 0072 6001 0000 721a 0000 0072  r#...r`...r....r
+000064d0: 1b00 0000 da02 6f78 da02 6f79 72aa 0000  ......ox..oyr...
+000064e0: 0072 2100 0000 290a 7261 0100 0072 6600  .r!...).ra...rf.
+000064f0: 0000 7267 0000 0072 7501 0000 7278 0100  ..rg...ru...rx..
+00006500: 0072 7901 0000 7270 0100 0072 7201 0000  .ry...rp...rr...
+00006510: 7227 0000 0072 7401 0000 7222 0000 00da  r'...rt...r"....
+00006520: 0a64 6177 5072 6576 6965 77d5 0400 0073  .dawPreview....s
+00006530: 8600 0000 0003 0c01 0402 1601 0a06 0401  ................
+00006540: 0401 0401 0401 0402 1801 2802 0e01 0402  ..........(.....
+00006550: 0e01 1401 0e01 1401 0401 0402 0a01 0c01  ................
+00006560: 0e03 1401 1401 1401 1402 0a01 0801 0a01  ................
+00006570: 0802 0c01 0601 0c01 0602 1201 1203 2001  .............. .
+00006580: 2003 1401 1402 0a01 0a02 1201 1202 1801   ...............
+00006590: 1802 1401 1402 1201 1202 1401 1404 1401  ................
+000065a0: 0801 0801 0e01 1209 1403 0801 0801 1601  ................
+000065b0: 0a01 0401 0401 0401 2801 7a17 4d79 4472  ........(.z.MyDr
+000065c0: 6177 5769 6467 6574 2e64 6177 5072 6576  awWidget.dawPrev
+000065d0: 6965 7763 0300 0000 0000 0000 0000 0000  iewc............
+000065e0: 0500 0000 0300 0000 4300 0000 7332 0000  ........C...s2..
+000065f0: 007c 006a 0072 2a74 017c 027c 006a 0283  .|.j.r*t.|.|.j..
+00006600: 027d 0374 037c 017c 031b 0083 017c 0314  .}.t.|.|.....|..
+00006610: 007d 0474 037c 0483 0153 0074 037c 0183  .}.t.|...S.t.|..
+00006620: 0153 0072 2900 0000 2904 72cf 0000 0072  .S.r)...).r....r
+00006630: 8001 0000 72ce 0000 0072 4000 0000 2905  ....r....r@...).
+00006640: 7227 0000 0072 1a00 0000 721b 0100 00da  r'...r....r.....
+00006650: 016d 5a0a 785f 7261 7374 6572 6564 7221  .mZ.x_rasteredr!
+00006660: 0000 0072 2100 0000 7222 0000 0072 3f00  ...r!...r"...r?.
+00006670: 0000 4d05 0000 730a 0000 0000 0106 020c  ..M...s.........
+00006680: 0110 0108 017a 134d 7944 7261 7757 6964  .....z.MyDrawWid
+00006690: 6765 742e 7261 7374 6572 7212 0000 0063  get.rasterr....c
+000066a0: 0300 0000 0000 0000 0000 0000 2300 0000  ............#...
+000066b0: 0e00 0000 4300 0000 736c 0b00 0074 00a0  ....C...sl...t..
+000066c0: 017c 01a1 017d 037c 03a0 027c 027c 02a1  .|...}.|...|.|..
+000066d0: 0201 007c 03a0 0374 006a 016a 04a1 0101  ...|...t.j.j....
+000066e0: 007c 03a0 0374 006a 016a 05a1 0101 0074  .|...t.j.j.....t
+000066f0: 00a0 067c 006a 076a 08a0 0964 01a1 0164  ...|.j.j...d...d
+00006700: 02a1 027d 047c 03a0 0a7c 04a1 0101 007c  ...}.|...|.....|
+00006710: 006a 076a 0ba0 0ca1 0072 d474 00a0 0d74  .j.j.....r.t...t
+00006720: 00a0 0e64 0364 0364 0364 03a1 0464 02a1  ...d.d.d.d...d..
+00006730: 027d 057c 03a0 0f74 10a0 1174 10a0 1264  .}.|...t...t...d
+00006740: 0464 04a1 0274 10a0 1274 137c 006a 1464  .d...t...t.|.j.d
+00006750: 0118 0083 0174 137c 006a 1564 0118 0083  .....t.|.j.d....
+00006760: 01a1 02a1 027c 05a1 0201 007c 017c 006b  .....|.....|.|.k
+00006770: 0272 f87c 03a0 1664 0464 047c 006a 1464  .r.|...d.d.|.j.d
+00006780: 0118 007c 006a 1564 0518 00a1 0401 006e  ...|.j.d.......n
+00006790: 247c 017c 006b 0272 f87c 03a0 1664 0464  $|.|.k.r.|...d.d
+000067a0: 047c 006a 1464 0118 007c 006a 1564 0518  .|.j.d...|.j.d..
+000067b0: 00a1 0401 007c 03a0 0a7c 04a1 0101 0074  .....|...|.....t
+000067c0: 1764 0664 0784 007c 006a 076a 18a0 19a1  .d.d...|.j.j....
+000067d0: 0044 0083 0183 017d 0667 007d 0767 007d  .D.....}.g.}.g.}
+000067e0: 087c 006a 1a44 005d 9c7d 0974 1b7c 0683  .|.j.D.].}.t.|..
+000067f0: 0164 046b 027d 0a74 1b7c 0683 0164 046b  .d.k.}.t.|...d.k
+00006800: 0390 016f 6074 1b74 1c74 177c 096a 1d83  ...o`t.t.t.|.j..
+00006810: 017c 0640 0083 0183 0164 046b 047d 0b7c  .|.@.....d.k.}.|
+00006820: 0a90 0173 6e7c 0b90 0172 2a7c 097c 086b  ...sn|...r*|.|.k
+00006830: 0790 0172 2a7c 006a 1e64 006b 0890 0172  ...r*|.j.d.k...r
+00006840: 907c 08a0 1f7c 09a1 0101 006e 347c 096a  .|...|.....n4|.j
+00006850: 207c 006a 1e6b 0290 0173 ba7c 096a 217c   |.j.k...s.|.j!|
+00006860: 006a 1e6b 0290 0173 ba7c 096a 227c 006a  .j.k...s.|.j"|.j
+00006870: 1e6b 0290 0172 2a7c 08a0 1f7c 09a1 0101  .k...r*|...|....
+00006880: 0090 0171 2a7c 006a 1a44 0090 055d f07d  ...q*|.j.D...].}
+00006890: 0964 087d 0c64 097d 0d7c 096a 227c 006a  .d.}.d.}.|.j"|.j
+000068a0: 1e6b 0290 0272 4c74 00a0 067c 006a 076a  .k...rLt...|.j.j
+000068b0: 08a0 0964 05a1 0164 0aa1 027d 0464 087d  ...d...d...}.d.}
+000068c0: 0c74 237c 006a 076a 2483 0144 005d 385c  .t#|.j.j$..D.]8\
+000068d0: 027d 0e7d 0f7c 0f64 0b19 007c 096a 226a  .}.}.|.d...|.j"j
+000068e0: 256b 0290 0272 1074 267c 0f64 0c19 0083  %k...r.t&|.d....
+000068f0: 0164 0d6b 0290 0272 4064 097d 0c01 0090  .d.k...r@d.}....
+00006900: 0371 4890 0271 106e fc74 00a0 067c 006a  .qH..q.n.t...|.j
+00006910: 076a 08a0 0964 01a1 0164 0ea1 027d 047c  .j...d...d...}.|
+00006920: 097c 086b 0690 0372 1c64 097d 0d64 087d  .|.k...r.d.}.d.}
+00006930: 0c74 237c 006a 076a 2483 0144 005d 4e5c  .t#|.j.j$..D.]N\
+00006940: 027d 0e7d 0f7c 0f64 0b19 007c 096a 226a  .}.}.|.d...|.j"j
+00006950: 256b 0290 0272 8074 267c 0f64 0f19 0083  %k...r.t&|.d....
+00006960: 0164 106b 0290 0272 b064 087d 0d74 267c  .d.k...r.d.}.t&|
+00006970: 0f64 0c19 0083 0164 0d6b 0290 0272 c664  .d.....d.k...r.d
+00006980: 097d 0c01 0090 0271 d090 0271 807c 0d90  .}.....q...q.|..
+00006990: 0272 ee74 00a0 067c 006a 076a 08a0 0964  .r.t...|.j.j...d
+000069a0: 01a1 0164 0ea1 027d 046e 1674 00a0 067c  ...d...}.n.t...|
+000069b0: 006a 076a 08a0 0964 05a1 0164 0ea1 027d  .j.j...d...d...}
+000069c0: 047c 04a0 2774 286a 29a1 0101 007c 04a0  .|..'t(j)....|..
+000069d0: 2a64 0ea1 0101 006e 2c7c 04a0 2774 286a  *d.....n,|..'t(j
+000069e0: 2ba1 0101 007c 04a0 2c64 0264 0567 02a1  +....|..,d.d.g..
+000069f0: 0101 007c 04a0 2a64 11a1 0101 0064 097d  ...|..*d.....d.}
+00006a00: 0d64 087d 0c7c 03a0 0a7c 04a1 0101 0064  .d.}.|...|.....d
+00006a10: 087d 1064 127d 117c 097c 086b 0690 0772  .}.d.}.|.|.k...r
+00006a20: 0a7c 006a 2d7c 037c 006a 2e74 137c 096a  .|.j-|.|.j.t.|.j
+00006a30: 206a 2f7c 1117 0083 0117 007c 006a 3074   j/|.......|.j0t
+00006a40: 137c 096a 206a 317c 1117 0083 0117 007c  .|.j j1|.......|
+00006a50: 006a 2e74 137c 096a 216a 2f7c 1117 0083  .j.t.|.j!j/|....
+00006a60: 0117 007c 006a 3074 137c 096a 216a 317c  ...|.j0t.|.j!j1|
+00006a70: 1117 0083 0117 007c 006a 2e74 137c 096a  .......|.j.t.|.j
+00006a80: 226a 2f64 1317 0083 0117 007c 006a 3074  "j/d.......|.j0t
+00006a90: 137c 096a 226a 3164 1317 0083 0117 007c  .|.j"j1d.......|
+00006aa0: 006a 2e74 137c 096a 326a 2f64 1317 0083  .j.t.|.j2j/d....
+00006ab0: 0117 007c 006a 3074 137c 096a 326a 3164  ...|.j0t.|.j2j1d
+00006ac0: 1317 0083 0117 007c 0d7c 0c64 148d 0b5c  .......|.|.d...\
+00006ad0: 027d 127d 137c 096a 207c 076b 0790 0472  .}.}.|.j |.k...r
+00006ae0: 307c 07a0 1f7c 096a 20a1 0101 007c 096a  0|...|.j ....|.j
+00006af0: 217c 076b 0790 0472 487c 07a0 1f7c 096a  !|.k...rH|...|.j
+00006b00: 21a1 0101 007c 096a 227c 076b 0790 0472  !....|.j"|.k...r
+00006b10: 607c 07a0 1f7c 096a 22a1 0101 007c 096a  `|...|.j"....|.j
+00006b20: 327c 076b 0790 0472 787c 07a0 1f7c 096a  2|.k...rx|...|.j
+00006b30: 32a1 0101 007c 096a 227c 006a 1e6b 0290  2....|.j"|.j.k..
+00006b40: 0472 a874 00a0 067c 006a 076a 08a0 0964  .r.t...|.j.j...d
+00006b50: 15a1 0164 0ea1 027d 047c 03a0 0a7c 04a1  ...d...}.|...|..
+00006b60: 0101 006e 2074 00a0 067c 006a 076a 08a0  ...n t...|.j.j..
+00006b70: 0964 02a1 0164 0ea1 027d 047c 03a0 0a7c  .d...d...}.|...|
+00006b80: 04a1 0101 007c 006a 076a 33a0 0ca1 0090  .....|.j.j3.....
+00006b90: 0572 8e7c 006a 076a 34a0 0ca1 0090 0772  .r.|.j.j4......r
+00006ba0: 087c 006a 1e7c 096a 226b 0290 0572 0a74  .|.j.|.j"k...r.t
+00006bb0: 00a0 0d7c 006a 076a 08a0 0964 05a1 0164  ...|.j.j...d...d
+00006bc0: 02a1 027d 146e 1674 00a0 0d7c 006a 076a  ...}.n.t...|.j.j
+00006bd0: 08a0 0964 16a1 0164 02a1 027d 1464 177d  ...d...d...}.d.}
+00006be0: 157a 2474 137c 006a 076a 35a0 36a1 0083  .z$t.|.j.j5.6...
+00006bf0: 017d 157c 03a0 3774 3864 187c 1583 02a1  .}.|..7t8d.|....
+00006c00: 0101 0057 006e 3004 0074 396b 0a90 0572  ...W.n0..t9k...r
+00006c10: 7801 007d 1601 007a 1074 3a74 267c 1683  x..}...z.t:t&|..
+00006c20: 0183 0101 0057 0035 0064 007d 167e 1658  .....W.5.d.}.~.X
+00006c30: 0059 006e 0258 007c 096a 226a 3ba0 3c7c  .Y.n.X.|.j"j;.<|
+00006c40: 037c 14a1 0201 0090 0771 be7c 006a 076a  .|.......q.|.j.j
+00006c50: 34a0 0ca1 0090 0772 be7c 006a 1e7c 096a  4......r.|.j.|.j
+00006c60: 226b 0290 0572 c274 00a0 0d7c 006a 076a  "k...r.t...|.j.j
+00006c70: 08a0 0964 05a1 0164 02a1 027d 146e 1674  ...d...d...}.n.t
+00006c80: 00a0 0d7c 006a 076a 08a0 0964 16a1 0164  ...|.j.j...d...d
+00006c90: 02a1 027d 147c 096a 206a 2f7c 096a 216a  ...}.|.j j/|.j!j
+00006ca0: 2f6b 0390 0672 2e7c 096a 206a 317c 096a  /k...r.|.j j1|.j
+00006cb0: 216a 316b 0390 0672 2e7c 006a 3d7c 1214  !j1k...r.|.j=|..
+00006cc0: 007d 177c 006a 3d7c 1314 007d 187c 006a  .}.|.j=|...}.|.j
+00006cd0: 3d7c 1264 1317 0014 007d 197c 006a 3d7c  =|.d.....}.|.j=|
+00006ce0: 1364 1317 0014 007d 1a6e 687c 006a 3d7c  .d.....}.nh|.j=|
+00006cf0: 006a 2e7c 096a 226a 2f17 0014 007d 177c  .j.|.j"j/....}.|
+00006d00: 006a 3d7c 006a 307c 096a 226a 3117 0014  .j=|.j0|.j"j1...
+00006d10: 007d 187c 006a 3d7c 006a 2e7c 096a 326a  .}.|.j=|.j.|.j2j
+00006d20: 3b6a 2f17 007c 096a 326a 3b6a 3e17 0014  ;j/..|.j2j;j>...
+00006d30: 007d 197c 006a 3d7c 006a 307c 096a 326a  .}.|.j=|.j0|.j2j
+00006d40: 3b6a 3117 007c 096a 326a 3b6a 3f17 0014  ;j1..|.j2j;j?...
+00006d50: 007d 1a64 177d 157a 2474 137c 006a 076a  .}.d.}.z$t.|.j.j
+00006d60: 35a0 36a1 0083 017d 157c 03a0 3774 3864  5.6....}.|..7t8d
+00006d70: 187c 1583 02a1 0101 0057 006e 3004 0074  .|.......W.n0..t
+00006d80: 396b 0a90 0672 ee01 007d 1601 007a 1074  9k...r...}...z.t
+00006d90: 3a74 267c 1683 0183 0101 0057 0035 0064  :t&|.......W.5.d
+00006da0: 007d 167e 1658 0059 006e 0258 007c 096a  .}.~.X.Y.n.X.|.j
+00006db0: 226a 3b6a 3c7c 037c 147c 197c 1a66 0264  "j;j<|.|.|.|.f.d
+00006dc0: 198d 0301 006e b47c 006a 2d7c 037c 006a  .....n.|.j-|.|.j
+00006dd0: 2e74 137c 096a 206a 2f7c 1117 0083 0117  .t.|.j j/|......
+00006de0: 007c 006a 3074 137c 096a 206a 317c 1117  .|.j0t.|.j j1|..
+00006df0: 0083 0117 007c 006a 2e74 137c 096a 216a  .....|.j.t.|.j!j
+00006e00: 2f7c 1117 0083 0117 007c 006a 3074 137c  /|.......|.j0t.|
+00006e10: 096a 216a 317c 1117 0083 0117 007c 006a  .j!j1|.......|.j
+00006e20: 2e74 137c 096a 226a 2f64 1317 0083 0117  .t.|.j"j/d......
+00006e30: 007c 006a 3074 137c 096a 226a 3164 1317  .|.j0t.|.j"j1d..
+00006e40: 0083 0117 007c 006a 2e74 137c 096a 326a  .....|.j.t.|.j2j
+00006e50: 2f64 1317 0083 0117 007c 006a 3074 137c  /d.......|.j0t.|
+00006e60: 096a 326a 3164 1317 0083 0117 007c 0d7c  .j2j1d.......|.|
+00006e70: 0c64 148d 0b5c 027d 127d 1390 0171 ce74  .d...\.}.}...q.t
+00006e80: 00a0 067c 006a 076a 08a0 0964 01a1 0164  ...|.j.j...d...d
+00006e90: 02a1 027d 047c 04a0 2774 286a 29a1 0101  ...}.|..'t(j)...
+00006ea0: 007c 03a0 0a7c 04a1 0101 007c 006a 4044  .|...|.....|.j@D
+00006eb0: 0090 035d 667d 1b7c 1b7c 006a 416b 0390  ...]f}.|.|.jAk..
+00006ec0: 0872 147c 1b6a 2f7d 1c7c 1b6a 317d 1d6e  .r.|.j/}.|.j1}.n
+00006ed0: 307c 1b7c 006a 416b 0290 0872 447c 006a  0|.|.jAk...rD|.j
+00006ee0: 427c 006a 3e17 007d 1c7c 006a 437c 006a  B|.j>..}.|.jC|.j
+00006ef0: 3f17 007d 1d7c 1c7c 1b5f 2f7c 1d7c 1b5f  ?..}.|.|._/|.|._
+00006f00: 317c 1b7c 006a 416b 0290 0872 6874 00a0  1|.|.jAk...rht..
+00006f10: 0d74 00a0 0e64 1a64 1a64 1b64 03a1 04a1  .t...d.d.d.d....
+00006f20: 017d 1e6e 887c 1b7c 006a 446b 0290 0872  .}.n.|.|.jDk...r
+00006f30: 8c74 00a0 0d74 00a0 0e64 1c64 1d64 1d64  .t...t...d.d.d.d
+00006f40: 03a1 04a1 017d 1e6e 647c 1b6a 4590 0872  .....}.nd|.jE..r
+00006f50: b87c 1b7c 006a 1e6b 0390 0872 b874 00a0  .|.|.j.k...r.t..
+00006f60: 0d7c 006a 076a 08a0 0964 04a1 0164 02a1  .|.j.j...d...d..
+00006f70: 027d 1e6e 387c 1b7c 006a 1e6b 0290 0872  .}.n8|.|.j.k...r
+00006f80: da74 00a0 0d7c 006a 076a 08a0 0964 13a1  .t...|.j.j...d..
+00006f90: 01a1 017d 1e6e 1674 00a0 0d7c 006a 076a  ...}.n.t...|.j.j
+00006fa0: 08a0 0964 04a1 0164 02a1 027d 1e74 137c  ...d...d...}.t.|
+00006fb0: 1c83 017d 1c74 137c 1d83 017d 1d7c 1b6a  ...}.t.|...}.|.j
+00006fc0: 4590 0972 6074 00a0 067c 006a 076a 08a0  E..r`t...|.j.j..
+00006fd0: 0964 15a1 0164 02a1 027d 047c 1b6a 4690  .d...d...}.|.jF.
+00006fe0: 0972 3e74 00a0 0d7c 006a 076a 08a0 0964  .r>t...|.j.j...d
+00006ff0: 1ea1 0164 02a1 027d 1e6e 1674 00a0 0d7c  ...d...}.n.t...|
+00007000: 006a 076a 08a0 0964 02a1 0164 02a1 027d  .j.j...d...d...}
+00007010: 1e7c 03a0 0a7c 04a1 0101 006e d67c 006a  .|...|.....n.|.j
+00007020: 3d7c 1c7c 006a 2e17 0014 007d 177c 006a  =|.|.j.....}.|.j
+00007030: 3d7c 1d64 1f18 007c 006a 3017 0014 007d  =|.d...|.j0....}
+00007040: 1874 00a0 067c 006a 076a 08a0 0964 15a1  .t...|.j.j...d..
+00007050: 0164 02a1 027d 047c 03a0 0a7c 04a1 0101  .d...}.|...|....
+00007060: 0064 207d 157a 2474 137c 006a 076a 47a0  .d }.z$t.|.j.jG.
+00007070: 36a1 0083 017d 157c 03a0 3774 3864 187c  6....}.|..7t8d.|
+00007080: 1583 02a1 0101 0057 006e 3004 0074 396b  .......W.n0..t9k
+00007090: 0a90 0972 fc01 007d 1601 007a 1074 3a74  ...r...}...z.t:t
+000070a0: 267c 1683 0183 0101 0057 0035 0064 007d  &|.......W.5.d.}
+000070b0: 167e 1658 0059 006e 0258 007c 006a 076a  .~.X.Y.n.X.|.j.j
+000070c0: 48a0 0ca1 0090 0a72 2474 00a0 0d7c 006a  H......r$t...|.j
+000070d0: 076a 08a0 0964 16a1 0164 02a1 027d 1f6e  .j...d...d...}.n
+000070e0: 0464 007d 1f7c 1b6a 3ba0 3c7c 037c 1fa1  .d.}.|.j;.<|.|..
+000070f0: 0201 007c 03a0 497c 1ea1 0101 007c 1b6a  ...|..I|.....|.j
+00007100: 4590 0a72 ec7c 1c64 1517 007d 207c 1d64  E..r.|.d...} |.d
+00007110: 1517 007d 2174 00a0 0674 00a0 0e64 0464  ...}!t...t...d.d
+00007120: 0464 0464 04a1 0464 04a1 027d 047c 03a0  .d.d...d...}.|..
+00007130: 0a7c 04a1 0101 007c 1b6a 4690 0a72 907c  .|.....|.jF..r.|
+00007140: 006a 076a 4aa0 0ca1 007d 226e 0c7c 006a  .j.jJ....}"n.|.j
+00007150: 076a 4ba0 0ca1 007d 227c 2290 0a72 ca7c  .jK....}"|"..r.|
+00007160: 1b7c 076b 0690 0a72 bc7c 1b6a 3c7c 0364  .|.k...r.|.j<|.d
+00007170: 0864 218d 0201 006e 0e7c 1b6a 3c7c 0364  .d!....n.|.j<|.d
+00007180: 0964 218d 0201 0074 00a0 067c 006a 076a  .d!....t...|.j.j
+00007190: 08a0 0964 01a1 0164 02a1 027d 047c 03a0  ...d...d...}.|..
+000071a0: 0a7c 04a1 0101 006e 6e74 00a0 0674 00a0  .|.....nnt...t..
+000071b0: 0e64 0464 0464 1c64 04a1 0464 04a1 027d  .d.d.d.d...d...}
+000071c0: 047c 03a0 0a7c 04a1 0101 007c 1b7c 076b  .|...|.....|.|.k
+000071d0: 0690 0b72 2a7c 1b6a 3c7c 037c 1e64 0864  ...r*|.j<|.|.d.d
+000071e0: 228d 0301 006e 107c 1b6a 3c7c 037c 1e64  "....n.|.j<|.|.d
+000071f0: 0964 228d 0301 0074 00a0 067c 006a 076a  .d"....t...|.j.j
+00007200: 08a0 0964 16a1 0164 02a1 027d 047c 03a0  ...d...d...}.|..
+00007210: 0a7c 04a1 0101 0090 0771 f47c 00a0 4c7c  .|.......q.|..L|
+00007220: 03a1 0101 007c 0353 0029 234e 7230 0000  .....|.S.)#Nr0..
+00007230: 0072 1200 0000 e9ff 0000 0072 0100 0000  .r.........r....
+00007240: 7269 0000 0063 0100 0000 0000 0000 0000  ri...c..........
+00007250: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00007260: 0000 0067 007c 005d 0c7d 017c 01a0 00a1  ...g.|.].}.|....
+00007270: 0091 0271 0453 0072 2100 0000 2901 da04  ...q.S.r!...)...
+00007280: 7465 7874 2902 720d 0100 00da 0469 7465  text).r......ite
+00007290: 6d72 2100 0000 7221 0000 0072 2200 0000  mr!...r!...r"...
+000072a0: 720e 0100 0077 0500 0073 0400 0000 0600  r....w...s......
+000072b0: 0200 7a26 4d79 4472 6177 5769 6467 6574  ..z&MyDrawWidget
+000072c0: 2e70 6169 6e74 2e3c 6c6f 6361 6c73 3e2e  .paint.<locals>.
+000072d0: 3c6c 6973 7463 6f6d 703e 5446 7225 0100  <listcomp>TFr%..
+000072e0: 00da 0973 686f 7274 6e61 6d65 7a0f 756e  ...shortnamez.un
+000072f0: 692d 6469 7265 6374 696f 6e61 6cda 0546  i-directional..F
+00007300: 616c 7365 6700 0000 0000 00f8 3f7a 0f6c  alseg.......?z.l
+00007310: 6f67 2074 7261 6e73 6163 7469 6f6e da04  og transaction..
+00007320: 5472 7565 72e0 0000 0072 3d01 0000 7268  Truer....r=...rh
+00007330: 0000 0029 0272 5c01 0000 725d 0100 00e9  ...).r\...r]....
+00007340: 0600 0000 7228 0100 0072 9500 0000 5a05  ....r(...r....Z.
+00007350: 4172 6961 6c29 0172 4700 0000 e922 0000  Arial).rG...."..
+00007360: 00e9 e600 0000 7299 0000 0072 dd00 0000  ......r....r....
+00007370: 725b 0000 00e9 0b00 0000 e90c 0000 0029  r[.............)
+00007380: 0172 6c00 0000 2902 7246 0000 0072 6c00  .rl...).rF...rl.
+00007390: 0000 294d 7206 0000 0072 0400 0000 da05  ..)Mr....r......
+000073a0: 7363 616c 6572 5701 0000 5a17 4869 6768  scalerW...Z.High
+000073b0: 5175 616c 6974 7941 6e74 6961 6c69 6173  QualityAntialias
+000073c0: 696e 675a 1054 6578 7441 6e74 6961 6c69  ingZ.TextAntiali
+000073d0: 6173 696e 6772 7b01 0000 7235 0000 0072  asingr{...r5...r
+000073e0: 8800 0000 727c 0100 0072 7d01 0000 da0a  ....r|...r}.....
+000073f0: 6368 6563 6b42 6f78 5f37 7237 0000 0072  checkBox_7r7...r
+00007400: 7e01 0000 727f 0100 0072 4300 0000 7203  ~...r....rC...r.
+00007410: 0000 0072 4100 0000 7242 0000 0072 4000  ...rA...rB...r@.
+00007420: 0000 729e 0000 0072 9f00 0000 7282 0100  ..r....r....r...
+00007430: 00da 0373 6574 da0b 6669 6c74 6572 436f  ...set..filterCo
+00007440: 6d62 6f5a 0d73 656c 6563 7465 6449 7465  mboZ.selectedIte
+00007450: 6d73 72b3 0000 0072 0f01 0000 7217 0100  msr....r....r...
+00007460: 0072 a800 0000 72f2 0000 0072 0501 0000  .r....r....r....
+00007470: 724b 0000 0072 4c00 0000 72a9 0000 00da  rK...rL...r.....
+00007480: 0965 6e75 6d65 7261 7465 da0a 656e 7472  .enumerate..entr
+00007490: 795f 6461 7461 721c 0000 0072 e900 0000  y_datar....r....
+000074a0: da08 7365 7453 7479 6c65 7207 0000 00da  ..setStyler.....
+000074b0: 0953 6f6c 6964 4c69 6e65 5a09 7365 7457  .SolidLineZ.setW
+000074c0: 6964 7468 46da 0844 6173 684c 696e 655a  idthF..DashLineZ
+000074d0: 0e73 6574 4461 7368 5061 7474 6572 6e72  .setDashPatternr
+000074e0: 6c01 0000 723c 0000 0072 1a00 0000 723d  l...r<...r....r=
+000074f0: 0000 0072 1b00 0000 72aa 0000 00da 0a63  ...r....r......c
+00007500: 6865 636b 426f 785f 35da 0a63 6865 636b  heckBox_5..check
+00007510: 426f 785f 32da 1173 7069 6e42 6f78 466f  Box_2..spinBoxFo
+00007520: 6e74 5369 7a65 5f32 da05 7661 6c75 65da  ntSize_2..value.
+00007530: 0773 6574 466f 6e74 7210 0000 0072 e800  .setFontr....r..
+00007540: 0000 7215 0000 0072 6000 0000 7252 0000  ..r....r`...rR..
+00007550: 0072 3400 0000 7225 0000 0072 2600 0000  .r4...r%...r&...
+00007560: 7296 0000 0072 b700 0000 72ca 0000 0072  r....r....r....r
+00007570: cb00 0000 72b8 0000 0072 6100 0000 7262  ....r....ra...rb
+00007580: 0000 00da 0f73 7069 6e42 6f78 466f 6e74  .....spinBoxFont
+00007590: 5369 7a65 723e 0000 00da 0873 6574 4272  Sizer>.....setBr
+000075a0: 7573 68da 0a63 6865 636b 426f 785f 36da  ush..checkBox_6.
+000075b0: 0a63 6865 636b 426f 785f 3372 8a01 0000  .checkBox_3r....
+000075c0: 2923 7227 0000 0072 e100 0000 72e2 0000  )#r'...r....r...
+000075d0: 0072 4500 0000 7283 0100 005a 0862 725f  .rE...r....Z.br_
+000075e0: 7768 6974 655a 0b66 696c 7465 725f 7661  whiteZ.filter_va
+000075f0: 6c73 5a0c 6163 7469 7665 5f62 6f78 6573  lsZ.active_boxes
+00007600: 5a11 6163 7469 7665 5f63 6f6e 6e65 6374  Z.active_connect
+00007610: 6f72 73da 0463 6f6e 6e5a 0c6e 6f5f 7365  ors..connZ.no_se
+00007620: 6c65 6374 696f 6e5a 0b69 735f 7365 6c65  lectionZ.is_sele
+00007630: 6374 6564 725d 0100 0072 5c01 0000 7260  ctedr]...r\...r`
+00007640: 0100 00da 0464 6174 6172 d000 0000 5a0a  .....datar....Z.
+00007650: 6f66 6673 6574 5f62 6f78 da02 7478 da02  offset_box..tx..
+00007660: 7479 7246 0000 00da 0866 6f6e 7473 697a  tyrF.....fontsiz
+00007670: 6572 9700 0000 724b 0000 0072 4c00 0000  er....rK...rL...
+00007680: da02 6132 da02 6232 7223 0000 0072 1a00  ..a2..b2r#...r..
+00007690: 0000 721b 0000 00da 0262 725a 0862 725f  ..r......brZ.br_
+000076a0: 6c61 6265 6c72 6f00 0000 7270 0000 005a  labelro...rp...Z
+000076b0: 0873 686f 775f 626f 7872 2100 0000 7221  .show_boxr!...r!
+000076c0: 0000 0072 2200 0000 72ec 0000 0055 0500  ...r"...r....U..
+000076d0: 0073 8c01 0000 0002 0a01 0c02 0e01 0e09  .s..............
+000076e0: 1601 0a03 0c01 1801 3801 0801 1e02 0801  ........8.......
+000076f0: 1c06 0a02 1a01 0401 0402 0a01 0c01 2801  ..............(.
+00007700: 0c01 0a02 0c01 0c02 2a01 0e03 0c02 0401  ........*.......
+00007710: 0402 0e02 1602 0401 1401 1202 1201 0402  ................
+00007720: 0c0b 1602 0a03 0401 0402 1401 1202 1201  ................
+00007730: 0402 1201 0402 0a02 0601 1802 1602 0c01  ................
+00007740: 0c03 0c02 0e01 0a02 0401 0403 0a07 0401  ................
+00007750: 0402 0a03 1a01 1401 1401 1401 1400 1401  ................
+00007760: 1400 1401 0201 02f9 0a0c 0c01 0c01 0c01  ................
+00007770: 0c01 0c01 0c01 0c01 0c02 0e01 1601 0c02  ................
+00007780: 1601 0a03 0e01 0e03 0e01 1802 1602 0402  ................
+00007790: 0201 1001 1402 1201 1e02 1002 0419 0e01  ................
+000077a0: 0e01 1802 1603 2403 0a01 0a02 0e01 1004  ......$.........
+000077b0: 1401 1402 2001 2003 0402 0201 1001 1402  .... . .........
+000077c0: 1201 1e02 1802 0225 1a01 1401 1401 1401  .......%........
+000077d0: 1400 1401 1400 1401 0201 02f9 0e11 1601  ................
+000077e0: 0c03 0a11 0c02 0c02 0601 0802 0c02 0c01  ................
+000077f0: 0c02 0601 060a 0c01 1801 0c01 1801 1408  ................
+00007800: 1803 0c01 1608 1602 0801 0802 0801 1602  ................
+00007810: 0801 1802 1602 0c0b 1001 1403 1601 0a04  ................
+00007820: 0402 0201 1001 1402 1201 1e04 0e02 1802  ................
+00007830: 040d 0e03 0a02 0802 0801 0802 1801 0a03  ................
+00007840: 0801 0e02 0c02 0601 0a08 100a 0e08 1601  ................
+00007850: 0c09 1802 0a11 0a01 1202 100c 1601 0e01  ................
+00007860: 0a05 7a12 4d79 4472 6177 5769 6467 6574  ..z.MyDrawWidget
+00007870: 2e70 6169 6e74 6302 0000 0000 0000 0000  .paintc.........
+00007880: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00007890: 0e00 0000 7c00 a000 7c00 a101 0100 6400  ....|...|.....d.
+000078a0: 5300 7229 0000 0029 0172 ec00 0000 72d4  S.r)...).r....r.
+000078b0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+000078c0: 0000 da0a 7061 696e 7445 7665 6e74 5d07  ....paintEvent].
+000078d0: 0000 7302 0000 0000 017a 174d 7944 7261  ..s......z.MyDra
+000078e0: 7757 6964 6765 742e 7061 696e 7445 7665  wWidget.paintEve
+000078f0: 6e74 6307 0000 0000 0000 0000 0000 0009  ntc.............
+00007900: 0000 0004 0000 0043 0000 0073 7c00 0000  .......C...s|...
+00007910: 7c00 6a00 7c03 7c00 6a01 1700 1400 7c01  |.j.|.|.j.....|.
+00007920: 7c00 6a00 1400 0400 0300 6b00 6f34 7c00  |.j.......k.o4|.
+00007930: 6a00 7c03 7c00 6a01 1700 7c05 1700 1400  j.|.|.j...|.....
+00007940: 6b00 6e04 0200 0100 7d07 7c00 6a00 7c04  k.n.....}.|.j.|.
+00007950: 7c00 6a02 1700 1400 7c02 7c00 6a00 1400  |.j.....|.|.j...
+00007960: 0400 0300 6b00 6f6e 7c00 6a00 7c04 7c06  ....k.on|.j.|.|.
+00007970: 1700 7c00 6a02 1700 1400 6b00 6e04 0200  ..|.j.....k.n...
+00007980: 0100 7d08 7c07 6f7a 7c08 5300 2901 7a6e  ..}.|.oz|.S.).zn
+00007990: 0a20 2020 2020 2020 2063 6865 636b 2069  .        check i
+000079a0: 6620 2878 2c79 2920 6c69 6573 2077 6974  f (x,y) lies wit
+000079b0: 6869 6e20 7468 6520 7265 6374 616e 676c  hin the rectangl
+000079c0: 650a 2020 2020 2020 2020 2878 622c 2079  e.        (xb, y
+000079d0: 6229 2c20 2878 622c 2079 622b 7779 292c  b), (xb, yb+wy),
+000079e0: 202e 2e2e 2e2c 2028 7862 2b77 782c 2079   ...., (xb+wx, y
+000079f0: 622b 7779 290a 2020 2020 2020 2020 2903  b+wy).        ).
+00007a00: 7234 0000 0072 3c00 0000 723d 0000 0029  r4...r<...r=...)
+00007a10: 0972 2700 0000 721a 0000 0072 1b00 0000  .r'...r....r....
+00007a20: da02 7862 da02 7962 721c 0100 0072 1d01  ..xb..ybr....r..
+00007a30: 0000 da05 636f 6e64 31da 0563 6f6e 6432  ....cond1..cond2
+00007a40: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00007a50: 0768 6974 5f62 6f78 6107 0000 7306 0000  .hit_boxa...s...
+00007a60: 0000 063a 013a 017a 144d 7944 7261 7757  ...:.:.z.MyDrawW
+00007a70: 6964 6765 742e 6869 745f 626f 7863 0200  idget.hit_boxc..
+00007a80: 0000 0000 0000 0000 0000 0b00 0000 0900  ................
+00007a90: 0000 4300 0000 734c 0400 0074 0064 0183  ..C...sL...t.d..
+00007aa0: 0101 007c 006a 01a0 027c 006a 037c 006a  ...|.j...|.j.|.j
+00007ab0: 04a1 0201 0074 05a0 05a1 007c 006a 0618  .....t.....|.j..
+00007ac0: 007d 0274 05a0 05a1 007c 005f 067c 01a0  .}.t.....|._.|..
+00007ad0: 07a1 0074 086a 096a 0a40 0072 4a64 027c  ...t.j.j.@.rJd.|
+00007ae0: 005f 0b6e 167c 01a0 07a1 0074 086a 096a  ._.n.|.....t.j.j
+00007af0: 0c40 0072 6064 037c 005f 0b7c 01a0 0da1  .@.r`d.|._.|....
+00007b00: 00a0 0ea1 007c 01a0 0da1 00a0 0fa1 0002  .....|..........
+00007b10: 007d 037d 0474 107c 037c 006a 111b 0083  .}.}.t.|.|.j....
+00007b20: 017d 0374 107c 047c 006a 111b 0083 017d  .}.t.|.|.j.....}
+00007b30: 047c 037c 005f 127c 047c 005f 137c 006a  .|.|._.|.|._.|.j
+00007b40: 147c 005f 157c 006a 167c 005f 1764 047d  .|._.|.j.|._.d.}
+00007b50: 0564 007c 005f 187c 006a 0344 005d 587d  .d.|._.|.j.D.]X}
+00007b60: 067c 006a 0b64 056b 0372 c27c 00a0 197c  .|.j.d.k.r.|...|
+00007b70: 037c 047c 066a 1a6a 0e7c 066a 1a6a 1b17  .|.|.j.j.|.j.j..
+00007b80: 007c 066a 1a6a 0f7c 066a 1a6a 1c17 0064  .|.j.j.|.j.j...d
+00007b90: 0618 0064 0764 08a1 0672 c264 097c 005f  ...d.d...r.d.|._
+00007ba0: 0b7c 066a 1a7c 005f 1874 0064 0a7c 066a  .|.j.|._.t.d.|.j
+00007bb0: 1d83 0201 0071 c27c 006a 0344 0090 035d  .....q.|.j.D...]
+00007bc0: 047d 067c 066a 1e90 0172 3664 0b7d 076e  .}.|.j...r6d.}.n
+00007bd0: 0464 0c7d 077c 006a 0b64 056b 0390 0172  .d.}.|.j.d.k...r
+00007be0: 227c 00a0 197c 037c 047c 066a 0e7c 066a  "|...|.|.|.j.|.j
+00007bf0: 0f7c 077c 07a1 0690 0172 2274 0064 0d7c  .|.|.....r"t.d.|
+00007c00: 066a 1d83 0201 0064 0e7d 057c 006a 0b64  .j.....d.}.|.j.d
+00007c10: 026b 0290 0172 9e7c 067c 005f 187c 066a  .k...r.|.|._.|.j
+00007c20: 0e7c 0318 007c 005f 1b7c 066a 0f7c 0418  .|...|._.|.j.|..
+00007c30: 007c 005f 1c90 0171 227c 006a 0b64 036b  .|._...q"|.j.d.k
+00007c40: 0290 0272 3e7c 0264 0f6b 0090 0172 da7c  ...r>|.d.k...r.|
+00007c50: 006a 1f64 006b 0890 0172 c67c 067c 005f  .j.d.k...r.|.|._
+00007c60: 1f7c 00a0 20a1 0001 0064 007c 005f 1f01  .|.. ....d.|._..
+00007c70: 0064 0053 007c 006a 1f7c 066b 0290 0272  .d.S.|.j.|.k...r
+00007c80: 0064 007c 005f 1f74 0064 107c 0683 0201  .d.|._.t.d.|....
+00007c90: 007c 00a0 21a1 0001 006e 1074 0064 117c  .|..!....n.t.d.|
+00007ca0: 0683 0201 007c 067c 005f 1f7c 066a 1e90  .....|.|._.|.j..
+00007cb0: 0272 327c 006a 1f7c 066b 0290 0272 327c  .r2|.j.|.k...r2|
+00007cc0: 006a 01a0 227c 066a 1da1 0101 007c 00a0  .j.."|.j.....|..
+00007cd0: 21a1 0001 0090 0171 227c 006a 0b64 126b  !......q"|.j.d.k
+00007ce0: 0290 0272 8c74 0064 137c 0683 0201 007c  ...r.t.d.|.....|
+00007cf0: 066a 1e90 0272 7074 0064 1483 0101 0074  .j...rpt.d.....t
+00007d00: 237c 007c 0683 027d 086e 1274 0064 1583  #|.|...}.n.t.d..
+00007d10: 0101 0074 247c 007c 0683 027d 0864 037c  ...t$|.|...}.d.|
+00007d20: 005f 0b90 0171 227c 006a 0b64 166b 0290  ._...q"|.j.d.k..
+00007d30: 0372 9674 2564 1783 0182 0164 007c 005f  .r.t%d.....d.|._
+00007d40: 1864 007c 005f 2664 007c 005f 277c 066a  .d.|._&d.|._'|.j
+00007d50: 1e90 0372 047c 066a 2864 006b 0990 0372  ...r.|.j(d.k...r
+00007d60: 047c 006a 03a0 297c 066a 286a 2aa1 0101  .|.j..)|.j(j*...
+00007d70: 007c 006a 03a0 297c 066a 286a 2ba1 0101  .|.j..)|.j(j+...
+00007d80: 007c 006a 04a0 297c 066a 28a1 0101 007c  .|.j..)|.j(....|
+00007d90: 00a0 21a1 0001 0064 027c 005f 0b6e 907c  ..!....d.|._.n.|
+00007da0: 006a 0444 005d 627d 097c 096a 2c7c 066b  .j.D.]b}.|.j,|.k
+00007db0: 0290 0373 267c 096a 2d7c 066b 0290 0372  ...s&|.j-|.k...r
+00007dc0: 0a7c 006a 04a0 297c 09a1 0101 007c 006a  .|.j..)|.....|.j
+00007dd0: 03a0 297c 096a 2ca1 0101 007c 006a 03a0  ..)|.j,....|.j..
+00007de0: 297c 096a 2da1 0101 007c 006a 03a0 297c  )|.j-....|.j..)|
+00007df0: 096a 2aa1 0101 007c 006a 03a0 297c 096a  .j*....|.j..)|.j
+00007e00: 2ba1 0101 0090 0371 0a7c 067c 006a 036b  +......q.|.|.j.k
+00007e10: 0690 0372 867c 006a 03a0 297c 06a1 0101  ...r.|.j..)|....
+00007e20: 007c 00a0 21a1 0001 0064 027c 005f 0b6e  .|..!....d.|._.n
+00007e30: 907c 006a 0b64 186b 0290 0172 2264 007c  .|.j.d.k...r"d.|
+00007e40: 005f 187c 006a 2664 006b 0890 0372 c47c  ._.|.j&d.k...r.|
+00007e50: 067c 005f 267c 00a0 21a1 0001 006e 627c  .|._&|..!....nb|
+00007e60: 006a 2764 006b 0890 0172 227c 066a 1e90  .j'd.k...r"|.j..
+00007e70: 0173 227c 067c 005f 2774 2e7c 006a 267c  .s"|.|._'t.|.j&|
+00007e80: 006a 2783 027d 0a7c 006a 04a0 2f7c 0aa1  .j'..}.|.j../|..
+00007e90: 0101 007c 006a 03a0 2f7c 0a6a 2aa1 0101  ...|.j../|.j*...
+00007ea0: 007c 006a 03a0 2f7c 0a6a 2ba1 0101 0064  .|.j../|.j+....d
+00007eb0: 007c 005f 2664 007c 005f 2764 027c 005f  .|._&d.|._'d.|._
+00007ec0: 0b90 0171 227c 0590 0473 487c 01a0 07a1  ...q"|...sH|....
+00007ed0: 0074 086a 096a 0c40 0090 0472 4864 057c  .t.j.j.@...rHd.|
+00007ee0: 005f 0b64 0053 0029 194e 7a17 4d4f 5553  ._.d.S.).Nz.MOUS
+00007ef0: 4520 5052 4553 5320 4452 4157 2057 4944  E PRESS DRAW WID
+00007f00: 4745 54da 0464 7261 6772 b000 0000 4672  GET..dragr....Fr
+00007f10: b200 0000 7295 0100 0072 3d01 0000 72d9  ....r....r=...r.
+00007f20: 0000 00da 0a64 7261 675f 6c61 6265 6c72  .....drag_labelr
+00007f30: b700 0000 72dd 0000 0072 ae00 0000 7a07  ....r....r....z.
+00007f40: 626f 7820 6869 7454 679a 9999 9999 99c9  box hitTg.......
+00007f50: 3f5a 0b75 6e68 6967 686c 6967 6874 5a09  ?Z.unhighlightZ.
+00007f60: 6869 6768 6c69 6768 745a 0465 6469 745a  highlightZ.editZ
+00007f70: 0445 4449 547a 0e45 4449 5420 434f 4e4e  .EDITz.EDIT CONN
+00007f80: 4543 544f 527a 0a45 4449 5420 4147 454e  ECTORz.EDIT AGEN
+00007f90: 54da 0664 656c 6574 657a 1944 656c 6574  T..deletez.Delet
+00007fa0: 6520 6d6f 6465 206e 6f74 2073 7570 706f  e mode not suppo
+00007fb0: 7274 6564 728c 0000 0029 3072 1500 0000  rtedr....)0r....
+00007fc0: 7235 0000 00da 1475 7064 6174 655f 6772  r5.....update_gr
+00007fd0: 6170 6869 6373 5f64 6174 6172 9600 0000  aphics_datar....
+00007fe0: 72b3 0000 0072 bb00 0000 72bc 0000 00da  r....r....r.....
+00007ff0: 0762 7574 746f 6e73 7203 0000 0072 0700  .buttonsr....r..
+00008000: 0000 da0b 5269 6768 7442 7574 746f 6e72  ....RightButtonr
+00008010: cd00 0000 da0a 4c65 6674 4275 7474 6f6e  ......LeftButton
+00008020: 727c 0000 0072 1a00 0000 721b 0000 0072  r|...r....r....r
+00008030: 4000 0000 7234 0000 0072 c400 0000 72c5  @...r4...r....r.
+00008040: 0000 0072 3c00 0000 72c6 0000 0072 3d00  ...r<...r....r=.
+00008050: 0000 72c7 0000 0072 b700 0000 72b6 0100  ..r....r....r...
+00008060: 0072 6000 0000 7225 0000 0072 2600 0000  .r`...r%...r&...
+00008070: 721c 0000 0072 6100 0000 72f2 0000 0072  r....ra...r....r
+00008080: 9400 0000 72d2 0000 00da 1164 6174 615f  ....r......data_
+00008090: 7365 6c65 6374 5f77 6865 7265 5a11 5472  select_whereZ.Tr
+000080a0: 616e 7361 6374 696f 6e45 6469 746f 725a  ansactionEditorZ
+000080b0: 0b41 6765 6e74 4564 6974 6f72 da0c 5275  .AgentEditor..Ru
+000080c0: 6e74 696d 6545 7272 6f72 72b8 0000 0072  ntimeErrorr....r
+000080d0: b900 0000 7263 0000 0072 ff00 0000 72a9  ....rc...r....r.
+000080e0: 0000 0072 aa00 0000 724b 0000 0072 4c00  ...r....rK...rL.
+000080f0: 0000 72a2 0000 0072 0501 0000 290b 7227  ..r....r....).r'
+00008100: 0000 0072 d500 0000 5a0a 7469 6d65 5f64  ...r....Z.time_d
+00008110: 656c 6179 721a 0000 0072 1b00 0000 5a07  elayr....r....Z.
+00008120: 626f 785f 6869 7472 2300 0000 726e 0000  box_hitr#...rn..
+00008130: 005a 0a6e 6577 5f65 6469 746f 7272 a901  .Z.new_editorr..
+00008140: 0000 da03 636f 6e72 2100 0000 7221 0000  ....conr!...r!..
+00008150: 0072 2200 0000 da0f 6d6f 7573 6550 7265  .r".....mousePre
+00008160: 7373 4576 656e 746b 0700 0073 be00 0000  ssEventk...s....
+00008170: 0001 0802 1202 0e01 0a03 1001 0802 1001  ................
+00008180: 0602 1a02 0e01 0e02 0601 0601 0801 0803  ................
+00008190: 0401 0603 0a02 3a01 0601 0801 0e03 0c01  ......:.........
+000081a0: 0801 0602 0402 2601 0c03 0401 0c01 0601  ......&.........
+000081b0: 0c01 1002 0c01 0a01 0c01 0601 0801 0601  ................
+000081c0: 0602 0c01 0601 0a01 0a02 0a01 0604 1401  ................
+000081d0: 0e02 0c02 0c01 0a02 0801 0801 0c03 0801  ................
+000081e0: 0a02 0a02 0c01 0801 0601 0601 0602 1401  ................
+000081f0: 1001 1001 0e01 0801 0804 0a01 1801 0c01  ................
+00008200: 0e01 0e01 0e01 1202 0c01 0c02 0801 0803  ................
+00008210: 0c01 0602 0c01 0601 0a02 1401 0602 0e01  ................
+00008220: 0c01 0e01 0e02 0601 0601 0a02 1802 7a1c  ..............z.
+00008230: 4d79 4472 6177 5769 6467 6574 2e6d 6f75  MyDrawWidget.mou
+00008240: 7365 5072 6573 7345 7665 6e74 6302 0000  sePressEventc...
+00008250: 0000 0000 0000 0000 0009 0000 0005 0000  ................
+00008260: 0043 0000 0073 b001 0000 7c01 a000 a100  .C...s....|.....
+00008270: a001 a100 7c01 a000 a100 a002 a100 0200  ....|...........
+00008280: 7d02 7d03 7403 7c02 7c00 6a04 1b00 8301  }.}.t.|.|.j.....
+00008290: 7d02 7403 7c03 7c00 6a04 1b00 8301 7d03  }.t.|.|.j.....}.
+000082a0: 7c02 7c00 5f05 7c03 7c00 5f06 7c00 6a07  |.|._.|.|._.|.j.
+000082b0: 6401 6b02 7274 7c02 7c00 6a08 1800 7d04  d.k.rt|.|.j...}.
+000082c0: 7c03 7c00 6a09 1800 7d05 7c04 7c00 6a0a  |.|.j...}.|.|.j.
+000082d0: 5f0b 7c05 7c00 6a0a 5f0c 9001 6e30 7c00  _.|.|.j._...n0|.
+000082e0: 6a07 6402 6b02 72c0 7c02 7d02 7c03 7d03  j.d.k.r.|.}.|.}.
+000082f0: 7c02 7c00 6a08 1800 7d04 7c03 7c00 6a09  |.|.j...}.|.|.j.
+00008300: 1800 7d05 7c00 a00d 7c00 6a0e 7c04 1700  ..}.|...|.j.|...
+00008310: a101 7c00 5f0f 7c00 a00d 7c00 6a10 7c05  ..|._.|...|.j.|.
+00008320: 1700 a101 7c00 5f11 6ee4 6403 7d06 7c00  ....|._.n.d.}.|.
+00008330: 6a12 4400 5dc6 7d07 7c07 6a13 72da 6404  j.D.].}.|.j.r.d.
+00008340: 7d08 6e04 6405 7d08 7c00 6a07 6402 6b03  }.n.d.}.|.j.d.k.
+00008350: 72ca 7c00 6a04 7c07 6a01 7c00 6a0f 1700  r.|.j.|.j.|.j...
+00008360: 1400 7c02 7c00 6a04 1400 0400 0300 6b00  ..|.|.j.......k.
+00008370: 9001 7224 7c00 6a04 7c07 6a01 7c00 6a0f  ..r$|.j.|.j.|.j.
+00008380: 1700 7c08 1700 1400 6b00 72ca 6e04 0100  ..|.....k.r.n...
+00008390: 71ca 7c00 6a04 7c07 6a02 7c00 6a11 1700  q.|.j.|.j.|.j...
+000083a0: 1400 7c03 7c00 6a04 1400 0400 0300 6b00  ..|.|.j.......k.
+000083b0: 9001 7264 7c00 6a04 7c07 6a02 7c08 1700  ..rd|.j.|.j.|...
+000083c0: 7c00 6a11 1700 1400 6b00 72ca 6e04 0100  |.j.....k.r.n...
+000083d0: 71ca 7c01 a014 a100 7415 6a16 6a17 4000  q.|.....t.j.j.@.
+000083e0: 9001 7280 6406 7c00 5f07 7c00 a018 7416  ..r.d.|._.|...t.
+000083f0: 6a19 a101 0100 6407 7d06 71ca 7c06 9001  j.....d.}.q.|...
+00008400: 73a4 7c00 a018 7416 6a1a a101 0100 7c00  s.|...t.j.....|.
+00008410: a01b a100 0100 6400 5300 2908 4e72 b801  ......d.S.).Nr..
+00008420: 0000 72b2 0000 0046 72dd 0000 0072 ae00  ..r....Fr....r..
+00008430: 0000 72b7 0100 0054 291c 727c 0000 0072  ..r....T).r|...r
+00008440: 1a00 0000 721b 0000 0072 4000 0000 7234  ....r....r@...r4
+00008450: 0000 0072 ca00 0000 72cb 0000 0072 cd00  ...r....r....r..
+00008460: 0000 72c4 0000 0072 c500 0000 72b7 0000  ..r....r....r...
+00008470: 0072 2500 0000 7226 0000 0072 3f00 0000  .r%...r&...r?...
+00008480: 72c6 0000 0072 3c00 0000 72c7 0000 0072  r....r<...r....r
+00008490: 3d00 0000 7296 0000 0072 6100 0000 72bb  =...r....ra...r.
+000084a0: 0100 0072 0300 0000 7207 0000 0072 bc01  ...r....r....r..
+000084b0: 0000 da09 7365 7443 7572 736f 72da 0e4f  ....setCursor..O
+000084c0: 7065 6e48 616e 6443 7572 736f 72da 0b41  penHandCursor..A
+000084d0: 7272 6f77 4375 7273 6f72 72d2 0000 0029  rrowCursorr....)
+000084e0: 0972 2700 0000 72d5 0000 0072 1a00 0000  .r'...r....r....
+000084f0: 721b 0000 0072 6600 0000 7267 0000 005a  r....rf...rg...Z
+00008500: 0868 6f76 6572 696e 6772 2300 0000 726e  .hoveringr#...rn
+00008510: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00008520: 0000 da0e 6d6f 7573 654d 6f76 6545 7665  ....mouseMoveEve
+00008530: 6e74 fa07 0000 733c 0000 0000 021a 020e  nt....s<........
+00008540: 010e 0206 0106 020a 020a 010a 0208 010c  ................
+00008550: 020a 0104 0104 020a 010a 0312 0114 0504  ................
+00008560: 010a 0106 0106 0204 018a 0212 0106 020c  ................
+00008570: 0106 0206 010c 037a 1b4d 7944 7261 7757  .......z.MyDrawW
+00008580: 6964 6765 742e 6d6f 7573 654d 6f76 6545  idget.mouseMoveE
+00008590: 7665 6e74 6302 0000 0000 0000 0000 0000  ventc...........
+000085a0: 0005 0000 0005 0000 0043 0000 0073 3801  .........C...s8.
+000085b0: 0000 7c00 6a00 7c00 5f01 7c00 6a02 7c00  ..|.j.|._.|.j.|.
+000085c0: 5f03 7c00 6a00 7c00 5f04 7c00 6a02 7c00  _.|.j.|._.|.j.|.
+000085d0: 5f05 7c00 6a06 6401 6b02 726c 7c00 6a07  _.|.j.d.k.rl|.j.
+000085e0: 6400 6b09 726c 7c00 6a07 0400 6a08 7c00  d.k.rl|.j...j.|.
+000085f0: 6a07 6a09 3700 0200 5f08 7c00 6a07 0400  j.j.7..._.|.j...
+00008600: 6a0a 7c00 6a07 6a0b 3700 0200 5f0a 6402  j.|.j.j.7..._.d.
+00008610: 7c00 6a07 5f09 6402 7c00 6a07 5f0b 7c00  |.j._.d.|.j._.|.
+00008620: 6a06 6403 6b02 9001 722e 7c01 a00c a100  j.d.k...r.|.....
+00008630: a008 a100 7c01 a00c a100 a00a a100 0200  ....|...........
+00008640: 7d02 7d03 7c00 6a0d 7d04 7c00 a00e 740f  }.}.|.j.}.|...t.
+00008650: 7c02 7c00 6a10 1b00 8301 7c04 a102 7d02  |.|.j.....|...}.
+00008660: 7c00 a00e 740f 7c03 7c00 6a10 1b00 8301  |...t.|.|.j.....
+00008670: 7c04 a102 7d03 7c02 7c00 5f11 7c03 7c00  |...}.|.|._.|.|.
+00008680: 5f12 7c00 6a07 6400 6b09 9001 7226 7c00  _.|.j.d.k...r&|.
+00008690: a00e 7c00 6a11 7c00 6a09 1700 a101 7c00  ..|.j.|.j.....|.
+000086a0: 6a07 5f08 7c00 a00e 7c00 6a12 7c00 6a0b  j._.|...|.j.|.j.
+000086b0: 1700 a101 7c00 6a07 5f0a 7c00 6a07 6a08  ....|.j._.|.j.j.
+000086c0: 7c00 6a07 5f13 7c00 6a07 6a0a 7c00 6a07  |.j._.|.j.j.|.j.
+000086d0: 5f14 6400 7c00 5f07 7c00 a015 a100 0100  _.d.|._.|.......
+000086e0: 6404 7c00 5f06 6400 5300 2905 4e72 b801  d.|._.d.S.).Nr..
+000086f0: 0000 7201 0000 0072 b701 0000 72b0 0000  ..r....r....r...
+00008700: 0029 1672 3c00 0000 72c6 0000 0072 3d00  .).r<...r....r=.
+00008710: 0000 72c7 0000 0072 c400 0000 72c5 0000  ..r....r....r...
+00008720: 0072 cd00 0000 72b7 0000 0072 1a00 0000  .r....r....r....
+00008730: 7225 0000 0072 1b00 0000 7226 0000 0072  r%...r....r&...r
+00008740: 7c00 0000 72ce 0000 0072 3f00 0000 7240  |...r....r?...r@
+00008750: 0000 0072 3400 0000 72ca 0000 0072 cb00  ...r4...r....r..
+00008760: 0000 725e 0000 0072 5f00 0000 72d2 0000  ..r^...r_...r...
+00008770: 0029 0572 2700 0000 72d5 0000 0072 1a00  .).r'...r....r..
+00008780: 0000 721b 0000 0072 8b01 0000 7221 0000  ..r....r....r!..
+00008790: 0072 2100 0000 7222 0000 00da 116d 6f75  .r!...r".....mou
+000087a0: 7365 5265 6c65 6173 6545 7665 6e74 2e08  seReleaseEvent..
+000087b0: 0000 7332 0000 0000 0208 0108 0108 0108  ..s2............
+000087c0: 020a 020a 0114 0114 0208 0108 030c 011a  ................
+000087d0: 0206 0116 0116 0206 0106 020c 0216 0116  ................
+000087e0: 010c 010c 0206 0108 027a 1e4d 7944 7261  .........z.MyDra
+000087f0: 7757 6964 6765 742e 6d6f 7573 6552 656c  wWidget.mouseRel
+00008800: 6561 7365 4576 656e 7429 0172 a300 0000  easeEvent).r....
+00008810: 2901 4629 0172 ae00 0000 2904 72d9 0000  ).F).r....).r...
+00008820: 0046 4672 6800 0000 2903 4654 5429 0172  .FFrh...).FTT).r
+00008830: 6800 0000 2901 7212 0000 0029 2b72 5300  h...).r....)+rS.
+00008840: 0000 7254 0000 0072 5500 0000 7233 0000  ..rT...rU...r3..
+00008850: 0072 2800 0000 72d3 0000 0072 8d00 0000  .r(...r....r....
+00008860: 72d8 0000 0072 db00 0000 72bf 0000 0072  r....r....r....r
+00008870: be00 0000 728f 0000 0072 f100 0000 7257  ....r....r....rW
+00008880: 0000 0072 f200 0000 7258 0000 0072 f800  ...r....rX...r..
+00008890: 0000 72f9 0000 0072 fb00 0000 72fe 0000  ..r....r....r...
+000088a0: 0072 9400 0000 7201 0100 0072 0301 0000  .r....r....r....
+000088b0: 7206 0100 0072 0701 0000 7208 0100 0072  r....r....r....r
+000088c0: 0b01 0000 7212 0100 0072 1401 0000 7215  ....r....r....r.
+000088d0: 0100 0072 2301 0000 7227 0100 0072 3c01  ...r#...r'...r<.
+000088e0: 0000 726c 0100 0072 8a01 0000 723f 0000  ..rl...r....r?..
+000088f0: 0072 ec00 0000 72b1 0100 0072 b601 0000  .r....r....r....
+00008900: 72c1 0100 0072 c501 0000 72c6 0100 0072  r....r....r....r
+00008910: 5900 0000 7221 0000 0072 2100 0000 721f  Y...r!...r!...r.
+00008920: 0000 0072 2200 0000 7232 0000 0054 0100  ...r"...r2...T..
+00008930: 0073 5e00 0000 0802 0402 0c45 080a 0804  .s^........E....
+00008940: 0809 080a 0809 0809 080d 0820 0201 0a03  ........... ....
+00008950: 0401 0a18 0808 0810 080d 0821 0804 0812  ...........!....
+00008960: 080a 0814 0806 0807 0a1e 0a11 080e 0826  ...............&
+00008970: 0a1d 0811 0a64 0a7f 007f 0041 0878 0a08  .....d.....A.x..
+00008980: 0a7f 007f 007f 007f 000c 0804 080a 087f  ................
+00008990: 0010 0834 7232 0000 0029 22da 0373 7973  ...4r2...)"..sys
+000089a0: da05 5079 5174 3572 0200 0000 7203 0000  ..PyQt5r....r...
+000089b0: 00da 0b50 7951 7435 2e51 7447 7569 7204  ...PyQt5.QtGuir.
+000089c0: 0000 0072 0500 0000 7206 0000 00da 0c50  ...r....r......P
+000089d0: 7951 7435 2e51 7443 6f72 6572 0700 0000  yQt5.QtCorer....
+000089e0: 7208 0000 00da 1173 6369 7079 2e69 6e74  r......scipy.int
+000089f0: 6572 706f 6c61 7465 7209 0000 0072 bb00  erpolater....r..
+00008a00: 0000 da0f 5079 5174 352e 5174 5769 6467  ....PyQt5.QtWidg
+00008a10: 6574 7372 0a00 0000 720b 0000 0072 0c00  etsr....r....r..
+00008a20: 0000 720d 0000 005a 1450 7951 7435 2e51  ..r....Z.PyQt5.Q
+00008a30: 7450 7269 6e74 5375 7070 6f72 7472 0e00  tPrintSupportr..
+00008a40: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00008a50: 0072 e400 0000 da05 6e75 6d70 7972 9a00  .r......numpyr..
+00008a60: 0000 da0c 6167 656e 745f 6564 6974 6f72  ....agent_editor
+00008a70: 7213 0000 0072 1400 0000 725a 0000 0072  r....r....rZ...r
+00008a80: a200 0000 727e 0000 0072 3200 0000 7221  ....r~...r2...r!
+00008a90: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00008aa0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00008ab0: 7326 0000 0008 0110 0110 010c 0110 010c  s&..............
+00008ac0: 0108 0110 010c 010c 0110 0110 0208 0108  ................
+00008ad0: 040c 030e 560e 7f00 3b0e 2e              ....V...;..
```

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mainloop_editor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/mamba_interpreter2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/output_display.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/output_display.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/pandasmodel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/qtattune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/qtattune.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/resources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/resources.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/theme_manager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/gui/attune/src/__pycache__/yaml_editor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/agent_editor.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/agent_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/code_editor.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/code_editor.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/draw_widget.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/draw_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1086,21 +1086,21 @@
                 else:
                     # method  = self.interpol_method
                     # alpha = np.linspace(0, 1, 60) #np.linspace(0, 1, 80)
 
                     c0x = 0.5*(xi-x0)
                     c0y = 0.5*(yi-y0) 
 
-                    r = 0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) 
+                    rx = max(3,0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) )
+                    ry = max(3,0.5 * np.sqrt((xi-xd)**2 + (yi-yd)**2) )
                     
                     t0 = np.arctan2((yi-y0) ,(xi-x0))
 
                     t = t0 + np.linspace(0,2*np.pi, 100)
-                    rx = r 
-                    ry = 0.7*r 
+                    
 
                     x_coords = [rx * np.cos(ti) * np.cos(t0) - ry * np.sin(ti) * np.sin(t0) + c0x + x0 for ti in t]
                     y_coords = [rx * np.cos(ti) * np.sin(t0) + ry* np.sin(ti) * np.cos(t0) + c0y + y0 for ti in t] 
                     
                     interpolated_points = list(zip(x_coords,y_coords))
 
                 
@@ -1132,21 +1132,21 @@
                 else:
                     # construct a circle with center point x0, y0 
                     # through xi,yi 
 
                     c0x = 0.5*(xi-x0)
                     c0y = 0.5*(yi-y0) 
 
-                    r = 0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) 
+                    rx = max(3,0.5 * np.sqrt((x0-xi)**2 + (y0-yi)**2) )
+                    ry = max(3,0.5 * np.sqrt((xi-xd)**2 + (yi-yd)**2) )
                     
                     t0 = np.arctan2((yi-y0) ,(xi-x0))
 
                     t = t0 + np.linspace(0,2*np.pi, 100)
-                    rx = r 
-                    ry = 0.7*r 
+                    
 
                     x_coords = [rx * np.cos(ti) * np.cos(t0) - ry * np.sin(ti) * np.sin(t0) + c0x + x0 for ti in t]
                     y_coords = [rx * np.cos(ti) * np.sin(t0) + ry* np.sin(ti) * np.cos(t0) + c0y + y0 for ti in t] 
                     
                     
                     
                 interpolated_points = list(zip(x_coords,y_coords))
```

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/income_viewer.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/income_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/mainloop_editor.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/mainloop_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/mamba_interpreter2.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/mamba_interpreter2.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/matrix_viewer.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/matrix_viewer.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/output_display.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/output_display.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/output_display.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/pandasmodel.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/qtattune.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/qtattune.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/resources.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/resources.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/search_dialog.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/search_dialog.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/settings_edit.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/settings_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/simulation_edit.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/simulation_edit.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/bright/main.txt` & `sfctools-1.0.6.0/sfctools/gui/attune/src/styles/bright/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/background.txt` & `sfctools-1.0.6.0/sfctools/gui/attune/src/styles/dark/background.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/styles/dark/main.txt` & `sfctools-1.0.6.0/sfctools/gui/attune/src/styles/dark/main.txt`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/theme_manager.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/theme_manager.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/transaction_designer_mainwindow.ui` & `sfctools-1.0.6.0/sfctools/gui/attune/src/transaction_designer_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/attune/src/yaml_editor.py` & `sfctools-1.0.6.0/sfctools/gui/attune/src/yaml_editor.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/CLA.pdf` & `sfctools-1.0.6.0/sfctools/gui/CLA.pdf`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/CONTRIBUTING.md` & `sfctools-1.0.6.0/sfctools/gui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/LICENSE` & `sfctools-1.0.6.0/sfctools/gui/LICENSE`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/gui/README.md` & `sfctools-1.0.6.0/sfctools/gui/README.md`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/MAMBA/__pycache__/mamba_interpreter2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/misc/__pycache__/mpl_plotting.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/misc/__pycache__/reporting_sheet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/misc/__pycache__/reporting_sheet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-311.pyc` & `sfctools-1.0.6.0/sfctools/misc/__pycache__/timeseries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/__pycache__/timeseries.cpython-38.pyc` & `sfctools-1.0.6.0/sfctools/misc/__pycache__/timeseries.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/mpl_plotting.py` & `sfctools-1.0.6.0/sfctools/misc/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/reporting_sheet.py` & `sfctools-1.0.6.0/sfctools/misc/reporting_sheet.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/sfctools/misc/timeseries.py` & `sfctools-1.0.6.0/sfctools/misc/timeseries.py`

 * *Files identical despite different names*

### Comparing `sfctools-1.0.5.9/setup.py` & `sfctools-1.0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
  'scipy>1.9.1',
  'seaborn',
  'setuptools>=50.0.0',
  'sympy>=1.10.0']
 
 setup_kwargs = {
     'name': 'sfctools',
-    'version': '1.0.5.9',
+    'version': '1.0.6.0',
     'description': 'Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.',
     'long_description': '# sfctools - A toolbox for stock-flow consistent, agent-based models\n\nSfctools is a lightweight and easy-to-use Python framework for agent-based macroeconomic, stock-flow consistent (ABM-SFC) modeling. It concentrates on agents in economics and helps you to construct agents, helps you to manage and document your model parameters, assures stock-flow consistency, and facilitates basic economic data structures (such as the balance sheet).\n\n\n## Installation\n\nWe recommend to install sfctools in a fresh Python 3.8 environment. For example, with conda, do\n\n    conda create --name sfcenv python=3.8\n    conda activate sfcenv\n    conda install pip\n\nThen, in a terminal of your choice, type:\n\n    pip install sfctools\n\nsee https://pypi.org/project/sfctools/\n\n## Usage with Graphical User Interface \'Attune\'\n\nType\n\n    python -m sfctools attune\n\nto start the GUI.\n\n## Usage inside Python\n\n```console\nfrom sfctools import Agent,World\nclass MyAgent(Agent):\n    def __init__(self, a):\n        super().__init__(self)\n        self.some_attribute = a\nmy_agent = MyAgent()\nprint(my_agent)\nprint(World().get_agents_of_type("MyAgent"))\n```\n\n## Running examples\n\n\n\n\n| Author Thomas Baldauf, German Aerospace Center (DLR), Curiestr. 4 70563 Stuttgart | thomas.baldauf@dlr.de |\n',
     'author': 'Thomas Baldauf',
     'author_email': 'thomas.baldauf@dlr.de',
     'maintainer': 'Thomas Baldauf, Benjamin Fuchs',
     'maintainer_email': 'thomas.baldauf@dlr.de, benjamin.fuchs@dlr.de',
     'url': 'https://gitlab.com/dlr-ve/esy/sfctools/framework',
```

### Comparing `sfctools-1.0.5.9/PKG-INFO` & `sfctools-1.0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfctools
-Version: 1.0.5.9
+Version: 1.0.6.0
 Summary: Framework for stock-flow consistent agent-based modeling, being developed at the German Aerospace Center (DLR) for and in the scientific context of energy systems analysis, however, it is widely applicable in other scientific fields.
 Home-page: https://gitlab.com/dlr-ve/esy/sfctools/framework
 License: MIT
 Keywords: stock-flow-consistent,agent-based,agent,macroeconomics,computational economics
 Author: Thomas Baldauf
 Author-email: thomas.baldauf@dlr.de
 Maintainer: Thomas Baldauf, Benjamin Fuchs
```

