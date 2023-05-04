# Comparing `tmp/themis-imager-readfile-1.0.9.tar.gz` & `tmp/themis_imager_readfile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis-imager-readfile-1.0.9.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.1.0.tar", max compression
```

## Comparing `themis-imager-readfile-1.0.9.tar` & `themis_imager_readfile-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.677225 themis-imager-readfile-1.0.9/LICENSE
--rw-r--r--   0        0        0     2347 2021-02-25 18:30:55.388189 themis-imager-readfile-1.0.9/README.md
--rw-r--r--   0        0        0      655 2021-06-24 15:13:55.137695 themis-imager-readfile-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       49 2021-06-24 15:13:55.209695 themis-imager-readfile-1.0.9/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8223 2021-06-24 15:12:24.501695 themis-imager-readfile-1.0.9/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3132 2021-06-24 15:14:03.376572 themis-imager-readfile-1.0.9/setup.py
--rw-r--r--   0        0        0     3098 2021-06-24 15:14:03.376946 themis-imager-readfile-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2475 2023-05-04 21:32:07.373602 themis_imager_readfile-1.1.0/README.md
+-rw-r--r--   0        0        0      660 2023-05-04 21:29:32.176684 themis_imager_readfile-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-04 21:29:32.214684 themis_imager_readfile-1.1.0/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8458 2021-11-17 16:36:55.000000 themis_imager_readfile-1.1.0/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.0/PKG-INFO
```

### Comparing `themis-imager-readfile-1.0.9/LICENSE` & `themis_imager_readfile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `themis-imager-readfile-1.0.9/README.md` & `themis_imager_readfile-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/themis-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/themis-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![PyPI Python versions](https://img.shields.io/pypi/pyversions/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)
 
 Python library for reading THEMIS All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca or http://themis.igpp.ucla.edu/index.shtml.
 
+## Supported Datasets
+
+- THEMIS ASI raw: [stream0](https://data.phys.ucalgary.ca/sort_by_project/THEMIS/asi/stream0) PGM files
+
 ## Installation
 
 The themis-imager-readfile library is available on PyPI:
 
 ```console
 $ python3 -m pip install themis-imager-readfile
 ```
 
 ## Supported Python Versions
 
-themis-imager-readfile officially supports Python 3.6+.
+themis-imager-readfile officially supports Python 3.8+.
 
 ## Examples
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
```

### Comparing `themis-imager-readfile-1.0.9/pyproject.toml` & `themis_imager_readfile-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.0.9"
+version = "1.1.0"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "themis_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.19.2"
+python = "^3.8.1"
+numpy = "^1.24.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^3.8.4"
-pylint = "^2.6.0"
+pytest = "^7.0.0"
+flake8 = "^6.0.0"
+pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `themis-imager-readfile-1.0.9/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.1.0/themis_imager_readfile/_themis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Author: Lukas Vollmerhaus
 # Date: 2020-10-16
 
 import gzip
+import bz2
 import numpy as np
 import signal
 from multiprocessing import Pool
 
 # globals
 THEMIS_IMAGE_SIZE_BYTES = 131072
 THEMIS_DT = np.dtype("uint16")
@@ -106,16 +107,20 @@
 
     # check file extension to see if it's gzipped or not
     try:
         if file.endswith("pgm.gz"):
             unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
+        elif file.endswith("pgm.bz2"):
+            unzipped = bz2.open(file, mode='rb')
         else:
             print("Unrecognized file type: %s" % (file))
+            problematic = True
+            error_message = "Unrecognized file type"
             return images, metadata_dict_list, problematic, file, error_message
     except Exception as e:
         print("Failed to open file '%s' " % (file))
         problematic = True
         error_message = "failed to open file: %s" % (str(e))
         return images, metadata_dict_list, problematic, file, error_message
 
@@ -169,15 +174,15 @@
             if ("Imager unique ID" not in metadata_dict):
                 metadata_dict["Imager unique ID"] = device_uid
             else:
                 device_uid = metadata_dict["Imager unique ID"]
 
             # split dictionaries up per frame, exposure plus initial readout is
             # always the end of metadata for frame
-            if (key.startswith("Exposure plus initial readout")):
+            if (key.startswith("Exposure plus initial readout") or key.startswith("Exposure duration plus readout")):
                 metadata_dict_list.append(metadata_dict)
                 metadata_dict = {}
         elif line == b'65535\n':
             # there are 2 lines between "exposure plus read out" and the image
             # data, the first is b'256 256\n' and the second is b'65535\n'
             #
             # read image
```

### Comparing `themis-imager-readfile-1.0.9/setup.py` & `themis_imager_readfile-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: themis-imager-readfile
+Version: 1.1.0
+Summary: Read functions for THEMIS ASI PGM raw files
+Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
+License: MIT
+Author: Darren Chaddock
+Author-email: dchaddoc@ucalgary.ca
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Project-URL: Repository, https://github.com/ucalgary-aurora/themis-imager-readfile
+Description-Content-Type: text/markdown
 
-packages = \
-['themis_imager_readfile']
+# THEMIS All-Sky Imager Raw PGM Data Readfile
 
-package_data = \
-{'': ['*']}
+[![Github Actions - Tests](https://github.com/ucalgary-aurora/themis-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/themis-imager-readfile/actions?query=workflow%3Atests)
+[![PyPI version](https://img.shields.io/pypi/v/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![PyPI Python versions](https://img.shields.io/pypi/pyversions/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)
 
-install_requires = \
-['numpy>=1.19.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'themis-imager-readfile',
-    'version': '1.0.9',
-    'description': 'Read functions for THEMIS ASI PGM raw files',
-    'long_description': '# THEMIS All-Sky Imager Raw PGM Data Readfile\n\n[![Github Actions - Tests](https://github.com/ucalgary-aurora/themis-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/themis-imager-readfile/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://img.shields.io/pypi/pyversions/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)\n\nPython library for reading THEMIS All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca or http://themis.igpp.ucla.edu/index.shtml.\n\n## Installation\n\nThe themis-imager-readfile library is available on PyPI:\n\n```console\n$ python3 -m pip install themis-imager-readfile\n```\n\n## Supported Python Versions\n\nthemis-imager-readfile officially supports Python 3.6+.\n\n## Examples\n\nExample Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.\n\n## Usage\n\nImport the library using `import themis_imager_readfile`\n\n### Read a single file\n\n```python\n>>> import themis_imager_readfile\n>>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"\n>>> img, meta, problematic_files = themis_imager_readfile.read(filename)\n```\n\n### Read multiple files\n\n```python\n>>> import themis_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")\n>>> img, meta, problematic_files = themis_imager_readfile.read(file_list)\n```\n\n### Read using multiple worker processes\n\n```python\n>>> import themis_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")\n>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4)\n```\n\n## Development\n\nClone the repository and install dependencies using Poetry.\n\n```console\n$ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git\n$ cd themis-imager-readfile/python\n$ make install\n```\n\n## Testing\n\n```console\n$ make test\n[ or do each test separately ]\n$ make test-flake8\n$ make test-pylint\n$ make test-pytest\n```\n',
-    'author': 'Darren Chaddock',
-    'author_email': 'dchaddoc@ucalgary.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ucalgary-aurora/themis-imager-readfile',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+Python library for reading THEMIS All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca or http://themis.igpp.ucla.edu/index.shtml.
 
+## Supported Datasets
+
+- THEMIS ASI raw: [stream0](https://data.phys.ucalgary.ca/sort_by_project/THEMIS/asi/stream0) PGM files
+
+## Installation
+
+The themis-imager-readfile library is available on PyPI:
+
+```console
+$ python3 -m pip install themis-imager-readfile
+```
+
+## Supported Python Versions
+
+themis-imager-readfile officially supports Python 3.8+.
+
+## Examples
+
+Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
+
+## Usage
+
+Import the library using `import themis_imager_readfile`
+
+### Read a single file
+
+```python
+>>> import themis_imager_readfile
+>>> filename = "path/to/data/2020/01/01/atha_themis02/ut06/20200101_0600_atha_themis02_full.pgm.gz"
+>>> img, meta, problematic_files = themis_imager_readfile.read(filename)
+```
+
+### Read multiple files
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list)
+```
+
+### Read using multiple worker processes
+
+```python
+>>> import themis_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/atha_themis02/ut06/*full.pgm*")
+>>> img, meta, problematic_files = themis_imager_readfile.read(file_list, workers=4)
+```
+
+## Development
+
+Clone the repository and install dependencies using Poetry.
+
+```console
+$ git clone https://github.com/ucalgary-aurora/themis-imager-readfile.git
+$ cd themis-imager-readfile/python
+$ make install
+```
+
+## Testing
+
+```console
+$ make test
+[ or do each test separately ]
+$ make test-flake8
+$ make test-pylint
+$ make test-pytest
+```
 
-setup(**setup_kwargs)
```

