# Comparing `tmp/honkaistarrail-0.0.2.tar.gz` & `tmp/honkaistarrail-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkaistarrail-0.0.2.tar", max compression
+gzip compressed data, was "honkaistarrail-0.0.3.tar", max compression
```

## Comparing `honkaistarrail-0.0.2.tar` & `honkaistarrail-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.2/honkaistarrail/calculator.py
--rw-r--r--   0        0        0     1246 2023-04-30 01:48:24.518000 honkaistarrail-0.0.2/honkaistarrail/modal.py
--rw-r--r--   0        0        0     4612 2023-04-30 02:10:08.645612 honkaistarrail-0.0.2/honkaistarrail/starrail.py
--rw-r--r--   0        0        0      480 2023-04-30 02:50:31.766312 honkaistarrail-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1080 2023-04-30 02:50:22.110995 honkaistarrail-0.0.2/README.md
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 honkaistarrail-0.0.2/setup.py
--rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 honkaistarrail-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.3/honkaistarrail/calculator.py
+-rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.3/honkaistarrail/modal.py
+-rw-r--r--   0        0        0    29135 2023-05-04 13:30:29.205747 honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
+-rw-r--r--   0        0        0    38022 2023-05-04 13:30:26.497309 honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/gacha_data.py
+-rw-r--r--   0        0        0     6803 2023-05-04 13:50:38.210012 honkaistarrail-0.0.3/honkaistarrail/starrail.py
+-rw-r--r--   0        0        0      480 2023-05-04 14:14:45.073560 honkaistarrail-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.3/README.md
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.3/setup.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.3/PKG-INFO
```

### Comparing `honkaistarrail-0.0.2/honkaistarrail/calculator.py` & `honkaistarrail-0.0.3/honkaistarrail/calculator.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.2/honkaistarrail/modal.py` & `honkaistarrail-0.0.3/honkaistarrail/modal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from pydantic import BaseModel
 from datetime import datetime
 from typing import List
 
 
+class ImageGacha(BaseModel):
+    icon: str
+    full: str
+
 class JumpRecord(BaseModel):
     uid: int
     id: int
     name: str
     rank: str
     count: int
     type: str
```

### Comparing `honkaistarrail-0.0.2/setup.py` & `honkaistarrail-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['honkaistarrail']
+['honkaistarrail', 'honkaistarrail.src.data.gacha']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkaistarrail',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Asynchronous module for working with API Honkai: Star Rail',
-    'long_description': '# HonkaiStarRail.py\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link,3,"en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n',
+    'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/HSR-BANNER.png" />\n</p>\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\nPyPi: [OPEN](https://pypi.org/project/honkaistarrail/)\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n### ID Banned:\n``1`` - Event Banner\n``2`` - Light Cone\n``3`` - Standart Banner\n\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link = link,banner = 1,lang = "en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\n\n# In developing:\n\n1. Automatic code redemption.\n2. Automatic collection of daily marks on HoYoLab.\n\n___\n<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/%D0%91%D0%B5%D0%B7-%D0%B8%D0%BC%D0%B5%D0%BD%D0%B8-1.png" />\n</p>\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiStarRail.py',
     'packages': packages,
     'package_data': package_data,
```

