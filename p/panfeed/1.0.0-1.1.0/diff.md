# Comparing `tmp/panfeed-1.0.0.tar.gz` & `tmp/panfeed-1.1.0.tar.gz`

## Comparing `panfeed-1.0.0.tar` & `panfeed-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.0.0/environment.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed-runner.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/__init__.py
--rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/get_kmers.py
--rw-r--r--   0        0        0    13281 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/panfeed.py
--rw-r--r--   0        0        0    16076 2020-02-02 00:00:00.000000 panfeed-1.0.0/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.0.0/LICENSE
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 panfeed-1.0.0/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 panfeed-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.1.0/environment.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/__init__.py
+-rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    13281 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/panfeed.py
+-rw-r--r--   0        0        0    16008 2020-02-02 00:00:00.000000 panfeed-1.1.0/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.1.0/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.1.0/PKG-INFO
```

### Comparing `panfeed-1.0.0/panfeed/__main__.py` & `panfeed-1.1.0/panfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/classes.py` & `panfeed-1.1.0/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/colorlog.py` & `panfeed-1.1.0/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/get_clusters.py` & `panfeed-1.1.0/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/get_kmers.py` & `panfeed-1.1.0/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/input.py` & `panfeed-1.1.0/panfeed/input.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/panfeed.py` & `panfeed-1.1.0/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/panfeed/plot.py` & `panfeed-1.1.0/panfeed/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,49 +254,43 @@
 
         # p-value matrix
         g = cl.pivot_table(index='strain', columns='gene_start',
                            values='significance',
                            aggfunc=max)
         # add missing strains for which no entry is present in k-mers table
         if len(strains.difference(g.index)) > 0:
-            g = g.T
-            g[sorted(strains.difference(g.index))] = np.nan
-            g = g.T
+            g = g.reindex(sorted(g.index) + sorted(strains.difference(g.index)))
         if args.phenotype_column is None:
             # sort the table by p-values
             g = g.loc[g.fillna(0).T.max().sort_values(ascending=False).index]
         else:
             # sort by phenotype
             g = g.loc[p.index]
 
         # nucleotide matrix
         b = cl.pivot_table(index='strain', columns='gene_start',
                            values='scalar',
                            aggfunc=handle_paralogs)
         # add missing strains for which no entry is present in k-mers table
         if len(strains.difference(b.index)) > 0:
-            b = b.T
-            b[sorted(strains.difference(b.index))] = np.nan
-            b = b.T
+            b = b.reindex(sorted(b.index) + sorted(strains.difference(b.index)))
         if args.phenotype_column is None:
             # sort the table by p-values
             b = b.loc[g.index]
         else:
             # sort by phenotype
             b = b.loc[p.index]
         if args.nucleotides:
             # nucleotide matrix
             t = cl.pivot_table(index='strain', columns='gene_start',
                                values='base',
                                aggfunc=handle_paralogs_text)
             # add missing strains for which no entry is present in k-mers table
             if len(strains.difference(t.index)) > 0:
-                t = t.T
-                t[sorted(strains.difference(b.index))] = '-'
-                t = t.T
+                t = t.reindex(sorted(t.index) + sorted(strains.difference(t.index)))
             if args.phenotype_column is None:
                 # sort the table by p-values
                 t = t.loc[g.index]
             else:
                 # sort by phenotype
                 t = t.loc[p.index]
```

### Comparing `panfeed-1.0.0/LICENSE` & `panfeed-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/README.md` & `panfeed-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Mapping of associated patterns to gene clusters and base resolution mapping of k-mers can be then achieved with the other two outputs of `panfeed`.
 Advantages of this approach over the generation of k-mers from a global de Bruijn
 graph include a lower chance of encountering artifacts
 due to repetitive regions and easier interpretations and visualization of results.
 
 # Citation
 
-Coming soon
+Neubauer, H., & Galardini, M. (2023). **Improved interpretability of bacterial genome-wide associations using gene cluster centric k-mers**. bioRxiv. [10.1101/2023.04.11.536385](https://www.biorxiv.org/content/10.1101/2023.04.11.536385v1)
 
 # Installation
 
 `panfeed` can be installed using `pip`:
 
     python3 -m pip install panfeed
```

### Comparing `panfeed-1.0.0/pyproject.toml` & `panfeed-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.0.0/PKG-INFO` & `panfeed-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.0.0
+Version: 1.1.0
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,15 @@
 Mapping of associated patterns to gene clusters and base resolution mapping of k-mers can be then achieved with the other two outputs of `panfeed`.
 Advantages of this approach over the generation of k-mers from a global de Bruijn
 graph include a lower chance of encountering artifacts
 due to repetitive regions and easier interpretations and visualization of results.
 
 # Citation
 
-Coming soon
+Neubauer, H., & Galardini, M. (2023). **Improved interpretability of bacterial genome-wide associations using gene cluster centric k-mers**. bioRxiv. [10.1101/2023.04.11.536385](https://www.biorxiv.org/content/10.1101/2023.04.11.536385v1)
 
 # Installation
 
 `panfeed` can be installed using `pip`:
 
     python3 -m pip install panfeed
```

