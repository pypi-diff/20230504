# Comparing `tmp/neopolitan-0.1.6.tar.gz` & `tmp/neopolitan-0.1.7.tar.gz`

## Comparing `neopolitan-0.1.6.tar` & `neopolitan-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.pylintrc
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.6/Notes.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/pytest.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.6/requirements.txt
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.vscode/settings.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/HowOperationsWork.md
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/ReadMe.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/const.py
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/neop.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/os_detection.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/testboardrunner.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/board.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/board_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/colors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/abstract_board_display.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/abstract_display.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/graphical_board_display.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/graphical_display.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/hardware_board_display.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/hardware_display.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/ReadMe.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/data_transformation.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/groups_8.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/letters_8.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/ReadMe.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/board_test.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/data_transformation_test.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/flip_test.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/groups_test.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/process_board_data_test.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/demo_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/main_test.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.6/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.6/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.7/.pylintrc
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.7/Notes.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.7/pytest.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.7/requirements.txt
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.7/.vscode/settings.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/HowOperationsWork.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/ReadMe.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/const.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/neop.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/os_detection.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/testboardrunner.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/board_functions/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/board_functions/board.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/board_functions/board_data.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/board_functions/colors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/abstract_board_display.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/abstract_display.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/graphical_board_display.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/graphical_display.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/hardware_board_display.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/display/hardware_display.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/writing/ReadMe.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/writing/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/writing/data_transformation.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/writing/groups_8.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.7/neopolitan/writing/letters_8.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/ReadMe.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/board_test.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/data_transformation_test.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/flip_test.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/groups_test.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.7/tests/process_board_data_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.7/visual_tests/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.7/visual_tests/demo_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.7/visual_tests/main_test.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 neopolitan-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.7/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.7/PKG-INFO
```

### Comparing `neopolitan-0.1.6/.github/workflows/python-package.yml` & `neopolitan-0.1.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/HowOperationsWork.md` & `neopolitan-0.1.7/neopolitan/HowOperationsWork.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/ReadMe.md` & `neopolitan-0.1.7/neopolitan/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/neop.py` & `neopolitan-0.1.7/neopolitan/neop.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 # pylint: disable=wildcard-import
 from neopolitan.const import *
 
 def initialize_logger(prep='logs/'):
     """Set up the log file"""
     # todo: prep arg validation
     import os
+    # make directory if it does not exist
+    # todo: is this ok?
+    if not os.path.exists(prep):
+        print('making', prep, 'directory')
+        os.makedirs(prep)
     log_time = str(datetime.datetime.now()) \
         .replace(" ", "_") \
         .replace(".", "_") \
         .replace(":", "-")
     filename = f'{os.getcwd()}/{prep}neopolitan_{log_time}.txt'
     print('log location:', filename)
     logging.basicConfig(filename=filename, encoding='utf=8', level=logging.DEBUG)
```

### Comparing `neopolitan-0.1.6/neopolitan/testboardrunner.py` & `neopolitan-0.1.7/neopolitan/testboardrunner.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/board_functions/board.py` & `neopolitan-0.1.7/neopolitan/board_functions/board.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/board_functions/board_data.py` & `neopolitan-0.1.7/neopolitan/board_functions/board_data.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/display/graphical_board_display.py` & `neopolitan-0.1.7/neopolitan/display/graphical_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/display/graphical_display.py` & `neopolitan-0.1.7/neopolitan/display/graphical_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/display/hardware_board_display.py` & `neopolitan-0.1.7/neopolitan/display/hardware_board_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/display/hardware_display.py` & `neopolitan-0.1.7/neopolitan/display/hardware_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/writing/ReadMe.md` & `neopolitan-0.1.7/neopolitan/writing/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/writing/data_transformation.py` & `neopolitan-0.1.7/neopolitan/writing/data_transformation.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/writing/groups_8.py` & `neopolitan-0.1.7/neopolitan/writing/groups_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/neopolitan/writing/letters_8.py` & `neopolitan-0.1.7/neopolitan/writing/letters_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/tests/board_test.py` & `neopolitan-0.1.7/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/tests/data_transformation_test.py` & `neopolitan-0.1.7/tests/data_transformation_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/tests/flip_test.py` & `neopolitan-0.1.7/tests/flip_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/tests/groups_test.py` & `neopolitan-0.1.7/tests/groups_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/tests/process_board_data_test.py` & `neopolitan-0.1.7/tests/process_board_data_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/.gitignore` & `neopolitan-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/LICENSE` & `neopolitan-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/README.md` & `neopolitan-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.6/pyproject.toml` & `neopolitan-0.1.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "neopolitan"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name = "alyo" },
 ]
 description = "Neopolitan: a library for displaying text on LED boards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neopolitan-0.1.6/PKG-INFO` & `neopolitan-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopolitan
-Version: 0.1.6
+Version: 0.1.7
 Summary: Neopolitan: a library for displaying text on LED boards
 Project-URL: Homepage, https://github.com/alyoshenka/neopolitan
 Author: alyo
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

