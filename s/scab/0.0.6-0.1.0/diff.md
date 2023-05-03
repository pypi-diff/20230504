# Comparing `tmp/scab-0.0.6.tar.gz` & `tmp/scab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scab-0.0.6.tar", last modified: Wed Aug 24 18:22:53 2022, max compression
+gzip compressed data, was "scab-0.1.0.tar", last modified: Wed May  3 23:52:59 2023, max compression
```

## Comparing `scab-0.0.6.tar` & `scab-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:53.494777 scab-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-24 18:22:40.000000 scab-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 18:22:40.000000 scab-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-24 18:22:53.494777 scab-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-08-24 18:22:40.000000 scab-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:53.490777 scab-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-24 18:22:40.000000 scab-0.0.6/docs/doc_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-08-24 18:22:40.000000 scab-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:53.490777 scab-0.0.6/scab/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-24 18:22:40.000000 scab-0.0.6/scab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29246 2022-08-24 18:22:40.000000 scab-0.0.6/scab/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:53.494777 scab-0.0.6/scab/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:40.000000 scab-0.0.6/scab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20989 2022-08-24 18:22:40.000000 scab-0.0.6/scab/models/lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)   117836 2022-08-24 18:22:40.000000 scab-0.0.6/scab/pl.py
--rw-r--r--   0 runner    (1001) docker     (121)    11297 2022-08-24 18:22:40.000000 scab-0.0.6/scab/pp.py
--rw-r--r--   0 runner    (1001) docker     (121)    34210 2022-08-24 18:22:40.000000 scab-0.0.6/scab/tl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-08-24 18:22:40.000000 scab-0.0.6/scab/ut.py
--rw-r--r--   0 runner    (1001) docker     (121)    20562 2022-08-24 18:22:40.000000 scab-0.0.6/scab/vdj.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-24 18:22:40.000000 scab-0.0.6/scab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 18:22:53.494777 scab-0.0.6/scab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-24 18:22:53.000000 scab-0.0.6/scab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-24 18:22:53.000000 scab-0.0.6/scab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 18:22:53.000000 scab-0.0.6/scab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-24 18:22:53.000000 scab-0.0.6/scab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-24 18:22:53.000000 scab-0.0.6/scab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-24 18:22:53.494777 scab-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-08-24 18:22:40.000000 scab-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.963057 scab-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 23:52:48.000000 scab-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 23:52:48.000000 scab-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 23:52:59.963057 scab-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 23:52:48.000000 scab-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 23:52:48.000000 scab-0.1.0/bin/batch_cellranger
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 23:52:48.000000 scab-0.1.0/bin/scabranger
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-03 23:52:48.000000 scab-0.1.0/docs/doc_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-03 23:52:48.000000 scab-0.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/scab/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 23:52:48.000000 scab-0.1.0/scab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/scab/cellranger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:48.000000 scab-0.1.0/scab/cellranger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-03 23:52:48.000000 scab-0.1.0/scab/cellranger/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    49603 2023-05-03 23:52:48.000000 scab-0.1.0/scab/cellranger/scabranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27350 2023-05-03 23:52:48.000000 scab-0.1.0/scab/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/scab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:48.000000 scab-0.1.0/scab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22566 2023-05-03 23:52:48.000000 scab-0.1.0/scab/models/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118547 2023-05-03 23:52:48.000000 scab-0.1.0/scab/pl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.963057 scab-0.1.0/scab/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/ridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-05-03 23:52:48.000000 scab-0.1.0/scab/plots/umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-03 23:52:48.000000 scab-0.1.0/scab/pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42079 2023-05-03 23:52:48.000000 scab-0.1.0/scab/tl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.963057 scab-0.1.0/scab/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:48.000000 scab-0.1.0/scab/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-03 23:52:48.000000 scab-0.1.0/scab/tools/batch_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-03 23:52:48.000000 scab-0.1.0/scab/tools/clonify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-03 23:52:48.000000 scab-0.1.0/scab/tools/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 23:52:48.000000 scab-0.1.0/scab/ut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-05-03 23:52:48.000000 scab-0.1.0/scab/vdj.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 23:52:48.000000 scab-0.1.0/scab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:52:59.959057 scab-0.1.0/scab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-03 23:52:59.000000 scab-0.1.0/scab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-03 23:52:59.000000 scab-0.1.0/scab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:52:59.000000 scab-0.1.0/scab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 23:52:59.000000 scab-0.1.0/scab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 23:52:59.000000 scab-0.1.0/scab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 23:52:59.963057 scab-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-03 23:52:48.000000 scab-0.1.0/setup.py
```

### Comparing `scab-0.0.6/LICENSE` & `scab-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scab-0.0.6/README.md` & `scab-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scab-0.0.6/scab/io.py` & `scab-0.1.0/scab/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,29 +25,32 @@
 
 import codecs
 from collections.abc import Iterable
 import pathlib
 import pickle
 import re
 import typing
-from typing import Any, Callable, Collection, Dict, Optional, Union
+from typing import Any, Callable, Collection, Dict, Literal, Optional, Union
 
 import numpy as np
 
 import scanpy as sc
 
 import anndata
 from anndata import AnnData
-from anndata.compat import Literal
+
+# from anndata.compat import Literal
 from anndata._core.merge import StrategiesLiteral
 
 import abstar
 from abutils.core.pair import Pair, assign_pairs
 from abutils.core.sequence import read_csv, read_fasta, read_json
 
+from .vdj import merge_bcr, merge_tcr
+
 
 def read_10x_mtx(
     mtx_path: str,
     *,
     bcr_file: Optional[str] = None,
     bcr_annot: Optional[str] = None,
     bcr_format: Literal["fasta", "delimited", "json"] = "fasta",
@@ -68,15 +71,15 @@
     abstar_output_format: Literal["airr", "json"] = "airr",
     abstar_germ_db: str = "human",
     gex_only: bool = False,
     hashes: Optional[Iterable] = None,
     cellhash_regex: str = "cell ?hash",
     ignore_cellhash_case: bool = True,
     agbcs: Optional[Iterable] = None,
-    agbc_regex: str= "agbc",
+    agbc_regex: str = "agbc",
     ignore_agbc_case: bool = True,
     log_transform_cellhashes: bool = True,
     ignore_zero_quantile_cellhashes: bool = True,
     rename_cellhashes: Optional[Dict[str, str]] = None,
     log_transform_agbcs: bool = True,
     ignore_zero_quantile_agbcs: bool = True,
     rename_agbcs: Optional[Dict[str, str]] = None,
@@ -85,278 +88,229 @@
     rename_features: Optional[Dict[str, str]] = None,
     feature_suffix: str = "_FBC",
     cellhash_quantile: Union[float, int] = 0.95,
     agbc_quantile: Union[float, int] = 0.95,
     feature_quantile: Union[float, int] = 0.95,
     cache: bool = True,
     verbose: bool = True,
-):
-
+) -> AnnData:
     """
-    Reads and integrates output files from 10x Genomics' CellRanger into a single ``AnnData`` object.  
+    Reads and integrates output files from 10x Genomics' CellRanger into a single ``AnnData`` object.
 
     Datasets can include gene expression (GEX), cell hashes, antigen barcodes (AgBCs), feature
     barcodes, and assembled BCR or TCR contig sequences.
 
-    Parameters  
-    ----------  
-    mtx_path : str  
-        Path to a CellRanger counts matrix folder, typically either ``'sample_feature_bc_matrix'`` 
-        or ``'raw_feature_bc_matrix'``.  
+    Parameters
+    ----------
+    mtx_path : str
+        Path to a CellRanger counts matrix folder, typically either ``'sample_feature_bc_matrix'``
+        or ``'raw_feature_bc_matrix'``.
 
-    [bcr|tcr]_file : str, optional  
-        Path to a file containing BCR/TCR data. The file can be in one of several formats:  
+    [bcr|tcr]_file : str, optional
+        Path to a file containing BCR/TCR data. The file can be in one of several formats:
 
-                - FASTA-formatted file, as output by CellRanger  
+                - FASTA-formatted file, as output by CellRanger
 
-                - delimited text file, containing annotated BCR/TCR sequences  
+                - delimited text file, containing annotated BCR/TCR sequences
 
-                - JSON-formatted file, containing annotated BCR/TCR sequences  
+                - JSON-formatted file, containing annotated BCR/TCR sequences
 
-    [bcr|tcr]_annot : str, optional  
-        Path to the CSV-formatted BCR/TCR annotations file produced by CellRanger. Matching the 
-        annotation file to `[bcr|tcr]_file` is preferred -- if ``'all_contig.fasta'`` is the supplied 
-        `[bcr|tcr]_file`, then ``'all_contig_annotations.csv'`` is the appropriate annotation file.  
+    [bcr|tcr]_annot : str, optional
+        Path to the CSV-formatted BCR/TCR annotations file produced by CellRanger. Matching the
+        annotation file to `[bcr|tcr]_file` is preferred -- if ``'all_contig.fasta'`` is the supplied
+        `[bcr|tcr]_file`, then ``'all_contig_annotations.csv'`` is the appropriate annotation file.
 
-    [bcr|tcr]_format : str, default='fasta'  
-        Format of the input `[bcr|tcr]_file`. Options are: ``'fasta'``, ``'delimited'``, and 
-        ``'json'``. If `[bcr|tcr]_format` is ``'fasta'``, `abstar`_ 
-        will be run on the input data to obtain annotated BCR/TCR data. By default, abstar will 
-        produce `AIRR-formatted`_  (tab-delimited) annotations.  
+    [bcr|tcr]_format : str, default='fasta'
+        Format of the input `[bcr|tcr]_file`. Options are: ``'fasta'``, ``'delimited'``, and
+        ``'json'``. If `[bcr|tcr]_format` is ``'fasta'``, `abstar`_
+        will be run on the input data to obtain annotated BCR/TCR data. By default, abstar will
+        produce `AIRR-formatted`_  (tab-delimited) annotations.
 
-    [bcr|tcr]_delimiter : str, default='\t'  
+    [bcr|tcr]_delimiter : str, default='\t'
         Delimiter used in `[bcr|tcr]_file`. Only used if `[bcr|tcr]_format` is ``'delimited'``.
-        Default is ``'\t'``, which conforms to AIRR-C data standards.  
+        Default is ``'\t'``, which conforms to AIRR-C data standards.
 
-    [bcr|tcr]_id_key : str, default='sequence_id'  
-        Name of the column or field in `[bcr|tcr]_file` that corresponds to the sequence ID.   
+    [bcr|tcr]_id_key : str, default='sequence_id'
+        Name of the column or field in `[bcr|tcr]_file` that corresponds to the sequence ID.
 
-    [bcr|tcr]_sequence_key : str, default='sequence'  
-        Name of the column or field in `[bcr|tcr]_file` that corresponds to the VDJ sequence.  
+    [bcr|tcr]_sequence_key : str, default='sequence'
+        Name of the column or field in `[bcr|tcr]_file` that corresponds to the VDJ sequence.
 
-    [bcr|tcr]_id_delimiter : str, default='_'  
+    [bcr|tcr]_id_delimiter : str, default='_'
         The delimiter used to separate the droplet and contig components of the sequence ID.
-        For example, default CellRanger names are formatted as: ``'AAACCTGAGAACTGTA-1_contig_1'``, where 
-        ``'AAACCTGAGAACTGTA-1'`` is the droplet identifier and ``'contig_1'`` is the contig identifier.  
+        For example, default CellRanger names are formatted as: ``'AAACCTGAGAACTGTA-1_contig_1'``, where
+        ``'AAACCTGAGAACTGTA-1'`` is the droplet identifier and ``'contig_1'`` is the contig identifier.
 
-    [bcr|tcr]_id_delimiter_num : str, default=1  
-        The occurance (1-based numbering) of the `[bcr|tcr]_id_delimiter`.  
+    [bcr|tcr]_id_delimiter_num : str, default=1
+        The occurance (1-based numbering) of the `[bcr|tcr]_id_delimiter`.
 
-    abstar_output_format : str, default='airr'  
-        Format for abstar annotations. Only used if `[bcr|tcr]_format` is ``'fasta'``. 
-        Options are ``'airr'``, ``'json'`` and ``'tabular'``.  
-
-    abstar_germ_db : str, default='human'  
-        Germline database to be used for annotation of BCR/TCR data. Built-in abstar options 
-        include: ``'human'``, ``'macaque'``, ``'mouse'`` and ``'humouse'``. Only used if 
+    abstar_output_format : str, default='airr'
+        Format for abstar annotations. Only used if `[bcr|tcr]_format` is ``'fasta'``.
+        Options are ``'airr'``, ``'json'`` and ``'tabular'``.
+
+    abstar_germ_db : str, default='human'
+        Germline database to be used for annotation of BCR/TCR data. Built-in abstar options
+        include: ``'human'``, ``'macaque'``, ``'mouse'`` and ``'humouse'``. Only used if
         one or both of `[bcr|tcr]_format` is ``'fasta'``.
 
-    gex_only : bool, default=False  
+    gex_only : bool, default=False
         If ``True``, return only gene expression data and ignore features and hashes. Note that
-        VDJ data will still be included in the returned ``AnnData`` object if `[bcr|tcr]_file` 
-        is provided.  
+        VDJ data will still be included in the returned ``AnnData`` object if `[bcr|tcr]_file`
+        is provided.
 
-    cellhash_regex : str, default='cell ?hash'  
-        A regular expression (regex) string used to identify cell hashes. The regex 
+    cellhash_regex : str, default='cell ?hash'
+        A regular expression (regex) string used to identify cell hashes. The regex
         must be found in all hash names. The default, combined with the
         default setting for `ignore_hash_regex_case`, will match ``'cellhash'`` or ``'cell hash'``
-        in any combination of upper and lower case letters.  
+        in any combination of upper and lower case letters.
 
-    ignore_cellhash_regex_case : bool, default=True  
-        If ``True``, searching for `hash_regex` will ignore case.  
+    ignore_cellhash_regex_case : bool, default=True
+        If ``True``, searching for `hash_regex` will ignore case.
 
-    agbc_regex : str, default='agbc'  
-        A regular expression (regex) string used to identify AgBCs. The regex 
+    agbc_regex : str, default='agbc'
+        A regular expression (regex) string used to identify AgBCs. The regex
         must be found in all AgBC names. The default, combined with the
         default setting for `ignore_hash_regex_case`, will match ``'agbc'``
-        in any combination of upper and lower case letters.  
+        in any combination of upper and lower case letters.
 
-    ignore_agbc_regex_case : bool, default=True  
-        If ``True``, searching for `agbc_regex` will ignore case.  
+    ignore_agbc_regex_case : bool, default=True
+        If ``True``, searching for `agbc_regex` will ignore case.
 
-    log_transform_cellhashes : bool, default=True  
-        If ``True``, cell hash UMI counts will be log2-plus-1 transformed.  
+    log_transform_cellhashes : bool, default=True
+        If ``True``, cell hash UMI counts will be log2-plus-1 transformed.
 
-    log_transform_agbcs : bool, default=True  
-        If ``True``, AgBC UMI counts will be log2-plus-1 transformed.  
-        
-    log_transform_features : bool, default=True  
-        If ``True``, feature UMI counts will be log2-plus-1 transformed.  
+    log_transform_agbcs : bool, default=True
+        If ``True``, AgBC UMI counts will be log2-plus-1 transformed.
 
-    ignore_zero_quantile_cellhashes : bool, default=True  
+    log_transform_features : bool, default=True
+        If ``True``, feature UMI counts will be log2-plus-1 transformed.
+
+    ignore_zero_quantile_cellhashes : bool, default=True
         If ``True``, any hashes for which the `cellhash_quantile`
-        percentile have a count of zero are ignored. Default is ``True`` and the default 
+        percentile have a count of zero are ignored. Default is ``True`` and the default
         `cellhash_quantile` is ``0.95``, resulting in cellhashes with zero counts for the 95th
-        percentile being ignored.  
-        
-    ignore_zero_quantile_agbcs : bool, default=True  
+        percentile being ignored.
+
+    ignore_zero_quantile_agbcs : bool, default=True
         If ``True``, any AgBCs for which the `agbc_quantile`
-        percentile have a count of zero are ignored. Default is ``True`` and the default 
+        percentile have a count of zero are ignored. Default is ``True`` and the default
         `agbc_quantile` is ``0.95``, resulting in AgBCs with zero counts for the 95th
-        percentile being ignored.  
+        percentile being ignored.
 
-    ignore_zero_quantile_features : bool, default=True  
+    ignore_zero_quantile_features : bool, default=True
         If ``True``, any features for which the `feature_quantile`
-        percentile have a count of zero are ignored. Default is ``True`` and the default 
+        percentile have a count of zero are ignored. Default is ``True`` and the default
         `feature_quantile` is ``0.95``, resulting in features with zero counts for the 95th
-        percentile being ignored.  
+        percentile being ignored.
 
-    rename_cellhashes : dict, optional  
-        A dictionary with keys and values corresponding to the existing and 
-        new cellhash names, respectively. For example, ``{'CellHash1': 'donor123}`` would result in the 
-        renaming of ``'CellHash1'`` to ``'donor123'``. Cellhashes not found in the `rename_cellhashes` 
-        dictionary will not be renamed.  
-
-    rename_agbcs : dict, optional  
-        A dictionary with keys and values corresponding to the existing and 
-        new AgBC names, respectively. For example, ``{'AgBC1': 'Influenza H1'}`` would result in the 
-        renaming of ``'AgBC1'`` to ``'Influenza H1'``. AgBCs not found in the `rename_agbcs` 
-        dictionary will not be renamed.  
-
-    rename_features : dict, optional  
-        A dictionary with keys and values corresponding to the existing and 
-        new feature names, respectively. For example, ``{'FeatureBC1': 'CD19}`` would result in the 
-        renaming of ``'FeatureBC1'`` to ``'CD19'``. Features not found in the `rename_features` 
-        dictionary will not be renamed.  
-
-    feature_suffix : str, default='_FBC'  
-        Suffix to add to the end of each feature name. Useful because feature 
-        names may overlap with gene names. The default value will result in the feature 
-        ``'CD19'`` being renamed to ``'CD19_FBC'``. The suffix is added after feature renaming. 
-        To skip the addition of a feature suffix, simply supply an empty string (``''``) as the argument.  
+    rename_cellhashes : dict, optional
+        A dictionary with keys and values corresponding to the existing and
+        new cellhash names, respectively. For example, ``{'CellHash1': 'donor123}`` would result in the
+        renaming of ``'CellHash1'`` to ``'donor123'``. Cellhashes not found in the `rename_cellhashes`
+        dictionary will not be renamed.
+
+    rename_agbcs : dict, optional
+        A dictionary with keys and values corresponding to the existing and
+        new AgBC names, respectively. For example, ``{'AgBC1': 'Influenza H1'}`` would result in the
+        renaming of ``'AgBC1'`` to ``'Influenza H1'``. AgBCs not found in the `rename_agbcs`
+        dictionary will not be renamed.
+
+    rename_features : dict, optional
+        A dictionary with keys and values corresponding to the existing and
+        new feature names, respectively. For example, ``{'FeatureBC1': 'CD19}`` would result in the
+        renaming of ``'FeatureBC1'`` to ``'CD19'``. Features not found in the `rename_features`
+        dictionary will not be renamed.
+
+    feature_suffix : str, default='_FBC'
+        Suffix to add to the end of each feature name. Useful because feature
+        names may overlap with gene names. The default value will result in the feature
+        ``'CD19'`` being renamed to ``'CD19_FBC'``. The suffix is added after feature renaming.
+        To skip the addition of a feature suffix, simply supply an empty string (``''``) as the argument.
 
-    cellhash_quantile : float, default=0.95  
+    cellhash_quantile : float, default=0.95
         Percentile for which cellhashes with zero counts will be ignored if
         `ignore_zero_quantile_cellhashes` is ``True``. Default is ``0.95``, which is equivalent to the
-        95th percentile.  
+        95th percentile.
 
-    agbc_quantile : float, default=0.95  
+    agbc_quantile : float, default=0.95
         Percentile for which AgBCs with zero counts will be ignored if
         `ignore_zero_quantile_agbcs` is ``True``. Default is ``0.95``, which is equivalent to the
-        95th percentile.  
+        95th percentile.
 
-    feature_quantile : float, default=0.95  
+    feature_quantile : float, default=0.95
         Percentile for which features with zero counts will be ignored if
         `ignore_zero_quantile_features` is ``True``. Default is ``0.95``, which is equivalent to the
-        95th percentile.  
+        95th percentile.
+
+    verbose : bool, default=True
+        Print progress updates.
 
-    verbose : bool, default=True  
-        Print progress updates.  
-    
 
     Returns
     -------
     adata : ``anndata.AnnData``
         An ``AnnData`` object containing gene expression data, with VDJ information located
-        at ``adata.obs.bcr`` and/or ``adata.obs.tcr``, and cellhash and feature barcode data 
-        found in ``adata.obs``. If ``gex_only`` is ``True``, cellhash and feature barcode data 
-        are not returned.  
+        at ``adata.obs.bcr`` and/or ``adata.obs.tcr``, and cellhash and feature barcode data
+        found in ``adata.obs``. If ``gex_only`` is ``True``, cellhash and feature barcode data
+        are not returned.
 
 
     .. _abstar:
         https://github.com/briney/abstar
 
     .. _AIRR-formatted:
         https://docs.airr-community.org/en/stable/datarep/rearrangements.html
     """
     # read 10x matrix file
     if verbose:
         print("reading 10x Genomics matrix file...")
     adata = sc.read_10x_mtx(mtx_path, gex_only=False, cache=cache)
     gex = adata[:, adata.var.feature_types == "Gene Expression"]
 
-    # process BCR data:
+    # process BCR/TCR data
     if bcr_file is not None:
-        if bcr_format == "delimited":
-            delim_renames = {'\t': 'tab', ',': 'comma'}
-            if verbose:
-                d = delim_renames.get(bcr_delimiter, f"'{bcr_delimiter}'")
-                print(f"reading {d}-delimited BCR data...")
-            sequences = read_csv(
-                bcr_file,
-                delimiter=bcr_delimiter,
-                id_key=bcr_id_key,
-                sequence_key=bcr_sequence_key,
-            )
-        elif bcr_format == "json":
-            if verbose:
-                print("reading JSON-formatted BCR data...")
-            sequences = read_json(
-                bcr_file, id_key=bcr_id_key, sequence_key=bcr_sequence_key
-            )
-        elif bcr_format == "fasta":
-            if verbose:
-                print("reading FASTA-formatted BCR data...")
-            raw_seqs = read_fasta(bcr_file)
-            if verbose:
-                print("annotating BCR sequences with abstar...")
-            sequences = abstar.run(
-                raw_seqs, 
-                output_type=abstar_output_format, 
-                germ_db=abstar_germ_db, 
-                verbose=verbose,
-            )
-        pairs = assign_pairs(
-            sequences,
-            id_key=bcr_id_key,
-            delim=bcr_id_delimiter,
-            delim_occurance=bcr_id_delimiter_num,
+        gex = merge_bcr(
+            adata=gex,
+            bcr_file=bcr_file,
+            bcr_annot=bcr_annot,
+            bcr_format=bcr_format,
+            bcr_delimiter=bcr_delimiter,
+            bcr_id_key=bcr_id_key,
+            bcr_sequence_key=bcr_sequence_key,
+            bcr_id_delimiter=bcr_id_delimiter,
+            bcr_id_delimiter_num=bcr_id_delimiter_num,
             chain_selection_func=chain_selection_func,
-            tenx_annot_file=bcr_annot,
+            abstar_output_format=abstar_output_format,
+            abstar_germ_db=abstar_germ_db,
+            verbose=verbose,
         )
-        pdict = {p.name: p for p in pairs}
-        gex.obs["bcr"] = [pdict.get(o, Pair([])) for o in gex.obs_names]
-
-    # process TCR data:
     if tcr_file is not None:
-        if tcr_format == "delimited":
-            delim_renames = {'\t': 'tab', ',': 'comma'}
-            if verbose:
-                d = delim_renames.get(tcr_delimiter, f"'{tcr_delimiter}'")
-                print(f"reading {d}-delimited BCR data...")
-            sequences = read_csv(
-                tcr_file,
-                delimiter=tcr_delimiter,
-                id_key=tcr_id_key,
-                sequence_key=tcr_sequence_key,
-            )
-        elif tcr_format == "json":
-            if verbose:
-                print("reading JSON-formatted TCR data...")
-            sequences = read_json(
-                tcr_file, id_key=tcr_id_key, sequence_key=tcr_sequence_key
-            )
-        elif tcr_format == "fasta":
-            if verbose:
-                print("reading FASTA-formatted TCR data...")
-            raw_seqs = read_fasta(tcr_file)
-            if verbose:
-                print("annotating TCR sequences with abstar...")
-            sequences = abstar.run(
-                raw_seqs,
-                receptor="tcr",
-                output_type=abstar_output_format,
-                germ_db=abstar_germ_db,
-                verbose=verbose,
-            )
-        pairs = assign_pairs(
-            sequences,
-            id_key=tcr_id_key,
-            delim=tcr_id_delimiter,
-            delim_occurance=tcr_id_delimiter_num,
+        gex = merge_tcr(
+            adata=gex,
+            tcr_file=tcr_file,
+            tcr_annot=tcr_annot,
+            tcr_format=tcr_format,
+            tcr_delimiter=tcr_delimiter,
+            tcr_id_key=tcr_id_key,
+            tcr_sequence_key=tcr_sequence_key,
+            tcr_id_delimiter=tcr_id_delimiter,
+            tcr_id_delimiter_num=tcr_id_delimiter_num,
             chain_selection_func=chain_selection_func,
-            tenx_annot_file=tcr_annot,
+            abstar_output_format=abstar_output_format,
+            abstar_germ_db=abstar_germ_db,
+            verbose=verbose,
         )
-        pdict = {p.name: p for p in pairs}
-        gex.obs["tcr"] = [pdict.get(o, Pair([])) for o in gex.obs_names]
+
     if gex_only:
         return gex
+    non_gex = adata[:, adata.var.feature_types != "Gene Expression"]
+    if non_gex.shape[1] == 0:
+        return gex
 
     # parse out features and cellhashes
-    non_gex = adata[:, adata.var.feature_types != "Gene Expression"]
     if ignore_cellhash_case:
         cellhash_pattern = re.compile(cellhash_regex, flags=re.IGNORECASE)
     else:
         cellhash_pattern = re.compile(cellhash_regex)
     if ignore_agbc_case:
         agbc_pattern = re.compile(agbc_regex, flags=re.IGNORECASE)
     else:
@@ -440,24 +394,24 @@
     for f in feature_df:
         gex.obs[rename_features.get(f, f)] = feature_df[f]
     return gex
 
 
 def read(h5ad_file: Union[str, pathlib.Path]) -> AnnData:
     """
-    Reads a serialized ``AnnData`` object. Similar to ``scanpy.read()``, except that ``scanpy`` 
+    Reads a serialized ``AnnData`` object. Similar to ``scanpy.read()``, except that ``scanpy``
     does not support serialized BCR/TCR data. If BCR/TCR data is included in the serialized ``AnnData``
     file, it will be separately deserialized into the original ``abutils.Pair`` objects.
 
     Parameters
     ----------
-    h5ad_file : str  
+    h5ad_file : str
         Path to the output file. The output will be written in ``h5ad`` format and must
         include ``'.h5ad'`` as the file extension. If it is not included, the extension will automatically
-        be added. Required.   
+        be added. Required.
 
 
     Returns
     -------
     adata : ``anndata.AnnData``
 
     """
@@ -473,31 +427,31 @@
             pickle.loads(codecs.decode(t.encode(), "base64")) for t in adata.obs.tcr
         ]
     return adata
 
 
 def write(adata: AnnData, h5ad_file: Union[str, pathlib.Path]):
     """
-    Serialized and writes an ``AnnData`` object to disk in ``h5ad`` format. Similar to 
+    Serialized and writes an ``AnnData`` object to disk in ``h5ad`` format. Similar to
     ``scanpy.write()``, except that ``scanpy`` does not support serializing BCR/TCR data. This
-    function serializes ``abutils.Pair`` objects stored in either ``adata.obs.bcr`` or 
+    function serializes ``abutils.Pair`` objects stored in either ``adata.obs.bcr`` or
     ``adata.obs.tcr`` using ``pickle`` prior to writing the ``AnnData`` object to disk.
 
     Parameters
     ----------
 
     adata
-        An ``AnnData`` object containing gene expression, feature barcode and 
+        An ``AnnData`` object containing gene expression, feature barcode and
         VDJ data. ``scab.read_10x_mtx()`` can be used to construct a multi-omics ``AnnData`` object
         from raw CellRanger outputs.
 
-    h5ad_file 
+    h5ad_file
         Path to the output file. The output will be written in ``h5ad`` format and must
         include ``'.h5ad'`` as the file extension. If it is not included, the extension will automatically
-        be added.  
+        be added.
     """
     if not h5ad_file.endswith("h5ad"):
         h5ad_file += ".h5ad"
     _adata = adata.copy()
     if "bcr" in _adata.obs:
         # pickle BCR data
         _adata.obs["bcr"] = [
@@ -509,98 +463,102 @@
             codecs.encode(pickle.dumps(t), "base64").decode() for t in _adata.obs.tcr
         ]
     _adata.write(h5ad_file)
 
 
 def save(adata: AnnData, h5ad_file: Union[str, pathlib.Path]):
     """
-    Serialized and writes an ``AnnData`` object to disk in ``h5ad`` format. Similar to 
+    Serialized and writes an ``AnnData`` object to disk in ``h5ad`` format. Similar to
     ``scanpy.write()``, except that ``scanpy`` does not support serializing BCR/TCR data. This
-    function serializes ``abutils.Pair`` objects stored in either ``adata.obs.bcr`` or 
+    function serializes ``abutils.Pair`` objects stored in either ``adata.obs.bcr`` or
     ``adata.obs.tcr`` using ``pickle`` prior to writing the ``AnnData`` object to disk.
 
     Parameters
     ----------
 
     adata
-        An ``AnnData`` object containing gene expression, feature barcode and 
+        An ``AnnData`` object containing gene expression, feature barcode and
         VDJ data. ``scab.read_10x_mtx()`` can be used to construct a multi-omics ``AnnData`` object
         from raw CellRanger outputs.
 
     h5ad_file
         Path to the output file. The output will be written in ``h5ad`` format and must
         include ``'.h5ad'`` as the file extension. If it is not included, the extension will automatically
-        be added.   
+        be added.
     """
     write(adata, h5ad_file)
 
 
-
 def concat(
     adatas: Union[Collection[AnnData], "typing.Mapping[str, AnnData]"],
     *,
     axis: Literal[0, 1] = 0,
     join: Literal["inner", "outer"] = "inner",
     merge: Union[StrategiesLiteral, Callable, None] = None,
-    uns_merge: Union[StrategiesLiteral, Callable, None] = None,
+    uns_merge: Union[StrategiesLiteral, Callable, None] = "unique",
     label: Optional[str] = None,
     keys: Optional[Collection] = None,
     index_unique: Optional[str] = None,
     fill_value: Optional[Any] = None,
-    pairwise: bool = False, 
-    obs_names_make_unique: bool = True
+    pairwise: bool = False,
+    obs_names_make_unique: bool = True,
 ) -> AnnData:
-    '''Concatenates AnnData objects using ``anndata.concat()``. Documentation was copied almost verbatim from the ``anndata.concat()`` `docstring`_
+    """Concatenates AnnData objects using ``anndata.concat()``.
+    Documentation was copied almost verbatim from the ``anndata.concat()`` `docstring`_.
+
+    The only major difference is that the default for `uns_merge` has been changed from
+    ``None`` (which doesn't merge any of the data in ``adata.uns``) to ``'unique'``, which
+    only merges ``adata.uns`` elements for which there is only one possible value.
 
     Parameters
     ----------
 
     adatas
         The objects to be concatenated. If a Mapping is passed, keys are used for the `keys`
         argument and values are concatenated.
-    
+
     axis
         Which axis to concatenate along. ``0`` is row-wise, ``1`` is column-wise.
 
     join
         How to align values when concatenating. If ``"outer"``, the union of the other axis
-        is taken. If ``"inner"``, the intersection is taken. For example::  
-    
+        is taken. If ``"inner"``, the intersection is taken. For example::
+
     merge
         How elements not aligned to the axis being concatenated along are selected.
         Currently implemented strategies include:
         * ``None``: No elements are kept.
         * ``"same"``: Elements that are the same in each of the objects.
         * ``"unique"``: Elements for which there is only one possible value.
         * ``"first"``: The first element seen at each from each position.
         * ``"only"``: Elements that show up in only one of the objects.
-    
+
     uns_merge
         How the elements of ``.uns`` are selected. Uses the same set of strategies as
         the `merge` argument, except applied recursively.
-    
+
     label
         Column in axis annotation (i.e. ``.obs`` or ``.var``) to place batch information in.
         If it's None, no column is added.
-    
+
     keys
         Names for each object being added. These values are used for column values for
         `label` or appended to the index if `index_unique` is not ``None``. Defaults to
         incrementing integer labels.
-    
+
     index_unique
         Whether to make the index unique by using the keys. If provided, this
         is the delimeter between "{orig_idx}{index_unique}{key}". When ``None``,
         the original indices are kept.
-    
+
     fill_value
         When ``join="outer"``, this is the value that will be used to fill the introduced
         indices. By default, sparse arrays are padded with zeros, while dense arrays and
         DataFrames are padded with missing values.
-    
+
     pairwise
         Whether pairwise elements along the concatenated dimension should be included.
         This is False by default, since the resulting arrays are often not meaningful.
 
     obs_names_make_unique
         If ``True``, will call ``obs_names_make_unique()`` on the concatenated ``AnnData``
         object prior to returning. Default is ``True``.
@@ -635,30 +593,30 @@
     ... )
     >>> c = ad.AnnData(
     ...     X=sparse.csr_matrix(np.array([[10, 11], [12, 13]])),
     ...     obs=pd.DataFrame({"group": ["a", "b"]}, index=["s1", "s2"]),
     ...     var=pd.DataFrame(index=["var3", "var4"]),
     ...     uns={"a": 1, "b": 4, "c": {"c.a": 3, "c.b": 4, "c.c": 5}},
     ... )
-    
+
     Concatenating along different axes
-    
+
     >>> ad.concat([a, b]).to_df()
         var1  var2
     s1   0.0   1.0
     s2   2.0   3.0
     s3   4.0   5.0
     s4   7.0   8.0
     >>> ad.concat([a, c], axis=1).to_df()
         var1  var2  var3  var4
     s1   0.0   1.0  10.0  11.0
     s2   2.0   3.0  12.0  13.0
-    
+
     Inner and outer joins
-    
+
     >>> inner = ad.concat([a, b])  # Joining on intersection of variables
     >>> inner
     AnnData object with n_obs × n_vars = 4 × 2
         obs: 'group'
     >>> (inner.obs_names, inner.var_names)
     (Index(['s1', 's2', 's3', 's4'], dtype='object'),
     Index(['var1', 'var2'], dtype='object'))
@@ -670,17 +628,17 @@
     Index(['var1', 'var2', 'var3'], dtype='object')
     >>> outer.to_df()  # Sparse arrays are padded with zeroes by default
         var1  var2  var3
     s1   0.0   1.0   0.0
     s2   2.0   3.0   0.0
     s3   4.0   5.0   6.0
     s4   7.0   8.0   9.0
-    
+
     Keeping track of source objects
-    
+
     >>> ad.concat({"a": a, "b": b}, label="batch").obs
        group batch
     s1     a     a
     s2     b     a
     s3     b     b
     s4     c     b
     >>> ad.concat([a, b], label="batch", keys=["a", "b"]).obs  # Equivalent to previous
@@ -691,17 +649,17 @@
     s4     c     b
     >>> ad.concat({"a": a, "b": b}, index_unique="-").obs
          group
     s1-a     a
     s2-a     b
     s3-b     b
     s4-b     c
-    
+
     Combining values not aligned to axis of concatenation
-    
+
     >>> ad.concat([a, b], merge="same")
     AnnData object with n_obs × n_vars = 4 × 2
         obs: 'group'
         varm: 'ones'
     >>> ad.concat([a, b], merge="unique")
     AnnData object with n_obs × n_vars = 4 × 2
         obs: 'group'
@@ -710,30 +668,30 @@
     AnnData object with n_obs × n_vars = 4 × 2
         obs: 'group'
         varm: 'ones', 'rand', 'zeros'
     >>> ad.concat([a, b], merge="only")
     AnnData object with n_obs × n_vars = 4 × 2
         obs: 'group'
         varm: 'zeros'
-    
+
     The same merge strategies can be used for elements in `.uns`
-    
+
     >>> dict(ad.concat([a, b, c], uns_merge="same").uns)
     {'a': 1, 'c': {'c.b': 4}}
     >>> dict(ad.concat([a, b, c], uns_merge="unique").uns)
     {'a': 1, 'c': {'c.a': 3, 'c.b': 4, 'c.c': 5}}
     >>> dict(ad.concat([a, b, c], uns_merge="only").uns)
     {'c': {'c.c': 5}}
     >>> dict(ad.concat([a, b, c], uns_merge="first").uns)
     {'a': 1, 'b': 2, 'c': {'c.a': 3, 'c.b': 4, 'c.c': 5}}
 
 
     .. _docstring
         https://github.com/scverse/anndata/blob/master/anndata/_core/merge.py#L628
-    '''
+    """
     adata = anndata.concat(
         adatas,
         axis=axis,
         join=join,
         merge=merge,
         uns_merge=uns_merge,
         label=label,
@@ -742,10 +700,7 @@
         fill_value=fill_value,
         pairwise=pairwise,
     )
 
     if obs_names_make_unique:
         adata.obs_names_make_unique()
     return adata
-
-
-
```

### Comparing `scab-0.0.6/scab/models/lineage.py` & `scab-0.1.0/scab/models/lineage.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,31 +19,32 @@
 # BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 
+import copy
 from collections import Counter
+from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from natsort import natsorted
 
 import prettytable as pt
 
 from abstar.core.germline import get_imgt_germlines
 from abstar.utils.regions import (
     IMGT_REGION_START_POSITIONS_AA,
     IMGT_REGION_END_POSITIONS_AA,
 )
 
-from abutils import Sequence
-from abutils.utils.alignment import muscle
+import abutils
 
 
 class Lineage:
     """
     docstring for Lineage
     """
 
@@ -114,14 +115,60 @@
             dot_alignment=dot_alignment,
             in_color=in_color,
             pairs_only=pairs_only,
             padding_width=padding_width,
         )
 
 
+class LineageAssignment:
+    """
+    docstring for LineageAssignment
+    """
+
+    def __init__(
+        self, pair: abutils.Pair, assignment_dict: dict,
+    ):
+        self.pair = pair
+        self.assignment_dict = assignment_dict
+        self.all_lineages = list(assignment_dict.values())
+
+    def __eq__(self, lineage_name) -> bool:
+        return lineage_name in self.all_lineages
+
+    def get(self, lineage_name) -> Optional[abutils.Pair]:
+        """
+        Gets the ``Pair`` that was assigned to a lineage. Note that if
+        the original ``Pair`` object contained multiple heavy chains,
+        a modified ``Pair`` is returned containing all light chains from the
+        original ``Pair`` but only the heavy chain assigned to the lineage.
+
+        Parameters
+        ----------
+        lineage_name : str
+            Lineage name. Required
+
+        Returns
+        -------
+        abutils.Pair
+            A ``Pair`` that was assigned to the specified lineage. Note that if
+            the original ``Pair`` object contained multiple heavy chains,
+            a modified ``Pair`` is returned containing all light chains from the
+            original ``Pair`` but only the heavy chain assigned to the lineage.
+        """
+        if lineage_name not in self.all_lineages:
+            return None
+        lookup = {v: k for k, v in self.assignment_dict.items()}
+        identifier = lookup[lineage_name]
+        i = int(identifier.split("__")[-1])
+        p = copy.deepcopy(self.pair)
+        p.heavy = p.heavies[i]
+        p.heavies = [p.heavy]
+        return p
+
+
 class LineageSummary:
     """
     docstring for LineageSummary
     """
 
     def __init__(
         self,
@@ -424,17 +471,17 @@
         cdr1_end = IMGT_REGION_END_POSITIONS_AA["CDR1"]
         cdr2_start = IMGT_REGION_START_POSITIONS_AA["CDR2"] - 1
         cdr2_end = IMGT_REGION_END_POSITIONS_AA["CDR2"]
         # junction_start = IMGT_REGION_END_POSITIONS_AA['FR3'] - 1
         # junction_end = IMGT_REGION_START_POSITIONS_AA['FR4']
         # get data for germline line
         d = {"name": "germ", "order": 0}
-        dbname = Counter([s["germline_database"] for s in notnone_sequences]).most_common(1)[0][
-            0
-        ]
+        dbname = Counter(
+            [s["germline_database"] for s in notnone_sequences]
+        ).most_common(1)[0][0]
         v_gene = Counter([s["v_call"] for s in notnone_sequences]).most_common(1)[0][0]
         j_gene = Counter([s["j_call"] for s in notnone_sequences]).most_common(1)[0][0]
         v_germ = get_imgt_germlines(dbname, "V", gene=v_gene)
         # j_germ = get_imgt_germlines(dbname, 'J', gene=j_gene)
         junction_v = ref["junction_germ_v_aa"]
         junction_j = ref["junction_germ_j_aa"]
         junction_x = "X" * (len(ref["junction_aa"]) - len(junction_v) - len(junction_j))
@@ -452,21 +499,21 @@
                     d[region] = "X"
             aln_data.append(d)
         # make a dataframe
         df = pd.DataFrame(aln_data).sort_values(by="order")
         # do the alignments
         names = df["name"]
         for region in ["cdr1", "cdr2", "junction"]:
-            aln_seqs = [Sequence(s, id=n) for s, n in zip(df[region], names)]
-            aln = muscle(aln_seqs)
+            aln_seqs = [abutils.Sequence(s, id=n) for s, n in zip(df[region], names)]
+            aln = abutils.tl.muscle(aln_seqs)
             # aln_dict = {rec.id: str(rec.seq) for rec in aln}
             aln_dict = {}
             for rec in aln:
                 if not str(rec.seq).replace("-", "").replace("X", ""):
-                    aln_dict[rec.id] = " " + len(str(rec.seq))
+                    aln_dict[rec.id] = " " * len(str(rec.seq))
                 else:
                     aln_dict[rec.id] = str(rec.seq)
             df[f"{region}_aligned"] = [aln_dict[str(n)] for n in names]
         # make a dot alignment
         for region in ["cdr1", "cdr2"]:
             dot_alns = []
             dot_ref = df[f"{region}_aligned"][0]
```

### Comparing `scab-0.0.6/scab/pl.py` & `scab-0.1.0/scab/pl.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 # BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 
+from .plots.bar import bar
+from .plots.kde import kde
+from .plots.qc import qc_metrics
+from .plots.ridge import ridge
+from .plots.scatter import scatter
+from .plots.umap import umap
+
+
 from collections import Counter
 import itertools
 import os
 import re
 import sys
 
 import numpy as np
@@ -56,183 +64,181 @@
 # ===========================
 
 #      QUALITY CONTROL
 
 # ===========================
 
 
-def qc_metrics(
-    adata,
-    ngenes_cutoff=2500,
-    mito_cutoff=10,
-    ig_cutoff=100,
-    read_count_bounds=[0, 5000],
-    gene_count_bounds=[0, 500],
-    fig_dir=None,
-    fig_prefix=None,
-):
-    if "ig" not in adata.var:
-        pattern = re.compile("IG[HKL][VDJ][1-9].+|TR[ABDG][VDJ][1-9]")
-        adata.var["ig"] = [
-            False if re.match(pattern, a) is None else True for a in adata.var.index
-        ]
-    if "mt" not in adata.var:
-        adata.var["mt"] = adata.var_names.str.startswith("MT-")
-    sc.pp.calculate_qc_metrics(
-        adata, qc_vars=["ig", "mt"], percent_top=None, log1p=False, inplace=True
-    )
-
-    palette = {"include": "#202020", "exclude": "#C0C0C0"}
-    hue_order = ["include", "exclude"]
-
-    # plot Ig
-    ig_hue = [
-        "include" if i < ig_cutoff else "exclude" for i in adata.obs.pct_counts_ig
-    ]
-    ig_counter = Counter(ig_hue)
-    g = sns.JointGrid(data=adata.obs, x="total_counts", y="pct_counts_ig")
-    g.plot_joint(
-        sns.scatterplot,
-        s=10,
-        linewidth=0,
-        hue=ig_hue,
-        hue_order=hue_order,
-        palette=palette,
-    )
-    g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
-    g.ax_joint.set_xlabel("total counts", fontsize=16)
-    g.ax_joint.set_ylabel("immunoglobulin counts (%)", fontsize=16)
-    g.ax_joint.tick_params(axis="both", labelsize=13)
-    handles, labels = g.ax_joint.get_legend_handles_labels()
-    labels = [f"{l} ({ig_counter[l]})" for l in labels]
-    g.ax_joint.legend(
-        handles, labels, title="ig filter", title_fontsize=14, fontsize=13
-    )
-    if fig_dir is not None:
-        plt.tight_layout()
-        if fig_prefix is not None:
-            fig_name = f"{fig_prefix}_pct-counts-ig.pdf"
-        else:
-            fig_name = "pct_counts_ig.pdf"
-        plt.savefig(os.path.join(fig_dir, fig_name))
-    else:
-        plt.show()
+# def qc_metrics(
+#     adata,
+#     ngenes_cutoff=2500,
+#     mito_cutoff=10,
+#     ig_cutoff=100,
+#     read_count_bounds=[0, 5000],
+#     gene_count_bounds=[0, 500],
+#     fig_dir=None,
+#     fig_prefix=None,
+# ):
+#     if "ig" not in adata.var:
+#         pattern = re.compile("IG[HKL][VDJ][1-9].+|TR[ABDG][VDJ][1-9]")
+#         adata.var["ig"] = [
+#             False if re.match(pattern, a) is None else True for a in adata.var.index
+#         ]
+#     if "mt" not in adata.var:
+#         adata.var["mt"] = adata.var_names.str.startswith("MT-")
+#     sc.pp.calculate_qc_metrics(
+#         adata, qc_vars=["ig", "mt"], percent_top=None, log1p=False, inplace=True
+#     )
 
-    # plot mito
-    mito_hue = [
-        "include" if i < mito_cutoff else "exclude" for i in adata.obs.pct_counts_mt
-    ]
-    mito_counter = Counter(mito_hue)
-    g = sns.JointGrid(data=adata.obs, x="total_counts", y="pct_counts_mt")
-    g.plot_joint(
-        sns.scatterplot,
-        s=10,
-        linewidth=0,
-        hue=mito_hue,
-        hue_order=hue_order,
-        palette=palette,
-    )
-    g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
-    g.ax_joint.set_xlabel("total counts", fontsize=16)
-    g.ax_joint.set_ylabel("mitochondrial counts (%)", fontsize=16)
-    g.ax_joint.tick_params(axis="both", labelsize=13)
-    handles, labels = g.ax_joint.get_legend_handles_labels()
-    labels = [f"{l} ({mito_counter[l]})" for l in labels]
-    g.ax_joint.legend(
-        handles, labels, title="mito filter", title_fontsize=14, fontsize=13
-    )
-    if fig_dir is not None:
-        plt.tight_layout()
-        if fig_prefix is not None:
-            fig_name = f"{fig_prefix}_pct-counts-mt.pdf"
-        else:
-            fig_name = "pct_counts_mt.pdf"
-        plt.savefig(os.path.join(fig_dir, fig_name))
-    else:
-        plt.show()
+#     palette = {"include": "#202020", "exclude": "#C0C0C0"}
+#     hue_order = ["include", "exclude"]
 
-    # plot N genes by counts
-    ngenes_hue = [
-        "include" if i < ngenes_cutoff else "exclude"
-        for i in adata.obs.n_genes_by_counts
-    ]
-    ngenes_counter = Counter(ngenes_hue)
-    g = sns.JointGrid(data=adata.obs, x="total_counts", y="n_genes_by_counts")
-    g.plot_joint(
-        sns.scatterplot,
-        s=10,
-        linewidth=0,
-        hue=ngenes_hue,
-        hue_order=hue_order,
-        palette=palette,
-    )
-    g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
-    g.ax_joint.set_xlabel("total counts", fontsize=16)
-    g.ax_joint.set_ylabel("number of genes", fontsize=16)
-    g.ax_joint.tick_params(axis="both", labelsize=13)
-    handles, labels = g.ax_joint.get_legend_handles_labels()
-    labels = [f"{l} ({ngenes_counter[l]})" for l in labels]
-    g.ax_joint.legend(
-        handles, labels, title="genes filter", title_fontsize=14, fontsize=13
-    )
-    if fig_dir is not None:
-        plt.tight_layout()
-        if fig_prefix is not None:
-            fig_name = f"{fig_prefix}_n-genes-by-counts.pdf"
-        else:
-            fig_name = "n_genes_by_counts.pdf"
-        plt.savefig(os.path.join(fig_dir, fig_name))
-    else:
-        plt.show()
+#     # plot Ig
+#     ig_hue = [
+#         "include" if i < ig_cutoff else "exclude" for i in adata.obs.pct_counts_ig
+#     ]
+#     ig_counter = Counter(ig_hue)
+#     g = sns.JointGrid(data=adata.obs, x="total_counts", y="pct_counts_ig")
+#     g.plot_joint(
+#         sns.scatterplot,
+#         s=10,
+#         linewidth=0,
+#         hue=ig_hue,
+#         hue_order=hue_order,
+#         palette=palette,
+#     )
+#     g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
+#     g.ax_joint.set_xlabel("total counts", fontsize=16)
+#     g.ax_joint.set_ylabel("immunoglobulin counts (%)", fontsize=16)
+#     g.ax_joint.tick_params(axis="both", labelsize=13)
+#     handles, labels = g.ax_joint.get_legend_handles_labels()
+#     labels = [f"{l} ({ig_counter[l]})" for l in labels]
+#     g.ax_joint.legend(
+#         handles, labels, title="ig filter", title_fontsize=14, fontsize=13
+#     )
+#     if fig_dir is not None:
+#         plt.tight_layout()
+#         if fig_prefix is not None:
+#             fig_name = f"{fig_prefix}_pct-counts-ig.pdf"
+#         else:
+#             fig_name = "pct_counts_ig.pdf"
+#         plt.savefig(os.path.join(fig_dir, fig_name))
+#     else:
+#         plt.show()
 
+#     # plot mito
+#     mito_hue = [
+#         "include" if i < mito_cutoff else "exclude" for i in adata.obs.pct_counts_mt
+#     ]
+#     mito_counter = Counter(mito_hue)
+#     g = sns.JointGrid(data=adata.obs, x="total_counts", y="pct_counts_mt")
+#     g.plot_joint(
+#         sns.scatterplot,
+#         s=10,
+#         linewidth=0,
+#         hue=mito_hue,
+#         hue_order=hue_order,
+#         palette=palette,
+#     )
+#     g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
+#     g.ax_joint.set_xlabel("total counts", fontsize=16)
+#     g.ax_joint.set_ylabel("mitochondrial counts (%)", fontsize=16)
+#     g.ax_joint.tick_params(axis="both", labelsize=13)
+#     handles, labels = g.ax_joint.get_legend_handles_labels()
+#     labels = [f"{l} ({mito_counter[l]})" for l in labels]
+#     g.ax_joint.legend(
+#         handles, labels, title="mito filter", title_fontsize=14, fontsize=13
+#     )
+#     if fig_dir is not None:
+#         plt.tight_layout()
+#         if fig_prefix is not None:
+#             fig_name = f"{fig_prefix}_pct-counts-mt.pdf"
+#         else:
+#             fig_name = "pct_counts_mt.pdf"
+#         plt.savefig(os.path.join(fig_dir, fig_name))
+#     else:
+#         plt.show()
 
-    # histogram of read counts
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=[12, 4])
-    sns.histplot(data=adata.obs, x='total_counts', binwidth=500, ax=ax1)
-    sns.histplot(data=adata.obs, x='total_counts', binwidth=100, ax=ax2)
-    ax2.set_xlim(read_count_bounds)
-
-    for ax in [ax1, ax2]:
-        ax.set_xlabel('read count', fontsize=16)
-        ax.set_ylabel('# of cells', fontsize=16)
-        ax.tick_params(axis='both', labelsize=12)
-        for s in ['left', 'right', 'top']:
-            ax.spines[s].set_visible(False)
-    if fig_dir is not None:
-        plt.tight_layout()
-        if fig_prefix is not None:
-            fig_name = f"{fig_prefix}_read-counts.pdf"
-        else:
-            fig_name = "read-counts.pdf"
-        plt.savefig(os.path.join(fig_dir, fig_name))
-    else:
-        plt.show()
+#     # plot N genes by counts
+#     ngenes_hue = [
+#         "include" if i < ngenes_cutoff else "exclude"
+#         for i in adata.obs.n_genes_by_counts
+#     ]
+#     ngenes_counter = Counter(ngenes_hue)
+#     g = sns.JointGrid(data=adata.obs, x="total_counts", y="n_genes_by_counts")
+#     g.plot_joint(
+#         sns.scatterplot,
+#         s=10,
+#         linewidth=0,
+#         hue=ngenes_hue,
+#         hue_order=hue_order,
+#         palette=palette,
+#     )
+#     g.plot_marginals(sns.kdeplot, shade=True, color="#404040")
+#     g.ax_joint.set_xlabel("total counts", fontsize=16)
+#     g.ax_joint.set_ylabel("number of genes", fontsize=16)
+#     g.ax_joint.tick_params(axis="both", labelsize=13)
+#     handles, labels = g.ax_joint.get_legend_handles_labels()
+#     labels = [f"{l} ({ngenes_counter[l]})" for l in labels]
+#     g.ax_joint.legend(
+#         handles, labels, title="genes filter", title_fontsize=14, fontsize=13
+#     )
+#     if fig_dir is not None:
+#         plt.tight_layout()
+#         if fig_prefix is not None:
+#             fig_name = f"{fig_prefix}_n-genes-by-counts.pdf"
+#         else:
+#             fig_name = "n_genes_by_counts.pdf"
+#         plt.savefig(os.path.join(fig_dir, fig_name))
+#     else:
+#         plt.show()
 
+#     # histogram of read counts
+#     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=[12, 4])
+#     sns.histplot(data=adata.obs, x="total_counts", binwidth=500, ax=ax1)
+#     sns.histplot(data=adata.obs, x="total_counts", binwidth=100, ax=ax2)
+#     ax2.set_xlim(read_count_bounds)
+
+#     for ax in [ax1, ax2]:
+#         ax.set_xlabel("read count", fontsize=16)
+#         ax.set_ylabel("# of cells", fontsize=16)
+#         ax.tick_params(axis="both", labelsize=12)
+#         for s in ["left", "right", "top"]:
+#             ax.spines[s].set_visible(False)
+#     if fig_dir is not None:
+#         plt.tight_layout()
+#         if fig_prefix is not None:
+#             fig_name = f"{fig_prefix}_read-counts.pdf"
+#         else:
+#             fig_name = "read-counts.pdf"
+#         plt.savefig(os.path.join(fig_dir, fig_name))
+#     else:
+#         plt.show()
 
-    # histogram of gene counts
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=[12, 4])
-    sns.histplot(data=adata.obs, x='n_genes_by_counts', binwidth=100, ax=ax1)
-    sns.histplot(data=adata.obs, x='n_genes_by_counts', binwidth=10, ax=ax2)
-    ax2.set_xlim(gene_count_bounds)
-
-    for ax in [ax1, ax2]:
-        ax.set_xlabel('gene count', fontsize=16)
-        ax.set_ylabel('# of cells', fontsize=16)
-        ax.tick_params(axis='both', labelsize=12)
-        for s in ['left', 'right', 'top']:
-            ax.spines[s].set_visible(False)
-    if fig_dir is not None:
-        plt.tight_layout()
-        if fig_prefix is not None:
-            fig_name = f"{fig_prefix}_gene-counts.pdf"
-        else:
-            fig_name = "gene-counts.pdf"
-        plt.savefig(os.path.join(fig_dir, fig_name))
-    else:
-        plt.show()
+#     # histogram of gene counts
+#     fig, (ax1, ax2) = plt.subplots(1, 2, figsize=[12, 4])
+#     sns.histplot(data=adata.obs, x="n_genes_by_counts", binwidth=100, ax=ax1)
+#     sns.histplot(data=adata.obs, x="n_genes_by_counts", binwidth=10, ax=ax2)
+#     ax2.set_xlim(gene_count_bounds)
+
+#     for ax in [ax1, ax2]:
+#         ax.set_xlabel("gene count", fontsize=16)
+#         ax.set_ylabel("# of cells", fontsize=16)
+#         ax.tick_params(axis="both", labelsize=12)
+#         for s in ["left", "right", "top"]:
+#             ax.spines[s].set_visible(False)
+#     if fig_dir is not None:
+#         plt.tight_layout()
+#         if fig_prefix is not None:
+#             fig_name = f"{fig_prefix}_gene-counts.pdf"
+#         else:
+#             fig_name = "gene-counts.pdf"
+#         plt.savefig(os.path.join(fig_dir, fig_name))
+#     else:
+#         plt.show()
 
 
 # ===========================
 
 #         FEATURES
 
 # ===========================
@@ -270,116 +276,116 @@
     **kwargs,
 ):
     """
     Produces a 2-dimensional KDE plot of two features.
 
     Parameters
     ----------
-    data : anndata.AnnData or pandas.DataFrame  
+    data : anndata.AnnData or pandas.DataFrame
         An ``AnnData`` object or a ``DataFrame`` containing the input data. Required.
 
     x : str
         Name of the column in `data` containing the feature to be plotted on the x-axis. Required.
 
-    y : str  
+    y : str
         Name of the column in `data` containing the feature to be plotted on the y-axis. Required.
 
-    hue : str, optional  
-        Name of the column in `data` containing categories for hue values. ``hue```` categories 
-        will each be plotted as differently colored densities on the same plot. 
+    hue : str, optional
+        Name of the column in `data` containing categories for hue values. ``hue```` categories
+        will each be plotted as differently colored densities on the same plot.
 
-    hue_order : iterable object, optional  
+    hue_order : iterable object, optional
         Iterable of hue categories, in the order they should be plotted and listed
         in the legend. If `hue_order` contains only a subset of the categories
         present in ``data[hue]`` or ``data.obs[hue]``, only the categories supplied in `hue_order`
         will be plotted.
 
-    colors : iterable object, optional  
-        List of colors to be used for `hue` categories. If `colors` is shorter than the 
-        list of hue categories, colors will be reused. If not provided, the 
-        `default Seaborn color palette`_ will be used. 
+    colors : iterable object, optional
+        List of colors to be used for `hue` categories. If `colors` is shorter than the
+        list of hue categories, colors will be reused. If not provided, the
+        `default Seaborn color palette`_ will be used.
 
-    thresh : float, default=0.1  
+    thresh : float, default=0.1
         Threshold for the KDE, as a fraction of the overall dataset.
-        
-    show_scatter : bool, default=True  
+
+    show_scatter : bool, default=True
         Show a scatterplot beneath the transparent KDE plot.
 
-    scatter_size : int or float, default=5  
+    scatter_size : int or float, default=5
         Size of the scatter points.
 
-    scatter_alpha : float, default=0.2  
+    scatter_alpha : float, default=0.2
         Alpha of the scatter points.
 
-    fill : bool, default=True  
+    fill : bool, default=True
         Whether or not to fill the KDE KDE plot. If ``False``, only the KDE boundary lines
         will be plotted.
 
-    kde_fill_alpha : float, default=0.7  
-        Alpha for the filled KDE plot. Ignored if `fill` is ``False``.  
-        
-    kde_line_alpha : float, default=1.0  
+    kde_fill_alpha : float, default=0.7
+        Alpha for the filled KDE plot. Ignored if `fill` is ``False``.
+
+    kde_line_alpha : float, default=1.0
         Alpha for the KDE boundary lines.
 
-    highlight_index : iterable object, optional  
-        An iterable of index names (present in `data`) of points to be highlighted on 
+    highlight_index : iterable object, optional
+        An iterable of index names (present in `data`) of points to be highlighted on
         the KDE plot. If provided, `highlight_x` and `highlight_y` are ignored.
 
-    highlight_x : iterable object, optional  
+    highlight_x : iterable object, optional
         An iterable of x-values for highlighted points. Also requires `highlight_y`.
-        
-    highlight_y : iterable object, optional  
+
+    highlight_y : iterable object, optional
         An iterable of y-values for highlighted points. Also requires `highlight_x`.
-        
-    highlight_marker : str, default='x'  
-        Marker style to be used for highlight points. Accepts any `matplotlib marker`_. 
 
-    highlight_size : int, default=90  
+    highlight_marker : str, default='x'
+        Marker style to be used for highlight points. Accepts any `matplotlib marker`_.
+
+    highlight_size : int, default=90
         Size of the highlight marker.
 
     highlight_color : string or list of color values, default='k'
         Color of the highlight points.
 
-    highlight_name : str, optional  
+    highlight_name : str, optional
         Name of the highlights, to be used in the plot legend. If not supplied,
         highlight points will not be included in the legend.
-        
-    highlight_alpha : float, default=0.8  
+
+    highlight_alpha : float, default=0.8
         Alpha of the highlight points.
 
-    xlabel : str, optional  
+    xlabel : str, optional
         Label for the x-axis. By default, the value for `x` is used.
 
-    ylabel : str, optional  
+    ylabel : str, optional
         Label for the y-axis. By default, the value for `y` is used.
 
     equal_axes : bool, default=True
         If ```True```, the the limits of the x- and y-axis will be equal.
-        
-    legend_kwargs : dict, optional  
+
+    legend_kwargs : dict, optional
         Dictionary of legend keyword arguments, which will be passed to ``ax.legend()``.
 
-    return_ax : bool, default=False  
+    return_ax : bool, default=False
         If ``True``, return the plot's ``ax`` object. Will not show or save the plot.
 
-    figsize : list, default=[6, 6]  
+    figsize : list, default=[6, 6]
         A list containg the dimensions of the plot, in inches.
 
-    figfile : str, optional  
-        Path to which the figure will be saved. If not provided, the figure will be 
+    figfile : str, optional
+        Path to which the figure will be saved. If not provided, the figure will be
         shown but not saved to file.
 
-    kwargs  
+    kwargs
         All other keyword arguments are passed to ``seaborn.kdeplot()``.
 
-    
-    .. _default Seaborn color palette: 
-        https://seaborn.pydata.org/generated/seaborn.color_palette.html  
 
-    .. _matplotlib marker: 
+    .. _default Seaborn color palette:
+        https://seaborn.pydata.org/generated/seaborn.color_palette.html
+
+    .. _matplotlib marker:
         https://matplotlib.org/stable/api/markers_api.html
 
     """
 
     # input data
     if isinstance(data, AnnData):
         _data = {}
@@ -558,830 +564,850 @@
     elif figfile is not None:
         plt.tight_layout()
         plt.savefig(figfile)
     else:
         plt.show()
 
 
-def scatter(
-    adata,
-    x,
-    y, 
-    hue=None, 
-    marker="o",
-    hue_order=None, 
-    force_categorical_hue=False,
-    palette=None,
-    color=None,
-    cmap=None,
-    size=20,
-    alpha=0.6,
-    receptor='bcr',
-    chain='heavy', 
-    x_chain=None,
-    y_chain=None,
-    hue_chain=None,
-    highlight_index=None,
-    highlight_x=None,
-    highlight_y=None,
-    highlight_marker="x",
-    highlight_size=90,
-    highlight_color="k",
-    highlight_name=None,
-    highlight_alpha=0.9,  
-    plot_kwargs=None,
-    legend_kwargs=None,
-    hide_legend=False,
-    xlabel=None,
-    ylabel=None,
-    title=None,
-    title_fontsize=20,
-    title_fontweight='normal',
-    title_loc='center',
-    title_pad=None,
-    show_title=False,
-    xlabel_fontsize=16,
-    ylabel_fontsize=16,
-    xtick_labelsize=14,
-    ytick_labelsize=14,
-    xtick_labelrotation=0,
-    ytick_labelrotation=0,
-    cbar_width=0.35,
-    cbar_height=0.05,
-    cbar_loc="lower right",
-    cbar_orientation="horizontal",
-    cbar_bbox_to_anchor=None,
-    cbar_flip_ticks=False,
-    cbar_title=None,
-    cbar_title_fontsize=12,
-    hide_cbar=False,
-    equal_axes=True,
-    ax=None,
-    show=False,
-    figsize=None,
-    figfile=None):
-    '''
-    Produces a scatter plot.
+# def scatter(
+#     adata,
+#     x,
+#     y,
+#     hue=None,
+#     marker="o",
+#     hue_order=None,
+#     force_categorical_hue=False,
+#     palette=None,
+#     color=None,
+#     cmap=None,
+#     size=20,
+#     alpha=0.6,
+#     receptor="bcr",
+#     chain="heavy",
+#     x_chain=None,
+#     y_chain=None,
+#     hue_chain=None,
+#     highlight_index=None,
+#     highlight_x=None,
+#     highlight_y=None,
+#     highlight_marker="x",
+#     highlight_size=90,
+#     highlight_color="k",
+#     highlight_name=None,
+#     highlight_alpha=0.9,
+#     plot_kwargs=None,
+#     legend_kwargs=None,
+#     hide_legend=False,
+#     xlabel=None,
+#     ylabel=None,
+#     title=None,
+#     title_fontsize=20,
+#     title_fontweight="normal",
+#     title_loc="center",
+#     title_pad=None,
+#     show_title=False,
+#     xlabel_fontsize=16,
+#     ylabel_fontsize=16,
+#     xtick_labelsize=14,
+#     ytick_labelsize=14,
+#     xtick_labelrotation=0,
+#     ytick_labelrotation=0,
+#     cbar_width=0.35,
+#     cbar_height=0.05,
+#     cbar_loc="lower right",
+#     cbar_orientation="horizontal",
+#     cbar_bbox_to_anchor=None,
+#     cbar_flip_ticks=False,
+#     cbar_title=None,
+#     cbar_title_fontsize=12,
+#     hide_cbar=False,
+#     equal_axes=True,
+#     ax=None,
+#     show=False,
+#     figsize=None,
+#     figfile=None,
+# ):
+#     """
+#     Produces a scatter plot.
 
-    Parameters
-    ----------
+#     Parameters
+#     ----------
 
-    adata : pandas.DataFrame  
-        A ``anndata.AnnData`` object containing the input data.  
+#     adata : pandas.DataFrame
+#         A ``anndata.AnnData`` object containing the input data.
 
-    x : str
-        Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the 
-        x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
-        if data from different chains is being analyzed, using `x_chain`. BCR/TCR annotation 
-        fields must contain numerical data. Required.   
+#     x : str
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the
+#         x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
+#         if data from different chains is being analyzed, using `x_chain`. BCR/TCR annotation
+#         fields must contain numerical data. Required.
+
+#     y : str
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the
+#         y-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
+#         if data from different chains is being analyzed, using `y_chain`. BCR/TCR annotation
+#         fields must contain numerical data. Required.
+
+#     hue : str, optional
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field containing hue values.
+#         BCR/TCR annotations can be further specified using `receptor` and `chain` or, if data
+#         from different chains is being analyzed, using `hue_chain`. BCR/TCR annotation
+#         fields must contain numerical data.
+
+#     marker : str, dict or iterable object, optional
+#         Marker style for the scatter plot. Accepts any of the following:
+#           * a `matplotlib marker`_ string
+#           * a ``dict`` mapping `hue` categories to a `matplotlib marker`_ string
+#           * a ``list`` of `matplotlib marker`_ strings, which should be the same
+#               length as `x` and `y`.
+
+#     hue_order : iterable object, optional
+#         List of `hue` categories in the order they should be plotted. If `hue_order` contains a
+#         subset of all categories found in `hue`, only the supplied categories will be plotted.
+#         If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.
 
-    y : str
-        Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the 
-        y-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
-        if data from different chains is being analyzed, using `y_chain`. BCR/TCR annotation 
-        fields must contain numerical data. Required.  
-
-    hue : str, optional  
-        Name of a column in `adata.obs` or a BCR/TCR annotation field containing hue values. 
-        BCR/TCR annotations can be further specified using `receptor` and `chain` or, if data 
-        from different chains is being analyzed, using `hue_chain`. BCR/TCR annotation 
-        fields must contain numerical data.   
-        
-    marker : str, dict or iterable object, optional  
-        Marker style for the scatter plot. Accepts any of the following:
-          * a `matplotlib marker`_ string
-          * a ``dict`` mapping `hue` categories to a `matplotlib marker`_ string
-          * a ``list`` of `matplotlib marker`_ strings, which should be the same 
-              length as `x` and `y`. 
-        
-    hue_order : iterable object, optional  
-        List of `hue` categories in the order they should be plotted. If `hue_order` contains a 
-        subset of all categories found in `hue`, only the supplied categories will be plotted.  
-        If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.  
-        
-    force_categorical_hue : bool, default=False  
-        If ``True``, `hue` data will be treated as categorical, even if the data appear to 
-        be continuous. This results in `color` being used to color the points rather than `cmap`.   
-        
-    palette : dict, optional  
-        Dictionary mapping `hue`, `x` or `y` names to colors. If if keys in `palette` match 
-        more than one category, `hue` categories take priority. If `palette` is not provided, 
-        bars are colored using `color` (if `hue` is ``None``) or a palette is generated 
-        automatically using ``sns.hls_palette()``.  
-
-    color : str or iterable object, optional. 
-        Color for the plot markers. Can be any of the following:
-          * a ``list`` or ``tuple`` containing RGB or RGBA values
-          * a color string, either from `Matplotlib's set of named colors`_ or a hex color value
-          * the name of a column in `data` that contains color values
-          * a ``list`` of colors (either as strings or RGB tuples) to be used for `hue` categories. 
-            If `colors` is shorter than the list of hue categories, colors will be reused.  
-        
-        .. tip::
-            If a single RGB or RGBA ``list`` or ``tuple`` is provided and `hue` is also supplied, 
-            there may be unexpected results as ``scatter()`` will attempt to map each of the 
-            individual RGB(A) values to a hue category.   
-        
-        Only used if `hue` contains categorical data (`cmap` is used for continuous data). If not 
-        provided, the `default Seaborn color palette`_ will be used. 
-        
-    cmap : str or matplotlib.color.Colormap, default='flare'   
-        Colormap to be used for continuous `hue` data.  
-        
-    size : str or float or iterable object, default=20  
-        Size of the scatter points. Either a   
-
-    alpha : float, default=0.6  
-        Alpha of the scatter points.  
-
-    receptor : str, default='bcr'  
-        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.  
-
-    chain : str, default='heavy'  
-        If `x`, `y` and/or `hue` are BCR/TCR annotation fields, chain for which annotation will be 
-        retrieved. Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``, 
-        ``'beta'``, ``'delta'`` or ``'gamma'``.  
-
-    x_chain : str
-        `chain` to be used for the x-axis. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-
-    y_chain : str
-        `chain` to be used for the y-axis. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-
-    hue_chain : str
-        `chain` to be used for the hue. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-        
-    highlight_index : iterable object, optional  
-        An iterable of index names (present in `data.index`) of points to be highlighted on 
-        the plot. If provided, `highlight_x` and `highlight_y` are ignored.
+#     force_categorical_hue : bool, default=False
+#         If ``True``, `hue` data will be treated as categorical, even if the data appear to
+#         be continuous. This results in `color` being used to color the points rather than `cmap`.
+
+#     palette : dict, optional
+#         Dictionary mapping `hue`, `x` or `y` names to colors. If if keys in `palette` match
+#         more than one category, `hue` categories take priority. If `palette` is not provided,
+#         bars are colored using `color` (if `hue` is ``None``) or a palette is generated
+#         automatically using ``sns.hls_palette()``.
+
+#     color : str or iterable object, optional.
+#         Color for the plot markers. Can be any of the following:
+#           * a ``list`` or ``tuple`` containing RGB or RGBA values
+#           * a color string, either from `Matplotlib's set of named colors`_ or a hex color value
+#           * the name of a column in `data` that contains color values
+#           * a ``list`` of colors (either as strings or RGB tuples) to be used for `hue` categories.
+#             If `colors` is shorter than the list of hue categories, colors will be reused.
+
+#         .. tip::
+#             If a single RGB or RGBA ``list`` or ``tuple`` is provided and `hue` is also supplied,
+#             there may be unexpected results as ``scatter()`` will attempt to map each of the
+#             individual RGB(A) values to a hue category.
+
+#         Only used if `hue` contains categorical data (`cmap` is used for continuous data). If not
+#         provided, the `default Seaborn color palette`_ will be used.
+
+#     cmap : str or matplotlib.color.Colormap, default='flare'
+#         Colormap to be used for continuous `hue` data.
+
+#     size : str or float or iterable object, default=20
+#         Size of the scatter points. Either a
+
+#     alpha : float, default=0.6
+#         Alpha of the scatter points.
+
+#     receptor : str, default='bcr'
+#         Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+#     chain : str, default='heavy'
+#         If `x`, `y` and/or `hue` are BCR/TCR annotation fields, chain for which annotation will be
+#         retrieved. Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``,
+#         ``'beta'``, ``'delta'`` or ``'gamma'``.
+
+#     x_chain : str
+#         `chain` to be used for the x-axis. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     y_chain : str
+#         `chain` to be used for the y-axis. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     hue_chain : str
+#         `chain` to be used for the hue. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     highlight_index : iterable object, optional
+#         An iterable of index names (present in `data.index`) of points to be highlighted on
+#         the plot. If provided, `highlight_x` and `highlight_y` are ignored.
 
-    highlight_x : iterable object, optional  
-        An iterable of x-values for highlighted points. Also requires `highlight_y`.
-        
-    highlight_y : iterable object, optional  
-        An iterable of y-values for highlighted points. Also requires `highlight_x`.
-        
-    highlight_marker : str, default='x'  
-        Marker style to be used for highlight points. Accepts any `matplotlib marker`_. 
+#     highlight_x : iterable object, optional
+#         An iterable of x-values for highlighted points. Also requires `highlight_y`.
 
-    highlight_size : int, default=90  
-        Size of the highlight marker.
+#     highlight_y : iterable object, optional
+#         An iterable of y-values for highlighted points. Also requires `highlight_x`.
 
-    highlight_color : string or list of color values, default='k'
-        Color of the highlight points.
+#     highlight_marker : str, default='x'
+#         Marker style to be used for highlight points. Accepts any `matplotlib marker`_.
 
-    highlight_name : str, optional  
-        Name of the highlights, to be used in the plot legend. If not supplied,
-        highlight points will not be included in the legend.
-        
-    highlight_alpha : float, default=0.9  
-        Alpha of the highlight points. 
+#     highlight_size : int, default=90
+#         Size of the highlight marker.
 
-    plot_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``pyplot.scatter()``.
+#     highlight_color : string or list of color values, default='k'
+#         Color of the highlight points.
 
-    legend_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
+#     highlight_name : str, optional
+#         Name of the highlights, to be used in the plot legend. If not supplied,
+#         highlight points will not be included in the legend.
 
-    hide_legend : bool, default=False  
-        By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-        the legend will not be shown.  
-        
-    xlabel : str, optional  
-        Text for the X-axis label. 
-
-    ylabel : str, optional  
-        Text for the Y-axis label.  
-        
-    xlabel_fontsize : int or float, default=16  
-        Fontsize for the X-axis label text.
+#     highlight_alpha : float, default=0.9
+#         Alpha of the highlight points.
 
-    ylabel_fontsize : int or float, default=16  
-        Fontsize for the Y-axis label text.
+#     plot_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``pyplot.scatter()``.
 
-    xtick_labelsize : int or float, default=14  
-        Fontsize for the X-axis tick labels.  
+#     legend_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
 
-    ytick_labelsize : int or float, default=14  
-        Fontsize for the Y-axis tick labels.  
+#     hide_legend : bool, default=False
+#         By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+#         the legend will not be shown.
 
-    xtick_labelrotation : int or float, default=0  
-        Rotation of the X-axis tick labels.  
-    
-    ytick_labelrotation : int or float, default=0  
-        Rotation of the Y-axis tick labels. 
-
-    cbar_width : int, default=35  
-        Width of the colorbar. Only used for continuous `hue` types.  
-
-    cbar_height : int, default=5  
-        Height of the colorbar. Only used for continuous `hue` types.  
-
-    cbar_loc : str or iterable object, default='lower right'  
-        Location of the colorbar. Accepts `any valid inset_axes() location`_.
-
-    cbar_orientation : str, default='horizontal'  
-        Orientation of the colorbar. Options are ``'horizontal'`` and ``'vertical'``.
-
-    cbar_bbox_to_anchor : list or tuple, optional
-        bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide 
-        fine-grained positioning of the colorbar.
-
-    cbar_flip_ticks : bool, default=False  
-        Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation` 
-        is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.  
-
-    cbar_title : str, optional  
-        Colorbar title. If not provided, `hue` is used.  
-
-    cbar_title_fontsize : int or float, default=12  
-        Fontsize for the colorbar title.  
-        
-    hide_cbar : bool, default=False. 
-        If ``True``, the color bar will be hidden on plots with continuous `hue` values.  
-        
-    equal_axes : bool, default=True
-        If ```True```, the the limits of the x- and y-axis will be equal.
+#     xlabel : str, optional
+#         Text for the X-axis label.
 
-    show :bool, default=False  
-        If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
-        is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
+#     ylabel : str, optional
+#         Text for the Y-axis label.
 
-    figsize : iterable object, default=[6, 4]  
-        List containing the figure size (as ``[x-dimension, y-dimension]``) in inches. 
+#     xlabel_fontsize : int or float, default=16
+#         Fontsize for the X-axis label text.
 
-    figfile : str, optional  
-        Path at which to save the figure file. If not provided, the figure is not saved
-        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.  
-        
-        
-    .. _matplotlib marker: 
-        https://matplotlib.org/stable/api/markers_api.html  
-
-    .. _Matplotlib's set of named colors:
-        https://matplotlib.org/stable/gallery/color/named_colors.html
-        
-    .. _default Seaborn color palette: 
-        https://seaborn.pydata.org/generated/seaborn.color_palette.html  
-
-    .. _any valid inset_axes() location: 
-        https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.axes_grid1.inset_locator.inset_axes.html
-        
-    '''    
-
-    # get x, y and hue data
-    d = {}
-    d['x'] = get_adata_values(
-        adata,
-        x, 
-        receptor=receptor, 
-        chain=x_chain if x_chain is not None else chain)
-    d['y'] = get_adata_values(
-        adata,
-        y, 
-        receptor=receptor, 
-        chain=y_chain if y_chain is not None else chain)
-    if hue is not None:
-        d[hue] = get_adata_values(
-            adata,
-            hue, 
-            receptor=receptor, 
-            chain=hue_chain if hue_chain is not None else chain)
-    df = pd.DataFrame(d, index=adata.obs.index)
-
-    ax = abutils.pl.scatter(
-        data=df,
-        x='x',
-        y='y', 
-        hue=hue, 
-        marker=marker,
-        hue_order=hue_order, 
-        force_categorical_hue=force_categorical_hue,
-        palette=palette,
-        color=color,
-        cmap=cmap,
-        size=size,
-        alpha=alpha,
-        highlight_index=highlight_index,
-        highlight_x=highlight_x,
-        highlight_y=highlight_y,
-        highlight_marker=highlight_marker,
-        highlight_size=highlight_size,
-        highlight_color=highlight_color,
-        highlight_name=highlight_name,
-        highlight_alpha=highlight_alpha,  
-        plot_kwargs=plot_kwargs,
-        legend_kwargs=legend_kwargs,
-        hide_legend=hide_legend,
-        xlabel=xlabel if xlabel is not None else x,
-        ylabel=ylabel if ylabel is not None else y,
-        title=title,
-        title_fontsize=title_fontsize,
-        title_fontweight=title_fontweight,
-        title_loc=title_loc,
-        title_pad=title_pad,
-        show_title=show_title,
-        xlabel_fontsize=xlabel_fontsize,
-        ylabel_fontsize=ylabel_fontsize,
-        xtick_labelsize=xtick_labelsize,
-        ytick_labelsize=ytick_labelsize,
-        xtick_labelrotation=xtick_labelrotation,
-        ytick_labelrotation=ytick_labelrotation,
-        cbar_width=cbar_width,
-        cbar_height=cbar_height,
-        cbar_loc=cbar_loc,
-        cbar_orientation=cbar_orientation,
-        cbar_bbox_to_anchor=cbar_bbox_to_anchor,
-        cbar_flip_ticks=cbar_flip_ticks,
-        cbar_title=cbar_title,
-        cbar_title_fontsize=cbar_title_fontsize,
-        hide_cbar=hide_cbar,
-        equal_axes=equal_axes,
-        ax=ax,
-        show=False,
-        figsize=figsize,
-        figfile=None
-    )
+#     ylabel_fontsize : int or float, default=16
+#         Fontsize for the Y-axis label text.
 
-    # save, show or return the ax
-    if figfile is not None:
-        plt.tight_layout()
-        plt.savefig(figfile)
-    elif show:
-        plt.show()
-    else:
-        return ax
-    
+#     xtick_labelsize : int or float, default=14
+#         Fontsize for the X-axis tick labels.
 
+#     ytick_labelsize : int or float, default=14
+#         Fontsize for the Y-axis tick labels.
 
+#     xtick_labelrotation : int or float, default=0
+#         Rotation of the X-axis tick labels.
 
-def umap(
-    adata,
-    hue=None, 
-    marker="o",
-    hue_order=None, 
-    force_categorical_hue=False,
-    palette=None,
-    color=None,
-    cmap=None,
-    size=10,
-    alpha=0.6,
-    n_col=2,
-    receptor='bcr',
-    chain='heavy', 
-    hue_chain=None,
-    highlight_index=None,
-    highlight_x=None,
-    highlight_y=None,
-    highlight_marker="x",
-    highlight_size=90,
-    highlight_color="k",
-    highlight_name=None,
-    highlight_alpha=0.9,  
-    plot_kwargs=None,
-    legend_on_data=False,
-    legend_fontsize=12,
-    legend_fontweight='bold',
-    legend_fontoutline=None,
-    legend_marker_alpha=0.8,
-    legend_kwargs=None,
-    hide_legend=False,
-    xlabel='UMAP1',
-    ylabel='UMAP2',
-    title=None,
-    title_fontsize=20,
-    title_fontweight='normal',
-    title_loc='center',
-    title_pad=None,
-    show_title=False,
-    xlabel_fontsize=16,
-    ylabel_fontsize=16,
-    xtick_labelsize=14,
-    ytick_labelsize=14,
-    xtick_labelrotation=0,
-    ytick_labelrotation=0,
-    tiny_axis=True,
-    cbar_width=0.35,
-    cbar_height=0.05,
-    cbar_loc="lower right",
-    cbar_orientation="horizontal",
-    cbar_bbox_to_anchor=None,
-    cbar_flip_ticks=False,
-    cbar_title=None,
-    cbar_title_fontsize=12,
-    hide_cbar=False,
-    equal_axes=True,
-    ax=None,
-    show=False,
-    figsize=None,
-    figfile=None):
-    '''
-    Produces a scatter plot.
+#     ytick_labelrotation : int or float, default=0
+#         Rotation of the Y-axis tick labels.
 
-    Parameters
-    ----------
+#     cbar_width : int, default=35
+#         Width of the colorbar. Only used for continuous `hue` types.
 
-    adata : pandas.DataFrame  
-        A ``anndata.AnnData`` object containing the input data.  
+#     cbar_height : int, default=5
+#         Height of the colorbar. Only used for continuous `hue` types.
 
-    x : str
-        Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the 
-        x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
-        if data from different chains is being analyzed, using `x_chain`. BCR/TCR annotation 
-        fields must contain numerical data. Required.   
+#     cbar_loc : str or iterable object, default='lower right'
+#         Location of the colorbar. Accepts `any valid inset_axes() location`_.
 
-    y : str
-        Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the 
-        y-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
-        if data from different chains is being analyzed, using `y_chain`. BCR/TCR annotation 
-        fields must contain numerical data. Required.  
-
-    hue : str, optional  
-        Name of a column in `adata.obs` or a BCR/TCR annotation field containing hue values. 
-        BCR/TCR annotations can be further specified using `receptor` and `chain` or, if data 
-        from different chains is being analyzed, using `hue_chain`. BCR/TCR annotation 
-        fields must contain numerical data.   
-        
-    marker : str, dict or iterable object, optional  
-        Marker style for the scatter plot. Accepts any of the following:
-          * a `matplotlib marker`_ string
-          * a ``dict`` mapping `hue` categories to a `matplotlib marker`_ string
-          * a ``list`` of `matplotlib marker`_ strings, which should be the same 
-              length as `x` and `y`. 
-        
-    hue_order : iterable object, optional  
-        List of `hue` categories in the order they should be plotted. If `hue_order` contains a 
-        subset of all categories found in `hue`, only the supplied categories will be plotted.  
-        If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.  
-        
-    force_categorical_hue : bool, default=False  
-        If ``True``, `hue` data will be treated as categorical, even if the data appear to 
-        be continuous. This results in `color` being used to color the points rather than `cmap`.   
-        
-    palette : dict, optional  
-        Dictionary mapping `hue`, `x` or `y` names to colors. If if keys in `palette` match 
-        more than one category, `hue` categories take priority. If `palette` is not provided, 
-        bars are colored using `color` (if `hue` is ``None``) or a palette is generated 
-        automatically using ``sns.hls_palette()``.  
-
-    color : str or iterable object, optional. 
-        Color for the plot markers. Can be any of the following:
-          * a ``list`` or ``tuple`` containing RGB or RGBA values
-          * a color string, either from `Matplotlib's set of named colors`_ or a hex color value
-          * the name of a column in `data` that contains color values
-          * a ``list`` of colors (either as strings or RGB tuples) to be used for `hue` categories. 
-            If `colors` is shorter than the list of hue categories, colors will be reused.  
-        
-        .. tip::
-            If a single RGB or RGBA ``list`` or ``tuple`` is provided and `hue` is also supplied, 
-            there may be unexpected results as ``scatter()`` will attempt to map each of the 
-            individual RGB(A) values to a hue category.   
-        
-        Only used if `hue` contains categorical data (`cmap` is used for continuous data). If not 
-        provided, the `default Seaborn color palette`_ will be used. 
-        
-    cmap : str or matplotlib.color.Colormap, default='flare'   
-        Colormap to be used for continuous `hue` data.  
-        
-    size : str or float or iterable object, default=20  
-        Size of the scatter points. Either a   
-
-    alpha : float, default=0.6  
-        Alpha of the scatter points.  
-
-    receptor : str, default='bcr'  
-        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.  
-
-    chain : str, default='heavy'  
-        If `x`, `y` and/or `hue` are BCR/TCR annotation fields, chain for which annotation will be 
-        retrieved. Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``, 
-        ``'beta'``, ``'delta'`` or ``'gamma'``.  
-
-    x_chain : str
-        `chain` to be used for the x-axis. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-
-    y_chain : str
-        `chain` to be used for the y-axis. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-
-    hue_chain : str
-        `chain` to be used for the hue. If not supplied, `chain` will be used. Only necessary 
-        when visualizing data from different chains on the same plot.  
-        
-    highlight_index : iterable object, optional  
-        An iterable of index names (present in `data.index`) of points to be highlighted on 
-        the plot. If provided, `highlight_x` and `highlight_y` are ignored.
+#     cbar_orientation : str, default='horizontal'
+#         Orientation of the colorbar. Options are ``'horizontal'`` and ``'vertical'``.
 
-    highlight_x : iterable object, optional  
-        An iterable of x-values for highlighted points. Also requires `highlight_y`.
-        
-    highlight_y : iterable object, optional  
-        An iterable of y-values for highlighted points. Also requires `highlight_x`.
-        
-    highlight_marker : str, default='x'  
-        Marker style to be used for highlight points. Accepts any `matplotlib marker`_. 
+#     cbar_bbox_to_anchor : list or tuple, optional
+#         bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide
+#         fine-grained positioning of the colorbar.
 
-    highlight_size : int, default=90  
-        Size of the highlight marker.
+#     cbar_flip_ticks : bool, default=False
+#         Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation`
+#         is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.
 
-    highlight_color : string or list of color values, default='k'
-        Color of the highlight points.
+#     cbar_title : str, optional
+#         Colorbar title. If not provided, `hue` is used.
 
-    highlight_name : str, optional  
-        Name of the highlights, to be used in the plot legend. If not supplied,
-        highlight points will not be included in the legend.
-        
-    highlight_alpha : float, default=0.9  
-        Alpha of the highlight points. 
+#     cbar_title_fontsize : int or float, default=12
+#         Fontsize for the colorbar title.
 
-    plot_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``pyplot.scatter()``.
+#     hide_cbar : bool, default=False.
+#         If ``True``, the color bar will be hidden on plots with continuous `hue` values.
 
-    legend_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
+#     equal_axes : bool, default=True
+#         If ```True```, the the limits of the x- and y-axis will be equal.
 
-    hide_legend : bool, default=False  
-        By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-        the legend will not be shown.  
-        
-    xlabel : str, optional  
-        Text for the X-axis label. 
-
-    ylabel : str, optional  
-        Text for the Y-axis label.  
-        
-    xlabel_fontsize : int or float, default=16  
-        Fontsize for the X-axis label text.
+#     show :bool, default=False
+#         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
+#         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
 
-    ylabel_fontsize : int or float, default=16  
-        Fontsize for the Y-axis label text.
+#     figsize : iterable object, default=[6, 4]
+#         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
 
-    xtick_labelsize : int or float, default=14  
-        Fontsize for the X-axis tick labels.  
+#     figfile : str, optional
+#         Path at which to save the figure file. If not provided, the figure is not saved
+#         and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
 
-    ytick_labelsize : int or float, default=14  
-        Fontsize for the Y-axis tick labels.  
 
-    xtick_labelrotation : int or float, default=0  
-        Rotation of the X-axis tick labels.  
-    
-    ytick_labelrotation : int or float, default=0  
-        Rotation of the Y-axis tick labels. 
-
-    cbar_width : float, default=0.35  
-        Width of the colorbar. Only used for continuous `hue` types.  
-
-    cbar_height : float, default=0.05  
-        Height of the colorbar. Only used for continuous `hue` types.  
-
-    cbar_loc : str or iterable object, default='lower right'  
-        Location of the colorbar. Accepts `any valid inset_axes() location`_.
-
-    cbar_orientation : str, default='horizontal'  
-        Orientation of the colorbar. Options are ``'horizontal'`` and ``'vertical'``.
-
-    cbar_bbox_to_anchor : list or tuple, optional
-        bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide 
-        fine-grained positioning of the colorbar.
-
-    cbar_flip_ticks : bool, default=False  
-        Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation` 
-        is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.  
-
-    cbar_title : str, optional  
-        Colorbar title. If not provided, `hue` is used.  
-
-    cbar_title_fontsize : int or float, default=12  
-        Fontsize for the colorbar title.  
-        
-    hide_cbar : bool, default=False. 
-        If ``True``, the color bar will be hidden on plots with continuous `hue` values.  
-        
-    equal_axes : bool, default=True
-        If ```True```, the the limits of the x- and y-axis will be equal.
+#     .. _matplotlib marker:
+#         https://matplotlib.org/stable/api/markers_api.html
 
-    show :bool, default=False  
-        If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
-        is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
+#     .. _Matplotlib's set of named colors:
+#         https://matplotlib.org/stable/gallery/color/named_colors.html
 
-    figsize : iterable object, default=[6, 4]  
-        List containing the figure size (as ``[x-dimension, y-dimension]``) in inches. 
+#     .. _default Seaborn color palette:
+#         https://seaborn.pydata.org/generated/seaborn.color_palette.html
 
-    figfile : str, optional  
-        Path at which to save the figure file. If not provided, the figure is not saved
-        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.  
-        
-        
-    .. _matplotlib marker: 
-        https://matplotlib.org/stable/api/markers_api.html  
-
-    .. _Matplotlib's set of named colors:
-        https://matplotlib.org/stable/gallery/color/named_colors.html
-        
-    .. _default Seaborn color palette: 
-        https://seaborn.pydata.org/generated/seaborn.color_palette.html  
-
-    .. _any valid inset_axes() location: 
-        https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.axes_grid1.inset_locator.inset_axes.html
-        
-    '''    
-    # check that the UMAP data exists
-    if 'X_umap' not in adata.obsm:
-        from .tl import dimensionality_reduction
-        adata = dimensionality_reduction(adata)
-    
-    # parse hues (if provided)
-    if hue is not None:
-        if isinstance(hue, str):
-            hues = [hue, ]
-        else:
-            hues = hue
-    else:
-        hues = [None, ]
-    
-    # set some UMAP-specific defaults
-    figsize = figsize if figsize is not None else [7, 7]
-    if legend_fontsize is not None:
-            if legend_kwargs is None:
-                legend_kwargs = {'fontsize': legend_fontsize}
-            else:
-                legend_kwargs['fontsize'] = legend_fontsize
-    
-    if len(hues) > 1:
-        n_row = int(np.ceil(len(hues) / n_col))
-        gridsize = [figsize[0] * n_col, figsize[1] * n_row]
-        fig, axes = plt.subplots(n_row, n_col, figsize=gridsize)
-        axes = axes.flatten()
-    else:
-        axes = [ax, ]
-    
-    # make plots
-    for ax, hue in zip(axes, hues):
-        # get X/Y data
-        d = {}
-        x, y = zip(*adata.obsm['X_umap'])
-        d['x'] = x
-        d['y'] = y
-        if hue is not None:
-            d[hue] = get_adata_values(
-                adata,
-                hue, 
-                receptor=receptor, 
-                chain=hue_chain if hue_chain is not None else chain)
-            continuous_hue = all([isinstance(h, float) for h in d[hue]]) and not force_categorical_hue
-        df = pd.DataFrame(d, index=adata.obs.index)        
-
-        # make the plot
-        # ax = scatter(
-        ax = abutils.pl.scatter(
-            data=df,
-            x='x',
-            y='y', 
-            hue=hue, 
-            marker=marker,
-            hue_order=hue_order, 
-            force_categorical_hue=force_categorical_hue,
-            palette=palette,
-            color=color,
-            cmap=cmap if cmap is not None else loupe_cmap,
-            size=size,
-            alpha=alpha,
-            highlight_index=highlight_index,
-            highlight_x=highlight_x,
-            highlight_y=highlight_y,
-            highlight_marker=highlight_marker,
-            highlight_size=highlight_size,
-            highlight_color=highlight_color,
-            highlight_name=highlight_name,
-            highlight_alpha=highlight_alpha,  
-            plot_kwargs=plot_kwargs,
-            legend_kwargs=legend_kwargs,
-            hide_legend=True if legend_on_data else hide_legend,
-            xlabel=xlabel if xlabel is not None else x,
-            ylabel=ylabel if ylabel is not None else y,
-            title=title if title is not None else hue,
-            title_fontsize=title_fontsize,
-            title_fontweight=title_fontweight,
-            title_loc=title_loc,
-            title_pad=title_pad,
-            show_title=show_title,
-            xlabel_fontsize=xlabel_fontsize,
-            ylabel_fontsize=ylabel_fontsize,
-            xtick_labelsize=xtick_labelsize,
-            ytick_labelsize=ytick_labelsize,
-            xtick_labelrotation=xtick_labelrotation,
-            ytick_labelrotation=ytick_labelrotation,
-            cbar_width=cbar_width,
-            cbar_height=cbar_height,
-            cbar_loc=cbar_loc,
-            cbar_orientation=cbar_orientation,
-            cbar_bbox_to_anchor=cbar_bbox_to_anchor,
-            cbar_flip_ticks=cbar_flip_ticks,
-            cbar_title=cbar_title,
-            cbar_title_fontsize=cbar_title_fontsize,
-            hide_cbar=hide_cbar,
-            equal_axes=equal_axes,
-            ax=ax,
-            show=False,
-            figsize=figsize,
-            figfile=None
-        )
+#     .. _any valid inset_axes() location:
+#         https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.axes_grid1.inset_locator.inset_axes.html
 
-        if tiny_axis:
-            # get coords for the UMAP-specific axes
-            if tiny_axis_xoffset is None:
-                tiny_axis_xoffset = 0
-            if tiny_axis_yoffset is None:
-                tiny_axis_yoffset = 0
-            xmin = df['x'].min()
-            xmax = df['x'].max()
-            ymin = df['y'].min()
-            ymax = df['y'].max()
-            x_range = abs(xmax - xmin)
-            y_range = abs(ymax - ymin)
-            x_offset = x_range * tiny_axis_xoffset
-            y_offset = y_range * tiny_axis_yoffset
-            x_start = xmin + x_offset
-            y_start = ymin + x_offset
-            x_end = xmin + (x_range / 5) + x_offset
-            x_center = x_start + ((x_end - x_start) / 2)
-            y_end = ymin + (y_range / 5) + y_offset
-            y_center = y_start + ((y_end - y_start) / 2)
-            # draw the new "mini" axis lines
-            ax.hlines(y_start, x_start, x_end, 'k', lw=2)
-            ax.vlines(x_start, y_start, y_end, 'k', lw=2)
-            ax.annotate(
-                xlabel,
-                xy=(x_center, ymin), 
-                xytext=(0, -5), 
-                textcoords='offset points',
-                fontsize=xlabel_fontsize, 
-                ha='center', 
-                va='top')
-            ax.annotate(
-                ylabel,
-                xy=(xmin, y_center), 
-                xytext=(-5, 0), 
-                textcoords='offset points',
-                fontsize=ylabel_fontsize, 
-                rotation='vertical',
-                ha='right', 
-                va='center')
-            # ax.text(xmin, y_center, ylabel, fontsize=ylabel_fontsize, rotation='vertical', ha='right', va='center')
-            # remove the normal axis lines
-            ax.set_xlabel('', fontsize=0)
-            ax.set_ylabel('', fontsize=0)
-            for s in ['left', 'right', 'top', 'bottom']:
-                ax.spines[s].set_visible(False)
-        # hide the ticks
-        ax.set_xticks([])
-        ax.set_yticks([])
-
-        if legend_on_data and not continuous_hue:
-            # configure the legend font outline
-            if legend_fontoutline is not None:
-                path_effect = [
-                    mpl.patheffects.withStroke(linewidth=legend_fontoutline, foreground='w')
-                ]
-            else:
-                path_effect = None
-            # add the on-data legend
-            for h in df[hue].unique():
-                _df = df[df[hue] == h]
-                hue_x = _df['x'].median()
-                hue_y = _df['y'].median()
-                ax.text(
-                    hue_x, 
-                    hue_y, 
-                    h, 
-                    c='k', 
-                    weight=legend_fontweight,
-                    verticalalignment='center',
-                    horizontalalignment='center',
-                    fontsize=legend_fontsize,
-                    path_effects=path_effect
-                )
+#     """
 
-    # save, show or return the ax
-    if figfile is not None:
-        plt.tight_layout()
-        plt.savefig(figfile)
-    elif show:
-        plt.tight_layout()
-        plt.show()
-    else:
-        return ax
+#     # get x, y and hue data
+#     d = {}
+#     d["x"] = get_adata_values(
+#         adata, x, receptor=receptor, chain=x_chain if x_chain is not None else chain
+#     )
+#     d["y"] = get_adata_values(
+#         adata, y, receptor=receptor, chain=y_chain if y_chain is not None else chain
+#     )
+#     if hue is not None:
+#         d[hue] = get_adata_values(
+#             adata,
+#             hue,
+#             receptor=receptor,
+#             chain=hue_chain if hue_chain is not None else chain,
+#         )
+#     df = pd.DataFrame(d, index=adata.obs.index)
 
+#     ax = abutils.pl.scatter(
+#         data=df,
+#         x="x",
+#         y="y",
+#         hue=hue,
+#         marker=marker,
+#         hue_order=hue_order,
+#         force_categorical_hue=force_categorical_hue,
+#         palette=palette,
+#         color=color,
+#         cmap=cmap,
+#         size=size,
+#         alpha=alpha,
+#         highlight_index=highlight_index,
+#         highlight_x=highlight_x,
+#         highlight_y=highlight_y,
+#         highlight_marker=highlight_marker,
+#         highlight_size=highlight_size,
+#         highlight_color=highlight_color,
+#         highlight_name=highlight_name,
+#         highlight_alpha=highlight_alpha,
+#         plot_kwargs=plot_kwargs,
+#         legend_kwargs=legend_kwargs,
+#         hide_legend=hide_legend,
+#         xlabel=xlabel if xlabel is not None else x,
+#         ylabel=ylabel if ylabel is not None else y,
+#         title=title,
+#         title_fontsize=title_fontsize,
+#         title_fontweight=title_fontweight,
+#         title_loc=title_loc,
+#         title_pad=title_pad,
+#         show_title=show_title,
+#         xlabel_fontsize=xlabel_fontsize,
+#         ylabel_fontsize=ylabel_fontsize,
+#         xtick_labelsize=xtick_labelsize,
+#         ytick_labelsize=ytick_labelsize,
+#         xtick_labelrotation=xtick_labelrotation,
+#         ytick_labelrotation=ytick_labelrotation,
+#         cbar_width=cbar_width,
+#         cbar_height=cbar_height,
+#         cbar_loc=cbar_loc,
+#         cbar_orientation=cbar_orientation,
+#         cbar_bbox_to_anchor=cbar_bbox_to_anchor,
+#         cbar_flip_ticks=cbar_flip_ticks,
+#         cbar_title=cbar_title,
+#         cbar_title_fontsize=cbar_title_fontsize,
+#         hide_cbar=hide_cbar,
+#         equal_axes=equal_axes,
+#         ax=ax,
+#         show=False,
+#         figsize=figsize,
+#         figfile=None,
+#     )
 
+#     # save, show or return the ax
+#     if figfile is not None:
+#         plt.tight_layout()
+#         plt.savefig(figfile)
+#     elif show:
+#         plt.show()
+#     else:
+#         return ax
 
 
+# def umap(
+#     adata,
+#     hue=None,
+#     marker="o",
+#     hue_order=None,
+#     force_categorical_hue=False,
+#     palette=None,
+#     color=None,
+#     cmap=None,
+#     size=10,
+#     alpha=0.6,
+#     n_col=2,
+#     receptor="bcr",
+#     chain="heavy",
+#     hue_chain=None,
+#     highlight_index=None,
+#     highlight_x=None,
+#     highlight_y=None,
+#     highlight_marker="x",
+#     highlight_size=90,
+#     highlight_color="k",
+#     highlight_name=None,
+#     highlight_alpha=0.9,
+#     plot_kwargs=None,
+#     legend_on_data=False,
+#     legend_fontsize=12,
+#     legend_fontweight="bold",
+#     legend_fontoutline=None,
+#     legend_marker_alpha=0.8,
+#     legend_label_position_offsets=None,
+#     legend_kwargs=None,
+#     hide_legend=False,
+#     xlabel="UMAP1",
+#     ylabel="UMAP2",
+#     title=None,
+#     title_fontsize=20,
+#     title_fontweight="normal",
+#     title_loc="center",
+#     title_pad=None,
+#     show_title=True,
+#     xlabel_fontsize=16,
+#     ylabel_fontsize=16,
+#     xtick_labelsize=14,
+#     ytick_labelsize=14,
+#     xtick_labelrotation=0,
+#     ytick_labelrotation=0,
+#     tiny_axis=True,
+#     tiny_axis_xoffset=None,
+#     tiny_axis_yoffset=None,
+#     cbar_width=0.35,
+#     cbar_height=0.05,
+#     cbar_loc="lower right",
+#     cbar_orientation="horizontal",
+#     cbar_bbox_to_anchor=None,
+#     cbar_flip_ticks=False,
+#     cbar_title=None,
+#     cbar_title_fontsize=12,
+#     hide_cbar=False,
+#     equal_axes=True,
+#     ax=None,
+#     show=False,
+#     figsize=None,
+#     figfile=None,
+# ):
+#     """
+#     Produces a scatter plot.
+
+#     Parameters
+#     ----------
+
+#     adata : pandas.DataFrame
+#         A ``anndata.AnnData`` object containing the input data.
+
+#     x : str
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the
+#         x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
+#         if data from different chains is being analyzed, using `x_chain`. BCR/TCR annotation
+#         fields must contain numerical data. Required.
+
+#     y : str
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field to be plotted on the
+#         y-axis. BCR/TCR annotations can be further specified using `receptor` and `chain` or,
+#         if data from different chains is being analyzed, using `y_chain`. BCR/TCR annotation
+#         fields must contain numerical data. Required.
+
+#     hue : str, optional
+#         Name of a column in `adata.obs` or a BCR/TCR annotation field containing hue values.
+#         BCR/TCR annotations can be further specified using `receptor` and `chain` or, if data
+#         from different chains is being analyzed, using `hue_chain`. BCR/TCR annotation
+#         fields must contain numerical data.
+
+#     marker : str, dict or iterable object, optional
+#         Marker style for the scatter plot. Accepts any of the following:
+#           * a `matplotlib marker`_ string
+#           * a ``dict`` mapping `hue` categories to a `matplotlib marker`_ string
+#           * a ``list`` of `matplotlib marker`_ strings, which should be the same
+#               length as `x` and `y`.
+
+#     hue_order : iterable object, optional
+#         List of `hue` categories in the order they should be plotted. If `hue_order` contains a
+#         subset of all categories found in `hue`, only the supplied categories will be plotted.
+#         If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.
+
+#     force_categorical_hue : bool, default=False
+#         If ``True``, `hue` data will be treated as categorical, even if the data appear to
+#         be continuous. This results in `color` being used to color the points rather than `cmap`.
+
+#     palette : dict, optional
+#         Dictionary mapping `hue`, `x` or `y` names to colors. If if keys in `palette` match
+#         more than one category, `hue` categories take priority. If `palette` is not provided,
+#         bars are colored using `color` (if `hue` is ``None``) or a palette is generated
+#         automatically using ``sns.hls_palette()``.
+
+#     color : str or iterable object, optional.
+#         Color for the plot markers. Can be any of the following:
+#           * a ``list`` or ``tuple`` containing RGB or RGBA values
+#           * a color string, either from `Matplotlib's set of named colors`_ or a hex color value
+#           * the name of a column in `data` that contains color values
+#           * a ``list`` of colors (either as strings or RGB tuples) to be used for `hue` categories.
+#             If `colors` is shorter than the list of hue categories, colors will be reused.
+
+#         .. tip::
+#             If a single RGB or RGBA ``list`` or ``tuple`` is provided and `hue` is also supplied,
+#             there may be unexpected results as ``scatter()`` will attempt to map each of the
+#             individual RGB(A) values to a hue category.
+
+#         Only used if `hue` contains categorical data (`cmap` is used for continuous data). If not
+#         provided, the `default Seaborn color palette`_ will be used.
+
+#     cmap : str or matplotlib.color.Colormap, default='flare'
+#         Colormap to be used for continuous `hue` data.
+
+#     size : str or float or iterable object, default=20
+#         Size of the scatter points. Either a
+
+#     alpha : float, default=0.6
+#         Alpha of the scatter points.
+
+#     receptor : str, default='bcr'
+#         Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+#     chain : str, default='heavy'
+#         If `x`, `y` and/or `hue` are BCR/TCR annotation fields, chain for which annotation will be
+#         retrieved. Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``,
+#         ``'beta'``, ``'delta'`` or ``'gamma'``.
+
+#     x_chain : str
+#         `chain` to be used for the x-axis. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     y_chain : str
+#         `chain` to be used for the y-axis. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     hue_chain : str
+#         `chain` to be used for the hue. If not supplied, `chain` will be used. Only necessary
+#         when visualizing data from different chains on the same plot.
+
+#     highlight_index : iterable object, optional
+#         An iterable of index names (present in `data.index`) of points to be highlighted on
+#         the plot. If provided, `highlight_x` and `highlight_y` are ignored.
+
+#     highlight_x : iterable object, optional
+#         An iterable of x-values for highlighted points. Also requires `highlight_y`.
+
+#     highlight_y : iterable object, optional
+#         An iterable of y-values for highlighted points. Also requires `highlight_x`.
+
+#     highlight_marker : str, default='x'
+#         Marker style to be used for highlight points. Accepts any `matplotlib marker`_.
+
+#     highlight_size : int, default=90
+#         Size of the highlight marker.
+
+#     highlight_color : string or list of color values, default='k'
+#         Color of the highlight points.
+
+#     highlight_name : str, optional
+#         Name of the highlights, to be used in the plot legend. If not supplied,
+#         highlight points will not be included in the legend.
+
+#     highlight_alpha : float, default=0.9
+#         Alpha of the highlight points.
+
+#     plot_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``pyplot.scatter()``.
+
+#     legend_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
+
+#     hide_legend : bool, default=False
+#         By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+#         the legend will not be shown.
+
+#     xlabel : str, optional
+#         Text for the X-axis label.
+
+#     ylabel : str, optional
+#         Text for the Y-axis label.
+
+#     xlabel_fontsize : int or float, default=16
+#         Fontsize for the X-axis label text.
+
+#     ylabel_fontsize : int or float, default=16
+#         Fontsize for the Y-axis label text.
+
+#     xtick_labelsize : int or float, default=14
+#         Fontsize for the X-axis tick labels.
+
+#     ytick_labelsize : int or float, default=14
+#         Fontsize for the Y-axis tick labels.
+
+#     xtick_labelrotation : int or float, default=0
+#         Rotation of the X-axis tick labels.
+
+#     ytick_labelrotation : int or float, default=0
+#         Rotation of the Y-axis tick labels.
+
+#     cbar_width : float, default=0.35
+#         Width of the colorbar. Only used for continuous `hue` types.
+
+#     cbar_height : float, default=0.05
+#         Height of the colorbar. Only used for continuous `hue` types.
+
+#     cbar_loc : str or iterable object, default='lower right'
+#         Location of the colorbar. Accepts `any valid inset_axes() location`_.
+
+#     cbar_orientation : str, default='horizontal'
+#         Orientation of the colorbar. Options are ``'horizontal'`` and ``'vertical'``.
+
+#     cbar_bbox_to_anchor : list or tuple, optional
+#         bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide
+#         fine-grained positioning of the colorbar.
+
+#     cbar_flip_ticks : bool, default=False
+#         Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation`
+#         is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.
+
+#     cbar_title : str, optional
+#         Colorbar title. If not provided, `hue` is used.
+
+#     cbar_title_fontsize : int or float, default=12
+#         Fontsize for the colorbar title.
+
+#     hide_cbar : bool, default=False.
+#         If ``True``, the color bar will be hidden on plots with continuous `hue` values.
+
+#     equal_axes : bool, default=True
+#         If ```True```, the the limits of the x- and y-axis will be equal.
+
+#     show :bool, default=False
+#         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
+#         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
+
+#     figsize : iterable object, default=[6, 4]
+#         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
+
+#     figfile : str, optional
+#         Path at which to save the figure file. If not provided, the figure is not saved
+#         and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
+
+
+#     .. _matplotlib marker:
+#         https://matplotlib.org/stable/api/markers_api.html
+
+#     .. _Matplotlib's set of named colors:
+#         https://matplotlib.org/stable/gallery/color/named_colors.html
+
+#     .. _default Seaborn color palette:
+#         https://seaborn.pydata.org/generated/seaborn.color_palette.html
+
+#     .. _any valid inset_axes() location:
+#         https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.axes_grid1.inset_locator.inset_axes.html
+
+#     """
+#     # check that the UMAP data exists
+#     if "X_umap" not in adata.obsm:
+#         from .tl import dimensionality_reduction
+
+#         adata = dimensionality_reduction(adata)
+
+#     # parse hues (if provided)
+#     if hue is not None:
+#         if isinstance(hue, str):
+#             hues = [
+#                 hue,
+#             ]
+#         else:
+#             hues = hue
+#     else:
+#         hues = [
+#             None,
+#         ]
+
+#     # set some UMAP-specific defaults
+#     figsize = figsize if figsize is not None else [7, 7]
+#     if legend_fontsize is not None:
+#         if legend_kwargs is None:
+#             legend_kwargs = {"fontsize": legend_fontsize}
+#         else:
+#             legend_kwargs["fontsize"] = legend_fontsize
+
+#     if len(hues) > 1:
+#         n_row = int(np.ceil(len(hues) / n_col))
+#         gridsize = [figsize[0] * n_col, figsize[1] * n_row]
+#         fig, axes = plt.subplots(n_row, n_col, figsize=gridsize)
+#         axes = axes.flatten()
+#     else:
+#         axes = [
+#             ax,
+#         ]
+
+#     # make plots
+#     for ax, hue in zip(axes, hues):
+#         # get X/Y data
+#         d = {}
+#         x, y = zip(*adata.obsm["X_umap"])
+#         d["x"] = x
+#         d["y"] = y
+#         if hue is not None:
+#             d[hue] = get_adata_values(
+#                 adata,
+#                 hue,
+#                 receptor=receptor,
+#                 chain=hue_chain if hue_chain is not None else chain,
+#             )
+#             continuous_hue = (
+#                 all([isinstance(h, float) for h in d[hue]])
+#                 and not force_categorical_hue
+#             )
+#         df = pd.DataFrame(d, index=adata.obs.index)
+
+#         # make the plot
+#         # ax = scatter(
+#         ax = abutils.pl.scatter(
+#             data=df,
+#             x="x",
+#             y="y",
+#             hue=hue,
+#             marker=marker,
+#             hue_order=hue_order,
+#             force_categorical_hue=force_categorical_hue,
+#             palette=palette,
+#             color=color,
+#             cmap=cmap if cmap is not None else loupe_cmap,
+#             size=size,
+#             alpha=alpha,
+#             highlight_index=highlight_index,
+#             highlight_x=highlight_x,
+#             highlight_y=highlight_y,
+#             highlight_marker=highlight_marker,
+#             highlight_size=highlight_size,
+#             highlight_color=highlight_color,
+#             highlight_name=highlight_name,
+#             highlight_alpha=highlight_alpha,
+#             plot_kwargs=plot_kwargs,
+#             legend_kwargs=legend_kwargs,
+#             hide_legend=True if legend_on_data else hide_legend,
+#             xlabel=xlabel if xlabel is not None else x,
+#             ylabel=ylabel if ylabel is not None else y,
+#             title=title if title is not None else hue,
+#             title_fontsize=title_fontsize,
+#             title_fontweight=title_fontweight,
+#             title_loc=title_loc,
+#             title_pad=title_pad,
+#             show_title=show_title,
+#             xlabel_fontsize=xlabel_fontsize,
+#             ylabel_fontsize=ylabel_fontsize,
+#             xtick_labelsize=xtick_labelsize,
+#             ytick_labelsize=ytick_labelsize,
+#             xtick_labelrotation=xtick_labelrotation,
+#             ytick_labelrotation=ytick_labelrotation,
+#             cbar_width=cbar_width,
+#             cbar_height=cbar_height,
+#             cbar_loc=cbar_loc,
+#             cbar_orientation=cbar_orientation,
+#             cbar_bbox_to_anchor=cbar_bbox_to_anchor,
+#             cbar_flip_ticks=cbar_flip_ticks,
+#             cbar_title=cbar_title,
+#             cbar_title_fontsize=cbar_title_fontsize,
+#             hide_cbar=hide_cbar,
+#             equal_axes=equal_axes,
+#             ax=ax,
+#             show=False,
+#             figsize=figsize,
+#             figfile=None,
+#         )
+
+#         if tiny_axis:
+#             # get coords for the UMAP-specific axes
+#             if tiny_axis_xoffset is None:
+#                 tiny_axis_xoffset = 0
+#             if tiny_axis_yoffset is None:
+#                 tiny_axis_yoffset = 0
+#             xmin = df["x"].min()
+#             xmax = df["x"].max()
+#             ymin = df["y"].min()
+#             ymax = df["y"].max()
+#             x_range = abs(xmax - xmin)
+#             y_range = abs(ymax - ymin)
+#             x_offset = x_range * tiny_axis_xoffset
+#             y_offset = y_range * tiny_axis_yoffset
+#             x_start = xmin + x_offset
+#             y_start = ymin + x_offset
+#             x_end = xmin + (x_range / 5) + x_offset
+#             x_center = x_start + ((x_end - x_start) / 2)
+#             y_end = ymin + (y_range / 5) + y_offset
+#             y_center = y_start + ((y_end - y_start) / 2)
+#             # draw the new "mini" axis lines
+#             ax.hlines(y_start, x_start, x_end, "k", lw=2)
+#             ax.vlines(x_start, y_start, y_end, "k", lw=2)
+#             ax.annotate(
+#                 xlabel,
+#                 xy=(x_center, ymin),
+#                 xytext=(0, -5),
+#                 textcoords="offset points",
+#                 fontsize=xlabel_fontsize,
+#                 ha="center",
+#                 va="top",
+#             )
+#             ax.annotate(
+#                 ylabel,
+#                 xy=(xmin, y_center),
+#                 xytext=(-5, 0),
+#                 textcoords="offset points",
+#                 fontsize=ylabel_fontsize,
+#                 rotation="vertical",
+#                 ha="right",
+#                 va="center",
+#             )
+#             # ax.text(xmin, y_center, ylabel, fontsize=ylabel_fontsize, rotation='vertical', ha='right', va='center')
+#             # remove the normal axis lines
+#             ax.set_xlabel("", fontsize=0)
+#             ax.set_ylabel("", fontsize=0)
+#             for s in ["left", "right", "top", "bottom"]:
+#                 ax.spines[s].set_visible(False)
+#         # hide the ticks
+#         ax.set_xticks([])
+#         ax.set_yticks([])
+
+#         if legend_on_data and not continuous_hue:
+#             # set up label offsets
+#             if legend_label_position_offsets is None:
+#                 legend_label_position_offsets = {}
+#             _xlim = ax.get_xlim()
+#             _ylim = ax.get_ylim()
+#             _xrange = _xlim[1] - _xlim[0]
+#             _yrange = _ylim[1] - _ylim[0]
+#             # configure the legend font outline
+#             if legend_fontoutline is not None:
+#                 path_effect = [
+#                     mpl.patheffects.withStroke(
+#                         linewidth=legend_fontoutline, foreground="w"
+#                     )
+#                 ]
+#             else:
+#                 path_effect = None
+#             # add the on-data legend
+#             for h in df[hue].unique():
+#                 _df = df[df[hue] == h]
+#                 xoffset, yoffset = legend_label_position_offsets.get(h, (0, 0))
+#                 hue_x = _df["x"].median() + (xoffset * _xrange)
+#                 hue_y = _df["y"].median() + (yoffset * _yrange)
+#                 ax.text(
+#                     hue_x,
+#                     hue_y,
+#                     h,
+#                     c="k",
+#                     weight=legend_fontweight,
+#                     verticalalignment="center",
+#                     horizontalalignment="center",
+#                     fontsize=legend_fontsize,
+#                     path_effects=path_effect,
+#                 )
+
+#     # save, show or return the ax
+#     if figfile is not None:
+#         plt.tight_layout()
+#         plt.savefig(figfile)
+#     elif show:
+#         plt.tight_layout()
+#         plt.show()
+#     else:
+#         return ax
+
 
 # def feature_scatter(
 #     data,
 #     x,
 #     y,
 #     hue=None,
 #     hue_order=None,
@@ -1417,141 +1443,141 @@
 #     **kwargs,
 # ):
 #     """
 #     Produces a scatter plot of two features, optionally colored by a third feature.
 
 #     Parameters
 #     ----------
-#     data : anndata.AnnData or pandas.DataFrame  
+#     data : anndata.AnnData or pandas.DataFrame
 #         An ``AnnData`` object or a ``DataFrame`` containing the input data. Required.
 
 #     x : str
 #         Name of the column in `data` containing the feature to be plotted on the x-axis. Required.
 
-#     y : str  
+#     y : str
 #         Name of the column in `data` containing the feature to be plotted on the y-axis. Required.
 
-#     hue : str, optional  
+#     hue : str, optional
 #         Name of the column in `data` containing categories for hue values. If `hue` is categorical,
-#         each category will be plotted in a different color (using the `color` for the colors). If 
-#         `hue` is continuous, points will be colored using a colormap (using `cmap` if supplied). 
+#         each category will be plotted in a different color (using the `color` for the colors). If
+#         `hue` is continuous, points will be colored using a colormap (using `cmap` if supplied).
 
-#     hue_order : iterable object, optional  
+#     hue_order : iterable object, optional
 #         Iterable of hue categories, in the order they should be plotted and listed
 #         in the legend. If `hue_order` contains only a subset of the categories
 #         present in ``data[hue]`` or ``data.obs[hue]``, only the categories supplied in `hue_order`
 #         will be plotted.
 
-#     force_categorical_hue : bool, default=False  
-#         If ``True``, `hue` data will be treated as categorical, even if the data appear to 
-#         be continuous. This results in `color` being used to color the points rather than `cmap`.  
+#     force_categorical_hue : bool, default=False
+#         If ``True``, `hue` data will be treated as categorical, even if the data appear to
+#         be continuous. This results in `color` being used to color the points rather than `cmap`.
 
 #     color : iterable object, optinoal
-#         List of colors to be used for `hue` categories. If `colors` is shorter than the list 
-#         of hue categories, colors will be reused. Only used if `hue` contains categorical data 
-#         (`cmap` is used for continuous data). If not provided, the `default Seaborn color palette`_ 
-#         will be used. 
-        
-#     cmap : str or matplotlib.color.Colormap, default='flare'   
-#         Colormap to be used for continuous `hue` data.  
+#         List of colors to be used for `hue` categories. If `colors` is shorter than the list
+#         of hue categories, colors will be reused. Only used if `hue` contains categorical data
+#         (`cmap` is used for continuous data). If not provided, the `default Seaborn color palette`_
+#         will be used.
 
-#     cbar_width : int, default=35  
-#         Width of the colorbar. Only used for continuous `hue` types.  
+#     cmap : str or matplotlib.color.Colormap, default='flare'
+#         Colormap to be used for continuous `hue` data.
 
-#     cbar_height : int, default=5  
-#         Height of the colorbar. Only used for continuous `hue` types.  
+#     cbar_width : int, default=35
+#         Width of the colorbar. Only used for continuous `hue` types.
 
-#     cbar_loc : str or iterable object, default='lower right'  
+#     cbar_height : int, default=5
+#         Height of the colorbar. Only used for continuous `hue` types.
+
+#     cbar_loc : str or iterable object, default='lower right'
 #         Location of the colorbar. Accepts `any valid inset_axes() location`_.
 
-#     cbar_orientation : str, default='horizontal'  
+#     cbar_orientation : str, default='horizontal'
 #         Orientation of the colorbar. Options are ``'horizontal'`` and ``'vertical'``.
 
 #     cbar_bbox_to_anchor : list or tuple, optional
-#         bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide 
+#         bbox_to_anchor for the colorbar. Used in combination with `cbar_loc` to provide
 #         fine-grained positioning of the colorbar.
 
-#     cbar_flip_ticks : bool, default=False  
-#         Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation` 
-#         is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.  
-
-#     cbar_title : str, optional  
-#         Colorbar title. If not provided, `hue` is used.  
-
-#     cbar_title_fontsize : int or float, default=12  
-#         Fontsize for the colorbar title.  
-        
-#     marker : str, default='o'  
-#         Marker style for the scatter plot. Accepts any `matplotlib marker`_.  
+#     cbar_flip_ticks : bool, default=False
+#         Flips the position of colorbar ticks. Ticks default to the bottom if `cbar_orientation`
+#         is  ``'horizontal'`` and the left if  `cbar_orientation` is ``'vertical'``.
+
+#     cbar_title : str, optional
+#         Colorbar title. If not provided, `hue` is used.
 
-#     size : int or float, default=20  
-#         Size of the scatter points.  
+#     cbar_title_fontsize : int or float, default=12
+#         Fontsize for the colorbar title.
 
-#     alpha : float, default=0.6  
-#         Alpha of the scatter points.  
+#     marker : str, default='o'
+#         Marker style for the scatter plot. Accepts any `matplotlib marker`_.
 
-#     highlight_index : iterable object, optional  
-#         An iterable of index names (present in `data`) of points to be highlighted on 
+#     size : int or float, default=20
+#         Size of the scatter points.
+
+#     alpha : float, default=0.6
+#         Alpha of the scatter points.
+
+#     highlight_index : iterable object, optional
+#         An iterable of index names (present in `data`) of points to be highlighted on
 #         the KDE plot. If provided, `highlight_x` and `highlight_y` are ignored.
 
-#     highlight_x : iterable object, optional  
+#     highlight_x : iterable object, optional
 #         An iterable of x-values for highlighted points. Also requires `highlight_y`.
-        
-#     highlight_y : iterable object, optional  
+
+#     highlight_y : iterable object, optional
 #         An iterable of y-values for highlighted points. Also requires `highlight_x`.
-        
-#     highlight_marker : str, default='x'  
-#         Marker style to be used for highlight points. Accepts any `matplotlib marker`_. 
 
-#     highlight_size : int, default=90  
+#     highlight_marker : str, default='x'
+#         Marker style to be used for highlight points. Accepts any `matplotlib marker`_.
+
+#     highlight_size : int, default=90
 #         Size of the highlight marker.
 
 #     highlight_color : string or list of color values, default='k'
 #         Color of the highlight points.
 
-#     highlight_name : str, optional  
+#     highlight_name : str, optional
 #         Name of the highlights, to be used in the plot legend. If not supplied,
 #         highlight points will not be included in the legend.
-        
-#     highlight_alpha : float, default=0.9  
+
+#     highlight_alpha : float, default=0.9
 #         Alpha of the highlight points.
 
-#     xlabel : str, optional  
+#     xlabel : str, optional
 #         Label for the x-axis. By default, the value for `x` is used.
 
-#     ylabel : str, optional  
+#     ylabel : str, optional
 #         Label for the y-axis. By default, the value for `y` is used.
 
 #     equal_axes : bool, default=True
 #         If ```True```, the the limits of the x- and y-axis will be equal.
-        
-#     legend_kwargs : dict, optional  
+
+#     legend_kwargs : dict, optional
 #         Dictionary of legend keyword arguments, which will be passed to ``ax.legend()``.
 
-#     return_ax : bool, default=False  
+#     return_ax : bool, default=False
 #         If ``True``, return the plot's ``ax`` object. Will not show or save the plot.
 
-#     figsize : list, default=[6, 6]  
+#     figsize : list, default=[6, 6]
 #         A list containg the dimensions of the plot, in inches.
 
-#     figfile : str, optional  
-#         Path to which the figure will be saved. If not provided, the figure will be 
-#         shown but not saved to file.  
+#     figfile : str, optional
+#         Path to which the figure will be saved. If not provided, the figure will be
+#         shown but not saved to file.
 
 #     kwargs
-#         All other keyword arguments are passed to ``matplotlib.pyplot.scatter()``.  
+#         All other keyword arguments are passed to ``matplotlib.pyplot.scatter()``.
 
 
-#     .. _default Seaborn color palette: 
-#         https://seaborn.pydata.org/generated/seaborn.color_palette.html  
+#     .. _default Seaborn color palette:
+#         https://seaborn.pydata.org/generated/seaborn.color_palette.html
 
-#     .. _matplotlib marker: 
-#         https://matplotlib.org/stable/api/markers_api.html  
+#     .. _matplotlib marker:
+#         https://matplotlib.org/stable/api/markers_api.html
 
-#     .. _any valid inset_axes() location: 
+#     .. _any valid inset_axes() location:
 #         https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.axes_grid1.inset_locator.inset_axes.html
 
 #     """
 #     # input data
 #     if isinstance(data, AnnData):
 #         _data = {}
 #         for var in [x, y, hue]:
@@ -1959,261 +1985,256 @@
 
     if figfile is not None:
         g.savefig(figfile)
     else:
         plt.show()
 
 
-
 # ===========================
 
 #          GENERAL
 
 # ===========================
 
 
-def bar(
-    adata, 
-    *,
-    x=None,
-    y=None,
-    hue=None, 
-    order=None, 
-    hue_order=None, 
-    palette=None,
-    color=None,
-    alt_color='#D3D3D3',
-    normalize=False, 
-    highlight=None, 
-    highlight_color=None,  
-    receptor='bcr',
-    chain='heavy', 
-    x_chain=None,
-    y_chain=None,
-    hue_chain=None,
-    orientation='vertical',
-    plot_kwargs=None,
-    legend_kwargs=None,
-    hide_legend=False,
-    xlabel=None,
-    ylabel=None,
-    xlabel_fontsize=16,
-    ylabel_fontsize=16,
-    xtick_labelsize=14,
-    ytick_labelsize=14,
-    xtick_labelrotation=0,
-    ytick_labelrotation=0,
-    show=False,
-    figsize=[6,4],
-    figfile=None,):
-    '''
-    Produces a bar plot of categorical data. For data with distinct batches, a stacked 
-    bar plot will be constructed.
+# def bar(
+#     adata,
+#     *,
+#     x=None,
+#     y=None,
+#     hue=None,
+#     order=None,
+#     hue_order=None,
+#     palette=None,
+#     color=None,
+#     alt_color="#D3D3D3",
+#     normalize=False,
+#     highlight=None,
+#     highlight_color=None,
+#     receptor="bcr",
+#     chain="heavy",
+#     x_chain=None,
+#     y_chain=None,
+#     hue_chain=None,
+#     orientation="vertical",
+#     plot_kwargs=None,
+#     legend_kwargs=None,
+#     hide_legend=False,
+#     xlabel=None,
+#     ylabel=None,
+#     xlabel_fontsize=16,
+#     ylabel_fontsize=16,
+#     xtick_labelsize=14,
+#     ytick_labelsize=14,
+#     xtick_labelrotation=0,
+#     ytick_labelrotation=0,
+#     show=False,
+#     figsize=[6, 4],
+#     figfile=None,
+# ):
+#     """
+#     Produces a bar plot of categorical data. For data with distinct batches, a stacked
+#     bar plot will be constructed.
 
-    Parameters
-    ----------
-    adata : anndata.AnnData  
-        An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr`` 
-        or ``adata.obs.tcr`` populated with annotated BCR/TCR information. Required
-        
-    x : str
-        Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be plotted on the 
-        x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain`. 
-        Required.
-
-    hue : str, optional  
-        Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be used to 
-        group data into stacked bars. If not provided, an un-stacked bar plot is created.  
-        
-    order : iterable object, optional  
-        List of `x` categories in the order they should be plotted. If `order` contains a 
-        subset of all categories found in `x`, only the supplied categories will be plotted.  
-        If not provided, categories will be plotted in ``natsort.natsorted()`` order.
-        
-    hue_order : iterable object, optional  
-        List of `hue` categories in the order they should be plotted. If `hue_order` contains a 
-        subset of all categories found in `hue`, only the supplied categories will be plotted.  
-        If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.
-        
-    palette : dict, optional  
-        Dictionary mapping `hue` or `x` names to colors. If both are provided, `hue` categories 
-        take priority. If neither `palette` nor `color` are provided, bars are colored using 
-        `color` (if `hue` is ``None``) or a palette is generated automatically using 
-        ``sns.hls_palette()``.   
-
-    color : str or iterable, optional  
-        Single color to be used for the bar plot. If not provided, the first color in the 
-        default ``Seaborn`` color palette will be used. If `highlight` is provided but 
-        `highlight_color` is not, `color` will be used to color highlighted bars.  
-        
-    alt_color : str or iterable, default='#D3D3D3'  
-        Alternate color for the bar plot. Used to color categories not provided in `palette` 
-        or to color categories not present in `highlight`.  
-
-    orientation : str, optional
-        Orientation of the plot. Options are ``'vertical'`` or ``'horizontal'``. Default is 
-        ``'vertical'``.  
-        
-    normalize : bool, default=False  
-        If ``True``, normalized frequencies are plotted instead of raw counts. If multiple `hue`
-        categories are present, each `x` category will be separately normalized such that all 
-        bars extend from [0,1] and each stacked bar is sized according to its fraction of the 
-        `x` category. If `hue` is not provided or there is only one `hue` category, the entire 
-        dataset is normalized.
-        
-    highlight : iterable, optional
-        List of `x` or `hue` categories to be highlighted. If `highlight_color` is provided, 
-        categories in `highlight` will use `highlight_color` and all others will use `alt_color`. 
-        If `highlight_color` is not provided, `palette` will be used. If both `highlight_color` 
-        and `palette` are not provided, `color` will be used. 
-        
-    highlight_color : str or iterable, optional  
-        Color to be used for categories in `highlight`. If  
-
-    receptor : str, default='bcr'  
-        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.  
-
-    chain : str, default='heavy'  
-        If `x` is a BCR/TCR annotation field, chain for which annotation will be retrieved. 
-        Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``, 
-        ``'beta'``, ``'delta'`` or ``'gamma'``.  
+#     Parameters
+#     ----------
+#     adata : anndata.AnnData
+#         An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr``
+#         or ``adata.obs.tcr`` populated with annotated BCR/TCR information. Required
 
-    plot_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``pyplot.bar()``.
+#     x : str
+#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be plotted on the
+#         x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain`.
+#         Required.
 
-    legend_kwargs : dict, optional  
-        Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
+#     hue : str, optional
+#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be used to
+#         group data into stacked bars. If not provided, an un-stacked bar plot is created.
+
+#     order : iterable object, optional
+#         List of `x` categories in the order they should be plotted. If `order` contains a
+#         subset of all categories found in `x`, only the supplied categories will be plotted.
+#         If not provided, categories will be plotted in ``natsort.natsorted()`` order.
 
-    hide_legend : bool, default=False  
-        By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-        the legend will not be shown.  
-        
-    xlabel : str, optional  
-        Text for the X-axis label. 
-
-    ylabel : str, optional  
-        Text for the Y-axis label.  
-        
-    xlabel_fontsize : int or float, default=16  
-        Fontsize for the X-axis label text.
+#     hue_order : iterable object, optional
+#         List of `hue` categories in the order they should be plotted. If `hue_order` contains a
+#         subset of all categories found in `hue`, only the supplied categories will be plotted.
+#         If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.
 
-    ylabel_fontsize : int or float, default=16  
-        Fontsize for the Y-axis label text.
+#     palette : dict, optional
+#         Dictionary mapping `hue` or `x` names to colors. If both are provided, `hue` categories
+#         take priority. If neither `palette` nor `color` are provided, bars are colored using
+#         `color` (if `hue` is ``None``) or a palette is generated automatically using
+#         ``sns.hls_palette()``.
+
+#     color : str or iterable, optional
+#         Single color to be used for the bar plot. If not provided, the first color in the
+#         default ``Seaborn`` color palette will be used. If `highlight` is provided but
+#         `highlight_color` is not, `color` will be used to color highlighted bars.
+
+#     alt_color : str or iterable, default='#D3D3D3'
+#         Alternate color for the bar plot. Used to color categories not provided in `palette`
+#         or to color categories not present in `highlight`.
+
+#     orientation : str, optional
+#         Orientation of the plot. Options are ``'vertical'`` or ``'horizontal'``. Default is
+#         ``'vertical'``.
 
-    xtick_labelsize : int or float, default=14  
-        Fontsize for the X-axis tick labels.  
+#     normalize : bool, default=False
+#         If ``True``, normalized frequencies are plotted instead of raw counts. If multiple `hue`
+#         categories are present, each `x` category will be separately normalized such that all
+#         bars extend from [0,1] and each stacked bar is sized according to its fraction of the
+#         `x` category. If `hue` is not provided or there is only one `hue` category, the entire
+#         dataset is normalized.
 
-    ytick_labelsize : int or float, default=14  
-        Fontsize for the Y-axis tick labels.  
+#     highlight : iterable, optional
+#         List of `x` or `hue` categories to be highlighted. If `highlight_color` is provided,
+#         categories in `highlight` will use `highlight_color` and all others will use `alt_color`.
+#         If `highlight_color` is not provided, `palette` will be used. If both `highlight_color`
+#         and `palette` are not provided, `color` will be used.
+
+#     highlight_color : str or iterable, optional
+#         Color to be used for categories in `highlight`. If
+
+#     receptor : str, default='bcr'
+#         Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+#     chain : str, default='heavy'
+#         If `x` is a BCR/TCR annotation field, chain for which annotation will be retrieved.
+#         Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``,
+#         ``'beta'``, ``'delta'`` or ``'gamma'``.
 
-    xtick_labelrotation : int or float, default=0  
-        Rotation of the X-axis tick labels.  
-    
-    ytick_labelrotation : int or float, default=0  
-        Rotation of the Y-axis tick labels. 
+#     plot_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``pyplot.bar()``.
 
-    show :bool, default=False  
-        If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
-        is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
+#     legend_kwargs : dict, optional
+#         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
 
-    figsize : iterable object, default=[6, 4]  
-        List containing the figure size (as ``[x-dimension, y-dimension]``) in inches. 
+#     hide_legend : bool, default=False
+#         By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+#         the legend will not be shown.
 
-    figfile : str, optional  
-        Path at which to save the figure file. If not provided, the figure is not saved
-        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.  
-    '''
+#     xlabel : str, optional
+#         Text for the X-axis label.
 
-    # get x, y and hue data
-    d = {}
-    if x is not None:
-        d['x'] = get_adata_values(
-            adata,
-            x, 
-            receptor=receptor, 
-            chain=x_chain if x_chain is not None else chain)
-        if xlabel is None:
-            xlabel = x
-        x = 'x'
-    if y is not None:
-        d['y'] = get_adata_values(
-            adata,
-            y, 
-            receptor=receptor, 
-            chain=y_chain if y_chain is not None else chain)
-        if ylabel is None:
-            ylabel = y
-        y = 'y'
-    if hue is not None:
-        d[hue] = get_adata_values(
-            adata,
-            hue, 
-            receptor=receptor, 
-            chain=hue_chain if hue_chain is not None else chain)
-    df = pd.DataFrame(d)
+#     ylabel : str, optional
+#         Text for the Y-axis label.
 
-    # make the plot
-    ax = abutils.pl.bar(
-        data=df,
-        x=x,
-        y=y, 
-        hue=hue, 
-        order=order, 
-        hue_order=hue_order, 
-        palette=palette,
-        color=color,
-        alt_color=alt_color,
-        normalize=normalize, 
-        highlight=highlight, 
-        highlight_color=highlight_color,  
-        orientation=orientation,
-        plot_kwargs=plot_kwargs,
-        legend_kwargs=legend_kwargs,
-        hide_legend=hide_legend,
-        xlabel=xlabel,
-        ylabel=ylabel,
-        xlabel_fontsize=xlabel_fontsize,
-        ylabel_fontsize=ylabel_fontsize,
-        xtick_labelsize=xtick_labelsize,
-        ytick_labelsize=ytick_labelsize,
-        xtick_labelrotation=xtick_labelrotation,
-        ytick_labelrotation=ytick_labelrotation,
-        show=False,
-        figsize=figsize,
-        figfile=None,
-        )
+#     xlabel_fontsize : int or float, default=16
+#         Fontsize for the X-axis label text.
 
-    # save, show or return the ax
-    if figfile is not None:
-        plt.tight_layout()
-        plt.savefig(figfile)
-    elif show:
-        plt.show()
-    else:
-        return ax
+#     ylabel_fontsize : int or float, default=16
+#         Fontsize for the Y-axis label text.
+
+#     xtick_labelsize : int or float, default=14
+#         Fontsize for the X-axis tick labels.
+
+#     ytick_labelsize : int or float, default=14
+#         Fontsize for the Y-axis tick labels.
+
+#     xtick_labelrotation : int or float, default=0
+#         Rotation of the X-axis tick labels.
+
+#     ytick_labelrotation : int or float, default=0
+#         Rotation of the Y-axis tick labels.
+
+#     show :bool, default=False
+#         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
+#         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
 
+#     figsize : iterable object, default=[6, 4]
+#         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
+
+#     figfile : str, optional
+#         Path at which to save the figure file. If not provided, the figure is not saved
+#         and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
+#     """
+
+#     # get x, y and hue data
+#     d = {}
+#     if x is not None:
+#         d["x"] = get_adata_values(
+#             adata, x, receptor=receptor, chain=x_chain if x_chain is not None else chain
+#         )
+#         if xlabel is None:
+#             xlabel = x
+#         x = "x"
+#     if y is not None:
+#         d["y"] = get_adata_values(
+#             adata, y, receptor=receptor, chain=y_chain if y_chain is not None else chain
+#         )
+#         if ylabel is None:
+#             ylabel = y
+#         y = "y"
+#     if hue is not None:
+#         d[hue] = get_adata_values(
+#             adata,
+#             hue,
+#             receptor=receptor,
+#             chain=hue_chain if hue_chain is not None else chain,
+#         )
+#     df = pd.DataFrame(d)
 
+#     df = df.dropna(subset=["x"])
 
+#     # make the plot
+#     ax = abutils.pl.bar(
+#         data=df,
+#         x=x,
+#         y=y,
+#         hue=hue,
+#         order=order,
+#         hue_order=hue_order,
+#         palette=palette,
+#         color=color,
+#         alt_color=alt_color,
+#         normalize=normalize,
+#         highlight=highlight,
+#         highlight_color=highlight_color,
+#         orientation=orientation,
+#         plot_kwargs=plot_kwargs,
+#         legend_kwargs=legend_kwargs,
+#         hide_legend=hide_legend,
+#         xlabel=xlabel,
+#         ylabel=ylabel,
+#         xlabel_fontsize=xlabel_fontsize,
+#         ylabel_fontsize=ylabel_fontsize,
+#         xtick_labelsize=xtick_labelsize,
+#         ytick_labelsize=ytick_labelsize,
+#         xtick_labelrotation=xtick_labelrotation,
+#         ytick_labelrotation=ytick_labelrotation,
+#         show=False,
+#         figsize=figsize,
+#         figfile=None,
+#     )
 
+#     # save, show or return the ax
+#     if figfile is not None:
+#         plt.tight_layout()
+#         plt.savefig(figfile)
+#     elif show:
+#         plt.show()
+#     else:
+#         return ax
 
 
 # def bar(
-#     adata, 
-#     x, 
-#     hue=None, 
-#     order=None, 
-#     hue_order=None, 
+#     adata,
+#     x,
+#     hue=None,
+#     order=None,
+#     hue_order=None,
 #     palette=None,
 #     color=None,
 #     alt_color='#D3D3D3',
-#     normalize=False, 
-#     highlight=None, 
-#     highlight_color=None,  
+#     normalize=False,
+#     highlight=None,
+#     highlight_color=None,
 #     receptor='bcr',
-#     chain='heavy', 
+#     chain='heavy',
 #     # orientation='vertical',
 #     plot_kwargs=None,
 #     legend_kwargs=None,
 #     hide_legend=False,
 #     xlabel=None,
 #     ylabel=None,
 #     xlabel_fontsize=16,
@@ -2222,132 +2243,132 @@
 #     ytick_labelsize=14,
 #     xtick_labelrotation=0,
 #     ytick_labelrotation=0,
 #     show=False,
 #     figsize=[6,4],
 #     figfile=None,):
 #     '''
-#     Produces a bar plot of categorical data. For data with distinct batches, a stacked 
+#     Produces a bar plot of categorical data. For data with distinct batches, a stacked
 #     bar plot will be constructed.
 
 #     Parameters
 #     ----------
-#     adata : anndata.AnnData  
-#         An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr`` 
+#     adata : anndata.AnnData
+#         An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr``
 #         or ``adata.obs.tcr`` populated with annotated BCR/TCR information. Required
-        
+
 #     x : str
-#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be plotted on the 
-#         x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain`. 
+#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be plotted on the
+#         x-axis. BCR/TCR annotations can be further specified using `receptor` and `chain`.
 #         Required.
 
-#     hue : str, optional  
-#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be used to 
-#         group data into stacked bars. If not provided, an un-stacked bar plot is created.  
-        
-#     order : iterable object, optional  
-#         List of `x` categories in the order they should be plotted. If `order` contains a 
-#         subset of all categories found in `x`, only the supplied categories will be plotted.  
+#     hue : str, optional
+#         Name of a column in ``adata.obs`` or a BCR/TCR annotation field to be used to
+#         group data into stacked bars. If not provided, an un-stacked bar plot is created.
+
+#     order : iterable object, optional
+#         List of `x` categories in the order they should be plotted. If `order` contains a
+#         subset of all categories found in `x`, only the supplied categories will be plotted.
 #         If not provided, categories will be plotted in ``natsort.natsorted()`` order.
-        
-#     hue_order : iterable object, optional  
-#         List of `hue` categories in the order they should be plotted. If `hue_order` contains a 
-#         subset of all categories found in `hue`, only the supplied categories will be plotted.  
+
+#     hue_order : iterable object, optional
+#         List of `hue` categories in the order they should be plotted. If `hue_order` contains a
+#         subset of all categories found in `hue`, only the supplied categories will be plotted.
 #         If not provided, `hue` categories will be plotted in ``natsort.natsorted()`` order.
-        
-#     palette : dict, optional  
-#         Dictionary mapping `hue` or `x` names to colors. If both are provided, `hue` categories 
-#         take priority. If neither `palette` nor `color` are provided, bars are colored using 
-#         `color` (if `hue` is ``None``) or a palette is generated automatically using 
-#         ``sns.hls_palette()``.   
-
-#     color : str or iterable, optional  
-#         Single color to be used for the bar plot. If not provided, the first color in the 
-#         default ``Seaborn`` color palette will be used. If `highlight` is provided but 
-#         `highlight_color` is not, `color` will be used to color highlighted bars.  
-        
-#     alt_color : str or iterable, default='#D3D3D3'  
-#         Alternate color for the bar plot. Used to color categories not provided in `palette` 
-#         or to color categories not present in `highlight`.  
-        
-#     normalize : bool, default=False  
+
+#     palette : dict, optional
+#         Dictionary mapping `hue` or `x` names to colors. If both are provided, `hue` categories
+#         take priority. If neither `palette` nor `color` are provided, bars are colored using
+#         `color` (if `hue` is ``None``) or a palette is generated automatically using
+#         ``sns.hls_palette()``.
+
+#     color : str or iterable, optional
+#         Single color to be used for the bar plot. If not provided, the first color in the
+#         default ``Seaborn`` color palette will be used. If `highlight` is provided but
+#         `highlight_color` is not, `color` will be used to color highlighted bars.
+
+#     alt_color : str or iterable, default='#D3D3D3'
+#         Alternate color for the bar plot. Used to color categories not provided in `palette`
+#         or to color categories not present in `highlight`.
+
+#     normalize : bool, default=False
 #         If ``True``, normalized frequencies are plotted instead of raw counts. If multiple `hue`
-#         categories are present, each `x` category will be separately normalized such that all 
-#         bars extend from [0,1] and each stacked bar is sized according to its fraction of the 
-#         `x` category. If `hue` is not provided or there is only one `hue` category, the entire 
+#         categories are present, each `x` category will be separately normalized such that all
+#         bars extend from [0,1] and each stacked bar is sized according to its fraction of the
+#         `x` category. If `hue` is not provided or there is only one `hue` category, the entire
 #         dataset is normalized.
-        
+
 #     highlight : iterable, optional
-#         List of `x` or `hue` categories to be highlighted. If `highlight_color` is provided, 
-#         categories in `highlight` will use `highlight_color` and all others will use `alt_color`. 
-#         If `highlight_color` is not provided, `palette` will be used. If both `highlight_color` 
-#         and `palette` are not provided, `color` will be used. 
-        
-#     highlight_color : str or iterable, optional  
-#         Color to be used for categories in `highlight`. If  
-
-#     receptor : str, default='bcr'  
-#         Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.  
-
-#     chain : str, default='heavy'  
-#         If `x` is a BCR/TCR annotation field, chain for which annotation will be retrieved. 
-#         Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``, 
-#         ``'beta'``, ``'delta'`` or ``'gamma'``.  
+#         List of `x` or `hue` categories to be highlighted. If `highlight_color` is provided,
+#         categories in `highlight` will use `highlight_color` and all others will use `alt_color`.
+#         If `highlight_color` is not provided, `palette` will be used. If both `highlight_color`
+#         and `palette` are not provided, `color` will be used.
+
+#     highlight_color : str or iterable, optional
+#         Color to be used for categories in `highlight`. If
+
+#     receptor : str, default='bcr'
+#         Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+#     chain : str, default='heavy'
+#         If `x` is a BCR/TCR annotation field, chain for which annotation will be retrieved.
+#         Options are ``'heavy'``, ``'light'``, ``'kappa'``, ``'lambda'``, ``'alpha'``,
+#         ``'beta'``, ``'delta'`` or ``'gamma'``.
 
-#     plot_kwargs : dict, optional  
+#     plot_kwargs : dict, optional
 #         Dictionary containing keyword arguments that will be passed to ``pyplot.bar()``.
 
-#     legend_kwargs : dict, optional  
+#     legend_kwargs : dict, optional
 #         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
 
-#     hide_legend : bool, default=False  
-#         By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-#         the legend will not be shown.  
-        
-#     xlabel : str, optional  
-#         Text for the X-axis label. 
-
-#     ylabel : str, optional  
-#         Text for the Y-axis label.  
-        
-#     xlabel_fontsize : int or float, default=16  
+#     hide_legend : bool, default=False
+#         By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+#         the legend will not be shown.
+
+#     xlabel : str, optional
+#         Text for the X-axis label.
+
+#     ylabel : str, optional
+#         Text for the Y-axis label.
+
+#     xlabel_fontsize : int or float, default=16
 #         Fontsize for the X-axis label text.
 
-#     ylabel_fontsize : int or float, default=16  
+#     ylabel_fontsize : int or float, default=16
 #         Fontsize for the Y-axis label text.
 
-#     xtick_labelsize : int or float, default=14  
-#         Fontsize for the X-axis tick labels.  
+#     xtick_labelsize : int or float, default=14
+#         Fontsize for the X-axis tick labels.
+
+#     ytick_labelsize : int or float, default=14
+#         Fontsize for the Y-axis tick labels.
 
-#     ytick_labelsize : int or float, default=14  
-#         Fontsize for the Y-axis tick labels.  
+#     xtick_labelrotation : int or float, default=0
+#         Rotation of the X-axis tick labels.
 
-#     xtick_labelrotation : int or float, default=0  
-#         Rotation of the X-axis tick labels.  
-    
-#     ytick_labelrotation : int or float, default=0  
-#         Rotation of the Y-axis tick labels. 
+#     ytick_labelrotation : int or float, default=0
+#         Rotation of the Y-axis tick labels.
 
-#     show :bool, default=False  
+#     show :bool, default=False
 #         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
 #         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
 
-#     figsize : iterable object, default=[6, 4]  
-#         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches. 
+#     figsize : iterable object, default=[6, 4]
+#         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
 
-#     figfile : str, optional  
+#     figfile : str, optional
 #         Path at which to save the figure file. If not provided, the figure is not saved
-#         and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.  
+#         and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
 #     '''
 #     # process input data
 #     if order is None:
 #         x_vals = natsorted(set(get_adata_values(adata, x, receptor=receptor, chain=chain)))
 #     else:
 #         x_vals = order
-    
+
 #     # process hue, if provided
 #     if hue is not None:
 #         hue_vals = get_adata_values(adata, hue, receptor=receptor, chain=chain)
 #         hue_order = (
 #             hue_order
 #             if hue_order is not None
 #             else natsorted(set(hue_vals))
@@ -2356,15 +2377,15 @@
 #     else:
 #         hue_order = [
 #             None,
 #         ]
 #         hue_batches = [
 #             adata,
 #         ]
-        
+
 #     # process batches
 #     batch_data = []
 #     for batch in hue_batches:
 #         y_dict = Counter(get_adata_values(batch, x, chain=chain, receptor=receptor))
 #         batch_data.append(y_dict)
 #     if normalize:
 #         if len(batch_data) > 1:
@@ -2375,15 +2396,15 @@
 #                     y_dict[xval] = yval / ytots[xval]
 #         else:
 #             for ydict in batch_data:
 #                 tot = sum(ydict.values())
 #                 for xval in x_vals:
 #                     yval = y_dict.get(xval, 0)
 #                     y_dict[xval] = yval / tot
-        
+
 #     # colors
 #     if palette is None:
 #         if len(hue_batches) > 1:
 #             palette = {h: c for h, c in zip(hue_order, sns.hls_palette(len(hue_order)))}
 #         else:
 #             palette = {}
 #         # palette is a dict assigning colors to x and/or hue categories
@@ -2400,35 +2421,35 @@
 #                     else:
 #                         _colors.append(palette.get(_hue, palette.get(_x, color)))
 #                 else:
 #                     _colors.append(alt_color)
 #             else:
 #                 _colors.append(palette.get(_hue, palette.get(_x, alt_color)))
 #         colors.append(_colors)
-            
+
 #     # plot kwargs
 #     default_plot_kwargs = {"width": 0.8, "linewidth": 1.5, "edgecolor": "w"}
 #     if plot_kwargs is not None:
 #         default_plot_kwargs.update(plot_kwargs)
 #     plot_kwargs = default_plot_kwargs
 
 #     # legend kwargs
 #     default_legend_kwargs = {"frameon": True, "loc": "best", "fontsize": 12}
 #     if legend_kwargs is not None:
 #         default_legend_kwargs.update(legend_kwargs)
 #     legend_kwargs = default_legend_kwargs
-    
+
 #     # make the plot
 #     plt.figure(figsize=figsize)
 #     bottom = np.zeros(len(x_vals))
 #     for h, d, c in zip(hue_order, batch_data, colors):
 #         y_vals = np.asarray([d.get(_x, 0) for _x in x_vals])
 #         plt.bar(x_vals, y_vals, bottom=bottom, color=c, label=h, **plot_kwargs)
 #         bottom += y_vals
-        
+
 #     # style the plot
 #     ax = plt.gca()
 #     if ylabel is None:
 #         ylabel = "Frequency (%)" if normalize else "Count"
 #     ax.set_xlabel(xlabel, fontsize=xlabel_fontsize)
 #     ax.set_ylabel(ylabel, fontsize=ylabel_fontsize)
 #     ax.tick_params(
@@ -2451,20 +2472,14 @@
 #         plt.savefig(figfile)
 #     elif show:
 #         plt.show()
 #     else:
 #         return ax
 
 
-
-
-
-
-
-
 # ===========================
 
 #           VDJ
 
 # ===========================
 
 
@@ -2495,104 +2510,104 @@
 ):
     """
     Produces a bar plot of germline gene usage. For datasets containing multiple batches, a stacked
     bar plot can optionally be generated.
 
     Parameters
     ----------
-    adata : anndata.AnnData  
-        An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr`` 
-        or ``adata.obs.tcr`` populated with annotated BCR/TCR information.  
-
-    gene_names : iterable object, optional  
-        A list of germline gene names to be plotted. If not provided, all germline genes 
-        found in the dataset will be shown.  
-
-    chain : str, default='heavy'  
-        Chain for which germline gene usage will be plotted. Options are ``'heavy'``, ``'light'``, 
-        ``'kappa'``, ``'lambda'``, ``'alpha'``, ``'beta'``, ``'delta'`` or ``'gamma'``.  
-
-    receptor : str, default='bcr'  
-        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.  
-
-    germline_key : str, default='v_call'  
-        Annotation key containing the germline gene to be plotted.  
-
-    batch_key : str, optional  
-        Field (found in ``adata.obs``) containing batch names. If provided, batches 
-        will be plotted as stacked bars. If not provided, all of the input data is 
-        assumed to be from a single batch and a standard bar plot is generated. 
-
-    batch_names : iterable object, optional  
-        List of batch names to be plotted. If `bnatch_names` contains a subset of all categories 
-        found in `batch_key`, only the supplied `batch_names` will be plotted.  If not provided, 
+    adata : anndata.AnnData
+        An ``AnnData`` object containing the input data. `adata` must have ``adata.obs.bcr``
+        or ``adata.obs.tcr`` populated with annotated BCR/TCR information.
+
+    gene_names : iterable object, optional
+        A list of germline gene names to be plotted. If not provided, all germline genes
+        found in the dataset will be shown.
+
+    chain : str, default='heavy'
+        Chain for which germline gene usage will be plotted. Options are ``'heavy'``, ``'light'``,
+        ``'kappa'``, ``'lambda'``, ``'alpha'``, ``'beta'``, ``'delta'`` or ``'gamma'``.
+
+    receptor : str, default='bcr'
+        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+    germline_key : str, default='v_call'
+        Annotation key containing the germline gene to be plotted.
+
+    batch_key : str, optional
+        Field (found in ``adata.obs``) containing batch names. If provided, batches
+        will be plotted as stacked bars. If not provided, all of the input data is
+        assumed to be from a single batch and a standard bar plot is generated.
+
+    batch_names : iterable object, optional
+        List of batch names to be plotted. If `bnatch_names` contains a subset of all categories
+        found in `batch_key`, only the supplied `batch_names` will be plotted.  If not provided,
         all batches will be plotted in ``natsort.natsorted()`` order.
 
-    palette : iterable, optional  
+    palette : iterable, optional
         List of batch colors. If none of `palette`, `color` or `germline_colors`
-        are provided, bars are colored by the germline gene family.  
+        are provided, bars are colored by the germline gene family.
 
-    color :str, optional  
-        Single color to be used for all bars in the plot. If none of `palette`, `color` 
-        or `germline_colors` are provided, bars are colored by the germline gene. If provided in 
-        combination with `germline_colors`, `color` will be used as the default color for genes 
-        not found in `germline_colors`. If `germline_colors` is supplied and `color` is not, 
+    color :str, optional
+        Single color to be used for all bars in the plot. If none of `palette`, `color`
+        or `germline_colors` are provided, bars are colored by the germline gene. If provided in
+        combination with `germline_colors`, `color` will be used as the default color for genes
+        not found in `germline_colors`. If `germline_colors` is supplied and `color` is not,
         `color` will default to ``'#D3D3D3'``.
 
-    germline_colors : dict, optional  
+    germline_colors : dict, optional
         Dictionary mapping germline genes to colors. Particularly useful when
-        highlighting one or more germline genes is desired. Germline genes not found as keys in 
+        highlighting one or more germline genes is desired. Germline genes not found as keys in
         `germline_colors` will be colored using `color` (or ``'#D3D3D3'`` if 'color` is not
-        provided).  
+        provided).
 
-    pairs_only : bool, default=False  
+    pairs_only : bool, default=False
         If ``True``, only sequences for which a heavy/light pair is present will be
-        plotted.  
+        plotted.
 
-    normalize : bool, default=False  
-        If ``True``, normalized frequencies are plotted instead of sequence counts. Note that 
+    normalize : bool, default=False
+        If ``True``, normalized frequencies are plotted instead of sequence counts. Note that
         normalization is performed separately for each batch, so the total frequency may exceed ``1.0``.
 
-    plot_kwargs : dict, optional  
+    plot_kwargs : dict, optional
         Dictionary containing keyword arguments that will be passed to ``pyplot.bar()``.
 
-    legend_kwargs : dict, optional  
+    legend_kwargs : dict, optional
         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
 
-    hide_legend : bool, default=False  
-        By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-        the legend will not be shown.  
+    hide_legend : bool, default=False
+        By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+        the legend will not be shown.
 
-    ylabel : str, optional  
-        Text for the Y-axis label.  
+    ylabel : str, optional
+        Text for the Y-axis label.
 
-    ylabel_fontsize : int or float, default=16  
+    ylabel_fontsize : int or float, default=16
         Fontsize for the Y-axis label text.
 
-    xtick_labelsize : int or float, default=14  
-        Fontsize for the X-axis tick labels.  
+    xtick_labelsize : int or float, default=14
+        Fontsize for the X-axis tick labels.
 
-    ytick_labelsize : int or float, default=14  
-        Fontsize for the Y-axis tick labels.  
+    ytick_labelsize : int or float, default=14
+        Fontsize for the Y-axis tick labels.
 
-    xtick_labelrotation : int or float, default=90  
-        Rotation of the X-axis tick labels.  
+    xtick_labelrotation : int or float, default=90
+        Rotation of the X-axis tick labels.
 
-    show :bool, default=False  
+    show :bool, default=False
         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
 
-    figsize : iterable object, optional  
+    figsize : iterable object, optional
         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
         If not provided, the figure size will be determined based on the number of germline genes
         found in the data.
 
-    figfile : str, optional  
+    figfile : str, optional
         Path at which to save the figure file. If not provided, the figure is not saved
-        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.  
+        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
 
     """
     # split input into batches
     if batch_key is not None:
         batch_names = (
             batch_names
             if batch_names is not None
@@ -2735,103 +2750,103 @@
     """
     Produces a bar plot of CDR3 length frequency. For datasets containing multiple batches, a stacked
     bar plot can optionally be generated.
 
     Parameters
     ----------
 
-    adata : anndata.AnnData  
+    adata : anndata.AnnData
         An ``AnnData`` object containing the input data. ``adata`` must have
         ``adata.obs[receptor]`` populated with annotated VDJ information. Required.
 
-    lengths : iterable object, optional  
-        A list of CDR3 lengths to be plotted. If not provided, all lengths found in the 
+    lengths : iterable object, optional
+        A list of CDR3 lengths to be plotted. If not provided, all lengths found in the
         dataset will be shown.
 
-    chain : str, default='heavy'  
-        Chain for which germline gene usage will be plotted. Options are ``'heavy'``, ``'light'``, 
-        ``'kappa'``, ``'lambda'``, ``'alpha'``, ``'beta'``, ``'delta'`` or ``'gamma'``.  
-
-    receptor : str, default='bcr'  
-        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``. 
-
-    cdr3_length_key : str, default='cdr3_length'  
-        Field containing the CDR3 length data to be plotted.  
-
-    batch_key : str, optional  
-        Field (found in ``adata.obs``) containing batch names. If provided, batches 
-        will be plotted as stacked bars. If not provided, all of the input data is 
-        assumed to be from a single batch and a standard bar plot is generated. 
-
-    batch_names : iterable object, optional  
-        List of batch names to be plotted. If `batch_names` contains a subset of all categories 
-        found in `batch_key`, only the supplied `batch_names` will be plotted.  If not provided, 
+    chain : str, default='heavy'
+        Chain for which germline gene usage will be plotted. Options are ``'heavy'``, ``'light'``,
+        ``'kappa'``, ``'lambda'``, ``'alpha'``, ``'beta'``, ``'delta'`` or ``'gamma'``.
+
+    receptor : str, default='bcr'
+        Receptor for which data should be plotted. Options are ``'bcr'`` and ``'tcr'``.
+
+    cdr3_length_key : str, default='cdr3_length'
+        Field containing the CDR3 length data to be plotted.
+
+    batch_key : str, optional
+        Field (found in ``adata.obs``) containing batch names. If provided, batches
+        will be plotted as stacked bars. If not provided, all of the input data is
+        assumed to be from a single batch and a standard bar plot is generated.
+
+    batch_names : iterable object, optional
+        List of batch names to be plotted. If `batch_names` contains a subset of all categories
+        found in `batch_key`, only the supplied `batch_names` will be plotted.  If not provided,
         all batches will be plotted in ``natsort.natsorted()`` order.
 
-    palette : iterable, optional  
+    palette : iterable, optional
         List of batch colors. If none of `palette`, `color` or `length_colors`
-        are provided, bars are colored by the germline gene family.  
+        are provided, bars are colored by the germline gene family.
 
-    color :str, optional  
-        Single color to be used for all bars in the plot. If none of `palette`, `color` 
-        or `length_colors` are provided, bars are colored by the germline gene. If provided in 
-        combination with `length_colors`, `color` will be used as the default color for genes 
-        not found in `length_colors`. If `length_colors` is supplied and `color` is not, 
+    color :str, optional
+        Single color to be used for all bars in the plot. If none of `palette`, `color`
+        or `length_colors` are provided, bars are colored by the germline gene. If provided in
+        combination with `length_colors`, `color` will be used as the default color for genes
+        not found in `length_colors`. If `length_colors` is supplied and `color` is not,
         `color` will default to ``'#D3D3D3'``.
 
-    length_colors : dict, optional  
+    length_colors : dict, optional
         Dictionary mapping CDR3 lengths to colors. Particularly useful when
-        highlighting one or more CDR3 lengths is desired. Any CDR3 lengths not found as keys in 
+        highlighting one or more CDR3 lengths is desired. Any CDR3 lengths not found as keys in
         `length_colors` will be colored using `color`.
 
-    pairs_only : bool, default=False  
+    pairs_only : bool, default=False
         If ``True``, only sequences for which a heavy/light pair is present will be
-        plotted.  
+        plotted.
 
-    normalize : bool, default=False  
-        If ``True``, normalized frequencies are plotted instead of sequence counts. Note that 
+    normalize : bool, default=False
+        If ``True``, normalized frequencies are plotted instead of sequence counts. Note that
         normalization is performed separately for each batch, so the total frequency may exceed ``1.0``.
 
-    plot_kwargs : dict, optional  
+    plot_kwargs : dict, optional
         Dictionary containing keyword arguments that will be passed to ``pyplot.bar()``.
 
-    legend_kwargs : dict, optional  
+    legend_kwargs : dict, optional
         Dictionary containing keyword arguments that will be passed to ``ax.legend()``.
 
-    hide_legend : bool, default=False  
-        By default, a plot legend will be shown if multiple batches are plotted. If ``True``, 
-        the legend will not be shown.  
+    hide_legend : bool, default=False
+        By default, a plot legend will be shown if multiple batches are plotted. If ``True``,
+        the legend will not be shown.
 
-    xlabel : str, optional  
-        Text for the X-axis label.  
+    xlabel : str, optional
+        Text for the X-axis label.
 
-    ylabel : str, optional  
-        Text for the Y-axis label.  
+    ylabel : str, optional
+        Text for the Y-axis label.
 
-    ylabel_fontsize : int or float, default=16  
+    ylabel_fontsize : int or float, default=16
         Fontsize for the Y-axis label text.
 
-    xtick_labelsize : int or float, default=14  
-        Fontsize for the X-axis tick labels.  
+    xtick_labelsize : int or float, default=14
+        Fontsize for the X-axis tick labels.
 
-    ytick_labelsize : int or float, default=14  
-        Fontsize for the Y-axis tick labels.  
+    ytick_labelsize : int or float, default=14
+        Fontsize for the Y-axis tick labels.
 
-    show :bool, default=False  
+    show :bool, default=False
         If ``True``, plot is shown and the plot ``Axes`` object is not returned. Default
         is ``False``, which does not call ``pyplot.show()`` and returns the ``Axes`` object.
 
-    figsize : iterable object, optional  
+    figsize : iterable object, optional
         List containing the figure size (as ``[x-dimension, y-dimension]``) in inches.
         If not provided, the figure size will be determined based on the number of germline genes
         found in the data.
 
-    figfile : str, optional  
+    figfile : str, optional
         Path at which to save the figure file. If not provided, the figure is not saved
-        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned. 
+        and is either shown (if `show` is ``True``) or the ``Axes`` object is returned.
 
     """
     # split input into batches
     if batch_key is not None:
         batch_names = (
             batch_names
             if batch_names is not None
@@ -2971,128 +2986,128 @@
     text_kws={},
     pie_kws={},
 ):
     """
     Creates a donut plot of a population of lineages, with arc widths proportional to lineage size.
 
     .. note::
-       For **continuous** hues (for example, AgBC UMI counts), the mean value for each lineage is used. 
+       For **continuous** hues (for example, AgBC UMI counts), the mean value for each lineage is used.
        For **boolean** hues (for example, specificity classifications), the lineage is considered ``True`` if
        any lineage member is ``True``. For **categorical** hues (for example, CDR3 length), the most common
-       value for each lineage is used. 
-    
+       value for each lineage is used.
+
     Parameters
     ----------
-    
-    adata : anndata.AnnData  
-        Input ``AnnData`` object. ``adata.obs`` must contain a column for the 
+
+    adata : anndata.AnnData
+        Input ``AnnData`` object. ``adata.obs`` must contain a column for the
         lineage name (`lineage_key`) and, optionally, a `hue` column.
-            
-    hue : str or dict, optional  
+
+    hue : str or dict, optional
         Can be either the name of a column in ``adata.obs`` or a ``dict`` mapping
-        lineage names to hue values. Used to determine the color of each lineage arc. If a ``dict`` 
-        is provided, any missing lineage names will still be included in the donut plot but will 
-        be colored using `alt_color`. There are three possible classes of hue values:  
-             
-                - **continuous:** hues that map to a continuous numerical space, identified by all `hue` 
+        lineage names to hue values. Used to determine the color of each lineage arc. If a ``dict``
+        is provided, any missing lineage names will still be included in the donut plot but will
+        be colored using `alt_color`. There are three possible classes of hue values:
+
+                - **continuous:** hues that map to a continuous numerical space, identified by all `hue`
                   values being floating point numbers. An example would be log2-transformed
                   antigen barcode UMI counts. For continuous hues, the mean of all members
-                  in a lineage will be plotted.  
-                  
+                  in a lineage will be plotted.
+
                 - **boolean:** hues that map to either ``True`` or ``False``. An example would be specificity
                   classification. For boolean hues, if any member of a lineage is ``True``, the
-                  entire lineage will be considered ``True``.  
-                  
-                - **categorical:** hues that map to one of a set of categories. An example would be isotypes. 
-                  For categorical hues, the most common value observed in a lineage will 
-                  be plotted.  
-                  
+                  entire lineage will be considered ``True``.
+
+                - **categorical:** hues that map to one of a set of categories. An example would be isotypes.
+                  For categorical hues, the most common value observed in a lineage will
+                  be plotted.
+
         Finally, if `hue` is not provided, the lineage name will be considered the `hue`, and
         each lineage will be colored separately.
-            
-    palette : dict, optional  
+
+    palette : dict, optional
         A ``dict`` mapping hue categories to colors. For boolean hue types, if `palette`
-        is not provided, `color` will be used for ``True`` and `alt_color` will be used for 
-        ``False``. For categorical hue types, if `color` is provided, a monochromatic palette 
+        is not provided, `color` will be used for ``True`` and `alt_color` will be used for
+        ``False``. For categorical hue types, if `color` is provided, a monochromatic palette
         consisting of various shades of `color` will be used. If `color` is not provided,
-        ``sns.hls_palette()`` will be used to generate a color palette.  
-            
-    color : str or list, optional  
+        ``sns.hls_palette()`` will be used to generate a color palette.
+
+    color : str or list, optional
         A color name, hex string or RGB list/tuple for coloring the donut plot. For
-        boolean hue types, `color` will be used for ``True`` and 'alt_color' will be used for 
-        ``False``. For categorical and continuous hue types, a monochromatic palette will 
-        be created containing various shades of `color`.  
-            
-    alt_color : str or list, default='#F5F5F5'    
-        A color name, hex string or RGB list/tuple for coloring alternate values 
+        boolean hue types, `color` will be used for ``True`` and 'alt_color' will be used for
+        ``False``. For categorical and continuous hue types, a monochromatic palette will
+        be created containing various shades of `color`.
+
+    alt_color : str or list, default='#F5F5F5'
+        A color name, hex string or RGB list/tuple for coloring alternate values
         (``False`` boolean hues or values not found in `palette`). Default is ``'#F5F5F5'``, which is
         a very light grey.
-        
-    singleton_color : str or list, default='lightgrey'  
-        A color name, hex string or RGB list/tuple for coloring the singleton arc in the donut plot.  
-            
-    shuffle_colors : bool, default=False  
+
+    singleton_color : str or list, default='lightgrey'
+        A color name, hex string or RGB list/tuple for coloring the singleton arc in the donut plot.
+
+    shuffle_colors : bool, default=False
         If ``True``, colors will be shuffled prior to assignment to hue categories. This
-        is primarily useful when the `hue` is the lineage name and a monochromatic palette is used,  
-        in order to make it easier to distinguish neighboring arcs on the plot.  
-            
-    name : str, optional  
+        is primarily useful when the `hue` is the lineage name and a monochromatic palette is used,
+        in order to make it easier to distinguish neighboring arcs on the plot.
+
+    name : str, optional
         Not currently used.
-        
-    hue_order : list, optional  
-        A list specifying the hue category order. This does not affect the ordering 
+
+    hue_order : list, optional
+        A list specifying the hue category order. This does not affect the ordering
         of lineages in the donut plot, just the assignment of colors to `hue` categories. For example,
         when plotting with a monochromatic palette (by providing `color`), `hue_order` will
         order the coloring of `hue` categories from dark to light.
-            
-    force_categorical_hue : bool, default=False  
-        By default, any `hue` categories consisting solely of ``float`` values 
-        will be considered continuous and will be colored using a user-supplied colormap (`cmap`) or 
+
+    force_categorical_hue : bool, default=False
+        By default, any `hue` categories consisting solely of ``float`` values
+        will be considered continuous and will be colored using a user-supplied colormap (`cmap`) or
         with a monochromatic color gradient (using `color` as the base color). If ``True``, `hue`
         categories will always be considered categorical.
-            
-    lineage_key : str, default='lineage'  
-        Column in ``adata.obs`` corresponding to the lineage name.  
-            
-    figfile : str, optional  
+
+    lineage_key : str, default='lineage'
+        Column in ``adata.obs`` corresponding to the lineage name.
+
+    figfile : str, optional
         Path to an output figure file. If not provided, the figure will be shown and not saved to file.
-            
-    figsize : iterable object, default=[6, 6]  
-        Figure size, in inches.  
-        
-    pairs_only : bool, default=False  
+
+    figsize : iterable object, default=[6, 6]
+        Figure size, in inches.
+
+    pairs_only : bool, default=False
         If ``True``, only paired BCR/TCR sequences (containing both heavy/light, alpha/beta or
-        delta/gamma chains) will be included.  
-            
-    edgecolor : str or list, default='white'  
-        A color name, hex string or RGB list/tuple for coloring the edges that divide donut arcs.  
-            
-    random_seed : int, float or str, default=1234  
-        Used to set the random seed using ``numpy.random.seed()``. Only applicable when 
+        delta/gamma chains) will be included.
+
+    edgecolor : str or list, default='white'
+        A color name, hex string or RGB list/tuple for coloring the edges that divide donut arcs.
+
+    random_seed : int, float or str, default=1234
+        Used to set the random seed using ``numpy.random.seed()``. Only applicable when
         `shuffle_colors` is ``True``, and provided mainly to allow users to recreate plots
         that use shuffled colors (otherwise the shuffle order would be random, thus creating
         a different color order each time the plotting function is called). Default is ``1234``.
-            
-    width : float, default=0.55  
-        Fraction of the donut plot radius that corresponds to the donut 'hole'.  
-            
-    fontsize : int or float, default=28  
-        Fontsize for the sequence count text displayed in the center of the plot.  
-            
-    linewidth : int or float, default=2  
-        Width of the lines separating lineage arcs.  
-        
-    pie_kws : dict, optional  
+
+    width : float, default=0.55
+        Fraction of the donut plot radius that corresponds to the donut 'hole'.
+
+    fontsize : int or float, default=28
+        Fontsize for the sequence count text displayed in the center of the plot.
+
+    linewidth : int or float, default=2
+        Width of the lines separating lineage arcs.
+
+    pie_kws : dict, optional
         Dictionary containing keyword arguments that will be passed directly to ``ax.pie()``.
-            
-    text_kws : dict, optional  
-        Dictionary containing keyword arguments that will be passed directly to ``ax.text()`` 
+
+    text_kws : dict, optional
+        Dictionary containing keyword arguments that will be passed directly to ``ax.text()``
         when drawing the text in the center of the plot.
-        
-    
+
+
     """
     adata = adata.copy()
     if pairs_only:
         adata = adata[[b.is_pair for b in adata.obs.bcr]]
 
     # organize linages into a DataFrame
     ldata = []
@@ -3193,15 +3208,15 @@
             else:
                 hue_order = (
                     hue_order
                     if hue_order is not None
                     else natsorted(df["hue"].dropna().unique())
                 )
             if color is not None:
-                colors = _get_monochrome_colors(color, len(hue_order))
+                colors = abutils.color.monochrome_palette(color, len(hue_order))
                 if shuffle_colors:
                     primary = colors[0]
                     secondary = colors[1:]
                     np.random.seed(random_seed)
                     np.random.shuffle(secondary)
                     colors = [primary] + secondary
             else:
@@ -3235,32 +3250,25 @@
 
     if figfile is not None:
         plt.savefig(figfile)
     else:
         plt.show()
 
 
-def _get_monochrome_colors(monochrome_color, n_col):
-    cmap = get_cmap(from_color=monochrome_color)
-    # this is a bit convoluted, but what's happening is we're getting different colormap
-    # values -- which range from 1 (darkest) to 0 (lightest). Calling cmap(i) returns an 
-    # rgba tuple, but we just need the rbg, so we drop the a. To make sure that one of 
-    # the colors isn't pure white, we ask np.linspace() for one more value than we need 
-    # and drop the lightest value
-    RGB_tuples = [cmap(i)[:-1] for i in np.linspace(1, 0, n_col + 1)][:-1]
-    return RGB_tuples
-
-
-
-def get_loupe_cmap():
-    ylorbr = mpl.cm.get_cmap("YlOrBr").copy()
-    cropped_ylorbr = ylorbr(np.linspace(0.1, 1, 255))
-    loupe_colors = [np.array([0.9, 0.9, 0.9, 1.0])] + list(cropped_ylorbr)
-
-    return mpl.colors.LinearSegmentedColormap.from_list('loupe', loupe_colors)
-
-loupe_cmap = get_loupe_cmap()
-
+# def _get_monochrome_colors(monochrome_color, n_col):
+#     cmap = get_cmap(from_color=monochrome_color)
+#     # this is a bit convoluted, but what's happening is we're getting different colormap
+#     # values -- which range from 1 (darkest) to 0 (lightest). Calling cmap(i) returns an
+#     # rgba tuple, but we just need the rbg, so we drop the a. To make sure that one of
+#     # the colors isn't pure white, we ask np.linspace() for one more value than we need
+#     # and drop the lightest value
+#     RGB_tuples = [cmap(i)[:-1] for i in np.linspace(1, 0, n_col + 1)][:-1]
+#     return RGB_tuples
 
 
+loupe_cmap = abutils.color.get_cmap(
+    "YlOrBr", zero_color=[0.9, 0.9, 0.9, 1.0], minval=0.1
+)
 
 
+def get_loupe_cmap():
+    return loupe_cmap
```

### Comparing `scab-0.0.6/scab/pp.py` & `scab-0.1.0/scab/pp.py`

 * *Files identical despite different names*

### Comparing `scab-0.0.6/scab/tl.py` & `scab-0.1.0/scab/tl.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,321 +19,507 @@
 # BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 import os
-import sys
 import re
+import sys
+from typing import Optional, Union
 
 from natsort import natsorted
 
 import numpy as np
 import pandas as pd
 
 import matplotlib.pyplot as plt
 
 import scanpy as sc
 
+import anndata
+
 from sklearn.neighbors import KernelDensity
 
 from scipy import stats
 from scipy.signal import argrelextrema
 
 # from scipy.stats import scoreatpercentile
 
 import statsmodels.api as sm
 
 from .io import read_10x_mtx
+from .tools.batch_correction import combat, mnn, scanorama
+from .tools.embeddings import umap, pca, dimensionality_reduction
 
 
-def dimensionality_reduction(
-    adata,
-    solver="arpack",
-    n_neighbors=20,
-    n_pcs=40,
-    ignore_ig=True,
-    paga=True,
-    use_rna_velocity=False,
-    use_rep=None,
-    random_state=None,
-    resolution=1.0,
-    verbose=True,
-):
-    """
-    Performs PCA, neighborhood graph construction and UMAP embedding. 
-    PAGA is optional, but is performed by default.  
-
-    Parameters
-    ----------
-
-    adata : anndata.AnnData)
-        ``AnnData`` object containing gene counts data.  
-
-    solver : str, default='arpack'  
-        Solver to use for the PCA.  
-
-    n_neighbors : int, default=10
-        Number of neighbors to calculate for the neighbor graph.  
-
-    n_pcs : int, default=40  
-        Number of principal components to use when computing the neighbor graph.
-        Although the default value is generally appropriate, it is sometimes useful
-        to empirically determine the optimal value for `n_pcs`.
-
-    paga : bool, default=True  
-        If ``True``, performs partition-based graph abstraction (PAGA_) prior to 
-        UMAP embedding.  
-
-    use_rna_velocity : bool, default=False  
-        If ``True``, uses RNA velocity information to compute PAGA. If ``False``, 
-        this option is ignored.  
-
-    use_rep : str, optional  
-        Representation to use when `computing neighbors`_. For example, if data have 
-        been batch normalized with ``scanorama``, the representation
-        should be ``'Scanorama'``. If not provided, ``scanpy``'s default 
-        representation is used.
-
-    random_state : int, optional  
-        Seed for the random state used by ``sc.tl.umap``.  
-
-    resolution : float, default=1.0  
-        Resolution for Leiden clustering.  
-
-    
-    Returns
-    -------
-    adata : ``anndata.AnnData``
-
-
-    .. _PAGA: 
-        https://github.com/theislab/paga  
-    .. _computing neighbors: 
-        https://scanpy.readthedocs.io/en/stable/generated/scanpy.pp.neighbors.html
-
-    """
-    if verbose:
-        print("performing PCA...")
-    if ignore_ig:
-        _adata = adata.copy()
-        _adata.var['highly_variable'] = _adata.var['highly_variable'] & ~(_adata.var['ig'])
-        sc.tl.pca(_adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
-        adata.obsm['X_pca'] = _adata.obsm['X_pca']
-        adata.varm['PCs'] = _adata.varm['PCs']
-        adata.uns['pca'] = {'variance_ratio': _adata.uns['pca']['variance_ratio'],
-                            'variance': _adata.uns['pca']['variance']}
-    else:
-        sc.tl.pca(adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
-    if verbose:
-        print("calculating neighbors...")
-    sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, use_rep=use_rep)
-    if verbose:
-        print("leiden clustering...")
-    sc.tl.leiden(adata, resolution=resolution)
-    if paga:
-        if verbose:
-            print("paga...")
-        #         solid_edges = 'transitions_confidence' if use_rna_velocity else 'connectivities'
-        sc.tl.paga(adata, use_rna_velocity=use_rna_velocity)
-        if use_rna_velocity:
-            adata.uns["paga"]["connectivities"] = adata.uns["paga"][
-                "transitions_confidence"
-            ]
-        sc.pl.paga(adata, plot=False)
-        if verbose:
-            print("umap...")
-        sc.tl.umap(
-            adata, init_pos="paga", random_state=random_state,
-        )
-    else:
-        if verbose:
-            print("umap...")
-        sc.tl.umap(adata, random_state=random_state)
-    return adata
-
-
-def combat(adata, batch_key="batch", covariates=None, dim_red=True):
-    """
-    Batch effect correction using ComBat_ [Johnson07]_.  
-
-    .. seealso::
-        | W. Evan Johnson, Cheng Li, Ariel Rabinovic
-        | Adjusting batch effects in microarray expression data using empirical Bayes methods
-        | *Biostatistics* 2007, doi: 10.1093/biostatistics/kxj037
-
-
-    Parameters
-    ----------
-
-    adata : anndata.AnnData
-        ``AnnData`` object containing gene counts data.
-
-    batch_key : str, default='batch'  
-        Name of the column in adata.obs that corresponds to the batch.  
-
-    covariates : iterable object, optional  
-        List of additional covariates besides the batch variable such as adjustment variables 
-        or biological condition. Not including covariates may lead to the removal of real
-        biological signal.  
-
-    dim_red : bool, default=True  
-        If ``True``, dimentionality reduction will be performed on the post-integration data using 
-        ``scab.tl.dimensionality_reduction()``.  
-
-    Returns
-    -------
-    adata : ``anndata.AnnData``
-
-
-    .. _ComBat: 
-        https://github.com/brentp/combat.py
-
-    """
-    adata_combat = sc.AnnData(X=adata.raw.X, var=adata.raw.var, obs=adata.obs)
-    adata_combat.layers = adata.layers
-    adata_combat.raw = adata_combat
-    # run combat
-    sc.pp.combat(adata_combat, key=batch_key, covariates=covariates)
-    sc.pp.highly_variable_genes(adata_combat)
-    if dim_red:
-        adata_combat = dimensionality_reduction(adata_combat)
-    return adata_combat
-
-
-def mnn(adata, batch_key="batch", min_hvg_batches=1, dim_red=True):
-    """
-    Data integration and batch correction using `mutual nearest neighbors`_ [Haghverdi19]_. Uses the 
-    ``scanpy.external.pp.mnn_correct()`` function.
-
-    .. seealso::
-        | Laleh Haghverdi, Aaron T L Lun, Michael D Morgan & John C Marioni
-        | Batch effects in single-cell RNA-sequencing data are corrected by matching mutual nearest neighbors
-        | *Nature Biotechnology* 2019, doi: 10.1038/nbt.4091
-
-    Parameters
-    ----------
-    adata : anndata.AnnData  
-        ``AnnData`` object containing gene counts data.
-
-    batch_key : str, default='batch'  
-        Name of the column in adata.obs that corresponds to the batch.  
-
-    min_hvg_batches : int, default=1  
-        Minimum number of batches in which highly variable genes are found in order to be included
-        in the list of genes used for batch correction. Default is ``1``, which results in the use 
-        of all HVGs found in any batch.
-        
-    dim_red : bool, default=True  
-        If ``True``, dimentionality reduction will be performed on the post-integration data using 
-        ``scab.tl.dimensionality_reduction()``.  
-
-
-    Returns
-    -------
-    adata : ``anndata.AnnData``
-
-
-    .. _mutual nearest neighbors:
-        https://github.com/chriscainx/mnnpy
-
-    """
-    adata_mnn = adata.raw.to_adata()
-    adata_mnn.layers = adata.layers
-    # variable genes
-    sc.pp.highly_variable_genes(
-        adata_mnn, min_mean=0.0125, max_mean=3, min_disp=0.5, batch_key=batch_key
-    )
-    var_select = adata_mnn.var.highly_variable_nbatches >= min_hvg_batches
-    var_genes = var_select.index[var_select]
-    # split per batch into new objects.
-    batches = adata_mnn.obs[batch_key].cat.categories.tolist()
-    alldata = {}
-    for batch in batches:
-        alldata[batch] = adata_mnn[
-            adata_mnn.obs[batch_key] == batch,
-        ]
-    # run MNN correction
-    cdata = sc.external.pp.mnn_correct(
-        *[alldata[b] for b in batches],
-        svd_dim=50,
-        batch_key=batch_key,
-        save_raw=True,
-        var_subset=var_genes,
-    )
-    corr_data = cdata[0][:, var_genes]
-    if dim_red:
-        corr_data = dimensionality_reduction(corr_data)
-    return corr_data
-
-
-def scanorama(adata, batch_key="batch", dim_red=True):
-    """
-    Batch correction using Scanorama_ [Hie19]_. 
-
-    .. seealso::
-        | Brian Hie, Bryan Bryson, and Bonnie Berger 
-        | Efficient integration of heterogeneous single-cell transcriptomes using Scanorama 
-        | *Nature Biotechnology* 2019, doi: 10.1038/s41587-019-0113-3
-
-    Parameters
-    ----------
-
-    adata : anndata.AnnData  
-        ``AnnData`` object containing gene counts data.
-
-    batch_key : str, default='batch'  
-        Name of the column in ``adata.obs`` that corresponds to the batch.  
-
-    dim_red : bool, default=True  
-        If ``True``, dimentionality reduction will be performed on the post-integration data using 
-        ``scab.tl.dimensionality_reduction``.  
-
-
-    Returns
-    -------
-    adata : ``anndata.AnnData``
-
-
-    .. _Scanorama: 
-        https://github.com/brianhie/scanorama
-    
-    """
-    import scanorama
-
-    adata_scanorama = adata.raw.to_adata()
-    adata_scanorama.layers = adata.layers
-    # split per batch into new objects.
-    batches = adata_scanorama.obs[batch_key].cat.categories.tolist()
-    alldata = {}
-    for batch in batches:
-        alldata[batch] = adata_scanorama[
-            adata_scanorama.obs[batch_key] == batch,
-        ]
-    adatas = [alldata[s] for s in alldata.keys()]
-    # run scanorama
-    scanorama.integrate_scanpy(adatas, dimred=50)
-    scanorama_int = [ad.obsm["X_scanorama"] for ad in adatas]
-    all_s = np.concatenate(scanorama_int)
-    adata_scanorama.obsm["Scanorama"] = all_s
-    if dim_red:
-        adata_scanorama = dimensionality_reduction(adata_scanorama, use_rep="Scanorama")
-    return adata_scanorama
+# def pca(
+#     adata: anndata.AnnData,
+#     solver: str = "arpack",
+#     n_pcs: int = 40,
+#     ignore_ig: bool = True,
+#     verbose: bool = True,
+# ) -> anndata.AnnData:
+#     """
+#     Performs PCA, neighborhood graph construction and UMAP embedding.
+#     PAGA is optional, but is performed by default.
+
+#     Parameters
+#     ----------
+
+#     adata : anndata.AnnData
+#         ``AnnData`` object containing gene counts data.
+
+#     solver : str, default='arpack'
+#         Solver to use for the PCA.
+
+#     n_pcs : int, default=40
+#         Number of principal components to use when computing the neighbor graph.
+#         Although the default value is generally appropriate, it is sometimes useful
+#         to empirically determine the optimal value for `n_pcs`.
+
+#     ignore_ig : bool, default=True
+#         Ignores immunoglobulin V, D and J genes when computing the PCA.
+
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _PAGA:
+#         https://github.com/theislab/paga
+#     .. _computing neighbors:
+#         https://scanpy.readthedocs.io/en/stable/generated/scanpy.pp.neighbors.html
+
+#     """
+#     if verbose:
+#         print("performing PCA...")
+#     if ignore_ig:
+#         _adata = adata.copy()
+#         _adata.var["highly_variable"] = _adata.var["highly_variable"] & ~(
+#             _adata.var["ig"]
+#         )
+#         sc.tl.pca(_adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
+#         adata.obsm["X_pca"] = _adata.obsm["X_pca"]
+#         adata.varm["PCs"] = _adata.varm["PCs"]
+#         adata.uns["pca"] = {
+#             "variance_ratio": _adata.uns["pca"]["variance_ratio"],
+#             "variance": _adata.uns["pca"]["variance"],
+#         }
+#     else:
+#         sc.tl.pca(adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
+#     return adata
+
+
+# def umap(
+#     adata: anndata.AnnData,
+#     solver: str = "arpack",
+#     n_neighbors: int = 20,
+#     n_pcs: int = 40,
+#     force_pca: bool = False,
+#     ignore_ig: bool = True,
+#     paga: bool = True,
+#     use_rna_velocity: bool = False,
+#     use_rep: Optional[str] = None,
+#     random_state: Union[int, float, str] = 42,
+#     resolution: float = 1.0,
+#     verbose: bool = True,
+# ) -> anndata.AnnData:
+#     """
+#     Performs PCA, neighborhood graph construction and UMAP embedding.
+#     PAGA is optional, but is performed by default.
+
+#     Parameters
+#     ----------
+
+#     adata : anndata.AnnData
+#         ``AnnData`` object containing gene counts data.
+
+#     solver : str, default='arpack'
+#         Solver to use for the PCA.
+
+#     n_neighbors : int, default=10
+#         Number of neighbors to calculate for the neighbor graph.
+
+#     n_pcs : int, default=40
+#         Number of principal components to use when computing the neighbor graph.
+#         Although the default value is generally appropriate, it is sometimes useful
+#         to empirically determine the optimal value for `n_pcs`.
+
+#     force_pca : bool, default=False
+#         Construct the PCA even if it has already been constructed (``"X_pcs"`` exists
+#         in ``adata.obsm``). Default is ``False``, which will use an existing PCA.
+
+#     ignore_ig : bool, default=True
+#         Ignores immunoglobulin V, D and J genes when computing the PCA.
+
+#     paga : bool, default=True
+#         If ``True``, performs partition-based graph abstraction (PAGA_) prior to
+#         UMAP embedding.
+
+#     use_rna_velocity : bool, default=False
+#         If ``True``, uses RNA velocity information to compute PAGA. If ``False``,
+#         this option is ignored.
+
+#     use_rep : str, optional
+#         Representation to use when `computing neighbors`_. For example, if data have
+#         been batch normalized with ``scanorama``, the representation
+#         should be ``'Scanorama'``. If not provided, ``scanpy``'s default
+#         representation is used.
+
+#     random_state : int, optional
+#         Seed for the random state used by ``sc.tl.umap``.
+
+#     resolution : float, default=1.0
+#         Resolution for Leiden clustering.
+
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _PAGA:
+#         https://github.com/theislab/paga
+#     .. _computing neighbors:
+#         https://scanpy.readthedocs.io/en/stable/generated/scanpy.pp.neighbors.html
+
+#     """
+#     if verbose:
+#         print("")
+#         print("UMAP EMBEDDING")
+#         print("--------------")
+#     # PCA
+#     if any([force_pca, "X_pca" not in adata.obsm_keys()]):
+#         if verbose:
+#             print("  - computing PCA")
+#         adata = pca(
+#             adata, solver=solver, n_pcs=n_pcs, ignore_ig=ignore_ig, verbose=False
+#         )
+#     # neighbors
+#     if verbose:
+#         print("  - calculating neighbors")
+#     sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, use_rep=use_rep)
+#     # leiden clustering
+#     if verbose:
+#         print("  - leiden clustering")
+#     sc.tl.leiden(adata, resolution=resolution)
+#     # umap (with or without PAGA first)
+#     if paga:
+#         if verbose:
+#             print("  - paga")
+#         sc.tl.paga(adata, use_rna_velocity=use_rna_velocity)
+#         if use_rna_velocity:
+#             adata.uns["paga"]["connectivities"] = adata.uns["paga"][
+#                 "transitions_confidence"
+#             ]
+#         sc.pl.paga(adata, plot=False)
+#         init_pos = "paga"
+#     else:
+#         init_pos = "spectral"
+#     if verbose:
+#         print("  - umap")
+#     sc.tl.umap(adata, init_pos=init_pos, random_state=random_state)
+#     return adata
+
+
+# def dimensionality_reduction(
+#     adata: anndata.AnnData,
+#     solver: str = "arpack",
+#     n_neighbors=20,
+#     n_pcs=40,
+#     ignore_ig=True,
+#     paga=True,
+#     use_rna_velocity=False,
+#     use_rep=None,
+#     random_state=42,
+#     resolution=1.0,
+#     verbose=True,
+# ):
+#     """
+#     Performs PCA, neighborhood graph construction and UMAP embedding.
+#     PAGA is optional, but is performed by default.
+
+#     Parameters
+#     ----------
+
+#     adata : anndata.AnnData)
+#         ``AnnData`` object containing gene counts data.
+
+#     solver : str, default='arpack'
+#         Solver to use for the PCA.
+
+#     n_neighbors : int, default=10
+#         Number of neighbors to calculate for the neighbor graph.
+
+#     n_pcs : int, default=40
+#         Number of principal components to use when computing the neighbor graph.
+#         Although the default value is generally appropriate, it is sometimes useful
+#         to empirically determine the optimal value for `n_pcs`.
+
+#     paga : bool, default=True
+#         If ``True``, performs partition-based graph abstraction (PAGA_) prior to
+#         UMAP embedding.
+
+#     use_rna_velocity : bool, default=False
+#         If ``True``, uses RNA velocity information to compute PAGA. If ``False``,
+#         this option is ignored.
+
+#     use_rep : str, optional
+#         Representation to use when `computing neighbors`_. For example, if data have
+#         been batch normalized with ``scanorama``, the representation
+#         should be ``'Scanorama'``. If not provided, ``scanpy``'s default
+#         representation is used.
+
+#     random_state : int, optional
+#         Seed for the random state used by ``sc.tl.umap``.
+
+#     resolution : float, default=1.0
+#         Resolution for Leiden clustering.
+
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _PAGA:
+#         https://github.com/theislab/paga
+#     .. _computing neighbors:
+#         https://scanpy.readthedocs.io/en/stable/generated/scanpy.pp.neighbors.html
+
+#     """
+#     if verbose:
+#         print("performing PCA...")
+#     if ignore_ig:
+#         _adata = adata.copy()
+#         _adata.var["highly_variable"] = _adata.var["highly_variable"] & ~(
+#             _adata.var["ig"]
+#         )
+#         sc.tl.pca(_adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
+#         adata.obsm["X_pca"] = _adata.obsm["X_pca"]
+#         adata.varm["PCs"] = _adata.varm["PCs"]
+#         adata.uns["pca"] = {
+#             "variance_ratio": _adata.uns["pca"]["variance_ratio"],
+#             "variance": _adata.uns["pca"]["variance"],
+#         }
+#     else:
+#         sc.tl.pca(adata, svd_solver=solver, n_comps=n_pcs, use_highly_variable=True)
+#     if verbose:
+#         print("calculating neighbors...")
+#     sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, use_rep=use_rep)
+#     if verbose:
+#         print("leiden clustering...")
+#     sc.tl.leiden(adata, resolution=resolution)
+#     if paga:
+#         if verbose:
+#             print("paga...")
+#         #         solid_edges = 'transitions_confidence' if use_rna_velocity else 'connectivities'
+#         sc.tl.paga(adata, use_rna_velocity=use_rna_velocity)
+#         if use_rna_velocity:
+#             adata.uns["paga"]["connectivities"] = adata.uns["paga"][
+#                 "transitions_confidence"
+#             ]
+#         sc.pl.paga(adata, plot=False)
+#         if verbose:
+#             print("umap...")
+#         sc.tl.umap(
+#             adata,
+#             init_pos="paga",
+#             random_state=random_state,
+#         )
+#     else:
+#         if verbose:
+#             print("umap...")
+#         sc.tl.umap(adata, random_state=random_state)
+#     return adata
+
+
+# def combat(adata, batch_key="batch", covariates=None, dim_red=True):
+#     """
+#     Batch effect correction using ComBat_ [Johnson07]_.
+
+#     .. seealso::
+#         | W. Evan Johnson, Cheng Li, Ariel Rabinovic
+#         | Adjusting batch effects in microarray expression data using empirical Bayes methods
+#         | *Biostatistics* 2007, doi: 10.1093/biostatistics/kxj037
+
+
+#     Parameters
+#     ----------
+
+#     adata : anndata.AnnData
+#         ``AnnData`` object containing gene counts data.
+
+#     batch_key : str, default='batch'
+#         Name of the column in adata.obs that corresponds to the batch.
+
+#     covariates : iterable object, optional
+#         List of additional covariates besides the batch variable such as adjustment variables
+#         or biological condition. Not including covariates may lead to the removal of real
+#         biological signal.
+
+#     dim_red : bool, default=True
+#         If ``True``, dimentionality reduction will be performed on the post-integration data using
+#         ``scab.tl.dimensionality_reduction()``.
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _ComBat:
+#         https://github.com/brentp/combat.py
+
+#     """
+#     adata_combat = sc.AnnData(X=adata.raw.X, var=adata.raw.var, obs=adata.obs)
+#     adata_combat.layers = adata.layers
+#     adata_combat.raw = adata_combat
+#     # run combat
+#     sc.pp.combat(adata_combat, key=batch_key, covariates=covariates)
+#     sc.pp.highly_variable_genes(adata_combat)
+#     if dim_red:
+#         adata_combat = dimensionality_reduction(adata_combat)
+#     return adata_combat
+
+
+# def mnn(adata, batch_key="batch", min_hvg_batches=1, dim_red=True):
+#     """
+#     Data integration and batch correction using `mutual nearest neighbors`_ [Haghverdi19]_. Uses the
+#     ``scanpy.external.pp.mnn_correct()`` function.
+
+#     .. seealso::
+#         | Laleh Haghverdi, Aaron T L Lun, Michael D Morgan & John C Marioni
+#         | Batch effects in single-cell RNA-sequencing data are corrected by matching mutual nearest neighbors
+#         | *Nature Biotechnology* 2019, doi: 10.1038/nbt.4091
+
+#     Parameters
+#     ----------
+#     adata : anndata.AnnData
+#         ``AnnData`` object containing gene counts data.
+
+#     batch_key : str, default='batch'
+#         Name of the column in adata.obs that corresponds to the batch.
+
+#     min_hvg_batches : int, default=1
+#         Minimum number of batches in which highly variable genes are found in order to be included
+#         in the list of genes used for batch correction. Default is ``1``, which results in the use
+#         of all HVGs found in any batch.
+
+#     dim_red : bool, default=True
+#         If ``True``, dimentionality reduction will be performed on the post-integration data using
+#         ``scab.tl.dimensionality_reduction()``.
+
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _mutual nearest neighbors:
+#         https://github.com/chriscainx/mnnpy
+
+#     """
+#     adata_mnn = adata.raw.to_adata()
+#     adata_mnn.layers = adata.layers
+#     # variable genes
+#     sc.pp.highly_variable_genes(
+#         adata_mnn, min_mean=0.0125, max_mean=3, min_disp=0.5, batch_key=batch_key
+#     )
+#     var_select = adata_mnn.var.highly_variable_nbatches >= min_hvg_batches
+#     var_genes = var_select.index[var_select]
+#     # split per batch into new objects.
+#     batches = adata_mnn.obs[batch_key].cat.categories.tolist()
+#     alldata = {}
+#     for batch in batches:
+#         alldata[batch] = adata_mnn[adata_mnn.obs[batch_key] == batch,]
+#     # run MNN correction
+#     cdata = sc.external.pp.mnn_correct(
+#         *[alldata[b] for b in batches],
+#         svd_dim=50,
+#         batch_key=batch_key,
+#         save_raw=True,
+#         var_subset=var_genes,
+#     )
+#     corr_data = cdata[0][:, var_genes]
+#     if dim_red:
+#         corr_data = dimensionality_reduction(corr_data)
+#     return corr_data
+
+
+# def scanorama(
+#     adata, batch_key="batch", scanorama_key="X_Scanorama", n_dim=50, dim_red=True
+# ):
+#     """
+#     Batch correction using Scanorama_ [Hie19]_.
+
+#     .. seealso::
+#         | Brian Hie, Bryan Bryson, and Bonnie Berger
+#         | Efficient integration of heterogeneous single-cell transcriptomes using Scanorama
+#         | *Nature Biotechnology* 2019, doi: 10.1038/s41587-019-0113-3
+
+#     Parameters
+#     ----------
+
+#     adata : anndata.AnnData
+#         ``AnnData`` object containing gene counts data.
+
+#     batch_key : str, default='batch'
+#         Name of the column in ``adata.obs`` that corresponds to the batch.
+
+#     dim_red : bool, default=True
+#         If ``True``, dimentionality reduction will be performed on the post-integration data using
+#         ``scab.tl.dimensionality_reduction``.
+
+
+#     Returns
+#     -------
+#     adata : ``anndata.AnnData``
+
+
+#     .. _Scanorama:
+#         https://github.com/brianhie/scanorama
+
+#     """
+#     import scanorama
+
+#     # make sure obs names are unique, since we'll need them to incorporate
+#     # Scanorama integrations into the original adata object
+#     # Also, Scanorama needs the raw gene counts, not normalized
+#     adata_scanorama = adata.raw.to_adata()
+#     adata_scanorama.layers = adata.layers
+#     # Scanorama needs the datasets to be dividied into individual batches
+#     # rather than just passing a batch key
+#     batch_names = adata_scanorama.obs[batch_key].cat.categories.tolist()
+#     adatas = [adata_scanorama[adata_scanorama.obs[batch_key] == b] for b in batch_names]
+#     # run Scanorama
+#     scanorama.integrate_scanpy(adatas, dimred=n_dim)
+#     # add the Scanorama to the "complete" adata object
+#     obs_names = [ad.obs_names for ad in adatas]
+#     integrations = [ad.obsm["X_Scanorama"] for ad in adatas]
+#     integrate_dict = {}
+#     for obs_name, integration in zip(obs_names, integrations):
+#         for o, i in zip(obs_names, integration):
+#             integrate_dict[o] = i
+#     all_s = np.array([integrate_dict[o] for o in adata.obs_names])
+#     adata.obsm["X_scanorama"] = all_s
+#     return adata
 
 
 def classify_specificity(
     adata,
     raw,
     agbcs=None,
     groups=None,
     rename=None,
     percentile=0.997,
     percentile_dict=None,
     update=True,
+    uns_batch=None,
     verbose=True,
 ):
     """
     Classifies BCR specificity using antigen barcodes (**AgBCs**). Thresholds are computed by 
     analyzing background AgBC UMI counts in empty droplets.
 
     .. note:: 
@@ -392,14 +578,29 @@
         of AgBCs or groups are provided in `percentile_dict`, all others will use `percentile`.
             
     update : bool, default=True  
         If ``True``, update `adata` with grouped UMI counts and classifications. If ``False``, 
         a Pandas ``DataFrame`` containg classifications will be returned and `adata` will 
         not be modified. 
 
+    uns_batch: str, default=None
+        If provided, `uns_batch` will add batch information to the percentile and threshold
+        data stored in ``adata.uns``. This results in an additional layer of nesting, which 
+        allows concateenating multiple ``AnnData`` objects represeting different batches for 
+        which classification is performed separately. If not provided, the data stored in ``uns`` 
+        would be formatted like::
+
+            adata.uns['agbc_percentiles'] = {agbc1: percentile1, ...}
+            adata.uns['agbc_thresholds'] = {agbc1: threshold1, ...}  
+
+        If `uns_batch` is provided, ``uns`` will be formatted like::
+
+            adata.ubs['agbc_percentiles'] = {uns_batch: {agbc1: percentile1, ...}}
+            adata.ubs['agbc_thresholds'] = {uns_batch: {agbc1: threshold1, ...}}
+
     verbose : bool, default=True  
         If ``True``, calculated threshold values are printed.  
             
     
     Returns
     -------
     output : ``anndata.AnnData`` or ``pandas.DataFrame``
@@ -440,14 +641,16 @@
     empty = raw[no_cell]
 
     # classify AgBC specificities
     if verbose:
         print("")
         print("  THRESHOLDS  ")
         print("--------------")
+    uns_thresholds = {}
+    uns_percentiles = {}
     for group, barcodes in groups.items():
         # remove missing AgBCs
         in_adata = [b for b in barcodes if b in adata.obs]
         in_empty = [b for b in barcodes if b in empty.obs]
         in_both = list(set(in_adata) & set(in_empty))
         if any([not in_adata, not in_empty]):
             err = f"\nERROR: group {group} cannot be processed because all AgBCs are missing from input or raw datasets.\n"
@@ -474,25 +677,34 @@
         # UMI counts for the entire group
         _data = np.sum([np.exp2(adata.obs[bc]) - 1 for bc in in_adata], axis=0)
         adata_groups[group_name] = np.log2(_data + 1)
         # threshold for the entire group (sum of the individual barcode thresholds)
         raw_threshold = np.sum(list(raw_bc_thresholds.values()))
         threshold = np.log2(raw_threshold + 1)
         classifications[group_name] = adata_groups[group_name] > threshold
+        # update uns dicts
+        uns_thresholds[group] = threshold
+        uns_percentiles[group] = pctile
         if verbose:
             print(group_name)
             print(f"percentile: {pctile}")
             print(f"threshold: {threshold}")
             for bc, rt in raw_bc_thresholds.items():
                 print(f"  - {bc}: {np.log2(rt + 1)}")
             print("")
     if update:
         for g, group_data in adata_groups.items():
             adata.obs[g] = group_data
             adata.obs[f"is_{g}"] = classifications[g]
+            if uns_batch is not None:
+                adata.uns["agbc_thresholds"] = {uns_batch: uns_thresholds}
+                adata.uns["agbc_percentiles"] = {uns_batch: uns_percentiles}
+            else:
+                adata.uns["agbc_thresholds"] = uns_thresholds
+                adata.uns["agbc_percentiles"] = uns_percentiles
         return adata
     else:
         return pd.DataFrame(classifications, index=adata.obs_names)
 
 
 def calculate_agbc_confidence(
     adata,
@@ -507,28 +719,28 @@
     Computes AgBC confidence using a control dataset.
 
     Args:
     -----
 
         adata (anndata.AnnData): ``AnnData`` object with AgBC count data (log2 transformed) located in ``adata.obs``.
 
-        control_adata (anndata.AnnData): ``AnnData`` object with AgBC count data (log2 transformed) located in 
-            ``control_adata.obs``. Should contain data from control cells (not antigen sorted) which will be used to 
+        control_adata (anndata.AnnData): ``AnnData`` object with AgBC count data (log2 transformed) located in
+            ``control_adata.obs``. Should contain data from control cells (not antigen sorted) which will be used to
             compute the confidence values
 
         agbcs (list): List of AgBC names. Each AgBC name must be present in both ``adata.obs`` and ``control_adata.obs``.
 
         update (bool): If ``True``, ``adata.obs`` is updated with confidence values (column names are ``f'{agbc}_confidence'``).
             If ``False``, a ``DataFrame`` is returned containing the confidence values. Default is ``True``.
 
-    
+
     Returns:
     --------
     Updated ``adata`` if ``update`` is ``True`` or a ``pandas.DataFrame`` if ``update`` is ``False``.
-    
+
     """
     conf_data = {}
     # check to make sure AgBCs are in both datasets
     if any([a not in control_adata.obs for a in agbcs]):
         missing = [a for a in agbcs if a not in control_adata.obs]
         if verbose:
             print(
```

### Comparing `scab-0.0.6/scab/ut.py` & `scab-0.1.0/scab/ut.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,24 @@
 # BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 # DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 
-
-
-
-
-def get_adata_values(adata, key, receptor='bcr', chain='heavy'):
+def get_adata_values(adata, key, receptor="bcr", chain="heavy"):
     try:
         return adata.obs_vector(key)
     except KeyError:
         data = []
         if receptor not in adata.obs:
-            raise ValueError(f'Receptor {receptor} was not found in the supplied AnnData object')
+            raise ValueError(
+                f"Receptor {receptor} was not found in the supplied AnnData object"
+            )
         vdjs = adata.obs[receptor]
         for vdj in vdjs:
             if (seq := getattr(vdj, chain)) is not None:
                 data.append(seq[key])
             else:
                 data.append(None)
         return data
 
-
```

### Comparing `scab-0.0.6/setup.py` & `scab-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "description": "Single cell analysis of B cells",
     "author": "Bryan Briney",
     "url": "https://www.github.com/briney/scab",
     "author_email": "briney@scripps.edu",
     "version": __version__,
     "install_requires": install_requires,
     "packages": ["scab"],
-    "scripts": [],
+    "scripts": ['bin/batch_cellranger', 'bin/scabranger'],
     "name": "scab",
     "include_package_data": True,
     "classifiers": [
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

