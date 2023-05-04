# Comparing `tmp/PaReBrick-0.4.tar.gz` & `tmp/PaReBrick-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.4.tar", last modified: Thu Mar  9 14:25:24 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.tar", last modified: Thu May  4 14:15:37 2023, max compression
```

## Comparing `PaReBrick-0.4.tar` & `PaReBrick-0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.942960 PaReBrick-0.4/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.4/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-03-09 14:25:24.942835 PaReBrick-0.4/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.940711 PaReBrick-0.4/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-03-09 14:25:24.000000 PaReBrick-0.4/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     3927 2023-03-09 14:20:36.000000 PaReBrick-0.4/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.941285 PaReBrick-0.4/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.941721 PaReBrick-0.4/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6184 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2021-07-05 10:42:17.000000 PaReBrick-0.4/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.941930 PaReBrick-0.4/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.4/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.4/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.4/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.4/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.4/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    20445 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.942141 PaReBrick-0.4/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.4/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7385 2023-03-09 14:22:38.000000 PaReBrick-0.4/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.4/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.942254 PaReBrick-0.4/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-03-09 14:25:24.942670 PaReBrick-0.4/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1106 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4675 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3960 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2390 2021-10-18 18:47:22.000000 PaReBrick-0.4/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.4/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-03-09 14:25:24.942998 PaReBrick-0.4/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1900 2023-03-09 14:22:38.000000 PaReBrick-0.4/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.408993 PaReBrick-0.5/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-05-04 14:15:37.408792 PaReBrick-0.5/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.404100 PaReBrick-0.5/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     4807 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 14:15:37.000000 PaReBrick-0.5/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     3927 2023-03-09 14:20:36.000000 PaReBrick-0.5/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.405373 PaReBrick-0.5/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.406273 PaReBrick-0.5/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6184 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.406726 PaReBrick-0.5/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    20480 2023-05-04 14:06:48.000000 PaReBrick-0.5/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.407132 PaReBrick-0.5/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:13:19.000000 PaReBrick-0.5/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.407371 PaReBrick-0.5/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 14:15:37.408429 PaReBrick-0.5/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1106 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4657 2023-05-04 14:02:30.000000 PaReBrick-0.5/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-03-09 16:51:12.000000 PaReBrick-0.5/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2390 2021-10-18 18:47:22.000000 PaReBrick-0.5/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 14:15:37.409034 PaReBrick-0.5/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1900 2023-05-04 14:15:29.000000 PaReBrick-0.5/setup.py
```

### Comparing `PaReBrick-0.4/LICENSE` & `PaReBrick-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/PKG-INFO` & `PaReBrick-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.4
+Version: 0.5
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.4/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5/PaReBrick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.4
+Version: 0.5
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.4/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/README.md` & `PaReBrick-0.5/README.md`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/characters/balanced.py` & `PaReBrick-0.5/parebrick/characters/balanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/characters/neighbours.py` & `PaReBrick-0.5/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/characters/unbalanced.py` & `PaReBrick-0.5/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/clustering/clustering.py` & `PaReBrick-0.5/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/drawer.py` & `PaReBrick-0.5/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/drawer_e_coli.py` & `PaReBrick-0.5/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/main.py` & `PaReBrick-0.5/parebrick/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,17 +410,18 @@
         balanced_rearrangements_stats()
         balanced_rearrangements_output()
 
     unbalanced_rearrangements_characters()
     unbalanced_rearrangements_stats_and_clustering()
     if len(ub_stats) != 0: unbalanced_rearrangements_output()
 
-    which_chromosome_characters()
-    which_chromosome_stats_and_clustering()
-    which_chromosome_output()
+    if which_chr_flag:
+        which_chromosome_characters()
+        which_chromosome_stats_and_clustering()
+        which_chromosome_output()
 
     if visualize_neighbours:
         neighbours_output()
 
     logger.info(f'Total elapsed time: {time() - start_time} seconds')
```

### Comparing `PaReBrick-0.4/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/tree/tree_holder.py` & `PaReBrick-0.5/parebrick/tree/tree_holder.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from itertools import combinations
 
 from parebrick.tree.neighbours_utils import generate_neighbour_face, align_neighbours, get_offsets
 
 
 class TreeHolder:
     def __init__(self, tree, logger, scale=None, labels_dict=None, node_colors=defaultdict(lambda: 'black'),
-                 reroot=True):
+                 reroot=True, hz_line_width=1, vt_line_width=1):
         self.tree = Tree(tree)
         self.scale = scale
 
         if reroot:
             r = self.tree.get_midpoint_outgroup()
             self.tree.set_outgroup(r)
 
@@ -22,14 +22,16 @@
                 logger.info(f'Children of root: {node.children}')
                 self.tree.set_outgroup(node.children[0])
             break
 
         for node in self.tree.traverse():
             # Hide node circles
             node.img_style['size'] = 0
+            node.img_style['hz_line_width'] = hz_line_width
+            node.img_style['vt_line_width'] = vt_line_width
 
             if node.is_leaf():
                 try:
                     name_face = TextFace(labels_dict[node.name] if labels_dict else node.name,
                                          fgcolor=node_colors[node.name])
                 except KeyError:
                     msg = f'There is not label for leaf {node.name} in labels file'
@@ -133,15 +135,15 @@
             for child in v.children:
                 if v.color != child.color and not (not count_second_color and (v.color == 2) or (child.color == 2)):
                     innovations[child.color].append(child)
                     insertions_deltitions[child.color - v.color].append(child)
                 count_innovations(child, innovations, self.insertions_deltitions)
 
         color_counter = Counter(leaf_colors.values())
-        print(color_counter)
+        # print(color_counter)
 
         # get colorsets for internal nodes
         root = self.tree.get_tree_root()
         assign_colorset_feature(root)
 
         # get color for internal nodes
         root_color = chose_color(root.colorset)
```

### Comparing `PaReBrick-0.4/parebrick/tree_holder_draw.py` & `PaReBrick-0.5/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/utils/data/converters.py` & `PaReBrick-0.5/parebrick/utils/data/converters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/utils/data/parsers.py` & `PaReBrick-0.5/parebrick/utils/data/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     genomes, blocks = set(), set()
 
     with open(grimm_file) as f:
         ls = f.readlines()
     block_genome_count = defaultdict(Counter)
 
     for i in range(0, len(ls), 2):
-        name = GRIMMReader.parse_genome_declaration_string(ls[i]).name.rsplit('.', 1)[0]
+        name = GRIMMReader.parse_genome_declaration_string(ls[i]).name
         data = GRIMMReader.parse_data_string(ls[i + 1])[1]
         genomes.add(name)
         for _, block in data:
             blocks.add(int(block))
             block_genome_count[int(block)][name] += 1
 
     return list(sorted(genomes)), list(sorted(blocks)), block_genome_count
```

### Comparing `PaReBrick-0.4/parebrick/utils/data/stats.py` & `PaReBrick-0.5/parebrick/utils/data/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
     logger.info(f'Strains in blocks file count: {len(block_genomes)}')
     logger.info(f'Strains in tree leafs count: {len(tree_genomes)}')
     logger.info(f'Intersected strains count: {len(block_genomes & tree_genomes)}')
 
     if not len(block_genomes & tree_genomes) == len(tree_genomes) == len(block_genomes):
         if len(block_genomes & tree_genomes) == 0:
-            logger.error('Tree genomes: {tree_genomes}')
-            logger.error('Blocks genomes: {block_genomes}')
+            logger.error(f'Tree genomes: {tree_genomes}')
+            logger.error(f'Blocks genomes: {block_genomes}')
             logger.error('Seems like strains in block files and in tree leafs have different ids, intersection is empty.')
             raise ValueError(
                 'Seems like strains in block files and in tree leafs have different ids, intersection is empty.')
         left_tree = tree_genomes - (block_genomes & tree_genomes)
         if len(left_tree) > 0:
             logger.warning('PRUNING TREE')
             logger.warning(f'Those strains are thrown away from tree because there were not found in blocks data: {", ".join(left_tree)}')
```

### Comparing `PaReBrick-0.4/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5/parebrick/utils/data/unique_gene_filters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/parebrick/utils/decorators.py` & `PaReBrick-0.5/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.4/setup.py` & `PaReBrick-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.4',
+    version='0.5',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

