# Comparing `tmp/PaReBrick-0.5.tar.gz` & `tmp/PaReBrick-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.5.tar", last modified: Thu May  4 14:15:37 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.1.tar", last modified: Thu May  4 14:38:25 2023, max compression
```

## Comparing `PaReBrick-0.5.tar` & `PaReBrick-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.408993 PaReBrick-0.5/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-05-04 14:15:37.408792 PaReBrick-0.5/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.404100 PaReBrick-0.5/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     3927 2023-03-09 14:20:36.000000 PaReBrick-0.5/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.405373 PaReBrick-0.5/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.406273 PaReBrick-0.5/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6184 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.406726 PaReBrick-0.5/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    20480 2023-05-04 14:06:48.000000 PaReBrick-0.5/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.407132 PaReBrick-0.5/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:13:19.000000 PaReBrick-0.5/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.407371 PaReBrick-0.5/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.408429 PaReBrick-0.5/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1106 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4657 2023-05-04 14:02:30.000000 PaReBrick-0.5/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-03-09 16:51:12.000000 PaReBrick-0.5/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2390 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:15:37.409034 PaReBrick-0.5/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1900 2023-05-04 14:15:29.000000 PaReBrick-0.5/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.735423 PaReBrick-0.5.1/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.1/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     4833 2023-05-04 14:38:25.735278 PaReBrick-0.5.1/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.730896 PaReBrick-0.5.1/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     4833 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     3951 2023-05-04 14:22:55.000000 PaReBrick-0.5.1/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.732248 PaReBrick-0.5.1/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.733250 PaReBrick-0.5.1/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6184 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.1/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.733762 PaReBrick-0.5.1/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.1/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.1/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    20480 2023-05-04 14:36:28.000000 PaReBrick-0.5.1/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.734112 PaReBrick-0.5.1/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.1/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:13:19.000000 PaReBrick-0.5.1/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.1/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.734340 PaReBrick-0.5.1/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.735048 PaReBrick-0.5.1/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1106 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4637 2023-05-04 14:35:41.000000 PaReBrick-0.5.1/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-03-09 16:51:12.000000 PaReBrick-0.5.1/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2390 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:38:25.735461 PaReBrick-0.5.1/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 14:36:44.000000 PaReBrick-0.5.1/setup.py
```

### Comparing `PaReBrick-0.5/LICENSE` & `PaReBrick-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/PKG-INFO` & `PaReBrick-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5
+Version: 0.5.1
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
@@ -92,19 +92,19 @@
 1. Clone all repository with data:
 ```bash
 git clone https://github.com/ctlab/parallel-rearrangements
 ```
 
 2. Change directory to data folder:
 ```bash
-cd parallel-rearrangements/example-data/streptococcus_pyogenes/input
+cd parallel-rearrangements/example-data/streptococcus_pyogenes
 ```
 
 3. (a) Running tool on example input:
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output -l labels.csv
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
```

### Comparing `PaReBrick-0.5/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5.1/PaReBrick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5
+Version: 0.5.1
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
@@ -92,19 +92,19 @@
 1. Clone all repository with data:
 ```bash
 git clone https://github.com/ctlab/parallel-rearrangements
 ```
 
 2. Change directory to data folder:
 ```bash
-cd parallel-rearrangements/example-data/streptococcus_pyogenes/input
+cd parallel-rearrangements/example-data/streptococcus_pyogenes
 ```
 
 3. (a) Running tool on example input:
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output -l labels.csv
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
```

### Comparing `PaReBrick-0.5/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5.1/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/README.md` & `PaReBrick-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,19 @@
 1. Clone all repository with data:
 ```bash
 git clone https://github.com/ctlab/parallel-rearrangements
 ```
 
 2. Change directory to data folder:
 ```bash
-cd parallel-rearrangements/example-data/streptococcus_pyogenes/input
+cd parallel-rearrangements/example-data/streptococcus_pyogenes
 ```
 
 3. (a) Running tool on example input:
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output -l labels.csv
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
-PaReBrick -t tree.nwk -b maf2synteny-output
+PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
```

### Comparing `PaReBrick-0.5/parebrick/characters/balanced.py` & `PaReBrick-0.5.1/parebrick/characters/balanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/characters/neighbours.py` & `PaReBrick-0.5.1/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/characters/unbalanced.py` & `PaReBrick-0.5.1/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5.1/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/clustering/clustering.py` & `PaReBrick-0.5.1/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5.1/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/drawer.py` & `PaReBrick-0.5.1/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5.1/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/drawer_e_coli.py` & `PaReBrick-0.5.1/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/main.py` & `PaReBrick-0.5.1/parebrick/main.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5.1/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/tree/tree_holder.py` & `PaReBrick-0.5.1/parebrick/tree/tree_holder.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/tree_holder_draw.py` & `PaReBrick-0.5.1/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/utils/data/converters.py` & `PaReBrick-0.5.1/parebrick/utils/data/converters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/utils/data/parsers.py` & `PaReBrick-0.5.1/parebrick/utils/data/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     block_neighbours = defaultdict(lambda: defaultdict(list))
     with open(grimm_file) as f: ls = f.readlines()
 
     i = 0
     while i < len(ls):
         l = ls[i]
         if GRIMMReader.is_genome_declaration_string(l):
-            strain, chr = GRIMMReader.parse_genome_declaration_string(l).name.rsplit('.', 1)
+            strain = GRIMMReader.parse_genome_declaration_string(l).name
             data_line = ls[i + 1]
             bs = GRIMMReader.parse_data_string(data_line)[1]
 
             n = len(bs)
             j = 0
 
             while j < n:
```

### Comparing `PaReBrick-0.5/parebrick/utils/data/stats.py` & `PaReBrick-0.5.1/parebrick/utils/data/stats.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5.1/parebrick/utils/data/unique_gene_filters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/parebrick/utils/decorators.py` & `PaReBrick-0.5.1/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5/setup.py` & `PaReBrick-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.5',
+    version='0.5.1',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

