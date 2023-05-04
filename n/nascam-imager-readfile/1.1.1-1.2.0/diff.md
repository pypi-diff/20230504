# Comparing `tmp/nascam_imager_readfile-1.1.1.tar.gz` & `tmp/nascam_imager_readfile-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nascam_imager_readfile-1.1.1.tar", max compression
+gzip compressed data, was "nascam_imager_readfile-1.2.0.tar", max compression
```

## Comparing `nascam_imager_readfile-1.1.1.tar` & `nascam_imager_readfile-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.1.1/LICENSE
--rw-r--r--   0        0        0     2513 2023-01-03 00:16:12.612892 nascam_imager_readfile-1.1.1/README.md
--rw-r--r--   0        0        0       49 2023-02-18 20:01:52.266525 nascam_imager_readfile-1.1.1/nascam_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8183 2023-02-18 20:01:20.250518 nascam_imager_readfile-1.1.1/nascam_imager_readfile/_nascam.py
--rw-r--r--   0        0        0      680 2023-02-18 20:01:52.190525 nascam_imager_readfile-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.1.1/setup.py
--rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2513 2023-01-03 00:16:12.000000 nascam_imager_readfile-1.2.0/README.md
+-rw-r--r--   0        0        0       49 2023-05-04 21:35:49.239774 nascam_imager_readfile-1.2.0/nascam_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8183 2023-05-04 21:33:12.222821 nascam_imager_readfile-1.2.0/nascam_imager_readfile/_nascam.py
+-rw-r--r--   0        0        0      681 2023-05-04 21:35:49.204773 nascam_imager_readfile-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.2.0/PKG-INFO
```

### Comparing `nascam_imager_readfile-1.1.1/LICENSE` & `nascam_imager_readfile-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.1.1/README.md` & `nascam_imager_readfile-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.1.1/nascam_imager_readfile/_nascam.py` & `nascam_imager_readfile-1.2.0/nascam_imager_readfile/_nascam.py`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.1.1/pyproject.toml` & `nascam_imager_readfile-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nascam-imager-readfile"
-version = "1.1.1"
+version = "1.2.0"
 description = "Read functions for NASCAM ASI raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "nascam_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
-numpy = "^1.21.0"
-opencv-python = "^4.4.0"
+python = "^3.8.1"
+numpy = "^1.24.0"
+opencv-python = "^4.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
-flake8 = "^5.0.0"
-pylint = "^2.6.0"
+flake8 = "^6.0.0"
+pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nascam_imager_readfile-1.1.1/setup.py` & `nascam_imager_readfile-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nascam-imager-readfile
+Version: 1.2.0
+Summary: Read functions for NASCAM ASI raw files
+Home-page: https://github.com/ucalgary-aurora/nascam-imager-readfile
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
+Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
+Project-URL: Repository, https://github.com/ucalgary-aurora/nascam-imager-readfile
+Description-Content-Type: text/markdown
 
-packages = \
-['nascam_imager_readfile']
+# NASCAM All-Sky Imager Raw PGM Data Readfile
 
-package_data = \
-{'': ['*']}
+[![Github Actions - Tests](https://github.com/ucalgary-aurora/nascam-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/nascam-imager-readfile/actions?query=workflow%3Atests)
+[![PyPI version](https://img.shields.io/pypi/v/nascam-imager-readfile.svg)](https://pypi.python.org/pypi/nascam-imager-readfile/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/ucalgary-aurora/nascam-imager-readfile/blob/main/LICENSE)
+[![PyPI Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.python.org/pypi/nascam-imager-readfile/)
 
-install_requires = \
-['numpy>=1.21.0,<2.0.0', 'opencv-python>=4.4.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'nascam-imager-readfile',
-    'version': '1.1.1',
-    'description': 'Read functions for NASCAM ASI raw files',
-    'long_description': '# NASCAM All-Sky Imager Raw PGM Data Readfile\n\n[![Github Actions - Tests](https://github.com/ucalgary-aurora/nascam-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/nascam-imager-readfile/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/nascam-imager-readfile.svg)](https://pypi.python.org/pypi/nascam-imager-readfile/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/ucalgary-aurora/nascam-imager-readfile/blob/main/LICENSE)\n[![PyPI Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.python.org/pypi/nascam-imager-readfile/)\n\nPython library for reading NASCAM All-Sky Imager (ASI) stream0 raw PNG-file data. The data can be found at https://data.phys.ucalgary.ca.\n\n## Supported Datasets\n\n- NASCAM ASI raw: [stream0.png](https://data.phys.ucalgary.ca/sort_by_project/NORSTAR/nascam-msi/stream0.png) PNG files\n\n## Installation\n\nThe nascam-imager-readfile library is available on PyPI:\n\n```console\n$ python3 -m pip install nascam-imager-readfile\n```\n\n## Supported Python Versions\n\nnascam-imager-readfile officially supports Python 3.6+.\n\n## Examples\n\nExample Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.\n\n## Usage\n\nImport the library using `import nascam_imager_readfile`\n\n### Read a single file\n\n```python\n>>> import nascam_imager_readfile\n>>> filename = "path/to/data/2010/01/01/atha_nascam-iccd04/ut06/20100101_0600_atha_nascam-iccd04.png.tar"\n>>> img, meta, problematic_files = nascam_imager_readfile.read(filename)\n```\n\n### Read multiple files\n\n```python\n>>> import nascam_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")\n>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list)\n```\n\n### Read using multiple worker processes\n\n```python\n>>> import nascam_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")\n>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4)\n```\n\n## Development\n\nClone the repository and install dependencies using Poetry.\n\n```console\n$ git clone https://github.com/ucalgary-aurora/nascam-imager-readfile.git\n$ cd nascam-imager-readfile/python\n$ make install\n```\n\n## Testing\n\n```console\n$ make test\n[ or do each test separately ]\n$ make test-flake8\n$ make test-pylint\n$ make test-pytest\n```\n',
-    'author': 'Darren Chaddock',
-    'author_email': 'dchaddoc@ucalgary.ca',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ucalgary-aurora/nascam-imager-readfile',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+Python library for reading NASCAM All-Sky Imager (ASI) stream0 raw PNG-file data. The data can be found at https://data.phys.ucalgary.ca.
 
+## Supported Datasets
+
+- NASCAM ASI raw: [stream0.png](https://data.phys.ucalgary.ca/sort_by_project/NORSTAR/nascam-msi/stream0.png) PNG files
+
+## Installation
+
+The nascam-imager-readfile library is available on PyPI:
+
+```console
+$ python3 -m pip install nascam-imager-readfile
+```
+
+## Supported Python Versions
+
+nascam-imager-readfile officially supports Python 3.6+.
+
+## Examples
+
+Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
+
+## Usage
+
+Import the library using `import nascam_imager_readfile`
+
+### Read a single file
+
+```python
+>>> import nascam_imager_readfile
+>>> filename = "path/to/data/2010/01/01/atha_nascam-iccd04/ut06/20100101_0600_atha_nascam-iccd04.png.tar"
+>>> img, meta, problematic_files = nascam_imager_readfile.read(filename)
+```
+
+### Read multiple files
+
+```python
+>>> import nascam_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
+>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list)
+```
+
+### Read using multiple worker processes
+
+```python
+>>> import nascam_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2010/01/01/atha_nascam-iccd04/ut06/*.tar")
+>>> img, meta, problematic_files = nascam_imager_readfile.read(file_list, workers=4)
+```
+
+## Development
+
+Clone the repository and install dependencies using Poetry.
+
+```console
+$ git clone https://github.com/ucalgary-aurora/nascam-imager-readfile.git
+$ cd nascam-imager-readfile/python
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

