# Comparing `tmp/textfiles-0.0.5.tar.gz` & `tmp/textfiles-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfiles-0.0.5.tar", last modified: Thu May  4 15:29:38 2023, max compression
+gzip compressed data, was "textfiles-0.0.6.tar", last modified: Thu May  4 16:42:09 2023, max compression
```

## Comparing `textfiles-0.0.5.tar` & `textfiles-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/
--rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.5/LICENSE
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:29:38.737907 textfiles-0.0.5/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 15:29:30.000000 textfiles-0.0.5/README.md
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 15:29:38.737907 textfiles-0.0.5/setup.cfg
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 15:29:30.000000 textfiles-0.0.5/setup.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/tests/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.5/tests/test_for_csv.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.5/tests/tests_for_txt.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/textfiles/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:17:13.000000 textfiles-0.0.5/textfiles/__init__.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     9423 2023-05-04 15:28:40.000000 textfiles-0.0.5/textfiles/csv_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1395 2023-05-04 15:27:17.000000 textfiles-0.0.5/textfiles/exceptions.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2580 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/file_factory.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     8496 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/json_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2427 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/text_file_parent.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     3735 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/txt_file.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/textfiles.egg-info/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/SOURCES.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/dependency_links.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.241960 textfiles-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-12 08:45:31.000000 textfiles-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3004 2023-05-04 16:42:09.240960 textfiles-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-05-04 16:32:01.000000 textfiles-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:42:09.242960 textfiles-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-04 16:32:01.000000 textfiles-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.224950 textfiles-0.0.6/textfiles/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/__init__.py
+-rw-rw-rw-   0        0        0     9737 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/csv_file.py
+-rw-rw-rw-   0        0        0     1455 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/exceptions.py
+-rw-rw-rw-   0        0        0     2673 2023-05-04 16:27:12.000000 textfiles-0.0.6/textfiles/file_factory.py
+-rw-rw-rw-   0        0        0     8710 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/json_file.py
+-rw-rw-rw-   0        0        0     2529 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/text_file_parent.py
+-rw-rw-rw-   0        0        0     3867 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/txt_file.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.239961 textfiles-0.0.6/textfiles.egg-info/
+-rw-rw-rw-   0        0        0     3004 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/top_level.txt
```

### Comparing `textfiles-0.0.5/LICENSE` & `textfiles-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.5/PKG-INFO` & `textfiles-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,97 @@
-Metadata-Version: 2.1
-Name: textfiles
-Version: 0.0.5
-Summary: Managing the text files txt, csv and json
-Author: Yael Ben Yair, Hemed Tov
-Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
-Keywords: python,text,file,csv,json,txt
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# TextFiles v0.0.5
-A convenient Python API for working with the text files CSV, JSON, TXT
-
-The library allows handling csv, txt and json files easily from within Python.
-
-## Installation
-```terminal
-pip install textfiles
-```
-
-## How to use:
-
-Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
-
-```python
-from textfiles.file_factory import TextFile
-```
-
-Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
-
-make_file_instance: This method creates an instance of the file class for an existing text file.
-
-make_file: This method creates a new file and a corresponding Python instance of it.
-
-To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
-
-Examples: Here are some examples of how to use TextFile:
-
-To create an instance of an existing file:
-
-```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
-```
-
-To create a new file:
-
-```python
-file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
-file = TextFile.make_file('txt', 'path/to/file.txt')
-file = TextFile.make_file('json', 'path/to/file.json')
-```
-Note - When creating a CSV file, it is mandatory to pass a header.
-
-### Main functions:
-```python
-    self.get_content()
-    self.search()
-    self.count()
-```
-
-### examples:
-
-#### CsvFile.update_cell()
-```python
-    my_csv = CsvFile('/path/to/my/csv/file.csv')
-    my_csv.update_cell(column=3, row=2, value='New content')
-```
-
-#### JsonFile.search()
-```python
-    with open ("example.json", "w") as f:
-        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
-
-
-    my_json = JsonFile('/path/to/my/json/file.json')
-    new = my_json.search("new")
-    print(new)
-```
-
-output:
-```python
-[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
-```
+Metadata-Version: 2.1
+Name: textfiles
+Version: 0.0.6
+Summary: Managing the text files txt, csv and json
+Home-page: UNKNOWN
+Author: Yael Ben Yair, Hemed Tov
+Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
+License: UNKNOWN
+Keywords: python,text,file,csv,json,txt
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# TextFiles v0.0.6
+A convenient Python API for working with the text files CSV, JSON, TXT
+
+The library allows handling csv, txt and json files easily from within Python.
+
+## Installation
+```terminal
+pip install textfiles
+```
+
+## How to use:
+
+Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
+
+```python
+from textfiles.file_factory import TextFile
+```
+
+Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
+
+make_file_instance: This method creates an instance of the file class for an existing text file.
+
+make_file: This method creates a new file and a corresponding Python instance of it.
+
+To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
+
+Examples: Here are some examples of how to use TextFile:
+
+To create an instance of an existing file:
+
+```python
+file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('path/to/file.txt', 'txt')
+file = TextFile.make_file_instance('path/to/file.json', 'json')
+```
+
+To create a new file:
+
+```python
+file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
+file = TextFile.make_file('txt', 'path/to/file.txt')
+file = TextFile.make_file('json', 'path/to/file.json')
+```
+Note - When creating a CSV file, it is mandatory to pass a header.
+
+### Main functions:
+```python
+    self.get_content()
+    self.search()
+    self.count()
+```
+
+### examples:
+
+#### CsvFile.update_cell()
+```python
+    my_csv = CsvFile('/path/to/my/csv/file.csv')
+    my_csv.update_cell(column=3, row=2, value='New content')
+```
+
+#### JsonFile.search()
+```python
+    with open ("example.json", "w") as f:
+        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
+
+
+    my_json = JsonFile('/path/to/my/json/file.json')
+    new = my_json.search("new")
+    print(new)
+```
+
+output:
+```python
+[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
+```
+
+
```

### Comparing `textfiles-0.0.5/README.md` & `textfiles-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# TextFiles v0.0.5
-A convenient Python API for working with the text files CSV, JSON, TXT
-
-The library allows handling csv, txt and json files easily from within Python.
-
-## Installation
-```terminal
-pip install textfiles
-```
-
-## How to use:
-
-Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
-
-```python
-from textfiles.file_factory import TextFile
-```
-
-Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
-
-make_file_instance: This method creates an instance of the file class for an existing text file.
-
-make_file: This method creates a new file and a corresponding Python instance of it.
-
-To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
-
-Examples: Here are some examples of how to use TextFile:
-
-To create an instance of an existing file:
-
-```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
-```
-
-To create a new file:
-
-```python
-file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
-file = TextFile.make_file('txt', 'path/to/file.txt')
-file = TextFile.make_file('json', 'path/to/file.json')
-```
-Note - When creating a CSV file, it is mandatory to pass a header.
-
-### Main functions:
-```python
-    self.get_content()
-    self.search()
-    self.count()
-```
-
-### examples:
-
-#### CsvFile.update_cell()
-```python
-    my_csv = CsvFile('/path/to/my/csv/file.csv')
-    my_csv.update_cell(column=3, row=2, value='New content')
-```
-
-#### JsonFile.search()
-```python
-    with open ("example.json", "w") as f:
-        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
-
-
-    my_json = JsonFile('/path/to/my/json/file.json')
-    new = my_json.search("new")
-    print(new)
-```
-
-output:
-```python
-[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
-```
+# TextFiles v0.0.6
+A convenient Python API for working with the text files CSV, JSON, TXT
+
+The library allows handling csv, txt and json files easily from within Python.
+
+## Installation
+```terminal
+pip install textfiles
+```
+
+## How to use:
+
+Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
+
+```python
+from textfiles.file_factory import TextFile
+```
+
+Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
+
+make_file_instance: This method creates an instance of the file class for an existing text file.
+
+make_file: This method creates a new file and a corresponding Python instance of it.
+
+To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
+
+Examples: Here are some examples of how to use TextFile:
+
+To create an instance of an existing file:
+
+```python
+file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('path/to/file.txt', 'txt')
+file = TextFile.make_file_instance('path/to/file.json', 'json')
+```
+
+To create a new file:
+
+```python
+file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
+file = TextFile.make_file('txt', 'path/to/file.txt')
+file = TextFile.make_file('json', 'path/to/file.json')
+```
+Note - When creating a CSV file, it is mandatory to pass a header.
+
+### Main functions:
+```python
+    self.get_content()
+    self.search()
+    self.count()
+```
+
+### examples:
+
+#### CsvFile.update_cell()
+```python
+    my_csv = CsvFile('/path/to/my/csv/file.csv')
+    my_csv.update_cell(column=3, row=2, value='New content')
+```
+
+#### JsonFile.search()
+```python
+    with open ("example.json", "w") as f:
+        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
+
+
+    my_json = JsonFile('/path/to/my/json/file.json')
+    new = my_json.search("new")
+    print(new)
+```
+
+output:
+```python
+[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
+```
```

### Comparing `textfiles-0.0.5/textfiles/csv_file.py` & `textfiles-0.0.6/textfiles/csv_file.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-from __future__ import annotations
-from .text_file_parent import TextFile
-import csv, os
-from .exceptions import *
-
-# Menu for this file:
-    # built-in functions
-    # public functions - read
-    # math functions - write
-    # private functions
-
-
-class CsvFile(TextFile):
-
-    def __init__(self, file_path, delimiter=',', has_header=True, as_dict=False):
-        """
-        This class allows a convenient Python API for handling CSV files.
-        :param file_path: str
-        :param delimiter: default is ","
-        :param has_header: bool,  does file have header
-        :param as_dict: bool, would you prefer to access the information as a dictionary? Default is as False.
-        """
-
-        self._isheader = has_header
-        self._delimiter = delimiter
-        self.as_dict = as_dict
-        super().__init__(file_path)
-        self.connection = ""
-
-
-    def __str__ (self):
-        return f"{self.file_name}\n" \
-               f"contains {len(self)} rows\n" \
-               f"header: {self.header}\n" \
-               f"file creation time: {self.creation_time}\n" \
-               f"file last modified: {self.last_modified}"
-
-    def __contains__(self, item):
-        for row in self._content:
-            if item in row:
-                return True
-        return False
-
-    def __add__(self, other : CsvFile):
-        """
-        Creates a new csv file which combines the two. Headers muse be identical.
-        :param CsvFile, the file you wish to add
-        :return: CsvFIle, the new file
-        """
-
-        # ensure other is csv
-        if not isinstance(other, CsvFile):
-            raise InstanceError(type(other), 'csv')
-
-        # ensure headers are identical
-        h1 = self.header
-        h2 = other.header
-        if None in (h1, h2):
-            raise HeaderError('Both files should be with header')
-        if not self._is_identical(h1, h2):
-            raise HeaderError('The headers are not identical')
-
-        # new file path
-        new_fp = os.path.join(self.root, self.file_name + '_' + other.file_name + self._ext)
-
-        if os.path.exists(new_fp):
-            raise PathAlreadyExistsError(new_fp)
-
-        with open(new_fp, "w", newline="") as new_csv:
-            writer = csv.writer(new_csv)
-
-            for row in self.content:
-                writer.writerow(row)
-            for row in other.content[1:]:
-                writer.writerow(row)
-
-        new_csv = CsvFile(new_fp, has_header=True)
-        return new_csv
-
-    def __len__(self):
-        """
-        :return: number of rows in file, not including header
-        """
-        if self._isheader:
-            num_of_rows = -1
-        else:
-            num_of_rows = 0
-        for row in self._content:
-            print(row)
-            print(num_of_rows)
-            num_of_rows += 1
-        return num_of_rows
-
-    def __iter__(self):
-        for row in self.content():
-            yield row
-
-    def shape(self):
-        """
-        returns (num_of_rows, num_of_columns)
-        """
-        num_of_rows = 0
-        for row in self._content:
-            num_of_rows += 1
-        num_of_col = len(self.content[0])
-
-        return num_of_rows, num_of_col
-
-    @property
-    def header(self) -> list | None:
-        """
-        :return: list of str, the header of the csv file
-        """
-        if self._isheader:
-            return self.content[0]
-        else:
-            return None
-
-    def get_row(self, n, w=False):
-        """
-        :param w: bool - with headers in row?
-        :param n: wanted row number
-        :return: row content
-        """
-        if n not in range(len(self)):
-            raise OutOfRange(n)
-
-        wanted_row = self.content[n]
-        if w:
-            if self._isheader:
-                wanted_row = {wanted_row[i]: self.header[i] for i in range(len(wanted_row))}
-
-            else:
-                raise HeaderError('File has no header')
-            return wanted_row
-
-    def get_column_header(self, n):
-        """
-        :param n: number of column
-        :return: column name
-        """
-        if self._isheader:
-            return self.header[n]
-        else:
-            return None
-
-    def get_column_data(self, n):
-        """
-        :param n: column number
-        :return: list with all cells in column
-        """
-        column_data = [self.content[n] for row in self.content]
-        return column_data
-
-    def get_cell(self, row_num, column_num):
-        """
-        :param row_num:
-        :param column_num:
-        :return: content of table cell
-        """
-        with open(self._file_path, 'r', newline="") as csvf:
-            read_f = csv.reader(csvf, delimiter=self._delimiter)
-            csv_list = list(read_f)
-
-            # if the row and column out of range
-            if len(csv_list) < row_num - 1 and len(csv_list[0]) < column_num:
-                # raise ValueError (out of range)
-                pass
-
-            return csv_list[row_num][column_num - 1]
-
-    def search(self, value):
-        """
-        finds all appearances of given value in the file
-        :param value to search
-        :return: []list of tuples(row_num, column_num)
-        """
-        locations = []
-        for index, row in enumerate(self._content):
-            if value in row:
-                for i, v in enumerate(row):
-                    if v == value:
-                        locations.append((index, i))
-        return locations
-
-    def count(self, value) -> int:
-        """
-        Counts appearances of specific value in file
-        :param value:
-        :return: int, number of appearances
-        """
-        return len(self.search(value))
-
-    def add_row(self, row_to_add: list):
-        """Add a row to csv file, at end of file
-        :param list, in which every item will be placed in a column by order
-        """
-        self.lock.acquire()
-        with open(self.file_path, 'a') as f:
-            writer = csv.writer(f, delimiter=self._delimiter)
-            writer.writerow(row_to_add)
-
-        self.lock.release()
-
-    def delete_row(self, row_num=None, row_content=None):
-        """
-        Deletes a row of data from csv file.
-        Provide either row number or row content to delete
-        :param row_num: int
-        :param row_content: list
-        """
-        self.lock.acquire()
-        content = self.content
-        if row_num:
-            row_content = content[row_num]
-        content.remove(row_content)
-
-        with open(self.file_path, "w") as fh:
-            writer = csv.writer(fh)
-            writer.writerows(content)
-
-        self.lock.release()
-
-    def update_cell(self, cell_row, cell_column, new_value):
-        """
-        Change value of specific cell in csv file
-
-        :param cell_row: int
-        :param cell_column: int
-        :param new_value: What should be in the cell
-
-        """
-        if cell_row > len(self):
-            raise OutOfRange(cell_row)
-        if cell_column > len(self.content[1]):
-            raise OutOfRange(cell_column)
-
-        self.lock.acquire()
-
-        content = self.content()
-        content[cell_row][cell_column] = new_value
-
-        with open(self.file_path, "w") as fh:
-            writer = csv.writer(fh)
-            writer.writerows(content)
-
-        self.lock.release()
-
-    def average(self, n, beginning_row=0, end_row=None):
-        """
-        Calculates the average of values in a column. Only relevant for columns consisting of numbers.
-         :param n: column serial number
-         :param beginning_row: row serial number, default is all file.
-         :param end_row: row serial number, default is all file.
-         :return: float
-         """
-        sum_num = self.sum_column(n, beginning_row, end_row if end_row is not None else len(self))
-        divider = len(self.content[beginning_row:end_row if end_row is not None else len(self)])
-        return sum_num/divider
-
-    def sum_column(self, n, beginning_row=0, end_row=None):
-        """
-        Calculates the sum of values in a column, only relevant for columns consisting of numbers.
-        :param n: column serial number
-        :param beginning_row: row serial number, default is all file.
-        :param end_row: row serial number, default is all file.
-        :return: float
-        """
-        sum_num = 0
-        column = self.get_column_data(n)
-        for item in column[beginning_row:end_row if end_row is not None else len(self)]:
-            if isinstance(item, (int, float)):
-                sum_num += item
-        return sum_num
-
-    def _csv_list(self, fd):
-        """
-        :return: csv as list of lists
-        """
-        ret_val = []
-        for row in csv.reader(fd, delimiter=self._delimiter):
-            ret_val.append(row)
-        return ret_val
-
-    def _csv_dict(self, fd):
-        """
-        :return: csv as list of dicts
-        """
-        ret_val = []
-        for row in csv.DictReader(fd, delimiter=self._delimiter):
-            ret_val.append(row)
-        return ret_val
-
-    def _specific_content(self, fd):
-        """
-        :param
-        :return: list
-        """
-        if not self.as_dict:
-            return self._csv_list(fd)
-        return self._csv_dict(fd)
-
-    def _ext(self):
-        return 'csv'
-
-    @staticmethod
-    def _is_identical(h1: list, h2: list) -> bool:
-        """
-        Compares headers to ensure safe join
-        :param h1: list
-        :param h2: list
-        :return: bool
-        """
-        return h1 == h2
+from __future__ import annotations
+from .text_file_parent import TextFile
+import csv, os
+from .exceptions import *
+
+# Menu for this file:
+    # built-in functions
+    # public functions - read
+    # math functions - write
+    # private functions
+
+
+class CsvFile(TextFile):
+
+    def __init__(self, file_path, delimiter=',', has_header=True, as_dict=False):
+        """
+        This class allows a convenient Python API for handling CSV files.
+        :param file_path: str
+        :param delimiter: default is ","
+        :param has_header: bool,  does file have header
+        :param as_dict: bool, would you prefer to access the information as a dictionary? Default is as False.
+        """
+
+        self._isheader = has_header
+        self._delimiter = delimiter
+        self.as_dict = as_dict
+        super().__init__(file_path)
+        self.connection = ""
+
+
+    def __str__ (self):
+        return f"{self.file_name}\n" \
+               f"contains {len(self)} rows\n" \
+               f"header: {self.header}\n" \
+               f"file creation time: {self.creation_time}\n" \
+               f"file last modified: {self.last_modified}"
+
+    def __contains__(self, item):
+        for row in self._content:
+            if item in row:
+                return True
+        return False
+
+    def __add__(self, other : CsvFile):
+        """
+        Creates a new csv file which combines the two. Headers muse be identical.
+        :param CsvFile, the file you wish to add
+        :return: CsvFIle, the new file
+        """
+
+        # ensure other is csv
+        if not isinstance(other, CsvFile):
+            raise InstanceError(type(other), 'csv')
+
+        # ensure headers are identical
+        h1 = self.header
+        h2 = other.header
+        if None in (h1, h2):
+            raise HeaderError('Both files should be with header')
+        if not self._is_identical(h1, h2):
+            raise HeaderError('The headers are not identical')
+
+        # new file path
+        new_fp = os.path.join(self.root, self.file_name + '_' + other.file_name + self._ext)
+
+        if os.path.exists(new_fp):
+            raise PathAlreadyExistsError(new_fp)
+
+        with open(new_fp, "w", newline="") as new_csv:
+            writer = csv.writer(new_csv)
+
+            for row in self.content:
+                writer.writerow(row)
+            for row in other.content[1:]:
+                writer.writerow(row)
+
+        new_csv = CsvFile(new_fp, has_header=True)
+        return new_csv
+
+    def __len__(self):
+        """
+        :return: number of rows in file, not including header
+        """
+        if self._isheader:
+            num_of_rows = -1
+        else:
+            num_of_rows = 0
+        for row in self._content:
+            print(row)
+            print(num_of_rows)
+            num_of_rows += 1
+        return num_of_rows
+
+    def __iter__(self):
+        for row in self.content():
+            yield row
+
+    def shape(self):
+        """
+        returns (num_of_rows, num_of_columns)
+        """
+        num_of_rows = 0
+        for row in self._content:
+            num_of_rows += 1
+        num_of_col = len(self.content[0])
+
+        return num_of_rows, num_of_col
+
+    @property
+    def header(self) -> list | None:
+        """
+        :return: list of str, the header of the csv file
+        """
+        if self._isheader:
+            return self.content[0]
+        else:
+            return None
+
+    def get_row(self, n, w=False):
+        """
+        :param w: bool - with headers in row?
+        :param n: wanted row number
+        :return: row content
+        """
+        if n not in range(len(self)):
+            raise OutOfRange(n)
+
+        wanted_row = self.content[n]
+        if w:
+            if self._isheader:
+                wanted_row = {wanted_row[i]: self.header[i] for i in range(len(wanted_row))}
+
+            else:
+                raise HeaderError('File has no header')
+            return wanted_row
+
+    def get_column_header(self, n):
+        """
+        :param n: number of column
+        :return: column name
+        """
+        if self._isheader:
+            return self.header[n]
+        else:
+            return None
+
+    def get_column_data(self, n):
+        """
+        :param n: column number
+        :return: list with all cells in column
+        """
+        column_data = [self.content[n] for row in self.content]
+        return column_data
+
+    def get_cell(self, row_num, column_num):
+        """
+        :param row_num:
+        :param column_num:
+        :return: content of table cell
+        """
+        with open(self._file_path, 'r', newline="") as csvf:
+            read_f = csv.reader(csvf, delimiter=self._delimiter)
+            csv_list = list(read_f)
+
+            # if the row and column out of range
+            if len(csv_list) < row_num - 1 and len(csv_list[0]) < column_num:
+                # raise ValueError (out of range)
+                pass
+
+            return csv_list[row_num][column_num - 1]
+
+    def search(self, value):
+        """
+        finds all appearances of given value in the file
+        :param value to search
+        :return: []list of tuples(row_num, column_num)
+        """
+        locations = []
+        for index, row in enumerate(self._content):
+            if value in row:
+                for i, v in enumerate(row):
+                    if v == value:
+                        locations.append((index, i))
+        return locations
+
+    def count(self, value) -> int:
+        """
+        Counts appearances of specific value in file
+        :param value:
+        :return: int, number of appearances
+        """
+        return len(self.search(value))
+
+    def add_row(self, row_to_add: list):
+        """Add a row to csv file, at end of file
+        :param list, in which every item will be placed in a column by order
+        """
+        self.lock.acquire()
+        with open(self.file_path, 'a') as f:
+            writer = csv.writer(f, delimiter=self._delimiter)
+            writer.writerow(row_to_add)
+
+        self.lock.release()
+
+    def delete_row(self, row_num=None, row_content=None):
+        """
+        Deletes a row of data from csv file.
+        Provide either row number or row content to delete
+        :param row_num: int
+        :param row_content: list
+        """
+        self.lock.acquire()
+        content = self.content
+        if row_num:
+            row_content = content[row_num]
+        content.remove(row_content)
+
+        with open(self.file_path, "w") as fh:
+            writer = csv.writer(fh)
+            writer.writerows(content)
+
+        self.lock.release()
+
+    def update_cell(self, cell_row, cell_column, new_value):
+        """
+        Change value of specific cell in csv file
+
+        :param cell_row: int
+        :param cell_column: int
+        :param new_value: What should be in the cell
+
+        """
+        if cell_row > len(self):
+            raise OutOfRange(cell_row)
+        if cell_column > len(self.content[1]):
+            raise OutOfRange(cell_column)
+
+        self.lock.acquire()
+
+        content = self.content()
+        content[cell_row][cell_column] = new_value
+
+        with open(self.file_path, "w") as fh:
+            writer = csv.writer(fh)
+            writer.writerows(content)
+
+        self.lock.release()
+
+    def average(self, n, beginning_row=0, end_row=None):
+        """
+        Calculates the average of values in a column. Only relevant for columns consisting of numbers.
+         :param n: column serial number
+         :param beginning_row: row serial number, default is all file.
+         :param end_row: row serial number, default is all file.
+         :return: float
+         """
+        sum_num = self.sum_column(n, beginning_row, end_row if end_row is not None else len(self))
+        divider = len(self.content[beginning_row:end_row if end_row is not None else len(self)])
+        return sum_num/divider
+
+    def sum_column(self, n, beginning_row=0, end_row=None):
+        """
+        Calculates the sum of values in a column, only relevant for columns consisting of numbers.
+        :param n: column serial number
+        :param beginning_row: row serial number, default is all file.
+        :param end_row: row serial number, default is all file.
+        :return: float
+        """
+        sum_num = 0
+        column = self.get_column_data(n)
+        for item in column[beginning_row:end_row if end_row is not None else len(self)]:
+            if isinstance(item, (int, float)):
+                sum_num += item
+        return sum_num
+
+    def _csv_list(self, fd):
+        """
+        :return: csv as list of lists
+        """
+        ret_val = []
+        for row in csv.reader(fd, delimiter=self._delimiter):
+            ret_val.append(row)
+        return ret_val
+
+    def _csv_dict(self, fd):
+        """
+        :return: csv as list of dicts
+        """
+        ret_val = []
+        for row in csv.DictReader(fd, delimiter=self._delimiter):
+            ret_val.append(row)
+        return ret_val
+
+    def _specific_content(self, fd):
+        """
+        :param
+        :return: list
+        """
+        if not self.as_dict:
+            return self._csv_list(fd)
+        return self._csv_dict(fd)
+
+    def _ext(self):
+        return 'csv'
+
+    @staticmethod
+    def _is_identical(h1: list, h2: list) -> bool:
+        """
+        Compares headers to ensure safe join
+        :param h1: list
+        :param h2: list
+        :return: bool
+        """
+        return h1 == h2
```

### Comparing `textfiles-0.0.5/textfiles/exceptions.py` & `textfiles-0.0.6/textfiles/exceptions.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-class TextFileExceptions(Exception):
-    pass
-
-
-class NoFile(TextFileExceptions):
-    pass
-
-
-class InvalidInputError(TextFileExceptions):
-    def __init__(self, val):
-        super().__init__(f"{val} not in..")
-
-
-# class TypeError(TextFileExceptions):
-#     pass
-
-
-class PathAlreadyExistsError(TextFileExceptions):
-    def __init__(self, val):
-        super().__init__(f"{val} already exist")
-
-
-class FilePathNotExistsError(TextFileExceptions):
-    def __init__(self, val):
-        super().__init__(f"'{val}': file not exists")
-
-
-class InstanceError(TextFileExceptions):
-    def __init__(self, type_other, type_class):
-        super().__init__(f"can't add {type_other} file to {type_class} file")
-
-
-class HeaderError(TextFileExceptions):
-    def __init__(self, text):
-        super().__init__(text)
-
-
-class OutOfRange(TextFileExceptions):
-    def __init__(self, param):
-        super().__init__(f'{param} not in range')
-
-class KeyValueError(TextFileExceptions):
-    def __init__(self, msg):
-        super().__init__(msg)
-
-
-class IndexValueError(TextFileExceptions):
-    def __init__(self, msg):
-        super().__init__(msg)
-
-
-class InvalidTypeError(TextFileExceptions):
-        def __init__(self, param):
-            super().__init__(f'{param} file not supported')
-
-
-class SizeError(TextFileExceptions):
-        def __init__(self, param):
-            super().__init__(f'{param} is too large')
-
+class TextFileExceptions(Exception):
+    pass
+
+
+class NoFile(TextFileExceptions):
+    pass
+
+
+class InvalidInputError(TextFileExceptions):
+    def __init__(self, val):
+        super().__init__(f"{val} not in..")
+
+
+# class TypeError(TextFileExceptions):
+#     pass
+
+
+class PathAlreadyExistsError(TextFileExceptions):
+    def __init__(self, val):
+        super().__init__(f"{val} already exist")
+
+
+class FilePathNotExistsError(TextFileExceptions):
+    def __init__(self, val):
+        super().__init__(f"'{val}': file not exists")
+
+
+class InstanceError(TextFileExceptions):
+    def __init__(self, type_other, type_class):
+        super().__init__(f"can't add {type_other} file to {type_class} file")
+
+
+class HeaderError(TextFileExceptions):
+    def __init__(self, text):
+        super().__init__(text)
+
+
+class OutOfRange(TextFileExceptions):
+    def __init__(self, param):
+        super().__init__(f'{param} not in range')
+
+class KeyValueError(TextFileExceptions):
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
+class IndexValueError(TextFileExceptions):
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
+class InvalidTypeError(TextFileExceptions):
+        def __init__(self, param):
+            super().__init__(f'{param} file not supported')
+
+
+class SizeError(TextFileExceptions):
+        def __init__(self, param):
+            super().__init__(f'{param} is too large')
+
```

### Comparing `textfiles-0.0.5/textfiles/file_factory.py` & `textfiles-0.0.6/textfiles/file_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import json, csv
-import os.path
-from .csv_file import CsvFile
-from .json_file import JsonFile
-from .txt_file import TxtFile
-from .exceptions import *
-
-
-class TextFile:
-
-    @staticmethod
-    def make_file_instance(path: str, filetype: str, has_header: bool = True, delimiter: str = ',', max_size: int = 50)\
-            ->\
-            CsvFile | TxtFile | JsonFile:
-        """
-        This functions creates a file class instance for an existing text file.
-        If the file type is not one of the three specified -> txt, csv, json,
-        it will not be possible to use the library.
-        :param filetype: str (csv/json/txt).
-        :param path: str, file path.
-        :param has_header: bool, applicable for csv files only. Does the file have a header? Default is True.
-        :param delimiter: str, applicable for csv files only. Character or sequence of characters that separate columns.
-         Default is ','.
-        :param max_size: int, max file size in MB that TextFile should allow. Default is 50.
-        :return: instance of CsvFile | TxtFile | JsonFile
-        """
-        max_size = max_size*1000000
-        size = os.path.getsize(path)
-
-        # ensures file is within size limits
-        if size > max_size:
-            raise SizeError()
-
-        # create instance
-        if filetype == 'csv':
-            return CsvFile(path, delimiter, has_header)
-        elif filetype == 'txt':
-            return TxtFile(path)
-        elif filetype == 'json':
-            return JsonFile(path)
-
-        else:
-            raise InvalidTypeError()
-
-
-    @staticmethod
-    def make_file(filetype: str, path: str, header: list = None) -> CsvFile | TxtFile | JsonFile:
-        """
-        Creates new file in the file path, and a corresponding Python instance of it.
-        :param filetype: str, must be 'csv', 'txt' or 'json'
-        :param path: str, must be valid clear path
-        :param header: list, for csv files only. Provide a list of column headers.
-        :return: instance of TxtFIle | JsonFile | CsvFile
-        """
-
-        if filetype == 'csv':
-            with open(path, 'w', newline="") as cv:
-                write = csv.DictWriter(cv, fieldnames=header)
-                write.writeheader()
-                return CsvFile(path)
-
-        elif filetype == 'txt':
-            fh = open(path, 'x')
-            fh.close()
-            return TxtFile(path)
-
-        elif filetype == 'json':
-            with open(path, 'w') as js:
-                json.dump(js, None)
-            return JsonFile(path)
-
-        else:
-            raise InvalidTypeError()
+import json, csv
+import os.path
+from .csv_file import CsvFile
+from .json_file import JsonFile
+from .txt_file import TxtFile
+from .exceptions import *
+
+
+class TextFile:
+
+    @staticmethod
+    def make_file_instance(path: str, filetype: str, has_header: bool = True, delimiter: str = ',', max_size: int = 50)\
+            ->\
+            CsvFile | TxtFile | JsonFile:
+        """
+        This functions creates a file class instance for an existing text file.
+        If the file type is not one of the three specified -> txt, csv, json,
+        it will not be possible to use the library.
+        :param filetype: str (csv/json/txt).
+        :param path: str, file path.
+        :param has_header: bool, applicable for csv files only. Does the file have a header? Default is True.
+        :param delimiter: str, applicable for csv files only. Character or sequence of characters that separate columns.
+         Default is ','.
+        :param max_size: int, max file size in MB that TextFile should allow. Default is 50.
+        :return: instance of CsvFile | TxtFile | JsonFile
+        """
+        max_size = max_size*1000000
+        size = os.path.getsize(path)
+
+        # ensures file is within size limits
+        if size > max_size:
+            raise SizeError(path)
+
+        # create instance
+        if filetype == 'csv':
+            return CsvFile(path, delimiter, has_header)
+        elif filetype == 'txt':
+            return TxtFile(path)
+        elif filetype == 'json':
+            return JsonFile(path)
+
+        else:
+            raise InvalidTypeError(filetype)
+
+
+    @staticmethod
+    def make_file(filetype: str, path: str, header: list = None) -> CsvFile | TxtFile | JsonFile:
+        """
+        Creates new file in the file path, and a corresponding Python instance of it.
+        :param filetype: str, must be 'csv', 'txt' or 'json'
+        :param path: str, must be valid clear path
+        :param header: list, for csv files only. Provide a list of column headers.
+        :return: instance of TxtFIle | JsonFile | CsvFile
+        """
+
+        if filetype == 'csv':
+            with open(path, 'w', newline="") as cv:
+                write = csv.DictWriter(cv, fieldnames=header)
+                write.writeheader()
+                return CsvFile(path)
+
+        elif filetype == 'txt':
+            fh = open(path, 'x')
+            fh.close()
+            return TxtFile(path)
+
+        elif filetype == 'json':
+            with open(path, 'w') as js:
+                json.dump(None, js)
+            return JsonFile(path)
+
+        else:
+            raise InvalidTypeError(filetype)
```

### Comparing `textfiles-0.0.5/textfiles/text_file_parent.py` & `textfiles-0.0.6/textfiles/text_file_parent.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from abc import ABC, abstractmethod
-import os
-from .exceptions import *
-import time
-from threading import Lock
-
-
-class TextFile(ABC):
-
-    def __init__(self, file_path: str):
-        self._file_path = file_path
-
-        if not os.path.exists(self._file_path):
-            raise FileNotFoundError()
-        if self._ext() != self.get_extension():
-            raise TypeError
-        if os.path.getsize(self._file_path) > 50000000:
-            raise SizeError("File to large to handle with this library")
-
-
-        self._content = self.load_content()
-        self._file_size = os.stat(self._file_path).st_size
-        self._root = os.path.dirname(self._file_path)
-        self._base_name = os.path.basename(self._file_path)
-        self._file_name = os.path.splitext(self.base_name)[0]
-        self._creation_t = self.get_creation_time()
-        self._last_modified_t = self._update_last_modified()
-        self.lock = Lock()
-
-    def __str__(self):
-        return str(self._content)
-
-    @abstractmethod
-    def _ext(self):
-        pass
-
-    @abstractmethod
-    def _specific_content(self, fd):
-        pass
-
-    @abstractmethod
-    def search(self, val):
-        raise Exception()
-
-
-    @abstractmethod
-    def count(self, val) -> int:
-        raise Exception()
-
-
-    def load_content(self):
-        """
-        The function loads the content of the file according to its type. -> csv, txt, json
-        """
-        with open(self._file_path, 'r') as fd:
-            content = self._specific_content(fd)
-        return content
-
-    def get_extension(self):
-        return os.path.splitext(self._file_path)[-1][1:]
-
-    def get_file_path(self):
-        return self._file_path
-
-    def get_creation_time(self):
-        return os.path.getctime(self._file_path)
-
-    def _update_last_modified(self):
-        return os.path.getmtime(self._file_path)
-
-
-    @property
-    def content(self):
-        return self._content
-
-    @property
-    def creation_time(self):
-        return self._creation_t
-
-    @property
-    def last_modified(self):
-        return time.ctime(self._last_modified_t)
-
-    @property
-    def file_path(self):
-        return self._file_path
-
-    @property
-    def file_size(self):
-        return self._file_size
-
-    @property
-    def root(self):
-        return self._root
-
-    @property
-    def base_name(self):
-        return self._base_name
-
-    @property
-    def file_name(self):
-        return self._file_name
+from abc import ABC, abstractmethod
+import os
+from .exceptions import *
+import time
+from threading import Lock
+
+
+class TextFile(ABC):
+
+    def __init__(self, file_path: str):
+        self._file_path = file_path
+
+        if not os.path.exists(self._file_path):
+            raise FileNotFoundError()
+        if self._ext() != self.get_extension():
+            raise TypeError
+        if os.path.getsize(self._file_path) > 50000000:
+            raise SizeError("File to large to handle with this library")
+
+
+        self._content = self.load_content()
+        self._file_size = os.stat(self._file_path).st_size
+        self._root = os.path.dirname(self._file_path)
+        self._base_name = os.path.basename(self._file_path)
+        self._file_name = os.path.splitext(self.base_name)[0]
+        self._creation_t = self.get_creation_time()
+        self._last_modified_t = self._update_last_modified()
+        self.lock = Lock()
+
+    def __str__(self):
+        return str(self._content)
+
+    @abstractmethod
+    def _ext(self):
+        pass
+
+    @abstractmethod
+    def _specific_content(self, fd):
+        pass
+
+    @abstractmethod
+    def search(self, val):
+        raise Exception()
+
+
+    @abstractmethod
+    def count(self, val) -> int:
+        raise Exception()
+
+
+    def load_content(self):
+        """
+        The function loads the content of the file according to its type. -> csv, txt, json
+        """
+        with open(self._file_path, 'r') as fd:
+            content = self._specific_content(fd)
+        return content
+
+    def get_extension(self):
+        return os.path.splitext(self._file_path)[-1][1:]
+
+    def get_file_path(self):
+        return self._file_path
+
+    def get_creation_time(self):
+        return os.path.getctime(self._file_path)
+
+    def _update_last_modified(self):
+        return os.path.getmtime(self._file_path)
+
+
+    @property
+    def content(self):
+        return self._content
+
+    @property
+    def creation_time(self):
+        return self._creation_t
+
+    @property
+    def last_modified(self):
+        return time.ctime(self._last_modified_t)
+
+    @property
+    def file_path(self):
+        return self._file_path
+
+    @property
+    def file_size(self):
+        return self._file_size
+
+    @property
+    def root(self):
+        return self._root
+
+    @property
+    def base_name(self):
+        return self._base_name
+
+    @property
+    def file_name(self):
+        return self._file_name
```

### Comparing `textfiles-0.0.5/textfiles/txt_file.py` & `textfiles-0.0.6/textfiles/txt_file.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-from .text_file_parent import TextFile
-from .exceptions import *
-import os
-
-
-class TxtFile (TextFile):
-    """
-    The class corresponds to a txt file, allowing an easy API for handling it.
-    To initiate, simply provide the file path as a string.
-    """
-
-    def __init__(self, file_path):
-        super().__init__(file_path)
-        self.lines = self._read_lines()
-
-    @staticmethod
-    def _specific_content(fd):
-        return fd.read()
-
-    def _read_lines(self):
-        with open(self.file_path) as fh:
-            lines = fh.readlines()
-        return lines
-
-    def __add__(self, other) -> bool:
-        """
-        Creates new file that combines two existing txt files
-        :param other: TxtFIle
-        :return: bool, just to approve file was created
-        """
-
-        if not isinstance(other, TxtFile):
-            raise ValueError("both files must be .txt")
-
-        self.lock.acquire()
-
-        new_name = os.path.join(self.root, self.file_name + '_' + other.file_name + '.' + self._ext)
-
-        if os.path.exists(new_name):
-            raise PathAlreadyExistsError(new_name)
-
-        with open(new_name, 'x') as fh:
-            fh.write(self._content + other._content)
-
-        self.lock.release()
-
-        return True
-
-    def __len__(self) -> int:
-        """
-        :return: int, number of words in txt
-        """
-        return len(self.words)
-
-    def __contains__(self, item: str | int) -> bool:
-
-        if item in self._content:
-            return True
-        else:
-            return False
-
-    def __iter__(self):
-        return iter(self.words)
-
-
-    def __str__(self):
-        return f"{self.file_name}\n" \
-               f"contains {len(self.lines)} lines\n" \
-               f"file creation time: {self.creation_time}\n" \
-               f"file last modified: {self.last_modified}"
-
-    @property
-    def words(self) -> list:
-        """
-        :return: list of words in txt file
-        """
-        to_remove = []
-        list_of_words = self._content.split()
-        for i in range(len(list_of_words)):
-            if list_of_words[i][-1] == "-":
-                list_of_words[i] = list_of_words[i][0:-2] + list_of_words[i + 1]
-                to_remove.append(list_of_words[i + 1])
-        for word in to_remove:
-            list_of_words.remove(word)
-        return list_of_words
-
-    def search(self, val):
-        """
-        :param val: string to search
-        :return: list of tuples with index and line for where str was found
-        """
-        if val not in self:
-            return None
-        findings = []
-        for index, line in enumerate(self.lines):
-            if val in line:
-                findings.append((index, line))
-        return findings
-
-    def add_line(self, line, line_num=None):
-        """
-        Adds a line to txt file in specified place (index).
-        :param line: str, content to be added
-        :param line_num: int, index number of line to add. Default is last line.
-        """
-        if line_num is None:
-            line_num = len(self.lines)
-
-            self.lock.acquire()
-            with open(self._file_path, "a") as fh:
-                fh.write(f"\n"
-                         f"{line}\n")
-            self.lock.release()
-
-        else:
-            self.lock.acquire()
-            new_text = self.lines[:line_num] + line + self.lines[line_num:]
-            with open(self.file_path, "w") as fh:
-                fh.write(new_text)
-            self.lock.release()
-
-    def count(self, val) -> int:
-        """
-        Counts appearance of value in file
-        :param: str, value to be searched
-        :return: int, number of appearances
-        """
-
-        return self.content.count(val)
-
-    def _ext(self):
-        return 'txt'
+from .text_file_parent import TextFile
+from .exceptions import *
+import os
+
+
+class TxtFile (TextFile):
+    """
+    The class corresponds to a txt file, allowing an easy API for handling it.
+    To initiate, simply provide the file path as a string.
+    """
+
+    def __init__(self, file_path):
+        super().__init__(file_path)
+        self.lines = self._read_lines()
+
+    @staticmethod
+    def _specific_content(fd):
+        return fd.read()
+
+    def _read_lines(self):
+        with open(self.file_path) as fh:
+            lines = fh.readlines()
+        return lines
+
+    def __add__(self, other) -> bool:
+        """
+        Creates new file that combines two existing txt files
+        :param other: TxtFIle
+        :return: bool, just to approve file was created
+        """
+
+        if not isinstance(other, TxtFile):
+            raise ValueError("both files must be .txt")
+
+        self.lock.acquire()
+
+        new_name = os.path.join(self.root, self.file_name + '_' + other.file_name + '.' + self._ext)
+
+        if os.path.exists(new_name):
+            raise PathAlreadyExistsError(new_name)
+
+        with open(new_name, 'x') as fh:
+            fh.write(self._content + other._content)
+
+        self.lock.release()
+
+        return True
+
+    def __len__(self) -> int:
+        """
+        :return: int, number of words in txt
+        """
+        return len(self.words)
+
+    def __contains__(self, item: str | int) -> bool:
+
+        if item in self._content:
+            return True
+        else:
+            return False
+
+    def __iter__(self):
+        return iter(self.words)
+
+
+    def __str__(self):
+        return f"{self.file_name}\n" \
+               f"contains {len(self.lines)} lines\n" \
+               f"file creation time: {self.creation_time}\n" \
+               f"file last modified: {self.last_modified}"
+
+    @property
+    def words(self) -> list:
+        """
+        :return: list of words in txt file
+        """
+        to_remove = []
+        list_of_words = self._content.split()
+        for i in range(len(list_of_words)):
+            if list_of_words[i][-1] == "-":
+                list_of_words[i] = list_of_words[i][0:-2] + list_of_words[i + 1]
+                to_remove.append(list_of_words[i + 1])
+        for word in to_remove:
+            list_of_words.remove(word)
+        return list_of_words
+
+    def search(self, val):
+        """
+        :param val: string to search
+        :return: list of tuples with index and line for where str was found
+        """
+        if val not in self:
+            return None
+        findings = []
+        for index, line in enumerate(self.lines):
+            if val in line:
+                findings.append((index, line))
+        return findings
+
+    def add_line(self, line, line_num=None):
+        """
+        Adds a line to txt file in specified place (index).
+        :param line: str, content to be added
+        :param line_num: int, index number of line to add. Default is last line.
+        """
+        if line_num is None:
+            line_num = len(self.lines)
+
+            self.lock.acquire()
+            with open(self._file_path, "a") as fh:
+                fh.write(f"\n"
+                         f"{line}\n")
+            self.lock.release()
+
+        else:
+            self.lock.acquire()
+            new_text = self.lines[:line_num] + line + self.lines[line_num:]
+            with open(self.file_path, "w") as fh:
+                fh.write(new_text)
+            self.lock.release()
+
+    def count(self, val) -> int:
+        """
+        Counts appearance of value in file
+        :param: str, value to be searched
+        :return: int, number of appearances
+        """
+
+        return self.content.count(val)
+
+    def _ext(self):
+        return 'txt'
```

### Comparing `textfiles-0.0.5/textfiles.egg-info/PKG-INFO` & `textfiles-0.0.6/textfiles.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,97 @@
-Metadata-Version: 2.1
-Name: textfiles
-Version: 0.0.5
-Summary: Managing the text files txt, csv and json
-Author: Yael Ben Yair, Hemed Tov
-Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
-Keywords: python,text,file,csv,json,txt
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# TextFiles v0.0.5
-A convenient Python API for working with the text files CSV, JSON, TXT
-
-The library allows handling csv, txt and json files easily from within Python.
-
-## Installation
-```terminal
-pip install textfiles
-```
-
-## How to use:
-
-Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
-
-```python
-from textfiles.file_factory import TextFile
-```
-
-Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
-
-make_file_instance: This method creates an instance of the file class for an existing text file.
-
-make_file: This method creates a new file and a corresponding Python instance of it.
-
-To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
-
-Examples: Here are some examples of how to use TextFile:
-
-To create an instance of an existing file:
-
-```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
-```
-
-To create a new file:
-
-```python
-file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
-file = TextFile.make_file('txt', 'path/to/file.txt')
-file = TextFile.make_file('json', 'path/to/file.json')
-```
-Note - When creating a CSV file, it is mandatory to pass a header.
-
-### Main functions:
-```python
-    self.get_content()
-    self.search()
-    self.count()
-```
-
-### examples:
-
-#### CsvFile.update_cell()
-```python
-    my_csv = CsvFile('/path/to/my/csv/file.csv')
-    my_csv.update_cell(column=3, row=2, value='New content')
-```
-
-#### JsonFile.search()
-```python
-    with open ("example.json", "w") as f:
-        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
-
-
-    my_json = JsonFile('/path/to/my/json/file.json')
-    new = my_json.search("new")
-    print(new)
-```
-
-output:
-```python
-[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
-```
+Metadata-Version: 2.1
+Name: textfiles
+Version: 0.0.6
+Summary: Managing the text files txt, csv and json
+Home-page: UNKNOWN
+Author: Yael Ben Yair, Hemed Tov
+Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
+License: UNKNOWN
+Keywords: python,text,file,csv,json,txt
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# TextFiles v0.0.6
+A convenient Python API for working with the text files CSV, JSON, TXT
+
+The library allows handling csv, txt and json files easily from within Python.
+
+## Installation
+```terminal
+pip install textfiles
+```
+
+## How to use:
+
+Import TextFile: Once you install the library you can import the TextFile class into your Python code. To do this, simply add the following line to your code:
+
+```python
+from textfiles.file_factory import TextFile
+```
+
+Use TextFile: You can now use the TextFile class to create instances of CsvFile, TxtFile, and JsonFile classes. The factory has two methods:
+
+make_file_instance: This method creates an instance of the file class for an existing text file.
+
+make_file: This method creates a new file and a corresponding Python instance of it.
+
+To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
+
+Examples: Here are some examples of how to use TextFile:
+
+To create an instance of an existing file:
+
+```python
+file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('path/to/file.txt', 'txt')
+file = TextFile.make_file_instance('path/to/file.json', 'json')
+```
+
+To create a new file:
+
+```python
+file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
+file = TextFile.make_file('txt', 'path/to/file.txt')
+file = TextFile.make_file('json', 'path/to/file.json')
+```
+Note - When creating a CSV file, it is mandatory to pass a header.
+
+### Main functions:
+```python
+    self.get_content()
+    self.search()
+    self.count()
+```
+
+### examples:
+
+#### CsvFile.update_cell()
+```python
+    my_csv = CsvFile('/path/to/my/csv/file.csv')
+    my_csv.update_cell(column=3, row=2, value='New content')
+```
+
+#### JsonFile.search()
+```python
+    with open ("example.json", "w") as f:
+        json.dump(f, {"State": "New York", "cities": ["New York", "Albeny", "New Paltz"]})
+
+
+    my_json = JsonFile('/path/to/my/json/file.json')
+    new = my_json.search("new")
+    print(new)
+```
+
+output:
+```python
+[{'State': 'New York'}, {'cities': [{'index[0]': 'New York'}, {'index[2]': 'New Paltz'}]}]
+```
+
+
```

