# Comparing `tmp/pylitterbot-2023.1.2.tar.gz` & `tmp/pylitterbot-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylitterbot-2023.1.2.tar", max compression
+gzip compressed data, was "pylitterbot-2023.4.0.tar", max compression
```

## Comparing `pylitterbot-2023.1.2.tar` & `pylitterbot-2023.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1076 2022-12-07 17:50:03.192551 pylitterbot-2023.1.2/LICENSE
--rw-r--r--   0        0        0     3177 2023-01-19 22:33:35.030091 pylitterbot-2023.1.2/README.md
--rw-r--r--   0        0        0      403 2023-01-19 22:36:40.169978 pylitterbot-2023.1.2/pylitterbot/__init__.py
--rw-r--r--   0        0        0     7546 2023-01-19 22:33:35.031260 pylitterbot-2023.1.2/pylitterbot/account.py
--rw-r--r--   0        0        0     1118 2022-12-07 18:02:31.737246 pylitterbot-2023.1.2/pylitterbot/activity.py
--rw-r--r--   0        0        0     4597 2023-01-19 22:33:35.031445 pylitterbot-2023.1.2/pylitterbot/enums.py
--rw-r--r--   0        0        0      348 2022-12-07 17:50:03.196005 pylitterbot-2023.1.2/pylitterbot/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-07 17:50:03.196040 pylitterbot-2023.1.2/pylitterbot/py.typed
--rw-r--r--   0        0        0     6838 2023-01-09 02:35:41.467367 pylitterbot-2023.1.2/pylitterbot/robot/__init__.py
--rw-r--r--   0        0        0    10459 2023-01-09 02:35:41.467599 pylitterbot-2023.1.2/pylitterbot/robot/feederrobot.py
--rw-r--r--   0        0        0     7187 2023-01-19 22:33:35.031678 pylitterbot-2023.1.2/pylitterbot/robot/litterrobot.py
--rw-r--r--   0        0        0    11704 2023-01-19 22:33:35.031877 pylitterbot-2023.1.2/pylitterbot/robot/litterrobot3.py
--rw-r--r--   0        0        0    25207 2023-01-19 22:33:35.032106 pylitterbot-2023.1.2/pylitterbot/robot/litterrobot4.py
--rw-r--r--   0        0        0     2364 2023-01-19 22:33:35.032287 pylitterbot-2023.1.2/pylitterbot/robot/models.py
--rw-r--r--   0        0        0     7738 2022-12-07 18:02:31.739910 pylitterbot-2023.1.2/pylitterbot/session.py
--rw-r--r--   0        0        0     2545 2023-01-19 22:33:35.032462 pylitterbot-2023.1.2/pylitterbot/utils.py
--rw-r--r--   0        0        0     5148 2023-01-09 02:35:41.468325 pylitterbot-2023.1.2/pylitterbot/ws_monitor.py
--rw-r--r--   0        0        0     1031 2023-01-19 22:36:40.170549 pylitterbot-2023.1.2/pyproject.toml
--rw-r--r--   0        0        0     4198 1970-01-01 00:00:00.000000 pylitterbot-2023.1.2/setup.py
--rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 pylitterbot-2023.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-12-07 17:50:03.192551 pylitterbot-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     3168 2023-04-20 15:27:40.760888 pylitterbot-2023.4.0/README.md
+-rw-r--r--   0        0        0      403 2023-04-20 15:28:39.998601 pylitterbot-2023.4.0/pylitterbot/__init__.py
+-rw-r--r--   0        0        0     7546 2023-01-19 22:33:35.031260 pylitterbot-2023.4.0/pylitterbot/account.py
+-rw-r--r--   0        0        0     1118 2022-12-07 18:02:31.737246 pylitterbot-2023.4.0/pylitterbot/activity.py
+-rw-r--r--   0        0        0     4597 2023-01-19 22:33:35.031445 pylitterbot-2023.4.0/pylitterbot/enums.py
+-rw-r--r--   0        0        0      348 2023-01-20 18:04:12.653826 pylitterbot-2023.4.0/pylitterbot/exceptions.py
+-rw-r--r--   0        0        0        0 2022-12-07 17:50:03.196040 pylitterbot-2023.4.0/pylitterbot/py.typed
+-rw-r--r--   0        0        0     6838 2023-01-09 02:35:41.467367 pylitterbot-2023.4.0/pylitterbot/robot/__init__.py
+-rw-r--r--   0        0        0    10446 2023-04-20 15:27:40.762530 pylitterbot-2023.4.0/pylitterbot/robot/feederrobot.py
+-rw-r--r--   0        0        0     7187 2023-01-19 22:33:35.031678 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot.py
+-rw-r--r--   0        0        0    11704 2023-01-19 22:33:35.031877 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot3.py
+-rw-r--r--   0        0        0    25329 2023-04-20 15:27:40.762808 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot4.py
+-rw-r--r--   0        0        0     2364 2023-01-19 22:33:35.032287 pylitterbot-2023.4.0/pylitterbot/robot/models.py
+-rw-r--r--   0        0        0     7738 2022-12-07 18:02:31.739910 pylitterbot-2023.4.0/pylitterbot/session.py
+-rw-r--r--   0        0        0     2545 2023-01-19 22:33:35.032462 pylitterbot-2023.4.0/pylitterbot/utils.py
+-rw-r--r--   0        0        0     5148 2023-01-09 02:35:41.468325 pylitterbot-2023.4.0/pylitterbot/ws_monitor.py
+-rw-r--r--   0        0        0     1027 2023-04-20 15:28:39.998966 pylitterbot-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pylitterbot-2023.4.0/setup.py
+-rw-r--r--   0        0        0     4138 1970-01-01 00:00:00.000000 pylitterbot-2023.4.0/PKG-INFO
```

### Comparing `pylitterbot-2023.1.2/LICENSE` & `pylitterbot-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/README.md` & `pylitterbot-2023.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```bash
 pip install pylitterbot
 ```
 
 Alternatively, clone the repository and run
 
 ```bash
-python setup.py install
+poetry install
 ```
 
 ## Usage
 
 ```python
 import asyncio
```

### Comparing `pylitterbot-2023.1.2/pylitterbot/account.py` & `pylitterbot-2023.4.0/pylitterbot/account.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/activity.py` & `pylitterbot-2023.4.0/pylitterbot/activity.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/enums.py` & `pylitterbot-2023.4.0/pylitterbot/enums.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/__init__.py` & `pylitterbot-2023.4.0/pylitterbot/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/feederrobot.py` & `pylitterbot-2023.4.0/pylitterbot/robot/feederrobot.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 COMMAND_ENDPOINT = (
     "https://42nk7qrhdg.execute-api.us-east-1.amazonaws.com/prod/command/feeder"
 )
 COMMAND_ENDPOINT_KEY = decode(
     "dzJ0UEZiamxQMTNHVW1iOGRNalVMNUIyWXlQVkQzcEo3RXk2Zno4dg=="
 )
 
-# FOOD_LEVEL_PERCENT_MAP = {9: 100, 8: 70, 7: 60, 6: 50, 5: 40, 4: 30, 3: 20, 2: 10, 1: 5, 0: 0}
+FOOD_LEVEL_MAP = {9: 100, 8: 70, 7: 60, 6: 50, 5: 40, 4: 30, 3: 20, 2: 10, 1: 5, 0: 0}
 MEAL_INSERT_SIZE_CUPS_MAP = {0: 1 / 4, 1: 1 / 8}
 MEAL_INSERT_SIZE_CUPS_REVERSE_MAP = {v: k for k, v in MEAL_INSERT_SIZE_CUPS_MAP.items()}
 
 
 class FeederRobot(Robot):  # pylint: disable=abstract-method
     """Data and methods for interacting with a Feeder-Robot automatic pet feeder."""
 
@@ -57,15 +57,15 @@
     def firmware(self) -> str:
         """Return the firmware version."""
         return str(self._state_info("fwVersion"))
 
     @property
     def food_level(self) -> int:
         """Return the food level."""
-        return int(round(self._state_info("level") / 9 * 100, -1))
+        return FOOD_LEVEL_MAP.get(self._state_info("level"), 0)
 
     @property
     def is_online(self) -> bool:
         """Return `True` if the robot is online."""
         return bool(self._state_info("online"))
 
     @property
```

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/litterrobot.py` & `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/litterrobot3.py` & `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot3.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/litterrobot4.py` & `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot4.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 try:
     from zoneinfo import ZoneInfo
 except ImportError:  # pragma: no cover
     from backports.zoneinfo import ZoneInfo  # type: ignore
 
 from ..activity import Activity, Insight
 from ..enums import LitterBoxStatus, LitterRobot4Command
-from ..exceptions import InvalidCommandException
+from ..exceptions import InvalidCommandException, LitterRobotException
 from ..utils import encode, to_timestamp, utcnow
 from .litterrobot import LitterRobot
 from .models import LITTER_ROBOT_4_MODEL
 
 if TYPE_CHECKING:
     from ..account import Account
 
@@ -28,15 +28,15 @@
 LR4_ENDPOINT = "https://lr4.iothings.site/graphql"
 LR4_STATUS_MAP = {
     "ROBOT_BONNET": LitterBoxStatus.BONNET_REMOVED,
     "ROBOT_CAT_DETECT": LitterBoxStatus.CAT_DETECTED,
     "ROBOT_CAT_DETECT_DELAY": LitterBoxStatus.CAT_SENSOR_TIMING,
     "ROBOT_CLEAN": LitterBoxStatus.CLEAN_CYCLE,
     "ROBOT_EMPTY": LitterBoxStatus.EMPTY_CYCLE,
-    "ROBOT_FIND_DUMP": LitterBoxStatus.DUMP_POSITION_FAULT,
+    "ROBOT_FIND_DUMP": LitterBoxStatus.CLEAN_CYCLE,
     "ROBOT_IDLE": LitterBoxStatus.READY,
     "ROBOT_POWER_DOWN": LitterBoxStatus.POWER_DOWN,
     "ROBOT_POWER_OFF": LitterBoxStatus.OFF,
     "ROBOT_POWER_UP": LitterBoxStatus.POWER_UP,
 }
 ACTIVITY_STATUS_MAP: dict[str, LitterBoxStatus | str] = {
     "bonnetRemovedYes": LitterBoxStatus.BONNET_REMOVED,
@@ -76,15 +76,15 @@
 
 
 class LitterRobot4(LitterRobot):  # pylint: disable=abstract-method
     """Data and methods for interacting with a Litter-Robot 4 automatic, self-cleaning litter box."""
 
     _attr_model = "Litter-Robot 4"
 
-    VALID_WAIT_TIMES = [3, 5, 7, 15, 30]
+    VALID_WAIT_TIMES = [3, 7, 15, 25, 30]
 
     _data_cycle_capacity = "DFINumberOfCycles"
     _data_cycle_count = "odometerCleanCycles"
     _data_drawer_full_cycles = "DFIFullCounter"
     _data_id = "unitId"
     _data_name = "name"
     _data_power_status = "unitPowerType"
@@ -504,14 +504,16 @@
                         "%Y-%m-%dT%H:%M:%S.%fZ"
                     ),
                     "timezoneOffset": timezone_offset,
                 },
             }
         )
         insight = cast(dict, data).get("data", {}).get("getLitterRobot4Insights", {})
+        if insight is None:
+            raise LitterRobotException("Insight data could not be retrieved.")
         return Insight(
             insight["totalCycles"],
             insight["averageCycles"],
             [
                 (
                     datetime.strptime(cycle["date"], "%Y-%m-%d").date(),
                     cycle["numberOfCycles"],
```

### Comparing `pylitterbot-2023.1.2/pylitterbot/robot/models.py` & `pylitterbot-2023.4.0/pylitterbot/robot/models.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/session.py` & `pylitterbot-2023.4.0/pylitterbot/session.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/utils.py` & `pylitterbot-2023.4.0/pylitterbot/utils.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pylitterbot/ws_monitor.py` & `pylitterbot-2023.4.0/pylitterbot/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.1.2/pyproject.toml` & `pylitterbot-2023.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylitterbot"
-version = "2023.1.2"
+version = "2023.4.0"
 description = "Python package for controlling Whisker automatic robots."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/pylitterbot"
 repository = "https://github.com/natekspencer/pylitterbot"
 keywords = ["Whisker", "Litter-Robot", "Feeder-Robot", "litter box", "pet feeder", "asynchronous"]
@@ -14,24 +14,24 @@
 python = "^3.7.2"
 aiohttp = "^3.8.1"
 deepdiff = "^6.2.1"
 PyJWT = "^2.4.0"
 "backports.zoneinfo" = {version = "^0.2.1", python = "<3.9"}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 pytest-freezegun = "^0.4.2"
 aioresponses = "^0.7.4"
-black = "^22.12.0"
-isort = "^5.11.4"
-mypy = "^0.991"
+black = "^23.3.0"
+isort = "^5.11.5"
+mypy = "^1.1"
 flake8 = "^5.0.4"
-pylint = "^2.15.10"
+pylint = "^2.17.2"
 tox = "^3.28.0"
-pydocstyle = "^6.2.3"
+pydocstyle = "^6.3.0"
 pytest-timeout = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylitterbot-2023.1.2/setup.py` & `pylitterbot-2023.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['PyJWT>=2.4.0,<3.0.0', 'aiohttp>=3.8.1,<4.0.0', 'deepdiff>=6.2.1,<7.0.0']
 
 extras_require = \
 {':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
 
 setup_kwargs = {
     'name': 'pylitterbot',
-    'version': '2023.1.2',
+    'version': '2023.4.0',
     'description': 'Python package for controlling Whisker automatic robots.',
-    'long_description': '[![pypi](https://img.shields.io/pypi/v/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![downloads](https://img.shields.io/pypi/dm/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)\n[![Purchase Litter-Robot](https://img.shields.io/badge/Buy_a_Litter--Robot-Save_$25-lightgrey?style=for-the-badge&labelColor=grey)](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ)\n\n# pylitterbot\n\nPython package for controlling Whisker connected self-cleaning litter boxes and feeders.\n\nThis is an unofficial API for controlling various Whisker automated robots. It currently supports Litter-Robot 3 (with connect), Litter-Robot 4 and Feeder-Robot.\n\n## Disclaimer\n\nThis API is experimental and was reverse-engineered by monitoring network traffic and decompiling source code from the Whisker app since no public API is currently available at this time. It may cease to work at any time. Use at your own risk.\n\n## Installation\n\nInstall using pip\n\n```bash\npip install pylitterbot\n```\n\nAlternatively, clone the repository and run\n\n```bash\npython setup.py install\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom pylitterbot import Account\n\n# Set email and password for initial authentication.\nusername = "Your username"\npassword = "Your password"\n\n\nasync def main():\n    # Create an account.\n    account = Account()\n\n    try:\n        # Connect to the API and load robots.\n        await account.connect(username=username, password=password, load_robots=True)\n\n        # Print robots associated with account.\n        print("Robots:")\n        for robot in account.robots:\n            print(robot)\n    finally:\n        # Disconnect from the API.\n        await account.disconnect()\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nwhich will output something like:\n\n```\nName: Litter-Robot Name, Serial: LR3C012345, id: a0123b4567cd8e\n```\n\nTo start a clean cycle\n\n```python\nawait robot.start_cleaning()\n```\n\nIf no exception occurred, your Litter-Robot should now perform a clean cycle.\n\nCurrently the following methods are available in the Robot class:\n\n- refresh()\n- start_cleaning()\n- reset_settings()\n- set_panel_lockout()\n- set_night_light()\n- set_power_status()\n- set_sleep_mode()\n- set_wait_time()\n- set_name()\n- get_activity_history()\n- get_insight()\n\n---\n\n## TODO\n\n- Improve support for Litter-Robot 4\n- Improve support for Feeder-Robot\n\n---\n\n## Support Me\n\nI\'m not employed by Whisker and provide this python package as-is.\n\nIf you don\'t already own a Litter-Robot, please consider using [my affiliate link](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ) to purchase your own robot and save $25!\n\nIf you already own a Litter-Robot and/or want to donate to me directly, consider buying me a coffee (or beer) instead by using the link below:\n\n<a href=\'https://ko-fi.com/natekspencer\' target=\'_blank\'><img height=\'35\' style=\'border:0px;height:46px;\' src=\'https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0\' border=\'0\' alt=\'Buy Me a Coffee at ko-fi.com\' />\n',
+    'long_description': '[![pypi](https://img.shields.io/pypi/v/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![downloads](https://img.shields.io/pypi/dm/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)\n[![Purchase Litter-Robot](https://img.shields.io/badge/Buy_a_Litter--Robot-Save_$25-lightgrey?style=for-the-badge&labelColor=grey)](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ)\n\n# pylitterbot\n\nPython package for controlling Whisker connected self-cleaning litter boxes and feeders.\n\nThis is an unofficial API for controlling various Whisker automated robots. It currently supports Litter-Robot 3 (with connect), Litter-Robot 4 and Feeder-Robot.\n\n## Disclaimer\n\nThis API is experimental and was reverse-engineered by monitoring network traffic and decompiling source code from the Whisker app since no public API is currently available at this time. It may cease to work at any time. Use at your own risk.\n\n## Installation\n\nInstall using pip\n\n```bash\npip install pylitterbot\n```\n\nAlternatively, clone the repository and run\n\n```bash\npoetry install\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom pylitterbot import Account\n\n# Set email and password for initial authentication.\nusername = "Your username"\npassword = "Your password"\n\n\nasync def main():\n    # Create an account.\n    account = Account()\n\n    try:\n        # Connect to the API and load robots.\n        await account.connect(username=username, password=password, load_robots=True)\n\n        # Print robots associated with account.\n        print("Robots:")\n        for robot in account.robots:\n            print(robot)\n    finally:\n        # Disconnect from the API.\n        await account.disconnect()\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nwhich will output something like:\n\n```\nName: Litter-Robot Name, Serial: LR3C012345, id: a0123b4567cd8e\n```\n\nTo start a clean cycle\n\n```python\nawait robot.start_cleaning()\n```\n\nIf no exception occurred, your Litter-Robot should now perform a clean cycle.\n\nCurrently the following methods are available in the Robot class:\n\n- refresh()\n- start_cleaning()\n- reset_settings()\n- set_panel_lockout()\n- set_night_light()\n- set_power_status()\n- set_sleep_mode()\n- set_wait_time()\n- set_name()\n- get_activity_history()\n- get_insight()\n\n---\n\n## TODO\n\n- Improve support for Litter-Robot 4\n- Improve support for Feeder-Robot\n\n---\n\n## Support Me\n\nI\'m not employed by Whisker and provide this python package as-is.\n\nIf you don\'t already own a Litter-Robot, please consider using [my affiliate link](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ) to purchase your own robot and save $25!\n\nIf you already own a Litter-Robot and/or want to donate to me directly, consider buying me a coffee (or beer) instead by using the link below:\n\n<a href=\'https://ko-fi.com/natekspencer\' target=\'_blank\'><img height=\'35\' style=\'border:0px;height:46px;\' src=\'https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0\' border=\'0\' alt=\'Buy Me a Coffee at ko-fi.com\' />\n',
     'author': 'Nathan Spencer',
     'author_email': 'natekspencer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/natekspencer/pylitterbot',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pylitterbot-2023.1.2/PKG-INFO` & `pylitterbot-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylitterbot
-Version: 2023.1.2
+Version: 2023.4.0
 Summary: Python package for controlling Whisker automatic robots.
 Home-page: https://github.com/natekspencer/pylitterbot
 License: MIT
 Keywords: Whisker,Litter-Robot,Feeder-Robot,litter box,pet feeder,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -43,15 +43,15 @@
 ```bash
 pip install pylitterbot
 ```
 
 Alternatively, clone the repository and run
 
 ```bash
-python setup.py install
+poetry install
 ```
 
 ## Usage
 
 ```python
 import asyncio
```

