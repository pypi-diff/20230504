# Comparing `tmp/timerdo-0.0.4.tar.gz` & `tmp/timerdo-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timerdo-0.0.4.tar", last modified: Thu May  4 19:59:54 2023, max compression
+gzip compressed data, was "timerdo-0.0.5b0.tar", last modified: Thu May  4 20:20:13 2023, max compression
```

## Comparing `timerdo-0.0.4.tar` & `timerdo-0.0.5b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       30 2023-05-04 19:59:13.280237 timerdo-0.0.4/.coveragerc
--rw-r--r--   0        0        0       99 2023-05-04 19:59:13.280237 timerdo-0.0.4/.flake8
--rw-r--r--   0        0        0      569 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      506 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0      566 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/test_suite.yml
--rw-r--r--   0        0        0      101 2023-05-04 19:59:13.280237 timerdo-0.0.4/.gitignore
--rw-r--r--   0        0        0      292 2023-05-04 19:59:13.284237 timerdo-0.0.4/Makefile
--rw-r--r--   0        0        0     1793 2023-05-04 19:59:13.284237 timerdo-0.0.4/README.md
--rw-r--r--   0        0        0     1211 2023-05-04 19:59:13.284237 timerdo-0.0.4/UNLICENSE
--rw-r--r--   0        0        0     3400 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/cli_reference.md
--rw-r--r--   0        0        0    37426 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/favicon.png
--rw-r--r--   0        0        0    76201 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/logo.png
--rw-r--r--   0        0        0    75292 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/screenshot_timerdo_report.png
--rw-r--r--   0        0        0    13786 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/timerdo_no_args.png
--rw-r--r--   0        0        0     1891 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/index.md
--rw-r--r--   0        0        0     2502 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/install.md
--rw-r--r--   0        0        0     4267 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/start.md
--rw-r--r--   0        0        0       48 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0    19982 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/tutorial_1.md
--rw-r--r--   0        0        0      376 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/tutorial_2.md
--rw-r--r--   0        0        0      138 2023-05-04 19:59:13.284237 timerdo-0.0.4/includes/abbreviations.md
--rw-r--r--   0        0        0     2240 2023-05-04 19:59:13.284237 timerdo-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0     1242 2023-05-04 19:59:13.284237 timerdo-0.0.4/pyproject.toml
--rwxr-xr-x   0        0        0      210 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/bootstrap.sh
--rw-r--r--   0        0        0      157 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/build_cli_ref.sh
--rw-r--r--   0        0        0      816 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_db.py
--rwxr-xr-x   0        0        0      241 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_preview.sh
--rwxr-xr-x   0        0        0      101 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_publish.sh
--rwxr-xr-x   0        0        0      354 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/format.sh
--rw-r--r--   0        0        0      207 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/gen_docs_db.sh
--rwxr-xr-x   0        0        0      110 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/publish.sh
--rwxr-xr-x   0        0        0      277 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/tests.sh
--rw-r--r--   0        0        0        0 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/conftest.py
--rw-r--r--   0        0        0     6658 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/test_core.py
--rw-r--r--   0        0        0     2559 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/test_main.py
--rw-r--r--   0        0        0      100 2023-05-04 19:59:13.284237 timerdo-0.0.4/timerdo/__init__.py
--rw-r--r--   0        0        0      955 2023-05-04 19:59:13.284237 timerdo-0.0.4/timerdo/config.py
--rw-r--r--   0        0        0    11739 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/core.py
--rw-r--r--   0        0        0     1075 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/database.py
--rw-r--r--   0        0        0      630 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/exceptions.py
--rw-r--r--   0        0        0     5417 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/main.py
--rw-r--r--   0        0        0     1681 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/models.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 timerdo-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.coveragerc
+-rw-r--r--   0        0        0       99 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.flake8
+-rw-r--r--   0        0        0      569 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      506 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0      566 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.github/workflows/test_suite.yml
+-rw-r--r--   0        0        0      101 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/.gitignore
+-rw-r--r--   0        0        0      292 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/Makefile
+-rw-r--r--   0        0        0     1793 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/README.md
+-rw-r--r--   0        0        0     1211 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/UNLICENSE
+-rw-r--r--   0        0        0     3400 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/cli_reference.md
+-rw-r--r--   0        0        0    37426 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/favicon.png
+-rw-r--r--   0        0        0    76201 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/logo.png
+-rw-r--r--   0        0        0    75292 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/screenshot_timerdo_report.png
+-rw-r--r--   0        0        0    13786 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/img/timerdo_no_args.png
+-rw-r--r--   0        0        0     1891 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/index.md
+-rw-r--r--   0        0        0     2502 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/install.md
+-rw-r--r--   0        0        0     4267 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/start.md
+-rw-r--r--   0        0        0       48 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0    19982 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/tutorial_1.md
+-rw-r--r--   0        0        0      376 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/docs/tutorial_2.md
+-rw-r--r--   0        0        0      138 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/includes/abbreviations.md
+-rw-r--r--   0        0        0     2240 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/mkdocs.yml
+-rw-r--r--   0        0        0     1242 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/pyproject.toml
+-rwxr-xr-x   0        0        0      210 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/scripts/bootstrap.sh
+-rw-r--r--   0        0        0      157 2023-05-04 20:19:32.358816 timerdo-0.0.5b0/scripts/build_cli_ref.sh
+-rw-r--r--   0        0        0      816 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_db.py
+-rwxr-xr-x   0        0        0      241 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_preview.sh
+-rwxr-xr-x   0        0        0      101 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/docs_publish.sh
+-rwxr-xr-x   0        0        0      354 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/format.sh
+-rw-r--r--   0        0        0      207 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/gen_docs_db.sh
+-rwxr-xr-x   0        0        0      110 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      277 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/scripts/tests.sh
+-rw-r--r--   0        0        0        0 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/conftest.py
+-rw-r--r--   0        0        0     6422 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/test_core.py
+-rw-r--r--   0        0        0     2557 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/test/test_main.py
+-rw-r--r--   0        0        0      101 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/__init__.py
+-rw-r--r--   0        0        0      955 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/config.py
+-rw-r--r--   0        0        0    11736 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/core.py
+-rw-r--r--   0        0        0     1075 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/database.py
+-rw-r--r--   0        0        0      630 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/exceptions.py
+-rw-r--r--   0        0        0     5417 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/main.py
+-rw-r--r--   0        0        0     1681 2023-05-04 20:19:32.362816 timerdo-0.0.5b0/timerdo/models.py
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 timerdo-0.0.5b0/PKG-INFO
```

### Comparing `timerdo-0.0.4/.github/workflows/publish_docs.yml` & `timerdo-0.0.5b0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/.github/workflows/test_suite.yml` & `timerdo-0.0.5b0/.github/workflows/test_suite.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/README.md` & `timerdo-0.0.5b0/README.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/UNLICENSE` & `timerdo-0.0.5b0/UNLICENSE`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/cli_reference.md` & `timerdo-0.0.5b0/docs/cli_reference.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/img/favicon.png` & `timerdo-0.0.5b0/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/img/logo.png` & `timerdo-0.0.5b0/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/img/screenshot_timerdo_report.png` & `timerdo-0.0.5b0/docs/img/screenshot_timerdo_report.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/img/timerdo_no_args.png` & `timerdo-0.0.5b0/docs/img/timerdo_no_args.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/index.md` & `timerdo-0.0.5b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/install.md` & `timerdo-0.0.5b0/docs/install.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/start.md` & `timerdo-0.0.5b0/docs/start.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/docs/tutorial_1.md` & `timerdo-0.0.5b0/docs/tutorial_1.md`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/mkdocs.yml` & `timerdo-0.0.5b0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/pyproject.toml` & `timerdo-0.0.5b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/scripts/docs_db.py` & `timerdo-0.0.5b0/scripts/docs_db.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/test/conftest.py` & `timerdo-0.0.5b0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/test/test_core.py` & `timerdo-0.0.5b0/test/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,14 @@
     add_timer,
     delete_item,
     edit_timer_item,
     edit_todo_item,
     finish_timer,
     query_with_text,
 )
-from timerdo.exceptions import (
-    DoneTaskError,
-    IdNotFoundError,
-    NegativeIntervalError,
-    NoChangingError,
-    NoTimeRunningError,
-    OutOffPeriodError,
-    RunningTimerError,
-)
 from timerdo.models import Status, Timer, ToDoItem
 
 
 def test_connection_add(tconnection, fake_todo_item):
     tconnection.add(fake_todo_item)
     assert tconnection.get_id(ToDoItem, 1).status == Status.to_do
 
@@ -221,11 +212,10 @@
 def test_edit_timer_wrong_id(tconnection):
     with pytest.raises(SystemExit) as e:
         edit_timer_item(2, finished_at=datetime.now(), session=tconnection)
         assert e.value.code == 1
 
 
 def test_select_all(tconnection, running_timer):
-    item = tconnection.get_id(ToDoItem, 1)
     script = """SELECT * FROM todo_list"""
     result = query_with_text(script, session=tconnection)
     assert '{' in result
```

### Comparing `timerdo-0.0.4/test/test_main.py` & `timerdo-0.0.5b0/test/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
     assert f'from 1789-07-14 until {datetime.now().date()}' in result.stdout
 
 
 def test_report_date():
     result = runner.invoke(
         app, ['report', '--init', '1988-10-10', '--end', '2022-10-10']
     )
-    assert f'from 1988-10-10 until 2022-10-10' in result.stdout
+    assert 'from 1988-10-10 until 2022-10-10' in result.stdout
 
 
 def test_report_date_init():
     result = runner.invoke(app, ['report', '--init', '1988-10-10'])
     assert f'from 1988-10-10 until {datetime.now().date()}' in result.stdout
 
 
 def test_report_date_end():
     result = runner.invoke(app, ['report', '--end', '1988-10-10'])
-    assert f'from 1789-07-14 until 1988-10-10' in result.stdout
+    assert 'from 1789-07-14 until 1988-10-10' in result.stdout
 
 
 def test_report_date_error():
     result = runner.invoke(
         app, ['report', '--end', '1400-10-10', '--init', '1988-10-10']
     )
     assert result.exit_code == 1
```

### Comparing `timerdo-0.0.4/timerdo/config.py` & `timerdo-0.0.5b0/timerdo/config.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/timerdo/core.py` & `timerdo-0.0.5b0/timerdo/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import json
+import sys
 from datetime import date, datetime
 from itertools import chain
 from string import capwords
 from typing import NoReturn
 
 import numpy as np
 import pandas as pd
@@ -29,15 +29,15 @@
 connection = Connection(engine)
 
 
 def exception_handler(func):
     """Handle exceptions with a prittyprint."""
 
     def wrapper(*args, **kwargs):
-        """Wrapper decorated function."""
+        """Wrap decorated function."""
         try:
             result = func(*args, **kwargs)
         except Exception as ex:
             print(f"[bold red]:boom-emoji: {ex}[/bold red]")
             sys.exit(1)
         return result
```

### Comparing `timerdo-0.0.4/timerdo/database.py` & `timerdo-0.0.5b0/timerdo/database.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/timerdo/exceptions.py` & `timerdo-0.0.5b0/timerdo/exceptions.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/timerdo/main.py` & `timerdo-0.0.5b0/timerdo/main.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/timerdo/models.py` & `timerdo-0.0.5b0/timerdo/models.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.4/PKG-INFO` & `timerdo-0.0.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timerdo
-Version: 0.0.4
+Version: 0.0.5b0
 Summary: Minimalist to-do list with built-in timer to keep your tasks on track.
 Author-email: Caio Mescouto Terra de Souza <caiomescouto@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.4, <2.1
 Requires-Dist: typer >=0.7.0, <0.9
 Requires-Dist: rich >=13.3, <13.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timerdo Version: 0.0.4 Summary: Minimalist to-do
+Metadata-Version: 2.1 Name: timerdo Version: 0.0.5b0 Summary: Minimalist to-do
 list with built-in timer to keep your tasks on track. Author-email: Caio
 Mescouto Terra de Souza
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.4, <2.1 Requires-Dist: typer >=0.7.0, <0.9
 Requires-Dist: rich >=13.3, <13.4 Requires-Dist: pandas[performance,feather]
 >=2.0.1, <2.1 Requires-Dist: black >=23.1, <23.2 ; extra == "dev" Requires-
 Dist: flake8 >=6.0, <6.1 ; extra == "dev" Requires-Dist: isort >=5.12, <5.13 ;
```

