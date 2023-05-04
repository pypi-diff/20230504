# Comparing `tmp/peewee_plus-1.2.1.tar.gz` & `tmp/peewee_plus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_plus-1.2.1.tar", max compression
+gzip compressed data, was "peewee_plus-1.3.0.tar", max compression
```

## Comparing `peewee_plus-1.2.1.tar` & `peewee_plus-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1053 2023-04-13 19:01:56.883362 peewee_plus-1.2.1/LICENSE.md
--rw-r--r--   0        0        0     4516 2023-04-13 19:01:56.907362 peewee_plus-1.2.1/README.md
--rw-r--r--   0        0        0    15314 2023-04-13 18:59:55.010556 peewee_plus-1.2.1/peewee_plus.py
--rw-r--r--   0        0        0     2521 2023-04-13 18:59:46.222493 peewee_plus-1.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0      348 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/fixtures.py
--rw-r--r--   0        0        0      999 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_about.py
--rw-r--r--   0        0        0     1443 2023-04-13 18:59:35.226414 peewee_plus-1.2.1/tests/test_calc_batch_size.py
--rw-r--r--   0        0        0     1218 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_enumfield.py
--rw-r--r--   0        0        0      794 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_jsonfield.py
--rw-r--r--   0        0        0     1899 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_pathfield.py
--rw-r--r--   0        0        0      985 2022-11-15 12:56:40.995229 peewee_plus-1.2.1/tests/test_precision_float_field.py
--rw-r--r--   0        0        0     5859 1970-01-01 00:00:00.000000 peewee_plus-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-05-04 19:27:56.826959 peewee_plus-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     4476 2023-05-04 19:27:56.870959 peewee_plus-1.3.0/README.md
+-rw-r--r--   0        0        0    16423 2023-05-04 19:26:40.138585 peewee_plus-1.3.0/peewee_plus.py
+-rw-r--r--   0        0        0     2524 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-15 12:56:40.995229 peewee_plus-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      348 2022-11-15 12:56:40.995229 peewee_plus-1.3.0/tests/fixtures.py
+-rw-r--r--   0        0        0     1811 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_calc_batch_size.py
+-rw-r--r--   0        0        0     1383 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_enum_field.py
+-rw-r--r--   0        0        0     1988 2023-05-04 19:26:40.138585 peewee_plus-1.3.0/tests/test_json_field.py
+-rw-r--r--   0        0        0     1163 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_meta.py
+-rw-r--r--   0        0        0     2064 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_path_field.py
+-rw-r--r--   0        0        0     1160 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_precision_float_field.py
+-rw-r--r--   0        0        0      949 2023-05-04 19:21:12.684990 peewee_plus-1.3.0/tests/test_timedelta_field.py
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 peewee_plus-1.3.0/PKG-INFO
```

### Comparing `peewee_plus-1.2.1/LICENSE.md` & `peewee_plus-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `peewee_plus-1.2.1/README.md` & `peewee_plus-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 See the [Changelog](https://github.com/enpaul/peewee-plus/blob/devel/CHANGELOG.md) for
 release history.
 
 ## Documentation
 
-*The documentation for this project is currently a work in progress. Please see the source code for complete docs*
+*The documentation for this project is currently a work in progress. Please see the source
+code for complete docs*
 
 - [Installing](#installing)
 - [Features](#features)
 - [For Developers](#for-developers)
 
 ## Installing
 
@@ -53,42 +54,44 @@
 [Peewee docs](http://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings).
 
 `SQLITE_DEFAULT_VARIABLE_LIMIT` - The maximum number of variables an SQL query can use
 when using SQLite
 
 ### Functions
 
-[`calc_batch_size`](blob/devel/peewee_plus.py#L93) - Helper function for writing
-backend-agnostic batch queries while accounting for the
+`calc_batch_size` - Helper function for writing backend-agnostic batch queries while
+accounting for the
 [SQLite max variable limit](https://www.sqlite.org/limits.html#max_variable_number).
 
-[`flat_transaction`](blob/devel/peewee_plus.py#L159) - Decorator function for wrapping
-callables in a database transaction without creating nested transactions
+`flat_transaction` - Decorator function for wrapping callables in a database transaction
+without creating nested transactions
 
 ### Classes
 
-[`PathField`](blob/devel/peewee_plus.py#204) - A Peewee database field for storing
+`PathField` - A Peewee database field for storing
 [Pathlib](https://docs.python.org/3/library/pathlib.html) objects, optionally relative to
 a runtime value.
 
-[`PrecisionFloatField`](blob/devel/peewee_plus.py#L262) - A Peewee database field for
-storing floats while specifying the
+`PrecisionFloatField` - A Peewee database field for storing floats while specifying the
 [MySQL precision parameters](https://dev.mysql.com/doc/refman/8.0/en/floating-point-types.html)
 `M` and `D`
 
-[`JSONField`](blob/devel/peewee_plus.py#L293) - A Peewee database field for storing
-arbitrary JSON-serializable data
+`JSONField` - A Peewee database field for storing arbitrary JSON-serializable data
 
-[`EnumField`](blob/devel/peewee_plus.py#L348) - A Peewee database field for storing Enums
-by name
+`EnumField` - A Peewee database field for storing Enums by name
+
+`TimedeltaField` A Peewee database field for natively storing
+[`datetime.timedelta`](https://docs.python.org/3/library/datetime.html#datetime.timedelta)
+objects
 
 ## For Developers
 
 All project contributors and participants are expected to adhere to the
-[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
+[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md)
+([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
 
 The `devel` branch has the latest (and potentially unstable) changes. The stable releases
 are tracked on [Github](https://github.com/enpaul/peewee-plus/releases),
 [PyPi](https://pypi.org/project/peewee-plus/#history), and in the
 [Changelog](CHANGELOG.md).
 
 - To report a bug, request a feature, or ask for assistance, please
```

### Comparing `peewee_plus-1.2.1/peewee_plus.py` & `peewee_plus-1.3.0/peewee_plus.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
                                   directly from the `Peewee documentation`_
 
 .. _`Peewee`: https://docs.peewee-orm.com/en/latest/
 
 .. _`Peewee documentation`: https://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings
 """
 import contextlib
+import datetime
 import enum
 import functools
 import json
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import Optional
@@ -28,15 +29,15 @@
 from typing import Type
 from typing import TypeVar
 
 import peewee
 
 
 __title__ = "peewee-plus"
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 __license__ = "MIT"
 __summary__ = "Various extensions, helpers, and utilities for Peewee"
 __url__ = "https://github.com/enpaul/peewee-plus/"
 __authors__ = ["Ethan Paul <24588726+enpaul@users.noreply.github.com>"]
 
 
 __all__ = [
@@ -50,14 +51,15 @@
     "EnumField",
     "flat_transaction",
     "JSONField",
     "PathField",
     "PrecisionFloatField",
     "SQLITE_DEFAULT_PRAGMAS",
     "SQLITE_DEFAULT_VARIABLE_LIMIT",
+    "TimedeltaField",
 ]
 
 
 SQLITE_DEFAULT_PRAGMAS: Dict[str, Any] = {
     "journal_mode": "wal",
     "cache_size": -1 * 64000,
     "foreign_keys": 1,
@@ -311,14 +313,16 @@
                  :err:`peewee.IntegrityError` will be raised
 
     .. warning:: This is a very bad way to store data in a RDBMS and effectively makes the data
                  contained in the field unqueriable.
 
     :param dump_params: Additional keyword arguments to unpack into :func:`json.dump`
     :param load_params: Additional keyword arguments to unpack into :func:`json.load`
+    :raises ValueError: When attempting to set a non-JSON serializable object to the field
+    :raises peewee.IntegrityError: When the underlying database value is not JSON serializable
     """
 
     def __init__(
         self,
         *args,
         dump_params: Optional[Dict[str, Any]] = None,
         load_params: Optional[Dict[str, Any]] = None,
@@ -328,15 +332,15 @@
         self.dump_params = dump_params or {}
         self.load_params = load_params or {}
 
     def db_value(self, value: Any) -> str:
         try:
             return super().db_value(json.dumps(value, **self.dump_params))
         except TypeError as err:
-            raise peewee.IntegrityError(
+            raise ValueError(
                 f"Failed to JSON encode object of type '{type(value)}'"
             ) from err
 
     def python_value(self, value: str) -> Any:
         try:
             return json.loads(super().python_value(value), **self.load_params)
         except json.JSONDecodeError as err:
@@ -395,7 +399,26 @@
                 if value is None and self.null
                 else self.enumeration[super().python_value(value)]
             )
         except KeyError:
             raise peewee.IntegrityError(
                 f"Enum {self.enumeration.__name__} has no value with name '{value}'"
             ) from None
+
+
+class TimedeltaField(peewee.BigIntegerField):
+    """Field class for storing python-native Timedelta objects
+
+    This is really just a helper wrapper around an integer field that performs the second conversions
+    automatically. It is a helpful helper though, so it's included.
+
+    .. note:: To avoid issues with float precision, this field stores the database value as an integer.
+              However, this necessitates the usage of the BigInt type to avoid overflowing the value.
+              Essentially, the value this field ends up storing is the number of microseconds in the
+              timedelta.
+    """
+
+    def db_value(self, value: datetime.timedelta) -> int:
+        return super().db_value(int(value.total_seconds() * 1000000))
+
+    def python_value(self, value: int) -> datetime.timedelta:
+        return datetime.timedelta(seconds=super().python_value(value) / 1000000)
```

### Comparing `peewee_plus-1.2.1/pyproject.toml` & `peewee_plus-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-plus"
-version = "1.2.1"
+version = "1.3.0"
 description = "Various extensions, helpers, and utilities for Peewee"
 authors = ["Ethan Paul <24588726+enpaul@users.noreply.github.com>"]
 repository = "https://github.com/enpaul/peewee-plus/"
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "peewee_plus.py"},
@@ -51,16 +51,16 @@
 bandit = {version = "^1.7.1", python = "^3.10"}
 poetry = {version = "^1.4.2", python = "^3.10"}
 safety = {version = "^2.2.0", python = "^3.10"}
 
 [tool.poetry.group.static.dependencies]
 black = {version = "^22.8.0", python = "^3.10"}
 blacken-docs = {version = "^1.12.0", python = "^3.10"}
-mdformat = {version = "^0.6.4", python = "^3.10"}
-mdformat-gfm = {version = "^0.2", python = "^3.10"}
+mdformat = {version = "^0.7.16", python = "^3.10"}
+mdformat-gfm = {version = "^0.3.5", python = "^3.10"}
 mypy = {version = "^1.2.0", python = "^3.10"}
 pre-commit = {version = "^2.15.0", python = "^3.10"}
 pre-commit-hooks = {version = "^4.0.1", python = "^3.10"}
 pylint = {version = "^2.13.0", python = "^3.10"}
 reorder-python-imports = {version = "^2.6.0", python = "^3.10"}
 toml = {version = "^0.10.2", python = "^3.10"}
 types-toml = {version = "^0.10.1", python = "^3.10"}
```

### Comparing `peewee_plus-1.2.1/tests/test_about.py` & `peewee_plus-1.3.0/tests/test_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,7 +27,14 @@
     assert (
         all(
             item in pyproject["tool"]["poetry"]["authors"]
             for item in peewee_plus.__authors__
         )
         is True
     )
+
+
+def test_all():
+    """Test that the string entries in ``__all__`` are correct"""
+
+    for item in peewee_plus.__all__:
+        assert hasattr(peewee_plus, item)
```

### Comparing `peewee_plus-1.2.1/tests/test_calc_batch_size.py` & `peewee_plus-1.3.0/tests/test_calc_batch_size.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 # pylint: disable=unused-import
 import peewee
 
 import peewee_plus
 from .fixtures import fakedb
 
 
+def test_public_api():
+    """Test that the public API components are exposed via ``__all__``"""
+
+    assert peewee_plus.calc_batch_size.__name__ in peewee_plus.__all__
+    assert peewee_plus.flat_transaction.__name__ in peewee_plus.__all__
+    assert "SQLITE_DEFAULT_VARIABLE_LIMIT" in peewee_plus.__all__
+    assert "SQLITE_DEFAULT_PRAGMAS" in peewee_plus.__all__
+
+
 def test_sqlite(fakedb):
     """Test the calculation of batch sizes on SQLite"""
 
     class TestModel(peewee.Model):
         class Meta:
             database = fakedb
```

### Comparing `peewee_plus-1.2.1/tests/test_enumfield.py` & `peewee_plus-1.3.0/tests/test_enum_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 import peewee
 import pytest
 
 import peewee_plus
 from .fixtures import fakedb
 
 
+def test_public_api():
+    """Test that the public API components are exposed via ``__all__``"""
+
+    assert peewee_plus.EnumField.__name__ in peewee_plus.__all__
+
+
 def test_enum(fakedb):
     """Test basic functionality of the enum field"""
 
     class TestEnum(enum.Enum):
         FOO = "fizz"
         BAR = "buzz"
```

### Comparing `peewee_plus-1.2.1/tests/test_pathfield.py` & `peewee_plus-1.3.0/tests/test_path_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 import peewee
 
 import peewee_plus
 from .fixtures import fakedb
 
 
+def test_public_api():
+    """Test that the public API components are exposed via ``__all__``"""
+
+    assert peewee_plus.PathField.__name__ in peewee_plus.__all__
+
+
 def test_conversion(fakedb):
     """Test basic usage of PathField for roundtrip compatibility"""
 
     class TestModel(peewee.Model):
         class Meta:
             database = fakedb
```

### Comparing `peewee_plus-1.2.1/tests/test_precision_float_field.py` & `peewee_plus-1.3.0/tests/test_precision_float_field.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 # pylint: disable=too-few-public-methods
 import peewee
 
 import peewee_plus
 from .fixtures import fakedb
 
 
+def test_public_api():
+    """Test that the public API components are exposed via ``__all__``"""
+
+    assert peewee_plus.PrecisionFloatField.__name__ in peewee_plus.__all__
+
+
 # There isn't anything we can really test here since this field implements
 # a MySQL-specific syntax and we test with SQLite. This test is here just
 # to ensure that the behavior is consistent with the normal FloatField when
 # working with an unsupported database backend
 def test_compatibility(fakedb):
     """Check that the precision float field works on sqlite"""
```

### Comparing `peewee_plus-1.2.1/PKG-INFO` & `peewee_plus-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-plus
-Version: 1.2.1
+Version: 1.3.0
 Summary: Various extensions, helpers, and utilities for Peewee
 Home-page: https://github.com/enpaul/peewee-plus/
 License: MIT
 Keywords: peewee,orm,extension,plguin,extra
 Author: Ethan Paul
 Author-email: 24588726+enpaul@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -42,15 +42,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 See the [Changelog](https://github.com/enpaul/peewee-plus/blob/devel/CHANGELOG.md) for
 release history.
 
 ## Documentation
 
-*The documentation for this project is currently a work in progress. Please see the source code for complete docs*
+*The documentation for this project is currently a work in progress. Please see the source
+code for complete docs*
 
 - [Installing](#installing)
 - [Features](#features)
 - [For Developers](#for-developers)
 
 ## Installing
 
@@ -85,42 +86,44 @@
 [Peewee docs](http://docs.peewee-orm.com/en/latest/peewee/database.html#recommended-settings).
 
 `SQLITE_DEFAULT_VARIABLE_LIMIT` - The maximum number of variables an SQL query can use
 when using SQLite
 
 ### Functions
 
-[`calc_batch_size`](blob/devel/peewee_plus.py#L93) - Helper function for writing
-backend-agnostic batch queries while accounting for the
+`calc_batch_size` - Helper function for writing backend-agnostic batch queries while
+accounting for the
 [SQLite max variable limit](https://www.sqlite.org/limits.html#max_variable_number).
 
-[`flat_transaction`](blob/devel/peewee_plus.py#L159) - Decorator function for wrapping
-callables in a database transaction without creating nested transactions
+`flat_transaction` - Decorator function for wrapping callables in a database transaction
+without creating nested transactions
 
 ### Classes
 
-[`PathField`](blob/devel/peewee_plus.py#204) - A Peewee database field for storing
+`PathField` - A Peewee database field for storing
 [Pathlib](https://docs.python.org/3/library/pathlib.html) objects, optionally relative to
 a runtime value.
 
-[`PrecisionFloatField`](blob/devel/peewee_plus.py#L262) - A Peewee database field for
-storing floats while specifying the
+`PrecisionFloatField` - A Peewee database field for storing floats while specifying the
 [MySQL precision parameters](https://dev.mysql.com/doc/refman/8.0/en/floating-point-types.html)
 `M` and `D`
 
-[`JSONField`](blob/devel/peewee_plus.py#L293) - A Peewee database field for storing
-arbitrary JSON-serializable data
+`JSONField` - A Peewee database field for storing arbitrary JSON-serializable data
 
-[`EnumField`](blob/devel/peewee_plus.py#L348) - A Peewee database field for storing Enums
-by name
+`EnumField` - A Peewee database field for storing Enums by name
+
+`TimedeltaField` A Peewee database field for natively storing
+[`datetime.timedelta`](https://docs.python.org/3/library/datetime.html#datetime.timedelta)
+objects
 
 ## For Developers
 
 All project contributors and participants are expected to adhere to the
-[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md) ([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
+[Contributor Covenant Code of Conduct, v2](CODE_OF_CONDUCT.md)
+([external link](https://www.contributor-covenant.org/version/2/0/code_of_conduct/)).
 
 The `devel` branch has the latest (and potentially unstable) changes. The stable releases
 are tracked on [Github](https://github.com/enpaul/peewee-plus/releases),
 [PyPi](https://pypi.org/project/peewee-plus/#history), and in the
 [Changelog](CHANGELOG.md).
 
 - To report a bug, request a feature, or ask for assistance, please
```

