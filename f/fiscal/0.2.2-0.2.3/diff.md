# Comparing `tmp/fiscal-0.2.2.tar.gz` & `tmp/fiscal-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiscal-0.2.2.tar", max compression
+gzip compressed data, was "fiscal-0.2.3.tar", max compression
```

## Comparing `fiscal-0.2.2.tar` & `fiscal-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1499 2022-12-17 18:51:42.541405 fiscal-0.2.2/LICENSE
--rw-r--r--   0        0        0     5378 2023-02-09 15:50:04.076666 fiscal-0.2.2/README.md
--rw-r--r--   0        0        0       79 2023-02-10 07:02:04.895322 fiscal-0.2.2/fiscal/__init__.py
--rw-r--r--   0        0        0      919 2023-02-10 07:09:33.665593 fiscal-0.2.2/fiscal/abstract_bands.py
--rw-r--r--   0        0        0      906 2023-02-10 07:32:07.491871 fiscal-0.2.2/fiscal/abstract_liability.py
--rw-r--r--   0        0        0     1526 2023-02-10 07:33:34.120191 fiscal-0.2.2/fiscal/allocators.py
--rw-r--r--   0        0        0      271 2022-12-28 09:44:45.569068 fiscal-0.2.2/fiscal/bands.py
--rw-r--r--   0        0        0      571 2022-12-29 12:59:23.629727 fiscal-0.2.2/fiscal/liability.py
--rw-r--r--   0        0        0      430 2023-02-10 07:02:54.003129 fiscal-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 fiscal-0.2.2/setup.py
--rw-r--r--   0        0        0     5778 1970-01-01 00:00:00.000000 fiscal-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1499 2022-12-17 18:51:42.541405 fiscal-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5378 2023-02-09 15:50:04.076666 fiscal-0.2.3/README.md
+-rw-r--r--   0        0        0       79 2023-02-10 07:02:04.895322 fiscal-0.2.3/fiscal/__init__.py
+-rw-r--r--   0        0        0      919 2023-02-10 07:09:33.665593 fiscal-0.2.3/fiscal/abstract_bands.py
+-rw-r--r--   0        0        0      906 2023-02-10 07:32:07.491871 fiscal-0.2.3/fiscal/abstract_liability.py
+-rw-r--r--   0        0        0     1526 2023-02-10 07:33:34.120191 fiscal-0.2.3/fiscal/allocators.py
+-rw-r--r--   0        0        0      271 2022-12-28 09:44:45.569068 fiscal-0.2.3/fiscal/bands.py
+-rw-r--r--   0        0        0      571 2022-12-29 12:59:23.629727 fiscal-0.2.3/fiscal/liability.py
+-rw-r--r--   0        0        0      475 2023-05-04 20:37:55.917314 fiscal-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 fiscal-0.2.3/setup.py
+-rw-r--r--   0        0        0     5821 1970-01-01 00:00:00.000000 fiscal-0.2.3/PKG-INFO
```

### Comparing `fiscal-0.2.2/LICENSE` & `fiscal-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/README.md` & `fiscal-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/fiscal/abstract_bands.py` & `fiscal-0.2.3/fiscal/abstract_bands.py`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/fiscal/abstract_liability.py` & `fiscal-0.2.3/fiscal/abstract_liability.py`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/fiscal/allocators.py` & `fiscal-0.2.3/fiscal/allocators.py`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/fiscal/liability.py` & `fiscal-0.2.3/fiscal/liability.py`

 * *Files identical despite different names*

### Comparing `fiscal-0.2.2/setup.py` & `fiscal-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['pytest>=7.2.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'fiscal',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': '',
     'long_description': '# Fiscal\n## A simple, systematic tax liability calculator\n\nFiscal is a simple, systematic tax calculator with soft-coded rate bands.  Specifically, Fiscal aims to side-step the commonly-seen behaviour of using \'if\' statements in tax calculators, and relying on hard-coded tax bands. \n\n### Fiscal, broken down\n\nThere are two key elements to Fiscal.\n\n1) Bands - a stream of pairwise tuples (a threshold, a percentage) with an \'allocator\'. The allocator dictates the manner in which taxable amounts are allocated between the threshold element of each band - the two predominant forms of allocator are provided:\n    - \'step\', which reflects the most common allocation; and \n    - \'slab\', which represents taxes for which the sole applicable rate is determined by the taxable amount (as in old stamp duty and early SDLT).\n\n2) Liabilities - a calculation of liability stored in a \'breakdown\' - a three-element tuple made up of: \n    - the amount allocated to the band;\n    - the percentage referable to that band; and\n    - the product of the amount and the percentage.\n\n## Allocators - examples\nTo draw an example from Stamp Duty Land Tax (SDLT), a land transfer tax in England (and previously throughout the UK).\n\n### SDLT - stepped calculation\n\nThe applicable bands for a commercial transaction were, after 17 March 2017, as follows:\n\n| Threshold | Percentage |\n|-----------|------------|\n| £150,000  | 0%         |\n| £100,000  | 2%         |\n| Surplus   | 5%         |\n\nThis can be represented by a band as follows:\n\n``` python-console\nstepped_bands = SteppedBands(((150_000, 0),(100_000, 2),("Infinity", 5)))\n```\n\n\nThe bands are allocated on the step basis, so £1m would be allocated as follows:\n\n| Threshold | Percentage | Liability |\n|-----------|------------|-----------|\n| £150,000  | 0%         | £0        |\n| £100,000  | 2%         | £2,000    |\n| £750,000  | 5%         | £37,500   |\n\n``` python-console\nallocation = stepped_bands.allocate(1_000_000)\nassert allocation == (\n    (Decimal("150000"), Decimal("0")),\n    (Decimal("100000"), Decimal("2")),\n    (Decimal("750000"), Decimal("5")),\n) # True\n\n```\n\n\nThe allocation is intended to be called within an instance of the Liability object.\n\n\n### SDLT - slabbed calculation\n\nPrior to 17 March 2017, the applicable SDLT rates for a commercial transaction were as follows:\n\n| Threshold | Percentage |\n|-----------|------------|\n| £150,000  | 0%         |\n| £100,000  | 1%         |\n| £250,000  | 3%         |\n| Surplus   | 4%         |\n\nThe bands were allocated on the \'slab\' basis. This means that the taxable amount is compared with the __cumulative__ thresholds, which are as follows:\n\n| Cumulative Threshold | Percentage |\n|----------------------|------------|\n| £150,000             | 0%         |\n| £250,000             | 1%         |\n| £500,000             | 3%         |\n| Surplus              | 4%         |\n\nThe first cumulative threshold to equal or exceed the taxable amount determines the applicable percentage.  So where the taxable amount was £200,000, the applicable percentage was **1%**.\n\n| Cumulative Threshold | Amount   | Percentage |\n|----------------------|----------|------------|\n| £150,000             |          | 0%         |\n| £250,000             | £200,000 | 1%         |\n| £500,000             |          | 3%         |\n| Surplus              |          | 4%         |\n\nWhere the taxable amount was £300,000, the applicable percentage was **3%**.\n\n| Cumulative Threshold | Amount   | Percentage |\n|----------------------|----------|------------|\n| £150,000             |          | 0%         |\n| £250,000             |          | 1%         |\n| £500,000             | £300,000 | 3%         |\n| Surplus              |          | 4%         |\n\nThresholds were inclusive, so where the taxable amount was £500,000, the applicable percentage was still **3%**.\n\n| Cumulative Threshold | Amount   | Percentage |\n|----------------------|----------|------------|\n| £150,000             |          | 0%         |\n| £250,000             |          | 1%         |\n| £500,000             | £500,000 | 3%         |\n| Surplus              |          | 4%         |\n\nBut where the taxable amount was £500,001, the applicable percentage was **4%**.\n\n| Cumulative Threshold | Amount   | Percentage |\n|----------------------|----------|------------|\n| £150,000             |          | 0%         |\n| £250,000             |          | 1%         |\n| £500,000             |          | 3%         |\n| Surplus              | £500,001 | 4%         |\n\n## Liabilities - examples\n\nLiabilities represent the calculation the follows the allocation of a taxable amount into the correct bands. \n\nThose liabilities are then aggregated into a total liability.\nSo by way of example, if calculating the current (9 February 2022) SDLT liability (non-residential property) for a £1m sum, the steps would be as follows.\n\n``` python-console\nbands = SteppedBands((150_000, 0),(100_000, 2),("Infinity", 5))\nliab = Liability(bands=bands, amount=1_000_000)\n```\nThe breakdown of liability would look as below:\n\n``` python-console\nassert liab.breakdown == (\n        (Decimal("150000"), Decimal("0"), Decimal("0")),\n        (Decimal("100000"), Decimal("2"), Decimal("2000")),\n        (Decimal("750000"), Decimal("5"), Decimal("37500")),\n    ) # True\nassert liab.total == Decimal("39500") # True\n```\n',
     'author': 'Chris Nyland',
     'author_email': 'chris.nyland@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/nylnd/fiscal',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.11,<4.0',
 }
```

### Comparing `fiscal-0.2.2/PKG-INFO` & `fiscal-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: fiscal
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
+Home-page: https://github.com/nylnd/fiscal
 License: BSD-3-Clause
 Author: Chris Nyland
 Author-email: chris.nyland@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

