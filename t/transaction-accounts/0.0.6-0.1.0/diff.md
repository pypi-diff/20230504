# Comparing `tmp/transaction-accounts-0.0.6.tar.gz` & `tmp/transaction-accounts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.0.6.tar", last modified: Sun Apr 23 15:22:45 2023, max compression
+gzip compressed data, was "transaction-accounts-0.1.0.tar", last modified: Thu May  4 11:57:41 2023, max compression
```

## Comparing `transaction-accounts-0.0.6.tar` & `transaction-accounts-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.482520 transaction-accounts-0.0.6/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.6/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-04-23 15:22:45.482666 transaction-accounts-0.0.6/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.478129 transaction-accounts-0.0.6/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.6/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)     7401 2023-04-23 14:17:53.000000 transaction-accounts-0.0.6/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10924 2023-04-23 14:19:31.000000 transaction-accounts-0.0.6/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-23 15:22:45.483187 transaction-accounts-0.0.6/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7614 2023-04-23 15:22:39.000000 transaction-accounts-0.0.6/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.480202 transaction-accounts-0.0.6/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     3254 2023-04-23 14:51:14.000000 transaction-accounts-0.0.6/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)      982 2023-04-23 03:03:07.000000 transaction-accounts-0.0.6/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.6/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2242 2023-04-23 14:55:48.000000 transaction-accounts-0.0.6/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.6/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.482223 transaction-accounts-0.0.6/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.830059 transaction-accounts-0.1.0/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.0/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-04 11:57:41.830221 transaction-accounts-0.1.0/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.820908 transaction-accounts-0.1.0/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.0/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.0/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    21470 2023-05-03 04:40:24.000000 transaction-accounts-0.1.0/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.0/accounts/utility.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-04 11:57:41.830803 transaction-accounts-0.1.0/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7614 2023-05-01 09:44:05.000000 transaction-accounts-0.1.0/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.827565 transaction-accounts-0.1.0/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.0/tests/test_calendar.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.0/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.0/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     4250 2023-05-03 04:48:05.000000 transaction-accounts-0.1.0/tests/test_loanGiven.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.0/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.0/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.0/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-04 11:57:41.829691 transaction-accounts-0.1.0/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-04 11:57:41.000000 transaction-accounts-0.1.0/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.0.6/LICENSE.txt` & `transaction-accounts-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.6/PKG-INFO` & `transaction-accounts-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.6
+Version: 0.1.0
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

### Comparing `transaction-accounts-0.0.6/accounts/metadata.py` & `transaction-accounts-0.1.0/accounts/metadata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from calendar import monthrange
-from dataclasses import dataclass, field
 from datetime import date
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional, Dict
 from pydantic import BaseModel
 
+from accounts.utility import CustomEncoder
+
 
 class TransactionOperation(Enum):
     CREDIT = 'credit'
     DEBIT = 'debit'
     SET = 'set'
 
 
@@ -43,53 +44,94 @@
 
 
 class PositionType(BaseModel):
     name: str
     label: str
 
 
+class DateType(BaseModel):
+    name: str
+    label: str
+    required: bool = True
+
+
 class RateTier(BaseModel):
     from_amount: Decimal
     to_amount: Decimal
     rate: Decimal
 
 
 class RateType(BaseModel):
     name: str
     label: str
-    rate_tiers: List[RateTier] = []
+    rate_tiers: Dict[str, List[RateTier]] = {}
 
-    def add_tier(self, to_amount: Decimal, rate: Decimal):
-        rate_tier = RateTier(from_amount=self.get_max_to_amount(), to_amount=to_amount, rate=rate)
-        self.rate_tiers.append(rate_tier)
+    class Config:
+        json_encoders = {Dict: CustomEncoder()}
 
-    def get_max_to_amount(self):
-        if len(self.rate_tiers) == 0:
+    @staticmethod
+    def __get_key(value_date):
+        return value_date.strftime("%Y-%m-%d")
+
+    def add_tier(self, value_date: date, to_amount: Decimal, rate: Decimal):
+        key = self.__get_key(value_date)
+        if key not in self.rate_tiers:
+            self.rate_tiers[key] = []
+
+        rate_tier = RateTier(from_amount=self.get_max_to_amount(value_date), to_amount=to_amount, rate=rate)
+        self.rate_tiers[key].append(rate_tier)
+
+    def get_max_to_amount(self, value_date: date):
+        key = self.__get_key(value_date)
+        if key not in self.rate_tiers:
             return Decimal(0)
 
-        max_value = max(self.rate_tiers, key=lambda tier: tier.to_amount)
+        rate_tiers = self.rate_tiers[key]
+
+        if len(rate_tiers) == 0:
+            return Decimal(0)
+
+        max_value = max(rate_tiers, key=lambda tier: tier.to_amount)
         return max_value.to_amount
 
-    def get_rate(self, amount: Decimal):
-        rate_tier = next(rt for rt in self.rate_tiers if rt.from_amount <= amount <= rt.to_amount)
+    def __get_tiers(self, value_date) -> List[RateTier]:
+        # find first date that is less than or equal to value_date
+        key = self.__get_key(value_date)
+        dates = [d for d in self.rate_tiers.keys() if d <= key]
+        if len(dates) == 0:
+            raise Exception(f"No rate tiers found for date {str(value_date)} in rate table {self.name}")
+        index_date = max(dates)
+        return self.rate_tiers[index_date]
+
+    def get_rate(self, value_date: date, amount: Decimal) -> Decimal:
+        applicable_tiers = (rt for rt in self.__get_tiers(value_date) if rt.from_amount <= amount <= rt.to_amount)
+
+        # if no tiers are applicable, raise an exception
+        rate_tier = next(applicable_tiers, None)
+        if rate_tier is None:
+            if amount < Decimal(0):
+                return Decimal(0)
+            else:
+                raise Exception(
+                    f"No rate tiers found for amount {str(amount)} on date {str(value_date)} in rate table {self.name}")
 
         return rate_tier.rate
 
     def get_daily_fee(self, users: Decimal, value_date: date):
         _, days_in_month = monthrange(value_date.year, value_date.month)
-        monthly_fee = Decimal(self.get_fee(Decimal(0), users))
+        monthly_fee = Decimal(self.get_fee(value_date, Decimal(0), users))
         return monthly_fee / Decimal(days_in_month)
 
-    def get_fee(self, from_amount: Decimal, to_amount: Decimal):
+    def get_fee(self, value_date: date, from_amount: Decimal, to_amount: Decimal):
         processed = from_amount
         fee = Decimal(0)
 
         exit_loop = False
 
-        for rate_tier in self.rate_tiers:
+        for rate_tier in self.__get_tiers(value_date):
             if rate_tier.from_amount <= processed < rate_tier.to_amount:
                 part_processed = rate_tier.to_amount - processed
 
                 if to_amount < rate_tier.to_amount:
                     part_processed = to_amount - processed
                     exit_loop = True
 
@@ -107,14 +149,15 @@
     position_type_name: str
 
 
 class TransactionType(BaseModel):
     name: str
     label: str
     position_rules: List[PositionRule] = []
+    maximum_precision: bool = False
 
     def add_position_rule(self, transaction_operation: TransactionOperation, position_type: PositionType):
         self.position_rules.append(PositionRule(operation=transaction_operation, position_type_name=position_type.name))
         return self
 
 
 class ScheduleType(BaseModel):
@@ -125,14 +168,15 @@
     business_day_adjustment: BusinessDayAdjustment
     interval_expression: str
     start_date_expression: str
     end_date_expression: str = None
     number_of_repeats_expression: str = None
     include_dates_expression: str = None
     exclude_dates_expression: str = None
+    editable: bool = True
 
 
 class ScheduledTransaction(BaseModel):
     schedule_name: str
     timing: ScheduledTransactionTiming
     generated_transaction_type: str
     amount_expression: str
@@ -145,35 +189,53 @@
 
 
 class PropertyType(BaseModel):
     name: str
     label: str
     data_type: DataType
     required: bool = True
+    value_dated: bool = False
+
+
+class InstalmentType(BaseModel):
+    name: str
+    label: str
+    timing: ScheduledTransactionTiming
+    schedule_name: str
+    transaction_type: str
+    property_name: str
+    solve_for_zero_position: str
+    solve_for_date: str
 
 
 class AccountType(BaseModel):
     name: str
     label: str
     transaction_types: List[TransactionType] = []
     position_types: List[PositionType] = []
+    date_types: List[DateType] = []
     rate_types: Dict[str, RateType] = {}
     triggered_transactions: List[TriggeredTransaction] = []
     schedule_types: List[ScheduleType] = []
     property_types: List[PropertyType] = []
     scheduled_transactions: List[ScheduledTransaction] = []
-    triggered_transactions: List[TriggeredTransaction] = []
+    instalment_type: InstalmentType = None
 
     def add_property_type(self, name: str, label: str, data_type: DataType, required: bool = True) -> PropertyType:
         property_type = PropertyType(name=name, label=label, data_type=data_type.value, required=required)
         self.property_types.append(property_type)
         return property_type
 
-    def add_transaction_type(self, name: str, label: str) -> TransactionType:
-        transaction_type = TransactionType(name=name, label=label)
+    def add_date_type(self, name: str, label: str) -> DateType:
+        date_type = DateType(name=name, label=label)
+        self.date_types.append(date_type)
+        return date_type
+
+    def add_transaction_type(self, name: str, label: str, maximum_precision: bool = False) -> TransactionType:
+        transaction_type = TransactionType(name=name, label=label, maximum_precision=maximum_precision)
         self.transaction_types.append(transaction_type)
         return transaction_type
 
     def add_position_type(self, name: str, label: str) -> PositionType:
         position_type = PositionType(name=name, label=label)
         self.position_types.append(position_type)
         return position_type
@@ -206,17 +268,25 @@
     def get_rate_type(self, rate_type_name: str):
         return next(rt for rt in self.rate_types if rt.name == rate_type_name)
 
     def get_trigger_transaction(self, trigger_transaction_type_name: str) -> Optional[TriggeredTransaction]:
         return next((tt for tt in self.triggered_transactions if
                      tt.trigger_transaction_type_name == trigger_transaction_type_name), None)
 
-
+    def add_instalment_type(self, name: str, label: str, timing: ScheduledTransactionTiming,
+                            transaction_type: str, property_name: str,
+                            solve_for_zero_position: str, solve_for_date: str,
+                            schedule_name: str) -> InstalmentType:
+
+        instalment_type = InstalmentType(name=name, label=label, timing=timing,
+                                         transaction_type=transaction_type,
+                                         property_name=property_name,
+                                         schedule_name=schedule_name,
+                                         solve_for_zero_position=solve_for_zero_position,
+                                         solve_for_date=solve_for_date)
+        self.instalment_type = instalment_type
 
     def __getattr__(self, method_name):
         if method_name in self.rate_types:
             return self.rate_types[method_name]
         else:
             raise AttributeError(f'No such attribute: {method_name}')
-
-
-
```

### Comparing `transaction-accounts-0.0.6/setup.py` & `transaction-accounts-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.0.6',
+    version='0.1.0',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction accounts.
```

### Comparing `transaction-accounts-0.0.6/tests/test_configuration.py` & `transaction-accounts-0.1.0/tests/test_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-
+import yaml
 from accounts.metadata import *
 from tests.test_config import create_savings_account
 
 
 class TestConfiguration(unittest.TestCase):
     def test_serialize(self):
         account_type = create_savings_account()
@@ -19,23 +19,23 @@
         self.assertEqual(text, text2)
 
 
 class RateTest(unittest.TestCase):
     def test_get_max_when_empy(self):
         rate_type = RateType(name='rates', label='Rates')
 
-        max_value = rate_type.get_max_to_amount()
+        max_value = rate_type.get_max_to_amount(value_date=date(2019, 7, 1))
 
         self.assertEqual(Decimal(0), max_value)
 
     def test_get_max_when_non_empy(self):
         rate_type = RateType(name='rates', label='Rates')
 
-        rate_type.add_tier(Decimal(100), Decimal(5))
+        rate_type.add_tier(date(2019, 1, 1), Decimal(100), Decimal(5))
 
-        max_value = rate_type.get_max_to_amount()
+        max_value = rate_type.get_max_to_amount(date(2019, 1, 1))
 
         self.assertEqual(Decimal(100), max_value)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `transaction-accounts-0.0.6/tests/test_schedule.py` & `transaction-accounts-0.1.0/tests/test_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TestSchedule(unittest.TestCase):
     start_date = date(2013, 3, 8)
     end_date = start_date + relativedelta(years=+25)
 
     def __get_daily_schedule(self, start_date: date, end_date: date, end_type: ScheduleEndType):
-        return Schedule(start_date= start_date,end_type= end_type,frequency= ScheduleFrequency.DAILY, interval=1,
+        return Schedule(start_date=start_date, end_type=end_type, frequency=ScheduleFrequency.DAILY, interval=1,
                         adjustement=BusinessDayAdjustment.NO_ADJUSTMENT, end_date=end_date)
 
     def test_daily_schedule_no_end_tests(self):
         accrual_schedule = self.__get_daily_schedule(self.start_date, self.end_date, ScheduleEndType.NO_END)
 
         accrual_dates = accrual_schedule.get_all_dates(self.end_date);
 
@@ -24,16 +24,17 @@
         self.assertEqual(accrual_schedule.is_due(self.end_date), True)
 
         self.assertEqual(accrual_schedule.is_due(self.start_date + relativedelta(days=-1)), False)
         self.assertEqual(accrual_schedule.is_due(self.end_date + relativedelta(days=+1)), True)
 
     def test_monthly_schedule(self):
         interest_start = date(2013, 3, 31)
-        schedule = Schedule(start_date=interest_start, end_type=ScheduleEndType.END_DATE, frequency=ScheduleFrequency.MONTHLY,
-                            interval=1,end_date=self.end_date)
+        schedule = Schedule(start_date=interest_start, end_type=ScheduleEndType.END_DATE,
+                            frequency=ScheduleFrequency.MONTHLY,
+                            interval=1, end_date=self.end_date)
 
         schedule.exclude_dates.append(date(2013, 12, 31))
         schedule.include_dates.append(self.end_date)
 
         interest_dates = schedule.get_all_dates(self.end_date)
 
         self.assertEqual(schedule.adjustment, BusinessDayAdjustment.NO_ADJUSTMENT)
@@ -64,15 +65,15 @@
 
         self.assertEqual(accrual_schedule.is_due(self.start_date + relativedelta(days=-1)), False)
         self.assertEqual(accrual_schedule.is_due(self.end_date + relativedelta(days=+1)), False)
 
     def test_monthly_repeats_schedule(self):
         start_date = date(2019, 12, 1)
         discount_schedule = Schedule(start_date=start_date, end_type=ScheduleEndType.END_REPEATS,
-                                     frequency= ScheduleFrequency.MONTHLY, interval=1,
+                                     frequency=ScheduleFrequency.MONTHLY, interval=1,
                                      adjustment=BusinessDayAdjustment.NO_ADJUSTMENT, number_of_repeats=3)
 
         discount_dates = discount_schedule.get_all_dates(self.end_date)
 
         self.assertEqual(len(discount_dates), 3)
         self.assertEqual(date(2020, 2, 1), discount_dates[2])
```

### Comparing `transaction-accounts-0.0.6/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.1.0/transaction_accounts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.6
+Version: 0.1.0
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

