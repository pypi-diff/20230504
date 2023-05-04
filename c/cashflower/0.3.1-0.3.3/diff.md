# Comparing `tmp/cashflower-0.3.1.tar.gz` & `tmp/cashflower-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.3.1.tar", last modified: Thu Mar 23 17:52:32 2023, max compression
+gzip compressed data, was "cashflower-0.3.3.tar", last modified: Thu May  4 17:45:15 2023, max compression
```

## Comparing `cashflower-0.3.1.tar` & `cashflower-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:52:32.141151 cashflower-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-23 17:52:12.000000 cashflower-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 17:52:12.000000 cashflower-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-23 17:52:32.141151 cashflower-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-23 17:52:12.000000 cashflower-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:52:32.137150 cashflower-0.3.1/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28382 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/cashflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:52:32.137150 cashflower-0.3.1/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-03-23 17:52:12.000000 cashflower-0.3.1/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:52:32.137150 cashflower-0.3.1/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-23 17:52:32.000000 cashflower-0.3.1/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-23 17:52:32.000000 cashflower-0.3.1/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:52:32.000000 cashflower-0.3.1/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 17:52:32.000000 cashflower-0.3.1/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 17:52:32.000000 cashflower-0.3.1/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 17:52:32.141151 cashflower-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-23 17:52:12.000000 cashflower-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:52:32.137150 cashflower-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-03-23 17:52:12.000000 cashflower-0.3.1/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-23 17:52:12.000000 cashflower-0.3.1/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-23 17:52:12.000000 cashflower-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 17:45:01.000000 cashflower-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 17:45:01.000000 cashflower-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-04 17:45:15.076512 cashflower-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-04 17:45:01.000000 cashflower-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29050 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/cashflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-04 17:45:01.000000 cashflower-0.3.3/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 17:45:15.000000 cashflower-0.3.3/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:45:15.076512 cashflower-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 17:45:02.000000 cashflower-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:15.076512 cashflower-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-04 17:45:02.000000 cashflower-0.3.3/tests/test_utils.py
```

### Comparing `cashflower-0.3.1/LICENSE` & `cashflower-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.1/PKG-INFO` & `cashflower-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.3.1
+Version: 0.3.3
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
@@ -52,29 +52,29 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable(model_point_set=main)
-death_prob = ModelVariable(model_point_set=main)
+age = ModelVariable()
+death_prob = ModelVariable()
 
 @assign(age)
-def age_formula(t):
+def _age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
 @assign(death_prob)
-def death_prob_formula(t):
+def _death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
```

### Comparing `cashflower-0.3.1/README.md` & `cashflower-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,29 +39,29 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable(model_point_set=main)
-death_prob = ModelVariable(model_point_set=main)
+age = ModelVariable()
+death_prob = ModelVariable()
 
 @assign(age)
-def age_formula(t):
+def _age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
 @assign(death_prob)
-def death_prob_formula(t):
+def _death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
```

### Comparing `cashflower-0.3.1/cashflower/cashflow.py` & `cashflower-0.3.3/cashflower/cashflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import os
 import time
 import pandas as pd
 import sys
 
 
-from .utils import clean_formula_source, is_recursive, list_called_funcs, print_log, split_to_ranges, unique_extend
+from .utils import *
 
 
 def assign(var):
     """Assign formula to an object.
     The decorator links model components and their formulas.
     The decorator also caches the function so that the results get remembered.
 
@@ -526,17 +526,34 @@
         for component in self.components:
             if removed_component in component.grandchildren:
                 component.grandchildren.remove(removed_component)
 
     def set_queue(self):
         """Set an ordrer in which model components should be evaluated."""
         queue = []
-        components = sorted(self.components)
+
+        # User has chosen components, so there is no need to calculate all of them
+        if len(self.settings["OUTPUT_COLUMNS"]) > 0:
+            components = []
+            for component_name in self.settings["OUTPUT_COLUMNS"]:
+                component = self.get_component_by_name(component_name)
+                components = unique_append(components, component)
+                components = unique_extend(components, component.grandchildren)
+            components = sorted(components)
+        else:
+            components = sorted(self.components)
+
         while components:
             component = components[0]
+
+            if len(component.grandchildren) != 0:
+                cycle = get_cycle(component, rest=components)
+                msg = f"Cycle of model components detected. Please review:\n {cycle_to_str(cycle)}"
+                raise CashflowModelError(msg)
+
             queue.append(component)
             self.remove_from_grandchildren(component)
             components.remove(component)
             components = sorted(components)
         self.queue = queue
 
     def set_empty_output(self):
@@ -686,15 +703,15 @@
         else:
             self.calculate()
 
         return self.output
 
     def save(self):
         """Only for single core (no multiprocessing)"""
-        timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+        timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
 
         if not os.path.exists("output"):
             os.makedirs("output")
 
         # Save output to csv
         if self.settings["SAVE_OUTPUT"]:
             print_log("Saving output:")
```

### Comparing `cashflower-0.3.1/cashflower/start.py` & `cashflower-0.3.3/cashflower/start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.1/cashflower.egg-info/PKG-INFO` & `cashflower-0.3.3/cashflower.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.3.1
+Version: 0.3.3
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
@@ -52,29 +52,29 @@
 assumption["mortality"] = pd.read_csv("C:/my_data/mortality.csv", index_col="age")
 ```
 
 ## Model
 
 my_model/model.py
 ```python
-age = ModelVariable(model_point_set=main)
-death_prob = ModelVariable(model_point_set=main)
+age = ModelVariable()
+death_prob = ModelVariable()
 
 @assign(age)
-def age_formula(t):
+def _age(t):
     if t == 0:
         return int(main.get("AGE"))
     elif t % 12 == 0:
         return age(t-1) + 1
     else:
         return age(t-1)
 
 
 @assign(death_prob)
-def death_prob_formula(t):
+def _death_prob(t):
     if age(t) == age(t-1):
         return death_prob(t-1) 
     elif age(t) <= 100:
         sex = main.get("SEX")
         yearly_rate = assumption["mortality"].loc[age(t)][sex]
         monthly_rate = (1 - (1 - yearly_rate)**(1/12))
         return monthly_rate
```

### Comparing `cashflower-0.3.1/setup.py` & `cashflower-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.3.1",
+    version="0.3.3",
 )
```

### Comparing `cashflower-0.3.1/tests/test_cashflow.py` & `cashflower-0.3.3/tests/test_cashflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,16 @@
         b = ModelVariable()
         c = ModelVariable()
 
         a.grandchildren = [b, c]
         b.grandchildren = [c]
         c.grandchildren = []
 
-        model = Model(None, [a, b, c], [], None, None)
+        settings = load_settings()
+        model = Model(None, [a, b, c], [], None, settings)
         model.set_queue()
         assert model.queue == [c, b, a]
 
     def test_set_empty_output(self):
         policy = ModelPointSet(data=pd.DataFrame({"id": [1, 2, 3]}), name="policy")
         fund = ModelPointSet(data=pd.DataFrame({"id": [1, 2, 2, 3]}), name="fund")
```

### Comparing `cashflower-0.3.1/tests/test_start.py` & `cashflower-0.3.3/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.3.1/tests/test_utils.py` & `cashflower-0.3.3/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -95,7 +95,39 @@
         assert is_recursive(cfs5, "my_func5") == 1
 
 
 class TestSplitToRanges(TestCase):
     def test_split_to_ranges(self):
         assert split_to_ranges(20, 3) == [(0, 6), (6, 12), (12, 20)]
         assert split_to_ranges(2, 3) == [(0, 2)]
+
+
+class TestGetCycle(TestCase):
+    def test_get_cycle(self):
+        class Object:
+            def __init__(self, name):
+                self.name = name
+                self.children = []
+
+        a = Object(name="a")
+        b = Object(name="b")
+
+        a.children = [b]
+        b.children = [a]
+
+        result = get_cycle(a, [a, b])
+        assert result == [b, a]
+
+
+class TestCycleToStr(TestCase):
+    def test_cycle_to_str(self):
+        class Object:
+            def __init__(self, name):
+                self.name = name
+
+        a = Object(name="a")
+        b = Object(name="b")
+
+        cycle = [b, a]
+        result = cycle_to_str(cycle)
+        assert result == "b --> a --> b"
+
```

