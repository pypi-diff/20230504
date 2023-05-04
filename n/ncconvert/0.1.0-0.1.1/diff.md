# Comparing `tmp/ncconvert-0.1.0.tar.gz` & `tmp/ncconvert-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncconvert-0.1.0.tar", last modified: Wed Apr 26 23:53:03 2023, max compression
+gzip compressed data, was "ncconvert-0.1.1.tar", last modified: Thu May  4 18:57:12 2023, max compression
```

## Comparing `ncconvert-0.1.0.tar` & `ncconvert-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.231469 ncconvert-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 23:52:52.000000 ncconvert-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.227469 ncconvert-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.231469 ncconvert-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-26 23:52:52.000000 ncconvert-0.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-26 23:52:52.000000 ncconvert-0.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 23:52:52.000000 ncconvert-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 23:52:52.000000 ncconvert-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-26 23:53:03.231469 ncconvert-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-26 23:52:52.000000 ncconvert-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-26 23:52:52.000000 ncconvert-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 23:53:03.231469 ncconvert-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-26 23:52:52.000000 ncconvert-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.227469 ncconvert-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.231469 ncconvert-0.1.0/src/ncconvert/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-26 23:52:52.000000 ncconvert-0.1.0/src/ncconvert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.231469 ncconvert-0.1.0/src/ncconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 23:53:03.000000 ncconvert-0.1.0/src/ncconvert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 23:53:03.231469 ncconvert-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-26 23:52:52.000000 ncconvert-0.1.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-26 23:52:52.000000 ncconvert-0.1.0/test/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-26 23:52:52.000000 ncconvert-0.1.0/test/test_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.195913 ncconvert-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 18:57:00.000000 ncconvert-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 18:57:00.000000 ncconvert-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 18:57:12.199913 ncconvert-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-04 18:57:00.000000 ncconvert-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 18:57:00.000000 ncconvert-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:57:12.199913 ncconvert-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 18:57:00.000000 ncconvert-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/ncconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-04 18:57:00.000000 ncconvert-0.1.1/src/ncconvert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/src/ncconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 18:57:12.000000 ncconvert-0.1.1/src/ncconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:57:12.199913 ncconvert-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-04 18:57:00.000000 ncconvert-0.1.1/test/test_parquet.py
```

### Comparing `ncconvert-0.1.0/.github/workflows/pypi.yml` & `ncconvert-0.1.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.0/.github/workflows/pytest.yml` & `ncconvert-0.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.0/pyproject.toml` & `ncconvert-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,34 @@
 [project.optional-dependencies]
 dev = [
   "pytest",
   "coverage",
   "build",
   "black",
   "ruff",
+  "isort",
 ]
 
 cli = [
   "typer",
+  "tqdm",
   "rich",
 ]
 
+[project.scripts]
+ncconvert = "ncconvert.cli:app"
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 ncconvert = ["py.typed"]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/ncconvert/_version.py"
 
 [tool.setuptools.dynamic]
-version = {attr = "ncconvert.__version__"}
+version = {attr = "ncconvert._version.__version__"}
```

### Comparing `ncconvert-0.1.0/src/ncconvert/csv.py` & `ncconvert-0.1.1/src/ncconvert/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Dict
 
 import xarray as xr
-from .utils import _to_dataframe_collection, _to_dataframe, _dump_metadata
+
+from .utils import _dump_metadata, _to_dataframe, _to_dataframe_collection
 
 
 def to_csv(
     dataset: xr.Dataset,
     filepath: str | Path,
     to_csv_kwargs: Dict[str, Any] | None = None,
 ) -> tuple[Path, Path]:
@@ -29,15 +30,15 @@
             file.
     """
     if to_csv_kwargs is None:
         to_csv_kwargs = {}
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
-    filepath, df = _to_dataframe(dataset, filepath)
+    filepath, df = _to_dataframe(dataset, filepath, ".csv")
     df.to_csv(filepath, **to_csv_kwargs)  # type: ignore
 
     metadata_path = _dump_metadata(dataset, filepath)
 
     return Path(filepath), metadata_path
 
 
@@ -80,7 +81,13 @@
     for fpath, df in data_groups:
         df.to_csv(fpath, **to_csv_kwargs)
         filepaths.append(fpath)
 
     metadata_path = _dump_metadata(dataset, filepath)
 
     return tuple(filepaths), metadata_path
+
+
+def to_timestream_csv():
+    ...
+
+    # tuple(filepaths), metadata_path
```

### Comparing `ncconvert-0.1.0/src/ncconvert/parquet.py` & `ncconvert-0.1.1/src/ncconvert/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Dict
 
 import xarray as xr
-from .utils import _to_dataframe_collection, _to_dataframe, _dump_metadata
+
+from .utils import _dump_metadata, _to_dataframe, _to_dataframe_collection
 
 
 def to_parquet(
     dataset: xr.Dataset,
     filepath: str | Path,
     to_parquet_kwargs: Dict[str, Any] | None = None,
 ) -> tuple[Path, Path]:
@@ -29,15 +30,15 @@
             file.
     """
     if to_parquet_kwargs is None:
         to_parquet_kwargs = {}
 
     Path(filepath).parent.mkdir(parents=True, exist_ok=True)
 
-    filepath, df = _to_dataframe(dataset, filepath)
+    filepath, df = _to_dataframe(dataset, filepath, ".parquet")
     df.to_parquet(filepath, **to_parquet_kwargs)  # type: ignore
 
     metadata_path = _dump_metadata(dataset, filepath)
 
     return Path(filepath), metadata_path
```

### Comparing `ncconvert-0.1.0/src/ncconvert/utils.py` & `ncconvert-0.1.1/src/ncconvert/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-from collections import defaultdict
 import json
+from collections import defaultdict
 from pathlib import Path
-import pandas as pd
 
+import pandas as pd
 import xarray as xr
 
 
 def _dump_metadata(dataset: xr.Dataset, filepath: str | Path) -> Path:
     metadata = dataset.to_dict(data=False, encoding=True)
-    metadata_json = json.dumps(metadata, indent=4)
+    metadata_json = json.dumps(metadata, default=str, indent=4)
     metadata_path = Path(filepath).with_suffix(".json")
     metadata_path.write_text(metadata_json)
     return metadata_path
 
 
 def _to_dataframe(
-    dataset: xr.Dataset, filepath: str | Path
+    dataset: xr.Dataset, filepath: str | Path, extension: str
 ) -> tuple[Path, pd.DataFrame]:
+    if not extension.startswith("."):
+        extension = "." + extension
+
     df = dataset.to_dataframe(dim_order=list(dataset.dims))
 
-    return Path(filepath), df
+    return Path(filepath).with_suffix(extension), df
 
 
 def _to_dataframe_collection(
     dataset: xr.Dataset, filepath: str | Path, extension: str
 ) -> tuple[tuple[Path, pd.DataFrame], ...]:
     outputs: list[tuple[Path, pd.DataFrame]] = []
```

### Comparing `ncconvert-0.1.0/src/ncconvert.egg-info/SOURCES.txt` & `ncconvert-0.1.1/src/ncconvert.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 pyproject.toml
 setup.py
 .github/workflows/pypi.yml
 .github/workflows/pytest.yml
 src/ncconvert/__init__.py
 src/ncconvert/__main__.py
 src/ncconvert/_version.py
+src/ncconvert/cli.py
 src/ncconvert/csv.py
 src/ncconvert/parquet.py
 src/ncconvert/py.typed
 src/ncconvert/utils.py
 src/ncconvert.egg-info/PKG-INFO
 src/ncconvert.egg-info/SOURCES.txt
 src/ncconvert.egg-info/dependency_links.txt
+src/ncconvert.egg-info/entry_points.txt
 src/ncconvert.egg-info/requires.txt
 src/ncconvert.egg-info/top_level.txt
 test/conftest.py
+test/test_cli.py
 test/test_csv.py
 test/test_parquet.py
```

### Comparing `ncconvert-0.1.0/test/conftest.py` & `ncconvert-0.1.1/test/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import pytest
-
 import pandas as pd
+import pytest
 import xarray as xr
 
 
 @pytest.fixture(autouse=True, scope="module")
 def dataset() -> xr.Dataset:
     return xr.Dataset(
         coords={
```

### Comparing `ncconvert-0.1.0/test/test_csv.py` & `ncconvert-0.1.1/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `ncconvert-0.1.0/test/test_parquet.py` & `ncconvert-0.1.1/test/test_parquet.py`

 * *Files identical despite different names*

