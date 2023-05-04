# Comparing `tmp/misura-1.3.0.tar.gz` & `tmp/misura-1.3.1.tar.gz`

## Comparing `misura-1.3.0.tar` & `misura-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.3.0/.gitattributes
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.3.0/Makefile
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.3.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.3.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.3.0/.github/SECURITY.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 misura-1.3.0/docs/docs.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/__init__.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/exceptions.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/globals.py
--rw-r--r--   0        0        0    15863 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/quantities.py
--rw-r--r--   0        0        0    11665 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/tables.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 misura-1.3.0/src/misura/utilities.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 misura-1.3.0/tests/tests.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.3.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.3.0/LICENSE
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 misura-1.3.0/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 misura-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 misura-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.3.1/.gitattributes
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.3.1/Makefile
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 misura-1.3.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 misura-1.3.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 misura-1.3.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 misura-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 misura-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 misura-1.3.1/docs/docs.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/__main__.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/exceptions.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/globals.py
+-rw-r--r--   0        0        0    15863 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/quantities.py
+-rw-r--r--   0        0        0    11665 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/tables.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 misura-1.3.1/src/misura/utilities.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 misura-1.3.1/tests/tests.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 misura-1.3.1/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 misura-1.3.1/PKG-INFO
```

### Comparing `misura-1.3.0/.github/CODE_OF_CONDUCT.md` & `misura-1.3.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/.github/CONTRIBUTING.md` & `misura-1.3.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/.github/SECURITY.md` & `misura-1.3.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `misura-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/.github/workflows/python-publish.yml` & `misura-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/docs/docs.md` & `misura-1.3.1/docs/docs.md`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/src/misura/exceptions.py` & `misura-1.3.1/src/misura/exceptions.py`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/src/misura/quantities.py` & `misura-1.3.1/src/misura/quantities.py`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/src/misura/tables.py` & `misura-1.3.1/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/src/misura/utilities.py` & `misura-1.3.1/src/misura/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,22 @@
             units[sym.replace(power, "")] = float(power)
 
     return units
 
 def unitFromDict(units: dict) -> str:
     return " ".join(sorted([sym + ("{}".format(units[sym]) if units[sym] != 1 else "") for sym in units if units[sym] != 0]))
 
+def getRep(family: str) -> str:
+    # Returns the reference unit given its family.
+    table = SI_TABLE.copy()
+    table.update(SI_DERIVED_TABLE)
+
+    if family in table:
+        return [unit for unit in table[family] if table[family][unit] == 1].pop()
+
 def getFamily(unit: str) -> str:
     # Returns the family of a convertible unit (length, mass, ...).
     table = SI_TABLE.copy()
     table.update(SI_DERIVED_TABLE)
 
     for family in table:
         if unit in table[family]:
```

### Comparing `misura-1.3.0/tests/tests.py` & `misura-1.3.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/LICENSE` & `misura-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.3.0/README.md` & `misura-1.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,71 @@
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
 
 	python3 -m pip install --upgrade misura
 
+### Verifying installation and base informations
+
+By:
+
+	python -m misura
+
+you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
+
+[^1]: Examle referring to version 1.3.1
+
+```
+misura v1.3.1
+
+Python library for easy unit handling and conversion for scientific & engineering applications.
+
+Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
+Documentation on https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Bug tracker on https://github.com/diantonioandrea/misura/issues
+
+Here's the list of available units.
+
+BASE UNITS
+
+Time: s.
+Length: m.
+Mass: kg.
+Electric current: A.
+Thermodynamic temperature: K.
+Amount of substance: mol.
+Luminous intensity: cd.
+
+DERIVED UNITS
+
+Plane angle: rad.
+Solid angle: sr.
+Frequency: Hz [s-1].
+Force: N [kg m s-2].
+Pressure: Pa [kg m-1 s-2].
+Energy: J [kg m2 s-2].
+Power: W [kg m2 s-3].
+Electric charge: C [A s].
+Electric potential: V [kg m2 s-3 A-1].
+Capacitance: F [kg-1 m-2 s4 A2].
+Resistance: Ω [kg m2 s-3 A-2].
+Electrical conductance: S [kg-1 m-2 s3 A2].
+Magnetic flux: Wb [kg m2 s-2 A-1].
+Magnetic flux density: T [kg s-2 A-1].
+Inductance: H [kg m2 s-2 A-2].
+Luminous flux: lm [cd sr].
+Illuminance: lx [cd sr m-2].
+Radionuclide activity: Bq [s-1].
+Absorbed dose: Gy [m2 s-2].
+Equivalent dose: Sv [m2 s-2].
+Catalyc activity: kat [mol s-1].
+```
+
+
 ### Importing misura
 
 **misura** can be imported by:
 
 	import misura
 
 ## Examples
@@ -206,8 +263,8 @@
 num1 = quantity(2000, "m s-1")
 
 print("Exponential notation: {:.2e}".format(num1))
 ```
 
 The output is:
 
-	Exponential notation: 2.00e+00 m / s
+	Exponential notation: 2.00e+00 m / s
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `misura-1.3.0/pyproject.toml` & `misura-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["colorama"]
+dependencies = ["colorama", "setuptools"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `misura-1.3.0/PKG-INFO` & `misura-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: colorama
+Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/misura)
 
 ![PyPI](https://img.shields.io/pypi/v/misura)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
@@ -51,14 +52,71 @@
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
 
 	python3 -m pip install --upgrade misura
 
+### Verifying installation and base informations
+
+By:
+
+	python -m misura
+
+you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
+
+[^1]: Examle referring to version 1.3.1
+
+```
+misura v1.3.1
+
+Python library for easy unit handling and conversion for scientific & engineering applications.
+
+Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
+Documentation on https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Bug tracker on https://github.com/diantonioandrea/misura/issues
+
+Here's the list of available units.
+
+BASE UNITS
+
+Time: s.
+Length: m.
+Mass: kg.
+Electric current: A.
+Thermodynamic temperature: K.
+Amount of substance: mol.
+Luminous intensity: cd.
+
+DERIVED UNITS
+
+Plane angle: rad.
+Solid angle: sr.
+Frequency: Hz [s-1].
+Force: N [kg m s-2].
+Pressure: Pa [kg m-1 s-2].
+Energy: J [kg m2 s-2].
+Power: W [kg m2 s-3].
+Electric charge: C [A s].
+Electric potential: V [kg m2 s-3 A-1].
+Capacitance: F [kg-1 m-2 s4 A2].
+Resistance: Ω [kg m2 s-3 A-2].
+Electrical conductance: S [kg-1 m-2 s3 A2].
+Magnetic flux: Wb [kg m2 s-2 A-1].
+Magnetic flux density: T [kg s-2 A-1].
+Inductance: H [kg m2 s-2 A-2].
+Luminous flux: lm [cd sr].
+Illuminance: lx [cd sr m-2].
+Radionuclide activity: Bq [s-1].
+Absorbed dose: Gy [m2 s-2].
+Equivalent dose: Sv [m2 s-2].
+Catalyc activity: kat [mol s-1].
+```
+
+
 ### Importing misura
 
 **misura** can be imported by:
 
 	import misura
 
 ## Examples
@@ -222,8 +280,8 @@
 num1 = quantity(2000, "m s-1")
 
 print("Exponential notation: {:.2e}".format(num1))
 ```
 
 The output is:
 
-	Exponential notation: 2.00e+00 m / s
+	Exponential notation: 2.00e+00 m / s
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

