# Comparing `tmp/neopolitan-0.1.5.tar.gz` & `tmp/neopolitan-0.1.6.tar.gz`

## Comparing `neopolitan-0.1.5.tar` & `neopolitan-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.5/.pylintrc
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.5/Notes.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.5/pytest.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.5/requirements.txt
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.5/.vscode/settings.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/ReadMe.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/const.py
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/neop.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/os_detection.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/testboardrunner.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/board_functions/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/board_functions/board.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/board_functions/board_data.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/board_functions/colors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/abstract_board_display.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/abstract_display.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/graphical_board_display.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/graphical_display.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/hardware_board_display.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/display/hardware_display.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/writing/ReadMe.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/writing/__init__.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/writing/data_transformation.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/writing/groups_8.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.5/neopolitan/writing/letters_8.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/ReadMe.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/board_test.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/data_transformation_test.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/flip_test.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/groups_test.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.5/tests/process_board_data_test.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.5/visual_tests/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.5/visual_tests/demo_test.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.5/visual_tests/main_test.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 neopolitan-0.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.5/LICENSE
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.5/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.pylintrc
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 neopolitan-0.1.6/Notes.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/pytest.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 neopolitan-0.1.6/requirements.txt
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.vscode/settings.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/HowOperationsWork.md
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/ReadMe.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/const.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/neop.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/os_detection.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/testboardrunner.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/board.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/board_data.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/board_functions/colors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/abstract_board_display.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/abstract_display.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/graphical_board_display.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/graphical_display.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/hardware_board_display.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/display/hardware_display.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/ReadMe.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/data_transformation.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/groups_8.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 neopolitan-0.1.6/neopolitan/writing/letters_8.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/ReadMe.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/board_test.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/data_transformation_test.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/flip_test.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/groups_test.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 neopolitan-0.1.6/tests/process_board_data_test.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/demo_test.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 neopolitan-0.1.6/visual_tests/main_test.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 neopolitan-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 neopolitan-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopolitan-0.1.6/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 neopolitan-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 neopolitan-0.1.6/PKG-INFO
```

### Comparing `neopolitan-0.1.5/.github/workflows/python-package.yml` & `neopolitan-0.1.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/ReadMe.md` & `neopolitan-0.1.6/neopolitan/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/neop.py` & `neopolitan-0.1.6/neopolitan/neop.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,22 @@
 from neopolitan.writing.data_transformation import str_to_data
 from neopolitan.os_detection import on_pi
 # pylint: disable=wildcard-import
 from neopolitan.const import *
 
 def initialize_logger(prep='logs/'):
     """Set up the log file"""
-    filename = prep + str(datetime.datetime.now()) + '.txt'
+    # todo: prep arg validation
+    import os
+    log_time = str(datetime.datetime.now()) \
+        .replace(" ", "_") \
+        .replace(".", "_") \
+        .replace(":", "-")
+    filename = f'{os.getcwd()}/{prep}neopolitan_{log_time}.txt'
+    print('log location:', filename)
     logging.basicConfig(filename=filename, encoding='utf=8', level=logging.DEBUG)
 
 def main(events=None):
     """Make a very simple display"""
 
     initialize_logger()
 
@@ -146,15 +153,20 @@
     return board_data
 
 def process_board_data_events(board_data, event_list):
     """Manipulate board data according to events"""
 
     first = event_list[0]
     if first == 'speed':
-        speed = event_list[1]
+        try:
+            speed = event_list[1]
+        # pylint: disable=broad-except
+        except Exception as err:
+            # todo: better explanation
+            logging.warning('No second value provided, %s', err)
         if speed == 'slow':
             board_data.scroll_slow()
             logging.info('set speed: slow')
         elif speed == 'medium':
             board_data.scroll_medium()
             logging.info('set speed: medium')
         elif speed == 'fast':
@@ -163,12 +175,27 @@
         else:
             try:
                 speed = float(speed)
                 board_data.set_scroll_wait(speed)
                 logging.info(f'set speed: {speed}')
             except ValueError:
                 logging.warning(f'Cannot parse speed: {speed}')
+    elif first == 'wrap':
+        try:
+            wrap = event_list[1]
+        # pylint: disable=broad-except
+        except Exception as err:
+            # todo: better explanation
+            logging.warning('No second value provided, %s', err)
+        if wrap in ('True', '1'):
+            board_data.should_wrap = True
+            logging.info('set wrap: True')
+        elif wrap in ('False', '0'):
+            board_data.should_wrap = False
+            logging.info('set wrap: False')
+        else:
+            logging.warning('Cannot parse wrap: %s', wrap)
 
     return board_data
 
 if __name__ == '__main__':
     main()
```

### Comparing `neopolitan-0.1.5/neopolitan/testboardrunner.py` & `neopolitan-0.1.6/neopolitan/testboardrunner.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,12 +17,15 @@
     t = Thread(target=main, args=(events,))
     t.start()
 
     Thread(target=add_to_queue, args=(events, 'speed fast', 1,)).start()
     Thread(target=add_to_queue, args=(events, 'speed 1.0', 2,)).start()
     Thread(target=add_to_queue, args=(events, 'speed banana', 3,)).start()
     Thread(target=add_to_queue, args=(events, 'say hello again', 5,)).start()
-    Thread(target=add_to_queue, args=(events, 'exit', 10,)).start()
+    # todo: test below
+    Thread(target=add_to_queue, args=(events, 'wrap False', 10,)).start()
+    Thread(target=add_to_queue, args=(events, 'wrap 1', 15,)).start()
+    Thread(target=add_to_queue, args=(events, 'exit', 20,)).start()
 
     t.join() # no difference
 
 runner()
```

### Comparing `neopolitan-0.1.5/neopolitan/board_functions/board.py` & `neopolitan-0.1.6/neopolitan/board_functions/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             data = data[0:self.size]
         self.data = data
 
     def turn_on(self, idx, color=ON):
         """Set the color of a given idx (default=white)"""
         if idx >= len(self.data):
             # pylint: disable=consider-using-f-string
-            logging.warning('index {0} out of bounds: size = {1}'.format(idx, self.size))
+            logging.warning('index %s out of bounds: size = %s', idx, self.size)
             return
         self.data[idx] = color
 
     def turn_off(self, idx):
         """'Turn off' a given idx (set to None)"""
         # todo: what about with led board?
         self.data[idx] = OFF
```

### Comparing `neopolitan-0.1.5/neopolitan/board_functions/board_data.py` & `neopolitan-0.1.6/neopolitan/board_functions/board_data.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/display/graphical_board_display.py` & `neopolitan-0.1.6/neopolitan/display/graphical_board_display.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Draws a board"""
 
-import pygame
 import logging
+import pygame
 from neopolitan.display.abstract_board_display import BoardDisplay
 from neopolitan.const import WIDTH, HEIGHT
 # from board import Board
 
 class GraphicalBoardDisplay(BoardDisplay):
     """Draws board data"""
     width = 0
@@ -23,15 +23,15 @@
     # pylint: disable=arguments-differ
     def draw_board(self, screen, space, size):
         """Draw all the 'lights' in the board"""
         assert self.board, 'No board assigned'
 
         for i in range(self.width * self.height):
             if i >= len(self.board.data):
-                logging.warning(f'index {i} outside of data array bounds')
+                logging.warning('index %i outside of data array bounds', i)
                 return
             color = self.board.data[i]
             row = self.get_row(i)
             col = self.get_col(i)
 
             if not self.board.data[i]:
                 continue
```

### Comparing `neopolitan-0.1.5/neopolitan/display/graphical_display.py` & `neopolitan-0.1.6/neopolitan/display/graphical_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/display/hardware_board_display.py` & `neopolitan-0.1.6/neopolitan/display/hardware_board_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         """Sets all the LEDs in accordance with the current data"""
         assert self.board, 'No board assigned'
 
         flipped_data = HardwareBoardDisplay.flip(self.board.data, HEIGHT)
 
         for i in range(self.size):
             if i >= len(self.board.data):
-                logging.warning(f'index {i} outside of data array bounds')
+                logging.warning('index %s outside of data array bounds', i)
                 return
             self.pixels[i] = flipped_data[i]
 
     # pylint: disable=no-self-argument
     def flip(data, height=HEIGHT, start_at_first=False):
         """
         Handles flipping alternate 'rows' so that data appears as expected;
```

### Comparing `neopolitan-0.1.5/neopolitan/display/hardware_display.py` & `neopolitan-0.1.6/neopolitan/display/hardware_display.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/writing/ReadMe.md` & `neopolitan-0.1.6/neopolitan/writing/ReadMe.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/writing/data_transformation.py` & `neopolitan-0.1.6/neopolitan/writing/data_transformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         return lowercase[ascii_val-97]
     if 65 <= ascii_val < 91:
         return uppercase[ascii_val-65]
     if 48 <= ascii_val < 58:
         return numbers[ascii_val-48]
     if char in symbols:
         return symbols[char]
-    logging.warning(f'Cannot find char: {char}')
+    logging.warning('Cannot find char: %s', char)
     return []
 
 def frame_length(sym):
     """Returns the highest multiple of 8 above the largest index in the symbol array.
     This makes it so the frame has the correct length, since it should 'fill' all columns it uses"""
     if sym == 'space':
         return 8*2
```

### Comparing `neopolitan-0.1.5/neopolitan/writing/groups_8.py` & `neopolitan-0.1.6/neopolitan/writing/groups_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/neopolitan/writing/letters_8.py` & `neopolitan-0.1.6/neopolitan/writing/letters_8.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/tests/board_test.py` & `neopolitan-0.1.6/tests/board_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/tests/data_transformation_test.py` & `neopolitan-0.1.6/tests/data_transformation_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/tests/flip_test.py` & `neopolitan-0.1.6/tests/flip_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/tests/groups_test.py` & `neopolitan-0.1.6/tests/groups_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/tests/process_board_data_test.py` & `neopolitan-0.1.6/tests/process_board_data_test.py`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/.gitignore` & `neopolitan-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/LICENSE` & `neopolitan-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/README.md` & `neopolitan-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `neopolitan-0.1.5/pyproject.toml` & `neopolitan-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "neopolitan"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name = "alyo" },
 ]
 description = "Neopolitan: a library for displaying text on LED boards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neopolitan-0.1.5/PKG-INFO` & `neopolitan-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neopolitan
-Version: 0.1.5
+Version: 0.1.6
 Summary: Neopolitan: a library for displaying text on LED boards
 Project-URL: Homepage, https://github.com/alyoshenka/neopolitan
 Author: alyo
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

