# Comparing `tmp/PaReBrick-0.5.3.tar.gz` & `tmp/PaReBrick-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.5.3.tar", last modified: Thu May  4 17:02:40 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.4.tar", last modified: Thu May  4 17:08:53 2023, max compression
```

## Comparing `PaReBrick-0.5.3.tar` & `PaReBrick-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.302467 PaReBrick-0.5.3/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.3/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:02:40.302346 PaReBrick-0.5.3/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.300291 PaReBrick-0.5.3/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.300836 PaReBrick-0.5.3/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301243 PaReBrick-0.5.3/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.3/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301447 PaReBrick-0.5.3/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.3/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.3/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 17:00:38.000000 PaReBrick-0.5.3/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301647 PaReBrick-0.5.3/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.3/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.3/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301763 PaReBrick-0.5.3/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.302175 PaReBrick-0.5.3/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1108 2023-05-04 16:55:27.000000 PaReBrick-0.5.3/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4644 2023-05-04 17:00:27.000000 PaReBrick-0.5.3/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 16:56:40.000000 PaReBrick-0.5.3/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2390 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 17:02:40.302499 PaReBrick-0.5.3/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 17:02:11.000000 PaReBrick-0.5.3/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.422947 PaReBrick-0.5.4/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.4/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:08:53.422814 PaReBrick-0.5.4/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.418702 PaReBrick-0.5.4/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.419806 PaReBrick-0.5.4/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.420773 PaReBrick-0.5.4/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.4/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421194 PaReBrick-0.5.4/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.4/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.4/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 17:06:28.000000 PaReBrick-0.5.4/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421617 PaReBrick-0.5.4/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.4/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.4/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421761 PaReBrick-0.5.4/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.422556 PaReBrick-0.5.4/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1108 2023-05-04 16:55:27.000000 PaReBrick-0.5.4/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4644 2023-05-04 17:00:27.000000 PaReBrick-0.5.4/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 16:56:40.000000 PaReBrick-0.5.4/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2370 2023-05-04 17:07:38.000000 PaReBrick-0.5.4/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 17:08:53.422986 PaReBrick-0.5.4/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 17:08:29.000000 PaReBrick-0.5.4/setup.py
```

### Comparing `PaReBrick-0.5.3/LICENSE` & `PaReBrick-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/PKG-INFO` & `PaReBrick-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.3
+Version: 0.5.4
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.3/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5.4/PaReBrick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.3
+Version: 0.5.4
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.3/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5.4/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/README.md` & `PaReBrick-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/characters/balanced.py` & `PaReBrick-0.5.4/parebrick/characters/balanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/characters/neighbours.py` & `PaReBrick-0.5.4/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/characters/unbalanced.py` & `PaReBrick-0.5.4/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5.4/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/clustering/clustering.py` & `PaReBrick-0.5.4/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5.4/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/drawer.py` & `PaReBrick-0.5.4/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5.4/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/drawer_e_coli.py` & `PaReBrick-0.5.4/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/main.py` & `PaReBrick-0.5.4/parebrick/main.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5.4/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/tree/tree_holder.py` & `PaReBrick-0.5.4/parebrick/tree/tree_holder.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/tree_holder_draw.py` & `PaReBrick-0.5.4/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/utils/data/converters.py` & `PaReBrick-0.5.4/parebrick/utils/data/converters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/utils/data/parsers.py` & `PaReBrick-0.5.4/parebrick/utils/data/parsers.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/utils/data/stats.py` & `PaReBrick-0.5.4/parebrick/utils/data/stats.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5.4/parebrick/utils/data/unique_gene_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     # make unique blocks list
     i = 0
     flt = Unique_Filter()
     while i < len(lines):
         line = lines[i]
         if GRIMMReader.is_genome_declaration_string(line):
-            strain, chr = GRIMMReader.parse_genome_declaration_string(line).name.rsplit('.', 1)
+            strain = GRIMMReader.parse_genome_declaration_string(line).name
             strains.add(strain)
 
             data_line = lines[i + 1]
             parsed = GRIMMReader.parse_data_string(data_line)[1]
             flt.update_allowed_blocks(parsed, strain)
             i += 2
         else:
```

### Comparing `PaReBrick-0.5.3/parebrick/utils/decorators.py` & `PaReBrick-0.5.4/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.3/setup.py` & `PaReBrick-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.5.3',
+    version='0.5.4',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

