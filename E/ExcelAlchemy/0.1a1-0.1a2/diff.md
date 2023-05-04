# Comparing `tmp/ExcelAlchemy-0.1a1.tar.gz` & `tmp/ExcelAlchemy-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExcelAlchemy-0.1a1.tar", last modified: Fri Feb 24 08:08:03 2023, max compression
+gzip compressed data, was "ExcelAlchemy-0.1a2.tar", last modified: Fri Feb 24 08:15:39 2023, max compression
```

## Comparing `ExcelAlchemy-0.1a1.tar` & `ExcelAlchemy-0.1a2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     3187 2023-02-24 06:02:05.822738 ExcelAlchemy-0.1a1/.gitignore
--rw-r--r--   0        0        0     1456 2023-02-24 06:30:51.166309 ExcelAlchemy-0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-02-24 06:02:05.822930 ExcelAlchemy-0.1a1/LICENSE
--rwxr-xr-x   0        0        0     2296 2023-02-24 06:02:05.823013 ExcelAlchemy-0.1a1/README.md
--rw-r--r--   0        0        0     3233 2023-02-24 08:06:55.549651 ExcelAlchemy-0.1a1/excelalchemy/__init__.py
--rw-r--r--   0        0        0     1333 2023-02-24 06:30:51.072371 ExcelAlchemy-0.1a1/excelalchemy/abstract.py
--rw-r--r--   0        0        0    35181 2023-02-24 06:30:51.174113 ExcelAlchemy-0.1a1/excelalchemy/alchemy.py
--rw-r--r--   0        0        0     1419 2023-02-24 06:30:51.105497 ExcelAlchemy-0.1a1/excelalchemy/const.py
--rw-r--r--   0        0        0     1927 2023-02-24 06:30:51.063495 ExcelAlchemy-0.1a1/excelalchemy/exception.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823675 ExcelAlchemy-0.1a1/excelalchemy/helper/__init__.py
--rw-r--r--   0        0        0     7335 2023-02-24 06:30:51.087128 ExcelAlchemy-0.1a1/excelalchemy/helper/pydantic.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823849 ExcelAlchemy-0.1a1/excelalchemy/model/__init__.py
--rw-r--r--   0        0        0    18460 2023-02-24 06:30:51.170856 ExcelAlchemy-0.1a1/excelalchemy/model/abstract.py
--rw-r--r--   0        0        0     5751 2023-02-24 06:30:51.093398 ExcelAlchemy-0.1a1/excelalchemy/model/excel.py
--rw-r--r--   0        0        0      456 2023-02-24 06:02:05.824152 ExcelAlchemy-0.1a1/excelalchemy/model/identity.py
--rw-r--r--   0        0        0     2433 2023-02-24 06:30:51.183138 ExcelAlchemy-0.1a1/excelalchemy/model/result.py
--rw-r--r--   0        0        0      278 2023-02-24 06:30:51.097098 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/__init__.py
--rw-r--r--   0        0        0     2021 2023-02-24 06:30:51.188212 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/boolean.py
--rw-r--r--   0        0        0     4012 2023-02-24 06:30:51.161662 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/date.py
--rw-r--r--   0        0        0     6009 2023-02-24 06:30:51.129907 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/date_range.py
--rw-r--r--   0        0        0      585 2023-02-24 06:30:51.077370 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/email.py
--rw-r--r--   0        0        0      335 2023-02-24 06:30:51.178048 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/money.py
--rw-r--r--   0        0        0     3284 2023-02-24 06:30:51.146249 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/multi_checkbox.py
--rw-r--r--   0        0        0     4363 2023-02-24 06:30:51.079918 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/number.py
--rw-r--r--   0        0        0     4758 2023-02-24 06:30:51.155194 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/number_range.py
--rw-r--r--   0        0        0     2811 2023-02-24 06:30:51.157636 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/organization.py
--rw-r--r--   0        0        0      614 2023-02-24 06:30:51.163555 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/phone_number.py
--rw-r--r--   0        0        0     2578 2023-02-24 06:30:51.095292 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/radio.py
--rw-r--r--   0        0        0     2955 2023-02-24 06:30:51.065628 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/staff.py
--rw-r--r--   0        0        0     4947 2023-02-24 06:30:51.089259 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/string.py
--rw-r--r--   0        0        0     2975 2023-02-24 06:30:51.113232 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/tree.py
--rw-r--r--   0        0        0      773 2023-02-24 06:30:51.074855 ExcelAlchemy-0.1a1/excelalchemy/model/value_type/url.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825504 ExcelAlchemy-0.1a1/excelalchemy/plugin/__init__.py
--rw-r--r--   0        0        0      576 2023-02-24 06:30:51.082414 ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/__init__.py
--rw-r--r--   0        0        0     4113 2023-02-24 06:30:51.127323 ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/builder.py
--rw-r--r--   0        0        0     5070 2023-02-24 06:30:51.085015 ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/config.py
--rw-r--r--   0        0        0    12752 2023-02-24 06:30:51.056689 ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/screen.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825884 ExcelAlchemy-0.1a1/excelalchemy/py.typed
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825956 ExcelAlchemy-0.1a1/excelalchemy/tool/__init__.py
--rw-r--r--   0        0        0     1470 2023-02-24 06:30:51.124528 ExcelAlchemy-0.1a1/excelalchemy/tool/convertor.py
--rw-r--r--   0        0        0     2736 2023-02-24 06:30:51.159637 ExcelAlchemy-0.1a1/excelalchemy/util.py
--rw-r--r--   0        0        0    16607 2023-02-24 06:30:51.110554 ExcelAlchemy-0.1a1/excelalchemy/writer.py
--rw-r--r--   0        0        0     2263 2023-02-24 08:04:38.941848 ExcelAlchemy-0.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.826382 ExcelAlchemy-0.1a1/tests/__init__.py
--rw-r--r--   0        0        0     6470 2023-02-24 06:30:51.103701 ExcelAlchemy-0.1a1/tests/test_alchemy.py
--rw-r--r--   0        0        0     3086 1970-01-01 00:00:00.000000 ExcelAlchemy-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3187 2023-02-24 06:02:05.822738 ExcelAlchemy-0.1a2/.gitignore
+-rw-r--r--   0        0        0     1456 2023-02-24 06:30:51.166309 ExcelAlchemy-0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-02-24 06:02:05.822930 ExcelAlchemy-0.1a2/LICENSE
+-rwxr-xr-x   0        0        0     2296 2023-02-24 06:02:05.823013 ExcelAlchemy-0.1a2/README.md
+-rw-r--r--   0        0        0     3233 2023-02-24 08:15:38.653220 ExcelAlchemy-0.1a2/excelalchemy/__init__.py
+-rw-r--r--   0        0        0     1333 2023-02-24 06:30:51.072371 ExcelAlchemy-0.1a2/excelalchemy/abstract.py
+-rw-r--r--   0        0        0    35181 2023-02-24 06:30:51.174113 ExcelAlchemy-0.1a2/excelalchemy/alchemy.py
+-rw-r--r--   0        0        0     1419 2023-02-24 06:30:51.105497 ExcelAlchemy-0.1a2/excelalchemy/const.py
+-rw-r--r--   0        0        0     1927 2023-02-24 06:30:51.063495 ExcelAlchemy-0.1a2/excelalchemy/exception.py
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823675 ExcelAlchemy-0.1a2/excelalchemy/helper/__init__.py
+-rw-r--r--   0        0        0     7335 2023-02-24 06:30:51.087128 ExcelAlchemy-0.1a2/excelalchemy/helper/pydantic.py
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823849 ExcelAlchemy-0.1a2/excelalchemy/model/__init__.py
+-rw-r--r--   0        0        0    18460 2023-02-24 06:30:51.170856 ExcelAlchemy-0.1a2/excelalchemy/model/abstract.py
+-rw-r--r--   0        0        0     5751 2023-02-24 06:30:51.093398 ExcelAlchemy-0.1a2/excelalchemy/model/excel.py
+-rw-r--r--   0        0        0      456 2023-02-24 06:02:05.824152 ExcelAlchemy-0.1a2/excelalchemy/model/identity.py
+-rw-r--r--   0        0        0     2433 2023-02-24 06:30:51.183138 ExcelAlchemy-0.1a2/excelalchemy/model/result.py
+-rw-r--r--   0        0        0      278 2023-02-24 06:30:51.097098 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/__init__.py
+-rw-r--r--   0        0        0     2021 2023-02-24 06:30:51.188212 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/boolean.py
+-rw-r--r--   0        0        0     4012 2023-02-24 06:30:51.161662 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date.py
+-rw-r--r--   0        0        0     6009 2023-02-24 06:30:51.129907 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date_range.py
+-rw-r--r--   0        0        0      585 2023-02-24 06:30:51.077370 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/email.py
+-rw-r--r--   0        0        0      335 2023-02-24 06:30:51.178048 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/money.py
+-rw-r--r--   0        0        0     3284 2023-02-24 06:30:51.146249 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/multi_checkbox.py
+-rw-r--r--   0        0        0     4363 2023-02-24 06:30:51.079918 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number.py
+-rw-r--r--   0        0        0     4758 2023-02-24 06:30:51.155194 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number_range.py
+-rw-r--r--   0        0        0     2811 2023-02-24 06:30:51.157636 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/organization.py
+-rw-r--r--   0        0        0      614 2023-02-24 06:30:51.163555 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/phone_number.py
+-rw-r--r--   0        0        0     2578 2023-02-24 06:30:51.095292 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/radio.py
+-rw-r--r--   0        0        0     2955 2023-02-24 06:30:51.065628 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/staff.py
+-rw-r--r--   0        0        0     4947 2023-02-24 06:30:51.089259 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/string.py
+-rw-r--r--   0        0        0     2975 2023-02-24 06:30:51.113232 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/tree.py
+-rw-r--r--   0        0        0      773 2023-02-24 06:30:51.074855 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/url.py
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825504 ExcelAlchemy-0.1a2/excelalchemy/plugin/__init__.py
+-rw-r--r--   0        0        0      576 2023-02-24 06:30:51.082414 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/__init__.py
+-rw-r--r--   0        0        0     4113 2023-02-24 06:30:51.127323 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/builder.py
+-rw-r--r--   0        0        0     5070 2023-02-24 06:30:51.085015 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/config.py
+-rw-r--r--   0        0        0    12752 2023-02-24 06:30:51.056689 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/screen.py
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825884 ExcelAlchemy-0.1a2/excelalchemy/py.typed
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825956 ExcelAlchemy-0.1a2/excelalchemy/tool/__init__.py
+-rw-r--r--   0        0        0     1470 2023-02-24 06:30:51.124528 ExcelAlchemy-0.1a2/excelalchemy/tool/convertor.py
+-rw-r--r--   0        0        0     2736 2023-02-24 06:30:51.159637 ExcelAlchemy-0.1a2/excelalchemy/util.py
+-rw-r--r--   0        0        0    16607 2023-02-24 06:30:51.110554 ExcelAlchemy-0.1a2/excelalchemy/writer.py
+-rw-r--r--   0        0        0     2332 2023-02-24 08:15:23.458018 ExcelAlchemy-0.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-24 06:02:05.826382 ExcelAlchemy-0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0     6470 2023-02-24 06:30:51.103701 ExcelAlchemy-0.1a2/tests/test_alchemy.py
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 ExcelAlchemy-0.1a2/PKG-INFO
```

### Comparing `ExcelAlchemy-0.1a1/.gitignore` & `ExcelAlchemy-0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/.pre-commit-config.yaml` & `ExcelAlchemy-0.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/LICENSE` & `ExcelAlchemy-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/README.md` & `ExcelAlchemy-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/__init__.py` & `ExcelAlchemy-0.1a2/excelalchemy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ExcelAlchemy, a Python library for reading and writing Excel files."""
 # pre-alpha
-__version__ = '0.1a1'
+__version__ = '0.1a2'
 
 from excelalchemy.alchemy import ExcelAlchemy
 from excelalchemy.exception import ExcelCellError
 from excelalchemy.exception import ProgrammaticError
 from excelalchemy.model.abstract import CharacterSet
 from excelalchemy.model.abstract import DataRangeOption
 from excelalchemy.model.abstract import DateFormat
```

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/abstract.py` & `ExcelAlchemy-0.1a2/excelalchemy/abstract.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/alchemy.py` & `ExcelAlchemy-0.1a2/excelalchemy/alchemy.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/const.py` & `ExcelAlchemy-0.1a2/excelalchemy/const.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/exception.py` & `ExcelAlchemy-0.1a2/excelalchemy/exception.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/helper/pydantic.py` & `ExcelAlchemy-0.1a2/excelalchemy/helper/pydantic.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/abstract.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/abstract.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/excel.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/excel.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/result.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/result.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/boolean.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/boolean.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/date.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/date_range.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date_range.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/email.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/email.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/multi_checkbox.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/multi_checkbox.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/number.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/number_range.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number_range.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/organization.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/organization.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/phone_number.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/phone_number.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/radio.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/radio.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/staff.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/staff.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/string.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/string.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/tree.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/tree.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/model/value_type/url.py` & `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/url.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/__init__.py` & `ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/__init__.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/builder.py` & `ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/builder.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/config.py` & `ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/config.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/plugin/esm/screen.py` & `ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/screen.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/tool/convertor.py` & `ExcelAlchemy-0.1a2/excelalchemy/tool/convertor.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/util.py` & `ExcelAlchemy-0.1a2/excelalchemy/util.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/excelalchemy/writer.py` & `ExcelAlchemy-0.1a2/excelalchemy/writer.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/pyproject.toml` & `ExcelAlchemy-0.1a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     "openpyxl >=3.0.10, <4",
     'pendulum >=2.1.2, <3',
 ]
 
 [tool.flit.module]
 name = "excelalchemy"
 
+[project.urls]
+Home = "https://github.com/SundayWindy/excelalchemy"
+
 [project.optional-dependencies]
 development = ["pandas-stubs", "black", "isort", "mypy", "pylint", "pre-commit"]
 
 [tool.pyright]
 exclude = [
     ".venv",
     "venv",
```

### Comparing `ExcelAlchemy-0.1a1/tests/test_alchemy.py` & `ExcelAlchemy-0.1a2/tests/test_alchemy.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a1/PKG-INFO` & `ExcelAlchemy-0.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExcelAlchemy
-Version: 0.1a1
+Version: 0.1a2
 Summary: ExcelAlchemy, a Python library for reading and writing Excel files.
 Author-email: 何睿 <hrui835@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pandas >=1.5.1, <1.6
 Requires-Dist: minio >=7.0.0, <8
@@ -13,14 +13,15 @@
 Requires-Dist: pendulum >=2.1.2, <3
 Requires-Dist: pandas-stubs ; extra == "development"
 Requires-Dist: black ; extra == "development"
 Requires-Dist: isort ; extra == "development"
 Requires-Dist: mypy ; extra == "development"
 Requires-Dist: pylint ; extra == "development"
 Requires-Dist: pre-commit ; extra == "development"
+Project-URL: Home, https://github.com/SundayWindy/excelalchemy
 Provides-Extra: development
 
 # ExcelAlchemy 开发指南
 
 ## 1. 项目介绍
 
 * ExcelAlchemy 负责从 Excel 解析用户的输入，转换、生成对应的数据结构，给后端使用。
```

