# Comparing `tmp/ont-remora-2.0.0.tar.gz` & `tmp/ont-remora-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-remora-2.0.0.tar", last modified: Tue Dec  6 03:06:31 2022, max compression
+gzip compressed data, was "ont-remora-2.1.0.tar", last modified: Wed May  3 18:51:13 2023, max compression
```

## Comparing `ont-remora-2.0.0.tar` & `ont-remora-2.1.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2022-12-06 03:06:31.513340 ont-remora-2.0.0/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2022-07-21 21:33:30.000000 ont-remora-2.0.0/LICENSE.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2022-09-30 13:36:35.000000 ont-remora-2.0.0/MANIFEST.in
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7818 2022-12-06 03:06:31.513449 ont-remora-2.0.0/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7394 2022-10-04 18:41:54.000000 ont-remora-2.0.0/README.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2022-07-21 21:33:30.000000 ont-remora-2.0.0/pyproject.toml
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1610 2022-12-06 03:06:31.513970 ont-remora-2.0.0/setup.cfg
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2022-07-21 21:33:30.000000 ont-remora-2.0.0/setup.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2022-12-06 03:06:31.504348 ont-remora-2.0.0/src/
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2022-12-06 03:06:31.506781 ont-remora-2.0.0/src/ont_remora.egg-info/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7818 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/PKG-INFO
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      846 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/SOURCES.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/dependency_links.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       43 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/entry_points.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2022-07-22 16:07:04.000000 ont-remora-2.0.0/src/ont_remora.egg-info/not-zip-safe
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      156 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/requires.txt
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2022-12-06 03:06:31.000000 ont-remora-2.0.0/src/ont_remora.egg-info/top_level.txt
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2022-12-06 03:06:31.512690 ont-remora-2.0.0/src/remora/
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2022-12-06 02:49:32.000000 ont-remora-2.0.0/src/remora/__init__.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2022-07-21 21:33:30.000000 ont-remora-2.0.0/src/remora/activations.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2688 2022-12-06 02:49:32.000000 ont-remora-2.0.0/src/remora/constants.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    56422 2022-12-03 19:07:12.000000 ont-remora-2.0.0/src/remora/data_chunks.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1350 2022-09-30 13:36:35.000000 ont-remora-2.0.0/src/remora/download.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3561 2022-10-25 18:47:18.000000 ont-remora-2.0.0/src/remora/duplex_utils.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2022-07-21 21:33:30.000000 ont-remora-2.0.0/src/remora/encoded_kmers.pyx
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    20147 2022-12-03 21:10:27.000000 ont-remora-2.0.0/src/remora/inference.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    28702 2022-12-03 21:10:27.000000 ont-remora-2.0.0/src/remora/io.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2388 2022-09-30 13:36:35.000000 ont-remora-2.0.0/src/remora/log.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1841 2022-09-30 13:36:35.000000 ont-remora-2.0.0/src/remora/main.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    20460 2022-10-18 22:35:00.000000 ont-remora-2.0.0/src/remora/model_util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    44169 2022-12-03 19:07:12.000000 ont-remora-2.0.0/src/remora/parsers.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     8660 2022-12-03 21:10:27.000000 ont-remora-2.0.0/src/remora/prepare_train_data.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    22854 2022-07-29 18:34:08.000000 ont-remora-2.0.0/src/remora/refine_signal_map.py
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18985 2022-08-30 23:02:50.000000 ont-remora-2.0.0/src/remora/refine_signal_map_core.pyx
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    13996 2022-09-30 13:36:35.000000 ont-remora-2.0.0/src/remora/train_model.py
-drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2022-12-06 03:06:31.513111 ont-remora-2.0.0/src/remora/trained_models/
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2022-09-30 13:36:35.000000 ont-remora-2.0.0/src/remora/trained_models/readme.rst
--rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    14622 2022-12-03 19:07:12.000000 ont-remora-2.0.0/src/remora/util.py
--rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    20700 2022-11-10 21:59:27.000000 ont-remora-2.0.0/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.788545 ont-remora-2.1.0/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    14471 2022-07-21 21:33:30.000000 ont-remora-2.1.0/LICENSE.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       45 2022-09-30 13:36:35.000000 ont-remora-2.1.0/MANIFEST.in
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    10741 2023-05-03 18:51:13.788630 ont-remora-2.1.0/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    10317 2023-03-28 22:16:30.000000 ont-remora-2.1.0/README.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      343 2022-07-21 21:33:30.000000 ont-remora-2.1.0/pyproject.toml
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1631 2023-05-03 18:51:13.789301 ont-remora-2.1.0/setup.cfg
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      791 2022-07-21 21:33:30.000000 ont-remora-2.1.0/setup.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.779819 ont-remora-2.1.0/src/
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.782312 ont-remora-2.1.0/src/ont_remora.egg-info/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    10741 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/PKG-INFO
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      939 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/SOURCES.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/dependency_links.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)       43 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/entry_points.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        1 2022-07-22 16:07:04.000000 ont-remora-2.1.0/src/ont_remora.egg-info/not-zip-safe
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      175 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/requires.txt
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)        7 2023-05-03 18:51:13.000000 ont-remora-2.1.0/src/ont_remora.egg-info/top_level.txt
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.787416 ont-remora-2.1.0/src/remora/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      127 2023-05-03 18:44:57.000000 ont-remora-2.1.0/src/remora/__init__.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      508 2022-07-21 21:33:30.000000 ont-remora-2.1.0/src/remora/activations.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2821 2023-03-17 13:40:19.000000 ont-remora-2.1.0/src/remora/constants.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    61354 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/data_chunks.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1670 2023-03-17 13:40:19.000000 ont-remora-2.1.0/src/remora/download.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3353 2023-04-03 18:17:26.000000 ont-remora-2.1.0/src/remora/duplex_utils.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     1484 2022-07-21 21:33:30.000000 ont-remora-2.1.0/src/remora/encoded_kmers.pyx
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    19661 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/inference.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    66346 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/io.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     2388 2022-09-30 13:36:35.000000 ont-remora-2.1.0/src/remora/log.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)     1896 2023-02-14 21:50:54.000000 ont-remora-2.1.0/src/remora/main.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     3839 2023-02-14 21:50:54.000000 ont-remora-2.1.0/src/remora/metrics.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    20462 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/model_util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    58171 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/parsers.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     7270 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/prepare_train_data.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    24777 2023-03-06 23:24:06.000000 ont-remora-2.1.0/src/remora/refine_signal_map.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    18990 2023-02-14 21:50:54.000000 ont-remora-2.1.0/src/remora/refine_signal_map_core.pyx
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    16130 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/train_model.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.787629 ont-remora-2.1.0/src/remora/trained_models/
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)      338 2022-09-30 13:36:35.000000 ont-remora-2.1.0/src/remora/trained_models/readme.rst
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    16314 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/util.py
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)    21001 2023-05-03 18:40:58.000000 ont-remora-2.1.0/src/remora/validate.py
+drwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)        0 2023-05-03 18:51:13.788391 ont-remora-2.1.0/tests/
+-rwxr-xr-x   0 Marcus.Stoiber   (503) staff       (20)      679 2022-09-30 13:36:35.000000 ont-remora-2.1.0/tests/test_coding_standards.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)    12174 2023-02-14 21:50:54.000000 ont-remora-2.1.0/tests/test_duplex.py
+-rw-r--r--   0 Marcus.Stoiber   (503) staff       (20)     8835 2023-05-03 18:40:58.000000 ont-remora-2.1.0/tests/test_main.py
```

### Comparing `ont-remora-2.0.0/LICENSE.txt` & `ont-remora-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ont-remora-2.0.0/PKG-INFO` & `ont-remora-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.0.0
+Version: 2.1.0
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
@@ -105,29 +105,36 @@
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
+Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
 
 .. code-block:: bash
 
   remora \
     dataset prepare \
-    can_signal.pod5 \
-    can_basecalls.bam \
+    can_reads.pod5 \
+    can_mappings.bam \
     --output-remora-training-file can_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
-   --mod-base-control
+    --mod-base-control
   remora \
     dataset prepare \
-    mod_signal.pod5 \
-    mod_basecalls.bam \
+    mod_reads.pod5 \
+    mod_mappings.bam \
     --output-remora-training-file mod_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
     --mod-base m 5mC
   remora \
     dataset merge \
     --input-dataset can_chunks.npz 10_000_000 \
     --input-dataset mod_chunks.npz 10_000_000 \
     --output-dataset chunks.npz
@@ -180,14 +187,76 @@
 
   remora \
     validate from_modbams \
     --bam-and-bed can_infer.bam can_ground_truth.bed \
     --bam-and-bed mod_infer.bam mod_ground_truth.bed \
     --full-output-filename validation_results.txt
 
+Raw Signal Analysis
+-------------------
+
+As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
+The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+Additional commands will be added to this group to produce more useful raw signal analysis tasks.
+
+The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
+
+As an example using the test data, the following command produces the plot below.
+
+.. code-block:: bash
+
+  remora \
+    analyze plot ref_region \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
+    --ref-regions ref_regions.bed \
+    --highlight-ranges mod_gt.bed \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --log-filename log.txt
+
+.. image:: images/plot_ref_region_fwd.png
+   :width: 600
+   :alt: Plot reference region image (forward strand)
+
+.. image:: images/plot_ref_region_rev.png
+   :width: 600
+   :alt: Plot reference region image (reverse strand)
+
+The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
+For each read, the mean level at each covered base is computed.
+Then for all reads covering a reference location the median of read levels is taken.
+These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
+The following command exemplifies this.
+
+.. code-block:: bash
+
+  remora \
+    analyze estimate_kmer_levels \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --kmer-context-bases 1 1 \
+    --min-coverage 3 \
+    --num-workers 8 \
+    --log-filename log.txt
+
+Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
+This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
+This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
+
+Raw Signal Analysis
+-------------------
+
+The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
+This is API is primarily accessed via the ``remora.io.Read`` object.
+
+The iPython notebooks included in this repository exemplify some common analyses.
+[TODO add notebooks to repo]
+
 Terms and Licence
 -----------------
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
```

### Comparing `ont-remora-2.0.0/README.rst` & `ont-remora-2.1.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -92,29 +92,36 @@
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
+Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
 
 .. code-block:: bash
 
   remora \
     dataset prepare \
-    can_signal.pod5 \
-    can_basecalls.bam \
+    can_reads.pod5 \
+    can_mappings.bam \
     --output-remora-training-file can_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
-   --mod-base-control
+    --mod-base-control
   remora \
     dataset prepare \
-    mod_signal.pod5 \
-    mod_basecalls.bam \
+    mod_reads.pod5 \
+    mod_mappings.bam \
     --output-remora-training-file mod_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
     --mod-base m 5mC
   remora \
     dataset merge \
     --input-dataset can_chunks.npz 10_000_000 \
     --input-dataset mod_chunks.npz 10_000_000 \
     --output-dataset chunks.npz
@@ -167,14 +174,76 @@
 
   remora \
     validate from_modbams \
     --bam-and-bed can_infer.bam can_ground_truth.bed \
     --bam-and-bed mod_infer.bam mod_ground_truth.bed \
     --full-output-filename validation_results.txt
 
+Raw Signal Analysis
+-------------------
+
+As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
+The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+Additional commands will be added to this group to produce more useful raw signal analysis tasks.
+
+The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
+
+As an example using the test data, the following command produces the plot below.
+
+.. code-block:: bash
+
+  remora \
+    analyze plot ref_region \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
+    --ref-regions ref_regions.bed \
+    --highlight-ranges mod_gt.bed \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --log-filename log.txt
+
+.. image:: images/plot_ref_region_fwd.png
+   :width: 600
+   :alt: Plot reference region image (forward strand)
+
+.. image:: images/plot_ref_region_rev.png
+   :width: 600
+   :alt: Plot reference region image (reverse strand)
+
+The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
+For each read, the mean level at each covered base is computed.
+Then for all reads covering a reference location the median of read levels is taken.
+These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
+The following command exemplifies this.
+
+.. code-block:: bash
+
+  remora \
+    analyze estimate_kmer_levels \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --kmer-context-bases 1 1 \
+    --min-coverage 3 \
+    --num-workers 8 \
+    --log-filename log.txt
+
+Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
+This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
+This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
+
+Raw Signal Analysis
+-------------------
+
+The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
+This is API is primarily accessed via the ``remora.io.Read`` object.
+
+The iPython notebooks included in this repository exemplify some common analyses.
+[TODO add notebooks to repo]
+
 Terms and Licence
 -----------------
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
```

### Comparing `ont-remora-2.0.0/setup.cfg` & `ont-remora-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 	toml
 	torch
 	numpy
 	scikit-learn
 	tabulate
 	thop
 	pandas
-	pod5 >= 0.0.43
+	pod5 >= 0.1.16
 	pysam >= 0.20.0
 	parasail
 	requests
+	matplotlib
+	seaborn
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
 	black==22.8.0
 	flake8
```

### Comparing `ont-remora-2.0.0/setup.py` & `ont-remora-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.0.0/src/ont_remora.egg-info/PKG-INFO` & `ont-remora-2.1.0/src/ont_remora.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-remora
-Version: 2.0.0
+Version: 2.1.0
 Summary: Nanopore methylation/modified base calling detached from basecalling
 Home-page: https://github.com/nanoporetech/remora
 License: ont_public_licence
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8; variant=GFM
@@ -105,29 +105,36 @@
 Data Preparation
 ----------------
 
 Remora data preparation begins from a POD5 file (containing signal data) and a BAM file containing basecalls from the POD5 file.
 Note that the BAM file must contain the move table (default in Bonito and ``--moves_out`` in Guppy).
 
 The following example generates training data from canonical (PCR) and modified (M.SssI treatment) samples in the same fashion as the releasd 5mC CG-context models.
+Example reads and kit14 level table can be found in the Remora respoitory in the  ``test/data/`` directory.
 
 .. code-block:: bash
 
   remora \
     dataset prepare \
-    can_signal.pod5 \
-    can_basecalls.bam \
+    can_reads.pod5 \
+    can_mappings.bam \
     --output-remora-training-file can_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
-   --mod-base-control
+    --mod-base-control
   remora \
     dataset prepare \
-    mod_signal.pod5 \
-    mod_basecalls.bam \
+    mod_reads.pod5 \
+    mod_mappings.bam \
     --output-remora-training-file mod_chunks.npz \
+    --log-filename prep_can.log \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
     --motif CG 0 \
     --mod-base m 5mC
   remora \
     dataset merge \
     --input-dataset can_chunks.npz 10_000_000 \
     --input-dataset mod_chunks.npz 10_000_000 \
     --output-dataset chunks.npz
@@ -180,14 +187,76 @@
 
   remora \
     validate from_modbams \
     --bam-and-bed can_infer.bam can_ground_truth.bed \
     --bam-and-bed mod_infer.bam mod_ground_truth.bed \
     --full-output-filename validation_results.txt
 
+Raw Signal Analysis
+-------------------
+
+As of version 2.1, Remora has made access to raw signal analysis more accessible via two CLI commands and an improved API.
+The ``remora analyze`` command group contains two commands ``plot ref_region`` and ``estimate_kmer_levels``.
+Additional commands will be added to this group to produce more useful raw signal analysis tasks.
+
+The ``plot ref_region`` command is useful for gaining intuition into signal attributes and visualize signal shifts around modified bases.
+
+As an example using the test data, the following command produces the plot below.
+
+.. code-block:: bash
+
+  remora \
+    analyze plot ref_region \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --pod5-and-bam mod_reads.pod5 mod_mappings.bam \
+    --ref-regions ref_regions.bed \
+    --highlight-ranges mod_gt.bed \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --log-filename log.txt
+
+.. image:: images/plot_ref_region_fwd.png
+   :width: 600
+   :alt: Plot reference region image (forward strand)
+
+.. image:: images/plot_ref_region_rev.png
+   :width: 600
+   :alt: Plot reference region image (reverse strand)
+
+The ``remora analyze estimate_kmer_levels`` command allows one to estimate the current level for each defined k-mer from the above signal.
+For each read, the mean level at each covered base is computed.
+Then for all reads covering a reference location the median of read levels is taken.
+These are grouped by kmer (defined by ``--kmer-context-bases``) and the median is taken over all occurences of each kmer to produce the output table.
+The following command exemplifies this.
+
+.. code-block:: bash
+
+  remora \
+    analyze estimate_kmer_levels \
+    --pod5-and-bam can_reads.pod5 can_mappings.bam \
+    --refine-kmer-level-table levels.txt \
+    --refine-rough-rescale \
+    --kmer-context-bases 1 1 \
+    --min-coverage 3 \
+    --num-workers 8 \
+    --log-filename log.txt
+
+Note that a reasonable starting kmer table is necessary to obtain reasonable output here.
+This command is only using 14 reads, so in practice ``--min-coverage`` should be >=10.
+This command is also only estimating a 3-mer model (``--kmer-context-bases 1 1``), so this can be increased on larger datasets for a more representative model.
+
+Raw Signal Analysis
+-------------------
+
+The new metrics API allows access to these per-read, per-site metrics for more advanced statistical analysis.
+This is API is primarily accessed via the ``remora.io.Read`` object.
+
+The iPython notebooks included in this repository exemplify some common analyses.
+[TODO add notebooks to repo]
+
 Terms and Licence
 -----------------
 
 This is a research release provided under the terms of the Oxford Nanopore Technologies' Public Licence.
 Research releases are provided as technology demonstrators to provide early access to features or stimulate Community development of tools.
 Support for this software will be minimal and is only provided directly by the developers. Feature requests, improvements, and discussions are welcome and can be implemented by forking and pull requests.
 Much as we would like to rectify every issue, the developers may have limited resource for support of this software.
```

### Comparing `ont-remora-2.0.0/src/ont_remora.egg-info/SOURCES.txt` & `ont-remora-2.1.0/src/ont_remora.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,20 @@
 src/remora/download.py
 src/remora/duplex_utils.py
 src/remora/encoded_kmers.pyx
 src/remora/inference.py
 src/remora/io.py
 src/remora/log.py
 src/remora/main.py
+src/remora/metrics.py
 src/remora/model_util.py
 src/remora/parsers.py
 src/remora/prepare_train_data.py
 src/remora/refine_signal_map.py
 src/remora/refine_signal_map_core.pyx
 src/remora/train_model.py
 src/remora/util.py
 src/remora/validate.py
-src/remora/trained_models/readme.rst
+src/remora/trained_models/readme.rst
+tests/test_coding_standards.py
+tests/test_duplex.py
+tests/test_main.py
```

### Comparing `ont-remora-2.0.0/src/remora/data_chunks.py` & `ont-remora-2.1.0/src/remora/data_chunks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import gc
 import re
+import os
 from collections import Counter
 from dataclasses import dataclass
-from typing import List, Tuple
 
 import torch
 import numpy as np
 from tqdm import tqdm
 
 from remora.refine_signal_map import SigMapRefiner
 from remora import constants, log, RemoraError, util, encoded_kmers
 
 LOGGER = log.get_logger()
 
-DEFAULT_BATCH_SIZE = 1024
 DATASET_VERSION = 2
 MISMATCH_ARRS = {
     0: np.array([1, 2, 3]),
     1: np.array([0, 2, 3]),
     2: np.array([0, 1, 3]),
     3: np.array([0, 1, 2]),
 }
 # CIGAR operations which correspond to query and reference sequence
 MATCH_OPS = np.array(
     [True, False, False, False, False, False, False, True, True]
 )
 QUERY_OPS = np.array([True, True, False, False, True, False, False, True, True])
-#                    ["M", "I",   "D",   "N", "S",   "H",    "P", "=", "X"]
 REF_OPS = np.array([True, False, True, True, False, False, False, True, True])
 CIGAR_CODES = ["M", "I", "D", "N", "S", "H", "P", "=", "X"]
 CODE_TO_OP = {
     "M": 0,
     "I": 1,
     "D": 2,
     "N": 3,
@@ -39,96 +37,95 @@
     "P": 6,
     "=": 7,
     "X": 8,
 }
 CIGAR_STRING_PATTERN = re.compile(r"(\d+)" + f"([{''.join(CIGAR_CODES)}])")
 
 
-def cigartuples_from_string(cigarstring: str) -> List[Tuple[int, int]]:
+def cigartuples_from_string(cigarstring):
     """
     Returns pysam-style list of (op, count) tuples from a cigarstring.
     """
     return [
         (CODE_TO_OP[m.group(2)], int(m.group(1)))
         for m in re.finditer(CIGAR_STRING_PATTERN, cigarstring)
     ]
 
 
-def map_ref_to_signal(
-    *, query_to_signal: np.ndarray, ref_to_query_knots: np.ndarray
-) -> np.ndarray:
+def map_ref_to_signal(*, query_to_signal, ref_to_query_knots):
+    """Compute interpolated mapping from reference, through query alignment to
+    signal coordinates
+
+    Args:
+        query_to_signal (np.array): Query to signal coordinate mapping
+        ref_to_query_knots (np.array): Reference to query coordinate mapping
+    """
     return np.floor(
         np.interp(
             ref_to_query_knots,
             np.arange(query_to_signal.size),
             query_to_signal,
         )
     ).astype(int)
 
 
-def compute_ref_to_signal(query_to_signal, cigar, *, query_seq, ref_seq):
-    ref_to_read_knots = make_sequence_coordinate_mapping(
-        cigar=cigar, read_seq=query_seq, ref_seq=ref_seq
-    )
-    return map_ref_to_signal(
-        query_to_signal=query_to_signal, ref_to_query_knots=ref_to_read_knots
-    )
-
+def make_sequence_coordinate_mapping(cigar):
+    """Maps an element in reference to every element in basecalls using
+    alignment in `cigar`.
 
-def make_sequence_coordinate_mapping(
-    cigar: list, *, read_seq: str, ref_seq: str
-) -> np.ndarray:
-    """
-    Maps an element in `read_seq` to every element in `ref_seq` using alignment
-    in `cigar`.
+    Args:
+        cigar (list): "cigartuples" representing alignment
 
-    :param cigar: "cigartuples" representing alignment
-    :param read_seq: a.k.a. query sequence
-    :param ref_seq: "aligned-to" reference sequence
-    :return: array shape (len(ref_seq),). [x_0, x_1, ..., x_(len(ref_seq))]
-             such that read_seq[x_i] <> ref_seq[i]
+    Returns:
+        array shape (ref_len,). [x_0, x_1, ..., x_(ref_len)]
+            such that read_seq[x_i] <> ref_seq[i]. Note that ref_len is derived
+            from the cigar input.
     """
     ops, lens = map(np.array, zip(*cigar))
-    ref_len = len(ref_seq)
-    read_len = len(read_seq)
+    assert ops.min() >= 0 and ops.max() <= 8, "invalid cigar op(s)"
+    assert lens.min() >= 0, "cigar lengths may not be negative"
 
     is_match = MATCH_OPS[ops]
     match_counts = lens[is_match]
     offsets = np.array([match_counts, np.ones_like(match_counts)])
 
+    # TODO remove knots around ambiguous indels (e.g. left justified HPs)
+    # note this requires the ref and query sequences
     ref_knots = np.cumsum(np.where(REF_OPS[ops], lens, 0))
     ref_knots = np.concatenate(
         [[0], (ref_knots[is_match] - offsets).T.flatten(), [ref_knots[-1]]]
     )
     query_knots = np.cumsum(np.where(QUERY_OPS[ops], lens, 0))
     query_knots = np.concatenate(
         [[0], (query_knots[is_match] - offsets).T.flatten(), [query_knots[-1]]]
     )
-    knots = np.interp(np.arange(ref_len + 1), ref_knots, query_knots).astype(
-        int
-    )
+    knots = np.interp(np.arange(ref_knots[-1] + 1), ref_knots, query_knots)
 
-    # +1 because knots include the end position of the last base
-    assert knots.shape[0] == ref_len + 1, "knots should be len(ref_seq) + 1"
-    assert (
-        np.max(knots[:-1]) < read_len
-    ), "knots map to position not contained in read"
+    return knots
 
-    assert np.min(knots) >= 0, "knots cannot be negative"
 
-    return knots
+def compute_ref_to_signal(query_to_signal, cigar):
+    ref_to_read_knots = make_sequence_coordinate_mapping(cigar)
+    assert query_to_signal.size == ref_to_read_knots[-1].astype(int) + 1, (
+        "discordant implied basecall lengths: move_table:"
+        f"{query_to_signal.size} cigar:{ref_to_read_knots[-1]}"
+    )
+    return map_ref_to_signal(
+        query_to_signal=query_to_signal, ref_to_query_knots=ref_to_read_knots
+    )
 
 
 @dataclass
 class RemoraRead:
     """Object to hold information about a read relevant to Remora training and
     inference.
 
     Args:
-        dacs (np.ndarray): Unnormalized DAC signal
+        dacs (np.ndarray): Unnormalized DAC signal. `dacs` should be reversed
+            already for reverse_signal data types.
         shift (float): Shift from dac to normalized signal. via formula:
             norm = (dac - shift) / scale
         scale (float): Scale from dac to normalized signal
         seq_to_sig_map (np.ndarray): Position within signal array assigned to
             each base in seq
         int_seq (np.ndarray): Encoded sequence for training/validation.
             See remora.util.seq_to_int
@@ -507,23 +504,18 @@
               1. Modified base predictions (dim: num_calls, num_mods + 1)
               2. Labels for each base (-1 if labels not provided)
               3. List of positions within the read
         """
         device = next(model.parameters()).device
         read_outputs, read_poss, read_labels = [], [], []
         for sigs, enc_kmers, labels, read_pos in self.batches:
-            read_outputs.append(
-                model.forward(
-                    sigs=torch.from_numpy(sigs).to(device),
-                    seqs=torch.from_numpy(enc_kmers).to(device),
-                )
-                .detach()
-                .cpu()
-                .numpy()
-            )
+            sigs = torch.from_numpy(sigs).to(device)
+            enc_kmers = torch.from_numpy(enc_kmers).to(device)
+            output = model(sigs, enc_kmers).detach().cpu().numpy()
+            read_outputs.append(output)
             read_labels.append(labels)
             read_poss.append(read_pos)
         read_outputs = np.concatenate(read_outputs, axis=0)
         read_labels = np.concatenate(read_labels)
         read_poss = np.concatenate(read_poss)
         return read_outputs, read_labels, read_poss
 
@@ -661,23 +653,26 @@
         kmer_context_bases (tuple): 2-tuple containing the bases to include in
             the encoded k-mer presented as input.
         base_pred (bool): Are labels predicting base? Default is mod_bases.
         mod_bases (str): Modified base single letter codes represented by labels
         mod_long_names (list): Modified base long names represented by labels
         motifs (list): Tuples containing sequence motifs and relative position.
             E.g. ("N", 0) for all-contexts or ("CG", 0) for CG-contexts.
+        reverse_signal (bool): Is nanopore signal 3' to 5' orientation?
+            Primarily for directRNA
         batch_size (int): Size of batches to be produced
         shuffle_on_iter (bool): Shuffle data before each iteration over batches
         drop_last (bool): Drop the last batch of each iteration
-        balanced_batch (bool): Balances each training batch
+        batch_label_props (np.array): Select proportion of each label
         sig_map_refiner (remora.refine_signal_map.SigMapRefiner): Signal
             mapping refiner
         base_start_justify (bool): Extract chunk centered on start of base
         offset (int): Extract chunk centered on base offset from base of
             interest
+        drop_read_attrs (bool): Drop read id and read focus positions
 
     Yields:
         Batches of data for training or inference
     """
 
     # data attributes
     sig_tensor: np.ndarray
@@ -693,28 +688,32 @@
     chunk_context: tuple = constants.DEFAULT_CHUNK_CONTEXT
     max_seq_len: int = None
     kmer_context_bases: tuple = constants.DEFAULT_KMER_CONTEXT_BASES
     base_pred: bool = False
     mod_bases: str = ""
     mod_long_names: list = None
     motifs: list = None
+    reverse_signal: bool = False
 
     # batch attributes (defaults set for training)
     batch_size: int = constants.DEFAULT_BATCH_SIZE
     shuffle_on_iter: bool = True
     drop_last: bool = True
-    balanced_batch: bool = False
+    batch_label_props: np.ndarray = None
 
     # signal mapping refinement params
     sig_map_refiner: SigMapRefiner = None
 
     # chunk extraction attributes
     base_start_justify: bool = False
     offset: int = 0
 
+    # extra attributes
+    drop_read_attrs: bool = False
+
     def set_nbatches(self):
         self.nbatches, remainder = divmod(self.nchunks, self.batch_size)
         if not self.drop_last and remainder > 0:
             self.nbatches += 1
 
     def __post_init__(self):
         if self.max_seq_len is None:
@@ -730,14 +729,19 @@
                 f"mod_long_names ({self.mod_long_names}) must be same length "
                 f"as mod_bases ({self.mod_bases})"
             )
         if self.motifs is not None:
             self.motifs = sorted(set(self.motifs))
         self.set_nbatches()
         self.shuffled = False
+        if self.drop_read_attrs:
+            self.read_ids = None
+            self.read_focus_bases = None
+            gc.collect()
+        self._class_ordered_indices = None
 
     def add_chunk(self, chunk):
         if self.nchunks >= self.labels.size:
             raise RemoraError("Cannot add chunk to currently allocated tensors")
         if chunk.seq_len > self.max_seq_len:
             raise RemoraError("Chunk sequence too long to store")
         self.sig_tensor[self.nchunks, 0] = chunk.signal
@@ -745,16 +749,17 @@
             self.nchunks, : chunk.seq_w_context.size
         ] = chunk.seq_w_context
         self.seq_mappings[
             self.nchunks, : chunk.seq_to_sig_map.size
         ] = chunk.seq_to_sig_map
         self.seq_lens[self.nchunks] = chunk.seq_len
         self.labels[self.nchunks] = chunk.label
-        self.read_ids[self.nchunks] = chunk.read_id
-        self.read_focus_bases[self.nchunks] = chunk.read_focus_base
+        if not self.drop_read_attrs:
+            self.read_ids[self.nchunks] = chunk.read_id
+            self.read_focus_bases[self.nchunks] = chunk.read_focus_base
         self.nchunks += 1
 
     def add_batch(
         self, b_sig, b_seq, b_ss_map, b_seq_lens, b_labels, b_rids, b_rfbs
     ):
         batch_size = b_labels.size
         b_st, b_en = self.nchunks, self.nchunks + batch_size
@@ -762,31 +767,33 @@
             raise RemoraError("Cannot add batch to currently allocated tensors")
         # TODO check that applicable dims are compatible
         self.sig_tensor[b_st:b_en] = b_sig
         self.seq_array[b_st:b_en] = b_seq
         self.seq_mappings[b_st:b_en] = b_ss_map
         self.seq_lens[b_st:b_en] = b_seq_lens
         self.labels[b_st:b_en] = b_labels
-        self.read_ids[b_st:b_en] = b_rids
-        self.read_focus_bases[b_st:b_en] = b_rfbs
+        if not self.drop_read_attrs:
+            self.read_ids[b_st:b_en] = b_rids
+            self.read_focus_bases[b_st:b_en] = b_rfbs
         self.nchunks += batch_size
 
     def clip_chunks(self):
         if self.nchunks == self.sig_tensor.shape[0]:
             self.set_nbatches()
             return
         elif self.nchunks > self.sig_tensor.shape[0]:
             raise RemoraError("More chunks indicated than provided.")
         self.sig_tensor = self.sig_tensor[: self.nchunks]
         self.seq_array = self.seq_array[: self.nchunks]
         self.seq_mappings = self.seq_mappings[: self.nchunks]
         self.seq_lens = self.seq_lens[: self.nchunks]
         self.labels = self.labels[: self.nchunks]
-        self.read_ids = self.read_ids[: self.nchunks]
-        self.read_focus_bases = self.read_focus_bases[: self.nchunks]
+        if not self.drop_read_attrs:
+            self.read_ids = self.read_ids[: self.nchunks]
+            self.read_focus_bases = self.read_focus_bases[: self.nchunks]
         # reset nbatches after clipping dataset
         self.set_nbatches()
 
     def trim_kmer_context_bases(self, new_kmer_context_bases):
         if new_kmer_context_bases is None:
             return
         if (
@@ -821,123 +828,249 @@
         ):
             raise RemoraError(
                 f"Cannot expand chunk_context (prev:{self.chunk_context} ; "
                 f"requested_new:{new_chunk_context})"
             )
         raise NotImplementedError("Cannot currently trim chunk context.")
 
+    def get_label_nchunks(self, target_nchunks):
+        """Get the number of chunks for each label most closely matching
+        specified batch_label_props,
+        """
+        if self.batch_label_props is None:
+            raise RemoraError("Must set batch_label_props to get label nchunks")
+        lab_nchunks = np.floor(target_nchunks * self.batch_label_props).astype(
+            int
+        )
+        while lab_nchunks.sum() < target_nchunks:
+            lab_nchunks[
+                np.argmin(
+                    (lab_nchunks / lab_nchunks.sum()) - self.batch_label_props
+                )
+            ] += 1
+        return lab_nchunks
+
+    def reorder_chunks(self, indices):
+        """Re-order chunks via specified indices"""
+        for attr in (
+            "sig_tensor",
+            "seq_array",
+            "seq_mappings",
+            "seq_lens",
+            "labels",
+        ):
+            setattr(self, attr, getattr(self, attr)[indices])
+            gc.collect()
+        if not self.drop_read_attrs:
+            self.read_ids = self.read_ids[indices]
+            self.read_focus_bases = self.read_focus_bases[indices]
+        gc.collect()
+
+    def order_chunks_by_batch_labels(self):
+        """Order chunks such that each slice of size self.batch_size includes
+        the specified proportion of each label. Also store the indices
+        cooresponding to each label to facilitate shuffling within each label
+        while maintaining specified batch balance.
+
+        Note that "extra" chunks are stored at the end of the dataset and will
+        be shuffled into the used portion of the dataset at each call to
+        shuffle_by_batch_labels.
+        """
+        class_indices = [
+            np.where(self.labels == class_label)[0]
+            for class_label in range(self.num_labels)
+        ]
+        batch_nchunks = self.get_label_nchunks(self.batch_size)
+        class_nbatches = [
+            ci.size // bnc for ci, bnc in zip(class_indices, batch_nchunks)
+        ]
+        # set to number of batches given smallest class size
+        self.nbatches = min(class_nbatches)
+        if self.nbatches < 1:
+            raise RemoraError("Ordering by batch labels produced no batches")
+        # set indices for each label within each batch
+        idx_starts = np.concatenate([[0], np.cumsum(batch_nchunks)])
+        class_extras = [
+            ci.size - (bnc * self.nbatches)
+            for ci, bnc in zip(class_indices, batch_nchunks)
+        ]
+        LOGGER.debug("Computing class order indices")
+        # store indcies for each class to order all chunks and save to shuffle
+        # within class each epoch
+        self._class_ordered_indices = []
+        extras_index = self.batch_size * self.nbatches
+        for lab in range(self.num_labels):
+            lab_b_rng = np.arange(idx_starts[lab], idx_starts[lab + 1])
+            self._class_ordered_indices.append(
+                np.concatenate(
+                    [
+                        lab_b_rng + (bn * self.batch_size)
+                        for bn in range(self.nbatches)
+                    ]
+                    + [
+                        np.arange(
+                            extras_index, extras_index + class_extras[lab]
+                        )
+                    ]
+                )
+            )
+            extras_index += class_extras[lab]
+        global_ordered_indices = np.empty(self.nchunks, dtype=int)
+        for ci, coi in zip(class_indices, self._class_ordered_indices):
+            global_ordered_indices[coi] = ci
+        gc.collect()
+        LOGGER.debug("Reordering chunks")
+        # order each tensor to batch ordering
+        self.reorder_chunks(global_ordered_indices)
+
+    def shuffle_by_batch_labels(self):
+        if self._class_ordered_indices is None:
+            raise RemoraError(
+                "Must run order_chunks_by_batch_labels before "
+                "shuffle_by_batch_labels"
+            )
+        global_ordered_indices = np.empty(self.nchunks, dtype=int)
+        for coi in self._class_ordered_indices:
+            global_ordered_indices[coi] = np.random.permutation(coi)
+        self.reorder_chunks(global_ordered_indices)
+        self.shuffled = True
+
     def shuffle(self):
         if not self.is_clipped:
             raise RemoraError("Cannot shuffle an unclipped dataset.")
+        if self.batch_label_props is not None:
+            raise RemoraError(
+                "Cannot shuffle dataset with batch_label_props. "
+                "Use shuffle_by_batch_labels"
+            )
         shuf_idx = np.random.permutation(self.nchunks)
-        self.sig_tensor = self.sig_tensor[shuf_idx]
-        self.seq_array = self.seq_array[shuf_idx]
-        self.seq_mappings = self.seq_mappings[shuf_idx]
-        self.seq_lens = self.seq_lens[shuf_idx]
-        self.labels = self.labels[shuf_idx]
-        self.read_ids = self.read_ids[shuf_idx]
-        self.read_focus_bases = self.read_focus_bases[shuf_idx]
+        self.reorder_chunks(shuf_idx)
         self.shuffled = True
 
+    def clone_metadata(self):
+        return {
+            "chunk_context": self.chunk_context,
+            "max_seq_len": self.max_seq_len,
+            "kmer_context_bases": self.kmer_context_bases,
+            "base_pred": self.base_pred,
+            "mod_bases": self.mod_bases,
+            "mod_long_names": self.mod_long_names,
+            "motifs": self.motifs,
+            "reverse_signal": self.reverse_signal,
+            "batch_size": self.batch_size,
+            "sig_map_refiner": self.sig_map_refiner,
+            "offset": self.offset,
+            "base_start_justify": self.base_start_justify,
+        }
+
     def head(
-        self, nchunks=None, prop=0.01, shuffle_on_iter=False, drop_last=False
+        self,
+        nchunks=None,
+        prop=0.01,
+        shuffle_on_iter=False,
+        drop_last=False,
+        stratified=False,
     ):
         if nchunks is None:
             nchunks = int(prop * self.nchunks)
+        read_ids = read_focus_bases = None
+        if stratified:
+            LOGGER.debug("Performing stratified head")
+            head_indices = []
+            for class_label in range(self.num_labels):
+                class_indices = np.where(self.labels == class_label)[0]
+                if class_indices.size == 0:
+                    continue
+                cls_val_idx = int(class_indices.size * nchunks / self.nchunks)
+                head_indices.append(class_indices[:cls_val_idx])
+
+            head_indices = np.concatenate(head_indices)
+            if not self.drop_read_attrs:
+                read_ids = self.read_ids[head_indices].copy()
+                read_focus_bases = self.read_focus_bases[head_indices].copy()
+            return RemoraDataset(
+                self.sig_tensor[head_indices].copy(),
+                self.seq_array[head_indices].copy(),
+                self.seq_mappings[head_indices].copy(),
+                self.seq_lens[head_indices].copy(),
+                self.labels[head_indices].copy(),
+                read_ids,
+                read_focus_bases,
+                shuffle_on_iter=shuffle_on_iter,
+                drop_last=drop_last,
+                drop_read_attrs=self.drop_read_attrs,
+                **self.clone_metadata(),
+            )
+
+        if not self.drop_read_attrs:
+            read_ids = self.read_ids[:nchunks].copy()
+            read_focus_bases = self.read_focus_bases[:nchunks].copy()
         return RemoraDataset(
             self.sig_tensor[:nchunks].copy(),
             self.seq_array[:nchunks].copy(),
             self.seq_mappings[:nchunks].copy(),
             self.seq_lens[:nchunks].copy(),
             self.labels[:nchunks].copy(),
-            self.read_ids[:nchunks].copy(),
-            self.read_focus_bases[:nchunks].copy(),
+            read_ids,
+            read_focus_bases,
             shuffle_on_iter=shuffle_on_iter,
             drop_last=drop_last,
-            chunk_context=self.chunk_context,
-            max_seq_len=self.max_seq_len,
-            kmer_context_bases=self.kmer_context_bases,
-            base_pred=self.base_pred,
-            mod_bases=self.mod_bases,
-            mod_long_names=self.mod_long_names,
-            motifs=self.motifs,
-            batch_size=self.batch_size,
-            sig_map_refiner=self.sig_map_refiner,
+            drop_read_attrs=self.drop_read_attrs,
+            **self.clone_metadata(),
         )
 
     def copy(self):
+        read_ids = read_focus_bases = None
+        if not self.drop_read_attrs:
+            read_ids = self.read_ids.copy()
+            read_focus_bases = self.read_focus_bases.copy()
         return RemoraDataset(
             self.sig_tensor.copy(),
             self.seq_array.copy(),
             self.seq_mappings.copy(),
             self.seq_lens.copy(),
             self.labels.copy(),
-            self.read_ids.copy(),
-            self.read_focus_bases.copy(),
+            read_ids,
+            read_focus_bases,
             shuffle_on_iter=self.shuffle_on_iter,
             drop_last=self.drop_last,
-            chunk_context=self.chunk_context,
-            max_seq_len=self.max_seq_len,
-            kmer_context_bases=self.kmer_context_bases,
-            base_pred=self.base_pred,
-            mod_bases=self.mod_bases,
-            mod_long_names=self.mod_long_names,
-            motifs=self.motifs,
-            batch_size=self.batch_size,
+            **self.clone_metadata(),
         )
 
     def __iter__(self):
-        if self.shuffle_on_iter:
+        if self.batch_label_props is not None:
+            self.shuffle_by_batch_labels()
+        elif self.shuffle_on_iter:
             self.shuffle()
         self._batch_i = 0
         return self
 
     def __next__(self):
         if self._batch_i >= self.nbatches:
             raise StopIteration
         self._batch_i += 1
-        if self.balanced_batch:
-            batch_ids = []
-            for class_label in range(self.num_labels):
-                class_indices = np.where(self.labels == class_label)[0]
-                size = int(self.batch_size / self.num_labels)
-                bi = np.random.choice(
-                    len(class_indices), size=size, replace=False
-                )
-                batch_ids.extend(class_indices[bi])
-            return (
-                (
-                    self.sig_tensor[batch_ids],
-                    self.seq_array[batch_ids],
-                    self.seq_mappings[batch_ids],
-                    self.seq_lens[batch_ids],
-                ),
-                self.labels[batch_ids],
-                (
-                    self.read_ids[batch_ids],
-                    self.read_focus_bases[batch_ids],
-                ),
-            )
-
-        else:
-            b_st = (self._batch_i - 1) * self.batch_size
-            b_en = b_st + self.batch_size
-            return (
-                (
-                    self.sig_tensor[b_st:b_en],
-                    self.seq_array[b_st:b_en],
-                    self.seq_mappings[b_st:b_en],
-                    self.seq_lens[b_st:b_en],
-                ),
-                self.labels[b_st:b_en],
-                (
-                    self.read_ids[b_st:b_en],
-                    self.read_focus_bases[b_st:b_en],
-                ),
-            )
+        b_st = (self._batch_i - 1) * self.batch_size
+        b_en = b_st + self.batch_size
+        read_ids = read_focus_bases = None
+        if not self.drop_read_attrs:
+            read_ids = self.read_ids[b_st:b_en]
+            read_focus_bases = self.read_focus_bases[b_st:b_en]
+        return (
+            (
+                self.sig_tensor[b_st:b_en],
+                self.seq_array[b_st:b_en],
+                self.seq_mappings[b_st:b_en],
+                self.seq_lens[b_st:b_en],
+            ),
+            self.labels[b_st:b_en],
+            (
+                read_ids,
+                read_focus_bases,
+            ),
+        )
 
     def __len__(self):
         return self.nbatches
 
     def get_label_counts(self):
         return Counter(self.labels[: self.nchunks])
 
@@ -965,44 +1098,20 @@
             if val_prop < 0:
                 raise RemoraError("val_prop < 0")
             val_num = int(self.nchunks * val_prop)
         if val_num > self.nchunks:
             raise RemoraError("Too many validation chunks for split")
         if val_num > self.nchunks // 2:
             LOGGER.warning("Val split contains more than half of chunks")
-        common_kwargs = {
-            "chunk_context": self.chunk_context,
-            "max_seq_len": self.max_seq_len,
-            "kmer_context_bases": self.kmer_context_bases,
-            "base_pred": self.base_pred,
-            "mod_bases": self.mod_bases,
-            "mod_long_names": self.mod_long_names,
-            "motifs": self.motifs,
-            "batch_size": self.batch_size,
-            "sig_map_refiner": self.sig_map_refiner,
-        }
+
         if not self.shuffled:
             self.shuffle()
 
-        if self.balanced_batch:
-            val_indices = []
-            trn_indices = []
-            class_counts = np.unique(self.labels, return_counts=True)
-            min_class_id = np.argmin(class_counts[1])
-            for class_label in range(self.num_labels):
-                class_indices = np.where(self.labels == class_label)[0]
-                if class_indices.size == 0:
-                    continue
-                np.random.shuffle(class_indices)
-                cls_val_idx = int(
-                    class_counts[1][min_class_id] * val_num / self.nchunks
-                )
-                val_indices.extend(class_indices[:cls_val_idx])
-                trn_indices.extend(class_indices[cls_val_idx:])
-        elif stratified:
+        if stratified:
+            LOGGER.debug("Performing stratified split")
             val_indices = []
             trn_indices = []
             for class_label in range(self.num_labels):
                 class_indices = np.where(self.labels == class_label)[0]
                 if class_indices.size == 0:
                     continue
                 np.random.shuffle(class_indices)
@@ -1012,38 +1121,50 @@
 
             val_indices = np.concatenate(val_indices)
             trn_indices = np.concatenate(trn_indices)
         else:
             val_indices = np.arange(0, val_num)
             trn_indices = np.arange(val_num, self.sig_tensor.shape[0])
 
+        LOGGER.debug("Extracting validation dataset")
+        val_read_ids = val_read_focus_bases = None
+        if not self.drop_read_attrs:
+            val_read_ids = self.read_ids[val_indices]
+            val_read_focus_bases = self.read_focus_bases[val_indices]
         val_ds = RemoraDataset(
             self.sig_tensor[val_indices],
             self.seq_array[val_indices],
             self.seq_mappings[val_indices],
             self.seq_lens[val_indices],
             self.labels[val_indices],
-            self.read_ids[val_indices],
-            self.read_focus_bases[val_indices],
+            val_read_ids,
+            val_read_focus_bases,
             shuffle_on_iter=False,
             drop_last=False,
-            **common_kwargs,
+            drop_read_attrs=self.drop_read_attrs,
+            **self.clone_metadata(),
         )
+        LOGGER.debug("Extracting train dataset")
+        trn_read_ids = trn_read_focus_bases = None
+        if not self.drop_read_attrs:
+            trn_read_ids = self.read_ids[trn_indices]
+            trn_read_focus_bases = self.read_focus_bases[trn_indices]
         trn_ds = RemoraDataset(
             self.sig_tensor[trn_indices],
             self.seq_array[trn_indices],
             self.seq_mappings[trn_indices],
             self.seq_lens[trn_indices],
             self.labels[trn_indices],
-            self.read_ids[trn_indices],
-            self.read_focus_bases[trn_indices],
+            trn_read_ids,
+            trn_read_focus_bases,
             shuffle_on_iter=True,
             drop_last=False,
-            balanced_batch=self.balanced_batch,
-            **common_kwargs,
+            drop_read_attrs=self.drop_read_attrs,
+            batch_label_props=self.batch_label_props,
+            **self.clone_metadata(),
         )
         return trn_ds, val_ds
 
     def split_by_label(self):
         if self.base_pred:
             labels = "ACGT"
         else:
@@ -1056,27 +1177,23 @@
                     label,
                     RemoraDataset(
                         self.sig_tensor[label_indices],
                         self.seq_array[label_indices],
                         self.seq_mappings[label_indices],
                         self.seq_lens[label_indices],
                         self.labels[label_indices],
-                        self.read_ids[label_indices],
-                        self.read_focus_bases[label_indices],
+                        None
+                        if self.drop_read_attrs
+                        else self.read_ids[label_indices],
+                        None
+                        if self.drop_read_attrs
+                        else self.read_focus_bases[label_indices],
                         shuffle_on_iter=False,
                         drop_last=False,
-                        chunk_context=self.chunk_context,
-                        max_seq_len=self.max_seq_len,
-                        kmer_context_bases=self.kmer_context_bases,
-                        base_pred=self.base_pred,
-                        mod_bases=self.mod_bases,
-                        mod_long_names=self.mod_long_names,
-                        motifs=self.motifs,
-                        batch_size=self.batch_size,
-                        sig_map_refiner=self.sig_map_refiner,
+                        **self.clone_metadata(),
                     ),
                 )
             )
         return label_datasets
 
     def balance_classes(self):
         min_class_len = min(self.get_label_counts().values())
@@ -1098,51 +1215,38 @@
 
         return RemoraDataset(
             sig_tensor=self.sig_tensor[choices],
             seq_array=self.seq_array[choices],
             seq_mappings=self.seq_mappings[choices],
             seq_lens=self.seq_lens[choices],
             labels=self.labels[choices],
-            read_ids=self.read_ids[choices],
-            read_focus_bases=self.read_focus_bases[choices],
+            read_ids=None if self.drop_read_attrs else self.read_ids[choices],
+            read_focus_bases=None
+            if self.drop_read_attrs
+            else self.read_focus_bases[choices],
             nchunks=outs * min_class_len,
-            chunk_context=self.chunk_context,
-            max_seq_len=self.max_seq_len,
-            kmer_context_bases=self.kmer_context_bases,
-            base_pred=self.base_pred,
-            mod_bases=self.mod_bases,
-            mod_long_names=self.mod_long_names,
-            motifs=self.motifs,
-            sig_map_refiner=self.sig_map_refiner,
+            **self.clone_metadata(),
         )
 
     def filter(self, indices):
         if len(indices) > self.sig_tensor.shape[0]:
             raise RemoraError(
                 "Filter indices cannot be longer than dataset size"
             )
         return RemoraDataset(
             self.sig_tensor[indices],
             self.seq_array[indices],
             self.seq_mappings[indices],
             self.seq_lens[indices],
             self.labels[indices],
-            self.read_ids[indices],
-            self.read_focus_bases[indices],
+            None if self.drop_read_attrs else self.read_ids[indices],
+            None if self.drop_read_attrs else self.read_focus_bases[indices],
             shuffle_on_iter=False,
             drop_last=False,
-            chunk_context=self.chunk_context,
-            max_seq_len=self.max_seq_len,
-            kmer_context_bases=self.kmer_context_bases,
-            base_pred=self.base_pred,
-            mod_bases=self.mod_bases,
-            mod_long_names=self.mod_long_names,
-            motifs=self.motifs,
-            batch_size=self.batch_size,
-            sig_map_refiner=self.sig_map_refiner,
+            **self.clone_metadata(),
         )
 
     def add_fake_base(self, new_mod_long_names, new_mod_bases):
         if not set(self.mod_long_names).issubset(new_mod_long_names):
             raise RemoraError(
                 "There are no mods in common between the model being trained "
                 f"({new_mod_long_names}) and the external validation set "
@@ -1160,23 +1264,26 @@
         np.savez(
             filename,
             sig_tensor=self.sig_tensor,
             seq_array=self.seq_array,
             seq_mappings=self.seq_mappings,
             seq_lens=self.seq_lens,
             labels=self.labels,
-            read_ids=self.read_ids,
-            read_focus_bases=self.read_focus_bases,
+            read_ids=None if self.drop_read_attrs else self.read_ids,
+            read_focus_bases=None
+            if self.drop_read_attrs
+            else self.read_focus_bases,
             chunk_context=self.chunk_context,
             kmer_context_bases=self.kmer_context_bases,
             base_pred=self.base_pred,
             mod_bases=self.mod_bases,
             mod_long_names=self.mod_long_names,
             motifs=[mot[0] for mot in self.motifs],
             motif_offset=[mot[1] for mot in self.motifs],
+            reverse_signal=int(self.reverse_signal),
             base_start_justify=int(self.base_start_justify),
             offset=self.offset,
             version=DATASET_VERSION,
             **self.sig_map_refiner.get_save_kwargs(),
         )
 
     @classmethod
@@ -1212,14 +1319,16 @@
                 (mot, mot_off)
                 for mot, mot_off in zip(
                     data["motifs"].tolist(), data["motif_offset"].tolist()
                 )
             ]
         sig_map_refiner = SigMapRefiner.load_from_np_savez(data)
         base_start_justify = bool(int(data["base_start_justify"].item()))
+        # default to reverse_signal=False for datasets without this attribute
+        reverse_signal = bool(int(data.get("reverse_signal", 0)))
         offset = int(data["offset"].item())
         return cls(
             data["sig_tensor"],
             data["seq_array"],
             data["seq_mappings"],
             data["seq_lens"],
             data["labels"],
@@ -1227,14 +1336,15 @@
             data["read_focus_bases"],
             chunk_context=chunk_context,
             kmer_context_bases=kmer_context_bases,
             base_pred=base_pred,
             mod_bases=mod_bases,
             mod_long_names=mod_long_names,
             motifs=motifs,
+            reverse_signal=reverse_signal,
             sig_map_refiner=sig_map_refiner,
             base_start_justify=base_start_justify,
             offset=offset,
             *args,
             **kwargs,
         )
 
@@ -1242,14 +1352,15 @@
         errs_added = 0
         for c_idx, c_num_mm in tqdm(
             enumerate(np.random.binomial(self.seq_lens, mm_rate)),
             smoothing=0,
             total=self.nchunks,
             desc="Mismatches",
             leave=False,
+            disable=os.environ.get("LOG_SAFE", False),
         ):
             if c_num_mm == 0:
                 continue
             for seq_pos in np.random.choice(
                 self.seq_lens[c_idx], c_num_mm, replace=False
             ):
                 # convert from position in chunk sequence to position in
@@ -1266,14 +1377,15 @@
     def perturb_seq_to_sig_map(self, sig_shift):
         for c_idx, c_seq_len in tqdm(
             enumerate(self.seq_lens),
             smoothing=0,
             total=self.nchunks,
             desc="Signal shifts",
             leave=False,
+            disable=os.environ.get("LOG_SAFE", False),
         ):
             # shift seq to sig mapping in the middle of chunk
             self.seq_mappings[c_idx, 1:c_seq_len] = np.clip(
                 self.seq_mappings[c_idx, 1:c_seq_len] + sig_shift,
                 self.seq_mappings[c_idx, 0],
                 self.seq_mappings[c_idx, c_seq_len],
             )
@@ -1307,14 +1419,15 @@
             f"       label distribution : {self.get_label_counts()}\n"
             f"                base_pred : {self.base_pred}\n"
             f"                mod_bases : {self.mod_bases}\n"
             f"           mod_long_names : {self.mod_long_names}\n"
             f"       kmer_context_bases : {self.kmer_context_bases}\n"
             f"            chunk_context : {self.chunk_context}\n"
             f"                   motifs : {self.motifs}\n"
+            f"           reverse_signal : {self.reverse_signal}\n"
             f" chunk_extract_base_start : {self.base_start_justify}\n"
             f"     chunk_extract_offset : {self.offset}\n"
             f"          sig_map_refiner : {self.sig_map_refiner}\n"
         )
 
     def __repr__(self):
         return self.summary
@@ -1371,15 +1484,15 @@
 def merge_datasets(input_datasets, balance=False, quiet=False):
     def load_dataset(ds_path, num_chunks):
         dataset = RemoraDataset.load_from_file(
             ds_path,
             shuffle_on_iter=False,
             drop_last=False,
         )
-        if num_chunks < dataset.nchunks:
+        if num_chunks is not None and num_chunks < dataset.nchunks:
             dataset.shuffle()
         else:
             num_chunks = dataset.nchunks
         return dataset, num_chunks
 
     log_fp = LOGGER.debug if quiet else LOGGER.info
 
@@ -1388,14 +1501,15 @@
     base_pred = dataset.base_pred
     chunk_context = dataset.chunk_context
     max_seq_len = dataset.max_seq_len
     kmer_context_bases = dataset.kmer_context_bases
     motifs = set(dataset.motifs)
     sig_map_refiner = dataset.sig_map_refiner
     base_start_justify = dataset.base_start_justify
+    reverse_signal = dataset.reverse_signal
     offset = dataset.offset
     raw_mod_long_names = []
     raw_mod_bases = []
     if not base_pred:
         for mod_base, mln in zip(dataset.mod_bases, dataset.mod_long_names):
             if mod_base not in raw_mod_bases:
                 raw_mod_bases.append(mod_base)
@@ -1451,14 +1565,15 @@
         chunk_context=chunk_context,
         max_seq_len=max_seq_len,
         kmer_context_bases=kmer_context_bases,
         base_pred=base_pred,
         mod_bases=all_mod_bases,
         mod_long_names=all_mod_long_names,
         motifs=motifs,
+        reverse_signal=reverse_signal,
         sig_map_refiner=sig_map_refiner,
         base_start_justify=base_start_justify,
         offset=offset,
     )
     LOGGER.info(f"Output dataset summary:\n{output_dataset.summary}")
     for ds_path, num_chunks in input_datasets:
         input_dataset, num_chunks = load_dataset(ds_path, num_chunks)
@@ -1499,15 +1614,14 @@
             )
         log_fp(
             f"Copied {added_chunks} chunks. New label distribution: "
             f"{output_dataset.get_label_counts()}"
         )
         del input_dataset
         gc.collect()
-
     output_dataset.clip_chunks()
     if balance:
         balanced_dataset = output_dataset.balance_classes()
         log_fp(
             f"Balanced out to {balanced_dataset.sig_tensor.shape[0]} chunks. "
             f"New label distribution: {balanced_dataset.get_label_counts()}"
         )
```

### Comparing `ont-remora-2.0.0/src/remora/duplex_utils.py` & `ont-remora-2.1.0/src/remora/duplex_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,28 +94,22 @@
     trimmed_duplex_seq: str
     duplex_offset: int
 
 
 def map_simplex_to_duplex(*, simplex_seq: str, duplex_seq: str):
     pairwise_alignment = parasail_align(query=simplex_seq, ref=duplex_seq)
 
-    trimmed_simplex = simplex_seq[
-        pairwise_alignment.query_start : pairwise_alignment.query_end
-    ]
     trimmed_duplex = duplex_seq[
         pairwise_alignment.ref_start : pairwise_alignment.ref_end
     ]
-    duplex_to_simplex_mapping = DC.make_sequence_coordinate_mapping(
-        pairwise_alignment.cigar,
-        read_seq=trimmed_simplex,
-        ref_seq=trimmed_duplex,
-    )
-
     duplex_to_simplex_mapping = (
-        duplex_to_simplex_mapping + pairwise_alignment.query_start
+        DC.make_sequence_coordinate_mapping(
+            pairwise_alignment.cigar,
+        ).astype(int)
+        + pairwise_alignment.query_start
     )
 
     return SimplexDuplexMapping(
         duplex_to_simplex_mapping=duplex_to_simplex_mapping,
         trimmed_duplex_seq=trimmed_duplex,
         duplex_offset=pairwise_alignment.ref_start,
     )
```

### Comparing `ont-remora-2.0.0/src/remora/encoded_kmers.pyx` & `ont-remora-2.1.0/src/remora/encoded_kmers.pyx`

 * *Files identical despite different names*

### Comparing `ont-remora-2.0.0/src/remora/inference.py` & `ont-remora-2.1.0/src/remora/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import os
 import itertools
 from copy import copy
 import array as pyarray
 from pathlib import Path
-from typing import Tuple, Any
 from collections import defaultdict
 
 import pod5
 import pysam
 import numpy as np
 from tqdm import tqdm
 from torch.jit._script import RecursiveScriptModule
 
 from remora import constants, log, RemoraError
 from remora.io import (
-    index_bam,
+    ReadIndexedBam,
     iter_signal,
-    prep_extract_alignments,
     extract_alignments,
     DuplexRead,
-    Read as IoRead,
     DuplexPairsBuilder,
 )
 from remora.util import (
     MultitaskMap,
     BackgroundIter,
     format_mm_ml_tags,
     softmax_axis1,
+    get_read_ids,
     Motif,
     revcomp,
 )
 
 LOGGER = log.get_logger()
 _PROF_PREP_FN = os.getenv("REMORA_INFER_PREP_DATA_PROFILE_FILE")
 _PROF_MODEL_FN = os.getenv("REMORA_INFER_RUN_MODEL_PROFILE_FILE")
@@ -215,15 +213,15 @@
             continue
         motifs = [Motif(*mot) for mot in model_metadata["motifs"]]
         remora_read.set_motif_focus_bases(motifs)
         remora_read.prepare_batches(model_metadata, batch_size)
         if len(remora_read.batches) == 0:
             out_read_errs.append((None, None, "No mod calls"))
             continue
-        out_read_errs.append((copy(io_read), remora_read, None))
+        out_read_errs.append((io_read, remora_read, None))
     return out_read_errs
 
 
 if _PROF_PREP_FN:
     _prepare_batches_wrapper = prepare_batches
 
     def prepare_batches(*args, **kwargs):
@@ -259,15 +257,15 @@
             if not (tag.startswith("MM") or tag.startswith("ML"))
         ]
         io_read.full_align["tags"].extend(mod_tags)
         if ref_anchored:
             io_read.full_align["cigar"] = f"{len(io_read.ref_seq)}M"
             io_read.full_align["seq"] = (
                 io_read.ref_seq
-                if io_read.ref_pos.strand == "+"
+                if io_read.ref_reg.strand == "+"
                 else revcomp(io_read.ref_seq)
             )
             io_read.full_align["qual"] = "*"
         out_read_errs.append((io_read, None))
     return out_read_errs
 
 
@@ -286,104 +284,86 @@
 def infer_from_pod5_and_bam(
     pod5_path,
     in_bam_path,
     model,
     model_metadata,
     out_bam_path,
     num_reads=None,
+    queue_max=1_000,
     num_extract_alignment_workers=1,
     num_prep_batch_workers=1,
-    num_infer_workers=1,
     batch_size=constants.DEFAULT_BATCH_SIZE,
     skip_non_primary=True,
     ref_anchored=False,
 ):
-    bam_idx, num_bam_reads = index_bam(in_bam_path, skip_non_primary)
+    bam_idx = ReadIndexedBam(in_bam_path, skip_non_primary, req_tags={"mv"})
     with pod5.Reader(Path(pod5_path)) as pod5_fh:
-        pod5_read_ids = set((str(read.read_id) for read in pod5_fh.reads()))
-        # pod5 will raise when it cannot find a "selected" read id, so we make
-        # sure they're all present before starting
-        # todo(arand) this could be performed using the read_table instead, but
-        #  it's worth checking that it's actually faster and doesn't explode
-        #  memory before switching from a sweep throug the pod5 file
-        pod5_bam_read_id_intersection = list(
-            set(bam_idx.keys()).intersection(pod5_read_ids)
-        )
-        num_pod5_reads = len(pod5_bam_read_id_intersection)
-        LOGGER.info(
-            f"Found {num_bam_reads} BAM records and "
-            f"{num_pod5_reads} POD5 reads"
-        )
-        if num_reads is None:
-            num_reads = num_pod5_reads
-        else:
-            num_reads = min(num_reads, num_pod5_reads)
+        read_ids, num_reads = get_read_ids(bam_idx, pod5_fh, num_reads)
 
     signals = BackgroundIter(
         iter_signal,
-        args=(pod5_path, num_reads, pod5_bam_read_id_intersection),
+        args=(pod5_path,),
+        kwargs={
+            "num_reads": num_reads,
+            "read_ids": read_ids,
+            "rev_sig": model_metadata["reverse_signal"],
+        },
         name="ExtractSignal",
         use_process=True,
+        q_maxsize=queue_max,
     )
     reads = MultitaskMap(
         extract_alignments,
         signals,
-        prep_func=prep_extract_alignments,
         num_workers=num_extract_alignment_workers,
-        args=(bam_idx, in_bam_path),
-        kwargs={"req_tags": {"mv"}},
+        args=(bam_idx, model_metadata["reverse_signal"]),
         name="AddAlignments",
         use_process=True,
+        q_maxsize=queue_max,
     )
     reads = MultitaskMap(
         prepare_batches,
         reads,
         num_workers=num_prep_batch_workers,
         args=(model_metadata, batch_size, ref_anchored),
         name="PrepBatches",
         use_process=True,
-    )
-
-    use_process = True
-    if isinstance(model, RecursiveScriptModule):
-        use_process = next(model.parameters()).device.type == "cpu"
-
-    mod_reads_mappings = MultitaskMap(
-        run_model,
-        reads,
-        num_workers=num_infer_workers,
-        args=(model, model_metadata, ref_anchored),
-        name="InferMods",
-        use_process=use_process,
+        q_maxsize=queue_max,
     )
 
     errs = defaultdict(int)
     pysam_save = pysam.set_verbosity(0)
     sig_called = 0
     in_bam = out_bam = pbar = None
     try:
         in_bam = pysam.AlignmentFile(in_bam_path, "rb")
         out_bam = pysam.AlignmentFile(out_bam_path, "wb", template=in_bam)
         pbar = tqdm(
             smoothing=0,
             total=num_reads,
             unit=" Reads",
             desc="Inferring mods",
+            disable=os.environ.get("LOG_SAFE", False),
         )
-        for read_errs in mod_reads_mappings:
+        # TODO add a batch -> run_model -> unbatch function here to run model
+        # more efficiently on larger batch size
+        for read_errs in reads:
             pbar.update()
             if len(read_errs) == 0:
                 errs["No valid mappings"] += 1
                 continue
 
             sig_called += sum(
-                read.signal.size for read, _ in read_errs if read is not None
+                read.dacs.size for read, _, _ in read_errs if read is not None
             )
             msps = sig_called / 1_000_000 / pbar.format_dict["elapsed"]
             pbar.set_postfix_str(f"{msps:.2f} Msamps/s", refresh=False)
+            read_errs = run_model(
+                read_errs, model, model_metadata, ref_anchored
+            )
 
             for io_read, err in read_errs:
                 if io_read is None:
                     errs[err] += 1
                     continue
                 out_bam.write(
                     pysam.AlignedSegment.from_dict(
@@ -413,22 +393,27 @@
 
         prof = cProfile.Profile()
         retval = prof.runcall(_infer_from_pod5_and_bam_wrapper, *args, **kwargs)
         prof.dump_stats(_PROF_MAIN_FN)
         return retval
 
 
-def check_simplex_alignments(
-    *, simplex_index: dict, duplex_index: dict, pairs: list
-):
+def check_simplex_alignments(*, simplex_index, duplex_index, pairs):
+    """Check that valid pairs are found
+
+    Args:
+        simplex_index (ReadIndexedBam): Simplex basecalls bam index
+        duplex_index (ReadIndexedBam): Duplex basecalls bam index
+        pairs (list): List of read pair strings
+    """
     if len(pairs) == 0:
         raise ValueError("no pairs found in file")
     all_paired_read_ids = set(itertools.chain(*pairs))
-    simplex_read_ids = set(simplex_index.keys())
-    duplex_read_ids = set(duplex_index)
+    simplex_read_ids = set(simplex_index.read_ids)
+    duplex_read_ids = set(duplex_index.read_ids)
     count_paired_simplex_alignments = sum(
         [1 for read_id in all_paired_read_ids if read_id in simplex_read_ids]
     )
     if count_paired_simplex_alignments == 0:
         raise ValueError("zero simplex alignments found")
 
     # valid meaning we have all the parts to perform inference
@@ -437,26 +422,30 @@
         for t, c in pairs
         if all(read_id in simplex_read_ids for read_id in (t, c))
         and t in duplex_read_ids
     ]
     return valid_read_pairs, len(valid_read_pairs)
 
 
-def prep_duplex_read_builder(simplex_index, pod5_path, simplex_bam_path):
+def prep_duplex_read_builder(simplex_index, pod5_path):
+    """Prepare a duplex pair builder object. For example pass to MultitaskMap
+    prep_func argument.
+
+    Args:
+        simplex_index (io.ReadIndexedBam): Read indexed BAM file handle
+        pod5_path (pod5.reader.Reader): POD5 file handle
+    """
     builder = DuplexPairsBuilder(
         simplex_index=simplex_index,
         pod5_path=pod5_path,
-        simplex_bam_path=simplex_bam_path,
     )
     return [builder], {}
 
 
-def iter_duplexed_io_reads(
-    read_id_pair: Tuple[str, str], builder: DuplexPairsBuilder
-):
+def iter_duplexed_io_reads(read_id_pair, builder):
     return builder.make_read_pair(read_id_pair)
 
 
 def infer_duplex(
     *,
     simplex_pod5_path: str,
     simplex_bam_path: str,
@@ -468,38 +457,39 @@
     num_extract_alignment_threads,
     num_duplex_prep_workers,
     num_infer_threads,
     num_reads=None,
     skip_non_primary=True,
     duplex_deliminator=";",
 ):
-    duplex_bam_index, _ = index_bam(
-        duplex_bam_path, skip_non_primary=skip_non_primary, req_tags=set()
+    duplex_bam_index = ReadIndexedBam(
+        duplex_bam_path,
+        skip_non_primary=skip_non_primary,
+        req_tags=set(),
+        read_id_converter=lambda k: k.split(duplex_deliminator)[0],
     )
-    duplex_bam_index = {
-        k.split(duplex_deliminator)[0]: v for k, v in duplex_bam_index.items()
-    }
 
-    simplex_bam_index, _ = index_bam(
+    simplex_bam_index = ReadIndexedBam(
         simplex_bam_path, skip_non_primary=True, req_tags={"mv"}
     )
-    pairs = DuplexPairsBuilder.parse_pairs(pairs_path)
+    with open(pairs_path, "r") as fh:
+        pairs = [tuple(line.split()) for line in fh]
     valid_pairs, num_valid_reads = check_simplex_alignments(
         simplex_index=simplex_bam_index,
         duplex_index=duplex_bam_index,
         pairs=pairs,
     )
     if num_reads is not None:
         num_reads = min(num_valid_reads, num_reads)
 
     # source of pipeline, template, complement read ID pairs
     # produces template, complement read id tuples
     def iter_pairs(pairs, num_reads):
-        for i, pair in enumerate(pairs):
-            if num_reads is not None and i > num_reads - 1:
+        for pair_num, pair in enumerate(pairs):
+            if num_reads is not None and pair_num >= num_reads:
                 return
             yield pair
 
     read_id_pairs = BackgroundIter(
         iter_pairs,
         kwargs=dict(pairs=valid_pairs, num_reads=num_reads),
         use_process=True,
@@ -508,25 +498,21 @@
     # consumes: tuple of template, complement read Ids
     # prep: open resources for Pod5 and simplex BAM
     # produces: (io.Read, io.Read), str
     io_read_pairs_results = MultitaskMap(
         iter_duplexed_io_reads,
         read_id_pairs,
         prep_func=prep_duplex_read_builder,
-        args=(simplex_bam_index, simplex_pod5_path, simplex_bam_path),
+        args=(simplex_bam_index, simplex_pod5_path),
         name="BuildDuplexedIoReads",
         num_workers=num_extract_alignment_threads,
         use_process=True,
     )
 
-    def make_duplex_reads(
-        read_pair_result: Tuple[Tuple[IoRead, IoRead], Any],
-        duplex_index,
-        bam_file_handle,
-    ):
+    def make_duplex_reads(read_pair_result, duplex_index, bam_file_handle):
         read_pair, err = read_pair_result
         if err is not None or read_pair is None:
             return None, err
         template, complement = read_pair
         if template.read_id not in duplex_index:
             return None, "duplex BAM record not found for read_id"
         for pointer in duplex_index[template.read_id]:
@@ -548,18 +534,15 @@
         io_read_pairs_results,
         num_workers=num_duplex_prep_workers,
         args=(duplex_bam_index, duplex_aln),
         name="MakeDuplexReads",
         use_process=True,
     )
 
-    def add_mod_mappings_to_alignment(
-        duplex_read_result: Tuple[DuplexRead, str],
-        caller: DuplexReadModCaller,
-    ):
+    def add_mod_mappings_to_alignment(duplex_read_result, caller):
         duplex_read, err = duplex_read_result
         if err is not None:
             return None, err
         mod_tags = caller.call_duplex_read_mods(duplex_read)
         mod_tags = list(mod_tags)
         assert len(mod_tags) == 2
         record = duplex_read.duplex_alignment
@@ -590,15 +573,17 @@
     )
 
     errs = defaultdict(int)
     pysam_save = pysam.set_verbosity(0)
     with pysam.AlignmentFile(duplex_bam_path, "rb", check_sq=False) as in_bam:
         with pysam.AlignmentFile(out_bam, "wb", template=in_bam) as out_bam:
             for mod_read_mapping, err in tqdm(
-                alignment_records_with_mod_tags, total=num_reads
+                alignment_records_with_mod_tags,
+                total=num_reads,
+                disable=os.environ.get("LOG_SAFE", False),
             ):
                 if err is not None:
                     errs[err] += 1
                     continue
                 out_bam.write(
                     pysam.AlignedSegment.from_dict(
                         mod_read_mapping, out_bam.header
```

### Comparing `ont-remora-2.0.0/src/remora/log.py` & `ont-remora-2.1.0/src/remora/log.py`

 * *Files identical despite different names*

### Comparing `ont-remora-2.0.0/src/remora/main.py` & `ont-remora-2.1.0/src/remora/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # from remora.common import logging
 from remora.parsers import (
     register_dataset,
     register_model,
     register_infer,
     register_validate,
+    register_analyze,
     SubcommandHelpFormatter,
 )
 
 # filter warnings about GPU on environments without a GPU
 warnings.filterwarnings(action="ignore", category=UserWarning, module="torch")
 
 # LOGGER = logging.get_logger()
@@ -48,14 +49,15 @@
     parser.set_defaults(func=lambda x: parser.print_help())
 
     subparsers = parser.add_subparsers(title="sub-commands")
     register_dataset(subparsers)
     register_model(subparsers)
     register_infer(subparsers)
     register_validate(subparsers)
+    register_analyze(subparsers)
 
     args = parser.parse_args()
     cmd_func = args.func
     if _DO_PROFILE:
         _func_wrapper = cmd_func
 
         def cmd_func(args):
```

### Comparing `ont-remora-2.0.0/src/remora/model_util.py` & `ont-remora-2.1.0/src/remora/model_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 import torch
 import numpy as np
 import pandas as pd
 from torch import nn
 from torch.nn.utils.fusion import fuse_conv_bn_eval
 
+from remora.download import ModelDownload
 from remora import log, RemoraError, constants
 from remora.refine_signal_map import SigMapRefiner
-from remora.download import ModelDownload
 
 LOGGER = log.get_logger()
 
 #############
 # Exporting #
 #############
 
@@ -35,14 +35,15 @@
     meta["kmer_context_bases"] = ckpt["kmer_context_bases"]
     meta["chunk_context"] = ckpt["chunk_context"]
 
     # add simple metadata
     for ckpt_key in (
         "base_pred",
         "mod_bases",
+        "reverse_signal",
         "refine_kmer_center_idx",
         "refine_do_rough_rescale",
         "refine_scale_iters",
         "refine_algo",
         "refine_half_bandwidth",
         "base_start_justify",
         "offset",
@@ -186,14 +187,15 @@
             )
         save_tensor("refine_kmer_levels", refine_kmer_levels)
 
     # add simple metadata
     for ckpt_key in (
         "mod_bases",
         "offset",
+        "reverse_signal",
     ):
         modbases[ckpt_key] = ckpt[ckpt_key]
 
     if ckpt["mod_bases"] is not None:
         for mod_idx in range(len(ckpt["mod_bases"])):
             modbases[f"mod_long_names_{mod_idx}"] = str(
                 ckpt["mod_long_names"][mod_idx]
@@ -201,15 +203,15 @@
     for key in ("chunk_context", "kmer_context_bases"):
         for idx in range(2):
             modbases[f"{key}_{idx}"] = ckpt[key][idx]
 
     if len(ckpt["motifs"]) > 1:
         raise RemoraError("Dorado only supports models with a single motif")
 
-    for (motif, motif_offset) in ckpt["motifs"]:
+    for motif, motif_offset in ckpt["motifs"]:
         modbases["motif"] = motif
         modbases["motif_offset"] = motif_offset
 
     metadata["general"] = general
     metadata["model_params"] = ckpt["model_params"]
     metadata["modbases"] = modbases
     metadata["refinement"] = refinement
@@ -243,15 +245,19 @@
     model_path = ckpt["model_path"] if model_path is None else model_path
     model = _load_python_model(model_path, **ckpt["model_params"])
     model.load_state_dict(ckpt["state_dict"])
     return ckpt, model
 
 
 def add_derived_metadata(model_metadata):
-    model_metadata["base_pred"] = model_metadata["base_pred"] == "True"
+    if "reverse_signal" not in model_metadata:
+        LOGGER.warning(
+            "reverse signal attribute not found in model. Assuming False"
+        )
+        model_metadata["reverse_signal"] = False
     if model_metadata["mod_bases"] == "None":
         model_metadata["mod_bases"] = None
         model_metadata["mod_long_names"] = None
     else:
         model_metadata["mod_long_names"] = []
         for mod_idx in range(len(model_metadata["mod_bases"])):
             model_metadata["mod_long_names"].append(
@@ -326,19 +332,14 @@
                 int(model_metadata["refine_do_rough_rescale"])
             ),
             scale_iters=int(model_metadata["refine_scale_iters"]),
             algo=model_metadata["refine_algo"],
             half_bandwidth=int(model_metadata["refine_half_bandwidth"]),
             sd_arr=refine_sd_arr,
         )
-
-        model_metadata["base_start_justify"] = (
-            model_metadata["base_start_justify"] == "True"
-        )
-        model_metadata["offset"] = int(model_metadata["offset"])
     else:
         # handle original models without sig_map_refiner
         model_metadata["sig_map_refiner"] = SigMapRefiner()
         model_metadata["base_start_justify"] = False
         model_metadata["offset"] = 0
 
 
@@ -368,15 +369,15 @@
 
 def load_torchscript_model(model_filename, device=None, quiet=False):
     """Load torchscript model. If device is specified load onto specified
     device.
 
     Args:
         model_filename (str): Model path
-        device (int): GPU device ID
+        device (torch.device): Torch device (or None)
         quiet (bool): Print model info to debug
 
     Returns:
         2-tuple containing:
           1. Compiled model object for calling mods
           2. Model metadata dictionary with information concerning data prep
     """
@@ -387,15 +388,15 @@
         model = torch.jit.load(
             model_filename, _extra_files=extra_files, map_location="cpu"
         )
     else:
         model = torch.jit.load(
             model_filename,
             _extra_files=extra_files,
-            map_location=torch.device(device),
+            map_location=device,
         )
     model_metadata = json.loads(extra_files["meta.txt"])
     add_derived_metadata(model_metadata)
     if not quiet:
         md_str = repr_model_metadata(model_metadata)
         LOGGER.debug(f"Loaded Remora model attrs\n{md_str}\n")
     return model, model_metadata
```

### Comparing `ont-remora-2.0.0/src/remora/parsers.py` & `ont-remora-2.1.0/src/remora/parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,147 +76,150 @@
         help="BAM file containing mv tags.",
     )
 
     out_grp = subparser.add_argument_group("Output Arguments")
     out_grp.add_argument(
         "--output-remora-training-file",
         default="remora_training_dataset.npz",
-        help="Output Remora training dataset file. Default: %(default)s",
+        help="Output Remora training dataset file.",
     )
     out_grp.add_argument(
         "--log-filename",
         help="Log filename. Default: Don't output log file.",
     )
 
     data_grp = subparser.add_argument_group("Data Arguments")
     data_grp.add_argument(
         "--motif",
         nargs=2,
         action="append",
         metavar=("MOTIF", "FOCUS_POSITION"),
-        help="Extract training chunks centered on a defined motif. Argument "
-        "takes 2 values representing 1) sequence motif and 2) focus position "
-        "within the motif. For example to restrict to CpG sites use "
-        '"--motif CG 0". Default: Any context ("N 0")',
+        help="""Extract training chunks centered on a defined motif. Argument
+        takes 2 values representing 1) sequence motif and 2) focus position
+        within the motif. For example to restrict to CpG sites use "
+        "--motif CG 0". Default: Any context ("N 0")""",
     )
     data_grp.add_argument(
         "--focus-reference-positions",
-        help="BED file containing reference positions around which to extract "
-        "training chunks.",
+        help="""BED file containing reference positions around which to extract
+        training chunks.""",
     )
     data_grp.add_argument(
         "--chunk-context",
         default=constants.DEFAULT_CHUNK_CONTEXT,
         type=int,
         nargs=2,
-        help="Number of context signal points to select around the central "
-        "position. Default: %(default)s",
+        metavar=("NUM_BEFORE", "NUM_AFTER"),
+        help="""Number of context signal points to select around the central
+        position.""",
     )
     data_grp.add_argument(
         "--min-samples-per-base",
         type=int,
         default=constants.DEFAULT_MIN_SAMPLES_PER_BASE,
-        help="Minimum number of samples per base. This sets the size of the "
-        "ragged arrays of chunk sequences. Default: %(default)s",
+        help="""Minimum number of samples per base. This sets the size of the
+        ragged arrays of chunk sequences.""",
     )
     data_grp.add_argument(
         "--kmer-context-bases",
         nargs=2,
         default=constants.DEFAULT_KMER_CONTEXT_BASES,
         type=int,
-        help="Definition of k-mer (derived from the reference) passed into "
-        "the model along with each signal position. Default: %(default)s",
+        metavar=("BASES_BEFORE", "BASES_AFTER"),
+        help="""Definition of k-mer (derived from the reference) passed into
+        the model along with each signal position.""",
     )
     data_grp.add_argument(
         "--max-chunks-per-read",
         type=int,
         default=15,
-        help="Maxiumum number of chunks to extract from a single read. "
-        "Default: %(default)s",
+        help="Maxiumum number of chunks to extract from a single read.",
     )
     data_grp.add_argument(
         "--base-start-justify",
         action="store_true",
-        help="Justify extracted chunk against the start of the base of "
-        "interest. Default justifies chunk to middle of signal of the base "
-        "of interest.",
+        help="""Justify extracted chunk against the start of the base of
+        interest. Default justifies chunk to middle of signal of the base
+        of interest.""",
     )
     data_grp.add_argument(
         "--offset",
         default=0,
         type=int,
-        help="Offset selected chunk position by a number of bases. "
-        "Default: %(default)d",
+        help="Offset selected chunk position by a number of bases.",
     )
     data_grp.add_argument(
         "--num-reads",
-        default=None,
         type=int,
         help="Number of reads.",
     )
     data_grp.add_argument(
-        "--base-call-anchor",
+        "--basecall-anchor",
+        action="store_true",
+        help="""Make dataset from basecall sequence instead of aligned
+        reference sequence""",
+    )
+    data_grp.add_argument(
+        "--reverse-signal",
         action="store_true",
-        help="makes dataset from base call sequence instead of aligned "
-        "reference sequence",
+        help="""Is nanopore signal 3' to 5' orientation? Primarily for direct
+        RNA""",
     )
 
     refine_grp = subparser.add_argument_group("Signal Mapping Refine Arguments")
     refine_grp.add_argument(
         "--refine-kmer-level-table",
-        help="Tab-delimited file containing no header and two fields: "
-        "1. string k-mer sequence and 2. float expected normalized level. "
-        "All k-mers must be the same length and all combinations of the bases "
-        "'ACGT' must be present in the file.",
+        help="""Tab-delimited file containing no header and two fields:
+        1. string k-mer sequence and 2. float expected normalized level.
+        All k-mers must be the same length and all combinations of the bases
+        'ACGT' must be present in the file.""",
     )
     refine_grp.add_argument(
         "--refine-rough-rescale",
         action="store_true",
-        help="Apply a rough rescaling using quantiles of signal+move table "
-        "and levels.",
+        help="""Apply a rough rescaling using quantiles of signal+move table
+        and levels.""",
     )
     refine_grp.add_argument(
         "--refine-scale-iters",
-        default=constants.DEFAULT_REFINE_SCALE_ITERS,
+        default=-1,
         type=int,
-        help="Number of iterations of signal mapping refinement and signal "
-        "re-scaling to perform. Set to 0 (default) in order to perform signal "
-        "mapping refinement, but skip re-scaling. Set to -1 to skip signal "
-        "mapping (potentially using levels for rough rescaling).",
+        help="""Number of iterations of signal mapping refinement and signal
+        re-scaling to perform. Set to 0 in order to perform signal mapping
+        refinement, but skip re-scaling. Set to -1 (default) to skip signal
+        mapping (potentially using levels for rough rescaling).""",
     )
     refine_grp.add_argument(
         "--refine-half-bandwidth",
         default=constants.DEFAULT_REFINE_HBW,
         type=int,
-        help="Half bandwidth around signal mapping over which to search for "
-        "new path.",
+        help="""Half bandwidth around signal mapping over which to search for
+        "new path.""",
     )
     refine_grp.add_argument(
         "--refine-algo",
         default=constants.DEFAULT_REFINE_ALGO,
         choices=constants.REFINE_ALGOS,
         help="Refinement algorithm to apply (if kmer level table is provided).",
     )
     refine_grp.add_argument(
         "--refine-short-dwell-parameters",
         default=constants.DEFAULT_REFINE_SHORT_DWELL_PARAMS,
         type=float,
         nargs=3,
         metavar=("TARGET", "LIMIT", "WEIGHT"),
-        help="Short dwell penalty refiner parameters. Dwells shorter than "
-        "LIMIT will be penalized a value of `WEIGHT * (dwell - TARGET)^2`. "
-        "Default: %(default)s",
+        help="""Short dwell penalty refiner parameters. Dwells shorter than
+        LIMIT will be penalized a value of `WEIGHT * (dwell - TARGET)^2`.""",
     )
 
     label_grp = subparser.add_argument_group("Label Arguments")
     label_grp.add_argument(
         "--mod-base",
         nargs=2,
         metavar=("SINGLE_LETTER_CODE", "MOD_BASE"),
-        default=None,
         help="Modified base information. Example: `--mod-base m 5mC`",
     )
     label_grp.add_argument(
         "--mod-base-control",
         action="store_true",
         help="Is this a modified bases control sample?",
     )
@@ -227,30 +230,30 @@
     )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--num-extract-alignment-workers",
         type=int,
         default=1,
-        help="Number of signal extraction workers. Default: %(default)d",
+        help="Number of signal extraction workers.",
     )
     comp_grp.add_argument(
         "--num-extract-chunks-workers",
         type=int,
         default=1,
-        help="Number of chunk extraction workers. If performing signal "
-        "refinement this should be increased. Default: %(default)d",
+        help="""Number of chunk extraction workers. If performing signal
+        refinement this should be increased.""",
     )
 
     subparser.set_defaults(func=run_dataset_prepare)
 
 
 def run_dataset_prepare(args):
-    from remora.io import parse_bed
     from remora.util import Motif
+    from remora.io import parse_bed
     from remora.refine_signal_map import SigMapRefiner
     from remora.prepare_train_data import extract_chunk_dataset
 
     if args.log_filename is not None:
         log.init_logger(args.log_filename)
     if args.mod_base is None and not args.mod_base_control:
         LOGGER.error("Must specify either --mod-base or --mod-base-control")
@@ -287,15 +290,16 @@
         args.base_pred,
         args.kmer_context_bases,
         args.base_start_justify,
         args.offset,
         args.num_reads,
         args.num_extract_alignment_workers,
         args.num_extract_chunks_workers,
-        base_call_anchor=args.base_call_anchor,
+        basecall_anchor=args.basecall_anchor,
+        rev_sig=args.reverse_signal,
     )
 
 
 def register_dataset_split(parser):
     subparser = parser.add_parser(
         "split",
         description="Split Remora dataset",
@@ -305,32 +309,32 @@
     subparser.add_argument(
         "input_remora_dataset",
         help="Remora training dataset to be split",
     )
     subparser.add_argument(
         "--output-basename",
         default="split_remora_dataset",
-        help="Basename for output datasets. Default: %(default)s",
+        help="Basename for output datasets.",
     )
     subparser.add_argument(
         "--val-prop",
         type=float,
-        help="The proportion of data to be split into validation set, where "
-        "val-prop in [0,0.5).",
+        help="""The proportion of data to be split into validation set, where
+        val-prop in [0,0.5).""",
     )
     subparser.add_argument(
         "--val-num",
         type=int,
         help="Number of validation chunks to select.",
     )
     subparser.add_argument(
         "--unstratified",
         action="store_true",
-        help="For --val-prop split, perform unstratified splitting. Default "
-        "will perform split stratified over labels.",
+        help="""For --val-prop split, perform unstratified splitting. Default
+        will perform split stratified over labels.""",
     )
     subparser.add_argument(
         "--by-label",
         action="store_true",
         help="Split dataset into one dataset for each unique label.",
     )
     subparser.set_defaults(func=run_dataset_split)
@@ -398,36 +402,46 @@
         description="Merge Remora datasets",
         help="Merge Remora datasets",
         formatter_class=SubcommandHelpFormatter,
     )
     subparser.add_argument(
         "--input-dataset",
         nargs=2,
+        metavar=("PATH", "NUM_CHUNKS"),
         action="append",
-        help="1) Remora training dataset path and 2) max number of chunks "
-        "to extract from this dataset.",
+        help="""1) Remora training dataset path and 2) max number of chunks
+        to extract from this dataset. Second argument can be "all" to use all
+        chunks from a dataset""",
     )
     subparser.add_argument(
         "--output-dataset",
         required=True,
         help="Output path for dataset",
     )
     subparser.add_argument(
         "--balance",
         action="store_true",
-        help="Automatically balance classes when merging",
+        help="Automatically balance classes after merging",
+    )
+    subparser.add_argument(
+        "--log-filename",
+        help="Log filename. (default: Don't output log file)",
     )
     subparser.set_defaults(func=run_dataset_merge)
 
 
 def run_dataset_merge(args):
     from remora.data_chunks import merge_datasets
 
+    if args.log_filename is not None:
+        log.init_logger(args.log_filename)
+
     input_datasets = [
-        (ds_path, int(num_chunks)) for ds_path, num_chunks in args.input_dataset
+        (ds_path, None if num_chunks == "all" else int(num_chunks))
+        for ds_path, num_chunks in args.input_dataset
     ]
     output_dataset = merge_datasets(input_datasets, args.balance)
     output_dataset.save(args.output_dataset)
 
 
 ################
 # remora model #
@@ -465,60 +479,67 @@
     )
 
     data_grp = subparser.add_argument_group("Data Arguments")
     data_grp.add_argument(
         "--val-prop",
         default=constants.DEFAULT_VAL_PROP,
         type=float,
-        help="Proportion of the dataset to be used as validation. "
-        "Default: %(default)f",
+        help="Proportion of the dataset to be used as validation.",
     )
     data_grp.add_argument(
         "--batch-size",
         default=constants.DEFAULT_BATCH_SIZE,
         type=int,
-        help="Number of samples per batch. Default: %(default)d",
+        help="Number of samples per batch.",
     )
     data_grp.add_argument(
         "--chunk-context",
         type=int,
         nargs=2,
-        help="Override chunk context from data prep. Number of context signal "
-        "points to select around the central position.",
+        metavar=("NUM_BEFORE", "NUM_AFTER"),
+        help="""Override chunk context from data prep. Number of context signal
+        points to select around the central position.""",
     )
     data_grp.add_argument(
         "--kmer-context-bases",
         nargs=2,
         type=int,
-        help="Override kmer context bases from data prep. Definition of "
-        "k-mer (derived from the reference) passed into the model along with "
-        "each signal position.",
+        metavar=("BASES_BEFORE", "BASES_AFTER"),
+        help="""Override kmer context bases from data prep. Definition of
+        k-mer (derived from the reference) passed into the model along with
+        each signal position.""",
     )
     data_grp.add_argument(
         "--ext-val",
         nargs="+",
         help="Path(s) to the external validation Remora datasets.",
     )
     data_grp.add_argument(
+        "--ext-val-names",
+        nargs="+",
+        help="""Names for external datasets. If provided must match length of
+        [--ext-val] argument""",
+    )
+    data_grp.add_argument(
         "--balance",
         action="store_true",
         help="Balance classes exactly prior to training",
     )
 
     out_grp = subparser.add_argument_group("Output Arguments")
     out_grp.add_argument(
         "--output-path",
         default="remora_train_results",
-        help="Path to the output files. Default: %(default)s",
+        help="Path to the output files.",
     )
     out_grp.add_argument(
         "--save-freq",
         default=10,
         type=int,
-        help="After how many epochs to save the model. Default %(default)d",
+        help="After how many epochs to save the model.",
     )
     out_grp.add_argument(
         "--overwrite",
         action="store_true",
         help="Overwrite existing output directory if existing.",
     )
 
@@ -526,107 +547,116 @@
     mdl_grp.add_argument(
         "--model", required=True, help="Model architecture file (required)"
     )
     mdl_grp.add_argument(
         "--size",
         type=int,
         default=constants.DEFAULT_NN_SIZE,
-        help="Model layer size. Default: %(default)d",
+        help="Model layer size.",
     )
 
     train_grp = subparser.add_argument_group("Training Arguments")
     train_grp.add_argument(
         "--epochs",
         default=constants.DEFAULT_EPOCHS,
         type=int,
-        help="Number of training epochs. Default: %(default)d",
+        help="Number of training epochs.",
     )
     train_grp.add_argument(
         "--optimizer",
         default=constants.OPTIMIZERS[0],
         choices=constants.OPTIMIZERS,
-        help="Optimizer setting. Default: %(default)s",
+        help="Optimizer setting.",
     )
     train_grp.add_argument(
         "--scheduler",
         default=None,
-        help="Scheduler setting. Default: %(default)s",
+        help="Scheduler setting.",
     )
     train_grp.add_argument(
         "--lr",
         default=constants.DEFAULT_LR,
         type=float,
-        help="Learning rate setting. Default: %(default)f",
+        help="Learning rate setting.",
     )
     train_grp.add_argument(
         "--weight-decay",
         default=constants.DEFAULT_WEIGHT_DECAY,
         type=float,
-        help="Weight decay setting. Default: %(default)f",
+        help="Weight decay setting.",
     )
     train_grp.add_argument(
         "--early-stopping",
-        default=10,
+        default=5,
         type=int,
-        help="Stops training after a number of epochs without improvement."
-        "If set to 0 no stopping is done. Default: %(default)d",
+        help="""Stops training after a number of epochs without improvement.
+        If set to 0 no stopping is done.""",
     )
     train_grp.add_argument(
         "--seed",
-        default=None,
         type=int,
-        help="Seed value. Default: Random seed",
+        help="Seed value.",
     )
     train_grp.add_argument(
         "--filter-fraction",
         default=constants.DEFAULT_FILT_FRAC,
         type=float,
-        help="Fraction of predictions to filter in validation reporting. "
-        "Un-filtered validation metrics will always be reported as well. "
-        "Default: %(default)f",
+        help="""Fraction of predictions to filter in validation reporting.
+        Un-filtered validation metrics will always be reported as well.""",
     )
     train_grp.add_argument(
         "--lr-sched-kwargs",
         nargs=3,
         action="append",
-        default=None,
         metavar=("NAME", "VALUE", "TYPE"),
     )
     train_grp.add_argument(
-        "--balanced-batch",
-        action="store_true",
-        help="Balance classes exactly for each batch in training",
+        "--batch-label-weights",
+        type=float,
+        nargs="+",
+        help="Select batch labels with specified weights",
+    )
+    train_grp.add_argument(
+        "--high-conf-incorrect-thr-frac",
+        nargs=2,
+        type=float,
+        metavar=("THRESHOLD", "FRACTION"),
+        help="1.) Threshold value of what to consider a high confidence "
+        " predicition. Based on the softmax output. \n"
+        "2.) Fraction (of the batch size) of highly confident incorrect "
+        "predictions to filter during training. Filtering up to this value, "
+        "but might be lower.",
     )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--device",
-        type=int,
-        help="ID of GPU that is used for training. Default: Use CPU.",
+        help="Device for neural network processing. See torch.device.",
     )
 
     subparser.set_defaults(func=run_model_train)
 
 
 def run_model_train(args):
+    from remora.util import parse_device
     from remora.train_model import train_model
 
     out_path = Path(args.output_path)
     if args.overwrite:
         if out_path.is_dir():
             rmtree(out_path)
         elif out_path.exists():
             out_path.unlink()
     elif out_path.exists():
         raise RemoraError("Refusing to overwrite existing training directory.")
     out_path.mkdir(parents=True, exist_ok=True)
     log.init_logger(os.path.join(out_path, "log.txt"))
     train_model(
         args.seed,
-        args.device,
+        parse_device(args.device),
         out_path,
         args.remora_dataset_path,
         args.chunk_context,
         args.kmer_context_bases,
         args.val_prop,
         args.batch_size,
         args.model,
@@ -636,17 +666,19 @@
         args.scheduler,
         args.weight_decay,
         args.epochs,
         args.save_freq,
         args.early_stopping,
         args.filter_fraction,
         args.ext_val,
+        args.ext_val_names,
         args.lr_sched_kwargs,
         args.balance,
-        args.balanced_batch,
+        args.batch_label_weights,
+        args.high_conf_incorrect_thr_frac,
     )
 
 
 def register_model_export(parser):
     subparser = parser.add_parser(
         "export",
         description="Export a model to TorchScript format for inference.",
@@ -655,26 +687,25 @@
     )
     subparser.add_argument(
         "checkpoint_path",
         help="Path to a pretrained model checkpoint.",
     )
     subparser.add_argument(
         "output_path",
-        help="Path to save the model file, or the directory in which to "
-        "save the dorado tensor files if '--format dorado' has been specified.",
+        help="Path or directory to save the model.",
     )
     subparser.add_argument(
         "--model-path",
         help="Path to a model architecture. Default: Use path from checkpoint.",
     )
     subparser.add_argument(
         "--format",
-        default="torchscript",
+        default="dorado",
         choices=["dorado", "torchscript"],
-        help="Export format. Default: torchscript",
+        help="Export format.",
     )
 
     subparser.set_defaults(func=run_model_export)
 
 
 def run_model_export(args):
     from remora.model_util import (
@@ -710,31 +741,30 @@
         description="List pre-trained modified base models.",
         help="List pre-trained modified base models.",
         formatter_class=SubcommandHelpFormatter,
     )
     subparser.add_argument("--pore", help="specify pore type")
     subparser.add_argument(
         "--basecall-model-type",
-        help="specify the basecaller model type (e.g., fast, hac or sup)",
+        help="Specify the basecaller model type (e.g., fast, hac or sup)",
     )
     subparser.add_argument(
-        "--basecall-model-version", help="specify the version of the basecaller"
+        "--basecall-model-version", help="Specify basecaller model version"
     )
     subparser.add_argument(
         "--modified-bases",
         nargs="+",
-        help="specify the modified base models you are interested in",
+        help="Specify the modified base(s)",
     )
     subparser.add_argument(
         "--remora-model-type",
-        help="specify the motif or context that the remora model has been "
-        "trained on",
+        help="Specify model motif (sequence context)",
     )
     subparser.add_argument(
-        "--remora-model-version", help="specify the remora model version"
+        "--remora-model-version", help="Specify Remora model version"
     )
     subparser.set_defaults(func=run_list_pretrained)
 
 
 def run_list_pretrained(args):
     from remora.model_util import get_pretrained_models
     from tabulate import tabulate
@@ -759,40 +789,40 @@
         description="Download pre-trained modified base models.",
         help="Download pre-trained modified base models.",
         formatter_class=SubcommandHelpFormatter,
     )
     subparser.add_argument("--pore", help="specify pore type")
     subparser.add_argument(
         "--basecall-model-type",
-        help="specify the basecaller model type (e.g., fast, hac or sup)",
+        help="Specify the basecaller model type (e.g., fast, hac or sup)",
     )
     subparser.add_argument(
-        "--basecall-model-version", help="specify the version of the basecaller"
+        "--basecall-model-version", help="Specify basecaller model version"
     )
     subparser.add_argument(
         "--modified-bases",
         nargs="+",
-        help="specify the modified base models you are interested in",
+        help="Specify the modified base(s)",
     )
     subparser.add_argument(
         "--remora-model-type",
-        help="specify the motif or context that the remora model has been "
-        "trained on",
+        help="Specify model motif (sequence context)",
     )
     subparser.add_argument(
-        "--remora-model-version", help="specify the remora model version"
+        "--remora-model-version", help="Specify Remora model version"
     )
     subparser.set_defaults(func=run_download)
 
 
 def run_download(args):
-    from remora.model_util import get_pretrained_models
-    from remora.download import ModelDownload
     import pkg_resources
 
+    from remora.download import ModelDownload
+    from remora.model_util import get_pretrained_models
+
     models, header = get_pretrained_models(
         args.pore,
         args.basecall_model_type,
         args.basecall_model_version,
         args.modified_bases,
         args.remora_model_type,
         args.remora_model_version,
@@ -876,16 +906,16 @@
     mdl_grp.add_argument(
         "--modified-bases",
         nargs="+",
         help="Long name of the modified bases to call (e.g., 5mc, 5hmc).",
     )
     mdl_grp.add_argument(
         "--remora-model-type",
-        help="Choose the specific motif of the model you want to load. "
-        "If None, load CG model.",
+        help="""Choose the specific motif of the model you want to load.
+        If None, load CG model.""",
     )
     mdl_grp.add_argument(
         "--remora-model-version",
         type=int,
         help="Choose the remora model version. If None, use latest.",
     )
 
@@ -895,48 +925,47 @@
         default=None,
         type=int,
         help="Number of reads.",
     )
     data_grp.add_argument(
         "--reference-anchored",
         action="store_true",
-        help="Infer per-read modified bases against reference bases instead "
-        "of basecalls.",
+        help="""Infer per-read modified bases against reference bases instead
+        of basecalls.""",
     )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--device",
         type=int,
         help="ID of GPU that is used for inference. Default: CPU only",
     )
     comp_grp.add_argument(
-        "--num-extract-alignment-workers",
+        "--queue-max",
         type=int,
-        default=1,
-        help="Number of signal extraction workers. Default: %(default)d",
+        default=1_000,
+        help="Maximum number of reads to store in each multiprocessing queue.",
     )
     comp_grp.add_argument(
-        "--num-prepare-batch-workers",
+        "--num-extract-alignment-workers",
         type=int,
         default=1,
-        help="Number of batch preparation workers. Default: %(default)d",
+        help="Number of signal extraction workers.",
     )
     comp_grp.add_argument(
-        "--num-infer-workers",
+        "--num-prepare-batch-workers",
         type=int,
         default=1,
-        help="Number of chunk extraction workers. If performing signal "
-        "refinement this should be increased. Default: %(default)d",
+        help="Number of batch preparation workers.",
     )
     comp_grp.add_argument(
         "--batch-size",
         default=constants.DEFAULT_BATCH_SIZE,
         type=int,
-        help="Number of input units per batch. Default: %(default)d",
+        help="Number of input units per batch.",
     )
 
     subparser.set_defaults(func=run_infer_from_pod5_and_bam)
 
 
 def register_infer_duplex_from_pod5_and_bam(parser):
     duplex_delim_flag = "--duplex-delim"
@@ -954,29 +983,29 @@
     )
     subparser.add_argument(
         "simplex_bam",
         help="Base called BAM file containing mv tags.",
     )
     subparser.add_argument(
         "duplex_bam",
-        help="BAM file containing duplex base called sequences (and optional "
-        "reference mappings). Record names may either be the template read_id "
-        "or template<delim>complement. The value of <delim> can be set with "
-        f"{duplex_delim_flag}.",
+        help=f"""BAM file containing duplex base called sequences (and optional
+        reference mappings). Record names may either be the template read_id
+        or template<delim>complement. The value of <delim> can be set with
+        {duplex_delim_flag}.""",
     )
     subparser.add_argument(
         "duplex_read_pairs",
-        help="Whitespace separated plain text file containing read ID pairs, no"
-        "header.",
+        help="""Whitespace separated plain text file containing read ID pairs,
+        no header.""",
     )
     subparser.add_argument(
         duplex_delim_flag,
-        help="deliminator string between template and complement read "
-        "ids in the duplex BAM",
         default=";",
+        help="""Deliminator string between template and complement read
+        ids in the duplex BAM""",
     )
 
     out_grp = subparser.add_argument_group("Output Arguments")
     out_grp.add_argument(
         "--out-bam",
         help="Output BAM path.",
     )
@@ -988,16 +1017,16 @@
     mdl_grp = subparser.add_argument_group("Model Arguments")
     mdl_grp.add_argument(
         "--model",
         help="Path to a pretrained model in torchscript format.",
     )
     mdl_grp.add_argument(
         "--pore",
-        help="Choose the type of pore the Remora model has been trained on "
-        "(e.g. dna_r10.4_e8.1)",
+        help="""Choose the type of pore the Remora model has been trained on
+        (e.g. dna_r10.4_e8.1)""",
     )
     mdl_grp.add_argument(
         "--basecall-model-type",
         help="Choose the basecaller model type (choose from fast, hac or sup)",
     )
     mdl_grp.add_argument(
         "--basecall-model-version",
@@ -1018,62 +1047,62 @@
         type=int,
         help="Choose the remora model version. If None, use latest.",
     )
 
     data_grp = subparser.add_argument_group("Data Arguments")
     data_grp.add_argument(
         "--num-reads",
-        default=None,
         type=int,
         help="Number of reads.",
     )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--device",
         type=int,
         help="ID of GPU that is used for inference. Default: CPU only",
     )
     comp_grp.add_argument(
         "--num-extract-alignment-workers",
         type=int,
         default=1,
-        help="Number of IO extraction workers. Default: %(default)d",
+        help="Number of IO extraction workers.",
     )
     comp_grp.add_argument(
         "--num-duplex-prep-workers",
         type=int,
         default=1,
-        help="Number of duplex prep workers (tends to bottleneck). Default:"
-        "%(default)d",
+        help="Number of duplex prep workers (tends to bottleneck).",
     )
     comp_grp.add_argument(
         "--num-infer-workers",
         type=int,
         default=1,
-        help="Number of chunk extraction workers. If performing signal "
-        "refinement this should be increased. Default: %(default)d",
+        help="""Number of chunk extraction workers. If performing signal
+        refinement this should be increased.""",
     )
 
     subparser.set_defaults(func=run_infer_from_pod5_and_bam_duplex)
 
 
 def _unpack_model_kw_args(args) -> dict:
+    from remora.util import parse_device
+
     if args.model and not os.path.exists(args.model):
         raise ValueError(f"didn't find model file at {args.model}")
 
     model_kwargs = {
         "model_filename": args.model,
         "pore": args.pore,
         "basecall_model_type": args.basecall_model_type,
         "basecall_model_version": args.basecall_model_version,
         "modified_bases": args.modified_bases,
         "remora_model_type": args.remora_model_type,
         "remora_model_version": args.remora_model_version,
-        "device": args.device,
+        "device": parse_device(args.device),
     }
     return model_kwargs
 
 
 def run_infer_from_pod5_and_bam(args):
     from remora.model_util import load_model
     from remora.inference import infer_from_pod5_and_bam
@@ -1086,17 +1115,17 @@
     infer_from_pod5_and_bam(
         pod5_path=args.pod5,
         in_bam_path=args.in_bam,
         model=model,
         model_metadata=model_metadata,
         out_bam_path=args.out_bam,
         num_reads=args.num_reads,
+        queue_max=args.queue_max,
         num_extract_alignment_workers=args.num_extract_alignment_workers,
         num_prep_batch_workers=args.num_prepare_batch_workers,
-        num_infer_workers=args.num_infer_workers,
         batch_size=args.batch_size,
         ref_anchored=args.reference_anchored,
     )
 
 
 def run_infer_from_pod5_and_bam_duplex(args):
     from remora.model_util import load_model
@@ -1176,16 +1205,16 @@
     )
     subparser.add_argument(
         "--full-results-filename", help="Output per-read calls to TSV file."
     )
     subparser.add_argument(
         "--name",
         default="sample",
-        help="Name of this sample/comparison. Useful when tabulating "
-        "several runs.",
+        help="""Name of this sample/comparison. Useful when tabulating
+        several runs.""",
     )
     subparser.add_argument(
         "--pct-filt",
         type=float,
         default=10.0,
         help="Filter a specified percentage (or less given ties) of calls.",
     )
@@ -1193,16 +1222,15 @@
         "--allow-unbalanced",
         action="store_true",
         help="Allow classes to be unbalanced for metric computation.",
     )
     subparser.add_argument(
         "--max-sites-per-read",
         type=int,
-        help="Maxiumum number of sites to extract from a single read. "
-        "Default: %(default)s",
+        help="Maxiumum number of sites to extract from a single read.",
     )
     subparser.add_argument(
         "--seed",
         type=int,
         help="Seed value. Default: Random seed",
     )
     subparser.add_argument(
@@ -1302,28 +1330,29 @@
     )
 
     comp_grp = subparser.add_argument_group("Compute Arguments")
     comp_grp.add_argument(
         "--batch-size",
         default=constants.DEFAULT_BATCH_SIZE,
         type=int,
-        help="Number of input units per batch. Default: %(default)d",
+        help="Number of input units per batch.",
     )
     comp_grp.add_argument(
         "--device",
         type=int,
         help="ID of GPU that is used for inference. Default: CPU",
     )
 
     subparser.set_defaults(func=run_validate_from_remora_dataset)
 
 
 def run_validate_from_remora_dataset(args):
     import torch
 
+    from remora.util import parse_device
     from remora.model_util import load_model
     from remora.validate import ValidationLogger
     from remora.data_chunks import RemoraDataset
 
     LOGGER.info("Loading dataset from Remora file")
     dataset = RemoraDataset.load_from_file(
         args.remora_dataset_path,
@@ -1337,15 +1366,15 @@
         args.model,
         pore=args.pore,
         basecall_model_type=args.basecall_model_type,
         basecall_model_version=args.basecall_model_version,
         modified_bases=args.modified_bases,
         remora_model_type=args.remora_model_type,
         remora_model_version=args.remora_model_version,
-        device=args.device,
+        device=parse_device(args.device),
     )
 
     dataset.trim_kmer_context_bases(model_metadata["kmer_context_bases"])
     dataset.trim_chunk_context(model_metadata["chunk_context"])
     LOGGER.info(f"Loaded dataset summary:\n{dataset.summary}")
 
     if args.out_file is None:
@@ -1363,9 +1392,394 @@
     val_fp = ValidationLogger(out_fp, full_results_fp)
     val_fp.validate_model(
         model,
         model_metadata["mod_bases"],
         torch.nn.CrossEntropyLoss(),
         dataset,
         args.pct_filt / 100,
-        display_progress_bar=True,
     )
+
+
+##################
+# remora analyze #
+##################
+
+
+def register_analyze(parser):
+    subparser = parser.add_parser(
+        "analyze",
+        description="Analyze nanopore data including raw signal",
+        help="Analyze nanopore data including raw signal",
+        formatter_class=SubcommandHelpFormatter,
+    )
+    ssubparser = subparser.add_subparsers(title="Analyze commands")
+    # register_estimate_kmer_levels(ssubparser)
+    # Since `plot` has several sub-commands, print help as default
+    subparser.set_defaults(func=lambda x: subparser.print_help())
+    # Register analyze sub commands
+    register_analyze_plot(ssubparser)
+
+
+def register_analyze_plot(parser):
+    subparser = parser.add_parser(
+        "plot",
+        description="Plot nanopore data including raw signal",
+        help="Plot nanopore data including raw signal",
+        formatter_class=SubcommandHelpFormatter,
+    )
+    ssubparser = subparser.add_subparsers(title="Plot commands")
+    # Since `plot` has several sub-commands, print help as default
+    subparser.set_defaults(func=lambda x: subparser.print_help())
+    # Register plot sub commands
+    register_plot_ref_region(ssubparser)
+
+
+def register_plot_ref_region(parser):
+    subparser = parser.add_parser(
+        "ref_region",
+        description="Plot signal at reference region",
+        help="Plot signal at reference region",
+        formatter_class=SubcommandHelpFormatter,
+    )
+
+    in_grp = subparser.add_argument_group("Input Arguments")
+    in_grp.add_argument(
+        "--pod5-and-bam",
+        required=True,
+        nargs=2,
+        metavar=("POD5", "BAM"),
+        action="append",
+        help="""POD5 signal path and BAM file path. BAM file must be mapped,
+        sorted and indexed and contain move table and MD tags. Multiple
+        samples can be supplied and will be plotted in different colors""",
+    )
+    in_grp.add_argument(
+        "--ref-regions",
+        required=True,
+        help="""Reference region(s) to plot specified in BED format. Each line
+        in this input file will produce one page in the output PDF.""",
+    )
+    in_grp.add_argument(
+        "--highlight-ranges",
+        help="""BED file containing regions to highlight""",
+    )
+    in_grp.add_argument(
+        "--highlight-color",
+        default="orange",
+        help="""Color or highlighted regions""",
+    )
+
+    refine_grp = subparser.add_argument_group("Signal Mapping Refine Arguments")
+    refine_grp.add_argument(
+        "--refine-kmer-level-table",
+        help="""Tab-delimited file containing no header and two fields:
+        1. string k-mer sequence and 2. float expected normalized level.
+        All k-mers must be the same length and all combinations of the bases
+        'ACGT' must be present in the file.""",
+    )
+    refine_grp.add_argument(
+        "--refine-rough-rescale",
+        action="store_true",
+        help="""Apply a rough rescaling using quantiles of signal+move table
+        and levels.""",
+    )
+    refine_grp.add_argument(
+        "--refine-scale-iters",
+        default=0,
+        type=int,
+        help="""Number of iterations of signal mapping refinement and signal
+        re-scaling to perform. Set to 0 (default) in order to perform signal
+        mapping refinement, but skip re-scaling. Set to -1 to skip signal
+        mapping (potentially using levels for rough rescaling).""",
+    )
+    refine_grp.add_argument(
+        "--refine-half-bandwidth",
+        default=constants.DEFAULT_REFINE_HBW,
+        type=int,
+        help="""Half bandwidth around signal mapping over which to search for
+        new path.""",
+    )
+    refine_grp.add_argument(
+        "--refine-algo",
+        default=constants.DEFAULT_REFINE_ALGO,
+        choices=constants.REFINE_ALGOS,
+        help="Refinement algorithm to apply (if kmer level table is provided).",
+    )
+    refine_grp.add_argument(
+        "--refine-short-dwell-parameters",
+        default=constants.DEFAULT_REFINE_SHORT_DWELL_PARAMS,
+        type=float,
+        nargs=3,
+        metavar=("TARGET", "LIMIT", "WEIGHT"),
+        help="""Short dwell penalty refiner parameters. Dwells shorter than
+        LIMIT will be penalized a value of `WEIGHT * (dwell - TARGET)^2`.""",
+    )
+
+    plt_grp = subparser.add_argument_group("Plot Arguments")
+    plt_grp.add_argument(
+        "--figsize",
+        nargs=2,
+        type=int,
+        metavar=("HEIGHT", "WIDTH"),
+        default=constants.DEFAULT_PLOT_FIG_SIZE,
+        help="Figure size",
+    )
+    plt_grp.add_argument(
+        "--ylim",
+        nargs=2,
+        type=int,
+        metavar=("MIN", "MAX"),
+        help="Signal plotting limits",
+    )
+
+    out_grp = subparser.add_argument_group("Output Arguments")
+    out_grp.add_argument(
+        "--plots-filename",
+        default="remora_raw_signal_plot.pdf",
+        help="Output plots PDF file location.",
+    )
+    out_grp.add_argument(
+        "--log-filename",
+        help="Log filename. Default: Don't output log file.",
+    )
+
+    subparser.set_defaults(func=run_plot_ref_region)
+
+
+def run_plot_ref_region(args):
+    import pod5
+    import pysam
+    from matplotlib import pyplot as plt
+    from matplotlib.backends.backend_pdf import PdfPages
+
+    from remora import log, io, refine_signal_map
+
+    if args.log_filename is not None:
+        log.init_logger(args.log_filename)
+    pod5_paths, bc_paths = zip(*args.pod5_and_bam)
+    bam_fhs = [pysam.AlignmentFile(bc_path) for bc_path in bc_paths]
+    pod5_fhs = [pod5.Reader(pod5_path) for pod5_path in pod5_paths]
+    sig_map_refiner = refine_signal_map.SigMapRefiner(
+        kmer_model_filename=args.refine_kmer_level_table,
+        do_rough_rescale=args.refine_rough_rescale,
+        scale_iters=args.refine_scale_iters,
+        algo=args.refine_algo,
+        half_bandwidth=args.refine_half_bandwidth,
+        sd_params=args.refine_short_dwell_parameters,
+        do_fix_guage=True,
+    )
+    highlight_ranges = None
+    if args.highlight_ranges is not None:
+        highlight_ranges = io.parse_bed(args.highlight_ranges)
+
+    with PdfPages(args.plots_filename) as pdf_fh:
+        for ref_reg in io.parse_bed_lines(args.ref_regions):
+            reg_highlight_ranges = None
+            if highlight_ranges is not None:
+                try:
+                    reg_highlight_ranges = [
+                        (pos, pos + 1, args.highlight_color)
+                        for pos in highlight_ranges[
+                            (ref_reg.ctg, ref_reg.strand)
+                        ]
+                        if ref_reg.start <= pos < ref_reg.end
+                    ]
+                except KeyError:
+                    LOGGER.debug(f"No highlight values for region {ref_reg}")
+                    pass
+            fig, ax = plt.subplots(figsize=args.figsize)
+            io.plot_signal_at_ref_region(
+                ref_reg,
+                zip(pod5_fhs, bam_fhs),
+                sig_map_refiner,
+                fig_ax=(fig, ax),
+                ylim=args.ylim,
+                highlight_ranges=reg_highlight_ranges,
+            )
+            pdf_fh.savefig(fig, bbox_inches="tight")
+
+
+def register_estimate_kmer_levels(parser):
+    subparser = parser.add_parser(
+        "estimate_kmer_levels",
+        description="Estimate k-mer level table",
+        help="Estimate k-mer level table",
+        formatter_class=SubcommandHelpFormatter,
+    )
+
+    in_grp = subparser.add_argument_group("Input Arguments")
+    in_grp.add_argument(
+        "--pod5-and-bam",
+        required=True,
+        nargs=2,
+        metavar=("POD5", "BAM"),
+        action="append",
+        help="""POD5 signal path and BAM file path. BAM file must be mapped,
+        sorted and indexed and contain move table and MD tags. Multiple
+        samples can be supplied and will be aggregated after site level
+        extraction""",
+    )
+
+    refine_grp = subparser.add_argument_group("Signal Mapping Refine Arguments")
+    refine_grp.add_argument(
+        "--refine-kmer-level-table",
+        help="""Tab-delimited file containing no header and two fields:
+        1. string k-mer sequence and 2. float expected normalized level.
+        All k-mers must be the same length and all combinations of the bases
+        'ACGT' must be present in the file.""",
+    )
+    refine_grp.add_argument(
+        "--refine-rough-rescale",
+        action="store_true",
+        help="""Apply a rough rescaling using quantiles of signal+move table
+        and levels.""",
+    )
+    refine_grp.add_argument(
+        "--refine-scale-iters",
+        default=0,
+        type=int,
+        help="""Number of iterations of signal mapping refinement and signal
+        re-scaling to perform. Set to 0 (default) in order to perform signal
+        mapping refinement (aka resquiggle), but skip fine re-scaling. Set to
+        -1 to skip signal mapping (potentially using levels for rough
+        rescaling).""",
+    )
+    refine_grp.add_argument(
+        "--refine-half-bandwidth",
+        default=constants.DEFAULT_REFINE_HBW,
+        type=int,
+        help="""Half bandwidth around signal mapping over which to search for
+        new path.""",
+    )
+    refine_grp.add_argument(
+        "--refine-algo",
+        default=constants.DEFAULT_REFINE_ALGO,
+        choices=constants.REFINE_ALGOS,
+        help="Refinement algorithm to apply (if kmer level table is provided).",
+    )
+    refine_grp.add_argument(
+        "--refine-short-dwell-parameters",
+        default=constants.DEFAULT_REFINE_SHORT_DWELL_PARAMS,
+        type=float,
+        nargs=3,
+        metavar=("TARGET", "LIMIT", "WEIGHT"),
+        help="""Short dwell penalty refiner parameters. Dwells shorter than
+        LIMIT will be penalized a value of `WEIGHT * (dwell - TARGET)^2`.""",
+    )
+
+    data_grp = subparser.add_argument_group("Data Arguments")
+    data_grp.add_argument(
+        "--min-coverage",
+        type=int,
+        default=10,
+        help="Miniumum coverage to include a site.",
+    )
+    data_grp.add_argument(
+        "--kmer-context-bases",
+        nargs=2,
+        default=(2, 2),
+        type=int,
+        metavar=("BASES_BEFORE", "BASES_AFTER"),
+        help="""Definition of k-mer by the number of bases before and after the
+        assigned signal position""",
+    )
+
+    out_grp = subparser.add_argument_group("Output Arguments")
+    out_grp.add_argument(
+        "--levels-filename",
+        default="remora_kmer_levels.txt",
+        help="Output file for kmer levels.",
+    )
+    out_grp.add_argument(
+        "--log-filename",
+        help="Log filename. Default: Don't output log file.",
+    )
+
+    comp_grp = subparser.add_argument_group("Compute Arguments")
+    comp_grp.add_argument(
+        "--num-workers",
+        type=int,
+        default=1,
+        help="Number of workers.",
+    )
+    comp_grp.add_argument(
+        "--chunk-width",
+        type=int,
+        default=1_000,
+        help="""Width of reference region to process at one time. Should be
+        smaller for very high coverage.""",
+    )
+    comp_grp.add_argument(
+        "--max-chunk-coverage",
+        type=int,
+        default=100,
+        help="Maxiumum mean chunk coverage for each region.",
+    )
+
+    subparser.set_defaults(func=run_estimate_kmer_levels)
+
+
+def run_estimate_kmer_levels(args):
+    from itertools import product
+
+    import pysam
+    import numpy as np
+
+    from remora import log, io, refine_signal_map
+
+    if args.log_filename is not None:
+        log.init_logger(args.log_filename)
+    # open first to avoid long process without write access
+    out_fh = open(args.levels_filename, "w")
+
+    sig_map_refiner = refine_signal_map.SigMapRefiner(
+        kmer_model_filename=args.refine_kmer_level_table,
+        do_rough_rescale=args.refine_rough_rescale,
+        scale_iters=args.refine_scale_iters,
+        algo=args.refine_algo,
+        half_bandwidth=args.refine_half_bandwidth,
+        sd_params=args.refine_short_dwell_parameters,
+        do_fix_guage=True,
+    )
+    if not sig_map_refiner.is_loaded or sig_map_refiner.scale_iters < 0:
+        LOGGER.warning(
+            "It is highly recommended to apply signal mapping refinement in "
+            "order to output a valid kmer level table."
+        )
+
+    kmer_len = sum(args.kmer_context_bases) + 1
+    all_kmer_levels = dict(
+        ("".join(bs), []) for bs in product("ACGT", repeat=kmer_len)
+    )
+    for pod5_path, bam_path in args.pod5_and_bam:
+        try:
+            with pysam.AlignmentFile(bam_path) as bam_fh:
+                _ = bam_fh.fetch(bam_fh.header.references[0], 0, 1)
+        except ValueError:
+            LOGGER.warning(
+                "Cannot estimate levels from BAM file without mappings or index"
+            )
+            continue
+        LOGGER.info(f"Extracting levels from {pod5_path} and {bam_path}")
+        for kmer, levels in io.get_site_kmer_levels(
+            pod5_path,
+            bam_path,
+            sig_map_refiner,
+            args.kmer_context_bases,
+            min_cov=args.min_coverage,
+            chunk_len=args.chunk_width,
+            max_chunk_cov=args.max_chunk_coverage,
+            num_workers=args.num_workers,
+        ).items():
+            all_kmer_levels[kmer].append(levels)
+    LOGGER.info("Aggregating and outputting levels")
+    been_warned = False
+    for kmer, levels in sorted(all_kmer_levels.items()):
+        levels = np.concatenate(levels)
+        if levels.size == 0:
+            if not been_warned:
+                LOGGER.warning("Some k-mers not observed.")
+                been_warned = True
+            out_fh.write(f"{kmer}\tnan\n")
+        else:
+            out_fh.write(f"{kmer}\t{np.median(levels)}\n")
+    out_fh.close()
```

### Comparing `ont-remora-2.0.0/src/remora/prepare_train_data.py` & `ont-remora-2.1.0/src/remora/prepare_train_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,19 @@
+import os
 from pathlib import Path
 from collections import defaultdict
 
 import pod5
-import pysam
 import numpy as np
 from tqdm import tqdm
 
 from remora import log, RemoraError
-from remora.util import MultitaskMap, BackgroundIter
-from remora.data_chunks import (
-    RemoraRead,
-    RemoraDataset,
-    compute_ref_to_signal,
-)
-from remora.io import (
-    index_bam,
-    iter_signal,
-    extract_signal,
-    iter_alignments,
-    read_is_primary,
-    extract_alignments,
-    prep_extract_signal,
-    prep_extract_alignments,
-)
+from remora.util import MultitaskMap, BackgroundIter, get_read_ids
+from remora.io import ReadIndexedBam, iter_signal, extract_alignments
+from remora.data_chunks import RemoraRead, RemoraDataset, compute_ref_to_signal
 
 LOGGER = log.get_logger()
 
 
 ####################
 # Chunk extraction #
 ####################
@@ -40,48 +27,48 @@
     sig_map_refiner,
     max_chunks_per_read,
     chunk_context,
     kmer_context_bases,
     base_pred,
     base_start_justify,
     offset,
-    basecall_anchored,
+    basecall_anchor,
 ):
     read_chunks = []
     for read_idx, (io_read, err) in enumerate(read_errs):
         if io_read is None:
             read_chunks.append(tuple((io_read, err)))
             continue
         if io_read.ref_seq is None:
             read_chunks.append(
                 tuple((None, "No reference sequence (missing MD tag)"))
             )
             continue
-        if basecall_anchored:
+        if basecall_anchor:
             remora_read = io_read.into_remora_read(use_reference_anchor=False)
-            remora_read.focus_bases = (
-                io_read.get_base_call_anchored_focus_bases(
-                    motifs=motifs,
-                    select_focus_reference_positions=focus_ref_pos,
-                )
+            remora_read.focus_bases = io_read.get_basecall_anchored_focus_bases(
+                motifs=motifs,
+                select_focus_reference_positions=focus_ref_pos,
             )
             remora_read.labels = np.full(len(io_read.seq), int_label, dtype=int)
         else:
             io_read.ref_to_signal = compute_ref_to_signal(
                 io_read.query_to_signal,
                 io_read.cigar,
-                query_seq=io_read.seq,
-                ref_seq=io_read.ref_seq,
             )
-            trim_signal = io_read.signal[
+            assert io_read.ref_to_signal.size == len(io_read.ref_seq) + 1, (
+                "discordant ref seq lengths: move+cigar:"
+                f"{io_read.ref_to_signal.size} ref_seq:{len(io_read.ref_seq)}"
+            )
+            trim_dacs = io_read.dacs[
                 io_read.ref_to_signal[0] : io_read.ref_to_signal[-1]
             ]
             shift_ref_to_sig = io_read.ref_to_signal - io_read.ref_to_signal[0]
             remora_read = RemoraRead(
-                dacs=trim_signal,
+                dacs=trim_dacs,
                 shift=io_read.shift_dacs_to_norm,
                 scale=io_read.scale_dacs_to_norm,
                 seq_to_sig_map=shift_ref_to_sig,
                 str_seq=io_read.ref_seq,
                 labels=np.full(len(io_read.ref_seq), int_label, dtype=int),
                 read_id=io_read.read_id,
             )
@@ -139,99 +126,65 @@
     base_pred,
     kmer_context_bases,
     base_start_justify,
     offset,
     num_reads,
     num_extract_alignment_threads,
     num_extract_chunks_threads,
-    signal_first=True,
     skip_non_primary=True,
-    base_call_anchor=False,
+    basecall_anchor=False,
+    rev_sig=False,
 ):
-    if signal_first:
-        bam_idx, num_bam_reads = index_bam(bam_fn, skip_non_primary)
-        with pod5.Reader(Path(pod5_path)) as pod5_fp:
-            num_pod5_reads = sum(1 for _ in pod5_fp.reads())
-            LOGGER.info(
-                f"Found {num_bam_reads} BAM records and "
-                f"{num_pod5_reads} POD5 reads"
-            )
-            if num_reads is None:
-                num_reads = min(num_pod5_reads, num_bam_reads)
-            else:
-                num_reads = min(num_reads, num_pod5_reads, num_bam_reads)
-    else:
-        LOGGER.info("Counting reads in BAM file")
-        pysam_save = pysam.set_verbosity(0)
-        with pysam.AlignmentFile(bam_fn, mode="rb", check_sq=False) as bam_fp:
-            num_bam_reads = bam_fp.count(
-                until_eof=True, read_callback=read_is_primary
-            )
-            LOGGER.info(f"Found {num_bam_reads} BAM records")
-            if num_reads is None:
-                num_reads = num_bam_reads
-            else:
-                num_reads = min(num_reads, num_bam_reads)
-        pysam.set_verbosity(pysam_save)
+    bam_idx = ReadIndexedBam(bam_fn, skip_non_primary)
+    with pod5.Reader(Path(pod5_path)) as pod5_fh:
+        read_ids, num_reads = get_read_ids(bam_idx, pod5_fh, num_reads)
+    if num_reads == 0:
+        return
 
     LOGGER.info(
-        f"Making {'base call' if base_call_anchor else 'reference'}-"
+        f"Making {'basecall' if basecall_anchor else 'reference'}-"
         f"anchored training data"
     )
     LOGGER.info("Allocating memory for output tensors")
     # initialize empty dataset with pre-allocated memory
     dataset = RemoraDataset.allocate_empty_chunks(
         num_chunks=max_chunks_per_read * num_reads,
         chunk_context=chunk_context,
         kmer_context_bases=kmer_context_bases,
         min_samps_per_base=min_samps_per_base,
         base_pred=base_pred,
         mod_bases=[] if mod_base_control else [mod_base[0]],
         mod_long_names=[] if mod_base_control else [mod_base[1]],
         motifs=[mot.to_tuple() for mot in motifs],
+        reverse_signal=rev_sig,
         sig_map_refiner=sig_map_refiner,
         base_start_justify=base_start_justify,
         offset=offset,
     )
 
-    assert len(bam_idx.keys()) > 0
-
     LOGGER.info("Processing reads")
-    if signal_first:
-        signals = BackgroundIter(
-            iter_signal,
-            args=(pod5_path, num_reads, list(bam_idx.keys())),
-            name="ExtractSignal",
-            use_process=True,
-        )
-        reads = MultitaskMap(
-            extract_alignments,
-            signals,
-            prep_func=prep_extract_alignments,
-            num_workers=num_extract_alignment_threads,
-            args=(bam_idx, bam_fn),
-            name="AddAlignments",
-            use_process=True,
-        )
-    else:
-        mappings = BackgroundIter(
-            iter_alignments,
-            args=(bam_fn, num_reads, skip_non_primary),
-            name="ExtractMappings",
-            use_process=True,
-        )
-        reads = MultitaskMap(
-            extract_signal,
-            mappings,
-            prep_func=prep_extract_signal,
-            num_workers=num_extract_alignment_threads,
-            args=(pod5_path,),
-            name="AddSignal",
-            use_process=True,
-        )
+    signals = BackgroundIter(
+        iter_signal,
+        args=(pod5_path,),
+        kwargs={
+            "num_reads": num_reads,
+            "read_ids": read_ids,
+            "rev_sig": rev_sig,
+        },
+        name="ExtractSignal",
+        use_process=True,
+    )
+    reads = MultitaskMap(
+        extract_alignments,
+        signals,
+        num_workers=num_extract_alignment_threads,
+        args=(bam_idx, rev_sig),
+        name="AddAlignments",
+        use_process=True,
+    )
     chunks = MultitaskMap(
         extract_chunks,
         reads,
         num_workers=num_extract_chunks_threads,
         args=[
             0 if mod_base_control else 1,
             motifs,
@@ -239,27 +192,28 @@
             sig_map_refiner,
             max_chunks_per_read,
             chunk_context,
             kmer_context_bases,
             base_pred,
             base_start_justify,
             offset,
-            base_call_anchor,
+            basecall_anchor,
         ],
         name="ExtractChunks",
         use_process=True,
     )
 
     errs = defaultdict(int)
     for read_chunks in tqdm(
         chunks,
         total=num_reads,
         smoothing=0,
         unit=" Reads",
         desc="Extracting chunks",
+        disable=os.environ.get("LOG_SAFE", False),
     ):
         if len(read_chunks) == 0:
             errs["No chunks extracted"] += 1
             continue
         for read_align_chunks, err in read_chunks:
             if read_align_chunks is None:
                 errs[err] += 1
```

### Comparing `ont-remora-2.0.0/src/remora/refine_signal_map.py` & `ont-remora-2.1.0/src/remora/refine_signal_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from scipy import stats
 
 from remora import RemoraError, log
 from remora.constants import (
     DEFAULT_REFINE_HBW,
     DEFAULT_REFINE_SHORT_DWELL_PARAMS,
     DEFAULT_REFINE_ALGO,
-    DEFAULT_REFINE_BAND_MIN_STEP,
     REFINE_ALGO_DWELL_PEN_NAME,
-    DEFAULT_REFINE_SCALE_ITERS,
 )
 from remora.refine_signal_map_core import (
     seq_banded_dp,
     extract_levels,
     adjust_seq_band,
 )
 
@@ -108,15 +106,15 @@
 
     Args:
         TODO
     """
 
     kmer_model_filename: str = None
     do_rough_rescale: bool = True
-    scale_iters: int = DEFAULT_REFINE_SCALE_ITERS
+    scale_iters: int = -1
     algo: str = DEFAULT_REFINE_ALGO
     half_bandwidth: int = DEFAULT_REFINE_HBW
     sd_params: tuple = None
     do_fix_guage: bool = False
 
     sd_arr: np.ndarray = DEFAULT_REFINE_SHORT_DWELL_PEN
     _levels_array: np.ndarray = None
@@ -142,17 +140,34 @@
         if self.scale_iters >= 0:
             r_str += (
                 " Signal mapping refinement will be executed using the "
                 f"{self.algo} refinement method (band half width: "
                 f"{self.half_bandwidth})."
             )
             if self.algo == REFINE_ALGO_DWELL_PEN_NAME:
-                r_str += f" Short dwell penalty array set to {self.sd_params}."
+                r_str += f" Short dwell penalty array set to {self.sd_arr}."
         return r_str
 
+    @property
+    def bases_before(self):
+        """Number of bases in k-mer before the central base"""
+        return self.center_idx
+
+    @property
+    def bases_after(self):
+        """Number of bases in k-mer after the central base"""
+        return self.kmer_len - self.center_idx - 1
+
+    def write_kmer_table(self, fh):
+        for kmer in product(*["ACGT"] * self.kmer_len):
+            fh.write(
+                f"{''.join(kmer)}\t"
+                f"{self._levels_array[index_from_kmer(kmer)]}\n"
+            )
+
     def load_kmer_table(self):
         self.str_kmer_levels = {}
         with open(self.kmer_model_filename) as kmer_fp:
             self.kmer_len = len(kmer_fp.readline().split()[0])
             kmer_fp.seek(0)
             for line in kmer_fp:
                 kmer, level = line.split()
@@ -204,34 +219,50 @@
             kmer_idx_stats.append(stats.kruskal(*kmer_idx_pos)[0])
             kmer_summ += f"\t{kmer_idx}\t{kmer_idx_stats[-1]:10.2f}\n"
         self.center_idx = np.argmax(kmer_idx_stats)
         LOGGER.debug(f"K-mer index stats:\n{kmer_summ}")
         LOGGER.debug(f"Choosen central position: {self.center_idx}")
 
     def __post_init__(self):
+        # determine if level model is loaded from any of 3 options
         if self._levels_array is not None and not np.array_equal(
             self._levels_array, np.array(None)
         ):
             self.is_loaded = True
             self.kmer_len = int(np.log(self._levels_array.size) / np.log(4))
             assert 4**self.kmer_len == self._levels_array.size
         elif self.kmer_model_filename is not None:
             self.load_kmer_table()
             self.is_loaded = True
             self.determine_dominant_pos()
             if self.do_fix_guage:
                 self.fix_gauge()
+        elif self.str_kmer_levels is not None:
+            self.is_loaded = True
+            self.determine_dominant_pos()
+            if self.do_fix_guage:
+                self.fix_gauge()
+
         if self.sd_params is not None:
             self.sd_arr = compute_dwell_pen_array(*self.sd_params)
         if (
             self.is_loaded
             and self.scale_iters >= 0
             and self.algo == REFINE_ALGO_DWELL_PEN_NAME
         ):
-            LOGGER.info(f"Refine short dwell penalty array: {self.sd_arr}")
+            LOGGER.debug(f"Refine short dwell penalty array: {self.sd_arr}")
+        if (
+            self.is_loaded
+            and not self.do_rough_rescale
+            and self.scale_iters < 0
+        ):
+            LOGGER.warning(
+                "K-mer table provided, but not used. "
+                "See rough rescaling options."
+            )
 
     def extract_levels(self, int_seq):
         return extract_levels(
             int_seq.astype(np.int32),
             self.levels_array,
             self.kmer_len,
             self.center_idx,
@@ -399,14 +430,42 @@
             do_rough_rescale=bool(int(data["refine_do_rough_rescale"].item())),
             scale_iters=int(data["refine_scale_iters"].item()),
             algo=str(data["refine_algo"].item()),
             half_bandwidth=int(data["refine_half_bandwidth"].item()),
             sd_arr=data["refine_sd_arr"],
         )
 
+    @classmethod
+    def load_from_dict(
+        cls,
+        data,
+        do_rough_rescale=True,
+        scale_iters=-1,
+        algo=DEFAULT_REFINE_ALGO,
+        half_bandwidth=DEFAULT_REFINE_HBW,
+        sd_params=None,
+        do_fix_guage=False,
+        sd_arr=DEFAULT_REFINE_SHORT_DWELL_PEN,
+    ):
+        """Create refiner from str_kmer_levels dict with kmer keys and float
+        current level values.
+        """
+        kmer_len = len(next(iter(data.keys())))
+        return cls(
+            do_rough_rescale=do_rough_rescale,
+            scale_iters=scale_iters,
+            algo=algo,
+            half_bandwidth=half_bandwidth,
+            sd_params=sd_params,
+            do_fix_guage=do_fix_guage,
+            sd_arr=sd_arr,
+            str_kmer_levels=data,
+            kmer_len=kmer_len,
+        )
+
 
 ###########
 # Banding #
 ###########
 
 
 def compute_sig_band(bps, levels, bhw=DEFAULT_REFINE_HBW, is_banded=True):
@@ -556,26 +615,29 @@
 def refine_signal_mapping(
     signal,
     seq_to_sig_map,
     levels,
     band_half_width=DEFAULT_REFINE_HBW,
     refine_algo=DEFAULT_REFINE_ALGO,
     short_dwell_pen=DEFAULT_REFINE_SHORT_DWELL_PEN,
+    adjust_band_min_step=2,
 ):
     """Refine input signal mapping to minimize difference difference between
     signal and levels.
 
     Args:
         signal (np.ndarray): Float32 array containing normalized signal values.
         seq_to_sig_map (np.ndarray): Int32 array with locations within
             signal for each base represented by levels. `seq_to_sig_map.size`
             should equal `levels.size + 1` in order to include the end of the
             last base. Values should be monotonically increasing (ties allowed).
         levels (np.ndarray): Float32 array containing estimated levels.
         band_half_width (int): Half bandwidth
+        adjust_band_min_step (int): Minimum step between one base and the next
+            to enforce in band adjustment.
 
     Returns:
         2-tuple containing:
             1. Signal mapping
             2. Mapping score
     """
     # Note that there is no guarantee the seq_to_sig_map go right to the end
@@ -590,15 +652,15 @@
     # TODO compute seq band directly with anti-diagonal band
     sig_band = compute_sig_band(
         seq_to_sig_map,
         levels,
         bhw=band_half_width,
     )
     seq_band = convert_to_seq_band(sig_band)
-    adjust_seq_band(seq_band, min_step=DEFAULT_REFINE_BAND_MIN_STEP)
+    adjust_seq_band(seq_band, min_step=adjust_band_min_step)
     validate_band(
         seq_band,
         sig_len=signal.shape[0],
         seq_len=levels.shape[0],
         is_sig_band=False,
     )
```

### Comparing `ont-remora-2.0.0/src/remora/refine_signal_map_core.pyx` & `ont-remora-2.1.0/src/remora/refine_signal_map_core.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 )
 
 
 ###########
 # Banding #
 ###########
 
-def adjust_seq_band(int[:, ::1] seq_band, int min_step=1):
+def adjust_seq_band(int[:, ::1] seq_band, int min_step=2):
     """Adjust band boundaries to disallow invalid paths. Namely, make sure each
     band start and end is at least one greater than the previous.
 
     Note input band will be updated in place
 
     Args:
         seq_band (np.ndarray): int32 np.ndarray with shape
             (2, seq_len = levels.shape[0]). The first row contains the lower
             band boundaries in signal coordinates and the second row contains
             the upper boundaries in signal coordinates. The first lower bound
             should be 0 and last upper bound should be signal.shape[0].
-       min_step (int): Minimum step between one base and the next to enforce
+        min_step (int): Minimum step between one base and the next to enforce
             in band adjustment.
     """
     cdef int band_min = seq_band[0, 0]
     cdef int seq_pos
     # fix starts to make sure each start is at least min_step less than prev
     for seq_pos in range(seq_band.shape[1] - 2, -1, -1):
         if seq_band[0, seq_pos] > seq_band[0, seq_pos + 1] - min_step:
@@ -89,15 +89,15 @@
     const float[::1] int_kmer_levels,
     int kmer_len,
     int center_idx
 ):
     levels = np.zeros(int_seq.shape[0], dtype=np.float32)
     cdef float[::1] levels_mv = levels
     cdef int pos, center_pos, kmer_idx
-    for pos in range(int_seq.shape[0] - kmer_len):
+    for pos in range(int_seq.shape[0] - kmer_len + 1):
         center_pos = pos + center_idx
         kmer_idx = index_from_int_kmer(int_seq[pos : pos + kmer_len], kmer_len)
         levels_mv[center_pos] = int_kmer_levels[kmer_idx]
     return levels
 
 
 ######################
```

### Comparing `ont-remora-2.0.0/src/remora/train_model.py` & `ont-remora-2.1.0/src/remora/train_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -104,40 +104,38 @@
     scheduler_name,
     weight_decay,
     epochs,
     save_freq,
     early_stopping,
     filt_frac,
     ext_val,
+    ext_val_names,
     lr_sched_kwargs,
     balance,
-    balanced_batch,
+    batch_label_weights,
+    high_conf_incorrect_thr_frac,
 ):
     seed = (
         np.random.randint(0, np.iinfo(np.uint32).max, dtype=np.uint32)
         if seed is None
         else seed
     )
     LOGGER.info(f"Seed selected is {seed}")
 
     np.random.seed(seed)
     torch.manual_seed(seed)
-    if torch.cuda.is_available() and device is not None:
+    if device is not None and device.type == "cuda":
         torch.cuda.manual_seed_all(seed)
         torch.cuda.set_device(device)
-    elif device is not None:
-        LOGGER.warning(
-            "Device option specified, but CUDA is not available from torch."
-        )
 
     LOGGER.info("Loading dataset from Remora file")
     dataset = RemoraDataset.load_from_file(
         remora_dataset_path,
         batch_size=batch_size,
-        balanced_batch=balanced_batch,
+        drop_read_attrs=True,
     )
     LOGGER.info(f"Dataset loaded with labels: {dataset.get_label_counts()}")
     if balance:
         dataset = dataset.balance_classes()
         LOGGER.info(f"Dataset balanced: {dataset.get_label_counts()}")
     dataset.trim_kmer_context_bases(kmer_context_bases)
     dataset.trim_chunk_context(chunk_context)
@@ -145,44 +143,52 @@
     LOGGER.info(f"Dataset summary:\n{dataset.summary}")
 
     val_fp = open(out_path / "validation.log", mode="w", buffering=1)
     atexit.register(val_fp.close)
     val_fp = validate.ValidationLogger(val_fp)
     batch_fp = open(out_path / "batch.log", "w", buffering=1)
     atexit.register(batch_fp.close)
-    batch_fp.write("Iteration\tLoss\n")
+    if high_conf_incorrect_thr_frac is not None:
+        batch_fp.write("Iteration\tLoss\tNumberFiltered\n")
+    else:
+        batch_fp.write("Iteration\tLoss\n")
 
     LOGGER.info("Loading model")
     copy_model_path = util.resolve_path(os.path.join(out_path, "model.py"))
     copyfile(model_path, copy_model_path)
     num_out = 4 if dataset.base_pred else len(dataset.mod_bases) + 1
     model_params = {
         "size": size,
         "kmer_len": sum(dataset.kmer_context_bases) + 1,
         "num_out": num_out,
     }
     model = model_util._load_python_model(copy_model_path, **model_params)
     LOGGER.info(f"Model structure:\n{model}")
 
     if ext_val:
+        if ext_val_names is None:
+            ext_val_names = [f"e_val_{idx}" for idx in range(len(ext_val))]
+        else:
+            assert len(ext_val_names) == len(ext_val)
         ext_sets = []
-        for path in ext_val:
+        for e_name, e_path in zip(ext_val_names, ext_val):
             ext_val_set = RemoraDataset.load_from_file(
-                path.strip(),
+                e_path.strip(),
                 batch_size=batch_size,
                 shuffle_on_iter=False,
                 drop_last=False,
+                drop_read_attrs=True,
             )
             if ext_val_set.mod_long_names != dataset.mod_long_names:
                 ext_val_set.add_fake_base(
                     dataset.mod_long_names, dataset.mod_bases
                 )
             ext_val_set.trim_kmer_context_bases(kmer_context_bases)
             ext_val_set.trim_chunk_context(chunk_context)
-            ext_sets.append(ext_val_set)
+            ext_sets.append((e_name, ext_val_set))
 
     kmer_dim = int((sum(dataset.kmer_context_bases) + 1) * 4)
     test_input_sig = torch.randn(batch_size, 1, sum(dataset.chunk_context))
     test_input_seq = torch.randn(
         batch_size, kmer_dim, sum(dataset.chunk_context)
     )
     macs, params = profile(
@@ -190,33 +196,39 @@
     )
     LOGGER.info(
         f" Params (k) {params / (1000):.2f} | MACs (M) {macs / (1000 ** 2):.2f}"
     )
 
     LOGGER.info("Preparing training settings")
     criterion = torch.nn.CrossEntropyLoss()
-    if torch.cuda.is_available():
-        model = model.cuda()
-        criterion = criterion.cuda()
+    model = model.to(device)
+    criterion = criterion.to(device)
     opt = load_optimizer(optimizer, model, lr, weight_decay)
 
     scheduler = select_scheduler(scheduler_name, opt, lr_sched_kwargs)
 
     label_counts = dataset.get_label_counts()
     LOGGER.info(f"Label distribution: {label_counts}")
     if len(label_counts) <= 1:
         raise RemoraError(
             "One or fewer output labels found. Ensure --focus-offset and "
             "--mod are specified correctly"
         )
+    LOGGER.debug("Splitting dataset")
     trn_ds, val_ds = dataset.split_data(val_prop=val_prop, stratified=True)
-    trn_ds.shuffle()
+    LOGGER.debug("Extracting head of train dataset")
     val_trn_ds = trn_ds.head(
-        prop=val_prop, shuffle_on_iter=False, drop_last=False
+        prop=val_prop, shuffle_on_iter=False, drop_last=False, stratified=True
     )
+    if batch_label_weights is not None:
+        LOGGER.debug("Applying batch label proportions")
+        trn_ds.batch_label_props = np.array(batch_label_weights) / sum(
+            batch_label_weights
+        )
+        trn_ds.order_chunks_by_batch_labels()
     LOGGER.info(f"Train label distribution: {trn_ds.get_label_counts()}")
     LOGGER.info(
         f"Held-out validation label distribution: {val_ds.get_label_counts()}"
     )
     LOGGER.info(
         "Training set validation label distribution: "
         f"{val_trn_ds.get_label_counts()}"
@@ -233,41 +245,43 @@
         criterion,
         val_trn_ds,
         filt_frac,
         "trn",
     )
 
     if ext_val:
-        best_alt_val_accs = [0] * len(ext_sets)
-        for e_set_idx in range(len(ext_sets)):
+        best_alt_val_accs = dict((e_name, 0) for e_name, _ in ext_sets)
+        for e_name, e_set in ext_sets:
             val_fp.validate_model(
                 model,
                 dataset.mod_bases,
                 criterion,
-                ext_sets[e_set_idx],
+                e_set,
                 filt_frac,
-                f"e_val_{e_set_idx}",
+                e_name,
             )
 
     LOGGER.info("Start training")
     ebar = tqdm(
         total=epochs,
         smoothing=0,
         desc="Epochs",
         dynamic_ncols=True,
         position=0,
         leave=True,
+        disable=os.environ.get("LOG_SAFE", False),
     )
     pbar = tqdm(
         total=len(trn_ds),
         desc="Epoch Progress",
         dynamic_ncols=True,
         position=1,
         leave=True,
         bar_format="{desc}: {percentage:3.0f}%|{bar}| " "{n_fmt}/{total_fmt}",
+        disable=os.environ.get("LOG_SAFE", False),
     )
     ebar.set_postfix(
         acc_val=f"{val_metrics.acc:.4f}",
         acc_train=f"{trn_metrics.acc:.4f}",
         loss_val=f"{val_metrics.loss:.6f}",
         loss_train=f"{trn_metrics.loss:.6f}",
     )
@@ -280,14 +294,15 @@
         "opt": opt.state_dict(),
         "model_path": copy_model_path,
         "model_params": model_params,
         "chunk_context": dataset.chunk_context,
         "fixed_seq_len_chunks": model._variable_width_possible,
         "motifs": dataset.motifs,
         "num_motifs": dataset.num_motifs,
+        "reverse_signal": dataset.reverse_signal,
         "mod_bases": dataset.mod_bases,
         "mod_long_names": dataset.mod_long_names,
         "base_pred": dataset.base_pred,
         "kmer_context_bases": dataset.kmer_context_bases,
         "base_start_justify": dataset.base_start_justify,
         "offset": dataset.offset,
         "model_version": constants.MODEL_VERSION,
@@ -307,50 +322,78 @@
             sigs = torch.from_numpy(sigs)
             enc_kmers = torch.from_numpy(
                 encoded_kmers.compute_encoded_kmer_batch(
                     bb, ab, seqs, seq_maps, seq_lens
                 )
             )
             labels = torch.from_numpy(labels)
-            if torch.cuda.is_available():
-                sigs = sigs.cuda()
-                enc_kmers = enc_kmers.cuda()
-                labels = labels.cuda()
+            sigs = sigs.to(device)
+            enc_kmers = enc_kmers.to(device)
             outputs = model(sigs, enc_kmers)
-            loss = criterion(outputs, labels)
+
+            if high_conf_incorrect_thr_frac is None:
+                labels = labels.to(device)
+                loss = criterion(outputs, labels)
+            else:
+                batch_size = outputs.shape[0]
+                conf_thresh, max_frac_skip = high_conf_incorrect_thr_frac
+                max_nr_skip = int(np.floor(batch_size * max_frac_skip))
+                preds = (
+                    torch.nn.functional.softmax(outputs, dim=1).detach().cpu()
+                )
+                highest_preds, high_conf_cl = torch.max(preds, dim=1)
+                cl_match = labels == high_conf_cl
+                # if there are more mismatches than the maximum number allowed
+                # to be skipped, set confidence threshold to allow no more than
+                # max_nr_skip items be skipped
+                if batch_size - cl_match.sum() > max_nr_skip:
+                    mm_preds = highest_preds[~cl_match]
+                    mm_preds.sort(descending=True)
+                    conf_thresh = max(conf_thresh, mm_preds[max_nr_skip])
+                mask = cl_match.logical_or(highest_preds < conf_thresh)
+                # avoid sending labels to device until after above computations
+                labels = labels.to(device)
+                loss = criterion(outputs[mask], labels[mask])
+
             opt.zero_grad()
             loss.backward()
             opt.step()
-
             batch_fp.write(
                 f"{(epoch * len(trn_ds)) + epoch_i}\t"
-                f"{loss.detach().cpu():.6f}\n"
+                f"{loss.detach().cpu():.6f}"
             )
+            if high_conf_incorrect_thr_frac is None:
+                batch_fp.write("\n")
+            else:
+                batch_fp.write(f"\t{batch_size - mask.sum()}\n")
+
             pbar.update()
             pbar.refresh()
 
         niter = (epoch + 1) * len(trn_ds)
         val_metrics = val_fp.validate_model(
             model,
             dataset.mod_bases,
             criterion,
             val_ds,
             filt_frac,
             nepoch=epoch + 1,
             niter=niter,
+            disable_pbar=True,
         )
         trn_metrics = val_fp.validate_model(
             model,
             dataset.mod_bases,
             criterion,
             val_trn_ds,
             filt_frac,
             "trn",
             nepoch=epoch + 1,
             niter=niter,
+            disable_pbar=True,
         )
 
         scheduler.step()
 
         if breached:
             if val_metrics.acc <= REGRESSION_THRESHOLD:
                 LOGGER.warning("Remora training unstable")
@@ -375,42 +418,43 @@
                 epoch,
                 opt,
             )
         else:
             early_stop_epochs += 1
 
         if ext_val:
-            for e_set_idx in range(len(ext_sets)):
+            for e_name, e_set in ext_sets:
                 e_val_metrics = val_fp.validate_model(
                     model,
                     dataset.mod_bases,
                     criterion,
-                    ext_sets[e_set_idx],
+                    e_set,
                     filt_frac,
-                    f"e_val_{e_set_idx}",
+                    e_name,
                     nepoch=epoch + 1,
                     niter=niter,
+                    disable_pbar=True,
                 )
-                if e_val_metrics.acc <= best_alt_val_accs[e_set_idx]:
+                if e_val_metrics.acc <= best_alt_val_accs[e_name]:
                     continue
-                best_alt_val_accs[e_set_idx] = e_val_metrics.acc
+                best_alt_val_accs[e_name] = e_val_metrics.acc
                 early_stop_epochs = 0
                 LOGGER.debug(
-                    f"Saving best model based on e_val_{e_set_idx} "
-                    f"validation sets after {epoch + 1} epochs "
+                    f"Saving best model based on {e_name} "
+                    f"validation set after {epoch + 1} epochs "
                     f"with val_acc {e_val_metrics.acc}"
                 )
                 save_model(
                     model,
                     ckpt_save_data,
                     out_path,
                     epoch,
                     opt,
-                    model_name=f"model_e_val_{e_set_idx}_best.checkpoint",
-                    model_name_torchscript=f"model_e_val_{e_set_idx}_best.pt",
+                    model_name=f"model_ext_val_{e_name}_best.checkpoint",
+                    model_name_torchscript=f"model_ext_val_{e_name}_best.pt",
                 )
 
         if int(epoch + 1) % save_freq == 0:
             save_model(
                 model,
                 ckpt_save_data,
                 out_path,
```

### Comparing `ont-remora-2.0.0/src/remora/util.py` & `ont-remora-2.1.0/src/remora/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import re
 import array
-import multiprocessing as mp
-import platform
 import queue
-import re
+import platform
 import traceback
 from time import sleep
+import multiprocessing as mp
 from threading import Thread
 from os.path import realpath, expanduser
 
+import torch
 import numpy as np
 
 from remora import log, RemoraError
 
 LOGGER = log.get_logger()
 
 CAN_ALPHABET = "ACGT"
@@ -38,18 +39,33 @@
 SEQ_TO_INT_ARR[0] = 0
 SEQ_TO_INT_ARR[2] = 1
 SEQ_TO_INT_ARR[6] = 2
 SEQ_TO_INT_ARR[19] = 3
 COMP_BASES = dict(zip(map(ord, "ACGT"), map(ord, "TGCA")))
 NP_COMP_BASES = np.array([3, 2, 1, 0], dtype=np.uintp)
 U_TO_T_BASES = {ord("U"): ord("T")}
+T_TO_U_BASES = {ord("T"): ord("U")}
 
 DEFAULT_QUEUE_SIZE = 10_000
 
 
+def parse_device(device):
+    if device is None:
+        return None
+    # convert int devices for legacy settings
+    try:
+        device = int(device)
+    except (ValueError, TypeError):
+        pass
+    device = torch.device(device)
+    if device.type == "cuda" and not torch.cuda.is_available():
+        LOGGER.warning("Device option specified, but CUDA not available.")
+    return device
+
+
 def iter_motif_hits(int_seq, motif):
     yield from np.where(
         np.logical_and.reduce(
             [
                 np.isin(
                     int_seq[
                         po : int_seq.size - len(motif.int_pattern) + po + 1
@@ -91,14 +107,18 @@
     return NP_COMP_BASES[np_seq][::-1]
 
 
 def u_to_t(seq):
     return seq.translate(U_TO_T_BASES)
 
 
+def t_to_u(seq):
+    return seq.translate(T_TO_U_BASES)
+
+
 def seq_to_int(seq):
     """Convert string sequence to integer encoded array
 
     Args:
         seq (str): Nucleotide sequence
 
     Returns:
@@ -149,14 +169,43 @@
 def softmax_axis1(x):
     """Compute softmax over axis=1"""
     e_x = np.exp((x.T - np.max(x, axis=1)).T)
     with np.errstate(divide="ignore"):
         return (e_x.T / e_x.sum(axis=1)).T
 
 
+def get_read_ids(bam_idx, pod5_fh, num_reads):
+    """Get overlapping read ids from bam index and pod5 file
+
+    Args:
+        bam_idx (ReadIndexedBam): Read indexed BAM
+        pod5_fh (pod5.Reader): POD5 file handle
+        num_reads (int): Maximum number of reads, or None for no max
+    """
+    LOGGER.info("Extracting read IDs from POD5")
+    pod5_read_ids = set(pod5_fh.read_ids)
+    num_pod5_reads = len(pod5_read_ids)
+    # pod5 will raise when it cannot find a "selected" read id, so we make
+    # sure they're all present before starting
+    # todo(arand) this could be performed using the read_table instead, but
+    #  it's worth checking that it's actually faster and doesn't explode
+    #  memory before switching from a sweep throug the pod5 file
+    both_read_ids = list(pod5_read_ids.intersection(bam_idx.read_ids))
+    num_both_read_ids = len(both_read_ids)
+    LOGGER.info(
+        f"Found {bam_idx.num_reads} BAM records, {num_pod5_reads} "
+        f"POD5 reads, and {num_both_read_ids} in common"
+    )
+    if num_reads is None:
+        num_reads = num_both_read_ids
+    else:
+        num_reads = min(num_reads, num_both_read_ids)
+    return both_read_ids, num_reads
+
+
 class Motif:
     def __init__(self, raw_motif, focus_pos=0):
         self.raw_motif = raw_motif
         try:
             self.focus_pos = int(focus_pos)
         except ValueError:
             raise RemoraError(
```

### Comparing `ont-remora-2.0.0/src/remora/validate.py` & `ont-remora-2.1.0/src/remora/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 import atexit
 from collections import defaultdict, namedtuple
 
 import torch
 import pysam
 import numpy as np
@@ -22,14 +23,15 @@
         "loss",
         "acc",
         "num_calls",
         "conf_mat",
         "filt_frac",
         "filt_acc",
         "filt_conf_mat",
+        "filt_thresh",
     ),
 )
 
 
 def mat_to_str(mat):
     return json.dumps(mat.tolist(), separators=(",", ":"))
 
@@ -46,26 +48,25 @@
     acc = correctly_labeled.sum() / labels.size
 
     # extract probability of predicted class for each observation
     # numpy advanced indexing is weird but this is the right way to do this
     pred_probs = np.take_along_axis(
         probs, np.expand_dims(pred_labels, -1), -1
     ).squeeze(-1)
-    conf_thr = np.quantile(pred_probs, filt_frac)
+    filt_thr = np.quantile(pred_probs, filt_frac)
     # if all values would be filtered make filter threshold slightly smaller
-    if conf_thr == pred_probs.max():
-        conf_thr *= 0.999999
-    LOGGER.debug(f"Confidence threshold: {conf_thr}")
-    conf_chunks = pred_probs > conf_thr
+    if filt_thr == pred_probs.max():
+        filt_thr *= 0.999999
+    conf_chunks = pred_probs > filt_thr
     filt_labels = labels[conf_chunks]
     filt_acc = correctly_labeled[conf_chunks].sum() / filt_labels.size
     filt_conf_mat = confusion_matrix(filt_labels, pred_labels[conf_chunks])
     filt_frac = 1 - (filt_labels.size / labels.size)
 
-    return acc, conf_mat, filt_frac, filt_acc, filt_conf_mat
+    return acc, conf_mat, filt_frac, filt_acc, filt_conf_mat, filt_thr
 
 
 def add_unmodeled_labels(output, unmodeled_labels):
     """Add unmodeled labels into the neural network output for validation.
 
     Args:
         output (np.array): Output from a Remora neural network.
@@ -99,16 +100,16 @@
 
 def _validate_model(
     model,
     model_mod_bases,
     criterion,
     dataset,
     filt_frac=constants.DEFAULT_FILT_FRAC,
-    display_progress_bar=True,
     full_results_fh=None,
+    disable_pbar=False,
 ):
     device = next(model.parameters()).device
     unmodeled_labels = np.array(
         [
             idx + 1
             for idx, mb in enumerate(dataset.mod_bases)
             if mb not in model_mod_bases
@@ -119,24 +120,27 @@
         model.eval()
         torch.set_grad_enabled(False)
 
     bb, ab = dataset.kmer_context_bases
     all_labels = []
     all_outputs = []
     all_loss = []
-    ds_iter = (
-        tqdm(dataset, smoothing=0, desc="Batches")
-        if display_progress_bar
-        else dataset
-    )
+
+    if os.environ.get("LOG_SAFE", False):
+        disable_pbar = True
     for (
         (sigs, seqs, seq_maps, seq_lens),
         labels,
         (read_ids, read_focus_bases),
-    ) in ds_iter:
+    ) in tqdm(
+        dataset,
+        smoothing=0,
+        desc="Batches",
+        disable=disable_pbar,
+    ):
         all_labels.append(labels)
         enc_kmers = encoded_kmers.compute_encoded_kmer_batch(
             bb, ab, seqs, seq_maps, seq_lens
         )
         if is_torch_model:
             sigs = torch.from_numpy(sigs).to(device)
             enc_kmers = torch.from_numpy(enc_kmers).to(device)
@@ -156,25 +160,31 @@
                 output, labels, read_ids, read_focus_bases
             )
     all_outputs = np.concatenate(all_outputs, axis=0)
     all_labels = np.concatenate(all_labels)
     if is_torch_model:
         torch.set_grad_enabled(True)
     all_probs = softmax_axis1(all_outputs)
-    acc, conf_mat, filt_frac, filt_acc, filt_conf_mat = compute_metrics(
-        all_probs, all_labels, filt_frac
-    )
+    (
+        acc,
+        conf_mat,
+        filt_frac,
+        filt_acc,
+        filt_conf_mat,
+        filt_thr,
+    ) = compute_metrics(all_probs, all_labels, filt_frac)
     return VAL_METRICS(
         loss=np.mean(all_loss),
         acc=acc,
         num_calls=all_labels.size,
         conf_mat=conf_mat,
         filt_frac=filt_frac,
         filt_acc=filt_acc,
         filt_conf_mat=filt_conf_mat,
+        filt_thresh=filt_thr,
     )
 
 
 def process_mods_probs(probs, labels, allow_unbalanced, pct_filt, name):
     if not allow_unbalanced:
         nlabs = labels.max() + 1
         # split probs
@@ -193,32 +203,38 @@
             if label_probs.shape[0] > min_size:
                 np.random.shuffle(label_probs)
             probs[lab_idx * min_size : (lab_idx + 1) * min_size] = label_probs[
                 :min_size
             ]
             labels[lab_idx * min_size : (lab_idx + 1) * min_size] = lab_idx
 
-    acc, conf_mat, filt_frac, filt_acc, filt_conf_mat = compute_metrics(
-        probs, labels, pct_filt / 100
-    )
+    (
+        acc,
+        conf_mat,
+        filt_frac,
+        filt_acc,
+        filt_conf_mat,
+        filt_thr,
+    ) = compute_metrics(probs, labels, pct_filt / 100)
     ms = VAL_METRICS(
         loss=np.NAN,
         acc=acc,
         num_calls=labels.size,
         conf_mat=conf_mat,
         filt_frac=filt_frac,
         filt_acc=filt_acc,
         filt_conf_mat=filt_conf_mat,
+        filt_thresh=filt_thr,
     )
     val_output = (
         f"\n{ValidationLogger.HEADER}\n"
         f"{name}\t0\t0\t"
         f"{ms.acc:.6f}\t{mat_to_str(ms.conf_mat)}\t"
         f"NAN\t{ms.num_calls}\t{ms.filt_frac:.4f}\t"
-        f"{ms.filt_acc:.6f}\t{mat_to_str(ms.filt_conf_mat)}\n"
+        f"{ms.filt_acc:.6f}\t{mat_to_str(ms.filt_conf_mat)}\t{ms.filt_thresh}\n"
     )
     LOGGER.info(val_output)
 
 
 class ResultsWriter:
     def __init__(self, out_fh):
         self.sep = "\t"
@@ -257,14 +273,15 @@
             "Accuracy",
             "Confusion_Matrix",
             "Loss",
             "Num_Calls",
             "Filtered_Fraction",
             "Filtered_Accuracy",
             "Filtered_Confusion_Matrix",
+            "Filtered_Threshold",
         )
     )
 
     def __init__(self, fp, full_results_fh=None):
         self.fp = fp
         self.fp.write(self.HEADER + "\n")
         if full_results_fh is None:
@@ -278,30 +295,31 @@
         model_mod_bases,
         criterion,
         dataset,
         filt_frac=constants.DEFAULT_FILT_FRAC,
         val_type="val",
         nepoch=0,
         niter=0,
-        display_progress_bar=False,
+        disable_pbar=False,
     ):
         ms = _validate_model(
             model,
             model_mod_bases,
             criterion,
             dataset,
             filt_frac,
-            display_progress_bar=display_progress_bar,
             full_results_fh=self.full_results_fh,
+            disable_pbar=disable_pbar,
         )
         self.fp.write(
             f"{val_type}\t{nepoch}\t{niter}\t"
             f"{ms.acc:.6f}\t{mat_to_str(ms.conf_mat)}\t"
             f"{ms.loss:.6f}\t{ms.num_calls}\t{ms.filt_frac:.4f}\t"
-            f"{ms.filt_acc:.6f}\t{mat_to_str(ms.filt_conf_mat)}\n"
+            f"{ms.filt_acc:.6f}\t{mat_to_str(ms.filt_conf_mat)}\t"
+            f"{ms.filt_thresh}\n"
         )
         return ms
 
 
 ##################
 # ModBAM Parsing #
 ##################
@@ -316,15 +334,19 @@
     nctx=5,
     max_sites=None,
 ):
     strand = "-" if read.is_reverse else "+"
     ctg_gt = gt_sites.get((read.reference_name, strand))
     ctg_gt_range = gt_ranges.get((read.reference_name, strand))
 
-    aligned_pairs = read.get_aligned_pairs(with_seq=True)
+    try:
+        aligned_pairs = read.get_aligned_pairs(with_seq=True)
+    except ValueError:
+        LOGGER.debug(f"Read missing MD tag {read.query_name}")
+        return [], []
     r_align = "".join([b.upper() if b else "-" for _, _, b in aligned_pairs])
     q_align = "".join(
         [
             read.query_sequence[q_pos] if q_pos else "-"
             for q_pos, _, _ in aligned_pairs
         ]
     )
@@ -418,15 +440,15 @@
         labels = [labels[idx] for idx in indices]
         probs = [probs[idx] for idx in indices]
     return probs, labels
 
 
 def check_mod_strand(read, bam_path, alphabet, do_warn_mod, do_warn_strand):
     if read.modified_bases is None:
-        LOGGER.debug(f"Not modified bases found in {read.query_name}")
+        LOGGER.debug(f"No modified bases found in {read.query_name}")
         return do_warn_mod, do_warn_strand, False
 
     valid_mods = False
     for _, mod_strand, mod_name in read.modified_bases.keys():
         if (mod_strand == 0 and read.is_reverse) or (
             mod_strand == 1 and not read.is_reverse
         ):
@@ -505,17 +527,16 @@
                 max_sites=max_sites,
             )
             probs.extend(read_probs)
             labels.extend(read_labels)
     pysam.set_verbosity(pysam_save)
     if len(probs) < 1:
         raise RemoraError(
-            f"No valid modification calls from {bam_path}. May need to revert "
-            "to original MM-tag style. Try `sed s/C+m?,/C+m,/g`and see "
-            "https://github.com/pysam-developers/pysam/issues/1123"
+            f"No valid modification calls from {bam_path}. Confirm that "
+            "contig names from reference FASTA and ground truth BED match."
         )
     LOGGER.debug(
         f"Parsed {len(probs)} modified base calls from file: {bam_path}"
     )
     return np.array(probs), np.array(labels)
 
 
@@ -569,15 +590,15 @@
             dict((cs, (min(poss), max(poss))) for cs, poss in gt_sites.items())
         )
         all_mods.update(samp_mods)
     if extra_bases is not None:
         all_mods.update(extra_bases)
     can_base = all_mods.intersection("ACGTU")
     if len(can_base) > 1:
-        raise RemoraError("More than one canonical base found: {can_base}")
+        raise RemoraError(f"More than one canonical base found: {can_base}")
     if len(can_base) == 0:
         raise RemoraError("No canonical bases found in ground truth.")
     mod_bases = all_mods.difference("ACGTU")
     alphabet = "".join(can_base) + "".join(sorted(mod_bases))
 
     LOGGER.info("Parsing modBAM files")
     all_probs, all_labels = [], []
```

