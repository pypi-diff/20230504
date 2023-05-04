# Comparing `tmp/handycsv-4.2.0.tar.gz` & `tmp/handycsv-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handycsv-4.2.0.tar", last modified: Tue May  2 05:20:28 2023, max compression
+gzip compressed data, was "handycsv-4.3.0.tar", last modified: Thu May  4 02:59:26 2023, max compression
```

## Comparing `handycsv-4.2.0.tar` & `handycsv-4.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:20:28.311370 handycsv-4.2.0/
--rw-r-----   0 nic       (1000) nic       (1000)     1525 2023-05-02 02:28:44.000000 handycsv-4.2.0/LICENSE
--rw-r-----   0 nic       (1000) nic       (1000)      131 2023-05-02 02:28:44.000000 handycsv-4.2.0/NOTICE
--rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-02 05:20:28.311370 handycsv-4.2.0/PKG-INFO
--rw-r-----   0 nic       (1000) nic       (1000)       79 2023-05-02 02:28:44.000000 handycsv-4.2.0/README.md
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:20:28.311370 handycsv-4.2.0/handycsv/
--rw-r-----   0 nic       (1000) nic       (1000)     1719 2023-05-02 05:19:48.000000 handycsv-4.2.0/handycsv/__init__.py
--rw-r-----   0 nic       (1000) nic       (1000)     7126 2023-05-02 05:18:18.000000 handycsv-4.2.0/handycsv/column_stats.py
--rw-r-----   0 nic       (1000) nic       (1000)    11533 2023-05-02 04:30:57.000000 handycsv-4.2.0/handycsv/csv.py
--rw-r-----   0 nic       (1000) nic       (1000)    10188 2023-05-02 05:17:16.000000 handycsv-4.2.0/handycsv/grid_stats.py
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:20:28.311370 handycsv-4.2.0/handycsv.egg-info/
--rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-02 05:20:28.000000 handycsv-4.2.0/handycsv.egg-info/PKG-INFO
--rw-r-----   0 nic       (1000) nic       (1000)      311 2023-05-02 05:20:28.000000 handycsv-4.2.0/handycsv.egg-info/SOURCES.txt
--rw-r-----   0 nic       (1000) nic       (1000)        1 2023-05-02 05:20:28.000000 handycsv-4.2.0/handycsv.egg-info/dependency_links.txt
--rw-r-----   0 nic       (1000) nic       (1000)        9 2023-05-02 05:20:28.000000 handycsv-4.2.0/handycsv.egg-info/top_level.txt
--rw-r-----   0 nic       (1000) nic       (1000)       38 2023-05-02 05:20:28.311370 handycsv-4.2.0/setup.cfg
--rw-r-----   0 nic       (1000) nic       (1000)     2473 2023-05-02 02:28:44.000000 handycsv-4.2.0/setup.py
-drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-02 05:20:28.311370 handycsv-4.2.0/test/
--rw-r-----   0 nic       (1000) nic       (1000)     4864 2023-05-02 05:19:33.000000 handycsv-4.2.0/test/test_columnstats.py
--rw-r-----   0 nic       (1000) nic       (1000)    15035 2023-05-02 04:32:57.000000 handycsv-4.2.0/test/test_csv.py
--rw-r-----   0 nic       (1000) nic       (1000)     8587 2023-05-02 05:19:12.000000 handycsv-4.2.0/test/test_gridstats.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-04 02:59:26.061685 handycsv-4.3.0/
+-rw-r-----   0 nic       (1000) nic       (1000)     1525 2023-05-02 02:28:44.000000 handycsv-4.3.0/LICENSE
+-rw-r-----   0 nic       (1000) nic       (1000)      131 2023-05-02 02:28:44.000000 handycsv-4.3.0/NOTICE
+-rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-04 02:59:26.061685 handycsv-4.3.0/PKG-INFO
+-rw-r-----   0 nic       (1000) nic       (1000)       79 2023-05-02 02:28:44.000000 handycsv-4.3.0/README.md
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-04 02:59:26.057685 handycsv-4.3.0/handycsv/
+-rw-r-----   0 nic       (1000) nic       (1000)     1719 2023-05-04 02:57:07.000000 handycsv-4.3.0/handycsv/__init__.py
+-rw-r-----   0 nic       (1000) nic       (1000)     7418 2023-05-03 17:02:59.000000 handycsv-4.3.0/handycsv/column_stats.py
+-rw-r-----   0 nic       (1000) nic       (1000)    11803 2023-05-03 17:01:12.000000 handycsv-4.3.0/handycsv/csv.py
+-rw-r-----   0 nic       (1000) nic       (1000)    10480 2023-05-03 17:02:56.000000 handycsv-4.3.0/handycsv/grid_stats.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-04 02:59:26.061685 handycsv-4.3.0/handycsv.egg-info/
+-rw-r-----   0 nic       (1000) nic       (1000)      238 2023-05-04 02:59:26.000000 handycsv-4.3.0/handycsv.egg-info/PKG-INFO
+-rw-r-----   0 nic       (1000) nic       (1000)      326 2023-05-04 02:59:26.000000 handycsv-4.3.0/handycsv.egg-info/SOURCES.txt
+-rw-r-----   0 nic       (1000) nic       (1000)        1 2023-05-04 02:59:26.000000 handycsv-4.3.0/handycsv.egg-info/dependency_links.txt
+-rw-r-----   0 nic       (1000) nic       (1000)        9 2023-05-04 02:59:26.000000 handycsv-4.3.0/handycsv.egg-info/top_level.txt
+-rw-r-----   0 nic       (1000) nic       (1000)      104 2023-05-04 02:58:40.000000 handycsv-4.3.0/pyproject.toml
+-rw-r-----   0 nic       (1000) nic       (1000)       38 2023-05-04 02:59:26.061685 handycsv-4.3.0/setup.cfg
+-rw-r-----   0 nic       (1000) nic       (1000)     2473 2023-05-02 02:28:44.000000 handycsv-4.3.0/setup.py
+drwxr-x---   0 nic       (1000) nic       (1000)        0 2023-05-04 02:59:26.061685 handycsv-4.3.0/test/
+-rw-r-----   0 nic       (1000) nic       (1000)     5096 2023-05-03 17:10:43.000000 handycsv-4.3.0/test/test_columnstats.py
+-rw-r-----   0 nic       (1000) nic       (1000)    15248 2023-05-04 02:56:41.000000 handycsv-4.3.0/test/test_csv.py
+-rw-r-----   0 nic       (1000) nic       (1000)     8794 2023-05-03 17:10:01.000000 handycsv-4.3.0/test/test_gridstats.py
```

### Comparing `handycsv-4.2.0/LICENSE` & `handycsv-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `handycsv-4.2.0/handycsv/__init__.py` & `handycsv-4.3.0/handycsv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,8 @@
  * POSSIBILITY OF SUCH DAMAGE.
 """
 
 from .column_stats import ColumnStats
 from .csv import Csv
 from .grid_stats import GridStats
 
-__version__ = '4.2.0'
+__version__ = '4.3.0'
```

### Comparing `handycsv-4.2.0/handycsv/column_stats.py` & `handycsv-4.3.0/handycsv/column_stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,24 +87,25 @@
       raise ValueError('ColumnStats must be rectangular')
     if stats.csv.num_columns(0) != 2:
       raise ValueError('ColumnStats have 2 columns per row')
     stats.__init_row_info()
     return stats
 
   @staticmethod
-  def load(text, transpose=False):
+  def load(text, transpose=False, delimiter=','):
     """
     Constructs a ColumnStats from a string
     Values default to int, then float, then str
 
     Args:
       text      (str)  : text of the grid
       transpose (bool) : to transpose the input
+      delimiter (str)  : value separator
     """
-    csv = Csv.load(text, transpose=transpose)
+    csv = Csv.load(text, transpose=transpose, delimiter=delimiter)
     return ColumnStats.make_from_csv(csv)
 
   @staticmethod
   def read(filename, transpose=False):
     """
     Constructs a ColumnStats from a CSV file
     Values default to int, then float, then str
@@ -134,14 +135,23 @@
 
   def __str__(self):
     """
     Returns the string representation in CSV format.
     """
     return str(self.csv)
 
+  def to_string(self, delimiter=','):
+    """
+    Returns the string representation in xSV format.
+
+    Args:
+      delimiter (str) : delimiter for value separation
+    """
+    return self.csv.to_string(delimiter)
+
   def pretty(self, precision=None, right_align=False):
     """
     Returns a pretty string.
     """
     return self.csv.pretty(precision=precision, right_align=right_align)
 
   def write(self, filename, transpose=False):
```

### Comparing `handycsv-4.2.0/handycsv/csv.py` & `handycsv-4.3.0/handycsv/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,32 +67,33 @@
     except ValueError:
       try:
         return float(value)
       except ValueError:
         return str(value)
 
   @staticmethod
-  def load(text, transpose=False):
+  def load(text, transpose=False, delimiter=','):
     """
     Constructs a CSV from a string.
     Values default to int, then float, then str.
 
     Args:
       text (str)       : text of the Csv
       transpose (bool) : to transpose the Csv
+      delimiter (str)  : value separator
     """
     csv = Csv()
     csv.raw = []
 
     # break text into lines
     lines = text.strip().split('\n')
 
     # break lines into raw data (columnar pieces)
     for line in lines:
-      columns = line.split(',')
+      columns = line.split(delimiter)
       columns = [x.strip() for x in columns]
 
       # transform values
       for idx in range(0, len(columns)):
         columns[idx] = Csv.autotype(columns[idx])
 
       # push new row into rows list
@@ -160,18 +161,27 @@
     """
     return self.raw == other.raw
 
   def __str__(self):
     """
     Returns the string representation in CSV format.
     """
-    csv = ''
+    return self.to_string()
+
+  def to_string(self, delimiter=','):
+    """
+    Returns the string representation in xSV format.
+
+    Args:
+      delimiter (str) : delimiter for value separation
+    """
+    xsv = ''
     for row in self.raw:
-      csv += ','.join([str(x) for x in row]) + '\n'
-    return csv
+      xsv += delimiter.join([str(x) for x in row]) + '\n'
+    return xsv
 
   def pretty(self, precision=None, right_align=False):
     """
     Returns a pretty string representation.
 
     Args:
       precision (None or int) : precision of floating point values if specified
```

### Comparing `handycsv-4.2.0/handycsv/grid_stats.py` & `handycsv-4.3.0/handycsv/grid_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,24 +102,25 @@
     if not stats.csv.is_rectangular:
       raise ValueError('GridStats must be rectangular')
     stats.__init_row_info()
     stats.__init_column_info()
     return stats
 
   @staticmethod
-  def load(text, transpose=False):
+  def load(text, transpose=False, delimiter=','):
     """
     Constructs a GridStats from a string
     Values default to int, then float, then str
 
     Args:
       text      (str)  : text of the grid
       transpose (bool) : to transpose the input
+      delimiter (str)  : value separator
     """
-    csv = Csv.load(text, transpose=transpose)
+    csv = Csv.load(text, transpose=transpose, delimiter=delimiter)
     return GridStats.make_from_csv(csv)
 
   @staticmethod
   def read(filename, transpose=False):
     """
     Constructs a GridStats from a CSV file
     Values default to int, then float, then str
@@ -161,14 +162,23 @@
 
   def __str__(self):
     """
     Returns the string representation in CSV format.
     """
     return str(self.csv)
 
+  def to_string(self, delimiter=','):
+    """
+    Returns the string representation in xSV format.
+
+    Args:
+      delimiter (str) : delimiter for value separation
+    """
+    return self.csv.to_string(delimiter)
+
   def pretty(self, precision=None, right_align=False):
     """
     Returns a pretty string.
     """
     return self.csv.pretty(precision=precision, right_align=right_align)
 
   def write(self, filename, transpose=False):
```

### Comparing `handycsv-4.2.0/setup.py` & `handycsv-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `handycsv-4.2.0/test/test_columnstats.py` & `handycsv-4.3.0/test/test_columnstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 import unittest
 import tempfile
 
 
 class TestColumnStats(unittest.TestCase):
 
   @staticmethod
-  def make_str(raw_vals):
-    return ''.join(','.join([str(v) for v in row]) + '\n' for row in raw_vals)
+  def make_str(raw_vals, delimiter=','):
+    return ''.join(delimiter.join([str(v) for v in row]) + '\n'
+                   for row in raw_vals)
 
   k4x2 = [
     ['-', 'a'],
     ['d', 0],
     ['e', 3],
     ['f', 6]
   ]
@@ -131,7 +132,11 @@
     skeleton = handycsv.ColumnStats.create(['-', 'd', 'e', 'f', 'g'])
     stats = handycsv.ColumnStats.load(text)
     stats.add_row('g', 7)
     self.assertEqual(skeleton.row_names(), stats.row_names())
     self.assertEqual(stats.get('g'), 7)
     self.assertEqual(stats.get('e'), 3)
     self.assertEqual(stats.get('f'), 6)
+
+    text = TestColumnStats.make_str(TestColumnStats.k4x2, delimiter=';')
+    stats = handycsv.ColumnStats.load(text, delimiter=';')
+    self.assertEqual(text, stats.to_string(delimiter=';'))
```

### Comparing `handycsv-4.2.0/test/test_csv.py` & `handycsv-4.3.0/test/test_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 import unittest
 import tempfile
 
 
 class TestCsv(unittest.TestCase):
 
   @staticmethod
-  def make_str(raw_vals):
-    return ''.join(','.join([str(v) for v in row]) + '\n' for row in raw_vals)
+  def make_str(raw_vals, delimiter=','):
+    return ''.join(delimiter.join([str(v) for v in row]) + '\n' for row in raw_vals)
 
   def check(self, csv, raw):
     # structure
     self.assertEqual(csv.num_rows(), len(raw))
     for row in range(csv.num_rows()):
       self.assertEqual(csv.num_columns(row), len(raw[row]))
     row_lens = csv.row_lengths()
@@ -214,14 +214,19 @@
     with self.assertRaises(IndexError):
       csv.remove_column(1)
 
     # transpose (again)
     with self.assertRaises(IndexError):
       csv.transpose()
 
+  def test_xsv(self):
+    text = TestCsv.make_str(TestCsv.kIrregular, delimiter=';')
+    csv = handycsv.Csv.load(text, delimiter=';')
+    self.assertEqual(text, csv.to_string(delimiter=';'))
+
   kEmpty = [['']]
 
   def check_empty(self, csv):
     self.check(csv, TestCsv.kEmpty)
 
     # shape
     self.assertTrue(csv.is_rectangular())
```

### Comparing `handycsv-4.2.0/test/test_gridstats.py` & `handycsv-4.3.0/test/test_gridstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 import unittest
 import tempfile
 
 
 class TestGridStats(unittest.TestCase):
 
   @staticmethod
-  def make_str(raw_vals):
-    return ''.join(','.join([str(v) for v in row]) + '\n' for row in raw_vals)
+  def make_str(raw_vals, delimiter=','):
+    return ''.join(delimiter.join([str(v) for v in row]) + '\n' for row in raw_vals)
 
   k4x4 = [
     ['-', 'a', 'b', 'c'],
     ['d', 0, 1, 2],
     ['e', 3, 4, 5],
     ['f', 6, 7, 8]
   ]
@@ -210,7 +210,11 @@
     stats = handycsv.GridStats.load(text)
     stats.add_row('g', {'a': 9, 'b': 8, 'c': 7})
     skeleton = handycsv.GridStats.create('-', ['d', 'e', 'f', 'g'],
                                          ['a', 'b', 'c'])
     self.assertEqual(skeleton.head(), stats.head())
     self.assertEqual(skeleton.row_names(), stats.row_names())
     self.assertEqual(skeleton.column_names(), stats.column_names())
+
+    text = TestGridStats.make_str(TestGridStats.k4x4, delimiter=';')
+    stats = handycsv.GridStats.load(text, delimiter=';')
+    self.assertEqual(text, stats.to_string(delimiter=';'))
```

