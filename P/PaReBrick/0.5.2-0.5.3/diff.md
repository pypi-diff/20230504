# Comparing `tmp/PaReBrick-0.5.2.tar.gz` & `tmp/PaReBrick-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.5.2.tar", last modified: Thu May  4 14:50:00 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.3.tar", last modified: Thu May  4 17:02:40 2023, max compression
```

## Comparing `PaReBrick-0.5.2.tar` & `PaReBrick-0.5.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972832 PaReBrick-0.5.2/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.2/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 14:50:00.972698 PaReBrick-0.5.2/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.969549 PaReBrick-0.5.2/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.970492 PaReBrick-0.5.2/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971141 PaReBrick-0.5.2/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.2/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971499 PaReBrick-0.5.2/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.2/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.2/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 14:49:36.000000 PaReBrick-0.5.2/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971929 PaReBrick-0.5.2/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.2/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.2/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972042 PaReBrick-0.5.2/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972529 PaReBrick-0.5.2/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1106 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4637 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2390 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:50:00.972866 PaReBrick-0.5.2/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.302467 PaReBrick-0.5.3/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.3/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:02:40.302346 PaReBrick-0.5.3/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.300291 PaReBrick-0.5.3/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 17:02:40.000000 PaReBrick-0.5.3/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.300836 PaReBrick-0.5.3/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301243 PaReBrick-0.5.3/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.3/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301447 PaReBrick-0.5.3/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.3/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.3/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 17:00:38.000000 PaReBrick-0.5.3/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301647 PaReBrick-0.5.3/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.3/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.3/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.301763 PaReBrick-0.5.3/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:02:40.302175 PaReBrick-0.5.3/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1108 2023-05-04 16:55:27.000000 PaReBrick-0.5.3/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4644 2023-05-04 17:00:27.000000 PaReBrick-0.5.3/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 16:56:40.000000 PaReBrick-0.5.3/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2390 2023-05-04 14:48:36.000000 PaReBrick-0.5.3/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.3/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 17:02:40.302499 PaReBrick-0.5.3/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 17:02:11.000000 PaReBrick-0.5.3/setup.py
```

### Comparing `PaReBrick-0.5.2/LICENSE` & `PaReBrick-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/PKG-INFO` & `PaReBrick-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.2
+Version: 0.5.3
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.2/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5.3/PaReBrick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.2
+Version: 0.5.3
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.2/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5.3/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/README.md` & `PaReBrick-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/characters/balanced.py` & `PaReBrick-0.5.3/parebrick/characters/balanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/characters/neighbours.py` & `PaReBrick-0.5.3/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/characters/unbalanced.py` & `PaReBrick-0.5.3/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5.3/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/clustering/clustering.py` & `PaReBrick-0.5.3/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5.3/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/drawer.py` & `PaReBrick-0.5.3/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5.3/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/drawer_e_coli.py` & `PaReBrick-0.5.3/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/main.py` & `PaReBrick-0.5.3/parebrick/main.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5.3/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/tree/tree_holder.py` & `PaReBrick-0.5.3/parebrick/tree/tree_holder.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/tree_holder_draw.py` & `PaReBrick-0.5.3/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/utils/data/converters.py` & `PaReBrick-0.5.3/parebrick/utils/data/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,9 @@
         for b in bs[1:-1]:
             block = b[1].split('#')[1]
             df_block = pd.read_csv(StringIO('\n'.join(b[2:])), sep='\t')
 
             print(f'>{block}', file=f)
             for index, row in df_block.iterrows():
                 chr_name, start, end, strand = chr_names[row['Seq_id']], row['Start'], row['End'], row['Strand']
-                print(chr_name + ':' + (f'{start}-{end}' if strand == '+' else f'{end}-{start}') + ' ' + strand, file=f)
+                print(chr_name + '.1:' + (f'{start}-{end}' if strand == '+' else f'{end}-{start}') + ' ' + strand, file=f)
             print(file=f)
```

### Comparing `PaReBrick-0.5.2/parebrick/utils/data/parsers.py` & `PaReBrick-0.5.3/parebrick/utils/data/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def genome_lengths_from_block_coords(in_file):
     with open(in_file) as f:
         head_lines = list(takewhile(lambda line: (line != BLOCKS_SEPARATOR + os.linesep) and
                                                  (line != BLOCKS_SEPARATOR + '\n'), f))
 
     # names of chromosomes
     df_head = pd.read_csv(StringIO(''.join(head_lines)), sep='\t')
-    return {row['Description']: row['Size'] for index, row in df_head.iterrows()}
+    return {row['Description'] + '.1': row['Size'] for index, row in df_head.iterrows()}
 
 def genome_genome_lengths_from_chromosomes_lengths(chr_lengths):
     lengths = defaultdict(int)
 
     for chr, len in chr_lengths.items():
         strain, _ = chr.rsplit('.', 1)
         lengths[strain] += len
```

### Comparing `PaReBrick-0.5.2/parebrick/utils/data/stats.py` & `PaReBrick-0.5.3/parebrick/utils/data/stats.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5.3/parebrick/utils/data/unique_gene_filters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/parebrick/utils/decorators.py` & `PaReBrick-0.5.3/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.2/setup.py` & `PaReBrick-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.5.2',
+    version='0.5.3',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

