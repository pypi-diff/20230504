# Comparing `tmp/MMM_Savings_Rate-0.4.tar.gz` & `tmp/MMM_Savings_Rate-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MMM_Savings_Rate-0.4.tar", last modified: Mon Feb  1 03:58:23 2016, max compression
+gzip compressed data, was "MMM_Savings_Rate-1.0.tar", last modified: Thu May  4 19:20:37 2023, max compression
```

## Comparing `MMM_Savings_Rate-0.4.tar` & `MMM_Savings_Rate-1.0.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/
--rw-rw-r--   0 brad      (1000) brad      (1000)     1161 2016-02-01 03:57:11.000000 MMM_Savings_Rate-0.4/setup.py
--rw-rw-r--   0 brad      (1000) brad      (1000)    32005 2016-01-22 02:59:26.000000 MMM_Savings_Rate-0.4/LICENSE.txt
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/csv/
--rw-rw-r--   0 brad      (1000) brad      (1000)      240 2016-01-22 00:39:09.000000 MMM_Savings_Rate-0.4/csv/savings-example.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)      225 2016-01-22 00:39:09.000000 MMM_Savings_Rate-0.4/csv/income-joe.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)      424 2016-01-22 00:39:09.000000 MMM_Savings_Rate-0.4/csv/income-example.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)      104 2016-01-22 00:39:09.000000 MMM_Savings_Rate-0.4/csv/savings-joe.csv
--rwxrwxr-x   0 brad      (1000) brad      (1000)      379 2016-01-22 00:47:24.000000 MMM_Savings_Rate-0.4/csv/savings.csv
--rwxrwxr-x   0 brad      (1000) brad      (1000)      936 2016-01-22 00:47:37.000000 MMM_Savings_Rate-0.4/csv/income.csv
--rwxrwxr-x   0 brad      (1000) brad      (1000)       65 2016-01-23 22:31:06.000000 MMM_Savings_Rate-0.4/csv/savings-uzia.csv
--rwxrwxr-x   0 brad      (1000) brad      (1000)      478 2016-01-23 22:31:22.000000 MMM_Savings_Rate-0.4/csv/income-uzia.csv
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/tests/
--rw-rw-r--   0 brad      (1000) brad      (1000)        0 2016-01-27 03:06:55.000000 MMM_Savings_Rate-0.4/tests/__init__.py
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/tests/test_csv/
--rw-rw-r--   0 brad      (1000) brad      (1000)       43 2016-01-31 18:55:42.000000 MMM_Savings_Rate-0.4/tests/test_csv/savings-empty.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)        1 2016-01-31 20:09:50.000000 MMM_Savings_Rate-0.4/tests/test_csv/income-blank.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)        1 2016-01-31 20:10:31.000000 MMM_Savings_Rate-0.4/tests/test_csv/savings-blank.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)      104 2016-01-31 18:54:22.000000 MMM_Savings_Rate-0.4/tests/test_csv/income-empty.csv
--rw-rw-r--   0 brad      (1000) brad      (1000)    10780 2016-01-31 23:53:43.000000 MMM_Savings_Rate-0.4/tests/test_savings_rate.py
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/tests/test_config/
--rw-rw-r--   0 brad      (1000) brad      (1000)      320 2016-01-31 19:02:32.000000 MMM_Savings_Rate-0.4/tests/test_config/account-config-empty-csv.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1835 2016-01-31 19:42:28.000000 MMM_Savings_Rate-0.4/tests/test_config/config-test-blank-csv.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1612 2016-01-29 18:33:45.000000 MMM_Savings_Rate-0.4/tests/test_config/config-julia-test.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)       91 2016-01-29 21:07:36.000000 MMM_Savings_Rate-0.4/tests/test_config/account-config-test-no-enemies.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1810 2016-01-30 18:27:29.000000 MMM_Savings_Rate-0.4/tests/test_config/config-joe-test.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)      310 2016-01-29 18:34:42.000000 MMM_Savings_Rate-0.4/tests/test_config/account-config.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)      310 2016-01-29 19:31:50.000000 MMM_Savings_Rate-0.4/tests/test_config/account-config-test-bad.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1817 2016-01-30 23:31:55.000000 MMM_Savings_Rate-0.4/tests/test_config/config-test.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)      320 2016-01-31 19:28:17.000000 MMM_Savings_Rate-0.4/tests/test_config/account-config-blank-csv.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1835 2016-01-31 19:09:50.000000 MMM_Savings_Rate-0.4/tests/test_config/config-test-empty-csv.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     4932 2016-01-31 22:57:43.000000 MMM_Savings_Rate-0.4/tests/test_config.py
--rw-rw-r--   0 brad      (1000) brad      (1000)     7868 2016-02-01 01:41:03.000000 MMM_Savings_Rate-0.4/README.md
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/
--rw-rw-r--   0 brad      (1000) brad      (1000)     1287 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/SOURCES.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)        1 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/dependency_links.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)       19 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/top_level.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)       60 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/requires.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)        1 2016-01-27 02:16:04.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/not-zip-safe
--rw-rw-r--   0 brad      (1000) brad      (1000)       50 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/entry_points.txt
--rw-rw-r--   0 brad      (1000) brad      (1000)    10283 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/PKG-INFO
--rw-rw-r--   0 brad      (1000) brad      (1000)       59 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/setup.cfg
--rw-rw-r--   0 brad      (1000) brad      (1000)    32971 2016-01-31 23:43:30.000000 MMM_Savings_Rate-0.4/savings_rate.py
-drwxrwxr-x   0 brad      (1000) brad      (1000)        0 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/config/
--rwxrwxr-x   0 brad      (1000) brad      (1000)     1891 2016-01-30 18:31:16.000000 MMM_Savings_Rate-0.4/config/config-uzia.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1867 2016-01-30 18:30:34.000000 MMM_Savings_Rate-0.4/config/config-example.ini
--rwxrwxr-x   0 brad      (1000) brad      (1000)     2438 2016-02-01 01:28:13.000000 MMM_Savings_Rate-0.4/config/config.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)      278 2016-01-25 02:21:05.000000 MMM_Savings_Rate-0.4/config/account-config-example.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)     1810 2016-01-30 18:30:56.000000 MMM_Savings_Rate-0.4/config/config-joe.ini
--rwxrwxr-x   0 brad      (1000) brad      (1000)      268 2016-01-25 00:03:43.000000 MMM_Savings_Rate-0.4/config/account-config.ini
--rw-rw-r--   0 brad      (1000) brad      (1000)    10283 2016-02-01 03:58:23.000000 MMM_Savings_Rate-0.4/PKG-INFO
--rw-rw-r--   0 brad      (1000) brad      (1000)      145 2016-02-01 03:55:57.000000 MMM_Savings_Rate-0.4/MANIFEST.in
--rw-rw-r--   0 brad      (1000) brad      (1000)     1879 2016-01-24 22:43:10.000000 MMM_Savings_Rate-0.4/sr_launcher.py
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/
+-rw-rw-r--   0 brad      (1001) brad      (1001)    32005 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/LICENSE.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)      145 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/MANIFEST.in
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.824360 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/
+-rw-rw-r--   0 brad      (1001) brad      (1001)    10930 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/PKG-INFO
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1320 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/SOURCES.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)        1 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/dependency_links.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)       50 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/entry_points.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)        1 2023-04-06 20:42:36.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/not-zip-safe
+-rw-rw-r--   0 brad      (1001) brad      (1001)      182 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/requires.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)       19 2023-05-04 19:20:37.000000 MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/top_level.txt
+-rw-rw-r--   0 brad      (1001) brad      (1001)    10930 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/PKG-INFO
+-rw-rw-r--   0 brad      (1001) brad      (1001)    10483 2023-05-04 18:02:04.000000 MMM_Savings_Rate-1.0/README.md
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.824360 MMM_Savings_Rate-1.0/config/
+-rw-rw-r--   0 brad      (1001) brad      (1001)      278 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/config/account-config-example.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     2111 2023-05-03 00:27:05.000000 MMM_Savings_Rate-1.0/config/config-example.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1399 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/config/config-joe.ini
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/csv/
+-rw-rw-r--   0 brad      (1001) brad      (1001)      424 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/csv/income-example.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)     5698 2023-04-07 03:04:45.000000 MMM_Savings_Rate-1.0/csv/income-example.xlsx
+-rw-rw-r--   0 brad      (1001) brad      (1001)      225 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/csv/income-joe.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)      240 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/csv/savings-example.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)     5519 2023-04-07 03:05:37.000000 MMM_Savings_Rate-1.0/csv/savings-example.xlsx
+-rw-rw-r--   0 brad      (1001) brad      (1001)      104 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/csv/savings-joe.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)    42426 2023-05-04 17:51:16.000000 MMM_Savings_Rate-1.0/savings_rate.py
+-rw-rw-r--   0 brad      (1001) brad      (1001)       38 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/setup.cfg
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1491 2023-05-04 19:19:10.000000 MMM_Savings_Rate-1.0/setup.py
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1853 2023-04-07 21:06:40.000000 MMM_Savings_Rate-1.0/sr_launcher.py
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/tests/
+-rw-rw-r--   0 brad      (1001) brad      (1001)        0 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/__init__.py
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/tests/test_config/
+-rw-rw-r--   0 brad      (1001) brad      (1001)      320 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/account-config-blank-csv.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)      320 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/account-config-empty-csv.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)      310 2023-04-07 01:28:11.000000 MMM_Savings_Rate-1.0/tests/test_config/account-config-test-bad.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)       91 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/account-config-test-no-enemies.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)      310 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/account-config.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1927 2023-04-12 04:10:20.000000 MMM_Savings_Rate-1.0/tests/test_config/config-bad-values.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1399 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/config-joe-test.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1201 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/config-julia-test.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     2111 2023-05-03 00:30:46.000000 MMM_Savings_Rate-1.0/tests/test_config/config-missing-values.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1401 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/config-test-blank-csv.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1401 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_config/config-test-empty-csv.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     1385 2023-04-07 02:49:13.000000 MMM_Savings_Rate-1.0/tests/test_config/config-test-xlsx.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     2097 2023-05-03 00:29:16.000000 MMM_Savings_Rate-1.0/tests/test_config/config-test.ini
+-rw-rw-r--   0 brad      (1001) brad      (1001)     9096 2023-05-03 00:44:59.000000 MMM_Savings_Rate-1.0/tests/test_config.py
+drwxrwxr-x   0 brad      (1001) brad      (1001)        0 2023-05-04 19:20:37.828360 MMM_Savings_Rate-1.0/tests/test_csv/
+-rw-rw-r--   0 brad      (1001) brad      (1001)        1 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_csv/income-blank.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)      104 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_csv/income-empty.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)        1 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_csv/savings-blank.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)       43 2023-04-06 20:42:35.000000 MMM_Savings_Rate-1.0/tests/test_csv/savings-empty.csv
+-rw-rw-r--   0 brad      (1001) brad      (1001)    15568 2023-04-09 21:00:19.000000 MMM_Savings_Rate-1.0/tests/test_savings_rate.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MMM_Savings_Rate-0.4/LICENSE.txt` & `MMM_Savings_Rate-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MMM_Savings_Rate-0.4/tests/test_config/config-test-blank-csv.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-test.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = tests/test_csv/income-blank.csv
+pay = csv/income-example.csv
 
 ; Spreadsheet column name that mapps to a date for an
 ; income or pay transaction.
 pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
@@ -16,39 +16,51 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = tests/test_csv/savings-blank.csv
+; Path to .csv file with information about savings.
+savings = csv/savings-example.csv
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
 
 ; Spreadsheet column name that mapps to a date for a 
 ; savings transaction.
 savings_date = Date
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
+; Settings for enabling the display of average US savings rates from FRED:
+; The Federal Reserve Bank of St. Louis. Both fred_url and fred_api_key must be
+; present. You can get a FRED api_key here: https://fred.stlouisfed.org/docs/api/api_key.html.
+fred_url = https://fred-test.com
+fred_api_key = test-api-key
+
+; Spreadsheet column that maps to notes or special events that you want to
+; show on your plot.
+notes = My Notes
+
+; Whether or not to show the running average
+show_average = true
+
+; An aspirational savings rate goal you are trying to hit.
+goal = 70
 
-; Username for mint.com
-username = user@email.com
+; FI number
+fi_number = 750000
 
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
+; Total account balances
+total_balances = Balances
 
+; % FI plot annotation column header
+percent_fi_notes = % FI Notes
 
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/tests/test_config/config-julia-test.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-test-empty-csv.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = /home/username/Documents/csv/income-joe.csv
+pay = tests/test_csv/income-empty.csv
+
+; Spreadsheet column name that mapps to a date for an
+; income or pay transaction.
+pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
 
 ; A .csv column header used for tracking an employer retirement plan match.
 employer_match = Employer Match
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
-taxes_and_fees = Federal Tax,State Tax,Professional Fees 
+taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = /home/username/Documents/csv/savings-joe.csv
+; Path to .csv file with information about savings.
+savings = tests/test_csv/savings-empty.csv
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
-savings_accounts = Savings Account
+savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
+
+; Spreadsheet column name that mapps to a date for a 
+; savings transaction.
+savings_date = Date
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
-
-; Username for mint.com
-username = joe@email.com
-
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Savings Account
-
-
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
-
```

### Comparing `MMM_Savings_Rate-0.4/tests/test_config/config-joe-test.ini` & `MMM_Savings_Rate-1.0/config/config-joe.ini`

 * *Files 14% similar despite different names*

```diff
@@ -16,40 +16,27 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = Federal Tax,State Tax,Professional Fees 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
+; Path to .csv file with information about savings.
 savings = /home/username/Documents/csv/savings-joe.csv
 
 ; Spreadsheet column name that mapps to a date for a 
 ; savings transaction.
 savings_date = Date
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Savings Account
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
-
-; Username for mint.com
-username = joe@email.com
-
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Savings Account
-
-
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/tests/test_config/config-test.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-test-xlsx.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = csv/income-example.csv
+pay = csv/income-example.xlsx
 
 ; Spreadsheet column name that mapps to a date for an
 ; income or pay transaction.
 pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
@@ -16,39 +16,26 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = csv/savings-example.csv
+; Path to .csv file with information about savings.
+savings = csv/savings-example.xlsx
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
 
 ; Spreadsheet column name that mapps to a date for a 
 ; savings transaction.
 savings_date = Date
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
-
-; Username for mint.com
-username = user@email.com
-
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
-
-
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/tests/test_config/config-test-empty-csv.ini` & `MMM_Savings_Rate-1.0/config/config-example.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = tests/test_csv/income-empty.csv
+pay = /home/username/Documents/csv/income-example.csv
 
 ; Spreadsheet column name that mapps to a date for an
 ; income or pay transaction.
 pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
@@ -16,39 +16,47 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = tests/test_csv/savings-empty.csv
+; Path to .csv file with information about savings.
+savings = /home/username/Documents/csv/savings-example.csv
+
+; Spreadsheet column name that mapps to a date for a 
+; savings transaction.
+savings_date = Date
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
 
-; Spreadsheet column name that mapps to a date for a 
-; savings transaction.
-savings_date = Date
+; Whether or not to show the running average
+show_average = true
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
+; Settings for enabling the display of average US savings rates from FRED:
+; The Federal Reserve Bank of St. Louis. Both fred_url and fred_api_key must be
+; present. You can get a FRED api_key here: https://fred.stlouisfed.org/docs/api/api_key.html.
+; fred_url = https://api.stlouisfed.org/fred/series/observations?series_id=PSAVERT&file_type=json
+; fred_api_key = fred-api-key
+
+; An aspirational savings rate goal you are trying to hit.
+;goal = 70
 
-; Username for mint.com
-username = user@email.com
+; FI number
+;fi_number = 1000000
 
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
+; Total account balances
+;total_balances = Net Worth
 
+; % FI plot annotation column header
+;percent_fi_notes = Net Worth Notes
 
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/README.md` & `MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,118 +1,173 @@
-# MMM_Savings_Rate
+Metadata-Version: 2.1
+Name: MMM-Savings-Rate
+Version: 1.0
+Summary: An application that can parse spreadsheets in order to calculate and plot a user's monthly savings rate over time. 
+Home-page: https://github.com/bbusenius/MMM_Savings_Rate.git
+Author: Brad Busenius
+Author-email: bbusenius@gmail.com
+License: GNU GPLv3, see LICENSE.txt
+Platform: UNKNOWN
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-This application is a command-line utility that allows users to calculate and track their monthly savings rates over time. Users simply enter their savings and income data into a spreadsheet saved as a .csv. Unique spreadsheet column headers are mapped to the application through user configuration files, allowing the utility to be used with any custom spreadsheet. When the simulation is run, user monthly savings rates are plotted on a line graph.
+# MMM Savings Rate
 
-![Example savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png)
-
-Additionally, users may supply secondary, "enemy" spreadsheets. This feature is provided in order to make the experience fun, game-like, and competitive for those who prefer such an experience. If an enemy spreadsheet is provided, the enemy savings rates are plotted alongside those of the user. This feature might be used by spouses who wish to compete with each other, for example.
+MMM Savings Rate is a tool that allows users to calculate and track their monthly savings rates over time. It was developed using functions from the [FI module](https://github.com/bbusenius/FI) and plots savings rates using [Bokeh](https://bokeh.org/). Users simply enter their savings and income data into a spreadsheet. Unique spreadsheet column headers are mapped to the application through user configuration files, allowing the utility to be used with any custom spreadsheet. When the simulation runs, the user's monthly savings rates are plotted on a line graph.
 
-*MMM_Savings_Rate was inspired by Mr. Money Mustache. Visit the Mr. Money Mustache website and [read this article to learn more](http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement).*
+![Example savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png)
 
-## Web version
-Though MMM_Savings_Rate is meant to be run from the command-line, a full, graphical, web-based version of the project exists at: https://savingsratewars.com/. Use the web-based version of the software if you don't want to deal with installation and configuration.
+Users may also supply secondary, "enemy" spreadsheets. This feature is provided to make the experience fun, game-like, and competitive for people who prefer such an experience. If an enemy spreadsheet is provided, the enemy savings rates are plotted alongside those of the main user. This feature is optional.
 
+*MMM Savings Rate was inspired by Mr. Money Mustache. Visit the Mr. Money Mustache website and [read this article to learn more](http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement).*
 
 ## Installation
 This package should generally be installed using pip.
 
 ### For users 
 
 ```
-pip install MMM-Savings-Rate
+pip install git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
 ```
 ### For developers
 
 ```
-git clone https://github.com/bbusenius/MMM_Savings_Rate.git
-python3 setup.py develop 
-```
-or 
-
-```
 pip install -e git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
 ```
-## Using the application
+## Setting up the application
 
 In order to get things going, you'll only need to take the following steps:
 
-1. Setup a directory of .csv files with the financial data needed to run the simulation.
+1. Setup a directory of spreadsheet files with the financial data needed to run the simulation.
 2. Configuration:
-  - Create an account-config.ini with player information.
+  - Create an account-config.ini with user information.
   - Create a config.ini with personal settings and column mappings.
-3. Run the simulation command with a path to your configuration files. 
-
-Read on to see how to do each of these things.
+3. Run the simulation command with a path to your configuration files.
 
 ### Spreadsheet files
-MMM_Savings_Rate was designed to be flexible in order to work with your preexisting spreadsheets. At the moment, spreadsheets must be saved as .csv files, however, column headers can be unique, so it doesn't matter what labels you use to categorize things. To get started you'll need financial data for both **income** and **savings**.
+MMM Savings Rate was designed to be flexible in order to work with a variety of spreadsheets. At the moment, spreadsheets must be saved as .xlsx or .csv files, however, column headers can be unique, so it doesn't matter what labels you use to categorize things. To get started you'll need financial data for both **income** and **savings**.
 
-This data can exist in a single spreadsheet with a variety of financial data or separate spreadsheets for income and savings. How you set it up is up to you, however, certain data is required. The application will allow you to map your column labels to fields, so you don't have to name them the same as outlined here. You also might want to split some of these fields over multiple columns in your spreadsheet. Jump to the configuration section to learn how to do this. In any event, however you decide to enter the data in your spreadsheet, all of the following fields must be represented in some fashion. 
+This data can exist in a single spreadsheet with other financial data or it can exist in separate spreadsheets. How you set it up is your choice, however, certain data is required. The application will allow you to map your column labels to fields, so you don't have to name them the same as outlined here. You also might want to split some of these fields over multiple columns in your spreadsheet. Jump to the configuration section to learn how to do this. However you decide to enter the data in your spreadsheet, all of the following fields must be represented in some fashion.
 
-- **Date for pay** - the date of your paycheck or date associated with the income being entered. The application can parse most date formats. 
+- **Date for pay** - the date of your paycheck or date associated with the income being entered. The application can parse most date formats.
 - **Gross Pay** - the amount of money you made in its entirety before taxes were withdrawn.
 - **Employer Match** - money contributed to a retirement plan by your employer.
-- **Taxes and Fees** - any taxes and fees taken out of your paycheck before it was delivered, e.g. OASDI, Medicare, etc.
+- **Taxes and Fees** - any taxes and fees taken out of your paycheck before it was delivered, e.g. FICA, Medicare, etc.
 - **Savings Accounts** - a dollar amount (mapped to 1 or multiple accounts)
 - **Date for savings** - the date you saved money into each account.
 
 *Note about "Savings Accounts": you might have multiple savings accounts, e.g. Bank Account, Vanguard Brokerage, Roth. Each one of these would contain a dollar amount representing the quantity of money saved for the month. Mapping will be handled in the configuration stage.*
 
-[For example spreadsheets please look in the csv directory](https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv). This should give you a good idea of how to lay things out. 
+[For example spreadsheets please look in the csv directory](https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv). This should give you a good idea of how to lay things out.
 
 ### Configuration
 
 In order to run the simulation the following two files are required:
 
-1. account-config.ini - the configuration for the players. Think of this as a listing of users. Each user has an id, name, and a link to his or her personal configuration.
+1. account-config.ini - the configuration for users. Think of this as a listing of users. Each user has an id, name, and a link to his or her personal configuration.
 2. config.ini - the configuration for the main user. Think of this as all of your personal settings.
 
 *Optional, "enemy" config files can be named however you like, e.g. config-spouse.ini. These should be setup in a similar fashion as config.ini and they should be listed as pipe separated groupings under "enemies" in account-config.ini.*
 
 #### account-config.ini
-A file must exist with the name account-config.ini. An example account-config.ini might look like this:
+A file must exist with the name `account-config.ini`. An example account-config.ini might look like this:
 
 ```
 [Users]
 ; Unique ID, name, and config file name for user.
 self = 1,My name,config.ini
 
-; Unique ID, name, and pipe separated list of config 
+; Unique ID, name, and pipe separated list of config
 ; file names for user's enemies.
 enemies = 2,Joe,config-spouse.ini|3,Brother,config-brother.ini
 ```
 
-The [Users] section is required. The "self" field represents the main player (you). This field should contain a comma separated list with a unique numerical ID, followed by a name, and the name of a main user config file.
- 
+The `[Users]` section is required. The "self" field represents the main user (you). This field should contain a comma separated list with a unique numerical ID, followed by a name, and the name of a main user config file.
+
 The "enemies" field is optional. If it's being used, it should be setup the same as the self field, however, if more than one enemy exists, this can be a pipe separated list of comma separated values.
 
 #### config.ini
-The config.ini file is the second configuration file. This file is required. It contains all of your personal settings and spreadsheet mappings. 
+The `config.ini` file is the second configuration file. This file is required. It contains all of your personal settings and spreadsheet mappings.
 
 [Please look at this example](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/config/config-example.ini).
 
-The majority of what's here is listed under [Sources]. Settings include:
+##### Main settings
+
+The majority of the main settings are listed under `[Sources]`. Settings include:
 
-- **pay** - a full path to your income .csv file.
-- **pay_date** - the name of a column header for the dates of income or pay transactions.
-- **savings** - a full path to your savings .csv file (can be the same file used for pay).
-- **savings_date** - the name of a column header for the dates of income or pay transactions.
-- **gross_income** - the name of a column header in your spreadsheet that represents gross pay.
+- **pay** - a full path to your income spreadsheet.
+- **pay_date** - the name of a column header for the dates of income or payment transactions.
+- **savings** - a full path to your savings spreadsheet (can be the same file used for pay).
+- **savings_date** - the name of a column header for the dates of income or payment transactions.
+- **gross_income** - the name of a column header in your spreadsheet representing gross pay.
 - **employer_match** - the name of a column header in your spreadsheet that represents your employer match.
-- **taxes_and_fees** - the names of column headers in your spreadsheet that contain taxes and fees.
-- **savings_accounts** - the names of column headers in your spreadsheet that contain savings data from an account or accounts.
+- **taxes_and_fees** - the names of column headers in your spreadsheet containing taxes and fees.
+- **savings_accounts** - the names of column headers in your spreadsheet that contain savings data from an investment account or accounts.
+- **goal** - optional setting that allows you to set a savings rate goal that you're trying to reach.
 - **war** - allows you to show or hide, "enemy" plots on your graph. Set this to, "off" if you only want to see your own data.
 
-Settings under [Graph] allow you to change the size of the plot that's generated. 
-*Note: Mint integration is not yet operational*.
+##### Graph settings
+
+Settings under `[Graph]` allow you to change the width and height of the plot that's generated (though plots are generally responsive).
+
+##### Additional settings
+
+###### US Average Savings Rates from FRED
+
+Optional settings allow you to plot the average US savings rates alongside your own. This data comes from the Federal Reserve Economic Data (FRED) at the Federal Reserve Bank of St. Louis.
+
+- **fred_url** - the url of the FRED API endpoint.
+- **fred_api_key** - an API token to use FRED.
+
+In order to use these settings, you will need to sign up for an account with FRED and request an API token. This takes about 5 minutes and [can be done on their website](https://fred.stlouisfed.org/docs/api/api_key.html).
+
+Once you enable FRED, you will be able to see how your savings rates dominate the US average*.
+
+![US average savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/FRED.png)
+
+*US average savings rates calculated by FRED are generated after removing outlays from personal income. Since outlays include purchases of durable and non-durable goods, these savings rates are inflated. Even so, as a Mustachian you will easily beat these averages.
+
+###### Notes and goal
+
+If you want to annotate points on your plot with text from your spreadsheet, you can map a `notes` field. This should match a column header on your spreadsheet. If you're using separate spreadsheets for savings and income, the application will look for the same column name in both spreadsheets and de-dupe duplicate notes for the same month while displaying all notes from both spreadsheets for the same month if they're unique.
+
+- **notes** - the name of a column header that maps to notes or special events that you want to show on your plot.
+
+A goal can be added to your plot as well.
+
+- **goal** - numeric value of a savings rate goal you'd like to reach, e.g. 70.
+
+![Savings rates plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/notes.png)
+
+###### % FI
+
+If you want to plot your progress towards FI as a percentage of your FI number, you can enable this with the following settings in your `config.ini`:
+
+- **fi_number** - your FI number.
+- **total_balances** - a spreadsheet heading that maps to a column where you track the total monthly balance of all your accounts.
+- **percent_fi_notes** - a spreadsheet heading that maps to a column with text that you want to show on the % FI plot. Entries will appear as event dots on the plot and will display tooltips with the notes on hover.
+
+This doesn't take into account liabilities so, if you have them, you can just as easily map these configurations to a column that tracks net worth.
+
+![Percent FI plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/percent-fi-notes.png)
 
 ### Running the simulation
 
-Once you have your .csv and your config files ready to go, you can run the application. Just open a terminal and type the command:
+Once you have your spreadsheet and your configuration files ready to go, you can run the application. Just open a terminal and type the command:
 
 ```
-savingsrates -p /home/joeconsumer/Documents/Code/Projects/MMM_Savings_Rate/config/
+savingsrates -p /home/joe_mustachian/Documents/Code/Projects/MMM_Savings_Rate/config/
 ```
-The -p flag should specify the full path to your directory of config files. When you run the command a plot of your monthly savings rates should open in a browser window.
+The -p flag should specify the full path to your directory of configuration files. When you run the command a plot of your monthly savings rates should open in a browser window.
 
 ## Requirements
-This utility runs on python 3.4. All additional dependencies should be automatically downloaded and included during installation. If you'd like to see all of what will be installed look at [setup.py](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py) or [requirements.txt](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt).
+
+This utility runs on python 3.x. All additional dependencies should be automatically downloaded and included during installation. If you'd like to see all of what will be installed look at [setup.py](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py) and [requirements.txt](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt).
+
+## Running tests
+
+```
+python3 -m unittest discover tests -p 'test_*.py'
+```
+
+
```

### Comparing `MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/SOURCES.txt` & `MMM_Savings_Rate-1.0/MMM_Savings_Rate.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,37 +8,35 @@
 MMM_Savings_Rate.egg-info/SOURCES.txt
 MMM_Savings_Rate.egg-info/dependency_links.txt
 MMM_Savings_Rate.egg-info/entry_points.txt
 MMM_Savings_Rate.egg-info/not-zip-safe
 MMM_Savings_Rate.egg-info/requires.txt
 MMM_Savings_Rate.egg-info/top_level.txt
 config/account-config-example.ini
-config/account-config.ini
 config/config-example.ini
 config/config-joe.ini
-config/config-uzia.ini
-config/config.ini
 csv/income-example.csv
+csv/income-example.xlsx
 csv/income-joe.csv
-csv/income-uzia.csv
-csv/income.csv
 csv/savings-example.csv
+csv/savings-example.xlsx
 csv/savings-joe.csv
-csv/savings-uzia.csv
-csv/savings.csv
 tests/__init__.py
 tests/test_config.py
 tests/test_savings_rate.py
 tests/test_config/account-config-blank-csv.ini
 tests/test_config/account-config-empty-csv.ini
 tests/test_config/account-config-test-bad.ini
 tests/test_config/account-config-test-no-enemies.ini
 tests/test_config/account-config.ini
+tests/test_config/config-bad-values.ini
 tests/test_config/config-joe-test.ini
 tests/test_config/config-julia-test.ini
+tests/test_config/config-missing-values.ini
 tests/test_config/config-test-blank-csv.ini
 tests/test_config/config-test-empty-csv.ini
+tests/test_config/config-test-xlsx.ini
 tests/test_config/config-test.ini
 tests/test_csv/income-blank.csv
 tests/test_csv/income-empty.csv
 tests/test_csv/savings-blank.csv
 tests/test_csv/savings-empty.csv
```

### Comparing `MMM_Savings_Rate-0.4/MMM_Savings_Rate.egg-info/PKG-INFO` & `MMM_Savings_Rate-1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,226 +1,173 @@
-Metadata-Version: 1.0
-Name: MMM-Savings-Rate
-Version: 0.4
+Metadata-Version: 2.1
+Name: MMM_Savings_Rate
+Version: 1.0
 Summary: An application that can parse spreadsheets in order to calculate and plot a user's monthly savings rate over time. 
 Home-page: https://github.com/bbusenius/MMM_Savings_Rate.git
 Author: Brad Busenius
 Author-email: bbusenius@gmail.com
 License: GNU GPLv3, see LICENSE.txt
-Description: MMM\_Savings\_Rate
-        ==================
-        
-        This application is a command-line utility that allows users to
-        calculate and track their monthly savings rates over time. Users simply
-        enter their savings and income data into a spreadsheet saved as a .csv.
-        Unique spreadsheet column headers are mapped to the application through
-        user configuration files, allowing the utility to be used with any
-        custom spreadsheet. When the simulation is run, user monthly savings
-        rates are plotted on a line graph.
-        
-        .. figure:: https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png
-           :alt: Example savings rates plotted
-        
-           Example savings rates plotted
-        
-        Additionally, users may supply secondary, "enemy" spreadsheets. This
-        feature is provided in order to make the experience fun, game-like, and
-        competitive for those who prefer such an experience. If an enemy
-        spreadsheet is provided, the enemy savings rates are plotted alongside
-        those of the user. This feature might be used by spouses who wish to
-        compete with each other, for example.
-        
-        *MMM\_Savings\_Rate was inspired by Mr. Money Mustache. Visit the Mr.
-        Money Mustache website and `read this article to learn
-        more <http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement>`__.*
-        
-        Web version
-        -----------
-        
-        Though MMM\_Savings\_Rate is meant to be run from the command-line, a
-        full, graphical, web-based version of the project exists at:
-        https://savingsratewars.com/. Use the web-based version of the software
-        if you don't want to deal with installation and configuration.
-        
-        Installation
-        ------------
-        
-        This package should generally be installed using pip.
-        
-        For users
-        ~~~~~~~~~
-        
-        ::
-        
-            pip install MMM-Savings-Rate
-        
-        For developers
-        ~~~~~~~~~~~~~~
-        
-        ::
-        
-            git clone https://github.com/bbusenius/MMM_Savings_Rate.git
-            python3 setup.py develop 
-        
-        or
-        
-        ::
-        
-            pip install -e git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
-        
-        Using the application
-        ---------------------
-        
-        In order to get things going, you'll only need to take the following
-        steps:
-        
-        1. Setup a directory of .csv files with the financial data needed to run
-           the simulation.
-        2. Configuration:
-        
-        -  Create an account-config.ini with player information.
-        -  Create a config.ini with personal settings and column mappings.
-        
-        3. Run the simulation command with a path to your configuration files.
-        
-        Read on to see how to do each of these things.
-        
-        Spreadsheet files
-        ~~~~~~~~~~~~~~~~~
-        
-        MMM\_Savings\_Rate was designed to be flexible in order to work with
-        your preexisting spreadsheets. At the moment, spreadsheets must be saved
-        as .csv files, however, column headers can be unique, so it doesn't
-        matter what labels you use to categorize things. To get started you'll
-        need financial data for both **income** and **savings**.
-        
-        This data can exist in a single spreadsheet with a variety of financial
-        data or separate spreadsheets for income and savings. How you set it up
-        is up to you, however, certain data is required. The application will
-        allow you to map your column labels to fields, so you don't have to name
-        them the same as outlined here. You also might want to split some of
-        these fields over multiple columns in your spreadsheet. Jump to the
-        configuration section to learn how to do this. In any event, however you
-        decide to enter the data in your spreadsheet, all of the following
-        fields must be represented in some fashion.
-        
-        -  **Date for pay** - the date of your paycheck or date associated with
-           the income being entered. The application can parse most date
-           formats.
-        -  **Gross Pay** - the amount of money you made in its entirety before
-           taxes were withdrawn.
-        -  **Employer Match** - money contributed to a retirement plan by your
-           employer.
-        -  **Taxes and Fees** - any taxes and fees taken out of your paycheck
-           before it was delivered, e.g. OASDI, Medicare, etc.
-        -  **Savings Accounts** - a dollar amount (mapped to 1 or multiple
-           accounts)
-        -  **Date for savings** - the date you saved money into each account.
-        
-        *Note about "Savings Accounts": you might have multiple savings
-        accounts, e.g. Bank Account, Vanguard Brokerage, Roth. Each one of these
-        would contain a dollar amount representing the quantity of money saved
-        for the month. Mapping will be handled in the configuration stage.*
-        
-        `For example spreadsheets please look in the csv
-        directory <https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv>`__.
-        This should give you a good idea of how to lay things out.
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        
-        In order to run the simulation the following two files are required:
-        
-        1. account-config.ini - the configuration for the players. Think of this
-           as a listing of users. Each user has an id, name, and a link to his
-           or her personal configuration.
-        2. config.ini - the configuration for the main user. Think of this as
-           all of your personal settings.
-        
-        *Optional, "enemy" config files can be named however you like, e.g.
-        config-spouse.ini. These should be setup in a similar fashion as
-        config.ini and they should be listed as pipe separated groupings under
-        "enemies" in account-config.ini.*
-        
-        account-config.ini
-        ^^^^^^^^^^^^^^^^^^
-        
-        A file must exist with the name account-config.ini. An example
-        account-config.ini might look like this:
-        
-        ::
-        
-            [Users]
-            ; Unique ID, name, and config file name for user.
-            self = 1,My name,config.ini
-        
-            ; Unique ID, name, and pipe separated list of config 
-            ; file names for user's enemies.
-            enemies = 2,Joe,config-spouse.ini|3,Brother,config-brother.ini
-        
-        The [Users] section is required. The "self" field represents the main
-        player (you). This field should contain a comma separated list with a
-        unique numerical ID, followed by a name, and the name of a main user
-        config file.
-        
-        The "enemies" field is optional. If it's being used, it should be setup
-        the same as the self field, however, if more than one enemy exists, this
-        can be a pipe separated list of comma separated values.
-        
-        config.ini
-        ^^^^^^^^^^
-        
-        The config.ini file is the second configuration file. This file is
-        required. It contains all of your personal settings and spreadsheet
-        mappings.
-        
-        `Please look at this
-        example <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/config/config-example.ini>`__.
-        
-        The majority of what's here is listed under [Sources]. Settings include:
-        
-        -  **pay** - a full path to your income .csv file.
-        -  **pay\_date** - the name of a column header for the dates of income
-           or pay transactions.
-        -  **savings** - a full path to your savings .csv file (can be the same
-           file used for pay).
-        -  **savings\_date** - the name of a column header for the dates of
-           income or pay transactions.
-        -  **gross\_income** - the name of a column header in your spreadsheet
-           that represents gross pay.
-        -  **employer\_match** - the name of a column header in your spreadsheet
-           that represents your employer match.
-        -  **taxes\_and\_fees** - the names of column headers in your
-           spreadsheet that contain taxes and fees.
-        -  **savings\_accounts** - the names of column headers in your
-           spreadsheet that contain savings data from an account or accounts.
-        -  **war** - allows you to show or hide, "enemy" plots on your graph.
-           Set this to, "off" if you only want to see your own data.
-        
-        Settings under [Graph] allow you to change the size of the plot that's
-        generated. *Note: Mint integration is not yet operational*.
-        
-        Running the simulation
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        Once you have your .csv and your config files ready to go, you can run
-        the application. Just open a terminal and type the command:
-        
-        ::
-        
-            savingsrates -p /home/joeconsumer/Documents/Code/Projects/MMM_Savings_Rate/config/
-        
-        The -p flag should specify the full path to your directory of config
-        files. When you run the command a plot of your monthly savings rates
-        should open in a browser window.
-        
-        Requirements
-        ------------
-        
-        This utility runs on python 3.4. All additional dependencies should be
-        automatically downloaded and included during installation. If you'd like
-        to see all of what will be installed look at
-        `setup.py <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py>`__
-        or
-        `requirements.txt <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt>`__.
-        
 Platform: UNKNOWN
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# MMM Savings Rate
+
+MMM Savings Rate is a tool that allows users to calculate and track their monthly savings rates over time. It was developed using functions from the [FI module](https://github.com/bbusenius/FI) and plots savings rates using [Bokeh](https://bokeh.org/). Users simply enter their savings and income data into a spreadsheet. Unique spreadsheet column headers are mapped to the application through user configuration files, allowing the utility to be used with any custom spreadsheet. When the simulation runs, the user's monthly savings rates are plotted on a line graph.
+
+![Example savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png)
+
+Users may also supply secondary, "enemy" spreadsheets. This feature is provided to make the experience fun, game-like, and competitive for people who prefer such an experience. If an enemy spreadsheet is provided, the enemy savings rates are plotted alongside those of the main user. This feature is optional.
+
+*MMM Savings Rate was inspired by Mr. Money Mustache. Visit the Mr. Money Mustache website and [read this article to learn more](http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement).*
+
+## Installation
+This package should generally be installed using pip.
+
+### For users 
+
+```
+pip install git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
+```
+### For developers
+
+```
+pip install -e git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
+```
+## Setting up the application
+
+In order to get things going, you'll only need to take the following steps:
+
+1. Setup a directory of spreadsheet files with the financial data needed to run the simulation.
+2. Configuration:
+  - Create an account-config.ini with user information.
+  - Create a config.ini with personal settings and column mappings.
+3. Run the simulation command with a path to your configuration files.
+
+### Spreadsheet files
+MMM Savings Rate was designed to be flexible in order to work with a variety of spreadsheets. At the moment, spreadsheets must be saved as .xlsx or .csv files, however, column headers can be unique, so it doesn't matter what labels you use to categorize things. To get started you'll need financial data for both **income** and **savings**.
+
+This data can exist in a single spreadsheet with other financial data or it can exist in separate spreadsheets. How you set it up is your choice, however, certain data is required. The application will allow you to map your column labels to fields, so you don't have to name them the same as outlined here. You also might want to split some of these fields over multiple columns in your spreadsheet. Jump to the configuration section to learn how to do this. However you decide to enter the data in your spreadsheet, all of the following fields must be represented in some fashion.
+
+- **Date for pay** - the date of your paycheck or date associated with the income being entered. The application can parse most date formats.
+- **Gross Pay** - the amount of money you made in its entirety before taxes were withdrawn.
+- **Employer Match** - money contributed to a retirement plan by your employer.
+- **Taxes and Fees** - any taxes and fees taken out of your paycheck before it was delivered, e.g. FICA, Medicare, etc.
+- **Savings Accounts** - a dollar amount (mapped to 1 or multiple accounts)
+- **Date for savings** - the date you saved money into each account.
+
+*Note about "Savings Accounts": you might have multiple savings accounts, e.g. Bank Account, Vanguard Brokerage, Roth. Each one of these would contain a dollar amount representing the quantity of money saved for the month. Mapping will be handled in the configuration stage.*
+
+[For example spreadsheets please look in the csv directory](https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv). This should give you a good idea of how to lay things out.
+
+### Configuration
+
+In order to run the simulation the following two files are required:
+
+1. account-config.ini - the configuration for users. Think of this as a listing of users. Each user has an id, name, and a link to his or her personal configuration.
+2. config.ini - the configuration for the main user. Think of this as all of your personal settings.
+
+*Optional, "enemy" config files can be named however you like, e.g. config-spouse.ini. These should be setup in a similar fashion as config.ini and they should be listed as pipe separated groupings under "enemies" in account-config.ini.*
+
+#### account-config.ini
+A file must exist with the name `account-config.ini`. An example account-config.ini might look like this:
+
+```
+[Users]
+; Unique ID, name, and config file name for user.
+self = 1,My name,config.ini
+
+; Unique ID, name, and pipe separated list of config
+; file names for user's enemies.
+enemies = 2,Joe,config-spouse.ini|3,Brother,config-brother.ini
+```
+
+The `[Users]` section is required. The "self" field represents the main user (you). This field should contain a comma separated list with a unique numerical ID, followed by a name, and the name of a main user config file.
+
+The "enemies" field is optional. If it's being used, it should be setup the same as the self field, however, if more than one enemy exists, this can be a pipe separated list of comma separated values.
+
+#### config.ini
+The `config.ini` file is the second configuration file. This file is required. It contains all of your personal settings and spreadsheet mappings.
+
+[Please look at this example](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/config/config-example.ini).
+
+##### Main settings
+
+The majority of the main settings are listed under `[Sources]`. Settings include:
+
+- **pay** - a full path to your income spreadsheet.
+- **pay_date** - the name of a column header for the dates of income or payment transactions.
+- **savings** - a full path to your savings spreadsheet (can be the same file used for pay).
+- **savings_date** - the name of a column header for the dates of income or payment transactions.
+- **gross_income** - the name of a column header in your spreadsheet representing gross pay.
+- **employer_match** - the name of a column header in your spreadsheet that represents your employer match.
+- **taxes_and_fees** - the names of column headers in your spreadsheet containing taxes and fees.
+- **savings_accounts** - the names of column headers in your spreadsheet that contain savings data from an investment account or accounts.
+- **goal** - optional setting that allows you to set a savings rate goal that you're trying to reach.
+- **war** - allows you to show or hide, "enemy" plots on your graph. Set this to, "off" if you only want to see your own data.
+
+##### Graph settings
+
+Settings under `[Graph]` allow you to change the width and height of the plot that's generated (though plots are generally responsive).
+
+##### Additional settings
+
+###### US Average Savings Rates from FRED
+
+Optional settings allow you to plot the average US savings rates alongside your own. This data comes from the Federal Reserve Economic Data (FRED) at the Federal Reserve Bank of St. Louis.
+
+- **fred_url** - the url of the FRED API endpoint.
+- **fred_api_key** - an API token to use FRED.
+
+In order to use these settings, you will need to sign up for an account with FRED and request an API token. This takes about 5 minutes and [can be done on their website](https://fred.stlouisfed.org/docs/api/api_key.html).
+
+Once you enable FRED, you will be able to see how your savings rates dominate the US average*.
+
+![US average savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/FRED.png)
+
+*US average savings rates calculated by FRED are generated after removing outlays from personal income. Since outlays include purchases of durable and non-durable goods, these savings rates are inflated. Even so, as a Mustachian you will easily beat these averages.
+
+###### Notes and goal
+
+If you want to annotate points on your plot with text from your spreadsheet, you can map a `notes` field. This should match a column header on your spreadsheet. If you're using separate spreadsheets for savings and income, the application will look for the same column name in both spreadsheets and de-dupe duplicate notes for the same month while displaying all notes from both spreadsheets for the same month if they're unique.
+
+- **notes** - the name of a column header that maps to notes or special events that you want to show on your plot.
+
+A goal can be added to your plot as well.
+
+- **goal** - numeric value of a savings rate goal you'd like to reach, e.g. 70.
+
+![Savings rates plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/notes.png)
+
+###### % FI
+
+If you want to plot your progress towards FI as a percentage of your FI number, you can enable this with the following settings in your `config.ini`:
+
+- **fi_number** - your FI number.
+- **total_balances** - a spreadsheet heading that maps to a column where you track the total monthly balance of all your accounts.
+- **percent_fi_notes** - a spreadsheet heading that maps to a column with text that you want to show on the % FI plot. Entries will appear as event dots on the plot and will display tooltips with the notes on hover.
+
+This doesn't take into account liabilities so, if you have them, you can just as easily map these configurations to a column that tracks net worth.
+
+![Percent FI plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/percent-fi-notes.png)
+
+### Running the simulation
+
+Once you have your spreadsheet and your configuration files ready to go, you can run the application. Just open a terminal and type the command:
+
+```
+savingsrates -p /home/joe_mustachian/Documents/Code/Projects/MMM_Savings_Rate/config/
+```
+The -p flag should specify the full path to your directory of configuration files. When you run the command a plot of your monthly savings rates should open in a browser window.
+
+## Requirements
+
+This utility runs on python 3.x. All additional dependencies should be automatically downloaded and included during installation. If you'd like to see all of what will be installed look at [setup.py](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py) and [requirements.txt](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt).
+
+## Running tests
+
+```
+python3 -m unittest discover tests -p 'test_*.py'
+```
+
+
```

### Comparing `MMM_Savings_Rate-0.4/config/config-uzia.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-missing-values.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = /home/brad/Documents/Code/Projects/MMM_Savings_Rate/csv/income-uzia.csv
+pay = csv/income-example.csv
 
 ; Spreadsheet column name that mapps to a date for an
 ; income or pay transaction.
 pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
@@ -14,42 +14,53 @@
 ; A .csv column header used for tracking an employer retirement plan match.
 employer_match = Employer Match
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
-taxes_and_fees = Social Security Tax,Medicare,Federal Withholding,State Tax 
+taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = /home/brad/Documents/Code/Projects/MMM_Savings_Rate/csv/savings-uzia.csv
+; Path to .csv file with information about savings.
+savings = csv/savings-example.csv
+
+; A coma separated list of column names from the savings .csv file. These are
+; the column names used to track savings
+savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
 
 ; Spreadsheet column name that mapps to a date for a 
 ; savings transaction.
 savings_date = Date
 
-; A coma separated list of column names from the savings .csv file. These are
-; the column names used to track savings
-savings_accounts = Chase Savings
-
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
+; Whether or not to show the running average
+;show_average = true
 
-; Username for mint.com
-username = bradb@neomailbox.ch
+; Settings for enabling the display of average US savings rates from FRED:
+; The Federal Reserve Bank of St. Louis. Both fred_url and fred_api_key must be
+; present. You can get a FRED api_key here: https://fred.stlouisfed.org/docs/api/api_key.html.
+;fred_url = https://fred-test.com
+;fred_api_key = test-api-key
+
+; Spreadsheet column that maps to notes or special events that you want to
+; show on your plot.
+;notes = Notes
+
+; An aspirational savings rate goal you are trying to hit.
+;goal = 70
 
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = 19453249:UChicagb
+; FI number
+;fi_number = 750000
 
+; Total account balances
+;total_balances = Balances
+
+; % FI plot annotation column header
+;percent_fi_notes = Total Balance Notes
 
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
-
```

### Comparing `MMM_Savings_Rate-0.4/config/config-example.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-test-blank-csv.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Sources]
 
 ; Path to .csv file with information about income listed in chronological 
 ; order with the oldest entry listed first and the newest entry listed last.
-pay = /home/username/Documents/csv/income-example.csv
+pay = tests/test_csv/income-blank.csv
 
 ; Spreadsheet column name that mapps to a date for an
 ; income or pay transaction.
 pay_date = Date
 
 ; A .csv column header used for tracking gross pay.
 gross_income = Gross Pay
@@ -16,39 +16,26 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = OASDI,Medicare,Federal Withholding,State Tax 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
-savings = /home/username/Documents/csv/savings-example.csv
-
-; Spreadsheet column name that mapps to a date for a 
-; savings transaction.
-savings_date = Date
+; Path to .csv file with information about savings.
+savings = tests/test_csv/savings-blank.csv
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
 
+; Spreadsheet column name that mapps to a date for a 
+; savings transaction.
+savings_date = Date
+
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
-
-; Username for mint.com
-username = user@email.com
-
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Scottrade,Vanguard 403b,Vanguard Roth
-
-
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/config/config-joe.ini` & `MMM_Savings_Rate-1.0/tests/test_config/config-joe-test.ini`

 * *Files 14% similar despite different names*

```diff
@@ -16,40 +16,27 @@
 
 ; A coma separated list of column names from the pay .csv file. These should 
 ; be the columns used to determine taxes and fees as part of the take home pay
 ; equation. See http://www.mrmoneymustache.com/2015/01/26/calculating-net-worth/
 ; for more information.
 taxes_and_fees = Federal Tax,State Tax,Professional Fees 
 
-; Path to .csv file with information about savings or "mint"
-; if the information is to be retrieved from mint.com.
+; Path to .csv file with information about savings.
 savings = /home/username/Documents/csv/savings-joe.csv
 
 ; Spreadsheet column name that mapps to a date for a 
 ; savings transaction.
 savings_date = Date
 
 ; A coma separated list of column names from the savings .csv file. These are
 ; the column names used to track savings
 savings_accounts = Savings Account
 
 ; Setting for determining if the user would like to plot his or her savings rate
 ; against enemies. Accepts "on" and "off" as possible values.
 war = on
 
-[Mint]
-; Upon running the application for the first time with the "savings" 
-; source set to mint, the application will attempt to store your 
-; password in your computer's system keyring.  
-
-; Username for mint.com
-username = joe@email.com
-
-; A colon separated list of accounts used to track savings in mint.
-savings_accounts = Savings Account
-
-
 [Graph]
 ; Width of the graph figure
 width = 1898
 height = 900
```

### Comparing `MMM_Savings_Rate-0.4/PKG-INFO` & `MMM_Savings_Rate-1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,226 +1,158 @@
-Metadata-Version: 1.0
-Name: MMM_Savings_Rate
-Version: 0.4
-Summary: An application that can parse spreadsheets in order to calculate and plot a user's monthly savings rate over time. 
-Home-page: https://github.com/bbusenius/MMM_Savings_Rate.git
-Author: Brad Busenius
-Author-email: bbusenius@gmail.com
-License: GNU GPLv3, see LICENSE.txt
-Description: MMM\_Savings\_Rate
-        ==================
-        
-        This application is a command-line utility that allows users to
-        calculate and track their monthly savings rates over time. Users simply
-        enter their savings and income data into a spreadsheet saved as a .csv.
-        Unique spreadsheet column headers are mapped to the application through
-        user configuration files, allowing the utility to be used with any
-        custom spreadsheet. When the simulation is run, user monthly savings
-        rates are plotted on a line graph.
-        
-        .. figure:: https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png
-           :alt: Example savings rates plotted
-        
-           Example savings rates plotted
-        
-        Additionally, users may supply secondary, "enemy" spreadsheets. This
-        feature is provided in order to make the experience fun, game-like, and
-        competitive for those who prefer such an experience. If an enemy
-        spreadsheet is provided, the enemy savings rates are plotted alongside
-        those of the user. This feature might be used by spouses who wish to
-        compete with each other, for example.
-        
-        *MMM\_Savings\_Rate was inspired by Mr. Money Mustache. Visit the Mr.
-        Money Mustache website and `read this article to learn
-        more <http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement>`__.*
-        
-        Web version
-        -----------
-        
-        Though MMM\_Savings\_Rate is meant to be run from the command-line, a
-        full, graphical, web-based version of the project exists at:
-        https://savingsratewars.com/. Use the web-based version of the software
-        if you don't want to deal with installation and configuration.
-        
-        Installation
-        ------------
-        
-        This package should generally be installed using pip.
-        
-        For users
-        ~~~~~~~~~
-        
-        ::
-        
-            pip install MMM-Savings-Rate
-        
-        For developers
-        ~~~~~~~~~~~~~~
-        
-        ::
-        
-            git clone https://github.com/bbusenius/MMM_Savings_Rate.git
-            python3 setup.py develop 
-        
-        or
-        
-        ::
-        
-            pip install -e git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
-        
-        Using the application
-        ---------------------
-        
-        In order to get things going, you'll only need to take the following
-        steps:
-        
-        1. Setup a directory of .csv files with the financial data needed to run
-           the simulation.
-        2. Configuration:
-        
-        -  Create an account-config.ini with player information.
-        -  Create a config.ini with personal settings and column mappings.
-        
-        3. Run the simulation command with a path to your configuration files.
-        
-        Read on to see how to do each of these things.
-        
-        Spreadsheet files
-        ~~~~~~~~~~~~~~~~~
-        
-        MMM\_Savings\_Rate was designed to be flexible in order to work with
-        your preexisting spreadsheets. At the moment, spreadsheets must be saved
-        as .csv files, however, column headers can be unique, so it doesn't
-        matter what labels you use to categorize things. To get started you'll
-        need financial data for both **income** and **savings**.
-        
-        This data can exist in a single spreadsheet with a variety of financial
-        data or separate spreadsheets for income and savings. How you set it up
-        is up to you, however, certain data is required. The application will
-        allow you to map your column labels to fields, so you don't have to name
-        them the same as outlined here. You also might want to split some of
-        these fields over multiple columns in your spreadsheet. Jump to the
-        configuration section to learn how to do this. In any event, however you
-        decide to enter the data in your spreadsheet, all of the following
-        fields must be represented in some fashion.
-        
-        -  **Date for pay** - the date of your paycheck or date associated with
-           the income being entered. The application can parse most date
-           formats.
-        -  **Gross Pay** - the amount of money you made in its entirety before
-           taxes were withdrawn.
-        -  **Employer Match** - money contributed to a retirement plan by your
-           employer.
-        -  **Taxes and Fees** - any taxes and fees taken out of your paycheck
-           before it was delivered, e.g. OASDI, Medicare, etc.
-        -  **Savings Accounts** - a dollar amount (mapped to 1 or multiple
-           accounts)
-        -  **Date for savings** - the date you saved money into each account.
-        
-        *Note about "Savings Accounts": you might have multiple savings
-        accounts, e.g. Bank Account, Vanguard Brokerage, Roth. Each one of these
-        would contain a dollar amount representing the quantity of money saved
-        for the month. Mapping will be handled in the configuration stage.*
-        
-        `For example spreadsheets please look in the csv
-        directory <https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv>`__.
-        This should give you a good idea of how to lay things out.
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        
-        In order to run the simulation the following two files are required:
-        
-        1. account-config.ini - the configuration for the players. Think of this
-           as a listing of users. Each user has an id, name, and a link to his
-           or her personal configuration.
-        2. config.ini - the configuration for the main user. Think of this as
-           all of your personal settings.
-        
-        *Optional, "enemy" config files can be named however you like, e.g.
-        config-spouse.ini. These should be setup in a similar fashion as
-        config.ini and they should be listed as pipe separated groupings under
-        "enemies" in account-config.ini.*
-        
-        account-config.ini
-        ^^^^^^^^^^^^^^^^^^
-        
-        A file must exist with the name account-config.ini. An example
-        account-config.ini might look like this:
-        
-        ::
-        
-            [Users]
-            ; Unique ID, name, and config file name for user.
-            self = 1,My name,config.ini
-        
-            ; Unique ID, name, and pipe separated list of config 
-            ; file names for user's enemies.
-            enemies = 2,Joe,config-spouse.ini|3,Brother,config-brother.ini
-        
-        The [Users] section is required. The "self" field represents the main
-        player (you). This field should contain a comma separated list with a
-        unique numerical ID, followed by a name, and the name of a main user
-        config file.
-        
-        The "enemies" field is optional. If it's being used, it should be setup
-        the same as the self field, however, if more than one enemy exists, this
-        can be a pipe separated list of comma separated values.
-        
-        config.ini
-        ^^^^^^^^^^
-        
-        The config.ini file is the second configuration file. This file is
-        required. It contains all of your personal settings and spreadsheet
-        mappings.
-        
-        `Please look at this
-        example <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/config/config-example.ini>`__.
-        
-        The majority of what's here is listed under [Sources]. Settings include:
-        
-        -  **pay** - a full path to your income .csv file.
-        -  **pay\_date** - the name of a column header for the dates of income
-           or pay transactions.
-        -  **savings** - a full path to your savings .csv file (can be the same
-           file used for pay).
-        -  **savings\_date** - the name of a column header for the dates of
-           income or pay transactions.
-        -  **gross\_income** - the name of a column header in your spreadsheet
-           that represents gross pay.
-        -  **employer\_match** - the name of a column header in your spreadsheet
-           that represents your employer match.
-        -  **taxes\_and\_fees** - the names of column headers in your
-           spreadsheet that contain taxes and fees.
-        -  **savings\_accounts** - the names of column headers in your
-           spreadsheet that contain savings data from an account or accounts.
-        -  **war** - allows you to show or hide, "enemy" plots on your graph.
-           Set this to, "off" if you only want to see your own data.
-        
-        Settings under [Graph] allow you to change the size of the plot that's
-        generated. *Note: Mint integration is not yet operational*.
-        
-        Running the simulation
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        Once you have your .csv and your config files ready to go, you can run
-        the application. Just open a terminal and type the command:
-        
-        ::
-        
-            savingsrates -p /home/joeconsumer/Documents/Code/Projects/MMM_Savings_Rate/config/
-        
-        The -p flag should specify the full path to your directory of config
-        files. When you run the command a plot of your monthly savings rates
-        should open in a browser window.
-        
-        Requirements
-        ------------
-        
-        This utility runs on python 3.4. All additional dependencies should be
-        automatically downloaded and included during installation. If you'd like
-        to see all of what will be installed look at
-        `setup.py <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py>`__
-        or
-        `requirements.txt <https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt>`__.
-        
-Platform: UNKNOWN
+# MMM Savings Rate
+
+MMM Savings Rate is a tool that allows users to calculate and track their monthly savings rates over time. It was developed using functions from the [FI module](https://github.com/bbusenius/FI) and plots savings rates using [Bokeh](https://bokeh.org/). Users simply enter their savings and income data into a spreadsheet. Unique spreadsheet column headers are mapped to the application through user configuration files, allowing the utility to be used with any custom spreadsheet. When the simulation runs, the user's monthly savings rates are plotted on a line graph.
+
+![Example savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/screenshot.png)
+
+Users may also supply secondary, "enemy" spreadsheets. This feature is provided to make the experience fun, game-like, and competitive for people who prefer such an experience. If an enemy spreadsheet is provided, the enemy savings rates are plotted alongside those of the main user. This feature is optional.
+
+*MMM Savings Rate was inspired by Mr. Money Mustache. Visit the Mr. Money Mustache website and [read this article to learn more](http://www.mrmoneymustache.com/2012/01/13/the-shockingly-simple-math-behind-early-retirement).*
+
+## Installation
+This package should generally be installed using pip.
+
+### For users 
+
+```
+pip install git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
+```
+### For developers
+
+```
+pip install -e git+https://github.com/bbusenius/MMM_Savings_Rate.git#egg=mmm_savings_rate
+```
+## Setting up the application
+
+In order to get things going, you'll only need to take the following steps:
+
+1. Setup a directory of spreadsheet files with the financial data needed to run the simulation.
+2. Configuration:
+  - Create an account-config.ini with user information.
+  - Create a config.ini with personal settings and column mappings.
+3. Run the simulation command with a path to your configuration files.
+
+### Spreadsheet files
+MMM Savings Rate was designed to be flexible in order to work with a variety of spreadsheets. At the moment, spreadsheets must be saved as .xlsx or .csv files, however, column headers can be unique, so it doesn't matter what labels you use to categorize things. To get started you'll need financial data for both **income** and **savings**.
+
+This data can exist in a single spreadsheet with other financial data or it can exist in separate spreadsheets. How you set it up is your choice, however, certain data is required. The application will allow you to map your column labels to fields, so you don't have to name them the same as outlined here. You also might want to split some of these fields over multiple columns in your spreadsheet. Jump to the configuration section to learn how to do this. However you decide to enter the data in your spreadsheet, all of the following fields must be represented in some fashion.
+
+- **Date for pay** - the date of your paycheck or date associated with the income being entered. The application can parse most date formats.
+- **Gross Pay** - the amount of money you made in its entirety before taxes were withdrawn.
+- **Employer Match** - money contributed to a retirement plan by your employer.
+- **Taxes and Fees** - any taxes and fees taken out of your paycheck before it was delivered, e.g. FICA, Medicare, etc.
+- **Savings Accounts** - a dollar amount (mapped to 1 or multiple accounts)
+- **Date for savings** - the date you saved money into each account.
+
+*Note about "Savings Accounts": you might have multiple savings accounts, e.g. Bank Account, Vanguard Brokerage, Roth. Each one of these would contain a dollar amount representing the quantity of money saved for the month. Mapping will be handled in the configuration stage.*
+
+[For example spreadsheets please look in the csv directory](https://github.com/bbusenius/MMM_Savings_Rate/tree/master/csv). This should give you a good idea of how to lay things out.
+
+### Configuration
+
+In order to run the simulation the following two files are required:
+
+1. account-config.ini - the configuration for users. Think of this as a listing of users. Each user has an id, name, and a link to his or her personal configuration.
+2. config.ini - the configuration for the main user. Think of this as all of your personal settings.
+
+*Optional, "enemy" config files can be named however you like, e.g. config-spouse.ini. These should be setup in a similar fashion as config.ini and they should be listed as pipe separated groupings under "enemies" in account-config.ini.*
+
+#### account-config.ini
+A file must exist with the name `account-config.ini`. An example account-config.ini might look like this:
+
+```
+[Users]
+; Unique ID, name, and config file name for user.
+self = 1,My name,config.ini
+
+; Unique ID, name, and pipe separated list of config
+; file names for user's enemies.
+enemies = 2,Joe,config-spouse.ini|3,Brother,config-brother.ini
+```
+
+The `[Users]` section is required. The "self" field represents the main user (you). This field should contain a comma separated list with a unique numerical ID, followed by a name, and the name of a main user config file.
+
+The "enemies" field is optional. If it's being used, it should be setup the same as the self field, however, if more than one enemy exists, this can be a pipe separated list of comma separated values.
+
+#### config.ini
+The `config.ini` file is the second configuration file. This file is required. It contains all of your personal settings and spreadsheet mappings.
+
+[Please look at this example](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/config/config-example.ini).
+
+##### Main settings
+
+The majority of the main settings are listed under `[Sources]`. Settings include:
+
+- **pay** - a full path to your income spreadsheet.
+- **pay_date** - the name of a column header for the dates of income or payment transactions.
+- **savings** - a full path to your savings spreadsheet (can be the same file used for pay).
+- **savings_date** - the name of a column header for the dates of income or payment transactions.
+- **gross_income** - the name of a column header in your spreadsheet representing gross pay.
+- **employer_match** - the name of a column header in your spreadsheet that represents your employer match.
+- **taxes_and_fees** - the names of column headers in your spreadsheet containing taxes and fees.
+- **savings_accounts** - the names of column headers in your spreadsheet that contain savings data from an investment account or accounts.
+- **goal** - optional setting that allows you to set a savings rate goal that you're trying to reach.
+- **war** - allows you to show or hide, "enemy" plots on your graph. Set this to, "off" if you only want to see your own data.
+
+##### Graph settings
+
+Settings under `[Graph]` allow you to change the width and height of the plot that's generated (though plots are generally responsive).
+
+##### Additional settings
+
+###### US Average Savings Rates from FRED
+
+Optional settings allow you to plot the average US savings rates alongside your own. This data comes from the Federal Reserve Economic Data (FRED) at the Federal Reserve Bank of St. Louis.
+
+- **fred_url** - the url of the FRED API endpoint.
+- **fred_api_key** - an API token to use FRED.
+
+In order to use these settings, you will need to sign up for an account with FRED and request an API token. This takes about 5 minutes and [can be done on their website](https://fred.stlouisfed.org/docs/api/api_key.html).
+
+Once you enable FRED, you will be able to see how your savings rates dominate the US average*.
+
+![US average savings rates plotted](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/FRED.png)
+
+*US average savings rates calculated by FRED are generated after removing outlays from personal income. Since outlays include purchases of durable and non-durable goods, these savings rates are inflated. Even so, as a Mustachian you will easily beat these averages.
+
+###### Notes and goal
+
+If you want to annotate points on your plot with text from your spreadsheet, you can map a `notes` field. This should match a column header on your spreadsheet. If you're using separate spreadsheets for savings and income, the application will look for the same column name in both spreadsheets and de-dupe duplicate notes for the same month while displaying all notes from both spreadsheets for the same month if they're unique.
+
+- **notes** - the name of a column header that maps to notes or special events that you want to show on your plot.
+
+A goal can be added to your plot as well.
+
+- **goal** - numeric value of a savings rate goal you'd like to reach, e.g. 70.
+
+![Savings rates plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/notes.png)
+
+###### % FI
+
+If you want to plot your progress towards FI as a percentage of your FI number, you can enable this with the following settings in your `config.ini`:
+
+- **fi_number** - your FI number.
+- **total_balances** - a spreadsheet heading that maps to a column where you track the total monthly balance of all your accounts.
+- **percent_fi_notes** - a spreadsheet heading that maps to a column with text that you want to show on the % FI plot. Entries will appear as event dots on the plot and will display tooltips with the notes on hover.
+
+This doesn't take into account liabilities so, if you have them, you can just as easily map these configurations to a column that tracks net worth.
+
+![Percent FI plotted with annotations](https://github.com/bbusenius/MMM_Savings_Rate/raw/master/docs/percent-fi-notes.png)
+
+### Running the simulation
+
+Once you have your spreadsheet and your configuration files ready to go, you can run the application. Just open a terminal and type the command:
+
+```
+savingsrates -p /home/joe_mustachian/Documents/Code/Projects/MMM_Savings_Rate/config/
+```
+The -p flag should specify the full path to your directory of configuration files. When you run the command a plot of your monthly savings rates should open in a browser window.
+
+## Requirements
+
+This utility runs on python 3.x. All additional dependencies should be automatically downloaded and included during installation. If you'd like to see all of what will be installed look at [setup.py](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/setup.py) and [requirements.txt](https://github.com/bbusenius/MMM_Savings_Rate/blob/master/requirements.txt).
+
+## Running tests
+
+```
+python3 -m unittest discover tests -p 'test_*.py'
+```
```

### Comparing `MMM_Savings_Rate-0.4/sr_launcher.py` & `MMM_Savings_Rate-1.0/sr_launcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# MMM Savings Rate is an application that can parse spreadsheets and  
-# use the data to calculate and plot a user's savings rate over time. 
+# MMM Savings Rate is an application that can parse spreadsheets and
+# use the data to calculate and plot a user's savings rate over time.
 # The application was inspired by Mr. Money Mustache and it uses his
 # methodology to make the calculations.
 
 # Copyright (C) 2016 Brad Busenius
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -11,40 +11,41 @@
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
-# along with this program.  If not, see 
+# along with this program.  If not, see
 # <https://www.gnu.org/licenses/gpl-3.0.html/>.
 
 import argparse
-from savings_rate import SRConfig, SavingsRate, Plot
+
+from savings_rate import Plot, SavingsRate, SRConfig
+
 
 def run():
     """
-    Run the application in, "ini" mode.
+    Run the application.
 
     Args:
-        config_path: string, path to a directory of config 
+        config_path: string, path to a directory of config
         .ini files. Should include a trailing "/".
     """
     # Capture commandline arguments. prog='' argument must
     # match the command name in setup.py entry_points
     parser = argparse.ArgumentParser(prog='savingsrates')
     parser.add_argument('-p', nargs='?', help='A path to a directory of config files.')
     args = parser.parse_args()
     inputs = {'p': args.p}
     config_path = inputs['p']
 
     # Instantiate a savings rate config object
-    config = SRConfig('ini', config_path, 'config.ini')
+    config = SRConfig(config_path, 'config.ini')
 
     # Instantiate a savings rate object for a user
     savings_rate = SavingsRate(config)
     monthly_rates = savings_rate.get_monthly_savings_rates()
 
     # Plot the user's savings rate
     user_plot = Plot(savings_rate)
     user_plot.plot_savings_rates(monthly_rates)
-
```

