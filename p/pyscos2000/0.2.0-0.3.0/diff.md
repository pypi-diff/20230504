# Comparing `tmp/pyscos2000-0.2.0.tar.gz` & `tmp/pyscos2000-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscos2000-0.2.0.tar", last modified: Tue Apr 18 06:43:22 2023, max compression
+gzip compressed data, was "pyscos2000-0.3.0.tar", last modified: Thu May  4 05:29:34 2023, max compression
```

## Comparing `pyscos2000-0.2.0.tar` & `pyscos2000-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-02-23 13:34:11.000000 pyscos2000-0.2.0/LICENSE
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      958 2023-02-23 13:33:27.000000 pyscos2000-0.2.0/README.md
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.571408 pyscos2000-0.2.0/pyscos2000/
--rw-r--r--   0 robertl   (1000) robertl   (1000)      653 2022-10-07 13:50:33.000000 pyscos2000-0.2.0/pyscos2000/__init__.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2550 2022-10-05 07:22:54.000000 pyscos2000-0.2.0/pyscos2000/browser.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     3195 2022-10-04 10:09:36.000000 pyscos2000-0.2.0/pyscos2000/checker.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    10518 2022-11-24 11:41:57.000000 pyscos2000-0.2.0/pyscos2000/concrete.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    10646 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/instance.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     6327 2023-01-26 11:48:30.000000 pyscos2000-0.2.0/pyscos2000/parametertypes.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1203 2022-09-23 08:00:41.000000 pyscos2000-0.2.0/pyscos2000/reporter.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    11907 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/schema.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    48311 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/scos2000.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1005 2022-10-07 13:50:15.000000 pyscos2000-0.2.0/pyscos2000/shared.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2035 2022-09-23 08:09:36.000000 pyscos2000-0.2.0/pyscos2000/synthetic.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)       21 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/version.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/pyscos2000.egg-info/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      541 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/SOURCES.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/dependency_links.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       56 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/entry_points.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       29 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/requires.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       11 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/top_level.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)      977 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/setup.cfg
--rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2022-08-16 13:42:40.000000 pyscos2000-0.2.0/setup.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/tests/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     3845 2023-04-17 14:14:58.000000 pyscos2000-0.2.0/tests/test_capcalib.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-02-23 13:34:11.000000 pyscos2000-0.3.0/LICENSE
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      958 2023-02-23 13:33:27.000000 pyscos2000-0.3.0/README.md
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/pyscos2000/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      653 2022-10-07 13:50:33.000000 pyscos2000-0.3.0/pyscos2000/__init__.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2550 2022-10-05 07:22:54.000000 pyscos2000-0.3.0/pyscos2000/browser.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3195 2022-10-04 10:09:36.000000 pyscos2000-0.3.0/pyscos2000/checker.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    10518 2022-11-24 11:41:57.000000 pyscos2000-0.3.0/pyscos2000/concrete.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    10861 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/pyscos2000/instance.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    10217 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/pyscos2000/parametertypes.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1203 2022-09-23 08:00:41.000000 pyscos2000-0.3.0/pyscos2000/reporter.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    11957 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/pyscos2000/schema.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    50714 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/pyscos2000/scos2000.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1005 2022-10-07 13:50:15.000000 pyscos2000-0.3.0/pyscos2000/shared.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2035 2022-09-23 08:09:36.000000 pyscos2000-0.3.0/pyscos2000/synthetic.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       21 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/pyscos2000/version.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/pyscos2000.egg-info/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      565 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/SOURCES.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/dependency_links.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       56 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/entry_points.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       29 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/requires.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       11 2023-05-04 05:29:34.000000 pyscos2000-0.3.0/pyscos2000.egg-info/top_level.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      977 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/setup.cfg
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2022-08-16 13:42:40.000000 pyscos2000-0.3.0/setup.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-05-04 05:29:34.218932 pyscos2000-0.3.0/tests/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3844 2023-05-04 05:28:57.000000 pyscos2000-0.3.0/tests/test_capcalib.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3880 2023-04-20 18:01:33.000000 pyscos2000-0.3.0/tests/test_esoccalib.py
```

### Comparing `pyscos2000-0.2.0/LICENSE` & `pyscos2000-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/PKG-INFO` & `pyscos2000-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscos2000
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python SCOS-2000 parsing and checking
 Home-page: https://gitlab.irf.se/irf/pyscos2000
 Author: Robert Labudda
 Author-email: robert.labudda@irf.se
 License: MIT
 Keywords: SCOS-2000,ESA
 Classifier: Intended Audience :: Developers
```

### Comparing `pyscos2000-0.2.0/README.md` & `pyscos2000-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/__init__.py` & `pyscos2000-0.3.0/pyscos2000/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/browser.py` & `pyscos2000-0.3.0/pyscos2000/browser.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/checker.py` & `pyscos2000-0.3.0/pyscos2000/checker.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/concrete.py` & `pyscos2000-0.3.0/pyscos2000/concrete.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/instance.py` & `pyscos2000-0.3.0/pyscos2000/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """SCOS Table instance classes"""
 import csv
 
 
 class TableCell:
     """A cell in an SCOS table"""
-    def __init__(self, table, column, rawvalue):
+    def __init__(self, table, column, row, rawvalue):
         self.table = table
         self.column = column
+        self.row = row
         assert column in self.table.definition.columns
 
         self.columnidx = self.table.definition.columns.index(column)
         self.rawvalue = rawvalue
         if len(rawvalue) > 0:
             self._value = column.type.parse(rawvalue)
         else:
@@ -200,22 +201,27 @@
                 reader = csv.reader(tabbed, dialect=CSVDialect)
                 self._parse_from_reader(reader)
         return self
 
     def _parse_from_reader(self, reader):
         """Parse the rows from the given csv.reader instance"""
         for linenr, row in enumerate(reader):
-            self.rows.append(self.ROW_TYPE(self, linenr+1))
+            tablerow = self.create_row(linenr+1)
+            self.rows.append(tablerow)
             for columnidx, field in enumerate(row):
                 column = self.definition.columns[columnidx]
-                self.rows[-1].append(self.create_cell(column, field))
+                tablerow.append(self.create_cell(column, tablerow, field))
 
-    def create_cell(self, column, field):
+    def create_cell(self, column, row, field):
         """Return a new instance of ``CELL_TYPE`` for this column"""
-        return self.CELL_TYPE(self, column, field)
+        return self.CELL_TYPE(self, column, row, field)
+
+    def create_row(self, linenr):
+        """Return a new instance of ``ROW_TYPE`` for this line"""
+        return self.ROW_TYPE(self, linenr)
 
     def can_merge(self, other):
         """Whether or not the ``other`` table's content can be merged
 
         Conditions are:
 
         - no clashing entries in the primary keys
```

### Comparing `pyscos2000-0.2.0/pyscos2000/reporter.py` & `pyscos2000-0.3.0/pyscos2000/reporter.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/schema.py` & `pyscos2000-0.3.0/pyscos2000/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,27 @@
 class Radix(enum.Enum):
     """The radix of an unsigned integer value's text representation"""
     UNDEFINED = None
     DECIMAL = 'D'
     HEXADECIMAL = 'H'
     OCTAL = 'O'
 
-    def convert(self, text):
-        """Convert the given text to an unsigned int given this radix"""
+    def radix(self):
+        """Return the radix value"""
         if self == Radix.DECIMAL:
-            return int(text)
+            return 10
         if self == Radix.HEXADECIMAL:
-            return int(text, 16)
+            return 16
         if self == Radix.OCTAL:
-            return int(text, 0)
-        raise ValueError(f"Cannot interprete {text} with radix {self}")
+            return 8
+        raise ValueError(f"Unspecified radix {self}")
+
+    def convert(self, text):
+        """Convert the given text to an unsigned int given this radix"""
+        return int(text, self.radix())
 
 
 class LimitInterpretation(enum.Enum):
     """What value to use to interprete limit values"""
 
     UNCALIBRATED = 'U'
     """Use RAW values"""
@@ -530,8 +534,8 @@
                             if column.is_key]
         self.columnnames = [c.name for c in self.columns]
         self.filename = self.name + '.dat'
 
     @property
     def has_primary_key(self):
         """Whether or not a primary key is defined"""
-        return len(self.primary_key) > 0
+        return len(self.primary_key) > 0
```

### Comparing `pyscos2000-0.2.0/pyscos2000/scos2000.py` & `pyscos2000-0.3.0/pyscos2000/scos2000.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     MonitoringCheckFlagColumn, PacketHeaderElementTypeColumn, PlannableColumn,
     CommandVerificationColumn, CommandInputFormatColumn, CommandCategoryColumn,
     CommandInterlockColumn, DisplayFormatColumn, IntegerFormatTypeColumn,
     TimeTagTypeColumn, PlannableBySourceColumn, StandaloneExecutionColumn,
     SequenceElementTypeColumn, ReleaseTimeTypeColumn, RelativePositionColumn,
     CommandSequenceInterlockColumn, ValueEditableColumn, CommandElementTypeColumn,
     ValueSourceColumn, FormatParameterTypeColumn, CommandValueRepresentationColumn,
+    CommandElementType, CommandValueRepresentation, Radix,
     )
 from .parametertypes import ParameterType, SignedIntegerParameter, UnsignedIntegerParameter
 from .synthetic import DynamicSyntheticParameter
 
 
 class SyntheticImplementationMissingError(RuntimeError):
     """Raised when the implementation of a synthetic parameter is missing"""
@@ -531,15 +532,15 @@
 class CSPTable(TableDefinition):
     """The csp.dat table in SCOS
 
     Command sequence formal parameters"""
     def __init__(self):
         super().__init__('csp', [
             ColumnDefinition('CSP_SQNAME', String(8), optional=False, is_key=True),
-            ColumnDefinition('CSP_FPQNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CSP_FPNAME', String(8), optional=False, is_key=True),
             ColumnDefinition('CSP_FPNUM', Number(8), optional=False),
             ColumnDefinition('CSP_DESCR', String(23), optional=True),
             ColumnDefinition('CSP_PTC', Number(2), optional=False),
             ColumnDefinition('CSP_PFC', Number(5), optional=False),
             ColumnDefinition('CSP_DISPFMT', CommandInputFormatColumn(),
                              optional=True, default='R'),
             ColumnDefinition('CSP_RADIX', RadixColumn(), optional=True, default='D'),
@@ -706,18 +707,79 @@
 
     class PCFNatureCell(TableCell):
         @property
         def is_synthetic(self):
             return self.table.definition.is_synthetic(self.value)
 
     class PCFTableInstance(Table):
-        def create_cell(self, column, field):
+        def create_cell(self, column, row, field):
             if column.name == 'PCF_NATUR':
-                return SCOS.PCFNatureCell(self, column, field)
-            return super().create_cell(column, field)
+                return SCOS.PCFNatureCell(self, column, row, field)
+            return super().create_cell(column, row, field)
+
+    class CDFValueCell(TableCell):
+        def interprete(self):
+            """Return the value interpreted using CDF_PTC and CDF_PFC"""
+            if self.value is None:
+                return None
+
+            if self.row['CDF_ELTYPE'] == CommandElementType.FIXED:
+                value = int(self.value, 16)
+                if value < 0:
+                    # TODO - extract this into a checker
+                    raise RuntimeError("Negative value")
+                return value
+
+            if self.row['CDF_INTER'] == CommandValueRepresentation.ENGINEERING:
+                return self.value
+
+            cpc = self.table.cpc.get(self.row['CDF_PNAME'])
+            assert cpc is not None  # TODO - move this into a checker
+            base = cpc['CPC_RADIX']
+            if base != Radix.UNDEFINED:
+                base = base.radix()
+            else:
+                base = None
+
+            type_ = ParameterType.resolve((self.row['CDF_PTC'].value,
+                                           self.row['CDF_PFC'].value))
+
+            return type_.parse(self.value, base=base)
+
+    class CDFTableInstance(Table):
+        def create_cell(self, column, row, field):
+            if column.name == 'CDF_VALUE':
+                return SCOS.CDFValueCell(self, column, row, field)
+            return super().create_cell(column, row, field)
+
+    class CPCDefaultValueCell(TableCell):
+        def interprete(self):
+            """Return the default value interpreted using CPC_PTC and CPC_PFC"""
+            if self.value is None:
+                return None
+
+            if self.row['CDF_INTER'] == CommandValueRepresentation.ENGINEERING:
+                return self.value
+
+            base = self.row['CPC_RADIX']
+            if base != Radix.UNDEFINED:
+                base = base.radix
+            else:
+                base = None
+
+            type_ = ParameterType.resolve((self.row['CPC_PTC'].value,
+                                           self.row['CPC_PFC'].value))
+
+            return type_.parse(self.value, base=base)
+
+    class CPCTableInstance(Table):
+        def create_cell(self, column, row, field):
+            if column.name == 'CPC_DEFVAL':
+                return SCOS.CPCDefaultValueCell(self, column, row, field)
+            return super().create_cell(column, row, field)
 
     def __init__(self, path):
         """Instantiate from the SCOS-2000 definition at ``path``.
 
         ``path`` may either be a folder with the ``.dat`` files or
         a ``.zip`` file containing the ``.dat`` files.
         """
@@ -756,16 +818,16 @@
             # TODO 'ppf': Table(self, PPFTable()).parse(),
             # TODO 'ppc': Table(self, PPCTable()).parse(),
             'tcp': Table(self, TCPTable()).parse(),
             'pcpc': Table(self, PCPCTable()).parse(),
             'pcdf': Table(self, PCDFTable()).parse(),
             'ccf': Table(self, CCFTable()).parse(),
             'dst': Table(self, DSTTable()).parse(),
-            'cpc': Table(self, CPCTable()).parse(),
-            'cdf': Table(self, CDFTable()).parse(),
+            'cpc': SCOS.CPCTableInstance(self, CPCTable()).parse(),
+            'cdf': SCOS.CDFTableInstance(self, CDFTable()).parse(),
             'ptv': Table(self, PTVTable()).parse(),
             'csf': Table(self, CSFTable()).parse(),
             'css': Table(self, CSSTable()).parse(),
             'sdf': Table(self, SDFTable()).parse(),
             'csp': Table(self, CSPTable()).parse(),
             # TODO 'cvs': Table(self, CVSTable()).parse(),
             # TODO 'cve': Table(self, CVETable()).parse(),
@@ -1085,8 +1147,8 @@
     ACCEPTED_TABLES = (PLFTable,)
 
     def check_row(self, row):
         if row['PLF_NBOCC'].value == 1 and not self.pedantic:
             return
         tdocc = row['PLF_TDOCC'].value
         if not (0 < tdocc <= 4080000):
-            self.error(f"Invalid TDOCC parameter value {tdocc}")
+            self.error(f"Invalid TDOCC parameter value {tdocc}")
```

### Comparing `pyscos2000-0.2.0/pyscos2000/shared.py` & `pyscos2000-0.3.0/pyscos2000/shared.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000/synthetic.py` & `pyscos2000-0.3.0/pyscos2000/synthetic.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/pyscos2000.egg-info/PKG-INFO` & `pyscos2000-0.3.0/pyscos2000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscos2000
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python SCOS-2000 parsing and checking
 Home-page: https://gitlab.irf.se/irf/pyscos2000
 Author: Robert Labudda
 Author-email: robert.labudda@irf.se
 License: MIT
 Keywords: SCOS-2000,ESA
 Classifier: Intended Audience :: Developers
```

### Comparing `pyscos2000-0.2.0/pyscos2000.egg-info/SOURCES.txt` & `pyscos2000-0.3.0/pyscos2000.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 pyscos2000/version.py
 pyscos2000.egg-info/PKG-INFO
 pyscos2000.egg-info/SOURCES.txt
 pyscos2000.egg-info/dependency_links.txt
 pyscos2000.egg-info/entry_points.txt
 pyscos2000.egg-info/requires.txt
 pyscos2000.egg-info/top_level.txt
-tests/test_capcalib.py
+tests/test_capcalib.py
+tests/test_esoccalib.py
```

### Comparing `pyscos2000-0.2.0/setup.cfg` & `pyscos2000-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.2.0/tests/test_capcalib.py` & `pyscos2000-0.3.0/tests/test_capcalib.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,8 +104,8 @@
         self.assertEqual(packet['PCF02'].eng, 2.5)
 
     def test_extrapolate2(self):
         """Test a succeeding extrapolation (below lower)"""
         packet = TestablePacket(self.scos, 15,
                                 [('PCF02', b'\x00')])
         self.assertEqual(packet['PCF02'].raw, 0)
-        self.assertTrue(abs(packet['PCF02'].eng + 1.6666) < 0.0001)
+        self.assertTrue(abs(packet['PCF02'].eng + 1.6666) < 0.0001)
```

