# Comparing `tmp/bioplotz-0.1.0.dev1.tar.gz` & `tmp/bioplotz-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioplotz-0.1.0.dev1.tar", last modified: Wed Apr 26 04:50:50 2023, max compression
+gzip compressed data, was "bioplotz-0.1.0.dev2.tar", last modified: Thu May  4 12:56:48 2023, max compression
```

## Comparing `bioplotz-0.1.0.dev1.tar` & `bioplotz-0.1.0.dev2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-04-26 04:50:50.176105 bioplotz-0.1.0.dev1/
--rw-r--r--   0 zsc       (1000) users      (100)       67 2023-04-26 04:27:01.000000 bioplotz-0.1.0.dev1/MANIFEST.in
--rw-r--r--   0 zsc       (1000) users      (100)    12311 2023-04-26 04:50:50.176105 bioplotz-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)    12037 2023-04-26 04:46:55.000000 bioplotz-0.1.0.dev1/README.md
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-04-26 04:50:50.176105 bioplotz-0.1.0.dev1/bioplotz/
--rw-r--r--   0 zsc       (1000) users      (100)      175 2023-04-26 04:27:01.000000 bioplotz-0.1.0.dev1/bioplotz/__init__.py
--rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-04-26 04:27:01.000000 bioplotz-0.1.0.dev1/bioplotz/chromosome.py
--rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-04-26 04:27:01.000000 bioplotz-0.1.0.dev1/bioplotz/genecluster.py
--rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-04-26 04:27:01.000000 bioplotz-0.1.0.dev1/bioplotz/manhattan.py
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-04-26 04:50:50.176105 bioplotz-0.1.0.dev1/bioplotz.egg-info/
--rw-r--r--   0 zsc       (1000) users      (100)    12311 2023-04-26 04:50:50.000000 bioplotz-0.1.0.dev1/bioplotz.egg-info/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)      279 2023-04-26 04:50:50.000000 bioplotz-0.1.0.dev1/bioplotz.egg-info/SOURCES.txt
--rw-r--r--   0 zsc       (1000) users      (100)        1 2023-04-26 04:50:50.000000 bioplotz-0.1.0.dev1/bioplotz.egg-info/dependency_links.txt
--rw-r--r--   0 zsc       (1000) users      (100)       24 2023-04-26 04:50:50.000000 bioplotz-0.1.0.dev1/bioplotz.egg-info/requires.txt
--rw-r--r--   0 zsc       (1000) users      (100)        9 2023-04-26 04:50:50.000000 bioplotz-0.1.0.dev1/bioplotz.egg-info/top_level.txt
--rw-r--r--   0 zsc       (1000) users      (100)       38 2023-04-26 04:50:50.176105 bioplotz-0.1.0.dev1/setup.cfg
--rw-r--r--   0 zsc       (1000) users      (100)      643 2023-04-26 04:50:25.000000 bioplotz-0.1.0.dev1/setup.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/
+-rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/LICENSE
+-rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/MANIFEST.in
+-rw-r--r--   0 zsc       (1000) users      (100)    13367 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)    13070 2023-05-04 12:42:00.000000 bioplotz-0.1.0.dev2/README.md
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/bioplotz/
+-rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-04 11:31:08.000000 bioplotz-0.1.0.dev2/bioplotz/__init__.py
+-rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/chromosome.py
+-rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/genecluster.py
+-rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/manhattan.py
+-rw-r--r--   0 zsc       (1000) users      (100)     3699 2023-05-04 12:08:05.000000 bioplotz-0.1.0.dev2/bioplotz/mulitalign.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/bioplotz.egg-info/
+-rw-r--r--   0 zsc       (1000) users      (100)    13367 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/SOURCES.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/dependency_links.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/requires.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/top_level.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/setup.cfg
+-rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-04 11:29:58.000000 bioplotz-0.1.0.dev2/setup.py
```

### Comparing `bioplotz-0.1.0.dev1/PKG-INFO` & `bioplotz-0.1.0.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## Introduction
 
 This is a package for plotting some images for bioinformatics.
 
 ## Dependencies
 Python modules:  
@@ -42,15 +43,15 @@
 | **block_line_width**     | value         | **value** if there are only one color, the block line will display as border, the width is set by this parameter                                                                                                                                                                                                                                                     |
 | **log_base**             | value         | log_base = 0 means not calucate value with log<br>log_base != 0 means log base for log values with it                                                                                                                                                                                                                                                                |
 | **reverse**              | Boolean       | if all data lower than 0, you may use it to show opposite values                                                                                                                                                                                                                                                                                                     |
 | **other parameters**     | value         | same with parameters used in **pyplot.scatter**                                                                                                                                                                                                                                                                                                                      |
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/manhattan.png"></td>
+<td><img width=600 src="examples/manhattan.png"></td>
 </tr>
 </table>
 
 ### Chromosome Plot
 
 ```python
 import bioplotz as bp
@@ -69,16 +70,16 @@
 | **cmap_parts**       | int                            | Yes      | 100          | how many parts for splitting cmap                                                                                                                                                                                                                                                                                 |
 | **s**                | float or array-like, shape(n,) | Yes      | None         | same with parameter s use in **pyplot.scatter**                                                                                                                                                                                                                                                                   |
 | **other parameters** | value                          | Yes      | None         | same with parameters used in **pyplot.plot**                                                                                                                                                                                                                                                                      |
 
 - If value_type is numeric, the return value clb will be colorbar, else None
 <table align="center">
 <tr>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome.png"></td>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome_h.png"></td>
+<td><img width=500 height=270 src="examples/chromosome.png"></td>
+<td><img width=500 height=270 src="examples/chromosome_h.png"></td>
 </tr>
 </table>
 
 ### Gene Cluster Plot
 
 ```python
 import bioplotz as bp
@@ -92,10 +93,40 @@
 | **edgewidth** | int         | Yes      | 1       | edge width for all genes                                                                                                                         |
 | **lw**        | int         | Yes      | 3       | line width to show the genome backbone                                                                                                           |
 
 **Notice**, the best figsize should be (gene count, 1), for example: plt.figure(figsize=(16, 1)), and the bbox_inches parameter which in savefig should be 'tight'.
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/genecluster.png"></td>
+<td><img width=600 src="examples/genecluster.png"></td>
+</tr>
+</table>
+
+### Multi Alignment Plot
+
+```python
+import bioplotz as bp
+
+fig, ax = bp.multialign(data)
+```
+| parameter          | value type | Optional | Default | explain                                             |
+|--------------------|------------|----------|---------|-----------------------------------------------------|
+| **data**           | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence |
+| **match_color**    | str        | Yes      | blue    | color for displaying matched bases                  |
+| **mismatch_color** | str        | Yes      | red     | color for highlighting mismatched bases             |
+| ****kwargs**       | any        | Yes      | -       | same with which use in ax.text                      |
+
+**Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
+like "Courier New", that sometimes user need add codes as following.
+```python
+import matplotlib as mpl
+import bioplotz as bp
+
+basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
+fig, ax = bp.multialign(data, fontproperties=basefont)
+```
+
+<table align="center">
+<tr>
+<td><img width=600 src="examples/multialign.png"></td>
 </tr>
 </table>
```

### Comparing `bioplotz-0.1.0.dev1/README.md` & `bioplotz-0.1.0.dev2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 | **block_line_width**     | value         | **value** if there are only one color, the block line will display as border, the width is set by this parameter                                                                                                                                                                                                                                                     |
 | **log_base**             | value         | log_base = 0 means not calucate value with log<br>log_base != 0 means log base for log values with it                                                                                                                                                                                                                                                                |
 | **reverse**              | Boolean       | if all data lower than 0, you may use it to show opposite values                                                                                                                                                                                                                                                                                                     |
 | **other parameters**     | value         | same with parameters used in **pyplot.scatter**                                                                                                                                                                                                                                                                                                                      |
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/manhattan.png"></td>
+<td><img width=600 src="examples/manhattan.png"></td>
 </tr>
 </table>
 
 ### Chromosome Plot
 
 ```python
 import bioplotz as bp
@@ -60,16 +60,16 @@
 | **cmap_parts**       | int                            | Yes      | 100          | how many parts for splitting cmap                                                                                                                                                                                                                                                                                 |
 | **s**                | float or array-like, shape(n,) | Yes      | None         | same with parameter s use in **pyplot.scatter**                                                                                                                                                                                                                                                                   |
 | **other parameters** | value                          | Yes      | None         | same with parameters used in **pyplot.plot**                                                                                                                                                                                                                                                                      |
 
 - If value_type is numeric, the return value clb will be colorbar, else None
 <table align="center">
 <tr>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome.png"></td>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome_h.png"></td>
+<td><img width=500 height=270 src="examples/chromosome.png"></td>
+<td><img width=500 height=270 src="examples/chromosome_h.png"></td>
 </tr>
 </table>
 
 ### Gene Cluster Plot
 
 ```python
 import bioplotz as bp
@@ -83,10 +83,40 @@
 | **edgewidth** | int         | Yes      | 1       | edge width for all genes                                                                                                                         |
 | **lw**        | int         | Yes      | 3       | line width to show the genome backbone                                                                                                           |
 
 **Notice**, the best figsize should be (gene count, 1), for example: plt.figure(figsize=(16, 1)), and the bbox_inches parameter which in savefig should be 'tight'.
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/genecluster.png"></td>
+<td><img width=600 src="examples/genecluster.png"></td>
 </tr>
 </table>
+
+### Multi Alignment Plot
+
+```python
+import bioplotz as bp
+
+fig, ax = bp.multialign(data)
+```
+| parameter          | value type | Optional | Default | explain                                             |
+|--------------------|------------|----------|---------|-----------------------------------------------------|
+| **data**           | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence |
+| **match_color**    | str        | Yes      | blue    | color for displaying matched bases                  |
+| **mismatch_color** | str        | Yes      | red     | color for highlighting mismatched bases             |
+| ****kwargs**       | any        | Yes      | -       | same with which use in ax.text                      |
+
+**Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
+like "Courier New", that sometimes user need add codes as following.
+```python
+import matplotlib as mpl
+import bioplotz as bp
+
+basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
+fig, ax = bp.multialign(data, fontproperties=basefont)
+```
+
+<table align="center">
+<tr>
+<td><img width=600 src="examples/multialign.png"></td>
+</tr>
+</table>
```

### Comparing `bioplotz-0.1.0.dev1/bioplotz/chromosome.py` & `bioplotz-0.1.0.dev2/bioplotz/chromosome.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev1/bioplotz/genecluster.py` & `bioplotz-0.1.0.dev2/bioplotz/genecluster.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev1/bioplotz/manhattan.py` & `bioplotz-0.1.0.dev2/bioplotz/manhattan.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev1/bioplotz.egg-info/PKG-INFO` & `bioplotz-0.1.0.dev2/bioplotz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## Introduction
 
 This is a package for plotting some images for bioinformatics.
 
 ## Dependencies
 Python modules:  
@@ -42,15 +43,15 @@
 | **block_line_width**     | value         | **value** if there are only one color, the block line will display as border, the width is set by this parameter                                                                                                                                                                                                                                                     |
 | **log_base**             | value         | log_base = 0 means not calucate value with log<br>log_base != 0 means log base for log values with it                                                                                                                                                                                                                                                                |
 | **reverse**              | Boolean       | if all data lower than 0, you may use it to show opposite values                                                                                                                                                                                                                                                                                                     |
 | **other parameters**     | value         | same with parameters used in **pyplot.scatter**                                                                                                                                                                                                                                                                                                                      |
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/manhattan.png"></td>
+<td><img width=600 src="examples/manhattan.png"></td>
 </tr>
 </table>
 
 ### Chromosome Plot
 
 ```python
 import bioplotz as bp
@@ -69,16 +70,16 @@
 | **cmap_parts**       | int                            | Yes      | 100          | how many parts for splitting cmap                                                                                                                                                                                                                                                                                 |
 | **s**                | float or array-like, shape(n,) | Yes      | None         | same with parameter s use in **pyplot.scatter**                                                                                                                                                                                                                                                                   |
 | **other parameters** | value                          | Yes      | None         | same with parameters used in **pyplot.plot**                                                                                                                                                                                                                                                                      |
 
 - If value_type is numeric, the return value clb will be colorbar, else None
 <table align="center">
 <tr>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome.png"></td>
-<td><img width=500 height=270 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/chromosome_h.png"></td>
+<td><img width=500 height=270 src="examples/chromosome.png"></td>
+<td><img width=500 height=270 src="examples/chromosome_h.png"></td>
 </tr>
 </table>
 
 ### Gene Cluster Plot
 
 ```python
 import bioplotz as bp
@@ -92,10 +93,40 @@
 | **edgewidth** | int         | Yes      | 1       | edge width for all genes                                                                                                                         |
 | **lw**        | int         | Yes      | 3       | line width to show the genome backbone                                                                                                           |
 
 **Notice**, the best figsize should be (gene count, 1), for example: plt.figure(figsize=(16, 1)), and the bbox_inches parameter which in savefig should be 'tight'.
 
 <table align="center">
 <tr>
-<td><img width=600 src="https://github.com/sc-zhang/bioplotz/blob/master/examples/genecluster.png"></td>
+<td><img width=600 src="examples/genecluster.png"></td>
+</tr>
+</table>
+
+### Multi Alignment Plot
+
+```python
+import bioplotz as bp
+
+fig, ax = bp.multialign(data)
+```
+| parameter          | value type | Optional | Default | explain                                             |
+|--------------------|------------|----------|---------|-----------------------------------------------------|
+| **data**           | dict       | No       | -       | **key**: gene name<br>**value**: alignment sequence |
+| **match_color**    | str        | Yes      | blue    | color for displaying matched bases                  |
+| **mismatch_color** | str        | Yes      | red     | color for highlighting mismatched bases             |
+| ****kwargs**       | any        | Yes      | -       | same with which use in ax.text                      |
+
+**Notice**, the figsize should be (8, x) where x=align_length/80*gene_count/5, and the font must be  monospaced, 
+like "Courier New", that sometimes user need add codes as following.
+```python
+import matplotlib as mpl
+import bioplotz as bp
+
+basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
+fig, ax = bp.multialign(data, fontproperties=basefont)
+```
+
+<table align="center">
+<tr>
+<td><img width=600 src="examples/multialign.png"></td>
 </tr>
 </table>
```

### Comparing `bioplotz-0.1.0.dev1/setup.py` & `bioplotz-0.1.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bioplotz',
-    version='0.1.0.dev1',
+    version='0.1.0.dev2',
     packages=['bioplotz'],
     url='https://github.com/sc-zhang/bioplotz',
     license='',
     author='Shengcheng Zhang',
     author_email='zsc-zhang@foxmail.com',
     description='A python package for drawing some bioinformatic pictures.',
     long_description=long_description,
```

