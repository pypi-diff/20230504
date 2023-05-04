# Comparing `tmp/bioplotz-0.1.0.dev2.tar.gz` & `tmp/bioplotz-0.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioplotz-0.1.0.dev2.tar", last modified: Thu May  4 12:56:48 2023, max compression
+gzip compressed data, was "bioplotz-0.1.0.dev3.tar", last modified: Thu May  4 13:09:28 2023, max compression
```

## Comparing `bioplotz-0.1.0.dev2.tar` & `bioplotz-0.1.0.dev3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/
--rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/LICENSE
--rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/MANIFEST.in
--rw-r--r--   0 zsc       (1000) users      (100)    13367 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)    13070 2023-05-04 12:42:00.000000 bioplotz-0.1.0.dev2/README.md
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/bioplotz/
--rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-04 11:31:08.000000 bioplotz-0.1.0.dev2/bioplotz/__init__.py
--rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/chromosome.py
--rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/genecluster.py
--rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev2/bioplotz/manhattan.py
--rw-r--r--   0 zsc       (1000) users      (100)     3699 2023-05-04 12:08:05.000000 bioplotz-0.1.0.dev2/bioplotz/mulitalign.py
-drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/bioplotz.egg-info/
--rw-r--r--   0 zsc       (1000) users      (100)    13367 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/PKG-INFO
--rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/SOURCES.txt
--rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/dependency_links.txt
--rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/requires.txt
--rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-04 12:56:48.000000 bioplotz-0.1.0.dev2/bioplotz.egg-info/top_level.txt
--rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-04 12:56:48.296678 bioplotz-0.1.0.dev2/setup.cfg
--rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-04 11:29:58.000000 bioplotz-0.1.0.dev2/setup.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 13:09:28.973014 bioplotz-0.1.0.dev3/
+-rw-r--r--   0 zsc       (1000) users      (100)     1305 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev3/LICENSE
+-rw-r--r--   0 zsc       (1000) users      (100)       67 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev3/MANIFEST.in
+-rw-r--r--   0 zsc       (1000) users      (100)    13431 2023-05-04 13:09:28.973014 bioplotz-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)    13134 2023-05-04 13:04:17.000000 bioplotz-0.1.0.dev3/README.md
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 13:09:28.973014 bioplotz-0.1.0.dev3/bioplotz/
+-rw-r--r--   0 zsc       (1000) users      (100)      225 2023-05-04 13:08:54.000000 bioplotz-0.1.0.dev3/bioplotz/__init__.py
+-rw-r--r--   0 zsc       (1000) users      (100)    10185 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev3/bioplotz/chromosome.py
+-rw-r--r--   0 zsc       (1000) users      (100)     2477 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev3/bioplotz/genecluster.py
+-rwxr-xr-x   0 zsc       (1000) users      (100)     6110 2023-05-04 12:54:04.000000 bioplotz-0.1.0.dev3/bioplotz/manhattan.py
+-rw-r--r--   0 zsc       (1000) users      (100)     3698 2023-05-04 13:03:25.000000 bioplotz-0.1.0.dev3/bioplotz/mulitalign.py
+drwxr-xr-x   0 zsc       (1000) users      (100)        0 2023-05-04 13:09:28.973014 bioplotz-0.1.0.dev3/bioplotz.egg-info/
+-rw-r--r--   0 zsc       (1000) users      (100)    13431 2023-05-04 13:09:28.000000 bioplotz-0.1.0.dev3/bioplotz.egg-info/PKG-INFO
+-rw-r--r--   0 zsc       (1000) users      (100)      310 2023-05-04 13:09:28.000000 bioplotz-0.1.0.dev3/bioplotz.egg-info/SOURCES.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        1 2023-05-04 13:09:28.000000 bioplotz-0.1.0.dev3/bioplotz.egg-info/dependency_links.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       24 2023-05-04 13:09:28.000000 bioplotz-0.1.0.dev3/bioplotz.egg-info/requires.txt
+-rw-r--r--   0 zsc       (1000) users      (100)        9 2023-05-04 13:09:28.000000 bioplotz-0.1.0.dev3/bioplotz.egg-info/top_level.txt
+-rw-r--r--   0 zsc       (1000) users      (100)       38 2023-05-04 13:09:28.973014 bioplotz-0.1.0.dev3/setup.cfg
+-rw-r--r--   0 zsc       (1000) users      (100)      643 2023-05-04 13:08:49.000000 bioplotz-0.1.0.dev3/setup.py
```

### Comparing `bioplotz-0.1.0.dev2/LICENSE` & `bioplotz-0.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev2/PKG-INFO` & `bioplotz-0.1.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,13 +120,16 @@
 ```python
 import matplotlib as mpl
 import bioplotz as bp
 
 basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
 fig, ax = bp.multialign(data, fontproperties=basefont)
 ```
-
+or
+```python
+plt.rcParams['font.sans-serif'] = 'Courier New'
+```
 <table align="center">
 <tr>
 <td><img width=600 src="examples/multialign.png"></td>
 </tr>
 </table>
```

### Comparing `bioplotz-0.1.0.dev2/README.md` & `bioplotz-0.1.0.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,13 +110,16 @@
 ```python
 import matplotlib as mpl
 import bioplotz as bp
 
 basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
 fig, ax = bp.multialign(data, fontproperties=basefont)
 ```
-
+or
+```python
+plt.rcParams['font.sans-serif'] = 'Courier New'
+```
 <table align="center">
 <tr>
 <td><img width=600 src="examples/multialign.png"></td>
 </tr>
 </table>
```

### Comparing `bioplotz-0.1.0.dev2/bioplotz/chromosome.py` & `bioplotz-0.1.0.dev3/bioplotz/chromosome.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev2/bioplotz/genecluster.py` & `bioplotz-0.1.0.dev3/bioplotz/genecluster.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev2/bioplotz/manhattan.py` & `bioplotz-0.1.0.dev3/bioplotz/manhattan.py`

 * *Files identical despite different names*

### Comparing `bioplotz-0.1.0.dev2/bioplotz/mulitalign.py` & `bioplotz-0.1.0.dev3/bioplotz/mulitalign.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 for j in sorted(self.__data):
                     cur_set.add(self.__data[j][k])
                 if len(cur_set) > 1:
                     colors[k - sp] = self.__mismatch_color
 
             for j in range(seq_cnt):
                 gid = seq_list[j]
-                y_ticks.append(i * (seq_cnt + 2) + j + .5)
+                y_ticks.append(i * (seq_cnt + 2) + j + 1)
                 y_labels.append(gid)
                 self.__rainbow_text(0, i * (seq_cnt + 2) + j + 1, self.__data[gid][sp: ep], colors, **kwargs)
         ax.set_ylim(0, total_row_cnt)
         ax.set_xticks([])
         ax.invert_yaxis()
         ax.set_yticks(y_ticks, y_labels)
         for i in ax.spines:
```

### Comparing `bioplotz-0.1.0.dev2/bioplotz.egg-info/PKG-INFO` & `bioplotz-0.1.0.dev3/bioplotz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioplotz
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
 Summary: A python package for drawing some bioinformatic pictures.
 Home-page: https://github.com/sc-zhang/bioplotz
 Author: Shengcheng Zhang
 Author-email: zsc-zhang@foxmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,13 +120,16 @@
 ```python
 import matplotlib as mpl
 import bioplotz as bp
 
 basefont = mpl.font_manager.FontProperties(fname="/path/to/font.ttf")
 fig, ax = bp.multialign(data, fontproperties=basefont)
 ```
-
+or
+```python
+plt.rcParams['font.sans-serif'] = 'Courier New'
+```
 <table align="center">
 <tr>
 <td><img width=600 src="examples/multialign.png"></td>
 </tr>
 </table>
```

### Comparing `bioplotz-0.1.0.dev2/setup.py` & `bioplotz-0.1.0.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='bioplotz',
-    version='0.1.0.dev2',
+    version='0.1.0.dev3',
     packages=['bioplotz'],
     url='https://github.com/sc-zhang/bioplotz',
     license='',
     author='Shengcheng Zhang',
     author_email='zsc-zhang@foxmail.com',
     description='A python package for drawing some bioinformatic pictures.',
     long_description=long_description,
```

