# Comparing `tmp/PaReBrick-0.5.4.tar.gz` & `tmp/PaReBrick-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PaReBrick-0.5.4.tar", last modified: Thu May  4 17:08:53 2023, max compression
+gzip compressed data, was "PaReBrick-0.5.5.tar", last modified: Thu May  4 18:00:54 2023, max compression
```

## Comparing `PaReBrick-0.5.4.tar` & `PaReBrick-0.5.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.422947 PaReBrick-0.5.4/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.4/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:08:53.422814 PaReBrick-0.5.4/PKG-INFO
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.418702 PaReBrick-0.5.4/PaReBrick.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 17:08:53.000000 PaReBrick-0.5.4/PaReBrick.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.419806 PaReBrick-0.5.4/parebrick/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.420773 PaReBrick-0.5.4/parebrick/characters/
--rw-r--r--   0 alexey     (501) staff       (20)     6167 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/balanced.py
--rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.4/parebrick/characters/neighbours.py
--rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/unbalanced.py
--rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/characters/which_chromosome.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421194 PaReBrick-0.5.4/parebrick/clustering/
--rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/clustering/clustering.py
--rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/clustering/distance_matrices.py
--rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/drawer.py
--rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.4/parebrick/drawer_b_mallei.py
--rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.4/parebrick/drawer_e_coli.py
--rw-r--r--   0 alexey     (501) staff       (20)    21624 2023-05-04 17:06:28.000000 PaReBrick-0.5.4/parebrick/main.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421617 PaReBrick-0.5.4/parebrick/tree/
--rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.4/parebrick/tree/neighbours_utils.py
--rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.4/parebrick/tree/tree_holder.py
--rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.4/parebrick/tree_holder_draw.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.421761 PaReBrick-0.5.4/parebrick/utils/
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 17:08:53.422556 PaReBrick-0.5.4/parebrick/utils/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1108 2023-05-04 16:55:27.000000 PaReBrick-0.5.4/parebrick/utils/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)     4644 2023-05-04 17:00:27.000000 PaReBrick-0.5.4/parebrick/utils/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 16:56:40.000000 PaReBrick-0.5.4/parebrick/utils/data/stats.py
--rw-r--r--   0 alexey     (501) staff       (20)     2370 2023-05-04 17:07:38.000000 PaReBrick-0.5.4/parebrick/utils/data/unique_gene_filters.py
--rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.4/parebrick/utils/decorators.py
--rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 17:08:53.422986 PaReBrick-0.5.4/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 17:08:29.000000 PaReBrick-0.5.4/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.528263 PaReBrick-0.5.5/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 PaReBrick-0.5.5/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 18:00:54.528129 PaReBrick-0.5.5/PKG-INFO
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.523731 PaReBrick-0.5.5/PaReBrick.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     5413 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      807 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)      164 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       43 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       10 2023-05-04 18:00:54.000000 PaReBrick-0.5.5/PaReBrick.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)     4531 2023-05-04 14:48:36.000000 PaReBrick-0.5.5/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.524936 PaReBrick-0.5.5/parebrick/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.525904 PaReBrick-0.5.5/parebrick/characters/
+-rw-r--r--   0 alexey     (501) staff       (20)     6079 2023-05-04 17:59:23.000000 PaReBrick-0.5.5/parebrick/characters/balanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)      706 2023-05-04 14:37:34.000000 PaReBrick-0.5.5/parebrick/characters/neighbours.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3704 2023-05-04 14:48:36.000000 PaReBrick-0.5.5/parebrick/characters/unbalanced.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3042 2023-05-04 14:48:36.000000 PaReBrick-0.5.5/parebrick/characters/which_chromosome.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.526356 PaReBrick-0.5.5/parebrick/clustering/
+-rw-r--r--   0 alexey     (501) staff       (20)     1501 2021-07-05 10:42:17.000000 PaReBrick-0.5.5/parebrick/clustering/clustering.py
+-rw-r--r--   0 alexey     (501) staff       (20)      952 2021-07-05 10:42:17.000000 PaReBrick-0.5.5/parebrick/clustering/distance_matrices.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7205 2021-07-05 10:42:17.000000 PaReBrick-0.5.5/parebrick/drawer.py
+-rw-r--r--   0 alexey     (501) staff       (20)     8449 2022-04-21 14:36:29.000000 PaReBrick-0.5.5/parebrick/drawer_b_mallei.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4680 2022-03-30 18:36:37.000000 PaReBrick-0.5.5/parebrick/drawer_e_coli.py
+-rw-r--r--   0 alexey     (501) staff       (20)    21627 2023-05-04 17:21:07.000000 PaReBrick-0.5.5/parebrick/main.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.526795 PaReBrick-0.5.5/parebrick/tree/
+-rw-r--r--   0 alexey     (501) staff       (20)     4452 2021-07-29 14:31:05.000000 PaReBrick-0.5.5/parebrick/tree/neighbours_utils.py
+-rw-r--r--   0 alexey     (501) staff       (20)     7541 2023-05-04 14:48:36.000000 PaReBrick-0.5.5/parebrick/tree/tree_holder.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2015 2021-08-20 11:14:40.000000 PaReBrick-0.5.5/parebrick/tree_holder_draw.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.526990 PaReBrick-0.5.5/parebrick/utils/
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 18:00:54.527847 PaReBrick-0.5.5/parebrick/utils/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1108 2023-05-04 16:55:27.000000 PaReBrick-0.5.5/parebrick/utils/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)     4644 2023-05-04 17:13:35.000000 PaReBrick-0.5.5/parebrick/utils/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3962 2023-05-04 17:19:11.000000 PaReBrick-0.5.5/parebrick/utils/data/stats.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2370 2023-05-04 17:07:38.000000 PaReBrick-0.5.5/parebrick/utils/data/unique_gene_filters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      600 2021-07-05 10:42:17.000000 PaReBrick-0.5.5/parebrick/utils/decorators.py
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 18:00:54.528302 PaReBrick-0.5.5/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1902 2023-05-04 18:00:34.000000 PaReBrick-0.5.5/setup.py
```

### Comparing `PaReBrick-0.5.4/LICENSE` & `PaReBrick-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/PKG-INFO` & `PaReBrick-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.4
+Version: 0.5.5
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.4/PaReBrick.egg-info/PKG-INFO` & `PaReBrick-0.5.5/PaReBrick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PaReBrick
-Version: 0.5.4
+Version: 0.5.5
 Summary: A bioinf tool for finding genome rearrangements in bacterial genomes
 Home-page: https://github.com/ctlab/parallel-rearrangements
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
 Keywords: genome rearrangements,phylogenetic trees,non-convex characters,synteny blocks,phylogenetic tree,pattern consistency
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PaReBrick-0.5.4/PaReBrick.egg-info/SOURCES.txt` & `PaReBrick-0.5.5/PaReBrick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/README.md` & `PaReBrick-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/characters/balanced.py` & `PaReBrick-0.5.5/parebrick/characters/balanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,40 +37,39 @@
             if neighbour_edge:
                 neighbour_edge_genomes = get_colors_by_edge(neighbour_edge)
                 neighbour_edge_genomes_count = sum(neighbour_edge_genomes.values())
 
                 neighbour_edge_genomes_names = set(g for g in genomes if neighbour_edge_genomes[BGGenome(g)])
                 white_genomes_at_neighbour_edge = len(neighbour_edge_genomes_names & white_genomes)
 
-                # if white_genomes_at_neighbour_edge < 1:
-                if neighbour_edge_genomes_count <= len(genomes) // 2:
+                if white_genomes_at_neighbour_edge < 1:
+                # if neighbour_edge_genomes_count <= len(genomes) // 2:
                     return 1
 
                 pair = (v1_neighbour, v2_neighbour)
                 if pair not in possible_edges:
                     possible_edges.append(pair)
                 return 3 + possible_edges.index(pair)
             else:
                 return 1
 
-    cnt = Counter([genome.name.rsplit('.', 1)[0]
+    cnt = Counter([genome.name
                    for genome, count in get_colors_by_edge(edge).items()
                    for _ in range(count)])
     possible_edges = []
     white_genomes = set(g for g in genomes if BGGenome(g))
     return {genome: get_genome_character_state_by_edge(genome) for genome in genomes}, possible_edges
 
 def construct_vertex_genome_index(bg):
     neighbour_index = {}
     for v in bg.bg:
         for edge in bg.get_edges_by_vertex(v):
             colors = get_colors_by_edge(edge)
             for color in colors:
-                strain, _ = color.name.rsplit('.', 1)
-                neighbour_index[(str(v), strain)] = edge.vertex2
+                neighbour_index[(str(v), color.name)] = edge.vertex2
 
     return neighbour_index
 
 def get_characters_balanced(grimm_file, genomes, logger):
     bg = GRIMMReader.get_breakpoint_graph(open(grimm_file))
     logger.info('Breakpoint graph parsed')
 
@@ -83,20 +82,20 @@
         nodes_len = len(list(component_bg.nodes()))
         if nodes_len == 2: continue
 
         logger.info(f'Getting characters from breakpoint graph component, size={len(component_bg.bg)}')
 
         neighbour_index = construct_vertex_genome_index(component_bg)
 
-        for i_edge, edge in enumerate(component_bg.edges()):
+        for edge in component_bg.edges():
             v1, v2 = edge.vertex1.name, edge.vertex2.name
             if v1 > v2: v1, v2 = v2, v1
 
             genome_colors, neighbour_edges = get_character_by_edge(component_bg, edge, genomes, neighbour_index)
-            if white_proportion(genome_colors.values()) < 0.5: continue
+            if white_proportion(genome_colors.values()) < 0.33: continue
 
             labels = ['adjacency exists', 'complex break of adjacency', 'some block is not presented'] + \
                      [f'inversion with {v1n}-{v2n}' for (v1n, v2n) in neighbour_edges]
 
             characters.append((v1, v2, genome_colors, labels))
 
     return characters
@@ -111,15 +110,15 @@
 
         score_rear, count_rear, count_all_rear = tree_holder.count_parallel_rearrangements(skip_grey=True)
         score_break, count_break = tree_holder.count_parallel_breakpoints()
 
         white_strains = [strain for strain, color in genome_colors.items() if color == 0]
         mean_break_length = np.mean([distance_between_blocks[(b1, b2)][strain] for strain in white_strains])
 
-        ans.append([f'{v1}–{v2}', int(mean_break_length), score_rear, count_rear, count_all_rear, score_break, count_break,
+        ans.append([f'{v1}-{v2}', int(mean_break_length), score_rear, count_rear, count_all_rear, score_break, count_break,
                     count_break <= 1])
 
     return ans
 
 def write_stats_csv_balanced(stats, stats_file):
     rows = [['id', 'adjacency', 'mean_break_length_nucleotide', 'parallel_rear_score', 'number_of_inconsistent_colors',
             'number_of_parallel_events', 'parallel_break_score', 'number_of_parallel_breaks', 'tree_consistent']] + \
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PaReBrick-0.5.4/parebrick/characters/neighbours.py` & `PaReBrick-0.5.5/parebrick/characters/neighbours.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/characters/unbalanced.py` & `PaReBrick-0.5.5/parebrick/characters/unbalanced.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/characters/which_chromosome.py` & `PaReBrick-0.5.5/parebrick/characters/which_chromosome.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/clustering/clustering.py` & `PaReBrick-0.5.5/parebrick/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/clustering/distance_matrices.py` & `PaReBrick-0.5.5/parebrick/clustering/distance_matrices.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/drawer.py` & `PaReBrick-0.5.5/parebrick/drawer.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/drawer_b_mallei.py` & `PaReBrick-0.5.5/parebrick/drawer_b_mallei.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/drawer_e_coli.py` & `PaReBrick-0.5.5/parebrick/drawer_e_coli.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/main.py` & `PaReBrick-0.5.5/parebrick/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
     export_df_to_infercars(unique_blocks_df, preprocessed_data_folder + INFERCARS_UNIQUE_FILENAME)
     blocks_df.to_csv(preprocessed_data_folder + CSV_BLOCK_FILENAME, index=False)
     unique_blocks_df.to_csv(preprocessed_data_folder + CSV_BLOCK_UNIQUE_FILENAME, index=False)
     with open(preprocessed_data_folder + CSV_GENOME_LENGTH, 'w') as f:
         w = csv.writer(f)
         w.writerow(['Genome', 'Length'])
-        w.writerows(chr_lengths.items())
+        w.writerows(genome_lengths.items())
 
     logger.info(f'Blocks count: {len(blocks_df["block"].unique())}')
     logger.info(f'Unique one-copy blocks count: {len(unique_blocks_df["block"].unique())}')
 
     logger.info(f'Mean block coverage: {get_mean_coverage(blocks_df, genome_lengths) * 100} %')
     logger.info(f'Mean common one-copy blocks coverage: '
                 f'{get_mean_coverage(unique_blocks_df, genome_lengths) * 100 if have_unique else 0} %')
```

### Comparing `PaReBrick-0.5.4/parebrick/tree/neighbours_utils.py` & `PaReBrick-0.5.5/parebrick/tree/neighbours_utils.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/tree/tree_holder.py` & `PaReBrick-0.5.5/parebrick/tree/tree_holder.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/tree_holder_draw.py` & `PaReBrick-0.5.5/parebrick/tree_holder_draw.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/utils/data/converters.py` & `PaReBrick-0.5.5/parebrick/utils/data/converters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/utils/data/parsers.py` & `PaReBrick-0.5.5/parebrick/utils/data/parsers.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/utils/data/stats.py` & `PaReBrick-0.5.5/parebrick/utils/data/stats.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/utils/data/unique_gene_filters.py` & `PaReBrick-0.5.5/parebrick/utils/data/unique_gene_filters.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/parebrick/utils/decorators.py` & `PaReBrick-0.5.5/parebrick/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PaReBrick-0.5.4/setup.py` & `PaReBrick-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='PaReBrick',
-    version='0.5.4',
+    version='0.5.5',
     description='A bioinf tool for finding genome rearrangements in bacterial genomes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ctlab/parallel-rearrangements',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

