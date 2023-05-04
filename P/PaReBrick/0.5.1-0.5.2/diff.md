# Comparing `tmp/PaReBrick-0.5.1.tar.gz` & `tmp/PaReBrick-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.5.1.tar", last modified: Thu May  4 14:38:25 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.2.tar", last modified: Thu May  4 14:50:00 2023, max compression
```

## Comparing `PaReBrick-0.5.1.tar` & `PaReBrick-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.735423 PaReBrick-0.5.1/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.1/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     4833 2023-05-04 14:38:25.735278 PaReBrick-0.5.1/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.730896 PaReBrick-0.5.1/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     4833 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:38:25.000000 PaReBrick-0.5.1/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     3951 2023-05-04 14:22:55.000000 PaReBrick-0.5.1/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.732248 PaReBrick-0.5.1/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.733250 PaReBrick-0.5.1/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6184 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.1/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.733762 PaReBrick-0.5.1/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.1/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.1/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    20480 2023-05-04 14:36:28.000000 PaReBrick-0.5.1/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.734112 PaReBrick-0.5.1/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.1/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:13:19.000000 PaReBrick-0.5.1/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.1/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.734340 PaReBrick-0.5.1/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:38:25.735048 PaReBrick-0.5.1/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1106 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4637 2023-05-04 14:35:41.000000 PaReBrick-0.5.1/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-03-09 16:51:12.000000 PaReBrick-0.5.1/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2390 2021-10-18 18:47:22.000000 PaReBrick-0.5.1/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.1/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:38:25.735461 PaReBrick-0.5.1/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 14:36:44.000000 PaReBrick-0.5.1/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972832 PaReBrick-0.5.2/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.2/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 14:50:00.972698 PaReBrick-0.5.2/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.969549 PaReBrick-0.5.2/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:50:00.000000 PaReBrick-0.5.2/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.970492 PaReBrick-0.5.2/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971141 PaReBrick-0.5.2/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.2/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971499 PaReBrick-0.5.2/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.2/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.2/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 14:49:36.000000 PaReBrick-0.5.2/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.971929 PaReBrick-0.5.2/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.2/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.2/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972042 PaReBrick-0.5.2/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:50:00.972529 PaReBrick-0.5.2/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1106 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4637 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2390 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.2/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:50:00.972866 PaReBrick-0.5.2/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 14:48:36.000000 PaReBrick-0.5.2/setup.py
```

### Comparing `PaReBrick-0.5.1/LICENSE` & `PaReBrick-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/PKG-INFO` & `PaReBrick-0.5.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.1
+Version: 0.5.2
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
@@ -19,27 +19,30 @@
 License-File: LICENSE
 
 # PaReBrick: PArallel REarrangements and BReakpoints identification toolkit
 
 ---
 ## Motivation
 High plasticity of bacterial genomes is provided by numerous mechanisms including horizontal gene transfer and recombination via numerous flanking repeats. 
-Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation. 
-Specifically, such rearrangements might be responsible for multi-virulence, antibiotic resistance, and antigenic variation. 
+Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation or phenotypic diversity. 
+Specifically, such rearrangements might be responsible for virulence, antibiotic resistance, and antigenic variation. 
 However, identification of such events requires laborious manual inspection and verification of phyletic pattern consistency.
 
 ## Methods and Results
 
 ![Pipeline of tool](figs/pipeline.svg)
 
 We present **tool `PaReBrick`** — implementation of an algorithmic solution for the identification of parallel rearrangements in bacterial population.
 We define the term "parallel rearrangements" as events that occur independently in phylogenetically distant bacterial strains and present a formalization of the problem of parallel rearrangements calling.
 
-The tool takes synteny blocks and a phylogenetic tree as input and outputs rearrangement events. 
-The tool tests each rearrangement for consistency with a tree, and sorts the events by their parallelism score and provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+The tool takes a collection of strains represented as a sequence of oriented synteny blocks and a phylogenetic tree as input data. 
+It identifies rearrangements, tests them for consistency with a tree, and sorts the events by their parallelism score. 
+The tool provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+
+We [demonstrated](https://doi.org/10.1093/bioinformatics/btab691) PaReBrick’s efficiency and accuracy and showed its potential to detect genome rearrangements responsible for pathogenicity and adaptation in bacterial genomes.
 
 ## Installation 
 
 PaReBrick can be installed with `pip`:
 
 ```bash
 pip install PaReBrick
@@ -104,7 +107,13 @@
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
+
+## Citation
+
+If you use `PaReBrick` in your research, please cite:
+
+Alexey Zabelkin, Yulia Yakovleva, Olga Bochkareva, Nikita Alexeev, PaReBrick: PArallel REarrangements and BReaks identification toolkit, Bioinformatics, 2021; btab691, https://doi.org/10.1093/bioinformatics/btab691
```

### Comparing `PaReBrick-0.5.1/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5.2/PaReBrick.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.1
+Version: 0.5.2
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
@@ -19,27 +19,30 @@
 License-File: LICENSE
 
 # PaReBrick: PArallel REarrangements and BReakpoints identification toolkit
 
 ---
 ## Motivation
 High plasticity of bacterial genomes is provided by numerous mechanisms including horizontal gene transfer and recombination via numerous flanking repeats. 
-Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation. 
-Specifically, such rearrangements might be responsible for multi-virulence, antibiotic resistance, and antigenic variation. 
+Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation or phenotypic diversity. 
+Specifically, such rearrangements might be responsible for virulence, antibiotic resistance, and antigenic variation. 
 However, identification of such events requires laborious manual inspection and verification of phyletic pattern consistency.
 
 ## Methods and Results
 
 ![Pipeline of tool](figs/pipeline.svg)
 
 We present **tool `PaReBrick`** — implementation of an algorithmic solution for the identification of parallel rearrangements in bacterial population.
 We define the term "parallel rearrangements" as events that occur independently in phylogenetically distant bacterial strains and present a formalization of the problem of parallel rearrangements calling.
 
-The tool takes synteny blocks and a phylogenetic tree as input and outputs rearrangement events. 
-The tool tests each rearrangement for consistency with a tree, and sorts the events by their parallelism score and provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+The tool takes a collection of strains represented as a sequence of oriented synteny blocks and a phylogenetic tree as input data. 
+It identifies rearrangements, tests them for consistency with a tree, and sorts the events by their parallelism score. 
+The tool provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+
+We [demonstrated](https://doi.org/10.1093/bioinformatics/btab691) PaReBrick’s efficiency and accuracy and showed its potential to detect genome rearrangements responsible for pathogenicity and adaptation in bacterial genomes.
 
 ## Installation 
 
 PaReBrick can be installed with `pip`:
 
 ```bash
 pip install PaReBrick
@@ -104,7 +107,13 @@
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
+
+## Citation
+
+If you use `PaReBrick` in your research, please cite:
+
+Alexey Zabelkin, Yulia Yakovleva, Olga Bochkareva, Nikita Alexeev, PaReBrick: PArallel REarrangements and BReaks identification toolkit, Bioinformatics, 2021; btab691, https://doi.org/10.1093/bioinformatics/btab691
```

### Comparing `PaReBrick-0.5.1/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5.2/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/README.md` & `PaReBrick-0.5.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # PaReBrick: PArallel REarrangements and BReakpoints identification toolkit
 
 ---
 ## Motivation
 High plasticity of bacterial genomes is provided by numerous mechanisms including horizontal gene transfer and recombination via numerous flanking repeats. 
-Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation. 
-Specifically, such rearrangements might be responsible for multi-virulence, antibiotic resistance, and antigenic variation. 
+Genome rearrangements such as inversions, deletions, insertions, and duplications may independently occur in different strains, providing parallel adaptation or phenotypic diversity. 
+Specifically, such rearrangements might be responsible for virulence, antibiotic resistance, and antigenic variation. 
 However, identification of such events requires laborious manual inspection and verification of phyletic pattern consistency.
 
 ## Methods and Results
 
 ![Pipeline of tool](figs/pipeline.svg)
 
 We present **tool `PaReBrick`** — implementation of an algorithmic solution for the identification of parallel rearrangements in bacterial population.
 We define the term "parallel rearrangements" as events that occur independently in phylogenetically distant bacterial strains and present a formalization of the problem of parallel rearrangements calling.
 
-The tool takes synteny blocks and a phylogenetic tree as input and outputs rearrangement events. 
-The tool tests each rearrangement for consistency with a tree, and sorts the events by their parallelism score and provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+The tool takes a collection of strains represented as a sequence of oriented synteny blocks and a phylogenetic tree as input data. 
+It identifies rearrangements, tests them for consistency with a tree, and sorts the events by their parallelism score. 
+The tool provides diagrams of the neighbors for each block of interest, allowing the detection of horizontally transferred blocks or their extra copies and the inversions in which copied blocks are involved.
+
+We [demonstrated](https://doi.org/10.1093/bioinformatics/btab691) PaReBrick’s efficiency and accuracy and showed its potential to detect genome rearrangements responsible for pathogenicity and adaptation in bacterial genomes.
 
 ## Installation 
 
 PaReBrick can be installed with `pip`:
 
 ```bash
 pip install PaReBrick
@@ -84,7 +87,13 @@
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output -l input/labels.csv
 ```
 
 3. (b) Or with minimal required arguments (no labels):
 ```
 PaReBrick -t input/tree.nwk -b input/maf2synteny-output
 ```
+
+## Citation
+
+If you use `PaReBrick` in your research, please cite:
+
+Alexey Zabelkin, Yulia Yakovleva, Olga Bochkareva, Nikita Alexeev, PaReBrick: PArallel REarrangements and BReaks identification toolkit, Bioinformatics, 2021; btab691, https://doi.org/10.1093/bioinformatics/btab691
```

### Comparing `PaReBrick-0.5.1/parebrick/characters/balanced.py` & `PaReBrick-0.5.2/parebrick/characters/balanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             v1, v2 = edge.vertex1.name, edge.vertex2.name
             if v1 > v2: v1, v2 = v2, v1
 
             genome_colors, neighbour_edges = get_character_by_edge(component_bg, edge, genomes, neighbour_index)
             if white_proportion(genome_colors.values()) < 0.5: continue
 
             labels = ['adjacency exists', 'complex break of adjacency', 'some block is not presented'] + \
-                     [f'inversion between {v1}-{v2} and {v1n}-{v2n}' for (v1n, v2n) in neighbour_edges]
+                     [f'inversion with {v1n}-{v2n}' for (v1n, v2n) in neighbour_edges]
 
             characters.append((v1, v2, genome_colors, labels))
 
     return characters
 
 def get_characters_stats_balanced(characters, tree_holder, distance_between_blocks):
     ans = []
```

### Comparing `PaReBrick-0.5.1/parebrick/characters/neighbours.py` & `PaReBrick-0.5.2/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/characters/unbalanced.py` & `PaReBrick-0.5.2/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5.2/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/clustering/clustering.py` & `PaReBrick-0.5.2/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5.2/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/drawer.py` & `PaReBrick-0.5.2/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5.2/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/drawer_e_coli.py` & `PaReBrick-0.5.2/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/main.py` & `PaReBrick-0.5.2/parebrick/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,24 @@
     if v.lower() in ('yes', 'true', 't', 'y', '1'):
         return True
     elif v.lower() in ('no', 'false', 'f', 'n', '0'):
         return False
     else:
         raise argparse.ArgumentTypeError('Boolean value expected.')
 
+def restricted_float(x):
+    try:
+        x = float(x)
+    except ValueError:
+        raise argparse.ArgumentTypeError("%r not a floating-point literal" % (x,))
+
+    if x < 0.0 or x > 1.0:
+        raise argparse.ArgumentTypeError("%r not in range [0.0, 1.0]"%(x,))
+    return x
+
 
 # argument parsing
 def initialize():
     global parser, GRIMM_FILENAME, UNIQUE_GRIMM_FILENAME, BLOCKS_COORD_FILENAME, INFERCARS_FILENAME, STATS_FILE, \
         BALANCED_FOLDER, UNBALANCED_FOLDER, CHARACTERS_FOLDER, TREES_FOLDER, BALANCED_COLORS, UNBALANCED_COLORS, \
         clustering_proximity_percentile, clustering_threshold, clustering_j, clustering_j, clustering_b, \
         CSV_BLOCK_FILENAME, CSV_BLOCK_UNIQUE_FILENAME, CSV_GENOME_LENGTH, have_unique, NEIGHBOURS_FOLDER, \
@@ -87,21 +97,28 @@
     optional.add_argument('--filter_for_balanced', '-fb', type=float, default=80,
                           help='Minimal percentage of block occurrences in genomes for balanced rearrangements. '
                                'All blocks with lower occurrences rate will be removed. Default: 80.')
 
     optional.add_argument('--visualize_neighbours', '-vn', type=str2bool, default=True,
                           help='Use module for visualizing neighbours. Default: True.')
 
+
     optional.add_argument('--which_chr', '-chr', type=str2bool, default=False,
                           help='Use information about in which chromosome block is located. Default: False.')
 
+    optional.add_argument('--clustering_tree_patterns_coef', '-j', type=restricted_float, metavar='[0-1]', default=0.8,
+                          help='Coefficient (0-1) of weight of tree patterns similarity in clustering in unbalanced (copy number variation) module.'
+                               'Rest of weight will be used in distance between blocks.'
+                               'E.g. if set to 0.8 (default) distance between blocks coefficient will be set to 0.2.')
+
+    optional.add_argument('--clustering_threshold', '-c', type=restricted_float, metavar='[0-1]', default=0.025,
+                          help='Threshold for algorithm of clustering, default is 0.025.'
+                               'Can be increased for getting larger clusters or decreased for getting smaller and more grouped clusters.')
+
     clustering_proximity_percentile = 25
-    clustering_threshold = 0.025
-    clustering_j = 0.8
-    clustering_b = 0.2
 
     GRIMM_FILENAME = 'genomes_permutations.txt'
     UNIQUE_GRIMM_FILENAME = 'genomes_permutations_unique.txt'
 
     BLOCKS_COORD_FILENAME = 'blocks_coords.txt'
     INFERCARS_FILENAME = 'blocks_coords.infercars'
     INFERCARS_UNIQUE_FILENAME = 'blocks_unique_coords.infercars'
@@ -377,23 +394,25 @@
         logging.basicConfig(
             level=logging.DEBUG,
             format='[%(asctime)s] %(levelname)s - %(message)s',
             handlers=handlers
         )
 
     global blocks_folder, output_folder, tree_file, labels_file, preprocessed_data_folder, show_branch_support, \
-        have_unique, keep_consistent, balanced_block_rate
+        have_unique, keep_consistent, balanced_block_rate, clustering_threshold, clustering_j, clustering_b
     initialize()
 
     start_time = time()
     d = vars(parser.parse_args())
     blocks_folder, output_folder, tree_file, labels_file, show_branch_support, keep_consistent, balanced_block_rate, \
-    visualize_neighbours, which_chr_flag = d['blocks_folder'], d['output'], d['tree'], d['labels'], \
-                                           d['show_branch_support'], d['keep_non_parallel'], \
-                                           d['filter_for_balanced'], d['visualize_neighbours'], d['which_chr']
+    visualize_neighbours, clustering_j, clustering_threshold, which_chr_flag = d['blocks_folder'], d['output'], \
+           d['tree'], d['labels'], d['show_branch_support'], d['keep_non_parallel'], d['filter_for_balanced'], \
+           d['visualize_neighbours'], d['clustering_tree_patterns_coef'], d['clustering_threshold'], d['which_chr']
+
+    clustering_b = 1 - clustering_j
 
     # folders
     if blocks_folder[-1] != '/': blocks_folder += '/'
     if output_folder[-1] != '/': output_folder += '/'
     shutil.rmtree(output_folder, ignore_errors=True)
     print('Cleaning output folder')
```

### Comparing `PaReBrick-0.5.1/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5.2/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/tree/tree_holder.py` & `PaReBrick-0.5.2/parebrick/tree/tree_holder.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/tree_holder_draw.py` & `PaReBrick-0.5.2/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/utils/data/converters.py` & `PaReBrick-0.5.2/parebrick/utils/data/converters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/utils/data/parsers.py` & `PaReBrick-0.5.2/parebrick/utils/data/parsers.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/utils/data/stats.py` & `PaReBrick-0.5.2/parebrick/utils/data/stats.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5.2/parebrick/utils/data/unique_gene_filters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/parebrick/utils/decorators.py` & `PaReBrick-0.5.2/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.1/setup.py` & `PaReBrick-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.5.1',
+    version='0.5.2',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

