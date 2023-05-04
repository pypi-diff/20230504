# Comparing `tmp/imgMS-0.2.3.tar.gz` & `tmp/imgMS-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgMS-0.2.3.tar", last modified: Thu May  4 15:45:05 2023, max compression
+gzip compressed data, was "imgMS-0.2.4.tar", last modified: Thu May  4 19:44:13 2023, max compression
```

## Comparing `imgMS-0.2.3.tar` & `imgMS-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:45:05.237044 imgMS-0.2.3/
--rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.3/LICENSE
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 15:45:05.236487 imgMS-0.2.3/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.3/README.md
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:45:05.232416 imgMS-0.2.3/imgMS/
--rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.3/imgMS/MSData.py
--rw-r--r--   0 nika       (501) staff       (20)    13472 2023-05-04 15:40:53.000000 imgMS-0.2.3/imgMS/MSEval.py
--rw-r--r--   0 nika       (501) staff       (20)     3541 2023-03-12 16:49:41.000000 imgMS-0.2.3/imgMS/MSStats.py
--rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.3/imgMS/__init__.py
--rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.3/imgMS/side_functions.py
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:45:05.235668 imgMS-0.2.3/imgMS.egg-info/
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 15:45:05.000000 imgMS-0.2.3/imgMS.egg-info/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 15:45:05.000000 imgMS-0.2.3/imgMS.egg-info/SOURCES.txt
--rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 15:45:05.000000 imgMS-0.2.3/imgMS.egg-info/dependency_links.txt
--rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 15:45:05.000000 imgMS-0.2.3/imgMS.egg-info/requires.txt
--rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 15:45:05.000000 imgMS-0.2.3/imgMS.egg-info/top_level.txt
--rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 15:45:05.237478 imgMS-0.2.3/setup.cfg
--rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 15:41:33.000000 imgMS-0.2.3/setup.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:44:13.636119 imgMS-0.2.4/
+-rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.4/LICENSE
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:44:13.635698 imgMS-0.2.4/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.4/README.md
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:44:13.632458 imgMS-0.2.4/imgMS/
+-rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.4/imgMS/MSData.py
+-rw-r--r--   0 nika       (501) staff       (20)    13407 2023-05-04 15:48:23.000000 imgMS-0.2.4/imgMS/MSEval.py
+-rw-r--r--   0 nika       (501) staff       (20)     3594 2023-05-04 15:53:03.000000 imgMS-0.2.4/imgMS/MSStats.py
+-rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.4/imgMS/__init__.py
+-rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.4/imgMS/side_functions.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:44:13.635018 imgMS-0.2.4/imgMS.egg-info/
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:44:13.000000 imgMS-0.2.4/imgMS.egg-info/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 19:44:13.000000 imgMS-0.2.4/imgMS.egg-info/SOURCES.txt
+-rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 19:44:13.000000 imgMS-0.2.4/imgMS.egg-info/dependency_links.txt
+-rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 19:44:13.000000 imgMS-0.2.4/imgMS.egg-info/requires.txt
+-rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 19:44:13.000000 imgMS-0.2.4/imgMS.egg-info/top_level.txt
+-rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 19:44:13.636266 imgMS-0.2.4/setup.cfg
+-rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 15:53:24.000000 imgMS-0.2.4/setup.py
```

### Comparing `imgMS-0.2.3/LICENSE` & `imgMS-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.3/PKG-INFO` & `imgMS-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.3
+Version: 0.2.4
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.3/README.md` & `imgMS-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.3/imgMS/MSData.py` & `imgMS-0.2.4/imgMS/MSData.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.3/imgMS/MSEval.py` & `imgMS-0.2.4/imgMS/MSEval.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,17 @@
 
         elif filetype == 'csv':
             data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter,
                                header=header, engine='python')
 
         elif filetype == 'asc':
         	try:
-            	data = pd.read_csv(filename, sep='\t', index_col=index_col, skipfooter=skipfooter, 
-            	                   header=header, engine='python')
+            	data = pd.read_csv(filename, sep='\t', index_col=index_col, skipfooter=skipfooter, header=header, engine='python')
             except:
-            	data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter,
-            	                   header=header, engine='python')
+            	data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter, header=header, engine='python')
                                
             data = data.drop(data.index[:drop], axis=0)
             data.dropna(axis=1, how='all', inplace=True)
             data = data.apply(pd.to_numeric, errors='coerce')
 
         else:
             warnings.warn('File type not supported.')
```

### Comparing `imgMS-0.2.3/imgMS/MSStats.py` & `imgMS-0.2.4/imgMS/MSStats.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,18 @@
         p = Path(verts)
         ind = p.contains_points(self.pix, radius=1)
         alpha = self.updateArray(self.array, ind)
         self.im.set_alpha(alpha)
         self.fig.canvas.draw_idle()
         self.stats(self.array, ind)
 
-    def __call__(self, vmax=None):
-        self.fig, self.ax = plt.subplots()
+    def __call__(self, ax=None, vmax=None):
+    	self.ax = ax
+    	if self.ax == None:
+        	self.fig, self.ax = plt.subplots()
 
         self.im = self.ax.imshow(self.array, vmax=vmax)
         self.ax.set_xlim([0, self.shape[1]])
         self.ax.set_ylim([0, self.shape[0]])
 
         lsso = LassoSelector(ax=self.ax, onselect=self.onSelect)
```

### Comparing `imgMS-0.2.3/imgMS/side_functions.py` & `imgMS-0.2.4/imgMS/side_functions.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.3/imgMS.egg-info/PKG-INFO` & `imgMS-0.2.4/imgMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.3
+Version: 0.2.4
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.3/setup.py` & `imgMS-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='imgMS',
-    version='0.2.3',
+    version='0.2.4',
     author='nikadilli',
     author_email='nikadilli@gmail.com',
     url="https://github.com/nikadilli/imgMS",
     packages=setuptools.find_packages(),
     scripts=[],
     license='LICENSE.txt',
     description='Package for data reduction of LA-ICP-MS data.',
```

