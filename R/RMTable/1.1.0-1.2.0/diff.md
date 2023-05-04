# Comparing `tmp/RMTable-1.1.0.tar.gz` & `tmp/RMTable-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMTable-1.1.0.tar", last modified: Tue May 31 15:31:28 2022, max compression
+gzip compressed data, was "dist/RMTable-1.2.0.tar", last modified: Thu May  4 09:01:00 2023, max compression
```

## Comparing `RMTable-1.1.0.tar` & `RMTable-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-05-31 15:31:28.018594 RMTable-1.1.0/
--rw-r--r--   0 cvaneck    (501) staff       (20)     1072 2019-04-22 15:49:25.000000 RMTable-1.1.0/LICENSE
--rw-r--r--   0 cvaneck    (501) staff       (20)     3697 2022-05-31 15:31:28.018025 RMTable-1.1.0/PKG-INFO
--rw-r--r--   0 cvaneck    (501) staff       (20)     2947 2022-05-10 15:43:31.000000 RMTable-1.1.0/README.md
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-05-31 15:31:28.014063 RMTable-1.1.0/RMTable.egg-info/
--rw-r--r--   0 cvaneck    (501) staff       (20)     3697 2022-05-31 15:31:27.000000 RMTable-1.1.0/RMTable.egg-info/PKG-INFO
--rw-r--r--   0 cvaneck    (501) staff       (20)      373 2022-05-31 15:31:27.000000 RMTable-1.1.0/RMTable.egg-info/SOURCES.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)        1 2022-05-31 15:31:27.000000 RMTable-1.1.0/RMTable.egg-info/dependency_links.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)       14 2022-05-31 15:31:27.000000 RMTable-1.1.0/RMTable.egg-info/requires.txt
--rw-r--r--   0 cvaneck    (501) staff       (20)        8 2022-05-31 15:31:27.000000 RMTable-1.1.0/RMTable.egg-info/top_level.txt
-drwxr-xr-x   0 cvaneck    (501) staff       (20)        0 2022-05-31 15:31:28.015984 RMTable-1.1.0/rmtable/
--rw-r--r--   0 cvaneck    (501) staff       (20)       22 2022-05-27 14:57:42.000000 RMTable-1.1.0/rmtable/__init__.py
--rw-r--r--   0 cvaneck    (501) staff       (20)    23377 2022-05-30 14:13:08.000000 RMTable-1.1.0/rmtable/rmtable.py
--rw-r--r--   0 cvaneck    (501) staff       (20)       38 2022-05-31 15:31:28.018797 RMTable-1.1.0/setup.cfg
--rw-r--r--   0 cvaneck    (501) staff       (20)     1548 2022-05-31 15:30:44.000000 RMTable-1.1.0/setup.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.443506 RMTable-1.2.0/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1072 2019-04-22 15:49:25.000000 RMTable-1.2.0/LICENSE
+-rw-r--r--   0 cvaneck    (503) staff       (20)     5151 2023-05-04 09:01:00.443159 RMTable-1.2.0/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4421 2022-07-26 14:25:27.000000 RMTable-1.2.0/README.md
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.428815 RMTable-1.2.0/RMTable.egg-info/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     5151 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)      442 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/SOURCES.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        1 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/dependency_links.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)       14 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/requires.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        8 2023-05-04 09:01:00.000000 RMTable-1.2.0/RMTable.egg-info/top_level.txt
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-05-04 09:01:00.442377 RMTable-1.2.0/rmtable/
+-rw-r--r--   0 cvaneck    (503) staff       (20)       22 2022-05-27 14:57:42.000000 RMTable-1.2.0/rmtable/__init__.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    13769 2023-05-04 00:13:29.000000 RMTable-1.2.0/rmtable/column_standard_v1.3.json
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1748 2023-05-04 00:13:48.000000 RMTable-1.2.0/rmtable/entries_standard_v1.3.json
+-rw-r--r--   0 cvaneck    (503) staff       (20)    25444 2023-03-20 05:27:35.000000 RMTable-1.2.0/rmtable/rmtable.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)       38 2023-05-04 09:01:00.443567 RMTable-1.2.0/setup.cfg
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1548 2023-05-03 23:14:10.000000 RMTable-1.2.0/setup.py
```

### Comparing `RMTable-1.1.0/LICENSE` & `RMTable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RMTable-1.1.0/PKG-INFO` & `RMTable-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: RMTable
-Version: 1.1.0
-Summary: Reading, writing, and manipulating RMTables (radio astronomy Faraday rotation catalogs)
-Home-page: https://github.com/CIRADA-Tools/RMTable
-Maintainer: Cameron Van Eck
-Maintainer-email: cameron.van.eck@utoronto.ca
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # RMTable
 Code to read/write tables of rotation measures following the proposed standard, in Python 3.
 
 ### [Documentation](https://github.com/CIRADA-Tools/RMTable/wiki)
 Detailed documentation, including installation instructions and example code, is available on the wiki linked above.  
 
 ***
@@ -44,20 +23,25 @@
 
 
 
 ***
 
 ### Catalog
 
-The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.0.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.0.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.0.xml.zip)  
+The consolidated catalog, which currently contains 55 819 RMs from 42 catalogs, is available in the consolidated_catalog_* files above or these links: [FITS format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.fits.zip) [TSV format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.tsv.zip) and [VOTable format](https://github.com/CIRADA-Tools/RMTable/raw/master/consolidated_catalog_ver1.0.1.xml.zip)  
 This catalog is provided on an as-is basis; there may be uncaught transcription errors in adapting the published catalogs into the RMTable catalog format. It's also known that some of the published values/sources are unphysical (negative Stokes I, fractional polarizations outside of \[0,1), unrealistic spectral indices, etc). Users should use their discretion when selecting sources in the catalog to use. Please see Section 3.2 of the [paper](https://www.dropbox.com/s/ebdnhad8vypx4cc/RMTable.pdf?dl=0) for more suggestions on catalog usage.
 
+The DOI for the current version of the catalog (ver1.0.1) is [10.5281/zenodo.6907975](https://zenodo.org/record/6907975/). The DOI for all versions of the catalog is [10.5281/zenodo.6702842](https://zenodo.org/record/6702842).
+
+
 The list of individual catalogs/papers that have been incorporated into the consolidated catalog, with some notes on how they were adapted, can be found [here](https://github.com/CIRADA-Tools/RMTable/raw/master/docs/Catalog_notes.pdf).
 
 ***
 
-Conversions of new catalogs into the RMTable format for inclusion into the consolidated catalog are very welcome. If you are interested in contributing a catalog to the consolidated catalog, or find any errors with the catalogs already included, please contact me.
+### Suggestions for catalog authors (or those converting older catalogs)
+Given the large number of columns in the standard, it may seem to potential RM catalog authors that the process of generating a catalog in RMTable format could be more effort than is merited. The majority of the columns defined in the standard are optional and can be omitted or left blank without creating problems, although every column that is included increases the value of the catalog to future users. The key minimum elements that must be adhered to follow the RMTable standard are twofold: first, the standard columns that **are** included must use the naming convention and units of the standard (to avoid users being unable to combine catalogs, or combining catalogs with inconsistent units); second, any columns added that are outside the RMTable standard must not have a name conflict with any of the defined standard columns (e.g., a column labelled ``b'' would conflict with the Galactic Latitude column in RMTable). As long as those two conditions are satisfied, catalog authors have the freedom to choose how much effort they invest into including more of the standard columns. Using this package will automatically ensure both conditions are satisfied.
 
-Cameron Van Eck (cameron.van.eck (at) utoronto.ca)
 
+Conversions of new catalogs into the RMTable format for inclusion into the consolidated catalog are very welcome. If you are interested in contributing a catalog to the consolidated catalog, or find any errors with the catalogs already included, please contact me.
 
+Cameron Van Eck (cameron.van.eck (at) utoronto.ca)
```

### Comparing `RMTable-1.1.0/rmtable/rmtable.py` & `RMTable-1.2.0/rmtable/rmtable.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from astropy.table import Table, Column, MaskedColumn
+from astropy.io import votable as vot
 from astropy.coordinates import SkyCoord
 import astropy.units as au
 import json
 import warnings
 
 try:
     import importlib.resources as importlib_resources
@@ -19,15 +20,15 @@
 RMTables into ASCII (tsv) or FITStable formats as well as convert new catalogs in the 
 form of a numpy ndarray into new RMTables with the correct columns. Methods to convert
 RMTables into numpy arrays or pandas dataframes are also included.
 A full description of the RMTable standard is currently located at 
 https://docs.google.com/document/d/1lo-W89G1X7xGoMOPHYS5japxJKPDamjEJ9uIGnRPnpo/edit
 """
 
-__version__ = "1.2"
+__version__ = "1.3"
 
 # Reading in standard here so they are read on import
 # rather than on first use.
 with importlib_resources.open_text(
     "rmtable", f"column_standard_v{__version__}.json"
 ) as f:
     __standard__ = json.load(f)
@@ -82,15 +83,15 @@
         self.standard_complexity_test = self.entries["complexity_test"]
         self.standard_ionosphere = self.entries["ionosphere"]
 
         super().__init__(data=data, *args, **kwargs)
         # Add ucds to meta of each column
         self._add_ucds()
         # Add descriptions to each column
-        self._add_descriptions()
+        self._add_descriptions(init=True)
         # These are for when extra columns might be added.
         # They point into the table where the columns can be found.
         self._set_rmtab_attrs()
         # Replace any masked columns with fill values
         self._unmask()
 
     def _set_rmtab_attrs(self):
@@ -100,15 +101,15 @@
         self.size = len(self)
 
     def _new_from_slice(self, slice_):
         # For some dumb reason, the OG _new_from_slice method
         # clears the meta attributes.
         ret = super()._new_from_slice(slice_)
         ret._add_ucds()
-        ret._add_descriptions()
+        ret._add_descriptions(init=True)
         ret._set_rmtab_attrs()
         return ret
 
     def _add_ucds(self):
         """Adds ucds to the meta of each column."""
         for col in self.columns:
             # Check if ucd has already been set
@@ -120,27 +121,30 @@
                         warnings.warn(
                             f"Empty ucd for column '{col}', replacing with standard '{self.standard[col]['ucd']}'"
                         )
                     self[col].meta["ucd"] = self.standard[col]["ucd"]
                 else:
                     self[col].meta["ucd"] = None
 
-    def _add_descriptions(self):
-        """Adds descriptions to each column."""
+    def _add_descriptions(self,init=False):
+        """Adds descriptions to each column.
+        init (bool): if true, disables warnings."""
         for col in self.columns:
             # Check if description has already been set
             if col in self.standard_columns and self[col].description is None:
-                warnings.warn(
-                    f"Empty description for column '{col}', replacing with standard '{self.standard[col]['description']}'"
-                )
+                if not init:
+                    warnings.warn(
+                        f"Empty description for column '{col}', replacing with standard '{self.standard[col]['description']}'"
+                    )
                 self[col].description = self.standard_descriptions[col]
 
     def read(*args, **kwargs):
         """Reads in a table from a file."""
         table = RMTable(Table.read(*args, **kwargs))
+        table.update_version()
         return table
 
     def _unmask(self):
         for col in self.columns:
             if type(self[col]) is MaskedColumn:
                 if self[col].dtype.kind == "f":
                     fill_value = np.nan
@@ -168,15 +172,18 @@
 
     def write_tsv(self, filename, *args, **kwargs):
         """Writes the table to a tsv file."""
         super().write(filename, *args, **kwargs, format="ascii.tab")
 
     def read_tsv(filename, *args, **kwargs):
         """Reads a table from a tsv file."""
-        return RMTable.read(filename, *args, **kwargs, format="ascii.tab")
+        table=RMTable.read(filename, *args, **kwargs, format="ascii.tab")
+        table.update_version()
+        return table
+
 
     @classmethod
     def input_numpy(
         cls, array, verbose=False, verify=True, keep_cols=[], coordinate_system="icrs"
     ):
         """Converts an input numpy array into an RM table object.
         Requires that array has named columns matching standard column names.
@@ -508,14 +515,26 @@
                 + invalid_flux
                 + invalid_ionosphere
             )
             == 0
         ):
             print("No problems found with standardized string entries.")
 
+
+    def verify_ucds(self):
+        """Confirm that all UCDs follow the expected conventions.
+        """
+        for colname, ucd in self.ucds.items():
+            check = vot.ucd.check_ucd(ucd)
+            if not check:
+                warnings.warning(f"{colname} has invalid ucd '{ucd}'")
+
+
+
+
     def add_missing_columns(self):
         """Adds in any missing default columns, with their default (blank) values.
         Can be used to make a table compliant with the standard in terms of having
         all the columns.
         """
         missing_columns = [
             column for column in self.standard_columns if column not in self.columns
@@ -533,14 +552,53 @@
                 )
             )
 
     def to_table(self):
         """Returns the table object."""
         return Table(self)
 
+
+
+    def update_version(self):
+        """Updates read-in tables with older versions to the most recent version.
+        This can't be done using the version number, since the version number
+        doesn't survive the read-write process. Must look for column names.
+        
+        Changes to be made:
+            v1.2: change interval column name to obs_interval
+                  change catalog column name to catalog_name
+            v1.1: Remove id, flagA/B/C_value, flagA/B/C_name columns
+            v1.0: Add rmsf_fwhm column"""
+            
+        #v1.0 updates:
+        if 'rmsf_fwhm' not in self.colnames:
+                self.add_column(
+                    Column(
+                        data=[self.standard_blanks['rmsf_fwhm']] * len(self),
+                        name='rmsf_fwhm',
+                        dtype=self.standard_dtypes['rmsf_fwhm'],
+                        unit=self.standard_units['rmsf_fwhm'],
+                        meta={"ucd": self.standard_ucds['rmsf_fwhm']},
+                    )
+                )
+
+        #v1.1 updates:
+        if 'flagA_value' in self.colnames:
+            self.remove_columns(['id','flagA_value','flagA_name',
+                                           'flagB_value','flagB_name',
+                                           'flagC_value','flagC_name'])
+            
+        #v1.2 updates:
+        if 'catalog' in self.colnames:
+            self.rename_column('catalog','catalog_name')
+            self.rename_column('interval','obs_interval')
+
+            
+        
+
     @staticmethod
     def calculate_missing_coordinates_column(long, lat, to_galactic):
         """Calculate a new pair of coordinate columns (equatorial/galactic) given
         the other pair and specified direction. Assumes input columns are already
         in degrees.
         Uses astropy coordinates for the transform.
         Input parameters:
```

### Comparing `RMTable-1.1.0/setup.py` & `RMTable-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import find_packages, setup, Command
 
 NAME = 'RMTable'
 DESCRIPTION = 'Reading, writing, and manipulating RMTables (radio astronomy Faraday rotation catalogs)'
 URL = 'https://github.com/CIRADA-Tools/RMTable'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.1.0'
+VERSION = '1.2.0'
 
 REQUIRED = [
     'numpy', 'astropy',
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
```

