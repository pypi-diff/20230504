# Comparing `tmp/pz-rail-pipelines-0.0.2.tar.gz` & `tmp/pz-rail-pipelines-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-pipelines-0.0.2.tar", last modified: Thu Sep  8 21:28:50 2022, max compression
+gzip compressed data, was "pz-rail-pipelines-0.0.3.tar", last modified: Thu May  4 06:17:22 2023, max compression
```

## Comparing `pz-rail-pipelines-0.0.2.tar` & `pz-rail-pipelines-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/nb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/nb/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/nb/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/nb/examples/goldenspike/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-09-08 21:28:50.000000 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-08 21:28:50.000000 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 21:28:50.000000 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-08 21:28:50.000000 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-08 21:28:50.000000 pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/src/rail/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/src/rail/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-08 21:28:48.000000 pz-rail-pipelines-0.0.2/src/rail/pipelines/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.462009 pz-rail-pipelines-0.0.2/src/rail/pipelines/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/src/rail/pipelines/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (121)     7518 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/src/rail/pipelines/examples/goldenspike/goldenspike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/src/rail/pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/src/rail/pipelines/utils/name_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 21:28:50.466009 pz-rail-pipelines-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-08 21:28:22.000000 pz-rail-pipelines-0.0.2/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/nb/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/nb/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/nb/examples/goldenspike/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2932 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-05-04 06:17:22.000000 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-05-04 06:17:22.000000 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 06:17:22.000000 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-04 06:17:22.000000 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 06:17:22.000000 pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/src/rail/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/src/rail/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 06:17:21.000000 pz-rail-pipelines-0.0.3/src/rail/pipelines/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.955373 pz-rail-pipelines-0.0.3/src/rail/pipelines/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/src/rail/pipelines/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (122)     7533 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/src/rail/pipelines/examples/goldenspike/goldenspike.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/src/rail/pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/src/rail/pipelines/utils/name_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:17:22.959374 pz-rail-pipelines-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-04 06:17:03.000000 pz-rail-pipelines-0.0.3/tests/test_pipelines.py
```

### Comparing `pz-rail-pipelines-0.0.2/.github/workflows/main.yml` & `pz-rail-pipelines-0.0.3/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install wheel numpy
         pip install .
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi			
     - name: Test with pytest
       run: |
         python -m pytest --cov=rail.pipelines --cov-report=xml
     - name: Upload coverage to Codecov
```

### Comparing `pz-rail-pipelines-0.0.2/.github/workflows/pypi.yaml` & `pz-rail-pipelines-0.0.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.2/.gitignore` & `pz-rail-pipelines-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.2/LICENSE` & `pz-rail-pipelines-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.2/PKG-INFO` & `pz-rail-pipelines-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.0.2
+Version: 0.0.3
 Summary: RAIL pipelines
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-pipelines-0.0.2/nb/examples/goldenspike/goldenspike.ipynb` & `pz-rail-pipelines-0.0.3/nb/examples/goldenspike/goldenspike.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.985646645021645%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(1, "flow_file = os.path.join(RAILDIR, '*

 * *            '\'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl\')\\n"), (2, '*

 * *            '"pipe.initialize(dict(model=flow_file), dict(output_dir=\'.\', log_dir=\'.\', '*

 * *            'resume=False), None)")], delete: [2, 1]}}, delete: [2]}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -20,24 +20,14 @@
                 "from rail.core.utils import RAILDIR\n",
                 "from rail.pipelines.examples.goldenspike.goldenspike import GoldenspikePipeline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "54cae849",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "flow_file = os.path.join(RAILDIR, 'examples/goldenspike/data/pretrained_flow.pkl')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "b972d07a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "pipe = GoldenspikePipeline()"
             ]
         },
@@ -45,16 +35,16 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "23efbbb5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from rail.core.utils import RAILDIR\n",
-                "flow_file = os.path.join(RAILDIR, 'examples/goldenspike/data/pretrained_flow.pkl')\n",
-                "pipe.initialize(dict(flow=flow_file), dict(output_dir='.', log_dir='.', resume=False), None)"
+                "flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')\n",
+                "pipe.initialize(dict(model=flow_file), dict(output_dir='.', log_dir='.', resume=False), None)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "67532a42",
             "metadata": {},
@@ -125,13 +115,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-pipelines-0.0.2/pyproject.toml` & `pz-rail-pipelines-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
-    "pz-rail-hub>=0.0.3",
+    "pz-rail-hub>=0.0.4",
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
     "pylint",
     "pytest",
```

### Comparing `pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/PKG-INFO` & `pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.0.2
+Version: 0.0.3
 Summary: RAIL pipelines
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-pipelines-0.0.2/src/pz_rail_pipelines.egg-info/SOURCES.txt` & `pz-rail-pipelines-0.0.3/src/pz_rail_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.2/src/rail/pipelines/examples/goldenspike/goldenspike.py` & `pz-rail-pipelines-0.0.3/src/rail/pipelines/examples/goldenspike/goldenspike.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from rail.core.stage import RailStage, RailPipeline
 
 import ceci
 
 
 namer = NameFactory()
 from rail.core.utils import RAILDIR
-flow_file = os.path.join(RAILDIR, 'examples/goldenspike/data/pretrained_flow.pkl')
+flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')
 
 
 class GoldenspikePipeline(RailPipeline):
 
     def __init__(self):
         RailPipeline.__init__(self)
```

### Comparing `pz-rail-pipelines-0.0.2/src/rail/pipelines/utils/name_factory.py` & `pz-rail-pipelines-0.0.3/src/rail/pipelines/utils/name_factory.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.2/tests/test_pipelines.py` & `pz-rail-pipelines-0.0.3/tests/test_pipelines.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
 from rail.core.utils import RAILDIR
 
 
 def test_golden():
     namer = NameFactory()
-    flow_file = os.path.join(RAILDIR, 'examples/goldenspike/data/pretrained_flow.pkl')
+    flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')
     output_dir = namer.get_project_dir('.', 'tmp_test', 'tmp_test')
     try:
         os.makedirs(output_dir)
     except OSError:  # pragma: no cover
         pass    
     pipe = GoldenspikePipeline()
     pipe.initialize(dict(model=flow_file), dict(output_dir=output_dir, log_dir=output_dir, resume=False), None)
```

