# Comparing `tmp/datacooker-0.4.0.tar.gz` & `tmp/datacooker-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacooker-0.4.0.tar", max compression
+gzip compressed data, was "datacooker-0.4.1.tar", max compression
```

## Comparing `datacooker-0.4.0.tar` & `datacooker-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1109 2023-01-17 17:21:25.499561 datacooker-0.4.0/LICENSE
--rw-r--r--   0        0        0      377 2023-01-17 17:21:25.499561 datacooker-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/__init__.py
--rw-r--r--   0        0        0      196 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/recipes/__init__.py
--rw-r--r--   0        0        0      946 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/recipes/auto_regressive_recipe.py
--rw-r--r--   0        0        0      397 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/recipes/logit_recipe.py
--rw-r--r--   0        0        0      393 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/recipes/poisson_recipe.py
--rw-r--r--   0        0        0     6590 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/recipes/recipe.py
--rw-r--r--   0        0        0       75 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/utils/__init__.py
--rw-r--r--   0        0        0      403 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/utils/is_valid_fraction.py
--rw-r--r--   0        0        0      186 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/__init__.py
--rw-r--r--   0        0        0     1156 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/continous_variable.py
--rw-r--r--   0        0        0      982 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/discrete_variable.py
--rw-r--r--   0        0        0     1253 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/error_messages.py
--rw-r--r--   0        0        0     1099 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/nominal_variable.py
--rw-r--r--   0        0        0     1405 2023-01-17 17:21:25.499561 datacooker-0.4.0/datacooker/variables/variable.py
--rw-r--r--   0        0        0      755 2023-01-17 17:21:25.499561 datacooker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 datacooker-0.4.0/setup.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 datacooker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-04 11:46:01.327021 datacooker-0.4.1/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-04 11:46:01.327021 datacooker-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/__init__.py
+-rw-r--r--   0        0        0      196 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/recipes/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/recipes/auto_regressive_recipe.py
+-rw-r--r--   0        0        0      397 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/recipes/logit_recipe.py
+-rw-r--r--   0        0        0      393 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/recipes/poisson_recipe.py
+-rw-r--r--   0        0        0     6590 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/recipes/recipe.py
+-rw-r--r--   0        0        0       75 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/utils/__init__.py
+-rw-r--r--   0        0        0      403 2023-05-04 11:46:01.327021 datacooker-0.4.1/datacooker/utils/is_valid_fraction.py
+-rw-r--r--   0        0        0      186 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/continous_variable.py
+-rw-r--r--   0        0        0      982 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/discrete_variable.py
+-rw-r--r--   0        0        0     1253 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/error_messages.py
+-rw-r--r--   0        0        0     1099 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/nominal_variable.py
+-rw-r--r--   0        0        0     1405 2023-05-04 11:46:01.331021 datacooker-0.4.1/datacooker/variables/variable.py
+-rw-r--r--   0        0        0      755 2023-05-04 11:46:01.331021 datacooker-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 datacooker-0.4.1/PKG-INFO
```

### Comparing `datacooker-0.4.0/LICENSE` & `datacooker-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/recipes/auto_regressive_recipe.py` & `datacooker-0.4.1/datacooker/recipes/auto_regressive_recipe.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/recipes/recipe.py` & `datacooker-0.4.1/datacooker/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/variables/continous_variable.py` & `datacooker-0.4.1/datacooker/variables/continous_variable.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/variables/discrete_variable.py` & `datacooker-0.4.1/datacooker/variables/discrete_variable.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/variables/error_messages.py` & `datacooker-0.4.1/datacooker/variables/error_messages.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/variables/nominal_variable.py` & `datacooker-0.4.1/datacooker/variables/nominal_variable.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/datacooker/variables/variable.py` & `datacooker-0.4.1/datacooker/variables/variable.py`

 * *Files identical despite different names*

### Comparing `datacooker-0.4.0/pyproject.toml` & `datacooker-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "datacooker"
-version = "0.4.0"
+version = "0.4.1"
 description = "Library for data generation based on model specs (Recipes)"
 authors = ["Guilherme <g.lisboa.oliveira@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "datacooker"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.23.4"
 scipy = "^1.9.2"
-pandas = "^1.5.0"
+pandas = "^2.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.3"
 
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.1.3"
-pytest-cov = "^3.0.0"
+pytest-cov = ">=3,<5"
 pytest-mock = "^3.9.0"
 statsmodels = "^0.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datacooker-0.4.0/PKG-INFO` & `datacooker-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: datacooker
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for data generation based on model specs (Recipes)
 License: MIT
 Author: Guilherme
 Author-email: g.lisboa.oliveira@outlook.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
-Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: scipy (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Data Cooker
 
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=OStatsAA_data-cooker&metric=coverage)](https://sonarcloud.io/summary/new_code?id=OStatsAA_data-cooker)
```

