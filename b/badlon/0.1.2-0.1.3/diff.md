# Comparing `tmp/badlon-0.1.2.tar.gz` & `tmp/badlon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badlon-0.1.2.tar", last modified: Mon Jul 11 11:44:11 2022, max compression
+gzip compressed data, was "badlon-0.1.3.tar", last modified: Thu May  4 13:55:30 2023, max compression
```

## Comparing `badlon-0.1.2.tar` & `badlon-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2022-07-11 11:44:11.517296 badlon-0.1.2/
--rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 badlon-0.1.2/LICENSE
--rw-r--r--   0 alexey     (501) staff       (20)     7702 2022-07-11 11:44:11.517175 badlon-0.1.2/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)     6832 2022-07-11 11:41:55.000000 badlon-0.1.2/README.md
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2022-07-11 11:44:11.514115 badlon-0.1.2/badlon/
--rw-r--r--   0 alexey     (501) staff       (20)     8957 2022-07-06 15:49:40.000000 badlon-0.1.2/badlon/block_gene_match.py
--rw-r--r--   0 alexey     (501) staff       (20)     3975 2022-07-06 15:02:57.000000 badlon-0.1.2/badlon/blocks_analysis.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2022-07-11 11:44:11.516085 badlon-0.1.2/badlon/charts/
--rw-r--r--   0 alexey     (501) staff       (20)     3257 2022-07-06 15:49:40.000000 badlon-0.1.2/badlon/charts/coverage.py
--rw-r--r--   0 alexey     (501) staff       (20)     1276 2022-06-23 11:42:57.000000 badlon-0.1.2/badlon/charts/inter_block_distribution.py
--rw-r--r--   0 alexey     (501) staff       (20)      590 2022-04-20 13:50:09.000000 badlon-0.1.2/badlon/charts/length_distribution.py
--rw-r--r--   0 alexey     (501) staff       (20)     3605 2022-04-21 14:57:00.000000 badlon-0.1.2/badlon/charts/pan_genome.py
--rw-r--r--   0 alexey     (501) staff       (20)      854 2022-04-20 13:45:45.000000 badlon-0.1.2/badlon/charts/u_curve.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2022-07-11 11:44:11.516919 badlon-0.1.2/badlon/data/
--rw-r--r--   0 alexey     (501) staff       (20)     1106 2022-04-19 13:26:52.000000 badlon-0.1.2/badlon/data/converters.py
--rw-r--r--   0 alexey     (501) staff       (20)      446 2022-04-20 10:57:44.000000 badlon-0.1.2/badlon/data/coverage.py
--rw-r--r--   0 alexey     (501) staff       (20)     2249 2022-07-06 15:23:50.000000 badlon-0.1.2/badlon/data/parsers.py
--rw-r--r--   0 alexey     (501) staff       (20)      919 2022-04-20 13:56:20.000000 badlon-0.1.2/badlon/data/process.py
--rw-r--r--   0 alexey     (501) staff       (20)     3367 2022-07-11 11:13:49.000000 badlon-0.1.2/badlon/prepare_data_for_sibeliaz.py
--rw-r--r--   0 alexey     (501) staff       (20)     1721 2022-07-06 14:44:14.000000 badlon-0.1.2/badlon/run_badlon.py
-drwxr-xr-x   0 alexey     (501) staff       (20)        0 2022-07-11 11:44:11.514882 badlon-0.1.2/badlon.egg-info/
--rw-r--r--   0 alexey     (501) staff       (20)     7702 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/PKG-INFO
--rw-r--r--   0 alexey     (501) staff       (20)      572 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/SOURCES.txt
--rw-r--r--   0 alexey     (501) staff       (20)        1 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/dependency_links.txt
--rw-r--r--   0 alexey     (501) staff       (20)       51 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/entry_points.txt
--rw-r--r--   0 alexey     (501) staff       (20)       31 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/requires.txt
--rw-r--r--   0 alexey     (501) staff       (20)        7 2022-07-11 11:44:11.000000 badlon-0.1.2/badlon.egg-info/top_level.txt
--rw-r--r--   0 alexey     (501) staff       (20)       38 2022-07-11 11:44:11.517341 badlon-0.1.2/setup.cfg
--rw-r--r--   0 alexey     (501) staff       (20)     1446 2022-07-11 11:44:02.000000 badlon-0.1.2/setup.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 13:55:30.433390 badlon-0.1.3/
+-rw-r--r--   0 alexey     (501) staff       (20)     1089 2021-07-05 10:42:16.000000 badlon-0.1.3/LICENSE
+-rw-r--r--   0 alexey     (501) staff       (20)     7812 2023-05-04 13:55:30.433236 badlon-0.1.3/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)     6978 2022-10-18 14:30:25.000000 badlon-0.1.3/README.md
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 13:55:30.429181 badlon-0.1.3/badlon/
+-rw-r--r--   0 alexey     (501) staff       (20)     9101 2023-05-04 13:46:10.000000 badlon-0.1.3/badlon/block_gene_match.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3975 2022-07-06 15:02:57.000000 badlon-0.1.3/badlon/blocks_analysis.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 13:55:30.431895 badlon-0.1.3/badlon/charts/
+-rw-r--r--   0 alexey     (501) staff       (20)     3257 2022-07-06 15:49:40.000000 badlon-0.1.3/badlon/charts/coverage.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1276 2022-06-23 11:42:57.000000 badlon-0.1.3/badlon/charts/inter_block_distribution.py
+-rw-r--r--   0 alexey     (501) staff       (20)      590 2022-04-20 13:50:09.000000 badlon-0.1.3/badlon/charts/length_distribution.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3605 2022-04-21 14:57:00.000000 badlon-0.1.3/badlon/charts/pan_genome.py
+-rw-r--r--   0 alexey     (501) staff       (20)      854 2022-04-20 13:45:45.000000 badlon-0.1.3/badlon/charts/u_curve.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 13:55:30.432937 badlon-0.1.3/badlon/data/
+-rw-r--r--   0 alexey     (501) staff       (20)     1106 2022-04-19 13:26:52.000000 badlon-0.1.3/badlon/data/converters.py
+-rw-r--r--   0 alexey     (501) staff       (20)      446 2022-04-20 10:57:44.000000 badlon-0.1.3/badlon/data/coverage.py
+-rw-r--r--   0 alexey     (501) staff       (20)     2249 2022-07-06 15:23:50.000000 badlon-0.1.3/badlon/data/parsers.py
+-rw-r--r--   0 alexey     (501) staff       (20)      919 2022-04-20 13:56:20.000000 badlon-0.1.3/badlon/data/process.py
+-rw-r--r--   0 alexey     (501) staff       (20)     3367 2022-07-11 11:13:49.000000 badlon-0.1.3/badlon/prepare_data_for_sibeliaz.py
+-rw-r--r--   0 alexey     (501) staff       (20)     1721 2022-07-06 14:44:14.000000 badlon-0.1.3/badlon/run_badlon.py
+drwxr-xr-x   0 alexey     (501) staff       (20)        0 2023-05-04 13:55:30.430285 badlon-0.1.3/badlon.egg-info/
+-rw-r--r--   0 alexey     (501) staff       (20)     7812 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/PKG-INFO
+-rw-r--r--   0 alexey     (501) staff       (20)      572 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        1 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       50 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/entry_points.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       31 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/requires.txt
+-rw-r--r--   0 alexey     (501) staff       (20)        7 2023-05-04 13:55:30.000000 badlon-0.1.3/badlon.egg-info/top_level.txt
+-rw-r--r--   0 alexey     (501) staff       (20)       38 2023-05-04 13:55:30.434198 badlon-0.1.3/setup.cfg
+-rw-r--r--   0 alexey     (501) staff       (20)     1446 2023-05-04 13:46:42.000000 badlon-0.1.3/setup.py
```

### Comparing `badlon-0.1.2/LICENSE` & `badlon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/PKG-INFO` & `badlon-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: badlon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A bioinf tool for analyzing pan-genome and other features based on synteny blocks
 Home-page: https://github.com/oxygen311/badlon
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
-License: UNKNOWN
 Keywords: synteny blocks,pan genome,core genome,bioinformatics,genome alignment
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +26,15 @@
 
 ```bash
 pip install badlon
 ```
 
 Now you can run tool from any directory as `badlon`.
 
-## Usage
+## Pipeline Usage
 
 ### Modules
 
 Badlon includes multiple modules to process data. They can be listed with help command:
 
 ```bash
 $ badlon --help
@@ -50,42 +48,50 @@
     analysis            Analyze pan-genome and other block-based features based on synteny blocks.
     match               Performs matching of block and genes based on coordinates.
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
+Here is recommended pipeline to process data with badlon:
+
 ### Step 1: prepare data with [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA)
 
-If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
+If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data for badlon using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
 
 To do so, you can use those commands:
 
 #### 1.1 Preparing data and tables with `PanACoTA prepare` module:
 
-`PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125`
+```
+PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125
+```
 
 * `--min 0 --max 1` are used to keep all genomes, parameter can be changed depending on task as well as all other parameters;
 * For check other parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#prepare-subcommand) documentation.
 
 #### 1.2 Annotating genomes with `PanACoTA annotate` module:
 
-`PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16`
+```
+PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16
+```
 
 * You can change label `-n ESCO` depending on your species (ESCO is for *Escherichia coli*);
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA annotate`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
 
 #### 1.3 Calling orthology genes using `PanACoTA pangenome` module:
 
-`PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome`
+```
+PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome
+```
 
 * You can change `-i` which is minimum sequence identity to be considered in the same cluster (float between 0 and 1). Default is 0.8.
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA pangenome`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#pangenome-subcommand) documentation.
 
-### Step 2: `prepare` module of `badlon`
+### Step 2: Preparing data for alignment with `badlon prepare` module
 
 Prepare module is used to prepare data for using SibeliaZ package keeping all necessary information: genome labels and chromosome numbers.
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon prepare --help
@@ -114,35 +120,39 @@
                         Folder with PanACoTA output. Will be used to search
                         genome files based on LSTINFO file from annotate
                         module.
 ```
 
 Example command:
 
-`badlon prepare -f 2-annotate -o for_sibeliaz.fna`
+```
+badlon prepare -f 2-annotate -o for_sibeliaz.fna
+```
 
-### Step 2. Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
+### Step 3: Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
 
-#### 2.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
+#### 3.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
 
 Example:
-`sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna`
+```
+sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna
+```
 
-* Watch out `-a` it's needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
+* Watch out `-a` it needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
 
-#### 2.2 Obtaining blocks from alignment
+#### 3.2 Obtaining blocks from alignment
 
 Check recommended command from `badlon prepare` module output. Usually it's (blocks minimal size 3000):
 ```bash
 cd sibeliaz_out
 echo $'30 150\n100 500\n500 1500' > fine.txt
 maf2synteny -s fine.txt -b 3000 blocks_coords.gff
 ```
 
-### Step 3. Calculating block based statistics and charts with `badlon analysis` module:
+### Step 4: Calculating block based statistics and charts with `badlon analysis` module:
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon analysis --help
 usage: badlon analysis [-h] --blocks_file BLOCKS_FILE --type {chr,contig}
                        [--output OUTPUT]
@@ -164,15 +174,15 @@
 Example command:
 
 ```bash
 cd ..
 badlon analysis -b sibeliaz_out/3000/blocks_coords.txt
 ```
 
-### Step 4 (optional): Match block and genes annotation with  `badlon match` module
+### Step 5 (optional): Match block and genes annotation with  `badlon match` module
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon match --help
 usage: badlon match [-h] --blocks_file BLOCKS_FILE --annotated_folder
                     ANNOTATED_FOLDER --pangenome_file PANGENOME_FILE --type
@@ -196,9 +206,10 @@
                         `pangenome` step of PanACoTA.
   --type {chr,contig}, -t {chr,contig}
                         Type of genome assembly, either 'chr' or 'contig'
 ```
 
 Example command:
 
-`badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig`
-
+```
+badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig
+```
```

### Comparing `badlon-0.1.2/README.md` & `badlon-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```bash
 pip install badlon
 ```
 
 Now you can run tool from any directory as `badlon`.
 
-## Usage
+## Pipeline Usage
 
 ### Modules
 
 Badlon includes multiple modules to process data. They can be listed with help command:
 
 ```bash
 $ badlon --help
@@ -28,42 +28,50 @@
     analysis            Analyze pan-genome and other block-based features based on synteny blocks.
     match               Performs matching of block and genes based on coordinates.
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
+Here is recommended pipeline to process data with badlon:
+
 ### Step 1: prepare data with [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA)
 
-If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
+If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data for badlon using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
 
 To do so, you can use those commands:
 
 #### 1.1 Preparing data and tables with `PanACoTA prepare` module:
 
-`PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125`
+```
+PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125
+```
 
 * `--min 0 --max 1` are used to keep all genomes, parameter can be changed depending on task as well as all other parameters;
 * For check other parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#prepare-subcommand) documentation.
 
 #### 1.2 Annotating genomes with `PanACoTA annotate` module:
 
-`PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16`
+```
+PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16
+```
 
 * You can change label `-n ESCO` depending on your species (ESCO is for *Escherichia coli*);
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA annotate`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
 
 #### 1.3 Calling orthology genes using `PanACoTA pangenome` module:
 
-`PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome`
+```
+PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome
+```
 
 * You can change `-i` which is minimum sequence identity to be considered in the same cluster (float between 0 and 1). Default is 0.8.
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA pangenome`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#pangenome-subcommand) documentation.
 
-### Step 2: `prepare` module of `badlon`
+### Step 2: Preparing data for alignment with `badlon prepare` module
 
 Prepare module is used to prepare data for using SibeliaZ package keeping all necessary information: genome labels and chromosome numbers.
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon prepare --help
@@ -92,35 +100,39 @@
                         Folder with PanACoTA output. Will be used to search
                         genome files based on LSTINFO file from annotate
                         module.
 ```
 
 Example command:
 
-`badlon prepare -f 2-annotate -o for_sibeliaz.fna`
+```
+badlon prepare -f 2-annotate -o for_sibeliaz.fna
+```
 
-### Step 2. Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
+### Step 3: Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
 
-#### 2.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
+#### 3.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
 
 Example:
-`sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna`
+```
+sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna
+```
 
-* Watch out `-a` it's needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
+* Watch out `-a` it needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
 
-#### 2.2 Obtaining blocks from alignment
+#### 3.2 Obtaining blocks from alignment
 
 Check recommended command from `badlon prepare` module output. Usually it's (blocks minimal size 3000):
 ```bash
 cd sibeliaz_out
 echo $'30 150\n100 500\n500 1500' > fine.txt
 maf2synteny -s fine.txt -b 3000 blocks_coords.gff
 ```
 
-### Step 3. Calculating block based statistics and charts with `badlon analysis` module:
+### Step 4: Calculating block based statistics and charts with `badlon analysis` module:
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon analysis --help
 usage: badlon analysis [-h] --blocks_file BLOCKS_FILE --type {chr,contig}
                        [--output OUTPUT]
@@ -142,15 +154,15 @@
 Example command:
 
 ```bash
 cd ..
 badlon analysis -b sibeliaz_out/3000/blocks_coords.txt
 ```
 
-### Step 4 (optional): Match block and genes annotation with  `badlon match` module
+### Step 5 (optional): Match block and genes annotation with  `badlon match` module
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon match --help
 usage: badlon match [-h] --blocks_file BLOCKS_FILE --annotated_folder
                     ANNOTATED_FOLDER --pangenome_file PANGENOME_FILE --type
@@ -174,8 +186,10 @@
                         `pangenome` step of PanACoTA.
   --type {chr,contig}, -t {chr,contig}
                         Type of genome assembly, either 'chr' or 'contig'
 ```
 
 Example command:
 
-`badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig`
+```
+badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig
+```
```

### Comparing `badlon-0.1.2/badlon/block_gene_match.py` & `badlon-0.1.3/badlon/block_gene_match.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,17 @@
 
 def match_blocks_genes(blocks_df, genes_df):
     def get_ogs_ids(genes_df, inverted=False):
         ogs = [0 if og == '' else (og if or_ == 'D' else -og) for og, or_ in zip(genes_df.og, genes_df.orientation)]
         ids = [id for id, or_ in zip(genes_df.gene_id, genes_df.orientation)]
         return ([-og for og in ogs[::-1]], ids[::-1]) if inverted else (ogs, ids)
 
-    block_to_left_border_ogs, block_to_left_border_ids = {}, {}
-    block_to_right_border_ogs, block_to_right_border_ids = {}, {}
-    block_to_ogs, block_to_ids = {}, {}
+    block_to_left_border_ogs, block_to_left_border_ids = defaultdict(list), defaultdict(list)
+    block_to_right_border_ogs, block_to_right_border_ids = defaultdict(list), defaultdict(list)
+    block_to_ogs, block_to_ids = defaultdict(list), defaultdict(list)
 
     gene_to_block = defaultdict(lambda: ('outside', ''))
 
     for strain, genes_strain_df in genes_df.groupby('genome'):
         for chr, genes_strain_chr_df in genes_strain_df.groupby('chr/contig'):
             blocks_strain_df = blocks_df[(blocks_df['genome'] == strain) & (blocks_df['chr/contig'] == str(chr))] \
                 .sort_values(by=['start'])
@@ -104,14 +104,16 @@
                 if genes_strain_chr_df.end.values[genes_start_index] < b_start:
                     genes_start_index += 1
 
                 current_genes = genes_strain_chr_df[genes_start_index:genes_end_index]
 
                 genes_start_index, genes_end_index = 0, len(current_genes)
 
+                if len(current_genes) == 0: continue
+
                 start_is_on_border = current_genes.start.values[0] < b_start
                 end_is_on_border = current_genes.end.values[-1] > b_end
 
                 if start_is_on_border: genes_start_index += 1
                 if end_is_on_border: genes_end_index -= 1
 
                 inverted = b_or == '-'
```

### Comparing `badlon-0.1.2/badlon/blocks_analysis.py` & `badlon-0.1.3/badlon/blocks_analysis.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/charts/coverage.py` & `badlon-0.1.3/badlon/charts/coverage.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/charts/inter_block_distribution.py` & `badlon-0.1.3/badlon/charts/inter_block_distribution.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/charts/length_distribution.py` & `badlon-0.1.3/badlon/charts/length_distribution.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/charts/pan_genome.py` & `badlon-0.1.3/badlon/charts/pan_genome.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/charts/u_curve.py` & `badlon-0.1.3/badlon/charts/u_curve.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/data/converters.py` & `badlon-0.1.3/badlon/data/converters.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/data/parsers.py` & `badlon-0.1.3/badlon/data/parsers.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/data/process.py` & `badlon-0.1.3/badlon/data/process.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/prepare_data_for_sibeliaz.py` & `badlon-0.1.3/badlon/prepare_data_for_sibeliaz.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon/run_badlon.py` & `badlon-0.1.3/badlon/run_badlon.py`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/badlon.egg-info/PKG-INFO` & `badlon-0.1.3/badlon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: badlon
-Version: 0.1.2
+Version: 0.1.3
 Summary: A bioinf tool for analyzing pan-genome and other features based on synteny blocks
 Home-page: https://github.com/oxygen311/badlon
 Author: Alexey Zabelkin
 Author-email: a.zabelkin@itmo.ru
-License: UNKNOWN
 Keywords: synteny blocks,pan genome,core genome,bioinformatics,genome alignment
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +26,15 @@
 
 ```bash
 pip install badlon
 ```
 
 Now you can run tool from any directory as `badlon`.
 
-## Usage
+## Pipeline Usage
 
 ### Modules
 
 Badlon includes multiple modules to process data. They can be listed with help command:
 
 ```bash
 $ badlon --help
@@ -50,42 +48,50 @@
     analysis            Analyze pan-genome and other block-based features based on synteny blocks.
     match               Performs matching of block and genes based on coordinates.
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
+Here is recommended pipeline to process data with badlon:
+
 ### Step 1: prepare data with [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA)
 
-If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
+If you have genomes in some folder called `some_folder` (one file for genome), we suggest preparing data for badlon using [`PanACoTA` pipeline](https://github.com/gem-pasteur/PanACoTA).
 
 To do so, you can use those commands:
 
 #### 1.1 Preparing data and tables with `PanACoTA prepare` module:
 
-`PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125`
+```
+PanACoTA prepare --norefseq --min 0 --max 1 -o 1-prepare -d some_folder --cutn 125
+```
 
 * `--min 0 --max 1` are used to keep all genomes, parameter can be changed depending on task as well as all other parameters;
 * For check other parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#prepare-subcommand) documentation.
 
 #### 1.2 Annotating genomes with `PanACoTA annotate` module:
 
-`PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16`
+```
+PanACoTA annotate --info 1-prepare/L* -r 2-annotate -n ESCO --threads 16
+```
 
 * You can change label `-n ESCO` depending on your species (ESCO is for *Escherichia coli*);
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA annotate`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
 
 #### 1.3 Calling orthology genes using `PanACoTA pangenome` module:
 
-`PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome`
+```
+PanACoTA pangenome -l 2-annotate/LSTINFO-* -n ESCO -d 2-annotate/Proteins/ -o 3-pangenome
+```
 
 * You can change `-i` which is minimum sequence identity to be considered in the same cluster (float between 0 and 1). Default is 0.8.
-* For check parameters visit [`PanACoTA prepare`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#annotate-subcommand) documentation.
+* For check parameters visit [`PanACoTA pangenome`](https://aperrin.pages.pasteur.fr/pipeline_annotation/html-doc/usage.html#pangenome-subcommand) documentation.
 
-### Step 2: `prepare` module of `badlon`
+### Step 2: Preparing data for alignment with `badlon prepare` module
 
 Prepare module is used to prepare data for using SibeliaZ package keeping all necessary information: genome labels and chromosome numbers.
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon prepare --help
@@ -114,35 +120,39 @@
                         Folder with PanACoTA output. Will be used to search
                         genome files based on LSTINFO file from annotate
                         module.
 ```
 
 Example command:
 
-`badlon prepare -f 2-annotate -o for_sibeliaz.fna`
+```
+badlon prepare -f 2-annotate -o for_sibeliaz.fna
+```
 
-### Step 2. Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
+### Step 3: Obtaining blocks with [SibeliaZ](https://github.com/medvedevgroup/SibeliaZ)
 
-#### 2.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
+#### 3.1 Running SibeliaZ with recommended command based on `badlon prepare` output.
 
 Example:
-`sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna`
+```
+sibeliaz -k 15 -a 100 -n -t 32 -o sibeliaz_out for_sibeliaz.fna
+```
 
-* Watch out `-a` it's needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
+* Watch out `-a` it needs to be equal around `number_of_genome * 20`, `badlon prepare` calculates it automatically.
 
-#### 2.2 Obtaining blocks from alignment
+#### 3.2 Obtaining blocks from alignment
 
 Check recommended command from `badlon prepare` module output. Usually it's (blocks minimal size 3000):
 ```bash
 cd sibeliaz_out
 echo $'30 150\n100 500\n500 1500' > fine.txt
 maf2synteny -s fine.txt -b 3000 blocks_coords.gff
 ```
 
-### Step 3. Calculating block based statistics and charts with `badlon analysis` module:
+### Step 4: Calculating block based statistics and charts with `badlon analysis` module:
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon analysis --help
 usage: badlon analysis [-h] --blocks_file BLOCKS_FILE --type {chr,contig}
                        [--output OUTPUT]
@@ -164,15 +174,15 @@
 Example command:
 
 ```bash
 cd ..
 badlon analysis -b sibeliaz_out/3000/blocks_coords.txt
 ```
 
-### Step 4 (optional): Match block and genes annotation with  `badlon match` module
+### Step 5 (optional): Match block and genes annotation with  `badlon match` module
 
 Parameters can be checked with help option:
 
 ```bash
 $ badlon match --help
 usage: badlon match [-h] --blocks_file BLOCKS_FILE --annotated_folder
                     ANNOTATED_FOLDER --pangenome_file PANGENOME_FILE --type
@@ -196,9 +206,10 @@
                         `pangenome` step of PanACoTA.
   --type {chr,contig}, -t {chr,contig}
                         Type of genome assembly, either 'chr' or 'contig'
 ```
 
 Example command:
 
-`badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig`
-
+```
+badlon match -b sibeliaz_out/3000/blocks_coords.txt -a 2-annotate/ -pg 3-pangenome/*.lst -t contig
+```
```

### Comparing `badlon-0.1.2/badlon.egg-info/SOURCES.txt` & `badlon-0.1.3/badlon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badlon-0.1.2/setup.py` & `badlon-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='badlon',
-    version='0.1.2',
+    version='0.1.3',
     description='A bioinf tool for analyzing pan-genome and other features based on synteny blocks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/oxygen311/badlon',
     author='Alexey Zabelkin',
     author_email='a.zabelkin@itmo.ru',
     classifiers=[
```

