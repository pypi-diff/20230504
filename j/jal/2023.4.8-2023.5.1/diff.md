# Comparing `tmp/jal-2023.4.8.tar.gz` & `tmp/jal-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jal-2023.4.8.tar", last modified: Sun Apr 23 12:20:32 2023, max compression
+gzip compressed data, was "jal-2023.5.1.tar", last modified: Thu May  4 21:56:30 2023, max compression
```

## Comparing `jal-2023.4.8.tar` & `jal-2023.5.1.tar`

### file list

```diff
@@ -1,218 +1,221 @@
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.026746 jal-2023.4.8/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.4.8/MANIFEST.in
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-23 12:20:32.026746 jal-2023.4.8/PKG-INFO
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.833411 jal-2023.4.8/docs/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-04-15 14:23:01.000000 jal-2023.4.8/docs/README.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.836744 jal-2023.4.8/jal/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-04-23 12:17:50.000000 jal-2023.4.8/jal/__init__.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3831 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/constants.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.843411 jal-2023.4.8/jal/data_export/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/data_export/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_export/dlsg.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.846744 jal-2023.4.8/jal/data_export/tax_reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/data_export/tax_reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/tax_reports/portugal.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.4.8/jal/data_export/tax_reports/portugal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/tax_reports/russia.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_export/tax_reports/russia.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/taxes.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/taxes_flow.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.860078 jal-2023.4.8/jal/data_export/templates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/templates/tax_prt_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/data_export/templates/tax_prt_shares.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_bonds.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_corporate_actions.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_crypto.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_derivatives.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_dividends.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_fees.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_flow.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_interests.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.4.8/jal/data_export/templates/tax_rus_trades.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.4.8/jal/data_export/xlsx.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.870078 jal-2023.4.8/jal/data_import/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/data_import/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.876744 jal-2023.4.8/jal/data_import/broker_statements/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.4.8/jal/data_import/broker_statements/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    65337 2023-04-21 18:16:02.000000 jal-2023.4.8/jal/data_import/broker_statements/ibkr.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19903 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/data_import/broker_statements/just2trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/data_import/broker_statements/kit.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.4.8/jal/data_import/broker_statements/open_portfolio.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    31284 2023-04-22 15:56:59.000000 jal-2023.4.8/jal/data_import/broker_statements/openbroker.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.4.8/jal/data_import/broker_statements/psb.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27485 2023-04-20 18:05:58.000000 jal-2023.4.8/jal/data_import/broker_statements/uralsib.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.4.8/jal/data_import/category_recognizer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/data_import/import_schema.json
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/data_import/slips.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/data_import/slips_tax.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35873 2023-04-22 16:02:25.000000 jal-2023.4.8/jal/data_import/statement.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.4.8/jal/data_import/statement_xls.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6950 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/data_import/statement_xml.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3224 2023-04-08 19:50:05.000000 jal-2023.4.8/jal/data_import/statements.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.896745 jal-2023.4.8/jal/db/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/db/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.4.8/jal/db/account.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21487 2023-04-14 11:26:23.000000 jal-2023.4.8/jal/db/asset.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.4.8/jal/db/backup_restore.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.4.8/jal/db/balances_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.4.8/jal/db/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/db/closed_trade.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.4.8/jal/db/country.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    18652 2023-04-15 13:39:15.000000 jal-2023.4.8/jal/db/db.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.4.8/jal/db/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15989 2023-04-14 11:27:05.000000 jal-2023.4.8/jal/db/holdings_model.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/db/ledger.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/db/operations.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7461 2023-04-20 16:47:43.000000 jal-2023.4.8/jal/db/operations_model.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.4.8/jal/db/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-04-15 13:54:08.000000 jal-2023.4.8/jal/db/reference_models.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1190 2023-01-06 21:49:49.000000 jal-2023.4.8/jal/db/settings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      438 2023-02-16 17:12:29.000000 jal-2023.4.8/jal/db/tag.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/db/tax_estimator.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.4.8/jal/db/view_model.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.920078 jal-2023.4.8/jal/img/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/accept.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/add.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/add_child.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/img/broom.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/cancel.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.4.8/jal/img/chart.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/copy.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/delete.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/ibkr.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.4.8/jal/img/j2t.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/img/jal.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.4.8/jal/img/kit.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.4.8/jal/img/list.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/img/meatballs.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/new.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.4.8/jal/img/open_portfolio.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/img/openbroker.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.4.8/jal/img/psb.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/quik.ico
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/reconcile.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.4.8/jal/img/remove.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.4.8/jal/img/tax.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.4.8/jal/img/uralsib.ico
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-01-19 12:05:21.000000 jal-2023.4.8/jal/jal.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91499 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/jal_init.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.923411 jal-2023.4.8/jal/languages/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.4.8/jal/languages/en.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/languages/en.qm
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.4.8/jal/languages/ru.png
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    87966 2023-04-20 18:09:17.000000 jal-2023.4.8/jal/languages/ru.qm
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.926745 jal-2023.4.8/jal/net/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.4.8/jal/net/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    25047 2023-04-22 15:07:28.000000 jal-2023.4.8/jal/net/downloader.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.4.8/jal/net/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.4.8/jal/pypi_description.md
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.936745 jal-2023.4.8/jal/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/category.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14386 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/deals.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3936 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/holdings.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17557 2023-04-16 16:12:41.000000 jal-2023.4.8/jal/reports/income_spending.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/peer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2023-04-16 16:04:35.000000 jal-2023.4.8/jal/reports/profit_loss.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3287 2023-02-16 10:22:14.000000 jal-2023.4.8/jal/reports/reports.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/reports/tag.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.946745 jal-2023.4.8/jal/ui/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/ui/__init__.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.956745 jal-2023.4.8/jal/ui/reports/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/ui/reports/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_category_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4099 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_deals_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4159 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_holdings_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4954 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_income_spending_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_peer_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_profit_loss_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_tag_report.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/reports/ui_tax_estimation.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_asset_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_flow_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_login_fns_dlg.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9324 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_operations_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_rebuild_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_reference_data_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_select_account_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_select_reference_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_slip_import_dlg.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_tax_export_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-04-20 18:08:23.000000 jal-2023.4.8/jal/ui/ui_update_quotes_window.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.996745 jal-2023.4.8/jal/updates/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/updates/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.4.8/jal/updates/jal_delta_10.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.4.8/jal/updates/jal_delta_11.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.4.8/jal/updates/jal_delta_12.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.4.8/jal/updates/jal_delta_13.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_14.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_15.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_16.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.4.8/jal/updates/jal_delta_17.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.4.8/jal/updates/jal_delta_18.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.4.8/jal/updates/jal_delta_19.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.4.8/jal/updates/jal_delta_20.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.4.8/jal/updates/jal_delta_21.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.4.8/jal/updates/jal_delta_22.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.4.8/jal/updates/jal_delta_23.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.4.8/jal/updates/jal_delta_24.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.4.8/jal/updates/jal_delta_25.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.4.8/jal/updates/jal_delta_26.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.4.8/jal/updates/jal_delta_27.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.4.8/jal/updates/jal_delta_28.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.4.8/jal/updates/jal_delta_29.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.4.8/jal/updates/jal_delta_30.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.4.8/jal/updates/jal_delta_31.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.4.8/jal/updates/jal_delta_32.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.4.8/jal/updates/jal_delta_33.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.4.8/jal/updates/jal_delta_34.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.4.8/jal/updates/jal_delta_35.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.4.8/jal/updates/jal_delta_36.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.4.8/jal/updates/jal_delta_37.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.4.8/jal/updates/jal_delta_38.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.4.8/jal/updates/jal_delta_39.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.4.8/jal/updates/jal_delta_40.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.4.8/jal/updates/jal_delta_41.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.4.8/jal/updates/jal_delta_42.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.4.8/jal/updates/jal_delta_43.sql
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.4.8/jal/updates/jal_delta_44.sql
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.020079 jal-2023.4.8/jal/widgets/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.4.8/jal/widgets/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-04-15 09:01:12.000000 jal-2023.4.8/jal/widgets/abstract_operation_details.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/account_select.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14491 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/asset_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/corporate_action_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:32.026746 jal-2023.4.8/jal/widgets/custom/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.4.8/jal/widgets/custom/__init__.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2023-04-20 16:58:35.000000 jal-2023.4.8/jal/widgets/custom/date_range_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/custom/db_lookup_combobox.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5874 2023-04-20 16:38:19.000000 jal-2023.4.8/jal/widgets/custom/log_viewer.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/delegates.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/dividend_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10438 2023-04-16 16:04:35.000000 jal-2023.4.8/jal/widgets/helpers.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/income_spending_widget.py
--rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13018 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/main_window.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/mdi.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.4.8/jal/widgets/operations_tabs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/operations_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/price_chart.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/qr_scanner.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/reference_data.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-04-15 13:54:08.000000 jal-2023.4.8/jal/widgets/reference_dialogs.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/reference_selector.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.4.8/jal/widgets/register_designer_plugins.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-04-15 14:14:41.000000 jal-2023.4.8/jal/widgets/selection_dialog.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7862 2023-04-14 18:14:21.000000 jal-2023.4.8/jal/widgets/tax_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/trade_widget.py
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-04-15 14:13:28.000000 jal-2023.4.8/jal/widgets/transfer_widget.py
-drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-04-23 12:20:31.840077 jal-2023.4.8/jal.egg-info/
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/PKG-INFO
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5592 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/SOURCES.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/dependency_links.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/entry_points.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/requires.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-04-23 12:20:31.000000 jal-2023.4.8/jal.egg-info/top_level.txt
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-04-23 12:20:32.026746 jal-2023.4.8/setup.cfg
--rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-04-14 18:14:21.000000 jal-2023.4.8/setup.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.509734 jal-2023.5.1/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      176 2022-01-13 06:08:45.000000 jal-2023.5.1/MANIFEST.in
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-05-04 21:56:30.509734 jal-2023.5.1/PKG-INFO
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.476401 jal-2023.5.1/docs/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7580 2023-05-03 13:22:40.000000 jal-2023.5.1/docs/README.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.476401 jal-2023.5.1/jal/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       24 2023-05-04 21:52:22.000000 jal-2023.5.1/jal/__init__.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3843 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/constants.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.476401 jal-2023.5.1/jal/data_export/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2022-01-13 15:45:51.000000 jal-2023.5.1/jal/data_export/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19856 2023-04-14 11:26:23.000000 jal-2023.5.1/jal/data_export/dlsg.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.479734 jal-2023.5.1/jal/data_export/tax_reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/data_export/tax_reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      990 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/tax_reports/portugal.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7089 2023-02-08 10:00:47.000000 jal-2023.5.1/jal/data_export/tax_reports/portugal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1532 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/tax_reports/russia.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    38366 2023-04-14 11:26:23.000000 jal-2023.5.1/jal/data_export/tax_reports/russia.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6433 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/taxes.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5299 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/taxes_flow.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.483067 jal-2023.5.1/jal/data_export/templates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-30 08:37:57.000000 jal-2023.5.1/jal/data_export/templates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1286 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/templates/tax_prt_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2594 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/data_export/templates/tax_prt_shares.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6163 2022-01-30 08:37:57.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_bonds.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4792 2022-02-13 11:04:18.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_corporate_actions.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4938 2022-04-30 20:05:13.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_crypto.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4948 2022-04-30 20:05:13.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_derivatives.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3249 2022-02-13 11:04:18.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_dividends.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1450 2022-01-30 08:37:57.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_fees.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1133 2022-06-19 17:39:33.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_flow.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1654 2022-07-20 07:00:10.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_interests.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5303 2022-01-30 08:37:57.000000 jal-2023.5.1/jal/data_export/templates/tax_rus_trades.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10842 2023-02-08 13:35:53.000000 jal-2023.5.1/jal/data_export/xlsx.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.483067 jal-2023.5.1/jal/data_import/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/data_import/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.483067 jal-2023.5.1/jal/data_import/broker_statements/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-22 16:32:16.000000 jal-2023.5.1/jal/data_import/broker_statements/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    66265 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/broker_statements/ibkr.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20214 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/broker_statements/just2trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9470 2022-08-21 07:15:06.000000 jal-2023.5.1/jal/data_import/broker_statements/kit.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5857 2023-02-14 12:14:19.000000 jal-2023.5.1/jal/data_import/broker_statements/open_portfolio.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    31284 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/broker_statements/openbroker.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15460 2022-12-07 21:59:21.000000 jal-2023.5.1/jal/data_import/broker_statements/psb.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    27485 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/broker_statements/uralsib.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     3893 2023-03-05 19:06:08.000000 jal-2023.5.1/jal/data_import/category_recognizer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      543 2021-08-05 15:24:10.000000 jal-2023.5.1/jal/data_import/import_schema.json
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15598 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/slips.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13145 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/slips_tax.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    36120 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/statement.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11314 2023-02-02 08:45:14.000000 jal-2023.5.1/jal/data_import/statement_xls.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6984 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/data_import/statement_xml.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3983 2023-05-03 15:42:34.000000 jal-2023.5.1/jal/data_import/statements.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.486401 jal-2023.5.1/jal/db/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/db/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17607 2023-02-27 16:25:45.000000 jal-2023.5.1/jal/db/account.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21761 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/db/asset.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     6074 2022-12-06 18:30:39.000000 jal-2023.5.1/jal/db/backup_restore.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7360 2023-02-27 17:48:37.000000 jal-2023.5.1/jal/db/balances_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4103 2023-02-27 16:03:46.000000 jal-2023.5.1/jal/db/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5218 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/db/closed_trade.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2399 2023-03-08 17:11:23.000000 jal-2023.5.1/jal/db/country.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    19123 2023-05-03 17:19:23.000000 jal-2023.5.1/jal/db/db.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3941 2023-04-12 09:44:25.000000 jal-2023.5.1/jal/db/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14901 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/db/holdings_model.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    16683 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/db/ledger.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    60565 2023-04-07 14:10:37.000000 jal-2023.5.1/jal/db/operations.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7461 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/db/operations_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3379 2023-02-20 16:05:40.000000 jal-2023.5.1/jal/db/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15204 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/db/reference_models.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2115 2023-05-03 17:19:23.000000 jal-2023.5.1/jal/db/settings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1420 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/db/tag.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6777 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/db/tax_estimator.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9785 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/db/trades_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5241 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/db/tree_model.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1458 2023-02-23 19:54:06.000000 jal-2023.5.1/jal/db/view_model.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.489734 jal-2023.5.1/jal/img/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2922 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/accept.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1443 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/add.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2049 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/add_child.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      435 2022-04-25 10:26:48.000000 jal-2023.5.1/jal/img/broom.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4004 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/cancel.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      806 2023-03-08 16:58:09.000000 jal-2023.5.1/jal/img/chart.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      898 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/copy.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2812 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/delete.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      583 2021-03-20 12:52:05.000000 jal-2023.5.1/jal/img/ibkr.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2340 2022-04-29 07:05:21.000000 jal-2023.5.1/jal/img/j2t.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5563 2022-01-13 06:08:45.000000 jal-2023.5.1/jal/img/jal.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1516 2021-03-22 11:20:31.000000 jal-2023.5.1/jal/img/kit.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1163 2022-12-28 10:47:37.000000 jal-2023.5.1/jal/img/list.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      342 2022-04-25 10:26:48.000000 jal-2023.5.1/jal/img/meatballs.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      611 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/new.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1175 2022-07-10 15:39:56.000000 jal-2023.5.1/jal/img/open_portfolio.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15086 2021-08-05 15:24:10.000000 jal-2023.5.1/jal/img/openbroker.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-08-05 15:24:10.000000 jal-2023.5.1/jal/img/psb.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1150 2021-03-20 12:52:05.000000 jal-2023.5.1/jal/img/quik.ico
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2651 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/reconcile.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      822 2021-05-26 12:51:46.000000 jal-2023.5.1/jal/img/remove.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1874 2023-03-08 16:53:42.000000 jal-2023.5.1/jal/img/tax.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1406 2021-03-20 12:52:05.000000 jal-2023.5.1/jal/img/uralsib.ico
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     1938 2023-05-02 18:03:03.000000 jal-2023.5.1/jal/jal.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    91725 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/jal_init.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.489734 jal-2023.5.1/jal/languages/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      424 2020-12-21 16:23:10.000000 jal-2023.5.1/jal/languages/en.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    32025 2022-01-13 06:08:45.000000 jal-2023.5.1/jal/languages/en.qm
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      287 2022-04-25 10:26:48.000000 jal-2023.5.1/jal/languages/ru.png
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    89942 2023-05-04 21:51:42.000000 jal-2023.5.1/jal/languages/ru.qm
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.489734 jal-2023.5.1/jal/net/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2021-08-17 15:15:47.000000 jal-2023.5.1/jal/net/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    25047 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/net/downloader.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2912 2023-01-27 21:53:46.000000 jal-2023.5.1/jal/net/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2040 2023-03-06 11:34:17.000000 jal-2023.5.1/jal/pypi_description.md
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.489734 jal-2023.5.1/jal/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2967 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/reports/category.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2363 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/reports/deals.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5116 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/reports/holdings.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17557 2023-05-03 13:22:52.000000 jal-2023.5.1/jal/reports/income_spending.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2855 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/reports/peer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8772 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/reports/profit_loss.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3477 2023-05-03 15:42:34.000000 jal-2023.5.1/jal/reports/reports.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2827 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/reports/tag.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.493067 jal-2023.5.1/jal/ui/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/ui/__init__.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.493067 jal-2023.5.1/jal/ui/reports/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-01-13 15:45:51.000000 jal-2023.5.1/jal/ui/reports/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5179 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_category_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4389 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_deals_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4603 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_holdings_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4954 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_income_spending_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5382 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_peer_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4687 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_profit_loss_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5353 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_tag_report.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4805 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/reports/ui_tax_estimation.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12742 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_asset_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4056 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_flow_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14782 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_login_fns_dlg.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     9633 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    14510 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_operations_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)     5707 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_rebuild_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7302 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_reference_data_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2903 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_select_account_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3253 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_select_reference_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16301 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_slip_import_dlg.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9674 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_tax_export_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4023 2023-05-04 21:50:35.000000 jal-2023.5.1/jal/ui/ui_update_quotes_window.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.506401 jal-2023.5.1/jal/updates/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/updates/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5122 2020-12-21 16:23:10.000000 jal-2023.5.1/jal/updates/jal_delta_10.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12870 2021-08-18 12:53:40.000000 jal-2023.5.1/jal/updates/jal_delta_11.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26116 2021-01-13 17:04:46.000000 jal-2023.5.1/jal/updates/jal_delta_12.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    16516 2021-01-30 16:01:43.000000 jal-2023.5.1/jal/updates/jal_delta_13.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    34961 2021-02-27 17:35:02.000000 jal-2023.5.1/jal/updates/jal_delta_14.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2250 2021-02-27 17:35:02.000000 jal-2023.5.1/jal/updates/jal_delta_15.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3630 2021-02-27 17:35:02.000000 jal-2023.5.1/jal/updates/jal_delta_16.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    20912 2021-02-27 17:35:02.000000 jal-2023.5.1/jal/updates/jal_delta_17.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      656 2021-03-07 11:58:53.000000 jal-2023.5.1/jal/updates/jal_delta_18.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      686 2021-03-08 13:39:11.000000 jal-2023.5.1/jal/updates/jal_delta_19.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13578 2021-03-12 14:26:01.000000 jal-2023.5.1/jal/updates/jal_delta_20.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1428 2021-03-19 12:24:53.000000 jal-2023.5.1/jal/updates/jal_delta_21.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      949 2021-03-22 11:20:31.000000 jal-2023.5.1/jal/updates/jal_delta_22.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    17602 2021-04-08 12:12:36.000000 jal-2023.5.1/jal/updates/jal_delta_23.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      344 2021-04-11 10:57:46.000000 jal-2023.5.1/jal/updates/jal_delta_24.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8270 2021-04-22 04:11:28.000000 jal-2023.5.1/jal/updates/jal_delta_25.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2492 2021-08-12 19:15:12.000000 jal-2023.5.1/jal/updates/jal_delta_26.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    26325 2022-01-13 05:57:31.000000 jal-2023.5.1/jal/updates/jal_delta_27.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13276 2022-01-13 06:08:45.000000 jal-2023.5.1/jal/updates/jal_delta_28.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    35370 2022-01-13 15:45:51.000000 jal-2023.5.1/jal/updates/jal_delta_29.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8671 2022-02-13 13:11:58.000000 jal-2023.5.1/jal/updates/jal_delta_30.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11413 2022-02-13 11:04:18.000000 jal-2023.5.1/jal/updates/jal_delta_31.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12545 2022-03-31 14:26:11.000000 jal-2023.5.1/jal/updates/jal_delta_32.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4229 2022-03-31 14:26:11.000000 jal-2023.5.1/jal/updates/jal_delta_33.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2287 2022-04-06 14:47:21.000000 jal-2023.5.1/jal/updates/jal_delta_34.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2858 2022-04-30 20:05:13.000000 jal-2023.5.1/jal/updates/jal_delta_35.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3427 2022-06-19 17:39:33.000000 jal-2023.5.1/jal/updates/jal_delta_36.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3755 2022-07-20 07:00:10.000000 jal-2023.5.1/jal/updates/jal_delta_37.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21913 2022-08-21 07:15:06.000000 jal-2023.5.1/jal/updates/jal_delta_38.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      343 2023-01-04 13:14:35.000000 jal-2023.5.1/jal/updates/jal_delta_39.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3055 2023-01-27 21:53:46.000000 jal-2023.5.1/jal/updates/jal_delta_40.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    48157 2023-02-07 18:26:24.000000 jal-2023.5.1/jal/updates/jal_delta_41.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2085 2023-02-20 14:55:36.000000 jal-2023.5.1/jal/updates/jal_delta_42.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2528 2023-03-08 16:23:30.000000 jal-2023.5.1/jal/updates/jal_delta_43.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3020 2023-04-07 14:10:37.000000 jal-2023.5.1/jal/updates/jal_delta_44.sql
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      534 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/updates/jal_delta_45.sql
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.506401 jal-2023.5.1/jal/widgets/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       89 2020-12-23 19:03:58.000000 jal-2023.5.1/jal/widgets/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3912 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/abstract_operation_details.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6846 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/account_select.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    15191 2023-05-04 21:50:11.000000 jal-2023.5.1/jal/widgets/asset_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11302 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/corporate_action_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.509734 jal-2023.5.1/jal/widgets/custom/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        0 2022-12-24 19:32:40.000000 jal-2023.5.1/jal/widgets/custom/__init__.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4703 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/custom/date_range_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2015 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/custom/db_lookup_combobox.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5874 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/custom/log_viewer.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    13628 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/delegates.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     9289 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/dividend_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10438 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/helpers.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    12488 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/income_spending_widget.py
+-rwxr-xr-x   0 vtitov    (1000) vtitov    (1000)    13837 2023-05-03 17:19:23.000000 jal-2023.5.1/jal/widgets/main_window.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3386 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/mdi.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2854 2022-12-26 13:26:40.000000 jal-2023.5.1/jal/widgets/operations_tabs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     7159 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/operations_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6013 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/price_chart.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5667 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/qr_scanner.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    11244 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/reference_data.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    21856 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/reference_dialogs.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     4779 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/reference_selector.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)      632 2022-12-26 08:54:07.000000 jal-2023.5.1/jal/widgets/register_designer_plugins.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     3499 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/selection_dialog.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     8205 2023-05-03 15:42:34.000000 jal-2023.5.1/jal/widgets/tax_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     6890 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/trade_widget.py
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)    10088 2023-05-03 13:22:40.000000 jal-2023.5.1/jal/widgets/transfer_widget.py
+drwxr-xr-x   0 vtitov    (1000) vtitov    (1000)        0 2023-05-04 21:56:30.476401 jal-2023.5.1/jal.egg-info/
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     2726 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/PKG-INFO
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     5665 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/SOURCES.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)        1 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/dependency_links.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       37 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/entry_points.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       67 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/requires.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       10 2023-05-04 21:56:30.000000 jal-2023.5.1/jal.egg-info/top_level.txt
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)       38 2023-05-04 21:56:30.509734 jal-2023.5.1/setup.cfg
+-rw-r--r--   0 vtitov    (1000) vtitov    (1000)     1756 2023-05-03 13:22:40.000000 jal-2023.5.1/setup.py
```

### Comparing `jal-2023.4.8/PKG-INFO` & `jal-2023.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.8
+Version: 2023.5.1
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.8/docs/README.md` & `jal-2023.5.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/constants.py` & `jal-2023.5.1/jal/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QApplication, QComboBox
 
 
 class Setup:
     DB_PATH = "jal.sqlite"
     DB_CONNECTION = "JAL.DB"
-    DB_REQUIRED_VERSION = 44
+    DB_REQUIRED_VERSION = 45
     SQLITE_MIN_VERSION = "3.35"
     MAIN_WND_NAME = "JAL_MainWindow"
     INIT_SCRIPT_PATH = 'jal_init.sql'
     UPDATES_PATH = 'updates'
     ICONS_PATH = "img"
     IMPORT_PATH = "data_import"
     EXPORT_PATH = "data_export"
@@ -115,14 +115,15 @@
         return QApplication.translate("AssetType", text)
 
 
 class AssetData:
     RegistrationCode = 1
     ExpiryDate = 2
     PrincipalValue = 3
+    Tag = 4
 
 
 class PredefinedPeer:
     Financial = 1
 
 
 class MarketDataFeed:
```

### Comparing `jal-2023.4.8/jal/data_export/dlsg.py` & `jal-2023.5.1/jal/data_export/dlsg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/tax_reports/portugal.json` & `jal-2023.5.1/jal/data_export/tax_reports/portugal.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/tax_reports/portugal.py` & `jal-2023.5.1/jal/data_export/tax_reports/portugal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/tax_reports/russia.json` & `jal-2023.5.1/jal/data_export/tax_reports/russia.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/tax_reports/russia.py` & `jal-2023.5.1/jal/data_export/tax_reports/russia.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/taxes.py` & `jal-2023.5.1/jal/data_export/taxes.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/taxes_flow.py` & `jal-2023.5.1/jal/data_export/taxes_flow.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_prt_dividends.json` & `jal-2023.5.1/jal/data_export/templates/tax_prt_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_prt_shares.json` & `jal-2023.5.1/jal/data_export/templates/tax_prt_shares.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_bonds.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_bonds.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_corporate_actions.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_corporate_actions.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_crypto.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_crypto.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_derivatives.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_derivatives.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_dividends.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_dividends.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_fees.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_fees.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_flow.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_flow.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_interests.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_interests.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/templates/tax_rus_trades.json` & `jal-2023.5.1/jal/data_export/templates/tax_rus_trades.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_export/xlsx.py` & `jal-2023.5.1/jal/data_export/xlsx.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/ibkr.py` & `jal-2023.5.1/jal/data_import/broker_statements/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from PySide6.QtWidgets import QApplication
 from jal.constants import PredefinedCategory
 from jal.widgets.helpers import ManipulateDate, ts2dt, ts2d
 from jal.db.helpers import format_decimal
 from jal.db.account import JalAccount
 from jal.db.operations import Dividend
-from jal.data_import.statement import FOF, Statement_ImportError
+from jal.data_import.statement import FOF, Statement_ImportError, Statement_Capabilities
 from jal.data_import.statement_xml import StatementXML
 
 JAL_STATEMENT_CLASS = "StatementIBKR"
 IBKR_CALCULATION_PRECISION = 10
 DIVIDENDS_TABLE_ASSET_FIELD = 7
 
 # -----------------------------------------------------------------------------------------------------------------------
@@ -267,16 +267,21 @@
                                       ('date', 'timestamp', datetime, None),
                                       ('total', 'amount', float, None),
                                       ('transactionID', 'number', str, ''),
                                       ('activityDescription', 'description', str, None)],
                            'loader': self.load_cfd_charges},
         }
 
-    def tr(self, text):
-        return QApplication.translate("IBKR", text)
+    @staticmethod
+    def tr(text):
+        return QApplication.translate("StatementIBKR", text)
+
+    @staticmethod
+    def capabilities() -> set:
+        return {Statement_Capabilities.MULTIPLE_LOAD}
 
     # Saves information from XML that is related with a given asset
     def save_debug_info(self, account, asset):
         # Dump statement info relevant to given asset
         debug_info = 'Statement data:\n----------------------------------------------------------------\n'
         assert self._statement is not None
         symbols = [x['symbol'] for x in self._data[FOF.SYMBOLS] if x["asset"] == asset]
@@ -314,17 +319,14 @@
         return IBKR_AssetType(xml_element.attrib[attr_name], sub_type).type
 
     # Convert attribute 'attr_name' value into JAL corporate action
     def attr_corp_action_type(self, xml_element, attr_name, default_value):
         if attr_name not in xml_element.attrib:
             return default_value
         asset_category = self.attr_asset_type(xml_element, 'assetCategory', None)
-        if asset_category not in [FOF.ASSET_STOCK, FOF.ASSET_BOND, FOF.ASSET_WARRANT, FOF.ASSET_CFD]:
-            logging.error(self.tr("Corporate action isn't supported for asset type: ") + f"'{asset_category}'")
-            return default_value
         return IBKR_CorpActionType(xml_element.attrib[attr_name]).type
 
     def attr_currency(self, xml_element, attr_name, default_value):
         if attr_name not in xml_element.attrib:
             return default_value
         currency_id = self.currency_id(xml_element.attrib[attr_name])
         if currency_id is None:
@@ -1103,7 +1105,31 @@
 
     # Removes data that was used during XML processing but isn't needed in final output:
     # Drop any assets with type 'right' as JAL won't import them
     def strip_unused_data(self):
         rights_id = [x['id'] for x in self._data[FOF.ASSETS] if x['type'] == FOF.ASSET_RIGHTS]
         for asset_id in rights_id:
             self.remove_asset(asset_id)
+
+    # -----------------------------------------------------------------------------------------------------------------------
+    @staticmethod
+    def order_statements(statementFiles) -> list:
+        READ_COUNT=1024
+        pattern = re.compile(r'<FlexStatement.*fromDate=\"([0-9]*)\"\stoDate=\"([0-9]*)\".*>')
+        files = []
+        for file in statementFiles:
+            with open(file) as f:
+                m = re.search(pattern, f.read(READ_COUNT))
+                if not m:
+                    logging.error(StatementIBKR.tr("Can't find a FlexStatement in first {} bytes of {}").format(READ_COUNT,file))
+                    return []
+                start = int(m.group(1))
+                end = int(m.group(2))
+                item = [start, end, file]
+                idx = 0
+                for i in files:
+                    if item[1] <= i[0]:
+                        break
+                    idx += 1
+                files.insert(idx, item)
+                f.close()
+        return [x[2] for x in files]
```

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/just2trade.py` & `jal-2023.5.1/jal/data_import/broker_statements/just2trade.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from jal.db.asset import JalAsset
 
 JAL_STATEMENT_CLASS = "StatementJ2T"
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class StatementJ2T(StatementXLS):
-    PeriodPattern = (1, 0, r"Отчет по счету клиента за период с (?P<S>\d\d\.\d\d\.\d\d\d\d) по (?P<E>\d\d\.\d\d\.\d\d\d\d)")
+    PeriodPattern = (1, 0, r"Report by Client Accounts over a Period from (?P<S>\d\d\.\d\d\.\d\d\d\d) to (?P<E>\d\d\.\d\d\.\d\d\d\d)")
     AccountPattern = (5, 4, r"(?P<ACCOUNT>\S*)\\.*")
     HeaderCol = 1
     money_section = "ДС на конец периода"
     money_columns = {
         "settled_end": "Сумма",
         "bonus": "Бонус",
         "currency": "Валюта"
     }
     asset_section = "Открытые позиции на конец периода"
     asset_columns = {
-        "name": "Наименование инструмента",
+        "name": "Instrument description \(Название инструмента\)",
         "isin": "ISIN",
-        "symbol": "Symbol",
-        "currency": "Валюта инструмента"
+        "symbol": "Symbol \(Символ\)",
+        "currency": "Instrument сurrency \(валюта инструмента\)"
     }
 
     def __init__(self):
         super().__init__()
         self.name = self.tr("Just2Trade")
         self.icon_name = "j2t.png"
         self.filename_filter = self.tr("Just2Trade statement (*.xlsx)")
@@ -144,24 +144,24 @@
             cnt += 1
             row += 1
         logging.info(self.tr("Stock trades loaded: ") + f"{cnt}")
 
     def _load_crypto_deals(self):
         cnt = 0
         columns = {
-            "number": "Номер сделки",
-            "timestamp": "Дата сделки",
-            "settlement": "Дата расчетов",
-            "account_currency": "Валюта счета",
+            "number": "Trade number \(Номер сделки\)",
+            "timestamp": "Trade date \(Дата сделки\)",
+            "settlement": "Settle date \(дата расчетов\)",
+            "account_currency": "Account currency \(Валюта счета\)",
             "asset_name": "Description",
-            "B/S": "Тип сделки",
-            "qty": "Кол-во",
-            "fee": "комиссия брокера в валюте счета",
-            "amount": "Итого в валюте счета",
-            "fee_ex": "Прочие комиссии в валюте счета"
+            "B/S": "Type of Transaction\(Тип сделки\)",
+            "qty": "Quantity \(Кол-во\)",
+            "fee": "Broker fees in account currency \(комиссия брокера в валюте счета\)",
+            "amount": "Net Value in account currency \(Итого в валюте счета\)",
+            "fee_ex": "Other fees in account currency \(прочие комиссии в валюте счета\)"
         }
 
         row, headers = self.find_section_start("Сделки c виртуальными \(крипто\) инструментами", columns,
                                                header_height=3)
         if row < 0:
             return
         while row < self._statement.shape[0]:
@@ -215,15 +215,16 @@
             '': None,
             'Переоценка': None,
             'Корпоративные действия::Дивиденды': self.dividend,
             'Внешние затраты::Комиссия внешнего брокера::Удержанный налог': None,  # Loaded in 2nd loop later
             'Внешние затраты::Комиссия внешнего депозитария': self.fee,
             'Перевод на ТП': self.transfer_in,
             'Списание c ТП': self.transfer_out,
-            'Корпоративные действия::Компенсации': self.skip_warning
+            'Корпоративные действия::Компенсации': self.skip_warning,
+            'Корректировка': self.skip_warning
         }
 
         start_row, headers = self.find_section_start("Движение денежных средств", columns)
         if start_row < 0:
             return
         cnt = 0
         row = start_row   # Process dividend rows
@@ -270,19 +271,19 @@
     def _find_asset_by_name(self, asset_name) -> int:
         candidates = [x for x in self._data[FOF.ASSETS] if 'name' in x and x['name'] == asset_name]
         if len(candidates) == 1:
             return candidates[0]["id"]
         asset_id = JalAsset(data={'name': asset_name}, search=True, create=False).id()
         return -asset_id  # Negative value to indicate that asset was found in db
 
-    # This methods finds dividend with given parameters in already loaded JSON data
+    # This method finds dividend with given parameters in already loaded JSON data
     def _locate_dividend(self, asset_id, timestamp, ex_date):
         for dividend in self._data[FOF.ASSET_PAYMENTS]:
             if dividend['type'] == FOF.PAYMENT_DIVIDEND and dividend['timestamp'] == timestamp and \
-                    dividend['ex-date'] == ex_date and dividend['asset'] == asset_id:
+                    dividend['ex_date'] == ex_date and dividend['asset'] == asset_id:
                 return dividend
         return None
 
     def _load_fees(self):
         cnt = 0
         columns = {
             "date": "Дата",
@@ -314,15 +315,15 @@
         dividend = parts.groupdict()
         if len(dividend) != DividendPattern.count("(?P<"):  # check that expected number of groups was matched
             raise Statement_ImportError(self.tr("Dividend description miss some data ") + f"'{note}'")
         asset_id = self._find_asset_by_name(dividend['asset'])
         ex_date = int(datetime.strptime(dividend['date'], "%d/%m/%Y").replace(tzinfo=timezone.utc).timestamp())
         new_id = max([0] + [x['id'] for x in self._data[FOF.ASSET_PAYMENTS]]) + 1
         payment = {"id": new_id, "type": FOF.PAYMENT_DIVIDEND, "account": account_id, "timestamp": timestamp,
-                   "ex-date": ex_date, "asset": asset_id, "amount": amount, "description": note}
+                   "ex_date": ex_date, "asset": asset_id, "amount": amount, "description": note}
         self._data[FOF.ASSET_PAYMENTS].append(payment)
 
     def tax(self, timestamp, amount, note):
         TaxPattern = r"Налог на дивиденды;\s+(Начисление дивидендов полученных по счету.*\.\s+)?Инструмент\s+(?P<asset>.*);\s+Дата отсечки\s+(?P<date>.*)"
         parts = re.match(TaxPattern, note, re.IGNORECASE)  # FIXME - below code used in ibkr.py as well
         if parts is None:
             raise Statement_ImportError(self.tr("Can't parse Dividend description ") + f"'{note}'")
```

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/kit.py` & `jal-2023.5.1/jal/data_import/broker_statements/kit.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/open_portfolio.py` & `jal-2023.5.1/jal/data_import/broker_statements/open_portfolio.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/openbroker.py` & `jal-2023.5.1/jal/data_import/broker_statements/openbroker.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/psb.py` & `jal-2023.5.1/jal/data_import/broker_statements/psb.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/broker_statements/uralsib.py` & `jal-2023.5.1/jal/data_import/broker_statements/uralsib.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/category_recognizer.py` & `jal-2023.5.1/jal/data_import/category_recognizer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/import_schema.json` & `jal-2023.5.1/jal/data_import/import_schema.json`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/slips.py` & `jal-2023.5.1/jal/data_import/slips.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/slips_tax.py` & `jal-2023.5.1/jal/data_import/slips_tax.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/statement.py` & `jal-2023.5.1/jal/data_import/statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         }
         return asset_types[asset_type]
 
 
 class Statement_ImportError(Exception):
     pass
 
+# Possible statement module capabilities
+class Statement_Capabilities:
+    MULTIPLE_LOAD = 1
+
 
 # -----------------------------------------------------------------------------------------------------------------------
 class Statement(QObject):   # derived from QObject to have proper string translation
     RU_PRICE_TOLERANCE = 1e-4   # TODO Probably need to switch imports to Decimal and remove it
 
     _asset_types = {
         FOF.ASSET_MONEY: PredefinedAsset.Money,
@@ -135,14 +139,19 @@
                     dump_file.write(f"JAL statement dump, {datetime.now().strftime('%y/%m/%d %H:%M:%S')}\n")
                     dump_file.write("----------------------------------------------------------------\n")
                     dump_file.write(str(kwargs['debug_info']))
                 logging.warning(self.tr("Debug information is saved in ") + dump_name)
             except Exception as e:
                 logging.error(self.tr("Failed to write statement dump into: ") + dump_name + ": " + str(e))
 
+    # Returns a specific capabilities that is supported by some statement modules
+    @staticmethod
+    def capabilities() -> set:
+        return set()
+
     # returns tuple (start_timestamp, end_timestamp)
     def period(self):
         if FOF.PERIOD in self._data:
             return self._data[FOF.PERIOD][0], self._data[FOF.PERIOD][1]
         else:
             return 0, 0
```

### Comparing `jal-2023.4.8/jal/data_import/statement_xls.py` & `jal-2023.5.1/jal/data_import/statement_xls.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/data_import/statement_xml.py` & `jal-2023.5.1/jal/data_import/statement_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     # Convert attribute 'attr_name' value to float or return default value if attribute not found / not a number
     @staticmethod
     def attr_number(xml_element, attr_name, default_value):
         if attr_name not in xml_element.attrib:
             return default_value
         try:
-            value = float(xml_element.attrib[attr_name])
+            value = float(xml_element.attrib[attr_name].replace(',', '').replace(' ', ''))
         except ValueError:
             return None
         return value
 
     # Convert attribute 'attr_name' value from strings "YYYYMMDD:hhmmss' or "YYYYMMDD" to datetime object
     # or return default value if attribute not found / has wrong format
     @staticmethod
```

### Comparing `jal-2023.4.8/jal/data_import/statements.py` & `jal-2023.5.1/jal/data_import/statements.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import os
 from collections import defaultdict
 
 from PySide6.QtCore import QObject, Signal
 from PySide6.QtWidgets import QFileDialog
 from jal.constants import Setup
 from jal.db.helpers import get_app_path
-from jal.data_import.statement import Statement_ImportError
+from jal.db.settings import JalSettings, FolderFor
+from jal.data_import.statement import Statement_ImportError, Statement_Capabilities
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 class Statements(QObject):
     load_completed = Signal(int, defaultdict)
     load_failed = Signal()
 
@@ -51,24 +52,36 @@
             })
             logging.debug(f"Class '{statement_class_name}' providing '{statement.name}' statement has been loaded")
         self.items = sorted(self.items, key=lambda item: item['name'])
 
     # method is called directly from menu, so it contains QAction that was triggered
     def load(self, action):
         statement_loader = self.items[action.data()]
-        statement_file, active_filter = QFileDialog.getOpenFileName(None, self.tr("Select statement file to import"),
-                                                                    ".", statement_loader['filename_filter'])
-        if not statement_file:
+        folder = JalSettings().getRecentFolder(FolderFor.Statement, '.')
+        statement_files, active_filter = QFileDialog.getOpenFileNames(None, self.tr("Select statement files to import"),
+                                                                      folder, statement_loader['filename_filter'])
+        if not statement_files:
             return
+        JalSettings().setRecentFolder(FolderFor.Statement, statement_files[0])
+
         module = statement_loader['module']
         class_instance = getattr(module, statement_loader['loader_class'])
-        statement = class_instance()
-        try:
-            statement.load(statement_file)
-            statement.validate_format()
-            statement.match_db_ids()
-            totals = statement.import_into_db()
-        except Statement_ImportError as e:
-            logging.error(self.tr("Import failed: ") + str(e))
-            self.load_failed.emit()
+        if len(statement_files) > 1:
+            if not Statement_Capabilities.MULTIPLE_LOAD in class_instance.capabilities():
+                logging.warning(statement_loader['name'] +
+                                self.tr(" - module doesn't support multiple statements load."))
+                return
+            statement_files = class_instance.order_statements(statement_files)
+        if not statement_files:
             return
+        for statement_file in statement_files:
+            statement = class_instance()
+            try:
+                statement.load(statement_file)
+                statement.validate_format()
+                statement.match_db_ids()
+                totals = statement.import_into_db()
+            except Statement_ImportError as e:
+                logging.error(self.tr("Import failed: ") + str(e))
+                self.load_failed.emit()
+                return
         self.load_completed.emit(statement.period()[1], totals)
```

### Comparing `jal-2023.4.8/jal/db/account.py` & `jal-2023.5.1/jal/db/account.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/asset.py` & `jal-2023.5.1/jal/db/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from decimal import Decimal, InvalidOperation
 from PySide6.QtCore import Qt, QDate
 from jal.constants import BookAccount, MarketDataFeed, AssetData, PredefinedAsset
 from jal.db.db import JalDB
 from jal.db.helpers import format_decimal, year_begin, year_end
 from jal.db.country import JalCountry
+from jal.db.tag import JalTag
 from jal.widgets.helpers import ts2d
 
 
 # Helper function to convert db timestamp string into an integer and replace it as 0 if error happens
 def db_timestamp2int(timestamp_string: str) -> int:
     try:
         timestamp = int(timestamp_string)
@@ -41,14 +42,18 @@
         self._name = self._data['full_name'] if self._data is not None else ''
         self._isin = self._data['isin'] if self._data is not None else None
         self._country = JalCountry(self._data['country_id']) if self._data is not None else JalCountry(0)
         self._reg_number = self._data.get('data', {}).get(AssetData.RegistrationCode, '') if self._data is not None else ''
         self._expiry = self._data.get('data', {}).get(AssetData.ExpiryDate, '') if self._data is not None else ''
         self._principal = self._data.get('data', {}).get(AssetData.PrincipalValue, '') if self._data is not None else ''
         self._principal = Decimal(self._principal) if self._principal else Decimal('0')
+        try:
+            self._tag = JalTag(int(self._data.get('data', {}).get(AssetData.Tag, 0)))
+        except (AttributeError, ValueError, TypeError):
+            self._tag = JalTag(0)
 
     def invalidate_cache(self):
         self._fetch_data()
 
     # JalAsset maintains single cache available for all instances
     @classmethod
     def class_cache(cls) -> True:
@@ -217,14 +222,17 @@
 
     def reg_number(self):
         return self._reg_number
 
     def principal(self) -> Decimal:
         return self._principal
 
+    def tag(self) -> JalTag:
+        return self._tag
+
     # Updates relevant asset data fields with information provided in data dictionary
     def update_data(self, data: dict) -> None:
         updaters = {
             'isin': self._update_isin,
             'name': self._update_name,
             'country': self._update_country,
             'reg_number': self._update_reg_number,
```

### Comparing `jal-2023.4.8/jal/db/backup_restore.py` & `jal-2023.5.1/jal/db/backup_restore.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/balances_model.py` & `jal-2023.5.1/jal/db/balances_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/category.py` & `jal-2023.5.1/jal/db/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/closed_trade.py` & `jal-2023.5.1/jal/db/closed_trade.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/country.py` & `jal-2023.5.1/jal/db/country.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/db.py` & `jal-2023.5.1/jal/db/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,21 @@
             return JalDBError(JalDBError.OutdatedSqlite)
         JalDB._tables = db.tables(QSql.Tables) + db.tables(QSql.Views)  # Bitwise or somehow doesn't work here :(
         if not JalDB._tables:
             logging.info("Loading DB initialization script")
             error = self.run_sql_script(db_path + Setup.INIT_SCRIPT_PATH)
             if error.code != JalDBError.NoError:
                 return error
+        if self._read("SELECT value FROM settings WHERE name='CleanDB'") == 1:
+            db.close()
+            os.remove(get_dbfilename(db_path))
+            db.open()
+            error = self.run_sql_script(db_path + Setup.INIT_SCRIPT_PATH)
+            if error.code != JalDBError.NoError:
+                return error
         schema_version = self._read("SELECT value FROM settings WHERE name='SchemaVersion'")
         if schema_version < Setup.DB_REQUIRED_VERSION:
             db.close()
             return JalDBError(JalDBError.OutdatedDbSchema)
         elif schema_version > Setup.DB_REQUIRED_VERSION:
             db.close()
             return JalDBError(JalDBError.NewerDbSchema,
@@ -144,14 +151,19 @@
         db = QSqlDatabase.database(Setup.DB_CONNECTION)
         if not db.isValid():
             raise RuntimeError(f"DB connection '{Setup.DB_CONNECTION}' is invalid")
         if not db.isOpen():
             logging.fatal(f"DB connection '{Setup.DB_CONNECTION}' is not open")
         return db
 
+    # Returns a name of current database file in use
+    @classmethod
+    def _db_path(cls) -> str:
+        return cls.connection().databaseName()
+
     # -------------------------------------------------------------------------------------------------------------------
     # Executes an SQL query from given sql_text
     # params is a list of tuples (":param", value) which are used to prepare SQL query
     # Current transaction will be committed if 'commit' set to true
     # Parameter 'forward_only' may be used for optimization
     # return value - QSqlQuery object (to allow iteration through result)
     @classmethod
```

### Comparing `jal-2023.4.8/jal/db/helpers.py` & `jal-2023.5.1/jal/db/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/holdings_model.py` & `jal-2023.5.1/jal/db/holdings_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,142 @@
+from __future__ import annotations
 from datetime import datetime
 from decimal import Decimal
 
-from PySide6.QtCore import Qt, Slot, QAbstractItemModel, QDate, QModelIndex
+from PySide6.QtCore import Qt, QDate
 from PySide6.QtGui import QBrush, QFont
 from PySide6.QtWidgets import QHeaderView
 from jal.constants import CustomColor, PredefindedAccountType
 from jal.db.helpers import localize_decimal
+from jal.db.tree_model import AbstractTreeItem, AbstractTreeModel
 from jal.db.account import JalAccount
 from jal.db.asset import JalAsset
 from jal.widgets.delegates import GridLinesDelegate
 from jal.widgets.helpers import ts2d
 
-
-class TreeItem:
-    def __init__(self, data, parent=None):
-        self._parent = parent
-        self.data = data.copy()
-        self._children = []
-
-    def appendChild(self, child):
-        child.setParent(self)
-        self._children.append(child)
-
-    def getChild(self, id):
-        if id < 0 or id > len(self._children):
+# ----------------------------------------------------------------------------------------------------------------------
+class AssetTreeItem(AbstractTreeItem):
+    def __init__(self, data=None, parent=None, group=''):
+        super().__init__(parent, group)
+        if data is None:
+            self._data = {
+                'currency_id': 0, 'currency': '', 'account_id': 0, 'account': '', 'asset_id': 0, 'tag': '',
+                'asset_is_currency': False, 'asset': '', 'asset_name': '', 'country_id': 0, 'country': '', 'expiry': 0,
+                'qty': Decimal('0'), 'value_i': Decimal('0'),
+                'quote': Decimal('0'), 'quote_ts': Decimal('0'), 'quote_a': Decimal('0')
+            }
+        else:
+            self._data = data.copy()
+        self._data['share'] = Decimal('0')
+        self._data['value'] = self._data['quote'] * self._data['qty']
+        self._data['value_a'] = self._data['quote_a'] * self._data['qty'] if self._data['quote_a'] else Decimal('0')
+        self._data['profit'] = self._data['quote'] * self._data['qty'] - self._data['value_i'] if not self._data['asset_is_currency'] else Decimal('0')
+        self._data['profit_rel'] = Decimal('100') * (self._data['quote'] * self._data['qty'] / self._data['value_i'] - 1) if self._data['value_i'] != Decimal('0') else Decimal('0')
+
+    def _calculateGroupTotals(self, child_data):
+        self._data['currency'] = child_data['currency']
+        self._data['account'] = child_data['account']
+        self._data['asset'] = child_data['asset']
+        self._data['country'] = child_data['country']
+        self._data['tag'] = child_data['tag']
+        self._data['value'] += child_data['value']
+        self._data['value_a'] += child_data['value_a']
+        self._data['profit'] += child_data['profit']
+        self._data['profit_rel'] = Decimal('100') * self._data['profit'] / (self._data['value'] - self._data['profit']) if self._data['value'] != self._data['profit'] else Decimal('0')
+
+    def _afterParentGroupUpdate(self, group_data):
+        self._data['share'] = Decimal('100') * self._data['value_a'] / group_data['value_a'] if group_data['value_a'] else Decimal('0')
+
+    def details(self):
+        return self._data
+
+    # assigns group value if this tree item is a group item
+    def setGroupValue(self, value):
+        if self._group:
+            self._data[self._group] = value
+
+    def getGroup(self):
+        if self._group:
+            return self._group, self._data[self._group]
+        else:
             return None
-        return self._children[id]
-
-    def count(self):
-        return len(self._children)
-
-    def setParent(self, parent):
-        self._parent = parent
-
-    def getParent(self):
-        return self._parent
 
+    # returns an element of tree that will provide right group parent for 'item' with given 'group_fields'
+    def getGroupLeaf(self, group_fields: list, item: AssetTreeItem) -> AssetTreeItem:
+        if group_fields:
+            group_item = None
+            group_name = group_fields[0]
+            for child in self._children:
+                if child.details()[group_name] == item.details()[group_name]:
+                    group_item = child
+            if group_item is None:
+                group_item = AssetTreeItem(None, parent=self, group=group_name)
+                group_item.setGroupValue(item.details()[group_name])
+                self._children.append(group_item)
+            return group_item.getGroupLeaf(group_fields[1:], item)
+        else:
+            return self
 
-class HoldingsModel(QAbstractItemModel):
+# ----------------------------------------------------------------------------------------------------------------------
+class HoldingsModel(AbstractTreeModel):
     def __init__(self, parent_view):
         super().__init__(parent_view)
-        self._view = parent_view
         self._grid_delegate = None
-        self._root = None
         self._currency = 0
         self._currency_name = ''
         self._date = QDate.currentDate().endOfDay(Qt.UTC).toSecsSinceEpoch()
-        self.calculated_names = ['share', 'profit', 'profit_rel', 'value', 'value_a']
-        self._columns = [self.tr("Currency/Account/Asset"),
-                         self.tr("Asset Name"),
-                         self.tr("Qty"),
-                         self.tr("Open"),
-                         self.tr("Last"),
-                         self.tr("Share, %"),
-                         self.tr("P/L, %"),
-                         self.tr("P/L"),
-                         self.tr("Value"),
-                         self.tr("Value, ")]
-
-    def rowCount(self, parent=None):
-        if not parent.isValid():
-            parent_item = self._root
-        else:
-            parent_item = parent.internalPointer()
-        if parent_item is not None:
-            return parent_item.count()
-        else:
-            return 0
-
-    def columnCount(self, parent=None):
-        return len(self._columns)
+        self._columns = [{'name': self.tr("Currency/Account/Asset")},
+                         {'name': self.tr("Asset Name")},
+                         {'name': self.tr("Qty")},
+                         {'name': self.tr("Open")},
+                         {'name': self.tr("Last")},
+                         {'name': self.tr("Share, %")},
+                         {'name': self.tr("P/L, %")},
+                         {'name': self.tr("P/L")},
+                         {'name': self.tr("Value")},
+                         {'name': self.tr("Value, ")}]
 
     def headerData(self, section, orientation, role=Qt.DisplayRole):
-        if orientation == Qt.Horizontal:
-            if role == Qt.DisplayRole:
-                col_name = self._columns[section] + self._currency_name if section == 9 else self._columns[section]
-                return col_name
-        return None
-
-    def headerWidth(self, section):
-        return self._view.header().sectionSize(section)
-
-    def index(self, row, column, parent=None):
-        if not parent.isValid():
-            parent = self._root
-        else:
-            parent = parent.internalPointer()
-        child = parent.getChild(row)
-        if child:
-            return self.createIndex(row, column, child)
-        return QModelIndex()
-
-    def parent(self, index):
-        if not index.isValid():
-            return QModelIndex()
-        child_item = index.internalPointer()
-        parent_item = child_item.getParent()
-        if parent_item == self._root:
-            return QModelIndex()
-        return self.createIndex(0, 0, parent_item)
+        value = super().headerData(section, orientation, role)
+        if orientation == Qt.Horizontal and role == Qt.DisplayRole and section == 9:
+            value += self._currency_name
+        return value
 
     def data(self, index, role=Qt.DisplayRole):
-        if not index.isValid():
+        try:
+            if not index.isValid():
+                return None
+            item = index.internalPointer()
+            if role == Qt.DisplayRole:
+                return self.data_text(item, index.column())
+            if role == Qt.FontRole:
+                return self.data_font(item, index.column())
+            if role == Qt.BackgroundRole:
+                return self.data_background(item, index.column(), self._view.isEnabled())
+            if role == Qt.ToolTipRole:
+                return self.data_tooltip(item.details(), index.column())
+            if role == Qt.TextAlignmentRole:
+                if index.column() < 2:
+                    return int(Qt.AlignLeft)
+                else:
+                    return int(Qt.AlignRight)
             return None
-        item = index.internalPointer()
-        if role == Qt.DisplayRole:
-            return self.data_text(item.data, index.column())
-        if role == Qt.FontRole:
-            return self.data_font(item.data, index.column())
-        if role == Qt.BackgroundRole:
-            return self.data_background(item.data, index.column(), self._view.isEnabled())
-        if role == Qt.ToolTipRole:
-            return self.data_tooltip(item.data, index.column())
-        if role == Qt.TextAlignmentRole:
-            if index.column() < 2:
-                return int(Qt.AlignLeft)
-            else:
-                return int(Qt.AlignRight)
-        return None
+        except Exception as e:
+            print(e)
 
-    def data_text(self, data, column):
+    def data_text(self, item, column):
+        data = item.details()
         if column == 0:
-            if data['level'] == 0:
-                return data['currency']
-            elif data['level'] == 1:
-                return data['account']
+            if item.isGroup():
+                group, value = item.getGroup()
+                return data[group.strip("_id")]
             else:
-                return data['asset']
+                all_fields = ['currency', 'account', 'asset']
+                display_fields = [y for y in all_fields if y not in [x.strip("_id") for x in self._groups]]
+                return ': '.join([data[x] for x in display_fields])
         elif column == 1:
             expiry_text = ""
             if data['expiry']:
                 expiry_header = self.tr("Exp:")
                 expiry_text = f" [{expiry_header} {ts2d(int(data['expiry']))}]"
             return data['asset_name'] + expiry_text
         elif column == 2:
@@ -149,34 +155,35 @@
             else:
                 return ''
         elif column == 4:
             return f"{float(data['quote']):,.4f}" if data['quote'] and float(data['qty']) != 0 else ''
         elif column == 5:
             return f"{data['share']:,.2f}" if data['share'] else '-.--'
         elif column == 6:
-            return f"{Decimal('100') * data['profit_rel']:,.2f}" if data['profit_rel'] else ''
+            return f"{data['profit_rel']:,.2f}" if data['profit_rel'] else ''
         elif column == 7:
             return f"{data['profit']:,.2f}" if data['profit'] else ''
         elif column == 8:
             return f"{data['value']:,.2f}" if data['value'] else ''
         elif column == 9:
             return f"{data['value_a']:,.2f}" if data['value_a'] else '-.--'
         else:
             assert False
 
     def data_tooltip(self, data, column):
-        if column >= 4 and column <= 8:
+        if 4 <= column <= 8:
             quote_date = datetime.utcfromtimestamp(int(data['quote_ts']))
             quote_age = int((datetime.utcnow() - quote_date).total_seconds() / 86400)
             if quote_age > 7:
                 return self.tr("Last quote date: ") + ts2d(int(data['quote_ts']))
         return ''
 
-    def data_font(self, data, column):
-        if data['level'] < 2:
+    def data_font(self, item, column):
+        data = item.details()
+        if item.isGroup():
             font = QFont()
             font.setBold(True)
             return font
         else:
             if column == 1 and data['expiry']:
                 expiry_date = datetime.utcfromtimestamp(int(data['expiry']))
                 days_remaining = int((expiry_date - datetime.utcnow()).total_seconds() / 86400)
@@ -191,20 +198,23 @@
                 quote_date = datetime.utcfromtimestamp(int(data['quote_ts']))
                 quote_age = int((datetime.utcnow()- quote_date).total_seconds() / 86400)
                 if quote_age > 7:
                     font = QFont()
                     font.setItalic(True)
                     return font
 
-    def data_background(self, data, column, enabled=True):
+    def data_background(self, item, column, enabled=True):
+        data = item.details()
         factor = 100 if enabled else 125
-        if data['level'] == 0:
-            return QBrush(CustomColor.LightPurple.lighter(factor))
-        if data['level'] == 1:
-            return QBrush(CustomColor.LightBlue.lighter(factor))
+        if item.isGroup():
+            group, value = item.getGroup()
+            if group == "currency_id":
+                return QBrush(CustomColor.LightPurple.lighter(factor))
+            if group == "account_id":
+                return QBrush(CustomColor.LightBlue.lighter(factor))
         if column == 6 and data['profit_rel']:
             if data['profit_rel'] >= 0:
                 return QBrush(CustomColor.LightGreen.lighter(factor))
             else:
                 return QBrush(CustomColor.LightRed.lighter(factor))
         if column == 7 and data['profit']:
             if data['profit'] >= 0:
@@ -220,38 +230,38 @@
         self._grid_delegate = GridLinesDelegate(self._view)
         for i in range(len(self._columns)):
             self._view.setItemDelegateForColumn(i, self._grid_delegate)
         font = self._view.header().font()
         font.setBold(True)
         self._view.header().setFont(font)
 
-    @Slot()
-    def setCurrency(self, currency_id):
+    def updateView(self, currency_id, date, grouping):
+        update = False
         if self._currency != currency_id:
             self._currency = currency_id
             self._currency_name = JalAsset(currency_id).symbol()
-            self.calculateHoldings()
-
-    @Slot()
-    def setDate(self, new_date):
-        if self._date != new_date.endOfDay(Qt.UTC).toSecsSinceEpoch():
-            self._date = new_date.endOfDay(Qt.UTC).toSecsSinceEpoch()
-            self.calculateHoldings()
+            update = True
+        if self._date != date.endOfDay(Qt.UTC).toSecsSinceEpoch():
+            self._date = date.endOfDay(Qt.UTC).toSecsSinceEpoch()
+            update = True
+        if self.setGrouping(grouping) or update:
+            self.prepareData()
+            self.configureView()
 
     def get_data_for_tax(self, index):
         if not index.isValid():
             return None
-        item = index.internalPointer()
-        return item.data['account_id'], item.data['asset_id'], item.data['currency_id'], item.data['qty']
+        data = index.internalPointer().details()
+        return data['account_id'], data['asset_id'], data['currency_id'], data['qty']
 
     def update(self):
-        self.calculateHoldings()
+        self.prepareData()
 
     # Populate table 'holdings' with data calculated for given parameters of model: _currency, _date,
-    def calculateHoldings(self):
+    def prepareData(self):
         holdings = []
         accounts = JalAccount.get_all_accounts(account_type=PredefindedAccountType.Investment)
         for account in accounts:
             account_holdings = []
             assets = account.assets_list(self._date)
             rate = JalAsset(account.currency()).quote(self._date, self._currency)[1]
             for asset_data in assets:
@@ -262,14 +272,17 @@
                     "currency": JalAsset(account.currency()).symbol(),
                     "account_id": account.id(),
                     "account": account.name(),
                     "asset_id": asset.id(),
                     "asset_is_currency": False,
                     "asset": asset.symbol(currency=account.currency()),
                     "asset_name": asset.name(),
+                    "country_id": asset.country().id(),
+                    "country": asset.country().name(),
+                    "tag": asset.tag().name() if asset.tag().name() else self.tr("N/A"),
                     "expiry": asset.expiry(),
                     "qty": asset_data['amount'],
                     "value_i": asset_data['value'],
                     "quote": quote,
                     "quote_ts": quote_ts,
                     "quote_a": rate * quote
                 }
@@ -281,89 +294,28 @@
                     "currency": JalAsset(account.currency()).symbol(),
                     "account_id": account.id(),
                     "account": account.name(),
                     "asset_id": account.currency(),
                     "asset_is_currency": True,
                     "asset": JalAsset(account.currency()).symbol(),
                     "asset_name": JalAsset(account.currency()).name(),
+                    "country_id": JalAsset(account.currency()).country().id(),
+                    "country": JalAsset(account.currency()).country().name(),
+                    "tag": self.tr("Money"),
                     "expiry": 0,
                     "qty": money,
                     "value_i": Decimal('0'),
                     "quote": Decimal('1'),
                     "quote_ts": QDate.currentDate().endOfDay(Qt.UTC).toSecsSinceEpoch(),
                     "quote_a": rate
                 })
-            account_total = sum(x['qty'] * x['quote'] for x in account_holdings)
-            for record in account_holdings:
-                record['total'] = account_total
             holdings += account_holdings
         holdings = sorted(holdings, key=lambda x: (x['currency'], x['account'], x['asset_is_currency'], x['asset']))
 
-        self._root = TreeItem({})
-        currency = 0
-        c_node = None
-        account = 0
-        a_node = None
-        for values in holdings:
-            values['level'] = 2
-            if values['currency_id'] != currency:
-                currency = values['currency_id']
-                c_node = TreeItem(values, self._root)
-                c_node.data['level'] = 0
-                c_node.data['asset_name'] = ''
-                c_node.data['expiry'] = 0
-                c_node.data['qty'] = Decimal('0')
-                self._root.appendChild(c_node)
-            if values['account_id'] != account:
-                account = values['account_id']
-                a_node = TreeItem(values, c_node)
-                a_node.data['level'] = 1
-                a_node.data['asset_name'] = ''
-                a_node.data['expiry'] = 0
-                a_node.data['qty'] = Decimal('0')
-                c_node.appendChild(a_node)
-            if values['quote']:
-                if values['asset_is_currency']:
-                    profit = Decimal('0')
-                else:
-                    profit = values['quote'] * values['qty'] - values['value_i']
-                if values['value_i'] != Decimal('0'):
-                    profit_relative = values['quote'] * values['qty'] / values['value_i'] - 1
-                else:
-                    profit_relative = Decimal('0')
-                value = values['quote'] * values['qty']
-                share = Decimal('100.0') * value / values['total']
-                value_adjusted = values['quote_a'] * values['qty'] if values['quote_a'] else Decimal('0')
-                values.update(dict(zip(self.calculated_names, [share, profit, profit_relative, value, value_adjusted])))
-            else:
-                values.update(dict(zip(self.calculated_names,
-                                       [Decimal('0'), Decimal('0'), Decimal('0'), Decimal('0'), Decimal('0')])))
-            node = TreeItem(values, a_node)
-            a_node.appendChild(node)
-
-        # Update totals
-        for i in range(self._root.count()):          # Iterate through each currency
-            currency_child = self._root.getChild(i)
-            for j in range(currency_child.count()):  # Iterate through each account for given currency
-                self.add_node_totals(currency_child.getChild(j))
-            self.add_node_totals(currency_child)
-            for j in range(currency_child.count()):  # Calculate share of each account within currency
-                if currency_child.data['value']:
-                    currency_child.getChild(j).data['share'] = \
-                        Decimal('100') * currency_child.getChild(j).data['value'] / currency_child.data['value']
-        # Get full total of totals for all currencies adjusted to common currency
-        total = sum([self._root.getChild(i).data['value_a'] for i in range(self._root.count())])
-        for i in range(self._root.count()):  # Calculate share of each currency (adjusted to common currency)
-            if total != Decimal('0'):
-                self._root.getChild(i).data['share'] = Decimal('100') * self._root.getChild(i).data['value_a'] / total
-            else:
-                self._root.getChild(i).data['share'] = None
+        self._root = AssetTreeItem()
+        for position in holdings:
+            new_item = AssetTreeItem(position)
+            leaf = self._root.getGroupLeaf(self._groups, new_item)
+            leaf.appendChild(new_item)
         self.modelReset.emit()
+        self.configureView()
         self._view.expandAll()
-
-    # Update node totals with sum of profit, value and adjusted profit and value of all children
-    def add_node_totals(self, node):
-        profit = sum([node.getChild(i).data['profit'] for i in range(node.count())])
-        value = sum([node.getChild(i).data['value'] for i in range(node.count())])
-        value_adjusted = sum([node.getChild(i).data['value_a'] for i in range(node.count())])
-        profit_relative = profit / (value - profit) if value != profit else 0
-        node.data.update(dict(zip(self.calculated_names, [Decimal('0'), profit, profit_relative, value, value_adjusted])))
```

### Comparing `jal-2023.4.8/jal/db/ledger.py` & `jal-2023.5.1/jal/db/ledger.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/operations.py` & `jal-2023.5.1/jal/db/operations.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/operations_model.py` & `jal-2023.5.1/jal/db/operations_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/peer.py` & `jal-2023.5.1/jal/db/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/reference_models.py` & `jal-2023.5.1/jal/db/reference_models.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/tax_estimator.py` & `jal-2023.5.1/jal/db/tax_estimator.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/db/view_model.py` & `jal-2023.5.1/jal/db/view_model.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/accept.png` & `jal-2023.5.1/jal/img/accept.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/add.png` & `jal-2023.5.1/jal/img/add.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/add_child.png` & `jal-2023.5.1/jal/img/add_child.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/cancel.png` & `jal-2023.5.1/jal/img/cancel.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/chart.png` & `jal-2023.5.1/jal/img/chart.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/copy.png` & `jal-2023.5.1/jal/img/copy.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/delete.png` & `jal-2023.5.1/jal/img/delete.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/ibkr.png` & `jal-2023.5.1/jal/img/ibkr.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/j2t.png` & `jal-2023.5.1/jal/img/j2t.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/jal.png` & `jal-2023.5.1/jal/img/jal.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/kit.png` & `jal-2023.5.1/jal/img/kit.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/list.png` & `jal-2023.5.1/jal/img/list.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/new.png` & `jal-2023.5.1/jal/img/new.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/open_portfolio.png` & `jal-2023.5.1/jal/img/open_portfolio.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/openbroker.ico` & `jal-2023.5.1/jal/img/openbroker.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/psb.ico` & `jal-2023.5.1/jal/img/psb.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/quik.ico` & `jal-2023.5.1/jal/img/quik.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/reconcile.png` & `jal-2023.5.1/jal/img/reconcile.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/remove.png` & `jal-2023.5.1/jal/img/remove.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/tax.png` & `jal-2023.5.1/jal/img/tax.png`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/img/uralsib.ico` & `jal-2023.5.1/jal/img/uralsib.ico`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/jal.py` & `jal-2023.5.1/jal/jal.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/jal_init.sql` & `jal-2023.5.1/jal/jal_init.sql`

 * *Files 0% similar despite different names*

```diff
@@ -658,25 +658,28 @@
 CREATE TRIGGER keep_predefined_categories BEFORE DELETE ON categories FOR EACH ROW WHEN OLD.special = 1
 BEGIN
     SELECT RAISE(ABORT, "JAL_SQL_MSG_0002");
 END;
 
 
 -- Initialize default values for settings
-INSERT INTO settings(id, name, value) VALUES (0, 'SchemaVersion', 44);
+INSERT INTO settings(id, name, value) VALUES (0, 'SchemaVersion', 45);
 INSERT INTO settings(id, name, value) VALUES (1, 'TriggersEnabled', 1);
 -- INSERT INTO settings(id, name, value) VALUES (2, 'BaseCurrency', 1); -- Deprecated and ID shouldn't be re-used
 INSERT INTO settings(id, name, value) VALUES (3, 'Language', 1);
 INSERT INTO settings(id, name, value) VALUES (4, 'RuTaxClientSecret', 'IyvrAbKt9h/8p6a7QPh8gpkXYQ4=');
 INSERT INTO settings(id, name, value) VALUES (5, 'RuTaxSessionId', '');
 INSERT INTO settings(id, name, value) VALUES (6, 'RuTaxRefreshToken', '');
 INSERT INTO settings(id, name, value) VALUES (7, 'RebuildDB', 0);
 INSERT INTO settings(id, name, value) VALUES (8, 'WindowGeometry', '');
 INSERT INTO settings(id, name, value) VALUES (9, 'WindowState', '');
 INSERT INTO settings(id, name, value) VALUES (10, 'MessageOnce', '');
+INSERT INTO settings(id, name, value) VALUES (11, 'RecentFolder_Statement', '.');
+INSERT INTO settings(id, name, value) VALUES (12, 'RecentFolder_Report', '.');
+INSERT INTO settings(id, name, value) VALUES (13, 'CleanDB', 0);
 
 -- Initialize available languages
 INSERT INTO languages (id, language) VALUES (1, 'en');
 INSERT INTO languages (id, language) VALUES (2, 'ru');
 
 -- Initialize sources of quotation data
 INSERT INTO data_sources (id, name) VALUES (-1, 'None');
```

### Comparing `jal-2023.4.8/jal/languages/en.qm` & `jal-2023.5.1/jal/languages/en.qm`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/languages/ru.qm` & `jal-2023.5.1/jal/languages/ru.qm`

 * *Files 2% similar despite different names*

```diff
@@ -1,5498 +1,5622 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0572 755f 5255 4200 001a 3800  .....ru_RUB...8.
-00000020: 0000 2300 001c 2500 0000 2300 0030 1300  ..#...%...#..0..
-00000030: 0000 2300 0132 3b00 0000 2300 0136 eb00  ..#..2;...#..6..
-00000040: 0000 2500 0091 9500 0004 7300 0005 b700  ..%.......s.....
-00000050: 0005 3b00 0009 4c00 0005 af00 0138 9c00  ..;...L......8..
-00000060: 0007 db00 00a8 7200 0031 0e00 007d 3900  ......r..1...}9.
-00000070: 0031 0e00 0126 0f00 0046 3900 0003 7000  .1...&...F9...p.
-00000080: 0046 3900 00a2 0000 0047 a400 0045 bf00  .F9......G...E..
-00000090: 0048 7200 0091 bc00 0048 7200 00a6 6200  .Hr......Hr...b.
-000000a0: 0048 b700 0092 1700 0048 b700 00a6 8e00  .H.......H......
-000000b0: 004a 7a00 0047 bd00 004a b300 0092 c500  .Jz..G...J......
-000000c0: 004a b300 00a6 ba00 004b 1a00 0047 e800  .J.......K...G..
-000000d0: 004b 3a00 0048 1300 004c b200 0093 3100  .K:..H...L....1.
-000000e0: 004c b200 00a6 e600 004c b500 0013 bf00  .L.......L......
-000000f0: 004c b500 0133 3f00 0050 7e00 0093 da00  .L...3?..P~.....
-00000100: 0050 7e00 00a7 1200 0051 3100 001e df00  .P~......Q1.....
-00000110: 0051 3100 0031 8400 0051 bc00 0094 0700  .Q1..1...Q......
-00000120: 0051 bc00 00a7 3e00 0051 be00 0094 3400  .Q....>..Q....4.
-00000130: 0051 be00 00a7 6a00 0052 ac00 0095 4200  .Q....j..R....B.
-00000140: 0052 ac00 0097 9b00 0053 3c00 0015 2300  .R.......S<...#.
-00000150: 0053 3c00 0036 c900 0053 8200 0094 6100  .S<..6...S....a.
-00000160: 0053 8200 00a7 9600 0053 8900 0094 8e00  .S.......S......
-00000170: 0053 8900 00a7 c200 0055 6600 0094 e800  .S.......Uf.....
-00000180: 0055 6600 00a7 ee00 0055 a400 0095 1500  .Uf......U......
-00000190: 0055 a400 00a8 1a00 0058 b900 0015 8a00  .U.......X......
-000001a0: 0058 b900 0020 5e00 0058 b900 0037 2800  .X... ^..X...7(.
-000001b0: 0058 b900 00ab 4d00 0058 b900 0122 1700  .X....M..X..."..
-000001c0: 0058 b900 0133 d300 0059 c000 0096 3900  .X...3...Y....9.
-000001d0: 0059 c000 00a8 4600 005a 7700 002b cf00  .Y....F..Zw..+..
-000001e0: 005a 7700 0088 d800 005a 7700 011c 1a00  .Zw......Zw.....
-000001f0: 005a 8800 0032 f900 005b 2a00 0027 6b00  .Z...2...[*..'k.
-00000200: 0070 7c00 005c 2100 047a 6e00 0005 4000  .p|..\!..zn...@.
-00000210: 047a 6e00 011a fc00 0498 9800 008e 2300  .zn...........#.
-00000220: 04a6 7900 006f 4800 04a6 7900 0084 5f00  ..y..oH...y..._.
-00000230: 04a8 a500 000e 0500 04a8 a500 009f 2100  ..............!.
-00000240: 04a8 a500 0121 6700 04a8 d300 0090 9400  .....!g.........
-00000250: 04cb c300 0093 5e00 04cf 3a00 0035 be00  ......^...:..5..
-00000260: 04d9 5d00 0138 3c00 04e3 1a00 0074 ad00  ..]..8<......t..
-00000270: 04e7 de00 000b 0d00 04e7 de00 000c 7500  ..............u.
-00000280: 0504 cf00 0077 e000 0528 a400 0035 ee00  .....w...(...5..
-00000290: 0548 3500 0006 1b00 0548 3500 000b 3c00  .H5......H5...<.
-000002a0: 0548 3500 0011 c100 0548 3500 008d 5900  .H5......H5...Y.
-000002b0: 0556 a500 0013 f800 0556 a500 001f 1200  .V.......V......
-000002c0: 0556 a500 002b 9a00 0556 a500 0031 f500  .V...+...V...1..
-000002d0: 0556 a500 0053 8b00 0556 a500 0133 7200  .V...S...V...3r.
-000002e0: 0556 a500 0138 6500 0565 c000 0043 cc00  .V...8e..e...C..
-000002f0: 0566 be00 0036 8f00 0566 be00 0121 9900  .f...6...f...!..
-00000300: 056b c200 0055 3a00 05a3 0000 004b d700  .k...U:......K..
-00000310: 05a7 aa00 011c fd00 05a7 e300 011f 0d00  ................
-00000320: 05b3 d800 0120 3600 05c0 6500 0021 a300  ..... 6...e..!..
-00000330: 05c0 6500 0033 2900 05db bb00 0027 9a00  ..e..3)......'..
-00000340: 05fb 8200 0027 d000 1530 3000 0012 3a00  .....'...00...:.
-00000350: 18d1 5000 00ef e700 2311 0000 0125 e200  ..P.....#....%..
-00000360: 26f2 9100 004c 0300 2aa8 a100 0056 e900  &....L..*....V..
-00000370: 2acf 0400 0057 1f00 2b37 fe00 0057 c500  *....W..+7...W..
-00000380: 2b76 1e00 0085 2e00 2ba7 e300 0059 c900  +v......+....Y..
-00000390: 2ec7 e000 0045 5e00 3153 c400 0093 9600  .....E^.1S......
-000003a0: 3d1a 0e00 005b 7c00 4182 8900 0100 e600  =....[|.A.......
-000003b0: 4796 c400 0077 6100 47af 8000 009b 3000  G....wa.G.....0.
-000003c0: 48a9 c400 0006 db00 48a9 c400 0012 8a00  H.......H.......
-000003d0: 48a9 c400 001c da00 48a9 c400 0029 9400  H.......H....)..
-000003e0: 48a9 c400 0030 6b00 48a9 c400 009e bc00  H....0k.H.......
-000003f0: 48a9 c400 00ab 1d00 48a9 c400 0132 8d00  H.......H....2..
-00000400: 48a9 c400 0137 4400 4964 b300 008f 9000  H....7D.Id......
-00000410: 4988 b300 008d e900 4a2b 8200 0046 c700  I.......J+...F..
-00000420: 4a2b 8200 006f 1500 4a36 9500 002a 4300  J+...o..J6...*C.
-00000430: 4a36 9500 0046 fe00 4a36 9500 0073 b900  J6...F..J6...s..
-00000440: 4a71 ec00 0025 3100 4ab8 3300 0028 d400  Jq...%1.J.3..(..
-00000450: 4b6b 9000 0105 8900 4d68 c800 0090 c400  Kk......Mh......
-00000460: 4d96 0a00 0025 df00 4dc4 b300 0090 f900  M....%..M.......
-00000470: 4e7e 1a00 0008 de00 522b 5a00 0073 ef00  N~......R+Z..s..
-00000480: 52e9 5500 0014 d900 5308 d400 0095 a500  R.U.....S.......
-00000490: 535d fe00 0074 dc00 5464 c900 0091 2c00  S]...t..Td....,.
-000004a0: 5464 c900 0094 bb00 5465 a800 0026 0e00  Td......Te...&..
-000004b0: 5483 8a00 0009 0d00 556a c300 0082 7d00  T.......Uj....}.
-000004c0: 55da be00 0012 0300 56bc 5a00 004a 9200  U.......V.Z..J..
-000004d0: 56bc 5a00 008c 4800 56bc 9300 008a 6800  V.Z...H.V.....h.
-000004e0: 578f 9500 0032 2c00 578f 9500 0133 a600  W....2,.W....3..
-000004f0: 57a1 7200 0027 2600 5839 2400 0069 8100  W.r..'&.X9$..i..
-00000500: 58c6 a500 009f 5100 5948 5c00 004e 5200  X.....Q.YH\..NR.
-00000510: 5948 5c00 0120 6a00 5a73 0400 001a 4a00  YH\.. j.Zs....J.
-00000520: 5a73 0400 0021 1900 5a79 2700 011e d700  Zs...!..Zy'.....
-00000530: 5a8a e000 0122 8400 5a8b c000 002f 6e00  Z...."..Z..../n.
-00000540: 5a8e c300 0096 6600 5a8e c300 012f 2000  Z.....f.Z..../ .
-00000550: 5b6a 7c00 000d 4600 5b6a 7c00 0096 9b00  [j|...F.[j|.....
-00000560: 5c06 8a00 004c 8d00 5c83 b500 0034 ec00  \....L..\....4..
-00000570: 5c83 b500 0037 9100 5fb8 5a00 0080 5300  \....7.._.Z...S.
-00000580: 5fb8 5a00 0130 8400 602e 0a00 0054 d800  _.Z..0..`....T..
-00000590: 67f7 0000 00f9 3600 70c5 c000 00c9 bd00  g.....6.p.......
-000005a0: 80a8 e500 0049 ce00 81bc 0000 00cf a600  .....I..........
-000005b0: 918d 3700 003c 4000 931f 2000 00db 1500  ..7..<@... .....
-000005c0: 9472 3000 006e ba00 9688 5400 00d5 f800  .r0..n....T.....
-000005d0: ab81 4000 0119 0f00 af00 f000 00b7 7c00  ..@...........|.
-000005e0: af26 4500 0126 6600 b27d 9f00 0078 7600  .&E..&f..}...xv.
-000005f0: b4d0 c500 0029 d900 b643 0000 00c4 4200  .....)...C....B.
-00000600: c9db ba00 0061 7e00 cfb0 f400 0031 1100  .....a~......1..
-00000610: e1f3 f000 0017 8d00 e25b 3000 002c f900  .........[0..,..
-00000620: ed2c 2500 0028 0000 fbe4 b100 0048 3e00  .,%..(.......H>.
-00000630: ff6b fe00 00b4 ba01 11c0 6000 013a d401  .k........`..:..
-00000640: 1c4b f000 0116 9701 2273 8300 008d 9701  .K......"s......
-00000650: 24a2 9700 003c f701 2bca d000 009d a501  $....<..+.......
-00000660: 3502 c000 00c6 1101 473b 2300 0070 5201  5.......G;#..pR.
-00000670: 5567 7000 00ce ff01 59b4 9000 001b 0d01  Ugp.....Y.......
-00000680: 6654 9000 003b 3701 7248 d000 0036 2801  fT...;7.rH...6(.
-00000690: 776d e000 00d7 1801 78c3 f500 0031 b001  wm......x....1..
-000006a0: 7e51 ea00 012c d501 873b 2300 0070 8401  ~Q...,...;#..p..
-000006b0: 887c d300 005c 4d01 9687 c000 010c 7201  .|...\M.......r.
-000006c0: 98a7 5300 004c bc01 a469 f900 0103 8201  ..S..L...i......
-000006d0: a885 4000 0136 0f01 aff7 3300 0000 0001  ..@..6....3.....
-000006e0: bef6 7000 00d4 1601 c26a 9a00 00a2 3501  ..p......j....5.
-000006f0: ce0a 1200 008b 5101 d48e 5000 0043 2801  ......Q...P..C(.
-00000700: da69 b000 0116 2a01 e128 5000 00c1 4801  .i....*..(P...H.
-00000710: e26a 9a00 0004 2801 f571 7000 00be 5702  .j....(..qp...W.
-00000720: 00dd 0100 0044 6a02 01b8 4900 003a 8d02  .....Dj...I..:..
-00000730: 01b8 4900 0087 8d02 01b8 4900 00a1 c002  ..I.......I.....
-00000740: 01b8 4900 0139 fc02 24d1 2000 00e0 cd02  ..I..9..$. .....
-00000750: 2b24 6500 012f e202 36c0 e700 006b c702  +$e../..6....k..
-00000760: 38ab b000 00b1 4b02 488e 8300 0129 2102  8.....K.H....)!.
-00000770: 5442 2f00 0022 3d02 6b41 b400 0130 af02  TB/.."=.kA...0..
-00000780: 705b 1000 005e cb02 75ac 0500 00d9 6502  p[...^..u.....e.
-00000790: 76e6 2500 0043 fd02 80f4 7400 005a 4102  v.%..C....t..ZA.
-000007a0: 83cb 1900 00ae 4d02 84df 6000 000d 0b02  ......M...`.....
-000007b0: 86cb d700 00af da02 960b 0000 0104 af02  ................
-000007c0: 9d24 b400 00c0 e502 a013 f300 00d5 9d02  .$..............
-000007d0: b6bc 9300 0058 3f02 b827 6100 00a3 fb02  .....X?..'a.....
-000007e0: c4de 6000 00ca 4b02 d6b9 7000 00e1 a802  ..`...K...p.....
-000007f0: d6b9 7000 00ed 9402 d6b9 7000 0104 0602  ..p.......p.....
-00000800: d6b9 7000 010e d202 da2f f000 00bc 8102  ..p....../......
-00000810: db87 a000 00f4 2702 ddd8 9000 0018 c702  ......'.........
-00000820: e4ef 0400 0020 9702 e60b 0000 0076 e402  ..... .......v..
-00000830: ecb9 d000 006c c303 0055 4a00 012c 3e03  .....l...UJ..,>.
-00000840: 0ae6 8700 0018 3203 0ae6 8700 001d ba03  ......2.........
-00000850: 0b8a 5a00 0079 f103 1108 9c00 0132 b603  ..Z..y.......2..
-00000860: 1638 c400 0095 ed03 1684 be00 001d 0d03  .8..............
-00000870: 2221 4000 00b0 c203 232f f000 00f5 6e03  "!@.....#/....n.
-00000880: 232f f000 010a 0d03 3500 5a00 0087 4103  #/......5.Z...A.
-00000890: 3f3c 8400 0112 a303 55cb 1a00 0075 4803  ?<......U....uH.
-000008a0: 57fa 2e00 0074 3603 5dae f000 010a bc03  W....t6.].......
-000008b0: 5dce f000 00e5 4103 6b8b d900 0127 fc03  ].....A.k....'..
-000008c0: 7321 8300 0111 8703 82a1 0000 00e1 d903  s!..............
-000008d0: 8a06 2000 0101 5603 8b39 a000 0105 f103  .. ...V..9......
-000008e0: 8b60 e400 003f b803 8c34 6500 0026 cd03  .`...?...4e..&..
-000008f0: 8f4e c000 0115 6303 9100 d000 005d d303  .N....c......]..
-00000900: 97c9 0000 0123 d903 b023 a000 00bb 3203  .....#...#....2.
-00000910: cafd 4000 0082 b603 d07e 2400 0067 a303  ..@......~$..g..
-00000920: d1c2 7400 0041 9203 d1e5 2200 0005 7103  ..t..A...."...q.
-00000930: da9c f300 0059 fb03 ec0c f700 003d bd03  .....Y.......=..
-00000940: f69b 8000 00c8 6b04 0029 e000 0127 4704  ......k..)...'G.
-00000950: 09f4 0a00 00bd e304 11d2 4900 000d 7704  ..........I...w.
-00000960: 11d2 a900 0056 5804 1263 4400 00b7 2e04  .....VX..cD.....
-00000970: 1564 8e00 0029 5a04 15b4 7000 013b 4d04  .d...)Z...p..;M.
-00000980: 195c b000 011a 6504 2e61 f000 0072 6c04  .\....e..a...rl.
-00000990: 449a c000 012e 2e04 56c0 a000 00b9 0604  D.......V.......
-000009a0: 62c1 c000 0100 5b04 65af 6900 004f 3104  b.....[.e.i..O1.
-000009b0: 66ac 6500 0138 fe04 7914 8000 00d2 b104  f.e..8..y.......
-000009c0: 7d16 7000 006d 9f04 846c 5400 002b 2e04  }.p..m...lT..+..
-000009d0: 846c 5400 0081 da04 846c 5400 0088 1104  .lT......lT.....
-000009e0: 846c 5400 0137 1104 8a9c b300 000a 1404  .lT..7..........
-000009f0: 8a9c b300 0091 e904 8c2d c700 0063 e904  .........-...c..
-00000a00: 8c2d c700 007b 6f04 8e23 4000 0000 c004  .-...{o..#@.....
-00000a10: 8e23 4000 001f e304 8e23 4000 0054 5e04  .#@......#@..T^.
-00000a20: 983c 8100 0046 9304 9849 bc00 0008 3504  .<...F...I....5.
-00000a30: 9e16 8200 0103 4304 9e84 d500 0092 4404  ......C.......D.
-00000a40: a577 1f00 0065 d004 a5e2 3000 0098 af04  .w...e....0.....
-00000a50: ac2c a500 0084 f504 ac2c a500 00a3 bf04  .,.......,......
-00000a60: bebd 0000 00a9 7504 c840 f000 00eb 1204  ......u..@......
-00000a70: c840 f000 00ee 4d04 c840 f000 0110 fd04  .@....M..@......
-00000a80: cc5c 9400 0028 4e04 cf4d c200 00f9 bd04  .\...(N..M......
-00000a90: d5c8 0000 0007 1a04 d7d5 4000 00cd 0004  ..........@.....
-00000aa0: dd34 9000 0015 bf04 ee54 4000 010d 7204  .4.......T@...r.
-00000ab0: f6d3 c900 00d5 3605 04e3 1000 0007 9505  ......6.........
-00000ac0: 079c 7300 0124 6705 161e a000 00b6 b905  ..s..$g.........
-00000ad0: 2caa 5000 00b5 1705 2cde 2300 00a4 5305  ,.P.....,.#...S.
-00000ae0: 304c 6a00 0049 9805 33ee 2500 0015 5205  0Lj..I..3.%...R.
-00000af0: 33ee 2500 0036 f405 3c8d c200 0018 7105  3.%..6..<.....q.
-00000b00: 3c8d c200 001e 8705 3d7b 7000 00ea ad05  <.......={p.....
-00000b10: 3d7b 7000 00ed e805 3d7b 7000 0105 2405  ={p.....={p...$.
-00000b20: 3d7b 7000 0110 1a05 49ee 8900 0067 0905  ={p.....I....g..
-00000b30: 4e5b d400 0119 5d05 5305 de00 0075 9605  N[....].S....u..
-00000b40: 5316 ce00 0074 7505 633f 7000 00e6 9b05  S....tu.c?p.....
-00000b50: 6945 5000 00c7 1f05 6bc4 2700 008a 2705  iEP.....k.'...'.
-00000b60: 6bcd a500 00b2 e205 6c90 5400 0095 6f05  k.......l.T...o.
-00000b70: 6ccc 4300 004b 7205 6edf f400 008c e305  l.C..Kr.n.......
-00000b80: 6fe5 c000 00f4 d905 802f 5e00 00b2 1605  o......../^.....
-00000b90: 812d 6000 0102 e605 88a7 e000 0122 4c05  .-`.........."L.
-00000ba0: 88a8 c000 004d c705 8c6a c300 009e 7f05  .....M...j......
-00000bb0: 8c6a c300 011b a605 8cbc 8e00 004b 3c05  .j...........K<.
-00000bc0: 98ab 6e00 008d 2505 9ca9 f100 0039 1905  ..n...%......9..
-00000bd0: 9dfd c000 00a8 f505 9e88 c300 0091 6105  ..............a.
-00000be0: a661 8700 004d fc05 a661 8700 004e d505  .a...M...a...N..
-00000bf0: a661 8700 0050 6705 a7f1 8700 0053 3505  .a...Pg......S5.
-00000c00: adfb 2800 009f 8c05 b039 5c00 000b 7b05  ..(......9\...{.
-00000c10: b039 5c00 011b e305 b093 0000 00c8 f905  .9\.............
-00000c20: b247 c400 009a d605 c068 c000 0009 a705  .G.......h......
-00000c30: c1f8 2200 008c 8805 ced0 2500 00d9 db05  ..".......%.....
-00000c40: d5fa e400 007f 5d05 d5fa e400 012c 8e05  ......]......,..
-00000c50: da03 6e00 005b dc05 dbc2 3900 0050 1e05  ..n..[....9..P..
-00000c60: dce3 0000 00d2 3705 dce3 0000 0102 6d05  ......7.......m.
-00000c70: dde3 7900 005e f505 e1ed 8400 00bf 4405  ..y..^........D.
-00000c80: ecff 1900 00ed 2305 f264 ba00 0047 3305  ......#..d...G3.
-00000c90: f662 ea00 00bd 6e05 facb 8300 008f cb06  .b....n.........
-00000ca0: 0826 4000 00d7 b406 08e3 9400 007a 8706  .&@..........z..
-00000cb0: 0ab9 9000 00e3 9b06 129d e000 00e0 5c06  ..............\.
-00000cc0: 148d a400 0021 d706 1867 1e00 0098 f906  .....!...g......
-00000cd0: 215f 7400 0061 2b06 2b00 1300 0037 fd06  !_t..a+.+....7..
-00000ce0: 2b00 1300 0038 8d06 2b00 1300 003a 0a06  +....8..+....:..
-00000cf0: 34af 4a00 0009 d706 3500 0f00 006a 5a06  4.J.....5....jZ.
-00000d00: 3c17 4000 00dd b406 3c17 4000 00e9 7006  <.@.....<.@...p.
-00000d10: 3c17 4000 00fb a606 3c17 4000 0115 1306  <.@.....<.@.....
-00000d20: 3cee 8400 00ad 0106 468c a000 00b1 ac06  <.......F.......
-00000d30: 4e38 c500 00a0 2d06 4f34 c000 0112 0506  N8....-.O4......
-00000d40: 53a5 f500 004b 0706 5479 d900 010f a906  S....K..Ty......
-00000d50: 580f ce00 002a 7e06 5a60 a900 00fa 0e06  X....*~.Z`......
-00000d60: 6318 9000 00e7 af06 68ee 6400 001c 8b06  c.......h.d.....
-00000d70: 69a9 8400 00a2 7e06 69b7 0200 012b 8f06  i.....~.i....+..
-00000d80: 70e2 d000 006d f606 7cd1 c500 004a 2206  p....m..|....J".
-00000d90: 7f33 4700 0032 ad06 8786 ea00 00a1 5f06  .3G..2........_.
-00000da0: 88a1 2400 0137 b006 8f30 5000 0120 9a06  ..$..7...0P.. ..
-00000db0: 9b5a 7700 011c 7c06 9bb8 0c00 0038 d406  .Zw...|......8..
-00000dc0: 9c50 2000 00c5 5f06 9fb2 5300 00ff 9406  .P ..._...S.....
-00000dd0: a6d5 8300 012f 4f06 a8dd 9c00 0051 5b06  ...../O......Q[.
-00000de0: aef9 ce00 0058 be06 afe6 3000 0071 9806  .....X....0..q..
-00000df0: b017 2200 00a0 ce06 b8bb 6000 00a9 f606  ..".......`.....
-00000e00: c10c 6000 00d0 3206 c215 0a00 0007 ee06  ..`...2.........
-00000e10: c227 5a00 0029 0b06 c5bd 6a00 0127 c806  .'Z..)....j..'..
-00000e20: ce8a a100 004c 4406 cf70 9900 0024 f606  .....LD..p...$..
-00000e30: d08b 2a00 00ca fd06 d81c 2e00 00da 4606  ..*...........F.
-00000e40: dbaf 2000 00f1 4e06 e231 4000 012e a506  .. ...N..1@.....
-00000e50: e6c0 4c00 0051 c007 0120 6600 0020 e707  ..L..Q... f.. ..
-00000e60: 0140 6600 0019 e407 0923 2000 0060 3807  .@f......# ..`8.
-00000e70: 0ac3 fa00 00a1 2107 0e35 d000 00dd 5407  ......!..5....T.
-00000e80: 126c 4400 013b ce07 1d24 9000 0107 0607  .lD..;...$......
-00000e90: 1db9 0500 0013 7407 3389 e000 00b8 4207  ......t.3.....B.
-00000ea0: 3c71 f700 000f 6607 449d 1f00 00bf a907  <q....f.D.......
-00000eb0: 47cf 0400 0040 ba07 4bcf e000 00e9 c007  G....@..K.......
-00000ec0: 5cec 7500 009f e907 62f5 3500 0040 4107  \.u.....b.5..@A.
-00000ed0: 65e8 b400 007e 0b07 65e8 b400 012a ed07  e....~..e....*..
-00000ee0: 6c21 5400 000b f607 7e9b 0500 00e8 c107  l!T.....~.......
-00000ef0: 9a56 2000 006f bc07 9a6c 1400 000c a507  .V ..o...l......
-00000f00: 9a6c 1400 001c 5207 9a6c 1400 0030 3907  .l....R..l...09.
-00000f10: 9a6c 1400 0051 2307 9a6c 1400 0081 a707  .l...Q#..l......
-00000f20: 9a6c 1400 0132 5e07 9aa9 6000 00cd 9807  .l...2^...`.....
-00000f30: 9db4 9000 00ba cb07 9db4 9000 00ff 2007  .............. .
-00000f40: 9e2e 7300 0139 9b07 a121 8000 0022 ea07  ..s..9...!..."..
-00000f50: a674 8700 00a2 d107 bdfe de00 002d 9a07  .t...........-..
-00000f60: cf9a 7000 00fd 4007 d231 3400 0003 9f07  ..p...@..14.....
-00000f70: daae 0000 0106 9907 dae0 ea00 011f 8b07  ................
-00000f80: e0a9 5000 000e a107 e0a9 5000 0089 6807  ..P.......P...h.
-00000f90: e0a9 5000 011d 9307 ebd7 9e00 00ac 2407  ..P...........$.
-00000fa0: ebd7 9e00 00af 0f07 ec42 a500 000a c507  .........B......
-00000fb0: ed5c 8000 0114 3207 f3d4 e000 00cb f207  .\....2.........
-00000fc0: f714 e400 00fa 8f08 0291 0000 0080 8408  ................
-00000fd0: 08a7 9000 00c6 9a08 1f02 9000 00b7 e208  ................
-00000fe0: 283b 1400 00ff eb08 284d 4300 0083 cb08  (;......(MC.....
-00000ff0: 28e8 e000 00f2 0508 2a45 4a00 00a3 1c08  (.......*EJ.....
-00001000: 2fe7 9000 009d 2d08 3267 1100 0008 a008  /.....-.2g......
-00001010: 41da 6e00 0085 8308 426e 6000 0118 1808  A.n.....Bn`.....
-00001020: 46c5 3a00 0045 f408 4d37 c500 0092 8008  F.:..E..M7......
-00001030: 4e6b 2a00 0047 7b08 4ef9 1500 005b 4608  Nk*..G{.N....[F.
-00001040: 4fd0 2000 0117 9508 6186 7000 0070 b608  O. .....a.p..p..
-00001050: 6c71 e200 00ae b008 6f32 c000 00db d608  lq......o2......
-00001060: 700d f000 00fc b908 70b2 8b00 0076 2308  p.......p....v#.
-00001070: 7219 0f00 0089 9f08 7a4a 5000 0079 1d08  r.......zJP..y..
-00001080: 8284 d500 000c d608 8284 d500 0082 0e08  ................
-00001090: 8599 7200 0138 c508 8958 2900 012d d508  ..r..8...X)..-..
-000010a0: 8b87 0000 00d3 6e08 8fa4 9300 0010 9908  ......n.........
-000010b0: 8fa4 9300 0085 d108 8fa4 9300 008b cd08  ................
-000010c0: 8fa4 9300 011c 4408 9a98 b400 001a c808  ......D.........
-000010d0: 9c61 5e00 011f e608 a1a4 9300 0057 ff08  .a^..........W..
-000010e0: a63b 3000 0110 8008 aa82 f400 0059 9008  .;0..........Y..
-000010f0: abe2 0900 002b 5f08 abe2 0900 0088 4608  .....+_.......F.
-00001100: af11 d500 0062 0308 b89a 9200 0026 9208  .....b.......&..
-00001110: bbfe c500 0002 ac08 bbfe c500 0128 d208  .............(..
-00001120: bd8a 6000 0119 db08 c000 5000 0097 5608  ..`.......P...V.
-00001130: c000 5000 0098 1908 c272 0900 0010 d608  ..P......r......
-00001140: c76b 0300 0059 0508 cd7c e400 00ab b409  .k...Y...|......
-00001150: 00f9 a400 0003 e009 162e f000 003b c609  .............;..
-00001160: 1afc d400 003e 7709 1fb9 f500 0075 c809  .....>w......u..
-00001170: 2254 0000 0123 7a09 2e57 df00 00a5 a109  "T...#z..W......
-00001180: 35e6 6000 0049 5509 3b85 e000 006b 3909  5.`..IU.;....k9.
-00001190: 4459 d000 00e3 0a09 4d67 fe00 011b 6609  DY......Mg....f.
-000011a0: 5962 c900 00e9 0009 5aa4 1000 00bb cf09  Yb......Z.......
-000011b0: 5b68 f000 005d 5909 5c07 3000 00f0 9f09  [h...]Y.\.0.....
-000011c0: 5ca2 3000 0134 4609 5d03 9000 0121 d709  \.0..4F.]....!..
-000011d0: 6302 2500 0139 6b09 667a 9000 00ee d609  c.%..9k.fz......
-000011e0: 66cc c900 0034 b109 700b c500 0012 cf09  f....4..p.......
-000011f0: 7a29 6900 0010 1909 8c00 0a00 004e 8f09  z)i..........N..
-00001200: 8c81 5e00 003a 4b09 8c81 5e00 004f d009  ..^..:K...^..O..
-00001210: 8c81 5e00 0097 cf09 8d04 b300 008f 0209  ..^.............
-00001220: 95cb c400 00d8 f809 a6af c300 0055 e109  .............U..
-00001230: a6c1 0a00 0028 9c09 a6c1 0a00 0045 8b09  .....(.......E..
-00001240: a6c1 0a00 0082 f709 a6c1 0a00 0097 1909  ................
-00001250: a6c1 0a00 0126 3609 a6c1 c300 0004 6f09  .....&6.......o.
-00001260: a87a 8000 00fb fd09 b56b a200 008c 0609  .z.......k......
-00001270: b889 ea00 0086 aa09 b889 ea00 00a5 0709  ................
-00001280: cf34 f000 00e2 7509 d82d 3f00 0083 2e09  .4....u..-?.....
-00001290: dbfe c000 00dc 950a 074b 5000 0071 ff0a  .........KP..q..
-000012a0: 159b 8000 001f 500a 159b 8000 0053 cc0a  ......P......S..
-000012b0: 17d3 5000 00ce 560a 20b0 6000 0078 170a  ..P...V. .`..x..
-000012c0: 20fc 9000 00b5 fb0a 22d2 d000 00e7 1a0a   .......".......
-000012d0: 2aef e000 00fd cb0a 2e99 7e00 0056 190a  *.........~..V..
-000012e0: 30f6 b500 002a d60a 338b 1000 00df db0a  0....*..3.......
-000012f0: 3f0e 9500 0080 0c0a 3f0e 9500 012d 940a  ?.......?....-..
-00001300: 4985 3000 0071 240a 4cb2 e000 00b9 860a  I.0..q$.L.......
-00001310: 5e50 b000 010c fb0a 62cd 3400 0035 6a0a  ^P......b.4..5j.
-00001320: 64c8 9500 0086 6e0a 65e3 f000 005c 9e0a  d.....n.e....\..
-00001330: 6c11 b300 0005 040a 6c5b d900 000a 580a  l.......l[....X.
-00001340: 6c5b d900 000c 3e0a 6c89 9300 0139 2e0a  l[....>.l....9..
-00001350: 6cba 2900 010f 270a 70ea 0000 0044 f00a  l.)...'.p....D..
-00001360: 8170 8e00 0135 1d0a 84e6 b500 001d 730a  .p...5........s.
-00001370: 84e6 b500 0030 d10a 84e6 b500 0052 2c0a  .....0.......R,.
-00001380: 84e6 b500 0133 020a 84e6 b500 0137 700a  .....3.......7p.
-00001390: 89ad 3000 00f7 d40a 89ad 3000 010e 340a  ..0.......0...4.
-000013a0: 8c5e f000 0065 210a 954c 2000 00de 050a  .^...e!..L .....
-000013b0: 9989 6300 0073 670a ac8c c000 00fb 2d0a  ..c..sg.......-.
-000013c0: ae3e fa00 0075 0e0a b4bc 2e00 002f 9e0a  .>...u......./..
-000013d0: b5ff 6400 00b3 7a0a b6d5 d000 00d4 960a  ..d...z.........
-000013e0: ba90 7000 00ea 2e0a be20 4a00 0011 1c0a  ..p...... J.....
-000013f0: c25d 1400 0042 530a c945 a000 00b5 6e0a  .]...BS..E....n.
-00001400: ca80 7300 0052 720a cf76 b400 0057 530a  ..s..Rr..v...WS.
-00001410: cfef 4000 0109 790a e1b0 da00 00aa 570a  ..@...y.......W.
-00001420: e1b4 8000 0117 1c0a e45f d000 00ba 440a  ........._....D.
-00001430: eb63 2000 0023 870a ee50 6000 0081 3c0a  .c ..#...P`...<.
-00001440: f3de 9e00 0084 9c0a f818 8000 00b9 bf0a  ................
-00001450: f818 8000 00fe 8e0b 0396 6300 0009 720b  ..........c...r.
-00001460: 03f9 7300 008e b80b 0476 b400 0057 8d0b  ..s......v...W..
-00001470: 0ac1 5a00 012d 2a0b 139f b500 0086 e20b  ..Z..-*.........
-00001480: 19b8 d700 008a a60b 1b90 b000 0104 360b  ..............6.
-00001490: 1fcd 0500 00a0 8a0b 20ce b000 00c4 cd0b  ........ .......
-000014a0: 2371 ce00 0001 3e0b 244d 8300 0108 550b  #q....>.$M....U.
-000014b0: 296c c900 0072 f80b 2d80 be00 000f c70b  )l...r..-.......
-000014c0: 2d80 be00 008b 030b 2d80 be00 011e 1a0b  -.......-.......
-000014d0: 2fa8 e400 0134 020b 4000 a500 0063 660b  /....4..@....cf.
-000014e0: 440d ae00 0059 3e0b 47ce c400 00ec 0e0b  D....Y>.G.......
-000014f0: 4841 e400 00be de0b 4e26 9900 0011 620b  HA......N&....b.
-00001500: 543a f400 00e4 3e0b 5467 9000 002b fd0b  T:....>.Tg...+..
-00001510: 6948 d000 00c7 b90b 6b4e 3000 005e 3c0b  iH......kN0..^<.
-00001520: 6f1b 4500 0060 a10b 76dd 9d00 0137 fb0b  o.E..`..v....7..
-00001530: 8a1a 2000 00e5 d50b 8a1a 2000 0113 df0b  .. ....... .....
-00001540: 8c6a e300 0058 800b 9253 4000 0002 280b  .j...X...S@...(.
-00001550: 94b6 5e00 00d1 7f0b 967b 5400 0032 5c0b  ..^......{T..2\.
-00001560: a0c9 de00 0006 5c0b a3fc 0c00 006f 7e0b  ......\......o~.
-00001570: a3fc 7000 00f3 ad0b a4a2 2500 0025 690b  ..p.......%..%i.
-00001580: c474 9000 00de a10b c4a6 f000 0062 f10b  .t...........b..
-00001590: c81a a000 00df 400b cbf1 c000 00e6 280b  ......@.......(.
-000015a0: cbf1 c000 00eb 9b0b cbf1 c000 00f6 230b  ..............#.
-000015b0: cbf1 c000 010b fe0b db2b b200 0026 430b  .........+...&C.
-000015c0: def4 0000 0131 4b0b e203 8700 000f 1f0b  .....1K.........
-000015d0: e217 6300 000e dc0b e4a0 3000 0016 c50b  ..c.......0.....
-000015e0: f39a 4000 003a ce0b f39a 4000 0080 cd0b  ..@..:....@.....
-000015f0: f39a 4000 00cb 800b fc32 3300 0046 290c  ..@......23..F).
-00001600: 04fe c500 0014 360c 0c17 6300 0056 a70c  ......6...c..V..
-00001610: 0ce3 2300 008e 620c 0dec 5a00 007f aa0c  ..#...b...Z.....
-00001620: 1d95 4000 00c2 fa0c 3834 1400 000e 3b0c  ..@.....84....;.
-00001630: 3834 1400 0089 060c 3834 1400 011d 310c  84......84....1.
-00001640: 5256 ae00 0034 730c 5bd6 a000 0008 670c  RV...4s.[.....g.
-00001650: 61ce a500 0035 240c 63ce a500 000b b00c  a....5$.c.......
-00001660: 6dca b800 0038 3e0c 808a a300 00a4 ad0c  m....8>.........
-00001670: 83b7 b000 0037 c40c 8910 0000 0006 9a0c  .....7..........
-00001680: 89ed e500 004a cf0c 98c0 0900 0005 e20c  .....J..........
-00001690: 98c0 0900 000a 8e0c 98c0 0900 000d c70c  ................
-000016a0: 98c0 0900 0082 450c 98c0 0900 0087 d00c  ......E.........
-000016b0: 98c0 0900 009e e90c 98c0 0900 011b 2d0c  ..............-.
-000016c0: 9fa9 6000 0122 bd0c b106 9a00 011f 3c0c  ..`.."........<.
-000016d0: b195 2700 007e b30c b1a8 e500 0031 4c0c  ..'..~.......1L.
-000016e0: ba9f 2400 0113 600c c1c5 c300 0090 510c  ..$...`.......Q.
-000016f0: c4e1 d500 0014 7f0c c5f7 d500 007c a80c  .............|..
-00001700: c7ee 6000 009b d60c c8e8 6400 0030 970c  ..`.......d..0..
-00001710: c9a0 2e00 007d 070c cba2 d500 00ec e30c  .....}..........
-00001720: db0c 0400 00b6 6b0c dda2 6e00 00b3 e80c  ......k...n.....
-00001730: e3ed a900 0090 060c f3b0 8500 0013 190c  ................
-00001740: fb0f b300 0092 f20d 0027 2000 00c1 cd0d  .........' .....
-00001750: 09a5 6000 0120 f20d 0a66 ed00 012a 610d  ..`.. ...f...*a.
-00001760: 0ad7 7300 004d 170d 0f91 6000 00f2 8f0d  ..s..M....`.....
-00001770: 0f91 6000 0107 ba0d 1201 a400 005a cf0d  ..`..........Z..
-00001780: 1cec 6700 011e 680d 2d41 7000 00b0 2b0d  ..g...h.-Ap...+.
-00001790: 32db 3000 00ef 310d 35c6 3000 010b 510d  2.0...1.5.0...Q.
-000017a0: 3b8c 3900 00ad ab0d 48cd 6500 0099 c70d  ;.9.....H.e.....
-000017b0: 51bd f000 00f6 9d0d 69f6 0000 009c 830d  Q.......i.......
-000017c0: 7298 e700 00af 670d 7c3b 4000 0114 a50d  r.....g.|;@.....
-000017d0: 80f6 3400 0096 ce0d 80f6 3400 0098 5e0d  ..4.......4...^.
-000017e0: 8344 9300 008f 480d 8c46 7500 0004 a70d  .D....H..Fu.....
-000017f0: 8c46 7500 00a5 420d 96e3 5000 00e1 540d  .Fu...B...P...T.
-00001800: 9df1 6500 001a 7d0d 9df1 6500 0021 520d  ..e...}...e..!R.
-00001810: 9ee3 5e00 006b 860d 9ee3 5e00 0077 9b0d  ..^..k....^..w..
-00001820: 9ee3 5e00 0084 140d 9ee3 5e00 00a3 710d  ..^.......^...q.
-00001830: 9ee3 5e00 00b8 c20d aa4e 9000 00e8 3d0d  ..^......N....=.
-00001840: c964 7400 00ac 7a0d d0e8 e000 00ca bf0d  .dt...z.........
-00001850: ded8 9000 001d ff0d ded8 9000 0052 ae0d  .............R..
-00001860: eb49 0000 007e eb0d ec49 8400 0048 950d  .I...~...I...H..
-00001870: f086 4a00 0039 b50d fcd5 7e00 003f 300d  ..J..9....~..?0.
-00001880: fe0b 6000 006e 5a0e 00f0 b000 00d6 990e  ..`..nZ.........
-00001890: 03af f000 0076 670e 1bf8 6400 0039 540e  .....vg...d..9T.
-000018a0: 1ddb 6300 0050 c30e 202b 3a00 007d 660e  ..c..P.. +:..}f.
-000018b0: 202b 3a00 0129 c80e 2511 7400 005f 3f0e   +:..)..%.t.._?.
-000018c0: 38a0 f000 0108 da0e 5c13 4700 011c b00e  8.......\.G.....
-000018d0: 6193 e900 0115 d30e 61d5 0400 00aa a60e  a.......a.......
-000018e0: 68cb dc00 0055 7b0e 6ac2 e300 0025 a00e  h....U{.j....%..
-000018f0: 7617 2000 007a d80e 8347 4400 0068 e70e  v. ..z...GD..h..
-00001900: 887b b500 0037 590e 887b b500 00ab 7d0e  .{...7Y..{....}.
-00001910: 9dcc d400 0033 560e a934 c000 005f be0e  .....3V..4..._..
-00001920: abf5 1300 0066 950e ae34 8000 005c f90e  .....f...4...\..
-00001930: b4a5 0a00 0062 8c0e b5c2 8000 009a 290e  .....b........).
-00001940: b803 9900 006d 4a0e b82d 1000 00f7 310e  .....mJ..-....1.
-00001950: c28b b000 0003 0c0e d945 de00 002e 560e  .........E....V.
-00001960: e77d 7000 0125 310e f7f8 4000 00f3 300f  .}p..%1...@...0.
-00001970: 09fd b000 00d8 5d0f 0cc4 c000 00fe 3b0f  ......].......;.
-00001980: 105e a000 00bd 030f 11be 6000 00c2 420f  .^........`...B.
-00001990: 1d28 1000 0101 fd0f 201d 8500 0088 850f  .(...... .......
-000019a0: 20f1 3000 00da 9d0f 4321 f500 0135 b40f   .0.....C!...5..
-000019b0: 4a90 4000 00b5 b20f 5e00 1000 00cc 7b0f  J.@.....^.....{.
-000019c0: 8e7b e000 00d0 dd0f 9222 7c00 00ad 6b0f  .{......."|...k.
-000019d0: 9450 0000 0118 840f 969b 9a00 004f 790f  .P...........Oy.
-000019e0: 9ebd c400 0048 ed0f 9fbc 6000 013a 3e0f  .....H....`..:>.
-000019f0: a262 9000 013c b50f a44f 0300 0000 5f0f  .b...<...O...._.
-00001a00: bd5e e700 011d ca0f cb15 5200 0068 9b0f  .^........R..h..
-00001a10: cf80 f000 00f8 780f d19a 7000 00c3 b30f  ......x...p.....
-00001a20: dfeb 7000 009e 140f e7f7 9000 013c 430f  ..p..........<C.
-00001a30: ea8a 0900 007d ab0f ea8a 0900 00a8 9d0f  .....}..........
-00001a40: ea8a 0900 012a 070f f87c e000 0024 6d0f  .....*...|...$m.
-00001a50: fe37 0300 0086 1069 0001 3d30 0300 0000  .7.....i..=0....
-00001a60: 2404 1e04 4204 3c04 3504 3d04 3804 4204  $...B.<.5.=.8.B.
-00001a70: 4c00 2004 3804 3704 3c04 3504 3d04 3504  L. .8.7.<.5.=.5.
-00001a80: 3d04 3804 4f08 0000 0000 0600 0000 0e43  =.8.O..........C
-00001a90: 616e 6365 6c20 6368 616e 6765 7307 0000  ancel changes...
-00001aa0: 0018 4162 7374 7261 6374 4f70 6572 6174  ..AbstractOperat
-00001ab0: 696f 6e44 6574 6169 6c73 0103 0000 0026  ionDetails.....&
-00001ac0: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
-00001ad0: 044c 0020 0438 0437 043c 0435 043d 0435  .L. .8.7.<.5.=.5
-00001ae0: 043d 0438 044f 0800 0000 0006 0000 000e  .=.8.O..........
-00001af0: 436f 6d6d 6974 2063 6861 6e67 6573 0700  Commit changes..
-00001b00: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
-00001b10: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
-00001b20: 3804 1e04 4804 3804 3104 3a04 3000 2004  8...H.8.1.:.0. .
-00001b30: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
-00001b40: 4104 3800 2004 3e04 3f04 3504 4004 3004  A.8. .>.?.5.@.0.
-00001b50: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
-00001b60: 0000 194f 7065 7261 7469 6f6e 2073 7562  ...Operation sub
-00001b70: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
-00001b80: 1841 6273 7472 6163 744f 7065 7261 7469  .AbstractOperati
-00001b90: 6f6e 4465 7461 696c 7301 0300 0000 8804  onDetails.......
-00001ba0: 1d04 3504 4104 3e04 4504 4004 3004 3d04  ..5.A.>.E.@.0.=.
-00001bb0: 5104 3d04 3d04 4b04 3500 2004 3804 3704  Q.=.=.K.5. .8.7.
-00001bc0: 3c04 3504 3d04 3504 3d04 3804 4f00 2004  <.5.=.5.=.8.O. .
-00001bd0: 3104 4b04 3b04 3800 2004 3e04 4204 3c04  1.K.;.8. .>.B.<.
-00001be0: 3504 3d04 3504 3d04 4b00 2004 3f04 3504  5.=.5.=.K. .?.5.
-00001bf0: 4004 3504 3400 2004 4104 3e04 3704 3404  @.5.4. .A.>.7.4.
-00001c00: 3004 3d04 3804 3504 3c00 2004 3d04 3e04  0.=.8.5.<. .=.>.
-00001c10: 3204 3e04 3900 2004 3e04 3f04 3504 4004  2.>.9. .>.?.5.@.
-00001c20: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
-00001c30: 3555 6e73 6176 6564 2063 6861 6e67 6573  5Unsaved changes
-00001c40: 2077 6572 6520 7265 7665 7274 6564 2074   were reverted t
-00001c50: 6f20 6372 6561 7465 206e 6577 206f 7065  o create new ope
-00001c60: 7261 7469 6f6e 0700 0000 1841 6273 7472  ration.....Abstr
-00001c70: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
-00001c80: 696c 7301 0300 0000 3a04 1d04 3504 3204  ils.....:...5.2.
-00001c90: 3504 4004 3d04 3e04 3500 2004 3704 3d04  5.@.=.>.5. .7.=.
-00001ca0: 3004 4704 3504 3d04 3804 3500 2004 3200  0.G.5.=.8.5. .2.
-00001cb0: 2004 4104 4204 3e04 3b04 3104 4604 3500   .A.B.>.;.1.F.5.
-00001cc0: 3a00 2008 0000 0000 0600 0000 1b43 6f6c  :. ..........Col
-00001cd0: 756d 6e20 6861 7320 6e6f 2076 616c 6964  umn has no valid
-00001ce0: 2076 616c 7565 3a20 0700 0000 1a41 6273   value: .....Abs
-00001cf0: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
-00001d00: 7374 4d6f 6465 6c01 0300 0000 1e04 1d04  stModel.........
-00001d10: 3504 3f04 3e04 3b04 3d04 4b04 3500 2004  5.?.>.;.=.K.5. .
-00001d20: 3404 3004 3d04 3d04 4b04 3508 0000 0000  4.0.=.=.K.5.....
-00001d30: 0600 0000 1344 6174 6120 6172 6520 696e  .....Data are in
-00001d40: 636f 6d70 6c65 7465 0700 0000 1a41 6273  complete.....Abs
-00001d50: 7472 6163 7452 6566 6572 656e 6365 4c69  tractReferenceLi
-00001d60: 7374 4d6f 6465 6c01 0300 0000 2604 1e04  stModel.....&...
-00001d70: 4804 3804 3104 3a04 3000 2004 4104 3e04  H.8.1.:.0. .A.>.
-00001d80: 4504 4004 3004 3d04 3504 3d04 3804 4f00  E.@.0.=.5.=.8.O.
-00001d90: 3a00 2008 0000 0000 0600 0000 0f53 7562  :. ..........Sub
-00001da0: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
-00001db0: 1a41 6273 7472 6163 7452 6566 6572 656e  .AbstractReferen
-00001dc0: 6365 4c69 7374 4d6f 6465 6c01 0300 0000  ceListModel.....
-00001dd0: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
-00001de0: 0600 0000 0341 4e59 0700 0000 0d41 6363  .....ANY.....Acc
-00001df0: 6f75 6e74 4275 7474 6f6e 0103 0000 0014  ountButton......
-00001e00: 041b 044e 0431 043e 0439 0020 0441 0447  ...N.1.>.9. .A.G
-00001e10: 0435 0442 0800 0000 0006 0000 000b 416e  .5.B..........An
-00001e20: 7920 6163 636f 756e 7407 0000 000d 4163  y account.....Ac
-00001e30: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
-00001e40: 1804 1204 4b04 3104 4004 3004 4204 4c00  ....K.1.@.0.B.L.
-00001e50: 2004 4104 4704 3504 4208 0000 0000 0600   .A.G.5.B.......
-00001e60: 0000 0e43 686f 6f73 6520 6163 636f 756e  ...Choose accoun
-00001e70: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
-00001e80: 746f 6e01 0300 0000 1404 2204 3804 3f00  ton.......".8.?.
-00001e90: 2004 4104 4704 3504 4204 3000 3a08 0000   .A.G.5.B.0.:...
-00001ea0: 0000 0600 0000 0d41 6363 6f75 6e74 2074  .......Account t
-00001eb0: 7970 653a 0700 0000 1141 6363 6f75 6e74  ype:.....Account
-00001ec0: 4c69 7374 4469 616c 6f67 0103 0000 000a  ListDialog......
-00001ed0: 0421 0447 0435 0442 0430 0800 0000 0006  .!.G.5.B.0......
-00001ee0: 0000 0008 4163 636f 756e 7473 0700 0000  ....Accounts....
-00001ef0: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
-00001f00: 6f67 0103 0000 002a 041f 043e 043a 0430  og.....*...>.:.0
-00001f10: 0437 044b 0432 0430 0442 044c 0020 043d  .7.K.2.0.B.L. .=
-00001f20: 0435 0430 043a 0442 0438 0432 043d 044b  .5.0.:.B.8.2.=.K
-00001f30: 0435 0800 0000 0006 0000 000d 5368 6f77  .5..........Show
-00001f40: 2069 6e61 6374 6976 6507 0000 0011 4163   inactive.....Ac
-00001f50: 636f 756e 744c 6973 7444 6961 6c6f 6701  countListDialog.
-00001f60: 0300 0000 0e21 1600 2004 4104 4704 3504  .....!.. .A.G.5.
-00001f70: 4204 3008 0000 0000 0600 0000 0941 6363  B.0..........Acc
-00001f80: 6f75 6e74 2023 0700 0000 1041 6363 6f75  ount #.....Accou
-00001f90: 6e74 4c69 7374 4d6f 6465 6c01 0300 0000  ntListModel.....
-00001fa0: 0804 1004 3a04 4200 2e08 0000 0000 0600  ....:.B.........
-00001fb0: 0000 0441 6374 2e07 0000 0010 4163 636f  ...Act......Acco
-00001fc0: 756e 744c 6973 744d 6f64 656c 0103 0000  untListModel....
-00001fd0: 0016 0411 0430 043d 043a 002f 0411 0440  .....0.=.:./...@
-00001fe0: 043e 043a 0435 0440 0800 0000 0006 0000  .>.:.5.@........
-00001ff0: 000b 4261 6e6b 2f42 726f 6b65 7207 0000  ..Bank/Broker...
-00002000: 0010 4163 636f 756e 744c 6973 744d 6f64  ..AccountListMod
-00002010: 656c 0103 0000 0004 041a 0421 0800 0000  el.........!....
-00002020: 0006 0000 0002 4343 0700 0000 1041 6363  ......CC.....Acc
-00002030: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
-00002040: 0000 0c04 1204 3004 3b04 4e04 4204 3008  ......0.;.N.B.0.
-00002050: 0000 0000 0600 0000 0843 7572 7265 6e63  .........Currenc
-00002060: 7907 0000 0010 4163 636f 756e 744c 6973  y.....AccountLis
-00002070: 744d 6f64 656c 0103 0000 0018 041d 0430  tModel.........0
-00002080: 0438 043c 0435 043d 043e 0432 0430 043d  .8.<.5.=.>.2.0.=
-00002090: 0438 0435 0800 0000 0006 0000 0004 4e61  .8.5..........Na
-000020a0: 6d65 0700 0000 1041 6363 6f75 6e74 4c69  me.....AccountLi
-000020b0: 7374 4d6f 6465 6c01 0300 0000 1004 2204  stModel.......".
-000020c0: 3e04 4704 3d04 3e04 4104 4204 4c08 0000  >.G.=.>.A.B.L...
-000020d0: 0000 0600 0000 0950 7265 6369 7369 6f6e  .......Precision
-000020e0: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
-000020f0: 4d6f 6465 6c01 0300 0000 1004 2104 3204  Model.......!.2.
-00002100: 3504 4004 3504 3d00 2000 4008 0000 0000  5.@.5.=. .@.....
-00002110: 0600 0000 0c52 6563 6f6e 6369 6c65 6420  .....Reconciled 
-00002120: 4007 0000 0010 4163 636f 756e 744c 6973  @.....AccountLis
-00002130: 744d 6f64 656c 0103 0000 001a 0426 0435  tModel.......&.5
-00002140: 043d 043d 0430 044f 0020 0431 0443 043c  .=.=.0.O. .1.C.<
-00002150: 0430 0433 0430 0800 0000 0006 0000 0005  .0.3.0..........
-00002160: 4173 7365 7407 0000 000b 4173 7365 7444  Asset.....AssetD
-00002170: 6961 6c6f 6701 0300 0000 3e04 1e04 4804  ialog.....>...H.
-00002180: 3804 3104 3a04 3000 2004 3704 3004 3f04  8.1.:.0. .7.0.?.
-00002190: 3804 4104 3800 2004 3804 3d04 4404 3e04  8.A.8. .8.=.D.>.
-000021a0: 4004 3c04 3004 4604 3804 3800 2004 3e00  @.<.0.F.8.8. .>.
-000021b0: 2004 2604 1100 3a00 2008 0000 0000 0600   .&...:. .......
-000021c0: 0000 1d41 7373 6574 2064 6574 6169 6c73  ...Asset details
-000021d0: 2073 7562 6d69 7420 6661 696c 6564 3a20   submit failed: 
-000021e0: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
-000021f0: 0103 0000 0024 041e 0448 0438 0431 043a  .....$...H.8.1.:
-00002200: 0430 0020 0437 0430 043f 0438 0441 0438  .0. .7.0.?.8.A.8
-00002210: 0020 0426 0415 003a 0020 0800 0000 0006  . .&...:. ......
-00002220: 0000 0015 4173 7365 7420 7375 626d 6974  ....Asset submit
-00002230: 2066 6169 6c65 643a 2007 0000 000b 4173   failed: .....As
-00002240: 7365 7444 6961 6c6f 6701 0300 0000 1c04  setDialog.......
-00002250: 1104 3004 3704 3e04 3204 4b04 3900 2004  ..0.7.>.2.K.9. .
-00002260: 3004 3a04 4204 3804 3200 3a08 0000 0000  0.:.B.8.2.:.....
-00002270: 0600 0000 0b42 6173 6520 6173 7365 743a  .....Base asset:
-00002280: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
-00002290: 0103 0000 000c 041e 0442 043c 0435 043d  .........B.<.5.=
-000022a0: 0430 0800 0000 0006 0000 0006 4361 6e63  .0..........Canc
-000022b0: 656c 0700 0000 0b41 7373 6574 4469 616c  el.....AssetDial
-000022c0: 6f67 0103 0000 0010 0421 0442 0440 0430  og.......!.B.@.0
-000022d0: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
-000022e0: 0009 436f 756e 7472 793a 2007 0000 000b  ..Country: .....
-000022f0: 4173 7365 7444 6961 6c6f 6701 0300 0000  AssetDialog.....
-00002300: 1404 1404 3e04 3f00 2e04 3404 3004 3d04  ....>.?...4.0.=.
-00002310: 3d04 4b04 3508 0000 0000 0600 0000 0a45  =.K.5..........E
-00002320: 7874 7261 2064 6174 6107 0000 000b 4173  xtra data.....As
-00002330: 7365 7444 6961 6c6f 6701 0300 0000 0a00  setDialog.......
-00002340: 4900 5300 4900 4e00 3a08 0000 0000 0600  I.S.I.N.:.......
-00002350: 0000 0549 5349 4e3a 0700 0000 0b41 7373  ...ISIN:.....Ass
-00002360: 6574 4469 616c 6f67 0103 0000 001a 041d  etDialog........
-00002370: 0430 0438 043c 0435 043d 043e 0432 0430  .0.8.<.5.=.>.2.0
-00002380: 043d 0438 0435 003a 0800 0000 0006 0000  .=.8.5.:........
-00002390: 0005 4e61 6d65 3a07 0000 000b 4173 7365  ..Name:.....Asse
-000023a0: 7444 6961 6c6f 6701 0300 0000 0404 1e04  tDialog.........
-000023b0: 1a08 0000 0000 0600 0000 024f 4b07 0000  ...........OK...
-000023c0: 000b 4173 7365 7444 6961 6c6f 6701 0300  ..AssetDialog...
-000023d0: 0000 0e04 2104 3804 3c04 3204 3e04 3b04  ....!.8.<.2.>.;.
-000023e0: 4b08 0000 0000 0600 0000 0753 796d 626f  K..........Symbo
-000023f0: 6c73 0700 0000 0b41 7373 6574 4469 616c  ls.....AssetDial
-00002400: 6f67 0103 0000 000a 0422 0438 043f 003a  og.......".8.?.:
-00002410: 0020 0800 0000 0006 0000 0006 5479 7065  . ..........Type
-00002420: 3a20 0700 0000 0b41 7373 6574 4469 616c  : .....AssetDial
-00002430: 6f67 0103 0000 000e 0422 0438 043f 0020  og.......".8.?. 
-00002440: 0426 0411 003a 0800 0000 0006 0000 000b  .&...:..........
-00002450: 4173 7365 7420 7479 7065 3a07 0000 000f  Asset type:.....
-00002460: 4173 7365 744c 6973 7444 6961 6c6f 6701  AssetListDialog.
-00002470: 0300 0000 1a04 2604 3504 3d04 3d04 4b04  ......&.5.=.=.K.
-00002480: 3500 2004 3104 4304 3c04 3004 3304 3808  5. .1.C.<.0.3.8.
-00002490: 0000 0000 0600 0000 0641 7373 6574 7307  .........Assets.
-000024a0: 0000 000f 4173 7365 744c 6973 7444 6961  ....AssetListDia
-000024b0: 6c6f 6701 0300 0000 0c04 2104 4204 4004  log.......!.B.@.
-000024c0: 3004 3d04 3008 0000 0000 0600 0000 0743  0.=.0..........C
-000024d0: 6f75 6e74 7279 0700 0000 0e41 7373 6574  ountry.....Asset
-000024e0: 4c69 7374 4d6f 6465 6c01 0300 0000 0c04  ListModel.......
-000024f0: 1204 3004 3b04 4e04 4204 3008 0000 0000  ..0.;.N.B.0.....
-00002500: 0600 0000 0843 7572 7265 6e63 7907 0000  .....Currency...
-00002510: 000e 4173 7365 744c 6973 744d 6f64 656c  ..AssetListModel
-00002520: 0103 0000 001a 0418 0441 0442 002e 043a  .........A.B...:
-00002530: 043e 0442 0438 0440 043e 0432 043e 043a  .>.B.8.@.>.2.>.:
-00002540: 0800 0000 0006 0000 000b 4461 7461 2073  ..........Data s
-00002550: 6f75 7263 6507 0000 000e 4173 7365 744c  ource.....AssetL
-00002560: 6973 744d 6f64 656c 0103 0000 0008 0049  istModel.......I
-00002570: 0053 0049 004e 0800 0000 0006 0000 0004  .S.I.N..........
-00002580: 4953 494e 0700 0000 0e41 7373 6574 4c69  ISIN.....AssetLi
-00002590: 7374 4d6f 6465 6c01 0300 0000 1804 1d04  stModel.........
-000025a0: 3004 3804 3c04 3504 3d04 3e04 3204 3004  0.8.<.5.=.>.2.0.
-000025b0: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
-000025c0: 616d 6507 0000 000e 4173 7365 744c 6973  ame.....AssetLis
-000025d0: 744d 6f64 656c 0103 0000 000c 0421 0438  tModel.......!.8
-000025e0: 043c 0432 043e 043b 0800 0000 0006 0000  .<.2.>.;........
-000025f0: 0006 5379 6d62 6f6c 0700 0000 0e41 7373  ..Symbol.....Ass
-00002600: 6574 4c69 7374 4d6f 6465 6c01 0300 0000  etListModel.....
-00002610: 1804 1d04 3004 3804 3c04 3504 3d04 3e04  ....0.8.<.5.=.>.
-00002620: 3204 3004 3d04 3804 3508 0000 0000 0600  2.0.=.8.5.......
-00002630: 0000 0a41 7373 6574 206e 616d 6507 0000  ...Asset name...
-00002640: 000f 4173 7365 7473 4c69 7374 4d6f 6465  ..AssetsListMode
-00002650: 6c01 0300 0000 1a04 1104 3004 3704 3e04  l.........0.7.>.
-00002660: 3204 4b04 3900 2004 3004 3a04 4204 3804  2.K.9. .0.:.B.8.
-00002670: 3208 0000 0000 0600 0000 0a42 6173 6520  2..........Base 
-00002680: 6173 7365 7407 0000 000f 4173 7365 7473  asset.....Assets
-00002690: 4c69 7374 4d6f 6465 6c01 0300 0000 0c04  ListModel.......
-000026a0: 2104 4204 4004 3004 3d04 3008 0000 0000  !.B.@.0.=.0.....
-000026b0: 0600 0000 0743 6f75 6e74 7279 0700 0000  .....Country....
-000026c0: 0f41 7373 6574 734c 6973 744d 6f64 656c  .AssetsListModel
-000026d0: 0103 0000 0008 0049 0053 0049 004e 0800  .......I.S.I.N..
-000026e0: 0000 0006 0000 0004 4953 494e 0700 0000  ........ISIN....
-000026f0: 0f41 7373 6574 734c 6973 744d 6f64 656c  .AssetsListModel
-00002700: 0103 0000 0008 0421 0447 0435 0442 0800  .......!.G.5.B..
-00002710: 0000 0006 0000 0007 4163 636f 756e 7407  ........Account.
-00002720: 0000 000d 4261 6c61 6e63 6573 4d6f 6465  ....BalancesMode
-00002730: 6c01 0300 0000 0c04 1104 3004 3b04 3004  l.........0.;.0.
-00002740: 3d04 4108 0000 0000 0600 0000 0742 616c  =.A..........Bal
-00002750: 616e 6365 0700 0000 0d42 616c 616e 6365  ance.....Balance
-00002760: 734d 6f64 656c 0103 0000 0010 0411 0430  sModel.........0
-00002770: 043b 0430 043d 0441 002c 0020 0800 0000  .;.0.=.A.,. ....
-00002780: 0006 0000 0009 4261 6c61 6e63 652c 2007  ......Balance, .
-00002790: 0000 000d 4261 6c61 6e63 6573 4d6f 6465  ....BalancesMode
-000027a0: 6c01 0300 0000 0a04 1804 4204 3e04 3304  l.........B.>.3.
-000027b0: 3e08 0000 0000 0600 0000 0554 6f74 616c  >..........Total
-000027c0: 0700 0000 0d42 616c 616e 6365 734d 6f64  .....BalancesMod
-000027d0: 656c 0103 0000 001c 0411 0430 0437 043e  el.........0.7.>
-000027e0: 0432 0430 044f 0020 0432 0430 043b 044e  .2.0.O. .2.0.;.N
-000027f0: 0442 0430 0800 0000 0006 0000 000d 4261  .B.0..........Ba
-00002800: 7365 2063 7572 7265 6e63 7907 0000 0012  se currency.....
-00002810: 4261 7365 4375 7272 656e 6379 4469 616c  BaseCurrencyDial
-00002820: 6f67 0103 0000 000c 0412 0430 043b 044e  og.........0.;.N
-00002830: 0442 0430 0800 0000 0006 0000 0008 4375  .B.0..........Cu
-00002840: 7272 656e 6379 0700 0000 1542 6173 6543  rrency.....BaseC
-00002850: 7572 7265 6e63 794c 6973 744d 6f64 656c  urrencyListModel
-00002860: 0103 0000 0008 0414 0430 0442 0430 0800  .........0.B.0..
-00002870: 0000 0006 0000 0004 4461 7465 0700 0000  ........Date....
-00002880: 1542 6173 6543 7572 7265 6e63 794c 6973  .BaseCurrencyLis
-00002890: 744d 6f64 656c 0103 0000 0024 0027 0020  tModel.....$.'. 
-000028a0: 0437 0430 043c 0435 043d 0435 043d 0430  .7.0.<.5.=.5.=.0
-000028b0: 0020 0443 0441 043f 0435 0448 043d 043e  . .C.A.?.5.H.=.>
-000028c0: 0800 0000 0006 0000 001b 2720 7761 7320  ..........' was 
-000028d0: 7375 6363 6573 7366 756c 6c79 2072 6570  successfully rep
-000028e0: 6c61 6365 6407 0000 0012 4361 7465 676f  laced.....Catego
-000028f0: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
-00002900: 000c 0027 0020 043d 0430 003a 0020 0800  ...'. .=.0.:. ..
-00002910: 0000 0006 0000 0008 2720 7769 7468 3a20  ........' with: 
-00002920: 0700 0000 1243 6174 6567 6f72 794c 6973  .....CategoryLis
-00002930: 7444 6961 6c6f 6701 0300 0000 1204 1a04  tDialog.........
-00002940: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
-00002950: 0000 0000 0600 0000 0a43 6174 6567 6f72  .........Categor
-00002960: 6965 7307 0000 0012 4361 7465 676f 7279  ies.....Category
-00002970: 4c69 7374 4469 616c 6f67 0103 0000 0016  ListDialog......
-00002980: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
-00002990: 044f 0020 0027 0800 0000 0006 0000 000a  .O. .'..........
-000029a0: 4361 7465 676f 7279 2027 0700 0000 1243  Category '.....C
-000029b0: 6174 6567 6f72 794c 6973 7444 6961 6c6f  ategoryListDialo
-000029c0: 6701 0300 0000 2804 1704 3004 3c04 3504  g.....(...0.<.5.
-000029d0: 3d04 3804 4204 4c00 2004 3a04 3004 4204  =.8.B.L. .:.0.B.
-000029e0: 3504 3304 3e04 4004 3804 4e00 2000 2708  5.3.>.@.8.N. .'.
-000029f0: 0000 0000 0600 0000 1252 6570 6c61 6365  .........Replace
-00002a00: 2063 6174 6567 6f72 7920 2707 0000 0012   category '.....
-00002a10: 4361 7465 676f 7279 4c69 7374 4469 616c  CategoryListDial
-00002a20: 6f67 0103 0000 001c 0417 0430 043c 0435  og.........0.<.5
-00002a30: 043d 0438 0442 044c 0020 043d 0430 002e  .=.8.B.L. .=.0..
-00002a40: 002e 002e 0800 0000 0006 0000 000f 5265  ..............Re
-00002a50: 706c 6163 6520 7769 7468 2e2e 2e07 0000  place with......
-00002a60: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
-00002a70: 616c 6f67 0103 0000 003c 041f 043e 043a  alog.....<...>.:
-00002a80: 0430 0437 0430 0442 044c 0020 043e 043f  .0.7.0.B.L. .>.?
-00002a90: 0435 0440 0430 0446 0438 0438 0020 0441  .5.@.0.F.8.8. .A
-00002aa0: 0020 041a 0430 0442 0435 0433 043e 0440  . ...0.B.5.3.>.@
-00002ab0: 0438 0435 0439 0800 0000 0006 0000 001d  .8.5.9..........
-00002ac0: 5368 6f77 206f 7065 7261 7469 6f6e 7320  Show operations 
-00002ad0: 7769 7468 2043 6174 6567 6f72 7907 0000  with Category...
-00002ae0: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
-00002af0: 616c 6f67 0103 0000 0010 041e 043f 0435  alog.........?.5
-00002b00: 0440 0430 0446 0438 0438 0800 0000 0006  .@.0.F.8.8......
-00002b10: 0000 000a 4f70 6572 6174 696f 6e73 0700  ....Operations..
-00002b20: 0000 0e43 6174 6567 6f72 7952 6570 6f72  ...CategoryRepor
-00002b30: 7401 0300 0000 1804 3f04 3e00 2004 1a04  t.......?.>. ...
-00002b40: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
-00002b50: 0000 0000 0600 0000 0b62 7920 4361 7465  .........by Cate
-00002b60: 676f 7279 0700 0000 0e43 6174 6567 6f72  gory.....Categor
-00002b70: 7952 6570 6f72 7401 0300 0000 1404 1a04  yReport.........
-00002b80: 3004 4204 3504 3304 3e04 4004 3804 4f00  0.B.5.3.>.@.8.O.
-00002b90: 3a08 0000 0000 0600 0000 0943 6174 6567  :..........Categ
-00002ba0: 6f72 793a 0700 0000 1443 6174 6567 6f72  ory:.....Categor
-00002bb0: 7952 6570 6f72 7457 6964 6765 7401 0300  yReportWidget...
-00002bc0: 0000 2404 1e04 4204 4704 5104 4200 2004  ..$...B.G.Q.B. .
-00002bd0: 3f04 3e00 2004 3a04 3004 4204 3504 3304  ?.>. .:.0.B.5.3.
+00000010: a700 0000 0572 755f 5255 4200 001a d000  .....ru_RUB.....
+00000020: 0000 2300 001c 2500 0000 2300 0030 b900  ..#...%...#..0..
+00000030: 0000 2300 0139 5b00 0000 2300 013e 0b00  ..#..9[...#..>..
+00000040: 0000 2500 0096 ed00 0004 7300 0005 b700  ..%.......s.....
+00000050: 0005 3b00 0009 4c00 0005 af00 013f bc00  ..;...L......?..
+00000060: 0007 db00 00ad ca00 0031 0e00 0082 9100  .........1......
+00000070: 0031 0e00 012d 2f00 0046 3900 0003 7000  .1...-/..F9...p.
+00000080: 0046 3900 00a7 5800 0047 a400 0048 9c00  .F9...X..G...H..
+00000090: 0048 7200 0097 1400 0048 7200 00ab ba00  .Hr......Hr.....
+000000a0: 0048 b700 0097 6f00 0048 b700 00ab e600  .H....o..H......
+000000b0: 004a 7a00 004a 9a00 004a b300 0098 1d00  .Jz..J...J......
+000000c0: 004a b300 00ac 1200 004b 1a00 004a c500  .J.......K...J..
+000000d0: 004b 3a00 004a f000 004c b200 0098 8900  .K:..J...L......
+000000e0: 004c b200 00ac 3e00 004c b500 0013 bf00  .L....>..L......
+000000f0: 004c b500 013a 5f00 0050 7e00 0099 3200  .L...:_..P~...2.
+00000100: 0050 7e00 00ac 6a00 0051 3100 001e df00  .P~...j..Q1.....
+00000110: 0051 3100 0032 2a00 0051 3100 0037 6800  .Q1..2*..Q1..7h.
+00000120: 0051 bc00 0099 5f00 0051 bc00 00ac 9600  .Q...._..Q......
+00000130: 0051 be00 0099 8c00 0051 be00 00ac c200  .Q.......Q......
+00000140: 0052 ac00 009a 9a00 0052 ac00 009c f300  .R.......R......
+00000150: 0053 3c00 0015 2300 0053 3c00 0037 cd00  .S<...#..S<..7..
+00000160: 0053 8200 0099 b900 0053 8200 00ac ee00  .S.......S......
+00000170: 0053 8900 0099 e600 0053 8900 00ad 1a00  .S.......S......
+00000180: 0055 6600 009a 4000 0055 6600 00ad 4600  .Uf...@..Uf...F.
+00000190: 0055 a400 009a 6d00 0055 a400 00ad 7200  .U....m..U....r.
+000001a0: 0058 b900 0015 8a00 0058 b900 0020 5e00  .X.......X... ^.
+000001b0: 0058 b900 0038 2c00 0058 b900 00b0 a500  .X...8,..X......
+000001c0: 0058 b900 0129 3700 0058 b900 013a f300  .X...)7..X...:..
+000001d0: 0059 c000 009b 9100 0059 c000 00ad 9e00  .Y.......Y......
+000001e0: 005a 7700 002c 7500 005a 7700 003c 1400  .Zw..,u..Zw..<..
+000001f0: 005a 7700 008e 3000 005a 7700 0123 3a00  .Zw...0..Zw..#:.
+00000200: 005a 8800 0033 9f00 005b 2a00 0027 9500  .Z...3...[*..'..
+00000210: 0070 7c00 005f 4200 007a 7700 0025 a000  .p|.._B..zw..%..
+00000220: 047a 6e00 0005 4000 047a 6e00 0122 1c00  .zn...@..zn.."..
+00000230: 0498 9800 0093 7b00 04a6 7900 0072 6900  ......{...y..ri.
+00000240: 04a6 7900 0089 b700 04a8 a500 000e 0500  ..y.............
+00000250: 04a8 a500 00a4 7900 04a8 a500 0128 8700  ......y......(..
+00000260: 04a8 d300 0095 ec00 04cb c300 0098 b600  ................
+00000270: 04cf 3a00 0036 6400 04d9 5d00 013f 5c00  ..:..6d...]..?\.
+00000280: 04e3 1a00 0077 ce00 04e7 de00 000b 0d00  .....w..........
+00000290: 04e7 de00 000c 7500 0504 cf00 007d 4c00  ......u......}L.
+000002a0: 0528 a400 0036 9400 0548 3500 0006 1b00  .(...6...H5.....
+000002b0: 0548 3500 000b 3c00 0548 3500 0011 c100  .H5...<..H5.....
+000002c0: 0548 3500 0092 b100 0556 a500 0013 f800  .H5......V......
+000002d0: 0556 a500 001f 1200 0556 a500 002c 4000  .V.......V...,@.
+000002e0: 0556 a500 0032 9b00 0556 a500 0056 6800  .V...2...V...Vh.
+000002f0: 0556 a500 013a 9200 0556 a500 013f 8500  .V...:...V...?..
+00000300: 0565 c000 0046 a900 0566 be00 0037 9300  .e...F...f...7..
+00000310: 0566 be00 0128 b900 056b c200 0058 1700  .f...(...k...X..
+00000320: 05a3 0000 004e b400 05a7 aa00 0124 1d00  .....N.......$..
+00000330: 05a7 e300 0126 2d00 05b3 d800 0127 5600  .....&-......'V.
+00000340: 05c0 6500 0021 a300 05c0 6500 0033 cf00  ..e..!....e..3..
+00000350: 05db bb00 0027 c400 05fb 8200 0027 fa00  .....'.......'..
+00000360: 1530 3000 0012 3a00 18d1 5000 00f6 2800  .00...:...P...(.
+00000370: 2311 0000 012d 0200 26f2 9100 004e e000  #....-..&....N..
+00000380: 2aa8 a100 0059 c600 2acf 0400 0059 fc00  *....Y..*....Y..
+00000390: 2b37 fe00 005a a200 2b76 1e00 008a 8600  +7...Z..+v......
+000003a0: 2ba7 e300 005c a600 2ec7 e000 0048 3b00  +....\.......H;.
+000003b0: 3153 c400 0098 ee00 3d1a 0e00 005e 9d00  1S......=....^..
+000003c0: 4182 8900 0107 2700 4796 c400 007a 8200  A.....'.G....z..
+000003d0: 47af 8000 00a0 8800 48a9 c400 0006 db00  G.......H.......
+000003e0: 48a9 c400 0012 8a00 48a9 c400 001c da00  H.......H.......
+000003f0: 48a9 c400 002a 0300 48a9 c400 0031 1100  H....*..H....1..
+00000400: 48a9 c400 0039 4200 48a9 c400 00a4 1400  H....9B.H.......
+00000410: 48a9 c400 00b0 7500 48a9 c400 0139 ad00  H.....u.H....9..
+00000420: 48a9 c400 013e 6400 4964 b300 0094 e800  H....>d.Id......
+00000430: 4988 b300 0093 4100 4a2b 8200 0049 a400  I.....A.J+...I..
+00000440: 4a2b 8200 0072 3600 4a36 9500 002a b200  J+...r6.J6...*..
+00000450: 4a36 9500 0049 db00 4a36 9500 0076 da00  J6...I..J6...v..
+00000460: 4a71 ec00 0025 3100 4ab8 3300 0028 fe00  Jq...%1.J.3..(..
+00000470: 4ab8 3300 002b 4500 4b6b 9000 010b ca00  J.3..+E.Kk......
+00000480: 4d68 c800 0096 1c00 4d96 0a00 0026 0900  Mh......M....&..
+00000490: 4dc4 b300 0096 5100 4e7e 1a00 0008 de00  M.....Q.N~......
+000004a0: 522b 5a00 0077 1000 52e9 5500 0014 d900  R+Z..w..R.U.....
+000004b0: 5308 d400 009a fd00 535d fe00 0077 fd00  S.......S]...w..
+000004c0: 5464 c900 0037 3500 5464 c900 0096 8400  Td...75.Td......
+000004d0: 5464 c900 009a 1300 5465 a800 0026 3800  Td......Te...&8.
+000004e0: 5483 8a00 0009 0d00 556a c300 0087 d500  T.......Uj......
+000004f0: 55da be00 0012 0300 56bc 5a00 004d 6f00  U.......V.Z..Mo.
+00000500: 56bc 5a00 0091 a000 56bc 9300 008f c000  V.Z.....V.......
+00000510: 578f 9500 0032 d200 578f 9500 013a c600  W....2..W....:..
+00000520: 57a1 7200 0027 5000 5839 2400 006c a200  W.r..'P.X9$..l..
+00000530: 58c6 a500 00a4 a900 5948 5c00 0051 2f00  X.......YH\..Q/.
+00000540: 5948 5c00 0127 8a00 5a73 0400 001a 4a00  YH\..'..Zs....J.
+00000550: 5a73 0400 0021 1900 5a79 2700 0125 f700  Zs...!..Zy'..%..
+00000560: 5a8a e000 0129 a400 5a8b c000 0030 1400  Z....)..Z....0..
+00000570: 5a8e c300 009b be00 5a8e c300 0136 4000  Z.......Z....6@.
+00000580: 5b6a 7c00 000d 4600 5b6a 7c00 009b f300  [j|...F.[j|.....
+00000590: 5c06 8a00 004f 6a00 5c83 b500 0035 9200  \....Oj.\....5..
+000005a0: 5c83 b500 0038 9500 5fb8 5a00 0085 ab00  \....8.._.Z.....
+000005b0: 5fb8 5a00 0137 a400 602e 0a00 0057 b500  _.Z..7..`....W..
+000005c0: 67f7 0000 00ff 7700 70c5 c000 00cf 1500  g.....w.p.......
+000005d0: 80a8 e500 004c ab00 81bc 0000 00d6 1800  .....L..........
+000005e0: 918d 3700 003f 1d00 931f 2000 00e0 ca00  ..7..?.... .....
+000005f0: 9472 3000 0071 db00 9688 5400 00db ad00  .r0..q....T.....
+00000600: ab81 4000 0120 2800 af00 f000 00bc d400  ..@.. (.........
+00000610: af26 4500 012d 8600 b27d 9f00 007d e200  .&E..-...}...}..
+00000620: b4d0 c500 002a 4800 b643 0000 00c9 9a00  .....*H..C......
+00000630: c9db ba00 0064 9f00 cfb0 f400 0031 b700  .....d.......1..
+00000640: e1f3 f000 0017 8d00 e25b 3000 002d 9f00  .........[0..-..
+00000650: ed2c 2500 0028 2a00 fbe4 b100 004b 1b00  .,%..(*......K..
+00000660: ff6b fe00 00ba 1201 11c0 6000 0141 f401  .k........`..A..
+00000670: 1c4b f000 011c d801 2273 8300 0092 ef01  .K......"s......
+00000680: 24a2 9700 003f d401 2bca d000 00a2 fd01  $....?..+.......
+00000690: 3502 c000 00cb 6901 473b 2300 0073 7301  5.....i.G;#..ss.
+000006a0: 5567 7000 00d5 7101 59b4 9000 001b 0d01  Ugp...q.Y.......
+000006b0: 610d fd00 00d1 ae01 6654 9000 003e 1401  a.......fT...>..
+000006c0: 7248 d000 0036 ce01 776d e000 00dc cd01  rH...6..wm......
+000006d0: 78c3 f500 0032 5601 7e51 ea00 0133 f501  x....2V.~Q...3..
+000006e0: 873b 2300 0073 a501 887c d300 005f 6e01  .;#..s...|..._n.
+000006f0: 9687 c000 0112 b301 98a7 5300 004f 9901  ..........S..O..
+00000700: a469 f900 0109 c301 a885 4000 013d 2f01  .i........@..=/.
+00000710: aff7 3300 0000 0001 bef6 7000 00d9 cb01  ..3.......p.....
+00000720: c26a 9a00 00a7 8d01 ce0a 1200 0090 a901  .j..............
+00000730: d48e 5000 0046 0501 da69 b000 011c 6b01  ..P..F...i....k.
+00000740: e128 5000 00c6 a001 e26a 9a00 0004 2801  .(P......j....(.
+00000750: f571 7000 00c3 af02 00dd 0100 0047 4702  .qp..........GG.
+00000760: 01b8 4900 003d 6a02 01b8 4900 008c e502  ..I..=j...I.....
+00000770: 01b8 4900 00a7 1802 01b8 4900 0141 1c02  ..I.......I..A..
+00000780: 24d1 2000 00e6 8202 2b24 6500 0137 0202  $. .....+$e..7..
+00000790: 36c0 e700 006e e802 38ab b000 00b6 a302  6....n..8.......
+000007a0: 488e 8300 0130 4102 5442 2f00 0022 3d02  H....0A.TB/.."=.
+000007b0: 6b41 b400 0137 cf02 705b 1000 0061 ec02  kA...7..p[...a..
+000007c0: 75ac 0500 00df 1a02 76e6 2500 0046 da02  u.......v.%..F..
+000007d0: 80f4 7400 005d 6202 83cb 1900 00b3 a502  ..t..]b.........
+000007e0: 84df 6000 000d 0b02 86cb d700 00b5 3202  ..`...........2.
+000007f0: 960b 0000 010a f002 9d24 b400 00c6 3d02  .........$....=.
+00000800: a013 f300 00db 5202 b230 f000 00e9 5002  ......R..0....P.
+00000810: b6bc 9300 005b 1c02 b827 6100 00a9 5302  .....[...'a...S.
+00000820: c4de 6000 00cf a302 d6b9 7000 00e7 5d02  ..`.......p...].
+00000830: d6b9 7000 00f3 d502 d6b9 7000 010a 4702  ..p.......p...G.
+00000840: d6b9 7000 0115 1302 da2f f000 00c1 d902  ..p....../......
+00000850: db87 a000 00fa 6802 ddd8 9000 0018 c702  ......h.........
+00000860: e4ef 0400 0020 9702 e60b 0000 007a 0502  ..... .......z..
+00000870: ecb9 d000 006f e403 0055 4a00 0133 5e03  .....o...UJ..3^.
+00000880: 0ae6 8700 0018 3203 0ae6 8700 001d ba03  ......2.........
+00000890: 0b8a 5a00 007f 5d03 1108 9c00 0139 d603  ..Z...]......9..
+000008a0: 1638 c400 009b 4503 1684 be00 001d 0d03  .8....E.........
+000008b0: 2221 4000 00b6 1a03 232f f000 00fb af03  "!@.....#/......
+000008c0: 232f f000 0110 4e03 3176 ac00 0039 7403  #/....N.1v...9t.
+000008d0: 3500 5a00 008c 9903 3f3c 8400 0118 e403  5.Z.....?<......
+000008e0: 55cb 1a00 0078 6903 57fa 2e00 0077 5703  U....xi.W....wW.
+000008f0: 5dae f000 0110 fd03 5dce f000 00eb 8203  ].......].......
+00000900: 6b8b d900 012f 1c03 7321 8300 0117 c803  k..../..s!......
+00000910: 82a1 0000 00e7 8e03 8a06 2000 0107 9703  .......... .....
+00000920: 8b39 a000 010c 3203 8b60 e400 0042 9503  .9....2..`...B..
+00000930: 8c34 6500 0026 f703 8f4e c000 011b a403  .4e..&...N......
+00000940: 9100 d000 0060 f403 97c9 0000 012a f903  .....`.......*..
+00000950: b023 a000 00c0 8a03 cafd 4000 0088 0e03  .#........@.....
+00000960: d07e 2400 006a c403 d1c2 7400 0044 6f03  .~$..j....t..Do.
+00000970: d1e5 2200 0005 7103 da9c f300 005c d803  .."...q......\..
+00000980: ec0c f700 0040 9a03 f69b 8000 00cd c304  .....@..........
+00000990: 0029 e000 012e 6704 09f4 0a00 00c3 3b04  .)....g.......;.
+000009a0: 11d2 4900 000d 7704 11d2 a900 0059 3504  ..I...w......Y5.
+000009b0: 1263 4400 00bc 8604 1564 8e00 0029 c904  .cD......d...)..
+000009c0: 15b4 7000 0142 6d04 195c b000 0121 8504  ..p..Bm..\...!..
+000009d0: 2e61 f000 0075 8d04 449a c000 0135 4e04  .a...u..D....5N.
+000009e0: 56c0 a000 00be 5e04 62c1 c000 0106 9c04  V.....^.b.......
+000009f0: 65af 6900 0052 0e04 66ac 6500 0140 1e04  e.i..R..f.e..@..
+00000a00: 7d16 7000 0070 c004 846c 5400 002b d404  }.p..p...lT..+..
+00000a10: 846c 5400 0087 3204 846c 5400 008d 6904  .lT...2..lT...i.
+00000a20: 846c 5400 013e 3104 8a9c b300 000a 1404  .lT..>1.........
+00000a30: 8a9c b300 0097 4104 8c2d c700 0067 0a04  ......A..-...g..
+00000a40: 8e23 4000 0000 c004 8e23 4000 001f e304  .#@......#@.....
+00000a50: 8e23 4000 0057 3b04 983c 8100 0049 7004  .#@..W;..<...Ip.
+00000a60: 9849 bc00 0008 3504 9e16 8200 0109 8404  .I....5.........
+00000a70: 9e84 d500 0097 9c04 a577 1f00 0068 f104  .........w...h..
+00000a80: a5e2 3000 009e 0704 ac2c a500 008a 4d04  ..0......,....M.
+00000a90: ac2c a500 00a9 1704 bebd 0000 00ae cd04  .,..............
+00000aa0: c840 f000 00f1 5304 c840 f000 00f4 8e04  .@....S..@......
+00000ab0: c840 f000 0117 3e04 cc5c 9400 0028 7804  .@....>..\...(x.
+00000ac0: cf4d c200 00ff fe04 d5c8 0000 0007 1a04  .M..............
+00000ad0: d7d5 4000 00d3 7204 dd34 9000 0015 bf04  ..@...r..4......
+00000ae0: e963 2e00 0080 db04 ee54 4000 0113 b304  .c.......T@.....
+00000af0: f6d3 c900 00da eb05 04e3 1000 0007 9505  ................
+00000b00: 079c 7300 012b 8705 161e a000 00bc 1105  ..s..+..........
+00000b10: 2caa 5000 00ba 6f05 2cde 2300 00a9 ab05  ,.P...o.,.#.....
+00000b20: 304c 6a00 004c 7505 33ee 2500 0015 5205  0Lj..Lu.3.%...R.
+00000b30: 33ee 2500 0037 f805 3c8d c200 0018 7105  3.%..7..<.....q.
+00000b40: 3c8d c200 001e 8705 3d7b 7000 00f0 ee05  <.......={p.....
+00000b50: 3d7b 7000 00f4 2905 3d7b 7000 010b 6505  ={p...).={p...e.
+00000b60: 3d7b 7000 0116 5b05 49ee 8900 006a 2a05  ={p...[.I....j*.
+00000b70: 5305 de00 0078 b705 5316 ce00 0077 9605  S....x..S....w..
+00000b80: 633f 7000 00ec dc05 6945 5000 00cc 7705  c?p.....iEP...w.
+00000b90: 6bc4 2700 008f 7f05 6bcd a500 00b8 3a05  k.'.....k.....:.
+00000ba0: 6c90 5400 009a c705 6ccc 4300 004e 4f05  l.T.....l.C..NO.
+00000bb0: 6edf f400 0092 3b05 6fe5 c000 00fb 1a05  n.....;.o.......
+00000bc0: 802f 5e00 00b7 6e05 812d 6000 0109 2705  ./^...n..-`...'.
+00000bd0: 88a7 e000 0129 6c05 88a8 c000 0050 a405  .....)l......P..
+00000be0: 8c6a c300 00a3 d705 8c6a c300 0122 c605  .j.......j..."..
+00000bf0: 8cbc 8e00 004e 1905 98ab 6e00 0092 7d05  .....N....n...}.
+00000c00: 9ca9 f100 003b 7805 9dfd c000 00ae 4d05  .....;x.......M.
+00000c10: 9e88 c300 0096 b905 a661 8700 0050 d905  .........a...P..
+00000c20: a661 8700 0051 b205 a661 8700 0053 4405  .a...Q...a...SD.
+00000c30: a7f1 8700 0056 1205 adfb 2800 00a4 e405  .....V....(.....
+00000c40: b039 5c00 000b 7b05 b039 5c00 0123 0305  .9\...{..9\..#..
+00000c50: b093 0000 00ce 5105 b247 c400 00a0 2e05  ......Q..G......
+00000c60: c068 c000 0009 a705 c1f8 2200 0091 e005  .h........".....
+00000c70: ced0 2500 00df 9005 d5fa e400 0084 b505  ..%.............
+00000c80: d5fa e400 0133 ae05 da03 6e00 005e fd05  .....3....n..^..
+00000c90: dbc2 3900 0052 fb05 dce3 0000 00d8 a905  ..9..R..........
+00000ca0: dce3 0000 0108 ae05 dde3 7900 0062 1605  ..........y..b..
+00000cb0: e1ed 8400 00c4 9c05 ecff 1900 00f3 6405  ..............d.
+00000cc0: f264 ba00 004a 1005 f662 ea00 00c2 c605  .d...J...b......
+00000cd0: facb 8300 0095 2306 0826 4000 00dd 6906  ......#..&@...i.
+00000ce0: 08e3 9400 007f f306 0ab9 9000 00e9 dc06  ................
+00000cf0: 129d e000 00e6 1106 148d a400 0021 d706  .............!..
+00000d00: 1867 1e00 009e 5106 215f 7400 0064 4c06  .g....Q.!_t..dL.
+00000d10: 2b00 1300 0039 0106 2b00 1300 003a ec06  +....9..+....:..
+00000d20: 2b00 1300 003c e706 34af 4a00 0009 d706  +....<..4.J.....
+00000d30: 3500 0f00 006d 7b06 3c17 4000 00e3 6906  5....m{.<.@...i.
+00000d40: 3c17 4000 00ef b106 3c17 4000 0101 e706  <.@.....<.@.....
+00000d50: 3c17 4000 011b 5406 3cee 8400 00b2 5906  <.@...T.<.....Y.
+00000d60: 468c a000 00b7 0406 4e38 c500 00a5 8506  F.......N8......
+00000d70: 4f34 c000 0118 4606 53a5 f500 004d e406  O4....F.S....M..
+00000d80: 5479 d900 0115 ea06 580f ce00 002a ed06  Ty......X....*..
+00000d90: 5a60 a900 0100 4f06 6318 9000 00ed f006  Z`....O.c.......
+00000da0: 68ee 6400 001c 8b06 69a9 8400 00a7 d606  h.d.....i.......
+00000db0: 69b7 0200 0132 af06 70e2 d000 0071 1706  i....2..p....q..
+00000dc0: 7cd1 c500 004c ff06 7f33 4700 0033 5306  |....L...3G..3S.
+00000dd0: 8786 ea00 00a6 b706 88a1 2400 013e d006  ..........$..>..
+00000de0: 8f30 5000 0127 ba06 9b5a 7700 0123 9c06  .0P..'...Zw..#..
+00000df0: 9bb8 0c00 003b 3306 9c50 2000 00ca b706  .....;3..P .....
+00000e00: 9fb2 5300 0105 d506 a6d5 8300 0136 6f06  ..S..........6o.
+00000e10: a8dd 9c00 0054 3806 aef9 ce00 005b 9b06  .....T8......[..
+00000e20: afe6 3000 0074 b906 b017 2200 00a6 2606  ..0..t...."...&.
+00000e30: b8bb 6000 00af 4e06 c10c 6000 00d6 a406  ..`...N...`.....
+00000e40: c215 0a00 0007 ee06 c227 5a00 0029 3506  .........'Z..)5.
+00000e50: c227 5a00 003c 9b06 c5bd 6a00 012e e806  .'Z..<....j.....
+00000e60: ce8a a100 004f 2106 cf70 9900 0024 f606  .....O!..p...$..
+00000e70: d08b 2a00 00d0 5506 d81c 2e00 00df fb06  ..*...U.........
+00000e80: dbaf 2000 00f7 8f06 e231 4000 0135 c506  .. ......1@..5..
+00000e90: e6c0 4c00 0054 9d07 0120 6600 0020 e707  ..L..T... f.. ..
+00000ea0: 0140 6600 0019 e407 0923 2000 0063 5907  .@f......# ..cY.
+00000eb0: 0ac3 fa00 00a6 7907 0e35 d000 00e3 0907  ......y..5......
+00000ec0: 126c 4400 0142 ee07 1d24 9000 010d 4707  .lD..B...$....G.
+00000ed0: 1db9 0500 0013 7407 3389 e000 00bd 9a07  ......t.3.......
+00000ee0: 3c71 f700 000f 6607 449d 1f00 00c5 0107  <q....f.D.......
+00000ef0: 47cf 0400 0043 9707 4bcf e000 00f0 0107  G....C..K.......
+00000f00: 5cec 7500 00a5 4107 62f5 3500 0043 1e07  \.u...A.b.5..C..
+00000f10: 65e8 b400 0083 6307 65e8 b400 0132 0d07  e.....c.e....2..
+00000f20: 6c21 5400 000b f607 7e9b 0500 00ef 0207  l!T.....~.......
+00000f30: 9a56 2000 0072 dd07 9a6c 1400 000c a507  .V ..r...l......
+00000f40: 9a6c 1400 001c 5207 9a6c 1400 0030 df07  .l....R..l...0..
+00000f50: 9a6c 1400 0054 0007 9a6c 1400 0086 ff07  .l...T...l......
+00000f60: 9a6c 1400 0139 7e07 9aa9 6000 00d4 0a07  .l...9~...`.....
+00000f70: 9db4 9000 00c0 2307 9db4 9000 0105 6107  ......#.......a.
+00000f80: 9e2e 7300 0140 bb07 9fdd d400 0039 fd07  ..s..@.......9..
+00000f90: a121 8000 0022 ea07 a674 8700 00a8 2907  .!..."...t....).
+00000fa0: bdfe de00 002e 4007 c07a 2000 00d1 4a07  ......@..z ...J.
+00000fb0: cf9a 7000 0103 8107 d231 3400 0003 9f07  ..p......14.....
+00000fc0: daae 0000 010c da07 dae0 ea00 0126 ab07  .............&..
+00000fd0: e0a9 5000 000e a107 e0a9 5000 008e c007  ..P.......P.....
+00000fe0: e0a9 5000 0124 b307 ebd7 9e00 00b1 7c07  ..P..$........|.
+00000ff0: ebd7 9e00 00b4 6707 ec42 a500 000a c507  ......g..B......
+00001000: ed5c 8000 011a 7307 f3d4 e000 00d2 6407  .\....s.......d.
+00001010: f714 e400 0100 d008 0291 0000 0085 dc08  ................
+00001020: 08a7 9000 00cb f208 1f02 9000 00bd 3a08  ..............:.
+00001030: 283b 1400 0106 2c08 284d 4300 0089 2308  (;....,.(MC...#.
+00001040: 28e8 e000 00f8 4608 2a45 4a00 00a8 7408  (.....F.*EJ...t.
+00001050: 2fe7 9000 00a2 8508 3267 1100 0008 a008  /.......2g......
+00001060: 41da 6e00 008a db08 426e 6000 011e 5908  A.n.....Bn`...Y.
+00001070: 4289 4c00 003a a108 46c5 3a00 0048 d108  B.L..:..F.:..H..
+00001080: 4d37 c500 0097 d808 4e6b 2a00 004a 5808  M7......Nk*..JX.
+00001090: 4ef9 1500 005e 6708 4fd0 2000 011d d608  N....^g.O. .....
+000010a0: 6186 7000 0073 d708 6c71 e200 00b4 0808  a.p..s..lq......
+000010b0: 6f32 c000 00e1 8b08 700d f000 0102 fa08  o2......p.......
+000010c0: 70b2 8b00 0079 4408 7219 0f00 008e f708  p....yD.r.......
+000010d0: 7a4a 5000 007e 8908 8284 d500 000c d608  zJP..~..........
+000010e0: 8284 d500 0087 6608 8599 7200 013f e508  ......f...r..?..
+000010f0: 8958 2900 0134 f508 8b87 0000 00d9 2308  .X)..4........#.
+00001100: 8fa4 9300 0010 9908 8fa4 9300 008b 2908  ..............).
+00001110: 8fa4 9300 0091 2508 8fa4 9300 0123 6408  ......%......#d.
+00001120: 9a98 b400 001a c808 9c61 5e00 0127 0608  .........a^..'..
+00001130: a1a4 9300 005a dc08 a63b 3000 0116 c108  .....Z...;0.....
+00001140: aa82 f400 005c 6d08 abe2 0900 002c 0508  .....\m......,..
+00001150: abe2 0900 008d 9e08 af11 d500 0065 2408  .............e$.
+00001160: b89a 9200 0026 bc08 bbfe c500 0002 ac08  .....&..........
+00001170: bbfe c500 012f f208 bd8a 6000 0120 fb08  ...../....`.. ..
+00001180: c000 5000 009c ae08 c000 5000 009d 7108  ..P.......P...q.
+00001190: c272 0900 0010 d608 c76b 0300 005b e208  .r.......k...[..
+000011a0: cd7c e400 00b1 0c09 00f9 a400 0003 e009  .|..............
+000011b0: 162e f000 003e a309 1afc d400 0041 5409  .....>.......AT.
+000011c0: 1fb9 f500 0078 e909 2254 0000 012a 9a09  .....x.."T...*..
+000011d0: 2e57 df00 00aa f909 35e6 6000 004c 3209  .W......5.`..L2.
+000011e0: 3b85 e000 006e 5a09 4459 d000 00e8 bf09  ;....nZ.DY......
+000011f0: 4d67 fe00 0122 8609 5962 c900 00ef 4109  Mg..."..Yb....A.
+00001200: 5aa4 1000 00c1 2709 5b68 f000 0060 7a09  Z.....'.[h...`z.
+00001210: 5c07 3000 00f6 e009 5ca2 3000 013b 6609  \.0.....\.0..;f.
+00001220: 5d03 9000 0128 f709 6302 2500 0140 8b09  ]....(..c.%..@..
+00001230: 667a 9000 00f5 1709 66cc c900 0035 5709  fz......f....5W.
+00001240: 700b c500 0012 cf09 7a29 6900 0010 1909  p.......z)i.....
+00001250: 8c00 0a00 0051 6c09 8c81 5e00 0029 8409  .....Ql...^..)..
+00001260: 8c81 5e00 003d 2809 8c81 5e00 0052 ad09  ..^..=(...^..R..
+00001270: 8c81 5e00 009d 2709 8d04 b300 0094 5a09  ..^...'.......Z.
+00001280: 95cb c400 00de ad09 a6af c300 0058 be09  .............X..
+00001290: a6c1 0a00 0028 c609 a6c1 0a00 0048 6809  .....(.......Hh.
+000012a0: a6c1 0a00 0088 4f09 a6c1 0a00 009c 7109  ......O.......q.
+000012b0: a6c1 0a00 012d 5609 a6c1 c300 0004 6f09  .....-V.......o.
+000012c0: a87a 8000 0102 3e09 b56b a200 0091 5e09  .z....>..k....^.
+000012d0: b889 ea00 008c 0209 b889 ea00 00aa 5f09  .............._.
+000012e0: cf34 f000 00e8 2a09 d82d 3f00 0088 8609  .4....*..-?.....
+000012f0: dbfe c000 00e2 4a0a 074b 5000 0075 200a  ......J..KP..u .
+00001300: 159b 8000 001f 500a 159b 8000 0056 a90a  ......P......V..
+00001310: 17d3 5000 00d4 c80a 20b0 6000 007d 830a  ..P..... .`..}..
+00001320: 20fc 9000 00bb 530a 22d2 d000 00ed 5b0a   .....S.".....[.
+00001330: 2aef e000 0104 0c0a 2e99 7e00 0058 f60a  *.........~..X..
+00001340: 30f6 b500 002b 7c0a 338b 1000 00e5 900a  0....+|.3.......
+00001350: 3f0e 9500 0085 640a 3f0e 9500 0134 b40a  ?.....d.?....4..
+00001360: 4985 3000 0074 450a 4cb2 e000 00be de0a  I.0..tE.L.......
+00001370: 5e50 b000 0113 3c0a 62cd 3400 0036 100a  ^P....<.b.4..6..
+00001380: 64c8 9500 008b c60a 65e3 f000 005f bf0a  d.......e...._..
+00001390: 6c11 b300 0005 040a 6c5b d900 000a 580a  l.......l[....X.
+000013a0: 6c5b d900 000c 3e0a 6c5b d900 0039 c10a  l[....>.l[...9..
+000013b0: 6c89 9300 0140 4e0a 6cba 2900 0115 680a  l....@N.l.)...h.
+000013c0: 70ea 0000 0047 cd0a 8170 8e00 013c 3d0a  p....G...p...<=.
+000013d0: 84e6 b500 001d 730a 84e6 b500 0031 770a  ......s......1w.
+000013e0: 84e6 b500 0055 090a 84e6 b500 013a 220a  .....U.......:".
+000013f0: 84e6 b500 013e 900a 89ad 3000 00fe 150a  .....>....0.....
+00001400: 89ad 3000 0114 750a 8c5e f000 0068 420a  ..0...u..^...hB.
+00001410: 954c 2000 00e3 ba0a 9989 6300 0076 880a  .L .......c..v..
+00001420: ac8c c000 0101 6e0a ae3e fa00 0078 2f0a  ......n..>...x/.
+00001430: b4bc 2e00 0030 440a b5ff 6400 00b8 d20a  .....0D...d.....
+00001440: b6d5 d000 00da 4b0a ba90 7000 00f0 6f0a  ......K...p...o.
+00001450: be20 4a00 0011 1c0a c25d 1400 0045 300a  . J......]...E0.
+00001460: c945 a000 00ba c60a ca80 7300 0055 4f0a  .E........s..UO.
+00001470: cf76 b400 005a 300a cfef 4000 010f ba0a  .v...Z0...@.....
+00001480: e1b0 da00 00af af0a e1b4 8000 011d 5d0a  ..............].
+00001490: e45f d000 00bf 9c0a eb63 2000 0023 870a  ._.......c ..#..
+000014a0: ee50 6000 0086 940a f3de 9e00 0089 f40a  .P`.............
+000014b0: f456 b400 0120 760a f818 8000 00bf 170a  .V... v.........
+000014c0: f818 8000 0104 cf0b 0396 6300 0009 720b  ..........c...r.
+000014d0: 03f9 7300 0094 100b 0476 b400 005a 6a0b  ..s......v...Zj.
+000014e0: 0ac1 5a00 0134 4a0b 139f b500 008c 3a0b  ..Z..4J.......:.
+000014f0: 19b8 d700 008f fe0b 1b90 b000 010a 770b  ..............w.
+00001500: 1fcd 0500 00a5 e20b 20ce b000 00ca 250b  ........ .....%.
+00001510: 2371 ce00 0001 3e0b 244d 8300 010e 960b  #q....>.$M......
+00001520: 296c c900 0076 190b 2d80 be00 000f c70b  )l...v..-.......
+00001530: 2d80 be00 0090 5b0b 2d80 be00 0125 3a0b  -.....[.-....%:.
+00001540: 2fa8 e400 013b 220b 4000 a500 0066 870b  /....;".@....f..
+00001550: 440d ae00 005c 1b0b 47ce c400 00f2 4f0b  D....\..G.....O.
+00001560: 4841 e400 00c4 360b 4e26 9900 0011 620b  HA....6.N&....b.
+00001570: 543a f400 00ea 7f0b 5467 9000 002c a30b  T:......Tg...,..
+00001580: 6948 d000 00cd 110b 6b4e 3000 0061 5d0b  iH......kN0..a].
+00001590: 6f1b 4500 0063 c20b 76dd 9d00 013f 1b0b  o.E..c..v....?..
+000015a0: 800e 0c00 005d 1e0b 8a1a 2000 00ec 160b  .....].... .....
+000015b0: 8a1a 2000 011a 200b 8c6a e300 005b 5d0b  .. ... ..j...[].
+000015c0: 9253 4000 0002 280b 94b6 5e00 00d7 f10b  .S@...(...^.....
+000015d0: 967b 5400 0033 020b a0c9 de00 0006 5c0b  .{T..3........\.
+000015e0: a3fc 0c00 0072 9f0b a3fc 7000 00f9 ee0b  .....r....p.....
+000015f0: a4a2 2500 0025 690b c474 9000 00e4 560b  ..%..%i..t....V.
+00001600: c4a6 f000 0066 120b c81a a000 00e4 f50b  .....f..........
+00001610: cbf1 c000 00ec 690b cbf1 c000 00f1 dc0b  ......i.........
+00001620: cbf1 c000 00fc 640b cbf1 c000 0112 3f0b  ......d.......?.
+00001630: db2b b200 0026 6d0b def4 0000 0138 6b0b  .+...&m......8k.
+00001640: e203 8700 000f 1f0b e217 6300 000e dc0b  ..........c.....
+00001650: e4a0 3000 0016 c50b f39a 4000 003d ab0b  ..0.......@..=..
+00001660: f39a 4000 0086 250b f39a 4000 00d0 d80b  ..@...%...@.....
+00001670: fc32 3300 0049 060c 04fe c500 0014 360c  .23..I........6.
+00001680: 0c17 6300 0059 840c 0ce3 2300 0093 ba0c  ..c..Y....#.....
+00001690: 0dec 5a00 0085 020c 1d95 4000 00c8 520c  ..Z.......@...R.
+000016a0: 2ab3 5e00 007b ec0c 3834 1400 000e 3b0c  *.^..{..84....;.
+000016b0: 3834 1400 008e 5e0c 3834 1400 0124 510c  84....^.84...$Q.
+000016c0: 5256 ae00 0035 190c 5bd6 a000 0008 670c  RV...5..[.....g.
+000016d0: 61ce a500 0035 ca0c 63ce a500 000b b00c  a....5..c.......
+000016e0: 6dca b800 003a 520c 808a a300 00aa 050c  m....:R.........
+000016f0: 83b7 b000 0038 c80c 8910 0000 0006 9a0c  .....8..........
+00001700: 89ed e500 004d ac0c 98c0 0900 0005 e20c  .....M..........
+00001710: 98c0 0900 000a 8e0c 98c0 0900 000d c70c  ................
+00001720: 98c0 0900 0087 9d0c 98c0 0900 008d 280c  ..............(.
+00001730: 98c0 0900 00a4 410c 98c0 0900 0122 4d0c  ......A......"M.
+00001740: 9fa9 6000 0129 dd0c b106 9a00 0126 5c0c  ..`..).......&\.
+00001750: b195 2700 0084 0b0c b1a8 e500 0031 f20c  ..'..........1..
+00001760: ba9f 2400 0119 a10c c1c5 c300 0095 a90c  ..$.............
+00001770: c4e1 d500 0014 7f0c c5f7 d500 0082 000c  ................
+00001780: c7ee 6000 00a1 2e0c c8e8 6400 0031 3d0c  ..`.......d..1=.
+00001790: c9a0 2e00 0082 5f0c cba2 d500 00f3 240c  ......_.......$.
+000017a0: db0c 0400 00bb c30c dda2 6e00 00b9 400c  ..........n...@.
+000017b0: e3ed a900 0095 5e0c f3b0 8500 0013 190c  ......^.........
+000017c0: fb0f b300 0098 4a0d 0027 2000 00c7 250d  ......J..' ...%.
+000017d0: 09a5 6000 0128 120d 0a66 ed00 0131 810d  ..`..(...f...1..
+000017e0: 0ad7 7300 004f f40d 0f91 6000 00f8 d00d  ..s..O....`.....
+000017f0: 0f91 6000 010d fb0d 1201 a400 005d f00d  ..`..........]..
+00001800: 1cec 6700 0125 880d 2d41 7000 00b5 830d  ..g..%..-Ap.....
+00001810: 32db 3000 00f5 720d 35c6 3000 0111 920d  2.0...r.5.0.....
+00001820: 3b8c 3900 00b3 030d 48cd 6500 009f 1f0d  ;.9.....H.e.....
+00001830: 51bd f000 00fc de0d 69f6 0000 00a1 db0d  Q.......i.......
+00001840: 7298 e700 00b4 bf0d 7c3b 4000 011a e60d  r.......|;@.....
+00001850: 80f6 3400 009c 260d 80f6 3400 009d b60d  ..4...&...4.....
+00001860: 8344 9300 0094 a00d 8c46 7500 0004 a70d  .D.......Fu.....
+00001870: 8c46 7500 00aa 9a0d 96e3 5000 00e7 090d  .Fu.......P.....
+00001880: 9df1 6500 001a 7d0d 9df1 6500 0021 520d  ..e...}...e..!R.
+00001890: 9ee3 5e00 006e a70d 9ee3 5e00 007b a70d  ..^..n....^..{..
+000018a0: 9ee3 5e00 0089 6c0d 9ee3 5e00 00a8 c90d  ..^...l...^.....
+000018b0: 9ee3 5e00 00be 1a0d aa4e 9000 00ee 7e0d  ..^......N....~.
+000018c0: c964 7400 00b1 d20d d0e8 e000 00d0 170d  .dt.............
+000018d0: ded8 9000 001d ff0d ded8 9000 0055 8b0d  .............U..
+000018e0: eb49 0000 0084 430d ec49 8400 004b 720d  .I....C..I...Kr.
+000018f0: f086 4a00 003c 460d fcd5 7e00 0042 0d0d  ..J..<F...~..B..
+00001900: fe0b 6000 0071 7b0e 00f0 b000 00dc 4e0e  ..`..q{.......N.
+00001910: 03af f000 0079 880e 1bf8 6400 003b b30e  .....y....d..;..
+00001920: 1ddb 6300 0053 a00e 202b 3a00 0082 be0e  ..c..S.. +:.....
+00001930: 202b 3a00 0130 e80e 2511 7400 0062 600e   +:..0..%.t..b`.
+00001940: 38a0 f000 010f 1b0e 46c3 2e00 011f 500e  8.......F.....P.
+00001950: 5c13 4700 0123 d00e 6193 e900 011c 140e  \.G..#..a.......
+00001960: 61d5 0400 00af fe0e 68cb dc00 0058 580e  a.......h....XX.
+00001970: 6ac2 e300 0025 ca0e 6e10 8f00 007a bc0e  j....%..n....z..
+00001980: 7617 2000 0080 440e 8347 4400 006c 080e  v. ...D..GD..l..
+00001990: 887b b500 0038 5d0e 887b b500 00b0 d50e  .{...8]..{......
+000019a0: 9dcc d400 0033 fc0e a934 c000 0062 df0e  .....3...4...b..
+000019b0: abf5 1300 0069 b60e ae34 8000 0060 1a0e  .....i...4...`..
+000019c0: b4a5 0a00 0065 ad0e b5c2 8000 009f 810e  .....e..........
+000019d0: b803 9900 0070 6b0e b82d 1000 00fd 720e  .....pk..-....r.
+000019e0: c28b b000 0003 0c0e d945 de00 002e fc0e  .........E......
+000019f0: e77d 7000 012c 510e f7f8 4000 00f9 710f  .}p..,Q...@...q.
+00001a00: 09fd b000 00de 120f 0cc4 c000 0104 7c0f  ..............|.
+00001a10: 105e a000 00c2 5b0f 11be 6000 00c7 9a0f  .^....[...`.....
+00001a20: 1d28 1000 0108 3e0f 201d 8500 008d dd0f  .(....>. .......
+00001a30: 20f1 3000 00e0 520f 4321 f500 013c d40f   .0...R.C!...<..
+00001a40: 4a90 4000 00bb 0a0f 5e00 1000 00d2 ed0f  J.@.....^.......
+00001a50: 76f2 2000 007d 040f 8e7b e000 00d7 4f0f  v. ..}...{....O.
+00001a60: 9222 7c00 00b2 c30f 9450 0000 011e c50f  ."|......P......
+00001a70: 969b 9a00 0052 560f 9ebd c400 004b ca0f  .....RV......K..
+00001a80: 9fbc 6000 0141 5e0f a262 9000 0143 d50f  ..`..A^..b...C..
+00001a90: a44f 0300 0000 5f0f bd5e e700 0124 ea0f  .O...._..^...$..
+00001aa0: cb15 5200 006b bc0f cf80 f000 00fe b90f  ..R..k..........
+00001ab0: d19a 7000 00c9 0b0f dfeb 7000 00a3 6c0f  ..p.......p...l.
+00001ac0: e7f7 9000 0143 630f ea8a 0900 0083 030f  .....Cc.........
+00001ad0: ea8a 0900 00ad f50f ea8a 0900 0131 270f  .............1'.
+00001ae0: f87c e000 0024 6d0f fe37 0300 008b 6869  .|...$m..7....hi
+00001af0: 0001 4450 0300 0000 2404 1e04 4204 3c04  ..DP....$...B.<.
+00001b00: 3504 3d04 3804 4204 4c00 2004 3804 3704  5.=.8.B.L. .8.7.
+00001b10: 3c04 3504 3d04 3504 3d04 3804 4f08 0000  <.5.=.5.=.8.O...
+00001b20: 0000 0600 0000 0e43 616e 6365 6c20 6368  .......Cancel ch
+00001b30: 616e 6765 7307 0000 0018 4162 7374 7261  anges.....Abstra
+00001b40: 6374 4f70 6572 6174 696f 6e44 6574 6169  ctOperationDetai
+00001b50: 6c73 0103 0000 0026 0421 043e 0445 0440  ls.....&.!.>.E.@
+00001b60: 0430 043d 0438 0442 044c 0020 0438 0437  .0.=.8.B.L. .8.7
+00001b70: 043c 0435 043d 0435 043d 0438 044f 0800  .<.5.=.5.=.8.O..
+00001b80: 0000 0006 0000 000e 436f 6d6d 6974 2063  ........Commit c
+00001b90: 6861 6e67 6573 0700 0000 1841 6273 7472  hanges.....Abstr
+00001ba0: 6163 744f 7065 7261 7469 6f6e 4465 7461  actOperationDeta
+00001bb0: 696c 7301 0300 0000 3804 1e04 4804 3804  ils.....8...H.8.
+00001bc0: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
+00001bd0: 3704 3004 3f04 3804 4104 3800 2004 3e04  7.0.?.8.A.8. .>.
+00001be0: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
+00001bf0: 2008 0000 0000 0600 0000 194f 7065 7261   ..........Opera
+00001c00: 7469 6f6e 2073 7562 6d69 7420 6661 696c  tion submit fail
+00001c10: 6564 3a20 0700 0000 1841 6273 7472 6163  ed: .....Abstrac
+00001c20: 744f 7065 7261 7469 6f6e 4465 7461 696c  tOperationDetail
+00001c30: 7301 0300 0000 8804 1d04 3504 4104 3e04  s.........5.A.>.
+00001c40: 4504 4004 3004 3d04 5104 3d04 3d04 4b04  E.@.0.=.Q.=.=.K.
+00001c50: 3500 2004 3804 3704 3c04 3504 3d04 3504  5. .8.7.<.5.=.5.
+00001c60: 3d04 3804 4f00 2004 3104 4b04 3b04 3800  =.8.O. .1.K.;.8.
+00001c70: 2004 3e04 4204 3c04 3504 3d04 3504 3d04   .>.B.<.5.=.5.=.
+00001c80: 4b00 2004 3f04 3504 4004 3504 3400 2004  K. .?.5.@.5.4. .
+00001c90: 4104 3e04 3704 3404 3004 3d04 3804 3504  A.>.7.4.0.=.8.5.
+00001ca0: 3c00 2004 3d04 3e04 3204 3e04 3900 2004  <. .=.>.2.>.9. .
+00001cb0: 3e04 3f04 3504 4004 3004 4604 3804 3808  >.?.5.@.0.F.8.8.
+00001cc0: 0000 0000 0600 0000 3555 6e73 6176 6564  ........5Unsaved
+00001cd0: 2063 6861 6e67 6573 2077 6572 6520 7265   changes were re
+00001ce0: 7665 7274 6564 2074 6f20 6372 6561 7465  verted to create
+00001cf0: 206e 6577 206f 7065 7261 7469 6f6e 0700   new operation..
+00001d00: 0000 1841 6273 7472 6163 744f 7065 7261  ...AbstractOpera
+00001d10: 7469 6f6e 4465 7461 696c 7301 0300 0000  tionDetails.....
+00001d20: 3a04 1d04 3504 3204 3504 4004 3d04 3e04  :...5.2.5.@.=.>.
+00001d30: 3500 2004 3704 3d04 3004 4704 3504 3d04  5. .7.=.0.G.5.=.
+00001d40: 3804 3500 2004 3200 2004 4104 4204 3e04  8.5. .2. .A.B.>.
+00001d50: 3b04 3104 4604 3500 3a00 2008 0000 0000  ;.1.F.5.:. .....
+00001d60: 0600 0000 1b43 6f6c 756d 6e20 6861 7320  .....Column has 
+00001d70: 6e6f 2076 616c 6964 2076 616c 7565 3a20  no valid value: 
+00001d80: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
+00001d90: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
+00001da0: 0300 0000 1e04 1d04 3504 3f04 3e04 3b04  ........5.?.>.;.
+00001db0: 3d04 4b04 3500 2004 3404 3004 3d04 3d04  =.K.5. .4.0.=.=.
+00001dc0: 4b04 3508 0000 0000 0600 0000 1344 6174  K.5..........Dat
+00001dd0: 6120 6172 6520 696e 636f 6d70 6c65 7465  a are incomplete
+00001de0: 0700 0000 1a41 6273 7472 6163 7452 6566  .....AbstractRef
+00001df0: 6572 656e 6365 4c69 7374 4d6f 6465 6c01  erenceListModel.
+00001e00: 0300 0000 2604 1e04 4804 3804 3104 3a04  ....&...H.8.1.:.
+00001e10: 3000 2004 4104 3e04 4504 4004 3004 3d04  0. .A.>.E.@.0.=.
+00001e20: 3504 3d04 3804 4f00 3a00 2008 0000 0000  5.=.8.O.:. .....
+00001e30: 0600 0000 0f53 7562 6d69 7420 6661 696c  .....Submit fail
+00001e40: 6564 3a20 0700 0000 1a41 6273 7472 6163  ed: .....Abstrac
+00001e50: 7452 6566 6572 656e 6365 4c69 7374 4d6f  tReferenceListMo
+00001e60: 6465 6c01 0300 0000 0a04 1b04 4e04 3104  del.........N.1.
+00001e70: 3e04 3908 0000 0000 0600 0000 0341 4e59  >.9..........ANY
+00001e80: 0700 0000 0d41 6363 6f75 6e74 4275 7474  .....AccountButt
+00001e90: 6f6e 0103 0000 0014 041b 044e 0431 043e  on.........N.1.>
+00001ea0: 0439 0020 0441 0447 0435 0442 0800 0000  .9. .A.G.5.B....
+00001eb0: 0006 0000 000b 416e 7920 6163 636f 756e  ......Any accoun
+00001ec0: 7407 0000 000d 4163 636f 756e 7442 7574  t.....AccountBut
+00001ed0: 746f 6e01 0300 0000 1804 1204 4b04 3104  ton.........K.1.
+00001ee0: 4004 3004 4204 4c00 2004 4104 4704 3504  @.0.B.L. .A.G.5.
+00001ef0: 4208 0000 0000 0600 0000 0e43 686f 6f73  B..........Choos
+00001f00: 6520 6163 636f 756e 7407 0000 000d 4163  e account.....Ac
+00001f10: 636f 756e 7442 7574 746f 6e01 0300 0000  countButton.....
+00001f20: 1404 2204 3804 3f00 2004 4104 4704 3504  ..".8.?. .A.G.5.
+00001f30: 4204 3000 3a08 0000 0000 0600 0000 0d41  B.0.:..........A
+00001f40: 6363 6f75 6e74 2074 7970 653a 0700 0000  ccount type:....
+00001f50: 1141 6363 6f75 6e74 4c69 7374 4469 616c  .AccountListDial
+00001f60: 6f67 0103 0000 000a 0421 0447 0435 0442  og.......!.G.5.B
+00001f70: 0430 0800 0000 0006 0000 0008 4163 636f  .0..........Acco
+00001f80: 756e 7473 0700 0000 1141 6363 6f75 6e74  unts.....Account
+00001f90: 4c69 7374 4469 616c 6f67 0103 0000 002a  ListDialog.....*
+00001fa0: 041f 043e 043a 0430 0437 044b 0432 0430  ...>.:.0.7.K.2.0
+00001fb0: 0442 044c 0020 043d 0435 0430 043a 0442  .B.L. .=.5.0.:.B
+00001fc0: 0438 0432 043d 044b 0435 0800 0000 0006  .8.2.=.K.5......
+00001fd0: 0000 000d 5368 6f77 2069 6e61 6374 6976  ....Show inactiv
+00001fe0: 6507 0000 0011 4163 636f 756e 744c 6973  e.....AccountLis
+00001ff0: 7444 6961 6c6f 6701 0300 0000 0e21 1600  tDialog......!..
+00002000: 2004 4104 4704 3504 4204 3008 0000 0000   .A.G.5.B.0.....
+00002010: 0600 0000 0941 6363 6f75 6e74 2023 0700  .....Account #..
+00002020: 0000 1041 6363 6f75 6e74 4c69 7374 4d6f  ...AccountListMo
+00002030: 6465 6c01 0300 0000 0804 1004 3a04 4200  del.........:.B.
+00002040: 2e08 0000 0000 0600 0000 0441 6374 2e07  ...........Act..
+00002050: 0000 0010 4163 636f 756e 744c 6973 744d  ....AccountListM
+00002060: 6f64 656c 0103 0000 0016 0411 0430 043d  odel.........0.=
+00002070: 043a 002f 0411 0440 043e 043a 0435 0440  .:./...@.>.:.5.@
+00002080: 0800 0000 0006 0000 000b 4261 6e6b 2f42  ..........Bank/B
+00002090: 726f 6b65 7207 0000 0010 4163 636f 756e  roker.....Accoun
+000020a0: 744c 6973 744d 6f64 656c 0103 0000 0004  tListModel......
+000020b0: 041a 0421 0800 0000 0006 0000 0002 4343  ...!..........CC
+000020c0: 0700 0000 1041 6363 6f75 6e74 4c69 7374  .....AccountList
+000020d0: 4d6f 6465 6c01 0300 0000 0c04 1204 3004  Model.........0.
+000020e0: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
+000020f0: 0843 7572 7265 6e63 7907 0000 0010 4163  .Currency.....Ac
+00002100: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
+00002110: 0000 0018 041d 0430 0438 043c 0435 043d  .......0.8.<.5.=
+00002120: 043e 0432 0430 043d 0438 0435 0800 0000  .>.2.0.=.8.5....
+00002130: 0006 0000 0004 4e61 6d65 0700 0000 1041  ......Name.....A
+00002140: 6363 6f75 6e74 4c69 7374 4d6f 6465 6c01  ccountListModel.
+00002150: 0300 0000 1004 2204 3e04 4704 3d04 3e04  ......".>.G.=.>.
+00002160: 4104 4204 4c08 0000 0000 0600 0000 0950  A.B.L..........P
+00002170: 7265 6369 7369 6f6e 0700 0000 1041 6363  recision.....Acc
+00002180: 6f75 6e74 4c69 7374 4d6f 6465 6c01 0300  ountListModel...
+00002190: 0000 1004 2104 3204 3504 4004 3504 3d00  ....!.2.5.@.5.=.
+000021a0: 2000 4008 0000 0000 0600 0000 0c52 6563   .@..........Rec
+000021b0: 6f6e 6369 6c65 6420 4007 0000 0010 4163  onciled @.....Ac
+000021c0: 636f 756e 744c 6973 744d 6f64 656c 0103  countListModel..
+000021d0: 0000 001a 0426 0435 043d 043d 0430 044f  .....&.5.=.=.0.O
+000021e0: 0020 0431 0443 043c 0430 0433 0430 0800  . .1.C.<.0.3.0..
+000021f0: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
+00002200: 000b 4173 7365 7444 6961 6c6f 6701 0300  ..AssetDialog...
+00002210: 0000 3e04 1e04 4804 3804 3104 3a04 3000  ..>...H.8.1.:.0.
+00002220: 2004 3704 3004 3f04 3804 4104 3800 2004   .7.0.?.8.A.8. .
+00002230: 3804 3d04 4404 3e04 4004 3c04 3004 4604  8.=.D.>.@.<.0.F.
+00002240: 3804 3800 2004 3e00 2004 2604 1100 3a00  8.8. .>. .&...:.
+00002250: 2008 0000 0000 0600 0000 1d41 7373 6574   ..........Asset
+00002260: 2064 6574 6169 6c73 2073 7562 6d69 7420   details submit 
+00002270: 6661 696c 6564 3a20 0700 0000 0b41 7373  failed: .....Ass
+00002280: 6574 4469 616c 6f67 0103 0000 0024 041e  etDialog.....$..
+00002290: 0448 0438 0431 043a 0430 0020 0437 0430  .H.8.1.:.0. .7.0
+000022a0: 043f 0438 0441 0438 0020 0426 0415 003a  .?.8.A.8. .&...:
+000022b0: 0020 0800 0000 0006 0000 0015 4173 7365  . ..........Asse
+000022c0: 7420 7375 626d 6974 2066 6169 6c65 643a  t submit failed:
+000022d0: 2007 0000 000b 4173 7365 7444 6961 6c6f   .....AssetDialo
+000022e0: 6701 0300 0000 1c04 1104 3004 3704 3e04  g.........0.7.>.
+000022f0: 3204 4b04 3900 2004 3004 3a04 4204 3804  2.K.9. .0.:.B.8.
+00002300: 3200 3a08 0000 0000 0600 0000 0b42 6173  2.:..........Bas
+00002310: 6520 6173 7365 743a 0700 0000 0b41 7373  e asset:.....Ass
+00002320: 6574 4469 616c 6f67 0103 0000 000c 041e  etDialog........
+00002330: 0442 043c 0435 043d 0430 0800 0000 0006  .B.<.5.=.0......
+00002340: 0000 0006 4361 6e63 656c 0700 0000 0b41  ....Cancel.....A
+00002350: 7373 6574 4469 616c 6f67 0103 0000 0010  ssetDialog......
+00002360: 0421 0442 0440 0430 043d 0430 003a 0020  .!.B.@.0.=.0.:. 
+00002370: 0800 0000 0006 0000 0009 436f 756e 7472  ..........Countr
+00002380: 793a 2007 0000 000b 4173 7365 7444 6961  y: .....AssetDia
+00002390: 6c6f 6701 0300 0000 1404 1404 3e04 3f00  log.........>.?.
+000023a0: 2e04 3404 3004 3d04 3d04 4b04 3508 0000  ..4.0.=.=.K.5...
+000023b0: 0000 0600 0000 0a45 7874 7261 2064 6174  .......Extra dat
+000023c0: 6107 0000 000b 4173 7365 7444 6961 6c6f  a.....AssetDialo
+000023d0: 6701 0300 0000 0a00 4900 5300 4900 4e00  g.......I.S.I.N.
+000023e0: 3a08 0000 0000 0600 0000 0549 5349 4e3a  :..........ISIN:
+000023f0: 0700 0000 0b41 7373 6574 4469 616c 6f67  .....AssetDialog
+00002400: 0103 0000 001a 041d 0430 0438 043c 0435  .........0.8.<.5
+00002410: 043d 043e 0432 0430 043d 0438 0435 003a  .=.>.2.0.=.8.5.:
+00002420: 0800 0000 0006 0000 0005 4e61 6d65 3a07  ..........Name:.
+00002430: 0000 000b 4173 7365 7444 6961 6c6f 6701  ....AssetDialog.
+00002440: 0300 0000 0404 1e04 1a08 0000 0000 0600  ................
+00002450: 0000 024f 4b07 0000 000b 4173 7365 7444  ...OK.....AssetD
+00002460: 6961 6c6f 6701 0300 0000 0e04 2104 3804  ialog.......!.8.
+00002470: 3c04 3204 3e04 3b04 4b08 0000 0000 0600  <.2.>.;.K.......
+00002480: 0000 0753 796d 626f 6c73 0700 0000 0b41  ...Symbols.....A
+00002490: 7373 6574 4469 616c 6f67 0103 0000 000a  ssetDialog......
+000024a0: 0422 0438 043f 003a 0020 0800 0000 0006  .".8.?.:. ......
+000024b0: 0000 0006 5479 7065 3a20 0700 0000 0b41  ....Type: .....A
+000024c0: 7373 6574 4469 616c 6f67 0103 0000 000e  ssetDialog......
+000024d0: 0422 0438 043f 0020 0426 0411 003a 0800  .".8.?. .&...:..
+000024e0: 0000 0006 0000 000b 4173 7365 7420 7479  ........Asset ty
+000024f0: 7065 3a07 0000 000f 4173 7365 744c 6973  pe:.....AssetLis
+00002500: 7444 6961 6c6f 6701 0300 0000 1a04 2604  tDialog.......&.
+00002510: 3504 3d04 3d04 4b04 3500 2004 3104 4304  5.=.=.K.5. .1.C.
+00002520: 3c04 3004 3304 3808 0000 0000 0600 0000  <.0.3.8.........
+00002530: 0641 7373 6574 7307 0000 000f 4173 7365  .Assets.....Asse
+00002540: 744c 6973 7444 6961 6c6f 6701 0300 0000  tListDialog.....
+00002550: 0c04 2104 4204 4004 3004 3d04 3008 0000  ..!.B.@.0.=.0...
+00002560: 0000 0600 0000 0743 6f75 6e74 7279 0700  .......Country..
+00002570: 0000 0e41 7373 6574 4c69 7374 4d6f 6465  ...AssetListMode
+00002580: 6c01 0300 0000 0c04 1204 3004 3b04 4e04  l.........0.;.N.
+00002590: 4204 3008 0000 0000 0600 0000 0843 7572  B.0..........Cur
+000025a0: 7265 6e63 7907 0000 000e 4173 7365 744c  rency.....AssetL
+000025b0: 6973 744d 6f64 656c 0103 0000 001a 0418  istModel........
+000025c0: 0441 0442 002e 043a 043e 0442 0438 0440  .A.B...:.>.B.8.@
+000025d0: 043e 0432 043e 043a 0800 0000 0006 0000  .>.2.>.:........
+000025e0: 000b 4461 7461 2073 6f75 7263 6507 0000  ..Data source...
+000025f0: 000e 4173 7365 744c 6973 744d 6f64 656c  ..AssetListModel
+00002600: 0103 0000 0008 0049 0053 0049 004e 0800  .......I.S.I.N..
+00002610: 0000 0006 0000 0004 4953 494e 0700 0000  ........ISIN....
+00002620: 0e41 7373 6574 4c69 7374 4d6f 6465 6c01  .AssetListModel.
+00002630: 0300 0000 1804 1d04 3004 3804 3c04 3504  ........0.8.<.5.
+00002640: 3d04 3e04 3204 3004 3d04 3804 3508 0000  =.>.2.0.=.8.5...
+00002650: 0000 0600 0000 044e 616d 6507 0000 000e  .......Name.....
+00002660: 4173 7365 744c 6973 744d 6f64 656c 0103  AssetListModel..
+00002670: 0000 000c 0421 0438 043c 0432 043e 043b  .....!.8.<.2.>.;
+00002680: 0800 0000 0006 0000 0006 5379 6d62 6f6c  ..........Symbol
+00002690: 0700 0000 0e41 7373 6574 4c69 7374 4d6f  .....AssetListMo
+000026a0: 6465 6c01 0300 0000 1804 1d04 3004 3804  del.........0.8.
+000026b0: 3c04 3504 3d04 3e04 3204 3004 3d04 3804  <.5.=.>.2.0.=.8.
+000026c0: 3508 0000 0000 0600 0000 0a41 7373 6574  5..........Asset
+000026d0: 206e 616d 6507 0000 000f 4173 7365 7473   name.....Assets
+000026e0: 4c69 7374 4d6f 6465 6c01 0300 0000 1a04  ListModel.......
+000026f0: 1104 3004 3704 3e04 3204 4b04 3900 2004  ..0.7.>.2.K.9. .
+00002700: 3004 3a04 4204 3804 3208 0000 0000 0600  0.:.B.8.2.......
+00002710: 0000 0a42 6173 6520 6173 7365 7407 0000  ...Base asset...
+00002720: 000f 4173 7365 7473 4c69 7374 4d6f 6465  ..AssetsListMode
+00002730: 6c01 0300 0000 0c04 2104 4204 4004 3004  l.......!.B.@.0.
+00002740: 3d04 3008 0000 0000 0600 0000 0743 6f75  =.0..........Cou
+00002750: 6e74 7279 0700 0000 0f41 7373 6574 734c  ntry.....AssetsL
+00002760: 6973 744d 6f64 656c 0103 0000 0008 0049  istModel.......I
+00002770: 0053 0049 004e 0800 0000 0006 0000 0004  .S.I.N..........
+00002780: 4953 494e 0700 0000 0f41 7373 6574 734c  ISIN.....AssetsL
+00002790: 6973 744d 6f64 656c 0103 0000 0008 0421  istModel.......!
+000027a0: 0447 0435 0442 0800 0000 0006 0000 0007  .G.5.B..........
+000027b0: 4163 636f 756e 7407 0000 000d 4261 6c61  Account.....Bala
+000027c0: 6e63 6573 4d6f 6465 6c01 0300 0000 0c04  ncesModel.......
+000027d0: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
+000027e0: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
+000027f0: 0d42 616c 616e 6365 734d 6f64 656c 0103  .BalancesModel..
+00002800: 0000 0010 0411 0430 043b 0430 043d 0441  .......0.;.0.=.A
+00002810: 002c 0020 0800 0000 0006 0000 0009 4261  .,. ..........Ba
+00002820: 6c61 6e63 652c 2007 0000 000d 4261 6c61  lance, .....Bala
+00002830: 6e63 6573 4d6f 6465 6c01 0300 0000 0a04  ncesModel.......
+00002840: 1804 4204 3e04 3304 3e08 0000 0000 0600  ..B.>.3.>.......
+00002850: 0000 0554 6f74 616c 0700 0000 0d42 616c  ...Total.....Bal
+00002860: 616e 6365 734d 6f64 656c 0103 0000 001c  ancesModel......
+00002870: 0411 0430 0437 043e 0432 0430 044f 0020  ...0.7.>.2.0.O. 
+00002880: 0432 0430 043b 044e 0442 0430 0800 0000  .2.0.;.N.B.0....
+00002890: 0006 0000 000d 4261 7365 2063 7572 7265  ......Base curre
+000028a0: 6e63 7907 0000 0012 4261 7365 4375 7272  ncy.....BaseCurr
+000028b0: 656e 6379 4469 616c 6f67 0103 0000 000c  encyDialog......
+000028c0: 0412 0430 043b 044e 0442 0430 0800 0000  ...0.;.N.B.0....
+000028d0: 0006 0000 0008 4375 7272 656e 6379 0700  ......Currency..
+000028e0: 0000 1542 6173 6543 7572 7265 6e63 794c  ...BaseCurrencyL
+000028f0: 6973 744d 6f64 656c 0103 0000 0008 0414  istModel........
+00002900: 0430 0442 0430 0800 0000 0006 0000 0004  .0.B.0..........
+00002910: 4461 7465 0700 0000 1542 6173 6543 7572  Date.....BaseCur
+00002920: 7265 6e63 794c 6973 744d 6f64 656c 0103  rencyListModel..
+00002930: 0000 0024 0027 0020 0437 0430 043c 0435  ...$.'. .7.0.<.5
+00002940: 043d 0435 043d 0430 0020 0443 0441 043f  .=.5.=.0. .C.A.?
+00002950: 0435 0448 043d 043e 0800 0000 0006 0000  .5.H.=.>........
+00002960: 001b 2720 7761 7320 7375 6363 6573 7366  ..' was successf
+00002970: 756c 6c79 2072 6570 6c61 6365 6407 0000  ully replaced...
+00002980: 0012 4361 7465 676f 7279 4c69 7374 4469  ..CategoryListDi
+00002990: 616c 6f67 0103 0000 000c 0027 0020 043d  alog.......'. .=
+000029a0: 0430 003a 0020 0800 0000 0006 0000 0008  .0.:. ..........
+000029b0: 2720 7769 7468 3a20 0700 0000 1243 6174  ' with: .....Cat
+000029c0: 6567 6f72 794c 6973 7444 6961 6c6f 6701  egoryListDialog.
+000029d0: 0300 0000 1204 1a04 3004 4204 3504 3304  ........0.B.5.3.
+000029e0: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
+000029f0: 0a43 6174 6567 6f72 6965 7307 0000 0012  .Categories.....
+00002a00: 4361 7465 676f 7279 4c69 7374 4469 616c  CategoryListDial
+00002a10: 6f67 0103 0000 0016 041a 0430 0442 0435  og.........0.B.5
+00002a20: 0433 043e 0440 0438 044f 0020 0027 0800  .3.>.@.8.O. .'..
+00002a30: 0000 0006 0000 000a 4361 7465 676f 7279  ........Category
+00002a40: 2027 0700 0000 1243 6174 6567 6f72 794c   '.....CategoryL
+00002a50: 6973 7444 6961 6c6f 6701 0300 0000 2804  istDialog.....(.
+00002a60: 1704 3004 3c04 3504 3d04 3804 4204 4c00  ..0.<.5.=.8.B.L.
+00002a70: 2004 3a04 3004 4204 3504 3304 3e04 4004   .:.0.B.5.3.>.@.
+00002a80: 3804 4e00 2000 2708 0000 0000 0600 0000  8.N. .'.........
+00002a90: 1252 6570 6c61 6365 2063 6174 6567 6f72  .Replace categor
+00002aa0: 7920 2707 0000 0012 4361 7465 676f 7279  y '.....Category
+00002ab0: 4c69 7374 4469 616c 6f67 0103 0000 001c  ListDialog......
+00002ac0: 0417 0430 043c 0435 043d 0438 0442 044c  ...0.<.5.=.8.B.L
+00002ad0: 0020 043d 0430 002e 002e 002e 0800 0000  . .=.0..........
+00002ae0: 0006 0000 000f 5265 706c 6163 6520 7769  ......Replace wi
+00002af0: 7468 2e2e 2e07 0000 0012 4361 7465 676f  th........Catego
+00002b00: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
+00002b10: 003c 041f 043e 043a 0430 0437 0430 0442  .<...>.:.0.7.0.B
+00002b20: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
+00002b30: 0438 0438 0020 0441 0020 041a 0430 0442  .8.8. .A. ...0.B
+00002b40: 0435 0433 043e 0440 0438 0435 0439 0800  .5.3.>.@.8.5.9..
+00002b50: 0000 0006 0000 001d 5368 6f77 206f 7065  ........Show ope
+00002b60: 7261 7469 6f6e 7320 7769 7468 2043 6174  rations with Cat
+00002b70: 6567 6f72 7907 0000 0012 4361 7465 676f  egory.....Catego
+00002b80: 7279 4c69 7374 4469 616c 6f67 0103 0000  ryListDialog....
+00002b90: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
+00002ba0: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
+00002bb0: 6174 696f 6e73 0700 0000 0e43 6174 6567  ations.....Categ
+00002bc0: 6f72 7952 6570 6f72 7401 0300 0000 1804  oryReport.......
+00002bd0: 3f04 3e00 2004 1a04 3004 4204 3504 3304  ?.>. ...0.B.5.3.
 00002be0: 3e04 4004 3804 3808 0000 0000 0600 0000  >.@.8.8.........
-00002bf0: 1252 6570 6f72 7420 6279 2063 6174 6567  .Report by categ
-00002c00: 6f72 7907 0000 0014 4361 7465 676f 7279  ory.....Category
-00002c10: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
-00002c20: 0018 041d 0430 0438 043c 0435 043d 043e  .....0.8.<.5.=.>
-00002c30: 0432 0430 043d 0438 0435 0800 0000 0006  .2.0.=.8.5......
-00002c40: 0000 0004 4e61 6d65 0700 0000 1143 6174  ....Name.....Cat
-00002c50: 6567 6f72 7954 7265 654d 6f64 656c 0103  egoryTreeModel..
-00002c60: 0000 000c 0427 0430 0441 0442 0430 044f  .....'.0.A.B.0.O
-00002c70: 0800 0000 0006 0000 0005 4f66 7465 6e07  ..........Often.
-00002c80: 0000 0011 4361 7465 676f 7279 5472 6565  ....CategoryTree
-00002c90: 4d6f 6465 6c01 0300 0000 2004 1304 4004  Model..... ...@.
-00002ca0: 3004 4404 3804 3a00 2004 4604 3504 3d04  0.D.8.:. .F.5.=.
-00002cb0: 4b00 2004 3404 3b04 4f00 2008 0000 0000  K. .4.;.O. .....
-00002cc0: 0600 0000 1050 7269 6365 2063 6861 7274  .....Price chart
-00002cd0: 2066 6f72 2007 0000 000b 4368 6172 7457   for .....ChartW
-00002ce0: 696e 646f 7701 0300 0000 1a04 2604 3504  indow.......&.5.
-00002cf0: 3d04 3d04 3004 4f00 2004 3104 4304 3c04  =.=.0.O. .1.C.<.
-00002d00: 3004 3304 3008 0000 0000 0600 0000 0541  0.3.0..........A
-00002d10: 7373 6574 0700 0000 1143 6c6f 7365 6454  sset.....ClosedT
-00002d20: 7261 6465 734d 6f64 656c 0103 0000 001a  radesModel......
-00002d30: 0414 0430 0442 0430 0020 0437 0430 043a  ...0.B.0. .7.0.:
-00002d40: 0440 044b 0442 0438 044f 0800 0000 0006  .@.K.B.8.O......
-00002d50: 0000 000a 436c 6f73 6520 4461 7465 0700  ....Close Date..
-00002d60: 0000 1143 6c6f 7365 6454 7261 6465 734d  ...ClosedTradesM
-00002d70: 6f64 656c 0103 0000 0026 0414 0430 0442  odel.....&...0.B
-00002d80: 0430 002f 0432 0440 0435 043c 044f 0020  .0./.2.@.5.<.O. 
-00002d90: 0437 0430 043a 0440 044b 0442 0438 044f  .7.0.:.@.K.B.8.O
-00002da0: 0800 0000 0006 0000 000f 436c 6f73 6520  ..........Close 
-00002db0: 4461 7465 2f54 696d 6507 0000 0011 436c  Date/Time.....Cl
-00002dc0: 6f73 6564 5472 6164 6573 4d6f 6465 6c01  osedTradesModel.
-00002dd0: 0300 0000 1a04 2604 3504 3d04 3000 2004  ......&.5.=.0. .
-00002de0: 3704 3004 3a04 4004 4b04 4204 3804 4f08  7.0.:.@.K.B.8.O.
-00002df0: 0000 0000 0600 0000 0b43 6c6f 7365 2050  .........Close P
-00002e00: 7269 6365 0700 0000 1143 6c6f 7365 6454  rice.....ClosedT
-00002e10: 7261 6465 734d 6f64 656c 0103 0000 0010  radesModel......
-00002e20: 041a 043e 043c 0438 0441 0441 0438 044f  ...>.<.8.A.A.8.O
-00002e30: 0800 0000 0006 0000 0003 4665 6507 0000  ..........Fee...
-00002e40: 0011 436c 6f73 6564 5472 6164 6573 4d6f  ..ClosedTradesMo
-00002e50: 6465 6c01 0300 0000 1404 1f04 4004 3804  del.........@.8.
-00002e60: 3c04 3504 4704 3004 3d04 3804 3508 0000  <.5.G.0.=.8.5...
-00002e70: 0000 0600 0000 044e 6f74 6507 0000 0011  .......Note.....
-00002e80: 436c 6f73 6564 5472 6164 6573 4d6f 6465  ClosedTradesMode
-00002e90: 6c01 0300 0000 1a04 1404 3004 4204 3000  l.........0.B.0.
-00002ea0: 2004 3e04 4204 3a04 4004 4b04 4204 3804   .>.B.:.@.K.B.8.
-00002eb0: 4f08 0000 0000 0600 0000 094f 7065 6e20  O..........Open 
-00002ec0: 4461 7465 0700 0000 1143 6c6f 7365 6454  Date.....ClosedT
-00002ed0: 7261 6465 734d 6f64 656c 0103 0000 0026  radesModel.....&
-00002ee0: 0414 0430 0442 0430 002f 0412 0440 0435  ...0.B.0./...@.5
-00002ef0: 043c 044f 0020 043e 0442 043a 0440 044b  .<.O. .>.B.:.@.K
-00002f00: 0442 0438 044f 0800 0000 0006 0000 000e  .B.8.O..........
-00002f10: 4f70 656e 2044 6174 652f 5469 6d65 0700  Open Date/Time..
-00002f20: 0000 1143 6c6f 7365 6454 7261 6465 734d  ...ClosedTradesM
-00002f30: 6f64 656c 0103 0000 001a 0426 0435 043d  odel.......&.5.=
-00002f40: 0430 0020 043e 0442 043a 0440 044b 0442  .0. .>.B.:.@.K.B
-00002f50: 0438 044f 0800 0000 0006 0000 000a 4f70  .8.O..........Op
-00002f60: 656e 2050 7269 6365 0700 0000 1143 6c6f  en Price.....Clo
-00002f70: 7365 6454 7261 6465 734d 6f64 656c 0103  sedTradesModel..
-00002f80: 0000 0006 041f 0438 0423 0800 0000 0006  .......8.#......
-00002f90: 0000 0003 502f 4c07 0000 0011 436c 6f73  ....P/L.....Clos
-00002fa0: 6564 5472 6164 6573 4d6f 6465 6c01 0300  edTradesModel...
-00002fb0: 0000 0c04 1f04 3804 2300 2c00 2000 2508  ......8.#.,. .%.
-00002fc0: 0000 0000 0600 0000 0650 2f4c 2c20 2507  .........P/L, %.
-00002fd0: 0000 0011 436c 6f73 6564 5472 6164 6573  ....ClosedTrades
-00002fe0: 4d6f 6465 6c01 0300 0000 0c04 1a04 3e04  Model.........>.
-00002ff0: 3b00 2d04 3204 3e08 0000 0000 0600 0000  ;.-.2.>.........
-00003000: 0351 7479 0700 0000 1143 6c6f 7365 6454  .Qty.....ClosedT
-00003010: 7261 6465 734d 6f64 656c 0103 0000 00a0  radesModel......
-00003020: 041a 043e 043b 0438 0447 0435 0442 0432  ...>.;.8.G.5.B.2
-00003030: 043e 0020 0446 0435 043d 043d 044b 0445  .>. .F.5.=.=.K.E
-00003040: 0020 0431 0443 043c 0430 0433 0020 043d  . .1.C.<.0.3. .=
-00003050: 0435 0434 043e 0441 0442 0430 0442 043e  .5.4.>.A.B.0.B.>
-00003060: 0447 043d 043e 0020 0434 043b 044f 0020  .G.=.>. .4.;.O. 
-00003070: 043e 0431 0440 0430 0431 043e 0442 043a  .>.1.@.0.1.>.B.:
-00003080: 0438 0020 043a 043e 0440 043f 043e 0440  .8. .:.>.@.?.>.@
-00003090: 0430 0442 0438 0432 043d 043e 0433 043e  .0.B.8.2.=.>.3.>
-000030a0: 0020 0441 043e 0431 044b 0442 0438 044f  . .A.>.1.K.B.8.O
-000030b0: 002e 0020 0414 0430 0442 0430 003a 0020  ... ...0.B.0.:. 
-000030c0: 0800 0000 0006 0000 0042 4173 7365 7420  .........BAsset 
-000030d0: 616d 6f75 6e74 2069 7320 6e6f 7420 656e  amount is not en
-000030e0: 6f75 6768 2066 6f72 2063 6f72 706f 7261  ough for corpora
-000030f0: 7465 2061 6374 696f 6e20 7072 6f63 6573  te action proces
-00003100: 7369 6e67 2e20 4461 7465 3a20 0700 0000  sing. Date: ....
-00003110: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003120: 0103 0000 0074 0426 0411 0020 043d 0435  .....t.&... .=.5
-00003130: 0020 044f 0432 043b 044f 0435 0442 0441  . .O.2.;.O.5.B.A
-00003140: 044f 0020 0447 0430 0441 0442 044c 044e  .O. .G.0.A.B.L.N
-00003150: 0020 0440 0435 0437 0443 043b 044c 0442  . .@.5.7.C.;.L.B
-00003160: 0430 0442 043e 0432 0020 043a 043e 0440  .0.B.>.2. .:.>.@
-00003170: 043f 043e 0440 0430 0442 0438 0432 043d  .?.>.@.0.B.8.2.=
-00003180: 043e 0433 043e 0020 0441 043e 0431 044b  .>.3.>. .A.>.1.K
-00003190: 0442 0438 044f 003a 0020 0800 0000 0006  .B.8.O.:. ......
-000031a0: 0000 0030 4173 7365 7420 6973 6e27 7420  ...0Asset isn't 
-000031b0: 6120 7061 7274 206f 6620 636f 7270 6f72  a part of corpor
-000031c0: 6174 6520 6163 7469 6f6e 2072 6573 756c  ate action resul
-000031d0: 7473 3a20 0700 0000 0f43 6f72 706f 7261  ts: .....Corpora
-000031e0: 7465 4163 7469 6f6e 0103 0000 0056 041d  teAction.....V..
-000031f0: 0435 0020 0437 0430 0434 0430 043d 0020  .5. .7.0.4.0.=. 
-00003200: 0442 0438 043f 0020 043a 043e 0440 043f  .B.8.?. .:.>.@.?
-00003210: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
-00003220: 0433 043e 0020 0441 043e 0431 044b 0442  .3.>. .A.>.1.K.B
-00003230: 0438 044f 002e 0020 0414 0430 0442 0430  .8.O... ...0.B.0
-00003240: 003a 0020 0800 0000 0006 0000 002b 436f  .:. .........+Co
-00003250: 7270 6f72 6174 6520 6163 7469 6f6e 2074  rporate action t
-00003260: 7970 6520 6973 6e27 7420 6465 6669 6e65  ype isn't define
-00003270: 642e 2044 6174 653a 2007 0000 000f 436f  d. Date: .....Co
-00003280: 7270 6f72 6174 6541 6374 696f 6e01 0300  rporateAction...
-00003290: 0000 1204 1404 3504 3b04 3804 4104 4204  ......5.;.8.A.B.
-000032a0: 3804 3d04 3308 0000 0000 0600 0000 0944  8.=.3..........D
-000032b0: 656c 6973 7469 6e67 0700 0000 0f43 6f72  elisting.....Cor
-000032c0: 706f 7261 7465 4163 7469 6f6e 0103 0000  porateAction....
-000032d0: 002c 0420 0435 043e 0440 0433 0430 043d  .,. .5.>.@.3.0.=
-000032e0: 0438 0437 0430 0446 0438 044f 0020 043a  .8.7.0.F.8.O. .:
-000032f0: 043e 043c 043f 0430 043d 0438 0438 0800  .>.<.?.0.=.8.8..
-00003300: 0000 0006 0000 0006 4d65 7267 6572 0700  ........Merger..
-00003310: 0000 0f43 6f72 706f 7261 7465 4163 7469  ...CorporateActi
-00003320: 6f6e 0103 0000 00ac 0420 0435 0437 0443  on....... .5.7.C
-00003330: 043b 044c 0442 0430 0442 044b 0020 043a  .;.L.B.0.B.K. .:
-00003340: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
-00003350: 0432 043d 043e 0433 043e 0020 0441 043e  .2.=.>.3.>. .A.>
-00003360: 0431 044b 0442 0438 044f 0020 043d 0435  .1.K.B.8.O. .=.5
-00003370: 0020 0440 0430 0441 043f 0440 0435 0434  . .@.0.A.?.@.5.4
-00003380: 0435 043b 044f 044e 0442 0020 0031 0030  .5.;.O.N.B. .1.0
-00003390: 0030 0025 0020 0441 0442 043e 0438 043c  .0.%. .A.B.>.8.<
-000033a0: 043e 0441 0442 0438 0020 0438 0437 043d  .>.A.B.8. .8.7.=
-000033b0: 0430 0447 0430 043b 044c 043d 043e 0433  .0.G.0.;.L.=.>.3
-000033c0: 043e 0020 0430 043a 0442 0438 0432 0430  .>. .0.:.B.8.2.0
-000033d0: 002e 0020 0800 0000 0006 0000 004d 5265  ... .........MRe
-000033e0: 7375 6c74 7320 7661 6c75 6520 6f66 2063  sults value of c
-000033f0: 6f72 706f 7261 7465 2061 6374 696f 6e20  orporate action 
-00003400: 646f 6573 6e27 7420 6d61 7463 6820 3130  doesn't match 10
-00003410: 3025 206f 6620 696e 6974 6961 6c20 6173  0% of initial as
-00003420: 7365 7420 7661 6c75 652e 2007 0000 000f  set value. .....
-00003430: 436f 7270 6f72 6174 6541 6374 696f 6e01  CorporateAction.
-00003440: 0300 0000 3a04 1204 4b04 3404 3504 3b04  ....:...K.4.5.;.
-00003450: 3504 3d04 3804 3500 2004 3a04 3e04 3c04  5.=.8.5. .:.>.<.
-00003460: 3f04 3004 3d04 3804 3800 2000 2804 4104  ?.0.=.8.8. .(.A.
-00003470: 3f04 3804 3d00 2d04 3e04 4404 4400 2908  ?.8.=.-.>.D.D.).
-00003480: 0000 0000 0600 0000 0853 7069 6e2d 6f66  .........Spin-of
-00003490: 6607 0000 000f 436f 7270 6f72 6174 6541  f.....CorporateA
-000034a0: 6374 696f 6e01 0300 0000 0a04 2104 3f04  ction.......!.?.
-000034b0: 3b04 3804 4208 0000 0000 0600 0000 0553  ;.8.B..........S
-000034c0: 706c 6974 0700 0000 0f43 6f72 706f 7261  plit.....Corpora
-000034d0: 7465 4163 7469 6f6e 0103 0000 001a 0421  teAction.......!
-000034e0: 043c 0435 043d 0430 0020 0441 0438 043c  .<.5.=.0. .A.8.<
-000034f0: 0432 043e 043b 0430 0800 0000 0006 0000  .2.>.;.0........
-00003500: 000d 5379 6d62 6f6c 2063 6861 6e67 6507  ..Symbol change.
-00003510: 0000 000f 436f 7270 6f72 6174 6541 6374  ....CorporateAct
-00003520: 696f 6e01 0300 0000 1804 1d04 1504 1e04  ion.............
-00003530: 1f04 2004 1504 1404 1504 1b04 1504 1d04  .. .............
-00003540: 1e08 0000 0000 0600 0000 0955 4e44 4546  ...........UNDEF
-00003550: 494e 4544 0700 0000 0f43 6f72 706f 7261  INED.....Corpora
-00003560: 7465 4163 7469 6f6e 0103 0000 00ae 041d  teAction........
-00003570: 0435 043f 043e 0434 0435 0440 0436 0438  .5.?.>.4.5.@.6.8
-00003580: 0432 0430 0435 043c 044b 0439 0020 0441  .2.0.5.<.K.9. .A
-00003590: 043b 0443 0447 0430 0439 003a 0020 041a  .;.C.G.0.9.:. ..
-000035a0: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
-000035b0: 0432 043d 043e 0435 0020 0441 043e 0431  .2.=.>.5. .A.>.1
-000035c0: 044b 0442 0438 0435 0020 043f 043e 043a  .K.B.8.5. .?.>.:
-000035d0: 0440 044b 0432 0430 0435 0442 0020 043d  .@.K.2.0.5.B. .=
-000035e0: 0435 0020 0432 0441 044e 0020 043e 0442  .5. .2.A.N. .>.B
-000035f0: 043a 0440 044b 0442 0443 044e 0020 043f  .:.@.K.B.C.N. .?
-00003600: 043e 0437 0438 0446 0438 044e 002e 0020  .>.7.8.F.8.N... 
-00003610: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
-00003620: 0006 0000 0046 556e 6861 6e64 6c65 6420  .....FUnhandled 
-00003630: 6361 7365 3a20 436f 7270 6f72 6174 6520  case: Corporate 
-00003640: 6163 7469 6f6e 2063 6f76 6572 7320 6e6f  action covers no
-00003650: 7420 6675 6c6c 206f 7065 6e20 706f 7369  t full open posi
-00003660: 7469 6f6e 2e20 4461 7465 3a20 0700 0000  tion. Date: ....
-00003670: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-00003680: 0103 0000 0002 2116 0800 0000 0006 0000  ......!.........
-00003690: 0001 2307 0000 0015 436f 7270 6f72 6174  ..#.....Corporat
-000036a0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
-000036b0: 0000 0804 2104 4704 3504 4208 0000 0000  ....!.G.5.B.....
-000036c0: 0600 0000 0741 6363 6f75 6e74 0700 0000  .....Account....
-000036d0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
-000036e0: 5769 6467 6574 0103 0000 001c 0414 043e  Widget.........>
-000036f0: 0431 0430 0432 0438 0442 044c 0020 0430  .1.0.2.8.B.L. .0
-00003700: 043a 0442 0438 0432 0800 0000 0006 0000  .:.B.8.2........
-00003710: 0009 4164 6420 6173 7365 7407 0000 0015  ..Add asset.....
-00003720: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003730: 6964 6765 7401 0300 0000 0404 2604 1108  idget.......&...
-00003740: 0000 0000 0600 0000 0541 7373 6574 0700  .........Asset..
-00003750: 0000 1543 6f72 706f 7261 7465 4163 7469  ...CorporateActi
-00003760: 6f6e 5769 6467 6574 0103 0000 002c 041a  onWidget.....,..
-00003770: 043e 0440 043f 043e 0440 0430 0442 0438  .>.@.?.>.@.0.B.8
-00003780: 0432 043d 043e 0435 0020 0434 0435 0439  .2.=.>.5. .4.5.9
-00003790: 0441 0442 0432 0438 0435 0800 0000 0006  .A.B.2.8.5......
-000037a0: 0000 0010 436f 7270 6f72 6174 6520 4163  ....Corporate Ac
-000037b0: 7469 6f6e 0700 0000 1543 6f72 706f 7261  tion.....Corpora
-000037c0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-000037d0: 0000 0014 0414 0430 0442 0430 002f 0412  .......0.B.0./..
-000037e0: 0440 0435 043c 044f 0800 0000 0006 0000  .@.5.<.O........
-000037f0: 0009 4461 7465 2f54 696d 6507 0000 0015  ..Date/Time.....
-00003800: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
-00003810: 6964 6765 7401 0300 0000 1204 1404 3504  idget.........5.
-00003820: 3b04 3804 4104 4204 3804 3d04 3308 0000  ;.8.A.B.8.=.3...
-00003830: 0000 0600 0000 0944 656c 6973 7469 6e67  .......Delisting
-00003840: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003850: 7469 6f6e 5769 6467 6574 0103 0000 0044  tionWidget.....D
-00003860: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00003870: 043d 043e 0020 0434 043e 0431 0430 0432  .=.>. .4.>.1.0.2
-00003880: 0438 0442 044c 0020 043d 043e 0432 0443  .8.B.L. .=.>.2.C
-00003890: 044e 0020 0437 0430 043f 0438 0441 044c  .N. .7.0.?.8.A.L
-000038a0: 003a 0020 0800 0000 0006 0000 001a 4661  .:. ..........Fa
-000038b0: 696c 6564 2074 6f20 6164 6420 6e65 7720  iled to add new 
-000038c0: 7265 636f 7264 3a20 0700 0000 1543 6f72  record: .....Cor
-000038d0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-000038e0: 6574 0103 0000 0028 041e 0431 044a 0435  et.....(...1.J.5
-000038f0: 0434 0438 043d 0435 043d 0438 0435 0020  .4.8.=.5.=.8.5. 
-00003900: 043a 043e 043c 043f 0430 043d 0438 0438  .:.>.<.?.0.=.8.8
-00003910: 0800 0000 0006 0000 0006 4d65 7267 6572  ..........Merger
-00003920: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
-00003930: 7469 6f6e 5769 6467 6574 0103 0000 0006  tionWidget......
-00003940: 004e 002f 0041 0800 0000 0006 0000 0003  .N./.A..........
-00003950: 4e2f 4107 0000 0015 436f 7270 6f72 6174  N/A.....Corporat
-00003960: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
-00003970: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
-00003980: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
-00003990: 6507 0000 0015 436f 7270 6f72 6174 6541  e.....CorporateA
-000039a0: 6374 696f 6e57 6964 6765 7401 0300 0000  ctionWidget.....
-000039b0: 4804 1e04 4804 3804 3104 3a04 3000 2004  H...H.8.1.:.0. .
-000039c0: 3f04 4004 3800 2004 3704 3004 3f04 3804  ?.@.8. .7.0.?.8.
-000039d0: 4104 3800 2004 3404 3504 4204 3004 3b04  A.8. .4.5.B.0.;.
-000039e0: 3504 3900 2004 3e04 3f04 3504 4004 3004  5.9. .>.?.5.@.0.
-000039f0: 4604 3804 3800 3a00 2008 0000 0000 0600  F.8.8.:. .......
-00003a00: 0000 214f 7065 7261 7469 6f6e 2064 6574  ..!Operation det
-00003a10: 6169 6c73 2073 7562 6d69 7420 6661 696c  ails submit fail
-00003a20: 6564 3a20 0700 0000 1543 6f72 706f 7261  ed: .....Corpora
-00003a30: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-00003a40: 0000 0038 041e 0448 0438 0431 043a 0430  ...8...H.8.1.:.0
-00003a50: 0020 043f 0440 0438 0020 0437 0430 043f  . .?.@.8. .7.0.?
-00003a60: 0438 0441 0438 0020 043e 043f 0435 0440  .8.A.8. .>.?.5.@
-00003a70: 0430 0446 0438 0438 003a 0020 0800 0000  .0.F.8.8.:. ....
-00003a80: 0006 0000 0019 4f70 6572 6174 696f 6e20  ......Operation 
-00003a90: 7375 626d 6974 2066 6169 6c65 643a 2007  submit failed: .
-00003aa0: 0000 0015 436f 7270 6f72 6174 6541 6374  ....CorporateAct
-00003ab0: 696f 6e57 6964 6765 7401 0300 0000 0c04  ionWidget.......
-00003ac0: 1a04 3e04 3b00 2d04 3204 3e08 0000 0000  ..>.;.-.2.>.....
-00003ad0: 0600 0000 0351 7479 0700 0000 1543 6f72  .....Qty.....Cor
-00003ae0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-00003af0: 6574 0103 0000 001a 0423 0434 0430 043b  et.......#.4.0.;
-00003b00: 0438 0442 044c 0020 0430 043a 0442 0438  .8.B.L. .0.:.B.8
-00003b10: 0432 0800 0000 0006 0000 000c 5265 6d6f  .2..........Remo
-00003b20: 7665 2061 7373 6574 0700 0000 1543 6f72  ve asset.....Cor
-00003b30: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-00003b40: 6574 0103 ffff ffff 0800 0000 0006 0000  et..............
-00003b50: 0008 5370 696e 2d4f 6666 0700 0000 1543  ..Spin-Off.....C
-00003b60: 6f72 706f 7261 7465 4163 7469 6f6e 5769  orporateActionWi
-00003b70: 6467 6574 0103 0000 000a 0421 043f 043b  dget.......!.?.;
-00003b80: 0438 0442 0800 0000 0006 0000 0005 5370  .8.B..........Sp
-00003b90: 6c69 7407 0000 0015 436f 7270 6f72 6174  lit.....Corporat
-00003ba0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
-00003bb0: 0000 1a04 2104 3c04 3504 3d04 3000 2004  ....!.<.5.=.0. .
-00003bc0: 4104 3804 3c04 3204 3e04 3b04 3008 0000  A.8.<.2.>.;.0...
-00003bd0: 0000 0600 0000 0d53 796d 626f 6c20 6368  .......Symbol ch
-00003be0: 616e 6765 0700 0000 1543 6f72 706f 7261  ange.....Corpora
-00003bf0: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
-00003c00: 0000 0006 0422 0438 043f 0800 0000 0006  .....".8.?......
-00003c10: 0000 0004 5479 7065 0700 0000 1543 6f72  ....Type.....Cor
-00003c20: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
-00003c30: 6574 0103 0000 0034 0424 043e 0440 043c  et.....4.$.>.@.<
-00003c40: 0430 0442 0020 0431 0430 0437 044b 0020  .0.B. .1.0.7.K. 
-00003c50: 0434 0430 043d 043d 044b 0445 0020 0443  .4.0.=.=.K.E. .C
-00003c60: 0441 0442 0430 0440 0435 043b 0800 0000  .A.B.0.@.5.;....
-00003c70: 0006 0000 001b 4461 7461 6261 7365 2066  ......Database f
-00003c80: 6f72 6d61 7420 6973 206f 7574 6461 7465  ormat is outdate
-00003c90: 6407 0000 0002 4442 0103 0000 0064 0412  d.....DB.....d..
-00003ca0: 044b 0020 0441 043e 0433 043b 0430 0441  .K. .A.>.3.;.0.A
-00003cb0: 043d 044b 0020 0441 043a 043e 043d 0432  .=.K. .A.:.>.=.2
-00003cc0: 0435 0440 0442 0438 0440 043e 0432 0430  .5.@.B.8.@.>.2.0
-00003cd0: 0442 044c 0020 0434 0430 043d 043d 044b  .B.L. .4.0.=.=.K
-00003ce0: 0435 0020 0432 0020 043d 043e 0432 044b  .5. .2. .=.>.2.K
-00003cf0: 0439 0020 0444 043e 0440 043c 0430 0442  .9. .D.>.@.<.0.B
-00003d00: 003f 0800 0000 0006 0000 0032 446f 2079  .?.........2Do y
-00003d10: 6f75 2061 6772 6565 2074 6f20 7570 6772  ou agree to upgr
-00003d20: 6164 6520 796f 7572 2064 6174 6120 746f  ade your data to
-00003d30: 206e 6577 6572 2066 6f72 6d61 743f 0700   newer format?..
-00003d40: 0000 0244 4201 0300 0000 5e04 2404 3e04  ...DB.....^.$.>.
-00003d50: 4004 3c04 3000 2000 3300 2d04 1d04 1404  @.<.0. .3.-.....
-00003d60: 2404 1b00 2004 3404 3b04 4f00 2004 4d04  $... .4.;.O. .M.
-00003d70: 4204 3e04 3304 3e00 2004 3304 3e04 3404  B.>.3.>. .3.>.4.
-00003d80: 3000 2004 3d04 3500 2004 3f04 3e04 3404  0. .=.5. .?.>.4.
-00003d90: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
-00003da0: 4204 4104 4f00 3a00 2008 0000 0000 0600  B.A.O.:. .......
-00003db0: 0000 2633 2d4e 4446 4c20 666f 726d 2069  ..&3-NDFL form i
-00003dc0: 736e 2774 2073 7570 6f6f 7274 6564 2066  sn't supoorted f
-00003dd0: 6f72 2079 6561 723a 2007 0000 0004 444c  or year: .....DL
-00003de0: 5347 0103 0000 0086 0421 0442 0440 0430  SG.......!.B.@.0
-00003df0: 043d 0430 0020 0426 0411 0020 043d 0435  .=.0. .&... .=.5
-00003e00: 0020 0437 0430 0434 0430 043d 0430 002c  . .7.0.4.0.=.0.,
-00003e10: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
-00003e20: 0434 0020 043d 0435 0020 0431 0443 0434  .4. .=.5. .1.C.4
-00003e30: 0435 0442 0020 0432 043a 043b 044e 0447  .5.B. .2.:.;.N.G
-00003e40: 0451 043d 0020 0432 0020 0434 0435 043a  .Q.=. .2. .4.5.:
-00003e50: 043b 0430 0440 0430 0446 0438 044e 0020  .;.0.@.0.F.8.N. 
-00003e60: 0033 002d 041d 0424 0414 041b 0020 0800  .3.-...$..... ..
-00003e70: 0000 0006 0000 0047 4163 636f 756e 7420  .......GAccount 
-00003e80: 636f 756e 7472 7920 6973 206e 6f74 2073  country is not s
-00003e90: 6574 2066 6f72 2061 7373 6574 2c20 6469  et for asset, di
-00003ea0: 7669 6465 6e64 2069 736e 2774 2069 6e63  vidend isn't inc
-00003eb0: 6c75 6465 2069 6e20 332d 4e44 464c 2007  lude in 3-NDFL .
-00003ec0: 0000 0004 444c 5347 0103 0000 004a 0412  ....DLSG.....J..
-00003ed0: 0430 043b 044e 0442 0430 0020 043d 0435  .0.;.N.B.0. .=.5
-00003ee0: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
-00003ef0: 0438 0432 0430 0435 0442 0441 044f 0020  .8.2.0.5.B.A.O. 
-00003f00: 0434 043b 044f 0020 0033 002d 041d 0414  .4.;.O. .3.-....
-00003f10: 0424 041b 003a 0020 0800 0000 0006 0000  .$...:. ........
-00003f20: 0026 4375 7272 656e 6379 2069 7320 6e6f  .&Currency is no
-00003f30: 7420 7375 7070 6f72 7465 6420 666f 7220  t supported for 
-00003f40: 332d 4e44 464c 3a20 0700 0000 0444 4c53  3-NDFL: .....DLS
-00003f50: 4701 0300 0000 1404 4d04 3a04 4104 3f04  G.......M.:.A.?.
-00003f60: 3804 4004 3004 4604 3804 4f08 0000 0000  8.@.0.F.8.O.....
-00003f70: 0600 0000 0665 7870 6972 7907 0000 000c  .....expiry.....
-00003f80: 4461 7461 4465 6c65 6761 7465 0103 0000  DataDelegate....
-00003f90: 000e 043d 043e 043c 0438 043d 0430 043b  ...=.>.<.8.=.0.;
-00003fa0: 0800 0000 0006 0000 0009 7072 696e 6369  ..........princi
-00003fb0: 7061 6c07 0000 000c 4461 7461 4465 6c65  pal.....DataDele
-00003fc0: 6761 7465 0103 0000 000e 0440 0435 0433  gate.......@.5.3
-00003fd0: 002e 043a 043e 0434 0800 0000 0006 0000  ...:.>.4........
-00003fe0: 0008 7265 672e 636f 6465 0700 0000 0c44  ..reg.code.....D
-00003ff0: 6174 6144 656c 6567 6174 6501 0300 0000  ataDelegate.....
-00004000: 1004 1204 4104 3500 2004 3404 3004 4204  ....A.5. .4.0.B.
-00004010: 4b08 0000 0000 0600 0000 0941 6c6c 2064  K..........All d
-00004020: 6174 6573 0700 0000 1144 6174 6552 616e  ates.....DateRan
-00004030: 6765 5365 6c65 6374 6f72 0103 0000 0004  geSelector......
-00004040: 0421 003a 0800 0000 0006 0000 0005 4672  .!.:..........Fr
-00004050: 6f6d 3a07 0000 0011 4461 7465 5261 6e67  om:.....DateRang
-00004060: 6553 656c 6563 746f 7201 0300 0000 0a04  eSelector.......
-00004070: 1c04 3504 4104 4f04 4608 0000 0000 0600  ..5.A.O.F.......
-00004080: 0000 054d 6f6e 7468 0700 0000 1144 6174  ...Month.....Dat
-00004090: 6552 616e 6765 5365 6c65 6374 6f72 0103  eRangeSelector..
-000040a0: 0000 001c 041f 0440 0435 0434 044b 0434  .......@.5.4.K.4
-000040b0: 0443 0449 0438 0439 0020 0433 043e 0434  .C.I.8.9. .3.>.4
-000040c0: 0800 0000 0006 0000 000d 5072 6576 696f  ..........Previo
-000040d0: 7573 2079 6561 7207 0000 0011 4461 7465  us year.....Date
-000040e0: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
-000040f0: 0000 0e04 1a04 3204 3004 4004 4204 3004  ......2.0.@.B.0.
-00004100: 3b08 0000 0000 0600 0000 0751 7561 7274  ;..........Quart
-00004110: 6572 0700 0000 1144 6174 6552 616e 6765  er.....DateRange
-00004120: 5365 6c65 6374 6f72 0103 0000 0024 0422  Selector.....$."
-00004130: 0435 043a 0443 0449 0438 0439 0020 0434  .5.:.C.I.8.9. .4
-00004140: 043e 0020 0441 0435 0433 043e 0434 043d  .>. .A.5.3.>.4.=
-00004150: 044f 0800 0000 0006 0000 000f 5175 6172  .O..........Quar
-00004160: 7465 7220 746f 2064 6174 6507 0000 0011  ter to date.....
-00004170: 4461 7465 5261 6e67 6553 656c 6563 746f  DateRangeSelecto
-00004180: 7201 0300 0000 1604 2204 3504 3a04 4304  r.......".5.:.C.
-00004190: 4904 3804 3900 2004 3304 3e04 3408 0000  I.8.9. .3.>.4...
-000041a0: 0000 0600 0000 0954 6869 7320 7965 6172  .......This year
-000041b0: 0700 0000 1144 6174 6552 616e 6765 5365  .....DateRangeSe
-000041c0: 6c65 6374 6f72 0103 0000 0006 0414 043e  lector.........>
-000041d0: 003a 0800 0000 0006 0000 0003 546f 3a07  .:..........To:.
-000041e0: 0000 0011 4461 7465 5261 6e67 6553 656c  ....DateRangeSel
-000041f0: 6563 746f 7201 0300 0000 0c04 1d04 3504  ector.........5.
-00004200: 3404 3504 3b04 4f08 0000 0000 0600 0000  4.5.;.O.........
-00004210: 0457 6565 6b07 0000 0011 4461 7465 5261  .Week.....DateRa
-00004220: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
-00004230: 0604 1304 3e04 3408 0000 0000 0600 0000  ....>.4.........
-00004240: 0459 6561 7207 0000 0011 4461 7465 5261  .Year.....DateRa
-00004250: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
-00004260: 1c04 1304 3e04 3400 2004 3404 3e00 2004  ....>.4. .4.>. .
-00004270: 4104 3504 3304 3e04 3404 3d04 4f08 0000  A.5.3.>.4.=.O...
-00004280: 0000 0600 0000 0c59 6561 7220 746f 2064  .......Year to d
-00004290: 6174 6507 0000 0011 4461 7465 5261 6e67  ate.....DateRang
-000042a0: 6553 656c 6563 746f 7201 0300 0000 1e04  eSelector.......
-000042b0: 2104 3404 3504 3b04 3a04 3800 2004 3f04  !.4.5.;.:.8. .?.
-000042c0: 3e00 2004 4104 4704 3504 4204 4308 0000  >. .A.G.5.B.C...
-000042d0: 0000 0600 0000 1044 6561 6c73 2062 7920  .......Deals by 
-000042e0: 4163 636f 756e 7407 0000 000b 4465 616c  Account.....Deal
-000042f0: 7352 6570 6f72 7401 0300 0000 0a04 2104  sReport.......!.
-00004300: 4704 3504 4200 3a08 0000 0000 0600 0000  G.5.B.:.........
-00004310: 0841 6363 6f75 6e74 3a07 0000 0011 4465  .Account:.....De
-00004320: 616c 7352 6570 6f72 7457 6964 6765 7401  alsReportWidget.
-00004330: 0300 0000 0c04 2104 3404 3504 3b04 3a04  ......!.4.5.;.:.
-00004340: 3808 0000 0000 0600 0000 0544 6561 6c73  8..........Deals
-00004350: 0700 0000 1144 6561 6c73 5265 706f 7274  .....DealsReport
-00004360: 5769 6467 6574 0103 0000 0020 0413 0440  Widget..... ...@
-00004370: 0443 043f 043f 0438 0440 043e 0432 0430  .C.?.?.8.@.>.2.0
-00004380: 0442 044c 0020 043f 043e 003a 0800 0000  .B.L. .?.>.:....
-00004390: 0006 0000 0009 4772 6f75 7020 6279 3a07  ......Group by:.
-000043a0: 0000 0011 4465 616c 7352 6570 6f72 7457  ....DealsReportW
-000043b0: 6964 6765 7401 0300 0000 0e00 3c04 1f04  idget.......<...
-000043c0: 4304 4104 4204 3e00 3e08 0000 0000 0600  C.A.B.>.>.......
-000043d0: 0000 063c 4e6f 6e65 3e07 0000 0011 4465  ...<None>.....De
-000043e0: 616c 7352 6570 6f72 7457 696e 646f 7701  alsReportWindow.
-000043f0: 0300 0000 1a04 2604 3504 3d04 3d04 3004  ......&.5.=.=.0.
-00004400: 4f00 2004 3104 4304 3c04 3004 3304 3008  O. .1.C.<.0.3.0.
-00004410: 0000 0000 0600 0000 0541 7373 6574 0700  .........Asset..
-00004420: 0000 1144 6561 6c73 5265 706f 7274 5769  ...DealsReportWi
-00004430: 6e64 6f77 0103 0000 0030 0426 0411 0020  ndow.....0.&... 
-00004440: 002d 0020 041e 0442 043a 0440 044b 0442  .-. ...B.:.@.K.B
-00004450: 0438 0435 0020 002d 0020 0417 0430 043a  .8.5. .-. ...0.:
-00004460: 0440 044b 0442 0438 0435 0800 0000 0006  .@.K.B.8.5......
-00004470: 0000 0014 4173 7365 7420 2d20 4f70 656e  ....Asset - Open
-00004480: 202d 2043 6c6f 7365 0700 0000 1144 6561   - Close.....Dea
-00004490: 6c73 5265 706f 7274 5769 6e64 6f77 0103  lsReportWindow..
-000044a0: 0000 0010 0417 0430 043a 0440 044b 0442  .......0.:.@.K.B
-000044b0: 0438 0435 0800 0000 0006 0000 0005 436c  .8.5..........Cl
-000044c0: 6f73 6507 0000 0011 4465 616c 7352 6570  ose.....DealsRep
-000044d0: 6f72 7457 696e 646f 7701 0300 0000 2604  ortWindow.....&.
-000044e0: 1704 3004 3a04 4004 4b04 4204 3804 3500  ..0.:.@.K.B.8.5.
-000044f0: 2000 2d00 2004 1e04 4204 3a04 4004 4b04   .-. ...B.:.@.K.
-00004500: 4204 3804 3508 0000 0000 0600 0000 0c43  B.8.5..........C
-00004510: 6c6f 7365 202d 204f 7065 6e07 0000 0011  lose - Open.....
-00004520: 4465 616c 7352 6570 6f72 7457 696e 646f  DealsReportWindo
-00004530: 7701 0300 0000 2604 1e04 4204 3a04 4004  w.....&...B.:.@.
-00004540: 4b04 4204 3804 3500 2000 2d00 2004 1704  K.B.8.5. .-. ...
-00004550: 3004 3a04 4004 4b04 4204 3804 3508 0000  0.:.@.K.B.8.5...
-00004560: 0000 0600 0000 0c4f 7065 6e20 2d20 436c  .......Open - Cl
-00004570: 6f73 6507 0000 0011 4465 616c 7352 6570  ose.....DealsRep
-00004580: 6f72 7457 696e 646f 7701 0300 0000 0a04  ortWindow.......
-00004590: 2104 4304 3c04 3c04 3008 0000 0000 0600  !.C.<.<.0.......
-000045a0: 0000 0641 6d6f 756e 7407 0000 000c 4465  ...Amount.....De
-000045b0: 7461 696c 734d 6f64 656c 0103 0000 0012  tailsModel......
-000045c0: 041a 0430 0442 0435 0433 043e 0440 0438  ...0.B.5.3.>.@.8
-000045d0: 044f 0800 0000 0006 0000 0008 4361 7465  .O..........Cate
-000045e0: 676f 7279 0700 0000 0c44 6574 6169 6c73  gory.....Details
-000045f0: 4d6f 6465 6c01 0300 0000 1004 1e04 3f04  Model.........?.
-00004600: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
-00004610: 0600 0000 044e 6f74 6507 0000 000c 4465  .....Note.....De
-00004620: 7461 696c 734d 6f64 656c 0103 0000 000a  tailsModel......
-00004630: 041c 0435 0442 043a 0430 0800 0000 0006  ...5.B.:.0......
-00004640: 0000 0003 5461 6707 0000 000c 4465 7461  ....Tag.....Deta
-00004650: 696c 734d 6f64 656c 0103 0000 009e 041d  ilsModel........
-00004660: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00004670: 043e 0020 043e 0431 0440 0430 0431 043e  .>. .>.1.@.0.1.>
-00004680: 0442 0430 0442 044c 0020 0434 0438 0432  .B.0.B.L. .4.8.2
-00004690: 0438 0434 0435 043d 0434 002c 0020 0442  .8.4.5.=.4.,. .B
-000046a0: 002e 043a 002e 0020 043d 0435 0020 0443  ...:... .=.5. .C
-000046b0: 043a 0430 0437 0430 043d 0020 0431 0430  .:.0.7.0.=. .1.0
-000046c0: 043d 043a 0020 0434 043b 044f 0020 0438  .=.:. .4.;.O. .8
-000046d0: 043d 0432 0435 0441 0442 0438 0446 0438  .=.2.5.A.B.8.F.8
-000046e0: 043e 043d 043d 043e 0433 043e 0020 0441  .>.=.=.>.3.>. .A
-000046f0: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
-00004700: 0006 0000 0041 4361 6e27 7420 7072 6f63  .....ACan't proc
-00004710: 6573 7320 6469 7669 6465 6e64 2061 7320  ess dividend as 
-00004720: 6261 6e6b 2069 736e 2774 2073 6574 2066  bank isn't set f
-00004730: 6f72 2069 6e76 6573 746d 656e 7420 6163  or investment ac
-00004740: 636f 756e 743a 2007 0000 0008 4469 7669  count: .....Divi
-00004750: 6465 6e64 0103 0000 005a 041d 0435 0020  dend.....Z...5. 
-00004760: 0437 0430 0434 0430 043d 0430 0020 0446  .7.0.4.0.=.0. .F
-00004770: 0435 043d 0430 0020 0434 043b 044f 0020  .5.=.0. .4.;.O. 
-00004780: 0432 044b 043f 043b 0430 0442 044b 0020  .2.K.?.;.0.B.K. 
-00004790: 0446 0435 043d 043d 044b 043c 0438 0020  .F.5.=.=.K.<.8. 
-000047a0: 0431 0443 043c 0430 0433 0430 043c 0438  .1.C.<.0.3.0.<.8
-000047b0: 003a 0020 0800 0000 0006 0000 002a 4e6f  .:. .........*No
-000047c0: 2070 7269 6365 2064 6174 6120 666f 7220   price data for 
-000047d0: 7374 6f63 6b20 6469 7669 6465 6e64 2f76  stock dividend/v
-000047e0: 6573 7469 6e67 3a20 0700 0000 0844 6976  esting: .....Div
-000047f0: 6964 656e 6401 0300 0000 7204 1d04 3504  idend.....r...5.
-00004800: 4200 2004 3a04 3e04 4204 3804 4004 3e04  B. .:.>.B.8.@.>.
-00004810: 3204 3a04 3800 2004 3404 3b04 4f00 2004  2.:.8. .4.;.O. .
-00004820: 3404 3804 3204 3804 3404 3504 3d04 3404  4.8.2.8.4.5.=.4.
-00004830: 3000 2004 3004 3a04 4604 3804 4f04 3c04  0. .0.:.F.8.O.<.
-00004840: 3800 2004 3804 3b04 3800 2004 3704 3004  8. .8.;.8. .7.0.
-00004850: 4704 3804 4104 3b04 3504 3d04 3804 4f00  G.8.A.;.5.=.8.O.
-00004860: 2004 3004 3a04 4604 3804 3900 2e08 0000   .0.:.F.8.9.....
-00004870: 0000 0600 0000 2d4e 6f20 7374 6f63 6b20  ......-No stock 
-00004880: 7175 6f74 6520 666f 7220 7374 6f63 6b20  quote for stock 
-00004890: 6469 7669 6465 6e64 206f 7220 7665 7374  dividend or vest
-000048a0: 696e 672e 0700 0000 0844 6976 6964 656e  ing......Dividen
-000048b0: 6401 0300 0000 b804 1d04 3504 3f04 3e04  d.........5.?.>.
-000048c0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-000048d0: 3504 3c04 3e04 3500 2004 3404 3504 3904  5.<.>.5. .4.5.9.
-000048e0: 4104 4204 3204 3804 3500 3a00 2004 3404  A.B.2.8.5.:. .4.
-000048f0: 3804 3204 3804 3404 3504 3d04 3400 2004  8.2.8.4.5.=.4. .
-00004900: 3004 3a04 4604 3804 4f04 3c04 3800 2004  0.:.F.8.O.<.8. .
-00004910: 3804 3b04 3800 2004 3704 3004 4704 3804  8.;.8. .7.0.G.8.
-00004920: 4104 3b04 3504 3d04 3804 3500 2004 3004  A.;.5.=.8.5. .0.
-00004930: 3a04 4604 3804 3900 2004 3704 3004 3a04  :.F.8.9. .7.0.:.
-00004940: 4004 4b04 3204 3004 3504 4200 2004 3a04  @.K.2.0.5.B. .:.
-00004950: 3e04 4004 3e04 4204 3a04 4304 4e00 2004  >.@.>.B.:.C.N. .
-00004960: 3f04 3e04 3704 3804 4604 3804 4e00 2e08  ?.>.7.8.F.8.N...
-00004970: 0000 0000 0600 0000 434e 6f74 2073 7570  ........CNot sup
-00004980: 706f 7274 6564 2061 6374 696f 6e3a 2073  ported action: s
-00004990: 746f 636b 2064 6976 6964 656e 6420 6f72  tock dividend or
-000049a0: 2076 6573 7469 6e67 2063 6c6f 7365 7320   vesting closes 
-000049b0: 7368 6f72 7420 7472 6164 652e 0700 0000  short trade.....
-000049c0: 0844 6976 6964 656e 6401 0300 0000 0e04  .Dividend.......
-000049d0: 1d04 3004 3b04 3e04 3300 3a00 2008 0000  ..0.;.>.3.:. ...
-000049e0: 0000 0600 0000 0554 6178 3a20 0700 0000  .......Tax: ....
-000049f0: 0844 6976 6964 656e 6401 0300 0000 3e04  .Dividend.....>.
-00004a00: 1d04 3504 3f04 3e04 3404 3404 3504 4004  ..5.?.>.4.4.5.@.
-00004a10: 3604 3804 3204 3004 3504 3c04 4b04 3900  6.8.2.0.5.<.K.9.
-00004a20: 2004 4204 3804 3f00 2004 3404 3804 3204   .B.8.?. .4.8.2.
-00004a30: 3804 3404 3504 3d04 3404 3000 2e08 0000  8.4.5.=.4.0.....
-00004a40: 0000 0600 0000 1a55 6e73 7570 706f 7274  .......Unsupport
-00004a50: 6564 2064 6976 6964 656e 6420 7479 7065  ed dividend type
-00004a60: 2e07 0000 0008 4469 7669 6465 6e64 0103  ......Dividend..
-00004a70: 0000 0002 2116 0800 0000 0006 0000 0001  ....!...........
-00004a80: 2307 0000 000e 4469 7669 6465 6e64 5769  #.....DividendWi
-00004a90: 6467 6574 0103 0000 0008 0421 0447 0435  dget.......!.G.5
-00004aa0: 0442 0800 0000 0006 0000 0007 4163 636f  .B..........Acco
-00004ab0: 756e 7407 0000 000e 4469 7669 6465 6e64  unt.....Dividend
-00004ac0: 5769 6467 6574 0103 0000 0004 0426 0411  Widget.......&..
-00004ad0: 0800 0000 0006 0000 0005 4173 7365 7407  ..........Asset.
-00004ae0: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
-00004af0: 6574 0103 0000 000a 041a 0443 043f 043e  et.........C.?.>
-00004b00: 043d 0800 0000 0006 0000 000d 426f 6e64  .=..........Bond
-00004b10: 2049 6e74 6572 6573 7407 0000 000e 4469   Interest.....Di
-00004b20: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004b30: 0014 0414 0430 0442 0430 002f 0412 0440  .....0.B.0./...@
-00004b40: 0435 043c 044f 0800 0000 0006 0000 0009  .5.<.O..........
-00004b50: 4461 7465 2f54 696d 6507 0000 000e 4469  Date/Time.....Di
-00004b60: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004b70: 0010 0414 0438 0432 0438 0434 0435 043d  .....8.2.8.4.5.=
-00004b80: 0434 0800 0000 0006 0000 0008 4469 7669  .4..........Divi
-00004b90: 6465 6e64 0700 0000 0e44 6976 6964 656e  dend.....Dividen
-00004ba0: 6457 6964 6765 7401 0300 0000 0e04 1e04  dWidget.........
-00004bb0: 4204 4104 3504 4704 3a04 3008 0000 0000  B.A.5.G.:.0.....
-00004bc0: 0600 0000 0745 782d 4461 7465 0700 0000  .....Ex-Date....
-00004bd0: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
-00004be0: 0300 0000 0600 4e00 2f00 4108 0000 0000  ......N./.A.....
-00004bf0: 0600 0000 034e 2f41 0700 0000 0e44 6976  .....N/A.....Div
-00004c00: 6964 656e 6457 6964 6765 7401 0300 0000  idendWidget.....
-00004c10: 1a04 1d04 3504 4200 2004 3a04 3e04 4204  ....5.B. .:.>.B.
-00004c20: 3804 4004 3e04 3204 3a04 3808 0000 0000  8.@.>.2.:.8.....
-00004c30: 0600 0000 084e 6f20 7175 6f74 6507 0000  .....No quote...
-00004c40: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
-00004c50: 0103 0000 0010 041e 043f 0438 0441 0430  .........?.8.A.0
-00004c60: 043d 0438 0435 0800 0000 0006 0000 0004  .=.8.5..........
-00004c70: 4e6f 7465 0700 0000 0e44 6976 6964 656e  Note.....Dividen
-00004c80: 6457 6964 6765 7401 0300 0000 0804 2604  dWidget.......&.
-00004c90: 3504 3d04 3008 0000 0000 0600 0000 0550  5.=.0..........P
-00004ca0: 7269 6365 0700 0000 0e44 6976 6964 656e  rice.....Dividen
-00004cb0: 6457 6964 6765 7401 0300 0000 2004 1404  dWidget..... ...
-00004cc0: 3804 3204 3804 3404 3504 3d04 3400 2004  8.2.8.4.5.=.4. .
-00004cd0: 3004 3a04 4604 3804 4f04 3c04 3808 0000  0.:.F.8.O.<.8...
-00004ce0: 0000 0600 0000 0e53 746f 636b 2044 6976  .......Stock Div
-00004cf0: 6964 656e 6407 0000 000e 4469 7669 6465  idend.....Divide
-00004d00: 6e64 5769 6467 6574 0103 0000 001c 041f  ndWidget........
-00004d10: 0435 0440 0435 0434 0430 0447 0430 0020  .5.@.5.4.0.G.0. 
-00004d20: 0430 043a 0446 0438 0439 0800 0000 0006  .0.:.F.8.9......
-00004d30: 0000 000d 5374 6f63 6b20 5665 7374 696e  ....Stock Vestin
-00004d40: 6707 0000 000e 4469 7669 6465 6e64 5769  g.....DividendWi
-00004d50: 6467 6574 0103 0000 000a 041d 0430 043b  dget.........0.;
-00004d60: 043e 0433 0800 0000 0006 0000 0003 5461  .>.3..........Ta
-00004d70: 7807 0000 000e 4469 7669 6465 6e64 5769  x.....DividendWi
-00004d80: 6467 6574 0103 0000 0006 0422 0438 043f  dget.......".8.?
-00004d90: 0800 0000 0006 0000 0004 5479 7065 0700  ..........Type..
-00004da0: 0000 0e44 6976 6964 656e 6457 6964 6765  ...DividendWidge
-00004db0: 7401 0300 0000 b204 1d04 4304 3604 3d04  t.........C.6.=.
-00004dc0: 3e00 2004 4304 4104 4204 3004 3d04 3e04  >. .C.A.B.0.=.>.
-00004dd0: 3204 3804 4204 4c00 2004 3a04 3e04 4204  2.8.B.L. .:.>.B.
-00004de0: 3804 4004 3e04 3204 3a04 4300 2004 3104  8.@.>.2.:.C. .1.
-00004df0: 4304 3c04 3004 3304 3800 2004 3404 3b04  C.<.0.3.8. .4.;.
-00004e00: 4f00 2004 1404 3004 4204 4b00 2f04 1204  O. ...0.B.K./...
-00004e10: 4004 3504 3c04 3504 3d04 3800 2004 3404  @.5.<.5.=.8. .4.
-00004e20: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
-00004e30: 2004 4704 3504 4004 3504 3700 2004 3c04   .G.5.@.5.7. .<.
-00004e40: 3504 3d04 4e00 2004 1404 3004 3d04 3d04  5.=.N. ...0.=.=.
-00004e50: 4b04 3500 2d00 3e04 1a04 3e04 4204 3804  K.5.-.>...>.B.8.
-00004e60: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
-00004e70: 0000 4859 6f75 2073 686f 756c 6420 7365  ..HYou should se
-00004e80: 7420 7175 6f74 6520 7669 6120 4461 7461  t quote via Data
-00004e90: 2d3e 5175 6f74 6573 206d 656e 7520 666f  ->Quotes menu fo
-00004ea0: 7220 4461 7465 2f54 696d 6520 6f66 2074  r Date/Time of t
-00004eb0: 6865 2064 6976 6964 656e 6407 0000 000e  he dividend.....
-00004ec0: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
-00004ed0: 0000 0014 043d 0435 0438 0437 0432 0435  .....=.5.8.7.2.5
-00004ee0: 0441 0442 043d 043e 0800 0000 0006 0000  .A.B.=.>........
-00004ef0: 0007 756e 6b6e 6f77 6e07 0000 000e 4469  ..unknown.....Di
-00004f00: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
-00004f10: 0010 0421 0432 043e 0439 0441 0442 0432  ...!.2.>.9.A.B.2
-00004f20: 043e 0800 0000 0006 0000 0008 5072 6f70  .>..........Prop
-00004f30: 6572 7479 0700 0000 0e45 7874 7261 4461  erty.....ExtraDa
-00004f40: 7461 4d6f 6465 6c01 0300 0000 1004 1704  taModel.........
-00004f50: 3d04 3004 4704 3504 3d04 3804 3508 0000  =.0.G.5.=.8.5...
-00004f60: 0000 0600 0000 0556 616c 7565 0700 0000  .......Value....
-00004f70: 0e45 7874 7261 4461 7461 4d6f 6465 6c01  .ExtraDataModel.
-00004f80: 0300 0000 1a04 2604 3504 3d04 3d04 3004  ......&.5.=.=.0.
-00004f90: 4f00 2004 3104 4304 3c04 3004 3304 3008  O. .1.C.<.0.3.0.
-00004fa0: 0000 0000 0600 0000 0a41 7373 6574 204e  .........Asset N
-00004fb0: 616d 6507 0000 000d 486f 6c64 696e 6773  ame.....Holdings
-00004fc0: 4d6f 6465 6c01 0300 0000 1c04 1204 3004  Model.........0.
-00004fd0: 3b04 4e04 4204 3000 2f04 2104 4704 5104  ;.N.B.0./.!.G.Q.
-00004fe0: 4200 2f04 2604 1108 0000 0000 0600 0000  B./.&...........
-00004ff0: 1643 7572 7265 6e63 792f 4163 636f 756e  .Currency/Accoun
-00005000: 742f 4173 7365 7407 0000 000d 486f 6c64  t/Asset.....Hold
-00005010: 696e 6773 4d6f 6465 6c01 0300 0000 0a04  ingsModel.......
-00005020: 2d04 3a04 4104 3f00 3a08 0000 0000 0600  -.:.A.?.:.......
-00005030: 0000 0445 7870 3a07 0000 000d 486f 6c64  ...Exp:.....Hold
-00005040: 696e 6773 4d6f 6465 6c01 0300 0000 1404  ingsModel.......
-00005050: 2604 3504 3d04 3000 2004 3704 3004 3a04  &.5.=.0. .7.0.:.
-00005060: 4000 2e08 0000 0000 0600 0000 044c 6173  @............Las
-00005070: 7407 0000 000d 486f 6c64 696e 6773 4d6f  t.....HoldingsMo
-00005080: 6465 6c01 0300 0000 3404 1404 3004 4204  del.....4...0.B.
-00005090: 3000 2004 3f04 3e04 4104 3b04 3504 3404  0. .?.>.A.;.5.4.
-000050a0: 3d04 3504 3900 2004 3a04 3e04 4204 3804  =.5.9. .:.>.B.8.
-000050b0: 4004 3e04 3204 3a04 3800 3a00 2008 0000  @.>.2.:.8.:. ...
-000050c0: 0000 0600 0000 114c 6173 7420 7175 6f74  .......Last quot
-000050d0: 6520 6461 7465 3a20 0700 0000 0d48 6f6c  e date: .....Hol
-000050e0: 6469 6e67 734d 6f64 656c 0103 0000 0014  dingsModel......
-000050f0: 0426 0435 043d 0430 0020 043e 0442 043a  .&.5.=.0. .>.B.:
-00005100: 0440 002e 0800 0000 0006 0000 0004 4f70  .@............Op
-00005110: 656e 0700 0000 0d48 6f6c 6469 6e67 734d  en.....HoldingsM
-00005120: 6f64 656c 0103 0000 0006 041f 0438 0423  odel.........8.#
-00005130: 0800 0000 0006 0000 0003 502f 4c07 0000  ..........P/L...
-00005140: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
-00005150: 0300 0000 0c04 1f04 3804 2300 2c00 2000  ........8.#.,. .
-00005160: 2508 0000 0000 0600 0000 0650 2f4c 2c20  %..........P/L, 
-00005170: 2507 0000 000d 486f 6c64 696e 6773 4d6f  %.....HoldingsMo
-00005180: 6465 6c01 0300 0000 0c04 1a04 3e04 3b00  del.........>.;.
-00005190: 2d04 3204 3e08 0000 0000 0600 0000 0351  -.2.>..........Q
-000051a0: 7479 0700 0000 0d48 6f6c 6469 6e67 734d  ty.....HoldingsM
-000051b0: 6f64 656c 0103 0000 000e 0414 043e 043b  odel.........>.;
-000051c0: 044f 002c 0020 0025 0800 0000 0006 0000  .O.,. .%........
-000051d0: 0008 5368 6172 652c 2025 0700 0000 0d48  ..Share, %.....H
-000051e0: 6f6c 6469 6e67 734d 6f64 656c 0103 0000  oldingsModel....
-000051f0: 000c 041e 0446 0435 043d 043a 0430 0800  .....F.5.=.:.0..
-00005200: 0000 0006 0000 0005 5661 6c75 6507 0000  ........Value...
-00005210: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
-00005220: 0300 0000 1004 1e04 4604 3504 3d04 3a04  ........F.5.=.:.
-00005230: 3000 2c00 2008 0000 0000 0600 0000 0756  0.,. ..........V
-00005240: 616c 7565 2c20 0700 0000 0d48 6f6c 6469  alue, .....Holdi
-00005250: 6e67 734d 6f64 656c 0103 0000 0016 041f  ngsModel........
-00005260: 043e 0440 0442 0444 0435 043b 044c 0020  .>.@.B.D.5.;.L. 
-00005270: 0426 0411 0800 0000 0006 0000 0008 486f  .&............Ho
-00005280: 6c64 696e 6773 0700 0000 0e48 6f6c 6469  ldings.....Holdi
-00005290: 6e67 7352 6570 6f72 7401 0300 0000 1a04  ngsReport.......
-000052a0: 1e04 4604 3504 3d04 3804 4204 4c00 2004  ..F.5.=.8.B.L. .
-000052b0: 3d04 3004 3b04 3e04 3308 0000 0000 0600  =.0.;.>.3.......
-000052c0: 0000 0c45 7374 696d 6174 6520 7461 7807  ...Estimate tax.
-000052d0: 0000 0014 486f 6c64 696e 6773 5265 706f  ....HoldingsRepo
-000052e0: 7274 5769 6e64 6f77 0103 0000 0016 041f  rtWindow........
-000052f0: 043e 0440 0442 0444 0435 043b 044c 0020  .>.@.B.D.5.;.L. 
-00005300: 0426 0411 0800 0000 0006 0000 0008 486f  .&............Ho
-00005310: 6c64 696e 6773 0700 0000 1448 6f6c 6469  ldings.....Holdi
-00005320: 6e67 7352 6570 6f72 7457 696e 646f 7701  ngsReportWindow.
-00005330: 0300 0000 1404 1f04 3e04 4004 4204 4304  ........>.@.B.C.
-00005340: 3304 3004 3b04 3804 4f08 0000 0000 0600  3.0.;.8.O.......
-00005350: 0000 0850 6f72 7475 6761 6c07 0000 0014  ...Portugal.....
-00005360: 486f 6c64 696e 6773 5265 706f 7274 5769  HoldingsReportWi
-00005370: 6e64 6f77 0103 0000 000c 0420 043e 0441  ndow....... .>.A
-00005380: 0441 0438 044f 0800 0000 0006 0000 0006  .A.8.O..........
-00005390: 5275 7373 6961 0700 0000 1448 6f6c 6469  Russia.....Holdi
-000053a0: 6e67 7352 6570 6f72 7457 696e 646f 7701  ngsReportWindow.
-000053b0: 0300 0000 2804 1f04 3e04 3a04 3004 3704  ....(...>.:.0.7.
-000053c0: 3004 4204 4c00 2004 3304 4004 3004 4404  0.B.L. .3.@.0.D.
-000053d0: 3804 3a00 2004 4604 3504 3d04 4b08 0000  8.:. .F.5.=.K...
-000053e0: 0000 0600 0000 1053 686f 7720 5072 6963  .......Show Pric
-000053f0: 6520 4368 6172 7407 0000 0014 486f 6c64  e Chart.....Hold
-00005400: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
-00005410: 0103 0000 0022 0412 0430 043b 044e 0442  ....."...0.;.N.B
-00005420: 0430 0020 043f 0435 0440 0435 0441 0447  .0. .?.5.@.5.A.G
-00005430: 0451 0442 0430 003a 0800 0000 0006 0000  .Q.B.0.:........
-00005440: 0010 436f 6d6d 6f6e 2063 7572 7265 6e63  ..Common currenc
-00005450: 793a 0700 0000 0e48 6f6c 6469 6e67 7357  y:.....HoldingsW
-00005460: 6964 6765 7401 0300 0000 1604 1f04 3e04  idget.........>.
-00005470: 4004 4204 4404 3504 3b04 4c00 2004 2604  @.B.D.5.;.L. .&.
-00005480: 1108 0000 0000 0600 0000 0848 6f6c 6469  ...........Holdi
-00005490: 6e67 7307 0000 000e 486f 6c64 696e 6773  ngs.....Holdings
-000054a0: 5769 6467 6574 0103 0000 0018 0421 043e  Widget.......!.>
-000054b0: 0445 0440 0430 043d 0438 0442 044c 002e  .E.@.0.=.8.B.L..
-000054c0: 002e 002e 0800 0000 0006 0000 0007 5361  ..............Sa
-000054d0: 7665 2e2e 2e07 0000 000e 486f 6c64 696e  ve........Holdin
-000054e0: 6773 5769 6467 6574 0103 0000 0014 0064  gsWidget.......d
-000054f0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
-00005500: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
-00005510: 4d2f 7979 7979 0700 0000 0e48 6f6c 6469  M/yyyy.....Holdi
-00005520: 6e67 7357 6964 6765 7401 0300 0000 3404  ngsWidget.....4.
-00005530: 2204 3804 3f00 2004 2604 1100 2004 3d04  ".8.?. .&... .=.
-00005540: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
-00005550: 3604 3804 3204 3004 3504 4204 4104 4f00  6.8.2.0.5.B.A.O.
-00005560: 3a00 2008 0000 0000 0600 0000 1c41 7373  :. ..........Ass
-00005570: 6574 2074 7970 6520 6973 6e27 7420 7375  et type isn't su
-00005580: 7070 6f72 7465 643a 2007 0000 0004 4942  pported: .....IB
-00005590: 4b52 0103 0000 0054 041a 043e 0440 043f  KR.....T...>.@.?
-000055a0: 043e 0440 0430 0442 0438 0432 043d 043e  .>.@.0.B.8.2.=.>
-000055b0: 0435 0020 0434 0435 0439 0441 0442 0432  .5. .4.5.9.A.B.2
-000055c0: 0438 0435 0020 043d 0435 0020 043f 043e  .8.5. .=.5. .?.>
-000055d0: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-000055e0: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
-000055f0: 0006 0000 0022 436f 7270 6f72 6174 6520  ....."Corporate 
-00005600: 6163 7469 6f6e 2069 736e 2774 2073 7570  action isn't sup
-00005610: 706f 7274 6564 3a20 0700 0000 0449 424b  ported: .....IBK
-00005620: 5201 0300 0000 4604 1d04 3504 3e04 3404  R.....F...5.>.4.
-00005630: 3d04 3e04 3704 3d04 3004 4704 3d04 3e04  =.>.7.=.0.G.=.>.
-00005640: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
-00005650: 3504 3d04 3804 3500 2004 4104 4704 5104  5.=.8.5. .A.G.Q.
-00005660: 4204 3000 2004 3404 3b04 4f00 2008 0000  B.0. .4.;.O. ...
-00005670: 0000 0600 0000 1b4d 756c 7469 706c 6520  .......Multiple 
-00005680: 6163 636f 756e 7420 6d61 7463 6820 666f  account match fo
-00005690: 7220 0700 0000 0449 424b 5201 0300 0000  r .....IBKR.....
-000056a0: 6800 4a00 5300 4f00 4e00 2004 4204 4d04  h.J.S.O.N. .B.M.
-000056b0: 3300 2000 2700 6400 6f00 6300 7500 6d00  3. .'.d.o.c.u.m.
-000056c0: 6500 6e00 7400 2700 2004 3e04 4204 4104  e.n.t.'. .>.B.A.
-000056d0: 4304 4204 4104 4204 3204 4304 3504 4200  C.B.A.B.2.C.5.B.
-000056e0: 2004 3204 3d04 4304 4204 4004 3800 2004   .2.=.C.B.@.8. .
-000056f0: 4204 4d04 3304 3000 2000 2700 7400 6900  B.M.3.0. .'.t.i.
-00005700: 6300 6b00 6500 7400 2708 0000 0000 0600  c.k.e.t.'.......
-00005710: 0000 2a43 616e 2774 2066 696e 6420 2764  ..*Can't find 'd
-00005720: 6f63 756d 656e 7427 2074 6167 2069 6e20  ocument' tag in 
-00005730: 6a73 6f6e 2027 7469 636b 6574 2707 0000  json 'ticket'...
-00005740: 0010 496d 706f 7274 536c 6970 4469 616c  ..ImportSlipDial
-00005750: 6f67 0103 0000 0072 004a 0053 004f 004e  og.....r.J.S.O.N
-00005760: 0020 0442 044d 0433 0020 0027 006f 0070  . .B.M.3. .'.o.p
-00005770: 0065 0072 0061 0074 0069 006f 006e 0054  .e.r.a.t.i.o.n.T
-00005780: 0079 0070 0065 0027 0020 043e 0442 0441  .y.p.e.'. .>.B.A
-00005790: 0443 0442 0441 0442 0432 0443 0435 0442  .C.B.A.B.2.C.5.B
-000057a0: 0020 0432 043d 0443 0442 0440 0438 0020  . .2.=.C.B.@.8. 
-000057b0: 0442 044d 0433 0430 0020 0027 0074 0069  .B.M.3.0. .'.t.i
-000057c0: 0063 006b 0065 0074 0027 0800 0000 0006  .c.k.e.t.'......
-000057d0: 0000 002f 4361 6e27 7420 6669 6e64 2027  .../Can't find '
-000057e0: 6f70 6572 6174 696f 6e54 7970 6527 2074  operationType' t
-000057f0: 6167 2069 6e20 6a73 6f6e 2027 7469 636b  ag in json 'tick
-00005800: 6574 2707 0000 0010 496d 706f 7274 536c  et'.....ImportSl
-00005810: 6970 4469 616c 6f67 0103 0000 006a 004a  ipDialog.....j.J
-00005820: 0053 004f 004e 0020 0442 044d 0433 0020  .S.O.N. .B.M.3. 
-00005830: 0027 0072 0065 0063 0065 0069 0070 0074  .'.r.e.c.e.i.p.t
-00005840: 0027 0020 043e 0442 0441 0443 0442 0441  .'. .>.B.A.C.B.A
-00005850: 0442 0432 0443 0435 0442 0020 0432 043d  .B.2.C.5.B. .2.=
-00005860: 0443 0442 0440 0438 0020 0442 044d 0433  .C.B.@.8. .B.M.3
-00005870: 0430 0020 0027 0064 006f 0063 0075 006d  .0. .'.d.o.c.u.m
-00005880: 0065 006e 0074 0027 0800 0000 0006 0000  .e.n.t.'........
-00005890: 002b 4361 6e27 7420 6669 6e64 2027 7265  .+Can't find 're
-000058a0: 6365 6970 7427 2074 6167 2069 6e20 6a73  ceipt' tag in js
-000058b0: 6f6e 2027 646f 6375 6d65 6e74 2707 0000  on 'document'...
-000058c0: 0010 496d 706f 7274 536c 6970 4469 616c  ..ImportSlipDial
-000058d0: 6f67 0103 0000 005e 041a 0430 0442 0435  og.....^...0.B.5
-000058e0: 0433 043e 0440 0438 0438 0020 043d 0435  .3.>.@.8.8. .=.5
-000058f0: 0020 0440 0430 0441 043f 043e 0437 043d  . .@.0.A.?.>.7.=
-00005900: 0430 043d 044b 003a 0020 0054 0065 006e  .0.=.K.:. .T.e.n
-00005910: 0073 006f 0072 006c 006f 0077 0020 043d  .s.o.r.l.o.w. .=
-00005920: 0435 0020 043e 0431 043d 0430 0440 0443  .5. .>.1.=.0.@.C
-00005930: 0436 0435 043d 0800 0000 0006 0000 0036  .6.5.=.........6
-00005940: 4361 7465 676f 7269 6573 2061 7265 206e  Categories are n
-00005950: 6f74 2072 6563 6f67 6e69 7a65 643a 2054  ot recognized: T
-00005960: 656e 736f 7266 6c6f 7720 6973 206e 6f74  ensorflow is not
-00005970: 2066 6f75 6e64 0700 0000 1049 6d70 6f72   found.....Impor
-00005980: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
-00005990: 4a04 1f04 4004 3504 3204 4b04 4804 3504  J...@.5.2.K.H.5.
-000059a0: 3d04 3e00 2004 3c04 3004 3a04 4104 3804  =.>. .<.0.:.A.8.
-000059b0: 3c04 3004 3b04 4c04 3d04 3e04 3500 2004  <.0.;.L.=.>.5. .
-000059c0: 4704 3804 4104 3b04 3e00 2004 3f04 3e04  G.8.A.;.>. .?.>.
-000059d0: 3f04 4b04 4204 3e04 3a00 2e08 0000 0000  ?.K.B.>.:.......
-000059e0: 0600 0000 194d 6178 2072 6574 7279 2063  .....Max retry c
-000059f0: 6f75 6e74 2065 7863 6565 6465 642e 0700  ount exceeded...
-00005a00: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
-00005a10: 6c6f 6701 0300 0000 4600 5100 5200 2004  log.....F.Q.R. .
-00005a20: 3a04 3e04 3400 2004 3d04 3500 2004 3e04  :.>.4. .=.5. .>.
-00005a30: 3104 3d04 3004 4004 4304 3604 3504 3d00  1.=.0.@.C.6.5.=.
-00005a40: 2004 3200 2004 3104 4304 4404 3504 4004   .2. .1.C.D.5.@.
-00005a50: 3500 2004 3e04 3104 3c04 3504 3d04 3008  5. .>.1.<.5.=.0.
-00005a60: 0000 0000 0600 0000 1e4e 6f20 5152 2063  .........No QR c
-00005a70: 6f64 6573 2066 6f75 6e64 2069 6e20 636c  odes found in cl
-00005a80: 6970 626f 6172 6407 0000 0010 496d 706f  ipboard.....Impo
-00005a90: 7274 536c 6970 4469 616c 6f67 0103 0000  rtSlipDialog....
-00005aa0: 0036 0051 0052 002d 043a 043e 0434 0020  .6.Q.R.-.:.>.4. 
-00005ab0: 0432 0020 0444 0430 0439 043b 0435 0020  .2. .D.0.9.;.5. 
-00005ac0: 043d 0435 0020 043e 0431 043d 0430 0440  .=.5. .>.1.=.0.@
-00005ad0: 0443 0436 0435 043d 0800 0000 0006 0000  .C.6.5.=........
-00005ae0: 001e 4e6f 2051 5220 636f 6465 7320 7765  ..No QR codes we
-00005af0: 7265 2066 6f75 6e64 2069 6e20 6669 6c65  re found in file
-00005b00: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005b10: 6961 6c6f 6701 0300 0000 7204 1d04 3504  ialog.....r...5.
-00005b20: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-00005b30: 2004 3404 3e04 3104 3004 3204 3804 4204   .4.>.1.0.2.8.B.
-00005b40: 4c00 2004 4704 3504 3a00 3a00 2004 3d04  L. .G.5.:.:. .=.
-00005b50: 3500 2004 4304 3a04 3004 3704 3004 3d00  5. .C.:.0.7.0.=.
-00005b60: 2004 3a04 3e04 3d04 4204 4004 3004 3304   .:.>.=.B.@.0.3.
-00005b70: 3504 3d04 4200 2004 3404 3b04 4f00 2004  5.=.B. .4.;.O. .
-00005b80: 3804 3c04 3f04 3e04 4004 4204 3008 0000  8.<.?.>.@.B.0...
-00005b90: 0000 0600 0000 414e 6f74 2070 6f73 7369  ......ANot possi
-00005ba0: 626c 6520 746f 2069 6d70 6f72 7420 736c  ble to import sl
-00005bb0: 6970 3a20 6361 6e27 7420 696d 706f 7274  ip: can't import
-00005bc0: 3a20 6e6f 2070 6565 7220 7365 7420 666f  : no peer set fo
-00005bd0: 7220 696d 706f 7274 0700 0000 1049 6d70  r import.....Imp
-00005be0: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
-00005bf0: 0000 6604 1d04 3504 3204 3e04 3704 3c04  ..f...5.2.>.7.<.
-00005c00: 3e04 3604 3d04 3e00 2004 3404 3e04 3104  >.6.=.>. .4.>.1.
-00005c10: 3004 3204 3804 4204 4c00 2004 4704 3504  0.2.8.B.L. .G.5.
-00005c20: 3a00 3a00 2004 3d04 3500 2004 4304 3a04  :.:. .=.5. .C.:.
-00005c30: 3004 3704 3004 3d00 2004 4104 4704 3504  0.7.0.=. .A.G.5.
-00005c40: 4200 2004 3404 3b04 4f00 2004 3804 3c04  B. .4.;.O. .8.<.
-00005c50: 3f04 3e04 4004 4204 3008 0000 0000 0600  ?.>.@.B.0.......
-00005c60: 0000 364e 6f74 2070 6f73 7369 626c 6520  ..6Not possible 
-00005c70: 746f 2069 6d70 6f72 7420 736c 6970 3a20  to import slip: 
-00005c80: 6e6f 2061 6363 6f75 6e74 2073 6574 2066  no account set f
-00005c90: 6f72 2069 6d70 6f72 7407 0000 0010 496d  or import.....Im
-00005ca0: 706f 7274 536c 6970 4469 616c 6f67 0103  portSlipDialog..
-00005cb0: 0000 0078 041d 0435 0432 043e 0437 043c  ...x...5.2.>.7.<
-00005cc0: 043e 0436 043d 043e 0020 0434 043e 0431  .>.6.=.>. .4.>.1
-00005cd0: 0430 0432 0438 0442 044c 0020 0447 0435  .0.2.8.B.L. .G.5
-00005ce0: 043a 003a 0020 043a 0430 0442 0435 0433  .:.:. .:.0.B.5.3
-00005cf0: 043e 0440 0438 0438 0020 0443 043a 0430  .>.@.8.8. .C.:.0
-00005d00: 0437 0430 043d 044b 0020 043d 0435 0020  .7.0.=.K. .=.5. 
-00005d10: 0434 043b 044f 0020 0432 0441 0435 0445  .4.;.O. .2.A.5.E
-00005d20: 0020 0441 0442 0440 043e 043a 0800 0000  . .A.B.@.>.:....
-00005d30: 0006 0000 0038 4e6f 7420 706f 7373 6962  .....8Not possib
-00005d40: 6c65 2074 6f20 696d 706f 7274 2073 6c69  le to import sli
-00005d50: 703a 2073 6f6d 6520 6361 7465 676f 7269  p: some categori
-00005d60: 6573 2061 7265 206e 6f74 2073 6574 0700  es are not set..
-00005d70: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
-00005d80: 6c6f 6701 0300 0000 5404 1d04 3504 3204  log.....T...5.2.
-00005d90: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-00005da0: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
-00005db0: 4204 4c00 2004 3f04 4004 3e04 4704 3804  B.L. .?.@.>.G.8.
-00005dc0: 4204 3004 3d04 3d04 4b04 3900 2000 5100  B.0.=.=.K.9. .Q.
-00005dd0: 5200 2d04 3a04 3e04 3400 3a00 2008 0000  R.-.:.>.4.:. ...
-00005de0: 0000 0600 0000 2b51 5220 6176 6169 6c61  ......+QR availa
-00005df0: 626c 6520 6275 7420 7061 7474 6572 6e20  ble but pattern 
-00005e00: 6973 6e27 7420 7265 636f 676e 697a 6564  isn't recognized
-00005e10: 3a20 0700 0000 1049 6d70 6f72 7453 6c69  : .....ImportSli
-00005e20: 7044 6961 6c6f 6701 0300 0000 0800 5100  pDialog.......Q.
-00005e30: 5200 3a00 2008 0000 0000 0600 0000 0451  R.:. ..........Q
-00005e40: 523a 2007 0000 0010 496d 706f 7274 536c  R: .....ImportSl
-00005e50: 6970 4469 616c 6f67 0103 0000 0030 0412  ipDialog.....0..
-00005e60: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
-00005e70: 0444 0430 0439 043b 0020 0441 0020 0051  .D.0.9.;. .A. .Q
-00005e80: 0052 002d 043a 043e 0434 043e 043c 0800  .R.-.:.>.4.>.<..
-00005e90: 0000 0006 0000 0018 5365 6c65 6374 2066  ........Select f
-00005ea0: 696c 6520 7769 7468 2051 5220 636f 6465  ile with QR code
-00005eb0: 0700 0000 1049 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00005ec0: 6961 6c6f 6701 0300 0000 4204 1204 4b04  ialog.....B...K.
-00005ed0: 3104 3504 4004 3804 4204 3500 2004 4404  1.5.@.8.B.5. .D.
-00005ee0: 3004 3904 3b00 2004 4100 2000 4a00 5300  0.9.;. .A. .J.S.
-00005ef0: 4f00 4e00 2d04 3404 3004 3d04 3d04 4b04  O.N.-.4.0.=.=.K.
-00005f00: 3c04 3800 2004 4704 3504 3a04 3008 0000  <.8. .G.5.:.0...
-00005f10: 0000 0600 0000 1f53 656c 6563 7420 6669  .......Select fi
-00005f20: 6c65 2077 6974 6820 736c 6970 204a 534f  le with slip JSO
-00005f30: 4e20 6461 7461 0700 0000 1049 6d70 6f72  N data.....Impor
-00005f40: 7453 6c69 7044 6961 6c6f 6701 0300 0000  tSlipDialog.....
-00005f50: 3204 1d04 3504 3804 3704 3204 3504 4104  2...5.8.7.2.5.A.
-00005f60: 4204 3d04 4b04 3900 2004 4204 3804 3f00  B.=.K.9. .B.8.?.
-00005f70: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-00005f80: 3800 2008 0000 0000 0600 0000 1755 6e6b  8. ..........Unk
-00005f90: 6e6f 776e 206f 7065 7261 7469 6f6e 2074  nown operation t
-00005fa0: 7970 6520 0700 0000 1049 6d70 6f72 7453  ype .....ImportS
-00005fb0: 6c69 7044 6961 6c6f 6701 0300 0000 0600  lipDialog.......
-00005fc0: 2027 9c00 2008 0000 0000 0600 0000 0520   '.. .......... 
-00005fd0: e29e 9c20 0700 0000 0d49 6d70 6f72 7453  ... .....ImportS
-00005fe0: 6c69 7044 6c67 0103 0000 000a 0421 0447  lipDlg.......!.G
-00005ff0: 0435 0442 003a 0800 0000 0006 0000 0008  .5.B.:..........
-00006000: 4163 636f 756e 743a 0700 0000 0d49 6d70  Account:.....Imp
-00006010: 6f72 7453 6c69 7044 6c67 0103 0000 0010  ortSlipDlg......
-00006020: 0414 043e 0431 0430 0432 0438 0442 044c  ...>.1.0.2.8.B.L
-00006030: 0800 0000 0006 0000 0003 4164 6407 0000  ..........Add...
-00006040: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-00006050: 0300 0000 0c04 2104 4304 3c04 3c04 3000  ......!.C.<.<.0.
-00006060: 3a08 0000 0000 0600 0000 0741 6d6f 756e  :..........Amoun
-00006070: 743a 0700 0000 0d49 6d70 6f72 7453 6c69  t:.....ImportSli
-00006080: 7044 6c67 0103 0000 0032 0410 0432 0442  pDlg.....2...2.B
-00006090: 043e 002d 043d 0430 0437 043d 0430 0447  .>.-.=.0.7.=.0.G
-000060a0: 0435 043d 0438 0435 0020 043a 0430 0442  .5.=.8.5. .:.0.B
-000060b0: 0435 0433 043e 0440 0438 0439 0800 0000  .5.3.>.@.8.9....
-000060c0: 0006 0000 0016 4175 746f 2d61 7373 6967  ......Auto-assig
-000060d0: 6e20 6361 7465 676f 7269 6573 0700 0000  n categories....
-000060e0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-000060f0: 0000 000c 041a 0430 043c 0435 0440 0430  .......0.<.5.@.0
-00006100: 0800 0000 0006 0000 0006 4361 6d65 7261  ..........Camera
-00006110: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00006120: 6c67 0103 0000 0010 041e 0447 0438 0441  lg.........G.8.A
-00006130: 0442 0438 0442 044c 0800 0000 0006 0000  .B.8.B.L........
-00006140: 0005 436c 6561 7207 0000 000d 496d 706f  ..Clear.....Impo
-00006150: 7274 536c 6970 446c 6701 0300 0000 0e04  rtSlipDlg.......
-00006160: 1704 3004 3a04 4004 4b04 4204 4c08 0000  ..0.:.@.K.B.L...
-00006170: 0000 0600 0000 0543 6c6f 7365 0700 0000  .......Close....
-00006180: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006190: 0000 001a 0414 0430 0442 0430 0020 002f  .......0.B.0. ./
-000061a0: 0020 0412 0440 0435 043c 044f 003a 0800  . ...@.5.<.O.:..
-000061b0: 0000 0006 0000 000c 4461 7465 202f 2054  ........Date / T
-000061c0: 696d 653a 0700 0000 0d49 6d70 6f72 7453  ime:.....ImportS
-000061d0: 6c69 7044 6c67 0103 0000 0016 0414 0430  lipDlg.........0
-000061e0: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
-000061f0: 003a 0800 0000 0006 0000 000a 4461 7465  .:..........Date
-00006200: 2f54 696d 653a 0700 0000 0d49 6d70 6f72  /Time:.....Impor
-00006210: 7453 6c69 7044 6c67 0103 0000 0006 0424  tSlipDlg.......$
-00006220: 0414 003a 0800 0000 0006 0000 0003 4644  ...:..........FD
-00006230: 3a07 0000 000d 496d 706f 7274 536c 6970  :.....ImportSlip
-00006240: 446c 6701 0300 0000 0604 2404 1d00 3a08  Dlg.......$...:.
-00006250: 0000 0000 0600 0000 0346 4e3a 0700 0000  .........FN:....
-00006260: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006270: 0000 0006 0424 041f 003a 0800 0000 0006  .....$...:......
-00006280: 0000 0003 4650 3a07 0000 000d 496d 706f  ....FP:.....Impo
-00006290: 7274 536c 6970 446c 6701 0300 0000 2604  rtSlipDlg.....&.
-000062a0: 2104 3a04 3004 3d04 3804 4004 3e04 3204  !.:.0.=.8.@.>.2.
-000062b0: 3004 4204 4c00 2004 3a04 3004 3c04 3504  0.B.L. .:.0.<.5.
-000062c0: 4004 3e04 3908 0000 0000 0600 0000 0f47  @.>.9..........G
-000062d0: 6574 2066 726f 6d20 6361 6d65 7261 0700  et from camera..
-000062e0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-000062f0: 0103 0000 0024 041f 043e 043b 0443 0447  .....$...>.;.C.G
-00006300: 0438 0442 044c 0020 0438 0437 0020 0431  .8.B.L. .8.7. .1
-00006310: 0443 0444 0435 0440 0430 0800 0000 0006  .C.D.5.@.0......
-00006320: 0000 0012 4765 7420 6672 6f6d 2063 6c69  ....Get from cli
-00006330: 7062 6f61 7264 0700 0000 0d49 6d70 6f72  pboard.....Impor
-00006340: 7453 6c69 7044 6c67 0103 0000 0030 041f  tSlipDlg.....0..
-00006350: 043e 043b 0443 0447 0438 0442 044c 0020  .>.;.C.G.8.B.L. 
-00006360: 0447 0435 043a 0020 0441 0020 0441 0430  .G.5.:. .A. .A.0
-00006370: 0439 0442 0430 0020 0424 041d 0421 0800  .9.B.0. .$...!..
-00006380: 0000 0006 0000 0016 4765 7420 736c 6970  ........Get slip
-00006390: 2066 726f 6d20 696e 7465 726e 6574 0700   from internet..
-000063a0: 0000 0d49 6d70 6f72 7453 6c69 7044 6c67  ...ImportSlipDlg
-000063b0: 0103 0000 0016 0418 043c 043f 043e 0440  .........<.?.>.@
-000063c0: 0442 0020 0447 0435 043a 0430 0800 0000  .B. .G.5.:.0....
-000063d0: 0006 0000 000b 496d 706f 7274 2053 6c69  ......Import Sli
-000063e0: 7007 0000 000d 496d 706f 7274 536c 6970  p.....ImportSlip
-000063f0: 446c 6701 0300 0000 0e04 2104 4204 4004  Dlg.......!.B.@.
-00006400: 3e04 3a04 3800 3a08 0000 0000 0600 0000  >.:.8.:.........
-00006410: 064c 696e 6573 3a07 0000 000d 496d 706f  .Lines:.....Impo
-00006420: 7274 536c 6970 446c 6701 0300 0000 2404  rtSlipDlg.....$.
-00006430: 1704 3004 3304 4004 4304 3704 3804 4204  ..0.3.@.C.7.8.B.
-00006440: 4c00 2004 3804 3700 2004 4404 3004 3904  L. .8.7. .D.0.9.
-00006450: 3b04 3008 0000 0000 0600 0000 0e4c 6f61  ;.0..........Loa
-00006460: 6420 6672 6f6d 2066 696c 6507 0000 000d  d from file.....
-00006470: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
-00006480: 0000 3604 1704 3004 3304 4304 3704 3804  ..6...0.3.C.7.8.
-00006490: 4204 4c00 2004 4704 3504 3a04 3000 2004  B.L. .G.5.:.0. .
-000064a0: 3804 3700 2000 4a00 5300 4f00 4e00 2d04  8.7. .J.S.O.N.-.
-000064b0: 4404 3004 3904 3b04 3008 0000 0000 0600  D.0.9.;.0.......
-000064c0: 0000 184c 6f61 6420 736c 6970 2066 726f  ...Load slip fro
-000064d0: 6d20 4a53 4f4e 2066 696c 6507 0000 000d  m JSON file.....
-000064e0: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
-000064f0: 0000 1604 1a04 3e04 3d04 4204 4004 3004  ......>.=.B.@.0.
-00006500: 3304 3504 3d04 4200 3a08 0000 0000 0600  3.5.=.B.:.......
-00006510: 0000 0550 6565 723a 0700 0000 0d49 6d70  ...Peer:.....Imp
-00006520: 6f72 7453 6c69 7044 6c67 0103 0000 000e  ortSlipDlg......
-00006530: 041f 043e 043a 0443 043f 043a 0430 0800  ...>.:.C.?.:.0..
-00006540: 0000 0006 0000 0008 5075 7263 6861 7365  ........Purchase
-00006550: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00006560: 6c67 0103 0000 000c 0051 0052 002d 043a  lg.......Q.R.-.:
-00006570: 043e 0434 0800 0000 0006 0000 0007 5152  .>.4..........QR
-00006580: 2d63 6f64 6507 0000 000d 496d 706f 7274  -code.....Import
-00006590: 536c 6970 446c 6701 0300 0000 0e04 1204  SlipDlg.........
-000065a0: 3e04 3704 3204 4004 3004 4208 0000 0000  >.7.2.@.0.B.....
-000065b0: 0600 0000 0652 6574 7572 6e07 0000 000d  .....Return.....
-000065c0: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
-000065d0: 0000 2e04 2304 4104 4204 3004 3d04 3e04  ....#.A.B.0.=.>.
-000065e0: 3204 3804 4204 4c00 2004 4204 4d04 3300  2.8.B.L. .B.M.3.
-000065f0: 2004 3404 3b04 4f00 2004 3204 4104 3504   .4.;.O. .2.A.5.
-00006600: 4508 0000 0000 0600 0000 1553 6574 2054  E..........Set T
-00006610: 6167 2066 6f72 2061 6c6c 206c 696e 6573  ag for all lines
-00006620: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00006630: 6c67 0103 0000 0006 0427 0435 043a 0800  lg.......'.5.:..
-00006640: 0000 0006 0000 0004 536c 6970 0700 0000  ........Slip....
-00006650: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
-00006660: 0000 0016 0414 0430 043d 043d 044b 0435  .......0.=.=.K.5
-00006670: 0020 0447 0435 043a 0430 0800 0000 0006  . .G.5.:.0......
-00006680: 0000 0009 536c 6970 2064 6174 6107 0000  ....Slip data...
-00006690: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
-000066a0: 0300 0000 1c04 1704 3004 3a04 4004 4b04  ........0.:.@.K.
-000066b0: 4204 4c00 2004 3a04 3004 3c04 3504 4004  B.L. .:.0.<.5.@.
-000066c0: 4308 0000 0000 0600 0000 0b53 746f 7020  C..........Stop 
-000066d0: 6361 6d65 7261 0700 0000 0d49 6d70 6f72  camera.....Impor
-000066e0: 7453 6c69 7044 6c67 0103 0000 0008 0422  tSlipDlg......."
-000066f0: 0438 043f 003a 0800 0000 0006 0000 0005  .8.?.:..........
-00006700: 5479 7065 3a07 0000 000d 496d 706f 7274  Type:.....Import
-00006710: 536c 6970 446c 6701 0300 0000 2600 6400  SlipDlg.....&.d.
-00006720: 6400 2f00 4d00 4d00 2f00 7900 7900 7900  d./.M.M./.y.y.y.
-00006730: 7900 2000 6800 6800 3a00 6d00 6d00 3a00  y. .h.h.:.m.m.:.
-00006740: 7300 7308 0000 0000 0600 0000 1364 642f  s.s..........dd/
-00006750: 4d4d 2f79 7979 7920 6868 3a6d 6d3a 7373  MM/yyyy hh:mm:ss
-00006760: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
-00006770: 6c67 0103 0000 0066 041d 0435 0432 043e  lg.....f...5.2.>
-00006780: 0437 043c 043e 0436 043d 043e 0020 043e  .7.<.>.6.=.>. .>
-00006790: 0431 0440 0430 0431 043e 0442 0430 0442  .1.@.0.1.>.B.0.B
-000067a0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
-000067b0: 0438 044e 0020 0431 0435 0437 0020 0434  .8.N. .1.5.7. .4
-000067c0: 0435 0442 0430 043b 044c 043d 044b 0445  .5.B.0.;.L.=.K.E
-000067d0: 0020 0434 0430 043d 043d 044b 0445 0800  . .4.0.=.=.K.E..
-000067e0: 0000 0006 0000 0027 4361 6e27 7420 7072  .......'Can't pr
-000067f0: 6f63 6573 7320 6f70 6572 6174 696f 6e20  ocess operation 
-00006800: 7769 7468 6f75 7420 6465 7461 696c 7307  without details.
-00006810: 0000 000e 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006820: 6e67 0103 0000 000c 041a 0443 0440 0441  ng.........C.@.A
-00006830: 003a 0020 0800 0000 0006 0000 0006 5261  .:. ..........Ra
-00006840: 7465 3a20 0700 0000 0e49 6e63 6f6d 6553  te: .....IncomeS
-00006850: 7065 6e64 696e 6701 0300 0000 1c04 1404  pending.........
-00006860: 3e04 4504 3e04 3404 4b00 2004 3800 2004  >.E.>.4.K. .8. .
-00006870: 2204 4004 3004 4204 4b08 0000 0000 0600  ".@.0.B.K.......
-00006880: 0000 1149 6e63 6f6d 6520 2620 5370 656e  ...Income & Spen
-00006890: 6469 6e67 0700 0000 1449 6e63 6f6d 6553  ding.....IncomeS
-000068a0: 7065 6e64 696e 6752 6570 6f72 7401 0300  pendingReport...
-000068b0: 0000 0a04 1804 2204 1e04 1304 1e08 0000  ......".........
-000068c0: 0000 0600 0000 0554 4f54 414c 0700 0000  .......TOTAL....
-000068d0: 1949 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-000068e0: 6570 6f72 744d 6f64 656c 0103 0000 000e  eportModel......
-000068f0: 0412 0430 043b 044e 0442 0430 003a 0800  ...0.;.N.B.0.:..
-00006900: 0000 0006 0000 0009 4375 7272 656e 6379  ........Currency
-00006910: 3a07 0000 001a 496e 636f 6d65 5370 656e  :.....IncomeSpen
-00006920: 6469 6e67 5265 706f 7274 5769 6467 6574  dingReportWidget
-00006930: 0103 0000 001c 0414 043e 0445 043e 0434  .........>.E.>.4
-00006940: 044b 0020 0438 0020 0422 0440 0430 0442  .K. .8. .".@.0.B
-00006950: 044b 0800 0000 0006 0000 0011 496e 636f  .K..........Inco
-00006960: 6d65 2026 2053 7065 6e64 696e 6707 0000  me & Spending...
-00006970: 001a 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006980: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
-00006990: 0012 041f 043e 043c 0435 0441 044f 0447  .....>.<.5.A.O.G
-000069a0: 043d 043e 0800 0000 0006 0000 0007 4d6f  .=.>..........Mo
-000069b0: 6e74 686c 7907 0000 001a 496e 636f 6d65  nthly.....Income
-000069c0: 5370 656e 6469 6e67 5265 706f 7274 5769  SpendingReportWi
-000069d0: 6467 6574 0103 0000 001c 041f 0435 0440  dget.........5.@
-000069e0: 0438 043e 0434 0438 0447 043d 043e 0441  .8.>.4.8.G.=.>.A
-000069f0: 0442 044c 003a 0800 0000 0006 0000 000c  .B.L.:..........
-00006a00: 5065 7269 6f64 6963 6974 793a 0700 0000  Periodicity:....
-00006a10: 1a49 6e63 6f6d 6553 7065 6e64 696e 6752  .IncomeSpendingR
-00006a20: 6570 6f72 7457 6964 6765 7401 0300 0000  eportWidget.....
-00006a30: 1804 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
-00006a40: 4204 4c00 2e00 2e00 2e08 0000 0000 0600  B.L.............
-00006a50: 0000 0753 6176 652e 2e2e 0700 0000 1a49  ...Save........I
-00006a60: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
-00006a70: 6f72 7457 6964 6765 7401 0300 0000 1404  ortWidget.......
-00006a80: 1f04 3e04 3d04 3504 3404 3504 3b04 4c04  ..>.=.5.4.5.;.L.
-00006a90: 3d04 3e08 0000 0000 0600 0000 0657 6565  =.>..........Wee
-00006aa0: 6b6c 7907 0000 001a 496e 636f 6d65 5370  kly.....IncomeSp
-00006ab0: 656e 6469 6e67 5265 706f 7274 5769 6467  endingReportWidg
-00006ac0: 6574 0103 0000 001c 0414 043e 0445 043e  et.........>.E.>
-00006ad0: 0434 044b 0020 0438 0020 0422 0440 0430  .4.K. .8. .".@.0
-00006ae0: 0442 044b 0800 0000 0006 0000 0011 496e  .B.K..........In
-00006af0: 636f 6d65 2026 2053 7065 6e64 696e 6707  come & Spending.
-00006b00: 0000 001a 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006b10: 6e67 5265 706f 7274 5769 6e64 6f77 0103  ngReportWindow..
-00006b20: 0000 0022 041f 043e 043a 0430 0437 0430  ..."...>.:.0.7.0
-00006b30: 0442 044c 0020 043e 043f 0435 0440 0430  .B.L. .>.?.5.@.0
-00006b40: 0446 0438 0438 0800 0000 0006 0000 000f  .F.8.8..........
-00006b50: 5368 6f77 206f 7065 7261 7469 6f6e 7307  Show operations.
-00006b60: 0000 001a 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
-00006b70: 6e67 5265 706f 7274 5769 6e64 6f77 0103  ngReportWindow..
-00006b80: 0000 0008 0421 0447 0435 0442 0800 0000  .....!.G.5.B....
-00006b90: 0006 0000 0007 4163 636f 756e 7407 0000  ......Account...
-00006ba0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006bb0: 5769 6467 6574 0103 0000 0032 0414 043e  Widget.....2...>
-00006bc0: 0431 0430 0432 0438 0442 044c 0020 0434  .1.0.2.8.B.L. .4
-00006bd0: 0435 0442 0430 043b 044c 043d 0443 044e  .5.B.0.;.L.=.C.N
-00006be0: 0020 0437 0430 043f 0438 0441 044c 0800  . .7.0.?.8.A.L..
-00006bf0: 0000 0006 0000 000a 4164 6420 6465 7461  ........Add deta
-00006c00: 696c 0700 0000 1449 6e63 6f6d 6553 7065  il.....IncomeSpe
-00006c10: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
-00006c20: 3804 2104 3a04 3e04 3f04 3804 4004 3e04  8.!.:.>.?.8.@.>.
-00006c30: 3204 3004 4204 4c00 2004 3404 3504 4204  2.0.B.L. .4.5.B.
-00006c40: 3004 3b04 4c04 3d04 4304 4e00 2004 3704  0.;.L.=.C.N. .7.
-00006c50: 3004 3f04 3804 4104 4c08 0000 0000 0600  0.?.8.A.L.......
-00006c60: 0000 0b43 6f70 7920 6465 7461 696c 0700  ...Copy detail..
-00006c70: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
-00006c80: 6757 6964 6765 7401 0300 0000 1404 1404  gWidget.........
-00006c90: 3004 4204 3000 2f04 1204 4004 3504 3c04  0.B.0./...@.5.<.
-00006ca0: 4f08 0000 0000 0600 0000 0944 6174 652f  O..........Date/
-00006cb0: 5469 6d65 0700 0000 1449 6e63 6f6d 6553  Time.....IncomeS
-00006cc0: 7065 6e64 696e 6757 6964 6765 7401 0300  pendingWidget...
-00006cd0: 0000 0c04 1404 3504 4204 3004 3b04 3808  ......5.B.0.;.8.
-00006ce0: 0000 0000 0600 0000 0744 6574 6169 6c73  .........Details
-00006cf0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00006d00: 696e 6757 6964 6765 7401 0300 0000 4404  ingWidget.....D.
-00006d10: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00006d20: 3d04 3e00 2004 3404 3e04 3104 3004 3204  =.>. .4.>.1.0.2.
-00006d30: 3804 4204 4c00 2004 3d04 3e04 3204 4304  8.B.L. .=.>.2.C.
-00006d40: 4e00 2004 3704 3004 3f04 3804 4104 4c00  N. .7.0.?.8.A.L.
-00006d50: 3a00 2008 0000 0000 0600 0000 1a46 6169  :. ..........Fai
-00006d60: 6c65 6420 746f 2061 6464 206e 6577 2072  led to add new r
-00006d70: 6563 6f72 643a 2007 0000 0014 496e 636f  ecord: .....Inco
-00006d80: 6d65 5370 656e 6469 6e67 5769 6467 6574  meSpendingWidget
-00006d90: 0103 0000 001c 0414 043e 0445 043e 0434  .........>.E.>.4
-00006da0: 0020 002f 0020 0420 0430 0441 0445 043e  . ./. . .0.A.E.>
-00006db0: 0434 0800 0000 0006 0000 0011 496e 636f  .4..........Inco
-00006dc0: 6d65 202f 2053 7065 6e64 696e 6707 0000  me / Spending...
-00006dd0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006de0: 5769 6467 6574 0103 0000 0014 041f 0440  Widget.........@
-00006df0: 0438 043c 0435 0447 0430 043d 0438 0435  .8.<.5.G.0.=.8.5
-00006e00: 0800 0000 0006 0000 0004 4e6f 7465 0700  ..........Note..
-00006e10: 0000 1449 6e63 6f6d 6553 7065 6e64 696e  ...IncomeSpendin
-00006e20: 6757 6964 6765 7401 0300 0000 4804 1e04  gWidget.....H...
-00006e30: 4804 3804 3104 3a04 3000 2004 3f04 4004  H.8.1.:.0. .?.@.
-00006e40: 3800 2004 3704 3004 3f04 3804 4104 3800  8. .7.0.?.8.A.8.
-00006e50: 2004 3404 3504 4204 3004 3b04 3504 3900   .4.5.B.0.;.5.9.
-00006e60: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-00006e70: 3800 3a00 2008 0000 0000 0600 0000 214f  8.:. .........!O
-00006e80: 7065 7261 7469 6f6e 2064 6574 6169 6c73  peration details
-00006e90: 2073 7562 6d69 7420 6661 696c 6564 3a20   submit failed: 
-00006ea0: 0700 0000 1449 6e63 6f6d 6553 7065 6e64  .....IncomeSpend
-00006eb0: 696e 6757 6964 6765 7401 0300 0000 3804  ingWidget.....8.
-00006ec0: 1e04 4804 3804 3104 3a04 3000 2004 3f04  ..H.8.1.:.0. .?.
-00006ed0: 4004 3800 2004 3704 3004 3f04 3804 4104  @.8. .7.0.?.8.A.
-00006ee0: 3800 2004 3e04 3f04 3504 4004 3004 4604  8. .>.?.5.@.0.F.
-00006ef0: 3804 3800 3a00 2008 0000 0000 0600 0000  8.8.:. .........
-00006f00: 194f 7065 7261 7469 6f6e 2073 7562 6d69  .Operation submi
-00006f10: 7420 6661 696c 6564 3a20 0700 0000 1449  t failed: .....I
-00006f20: 6e63 6f6d 6553 7065 6e64 696e 6757 6964  ncomeSpendingWid
-00006f30: 6765 7401 0300 0000 2004 1e04 3f04 3b04  get..... ...?.;.
-00006f40: 3004 4204 3000 2004 3200 2004 3204 3004  0.B.0. .2. .2.0.
-00006f50: 3b04 4e04 4204 3500 3a08 0000 0000 0600  ;.N.B.5.:.......
-00006f60: 0000 1950 6169 6420 696e 2066 6f72 6569  ...Paid in forei
-00006f70: 676e 2063 7572 7265 6e63 793a 0700 0000  gn currency:....
-00006f80: 1449 6e63 6f6d 6553 7065 6e64 696e 6757  .IncomeSpendingW
-00006f90: 6964 6765 7401 0300 0000 1404 1a04 3e04  idget.........>.
-00006fa0: 3d04 4204 4004 3004 3304 3504 3d04 4208  =.B.@.0.3.5.=.B.
-00006fb0: 0000 0000 0600 0000 0450 6565 7207 0000  .........Peer...
-00006fc0: 0014 496e 636f 6d65 5370 656e 6469 6e67  ..IncomeSpending
-00006fd0: 5769 6467 6574 0103 0000 0030 0423 0434  Widget.....0.#.4
-00006fe0: 0430 043b 0438 0442 044c 0020 0434 0435  .0.;.8.B.L. .4.5
-00006ff0: 0442 0430 043b 044c 043d 0443 044e 0020  .B.0.;.L.=.C.N. 
-00007000: 0437 0430 043f 0438 0441 044c 0800 0000  .7.0.?.8.A.L....
-00007010: 0006 0000 000d 5265 6d6f 7665 2064 6574  ......Remove det
-00007020: 6169 6c07 0000 0014 496e 636f 6d65 5370  ail.....IncomeSp
-00007030: 656e 6469 6e67 5769 6467 6574 0103 0000  endingWidget....
-00007040: 000c 0026 0421 0447 0435 0442 0430 0800  ...&.!.G.5.B.0..
-00007050: 0000 0006 0000 0009 2641 6363 6f75 6e74  ........&Account
-00007060: 7307 0000 000e 4a41 4c5f 4d61 696e 5769  s.....JAL_MainWi
-00007070: 6e64 6f77 0103 0000 0012 0026 0411 044d  ndow.......&...M
-00007080: 043a 0430 043f 002e 002e 002e 0800 0000  .:.0.?..........
-00007090: 0006 0000 000a 2642 6163 6b75 702e 2e2e  ......&Backup...
-000070a0: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
-000070b0: 646f 7701 0300 0000 1e00 2604 1104 3004  dow.......&...0.
-000070c0: 3704 3e04 3204 3004 4f00 2004 3204 3004  7.>.2.0.O. .2.0.
-000070d0: 3b04 4e04 4204 3008 0000 0000 0600 0000  ;.N.B.0.........
-000070e0: 0e26 4261 7365 2043 7572 7265 6e63 7907  .&Base Currency.
-000070f0: 0000 000e 4a41 4c5f 4d61 696e 5769 6e64  ....JAL_MainWind
-00007100: 6f77 0103 0000 0014 0026 041a 0430 0442  ow.......&...0.B
-00007110: 0435 0433 043e 0440 0438 0438 0800 0000  .5.3.>.@.8.8....
-00007120: 0006 0000 000b 2643 6174 6567 6f72 6965  ......&Categorie
-00007130: 7307 0000 000e 4a41 4c5f 4d61 696e 5769  s.....JAL_MainWi
-00007140: 6e64 6f77 0103 0000 000e 0026 0414 0430  ndow.......&...0
-00007150: 043d 043d 044b 0435 0800 0000 0006 0000  .=.=.K.5........
-00007160: 0005 2644 6174 6107 0000 000e 4a41 4c5f  ..&Data.....JAL_
-00007170: 4d61 696e 5769 6e64 6f77 0103 0000 000c  MainWindow......
-00007180: 0026 0412 044b 0445 043e 0434 0800 0000  .&...K.E.>.4....
-00007190: 0006 0000 0005 2645 7869 7407 0000 000e  ......&Exit.....
-000071a0: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
-000071b0: 0000 0010 0026 042d 043a 0441 043f 043e  .....&.-.:.A.?.>
-000071c0: 0440 0442 0800 0000 0006 0000 0007 2645  .@.B..........&E
-000071d0: 7870 6f72 7407 0000 000e 4a41 4c5f 4d61  xport.....JAL_Ma
-000071e0: 696e 5769 6e64 6f77 0103 0000 000e 0026  inWindow.......&
-000071f0: 0418 043c 043f 043e 0440 0442 0800 0000  ...<.?.>.@.B....
-00007200: 0006 0000 0007 2649 6d70 6f72 7407 0000  ......&Import...
-00007210: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-00007220: 0103 0000 0012 0026 041e 0441 043d 043e  .......&...A.=.>
-00007230: 0432 043d 043e 0435 0800 0000 0006 0000  .2.=.>.5........
-00007240: 0005 264d 6169 6e07 0000 000e 4a41 4c5f  ..&Main.....JAL_
-00007250: 4d61 696e 5769 6e64 6f77 0103 0000 0012  MainWindow......
-00007260: 0026 041e 043f 0435 0440 0430 0446 0438  .&...?.5.@.0.F.8
-00007270: 0438 0800 0000 0006 0000 000b 264f 7065  .8..........&Ope
-00007280: 7261 7469 6f6e 7307 0000 000e 4a41 4c5f  rations.....JAL_
-00007290: 4d61 696e 5769 6e64 6f77 0103 0000 0018  MainWindow......
-000072a0: 041a 0026 043e 043d 0442 0440 0430 0433  ...&.>.=.B.@.0.3
-000072b0: 0435 043d 0442 044b 0800 0000 0006 0000  .5.=.B.K........
-000072c0: 0006 2650 6565 7273 0700 0000 0e4a 414c  ..&Peers.....JAL
-000072d0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
-000072e0: 1400 2604 1a04 3e04 4204 3804 4004 3e04  ..&...>.B.8.@.>.
-000072f0: 3204 3a04 3808 0000 0000 0600 0000 0726  2.:.8..........&
-00007300: 5175 6f74 6573 0700 0000 0e4a 414c 5f4d  Quotes.....JAL_M
-00007310: 6169 6e57 696e 646f 7701 0300 0000 1a00  ainWindow.......
-00007320: 2604 1a04 3e04 4204 3804 4004 3e04 3204  &...>.B.8.@.>.2.
-00007330: 3a04 3800 2e00 2e00 2e08 0000 0000 0600  :.8.............
-00007340: 0000 0a26 5175 6f74 6573 2e2e 2e07 0000  ...&Quotes......
-00007350: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
-00007360: 0103 0000 000e 0026 041e 0442 0447 0435  .......&...B.G.5
-00007370: 0442 044b 0800 0000 0006 0000 0008 2652  .B.K..........&R
-00007380: 6570 6f72 7473 0700 0000 0e4a 414c 5f4d  eports.....JAL_M
-00007390: 6169 6e57 696e 646f 7701 0300 0000 2400  ainWindow.....$.
-000073a0: 2604 1204 3e04 4104 4104 4204 3004 3d04  &...>.A.A.B.0.=.
-000073b0: 3e04 3204 3b04 3504 3d04 3804 3500 2e00  >.2.;.5.=.8.5...
-000073c0: 2e00 2e08 0000 0000 0600 0000 0b26 5265  .............&Re
-000073d0: 7374 6f72 652e 2e2e 0700 0000 0e4a 414c  store........JAL
-000073e0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
-000073f0: 0c00 2604 1e04 4204 4704 5104 4208 0000  ..&...B.G.Q.B...
-00007400: 0000 0600 0000 0a26 5374 6174 656d 656e  .......&Statemen
-00007410: 7407 0000 000e 4a41 4c5f 4d61 696e 5769  t.....JAL_MainWi
-00007420: 6e64 6f77 0103 0000 000a 0026 0422 044d  ndow.......&.".M
-00007430: 0433 0438 0800 0000 0006 0000 0005 2654  .3.8..........&T
-00007440: 6167 7307 0000 000e 4a41 4c5f 4d61 696e  ags.....JAL_Main
-00007450: 5769 6e64 6f77 0103 0000 001c 0026 0426  Window.......&.&
-00007460: 0435 043d 043d 044b 0435 0020 0431 0443  .5.=.=.K.5. .1.C
-00007470: 043c 0430 0433 0438 0800 0000 0006 0000  .<.0.3.8........
-00007480: 0007 4126 7373 6574 7307 0000 000e 4a41  ..A&ssets.....JA
-00007490: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-000074a0: 004e 041e 0442 0447 0435 0442 0020 043e  .N...B.G.5.B. .>
-000074b0: 0020 0026 0434 0432 0438 0436 0435 043d  . .&.4.2.8.6.5.=
-000074c0: 0438 044f 0445 0020 043f 043e 0020 0437  .8.O.E. .?.>. .7
-000074d0: 0430 0440 0443 0431 0435 0436 043d 044b  .0.@.C.1.5.6.=.K
-000074e0: 043c 0020 0441 0447 0435 0442 0430 043c  .<. .A.G.5.B.0.<
-000074f0: 0800 0000 0006 0000 001d 466f 7265 6967  ..........Foreig
-00007500: 6e20 6163 636f 756e 7473 2026 666c 6f77  n accounts &flow
-00007510: 2072 6570 6f72 7407 0000 000e 4a41 4c5f   report.....JAL_
-00007520: 4d61 696e 5769 6e64 6f77 0103 0000 003e  MainWindow.....>
-00007530: 0418 043d 0432 0435 0441 0442 0438 0446  ...=.2.5.A.B.8.F
-00007540: 0438 043e 043d 043d 044b 0439 0020 0026  .8.>.=.=.K.9. .&
-00007550: 043d 0430 043b 043e 0433 043e 0432 044b  .=.0.;.>.3.>.2.K
-00007560: 0439 0020 043e 0442 0447 0435 0442 0800  .9. .>.B.G.5.B..
-00007570: 0000 0006 0000 0016 496e 7665 7374 6d65  ........Investme
-00007580: 6e74 2026 7461 7820 7265 706f 7274 0700  nt &tax report..
-00007590: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
-000075a0: 7701 0300 0000 0a00 2604 2f04 3704 4b04  w.......&./.7.K.
-000075b0: 3a08 0000 0000 0600 0000 094c 2661 6e67  :..........L&ang
-000075c0: 7561 6765 0700 0000 0e4a 414c 5f4d 6169  uage.....JAL_Mai
-000075d0: 6e57 696e 646f 7701 0300 0000 2a04 1f04  nWindow.....*...
-000075e0: 3504 4004 3504 4104 4704 3804 4204 3004  5.@.5.A.G.8.B.0.
-000075f0: 4204 4c00 2000 2604 3804 4204 3e04 3304  B.L. .&.8.B.>.3.
-00007600: 3800 2e00 2e00 2e08 0000 0000 0600 0000  8...............
-00007610: 1352 652d 6275 696c 6420 264c 6564 6765  .Re-build &Ledge
-00007620: 722e 2e2e 0700 0000 0e4a 414c 5f4d 6169  r........JAL_Mai
-00007630: 6e57 696e 646f 7701 0300 0000 1604 2704  nWindow.......'.
-00007640: 3504 3a00 2000 5b00 5200 5500 5d00 2e00  5.:. .[.R.U.]...
-00007650: 2e00 2e08 0000 0000 0600 0000 0c53 6c69  .............Sli
-00007660: 7020 5b52 555d 2e2e 2e07 0000 000e 4a41  p [RU]........JA
-00007670: 4c5f 4d61 696e 5769 6e64 6f77 0103 0000  L_MainWindow....
-00007680: 0006 006a 0061 006c 0800 0000 0006 0000  ...j.a.l........
-00007690: 0003 6a61 6c07 0000 000e 4a41 4c5f 4d61  ..jal.....JAL_Ma
-000076a0: 696e 5769 6e64 6f77 0103 0000 0020 0411  inWindow..... ..
-000076b0: 0430 043d 043a 0020 0434 043b 044f 0020  .0.=.:. .4.;.O. 
-000076c0: 0441 0447 0435 0442 0430 0020 2116 0800  .A.G.5.B.0. !...
-000076d0: 0000 0006 0000 0012 4261 6e6b 2066 6f72  ........Bank for
-000076e0: 2061 6363 6f75 6e74 2023 0700 0000 0a4a   account #.....J
-000076f0: 616c 4163 636f 756e 7401 0300 0000 2a04  alAccount.....*.
-00007700: 2104 4204 4004 3004 3d04 3000 2004 3e04  !.B.@.0.=.0. .>.
-00007710: 3104 3d04 3e04 3204 3b04 5104 3d04 3000  1.=.>.2.;.Q.=.0.
-00007720: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
-00007730: 0000 1443 6f75 6e74 7279 2075 7064 6174  ...Country updat
-00007740: 6564 2066 6f72 2007 0000 0008 4a61 6c41  ed for .....JalA
-00007750: 7373 6574 0103 0000 002a 041a 043e 0442  sset.....*...>.B
-00007760: 0438 0440 043e 0432 043a 0438 0020 043e  .8.@.>.2.:.8. .>
-00007770: 0431 043d 043e 0432 043b 0435 043d 044b  .1.=.>.2.;.5.=.K
-00007780: 003a 0020 0800 0000 0006 0000 0019 5175  .:. ..........Qu
-00007790: 6f74 6174 696f 6e73 2077 6572 6520 7570  otations were up
-000077a0: 6461 7465 643a 2007 0000 0008 4a61 6c41  dated: .....JalA
-000077b0: 7373 6574 0103 0000 0046 0420 0435 0433  sset.....F. .5.3
-000077c0: 0438 0441 0442 0440 0430 0446 0438 043e  .8.A.B.@.0.F.8.>
-000077d0: 043d 043d 044b 0439 0020 043d 043e 043c  .=.=.K.9. .=.>.<
-000077e0: 0435 0440 0020 043e 0431 043d 043e 0432  .5.@. .>.1.=.>.2
-000077f0: 043b 0451 043d 0020 0434 043b 044f 0020  .;.Q.=. .4.;.O. 
-00007800: 0800 0000 0006 0000 0017 5265 672e 6e75  ..........Reg.nu
-00007810: 6d62 6572 2075 7064 6174 6564 2066 6f72  mber updated for
-00007820: 2007 0000 0008 4a61 6c41 7373 6574 0103   .....JalAsset..
-00007830: 0000 0030 041d 0435 0442 0020 043a 043e  ...0...5.B. .:.>
-00007840: 0442 0438 0440 043e 0432 043a 0438 002f  .B.8.@.>.2.:.8./
-00007850: 043a 0443 0440 0441 0430 0020 0434 043b  .:.C.@.A.0. .4.;
-00007860: 044f 0020 0800 0000 0006 0000 001c 5468  .O. ..........Th
-00007870: 6572 6520 6172 6520 6e6f 2071 756f 7465  ere are no quote
-00007880: 2f72 6174 6520 666f 7220 0700 0000 084a  /rate for .....J
-00007890: 616c 4173 7365 7401 0300 0000 4c04 1d04  alAsset.....L...
-000078a0: 3504 3e04 3604 3804 3404 3004 3d04 3d04  5.>.6.8.4.0.=.=.
-000078b0: 3004 4f00 2004 3f04 3e04 3f04 4b04 4204  0.O. .?.>.?.K.B.
-000078c0: 3a04 3000 2004 3e04 3104 3d04 3e04 3204  :.0. .>.1.=.>.2.
-000078d0: 3804 4204 4c00 2000 4900 5300 4900 4e00  8.B.L. .I.S.I.N.
-000078e0: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
-000078f0: 0000 2655 6e65 7870 6563 7465 6420 6174  ..&Unexpected at
-00007900: 7465 6d70 7420 746f 2075 7064 6174 6520  tempt to update 
-00007910: 4953 494e 2066 6f72 2007 0000 0008 4a61  ISIN for .....Ja
-00007920: 6c41 7373 6574 0103 0000 0006 0020 0432  lAsset....... .2
-00007930: 0020 0800 0000 0006 0000 0006 2069 6e74  . .......... int
-00007940: 6f20 0700 0000 094a 616c 4261 636b 7570  o .....JalBackup
-00007950: 0103 0000 001c 0410 0440 0445 0438 0432  .........@.E.8.2
-00007960: 044b 0020 0028 002a 002e 0074 0067 007a  .K. .(.*...t.g.z
-00007970: 0029 0800 0000 0006 0000 0010 4172 6368  .)..........Arch
-00007980: 6976 6573 2028 2a2e 7467 7a29 0700 0000  ives (*.tgz)....
-00007990: 094a 616c 4261 636b 7570 0103 0000 0046  .JalBackup.....F
-000079a0: 041d 0435 0020 0440 0430 0441 043f 043e  ...5. .@.0.A.?.>
-000079b0: 0437 043d 0430 043d 0430 0020 043c 0435  .7.=.0.=.0. .<.5
-000079c0: 0442 043a 0430 0020 0440 0435 0437 0435  .B.:.0. .@.5.7.5
-000079d0: 0440 0432 043d 043e 0439 0020 043a 043e  .@.2.=.>.9. .:.>
-000079e0: 043f 0438 0438 0800 0000 0006 0000 001b  .?.8.8..........
-000079f0: 4261 636b 7570 206c 6162 656c 206e 6f74  Backup label not
-00007a00: 2072 6563 6f67 6e69 7a65 6407 0000 0009   recognized.....
-00007a10: 4a61 6c42 6163 6b75 7001 0300 0000 4604  JalBackup.....F.
-00007a20: 2004 3504 3704 3504 4004 3204 3d04 3004   .5.7.5.@.2.=.0.
-00007a30: 4f00 2004 3a04 3e04 3f04 3804 4f00 2004  O. .:.>.?.8.O. .
-00007a40: 3204 3e04 4104 4104 4204 3004 3204 3d04  2.>.A.A.B.0.2.=.
-00007a50: 3e04 3204 3b04 3504 3d04 3000 2004 3804  >.2.;.5.=.0. .8.
-00007a60: 3700 3a00 2008 0000 0000 0600 0000 1642  7.:. ..........B
-00007a70: 6163 6b75 7020 7265 7374 6f72 6564 2066  ackup restored f
-00007a80: 726f 6d3a 2007 0000 0009 4a61 6c42 6163  rom: .....JalBac
-00007a90: 6b75 7001 0300 0000 3a04 2004 3504 3704  kup.....:. .5.7.
-00007aa0: 3504 4004 3204 3d04 3004 4f00 2004 3a04  5.@.2.=.0.O. .:.
-00007ab0: 3e04 3f04 3804 4f00 2004 4104 3e04 4504  >.?.8.O. .A.>.E.
-00007ac0: 4004 3004 3d04 5104 3d04 3000 2004 3200  @.0.=.Q.=.0. .2.
-00007ad0: 3a00 2008 0000 0000 0600 0000 1142 6163  :. ..........Bac
-00007ae0: 6b75 7020 7361 7665 6420 696e 3a20 0700  kup saved in: ..
-00007af0: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
-00007b00: 0052 041d 0435 0432 043e 0437 043c 043e  .R...5.2.>.7.<.>
-00007b10: 0436 043d 043e 0020 043f 0440 043e 0432  .6.=.>. .?.@.>.2
-00007b20: 0435 0440 0438 0442 044c 0020 0434 0430  .5.@.8.B.L. .4.0
-00007b30: 0442 0443 0020 0440 0435 0437 0435 0440  .B.C. .@.5.7.5.@
-00007b40: 0432 043d 043e 0439 0020 043a 043e 043f  .2.=.>.9. .:.>.?
-00007b50: 0438 0438 0800 0000 0006 0000 001a 4361  .8.8..........Ca
-00007b60: 6e27 7420 7661 6c69 6461 7465 2062 6163  n't validate bac
-00007b70: 6b75 7020 6461 7465 0700 0000 094a 616c  kup date.....Jal
-00007b80: 4261 636b 7570 0103 0000 0028 0414 0430  Backup.....(...0
-00007b90: 043d 043d 044b 0435 0020 0432 043e 0441  .=.=.K.5. .2.>.A
-00007ba0: 0441 0442 0430 043d 043e 0432 043b 0435  .A.B.0.=.>.2.;.5
-00007bb0: 043d 044b 0800 0000 0006 0000 000d 4461  .=.K..........Da
-00007bc0: 7461 2072 6573 746f 7265 6407 0000 0009  ta restored.....
-00007bd0: 4a61 6c42 6163 6b75 7001 0300 0000 4204  JalBackup.....B.
-00007be0: 1404 3004 3d04 3d04 4b04 3500 2004 3104  ..0.=.=.K.5. .1.
-00007bf0: 4b04 3b04 3800 2004 3704 3004 3304 4004  K.;.8. .7.0.3.@.
-00007c00: 4304 3604 3504 3d04 4b00 2004 3804 3700  C.6.5.=.K. .8.7.
-00007c10: 2004 3104 4d04 3a04 3004 3f04 3000 2e00   .1.M.:.0.?.0...
-00007c20: 0a08 0000 0000 0600 0000 2544 6174 6162  ..........%Datab
-00007c30: 6173 6520 7761 7320 6c6f 6164 6564 2066  ase was loaded f
-00007c40: 726f 6d20 7468 6520 6261 636b 7570 2e0a  rom the backup..
-00007c50: 0700 0000 094a 616c 4261 636b 7570 0103  .....JalBackup..
-00007c60: 0000 004e 041d 0435 0020 0443 0434 0430  ...N...5. .C.4.0
-00007c70: 043b 043e 0441 044c 0020 0432 043e 0441  .;.>.A.L. .2.>.A
-00007c80: 0441 0442 0430 043d 043e 0432 0438 0442  .A.B.0.=.>.2.8.B
-00007c90: 044c 0020 0440 0435 0437 0435 0440 0432  .L. .@.5.7.5.@.2
-00007ca0: 043d 0443 044e 0020 043a 043e 043f 0438  .=.C.N. .:.>.?.8
-00007cb0: 044e 0800 0000 0006 0000 001d 4661 696c  .N..........Fail
-00007cc0: 6564 2074 6f20 7265 7374 6f72 6520 6261  ed to restore ba
-00007cd0: 636b 7570 2066 696c 6507 0000 0009 4a61  ckup file.....Ja
-00007ce0: 6c42 6163 6b75 7001 0300 0000 3804 2104  lBackup.....8.!.
-00007cf0: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
-00007d00: 2004 4004 3504 3704 3504 4004 3204 3d04   .@.5.7.5.@.2.=.
-00007d10: 4304 4e00 2004 3a04 3e04 3f04 3804 4e00  C.N. .:.>.?.8.N.
-00007d20: 2004 3200 3a08 0000 0000 0600 0000 0f53   .2.:..........S
-00007d30: 6176 6520 6261 636b 7570 2074 6f3a 0700  ave backup to:..
-00007d40: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
-00007d50: 0040 0412 044b 0431 0435 0440 0438 0442  .@...K.1.5.@.8.B
-00007d60: 0435 0020 0444 0430 0439 043b 0020 0441  .5. .D.0.9.;. .A
-00007d70: 0020 0440 0435 0437 0435 0440 0432 043d  . .@.5.7.5.@.2.=
-00007d80: 043e 0439 0020 043a 043e 043f 0438 0435  .>.9. .:.>.?.8.5
-00007d90: 0439 0800 0000 0006 0000 0017 5365 6c65  .9..........Sele
-00007da0: 6374 2066 696c 6520 7769 7468 2062 6163  ct file with bac
-00007db0: 6b75 7007 0000 0009 4a61 6c42 6163 6b75  kup.....JalBacku
-00007dc0: 7001 0300 0000 4a04 1d04 3504 3204 3504  p.....J...5.2.5.
-00007dd0: 4004 3d04 4b04 3900 2004 4404 3e04 4004  @.=.K.9. .D.>.@.
-00007de0: 3c04 3004 4200 2004 4404 3004 3904 3b04  <.0.B. .D.0.9.;.
-00007df0: 3000 2004 4004 3504 3704 3504 4004 3204  0. .@.5.7.5.@.2.
-00007e00: 3d04 3e04 3900 2004 3a04 3e04 3f04 3804  =.>.9. .:.>.?.8.
-00007e10: 3808 0000 0000 0600 0000 1b57 726f 6e67  8..........Wrong
-00007e20: 2066 6f72 6d61 7420 6f66 2062 6163 6b75   format of backu
-00007e30: 7020 6669 6c65 0700 0000 094a 616c 4261  p file.....JalBa
-00007e40: 636b 7570 0103 0000 00c8 0412 044b 0020  ckup.........K. 
-00007e50: 0434 043e 043b 0436 043d 044b 0020 043f  .4.>.;.6.=.K. .?
-00007e60: 0435 0440 0435 0437 0430 043f 0443 0441  .5.@.5.7.0.?.C.A
-00007e70: 0442 0438 0442 044c 0020 043f 0440 0438  .B.8.B.L. .?.@.8
-00007e80: 043b 043e 0436 0435 043d 0438 0435 002c  .;.>.6.5.=.8.5.,
-00007e90: 0020 0447 0442 043e 0431 044b 0020 043f  . .G.B.>.1.K. .?
-00007ea0: 0440 0438 043c 0435 043d 0438 0442 044c  .@.8.<.5.=.8.B.L
-00007eb0: 0020 0438 0437 043c 0435 043d 0435 043d  . .8.7.<.5.=.5.=
-00007ec0: 0438 044f 000a 041f 0440 0438 043b 043e  .8.O.....@.8.;.>
-00007ed0: 0436 0435 043d 0438 0435 0020 0441 0435  .6.5.=.8.5. .A.5
-00007ee0: 0439 0447 0430 0441 0020 0437 0430 0432  .9.G.0.A. .7.0.2
-00007ef0: 0435 0440 0448 0438 0442 0020 0441 0432  .5.@.H.8.B. .A.2
-00007f00: 043e 044e 0020 0440 0430 0431 043e 0442  .>.N. .@.0.1.>.B
-00007f10: 0443 0800 0000 0006 0000 0052 596f 7520  .C.........RYou 
-00007f20: 7368 6f75 6c64 2072 6573 7461 7274 2061  should restart a
-00007f30: 7070 6c69 6361 7469 6f6e 2074 6f20 6170  pplication to ap
-00007f40: 706c 7920 6368 616e 6765 730a 4170 706c  ply changes.Appl
-00007f50: 6963 6174 696f 6e20 7769 6c6c 2062 6520  ication will be 
-00007f60: 7465 726d 696e 6174 6564 206e 6f77 0700  terminated now..
-00007f70: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
-00007f80: 0064 041e 043f 0435 0440 0430 0446 0438  .d...?.5.@.0.F.8
-00007f90: 044f 0020 0443 0436 0435 0020 0435 0441  .O. .C.6.5. .5.A
-00007fa0: 0442 044c 0020 0432 0020 0431 0430 0437  .B.L. .2. .1.0.7
-00007fb0: 0435 0020 0434 0430 043d 043d 044b 0445  .5. .4.0.=.=.K.E
-00007fc0: 0020 0438 0020 0431 044b 043b 0430 0020  . .8. .1.K.;.0. 
-00007fd0: 043f 0440 043e 043f 0443 0449 0435 043d  .?.@.>.?.C.I.5.=
-00007fe0: 0430 003a 0020 0800 0000 0006 0000 0031  .0.:. .........1
-00007ff0: 4f70 6572 6174 696f 6e20 616c 7265 6164  Operation alread
-00008000: 7920 7072 6573 656e 7420 696e 2064 6220  y present in db 
-00008010: 616e 6420 7761 7320 736b 6970 7065 643a  and was skipped:
-00008020: 2007 0000 0005 4a61 6c44 4201 0300 0000   .....JalDB.....
-00008030: 6e00 2004 3804 3c04 3504 3504 4200 2004  n. .8.<.5.5.B. .
-00008040: 3d04 3504 4104 3e04 4504 4004 3004 3d04  =.5.A.>.E.@.0.=.
-00008050: 5104 3d04 3d04 4b04 3500 2004 3804 3704  Q.=.=.K.5. .8.7.
-00008060: 3c04 3504 3d04 3504 3d04 3804 4f00 2c00  <.5.=.5.=.8.O.,.
-00008070: 0a04 3204 4b00 2004 4504 3e04 4204 3804  ..2.K. .E.>.B.8.
-00008080: 4204 3500 2004 3804 4500 2004 4104 3e04  B.5. .8.E. .A.>.
-00008090: 4504 4004 3004 3d04 3804 4204 4c00 3f08  E.@.0.=.8.B.L.?.
-000080a0: 0000 0000 0600 0000 3120 6861 7320 756e  ........1 has un
-000080b0: 636f 6d6d 6974 7465 6420 6368 616e 6765  committed change
-000080c0: 732c 0a64 6f20 796f 7520 7761 6e74 2074  s,.do you want t
-000080d0: 6f20 7361 7665 2069 743f 0700 0000 114a  o save it?.....J
-000080e0: 616c 4f70 6572 6174 696f 6e73 5461 6273  alOperationsTabs
-000080f0: 0103 0000 0036 0415 0441 0442 044c 0020  .....6...A.B.L. 
-00008100: 043d 0435 0441 043e 0445 0440 0430 043d  .=.5.A.>.E.@.0.=
-00008110: 0451 043d 043d 044b 0435 0020 0438 0437  .Q.=.=.K.5. .8.7
-00008120: 043c 0435 043d 043d 0438 044f 0800 0000  .<.5.=.=.8.O....
-00008130: 0006 0000 0018 596f 7520 6861 7665 2075  ......You have u
-00008140: 6e73 6176 6564 2063 6861 6e67 6573 0700  nsaved changes..
-00008150: 0000 114a 616c 4f70 6572 6174 696f 6e73  ...JalOperations
-00008160: 5461 6273 0103 0000 005a 041d 0435 0432  Tabs.....Z...5.2
-00008170: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00008180: 0443 0434 0430 043b 0438 0442 044c 0020  .C.4.0.;.8.B.L. 
-00008190: 043f 0440 0435 0434 043e 043f 0440 0435  .?.@.5.4.>.?.@.5
-000081a0: 0434 0435 043b 0451 043d 043d 0443 044e  .4.5.;.Q.=.=.C.N
-000081b0: 0020 043a 0430 0442 0435 0433 043e 0440  . .:.0.B.5.3.>.@
-000081c0: 0438 044e 0800 0000 0006 0000 0020 4361  .8.N......... Ca
-000081d0: 6e27 7420 6465 6c65 7465 2070 7265 6465  n't delete prede
-000081e0: 6669 6e65 6420 6361 7465 676f 7279 0700  fined category..
-000081f0: 0000 0b4a 616c 5371 6c45 7272 6f72 0103  ...JalSqlError..
-00008200: 0000 009e 042d 0442 0438 0020 0434 0430  .....-.B.8. .4.0
-00008210: 043d 043d 044b 0435 0020 043d 0435 0020  .=.=.K.5. .=.5. 
-00008220: 043c 043e 0433 0443 0442 0020 0431 044b  .<.>.3.C.B. .1.K
-00008230: 0442 044c 0020 043c 043e 0434 0438 0444  .B.L. .<.>.4.8.D
-00008240: 0438 0446 0438 0440 043e 0432 0430 043d  .8.F.8.@.>.2.0.=
-00008250: 044b 002c 0020 0442 002e 043a 002e 0020  .K.,. .B...:... 
-00008260: 043d 0430 0020 043d 0438 0445 0020 0435  .=.0. .=.8.E. .5
-00008270: 0441 0442 044c 0020 0441 0441 044b 043b  .A.B.L. .A.A.K.;
-00008280: 043a 0430 0020 0432 0020 0434 0440 0443  .:.0. .2. .4.@.C
-00008290: 0433 043e 043c 0020 043c 0435 0441 0442  .3.>.<. .<.5.A.B
-000082a0: 0435 0800 0000 0006 0000 003a 4461 7461  .5.........:Data
-000082b0: 2061 7265 2072 6566 6572 656e 6365 6420   are referenced 
-000082c0: 696e 2061 6e6f 7468 6572 2070 6c61 6365  in another place
-000082d0: 2061 6e64 2063 616e 2774 2062 6520 6d6f   and can't be mo
-000082e0: 6469 6669 6564 0700 0000 0b4a 616c 5371  dified.....JalSq
-000082f0: 6c45 7272 6f72 0103 0000 001e 041e 0448  lError.........H
-00008300: 0438 0431 043a 0430 0020 0432 0020 0434  .8.1.:.0. .2. .4
-00008310: 0430 043d 043d 044b 0445 0800 0000 0006  .0.=.=.K.E......
-00008320: 0000 000e 4461 7461 6261 7365 2065 7272  ....Database err
-00008330: 6f72 0700 0000 0b4a 616c 5371 6c45 7272  or.....JalSqlErr
-00008340: 6f72 0103 0000 0050 041d 0435 0432 0435  or.....P...5.2.5
-00008350: 0440 043d 043e 0020 0432 044b 0431 0440  .@.=.>. .2.K.1.@
-00008360: 0430 043d 0430 0020 0432 0430 043b 044e  .0.=.0. .2.0.;.N
-00008370: 0442 0430 0020 0434 043b 044f 0020 0446  .B.0. .4.;.O. .F
-00008380: 0435 043d 043d 043e 0439 0020 0431 0443  .5.=.=.>.9. .1.C
-00008390: 043c 0430 0433 0438 0800 0000 0006 0000  .<.0.3.8........
-000083a0: 002a 496e 636f 7272 6563 7420 6375 7272  .*Incorrect curr
-000083b0: 656e 6379 2061 7373 6967 6e6d 656e 7420  ency assignment 
-000083c0: 666f 7220 616e 2061 7373 6574 0700 0000  for an asset....
-000083d0: 0b4a 616c 5371 6c45 7272 6f72 0103 0000  .JalSqlError....
-000083e0: 0080 041f 043e 043b 0435 0020 0411 0430  .....>.;.5. ...0
-000083f0: 043d 043a 002f 0411 0440 043e 043a 0435  .=.:./...@.>.:.5
-00008400: 0440 0020 0434 043e 043b 0436 043d 043e  .@. .4.>.;.6.=.>
-00008410: 0020 0431 044b 0442 044c 0020 0437 0430  . .1.K.B.L. .7.0
-00008420: 043f 043e 043b 043d 0435 043d 043e 0020  .?.>.;.=.5.=.>. 
-00008430: 0434 043b 044f 0020 0438 043d 0432 0435  .4.;.O. .8.=.2.5
-00008440: 0441 0442 0438 0446 0438 043e 043d 043d  .A.B.8.F.8.>.=.=
-00008450: 043e 0433 043e 0020 0441 0447 0435 0442  .>.3.>. .A.G.5.B
-00008460: 0430 0800 0000 0006 0000 0039 496e 7665  .0.........9Inve
-00008470: 7374 6d65 6e74 2061 6363 6f75 6e74 2073  stment account s
-00008480: 686f 756c 6420 6861 7665 2061 7373 6f63  hould have assoc
-00008490: 6961 7465 6420 6272 6f6b 6572 2061 7373  iated broker ass
-000084a0: 6967 6e65 6407 0000 000b 4a61 6c53 716c  igned.....JalSql
-000084b0: 4572 726f 7201 0300 0000 8800 2004 3e04  Error....... .>.
-000084c0: 3f04 3504 4004 3004 4604 3804 3900 2004  ?.5.@.0.F.8.9. .
-000084d0: 4204 4004 3504 3104 4304 4e04 4200 2004  B.@.5.1.C.N.B. .
-000084e0: 3f04 3504 4004 3504 4004 3004 4104 4704  ?.5.@.5.@.0.A.G.
-000084f0: 3504 4204 3000 2e00 2004 1204 4b00 2004  5.B.0... ...K. .
-00008500: 4504 3e04 3404 3804 4204 3500 2004 3204  E.>.4.8.B.5. .2.
-00008510: 4b04 3f04 3e04 3b04 3d04 3804 4204 4c00  K.?.>.;.=.8.B.L.
-00008520: 2004 3504 3304 3e00 2004 3f04 4004 4f04   .5.3.>. .?.@.O.
-00008530: 3c04 3e00 2004 4104 3504 3904 4704 3004  <.>. .A.5.9.G.0.
-00008540: 4100 3f08 0000 0000 0600 0000 3c20 6f70  A.?.........< op
-00008550: 6572 6174 696f 6e73 2072 6571 7569 7265  erations require
-00008560: 2072 6562 7569 6c64 2e20 446f 2079 6f75   rebuild. Do you
-00008570: 2077 616e 7420 746f 2064 6f20 6974 2072   want to do it r
-00008580: 6967 6874 206e 6f77 3f07 0000 0006 4c65  ight now?.....Le
-00008590: 6467 6572 0103 0000 0022 002c 0020 043d  dger.....".,. .=
-000085a0: 043e 0432 0430 044f 0020 0433 0440 0430  .>.2.0.O. .3.@.0
-000085b0: 043d 0438 0446 0430 003a 0020 0800 0000  .=.8.F.0.:. ....
-000085c0: 0006 0000 0010 2c20 6e65 7720 6672 6f6e  ......, new fron
-000085d0: 7469 6572 3a20 0700 0000 064c 6564 6765  tier: .....Ledge
-000085e0: 7201 0300 0000 1a04 1f04 3e04 3404 4204  r.........>.4.B.
-000085f0: 3204 3504 4004 3604 3404 3504 3d04 3804  2.5.@.6.4.5.=.8.
-00008600: 3508 0000 0000 0600 0000 0c43 6f6e 6669  5..........Confi
-00008610: 726d 6174 696f 6e07 0000 0006 4c65 6467  rmation.....Ledg
-00008620: 6572 0103 0000 0094 041f 0440 043e 0438  er.........@.>.8
-00008630: 0437 043e 0448 043b 0430 0020 043e 0448  .7.>.H.;.0. .>.H
-00008640: 0438 0431 043a 0430 002e 0020 0420 0430  .8.1.:.0... . .0
-00008650: 0441 0447 0451 0442 0020 0438 0442 043e  .A.G.Q.B. .8.B.>
-00008660: 0433 043e 0432 0020 043d 0435 0020 043e  .3.>.2. .=.5. .>
-00008670: 043a 043e 043d 0447 0435 043d 002e 0020  .:.>.=.G.5.=... 
-00008680: 041f 0440 043e 0432 0435 0440 044c 0442  ...@.>.2.5.@.L.B
-00008690: 0435 0020 0441 043e 043e 0431 0449 0435  .5. .A.>.>.1.I.5
-000086a0: 043d 0438 044f 0020 043e 0431 0020 043e  .=.8.O. .>.1. .>
-000086b0: 0448 0438 0431 043a 0430 0445 0800 0000  .H.8.1.:.0.E....
-000086c0: 0006 0000 004d 4578 6365 7074 696f 6e20  .....MException 
-000086d0: 6861 7070 656e 6564 2e20 4c65 6467 6572  happened. Ledger
-000086e0: 2069 7320 696e 636f 6d70 6c65 7465 2e20   is incomplete. 
-000086f0: 506c 6561 7365 2063 6f72 7265 6374 2065  Please correct e
-00008700: 7272 6f72 7320 6c69 7374 6564 2069 6e20  rrors listed in 
-00008710: 6c6f 6707 0000 0006 4c65 6467 6572 0103  log.....Ledger..
-00008720: 0000 004a 0418 0442 043e 0433 0438 0020  ...J...B.>.3.8. 
-00008730: 0440 0430 0441 0441 0447 0438 0442 0430  .@.0.A.A.G.8.B.0
-00008740: 043d 044b 002e 0020 0417 0430 0442 0440  .=.K... ...0.B.@
-00008750: 0430 0447 0435 043d 043d 043e 0435 0020  .0.G.5.=.=.>.5. 
-00008760: 0432 0440 0435 043c 044f 003a 0020 0800  .2.@.5.<.O.:. ..
-00008770: 0000 0006 0000 0022 4c65 6467 6572 2069  ......."Ledger i
-00008780: 7320 636f 6d70 6c65 7465 2e20 456c 6170  s complete. Elap
-00008790: 7365 6420 7469 6d65 3a20 0700 0000 064c  sed time: .....L
-000087a0: 6564 6765 7201 0300 0000 2c04 2204 4004  edger.....,.".@.
-000087b0: 3004 3d04 3704 3004 3a04 4604 3804 3800  0.=.7.0.:.F.8.8.
-000087c0: 2004 3e04 4204 4104 4304 4204 4104 4204   .>.B.A.C.B.A.B.
-000087d0: 3204 4304 4e04 4208 0000 0000 0600 0000  2.C.N.B.........
-000087e0: 0e4c 6567 6572 2069 7320 656d 7074 7907  .Leger is empty.
-000087f0: 0000 0006 4c65 6467 6572 0103 0000 0026  ....Ledger.....&
-00008800: 041d 0435 0020 0443 043a 0430 0437 0430  ...5. .C.:.0.7.0
-00008810: 043d 0430 0020 0426 0411 0020 0434 043b  .=.0. .&... .4.;
-00008820: 044f 003a 0020 0800 0000 0006 0000 0016  .O.:. ..........
-00008830: 4e6f 2061 7373 6574 2064 6566 696e 6564  No asset defined
-00008840: 2066 6f72 3a20 0700 0000 064c 6564 6765   for: .....Ledge
-00008850: 7201 0300 0000 3404 1d04 4300 2004 4304  r.....4...C. .C.
-00008860: 3a04 3004 3704 3004 3d04 3000 2004 3a04  :.0.7.0.=.0. .:.
-00008870: 3004 4204 3504 3304 3e04 4004 3804 4f00  0.B.5.3.>.@.8.O.
-00008880: 2004 3404 3b04 4f00 3a00 2008 0000 0000   .4.;.O.:. .....
-00008890: 0600 0000 154e 6f20 6361 7465 676f 7279  .....No category
-000088a0: 2073 6574 2066 6f72 3a20 0700 0000 064c   set for: .....L
-000088b0: 6564 6765 7201 0300 0000 3404 1d04 3500  edger.....4...5.
-000088c0: 2004 4304 3a04 3004 3704 3004 3d00 2004   .C.:.0.7.0.=. .
-000088d0: 3a04 3e04 3d04 4204 4004 3004 3304 3504  :.>.=.B.@.0.3.5.
-000088e0: 3d04 4200 2004 3404 3b04 4f00 3a00 2008  =.B. .4.;.O.:. .
-000088f0: 0000 0000 0600 0000 114e 6f20 7065 6572  .........No peer
-00008900: 2073 6574 2066 6f72 3a20 0700 0000 064c   set for: .....L
-00008910: 6564 6765 7201 0300 0000 2604 1f04 3504  edger.....&...5.
-00008920: 4004 3504 4104 4704 5104 4200 2004 3804  @.5.A.G.Q.B. .8.
-00008930: 4204 3e04 3304 3e04 3200 2004 4100 3a00  B.>.3.>.2. .A.:.
-00008940: 2008 0000 0000 0600 0000 1a52 652d 6275   ..........Re-bu
-00008950: 696c 6469 6e67 206c 6564 6765 7220 7369  ilding ledger si
-00008960: 6e63 653a 2007 0000 0006 4c65 6467 6572  nce: .....Ledger
-00008970: 0103 0000 0010 041e 0447 0438 0441 0442  .........G.8.A.B
-00008980: 0438 0442 044c 0800 0000 0006 0000 0005  .8.B.L..........
-00008990: 436c 6561 7207 0000 0009 4c6f 6756 6965  Clear.....LogVie
-000089a0: 7765 7201 0300 0000 1404 1a04 3e04 3f04  wer.........>.?.
-000089b0: 3804 4004 3e04 3204 3004 4204 4c08 0000  8.@.>.2.0.B.L...
-000089c0: 0000 0600 0000 0443 6f70 7907 0000 0009  .......Copy.....
-000089d0: 4c6f 6756 6965 7765 7201 0300 0000 1604  LogViewer.......
-000089e0: 1204 4b04 3104 4004 3004 4204 4c00 2004  ..K.1.@.0.B.L. .
-000089f0: 3204 4104 5108 0000 0000 0600 0000 0a53  2.A.Q..........S
-00008a00: 656c 6563 7420 616c 6c07 0000 0009 4c6f  elect all.....Lo
-00008a10: 6756 6965 7765 7201 0300 0000 5804 1d04  gViewer.....X...
-00008a20: 3504 3804 3704 3204 3504 4104 4204 3d04  5.8.7.2.5.A.B.=.
-00008a30: 4b04 3900 2004 3f04 3004 4004 3004 3c04  K.9. .?.0.@.0.<.
-00008a40: 3504 4204 4000 2004 3a04 4004 3804 4204  5.B.@. .:.@.8.B.
-00008a50: 3804 4704 3d04 3e04 4104 4204 3800 2004  8.G.=.>.A.B.8. .
-00008a60: 4104 3e04 3e04 3104 4904 3504 3d04 3804  A.>.>.1.I.5.=.8.
-00008a70: 4f00 3a00 2008 0000 0000 0600 0000 2055  O.:. ......... U
-00008a80: 6e6b 6e6f 776e 206c 6f67 6769 6e67 206c  nknown logging l
-00008a90: 6576 656c 2070 726f 7669 6465 643a 2007  evel provided: .
-00008aa0: 0000 0009 4c6f 6756 6965 7765 7201 0300  ....LogViewer...
-00008ab0: 0000 0c25 b200 2000 6c00 6f00 6700 7308  ...%.. .l.o.g.s.
-00008ac0: 0000 0000 0600 0000 08e2 96b2 206c 6f67  ............ log
-00008ad0: 7307 0000 0009 4c6f 6756 6965 7765 7201  s.....LogViewer.
-00008ae0: 0300 0000 0c25 b600 2000 6c00 6f00 6700  .....%.. .l.o.g.
-00008af0: 7308 0000 0000 0600 0000 08e2 96b6 206c  s............. l
-00008b00: 6f67 7307 0000 0009 4c6f 6756 6965 7765  ogs.....LogViewe
-00008b10: 7201 0300 0000 3e04 1e04 4804 3804 3104  r.....>...H.8.1.
-00008b20: 3a04 3000 2004 3b04 3e04 3304 3804 3d04  :.0. .;.>.3.8.=.
-00008b30: 3000 2004 4704 3504 4004 3504 3700 2004  0. .G.5.@.5.7. .
-00008b40: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
-00008b50: 3800 3a00 2008 0000 0000 0600 0000 1345  8.:. ..........E
-00008b60: 5349 4120 6c6f 6769 6e20 6661 696c 6564  SIA login failed
-00008b70: 3a20 0700 0000 084c 6f67 696e 464e 5301  : .....LoginFNS.
-00008b80: 0300 0000 4004 2304 4104 3f04 3504 4804  ....@.#.A.?.5.H.
-00008b90: 3d04 4b04 3900 2004 3b04 3e04 3304 3804  =.K.9. .;.>.3.8.
-00008ba0: 3d00 2004 4704 3504 4004 3504 3700 2004  =. .G.5.@.5.7. .
-00008bb0: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
-00008bc0: 3800 3a00 2008 0000 0000 0600 0000 1745  8.:. ..........E
-00008bd0: 5349 4120 6c6f 6769 6e20 7375 6363 6573  SIA login succes
-00008be0: 7366 756c 3a20 0700 0000 084c 6f67 696e  sful: .....Login
-00008bf0: 464e 5301 0300 0000 3804 1e04 4804 3804  FNS.....8...H.8.
-00008c00: 3104 3a04 3000 2004 3b04 3e04 3304 3804  1.:.0. .;.>.3.8.
-00008c10: 3d04 3000 2004 4704 3504 4004 3504 3700  =.0. .G.5.@.5.7.
-00008c20: 2004 1b04 1a00 2004 2404 1d04 2100 3a00   ..... .$...!.:.
-00008c30: 2008 0000 0000 0600 0000 1246 4e53 206c   ..........FNS l
-00008c40: 6f67 696e 2066 6169 6c65 643a 2007 0000  ogin failed: ...
-00008c50: 0008 4c6f 6769 6e46 4e53 0103 0000 003a  ..LoginFNS.....:
-00008c60: 0423 0441 043f 0435 0448 043d 044b 0439  .#.A.?.5.H.=.K.9
-00008c70: 0020 043b 043e 0433 0438 043d 0020 0447  . .;.>.3.8.=. .G
-00008c80: 0435 0440 0435 0437 0020 041b 041a 0020  .5.@.5.7. ..... 
-00008c90: 0424 041d 0421 003a 0020 0800 0000 0006  .$...!.:. ......
-00008ca0: 0000 0016 464e 5320 6c6f 6769 6e20 7375  ....FNS login su
-00008cb0: 6363 6573 7366 756c 3a20 0700 0000 084c  ccessful: .....L
-00008cc0: 6f67 696e 464e 5301 0300 0000 5a04 1e04  oginFNS.....Z...
-00008cd0: 4804 3804 3104 3a04 3000 2004 3f04 3e04  H.8.1.:.0. .?.>.
-00008ce0: 3b04 4304 4704 3504 3d04 3804 4f00 2000  ;.C.G.5.=.8.O. .
-00008cf0: 5500 5200 4c00 2004 3b04 3e04 3304 3804  U.R.L. .;.>.3.8.
-00008d00: 3d04 3000 2004 4704 3504 4004 3504 3700  =.0. .G.5.@.5.7.
-00008d10: 2004 1304 3e04 4104 4304 4104 3b04 4304   ...>.A.C.A.;.C.
-00008d20: 3304 3800 3a00 2008 0000 0000 0600 0000  3.8.:. .........
-00008d30: 1547 6574 2045 5349 4120 5552 4c20 6661  .Get ESIA URL fa
-00008d40: 696c 6564 3a20 0700 0000 084c 6f67 696e  iled: .....Login
-00008d50: 464e 5301 0300 0000 3400 5300 4d00 5300  FNS.....4.S.M.S.
-00008d60: 2004 3104 4b04 3b04 3e00 2004 3704 3004   .1.K.;.>. .7.0.
-00008d70: 3f04 4004 3e04 4804 3504 3d04 3e00 2004  ?.@.>.H.5.=.>. .
-00008d80: 4304 4104 3f04 3504 4804 3d04 3e08 0000  C.A.?.5.H.=.>...
-00008d90: 0000 0600 0000 1e53 4d53 2077 6173 2072  .......SMS was r
-00008da0: 6571 7565 7374 6564 2073 7563 6365 7373  equested success
-00008db0: 6675 6c6c 7907 0000 0008 4c6f 6769 6e46  fully.....LoginF
-00008dc0: 4e53 0103 0000 001e 0410 0432 0442 043e  NS.........2.B.>
-00008dd0: 0440 0438 0437 0430 0446 0438 044f 0020  .@.8.7.0.F.8.O. 
-00008de0: 0424 041d 0421 0800 0000 0006 0000 0011  .$...!..........
-00008df0: 4175 7468 6f72 697a 6174 696f 6e20 464e  Authorization FN
-00008e00: 5307 0000 000e 4c6f 6769 6e46 4e53 4469  S.....LoginFNSDi
-00008e10: 616c 6f67 0103 0000 000e 0417 0430 043a  alog.........0.:
-00008e20: 0440 044b 0442 044c 0800 0000 0006 0000  .@.K.B.L........
-00008e30: 0005 436c 6f73 6507 0000 000e 4c6f 6769  ..Close.....Logi
-00008e40: 6e46 4e53 4469 616c 6f67 0103 0000 0016  nFNSDialog......
-00008e50: 041a 043e 0434 0020 0438 0437 0020 0053  ...>.4. .8.7. .S
-00008e60: 004d 0053 003a 0800 0000 0006 0000 000e  .M.S.:..........
-00008e70: 436f 6465 2066 726f 6d20 534d 533a 0700  Code from SMS:..
-00008e80: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
-00008e90: 6701 0300 0000 1204 1304 3e04 4104 4304  g.........>.A.C.
-00008ea0: 4104 3b04 4304 3304 3808 0000 0000 0600  A.;.C.3.8.......
-00008eb0: 0000 0a45 5349 4120 4c6f 6769 6e07 0000  ...ESIA Login...
-00008ec0: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
-00008ed0: 0103 0000 000c 041b 041a 0020 0424 041d  ........... .$..
-00008ee0: 0421 0800 0000 0006 0000 0009 464e 5320  .!..........FNS 
-00008ef0: 4c6f 6769 6e07 0000 000e 4c6f 6769 6e46  Login.....LoginF
-00008f00: 4e53 4469 616c 6f67 0103 0000 0008 0418  NSDialog........
-00008f10: 041d 041d 003a 0800 0000 0006 0000 0004  .....:..........
-00008f20: 494e 4e3a 0700 0000 0e4c 6f67 696e 464e  INN:.....LoginFN
-00008f30: 5344 6961 6c6f 6701 0300 0000 0a04 1b04  SDialog.........
-00008f40: 3e04 3304 3804 3d08 0000 0000 0600 0000  >.3.8.=.........
-00008f50: 054c 6f67 696e 0700 0000 0e4c 6f67 696e  .Login.....Login
-00008f60: 464e 5344 6961 6c6f 6701 0300 0000 0e04  FNSDialog.......
-00008f70: 1f04 3004 4004 3e04 3b04 4c00 3a08 0000  ..0.@.>.;.L.:...
-00008f80: 0000 0600 0000 0950 6173 7377 6f72 643a  .......Password:
-00008f90: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
-00008fa0: 6c6f 6701 0300 0000 1e04 1d04 3e04 3c04  log.........>.<.
-00008fb0: 3504 4000 2004 4204 3504 3b04 3504 4404  5.@. .B.5.;.5.D.
-00008fc0: 3e04 3d04 3000 3a08 0000 0000 0600 0000  >.=.0.:.........
-00008fd0: 0d50 686f 6e65 206e 756d 6265 723a 0700  .Phone number:..
-00008fe0: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
-00008ff0: 6701 0300 0000 0600 5300 4d00 5308 0000  g.......S.M.S...
-00009000: 0000 0600 0000 0953 4d53 204c 6f67 696e  .......SMS Login
-00009010: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
-00009020: 6c6f 6701 0300 0000 2604 1204 4b04 4104  log.....&...K.A.
-00009030: 3b04 3004 4204 4c00 2000 5300 4d00 5300  ;.0.B.L. .S.M.S.
-00009040: 2004 4100 2004 3a04 3e04 3404 3e04 3c08   .A. .:.>.4.>.<.
-00009050: 0000 0000 0600 0000 1253 656e 6420 534d  .........Send SM
-00009060: 5320 7769 7468 2063 6f64 6507 0000 000e  S with code.....
-00009070: 4c6f 6769 6e46 4e53 4469 616c 6f67 0103  LoginFNSDialog..
-00009080: 0000 0016 0061 0062 006f 0075 0074 003a  .....a.b.o.u.t.:
-00009090: 0062 006c 0061 006e 006b 0800 0000 0006  .b.l.a.n.k......
-000090a0: 0000 000b 6162 6f75 743a 626c 616e 6b07  ....about:blank.
-000090b0: 0000 000e 4c6f 6769 6e46 4e53 4469 616c  ....LoginFNSDial
-000090c0: 6f67 0103 0000 0044 041d 0430 0439 0434  og.....D...0.9.4
-000090d0: 0435 043d 043e 0020 043d 0435 0441 043a  .5.=.>. .=.5.A.:
-000090e0: 043e 043b 044c 043a 043e 0020 0426 0411  .>.;.L.:.>. .&..
-000090f0: 0020 043d 0430 0020 004d 004f 0045 0058  . .=.0. .M.O.E.X
-00009100: 0020 0434 043b 044f 003a 0020 0800 0000  . .4.;.O.:. ....
-00009110: 0006 0000 0020 4d75 6c74 6970 6c65 204d  ..... Multiple M
-00009120: 4f45 5820 6173 7365 7473 2066 6f75 6e64  OEX assets found
-00009130: 2066 6f72 3a20 0700 0000 044d 4f45 5801   for: .....MOEX.
-00009140: 0300 0000 4404 1d04 3504 3f04 3e04 3404  ....D...5.?.>.4.
-00009150: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
-00009160: 3c04 4b04 3900 2004 4204 3804 3f00 2004  <.K.9. .B.8.?. .
-00009170: 2604 1100 2004 1c04 3e04 4104 1104 3804  &... ...>.A...8.
-00009180: 4004 3604 3800 3a00 2008 0000 0000 0600  @.6.8.:. .......
-00009190: 0000 2055 6e73 7570 706f 7274 6564 204d  .. Unsupported M
-000091a0: 4f45 5820 7365 6375 7269 7479 2074 7970  OEX security typ
-000091b0: 653a 2007 0000 0004 4d4f 4558 0103 0000  e: .....MOEX....
-000091c0: 0016 041e 0020 043f 0440 043e 0433 0440  ..... .?.@.>.3.@
-000091d0: 0430 043c 043c 0435 0800 0000 0006 0000  .0.<.<.5........
-000091e0: 0005 4162 6f75 7407 0000 000a 4d61 696e  ..About.....Main
-000091f0: 5769 6e64 6f77 0103 0000 001a 041f 043e  Window.........>
-00009200: 0434 0442 0432 0435 0440 0436 0434 0435  .4.B.2.5.@.6.4.5
-00009210: 043d 0438 0435 0800 0000 0006 0000 000c  .=.8.5..........
-00009220: 436f 6e66 6972 6d61 7469 6f6e 0700 0000  Confirmation....
-00009230: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
-00009240: 1404 1804 3d04 4404 3e04 4004 3c04 3004  ....=.D.>.@.<.0.
-00009250: 4604 3804 4f08 0000 0000 0600 0000 0449  F.8.O..........I
-00009260: 6e66 6f07 0000 000a 4d61 696e 5769 6e64  nfo.....MainWind
-00009270: 6f77 0103 0000 0028 042f 0437 044b 043a  ow.....(./.7.K.:
-00009280: 0020 0431 044b 043b 0020 0438 0437 043c  . .1.K.;. .8.7.<
-00009290: 0435 043d 0451 043d 0020 043d 0430 0020  .5.=.Q.=. .=.0. 
-000092a0: 0800 0000 0006 0000 0018 4c61 6e67 7561  ..........Langua
-000092b0: 6765 2077 6173 2063 6861 6e67 6564 2074  ge was changed t
-000092c0: 6f20 0700 0000 0a4d 6169 6e57 696e 646f  o .....MainWindo
-000092d0: 7701 0300 0000 6204 1804 4204 3e04 3304  w.....b...B.>.3.
-000092e0: 3800 2004 4204 4004 3004 3d04 3704 3004  8. .B.@.0.=.7.0.
-000092f0: 3a04 4604 3804 3900 2004 3d04 3504 3004  :.F.8.9. .=.5.0.
-00009300: 3a04 4204 4304 3004 3b04 4c04 3d04 4b00  :.B.C.0.;.L.=.K.
-00009310: 2e00 2004 1f04 3504 4004 3504 4104 4704  .. ...5.@.5.A.G.
-00009320: 3804 4204 3004 4204 4c00 2004 4104 3504  8.B.0.B.L. .A.5.
-00009330: 3904 4704 3004 4100 3f08 0000 0000 0600  9.G.0.A.?.......
-00009340: 0000 264c 6564 6765 7220 6973 6e27 7420  ..&Ledger isn't 
-00009350: 636f 6d70 6c65 7465 2e20 5265 6275 696c  complete. Rebuil
-00009360: 6420 6974 206e 6f77 3f07 0000 000a 4d61  d it now?.....Ma
-00009370: 696e 5769 6e64 6f77 0103 0000 0080 0414  inWindow........
-00009380: 043e 043f 043e 043b 043d 0438 0442 0435  .>.?.>.;.=.8.B.5
-00009390: 043b 044c 043d 0430 044f 0020 0438 043d  .;.L.=.0.O. .8.=
-000093a0: 0444 043e 0440 043c 0430 0446 0438 044f  .D.>.@.<.0.F.8.O
-000093b0: 002c 0020 0438 043d 0441 0442 0440 0443  .,. .8.=.A.B.@.C
-000093c0: 043a 0446 0438 0438 002c 0020 0441 043e  .:.F.8.8.,. .A.>
-000093d0: 043e 0431 0449 0435 043d 0438 044f 0020  .>.1.I.5.=.8.O. 
-000093e0: 043e 0020 043f 0440 043e 0431 043b 0435  .>. .?.@.>.1.;.5
-000093f0: 043c 0430 0445 0020 043d 0430 0020 0800  .<.0.E. .=.0. ..
-00009400: 0000 0006 0000 0035 4d6f 7265 2069 6e66  .......5More inf
-00009410: 6f72 6d61 7469 6f6e 2c20 6d61 6e75 616c  ormation, manual
-00009420: 7320 616e 6420 7072 6f62 6c65 6d20 7265  s and problem re
-00009430: 706f 7274 7320 6172 6520 6174 2007 0000  ports are at ...
-00009440: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-00009450: 0050 0412 043e 043f 0440 043e 0441 044b  .P...>.?.@.>.A.K
-00009460: 002c 0020 043a 043e 043c 043c 0435 043d  .,. .:.>.<.<.5.=
-00009470: 0442 0430 0440 0438 0438 002c 0020 043f  .B.0.@.8.8.,. .?
-00009480: 043e 043c 043e 0449 044c 0020 0438 043b  .>.<.>.I.L. .8.;
-00009490: 0438 0020 0434 043e 043d 0430 0442 044b  .8. .4.>.=.0.B.K
-000094a0: 003a 0800 0000 0006 0000 0027 5175 6573  .:.........'Ques
-000094b0: 7469 6f6e 732c 2063 6f6d 6d65 6e74 732c  tions, comments,
-000094c0: 2068 656c 7020 6f72 2064 6f6e 6174 696f   help or donatio
-000094d0: 6e73 3a07 0000 000a 4d61 696e 5769 6e64  ns:.....MainWind
-000094e0: 6f77 0103 0000 0022 0422 0440 0435 0431  ow.....".".@.5.1
-000094f0: 0443 0435 0442 0441 044f 0020 0440 0435  .C.5.B.A.O. .@.5
-00009500: 0441 0442 0430 0440 0442 0800 0000 0006  .A.B.0.@.B......
-00009510: 0000 0010 5265 7374 6172 7420 7265 7175  ....Restart requ
-00009520: 6972 6564 0700 0000 0a4d 6169 6e57 696e  ired.....MainWin
-00009530: 646f 7701 0300 0000 5004 1a04 3e04 3d04  dow.....P...>.=.
-00009540: 3504 4704 3d04 4b04 3900 2004 3104 3004  5.G.=.K.9. .1.0.
-00009550: 3b04 3004 3d04 4100 2004 3f04 3e00 2004  ;.0.=.A. .?.>. .
-00009560: 3e04 4204 4704 5104 4204 4300 2004 3d04  >.B.G.Q.B.C. .=.
-00009570: 3500 2004 4104 3e04 3204 3f04 3004 3404  5. .A.>.2.?.0.4.
-00009580: 3004 3504 4200 3a00 2008 0000 0000 0600  0.5.B.:. .......
-00009590: 0000 2853 7461 7465 6d65 6e74 2065 6e64  ..(Statement end
-000095a0: 696e 6720 6261 6c61 6e63 6520 646f 6573  ing balance does
-000095b0: 6e27 7420 6d61 7463 683a 2007 0000 000a  n't match: .....
-000095c0: 4d61 696e 5769 6e64 6f77 0103 0000 00c8  MainWindow......
-000095d0: 0412 044b 0020 0434 043e 043b 0436 043d  ...K. .4.>.;.6.=
-000095e0: 044b 0020 043f 0435 0440 0435 0437 0430  .K. .?.5.@.5.7.0
-000095f0: 043f 0443 0441 0442 0438 0442 044c 0020  .?.C.A.B.8.B.L. 
-00009600: 043f 0440 0438 043b 043e 0436 0435 043d  .?.@.8.;.>.6.5.=
-00009610: 0438 0435 002c 0020 0447 0442 043e 0431  .8.5.,. .G.B.>.1
-00009620: 044b 0020 043f 0440 0438 043c 0435 043d  .K. .?.@.8.<.5.=
-00009630: 0438 0442 044c 0020 0438 0437 043c 0435  .8.B.L. .8.7.<.5
-00009640: 043d 0435 043d 0438 044f 000a 041f 0440  .=.5.=.8.O.....@
-00009650: 0438 043b 043e 0436 0435 043d 0438 0435  .8.;.>.6.5.=.8.5
-00009660: 0020 0441 0435 0439 0447 0430 0441 0020  . .A.5.9.G.0.A. 
-00009670: 0437 0430 0432 0435 0440 0448 0438 0442  .7.0.2.5.@.H.8.B
-00009680: 0020 0441 0432 043e 044e 0020 0440 0430  . .A.2.>.N. .@.0
-00009690: 0431 043e 0442 0443 0800 0000 0006 0000  .1.>.B.C........
-000096a0: 0052 596f 7520 7368 6f75 6c64 2072 6573  .RYou should res
-000096b0: 7461 7274 2061 7070 6c69 6361 7469 6f6e  tart application
-000096c0: 2074 6f20 6170 706c 7920 6368 616e 6765   to apply change
-000096d0: 730a 4170 706c 6963 6174 696f 6e20 7769  s.Application wi
-000096e0: 6c6c 2062 6520 7465 726d 696e 6174 6564  ll be terminated
-000096f0: 206e 6f77 0700 0000 0a4d 6169 6e57 696e   now.....MainWin
-00009700: 646f 7701 0300 0000 3004 3404 3e04 3c04  dow.....0.4.>.<.
-00009710: 3004 4804 3d04 3504 3900 2004 4104 4204  0.H.=.5.9. .A.B.
-00009720: 4004 3004 3d04 3804 4604 3500 2000 6700  @.0.=.8.F.5. .g.
-00009730: 6900 7400 6800 7500 6208 0000 0000 0600  i.t.h.u.b.......
-00009740: 0000 1067 6974 6875 6220 686f 6d65 2070  ...github home p
-00009750: 6167 6507 0000 000a 4d61 696e 5769 6e64  age.....MainWind
-00009760: 6f77 0103 0000 000c 0432 0435 0440 0441  ow.......2.5.@.A
-00009770: 0438 044f 0800 0000 0006 0000 0007 7665  .8.O..........ve
-00009780: 7273 696f 6e07 0000 000a 4d61 696e 5769  rsion.....MainWi
-00009790: 6e64 6f77 0103 0000 0006 002e 002e 002e  ndow............
-000097a0: 0800 0000 0006 0000 0003 2e2e 2e07 0000  ................
-000097b0: 000f 4d6f 6e65 7946 6c6f 7757 6964 6765  ..MoneyFlowWidge
-000097c0: 7401 0300 0000 1604 2404 3004 3904 3b00  t.......$.0.9.;.
-000097d0: 2000 4500 7800 6300 6500 6c00 3a08 0000   .E.x.c.e.l.:...
-000097e0: 0000 0600 0000 0b45 7863 656c 2066 696c  .......Excel fil
-000097f0: 653a 0700 0000 0f4d 6f6e 6579 466c 6f77  e:.....MoneyFlow
-00009800: 5769 6467 6574 0103 0000 0028 0424 0430  Widget.....(.$.0
-00009810: 0439 043b 044b 0020 0045 0078 0063 0065  .9.;.K. .E.x.c.e
-00009820: 006c 0020 0028 002a 002e 0078 0073 006c  .l. .(.*...x.s.l
-00009830: 0078 0029 0800 0000 0006 0000 0014 4578  .x.)..........Ex
-00009840: 6365 6c20 6669 6c65 7320 282a 2e78 6c73  cel files (*.xls
-00009850: 7829 0700 0000 0f4d 6f6e 6579 466c 6f77  x).....MoneyFlow
-00009860: 5769 6467 6574 0103 0000 0056 0424 0430  Widget.....V.$.0
-00009870: 0439 043b 0020 0434 043b 044f 0020 0441  .9.;. .4.;.O. .A
-00009880: 043e 0445 0440 0430 043d 0435 043d 0438  .>.E.@.0.=.5.=.8
-00009890: 044f 0020 0440 0430 0441 0447 0451 0442  .O. .@.0.A.G.Q.B
-000098a0: 0430 0020 0432 0020 0444 043e 0440 043c  .0. .2. .D.>.@.<
-000098b0: 0430 0442 0435 0020 0045 0078 0063 0065  .0.B.5. .E.x.c.e
-000098c0: 006c 0800 0000 0006 0000 002e 4669 6c65  .l..........File
-000098d0: 2077 6865 7265 2074 6f20 7374 6f72 6520   where to store 
-000098e0: 7461 7820 7265 706f 7274 2069 6e20 4578  tax report in Ex
-000098f0: 6365 6c20 666f 726d 6174 0700 0000 0f4d  cel format.....M
-00009900: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
-00009910: 0000 000a 041e 043e 0414 0414 0421 0800  .......>.....!..
-00009920: 0000 0006 0000 000a 4d6f 6e65 7920 466c  ........Money Fl
-00009930: 6f77 0700 0000 0f4d 6f6e 6579 466c 6f77  ow.....MoneyFlow
-00009940: 5769 6467 6574 0103 0000 002e 041e 043e  Widget.........>
-00009950: 0414 0414 0421 0020 0441 043e 0445 0440  .....!. .A.>.E.@
-00009960: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
-00009970: 0430 0439 043b 0435 0020 0800 0000 0006  .0.9.;.5. ......
-00009980: 0000 0020 4d6f 6e65 7920 666c 6f77 2072  ... Money flow r
-00009990: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
-000099a0: 696c 6520 0700 0000 0f4d 6f6e 6579 466c  ile .....MoneyFl
-000099b0: 6f77 5769 6467 6574 0103 0000 001e 0421  owWidget.......!
-000099c0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
-000099d0: 0020 041e 0442 0447 0451 0442 0800 0000  . ...B.G.Q.B....
-000099e0: 0006 0000 000b 5361 7665 2052 6570 6f72  ......Save Repor
-000099f0: 7407 0000 000f 4d6f 6e65 7946 6c6f 7757  t.....MoneyFlowW
-00009a00: 6964 6765 7401 0300 0000 2404 2104 3e04  idget.....$.!.>.
-00009a10: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
-00009a20: 1e04 3e04 1404 1404 2100 2004 3200 3a08  ..>.....!. .2.:.
-00009a30: 0000 0000 0600 0000 1a53 6176 6520 6d6f  .........Save mo
-00009a40: 6e65 7920 666c 6f77 2072 6570 6f72 7420  ney flow report 
-00009a50: 746f 3a07 0000 000f 4d6f 6e65 7946 6c6f  to:.....MoneyFlo
-00009a60: 7757 6964 6765 7401 0300 0000 1804 1204  wWidget.........
-00009a70: 4b04 3104 3504 4004 3804 4200 2004 4404  K.1.5.@.8.B. .D.
-00009a80: 3004 3904 3b08 0000 0000 0600 0000 0b53  0.9.;..........S
-00009a90: 656c 6563 7420 6669 6c65 0700 0000 0f4d  elect file.....M
-00009aa0: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
-00009ab0: 0000 0008 0413 043e 0434 003a 0800 0000  .......>.4.:....
-00009ac0: 0006 0000 0005 5965 6172 3a07 0000 000f  ......Year:.....
-00009ad0: 4d6f 6e65 7946 6c6f 7757 6964 6765 7401  MoneyFlowWidget.
-00009ae0: 0300 0000 2800 2004 3d04 3504 4304 4104  ....(. .=.5.C.A.
-00009af0: 3f04 3504 4804 3d04 4b04 3900 2004 3704  ?.5.H.=.K.9. .7.
-00009b00: 3004 3f04 4004 3e04 4100 3a00 2008 0000  0.?.@.>.A.:. ...
-00009b10: 0000 0600 0000 0920 6661 696c 6564 3a20  ....... failed: 
-00009b20: 0700 0000 034e 6574 0103 0000 0034 0422  .....Net.....4."
-00009b30: 0438 043f 0020 0426 0411 0020 043d 0435  .8.?. .&... .=.5
-00009b40: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
-00009b50: 0438 0432 0430 0435 0442 0441 044f 003a  .8.2.0.5.B.A.O.:
-00009b60: 0020 0800 0000 0006 0000 001c 4173 7365  . ..........Asse
-00009b70: 7420 7479 7065 2069 736e 2774 2073 7570  t type isn't sup
-00009b80: 706f 7274 6564 3a20 0700 0000 0a4f 7065  ported: .....Ope
-00009b90: 6e42 726f 6b65 7201 0300 0000 3204 1104  nBroker.....2...
-00009ba0: 3804 4004 3604 3000 2004 3d04 3500 2004  8.@.6.0. .=.5. .
-00009bb0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-00009bc0: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
-00009bd0: 0000 0000 0600 0000 1a45 7863 6861 6e67  .........Exchang
-00009be0: 6520 6973 6e27 7420 7375 7070 6f72 7465  e isn't supporte
-00009bf0: 643a 2007 0000 000a 4f70 656e 4272 6f6b  d: .....OpenBrok
-00009c00: 6572 0103 0000 0008 0421 0447 0435 0442  er.......!.G.5.B
-00009c10: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
-00009c20: 7407 0000 000f 4f70 6572 6174 696f 6e73  t.....Operations
-00009c30: 4d6f 6465 6c01 0300 0000 0a04 2104 4304  Model.......!.C.
-00009c40: 3c04 3c04 3008 0000 0000 0600 0000 0641  <.<.0..........A
-00009c50: 6d6f 756e 7407 0000 000f 4f70 6572 6174  mount.....Operat
-00009c60: 696f 6e73 4d6f 6465 6c01 0300 0000 0c04  ionsModel.......
-00009c70: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
-00009c80: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
-00009c90: 0f4f 7065 7261 7469 6f6e 734d 6f64 656c  .OperationsModel
-00009ca0: 0103 0000 000c 0412 0430 043b 044e 0442  .........0.;.N.B
-00009cb0: 0430 0800 0000 0006 0000 0008 4375 7272  .0..........Curr
-00009cc0: 656e 6379 0700 0000 0f4f 7065 7261 7469  ency.....Operati
-00009cd0: 6f6e 734d 6f64 656c 0103 0000 0010 041e  onsModel........
-00009ce0: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
-00009cf0: 0000 0006 0000 0005 4e6f 7465 7307 0000  ........Notes...
-00009d00: 000f 4f70 6572 6174 696f 6e73 4d6f 6465  ..OperationsMode
-00009d10: 6c01 0300 0000 1404 1404 3004 4204 3000  l.........0.B.0.
-00009d20: 2f04 1204 4004 3504 3c04 4f08 0000 0000  /...@.5.<.O.....
-00009d30: 0600 0000 0954 696d 6573 7461 6d70 0700  .....Timestamp..
-00009d40: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
-00009d50: 656c 0103 0000 000a 0421 0447 0435 0442  el.......!.G.5.B
-00009d60: 003a 0800 0000 0006 0000 0008 4163 636f  .:..........Acco
-00009d70: 756e 743a 0700 0000 104f 7065 7261 7469  unt:.....Operati
-00009d80: 6f6e 7357 6964 6765 7401 0300 0000 4a04  onsWidget.....J.
-00009d90: 1204 4b00 2004 4504 3e04 4204 3804 4204  ..K. .E.>.B.8.B.
-00009da0: 3500 2004 4304 3404 3004 3b04 3804 4204  5. .C.4.0.;.8.B.
-00009db0: 4c00 2004 3204 4b04 3104 4004 3004 3d04  L. .2.K.1.@.0.=.
-00009dc0: 3d04 4b04 3500 2004 3e04 3f04 3504 4004  =.K.5. .>.?.5.@.
-00009dd0: 3004 4604 3804 3800 3f08 0000 0000 0600  0.F.8.8.?.......
-00009de0: 0000 2e41 7265 2079 6f75 2073 7572 6520  ...Are you sure 
-00009df0: 746f 2064 656c 6574 6520 7365 6c65 6374  to delete select
-00009e00: 6564 2074 7261 6e73 6163 696f 6e28 7329  ed transacion(s)
-00009e10: 3f07 0000 0010 4f70 6572 6174 696f 6e73  ?.....Operations
-00009e20: 5769 6467 6574 0103 0000 001c 0411 0430  Widget.........0
-00009e30: 043b 0430 043d 0441 044b 0020 0441 0447  .;.0.=.A.K. .A.G
-00009e40: 0435 0442 043e 0432 0800 0000 0006 0000  .5.B.>.2........
-00009e50: 0008 4261 6c61 6e63 6573 0700 0000 104f  ..Balances.....O
-00009e60: 7065 7261 7469 6f6e 7357 6964 6765 7401  perationsWidget.
-00009e70: 0300 0000 1a04 1f04 3e04 3404 4204 3204  ........>.4.B.2.
-00009e80: 3504 4004 3604 3404 3504 3d04 3804 3508  5.@.6.4.5.=.8.5.
-00009e90: 0000 0000 0600 0000 0c43 6f6e 6669 726d  .........Confirm
-00009ea0: 6174 696f 6e07 0000 0010 4f70 6572 6174  ation.....Operat
-00009eb0: 696f 6e73 5769 6467 6574 0103 0000 0014  ionsWidget......
-00009ec0: 041a 043e 043f 0438 0440 043e 0432 0430  ...>.?.8.@.>.2.0
-00009ed0: 0442 044c 0800 0000 0006 0000 0004 436f  .B.L..........Co
-00009ee0: 7079 0700 0000 104f 7065 7261 7469 6f6e  py.....Operation
-00009ef0: 7357 6964 6765 7401 0300 0000 2604 1a04  sWidget.....&...
-00009f00: 3e04 3f04 3804 4004 3e04 3204 3004 4204  >.?.8.@.>.2.0.B.
-00009f10: 4c00 2004 3e04 3f04 3504 4004 3004 4604  L. .>.?.5.@.0.F.
-00009f20: 3804 4e08 0000 0000 0600 0000 0e43 6f70  8.N..........Cop
-00009f30: 7920 6f70 6572 6174 696f 6e07 0000 0010  y operation.....
-00009f40: 4f70 6572 6174 696f 6e73 5769 6467 6574  OperationsWidget
-00009f50: 0103 0000 000e 0423 0434 0430 043b 0438  .......#.4.0.;.8
-00009f60: 0442 044c 0800 0000 0006 0000 0006 4465  .B.L..........De
-00009f70: 6c65 7465 0700 0000 104f 7065 7261 7469  lete.....Operati
-00009f80: 6f6e 7357 6964 6765 7401 0300 0000 2004  onsWidget..... .
-00009f90: 2304 3404 3004 3b04 3804 4204 4c00 2004  #.4.0.;.8.B.L. .
-00009fa0: 3e04 3f04 3504 4004 3004 4604 3804 4e08  >.?.5.@.0.F.8.N.
-00009fb0: 0000 0000 0600 0000 1044 656c 6574 6520  .........Delete 
-00009fc0: 6f70 6572 6174 696f 6e07 0000 0010 4f70  operation.....Op
-00009fd0: 6572 6174 696f 6e73 5769 6467 6574 0103  erationsWidget..
-00009fe0: 0000 001c 041d 043e 0432 0430 044f 0020  .......>.2.0.O. 
-00009ff0: 043e 043f 0435 0440 0430 0446 0438 044f  .>.?.5.@.0.F.8.O
-0000a000: 0800 0000 0006 0000 000d 4e65 7720 6f70  ..........New op
-0000a010: 6572 6174 696f 6e07 0000 0010 4f70 6572  eration.....Oper
-0000a020: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
-0000a030: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
-0000a040: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
-0000a050: 6174 696f 6e73 0700 0000 104f 7065 7261  ations.....Opera
-0000a060: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
-0000a070: 2404 1e04 3f04 3504 4004 3004 4604 3804  $...?.5.@.0.F.8.
-0000a080: 3800 2004 3800 2004 1104 3004 3b04 3004  8. .8. ...0.;.0.
-0000a090: 3d04 4104 4b08 0000 0000 0600 0000 154f  =.A.K..........O
-0000a0a0: 7065 7261 7469 6f6e 7320 2620 4261 6c61  perations & Bala
-0000a0b0: 6e63 6573 0700 0000 104f 7065 7261 7469  nces.....Operati
-0000a0c0: 6f6e 7357 6964 6765 7401 0300 0000 0e04  onsWidget.......
-0000a0d0: 2104 3204 3504 4004 3804 4204 4c08 0000  !.2.5.@.8.B.L...
-0000a0e0: 0000 0600 0000 0952 6563 6f6e 6369 6c65  .......Reconcile
-0000a0f0: 0700 0000 104f 7065 7261 7469 6f6e 7357  .....OperationsW
-0000a100: 6964 6765 7401 0300 0000 0c04 1f04 3e04  idget.........>.
-0000a110: 3804 4104 3a00 3a08 0000 0000 0600 0000  8.A.:.:.........
-0000a120: 0753 6561 7263 683a 0700 0000 104f 7065  .Search:.....Ope
-0000a130: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
-0000a140: 0000 2c04 1f04 3e04 3a04 3004 3704 4b04  ..,...>.:.0.7.K.
-0000a150: 3204 3004 4204 4c00 2000 2604 3d04 3504  2.0.B.L. .&.=.5.
-0000a160: 3004 3a04 4204 3804 3204 3d04 4b04 3508  0.:.B.8.2.=.K.5.
-0000a170: 0000 0000 0600 0000 0e53 686f 7720 2649  .........Show &I
-0000a180: 6e61 6374 6976 6507 0000 0010 4f70 6572  nactive.....Oper
-0000a190: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
-0000a1a0: 001a 0412 0430 043b 044e 0442 0430 0020  .....0.;.N.B.0. 
-0000a1b0: 0438 0442 043e 0433 043e 003a 0800 0000  .8.B.>.3.>.:....
-0000a1c0: 0006 0000 000d 5375 6d20 4375 7272 656e  ......Sum Curren
-0000a1d0: 6379 3a07 0000 0010 4f70 6572 6174 696f  cy:.....Operatio
-0000a1e0: 6e73 5769 6467 6574 0103 0000 0014 0064  nsWidget.......d
-0000a1f0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
-0000a200: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
-0000a210: 4d2f 7979 7979 0700 0000 104f 7065 7261  M/yyyy.....Opera
-0000a220: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
-0000a230: 0c04 1204 3004 3b04 4e04 4204 3008 0000  ....0.;.N.B.0...
-0000a240: 0000 0600 0000 0843 7572 7265 6e63 7907  .......Currency.
-0000a250: 0000 0018 4f70 7469 6f6e 616c 4375 7272  ....OptionalCurr
-0000a260: 656e 6379 436f 6d62 6f42 6f78 0103 0000  encyComboBox....
-0000a270: 000a 0421 0443 043c 043c 0430 0800 0000  ...!.C.<.<.0....
-0000a280: 0006 0000 0006 416d 6f75 6e74 0700 0000  ......Amount....
-0000a290: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
-0000a2a0: 6c01 0300 0000 1204 1a04 3004 4204 3504  l.........0.B.5.
-0000a2b0: 3304 3e04 4004 3804 4f08 0000 0000 0600  3.>.@.8.O.......
-0000a2c0: 0000 0843 6174 6567 6f72 7907 0000 0010  ...Category.....
-0000a2d0: 5061 6e64 6173 4c69 6e65 734d 6f64 656c  PandasLinesModel
-0000a2e0: 0103 0000 0022 041d 0430 0437 0432 0430  ....."...0.7.2.0
-0000a2f0: 043d 0438 0435 0020 043f 0440 043e 0434  .=.8.5. .?.@.>.4
-0000a300: 0443 043a 0442 0430 0800 0000 0006 0000  .C.:.B.0........
-0000a310: 000c 5072 6f64 7563 7420 6e61 6d65 0700  ..Product name..
-0000a320: 0000 1050 616e 6461 734c 696e 6573 4d6f  ...PandasLinesMo
-0000a330: 6465 6c01 0300 0000 0604 2204 4d04 3308  del.......".M.3.
-0000a340: 0000 0000 0600 0000 0354 6167 0700 0000  .........Tag....
-0000a350: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
-0000a360: 6c01 0300 0000 2400 2700 2004 3704 3004  l.....$.'. .7.0.
-0000a370: 3c04 3504 3d04 3504 3d04 3000 2004 4304  <.5.=.5.=.0. .C.
-0000a380: 4104 3f04 3504 4804 3d04 3e08 0000 0000  A.?.5.H.=.>.....
-0000a390: 0600 0000 1b27 2077 6173 2073 7563 6365  .....' was succe
-0000a3a0: 7373 6675 6c6c 7920 7265 706c 6163 6564  ssfully replaced
-0000a3b0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
-0000a3c0: 6c6f 6701 0300 0000 0c00 2700 2004 3d04  log.......'. .=.
-0000a3d0: 3000 3a00 2008 0000 0000 0600 0000 0827  0.:. ..........'
-0000a3e0: 2077 6974 683a 2007 0000 000e 5065 6572   with: .....Peer
-0000a3f0: 4c69 7374 4469 616c 6f67 0103 0000 004e  ListDialog.....N
-0000a400: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
-0000a410: 044c 0020 0441 0442 0430 0440 043e 0435  .L. .A.B.0.@.>.5
-0000a420: 0020 043d 0430 0437 0432 0430 043d 0438  . .=.0.7.2.0.=.8
-0000a430: 0435 0020 0432 0020 043f 0440 0438 043c  .5. .2. .?.@.8.<
-0000a440: 0435 0447 0430 043d 0438 0438 003f 0800  .5.G.0.=.8.8.?..
-0000a450: 0000 0006 0000 0017 4b65 6570 206f 6c64  ........Keep old
-0000a460: 206e 616d 6520 696e 206e 6f74 6573 3f07   name in notes?.
-0000a470: 0000 000e 5065 6572 4c69 7374 4469 616c  ....PeerListDial
-0000a480: 6f67 0103 0000 0018 041a 043e 043d 0442  og.........>.=.B
-0000a490: 0440 0430 0433 0435 043d 0442 0020 0027  .@.0.3.5.=.B. .'
-0000a4a0: 0800 0000 0006 0000 0006 5065 6572 2027  ..........Peer '
-0000a4b0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
-0000a4c0: 6c6f 6701 0300 0000 1604 1a04 3e04 3d04  log.........>.=.
-0000a4d0: 4204 4004 3004 3304 3504 3d04 4204 4b08  B.@.0.3.5.=.B.K.
-0000a4e0: 0000 0000 0600 0000 0550 6565 7273 0700  .........Peers..
-0000a4f0: 0000 0e50 6565 724c 6973 7444 6961 6c6f  ...PeerListDialo
-0000a500: 6701 0300 0000 2c04 1704 3004 3c04 3504  g.....,...0.<.5.
-0000a510: 3d04 3804 4204 4c00 2004 3a04 3e04 3d04  =.8.B.L. .:.>.=.
-0000a520: 4204 4004 3004 3304 3504 3d04 4204 3000  B.@.0.3.5.=.B.0.
-0000a530: 2000 2708 0000 0000 0600 0000 0e52 6570   .'..........Rep
-0000a540: 6c61 6365 2070 6565 7220 2707 0000 000e  lace peer '.....
-0000a550: 5065 6572 4c69 7374 4469 616c 6f67 0103  PeerListDialog..
-0000a560: 0000 001c 0417 0430 043c 0435 043d 0438  .......0.<.5.=.8
-0000a570: 0442 044c 0020 043d 0430 002e 002e 002e  .B.L. .=.0......
-0000a580: 0800 0000 0006 0000 000f 5265 706c 6163  ..........Replac
-0000a590: 6520 7769 7468 2e2e 2e07 0000 000e 5065  e with........Pe
-0000a5a0: 6572 4c69 7374 4469 616c 6f67 0103 0000  erListDialog....
-0000a5b0: 0040 041f 043e 043a 0430 0437 0430 0442  .@...>.:.0.7.0.B
-0000a5c0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
-0000a5d0: 0438 0438 0020 0441 0020 041a 043e 043d  .8.8. .A. ...>.=
-0000a5e0: 0442 0440 0430 0433 0435 043d 0442 043e  .B.@.0.3.5.=.B.>
-0000a5f0: 043c 0800 0000 0006 0000 0019 5368 6f77  .<..........Show
-0000a600: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
-0000a610: 2050 6565 7207 0000 000e 5065 6572 4c69   Peer.....PeerLi
-0000a620: 7374 4469 616c 6f67 0103 0000 0010 041e  stDialog........
-0000a630: 043f 0435 0440 0430 0446 0438 0438 0800  .?.5.@.0.F.8.8..
-0000a640: 0000 0006 0000 000a 4f70 6572 6174 696f  ........Operatio
-0000a650: 6e73 0700 0000 0a50 6565 7252 6570 6f72  ns.....PeerRepor
-0000a660: 7401 0300 0000 1c04 3f04 3e00 2004 1a04  t.......?.>. ...
-0000a670: 3e04 3d04 4204 4004 3004 3304 3504 3d04  >.=.B.@.0.3.5.=.
-0000a680: 4204 4308 0000 0000 0600 0000 0762 7920  B.C..........by 
-0000a690: 5065 6572 0700 0000 0a50 6565 7252 6570  Peer.....PeerRep
-0000a6a0: 6f72 7401 0300 0000 1604 1a04 3e04 3d04  ort.........>.=.
-0000a6b0: 4204 4004 3004 3304 3504 3d04 4200 3a08  B.@.0.3.5.=.B.:.
-0000a6c0: 0000 0000 0600 0000 0550 6565 723a 0700  .........Peer:..
-0000a6d0: 0000 1050 6565 7252 6570 6f72 7457 6964  ...PeerReportWid
-0000a6e0: 6765 7401 0300 0000 2804 1e04 4204 4704  get.....(...B.G.
-0000a6f0: 3504 4200 2004 3f04 3e00 2004 3a04 3e04  5.B. .?.>. .:.>.
-0000a700: 3d04 4204 4004 3004 3304 3504 3d04 4204  =.B.@.0.3.5.=.B.
-0000a710: 4308 0000 0000 0600 0000 0e52 6570 6f72  C..........Repor
-0000a720: 7420 6279 2070 6565 7207 0000 0010 5065  t by peer.....Pe
-0000a730: 6572 5265 706f 7274 5769 6467 6574 0103  erReportWidget..
-0000a740: 0000 0016 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
-0000a750: 0020 0434 043e 043a 002e 0800 0000 0006  . .4.>.:........
-0000a760: 0000 000a 446f 6373 2063 6f75 6e74 0700  ....Docs count..
-0000a770: 0000 0d50 6565 7254 7265 654d 6f64 656c  ...PeerTreeModel
-0000a780: 0103 0000 000a 0410 0434 0440 0435 0441  .........4.@.5.A
-0000a790: 0800 0000 0006 0000 0008 4c6f 6361 7469  ..........Locati
-0000a7a0: 6f6e 0700 0000 0d50 6565 7254 7265 654d  on.....PeerTreeM
-0000a7b0: 6f64 656c 0103 0000 0018 041d 0430 0438  odel.........0.8
-0000a7c0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
-0000a7d0: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
-0000a7e0: 0700 0000 0d50 6565 7254 7265 654d 6f64  .....PeerTreeMod
-0000a7f0: 656c 0103 0000 001a 0421 0447 0435 0442  el.......!.G.5.B
-0000a800: 0430 0020 0432 0020 0431 0430 043d 043a  .0. .2. .1.0.=.:
-0000a810: 0435 0800 0000 0006 0000 000d 4261 6e6b  .5..........Bank
-0000a820: 2061 6363 6f75 6e74 7307 0000 0016 5072   accounts.....Pr
-0000a830: 6564 6566 696e 6465 6441 6363 6f75 6e74  edefindedAccount
-0000a840: 5479 7065 0103 0000 000a 041a 0430 0440  Type.........0.@
-0000a850: 0442 044b 0800 0000 0006 0000 0005 4361  .B.K..........Ca
-0000a860: 7264 7307 0000 0016 5072 6564 6566 696e  rds.....Predefin
-0000a870: 6465 6441 6363 6f75 6e74 5479 7065 0103  dedAccountType..
-0000a880: 0000 0010 041d 0430 043b 0438 0447 043d  .......0.;.8.G.=
-0000a890: 044b 0435 0800 0000 0006 0000 0004 4361  .K.5..........Ca
-0000a8a0: 7368 0700 0000 1650 7265 6465 6669 6e64  sh.....Predefind
-0000a8b0: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
-0000a8c0: 0000 1e04 1a04 4004 3504 3404 3804 4204  ......@.5.4.8.B.
-0000a8d0: 4b00 2000 2f00 2004 1404 3e04 3b04 3304  K. ./. ...>.;.3.
-0000a8e0: 3808 0000 0000 0600 0000 0d44 6562 7473  8..........Debts
-0000a8f0: 202f 204c 6f61 6e73 0700 0000 1650 7265   / Loans.....Pre
-0000a900: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
-0000a910: 7970 6501 0300 0000 1404 1804 3d04 3204  ype.........=.2.
-0000a920: 3504 4104 4204 3804 4604 3804 3808 0000  5.A.B.8.F.8.8...
-0000a930: 0000 0600 0000 0b49 6e76 6573 746d 656e  .......Investmen
-0000a940: 7473 0700 0000 1650 7265 6465 6669 6e64  ts.....Predefind
-0000a950: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
-0000a960: 0000 1404 2104 3104 3504 4004 3504 3604  ....!.1.5.@.5.6.
-0000a970: 3504 3d04 3804 4f08 0000 0000 0600 0000  5.=.8.O.........
-0000a980: 0753 6176 696e 6773 0700 0000 1650 7265  .Savings.....Pre
-0000a990: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
-0000a9a0: 7970 6501 0300 0000 1400 6500 2d04 1a04  ype.......e.-...
-0000a9b0: 3e04 4804 3504 3b04 4c04 3a04 3808 0000  >.H.5.;.L.:.8...
-0000a9c0: 0000 0600 0000 0965 2d57 616c 6c65 7473  .......e-Wallets
-0000a9d0: 0700 0000 1650 7265 6465 6669 6e64 6564  .....Predefinded
-0000a9e0: 4163 636f 756e 7454 7970 6501 0300 0000  AccountType.....
-0000a9f0: 1204 1e04 3104 3b04 3804 3304 3004 4604  ....1.;.8.3.0.F.
-0000aa00: 3804 3808 0000 0000 0600 0000 0542 6f6e  8.8..........Bon
-0000aa10: 6473 0700 0000 0f50 7265 6465 6669 6e65  ds.....Predefine
-0000aa20: 6441 7373 6574 0103 0000 000c 0422 043e  dAsset.......".>
-0000aa30: 0432 0430 0440 044b 0800 0000 0006 0000  .2.0.@.K........
-0000aa40: 000b 436f 6d6d 6f64 6974 6965 7307 0000  ..Commodities...
-0000aa50: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
-0000aa60: 7401 0300 0000 1804 1a04 4004 3804 3f04  t.........@.8.?.
-0000aa70: 4204 3e04 3204 3004 3b04 4e04 4204 4b08  B.>.2.0.;.N.B.K.
-0000aa80: 0000 0000 0600 0000 0f43 7279 7074 6f2d  .........Crypto-
-0000aa90: 6375 7272 656e 6379 0700 0000 0f50 7265  currency.....Pre
-0000aaa0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
-0000aab0: 0014 0414 0435 0440 0438 0432 0430 0442  .....5.@.8.2.0.B
-0000aac0: 0438 0432 044b 0800 0000 0006 0000 000b  .8.2.K..........
-0000aad0: 4465 7269 7661 7469 7665 7307 0000 000f  Derivatives.....
-0000aae0: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
-0000aaf0: 0300 0000 0804 1104 1f04 1804 2408 0000  ............$...
-0000ab00: 0000 0600 0000 0445 5446 7307 0000 000f  .......ETFs.....
-0000ab10: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
-0000ab20: 0300 0000 0c04 2404 3e04 4004 3504 3a04  ......$.>.@.5.:.
-0000ab30: 4108 0000 0000 0600 0000 0546 6f72 6578  A..........Forex
-0000ab40: 0700 0000 0f50 7265 6465 6669 6e65 6441  .....PredefinedA
-0000ab50: 7373 6574 0103 0000 000a 0424 043e 043d  sset.......$.>.=
-0000ab60: 0434 044b 0800 0000 0006 0000 0005 4675  .4.K..........Fu
-0000ab70: 6e64 7307 0000 000f 5072 6564 6566 696e  nds.....Predefin
-0000ab80: 6564 4173 7365 7401 0300 0000 0c04 1204  edAsset.........
-0000ab90: 3004 3b04 4e04 4204 4b08 0000 0000 0600  0.;.N.B.K.......
-0000aba0: 0000 054d 6f6e 6579 0700 0000 0f50 7265  ...Money.....Pre
-0000abb0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
-0000abc0: 000a 0410 043a 0446 0438 0438 0800 0000  .....:.F.8.8....
-0000abd0: 0006 0000 0006 5368 6172 6573 0700 0000  ......Shares....
-0000abe0: 0f50 7265 6465 6669 6e65 6441 7373 6574  .PredefinedAsset
-0000abf0: 0103 0000 0002 0025 0800 0000 0006 0000  .......%........
-0000ac00: 0001 2507 0000 000f 5072 6f66 6974 4c6f  ..%.....ProfitLo
-0000ac10: 7373 4d6f 6465 6c01 0300 0000 0604 1004  ssModel.........
-0000ac20: 3f04 4008 0000 0000 0600 0000 0341 7072  ?.@..........Apr
-0000ac30: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
-0000ac40: 6f64 656c 0103 0000 0004 0426 0411 0800  odel.......&....
-0000ac50: 0000 0006 0000 0006 4173 7365 7473 0700  ........Assets..
-0000ac60: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
-0000ac70: 656c 0103 0000 0006 0410 0432 0433 0800  el.........2.3..
-0000ac80: 0000 0006 0000 0003 4175 6707 0000 000f  ........Aug.....
-0000ac90: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
-0000aca0: 0300 0000 1204 1804 3704 3c04 3504 3d04  ........7.<.5.=.
-0000acb0: 3504 3d04 3804 3508 0000 0000 0600 0000  5.=.8.5.........
-0000acc0: 0643 6861 6e67 6507 0000 000f 5072 6f66  .Change.....Prof
-0000acd0: 6974 4c6f 7373 4d6f 6465 6c01 0300 0000  itLossModel.....
-0000ace0: 1804 1804 3704 3c04 3504 3d04 3504 3d04  ....7.<.5.=.5.=.
-0000acf0: 3804 3500 2c00 2000 2508 0000 0000 0600  8.5.,. .%.......
-0000ad00: 0000 0943 6861 6e67 652c 2025 0700 0000  ...Change, %....
-0000ad10: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000ad20: 0103 0000 0006 0414 0435 043a 0800 0000  .........5.:....
-0000ad30: 0006 0000 0003 4465 6307 0000 000f 5072  ......Dec.....Pr
-0000ad40: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000ad50: 0000 1204 1404 3804 3204 3804 3404 3504  ......8.2.8.4.5.
-0000ad60: 3d04 3404 4b08 0000 0000 0600 0000 0944  =.4.K..........D
-0000ad70: 6976 6964 656e 6473 0700 0000 0f50 726f  ividends.....Pro
-0000ad80: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
-0000ad90: 0006 0424 0435 0432 0800 0000 0006 0000  ...$.5.2........
-0000ada0: 0003 4665 6207 0000 000f 5072 6f66 6974  ..Feb.....Profit
-0000adb0: 4c6f 7373 4d6f 6465 6c01 0300 0000 1004  LossModel.......
-0000adc0: 1a04 3e04 3c04 3804 4104 4104 3804 3808  ..>.<.8.A.A.8.8.
-0000add0: 0000 0000 0600 0000 0446 6565 7307 0000  .........Fees...
-0000ade0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000adf0: 6c01 0300 0000 1804 1204 3204 3e04 3400  l.........2.>.4.
-0000ae00: 2000 2f00 2004 1204 4b04 3204 3e04 3408   ./. ...K.2.>.4.
-0000ae10: 0000 0000 0600 0000 0849 6e20 2f20 4f75  .........In / Ou
-0000ae20: 7407 0000 000f 5072 6f66 6974 4c6f 7373  t.....ProfitLoss
-0000ae30: 4d6f 6465 6c01 0300 0000 0604 2f04 3d04  Model......./.=.
-0000ae40: 3208 0000 0000 0600 0000 034a 616e 0700  2..........Jan..
-0000ae50: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
-0000ae60: 656c 0103 0000 0006 0418 044e 043b 0800  el.........N.;..
-0000ae70: 0000 0006 0000 0003 4a75 6c07 0000 000f  ........Jul.....
-0000ae80: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
-0000ae90: 0300 0000 0604 1804 4e04 3d08 0000 0000  ........N.=.....
-0000aea0: 0600 0000 034a 756e 0700 0000 0f50 726f  .....Jun.....Pro
-0000aeb0: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
-0000aec0: 0006 041c 0430 0440 0800 0000 0006 0000  .....0.@........
-0000aed0: 0003 4d61 7207 0000 000f 5072 6f66 6974  ..Mar.....Profit
-0000aee0: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
-0000aef0: 1c04 3004 3908 0000 0000 0600 0000 034d  ..0.9..........M
-0000af00: 6179 0700 0000 0f50 726f 6669 744c 6f73  ay.....ProfitLos
-0000af10: 734d 6f64 656c 0103 0000 0004 0414 0421  sModel.........!
-0000af20: 0800 0000 0006 0000 0005 4d6f 6e65 7907  ..........Money.
-0000af30: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
-0000af40: 6465 6c01 0300 0000 0604 1d04 3e04 4f08  del.........>.O.
-0000af50: 0000 0000 0600 0000 034e 6f76 0700 0000  .........Nov....
-0000af60: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000af70: 0103 0000 0006 041e 043a 0442 0800 0000  .........:.B....
-0000af80: 0006 0000 0003 4f63 7407 0000 000f 5072  ......Oct.....Pr
-0000af90: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
-0000afa0: 0000 0604 1f04 3804 2308 0000 0000 0600  ......8.#.......
-0000afb0: 0000 0350 264c 0700 0000 0f50 726f 6669  ...P&L.....Profi
-0000afc0: 744c 6f73 734d 6f64 656c 0103 0000 000c  tLossModel......
-0000afd0: 041f 0435 0440 0438 043e 0434 0800 0000  ...5.@.8.>.4....
-0000afe0: 0006 0000 0006 5065 7269 6f64 0700 0000  ......Period....
-0000aff0: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
-0000b000: 0103 0000 001a 041a 043e 043d 0435 0446  .........>.=.5.F
-0000b010: 0020 043f 0435 0440 0438 043e 0434 0430  . .?.5.@.8.>.4.0
-0000b020: 0800 0000 0006 0000 000a 5065 7269 6f64  ..........Period
-0000b030: 2065 6e64 0700 0000 0f50 726f 6669 744c   end.....ProfitL
-0000b040: 6f73 734d 6f64 656c 0103 0000 001c 041d  ossModel........
-0000b050: 0430 0447 0430 043b 043e 0020 043f 0435  .0.G.0.;.>. .?.5
-0000b060: 0440 0438 043e 0434 0430 0800 0000 0006  .@.8.>.4.0......
-0000b070: 0000 000c 5065 7269 6f64 2073 7461 7274  ....Period start
-0000b080: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
-0000b090: 6f64 656c 0103 0000 0006 0421 0435 043d  odel.......!.5.=
-0000b0a0: 0800 0000 0006 0000 0003 5365 7007 0000  ..........Sep...
-0000b0b0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
-0000b0c0: 6c01 0300 0000 0c04 1d04 3004 3b04 3e04  l.........0.;.>.
-0000b0d0: 3304 3808 0000 0000 0600 0000 0554 6178  3.8..........Tax
-0000b0e0: 6573 0700 0000 0f50 726f 6669 744c 6f73  es.....ProfitLos
-0000b0f0: 734d 6f64 656c 0103 0000 000a 0418 0442  sModel.........B
-0000b100: 043e 0433 043e 0800 0000 0006 0000 0005  .>.3.>..........
-0000b110: 546f 7461 6c07 0000 000f 5072 6f66 6974  Total.....Profit
-0000b120: 4c6f 7373 4d6f 6465 6c01 0300 0000 1804  LossModel.......
-0000b130: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
-0000b140: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
-0000b150: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
-0000b160: 0000 0010 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
-0000b170: 706f 7274 0103 0000 000a 0421 0447 0435  port.......!.G.5
-0000b180: 0442 003a 0800 0000 0006 0000 0008 4163  .B.:..........Ac
-0000b190: 636f 756e 743a 0700 0000 1650 726f 6669  count:.....Profi
-0000b1a0: 744c 6f73 7352 6570 6f72 7457 6964 6765  tLossReportWidge
-0000b1b0: 7401 0300 0000 1004 1204 3004 3b04 4e04  t.........0.;.N.
-0000b1c0: 4204 3000 3a00 2008 0000 0000 0600 0000  B.0.:. .........
-0000b1d0: 0a43 7572 7265 6e63 793a 2007 0000 0016  .Currency: .....
-0000b1e0: 5072 6f66 6974 4c6f 7373 5265 706f 7274  ProfitLossReport
-0000b1f0: 5769 6467 6574 0103 0000 0006 041f 0438  Widget.........8
-0000b200: 0423 0800 0000 0006 0000 0003 5026 4c07  .#..........P&L.
-0000b210: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
-0000b220: 706f 7274 5769 6467 6574 0103 0000 0018  portWidget......
-0000b230: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
-0000b240: 044c 002e 002e 002e 0800 0000 0006 0000  .L..............
-0000b250: 0007 5361 7665 2e2e 2e07 0000 0016 5072  ..Save........Pr
-0000b260: 6f66 6974 4c6f 7373 5265 706f 7274 5769  ofitLossReportWi
-0000b270: 6467 6574 0103 0000 0010 0412 0430 043b  dget.........0.;
-0000b280: 044e 0442 0430 003a 0020 0800 0000 0006  .N.B.0.:. ......
-0000b290: 0000 000a 4375 7272 656e 6379 3a20 0700  ....Currency: ..
-0000b2a0: 0000 1650 726f 6669 744c 6f73 7352 6570  ...ProfitLossRep
-0000b2b0: 6f72 7457 696e 646f 7701 0300 0000 1804  ortWindow.......
-0000b2c0: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
-0000b2d0: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
-0000b2e0: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
-0000b2f0: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
-0000b300: 706f 7274 5769 6e64 6f77 0103 0000 001e  portWindow......
-0000b310: 041e 0448 0438 0431 043a 0430 0020 043a  ...H.8.1.:.0. .:
-0000b320: 0430 043c 0435 0440 044b 003a 0020 0800  .0.<.5.@.K.:. ..
-0000b330: 0000 0006 0000 000e 4361 6d65 7261 2065  ........Camera e
-0000b340: 7272 6f72 3a20 0700 0000 0951 5253 6361  rror: .....QRSca
-0000b350: 6e6e 6572 0103 0000 0084 041d 0435 0020  nner.........5. 
-0000b360: 043e 0431 043d 0430 0440 0443 0436 0435  .>.1.=.0.@.C.6.5
-0000b370: 043d 0020 043f 0430 043a 0435 0442 0020  .=. .?.0.:.5.B. 
-0000b380: 0070 0079 007a 0062 0061 0072 002c 0020  .p.y.z.b.a.r.,. 
-0000b390: 043d 0435 043e 0431 0445 043e 0434 0438  .=.5.>.1.E.>.4.8
-0000b3a0: 043c 044b 0439 0020 0434 043b 044f 0020  .<.K.9. .4.;.O. 
-0000b3b0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
-0000b3c0: 0432 0430 043d 0438 044f 0020 0051 0052  .2.0.=.8.O. .Q.R
-0000b3d0: 0020 043a 043e 0434 043e 0432 002e 0800  . .:.>.4.>.2....
-0000b3e0: 0000 0006 0000 002c 5061 636b 6167 6520  .......,Package 
-0000b3f0: 7079 7a62 6172 206e 6f74 2066 6f75 6e64  pyzbar not found
-0000b400: 2066 6f72 2051 5220 7265 636f 676e 6974   for QR recognit
-0000b410: 696f 6e2e 0700 0000 0951 5253 6361 6e6e  ion......QRScann
-0000b420: 6572 0103 0000 0026 041d 0435 0442 0020  er.....&...5.B. 
-0000b430: 0434 043e 0441 0442 0443 043f 043d 044b  .4.>.A.B.C.?.=.K
-0000b440: 0445 0020 043a 0430 043c 0435 0440 0800  .E. .:.0.<.5.@..
-0000b450: 0000 0006 0000 001e 5468 6572 6520 6172  ........There ar
-0000b460: 6520 6e6f 2063 616d 6572 6173 2061 7661  e no cameras ava
-0000b470: 696c 6162 6c65 0700 0000 0951 5253 6361  ilable.....QRSca
-0000b480: 6e6e 6572 0103 0000 0068 041d 0435 0432  nner.....h...5.2
-0000b490: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-0000b4a0: 043e 0431 0440 0430 0431 043e 0442 0430  .>.1.@.0.1.>.B.0
-0000b4b0: 0442 044c 0020 0434 0430 043d 043d 044b  .B.L. .4.0.=.=.K
-0000b4c0: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
-0000b4d0: 0432 043e 043a 0020 0441 0020 0431 0438  .2.>.:. .A. .1.8
-0000b4e0: 0440 0436 0438 0020 0054 0053 0058 003a  .@.6.8. .T.S.X.:
-0000b4f0: 0020 0800 0000 0006 0000 0021 4361 6e27  . .........!Can'
-0000b500: 7420 7061 7273 6520 6461 7461 2066 6f72  t parse data for
-0000b510: 2054 5358 2071 756f 7465 733a 2007 0000   TSX quotes: ...
-0000b520: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
-0000b530: 7201 0300 0000 2404 1704 3004 3304 4004  r.....$...0.3.@.
-0000b540: 4304 3704 3a04 3000 2004 3704 3004 3204  C.7.:.0. .7.0.2.
-0000b550: 3504 4004 4804 3504 3d04 3008 0000 0000  5.@.H.5.=.0.....
-0000b560: 0600 0000 1244 6f77 6e6c 6f61 6420 636f  .....Download co
-0000b570: 6d70 6c65 7465 6407 0000 000f 5175 6f74  mpleted.....Quot
-0000b580: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
-0000b590: 6000 4900 5300 4900 4e00 2004 3200 2004  `.I.S.I.N. .2. .
-0000b5a0: 3804 4104 4204 3e04 4004 3804 3800 2004  8.A.B.>.@.8.8. .
-0000b5b0: 3a04 3e04 4204 3804 4004 3e04 3204 3e04  :.>.B.8.@.>.2.>.
-0000b5c0: 3a00 2000 4500 7500 7200 6f00 6e00 6500  :. .E.u.r.o.n.e.
-0000b5d0: 7800 7400 2004 3d04 3500 2004 4104 3e04  x.t. .=.5. .A.>.
-0000b5e0: 3204 3f04 3004 3404 3004 3504 4200 3a00  2.?.0.4.0.5.B.:.
-0000b5f0: 2008 0000 0000 0600 0000 2245 7572 6f6e   ........."Euron
-0000b600: 6578 7420 7175 6f74 6573 2049 5349 4e20  ext quotes ISIN 
-0000b610: 6d69 736d 6174 6368 2069 6e3a 2007 0000  mismatch in: ...
-0000b620: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
-0000b630: 7201 0300 0000 6404 1704 3004 3304 3e04  r.....d...0.3.>.
-0000b640: 3b04 3e04 3204 3e04 3a00 2004 3804 4104  ;.>.2.>.:. .8.A.
-0000b650: 4204 3e04 4004 3804 3800 2004 3a04 3e04  B.>.@.8.8. .:.>.
-0000b660: 4204 3804 4004 3e04 3204 3e04 3a00 2000  B.8.@.>.2.>.:. .
-0000b670: 4500 7500 7200 6f00 6e00 6500 7800 7400  E.u.r.o.n.e.x.t.
-0000b680: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
-0000b690: 3504 3d00 2004 3200 3a00 2008 0000 0000  5.=. .2.:. .....
-0000b6a0: 0600 0000 2545 7572 6f6e 6578 7420 7175  ....%Euronext qu
-0000b6b0: 6f74 6573 2068 6561 6465 7220 6e6f 7420  otes header not 
-0000b6c0: 666f 756e 6420 696e 3a20 0700 0000 0f51  found in: .....Q
-0000b6d0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
-0000b6e0: 0000 005a 0418 0441 0442 043e 0440 0438  ...Z...A.B.>.@.8
-0000b6f0: 044f 0020 043a 043e 0442 0438 0440 043e  .O. .:.>.B.8.@.>
-0000b700: 0432 043e 043a 0020 0045 0075 0072 006f  .2.>.:. .E.u.r.o
-0000b710: 006e 0065 0078 0074 0020 0441 043b 0438  .n.e.x.t. .A.;.8
-0000b720: 0448 043a 043e 043c 0020 043a 043e 0440  .H.:.>.<. .:.>.@
-0000b730: 043e 0442 043a 0430 044f 003a 0020 0800  .>.B.:.0.O.:. ..
-0000b740: 0000 0006 0000 002c 4575 726f 6e65 7874  .......,Euronext
-0000b750: 2071 756f 7465 7320 6869 7374 6f72 7920   quotes history 
-0000b760: 7265 706c 7920 6973 2074 6f6f 2073 686f  reply is too sho
-0000b770: 7274 3a20 0700 0000 0f51 756f 7465 446f  rt: .....QuoteDo
-0000b780: 776e 6c6f 6164 6572 0103 0000 0036 041d  wnloader.....6..
-0000b790: 0435 0020 0437 0430 0433 0440 0443 0436  .5. .7.0.3.@.C.6
-0000b7a0: 0435 043d 044b 0020 043a 043e 0442 0438  .5.=.K. .:.>.B.8
-0000b7b0: 0440 043e 0432 043a 0438 0020 0434 043b  .@.>.2.:.8. .4.;
-0000b7c0: 044f 0020 0800 0000 0006 0000 001e 4e6f  .O. ..........No
-0000b7d0: 2071 756f 7465 7320 7765 7265 2064 6f77   quotes were dow
-0000b7e0: 6e6c 6f61 6465 6420 666f 7220 0700 0000  nloaded for ....
-0000b7f0: 0f51 756f 7465 446f 776e 6c6f 6164 6572  .QuoteDownloader
-0000b800: 0103 0000 002e 041d 0435 0020 0437 0430  .........5. .7.0
-0000b810: 0433 0440 0443 0436 0435 043d 044b 0020  .3.@.C.6.5.=.K. 
-0000b820: 043a 0443 0440 0441 044b 0020 0434 043b  .:.C.@.A.K. .4.;
-0000b830: 044f 0020 0800 0000 0006 0000 001d 4e6f  .O. ..........No
-0000b840: 2072 6174 6573 2077 6572 6520 646f 776e   rates were down
-0000b850: 6c6f 6164 6564 2066 6f72 2007 0000 000f  loaded for .....
-0000b860: 5175 6f74 6544 6f77 6e6c 6f61 6465 7201  QuoteDownloader.
-0000b870: 0300 0000 2c04 1d04 3504 4200 2004 3404  ....,...5.B. .4.
-0000b880: 3004 3d04 3d04 4b04 4500 2004 2604 1100  0.=.=.K.E. .&...
-0000b890: 2004 2004 2400 2004 3404 3b04 4f00 3a00   . .$. .4.;.O.:.
-0000b8a0: 2008 0000 0000 0600 0000 1b54 6865 7265   ..........There
-0000b8b0: 2061 7265 206e 6f20 4342 5220 6461 7461   are no CBR data
-0000b8c0: 2066 6f72 3a20 0700 0000 0f51 756f 7465   for: .....Quote
-0000b8d0: 446f 776e 6c6f 6164 6572 0103 0000 0012  Downloader......
-0000b8e0: 041a 043e 0442 0438 0440 043e 0432 043a  ...>.B.8.@.>.2.:
-0000b8f0: 0438 0800 0000 0006 0000 0006 5175 6f74  .8..........Quot
-0000b900: 6573 0700 0000 1051 756f 7465 734c 6973  es.....QuotesLis
-0000b910: 7444 6961 6c6f 6701 0300 0000 0404 2604  tDialog.......&.
-0000b920: 1108 0000 0000 0600 0000 0541 7373 6574  ...........Asset
-0000b930: 0700 0000 0f51 756f 7465 734c 6973 744d  .....QuotesListM
-0000b940: 6f64 656c 0103 0000 000c 0412 0430 043b  odel.........0.;
-0000b950: 044e 0442 0430 0800 0000 0006 0000 0008  .N.B.0..........
-0000b960: 4375 7272 656e 6379 0700 0000 0f51 756f  Currency.....Quo
-0000b970: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
-0000b980: 0008 0414 0430 0442 0430 0800 0000 0006  .....0.B.0......
-0000b990: 0000 0004 4461 7465 0700 0000 0f51 756f  ....Date.....Quo
-0000b9a0: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
-0000b9b0: 0012 041a 043e 0442 0438 0440 043e 0432  .....>.B.8.@.>.2
-0000b9c0: 043a 0430 0800 0000 0006 0000 0005 5175  .:.0..........Qu
-0000b9d0: 6f74 6507 0000 000f 5175 6f74 6573 4c69  ote.....QuotesLi
-0000b9e0: 7374 4d6f 6465 6c01 0300 0000 2800 2604  stModel.....(.&.
-0000b9f0: 1f04 3e04 3b04 3d04 3e04 4104 4204 4c04  ..>.;.=.>.A.B.L.
-0000ba00: 4e00 2c00 2004 4100 2004 3d04 3004 4704  N.,. .A. .=.0.G.
-0000ba10: 3004 3b04 3008 0000 0000 0600 0000 1326  0.;.0..........&
-0000ba20: 4675 6c6c 2c20 6672 6f6d 2073 6372 6174  Full, from scrat
-0000ba30: 6368 0700 0000 0d52 6542 7569 6c64 4469  ch.....ReBuildDi
-0000ba40: 616c 6f67 0103 0000 0018 0418 043d 0442  alog.........=.B
-0000ba50: 0435 0440 0432 0430 043b 0020 0434 0430  .5.@.2.0.;. .4.0
-0000ba60: 0442 0800 0000 0006 0000 000a 4461 7465  .B..........Date
-0000ba70: 2052 616e 6765 0700 0000 0d52 6542 7569   Range.....ReBui
-0000ba80: 6c64 4469 616c 6f67 0103 0000 002a 0026  ldDialog.....*.&
-0000ba90: 0411 044b 0441 0442 0440 043e 002c 0020  ...K.A.B.@.>.,. 
-0000baa0: 043d 043e 0020 043d 0435 043d 0430 0434  .=.>. .=.5.=.0.4
-0000bab0: 0451 0436 043d 043e 0800 0000 0006 0000  .Q.6.=.>........
-0000bac0: 0011 4661 7374 2c20 2675 6e72 656c 6961  ..Fast, &unrelia
-0000bad0: 626c 6507 0000 000d 5265 4275 696c 6444  ble.....ReBuildD
-0000bae0: 6961 6c6f 6701 0300 0000 1604 1404 3004  ialog.........0.
-0000baf0: 4204 3004 1304 4004 3004 3d04 3804 4604  B.0...@.0.=.8.F.
-0000bb00: 4b08 0000 0000 0600 0000 0c46 726f 6e74  K..........Front
-0000bb10: 6965 7244 6174 6507 0000 000d 5265 4275  ierDate.....ReBu
-0000bb20: 696c 6444 6961 6c6f 6701 0300 0000 2204  ildDialog.....".
-0000bb30: 1f04 3504 4004 3504 4104 4704 3804 4204  ..5.@.5.A.G.8.B.
-0000bb40: 3004 4204 4c00 2004 3804 4204 3e04 3304  0.B.L. .8.B.>.3.
-0000bb50: 3808 0000 0000 0600 0000 0f52 652d 4275  8..........Re-Bu
-0000bb60: 696c 6420 4c65 6467 6572 0700 0000 0d52  ild Ledger.....R
-0000bb70: 6542 7569 6c64 4469 616c 6f67 0103 0000  eBuildDialog....
-0000bb80: 0010 0421 0020 0026 0414 0430 0442 044b  ...!. .&...0.B.K
-0000bb90: 003a 0800 0000 0006 0000 000c 5369 6e63  .:..........Sinc
-0000bba0: 6520 2644 6174 653a 0700 0000 0d52 6542  e &Date:.....ReB
-0000bbb0: 7569 6c64 4469 616c 6f67 0103 0000 002c  uildDialog.....,
-0000bbc0: 0421 0020 043a 0440 0430 0439 043d 0435  .!. .:.@.0.9.=.5
-0000bbd0: 0439 0020 0026 0430 043a 0442 0443 0430  .9. .&.0.:.B.C.0
-0000bbe0: 043b 044c 043d 043e 0439 003a 0800 0000  .;.L.=.>.9.:....
-0000bbf0: 0006 0000 0013 5369 6e63 6520 264c 6173  ......Since &Las
-0000bc00: 7420 6163 7475 616c 3a07 0000 000d 5265  t actual:.....Re
-0000bc10: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
-0000bc20: 1400 6400 6400 2f00 4d00 4d00 2f00 7900  ..d.d./.M.M./.y.
-0000bc30: 7900 7900 7908 0000 0000 0600 0000 0a64  y.y.y..........d
-0000bc40: 642f 4d4d 2f79 7979 7907 0000 000d 5265  d/MM/yyyy.....Re
-0000bc50: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
-0000bc60: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
-0000bc70: 0600 0000 0341 4e59 0700 0000 1352 6566  .....ANY.....Ref
-0000bc80: 6572 656e 6365 4461 7461 4469 616c 6f67  erenceDataDialog
-0000bc90: 0103 0000 0014 0422 0438 043f 0020 0441  .......".8.?. .A
-0000bca0: 0447 0435 0442 0430 003a 0800 0000 0006  .G.5.B.0.:......
-0000bcb0: 0000 000d 4163 636f 756e 7420 5479 7065  ....Account Type
-0000bcc0: 3a07 0000 0013 5265 6665 7265 6e63 6544  :.....ReferenceD
-0000bcd0: 6174 6144 6961 6c6f 6701 0300 0000 2204  ataDialog.....".
-0000bce0: 1404 3e04 3104 3004 3204 3804 4204 4c00  ..>.1.0.2.8.B.L.
-0000bcf0: 2004 3404 3e04 4704 3504 4004 3d04 3804   .4.>.G.5.@.=.8.
-0000bd00: 3908 0000 0000 0600 0000 0941 6464 2063  9..........Add c
-0000bd10: 6869 6c64 0700 0000 1352 6566 6572 656e  hild.....Referen
-0000bd20: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
-0000bd30: 001c 0414 043e 0431 0430 0432 0438 0442  .....>.1.0.2.8.B
-0000bd40: 044c 0020 043d 043e 0432 044b 0439 0800  .L. .=.>.2.K.9..
-0000bd50: 0000 0006 0000 0007 4164 6420 6e65 7707  ........Add new.
-0000bd60: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
-0000bd70: 6144 6961 6c6f 6701 0300 0000 1e04 2104  aDialog.......!.
-0000bd80: 3c04 3504 3d04 3804 4204 4c00 2004 4204  <.5.=.8.B.L. .B.
-0000bd90: 3804 3f00 2004 3d04 3000 3a08 0000 0000  8.?. .=.0.:.....
-0000bda0: 0600 0000 0f43 6861 6e67 6520 7479 7065  .....Change type
-0000bdb0: 2074 6f3a 0700 0000 1352 6566 6572 656e   to:.....Referen
-0000bdc0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
-0000bdd0: 001a 041f 043e 0434 0442 0432 0435 0440  .....>.4.B.2.5.@
-0000bde0: 0436 0434 0435 043d 0438 0435 0800 0000  .6.4.5.=.8.5....
-0000bdf0: 0006 0000 000c 436f 6e66 6972 6d61 7469  ......Confirmati
-0000be00: 6f6e 0700 0000 1352 6566 6572 656e 6365  on.....Reference
-0000be10: 4461 7461 4469 616c 6f67 0103 0000 000e  DataDialog......
-0000be20: 0423 0434 0430 043b 0438 0442 044c 0800  .#.4.0.;.8.B.L..
-0000be30: 0000 0006 0000 0006 4465 6c65 7465 0700  ........Delete..
-0000be40: 0000 1352 6566 6572 656e 6365 4461 7461  ...ReferenceData
-0000be50: 4469 616c 6f67 0103 0000 0022 0421 043f  Dialog.....".!.?
-0000be60: 0440 0430 0432 043e 0447 043d 044b 0435  .@.0.2.>.G.=.K.5
-0000be70: 0020 0434 0430 043d 043d 044b 0435 0800  . .4.0.=.=.K.5..
-0000be80: 0000 0006 0000 000e 5265 6665 7265 6e63  ........Referenc
-0000be90: 6520 4461 7461 0700 0000 1352 6566 6572  e Data.....Refer
-0000bea0: 656e 6365 4461 7461 4469 616c 6f67 0103  enceDataDialog..
-0000beb0: 0000 0024 041e 0442 043c 0435 043d 0438  ...$...B.<.5.=.8
-0000bec0: 0442 044c 0020 0438 0437 043c 0435 043d  .B.L. .8.7.<.5.=
-0000bed0: 0435 043d 0438 044f 0800 0000 0006 0000  .5.=.8.O........
-0000bee0: 000e 5265 7665 7274 2063 6861 6e67 6573  ..Revert changes
-0000bef0: 0700 0000 1352 6566 6572 656e 6365 4461  .....ReferenceDa
-0000bf00: 7461 4469 616c 6f67 0103 0000 0026 0421  taDialog.....&.!
-0000bf10: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
-0000bf20: 0020 0438 0437 043c 0435 043d 0435 043d  . .8.7.<.5.=.5.=
-0000bf30: 0438 044f 0800 0000 0006 0000 000c 5361  .8.O..........Sa
-0000bf40: 7665 2063 6861 6e67 6573 0700 0000 1352  ve changes.....R
-0000bf50: 6566 6572 656e 6365 4461 7461 4469 616c  eferenceDataDial
-0000bf60: 6f67 0103 0000 000c 041f 043e 0438 0441  og.........>.8.A
-0000bf70: 043a 003a 0800 0000 0006 0000 0007 5365  .:.:..........Se
-0000bf80: 6172 6368 3a07 0000 0013 5265 6665 7265  arch:.....Refere
-0000bf90: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000bfa0: 0000 2a04 1f04 3e04 3a04 3004 3704 4b04  ..*...>.:.0.7.K.
-0000bfb0: 3204 3004 4204 4c00 2004 3d04 3504 3004  2.0.B.L. .=.5.0.
-0000bfc0: 3a04 4204 3804 3204 3d04 4b04 3508 0000  :.B.8.2.=.K.5...
-0000bfd0: 0000 0600 0000 0d53 686f 7720 696e 6163  .......Show inac
-0000bfe0: 7469 7665 0700 0000 1352 6566 6572 656e  tive.....Referen
-0000bff0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
-0000c000: 0066 0423 0020 0432 0430 0441 0020 0435  .f.#. .2.0.A. .5
-0000c010: 0441 0442 044c 0020 043d 0435 0441 043e  .A.B.L. .=.5.A.>
-0000c020: 0445 0440 0430 043d 0451 043d 043d 044b  .E.@.0.=.Q.=.=.K
-0000c030: 0435 0020 0434 0430 043d 043d 044b 0435  .5. .4.0.=.=.K.5
-0000c040: 002e 0020 0412 0441 0451 0020 0440 0430  ... ...A.Q. .@.0
-0000c050: 0432 043d 043e 0020 0437 0430 043a 0440  .2.=.>. .7.0.:.@
-0000c060: 044b 0442 044c 003f 0800 0000 0006 0000  .K.B.L.?........
-0000c070: 0033 596f 7520 6861 7665 2075 6e63 6f6d  .3You have uncom
-0000c080: 6d69 7474 6564 2063 6861 6e67 6573 2e20  mitted changes. 
-0000c090: 446f 2079 6f75 2077 616e 7420 746f 2063  Do you want to c
-0000c0a0: 6c6f 7365 3f07 0000 0013 5265 6665 7265  lose?.....Refere
-0000c0b0: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
-0000c0c0: 0000 0604 1004 3f04 4008 0000 0000 0600  ......?.@.......
-0000c0d0: 0000 0341 7072 0700 0000 0e52 6570 6f72  ...Apr.....Repor
-0000c0e0: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
-0000c0f0: 1004 3204 3308 0000 0000 0600 0000 0341  ..2.3..........A
-0000c100: 7567 0700 0000 0e52 6570 6f72 7454 7265  ug.....ReportTre
-0000c110: 6549 7465 6d01 0300 0000 0604 1404 3504  eItem.........5.
-0000c120: 3a08 0000 0000 0600 0000 0344 6563 0700  :..........Dec..
-0000c130: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
-0000c140: 6d01 0300 0000 0604 2404 3504 3208 0000  m.......$.5.2...
-0000c150: 0000 0600 0000 0346 6562 0700 0000 0e52  .......Feb.....R
-0000c160: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
-0000c170: 0000 0604 2f04 3d04 3208 0000 0000 0600  ..../.=.2.......
-0000c180: 0000 034a 616e 0700 0000 0e52 6570 6f72  ...Jan.....Repor
-0000c190: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
-0000c1a0: 1804 4e04 3b08 0000 0000 0600 0000 034a  ..N.;..........J
-0000c1b0: 756c 0700 0000 0e52 6570 6f72 7454 7265  ul.....ReportTre
-0000c1c0: 6549 7465 6d01 0300 0000 0604 1804 4e04  eItem.........N.
-0000c1d0: 3d08 0000 0000 0600 0000 034a 756e 0700  =..........Jun..
-0000c1e0: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
-0000c1f0: 6d01 0300 0000 0604 1c04 3004 4008 0000  m.........0.@...
-0000c200: 0000 0600 0000 034d 6172 0700 0000 0e52  .......Mar.....R
-0000c210: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
-0000c220: 0000 0604 1c04 3004 3908 0000 0000 0600  ......0.9.......
-0000c230: 0000 034d 6179 0700 0000 0e52 6570 6f72  ...May.....Repor
-0000c240: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
-0000c250: 1d04 3e04 4f08 0000 0000 0600 0000 034e  ..>.O..........N
-0000c260: 6f76 0700 0000 0e52 6570 6f72 7454 7265  ov.....ReportTre
-0000c270: 6549 7465 6d01 0300 0000 0604 1e04 3a04  eItem.........:.
-0000c280: 4208 0000 0000 0600 0000 034f 6374 0700  B..........Oct..
-0000c290: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
-0000c2a0: 6d01 0300 0000 0604 2104 3504 3d08 0000  m.......!.5.=...
-0000c2b0: 0000 0600 0000 0353 6570 0700 0000 0e52  .......Sep.....R
-0000c2c0: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
-0000c2d0: 0000 0604 3d04 3504 3408 0000 0000 0600  ....=.5.4.......
-0000c2e0: 0000 0277 6b07 0000 000e 5265 706f 7274  ...wk.....Report
-0000c2f0: 5472 6565 4974 656d 0103 0000 0028 0424  TreeItem.....(.$
-0000c300: 0430 0439 043b 044b 0020 0045 0078 0063  .0.9.;.K. .E.x.c
-0000c310: 0065 006c 0020 0028 002a 002e 0078 0073  .e.l. .(.*...x.s
-0000c320: 006c 0078 0029 0800 0000 0006 0000 0014  .l.x.)..........
-0000c330: 4578 6365 6c20 6669 6c65 7320 282a 2e78  Excel files (*.x
-0000c340: 6c73 7829 0700 0000 0752 6570 6f72 7473  lsx).....Reports
-0000c350: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
-0000c360: 043c 043e 0436 043d 043e 0020 0437 0430  .<.>.6.=.>. .7.0
-0000c370: 0433 0440 0443 0437 0438 0442 044c 0020  .3.@.C.7.8.B.L. 
-0000c380: 043a 043b 0430 0441 0441 0020 043e 0442  .:.;.0.A.A. .>.B
-0000c390: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
-0000c3a0: 0006 0000 001e 5265 706f 7274 2063 6c61  ......Report cla
-0000c3b0: 7373 2063 616e 2774 2062 6520 6c6f 6164  ss can't be load
-0000c3c0: 6564 3a20 0700 0000 0752 6570 6f72 7473  ed: .....Reports
-0000c3d0: 0103 0000 0042 041e 0442 0447 0435 0442  .....B...B.G.5.B
-0000c3e0: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
-0000c3f0: 0435 043d 0020 0434 043b 044f 0020 043a  .5.=. .4.;.O. .:
-0000c400: 043b 0430 0441 0441 0430 0020 043e 043a  .;.0.A.A.0. .>.:
-0000c410: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
-0000c420: 0023 5265 706f 7274 206e 6f74 2066 6f75  .#Report not fou
-0000c430: 6e64 2066 6f72 2077 696e 646f 7720 636c  nd for window cl
-0000c440: 6173 733a 2007 0000 0007 5265 706f 7274  ass: .....Report
-0000c450: 7301 0300 0000 2c04 1e04 4204 4704 3504  s.....,...B.G.5.
-0000c460: 4200 2004 4104 3e04 4504 4004 3004 3d04  B. .A.>.E.@.0.=.
-0000c470: 5104 3d00 2004 3200 2004 4404 3004 3904  Q.=. .2. .D.0.9.
-0000c480: 3b00 2008 0000 0000 0600 0000 1952 6570  ;. ..........Rep
-0000c490: 6f72 7420 7761 7320 7361 7665 6420 746f  ort was saved to
-0000c4a0: 2066 696c 6520 0700 0000 0752 6570 6f72   file .....Repor
-0000c4b0: 7473 0103 0000 0024 0421 043e 0445 0440  ts.....$.!.>.E.@
-0000c4c0: 0430 043d 0438 0442 044c 0020 043e 0442  .0.=.8.B.L. .>.B
-0000c4d0: 0447 0435 0442 0020 0432 003a 0800 0000  .G.5.B. .2.:....
-0000c4e0: 0006 0000 000f 5361 7665 2072 6570 6f72  ......Save repor
-0000c4f0: 7420 746f 3a07 0000 0007 5265 706f 7274  t to:.....Report
-0000c500: 7301 0300 0000 3c04 1b04 3e04 3304 3804  s.....<...>.3.8.
-0000c510: 3d00 2004 4704 3504 4004 3504 3700 2004  =. .G.5.@.5.7. .
-0000c520: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
-0000c530: 3800 2004 3704 3004 3204 3504 4004 4804  8. .7.0.2.5.@.H.
-0000c540: 5104 3d08 0000 0000 0600 0000 1445 5349  Q.=..........ESI
-0000c550: 4120 6c6f 6769 6e20 636f 6d70 6c65 7465  A login complete
-0000c560: 6407 0000 0012 5265 7175 6573 7449 6e74  d.....RequestInt
-0000c570: 6572 6365 7074 6f72 0103 0000 000a 0410  erceptor........
-0000c580: 043a 0442 0438 0432 0800 0000 0006 0000  .:.B.8.2........
-0000c590: 0005 4173 7365 7407 0000 000c 5265 7375  ..Asset.....Resu
-0000c5a0: 6c74 734d 6f64 656c 0103 0000 000c 041a  ltsModel........
-0000c5b0: 043e 043b 002d 0432 043e 0800 0000 0006  .>.;.-.2.>......
-0000c5c0: 0000 0003 5174 7907 0000 000c 5265 7375  ....Qty.....Resu
-0000c5d0: 6c74 734d 6f64 656c 0103 0000 000e 0414  ltsModel........
-0000c5e0: 043e 043b 044f 002c 0020 0025 0800 0000  .>.;.O.,. .%....
-0000c5f0: 0006 0000 0008 5368 6172 652c 2025 0700  ......Share, %..
-0000c600: 0000 0c52 6573 756c 7473 4d6f 6465 6c01  ...ResultsModel.
-0000c610: 0300 0000 3004 1204 4b04 3104 4004 3004  ....0...K.1.@.0.
-0000c620: 3d00 2004 3d04 3504 3a04 3e04 4004 4004  =. .=.5.:.>.@.@.
-0000c630: 3504 3a04 4204 3d04 4b04 3900 2004 4104  5.:.B.=.K.9. .A.
-0000c640: 4704 5104 4208 0000 0000 0600 0000 1849  G.Q.B..........I
-0000c650: 6e76 616c 6964 2061 6363 6f75 6e74 2073  nvalid account s
-0000c660: 656c 6563 7465 6407 0000 0013 5365 6c65  elected.....Sele
-0000c670: 6374 4163 636f 756e 7444 6961 6c6f 6701  ctAccountDialog.
-0000c680: 0300 0000 2204 1d04 3804 4704 3504 3304  ...."...8.G.5.3.
-0000c690: 3e00 2004 3d04 3500 2004 3204 4b04 3104  >. .=.5. .2.K.1.
-0000c6a0: 4004 3004 3d04 3e08 0000 0000 0600 0000  @.0.=.>.........
-0000c6b0: 0c4e 6f20 7365 6c65 6374 696f 6e07 0000  .No selection...
-0000c6c0: 0013 5365 6c65 6374 4163 636f 756e 7444  ..SelectAccountD
-0000c6d0: 6961 6c6f 6701 0300 0000 4004 1f04 3e04  ialog.....@...>.
-0000c6e0: 3604 3004 3b04 4304 3904 4104 4204 3000  6.0.;.C.9.A.B.0.
-0000c6f0: 2c00 2004 3204 4b04 3104 3504 4004 3804  ,. .2.K.1.5.@.8.
-0000c700: 4204 3500 2004 3404 4004 4304 3304 3e04  B.5. .4.@.C.3.>.
-0000c710: 3900 2004 4104 4704 5104 4208 0000 0000  9. .A.G.Q.B.....
-0000c720: 0600 0000 1f50 6c65 6173 6520 7365 6c65  .....Please sele
-0000c730: 6374 2064 6966 6665 7265 6e74 2061 6363  ct different acc
-0000c740: 6f75 6e74 0700 0000 1353 656c 6563 7441  ount.....SelectA
-0000c750: 6363 6f75 6e74 4469 616c 6f67 0103 0000  ccountDialog....
-0000c760: 0030 041f 043e 0436 0430 043b 0443 0439  .0...>.6.0.;.C.9
-0000c770: 0441 0442 0430 0020 0432 044b 0431 0435  .A.B.0. .2.K.1.5
-0000c780: 0440 0438 0442 0435 0020 0441 0447 0451  .@.8.B.5. .A.G.Q
-0000c790: 0442 0800 0000 0006 0000 0015 506c 6561  .B..........Plea
-0000c7a0: 7365 2073 656c 6563 7420 6163 636f 756e  se select accoun
-0000c7b0: 7407 0000 0010 5365 6c65 6374 4163 636f  t.....SelectAcco
-0000c7c0: 756e 7444 6c67 0103 0000 0012 0421 043e  untDlg.......!.>
-0000c7d0: 043e 0431 0449 0435 043d 0438 0435 0800  .>.1.I.5.=.8.5..
-0000c7e0: 0000 0006 0000 0009 5465 7874 4c61 6265  ........TextLabe
-0000c7f0: 6c07 0000 0010 5365 6c65 6374 4163 636f  l.....SelectAcco
-0000c800: 756e 7444 6c67 0103 0000 0056 0418 0441  untDlg.....V...A
-0000c810: 043f 043e 043b 044c 0437 043e 0432 0430  .?.>.;.L.7.>.2.0
-0000c820: 0442 044c 0020 044d 0442 043e 0442 0020  .B.L. .M.B.>.B. 
-0000c830: 0436 0435 0020 0441 0447 0451 0442 0020  .6.5. .A.G.Q.B. 
-0000c840: 0434 043b 044f 0020 0434 0430 043d 043d  .4.;.O. .4.0.=.=
-0000c850: 043e 0439 0020 0432 0430 043b 044e 0442  .>.9. .2.0.;.N.B
-0000c860: 044b 0800 0000 0006 0000 0027 5573 6520  .K.........'Use 
-0000c870: 7468 6520 7361 6d65 2061 6363 6f75 6e74  the same account
-0000c880: 2066 6f72 2067 6976 656e 2063 7572 7265   for given curre
-0000c890: 6e63 7907 0000 0010 5365 6c65 6374 4163  ncy.....SelectAc
-0000c8a0: 636f 756e 7444 6c67 0103 0000 0024 0412  countDlg.....$..
-0000c8b0: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
-0000c8c0: 043a 0430 0442 0435 0433 043e 0440 0438  .:.0.B.5.3.>.@.8
-0000c8d0: 044e 0800 0000 0006 0000 0016 506c 6561  .N..........Plea
-0000c8e0: 7365 2073 656c 6563 7420 6361 7465 676f  se select catego
-0000c8f0: 7279 0700 0000 1453 656c 6563 7443 6174  ry.....SelectCat
-0000c900: 6567 6f72 7944 6961 6c6f 6701 0300 0000  egoryDialog.....
-0000c910: 2804 1204 4b04 3104 3504 4004 3804 4204  (...K.1.5.@.8.B.
-0000c920: 3500 2004 3a04 3e04 3d04 4204 4004 3004  5. .:.>.=.B.@.0.
-0000c930: 3304 3504 3d04 4204 3008 0000 0000 0600  3.5.=.B.0.......
-0000c940: 0000 1250 6c65 6173 6520 7365 6c65 6374  ...Please select
-0000c950: 2070 6565 7207 0000 0010 5365 6c65 6374   peer.....Select
-0000c960: 5065 6572 4469 616c 6f67 0103 0000 0022  PeerDialog....."
-0000c970: 041d 0438 0447 0435 0433 043e 0020 043d  ...8.G.5.3.>. .=
-0000c980: 0435 0020 0432 044b 0431 0440 0430 043d  .5. .2.K.1.@.0.=
-0000c990: 043e 0800 0000 0006 0000 000c 4e6f 2073  .>..........No s
-0000c9a0: 656c 6563 7469 6f6e 0700 0000 1553 656c  election.....Sel
-0000c9b0: 6563 7452 6566 6572 656e 6365 4469 616c  ectReferenceDial
-0000c9c0: 6f67 0103 0000 002e 0412 044b 0020 0434  og.........K. .4
-0000c9d0: 043e 043b 0436 043d 044b 0020 0441 0434  .>.;.6.=.K. .A.4
-0000c9e0: 0435 043b 0430 0442 044c 0020 0432 044b  .5.;.0.B.L. .2.K
-0000c9f0: 0431 043e 0440 0800 0000 0006 0000 001b  .1.>.@..........
-0000ca00: 596f 7520 7368 6f75 6c64 2073 656c 6563  You should selec
-0000ca10: 7420 736f 6d65 7468 696e 6707 0000 0015  t something.....
-0000ca20: 5365 6c65 6374 5265 6665 7265 6e63 6544  SelectReferenceD
-0000ca30: 6961 6c6f 6701 0300 0000 1c04 1204 4b04  ialog.........K.
-0000ca40: 3104 3504 4004 3804 4204 3500 2004 3c04  1.5.@.8.B.5. .<.
-0000ca50: 3504 4204 3a04 4308 0000 0000 0600 0000  5.B.:.C.........
-0000ca60: 1150 6c65 6173 6520 7365 6c65 6374 2074  .Please select t
-0000ca70: 6167 0700 0000 0f53 656c 6563 7454 6167  ag.....SelectTag
-0000ca80: 4469 616c 6f67 0103 0000 005a 041d 0435  Dialog.....Z...5
-0000ca90: 0020 0443 0434 0430 043b 043e 0441 044c  . .C.4.0.;.>.A.L
-0000caa0: 0020 043f 043e 043b 0443 0447 0438 0442  . .?.>.;.C.G.8.B
-0000cab0: 044c 0020 043d 0430 0437 0432 0430 043d  .L. .=.0.7.2.0.=
-0000cac0: 0438 0435 0020 043e 0433 0440 0430 043d  .8.5. .>.3.@.0.=
-0000cad0: 0438 0437 0430 0446 0438 0438 0020 0438  .8.7.0.F.8.8. .8
-0000cae0: 0437 003a 0020 0800 0000 0006 0000 001d  .7.:. ..........
-0000caf0: 4361 6e27 7420 6765 7420 636f 6d70 616e  Can't get compan
-0000cb00: 7920 6e61 6d65 2066 726f 6d3a 2007 0000  y name from: ...
-0000cb10: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
-0000cb20: 0000 4804 1d04 3504 3204 3e04 3704 3c04  ..H...5.2.>.7.<.
-0000cb30: 3e04 3604 3d04 3e00 2004 3e04 3104 3204  >.6.=.>. .>.1.2.
-0000cb40: 3d04 3e04 3204 3804 4204 4c00 2004 4104  =.>.2.8.B.L. .A.
-0000cb50: 3504 4104 4104 3804 4e00 2c00 2004 3e04  5.A.A.8.N.,. .>.
-0000cb60: 4204 3204 3504 4200 3a00 2008 0000 0000  B.2.5.B.:. .....
-0000cb70: 0600 0000 2143 616e 2774 2072 6566 7265  ....!Can't refre
-0000cb80: 7368 2073 6573 7369 6f6e 2c20 7265 7370  sh session, resp
-0000cb90: 6f6e 7365 3a20 0700 0000 0b53 6c69 7073  onse: .....Slips
-0000cba0: 5461 7841 5049 0103 0000 002e 041e 0448  TaxAPI.........H
-0000cbb0: 0438 0431 043a 0430 0020 043f 043e 043b  .8.1.:.0. .?.>.;
-0000cbc0: 0443 0447 0435 043d 0438 044f 0020 0447  .C.G.5.=.8.O. .G
-0000cbd0: 0435 043a 0430 003a 0020 0800 0000 0006  .5.:.0.:. ......
-0000cbe0: 0000 0013 4765 7420 7469 636b 6574 2066  ....Get ticket f
-0000cbf0: 6169 6c65 643a 2007 0000 000b 536c 6970  ailed: .....Slip
-0000cc00: 7354 6178 4150 4901 0300 0000 3404 1e04  sTaxAPI.....4...
-0000cc10: 4804 3804 3104 3a04 3000 2004 3f04 3e04  H.8.1.:.0. .?.>.
-0000cc20: 3b04 4304 4704 3504 3d04 3804 4f00 2000  ;.C.G.5.=.8.O. .
-0000cc30: 6900 6400 2004 4704 3504 3a04 3000 3a00  i.d. .G.5.:.0.:.
-0000cc40: 2008 0000 0000 0600 0000 1647 6574 2074   ..........Get t
-0000cc50: 6963 6b65 7420 6964 2066 6169 6c65 643a  icket id failed:
-0000cc60: 2007 0000 000b 536c 6970 7354 6178 4150   .....SlipsTaxAP
-0000cc70: 4901 0300 0000 7c04 1d04 3504 3204 3504  I.....|...5.2.5.
-0000cc80: 4004 3d04 3004 4f00 2004 3404 3b04 3804  @.=.0.O. .4.;.8.
-0000cc90: 3d04 3000 2004 1804 1d04 1d00 2e00 2004  =.0. ......... .
-0000cca0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-0000ccb0: 3d04 3e00 2004 3f04 3e04 3b04 4304 4704  =.>. .?.>.;.C.G.
-0000ccc0: 3804 4204 4c00 2004 3d04 3004 3804 3c04  8.B.L. .=.0.8.<.
-0000ccd0: 3504 3d04 3e04 3204 3004 3d04 3804 3500  5.=.>.2.0.=.8.5.
-0000cce0: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
-0000ccf0: 3800 2e08 0000 0000 0600 0000 3049 6e63  8...........0Inc
-0000cd00: 6f72 7265 6374 206c 656e 6774 6820 6f66  orrect length of
-0000cd10: 2049 4e4e 2e20 4361 6e27 7420 6765 7420   INN. Can't get 
-0000cd20: 636f 6d70 616e 7920 6e61 6d65 2e07 0000  company name....
-0000cd30: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
-0000cd40: 0000 5604 1d04 3504 4200 2000 5300 6500  ..V...5.B. .S.e.
-0000cd50: 7300 7300 6900 6f00 6e00 4900 6400 2004  s.s.i.o.n.I.d. .
-0000cd60: 3404 3b04 4f00 2004 3704 3004 3304 4004  4.;.O. .7.0.3.@.
-0000cd70: 4304 3704 3a04 3800 2004 4704 3504 3a04  C.7.:.8. .G.5.:.
-0000cd80: 3000 2004 4100 2004 4104 3004 3904 4204  0. .A. .A.0.9.B.
-0000cd90: 3000 2004 2404 1d04 2108 0000 0000 0600  0. .$...!.......
-0000cda0: 0000 224e 6f20 5275 7373 6961 6e20 5461  .."No Russian Ta
-0000cdb0: 7820 5365 7373 696f 6e49 6420 6176 6169  x SessionId avai
-0000cdc0: 6c61 626c 6507 0000 000b 536c 6970 7354  lable.....SlipsT
-0000cdd0: 6178 4150 4901 0300 0000 3604 1d04 3504  axAPI.....6...5.
-0000cde0: 4200 2004 3004 3a04 4204 3804 3204 3d04  B. .0.:.B.8.2.=.
-0000cdf0: 3e04 3900 2004 4104 3504 4104 4104 3804  >.9. .A.5.A.A.8.
-0000ce00: 3800 2004 3404 3b04 4f00 2004 2404 1d04  8. .4.;.O. .$...
-0000ce10: 2108 0000 0000 0600 0000 184e 6f20 7661  !..........No va
-0000ce20: 6c69 6420 7365 7373 696f 6e20 7072 6573  lid session pres
-0000ce30: 656e 7407 0000 000b 536c 6970 7354 6178  ent.....SlipsTax
-0000ce40: 4150 4901 0300 0000 7a04 1e04 3f04 3504  API.....z...?.5.
-0000ce50: 4004 3004 4604 3804 4f00 2004 3e04 3104  @.0.F.8.O. .>.1.
-0000ce60: 4004 3004 3104 3004 4204 4b04 3204 3004  @.0.1.0.B.K.2.0.
-0000ce70: 3504 4204 4104 4f00 2004 3d04 3000 2004  5.B.A.O. .=.0. .
-0000ce80: 4104 4204 3e04 4004 3e04 3d04 3500 2004  A.B.>.@.>.=.5. .
-0000ce90: 4104 3504 4004 3204 3504 4004 3000 2e00  A.5.@.2.5.@.0...
-0000cea0: 2004 1f04 3e04 3204 4204 3e04 4004 4f04   ...>.2.B.>.@.O.
-0000ceb0: 4e00 2004 3504 4904 5100 2004 4004 3004  N. .5.I.Q. .@.0.
-0000cec0: 3700 2e08 0000 0000 0600 0000 384f 7065  7...........8Ope
-0000ced0: 7261 7469 6f6e 206d 6967 6874 2062 6520  ration might be 
-0000cee0: 7065 6e64 696e 6720 6f6e 2073 6572 7665  pending on serve
-0000cef0: 7220 7369 6465 2e20 5472 7969 6e67 2061  r side. Trying a
-0000cf00: 6761 696e 2e07 0000 000b 536c 6970 7354  gain......SlipsT
-0000cf10: 6178 4150 4901 0300 0000 2804 1e04 3104  axAPI.....(...1.
-0000cf20: 3d04 3e04 3204 3b04 3504 3d04 3804 3500  =.>.2.;.5.=.8.5.
-0000cf30: 2004 4104 3504 4104 4104 3804 3800 2e00   .A.5.A.A.8.8...
-0000cf40: 2e00 2e08 0000 0000 0600 0000 1552 6566  .............Ref
-0000cf50: 7265 7368 696e 6720 7365 7373 696f 6e2e  reshing session.
-0000cf60: 2e2e 0700 0000 0b53 6c69 7073 5461 7841  .......SlipsTaxA
-0000cf70: 5049 0103 0000 0024 0421 0435 0441 0441  PI.....$.!.5.A.A
-0000cf80: 0438 044f 0020 043e 0431 043d 043e 0432  .8.O. .>.1.=.>.2
-0000cf90: 043b 0435 043d 0430 003a 0020 0800 0000  .;.5.=.0.:. ....
-0000cfa0: 0006 0000 0013 5365 7373 696f 6e20 7265  ......Session re
-0000cfb0: 6672 6573 6865 643a 2007 0000 000b 536c  freshed: .....Sl
-0000cfc0: 6970 7354 6178 4150 4901 0300 0000 1804  ipsTaxAPI.......
-0000cfd0: 2704 3504 3a00 2004 3d04 3004 3904 3404  '.5.:. .=.0.9.4.
-0000cfe0: 3504 3d00 3a00 2008 0000 0000 0600 0000  5.=.:. .........
-0000cff0: 0c53 6c69 7020 666f 756e 643a 2007 0000  .Slip found: ...
-0000d000: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
-0000d010: 0000 1c04 2704 3504 3a00 2004 3704 3004  ....'.5.:. .7.0.
-0000d020: 3304 4004 4304 3604 3504 3d00 3a00 2008  3.@.C.6.5.=.:. .
-0000d030: 0000 0000 0600 0000 0d53 6c69 7020 6c6f  .........Slip lo
-0000d040: 6164 6564 3a20 0700 0000 0b53 6c69 7073  aded: .....Slips
-0000d050: 5461 7841 5049 0103 0000 0036 041d 0435  TaxAPI.....6...5
-0000d060: 0430 0432 0442 043e 0440 0438 0437 043e  .0.2.B.>.@.8.7.>
-0000d070: 0432 0430 043d 043e 0020 043f 043e 0020  .2.0.=.>. .?.>. 
-0000d080: 043f 0440 0438 0447 0438 043d 0435 003a  .?.@.8.G.8.=.5.:
-0000d090: 0020 0800 0000 0006 0000 001a 556e 6175  . ..........Unau
-0000d0a0: 7468 6f72 697a 6564 2077 6974 6820 7265  thorized with re
-0000d0b0: 6173 6f6e 3a20 0700 0000 0b53 6c69 7073  ason: .....Slips
-0000d0c0: 5461 7841 5049 0103 0000 001c 0421 0447  TaxAPI.......!.G
-0000d0d0: 0451 0442 0020 043d 0435 0020 0432 044b  .Q.B. .=.5. .2.K
-0000d0e0: 0431 0440 0430 043d 0800 0000 0006 0000  .1.@.0.=........
-0000d0f0: 0014 4163 636f 756e 7420 6e6f 7420 7365  ..Account not se
-0000d100: 6c65 6374 6564 0700 0000 0953 7461 7465  lected.....State
-0000d110: 6d65 6e74 0103 0000 0034 0414 0430 043d  ment.....4...0.=
-0000d120: 043d 044b 0435 0020 043d 0435 0020 043f  .=.K.5. .=.5. .?
-0000d130: 0440 0438 0432 044f 0437 0430 043d 044b  .@.8.2.O.7.0.=.K
-0000d140: 0020 043a 0020 0426 0411 003a 0020 0800  . .:. .&...:. ..
-0000d150: 0000 0006 0000 0023 4173 7365 7420 6461  .......#Asset da
-0000d160: 7461 2061 7265 6e27 7420 6c69 6e6b 6564  ta aren't linked
-0000d170: 2074 6f20 6173 7365 743a 2007 0000 0009   to asset: .....
-0000d180: 5374 6174 656d 656e 7401 0300 0000 1e04  Statement.......
-0000d190: 2604 1100 2000 6900 6400 2004 3d04 3500  &... .i.d. .=.5.
-0000d1a0: 2004 3d04 3004 3904 3404 3504 3d08 0000   .=.0.9.4.5.=...
-0000d1b0: 0000 0600 0000 1241 7373 6574 2069 6420  .......Asset id 
-0000d1c0: 6e6f 7420 666f 756e 6407 0000 0009 5374  not found.....St
-0000d1d0: 6174 656d 656e 7401 0300 0000 3204 1d04  atement.....2...
-0000d1e0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-0000d1f0: 3e00 2004 4104 3e04 3704 3404 3004 4204  >. .A.>.7.4.0.B.
-0000d200: 4c00 2004 4104 4704 5104 4200 3a00 2008  L. .A.G.Q.B.:. .
-0000d210: 0000 0000 0600 0000 1643 616e 2774 2063  .........Can't c
-0000d220: 7265 6174 6520 6163 636f 756e 743a 2007  reate account: .
-0000d230: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000d240: 0000 2e04 1d04 3504 3204 3e04 3704 3c04  ......5.2.>.7.<.
-0000d250: 3e04 3604 3d04 3e00 2004 4104 3e04 3704  >.6.=.>. .A.>.7.
-0000d260: 3404 3004 4204 4c00 2004 2604 1100 3a00  4.0.B.L. .&...:.
-0000d270: 2008 0000 0000 0600 0000 1443 616e 2774   ..........Can't
-0000d280: 2063 7265 6174 6520 6173 7365 743a 2007   create asset: .
-0000d290: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000d2a0: 0000 3c04 1d04 3504 3204 3e04 3704 3c04  ..<...5.2.>.7.<.
-0000d2b0: 3e04 3604 3d04 3e00 2004 3d04 3004 3904  >.6.=.>. .=.0.9.
-0000d2c0: 4204 3500 2004 2604 1100 2004 3200 2004  B.5. .&... .2. .
-0000d2d0: 3e04 4204 4704 5104 4204 3500 3a00 2008  >.B.G.Q.B.5.:. .
-0000d2e0: 0000 0000 0600 0000 2643 616e 2774 206c  ........&Can't l
-0000d2f0: 6f63 6174 6520 6173 7365 7420 696e 2073  ocate asset in s
-0000d300: 7461 7465 6d65 6e74 2064 6174 613a 2007  tatement data: .
-0000d310: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000d320: 0000 1a04 1f04 3e04 3404 4204 3204 3504  ......>.4.B.2.5.
-0000d330: 4004 3604 3404 3504 3d04 3804 3508 0000  @.6.4.5.=.8.5...
-0000d340: 0000 0600 0000 0c43 6f6e 6669 726d 6174  .......Confirmat
-0000d350: 696f 6e07 0000 0009 5374 6174 656d 656e  ion.....Statemen
-0000d360: 7401 0300 0000 4404 1e04 4204 3b04 3004  t.....D...B.;.0.
-0000d370: 3404 3e04 4704 3d04 3004 4f00 2004 3804  4.>.G.=.0.O. .8.
-0000d380: 3d04 4404 3e04 4004 3c04 3004 4604 3804  =.D.>.@.<.0.F.8.
-0000d390: 4f00 2004 4104 3e04 4504 4004 3004 3d04  O. .A.>.E.@.0.=.
-0000d3a0: 3504 3d04 3000 2004 3200 2008 0000 0000  5.=.0. .2. .....
-0000d3b0: 0600 0000 1e44 6562 7567 2069 6e66 6f72  .....Debug infor
-0000d3c0: 6d61 7469 6f6e 2069 7320 7361 7665 6420  mation is saved 
-0000d3d0: 696e 2007 0000 0009 5374 6174 656d 656e  in .....Statemen
-0000d3e0: 7401 0300 0000 1004 1404 3504 3f04 3e04  t.........5.?.>.
-0000d3f0: 3704 3804 4200 2008 0000 0000 0600 0000  7.8.B. .........
-0000d400: 0b44 6570 6f73 6974 206f 6620 0700 0000  .Deposit of ....
-0000d410: 0953 7461 7465 6d65 6e74 0103 0000 0048  .Statement.....H
-0000d420: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000d430: 043d 043e 0020 043f 0440 043e 0447 0438  .=.>. .?.@.>.G.8
-0000d440: 0442 0430 0442 044c 0020 004a 0053 004f  .B.0.B.L. .J.S.O
-0000d450: 004e 0020 0438 0437 0020 0444 0430 0439  .N. .8.7. .D.0.9
-0000d460: 043b 0430 003a 0020 0800 0000 0006 0000  .;.0.:. ........
-0000d470: 001f 4661 696c 6564 2074 6f20 7265 6164  ..Failed to read
-0000d480: 204a 534f 4e20 6672 6f6d 2066 696c 653a   JSON from file:
-0000d490: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
-0000d4a0: 0300 0000 4804 1d04 3500 2004 4304 3404  ....H...5. .C.4.
-0000d4b0: 3004 3b04 3e04 4104 4c00 2004 3f04 4004  0.;.>.A.L. .?.@.
-0000d4c0: 3e04 4704 3804 4204 3004 4204 4c00 2004  >.G.8.B.0.B.L. .
-0000d4d0: 4104 4504 3504 3c04 4300 2000 4a00 5300  A.E.5.<.C. .J.S.
-0000d4e0: 4f00 4e00 2004 3804 3700 3a00 2008 0000  O.N. .8.7.:. ...
-0000d4f0: 0000 0600 0000 2146 6169 6c65 6420 746f  ......!Failed to
-0000d500: 2072 6561 6420 4a53 4f4e 2073 6368 656d   read JSON schem
-0000d510: 6120 6672 6f6d 3a20 0700 0000 0953 7461  a from: .....Sta
-0000d520: 7465 6d65 6e74 0103 0000 0034 041d 0435  tement.....4...5
-0000d530: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-0000d540: 0020 043f 0440 043e 0447 0435 0441 0442  . .?.@.>.G.5.A.B
-0000d550: 044c 0020 0444 0430 0439 043b 003a 0020  .L. .D.0.9.;.:. 
-0000d560: 0800 0000 0006 0000 0015 4661 696c 6564  ..........Failed
-0000d570: 2074 6f20 7265 6164 2066 696c 653a 2007   to read file: .
-0000d580: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000d590: 0000 5a04 1e04 4804 3804 3104 3a04 3000  ..Z...H.8.1.:.0.
-0000d5a0: 2004 3f04 4004 3800 2004 4104 3e04 4504   .?.@.8. .A.>.E.
-0000d5b0: 4004 3004 3d04 3504 3d04 3804 3800 2004  @.0.=.5.=.8.8. .
-0000d5c0: 3e04 4204 3b04 3004 3404 3e04 4704 3d04  >.B.;.0.4.>.G.=.
-0000d5d0: 3e04 3900 2004 3804 3d04 4404 3e04 4004  >.9. .8.=.D.>.@.
-0000d5e0: 3c04 3004 4604 3804 3800 3a00 2008 0000  <.0.F.8.8.:. ...
-0000d5f0: 0000 0600 0000 2546 6169 6c65 6420 746f  ......%Failed to
-0000d600: 2077 7269 7465 2073 7461 7465 6d65 6e74   write statement
-0000d610: 2064 756d 7020 696e 746f 3a20 0700 0000   dump into: ....
-0000d620: 0953 7461 7465 6d65 6e74 0103 0000 0066  .Statement.....f
-0000d630: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000d640: 043d 043e 0020 043a 043e 043d 0442 0432  .=.>. .:.>.=.B.2
-0000d650: 0435 0440 0442 0438 0440 043e 0432 0430  .5.@.B.8.@.>.2.0
-0000d660: 0442 044c 0020 0442 0438 043f 0020 0430  .B.L. .B.8.?. .0
-0000d670: 043a 0442 0438 0432 0430 0020 0432 0020  .:.B.8.2.0. .2. 
-0000d680: 0442 0440 0430 043d 0441 0444 0435 0440  .B.@.0.=.A.D.5.@
-0000d690: 0435 003a 0020 0800 0000 0006 0000 002e  .5.:. ..........
-0000d6a0: 496d 706f 7373 6962 6c65 2074 6f20 636f  Impossible to co
-0000d6b0: 6e76 6572 7420 6173 7365 7420 7479 7065  nvert asset type
-0000d6c0: 2069 6e20 7472 616e 7366 6572 3a20 0700   in transfer: ..
-0000d6d0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000d6e0: 0048 041d 0435 043e 0434 043d 043e 0437  .H...5.>.4.=.>.7
-0000d6f0: 043d 0430 0447 043d 043e 0435 0020 0441  .=.0.G.=.>.5. .A
-0000d700: 043e 0432 043f 0430 0434 0435 043d 0438  .>.2.?.0.4.5.=.8
-0000d710: 0435 0020 0432 0430 043b 044e 0442 044b  .5. .2.0.;.N.B.K
-0000d720: 0020 0434 043b 044f 0020 0800 0000 0006  . .4.;.O. ......
-0000d730: 0000 001c 4d75 6c74 6970 6c65 2063 7572  ....Multiple cur
-0000d740: 7265 6e63 7920 6d61 7463 6820 666f 7220  rency match for 
-0000d750: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000d760: 0000 003a 041d 0435 043e 0434 043d 043e  ...:...5.>.4.=.>
-0000d770: 0437 043d 0430 0447 043d 043e 0435 0020  .7.=.0.G.=.>.5. 
-0000d780: 0441 043e 0432 043f 0430 0434 0435 043d  .A.>.2.?.0.4.5.=
-0000d790: 0438 0435 0020 0434 043b 044f 0020 0800  .8.5. .4.;.O. ..
-0000d7a0: 0000 0006 0000 0013 4d75 6c74 6970 6c65  ........Multiple
-0000d7b0: 206d 6174 6368 2066 6f72 2007 0000 0009   match for .....
-0000d7c0: 5374 6174 656d 656e 7401 0300 0000 3a04  Statement.....:.
-0000d7d0: 1204 4b04 3104 3504 4004 3804 4204 3500  ..K.1.5.@.8.B.5.
-0000d7e0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
-0000d7f0: 4f00 2004 3704 3004 4704 3804 4104 3b04  O. .7.0.G.8.A.;.
-0000d800: 3504 3d04 3804 4f00 3a08 0000 0000 0600  5.=.8.O.:.......
-0000d810: 0000 1d53 656c 6563 7420 6163 636f 756e  ...Select accoun
-0000d820: 7420 746f 2064 6570 6f73 6974 2074 6f3a  t to deposit to:
-0000d830: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000d840: 0000 0036 0412 044b 0431 0435 0440 0438  ...6...K.1.5.@.8
-0000d850: 0442 0435 0020 0441 0447 0451 0442 0020  .B.5. .A.G.Q.B. 
-0000d860: 0434 043b 044f 0020 0441 043f 0438 0441  .4.;.O. .A.?.8.A
-0000d870: 0430 043d 0438 044f 003a 0800 0000 0006  .0.=.8.O.:......
-0000d880: 0000 0020 5365 6c65 6374 2061 6363 6f75  ... Select accou
-0000d890: 6e74 2074 6f20 7769 7468 6472 6177 2066  nt to withdraw f
-0000d8a0: 726f 6d3a 0700 0000 0953 7461 7465 6d65  rom:.....Stateme
-0000d8b0: 6e74 0103 0000 0048 041d 0435 043a 043e  nt.....H...5.:.>
-0000d8c0: 0442 043e 0440 044b 0435 0020 0441 0435  .B.>.@.K.5. .A.5
-0000d8d0: 043a 0446 0438 0438 0020 043d 0435 0020  .:.F.8.8. .=.5. 
-0000d8e0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-0000d8f0: 0432 0430 044e 0442 0441 044f 003a 0020  .2.0.N.B.A.O.:. 
-0000d900: 0800 0000 0006 0000 0021 536f 6d65 2073  .........!Some s
-0000d910: 6563 7469 6f6e 7320 6172 6520 6e6f 7420  ections are not 
-0000d920: 7375 7070 6f72 7465 643a 2007 0000 0009  supported: .....
-0000d930: 5374 6174 656d 656e 7401 0300 0000 2a04  Statement.....*.
-0000d940: 1804 3c04 3f04 3e04 4004 4200 2004 3e04  ..<.?.>.@.B. .>.
-0000d950: 4204 4704 5104 4204 3000 2004 3f04 4004  B.G.Q.B.0. .?.@.
-0000d960: 3504 4004 3204 3004 3d08 0000 0000 0600  5.@.2.0.=.......
-0000d970: 0000 1e53 7461 7465 6d65 6e74 2069 6d70  ...Statement imp
-0000d980: 6f72 7420 7761 7320 6361 6e63 656c 6c65  ort was cancelle
-0000d990: 6407 0000 0009 5374 6174 656d 656e 7401  d.....Statement.
-0000d9a0: 0300 0000 2c04 1d04 3504 3204 3504 4004  ....,...5.2.5.@.
-0000d9b0: 3d04 4b04 3900 2004 3f04 3504 4004 3804  =.K.9. .?.5.@.8.
-0000d9c0: 3e04 3400 2004 3e04 4204 4704 5104 4204  >.4. .>.B.G.Q.B.
-0000d9d0: 3008 0000 0000 0600 0000 1b53 7461 7465  0..........State
-0000d9e0: 6d65 6e74 2070 6572 696f 6420 6973 2069  ment period is i
-0000d9f0: 6e76 616c 6964 0700 0000 0953 7461 7465  nvalid.....State
-0000da00: 6d65 6e74 0103 0000 00c6 041f 0435 0440  ment.........5.@
-0000da10: 0438 043e 0434 0020 043e 0442 0447 0451  .8.>.4. .>.B.G.Q
-0000da20: 0442 0430 0020 043d 0430 0447 0438 043d  .B.0. .=.0.G.8.=
-0000da30: 0430 0435 0442 0441 044f 0020 0440 0430  .0.5.B.A.O. .@.0
-0000da40: 043d 0435 0435 0020 043f 043e 0441 043b  .=.5.5. .?.>.A.;
-0000da50: 0435 0434 043d 0435 0439 0020 043e 043f  .5.4.=.5.9. .>.?
-0000da60: 0435 0440 0430 0446 0438 0438 0020 0434  .5.@.0.F.8.8. .4
-0000da70: 043b 044f 0020 0441 0447 0451 0442 0430  .;.O. .A.G.Q.B.0
-0000da80: 0020 0028 043f 043e 0432 0442 043e 0440  . .(.?.>.2.B.>.@
-0000da90: 043d 044b 0439 0020 0438 043c 043f 043e  .=.K.9. .8.<.?.>
-0000daa0: 0440 0442 003f 0029 002e 0020 041f 0440  .@.B.?.)... ...@
-0000dab0: 043e 0434 043e 043b 0436 0438 0442 044c  .>.4.>.;.6.8.B.L
-0000dac0: 0020 0438 043c 043f 043e 0440 0442 003f  . .8.<.?.>.@.B.?
-0000dad0: 0800 0000 0006 0000 0058 5374 6174 656d  .........XStatem
-0000dae0: 656e 7420 7065 7269 6f64 2073 7461 7274  ent period start
-0000daf0: 7320 6265 666f 7265 206c 6173 7420 7265  s before last re
-0000db00: 636f 7264 6564 206f 7065 7261 7469 6f6e  corded operation
-0000db10: 2066 6f72 2074 6865 2061 6363 6f75 6e74   for the account
-0000db20: 2e20 436f 6e74 696e 7565 2069 6d70 6f72  . Continue impor
-0000db30: 743f 0700 0000 0953 7461 7465 6d65 6e74  t?.....Statement
-0000db40: 0103 0000 002a 041e 0442 0447 0451 0442  .....*...B.G.Q.B
-0000db50: 0020 0441 043e 0434 0435 0440 0436 0438  . .A.>.4.5.@.6.8
-0000db60: 0442 0020 043e 0448 0438 0431 043a 0438  .B. .>.H.8.1.:.8
-0000db70: 0800 0000 0006 0000 001b 5374 6174 656d  ..........Statem
-0000db80: 656e 7420 7661 6c69 6461 7469 6f6e 2066  ent validation f
-0000db90: 6169 6c65 6407 0000 0009 5374 6174 656d  ailed.....Statem
-0000dba0: 656e 7401 0300 0000 4004 2104 3804 3c04  ent.....@.!.8.<.
-0000dbb0: 3204 3e04 3b00 2004 3204 3004 3b04 4e04  2.>.;. .2.0.;.N.
-0000dbc0: 4204 4b00 2004 3d04 3500 2004 3f04 4004  B.K. .=.5. .?.@.
-0000dbd0: 3804 3204 4f04 3704 3004 3d00 2004 3a00  8.2.O.7.0.=. .:.
-0000dbe0: 2004 2604 1100 3a00 2008 0000 0000 0600   .&...:. .......
-0000dbf0: 0000 2753 796d 626f 6c20 6375 7272 656e  ..'Symbol curren
-0000dc00: 6379 2069 736e 2774 206c 696e 6b65 6420  cy isn't linked 
-0000dc10: 746f 2061 7373 6574 3a20 0700 0000 0953  to asset: .....S
-0000dc20: 7461 7465 6d65 6e74 0103 0000 0032 0421  tatement.....2.!
-0000dc30: 0438 043c 0432 043e 043b 0020 043d 0435  .8.<.2.>.;. .=.5
-0000dc40: 0020 043f 0440 0438 0432 044f 0437 0430  . .?.@.8.2.O.7.0
-0000dc50: 043d 0020 043a 0020 0426 0411 003a 0020  .=. .:. .&...:. 
-0000dc60: 0800 0000 0006 0000 0025 5379 6d62 6f6c  .........%Symbol
-0000dc70: 2074 6963 6b65 7220 6973 6e27 7420 6c69   ticker isn't li
-0000dc80: 6e6b 6564 2074 6f20 6173 7365 743a 2007  nked to asset: .
-0000dc90: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000dca0: 0000 7204 1d04 3504 3204 3e04 3704 3c04  ..r...5.2.>.7.<.
-0000dcb0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
-0000dcc0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
-0000dcd0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
-0000dce0: 4f00 2004 3a04 3e04 4004 3f04 3e04 4004  O. .:.>.@.?.>.@.
-0000dcf0: 3004 4204 3804 3204 3d04 3e04 3304 3e00  0.B.8.2.=.>.3.>.
-0000dd00: 2004 3404 3504 3904 4104 4204 3204 3804   .4.5.9.A.B.2.8.
-0000dd10: 4f00 3a00 2008 0000 0000 0600 0000 2855  O.:. .........(U
-0000dd20: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
-0000dd30: 2066 6f72 2063 6f72 706f 7261 7465 2061   for corporate a
-0000dd40: 6374 696f 6e3a 2007 0000 0009 5374 6174  ction: .....Stat
-0000dd50: 656d 656e 7401 0300 0000 7404 1d04 3504  ement.....t...5.
-0000dd60: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-0000dd70: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
-0000dd80: 3204 3804 4204 4c00 2004 4104 4704 5104  2.8.B.L. .A.G.Q.
-0000dd90: 4200 2004 3404 3b04 4f00 2004 3e04 3f04  B. .4.;.O. .>.?.
-0000dda0: 3504 4004 3004 4604 3804 3800 2004 3f04  5.@.0.F.8.8. .?.
-0000ddb0: 4004 3804 4504 3e04 3404 3000 2f04 4004  @.8.E.>.4.0./.@.
-0000ddc0: 3004 4104 4504 3e04 3404 3000 3a00 2008  0.A.E.>.4.0.:. .
-0000ddd0: 0000 0000 0600 0000 2755 6e6d 6174 6368  ........'Unmatch
-0000dde0: 6564 2061 6363 6f75 6e74 2066 6f72 2069  ed account for i
-0000ddf0: 6e63 6f6d 652f 7370 656e 6469 6e67 3a20  ncome/spending: 
-0000de00: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
-0000de10: 0000 0052 041d 0435 0432 043e 0437 043c  ...R...5.2.>.7.<
-0000de20: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
-0000de30: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
-0000de40: 0020 0441 0447 0451 0442 0020 0434 043b  . .A.G.Q.B. .4.;
-0000de50: 044f 0020 0432 044b 043f 043b 0430 0442  .O. .2.K.?.;.0.B
-0000de60: 044b 003a 0020 0800 0000 0006 0000 001f  .K.:. ..........
-0000de70: 556e 6d61 7463 6865 6420 6163 636f 756e  Unmatched accoun
-0000de80: 7420 666f 7220 7061 796d 656e 743a 2007  t for payment: .
-0000de90: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
-0000dea0: 0000 5004 1d04 3504 3204 3e04 3704 3c04  ..P...5.2.>.7.<.
-0000deb0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
-0000dec0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
-0000ded0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
-0000dee0: 4f00 2004 4104 3404 3504 3b04 3a04 3800  O. .A.4.5.;.:.8.
-0000def0: 3a00 2008 0000 0000 0600 0000 1d55 6e6d  :. ..........Unm
-0000df00: 6174 6368 6564 2061 6363 6f75 6e74 2066  atched account f
-0000df10: 6f72 2074 7261 6465 3a20 0700 0000 0953  or trade: .....S
-0000df20: 7461 7465 6d65 6e74 0103 0000 0054 041d  tatement.....T..
-0000df30: 0435 0432 0437 043e 043c 043e 0436 043d  .5.2.7.>.<.>.6.=
-0000df40: 043e 0020 0441 043e 043f 043e 0441 0442  .>. .A.>.?.>.A.B
-0000df50: 0430 0432 0438 0442 044c 0020 0441 0447  .0.2.8.B.L. .A.G
-0000df60: 0451 0442 0020 0434 043b 044f 0020 043f  .Q.B. .4.;.O. .?
-0000df70: 0435 0440 0435 0432 043e 0434 0430 003a  .5.@.5.2.>.4.0.:
-0000df80: 0020 0800 0000 0006 0000 0020 556e 6d61  . ......... Unma
-0000df90: 7463 6865 6420 6163 636f 756e 7420 666f  tched account fo
-0000dfa0: 7220 7472 616e 7366 6572 3a20 0700 0000  r transfer: ....
-0000dfb0: 0953 7461 7465 6d65 6e74 0103 0000 006e  .Statement.....n
-0000dfc0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000dfd0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000dfe0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
-0000dff0: 0411 0020 0434 043b 044f 0020 043a 043e  ... .4.;.O. .:.>
-0000e000: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
-0000e010: 043d 043e 0433 043e 0020 0434 0435 0439  .=.>.3.>. .4.5.9
-0000e020: 0441 0442 0432 0438 044f 003a 0020 0800  .A.B.2.8.O.:. ..
-0000e030: 0000 0006 0000 0026 556e 6d61 7463 6865  .......&Unmatche
-0000e040: 6420 6173 7365 7420 666f 7220 636f 7270  d asset for corp
-0000e050: 6f72 6174 6520 6163 7469 6f6e 3a20 0700  orate action: ..
-0000e060: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
-0000e070: 004e 041d 0435 0432 043e 0437 043c 043e  .N...5.2.>.7.<.>
-0000e080: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
-0000e090: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
-0000e0a0: 0426 0411 0020 0434 043b 044f 0020 0432  .&... .4.;.O. .2
-0000e0b0: 044b 043f 043b 0430 0442 044b 003a 0020  .K.?.;.0.B.K.:. 
-0000e0c0: 0800 0000 0006 0000 001d 556e 6d61 7463  ..........Unmatc
-0000e0d0: 6865 6420 6173 7365 7420 666f 7220 7061  hed asset for pa
-0000e0e0: 796d 656e 743a 2007 0000 0009 5374 6174  yment: .....Stat
-0000e0f0: 656d 656e 7401 0300 0000 4c04 1d04 3504  ement.....L...5.
-0000e100: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-0000e110: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
-0000e120: 3204 3804 4204 4c00 2004 2604 1100 2004  2.8.B.L. .&... .
-0000e130: 3404 3b04 4f00 2004 4104 3404 3504 3b04  4.;.O. .A.4.5.;.
-0000e140: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
-0000e150: 1b55 6e6d 6174 6368 6564 2061 7373 6574  .Unmatched asset
-0000e160: 2066 6f72 2074 7261 6465 3a20 0700 0000   for trade: ....
-0000e170: 0953 7461 7465 6d65 6e74 0103 0000 005e  .Statement.....^
-0000e180: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000e190: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
-0000e1a0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
-0000e1b0: 0411 002f 0432 0430 043b 044e 0442 0443  .../.2.0.;.N.B.C
-0000e1c0: 0020 0434 043b 044f 0020 043f 0435 0440  . .4.;.O. .?.5.@
-0000e1d0: 0435 0432 043e 0434 0430 003a 0020 0800  .5.2.>.4.0.:. ..
-0000e1e0: 0000 0006 0000 001e 556e 6d61 7463 6865  ........Unmatche
-0000e1f0: 6420 6173 7365 7420 666f 7220 7472 616e  d asset for tran
-0000e200: 7366 6572 3a20 0700 0000 0953 7461 7465  sfer: .....State
-0000e210: 6d65 6e74 0103 0000 006c 041d 0435 0432  ment.....l...5.2
-0000e220: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-0000e230: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
-0000e240: 0438 0442 044c 0020 043a 0430 0442 0435  .8.B.L. .:.0.B.5
-0000e250: 0433 043e 0440 0438 044e 0020 0434 043b  .3.>.@.8.N. .4.;
-0000e260: 044f 0020 043f 0440 0438 0445 043e 0434  .O. .?.@.8.E.>.4
-0000e270: 0430 002f 0440 0430 0441 0445 043e 0434  .0./.@.0.A.E.>.4
-0000e280: 0430 003a 0020 0800 0000 0006 0000 0028  .0.:. .........(
-0000e290: 556e 6d61 7463 6865 6420 6361 7465 676f  Unmatched catego
-0000e2a0: 7279 2066 6f72 2069 6e63 6f6d 652f 7370  ry for income/sp
-0000e2b0: 656e 6469 6e67 3a20 0700 0000 0953 7461  ending: .....Sta
-0000e2c0: 7465 6d65 6e74 0103 0000 0050 041d 0435  tement.....P...5
-0000e2d0: 0432 043e 0437 043c 043e 043d 043e 0020  .2.>.7.<.>.=.>. 
-0000e2e0: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
-0000e2f0: 0438 0442 044c 0020 0432 0430 043b 044e  .8.B.L. .2.0.;.N
-0000e300: 0442 0443 0020 0434 043b 044f 0020 0441  .B.C. .4.;.O. .A
-0000e310: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
-0000e320: 0006 0000 0020 556e 6d61 7463 6865 6420  ..... Unmatched 
-0000e330: 6375 7272 656e 6379 2066 6f72 2061 6363  currency for acc
-0000e340: 6f75 6e74 3a20 0700 0000 0953 7461 7465  ount: .....State
-0000e350: 6d65 6e74 0103 0000 0082 041d 0435 0432  ment.........5.2
-0000e360: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-0000e370: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
-0000e380: 0438 0442 044c 0020 043a 043e 043d 0442  .8.B.L. .:.>.=.B
-0000e390: 0440 0430 0433 0435 043d 0442 0430 0020  .@.0.3.5.=.B.0. 
-0000e3a0: 0434 043b 044f 0020 043e 043f 0435 0440  .4.;.O. .>.?.5.@
-0000e3b0: 0430 0446 0438 0438 0020 043f 0440 0438  .0.F.8.8. .?.@.8
-0000e3c0: 0445 043e 0434 0430 002f 0440 0430 0441  .E.>.4.0./.@.0.A
-0000e3d0: 0445 043e 0434 0430 003a 0020 0800 0000  .E.>.4.0.:. ....
-0000e3e0: 0006 0000 0024 556e 6d61 7463 6865 6420  .....$Unmatched 
-0000e3f0: 7065 6572 2066 6f72 2069 6e63 6f6d 652f  peer for income/
-0000e400: 7370 656e 6469 6e67 3a20 0700 0000 0953  spending: .....S
-0000e410: 7461 7465 6d65 6e74 0103 0000 0052 041d  tatement.....R..
-0000e420: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
-0000e430: 0438 0432 0430 0435 043c 043e 0435 0020  .8.2.0.5.<.>.5. 
-0000e440: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
-0000e450: 0438 0432 043d 043e 0435 0020 0434 0435  .8.2.=.>.5. .4.5
-0000e460: 0439 0441 0442 0432 0438 0435 003a 0020  .9.A.B.2.8.5.:. 
-0000e470: 0800 0000 0006 0000 001e 556e 7375 7070  ..........Unsupp
-0000e480: 6f72 7465 6420 636f 7270 6f72 6174 6520  orted corporate 
-0000e490: 6163 7469 6f6e 3a20 0700 0000 0953 7461  action: .....Sta
-0000e4a0: 7465 6d65 6e74 0103 0000 003c 041d 0435  tement.....<...5
-0000e4b0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
-0000e4c0: 0432 0430 0435 043c 044b 0439 0020 0442  .2.0.5.<.K.9. .B
-0000e4d0: 0438 043f 0020 0432 044b 043f 043b 0430  .8.?. .2.K.?.;.0
-0000e4e0: 0442 044b 003a 0020 0800 0000 0006 0000  .B.K.:. ........
-0000e4f0: 001a 556e 7375 7070 6f72 7465 6420 7061  ..Unsupported pa
-0000e500: 796d 656e 7420 7479 7065 3a20 0700 0000  yment type: ....
-0000e510: 0953 7461 7465 6d65 6e74 0103 0000 0012  .Statement......
-0000e520: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
-0000e530: 0020 0800 0000 0006 0000 000e 5769 7468  . ..........With
-0000e540: 6472 6177 616c 206f 6620 0700 0000 0953  drawal of .....S
-0000e550: 7461 7465 6d65 6e74 0103 0000 0044 002a  tatement.....D.*
-0000e560: 002a 002a 0020 041d 0415 041e 0411 0425  .*.*. .........%
-0000e570: 041e 0414 0418 041c 0410 0020 0420 0423  ........... . .#
-0000e580: 0427 041d 0410 042f 0020 041f 0420 041e  .'...../. ... ..
-0000e590: 0412 0415 0420 041a 0410 0020 002a 002a  ..... ..... .*.*
-0000e5a0: 002a 0800 0000 0006 0000 001d 2a2a 2a20  .*..........*** 
-0000e5b0: 4d41 4e55 414c 2045 4e54 5259 2052 4551  MANUAL ENTRY REQ
-0000e5c0: 5549 5245 4420 2a2a 2a07 0000 000d 5374  UIRED ***.....St
-0000e5d0: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000e5e0: 3404 2204 3804 3f00 2004 2604 1100 2004  4.".8.?. .&... .
-0000e5f0: 3d04 3500 2004 3f04 3e04 3404 3404 3504  =.5. .?.>.4.4.5.
-0000e600: 4004 3604 3804 3204 3004 3504 4204 4104  @.6.8.2.0.5.B.A.
-0000e610: 4f00 3a00 2008 0000 0000 0600 0000 1c41  O.:. ..........A
-0000e620: 7373 6574 2074 7970 6520 6973 6e27 7420  sset type isn't 
-0000e630: 7375 7070 6f72 7465 643a 2007 0000 000d  supported: .....
-0000e640: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000e650: 0000 4804 1d04 3504 3204 3e04 3704 3c04  ..H...5.2.>.7.<.
-0000e660: 3e04 3604 3d04 3e00 2004 3d04 3004 3904  >.6.=.>. .=.0.9.
-0000e670: 4204 3800 2004 3f04 3b04 3004 4204 5104  B.8. .?.;.0.B.Q.
-0000e680: 3600 2004 3404 3b04 4f00 2004 3e04 4204  6. .4.;.O. .>.B.
-0000e690: 3c04 3504 3d04 4b00 3a00 2008 0000 0000  <.5.=.K.:. .....
-0000e6a0: 0600 0000 1f43 616e 2774 2066 696e 6420  .....Can't find 
-0000e6b0: 6d61 7463 6820 666f 7220 7265 7665 7273  match for revers
-0000e6c0: 616c 3a20 0700 0000 0d53 7461 7465 6d65  al: .....Stateme
-0000e6d0: 6e74 4942 4b52 0103 0000 0046 041d 0435  ntIBKR.....F...5
-0000e6e0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-0000e6f0: 0020 043d 0430 0439 0442 0438 0020 043f  . .=.0.9.B.8. .?
-0000e700: 0430 0440 043d 0443 044e 0020 0437 0430  .0.@.=.C.N. .7.0
-0000e710: 043f 0438 0441 044c 0020 0434 043b 044f  .?.8.A.L. .4.;.O
-0000e720: 0020 0800 0000 0006 0000 001d 4361 6e27  . ..........Can'
-0000e730: 7420 6669 6e64 2070 6169 7265 6420 7265  t find paired re
-0000e740: 636f 7264 2066 6f72 2007 0000 000d 5374  cord for .....St
-0000e750: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000e760: 4e04 1d04 3504 3204 3e04 3c04 3e04 3604  N...5.2.>.<.>.6.
-0000e770: 3d04 3e00 2004 3e04 3f04 4004 3504 3404  =.>. .>.?.@.5.4.
-0000e780: 3504 3b04 3804 4204 4c00 2004 3204 3004  5.;.8.B.L. .2.0.
-0000e790: 3b04 4e04 4204 4300 2004 3404 3b04 4f00  ;.N.B.C. .4.;.O.
-0000e7a0: 2004 4104 4704 5104 4204 3000 3a00 2008   .A.G.Q.B.0.:. .
-0000e7b0: 0000 0000 0600 0000 2843 616e 2774 2067  ........(Can't g
-0000e7c0: 6574 2061 6363 6f75 6e74 2063 7572 7265  et account curre
-0000e7d0: 6e63 7920 666f 7220 6163 636f 756e 743a  ncy for account:
-0000e7e0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000e7f0: 424b 5201 0300 0000 7004 1d04 3504 3204  BKR.....p...5.2.
-0000e800: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
-0000e810: 3e04 3f04 4004 3504 3404 3504 3b04 3804  >.?.@.5.4.5.;.8.
-0000e820: 4204 4c00 2004 3204 3004 3b04 4e04 4204  B.L. .2.0.;.N.B.
-0000e830: 4b00 2004 3404 3b04 4f00 2004 3e04 3f04  K. .4.;.O. .>.?.
-0000e840: 3504 4004 3004 4604 3804 3800 2004 3e04  5.@.0.F.8.8. .>.
-0000e850: 3104 3c04 3504 3d04 3000 2004 3204 3004  1.<.5.=.0. .2.0.
-0000e860: 3b04 4e04 4200 3a00 2008 0000 0000 0600  ;.N.B.:. .......
-0000e870: 0000 2c43 616e 2774 2067 6574 2063 7572  ..,Can't get cur
-0000e880: 7265 6e63 6965 7320 666f 7220 6375 7272  rencies for curr
-0000e890: 656e 6379 2065 7863 6861 6e67 653a 2007  ency exchange: .
-0000e8a0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000e8b0: 5201 0300 0000 6804 1d04 3504 3204 3e04  R.....h...5.2.>.
-0000e8c0: 3704 3c04 3e04 3604 3d04 3e00 2004 4004  7.<.>.6.=.>. .@.
-0000e8d0: 3004 4104 3f04 3e04 3704 3d04 3004 4204  0.A.?.>.7.=.0.B.
-0000e8e0: 4c00 2004 3e04 3f04 3804 4104 3004 3d04  L. .>.?.8.A.0.=.
-0000e8f0: 3804 3500 2004 1e04 3104 4a04 3504 3404  8.5. ...1.J.5.4.
-0000e900: 3804 3d04 3504 3d04 3804 4f00 2004 3a04  8.=.5.=.8.O. .:.
-0000e910: 3e04 3c04 3f04 3004 3d04 3804 3900 2008  >.<.?.0.=.8.9. .
-0000e920: 0000 0000 0600 0000 1f43 616e 2774 2070  .........Can't p
-0000e930: 6172 7365 204d 6572 6765 7220 6465 7363  arse Merger desc
-0000e940: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
-0000e950: 7465 6d65 6e74 4942 4b52 0103 0000 0064  tementIBKR.....d
-0000e960: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000e970: 043d 043e 0020 0440 0430 0441 043f 043e  .=.>. .@.0.A.?.>
-0000e980: 0437 043d 0430 0442 044c 0020 043e 043f  .7.=.0.B.L. .>.?
-0000e990: 0438 0441 0430 043d 0438 0435 0020 0412  .8.A.0.=.8.5. ..
-0000e9a0: 044b 0434 0435 043b 0435 043d 0438 044f  .K.4.5.;.5.=.8.O
-0000e9b0: 0020 043a 043e 043c 043f 0430 043d 0438  . .:.>.<.?.0.=.8
-0000e9c0: 0438 0020 0800 0000 0006 0000 0021 4361  .8. .........!Ca
-0000e9d0: 6e27 7420 7061 7273 6520 5370 696e 2d6f  n't parse Spin-o
-0000e9e0: 6666 2064 6573 6372 6970 7469 6f6e 2007  ff description .
-0000e9f0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000ea00: 5201 0300 0000 4c04 1d04 3504 3204 3e04  R.....L...5.2.>.
-0000ea10: 3704 3c04 3e04 3604 3d04 3e00 2004 4004  7.<.>.6.=.>. .@.
-0000ea20: 3004 4104 3f04 3e04 3704 3d04 3004 4204  0.A.?.>.7.=.0.B.
-0000ea30: 4c00 2004 3e04 3f04 3804 4104 3004 3d04  L. .>.?.8.A.0.=.
-0000ea40: 3804 3500 2004 2104 3f04 3b04 3804 4204  8.5. .!.?.;.8.B.
-0000ea50: 3000 2008 0000 0000 0600 0000 1e43 616e  0. ..........Can
-0000ea60: 2774 2070 6172 7365 2053 706c 6974 2064  't parse Split d
-0000ea70: 6573 6372 6970 7469 6f6e 2007 0000 000d  escription .....
-0000ea80: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
-0000ea90: 0000 6204 1d04 3504 3204 3e04 3704 3c04  ..b...5.2.>.7.<.
-0000eaa0: 3e04 3604 3d04 3e00 2004 4004 3004 4104  >.6.=.>. .@.0.A.
-0000eab0: 3f04 3e04 3704 3d04 3004 4204 4c00 2004  ?.>.7.=.0.B.L. .
-0000eac0: 3e04 3f04 3804 4104 3004 3d04 3804 3500  >.?.8.A.0.=.8.5.
-0000ead0: 2004 1404 3804 3204 3804 3404 3504 3d04   ...8.2.8.4.5.=.
-0000eae0: 3404 3000 2004 3004 3a04 4604 3804 4f04  4.0. .0.:.F.8.O.
-0000eaf0: 3c04 3800 2008 0000 0000 0600 0000 2743  <.8. .........'C
-0000eb00: 616e 2774 2070 6172 7365 2053 746f 636b  an't parse Stock
-0000eb10: 2044 6976 6964 656e 6420 6465 7363 7269   Dividend descri
-0000eb20: 7074 696f 6e20 0700 0000 0d53 7461 7465  ption .....State
-0000eb30: 6d65 6e74 4942 4b52 0103 0000 005a 041d  mentIBKR.....Z..
-0000eb40: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-0000eb50: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
-0000eb60: 043d 0430 0442 044c 0020 043e 043f 0438  .=.0.B.L. .>.?.8
-0000eb70: 0441 0430 043d 0438 0435 0020 0421 043c  .A.0.=.8.5. .!.<
-0000eb80: 0435 043d 044b 0020 0441 0438 043c 0432  .5.=.K. .A.8.<.2
-0000eb90: 043e 043b 0430 0020 0800 0000 0006 0000  .>.;.0. ........
-0000eba0: 0026 4361 6e27 7420 7061 7273 6520 5379  .&Can't parse Sy
-0000ebb0: 6d62 6f6c 2043 6861 6e67 6520 6465 7363  mbol Change desc
-0000ebc0: 7269 7074 696f 6e20 0700 0000 0d53 7461  ription .....Sta
-0000ebd0: 7465 6d65 6e74 4942 4b52 0103 0000 006e  tementIBKR.....n
-0000ebe0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-0000ebf0: 043d 043e 0020 043e 0431 0440 0430 0431  .=.>. .>.1.@.0.1
-0000ec00: 043e 0442 0430 0442 044c 0020 043e 0442  .>.B.0.B.L. .>.B
-0000ec10: 043c 0435 043d 0451 043d 043d 043e 0435  .<.5.=.Q.=.=.>.5
-0000ec20: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
-0000ec30: 0442 0438 0432 043d 043e 0435 0020 0434  .B.8.2.=.>.5. .4
-0000ec40: 0435 0439 0441 0442 0432 0438 0435 0800  .5.9.A.B.2.8.5..
-0000ec50: 0000 0006 0000 0028 4361 6e27 7420 7072  .......(Can't pr
-0000ec60: 6f63 6573 7320 6361 6e63 656c 6c65 6420  ocess cancelled 
-0000ec70: 636f 7270 6f72 6174 6520 6163 7469 6f6e  corporate action
-0000ec80: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
-0000ec90: 4b52 0103 0000 003e 0414 0435 043d 0435  KR.....>...5.=.5
-0000eca0: 0436 043d 044b 0435 0020 0442 0440 0430  .6.=.K.5. .B.@.0
-0000ecb0: 043d 0437 0430 043a 0446 0438 0438 0020  .=.7.0.:.F.8.8. 
-0000ecc0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-0000ecd0: 044b 003a 0020 0800 0000 0006 0000 001a  .K.:. ..........
-0000ece0: 4361 7368 2074 7261 6e73 6163 7469 6f6e  Cash transaction
-0000ecf0: 7320 6c6f 6164 6564 3a20 0700 0000 0d53  s loaded: .....S
-0000ed00: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000ed10: 006a 041a 043e 0440 043f 043e 0440 0430  .j...>.@.?.>.@.0
-0000ed20: 0442 0438 0432 043d 043e 0435 0020 0441  .B.8.2.=.>.5. .A
-0000ed30: 043e 0431 044b 0442 0438 0435 0020 043d  .>.1.K.B.8.5. .=
-0000ed40: 0435 0020 043f 043e 0434 0434 0435 0440  .5. .?.>.4.4.5.@
-0000ed50: 0436 0438 0432 0430 0435 0442 0441 044f  .6.8.2.0.5.B.A.O
-0000ed60: 0020 0434 043b 044f 0020 0442 0438 043f  . .4.;.O. .B.8.?
-0000ed70: 0430 0020 0426 0411 003a 0020 0800 0000  .0. .&...:. ....
-0000ed80: 0006 0000 0031 436f 7270 6f72 6174 6520  .....1Corporate 
-0000ed90: 6163 7469 6f6e 2069 736e 2774 2073 7570  action isn't sup
-0000eda0: 706f 7274 6564 2066 6f72 2061 7373 6574  ported for asset
-0000edb0: 2074 7970 653a 2007 0000 000d 5374 6174   type: .....Stat
-0000edc0: 656d 656e 7449 424b 5201 0300 0000 5e04  ementIBKR.....^.
-0000edd0: 2204 3804 3f00 2004 3a04 3e04 4004 3f04  ".8.?. .:.>.@.?.
-0000ede0: 3e04 4004 3004 4204 3804 3204 3d04 3e04  >.@.0.B.8.2.=.>.
-0000edf0: 3304 3e00 2004 3404 3504 3904 4104 4204  3.>. .4.5.9.A.B.
-0000ee00: 3204 3804 4f00 2004 3d04 3500 2004 3f04  2.8.O. .=.5. .?.
-0000ee10: 3e04 3404 3404 3504 4004 3604 3804 3204  >.4.4.5.@.6.8.2.
-0000ee20: 3004 3504 4204 4104 4f00 3a00 2008 0000  0.5.B.A.O.:. ...
-0000ee30: 0000 0600 0000 2843 6f72 706f 7261 7465  ......(Corporate
-0000ee40: 2061 6374 696f 6e20 7479 7065 2069 7320   action type is 
-0000ee50: 6e6f 7420 7375 7070 6f72 7465 643a 2007  not supported: .
-0000ee60: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000ee70: 5201 0300 0000 4404 1a04 3e04 4004 3f04  R.....D...>.@.?.
-0000ee80: 3e04 4004 3004 4204 3804 3204 3d04 4b04  >.@.0.B.8.2.=.K.
-0000ee90: 3500 2004 3404 3504 3904 4104 4204 3204  5. .4.5.9.A.B.2.
-0000eea0: 3804 4f00 2004 3704 3004 3304 4004 4304  8.O. .7.0.3.@.C.
-0000eeb0: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
-0000eec0: 0600 0000 1a43 6f72 706f 7261 7465 2061  .....Corporate a
-0000eed0: 6374 696f 6e73 206c 6f61 6465 643a 2007  ctions loaded: .
-0000eee0: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000eef0: 5201 0300 0000 5604 1404 3804 3204 3804  R.....V...8.2.8.
-0000ef00: 3404 3504 3d04 3400 2004 3d04 3500 2004  4.5.=.4. .=.5. .
-0000ef10: 3d04 3004 3904 3404 3504 3d00 2004 3404  =.0.9.4.5.=. .4.
-0000ef20: 3b04 4f00 2004 4304 3404 3504 4004 3604  ;.O. .C.4.5.@.6.
-0000ef30: 3004 3d04 3d04 3e04 3304 3e00 2004 3d04  0.=.=.>.3.>. .=.
-0000ef40: 3004 3b04 3e04 3304 3000 3a00 2008 0000  0.;.>.3.0.:. ...
-0000ef50: 0000 0600 0000 2844 6976 6964 656e 6420  ......(Dividend 
-0000ef60: 6e6f 7420 666f 756e 6420 666f 7220 7769  not found for wi
-0000ef70: 7468 686f 6c64 696e 6720 7461 783a 2007  thholding tax: .
-0000ef80: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000ef90: 5201 0300 0000 2e00 4900 4200 4b00 5200  R.......I.B.K.R.
-0000efa0: 2000 6600 6c00 6500 7800 2d04 3e04 4204   .f.l.e.x.-.>.B.
-0000efb0: 4704 5104 4200 2000 2800 2a00 2e00 7800  G.Q.B. .(.*...x.
-0000efc0: 6d00 6c00 2908 0000 0000 0600 0000 1749  m.l.)..........I
-0000efd0: 424b 5220 666c 6578 2d71 7565 7279 2028  BKR flex-query (
-0000efe0: 2a2e 786d 6c29 0700 0000 0d53 7461 7465  *.xml).....State
-0000eff0: 6d65 6e74 4942 4b52 0103 0000 0026 0049  mentIBKR.....&.I
-0000f000: 006e 0074 0065 0072 0061 0063 0074 0069  .n.t.e.r.a.c.t.i
-0000f010: 0076 0065 0020 0042 0072 006f 006b 0065  .v.e. .B.r.o.k.e
-0000f020: 0072 0073 0800 0000 0006 0000 0013 496e  .r.s..........In
-0000f030: 7465 7261 6374 6976 6520 4272 6f6b 6572  teractive Broker
-0000f040: 7307 0000 000d 5374 6174 656d 656e 7449  s.....StatementI
-0000f050: 424b 5201 0300 0000 5604 2204 3804 3f00  BKR.....V.".8.?.
-0000f060: 2004 3e04 4204 4704 5104 4204 3000 2000   .>.B.G.Q.B.0. .
-0000f070: 4900 6e00 7400 6500 7200 6100 6300 7400  I.n.t.e.r.a.c.t.
-0000f080: 6900 7600 6500 2000 4200 7200 6f00 6b00  i.v.e. .B.r.o.k.
-0000f090: 6500 7200 7300 2004 3d04 3500 2004 3e04  e.r.s. .=.5. .>.
-0000f0a0: 3f04 4004 3504 3404 3504 3b04 5104 3d08  ?.@.5.4.5.;.Q.=.
-0000f0b0: 0000 0000 0600 0000 2949 6e74 6572 6163  ........)Interac
-0000f0c0: 7469 7665 2042 726f 6b65 7273 2072 6570  tive Brokers rep
-0000f0d0: 6f72 7420 7479 7065 206e 6f74 2066 6f75  ort type not fou
-0000f0e0: 6e64 0700 0000 0d53 7461 7465 6d65 6e74  nd.....Statement
-0000f0f0: 4942 4b52 0103 0000 003a 0417 0430 0433  IBKR.....:...0.3
-0000f100: 0440 0443 0437 043a 0430 0020 043e 0442  .@.C.7.:.0. .>.B
-0000f110: 0447 0451 0442 0430 0020 0049 0042 0020  .G.Q.B.0. .I.B. 
-0000f120: 0434 043b 044f 0020 0441 0447 0451 0442  .4.;.O. .A.G.Q.B
-0000f130: 0430 0020 0800 0000 0006 0000 0023 4c6f  .0. .........#Lo
-0000f140: 6164 2049 4220 466c 6578 2d73 7461 7465  ad IB Flex-state
-0000f150: 6d65 6e74 2066 6f72 2061 6363 6f75 6e74  ment for account
-0000f160: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000f170: 424b 5201 0300 0000 5804 1d04 3504 3404  BKR.....X...5.4.
-0000f180: 3e04 4104 4204 3004 4204 3e04 4704 3d04  >.A.B.0.B.>.G.=.
-0000f190: 3e00 2004 3404 3004 3d04 3d04 4b04 4500  >. .4.0.=.=.K.E.
-0000f1a0: 2004 3e04 3100 2004 1e04 3104 4a04 3504   .>.1. ...1.J.5.
-0000f1b0: 3404 3804 3d04 3504 3d04 3804 3800 2004  4.8.=.5.=.8.8. .
-0000f1c0: 3a04 3e04 3c04 3f04 3004 3d04 3804 3900  :.>.<.?.0.=.8.9.
-0000f1d0: 2008 0000 0000 0600 0000 224d 6572 6765   ........."Merge
-0000f1e0: 7220 6465 7363 7269 7074 696f 6e20 6d69  r description mi
-0000f1f0: 7373 2073 6f6d 6520 6461 7461 2007 0000  ss some data ...
-0000f200: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000f210: 0300 0000 5e04 1d04 3504 3e04 3404 3d04  ....^...5.>.4.=.
-0000f220: 3e04 3704 3d04 3004 4704 3d04 3e04 3500  >.7.=.0.G.=.>.5.
-0000f230: 2004 4104 3e04 3204 3f04 3004 3404 3504   .A.>.2.?.0.4.5.
-0000f240: 3d04 3804 3500 2004 4104 3e04 3104 4b04  =.8.5. .A.>.1.K.
-0000f250: 4204 3804 3900 2004 4004 3504 3e04 4004  B.8.9. .@.5.>.@.
-0000f260: 3304 3004 3d04 3804 3704 3004 4604 3804  3.0.=.8.7.0.F.8.
-0000f270: 3800 2008 0000 0000 0600 0000 294d 756c  8. .........)Mul
-0000f280: 7469 706c 6520 6d65 7267 6572 2072 6563  tiple merger rec
-0000f290: 6f72 6473 2061 6c72 6561 6479 2065 7869  ords already exi
-0000f2a0: 7374 2061 7420 0700 0000 0d53 7461 7465  st at .....State
-0000f2b0: 6d65 6e74 4942 4b52 0103 0000 0052 0414  mentIBKR.....R..
-0000f2c0: 0435 0439 0441 0442 0432 0438 0435 0020  .5.9.A.B.2.8.5. 
-0000f2d0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
-0000f2e0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
-0000f2f0: 044f 0020 0434 043b 044f 0020 043e 043f  .O. .4.;.O. .>.?
-0000f300: 0446 0438 043e 043d 043e 0432 003a 0020  .F.8.>.=.>.2.:. 
-0000f310: 0800 0000 0006 0000 0027 4f70 7469 6f6e  .........'Option
-0000f320: 2045 2641 2645 2061 6374 696f 6e20 6973   E&A&E action is
-0000f330: 6e27 7420 696d 706c 656d 656e 7465 643a  n't implemented:
-0000f340: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000f350: 424b 5201 0300 0000 3a04 1804 4104 3f04  BKR.....:...A.?.
-0000f360: 3e04 3b04 3d04 3504 3d04 3804 3500 2004  >.;.=.5.=.8.5. .
-0000f370: 3f04 4004 3e04 3404 3004 3d04 3d04 3e04  ?.@.>.4.0.=.=.>.
-0000f380: 3304 3e00 2004 3e04 3f04 4604 3804 3e04  3.>. .>.?.F.8.>.
-0000f390: 3d04 3008 0000 0000 0600 0000 114f 7074  =.0..........Opt
-0000f3a0: 696f 6e20 6173 7369 676e 6d65 6e74 0700  ion assignment..
-0000f3b0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000f3c0: 0103 0000 003a 0418 0441 043f 043e 043b  .....:...A.?.>.;
-0000f3d0: 043d 0435 043d 0438 0435 002f 044d 043a  .=.5.=.8.5./.M.:
-0000f3e0: 0441 043f 0438 0440 0430 0446 0438 044f  .A.?.8.@.0.F.8.O
-0000f3f0: 0020 043e 043f 0446 0438 043e 043d 0430  . .>.?.F.8.>.=.0
-0000f400: 0800 0000 0006 0000 001a 4f70 7469 6f6e  ..........Option
-0000f410: 2061 7373 6967 6e6d 656e 742f 6578 6572   assignment/exer
-0000f420: 6369 7365 0700 0000 0d53 7461 7465 6d65  cise.....Stateme
-0000f430: 6e74 4942 4b52 0103 0000 003a 0418 0441  ntIBKR.....:...A
-0000f440: 043f 043e 043b 043d 0435 043d 0438 0435  .?.>.;.=.5.=.8.5
-0000f450: 0020 043a 0443 043f 043b 0435 043d 043d  . .:.C.?.;.5.=.=
-0000f460: 043e 0433 043e 0020 043e 043f 0446 0438  .>.3.>. .>.?.F.8
-0000f470: 043e 043d 0430 0800 0000 0006 0000 000f  .>.=.0..........
-0000f480: 4f70 7469 6f6e 2065 7865 7263 6973 6507  Option exercise.
-0000f490: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f4a0: 5201 0300 0000 2404 2d04 3a04 4104 3f04  R.....$.-.:.A.?.
-0000f4b0: 3804 4004 3004 4604 3804 4f00 2004 3e04  8.@.0.F.8.O. .>.
-0000f4c0: 3f04 4604 3804 3e04 3d04 3008 0000 0000  ?.F.8.>.=.0.....
-0000f4d0: 0600 0000 114f 7074 696f 6e20 6578 7069  .....Option expi
-0000f4e0: 7261 7469 6f6e 0700 0000 0d53 7461 7465  ration.....State
-0000f4f0: 6d65 6e74 4942 4b52 0103 0000 0040 0414  mentIBKR.....@..
-0000f500: 0435 0439 0441 0442 0432 0438 044f 0020  .5.9.A.B.2.8.O. 
-0000f510: 0441 0020 043e 043f 0446 0438 043e 043d  .A. .>.?.F.8.>.=
-0000f520: 0430 043c 0438 0020 0437 0430 0433 0440  .0.<.8. .7.0.3.@
-0000f530: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
-0000f540: 0000 0006 0000 0016 4f70 7469 6f6e 7320  ........Options 
-0000f550: 4526 4126 4520 6c6f 6164 6564 3a20 0700  E&A&E loaded: ..
-0000f560: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000f570: 0103 0000 006a 041d 0435 0020 043d 0430  .....j...5. .=.0
-0000f580: 0439 0434 0435 043d 0430 0020 0441 0434  .9.4.5.=.0. .A.4
-0000f590: 0435 043b 043a 0430 0020 0434 043b 044f  .5.;.:.0. .4.;.O
-0000f5a0: 0020 0438 0441 043f 043e 043b 043d 0435  . .8.A.?.>.;.=.5
-0000f5b0: 043d 0438 044f 002f 044d 043a 0441 043f  .=.8.O./.M.:.A.?
-0000f5c0: 0438 0440 0430 0446 0438 0438 0020 043e  .8.@.0.F.8.8. .>
-0000f5d0: 043f 0446 0438 043e 043d 0430 003a 0020  .?.F.8.>.=.0.:. 
-0000f5e0: 0800 0000 0006 0000 0035 4f72 6967 696e  .........5Origin
-0000f5f0: 616c 2074 7261 6465 206e 6f74 2066 6f75  al trade not fou
-0000f600: 6e64 2066 6f72 204f 7074 696f 6e20 4526  nd for Option E&
-0000f610: 4126 4520 6f70 6572 6174 696f 6e3a 2007  A&E operation: .
-0000f620: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
-0000f630: 5201 0300 0000 6c04 1f04 3b04 3004 4204  R.....l...;.0.B.
-0000f640: 5104 3600 2004 3104 4b04 3b00 2004 3e04  Q.6. .1.K.;. .>.
-0000f650: 4204 3c04 3504 3d04 5104 3d00 2004 3f04  B.<.5.=.Q.=. .?.
-0000f660: 3e00 2004 3f04 4004 3804 3c04 3504 4004  >. .?.@.8.<.5.@.
-0000f670: 3d04 3e04 3c04 4300 2004 4104 3e04 3204  =.>.<.C. .A.>.2.
-0000f680: 3f04 3004 3404 3504 3d04 3804 4e00 2004  ?.0.4.5.=.8.N. .
-0000f690: 3e04 3f04 3804 4104 3004 3d04 3804 4f00  >.?.8.A.0.=.8.O.
-0000f6a0: 3a00 2008 0000 0000 0600 0000 3150 6179  :. .........1Pay
-0000f6b0: 6d65 6e74 2077 6173 2072 6576 6572 7365  ment was reverse
-0000f6c0: 6420 6279 2061 7070 726f 7869 6d61 7465  d by approximate
-0000f6d0: 2064 6573 6372 6970 7469 6f6e 3a20 0700   description: ..
-0000f6e0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000f6f0: 0103 0000 006a 041f 043b 0430 0442 0451  .....j...;.0.B.Q
-0000f700: 0436 0020 0431 044b 043b 0020 043e 0442  .6. .1.K.;. .>.B
-0000f710: 043c 0435 043d 0451 043d 002c 0020 043d  .<.5.=.Q.=.,. .=
-0000f720: 043e 0020 0441 0020 043d 0435 0441 043e  .>. .A. .=.5.A.>
-0000f730: 0432 043f 0430 0434 0430 044e 0449 0435  .2.?.0.4.0.N.I.5
-0000f740: 0439 0020 0434 0430 0442 043e 0439 0020  .9. .4.0.B.>.9. 
-0000f750: 043e 0442 0447 0451 0442 0430 003a 0020  .>.B.G.Q.B.0.:. 
-0000f760: 0800 0000 0006 0000 0033 5061 796d 656e  .........3Paymen
-0000f770: 7420 7761 7320 7265 7665 7273 6564 2077  t was reversed w
-0000f780: 6974 6820 6469 6666 6572 656e 7420 7265  ith different re
-0000f790: 706f 7274 6564 2064 6174 653a 2007 0000  ported date: ...
-0000f7a0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000f7b0: 0300 0000 2804 1f04 3b04 3004 4204 5104  ....(...;.0.B.Q.
-0000f7c0: 3600 2004 3104 4b04 3b00 2004 3e04 4204  6. .1.K.;. .>.B.
-0000f7d0: 3c04 3504 3d04 5104 3d00 3a00 2008 0000  <.5.=.Q.=.:. ...
-0000f7e0: 0000 0600 0000 1650 6179 6d65 6e74 2077  .......Payment w
-0000f7f0: 6173 2072 6576 6572 7365 643a 2007 0000  as reversed: ...
-0000f800: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000f810: 0300 0000 1c04 2604 1100 2004 3704 3004  ......&... .7.0.
-0000f820: 3304 4004 4304 3604 3504 3d04 4b00 3a00  3.@.C.6.5.=.K.:.
-0000f830: 2008 0000 0000 0600 0000 1353 6563 7572   ..........Secur
-0000f840: 6974 6965 7320 6c6f 6164 6564 3a20 0700  ities loaded: ..
-0000f850: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000f860: 0103 0000 0056 041d 0435 0434 043e 0441  .....V...5.4.>.A
-0000f870: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
-0000f880: 0434 0430 043d 043d 044b 0445 0020 0434  .4.0.=.=.K.E. .4
-0000f890: 043b 044f 0020 0412 044b 0434 0435 043b  .;.O. ...K.4.5.;
-0000f8a0: 0435 043d 0438 044f 0020 043a 043e 043c  .5.=.8.O. .:.>.<
-0000f8b0: 043f 0430 043d 0438 0438 0020 0800 0000  .?.0.=.8.8. ....
-0000f8c0: 0006 0000 0024 5370 696e 2d6f 6666 2064  .....$Spin-off d
-0000f8d0: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
-0000f8e0: 736f 6d65 2064 6174 6120 0700 0000 0d53  some data .....S
-0000f8f0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000f900: 005c 0418 0441 0445 043e 0434 043d 0430  .\...A.E.>.4.=.0
-0000f910: 044f 0020 0426 0411 0020 0434 043b 044f  .O. .&... .4.;.O
-0000f920: 0020 0432 044b 0434 0435 043b 0435 043d  . .2.K.4.5.;.5.=
-0000f930: 0438 044f 0020 043a 043e 043c 043f 0430  .8.O. .:.>.<.?.0
-0000f940: 043d 0438 0438 0020 043d 0435 0020 043d  .=.8.8. .=.5. .=
-0000f950: 0430 0439 0434 0435 043d 0430 0020 0800  .0.9.4.5.=.0. ..
-0000f960: 0000 0006 0000 0021 5370 696e 2d6f 6666  .......!Spin-off
-0000f970: 2069 6e69 7469 616c 2061 7373 6574 206e   initial asset n
-0000f980: 6f74 2066 6f75 6e64 2007 0000 000d 5374  ot found .....St
-0000f990: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
-0000f9a0: 5604 1e04 4804 3804 3104 3a04 3000 2004  V...H.8.1.:.0. .
-0000f9b0: 3e04 3a04 4004 4304 3304 3b04 3504 3d04  >.:.@.C.3.;.5.=.
-0000f9c0: 3804 4f00 2000 5300 7000 6900 6e00 2d00  8.O. .S.p.i.n.-.
-0000f9d0: 6f00 6600 6600 2004 4104 3b04 3804 4804  o.f.f. .A.;.8.H.
-0000f9e0: 3a04 3e04 3c00 2004 3104 3e04 3b04 4c04  :.>.<. .1.>.;.L.
-0000f9f0: 4804 3004 4f00 2008 0000 0000 0600 0000  H.0.O. .........
-0000fa00: 2353 7069 6e2d 6f66 6620 726f 756e 6469  #Spin-off roundi
-0000fa10: 6e67 2065 7272 6f72 2069 7320 746f 6f20  ng error is too 
-0000fa20: 6269 6720 0700 0000 0d53 7461 7465 6d65  big .....Stateme
-0000fa30: 6e74 4942 4b52 0103 0000 003e 041d 0435  ntIBKR.....>...5
-0000fa40: 0434 043e 0441 0442 0430 0442 043e 0447  .4.>.A.B.0.B.>.G
-0000fa50: 043d 043e 0020 0434 0430 043d 043d 044b  .=.>. .4.0.=.=.K
-0000fa60: 0445 0020 0434 043b 044f 0020 0421 043f  .E. .4.;.O. .!.?
-0000fa70: 043b 0438 0442 0430 0020 0800 0000 0006  .;.8.B.0. ......
-0000fa80: 0000 0021 5370 6c69 7420 6465 7363 7269  ...!Split descri
-0000fa90: 7074 696f 6e20 6d69 7373 2073 6f6d 6520  ption miss some 
-0000faa0: 6461 7461 2007 0000 000d 5374 6174 656d  data .....Statem
-0000fab0: 656e 7449 424b 5201 0300 0000 3804 1704  entIBKR.....8...
-0000fac0: 3004 4704 3804 4104 3b04 3504 3d04 3804  0.G.8.A.;.5.=.8.
-0000fad0: 3500 2004 3004 3a04 4604 3804 3900 2004  5. .0.:.F.8.9. .
-0000fae0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
-0000faf0: 3e00 3a00 2008 0000 0000 0600 0000 1753  >.:. ..........S
-0000fb00: 746f 636b 2076 6573 7469 6e67 7320 6c6f  tock vestings lo
-0000fb10: 6164 6564 3a20 0700 0000 0d53 7461 7465  aded: .....State
-0000fb20: 6d65 6e74 4942 4b52 0103 0000 0048 041a  mentIBKR.....H..
-0000fb30: 043e 0440 0440 0435 043a 0442 0438 0440  .>.@.@.5.:.B.8.@
-0000fb40: 043e 0432 043a 0430 0020 043d 0430 043b  .>.2.:.0. .=.0.;
-0000fb50: 043e 0433 0430 0020 0434 043b 044f 0020  .>.3.0. .4.;.O. 
-0000fb60: 0434 0438 0432 0438 0434 0435 043d 0434  .4.8.2.8.4.5.=.4
-0000fb70: 0430 003a 0020 0800 0000 0006 0000 001d  .0.:. ..........
-0000fb80: 5461 7820 6164 6a75 7374 6d65 6e74 2066  Tax adjustment f
-0000fb90: 6f72 2064 6976 6964 656e 643a 2007 0000  or dividend: ...
-0000fba0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
-0000fbb0: 0300 0000 2404 1d04 3004 3b04 3e04 3304  ....$...0.;.>.3.
-0000fbc0: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
-0000fbd0: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
-0000fbe0: 0000 0e54 6178 6573 206c 6f61 6465 643a  ...Taxes loaded:
-0000fbf0: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
-0000fc00: 424b 5201 03ff ffff ff08 0000 0000 0600  BKR.............
-0000fc10: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
-0000fc20: 3a20 0700 0000 0d53 7461 7465 6d65 6e74  : .....Statement
-0000fc30: 4942 4b52 0103 0000 0058 041d 0435 043f  IBKR.....X...5.?
-0000fc40: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
-0000fc50: 0430 0435 043c 044b 0439 0020 0444 043e  .0.5.<.K.9. .D.>
-0000fc60: 0440 043c 0430 0442 0020 043e 043f 0438  .@.<.0.B. .>.?.8
-0000fc70: 0441 0430 043d 0438 044f 0020 0434 0438  .A.0.=.8.O. .4.8
-0000fc80: 0432 0438 0434 0435 043d 0434 0430 003a  .2.8.4.5.=.4.0.:
-0000fc90: 0020 0800 0000 0006 0000 0022 556e 6861  . ........."Unha
-0000fca0: 6e64 6c65 6420 6469 7669 6465 6e64 2070  ndled dividend p
-0000fcb0: 6174 7465 726e 2066 6f75 6e64 3a20 0700  attern found: ..
-0000fcc0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
-0000fcd0: 0103 0000 004e 041d 0435 043f 043e 0434  .....N...5.?.>.4
-0000fce0: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
-0000fcf0: 043c 044b 0439 0020 0444 043e 0440 043c  .<.K.9. .D.>.@.<
-0000fd00: 0430 0442 0020 0441 0442 0440 0430 043d  .0.B. .A.B.@.0.=
-0000fd10: 044b 0020 043d 0430 043b 043e 0433 0430  .K. .=.0.;.>.3.0
-0000fd20: 003a 0020 0800 0000 0006 0000 0025 556e  .:. .........%Un
-0000fd30: 6861 6e64 6c65 6420 7461 7820 636f 756e  handled tax coun
-0000fd40: 7472 7920 7061 7474 6572 6e20 666f 756e  try pattern foun
-0000fd50: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
-0000fd60: 7449 424b 5201 0300 0000 5204 1d04 3504  tIBKR.....R...5.
-0000fd70: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
-0000fd80: 3204 3004 3504 3c04 4b04 3900 2004 4404  2.0.5.<.K.9. .D.
-0000fd90: 3e04 4004 3c04 3004 4200 2004 3e04 3f04  >.@.<.0.B. .>.?.
-0000fda0: 3804 4104 3004 3d04 3804 4f00 2004 3d04  8.A.0.=.8.O. .=.
-0000fdb0: 3004 3b04 3e04 3304 3000 3a00 2008 0000  0.;.>.3.0.:. ...
-0000fdc0: 0000 0600 0000 1d55 6e68 616e 646c 6564  .......Unhandled
-0000fdd0: 2074 6178 2070 6174 7465 726e 2066 6f75   tax pattern fou
-0000fde0: 6e64 3a20 0700 0000 0d53 7461 7465 6d65  nd: .....Stateme
-0000fdf0: 6e74 4942 4b52 0103 0000 0058 041d 0435  ntIBKR.....X...5
-0000fe00: 0438 0437 0432 0435 0441 0442 043d 044b  .8.7.2.5.A.B.=.K
-0000fe10: 0439 0020 0442 0438 043f 0020 043e 0442  .9. .B.8.?. .>.B
-0000fe20: 0447 0451 0442 0430 0020 0049 006e 0074  .G.Q.B.0. .I.n.t
-0000fe30: 0065 0072 0061 0063 0074 0069 0076 0065  .e.r.a.c.t.i.v.e
-0000fe40: 0020 0042 0072 006f 006b 0065 0072 0073  . .B.r.o.k.e.r.s
-0000fe50: 003a 0020 0800 0000 0006 0000 0029 556e  .:. .........)Un
-0000fe60: 6b6e 6f77 6e20 496e 7465 7261 6374 6976  known Interactiv
-0000fe70: 6520 4272 6f6b 6572 7320 7265 706f 7274  e Brokers report
-0000fe80: 2074 7970 653a 2007 0000 000d 5374 6174   type: .....Stat
-0000fe90: 656d 656e 7449 424b 5201 0300 0000 a204  ementIBKR.......
-0000fea0: 1204 4b00 2004 3f04 4b04 4204 3004 3504  ..K. .?.K.B.0.5.
-0000feb0: 4204 3504 4104 4c00 2004 3704 3004 3304  B.5.A.L. .7.0.3.
-0000fec0: 4004 4304 3704 3804 4204 4c00 2004 3e04  @.C.7.8.B.L. .>.
-0000fed0: 4204 4704 5104 4200 2004 3e00 2004 3f04  B.G.Q.B. .>. .?.
-0000fee0: 3e04 3404 4204 3204 3504 4004 3604 3404  >.4.B.2.5.@.6.4.
-0000fef0: 5104 3d04 3d04 4b04 4500 2004 4104 3404  Q.=.=.K.E. .A.4.
-0000ff00: 3504 3b04 3a04 3004 4500 2004 3204 3c04  5.;.:.0.E. .2.<.
-0000ff10: 3504 4104 4204 3e00 2004 3e04 4204 4704  5.A.B.>. .>.B.G.
-0000ff20: 5104 4204 3000 2004 3f04 3e00 2004 1004  Q.B.0. .?.>. ...
-0000ff30: 3a04 4204 3804 3204 3d04 3e04 4104 4204  :.B.8.2.=.>.A.B.
-0000ff40: 3808 0000 0000 0600 0000 3f59 6f75 2074  8.........?You t
-0000ff50: 7279 2074 6f20 696d 706f 7274 2054 7261  ry to import Tra
-0000ff60: 6465 2063 6f6e 6669 6d61 7469 6f6e 2072  de confimation r
-0000ff70: 6570 6f72 742c 206e 6f74 2041 6374 6976  eport, not Activ
-0000ff80: 6974 7920 7265 706f 7274 0700 0000 0d53  ity report.....S
-0000ff90: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
-0000ffa0: 0052 041d 0435 0432 043e 0437 043c 043e  .R...5.2.>.7.<.>
-0000ffb0: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
-0000ffc0: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
-0000ffd0: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
-0000ffe0: 0434 0438 0432 0438 0434 0435 043d 0434  .4.8.2.8.4.5.=.4
-0000fff0: 0430 0020 0800 0000 0006 0000 0021 4361  .0. .........!Ca
-00010000: 6e27 7420 7061 7273 6520 4469 7669 6465  n't parse Divide
-00010010: 6e64 2064 6573 6372 6970 7469 6f6e 2007  nd description .
-00010020: 0000 000c 5374 6174 656d 656e 744a 3254  ....StatementJ2T
-00010030: 0103 0000 001c 0414 0421 0020 0437 0430  .........!. .7.0
-00010040: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
-00010050: 0020 0800 0000 0006 0000 0016 4361 7368  . ..........Cash
-00010060: 2062 616c 616e 6365 7320 6c6f 6164 6564   balances loaded
-00010070: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00010080: 4a32 5401 0300 0000 3a04 1404 3504 3d04  J2T.....:...5.=.
-00010090: 3504 3604 3d04 4b04 4500 2004 3e04 3f04  5.6.=.K.E. .>.?.
-000100a0: 3504 4004 3004 4604 3804 3900 2004 3704  5.@.0.F.8.9. .7.
-000100b0: 3004 3304 4004 4304 3604 3504 3d04 3e00  0.3.@.C.6.5.=.>.
-000100c0: 3a00 2008 0000 0000 0600 0000 1843 6173  :. ..........Cas
-000100d0: 6820 6f70 6572 6174 696f 6e73 206c 6f61  h operations loa
-000100e0: 6465 643a 2007 0000 000c 5374 6174 656d  ded: .....Statem
-000100f0: 656e 744a 3254 0103 0000 0048 0421 0434  entJ2T.....H.!.4
-00010100: 0435 043b 043a 0438 0020 0441 0020 043a  .5.;.:.8. .A. .:
-00010110: 0440 0438 043f 0442 043e 002d 0432 0430  .@.8.?.B.>.-.2.0
-00010120: 043b 044e 0442 0430 043c 0438 0020 0437  .;.N.B.0.<.8. .7
-00010130: 0430 0433 0440 0443 0436 0435 043d 044b  .0.3.@.C.6.5.=.K
-00010140: 003a 0020 0800 0000 0006 0000 0016 4372  .:. ..........Cr
-00010150: 7970 746f 2074 7261 6465 7320 6c6f 6164  ypto trades load
-00010160: 6564 3a20 0700 0000 0c53 7461 7465 6d65  ed: .....Stateme
-00010170: 6e74 4a32 5401 0300 0000 5004 1200 2004  ntJ2T.....P... .
-00010180: 3e04 3f04 3804 4104 3004 3d04 3804 3800  >.?.8.A.0.=.8.8.
-00010190: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
-000101a0: 3404 3000 2004 3e04 4204 4104 4304 4204  4.0. .>.B.A.C.B.
-000101b0: 4104 4204 3204 4304 4e04 4200 2004 3404  A.B.2.C.N.B. .4.
-000101c0: 3004 3d04 3d04 4b04 3500 2008 0000 0000  0.=.=.K.5. .....
-000101d0: 0600 0000 2444 6976 6964 656e 6420 6465  ....$Dividend de
-000101e0: 7363 7269 7074 696f 6e20 6d69 7373 2073  scription miss s
-000101f0: 6f6d 6520 6461 7461 2007 0000 000c 5374  ome data .....St
-00010200: 6174 656d 656e 744a 3254 0103 0000 004e  atementJ2T.....N
-00010210: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
-00010220: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
-00010230: 0435 043d 0020 0434 043b 044f 0020 0441  .5.=. .4.;.O. .A
-00010240: 043f 0438 0441 0430 043d 0438 044f 0020  .?.8.A.0.=.8.O. 
-00010250: 043d 0430 043b 043e 0433 0430 0020 0800  .=.0.;.>.3.0. ..
-00010260: 0000 0006 0000 001f 4469 7669 6465 6e64  ........Dividend
-00010270: 2066 6f72 2074 6178 2077 6173 206e 6f74   for tax was not
-00010280: 2066 6f75 6e64 2007 0000 000c 5374 6174   found .....Stat
-00010290: 656d 656e 744a 3254 0103 0000 0044 0422  ementJ2T.....D."
-000102a0: 0440 0430 043d 0437 0430 043a 0446 0438  .@.0.=.7.0.:.F.8
-000102b0: 044f 0020 043f 0440 043e 043f 0443 0449  .O. .?.@.>.?.C.I
-000102c0: 0435 043d 0430 0020 043f 0440 0438 0020  .5.=.0. .?.@.8. 
-000102d0: 0438 043c 043f 043e 0440 0442 0435 003a  .8.<.?.>.@.B.5.:
-000102e0: 0020 0800 0000 0006 0000 001f 496d 706f  . ..........Impo
-000102f0: 7274 2073 6b69 7070 6564 206f 6620 7472  rt skipped of tr
-00010300: 616e 7361 6374 696f 6e3a 2007 0000 000c  ansaction: .....
-00010310: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
-00010320: 0014 004a 0075 0073 0074 0032 0054 0072  ...J.u.s.t.2.T.r
-00010330: 0061 0064 0065 0800 0000 0006 0000 000a  .a.d.e..........
-00010340: 4a75 7374 3254 7261 6465 0700 0000 0c53  Just2Trade.....S
-00010350: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
-00010360: 3204 1e04 4204 4704 5104 4200 2000 4a00  2...B.G.Q.B. .J.
-00010370: 7500 7300 7400 3200 5400 7200 6100 6400  u.s.t.2.T.r.a.d.
-00010380: 6500 2000 2800 2a00 2e00 7800 6c00 7300  e. .(.*...x.l.s.
-00010390: 7800 2908 0000 0000 0600 0000 1d4a 7573  x.)..........Jus
-000103a0: 7432 5472 6164 6520 7374 6174 656d 656e  t2Trade statemen
-000103b0: 7420 282a 2e78 6c73 7829 0700 0000 0c53  t (*.xlsx).....S
-000103c0: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
-000103d0: 1c04 2604 1100 2004 3704 3004 3304 4004  ..&... .7.0.3.@.
-000103e0: 4304 3604 3504 3d04 4b00 3a00 2008 0000  C.6.5.=.K.:. ...
-000103f0: 0000 0600 0000 1353 6563 7572 6974 6965  .......Securitie
-00010400: 7320 6c6f 6164 6564 3a20 0700 0000 0c53  s loaded: .....S
-00010410: 7461 7465 6d65 6e74 4a32 5401 0300 0000  tatementJ2T.....
-00010420: 3804 2104 3404 3504 3b04 3a04 3800 2004  8.!.4.5.;.:.8. .
-00010430: 4100 2004 3004 3a04 4604 3804 4f04 3c04  A. .0.:.F.8.O.<.
-00010440: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
-00010450: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
-00010460: 0000 1553 746f 636b 2074 7261 6465 7320  ...Stock trades 
-00010470: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
-00010480: 7465 6d65 6e74 4a32 5401 0300 0000 4004  tementJ2T.....@.
-00010490: 1d04 3504 3804 3704 3204 3504 4104 4204  ..5.8.7.2.5.A.B.
-000104a0: 3d04 3004 4f00 2004 3404 3504 3d04 3504  =.0.O. .4.5.=.5.
-000104b0: 3604 3d04 3004 4f00 2004 4204 4004 3004  6.=.0.O. .B.@.0.
-000104c0: 3d04 3704 3004 3a04 4604 3804 4f00 2008  =.7.0.:.F.8.O. .
-000104d0: 0000 0000 0600 0000 1e55 6e6b 6e6f 776e  .........Unknown
-000104e0: 2063 6173 6820 7472 616e 7361 6374 696f   cash transactio
-000104f0: 6e20 7479 7065 2007 0000 000c 5374 6174  n type .....Stat
-00010500: 656d 656e 744a 3254 0103 0000 0030 041d  ementJ2T.....0..
-00010510: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
-00010520: 044b 0439 0020 0442 0438 043f 0020 0441  .K.9. .B.8.?. .A
-00010530: 0434 0435 043b 043a 0438 003a 0020 0800  .4.5.;.:.8.:. ..
-00010540: 0000 0006 0000 0014 556e 6b6e 6f77 6e20  ........Unknown 
-00010550: 7472 6164 6520 7479 7065 3a20 0700 0000  trade type: ....
-00010560: 0c53 7461 7465 6d65 6e74 4a32 5401 0300  .StatementJ2T...
-00010570: 0000 4a04 1d04 3504 3f04 3e04 3404 3404  ..J...5.?.>.4.4.
-00010580: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
-00010590: 3004 4f00 2004 3404 3504 3d04 3504 3604  0.O. .4.5.=.5.6.
-000105a0: 3d04 3004 4f00 2004 4204 4004 3004 3d04  =.0.O. .B.@.0.=.
-000105b0: 3704 3004 3a04 4604 3804 4f00 2008 0000  7.0.:.F.8.O. ...
-000105c0: 0000 0600 0000 1e55 6e73 7570 7070 6f72  .......Unsupppor
-000105d0: 7465 6420 6361 7368 2074 7261 6e73 6163  ted cash transac
-000105e0: 7469 6f6e 2007 0000 000c 5374 6174 656d  tion .....Statem
-000105f0: 656e 744a 3254 0103 0000 003a 0414 0435  entJ2T.....:...5
-00010600: 043d 0435 0436 043d 044b 0445 0020 043e  .=.5.6.=.K.E. .>
-00010610: 043f 0435 0440 0430 0446 0438 0439 0020  .?.5.@.0.F.8.9. 
-00010620: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-00010630: 043e 003a 0020 0800 0000 0006 0000 0018  .>.:. ..........
-00010640: 4361 7368 206f 7065 7261 7469 6f6e 7320  Cash operations 
-00010650: 6c6f 6164 6564 3a20 0700 0000 0c53 7461  loaded: .....Sta
-00010660: 7465 6d65 6e74 4b49 5401 0300 0000 7604  tementKIT.....v.
-00010670: 1d04 3004 3b04 3e04 3300 2004 3d04 3000  ..0.;.>.3. .=.0.
-00010680: 2004 3404 3804 3204 3804 3404 3504 3d04   .4.8.2.8.4.5.=.
-00010690: 3404 4b00 2004 3d04 3500 2004 3f04 3e04  4.K. .=.5. .?.>.
-000106a0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-000106b0: 3504 4204 4104 4f00 2004 3404 3b04 4f00  5.B.A.O. .4.;.O.
-000106c0: 2004 3104 4004 3e04 3a04 3504 4004 3000   .1.@.>.:.5.@.0.
-000106d0: 2004 1a04 1804 2200 2d04 4404 3804 3d04   .....".-.D.8.=.
-000106e0: 3004 3d04 4108 0000 0000 0600 0000 3e44  0.=.A.........>D
-000106f0: 6976 6964 656e 6420 7461 7865 7320 6172  ividend taxes ar
-00010700: 6520 6e6f 7420 7375 7070 6f72 7465 6420  e not supported 
-00010710: 666f 7220 4b49 5420 6272 6f6b 6572 2073  for KIT broker s
-00010720: 7461 7465 6d65 6e74 7320 7965 7407 0000  tatements yet...
-00010730: 000c 5374 6174 656d 656e 744b 4954 0103  ..StatementKIT..
-00010740: 0000 0014 041a 0418 0422 0020 0424 0438  .........". .$.8
-00010750: 043d 0430 043d 0441 0800 0000 0006 0000  .=.0.=.A........
-00010760: 000b 4b49 5420 4669 6e61 6e63 6507 0000  ..KIT Finance...
-00010770: 000c 5374 6174 656d 656e 744b 4954 0103  ..StatementKIT..
-00010780: 0000 0032 041e 0442 0447 0451 0442 0020  ...2...B.G.Q.B. 
-00010790: 041a 0418 0422 0020 0424 0438 043d 0430  .....". .$.8.=.0
-000107a0: 043d 0441 0020 0028 002a 002e 0078 006c  .=.A. .(.*...x.l
-000107b0: 0073 0078 0029 0800 0000 0006 0000 001e  .s.x.)..........
-000107c0: 4b49 5420 4669 6e61 6e63 6520 7374 6174  KIT Finance stat
-000107d0: 656d 656e 7420 282a 2e78 6c73 7829 0700  ement (*.xlsx)..
-000107e0: 0000 0c53 7461 7465 6d65 6e74 4b49 5401  ...StatementKIT.
-000107f0: 0300 0000 2404 2104 3404 3504 3b04 3a04  ....$.!.4.5.;.:.
-00010800: 3800 2004 3704 3004 3304 4004 4304 3604  8. .7.0.3.@.C.6.
-00010810: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
-00010820: 0000 0f54 7261 6465 7320 6c6f 6164 6564  ...Trades loaded
-00010830: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00010840: 4b49 5401 0300 0000 3004 1d04 3504 3804  KIT.....0...5.8.
-00010850: 3704 3204 3504 4104 4204 3d04 4b04 3900  7.2.5.A.B.=.K.9.
-00010860: 2004 4204 3804 3f00 2004 4104 3404 3504   .B.8.?. .A.4.5.
-00010870: 3b04 3a04 3800 3a00 2008 0000 0000 0600  ;.:.8.:. .......
-00010880: 0000 1455 6e6b 6e6f 776e 2074 7261 6465  ...Unknown trade
-00010890: 2074 7970 653a 2007 0000 000c 5374 6174   type: .....Stat
-000108a0: 656d 656e 744b 4954 0103 0000 004a 041d  ementKIT.....J..
-000108b0: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
-000108c0: 0438 0432 0430 0435 043c 0430 044f 0020  .8.2.0.5.<.0.O. 
-000108d0: 0434 0435 043d 0435 0436 043d 0430 044f  .4.5.=.5.6.=.0.O
-000108e0: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
-000108f0: 0446 0438 044f 0020 0800 0000 0006 0000  .F.8.O. ........
-00010900: 001e 556e 7375 7070 706f 7274 6564 2063  ..Unsuppported c
-00010910: 6173 6820 7472 616e 7361 6374 696f 6e20  ash transaction 
-00010920: 0700 0000 0c53 7461 7465 6d65 6e74 4b49  .....StatementKI
-00010930: 5401 0300 0000 2204 2104 4704 3504 4204  T.....".!.G.5.B.
-00010940: 3000 2004 3704 3004 3304 4004 4304 3604  0. .7.0.3.@.C.6.
-00010950: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
-00010960: 0000 1141 6363 6f75 6e74 7320 6c6f 6164  ...Accounts load
-00010970: 6564 3a20 0700 0000 1353 7461 7465 6d65  ed: .....Stateme
-00010980: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00010990: 0064 041e 0442 0441 0443 0442 0441 0442  .d...B.A.C.B.A.B
-000109a0: 0432 0443 044e 0442 0020 0434 0430 043d  .2.C.N.B. .4.0.=
-000109b0: 043d 044b 0435 0020 0432 0020 043e 043f  .=.K.5. .2. .>.?
-000109c0: 0438 0441 0430 043d 0438 0438 0020 043f  .8.A.0.=.8.8. .?
-000109d0: 043e 0433 0430 0448 0435 043d 0438 044f  .>.3.0.H.5.=.8.O
-000109e0: 0020 043e 0431 043b 0438 0433 0430 0446  . .>.1.;.8.3.0.F
-000109f0: 0438 0438 0020 0800 0000 0006 0000 002a  .8.8. .........*
-00010a00: 426f 6e64 2072 6570 6179 6d65 6e74 2064  Bond repayment d
-00010a10: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
-00010a20: 736f 6d65 2064 6174 6120 0700 0000 1353  some data .....S
-00010a30: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
-00010a40: 6572 0103 0000 0068 041d 0435 0432 043e  er.....h...5.2.>
-00010a50: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
-00010a60: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
-00010a70: 044c 0020 043d 0430 0437 0432 0430 043d  .L. .=.0.7.2.0.=
-00010a80: 0438 0435 0020 043e 0431 043b 0438 0433  .8.5. .>.1.;.8.3
-00010a90: 0430 0446 0438 0438 0020 0432 0020 043e  .0.F.8.8. .2. .>
-00010aa0: 043f 0438 0441 0430 043d 0438 0438 0020  .?.8.A.0.=.8.8. 
-00010ab0: 0800 0000 0006 0000 0028 4361 6e27 7420  .........(Can't 
-00010ac0: 6465 7465 6374 2062 6f6e 6420 6e61 6d65  detect bond name
-00010ad0: 2066 726f 6d20 6465 7363 7269 7074 696f   from descriptio
-00010ae0: 6e20 0700 0000 1353 7461 7465 6d65 6e74  n .....Statement
-00010af0: 4f70 656e 4272 6f6b 6572 0103 0000 0062  OpenBroker.....b
-00010b00: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00010b10: 043d 043e 0020 043e 043f 0440 0435 0434  .=.>. .>.?.@.5.4
-00010b20: 0435 043b 0438 0442 044c 0020 0442 0438  .5.;.8.B.L. .B.8
-00010b30: 043f 002f 043a 043e 043b 0438 0447 0435  .?./.:.>.;.8.G.5
-00010b40: 0441 0442 0432 043e 0020 0434 043b 044f  .A.B.2.>. .4.;.O
-00010b50: 0020 0441 0434 0435 043b 043a 0438 003a  . .A.4.5.;.:.8.:
-00010b60: 0020 0800 0000 0006 0000 0025 4361 6e27  . .........%Can'
-00010b70: 7420 6465 7465 726d 696e 6520 7472 6164  t determine trad
-00010b80: 6520 7479 7065 2f71 7561 6e74 6974 793a  e type/quantity:
-00010b90: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
-00010ba0: 7065 6e42 726f 6b65 7201 0300 0000 6804  penBroker.....h.
-00010bb0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00010bc0: 3d04 3e00 2004 3e04 3f04 4004 3504 3404  =.>. .>.?.@.5.4.
-00010bd0: 3504 3b04 3804 4204 4c00 2004 4104 4704  5.;.8.B.L. .A.G.
-00010be0: 5104 4200 2004 3404 3b04 4f00 2004 3404  Q.B. .4.;.O. .4.
-00010bf0: 3504 3d04 3504 3604 3d04 3e04 3900 2004  5.=.5.6.=.>.9. .
-00010c00: 4204 4004 3004 3d04 3704 3004 3a04 4604  B.@.0.=.7.0.:.F.
-00010c10: 3804 3800 3a00 2008 0000 0000 0600 0000  8.8.:. .........
-00010c20: 2743 616e 2774 2066 696e 6420 6163 636f  'Can't find acco
-00010c30: 756e 7420 666f 7220 6361 7368 206f 7065  unt for cash ope
-00010c40: 7261 7469 6f6e 3a20 0700 0000 1353 7461  ration: .....Sta
-00010c50: 7465 6d65 6e74 4f70 656e 4272 6f6b 6572  tementOpenBroker
-00010c60: 0103 0000 0044 041d 0435 0432 043e 0437  .....D...5.2.>.7
-00010c70: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
-00010c80: 0439 0442 0438 0020 0441 0447 0451 0442  .9.B.8. .A.G.Q.B
-00010c90: 0020 0434 043b 044f 0020 0441 0434 0435  . .4.;.O. .A.4.5
-00010ca0: 043b 043a 0438 003a 0020 0800 0000 0006  .;.:.8.:. ......
-00010cb0: 0000 001e 4361 6e27 7420 6669 6e64 2061  ....Can't find a
-00010cc0: 6363 6f75 6e74 2066 6f72 2074 7261 6465  ccount for trade
-00010cd0: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
-00010ce0: 4f70 656e 4272 6f6b 6572 0103 0000 0050  OpenBroker.....P
-00010cf0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
-00010d00: 043d 043e 0020 043d 0430 0439 0442 0438  .=.>. .=.0.9.B.8
-00010d10: 0020 0437 0430 043f 0438 0441 044c 0020  . .7.0.?.8.A.L. 
-00010d20: 0441 043f 0438 0441 0430 043d 0438 044f  .A.?.8.A.0.=.8.O
-00010d30: 0020 0426 0411 0020 0434 043b 044f 0020  . .&... .4.;.O. 
-00010d40: 0800 0000 0006 0000 0029 4361 6e27 7420  .........)Can't 
-00010d50: 6669 6e64 2061 7373 6574 2063 616e 6365  find asset cance
-00010d60: 6c6c 6174 696f 6e20 7265 636f 7264 2066  llation record f
-00010d70: 6f72 2007 0000 0013 5374 6174 656d 656e  or .....Statemen
-00010d80: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
-00010d90: 3204 1d04 3500 2004 3d04 3004 3904 3404  2...5. .=.0.9.4.
-00010da0: 3504 3d04 3000 2004 2604 1100 2004 3404  5.=.0. .&... .4.
-00010db0: 3b04 4f00 2004 3a04 4304 3f04 3e04 3d04  ;.O. .:.C.?.>.=.
-00010dc0: 3000 2008 0000 0000 0600 0000 2343 616e  0. .........#Can
-00010dd0: 2774 2066 696e 6420 6173 7365 7420 666f  't find asset fo
-00010de0: 7220 626f 6e64 2069 6e74 6572 6573 7420  r bond interest 
-00010df0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00010e00: 656e 4272 6f6b 6572 0103 0000 003c 041d  enBroker.....<..
-00010e10: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00010e20: 043e 0020 0441 043e 043f 043e 0441 0442  .>. .A.>.?.>.A.B
-00010e30: 0430 0432 0438 0442 044c 0020 0426 0411  .0.2.8.B.L. .&..
-00010e40: 0020 0434 043b 044f 0020 0800 0000 0006  . .4.;.O. ......
-00010e50: 0000 0016 4361 6e27 7420 6d61 7463 6820  ....Can't match 
-00010e60: 6173 7365 7420 666f 7220 0700 0000 1353  asset for .....S
-00010e70: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
-00010e80: 6572 0103 0000 0066 041d 0435 0432 043e  er.....f...5.2.>
-00010e90: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
-00010ea0: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
-00010eb0: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
-00010ec0: 0438 0435 0020 043f 043e 0433 0430 0448  .8.5. .?.>.3.0.H
-00010ed0: 0435 043d 0438 044f 0020 043e 0431 043b  .5.=.8.O. .>.1.;
-00010ee0: 0438 0433 0430 0446 0438 0438 0020 0800  .8.3.0.F.8.8. ..
-00010ef0: 0000 0006 0000 0024 4361 6e27 7420 7061  .......$Can't pa
-00010f00: 7273 6520 426f 6e64 204d 6174 7572 6520  rse Bond Mature 
-00010f10: 6465 7363 7269 7074 696f 6e20 0700 0000  description ....
-00010f20: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
-00010f30: 6f6b 6572 0103 0000 004c 041d 0435 0432  oker.....L...5.2
-00010f40: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-00010f50: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
-00010f60: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
-00010f70: 043d 0438 0435 0020 043a 0443 043f 043e  .=.8.5. .:.C.?.>
-00010f80: 043d 0430 0020 0800 0000 0006 0000 0021  .=.0. .........!
-00010f90: 4361 6e27 7420 7061 7273 6520 496e 7465  Can't parse Inte
-00010fa0: 7265 7374 2064 6573 6372 6970 7469 6f6e  rest description
-00010fb0: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
-00010fc0: 7065 6e42 726f 6b65 7201 0300 0000 6604  penBroker.....f.
-00010fd0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00010fe0: 3d04 3e00 2004 4004 3004 4104 3f04 3e04  =.>. .@.0.A.?.>.
-00010ff0: 3704 3d04 3004 4204 4c00 2004 3e04 3f04  7.=.0.B.L. .>.?.
-00011000: 3804 4104 3004 3d04 3804 3500 2004 3f04  8.A.0.=.8.5. .?.
-00011010: 3e04 3304 3004 4804 3504 3d04 3804 4f00  >.3.0.H.5.=.8.O.
-00011020: 2004 3e04 3104 3b04 3804 3304 3004 4604   .>.1.;.8.3.0.F.
-00011030: 3804 3800 2008 0000 0000 0600 0000 2743  8.8. .........'C
-00011040: 616e 2774 2070 6172 7365 2062 6f6e 6420  an't parse bond 
-00011050: 7265 7061 796d 656e 7420 6465 7363 7269  repayment descri
-00011060: 7074 696f 6e20 0700 0000 1353 7461 7465  ption .....State
-00011070: 6d65 6e74 4f70 656e 4272 6f6b 6572 0103  mentOpenBroker..
-00011080: 0000 003a 0414 0435 043d 0435 0436 043d  ...:...5.=.5.6.=
-00011090: 044b 0445 0020 043e 043f 0435 0440 0430  .K.E. .>.?.5.@.0
-000110a0: 0446 0438 0439 0020 0437 0430 0433 0440  .F.8.9. .7.0.3.@
-000110b0: 0443 0436 0435 043d 043e 003a 0020 0800  .C.6.5.=.>.:. ..
-000110c0: 0000 0006 0000 0018 4361 7368 206f 7065  ........Cash ope
-000110d0: 7261 7469 6f6e 7320 6c6f 6164 6564 3a20  rations loaded: 
-000110e0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-000110f0: 656e 4272 6f6b 6572 0103 0000 0048 041e  enBroker.....H..
-00011100: 0442 0441 0443 0442 0441 0442 0432 0443  .B.A.C.B.A.B.2.C
-00011110: 044e 0442 0020 0434 0430 043d 043d 044b  .N.B. .4.0.=.=.K
-00011120: 0435 0020 0432 0020 043e 043f 0438 0441  .5. .2. .>.?.8.A
-00011130: 0430 043d 0438 0020 043a 0443 043f 043e  .0.=.8. .:.C.?.>
-00011140: 043d 0430 0020 0800 0000 0006 0000 0024  .=.0. .........$
-00011150: 496e 7465 7265 7374 2064 6573 6372 6970  Interest descrip
-00011160: 7469 6f6e 206d 6973 7320 736f 6d65 2064  tion miss some d
-00011170: 6174 6120 0700 0000 1353 7461 7465 6d65  ata .....Stateme
-00011180: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
-00011190: 0054 0417 0430 0433 0440 0443 0437 043a  .T...0.3.@.C.7.:
-000111a0: 0430 0020 043e 0442 0447 0451 0442 0430  .0. .>.B.G.Q.B.0
-000111b0: 0020 041e 0442 043a 0440 044b 0442 0438  . ...B.:.@.K.B.8
-000111c0: 0435 0020 0431 0440 043e 043a 0435 0440  .5. .1.@.>.:.5.@
-000111d0: 0020 0434 043b 044f 0020 0441 0447 0451  . .4.;.O. .A.G.Q
-000111e0: 0442 0430 0020 0800 0000 0006 0000 0027  .B.0. .........'
-000111f0: 4c6f 6164 204f 7065 6e20 4272 6f6b 6572  Load Open Broker
-00011200: 2073 7461 7465 6d65 6e74 2066 6f72 2061   statement for a
-00011210: 6363 6f75 6e74 2007 0000 0013 5374 6174  ccount .....Stat
-00011220: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
-00011230: 0300 0000 5604 1d04 3004 3904 3404 3504  ....V...0.9.4.5.
-00011240: 3d04 4b00 2004 3d04 3504 4104 3a04 3e04  =.K. .=.5.A.:.>.
-00011250: 3b04 4c04 3a04 3e00 2004 3704 3004 3f04  ;.L.:.>. .7.0.?.
-00011260: 3804 4104 3504 3900 2004 3f04 3e04 3304  8.A.5.9. .?.>.3.
-00011270: 3004 4804 3504 3d04 3804 4f00 2004 2604  0.H.5.=.8.O. .&.
-00011280: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
-00011290: 0600 0000 264d 756c 7469 706c 6520 6173  ....&Multiple as
-000112a0: 7365 7420 6361 6e63 656c 6c61 7469 6f6e  set cancellation
-000112b0: 206d 6174 6368 2066 6f72 2007 0000 0013   match for .....
-000112c0: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
-000112d0: 6b65 7201 0300 0000 7404 1d04 3504 4104  ker.....t...5.A.
-000112e0: 3a04 3e04 3b04 4c04 3a04 3e00 2004 4104  :.>.;.L.:.>. .A.
-000112f0: 3e04 3204 3f04 3004 3404 3504 3d04 3804  >.2.?.0.4.5.=.8.
-00011300: 3900 2004 3404 3b04 4f00 2004 4104 3804  9. .4.;.O. .A.8.
-00011310: 3c04 3204 3e04 3b04 3000 2c00 2004 3804  <.2.>.;.0.,. .8.
-00011320: 4104 3f04 3e04 3b04 4c04 3704 4304 3504  A.?.>.;.L.7.C.5.
-00011330: 3c04 3e04 3304 3e00 2004 3104 4004 3e04  <.>.3.>. .1.@.>.
-00011340: 3a04 3504 4004 3e04 3c00 3a00 2008 0000  :.5.@.>.<.:. ...
-00011350: 0000 0600 0000 224d 756c 7469 706c 6520  ......"Multiple 
-00011360: 6d61 7463 6820 666f 7220 6272 6f6b 6572  match for broker
-00011370: 2073 796d 626f 6c3a 2007 0000 0013 5374   symbol: .....St
-00011380: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
-00011390: 7201 0300 0000 4404 1d04 3504 4104 3a04  r.....D...5.A.:.
-000113a0: 3e04 3b04 4c04 3a04 3e00 2004 4104 3e04  >.;.L.:.>. .A.>.
-000113b0: 3204 3f04 3004 3404 3504 3d04 3804 3900  2.?.0.4.5.=.8.9.
-000113c0: 2004 3404 3b04 4f00 2004 4104 3804 3c04   .4.;.O. .A.8.<.
-000113d0: 3204 3e04 3b04 3000 3a00 2008 0000 0000  2.>.;.0.:. .....
-000113e0: 0600 0000 1b4d 756c 7469 706c 6520 6d61  .....Multiple ma
-000113f0: 7463 6820 666f 7220 7379 6d62 6f6c 3a20  tch for symbol: 
-00011400: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011410: 656e 4272 6f6b 6572 0103 0000 001e 041e  enBroker........
-00011420: 0442 043a 0440 044b 0442 0438 0435 0020  .B.:.@.K.B.8.5. 
-00011430: 0431 0440 043e 043a 0435 0440 0800 0000  .1.@.>.:.5.@....
-00011440: 0006 0000 000b 4f70 656e 2042 726f 6b65  ......Open Broke
-00011450: 7207 0000 0013 5374 6174 656d 656e 744f  r.....StatementO
-00011460: 7065 6e42 726f 6b65 7201 0300 0000 3c04  penBroker.....<.
-00011470: 1e04 4204 4704 5104 4200 2004 3104 4004  ..B.G.Q.B. .1.@.
-00011480: 3e04 3a04 3504 4004 3000 2004 1e04 4204  >.:.5.@.0. ...B.
-00011490: 3a04 4004 4b04 4204 3804 3500 2000 2800  :.@.K.B.8.5. .(.
-000114a0: 2a00 2e00 7800 6d00 6c00 2908 0000 0000  *...x.m.l.).....
-000114b0: 0600 0000 1d4f 7065 6e20 4272 6f6b 6572  .....Open Broker
-000114c0: 2073 7461 7465 6d65 6e74 2028 2a2e 786d   statement (*.xm
-000114d0: 6c29 0700 0000 1353 7461 7465 6d65 6e74  l).....Statement
-000114e0: 4f70 656e 4272 6f6b 6572 0103 0000 0054  OpenBroker.....T
-000114f0: 0417 0430 0433 043e 043b 043e 0432 043e  ...0.3.>.;.>.2.>
-00011500: 043a 0020 043e 0442 0447 0451 0442 0430  .:. .>.B.G.Q.B.0
-00011510: 0020 041e 0442 043a 0440 044b 0442 0438  . ...B.:.@.K.B.8
-00011520: 0435 0020 0431 0440 043e 043a 0435 0440  .5. .1.@.>.:.5.@
-00011530: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
-00011540: 0435 043d 0800 0000 0006 0000 0022 4f70  .5.=........."Op
-00011550: 656e 2062 726f 6b65 7220 7265 706f 7274  en broker report
-00011560: 2074 6974 6c65 206e 6f74 2066 6f75 6e64   title not found
-00011570: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011580: 656e 4272 6f6b 6572 0103 0000 0038 041e  enBroker.....8..
-00011590: 043f 0435 0440 0430 0446 0438 044f 0020  .?.5.@.0.F.8.O. 
-000115a0: 043d 0435 0020 043f 043e 0434 0434 0435  .=.5. .?.>.4.4.5
-000115b0: 0440 0436 0438 0432 0430 0435 0442 0441  .@.6.8.2.0.5.B.A
-000115c0: 044f 003a 0020 0800 0000 0006 0000 0019  .O.:. ..........
-000115d0: 4f70 6572 6174 696f 6e20 6e6f 7420 7375  Operation not su
-000115e0: 7070 6f72 7465 643a 2007 0000 0013 5374  pported: .....St
-000115f0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
-00011600: 7201 0300 0000 1c04 2604 1100 2004 3704  r.......&... .7.
-00011610: 3004 3304 4004 4304 3604 3504 3d04 4b00  0.3.@.C.6.5.=.K.
-00011620: 3a00 2008 0000 0000 0600 0000 1353 6563  :. ..........Sec
-00011630: 7572 6974 6965 7320 6c6f 6164 6564 3a20  urities loaded: 
-00011640: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011650: 656e 4272 6f6b 6572 0103 0000 006e 041d  enBroker.....n..
-00011660: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
-00011670: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
-00011680: 0437 0430 0433 043e 043b 043e 0432 043e  .7.0.3.>.;.>.2.>
-00011690: 043a 0020 043e 0442 0447 0451 0442 0430  .:. .>.B.G.Q.B.0
-000116a0: 0020 0434 043b 044f 0020 041e 0442 043a  . .4.;.O. ...B.:
-000116b0: 0440 044b 0442 0438 0435 0020 0431 0440  .@.K.B.8.5. .1.@
-000116c0: 043e 043a 0435 0440 003a 0020 0800 0000  .>.:.5.@.:. ....
-000116d0: 0006 0000 0026 556e 6578 7065 6374 6564  .....&Unexpected
-000116e0: 204f 7065 6e20 6272 6f6b 6572 2072 6570   Open broker rep
-000116f0: 6f72 7420 6865 6164 6572 3a20 0700 0000  ort header: ....
-00011700: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
-00011710: 6f6b 6572 0103 0000 0042 041d 0435 0438  oker.....B...5.8
-00011720: 0437 0432 0435 0441 0442 043d 0430 044f  .7.2.5.A.B.=.0.O
-00011730: 0020 043d 0435 0442 043e 0440 0433 043e  . .=.5.B.>.@.3.>
-00011740: 0432 0430 044f 0020 043e 043f 0435 0440  .2.0.O. .>.?.5.@
-00011750: 0430 0446 0438 044f 003a 0020 0800 0000  .0.F.8.O.:. ....
-00011760: 0006 0000 001d 556e 6b6e 6f77 6e20 6e6f  ......Unknown no
-00011770: 6e2d 7472 6164 6520 6f70 6572 6174 696f  n-trade operatio
-00011780: 6e3a 2007 0000 0013 5374 6174 656d 656e  n: .....Statemen
-00011790: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
-000117a0: 4604 1d04 3504 3f04 3e04 3404 3404 3504  F...5.?.>.4.4.5.
-000117b0: 4004 3604 3804 3204 3004 3504 3c04 3e04  @.6.8.2.0.5.<.>.
-000117c0: 3500 2004 3e04 3f04 3804 4104 3004 3d04  5. .>.?.8.A.0.=.
-000117d0: 3804 3500 2004 3f04 3b04 3004 4204 3504  8.5. .?.;.0.B.5.
-000117e0: 3604 3000 3a00 2008 0000 0000 0600 0000  6.0.:. .........
-000117f0: 1d55 6e6b 6e6f 776e 2070 6179 6d65 6e74  .Unknown payment
-00011800: 2064 6573 6372 6970 7469 6f6e 3a20 0700   description: ..
-00011810: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-00011820: 4272 6f6b 6572 0103 0000 0032 041d 0435  Broker.....2...5
-00011830: 0438 0437 0432 0435 0441 0442 043d 044b  .8.7.2.5.A.B.=.K
-00011840: 0439 0020 0442 0438 043f 0020 043f 043b  .9. .B.8.?. .?.;
-00011850: 0430 0442 0435 0436 0430 003a 0020 0800  .0.B.5.6.0.:. ..
-00011860: 0000 0006 0000 0016 556e 6b6e 6f77 6e20  ........Unknown 
-00011870: 7061 796d 656e 7420 7479 7065 3a20 0700  payment type: ..
-00011880: 0000 1353 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-00011890: 4272 6f6b 6572 0103 0000 0016 0426 0411  Broker.......&..
-000118a0: 0020 0431 0435 0437 0020 0069 0064 003a  . .1.5.7. .i.d.:
-000118b0: 0020 0800 0000 0006 0000 0012 4173 7365  . ..........Asse
-000118c0: 7420 7769 7468 6f75 7420 6964 3a20 0700  t without id: ..
-000118d0: 0000 1653 7461 7465 6d65 6e74 4f70 656e  ...StatementOpen
-000118e0: 506f 7274 666f 6c69 6f01 0300 0000 4804  Portfolio.....H.
-000118f0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-00011900: 3d04 3e00 2004 3f04 4004 3e04 4704 3804  =.>. .?.@.>.G.8.
-00011910: 4204 3004 4204 4c00 2000 4a00 5300 4f00  B.0.B.L. .J.S.O.
-00011920: 4e00 2004 3804 3700 2004 4404 3004 3904  N. .8.7. .D.0.9.
-00011930: 3b04 3000 3a00 2008 0000 0000 0600 0000  ;.0.:. .........
-00011940: 1f46 6169 6c65 6420 746f 2072 6561 6420  .Failed to read 
-00011950: 4a53 4f4e 2066 726f 6d20 6669 6c65 3a20  JSON from file: 
-00011960: 0700 0000 1653 7461 7465 6d65 6e74 4f70  .....StatementOp
-00011970: 656e 506f 7274 666f 6c69 6f01 0300 0000  enPortfolio.....
-00011980: 3404 1d04 3504 3204 3e04 3704 3c04 3e04  4...5.2.>.7.<.>.
-00011990: 3604 3d04 3e00 2004 3f04 4004 3e04 4704  6.=.>. .?.@.>.G.
-000119a0: 3504 4104 4204 4c00 2004 4404 3004 3904  5.A.B.L. .D.0.9.
-000119b0: 3b00 3a00 2008 0000 0000 0600 0000 1546  ;.:. ..........F
-000119c0: 6169 6c65 6420 746f 2072 6561 6420 6669  ailed to read fi
-000119d0: 6c65 3a20 0700 0000 1653 7461 7465 6d65  le: .....Stateme
-000119e0: 6e74 4f70 656e 506f 7274 666f 6c69 6f01  ntOpenPortfolio.
-000119f0: 0300 0000 2204 1804 3c04 3f04 3e04 4004  ...."...<.?.>.@.
-00011a00: 4204 3804 4004 3e04 3204 3004 3d04 3d04  B.8.@.>.2.0.=.=.
-00011a10: 4b04 3900 2021 1608 0000 0000 0600 0000  K.9. !..........
-00011a20: 0a49 6d70 6f72 7465 6420 2307 0000 0016  .Imported #.....
-00011a30: 5374 6174 656d 656e 744f 7065 6e50 6f72  StatementOpenPor
-00011a40: 7466 6f6c 696f 0103 0000 002e 0049 006e  tfolio.......I.n
-00011a50: 0076 0065 0073 0074 0062 006f 006f 006b  .v.e.s.t.b.o.o.k
-00011a60: 0020 002f 0020 0049 005a 0049 002d 0069  . ./. .I.Z.I.-.i
-00011a70: 006e 0076 0065 0073 0074 0800 0000 0006  .n.v.e.s.t......
-00011a80: 0000 0017 496e 7665 7374 626f 6f6b 202f  ....Investbook /
-00011a90: 2049 5a49 2d49 6e76 6573 7407 0000 0016   IZI-Invest.....
-00011aa0: 5374 6174 656d 656e 744f 7065 6e50 6f72  StatementOpenPor
-00011ab0: 7466 6f6c 696f 0103 0000 0042 041e 0431  tfolio.....B...1
-00011ac0: 044f 0437 0430 0442 0435 043b 044c 043d  .O.7.0.B.5.;.L.=
-00011ad0: 0430 044f 0020 0441 0435 043a 0446 0438  .0.O. .A.5.:.F.8
-00011ae0: 044f 0020 043e 0442 0441 0443 0442 0441  .O. .>.B.A.C.B.A
-00011af0: 0442 0432 0443 0435 0442 003a 0020 0800  .B.2.C.5.B.:. ..
-00011b00: 0000 0006 0000 001e 4d61 6e64 6174 6f72  ........Mandator
-00011b10: 7920 7365 6374 696f 6e20 6973 206d 6973  y section is mis
-00011b20: 7369 6e67 3a20 0700 0000 1653 7461 7465  sing: .....State
-00011b30: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
-00011b40: 6f01 0300 0000 2e00 4f00 7000 6500 6e00  o.......O.p.e.n.
-00011b50: 2000 7000 6f00 7200 7400 6600 6f00 6c00   .p.o.r.t.f.o.l.
-00011b60: 6900 6f00 2000 2800 2a00 2e00 6a00 7300  i.o. .(.*...j.s.
-00011b70: 6f00 6e00 2908 0000 0000 0600 0000 174f  o.n.)..........O
-00011b80: 7065 6e20 706f 7274 666f 6c69 6f20 282a  pen portfolio (*
-00011b90: 2e6a 736f 6e29 0700 0000 1653 7461 7465  .json).....State
-00011ba0: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
-00011bb0: 6f01 0300 0000 4e04 1d04 3504 3f04 3e04  o.....N...5.?.>.
-00011bc0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00011bd0: 3504 3c04 3004 4f00 2004 3204 3504 4004  5.<.0.O. .2.5.@.
-00011be0: 4104 3804 4f00 2004 4404 3e04 4004 3c04  A.8.O. .D.>.@.<.
-00011bf0: 3004 4204 3000 2004 4404 3004 3904 3b04  0.B.0. .D.0.9.;.
-00011c00: 3000 3a00 2008 0000 0000 0600 0000 2e55  0.:. ..........U
-00011c10: 6e73 7570 706f 7274 6564 2076 6572 7369  nsupported versi
-00011c20: 6f6e 206f 6620 6f70 656e 2070 6f72 7466  on of open portf
-00011c30: 6f6c 696f 2066 6f72 6d61 743a 2007 0000  olio format: ...
-00011c40: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
-00011c50: 6f72 7466 6f6c 696f 0103 0000 0038 041a  ortfolio.....8..
-00011c60: 0443 043f 043e 043d 044b 0020 043e 0431  .C.?.>.=.K. .>.1
-00011c70: 043b 0438 0433 0430 0446 0438 0439 0020  .;.8.3.0.F.8.9. 
-00011c80: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-00011c90: 044b 003a 0020 0800 0000 0006 0000 0017  .K.:. ..........
-00011ca0: 426f 6e64 2069 6e74 6572 6573 7473 206c  Bond interests l
-00011cb0: 6f61 6465 643a 2007 0000 000c 5374 6174  oaded: .....Stat
-00011cc0: 656d 656e 7450 5342 0103 0000 003e 0414  ementPSB.....>..
-00011cd0: 0435 043d 0435 0436 043d 044b 0435 0020  .5.=.5.6.=.K.5. 
-00011ce0: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
-00011cf0: 0438 0438 0020 0437 0430 0433 0440 0443  .8.8. .7.0.3.@.C
-00011d00: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
-00011d10: 0006 0000 001a 4361 7368 2074 7261 6e73  ......Cash trans
-00011d20: 6163 7469 6f6e 7320 6c6f 6164 6564 3a20  actions loaded: 
-00011d30: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
-00011d40: 4201 0300 0000 2a04 1404 3804 3204 3804  B.....*...8.2.8.
-00011d50: 3404 3504 3d04 3404 4b00 2004 3704 3004  4.5.=.4.K. .7.0.
-00011d60: 3304 4004 4304 3604 3504 3d04 4b00 3a00  3.@.C.6.5.=.K.:.
-00011d70: 2008 0000 0000 0600 0000 1244 6976 6964   ..........Divid
-00011d80: 656e 6473 206c 6f61 6465 643a 2007 0000  ends loaded: ...
-00011d90: 000c 5374 6174 656d 656e 7450 5342 0103  ..StatementPSB..
-00011da0: 0000 0014 041f 0421 0411 002d 0431 0440  .......!...-.1.@
-00011db0: 043e 043a 0435 0440 0800 0000 0006 0000  .>.:.5.@........
-00011dc0: 000a 5053 4220 4272 6f6b 6572 0700 0000  ..PSB Broker....
-00011dd0: 0c53 7461 7465 6d65 6e74 5053 4201 0300  .StatementPSB...
-00011de0: 0000 4004 1e04 4204 4704 5104 4200 2004  ..@...B.G.Q.B. .
-00011df0: 3104 4004 3e04 3a04 3504 4004 3000 2004  1.@.>.:.5.@.0. .
-00011e00: 1f04 2104 1100 2000 2800 2a00 2e00 7800  ..!... .(.*...x.
-00011e10: 6c00 7300 7800 2000 2a00 2e00 7800 6c00  l.s.x. .*...x.l.
-00011e20: 7300 2908 0000 0000 0600 0000 2350 5342  s.).........#PSB
-00011e30: 2062 726f 6b65 7220 7374 6174 656d 656e   broker statemen
-00011e40: 7420 282a 2e78 6c73 7820 2a2e 786c 7329  t (*.xlsx *.xls)
-00011e50: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
-00011e60: 4201 03ff ffff ff08 0000 0000 0600 0000  B...............
-00011e70: 0f54 7261 6465 7320 6c6f 6164 6564 3a20  .Trades loaded: 
-00011e80: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
-00011e90: 4201 0300 0000 4004 1d04 3504 3f04 3e04  B.....@...5.?.>.
-00011ea0: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
-00011eb0: 3504 3c04 3004 4f00 2004 3e04 3f04 3504  5.<.0.O. .>.?.5.
-00011ec0: 4004 3004 4604 3804 4f00 2004 4100 2004  @.0.F.8.O. .A. .
-00011ed0: 1404 2100 3a00 2008 0000 0000 0600 0000  ..!.:. .........
-00011ee0: 1855 6e6b 6e6f 776e 2063 6173 6820 6f70  .Unknown cash op
-00011ef0: 6572 6174 696f 6e3a 2007 0000 000c 5374  eration: .....St
-00011f00: 6174 656d 656e 7450 5342 0103 0000 003a  atementPSB.....:
-00011f10: 041d 0435 0438 0437 0432 0435 0441 0442  ...5.8.7.2.5.A.B
-00011f20: 043d 044b 0439 0020 0442 0438 043f 0020  .=.K.9. .B.8.?. 
-00011f30: 0434 0432 0438 0436 0435 043d 0438 044f  .4.2.8.6.5.=.8.O
-00011f40: 0020 0414 0421 003a 0020 0800 0000 0006  . ...!.:. ......
-00011f50: 0000 001a 556e 6b6e 6f77 6e20 6361 7368  ....Unknown cash
-00011f60: 2074 7261 6e73 6163 7469 6f6e 3a20 0700   transaction: ..
-00011f70: 0000 0c53 7461 7465 6d65 6e74 5053 4201  ...StatementPSB.
-00011f80: 0300 0000 3004 1d04 3504 3804 3704 3204  ....0...5.8.7.2.
-00011f90: 3504 4104 4204 3d04 4b04 3900 2004 4204  5.A.B.=.K.9. .B.
-00011fa0: 3804 3f00 2004 4104 3404 3504 3b04 3a04  8.?. .A.4.5.;.:.
-00011fb0: 3800 3a00 2008 0000 0000 0600 0000 1455  8.:. ..........U
-00011fc0: 6e6b 6e6f 776e 2074 7261 6465 2074 7970  nknown trade typ
-00011fd0: 653a 2007 0000 000c 5374 6174 656d 656e  e: .....Statemen
-00011fe0: 7450 5342 0103 0000 0032 041d 0435 043f  tPSB.....2...5.?
-00011ff0: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
-00012000: 0430 0435 043c 044b 0439 0020 043f 043b  .0.5.<.K.9. .?.;
-00012010: 0430 0442 0451 0436 003a 0020 0800 0000  .0.B.Q.6.:. ....
-00012020: 0006 0000 0015 556e 7375 7070 6f72 7465  ......Unsupporte
-00012030: 6420 7061 796d 656e 743a 2007 0000 000c  d payment: .....
-00012040: 5374 6174 656d 656e 7450 5342 0103 0000  StatementPSB....
-00012050: 005a 0421 0434 0435 043b 043a 0430 0020  .Z.!.4.5.;.:.0. 
-00012060: 0441 0020 0440 0430 0437 043d 044b 043c  .A. .@.0.7.=.K.<
-00012070: 0438 0020 0432 0430 043b 044e 0442 0430  .8. .2.0.;.N.B.0
-00012080: 043c 0438 0020 043d 0435 0020 043f 043e  .<.8. .=.5. .?.>
-00012090: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
-000120a0: 0435 0442 0441 044f 003a 0020 0800 0000  .5.B.A.O.:. ....
-000120b0: 0006 0000 002d 556e 7375 7070 6f72 7465  .....-Unsupporte
-000120c0: 6420 7472 6164 6520 7769 7468 2064 6966  d trade with dif
-000120d0: 6665 7265 6e74 2063 7572 7265 6e63 6965  ferent currencie
-000120e0: 733a 2007 0000 000c 5374 6174 656d 656e  s: .....Statemen
-000120f0: 7450 5342 0103 0000 0032 041e 043f 0435  tPSB.....2...?.5
-00012100: 0440 0430 0446 0438 0438 0020 0441 0020  .@.0.F.8.8. .A. 
-00012110: 0426 0411 0020 0437 0430 0433 0440 0443  .&... .7.0.3.@.C
-00012120: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
-00012130: 0006 0000 0019 4173 7365 7420 6f70 6572  ......Asset oper
-00012140: 6174 696f 6e73 206c 6f61 6465 643a 2007  ations loaded: .
-00012150: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
-00012160: 5501 0300 0000 6804 1e04 4204 4104 4304  U.....h...B.A.C.
-00012170: 4204 4104 4204 3204 4304 4e04 4200 2004  B.A.B.2.C.N.B. .
-00012180: 3e04 3604 3804 3404 3004 3504 3c04 4b04  >.6.8.4.0.5.<.K.
-00012190: 3500 2004 3404 3004 3d04 3d04 4b04 3500  5. .4.0.=.=.K.5.
-000121a0: 2004 3200 2004 3e04 3f04 3804 4104 3004   .2. .>.?.8.A.0.
-000121b0: 3d04 3804 3800 2004 3f04 3504 4004 3504  =.8.8. .?.5.@.5.
-000121c0: 3204 3e04 3404 3000 2004 2604 1100 2008  2.>.4.0. .&... .
-000121d0: 0000 0000 0600 0000 2a41 7373 6574 2074  ........*Asset t
-000121e0: 7261 6e73 6665 7220 6465 7363 7269 7074  ransfer descript
-000121f0: 696f 6e20 6d69 7373 2073 6f6d 6520 6461  ion miss some da
-00012200: 7461 2007 0000 000d 5374 6174 656d 656e  ta .....Statemen
-00012210: 7455 4b46 5501 0300 0000 5004 1d04 3504  tUKFU.....P...5.
-00012220: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-00012230: 2004 3d04 3004 3904 4204 3800 2004 3704   .=.0.9.B.8. .7.
-00012240: 3004 3f04 3804 4104 4c00 2004 4104 3f04  0.?.8.A.L. .A.?.
-00012250: 3804 4104 3004 3d04 3804 4f00 2004 2604  8.A.0.=.8.O. .&.
-00012260: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
-00012270: 0600 0000 2943 616e 2774 2066 696e 6420  ....)Can't find 
-00012280: 6173 7365 7420 6361 6e63 656c 6c61 7469  asset cancellati
-00012290: 6f6e 2072 6563 6f72 6420 666f 7220 0700  on record for ..
-000122a0: 0000 0d53 7461 7465 6d65 6e74 554b 4655  ...StatementUKFU
-000122b0: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
-000122c0: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
-000122d0: 0439 0442 0438 0020 0437 0430 0433 043e  .9.B.8. .7.0.3.>
-000122e0: 043b 043e 0432 043e 043a 0020 043a 043e  .;.>.2.>.:. .:.>
-000122f0: 043c 0438 0441 0441 0438 0439 0800 0000  .<.8.A.A.8.9....
-00012300: 0006 0000 001d 4361 6e27 7420 6765 7420  ......Can't get 
-00012310: 6865 6164 6572 2074 6f20 6669 6e64 2066  header to find f
-00012320: 6565 7307 0000 000d 5374 6174 656d 656e  ees.....Statemen
-00012330: 7455 4b46 5501 0300 0000 5604 1d04 3504  tUKFU.....V...5.
-00012340: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
-00012350: 2004 4004 3004 4104 3f04 3e04 3704 3d04   .@.0.A.?.>.7.=.
-00012360: 3004 4204 4c00 2004 3e04 3f04 3804 4104  0.B.L. .>.?.8.A.
-00012370: 3004 3d04 3804 3500 2004 3f04 3504 4004  0.=.8.5. .?.5.@.
-00012380: 3504 3204 3e04 3404 3000 2004 2604 1100  5.2.>.4.0. .&...
-00012390: 2008 0000 0000 0600 0000 2743 616e 2774   .........'Can't
-000123a0: 2070 6172 7365 2061 7373 6574 2074 7261   parse asset tra
-000123b0: 6e73 6665 7220 6465 7363 7269 7074 696f  nsfer descriptio
-000123c0: 6e20 0700 0000 0d53 7461 7465 6d65 6e74  n .....Statement
-000123d0: 554b 4655 0103 0000 004c 041d 0435 0432  UKFU.....L...5.2
-000123e0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
-000123f0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
-00012400: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
-00012410: 043d 0438 0435 0020 043a 0443 043f 043e  .=.8.5. .:.C.?.>
-00012420: 043d 0430 0020 0800 0000 0006 0000 0026  .=.0. .........&
-00012430: 4361 6e27 7420 7061 7273 6520 626f 6e64  Can't parse bond
-00012440: 2069 6e74 6572 6573 7420 6465 7363 7269   interest descri
-00012450: 7074 696f 6e20 0700 0000 0d53 7461 7465  ption .....State
-00012460: 6d65 6e74 554b 4655 0103 0000 0066 041d  mentUKFU.....f..
-00012470: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00012480: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
-00012490: 043d 0430 0442 044c 0020 043e 043f 0438  .=.0.B.L. .>.?.8
-000124a0: 0441 0430 043d 0438 0435 0020 043f 043e  .A.0.=.8.5. .?.>
-000124b0: 0433 0430 0448 0435 043d 0438 044f 0020  .3.0.H.5.=.8.O. 
-000124c0: 043e 0431 043b 0438 0433 0430 0446 0438  .>.1.;.8.3.0.F.8
-000124d0: 0438 0020 0800 0000 0006 0000 0027 4361  .8. .........'Ca
-000124e0: 6e27 7420 7061 7273 6520 626f 6e64 2072  n't parse bond r
-000124f0: 6570 6179 6d65 6e74 2064 6573 6372 6970  epayment descrip
-00012500: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
-00012510: 656e 7455 4b46 5501 0300 0000 5204 1d04  entUKFU.....R...
-00012520: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-00012530: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
-00012540: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
-00012550: 4104 3004 3d04 3804 3500 2004 3404 3804  A.0.=.8.5. .4.8.
-00012560: 3204 3804 3404 3504 3d04 3404 3000 2008  2.8.4.5.=.4.0. .
-00012570: 0000 0000 0600 0000 2143 616e 2774 2070  ........!Can't p
-00012580: 6172 7365 2064 6976 6964 656e 6420 6465  arse dividend de
-00012590: 7363 7269 7074 696f 6e20 0700 0000 0d53  scription .....S
-000125a0: 7461 7465 6d65 6e74 554b 4655 0103 0000  tatementUKFU....
-000125b0: 0064 041d 0435 0432 043e 0437 043c 043e  .d...5.2.>.7.<.>
-000125c0: 0436 043d 043e 0020 0440 0430 0441 043f  .6.=.>. .@.0.A.?
-000125d0: 043e 0437 043d 0430 0442 044c 0020 043e  .>.7.=.0.B.L. .>
-000125e0: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
-000125f0: 0434 0435 043d 0435 0436 043d 043e 0433  .4.5.=.5.6.=.>.3
-00012600: 043e 0020 043f 0435 0440 0435 0432 043e  .>. .?.5.@.5.2.>
-00012610: 0434 0430 0020 0800 0000 0006 0000 0027  .4.0. .........'
-00012620: 4361 6e27 7420 7061 7273 6520 6d6f 6e65  Can't parse mone
-00012630: 7920 7472 616e 7366 6572 2064 6573 6372  y transfer descr
-00012640: 6970 7469 6f6e 2007 0000 000d 5374 6174  iption .....Stat
-00012650: 656d 656e 7455 4b46 5501 0300 0000 3a04  ementUKFU.....:.
-00012660: 1404 3504 3d04 3504 3604 3d04 4b04 4500  ..5.=.5.6.=.K.E.
-00012670: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
-00012680: 3900 2004 3704 3004 3304 4004 4304 3604  9. .7.0.3.@.C.6.
-00012690: 3504 3d04 3e00 3a00 2008 0000 0000 0600  5.=.>.:. .......
-000126a0: 0000 1843 6173 6820 6f70 6572 6174 696f  ...Cash operatio
-000126b0: 6e73 206c 6f61 6465 643a 2007 0000 000d  ns loaded: .....
-000126c0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
-000126d0: 0000 4804 1e04 4804 3804 3104 3a04 3000  ..H...H.8.1.:.0.
-000126e0: 2004 3f04 4004 3800 2004 3a04 3e04 3d04   .?.@.8. .:.>.=.
-000126f0: 3204 3504 4004 4204 3004 4604 3804 3800  2.5.@.B.0.F.8.8.
-00012700: 2004 4104 4304 3c04 3c04 4b00 2004 3d04   .A.C.<.<.K. .=.
-00012710: 3004 3b04 3e04 3304 3000 2008 0000 0000  0.;.>.3.0. .....
-00012720: 0600 0000 1f46 6169 6c65 6420 746f 2063  .....Failed to c
-00012730: 6f6e 7665 7274 2064 6976 6964 656e 6420  onvert dividend 
-00012740: 7461 7820 0700 0000 0d53 7461 7465 6d65  tax .....Stateme
-00012750: 6e74 554b 4655 0103 0000 003e 0421 0434  ntUKFU.....>.!.4
-00012760: 0435 043b 043e 043a 0020 0441 0020 0444  .5.;.>.:. .A. .D
-00012770: 044c 044e 0447 0435 0440 0441 0430 043c  .L.N.G.5.@.A.0.<
-00012780: 0438 0020 0437 0430 0433 0440 0443 0436  .8. .7.0.3.@.C.6
-00012790: 0435 043d 043e 003a 0020 0800 0000 0006  .5.=.>.:. ......
-000127a0: 0000 0017 4675 7475 7265 7320 7472 6164  ....Futures trad
-000127b0: 6573 206c 6f61 6465 643a 2007 0000 000d  es loaded: .....
-000127c0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
-000127d0: 0000 7604 1e04 4204 4104 4304 4204 4104  ..v...B.A.C.B.A.
-000127e0: 4204 3204 4304 4e04 4200 2004 3e04 3604  B.2.C.N.B. .>.6.
-000127f0: 3804 3404 3004 3504 3c04 4b04 3500 2004  8.4.0.5.<.K.5. .
-00012800: 3404 3004 3d04 3d04 4b04 3500 2004 3200  4.0.=.=.K.5. .2.
-00012810: 2004 3e04 3f04 3804 4104 3004 3d04 3804   .>.?.8.A.0.=.8.
-00012820: 3800 2004 3404 3504 3d04 3504 3604 3d04  8. .4.5.=.5.6.=.
-00012830: 3e04 3304 3e00 2004 3f04 3504 4004 3504  >.3.>. .?.5.@.5.
-00012840: 3204 3e04 3404 3000 2008 0000 0000 0600  2.>.4.0. .......
-00012850: 0000 2a4d 6f6e 6579 2074 7261 6e73 6665  ..*Money transfe
-00012860: 7220 6465 7363 7269 7074 696f 6e20 6d69  r description mi
-00012870: 7373 2073 6f6d 6520 6461 7461 2007 0000  ss some data ...
-00012880: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
-00012890: 0300 0000 5604 1d04 3004 3904 3404 3504  ....V...0.9.4.5.
-000128a0: 3d04 4b00 2004 3d04 3504 4104 3a04 3e04  =.K. .=.5.A.:.>.
-000128b0: 3b04 4c04 3a04 3e00 2004 3704 3004 3f04  ;.L.:.>. .7.0.?.
-000128c0: 3804 4104 3504 3900 2004 3f04 3e04 3304  8.A.5.9. .?.>.3.
-000128d0: 3004 4804 3504 3d04 3804 4f00 2004 2604  0.H.5.=.8.O. .&.
-000128e0: 1100 2004 3404 3b04 4f00 2008 0000 0000  .. .4.;.O. .....
-000128f0: 0600 0000 264d 756c 7469 706c 6520 6173  ....&Multiple as
-00012900: 7365 7420 6361 6e63 656c 6c61 7469 6f6e  set cancellation
-00012910: 206d 6174 6368 2066 6f72 2007 0000 000d   match for .....
-00012920: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
-00012930: 0000 2404 2104 3404 3504 3b04 3e04 3a00  ..$.!.4.5.;.>.:.
-00012940: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
-00012950: 3d04 3e00 3a00 2008 0000 0000 0600 0000  =.>.:. .........
-00012960: 0f54 7261 6465 7320 6c6f 6164 6564 3a20  .Trades loaded: 
-00012970: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
-00012980: 4655 0103 0000 0040 0422 0432 043e 0439  FU.....@.".2.>.9
-00012990: 0020 0431 0440 043e 043a 0435 0440 0020  . .1.@.>.:.5.@. 
-000129a0: 0028 0065 0078 002e 0020 0431 0440 043e  .(.e.x... .1.@.>
-000129b0: 043a 0435 0440 0020 0423 0440 0430 043b  .:.5.@. .#.@.0.;
-000129c0: 0441 0438 0431 0029 0800 0000 0006 0000  .A.8.1.)........
-000129d0: 0020 5476 6f79 2042 726f 6b65 7220 2865  . Tvoy Broker (e
-000129e0: 782e 2055 7261 6c73 6962 2042 726f 6b65  x. Uralsib Broke
-000129f0: 7229 0700 0000 0d53 7461 7465 6d65 6e74  r).....Statement
-00012a00: 554b 4655 0103 0000 0032 041e 0442 0447  UKFU.....2...B.G
-00012a10: 0451 0442 0020 0422 0432 043e 0439 0020  .Q.B. .".2.>.9. 
-00012a20: 0431 0440 043e 043a 0435 0440 0020 0028  .1.@.>.:.5.@. .(
-00012a30: 002a 002e 007a 0069 0070 0029 0800 0000  .*...z.i.p.)....
-00012a40: 0006 0000 001d 5476 6f79 2042 726f 6b65  ......Tvoy Broke
-00012a50: 7220 7374 6174 656d 656e 7420 282a 2e7a  r statement (*.z
-00012a60: 6970 2907 0000 000d 5374 6174 656d 656e  ip).....Statemen
-00012a70: 7455 4b46 5501 0300 0000 3004 1d04 3504  tUKFU.....0...5.
-00012a80: 3804 3704 3204 3504 4104 4204 3d04 4b04  8.7.2.5.A.B.=.K.
-00012a90: 3900 2004 4204 3804 3f00 2004 4104 3404  9. .B.8.?. .A.4.
-00012aa0: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
-00012ab0: 0600 0000 1455 6e6b 6e6f 776e 2074 7261  .....Unknown tra
-00012ac0: 6465 2074 7970 653a 2007 0000 000d 5374  de type: .....St
-00012ad0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
-00012ae0: 3e04 1d04 3504 3f04 3e04 3404 3404 3504  >...5.?.>.4.4.5.
-00012af0: 4004 3604 3804 3204 3004 3504 3c04 3004  @.6.8.2.0.5.<.0.
-00012b00: 4f00 2004 3e04 3f04 3504 4004 3004 4604  O. .>.?.5.@.0.F.
-00012b10: 3804 4f00 2004 4100 2004 2604 1100 2008  8.O. .A. .&... .
-00012b20: 0000 0000 0600 0000 1d55 6e73 7570 7070  .........Unsuppp
-00012b30: 6f72 7465 6420 6173 7365 7420 6f70 6572  orted asset oper
-00012b40: 6174 696f 6e20 0700 0000 0d53 7461 7465  ation .....State
-00012b50: 6d65 6e74 554b 4655 0103 0000 004a 041d  mentUKFU.....J..
-00012b60: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
-00012b70: 0438 0432 0430 0435 043c 0430 044f 0020  .8.2.0.5.<.0.O. 
-00012b80: 0434 0435 043d 0435 0436 043d 0430 044f  .4.5.=.5.6.=.0.O
-00012b90: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
-00012ba0: 0446 0438 044f 0020 0800 0000 0006 0000  .F.8.O. ........
-00012bb0: 001e 556e 7375 7070 706f 7274 6564 2063  ..Unsuppported c
-00012bc0: 6173 6820 7472 616e 7361 6374 696f 6e20  ash transaction 
-00012bd0: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
-00012be0: 4655 0103 0000 003e 0410 0440 0445 0438  FU.....>...@.E.8
-00012bf0: 0432 0020 0441 043e 0434 0435 0440 0436  .2. .A.>.4.5.@.6
-00012c00: 0438 0442 0020 043d 0435 0441 043a 043e  .8.B. .=.5.A.:.>
-00012c10: 043b 044c 043a 043e 0020 0444 0430 0439  .;.L.:.>. .D.0.9
-00012c20: 043b 043e 0432 0800 0000 0006 0000 001f  .;.>.2..........
-00012c30: 4172 6368 6976 6520 636f 6e74 6169 6e73  Archive contains
-00012c40: 206d 756c 7469 706c 6520 6669 6c65 7307   multiple files.
-00012c50: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012c60: 0103 0000 005a 041d 0435 0020 0443 0434  .....Z...5. .C.4
-00012c70: 0430 043b 043e 0441 044c 0020 043d 0430  .0.;.>.A.L. .=.0
-00012c80: 0439 0442 0438 0020 043e 0436 0438 0434  .9.B.8. .>.6.8.4
-00012c90: 0430 0435 043c 044b 0439 0020 0437 0430  .0.5.<.K.9. .7.0
-00012ca0: 0433 043e 043b 043e 0432 043e 043a 0020  .3.>.;.>.2.>.:. 
-00012cb0: 043e 0442 0447 0451 0442 0430 003a 0020  .>.B.G.Q.B.0.:. 
-00012cc0: 0800 0000 0006 0000 0023 4361 6e27 7420  .........#Can't 
-00012cd0: 6669 6e64 2065 7870 6563 7465 6420 7265  find expected re
-00012ce0: 706f 7274 2068 6561 6465 723a 2007 0000  port header: ...
-00012cf0: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
-00012d00: 0000 0066 041d 0435 0020 0443 0434 0430  ...f...5. .C.4.0
-00012d10: 043b 043e 0441 044c 0020 043e 043f 0440  .;.>.A.L. .>.?.@
-00012d20: 0435 0434 0435 043b 0438 0442 044c 0020  .5.4.5.;.8.B.L. 
-00012d30: 0432 0430 043b 044e 0442 044b 0020 0438  .2.0.;.N.B.K. .8
-00012d40: 0437 0020 043e 0431 0449 0435 0439 0020  .7. .>.1.I.5.9. 
-00012d50: 0441 0435 043a 0446 0438 0438 0020 043e  .A.5.:.F.8.8. .>
-00012d60: 0442 0447 0451 0442 0430 0800 0000 0006  .B.G.Q.B.0......
-00012d70: 0000 0036 4361 6e27 7420 6765 7420 6375  ...6Can't get cu
-00012d80: 7272 656e 6369 6573 2066 726f 6d20 7375  rrencies from su
-00012d90: 6d6d 6172 7920 7365 6374 696f 6e20 6f66  mmary section of
-00012da0: 2073 7461 7465 6d65 6e74 0700 0000 0c53   statement.....S
-00012db0: 7461 7465 6d65 6e74 584c 5301 0300 0000  tatementXLS.....
-00012dc0: 4604 1d04 3504 3204 3e04 3704 3c04 3e04  F...5.2.>.7.<.>.
-00012dd0: 3604 3d04 3e00 2004 3e04 3f04 4004 3504  6.=.>. .>.?.@.5.
-00012de0: 3404 3504 3b04 3804 4204 4c00 2004 3f04  4.5.;.8.B.L. .?.
-00012df0: 3504 4004 3804 3e04 3400 2004 3e04 4204  5.@.8.>.4. .>.B.
-00012e00: 4704 5104 4204 3008 0000 0000 0600 0000  G.Q.B.0.........
-00012e10: 1843 616e 2774 2072 6561 6420 7265 706f  .Can't read repo
-00012e20: 7274 2070 6572 696f 6407 0000 000c 5374  rt period.....St
-00012e30: 6174 656d 656e 7458 4c53 0103 0000 001c  atementXLS......
-00012e40: 0414 0421 0020 0437 0430 0433 0440 0443  ...!. .7.0.3.@.C
-00012e50: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
-00012e60: 0006 0000 0016 4361 7368 2062 616c 616e  ......Cash balan
-00012e70: 6365 7320 6c6f 6164 6564 3a20 0700 0000  ces loaded: ....
-00012e80: 0c53 7461 7465 6d65 6e74 584c 5301 0300  .StatementXLS...
-00012e90: 0000 3604 2104 4204 3e04 3b04 3104 3504  ..6.!.B.>.;.1.5.
-00012ea0: 4600 2004 3d04 3500 2004 3d04 3004 3904  F. .=.5. .=.0.9.
-00012eb0: 3404 3504 3d00 2004 3200 2004 4104 3504  4.5.=. .2. .A.5.
-00012ec0: 3a04 4604 3804 3800 2008 0000 0000 0600  :.F.8.8. .......
-00012ed0: 0000 1c43 6f6c 756d 6e20 6e6f 7420 666f  ...Column not fo
-00012ee0: 756e 6420 696e 2073 6563 7469 6f6e 2007  und in section .
-00012ef0: 0000 000c 5374 6174 656d 656e 7458 4c53  ....StatementXLS
-00012f00: 0103 0000 0034 041d 0435 0441 043a 043e  .....4...5.A.:.>
-00012f10: 043b 044c 043a 043e 0020 0441 0447 0435  .;.L.:.>. .A.G.5
-00012f20: 0442 043e 0432 0020 043d 0430 0439 0434  .B.>.2. .=.0.9.4
-00012f30: 0435 043d 043e 003a 0020 0800 0000 0006  .5.=.>.:. ......
-00012f40: 0000 0019 4d75 6c74 6970 6c65 2061 6363  ....Multiple acc
-00012f50: 6f75 6e74 7320 666f 756e 643a 2007 0000  ounts found: ...
-00012f60: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
-00012f70: 0000 001c 0426 0411 0020 0437 0430 0433  .....&... .7.0.3
-00012f80: 0440 0443 0436 0435 043d 044b 003a 0020  .@.C.6.5.=.K.:. 
-00012f90: 0800 0000 0006 0000 0013 5365 6375 7269  ..........Securi
-00012fa0: 7469 6573 206c 6f61 6465 643a 2007 0000  ties loaded: ...
-00012fb0: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
-00012fc0: 0000 0030 041e 0442 0447 0451 0442 0020  ...0...B.G.Q.B. 
-00012fd0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
-00012fe0: 0020 0443 0441 043f 0435 0448 043d 043e  . .C.A.?.5.H.=.>
-00012ff0: 003a 0020 0800 0000 0006 0000 001f 5374  .:. ..........St
-00013000: 6174 656d 656e 7420 6c6f 6164 6564 2073  atement loaded s
-00013010: 7563 6365 7373 6675 6c6c 793a 2007 0000  uccessfully: ...
-00013020: 000c 5374 6174 656d 656e 7458 4c53 0103  ..StatementXLS..
-00013030: 0000 0022 0020 0437 0430 0433 0440 0443  ...". .7.0.3.@.C
-00013040: 0436 0435 043d 0020 0443 0441 043f 0435  .6.5.=. .C.A.?.5
-00013050: 0448 043d 043e 0800 0000 0006 0000 0014  .H.=.>..........
-00013060: 206c 6f61 6465 6420 7375 6363 6573 7366   loaded successf
-00013070: 756c 6c79 0700 0000 0c53 7461 7465 6d65  ully.....Stateme
-00013080: 6e74 584d 4c01 0300 0000 3604 1d04 3504  ntXML.....6...5.
-00013090: 3204 3504 4004 3d04 4b04 3900 2004 4404  2.5.@.=.K.9. .D.
-000130a0: 3e04 4004 3c04 3004 4200 2000 5800 4d00  >.@.<.0.B. .X.M.
-000130b0: 4c00 2004 4404 3004 3904 3b04 3000 3a00  L. .D.0.9.;.0.:.
-000130c0: 2008 0000 0000 0600 0000 1643 616e 2774   ..........Can't
-000130d0: 2070 6172 7365 2058 4d4c 2066 696c 653a   parse XML file:
-000130e0: 2007 0000 000c 5374 6174 656d 656e 7458   .....StatementX
-000130f0: 4d4c 0103 0000 0044 041d 0435 0432 043e  ML.....D...5.2.>
-00013100: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
-00013110: 0430 0433 0440 0443 0437 0438 0442 044c  .0.3.@.C.7.8.B.L
-00013120: 0020 043e 0442 0447 0451 0442 0020 043d  . .>.B.G.Q.B. .=
-00013130: 043e 043c 0435 0440 003a 0020 0800 0000  .>.<.5.@.:. ....
-00013140: 0006 0000 0020 4661 696c 6564 2074 6f20  ..... Failed to 
-00013150: 6669 6e64 2073 7461 7465 6d65 6e74 2069  find statement i
-00013160: 6e64 6578 3a20 0700 0000 0c53 7461 7465  ndex: .....State
-00013170: 6d65 6e74 584d 4c01 0300 0000 3e04 1d04  mentXML.....>...
-00013180: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
-00013190: 3e00 2004 3704 3004 3304 4004 4304 3704  >. .7.0.3.@.C.7.
-000131a0: 3804 4204 4c00 2004 3004 4204 4204 4004  8.B.L. .0.B.B.@.
-000131b0: 3804 3104 4304 4200 3a00 2008 0000 0000  8.1.C.B.:. .....
-000131c0: 0600 0000 1a46 6169 6c65 6420 746f 206c  .....Failed to l
-000131d0: 6f61 6420 6174 7472 6962 7574 653a 2007  oad attribute: .
-000131e0: 0000 000c 5374 6174 656d 656e 7458 4d4c  ....StatementXML
-000131f0: 0103 0000 0042 041e 0442 0447 0451 0442  .....B...B.G.Q.B
-00013200: 0020 0431 0440 043e 043a 0435 0440 0430  . .1.@.>.:.5.@.0
-00013210: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
-00013220: 0435 043d 0020 0432 0020 0444 0430 0439  .5.=. .2. .D.0.9
-00013230: 043b 0435 003a 0020 0800 0000 0006 0000  .;.5.:. ........
-00013240: 0020 4e6f 2073 7461 7465 6d65 6e74 2077  . No statement w
-00013250: 6173 2066 6f75 6e64 2069 6e20 6669 6c65  as found in file
-00013260: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
-00013270: 584d 4c01 0300 0000 3404 1d04 3504 3804  XML.....4...5.8.
-00013280: 3704 3204 3504 4104 4204 3d04 3004 4f00  7.2.5.A.B.=.0.O.
-00013290: 2004 3c04 3504 4204 3a04 3000 2004 3e04   .<.5.B.:.0. .>.
-000132a0: 4204 4704 5104 4204 3000 3a00 2008 0000  B.G.Q.B.0.:. ...
-000132b0: 0000 0600 0000 1755 6e6b 6e6f 776e 2073  .......Unknown s
-000132c0: 7461 7465 6d65 6e74 2074 6167 3a20 0700  tatement tag: ..
-000132d0: 0000 0c53 7461 7465 6d65 6e74 584d 4c01  ...StatementXML.
-000132e0: 0300 0000 4c04 1d04 3504 3f04 3e04 3404  ....L...5.?.>.4.
-000132f0: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
-00013300: 3c04 4b04 3900 2004 4404 3e04 4004 3c04  <.K.9. .D.>.@.<.
-00013310: 3004 4200 2004 3404 3004 4204 4b00 2f04  0.B. .4.0.B.K./.
-00013320: 3204 4004 3504 3c04 3504 3d04 3800 3a00  2.@.5.<.5.=.8.:.
-00013330: 2008 0000 0000 0600 0000 1e55 6e73 7570   ..........Unsup
-00013340: 706f 7274 6564 2064 6174 652f 7469 6d65  ported date/time
-00013350: 2066 6f72 6d61 743a 2007 0000 000c 5374   format: .....St
-00013360: 6174 656d 656e 7458 4d4c 0103 0000 0020  atementXML..... 
-00013370: 041e 0448 0438 0431 043a 0430 0020 0438  ...H.8.1.:.0. .8
-00013380: 043c 043f 043e 0440 0442 0430 003a 0020  .<.?.>.@.B.0.:. 
-00013390: 0800 0000 0006 0000 000f 496d 706f 7274  ..........Import
-000133a0: 2066 6169 6c65 643a 2007 0000 000a 5374   failed: .....St
-000133b0: 6174 656d 656e 7473 0103 0000 0040 0412  atements.....@..
-000133c0: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
-000133d0: 0444 0430 0439 043b 0020 043e 0442 0447  .D.0.9.;. .>.B.G
-000133e0: 0435 0442 0430 0020 0434 043b 044f 0020  .5.B.0. .4.;.O. 
-000133f0: 0438 043c 043f 043e 0440 0442 0430 0800  .8.<.?.>.@.B.0..
-00013400: 0000 0006 0000 001f 5365 6c65 6374 2073  ........Select s
-00013410: 7461 7465 6d65 6e74 2066 696c 6520 746f  tatement file to
-00013420: 2069 6d70 6f72 7407 0000 000a 5374 6174   import.....Stat
-00013430: 656d 656e 7473 0103 0000 004a 041a 043b  ements.....J...;
-00013440: 0430 0441 0441 0020 043e 0442 0447 0451  .0.A.A. .>.B.G.Q
-00013450: 0442 0430 0020 043d 0435 0020 043c 043e  .B.0. .=.5. .<.>
-00013460: 0436 0435 0442 0020 0431 044b 0442 044c  .6.5.B. .1.K.B.L
-00013470: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
-00013480: 043d 003a 0020 0800 0000 0006 0000 0021  .=.:. .........!
-00013490: 5374 6174 656d 656e 7420 636c 6173 7320  Statement class 
-000134a0: 6361 6e27 7420 6265 206c 6f61 6465 643a  can't be loaded:
-000134b0: 2007 0000 000a 5374 6174 656d 656e 7473   .....Statements
-000134c0: 0103 0000 0054 041c 043e 0434 0443 043b  .....T...>.4.C.;
-000134d0: 044c 0020 043e 0442 0447 0451 0442 0430  .L. .>.B.G.Q.B.0
-000134e0: 0020 043d 0435 0020 043c 043e 0436 0435  . .=.5. .<.>.6.5
-000134f0: 0442 0020 0431 044b 0442 044c 0020 0438  .B. .1.K.B.L. .8
-00013500: 043c 043f 043e 0440 0442 0438 0440 043e  .<.?.>.@.B.8.@.>
-00013510: 0432 0430 043d 003a 0020 0800 0000 0006  .2.0.=.:. ......
-00013520: 0000 0024 5374 6174 656d 656e 7420 6d6f  ...$Statement mo
-00013530: 6475 6c65 2063 616e 2774 2062 6520 696d  dule can't be im
-00013540: 706f 7274 6564 3a20 0700 0000 0a53 7461  ported: .....Sta
-00013550: 7465 6d65 6e74 7301 0300 0000 0804 1004  tements.........
-00013560: 3a04 4200 2e08 0000 0000 0600 0000 0441  :.B............A
-00013570: 6374 2e07 0000 0010 5379 6d62 6f6c 734c  ct......SymbolsL
-00013580: 6973 744d 6f64 656c 0103 0000 000c 0412  istModel........
-00013590: 0430 043b 044e 0442 0430 0800 0000 0006  .0.;.N.B.0......
-000135a0: 0000 0008 4375 7272 656e 6379 0700 0000  ....Currency....
-000135b0: 1053 796d 626f 6c73 4c69 7374 4d6f 6465  .SymbolsListMode
-000135c0: 6c01 0300 0000 1004 1e04 3f04 3804 4104  l.........?.8.A.
-000135d0: 3004 3d04 3804 3508 0000 0000 0600 0000  0.=.8.5.........
-000135e0: 0b44 6573 6372 6970 7469 6f6e 0700 0000  .Description....
-000135f0: 1053 796d 626f 6c73 4c69 7374 4d6f 6465  .SymbolsListMode
-00013600: 6c01 0300 0000 1204 1a04 3e04 4204 3804  l.........>.B.8.
-00013610: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
-00013620: 0000 0651 756f 7465 7307 0000 0010 5379  ...Quotes.....Sy
-00013630: 6d62 6f6c 734c 6973 744d 6f64 656c 0103  mbolsListModel..
-00013640: 0000 000c 0421 0438 043c 0432 043e 043b  .....!.8.<.2.>.;
-00013650: 0800 0000 0006 0000 0006 5379 6d62 6f6c  ..........Symbol
-00013660: 0700 0000 1053 796d 626f 6c73 4c69 7374  .....SymbolsList
-00013670: 4d6f 6465 6c01 0300 0000 0604 2204 4d04  Model.......".M.
-00013680: 3308 0000 0000 0600 0000 0354 6167 0700  3..........Tag..
-00013690: 0000 0c54 6167 4c69 7374 4d6f 6465 6c01  ...TagListModel.
-000136a0: 0300 0000 1004 1e04 3f04 3504 4004 3004  ........?.5.@.0.
-000136b0: 4604 3804 3808 0000 0000 0600 0000 0a4f  F.8.8..........O
-000136c0: 7065 7261 7469 6f6e 7307 0000 0009 5461  perations.....Ta
-000136d0: 6752 6570 6f72 7401 0300 0000 1004 3f04  gReport.......?.
-000136e0: 3e00 2004 1c04 3504 4204 3a04 3508 0000  >. ...5.B.:.5...
-000136f0: 0000 0600 0000 0662 7920 5461 6707 0000  .......by Tag...
-00013700: 0009 5461 6752 6570 6f72 7401 0300 0000  ..TagReport.....
-00013710: 1c04 1e04 4204 4704 3504 4200 2004 3f04  ....B.G.5.B. .?.
-00013720: 3e00 2004 3c04 3504 4204 3a04 3508 0000  >. .<.5.B.:.5...
-00013730: 0000 0600 0000 0d52 6570 6f72 7420 6279  .......Report by
-00013740: 2074 6167 0700 0000 0f54 6167 5265 706f   tag.....TagRepo
-00013750: 7274 5769 6467 6574 0103 0000 000c 041c  rtWidget........
-00013760: 0435 0442 043a 0430 003a 0800 0000 0006  .5.B.:.0.:......
-00013770: 0000 0004 5461 673a 0700 0000 0f54 6167  ....Tag:.....Tag
-00013780: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
-00013790: 0024 0027 0020 0437 0430 043c 0435 043d  .$.'. .7.0.<.5.=
-000137a0: 0435 043d 0430 0020 0443 0441 043f 0435  .5.=.0. .C.A.?.5
-000137b0: 0448 043d 043e 0800 0000 0006 0000 001b  .H.=.>..........
-000137c0: 2720 7761 7320 7375 6363 6573 7366 756c  ' was successful
-000137d0: 6c79 2072 6570 6c61 6365 6407 0000 000e  ly replaced.....
-000137e0: 5461 6773 4c69 7374 4469 616c 6f67 0103  TagsListDialog..
-000137f0: 0000 000c 0027 0020 043d 0430 003a 0020  .....'. .=.0.:. 
-00013800: 0800 0000 0006 0000 0008 2720 7769 7468  ..........' with
-00013810: 3a20 0700 0000 0e54 6167 734c 6973 7444  : .....TagsListD
-00013820: 6961 6c6f 6701 0300 0000 2004 1704 3004  ialog..... ...0.
-00013830: 3c04 3504 3d04 3804 4204 4c00 2004 3c04  <.5.=.8.B.L. .<.
-00013840: 3504 4204 3a04 4300 2000 2708 0000 0000  5.B.:.C. .'.....
-00013850: 0600 0000 0d52 6570 6c61 6365 2074 6167  .....Replace tag
-00013860: 2027 0700 0000 0e54 6167 734c 6973 7444   '.....TagsListD
-00013870: 6961 6c6f 6701 0300 0000 1c04 1704 3004  ialog.........0.
-00013880: 3c04 3504 3d04 3804 4204 4c00 2004 3d04  <.5.=.8.B.L. .=.
-00013890: 3000 2e00 2e00 2e08 0000 0000 0600 0000  0...............
-000138a0: 0f52 6570 6c61 6365 2077 6974 682e 2e2e  .Replace with...
-000138b0: 0700 0000 0e54 6167 734c 6973 7444 6961  .....TagsListDia
-000138c0: 6c6f 6701 0300 0000 3404 1f04 3e04 3a04  log.....4...>.:.
-000138d0: 3004 3704 3004 4204 4c00 2004 3e04 3f04  0.7.0.B.L. .>.?.
-000138e0: 3504 4004 3004 4604 3804 3800 2004 4100  5.@.0.F.8.8. .A.
-000138f0: 2004 1c04 3504 4204 3a04 3e04 3908 0000   ...5.B.:.>.9...
-00013900: 0000 0600 0000 1853 686f 7720 6f70 6572  .......Show oper
-00013910: 6174 696f 6e73 2077 6974 6820 5461 6707  ations with Tag.
-00013920: 0000 000e 5461 6773 4c69 7374 4469 616c  ....TagsListDial
-00013930: 6f67 0103 0000 000e 041c 0435 0442 043a  og.........5.B.:
-00013940: 0430 0020 0027 0800 0000 0006 0000 0005  .0. .'..........
-00013950: 5461 6720 2707 0000 000e 5461 6773 4c69  Tag '.....TagsLi
-00013960: 7374 4469 616c 6f67 0103 0000 0008 0422  stDialog......."
-00013970: 044d 0433 0438 0800 0000 0006 0000 0004  .M.3.8..........
-00013980: 5461 6773 0700 0000 0e54 6167 734c 6973  Tags.....TagsLis
-00013990: 7444 6961 6c6f 6701 0300 0000 1a04 2204  tDialog.......".
-000139a0: 3504 3a04 4304 4904 3804 3900 2004 3a04  5.:.C.I.8.9. .:.
-000139b0: 4304 4004 4100 3a08 0000 0000 0600 0000  C.@.A.:.........
-000139c0: 0d43 7572 7265 6e74 2072 6174 653a 0700  .Current rate:..
-000139d0: 0000 1354 6178 4573 7469 6d61 7469 6f6e  ...TaxEstimation
-000139e0: 4469 616c 6f67 0103 0000 0028 041f 043e  Dialog.....(...>
-000139f0: 0441 043b 0435 0434 043d 044f 044f 0020  .A.;.5.4.=.O.O. 
-00013a00: 043a 043e 0442 0438 0440 043e 0432 043a  .:.>.B.8.@.>.2.:
-00013a10: 0430 003a 0800 0000 0006 0000 000b 4c61  .0.:..........La
-00013a20: 7374 2071 756f 7465 3a07 0000 0013 5461  st quote:.....Ta
-00013a30: 7845 7374 696d 6174 696f 6e44 6961 6c6f  xEstimationDialo
-00013a40: 6701 0300 0000 1a04 1e04 4604 3504 3d04  g.........F.5.=.
-00013a50: 3a04 3000 2004 3d04 3004 3b04 3e04 3304  :.0. .=.0.;.>.3.
-00013a60: 3008 0000 0000 0600 0000 0e54 6178 2045  0..........Tax E
-00013a70: 7374 696d 6174 696f 6e07 0000 0013 5461  stimation.....Ta
-00013a80: 7845 7374 696d 6174 696f 6e44 6961 6c6f  xEstimationDialo
-00013a90: 6701 0300 0000 0800 5800 2e00 5800 5808  g.......X...X.X.
-00013aa0: 0000 0000 0600 0000 0458 2e58 5807 0000  .........X.XX...
-00013ab0: 0013 5461 7845 7374 696d 6174 696f 6e44  ..TaxEstimationD
-00013ac0: 6961 6c6f 6701 0300 0000 0a04 1804 2204  ialog.........".
-00013ad0: 1e04 1304 1e08 0000 0000 0600 0000 0554  ...............T
-00013ae0: 4f54 414c 0700 0000 0c54 6178 4573 7469  OTAL.....TaxEsti
-00013af0: 6d61 746f 7201 0300 0000 2404 1e04 4604  mator.....$...F.
-00013b00: 3504 3d04 3a04 3000 2004 3d04 3004 3b04  5.=.:.0. .=.0.;.
-00013b10: 3e04 3304 3000 2004 3404 3b04 4f00 2008  >.3.0. .4.;.O. .
-00013b20: 0000 0000 0600 0000 1354 6178 2065 7374  .........Tax est
-00013b30: 696d 6174 696f 6e20 666f 7220 0700 0000  imation for ....
-00013b40: 0c54 6178 4573 7469 6d61 746f 7201 0300  .TaxEstimator...
-00013b50: 0000 3c04 2104 4204 3004 3204 3a04 3000  ..<.!.B.0.2.:.0.
-00013b60: 2004 3d04 3004 3b04 3e04 3304 3000 2004   .=.0.;.>.3.0. .
-00013b70: 3d04 3500 2004 3d04 3004 3904 3404 3504  =.5. .=.0.9.4.5.
-00013b80: 3d04 3000 2004 3404 3b04 4f00 3a00 2008  =.0. .4.;.O.:. .
-00013b90: 0000 0000 0600 0000 1854 6178 2072 6174  .........Tax rat
-00013ba0: 6520 6e6f 7420 666f 756e 6420 666f 723a  e not found for:
-00013bb0: 2007 0000 000c 5461 7845 7374 696d 6174   .....TaxEstimat
-00013bc0: 6f72 0103 0000 0008 0414 0430 0442 0430  or.........0.B.0
-00013bd0: 0800 0000 0006 0000 0004 4461 7465 0700  ..........Date..
-00013be0: 0000 1154 6178 4573 7469 6d61 746f 724d  ...TaxEstimatorM
-00013bf0: 6f64 656c 0103 0000 0014 0426 0435 043d  odel.......&.5.=
-00013c00: 0430 0020 043e 0442 043a 0440 002e 0800  .0. .>.B.:.@....
-00013c10: 0000 0006 0000 0004 4f70 656e 0700 0000  ........Open....
-00013c20: 1154 6178 4573 7469 6d61 746f 724d 6f64  .TaxEstimatorMod
-00013c30: 656c 0103 0000 0012 041f 0440 0438 0431  el.........@.8.1
-00013c40: 044b 043b 044c 002c 0020 0800 0000 0006  .K.;.L.,. ......
-00013c50: 0000 0008 5072 6f66 6974 2c20 0700 0000  ....Profit, ....
-00013c60: 1154 6178 4573 7469 6d61 746f 724d 6f64  .TaxEstimatorMod
-00013c70: 656c 0103 0000 000c 041a 043e 043b 002d  el.........>.;.-
-00013c80: 0432 043e 0800 0000 0006 0000 0003 5174  .2.>..........Qt
-00013c90: 7907 0000 0011 5461 7845 7374 696d 6174  y.....TaxEstimat
-00013ca0: 6f72 4d6f 6465 6c01 0300 0000 0c04 1a04  orModel.........
-00013cb0: 4304 4004 4100 2c00 2008 0000 0000 0600  C.@.A.,. .......
-00013cc0: 0000 0652 6174 652c 2007 0000 0011 5461  ...Rate, .....Ta
-00013cd0: 7845 7374 696d 6174 6f72 4d6f 6465 6c01  xEstimatorModel.
-00013ce0: 0300 0000 0e04 1d04 3004 3b04 3e04 3300  ........0.;.>.3.
-00013cf0: 2c00 2008 0000 0000 0600 0000 0554 6178  ,. ..........Tax
-00013d00: 2c20 0700 0000 1154 6178 4573 7469 6d61  , .....TaxEstima
-00013d10: 746f 724d 6f64 656c 0103 0000 0074 041d  torModel.....t..
-00013d20: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
-00013d30: 043e 0020 0437 0430 0433 0440 0443 0437  .>. .7.0.3.@.C.7
-00013d40: 0438 0442 044c 0020 043f 0430 0440 0430  .8.B.L. .?.0.@.0
-00013d50: 043c 0435 0442 0440 044b 0020 043d 0430  .<.5.B.@.K. .=.0
-00013d60: 043b 043e 0433 043e 0432 043e 0433 043e  .;.>.3.>.2.>.3.>
-00013d70: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
-00013d80: 0438 0437 0020 0444 0430 0439 043b 0430  .8.7. .D.0.9.;.0
-00013d90: 0020 0800 0000 0006 0000 002b 4361 6e27  . .........+Can'
-00013da0: 7420 6c6f 6164 2074 6178 2072 6570 6f72  t load tax repor
-00013db0: 7420 7061 7261 6d65 7465 7273 2066 726f  t parameters fro
-00013dc0: 6d20 6669 6c65 2007 0000 0009 5461 7852  m file .....TaxR
-00013dd0: 6570 6f72 7401 0300 0000 2804 1d04 3504  eport.....(...5.
-00013de0: 3804 3704 3204 3504 4104 4204 3d04 3004  8.7.2.5.A.B.=.0.
-00013df0: 4f00 2004 3204 3004 3b04 4e04 4204 3000  O. .2.0.;.N.B.0.
-00013e00: 3a00 2008 0000 0000 0600 0000 1943 7572  :. ..........Cur
-00013e10: 7265 6e63 7920 6973 206e 6f74 2064 6566  rency is not def
-00013e20: 696e 6564 3a20 0700 0000 0954 6178 5265  ined: .....TaxRe
-00013e30: 706f 7274 0103 0000 004a 041d 0435 0020  port.....J...5. 
-00013e40: 0443 043a 0430 0437 0430 043d 0020 0448  .C.:.0.7.0.=. .H
-00013e50: 0430 0431 043b 043e 043d 0020 043e 0442  .0.1.;.>.=. .>.B
-00013e60: 0447 0435 0442 0430 0020 0434 043b 044f  .G.5.B.0. .4.;.O
-00013e70: 0020 0440 0430 0437 0434 0435 043b 0430  . .@.0.7.4.5.;.0
-00013e80: 003a 0020 0800 0000 0006 0000 0026 4e6f  .:. .........&No
-00013e90: 2072 6570 6f72 7420 7465 6d70 6c61 7465   report template
-00013ea0: 2066 6f75 6e64 2066 6f72 2073 6563 7469   found for secti
-00013eb0: 6f6e 3a20 0700 0000 0954 6178 5265 706f  on: .....TaxRepo
-00013ec0: 7274 0103 0000 006a 041d 0435 0442 0020  rt.....j...5.B. 
-00013ed0: 0438 043d 0444 043e 0440 043c 0430 0446  .8.=.D.>.@.<.0.F
-00013ee0: 0438 0438 0020 043e 0020 0421 043e 0418  .8.8. .>. .!.>..
-00013ef0: 0414 041d 0020 0432 0020 043f 0430 0440  ..... .2. .?.0.@
-00013f00: 0430 043c 0435 0442 0440 0430 0445 0020  .0.<.5.B.@.0.E. 
-00013f10: 043d 0430 043b 043e 0433 043e 0432 043e  .=.0.;.>.3.>.2.>
-00013f20: 0433 043e 0020 043e 0442 0447 0451 0442  .3.>. .>.B.G.Q.B
-00013f30: 0430 0800 0000 0006 0000 0042 5468 6572  .0.........BTher
-00013f40: 6520 6172 6520 6e6f 2069 6e66 6f72 6d61  e are no informa
-00013f50: 7469 6f6e 2061 626f 7574 2074 6178 2074  tion about tax t
-00013f60: 7265 6174 7920 696e 2074 6178 2072 6570  reaty in tax rep
-00013f70: 6f72 7420 7061 7261 6d65 7465 7273 0700  ort parameters..
-00013f80: 0000 0954 6178 5265 706f 7274 0103 0000  ...TaxReport....
-00013f90: 0060 041d 0435 0020 0437 0430 0434 0430  .`...5. .7.0.4.0
-00013fa0: 043d 044b 0020 043f 0430 0440 0430 043c  .=.K. .?.0.@.0.<
-00013fb0: 0435 0442 0440 044b 0020 043d 0430 043b  .5.B.@.K. .=.0.;
-00013fc0: 043e 0433 043e 0432 043e 0433 043e 0020  .>.3.>.2.>.3.>. 
-00013fd0: 043e 0442 0447 0451 0442 0430 0020 0434  .>.B.G.Q.B.0. .4
-00013fe0: 043b 044f 0020 0433 043e 0434 0430 003a  .;.O. .3.>.4.0.:
-00013ff0: 0020 0800 0000 0006 0000 0033 5468 6572  . .........3Ther
-00014000: 6520 6172 6520 6e6f 2070 6172 616d 6574  e are no paramet
-00014010: 6572 7320 666f 756e 6420 666f 7220 7461  ers found for ta
-00014020: 7820 7265 706f 7274 2079 6561 723a 2007  x report year: .
-00014030: 0000 0009 5461 7852 6570 6f72 7401 0300  ....TaxReport...
-00014040: 0000 0a00 2000 2e00 2e00 2e00 2008 0000  .... ....... ...
-00014050: 0000 0600 0000 0520 2e2e 2e20 0700 0000  ....... ... ....
-00014060: 0954 6178 5769 6467 6574 0103 0000 0006  .TaxWidget......
-00014070: 002e 002e 002e 0800 0000 0006 0000 0003  ................
-00014080: 2e2e 2e07 0000 0009 5461 7857 6964 6765  ........TaxWidge
-00014090: 7401 0300 0000 0a04 2104 4704 3504 4200  t.......!.G.5.B.
-000140a0: 3a08 0000 0000 0600 0000 0841 6363 6f75  :..........Accou
-000140b0: 6e74 3a07 0000 0009 5461 7857 6964 6765  nt:.....TaxWidge
-000140c0: 7401 0300 0000 9004 1d04 3804 3604 3500  t.........8.6.5.
-000140d0: 2004 4004 3004 4104 3f04 3e04 3b04 3e04   .@.0.A.?.>.;.>.
-000140e0: 3604 3504 3d04 4b00 2004 4d04 3a04 4104  6.5.=.K. .M.:.A.
-000140f0: 3f04 3504 4004 3804 3c04 3504 3d04 4204  ?.5.@.8.<.5.=.B.
-00014100: 3004 3b04 4c04 3d04 4b04 3500 2004 4404  0.;.L.=.K.5. .D.
-00014110: 4304 3d04 3a04 4604 3804 3800 2000 2d00  C.=.:.F.8.8. .-.
-00014120: 2004 3804 4104 3f04 3e04 3b04 4c04 3704   .8.A.?.>.;.L.7.
-00014130: 4304 3904 4204 3500 2004 4100 2004 3e04  C.9.B.5. .A. .>.
-00014140: 4104 4204 3e04 4004 3e04 3604 3d04 3e04  A.B.>.@.>.6.=.>.
-00014150: 4104 4204 4c04 4e08 0000 0000 0600 0000  A.B.L.N.........
-00014160: 3342 656c 6f77 2066 756e 6374 696f 6e73  3Below functions
-00014170: 2061 7265 2065 7870 6572 696d 656e 7461   are experimenta
-00014180: 6c20 2d20 7573 6520 6974 2077 6974 6820  l - use it with 
-00014190: 6361 7265 0700 0000 0954 6178 5769 6467  care.....TaxWidg
-000141a0: 6574 0103 0000 0044 041d 0435 0432 043e  et.....D...5.2.>
-000141b0: 0437 043c 043e 0436 043d 043e 0020 0437  .7.<.>.6.=.>. .7
-000141c0: 0430 043f 0438 0441 0430 0442 044c 0020  .0.?.8.A.0.B.L. 
-000141d0: 0033 002d 041d 0414 0424 041b 0020 0432  .3.-.....$... .2
-000141e0: 0020 0444 0430 0439 043b 0020 0800 0000  . .D.0.9.;. ....
-000141f0: 0006 0000 001f 4361 6e27 7420 7772 6974  ......Can't writ
-00014200: 6520 7461 7820 666f 726d 2069 6e74 6f20  e tax form into 
-00014210: 6669 6c65 2007 0000 0009 5461 7857 6964  file .....TaxWid
-00014220: 6765 7401 0300 0000 0e04 2104 4204 4004  get.......!.B.@.
-00014230: 3004 3d04 3000 3a08 0000 0000 0600 0000  0.=.0.:.........
-00014240: 0843 6f75 6e74 7279 3a07 0000 0009 5461  .Country:.....Ta
-00014250: 7857 6964 6765 7401 0300 0000 7804 2104  xWidget.....x.!.
-00014260: 3e04 3704 3404 3004 4204 4c00 2004 4404  >.7.4.0.B.L. .D.
-00014270: 3004 3904 3b00 2000 3300 2d04 1d04 2404  0.9.;. .3.-...$.
-00014280: 1404 1b00 2004 3200 2004 4404 3e04 4004  .... .2. .D.>.@.
-00014290: 3c04 3004 4204 3500 2004 3f04 4004 3e04  <.0.B.5. .?.@.>.
-000142a0: 3304 4004 3004 3c04 3c04 4b00 2000 2204  3.@.0.<.<.K. .".
-000142b0: 1404 3504 3a04 3b04 3004 4004 3004 4604  ..5.:.;.0.@.0.F.
-000142c0: 3804 4f00 2200 2000 2800 2a00 2e00 6400  8.O.". .(.*...d.
-000142d0: 6300 5800 2908 0000 0000 0600 0000 4043  c.X.).........@C
-000142e0: 7265 6174 6520 7461 7820 666f 726d 2069  reate tax form i
-000142f0: 6e20 22d0 94d0 b5d0 bad0 bbd0 b0d1 80d0  n ".............
-00014300: b0d1 86d0 b8d1 8f22 2070 726f 6772 616d  ......." program
-00014310: 2066 6f72 6d61 7420 282a 2e64 6358 2907   format (*.dcX).
-00014320: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
-00014330: 0000 1e04 1404 3004 3d04 3d04 4b04 3500  ......0.=.=.K.5.
-00014340: 2004 3d04 3504 3f04 3e04 3b04 3d04 4b04   .=.5.?.>.;.=.K.
-00014350: 3508 0000 0000 0600 0000 1344 6174 6120  5..........Data 
-00014360: 6172 6520 696e 636f 6d70 6c65 7465 0700  are incomplete..
-00014370: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-00014380: 005c 041d 0435 0020 0438 0441 043f 043e  .\...5. .8.A.?.>
-00014390: 043b 044c 0437 043e 0432 0430 0442 044c  .;.L.7.>.2.0.B.L
-000143a0: 0020 0434 0430 0442 0443 0020 043f 043e  . .4.0.B.C. .?.>
-000143b0: 0441 0442 0430 0432 043a 0438 0020 0434  .A.B.0.2.:.8. .4
-000143c0: 043b 044f 0020 043a 0443 0440 0441 043e  .;.O. .:.C.@.A.>
-000143d0: 0432 0020 0432 0430 043b 044e 0442 0800  .2. .2.0.;.N.B..
-000143e0: 0000 0006 0000 002d 446f 206e 6f74 2075  .......-Do not u
-000143f0: 7365 2073 6574 746c 656d 656e 7420 6461  se settlement da
-00014400: 7465 2066 6f72 2063 7572 7265 6e63 7920  te for currency 
-00014410: 7261 7465 7307 0000 0009 5461 7857 6964  rates.....TaxWid
-00014420: 6765 7401 0300 0000 1604 2404 3004 3904  get.......$.0.9.
-00014430: 3b00 2000 4500 7800 6300 6500 6c00 3a08  ;. .E.x.c.e.l.:.
-00014440: 0000 0000 0600 0000 0b45 7863 656c 2066  .........Excel f
-00014450: 696c 653a 0700 0000 0954 6178 5769 6467  ile:.....TaxWidg
-00014460: 6574 0103 0000 0028 0424 0430 0439 043b  et.....(.$.0.9.;
-00014470: 044b 0020 0045 0078 0063 0065 006c 0020  .K. .E.x.c.e.l. 
-00014480: 0028 002a 002e 0078 0073 006c 0078 0029  .(.*...x.s.l.x.)
-00014490: 0800 0000 0006 0000 0014 4578 6365 6c20  ..........Excel 
-000144a0: 6669 6c65 7320 282a 2e78 6c73 7829 0700  files (*.xlsx)..
-000144b0: 0000 0954 6178 5769 6467 6574 0103 0000  ...TaxWidget....
-000144c0: 004a 0424 0430 0439 043b 0020 0434 043b  .J.$.0.9.;. .4.;
-000144d0: 044f 0020 0441 043e 0445 0440 0430 043d  .O. .A.>.E.@.0.=
-000144e0: 0435 043d 0438 044f 0020 0434 0435 043a  .5.=.8.O. .4.5.:
-000144f0: 043b 0430 0440 0430 0446 0438 0438 0020  .;.0.@.0.F.8.8. 
-00014500: 0033 002d 041d 0414 0424 041b 0800 0000  .3.-.....$......
-00014510: 0006 0000 0024 4669 6c65 2077 6865 7265  .....$File where
-00014520: 2074 6f20 7374 6f72 6520 7275 7373 6961   to store russia
-00014530: 6e20 7461 7820 666f 726d 0700 0000 0954  n tax form.....T
-00014540: 6178 5769 6467 6574 0103 0000 0056 0424  axWidget.....V.$
-00014550: 0430 0439 043b 0020 0434 043b 044f 0020  .0.9.;. .4.;.O. 
-00014560: 0441 043e 0445 0440 0430 043d 0435 043d  .A.>.E.@.0.=.5.=
-00014570: 0438 044f 0020 0440 0430 0441 0447 0451  .8.O. .@.0.A.G.Q
-00014580: 0442 0430 0020 0432 0020 0444 043e 0440  .B.0. .2. .D.>.@
-00014590: 043c 0430 0442 0435 0020 0045 0078 0063  .<.0.B.5. .E.x.c
-000145a0: 0065 006c 0800 0000 0006 0000 002e 4669  .e.l..........Fi
-000145b0: 6c65 2077 6865 7265 2074 6f20 7374 6f72  le where to stor
-000145c0: 6520 7461 7820 7265 706f 7274 2069 6e20  e tax report in 
-000145d0: 4578 6365 6c20 666f 726d 6174 0700 0000  Excel format....
-000145e0: 0954 6178 5769 6467 6574 0103 0000 0068  .TaxWidget.....h
-000145f0: 0417 0430 0440 0443 0431 0435 0436 043d  ...0.@.C.1.5.6.=
-00014600: 044b 0439 0020 0441 0447 0451 0442 0020  .K.9. .A.G.Q.B. 
-00014610: 0434 043b 044f 0020 043a 043e 0442 043e  .4.;.O. .:.>.B.>
-00014620: 0440 043e 0433 043e 0020 043d 0443 0436  .@.>.3.>. .=.C.6
-00014630: 043d 043e 0020 043f 043e 0434 0433 043e  .=.>. .?.>.4.3.>
-00014640: 0442 043e 0432 0438 0442 044c 0020 043e  .B.>.2.8.B.L. .>
-00014650: 0442 0447 0451 0442 0800 0000 0006 0000  .B.G.Q.B........
-00014660: 0029 466f 7265 6967 6e20 6163 636f 756e  .)Foreign accoun
-00014670: 7420 746f 2070 7265 7061 7265 2074 6178  t to prepare tax
-00014680: 2072 6570 6f72 7420 666f 7207 0000 0009   report for.....
-00014690: 5461 7857 6964 6765 7401 0300 0000 2604  TaxWidget.....&.
-000146a0: 2404 3004 3904 3b00 2004 4100 2004 4004  $.0.9.;. .A. .@.
-000146b0: 3504 3704 4304 3b04 4c04 4204 3004 4204  5.7.C.;.L.B.0.B.
-000146c0: 3e04 3c00 3a08 0000 0000 0600 0000 0c4f  >.<.:..........O
-000146d0: 7574 7075 7420 6669 6c65 3a07 0000 0009  utput file:.....
-000146e0: 5461 7857 6964 6765 7401 0300 0000 1e04  TaxWidget.......
-000146f0: 2104 3e04 4504 4004 3004 3d04 3804 4204  !.>.E.@.0.=.8.B.
-00014700: 4c00 2004 1e04 4204 4704 5104 4208 0000  L. ...B.G.Q.B...
-00014710: 0000 0600 0000 0b53 6176 6520 5265 706f  .......Save Repo
-00014720: 7274 0700 0000 0954 6178 5769 6467 6574  rt.....TaxWidget
-00014730: 0103 0000 0026 0421 043e 0445 0440 0430  .....&.!.>.E.@.0
-00014740: 043d 0438 0442 044c 0020 0033 002d 041d  .=.8.B.L. .3.-..
-00014750: 0414 0424 041b 0020 0432 003a 0800 0000  ...$... .2.:....
-00014760: 0006 0000 0011 5361 7665 2074 6178 2066  ......Save tax f
-00014770: 6f72 6d20 746f 3a07 0000 0009 5461 7857  orm to:.....TaxW
-00014780: 6964 6765 7401 0300 0000 3804 2104 3e04  idget.....8.!.>.
-00014790: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
-000147a0: 3d04 3004 3b04 3e04 3304 3e04 3204 4b04  =.0.;.>.3.>.2.K.
-000147b0: 3900 2004 3e04 4204 4704 5104 4200 2004  9. .>.B.G.Q.B. .
-000147c0: 3200 3a08 0000 0000 0600 0000 1453 6176  2.:..........Sav
-000147d0: 6520 7461 7820 7265 706f 7274 7320 746f  e tax reports to
-000147e0: 3a07 0000 0009 5461 7857 6964 6765 7401  :.....TaxWidget.
-000147f0: 0300 0000 1804 1204 4b04 3104 3504 4004  ........K.1.5.@.
-00014800: 3804 4200 2004 4404 3004 3904 3b08 0000  8.B. .D.0.9.;...
-00014810: 0000 0600 0000 0b53 656c 6563 7420 6669  .......Select fi
-00014820: 6c65 0700 0000 0954 6178 5769 6467 6574  le.....TaxWidget
-00014830: 0103 0000 0028 041d 0430 043b 043e 0433  .....(...0.;.>.3
-00014840: 043e 0432 044b 0439 0020 043e 0442 0447  .>.2.K.9. .>.B.G
-00014850: 0451 0442 0020 043f 0443 0441 0442 0800  .Q.B. .?.C.A.B..
-00014860: 0000 0006 0000 0013 5461 7820 7265 706f  ........Tax repo
-00014870: 7274 2069 7320 656d 7074 7907 0000 0009  rt is empty.....
-00014880: 5461 7857 6964 6765 7401 0300 0000 4004  TaxWidget.....@.
-00014890: 1d04 3004 3b04 3e04 3304 3e04 3204 4b04  ..0.;.>.3.>.2.K.
-000148a0: 3900 2004 3e04 4204 4704 5104 4200 2004  9. .>.B.G.Q.B. .
-000148b0: 4104 3e04 4504 4004 3004 3d04 5104 3d00  A.>.E.@.0.=.Q.=.
-000148c0: 2004 3200 2004 4404 3004 3904 3b00 2008   .2. .D.0.9.;. .
-000148d0: 0000 0000 0600 0000 1954 6178 2072 6570  .........Tax rep
-000148e0: 6f72 7420 7361 7665 6420 746f 2066 696c  ort saved to fil
-000148f0: 6520 0700 0000 0954 6178 5769 6467 6574  e .....TaxWidget
-00014900: 0103 0000 0040 041d 0430 043b 043e 0433  .....@...0.;.>.3
-00014910: 043e 0432 044b 0439 0020 043e 0442 0447  .>.2.K.9. .>.B.G
-00014920: 0451 0442 0020 0441 043e 0445 0440 0430  .Q.B. .A.>.E.@.0
-00014930: 043d 0451 043d 0020 0432 0020 0444 0430  .=.Q.=. .2. .D.0
-00014940: 0439 043b 0020 0800 0000 0006 0000 001d  .9.;. ..........
-00014950: 5461 7820 7265 706f 7274 2077 6173 2073  Tax report was s
-00014960: 6176 6564 2074 6f20 6669 6c65 2007 0000  aved to file ...
-00014970: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
-00014980: 0c04 1d04 3004 3b04 3e04 3304 3808 0000  ....0.;.>.3.8...
-00014990: 0000 0600 0000 0554 6178 6573 0700 0000  .......Taxes....
-000149a0: 0954 6178 5769 6467 6574 0103 0000 004e  .TaxWidget.....N
-000149b0: 041e 0431 043d 043e 0432 0438 0442 044c  ...1.=.>.2.8.B.L
-000149c0: 0020 0442 043e 043b 044c 043a 043e 0020  . .B.>.;.L.:.>. 
-000149d0: 0438 043d 0444 043e 0440 043c 0430 0446  .8.=.D.>.@.<.0.F
-000149e0: 0438 044e 0020 043e 0020 0434 0438 0432  .8.N. .>. .4.8.2
-000149f0: 0438 0434 0435 043d 0434 0430 0445 0800  .8.4.5.=.4.0.E..
-00014a00: 0000 0006 0000 0027 5570 6461 7465 206f  .......'Update o
-00014a10: 6e6c 7920 696e 666f 726d 6174 696f 6e20  nly information 
-00014a20: 6162 6f75 7420 6469 7669 6465 6e64 7307  about dividends.
-00014a30: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
-00014a40: 0000 6404 1804 4104 3f04 3e04 3b04 4c04  ..d...A.?.>.;.L.
-00014a50: 3704 3e04 3204 3004 4204 4c00 2004 3d04  7.>.2.0.B.L. .=.
-00014a60: 3004 3704 3204 3004 3d04 3804 3500 2004  0.7.2.0.=.8.5. .
-00014a70: 3104 4004 3e04 3a04 3504 4004 3000 2004  1.@.>.:.5.@.0. .
-00014a80: 3a04 3004 3a00 2004 3804 4104 4204 3e04  :.0.:. .8.A.B.>.
-00014a90: 4704 3d04 3804 3a00 2004 3204 4b04 3f04  G.=.8.:. .2.K.?.
-00014aa0: 3b04 3004 4204 4b08 0000 0000 0600 0000  ;.0.B.K.........
-00014ab0: 2055 7365 2062 726f 6b65 7220 6e61 6d65   Use broker name
-00014ac0: 2061 7320 696e 636f 6d65 2073 6f75 7263   as income sourc
-00014ad0: 6507 0000 0009 5461 7857 6964 6765 7401  e.....TaxWidget.
-00014ae0: 0300 0000 0804 1304 3e04 3400 3a08 0000  ........>.4.:...
-00014af0: 0000 0600 0000 0559 6561 723a 0700 0000  .......Year:....
-00014b00: 0954 6178 5769 6467 6574 0103 0000 0050  .TaxWidget.....P
-00014b10: 0412 044b 0020 043d 0435 0020 0432 044b  ...K. .=.5. .2.K
-00014b20: 0431 0440 0430 043b 0438 0020 0441 0447  .1.@.0.;.8. .A.G
-00014b30: 0451 0442 0020 0434 043b 044f 0020 043d  .Q.B. .4.;.O. .=
-00014b40: 0430 043b 043e 0433 043e 0432 043e 0433  .0.;.>.3.>.2.>.3
-00014b50: 043e 0020 043e 0442 0447 0451 0442 0430  .>. .>.B.G.Q.B.0
-00014b60: 0800 0000 0006 0000 002e 596f 7520 6861  ..........You ha
-00014b70: 7665 6e27 7420 7365 6c65 6374 6564 2061  ven't selected a
-00014b80: 6e20 6163 636f 756e 7420 666f 7220 7461  n account for ta
-00014b90: 7820 7265 706f 7274 0700 0000 0954 6178  x report.....Tax
-00014ba0: 5769 6467 6574 0103 0000 0098 041d 0435  Widget.........5
-00014bb0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
-00014bc0: 0020 043e 0431 0440 0430 0431 043e 0442  . .>.1.@.0.1.>.B
-00014bd0: 0430 0442 044c 0020 0441 0434 0435 043b  .0.B.L. .A.4.5.;
-00014be0: 043a 0443 002c 0020 0442 002e 043a 002e  .:.C.,. .B...:..
-00014bf0: 0020 043d 0435 0020 0437 0430 0434 0430  . .=.5. .7.0.4.0
-00014c00: 043d 0020 0431 0430 043d 043a 0020 0434  .=. .1.0.=.:. .4
-00014c10: 043b 044f 0020 0438 043d 0432 0435 0441  .;.O. .8.=.2.5.A
-00014c20: 0442 0438 0446 0438 043e 043d 043d 043e  .B.8.F.8.>.=.=.>
-00014c30: 0433 043e 0020 0441 0447 0451 0442 0430  .3.>. .A.G.Q.B.0
-00014c40: 003a 0020 0800 0000 0006 0000 003e 4361  .:. .........>Ca
-00014c50: 6e27 7420 7072 6f63 6573 7320 7472 6164  n't process trad
-00014c60: 6520 6173 2062 616e 6b20 6973 6e27 7420  e as bank isn't 
-00014c70: 7365 7420 666f 7220 696e 7665 7374 6d65  set for investme
-00014c80: 6e74 2061 6363 6f75 6e74 3a20 0700 0000  nt account: ....
-00014c90: 0554 7261 6465 0103 0000 0002 2116 0800  .Trade......!...
-00014ca0: 0000 0006 0000 0001 2307 0000 000b 5472  ........#.....Tr
-00014cb0: 6164 6557 6964 6765 7401 0300 0000 0804  adeWidget.......
-00014cc0: 2104 4704 3504 4208 0000 0000 0600 0000  !.G.5.B.........
-00014cd0: 0741 6363 6f75 6e74 0700 0000 0b54 7261  .Account.....Tra
-00014ce0: 6465 5769 6467 6574 0103 0000 0004 0426  deWidget.......&
-00014cf0: 0411 0800 0000 0006 0000 0005 4173 7365  ............Asse
-00014d00: 7407 0000 000b 5472 6164 6557 6964 6765  t.....TradeWidge
-00014d10: 7401 0300 0000 2204 1f04 3e04 3a04 4304  t....."...>.:.C.
-00014d20: 3f04 3a04 3000 2000 2f00 2004 1f04 4004  ?.:.0. ./. ...@.
-00014d30: 3e04 3404 3004 3604 3008 0000 0000 0600  >.4.0.6.0.......
-00014d40: 0000 0a42 7579 202f 2053 656c 6c07 0000  ...Buy / Sell...
-00014d50: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
-00014d60: 0000 1404 1404 3004 4204 3000 2f04 1204  ......0.B.0./...
-00014d70: 4004 3504 3c04 4f08 0000 0000 0600 0000  @.5.<.O.........
-00014d80: 0944 6174 652f 5469 6d65 0700 0000 0b54  .Date/Time.....T
-00014d90: 7261 6465 5769 6467 6574 0103 0000 0010  radeWidget......
-00014da0: 041a 043e 043c 0438 0441 0441 0438 044f  ...>.<.8.A.A.8.O
-00014db0: 0800 0000 0006 0000 0003 4665 6507 0000  ..........Fee...
-00014dc0: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
-00014dd0: 0000 1004 1e04 3f04 3804 4104 3004 3d04  ......?.8.A.0.=.
-00014de0: 3804 3508 0000 0000 0600 0000 044e 6f74  8.5..........Not
-00014df0: 6507 0000 000b 5472 6164 6557 6964 6765  e.....TradeWidge
-00014e00: 7401 0300 0000 0804 2604 3504 3d04 3008  t.......&.5.=.0.
-00014e10: 0000 0000 0600 0000 0550 7269 6365 0700  .........Price..
-00014e20: 0000 0b54 7261 6465 5769 6467 6574 0103  ...TradeWidget..
-00014e30: 0000 000c 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
-00014e40: 0800 0000 0006 0000 0003 5174 7907 0000  ..........Qty...
-00014e50: 000b 5472 6164 6557 6964 6765 7401 0300  ..TradeWidget...
-00014e60: 0000 1a04 1404 3004 4204 3000 2004 4004  ......0.B.0. .@.
-00014e70: 3004 4104 4704 3504 4204 3e04 3208 0000  0.A.G.5.B.>.2...
-00014e80: 0000 0600 0000 0a53 6574 746c 656d 656e  .......Settlemen
-00014e90: 7407 0000 000b 5472 6164 6557 6964 6765  t.....TradeWidge
-00014ea0: 7401 0300 0000 7a04 1a04 3e04 3b04 3804  t.....z...>.;.8.
-00014eb0: 4704 3504 4104 4204 3204 3e00 2004 3004  G.5.A.B.2.>. .0.
-00014ec0: 3a04 4204 3804 3204 3000 2004 3d04 3504  :.B.8.2.0. .=.5.
-00014ed0: 3404 3e04 4104 4204 3004 4204 3e04 4704  4.>.A.B.0.B.>.G.
-00014ee0: 3d04 3e00 2004 3404 3b04 4f00 2004 3e04  =.>. .4.;.O. .>.
-00014ef0: 3104 4004 3004 3104 3e04 4204 3a04 3800  1.@.0.1.>.B.:.8.
-00014f00: 2004 3f04 3504 4004 3504 3204 3e04 3404   .?.5.@.5.2.>.4.
-00014f10: 3000 2e00 2004 1404 3004 4204 3000 3a00  0... ...0.B.0.:.
-00014f20: 2008 0000 0000 0600 0000 4041 7373 6574   .........@Asset
-00014f30: 2061 6d6f 756e 7420 6973 206e 6f74 2065   amount is not e
-00014f40: 6e6f 7567 6820 666f 7220 6173 7365 7420  nough for asset 
-00014f50: 7472 616e 7366 6572 2070 726f 6365 7373  transfer process
-00014f60: 696e 672e 2044 6174 653a 2007 0000 0008  ing. Date: .....
-00014f70: 5472 616e 7366 6572 0103 0000 0052 0421  Transfer.....R.!
-00014f80: 043f 0438 0441 0430 043d 0438 0435 0020  .?.8.A.0.=.8.5. 
-00014f90: 0430 043a 0442 0438 0432 0430 0020 043d  .0.:.B.8.2.0. .=
-00014fa0: 0435 0020 043d 0430 0439 0434 0435 043d  .5. .=.0.9.4.5.=
-00014fb0: 043e 0020 0434 043b 044f 0020 0442 0440  .>. .4.;.O. .B.@
-00014fc0: 0430 043d 0441 0444 0435 0440 0430 002e  .0.=.A.D.5.@.0..
-00014fd0: 0800 0000 0006 0000 0028 4173 7365 7420  .........(Asset 
-00014fe0: 7769 7468 6472 6177 616c 206e 6f74 2066  withdrawal not f
-00014ff0: 6f75 6e64 2066 6f72 2074 7261 6e73 6665  ound for transfe
-00015000: 722e 0700 0000 0854 7261 6e73 6665 7201  r......Transfer.
-00015010: 0300 0000 2e04 1e04 4804 3804 3104 3a04  ........H.8.1.:.
-00015020: 3000 2e00 2004 1a04 4304 4004 4100 2004  0... ...C.@.A. .
-00015030: 4004 3004 3204 3504 3d00 2004 3d04 4304  @.0.2.5.=. .=.C.
-00015040: 3b04 4e08 0000 0000 0600 0000 1045 7272  ;.N..........Err
-00015050: 6f72 2e20 5a65 726f 2072 6174 6507 0000  or. Zero rate...
-00015060: 0008 5472 616e 7366 6572 0103 0000 0084  ..Transfer......
-00015070: 041e 0431 0440 0430 0431 043e 0442 0430  ...1.@.0.1.>.B.0
-00015080: 043d 043d 043e 0435 0020 043a 043e 043b  .=.=.>.5. .:.>.;
-00015090: 0438 0447 0435 0441 0442 0432 043e 0020  .8.G.5.A.B.2.>. 
-000150a0: 043c 0435 043d 044c 0448 0435 002c 0020  .<.5.=.L.H.5.,. 
-000150b0: 0447 0435 043c 0020 043a 043e 043b 0438  .G.5.<. .:.>.;.8
-000150c0: 0447 0435 0441 0442 0432 043e 0020 0432  .G.5.A.B.2.>. .2
-000150d0: 0020 0442 0440 0430 043d 0441 0444 0435  . .B.@.0.=.A.D.5
-000150e0: 0440 0435 002e 0020 0414 0430 0442 0430  .@.5... ...0.B.0
-000150f0: 003a 0020 0800 0000 0006 0000 003b 5072  .:. .........;Pr
-00015100: 6f63 6573 7365 6420 6173 7365 7420 616d  ocessed asset am
-00015110: 6f75 6e74 2069 7320 6c65 7373 2074 6861  ount is less tha
-00015120: 6e20 7472 616e 7366 6572 2061 6d6f 756e  n transfer amoun
-00015130: 742e 2044 6174 653a 2007 0000 0008 5472  t. Date: .....Tr
-00015140: 616e 7366 6572 0103 0000 0002 2116 0800  ansfer......!...
-00015150: 0000 0006 0000 0001 2307 0000 000e 5472  ........#.....Tr
-00015160: 616e 7366 6572 5769 6467 6574 0103 0000  ansferWidget....
-00015170: 000a 0421 0443 043c 043c 0430 0800 0000  ...!.C.<.<.0....
-00015180: 0006 0000 0006 416d 6f75 6e74 0700 0000  ......Amount....
-00015190: 0e54 7261 6e73 6665 7257 6964 6765 7401  .TransferWidget.
-000151a0: 0300 0000 0404 2604 1108 0000 0000 0600  ......&.........
-000151b0: 0000 0541 7373 6574 0700 0000 0e54 7261  ...Asset.....Tra
-000151c0: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
-000151d0: 1404 1404 3004 4204 3000 2f04 1204 4004  ....0.B.0./...@.
-000151e0: 3504 3c04 4f08 0000 0000 0600 0000 0944  5.<.O..........D
-000151f0: 6174 652f 5469 6d65 0700 0000 0e54 7261  ate/Time.....Tra
-00015200: 6e73 6665 7257 6964 6765 7401 0300 0000  nsferWidget.....
-00015210: 1e04 2004 3004 3704 3c04 3504 4000 2004  .. .0.7.<.5.@. .
-00015220: 3a04 3e04 3c04 3804 4104 4104 3804 3808  :.>.<.8.A.A.8.8.
-00015230: 0000 0000 0600 0000 0a46 6565 2061 6d6f  .........Fee amo
-00015240: 756e 7407 0000 000e 5472 616e 7366 6572  unt.....Transfer
-00015250: 5769 6467 6574 0103 0000 0016 041a 043e  Widget.........>
-00015260: 043c 043c 0438 0441 0441 0438 044f 0020  .<.<.8.A.A.8.O. 
-00015270: 0441 0800 0000 0006 0000 0008 4665 6520  .A..........Fee 
-00015280: 6672 6f6d 0700 0000 0e54 7261 6e73 6665  from.....Transfe
-00015290: 7257 6964 6765 7401 0300 0000 0204 2108  rWidget.......!.
-000152a0: 0000 0000 0600 0000 0446 726f 6d07 0000  .........From...
-000152b0: 000e 5472 616e 7366 6572 5769 6467 6574  ..TransferWidget
-000152c0: 0103 0000 0010 041e 043f 0438 0441 0430  .........?.8.A.0
-000152d0: 043d 0438 0435 0800 0000 0006 0000 0004  .=.8.5..........
-000152e0: 4e6f 7465 0700 0000 0e54 7261 6e73 6665  Note.....Transfe
-000152f0: 7257 6964 6765 7401 0300 0000 0404 1d04  rWidget.........
-00015300: 3008 0000 0000 0600 0000 0254 6f07 0000  0..........To...
-00015310: 000e 5472 616e 7366 6572 5769 6467 6574  ..TransferWidget
-00015320: 0103 0000 000e 041f 0435 0440 0435 0432  .........5.@.5.2
-00015330: 043e 0434 0800 0000 0006 0000 0008 5472  .>.4..........Tr
-00015340: 616e 7366 6572 0700 0000 0e54 7261 6e73  ansfer.....Trans
-00015350: 6665 7257 6964 6765 7401 0300 0000 0404  ferWidget.......
-00015360: 1f04 3e08 0000 0000 0600 0000 0845 6e64  ..>..........End
-00015370: 2064 6174 6507 0000 000f 5570 6461 7465   date.....Update
-00015380: 5175 6f74 6573 446c 6701 0300 0000 1204  QuotesDlg.......
-00015390: 1804 4104 4204 3e04 4704 3d04 3804 3a04  ..A.B.>.G.=.8.:.
-000153a0: 3808 0000 0000 0600 0000 0753 6f75 7263  8..........Sourc
-000153b0: 6573 0700 0000 0f55 7064 6174 6551 756f  es.....UpdateQuo
-000153c0: 7465 7344 6c67 0103 0000 0002 0421 0800  tesDlg.......!..
-000153d0: 0000 0006 0000 000a 5374 6172 7420 6461  ........Start da
-000153e0: 7465 0700 0000 0f55 7064 6174 6551 756f  te.....UpdateQuo
-000153f0: 7465 7344 6c67 0103 0000 0028 041e 0431  tesDlg.....(...1
-00015400: 043d 043e 0432 043b 0435 043d 0438 0435  .=.>.2.;.5.=.8.5
-00015410: 0020 043a 043e 0442 0438 0440 043e 0432  . .:.>.B.8.@.>.2
-00015420: 043e 043a 0800 0000 0006 0000 0015 5570  .>.:..........Up
-00015430: 6461 7465 2061 7373 6574 2773 2071 756f  date asset's quo
-00015440: 7465 7307 0000 000f 5570 6461 7465 5175  tes.....UpdateQu
-00015450: 6f74 6573 446c 6701 0300 0000 1400 6400  otesDlg.......d.
-00015460: 6400 2f00 4d00 4d00 2f00 7900 7900 7900  d./.M.M./.y.y.y.
-00015470: 7908 0000 0000 0600 0000 0a64 642f 4d4d  y..........dd/MM
-00015480: 2f79 7979 7907 0000 000f 5570 6461 7465  /yyyy.....Update
-00015490: 5175 6f74 6573 446c 6701 0300 0000 5804  QuotesDlg.....X.
-000154a0: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
-000154b0: 3d04 3e00 2004 3f04 4004 3e04 4704 3804  =.>. .?.@.>.G.8.
-000154c0: 4204 3004 4204 4c00 2004 4804 3004 3104  B.0.B.L. .H.0.1.
-000154d0: 3b04 3e04 3d00 2004 3e04 4204 4704 5104  ;.>.=. .>.B.G.Q.
-000154e0: 4204 3000 2004 3804 3700 2004 4404 3004  B.0. .8.7. .D.0.
-000154f0: 3904 3b04 3000 2008 0000 0000 0600 0000  9.;.0. .........
-00015500: 2543 616e 2774 206c 6f61 6420 7265 706f  %Can't load repo
-00015510: 7274 2074 656d 706c 6174 6520 6672 6f6d  rt template from
-00015520: 2066 696c 6520 0700 0000 0458 4c53 5801   file .....XLSX.
-00015530: 0300 0000 4404 1d04 3504 3204 3e04 3704  ....D...5.2.>.7.
-00015540: 3c04 3e04 3604 3d04 3e00 2004 4104 3e04  <.>.6.=.>. .A.>.
-00015550: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
-00015560: 3e04 4204 4704 5104 4200 2004 3200 2004  >.B.G.Q.B. .2. .
-00015570: 4404 3004 3904 3b00 2008 0000 0000 0600  D.0.9.;. .......
-00015580: 0000 1c43 616e 2774 2073 6176 6520 7265  ...Can't save re
-00015590: 706f 7274 2069 6e74 6f20 6669 6c65 2007  port into file .
-000155a0: 0000 0004 584c 5358 0103 0000 0044 041d  ....XLSX.....D..
-000155b0: 0435 0020 0443 043a 0430 0437 0430 043d  .5. .C.:.0.7.0.=
-000155c0: 0020 0444 043e 0440 043c 0430 0442 0020  . .D.>.@.<.0.B. 
-000155d0: 0434 043b 044f 0020 043f 043e 043b 044f  .4.;.O. .?.>.;.O
-000155e0: 0020 043e 0442 0447 0451 0442 0430 003a  . .>.B.G.Q.B.0.:
-000155f0: 0020 0800 0000 0006 0000 0024 466f 726d  . .........$Form
-00015600: 6174 2069 7320 6d69 7373 696e 6720 666f  at is missing fo
-00015610: 7220 7265 706f 7274 2066 6965 6c64 3a20  r report field: 
-00015620: 0700 0000 0458 4c53 5801 0300 0000 4204  .....XLSX.....B.
-00015630: 1d04 3500 2004 3704 3004 3404 3004 3d00  ..5. .7.0.4.0.=.
-00015640: 2004 4804 3004 3104 3b04 3e04 3d00 2004   .H.0.1.;.>.=. .
-00015650: 3404 3b04 4f00 2004 3404 3004 3d04 3d04  4.;.O. .4.0.=.=.
-00015660: 4b04 4500 2004 3e04 4204 4704 5104 4204  K.E. .>.B.G.Q.B.
-00015670: 3008 0000 0000 0600 0000 1a4e 6f20 7265  0..........No re
-00015680: 706f 7274 2072 6f77 2074 656d 706c 6174  port row templat
-00015690: 6520 7365 7407 0000 0004 584c 5358 0103  e set.....XLSX..
-000156a0: 0000 003a 0428 0430 0431 043b 043e 043d  ...:.(.0.1.;.>.=
-000156b0: 0020 0434 043b 044f 0020 0434 0430 043d  . .4.;.O. .4.0.=
-000156c0: 043d 044b 0445 0020 043d 0435 0020 043d  .=.K.E. .=.5. .=
-000156d0: 0430 0439 0434 0435 043d 003a 0020 0800  .0.9.4.5.=.:. ..
-000156e0: 0000 0006 0000 001f 5265 706f 7274 2072  ........Report r
-000156f0: 6f77 2074 656d 706c 6174 6520 6e6f 7420  ow template not 
-00015700: 666f 756e 643a 2007 0000 0004 584c 5358  found: .....XLSX
-00015710: 0103 0000 0046 041d 0435 0438 0437 0432  .....F...5.8.7.2
-00015720: 0435 0441 0442 043d 0430 044f 0020 0441  .5.A.B.=.0.O. .A
-00015730: 0442 0440 043e 043a 0430 0020 0444 043e  .B.@.>.:.0. .D.>
-00015740: 0440 043c 0430 0442 0438 0440 043e 0432  .@.<.0.B.8.@.>.2
-00015750: 0430 043d 0438 044f 003a 0020 0800 0000  .0.=.8.O.:. ....
-00015760: 0006 0000 001c 556e 7265 636f 676e 697a  ......Unrecogniz
-00015770: 6564 2066 6f72 6d61 7420 7374 7269 6e67  ed format string
-00015780: 3a20 0700 0000 0458 4c53 5801 8800 0000  : .....XLSX.....
-00015790: 0d11 01fd 290b ff14 0204 fd2c 0a13       ....)......,..
+00002bf0: 0b62 7920 4361 7465 676f 7279 0700 0000  .by Category....
+00002c00: 0e43 6174 6567 6f72 7952 6570 6f72 7401  .CategoryReport.
+00002c10: 0300 0000 1404 1a04 3004 4204 3504 3304  ........0.B.5.3.
+00002c20: 3e04 4004 3804 4f00 3a08 0000 0000 0600  >.@.8.O.:.......
+00002c30: 0000 0943 6174 6567 6f72 793a 0700 0000  ...Category:....
+00002c40: 1443 6174 6567 6f72 7952 6570 6f72 7457  .CategoryReportW
+00002c50: 6964 6765 7401 0300 0000 2404 1e04 4204  idget.....$...B.
+00002c60: 4704 5104 4200 2004 3f04 3e00 2004 3a04  G.Q.B. .?.>. .:.
+00002c70: 3004 4204 3504 3304 3e04 4004 3804 3808  0.B.5.3.>.@.8.8.
+00002c80: 0000 0000 0600 0000 1252 6570 6f72 7420  .........Report 
+00002c90: 6279 2063 6174 6567 6f72 7907 0000 0014  by category.....
+00002ca0: 4361 7465 676f 7279 5265 706f 7274 5769  CategoryReportWi
+00002cb0: 6467 6574 0103 0000 0018 041d 0430 0438  dget.........0.8
+00002cc0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
+00002cd0: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
+00002ce0: 0700 0000 1143 6174 6567 6f72 7954 7265  .....CategoryTre
+00002cf0: 654d 6f64 656c 0103 0000 000c 0427 0430  eModel.......'.0
+00002d00: 0441 0442 0430 044f 0800 0000 0006 0000  .A.B.0.O........
+00002d10: 0005 4f66 7465 6e07 0000 0011 4361 7465  ..Often.....Cate
+00002d20: 676f 7279 5472 6565 4d6f 6465 6c01 0300  goryTreeModel...
+00002d30: 0000 2004 1304 4004 3004 4404 3804 3a00  .. ...@.0.D.8.:.
+00002d40: 2004 4604 3504 3d04 4b00 2004 3404 3b04   .F.5.=.K. .4.;.
+00002d50: 4f00 2008 0000 0000 0600 0000 1050 7269  O. ..........Pri
+00002d60: 6365 2063 6861 7274 2066 6f72 2007 0000  ce chart for ...
+00002d70: 000b 4368 6172 7457 696e 646f 7701 0300  ..ChartWindow...
+00002d80: 0000 1a04 2604 3504 3d04 3d04 3004 4f00  ....&.5.=.=.0.O.
+00002d90: 2004 3104 4304 3c04 3004 3304 3008 0000   .1.C.<.0.3.0...
+00002da0: 0000 0600 0000 0541 7373 6574 0700 0000  .......Asset....
+00002db0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002dc0: 656c 0103 0000 001a 0414 0430 0442 0430  el.........0.B.0
+00002dd0: 0020 0437 0430 043a 0440 044b 0442 0438  . .7.0.:.@.K.B.8
+00002de0: 044f 0800 0000 0006 0000 000a 436c 6f73  .O..........Clos
+00002df0: 6520 4461 7465 0700 0000 1143 6c6f 7365  e Date.....Close
+00002e00: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
+00002e10: 0026 0414 0430 0442 0430 002f 0432 0440  .&...0.B.0./.2.@
+00002e20: 0435 043c 044f 0020 0437 0430 043a 0440  .5.<.O. .7.0.:.@
+00002e30: 044b 0442 0438 044f 0800 0000 0006 0000  .K.B.8.O........
+00002e40: 000f 436c 6f73 6520 4461 7465 2f54 696d  ..Close Date/Tim
+00002e50: 6507 0000 0011 436c 6f73 6564 5472 6164  e.....ClosedTrad
+00002e60: 6573 4d6f 6465 6c01 0300 0000 1a04 2604  esModel.......&.
+00002e70: 3504 3d04 3000 2004 3704 3004 3a04 4004  5.=.0. .7.0.:.@.
+00002e80: 4b04 4204 3804 4f08 0000 0000 0600 0000  K.B.8.O.........
+00002e90: 0b43 6c6f 7365 2050 7269 6365 0700 0000  .Close Price....
+00002ea0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002eb0: 656c 0103 0000 0010 041a 043e 043c 0438  el.........>.<.8
+00002ec0: 0441 0441 0438 044f 0800 0000 0006 0000  .A.A.8.O........
+00002ed0: 0003 4665 6507 0000 0011 436c 6f73 6564  ..Fee.....Closed
+00002ee0: 5472 6164 6573 4d6f 6465 6c01 0300 0000  TradesModel.....
+00002ef0: 1404 1f04 4004 3804 3c04 3504 4704 3004  ....@.8.<.5.G.0.
+00002f00: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
+00002f10: 6f74 6507 0000 0011 436c 6f73 6564 5472  ote.....ClosedTr
+00002f20: 6164 6573 4d6f 6465 6c01 0300 0000 1a04  adesModel.......
+00002f30: 1404 3004 4204 3000 2004 3e04 4204 3a04  ..0.B.0. .>.B.:.
+00002f40: 4004 4b04 4204 3804 4f08 0000 0000 0600  @.K.B.8.O.......
+00002f50: 0000 094f 7065 6e20 4461 7465 0700 0000  ...Open Date....
+00002f60: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+00002f70: 656c 0103 0000 0026 0414 0430 0442 0430  el.....&...0.B.0
+00002f80: 002f 0412 0440 0435 043c 044f 0020 043e  ./...@.5.<.O. .>
+00002f90: 0442 043a 0440 044b 0442 0438 044f 0800  .B.:.@.K.B.8.O..
+00002fa0: 0000 0006 0000 000e 4f70 656e 2044 6174  ........Open Dat
+00002fb0: 652f 5469 6d65 0700 0000 1143 6c6f 7365  e/Time.....Close
+00002fc0: 6454 7261 6465 734d 6f64 656c 0103 0000  dTradesModel....
+00002fd0: 001a 0426 0435 043d 0430 0020 043e 0442  ...&.5.=.0. .>.B
+00002fe0: 043a 0440 044b 0442 0438 044f 0800 0000  .:.@.K.B.8.O....
+00002ff0: 0006 0000 000a 4f70 656e 2050 7269 6365  ......Open Price
+00003000: 0700 0000 1143 6c6f 7365 6454 7261 6465  .....ClosedTrade
+00003010: 734d 6f64 656c 0103 0000 0006 041f 0438  sModel.........8
+00003020: 0423 0800 0000 0006 0000 0003 502f 4c07  .#..........P/L.
+00003030: 0000 0011 436c 6f73 6564 5472 6164 6573  ....ClosedTrades
+00003040: 4d6f 6465 6c01 0300 0000 0c04 1f04 3804  Model.........8.
+00003050: 2300 2c00 2000 2508 0000 0000 0600 0000  #.,. .%.........
+00003060: 0650 2f4c 2c20 2507 0000 0011 436c 6f73  .P/L, %.....Clos
+00003070: 6564 5472 6164 6573 4d6f 6465 6c01 0300  edTradesModel...
+00003080: 0000 0c04 1a04 3e04 3b00 2d04 3204 3e08  ......>.;.-.2.>.
+00003090: 0000 0000 0600 0000 0351 7479 0700 0000  .........Qty....
+000030a0: 1143 6c6f 7365 6454 7261 6465 734d 6f64  .ClosedTradesMod
+000030b0: 656c 0103 0000 00a0 041a 043e 043b 0438  el.........>.;.8
+000030c0: 0447 0435 0442 0432 043e 0020 0446 0435  .G.5.B.2.>. .F.5
+000030d0: 043d 043d 044b 0445 0020 0431 0443 043c  .=.=.K.E. .1.C.<
+000030e0: 0430 0433 0020 043d 0435 0434 043e 0441  .0.3. .=.5.4.>.A
+000030f0: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
+00003100: 0434 043b 044f 0020 043e 0431 0440 0430  .4.;.O. .>.1.@.0
+00003110: 0431 043e 0442 043a 0438 0020 043a 043e  .1.>.B.:.8. .:.>
+00003120: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
+00003130: 043d 043e 0433 043e 0020 0441 043e 0431  .=.>.3.>. .A.>.1
+00003140: 044b 0442 0438 044f 002e 0020 0414 0430  .K.B.8.O... ...0
+00003150: 0442 0430 003a 0020 0800 0000 0006 0000  .B.0.:. ........
+00003160: 0042 4173 7365 7420 616d 6f75 6e74 2069  .BAsset amount i
+00003170: 7320 6e6f 7420 656e 6f75 6768 2066 6f72  s not enough for
+00003180: 2063 6f72 706f 7261 7465 2061 6374 696f   corporate actio
+00003190: 6e20 7072 6f63 6573 7369 6e67 2e20 4461  n processing. Da
+000031a0: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
+000031b0: 7465 4163 7469 6f6e 0103 0000 0074 0426  teAction.....t.&
+000031c0: 0411 0020 043d 0435 0020 044f 0432 043b  ... .=.5. .O.2.;
+000031d0: 044f 0435 0442 0441 044f 0020 0447 0430  .O.5.B.A.O. .G.0
+000031e0: 0441 0442 044c 044e 0020 0440 0435 0437  .A.B.L.N. .@.5.7
+000031f0: 0443 043b 044c 0442 0430 0442 043e 0432  .C.;.L.B.0.B.>.2
+00003200: 0020 043a 043e 0440 043f 043e 0440 0430  . .:.>.@.?.>.@.0
+00003210: 0442 0438 0432 043d 043e 0433 043e 0020  .B.8.2.=.>.3.>. 
+00003220: 0441 043e 0431 044b 0442 0438 044f 003a  .A.>.1.K.B.8.O.:
+00003230: 0020 0800 0000 0006 0000 0030 4173 7365  . .........0Asse
+00003240: 7420 6973 6e27 7420 6120 7061 7274 206f  t isn't a part o
+00003250: 6620 636f 7270 6f72 6174 6520 6163 7469  f corporate acti
+00003260: 6f6e 2072 6573 756c 7473 3a20 0700 0000  on results: ....
+00003270: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003280: 0103 0000 0056 041d 0435 0020 0437 0430  .....V...5. .7.0
+00003290: 0434 0430 043d 0020 0442 0438 043f 0020  .4.0.=. .B.8.?. 
+000032a0: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
+000032b0: 0438 0432 043d 043e 0433 043e 0020 0441  .8.2.=.>.3.>. .A
+000032c0: 043e 0431 044b 0442 0438 044f 002e 0020  .>.1.K.B.8.O... 
+000032d0: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
+000032e0: 0006 0000 002b 436f 7270 6f72 6174 6520  .....+Corporate 
+000032f0: 6163 7469 6f6e 2074 7970 6520 6973 6e27  action type isn'
+00003300: 7420 6465 6669 6e65 642e 2044 6174 653a  t defined. Date:
+00003310: 2007 0000 000f 436f 7270 6f72 6174 6541   .....CorporateA
+00003320: 6374 696f 6e01 0300 0000 1204 1404 3504  ction.........5.
+00003330: 3b04 3804 4104 4204 3804 3d04 3308 0000  ;.8.A.B.8.=.3...
+00003340: 0000 0600 0000 0944 656c 6973 7469 6e67  .......Delisting
+00003350: 0700 0000 0f43 6f72 706f 7261 7465 4163  .....CorporateAc
+00003360: 7469 6f6e 0103 0000 002c 0420 0435 043e  tion.....,. .5.>
+00003370: 0440 0433 0430 043d 0438 0437 0430 0446  .@.3.0.=.8.7.0.F
+00003380: 0438 044f 0020 043a 043e 043c 043f 0430  .8.O. .:.>.<.?.0
+00003390: 043d 0438 0438 0800 0000 0006 0000 0006  .=.8.8..........
+000033a0: 4d65 7267 6572 0700 0000 0f43 6f72 706f  Merger.....Corpo
+000033b0: 7261 7465 4163 7469 6f6e 0103 0000 00ac  rateAction......
+000033c0: 0420 0435 0437 0443 043b 044c 0442 0430  . .5.7.C.;.L.B.0
+000033d0: 0442 044b 0020 043a 043e 0440 043f 043e  .B.K. .:.>.@.?.>
+000033e0: 0440 0430 0442 0438 0432 043d 043e 0433  .@.0.B.8.2.=.>.3
+000033f0: 043e 0020 0441 043e 0431 044b 0442 0438  .>. .A.>.1.K.B.8
+00003400: 044f 0020 043d 0435 0020 0440 0430 0441  .O. .=.5. .@.0.A
+00003410: 043f 0440 0435 0434 0435 043b 044f 044e  .?.@.5.4.5.;.O.N
+00003420: 0442 0020 0031 0030 0030 0025 0020 0441  .B. .1.0.0.%. .A
+00003430: 0442 043e 0438 043c 043e 0441 0442 0438  .B.>.8.<.>.A.B.8
+00003440: 0020 0438 0437 043d 0430 0447 0430 043b  . .8.7.=.0.G.0.;
+00003450: 044c 043d 043e 0433 043e 0020 0430 043a  .L.=.>.3.>. .0.:
+00003460: 0442 0438 0432 0430 002e 0020 0800 0000  .B.8.2.0... ....
+00003470: 0006 0000 004d 5265 7375 6c74 7320 7661  .....MResults va
+00003480: 6c75 6520 6f66 2063 6f72 706f 7261 7465  lue of corporate
+00003490: 2061 6374 696f 6e20 646f 6573 6e27 7420   action doesn't 
+000034a0: 6d61 7463 6820 3130 3025 206f 6620 696e  match 100% of in
+000034b0: 6974 6961 6c20 6173 7365 7420 7661 6c75  itial asset valu
+000034c0: 652e 2007 0000 000f 436f 7270 6f72 6174  e. .....Corporat
+000034d0: 6541 6374 696f 6e01 0300 0000 3a04 1204  eAction.....:...
+000034e0: 4b04 3404 3504 3b04 3504 3d04 3804 3500  K.4.5.;.5.=.8.5.
+000034f0: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
+00003500: 3800 2000 2804 4104 3f04 3804 3d00 2d04  8. .(.A.?.8.=.-.
+00003510: 3e04 4404 4400 2908 0000 0000 0600 0000  >.D.D.).........
+00003520: 0853 7069 6e2d 6f66 6607 0000 000f 436f  .Spin-off.....Co
+00003530: 7270 6f72 6174 6541 6374 696f 6e01 0300  rporateAction...
+00003540: 0000 0a04 2104 3f04 3b04 3804 4208 0000  ....!.?.;.8.B...
+00003550: 0000 0600 0000 0553 706c 6974 0700 0000  .......Split....
+00003560: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003570: 0103 0000 001a 0421 043c 0435 043d 0430  .......!.<.5.=.0
+00003580: 0020 0441 0438 043c 0432 043e 043b 0430  . .A.8.<.2.>.;.0
+00003590: 0800 0000 0006 0000 000d 5379 6d62 6f6c  ..........Symbol
+000035a0: 2063 6861 6e67 6507 0000 000f 436f 7270   change.....Corp
+000035b0: 6f72 6174 6541 6374 696f 6e01 0300 0000  orateAction.....
+000035c0: 1804 1d04 1504 1e04 1f04 2004 1504 1404  .......... .....
+000035d0: 1504 1b04 1504 1d04 1e08 0000 0000 0600  ................
+000035e0: 0000 0955 4e44 4546 494e 4544 0700 0000  ...UNDEFINED....
+000035f0: 0f43 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003600: 0103 0000 00ae 041d 0435 043f 043e 0434  .........5.?.>.4
+00003610: 0435 0440 0436 0438 0432 0430 0435 043c  .5.@.6.8.2.0.5.<
+00003620: 044b 0439 0020 0441 043b 0443 0447 0430  .K.9. .A.;.C.G.0
+00003630: 0439 003a 0020 041a 043e 0440 043f 043e  .9.:. ...>.@.?.>
+00003640: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
+00003650: 0020 0441 043e 0431 044b 0442 0438 0435  . .A.>.1.K.B.8.5
+00003660: 0020 043f 043e 043a 0440 044b 0432 0430  . .?.>.:.@.K.2.0
+00003670: 0435 0442 0020 043d 0435 0020 0432 0441  .5.B. .=.5. .2.A
+00003680: 044e 0020 043e 0442 043a 0440 044b 0442  .N. .>.B.:.@.K.B
+00003690: 0443 044e 0020 043f 043e 0437 0438 0446  .C.N. .?.>.7.8.F
+000036a0: 0438 044e 002e 0020 0414 0430 0442 0430  .8.N... ...0.B.0
+000036b0: 003a 0020 0800 0000 0006 0000 0046 556e  .:. .........FUn
+000036c0: 6861 6e64 6c65 6420 6361 7365 3a20 436f  handled case: Co
+000036d0: 7270 6f72 6174 6520 6163 7469 6f6e 2063  rporate action c
+000036e0: 6f76 6572 7320 6e6f 7420 6675 6c6c 206f  overs not full o
+000036f0: 7065 6e20 706f 7369 7469 6f6e 2e20 4461  pen position. Da
+00003700: 7465 3a20 0700 0000 0f43 6f72 706f 7261  te: .....Corpora
+00003710: 7465 4163 7469 6f6e 0103 0000 0002 2116  teAction......!.
+00003720: 0800 0000 0006 0000 0001 2307 0000 0015  ..........#.....
+00003730: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003740: 6964 6765 7401 0300 0000 0804 2104 4704  idget.......!.G.
+00003750: 3504 4208 0000 0000 0600 0000 0741 6363  5.B..........Acc
+00003760: 6f75 6e74 0700 0000 1543 6f72 706f 7261  ount.....Corpora
+00003770: 7465 4163 7469 6f6e 5769 6467 6574 0103  teActionWidget..
+00003780: 0000 001c 0414 043e 0431 0430 0432 0438  .......>.1.0.2.8
+00003790: 0442 044c 0020 0430 043a 0442 0438 0432  .B.L. .0.:.B.8.2
+000037a0: 0800 0000 0006 0000 0009 4164 6420 6173  ..........Add as
+000037b0: 7365 7407 0000 0015 436f 7270 6f72 6174  set.....Corporat
+000037c0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+000037d0: 0000 0404 2604 1108 0000 0000 0600 0000  ....&...........
+000037e0: 0541 7373 6574 0700 0000 1543 6f72 706f  .Asset.....Corpo
+000037f0: 7261 7465 4163 7469 6f6e 5769 6467 6574  rateActionWidget
+00003800: 0103 0000 002c 041a 043e 0440 043f 043e  .....,...>.@.?.>
+00003810: 0440 0430 0442 0438 0432 043d 043e 0435  .@.0.B.8.2.=.>.5
+00003820: 0020 0434 0435 0439 0441 0442 0432 0438  . .4.5.9.A.B.2.8
+00003830: 0435 0800 0000 0006 0000 0010 436f 7270  .5..........Corp
+00003840: 6f72 6174 6520 4163 7469 6f6e 0700 0000  orate Action....
+00003850: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003860: 5769 6467 6574 0103 0000 0014 0414 0430  Widget.........0
+00003870: 0442 0430 002f 0412 0440 0435 043c 044f  .B.0./...@.5.<.O
+00003880: 0800 0000 0006 0000 0009 4461 7465 2f54  ..........Date/T
+00003890: 696d 6507 0000 0015 436f 7270 6f72 6174  ime.....Corporat
+000038a0: 6541 6374 696f 6e57 6964 6765 7401 0300  eActionWidget...
+000038b0: 0000 1204 1404 3504 3b04 3804 4104 4204  ......5.;.8.A.B.
+000038c0: 3804 3d04 3308 0000 0000 0600 0000 0944  8.=.3..........D
+000038d0: 656c 6973 7469 6e67 0700 0000 1543 6f72  elisting.....Cor
+000038e0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+000038f0: 6574 0103 0000 0044 041d 0435 0432 043e  et.....D...5.2.>
+00003900: 0437 043c 043e 0436 043d 043e 0020 0434  .7.<.>.6.=.>. .4
+00003910: 043e 0431 0430 0432 0438 0442 044c 0020  .>.1.0.2.8.B.L. 
+00003920: 043d 043e 0432 0443 044e 0020 0437 0430  .=.>.2.C.N. .7.0
+00003930: 043f 0438 0441 044c 003a 0020 0800 0000  .?.8.A.L.:. ....
+00003940: 0006 0000 001a 4661 696c 6564 2074 6f20  ......Failed to 
+00003950: 6164 6420 6e65 7720 7265 636f 7264 3a20  add new record: 
+00003960: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003970: 7469 6f6e 5769 6467 6574 0103 0000 0028  tionWidget.....(
+00003980: 041e 0431 044a 0435 0434 0438 043d 0435  ...1.J.5.4.8.=.5
+00003990: 043d 0438 0435 0020 043a 043e 043c 043f  .=.8.5. .:.>.<.?
+000039a0: 0430 043d 0438 0438 0800 0000 0006 0000  .0.=.8.8........
+000039b0: 0006 4d65 7267 6572 0700 0000 1543 6f72  ..Merger.....Cor
+000039c0: 706f 7261 7465 4163 7469 6f6e 5769 6467  porateActionWidg
+000039d0: 6574 0103 0000 0006 004e 002f 0041 0800  et.......N./.A..
+000039e0: 0000 0006 0000 0003 4e2f 4107 0000 0015  ........N/A.....
+000039f0: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003a00: 6964 6765 7401 0300 0000 1004 1e04 3f04  idget.........?.
+00003a10: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
+00003a20: 0600 0000 044e 6f74 6507 0000 0015 436f  .....Note.....Co
+00003a30: 7270 6f72 6174 6541 6374 696f 6e57 6964  rporateActionWid
+00003a40: 6765 7401 0300 0000 4804 1e04 4804 3804  get.....H...H.8.
+00003a50: 3104 3a04 3000 2004 3f04 4004 3800 2004  1.:.0. .?.@.8. .
+00003a60: 3704 3004 3f04 3804 4104 3800 2004 3404  7.0.?.8.A.8. .4.
+00003a70: 3504 4204 3004 3b04 3504 3900 2004 3e04  5.B.0.;.5.9. .>.
+00003a80: 3f04 3504 4004 3004 4604 3804 3800 3a00  ?.5.@.0.F.8.8.:.
+00003a90: 2008 0000 0000 0600 0000 214f 7065 7261   .........!Opera
+00003aa0: 7469 6f6e 2064 6574 6169 6c73 2073 7562  tion details sub
+00003ab0: 6d69 7420 6661 696c 6564 3a20 0700 0000  mit failed: ....
+00003ac0: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003ad0: 5769 6467 6574 0103 0000 0038 041e 0448  Widget.....8...H
+00003ae0: 0438 0431 043a 0430 0020 043f 0440 0438  .8.1.:.0. .?.@.8
+00003af0: 0020 0437 0430 043f 0438 0441 0438 0020  . .7.0.?.8.A.8. 
+00003b00: 043e 043f 0435 0440 0430 0446 0438 0438  .>.?.5.@.0.F.8.8
+00003b10: 003a 0020 0800 0000 0006 0000 0019 4f70  .:. ..........Op
+00003b20: 6572 6174 696f 6e20 7375 626d 6974 2066  eration submit f
+00003b30: 6169 6c65 643a 2007 0000 0015 436f 7270  ailed: .....Corp
+00003b40: 6f72 6174 6541 6374 696f 6e57 6964 6765  orateActionWidge
+00003b50: 7401 0300 0000 0c04 1a04 3e04 3b00 2d04  t.........>.;.-.
+00003b60: 3204 3e08 0000 0000 0600 0000 0351 7479  2.>..........Qty
+00003b70: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003b80: 7469 6f6e 5769 6467 6574 0103 0000 001a  tionWidget......
+00003b90: 0423 0434 0430 043b 0438 0442 044c 0020  .#.4.0.;.8.B.L. 
+00003ba0: 0430 043a 0442 0438 0432 0800 0000 0006  .0.:.B.8.2......
+00003bb0: 0000 000c 5265 6d6f 7665 2061 7373 6574  ....Remove asset
+00003bc0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003bd0: 7469 6f6e 5769 6467 6574 0103 ffff ffff  tionWidget......
+00003be0: 0800 0000 0006 0000 0008 5370 696e 2d4f  ..........Spin-O
+00003bf0: 6666 0700 0000 1543 6f72 706f 7261 7465  ff.....Corporate
+00003c00: 4163 7469 6f6e 5769 6467 6574 0103 0000  ActionWidget....
+00003c10: 000a 0421 043f 043b 0438 0442 0800 0000  ...!.?.;.8.B....
+00003c20: 0006 0000 0005 5370 6c69 7407 0000 0015  ......Split.....
+00003c30: 436f 7270 6f72 6174 6541 6374 696f 6e57  CorporateActionW
+00003c40: 6964 6765 7401 0300 0000 1a04 2104 3c04  idget.......!.<.
+00003c50: 3504 3d04 3000 2004 4104 3804 3c04 3204  5.=.0. .A.8.<.2.
+00003c60: 3e04 3b04 3008 0000 0000 0600 0000 0d53  >.;.0..........S
+00003c70: 796d 626f 6c20 6368 616e 6765 0700 0000  ymbol change....
+00003c80: 1543 6f72 706f 7261 7465 4163 7469 6f6e  .CorporateAction
+00003c90: 5769 6467 6574 0103 0000 0006 0422 0438  Widget.......".8
+00003ca0: 043f 0800 0000 0006 0000 0004 5479 7065  .?..........Type
+00003cb0: 0700 0000 1543 6f72 706f 7261 7465 4163  .....CorporateAc
+00003cc0: 7469 6f6e 5769 6467 6574 0103 0000 0034  tionWidget.....4
+00003cd0: 0424 043e 0440 043c 0430 0442 0020 0431  .$.>.@.<.0.B. .1
+00003ce0: 0430 0437 044b 0020 0434 0430 043d 043d  .0.7.K. .4.0.=.=
+00003cf0: 044b 0445 0020 0443 0441 0442 0430 0440  .K.E. .C.A.B.0.@
+00003d00: 0435 043b 0800 0000 0006 0000 001b 4461  .5.;..........Da
+00003d10: 7461 6261 7365 2066 6f72 6d61 7420 6973  tabase format is
+00003d20: 206f 7574 6461 7465 6407 0000 0002 4442   outdated.....DB
+00003d30: 0103 0000 0064 0412 044b 0020 0441 043e  .....d...K. .A.>
+00003d40: 0433 043b 0430 0441 043d 044b 0020 0441  .3.;.0.A.=.K. .A
+00003d50: 043a 043e 043d 0432 0435 0440 0442 0438  .:.>.=.2.5.@.B.8
+00003d60: 0440 043e 0432 0430 0442 044c 0020 0434  .@.>.2.0.B.L. .4
+00003d70: 0430 043d 043d 044b 0435 0020 0432 0020  .0.=.=.K.5. .2. 
+00003d80: 043d 043e 0432 044b 0439 0020 0444 043e  .=.>.2.K.9. .D.>
+00003d90: 0440 043c 0430 0442 003f 0800 0000 0006  .@.<.0.B.?......
+00003da0: 0000 0032 446f 2079 6f75 2061 6772 6565  ...2Do you agree
+00003db0: 2074 6f20 7570 6772 6164 6520 796f 7572   to upgrade your
+00003dc0: 2064 6174 6120 746f 206e 6577 6572 2066   data to newer f
+00003dd0: 6f72 6d61 743f 0700 0000 0244 4201 0300  ormat?.....DB...
+00003de0: 0000 5e04 2404 3e04 4004 3c04 3000 2000  ..^.$.>.@.<.0. .
+00003df0: 3300 2d04 1d04 1404 2404 1b00 2004 3404  3.-.....$... .4.
+00003e00: 3b04 4f00 2004 4d04 4204 3e04 3304 3e00  ;.O. .M.B.>.3.>.
+00003e10: 2004 3304 3e04 3404 3000 2004 3d04 3500   .3.>.4.0. .=.5.
+00003e20: 2004 3f04 3e04 3404 3404 3504 4004 3604   .?.>.4.4.5.@.6.
+00003e30: 3804 3204 3004 3504 4204 4104 4f00 3a00  8.2.0.5.B.A.O.:.
+00003e40: 2008 0000 0000 0600 0000 2633 2d4e 4446   .........&3-NDF
+00003e50: 4c20 666f 726d 2069 736e 2774 2073 7570  L form isn't sup
+00003e60: 6f6f 7274 6564 2066 6f72 2079 6561 723a  oorted for year:
+00003e70: 2007 0000 0004 444c 5347 0103 0000 0086   .....DLSG......
+00003e80: 0421 0442 0440 0430 043d 0430 0020 0426  .!.B.@.0.=.0. .&
+00003e90: 0411 0020 043d 0435 0020 0437 0430 0434  ... .=.5. .7.0.4
+00003ea0: 0430 043d 0430 002c 0020 0434 0438 0432  .0.=.0.,. .4.8.2
+00003eb0: 0438 0434 0435 043d 0434 0020 043d 0435  .8.4.5.=.4. .=.5
+00003ec0: 0020 0431 0443 0434 0435 0442 0020 0432  . .1.C.4.5.B. .2
+00003ed0: 043a 043b 044e 0447 0451 043d 0020 0432  .:.;.N.G.Q.=. .2
+00003ee0: 0020 0434 0435 043a 043b 0430 0440 0430  . .4.5.:.;.0.@.0
+00003ef0: 0446 0438 044e 0020 0033 002d 041d 0424  .F.8.N. .3.-...$
+00003f00: 0414 041b 0020 0800 0000 0006 0000 0047  ..... .........G
+00003f10: 4163 636f 756e 7420 636f 756e 7472 7920  Account country 
+00003f20: 6973 206e 6f74 2073 6574 2066 6f72 2061  is not set for a
+00003f30: 7373 6574 2c20 6469 7669 6465 6e64 2069  sset, dividend i
+00003f40: 736e 2774 2069 6e63 6c75 6465 2069 6e20  sn't include in 
+00003f50: 332d 4e44 464c 2007 0000 0004 444c 5347  3-NDFL .....DLSG
+00003f60: 0103 0000 004a 0412 0430 043b 044e 0442  .....J...0.;.N.B
+00003f70: 0430 0020 043d 0435 0020 043f 043e 0434  .0. .=.5. .?.>.4
+00003f80: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
+00003f90: 0442 0441 044f 0020 0434 043b 044f 0020  .B.A.O. .4.;.O. 
+00003fa0: 0033 002d 041d 0414 0424 041b 003a 0020  .3.-.....$...:. 
+00003fb0: 0800 0000 0006 0000 0026 4375 7272 656e  .........&Curren
+00003fc0: 6379 2069 7320 6e6f 7420 7375 7070 6f72  cy is not suppor
+00003fd0: 7465 6420 666f 7220 332d 4e44 464c 3a20  ted for 3-NDFL: 
+00003fe0: 0700 0000 0444 4c53 4701 0300 0000 1404  .....DLSG.......
+00003ff0: 4d04 3a04 4104 3f04 3804 4004 3004 4604  M.:.A.?.8.@.0.F.
+00004000: 3804 4f08 0000 0000 0600 0000 0665 7870  8.O..........exp
+00004010: 6972 7907 0000 000c 4461 7461 4465 6c65  iry.....DataDele
+00004020: 6761 7465 0103 0000 000e 043d 043e 043c  gate.......=.>.<
+00004030: 0438 043d 0430 043b 0800 0000 0006 0000  .8.=.0.;........
+00004040: 0009 7072 696e 6369 7061 6c07 0000 000c  ..principal.....
+00004050: 4461 7461 4465 6c65 6761 7465 0103 0000  DataDelegate....
+00004060: 000e 0440 0435 0433 002e 043a 043e 0434  ...@.5.3...:.>.4
+00004070: 0800 0000 0006 0000 0008 7265 672e 636f  ..........reg.co
+00004080: 6465 0700 0000 0c44 6174 6144 656c 6567  de.....DataDeleg
+00004090: 6174 6501 0300 0000 0604 4204 4d04 3308  ate.......B.M.3.
+000040a0: 0000 0000 0600 0000 0374 6167 0700 0000  .........tag....
+000040b0: 0c44 6174 6144 656c 6567 6174 6501 0300  .DataDelegate...
+000040c0: 0000 1004 1204 4104 3500 2004 3404 3004  ......A.5. .4.0.
+000040d0: 4204 4b08 0000 0000 0600 0000 0941 6c6c  B.K..........All
+000040e0: 2064 6174 6573 0700 0000 1144 6174 6552   dates.....DateR
+000040f0: 616e 6765 5365 6c65 6374 6f72 0103 0000  angeSelector....
+00004100: 0004 0421 003a 0800 0000 0006 0000 0005  ...!.:..........
+00004110: 4672 6f6d 3a07 0000 0011 4461 7465 5261  From:.....DateRa
+00004120: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
+00004130: 0a04 1c04 3504 4104 4f04 4608 0000 0000  ....5.A.O.F.....
+00004140: 0600 0000 054d 6f6e 7468 0700 0000 1144  .....Month.....D
+00004150: 6174 6552 616e 6765 5365 6c65 6374 6f72  ateRangeSelector
+00004160: 0103 0000 001c 041f 0440 0435 0434 044b  .........@.5.4.K
+00004170: 0434 0443 0449 0438 0439 0020 0433 043e  .4.C.I.8.9. .3.>
+00004180: 0434 0800 0000 0006 0000 000d 5072 6576  .4..........Prev
+00004190: 696f 7573 2079 6561 7207 0000 0011 4461  ious year.....Da
+000041a0: 7465 5261 6e67 6553 656c 6563 746f 7201  teRangeSelector.
+000041b0: 0300 0000 0e04 1a04 3204 3004 4004 4204  ........2.0.@.B.
+000041c0: 3004 3b08 0000 0000 0600 0000 0751 7561  0.;..........Qua
+000041d0: 7274 6572 0700 0000 1144 6174 6552 616e  rter.....DateRan
+000041e0: 6765 5365 6c65 6374 6f72 0103 0000 0024  geSelector.....$
+000041f0: 0422 0435 043a 0443 0449 0438 0439 0020  .".5.:.C.I.8.9. 
+00004200: 0434 043e 0020 0441 0435 0433 043e 0434  .4.>. .A.5.3.>.4
+00004210: 043d 044f 0800 0000 0006 0000 000f 5175  .=.O..........Qu
+00004220: 6172 7465 7220 746f 2064 6174 6507 0000  arter to date...
+00004230: 0011 4461 7465 5261 6e67 6553 656c 6563  ..DateRangeSelec
+00004240: 746f 7201 0300 0000 1604 2204 3504 3a04  tor.......".5.:.
+00004250: 4304 4904 3804 3900 2004 3304 3e04 3408  C.I.8.9. .3.>.4.
+00004260: 0000 0000 0600 0000 0954 6869 7320 7965  .........This ye
+00004270: 6172 0700 0000 1144 6174 6552 616e 6765  ar.....DateRange
+00004280: 5365 6c65 6374 6f72 0103 0000 0006 0414  Selector........
+00004290: 043e 003a 0800 0000 0006 0000 0003 546f  .>.:..........To
+000042a0: 3a07 0000 0011 4461 7465 5261 6e67 6553  :.....DateRangeS
+000042b0: 656c 6563 746f 7201 0300 0000 0c04 1d04  elector.........
+000042c0: 3504 3404 3504 3b04 4f08 0000 0000 0600  5.4.5.;.O.......
+000042d0: 0000 0457 6565 6b07 0000 0011 4461 7465  ...Week.....Date
+000042e0: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
+000042f0: 0000 0604 1304 3e04 3408 0000 0000 0600  ......>.4.......
+00004300: 0000 0459 6561 7207 0000 0011 4461 7465  ...Year.....Date
+00004310: 5261 6e67 6553 656c 6563 746f 7201 0300  RangeSelector...
+00004320: 0000 1c04 1304 3e04 3400 2004 3404 3e00  ......>.4. .4.>.
+00004330: 2004 4104 3504 3304 3e04 3404 3d04 4f08   .A.5.3.>.4.=.O.
+00004340: 0000 0000 0600 0000 0c59 6561 7220 746f  .........Year to
+00004350: 2064 6174 6507 0000 0011 4461 7465 5261   date.....DateRa
+00004360: 6e67 6553 656c 6563 746f 7201 0300 0000  ngeSelector.....
+00004370: 1e04 2104 3404 3504 3b04 3a04 3800 2004  ..!.4.5.;.:.8. .
+00004380: 3f04 3e00 2004 4104 4704 3504 4204 4308  ?.>. .A.G.5.B.C.
+00004390: 0000 0000 0600 0000 1044 6561 6c73 2062  .........Deals b
+000043a0: 7920 4163 636f 756e 7407 0000 000b 4465  y Account.....De
+000043b0: 616c 7352 6570 6f72 7401 0300 0000 0a04  alsReport.......
+000043c0: 2104 4704 3504 4200 3a08 0000 0000 0600  !.G.5.B.:.......
+000043d0: 0000 0841 6363 6f75 6e74 3a07 0000 0011  ...Account:.....
+000043e0: 4465 616c 7352 6570 6f72 7457 6964 6765  DealsReportWidge
+000043f0: 7401 0300 0000 0c04 2104 3404 3504 3b04  t.......!.4.5.;.
+00004400: 3a04 3808 0000 0000 0600 0000 0544 6561  :.8..........Dea
+00004410: 6c73 0700 0000 1144 6561 6c73 5265 706f  ls.....DealsRepo
+00004420: 7274 5769 6467 6574 0103 0000 0020 0413  rtWidget..... ..
+00004430: 0440 0443 043f 043f 0438 0440 043e 0432  .@.C.?.?.8.@.>.2
+00004440: 0430 0442 044c 0020 043f 043e 003a 0800  .0.B.L. .?.>.:..
+00004450: 0000 0006 0000 0009 4772 6f75 7020 6279  ........Group by
+00004460: 3a07 0000 0011 4465 616c 7352 6570 6f72  :.....DealsRepor
+00004470: 7457 6964 6765 7401 0300 0000 1804 2104  tWidget.......!.
+00004480: 3e04 4504 4004 3004 3d04 3804 4204 4c00  >.E.@.0.=.8.B.L.
+00004490: 2e00 2e00 2e08 0000 0000 0600 0000 0753  ...............S
+000044a0: 6176 652e 2e2e 0700 0000 1144 6561 6c73  ave........Deals
+000044b0: 5265 706f 7274 5769 6467 6574 0103 0000  ReportWidget....
+000044c0: 000e 003c 041f 0443 0441 0442 043e 003e  ...<...C.A.B.>.>
+000044d0: 0800 0000 0006 0000 0006 3c4e 6f6e 653e  ..........<None>
+000044e0: 0700 0000 1144 6561 6c73 5265 706f 7274  .....DealsReport
+000044f0: 5769 6e64 6f77 0103 0000 001a 0426 0435  Window.......&.5
+00004500: 043d 043d 0430 044f 0020 0431 0443 043c  .=.=.0.O. .1.C.<
+00004510: 0430 0433 0430 0800 0000 0006 0000 0005  .0.3.0..........
+00004520: 4173 7365 7407 0000 0011 4465 616c 7352  Asset.....DealsR
+00004530: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
+00004540: 3004 2604 1100 2000 2d00 2004 1e04 4204  0.&... .-. ...B.
+00004550: 3a04 4004 4b04 4204 3804 3500 2000 2d00  :.@.K.B.8.5. .-.
+00004560: 2004 1704 3004 3a04 4004 4b04 4204 3804   ...0.:.@.K.B.8.
+00004570: 3508 0000 0000 0600 0000 1441 7373 6574  5..........Asset
+00004580: 202d 204f 7065 6e20 2d20 436c 6f73 6507   - Open - Close.
+00004590: 0000 0011 4465 616c 7352 6570 6f72 7457  ....DealsReportW
+000045a0: 696e 646f 7701 0300 0000 1004 1704 3004  indow.........0.
+000045b0: 3a04 4004 4b04 4204 3804 3508 0000 0000  :.@.K.B.8.5.....
+000045c0: 0600 0000 0543 6c6f 7365 0700 0000 1144  .....Close.....D
+000045d0: 6561 6c73 5265 706f 7274 5769 6e64 6f77  ealsReportWindow
+000045e0: 0103 0000 0026 0417 0430 043a 0440 044b  .....&...0.:.@.K
+000045f0: 0442 0438 0435 0020 002d 0020 041e 0442  .B.8.5. .-. ...B
+00004600: 043a 0440 044b 0442 0438 0435 0800 0000  .:.@.K.B.8.5....
+00004610: 0006 0000 000c 436c 6f73 6520 2d20 4f70  ......Close - Op
+00004620: 656e 0700 0000 1144 6561 6c73 5265 706f  en.....DealsRepo
+00004630: 7274 5769 6e64 6f77 0103 0000 000c 0421  rtWindow.......!
+00004640: 0434 0435 043b 043a 0438 0800 0000 0006  .4.5.;.:.8......
+00004650: 0000 0005 4465 616c 7307 0000 0011 4465  ....Deals.....De
+00004660: 616c 7352 6570 6f72 7457 696e 646f 7701  alsReportWindow.
+00004670: 0300 0000 2604 1e04 4204 3a04 4004 4b04  ....&...B.:.@.K.
+00004680: 4204 3804 3500 2000 2d00 2004 1704 3004  B.8.5. .-. ...0.
+00004690: 3a04 4004 4b04 4204 3804 3508 0000 0000  :.@.K.B.8.5.....
+000046a0: 0600 0000 0c4f 7065 6e20 2d20 436c 6f73  .....Open - Clos
+000046b0: 6507 0000 0011 4465 616c 7352 6570 6f72  e.....DealsRepor
+000046c0: 7457 696e 646f 7701 0300 0000 0a04 2104  tWindow.......!.
+000046d0: 4304 3c04 3c04 3008 0000 0000 0600 0000  C.<.<.0.........
+000046e0: 0641 6d6f 756e 7407 0000 000c 4465 7461  .Amount.....Deta
+000046f0: 696c 734d 6f64 656c 0103 0000 0012 041a  ilsModel........
+00004700: 0430 0442 0435 0433 043e 0440 0438 044f  .0.B.5.3.>.@.8.O
+00004710: 0800 0000 0006 0000 0008 4361 7465 676f  ..........Catego
+00004720: 7279 0700 0000 0c44 6574 6169 6c73 4d6f  ry.....DetailsMo
+00004730: 6465 6c01 0300 0000 1004 1e04 3f04 3804  del.........?.8.
+00004740: 4104 3004 3d04 3804 3508 0000 0000 0600  A.0.=.8.5.......
+00004750: 0000 044e 6f74 6507 0000 000c 4465 7461  ...Note.....Deta
+00004760: 696c 734d 6f64 656c 0103 0000 000a 041c  ilsModel........
+00004770: 0435 0442 043a 0430 0800 0000 0006 0000  .5.B.:.0........
+00004780: 0003 5461 6707 0000 000c 4465 7461 696c  ..Tag.....Detail
+00004790: 734d 6f64 656c 0103 0000 009e 041d 0435  sModel.........5
+000047a0: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+000047b0: 0020 043e 0431 0440 0430 0431 043e 0442  . .>.1.@.0.1.>.B
+000047c0: 0430 0442 044c 0020 0434 0438 0432 0438  .0.B.L. .4.8.2.8
+000047d0: 0434 0435 043d 0434 002c 0020 0442 002e  .4.5.=.4.,. .B..
+000047e0: 043a 002e 0020 043d 0435 0020 0443 043a  .:... .=.5. .C.:
+000047f0: 0430 0437 0430 043d 0020 0431 0430 043d  .0.7.0.=. .1.0.=
+00004800: 043a 0020 0434 043b 044f 0020 0438 043d  .:. .4.;.O. .8.=
+00004810: 0432 0435 0441 0442 0438 0446 0438 043e  .2.5.A.B.8.F.8.>
+00004820: 043d 043d 043e 0433 043e 0020 0441 0447  .=.=.>.3.>. .A.G
+00004830: 0451 0442 0430 003a 0020 0800 0000 0006  .Q.B.0.:. ......
+00004840: 0000 0041 4361 6e27 7420 7072 6f63 6573  ...ACan't proces
+00004850: 7320 6469 7669 6465 6e64 2061 7320 6261  s dividend as ba
+00004860: 6e6b 2069 736e 2774 2073 6574 2066 6f72  nk isn't set for
+00004870: 2069 6e76 6573 746d 656e 7420 6163 636f   investment acco
+00004880: 756e 743a 2007 0000 0008 4469 7669 6465  unt: .....Divide
+00004890: 6e64 0103 0000 005a 041d 0435 0020 0437  nd.....Z...5. .7
+000048a0: 0430 0434 0430 043d 0430 0020 0446 0435  .0.4.0.=.0. .F.5
+000048b0: 043d 0430 0020 0434 043b 044f 0020 0432  .=.0. .4.;.O. .2
+000048c0: 044b 043f 043b 0430 0442 044b 0020 0446  .K.?.;.0.B.K. .F
+000048d0: 0435 043d 043d 044b 043c 0438 0020 0431  .5.=.=.K.<.8. .1
+000048e0: 0443 043c 0430 0433 0430 043c 0438 003a  .C.<.0.3.0.<.8.:
+000048f0: 0020 0800 0000 0006 0000 002a 4e6f 2070  . .........*No p
+00004900: 7269 6365 2064 6174 6120 666f 7220 7374  rice data for st
+00004910: 6f63 6b20 6469 7669 6465 6e64 2f76 6573  ock dividend/ves
+00004920: 7469 6e67 3a20 0700 0000 0844 6976 6964  ting: .....Divid
+00004930: 656e 6401 0300 0000 7204 1d04 3504 4200  end.....r...5.B.
+00004940: 2004 3a04 3e04 4204 3804 4004 3e04 3204   .:.>.B.8.@.>.2.
+00004950: 3a04 3800 2004 3404 3b04 4f00 2004 3404  :.8. .4.;.O. .4.
+00004960: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
+00004970: 2004 3004 3a04 4604 3804 4f04 3c04 3800   .0.:.F.8.O.<.8.
+00004980: 2004 3804 3b04 3800 2004 3704 3004 4704   .8.;.8. .7.0.G.
+00004990: 3804 4104 3b04 3504 3d04 3804 4f00 2004  8.A.;.5.=.8.O. .
+000049a0: 3004 3a04 4604 3804 3900 2e08 0000 0000  0.:.F.8.9.......
+000049b0: 0600 0000 2d4e 6f20 7374 6f63 6b20 7175  ....-No stock qu
+000049c0: 6f74 6520 666f 7220 7374 6f63 6b20 6469  ote for stock di
+000049d0: 7669 6465 6e64 206f 7220 7665 7374 696e  vidend or vestin
+000049e0: 672e 0700 0000 0844 6976 6964 656e 6401  g......Dividend.
+000049f0: 0300 0000 b804 1d04 3504 3f04 3e04 3404  ........5.?.>.4.
+00004a00: 3404 3504 4004 3604 3804 3204 3004 3504  4.5.@.6.8.2.0.5.
+00004a10: 3c04 3e04 3500 2004 3404 3504 3904 4104  <.>.5. .4.5.9.A.
+00004a20: 4204 3204 3804 3500 3a00 2004 3404 3804  B.2.8.5.:. .4.8.
+00004a30: 3204 3804 3404 3504 3d04 3400 2004 3004  2.8.4.5.=.4. .0.
+00004a40: 3a04 4604 3804 4f04 3c04 3800 2004 3804  :.F.8.O.<.8. .8.
+00004a50: 3b04 3800 2004 3704 3004 4704 3804 4104  ;.8. .7.0.G.8.A.
+00004a60: 3b04 3504 3d04 3804 3500 2004 3004 3a04  ;.5.=.8.5. .0.:.
+00004a70: 4604 3804 3900 2004 3704 3004 3a04 4004  F.8.9. .7.0.:.@.
+00004a80: 4b04 3204 3004 3504 4200 2004 3a04 3e04  K.2.0.5.B. .:.>.
+00004a90: 4004 3e04 4204 3a04 4304 4e00 2004 3f04  @.>.B.:.C.N. .?.
+00004aa0: 3e04 3704 3804 4604 3804 4e00 2e08 0000  >.7.8.F.8.N.....
+00004ab0: 0000 0600 0000 434e 6f74 2073 7570 706f  ......CNot suppo
+00004ac0: 7274 6564 2061 6374 696f 6e3a 2073 746f  rted action: sto
+00004ad0: 636b 2064 6976 6964 656e 6420 6f72 2076  ck dividend or v
+00004ae0: 6573 7469 6e67 2063 6c6f 7365 7320 7368  esting closes sh
+00004af0: 6f72 7420 7472 6164 652e 0700 0000 0844  ort trade......D
+00004b00: 6976 6964 656e 6401 0300 0000 0e04 1d04  ividend.........
+00004b10: 3004 3b04 3e04 3300 3a00 2008 0000 0000  0.;.>.3.:. .....
+00004b20: 0600 0000 0554 6178 3a20 0700 0000 0844  .....Tax: .....D
+00004b30: 6976 6964 656e 6401 0300 0000 3e04 1d04  ividend.....>...
+00004b40: 3504 3f04 3e04 3404 3404 3504 4004 3604  5.?.>.4.4.5.@.6.
+00004b50: 3804 3204 3004 3504 3c04 4b04 3900 2004  8.2.0.5.<.K.9. .
+00004b60: 4204 3804 3f00 2004 3404 3804 3204 3804  B.8.?. .4.8.2.8.
+00004b70: 3404 3504 3d04 3404 3000 2e08 0000 0000  4.5.=.4.0.......
+00004b80: 0600 0000 1a55 6e73 7570 706f 7274 6564  .....Unsupported
+00004b90: 2064 6976 6964 656e 6420 7479 7065 2e07   dividend type..
+00004ba0: 0000 0008 4469 7669 6465 6e64 0103 0000  ....Dividend....
+00004bb0: 0002 2116 0800 0000 0006 0000 0001 2307  ..!...........#.
+00004bc0: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
+00004bd0: 6574 0103 0000 0008 0421 0447 0435 0442  et.......!.G.5.B
+00004be0: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
+00004bf0: 7407 0000 000e 4469 7669 6465 6e64 5769  t.....DividendWi
+00004c00: 6467 6574 0103 0000 0004 0426 0411 0800  dget.......&....
+00004c10: 0000 0006 0000 0005 4173 7365 7407 0000  ........Asset...
+00004c20: 000e 4469 7669 6465 6e64 5769 6467 6574  ..DividendWidget
+00004c30: 0103 0000 000a 041a 0443 043f 043e 043d  .........C.?.>.=
+00004c40: 0800 0000 0006 0000 000d 426f 6e64 2049  ..........Bond I
+00004c50: 6e74 6572 6573 7407 0000 000e 4469 7669  nterest.....Divi
+00004c60: 6465 6e64 5769 6467 6574 0103 0000 0014  dendWidget......
+00004c70: 0414 0430 0442 0430 002f 0412 0440 0435  ...0.B.0./...@.5
+00004c80: 043c 044f 0800 0000 0006 0000 0009 4461  .<.O..........Da
+00004c90: 7465 2f54 696d 6507 0000 000e 4469 7669  te/Time.....Divi
+00004ca0: 6465 6e64 5769 6467 6574 0103 0000 0010  dendWidget......
+00004cb0: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
+00004cc0: 0800 0000 0006 0000 0008 4469 7669 6465  ..........Divide
+00004cd0: 6e64 0700 0000 0e44 6976 6964 656e 6457  nd.....DividendW
+00004ce0: 6964 6765 7401 0300 0000 0e04 1e04 4204  idget.........B.
+00004cf0: 4104 3504 4704 3a04 3008 0000 0000 0600  A.5.G.:.0.......
+00004d00: 0000 0745 782d 4461 7465 0700 0000 0e44  ...Ex-Date.....D
+00004d10: 6976 6964 656e 6457 6964 6765 7401 0300  ividendWidget...
+00004d20: 0000 0600 4e00 2f00 4108 0000 0000 0600  ....N./.A.......
+00004d30: 0000 034e 2f41 0700 0000 0e44 6976 6964  ...N/A.....Divid
+00004d40: 656e 6457 6964 6765 7401 0300 0000 1a04  endWidget.......
+00004d50: 1d04 3504 4200 2004 3a04 3e04 4204 3804  ..5.B. .:.>.B.8.
+00004d60: 4004 3e04 3204 3a04 3808 0000 0000 0600  @.>.2.:.8.......
+00004d70: 0000 084e 6f20 7175 6f74 6507 0000 000e  ...No quote.....
+00004d80: 4469 7669 6465 6e64 5769 6467 6574 0103  DividendWidget..
+00004d90: 0000 0010 041e 043f 0438 0441 0430 043d  .......?.8.A.0.=
+00004da0: 0438 0435 0800 0000 0006 0000 0004 4e6f  .8.5..........No
+00004db0: 7465 0700 0000 0e44 6976 6964 656e 6457  te.....DividendW
+00004dc0: 6964 6765 7401 0300 0000 0804 2604 3504  idget.......&.5.
+00004dd0: 3d04 3008 0000 0000 0600 0000 0550 7269  =.0..........Pri
+00004de0: 6365 0700 0000 0e44 6976 6964 656e 6457  ce.....DividendW
+00004df0: 6964 6765 7401 0300 0000 2004 1404 3804  idget..... ...8.
+00004e00: 3204 3804 3404 3504 3d04 3400 2004 3004  2.8.4.5.=.4. .0.
+00004e10: 3a04 4604 3804 4f04 3c04 3808 0000 0000  :.F.8.O.<.8.....
+00004e20: 0600 0000 0e53 746f 636b 2044 6976 6964  .....Stock Divid
+00004e30: 656e 6407 0000 000e 4469 7669 6465 6e64  end.....Dividend
+00004e40: 5769 6467 6574 0103 0000 001c 041f 0435  Widget.........5
+00004e50: 0440 0435 0434 0430 0447 0430 0020 0430  .@.5.4.0.G.0. .0
+00004e60: 043a 0446 0438 0439 0800 0000 0006 0000  .:.F.8.9........
+00004e70: 000d 5374 6f63 6b20 5665 7374 696e 6707  ..Stock Vesting.
+00004e80: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
+00004e90: 6574 0103 0000 000a 041d 0430 043b 043e  et.........0.;.>
+00004ea0: 0433 0800 0000 0006 0000 0003 5461 7807  .3..........Tax.
+00004eb0: 0000 000e 4469 7669 6465 6e64 5769 6467  ....DividendWidg
+00004ec0: 6574 0103 0000 0006 0422 0438 043f 0800  et.......".8.?..
+00004ed0: 0000 0006 0000 0004 5479 7065 0700 0000  ........Type....
+00004ee0: 0e44 6976 6964 656e 6457 6964 6765 7401  .DividendWidget.
+00004ef0: 0300 0000 b204 1d04 4304 3604 3d04 3e00  ........C.6.=.>.
+00004f00: 2004 4304 4104 4204 3004 3d04 3e04 3204   .C.A.B.0.=.>.2.
+00004f10: 3804 4204 4c00 2004 3a04 3e04 4204 3804  8.B.L. .:.>.B.8.
+00004f20: 4004 3e04 3204 3a04 4300 2004 3104 4304  @.>.2.:.C. .1.C.
+00004f30: 3c04 3004 3304 3800 2004 3404 3b04 4f00  <.0.3.8. .4.;.O.
+00004f40: 2004 1404 3004 4204 4b00 2f04 1204 4004   ...0.B.K./...@.
+00004f50: 3504 3c04 3504 3d04 3800 2004 3404 3804  5.<.5.=.8. .4.8.
+00004f60: 3204 3804 3404 3504 3d04 3404 3000 2004  2.8.4.5.=.4.0. .
+00004f70: 4704 3504 4004 3504 3700 2004 3c04 3504  G.5.@.5.7. .<.5.
+00004f80: 3d04 4e00 2004 1404 3004 3d04 3d04 4b04  =.N. ...0.=.=.K.
+00004f90: 3500 2d00 3e04 1a04 3e04 4204 3804 4004  5.-.>...>.B.8.@.
+00004fa0: 3e04 3204 3a04 3808 0000 0000 0600 0000  >.2.:.8.........
+00004fb0: 4859 6f75 2073 686f 756c 6420 7365 7420  HYou should set 
+00004fc0: 7175 6f74 6520 7669 6120 4461 7461 2d3e  quote via Data->
+00004fd0: 5175 6f74 6573 206d 656e 7520 666f 7220  Quotes menu for 
+00004fe0: 4461 7465 2f54 696d 6520 6f66 2074 6865  Date/Time of the
+00004ff0: 2064 6976 6964 656e 6407 0000 000e 4469   dividend.....Di
+00005000: 7669 6465 6e64 5769 6467 6574 0103 0000  videndWidget....
+00005010: 0014 043d 0435 0438 0437 0432 0435 0441  ...=.5.8.7.2.5.A
+00005020: 0442 043d 043e 0800 0000 0006 0000 0007  .B.=.>..........
+00005030: 756e 6b6e 6f77 6e07 0000 000e 4469 7669  unknown.....Divi
+00005040: 6465 6e64 5769 6467 6574 0103 0000 0010  dendWidget......
+00005050: 0421 0432 043e 0439 0441 0442 0432 043e  .!.2.>.9.A.B.2.>
+00005060: 0800 0000 0006 0000 0008 5072 6f70 6572  ..........Proper
+00005070: 7479 0700 0000 0e45 7874 7261 4461 7461  ty.....ExtraData
+00005080: 4d6f 6465 6c01 0300 0000 1004 1704 3d04  Model.........=.
+00005090: 3004 4704 3504 3d04 3804 3508 0000 0000  0.G.5.=.8.5.....
+000050a0: 0600 0000 0556 616c 7565 0700 0000 0e45  .....Value.....E
+000050b0: 7874 7261 4461 7461 4d6f 6465 6c01 0300  xtraDataModel...
+000050c0: 0000 1a04 2604 3504 3d04 3d04 3004 4f00  ....&.5.=.=.0.O.
+000050d0: 2004 3104 4304 3c04 3004 3304 3008 0000   .1.C.<.0.3.0...
+000050e0: 0000 0600 0000 0a41 7373 6574 204e 616d  .......Asset Nam
+000050f0: 6507 0000 000d 486f 6c64 696e 6773 4d6f  e.....HoldingsMo
+00005100: 6465 6c01 0300 0000 1c04 1204 3004 3b04  del.........0.;.
+00005110: 4e04 4204 3000 2f04 2104 4704 5104 4200  N.B.0./.!.G.Q.B.
+00005120: 2f04 2604 1108 0000 0000 0600 0000 1643  /.&............C
+00005130: 7572 7265 6e63 792f 4163 636f 756e 742f  urrency/Account/
+00005140: 4173 7365 7407 0000 000d 486f 6c64 696e  Asset.....Holdin
+00005150: 6773 4d6f 6465 6c01 0300 0000 0a04 2d04  gsModel.......-.
+00005160: 3a04 4104 3f00 3a08 0000 0000 0600 0000  :.A.?.:.........
+00005170: 0445 7870 3a07 0000 000d 486f 6c64 696e  .Exp:.....Holdin
+00005180: 6773 4d6f 6465 6c01 0300 0000 1404 2604  gsModel.......&.
+00005190: 3504 3d04 3000 2004 3704 3004 3a04 4000  5.=.0. .7.0.:.@.
+000051a0: 2e08 0000 0000 0600 0000 044c 6173 7407  ...........Last.
+000051b0: 0000 000d 486f 6c64 696e 6773 4d6f 6465  ....HoldingsMode
+000051c0: 6c01 0300 0000 3404 1404 3004 4204 3000  l.....4...0.B.0.
+000051d0: 2004 3f04 3e04 4104 3b04 3504 3404 3d04   .?.>.A.;.5.4.=.
+000051e0: 3504 3900 2004 3a04 3e04 4204 3804 4004  5.9. .:.>.B.8.@.
+000051f0: 3e04 3204 3a04 3800 3a00 2008 0000 0000  >.2.:.8.:. .....
+00005200: 0600 0000 114c 6173 7420 7175 6f74 6520  .....Last quote 
+00005210: 6461 7465 3a20 0700 0000 0d48 6f6c 6469  date: .....Holdi
+00005220: 6e67 734d 6f64 656c 0103 0000 000c 0414  ngsModel........
+00005230: 0435 043d 044c 0433 0438 0800 0000 0006  .5.=.L.3.8......
+00005240: 0000 0005 4d6f 6e65 7907 0000 000d 486f  ....Money.....Ho
+00005250: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
+00005260: 0600 4e00 2f00 4108 0000 0000 0600 0000  ..N./.A.........
+00005270: 034e 2f41 0700 0000 0d48 6f6c 6469 6e67  .N/A.....Holding
+00005280: 734d 6f64 656c 0103 0000 0014 0426 0435  sModel.......&.5
+00005290: 043d 0430 0020 043e 0442 043a 0440 002e  .=.0. .>.B.:.@..
+000052a0: 0800 0000 0006 0000 0004 4f70 656e 0700  ..........Open..
+000052b0: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
+000052c0: 0103 0000 0006 041f 0438 0423 0800 0000  .........8.#....
+000052d0: 0006 0000 0003 502f 4c07 0000 000d 486f  ......P/L.....Ho
+000052e0: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
+000052f0: 0c04 1f04 3804 2300 2c00 2000 2508 0000  ....8.#.,. .%...
+00005300: 0000 0600 0000 0650 2f4c 2c20 2507 0000  .......P/L, %...
+00005310: 000d 486f 6c64 696e 6773 4d6f 6465 6c01  ..HoldingsModel.
+00005320: 0300 0000 0c04 1a04 3e04 3b00 2d04 3204  ........>.;.-.2.
+00005330: 3e08 0000 0000 0600 0000 0351 7479 0700  >..........Qty..
+00005340: 0000 0d48 6f6c 6469 6e67 734d 6f64 656c  ...HoldingsModel
+00005350: 0103 0000 000e 0414 043e 043b 044f 002c  .........>.;.O.,
+00005360: 0020 0025 0800 0000 0006 0000 0008 5368  . .%..........Sh
+00005370: 6172 652c 2025 0700 0000 0d48 6f6c 6469  are, %.....Holdi
+00005380: 6e67 734d 6f64 656c 0103 0000 000c 041e  ngsModel........
+00005390: 0446 0435 043d 043a 0430 0800 0000 0006  .F.5.=.:.0......
+000053a0: 0000 0005 5661 6c75 6507 0000 000d 486f  ....Value.....Ho
+000053b0: 6c64 696e 6773 4d6f 6465 6c01 0300 0000  ldingsModel.....
+000053c0: 1004 1e04 4604 3504 3d04 3a04 3000 2c00  ....F.5.=.:.0.,.
+000053d0: 2008 0000 0000 0600 0000 0756 616c 7565   ..........Value
+000053e0: 2c20 0700 0000 0d48 6f6c 6469 6e67 734d  , .....HoldingsM
+000053f0: 6f64 656c 0103 0000 0016 041f 043e 0440  odel.........>.@
+00005400: 0442 0444 0435 043b 044c 0020 0426 0411  .B.D.5.;.L. .&..
+00005410: 0800 0000 0006 0000 0008 486f 6c64 696e  ..........Holdin
+00005420: 6773 0700 0000 0e48 6f6c 6469 6e67 7352  gs.....HoldingsR
+00005430: 6570 6f72 7401 0300 0000 0404 2604 1108  eport.......&...
+00005440: 0000 0000 0600 0000 0541 7373 6574 0700  .........Asset..
+00005450: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
+00005460: 7457 696e 646f 7701 0300 0000 1804 2104  tWindow.......!.
+00005470: 3204 3504 4004 3d04 4304 4204 4c00 2004  2.5.@.=.C.B.L. .
+00005480: 1204 4104 3508 0000 0000 0600 0000 0c43  ..A.5..........C
+00005490: 6f6c 6c61 7073 6520 416c 6c07 0000 0014  ollapse All.....
+000054a0: 486f 6c64 696e 6773 5265 706f 7274 5769  HoldingsReportWi
+000054b0: 6e64 6f77 0103 0000 000c 0421 0442 0440  ndow.......!.B.@
+000054c0: 0430 043d 0430 0800 0000 0006 0000 0007  .0.=.0..........
+000054d0: 436f 756e 7472 7907 0000 0014 486f 6c64  Country.....Hold
+000054e0: 696e 6773 5265 706f 7274 5769 6e64 6f77  ingsReportWindow
+000054f0: 0103 0000 001a 0412 0430 043b 044e 0442  .........0.;.N.B
+00005500: 0430 0020 002d 0020 0421 0447 0451 0442  .0. .-. .!.G.Q.B
+00005510: 0800 0000 0006 0000 0012 4375 7272 656e  ..........Curren
+00005520: 6379 202d 2041 6363 6f75 6e74 0700 0000  cy - Account....
+00005530: 1448 6f6c 6469 6e67 7352 6570 6f72 7457  .HoldingsReportW
+00005540: 696e 646f 7701 0300 0000 1a04 1e04 4604  indow.........F.
+00005550: 3504 3d04 3804 4204 4c00 2004 3d04 3004  5.=.8.B.L. .=.0.
+00005560: 3b04 3e04 3308 0000 0000 0600 0000 0c45  ;.>.3..........E
+00005570: 7374 696d 6174 6520 7461 7807 0000 0014  stimate tax.....
+00005580: 486f 6c64 696e 6773 5265 706f 7274 5769  HoldingsReportWi
+00005590: 6e64 6f77 0103 0000 0018 0420 0430 0441  ndow....... .0.A
+000055a0: 043a 0440 044b 0442 044c 0020 0412 0441  .:.@.K.B.L. ...A
+000055b0: 0435 0800 0000 0006 0000 000a 4578 7061  .5..........Expa
+000055c0: 6e64 2041 6c6c 0700 0000 1448 6f6c 6469  nd All.....Holdi
+000055d0: 6e67 7352 6570 6f72 7457 696e 646f 7701  ngsReportWindow.
+000055e0: 0300 0000 1604 1f04 3e04 4004 4204 4404  ........>.@.B.D.
+000055f0: 3504 3b04 4c00 2004 2604 1108 0000 0000  5.;.L. .&.......
+00005600: 0600 0000 0848 6f6c 6469 6e67 7307 0000  .....Holdings...
+00005610: 0014 486f 6c64 696e 6773 5265 706f 7274  ..HoldingsReport
+00005620: 5769 6e64 6f77 0103 0000 0014 041f 043e  Window.........>
+00005630: 0440 0442 0443 0433 0430 043b 0438 044f  .@.B.C.3.0.;.8.O
+00005640: 0800 0000 0006 0000 0008 506f 7274 7567  ..........Portug
+00005650: 616c 0700 0000 1448 6f6c 6469 6e67 7352  al.....HoldingsR
+00005660: 6570 6f72 7457 696e 646f 7701 0300 0000  eportWindow.....
+00005670: 0c04 2004 3e04 4104 4104 3804 4f08 0000  .. .>.A.A.8.O...
+00005680: 0000 0600 0000 0652 7573 7369 6107 0000  .......Russia...
+00005690: 0014 486f 6c64 696e 6773 5265 706f 7274  ..HoldingsReport
+000056a0: 5769 6e64 6f77 0103 0000 0028 041f 043e  Window.....(...>
+000056b0: 043a 0430 0437 0430 0442 044c 0020 0433  .:.0.7.0.B.L. .3
+000056c0: 0440 0430 0444 0438 043a 0020 0446 0435  .@.0.D.8.:. .F.5
+000056d0: 043d 044b 0800 0000 0006 0000 0010 5368  .=.K..........Sh
+000056e0: 6f77 2050 7269 6365 2043 6861 7274 0700  ow Price Chart..
+000056f0: 0000 1448 6f6c 6469 6e67 7352 6570 6f72  ...HoldingsRepor
+00005700: 7457 696e 646f 7701 0300 0000 0604 2204  tWindow.......".
+00005710: 4d04 3308 0000 0000 0600 0000 0354 6167  M.3..........Tag
+00005720: 0700 0000 1448 6f6c 6469 6e67 7352 6570  .....HoldingsRep
+00005730: 6f72 7457 696e 646f 7701 0300 0000 2204  ortWindow.....".
+00005740: 1204 3004 3b04 4e04 4204 3000 2004 3f04  ..0.;.N.B.0. .?.
+00005750: 3504 4004 3504 4104 4704 5104 4204 3000  5.@.5.A.G.Q.B.0.
+00005760: 3a08 0000 0000 0600 0000 1043 6f6d 6d6f  :..........Commo
+00005770: 6e20 6375 7272 656e 6379 3a07 0000 000e  n currency:.....
+00005780: 486f 6c64 696e 6773 5769 6467 6574 0103  HoldingsWidget..
+00005790: 0000 0020 0413 0440 0443 043f 043f 0438  ... ...@.C.?.?.8
+000057a0: 0440 043e 0432 0430 0442 044c 0020 043f  .@.>.2.0.B.L. .?
+000057b0: 043e 003a 0800 0000 0006 0000 0009 4772  .>.:..........Gr
+000057c0: 6f75 7020 6279 3a07 0000 000e 486f 6c64  oup by:.....Hold
+000057d0: 696e 6773 5769 6467 6574 0103 0000 0016  ingsWidget......
+000057e0: 041f 043e 0440 0442 0444 0435 043b 044c  ...>.@.B.D.5.;.L
+000057f0: 0020 0426 0411 0800 0000 0006 0000 0008  . .&............
+00005800: 486f 6c64 696e 6773 0700 0000 0e48 6f6c  Holdings.....Hol
+00005810: 6469 6e67 7357 6964 6765 7401 0300 0000  dingsWidget.....
+00005820: 1804 2104 3e04 4504 4004 3004 3d04 3804  ..!.>.E.@.0.=.8.
+00005830: 4204 4c00 2e00 2e00 2e08 0000 0000 0600  B.L.............
+00005840: 0000 0753 6176 652e 2e2e 0700 0000 0e48  ...Save........H
+00005850: 6f6c 6469 6e67 7357 6964 6765 7401 0300  oldingsWidget...
+00005860: 0000 1400 6400 6400 2f00 4d00 4d00 2f00  ....d.d./.M.M./.
+00005870: 7900 7900 7900 7908 0000 0000 0600 0000  y.y.y.y.........
+00005880: 0a64 642f 4d4d 2f79 7979 7907 0000 000e  .dd/MM/yyyy.....
+00005890: 486f 6c64 696e 6773 5769 6467 6574 0103  HoldingsWidget..
+000058a0: 0000 0034 0422 0438 043f 0020 0426 0411  ...4.".8.?. .&..
+000058b0: 0020 043d 0435 0020 043f 043e 0434 0434  . .=.5. .?.>.4.4
+000058c0: 0435 0440 0436 0438 0432 0430 0435 0442  .5.@.6.8.2.0.5.B
+000058d0: 0441 044f 003a 0020 0800 0000 0006 0000  .A.O.:. ........
+000058e0: 001c 4173 7365 7420 7479 7065 2069 736e  ..Asset type isn
+000058f0: 2774 2073 7570 706f 7274 6564 3a20 0700  't supported: ..
+00005900: 0000 0449 424b 5201 0300 0000 5404 1a04  ...IBKR.....T...
+00005910: 3e04 4004 3f04 3e04 4004 3004 4204 3804  >.@.?.>.@.0.B.8.
+00005920: 3204 3d04 3e04 3500 2004 3404 3504 3904  2.=.>.5. .4.5.9.
+00005930: 4104 4204 3204 3804 3500 2004 3d04 3500  A.B.2.8.5. .=.5.
+00005940: 2004 3f04 3e04 3404 3404 3504 4004 3604   .?.>.4.4.5.@.6.
+00005950: 3804 3204 3004 3504 4204 4104 4f00 3a00  8.2.0.5.B.A.O.:.
+00005960: 2008 0000 0000 0600 0000 2243 6f72 706f   ........."Corpo
+00005970: 7261 7465 2061 6374 696f 6e20 6973 6e27  rate action isn'
+00005980: 7420 7375 7070 6f72 7465 643a 2007 0000  t supported: ...
+00005990: 0004 4942 4b52 0103 0000 0046 041d 0435  ..IBKR.....F...5
+000059a0: 043e 0434 043d 043e 0437 043d 0430 0447  .>.4.=.>.7.=.0.G
+000059b0: 043d 043e 0435 0020 0441 043e 0432 043f  .=.>.5. .A.>.2.?
+000059c0: 0430 0434 0435 043d 0438 0435 0020 0441  .0.4.5.=.8.5. .A
+000059d0: 0447 0451 0442 0430 0020 0434 043b 044f  .G.Q.B.0. .4.;.O
+000059e0: 0020 0800 0000 0006 0000 001b 4d75 6c74  . ..........Mult
+000059f0: 6970 6c65 2061 6363 6f75 6e74 206d 6174  iple account mat
+00005a00: 6368 2066 6f72 2007 0000 0004 4942 4b52  ch for .....IBKR
+00005a10: 0103 0000 0068 004a 0053 004f 004e 0020  .....h.J.S.O.N. 
+00005a20: 0442 044d 0433 0020 0027 0064 006f 0063  .B.M.3. .'.d.o.c
+00005a30: 0075 006d 0065 006e 0074 0027 0020 043e  .u.m.e.n.t.'. .>
+00005a40: 0442 0441 0443 0442 0441 0442 0432 0443  .B.A.C.B.A.B.2.C
+00005a50: 0435 0442 0020 0432 043d 0443 0442 0440  .5.B. .2.=.C.B.@
+00005a60: 0438 0020 0442 044d 0433 0430 0020 0027  .8. .B.M.3.0. .'
+00005a70: 0074 0069 0063 006b 0065 0074 0027 0800  .t.i.c.k.e.t.'..
+00005a80: 0000 0006 0000 002a 4361 6e27 7420 6669  .......*Can't fi
+00005a90: 6e64 2027 646f 6375 6d65 6e74 2720 7461  nd 'document' ta
+00005aa0: 6720 696e 206a 736f 6e20 2774 6963 6b65  g in json 'ticke
+00005ab0: 7427 0700 0000 1049 6d70 6f72 7453 6c69  t'.....ImportSli
+00005ac0: 7044 6961 6c6f 6701 0300 0000 7200 4a00  pDialog.....r.J.
+00005ad0: 5300 4f00 4e00 2004 4204 4d04 3300 2000  S.O.N. .B.M.3. .
+00005ae0: 2700 6f00 7000 6500 7200 6100 7400 6900  '.o.p.e.r.a.t.i.
+00005af0: 6f00 6e00 5400 7900 7000 6500 2700 2004  o.n.T.y.p.e.'. .
+00005b00: 3e04 4204 4104 4304 4204 4104 4204 3204  >.B.A.C.B.A.B.2.
+00005b10: 4304 3504 4200 2004 3204 3d04 4304 4204  C.5.B. .2.=.C.B.
+00005b20: 4004 3800 2004 4204 4d04 3304 3000 2000  @.8. .B.M.3.0. .
+00005b30: 2700 7400 6900 6300 6b00 6500 7400 2708  '.t.i.c.k.e.t.'.
+00005b40: 0000 0000 0600 0000 2f43 616e 2774 2066  ......../Can't f
+00005b50: 696e 6420 276f 7065 7261 7469 6f6e 5479  ind 'operationTy
+00005b60: 7065 2720 7461 6720 696e 206a 736f 6e20  pe' tag in json 
+00005b70: 2774 6963 6b65 7427 0700 0000 1049 6d70  'ticket'.....Imp
+00005b80: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
+00005b90: 0000 6a00 4a00 5300 4f00 4e00 2004 4204  ..j.J.S.O.N. .B.
+00005ba0: 4d04 3300 2000 2700 7200 6500 6300 6500  M.3. .'.r.e.c.e.
+00005bb0: 6900 7000 7400 2700 2004 3e04 4204 4104  i.p.t.'. .>.B.A.
+00005bc0: 4304 4204 4104 4204 3204 4304 3504 4200  C.B.A.B.2.C.5.B.
+00005bd0: 2004 3204 3d04 4304 4204 4004 3800 2004   .2.=.C.B.@.8. .
+00005be0: 4204 4d04 3304 3000 2000 2700 6400 6f00  B.M.3.0. .'.d.o.
+00005bf0: 6300 7500 6d00 6500 6e00 7400 2708 0000  c.u.m.e.n.t.'...
+00005c00: 0000 0600 0000 2b43 616e 2774 2066 696e  ......+Can't fin
+00005c10: 6420 2772 6563 6569 7074 2720 7461 6720  d 'receipt' tag 
+00005c20: 696e 206a 736f 6e20 2764 6f63 756d 656e  in json 'documen
+00005c30: 7427 0700 0000 1049 6d70 6f72 7453 6c69  t'.....ImportSli
+00005c40: 7044 6961 6c6f 6701 0300 0000 5e04 1a04  pDialog.....^...
+00005c50: 3004 4204 3504 3304 3e04 4004 3804 3800  0.B.5.3.>.@.8.8.
+00005c60: 2004 3d04 3500 2004 4004 3004 4104 3f04   .=.5. .@.0.A.?.
+00005c70: 3e04 3704 3d04 3004 3d04 4b00 3a00 2000  >.7.=.0.=.K.:. .
+00005c80: 5400 6500 6e00 7300 6f00 7200 6c00 6f00  T.e.n.s.o.r.l.o.
+00005c90: 7700 2004 3d04 3500 2004 3e04 3104 3d04  w. .=.5. .>.1.=.
+00005ca0: 3004 4004 4304 3604 3504 3d08 0000 0000  0.@.C.6.5.=.....
+00005cb0: 0600 0000 3643 6174 6567 6f72 6965 7320  ....6Categories 
+00005cc0: 6172 6520 6e6f 7420 7265 636f 676e 697a  are not recogniz
+00005cd0: 6564 3a20 5465 6e73 6f72 666c 6f77 2069  ed: Tensorflow i
+00005ce0: 7320 6e6f 7420 666f 756e 6407 0000 0010  s not found.....
+00005cf0: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
+00005d00: 0103 0000 004a 041f 0440 0435 0432 044b  .....J...@.5.2.K
+00005d10: 0448 0435 043d 043e 0020 043c 0430 043a  .H.5.=.>. .<.0.:
+00005d20: 0441 0438 043c 0430 043b 044c 043d 043e  .A.8.<.0.;.L.=.>
+00005d30: 0435 0020 0447 0438 0441 043b 043e 0020  .5. .G.8.A.;.>. 
+00005d40: 043f 043e 043f 044b 0442 043e 043a 002e  .?.>.?.K.B.>.:..
+00005d50: 0800 0000 0006 0000 0019 4d61 7820 7265  ..........Max re
+00005d60: 7472 7920 636f 756e 7420 6578 6365 6564  try count exceed
+00005d70: 6564 2e07 0000 0010 496d 706f 7274 536c  ed......ImportSl
+00005d80: 6970 4469 616c 6f67 0103 0000 0046 0051  ipDialog.....F.Q
+00005d90: 0052 0020 043a 043e 0434 0020 043d 0435  .R. .:.>.4. .=.5
+00005da0: 0020 043e 0431 043d 0430 0440 0443 0436  . .>.1.=.0.@.C.6
+00005db0: 0435 043d 0020 0432 0020 0431 0443 0444  .5.=. .2. .1.C.D
+00005dc0: 0435 0440 0435 0020 043e 0431 043c 0435  .5.@.5. .>.1.<.5
+00005dd0: 043d 0430 0800 0000 0006 0000 001e 4e6f  .=.0..........No
+00005de0: 2051 5220 636f 6465 7320 666f 756e 6420   QR codes found 
+00005df0: 696e 2063 6c69 7062 6f61 7264 0700 0000  in clipboard....
+00005e00: 1049 6d70 6f72 7453 6c69 7044 6961 6c6f  .ImportSlipDialo
+00005e10: 6701 0300 0000 3600 5100 5200 2d04 3a04  g.....6.Q.R.-.:.
+00005e20: 3e04 3400 2004 3200 2004 4404 3004 3904  >.4. .2. .D.0.9.
+00005e30: 3b04 3500 2004 3d04 3500 2004 3e04 3104  ;.5. .=.5. .>.1.
+00005e40: 3d04 3004 4004 4304 3604 3504 3d08 0000  =.0.@.C.6.5.=...
+00005e50: 0000 0600 0000 1e4e 6f20 5152 2063 6f64  .......No QR cod
+00005e60: 6573 2077 6572 6520 666f 756e 6420 696e  es were found in
+00005e70: 2066 696c 6507 0000 0010 496d 706f 7274   file.....Import
+00005e80: 536c 6970 4469 616c 6f67 0103 0000 0072  SlipDialog.....r
+00005e90: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00005ea0: 043d 043e 0020 0434 043e 0431 0430 0432  .=.>. .4.>.1.0.2
+00005eb0: 0438 0442 044c 0020 0447 0435 043a 003a  .8.B.L. .G.5.:.:
+00005ec0: 0020 043d 0435 0020 0443 043a 0430 0437  . .=.5. .C.:.0.7
+00005ed0: 0430 043d 0020 043a 043e 043d 0442 0440  .0.=. .:.>.=.B.@
+00005ee0: 0430 0433 0435 043d 0442 0020 0434 043b  .0.3.5.=.B. .4.;
+00005ef0: 044f 0020 0438 043c 043f 043e 0440 0442  .O. .8.<.?.>.@.B
+00005f00: 0430 0800 0000 0006 0000 0041 4e6f 7420  .0.........ANot 
+00005f10: 706f 7373 6962 6c65 2074 6f20 696d 706f  possible to impo
+00005f20: 7274 2073 6c69 703a 2063 616e 2774 2069  rt slip: can't i
+00005f30: 6d70 6f72 743a 206e 6f20 7065 6572 2073  mport: no peer s
+00005f40: 6574 2066 6f72 2069 6d70 6f72 7407 0000  et for import...
+00005f50: 0010 496d 706f 7274 536c 6970 4469 616c  ..ImportSlipDial
+00005f60: 6f67 0103 0000 0066 041d 0435 0432 043e  og.....f...5.2.>
+00005f70: 0437 043c 043e 0436 043d 043e 0020 0434  .7.<.>.6.=.>. .4
+00005f80: 043e 0431 0430 0432 0438 0442 044c 0020  .>.1.0.2.8.B.L. 
+00005f90: 0447 0435 043a 003a 0020 043d 0435 0020  .G.5.:.:. .=.5. 
+00005fa0: 0443 043a 0430 0437 0430 043d 0020 0441  .C.:.0.7.0.=. .A
+00005fb0: 0447 0435 0442 0020 0434 043b 044f 0020  .G.5.B. .4.;.O. 
+00005fc0: 0438 043c 043f 043e 0440 0442 0430 0800  .8.<.?.>.@.B.0..
+00005fd0: 0000 0006 0000 0036 4e6f 7420 706f 7373  .......6Not poss
+00005fe0: 6962 6c65 2074 6f20 696d 706f 7274 2073  ible to import s
+00005ff0: 6c69 703a 206e 6f20 6163 636f 756e 7420  lip: no account 
+00006000: 7365 7420 666f 7220 696d 706f 7274 0700  set for import..
+00006010: 0000 1049 6d70 6f72 7453 6c69 7044 6961  ...ImportSlipDia
+00006020: 6c6f 6701 0300 0000 7804 1d04 3504 3204  log.....x...5.2.
+00006030: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+00006040: 3404 3e04 3104 3004 3204 3804 4204 4c00  4.>.1.0.2.8.B.L.
+00006050: 2004 4704 3504 3a00 3a00 2004 3a04 3004   .G.5.:.:. .:.0.
+00006060: 4204 3504 3304 3e04 4004 3804 3800 2004  B.5.3.>.@.8.8. .
+00006070: 4304 3a04 3004 3704 3004 3d04 4b00 2004  C.:.0.7.0.=.K. .
+00006080: 3d04 3500 2004 3404 3b04 4f00 2004 3204  =.5. .4.;.O. .2.
+00006090: 4104 3504 4500 2004 4104 4204 4004 3e04  A.5.E. .A.B.@.>.
+000060a0: 3a08 0000 0000 0600 0000 384e 6f74 2070  :.........8Not p
+000060b0: 6f73 7369 626c 6520 746f 2069 6d70 6f72  ossible to impor
+000060c0: 7420 736c 6970 3a20 736f 6d65 2063 6174  t slip: some cat
+000060d0: 6567 6f72 6965 7320 6172 6520 6e6f 7420  egories are not 
+000060e0: 7365 7407 0000 0010 496d 706f 7274 536c  set.....ImportSl
+000060f0: 6970 4469 616c 6f67 0103 0000 0054 041d  ipDialog.....T..
+00006100: 0435 0432 043e 0437 043c 043e 0436 043d  .5.2.>.7.<.>.6.=
+00006110: 043e 0020 0440 0430 0441 043f 043e 0437  .>. .@.0.A.?.>.7
+00006120: 043d 0430 0442 044c 0020 043f 0440 043e  .=.0.B.L. .?.@.>
+00006130: 0447 0438 0442 0430 043d 043d 044b 0439  .G.8.B.0.=.=.K.9
+00006140: 0020 0051 0052 002d 043a 043e 0434 003a  . .Q.R.-.:.>.4.:
+00006150: 0020 0800 0000 0006 0000 002b 5152 2061  . .........+QR a
+00006160: 7661 696c 6162 6c65 2062 7574 2070 6174  vailable but pat
+00006170: 7465 726e 2069 736e 2774 2072 6563 6f67  tern isn't recog
+00006180: 6e69 7a65 643a 2007 0000 0010 496d 706f  nized: .....Impo
+00006190: 7274 536c 6970 4469 616c 6f67 0103 0000  rtSlipDialog....
+000061a0: 0008 0051 0052 003a 0020 0800 0000 0006  ...Q.R.:. ......
+000061b0: 0000 0004 5152 3a20 0700 0000 1049 6d70  ....QR: .....Imp
+000061c0: 6f72 7453 6c69 7044 6961 6c6f 6701 0300  ortSlipDialog...
+000061d0: 0000 3004 1204 4b04 3104 3504 4004 3804  ..0...K.1.5.@.8.
+000061e0: 4204 3500 2004 4404 3004 3904 3b00 2004  B.5. .D.0.9.;. .
+000061f0: 4100 2000 5100 5200 2d04 3a04 3e04 3404  A. .Q.R.-.:.>.4.
+00006200: 3e04 3c08 0000 0000 0600 0000 1853 656c  >.<..........Sel
+00006210: 6563 7420 6669 6c65 2077 6974 6820 5152  ect file with QR
+00006220: 2063 6f64 6507 0000 0010 496d 706f 7274   code.....Import
+00006230: 536c 6970 4469 616c 6f67 0103 0000 0042  SlipDialog.....B
+00006240: 0412 044b 0431 0435 0440 0438 0442 0435  ...K.1.5.@.8.B.5
+00006250: 0020 0444 0430 0439 043b 0020 0441 0020  . .D.0.9.;. .A. 
+00006260: 004a 0053 004f 004e 002d 0434 0430 043d  .J.S.O.N.-.4.0.=
+00006270: 043d 044b 043c 0438 0020 0447 0435 043a  .=.K.<.8. .G.5.:
+00006280: 0430 0800 0000 0006 0000 001f 5365 6c65  .0..........Sele
+00006290: 6374 2066 696c 6520 7769 7468 2073 6c69  ct file with sli
+000062a0: 7020 4a53 4f4e 2064 6174 6107 0000 0010  p JSON data.....
+000062b0: 496d 706f 7274 536c 6970 4469 616c 6f67  ImportSlipDialog
+000062c0: 0103 0000 0032 041d 0435 0438 0437 0432  .....2...5.8.7.2
+000062d0: 0435 0441 0442 043d 044b 0439 0020 0442  .5.A.B.=.K.9. .B
+000062e0: 0438 043f 0020 043e 043f 0435 0440 0430  .8.?. .>.?.5.@.0
+000062f0: 0446 0438 0438 0020 0800 0000 0006 0000  .F.8.8. ........
+00006300: 0017 556e 6b6e 6f77 6e20 6f70 6572 6174  ..Unknown operat
+00006310: 696f 6e20 7479 7065 2007 0000 0010 496d  ion type .....Im
+00006320: 706f 7274 536c 6970 4469 616c 6f67 0103  portSlipDialog..
+00006330: 0000 0006 0020 279c 0020 0800 0000 0006  ..... '.. ......
+00006340: 0000 0005 20e2 9e9c 2007 0000 000d 496d  .... ... .....Im
+00006350: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
+00006360: 0a04 2104 4704 3504 4200 3a08 0000 0000  ..!.G.5.B.:.....
+00006370: 0600 0000 0841 6363 6f75 6e74 3a07 0000  .....Account:...
+00006380: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+00006390: 0300 0000 1004 1404 3e04 3104 3004 3204  ........>.1.0.2.
+000063a0: 3804 4204 4c08 0000 0000 0600 0000 0341  8.B.L..........A
+000063b0: 6464 0700 0000 0d49 6d70 6f72 7453 6c69  dd.....ImportSli
+000063c0: 7044 6c67 0103 0000 000c 0421 0443 043c  pDlg.......!.C.<
+000063d0: 043c 0430 003a 0800 0000 0006 0000 0007  .<.0.:..........
+000063e0: 416d 6f75 6e74 3a07 0000 000d 496d 706f  Amount:.....Impo
+000063f0: 7274 536c 6970 446c 6701 0300 0000 3204  rtSlipDlg.....2.
+00006400: 1004 3204 4204 3e00 2d04 3d04 3004 3704  ..2.B.>.-.=.0.7.
+00006410: 3d04 3004 4704 3504 3d04 3804 3500 2004  =.0.G.5.=.8.5. .
+00006420: 3a04 3004 4204 3504 3304 3e04 4004 3804  :.0.B.5.3.>.@.8.
+00006430: 3908 0000 0000 0600 0000 1641 7574 6f2d  9..........Auto-
+00006440: 6173 7369 676e 2063 6174 6567 6f72 6965  assign categorie
+00006450: 7307 0000 000d 496d 706f 7274 536c 6970  s.....ImportSlip
+00006460: 446c 6701 0300 0000 0c04 1a04 3004 3c04  Dlg.........0.<.
+00006470: 3504 4004 3008 0000 0000 0600 0000 0643  5.@.0..........C
+00006480: 616d 6572 6107 0000 000d 496d 706f 7274  amera.....Import
+00006490: 536c 6970 446c 6701 0300 0000 1004 1e04  SlipDlg.........
+000064a0: 4704 3804 4104 4204 3804 4204 4c08 0000  G.8.A.B.8.B.L...
+000064b0: 0000 0600 0000 0543 6c65 6172 0700 0000  .......Clear....
+000064c0: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+000064d0: 0000 000e 0417 0430 043a 0440 044b 0442  .......0.:.@.K.B
+000064e0: 044c 0800 0000 0006 0000 0005 436c 6f73  .L..........Clos
+000064f0: 6507 0000 000d 496d 706f 7274 536c 6970  e.....ImportSlip
+00006500: 446c 6701 0300 0000 1a04 1404 3004 4204  Dlg.........0.B.
+00006510: 3000 2000 2f00 2004 1204 4004 3504 3c04  0. ./. ...@.5.<.
+00006520: 4f00 3a08 0000 0000 0600 0000 0c44 6174  O.:..........Dat
+00006530: 6520 2f20 5469 6d65 3a07 0000 000d 496d  e / Time:.....Im
+00006540: 706f 7274 536c 6970 446c 6701 0300 0000  portSlipDlg.....
+00006550: 1604 1404 3004 4204 3000 2f04 1204 4004  ....0.B.0./...@.
+00006560: 3504 3c04 4f00 3a08 0000 0000 0600 0000  5.<.O.:.........
+00006570: 0a44 6174 652f 5469 6d65 3a07 0000 000d  .Date/Time:.....
+00006580: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+00006590: 0000 0604 2404 1400 3a08 0000 0000 0600  ....$...:.......
+000065a0: 0000 0346 443a 0700 0000 0d49 6d70 6f72  ...FD:.....Impor
+000065b0: 7453 6c69 7044 6c67 0103 0000 0006 0424  tSlipDlg.......$
+000065c0: 041d 003a 0800 0000 0006 0000 0003 464e  ...:..........FN
+000065d0: 3a07 0000 000d 496d 706f 7274 536c 6970  :.....ImportSlip
+000065e0: 446c 6701 0300 0000 0604 2404 1f00 3a08  Dlg.......$...:.
+000065f0: 0000 0000 0600 0000 0346 503a 0700 0000  .........FP:....
+00006600: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+00006610: 0000 0026 0421 043a 0430 043d 0438 0440  ...&.!.:.0.=.8.@
+00006620: 043e 0432 0430 0442 044c 0020 043a 0430  .>.2.0.B.L. .:.0
+00006630: 043c 0435 0440 043e 0439 0800 0000 0006  .<.5.@.>.9......
+00006640: 0000 000f 4765 7420 6672 6f6d 2063 616d  ....Get from cam
+00006650: 6572 6107 0000 000d 496d 706f 7274 536c  era.....ImportSl
+00006660: 6970 446c 6701 0300 0000 2404 1f04 3e04  ipDlg.....$...>.
+00006670: 3b04 4304 4704 3804 4204 4c00 2004 3804  ;.C.G.8.B.L. .8.
+00006680: 3700 2004 3104 4304 4404 3504 4004 3008  7. .1.C.D.5.@.0.
+00006690: 0000 0000 0600 0000 1247 6574 2066 726f  .........Get fro
+000066a0: 6d20 636c 6970 626f 6172 6407 0000 000d  m clipboard.....
+000066b0: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+000066c0: 0000 3004 1f04 3e04 3b04 4304 4704 3804  ..0...>.;.C.G.8.
+000066d0: 4204 4c00 2004 4704 3504 3a00 2004 4100  B.L. .G.5.:. .A.
+000066e0: 2004 4104 3004 3904 4204 3000 2004 2404   .A.0.9.B.0. .$.
+000066f0: 1d04 2108 0000 0000 0600 0000 1647 6574  ..!..........Get
+00006700: 2073 6c69 7020 6672 6f6d 2069 6e74 6572   slip from inter
+00006710: 6e65 7407 0000 000d 496d 706f 7274 536c  net.....ImportSl
+00006720: 6970 446c 6701 0300 0000 1604 1804 3c04  ipDlg.........<.
+00006730: 3f04 3e04 4004 4200 2004 4704 3504 3a04  ?.>.@.B. .G.5.:.
+00006740: 3008 0000 0000 0600 0000 0b49 6d70 6f72  0..........Impor
+00006750: 7420 536c 6970 0700 0000 0d49 6d70 6f72  t Slip.....Impor
+00006760: 7453 6c69 7044 6c67 0103 0000 000e 0421  tSlipDlg.......!
+00006770: 0442 0440 043e 043a 0438 003a 0800 0000  .B.@.>.:.8.:....
+00006780: 0006 0000 0006 4c69 6e65 733a 0700 0000  ......Lines:....
+00006790: 0d49 6d70 6f72 7453 6c69 7044 6c67 0103  .ImportSlipDlg..
+000067a0: 0000 0024 0417 0430 0433 0440 0443 0437  ...$...0.3.@.C.7
+000067b0: 0438 0442 044c 0020 0438 0437 0020 0444  .8.B.L. .8.7. .D
+000067c0: 0430 0439 043b 0430 0800 0000 0006 0000  .0.9.;.0........
+000067d0: 000e 4c6f 6164 2066 726f 6d20 6669 6c65  ..Load from file
+000067e0: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+000067f0: 6c67 0103 0000 0036 0417 0430 0433 0443  lg.....6...0.3.C
+00006800: 0437 0438 0442 044c 0020 0447 0435 043a  .7.8.B.L. .G.5.:
+00006810: 0430 0020 0438 0437 0020 004a 0053 004f  .0. .8.7. .J.S.O
+00006820: 004e 002d 0444 0430 0439 043b 0430 0800  .N.-.D.0.9.;.0..
+00006830: 0000 0006 0000 0018 4c6f 6164 2073 6c69  ........Load sli
+00006840: 7020 6672 6f6d 204a 534f 4e20 6669 6c65  p from JSON file
+00006850: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006860: 6c67 0103 0000 0016 041a 043e 043d 0442  lg.........>.=.B
+00006870: 0440 0430 0433 0435 043d 0442 003a 0800  .@.0.3.5.=.B.:..
+00006880: 0000 0006 0000 0005 5065 6572 3a07 0000  ........Peer:...
+00006890: 000d 496d 706f 7274 536c 6970 446c 6701  ..ImportSlipDlg.
+000068a0: 0300 0000 0e04 1f04 3e04 3a04 4304 3f04  ........>.:.C.?.
+000068b0: 3a04 3008 0000 0000 0600 0000 0850 7572  :.0..........Pur
+000068c0: 6368 6173 6507 0000 000d 496d 706f 7274  chase.....Import
+000068d0: 536c 6970 446c 6701 0300 0000 0c00 5100  SlipDlg.......Q.
+000068e0: 5200 2d04 3a04 3e04 3408 0000 0000 0600  R.-.:.>.4.......
+000068f0: 0000 0751 522d 636f 6465 0700 0000 0d49  ...QR-code.....I
+00006900: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
+00006910: 000e 0412 043e 0437 0432 0440 0430 0442  .....>.7.2.@.0.B
+00006920: 0800 0000 0006 0000 0006 5265 7475 726e  ..........Return
+00006930: 0700 0000 0d49 6d70 6f72 7453 6c69 7044  .....ImportSlipD
+00006940: 6c67 0103 0000 002e 0423 0441 0442 0430  lg.......#.A.B.0
+00006950: 043d 043e 0432 0438 0442 044c 0020 0442  .=.>.2.8.B.L. .B
+00006960: 044d 0433 0020 0434 043b 044f 0020 0432  .M.3. .4.;.O. .2
+00006970: 0441 0435 0445 0800 0000 0006 0000 0015  .A.5.E..........
+00006980: 5365 7420 5461 6720 666f 7220 616c 6c20  Set Tag for all 
+00006990: 6c69 6e65 7307 0000 000d 496d 706f 7274  lines.....Import
+000069a0: 536c 6970 446c 6701 0300 0000 0604 2704  SlipDlg.......'.
+000069b0: 3504 3a08 0000 0000 0600 0000 0453 6c69  5.:..........Sli
+000069c0: 7007 0000 000d 496d 706f 7274 536c 6970  p.....ImportSlip
+000069d0: 446c 6701 0300 0000 1604 1404 3004 3d04  Dlg.........0.=.
+000069e0: 3d04 4b04 3500 2004 4704 3504 3a04 3008  =.K.5. .G.5.:.0.
+000069f0: 0000 0000 0600 0000 0953 6c69 7020 6461  .........Slip da
+00006a00: 7461 0700 0000 0d49 6d70 6f72 7453 6c69  ta.....ImportSli
+00006a10: 7044 6c67 0103 0000 001c 0417 0430 043a  pDlg.........0.:
+00006a20: 0440 044b 0442 044c 0020 043a 0430 043c  .@.K.B.L. .:.0.<
+00006a30: 0435 0440 0443 0800 0000 0006 0000 000b  .5.@.C..........
+00006a40: 5374 6f70 2063 616d 6572 6107 0000 000d  Stop camera.....
+00006a50: 496d 706f 7274 536c 6970 446c 6701 0300  ImportSlipDlg...
+00006a60: 0000 0804 2204 3804 3f00 3a08 0000 0000  ....".8.?.:.....
+00006a70: 0600 0000 0554 7970 653a 0700 0000 0d49  .....Type:.....I
+00006a80: 6d70 6f72 7453 6c69 7044 6c67 0103 0000  mportSlipDlg....
+00006a90: 0026 0064 0064 002f 004d 004d 002f 0079  .&.d.d./.M.M./.y
+00006aa0: 0079 0079 0079 0020 0068 0068 003a 006d  .y.y.y. .h.h.:.m
+00006ab0: 006d 003a 0073 0073 0800 0000 0006 0000  .m.:.s.s........
+00006ac0: 0013 6464 2f4d 4d2f 7979 7979 2068 683a  ..dd/MM/yyyy hh:
+00006ad0: 6d6d 3a73 7307 0000 000d 496d 706f 7274  mm:ss.....Import
+00006ae0: 536c 6970 446c 6701 0300 0000 6604 1d04  SlipDlg.....f...
+00006af0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+00006b00: 3e00 2004 3e04 3104 4004 3004 3104 3e04  >. .>.1.@.0.1.>.
+00006b10: 4204 3004 4204 4c00 2004 3e04 3f04 3504  B.0.B.L. .>.?.5.
+00006b20: 4004 3004 4604 3804 4e00 2004 3104 3504  @.0.F.8.N. .1.5.
+00006b30: 3700 2004 3404 3504 4204 3004 3b04 4c04  7. .4.5.B.0.;.L.
+00006b40: 3d04 4b04 4500 2004 3404 3004 3d04 3d04  =.K.E. .4.0.=.=.
+00006b50: 4b04 4508 0000 0000 0600 0000 2743 616e  K.E.........'Can
+00006b60: 2774 2070 726f 6365 7373 206f 7065 7261  't process opera
+00006b70: 7469 6f6e 2077 6974 686f 7574 2064 6574  tion without det
+00006b80: 6169 6c73 0700 0000 0e49 6e63 6f6d 6553  ails.....IncomeS
+00006b90: 7065 6e64 696e 6701 0300 0000 0c04 1a04  pending.........
+00006ba0: 4304 4004 4100 3a00 2008 0000 0000 0600  C.@.A.:. .......
+00006bb0: 0000 0652 6174 653a 2007 0000 000e 496e  ...Rate: .....In
+00006bc0: 636f 6d65 5370 656e 6469 6e67 0103 0000  comeSpending....
+00006bd0: 001c 0414 043e 0445 043e 0434 044b 0020  .....>.E.>.4.K. 
+00006be0: 0438 0020 0422 0440 0430 0442 044b 0800  .8. .".@.0.B.K..
+00006bf0: 0000 0006 0000 0011 496e 636f 6d65 2026  ........Income &
+00006c00: 2053 7065 6e64 696e 6707 0000 0014 496e   Spending.....In
+00006c10: 636f 6d65 5370 656e 6469 6e67 5265 706f  comeSpendingRepo
+00006c20: 7274 0103 0000 000a 0418 0422 041e 0413  rt........."....
+00006c30: 041e 0800 0000 0006 0000 0005 544f 5441  ............TOTA
+00006c40: 4c07 0000 0019 496e 636f 6d65 5370 656e  L.....IncomeSpen
+00006c50: 6469 6e67 5265 706f 7274 4d6f 6465 6c01  dingReportModel.
+00006c60: 0300 0000 0e04 1204 3004 3b04 4e04 4204  ........0.;.N.B.
+00006c70: 3000 3a08 0000 0000 0600 0000 0943 7572  0.:..........Cur
+00006c80: 7265 6e63 793a 0700 0000 1a49 6e63 6f6d  rency:.....Incom
+00006c90: 6553 7065 6e64 696e 6752 6570 6f72 7457  eSpendingReportW
+00006ca0: 6964 6765 7401 0300 0000 1c04 1404 3e04  idget.........>.
+00006cb0: 4504 3e04 3404 4b00 2004 3800 2004 2204  E.>.4.K. .8. .".
+00006cc0: 4004 3004 4204 4b08 0000 0000 0600 0000  @.0.B.K.........
+00006cd0: 1149 6e63 6f6d 6520 2620 5370 656e 6469  .Income & Spendi
+00006ce0: 6e67 0700 0000 1a49 6e63 6f6d 6553 7065  ng.....IncomeSpe
+00006cf0: 6e64 696e 6752 6570 6f72 7457 6964 6765  ndingReportWidge
+00006d00: 7401 0300 0000 1204 1f04 3e04 3c04 3504  t.........>.<.5.
+00006d10: 4104 4f04 4704 3d04 3e08 0000 0000 0600  A.O.G.=.>.......
+00006d20: 0000 074d 6f6e 7468 6c79 0700 0000 1a49  ...Monthly.....I
+00006d30: 6e63 6f6d 6553 7065 6e64 696e 6752 6570  ncomeSpendingRep
+00006d40: 6f72 7457 6964 6765 7401 0300 0000 1c04  ortWidget.......
+00006d50: 1f04 3504 4004 3804 3e04 3404 3804 4704  ..5.@.8.>.4.8.G.
+00006d60: 3d04 3e04 4104 4204 4c00 3a08 0000 0000  =.>.A.B.L.:.....
+00006d70: 0600 0000 0c50 6572 696f 6469 6369 7479  .....Periodicity
+00006d80: 3a07 0000 001a 496e 636f 6d65 5370 656e  :.....IncomeSpen
+00006d90: 6469 6e67 5265 706f 7274 5769 6467 6574  dingReportWidget
+00006da0: 0103 0000 0018 0421 043e 0445 0440 0430  .......!.>.E.@.0
+00006db0: 043d 0438 0442 044c 002e 002e 002e 0800  .=.8.B.L........
+00006dc0: 0000 0006 0000 0007 5361 7665 2e2e 2e07  ........Save....
+00006dd0: 0000 001a 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+00006de0: 6e67 5265 706f 7274 5769 6467 6574 0103  ngReportWidget..
+00006df0: 0000 0014 041f 043e 043d 0435 0434 0435  .......>.=.5.4.5
+00006e00: 043b 044c 043d 043e 0800 0000 0006 0000  .;.L.=.>........
+00006e10: 0006 5765 656b 6c79 0700 0000 1a49 6e63  ..Weekly.....Inc
+00006e20: 6f6d 6553 7065 6e64 696e 6752 6570 6f72  omeSpendingRepor
+00006e30: 7457 6964 6765 7401 0300 0000 1c04 1404  tWidget.........
+00006e40: 3e04 4504 3e04 3404 4b00 2004 3800 2004  >.E.>.4.K. .8. .
+00006e50: 2204 4004 3004 4204 4b08 0000 0000 0600  ".@.0.B.K.......
+00006e60: 0000 1149 6e63 6f6d 6520 2620 5370 656e  ...Income & Spen
+00006e70: 6469 6e67 0700 0000 1a49 6e63 6f6d 6553  ding.....IncomeS
+00006e80: 7065 6e64 696e 6752 6570 6f72 7457 696e  pendingReportWin
+00006e90: 646f 7701 0300 0000 2204 1f04 3e04 3a04  dow....."...>.:.
+00006ea0: 3004 3704 3004 4204 4c00 2004 3e04 3f04  0.7.0.B.L. .>.?.
+00006eb0: 3504 4004 3004 4604 3804 3808 0000 0000  5.@.0.F.8.8.....
+00006ec0: 0600 0000 0f53 686f 7720 6f70 6572 6174  .....Show operat
+00006ed0: 696f 6e73 0700 0000 1a49 6e63 6f6d 6553  ions.....IncomeS
+00006ee0: 7065 6e64 696e 6752 6570 6f72 7457 696e  pendingReportWin
+00006ef0: 646f 7701 0300 0000 0804 2104 4704 3504  dow.......!.G.5.
+00006f00: 4208 0000 0000 0600 0000 0741 6363 6f75  B..........Accou
+00006f10: 6e74 0700 0000 1449 6e63 6f6d 6553 7065  nt.....IncomeSpe
+00006f20: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00006f30: 3204 1404 3e04 3104 3004 3204 3804 4204  2...>.1.0.2.8.B.
+00006f40: 4c00 2004 3404 3504 4204 3004 3b04 4c04  L. .4.5.B.0.;.L.
+00006f50: 3d04 4304 4e00 2004 3704 3004 3f04 3804  =.C.N. .7.0.?.8.
+00006f60: 4104 4c08 0000 0000 0600 0000 0a41 6464  A.L..........Add
+00006f70: 2064 6574 6169 6c07 0000 0014 496e 636f   detail.....Inco
+00006f80: 6d65 5370 656e 6469 6e67 5769 6467 6574  meSpendingWidget
+00006f90: 0103 0000 0038 0421 043a 043e 043f 0438  .....8.!.:.>.?.8
+00006fa0: 0440 043e 0432 0430 0442 044c 0020 0434  .@.>.2.0.B.L. .4
+00006fb0: 0435 0442 0430 043b 044c 043d 0443 044e  .5.B.0.;.L.=.C.N
+00006fc0: 0020 0437 0430 043f 0438 0441 044c 0800  . .7.0.?.8.A.L..
+00006fd0: 0000 0006 0000 000b 436f 7079 2064 6574  ........Copy det
+00006fe0: 6169 6c07 0000 0014 496e 636f 6d65 5370  ail.....IncomeSp
+00006ff0: 656e 6469 6e67 5769 6467 6574 0103 0000  endingWidget....
+00007000: 0014 0414 0430 0442 0430 002f 0412 0440  .....0.B.0./...@
+00007010: 0435 043c 044f 0800 0000 0006 0000 0009  .5.<.O..........
+00007020: 4461 7465 2f54 696d 6507 0000 0014 496e  Date/Time.....In
+00007030: 636f 6d65 5370 656e 6469 6e67 5769 6467  comeSpendingWidg
+00007040: 6574 0103 0000 000c 0414 0435 0442 0430  et.........5.B.0
+00007050: 043b 0438 0800 0000 0006 0000 0007 4465  .;.8..........De
+00007060: 7461 696c 7307 0000 0014 496e 636f 6d65  tails.....Income
+00007070: 5370 656e 6469 6e67 5769 6467 6574 0103  SpendingWidget..
+00007080: 0000 0044 041d 0435 0432 043e 0437 043c  ...D...5.2.>.7.<
+00007090: 043e 0436 043d 043e 0020 0434 043e 0431  .>.6.=.>. .4.>.1
+000070a0: 0430 0432 0438 0442 044c 0020 043d 043e  .0.2.8.B.L. .=.>
+000070b0: 0432 0443 044e 0020 0437 0430 043f 0438  .2.C.N. .7.0.?.8
+000070c0: 0441 044c 003a 0020 0800 0000 0006 0000  .A.L.:. ........
+000070d0: 001a 4661 696c 6564 2074 6f20 6164 6420  ..Failed to add 
+000070e0: 6e65 7720 7265 636f 7264 3a20 0700 0000  new record: ....
+000070f0: 1449 6e63 6f6d 6553 7065 6e64 696e 6757  .IncomeSpendingW
+00007100: 6964 6765 7401 0300 0000 1c04 1404 3e04  idget.........>.
+00007110: 4504 3e04 3400 2000 2f00 2004 2004 3004  E.>.4. ./. . .0.
+00007120: 4104 4504 3e04 3408 0000 0000 0600 0000  A.E.>.4.........
+00007130: 1149 6e63 6f6d 6520 2f20 5370 656e 6469  .Income / Spendi
+00007140: 6e67 0700 0000 1449 6e63 6f6d 6553 7065  ng.....IncomeSpe
+00007150: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00007160: 1404 1f04 4004 3804 3c04 3504 4704 3004  ....@.8.<.5.G.0.
+00007170: 3d04 3804 3508 0000 0000 0600 0000 044e  =.8.5..........N
+00007180: 6f74 6507 0000 0014 496e 636f 6d65 5370  ote.....IncomeSp
+00007190: 656e 6469 6e67 5769 6467 6574 0103 0000  endingWidget....
+000071a0: 0048 041e 0448 0438 0431 043a 0430 0020  .H...H.8.1.:.0. 
+000071b0: 043f 0440 0438 0020 0437 0430 043f 0438  .?.@.8. .7.0.?.8
+000071c0: 0441 0438 0020 0434 0435 0442 0430 043b  .A.8. .4.5.B.0.;
+000071d0: 0435 0439 0020 043e 043f 0435 0440 0430  .5.9. .>.?.5.@.0
+000071e0: 0446 0438 0438 003a 0020 0800 0000 0006  .F.8.8.:. ......
+000071f0: 0000 0021 4f70 6572 6174 696f 6e20 6465  ...!Operation de
+00007200: 7461 696c 7320 7375 626d 6974 2066 6169  tails submit fai
+00007210: 6c65 643a 2007 0000 0014 496e 636f 6d65  led: .....Income
+00007220: 5370 656e 6469 6e67 5769 6467 6574 0103  SpendingWidget..
+00007230: 0000 0038 041e 0448 0438 0431 043a 0430  ...8...H.8.1.:.0
+00007240: 0020 043f 0440 0438 0020 0437 0430 043f  . .?.@.8. .7.0.?
+00007250: 0438 0441 0438 0020 043e 043f 0435 0440  .8.A.8. .>.?.5.@
+00007260: 0430 0446 0438 0438 003a 0020 0800 0000  .0.F.8.8.:. ....
+00007270: 0006 0000 0019 4f70 6572 6174 696f 6e20  ......Operation 
+00007280: 7375 626d 6974 2066 6169 6c65 643a 2007  submit failed: .
+00007290: 0000 0014 496e 636f 6d65 5370 656e 6469  ....IncomeSpendi
+000072a0: 6e67 5769 6467 6574 0103 0000 0020 041e  ngWidget..... ..
+000072b0: 043f 043b 0430 0442 0430 0020 0432 0020  .?.;.0.B.0. .2. 
+000072c0: 0432 0430 043b 044e 0442 0435 003a 0800  .2.0.;.N.B.5.:..
+000072d0: 0000 0006 0000 0019 5061 6964 2069 6e20  ........Paid in 
+000072e0: 666f 7265 6967 6e20 6375 7272 656e 6379  foreign currency
+000072f0: 3a07 0000 0014 496e 636f 6d65 5370 656e  :.....IncomeSpen
+00007300: 6469 6e67 5769 6467 6574 0103 0000 0014  dingWidget......
+00007310: 041a 043e 043d 0442 0440 0430 0433 0435  ...>.=.B.@.0.3.5
+00007320: 043d 0442 0800 0000 0006 0000 0004 5065  .=.B..........Pe
+00007330: 6572 0700 0000 1449 6e63 6f6d 6553 7065  er.....IncomeSpe
+00007340: 6e64 696e 6757 6964 6765 7401 0300 0000  ndingWidget.....
+00007350: 3004 2304 3404 3004 3b04 3804 4204 4c00  0.#.4.0.;.8.B.L.
+00007360: 2004 3404 3504 4204 3004 3b04 4c04 3d04   .4.5.B.0.;.L.=.
+00007370: 4304 4e00 2004 3704 3004 3f04 3804 4104  C.N. .7.0.?.8.A.
+00007380: 4c08 0000 0000 0600 0000 0d52 656d 6f76  L..........Remov
+00007390: 6520 6465 7461 696c 0700 0000 1449 6e63  e detail.....Inc
+000073a0: 6f6d 6553 7065 6e64 696e 6757 6964 6765  omeSpendingWidge
+000073b0: 7401 0300 0000 0c00 2604 2104 4704 3504  t.......&.!.G.5.
+000073c0: 4204 3008 0000 0000 0600 0000 0926 4163  B.0..........&Ac
+000073d0: 636f 756e 7473 0700 0000 0e4a 414c 5f4d  counts.....JAL_M
+000073e0: 6169 6e57 696e 646f 7701 0300 0000 1200  ainWindow.......
+000073f0: 2604 1104 4d04 3a04 3004 3f00 2e00 2e00  &...M.:.0.?.....
+00007400: 2e08 0000 0000 0600 0000 0a26 4261 636b  ...........&Back
+00007410: 7570 2e2e 2e07 0000 000e 4a41 4c5f 4d61  up........JAL_Ma
+00007420: 696e 5769 6e64 6f77 0103 0000 001e 0026  inWindow.......&
+00007430: 0411 0430 0437 043e 0432 0430 044f 0020  ...0.7.>.2.0.O. 
+00007440: 0432 0430 043b 044e 0442 0430 0800 0000  .2.0.;.N.B.0....
+00007450: 0006 0000 000e 2642 6173 6520 4375 7272  ......&Base Curr
+00007460: 656e 6379 0700 0000 0e4a 414c 5f4d 6169  ency.....JAL_Mai
+00007470: 6e57 696e 646f 7701 0300 0000 1400 2604  nWindow.......&.
+00007480: 1a04 3004 4204 3504 3304 3e04 4004 3804  ..0.B.5.3.>.@.8.
+00007490: 3808 0000 0000 0600 0000 0b26 4361 7465  8..........&Cate
+000074a0: 676f 7269 6573 0700 0000 0e4a 414c 5f4d  gories.....JAL_M
+000074b0: 6169 6e57 696e 646f 7701 0300 0000 0e00  ainWindow.......
+000074c0: 2604 1404 3004 3d04 3d04 4b04 3508 0000  &...0.=.=.K.5...
+000074d0: 0000 0600 0000 0526 4461 7461 0700 0000  .......&Data....
+000074e0: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
+000074f0: 0300 0000 0c00 2604 1204 4b04 4504 3e04  ......&...K.E.>.
+00007500: 3408 0000 0000 0600 0000 0526 4578 6974  4..........&Exit
+00007510: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
+00007520: 646f 7701 0300 0000 1000 2604 2d04 3a04  dow.......&.-.:.
+00007530: 4104 3f04 3e04 4004 4208 0000 0000 0600  A.?.>.@.B.......
+00007540: 0000 0726 4578 706f 7274 0700 0000 0e4a  ...&Export.....J
+00007550: 414c 5f4d 6169 6e57 696e 646f 7701 0300  AL_MainWindow...
+00007560: 0000 0e00 2604 1804 3c04 3f04 3e04 4004  ....&...<.?.>.@.
+00007570: 4208 0000 0000 0600 0000 0726 496d 706f  B..........&Impo
+00007580: 7274 0700 0000 0e4a 414c 5f4d 6169 6e57  rt.....JAL_MainW
+00007590: 696e 646f 7701 0300 0000 1200 2604 1e04  indow.......&...
+000075a0: 4104 3d04 3e04 3204 3d04 3e04 3508 0000  A.=.>.2.=.>.5...
+000075b0: 0000 0600 0000 0526 4d61 696e 0700 0000  .......&Main....
+000075c0: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
+000075d0: 0300 0000 1200 2604 1e04 3f04 3504 4004  ......&...?.5.@.
+000075e0: 3004 4604 3804 3808 0000 0000 0600 0000  0.F.8.8.........
+000075f0: 0b26 4f70 6572 6174 696f 6e73 0700 0000  .&Operations....
+00007600: 0e4a 414c 5f4d 6169 6e57 696e 646f 7701  .JAL_MainWindow.
+00007610: 0300 0000 1804 1a00 2604 3e04 3d04 4204  ........&.>.=.B.
+00007620: 4004 3004 3304 3504 3d04 4204 4b08 0000  @.0.3.5.=.B.K...
+00007630: 0000 0600 0000 0626 5065 6572 7307 0000  .......&Peers...
+00007640: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007650: 0103 0000 0014 0026 041a 043e 0442 0438  .......&...>.B.8
+00007660: 0440 043e 0432 043a 0438 0800 0000 0006  .@.>.2.:.8......
+00007670: 0000 0007 2651 756f 7465 7307 0000 000e  ....&Quotes.....
+00007680: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+00007690: 0000 001a 0026 041a 043e 0442 0438 0440  .....&...>.B.8.@
+000076a0: 043e 0432 043a 0438 002e 002e 002e 0800  .>.2.:.8........
+000076b0: 0000 0006 0000 000a 2651 756f 7465 732e  ........&Quotes.
+000076c0: 2e2e 0700 0000 0e4a 414c 5f4d 6169 6e57  .......JAL_MainW
+000076d0: 696e 646f 7701 0300 0000 0e00 2604 1e04  indow.......&...
+000076e0: 4204 4704 3504 4204 4b08 0000 0000 0600  B.G.5.B.K.......
+000076f0: 0000 0826 5265 706f 7274 7307 0000 000e  ...&Reports.....
+00007700: 4a41 4c5f 4d61 696e 5769 6e64 6f77 0103  JAL_MainWindow..
+00007710: 0000 0024 0026 0412 043e 0441 0441 0442  ...$.&...>.A.A.B
+00007720: 0430 043d 043e 0432 043b 0435 043d 0438  .0.=.>.2.;.5.=.8
+00007730: 0435 002e 002e 002e 0800 0000 0006 0000  .5..............
+00007740: 000b 2652 6573 746f 7265 2e2e 2e07 0000  ..&Restore......
+00007750: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007760: 0103 0000 000c 0026 041e 0442 0447 0451  .......&...B.G.Q
+00007770: 0442 0800 0000 0006 0000 000a 2653 7461  .B..........&Sta
+00007780: 7465 6d65 6e74 0700 0000 0e4a 414c 5f4d  tement.....JAL_M
+00007790: 6169 6e57 696e 646f 7701 0300 0000 0a00  ainWindow.......
+000077a0: 2604 2204 4d04 3304 3808 0000 0000 0600  &.".M.3.8.......
+000077b0: 0000 0526 5461 6773 0700 0000 0e4a 414c  ...&Tags.....JAL
+000077c0: 5f4d 6169 6e57 696e 646f 7701 0300 0000  _MainWindow.....
+000077d0: 1c00 2604 2604 3504 3d04 3d04 4b04 3500  ..&.&.5.=.=.K.5.
+000077e0: 2004 3104 4304 3c04 3004 3304 3808 0000   .1.C.<.0.3.8...
+000077f0: 0000 0600 0000 0741 2673 7365 7473 0700  .......A&ssets..
+00007800: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
+00007810: 7701 0300 0000 1804 1e04 4704 3804 4104  w.........G.8.A.
+00007820: 4204 3804 4204 4c00 2004 1204 4104 5108  B.8.B.L. ...A.Q.
+00007830: 0000 0000 0600 0000 0943 6c65 616e 2041  .........Clean A
+00007840: 6c6c 0700 0000 0e4a 414c 5f4d 6169 6e57  ll.....JAL_MainW
+00007850: 696e 646f 7701 0300 0000 4e04 1e04 4204  indow.....N...B.
+00007860: 4704 3504 4200 2004 3e00 2000 2604 3404  G.5.B. .>. .&.4.
+00007870: 3204 3804 3604 3504 3d04 3804 4f04 4500  2.8.6.5.=.8.O.E.
+00007880: 2004 3f04 3e00 2004 3704 3004 4004 4304   .?.>. .7.0.@.C.
+00007890: 3104 3504 3604 3d04 4b04 3c00 2004 4104  1.5.6.=.K.<. .A.
+000078a0: 4704 3504 4204 3004 3c08 0000 0000 0600  G.5.B.0.<.......
+000078b0: 0000 1d46 6f72 6569 676e 2061 6363 6f75  ...Foreign accou
+000078c0: 6e74 7320 2666 6c6f 7720 7265 706f 7274  nts &flow report
+000078d0: 0700 0000 0e4a 414c 5f4d 6169 6e57 696e  .....JAL_MainWin
+000078e0: 646f 7701 0300 0000 3e04 1804 3d04 3204  dow.....>...=.2.
+000078f0: 3504 4104 4204 3804 4604 3804 3e04 3d04  5.A.B.8.F.8.>.=.
+00007900: 3d04 4b04 3900 2000 2604 3d04 3004 3b04  =.K.9. .&.=.0.;.
+00007910: 3e04 3304 3e04 3204 4b04 3900 2004 3e04  >.3.>.2.K.9. .>.
+00007920: 4204 4704 3504 4208 0000 0000 0600 0000  B.G.5.B.........
+00007930: 1649 6e76 6573 746d 656e 7420 2674 6178  .Investment &tax
+00007940: 2072 6570 6f72 7407 0000 000e 4a41 4c5f   report.....JAL_
+00007950: 4d61 696e 5769 6e64 6f77 0103 0000 000a  MainWindow......
+00007960: 0026 042f 0437 044b 043a 0800 0000 0006  .&./.7.K.:......
+00007970: 0000 0009 4c26 616e 6775 6167 6507 0000  ....L&anguage...
+00007980: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+00007990: 0103 0000 002a 041f 0435 0440 0435 0441  .....*...5.@.5.A
+000079a0: 0447 0438 0442 0430 0442 044c 0020 0026  .G.8.B.0.B.L. .&
+000079b0: 0438 0442 043e 0433 0438 002e 002e 002e  .8.B.>.3.8......
+000079c0: 0800 0000 0006 0000 0013 5265 2d62 7569  ..........Re-bui
+000079d0: 6c64 2026 4c65 6467 6572 2e2e 2e07 0000  ld &Ledger......
+000079e0: 000e 4a41 4c5f 4d61 696e 5769 6e64 6f77  ..JAL_MainWindow
+000079f0: 0103 0000 0016 0427 0435 043a 0020 005b  .......'.5.:. .[
+00007a00: 0052 0055 005d 002e 002e 002e 0800 0000  .R.U.]..........
+00007a10: 0006 0000 000c 536c 6970 205b 5255 5d2e  ......Slip [RU].
+00007a20: 2e2e 0700 0000 0e4a 414c 5f4d 6169 6e57  .......JAL_MainW
+00007a30: 696e 646f 7701 0300 0000 0600 6a00 6100  indow.......j.a.
+00007a40: 6c08 0000 0000 0600 0000 036a 616c 0700  l..........jal..
+00007a50: 0000 0e4a 414c 5f4d 6169 6e57 696e 646f  ...JAL_MainWindo
+00007a60: 7701 0300 0000 2004 1104 3004 3d04 3a00  w..... ...0.=.:.
+00007a70: 2004 3404 3b04 4f00 2004 4104 4704 3504   .4.;.O. .A.G.5.
+00007a80: 4204 3000 2021 1608 0000 0000 0600 0000  B.0. !..........
+00007a90: 1242 616e 6b20 666f 7220 6163 636f 756e  .Bank for accoun
+00007aa0: 7420 2307 0000 000a 4a61 6c41 6363 6f75  t #.....JalAccou
+00007ab0: 6e74 0103 0000 002a 0421 0442 0440 0430  nt.....*.!.B.@.0
+00007ac0: 043d 0430 0020 043e 0431 043d 043e 0432  .=.0. .>.1.=.>.2
+00007ad0: 043b 0451 043d 0430 0020 0434 043b 044f  .;.Q.=.0. .4.;.O
+00007ae0: 0020 0800 0000 0006 0000 0014 436f 756e  . ..........Coun
+00007af0: 7472 7920 7570 6461 7465 6420 666f 7220  try updated for 
+00007b00: 0700 0000 084a 616c 4173 7365 7401 0300  .....JalAsset...
+00007b10: 0000 2a04 1a04 3e04 4204 3804 4004 3e04  ..*...>.B.8.@.>.
+00007b20: 3204 3a04 3800 2004 3e04 3104 3d04 3e04  2.:.8. .>.1.=.>.
+00007b30: 3204 3b04 3504 3d04 4b00 3a00 2008 0000  2.;.5.=.K.:. ...
+00007b40: 0000 0600 0000 1951 756f 7461 7469 6f6e  .......Quotation
+00007b50: 7320 7765 7265 2075 7064 6174 6564 3a20  s were updated: 
+00007b60: 0700 0000 084a 616c 4173 7365 7401 0300  .....JalAsset...
+00007b70: 0000 4604 2004 3504 3304 3804 4104 4204  ..F. .5.3.8.A.B.
+00007b80: 4004 3004 4604 3804 3e04 3d04 3d04 4b04  @.0.F.8.>.=.=.K.
+00007b90: 3900 2004 3d04 3e04 3c04 3504 4000 2004  9. .=.>.<.5.@. .
+00007ba0: 3e04 3104 3d04 3e04 3204 3b04 5104 3d00  >.1.=.>.2.;.Q.=.
+00007bb0: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
+00007bc0: 0000 1752 6567 2e6e 756d 6265 7220 7570  ...Reg.number up
+00007bd0: 6461 7465 6420 666f 7220 0700 0000 084a  dated for .....J
+00007be0: 616c 4173 7365 7401 0300 0000 3004 1d04  alAsset.....0...
+00007bf0: 3504 4200 2004 3a04 3e04 4204 3804 4004  5.B. .:.>.B.8.@.
+00007c00: 3e04 3204 3a04 3800 2f04 3a04 4304 4004  >.2.:.8./.:.C.@.
+00007c10: 4104 3000 2004 3404 3b04 4f00 2008 0000  A.0. .4.;.O. ...
+00007c20: 0000 0600 0000 1c54 6865 7265 2061 7265  .......There are
+00007c30: 206e 6f20 7175 6f74 652f 7261 7465 2066   no quote/rate f
+00007c40: 6f72 2007 0000 0008 4a61 6c41 7373 6574  or .....JalAsset
+00007c50: 0103 0000 004c 041d 0435 043e 0436 0438  .....L...5.>.6.8
+00007c60: 0434 0430 043d 043d 0430 044f 0020 043f  .4.0.=.=.0.O. .?
+00007c70: 043e 043f 044b 0442 043a 0430 0020 043e  .>.?.K.B.:.0. .>
+00007c80: 0431 043d 043e 0432 0438 0442 044c 0020  .1.=.>.2.8.B.L. 
+00007c90: 0049 0053 0049 004e 0020 0434 043b 044f  .I.S.I.N. .4.;.O
+00007ca0: 0020 0800 0000 0006 0000 0026 556e 6578  . .........&Unex
+00007cb0: 7065 6374 6564 2061 7474 656d 7074 2074  pected attempt t
+00007cc0: 6f20 7570 6461 7465 2049 5349 4e20 666f  o update ISIN fo
+00007cd0: 7220 0700 0000 084a 616c 4173 7365 7401  r .....JalAsset.
+00007ce0: 0300 0000 0600 2004 3200 2008 0000 0000  ...... .2. .....
+00007cf0: 0600 0000 0620 696e 746f 2007 0000 0009  ..... into .....
+00007d00: 4a61 6c42 6163 6b75 7001 0300 0000 1c04  JalBackup.......
+00007d10: 1004 4004 4504 3804 3204 4b00 2000 2800  ..@.E.8.2.K. .(.
+00007d20: 2a00 2e00 7400 6700 7a00 2908 0000 0000  *...t.g.z.).....
+00007d30: 0600 0000 1041 7263 6869 7665 7320 282a  .....Archives (*
+00007d40: 2e74 677a 2907 0000 0009 4a61 6c42 6163  .tgz).....JalBac
+00007d50: 6b75 7001 0300 0000 4604 1d04 3500 2004  kup.....F...5. .
+00007d60: 4004 3004 4104 3f04 3e04 3704 3d04 3004  @.0.A.?.>.7.=.0.
+00007d70: 3d04 3000 2004 3c04 3504 4204 3a04 3000  =.0. .<.5.B.:.0.
+00007d80: 2004 4004 3504 3704 3504 4004 3204 3d04   .@.5.7.5.@.2.=.
+00007d90: 3e04 3900 2004 3a04 3e04 3f04 3804 3808  >.9. .:.>.?.8.8.
+00007da0: 0000 0000 0600 0000 1b42 6163 6b75 7020  .........Backup 
+00007db0: 6c61 6265 6c20 6e6f 7420 7265 636f 676e  label not recogn
+00007dc0: 697a 6564 0700 0000 094a 616c 4261 636b  ized.....JalBack
+00007dd0: 7570 0103 0000 0046 0420 0435 0437 0435  up.....F. .5.7.5
+00007de0: 0440 0432 043d 0430 044f 0020 043a 043e  .@.2.=.0.O. .:.>
+00007df0: 043f 0438 044f 0020 0432 043e 0441 0441  .?.8.O. .2.>.A.A
+00007e00: 0442 0430 0432 043d 043e 0432 043b 0435  .B.0.2.=.>.2.;.5
+00007e10: 043d 0430 0020 0438 0437 003a 0020 0800  .=.0. .8.7.:. ..
+00007e20: 0000 0006 0000 0016 4261 636b 7570 2072  ........Backup r
+00007e30: 6573 746f 7265 6420 6672 6f6d 3a20 0700  estored from: ..
+00007e40: 0000 094a 616c 4261 636b 7570 0103 0000  ...JalBackup....
+00007e50: 003a 0420 0435 0437 0435 0440 0432 043d  .:. .5.7.5.@.2.=
+00007e60: 0430 044f 0020 043a 043e 043f 0438 044f  .0.O. .:.>.?.8.O
+00007e70: 0020 0441 043e 0445 0440 0430 043d 0451  . .A.>.E.@.0.=.Q
+00007e80: 043d 0430 0020 0432 003a 0020 0800 0000  .=.0. .2.:. ....
+00007e90: 0006 0000 0011 4261 636b 7570 2073 6176  ......Backup sav
+00007ea0: 6564 2069 6e3a 2007 0000 0009 4a61 6c42  ed in: .....JalB
+00007eb0: 6163 6b75 7001 0300 0000 5204 1d04 3504  ackup.....R...5.
+00007ec0: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00007ed0: 2004 3f04 4004 3e04 3204 3504 4004 3804   .?.@.>.2.5.@.8.
+00007ee0: 4204 4c00 2004 3404 3004 4204 4300 2004  B.L. .4.0.B.C. .
+00007ef0: 4004 3504 3704 3504 4004 3204 3d04 3e04  @.5.7.5.@.2.=.>.
+00007f00: 3900 2004 3a04 3e04 3f04 3804 3808 0000  9. .:.>.?.8.8...
+00007f10: 0000 0600 0000 1a43 616e 2774 2076 616c  .......Can't val
+00007f20: 6964 6174 6520 6261 636b 7570 2064 6174  idate backup dat
+00007f30: 6507 0000 0009 4a61 6c42 6163 6b75 7001  e.....JalBackup.
+00007f40: 0300 0000 2804 1404 3004 3d04 3d04 4b04  ....(...0.=.=.K.
+00007f50: 3500 2004 3204 3e04 4104 4104 4204 3004  5. .2.>.A.A.B.0.
+00007f60: 3d04 3e04 3204 3b04 3504 3d04 4b08 0000  =.>.2.;.5.=.K...
+00007f70: 0000 0600 0000 0d44 6174 6120 7265 7374  .......Data rest
+00007f80: 6f72 6564 0700 0000 094a 616c 4261 636b  ored.....JalBack
+00007f90: 7570 0103 0000 0042 0414 0430 043d 043d  up.....B...0.=.=
+00007fa0: 044b 0435 0020 0431 044b 043b 0438 0020  .K.5. .1.K.;.8. 
+00007fb0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00007fc0: 044b 0020 0438 0437 0020 0431 044d 043a  .K. .8.7. .1.M.:
+00007fd0: 0430 043f 0430 002e 000a 0800 0000 0006  .0.?.0..........
+00007fe0: 0000 0025 4461 7461 6261 7365 2077 6173  ...%Database was
+00007ff0: 206c 6f61 6465 6420 6672 6f6d 2074 6865   loaded from the
+00008000: 2062 6163 6b75 702e 0a07 0000 0009 4a61   backup.......Ja
+00008010: 6c42 6163 6b75 7001 0300 0000 4e04 1d04  lBackup.....N...
+00008020: 3500 2004 4304 3404 3004 3b04 3e04 4104  5. .C.4.0.;.>.A.
+00008030: 4c00 2004 3204 3e04 4104 4104 4204 3004  L. .2.>.A.A.B.0.
+00008040: 3d04 3e04 3204 3804 4204 4c00 2004 4004  =.>.2.8.B.L. .@.
+00008050: 3504 3704 3504 4004 3204 3d04 4304 4e00  5.7.5.@.2.=.C.N.
+00008060: 2004 3a04 3e04 3f04 3804 4e08 0000 0000   .:.>.?.8.N.....
+00008070: 0600 0000 1d46 6169 6c65 6420 746f 2072  .....Failed to r
+00008080: 6573 746f 7265 2062 6163 6b75 7020 6669  estore backup fi
+00008090: 6c65 0700 0000 094a 616c 4261 636b 7570  le.....JalBackup
+000080a0: 0103 0000 0038 0421 043e 0445 0440 0430  .....8.!.>.E.@.0
+000080b0: 043d 0438 0442 044c 0020 0440 0435 0437  .=.8.B.L. .@.5.7
+000080c0: 0435 0440 0432 043d 0443 044e 0020 043a  .5.@.2.=.C.N. .:
+000080d0: 043e 043f 0438 044e 0020 0432 003a 0800  .>.?.8.N. .2.:..
+000080e0: 0000 0006 0000 000f 5361 7665 2062 6163  ........Save bac
+000080f0: 6b75 7020 746f 3a07 0000 0009 4a61 6c42  kup to:.....JalB
+00008100: 6163 6b75 7001 0300 0000 4004 1204 4b04  ackup.....@...K.
+00008110: 3104 3504 4004 3804 4204 3500 2004 4404  1.5.@.8.B.5. .D.
+00008120: 3004 3904 3b00 2004 4100 2004 4004 3504  0.9.;. .A. .@.5.
+00008130: 3704 3504 4004 3204 3d04 3e04 3900 2004  7.5.@.2.=.>.9. .
+00008140: 3a04 3e04 3f04 3804 3504 3908 0000 0000  :.>.?.8.5.9.....
+00008150: 0600 0000 1753 656c 6563 7420 6669 6c65  .....Select file
+00008160: 2077 6974 6820 6261 636b 7570 0700 0000   with backup....
+00008170: 094a 616c 4261 636b 7570 0103 0000 004a  .JalBackup.....J
+00008180: 041d 0435 0432 0435 0440 043d 044b 0439  ...5.2.5.@.=.K.9
+00008190: 0020 0444 043e 0440 043c 0430 0442 0020  . .D.>.@.<.0.B. 
+000081a0: 0444 0430 0439 043b 0430 0020 0440 0435  .D.0.9.;.0. .@.5
+000081b0: 0437 0435 0440 0432 043d 043e 0439 0020  .7.5.@.2.=.>.9. 
+000081c0: 043a 043e 043f 0438 0438 0800 0000 0006  .:.>.?.8.8......
+000081d0: 0000 001b 5772 6f6e 6720 666f 726d 6174  ....Wrong format
+000081e0: 206f 6620 6261 636b 7570 2066 696c 6507   of backup file.
+000081f0: 0000 0009 4a61 6c42 6163 6b75 7001 0300  ....JalBackup...
+00008200: 0000 c804 1204 4b00 2004 3404 3e04 3b04  ......K. .4.>.;.
+00008210: 3604 3d04 4b00 2004 3f04 3504 4004 3504  6.=.K. .?.5.@.5.
+00008220: 3704 3004 3f04 4304 4104 4204 3804 4204  7.0.?.C.A.B.8.B.
+00008230: 4c00 2004 3f04 4004 3804 3b04 3e04 3604  L. .?.@.8.;.>.6.
+00008240: 3504 3d04 3804 3500 2c00 2004 4704 4204  5.=.8.5.,. .G.B.
+00008250: 3e04 3104 4b00 2004 3f04 4004 3804 3c04  >.1.K. .?.@.8.<.
+00008260: 3504 3d04 3804 4204 4c00 2004 3804 3704  5.=.8.B.L. .8.7.
+00008270: 3c04 3504 3d04 3504 3d04 3804 4f00 0a04  <.5.=.5.=.8.O...
+00008280: 1f04 4004 3804 3b04 3e04 3604 3504 3d04  ..@.8.;.>.6.5.=.
+00008290: 3804 3500 2004 4104 3504 3904 4704 3004  8.5. .A.5.9.G.0.
+000082a0: 4100 2004 3704 3004 3204 3504 4004 4804  A. .7.0.2.5.@.H.
+000082b0: 3804 4200 2004 4104 3204 3e04 4e00 2004  8.B. .A.2.>.N. .
+000082c0: 4004 3004 3104 3e04 4204 4308 0000 0000  @.0.1.>.B.C.....
+000082d0: 0600 0000 5259 6f75 2073 686f 756c 6420  ....RYou should 
+000082e0: 7265 7374 6172 7420 6170 706c 6963 6174  restart applicat
+000082f0: 696f 6e20 746f 2061 7070 6c79 2063 6861  ion to apply cha
+00008300: 6e67 6573 0a41 7070 6c69 6361 7469 6f6e  nges.Application
+00008310: 2077 696c 6c20 6265 2074 6572 6d69 6e61   will be termina
+00008320: 7465 6420 6e6f 7707 0000 0009 4a61 6c42  ted now.....JalB
+00008330: 6163 6b75 7001 0300 0000 6404 1e04 3f04  ackup.....d...?.
+00008340: 3504 4004 3004 4604 3804 4f00 2004 4304  5.@.0.F.8.O. .C.
+00008350: 3604 3500 2004 3504 4104 4204 4c00 2004  6.5. .5.A.B.L. .
+00008360: 3200 2004 3104 3004 3704 3500 2004 3404  2. .1.0.7.5. .4.
+00008370: 3004 3d04 3d04 4b04 4500 2004 3800 2004  0.=.=.K.E. .8. .
+00008380: 3104 4b04 3b04 3000 2004 3f04 4004 3e04  1.K.;.0. .?.@.>.
+00008390: 3f04 4304 4904 3504 3d04 3000 3a00 2008  ?.C.I.5.=.0.:. .
+000083a0: 0000 0000 0600 0000 314f 7065 7261 7469  ........1Operati
+000083b0: 6f6e 2061 6c72 6561 6479 2070 7265 7365  on already prese
+000083c0: 6e74 2069 6e20 6462 2061 6e64 2077 6173  nt in db and was
+000083d0: 2073 6b69 7070 6564 3a20 0700 0000 054a   skipped: .....J
+000083e0: 616c 4442 0103 0000 006e 0020 0438 043c  alDB.....n. .8.<
+000083f0: 0435 0435 0442 0020 043d 0435 0441 043e  .5.5.B. .=.5.A.>
+00008400: 0445 0440 0430 043d 0451 043d 043d 044b  .E.@.0.=.Q.=.=.K
+00008410: 0435 0020 0438 0437 043c 0435 043d 0435  .5. .8.7.<.5.=.5
+00008420: 043d 0438 044f 002c 000a 0432 044b 0020  .=.8.O.,...2.K. 
+00008430: 0445 043e 0442 0438 0442 0435 0020 0438  .E.>.B.8.B.5. .8
+00008440: 0445 0020 0441 043e 0445 0440 0430 043d  .E. .A.>.E.@.0.=
+00008450: 0438 0442 044c 003f 0800 0000 0006 0000  .8.B.L.?........
+00008460: 0031 2068 6173 2075 6e63 6f6d 6d69 7474  .1 has uncommitt
+00008470: 6564 2063 6861 6e67 6573 2c0a 646f 2079  ed changes,.do y
+00008480: 6f75 2077 616e 7420 746f 2073 6176 6520  ou want to save 
+00008490: 6974 3f07 0000 0011 4a61 6c4f 7065 7261  it?.....JalOpera
+000084a0: 7469 6f6e 7354 6162 7301 0300 0000 3604  tionsTabs.....6.
+000084b0: 1504 4104 4204 4c00 2004 3d04 3504 4104  ..A.B.L. .=.5.A.
+000084c0: 3e04 4504 4004 3004 3d04 5104 3d04 3d04  >.E.@.0.=.Q.=.=.
+000084d0: 4b04 3500 2004 3804 3704 3c04 3504 3d04  K.5. .8.7.<.5.=.
+000084e0: 3d04 3804 4f08 0000 0000 0600 0000 1859  =.8.O..........Y
+000084f0: 6f75 2068 6176 6520 756e 7361 7665 6420  ou have unsaved 
+00008500: 6368 616e 6765 7307 0000 0011 4a61 6c4f  changes.....JalO
+00008510: 7065 7261 7469 6f6e 7354 6162 7301 0300  perationsTabs...
+00008520: 0000 5a04 1d04 3504 3204 3e04 3704 3c04  ..Z...5.2.>.7.<.
+00008530: 3e04 3604 3d04 3e00 2004 4304 3404 3004  >.6.=.>. .C.4.0.
+00008540: 3b04 3804 4204 4c00 2004 3f04 4004 3504  ;.8.B.L. .?.@.5.
+00008550: 3404 3e04 3f04 4004 3504 3404 3504 3b04  4.>.?.@.5.4.5.;.
+00008560: 5104 3d04 3d04 4304 4e00 2004 3a04 3004  Q.=.=.C.N. .:.0.
+00008570: 4204 3504 3304 3e04 4004 3804 4e08 0000  B.5.3.>.@.8.N...
+00008580: 0000 0600 0000 2043 616e 2774 2064 656c  ...... Can't del
+00008590: 6574 6520 7072 6564 6566 696e 6564 2063  ete predefined c
+000085a0: 6174 6567 6f72 7907 0000 000b 4a61 6c53  ategory.....JalS
+000085b0: 716c 4572 726f 7201 0300 0000 9e04 2d04  qlError.......-.
+000085c0: 4204 3800 2004 3404 3004 3d04 3d04 4b04  B.8. .4.0.=.=.K.
+000085d0: 3500 2004 3d04 3500 2004 3c04 3e04 3304  5. .=.5. .<.>.3.
+000085e0: 4304 4200 2004 3104 4b04 4204 4c00 2004  C.B. .1.K.B.L. .
+000085f0: 3c04 3e04 3404 3804 4404 3804 4604 3804  <.>.4.8.D.8.F.8.
+00008600: 4004 3e04 3204 3004 3d04 4b00 2c00 2004  @.>.2.0.=.K.,. .
+00008610: 4200 2e04 3a00 2e00 2004 3d04 3000 2004  B...:... .=.0. .
+00008620: 3d04 3804 4500 2004 3504 4104 4204 4c00  =.8.E. .5.A.B.L.
+00008630: 2004 4104 4104 4b04 3b04 3a04 3000 2004   .A.A.K.;.:.0. .
+00008640: 3200 2004 3404 4004 4304 3304 3e04 3c00  2. .4.@.C.3.>.<.
+00008650: 2004 3c04 3504 4104 4204 3508 0000 0000   .<.5.A.B.5.....
+00008660: 0600 0000 3a44 6174 6120 6172 6520 7265  ....:Data are re
+00008670: 6665 7265 6e63 6564 2069 6e20 616e 6f74  ferenced in anot
+00008680: 6865 7220 706c 6163 6520 616e 6420 6361  her place and ca
+00008690: 6e27 7420 6265 206d 6f64 6966 6965 6407  n't be modified.
+000086a0: 0000 000b 4a61 6c53 716c 4572 726f 7201  ....JalSqlError.
+000086b0: 0300 0000 1e04 1e04 4804 3804 3104 3a04  ........H.8.1.:.
+000086c0: 3000 2004 3200 2004 3404 3004 3d04 3d04  0. .2. .4.0.=.=.
+000086d0: 4b04 4508 0000 0000 0600 0000 0e44 6174  K.E..........Dat
+000086e0: 6162 6173 6520 6572 726f 7207 0000 000b  abase error.....
+000086f0: 4a61 6c53 716c 4572 726f 7201 0300 0000  JalSqlError.....
+00008700: 5004 1d04 3504 3204 3504 4004 3d04 3e00  P...5.2.5.@.=.>.
+00008710: 2004 3204 4b04 3104 4004 3004 3d04 3000   .2.K.1.@.0.=.0.
+00008720: 2004 3204 3004 3b04 4e04 4204 3000 2004   .2.0.;.N.B.0. .
+00008730: 3404 3b04 4f00 2004 4604 3504 3d04 3d04  4.;.O. .F.5.=.=.
+00008740: 3e04 3900 2004 3104 4304 3c04 3004 3304  >.9. .1.C.<.0.3.
+00008750: 3808 0000 0000 0600 0000 2a49 6e63 6f72  8.........*Incor
+00008760: 7265 6374 2063 7572 7265 6e63 7920 6173  rect currency as
+00008770: 7369 676e 6d65 6e74 2066 6f72 2061 6e20  signment for an 
+00008780: 6173 7365 7407 0000 000b 4a61 6c53 716c  asset.....JalSql
+00008790: 4572 726f 7201 0300 0000 8004 1f04 3e04  Error.........>.
+000087a0: 3b04 3500 2004 1104 3004 3d04 3a00 2f04  ;.5. ...0.=.:./.
+000087b0: 1104 4004 3e04 3a04 3504 4000 2004 3404  ..@.>.:.5.@. .4.
+000087c0: 3e04 3b04 3604 3d04 3e00 2004 3104 4b04  >.;.6.=.>. .1.K.
+000087d0: 4204 4c00 2004 3704 3004 3f04 3e04 3b04  B.L. .7.0.?.>.;.
+000087e0: 3d04 3504 3d04 3e00 2004 3404 3b04 4f00  =.5.=.>. .4.;.O.
+000087f0: 2004 3804 3d04 3204 3504 4104 4204 3804   .8.=.2.5.A.B.8.
+00008800: 4604 3804 3e04 3d04 3d04 3e04 3304 3e00  F.8.>.=.=.>.3.>.
+00008810: 2004 4104 4704 3504 4204 3008 0000 0000   .A.G.5.B.0.....
+00008820: 0600 0000 3949 6e76 6573 746d 656e 7420  ....9Investment 
+00008830: 6163 636f 756e 7420 7368 6f75 6c64 2068  account should h
+00008840: 6176 6520 6173 736f 6369 6174 6564 2062  ave associated b
+00008850: 726f 6b65 7220 6173 7369 676e 6564 0700  roker assigned..
+00008860: 0000 0b4a 616c 5371 6c45 7272 6f72 0103  ...JalSqlError..
+00008870: 0000 0088 0020 043e 043f 0435 0440 0430  ..... .>.?.5.@.0
+00008880: 0446 0438 0439 0020 0442 0440 0435 0431  .F.8.9. .B.@.5.1
+00008890: 0443 044e 0442 0020 043f 0435 0440 0435  .C.N.B. .?.5.@.5
+000088a0: 0440 0430 0441 0447 0435 0442 0430 002e  .@.0.A.G.5.B.0..
+000088b0: 0020 0412 044b 0020 0445 043e 0434 0438  . ...K. .E.>.4.8
+000088c0: 0442 0435 0020 0432 044b 043f 043e 043b  .B.5. .2.K.?.>.;
+000088d0: 043d 0438 0442 044c 0020 0435 0433 043e  .=.8.B.L. .5.3.>
+000088e0: 0020 043f 0440 044f 043c 043e 0020 0441  . .?.@.O.<.>. .A
+000088f0: 0435 0439 0447 0430 0441 003f 0800 0000  .5.9.G.0.A.?....
+00008900: 0006 0000 003c 206f 7065 7261 7469 6f6e  .....< operation
+00008910: 7320 7265 7175 6972 6520 7265 6275 696c  s require rebuil
+00008920: 642e 2044 6f20 796f 7520 7761 6e74 2074  d. Do you want t
+00008930: 6f20 646f 2069 7420 7269 6768 7420 6e6f  o do it right no
+00008940: 773f 0700 0000 064c 6564 6765 7201 0300  w?.....Ledger...
+00008950: 0000 2200 2c00 2004 3d04 3e04 3204 3004  ..".,. .=.>.2.0.
+00008960: 4f00 2004 3304 4004 3004 3d04 3804 4604  O. .3.@.0.=.8.F.
+00008970: 3000 3a00 2008 0000 0000 0600 0000 102c  0.:. ..........,
+00008980: 206e 6577 2066 726f 6e74 6965 723a 2007   new frontier: .
+00008990: 0000 0006 4c65 6467 6572 0103 0000 001a  ....Ledger......
+000089a0: 041f 043e 0434 0442 0432 0435 0440 0436  ...>.4.B.2.5.@.6
+000089b0: 0434 0435 043d 0438 0435 0800 0000 0006  .4.5.=.8.5......
+000089c0: 0000 000c 436f 6e66 6972 6d61 7469 6f6e  ....Confirmation
+000089d0: 0700 0000 064c 6564 6765 7201 0300 0000  .....Ledger.....
+000089e0: 9404 1f04 4004 3e04 3804 3704 3e04 4804  ....@.>.8.7.>.H.
+000089f0: 3b04 3000 2004 3e04 4804 3804 3104 3a04  ;.0. .>.H.8.1.:.
+00008a00: 3000 2e00 2004 2004 3004 4104 4704 5104  0... . .0.A.G.Q.
+00008a10: 4200 2004 3804 4204 3e04 3304 3e04 3200  B. .8.B.>.3.>.2.
+00008a20: 2004 3d04 3500 2004 3e04 3a04 3e04 3d04   .=.5. .>.:.>.=.
+00008a30: 4704 3504 3d00 2e00 2004 1f04 4004 3e04  G.5.=... ...@.>.
+00008a40: 3204 3504 4004 4c04 4204 3500 2004 4104  2.5.@.L.B.5. .A.
+00008a50: 3e04 3e04 3104 4904 3504 3d04 3804 4f00  >.>.1.I.5.=.8.O.
+00008a60: 2004 3e04 3100 2004 3e04 4804 3804 3104   .>.1. .>.H.8.1.
+00008a70: 3a04 3004 4508 0000 0000 0600 0000 4d45  :.0.E.........ME
+00008a80: 7863 6570 7469 6f6e 2068 6170 7065 6e65  xception happene
+00008a90: 642e 204c 6564 6765 7220 6973 2069 6e63  d. Ledger is inc
+00008aa0: 6f6d 706c 6574 652e 2050 6c65 6173 6520  omplete. Please 
+00008ab0: 636f 7272 6563 7420 6572 726f 7273 206c  correct errors l
+00008ac0: 6973 7465 6420 696e 206c 6f67 0700 0000  isted in log....
+00008ad0: 064c 6564 6765 7201 0300 0000 4a04 1804  .Ledger.....J...
+00008ae0: 4204 3e04 3304 3800 2004 4004 3004 4104  B.>.3.8. .@.0.A.
+00008af0: 4104 4704 3804 4204 3004 3d04 4b00 2e00  A.G.8.B.0.=.K...
+00008b00: 2004 1704 3004 4204 4004 3004 4704 3504   ...0.B.@.0.G.5.
+00008b10: 3d04 3d04 3e04 3500 2004 3204 4004 3504  =.=.>.5. .2.@.5.
+00008b20: 3c04 4f00 3a00 2008 0000 0000 0600 0000  <.O.:. .........
+00008b30: 224c 6564 6765 7220 6973 2063 6f6d 706c  "Ledger is compl
+00008b40: 6574 652e 2045 6c61 7073 6564 2074 696d  ete. Elapsed tim
+00008b50: 653a 2007 0000 0006 4c65 6467 6572 0103  e: .....Ledger..
+00008b60: 0000 002c 0422 0440 0430 043d 0437 0430  ...,.".@.0.=.7.0
+00008b70: 043a 0446 0438 0438 0020 043e 0442 0441  .:.F.8.8. .>.B.A
+00008b80: 0443 0442 0441 0442 0432 0443 044e 0442  .C.B.A.B.2.C.N.B
+00008b90: 0800 0000 0006 0000 000e 4c65 6765 7220  ..........Leger 
+00008ba0: 6973 2065 6d70 7479 0700 0000 064c 6564  is empty.....Led
+00008bb0: 6765 7201 0300 0000 2604 1d04 3500 2004  ger.....&...5. .
+00008bc0: 4304 3a04 3004 3704 3004 3d04 3000 2004  C.:.0.7.0.=.0. .
+00008bd0: 2604 1100 2004 3404 3b04 4f00 3a00 2008  &... .4.;.O.:. .
+00008be0: 0000 0000 0600 0000 164e 6f20 6173 7365  .........No asse
+00008bf0: 7420 6465 6669 6e65 6420 666f 723a 2007  t defined for: .
+00008c00: 0000 0006 4c65 6467 6572 0103 0000 0034  ....Ledger.....4
+00008c10: 041d 0443 0020 0443 043a 0430 0437 0430  ...C. .C.:.0.7.0
+00008c20: 043d 0430 0020 043a 0430 0442 0435 0433  .=.0. .:.0.B.5.3
+00008c30: 043e 0440 0438 044f 0020 0434 043b 044f  .>.@.8.O. .4.;.O
+00008c40: 003a 0020 0800 0000 0006 0000 0015 4e6f  .:. ..........No
+00008c50: 2063 6174 6567 6f72 7920 7365 7420 666f   category set fo
+00008c60: 723a 2007 0000 0006 4c65 6467 6572 0103  r: .....Ledger..
+00008c70: 0000 0034 041d 0435 0020 0443 043a 0430  ...4...5. .C.:.0
+00008c80: 0437 0430 043d 0020 043a 043e 043d 0442  .7.0.=. .:.>.=.B
+00008c90: 0440 0430 0433 0435 043d 0442 0020 0434  .@.0.3.5.=.B. .4
+00008ca0: 043b 044f 003a 0020 0800 0000 0006 0000  .;.O.:. ........
+00008cb0: 0011 4e6f 2070 6565 7220 7365 7420 666f  ..No peer set fo
+00008cc0: 723a 2007 0000 0006 4c65 6467 6572 0103  r: .....Ledger..
+00008cd0: 0000 0026 041f 0435 0440 0435 0441 0447  ...&...5.@.5.A.G
+00008ce0: 0451 0442 0020 0438 0442 043e 0433 043e  .Q.B. .8.B.>.3.>
+00008cf0: 0432 0020 0441 003a 0020 0800 0000 0006  .2. .A.:. ......
+00008d00: 0000 001a 5265 2d62 7569 6c64 696e 6720  ....Re-building 
+00008d10: 6c65 6467 6572 2073 696e 6365 3a20 0700  ledger since: ..
+00008d20: 0000 064c 6564 6765 7201 0300 0000 1004  ...Ledger.......
+00008d30: 1e04 4704 3804 4104 4204 3804 4204 4c08  ..G.8.A.B.8.B.L.
+00008d40: 0000 0000 0600 0000 0543 6c65 6172 0700  .........Clear..
+00008d50: 0000 094c 6f67 5669 6577 6572 0103 0000  ...LogViewer....
+00008d60: 0014 041a 043e 043f 0438 0440 043e 0432  .....>.?.8.@.>.2
+00008d70: 0430 0442 044c 0800 0000 0006 0000 0004  .0.B.L..........
+00008d80: 436f 7079 0700 0000 094c 6f67 5669 6577  Copy.....LogView
+00008d90: 6572 0103 0000 0016 0412 044b 0431 0440  er.........K.1.@
+00008da0: 0430 0442 044c 0020 0432 0441 0451 0800  .0.B.L. .2.A.Q..
+00008db0: 0000 0006 0000 000a 5365 6c65 6374 2061  ........Select a
+00008dc0: 6c6c 0700 0000 094c 6f67 5669 6577 6572  ll.....LogViewer
+00008dd0: 0103 0000 0058 041d 0435 0438 0437 0432  .....X...5.8.7.2
+00008de0: 0435 0441 0442 043d 044b 0439 0020 043f  .5.A.B.=.K.9. .?
+00008df0: 0430 0440 0430 043c 0435 0442 0440 0020  .0.@.0.<.5.B.@. 
+00008e00: 043a 0440 0438 0442 0438 0447 043d 043e  .:.@.8.B.8.G.=.>
+00008e10: 0441 0442 0438 0020 0441 043e 043e 0431  .A.B.8. .A.>.>.1
+00008e20: 0449 0435 043d 0438 044f 003a 0020 0800  .I.5.=.8.O.:. ..
+00008e30: 0000 0006 0000 0020 556e 6b6e 6f77 6e20  ....... Unknown 
+00008e40: 6c6f 6767 696e 6720 6c65 7665 6c20 7072  logging level pr
+00008e50: 6f76 6964 6564 3a20 0700 0000 094c 6f67  ovided: .....Log
+00008e60: 5669 6577 6572 0103 0000 000c 25b2 0020  Viewer......%.. 
+00008e70: 006c 006f 0067 0073 0800 0000 0006 0000  .l.o.g.s........
+00008e80: 0008 e296 b220 6c6f 6773 0700 0000 094c  ..... logs.....L
+00008e90: 6f67 5669 6577 6572 0103 0000 000c 25b6  ogViewer......%.
+00008ea0: 0020 006c 006f 0067 0073 0800 0000 0006  . .l.o.g.s......
+00008eb0: 0000 0008 e296 b620 6c6f 6773 0700 0000  ....... logs....
+00008ec0: 094c 6f67 5669 6577 6572 0103 0000 003e  .LogViewer.....>
+00008ed0: 041e 0448 0438 0431 043a 0430 0020 043b  ...H.8.1.:.0. .;
+00008ee0: 043e 0433 0438 043d 0430 0020 0447 0435  .>.3.8.=.0. .G.5
+00008ef0: 0440 0435 0437 0020 0413 043e 0441 0443  .@.5.7. ...>.A.C
+00008f00: 0441 043b 0443 0433 0438 003a 0020 0800  .A.;.C.3.8.:. ..
+00008f10: 0000 0006 0000 0013 4553 4941 206c 6f67  ........ESIA log
+00008f20: 696e 2066 6169 6c65 643a 2007 0000 0008  in failed: .....
+00008f30: 4c6f 6769 6e46 4e53 0103 0000 0040 0423  LoginFNS.....@.#
+00008f40: 0441 043f 0435 0448 043d 044b 0439 0020  .A.?.5.H.=.K.9. 
+00008f50: 043b 043e 0433 0438 043d 0020 0447 0435  .;.>.3.8.=. .G.5
+00008f60: 0440 0435 0437 0020 0413 043e 0441 0443  .@.5.7. ...>.A.C
+00008f70: 0441 043b 0443 0433 0438 003a 0020 0800  .A.;.C.3.8.:. ..
+00008f80: 0000 0006 0000 0017 4553 4941 206c 6f67  ........ESIA log
+00008f90: 696e 2073 7563 6365 7373 6675 6c3a 2007  in successful: .
+00008fa0: 0000 0008 4c6f 6769 6e46 4e53 0103 0000  ....LoginFNS....
+00008fb0: 0038 041e 0448 0438 0431 043a 0430 0020  .8...H.8.1.:.0. 
+00008fc0: 043b 043e 0433 0438 043d 0430 0020 0447  .;.>.3.8.=.0. .G
+00008fd0: 0435 0440 0435 0437 0020 041b 041a 0020  .5.@.5.7. ..... 
+00008fe0: 0424 041d 0421 003a 0020 0800 0000 0006  .$...!.:. ......
+00008ff0: 0000 0012 464e 5320 6c6f 6769 6e20 6661  ....FNS login fa
+00009000: 696c 6564 3a20 0700 0000 084c 6f67 696e  iled: .....Login
+00009010: 464e 5301 0300 0000 3a04 2304 4104 3f04  FNS.....:.#.A.?.
+00009020: 3504 4804 3d04 4b04 3900 2004 3b04 3e04  5.H.=.K.9. .;.>.
+00009030: 3304 3804 3d00 2004 4704 3504 4004 3504  3.8.=. .G.5.@.5.
+00009040: 3700 2004 1b04 1a00 2004 2404 1d04 2100  7. ..... .$...!.
+00009050: 3a00 2008 0000 0000 0600 0000 1646 4e53  :. ..........FNS
+00009060: 206c 6f67 696e 2073 7563 6365 7373 6675   login successfu
+00009070: 6c3a 2007 0000 0008 4c6f 6769 6e46 4e53  l: .....LoginFNS
+00009080: 0103 0000 005a 041e 0448 0438 0431 043a  .....Z...H.8.1.:
+00009090: 0430 0020 043f 043e 043b 0443 0447 0435  .0. .?.>.;.C.G.5
+000090a0: 043d 0438 044f 0020 0055 0052 004c 0020  .=.8.O. .U.R.L. 
+000090b0: 043b 043e 0433 0438 043d 0430 0020 0447  .;.>.3.8.=.0. .G
+000090c0: 0435 0440 0435 0437 0020 0413 043e 0441  .5.@.5.7. ...>.A
+000090d0: 0443 0441 043b 0443 0433 0438 003a 0020  .C.A.;.C.3.8.:. 
+000090e0: 0800 0000 0006 0000 0015 4765 7420 4553  ..........Get ES
+000090f0: 4941 2055 524c 2066 6169 6c65 643a 2007  IA URL failed: .
+00009100: 0000 0008 4c6f 6769 6e46 4e53 0103 0000  ....LoginFNS....
+00009110: 0034 0053 004d 0053 0020 0431 044b 043b  .4.S.M.S. .1.K.;
+00009120: 043e 0020 0437 0430 043f 0440 043e 0448  .>. .7.0.?.@.>.H
+00009130: 0435 043d 043e 0020 0443 0441 043f 0435  .5.=.>. .C.A.?.5
+00009140: 0448 043d 043e 0800 0000 0006 0000 001e  .H.=.>..........
+00009150: 534d 5320 7761 7320 7265 7175 6573 7465  SMS was requeste
+00009160: 6420 7375 6363 6573 7366 756c 6c79 0700  d successfully..
+00009170: 0000 084c 6f67 696e 464e 5301 0300 0000  ...LoginFNS.....
+00009180: 1e04 1004 3204 4204 3e04 4004 3804 3704  ....2.B.>.@.8.7.
+00009190: 3004 4604 3804 4f00 2004 2404 1d04 2108  0.F.8.O. .$...!.
+000091a0: 0000 0000 0600 0000 1141 7574 686f 7269  .........Authori
+000091b0: 7a61 7469 6f6e 2046 4e53 0700 0000 0e4c  zation FNS.....L
+000091c0: 6f67 696e 464e 5344 6961 6c6f 6701 0300  oginFNSDialog...
+000091d0: 0000 0e04 1704 3004 3a04 4004 4b04 4204  ......0.:.@.K.B.
+000091e0: 4c08 0000 0000 0600 0000 0543 6c6f 7365  L..........Close
+000091f0: 0700 0000 0e4c 6f67 696e 464e 5344 6961  .....LoginFNSDia
+00009200: 6c6f 6701 0300 0000 1604 1a04 3e04 3400  log.........>.4.
+00009210: 2004 3804 3700 2000 5300 4d00 5300 3a08   .8.7. .S.M.S.:.
+00009220: 0000 0000 0600 0000 0e43 6f64 6520 6672  .........Code fr
+00009230: 6f6d 2053 4d53 3a07 0000 000e 4c6f 6769  om SMS:.....Logi
+00009240: 6e46 4e53 4469 616c 6f67 0103 0000 0012  nFNSDialog......
+00009250: 0413 043e 0441 0443 0441 043b 0443 0433  ...>.A.C.A.;.C.3
+00009260: 0438 0800 0000 0006 0000 000a 4553 4941  .8..........ESIA
+00009270: 204c 6f67 696e 0700 0000 0e4c 6f67 696e   Login.....Login
+00009280: 464e 5344 6961 6c6f 6701 0300 0000 0c04  FNSDialog.......
+00009290: 1b04 1a00 2004 2404 1d04 2108 0000 0000  .... .$...!.....
+000092a0: 0600 0000 0946 4e53 204c 6f67 696e 0700  .....FNS Login..
+000092b0: 0000 0e4c 6f67 696e 464e 5344 6961 6c6f  ...LoginFNSDialo
+000092c0: 6701 0300 0000 0804 1804 1d04 1d00 3a08  g.............:.
+000092d0: 0000 0000 0600 0000 0449 4e4e 3a07 0000  .........INN:...
+000092e0: 000e 4c6f 6769 6e46 4e53 4469 616c 6f67  ..LoginFNSDialog
+000092f0: 0103 0000 000a 041b 043e 0433 0438 043d  .........>.3.8.=
+00009300: 0800 0000 0006 0000 0005 4c6f 6769 6e07  ..........Login.
+00009310: 0000 000e 4c6f 6769 6e46 4e53 4469 616c  ....LoginFNSDial
+00009320: 6f67 0103 0000 000e 041f 0430 0440 043e  og.........0.@.>
+00009330: 043b 044c 003a 0800 0000 0006 0000 0009  .;.L.:..........
+00009340: 5061 7373 776f 7264 3a07 0000 000e 4c6f  Password:.....Lo
+00009350: 6769 6e46 4e53 4469 616c 6f67 0103 0000  ginFNSDialog....
+00009360: 001e 041d 043e 043c 0435 0440 0020 0442  .....>.<.5.@. .B
+00009370: 0435 043b 0435 0444 043e 043d 0430 003a  .5.;.5.D.>.=.0.:
+00009380: 0800 0000 0006 0000 000d 5068 6f6e 6520  ..........Phone 
+00009390: 6e75 6d62 6572 3a07 0000 000e 4c6f 6769  number:.....Logi
+000093a0: 6e46 4e53 4469 616c 6f67 0103 0000 0006  nFNSDialog......
+000093b0: 0053 004d 0053 0800 0000 0006 0000 0009  .S.M.S..........
+000093c0: 534d 5320 4c6f 6769 6e07 0000 000e 4c6f  SMS Login.....Lo
+000093d0: 6769 6e46 4e53 4469 616c 6f67 0103 0000  ginFNSDialog....
+000093e0: 0026 0412 044b 0441 043b 0430 0442 044c  .&...K.A.;.0.B.L
+000093f0: 0020 0053 004d 0053 0020 0441 0020 043a  . .S.M.S. .A. .:
+00009400: 043e 0434 043e 043c 0800 0000 0006 0000  .>.4.>.<........
+00009410: 0012 5365 6e64 2053 4d53 2077 6974 6820  ..Send SMS with 
+00009420: 636f 6465 0700 0000 0e4c 6f67 696e 464e  code.....LoginFN
+00009430: 5344 6961 6c6f 6701 0300 0000 1600 6100  SDialog.......a.
+00009440: 6200 6f00 7500 7400 3a00 6200 6c00 6100  b.o.u.t.:.b.l.a.
+00009450: 6e00 6b08 0000 0000 0600 0000 0b61 626f  n.k..........abo
+00009460: 7574 3a62 6c61 6e6b 0700 0000 0e4c 6f67  ut:blank.....Log
+00009470: 696e 464e 5344 6961 6c6f 6701 0300 0000  inFNSDialog.....
+00009480: 4404 1d04 3004 3904 3404 3504 3d04 3e00  D...0.9.4.5.=.>.
+00009490: 2004 3d04 3504 4104 3a04 3e04 3b04 4c04   .=.5.A.:.>.;.L.
+000094a0: 3a04 3e00 2004 2604 1100 2004 3d04 3000  :.>. .&... .=.0.
+000094b0: 2000 4d00 4f00 4500 5800 2004 3404 3b04   .M.O.E.X. .4.;.
+000094c0: 4f00 3a00 2008 0000 0000 0600 0000 204d  O.:. ......... M
+000094d0: 756c 7469 706c 6520 4d4f 4558 2061 7373  ultiple MOEX ass
+000094e0: 6574 7320 666f 756e 6420 666f 723a 2007  ets found for: .
+000094f0: 0000 0004 4d4f 4558 0103 0000 0044 041d  ....MOEX.....D..
+00009500: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+00009510: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
+00009520: 0442 0438 043f 0020 0426 0411 0020 041c  .B.8.?. .&... ..
+00009530: 043e 0441 0411 0438 0440 0436 0438 003a  .>.A...8.@.6.8.:
+00009540: 0020 0800 0000 0006 0000 0020 556e 7375  . ......... Unsu
+00009550: 7070 6f72 7465 6420 4d4f 4558 2073 6563  pported MOEX sec
+00009560: 7572 6974 7920 7479 7065 3a20 0700 0000  urity type: ....
+00009570: 044d 4f45 5801 0300 0000 1604 1e00 2004  .MOEX......... .
+00009580: 3f04 4004 3e04 3304 4004 3004 3c04 3c04  ?.@.>.3.@.0.<.<.
+00009590: 3508 0000 0000 0600 0000 0541 626f 7574  5..........About
+000095a0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+000095b0: 0300 0000 8804 1204 4104 3500 2004 3404  ........A.5. .4.
+000095c0: 3004 3d04 3d04 4b04 3500 2004 3104 4304  0.=.=.K.5. .1.C.
+000095d0: 3404 4304 4200 2004 4304 3404 3004 3b04  4.C.B. .C.4.0.;.
+000095e0: 3504 3d04 4b00 2004 3104 3504 3700 2004  5.=.K. .1.5.7. .
+000095f0: 3204 3e04 3704 3c04 3e04 3604 3d04 3e04  2.>.7.<.>.6.=.>.
+00009600: 4104 4204 3800 2004 3204 3e04 4104 4104  A.B.8. .2.>.A.A.
+00009610: 4204 3004 3d04 3e04 3204 3b04 3504 3d04  B.0.=.>.2.;.5.=.
+00009620: 3804 4f00 2e00 0a04 1204 4b00 2004 4304  8.O.......K. .C.
+00009630: 3204 3504 4004 3504 3d04 4b00 3f08 0000  2.5.@.5.=.K.?...
+00009640: 0000 0600 0000 4441 6c6c 2064 6174 6120  ......DAll data 
+00009650: 7769 6c6c 2062 6520 6465 6c65 7465 642e  will be deleted.
+00009660: 2054 6865 2061 6374 696f 6e73 2063 616e   The actions can
+00009670: 2774 2062 6520 756e 646f 6e65 2e0a 4172  't be undone..Ar
+00009680: 6520 796f 7520 7375 7265 3f07 0000 000a  e you sure?.....
+00009690: 4d61 696e 5769 6e64 6f77 0103 0000 001a  MainWindow......
+000096a0: 041f 043e 0434 0442 0432 0435 0440 0436  ...>.4.B.2.5.@.6
+000096b0: 0434 0435 043d 0438 0435 0800 0000 0006  .4.5.=.8.5......
+000096c0: 0000 000c 436f 6e66 6972 6d61 7469 6f6e  ....Confirmation
+000096d0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+000096e0: 0300 0000 aa04 1104 3004 3704 3000 2004  ........0.7.0. .
+000096f0: 3404 3004 3d04 3d04 4b04 4500 2004 3104  4.0.=.=.K.E. .1.
+00009700: 4304 3404 3504 4200 2004 3e04 4704 3804  C.4.5.B. .>.G.8.
+00009710: 4904 3504 3d04 3000 2004 3f04 4004 3800  I.5.=.0. .?.@.8.
+00009720: 2004 4104 3b04 3504 3404 4304 4e04 4904   .A.;.5.4.C.N.I.
+00009730: 3504 3c00 2004 3704 3004 3f04 4304 4104  5.<. .7.0.?.C.A.
+00009740: 3a04 3500 2000 4a00 4100 4c00 2e00 0a04  :.5. .J.A.L.....
+00009750: 2104 3504 3904 4704 3004 4100 2004 3f04  !.5.9.G.0.A. .?.
+00009760: 4004 3804 3b04 3e04 3604 3504 3d04 3804  @.8.;.>.6.5.=.8.
+00009770: 3500 2004 3104 4304 3404 3504 4200 2004  5. .1.C.4.5.B. .
+00009780: 3704 3004 3a04 4004 4b04 4204 3e00 2e08  7.0.:.@.K.B.>...
+00009790: 0000 0000 0600 0000 4f44 6174 6162 6173  ........ODatabas
+000097a0: 6520 7769 6c6c 2062 6520 7265 6d6f 7665  e will be remove
+000097b0: 6420 6174 206e 6578 7420 4a41 4c20 7374  d at next JAL st
+000097c0: 6172 742e 0a41 7070 6c69 6361 7469 6f6e  art..Application
+000097d0: 2077 696c 6c20 6265 2074 6572 6d69 6e61   will be termina
+000097e0: 7465 6420 6e6f 772e 0700 0000 0a4d 6169  ted now......Mai
+000097f0: 6e57 696e 646f 7701 0300 0000 1c04 1f04  nWindow.........
+00009800: 3e04 3b04 3d04 3004 4f00 2004 3e04 4704  >.;.=.0.O. .>.G.
+00009810: 3804 4104 4204 3a04 3008 0000 0000 0600  8.A.B.:.0.......
+00009820: 0000 0d46 756c 6c20 636c 6561 6e2d 7570  ...Full clean-up
+00009830: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00009840: 0300 0000 1404 1804 3d04 4404 3e04 4004  ........=.D.>.@.
+00009850: 3c04 3004 4604 3804 4f08 0000 0000 0600  <.0.F.8.O.......
+00009860: 0000 0449 6e66 6f07 0000 000a 4d61 696e  ...Info.....Main
+00009870: 5769 6e64 6f77 0103 0000 0028 042f 0437  Window.....(./.7
+00009880: 044b 043a 0020 0431 044b 043b 0020 0438  .K.:. .1.K.;. .8
+00009890: 0437 043c 0435 043d 0451 043d 0020 043d  .7.<.5.=.Q.=. .=
+000098a0: 0430 0020 0800 0000 0006 0000 0018 4c61  .0. ..........La
+000098b0: 6e67 7561 6765 2077 6173 2063 6861 6e67  nguage was chang
+000098c0: 6564 2074 6f20 0700 0000 0a4d 6169 6e57  ed to .....MainW
+000098d0: 696e 646f 7701 0300 0000 6204 1804 4204  indow.....b...B.
+000098e0: 3e04 3304 3800 2004 4204 4004 3004 3d04  >.3.8. .B.@.0.=.
+000098f0: 3704 3004 3a04 4604 3804 3900 2004 3d04  7.0.:.F.8.9. .=.
+00009900: 3504 3004 3a04 4204 4304 3004 3b04 4c04  5.0.:.B.C.0.;.L.
+00009910: 3d04 4b00 2e00 2004 1f04 3504 4004 3504  =.K... ...5.@.5.
+00009920: 4104 4704 3804 4204 3004 4204 4c00 2004  A.G.8.B.0.B.L. .
+00009930: 4104 3504 3904 4704 3004 4100 3f08 0000  A.5.9.G.0.A.?...
+00009940: 0000 0600 0000 264c 6564 6765 7220 6973  ......&Ledger is
+00009950: 6e27 7420 636f 6d70 6c65 7465 2e20 5265  n't complete. Re
+00009960: 6275 696c 6420 6974 206e 6f77 3f07 0000  build it now?...
+00009970: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
+00009980: 0080 0414 043e 043f 043e 043b 043d 0438  .....>.?.>.;.=.8
+00009990: 0442 0435 043b 044c 043d 0430 044f 0020  .B.5.;.L.=.0.O. 
+000099a0: 0438 043d 0444 043e 0440 043c 0430 0446  .8.=.D.>.@.<.0.F
+000099b0: 0438 044f 002c 0020 0438 043d 0441 0442  .8.O.,. .8.=.A.B
+000099c0: 0440 0443 043a 0446 0438 0438 002c 0020  .@.C.:.F.8.8.,. 
+000099d0: 0441 043e 043e 0431 0449 0435 043d 0438  .A.>.>.1.I.5.=.8
+000099e0: 044f 0020 043e 0020 043f 0440 043e 0431  .O. .>. .?.@.>.1
+000099f0: 043b 0435 043c 0430 0445 0020 043d 0430  .;.5.<.0.E. .=.0
+00009a00: 0020 0800 0000 0006 0000 0035 4d6f 7265  . .........5More
+00009a10: 2069 6e66 6f72 6d61 7469 6f6e 2c20 6d61   information, ma
+00009a20: 6e75 616c 7320 616e 6420 7072 6f62 6c65  nuals and proble
+00009a30: 6d20 7265 706f 7274 7320 6172 6520 6174  m reports are at
+00009a40: 2007 0000 000a 4d61 696e 5769 6e64 6f77   .....MainWindow
+00009a50: 0103 0000 0050 0412 043e 043f 0440 043e  .....P...>.?.@.>
+00009a60: 0441 044b 002c 0020 043a 043e 043c 043c  .A.K.,. .:.>.<.<
+00009a70: 0435 043d 0442 0430 0440 0438 0438 002c  .5.=.B.0.@.8.8.,
+00009a80: 0020 043f 043e 043c 043e 0449 044c 0020  . .?.>.<.>.I.L. 
+00009a90: 0438 043b 0438 0020 0434 043e 043d 0430  .8.;.8. .4.>.=.0
+00009aa0: 0442 044b 003a 0800 0000 0006 0000 0027  .B.K.:.........'
+00009ab0: 5175 6573 7469 6f6e 732c 2063 6f6d 6d65  Questions, comme
+00009ac0: 6e74 732c 2068 656c 7020 6f72 2064 6f6e  nts, help or don
+00009ad0: 6174 696f 6e73 3a07 0000 000a 4d61 696e  ations:.....Main
+00009ae0: 5769 6e64 6f77 0103 0000 0022 0422 0440  Window.....".".@
+00009af0: 0435 0431 0443 0435 0442 0441 044f 0020  .5.1.C.5.B.A.O. 
+00009b00: 0440 0435 0441 0442 0430 0440 0442 0800  .@.5.A.B.0.@.B..
+00009b10: 0000 0006 0000 0010 5265 7374 6172 7420  ........Restart 
+00009b20: 7265 7175 6972 6564 0700 0000 0a4d 6169  required.....Mai
+00009b30: 6e57 696e 646f 7701 0300 0000 5004 1a04  nWindow.....P...
+00009b40: 3e04 3d04 3504 4704 3d04 4b04 3900 2004  >.=.5.G.=.K.9. .
+00009b50: 3104 3004 3b04 3004 3d04 4100 2004 3f04  1.0.;.0.=.A. .?.
+00009b60: 3e00 2004 3e04 4204 4704 5104 4204 4300  >. .>.B.G.Q.B.C.
+00009b70: 2004 3d04 3500 2004 4104 3e04 3204 3f04   .=.5. .A.>.2.?.
+00009b80: 3004 3404 3004 3504 4200 3a00 2008 0000  0.4.0.5.B.:. ...
+00009b90: 0000 0600 0000 2853 7461 7465 6d65 6e74  ......(Statement
+00009ba0: 2065 6e64 696e 6720 6261 6c61 6e63 6520   ending balance 
+00009bb0: 646f 6573 6e27 7420 6d61 7463 683a 2007  doesn't match: .
+00009bc0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00009bd0: 0000 00b2 041d 0443 0436 043d 043e 0020  .......C.6.=.>. 
+00009be0: 043f 0435 0440 0435 0437 0430 043f 0443  .?.5.@.5.7.0.?.C
+00009bf0: 0441 0442 0438 0442 044c 0020 043f 0440  .A.B.8.B.L. .?.@
+00009c00: 0438 043b 043e 0436 0435 043d 0438 0435  .8.;.>.6.5.=.8.5
+00009c10: 0020 0434 043b 044f 0020 043f 0440 0438  . .4.;.O. .?.@.8
+00009c20: 043c 0435 043d 0435 043d 0438 044f 0020  .<.5.=.5.=.8.O. 
+00009c30: 0438 0437 043c 0435 043d 0435 043d 0438  .8.7.<.5.=.5.=.8
+00009c40: 0439 002e 000a 0421 0435 0439 0447 0430  .9.....!.5.9.G.0
+00009c50: 0441 0020 043f 0440 0438 043b 043e 0436  .A. .?.@.8.;.>.6
+00009c60: 0435 043d 0438 0435 0020 0431 0443 0434  .5.=.8.5. .1.C.4
+00009c70: 0435 0442 0020 0437 0430 043a 0440 044b  .5.B. .7.0.:.@.K
+00009c80: 0442 043e 002e 0800 0000 0006 0000 0054  .B.>...........T
+00009c90: 596f 7520 7368 6f75 6c64 2072 6573 7461  You should resta
+00009ca0: 7274 2061 7070 6c69 6361 7469 6f6e 2074  rt application t
+00009cb0: 6f20 6170 706c 7920 6368 616e 6765 732e  o apply changes.
+00009cc0: 0a41 7070 6c69 6361 7469 6f6e 2077 696c  .Application wil
+00009cd0: 6c20 6265 2074 6572 6d69 6e61 7465 6420  l be terminated 
+00009ce0: 6e6f 772e 0700 0000 0a4d 6169 6e57 696e  now......MainWin
+00009cf0: 646f 7701 0300 0000 3004 3404 3e04 3c04  dow.....0.4.>.<.
+00009d00: 3004 4804 3d04 3504 3900 2004 4104 4204  0.H.=.5.9. .A.B.
+00009d10: 4004 3004 3d04 3804 4604 3500 2000 6700  @.0.=.8.F.5. .g.
+00009d20: 6900 7400 6800 7500 6208 0000 0000 0600  i.t.h.u.b.......
+00009d30: 0000 1067 6974 6875 6220 686f 6d65 2070  ...github home p
+00009d40: 6167 6507 0000 000a 4d61 696e 5769 6e64  age.....MainWind
+00009d50: 6f77 0103 0000 000c 0432 0435 0440 0441  ow.......2.5.@.A
+00009d60: 0438 044f 0800 0000 0006 0000 0007 7665  .8.O..........ve
+00009d70: 7273 696f 6e07 0000 000a 4d61 696e 5769  rsion.....MainWi
+00009d80: 6e64 6f77 0103 0000 0006 002e 002e 002e  ndow............
+00009d90: 0800 0000 0006 0000 0003 2e2e 2e07 0000  ................
+00009da0: 000f 4d6f 6e65 7946 6c6f 7757 6964 6765  ..MoneyFlowWidge
+00009db0: 7401 0300 0000 1604 2404 3004 3904 3b00  t.......$.0.9.;.
+00009dc0: 2000 4500 7800 6300 6500 6c00 3a08 0000   .E.x.c.e.l.:...
+00009dd0: 0000 0600 0000 0b45 7863 656c 2066 696c  .......Excel fil
+00009de0: 653a 0700 0000 0f4d 6f6e 6579 466c 6f77  e:.....MoneyFlow
+00009df0: 5769 6467 6574 0103 0000 0028 0424 0430  Widget.....(.$.0
+00009e00: 0439 043b 044b 0020 0045 0078 0063 0065  .9.;.K. .E.x.c.e
+00009e10: 006c 0020 0028 002a 002e 0078 0073 006c  .l. .(.*...x.s.l
+00009e20: 0078 0029 0800 0000 0006 0000 0014 4578  .x.)..........Ex
+00009e30: 6365 6c20 6669 6c65 7320 282a 2e78 6c73  cel files (*.xls
+00009e40: 7829 0700 0000 0f4d 6f6e 6579 466c 6f77  x).....MoneyFlow
+00009e50: 5769 6467 6574 0103 0000 0056 0424 0430  Widget.....V.$.0
+00009e60: 0439 043b 0020 0434 043b 044f 0020 0441  .9.;. .4.;.O. .A
+00009e70: 043e 0445 0440 0430 043d 0435 043d 0438  .>.E.@.0.=.5.=.8
+00009e80: 044f 0020 0440 0430 0441 0447 0451 0442  .O. .@.0.A.G.Q.B
+00009e90: 0430 0020 0432 0020 0444 043e 0440 043c  .0. .2. .D.>.@.<
+00009ea0: 0430 0442 0435 0020 0045 0078 0063 0065  .0.B.5. .E.x.c.e
+00009eb0: 006c 0800 0000 0006 0000 002e 4669 6c65  .l..........File
+00009ec0: 2077 6865 7265 2074 6f20 7374 6f72 6520   where to store 
+00009ed0: 7461 7820 7265 706f 7274 2069 6e20 4578  tax report in Ex
+00009ee0: 6365 6c20 666f 726d 6174 0700 0000 0f4d  cel format.....M
+00009ef0: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
+00009f00: 0000 000a 041e 043e 0414 0414 0421 0800  .......>.....!..
+00009f10: 0000 0006 0000 000a 4d6f 6e65 7920 466c  ........Money Fl
+00009f20: 6f77 0700 0000 0f4d 6f6e 6579 466c 6f77  ow.....MoneyFlow
+00009f30: 5769 6467 6574 0103 0000 002e 041e 043e  Widget.........>
+00009f40: 0414 0414 0421 0020 0441 043e 0445 0440  .....!. .A.>.E.@
+00009f50: 0430 043d 0451 043d 0020 0432 0020 0444  .0.=.Q.=. .2. .D
+00009f60: 0430 0439 043b 0435 0020 0800 0000 0006  .0.9.;.5. ......
+00009f70: 0000 0020 4d6f 6e65 7920 666c 6f77 2072  ... Money flow r
+00009f80: 6570 6f72 7420 7361 7665 6420 746f 2066  eport saved to f
+00009f90: 696c 6520 0700 0000 0f4d 6f6e 6579 466c  ile .....MoneyFl
+00009fa0: 6f77 5769 6467 6574 0103 0000 001e 0421  owWidget.......!
+00009fb0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+00009fc0: 0020 041e 0442 0447 0451 0442 0800 0000  . ...B.G.Q.B....
+00009fd0: 0006 0000 000b 5361 7665 2052 6570 6f72  ......Save Repor
+00009fe0: 7407 0000 000f 4d6f 6e65 7946 6c6f 7757  t.....MoneyFlowW
+00009ff0: 6964 6765 7401 0300 0000 2404 2104 3e04  idget.....$.!.>.
+0000a000: 4504 4004 3004 3d04 3804 4204 4c00 2004  E.@.0.=.8.B.L. .
+0000a010: 1e04 3e04 1404 1404 2100 2004 3200 3a08  ..>.....!. .2.:.
+0000a020: 0000 0000 0600 0000 1a53 6176 6520 6d6f  .........Save mo
+0000a030: 6e65 7920 666c 6f77 2072 6570 6f72 7420  ney flow report 
+0000a040: 746f 3a07 0000 000f 4d6f 6e65 7946 6c6f  to:.....MoneyFlo
+0000a050: 7757 6964 6765 7401 0300 0000 1804 1204  wWidget.........
+0000a060: 4b04 3104 3504 4004 3804 4200 2004 4404  K.1.5.@.8.B. .D.
+0000a070: 3004 3904 3b08 0000 0000 0600 0000 0b53  0.9.;..........S
+0000a080: 656c 6563 7420 6669 6c65 0700 0000 0f4d  elect file.....M
+0000a090: 6f6e 6579 466c 6f77 5769 6467 6574 0103  oneyFlowWidget..
+0000a0a0: 0000 0008 0413 043e 0434 003a 0800 0000  .......>.4.:....
+0000a0b0: 0006 0000 0005 5965 6172 3a07 0000 000f  ......Year:.....
+0000a0c0: 4d6f 6e65 7946 6c6f 7757 6964 6765 7401  MoneyFlowWidget.
+0000a0d0: 0300 0000 2800 2004 3d04 3504 4304 4104  ....(. .=.5.C.A.
+0000a0e0: 3f04 3504 4804 3d04 4b04 3900 2004 3704  ?.5.H.=.K.9. .7.
+0000a0f0: 3004 3f04 4004 3e04 4100 3a00 2008 0000  0.?.@.>.A.:. ...
+0000a100: 0000 0600 0000 0920 6661 696c 6564 3a20  ....... failed: 
+0000a110: 0700 0000 034e 6574 0103 0000 0034 0422  .....Net.....4."
+0000a120: 0438 043f 0020 0426 0411 0020 043d 0435  .8.?. .&... .=.5
+0000a130: 0020 043f 043e 0434 0434 0435 0440 0436  . .?.>.4.4.5.@.6
+0000a140: 0438 0432 0430 0435 0442 0441 044f 003a  .8.2.0.5.B.A.O.:
+0000a150: 0020 0800 0000 0006 0000 001c 4173 7365  . ..........Asse
+0000a160: 7420 7479 7065 2069 736e 2774 2073 7570  t type isn't sup
+0000a170: 706f 7274 6564 3a20 0700 0000 0a4f 7065  ported: .....Ope
+0000a180: 6e42 726f 6b65 7201 0300 0000 3204 1104  nBroker.....2...
+0000a190: 3804 4004 3604 3000 2004 3d04 3500 2004  8.@.6.0. .=.5. .
+0000a1a0: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+0000a1b0: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
+0000a1c0: 0000 0000 0600 0000 1a45 7863 6861 6e67  .........Exchang
+0000a1d0: 6520 6973 6e27 7420 7375 7070 6f72 7465  e isn't supporte
+0000a1e0: 643a 2007 0000 000a 4f70 656e 4272 6f6b  d: .....OpenBrok
+0000a1f0: 6572 0103 0000 0008 0421 0447 0435 0442  er.......!.G.5.B
+0000a200: 0800 0000 0006 0000 0007 4163 636f 756e  ..........Accoun
+0000a210: 7407 0000 000f 4f70 6572 6174 696f 6e73  t.....Operations
+0000a220: 4d6f 6465 6c01 0300 0000 0a04 2104 4304  Model.......!.C.
+0000a230: 3c04 3c04 3008 0000 0000 0600 0000 0641  <.<.0..........A
+0000a240: 6d6f 756e 7407 0000 000f 4f70 6572 6174  mount.....Operat
+0000a250: 696f 6e73 4d6f 6465 6c01 0300 0000 0c04  ionsModel.......
+0000a260: 1104 3004 3b04 3004 3d04 4108 0000 0000  ..0.;.0.=.A.....
+0000a270: 0600 0000 0742 616c 616e 6365 0700 0000  .....Balance....
+0000a280: 0f4f 7065 7261 7469 6f6e 734d 6f64 656c  .OperationsModel
+0000a290: 0103 0000 000c 0412 0430 043b 044e 0442  .........0.;.N.B
+0000a2a0: 0430 0800 0000 0006 0000 0008 4375 7272  .0..........Curr
+0000a2b0: 656e 6379 0700 0000 0f4f 7065 7261 7469  ency.....Operati
+0000a2c0: 6f6e 734d 6f64 656c 0103 0000 0010 041e  onsModel........
+0000a2d0: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
+0000a2e0: 0000 0006 0000 0005 4e6f 7465 7307 0000  ........Notes...
+0000a2f0: 000f 4f70 6572 6174 696f 6e73 4d6f 6465  ..OperationsMode
+0000a300: 6c01 0300 0000 1404 1404 3004 4204 3000  l.........0.B.0.
+0000a310: 2f04 1204 4004 3504 3c04 4f08 0000 0000  /...@.5.<.O.....
+0000a320: 0600 0000 0954 696d 6573 7461 6d70 0700  .....Timestamp..
+0000a330: 0000 0f4f 7065 7261 7469 6f6e 734d 6f64  ...OperationsMod
+0000a340: 656c 0103 0000 000a 0421 0447 0435 0442  el.......!.G.5.B
+0000a350: 003a 0800 0000 0006 0000 0008 4163 636f  .:..........Acco
+0000a360: 756e 743a 0700 0000 104f 7065 7261 7469  unt:.....Operati
+0000a370: 6f6e 7357 6964 6765 7401 0300 0000 4a04  onsWidget.....J.
+0000a380: 1204 4b00 2004 4504 3e04 4204 3804 4204  ..K. .E.>.B.8.B.
+0000a390: 3500 2004 4304 3404 3004 3b04 3804 4204  5. .C.4.0.;.8.B.
+0000a3a0: 4c00 2004 3204 4b04 3104 4004 3004 3d04  L. .2.K.1.@.0.=.
+0000a3b0: 3d04 4b04 3500 2004 3e04 3f04 3504 4004  =.K.5. .>.?.5.@.
+0000a3c0: 3004 4604 3804 3800 3f08 0000 0000 0600  0.F.8.8.?.......
+0000a3d0: 0000 2e41 7265 2079 6f75 2073 7572 6520  ...Are you sure 
+0000a3e0: 746f 2064 656c 6574 6520 7365 6c65 6374  to delete select
+0000a3f0: 6564 2074 7261 6e73 6163 696f 6e28 7329  ed transacion(s)
+0000a400: 3f07 0000 0010 4f70 6572 6174 696f 6e73  ?.....Operations
+0000a410: 5769 6467 6574 0103 0000 001c 0411 0430  Widget.........0
+0000a420: 043b 0430 043d 0441 044b 0020 0441 0447  .;.0.=.A.K. .A.G
+0000a430: 0435 0442 043e 0432 0800 0000 0006 0000  .5.B.>.2........
+0000a440: 0008 4261 6c61 6e63 6573 0700 0000 104f  ..Balances.....O
+0000a450: 7065 7261 7469 6f6e 7357 6964 6765 7401  perationsWidget.
+0000a460: 0300 0000 1a04 1f04 3e04 3404 4204 3204  ........>.4.B.2.
+0000a470: 3504 4004 3604 3404 3504 3d04 3804 3508  5.@.6.4.5.=.8.5.
+0000a480: 0000 0000 0600 0000 0c43 6f6e 6669 726d  .........Confirm
+0000a490: 6174 696f 6e07 0000 0010 4f70 6572 6174  ation.....Operat
+0000a4a0: 696f 6e73 5769 6467 6574 0103 0000 0014  ionsWidget......
+0000a4b0: 041a 043e 043f 0438 0440 043e 0432 0430  ...>.?.8.@.>.2.0
+0000a4c0: 0442 044c 0800 0000 0006 0000 0004 436f  .B.L..........Co
+0000a4d0: 7079 0700 0000 104f 7065 7261 7469 6f6e  py.....Operation
+0000a4e0: 7357 6964 6765 7401 0300 0000 2604 1a04  sWidget.....&...
+0000a4f0: 3e04 3f04 3804 4004 3e04 3204 3004 4204  >.?.8.@.>.2.0.B.
+0000a500: 4c00 2004 3e04 3f04 3504 4004 3004 4604  L. .>.?.5.@.0.F.
+0000a510: 3804 4e08 0000 0000 0600 0000 0e43 6f70  8.N..........Cop
+0000a520: 7920 6f70 6572 6174 696f 6e07 0000 0010  y operation.....
+0000a530: 4f70 6572 6174 696f 6e73 5769 6467 6574  OperationsWidget
+0000a540: 0103 0000 000e 0423 0434 0430 043b 0438  .......#.4.0.;.8
+0000a550: 0442 044c 0800 0000 0006 0000 0006 4465  .B.L..........De
+0000a560: 6c65 7465 0700 0000 104f 7065 7261 7469  lete.....Operati
+0000a570: 6f6e 7357 6964 6765 7401 0300 0000 2004  onsWidget..... .
+0000a580: 2304 3404 3004 3b04 3804 4204 4c00 2004  #.4.0.;.8.B.L. .
+0000a590: 3e04 3f04 3504 4004 3004 4604 3804 4e08  >.?.5.@.0.F.8.N.
+0000a5a0: 0000 0000 0600 0000 1044 656c 6574 6520  .........Delete 
+0000a5b0: 6f70 6572 6174 696f 6e07 0000 0010 4f70  operation.....Op
+0000a5c0: 6572 6174 696f 6e73 5769 6467 6574 0103  erationsWidget..
+0000a5d0: 0000 001c 041d 043e 0432 0430 044f 0020  .......>.2.0.O. 
+0000a5e0: 043e 043f 0435 0440 0430 0446 0438 044f  .>.?.5.@.0.F.8.O
+0000a5f0: 0800 0000 0006 0000 000d 4e65 7720 6f70  ..........New op
+0000a600: 6572 6174 696f 6e07 0000 0010 4f70 6572  eration.....Oper
+0000a610: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
+0000a620: 0010 041e 043f 0435 0440 0430 0446 0438  .....?.5.@.0.F.8
+0000a630: 0438 0800 0000 0006 0000 000a 4f70 6572  .8..........Oper
+0000a640: 6174 696f 6e73 0700 0000 104f 7065 7261  ations.....Opera
+0000a650: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
+0000a660: 2404 1e04 3f04 3504 4004 3004 4604 3804  $...?.5.@.0.F.8.
+0000a670: 3800 2004 3800 2004 1104 3004 3b04 3004  8. .8. ...0.;.0.
+0000a680: 3d04 4104 4b08 0000 0000 0600 0000 154f  =.A.K..........O
+0000a690: 7065 7261 7469 6f6e 7320 2620 4261 6c61  perations & Bala
+0000a6a0: 6e63 6573 0700 0000 104f 7065 7261 7469  nces.....Operati
+0000a6b0: 6f6e 7357 6964 6765 7401 0300 0000 0e04  onsWidget.......
+0000a6c0: 2104 3204 3504 4004 3804 4204 4c08 0000  !.2.5.@.8.B.L...
+0000a6d0: 0000 0600 0000 0952 6563 6f6e 6369 6c65  .......Reconcile
+0000a6e0: 0700 0000 104f 7065 7261 7469 6f6e 7357  .....OperationsW
+0000a6f0: 6964 6765 7401 0300 0000 0c04 1f04 3e04  idget.........>.
+0000a700: 3804 4104 3a00 3a08 0000 0000 0600 0000  8.A.:.:.........
+0000a710: 0753 6561 7263 683a 0700 0000 104f 7065  .Search:.....Ope
+0000a720: 7261 7469 6f6e 7357 6964 6765 7401 0300  rationsWidget...
+0000a730: 0000 2c04 1f04 3e04 3a04 3004 3704 4b04  ..,...>.:.0.7.K.
+0000a740: 3204 3004 4204 4c00 2000 2604 3d04 3504  2.0.B.L. .&.=.5.
+0000a750: 3004 3a04 4204 3804 3204 3d04 4b04 3508  0.:.B.8.2.=.K.5.
+0000a760: 0000 0000 0600 0000 0e53 686f 7720 2649  .........Show &I
+0000a770: 6e61 6374 6976 6507 0000 0010 4f70 6572  nactive.....Oper
+0000a780: 6174 696f 6e73 5769 6467 6574 0103 0000  ationsWidget....
+0000a790: 001a 0412 0430 043b 044e 0442 0430 0020  .....0.;.N.B.0. 
+0000a7a0: 0438 0442 043e 0433 043e 003a 0800 0000  .8.B.>.3.>.:....
+0000a7b0: 0006 0000 000d 5375 6d20 4375 7272 656e  ......Sum Curren
+0000a7c0: 6379 3a07 0000 0010 4f70 6572 6174 696f  cy:.....Operatio
+0000a7d0: 6e73 5769 6467 6574 0103 0000 0014 0064  nsWidget.......d
+0000a7e0: 0064 002f 004d 004d 002f 0079 0079 0079  .d./.M.M./.y.y.y
+0000a7f0: 0079 0800 0000 0006 0000 000a 6464 2f4d  .y..........dd/M
+0000a800: 4d2f 7979 7979 0700 0000 104f 7065 7261  M/yyyy.....Opera
+0000a810: 7469 6f6e 7357 6964 6765 7401 0300 0000  tionsWidget.....
+0000a820: 0c04 1204 3004 3b04 4e04 4204 3008 0000  ....0.;.N.B.0...
+0000a830: 0000 0600 0000 0843 7572 7265 6e63 7907  .......Currency.
+0000a840: 0000 0018 4f70 7469 6f6e 616c 4375 7272  ....OptionalCurr
+0000a850: 656e 6379 436f 6d62 6f42 6f78 0103 0000  encyComboBox....
+0000a860: 000a 0421 0443 043c 043c 0430 0800 0000  ...!.C.<.<.0....
+0000a870: 0006 0000 0006 416d 6f75 6e74 0700 0000  ......Amount....
+0000a880: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
+0000a890: 6c01 0300 0000 1204 1a04 3004 4204 3504  l.........0.B.5.
+0000a8a0: 3304 3e04 4004 3804 4f08 0000 0000 0600  3.>.@.8.O.......
+0000a8b0: 0000 0843 6174 6567 6f72 7907 0000 0010  ...Category.....
+0000a8c0: 5061 6e64 6173 4c69 6e65 734d 6f64 656c  PandasLinesModel
+0000a8d0: 0103 0000 0022 041d 0430 0437 0432 0430  ....."...0.7.2.0
+0000a8e0: 043d 0438 0435 0020 043f 0440 043e 0434  .=.8.5. .?.@.>.4
+0000a8f0: 0443 043a 0442 0430 0800 0000 0006 0000  .C.:.B.0........
+0000a900: 000c 5072 6f64 7563 7420 6e61 6d65 0700  ..Product name..
+0000a910: 0000 1050 616e 6461 734c 696e 6573 4d6f  ...PandasLinesMo
+0000a920: 6465 6c01 0300 0000 0604 2204 4d04 3308  del.......".M.3.
+0000a930: 0000 0000 0600 0000 0354 6167 0700 0000  .........Tag....
+0000a940: 1050 616e 6461 734c 696e 6573 4d6f 6465  .PandasLinesMode
+0000a950: 6c01 0300 0000 2400 2700 2004 3704 3004  l.....$.'. .7.0.
+0000a960: 3c04 3504 3d04 3504 3d04 3000 2004 4304  <.5.=.5.=.0. .C.
+0000a970: 4104 3f04 3504 4804 3d04 3e08 0000 0000  A.?.5.H.=.>.....
+0000a980: 0600 0000 1b27 2077 6173 2073 7563 6365  .....' was succe
+0000a990: 7373 6675 6c6c 7920 7265 706c 6163 6564  ssfully replaced
+0000a9a0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
+0000a9b0: 6c6f 6701 0300 0000 0c00 2700 2004 3d04  log.......'. .=.
+0000a9c0: 3000 3a00 2008 0000 0000 0600 0000 0827  0.:. ..........'
+0000a9d0: 2077 6974 683a 2007 0000 000e 5065 6572   with: .....Peer
+0000a9e0: 4c69 7374 4469 616c 6f67 0103 0000 004e  ListDialog.....N
+0000a9f0: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
+0000aa00: 044c 0020 0441 0442 0430 0440 043e 0435  .L. .A.B.0.@.>.5
+0000aa10: 0020 043d 0430 0437 0432 0430 043d 0438  . .=.0.7.2.0.=.8
+0000aa20: 0435 0020 0432 0020 043f 0440 0438 043c  .5. .2. .?.@.8.<
+0000aa30: 0435 0447 0430 043d 0438 0438 003f 0800  .5.G.0.=.8.8.?..
+0000aa40: 0000 0006 0000 0017 4b65 6570 206f 6c64  ........Keep old
+0000aa50: 206e 616d 6520 696e 206e 6f74 6573 3f07   name in notes?.
+0000aa60: 0000 000e 5065 6572 4c69 7374 4469 616c  ....PeerListDial
+0000aa70: 6f67 0103 0000 0018 041a 043e 043d 0442  og.........>.=.B
+0000aa80: 0440 0430 0433 0435 043d 0442 0020 0027  .@.0.3.5.=.B. .'
+0000aa90: 0800 0000 0006 0000 0006 5065 6572 2027  ..........Peer '
+0000aaa0: 0700 0000 0e50 6565 724c 6973 7444 6961  .....PeerListDia
+0000aab0: 6c6f 6701 0300 0000 1604 1a04 3e04 3d04  log.........>.=.
+0000aac0: 4204 4004 3004 3304 3504 3d04 4204 4b08  B.@.0.3.5.=.B.K.
+0000aad0: 0000 0000 0600 0000 0550 6565 7273 0700  .........Peers..
+0000aae0: 0000 0e50 6565 724c 6973 7444 6961 6c6f  ...PeerListDialo
+0000aaf0: 6701 0300 0000 2c04 1704 3004 3c04 3504  g.....,...0.<.5.
+0000ab00: 3d04 3804 4204 4c00 2004 3a04 3e04 3d04  =.8.B.L. .:.>.=.
+0000ab10: 4204 4004 3004 3304 3504 3d04 4204 3000  B.@.0.3.5.=.B.0.
+0000ab20: 2000 2708 0000 0000 0600 0000 0e52 6570   .'..........Rep
+0000ab30: 6c61 6365 2070 6565 7220 2707 0000 000e  lace peer '.....
+0000ab40: 5065 6572 4c69 7374 4469 616c 6f67 0103  PeerListDialog..
+0000ab50: 0000 001c 0417 0430 043c 0435 043d 0438  .......0.<.5.=.8
+0000ab60: 0442 044c 0020 043d 0430 002e 002e 002e  .B.L. .=.0......
+0000ab70: 0800 0000 0006 0000 000f 5265 706c 6163  ..........Replac
+0000ab80: 6520 7769 7468 2e2e 2e07 0000 000e 5065  e with........Pe
+0000ab90: 6572 4c69 7374 4469 616c 6f67 0103 0000  erListDialog....
+0000aba0: 0040 041f 043e 043a 0430 0437 0430 0442  .@...>.:.0.7.0.B
+0000abb0: 044c 0020 043e 043f 0435 0440 0430 0446  .L. .>.?.5.@.0.F
+0000abc0: 0438 0438 0020 0441 0020 041a 043e 043d  .8.8. .A. ...>.=
+0000abd0: 0442 0440 0430 0433 0435 043d 0442 043e  .B.@.0.3.5.=.B.>
+0000abe0: 043c 0800 0000 0006 0000 0019 5368 6f77  .<..........Show
+0000abf0: 206f 7065 7261 7469 6f6e 7320 7769 7468   operations with
+0000ac00: 2050 6565 7207 0000 000e 5065 6572 4c69   Peer.....PeerLi
+0000ac10: 7374 4469 616c 6f67 0103 0000 0010 041e  stDialog........
+0000ac20: 043f 0435 0440 0430 0446 0438 0438 0800  .?.5.@.0.F.8.8..
+0000ac30: 0000 0006 0000 000a 4f70 6572 6174 696f  ........Operatio
+0000ac40: 6e73 0700 0000 0a50 6565 7252 6570 6f72  ns.....PeerRepor
+0000ac50: 7401 0300 0000 1c04 3f04 3e00 2004 1a04  t.......?.>. ...
+0000ac60: 3e04 3d04 4204 4004 3004 3304 3504 3d04  >.=.B.@.0.3.5.=.
+0000ac70: 4204 4308 0000 0000 0600 0000 0762 7920  B.C..........by 
+0000ac80: 5065 6572 0700 0000 0a50 6565 7252 6570  Peer.....PeerRep
+0000ac90: 6f72 7401 0300 0000 1604 1a04 3e04 3d04  ort.........>.=.
+0000aca0: 4204 4004 3004 3304 3504 3d04 4200 3a08  B.@.0.3.5.=.B.:.
+0000acb0: 0000 0000 0600 0000 0550 6565 723a 0700  .........Peer:..
+0000acc0: 0000 1050 6565 7252 6570 6f72 7457 6964  ...PeerReportWid
+0000acd0: 6765 7401 0300 0000 2804 1e04 4204 4704  get.....(...B.G.
+0000ace0: 3504 4200 2004 3f04 3e00 2004 3a04 3e04  5.B. .?.>. .:.>.
+0000acf0: 3d04 4204 4004 3004 3304 3504 3d04 4204  =.B.@.0.3.5.=.B.
+0000ad00: 4308 0000 0000 0600 0000 0e52 6570 6f72  C..........Repor
+0000ad10: 7420 6279 2070 6565 7207 0000 0010 5065  t by peer.....Pe
+0000ad20: 6572 5265 706f 7274 5769 6467 6574 0103  erReportWidget..
+0000ad30: 0000 0016 041a 043e 043b 002d 0432 043e  .......>.;.-.2.>
+0000ad40: 0020 0434 043e 043a 002e 0800 0000 0006  . .4.>.:........
+0000ad50: 0000 000a 446f 6373 2063 6f75 6e74 0700  ....Docs count..
+0000ad60: 0000 0d50 6565 7254 7265 654d 6f64 656c  ...PeerTreeModel
+0000ad70: 0103 0000 000a 0410 0434 0440 0435 0441  .........4.@.5.A
+0000ad80: 0800 0000 0006 0000 0008 4c6f 6361 7469  ..........Locati
+0000ad90: 6f6e 0700 0000 0d50 6565 7254 7265 654d  on.....PeerTreeM
+0000ada0: 6f64 656c 0103 0000 0018 041d 0430 0438  odel.........0.8
+0000adb0: 043c 0435 043d 043e 0432 0430 043d 0438  .<.5.=.>.2.0.=.8
+0000adc0: 0435 0800 0000 0006 0000 0004 4e61 6d65  .5..........Name
+0000add0: 0700 0000 0d50 6565 7254 7265 654d 6f64  .....PeerTreeMod
+0000ade0: 656c 0103 0000 001a 0421 0447 0435 0442  el.......!.G.5.B
+0000adf0: 0430 0020 0432 0020 0431 0430 043d 043a  .0. .2. .1.0.=.:
+0000ae00: 0435 0800 0000 0006 0000 000d 4261 6e6b  .5..........Bank
+0000ae10: 2061 6363 6f75 6e74 7307 0000 0016 5072   accounts.....Pr
+0000ae20: 6564 6566 696e 6465 6441 6363 6f75 6e74  edefindedAccount
+0000ae30: 5479 7065 0103 0000 000a 041a 0430 0440  Type.........0.@
+0000ae40: 0442 044b 0800 0000 0006 0000 0005 4361  .B.K..........Ca
+0000ae50: 7264 7307 0000 0016 5072 6564 6566 696e  rds.....Predefin
+0000ae60: 6465 6441 6363 6f75 6e74 5479 7065 0103  dedAccountType..
+0000ae70: 0000 0010 041d 0430 043b 0438 0447 043d  .......0.;.8.G.=
+0000ae80: 044b 0435 0800 0000 0006 0000 0004 4361  .K.5..........Ca
+0000ae90: 7368 0700 0000 1650 7265 6465 6669 6e64  sh.....Predefind
+0000aea0: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
+0000aeb0: 0000 1e04 1a04 4004 3504 3404 3804 4204  ......@.5.4.8.B.
+0000aec0: 4b00 2000 2f00 2004 1404 3e04 3b04 3304  K. ./. ...>.;.3.
+0000aed0: 3808 0000 0000 0600 0000 0d44 6562 7473  8..........Debts
+0000aee0: 202f 204c 6f61 6e73 0700 0000 1650 7265   / Loans.....Pre
+0000aef0: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
+0000af00: 7970 6501 0300 0000 1404 1804 3d04 3204  ype.........=.2.
+0000af10: 3504 4104 4204 3804 4604 3804 3808 0000  5.A.B.8.F.8.8...
+0000af20: 0000 0600 0000 0b49 6e76 6573 746d 656e  .......Investmen
+0000af30: 7473 0700 0000 1650 7265 6465 6669 6e64  ts.....Predefind
+0000af40: 6564 4163 636f 756e 7454 7970 6501 0300  edAccountType...
+0000af50: 0000 1404 2104 3104 3504 4004 3504 3604  ....!.1.5.@.5.6.
+0000af60: 3504 3d04 3804 4f08 0000 0000 0600 0000  5.=.8.O.........
+0000af70: 0753 6176 696e 6773 0700 0000 1650 7265  .Savings.....Pre
+0000af80: 6465 6669 6e64 6564 4163 636f 756e 7454  defindedAccountT
+0000af90: 7970 6501 0300 0000 1400 6500 2d04 1a04  ype.......e.-...
+0000afa0: 3e04 4804 3504 3b04 4c04 3a04 3808 0000  >.H.5.;.L.:.8...
+0000afb0: 0000 0600 0000 0965 2d57 616c 6c65 7473  .......e-Wallets
+0000afc0: 0700 0000 1650 7265 6465 6669 6e64 6564  .....Predefinded
+0000afd0: 4163 636f 756e 7454 7970 6501 0300 0000  AccountType.....
+0000afe0: 1204 1e04 3104 3b04 3804 3304 3004 4604  ....1.;.8.3.0.F.
+0000aff0: 3804 3808 0000 0000 0600 0000 0542 6f6e  8.8..........Bon
+0000b000: 6473 0700 0000 0f50 7265 6465 6669 6e65  ds.....Predefine
+0000b010: 6441 7373 6574 0103 0000 000c 0422 043e  dAsset.......".>
+0000b020: 0432 0430 0440 044b 0800 0000 0006 0000  .2.0.@.K........
+0000b030: 000b 436f 6d6d 6f64 6974 6965 7307 0000  ..Commodities...
+0000b040: 000f 5072 6564 6566 696e 6564 4173 7365  ..PredefinedAsse
+0000b050: 7401 0300 0000 1804 1a04 4004 3804 3f04  t.........@.8.?.
+0000b060: 4204 3e04 3204 3004 3b04 4e04 4204 4b08  B.>.2.0.;.N.B.K.
+0000b070: 0000 0000 0600 0000 0f43 7279 7074 6f2d  .........Crypto-
+0000b080: 6375 7272 656e 6379 0700 0000 0f50 7265  currency.....Pre
+0000b090: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
+0000b0a0: 0014 0414 0435 0440 0438 0432 0430 0442  .....5.@.8.2.0.B
+0000b0b0: 0438 0432 044b 0800 0000 0006 0000 000b  .8.2.K..........
+0000b0c0: 4465 7269 7661 7469 7665 7307 0000 000f  Derivatives.....
+0000b0d0: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
+0000b0e0: 0300 0000 0804 1104 1f04 1804 2408 0000  ............$...
+0000b0f0: 0000 0600 0000 0445 5446 7307 0000 000f  .......ETFs.....
+0000b100: 5072 6564 6566 696e 6564 4173 7365 7401  PredefinedAsset.
+0000b110: 0300 0000 0c04 2404 3e04 4004 3504 3a04  ......$.>.@.5.:.
+0000b120: 4108 0000 0000 0600 0000 0546 6f72 6578  A..........Forex
+0000b130: 0700 0000 0f50 7265 6465 6669 6e65 6441  .....PredefinedA
+0000b140: 7373 6574 0103 0000 000a 0424 043e 043d  sset.......$.>.=
+0000b150: 0434 044b 0800 0000 0006 0000 0005 4675  .4.K..........Fu
+0000b160: 6e64 7307 0000 000f 5072 6564 6566 696e  nds.....Predefin
+0000b170: 6564 4173 7365 7401 0300 0000 0c04 1204  edAsset.........
+0000b180: 3004 3b04 4e04 4204 4b08 0000 0000 0600  0.;.N.B.K.......
+0000b190: 0000 054d 6f6e 6579 0700 0000 0f50 7265  ...Money.....Pre
+0000b1a0: 6465 6669 6e65 6441 7373 6574 0103 0000  definedAsset....
+0000b1b0: 000a 0410 043a 0446 0438 0438 0800 0000  .....:.F.8.8....
+0000b1c0: 0006 0000 0006 5368 6172 6573 0700 0000  ......Shares....
+0000b1d0: 0f50 7265 6465 6669 6e65 6441 7373 6574  .PredefinedAsset
+0000b1e0: 0103 0000 0002 0025 0800 0000 0006 0000  .......%........
+0000b1f0: 0001 2507 0000 000f 5072 6f66 6974 4c6f  ..%.....ProfitLo
+0000b200: 7373 4d6f 6465 6c01 0300 0000 0604 1004  ssModel.........
+0000b210: 3f04 4008 0000 0000 0600 0000 0341 7072  ?.@..........Apr
+0000b220: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
+0000b230: 6f64 656c 0103 0000 0004 0426 0411 0800  odel.......&....
+0000b240: 0000 0006 0000 0006 4173 7365 7473 0700  ........Assets..
+0000b250: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
+0000b260: 656c 0103 0000 0006 0410 0432 0433 0800  el.........2.3..
+0000b270: 0000 0006 0000 0003 4175 6707 0000 000f  ........Aug.....
+0000b280: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000b290: 0300 0000 1204 1804 3704 3c04 3504 3d04  ........7.<.5.=.
+0000b2a0: 3504 3d04 3804 3508 0000 0000 0600 0000  5.=.8.5.........
+0000b2b0: 0643 6861 6e67 6507 0000 000f 5072 6f66  .Change.....Prof
+0000b2c0: 6974 4c6f 7373 4d6f 6465 6c01 0300 0000  itLossModel.....
+0000b2d0: 1804 1804 3704 3c04 3504 3d04 3504 3d04  ....7.<.5.=.5.=.
+0000b2e0: 3804 3500 2c00 2000 2508 0000 0000 0600  8.5.,. .%.......
+0000b2f0: 0000 0943 6861 6e67 652c 2025 0700 0000  ...Change, %....
+0000b300: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000b310: 0103 0000 0006 0414 0435 043a 0800 0000  .........5.:....
+0000b320: 0006 0000 0003 4465 6307 0000 000f 5072  ......Dec.....Pr
+0000b330: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000b340: 0000 1204 1404 3804 3204 3804 3404 3504  ......8.2.8.4.5.
+0000b350: 3d04 3404 4b08 0000 0000 0600 0000 0944  =.4.K..........D
+0000b360: 6976 6964 656e 6473 0700 0000 0f50 726f  ividends.....Pro
+0000b370: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000b380: 0006 0424 0435 0432 0800 0000 0006 0000  ...$.5.2........
+0000b390: 0003 4665 6207 0000 000f 5072 6f66 6974  ..Feb.....Profit
+0000b3a0: 4c6f 7373 4d6f 6465 6c01 0300 0000 1004  LossModel.......
+0000b3b0: 1a04 3e04 3c04 3804 4104 4104 3804 3808  ..>.<.8.A.A.8.8.
+0000b3c0: 0000 0000 0600 0000 0446 6565 7307 0000  .........Fees...
+0000b3d0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000b3e0: 6c01 0300 0000 1804 1204 3204 3e04 3400  l.........2.>.4.
+0000b3f0: 2000 2f00 2004 1204 4b04 3204 3e04 3408   ./. ...K.2.>.4.
+0000b400: 0000 0000 0600 0000 0849 6e20 2f20 4f75  .........In / Ou
+0000b410: 7407 0000 000f 5072 6f66 6974 4c6f 7373  t.....ProfitLoss
+0000b420: 4d6f 6465 6c01 0300 0000 0604 2f04 3d04  Model......./.=.
+0000b430: 3208 0000 0000 0600 0000 034a 616e 0700  2..........Jan..
+0000b440: 0000 0f50 726f 6669 744c 6f73 734d 6f64  ...ProfitLossMod
+0000b450: 656c 0103 0000 0006 0418 044e 043b 0800  el.........N.;..
+0000b460: 0000 0006 0000 0003 4a75 6c07 0000 000f  ........Jul.....
+0000b470: 5072 6f66 6974 4c6f 7373 4d6f 6465 6c01  ProfitLossModel.
+0000b480: 0300 0000 0604 1804 4e04 3d08 0000 0000  ........N.=.....
+0000b490: 0600 0000 034a 756e 0700 0000 0f50 726f  .....Jun.....Pro
+0000b4a0: 6669 744c 6f73 734d 6f64 656c 0103 0000  fitLossModel....
+0000b4b0: 0006 041c 0430 0440 0800 0000 0006 0000  .....0.@........
+0000b4c0: 0003 4d61 7207 0000 000f 5072 6f66 6974  ..Mar.....Profit
+0000b4d0: 4c6f 7373 4d6f 6465 6c01 0300 0000 0604  LossModel.......
+0000b4e0: 1c04 3004 3908 0000 0000 0600 0000 034d  ..0.9..........M
+0000b4f0: 6179 0700 0000 0f50 726f 6669 744c 6f73  ay.....ProfitLos
+0000b500: 734d 6f64 656c 0103 0000 0004 0414 0421  sModel.........!
+0000b510: 0800 0000 0006 0000 0005 4d6f 6e65 7907  ..........Money.
+0000b520: 0000 000f 5072 6f66 6974 4c6f 7373 4d6f  ....ProfitLossMo
+0000b530: 6465 6c01 0300 0000 0604 1d04 3e04 4f08  del.........>.O.
+0000b540: 0000 0000 0600 0000 034e 6f76 0700 0000  .........Nov....
+0000b550: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000b560: 0103 0000 0006 041e 043a 0442 0800 0000  .........:.B....
+0000b570: 0006 0000 0003 4f63 7407 0000 000f 5072  ......Oct.....Pr
+0000b580: 6f66 6974 4c6f 7373 4d6f 6465 6c01 0300  ofitLossModel...
+0000b590: 0000 0604 1f04 3804 2308 0000 0000 0600  ......8.#.......
+0000b5a0: 0000 0350 264c 0700 0000 0f50 726f 6669  ...P&L.....Profi
+0000b5b0: 744c 6f73 734d 6f64 656c 0103 0000 000c  tLossModel......
+0000b5c0: 041f 0435 0440 0438 043e 0434 0800 0000  ...5.@.8.>.4....
+0000b5d0: 0006 0000 0006 5065 7269 6f64 0700 0000  ......Period....
+0000b5e0: 0f50 726f 6669 744c 6f73 734d 6f64 656c  .ProfitLossModel
+0000b5f0: 0103 0000 001a 041a 043e 043d 0435 0446  .........>.=.5.F
+0000b600: 0020 043f 0435 0440 0438 043e 0434 0430  . .?.5.@.8.>.4.0
+0000b610: 0800 0000 0006 0000 000a 5065 7269 6f64  ..........Period
+0000b620: 2065 6e64 0700 0000 0f50 726f 6669 744c   end.....ProfitL
+0000b630: 6f73 734d 6f64 656c 0103 0000 001c 041d  ossModel........
+0000b640: 0430 0447 0430 043b 043e 0020 043f 0435  .0.G.0.;.>. .?.5
+0000b650: 0440 0438 043e 0434 0430 0800 0000 0006  .@.8.>.4.0......
+0000b660: 0000 000c 5065 7269 6f64 2073 7461 7274  ....Period start
+0000b670: 0700 0000 0f50 726f 6669 744c 6f73 734d  .....ProfitLossM
+0000b680: 6f64 656c 0103 0000 0006 0421 0435 043d  odel.......!.5.=
+0000b690: 0800 0000 0006 0000 0003 5365 7007 0000  ..........Sep...
+0000b6a0: 000f 5072 6f66 6974 4c6f 7373 4d6f 6465  ..ProfitLossMode
+0000b6b0: 6c01 0300 0000 0c04 1d04 3004 3b04 3e04  l.........0.;.>.
+0000b6c0: 3304 3808 0000 0000 0600 0000 0554 6178  3.8..........Tax
+0000b6d0: 6573 0700 0000 0f50 726f 6669 744c 6f73  es.....ProfitLos
+0000b6e0: 734d 6f64 656c 0103 0000 000a 0418 0442  sModel.........B
+0000b6f0: 043e 0433 043e 0800 0000 0006 0000 0005  .>.3.>..........
+0000b700: 546f 7461 6c07 0000 000f 5072 6f66 6974  Total.....Profit
+0000b710: 4c6f 7373 4d6f 6465 6c01 0300 0000 1804  LossModel.......
+0000b720: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
+0000b730: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
+0000b740: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
+0000b750: 0000 0010 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b760: 706f 7274 0103 0000 000a 0421 0447 0435  port.......!.G.5
+0000b770: 0442 003a 0800 0000 0006 0000 0008 4163  .B.:..........Ac
+0000b780: 636f 756e 743a 0700 0000 1650 726f 6669  count:.....Profi
+0000b790: 744c 6f73 7352 6570 6f72 7457 6964 6765  tLossReportWidge
+0000b7a0: 7401 0300 0000 1004 1204 3004 3b04 4e04  t.........0.;.N.
+0000b7b0: 4204 3000 3a00 2008 0000 0000 0600 0000  B.0.:. .........
+0000b7c0: 0a43 7572 7265 6e63 793a 2007 0000 0016  .Currency: .....
+0000b7d0: 5072 6f66 6974 4c6f 7373 5265 706f 7274  ProfitLossReport
+0000b7e0: 5769 6467 6574 0103 0000 0006 041f 0438  Widget.........8
+0000b7f0: 0423 0800 0000 0006 0000 0003 5026 4c07  .#..........P&L.
+0000b800: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b810: 706f 7274 5769 6467 6574 0103 0000 0018  portWidget......
+0000b820: 0421 043e 0445 0440 0430 043d 0438 0442  .!.>.E.@.0.=.8.B
+0000b830: 044c 002e 002e 002e 0800 0000 0006 0000  .L..............
+0000b840: 0007 5361 7665 2e2e 2e07 0000 0016 5072  ..Save........Pr
+0000b850: 6f66 6974 4c6f 7373 5265 706f 7274 5769  ofitLossReportWi
+0000b860: 6467 6574 0103 0000 0010 0412 0430 043b  dget.........0.;
+0000b870: 044e 0442 0430 003a 0020 0800 0000 0006  .N.B.0.:. ......
+0000b880: 0000 000a 4375 7272 656e 6379 3a20 0700  ....Currency: ..
+0000b890: 0000 1650 726f 6669 744c 6f73 7352 6570  ...ProfitLossRep
+0000b8a0: 6f72 7457 696e 646f 7701 0300 0000 1804  ortWindow.......
+0000b8b0: 1f04 3804 2300 2004 3f04 3e00 2004 4104  ..8.#. .?.>. .A.
+0000b8c0: 4704 5104 4204 4308 0000 0000 0600 0000  G.Q.B.C.........
+0000b8d0: 0e50 264c 2062 7920 4163 636f 756e 7407  .P&L by Account.
+0000b8e0: 0000 0016 5072 6f66 6974 4c6f 7373 5265  ....ProfitLossRe
+0000b8f0: 706f 7274 5769 6e64 6f77 0103 0000 001e  portWindow......
+0000b900: 041e 0448 0438 0431 043a 0430 0020 043a  ...H.8.1.:.0. .:
+0000b910: 0430 043c 0435 0440 044b 003a 0020 0800  .0.<.5.@.K.:. ..
+0000b920: 0000 0006 0000 000e 4361 6d65 7261 2065  ........Camera e
+0000b930: 7272 6f72 3a20 0700 0000 0951 5253 6361  rror: .....QRSca
+0000b940: 6e6e 6572 0103 0000 0084 041d 0435 0020  nner.........5. 
+0000b950: 043e 0431 043d 0430 0440 0443 0436 0435  .>.1.=.0.@.C.6.5
+0000b960: 043d 0020 043f 0430 043a 0435 0442 0020  .=. .?.0.:.5.B. 
+0000b970: 0070 0079 007a 0062 0061 0072 002c 0020  .p.y.z.b.a.r.,. 
+0000b980: 043d 0435 043e 0431 0445 043e 0434 0438  .=.5.>.1.E.>.4.8
+0000b990: 043c 044b 0439 0020 0434 043b 044f 0020  .<.K.9. .4.;.O. 
+0000b9a0: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+0000b9b0: 0432 0430 043d 0438 044f 0020 0051 0052  .2.0.=.8.O. .Q.R
+0000b9c0: 0020 043a 043e 0434 043e 0432 002e 0800  . .:.>.4.>.2....
+0000b9d0: 0000 0006 0000 002c 5061 636b 6167 6520  .......,Package 
+0000b9e0: 7079 7a62 6172 206e 6f74 2066 6f75 6e64  pyzbar not found
+0000b9f0: 2066 6f72 2051 5220 7265 636f 676e 6974   for QR recognit
+0000ba00: 696f 6e2e 0700 0000 0951 5253 6361 6e6e  ion......QRScann
+0000ba10: 6572 0103 0000 0026 041d 0435 0442 0020  er.....&...5.B. 
+0000ba20: 0434 043e 0441 0442 0443 043f 043d 044b  .4.>.A.B.C.?.=.K
+0000ba30: 0445 0020 043a 0430 043c 0435 0440 0800  .E. .:.0.<.5.@..
+0000ba40: 0000 0006 0000 001e 5468 6572 6520 6172  ........There ar
+0000ba50: 6520 6e6f 2063 616d 6572 6173 2061 7661  e no cameras ava
+0000ba60: 696c 6162 6c65 0700 0000 0951 5253 6361  ilable.....QRSca
+0000ba70: 6e6e 6572 0103 0000 0068 041d 0435 0432  nner.....h...5.2
+0000ba80: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000ba90: 043e 0431 0440 0430 0431 043e 0442 0430  .>.1.@.0.1.>.B.0
+0000baa0: 0442 044c 0020 0434 0430 043d 043d 044b  .B.L. .4.0.=.=.K
+0000bab0: 0435 0020 043a 043e 0442 0438 0440 043e  .5. .:.>.B.8.@.>
+0000bac0: 0432 043e 043a 0020 0441 0020 0431 0438  .2.>.:. .A. .1.8
+0000bad0: 0440 0436 0438 0020 0054 0053 0058 003a  .@.6.8. .T.S.X.:
+0000bae0: 0020 0800 0000 0006 0000 0021 4361 6e27  . .........!Can'
+0000baf0: 7420 7061 7273 6520 6461 7461 2066 6f72  t parse data for
+0000bb00: 2054 5358 2071 756f 7465 733a 2007 0000   TSX quotes: ...
+0000bb10: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
+0000bb20: 7201 0300 0000 2404 1704 3004 3304 4004  r.....$...0.3.@.
+0000bb30: 4304 3704 3a04 3000 2004 3704 3004 3204  C.7.:.0. .7.0.2.
+0000bb40: 3504 4004 4804 3504 3d04 3008 0000 0000  5.@.H.5.=.0.....
+0000bb50: 0600 0000 1244 6f77 6e6c 6f61 6420 636f  .....Download co
+0000bb60: 6d70 6c65 7465 6407 0000 000f 5175 6f74  mpleted.....Quot
+0000bb70: 6544 6f77 6e6c 6f61 6465 7201 0300 0000  eDownloader.....
+0000bb80: 6000 4900 5300 4900 4e00 2004 3200 2004  `.I.S.I.N. .2. .
+0000bb90: 3804 4104 4204 3e04 4004 3804 3800 2004  8.A.B.>.@.8.8. .
+0000bba0: 3a04 3e04 4204 3804 4004 3e04 3204 3e04  :.>.B.8.@.>.2.>.
+0000bbb0: 3a00 2000 4500 7500 7200 6f00 6e00 6500  :. .E.u.r.o.n.e.
+0000bbc0: 7800 7400 2004 3d04 3500 2004 4104 3e04  x.t. .=.5. .A.>.
+0000bbd0: 3204 3f04 3004 3404 3004 3504 4200 3a00  2.?.0.4.0.5.B.:.
+0000bbe0: 2008 0000 0000 0600 0000 2245 7572 6f6e   ........."Euron
+0000bbf0: 6578 7420 7175 6f74 6573 2049 5349 4e20  ext quotes ISIN 
+0000bc00: 6d69 736d 6174 6368 2069 6e3a 2007 0000  mismatch in: ...
+0000bc10: 000f 5175 6f74 6544 6f77 6e6c 6f61 6465  ..QuoteDownloade
+0000bc20: 7201 0300 0000 6404 1704 3004 3304 3e04  r.....d...0.3.>.
+0000bc30: 3b04 3e04 3204 3e04 3a00 2004 3804 4104  ;.>.2.>.:. .8.A.
+0000bc40: 4204 3e04 4004 3804 3800 2004 3a04 3e04  B.>.@.8.8. .:.>.
+0000bc50: 4204 3804 4004 3e04 3204 3e04 3a00 2000  B.8.@.>.2.>.:. .
+0000bc60: 4500 7500 7200 6f00 6e00 6500 7800 7400  E.u.r.o.n.e.x.t.
+0000bc70: 2004 3d04 3500 2004 3d04 3004 3904 3404   .=.5. .=.0.9.4.
+0000bc80: 3504 3d00 2004 3200 3a00 2008 0000 0000  5.=. .2.:. .....
+0000bc90: 0600 0000 2545 7572 6f6e 6578 7420 7175  ....%Euronext qu
+0000bca0: 6f74 6573 2068 6561 6465 7220 6e6f 7420  otes header not 
+0000bcb0: 666f 756e 6420 696e 3a20 0700 0000 0f51  found in: .....Q
+0000bcc0: 756f 7465 446f 776e 6c6f 6164 6572 0103  uoteDownloader..
+0000bcd0: 0000 005a 0418 0441 0442 043e 0440 0438  ...Z...A.B.>.@.8
+0000bce0: 044f 0020 043a 043e 0442 0438 0440 043e  .O. .:.>.B.8.@.>
+0000bcf0: 0432 043e 043a 0020 0045 0075 0072 006f  .2.>.:. .E.u.r.o
+0000bd00: 006e 0065 0078 0074 0020 0441 043b 0438  .n.e.x.t. .A.;.8
+0000bd10: 0448 043a 043e 043c 0020 043a 043e 0440  .H.:.>.<. .:.>.@
+0000bd20: 043e 0442 043a 0430 044f 003a 0020 0800  .>.B.:.0.O.:. ..
+0000bd30: 0000 0006 0000 002c 4575 726f 6e65 7874  .......,Euronext
+0000bd40: 2071 756f 7465 7320 6869 7374 6f72 7920   quotes history 
+0000bd50: 7265 706c 7920 6973 2074 6f6f 2073 686f  reply is too sho
+0000bd60: 7274 3a20 0700 0000 0f51 756f 7465 446f  rt: .....QuoteDo
+0000bd70: 776e 6c6f 6164 6572 0103 0000 0036 041d  wnloader.....6..
+0000bd80: 0435 0020 0437 0430 0433 0440 0443 0436  .5. .7.0.3.@.C.6
+0000bd90: 0435 043d 044b 0020 043a 043e 0442 0438  .5.=.K. .:.>.B.8
+0000bda0: 0440 043e 0432 043a 0438 0020 0434 043b  .@.>.2.:.8. .4.;
+0000bdb0: 044f 0020 0800 0000 0006 0000 001e 4e6f  .O. ..........No
+0000bdc0: 2071 756f 7465 7320 7765 7265 2064 6f77   quotes were dow
+0000bdd0: 6e6c 6f61 6465 6420 666f 7220 0700 0000  nloaded for ....
+0000bde0: 0f51 756f 7465 446f 776e 6c6f 6164 6572  .QuoteDownloader
+0000bdf0: 0103 0000 002e 041d 0435 0020 0437 0430  .........5. .7.0
+0000be00: 0433 0440 0443 0436 0435 043d 044b 0020  .3.@.C.6.5.=.K. 
+0000be10: 043a 0443 0440 0441 044b 0020 0434 043b  .:.C.@.A.K. .4.;
+0000be20: 044f 0020 0800 0000 0006 0000 001d 4e6f  .O. ..........No
+0000be30: 2072 6174 6573 2077 6572 6520 646f 776e   rates were down
+0000be40: 6c6f 6164 6564 2066 6f72 2007 0000 000f  loaded for .....
+0000be50: 5175 6f74 6544 6f77 6e6c 6f61 6465 7201  QuoteDownloader.
+0000be60: 0300 0000 2c04 1d04 3504 4200 2004 3404  ....,...5.B. .4.
+0000be70: 3004 3d04 3d04 4b04 4500 2004 2604 1100  0.=.=.K.E. .&...
+0000be80: 2004 2004 2400 2004 3404 3b04 4f00 3a00   . .$. .4.;.O.:.
+0000be90: 2008 0000 0000 0600 0000 1b54 6865 7265   ..........There
+0000bea0: 2061 7265 206e 6f20 4342 5220 6461 7461   are no CBR data
+0000beb0: 2066 6f72 3a20 0700 0000 0f51 756f 7465   for: .....Quote
+0000bec0: 446f 776e 6c6f 6164 6572 0103 0000 0012  Downloader......
+0000bed0: 041a 043e 0442 0438 0440 043e 0432 043a  ...>.B.8.@.>.2.:
+0000bee0: 0438 0800 0000 0006 0000 0006 5175 6f74  .8..........Quot
+0000bef0: 6573 0700 0000 1051 756f 7465 734c 6973  es.....QuotesLis
+0000bf00: 7444 6961 6c6f 6701 0300 0000 0404 2604  tDialog.......&.
+0000bf10: 1108 0000 0000 0600 0000 0541 7373 6574  ...........Asset
+0000bf20: 0700 0000 0f51 756f 7465 734c 6973 744d  .....QuotesListM
+0000bf30: 6f64 656c 0103 0000 000c 0412 0430 043b  odel.........0.;
+0000bf40: 044e 0442 0430 0800 0000 0006 0000 0008  .N.B.0..........
+0000bf50: 4375 7272 656e 6379 0700 0000 0f51 756f  Currency.....Quo
+0000bf60: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
+0000bf70: 0008 0414 0430 0442 0430 0800 0000 0006  .....0.B.0......
+0000bf80: 0000 0004 4461 7465 0700 0000 0f51 756f  ....Date.....Quo
+0000bf90: 7465 734c 6973 744d 6f64 656c 0103 0000  tesListModel....
+0000bfa0: 0012 041a 043e 0442 0438 0440 043e 0432  .....>.B.8.@.>.2
+0000bfb0: 043a 0430 0800 0000 0006 0000 0005 5175  .:.0..........Qu
+0000bfc0: 6f74 6507 0000 000f 5175 6f74 6573 4c69  ote.....QuotesLi
+0000bfd0: 7374 4d6f 6465 6c01 0300 0000 2800 2604  stModel.....(.&.
+0000bfe0: 1f04 3e04 3b04 3d04 3e04 4104 4204 4c04  ..>.;.=.>.A.B.L.
+0000bff0: 4e00 2c00 2004 4100 2004 3d04 3004 4704  N.,. .A. .=.0.G.
+0000c000: 3004 3b04 3008 0000 0000 0600 0000 1326  0.;.0..........&
+0000c010: 4675 6c6c 2c20 6672 6f6d 2073 6372 6174  Full, from scrat
+0000c020: 6368 0700 0000 0d52 6542 7569 6c64 4469  ch.....ReBuildDi
+0000c030: 616c 6f67 0103 0000 0018 0418 043d 0442  alog.........=.B
+0000c040: 0435 0440 0432 0430 043b 0020 0434 0430  .5.@.2.0.;. .4.0
+0000c050: 0442 0800 0000 0006 0000 000a 4461 7465  .B..........Date
+0000c060: 2052 616e 6765 0700 0000 0d52 6542 7569   Range.....ReBui
+0000c070: 6c64 4469 616c 6f67 0103 0000 002a 0026  ldDialog.....*.&
+0000c080: 0411 044b 0441 0442 0440 043e 002c 0020  ...K.A.B.@.>.,. 
+0000c090: 043d 043e 0020 043d 0435 043d 0430 0434  .=.>. .=.5.=.0.4
+0000c0a0: 0451 0436 043d 043e 0800 0000 0006 0000  .Q.6.=.>........
+0000c0b0: 0011 4661 7374 2c20 2675 6e72 656c 6961  ..Fast, &unrelia
+0000c0c0: 626c 6507 0000 000d 5265 4275 696c 6444  ble.....ReBuildD
+0000c0d0: 6961 6c6f 6701 0300 0000 1604 1404 3004  ialog.........0.
+0000c0e0: 4204 3004 1304 4004 3004 3d04 3804 4604  B.0...@.0.=.8.F.
+0000c0f0: 4b08 0000 0000 0600 0000 0c46 726f 6e74  K..........Front
+0000c100: 6965 7244 6174 6507 0000 000d 5265 4275  ierDate.....ReBu
+0000c110: 696c 6444 6961 6c6f 6701 0300 0000 2204  ildDialog.....".
+0000c120: 1f04 3504 4004 3504 4104 4704 3804 4204  ..5.@.5.A.G.8.B.
+0000c130: 3004 4204 4c00 2004 3804 4204 3e04 3304  0.B.L. .8.B.>.3.
+0000c140: 3808 0000 0000 0600 0000 0f52 652d 4275  8..........Re-Bu
+0000c150: 696c 6420 4c65 6467 6572 0700 0000 0d52  ild Ledger.....R
+0000c160: 6542 7569 6c64 4469 616c 6f67 0103 0000  eBuildDialog....
+0000c170: 0010 0421 0020 0026 0414 0430 0442 044b  ...!. .&...0.B.K
+0000c180: 003a 0800 0000 0006 0000 000c 5369 6e63  .:..........Sinc
+0000c190: 6520 2644 6174 653a 0700 0000 0d52 6542  e &Date:.....ReB
+0000c1a0: 7569 6c64 4469 616c 6f67 0103 0000 002c  uildDialog.....,
+0000c1b0: 0421 0020 043a 0440 0430 0439 043d 0435  .!. .:.@.0.9.=.5
+0000c1c0: 0439 0020 0026 0430 043a 0442 0443 0430  .9. .&.0.:.B.C.0
+0000c1d0: 043b 044c 043d 043e 0439 003a 0800 0000  .;.L.=.>.9.:....
+0000c1e0: 0006 0000 0013 5369 6e63 6520 264c 6173  ......Since &Las
+0000c1f0: 7420 6163 7475 616c 3a07 0000 000d 5265  t actual:.....Re
+0000c200: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
+0000c210: 1400 6400 6400 2f00 4d00 4d00 2f00 7900  ..d.d./.M.M./.y.
+0000c220: 7900 7900 7908 0000 0000 0600 0000 0a64  y.y.y..........d
+0000c230: 642f 4d4d 2f79 7979 7907 0000 000d 5265  d/MM/yyyy.....Re
+0000c240: 4275 696c 6444 6961 6c6f 6701 0300 0000  BuildDialog.....
+0000c250: 0a04 1b04 4e04 3104 3e04 3908 0000 0000  ....N.1.>.9.....
+0000c260: 0600 0000 0341 4e59 0700 0000 1352 6566  .....ANY.....Ref
+0000c270: 6572 656e 6365 4461 7461 4469 616c 6f67  erenceDataDialog
+0000c280: 0103 0000 0014 0422 0438 043f 0020 0441  .......".8.?. .A
+0000c290: 0447 0435 0442 0430 003a 0800 0000 0006  .G.5.B.0.:......
+0000c2a0: 0000 000d 4163 636f 756e 7420 5479 7065  ....Account Type
+0000c2b0: 3a07 0000 0013 5265 6665 7265 6e63 6544  :.....ReferenceD
+0000c2c0: 6174 6144 6961 6c6f 6701 0300 0000 2204  ataDialog.....".
+0000c2d0: 1404 3e04 3104 3004 3204 3804 4204 4c00  ..>.1.0.2.8.B.L.
+0000c2e0: 2004 3404 3e04 4704 3504 4004 3d04 3804   .4.>.G.5.@.=.8.
+0000c2f0: 3908 0000 0000 0600 0000 0941 6464 2063  9..........Add c
+0000c300: 6869 6c64 0700 0000 1352 6566 6572 656e  hild.....Referen
+0000c310: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000c320: 001c 0414 043e 0431 0430 0432 0438 0442  .....>.1.0.2.8.B
+0000c330: 044c 0020 043d 043e 0432 044b 0439 0800  .L. .=.>.2.K.9..
+0000c340: 0000 0006 0000 0007 4164 6420 6e65 7707  ........Add new.
+0000c350: 0000 0013 5265 6665 7265 6e63 6544 6174  ....ReferenceDat
+0000c360: 6144 6961 6c6f 6701 0300 0000 1e04 2104  aDialog.......!.
+0000c370: 3c04 3504 3d04 3804 4204 4c00 2004 4204  <.5.=.8.B.L. .B.
+0000c380: 3804 3f00 2004 3d04 3000 3a08 0000 0000  8.?. .=.0.:.....
+0000c390: 0600 0000 0f43 6861 6e67 6520 7479 7065  .....Change type
+0000c3a0: 2074 6f3a 0700 0000 1352 6566 6572 656e   to:.....Referen
+0000c3b0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000c3c0: 001a 041f 043e 0434 0442 0432 0435 0440  .....>.4.B.2.5.@
+0000c3d0: 0436 0434 0435 043d 0438 0435 0800 0000  .6.4.5.=.8.5....
+0000c3e0: 0006 0000 000c 436f 6e66 6972 6d61 7469  ......Confirmati
+0000c3f0: 6f6e 0700 0000 1352 6566 6572 656e 6365  on.....Reference
+0000c400: 4461 7461 4469 616c 6f67 0103 0000 000e  DataDialog......
+0000c410: 0423 0434 0430 043b 0438 0442 044c 0800  .#.4.0.;.8.B.L..
+0000c420: 0000 0006 0000 0006 4465 6c65 7465 0700  ........Delete..
+0000c430: 0000 1352 6566 6572 656e 6365 4461 7461  ...ReferenceData
+0000c440: 4469 616c 6f67 0103 0000 0022 0421 043f  Dialog.....".!.?
+0000c450: 0440 0430 0432 043e 0447 043d 044b 0435  .@.0.2.>.G.=.K.5
+0000c460: 0020 0434 0430 043d 043d 044b 0435 0800  . .4.0.=.=.K.5..
+0000c470: 0000 0006 0000 000e 5265 6665 7265 6e63  ........Referenc
+0000c480: 6520 4461 7461 0700 0000 1352 6566 6572  e Data.....Refer
+0000c490: 656e 6365 4461 7461 4469 616c 6f67 0103  enceDataDialog..
+0000c4a0: 0000 0024 041e 0442 043c 0435 043d 0438  ...$...B.<.5.=.8
+0000c4b0: 0442 044c 0020 0438 0437 043c 0435 043d  .B.L. .8.7.<.5.=
+0000c4c0: 0435 043d 0438 044f 0800 0000 0006 0000  .5.=.8.O........
+0000c4d0: 000e 5265 7665 7274 2063 6861 6e67 6573  ..Revert changes
+0000c4e0: 0700 0000 1352 6566 6572 656e 6365 4461  .....ReferenceDa
+0000c4f0: 7461 4469 616c 6f67 0103 0000 0026 0421  taDialog.....&.!
+0000c500: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+0000c510: 0020 0438 0437 043c 0435 043d 0435 043d  . .8.7.<.5.=.5.=
+0000c520: 0438 044f 0800 0000 0006 0000 000c 5361  .8.O..........Sa
+0000c530: 7665 2063 6861 6e67 6573 0700 0000 1352  ve changes.....R
+0000c540: 6566 6572 656e 6365 4461 7461 4469 616c  eferenceDataDial
+0000c550: 6f67 0103 0000 000c 041f 043e 0438 0441  og.........>.8.A
+0000c560: 043a 003a 0800 0000 0006 0000 0007 5365  .:.:..........Se
+0000c570: 6172 6368 3a07 0000 0013 5265 6665 7265  arch:.....Refere
+0000c580: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
+0000c590: 0000 2a04 1f04 3e04 3a04 3004 3704 4b04  ..*...>.:.0.7.K.
+0000c5a0: 3204 3004 4204 4c00 2004 3d04 3504 3004  2.0.B.L. .=.5.0.
+0000c5b0: 3a04 4204 3804 3204 3d04 4b04 3508 0000  :.B.8.2.=.K.5...
+0000c5c0: 0000 0600 0000 0d53 686f 7720 696e 6163  .......Show inac
+0000c5d0: 7469 7665 0700 0000 1352 6566 6572 656e  tive.....Referen
+0000c5e0: 6365 4461 7461 4469 616c 6f67 0103 0000  ceDataDialog....
+0000c5f0: 0066 0423 0020 0432 0430 0441 0020 0435  .f.#. .2.0.A. .5
+0000c600: 0441 0442 044c 0020 043d 0435 0441 043e  .A.B.L. .=.5.A.>
+0000c610: 0445 0440 0430 043d 0451 043d 043d 044b  .E.@.0.=.Q.=.=.K
+0000c620: 0435 0020 0434 0430 043d 043d 044b 0435  .5. .4.0.=.=.K.5
+0000c630: 002e 0020 0412 0441 0451 0020 0440 0430  ... ...A.Q. .@.0
+0000c640: 0432 043d 043e 0020 0437 0430 043a 0440  .2.=.>. .7.0.:.@
+0000c650: 044b 0442 044c 003f 0800 0000 0006 0000  .K.B.L.?........
+0000c660: 0033 596f 7520 6861 7665 2075 6e63 6f6d  .3You have uncom
+0000c670: 6d69 7474 6564 2063 6861 6e67 6573 2e20  mitted changes. 
+0000c680: 446f 2079 6f75 2077 616e 7420 746f 2063  Do you want to c
+0000c690: 6c6f 7365 3f07 0000 0013 5265 6665 7265  lose?.....Refere
+0000c6a0: 6e63 6544 6174 6144 6961 6c6f 6701 0300  nceDataDialog...
+0000c6b0: 0000 0604 1004 3f04 4008 0000 0000 0600  ......?.@.......
+0000c6c0: 0000 0341 7072 0700 0000 0e52 6570 6f72  ...Apr.....Repor
+0000c6d0: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c6e0: 1004 3204 3308 0000 0000 0600 0000 0341  ..2.3..........A
+0000c6f0: 7567 0700 0000 0e52 6570 6f72 7454 7265  ug.....ReportTre
+0000c700: 6549 7465 6d01 0300 0000 0604 1404 3504  eItem.........5.
+0000c710: 3a08 0000 0000 0600 0000 0344 6563 0700  :..........Dec..
+0000c720: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c730: 6d01 0300 0000 0604 2404 3504 3208 0000  m.......$.5.2...
+0000c740: 0000 0600 0000 0346 6562 0700 0000 0e52  .......Feb.....R
+0000c750: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c760: 0000 0604 2f04 3d04 3208 0000 0000 0600  ..../.=.2.......
+0000c770: 0000 034a 616e 0700 0000 0e52 6570 6f72  ...Jan.....Repor
+0000c780: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c790: 1804 4e04 3b08 0000 0000 0600 0000 034a  ..N.;..........J
+0000c7a0: 756c 0700 0000 0e52 6570 6f72 7454 7265  ul.....ReportTre
+0000c7b0: 6549 7465 6d01 0300 0000 0604 1804 4e04  eItem.........N.
+0000c7c0: 3d08 0000 0000 0600 0000 034a 756e 0700  =..........Jun..
+0000c7d0: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c7e0: 6d01 0300 0000 0604 1c04 3004 4008 0000  m.........0.@...
+0000c7f0: 0000 0600 0000 034d 6172 0700 0000 0e52  .......Mar.....R
+0000c800: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c810: 0000 0604 1c04 3004 3908 0000 0000 0600  ......0.9.......
+0000c820: 0000 034d 6179 0700 0000 0e52 6570 6f72  ...May.....Repor
+0000c830: 7454 7265 6549 7465 6d01 0300 0000 0604  tTreeItem.......
+0000c840: 1d04 3e04 4f08 0000 0000 0600 0000 034e  ..>.O..........N
+0000c850: 6f76 0700 0000 0e52 6570 6f72 7454 7265  ov.....ReportTre
+0000c860: 6549 7465 6d01 0300 0000 0604 1e04 3a04  eItem.........:.
+0000c870: 4208 0000 0000 0600 0000 034f 6374 0700  B..........Oct..
+0000c880: 0000 0e52 6570 6f72 7454 7265 6549 7465  ...ReportTreeIte
+0000c890: 6d01 0300 0000 0604 2104 3504 3d08 0000  m.......!.5.=...
+0000c8a0: 0000 0600 0000 0353 6570 0700 0000 0e52  .......Sep.....R
+0000c8b0: 6570 6f72 7454 7265 6549 7465 6d01 0300  eportTreeItem...
+0000c8c0: 0000 0604 3d04 3504 3408 0000 0000 0600  ....=.5.4.......
+0000c8d0: 0000 0277 6b07 0000 000e 5265 706f 7274  ...wk.....Report
+0000c8e0: 5472 6565 4974 656d 0103 0000 0028 0424  TreeItem.....(.$
+0000c8f0: 0430 0439 043b 044b 0020 0045 0078 0063  .0.9.;.K. .E.x.c
+0000c900: 0065 006c 0020 0028 002a 002e 0078 0073  .e.l. .(.*...x.s
+0000c910: 006c 0078 0029 0800 0000 0006 0000 0014  .l.x.)..........
+0000c920: 4578 6365 6c20 6669 6c65 7320 282a 2e78  Excel files (*.x
+0000c930: 6c73 7829 0700 0000 0752 6570 6f72 7473  lsx).....Reports
+0000c940: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
+0000c950: 043c 043e 0436 043d 043e 0020 0437 0430  .<.>.6.=.>. .7.0
+0000c960: 0433 0440 0443 0437 0438 0442 044c 0020  .3.@.C.7.8.B.L. 
+0000c970: 043a 043b 0430 0441 0441 0020 043e 0442  .:.;.0.A.A. .>.B
+0000c980: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+0000c990: 0006 0000 001e 5265 706f 7274 2063 6c61  ......Report cla
+0000c9a0: 7373 2063 616e 2774 2062 6520 6c6f 6164  ss can't be load
+0000c9b0: 6564 3a20 0700 0000 0752 6570 6f72 7473  ed: .....Reports
+0000c9c0: 0103 0000 0042 041e 0442 0447 0435 0442  .....B...B.G.5.B
+0000c9d0: 0020 043d 0435 0020 043d 0430 0439 0434  . .=.5. .=.0.9.4
+0000c9e0: 0435 043d 0020 0434 043b 044f 0020 043a  .5.=. .4.;.O. .:
+0000c9f0: 043b 0430 0441 0441 0430 0020 043e 043a  .;.0.A.A.0. .>.:
+0000ca00: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
+0000ca10: 0023 5265 706f 7274 206e 6f74 2066 6f75  .#Report not fou
+0000ca20: 6e64 2066 6f72 2077 696e 646f 7720 636c  nd for window cl
+0000ca30: 6173 733a 2007 0000 0007 5265 706f 7274  ass: .....Report
+0000ca40: 7301 0300 0000 2c04 1e04 4204 4704 3504  s.....,...B.G.5.
+0000ca50: 4200 2004 4104 3e04 4504 4004 3004 3d04  B. .A.>.E.@.0.=.
+0000ca60: 5104 3d00 2004 3200 2004 4404 3004 3904  Q.=. .2. .D.0.9.
+0000ca70: 3b00 2008 0000 0000 0600 0000 1952 6570  ;. ..........Rep
+0000ca80: 6f72 7420 7761 7320 7361 7665 6420 746f  ort was saved to
+0000ca90: 2066 696c 6520 0700 0000 0752 6570 6f72   file .....Repor
+0000caa0: 7473 0103 0000 0024 0421 043e 0445 0440  ts.....$.!.>.E.@
+0000cab0: 0430 043d 0438 0442 044c 0020 043e 0442  .0.=.8.B.L. .>.B
+0000cac0: 0447 0435 0442 0020 0432 003a 0800 0000  .G.5.B. .2.:....
+0000cad0: 0006 0000 000f 5361 7665 2072 6570 6f72  ......Save repor
+0000cae0: 7420 746f 3a07 0000 0007 5265 706f 7274  t to:.....Report
+0000caf0: 7301 0300 0000 3c04 1b04 3e04 3304 3804  s.....<...>.3.8.
+0000cb00: 3d00 2004 4704 3504 4004 3504 3700 2004  =. .G.5.@.5.7. .
+0000cb10: 1304 3e04 4104 4304 4104 3b04 4304 3304  ..>.A.C.A.;.C.3.
+0000cb20: 3800 2004 3704 3004 3204 3504 4004 4804  8. .7.0.2.5.@.H.
+0000cb30: 5104 3d08 0000 0000 0600 0000 1445 5349  Q.=..........ESI
+0000cb40: 4120 6c6f 6769 6e20 636f 6d70 6c65 7465  A login complete
+0000cb50: 6407 0000 0012 5265 7175 6573 7449 6e74  d.....RequestInt
+0000cb60: 6572 6365 7074 6f72 0103 0000 000a 0410  erceptor........
+0000cb70: 043a 0442 0438 0432 0800 0000 0006 0000  .:.B.8.2........
+0000cb80: 0005 4173 7365 7407 0000 000c 5265 7375  ..Asset.....Resu
+0000cb90: 6c74 734d 6f64 656c 0103 0000 000c 041a  ltsModel........
+0000cba0: 043e 043b 002d 0432 043e 0800 0000 0006  .>.;.-.2.>......
+0000cbb0: 0000 0003 5174 7907 0000 000c 5265 7375  ....Qty.....Resu
+0000cbc0: 6c74 734d 6f64 656c 0103 0000 000e 0414  ltsModel........
+0000cbd0: 043e 043b 044f 002c 0020 0025 0800 0000  .>.;.O.,. .%....
+0000cbe0: 0006 0000 0008 5368 6172 652c 2025 0700  ......Share, %..
+0000cbf0: 0000 0c52 6573 756c 7473 4d6f 6465 6c01  ...ResultsModel.
+0000cc00: 0300 0000 3004 1204 4b04 3104 4004 3004  ....0...K.1.@.0.
+0000cc10: 3d00 2004 3d04 3504 3a04 3e04 4004 4004  =. .=.5.:.>.@.@.
+0000cc20: 3504 3a04 4204 3d04 4b04 3900 2004 4104  5.:.B.=.K.9. .A.
+0000cc30: 4704 5104 4208 0000 0000 0600 0000 1849  G.Q.B..........I
+0000cc40: 6e76 616c 6964 2061 6363 6f75 6e74 2073  nvalid account s
+0000cc50: 656c 6563 7465 6407 0000 0013 5365 6c65  elected.....Sele
+0000cc60: 6374 4163 636f 756e 7444 6961 6c6f 6701  ctAccountDialog.
+0000cc70: 0300 0000 2204 1d04 3804 4704 3504 3304  ...."...8.G.5.3.
+0000cc80: 3e00 2004 3d04 3500 2004 3204 4b04 3104  >. .=.5. .2.K.1.
+0000cc90: 4004 3004 3d04 3e08 0000 0000 0600 0000  @.0.=.>.........
+0000cca0: 0c4e 6f20 7365 6c65 6374 696f 6e07 0000  .No selection...
+0000ccb0: 0013 5365 6c65 6374 4163 636f 756e 7444  ..SelectAccountD
+0000ccc0: 6961 6c6f 6701 0300 0000 4004 1f04 3e04  ialog.....@...>.
+0000ccd0: 3604 3004 3b04 4304 3904 4104 4204 3000  6.0.;.C.9.A.B.0.
+0000cce0: 2c00 2004 3204 4b04 3104 3504 4004 3804  ,. .2.K.1.5.@.8.
+0000ccf0: 4204 3500 2004 3404 4004 4304 3304 3e04  B.5. .4.@.C.3.>.
+0000cd00: 3900 2004 4104 4704 5104 4208 0000 0000  9. .A.G.Q.B.....
+0000cd10: 0600 0000 1f50 6c65 6173 6520 7365 6c65  .....Please sele
+0000cd20: 6374 2064 6966 6665 7265 6e74 2061 6363  ct different acc
+0000cd30: 6f75 6e74 0700 0000 1353 656c 6563 7441  ount.....SelectA
+0000cd40: 6363 6f75 6e74 4469 616c 6f67 0103 0000  ccountDialog....
+0000cd50: 0030 041f 043e 0436 0430 043b 0443 0439  .0...>.6.0.;.C.9
+0000cd60: 0441 0442 0430 0020 0432 044b 0431 0435  .A.B.0. .2.K.1.5
+0000cd70: 0440 0438 0442 0435 0020 0441 0447 0451  .@.8.B.5. .A.G.Q
+0000cd80: 0442 0800 0000 0006 0000 0015 506c 6561  .B..........Plea
+0000cd90: 7365 2073 656c 6563 7420 6163 636f 756e  se select accoun
+0000cda0: 7407 0000 0010 5365 6c65 6374 4163 636f  t.....SelectAcco
+0000cdb0: 756e 7444 6c67 0103 0000 0012 0421 043e  untDlg.......!.>
+0000cdc0: 043e 0431 0449 0435 043d 0438 0435 0800  .>.1.I.5.=.8.5..
+0000cdd0: 0000 0006 0000 0009 5465 7874 4c61 6265  ........TextLabe
+0000cde0: 6c07 0000 0010 5365 6c65 6374 4163 636f  l.....SelectAcco
+0000cdf0: 756e 7444 6c67 0103 0000 0056 0418 0441  untDlg.....V...A
+0000ce00: 043f 043e 043b 044c 0437 043e 0432 0430  .?.>.;.L.7.>.2.0
+0000ce10: 0442 044c 0020 044d 0442 043e 0442 0020  .B.L. .M.B.>.B. 
+0000ce20: 0436 0435 0020 0441 0447 0451 0442 0020  .6.5. .A.G.Q.B. 
+0000ce30: 0434 043b 044f 0020 0434 0430 043d 043d  .4.;.O. .4.0.=.=
+0000ce40: 043e 0439 0020 0432 0430 043b 044e 0442  .>.9. .2.0.;.N.B
+0000ce50: 044b 0800 0000 0006 0000 0027 5573 6520  .K.........'Use 
+0000ce60: 7468 6520 7361 6d65 2061 6363 6f75 6e74  the same account
+0000ce70: 2066 6f72 2067 6976 656e 2063 7572 7265   for given curre
+0000ce80: 6e63 7907 0000 0010 5365 6c65 6374 4163  ncy.....SelectAc
+0000ce90: 636f 756e 7444 6c67 0103 0000 0024 0412  countDlg.....$..
+0000cea0: 044b 0431 0435 0440 0438 0442 0435 0020  .K.1.5.@.8.B.5. 
+0000ceb0: 043a 0430 0442 0435 0433 043e 0440 0438  .:.0.B.5.3.>.@.8
+0000cec0: 044e 0800 0000 0006 0000 0016 506c 6561  .N..........Plea
+0000ced0: 7365 2073 656c 6563 7420 6361 7465 676f  se select catego
+0000cee0: 7279 0700 0000 1453 656c 6563 7443 6174  ry.....SelectCat
+0000cef0: 6567 6f72 7944 6961 6c6f 6701 0300 0000  egoryDialog.....
+0000cf00: 2804 1204 4b04 3104 3504 4004 3804 4204  (...K.1.5.@.8.B.
+0000cf10: 3500 2004 3a04 3e04 3d04 4204 4004 3004  5. .:.>.=.B.@.0.
+0000cf20: 3304 3504 3d04 4204 3008 0000 0000 0600  3.5.=.B.0.......
+0000cf30: 0000 1250 6c65 6173 6520 7365 6c65 6374  ...Please select
+0000cf40: 2070 6565 7207 0000 0010 5365 6c65 6374   peer.....Select
+0000cf50: 5065 6572 4469 616c 6f67 0103 0000 0022  PeerDialog....."
+0000cf60: 041d 0438 0447 0435 0433 043e 0020 043d  ...8.G.5.3.>. .=
+0000cf70: 0435 0020 0432 044b 0431 0440 0430 043d  .5. .2.K.1.@.0.=
+0000cf80: 043e 0800 0000 0006 0000 000c 4e6f 2073  .>..........No s
+0000cf90: 656c 6563 7469 6f6e 0700 0000 1553 656c  election.....Sel
+0000cfa0: 6563 7452 6566 6572 656e 6365 4469 616c  ectReferenceDial
+0000cfb0: 6f67 0103 0000 002e 0412 044b 0020 0434  og.........K. .4
+0000cfc0: 043e 043b 0436 043d 044b 0020 0441 0434  .>.;.6.=.K. .A.4
+0000cfd0: 0435 043b 0430 0442 044c 0020 0432 044b  .5.;.0.B.L. .2.K
+0000cfe0: 0431 043e 0440 0800 0000 0006 0000 001b  .1.>.@..........
+0000cff0: 596f 7520 7368 6f75 6c64 2073 656c 6563  You should selec
+0000d000: 7420 736f 6d65 7468 696e 6707 0000 0015  t something.....
+0000d010: 5365 6c65 6374 5265 6665 7265 6e63 6544  SelectReferenceD
+0000d020: 6961 6c6f 6701 0300 0000 1c04 1204 4b04  ialog.........K.
+0000d030: 3104 3504 4004 3804 4204 3500 2004 3c04  1.5.@.8.B.5. .<.
+0000d040: 3504 4204 3a04 4308 0000 0000 0600 0000  5.B.:.C.........
+0000d050: 1150 6c65 6173 6520 7365 6c65 6374 2074  .Please select t
+0000d060: 6167 0700 0000 0f53 656c 6563 7454 6167  ag.....SelectTag
+0000d070: 4469 616c 6f67 0103 0000 005a 041d 0435  Dialog.....Z...5
+0000d080: 0020 0443 0434 0430 043b 043e 0441 044c  . .C.4.0.;.>.A.L
+0000d090: 0020 043f 043e 043b 0443 0447 0438 0442  . .?.>.;.C.G.8.B
+0000d0a0: 044c 0020 043d 0430 0437 0432 0430 043d  .L. .=.0.7.2.0.=
+0000d0b0: 0438 0435 0020 043e 0433 0440 0430 043d  .8.5. .>.3.@.0.=
+0000d0c0: 0438 0437 0430 0446 0438 0438 0020 0438  .8.7.0.F.8.8. .8
+0000d0d0: 0437 003a 0020 0800 0000 0006 0000 001d  .7.:. ..........
+0000d0e0: 4361 6e27 7420 6765 7420 636f 6d70 616e  Can't get compan
+0000d0f0: 7920 6e61 6d65 2066 726f 6d3a 2007 0000  y name from: ...
+0000d100: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000d110: 0000 4804 1d04 3504 3204 3e04 3704 3c04  ..H...5.2.>.7.<.
+0000d120: 3e04 3604 3d04 3e00 2004 3e04 3104 3204  >.6.=.>. .>.1.2.
+0000d130: 3d04 3e04 3204 3804 4204 4c00 2004 4104  =.>.2.8.B.L. .A.
+0000d140: 3504 4104 4104 3804 4e00 2c00 2004 3e04  5.A.A.8.N.,. .>.
+0000d150: 4204 3204 3504 4200 3a00 2008 0000 0000  B.2.5.B.:. .....
+0000d160: 0600 0000 2143 616e 2774 2072 6566 7265  ....!Can't refre
+0000d170: 7368 2073 6573 7369 6f6e 2c20 7265 7370  sh session, resp
+0000d180: 6f6e 7365 3a20 0700 0000 0b53 6c69 7073  onse: .....Slips
+0000d190: 5461 7841 5049 0103 0000 002e 041e 0448  TaxAPI.........H
+0000d1a0: 0438 0431 043a 0430 0020 043f 043e 043b  .8.1.:.0. .?.>.;
+0000d1b0: 0443 0447 0435 043d 0438 044f 0020 0447  .C.G.5.=.8.O. .G
+0000d1c0: 0435 043a 0430 003a 0020 0800 0000 0006  .5.:.0.:. ......
+0000d1d0: 0000 0013 4765 7420 7469 636b 6574 2066  ....Get ticket f
+0000d1e0: 6169 6c65 643a 2007 0000 000b 536c 6970  ailed: .....Slip
+0000d1f0: 7354 6178 4150 4901 0300 0000 3404 1e04  sTaxAPI.....4...
+0000d200: 4804 3804 3104 3a04 3000 2004 3f04 3e04  H.8.1.:.0. .?.>.
+0000d210: 3b04 4304 4704 3504 3d04 3804 4f00 2000  ;.C.G.5.=.8.O. .
+0000d220: 6900 6400 2004 4704 3504 3a04 3000 3a00  i.d. .G.5.:.0.:.
+0000d230: 2008 0000 0000 0600 0000 1647 6574 2074   ..........Get t
+0000d240: 6963 6b65 7420 6964 2066 6169 6c65 643a  icket id failed:
+0000d250: 2007 0000 000b 536c 6970 7354 6178 4150   .....SlipsTaxAP
+0000d260: 4901 0300 0000 7c04 1d04 3504 3204 3504  I.....|...5.2.5.
+0000d270: 4004 3d04 3004 4f00 2004 3404 3b04 3804  @.=.0.O. .4.;.8.
+0000d280: 3d04 3000 2004 1804 1d04 1d00 2e00 2004  =.0. ......... .
+0000d290: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+0000d2a0: 3d04 3e00 2004 3f04 3e04 3b04 4304 4704  =.>. .?.>.;.C.G.
+0000d2b0: 3804 4204 4c00 2004 3d04 3004 3804 3c04  8.B.L. .=.0.8.<.
+0000d2c0: 3504 3d04 3e04 3204 3004 3d04 3804 3500  5.=.>.2.0.=.8.5.
+0000d2d0: 2004 3a04 3e04 3c04 3f04 3004 3d04 3804   .:.>.<.?.0.=.8.
+0000d2e0: 3800 2e08 0000 0000 0600 0000 3049 6e63  8...........0Inc
+0000d2f0: 6f72 7265 6374 206c 656e 6774 6820 6f66  orrect length of
+0000d300: 2049 4e4e 2e20 4361 6e27 7420 6765 7420   INN. Can't get 
+0000d310: 636f 6d70 616e 7920 6e61 6d65 2e07 0000  company name....
+0000d320: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000d330: 0000 5604 1d04 3504 4200 2000 5300 6500  ..V...5.B. .S.e.
+0000d340: 7300 7300 6900 6f00 6e00 4900 6400 2004  s.s.i.o.n.I.d. .
+0000d350: 3404 3b04 4f00 2004 3704 3004 3304 4004  4.;.O. .7.0.3.@.
+0000d360: 4304 3704 3a04 3800 2004 4704 3504 3a04  C.7.:.8. .G.5.:.
+0000d370: 3000 2004 4100 2004 4104 3004 3904 4204  0. .A. .A.0.9.B.
+0000d380: 3000 2004 2404 1d04 2108 0000 0000 0600  0. .$...!.......
+0000d390: 0000 224e 6f20 5275 7373 6961 6e20 5461  .."No Russian Ta
+0000d3a0: 7820 5365 7373 696f 6e49 6420 6176 6169  x SessionId avai
+0000d3b0: 6c61 626c 6507 0000 000b 536c 6970 7354  lable.....SlipsT
+0000d3c0: 6178 4150 4901 0300 0000 3604 1d04 3504  axAPI.....6...5.
+0000d3d0: 4200 2004 3004 3a04 4204 3804 3204 3d04  B. .0.:.B.8.2.=.
+0000d3e0: 3e04 3900 2004 4104 3504 4104 4104 3804  >.9. .A.5.A.A.8.
+0000d3f0: 3800 2004 3404 3b04 4f00 2004 2404 1d04  8. .4.;.O. .$...
+0000d400: 2108 0000 0000 0600 0000 184e 6f20 7661  !..........No va
+0000d410: 6c69 6420 7365 7373 696f 6e20 7072 6573  lid session pres
+0000d420: 656e 7407 0000 000b 536c 6970 7354 6178  ent.....SlipsTax
+0000d430: 4150 4901 0300 0000 7a04 1e04 3f04 3504  API.....z...?.5.
+0000d440: 4004 3004 4604 3804 4f00 2004 3e04 3104  @.0.F.8.O. .>.1.
+0000d450: 4004 3004 3104 3004 4204 4b04 3204 3004  @.0.1.0.B.K.2.0.
+0000d460: 3504 4204 4104 4f00 2004 3d04 3000 2004  5.B.A.O. .=.0. .
+0000d470: 4104 4204 3e04 4004 3e04 3d04 3500 2004  A.B.>.@.>.=.5. .
+0000d480: 4104 3504 4004 3204 3504 4004 3000 2e00  A.5.@.2.5.@.0...
+0000d490: 2004 1f04 3e04 3204 4204 3e04 4004 4f04   ...>.2.B.>.@.O.
+0000d4a0: 4e00 2004 3504 4904 5100 2004 4004 3004  N. .5.I.Q. .@.0.
+0000d4b0: 3700 2e08 0000 0000 0600 0000 384f 7065  7...........8Ope
+0000d4c0: 7261 7469 6f6e 206d 6967 6874 2062 6520  ration might be 
+0000d4d0: 7065 6e64 696e 6720 6f6e 2073 6572 7665  pending on serve
+0000d4e0: 7220 7369 6465 2e20 5472 7969 6e67 2061  r side. Trying a
+0000d4f0: 6761 696e 2e07 0000 000b 536c 6970 7354  gain......SlipsT
+0000d500: 6178 4150 4901 0300 0000 2804 1e04 3104  axAPI.....(...1.
+0000d510: 3d04 3e04 3204 3b04 3504 3d04 3804 3500  =.>.2.;.5.=.8.5.
+0000d520: 2004 4104 3504 4104 4104 3804 3800 2e00   .A.5.A.A.8.8...
+0000d530: 2e00 2e08 0000 0000 0600 0000 1552 6566  .............Ref
+0000d540: 7265 7368 696e 6720 7365 7373 696f 6e2e  reshing session.
+0000d550: 2e2e 0700 0000 0b53 6c69 7073 5461 7841  .......SlipsTaxA
+0000d560: 5049 0103 0000 0024 0421 0435 0441 0441  PI.....$.!.5.A.A
+0000d570: 0438 044f 0020 043e 0431 043d 043e 0432  .8.O. .>.1.=.>.2
+0000d580: 043b 0435 043d 0430 003a 0020 0800 0000  .;.5.=.0.:. ....
+0000d590: 0006 0000 0013 5365 7373 696f 6e20 7265  ......Session re
+0000d5a0: 6672 6573 6865 643a 2007 0000 000b 536c  freshed: .....Sl
+0000d5b0: 6970 7354 6178 4150 4901 0300 0000 1804  ipsTaxAPI.......
+0000d5c0: 2704 3504 3a00 2004 3d04 3004 3904 3404  '.5.:. .=.0.9.4.
+0000d5d0: 3504 3d00 3a00 2008 0000 0000 0600 0000  5.=.:. .........
+0000d5e0: 0c53 6c69 7020 666f 756e 643a 2007 0000  .Slip found: ...
+0000d5f0: 000b 536c 6970 7354 6178 4150 4901 0300  ..SlipsTaxAPI...
+0000d600: 0000 1c04 2704 3504 3a00 2004 3704 3004  ....'.5.:. .7.0.
+0000d610: 3304 4004 4304 3604 3504 3d00 3a00 2008  3.@.C.6.5.=.:. .
+0000d620: 0000 0000 0600 0000 0d53 6c69 7020 6c6f  .........Slip lo
+0000d630: 6164 6564 3a20 0700 0000 0b53 6c69 7073  aded: .....Slips
+0000d640: 5461 7841 5049 0103 0000 0036 041d 0435  TaxAPI.....6...5
+0000d650: 0430 0432 0442 043e 0440 0438 0437 043e  .0.2.B.>.@.8.7.>
+0000d660: 0432 0430 043d 043e 0020 043f 043e 0020  .2.0.=.>. .?.>. 
+0000d670: 043f 0440 0438 0447 0438 043d 0435 003a  .?.@.8.G.8.=.5.:
+0000d680: 0020 0800 0000 0006 0000 001a 556e 6175  . ..........Unau
+0000d690: 7468 6f72 697a 6564 2077 6974 6820 7265  thorized with re
+0000d6a0: 6173 6f6e 3a20 0700 0000 0b53 6c69 7073  ason: .....Slips
+0000d6b0: 5461 7841 5049 0103 0000 001c 0421 0447  TaxAPI.......!.G
+0000d6c0: 0451 0442 0020 043d 0435 0020 0432 044b  .Q.B. .=.5. .2.K
+0000d6d0: 0431 0440 0430 043d 0800 0000 0006 0000  .1.@.0.=........
+0000d6e0: 0014 4163 636f 756e 7420 6e6f 7420 7365  ..Account not se
+0000d6f0: 6c65 6374 6564 0700 0000 0953 7461 7465  lected.....State
+0000d700: 6d65 6e74 0103 0000 0034 0414 0430 043d  ment.....4...0.=
+0000d710: 043d 044b 0435 0020 043d 0435 0020 043f  .=.K.5. .=.5. .?
+0000d720: 0440 0438 0432 044f 0437 0430 043d 044b  .@.8.2.O.7.0.=.K
+0000d730: 0020 043a 0020 0426 0411 003a 0020 0800  . .:. .&...:. ..
+0000d740: 0000 0006 0000 0023 4173 7365 7420 6461  .......#Asset da
+0000d750: 7461 2061 7265 6e27 7420 6c69 6e6b 6564  ta aren't linked
+0000d760: 2074 6f20 6173 7365 743a 2007 0000 0009   to asset: .....
+0000d770: 5374 6174 656d 656e 7401 0300 0000 1e04  Statement.......
+0000d780: 2604 1100 2000 6900 6400 2004 3d04 3500  &... .i.d. .=.5.
+0000d790: 2004 3d04 3004 3904 3404 3504 3d08 0000   .=.0.9.4.5.=...
+0000d7a0: 0000 0600 0000 1241 7373 6574 2069 6420  .......Asset id 
+0000d7b0: 6e6f 7420 666f 756e 6407 0000 0009 5374  not found.....St
+0000d7c0: 6174 656d 656e 7401 0300 0000 3204 1d04  atement.....2...
+0000d7d0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000d7e0: 3e00 2004 4104 3e04 3704 3404 3004 4204  >. .A.>.7.4.0.B.
+0000d7f0: 4c00 2004 4104 4704 5104 4200 3a00 2008  L. .A.G.Q.B.:. .
+0000d800: 0000 0000 0600 0000 1643 616e 2774 2063  .........Can't c
+0000d810: 7265 6174 6520 6163 636f 756e 743a 2007  reate account: .
+0000d820: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d830: 0000 2e04 1d04 3504 3204 3e04 3704 3c04  ......5.2.>.7.<.
+0000d840: 3e04 3604 3d04 3e00 2004 4104 3e04 3704  >.6.=.>. .A.>.7.
+0000d850: 3404 3004 4204 4c00 2004 2604 1100 3a00  4.0.B.L. .&...:.
+0000d860: 2008 0000 0000 0600 0000 1443 616e 2774   ..........Can't
+0000d870: 2063 7265 6174 6520 6173 7365 743a 2007   create asset: .
+0000d880: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d890: 0000 3c04 1d04 3504 3204 3e04 3704 3c04  ..<...5.2.>.7.<.
+0000d8a0: 3e04 3604 3d04 3e00 2004 3d04 3004 3904  >.6.=.>. .=.0.9.
+0000d8b0: 4204 3500 2004 2604 1100 2004 3200 2004  B.5. .&... .2. .
+0000d8c0: 3e04 4204 4704 5104 4204 3500 3a00 2008  >.B.G.Q.B.5.:. .
+0000d8d0: 0000 0000 0600 0000 2643 616e 2774 206c  ........&Can't l
+0000d8e0: 6f63 6174 6520 6173 7365 7420 696e 2073  ocate asset in s
+0000d8f0: 7461 7465 6d65 6e74 2064 6174 613a 2007  tatement data: .
+0000d900: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000d910: 0000 1a04 1f04 3e04 3404 4204 3204 3504  ......>.4.B.2.5.
+0000d920: 4004 3604 3404 3504 3d04 3804 3508 0000  @.6.4.5.=.8.5...
+0000d930: 0000 0600 0000 0c43 6f6e 6669 726d 6174  .......Confirmat
+0000d940: 696f 6e07 0000 0009 5374 6174 656d 656e  ion.....Statemen
+0000d950: 7401 0300 0000 4404 1e04 4204 3b04 3004  t.....D...B.;.0.
+0000d960: 3404 3e04 4704 3d04 3004 4f00 2004 3804  4.>.G.=.0.O. .8.
+0000d970: 3d04 4404 3e04 4004 3c04 3004 4604 3804  =.D.>.@.<.0.F.8.
+0000d980: 4f00 2004 4104 3e04 4504 4004 3004 3d04  O. .A.>.E.@.0.=.
+0000d990: 3504 3d04 3000 2004 3200 2008 0000 0000  5.=.0. .2. .....
+0000d9a0: 0600 0000 1e44 6562 7567 2069 6e66 6f72  .....Debug infor
+0000d9b0: 6d61 7469 6f6e 2069 7320 7361 7665 6420  mation is saved 
+0000d9c0: 696e 2007 0000 0009 5374 6174 656d 656e  in .....Statemen
+0000d9d0: 7401 0300 0000 1004 1404 3504 3f04 3e04  t.........5.?.>.
+0000d9e0: 3704 3804 4200 2008 0000 0000 0600 0000  7.8.B. .........
+0000d9f0: 0b44 6570 6f73 6974 206f 6620 0700 0000  .Deposit of ....
+0000da00: 0953 7461 7465 6d65 6e74 0103 0000 0048  .Statement.....H
+0000da10: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000da20: 043d 043e 0020 043f 0440 043e 0447 0438  .=.>. .?.@.>.G.8
+0000da30: 0442 0430 0442 044c 0020 004a 0053 004f  .B.0.B.L. .J.S.O
+0000da40: 004e 0020 0438 0437 0020 0444 0430 0439  .N. .8.7. .D.0.9
+0000da50: 043b 0430 003a 0020 0800 0000 0006 0000  .;.0.:. ........
+0000da60: 001f 4661 696c 6564 2074 6f20 7265 6164  ..Failed to read
+0000da70: 204a 534f 4e20 6672 6f6d 2066 696c 653a   JSON from file:
+0000da80: 2007 0000 0009 5374 6174 656d 656e 7401   .....Statement.
+0000da90: 0300 0000 4804 1d04 3500 2004 4304 3404  ....H...5. .C.4.
+0000daa0: 3004 3b04 3e04 4104 4c00 2004 3f04 4004  0.;.>.A.L. .?.@.
+0000dab0: 3e04 4704 3804 4204 3004 4204 4c00 2004  >.G.8.B.0.B.L. .
+0000dac0: 4104 4504 3504 3c04 4300 2000 4a00 5300  A.E.5.<.C. .J.S.
+0000dad0: 4f00 4e00 2004 3804 3700 3a00 2008 0000  O.N. .8.7.:. ...
+0000dae0: 0000 0600 0000 2146 6169 6c65 6420 746f  ......!Failed to
+0000daf0: 2072 6561 6420 4a53 4f4e 2073 6368 656d   read JSON schem
+0000db00: 6120 6672 6f6d 3a20 0700 0000 0953 7461  a from: .....Sta
+0000db10: 7465 6d65 6e74 0103 0000 0034 041d 0435  tement.....4...5
+0000db20: 0432 043e 0437 043c 043e 0436 043d 043e  .2.>.7.<.>.6.=.>
+0000db30: 0020 043f 0440 043e 0447 0435 0441 0442  . .?.@.>.G.5.A.B
+0000db40: 044c 0020 0444 0430 0439 043b 003a 0020  .L. .D.0.9.;.:. 
+0000db50: 0800 0000 0006 0000 0015 4661 696c 6564  ..........Failed
+0000db60: 2074 6f20 7265 6164 2066 696c 653a 2007   to read file: .
+0000db70: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000db80: 0000 5a04 1e04 4804 3804 3104 3a04 3000  ..Z...H.8.1.:.0.
+0000db90: 2004 3f04 4004 3800 2004 4104 3e04 4504   .?.@.8. .A.>.E.
+0000dba0: 4004 3004 3d04 3504 3d04 3804 3800 2004  @.0.=.5.=.8.8. .
+0000dbb0: 3e04 4204 3b04 3004 3404 3e04 4704 3d04  >.B.;.0.4.>.G.=.
+0000dbc0: 3e04 3900 2004 3804 3d04 4404 3e04 4004  >.9. .8.=.D.>.@.
+0000dbd0: 3c04 3004 4604 3804 3800 3a00 2008 0000  <.0.F.8.8.:. ...
+0000dbe0: 0000 0600 0000 2546 6169 6c65 6420 746f  ......%Failed to
+0000dbf0: 2077 7269 7465 2073 7461 7465 6d65 6e74   write statement
+0000dc00: 2064 756d 7020 696e 746f 3a20 0700 0000   dump into: ....
+0000dc10: 0953 7461 7465 6d65 6e74 0103 0000 0066  .Statement.....f
+0000dc20: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000dc30: 043d 043e 0020 043a 043e 043d 0442 0432  .=.>. .:.>.=.B.2
+0000dc40: 0435 0440 0442 0438 0440 043e 0432 0430  .5.@.B.8.@.>.2.0
+0000dc50: 0442 044c 0020 0442 0438 043f 0020 0430  .B.L. .B.8.?. .0
+0000dc60: 043a 0442 0438 0432 0430 0020 0432 0020  .:.B.8.2.0. .2. 
+0000dc70: 0442 0440 0430 043d 0441 0444 0435 0440  .B.@.0.=.A.D.5.@
+0000dc80: 0435 003a 0020 0800 0000 0006 0000 002e  .5.:. ..........
+0000dc90: 496d 706f 7373 6962 6c65 2074 6f20 636f  Impossible to co
+0000dca0: 6e76 6572 7420 6173 7365 7420 7479 7065  nvert asset type
+0000dcb0: 2069 6e20 7472 616e 7366 6572 3a20 0700   in transfer: ..
+0000dcc0: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000dcd0: 0048 041d 0435 043e 0434 043d 043e 0437  .H...5.>.4.=.>.7
+0000dce0: 043d 0430 0447 043d 043e 0435 0020 0441  .=.0.G.=.>.5. .A
+0000dcf0: 043e 0432 043f 0430 0434 0435 043d 0438  .>.2.?.0.4.5.=.8
+0000dd00: 0435 0020 0432 0430 043b 044e 0442 044b  .5. .2.0.;.N.B.K
+0000dd10: 0020 0434 043b 044f 0020 0800 0000 0006  . .4.;.O. ......
+0000dd20: 0000 001c 4d75 6c74 6970 6c65 2063 7572  ....Multiple cur
+0000dd30: 7265 6e63 7920 6d61 7463 6820 666f 7220  rency match for 
+0000dd40: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000dd50: 0000 003a 041d 0435 043e 0434 043d 043e  ...:...5.>.4.=.>
+0000dd60: 0437 043d 0430 0447 043d 043e 0435 0020  .7.=.0.G.=.>.5. 
+0000dd70: 0441 043e 0432 043f 0430 0434 0435 043d  .A.>.2.?.0.4.5.=
+0000dd80: 0438 0435 0020 0434 043b 044f 0020 0800  .8.5. .4.;.O. ..
+0000dd90: 0000 0006 0000 0013 4d75 6c74 6970 6c65  ........Multiple
+0000dda0: 206d 6174 6368 2066 6f72 2007 0000 0009   match for .....
+0000ddb0: 5374 6174 656d 656e 7401 0300 0000 3a04  Statement.....:.
+0000ddc0: 1204 4b04 3104 3504 4004 3804 4204 3500  ..K.1.5.@.8.B.5.
+0000ddd0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000dde0: 4f00 2004 3704 3004 4704 3804 4104 3b04  O. .7.0.G.8.A.;.
+0000ddf0: 3504 3d04 3804 4f00 3a08 0000 0000 0600  5.=.8.O.:.......
+0000de00: 0000 1d53 656c 6563 7420 6163 636f 756e  ...Select accoun
+0000de10: 7420 746f 2064 6570 6f73 6974 2074 6f3a  t to deposit to:
+0000de20: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000de30: 0000 0036 0412 044b 0431 0435 0440 0438  ...6...K.1.5.@.8
+0000de40: 0442 0435 0020 0441 0447 0451 0442 0020  .B.5. .A.G.Q.B. 
+0000de50: 0434 043b 044f 0020 0441 043f 0438 0441  .4.;.O. .A.?.8.A
+0000de60: 0430 043d 0438 044f 003a 0800 0000 0006  .0.=.8.O.:......
+0000de70: 0000 0020 5365 6c65 6374 2061 6363 6f75  ... Select accou
+0000de80: 6e74 2074 6f20 7769 7468 6472 6177 2066  nt to withdraw f
+0000de90: 726f 6d3a 0700 0000 0953 7461 7465 6d65  rom:.....Stateme
+0000dea0: 6e74 0103 0000 0048 041d 0435 043a 043e  nt.....H...5.:.>
+0000deb0: 0442 043e 0440 044b 0435 0020 0441 0435  .B.>.@.K.5. .A.5
+0000dec0: 043a 0446 0438 0438 0020 043d 0435 0020  .:.F.8.8. .=.5. 
+0000ded0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+0000dee0: 0432 0430 044e 0442 0441 044f 003a 0020  .2.0.N.B.A.O.:. 
+0000def0: 0800 0000 0006 0000 0021 536f 6d65 2073  .........!Some s
+0000df00: 6563 7469 6f6e 7320 6172 6520 6e6f 7420  ections are not 
+0000df10: 7375 7070 6f72 7465 643a 2007 0000 0009  supported: .....
+0000df20: 5374 6174 656d 656e 7401 0300 0000 2a04  Statement.....*.
+0000df30: 1804 3c04 3f04 3e04 4004 4200 2004 3e04  ..<.?.>.@.B. .>.
+0000df40: 4204 4704 5104 4204 3000 2004 3f04 4004  B.G.Q.B.0. .?.@.
+0000df50: 3504 4004 3204 3004 3d08 0000 0000 0600  5.@.2.0.=.......
+0000df60: 0000 1e53 7461 7465 6d65 6e74 2069 6d70  ...Statement imp
+0000df70: 6f72 7420 7761 7320 6361 6e63 656c 6c65  ort was cancelle
+0000df80: 6407 0000 0009 5374 6174 656d 656e 7401  d.....Statement.
+0000df90: 0300 0000 2c04 1d04 3504 3204 3504 4004  ....,...5.2.5.@.
+0000dfa0: 3d04 4b04 3900 2004 3f04 3504 4004 3804  =.K.9. .?.5.@.8.
+0000dfb0: 3e04 3400 2004 3e04 4204 4704 5104 4204  >.4. .>.B.G.Q.B.
+0000dfc0: 3008 0000 0000 0600 0000 1b53 7461 7465  0..........State
+0000dfd0: 6d65 6e74 2070 6572 696f 6420 6973 2069  ment period is i
+0000dfe0: 6e76 616c 6964 0700 0000 0953 7461 7465  nvalid.....State
+0000dff0: 6d65 6e74 0103 0000 00c6 041f 0435 0440  ment.........5.@
+0000e000: 0438 043e 0434 0020 043e 0442 0447 0451  .8.>.4. .>.B.G.Q
+0000e010: 0442 0430 0020 043d 0430 0447 0438 043d  .B.0. .=.0.G.8.=
+0000e020: 0430 0435 0442 0441 044f 0020 0440 0430  .0.5.B.A.O. .@.0
+0000e030: 043d 0435 0435 0020 043f 043e 0441 043b  .=.5.5. .?.>.A.;
+0000e040: 0435 0434 043d 0435 0439 0020 043e 043f  .5.4.=.5.9. .>.?
+0000e050: 0435 0440 0430 0446 0438 0438 0020 0434  .5.@.0.F.8.8. .4
+0000e060: 043b 044f 0020 0441 0447 0451 0442 0430  .;.O. .A.G.Q.B.0
+0000e070: 0020 0028 043f 043e 0432 0442 043e 0440  . .(.?.>.2.B.>.@
+0000e080: 043d 044b 0439 0020 0438 043c 043f 043e  .=.K.9. .8.<.?.>
+0000e090: 0440 0442 003f 0029 002e 0020 041f 0440  .@.B.?.)... ...@
+0000e0a0: 043e 0434 043e 043b 0436 0438 0442 044c  .>.4.>.;.6.8.B.L
+0000e0b0: 0020 0438 043c 043f 043e 0440 0442 003f  . .8.<.?.>.@.B.?
+0000e0c0: 0800 0000 0006 0000 0058 5374 6174 656d  .........XStatem
+0000e0d0: 656e 7420 7065 7269 6f64 2073 7461 7274  ent period start
+0000e0e0: 7320 6265 666f 7265 206c 6173 7420 7265  s before last re
+0000e0f0: 636f 7264 6564 206f 7065 7261 7469 6f6e  corded operation
+0000e100: 2066 6f72 2074 6865 2061 6363 6f75 6e74   for the account
+0000e110: 2e20 436f 6e74 696e 7565 2069 6d70 6f72  . Continue impor
+0000e120: 743f 0700 0000 0953 7461 7465 6d65 6e74  t?.....Statement
+0000e130: 0103 0000 002a 041e 0442 0447 0451 0442  .....*...B.G.Q.B
+0000e140: 0020 0441 043e 0434 0435 0440 0436 0438  . .A.>.4.5.@.6.8
+0000e150: 0442 0020 043e 0448 0438 0431 043a 0438  .B. .>.H.8.1.:.8
+0000e160: 0800 0000 0006 0000 001b 5374 6174 656d  ..........Statem
+0000e170: 656e 7420 7661 6c69 6461 7469 6f6e 2066  ent validation f
+0000e180: 6169 6c65 6407 0000 0009 5374 6174 656d  ailed.....Statem
+0000e190: 656e 7401 0300 0000 4004 2104 3804 3c04  ent.....@.!.8.<.
+0000e1a0: 3204 3e04 3b00 2004 3204 3004 3b04 4e04  2.>.;. .2.0.;.N.
+0000e1b0: 4204 4b00 2004 3d04 3500 2004 3f04 4004  B.K. .=.5. .?.@.
+0000e1c0: 3804 3204 4f04 3704 3004 3d00 2004 3a00  8.2.O.7.0.=. .:.
+0000e1d0: 2004 2604 1100 3a00 2008 0000 0000 0600   .&...:. .......
+0000e1e0: 0000 2753 796d 626f 6c20 6375 7272 656e  ..'Symbol curren
+0000e1f0: 6379 2069 736e 2774 206c 696e 6b65 6420  cy isn't linked 
+0000e200: 746f 2061 7373 6574 3a20 0700 0000 0953  to asset: .....S
+0000e210: 7461 7465 6d65 6e74 0103 0000 0032 0421  tatement.....2.!
+0000e220: 0438 043c 0432 043e 043b 0020 043d 0435  .8.<.2.>.;. .=.5
+0000e230: 0020 043f 0440 0438 0432 044f 0437 0430  . .?.@.8.2.O.7.0
+0000e240: 043d 0020 043a 0020 0426 0411 003a 0020  .=. .:. .&...:. 
+0000e250: 0800 0000 0006 0000 0025 5379 6d62 6f6c  .........%Symbol
+0000e260: 2074 6963 6b65 7220 6973 6e27 7420 6c69   ticker isn't li
+0000e270: 6e6b 6564 2074 6f20 6173 7365 743a 2007  nked to asset: .
+0000e280: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000e290: 0000 7204 1d04 3504 3204 3e04 3704 3c04  ..r...5.2.>.7.<.
+0000e2a0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
+0000e2b0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
+0000e2c0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000e2d0: 4f00 2004 3a04 3e04 4004 3f04 3e04 4004  O. .:.>.@.?.>.@.
+0000e2e0: 3004 4204 3804 3204 3d04 3e04 3304 3e00  0.B.8.2.=.>.3.>.
+0000e2f0: 2004 3404 3504 3904 4104 4204 3204 3804   .4.5.9.A.B.2.8.
+0000e300: 4f00 3a00 2008 0000 0000 0600 0000 2855  O.:. .........(U
+0000e310: 6e6d 6174 6368 6564 2061 6363 6f75 6e74  nmatched account
+0000e320: 2066 6f72 2063 6f72 706f 7261 7465 2061   for corporate a
+0000e330: 6374 696f 6e3a 2007 0000 0009 5374 6174  ction: .....Stat
+0000e340: 656d 656e 7401 0300 0000 7404 1d04 3504  ement.....t...5.
+0000e350: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+0000e360: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
+0000e370: 3204 3804 4204 4c00 2004 4104 4704 5104  2.8.B.L. .A.G.Q.
+0000e380: 4200 2004 3404 3b04 4f00 2004 3e04 3f04  B. .4.;.O. .>.?.
+0000e390: 3504 4004 3004 4604 3804 3800 2004 3f04  5.@.0.F.8.8. .?.
+0000e3a0: 4004 3804 4504 3e04 3404 3000 2f04 4004  @.8.E.>.4.0./.@.
+0000e3b0: 3004 4104 4504 3e04 3404 3000 3a00 2008  0.A.E.>.4.0.:. .
+0000e3c0: 0000 0000 0600 0000 2755 6e6d 6174 6368  ........'Unmatch
+0000e3d0: 6564 2061 6363 6f75 6e74 2066 6f72 2069  ed account for i
+0000e3e0: 6e63 6f6d 652f 7370 656e 6469 6e67 3a20  ncome/spending: 
+0000e3f0: 0700 0000 0953 7461 7465 6d65 6e74 0103  .....Statement..
+0000e400: 0000 0052 041d 0435 0432 043e 0437 043c  ...R...5.2.>.7.<
+0000e410: 043e 0436 043d 043e 0020 0441 043e 043f  .>.6.=.>. .A.>.?
+0000e420: 043e 0441 0442 0430 0432 0438 0442 044c  .>.A.B.0.2.8.B.L
+0000e430: 0020 0441 0447 0451 0442 0020 0434 043b  . .A.G.Q.B. .4.;
+0000e440: 044f 0020 0432 044b 043f 043b 0430 0442  .O. .2.K.?.;.0.B
+0000e450: 044b 003a 0020 0800 0000 0006 0000 001f  .K.:. ..........
+0000e460: 556e 6d61 7463 6865 6420 6163 636f 756e  Unmatched accoun
+0000e470: 7420 666f 7220 7061 796d 656e 743a 2007  t for payment: .
+0000e480: 0000 0009 5374 6174 656d 656e 7401 0300  ....Statement...
+0000e490: 0000 5004 1d04 3504 3204 3e04 3704 3c04  ..P...5.2.>.7.<.
+0000e4a0: 3e04 3604 3d04 3e00 2004 4104 3e04 3f04  >.6.=.>. .A.>.?.
+0000e4b0: 3e04 4104 4204 3004 3204 3804 4204 4c00  >.A.B.0.2.8.B.L.
+0000e4c0: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+0000e4d0: 4f00 2004 4104 3404 3504 3b04 3a04 3800  O. .A.4.5.;.:.8.
+0000e4e0: 3a00 2008 0000 0000 0600 0000 1d55 6e6d  :. ..........Unm
+0000e4f0: 6174 6368 6564 2061 6363 6f75 6e74 2066  atched account f
+0000e500: 6f72 2074 7261 6465 3a20 0700 0000 0953  or trade: .....S
+0000e510: 7461 7465 6d65 6e74 0103 0000 0054 041d  tatement.....T..
+0000e520: 0435 0432 0437 043e 043c 043e 0436 043d  .5.2.7.>.<.>.6.=
+0000e530: 043e 0020 0441 043e 043f 043e 0441 0442  .>. .A.>.?.>.A.B
+0000e540: 0430 0432 0438 0442 044c 0020 0441 0447  .0.2.8.B.L. .A.G
+0000e550: 0451 0442 0020 0434 043b 044f 0020 043f  .Q.B. .4.;.O. .?
+0000e560: 0435 0440 0435 0432 043e 0434 0430 003a  .5.@.5.2.>.4.0.:
+0000e570: 0020 0800 0000 0006 0000 0020 556e 6d61  . ......... Unma
+0000e580: 7463 6865 6420 6163 636f 756e 7420 666f  tched account fo
+0000e590: 7220 7472 616e 7366 6572 3a20 0700 0000  r transfer: ....
+0000e5a0: 0953 7461 7465 6d65 6e74 0103 0000 006e  .Statement.....n
+0000e5b0: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000e5c0: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+0000e5d0: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
+0000e5e0: 0411 0020 0434 043b 044f 0020 043a 043e  ... .4.;.O. .:.>
+0000e5f0: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
+0000e600: 043d 043e 0433 043e 0020 0434 0435 0439  .=.>.3.>. .4.5.9
+0000e610: 0441 0442 0432 0438 044f 003a 0020 0800  .A.B.2.8.O.:. ..
+0000e620: 0000 0006 0000 0026 556e 6d61 7463 6865  .......&Unmatche
+0000e630: 6420 6173 7365 7420 666f 7220 636f 7270  d asset for corp
+0000e640: 6f72 6174 6520 6163 7469 6f6e 3a20 0700  orate action: ..
+0000e650: 0000 0953 7461 7465 6d65 6e74 0103 0000  ...Statement....
+0000e660: 004e 041d 0435 0432 043e 0437 043c 043e  .N...5.2.>.7.<.>
+0000e670: 0436 043d 043e 0020 0441 043e 043f 043e  .6.=.>. .A.>.?.>
+0000e680: 0441 0442 0430 0432 0438 0442 044c 0020  .A.B.0.2.8.B.L. 
+0000e690: 0426 0411 0020 0434 043b 044f 0020 0432  .&... .4.;.O. .2
+0000e6a0: 044b 043f 043b 0430 0442 044b 003a 0020  .K.?.;.0.B.K.:. 
+0000e6b0: 0800 0000 0006 0000 001d 556e 6d61 7463  ..........Unmatc
+0000e6c0: 6865 6420 6173 7365 7420 666f 7220 7061  hed asset for pa
+0000e6d0: 796d 656e 743a 2007 0000 0009 5374 6174  yment: .....Stat
+0000e6e0: 656d 656e 7401 0300 0000 4c04 1d04 3504  ement.....L...5.
+0000e6f0: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+0000e700: 2004 4104 3e04 3f04 3e04 4104 4204 3004   .A.>.?.>.A.B.0.
+0000e710: 3204 3804 4204 4c00 2004 2604 1100 2004  2.8.B.L. .&... .
+0000e720: 3404 3b04 4f00 2004 4104 3404 3504 3b04  4.;.O. .A.4.5.;.
+0000e730: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
+0000e740: 1b55 6e6d 6174 6368 6564 2061 7373 6574  .Unmatched asset
+0000e750: 2066 6f72 2074 7261 6465 3a20 0700 0000   for trade: ....
+0000e760: 0953 7461 7465 6d65 6e74 0103 0000 005e  .Statement.....^
+0000e770: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+0000e780: 043d 043e 0020 0441 043e 043f 043e 0441  .=.>. .A.>.?.>.A
+0000e790: 0442 0430 0432 0438 0442 044c 0020 0426  .B.0.2.8.B.L. .&
+0000e7a0: 0411 002f 0432 0430 043b 044e 0442 0443  .../.2.0.;.N.B.C
+0000e7b0: 0020 0434 043b 044f 0020 043f 0435 0440  . .4.;.O. .?.5.@
+0000e7c0: 0435 0432 043e 0434 0430 003a 0020 0800  .5.2.>.4.0.:. ..
+0000e7d0: 0000 0006 0000 001e 556e 6d61 7463 6865  ........Unmatche
+0000e7e0: 6420 6173 7365 7420 666f 7220 7472 616e  d asset for tran
+0000e7f0: 7366 6572 3a20 0700 0000 0953 7461 7465  sfer: .....State
+0000e800: 6d65 6e74 0103 0000 006c 041d 0435 0432  ment.....l...5.2
+0000e810: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000e820: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e830: 0438 0442 044c 0020 043a 0430 0442 0435  .8.B.L. .:.0.B.5
+0000e840: 0433 043e 0440 0438 044e 0020 0434 043b  .3.>.@.8.N. .4.;
+0000e850: 044f 0020 043f 0440 0438 0445 043e 0434  .O. .?.@.8.E.>.4
+0000e860: 0430 002f 0440 0430 0441 0445 043e 0434  .0./.@.0.A.E.>.4
+0000e870: 0430 003a 0020 0800 0000 0006 0000 0028  .0.:. .........(
+0000e880: 556e 6d61 7463 6865 6420 6361 7465 676f  Unmatched catego
+0000e890: 7279 2066 6f72 2069 6e63 6f6d 652f 7370  ry for income/sp
+0000e8a0: 656e 6469 6e67 3a20 0700 0000 0953 7461  ending: .....Sta
+0000e8b0: 7465 6d65 6e74 0103 0000 0050 041d 0435  tement.....P...5
+0000e8c0: 0432 043e 0437 043c 043e 043d 043e 0020  .2.>.7.<.>.=.>. 
+0000e8d0: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e8e0: 0438 0442 044c 0020 0432 0430 043b 044e  .8.B.L. .2.0.;.N
+0000e8f0: 0442 0443 0020 0434 043b 044f 0020 0441  .B.C. .4.;.O. .A
+0000e900: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+0000e910: 0006 0000 0020 556e 6d61 7463 6865 6420  ..... Unmatched 
+0000e920: 6375 7272 656e 6379 2066 6f72 2061 6363  currency for acc
+0000e930: 6f75 6e74 3a20 0700 0000 0953 7461 7465  ount: .....State
+0000e940: 6d65 6e74 0103 0000 0082 041d 0435 0432  ment.........5.2
+0000e950: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000e960: 0441 043e 043f 043e 0441 0442 0430 0432  .A.>.?.>.A.B.0.2
+0000e970: 0438 0442 044c 0020 043a 043e 043d 0442  .8.B.L. .:.>.=.B
+0000e980: 0440 0430 0433 0435 043d 0442 0430 0020  .@.0.3.5.=.B.0. 
+0000e990: 0434 043b 044f 0020 043e 043f 0435 0440  .4.;.O. .>.?.5.@
+0000e9a0: 0430 0446 0438 0438 0020 043f 0440 0438  .0.F.8.8. .?.@.8
+0000e9b0: 0445 043e 0434 0430 002f 0440 0430 0441  .E.>.4.0./.@.0.A
+0000e9c0: 0445 043e 0434 0430 003a 0020 0800 0000  .E.>.4.0.:. ....
+0000e9d0: 0006 0000 0024 556e 6d61 7463 6865 6420  .....$Unmatched 
+0000e9e0: 7065 6572 2066 6f72 2069 6e63 6f6d 652f  peer for income/
+0000e9f0: 7370 656e 6469 6e67 3a20 0700 0000 0953  spending: .....S
+0000ea00: 7461 7465 6d65 6e74 0103 0000 0052 041d  tatement.....R..
+0000ea10: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+0000ea20: 0438 0432 0430 0435 043c 043e 0435 0020  .8.2.0.5.<.>.5. 
+0000ea30: 043a 043e 0440 043f 043e 0440 0430 0442  .:.>.@.?.>.@.0.B
+0000ea40: 0438 0432 043d 043e 0435 0020 0434 0435  .8.2.=.>.5. .4.5
+0000ea50: 0439 0441 0442 0432 0438 0435 003a 0020  .9.A.B.2.8.5.:. 
+0000ea60: 0800 0000 0006 0000 001e 556e 7375 7070  ..........Unsupp
+0000ea70: 6f72 7465 6420 636f 7270 6f72 6174 6520  orted corporate 
+0000ea80: 6163 7469 6f6e 3a20 0700 0000 0953 7461  action: .....Sta
+0000ea90: 7465 6d65 6e74 0103 0000 003c 041d 0435  tement.....<...5
+0000eaa0: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+0000eab0: 0432 0430 0435 043c 044b 0439 0020 0442  .2.0.5.<.K.9. .B
+0000eac0: 0438 043f 0020 0432 044b 043f 043b 0430  .8.?. .2.K.?.;.0
+0000ead0: 0442 044b 003a 0020 0800 0000 0006 0000  .B.K.:. ........
+0000eae0: 001a 556e 7375 7070 6f72 7465 6420 7061  ..Unsupported pa
+0000eaf0: 796d 656e 7420 7479 7065 3a20 0700 0000  yment type: ....
+0000eb00: 0953 7461 7465 6d65 6e74 0103 0000 0012  .Statement......
+0000eb10: 0421 043f 0438 0441 0430 043d 0438 0435  .!.?.8.A.0.=.8.5
+0000eb20: 0020 0800 0000 0006 0000 000e 5769 7468  . ..........With
+0000eb30: 6472 6177 616c 206f 6620 0700 0000 0953  drawal of .....S
+0000eb40: 7461 7465 6d65 6e74 0103 0000 0044 002a  tatement.....D.*
+0000eb50: 002a 002a 0020 041d 0415 041e 0411 0425  .*.*. .........%
+0000eb60: 041e 0414 0418 041c 0410 0020 0420 0423  ........... . .#
+0000eb70: 0427 041d 0410 042f 0020 041f 0420 041e  .'...../. ... ..
+0000eb80: 0412 0415 0420 041a 0410 0020 002a 002a  ..... ..... .*.*
+0000eb90: 002a 0800 0000 0006 0000 001d 2a2a 2a20  .*..........*** 
+0000eba0: 4d41 4e55 414c 2045 4e54 5259 2052 4551  MANUAL ENTRY REQ
+0000ebb0: 5549 5245 4420 2a2a 2a07 0000 000d 5374  UIRED ***.....St
+0000ebc0: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000ebd0: 3404 2204 3804 3f00 2004 2604 1100 2004  4.".8.?. .&... .
+0000ebe0: 3d04 3500 2004 3f04 3e04 3404 3404 3504  =.5. .?.>.4.4.5.
+0000ebf0: 4004 3604 3804 3204 3004 3504 4204 4104  @.6.8.2.0.5.B.A.
+0000ec00: 4f00 3a00 2008 0000 0000 0600 0000 1c41  O.:. ..........A
+0000ec10: 7373 6574 2074 7970 6520 6973 6e27 7420  sset type isn't 
+0000ec20: 7375 7070 6f72 7465 643a 2007 0000 000d  supported: .....
+0000ec30: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000ec40: 0000 2e04 1a04 3e04 3c04 3804 4104 4104  ......>.<.8.A.A.
+0000ec50: 3804 3800 2000 4300 4600 4400 2004 3704  8.8. .C.F.D. .7.
+0000ec60: 3004 4004 4304 3604 3504 3d04 4b00 3a00  0.@.C.6.5.=.K.:.
+0000ec70: 2008 0000 0000 0600 0000 1443 4644 2063   ..........CFD c
+0000ec80: 6861 7267 6573 206c 6f61 6465 643a 2007  harges loaded: .
+0000ec90: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000eca0: 5201 0300 0000 6204 2204 4d04 3300 2000  R.....b.".M.3. .
+0000ecb0: 4600 6c00 6500 7800 5300 7400 6100 7400  F.l.e.x.S.t.a.t.
+0000ecc0: 6500 6d00 6500 6e00 7400 2004 3d04 3500  e.m.e.n.t. .=.5.
+0000ecd0: 2004 3d04 3004 3904 3404 3504 3d00 2004   .=.0.9.4.5.=. .
+0000ece0: 3200 2004 3f04 3504 4004 3204 4b04 4500  2. .?.5.@.2.K.E.
+0000ecf0: 2000 7b00 7d00 2004 3104 3004 3904 4204   .{.}. .1.0.9.B.
+0000ed00: 3004 4500 2000 7b00 7d08 0000 0000 0600  0.E. .{.}.......
+0000ed10: 0000 3243 616e 2774 2066 696e 6420 6120  ..2Can't find a 
+0000ed20: 466c 6578 5374 6174 656d 656e 7420 696e  FlexStatement in
+0000ed30: 2066 6972 7374 207b 7d20 6279 7465 7320   first {} bytes 
+0000ed40: 6f66 207b 7d07 0000 000d 5374 6174 656d  of {}.....Statem
+0000ed50: 656e 7449 424b 5201 0300 0000 4804 1d04  entIBKR.....H...
+0000ed60: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000ed70: 3e00 2004 3d04 3004 3904 4204 3800 2004  >. .=.0.9.B.8. .
+0000ed80: 3f04 3b04 3004 4204 5104 3600 2004 3404  ?.;.0.B.Q.6. .4.
+0000ed90: 3b04 4f00 2004 3e04 4204 3c04 3504 3d04  ;.O. .>.B.<.5.=.
+0000eda0: 4b00 3a00 2008 0000 0000 0600 0000 1f43  K.:. ..........C
+0000edb0: 616e 2774 2066 696e 6420 6d61 7463 6820  an't find match 
+0000edc0: 666f 7220 7265 7665 7273 616c 3a20 0700  for reversal: ..
+0000edd0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000ede0: 0103 0000 0046 041d 0435 0432 043e 0437  .....F...5.2.>.7
+0000edf0: 043c 043e 0436 043d 043e 0020 043d 0430  .<.>.6.=.>. .=.0
+0000ee00: 0439 0442 0438 0020 043f 0430 0440 043d  .9.B.8. .?.0.@.=
+0000ee10: 0443 044e 0020 0437 0430 043f 0438 0441  .C.N. .7.0.?.8.A
+0000ee20: 044c 0020 0434 043b 044f 0020 0800 0000  .L. .4.;.O. ....
+0000ee30: 0006 0000 001d 4361 6e27 7420 6669 6e64  ......Can't find
+0000ee40: 2070 6169 7265 6420 7265 636f 7264 2066   paired record f
+0000ee50: 6f72 2007 0000 000d 5374 6174 656d 656e  or .....Statemen
+0000ee60: 7449 424b 5201 0300 0000 4e04 1d04 3504  tIBKR.....N...5.
+0000ee70: 3204 3e04 3c04 3e04 3604 3d04 3e00 2004  2.>.<.>.6.=.>. .
+0000ee80: 3e04 3f04 4004 3504 3404 3504 3b04 3804  >.?.@.5.4.5.;.8.
+0000ee90: 4204 4c00 2004 3204 3004 3b04 4e04 4204  B.L. .2.0.;.N.B.
+0000eea0: 4300 2004 3404 3b04 4f00 2004 4104 4704  C. .4.;.O. .A.G.
+0000eeb0: 5104 4204 3000 3a00 2008 0000 0000 0600  Q.B.0.:. .......
+0000eec0: 0000 2843 616e 2774 2067 6574 2061 6363  ..(Can't get acc
+0000eed0: 6f75 6e74 2063 7572 7265 6e63 7920 666f  ount currency fo
+0000eee0: 7220 6163 636f 756e 743a 2007 0000 000d  r account: .....
+0000eef0: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000ef00: 0000 7004 1d04 3504 3204 3e04 3704 3c04  ..p...5.2.>.7.<.
+0000ef10: 3e04 3604 3d04 3e00 2004 3e04 3f04 4004  >.6.=.>. .>.?.@.
+0000ef20: 3504 3404 3504 3b04 3804 4204 4c00 2004  5.4.5.;.8.B.L. .
+0000ef30: 3204 3004 3b04 4e04 4204 4b00 2004 3404  2.0.;.N.B.K. .4.
+0000ef40: 3b04 4f00 2004 3e04 3f04 3504 4004 3004  ;.O. .>.?.5.@.0.
+0000ef50: 4604 3804 3800 2004 3e04 3104 3c04 3504  F.8.8. .>.1.<.5.
+0000ef60: 3d04 3000 2004 3204 3004 3b04 4e04 4200  =.0. .2.0.;.N.B.
+0000ef70: 3a00 2008 0000 0000 0600 0000 2c43 616e  :. .........,Can
+0000ef80: 2774 2067 6574 2063 7572 7265 6e63 6965  't get currencie
+0000ef90: 7320 666f 7220 6375 7272 656e 6379 2065  s for currency e
+0000efa0: 7863 6861 6e67 653a 2007 0000 000d 5374  xchange: .....St
+0000efb0: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000efc0: 6804 1d04 3504 3204 3e04 3704 3c04 3e04  h...5.2.>.7.<.>.
+0000efd0: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+0000efe0: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
+0000eff0: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
+0000f000: 1e04 3104 4a04 3504 3404 3804 3d04 3504  ..1.J.5.4.8.=.5.
+0000f010: 3d04 3804 4f00 2004 3a04 3e04 3c04 3f04  =.8.O. .:.>.<.?.
+0000f020: 3004 3d04 3804 3900 2008 0000 0000 0600  0.=.8.9. .......
+0000f030: 0000 1f43 616e 2774 2070 6172 7365 204d  ...Can't parse M
+0000f040: 6572 6765 7220 6465 7363 7269 7074 696f  erger descriptio
+0000f050: 6e20 0700 0000 0d53 7461 7465 6d65 6e74  n .....Statement
+0000f060: 4942 4b52 0103 0000 0064 041d 0435 0432  IBKR.....d...5.2
+0000f070: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000f080: 0440 0430 0441 043f 043e 0437 043d 0430  .@.0.A.?.>.7.=.0
+0000f090: 0442 044c 0020 043e 043f 0438 0441 0430  .B.L. .>.?.8.A.0
+0000f0a0: 043d 0438 0435 0020 0412 044b 0434 0435  .=.8.5. ...K.4.5
+0000f0b0: 043b 0435 043d 0438 044f 0020 043a 043e  .;.5.=.8.O. .:.>
+0000f0c0: 043c 043f 0430 043d 0438 0438 0020 0800  .<.?.0.=.8.8. ..
+0000f0d0: 0000 0006 0000 0021 4361 6e27 7420 7061  .......!Can't pa
+0000f0e0: 7273 6520 5370 696e 2d6f 6666 2064 6573  rse Spin-off des
+0000f0f0: 6372 6970 7469 6f6e 2007 0000 000d 5374  cription .....St
+0000f100: 6174 656d 656e 7449 424b 5201 0300 0000  atementIBKR.....
+0000f110: 4c04 1d04 3504 3204 3e04 3704 3c04 3e04  L...5.2.>.7.<.>.
+0000f120: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+0000f130: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
+0000f140: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
+0000f150: 2104 3f04 3b04 3804 4204 3000 2008 0000  !.?.;.8.B.0. ...
+0000f160: 0000 0600 0000 1e43 616e 2774 2070 6172  .......Can't par
+0000f170: 7365 2053 706c 6974 2064 6573 6372 6970  se Split descrip
+0000f180: 7469 6f6e 2007 0000 000d 5374 6174 656d  tion .....Statem
+0000f190: 656e 7449 424b 5201 0300 0000 6204 1d04  entIBKR.....b...
+0000f1a0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+0000f1b0: 3e00 2004 4004 3004 4104 3f04 3e04 3704  >. .@.0.A.?.>.7.
+0000f1c0: 3d04 3004 4204 4c00 2004 3e04 3f04 3804  =.0.B.L. .>.?.8.
+0000f1d0: 4104 3004 3d04 3804 3500 2004 1404 3804  A.0.=.8.5. ...8.
+0000f1e0: 3204 3804 3404 3504 3d04 3404 3000 2004  2.8.4.5.=.4.0. .
+0000f1f0: 3004 3a04 4604 3804 4f04 3c04 3800 2008  0.:.F.8.O.<.8. .
+0000f200: 0000 0000 0600 0000 2743 616e 2774 2070  ........'Can't p
+0000f210: 6172 7365 2053 746f 636b 2044 6976 6964  arse Stock Divid
+0000f220: 656e 6420 6465 7363 7269 7074 696f 6e20  end description 
+0000f230: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+0000f240: 4b52 0103 0000 005a 041d 0435 0432 043e  KR.....Z...5.2.>
+0000f250: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
+0000f260: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
+0000f270: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
+0000f280: 0438 0435 0020 0421 043c 0435 043d 044b  .8.5. .!.<.5.=.K
+0000f290: 0020 0441 0438 043c 0432 043e 043b 0430  . .A.8.<.2.>.;.0
+0000f2a0: 0020 0800 0000 0006 0000 0026 4361 6e27  . .........&Can'
+0000f2b0: 7420 7061 7273 6520 5379 6d62 6f6c 2043  t parse Symbol C
+0000f2c0: 6861 6e67 6520 6465 7363 7269 7074 696f  hange descriptio
+0000f2d0: 6e20 0700 0000 0d53 7461 7465 6d65 6e74  n .....Statement
+0000f2e0: 4942 4b52 0103 0000 006e 041d 0435 0432  IBKR.....n...5.2
+0000f2f0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+0000f300: 043e 0431 0440 0430 0431 043e 0442 0430  .>.1.@.0.1.>.B.0
+0000f310: 0442 044c 0020 043e 0442 043c 0435 043d  .B.L. .>.B.<.5.=
+0000f320: 0451 043d 043d 043e 0435 0020 043a 043e  .Q.=.=.>.5. .:.>
+0000f330: 0440 043f 043e 0440 0430 0442 0438 0432  .@.?.>.@.0.B.8.2
+0000f340: 043d 043e 0435 0020 0434 0435 0439 0441  .=.>.5. .4.5.9.A
+0000f350: 0442 0432 0438 0435 0800 0000 0006 0000  .B.2.8.5........
+0000f360: 0028 4361 6e27 7420 7072 6f63 6573 7320  .(Can't process 
+0000f370: 6361 6e63 656c 6c65 6420 636f 7270 6f72  cancelled corpor
+0000f380: 6174 6520 6163 7469 6f6e 0700 0000 0d53  ate action.....S
+0000f390: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000f3a0: 003e 0414 0435 043d 0435 0436 043d 044b  .>...5.=.5.6.=.K
+0000f3b0: 0435 0020 0442 0440 0430 043d 0437 0430  .5. .B.@.0.=.7.0
+0000f3c0: 043a 0446 0438 0438 0020 0437 0430 0433  .:.F.8.8. .7.0.3
+0000f3d0: 0440 0443 0436 0435 043d 044b 003a 0020  .@.C.6.5.=.K.:. 
+0000f3e0: 0800 0000 0006 0000 001a 4361 7368 2074  ..........Cash t
+0000f3f0: 7261 6e73 6163 7469 6f6e 7320 6c6f 6164  ransactions load
+0000f400: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
+0000f410: 6e74 4942 4b52 0103 0000 005e 0422 0438  ntIBKR.....^.".8
+0000f420: 043f 0020 043a 043e 0440 043f 043e 0440  .?. .:.>.@.?.>.@
+0000f430: 0430 0442 0438 0432 043d 043e 0433 043e  .0.B.8.2.=.>.3.>
+0000f440: 0020 0434 0435 0439 0441 0442 0432 0438  . .4.5.9.A.B.2.8
+0000f450: 044f 0020 043d 0435 0020 043f 043e 0434  .O. .=.5. .?.>.4
+0000f460: 0434 0435 0440 0436 0438 0432 0430 0435  .4.5.@.6.8.2.0.5
+0000f470: 0442 0441 044f 003a 0020 0800 0000 0006  .B.A.O.:. ......
+0000f480: 0000 0028 436f 7270 6f72 6174 6520 6163  ...(Corporate ac
+0000f490: 7469 6f6e 2074 7970 6520 6973 206e 6f74  tion type is not
+0000f4a0: 2073 7570 706f 7274 6564 3a20 0700 0000   supported: ....
+0000f4b0: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000f4c0: 0000 0044 041a 043e 0440 043f 043e 0440  ...D...>.@.?.>.@
+0000f4d0: 0430 0442 0438 0432 043d 044b 0435 0020  .0.B.8.2.=.K.5. 
+0000f4e0: 0434 0435 0439 0441 0442 0432 0438 044f  .4.5.9.A.B.2.8.O
+0000f4f0: 0020 0437 0430 0433 0440 0443 0436 0435  . .7.0.3.@.C.6.5
+0000f500: 043d 044b 003a 0020 0800 0000 0006 0000  .=.K.:. ........
+0000f510: 001a 436f 7270 6f72 6174 6520 6163 7469  ..Corporate acti
+0000f520: 6f6e 7320 6c6f 6164 6564 3a20 0700 0000  ons loaded: ....
+0000f530: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000f540: 0000 0056 0414 0438 0432 0438 0434 0435  ...V...8.2.8.4.5
+0000f550: 043d 0434 0020 043d 0435 0020 043d 0430  .=.4. .=.5. .=.0
+0000f560: 0439 0434 0435 043d 0020 0434 043b 044f  .9.4.5.=. .4.;.O
+0000f570: 0020 0443 0434 0435 0440 0436 0430 043d  . .C.4.5.@.6.0.=
+0000f580: 043d 043e 0433 043e 0020 043d 0430 043b  .=.>.3.>. .=.0.;
+0000f590: 043e 0433 0430 003a 0020 0800 0000 0006  .>.3.0.:. ......
+0000f5a0: 0000 0028 4469 7669 6465 6e64 206e 6f74  ...(Dividend not
+0000f5b0: 2066 6f75 6e64 2066 6f72 2077 6974 6868   found for withh
+0000f5c0: 6f6c 6469 6e67 2074 6178 3a20 0700 0000  olding tax: ....
+0000f5d0: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000f5e0: 0000 002e 0049 0042 004b 0052 0020 0066  .....I.B.K.R. .f
+0000f5f0: 006c 0065 0078 002d 043e 0442 0447 0451  .l.e.x.-.>.B.G.Q
+0000f600: 0442 0020 0028 002a 002e 0078 006d 006c  .B. .(.*...x.m.l
+0000f610: 0029 0800 0000 0006 0000 0017 4942 4b52  .)..........IBKR
+0000f620: 2066 6c65 782d 7175 6572 7920 282a 2e78   flex-query (*.x
+0000f630: 6d6c 2907 0000 000d 5374 6174 656d 656e  ml).....Statemen
+0000f640: 7449 424b 5201 0300 0000 2600 4900 6e00  tIBKR.....&.I.n.
+0000f650: 7400 6500 7200 6100 6300 7400 6900 7600  t.e.r.a.c.t.i.v.
+0000f660: 6500 2000 4200 7200 6f00 6b00 6500 7200  e. .B.r.o.k.e.r.
+0000f670: 7308 0000 0000 0600 0000 1349 6e74 6572  s..........Inter
+0000f680: 6163 7469 7665 2042 726f 6b65 7273 0700  active Brokers..
+0000f690: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f6a0: 0103 0000 0056 0422 0438 043f 0020 043e  .....V.".8.?. .>
+0000f6b0: 0442 0447 0451 0442 0430 0020 0049 006e  .B.G.Q.B.0. .I.n
+0000f6c0: 0074 0065 0072 0061 0063 0074 0069 0076  .t.e.r.a.c.t.i.v
+0000f6d0: 0065 0020 0042 0072 006f 006b 0065 0072  .e. .B.r.o.k.e.r
+0000f6e0: 0073 0020 043d 0435 0020 043e 043f 0440  .s. .=.5. .>.?.@
+0000f6f0: 0435 0434 0435 043b 0451 043d 0800 0000  .5.4.5.;.Q.=....
+0000f700: 0006 0000 0029 496e 7465 7261 6374 6976  .....)Interactiv
+0000f710: 6520 4272 6f6b 6572 7320 7265 706f 7274  e Brokers report
+0000f720: 2074 7970 6520 6e6f 7420 666f 756e 6407   type not found.
+0000f730: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+0000f740: 5201 0300 0000 3a04 1704 3004 3304 4004  R.....:...0.3.@.
+0000f750: 4304 3704 3a04 3000 2004 3e04 4204 4704  C.7.:.0. .>.B.G.
+0000f760: 5104 4204 3000 2000 4900 4200 2004 3404  Q.B.0. .I.B. .4.
+0000f770: 3b04 4f00 2004 4104 4704 5104 4204 3000  ;.O. .A.G.Q.B.0.
+0000f780: 2008 0000 0000 0600 0000 234c 6f61 6420   .........#Load 
+0000f790: 4942 2046 6c65 782d 7374 6174 656d 656e  IB Flex-statemen
+0000f7a0: 7420 666f 7220 6163 636f 756e 7420 0700  t for account ..
+0000f7b0: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f7c0: 0103 0000 0058 041d 0435 0434 043e 0441  .....X...5.4.>.A
+0000f7d0: 0442 0430 0442 043e 0447 043d 043e 0020  .B.0.B.>.G.=.>. 
+0000f7e0: 0434 0430 043d 043d 044b 0445 0020 043e  .4.0.=.=.K.E. .>
+0000f7f0: 0431 0020 041e 0431 044a 0435 0434 0438  .1. ...1.J.5.4.8
+0000f800: 043d 0435 043d 0438 0438 0020 043a 043e  .=.5.=.8.8. .:.>
+0000f810: 043c 043f 0430 043d 0438 0439 0020 0800  .<.?.0.=.8.9. ..
+0000f820: 0000 0006 0000 0022 4d65 7267 6572 2064  ......."Merger d
+0000f830: 6573 6372 6970 7469 6f6e 206d 6973 7320  escription miss 
+0000f840: 736f 6d65 2064 6174 6120 0700 0000 0d53  some data .....S
+0000f850: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000f860: 005e 041d 0435 043e 0434 043d 043e 0437  .^...5.>.4.=.>.7
+0000f870: 043d 0430 0447 043d 043e 0435 0020 0441  .=.0.G.=.>.5. .A
+0000f880: 043e 0432 043f 0430 0434 0435 043d 0438  .>.2.?.0.4.5.=.8
+0000f890: 0435 0020 0441 043e 0431 044b 0442 0438  .5. .A.>.1.K.B.8
+0000f8a0: 0439 0020 0440 0435 043e 0440 0433 0430  .9. .@.5.>.@.3.0
+0000f8b0: 043d 0438 0437 0430 0446 0438 0438 0020  .=.8.7.0.F.8.8. 
+0000f8c0: 0800 0000 0006 0000 0029 4d75 6c74 6970  .........)Multip
+0000f8d0: 6c65 206d 6572 6765 7220 7265 636f 7264  le merger record
+0000f8e0: 7320 616c 7265 6164 7920 6578 6973 7420  s already exist 
+0000f8f0: 6174 2007 0000 000d 5374 6174 656d 656e  at .....Statemen
+0000f900: 7449 424b 5201 0300 0000 5204 1404 3504  tIBKR.....R...5.
+0000f910: 3904 4104 4204 3204 3804 3500 2004 3d04  9.A.B.2.8.5. .=.
+0000f920: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
+0000f930: 3604 3804 3204 3004 3504 4204 4104 4f00  6.8.2.0.5.B.A.O.
+0000f940: 2004 3404 3b04 4f00 2004 3e04 3f04 4604   .4.;.O. .>.?.F.
+0000f950: 3804 3e04 3d04 3e04 3200 3a00 2008 0000  8.>.=.>.2.:. ...
+0000f960: 0000 0600 0000 274f 7074 696f 6e20 4526  ......'Option E&
+0000f970: 4126 4520 6163 7469 6f6e 2069 736e 2774  A&E action isn't
+0000f980: 2069 6d70 6c65 6d65 6e74 6564 3a20 0700   implemented: ..
+0000f990: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+0000f9a0: 0103 0000 003a 0418 0441 043f 043e 043b  .....:...A.?.>.;
+0000f9b0: 043d 0435 043d 0438 0435 0020 043f 0440  .=.5.=.8.5. .?.@
+0000f9c0: 043e 0434 0430 043d 043d 043e 0433 043e  .>.4.0.=.=.>.3.>
+0000f9d0: 0020 043e 043f 0446 0438 043e 043d 0430  . .>.?.F.8.>.=.0
+0000f9e0: 0800 0000 0006 0000 0011 4f70 7469 6f6e  ..........Option
+0000f9f0: 2061 7373 6967 6e6d 656e 7407 0000 000d   assignment.....
+0000fa00: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000fa10: 0000 3a04 1804 4104 3f04 3e04 3b04 3d04  ..:...A.?.>.;.=.
+0000fa20: 3504 3d04 3804 3500 2f04 4d04 3a04 4104  5.=.8.5./.M.:.A.
+0000fa30: 3f04 3804 4004 3004 4604 3804 4f00 2004  ?.8.@.0.F.8.O. .
+0000fa40: 3e04 3f04 4604 3804 3e04 3d04 3008 0000  >.?.F.8.>.=.0...
+0000fa50: 0000 0600 0000 1a4f 7074 696f 6e20 6173  .......Option as
+0000fa60: 7369 676e 6d65 6e74 2f65 7865 7263 6973  signment/exercis
+0000fa70: 6507 0000 000d 5374 6174 656d 656e 7449  e.....StatementI
+0000fa80: 424b 5201 0300 0000 3a04 1804 4104 3f04  BKR.....:...A.?.
+0000fa90: 3e04 3b04 3d04 3504 3d04 3804 3500 2004  >.;.=.5.=.8.5. .
+0000faa0: 3a04 4304 3f04 3b04 3504 3d04 3d04 3e04  :.C.?.;.5.=.=.>.
+0000fab0: 3304 3e00 2004 3e04 3f04 4604 3804 3e04  3.>. .>.?.F.8.>.
+0000fac0: 3d04 3008 0000 0000 0600 0000 0f4f 7074  =.0..........Opt
+0000fad0: 696f 6e20 6578 6572 6369 7365 0700 0000  ion exercise....
+0000fae0: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000faf0: 0000 0024 042d 043a 0441 043f 0438 0440  ...$.-.:.A.?.8.@
+0000fb00: 0430 0446 0438 044f 0020 043e 043f 0446  .0.F.8.O. .>.?.F
+0000fb10: 0438 043e 043d 0430 0800 0000 0006 0000  .8.>.=.0........
+0000fb20: 0011 4f70 7469 6f6e 2065 7870 6972 6174  ..Option expirat
+0000fb30: 696f 6e07 0000 000d 5374 6174 656d 656e  ion.....Statemen
+0000fb40: 7449 424b 5201 0300 0000 4004 1404 3504  tIBKR.....@...5.
+0000fb50: 3904 4104 4204 3204 3804 4f00 2004 4100  9.A.B.2.8.O. .A.
+0000fb60: 2004 3e04 3f04 4604 3804 3e04 3d04 3004   .>.?.F.8.>.=.0.
+0000fb70: 3c04 3800 2004 3704 3004 3304 4004 4304  <.8. .7.0.3.@.C.
+0000fb80: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+0000fb90: 0600 0000 164f 7074 696f 6e73 2045 2641  .....Options E&A
+0000fba0: 2645 206c 6f61 6465 643a 2007 0000 000d  &E loaded: .....
+0000fbb0: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000fbc0: 0000 6a04 1d04 3500 2004 3d04 3004 3904  ..j...5. .=.0.9.
+0000fbd0: 3404 3504 3d04 3000 2004 4104 3404 3504  4.5.=.0. .A.4.5.
+0000fbe0: 3b04 3a04 3000 2004 3404 3b04 4f00 2004  ;.:.0. .4.;.O. .
+0000fbf0: 3804 4104 3f04 3e04 3b04 3d04 3504 3d04  8.A.?.>.;.=.5.=.
+0000fc00: 3804 4f00 2f04 4d04 3a04 4104 3f04 3804  8.O./.M.:.A.?.8.
+0000fc10: 4004 3004 4604 3804 3800 2004 3e04 3f04  @.0.F.8.8. .>.?.
+0000fc20: 4604 3804 3e04 3d04 3000 3a00 2008 0000  F.8.>.=.0.:. ...
+0000fc30: 0000 0600 0000 354f 7269 6769 6e61 6c20  ......5Original 
+0000fc40: 7472 6164 6520 6e6f 7420 666f 756e 6420  trade not found 
+0000fc50: 666f 7220 4f70 7469 6f6e 2045 2641 2645  for Option E&A&E
+0000fc60: 206f 7065 7261 7469 6f6e 3a20 0700 0000   operation: ....
+0000fc70: 0d53 7461 7465 6d65 6e74 4942 4b52 0103  .StatementIBKR..
+0000fc80: 0000 006c 041f 043b 0430 0442 0451 0436  ...l...;.0.B.Q.6
+0000fc90: 0020 0431 044b 043b 0020 043e 0442 043c  . .1.K.;. .>.B.<
+0000fca0: 0435 043d 0451 043d 0020 043f 043e 0020  .5.=.Q.=. .?.>. 
+0000fcb0: 043f 0440 0438 043c 0435 0440 043d 043e  .?.@.8.<.5.@.=.>
+0000fcc0: 043c 0443 0020 0441 043e 0432 043f 0430  .<.C. .A.>.2.?.0
+0000fcd0: 0434 0435 043d 0438 044e 0020 043e 043f  .4.5.=.8.N. .>.?
+0000fce0: 0438 0441 0430 043d 0438 044f 003a 0020  .8.A.0.=.8.O.:. 
+0000fcf0: 0800 0000 0006 0000 0031 5061 796d 656e  .........1Paymen
+0000fd00: 7420 7761 7320 7265 7665 7273 6564 2062  t was reversed b
+0000fd10: 7920 6170 7072 6f78 696d 6174 6520 6465  y approximate de
+0000fd20: 7363 7269 7074 696f 6e3a 2007 0000 000d  scription: .....
+0000fd30: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000fd40: 0000 6a04 1f04 3b04 3004 4204 5104 3600  ..j...;.0.B.Q.6.
+0000fd50: 2004 3104 4b04 3b00 2004 3e04 4204 3c04   .1.K.;. .>.B.<.
+0000fd60: 3504 3d04 5104 3d00 2c00 2004 3d04 3e00  5.=.Q.=.,. .=.>.
+0000fd70: 2004 4100 2004 3d04 3504 4104 3e04 3204   .A. .=.5.A.>.2.
+0000fd80: 3f04 3004 3404 3004 4e04 4904 3504 3900  ?.0.4.0.N.I.5.9.
+0000fd90: 2004 3404 3004 4204 3e04 3900 2004 3e04   .4.0.B.>.9. .>.
+0000fda0: 4204 4704 5104 4204 3000 3a00 2008 0000  B.G.Q.B.0.:. ...
+0000fdb0: 0000 0600 0000 3350 6179 6d65 6e74 2077  ......3Payment w
+0000fdc0: 6173 2072 6576 6572 7365 6420 7769 7468  as reversed with
+0000fdd0: 2064 6966 6665 7265 6e74 2072 6570 6f72   different repor
+0000fde0: 7465 6420 6461 7465 3a20 0700 0000 0d53  ted date: .....S
+0000fdf0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000fe00: 0028 041f 043b 0430 0442 0451 0436 0020  .(...;.0.B.Q.6. 
+0000fe10: 0431 044b 043b 0020 043e 0442 043c 0435  .1.K.;. .>.B.<.5
+0000fe20: 043d 0451 043d 003a 0020 0800 0000 0006  .=.Q.=.:. ......
+0000fe30: 0000 0016 5061 796d 656e 7420 7761 7320  ....Payment was 
+0000fe40: 7265 7665 7273 6564 3a20 0700 0000 0d53  reversed: .....S
+0000fe50: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+0000fe60: 001c 0426 0411 0020 0437 0430 0433 0440  ...&... .7.0.3.@
+0000fe70: 0443 0436 0435 043d 044b 003a 0020 0800  .C.6.5.=.K.:. ..
+0000fe80: 0000 0006 0000 0013 5365 6375 7269 7469  ........Securiti
+0000fe90: 6573 206c 6f61 6465 643a 2007 0000 000d  es loaded: .....
+0000fea0: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+0000feb0: 0000 5604 1d04 3504 3404 3e04 4104 4204  ..V...5.4.>.A.B.
+0000fec0: 3004 4204 3e04 4704 3d04 3e00 2004 3404  0.B.>.G.=.>. .4.
+0000fed0: 3004 3d04 3d04 4b04 4500 2004 3404 3b04  0.=.=.K.E. .4.;.
+0000fee0: 4f00 2004 1204 4b04 3404 3504 3b04 3504  O. ...K.4.5.;.5.
+0000fef0: 3d04 3804 4f00 2004 3a04 3e04 3c04 3f04  =.8.O. .:.>.<.?.
+0000ff00: 3004 3d04 3804 3800 2008 0000 0000 0600  0.=.8.8. .......
+0000ff10: 0000 2453 7069 6e2d 6f66 6620 6465 7363  ..$Spin-off desc
+0000ff20: 7269 7074 696f 6e20 6d69 7373 2073 6f6d  ription miss som
+0000ff30: 6520 6461 7461 2007 0000 000d 5374 6174  e data .....Stat
+0000ff40: 656d 656e 7449 424b 5201 0300 0000 5c04  ementIBKR.....\.
+0000ff50: 1804 4104 4504 3e04 3404 3d04 3004 4f00  ..A.E.>.4.=.0.O.
+0000ff60: 2004 2604 1100 2004 3404 3b04 4f00 2004   .&... .4.;.O. .
+0000ff70: 3204 4b04 3404 3504 3b04 3504 3d04 3804  2.K.4.5.;.5.=.8.
+0000ff80: 4f00 2004 3a04 3e04 3c04 3f04 3004 3d04  O. .:.>.<.?.0.=.
+0000ff90: 3804 3800 2004 3d04 3500 2004 3d04 3004  8.8. .=.5. .=.0.
+0000ffa0: 3904 3404 3504 3d04 3000 2008 0000 0000  9.4.5.=.0. .....
+0000ffb0: 0600 0000 2153 7069 6e2d 6f66 6620 696e  ....!Spin-off in
+0000ffc0: 6974 6961 6c20 6173 7365 7420 6e6f 7420  itial asset not 
+0000ffd0: 666f 756e 6420 0700 0000 0d53 7461 7465  found .....State
+0000ffe0: 6d65 6e74 4942 4b52 0103 0000 0056 041e  mentIBKR.....V..
+0000fff0: 0448 0438 0431 043a 0430 0020 043e 043a  .H.8.1.:.0. .>.:
+00010000: 0440 0443 0433 043b 0435 043d 0438 044f  .@.C.3.;.5.=.8.O
+00010010: 0020 0053 0070 0069 006e 002d 006f 0066  . .S.p.i.n.-.o.f
+00010020: 0066 0020 0441 043b 0438 0448 043a 043e  .f. .A.;.8.H.:.>
+00010030: 043c 0020 0431 043e 043b 044c 0448 0430  .<. .1.>.;.L.H.0
+00010040: 044f 0020 0800 0000 0006 0000 0023 5370  .O. .........#Sp
+00010050: 696e 2d6f 6666 2072 6f75 6e64 696e 6720  in-off rounding 
+00010060: 6572 726f 7220 6973 2074 6f6f 2062 6967  error is too big
+00010070: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+00010080: 424b 5201 0300 0000 3e04 1d04 3504 3404  BKR.....>...5.4.
+00010090: 3e04 4104 4204 3004 4204 3e04 4704 3d04  >.A.B.0.B.>.G.=.
+000100a0: 3e00 2004 3404 3004 3d04 3d04 4b04 4500  >. .4.0.=.=.K.E.
+000100b0: 2004 3404 3b04 4f00 2004 2104 3f04 3b04   .4.;.O. .!.?.;.
+000100c0: 3804 4204 3000 2008 0000 0000 0600 0000  8.B.0. .........
+000100d0: 2153 706c 6974 2064 6573 6372 6970 7469  !Split descripti
+000100e0: 6f6e 206d 6973 7320 736f 6d65 2064 6174  on miss some dat
+000100f0: 6120 0700 0000 0d53 7461 7465 6d65 6e74  a .....Statement
+00010100: 4942 4b52 0103 0000 0038 0417 0430 0447  IBKR.....8...0.G
+00010110: 0438 0441 043b 0435 043d 0438 0435 0020  .8.A.;.5.=.8.5. 
+00010120: 0430 043a 0446 0438 0439 0020 0437 0430  .0.:.F.8.9. .7.0
+00010130: 0433 0440 0443 0436 0435 043d 043e 003a  .3.@.C.6.5.=.>.:
+00010140: 0020 0800 0000 0006 0000 0017 5374 6f63  . ..........Stoc
+00010150: 6b20 7665 7374 696e 6773 206c 6f61 6465  k vestings loade
+00010160: 643a 2007 0000 000d 5374 6174 656d 656e  d: .....Statemen
+00010170: 7449 424b 5201 0300 0000 4804 1a04 3e04  tIBKR.....H...>.
+00010180: 4004 4004 3504 3a04 4204 3804 4004 3e04  @.@.5.:.B.8.@.>.
+00010190: 3204 3a04 3000 2004 3d04 3004 3b04 3e04  2.:.0. .=.0.;.>.
+000101a0: 3304 3000 2004 3404 3b04 4f00 2004 3404  3.0. .4.;.O. .4.
+000101b0: 3804 3204 3804 3404 3504 3d04 3404 3000  8.2.8.4.5.=.4.0.
+000101c0: 3a00 2008 0000 0000 0600 0000 1d54 6178  :. ..........Tax
+000101d0: 2061 646a 7573 746d 656e 7420 666f 7220   adjustment for 
+000101e0: 6469 7669 6465 6e64 3a20 0700 0000 0d53  dividend: .....S
+000101f0: 7461 7465 6d65 6e74 4942 4b52 0103 0000  tatementIBKR....
+00010200: 0024 041d 0430 043b 043e 0433 0438 0020  .$...0.;.>.3.8. 
+00010210: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00010220: 044b 003a 0020 0800 0000 0006 0000 000e  .K.:. ..........
+00010230: 5461 7865 7320 6c6f 6164 6564 3a20 0700  Taxes loaded: ..
+00010240: 0000 0d53 7461 7465 6d65 6e74 4942 4b52  ...StatementIBKR
+00010250: 0103 ffff ffff 0800 0000 0006 0000 000f  ................
+00010260: 5472 6164 6573 206c 6f61 6465 643a 2007  Trades loaded: .
+00010270: 0000 000d 5374 6174 656d 656e 7449 424b  ....StatementIBK
+00010280: 5201 0300 0000 5804 1d04 3504 3f04 3e04  R.....X...5.?.>.
+00010290: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+000102a0: 3504 3c04 4b04 3900 2004 4404 3e04 4004  5.<.K.9. .D.>.@.
+000102b0: 3c04 3004 4200 2004 3e04 3f04 3804 4104  <.0.B. .>.?.8.A.
+000102c0: 3004 3d04 3804 4f00 2004 3404 3804 3204  0.=.8.O. .4.8.2.
+000102d0: 3804 3404 3504 3d04 3404 3000 3a00 2008  8.4.5.=.4.0.:. .
+000102e0: 0000 0000 0600 0000 2255 6e68 616e 646c  ........"Unhandl
+000102f0: 6564 2064 6976 6964 656e 6420 7061 7474  ed dividend patt
+00010300: 6572 6e20 666f 756e 643a 2007 0000 000d  ern found: .....
+00010310: 5374 6174 656d 656e 7449 424b 5201 0300  StatementIBKR...
+00010320: 0000 4e04 1d04 3504 3f04 3e04 3404 3404  ..N...5.?.>.4.4.
+00010330: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
+00010340: 4b04 3900 2004 4404 3e04 4004 3c04 3004  K.9. .D.>.@.<.0.
+00010350: 4200 2004 4104 4204 4004 3004 3d04 4b00  B. .A.B.@.0.=.K.
+00010360: 2004 3d04 3004 3b04 3e04 3304 3000 3a00   .=.0.;.>.3.0.:.
+00010370: 2008 0000 0000 0600 0000 2555 6e68 616e   .........%Unhan
+00010380: 646c 6564 2074 6178 2063 6f75 6e74 7279  dled tax country
+00010390: 2070 6174 7465 726e 2066 6f75 6e64 3a20   pattern found: 
+000103a0: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+000103b0: 4b52 0103 0000 0052 041d 0435 043f 043e  KR.....R...5.?.>
+000103c0: 0434 0434 0435 0440 0436 0438 0432 0430  .4.4.5.@.6.8.2.0
+000103d0: 0435 043c 044b 0439 0020 0444 043e 0440  .5.<.K.9. .D.>.@
+000103e0: 043c 0430 0442 0020 043e 043f 0438 0441  .<.0.B. .>.?.8.A
+000103f0: 0430 043d 0438 044f 0020 043d 0430 043b  .0.=.8.O. .=.0.;
+00010400: 043e 0433 0430 003a 0020 0800 0000 0006  .>.3.0.:. ......
+00010410: 0000 001d 556e 6861 6e64 6c65 6420 7461  ....Unhandled ta
+00010420: 7820 7061 7474 6572 6e20 666f 756e 643a  x pattern found:
+00010430: 2007 0000 000d 5374 6174 656d 656e 7449   .....StatementI
+00010440: 424b 5201 0300 0000 4a04 1e04 3f04 3804  BKR.....J...?.8.
+00010450: 4104 3004 3d04 3804 3500 2004 3a04 3e04  A.0.=.8.5. .:.>.
+00010460: 3c04 3804 4104 4104 3804 3800 2000 4300  <.8.A.A.8.8. .C.
+00010470: 4600 4400 2004 3d04 3500 2004 4004 3004  F.D. .=.5. .@.0.
+00010480: 4104 3f04 3e04 3704 3d04 3004 3d04 3e00  A.?.>.7.=.0.=.>.
+00010490: 3a00 2008 0000 0000 0600 0000 2055 6e6b  :. ......... Unk
+000104a0: 6e6f 776e 2043 4644 2063 6861 7267 6520  nown CFD charge 
+000104b0: 6465 7363 7269 7074 696f 6e3a 2007 0000  description: ...
+000104c0: 000d 5374 6174 656d 656e 7449 424b 5201  ..StatementIBKR.
+000104d0: 0300 0000 5804 1d04 3504 3804 3704 3204  ....X...5.8.7.2.
+000104e0: 3504 4104 4204 3d04 4b04 3900 2004 4204  5.A.B.=.K.9. .B.
+000104f0: 3804 3f00 2004 3e04 4204 4704 5104 4204  8.?. .>.B.G.Q.B.
+00010500: 3000 2000 4900 6e00 7400 6500 7200 6100  0. .I.n.t.e.r.a.
+00010510: 6300 7400 6900 7600 6500 2000 4200 7200  c.t.i.v.e. .B.r.
+00010520: 6f00 6b00 6500 7200 7300 3a00 2008 0000  o.k.e.r.s.:. ...
+00010530: 0000 0600 0000 2955 6e6b 6e6f 776e 2049  ......)Unknown I
+00010540: 6e74 6572 6163 7469 7665 2042 726f 6b65  nteractive Broke
+00010550: 7273 2072 6570 6f72 7420 7479 7065 3a20  rs report type: 
+00010560: 0700 0000 0d53 7461 7465 6d65 6e74 4942  .....StatementIB
+00010570: 4b52 0103 0000 00a2 0412 044b 0020 043f  KR.........K. .?
+00010580: 044b 0442 0430 0435 0442 0435 0441 044c  .K.B.0.5.B.5.A.L
+00010590: 0020 0437 0430 0433 0440 0443 0437 0438  . .7.0.3.@.C.7.8
+000105a0: 0442 044c 0020 043e 0442 0447 0451 0442  .B.L. .>.B.G.Q.B
+000105b0: 0020 043e 0020 043f 043e 0434 0442 0432  . .>. .?.>.4.B.2
+000105c0: 0435 0440 0436 0434 0451 043d 043d 044b  .5.@.6.4.Q.=.=.K
+000105d0: 0445 0020 0441 0434 0435 043b 043a 0430  .E. .A.4.5.;.:.0
+000105e0: 0445 0020 0432 043c 0435 0441 0442 043e  .E. .2.<.5.A.B.>
+000105f0: 0020 043e 0442 0447 0451 0442 0430 0020  . .>.B.G.Q.B.0. 
+00010600: 043f 043e 0020 0410 043a 0442 0438 0432  .?.>. ...:.B.8.2
+00010610: 043d 043e 0441 0442 0438 0800 0000 0006  .=.>.A.B.8......
+00010620: 0000 003f 596f 7520 7472 7920 746f 2069  ...?You try to i
+00010630: 6d70 6f72 7420 5472 6164 6520 636f 6e66  mport Trade conf
+00010640: 696d 6174 696f 6e20 7265 706f 7274 2c20  imation report, 
+00010650: 6e6f 7420 4163 7469 7669 7479 2072 6570  not Activity rep
+00010660: 6f72 7407 0000 000d 5374 6174 656d 656e  ort.....Statemen
+00010670: 7449 424b 5201 0300 0000 5204 1d04 3504  tIBKR.....R...5.
+00010680: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00010690: 2004 4004 3004 4104 3f04 3e04 3704 3d04   .@.0.A.?.>.7.=.
+000106a0: 3004 4204 4c00 2004 3e04 3f04 3804 4104  0.B.L. .>.?.8.A.
+000106b0: 3004 3d04 3804 3500 2004 3404 3804 3204  0.=.8.5. .4.8.2.
+000106c0: 3804 3404 3504 3d04 3404 3000 2008 0000  8.4.5.=.4.0. ...
+000106d0: 0000 0600 0000 2143 616e 2774 2070 6172  ......!Can't par
+000106e0: 7365 2044 6976 6964 656e 6420 6465 7363  se Dividend desc
+000106f0: 7269 7074 696f 6e20 0700 0000 0c53 7461  ription .....Sta
+00010700: 7465 6d65 6e74 4a32 5401 0300 0000 1c04  tementJ2T.......
+00010710: 1404 2100 2004 3704 3004 3304 4004 4304  ..!. .7.0.3.@.C.
+00010720: 3604 3504 3d04 4b00 3a00 2008 0000 0000  6.5.=.K.:. .....
+00010730: 0600 0000 1643 6173 6820 6261 6c61 6e63  .....Cash balanc
+00010740: 6573 206c 6f61 6465 643a 2007 0000 000c  es loaded: .....
+00010750: 5374 6174 656d 656e 744a 3254 0103 0000  StatementJ2T....
+00010760: 003a 0414 0435 043d 0435 0436 043d 044b  .:...5.=.5.6.=.K
+00010770: 0445 0020 043e 043f 0435 0440 0430 0446  .E. .>.?.5.@.0.F
+00010780: 0438 0439 0020 0437 0430 0433 0440 0443  .8.9. .7.0.3.@.C
+00010790: 0436 0435 043d 043e 003a 0020 0800 0000  .6.5.=.>.:. ....
+000107a0: 0006 0000 0018 4361 7368 206f 7065 7261  ......Cash opera
+000107b0: 7469 6f6e 7320 6c6f 6164 6564 3a20 0700  tions loaded: ..
+000107c0: 0000 0c53 7461 7465 6d65 6e74 4a32 5401  ...StatementJ2T.
+000107d0: 0300 0000 4804 2104 3404 3504 3b04 3a04  ....H.!.4.5.;.:.
+000107e0: 3800 2004 4100 2004 3a04 4004 3804 3f04  8. .A. .:.@.8.?.
+000107f0: 4204 3e00 2d04 3204 3004 3b04 4e04 4204  B.>.-.2.0.;.N.B.
+00010800: 3004 3c04 3800 2004 3704 3004 3304 4004  0.<.8. .7.0.3.@.
+00010810: 4304 3604 3504 3d04 4b00 3a00 2008 0000  C.6.5.=.K.:. ...
+00010820: 0000 0600 0000 1643 7279 7074 6f20 7472  .......Crypto tr
+00010830: 6164 6573 206c 6f61 6465 643a 2007 0000  ades loaded: ...
+00010840: 000c 5374 6174 656d 656e 744a 3254 0103  ..StatementJ2T..
+00010850: 0000 0050 0412 0020 043e 043f 0438 0441  ...P... .>.?.8.A
+00010860: 0430 043d 0438 0438 0020 0434 0438 0432  .0.=.8.8. .4.8.2
+00010870: 0438 0434 0435 043d 0434 0430 0020 043e  .8.4.5.=.4.0. .>
+00010880: 0442 0441 0443 0442 0441 0442 0432 0443  .B.A.C.B.A.B.2.C
+00010890: 044e 0442 0020 0434 0430 043d 043d 044b  .N.B. .4.0.=.=.K
+000108a0: 0435 0020 0800 0000 0006 0000 0024 4469  .5. .........$Di
+000108b0: 7669 6465 6e64 2064 6573 6372 6970 7469  vidend descripti
+000108c0: 6f6e 206d 6973 7320 736f 6d65 2064 6174  on miss some dat
+000108d0: 6120 0700 0000 0c53 7461 7465 6d65 6e74  a .....Statement
+000108e0: 4a32 5401 0300 0000 4e04 1404 3804 3204  J2T.....N...8.2.
+000108f0: 3804 3404 3504 3d04 3400 2004 3d04 3500  8.4.5.=.4. .=.5.
+00010900: 2004 3d04 3004 3904 3404 3504 3d00 2004   .=.0.9.4.5.=. .
+00010910: 3404 3b04 4f00 2004 4104 3f04 3804 4104  4.;.O. .A.?.8.A.
+00010920: 3004 3d04 3804 4f00 2004 3d04 3004 3b04  0.=.8.O. .=.0.;.
+00010930: 3e04 3304 3000 2008 0000 0000 0600 0000  >.3.0. .........
+00010940: 1f44 6976 6964 656e 6420 666f 7220 7461  .Dividend for ta
+00010950: 7820 7761 7320 6e6f 7420 666f 756e 6420  x was not found 
+00010960: 0700 0000 0c53 7461 7465 6d65 6e74 4a32  .....StatementJ2
+00010970: 5401 0300 0000 4404 2204 4004 3004 3d04  T.....D.".@.0.=.
+00010980: 3704 3004 3a04 4604 3804 4f00 2004 3f04  7.0.:.F.8.O. .?.
+00010990: 4004 3e04 3f04 4304 4904 3504 3d04 3000  @.>.?.C.I.5.=.0.
+000109a0: 2004 3f04 4004 3800 2004 3804 3c04 3f04   .?.@.8. .8.<.?.
+000109b0: 3e04 4004 4204 3500 3a00 2008 0000 0000  >.@.B.5.:. .....
+000109c0: 0600 0000 1f49 6d70 6f72 7420 736b 6970  .....Import skip
+000109d0: 7065 6420 6f66 2074 7261 6e73 6163 7469  ped of transacti
+000109e0: 6f6e 3a20 0700 0000 0c53 7461 7465 6d65  on: .....Stateme
+000109f0: 6e74 4a32 5401 0300 0000 1400 4a00 7500  ntJ2T.......J.u.
+00010a00: 7300 7400 3200 5400 7200 6100 6400 6508  s.t.2.T.r.a.d.e.
+00010a10: 0000 0000 0600 0000 0a4a 7573 7432 5472  .........Just2Tr
+00010a20: 6164 6507 0000 000c 5374 6174 656d 656e  ade.....Statemen
+00010a30: 744a 3254 0103 0000 0032 041e 0442 0447  tJ2T.....2...B.G
+00010a40: 0451 0442 0020 004a 0075 0073 0074 0032  .Q.B. .J.u.s.t.2
+00010a50: 0054 0072 0061 0064 0065 0020 0028 002a  .T.r.a.d.e. .(.*
+00010a60: 002e 0078 006c 0073 0078 0029 0800 0000  ...x.l.s.x.)....
+00010a70: 0006 0000 001d 4a75 7374 3254 7261 6465  ......Just2Trade
+00010a80: 2073 7461 7465 6d65 6e74 2028 2a2e 786c   statement (*.xl
+00010a90: 7378 2907 0000 000c 5374 6174 656d 656e  sx).....Statemen
+00010aa0: 744a 3254 0103 0000 001c 0426 0411 0020  tJ2T.......&... 
+00010ab0: 0437 0430 0433 0440 0443 0436 0435 043d  .7.0.3.@.C.6.5.=
+00010ac0: 044b 003a 0020 0800 0000 0006 0000 0013  .K.:. ..........
+00010ad0: 5365 6375 7269 7469 6573 206c 6f61 6465  Securities loade
+00010ae0: 643a 2007 0000 000c 5374 6174 656d 656e  d: .....Statemen
+00010af0: 744a 3254 0103 0000 0038 0421 0434 0435  tJ2T.....8.!.4.5
+00010b00: 043b 043a 0438 0020 0441 0020 0430 043a  .;.:.8. .A. .0.:
+00010b10: 0446 0438 044f 043c 0438 0020 0437 0430  .F.8.O.<.8. .7.0
+00010b20: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
+00010b30: 0020 0800 0000 0006 0000 0015 5374 6f63  . ..........Stoc
+00010b40: 6b20 7472 6164 6573 206c 6f61 6465 643a  k trades loaded:
+00010b50: 2007 0000 000c 5374 6174 656d 656e 744a   .....StatementJ
+00010b60: 3254 0103 0000 0040 041d 0435 0438 0437  2T.....@...5.8.7
+00010b70: 0432 0435 0441 0442 043d 0430 044f 0020  .2.5.A.B.=.0.O. 
+00010b80: 0434 0435 043d 0435 0436 043d 0430 044f  .4.5.=.5.6.=.0.O
+00010b90: 0020 0442 0440 0430 043d 0437 0430 043a  . .B.@.0.=.7.0.:
+00010ba0: 0446 0438 044f 0020 0800 0000 0006 0000  .F.8.O. ........
+00010bb0: 001e 556e 6b6e 6f77 6e20 6361 7368 2074  ..Unknown cash t
+00010bc0: 7261 6e73 6163 7469 6f6e 2074 7970 6520  ransaction type 
+00010bd0: 0700 0000 0c53 7461 7465 6d65 6e74 4a32  .....StatementJ2
+00010be0: 5401 0300 0000 3004 1d04 3504 3804 3704  T.....0...5.8.7.
+00010bf0: 3204 3504 4104 4204 3d04 4b04 3900 2004  2.5.A.B.=.K.9. .
+00010c00: 4204 3804 3f00 2004 4104 3404 3504 3b04  B.8.?. .A.4.5.;.
+00010c10: 3a04 3800 3a00 2008 0000 0000 0600 0000  :.8.:. .........
+00010c20: 1455 6e6b 6e6f 776e 2074 7261 6465 2074  .Unknown trade t
+00010c30: 7970 653a 2007 0000 000c 5374 6174 656d  ype: .....Statem
+00010c40: 656e 744a 3254 0103 0000 004a 041d 0435  entJ2T.....J...5
+00010c50: 043f 043e 0434 0434 0435 0440 0436 0438  .?.>.4.4.5.@.6.8
+00010c60: 0432 0430 0435 043c 0430 044f 0020 0434  .2.0.5.<.0.O. .4
+00010c70: 0435 043d 0435 0436 043d 0430 044f 0020  .5.=.5.6.=.0.O. 
+00010c80: 0442 0440 0430 043d 0437 0430 043a 0446  .B.@.0.=.7.0.:.F
+00010c90: 0438 044f 0020 0800 0000 0006 0000 001e  .8.O. ..........
+00010ca0: 556e 7375 7070 706f 7274 6564 2063 6173  Unsuppported cas
+00010cb0: 6820 7472 616e 7361 6374 696f 6e20 0700  h transaction ..
+00010cc0: 0000 0c53 7461 7465 6d65 6e74 4a32 5401  ...StatementJ2T.
+00010cd0: 0300 0000 3a04 1404 3504 3d04 3504 3604  ....:...5.=.5.6.
+00010ce0: 3d04 4b04 4500 2004 3e04 3f04 3504 4004  =.K.E. .>.?.5.@.
+00010cf0: 3004 4604 3804 3900 2004 3704 3004 3304  0.F.8.9. .7.0.3.
+00010d00: 4004 4304 3604 3504 3d04 3e00 3a00 2008  @.C.6.5.=.>.:. .
+00010d10: 0000 0000 0600 0000 1843 6173 6820 6f70  .........Cash op
+00010d20: 6572 6174 696f 6e73 206c 6f61 6465 643a  erations loaded:
+00010d30: 2007 0000 000c 5374 6174 656d 656e 744b   .....StatementK
+00010d40: 4954 0103 0000 0076 041d 0430 043b 043e  IT.....v...0.;.>
+00010d50: 0433 0020 043d 0430 0020 0434 0438 0432  .3. .=.0. .4.8.2
+00010d60: 0438 0434 0435 043d 0434 044b 0020 043d  .8.4.5.=.4.K. .=
+00010d70: 0435 0020 043f 043e 0434 0434 0435 0440  .5. .?.>.4.4.5.@
+00010d80: 0436 0438 0432 0430 0435 0442 0441 044f  .6.8.2.0.5.B.A.O
+00010d90: 0020 0434 043b 044f 0020 0431 0440 043e  . .4.;.O. .1.@.>
+00010da0: 043a 0435 0440 0430 0020 041a 0418 0422  .:.5.@.0. ....."
+00010db0: 002d 0444 0438 043d 0430 043d 0441 0800  .-.D.8.=.0.=.A..
+00010dc0: 0000 0006 0000 003e 4469 7669 6465 6e64  .......>Dividend
+00010dd0: 2074 6178 6573 2061 7265 206e 6f74 2073   taxes are not s
+00010de0: 7570 706f 7274 6564 2066 6f72 204b 4954  upported for KIT
+00010df0: 2062 726f 6b65 7220 7374 6174 656d 656e   broker statemen
+00010e00: 7473 2079 6574 0700 0000 0c53 7461 7465  ts yet.....State
+00010e10: 6d65 6e74 4b49 5401 0300 0000 1404 1a04  mentKIT.........
+00010e20: 1804 2200 2004 2404 3804 3d04 3004 3d04  ..". .$.8.=.0.=.
+00010e30: 4108 0000 0000 0600 0000 0b4b 4954 2046  A..........KIT F
+00010e40: 696e 616e 6365 0700 0000 0c53 7461 7465  inance.....State
+00010e50: 6d65 6e74 4b49 5401 0300 0000 3204 1e04  mentKIT.....2...
+00010e60: 4204 4704 5104 4200 2004 1a04 1804 2200  B.G.Q.B. .....".
+00010e70: 2004 2404 3804 3d04 3004 3d04 4100 2000   .$.8.=.0.=.A. .
+00010e80: 2800 2a00 2e00 7800 6c00 7300 7800 2908  (.*...x.l.s.x.).
+00010e90: 0000 0000 0600 0000 1e4b 4954 2046 696e  .........KIT Fin
+00010ea0: 616e 6365 2073 7461 7465 6d65 6e74 2028  ance statement (
+00010eb0: 2a2e 786c 7378 2907 0000 000c 5374 6174  *.xlsx).....Stat
+00010ec0: 656d 656e 744b 4954 0103 0000 0024 0421  ementKIT.....$.!
+00010ed0: 0434 0435 043b 043a 0438 0020 0437 0430  .4.5.;.:.8. .7.0
+00010ee0: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
+00010ef0: 0020 0800 0000 0006 0000 000f 5472 6164  . ..........Trad
+00010f00: 6573 206c 6f61 6465 643a 2007 0000 000c  es loaded: .....
+00010f10: 5374 6174 656d 656e 744b 4954 0103 0000  StatementKIT....
+00010f20: 0030 041d 0435 0438 0437 0432 0435 0441  .0...5.8.7.2.5.A
+00010f30: 0442 043d 044b 0439 0020 0442 0438 043f  .B.=.K.9. .B.8.?
+00010f40: 0020 0441 0434 0435 043b 043a 0438 003a  . .A.4.5.;.:.8.:
+00010f50: 0020 0800 0000 0006 0000 0014 556e 6b6e  . ..........Unkn
+00010f60: 6f77 6e20 7472 6164 6520 7479 7065 3a20  own trade type: 
+00010f70: 0700 0000 0c53 7461 7465 6d65 6e74 4b49  .....StatementKI
+00010f80: 5401 0300 0000 4a04 1d04 3504 3f04 3e04  T.....J...5.?.>.
+00010f90: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00010fa0: 3504 3c04 3004 4f00 2004 3404 3504 3d04  5.<.0.O. .4.5.=.
+00010fb0: 3504 3604 3d04 3004 4f00 2004 4204 4004  5.6.=.0.O. .B.@.
+00010fc0: 3004 3d04 3704 3004 3a04 4604 3804 4f00  0.=.7.0.:.F.8.O.
+00010fd0: 2008 0000 0000 0600 0000 1e55 6e73 7570   ..........Unsup
+00010fe0: 7070 6f72 7465 6420 6361 7368 2074 7261  pported cash tra
+00010ff0: 6e73 6163 7469 6f6e 2007 0000 000c 5374  nsaction .....St
+00011000: 6174 656d 656e 744b 4954 0103 0000 0022  atementKIT....."
+00011010: 0421 0447 0435 0442 0430 0020 0437 0430  .!.G.5.B.0. .7.0
+00011020: 0433 0440 0443 0436 0435 043d 044b 003a  .3.@.C.6.5.=.K.:
+00011030: 0020 0800 0000 0006 0000 0011 4163 636f  . ..........Acco
+00011040: 756e 7473 206c 6f61 6465 643a 2007 0000  unts loaded: ...
+00011050: 0013 5374 6174 656d 656e 744f 7065 6e42  ..StatementOpenB
+00011060: 726f 6b65 7201 0300 0000 6404 1e04 4204  roker.....d...B.
+00011070: 4104 4304 4204 4104 4204 3204 4304 4e04  A.C.B.A.B.2.C.N.
+00011080: 4200 2004 3404 3004 3d04 3d04 4b04 3500  B. .4.0.=.=.K.5.
+00011090: 2004 3200 2004 3e04 3f04 3804 4104 3004   .2. .>.?.8.A.0.
+000110a0: 3d04 3804 3800 2004 3f04 3e04 3304 3004  =.8.8. .?.>.3.0.
+000110b0: 4804 3504 3d04 3804 4f00 2004 3e04 3104  H.5.=.8.O. .>.1.
+000110c0: 3b04 3804 3304 3004 4604 3804 3800 2008  ;.8.3.0.F.8.8. .
+000110d0: 0000 0000 0600 0000 2a42 6f6e 6420 7265  ........*Bond re
+000110e0: 7061 796d 656e 7420 6465 7363 7269 7074  payment descript
+000110f0: 696f 6e20 6d69 7373 2073 6f6d 6520 6461  ion miss some da
+00011100: 7461 2007 0000 0013 5374 6174 656d 656e  ta .....Statemen
+00011110: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00011120: 6804 1d04 3504 3204 3e04 3704 3c04 3e04  h...5.2.>.7.<.>.
+00011130: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+00011140: 3e04 3704 3d04 3004 4204 4c00 2004 3d04  >.7.=.0.B.L. .=.
+00011150: 3004 3704 3204 3004 3d04 3804 3500 2004  0.7.2.0.=.8.5. .
+00011160: 3e04 3104 3b04 3804 3304 3004 4604 3804  >.1.;.8.3.0.F.8.
+00011170: 3800 2004 3200 2004 3e04 3f04 3804 4104  8. .2. .>.?.8.A.
+00011180: 3004 3d04 3804 3800 2008 0000 0000 0600  0.=.8.8. .......
+00011190: 0000 2843 616e 2774 2064 6574 6563 7420  ..(Can't detect 
+000111a0: 626f 6e64 206e 616d 6520 6672 6f6d 2064  bond name from d
+000111b0: 6573 6372 6970 7469 6f6e 2007 0000 0013  escription .....
+000111c0: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+000111d0: 6b65 7201 0300 0000 6204 1d04 3504 3204  ker.....b...5.2.
+000111e0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+000111f0: 3e04 3f04 4004 3504 3404 3504 3b04 3804  >.?.@.5.4.5.;.8.
+00011200: 4204 4c00 2004 4204 3804 3f00 2f04 3a04  B.L. .B.8.?./.:.
+00011210: 3e04 3b04 3804 4704 3504 4104 4204 3204  >.;.8.G.5.A.B.2.
+00011220: 3e00 2004 3404 3b04 4f00 2004 4104 3404  >. .4.;.O. .A.4.
+00011230: 3504 3b04 3a04 3800 3a00 2008 0000 0000  5.;.:.8.:. .....
+00011240: 0600 0000 2543 616e 2774 2064 6574 6572  ....%Can't deter
+00011250: 6d69 6e65 2074 7261 6465 2074 7970 652f  mine trade type/
+00011260: 7175 616e 7469 7479 3a20 0700 0000 1353  quantity: .....S
+00011270: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+00011280: 6572 0103 0000 0068 041d 0435 0432 043e  er.....h...5.2.>
+00011290: 0437 043c 043e 0436 043d 043e 0020 043e  .7.<.>.6.=.>. .>
+000112a0: 043f 0440 0435 0434 0435 043b 0438 0442  .?.@.5.4.5.;.8.B
+000112b0: 044c 0020 0441 0447 0451 0442 0020 0434  .L. .A.G.Q.B. .4
+000112c0: 043b 044f 0020 0434 0435 043d 0435 0436  .;.O. .4.5.=.5.6
+000112d0: 043d 043e 0439 0020 0442 0440 0430 043d  .=.>.9. .B.@.0.=
+000112e0: 0437 0430 043a 0446 0438 0438 003a 0020  .7.0.:.F.8.8.:. 
+000112f0: 0800 0000 0006 0000 0027 4361 6e27 7420  .........'Can't 
+00011300: 6669 6e64 2061 6363 6f75 6e74 2066 6f72  find account for
+00011310: 2063 6173 6820 6f70 6572 6174 696f 6e3a   cash operation:
+00011320: 2007 0000 0013 5374 6174 656d 656e 744f   .....StatementO
+00011330: 7065 6e42 726f 6b65 7201 0300 0000 4404  penBroker.....D.
+00011340: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+00011350: 3d04 3e00 2004 3d04 3004 3904 4204 3800  =.>. .=.0.9.B.8.
+00011360: 2004 4104 4704 5104 4200 2004 3404 3b04   .A.G.Q.B. .4.;.
+00011370: 4f00 2004 4104 3404 3504 3b04 3a04 3800  O. .A.4.5.;.:.8.
+00011380: 3a00 2008 0000 0000 0600 0000 1e43 616e  :. ..........Can
+00011390: 2774 2066 696e 6420 6163 636f 756e 7420  't find account 
+000113a0: 666f 7220 7472 6164 653a 2007 0000 0013  for trade: .....
+000113b0: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+000113c0: 6b65 7201 0300 0000 5004 1d04 3504 3204  ker.....P...5.2.
+000113d0: 3e04 3704 3c04 3e04 3604 3d04 3e00 2004  >.7.<.>.6.=.>. .
+000113e0: 3d04 3004 3904 4204 3800 2004 3704 3004  =.0.9.B.8. .7.0.
+000113f0: 3f04 3804 4104 4c00 2004 4104 3f04 3804  ?.8.A.L. .A.?.8.
+00011400: 4104 3004 3d04 3804 4f00 2004 2604 1100  A.0.=.8.O. .&...
+00011410: 2004 3404 3b04 4f00 2008 0000 0000 0600   .4.;.O. .......
+00011420: 0000 2943 616e 2774 2066 696e 6420 6173  ..)Can't find as
+00011430: 7365 7420 6361 6e63 656c 6c61 7469 6f6e  set cancellation
+00011440: 2072 6563 6f72 6420 666f 7220 0700 0000   record for ....
+00011450: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+00011460: 6f6b 6572 0103 0000 0032 041d 0435 0020  oker.....2...5. 
+00011470: 043d 0430 0439 0434 0435 043d 0430 0020  .=.0.9.4.5.=.0. 
+00011480: 0426 0411 0020 0434 043b 044f 0020 043a  .&... .4.;.O. .:
+00011490: 0443 043f 043e 043d 0430 0020 0800 0000  .C.?.>.=.0. ....
+000114a0: 0006 0000 0023 4361 6e27 7420 6669 6e64  .....#Can't find
+000114b0: 2061 7373 6574 2066 6f72 2062 6f6e 6420   asset for bond 
+000114c0: 696e 7465 7265 7374 2007 0000 0013 5374  interest .....St
+000114d0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+000114e0: 7201 0300 0000 3c04 1d04 3504 3204 3e04  r.....<...5.2.>.
+000114f0: 3704 3c04 3e04 3604 3d04 3e00 2004 4104  7.<.>.6.=.>. .A.
+00011500: 3e04 3f04 3e04 4104 4204 3004 3204 3804  >.?.>.A.B.0.2.8.
+00011510: 4204 4c00 2004 2604 1100 2004 3404 3b04  B.L. .&... .4.;.
+00011520: 4f00 2008 0000 0000 0600 0000 1643 616e  O. ..........Can
+00011530: 2774 206d 6174 6368 2061 7373 6574 2066  't match asset f
+00011540: 6f72 2007 0000 0013 5374 6174 656d 656e  or .....Statemen
+00011550: 744f 7065 6e42 726f 6b65 7201 0300 0000  tOpenBroker.....
+00011560: 6604 1d04 3504 3204 3e04 3704 3c04 3e04  f...5.2.>.7.<.>.
+00011570: 3604 3d04 3e00 2004 4004 3004 4104 3f04  6.=.>. .@.0.A.?.
+00011580: 3e04 3704 3d04 3004 4204 4c00 2004 3e04  >.7.=.0.B.L. .>.
+00011590: 3f04 3804 4104 3004 3d04 3804 3500 2004  ?.8.A.0.=.8.5. .
+000115a0: 3f04 3e04 3304 3004 4804 3504 3d04 3804  ?.>.3.0.H.5.=.8.
+000115b0: 4f00 2004 3e04 3104 3b04 3804 3304 3004  O. .>.1.;.8.3.0.
+000115c0: 4604 3804 3800 2008 0000 0000 0600 0000  F.8.8. .........
+000115d0: 2443 616e 2774 2070 6172 7365 2042 6f6e  $Can't parse Bon
+000115e0: 6420 4d61 7475 7265 2064 6573 6372 6970  d Mature descrip
+000115f0: 7469 6f6e 2007 0000 0013 5374 6174 656d  tion .....Statem
+00011600: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
+00011610: 0000 4c04 1d04 3504 3204 3e04 3704 3c04  ..L...5.2.>.7.<.
+00011620: 3e04 3604 3d04 3e00 2004 4004 3004 4104  >.6.=.>. .@.0.A.
+00011630: 3f04 3e04 3704 3d04 3004 4204 4c00 2004  ?.>.7.=.0.B.L. .
+00011640: 3e04 3f04 3804 4104 3004 3d04 3804 3500  >.?.8.A.0.=.8.5.
+00011650: 2004 3a04 4304 3f04 3e04 3d04 3000 2008   .:.C.?.>.=.0. .
+00011660: 0000 0000 0600 0000 2143 616e 2774 2070  ........!Can't p
+00011670: 6172 7365 2049 6e74 6572 6573 7420 6465  arse Interest de
+00011680: 7363 7269 7074 696f 6e20 0700 0000 1353  scription .....S
+00011690: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+000116a0: 6572 0103 0000 0066 041d 0435 0432 043e  er.....f...5.2.>
+000116b0: 0437 043c 043e 0436 043d 043e 0020 0440  .7.<.>.6.=.>. .@
+000116c0: 0430 0441 043f 043e 0437 043d 0430 0442  .0.A.?.>.7.=.0.B
+000116d0: 044c 0020 043e 043f 0438 0441 0430 043d  .L. .>.?.8.A.0.=
+000116e0: 0438 0435 0020 043f 043e 0433 0430 0448  .8.5. .?.>.3.0.H
+000116f0: 0435 043d 0438 044f 0020 043e 0431 043b  .5.=.8.O. .>.1.;
+00011700: 0438 0433 0430 0446 0438 0438 0020 0800  .8.3.0.F.8.8. ..
+00011710: 0000 0006 0000 0027 4361 6e27 7420 7061  .......'Can't pa
+00011720: 7273 6520 626f 6e64 2072 6570 6179 6d65  rse bond repayme
+00011730: 6e74 2064 6573 6372 6970 7469 6f6e 2007  nt description .
+00011740: 0000 0013 5374 6174 656d 656e 744f 7065  ....StatementOpe
+00011750: 6e42 726f 6b65 7201 0300 0000 3a04 1404  nBroker.....:...
+00011760: 3504 3d04 3504 3604 3d04 4b04 4500 2004  5.=.5.6.=.K.E. .
+00011770: 3e04 3f04 3504 4004 3004 4604 3804 3900  >.?.5.@.0.F.8.9.
+00011780: 2004 3704 3004 3304 4004 4304 3604 3504   .7.0.3.@.C.6.5.
+00011790: 3d04 3e00 3a00 2008 0000 0000 0600 0000  =.>.:. .........
+000117a0: 1843 6173 6820 6f70 6572 6174 696f 6e73  .Cash operations
+000117b0: 206c 6f61 6465 643a 2007 0000 0013 5374   loaded: .....St
+000117c0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+000117d0: 7201 0300 0000 4804 1e04 4204 4104 4304  r.....H...B.A.C.
+000117e0: 4204 4104 4204 3204 4304 4e04 4200 2004  B.A.B.2.C.N.B. .
+000117f0: 3404 3004 3d04 3d04 4b04 3500 2004 3200  4.0.=.=.K.5. .2.
+00011800: 2004 3e04 3f04 3804 4104 3004 3d04 3800   .>.?.8.A.0.=.8.
+00011810: 2004 3a04 4304 3f04 3e04 3d04 3000 2008   .:.C.?.>.=.0. .
+00011820: 0000 0000 0600 0000 2449 6e74 6572 6573  ........$Interes
+00011830: 7420 6465 7363 7269 7074 696f 6e20 6d69  t description mi
+00011840: 7373 2073 6f6d 6520 6461 7461 2007 0000  ss some data ...
+00011850: 0013 5374 6174 656d 656e 744f 7065 6e42  ..StatementOpenB
+00011860: 726f 6b65 7201 0300 0000 5404 1704 3004  roker.....T...0.
+00011870: 3304 4004 4304 3704 3a04 3000 2004 3e04  3.@.C.7.:.0. .>.
+00011880: 4204 4704 5104 4204 3000 2004 1e04 4204  B.G.Q.B.0. ...B.
+00011890: 3a04 4004 4b04 4204 3804 3500 2004 3104  :.@.K.B.8.5. .1.
+000118a0: 4004 3e04 3a04 3504 4000 2004 3404 3b04  @.>.:.5.@. .4.;.
+000118b0: 4f00 2004 4104 4704 5104 4204 3000 2008  O. .A.G.Q.B.0. .
+000118c0: 0000 0000 0600 0000 274c 6f61 6420 4f70  ........'Load Op
+000118d0: 656e 2042 726f 6b65 7220 7374 6174 656d  en Broker statem
+000118e0: 656e 7420 666f 7220 6163 636f 756e 7420  ent for account 
+000118f0: 0700 0000 1353 7461 7465 6d65 6e74 4f70  .....StatementOp
+00011900: 656e 4272 6f6b 6572 0103 0000 0056 041d  enBroker.....V..
+00011910: 0430 0439 0434 0435 043d 044b 0020 043d  .0.9.4.5.=.K. .=
+00011920: 0435 0441 043a 043e 043b 044c 043a 043e  .5.A.:.>.;.L.:.>
+00011930: 0020 0437 0430 043f 0438 0441 0435 0439  . .7.0.?.8.A.5.9
+00011940: 0020 043f 043e 0433 0430 0448 0435 043d  . .?.>.3.0.H.5.=
+00011950: 0438 044f 0020 0426 0411 0020 0434 043b  .8.O. .&... .4.;
+00011960: 044f 0020 0800 0000 0006 0000 0026 4d75  .O. .........&Mu
+00011970: 6c74 6970 6c65 2061 7373 6574 2063 616e  ltiple asset can
+00011980: 6365 6c6c 6174 696f 6e20 6d61 7463 6820  cellation match 
+00011990: 666f 7220 0700 0000 1353 7461 7465 6d65  for .....Stateme
+000119a0: 6e74 4f70 656e 4272 6f6b 6572 0103 0000  ntOpenBroker....
+000119b0: 0074 041d 0435 0441 043a 043e 043b 044c  .t...5.A.:.>.;.L
+000119c0: 043a 043e 0020 0441 043e 0432 043f 0430  .:.>. .A.>.2.?.0
+000119d0: 0434 0435 043d 0438 0439 0020 0434 043b  .4.5.=.8.9. .4.;
+000119e0: 044f 0020 0441 0438 043c 0432 043e 043b  .O. .A.8.<.2.>.;
+000119f0: 0430 002c 0020 0438 0441 043f 043e 043b  .0.,. .8.A.?.>.;
+00011a00: 044c 0437 0443 0435 043c 043e 0433 043e  .L.7.C.5.<.>.3.>
+00011a10: 0020 0431 0440 043e 043a 0435 0440 043e  . .1.@.>.:.5.@.>
+00011a20: 043c 003a 0020 0800 0000 0006 0000 0022  .<.:. ........."
+00011a30: 4d75 6c74 6970 6c65 206d 6174 6368 2066  Multiple match f
+00011a40: 6f72 2062 726f 6b65 7220 7379 6d62 6f6c  or broker symbol
+00011a50: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+00011a60: 4f70 656e 4272 6f6b 6572 0103 0000 0044  OpenBroker.....D
+00011a70: 041d 0435 0441 043a 043e 043b 044c 043a  ...5.A.:.>.;.L.:
+00011a80: 043e 0020 0441 043e 0432 043f 0430 0434  .>. .A.>.2.?.0.4
+00011a90: 0435 043d 0438 0439 0020 0434 043b 044f  .5.=.8.9. .4.;.O
+00011aa0: 0020 0441 0438 043c 0432 043e 043b 0430  . .A.8.<.2.>.;.0
+00011ab0: 003a 0020 0800 0000 0006 0000 001b 4d75  .:. ..........Mu
+00011ac0: 6c74 6970 6c65 206d 6174 6368 2066 6f72  ltiple match for
+00011ad0: 2073 796d 626f 6c3a 2007 0000 0013 5374   symbol: .....St
+00011ae0: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+00011af0: 7201 0300 0000 1e04 1e04 4204 3a04 4004  r.........B.:.@.
+00011b00: 4b04 4204 3804 3500 2004 3104 4004 3e04  K.B.8.5. .1.@.>.
+00011b10: 3a04 3504 4008 0000 0000 0600 0000 0b4f  :.5.@..........O
+00011b20: 7065 6e20 4272 6f6b 6572 0700 0000 1353  pen Broker.....S
+00011b30: 7461 7465 6d65 6e74 4f70 656e 4272 6f6b  tatementOpenBrok
+00011b40: 6572 0103 0000 003c 041e 0442 0447 0451  er.....<...B.G.Q
+00011b50: 0442 0020 0431 0440 043e 043a 0435 0440  .B. .1.@.>.:.5.@
+00011b60: 0430 0020 041e 0442 043a 0440 044b 0442  .0. ...B.:.@.K.B
+00011b70: 0438 0435 0020 0028 002a 002e 0078 006d  .8.5. .(.*...x.m
+00011b80: 006c 0029 0800 0000 0006 0000 001d 4f70  .l.)..........Op
+00011b90: 656e 2042 726f 6b65 7220 7374 6174 656d  en Broker statem
+00011ba0: 656e 7420 282a 2e78 6d6c 2907 0000 0013  ent (*.xml).....
+00011bb0: 5374 6174 656d 656e 744f 7065 6e42 726f  StatementOpenBro
+00011bc0: 6b65 7201 0300 0000 5404 1704 3004 3304  ker.....T...0.3.
+00011bd0: 3e04 3b04 3e04 3204 3e04 3a00 2004 3e04  >.;.>.2.>.:. .>.
+00011be0: 4204 4704 5104 4204 3000 2004 1e04 4204  B.G.Q.B.0. ...B.
+00011bf0: 3a04 4004 4b04 4204 3804 3500 2004 3104  :.@.K.B.8.5. .1.
+00011c00: 4004 3e04 3a04 3504 4000 2004 3d04 3500  @.>.:.5.@. .=.5.
+00011c10: 2004 3d04 3004 3904 3404 3504 3d08 0000   .=.0.9.4.5.=...
+00011c20: 0000 0600 0000 224f 7065 6e20 6272 6f6b  ......"Open brok
+00011c30: 6572 2072 6570 6f72 7420 7469 746c 6520  er report title 
+00011c40: 6e6f 7420 666f 756e 6407 0000 0013 5374  not found.....St
+00011c50: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+00011c60: 7201 0300 0000 3804 1e04 3f04 3504 4004  r.....8...?.5.@.
+00011c70: 3004 4604 3804 4f00 2004 3d04 3500 2004  0.F.8.O. .=.5. .
+00011c80: 3f04 3e04 3404 3404 3504 4004 3604 3804  ?.>.4.4.5.@.6.8.
+00011c90: 3204 3004 3504 4204 4104 4f00 3a00 2008  2.0.5.B.A.O.:. .
+00011ca0: 0000 0000 0600 0000 194f 7065 7261 7469  .........Operati
+00011cb0: 6f6e 206e 6f74 2073 7570 706f 7274 6564  on not supported
+00011cc0: 3a20 0700 0000 1353 7461 7465 6d65 6e74  : .....Statement
+00011cd0: 4f70 656e 4272 6f6b 6572 0103 0000 001c  OpenBroker......
+00011ce0: 0426 0411 0020 0437 0430 0433 0440 0443  .&... .7.0.3.@.C
+00011cf0: 0436 0435 043d 044b 003a 0020 0800 0000  .6.5.=.K.:. ....
+00011d00: 0006 0000 0013 5365 6375 7269 7469 6573  ......Securities
+00011d10: 206c 6f61 6465 643a 2007 0000 0013 5374   loaded: .....St
+00011d20: 6174 656d 656e 744f 7065 6e42 726f 6b65  atementOpenBroke
+00011d30: 7201 0300 0000 6e04 1d04 3504 3f04 3e04  r.....n...5.?.>.
+00011d40: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00011d50: 3504 3c04 4b04 3900 2004 3704 3004 3304  5.<.K.9. .7.0.3.
+00011d60: 3e04 3b04 3e04 3204 3e04 3a00 2004 3e04  >.;.>.2.>.:. .>.
+00011d70: 4204 4704 5104 4204 3000 2004 3404 3b04  B.G.Q.B.0. .4.;.
+00011d80: 4f00 2004 1e04 4204 3a04 4004 4b04 4204  O. ...B.:.@.K.B.
+00011d90: 3804 3500 2004 3104 4004 3e04 3a04 3504  8.5. .1.@.>.:.5.
+00011da0: 4000 3a00 2008 0000 0000 0600 0000 2655  @.:. .........&U
+00011db0: 6e65 7870 6563 7465 6420 4f70 656e 2062  nexpected Open b
+00011dc0: 726f 6b65 7220 7265 706f 7274 2068 6561  roker report hea
+00011dd0: 6465 723a 2007 0000 0013 5374 6174 656d  der: .....Statem
+00011de0: 656e 744f 7065 6e42 726f 6b65 7201 0300  entOpenBroker...
+00011df0: 0000 4204 1d04 3504 3804 3704 3204 3504  ..B...5.8.7.2.5.
+00011e00: 4104 4204 3d04 3004 4f00 2004 3d04 3504  A.B.=.0.O. .=.5.
+00011e10: 4204 3e04 4004 3304 3e04 3204 3004 4f00  B.>.@.3.>.2.0.O.
+00011e20: 2004 3e04 3f04 3504 4004 3004 4604 3804   .>.?.5.@.0.F.8.
+00011e30: 4f00 3a00 2008 0000 0000 0600 0000 1d55  O.:. ..........U
+00011e40: 6e6b 6e6f 776e 206e 6f6e 2d74 7261 6465  nknown non-trade
+00011e50: 206f 7065 7261 7469 6f6e 3a20 0700 0000   operation: ....
+00011e60: 1353 7461 7465 6d65 6e74 4f70 656e 4272  .StatementOpenBr
+00011e70: 6f6b 6572 0103 0000 0046 041d 0435 043f  oker.....F...5.?
+00011e80: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
+00011e90: 0430 0435 043c 043e 0435 0020 043e 043f  .0.5.<.>.5. .>.?
+00011ea0: 0438 0441 0430 043d 0438 0435 0020 043f  .8.A.0.=.8.5. .?
+00011eb0: 043b 0430 0442 0435 0436 0430 003a 0020  .;.0.B.5.6.0.:. 
+00011ec0: 0800 0000 0006 0000 001d 556e 6b6e 6f77  ..........Unknow
+00011ed0: 6e20 7061 796d 656e 7420 6465 7363 7269  n payment descri
+00011ee0: 7074 696f 6e3a 2007 0000 0013 5374 6174  ption: .....Stat
+00011ef0: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
+00011f00: 0300 0000 3204 1d04 3504 3804 3704 3204  ....2...5.8.7.2.
+00011f10: 3504 4104 4204 3d04 4b04 3900 2004 4204  5.A.B.=.K.9. .B.
+00011f20: 3804 3f00 2004 3f04 3b04 3004 4204 3504  8.?. .?.;.0.B.5.
+00011f30: 3604 3000 3a00 2008 0000 0000 0600 0000  6.0.:. .........
+00011f40: 1655 6e6b 6e6f 776e 2070 6179 6d65 6e74  .Unknown payment
+00011f50: 2074 7970 653a 2007 0000 0013 5374 6174   type: .....Stat
+00011f60: 656d 656e 744f 7065 6e42 726f 6b65 7201  ementOpenBroker.
+00011f70: 0300 0000 1604 2604 1100 2004 3104 3504  ......&... .1.5.
+00011f80: 3700 2000 6900 6400 3a00 2008 0000 0000  7. .i.d.:. .....
+00011f90: 0600 0000 1241 7373 6574 2077 6974 686f  .....Asset witho
+00011fa0: 7574 2069 643a 2007 0000 0016 5374 6174  ut id: .....Stat
+00011fb0: 656d 656e 744f 7065 6e50 6f72 7466 6f6c  ementOpenPortfol
+00011fc0: 696f 0103 0000 0048 041d 0435 0432 043e  io.....H...5.2.>
+00011fd0: 0437 043c 043e 0436 043d 043e 0020 043f  .7.<.>.6.=.>. .?
+00011fe0: 0440 043e 0447 0438 0442 0430 0442 044c  .@.>.G.8.B.0.B.L
+00011ff0: 0020 004a 0053 004f 004e 0020 0438 0437  . .J.S.O.N. .8.7
+00012000: 0020 0444 0430 0439 043b 0430 003a 0020  . .D.0.9.;.0.:. 
+00012010: 0800 0000 0006 0000 001f 4661 696c 6564  ..........Failed
+00012020: 2074 6f20 7265 6164 204a 534f 4e20 6672   to read JSON fr
+00012030: 6f6d 2066 696c 653a 2007 0000 0016 5374  om file: .....St
+00012040: 6174 656d 656e 744f 7065 6e50 6f72 7466  atementOpenPortf
+00012050: 6f6c 696f 0103 0000 0034 041d 0435 0432  olio.....4...5.2
+00012060: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+00012070: 043f 0440 043e 0447 0435 0441 0442 044c  .?.@.>.G.5.A.B.L
+00012080: 0020 0444 0430 0439 043b 003a 0020 0800  . .D.0.9.;.:. ..
+00012090: 0000 0006 0000 0015 4661 696c 6564 2074  ........Failed t
+000120a0: 6f20 7265 6164 2066 696c 653a 2007 0000  o read file: ...
+000120b0: 0016 5374 6174 656d 656e 744f 7065 6e50  ..StatementOpenP
+000120c0: 6f72 7466 6f6c 696f 0103 0000 0022 0418  ortfolio....."..
+000120d0: 043c 043f 043e 0440 0442 0438 0440 043e  .<.?.>.@.B.8.@.>
+000120e0: 0432 0430 043d 043d 044b 0439 0020 2116  .2.0.=.=.K.9. !.
+000120f0: 0800 0000 0006 0000 000a 496d 706f 7274  ..........Import
+00012100: 6564 2023 0700 0000 1653 7461 7465 6d65  ed #.....Stateme
+00012110: 6e74 4f70 656e 506f 7274 666f 6c69 6f01  ntOpenPortfolio.
+00012120: 0300 0000 2e00 4900 6e00 7600 6500 7300  ......I.n.v.e.s.
+00012130: 7400 6200 6f00 6f00 6b00 2000 2f00 2000  t.b.o.o.k. ./. .
+00012140: 4900 5a00 4900 2d00 6900 6e00 7600 6500  I.Z.I.-.i.n.v.e.
+00012150: 7300 7408 0000 0000 0600 0000 1749 6e76  s.t..........Inv
+00012160: 6573 7462 6f6f 6b20 2f20 495a 492d 496e  estbook / IZI-In
+00012170: 7665 7374 0700 0000 1653 7461 7465 6d65  vest.....Stateme
+00012180: 6e74 4f70 656e 506f 7274 666f 6c69 6f01  ntOpenPortfolio.
+00012190: 0300 0000 4204 1e04 3104 4f04 3704 3004  ....B...1.O.7.0.
+000121a0: 4204 3504 3b04 4c04 3d04 3004 4f00 2004  B.5.;.L.=.0.O. .
+000121b0: 4104 3504 3a04 4604 3804 4f00 2004 3e04  A.5.:.F.8.O. .>.
+000121c0: 4204 4104 4304 4204 4104 4204 3204 4304  B.A.C.B.A.B.2.C.
+000121d0: 3504 4200 3a00 2008 0000 0000 0600 0000  5.B.:. .........
+000121e0: 1e4d 616e 6461 746f 7279 2073 6563 7469  .Mandatory secti
+000121f0: 6f6e 2069 7320 6d69 7373 696e 673a 2007  on is missing: .
+00012200: 0000 0016 5374 6174 656d 656e 744f 7065  ....StatementOpe
+00012210: 6e50 6f72 7466 6f6c 696f 0103 0000 002e  nPortfolio......
+00012220: 004f 0070 0065 006e 0020 0070 006f 0072  .O.p.e.n. .p.o.r
+00012230: 0074 0066 006f 006c 0069 006f 0020 0028  .t.f.o.l.i.o. .(
+00012240: 002a 002e 006a 0073 006f 006e 0029 0800  .*...j.s.o.n.)..
+00012250: 0000 0006 0000 0017 4f70 656e 2070 6f72  ........Open por
+00012260: 7466 6f6c 696f 2028 2a2e 6a73 6f6e 2907  tfolio (*.json).
+00012270: 0000 0016 5374 6174 656d 656e 744f 7065  ....StatementOpe
+00012280: 6e50 6f72 7466 6f6c 696f 0103 0000 004e  nPortfolio.....N
+00012290: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+000122a0: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
+000122b0: 0020 0432 0435 0440 0441 0438 044f 0020  . .2.5.@.A.8.O. 
+000122c0: 0444 043e 0440 043c 0430 0442 0430 0020  .D.>.@.<.0.B.0. 
+000122d0: 0444 0430 0439 043b 0430 003a 0020 0800  .D.0.9.;.0.:. ..
+000122e0: 0000 0006 0000 002e 556e 7375 7070 6f72  ........Unsuppor
+000122f0: 7465 6420 7665 7273 696f 6e20 6f66 206f  ted version of o
+00012300: 7065 6e20 706f 7274 666f 6c69 6f20 666f  pen portfolio fo
+00012310: 726d 6174 3a20 0700 0000 1653 7461 7465  rmat: .....State
+00012320: 6d65 6e74 4f70 656e 506f 7274 666f 6c69  mentOpenPortfoli
+00012330: 6f01 0300 0000 3804 1a04 4304 3f04 3e04  o.....8...C.?.>.
+00012340: 3d04 4b00 2004 3e04 3104 3b04 3804 3304  =.K. .>.1.;.8.3.
+00012350: 3004 4604 3804 3900 2004 3704 3004 3304  0.F.8.9. .7.0.3.
+00012360: 4004 4304 3604 3504 3d04 4b00 3a00 2008  @.C.6.5.=.K.:. .
+00012370: 0000 0000 0600 0000 1742 6f6e 6420 696e  .........Bond in
+00012380: 7465 7265 7374 7320 6c6f 6164 6564 3a20  terests loaded: 
+00012390: 0700 0000 0c53 7461 7465 6d65 6e74 5053  .....StatementPS
+000123a0: 4201 0300 0000 3e04 1404 3504 3d04 3504  B.....>...5.=.5.
+000123b0: 3604 3d04 4b04 3500 2004 4204 4004 3004  6.=.K.5. .B.@.0.
+000123c0: 3d04 3704 3004 3a04 4604 3804 3800 2004  =.7.0.:.F.8.8. .
+000123d0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+000123e0: 4b00 3a00 2008 0000 0000 0600 0000 1a43  K.:. ..........C
+000123f0: 6173 6820 7472 616e 7361 6374 696f 6e73  ash transactions
+00012400: 206c 6f61 6465 643a 2007 0000 000c 5374   loaded: .....St
+00012410: 6174 656d 656e 7450 5342 0103 0000 002a  atementPSB.....*
+00012420: 0414 0438 0432 0438 0434 0435 043d 0434  ...8.2.8.4.5.=.4
+00012430: 044b 0020 0437 0430 0433 0440 0443 0436  .K. .7.0.3.@.C.6
+00012440: 0435 043d 044b 003a 0020 0800 0000 0006  .5.=.K.:. ......
+00012450: 0000 0012 4469 7669 6465 6e64 7320 6c6f  ....Dividends lo
+00012460: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
+00012470: 6d65 6e74 5053 4201 0300 0000 1404 1f04  mentPSB.........
+00012480: 2104 1100 2d04 3104 4004 3e04 3a04 3504  !...-.1.@.>.:.5.
+00012490: 4008 0000 0000 0600 0000 0a50 5342 2042  @..........PSB B
+000124a0: 726f 6b65 7207 0000 000c 5374 6174 656d  roker.....Statem
+000124b0: 656e 7450 5342 0103 0000 0040 041e 0442  entPSB.....@...B
+000124c0: 0447 0451 0442 0020 0431 0440 043e 043a  .G.Q.B. .1.@.>.:
+000124d0: 0435 0440 0430 0020 041f 0421 0411 0020  .5.@.0. ...!... 
+000124e0: 0028 002a 002e 0078 006c 0073 0078 0020  .(.*...x.l.s.x. 
+000124f0: 002a 002e 0078 006c 0073 0029 0800 0000  .*...x.l.s.)....
+00012500: 0006 0000 0023 5053 4220 6272 6f6b 6572  .....#PSB broker
+00012510: 2073 7461 7465 6d65 6e74 2028 2a2e 786c   statement (*.xl
+00012520: 7378 202a 2e78 6c73 2907 0000 000c 5374  sx *.xls).....St
+00012530: 6174 656d 656e 7450 5342 0103 ffff ffff  atementPSB......
+00012540: 0800 0000 0006 0000 000f 5472 6164 6573  ..........Trades
+00012550: 206c 6f61 6465 643a 2007 0000 000c 5374   loaded: .....St
+00012560: 6174 656d 656e 7450 5342 0103 0000 0040  atementPSB.....@
+00012570: 041d 0435 043f 043e 0434 0434 0435 0440  ...5.?.>.4.4.5.@
+00012580: 0436 0438 0432 0430 0435 043c 0430 044f  .6.8.2.0.5.<.0.O
+00012590: 0020 043e 043f 0435 0440 0430 0446 0438  . .>.?.5.@.0.F.8
+000125a0: 044f 0020 0441 0020 0414 0421 003a 0020  .O. .A. ...!.:. 
+000125b0: 0800 0000 0006 0000 0018 556e 6b6e 6f77  ..........Unknow
+000125c0: 6e20 6361 7368 206f 7065 7261 7469 6f6e  n cash operation
+000125d0: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+000125e0: 5053 4201 0300 0000 3a04 1d04 3504 3804  PSB.....:...5.8.
+000125f0: 3704 3204 3504 4104 4204 3d04 4b04 3900  7.2.5.A.B.=.K.9.
+00012600: 2004 4204 3804 3f00 2004 3404 3204 3804   .B.8.?. .4.2.8.
+00012610: 3604 3504 3d04 3804 4f00 2004 1404 2100  6.5.=.8.O. ...!.
+00012620: 3a00 2008 0000 0000 0600 0000 1a55 6e6b  :. ..........Unk
+00012630: 6e6f 776e 2063 6173 6820 7472 616e 7361  nown cash transa
+00012640: 6374 696f 6e3a 2007 0000 000c 5374 6174  ction: .....Stat
+00012650: 656d 656e 7450 5342 0103 0000 0030 041d  ementPSB.....0..
+00012660: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
+00012670: 044b 0439 0020 0442 0438 043f 0020 0441  .K.9. .B.8.?. .A
+00012680: 0434 0435 043b 043a 0438 003a 0020 0800  .4.5.;.:.8.:. ..
+00012690: 0000 0006 0000 0014 556e 6b6e 6f77 6e20  ........Unknown 
+000126a0: 7472 6164 6520 7479 7065 3a20 0700 0000  trade type: ....
+000126b0: 0c53 7461 7465 6d65 6e74 5053 4201 0300  .StatementPSB...
+000126c0: 0000 3204 1d04 3504 3f04 3e04 3404 3404  ..2...5.?.>.4.4.
+000126d0: 3504 4004 3604 3804 3204 3004 3504 3c04  5.@.6.8.2.0.5.<.
+000126e0: 4b04 3900 2004 3f04 3b04 3004 4204 5104  K.9. .?.;.0.B.Q.
+000126f0: 3600 3a00 2008 0000 0000 0600 0000 1555  6.:. ..........U
+00012700: 6e73 7570 706f 7274 6564 2070 6179 6d65  nsupported payme
+00012710: 6e74 3a20 0700 0000 0c53 7461 7465 6d65  nt: .....Stateme
+00012720: 6e74 5053 4201 0300 0000 5a04 2104 3404  ntPSB.....Z.!.4.
+00012730: 3504 3b04 3a04 3000 2004 4100 2004 4004  5.;.:.0. .A. .@.
+00012740: 3004 3704 3d04 4b04 3c04 3800 2004 3204  0.7.=.K.<.8. .2.
+00012750: 3004 3b04 4e04 4204 3004 3c04 3800 2004  0.;.N.B.0.<.8. .
+00012760: 3d04 3500 2004 3f04 3e04 3404 3404 3504  =.5. .?.>.4.4.5.
+00012770: 4004 3604 3804 3204 3004 3504 4204 4104  @.6.8.2.0.5.B.A.
+00012780: 4f00 3a00 2008 0000 0000 0600 0000 2d55  O.:. .........-U
+00012790: 6e73 7570 706f 7274 6564 2074 7261 6465  nsupported trade
+000127a0: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
+000127b0: 6375 7272 656e 6369 6573 3a20 0700 0000  currencies: ....
+000127c0: 0c53 7461 7465 6d65 6e74 5053 4201 0300  .StatementPSB...
+000127d0: 0000 3204 1e04 3f04 3504 4004 3004 4604  ..2...?.5.@.0.F.
+000127e0: 3804 3800 2004 4100 2004 2604 1100 2004  8.8. .A. .&... .
+000127f0: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+00012800: 4b00 3a00 2008 0000 0000 0600 0000 1941  K.:. ..........A
+00012810: 7373 6574 206f 7065 7261 7469 6f6e 7320  sset operations 
+00012820: 6c6f 6164 6564 3a20 0700 0000 0d53 7461  loaded: .....Sta
+00012830: 7465 6d65 6e74 554b 4655 0103 0000 0068  tementUKFU.....h
+00012840: 041e 0442 0441 0443 0442 0441 0442 0432  ...B.A.C.B.A.B.2
+00012850: 0443 044e 0442 0020 043e 0436 0438 0434  .C.N.B. .>.6.8.4
+00012860: 0430 0435 043c 044b 0435 0020 0434 0430  .0.5.<.K.5. .4.0
+00012870: 043d 043d 044b 0435 0020 0432 0020 043e  .=.=.K.5. .2. .>
+00012880: 043f 0438 0441 0430 043d 0438 0438 0020  .?.8.A.0.=.8.8. 
+00012890: 043f 0435 0440 0435 0432 043e 0434 0430  .?.5.@.5.2.>.4.0
+000128a0: 0020 0426 0411 0020 0800 0000 0006 0000  . .&... ........
+000128b0: 002a 4173 7365 7420 7472 616e 7366 6572  .*Asset transfer
+000128c0: 2064 6573 6372 6970 7469 6f6e 206d 6973   description mis
+000128d0: 7320 736f 6d65 2064 6174 6120 0700 0000  s some data ....
+000128e0: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
+000128f0: 0000 0050 041d 0435 0432 043e 0437 043c  ...P...5.2.>.7.<
+00012900: 043e 0436 043d 043e 0020 043d 0430 0439  .>.6.=.>. .=.0.9
+00012910: 0442 0438 0020 0437 0430 043f 0438 0441  .B.8. .7.0.?.8.A
+00012920: 044c 0020 0441 043f 0438 0441 0430 043d  .L. .A.?.8.A.0.=
+00012930: 0438 044f 0020 0426 0411 0020 0434 043b  .8.O. .&... .4.;
+00012940: 044f 0020 0800 0000 0006 0000 0029 4361  .O. .........)Ca
+00012950: 6e27 7420 6669 6e64 2061 7373 6574 2063  n't find asset c
+00012960: 616e 6365 6c6c 6174 696f 6e20 7265 636f  ancellation reco
+00012970: 7264 2066 6f72 2007 0000 000d 5374 6174  rd for .....Stat
+00012980: 656d 656e 7455 4b46 5501 0300 0000 4604  ementUKFU.....F.
+00012990: 1d04 3504 3204 3e04 3704 3c04 3e04 3604  ..5.2.>.7.<.>.6.
+000129a0: 3d04 3e00 2004 3d04 3004 3904 4204 3800  =.>. .=.0.9.B.8.
+000129b0: 2004 3704 3004 3304 3e04 3b04 3e04 3204   .7.0.3.>.;.>.2.
+000129c0: 3e04 3a00 2004 3a04 3e04 3c04 3804 4104  >.:. .:.>.<.8.A.
+000129d0: 4104 3804 3908 0000 0000 0600 0000 1d43  A.8.9..........C
+000129e0: 616e 2774 2067 6574 2068 6561 6465 7220  an't get header 
+000129f0: 746f 2066 696e 6420 6665 6573 0700 0000  to find fees....
+00012a00: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
+00012a10: 0000 0056 041d 0435 0432 043e 0437 043c  ...V...5.2.>.7.<
+00012a20: 043e 0436 043d 043e 0020 0440 0430 0441  .>.6.=.>. .@.0.A
+00012a30: 043f 043e 0437 043d 0430 0442 044c 0020  .?.>.7.=.0.B.L. 
+00012a40: 043e 043f 0438 0441 0430 043d 0438 0435  .>.?.8.A.0.=.8.5
+00012a50: 0020 043f 0435 0440 0435 0432 043e 0434  . .?.5.@.5.2.>.4
+00012a60: 0430 0020 0426 0411 0020 0800 0000 0006  .0. .&... ......
+00012a70: 0000 0027 4361 6e27 7420 7061 7273 6520  ...'Can't parse 
+00012a80: 6173 7365 7420 7472 616e 7366 6572 2064  asset transfer d
+00012a90: 6573 6372 6970 7469 6f6e 2007 0000 000d  escription .....
+00012aa0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
+00012ab0: 0000 4c04 1d04 3504 3204 3e04 3704 3c04  ..L...5.2.>.7.<.
+00012ac0: 3e04 3604 3d04 3e00 2004 4004 3004 4104  >.6.=.>. .@.0.A.
+00012ad0: 3f04 3e04 3704 3d04 3004 4204 4c00 2004  ?.>.7.=.0.B.L. .
+00012ae0: 3e04 3f04 3804 4104 3004 3d04 3804 3500  >.?.8.A.0.=.8.5.
+00012af0: 2004 3a04 4304 3f04 3e04 3d04 3000 2008   .:.C.?.>.=.0. .
+00012b00: 0000 0000 0600 0000 2643 616e 2774 2070  ........&Can't p
+00012b10: 6172 7365 2062 6f6e 6420 696e 7465 7265  arse bond intere
+00012b20: 7374 2064 6573 6372 6970 7469 6f6e 2007  st description .
+00012b30: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
+00012b40: 5501 0300 0000 6604 1d04 3504 3204 3e04  U.....f...5.2.>.
+00012b50: 3704 3c04 3e04 3604 3d04 3e00 2004 4004  7.<.>.6.=.>. .@.
+00012b60: 3004 4104 3f04 3e04 3704 3d04 3004 4204  0.A.?.>.7.=.0.B.
+00012b70: 4c00 2004 3e04 3f04 3804 4104 3004 3d04  L. .>.?.8.A.0.=.
+00012b80: 3804 3500 2004 3f04 3e04 3304 3004 4804  8.5. .?.>.3.0.H.
+00012b90: 3504 3d04 3804 4f00 2004 3e04 3104 3b04  5.=.8.O. .>.1.;.
+00012ba0: 3804 3304 3004 4604 3804 3800 2008 0000  8.3.0.F.8.8. ...
+00012bb0: 0000 0600 0000 2743 616e 2774 2070 6172  ......'Can't par
+00012bc0: 7365 2062 6f6e 6420 7265 7061 796d 656e  se bond repaymen
+00012bd0: 7420 6465 7363 7269 7074 696f 6e20 0700  t description ..
+00012be0: 0000 0d53 7461 7465 6d65 6e74 554b 4655  ...StatementUKFU
+00012bf0: 0103 0000 0052 041d 0435 0432 043e 0437  .....R...5.2.>.7
+00012c00: 043c 043e 0436 043d 043e 0020 0440 0430  .<.>.6.=.>. .@.0
+00012c10: 0441 043f 043e 0437 043d 0430 0442 044c  .A.?.>.7.=.0.B.L
+00012c20: 0020 043e 043f 0438 0441 0430 043d 0438  . .>.?.8.A.0.=.8
+00012c30: 0435 0020 0434 0438 0432 0438 0434 0435  .5. .4.8.2.8.4.5
+00012c40: 043d 0434 0430 0020 0800 0000 0006 0000  .=.4.0. ........
+00012c50: 0021 4361 6e27 7420 7061 7273 6520 6469  .!Can't parse di
+00012c60: 7669 6465 6e64 2064 6573 6372 6970 7469  vidend descripti
+00012c70: 6f6e 2007 0000 000d 5374 6174 656d 656e  on .....Statemen
+00012c80: 7455 4b46 5501 0300 0000 6404 1d04 3504  tUKFU.....d...5.
+00012c90: 3204 3e04 3704 3c04 3e04 3604 3d04 3e00  2.>.7.<.>.6.=.>.
+00012ca0: 2004 4004 3004 4104 3f04 3e04 3704 3d04   .@.0.A.?.>.7.=.
+00012cb0: 3004 4204 4c00 2004 3e04 3f04 3804 4104  0.B.L. .>.?.8.A.
+00012cc0: 3004 3d04 3804 3500 2004 3404 3504 3d04  0.=.8.5. .4.5.=.
+00012cd0: 3504 3604 3d04 3e04 3304 3e00 2004 3f04  5.6.=.>.3.>. .?.
+00012ce0: 3504 4004 3504 3204 3e04 3404 3000 2008  5.@.5.2.>.4.0. .
+00012cf0: 0000 0000 0600 0000 2743 616e 2774 2070  ........'Can't p
+00012d00: 6172 7365 206d 6f6e 6579 2074 7261 6e73  arse money trans
+00012d10: 6665 7220 6465 7363 7269 7074 696f 6e20  fer description 
+00012d20: 0700 0000 0d53 7461 7465 6d65 6e74 554b  .....StatementUK
+00012d30: 4655 0103 0000 003a 0414 0435 043d 0435  FU.....:...5.=.5
+00012d40: 0436 043d 044b 0445 0020 043e 043f 0435  .6.=.K.E. .>.?.5
+00012d50: 0440 0430 0446 0438 0439 0020 0437 0430  .@.0.F.8.9. .7.0
+00012d60: 0433 0440 0443 0436 0435 043d 043e 003a  .3.@.C.6.5.=.>.:
+00012d70: 0020 0800 0000 0006 0000 0018 4361 7368  . ..........Cash
+00012d80: 206f 7065 7261 7469 6f6e 7320 6c6f 6164   operations load
+00012d90: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
+00012da0: 6e74 554b 4655 0103 0000 0048 041e 0448  ntUKFU.....H...H
+00012db0: 0438 0431 043a 0430 0020 043f 0440 0438  .8.1.:.0. .?.@.8
+00012dc0: 0020 043a 043e 043d 0432 0435 0440 0442  . .:.>.=.2.5.@.B
+00012dd0: 0430 0446 0438 0438 0020 0441 0443 043c  .0.F.8.8. .A.C.<
+00012de0: 043c 044b 0020 043d 0430 043b 043e 0433  .<.K. .=.0.;.>.3
+00012df0: 0430 0020 0800 0000 0006 0000 001f 4661  .0. ..........Fa
+00012e00: 696c 6564 2074 6f20 636f 6e76 6572 7420  iled to convert 
+00012e10: 6469 7669 6465 6e64 2074 6178 2007 0000  dividend tax ...
+00012e20: 000d 5374 6174 656d 656e 7455 4b46 5501  ..StatementUKFU.
+00012e30: 0300 0000 3e04 2104 3404 3504 3b04 3e04  ....>.!.4.5.;.>.
+00012e40: 3a00 2004 4100 2004 4404 4c04 4e04 4704  :. .A. .D.L.N.G.
+00012e50: 3504 4004 4104 3004 3c04 3800 2004 3704  5.@.A.0.<.8. .7.
+00012e60: 3004 3304 4004 4304 3604 3504 3d04 3e00  0.3.@.C.6.5.=.>.
+00012e70: 3a00 2008 0000 0000 0600 0000 1746 7574  :. ..........Fut
+00012e80: 7572 6573 2074 7261 6465 7320 6c6f 6164  ures trades load
+00012e90: 6564 3a20 0700 0000 0d53 7461 7465 6d65  ed: .....Stateme
+00012ea0: 6e74 554b 4655 0103 0000 0076 041e 0442  ntUKFU.....v...B
+00012eb0: 0441 0443 0442 0441 0442 0432 0443 044e  .A.C.B.A.B.2.C.N
+00012ec0: 0442 0020 043e 0436 0438 0434 0430 0435  .B. .>.6.8.4.0.5
+00012ed0: 043c 044b 0435 0020 0434 0430 043d 043d  .<.K.5. .4.0.=.=
+00012ee0: 044b 0435 0020 0432 0020 043e 043f 0438  .K.5. .2. .>.?.8
+00012ef0: 0441 0430 043d 0438 0438 0020 0434 0435  .A.0.=.8.8. .4.5
+00012f00: 043d 0435 0436 043d 043e 0433 043e 0020  .=.5.6.=.>.3.>. 
+00012f10: 043f 0435 0440 0435 0432 043e 0434 0430  .?.5.@.5.2.>.4.0
+00012f20: 0020 0800 0000 0006 0000 002a 4d6f 6e65  . .........*Mone
+00012f30: 7920 7472 616e 7366 6572 2064 6573 6372  y transfer descr
+00012f40: 6970 7469 6f6e 206d 6973 7320 736f 6d65  iption miss some
+00012f50: 2064 6174 6120 0700 0000 0d53 7461 7465   data .....State
+00012f60: 6d65 6e74 554b 4655 0103 0000 0056 041d  mentUKFU.....V..
+00012f70: 0430 0439 0434 0435 043d 044b 0020 043d  .0.9.4.5.=.K. .=
+00012f80: 0435 0441 043a 043e 043b 044c 043a 043e  .5.A.:.>.;.L.:.>
+00012f90: 0020 0437 0430 043f 0438 0441 0435 0439  . .7.0.?.8.A.5.9
+00012fa0: 0020 043f 043e 0433 0430 0448 0435 043d  . .?.>.3.0.H.5.=
+00012fb0: 0438 044f 0020 0426 0411 0020 0434 043b  .8.O. .&... .4.;
+00012fc0: 044f 0020 0800 0000 0006 0000 0026 4d75  .O. .........&Mu
+00012fd0: 6c74 6970 6c65 2061 7373 6574 2063 616e  ltiple asset can
+00012fe0: 6365 6c6c 6174 696f 6e20 6d61 7463 6820  cellation match 
+00012ff0: 666f 7220 0700 0000 0d53 7461 7465 6d65  for .....Stateme
+00013000: 6e74 554b 4655 0103 0000 0024 0421 0434  ntUKFU.....$.!.4
+00013010: 0435 043b 043e 043a 0020 0437 0430 0433  .5.;.>.:. .7.0.3
+00013020: 0440 0443 0436 0435 043d 043e 003a 0020  .@.C.6.5.=.>.:. 
+00013030: 0800 0000 0006 0000 000f 5472 6164 6573  ..........Trades
+00013040: 206c 6f61 6465 643a 2007 0000 000d 5374   loaded: .....St
+00013050: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
+00013060: 4004 2204 3204 3e04 3900 2004 3104 4004  @.".2.>.9. .1.@.
+00013070: 3e04 3a04 3504 4000 2000 2800 6500 7800  >.:.5.@. .(.e.x.
+00013080: 2e00 2004 3104 4004 3e04 3a04 3504 4000  .. .1.@.>.:.5.@.
+00013090: 2004 2304 4004 3004 3b04 4104 3804 3100   .#.@.0.;.A.8.1.
+000130a0: 2908 0000 0000 0600 0000 2054 766f 7920  )......... Tvoy 
+000130b0: 4272 6f6b 6572 2028 6578 2e20 5572 616c  Broker (ex. Ural
+000130c0: 7369 6220 4272 6f6b 6572 2907 0000 000d  sib Broker).....
+000130d0: 5374 6174 656d 656e 7455 4b46 5501 0300  StatementUKFU...
+000130e0: 0000 3204 1e04 4204 4704 5104 4200 2004  ..2...B.G.Q.B. .
+000130f0: 2204 3204 3e04 3900 2004 3104 4004 3e04  ".2.>.9. .1.@.>.
+00013100: 3a04 3504 4000 2000 2800 2a00 2e00 7a00  :.5.@. .(.*...z.
+00013110: 6900 7000 2908 0000 0000 0600 0000 1d54  i.p.)..........T
+00013120: 766f 7920 4272 6f6b 6572 2073 7461 7465  voy Broker state
+00013130: 6d65 6e74 2028 2a2e 7a69 7029 0700 0000  ment (*.zip)....
+00013140: 0d53 7461 7465 6d65 6e74 554b 4655 0103  .StatementUKFU..
+00013150: 0000 0030 041d 0435 0438 0437 0432 0435  ...0...5.8.7.2.5
+00013160: 0441 0442 043d 044b 0439 0020 0442 0438  .A.B.=.K.9. .B.8
+00013170: 043f 0020 0441 0434 0435 043b 043a 0438  .?. .A.4.5.;.:.8
+00013180: 003a 0020 0800 0000 0006 0000 0014 556e  .:. ..........Un
+00013190: 6b6e 6f77 6e20 7472 6164 6520 7479 7065  known trade type
+000131a0: 3a20 0700 0000 0d53 7461 7465 6d65 6e74  : .....Statement
+000131b0: 554b 4655 0103 0000 003e 041d 0435 043f  UKFU.....>...5.?
+000131c0: 043e 0434 0434 0435 0440 0436 0438 0432  .>.4.4.5.@.6.8.2
+000131d0: 0430 0435 043c 0430 044f 0020 043e 043f  .0.5.<.0.O. .>.?
+000131e0: 0435 0440 0430 0446 0438 044f 0020 0441  .5.@.0.F.8.O. .A
+000131f0: 0020 0426 0411 0020 0800 0000 0006 0000  . .&... ........
+00013200: 001d 556e 7375 7070 706f 7274 6564 2061  ..Unsuppported a
+00013210: 7373 6574 206f 7065 7261 7469 6f6e 2007  sset operation .
+00013220: 0000 000d 5374 6174 656d 656e 7455 4b46  ....StatementUKF
+00013230: 5501 0300 0000 4a04 1d04 3504 3f04 3e04  U.....J...5.?.>.
+00013240: 3404 3404 3504 4004 3604 3804 3204 3004  4.4.5.@.6.8.2.0.
+00013250: 3504 3c04 3004 4f00 2004 3404 3504 3d04  5.<.0.O. .4.5.=.
+00013260: 3504 3604 3d04 3004 4f00 2004 4204 4004  5.6.=.0.O. .B.@.
+00013270: 3004 3d04 3704 3004 3a04 4604 3804 4f00  0.=.7.0.:.F.8.O.
+00013280: 2008 0000 0000 0600 0000 1e55 6e73 7570   ..........Unsup
+00013290: 7070 6f72 7465 6420 6361 7368 2074 7261  pported cash tra
+000132a0: 6e73 6163 7469 6f6e 2007 0000 000d 5374  nsaction .....St
+000132b0: 6174 656d 656e 7455 4b46 5501 0300 0000  atementUKFU.....
+000132c0: 3e04 1004 4004 4504 3804 3200 2004 4104  >...@.E.8.2. .A.
+000132d0: 3e04 3404 3504 4004 3604 3804 4200 2004  >.4.5.@.6.8.B. .
+000132e0: 3d04 3504 4104 3a04 3e04 3b04 4c04 3a04  =.5.A.:.>.;.L.:.
+000132f0: 3e00 2004 4404 3004 3904 3b04 3e04 3208  >. .D.0.9.;.>.2.
+00013300: 0000 0000 0600 0000 1f41 7263 6869 7665  .........Archive
+00013310: 2063 6f6e 7461 696e 7320 6d75 6c74 6970   contains multip
+00013320: 6c65 2066 696c 6573 0700 0000 0c53 7461  le files.....Sta
+00013330: 7465 6d65 6e74 584c 5301 0300 0000 5a04  tementXLS.....Z.
+00013340: 1d04 3500 2004 4304 3404 3004 3b04 3e04  ..5. .C.4.0.;.>.
+00013350: 4104 4c00 2004 3d04 3004 3904 4204 3800  A.L. .=.0.9.B.8.
+00013360: 2004 3e04 3604 3804 3404 3004 3504 3c04   .>.6.8.4.0.5.<.
+00013370: 4b04 3900 2004 3704 3004 3304 3e04 3b04  K.9. .7.0.3.>.;.
+00013380: 3e04 3204 3e04 3a00 2004 3e04 4204 4704  >.2.>.:. .>.B.G.
+00013390: 5104 4204 3000 3a00 2008 0000 0000 0600  Q.B.0.:. .......
+000133a0: 0000 2343 616e 2774 2066 696e 6420 6578  ..#Can't find ex
+000133b0: 7065 6374 6564 2072 6570 6f72 7420 6865  pected report he
+000133c0: 6164 6572 3a20 0700 0000 0c53 7461 7465  ader: .....State
+000133d0: 6d65 6e74 584c 5301 0300 0000 6604 1d04  mentXLS.....f...
+000133e0: 3500 2004 4304 3404 3004 3b04 3e04 4104  5. .C.4.0.;.>.A.
+000133f0: 4c00 2004 3e04 3f04 4004 3504 3404 3504  L. .>.?.@.5.4.5.
+00013400: 3b04 3804 4204 4c00 2004 3204 3004 3b04  ;.8.B.L. .2.0.;.
+00013410: 4e04 4204 4b00 2004 3804 3700 2004 3e04  N.B.K. .8.7. .>.
+00013420: 3104 4904 3504 3900 2004 4104 3504 3a04  1.I.5.9. .A.5.:.
+00013430: 4604 3804 3800 2004 3e04 4204 4704 5104  F.8.8. .>.B.G.Q.
+00013440: 4204 3008 0000 0000 0600 0000 3643 616e  B.0.........6Can
+00013450: 2774 2067 6574 2063 7572 7265 6e63 6965  't get currencie
+00013460: 7320 6672 6f6d 2073 756d 6d61 7279 2073  s from summary s
+00013470: 6563 7469 6f6e 206f 6620 7374 6174 656d  ection of statem
+00013480: 656e 7407 0000 000c 5374 6174 656d 656e  ent.....Statemen
+00013490: 7458 4c53 0103 0000 0046 041d 0435 0432  tXLS.....F...5.2
+000134a0: 043e 0437 043c 043e 0436 043d 043e 0020  .>.7.<.>.6.=.>. 
+000134b0: 043e 043f 0440 0435 0434 0435 043b 0438  .>.?.@.5.4.5.;.8
+000134c0: 0442 044c 0020 043f 0435 0440 0438 043e  .B.L. .?.5.@.8.>
+000134d0: 0434 0020 043e 0442 0447 0451 0442 0430  .4. .>.B.G.Q.B.0
+000134e0: 0800 0000 0006 0000 0018 4361 6e27 7420  ..........Can't 
+000134f0: 7265 6164 2072 6570 6f72 7420 7065 7269  read report peri
+00013500: 6f64 0700 0000 0c53 7461 7465 6d65 6e74  od.....Statement
+00013510: 584c 5301 0300 0000 1c04 1404 2100 2004  XLS.........!. .
+00013520: 3704 3004 3304 4004 4304 3604 3504 3d04  7.0.3.@.C.6.5.=.
+00013530: 4b00 3a00 2008 0000 0000 0600 0000 1643  K.:. ..........C
+00013540: 6173 6820 6261 6c61 6e63 6573 206c 6f61  ash balances loa
+00013550: 6465 643a 2007 0000 000c 5374 6174 656d  ded: .....Statem
+00013560: 656e 7458 4c53 0103 0000 0036 0421 0442  entXLS.....6.!.B
+00013570: 043e 043b 0431 0435 0446 0020 043d 0435  .>.;.1.5.F. .=.5
+00013580: 0020 043d 0430 0439 0434 0435 043d 0020  . .=.0.9.4.5.=. 
+00013590: 0432 0020 0441 0435 043a 0446 0438 0438  .2. .A.5.:.F.8.8
+000135a0: 0020 0800 0000 0006 0000 001c 436f 6c75  . ..........Colu
+000135b0: 6d6e 206e 6f74 2066 6f75 6e64 2069 6e20  mn not found in 
+000135c0: 7365 6374 696f 6e20 0700 0000 0c53 7461  section .....Sta
+000135d0: 7465 6d65 6e74 584c 5301 0300 0000 3404  tementXLS.....4.
+000135e0: 1d04 3504 4104 3a04 3e04 3b04 4c04 3a04  ..5.A.:.>.;.L.:.
+000135f0: 3e00 2004 4104 4704 3504 4204 3e04 3200  >. .A.G.5.B.>.2.
+00013600: 2004 3d04 3004 3904 3404 3504 3d04 3e00   .=.0.9.4.5.=.>.
+00013610: 3a00 2008 0000 0000 0600 0000 194d 756c  :. ..........Mul
+00013620: 7469 706c 6520 6163 636f 756e 7473 2066  tiple accounts f
+00013630: 6f75 6e64 3a20 0700 0000 0c53 7461 7465  ound: .....State
+00013640: 6d65 6e74 584c 5301 0300 0000 1c04 2604  mentXLS.......&.
+00013650: 1100 2004 3704 3004 3304 4004 4304 3604  .. .7.0.3.@.C.6.
+00013660: 3504 3d04 4b00 3a00 2008 0000 0000 0600  5.=.K.:. .......
+00013670: 0000 1353 6563 7572 6974 6965 7320 6c6f  ...Securities lo
+00013680: 6164 6564 3a20 0700 0000 0c53 7461 7465  aded: .....State
+00013690: 6d65 6e74 584c 5301 0300 0000 3004 1e04  mentXLS.....0...
+000136a0: 4204 4704 5104 4200 2004 3704 3004 3304  B.G.Q.B. .7.0.3.
+000136b0: 4004 4304 3604 3504 3d00 2004 4304 4104  @.C.6.5.=. .C.A.
+000136c0: 3f04 3504 4804 3d04 3e00 3a00 2008 0000  ?.5.H.=.>.:. ...
+000136d0: 0000 0600 0000 1f53 7461 7465 6d65 6e74  .......Statement
+000136e0: 206c 6f61 6465 6420 7375 6363 6573 7366   loaded successf
+000136f0: 756c 6c79 3a20 0700 0000 0c53 7461 7465  ully: .....State
+00013700: 6d65 6e74 584c 5301 0300 0000 2200 2004  mentXLS.....". .
+00013710: 3704 3004 3304 4004 4304 3604 3504 3d00  7.0.3.@.C.6.5.=.
+00013720: 2004 4304 4104 3f04 3504 4804 3d04 3e08   .C.A.?.5.H.=.>.
+00013730: 0000 0000 0600 0000 1420 6c6f 6164 6564  ......... loaded
+00013740: 2073 7563 6365 7373 6675 6c6c 7907 0000   successfully...
+00013750: 000c 5374 6174 656d 656e 7458 4d4c 0103  ..StatementXML..
+00013760: 0000 0036 041d 0435 0432 0435 0440 043d  ...6...5.2.5.@.=
+00013770: 044b 0439 0020 0444 043e 0440 043c 0430  .K.9. .D.>.@.<.0
+00013780: 0442 0020 0058 004d 004c 0020 0444 0430  .B. .X.M.L. .D.0
+00013790: 0439 043b 0430 003a 0020 0800 0000 0006  .9.;.0.:. ......
+000137a0: 0000 0016 4361 6e27 7420 7061 7273 6520  ....Can't parse 
+000137b0: 584d 4c20 6669 6c65 3a20 0700 0000 0c53  XML file: .....S
+000137c0: 7461 7465 6d65 6e74 584d 4c01 0300 0000  tatementXML.....
+000137d0: 4404 1d04 3504 3204 3e04 3704 3c04 3e04  D...5.2.>.7.<.>.
+000137e0: 3604 3d04 3e00 2004 3704 3004 3304 4004  6.=.>. .7.0.3.@.
+000137f0: 4304 3704 3804 4204 4c00 2004 3e04 4204  C.7.8.B.L. .>.B.
+00013800: 4704 5104 4200 2004 3d04 3e04 3c04 3504  G.Q.B. .=.>.<.5.
+00013810: 4000 3a00 2008 0000 0000 0600 0000 2046  @.:. ......... F
+00013820: 6169 6c65 6420 746f 2066 696e 6420 7374  ailed to find st
+00013830: 6174 656d 656e 7420 696e 6465 783a 2007  atement index: .
+00013840: 0000 000c 5374 6174 656d 656e 7458 4d4c  ....StatementXML
+00013850: 0103 0000 003e 041d 0435 0432 043e 0437  .....>...5.2.>.7
+00013860: 043c 043e 0436 043d 043e 0020 0437 0430  .<.>.6.=.>. .7.0
+00013870: 0433 0440 0443 0437 0438 0442 044c 0020  .3.@.C.7.8.B.L. 
+00013880: 0430 0442 0442 0440 0438 0431 0443 0442  .0.B.B.@.8.1.C.B
+00013890: 003a 0020 0800 0000 0006 0000 001a 4661  .:. ..........Fa
+000138a0: 696c 6564 2074 6f20 6c6f 6164 2061 7474  iled to load att
+000138b0: 7269 6275 7465 3a20 0700 0000 0c53 7461  ribute: .....Sta
+000138c0: 7465 6d65 6e74 584d 4c01 0300 0000 4204  tementXML.....B.
+000138d0: 1e04 4204 4704 5104 4200 2004 3104 4004  ..B.G.Q.B. .1.@.
+000138e0: 3e04 3a04 3504 4004 3000 2004 3d04 3500  >.:.5.@.0. .=.5.
+000138f0: 2004 3d04 3004 3904 3404 3504 3d00 2004   .=.0.9.4.5.=. .
+00013900: 3200 2004 4404 3004 3904 3b04 3500 3a00  2. .D.0.9.;.5.:.
+00013910: 2008 0000 0000 0600 0000 204e 6f20 7374   ......... No st
+00013920: 6174 656d 656e 7420 7761 7320 666f 756e  atement was foun
+00013930: 6420 696e 2066 696c 653a 2007 0000 000c  d in file: .....
+00013940: 5374 6174 656d 656e 7458 4d4c 0103 0000  StatementXML....
+00013950: 0034 041d 0435 0438 0437 0432 0435 0441  .4...5.8.7.2.5.A
+00013960: 0442 043d 0430 044f 0020 043c 0435 0442  .B.=.0.O. .<.5.B
+00013970: 043a 0430 0020 043e 0442 0447 0451 0442  .:.0. .>.B.G.Q.B
+00013980: 0430 003a 0020 0800 0000 0006 0000 0017  .0.:. ..........
+00013990: 556e 6b6e 6f77 6e20 7374 6174 656d 656e  Unknown statemen
+000139a0: 7420 7461 673a 2007 0000 000c 5374 6174  t tag: .....Stat
+000139b0: 656d 656e 7458 4d4c 0103 0000 004c 041d  ementXML.....L..
+000139c0: 0435 043f 043e 0434 0434 0435 0440 0436  .5.?.>.4.4.5.@.6
+000139d0: 0438 0432 0430 0435 043c 044b 0439 0020  .8.2.0.5.<.K.9. 
+000139e0: 0444 043e 0440 043c 0430 0442 0020 0434  .D.>.@.<.0.B. .4
+000139f0: 0430 0442 044b 002f 0432 0440 0435 043c  .0.B.K./.2.@.5.<
+00013a00: 0435 043d 0438 003a 0020 0800 0000 0006  .5.=.8.:. ......
+00013a10: 0000 001e 556e 7375 7070 6f72 7465 6420  ....Unsupported 
+00013a20: 6461 7465 2f74 696d 6520 666f 726d 6174  date/time format
+00013a30: 3a20 0700 0000 0c53 7461 7465 6d65 6e74  : .....Statement
+00013a40: 584d 4c01 0300 0000 8600 2000 2d00 2004  XML....... .-. .
+00013a50: 3c04 3e04 3404 4304 3b04 4c00 2004 3d04  <.>.4.C.;.L. .=.
+00013a60: 3500 2004 3f04 3e04 3404 3404 3504 4004  5. .?.>.4.4.5.@.
+00013a70: 3604 3804 3204 3004 3504 4200 2004 3704  6.8.2.0.5.B. .7.
+00013a80: 3004 3304 4004 4304 3704 3a04 4300 2004  0.3.@.C.7.:.C. .
+00013a90: 3d04 3504 4104 3a04 3e04 3b04 4c04 3a04  =.5.A.:.>.;.L.:.
+00013aa0: 3804 4500 2004 3e04 4204 4704 5104 4204  8.E. .>.B.G.Q.B.
+00013ab0: 3e04 3200 2004 3e04 3404 3d04 3e04 3204  >.2. .>.4.=.>.2.
+00013ac0: 4004 3504 3c04 3504 3d04 3d04 3e00 2e08  @.5.<.5.=.=.>...
+00013ad0: 0000 0000 0600 0000 3320 2d20 6d6f 6475  ........3 - modu
+00013ae0: 6c65 2064 6f65 736e 2774 2073 7570 706f  le doesn't suppo
+00013af0: 7274 206d 756c 7469 706c 6520 7374 6174  rt multiple stat
+00013b00: 656d 656e 7473 206c 6f61 642e 0700 0000  ements load.....
+00013b10: 0a53 7461 7465 6d65 6e74 7301 0300 0000  .Statements.....
+00013b20: 2004 1e04 4804 3804 3104 3a04 3000 2004   ...H.8.1.:.0. .
+00013b30: 3804 3c04 3f04 3e04 4004 4204 3000 3a00  8.<.?.>.@.B.0.:.
+00013b40: 2008 0000 0000 0600 0000 0f49 6d70 6f72   ..........Impor
+00013b50: 7420 6661 696c 6564 3a20 0700 0000 0a53  t failed: .....S
+00013b60: 7461 7465 6d65 6e74 7301 0300 0000 4604  tatements.....F.
+00013b70: 1204 4b04 3104 3504 4004 3804 4204 3500  ..K.1.5.@.8.B.5.
+00013b80: 2004 4404 3004 3904 3b04 4b00 2004 3e04   .D.0.9.;.K. .>.
+00013b90: 4204 4704 5104 4204 3e04 3200 2004 3404  B.G.Q.B.>.2. .4.
+00013ba0: 3b04 4f00 2004 3704 3004 3304 4004 4304  ;.O. .7.0.3.@.C.
+00013bb0: 3704 3a04 3808 0000 0000 0600 0000 2053  7.:.8......... S
+00013bc0: 656c 6563 7420 7374 6174 656d 656e 7420  elect statement 
+00013bd0: 6669 6c65 7320 746f 2069 6d70 6f72 7407  files to import.
+00013be0: 0000 000a 5374 6174 656d 656e 7473 0103  ....Statements..
+00013bf0: 0000 004a 041a 043b 0430 0441 0441 0020  ...J...;.0.A.A. 
+00013c00: 043e 0442 0447 0451 0442 0430 0020 043d  .>.B.G.Q.B.0. .=
+00013c10: 0435 0020 043c 043e 0436 0435 0442 0020  .5. .<.>.6.5.B. 
+00013c20: 0431 044b 0442 044c 0020 0437 0430 0433  .1.K.B.L. .7.0.3
+00013c30: 0440 0443 0436 0435 043d 003a 0020 0800  .@.C.6.5.=.:. ..
+00013c40: 0000 0006 0000 0021 5374 6174 656d 656e  .......!Statemen
+00013c50: 7420 636c 6173 7320 6361 6e27 7420 6265  t class can't be
+00013c60: 206c 6f61 6465 643a 2007 0000 000a 5374   loaded: .....St
+00013c70: 6174 656d 656e 7473 0103 0000 0054 041c  atements.....T..
+00013c80: 043e 0434 0443 043b 044c 0020 043e 0442  .>.4.C.;.L. .>.B
+00013c90: 0447 0451 0442 0430 0020 043d 0435 0020  .G.Q.B.0. .=.5. 
+00013ca0: 043c 043e 0436 0435 0442 0020 0431 044b  .<.>.6.5.B. .1.K
+00013cb0: 0442 044c 0020 0438 043c 043f 043e 0440  .B.L. .8.<.?.>.@
+00013cc0: 0442 0438 0440 043e 0432 0430 043d 003a  .B.8.@.>.2.0.=.:
+00013cd0: 0020 0800 0000 0006 0000 0024 5374 6174  . .........$Stat
+00013ce0: 656d 656e 7420 6d6f 6475 6c65 2063 616e  ement module can
+00013cf0: 2774 2062 6520 696d 706f 7274 6564 3a20  't be imported: 
+00013d00: 0700 0000 0a53 7461 7465 6d65 6e74 7301  .....Statements.
+00013d10: 0300 0000 0804 1004 3a04 4200 2e08 0000  ........:.B.....
+00013d20: 0000 0600 0000 0441 6374 2e07 0000 0010  .......Act......
+00013d30: 5379 6d62 6f6c 734c 6973 744d 6f64 656c  SymbolsListModel
+00013d40: 0103 0000 000c 0412 0430 043b 044e 0442  .........0.;.N.B
+00013d50: 0430 0800 0000 0006 0000 0008 4375 7272  .0..........Curr
+00013d60: 656e 6379 0700 0000 1053 796d 626f 6c73  ency.....Symbols
+00013d70: 4c69 7374 4d6f 6465 6c01 0300 0000 1004  ListModel.......
+00013d80: 1e04 3f04 3804 4104 3004 3d04 3804 3508  ..?.8.A.0.=.8.5.
+00013d90: 0000 0000 0600 0000 0b44 6573 6372 6970  .........Descrip
+00013da0: 7469 6f6e 0700 0000 1053 796d 626f 6c73  tion.....Symbols
+00013db0: 4c69 7374 4d6f 6465 6c01 0300 0000 1204  ListModel.......
+00013dc0: 1a04 3e04 4204 3804 4004 3e04 3204 3a04  ..>.B.8.@.>.2.:.
+00013dd0: 3808 0000 0000 0600 0000 0651 756f 7465  8..........Quote
+00013de0: 7307 0000 0010 5379 6d62 6f6c 734c 6973  s.....SymbolsLis
+00013df0: 744d 6f64 656c 0103 0000 000c 0421 0438  tModel.......!.8
+00013e00: 043c 0432 043e 043b 0800 0000 0006 0000  .<.2.>.;........
+00013e10: 0006 5379 6d62 6f6c 0700 0000 1053 796d  ..Symbol.....Sym
+00013e20: 626f 6c73 4c69 7374 4d6f 6465 6c01 0300  bolsListModel...
+00013e30: 0000 0604 2204 4d04 3308 0000 0000 0600  ....".M.3.......
+00013e40: 0000 0354 6167 0700 0000 0c54 6167 4c69  ...Tag.....TagLi
+00013e50: 7374 4d6f 6465 6c01 0300 0000 1004 1e04  stModel.........
+00013e60: 3f04 3504 4004 3004 4604 3804 3808 0000  ?.5.@.0.F.8.8...
+00013e70: 0000 0600 0000 0a4f 7065 7261 7469 6f6e  .......Operation
+00013e80: 7307 0000 0009 5461 6752 6570 6f72 7401  s.....TagReport.
+00013e90: 0300 0000 1004 3f04 3e00 2004 1c04 3504  ......?.>. ...5.
+00013ea0: 4204 3a04 3508 0000 0000 0600 0000 0662  B.:.5..........b
+00013eb0: 7920 5461 6707 0000 0009 5461 6752 6570  y Tag.....TagRep
+00013ec0: 6f72 7401 0300 0000 1c04 1e04 4204 4704  ort.........B.G.
+00013ed0: 3504 4200 2004 3f04 3e00 2004 3c04 3504  5.B. .?.>. .<.5.
+00013ee0: 4204 3a04 3508 0000 0000 0600 0000 0d52  B.:.5..........R
+00013ef0: 6570 6f72 7420 6279 2074 6167 0700 0000  eport by tag....
+00013f00: 0f54 6167 5265 706f 7274 5769 6467 6574  .TagReportWidget
+00013f10: 0103 0000 000c 041c 0435 0442 043a 0430  .........5.B.:.0
+00013f20: 003a 0800 0000 0006 0000 0004 5461 673a  .:..........Tag:
+00013f30: 0700 0000 0f54 6167 5265 706f 7274 5769  .....TagReportWi
+00013f40: 6467 6574 0103 0000 0024 0027 0020 0437  dget.....$.'. .7
+00013f50: 0430 043c 0435 043d 0435 043d 0430 0020  .0.<.5.=.5.=.0. 
+00013f60: 0443 0441 043f 0435 0448 043d 043e 0800  .C.A.?.5.H.=.>..
+00013f70: 0000 0006 0000 001b 2720 7761 7320 7375  ........' was su
+00013f80: 6363 6573 7366 756c 6c79 2072 6570 6c61  ccessfully repla
+00013f90: 6365 6407 0000 000e 5461 6773 4c69 7374  ced.....TagsList
+00013fa0: 4469 616c 6f67 0103 0000 000c 0027 0020  Dialog.......'. 
+00013fb0: 043d 0430 003a 0020 0800 0000 0006 0000  .=.0.:. ........
+00013fc0: 0008 2720 7769 7468 3a20 0700 0000 0e54  ..' with: .....T
+00013fd0: 6167 734c 6973 7444 6961 6c6f 6701 0300  agsListDialog...
+00013fe0: 0000 2004 1704 3004 3c04 3504 3d04 3804  .. ...0.<.5.=.8.
+00013ff0: 4204 4c00 2004 3c04 3504 4204 3a04 4300  B.L. .<.5.B.:.C.
+00014000: 2000 2708 0000 0000 0600 0000 0d52 6570   .'..........Rep
+00014010: 6c61 6365 2074 6167 2027 0700 0000 0e54  lace tag '.....T
+00014020: 6167 734c 6973 7444 6961 6c6f 6701 0300  agsListDialog...
+00014030: 0000 1c04 1704 3004 3c04 3504 3d04 3804  ......0.<.5.=.8.
+00014040: 4204 4c00 2004 3d04 3000 2e00 2e00 2e08  B.L. .=.0.......
+00014050: 0000 0000 0600 0000 0f52 6570 6c61 6365  .........Replace
+00014060: 2077 6974 682e 2e2e 0700 0000 0e54 6167   with........Tag
+00014070: 734c 6973 7444 6961 6c6f 6701 0300 0000  sListDialog.....
+00014080: 3404 1f04 3e04 3a04 3004 3704 3004 4204  4...>.:.0.7.0.B.
+00014090: 4c00 2004 3e04 3f04 3504 4004 3004 4604  L. .>.?.5.@.0.F.
+000140a0: 3804 3800 2004 4100 2004 1c04 3504 4204  8.8. .A. ...5.B.
+000140b0: 3a04 3e04 3908 0000 0000 0600 0000 1853  :.>.9..........S
+000140c0: 686f 7720 6f70 6572 6174 696f 6e73 2077  how operations w
+000140d0: 6974 6820 5461 6707 0000 000e 5461 6773  ith Tag.....Tags
+000140e0: 4c69 7374 4469 616c 6f67 0103 0000 000e  ListDialog......
+000140f0: 041c 0435 0442 043a 0430 0020 0027 0800  ...5.B.:.0. .'..
+00014100: 0000 0006 0000 0005 5461 6720 2707 0000  ........Tag '...
+00014110: 000e 5461 6773 4c69 7374 4469 616c 6f67  ..TagsListDialog
+00014120: 0103 0000 0008 0422 044d 0433 0438 0800  .......".M.3.8..
+00014130: 0000 0006 0000 0004 5461 6773 0700 0000  ........Tags....
+00014140: 0e54 6167 734c 6973 7444 6961 6c6f 6701  .TagsListDialog.
+00014150: 0300 0000 1a04 2204 3504 3a04 4304 4904  ......".5.:.C.I.
+00014160: 3804 3900 2004 3a04 4304 4004 4100 3a08  8.9. .:.C.@.A.:.
+00014170: 0000 0000 0600 0000 0d43 7572 7265 6e74  .........Current
+00014180: 2072 6174 653a 0700 0000 1354 6178 4573   rate:.....TaxEs
+00014190: 7469 6d61 7469 6f6e 4469 616c 6f67 0103  timationDialog..
+000141a0: 0000 0028 041f 043e 0441 043b 0435 0434  ...(...>.A.;.5.4
+000141b0: 043d 044f 044f 0020 043a 043e 0442 0438  .=.O.O. .:.>.B.8
+000141c0: 0440 043e 0432 043a 0430 003a 0800 0000  .@.>.2.:.0.:....
+000141d0: 0006 0000 000b 4c61 7374 2071 756f 7465  ......Last quote
+000141e0: 3a07 0000 0013 5461 7845 7374 696d 6174  :.....TaxEstimat
+000141f0: 696f 6e44 6961 6c6f 6701 0300 0000 1a04  ionDialog.......
+00014200: 1e04 4604 3504 3d04 3a04 3000 2004 3d04  ..F.5.=.:.0. .=.
+00014210: 3004 3b04 3e04 3304 3008 0000 0000 0600  0.;.>.3.0.......
+00014220: 0000 0e54 6178 2045 7374 696d 6174 696f  ...Tax Estimatio
+00014230: 6e07 0000 0013 5461 7845 7374 696d 6174  n.....TaxEstimat
+00014240: 696f 6e44 6961 6c6f 6701 0300 0000 0800  ionDialog.......
+00014250: 5800 2e00 5800 5808 0000 0000 0600 0000  X...X.X.........
+00014260: 0458 2e58 5807 0000 0013 5461 7845 7374  .X.XX.....TaxEst
+00014270: 696d 6174 696f 6e44 6961 6c6f 6701 0300  imationDialog...
+00014280: 0000 0a04 1804 2204 1e04 1304 1e08 0000  ......".........
+00014290: 0000 0600 0000 0554 4f54 414c 0700 0000  .......TOTAL....
+000142a0: 0c54 6178 4573 7469 6d61 746f 7201 0300  .TaxEstimator...
+000142b0: 0000 2404 1e04 4604 3504 3d04 3a04 3000  ..$...F.5.=.:.0.
+000142c0: 2004 3d04 3004 3b04 3e04 3304 3000 2004   .=.0.;.>.3.0. .
+000142d0: 3404 3b04 4f00 2008 0000 0000 0600 0000  4.;.O. .........
+000142e0: 1354 6178 2065 7374 696d 6174 696f 6e20  .Tax estimation 
+000142f0: 666f 7220 0700 0000 0c54 6178 4573 7469  for .....TaxEsti
+00014300: 6d61 746f 7201 0300 0000 3c04 2104 4204  mator.....<.!.B.
+00014310: 3004 3204 3a04 3000 2004 3d04 3004 3b04  0.2.:.0. .=.0.;.
+00014320: 3e04 3304 3000 2004 3d04 3500 2004 3d04  >.3.0. .=.5. .=.
+00014330: 3004 3904 3404 3504 3d04 3000 2004 3404  0.9.4.5.=.0. .4.
+00014340: 3b04 4f00 3a00 2008 0000 0000 0600 0000  ;.O.:. .........
+00014350: 1854 6178 2072 6174 6520 6e6f 7420 666f  .Tax rate not fo
+00014360: 756e 6420 666f 723a 2007 0000 000c 5461  und for: .....Ta
+00014370: 7845 7374 696d 6174 6f72 0103 0000 0008  xEstimator......
+00014380: 0414 0430 0442 0430 0800 0000 0006 0000  ...0.B.0........
+00014390: 0004 4461 7465 0700 0000 1154 6178 4573  ..Date.....TaxEs
+000143a0: 7469 6d61 746f 724d 6f64 656c 0103 0000  timatorModel....
+000143b0: 0014 0426 0435 043d 0430 0020 043e 0442  ...&.5.=.0. .>.B
+000143c0: 043a 0440 002e 0800 0000 0006 0000 0004  .:.@............
+000143d0: 4f70 656e 0700 0000 1154 6178 4573 7469  Open.....TaxEsti
+000143e0: 6d61 746f 724d 6f64 656c 0103 0000 0012  matorModel......
+000143f0: 041f 0440 0438 0431 044b 043b 044c 002c  ...@.8.1.K.;.L.,
+00014400: 0020 0800 0000 0006 0000 0008 5072 6f66  . ..........Prof
+00014410: 6974 2c20 0700 0000 1154 6178 4573 7469  it, .....TaxEsti
+00014420: 6d61 746f 724d 6f64 656c 0103 0000 000c  matorModel......
+00014430: 041a 043e 043b 002d 0432 043e 0800 0000  ...>.;.-.2.>....
+00014440: 0006 0000 0003 5174 7907 0000 0011 5461  ......Qty.....Ta
+00014450: 7845 7374 696d 6174 6f72 4d6f 6465 6c01  xEstimatorModel.
+00014460: 0300 0000 0c04 1a04 4304 4004 4100 2c00  ........C.@.A.,.
+00014470: 2008 0000 0000 0600 0000 0652 6174 652c   ..........Rate,
+00014480: 2007 0000 0011 5461 7845 7374 696d 6174   .....TaxEstimat
+00014490: 6f72 4d6f 6465 6c01 0300 0000 0e04 1d04  orModel.........
+000144a0: 3004 3b04 3e04 3300 2c00 2008 0000 0000  0.;.>.3.,. .....
+000144b0: 0600 0000 0554 6178 2c20 0700 0000 1154  .....Tax, .....T
+000144c0: 6178 4573 7469 6d61 746f 724d 6f64 656c  axEstimatorModel
+000144d0: 0103 0000 0074 041d 0435 0432 043e 0437  .....t...5.2.>.7
+000144e0: 043c 043e 0436 043d 043e 0020 0437 0430  .<.>.6.=.>. .7.0
+000144f0: 0433 0440 0443 0437 0438 0442 044c 0020  .3.@.C.7.8.B.L. 
+00014500: 043f 0430 0440 0430 043c 0435 0442 0440  .?.0.@.0.<.5.B.@
+00014510: 044b 0020 043d 0430 043b 043e 0433 043e  .K. .=.0.;.>.3.>
+00014520: 0432 043e 0433 043e 0020 043e 0442 0447  .2.>.3.>. .>.B.G
+00014530: 0451 0442 0430 0020 0438 0437 0020 0444  .Q.B.0. .8.7. .D
+00014540: 0430 0439 043b 0430 0020 0800 0000 0006  .0.9.;.0. ......
+00014550: 0000 002b 4361 6e27 7420 6c6f 6164 2074  ...+Can't load t
+00014560: 6178 2072 6570 6f72 7420 7061 7261 6d65  ax report parame
+00014570: 7465 7273 2066 726f 6d20 6669 6c65 2007  ters from file .
+00014580: 0000 0009 5461 7852 6570 6f72 7401 0300  ....TaxReport...
+00014590: 0000 2804 1d04 3504 3804 3704 3204 3504  ..(...5.8.7.2.5.
+000145a0: 4104 4204 3d04 3004 4f00 2004 3204 3004  A.B.=.0.O. .2.0.
+000145b0: 3b04 4e04 4204 3000 3a00 2008 0000 0000  ;.N.B.0.:. .....
+000145c0: 0600 0000 1943 7572 7265 6e63 7920 6973  .....Currency is
+000145d0: 206e 6f74 2064 6566 696e 6564 3a20 0700   not defined: ..
+000145e0: 0000 0954 6178 5265 706f 7274 0103 0000  ...TaxReport....
+000145f0: 004a 041d 0435 0020 0443 043a 0430 0437  .J...5. .C.:.0.7
+00014600: 0430 043d 0020 0448 0430 0431 043b 043e  .0.=. .H.0.1.;.>
+00014610: 043d 0020 043e 0442 0447 0435 0442 0430  .=. .>.B.G.5.B.0
+00014620: 0020 0434 043b 044f 0020 0440 0430 0437  . .4.;.O. .@.0.7
+00014630: 0434 0435 043b 0430 003a 0020 0800 0000  .4.5.;.0.:. ....
+00014640: 0006 0000 0026 4e6f 2072 6570 6f72 7420  .....&No report 
+00014650: 7465 6d70 6c61 7465 2066 6f75 6e64 2066  template found f
+00014660: 6f72 2073 6563 7469 6f6e 3a20 0700 0000  or section: ....
+00014670: 0954 6178 5265 706f 7274 0103 0000 006a  .TaxReport.....j
+00014680: 041d 0435 0442 0020 0438 043d 0444 043e  ...5.B. .8.=.D.>
+00014690: 0440 043c 0430 0446 0438 0438 0020 043e  .@.<.0.F.8.8. .>
+000146a0: 0020 0421 043e 0418 0414 041d 0020 0432  . .!.>....... .2
+000146b0: 0020 043f 0430 0440 0430 043c 0435 0442  . .?.0.@.0.<.5.B
+000146c0: 0440 0430 0445 0020 043d 0430 043b 043e  .@.0.E. .=.0.;.>
+000146d0: 0433 043e 0432 043e 0433 043e 0020 043e  .3.>.2.>.3.>. .>
+000146e0: 0442 0447 0451 0442 0430 0800 0000 0006  .B.G.Q.B.0......
+000146f0: 0000 0042 5468 6572 6520 6172 6520 6e6f  ...BThere are no
+00014700: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00014710: 7574 2074 6178 2074 7265 6174 7920 696e  ut tax treaty in
+00014720: 2074 6178 2072 6570 6f72 7420 7061 7261   tax report para
+00014730: 6d65 7465 7273 0700 0000 0954 6178 5265  meters.....TaxRe
+00014740: 706f 7274 0103 0000 0060 041d 0435 0020  port.....`...5. 
+00014750: 0437 0430 0434 0430 043d 044b 0020 043f  .7.0.4.0.=.K. .?
+00014760: 0430 0440 0430 043c 0435 0442 0440 044b  .0.@.0.<.5.B.@.K
+00014770: 0020 043d 0430 043b 043e 0433 043e 0432  . .=.0.;.>.3.>.2
+00014780: 043e 0433 043e 0020 043e 0442 0447 0451  .>.3.>. .>.B.G.Q
+00014790: 0442 0430 0020 0434 043b 044f 0020 0433  .B.0. .4.;.O. .3
+000147a0: 043e 0434 0430 003a 0020 0800 0000 0006  .>.4.0.:. ......
+000147b0: 0000 0033 5468 6572 6520 6172 6520 6e6f  ...3There are no
+000147c0: 2070 6172 616d 6574 6572 7320 666f 756e   parameters foun
+000147d0: 6420 666f 7220 7461 7820 7265 706f 7274  d for tax report
+000147e0: 2079 6561 723a 2007 0000 0009 5461 7852   year: .....TaxR
+000147f0: 6570 6f72 7401 0300 0000 0a00 2000 2e00  eport....... ...
+00014800: 2e00 2e00 2008 0000 0000 0600 0000 0520  .... .......... 
+00014810: 2e2e 2e20 0700 0000 0954 6178 5769 6467  ... .....TaxWidg
+00014820: 6574 0103 0000 0006 002e 002e 002e 0800  et..............
+00014830: 0000 0006 0000 0003 2e2e 2e07 0000 0009  ................
+00014840: 5461 7857 6964 6765 7401 0300 0000 0a04  TaxWidget.......
+00014850: 2104 4704 3504 4200 3a08 0000 0000 0600  !.G.5.B.:.......
+00014860: 0000 0841 6363 6f75 6e74 3a07 0000 0009  ...Account:.....
+00014870: 5461 7857 6964 6765 7401 0300 0000 9004  TaxWidget.......
+00014880: 1d04 3804 3604 3500 2004 4004 3004 4104  ..8.6.5. .@.0.A.
+00014890: 3f04 3e04 3b04 3e04 3604 3504 3d04 4b00  ?.>.;.>.6.5.=.K.
+000148a0: 2004 4d04 3a04 4104 3f04 3504 4004 3804   .M.:.A.?.5.@.8.
+000148b0: 3c04 3504 3d04 4204 3004 3b04 4c04 3d04  <.5.=.B.0.;.L.=.
+000148c0: 4b04 3500 2004 4404 4304 3d04 3a04 4604  K.5. .D.C.=.:.F.
+000148d0: 3804 3800 2000 2d00 2004 3804 4104 3f04  8.8. .-. .8.A.?.
+000148e0: 3e04 3b04 4c04 3704 4304 3904 4204 3500  >.;.L.7.C.9.B.5.
+000148f0: 2004 4100 2004 3e04 4104 4204 3e04 4004   .A. .>.A.B.>.@.
+00014900: 3e04 3604 3d04 3e04 4104 4204 4c04 4e08  >.6.=.>.A.B.L.N.
+00014910: 0000 0000 0600 0000 3342 656c 6f77 2066  ........3Below f
+00014920: 756e 6374 696f 6e73 2061 7265 2065 7870  unctions are exp
+00014930: 6572 696d 656e 7461 6c20 2d20 7573 6520  erimental - use 
+00014940: 6974 2077 6974 6820 6361 7265 0700 0000  it with care....
+00014950: 0954 6178 5769 6467 6574 0103 0000 0044  .TaxWidget.....D
+00014960: 041d 0435 0432 043e 0437 043c 043e 0436  ...5.2.>.7.<.>.6
+00014970: 043d 043e 0020 0437 0430 043f 0438 0441  .=.>. .7.0.?.8.A
+00014980: 0430 0442 044c 0020 0033 002d 041d 0414  .0.B.L. .3.-....
+00014990: 0424 041b 0020 0432 0020 0444 0430 0439  .$... .2. .D.0.9
+000149a0: 043b 0020 0800 0000 0006 0000 001f 4361  .;. ..........Ca
+000149b0: 6e27 7420 7772 6974 6520 7461 7820 666f  n't write tax fo
+000149c0: 726d 2069 6e74 6f20 6669 6c65 2007 0000  rm into file ...
+000149d0: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+000149e0: 0e04 2104 4204 4004 3004 3d04 3000 3a08  ..!.B.@.0.=.0.:.
+000149f0: 0000 0000 0600 0000 0843 6f75 6e74 7279  .........Country
+00014a00: 3a07 0000 0009 5461 7857 6964 6765 7401  :.....TaxWidget.
+00014a10: 0300 0000 7804 2104 3e04 3704 3404 3004  ....x.!.>.7.4.0.
+00014a20: 4204 4c00 2004 4404 3004 3904 3b00 2000  B.L. .D.0.9.;. .
+00014a30: 3300 2d04 1d04 2404 1404 1b00 2004 3200  3.-...$..... .2.
+00014a40: 2004 4404 3e04 4004 3c04 3004 4204 3500   .D.>.@.<.0.B.5.
+00014a50: 2004 3f04 4004 3e04 3304 4004 3004 3c04   .?.@.>.3.@.0.<.
+00014a60: 3c04 4b00 2000 2204 1404 3504 3a04 3b04  <.K. ."...5.:.;.
+00014a70: 3004 4004 3004 4604 3804 4f00 2200 2000  0.@.0.F.8.O.". .
+00014a80: 2800 2a00 2e00 6400 6300 5800 2908 0000  (.*...d.c.X.)...
+00014a90: 0000 0600 0000 4043 7265 6174 6520 7461  ......@Create ta
+00014aa0: 7820 666f 726d 2069 6e20 22d0 94d0 b5d0  x form in ".....
+00014ab0: bad0 bbd0 b0d1 80d0 b0d1 86d0 b8d1 8f22  ..............."
+00014ac0: 2070 726f 6772 616d 2066 6f72 6d61 7420   program format 
+00014ad0: 282a 2e64 6358 2907 0000 0009 5461 7857  (*.dcX).....TaxW
+00014ae0: 6964 6765 7401 0300 0000 1e04 1404 3004  idget.........0.
+00014af0: 3d04 3d04 4b04 3500 2004 3d04 3504 3f04  =.=.K.5. .=.5.?.
+00014b00: 3e04 3b04 3d04 4b04 3508 0000 0000 0600  >.;.=.K.5.......
+00014b10: 0000 1344 6174 6120 6172 6520 696e 636f  ...Data are inco
+00014b20: 6d70 6c65 7465 0700 0000 0954 6178 5769  mplete.....TaxWi
+00014b30: 6467 6574 0103 0000 005c 041d 0435 0020  dget.....\...5. 
+00014b40: 0438 0441 043f 043e 043b 044c 0437 043e  .8.A.?.>.;.L.7.>
+00014b50: 0432 0430 0442 044c 0020 0434 0430 0442  .2.0.B.L. .4.0.B
+00014b60: 0443 0020 043f 043e 0441 0442 0430 0432  .C. .?.>.A.B.0.2
+00014b70: 043a 0438 0020 0434 043b 044f 0020 043a  .:.8. .4.;.O. .:
+00014b80: 0443 0440 0441 043e 0432 0020 0432 0430  .C.@.A.>.2. .2.0
+00014b90: 043b 044e 0442 0800 0000 0006 0000 002d  .;.N.B.........-
+00014ba0: 446f 206e 6f74 2075 7365 2073 6574 746c  Do not use settl
+00014bb0: 656d 656e 7420 6461 7465 2066 6f72 2063  ement date for c
+00014bc0: 7572 7265 6e63 7920 7261 7465 7307 0000  urrency rates...
+00014bd0: 0009 5461 7857 6964 6765 7401 0300 0000  ..TaxWidget.....
+00014be0: 1604 2404 3004 3904 3b00 2000 4500 7800  ..$.0.9.;. .E.x.
+00014bf0: 6300 6500 6c00 3a08 0000 0000 0600 0000  c.e.l.:.........
+00014c00: 0b45 7863 656c 2066 696c 653a 0700 0000  .Excel file:....
+00014c10: 0954 6178 5769 6467 6574 0103 0000 0028  .TaxWidget.....(
+00014c20: 0424 0430 0439 043b 044b 0020 0045 0078  .$.0.9.;.K. .E.x
+00014c30: 0063 0065 006c 0020 0028 002a 002e 0078  .c.e.l. .(.*...x
+00014c40: 0073 006c 0078 0029 0800 0000 0006 0000  .s.l.x.)........
+00014c50: 0014 4578 6365 6c20 6669 6c65 7320 282a  ..Excel files (*
+00014c60: 2e78 6c73 7829 0700 0000 0954 6178 5769  .xlsx).....TaxWi
+00014c70: 6467 6574 0103 0000 004a 0424 0430 0439  dget.....J.$.0.9
+00014c80: 043b 0020 0434 043b 044f 0020 0441 043e  .;. .4.;.O. .A.>
+00014c90: 0445 0440 0430 043d 0435 043d 0438 044f  .E.@.0.=.5.=.8.O
+00014ca0: 0020 0434 0435 043a 043b 0430 0440 0430  . .4.5.:.;.0.@.0
+00014cb0: 0446 0438 0438 0020 0033 002d 041d 0414  .F.8.8. .3.-....
+00014cc0: 0424 041b 0800 0000 0006 0000 0024 4669  .$...........$Fi
+00014cd0: 6c65 2077 6865 7265 2074 6f20 7374 6f72  le where to stor
+00014ce0: 6520 7275 7373 6961 6e20 7461 7820 666f  e russian tax fo
+00014cf0: 726d 0700 0000 0954 6178 5769 6467 6574  rm.....TaxWidget
+00014d00: 0103 0000 0056 0424 0430 0439 043b 0020  .....V.$.0.9.;. 
+00014d10: 0434 043b 044f 0020 0441 043e 0445 0440  .4.;.O. .A.>.E.@
+00014d20: 0430 043d 0435 043d 0438 044f 0020 0440  .0.=.5.=.8.O. .@
+00014d30: 0430 0441 0447 0451 0442 0430 0020 0432  .0.A.G.Q.B.0. .2
+00014d40: 0020 0444 043e 0440 043c 0430 0442 0435  . .D.>.@.<.0.B.5
+00014d50: 0020 0045 0078 0063 0065 006c 0800 0000  . .E.x.c.e.l....
+00014d60: 0006 0000 002e 4669 6c65 2077 6865 7265  ......File where
+00014d70: 2074 6f20 7374 6f72 6520 7461 7820 7265   to store tax re
+00014d80: 706f 7274 2069 6e20 4578 6365 6c20 666f  port in Excel fo
+00014d90: 726d 6174 0700 0000 0954 6178 5769 6467  rmat.....TaxWidg
+00014da0: 6574 0103 0000 0068 0417 0430 0440 0443  et.....h...0.@.C
+00014db0: 0431 0435 0436 043d 044b 0439 0020 0441  .1.5.6.=.K.9. .A
+00014dc0: 0447 0451 0442 0020 0434 043b 044f 0020  .G.Q.B. .4.;.O. 
+00014dd0: 043a 043e 0442 043e 0440 043e 0433 043e  .:.>.B.>.@.>.3.>
+00014de0: 0020 043d 0443 0436 043d 043e 0020 043f  . .=.C.6.=.>. .?
+00014df0: 043e 0434 0433 043e 0442 043e 0432 0438  .>.4.3.>.B.>.2.8
+00014e00: 0442 044c 0020 043e 0442 0447 0451 0442  .B.L. .>.B.G.Q.B
+00014e10: 0800 0000 0006 0000 0029 466f 7265 6967  .........)Foreig
+00014e20: 6e20 6163 636f 756e 7420 746f 2070 7265  n account to pre
+00014e30: 7061 7265 2074 6178 2072 6570 6f72 7420  pare tax report 
+00014e40: 666f 7207 0000 0009 5461 7857 6964 6765  for.....TaxWidge
+00014e50: 7401 0300 0000 2604 2404 3004 3904 3b00  t.....&.$.0.9.;.
+00014e60: 2004 4100 2004 4004 3504 3704 4304 3b04   .A. .@.5.7.C.;.
+00014e70: 4c04 4204 3004 4204 3e04 3c00 3a08 0000  L.B.0.B.>.<.:...
+00014e80: 0000 0600 0000 0c4f 7574 7075 7420 6669  .......Output fi
+00014e90: 6c65 3a07 0000 0009 5461 7857 6964 6765  le:.....TaxWidge
+00014ea0: 7401 0300 0000 1e04 2104 3e04 4504 4004  t.......!.>.E.@.
+00014eb0: 3004 3d04 3804 4204 4c00 2004 1e04 4204  0.=.8.B.L. ...B.
+00014ec0: 4704 5104 4208 0000 0000 0600 0000 0b53  G.Q.B..........S
+00014ed0: 6176 6520 5265 706f 7274 0700 0000 0954  ave Report.....T
+00014ee0: 6178 5769 6467 6574 0103 0000 0026 0421  axWidget.....&.!
+00014ef0: 043e 0445 0440 0430 043d 0438 0442 044c  .>.E.@.0.=.8.B.L
+00014f00: 0020 0033 002d 041d 0414 0424 041b 0020  . .3.-.....$... 
+00014f10: 0432 003a 0800 0000 0006 0000 0011 5361  .2.:..........Sa
+00014f20: 7665 2074 6178 2066 6f72 6d20 746f 3a07  ve tax form to:.
+00014f30: 0000 0009 5461 7857 6964 6765 7401 0300  ....TaxWidget...
+00014f40: 0000 3804 2104 3e04 4504 4004 3004 3d04  ..8.!.>.E.@.0.=.
+00014f50: 3804 4204 4c00 2004 3d04 3004 3b04 3e04  8.B.L. .=.0.;.>.
+00014f60: 3304 3e04 3204 4b04 3900 2004 3e04 4204  3.>.2.K.9. .>.B.
+00014f70: 4704 5104 4200 2004 3200 3a08 0000 0000  G.Q.B. .2.:.....
+00014f80: 0600 0000 1453 6176 6520 7461 7820 7265  .....Save tax re
+00014f90: 706f 7274 7320 746f 3a07 0000 0009 5461  ports to:.....Ta
+00014fa0: 7857 6964 6765 7401 0300 0000 1804 1204  xWidget.........
+00014fb0: 4b04 3104 3504 4004 3804 4200 2004 4404  K.1.5.@.8.B. .D.
+00014fc0: 3004 3904 3b08 0000 0000 0600 0000 0b53  0.9.;..........S
+00014fd0: 656c 6563 7420 6669 6c65 0700 0000 0954  elect file.....T
+00014fe0: 6178 5769 6467 6574 0103 0000 0028 041d  axWidget.....(..
+00014ff0: 0430 043b 043e 0433 043e 0432 044b 0439  .0.;.>.3.>.2.K.9
+00015000: 0020 043e 0442 0447 0451 0442 0020 043f  . .>.B.G.Q.B. .?
+00015010: 0443 0441 0442 0800 0000 0006 0000 0013  .C.A.B..........
+00015020: 5461 7820 7265 706f 7274 2069 7320 656d  Tax report is em
+00015030: 7074 7907 0000 0009 5461 7857 6964 6765  pty.....TaxWidge
+00015040: 7401 0300 0000 4004 1d04 3004 3b04 3e04  t.....@...0.;.>.
+00015050: 3304 3e04 3204 4b04 3900 2004 3e04 4204  3.>.2.K.9. .>.B.
+00015060: 4704 5104 4200 2004 4104 3e04 4504 4004  G.Q.B. .A.>.E.@.
+00015070: 3004 3d04 5104 3d00 2004 3200 2004 4404  0.=.Q.=. .2. .D.
+00015080: 3004 3904 3b00 2008 0000 0000 0600 0000  0.9.;. .........
+00015090: 1954 6178 2072 6570 6f72 7420 7361 7665  .Tax report save
+000150a0: 6420 746f 2066 696c 6520 0700 0000 0954  d to file .....T
+000150b0: 6178 5769 6467 6574 0103 0000 0040 041d  axWidget.....@..
+000150c0: 0430 043b 043e 0433 043e 0432 044b 0439  .0.;.>.3.>.2.K.9
+000150d0: 0020 043e 0442 0447 0451 0442 0020 0441  . .>.B.G.Q.B. .A
+000150e0: 043e 0445 0440 0430 043d 0451 043d 0020  .>.E.@.0.=.Q.=. 
+000150f0: 0432 0020 0444 0430 0439 043b 0020 0800  .2. .D.0.9.;. ..
+00015100: 0000 0006 0000 001d 5461 7820 7265 706f  ........Tax repo
+00015110: 7274 2077 6173 2073 6176 6564 2074 6f20  rt was saved to 
+00015120: 6669 6c65 2007 0000 0009 5461 7857 6964  file .....TaxWid
+00015130: 6765 7401 0300 0000 0c04 1d04 3004 3b04  get.........0.;.
+00015140: 3e04 3304 3808 0000 0000 0600 0000 0554  >.3.8..........T
+00015150: 6178 6573 0700 0000 0954 6178 5769 6467  axes.....TaxWidg
+00015160: 6574 0103 0000 004e 041e 0431 043d 043e  et.....N...1.=.>
+00015170: 0432 0438 0442 044c 0020 0442 043e 043b  .2.8.B.L. .B.>.;
+00015180: 044c 043a 043e 0020 0438 043d 0444 043e  .L.:.>. .8.=.D.>
+00015190: 0440 043c 0430 0446 0438 044e 0020 043e  .@.<.0.F.8.N. .>
+000151a0: 0020 0434 0438 0432 0438 0434 0435 043d  . .4.8.2.8.4.5.=
+000151b0: 0434 0430 0445 0800 0000 0006 0000 0027  .4.0.E.........'
+000151c0: 5570 6461 7465 206f 6e6c 7920 696e 666f  Update only info
+000151d0: 726d 6174 696f 6e20 6162 6f75 7420 6469  rmation about di
+000151e0: 7669 6465 6e64 7307 0000 0009 5461 7857  vidends.....TaxW
+000151f0: 6964 6765 7401 0300 0000 6404 1804 4104  idget.....d...A.
+00015200: 3f04 3e04 3b04 4c04 3704 3e04 3204 3004  ?.>.;.L.7.>.2.0.
+00015210: 4204 4c00 2004 3d04 3004 3704 3204 3004  B.L. .=.0.7.2.0.
+00015220: 3d04 3804 3500 2004 3104 4004 3e04 3a04  =.8.5. .1.@.>.:.
+00015230: 3504 4004 3000 2004 3a04 3004 3a00 2004  5.@.0. .:.0.:. .
+00015240: 3804 4104 4204 3e04 4704 3d04 3804 3a00  8.A.B.>.G.=.8.:.
+00015250: 2004 3204 4b04 3f04 3b04 3004 4204 4b08   .2.K.?.;.0.B.K.
+00015260: 0000 0000 0600 0000 2055 7365 2062 726f  ........ Use bro
+00015270: 6b65 7220 6e61 6d65 2061 7320 696e 636f  ker name as inco
+00015280: 6d65 2073 6f75 7263 6507 0000 0009 5461  me source.....Ta
+00015290: 7857 6964 6765 7401 0300 0000 0804 1304  xWidget.........
+000152a0: 3e04 3400 3a08 0000 0000 0600 0000 0559  >.4.:..........Y
+000152b0: 6561 723a 0700 0000 0954 6178 5769 6467  ear:.....TaxWidg
+000152c0: 6574 0103 0000 0050 0412 044b 0020 043d  et.....P...K. .=
+000152d0: 0435 0020 0432 044b 0431 0440 0430 043b  .5. .2.K.1.@.0.;
+000152e0: 0438 0020 0441 0447 0451 0442 0020 0434  .8. .A.G.Q.B. .4
+000152f0: 043b 044f 0020 043d 0430 043b 043e 0433  .;.O. .=.0.;.>.3
+00015300: 043e 0432 043e 0433 043e 0020 043e 0442  .>.2.>.3.>. .>.B
+00015310: 0447 0451 0442 0430 0800 0000 0006 0000  .G.Q.B.0........
+00015320: 002e 596f 7520 6861 7665 6e27 7420 7365  ..You haven't se
+00015330: 6c65 6374 6564 2061 6e20 6163 636f 756e  lected an accoun
+00015340: 7420 666f 7220 7461 7820 7265 706f 7274  t for tax report
+00015350: 0700 0000 0954 6178 5769 6467 6574 0103  .....TaxWidget..
+00015360: 0000 0098 041d 0435 0432 043e 0437 043c  .......5.2.>.7.<
+00015370: 043e 0436 043d 043e 0020 043e 0431 0440  .>.6.=.>. .>.1.@
+00015380: 0430 0431 043e 0442 0430 0442 044c 0020  .0.1.>.B.0.B.L. 
+00015390: 0441 0434 0435 043b 043a 0443 002c 0020  .A.4.5.;.:.C.,. 
+000153a0: 0442 002e 043a 002e 0020 043d 0435 0020  .B...:... .=.5. 
+000153b0: 0437 0430 0434 0430 043d 0020 0431 0430  .7.0.4.0.=. .1.0
+000153c0: 043d 043a 0020 0434 043b 044f 0020 0438  .=.:. .4.;.O. .8
+000153d0: 043d 0432 0435 0441 0442 0438 0446 0438  .=.2.5.A.B.8.F.8
+000153e0: 043e 043d 043d 043e 0433 043e 0020 0441  .>.=.=.>.3.>. .A
+000153f0: 0447 0451 0442 0430 003a 0020 0800 0000  .G.Q.B.0.:. ....
+00015400: 0006 0000 003e 4361 6e27 7420 7072 6f63  .....>Can't proc
+00015410: 6573 7320 7472 6164 6520 6173 2062 616e  ess trade as ban
+00015420: 6b20 6973 6e27 7420 7365 7420 666f 7220  k isn't set for 
+00015430: 696e 7665 7374 6d65 6e74 2061 6363 6f75  investment accou
+00015440: 6e74 3a20 0700 0000 0554 7261 6465 0103  nt: .....Trade..
+00015450: 0000 0002 2116 0800 0000 0006 0000 0001  ....!...........
+00015460: 2307 0000 000b 5472 6164 6557 6964 6765  #.....TradeWidge
+00015470: 7401 0300 0000 0804 2104 4704 3504 4208  t.......!.G.5.B.
+00015480: 0000 0000 0600 0000 0741 6363 6f75 6e74  .........Account
+00015490: 0700 0000 0b54 7261 6465 5769 6467 6574  .....TradeWidget
+000154a0: 0103 0000 0004 0426 0411 0800 0000 0006  .......&........
+000154b0: 0000 0005 4173 7365 7407 0000 000b 5472  ....Asset.....Tr
+000154c0: 6164 6557 6964 6765 7401 0300 0000 2204  adeWidget.....".
+000154d0: 1f04 3e04 3a04 4304 3f04 3a04 3000 2000  ..>.:.C.?.:.0. .
+000154e0: 2f00 2004 1f04 4004 3e04 3404 3004 3604  /. ...@.>.4.0.6.
+000154f0: 3008 0000 0000 0600 0000 0a42 7579 202f  0..........Buy /
+00015500: 2053 656c 6c07 0000 000b 5472 6164 6557   Sell.....TradeW
+00015510: 6964 6765 7401 0300 0000 1404 1404 3004  idget.........0.
+00015520: 4204 3000 2f04 1204 4004 3504 3c04 4f08  B.0./...@.5.<.O.
+00015530: 0000 0000 0600 0000 0944 6174 652f 5469  .........Date/Ti
+00015540: 6d65 0700 0000 0b54 7261 6465 5769 6467  me.....TradeWidg
+00015550: 6574 0103 0000 0010 041a 043e 043c 0438  et.........>.<.8
+00015560: 0441 0441 0438 044f 0800 0000 0006 0000  .A.A.8.O........
+00015570: 0003 4665 6507 0000 000b 5472 6164 6557  ..Fee.....TradeW
+00015580: 6964 6765 7401 0300 0000 1004 1e04 3f04  idget.........?.
+00015590: 3804 4104 3004 3d04 3804 3508 0000 0000  8.A.0.=.8.5.....
+000155a0: 0600 0000 044e 6f74 6507 0000 000b 5472  .....Note.....Tr
+000155b0: 6164 6557 6964 6765 7401 0300 0000 0804  adeWidget.......
+000155c0: 2604 3504 3d04 3008 0000 0000 0600 0000  &.5.=.0.........
+000155d0: 0550 7269 6365 0700 0000 0b54 7261 6465  .Price.....Trade
+000155e0: 5769 6467 6574 0103 0000 000c 041a 043e  Widget.........>
+000155f0: 043b 002d 0432 043e 0800 0000 0006 0000  .;.-.2.>........
+00015600: 0003 5174 7907 0000 000b 5472 6164 6557  ..Qty.....TradeW
+00015610: 6964 6765 7401 0300 0000 1a04 1404 3004  idget.........0.
+00015620: 4204 3000 2004 4004 3004 4104 4704 3504  B.0. .@.0.A.G.5.
+00015630: 4204 3e04 3208 0000 0000 0600 0000 0a53  B.>.2..........S
+00015640: 6574 746c 656d 656e 7407 0000 000b 5472  ettlement.....Tr
+00015650: 6164 6557 6964 6765 7401 0300 0000 7a04  adeWidget.....z.
+00015660: 1a04 3e04 3b04 3804 4704 3504 4104 4204  ..>.;.8.G.5.A.B.
+00015670: 3204 3e00 2004 3004 3a04 4204 3804 3204  2.>. .0.:.B.8.2.
+00015680: 3000 2004 3d04 3504 3404 3e04 4104 4204  0. .=.5.4.>.A.B.
+00015690: 3004 4204 3e04 4704 3d04 3e00 2004 3404  0.B.>.G.=.>. .4.
+000156a0: 3b04 4f00 2004 3e04 3104 4004 3004 3104  ;.O. .>.1.@.0.1.
+000156b0: 3e04 4204 3a04 3800 2004 3f04 3504 4004  >.B.:.8. .?.5.@.
+000156c0: 3504 3204 3e04 3404 3000 2e00 2004 1404  5.2.>.4.0... ...
+000156d0: 3004 4204 3000 3a00 2008 0000 0000 0600  0.B.0.:. .......
+000156e0: 0000 4041 7373 6574 2061 6d6f 756e 7420  ..@Asset amount 
+000156f0: 6973 206e 6f74 2065 6e6f 7567 6820 666f  is not enough fo
+00015700: 7220 6173 7365 7420 7472 616e 7366 6572  r asset transfer
+00015710: 2070 726f 6365 7373 696e 672e 2044 6174   processing. Dat
+00015720: 653a 2007 0000 0008 5472 616e 7366 6572  e: .....Transfer
+00015730: 0103 0000 0052 0421 043f 0438 0441 0430  .....R.!.?.8.A.0
+00015740: 043d 0438 0435 0020 0430 043a 0442 0438  .=.8.5. .0.:.B.8
+00015750: 0432 0430 0020 043d 0435 0020 043d 0430  .2.0. .=.5. .=.0
+00015760: 0439 0434 0435 043d 043e 0020 0434 043b  .9.4.5.=.>. .4.;
+00015770: 044f 0020 0442 0440 0430 043d 0441 0444  .O. .B.@.0.=.A.D
+00015780: 0435 0440 0430 002e 0800 0000 0006 0000  .5.@.0..........
+00015790: 0028 4173 7365 7420 7769 7468 6472 6177  .(Asset withdraw
+000157a0: 616c 206e 6f74 2066 6f75 6e64 2066 6f72  al not found for
+000157b0: 2074 7261 6e73 6665 722e 0700 0000 0854   transfer......T
+000157c0: 7261 6e73 6665 7201 0300 0000 2e04 1e04  ransfer.........
+000157d0: 4804 3804 3104 3a04 3000 2e00 2004 1a04  H.8.1.:.0... ...
+000157e0: 4304 4004 4100 2004 4004 3004 3204 3504  C.@.A. .@.0.2.5.
+000157f0: 3d00 2004 3d04 4304 3b04 4e08 0000 0000  =. .=.C.;.N.....
+00015800: 0600 0000 1045 7272 6f72 2e20 5a65 726f  .....Error. Zero
+00015810: 2072 6174 6507 0000 0008 5472 616e 7366   rate.....Transf
+00015820: 6572 0103 0000 0084 041e 0431 0440 0430  er.........1.@.0
+00015830: 0431 043e 0442 0430 043d 043d 043e 0435  .1.>.B.0.=.=.>.5
+00015840: 0020 043a 043e 043b 0438 0447 0435 0441  . .:.>.;.8.G.5.A
+00015850: 0442 0432 043e 0020 043c 0435 043d 044c  .B.2.>. .<.5.=.L
+00015860: 0448 0435 002c 0020 0447 0435 043c 0020  .H.5.,. .G.5.<. 
+00015870: 043a 043e 043b 0438 0447 0435 0441 0442  .:.>.;.8.G.5.A.B
+00015880: 0432 043e 0020 0432 0020 0442 0440 0430  .2.>. .2. .B.@.0
+00015890: 043d 0441 0444 0435 0440 0435 002e 0020  .=.A.D.5.@.5... 
+000158a0: 0414 0430 0442 0430 003a 0020 0800 0000  ...0.B.0.:. ....
+000158b0: 0006 0000 003b 5072 6f63 6573 7365 6420  .....;Processed 
+000158c0: 6173 7365 7420 616d 6f75 6e74 2069 7320  asset amount is 
+000158d0: 6c65 7373 2074 6861 6e20 7472 616e 7366  less than transf
+000158e0: 6572 2061 6d6f 756e 742e 2044 6174 653a  er amount. Date:
+000158f0: 2007 0000 0008 5472 616e 7366 6572 0103   .....Transfer..
+00015900: 0000 0002 2116 0800 0000 0006 0000 0001  ....!...........
+00015910: 2307 0000 000e 5472 616e 7366 6572 5769  #.....TransferWi
+00015920: 6467 6574 0103 0000 000a 0421 0443 043c  dget.......!.C.<
+00015930: 043c 0430 0800 0000 0006 0000 0006 416d  .<.0..........Am
+00015940: 6f75 6e74 0700 0000 0e54 7261 6e73 6665  ount.....Transfe
+00015950: 7257 6964 6765 7401 0300 0000 0404 2604  rWidget.......&.
+00015960: 1108 0000 0000 0600 0000 0541 7373 6574  ...........Asset
+00015970: 0700 0000 0e54 7261 6e73 6665 7257 6964  .....TransferWid
+00015980: 6765 7401 0300 0000 1404 1404 3004 4204  get.........0.B.
+00015990: 3000 2f04 1204 4004 3504 3c04 4f08 0000  0./...@.5.<.O...
+000159a0: 0000 0600 0000 0944 6174 652f 5469 6d65  .......Date/Time
+000159b0: 0700 0000 0e54 7261 6e73 6665 7257 6964  .....TransferWid
+000159c0: 6765 7401 0300 0000 1e04 2004 3004 3704  get....... .0.7.
+000159d0: 3c04 3504 4000 2004 3a04 3e04 3c04 3804  <.5.@. .:.>.<.8.
+000159e0: 4104 4104 3804 3808 0000 0000 0600 0000  A.A.8.8.........
+000159f0: 0a46 6565 2061 6d6f 756e 7407 0000 000e  .Fee amount.....
+00015a00: 5472 616e 7366 6572 5769 6467 6574 0103  TransferWidget..
+00015a10: 0000 0016 041a 043e 043c 043c 0438 0441  .......>.<.<.8.A
+00015a20: 0441 0438 044f 0020 0441 0800 0000 0006  .A.8.O. .A......
+00015a30: 0000 0008 4665 6520 6672 6f6d 0700 0000  ....Fee from....
+00015a40: 0e54 7261 6e73 6665 7257 6964 6765 7401  .TransferWidget.
+00015a50: 0300 0000 0204 2108 0000 0000 0600 0000  ......!.........
+00015a60: 0446 726f 6d07 0000 000e 5472 616e 7366  .From.....Transf
+00015a70: 6572 5769 6467 6574 0103 0000 0010 041e  erWidget........
+00015a80: 043f 0438 0441 0430 043d 0438 0435 0800  .?.8.A.0.=.8.5..
+00015a90: 0000 0006 0000 0004 4e6f 7465 0700 0000  ........Note....
+00015aa0: 0e54 7261 6e73 6665 7257 6964 6765 7401  .TransferWidget.
+00015ab0: 0300 0000 0404 1d04 3008 0000 0000 0600  ........0.......
+00015ac0: 0000 0254 6f07 0000 000e 5472 616e 7366  ...To.....Transf
+00015ad0: 6572 5769 6467 6574 0103 0000 000e 041f  erWidget........
+00015ae0: 0435 0440 0435 0432 043e 0434 0800 0000  .5.@.5.2.>.4....
+00015af0: 0006 0000 0008 5472 616e 7366 6572 0700  ......Transfer..
+00015b00: 0000 0e54 7261 6e73 6665 7257 6964 6765  ...TransferWidge
+00015b10: 7401 0300 0000 0404 1f04 3e08 0000 0000  t.........>.....
+00015b20: 0600 0000 0845 6e64 2064 6174 6507 0000  .....End date...
+00015b30: 000f 5570 6461 7465 5175 6f74 6573 446c  ..UpdateQuotesDl
+00015b40: 6701 0300 0000 1204 1804 4104 4204 3e04  g.........A.B.>.
+00015b50: 4704 3d04 3804 3a04 3808 0000 0000 0600  G.=.8.:.8.......
+00015b60: 0000 0753 6f75 7263 6573 0700 0000 0f55  ...Sources.....U
+00015b70: 7064 6174 6551 756f 7465 7344 6c67 0103  pdateQuotesDlg..
+00015b80: 0000 0002 0421 0800 0000 0006 0000 000a  .....!..........
+00015b90: 5374 6172 7420 6461 7465 0700 0000 0f55  Start date.....U
+00015ba0: 7064 6174 6551 756f 7465 7344 6c67 0103  pdateQuotesDlg..
+00015bb0: 0000 0028 041e 0431 043d 043e 0432 043b  ...(...1.=.>.2.;
+00015bc0: 0435 043d 0438 0435 0020 043a 043e 0442  .5.=.8.5. .:.>.B
+00015bd0: 0438 0440 043e 0432 043e 043a 0800 0000  .8.@.>.2.>.:....
+00015be0: 0006 0000 0015 5570 6461 7465 2061 7373  ......Update ass
+00015bf0: 6574 2773 2071 756f 7465 7307 0000 000f  et's quotes.....
+00015c00: 5570 6461 7465 5175 6f74 6573 446c 6701  UpdateQuotesDlg.
+00015c10: 0300 0000 1400 6400 6400 2f00 4d00 4d00  ......d.d./.M.M.
+00015c20: 2f00 7900 7900 7900 7908 0000 0000 0600  /.y.y.y.y.......
+00015c30: 0000 0a64 642f 4d4d 2f79 7979 7907 0000  ...dd/MM/yyyy...
+00015c40: 000f 5570 6461 7465 5175 6f74 6573 446c  ..UpdateQuotesDl
+00015c50: 6701 0300 0000 5804 1d04 3504 3204 3e04  g.....X...5.2.>.
+00015c60: 3704 3c04 3e04 3604 3d04 3e00 2004 3f04  7.<.>.6.=.>. .?.
+00015c70: 4004 3e04 4704 3804 4204 3004 4204 4c00  @.>.G.8.B.0.B.L.
+00015c80: 2004 4804 3004 3104 3b04 3e04 3d00 2004   .H.0.1.;.>.=. .
+00015c90: 3e04 4204 4704 5104 4204 3000 2004 3804  >.B.G.Q.B.0. .8.
+00015ca0: 3700 2004 4404 3004 3904 3b04 3000 2008  7. .D.0.9.;.0. .
+00015cb0: 0000 0000 0600 0000 2543 616e 2774 206c  ........%Can't l
+00015cc0: 6f61 6420 7265 706f 7274 2074 656d 706c  oad report templ
+00015cd0: 6174 6520 6672 6f6d 2066 696c 6520 0700  ate from file ..
+00015ce0: 0000 0458 4c53 5801 0300 0000 4404 1d04  ...XLSX.....D...
+00015cf0: 3504 3204 3e04 3704 3c04 3e04 3604 3d04  5.2.>.7.<.>.6.=.
+00015d00: 3e00 2004 4104 3e04 4504 4004 3004 3d04  >. .A.>.E.@.0.=.
+00015d10: 3804 4204 4c00 2004 3e04 4204 4704 5104  8.B.L. .>.B.G.Q.
+00015d20: 4200 2004 3200 2004 4404 3004 3904 3b00  B. .2. .D.0.9.;.
+00015d30: 2008 0000 0000 0600 0000 1c43 616e 2774   ..........Can't
+00015d40: 2073 6176 6520 7265 706f 7274 2069 6e74   save report int
+00015d50: 6f20 6669 6c65 2007 0000 0004 584c 5358  o file .....XLSX
+00015d60: 0103 0000 0044 041d 0435 0020 0443 043a  .....D...5. .C.:
+00015d70: 0430 0437 0430 043d 0020 0444 043e 0440  .0.7.0.=. .D.>.@
+00015d80: 043c 0430 0442 0020 0434 043b 044f 0020  .<.0.B. .4.;.O. 
+00015d90: 043f 043e 043b 044f 0020 043e 0442 0447  .?.>.;.O. .>.B.G
+00015da0: 0451 0442 0430 003a 0020 0800 0000 0006  .Q.B.0.:. ......
+00015db0: 0000 0024 466f 726d 6174 2069 7320 6d69  ...$Format is mi
+00015dc0: 7373 696e 6720 666f 7220 7265 706f 7274  ssing for report
+00015dd0: 2066 6965 6c64 3a20 0700 0000 0458 4c53   field: .....XLS
+00015de0: 5801 0300 0000 4204 1d04 3500 2004 3704  X.....B...5. .7.
+00015df0: 3004 3404 3004 3d00 2004 4804 3004 3104  0.4.0.=. .H.0.1.
+00015e00: 3b04 3e04 3d00 2004 3404 3b04 4f00 2004  ;.>.=. .4.;.O. .
+00015e10: 3404 3004 3d04 3d04 4b04 4500 2004 3e04  4.0.=.=.K.E. .>.
+00015e20: 4204 4704 5104 4204 3008 0000 0000 0600  B.G.Q.B.0.......
+00015e30: 0000 1a4e 6f20 7265 706f 7274 2072 6f77  ...No report row
+00015e40: 2074 656d 706c 6174 6520 7365 7407 0000   template set...
+00015e50: 0004 584c 5358 0103 0000 003a 0428 0430  ..XLSX.....:.(.0
+00015e60: 0431 043b 043e 043d 0020 0434 043b 044f  .1.;.>.=. .4.;.O
+00015e70: 0020 0434 0430 043d 043d 044b 0445 0020  . .4.0.=.=.K.E. 
+00015e80: 043d 0435 0020 043d 0430 0439 0434 0435  .=.5. .=.0.9.4.5
+00015e90: 043d 003a 0020 0800 0000 0006 0000 001f  .=.:. ..........
+00015ea0: 5265 706f 7274 2072 6f77 2074 656d 706c  Report row templ
+00015eb0: 6174 6520 6e6f 7420 666f 756e 643a 2007  ate not found: .
+00015ec0: 0000 0004 584c 5358 0103 0000 0046 041d  ....XLSX.....F..
+00015ed0: 0435 0438 0437 0432 0435 0441 0442 043d  .5.8.7.2.5.A.B.=
+00015ee0: 0430 044f 0020 0441 0442 0440 043e 043a  .0.O. .A.B.@.>.:
+00015ef0: 0430 0020 0444 043e 0440 043c 0430 0442  .0. .D.>.@.<.0.B
+00015f00: 0438 0440 043e 0432 0430 043d 0438 044f  .8.@.>.2.0.=.8.O
+00015f10: 003a 0020 0800 0000 0006 0000 001c 556e  .:. ..........Un
+00015f20: 7265 636f 676e 697a 6564 2066 6f72 6d61  recognized forma
+00015f30: 7420 7374 7269 6e67 3a20 0700 0000 0458  t string: .....X
+00015f40: 4c53 5801 8800 0000 0d11 01fd 290b ff14  LSX.........)...
+00015f50: 0204 fd2c 0a13                           ...,..
```

### Comparing `jal-2023.4.8/jal/net/downloader.py` & `jal-2023.5.1/jal/net/downloader.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/net/helpers.py` & `jal-2023.5.1/jal/net/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/pypi_description.md` & `jal-2023.5.1/jal/pypi_description.md`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/reports/category.py` & `jal-2023.5.1/jal/reports/category.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/reports/deals.py` & `jal-2023.5.1/jal/widgets/delegates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,330 +1,334 @@
-from __future__ import annotations
-
-from decimal import Decimal
-from PySide6.QtCore import Qt, Slot, QObject, QAbstractItemModel, QModelIndex
-from jal.ui.reports.ui_deals_report import Ui_DealsReportWidget
-from jal.reports.reports import Reports
+from datetime import datetime
+from decimal import Decimal, InvalidOperation
+from PySide6.QtWidgets import QWidget, QStyledItemDelegate, QLineEdit, QDateTimeEdit, QTreeView
+from PySide6.QtCore import Qt, QModelIndex, QEvent, QLocale, QDateTime, QDate, QTime, QTimeZone
+from PySide6.QtGui import QDoubleValidator, QBrush, QKeyEvent
+from jal.constants import CustomColor
+from jal.widgets.reference_selector import AssetSelector, PeerSelector, CategorySelector, TagSelector
+from jal.db.db import JalModel
+from jal.db.helpers import localize_decimal, delocalize_decimal
 from jal.db.account import JalAccount
-from jal.db.operations import LedgerTransaction
-from jal.widgets.helpers import ts2d
-from jal.widgets.delegates import TimestampDelegate, FloatDelegate
-from jal.widgets.mdi import MdiWidget
-from jal.widgets.delegates import GridLinesDelegate
 
-JAL_REPORT_CLASS = "DealsReport"
+
+# ----------------------------------------------------------------------------------------------------------------------
+# Base class to provide different delegates for WidgetDataMappers in operations widgets
+# Separate delegate class is subclassed for every operation widget with own definition of self.delegates for columns
+class WidgetMapperDelegateBase(QStyledItemDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+
+        self.timestamp_delegate = TimestampDelegate()
+        self.decimal_delegate = FloatDelegate(2)
+        self.symbol_delegate = SymbolDelegate()
+        self.default = QStyledItemDelegate()
+
+        self.delegates = {}
+
+    def get_delegate(self, index):
+        column_name = index.model().record().fieldName(index.column())
+        try:
+            delegate = self.delegates[column_name]
+        except KeyError:
+            delegate = self.default
+        return delegate
+
+    def paint(self, painter, option, index):
+        delegate = self.get_delegate(index)
+        delegate.paint(painter, option, index)
+
+    def createEditor(self, aParent, option, index):
+        delegate = self.get_delegate(index)
+        delegate.createEditor(aParent, option, index)
+
+    def setEditorData(self, editor, index):
+        delegate = self.get_delegate(index)
+        delegate.setEditorData(editor, index)
+
+    def setModelData(self, editor, model, index):
+        delegate = self.get_delegate(index)
+        delegate.setModelData(editor, model, index)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-# Class to group trades and display them in TreeView
-class TradeTreeItem:
-    def __init__(self, trade, parent=None, group=''):
-        self._parent = parent
-        self._trade = trade
-        self._children = []
-        self._group = group
-        if trade is None:
-            self._data = {
-                'symbol': '',
-                'open_ts': 0, 'open_date': '', 'close_ts': 0, 'close_date': '',
-                'open_price': Decimal('0'), 'close_price': Decimal('0'),
-                'qty': Decimal('0'), 'fee': Decimal('0'), 'p/l': Decimal('0'), 'p/l%': Decimal('0'),
-                'note': ''
-            }
-        else:
-            self._data = {
-                'symbol': self._trade.symbol(),
-                'open_ts': self._trade.open_operation().timestamp(),
-                'open_date': ts2d(self._trade.open_operation().timestamp()),
-                'close_ts': self._trade.close_operation().timestamp(),
-                'close_date': ts2d(self._trade.close_operation().timestamp()),
-                'open_price': self._trade.open_price(),
-                'close_price': self._trade.close_price(),
-                'qty': self._trade.qty(),
-                'fee': self._trade.fee(),
-                'p/l': self._trade.profit(),
-                'p/l%': self._trade.profit(percent=True),
-                'note': ''
-            }
-            if self._trade.open_operation().type() == LedgerTransaction.CorporateAction:
-                self._data['note'] += self._trade.open_operation().name() + " ▶"
-            if self._trade.close_operation().type() == LedgerTransaction.CorporateAction:
-                self._data['note'] += "▶ " + self._trade.close_operation().name()
+# Custom DateTimeEdit that is able to reset value to None
+# i.e. it handles keypress '-', sets timestamp to 0 that effectively cleans the field
+class DateTimeEditWithReset(QDateTimeEdit):
+    def __init__(self, parent):
+        super().__init__(parent)
+
+    def keyPressEvent(self, event: QKeyEvent) -> None:
+        if event.key() == Qt.Key_Minus:
+            self.setDateTime(QDateTime(QDate(1970, 1, 1), QTime(0, 0, 0), Qt.UTC))  # = 0 timestamp
+        super().keyPressEvent(event)
 
-    def setParent(self, parent):
+
+# ----------------------------------------------------------------------------------------------------------------------
+# Delegate to convert timestamp from unix-time to QDateTime and display it according to the given format
+class TimestampDelegate(QStyledItemDelegate):
+    def __init__(self, display_format='%d/%m/%Y %H:%M:%S', parent=None):
+        super().__init__(parent=parent)
         self._parent = parent
+        self._format = display_format
 
-    def getParent(self):
-        return self._parent
+    def displayText(self, value, locale):
+        if isinstance(value, str):  # int value comes here in form of string in case of SQL aggregate function results
+            value = int(value)
+        text = datetime.utcfromtimestamp(value).strftime(self._format) if value else ''
+        return text
+
+    def createEditor(self, aParent, option, index):
+        editor = DateTimeEditWithReset(aParent)
+        editor.setTimeSpec(Qt.UTC)
+        if 'H' in self._format:  # we have hours and need DataTime editor to edit it
+            editor.setDisplayFormat("dd/MM/yyyy hh:mm:ss")
+        else:
+            editor.setDisplayFormat("dd/MM/yyyy")
+        return editor
 
-    def appendChild(self, child):
-        child.setParent(self)
-        self._children.append(child)
-        if self._group:
-            self.updateGroupDetails(child.details())
-
-    def updateGroupDetails(self, child_data):
-        self._data['symbol'] = child_data['symbol']
-        if self._data['open_ts'] == 0 or self._data['open_ts'] > child_data['open_ts']:
-            self._data['open_ts'] = child_data['open_ts']
-        if self._data['close_ts'] < child_data['close_ts']:
-            self._data['close_ts'] = child_data['close_ts']
-        self._data['open_price'] = (self._data['open_price'] * self._data['qty'] + child_data['open_price'] *
-                                    child_data['qty']) / (self._data['qty'] + child_data['qty'])
-        self._data['close_price'] = (self._data['close_price'] * self._data['qty'] + child_data['close_price'] *
-                                     child_data['qty']) / (self._data['qty'] + child_data['qty'])
-        self._data['qty'] += child_data['qty']
-        self._data['fee'] += child_data['fee']
-        self._data['p/l'] += child_data['p/l']
-        self._data['p/l%'] = Decimal('100') * self._data['p/l'] / (self._data['open_price'] * self._data['qty'])
-        if self._parent is not None:
-            self._parent.updateGroupDetails(child_data)
-
-    def getChild(self, id):
-        if id < 0 or id > len(self._children):
-            return None
-        return self._children[id]
-
-    def childrenCount(self):
-        return len(self._children)
-
-    def details(self):
-        return self._data
-
-    def isGroup(self):
-        return self._group != ''
-
-    # assigns group value if this tree item is a group item
-    def setGroupValue(self, value):
-        if self._group:
-            self._data[self._group] = value
-
-    # returns (group_field_name, group_value) if item is a group item, otherwise returns None
-    def getGroup(self):
-        if self._group:
-            return self._group, self._data[self._group]
+    def setEditorData(self, editor, index):
+        timestamp = index.model().data(index, Qt.EditRole)
+        if timestamp == '':
+            QStyledItemDelegate.setEditorData(self, editor, index)
         else:
-            return None
+            editor.setDateTime(QDateTime.fromSecsSinceEpoch(timestamp, QTimeZone(0)))
+
+    def setModelData(self, editor, model, index):
+        timestamp = editor.dateTime().toSecsSinceEpoch()
+        model.setData(index, timestamp)
+
+    def paint(self, painter, option, index):
+        super().paint(painter, option, index)
+        if type(self._parent) == QTreeView:    # Extra code for tree views - to draw grid lines
+            painter.save()
+            pen = painter.pen()
+            pen.setWidth(1)
+            pen.setStyle(Qt.DotLine)
+            pen.setColor(Qt.GlobalColor.lightGray)
+            painter.setPen(pen)
+            painter.drawRect(option.rect)
+            painter.restore()
+
+
+# -----------------------------------------------------------------------------------------------------------------------
+# Delegate for float numbers formatting
+# By default has 6 decimal places that may be controlled with 'tolerance' parameter
+# 'allow_tail' - display more digits for numbers that have more digits than 'tolerance'
+#                and only 'tolerance' digits otherwise
+# 'colors' - make Green/Red background for positive/negative values
+# 'percent' - multiply values by 100 in order to display percents
+# 'empty_zero' - display nothing instead of number 0
+class FloatDelegate(QStyledItemDelegate):
+    DEFAULT_TOLERANCE = 6
 
-    # returns an element of tree that will provide right group parent for 'item' with given 'group_fields'
-    def getGroupLeaf(self, group_fields: list, item: TradeTreeItem) -> TradeTreeItem:
-        if group_fields:
-            group_item = None
-            group_name = group_fields[0]
-            for child in self._children:
-                if child.details()[group_name] == item.details()[group_name]:
-                    group_item = child
-            if group_item is None:
-                group_item = TradeTreeItem(None, parent=self, group=group_name)
-                group_item.setGroupValue(item.details()[group_name])
-                self._children.append(group_item)
-            return group_item.getGroupLeaf(group_fields[1:], item)
+    def __init__(self, tolerance=None, allow_tail=True, colors=False, percent=False, empty_zero=False, parent=None):
+        self._parent = parent
+        super().__init__(parent=parent)
+        try:
+            self._tolerance = int(tolerance)
+        except (ValueError, TypeError):
+            self._tolerance = self.DEFAULT_TOLERANCE
+        self._allow_tail = allow_tail
+        self._colors = colors
+        self._color = None
+        self._percent = percent
+        self._empty_zero = empty_zero
+        self._validator = QDoubleValidator()
+        self._validator.setLocale(QLocale().system())
+
+    def displayText(self, value, locale):
+        try:
+            amount = Decimal(value)
+        except ValueError:
+            amount = Decimal('0')
+        amount = Decimal('0') if amount.is_nan() else amount  # Protection against occasional NaNs in database
+        if self._percent:
+            amount *= Decimal('100')
+        if amount > Decimal('0'):
+            self._color = CustomColor.LightGreen
+        elif amount < Decimal('0'):
+            self._color = CustomColor.LightRed
         else:
-            return self
+            self._color = None
+            if self._empty_zero:
+                return ''
+        decimal_places = -amount.normalize().as_tuple().exponent
+        decimal_places = decimal_places if self._allow_tail and (decimal_places > self._tolerance) else self._tolerance
+        return QLocale().toString(float(amount), 'f', decimal_places)
+
+    # this is required when edit operation is called from QTableView
+    def createEditor(self, aParent, option, index):
+        float_editor = QLineEdit(aParent)
+        float_editor.setValidator(self._validator)
+        return float_editor
+
+    def setEditorData(self, editor, index):
+        try:
+            amount = Decimal(index.model().data(index, Qt.EditRole))
+        except (InvalidOperation, TypeError):   # Set to zero if we have None in database
+            amount = Decimal('0')
+        editor.setText(localize_decimal(amount, self._tolerance, self._percent))
+
+    def setModelData(self, editor, model, index):
+        number_text = delocalize_decimal(editor.text())
+        value = Decimal(number_text) if number_text else Decimal('0')
+        if self._percent:
+            value /= Decimal('100')
+        model.setData(index, str(value))
+
+    def initStyleOption(self, option, index):
+        super().initStyleOption(option, index)
+        option.displayAlignment = Qt.AlignRight
+        if self._colors and self._color is not None:
+            option.backgroundBrush = QBrush(self._color)
+
+    def paint(self, painter, option, index):
+        super().paint(painter, option, index)
+        if type(self._parent) == QTreeView:  # Extra code for tree views - to draw grid lines
+            painter.save()
+            pen = painter.pen()
+            pen.setWidth(1)
+            pen.setStyle(Qt.DotLine)
+            pen.setColor(Qt.GlobalColor.lightGray)
+            painter.setPen(pen)
+            painter.drawRect(option.rect)
+            painter.restore()
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class ClosedTradesModel(QAbstractItemModel):
-    def __init__(self, parent_view):
-        super().__init__(parent_view)
-        self._view = parent_view
-        self._root = None
-        self._trades = []
-        self._account_id = 0
-        self._begin = self._end = 0
-        self._groups = []
-        self._grid_delegate = None
-        self._float_delegate = None
-        self._float2_delegate = None
-        self._float4_delegate = None
-        self._timestamp_delegate = None
-        self._profit_delegate = None
-        self._columns = [
-            {'name': self.tr("Asset"), 'field': 'symbol'},
-            {'name': self.tr("Open Date/Time"), 'field': 'open_ts'},
-            {'name': self.tr("Open Date"), 'field': 'open_date'},
-            {'name': self.tr("Close Date/Time"), 'field': 'close_ts'},
-            {'name': self.tr("Close Date"), 'field': 'close_date'},
-            {'name': self.tr("Open Price"), 'field': 'open_price'},
-            {'name': self.tr("Close Price"), 'field': 'close_price'},
-            {'name': self.tr("Qty"), 'field': 'qty'},
-            {'name': self.tr("Fee"), 'field': 'fee'},
-            {'name': self.tr("P/L"), 'field': 'p/l'},
-            {'name': self.tr("P/L, %"), 'field': 'p/l%'},
-            {'name': self.tr("Note"), 'field': 'note'}
-        ]
-
-    def fieldIndex(self, field_name: str) -> int:
-        for i, column in enumerate(self._columns):
-            if column['field'] == field_name:
-                return i
-        return -1
-
-    def rowCount(self, parent=None):
-        if not parent.isValid():
-            parent_item = self._root
-        else:
-            parent_item = parent.internalPointer()
-        if parent_item is not None:
-            return parent_item.childrenCount()
-        else:
-            return 0
+# Delegate to apply currency filter for AssetSelector widgets based on current account
+class SymbolDelegate(QStyledItemDelegate):
+    def setEditorData(self, editor, index):
+        account_currency = JalAccount(index.model().data(index.sibling(index.row(),
+                                                                       index.model().fieldIndex('account_id')),
+                                                         Qt.EditRole)).currency()
+        editor.setFilterValue(account_currency)
+        QStyledItemDelegate.setEditorData(self, editor, index)
 
-    def columnCount(self, parent=None):
-        if parent is None:
-            parent_item = self._root
-        elif not parent.isValid():
-            parent_item = self._root
-        else:
-            parent_item = parent.internalPointer()
-        if parent_item is not None:
-            return len(self._columns)
-        else:
-            return 0
 
-    def index(self, row, column, parent=None):
-        if not parent.isValid():
-            parent = self._root
+# ----------------------------------------------------------------------------------------------------------------------
+# Display '*' if true and empty cell if false
+# Toggle True/False by mouse click
+class BoolDelegate(QStyledItemDelegate):
+    def __init__(self, parent=None):
+        self._parent = parent
+        super().__init__(parent=parent)
+
+    def displayText(self, value, locale):
+        if value:
+            return ' ☒ '
         else:
-            parent = parent.internalPointer()
-        child = parent.getChild(row)
-        if child:
-            return self.createIndex(row, column, child)
-        return QModelIndex()
-
-    def parent(self, index=None):
-        if not index.isValid():
-            return QModelIndex()
-        child_item = index.internalPointer()
-        parent_item = child_item.getParent()
-        if parent_item == self._root:
-            return QModelIndex()
-        return self.createIndex(0, 0, parent_item)
-
-    def headerData(self, section, orientation, role=Qt.DisplayRole):
-        if orientation == Qt.Horizontal:
-            if role == Qt.DisplayRole:
-                return self._columns[section]['name']
-            if role == Qt.TextAlignmentRole:
-                return int(Qt.AlignCenter)
-        return None
-
-    def data(self, index, role=Qt.DisplayRole):
-        if not index.isValid():
-            return None
-        item = index.internalPointer()
-        if role == Qt.DisplayRole:
-            if item.isGroup():
-                field = self._columns[index.column()]['field']
-                if field == 'symbol':
-                    group, value = item.getGroup()
-                    display_name = [x['name'] for x in self._columns if x['field']==group][0]
-                    return f"{display_name}: {value}"
-                if field == 'open_ts' or field == 'close_ts':
-                    return 0
-            return item.details()[self._columns[index.column()]['field']]
-        return None
-
-    def setAccount(self, account_id):
-        self._account_id = account_id
-        self.prepareData()
-        self.configureView()
-
-    def prepareData(self):
-        self._trades = JalAccount(self._account_id).closed_trades_list()
-        self._trades = [x for x in self._trades if self._begin <= x.close_operation().timestamp() <= self._end]
-        self._root = TradeTreeItem(None)
-        for trade in self._trades:
-            new_item = TradeTreeItem(trade)
-            leaf = self._root.getGroupLeaf(self._groups, new_item)
-            leaf.appendChild(new_item)
-        self.modelReset.emit()
-        self._view.expandAll()
-
-    def configureView(self):
-        self._view.setSortingEnabled(True)
-        for column in range(self.columnCount()):
-            if column == 0:
-                self._view.setColumnWidth(column, 300)
+            return ' ☐ '
+
+    def initStyleOption(self, option, index):
+        super().initStyleOption(option, index)
+        option.displayAlignment = Qt.AlignCenter
+
+    def paint(self, painter, option, index):
+        super().paint(painter, option, index)
+        if type(self._parent) == QTreeView:  # Extra code for tree views - to draw grid lines
+            painter.save()
+            pen = painter.pen()
+            pen.setWidth(1)
+            pen.setStyle(Qt.DotLine)
+            pen.setColor(Qt.GlobalColor.lightGray)
+            painter.setPen(pen)
+            painter.drawRect(option.rect)
+            painter.restore()
+
+    def editorEvent(self, event, model, option, index):
+        if event.type() == QEvent.MouseButtonPress:
+            if model.data(index, Qt.DisplayRole):  # Toggle value - from 1 to 0 and from 0 to 1
+                model.setData(index, 0)
             else:
-                self._view.setColumnWidth(column, 100)
-        font = self._view.header().font()
-        font.setBold(True)
-        self._view.header().setFont(font)
-        self._view.setColumnHidden(self.fieldIndex('open_date'), True)
-        self._view.setColumnHidden(self.fieldIndex('close_date'), True)
-        self._view.setColumnWidth(self.fieldIndex('open_ts'), self._view.fontMetrics().horizontalAdvance("00/00/0000 00:00:00") * 1.1)
-        self._view.setColumnWidth(self.fieldIndex('close_ts'), self._view.fontMetrics().horizontalAdvance("00/00/0000 00:00:00") * 1.1)
-        self._grid_delegate = GridLinesDelegate(self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex('symbol'), self._grid_delegate)
-        self._view.setItemDelegateForColumn(self.fieldIndex('note'), self._grid_delegate)
-        self._timestamp_delegate = TimestampDelegate(parent=self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex('open_ts'), self._timestamp_delegate)
-        self._view.setItemDelegateForColumn(self.fieldIndex('close_ts'), self._timestamp_delegate)
-        self._float_delegate = FloatDelegate(0, allow_tail=True, parent=self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex("qty"), self._float_delegate)
-        self._float2_delegate = FloatDelegate(2, allow_tail=False, parent=self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex("fee"), self._float2_delegate)
-        self._float4_delegate = FloatDelegate(4, allow_tail=False, parent=self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex('open_price'), self._float4_delegate)
-        self._view.setItemDelegateForColumn(self.fieldIndex('close_price'), self._float4_delegate)
-        self._profit_delegate = FloatDelegate(2, allow_tail=False, colors=True, parent=self._view)
-        self._view.setItemDelegateForColumn(self.fieldIndex("p/l"), self._profit_delegate)
-        self._view.setItemDelegateForColumn(self.fieldIndex("p/l%"), self._profit_delegate)
-
-    def setDatesRange(self, begin, end):
-        self._begin = begin
-        self._end = end
-        self.prepareData()
-        self.configureView()
-
-    # defines report grouping by provided field list - 'group_field1;group_field2;...'
-    def setGrouping(self, group_list):
-        if group_list:
-            self._groups = group_list.split(';')
-        else:
-            self._groups = []
-        self.prepareData()
-        self.configureView()
+                model.setData(index, 1)
+        return True
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-class DealsReport(QObject):
-    def __init__(self):
-        super().__init__()
-        self.name = self.name = self.tr("Deals by Account")
-        self.window_class = "DealsReportWindow"
+# QTreeView doesn't draw grid lines and have no normal method to implement it
+# So the purpose of this delegate is solely to draw dotted box around report cell
+class GridLinesDelegate(QStyledItemDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+
+    def paint(self, painter, option, index):
+        painter.save()
+        pen = painter.pen()
+        pen.setWidth(1)
+        pen.setStyle(Qt.DotLine)
+        pen.setColor(Qt.GlobalColor.lightGray)
+        painter.setPen(pen)
+        painter.drawRect(option.rect)
+        painter.restore()
+        super().paint(painter, option, index)
+
+
+# -----------------------------------------------------------------------------------------------------------------------
+# Base class for lookup delegate that allows Asset, Peer, Category and Tag selection
+class LookupSelectorDelegate(QStyledItemDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._table = ''
+        self._field = ''
+        self._selector = None
+
+    def displayText(self, value, locale):
+        item_name = JalModel(self, self._table).get_value(self._field, "id", value)
+        if item_name is None:
+            return ''
+        else:
+            return item_name
 
+    def createSelector(self, parent) -> None:
+        raise NotImplementedError("Method createSelector() isn't defined")
 
-# ----------------------------------------------------------------------------------------------------------------------
-class DealsReportWindow(MdiWidget):
-    def __init__(self, parent: Reports, settings: dict = None):
-        super().__init__(parent.mdi_area())
-        self.ui = Ui_DealsReportWidget()
-        self.ui.setupUi(self)
-        self._parent = parent
+    def createEditor(self, aParent, option, index):
+        self.createSelector(aParent)
+        assert self._selector is not None, "Selector isn't created in LookupSelectorDelegate descendant"
+        return self._selector
+
+    def setEditorData(self, editor: QWidget, index: QModelIndex) -> None:
+        editor.selected_id = index.data()
+
+    def setModelData(self, editor, model, index):
+        model.setData(index, editor.selected_id)
+
+
+class CategorySelectorDelegate(LookupSelectorDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._table = "categories"
+        self._field = "name"
+
+    def createSelector(self, parent) -> None:
+        self._selector = CategorySelector(parent)
+
+
+class TagSelectorDelegate(LookupSelectorDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._table = "tags"
+        self._field = "tag"
+
+    def createSelector(self, parent) -> None:
+        self._selector = TagSelector(parent)
+
+
+class PeerSelectorDelegate(LookupSelectorDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._table = "agents"
+        self._field = "name"
+
+    def createSelector(self, parent) -> None:
+        self._selector = PeerSelector(parent)
+
+
+class AssetSelectorDelegate(LookupSelectorDelegate):
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+        self._table = "assets_ext"
+        self._field = "symbol"
 
-        # Add available groupings
-        self.ui.GroupCombo.addItem(self.tr("<None>"), "")
-        self.ui.GroupCombo.addItem(self.tr("Asset"), "symbol")
-        self.ui.GroupCombo.addItem(self.tr("Close"), "close_date")
-        self.ui.GroupCombo.addItem(self.tr("Asset - Open - Close"), "symbol;open_date;close_date")
-        self.ui.GroupCombo.addItem(self.tr("Open - Close"), "open_date;close_date")
-        self.ui.GroupCombo.addItem(self.tr("Close - Open"), "close_date;open_date")
-
-        self.trades_model = ClosedTradesModel(self.ui.ReportTreeView)
-        self.ui.ReportTreeView.setModel(self.trades_model)
-
-        self.connect_signals_and_slots()
-
-    def connect_signals_and_slots(self):
-        self.ui.ReportAccountBtn.changed.connect(self.onAccountChange)
-        self.ui.ReportRange.changed.connect(self.ui.ReportTreeView.model().setDatesRange)
-        self.ui.GroupCombo.currentIndexChanged.connect(self.onGroupingChange)
-
-    @Slot()
-    def onAccountChange(self):
-        self.ui.ReportTreeView.model().setAccount(self.ui.ReportAccountBtn.account_id)
-
-    @Slot()
-    def onGroupingChange(self, idx):
-        self.ui.ReportTreeView.model().setGrouping(self.ui.GroupCombo.itemData(idx))
+    def createSelector(self, parent) -> None:
+        self._selector = AssetSelector(parent)
```

### Comparing `jal-2023.4.8/jal/reports/income_spending.py` & `jal-2023.5.1/jal/reports/income_spending.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/reports/peer.py` & `jal-2023.5.1/jal/reports/peer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/reports/profit_loss.py` & `jal-2023.5.1/jal/reports/profit_loss.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/reports/reports.py` & `jal-2023.5.1/jal/reports/reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import importlib
 
 from PySide6.QtWidgets import QFileDialog
 from PySide6.QtCore import QObject
 from jal.constants import Setup
 from jal.db.helpers import get_app_path
+from jal.db.settings import JalSettings, FolderFor
 from jal.data_export.xlsx import XLSX
 
 
 class Reports(QObject):
     def __init__(self, parent, MdiArea):
         super().__init__()
         self.parent = parent
@@ -60,18 +61,20 @@
         module = report_loader['module']
         class_instance = getattr(module, report_loader['window_class'])
         report = class_instance(self, settings)
         self._mdi.addSubWindow(report, maximized=maximized)
 
     # Save report content from the model to xls-file chosen by the user
     def save_report(self, name, model):
+        folder = JalSettings().getRecentFolder(FolderFor.Report, '.')
         filename, filter = QFileDialog.getSaveFileName(self._mdi, self.tr("Save report to:"),
-                                                       ".", self.tr("Excel files (*.xlsx)"))
+                                                       folder, self.tr("Excel files (*.xlsx)"))
         if filename:
             if filter == self.tr("Excel files (*.xlsx)") and filename[-5:] != '.xlsx':
                 filename = filename + '.xlsx'
         else:
             return
+        JalSettings().setRecentFolder(FolderFor.Report, filename)
         report = XLSX(filename)
         report.output_model(name, model)
         report.save()
         logging.info(self.tr("Report was saved to file ") + f"'{filename}'")
```

### Comparing `jal-2023.4.8/jal/reports/tag.py` & `jal-2023.5.1/jal/reports/tag.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_category_report.py` & `jal-2023.5.1/jal/ui/reports/ui_category_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_deals_report.py` & `jal-2023.5.1/jal/ui/reports/ui_deals_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
 from PySide6.QtWidgets import (QAbstractItemView, QApplication, QComboBox, QFrame,
-    QHBoxLayout, QHeaderView, QLabel, QSizePolicy,
-    QSpacerItem, QTreeView, QVBoxLayout, QWidget)
+    QHBoxLayout, QHeaderView, QLabel, QPushButton,
+    QSizePolicy, QSpacerItem, QTreeView, QVBoxLayout,
+    QWidget)
 
 from jal.widgets.account_select import AccountButton
 from jal.widgets.custom.date_range_selector import DateRangeSelector
 
 class Ui_DealsReportWidget(object):
     def setupUi(self, DealsReportWidget):
         if not DealsReportWidget.objectName():
@@ -65,14 +66,19 @@
 
         self.horizontalLayout.addWidget(self.ReportAccountBtn)
 
         self.ReportFrameSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout.addItem(self.ReportFrameSpacer)
 
+        self.SaveButton = QPushButton(self.ReportParamsFrame)
+        self.SaveButton.setObjectName(u"SaveButton")
+
+        self.horizontalLayout.addWidget(self.SaveButton)
+
 
         self.verticalLayout.addWidget(self.ReportParamsFrame)
 
         self.ReportTreeView = QTreeView(DealsReportWidget)
         self.ReportTreeView.setObjectName(u"ReportTreeView")
         self.ReportTreeView.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.ReportTreeView.setAlternatingRowColors(True)
@@ -86,9 +92,10 @@
         QMetaObject.connectSlotsByName(DealsReportWidget)
     # setupUi
 
     def retranslateUi(self, DealsReportWidget):
         DealsReportWidget.setWindowTitle(QCoreApplication.translate("DealsReportWidget", u"Deals", None))
         self.GroupLbl.setText(QCoreApplication.translate("DealsReportWidget", u"Group by:", None))
         self.ReportAccountLbl.setText(QCoreApplication.translate("DealsReportWidget", u"Account:", None))
+        self.SaveButton.setText(QCoreApplication.translate("DealsReportWidget", u"Save...", None))
     # retranslateUi
```

### Comparing `jal-2023.4.8/jal/ui/reports/ui_holdings_report.py` & `jal-2023.5.1/jal/ui/reports/ui_holdings_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
     QFont, QFontDatabase, QGradient, QIcon,
     QImage, QKeySequence, QLinearGradient, QPainter,
     QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QApplication, QDateEdit, QFrame, QHBoxLayout,
-    QHeaderView, QLabel, QPushButton, QSizePolicy,
-    QSpacerItem, QTreeView, QVBoxLayout, QWidget)
+from PySide6.QtWidgets import (QApplication, QComboBox, QDateEdit, QFrame,
+    QHBoxLayout, QHeaderView, QLabel, QPushButton,
+    QSizePolicy, QSpacerItem, QTreeView, QVBoxLayout,
+    QWidget)
 
 from jal.widgets.account_select import CurrencyComboBox
 
 class Ui_HoldingsWidget(object):
     def setupUi(self, HoldingsWidget):
         if not HoldingsWidget.objectName():
             HoldingsWidget.setObjectName(u"HoldingsWidget")
@@ -42,14 +43,24 @@
         self.HoldingsDate.setObjectName(u"HoldingsDate")
         self.HoldingsDate.setDateTime(QDateTime(QDate(2020, 11, 24), QTime(0, 0, 0)))
         self.HoldingsDate.setCalendarPopup(True)
         self.HoldingsDate.setTimeSpec(Qt.UTC)
 
         self.horizontalLayout_8.addWidget(self.HoldingsDate)
 
+        self.GroupLbl = QLabel(self.HoldingsParamsFrame)
+        self.GroupLbl.setObjectName(u"GroupLbl")
+
+        self.horizontalLayout_8.addWidget(self.GroupLbl)
+
+        self.GroupCombo = QComboBox(self.HoldingsParamsFrame)
+        self.GroupCombo.setObjectName(u"GroupCombo")
+
+        self.horizontalLayout_8.addWidget(self.GroupCombo)
+
         self.HoldingsCurrencyLbl = QLabel(self.HoldingsParamsFrame)
         self.HoldingsCurrencyLbl.setObjectName(u"HoldingsCurrencyLbl")
 
         self.horizontalLayout_8.addWidget(self.HoldingsCurrencyLbl)
 
         self.HoldingsCurrencyCombo = CurrencyComboBox(self.HoldingsParamsFrame)
         self.HoldingsCurrencyCombo.setObjectName(u"HoldingsCurrencyCombo")
@@ -64,29 +75,30 @@
         self.SaveButton.setObjectName(u"SaveButton")
 
         self.horizontalLayout_8.addWidget(self.SaveButton)
 
 
         self.verticalLayout.addWidget(self.HoldingsParamsFrame)
 
-        self.HoldingsTableView = QTreeView(HoldingsWidget)
-        self.HoldingsTableView.setObjectName(u"HoldingsTableView")
-        self.HoldingsTableView.setFrameShape(QFrame.Panel)
-        self.HoldingsTableView.setAlternatingRowColors(True)
-        self.HoldingsTableView.setAnimated(True)
-        self.HoldingsTableView.setAllColumnsShowFocus(True)
+        self.HoldingsTreeView = QTreeView(HoldingsWidget)
+        self.HoldingsTreeView.setObjectName(u"HoldingsTreeView")
+        self.HoldingsTreeView.setFrameShape(QFrame.Panel)
+        self.HoldingsTreeView.setAlternatingRowColors(True)
+        self.HoldingsTreeView.setAnimated(True)
+        self.HoldingsTreeView.setAllColumnsShowFocus(True)
 
-        self.verticalLayout.addWidget(self.HoldingsTableView)
+        self.verticalLayout.addWidget(self.HoldingsTreeView)
 
 
         self.retranslateUi(HoldingsWidget)
 
         QMetaObject.connectSlotsByName(HoldingsWidget)
     # setupUi
 
     def retranslateUi(self, HoldingsWidget):
         HoldingsWidget.setWindowTitle(QCoreApplication.translate("HoldingsWidget", u"Holdings", None))
         self.HoldingsDate.setDisplayFormat(QCoreApplication.translate("HoldingsWidget", u"dd/MM/yyyy", None))
+        self.GroupLbl.setText(QCoreApplication.translate("HoldingsWidget", u"Group by:", None))
         self.HoldingsCurrencyLbl.setText(QCoreApplication.translate("HoldingsWidget", u"Common currency:", None))
         self.SaveButton.setText(QCoreApplication.translate("HoldingsWidget", u"Save...", None))
     # retranslateUi
```

### Comparing `jal-2023.4.8/jal/ui/reports/ui_income_spending_report.py` & `jal-2023.5.1/jal/ui/reports/ui_income_spending_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_peer_report.py` & `jal-2023.5.1/jal/ui/reports/ui_peer_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_profit_loss_report.py` & `jal-2023.5.1/jal/ui/reports/ui_profit_loss_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_tag_report.py` & `jal-2023.5.1/jal/ui/reports/ui_tag_report.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/reports/ui_tax_estimation.py` & `jal-2023.5.1/jal/ui/reports/ui_tax_estimation.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_asset_dlg.py` & `jal-2023.5.1/jal/ui/ui_asset_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_flow_export_widget.py` & `jal-2023.5.1/jal/ui/ui_flow_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_login_fns_dlg.py` & `jal-2023.5.1/jal/ui/ui_login_fns_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_main_window.py` & `jal-2023.5.1/jal/ui/ui_main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         self.actionQuotes.setObjectName(u"actionQuotes")
         self.actionOperations = QAction(JAL_MainWindow)
         self.actionOperations.setObjectName(u"actionOperations")
         self.PrepareFlowReport = QAction(JAL_MainWindow)
         self.PrepareFlowReport.setObjectName(u"PrepareFlowReport")
         self.actionBaseCurrency = QAction(JAL_MainWindow)
         self.actionBaseCurrency.setObjectName(u"actionBaseCurrency")
+        self.actionCleanAll = QAction(JAL_MainWindow)
+        self.actionCleanAll.setObjectName(u"actionCleanAll")
         self.centralwidget = QWidget(JAL_MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.centralwidget.setMaximumSize(QSize(16777215, 16777215))
         self.verticalLayout = QVBoxLayout(self.centralwidget)
         self.verticalLayout.setSpacing(0)
         self.verticalLayout.setObjectName(u"verticalLayout")
         self.verticalLayout.setContentsMargins(0, 0, 0, 0)
@@ -109,27 +111,29 @@
         self.MainMenu.addAction(self.menuReports.menuAction())
         self.MainMenu.addAction(self.menuImport.menuAction())
         self.MainMenu.addAction(self.menu_Export.menuAction())
         self.MainMenu.addAction(self.menuLanguage.menuAction())
         self.menuMain.addAction(self.actionOperations)
         self.menuMain.addAction(self.actionExit)
         self.menu_Data.addSeparator()
+        self.menu_Data.addAction(self.action_Re_build_Ledger)
+        self.menu_Data.addSeparator()
         self.menu_Data.addAction(self.actionAccounts)
         self.menu_Data.addAction(self.actionAssets)
         self.menu_Data.addAction(self.actionPeers)
         self.menu_Data.addAction(self.actionCategories)
         self.menu_Data.addAction(self.actionTags)
         self.menu_Data.addAction(self.actionQuotes)
         self.menu_Data.addSeparator()
         self.menu_Data.addAction(self.actionBaseCurrency)
         self.menu_Data.addSeparator()
         self.menu_Data.addAction(self.actionBackup)
         self.menu_Data.addAction(self.actionRestore)
         self.menu_Data.addSeparator()
-        self.menu_Data.addAction(self.action_Re_build_Ledger)
+        self.menu_Data.addAction(self.actionCleanAll)
         self.menu_Export.addAction(self.PrepareTaxForms)
         self.menu_Export.addAction(self.PrepareFlowReport)
         self.menuImport.addAction(self.action_LoadQuotes)
         self.menuImport.addAction(self.menuStatement.menuAction())
         self.menuImport.addAction(self.actionImportSlipRU)
 
         self.retranslateUi(JAL_MainWindow)
@@ -151,14 +155,15 @@
         self.PrepareTaxForms.setText(QCoreApplication.translate("JAL_MainWindow", u"Investment &tax report", None))
         self.actionTags.setText(QCoreApplication.translate("JAL_MainWindow", u"&Tags", None))
         self.actionImportSlipRU.setText(QCoreApplication.translate("JAL_MainWindow", u"Slip [RU]...", None))
         self.actionQuotes.setText(QCoreApplication.translate("JAL_MainWindow", u"&Quotes", None))
         self.actionOperations.setText(QCoreApplication.translate("JAL_MainWindow", u"&Operations", None))
         self.PrepareFlowReport.setText(QCoreApplication.translate("JAL_MainWindow", u"Foreign accounts &flow report", None))
         self.actionBaseCurrency.setText(QCoreApplication.translate("JAL_MainWindow", u"&Base Currency", None))
+        self.actionCleanAll.setText(QCoreApplication.translate("JAL_MainWindow", u"Clean All", None))
         self.menuMain.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Main", None))
         self.menu_Data.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Data", None))
         self.menu_Export.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Export", None))
         self.menuLanguage.setTitle(QCoreApplication.translate("JAL_MainWindow", u"L&anguage", None))
         self.menuImport.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Import", None))
         self.menuStatement.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Statement", None))
         self.menuReports.setTitle(QCoreApplication.translate("JAL_MainWindow", u"&Reports", None))
```

### Comparing `jal-2023.4.8/jal/ui/ui_operations_widget.py` & `jal-2023.5.1/jal/ui/ui_operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_rebuild_window.py` & `jal-2023.5.1/jal/ui/ui_rebuild_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_reference_data_dlg.py` & `jal-2023.5.1/jal/ui/ui_reference_data_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_select_account_dlg.py` & `jal-2023.5.1/jal/ui/ui_select_account_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_select_reference_dlg.py` & `jal-2023.5.1/jal/ui/ui_select_reference_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_slip_import_dlg.py` & `jal-2023.5.1/jal/ui/ui_slip_import_dlg.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_tax_export_widget.py` & `jal-2023.5.1/jal/ui/ui_tax_export_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/ui/ui_update_quotes_window.py` & `jal-2023.5.1/jal/ui/ui_update_quotes_window.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_10.sql` & `jal-2023.5.1/jal/updates/jal_delta_10.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_11.sql` & `jal-2023.5.1/jal/updates/jal_delta_11.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_12.sql` & `jal-2023.5.1/jal/updates/jal_delta_12.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_13.sql` & `jal-2023.5.1/jal/updates/jal_delta_13.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_14.sql` & `jal-2023.5.1/jal/updates/jal_delta_14.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_15.sql` & `jal-2023.5.1/jal/updates/jal_delta_15.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_16.sql` & `jal-2023.5.1/jal/updates/jal_delta_16.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_17.sql` & `jal-2023.5.1/jal/updates/jal_delta_17.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_18.sql` & `jal-2023.5.1/jal/updates/jal_delta_18.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_19.sql` & `jal-2023.5.1/jal/updates/jal_delta_19.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_20.sql` & `jal-2023.5.1/jal/updates/jal_delta_20.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_21.sql` & `jal-2023.5.1/jal/updates/jal_delta_21.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_22.sql` & `jal-2023.5.1/jal/updates/jal_delta_22.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_23.sql` & `jal-2023.5.1/jal/updates/jal_delta_23.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_25.sql` & `jal-2023.5.1/jal/updates/jal_delta_25.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_26.sql` & `jal-2023.5.1/jal/updates/jal_delta_26.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_27.sql` & `jal-2023.5.1/jal/updates/jal_delta_27.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_28.sql` & `jal-2023.5.1/jal/updates/jal_delta_28.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_29.sql` & `jal-2023.5.1/jal/updates/jal_delta_29.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_30.sql` & `jal-2023.5.1/jal/updates/jal_delta_30.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_31.sql` & `jal-2023.5.1/jal/updates/jal_delta_31.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_32.sql` & `jal-2023.5.1/jal/updates/jal_delta_32.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_33.sql` & `jal-2023.5.1/jal/updates/jal_delta_33.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_34.sql` & `jal-2023.5.1/jal/updates/jal_delta_34.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_35.sql` & `jal-2023.5.1/jal/updates/jal_delta_35.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_36.sql` & `jal-2023.5.1/jal/updates/jal_delta_36.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_37.sql` & `jal-2023.5.1/jal/updates/jal_delta_37.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_38.sql` & `jal-2023.5.1/jal/updates/jal_delta_38.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_40.sql` & `jal-2023.5.1/jal/updates/jal_delta_40.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_41.sql` & `jal-2023.5.1/jal/updates/jal_delta_41.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_42.sql` & `jal-2023.5.1/jal/updates/jal_delta_42.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_43.sql` & `jal-2023.5.1/jal/updates/jal_delta_43.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/updates/jal_delta_44.sql` & `jal-2023.5.1/jal/updates/jal_delta_44.sql`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/abstract_operation_details.py` & `jal-2023.5.1/jal/widgets/abstract_operation_details.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/account_select.py` & `jal-2023.5.1/jal/widgets/account_select.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/asset_dialog.py` & `jal-2023.5.1/jal/widgets/asset_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from PySide6.QtSql import QSqlRelation, QSqlRelationalDelegate
 from PySide6.QtWidgets import QDialog, QDataWidgetMapper, QStyledItemDelegate, QComboBox, QLineEdit
 from jal.ui.ui_asset_dlg import Ui_AssetDialog
 from jal.constants import PredefinedAsset, AssetData
 from jal.db.helpers import load_icon, localize_decimal
 from jal.widgets.delegates import DateTimeEditWithReset, BoolDelegate
 from jal.db.reference_models import AbstractReferenceListModel
+from jal.db.tag import JalTag
+from jal.widgets.reference_selector import TagSelector
 
 
 class AssetsListModel(AbstractReferenceListModel):
     def __init__(self, table, parent_view):
         super().__init__(table=table, parent_view=parent_view)
         self._columns = [("id", ''),
                          ("type_id", 'Asset type'),
@@ -181,29 +183,32 @@
     def __init__(self, key_field, value_field, parent=None):
         super().__init__(parent=parent)
         self._key = key_field
         self._value = value_field
         self.types = {
             AssetData.RegistrationCode: (self.tr("reg.code"), "str"),
             AssetData.ExpiryDate: (self.tr("expiry"), "date"),
-            AssetData.PrincipalValue: (self.tr("principal"), "float")
+            AssetData.PrincipalValue: (self.tr("principal"), "float"),
+            AssetData.Tag: (self.tr("tag"), "tag")
         }
 
     def type(self, index):
         return self.types[index][0]
 
     def display_value(self, type_index, value):
         datatype = self.types[type_index][1]
         try:
             if datatype == "str":
                 return value
             elif datatype == "date":
                 return datetime.utcfromtimestamp(int(value)).strftime("%d/%m/%Y")
             elif datatype == "float":
                 return f"{value:.2f}"
+            elif datatype == "tag":
+                return JalTag(int(value)).name()
             else:
                 assert False, "Unknown data type of asset data"
         except ValueError:
             return ''
 
     def createEditor(self, aParent, option, index):
         if index.column() == self._key:
@@ -214,14 +219,16 @@
             type_idx = index.model().data(index.sibling(index.row(), self._key), role=Qt.EditRole)
             if self.types[type_idx][1] == "str" or self.types[type_idx][1] == "float":
                 editor = QLineEdit(aParent)
             elif self.types[type_idx][1] == "date":
                 editor = DateTimeEditWithReset(aParent)
                 editor.setTimeSpec(Qt.UTC)
                 editor.setDisplayFormat("dd/MM/yyyy")
+            elif self.types[type_idx][1] == "tag":
+                editor = TagSelector(aParent)
             else:
                 assert False, f"Unknown data type '{self.types[type_idx][1]}' in DataDelegate.createEditor()"
         else:
             assert False, f"Delegate DataDelegate.createEditor() called for not-initialized column {index.column()}"
         return editor
 
     def setEditorData(self, editor, index):
@@ -239,14 +246,20 @@
                     QStyledItemDelegate.setEditorData(self, editor, index)
             elif self.types[type_idx][1] == "float":
                 try:
                     amount = Decimal(index.model().data(index, Qt.EditRole))
                 except (ValueError, TypeError):
                     amount = Decimal('0')
                 editor.setText(localize_decimal(amount))
+            elif self.types[type_idx][1] == "tag":
+                try:
+                    tag_id = int(index.model().data(index, Qt.EditRole))
+                except (ValueError, TypeError):
+                    tag_id = 0
+                editor.selected_id = tag_id
             else:
                 assert False, f"Unknown data type '{self.types[type_idx][1]}' in DataDelegate.setEditorData()"
         else:
             assert False, f"Delegate DataDelegate.setEditorData() called for not-initialized column {index.column()}"
 
     def setModelData(self, editor, model, index):
         if index.column() == self._key:
@@ -258,14 +271,16 @@
                 model.setData(index, editor.text())
             elif self.types[type_idx][1] == "date":
                 timestamp = editor.dateTime().toSecsSinceEpoch()
                 model.setData(index, str(timestamp))
             elif self.types[type_idx][1] == "float":
                 value = QLocale().toDouble(editor.text())[0]
                 model.setData(index, value)
+            elif self.types[type_idx][1] == "tag":
+                model.setData(index, str(editor.selected_id))
             else:
                 assert False, f"Unknown data type '{self.types[type_idx][1]}' in DataDelegate.setModelData()"
         else:
             assert False, f"Delegate DataDelegate.setModelData() called for not-initialized column {index.column()}"
 
 
 class ExtraDataModel(AbstractReferenceListModel):
```

### Comparing `jal-2023.4.8/jal/widgets/corporate_action_widget.py` & `jal-2023.5.1/jal/widgets/corporate_action_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/custom/date_range_selector.py` & `jal-2023.5.1/jal/widgets/custom/date_range_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/custom/db_lookup_combobox.py` & `jal-2023.5.1/jal/widgets/custom/db_lookup_combobox.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/custom/log_viewer.py` & `jal-2023.5.1/jal/widgets/custom/log_viewer.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/dividend_widget.py` & `jal-2023.5.1/jal/widgets/dividend_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/helpers.py` & `jal-2023.5.1/jal/widgets/helpers.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/income_spending_widget.py` & `jal-2023.5.1/jal/widgets/income_spending_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/main_window.py` & `jal-2023.5.1/jal/widgets/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         self.statementGroup.triggered.connect(self.statements.load)
         self.reportsGroup.triggered.connect(self.reports.show)
         self.ui.action_LoadQuotes.triggered.connect(partial(self.downloader.showQuoteDownloadDialog, self))
         self.ui.actionImportSlipRU.triggered.connect(self.importSlip)
         self.ui.actionBackup.triggered.connect(self.backup.create)
         self.ui.actionRestore.triggered.connect(self.backup.restore)
         self.ui.action_Re_build_Ledger.triggered.connect(partial(self.ledger.showRebuildDialog, self))
+        self.ui.actionCleanAll.triggered.connect(self.onCleanDB)
         self.ui.actionAccounts.triggered.connect(partial(self.onDataDialog, "accounts"))
         self.ui.actionAssets.triggered.connect(partial(self.onDataDialog, "assets"))
         self.ui.actionPeers.triggered.connect(partial(self.onDataDialog, "agents"))
         self.ui.actionCategories.triggered.connect(partial(self.onDataDialog, "categories"))
         self.ui.actionTags.triggered.connect(partial(self.onDataDialog, "tags"))
         self.ui.actionQuotes.triggered.connect(partial(self.onDataDialog, "quotes"))
         self.ui.actionBaseCurrency.triggered.connect(partial(self.onDataDialog, "base_currency"))
@@ -155,19 +156,32 @@
     def onLanguageChanged(self, action):
         language_code = action.data()
         if language_code != self.currentLanguage:
             JalSettings().setLanguage(language_code)
             QMessageBox().information(self, self.tr("Restart required"),
                                       self.tr("Language was changed to ") +
                                       QLocale.languageToString(QLocale(language_code).language()) + "\n" +
-                                      self.tr("You should restart application to apply changes\n"
-                                           "Application will be terminated now"),
+                                      self.tr("You should restart application to apply changes.\n"
+                                           "Application will be terminated now."),
                                       QMessageBox.Ok)
             self.close()
 
+    @Slot()
+    def onCleanDB(self, action):
+        if QMessageBox().warning(None, self.tr("Full clean-up"),
+                                 self.tr("All data will be deleted. The actions can't be undone.\nAre you sure?"),
+                                 QMessageBox.Yes, QMessageBox.No) == QMessageBox.No:
+            return
+        JalSettings().setValue("CleanDB", 1)
+        QMessageBox().information(self, self.tr("Restart required"),
+                                  self.tr("Database will be removed at next JAL start.\n"
+                                          "Application will be terminated now."),
+                                  QMessageBox.Ok)
+        self.close()
+
     # Create import menu for all known statements based on self.statements.items values
     def createStatementsImportMenu(self):
         for i, statement in enumerate(self.statements.items):
             statement_name = statement['name'].replace('&', '&&')  # & -> && to prevent shortcut creation
             if statement['icon']:
                 statement_icon = load_icon(statement['icon'])
                 action = QAction(statement_icon, statement_name, self)
@@ -200,15 +214,16 @@
 
     @Slot()
     def showAboutWindow(self):
         about_box = QMessageBox(self)
         about_box.setAttribute(Qt.WA_DeleteOnClose)
         about_box.setWindowTitle(self.tr("About"))
         version = f"{__version__} (db{Setup.DB_REQUIRED_VERSION})"
-        title = "<h3>JAL</h3><p>Just Another Ledger, " + self.tr("version") + " " + version +"</p>"
+        title = "<h3>JAL</h3><p>Just Another Ledger, " + self.tr("version") + " " + version +"</p>" + \
+            "<p>DB file: " + JalSettings().DbPath() + "</p>"
         about_box.setText(title)
         about_text = "<p>" + self.tr("More information, manuals and problem reports are at ") + \
                      "<a href=https://github.com/titov-vv/jal>" + self.tr("github home page") + "</a></p><p>" + \
                      self.tr("Questions, comments, help or donations:") + \
                      "</p><p><a href=mailto:jal@gmx.ru>jal@gmx.ru</a></p>" + \
                      "<p><a href=https://t.me/jal_support>Telegram</a></p>"
         about_box.setInformativeText(about_text)
```

### Comparing `jal-2023.4.8/jal/widgets/mdi.py` & `jal-2023.5.1/jal/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/operations_tabs.py` & `jal-2023.5.1/jal/widgets/operations_tabs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/operations_widget.py` & `jal-2023.5.1/jal/widgets/operations_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/price_chart.py` & `jal-2023.5.1/jal/widgets/price_chart.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/qr_scanner.py` & `jal-2023.5.1/jal/widgets/qr_scanner.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/reference_data.py` & `jal-2023.5.1/jal/widgets/reference_data.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/reference_dialogs.py` & `jal-2023.5.1/jal/widgets/reference_dialogs.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/reference_selector.py` & `jal-2023.5.1/jal/widgets/reference_selector.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/register_designer_plugins.py` & `jal-2023.5.1/jal/widgets/register_designer_plugins.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/selection_dialog.py` & `jal-2023.5.1/jal/widgets/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/tax_widget.py` & `jal-2023.5.1/jal/widgets/tax_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from PySide6.QtWidgets import QFileDialog, QMessageBox, QApplication
 from jal.ui.ui_tax_export_widget import Ui_TaxWidget
 from jal.ui.ui_flow_export_widget import Ui_MoneyFlowWidget
 from jal.widgets.mdi import MdiWidget
 from jal.widgets.helpers import ts2d
 from jal.db.asset import JalAsset
 from jal.db.peer import JalPeer
+from jal.db.settings import JalSettings, FolderFor
 from jal.data_export.taxes import TaxReport
 from jal.data_export.taxes_flow import TaxesFlowRus
 from jal.data_export.xlsx import XLSX
 from jal.data_export.dlsg import DLSG
 
 
 class TaxWidget(MdiWidget):
@@ -58,20 +59,22 @@
             selector = (self.tr("Save tax reports to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.ui.XlsFileName)
         elif type == 'DLSG':
             last_digit = self.year % 10
             selector = (self.tr("Save tax form to:"), self.tr(f"Tax form (*.dc{last_digit})"),
                         f".dc{last_digit}", self.ui.DlsgFileName)
         else:
             raise ValueError
-        filename = QFileDialog.getSaveFileName(self, selector[0], ".", selector[1])
+        folder = JalSettings().getRecentFolder(FolderFor.Report, '.')
+        filename = QFileDialog.getSaveFileName(self, selector[0], folder, selector[1])
         if filename[0]:
             if filename[1] == selector[1] and filename[0][-len(selector[2]):] != selector[2]:
                 selector[3].setText(filename[0] + selector[2])
             else:
                 selector[3].setText(filename[0])
+            JalSettings().setRecentFolder(FolderFor.Report, filename[0])
 
     def getYear(self):
         return self.ui.Year.value()
 
     def getXlsFilename(self):
         return self.ui.XlsFileName.text()
 
@@ -155,20 +158,22 @@
     @staticmethod
     def showInMDI(parent_mdi):
         parent_mdi.addSubWindow(MoneyFlowWidget(parent_mdi), maximized=False)
 
     @Slot()
     def OnFileBtn(self):
         selector = (self.tr("Save money flow report to:"), self.tr("Excel files (*.xlsx)"), '.xlsx', self.ui.XlsFileName)
-        filename = QFileDialog.getSaveFileName(self, selector[0], ".", selector[1])
+        folder = JalSettings().getRecentFolder(FolderFor.Report, '.')
+        filename = QFileDialog.getSaveFileName(self, selector[0], folder, selector[1])
         if filename[0]:
             if filename[1] == selector[1] and filename[0][-len(selector[2]):] != selector[2]:
                 selector[3].setText(filename[0] + selector[2])
             else:
                 selector[3].setText(filename[0])
+            JalSettings().setRecentFolder(FolderFor.Report, filename[0])
 
     def getYear(self):
         return self.ui.Year.value()
 
     def getXlsFilename(self):
         return self.ui.XlsFileName.text()
```

### Comparing `jal-2023.4.8/jal/widgets/trade_widget.py` & `jal-2023.5.1/jal/widgets/trade_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal/widgets/transfer_widget.py` & `jal-2023.5.1/jal/widgets/transfer_widget.py`

 * *Files identical despite different names*

### Comparing `jal-2023.4.8/jal.egg-info/PKG-INFO` & `jal-2023.5.1/jal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jal
-Version: 2023.4.8
+Version: 2023.5.1
 Summary: Just Another Ledger - project to track personal financial records
 Home-page: https://github.com/titov-vv/jal
 Author-email: jal@gmx.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `jal-2023.4.8/jal.egg-info/SOURCES.txt` & `jal-2023.5.1/jal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 jal/db/operations.py
 jal/db/operations_model.py
 jal/db/peer.py
 jal/db/reference_models.py
 jal/db/settings.py
 jal/db/tag.py
 jal/db/tax_estimator.py
+jal/db/trades_model.py
+jal/db/tree_model.py
 jal/db/view_model.py
 jal/img/accept.png
 jal/img/add.png
 jal/img/add_child.png
 jal/img/broom.png
 jal/img/cancel.png
 jal/img/chart.png
@@ -164,14 +166,15 @@
 jal/updates/jal_delta_38.sql
 jal/updates/jal_delta_39.sql
 jal/updates/jal_delta_40.sql
 jal/updates/jal_delta_41.sql
 jal/updates/jal_delta_42.sql
 jal/updates/jal_delta_43.sql
 jal/updates/jal_delta_44.sql
+jal/updates/jal_delta_45.sql
 jal/widgets/__init__.py
 jal/widgets/abstract_operation_details.py
 jal/widgets/account_select.py
 jal/widgets/asset_dialog.py
 jal/widgets/corporate_action_widget.py
 jal/widgets/delegates.py
 jal/widgets/dividend_widget.py
```

### Comparing `jal-2023.4.8/setup.py` & `jal-2023.5.1/setup.py`

 * *Files identical despite different names*

