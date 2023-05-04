# Comparing `tmp/misura-1.4.0.tar.gz` & `tmp/misura-1.4.1.tar.gz`

## Comparing `misura-1.4.0.tar` & `misura-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.4.0/.gitattributes
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.4.0/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 misura-1.4.0/docs/docs.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/__main__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/exceptions.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/globals.py
--rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/quantities.py
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/tables.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 misura-1.4.0/src/misura/utilities.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 misura-1.4.0/tests/tests.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.4.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.4.0/LICENSE
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 misura-1.4.0/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 misura-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.4.1/.gitattributes
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.4.1/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 misura-1.4.1/docs/docs.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/__main__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/exceptions.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/globals.py
+-rw-r--r--   0        0        0    19140 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/quantities.py
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/tables.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/utilities.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 misura-1.4.1/tests/tests.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.4.1/LICENSE
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 misura-1.4.1/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 misura-1.4.1/PKG-INFO
```

### Comparing `misura-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/.github/workflows/python-publish.yml` & `misura-1.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/docs/docs.md` & `misura-1.4.1/docs/docs.md`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/src/misura/__main__.py` & `misura-1.4.1/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/src/misura/exceptions.py` & `misura-1.4.1/src/misura/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,22 +52,36 @@
 
 
 class PackError(Exception):
     """
     Raised on errors during conversions.
     """
 
-    def __init__(self, qnt, target: str, full: bool = False) -> None:
-        super().__init__(
-            "cannot {3}pack '{0}' to '{1}'\nraised by: '{2}'".format(
-                qnt.unit(), target, qnt, "fully " if full else ""
+    def __init__(self, qnt, target: str, ignore: str = "", full: bool = False) -> None:
+        if ignore:  # Error on ignore.
+            super().__init__(
+                "cannot ignore '{1}'\nraised by: '{0}'".format(qnt, ignore)
+            )
+
+        elif not target:  # Missing target.
+            super().__init__("cannot automatically pack\nraised by: '{0}'".format(qnt))
+
+        elif full:
+            super().__init__(
+                "cannot fully pack '{2}' to '{1}'\nraised by: '{0}'".format(
+                    qnt, target, qnt.unit()
+                )
+            )
+
+        else:
+            super().__init__(
+                "cannot pack '{2}' to '{1}'\nraised by: '{0}'".format(
+                    qnt, target, qnt.unit()
+                )
             )
-            if target != ""
-            else "cannot automatically pack"
-        )
 
 
 class DefinitionError(Exception):
     """
     Raised on errors during unit definition.
     """
```

### Comparing `misura-1.4.0/src/misura/quantities.py` & `misura-1.4.1/src/misura/quantities.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .exceptions import (
     UnitError,
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
 )
-from .tables import getBase, getDerived, getDerivedUnpacking, getFamily
+from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
 from .utilities import dictFromUnit, unitFromDict
 
 # QUANTITIES
 
 
 class quantity:
     """
@@ -62,44 +62,44 @@
 
         # Fancy version.
         if print:
             # {"m": 1, "s": -1} -> "[m / s]".
             numerator = " ".join(
                 sorted(
                     [
-                        sym
+                        unit
                         + (
-                            "({})".format(self.units[sym])
-                            if self.units[sym] != 1
+                            "({})".format(self.units[unit])
+                            if self.units[unit] != 1
                             else ""
                         )
-                        for sym in self.units
-                        if self.units[sym] > 0
+                        for unit in self.units
+                        if self.units[unit] > 0
                     ]
                 )
             )
             denominator = (
                 (
                     " / "
                     + " ".join(
                         sorted(
                             [
-                                sym
+                                unit
                                 + (
-                                    "({})".format(-1 * self.units[sym])
-                                    if self.units[sym] != -1
+                                    "({})".format(-1 * self.units[unit])
+                                    if self.units[unit] != -1
                                     else ""
                                 )
-                                for sym in self.units
-                                if self.units[sym] < 0
+                                for unit in self.units
+                                if self.units[unit] < 0
                             ]
                         )
                     )
                 )
-                if len([sym for sym in self.units if self.units[sym] < 0])
+                if len([unit for unit in self.units if self.units[unit] < 0])
                 else ""
             )
 
             if not numerator and denominator:
                 numerator = "1"
 
             if style.quantityHighlighting:
@@ -123,45 +123,45 @@
         if not len(self.dimensionalities):
             return ""
 
         # {"length": 2, "time": -1} -> "[length(2) / time]".
         numerator = " * ".join(
             sorted(
                 [
-                    sym
+                    dim
                     + (
-                        "({})".format(self.dimensionalities[sym])
-                        if self.dimensionalities[sym] != 1
+                        "({})".format(self.dimensionalities[dim])
+                        if self.dimensionalities[dim] != 1
                         else ""
                     )
-                    for sym in self.dimensionalities
-                    if self.dimensionalities[sym] > 0
+                    for dim in self.dimensionalities
+                    if self.dimensionalities[dim] > 0
                 ]
             )
         )
         denominator = (
             (
                 " / "
                 + " * ".join(
                     sorted(
                         [
-                            sym
+                            dim
                             + (
-                                "({})".format(-1 * self.dimensionalities[sym])
-                                if self.dimensionalities[sym] != -1
+                                "({})".format(-1 * self.dimensionalities[dim])
+                                if self.dimensionalities[dim] != -1
                                 else ""
                             )
-                            for sym in self.dimensionalities
-                            if self.dimensionalities[sym] < 0
+                            for dim in self.dimensionalities
+                            if self.dimensionalities[dim] < 0
                         ]
                     )
                 )
             )
             if len(
-                [sym for sym in self.dimensionalities if self.dimensionalities[sym] < 0]
+                [dim for dim in self.dimensionalities if self.dimensionalities[dim] < 0]
             )
             else ""
         )
 
         if not numerator and denominator:
             numerator = "1"
 
@@ -176,15 +176,15 @@
             else str(self.value)
         )
 
     def __repr__(self) -> str:
         return str(self)
 
     def __format__(self, string) -> str:  # Unit highlighting works for print only.
-        # This works with units only.
+        # This works with print only.
         return self.value.__format__(string) + (
             " " + self.unit(print=True) if self.unit() else ""
         )
 
     # PYTHON TYPES CONVERSION.
 
     # Int.
@@ -293,21 +293,21 @@
             return quantity(self.value * other, self.unit())
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
-        for sym in newUnits:
-            if sym in other.units:
-                newUnits[sym] += other.units[sym]
-
-        for sym in other.units:
-            if sym not in newUnits:
-                newUnits[sym] = other.units[sym]
+        for unit in newUnits:
+            if unit in other.units:
+                newUnits[unit] += other.units[unit]
+
+        for unit in other.units:
+            if unit not in newUnits:
+                newUnits[unit] = other.units[unit]
 
         return (
             quantity(self.value * other.value, unitFromDict(newUnits))
             if unitFromDict(newUnits)
             else self.value * other.value
         )
 
@@ -320,21 +320,21 @@
             return quantity(self.value / other, self.unit())
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
-        for sym in newUnits:
-            if sym in other.units:
-                newUnits[sym] -= other.units[sym]
-
-        for sym in other.units:
-            if sym not in newUnits:
-                newUnits[sym] = -other.units[sym]
+        for unit in newUnits:
+            if unit in other.units:
+                newUnits[unit] -= other.units[unit]
+
+        for unit in other.units:
+            if unit not in newUnits:
+                newUnits[unit] = -other.units[unit]
 
         return (
             quantity(self.value / other.value, unitFromDict(newUnits))
             if unitFromDict(newUnits)
             else self.value / other.value
         )
 
@@ -347,16 +347,16 @@
     # Power.
     def __pow__(self, other: any) -> quantity:
         if other == 0:
             return 1
 
         newUnits = self.units.copy()
 
-        for sym in newUnits:
-            newUnits[sym] *= other
+        for unit in newUnits:
+            newUnits[unit] *= other
 
         return quantity(self.value**other, unitFromDict(newUnits))
 
     # Modulo.
     def __mod__(self, other: any) -> quantity:
         return quantity(self.value % other, self.unit())
 
@@ -456,64 +456,63 @@
         ):
             raise ConversionError(qnt, targets)
 
     # Automatic (un)packing.
     # Version 1.
     if un_pack and not partial:
         try:
-            return convert(pack(qnt, targets), targets, partial=False, un_pack=False)
+            return convert(pack(qnt, targets), targets, un_pack=False)
 
         except ConversionError:
             pass
 
         return convert(
             unpack(qnt),
             unpack(quantity(1, targets)).unit(),
-            partial=False,
             un_pack=False,
         )
 
     factor: float = 1.0
     units: dict = qnt.units.copy()
     targetUnits: dict = dictFromUnit(targets)
 
     partialTargets: dict = dict()
 
     table: dict = getBase()
     table.update(getDerived())
 
-    for sym in units.keys():
-        family = getFamily(sym)
+    for unit in units.keys():
+        family = getFamily(unit)
         familyCounter = 0
 
         for targetSym in targetUnits:
             if targetSym in table[family]:
                 targetUnit = targetSym
                 familyCounter += 1
 
         if familyCounter == 0:
             if not partial:
                 raise ConversionError(qnt, targets)
 
-            partialTargets[sym] = units[sym]
+            partialTargets[unit] = units[unit]
             continue
 
         elif familyCounter > 1:
             raise ConversionError(qnt, targets)
 
-        elif sym != targetUnit:
-            if units[sym] != targetUnits[targetUnit]:
+        elif unit != targetUnit:
+            if units[unit] != targetUnits[targetUnit]:
                 raise ConversionError(qnt, targets)
 
-            factor *= (table[family][sym] / table[family][targetUnit]) ** units[sym]
+            factor *= (table[family][unit] / table[family][targetUnit]) ** units[unit]
             partialTargets[targetUnit] = targetUnits[targetUnit]
             continue
 
         elif partial:
-            partialTargets[sym] = units[sym]
+            partialTargets[unit] = units[unit]
 
     return (
         quantity(qnt.value * factor, targets)
         if not partial
         else quantity(qnt.value * factor, unitFromDict(partialTargets))
     )
 
@@ -533,20 +532,18 @@
             [unit for unit in qnt.units if getFamily(unit) in derivedTable]
         )
 
         if targets == "":
             return qnt
 
     for target in dictFromUnit(targets):
-        # these shouldn't raise an IndexError as long as there's a reference quantity for every family.
-        conversionTarget = [
-            unit
-            for unit in derivedTable[getFamily(target)]
-            if derivedTable[getFamily(target)][unit] == 1
-        ].pop()
+        if getFamily(target) not in [getFamily(unit) for unit in qnt.units]:
+            raise UnpackError(qnt, target)
+
+        conversionTarget = getRep(getFamily(target))
         conversionTargetPower = [
             qnt.units[unit]
             for unit in qnt.units
             if getFamily(unit) == getFamily(target)
         ].pop()
 
         qnt = convert(
@@ -580,25 +577,30 @@
     unitsTable: dict = getBase()
     unitsTable.update(getDerived())
 
     if targets == "":
         raise PackError(qnt, "")
 
     # Simplify qnt -> base unit.
-    for unit in qnt.units.keys():
+    for unit in qnt.units:
         conversionTarget = [
             unit
             for unit in unitsTable[getFamily(unit)]
             if unitsTable[getFamily(unit)][unit] == 1
         ].pop()
         qnt = convert(
             qnt, conversionTarget + str(qnt.units[unit]), partial=True, un_pack=False
         )
 
     # Unpack only relevant units.
+    if ignore:
+        for ignored in dictFromUnit(ignore):
+            if getFamily(ignored) not in [getFamily(unit) for unit in qnt.units]:
+                raise PackError(qnt, targets, ignore)
+
     qnt = (
         quantity(
             qnt.value,
             unitFromDict(
                 {
                     unit: qnt.units[unit]
                     for unit in qnt.units
@@ -626,32 +628,33 @@
         if target not in packTable:
             continue
 
         targetUnits = dictFromUnit(packTable[target])
 
         # Packing powers.
         powers = {
-            qnt.units[targetUnit] // targetUnits[targetUnit]
+            # Updated from // to / to account for fractional powers.
+            qnt.units[targetUnit] / targetUnits[targetUnit]
             for targetUnit in targetUnits
             if targetUnit in qnt.units
         }
 
         if not len(powers):
             raise PackError(qnt, targets)
 
-        if full:  # The packability check can be skipped
+        if full:
             # Packability check.
             for targetUnit in targetUnits:
                 if targetUnit not in qnt.units:
-                    raise PackError(qnt, targets, True)
+                    raise PackError(qnt, targets, full=True)
 
                 if qnt.units[targetUnit] % targetUnits[targetUnit]:
-                    raise PackError(qnt, targets, True)
+                    raise PackError(qnt, targets, full=True)
 
             if min(powers) < max(powers) or max(powers) < 0:
-                raise PackError(qnt, targets, True)
+                raise PackError(qnt, targets, full=True)
 
         qnt *= (quantity(1, target) / quantity(1, unitFromDict(targetUnits))) ** max(
             powers
         )
 
     return qnt
```

### Comparing `misura-1.4.0/src/misura/tables.py` & `misura-1.4.1/src/misura/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Returns a reference unit given its family.
     """
 
     table = getBase()
     table.update(getDerived())
 
     if family in table:
+        # This shouldn't raise an IndexError as long as there's a reference unit for every family.
         return [unit for unit in table[family] if table[family][unit] == 1].pop()
 
 
 def getFamily(unit: str) -> str:
     """
     Returns the family of a convertible unit.
     """
```

### Comparing `misura-1.4.0/src/misura/utilities.py` & `misura-1.4.1/src/misura/utilities.py`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/tests/tests.py` & `misura-1.4.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/LICENSE` & `misura-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/README.md` & `misura-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `misura-1.4.0/pyproject.toml` & `misura-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.4.0/PKG-INFO` & `misura-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

