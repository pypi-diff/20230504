# Comparing `tmp/pdcscore-1.0.4.tar.gz` & `tmp/pdcscore-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.0.4.tar", last modified: Thu May  4 06:26:21 2023, max compression
+gzip compressed data, was "pdcscore-1.0.5.tar", last modified: Thu May  4 13:36:14 2023, max compression
```

## Comparing `pdcscore-1.0.4.tar` & `pdcscore-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 06:26:21.189121 pdcscore-1.0.4/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4658 2023-05-04 06:26:21.189121 pdcscore-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2023-05-04 06:24:51.000000 pdcscore-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 06:26:21.174609 pdcscore-1.0.4/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.4/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.4/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:26:21.187122 pdcscore-1.0.4/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4658 2023-05-04 06:26:21.000000 pdcscore-1.0.4/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-04 06:26:21.000000 pdcscore-1.0.4/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 06:26:21.000000 pdcscore-1.0.4/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 06:26:21.000000 pdcscore-1.0.4/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 06:26:21.000000 pdcscore-1.0.4/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 06:26:21.189121 pdcscore-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1502 2023-05-04 06:23:15.000000 pdcscore-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:36:14.339563 pdcscore-1.0.5/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5162 2023-05-04 13:36:14.339563 pdcscore-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4012 2023-05-04 13:32:04.000000 pdcscore-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 13:36:14.317637 pdcscore-1.0.5/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.5/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.5/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:36:14.337564 pdcscore-1.0.5/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     5162 2023-05-04 13:36:14.000000 pdcscore-1.0.5/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-04 13:36:14.000000 pdcscore-1.0.5/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:36:14.000000 pdcscore-1.0.5/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 13:36:14.000000 pdcscore-1.0.5/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 13:36:14.000000 pdcscore-1.0.5/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:36:14.340562 pdcscore-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1502 2023-05-04 13:29:28.000000 pdcscore-1.0.5/setup.py
```

### Comparing `pdcscore-1.0.4/LICENSE` & `pdcscore-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.4/PKG-INFO` & `pdcscore-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-The purpose of this package is to provide a python-native means to calculate a common industry metric for medication adherence, Proportion of Days Covered (PDC). Much of the healthcare analytics industry is transitioning from SAS and are working to replicate such fundametal metrics in new environments. The goal is to offer one less thing that needs to be rebuilt from scratch, and hopefully make work easier for business analysts in the healthcare ecosystem.
+The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
 I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf 
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 Current update is optimized for multiprocessing large datasets.
 
@@ -60,15 +60,15 @@
 
 **PDC_SCORE** - *The patient's PDC score, calculated as DAYSCOVERED / TOTALDAYS. Set to 0 if days of coverage is 0. FORMAT = FLOAT*
 
 
 
 
 
-**USAGE EXAMPLE**
+## Usage Example
 ```python
 
 #  Import required libraries
 import pandas as pd
 import numpy as np
 from pdcscore import pdccalc
 
@@ -94,8 +94,22 @@
                                          , mbr_elig_start_dt_col='START_DT', mbr_elig_end_dt_col='END_DT')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
 
 
+<button class="btn" data-clipboard-target="#usage-example">Copy</button>
+
+<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.8/clipboard.min.js"></script>
+<script>
+  var clipboard = new ClipboardJS('.btn');
+
+  clipboard.on('success', function(e) {
+    console.log('Copied!');
+  });
+
+  clipboard.on('error', function(e) {
+    console.log('Error copying: ' + e);
+  });
+</script>
```

### Comparing `pdcscore-1.0.4/README.md` & `pdcscore-1.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,221 +1,251 @@
-00000000: 5468 6520 7075 7270 6f73 6520 6f66 2074  The purpose of t
-00000010: 6869 7320 7061 636b 6167 6520 6973 2074  his package is t
-00000020: 6f20 7072 6f76 6964 6520 6120 7079 7468  o provide a pyth
-00000030: 6f6e 2d6e 6174 6976 6520 6d65 616e 7320  on-native means 
-00000040: 746f 2063 616c 6375 6c61 7465 2061 2063  to calculate a c
-00000050: 6f6d 6d6f 6e20 696e 6475 7374 7279 206d  ommon industry m
-00000060: 6574 7269 6320 666f 7220 6d65 6469 6361  etric for medica
-00000070: 7469 6f6e 2061 6468 6572 656e 6365 2c20  tion adherence, 
-00000080: 5072 6f70 6f72 7469 6f6e 206f 6620 4461  Proportion of Da
-00000090: 7973 2043 6f76 6572 6564 2028 5044 4329  ys Covered (PDC)
-000000a0: 2e20 4d75 6368 206f 6620 7468 6520 6865  . Much of the he
-000000b0: 616c 7468 6361 7265 2061 6e61 6c79 7469  althcare analyti
-000000c0: 6373 2069 6e64 7573 7472 7920 6973 2074  cs industry is t
-000000d0: 7261 6e73 6974 696f 6e69 6e67 2066 726f  ransitioning fro
-000000e0: 6d20 5341 5320 616e 6420 6172 6520 776f  m SAS and are wo
-000000f0: 726b 696e 6720 746f 2072 6570 6c69 6361  rking to replica
-00000100: 7465 2073 7563 6820 6675 6e64 616d 6574  te such fundamet
-00000110: 616c 206d 6574 7269 6373 2069 6e20 6e65  al metrics in ne
-00000120: 7720 656e 7669 726f 6e6d 656e 7473 2e20  w environments. 
-00000130: 5468 6520 676f 616c 2069 7320 746f 206f  The goal is to o
-00000140: 6666 6572 206f 6e65 206c 6573 7320 7468  ffer one less th
-00000150: 696e 6720 7468 6174 206e 6565 6473 2074  ing that needs t
-00000160: 6f20 6265 2072 6562 7569 6c74 2066 726f  o be rebuilt fro
-00000170: 6d20 7363 7261 7463 682c 2061 6e64 2068  m scratch, and h
-00000180: 6f70 6566 756c 6c79 206d 616b 6520 776f  opefully make wo
-00000190: 726b 2065 6173 6965 7220 666f 7220 6275  rk easier for bu
-000001a0: 7369 6e65 7373 2061 6e61 6c79 7374 7320  siness analysts 
-000001b0: 696e 2074 6865 2068 6561 6c74 6863 6172  in the healthcar
-000001c0: 6520 6563 6f73 7973 7465 6d2e 0a0a 4920  e ecosystem...I 
-000001d0: 666f 6c6c 6f77 6564 2074 6865 206f 7269  followed the ori
-000001e0: 6769 6e61 6c20 696d 706c 656d 656e 7461  ginal implementa
-000001f0: 7469 6f6e 206c 6f67 6963 206f 6620 5044  tion logic of PD
-00000200: 4320 696e 2053 4153 2c20 7468 6973 2063  C in SAS, this c
-00000210: 616e 2062 6520 666f 756e 6420 6174 2068  an be found at h
-00000220: 7474 7073 3a2f 2f73 7570 706f 7274 2e73  ttps://support.s
-00000230: 6173 2e63 6f6d 2f72 6573 6f75 7263 6573  as.com/resources
-00000240: 2f70 6170 6572 732f 7072 6f63 6565 6469  /papers/proceedi
-00000250: 6e67 7331 332f 3136 372d 3230 3133 2e70  ngs13/167-2013.p
-00000260: 6466 200a 0a54 6869 7320 7061 7065 7220  df ..This paper 
-00000270: 6f66 6665 7273 2061 2067 656e 746c 652c  offers a gentle,
-00000280: 2079 6574 2064 6574 6169 6c65 6420 696e   yet detailed in
-00000290: 7472 6f64 7563 7469 6f6e 2074 6f20 7468  troduction to th
-000002a0: 6520 746f 7069 632c 2061 6e64 2077 696c  e topic, and wil
-000002b0: 6c20 7365 7276 6520 6173 2061 2072 6566  l serve as a ref
-000002c0: 6572 656e 6365 2074 6f20 616e 796f 6e65  erence to anyone
-000002d0: 206e 6577 2074 6f20 7468 6520 7375 626a   new to the subj
-000002e0: 6563 742e 0a0a 4375 7272 656e 7420 7570  ect...Current up
-000002f0: 6461 7465 2069 7320 6f70 7469 6d69 7a65  date is optimize
-00000300: 6420 666f 7220 6d75 6c74 6970 726f 6365  d for multiproce
-00000310: 7373 696e 6720 6c61 7267 6520 6461 7461  ssing large data
-00000320: 7365 7473 2e0a 0a50 6c65 6173 6520 7573  sets...Please us
-00000330: 6520 6173 2064 6573 6372 6962 6564 2062  e as described b
-00000340: 656c 6f77 3a0a 0a2a 2a50 4152 414d 4554  elow:..**PARAMET
-00000350: 4552 533a 2a2a 0a0a 2a2a 6461 7461 6672  ERS:**..**datafr
-00000360: 616d 652a 2a20 2d20 2a41 2070 616e 6461  ame** - *A panda
-00000370: 7320 6461 7461 6672 616d 6520 636f 6e74  s dataframe cont
-00000380: 6169 6e69 6e67 2074 6865 2072 6571 7569  aining the requi
-00000390: 7265 6420 636f 6c75 6d6e 7320 6465 7363  red columns desc
-000003a0: 7269 6265 6420 6265 6c6f 772e 2a0a 0a2a  ribed below.*..*
-000003b0: 2a70 6174 6965 6e74 5f69 645f 636f 6c2a  *patient_id_col*
-000003c0: 2a20 2d20 2a41 2075 6e69 7175 6520 7061  * - *A unique pa
-000003d0: 7469 656e 7420 6964 656e 7469 6669 6572  tient identifier
-000003e0: 2e20 466f 726d 6174 203d 2053 5452 494e  . Format = STRIN
-000003f0: 4720 6f72 2049 4e54 4547 4552 2a0a 0a2a  G or INTEGER*..*
-00000400: 2a64 7275 676e 616d 655f 636f 6c2a 2a20  *drugname_col** 
-00000410: 2d20 2a54 6865 206e 616d 6520 6f66 2074  - *The name of t
-00000420: 6865 2064 7275 6720 6265 696e 6720 6669  he drug being fi
-00000430: 6c6c 6564 206f 7220 6472 7567 2063 6c61  lled or drug cla
-00000440: 7373 206f 7220 4765 6e65 7269 6320 6e61  ss or Generic na
-00000450: 6d65 2c20 7065 7220 7573 7561 6c20 5044  me, per usual PD
-00000460: 4320 7265 7175 6972 656d 656e 7473 2e20  C requirements. 
-00000470: 466f 726d 6174 203d 2053 5452 494e 472a  Format = STRING*
-00000480: 0a0a 2a2a 6669 6c6c 6461 7465 5f63 6f6c  ..**filldate_col
-00000490: 2a2a 202d 202a 5468 6520 6461 7465 206f  ** - *The date o
-000004a0: 6620 7468 6520 6669 6c6c 2062 6569 6e67  f the fill being
-000004b0: 2064 6973 7065 6e73 6564 2e20 466f 726d   dispensed. Form
-000004c0: 6174 203d 2044 4154 452a 0a0a 2a2a 7375  at = DATE*..**su
-000004d0: 7070 6c79 5f64 6179 735f 636f 6c2a 2a20  pply_days_col** 
-000004e0: 2d20 2a44 6179 7320 6f66 2073 7570 706c  - *Days of suppl
-000004f0: 7920 6265 696e 6720 6469 7370 656e 7365  y being dispense
-00000500: 6420 6174 2066 696c 6c2e 2046 6f72 6d61  d at fill. Forma
-00000510: 7420 3d20 494e 5445 4745 522a 0a0a 2a2a  t = INTEGER*..**
-00000520: 6d62 725f 656c 6967 5f73 7461 7274 5f64  mbr_elig_start_d
-00000530: 745f 636f 6c2a 2a20 2d20 2a46 6972 7374  t_col** - *First
-00000540: 2064 6174 6520 6f66 2063 6f76 6572 6167   date of coverag
-00000550: 6520 656c 6967 6962 6c69 7479 2066 6f72  e eligiblity for
-00000560: 2070 6174 6965 6e74 206f 7220 6120 7265   patient or a re
-00000570: 6665 7265 6e63 6520 5354 4152 5420 4441  ference START DA
-00000580: 5445 2e20 466f 726d 6174 203d 2044 4154  TE. Format = DAT
-00000590: 452a 0a0a 2a2a 4d42 5245 4c49 4745 4e44  E*..**MBRELIGEND
-000005a0: 2a2a 202d 202a 4c61 7374 2064 6174 6520  ** - *Last date 
-000005b0: 6f66 2063 6f76 6572 6167 6520 656c 6967  of coverage elig
-000005c0: 6962 6c69 7479 2066 6f72 2070 6174 6965  iblity for patie
-000005d0: 6e74 206f 7220 6120 7265 6665 7265 6e63  nt or a referenc
-000005e0: 6520 454e 4420 4441 5445 2e20 466f 726d  e END DATE. Form
-000005f0: 6174 203d 2044 4154 452a 0a0a 2a2a 5265  at = DATE*..**Re
-00000600: 7475 726e 732a 2a20 2d20 2a41 2050 616e  turns** - *A Pan
-00000610: 6461 7320 6461 7461 6672 616d 6520 636f  das dataframe co
-00000620: 6e74 6169 6e69 6e67 2074 6865 2066 6f6c  ntaining the fol
-00000630: 6c6f 7769 6e67 2063 6f6c 756d 6e73 2a0a  lowing columns*.
-00000640: 0a2a 2a70 6174 6965 6e74 5f69 645f 636f  .**patient_id_co
-00000650: 6c2a 2a20 2d20 2a54 6869 7320 7769 6c6c  l** - *This will
-00000660: 2072 6574 7572 6e20 6120 636f 6c75 6d6e   return a column
-00000670: 206e 616d 6520 7265 7072 6573 656e 7469   name representi
-00000680: 6e67 2061 2075 6e69 7175 6520 7061 7469  ng a unique pati
-00000690: 656e 7420 6964 656e 7469 6669 6572 2061  ent identifier a
-000006a0: 7320 7072 6f76 6964 6564 2069 6e20 6f72  s provided in or
-000006b0: 6967 696e 616c 2069 6e70 7574 2064 6174  iginal input dat
-000006c0: 6166 7261 6d65 2e20 464f 524d 4154 203d  aframe. FORMAT =
-000006d0: 2053 5452 494e 472a 0a0a 2a2a 6472 7567   STRING*..**drug
-000006e0: 6e61 6d65 5f63 6f6c 2a2a 202d 202a 5468  name_col** - *Th
-000006f0: 6520 6e61 6d65 206f 6620 7468 6520 6472  e name of the dr
-00000700: 7567 2062 6569 6e67 2066 696c 6c65 6420  ug being filled 
-00000710: 6f72 2064 7275 6720 636c 6173 7320 6f72  or drug class or
-00000720: 2047 656e 6572 6963 206e 616d 652c 2061   Generic name, a
-00000730: 7320 7072 6f76 6964 6564 2069 6e20 6f72  s provided in or
-00000740: 6967 696e 616c 2069 6e70 7574 2064 6174  iginal input dat
-00000750: 6166 7261 6d65 2e2a 0a0a 2a2a 4441 5953  aframe.*..**DAYS
-00000760: 434f 5645 5245 442a 2a2d 202a 5468 6520  COVERED**- *The 
-00000770: 6e75 6d62 6572 206f 6620 756e 6971 7565  number of unique
-00000780: 2064 6179 7320 6f66 2064 7275 6720 636f   days of drug co
-00000790: 7665 7261 6765 2c20 6166 7465 7220 7368  verage, after sh
-000007a0: 6966 7469 6e67 2063 6f76 6572 6167 6520  ifting coverage 
-000007b0: 746f 2061 6363 6f6d 6d6f 6461 7465 2065  to accommodate e
-000007c0: 6172 6c79 2072 6566 696c 6c73 2e20 464f  arly refills. FO
-000007d0: 524d 4154 203d 2049 4e54 4547 4552 2a0a  RMAT = INTEGER*.
-000007e0: 0a2a 2a54 4f54 414c 4441 5953 2a2a 202d  .**TOTALDAYS** -
-000007f0: 202a 5468 6520 746f 7461 6c20 6e75 6d62   *The total numb
-00000800: 6572 206f 6620 6461 7973 2069 6e20 7061  er of days in pa
-00000810: 7469 656e 7420 616e 616c 7973 6973 2077  tient analysis w
-00000820: 696e 646f 772e 2053 6574 2074 6f20 3020  indow. Set to 0 
-00000830: 6966 2064 6179 7320 6f66 2063 6f76 6572  if days of cover
-00000840: 6167 6520 6973 2030 2e20 464f 524d 4154  age is 0. FORMAT
-00000850: 203d 2049 4e54 4547 4552 2a0a 0a2a 2a50   = INTEGER*..**P
-00000860: 4443 5f53 434f 5245 2a2a 202d 202a 5468  DC_SCORE** - *Th
-00000870: 6520 7061 7469 656e 7427 7320 5044 4320  e patient's PDC 
-00000880: 7363 6f72 652c 2063 616c 6375 6c61 7465  score, calculate
-00000890: 6420 6173 2044 4159 5343 4f56 4552 4544  d as DAYSCOVERED
-000008a0: 202f 2054 4f54 414c 4441 5953 2e20 5365   / TOTALDAYS. Se
-000008b0: 7420 746f 2030 2069 6620 6461 7973 206f  t to 0 if days o
-000008c0: 6620 636f 7665 7261 6765 2069 7320 302e  f coverage is 0.
-000008d0: 2046 4f52 4d41 5420 3d20 464c 4f41 542a   FORMAT = FLOAT*
-000008e0: 0a0a 0a0a 0a0a 2a2a 5553 4147 4520 4558  ......**USAGE EX
-000008f0: 414d 504c 452a 2a0a 6060 6070 7974 686f  AMPLE**.```pytho
-00000900: 6e0a 0a23 2020 496d 706f 7274 2072 6571  n..#  Import req
-00000910: 7569 7265 6420 6c69 6272 6172 6965 730a  uired libraries.
-00000920: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
-00000930: 2070 640a 696d 706f 7274 206e 756d 7079   pd.import numpy
-00000940: 2061 7320 6e70 0a66 726f 6d20 7064 6373   as np.from pdcs
-00000950: 636f 7265 2069 6d70 6f72 7420 7064 6363  core import pdcc
-00000960: 616c 630a 0a23 2043 7265 6174 6520 6120  alc..# Create a 
-00000970: 7361 6d70 6c65 2064 6174 6166 7261 6d65  sample dataframe
-00000980: 0a64 6620 3d20 7064 2e44 6174 6146 7261  .df = pd.DataFra
-00000990: 6d65 287b 0a20 2020 2027 4d43 4944 273a  me({.    'MCID':
-000009a0: 205b 2741 272c 2027 4127 2c20 2741 272c   ['A', 'A', 'A',
-000009b0: 2027 4227 2c20 2742 272c 2027 4227 5d2c   'B', 'B', 'B'],
-000009c0: 0a20 2020 2027 4452 5547 4e41 4d45 273a  .    'DRUGNAME':
-000009d0: 205b 2758 272c 2027 5827 2c20 2758 272c   ['X', 'X', 'X',
-000009e0: 2027 5927 2c20 2759 272c 2027 5927 5d2c   'Y', 'Y', 'Y'],
-000009f0: 0a20 2020 2027 5258 5f46 494c 4c45 445f  .    'RX_FILLED_
-00000a00: 4454 273a 2070 642e 746f 5f64 6174 6574  DT': pd.to_datet
-00000a10: 696d 6528 5b27 3230 3232 2d30 312d 3031  ime(['2022-01-01
-00000a20: 272c 2027 3230 3232 2d30 312d 3231 272c  ', '2022-01-21',
-00000a30: 2027 3230 3232 2d30 332d 3230 272c 0a20   '2022-03-20',. 
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000a60: 3230 3232 2d30 312d 3031 272c 2027 3230  2022-01-01', '20
-00000a70: 3232 2d30 322d 3031 272c 2027 3230 3232  22-02-01', '2022
-00000a80: 2d30 332d 3031 275d 292c 0a20 2020 2027  -03-01']),.    '
-00000a90: 4441 5953 5f53 504c 595f 4e42 5227 3a20  DAYS_SPLY_NBR': 
-00000aa0: 5b33 302c 2033 302c 2033 302c 2033 302c  [30, 30, 30, 30,
-00000ab0: 2033 302c 2033 305d 2c0a 2020 2020 2753   30, 30],.    'S
-00000ac0: 5441 5254 5f44 5427 3a20 7064 2e74 6f5f  TART_DT': pd.to_
-00000ad0: 6461 7465 7469 6d65 285b 2732 3032 322d  datetime(['2022-
-00000ae0: 3031 2d30 3127 2c20 2732 3032 322d 3031  01-01', '2022-01
-00000af0: 2d30 3127 2c20 2732 3032 322d 3031 2d30  -01', '2022-01-0
-00000b00: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 2020 2020 2020 2020 2020 2027 3230               '20
-00000b30: 3232 2d30 322d 3031 272c 2027 3230 3232  22-02-01', '2022
-00000b40: 2d30 322d 3031 272c 2027 3230 3232 2d30  -02-01', '2022-0
-00000b50: 322d 3031 275d 292c 0a20 2020 2027 454e  2-01']),.    'EN
-00000b60: 445f 4454 273a 2070 642e 746f 5f64 6174  D_DT': pd.to_dat
-00000b70: 6574 696d 6528 5b27 3230 3232 2d30 332d  etime(['2022-03-
-00000b80: 3331 272c 2027 3230 3232 2d30 332d 3331  31', '2022-03-31
-00000b90: 272c 2027 3230 3232 2d30 332d 3331 272c  ', '2022-03-31',
-00000ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 2020 2020 2732 3032 322d 3033          '2022-03
-00000bd0: 2d33 3127 2c20 2732 3032 322d 3033 2d33  -31', '2022-03-3
+00000000: 5468 6520 6f62 6a65 6374 6976 6520 6f66  The objective of
+00000010: 2074 6869 7320 7061 636b 6167 6520 6973   this package is
+00000020: 2074 6f20 6f66 6665 7220 6120 5079 7468   to offer a Pyth
+00000030: 6f6e 2d62 6173 6564 2073 6f6c 7574 696f  on-based solutio
+00000040: 6e20 666f 7220 636f 6d70 7574 696e 6720  n for computing 
+00000050: 7468 6520 5072 6f70 6f72 7469 6f6e 206f  the Proportion o
+00000060: 6620 4461 7973 2043 6f76 6572 6564 2028  f Days Covered (
+00000070: 5044 4329 2c20 6120 7769 6465 6c79 2075  PDC), a widely u
+00000080: 7365 6420 6d65 7472 6963 2069 6e20 7468  sed metric in th
+00000090: 6520 6865 616c 7468 6361 7265 2069 6e64  e healthcare ind
+000000a0: 7573 7472 7920 746f 2065 7661 6c75 6174  ustry to evaluat
+000000b0: 6520 6d65 6469 6361 7469 6f6e 2061 6468  e medication adh
+000000c0: 6572 656e 6365 2e20 4173 2074 6865 2068  erence. As the h
+000000d0: 6561 6c74 6863 6172 6520 616e 616c 7974  ealthcare analyt
+000000e0: 6963 7320 7365 6374 6f72 2073 6869 6674  ics sector shift
+000000f0: 7320 6177 6179 2066 726f 6d20 5341 532c  s away from SAS,
+00000100: 2074 6865 7265 2069 7320 6120 6772 6f77   there is a grow
+00000110: 696e 6720 6e65 6564 2074 6f20 7265 6372  ing need to recr
+00000120: 6561 7465 206b 6579 206d 6574 7269 6373  eate key metrics
+00000130: 2069 6e20 616c 7465 726e 6174 6976 6520   in alternative 
+00000140: 706c 6174 666f 726d 732e 2054 6869 7320  platforms. This 
+00000150: 7061 636b 6167 6520 6169 6d73 2074 6f20  package aims to 
+00000160: 7369 6d70 6c69 6679 2074 6865 2070 726f  simplify the pro
+00000170: 6365 7373 2061 6e64 2072 6564 7563 6520  cess and reduce 
+00000180: 7468 6520 776f 726b 6c6f 6164 2066 6f72  the workload for
+00000190: 2062 7573 696e 6573 7320 616e 616c 7973   business analys
+000001a0: 7473 2069 6e20 7468 6520 6865 616c 7468  ts in the health
+000001b0: 6361 7265 2065 636f 7379 7374 656d 2062  care ecosystem b
+000001c0: 7920 7072 6f76 6964 696e 6720 6120 7265  y providing a re
+000001d0: 6164 696c 7920 6176 6169 6c61 626c 6520  adily available 
+000001e0: 5044 4320 6361 6c63 756c 6174 696f 6e20  PDC calculation 
+000001f0: 746f 6f6c 2c20 7468 6572 6562 7920 656c  tool, thereby el
+00000200: 696d 696e 6174 696e 6720 7468 6520 6e65  iminating the ne
+00000210: 6564 2074 6f20 6275 696c 6420 6974 2066  ed to build it f
+00000220: 726f 6d20 7363 7261 7463 682e 0a0a 4920  rom scratch...I 
+00000230: 666f 6c6c 6f77 6564 2074 6865 206f 7269  followed the ori
+00000240: 6769 6e61 6c20 696d 706c 656d 656e 7461  ginal implementa
+00000250: 7469 6f6e 206c 6f67 6963 206f 6620 5044  tion logic of PD
+00000260: 4320 696e 2053 4153 2c20 7468 6973 2063  C in SAS, this c
+00000270: 616e 2062 6520 666f 756e 6420 6174 2068  an be found at h
+00000280: 7474 7073 3a2f 2f73 7570 706f 7274 2e73  ttps://support.s
+00000290: 6173 2e63 6f6d 2f72 6573 6f75 7263 6573  as.com/resources
+000002a0: 2f70 6170 6572 732f 7072 6f63 6565 6469  /papers/proceedi
+000002b0: 6e67 7331 332f 3136 372d 3230 3133 2e70  ngs13/167-2013.p
+000002c0: 6466 200a 0a54 6869 7320 7061 7065 7220  df ..This paper 
+000002d0: 6f66 6665 7273 2061 2067 656e 746c 652c  offers a gentle,
+000002e0: 2079 6574 2064 6574 6169 6c65 6420 696e   yet detailed in
+000002f0: 7472 6f64 7563 7469 6f6e 2074 6f20 7468  troduction to th
+00000300: 6520 746f 7069 632c 2061 6e64 2077 696c  e topic, and wil
+00000310: 6c20 7365 7276 6520 6173 2061 2072 6566  l serve as a ref
+00000320: 6572 656e 6365 2074 6f20 616e 796f 6e65  erence to anyone
+00000330: 206e 6577 2074 6f20 7468 6520 7375 626a   new to the subj
+00000340: 6563 742e 0a0a 4375 7272 656e 7420 7570  ect...Current up
+00000350: 6461 7465 2069 7320 6f70 7469 6d69 7a65  date is optimize
+00000360: 6420 666f 7220 6d75 6c74 6970 726f 6365  d for multiproce
+00000370: 7373 696e 6720 6c61 7267 6520 6461 7461  ssing large data
+00000380: 7365 7473 2e0a 0a50 6c65 6173 6520 7573  sets...Please us
+00000390: 6520 6173 2064 6573 6372 6962 6564 2062  e as described b
+000003a0: 656c 6f77 3a0a 0a2a 2a50 4152 414d 4554  elow:..**PARAMET
+000003b0: 4552 533a 2a2a 0a0a 2a2a 6461 7461 6672  ERS:**..**datafr
+000003c0: 616d 652a 2a20 2d20 2a41 2070 616e 6461  ame** - *A panda
+000003d0: 7320 6461 7461 6672 616d 6520 636f 6e74  s dataframe cont
+000003e0: 6169 6e69 6e67 2074 6865 2072 6571 7569  aining the requi
+000003f0: 7265 6420 636f 6c75 6d6e 7320 6465 7363  red columns desc
+00000400: 7269 6265 6420 6265 6c6f 772e 2a0a 0a2a  ribed below.*..*
+00000410: 2a70 6174 6965 6e74 5f69 645f 636f 6c2a  *patient_id_col*
+00000420: 2a20 2d20 2a41 2075 6e69 7175 6520 7061  * - *A unique pa
+00000430: 7469 656e 7420 6964 656e 7469 6669 6572  tient identifier
+00000440: 2e20 466f 726d 6174 203d 2053 5452 494e  . Format = STRIN
+00000450: 4720 6f72 2049 4e54 4547 4552 2a0a 0a2a  G or INTEGER*..*
+00000460: 2a64 7275 676e 616d 655f 636f 6c2a 2a20  *drugname_col** 
+00000470: 2d20 2a54 6865 206e 616d 6520 6f66 2074  - *The name of t
+00000480: 6865 2064 7275 6720 6265 696e 6720 6669  he drug being fi
+00000490: 6c6c 6564 206f 7220 6472 7567 2063 6c61  lled or drug cla
+000004a0: 7373 206f 7220 4765 6e65 7269 6320 6e61  ss or Generic na
+000004b0: 6d65 2c20 7065 7220 7573 7561 6c20 5044  me, per usual PD
+000004c0: 4320 7265 7175 6972 656d 656e 7473 2e20  C requirements. 
+000004d0: 466f 726d 6174 203d 2053 5452 494e 472a  Format = STRING*
+000004e0: 0a0a 2a2a 6669 6c6c 6461 7465 5f63 6f6c  ..**filldate_col
+000004f0: 2a2a 202d 202a 5468 6520 6461 7465 206f  ** - *The date o
+00000500: 6620 7468 6520 6669 6c6c 2062 6569 6e67  f the fill being
+00000510: 2064 6973 7065 6e73 6564 2e20 466f 726d   dispensed. Form
+00000520: 6174 203d 2044 4154 452a 0a0a 2a2a 7375  at = DATE*..**su
+00000530: 7070 6c79 5f64 6179 735f 636f 6c2a 2a20  pply_days_col** 
+00000540: 2d20 2a44 6179 7320 6f66 2073 7570 706c  - *Days of suppl
+00000550: 7920 6265 696e 6720 6469 7370 656e 7365  y being dispense
+00000560: 6420 6174 2066 696c 6c2e 2046 6f72 6d61  d at fill. Forma
+00000570: 7420 3d20 494e 5445 4745 522a 0a0a 2a2a  t = INTEGER*..**
+00000580: 6d62 725f 656c 6967 5f73 7461 7274 5f64  mbr_elig_start_d
+00000590: 745f 636f 6c2a 2a20 2d20 2a46 6972 7374  t_col** - *First
+000005a0: 2064 6174 6520 6f66 2063 6f76 6572 6167   date of coverag
+000005b0: 6520 656c 6967 6962 6c69 7479 2066 6f72  e eligiblity for
+000005c0: 2070 6174 6965 6e74 206f 7220 6120 7265   patient or a re
+000005d0: 6665 7265 6e63 6520 5354 4152 5420 4441  ference START DA
+000005e0: 5445 2e20 466f 726d 6174 203d 2044 4154  TE. Format = DAT
+000005f0: 452a 0a0a 2a2a 4d42 5245 4c49 4745 4e44  E*..**MBRELIGEND
+00000600: 2a2a 202d 202a 4c61 7374 2064 6174 6520  ** - *Last date 
+00000610: 6f66 2063 6f76 6572 6167 6520 656c 6967  of coverage elig
+00000620: 6962 6c69 7479 2066 6f72 2070 6174 6965  iblity for patie
+00000630: 6e74 206f 7220 6120 7265 6665 7265 6e63  nt or a referenc
+00000640: 6520 454e 4420 4441 5445 2e20 466f 726d  e END DATE. Form
+00000650: 6174 203d 2044 4154 452a 0a0a 2a2a 5265  at = DATE*..**Re
+00000660: 7475 726e 732a 2a20 2d20 2a41 2050 616e  turns** - *A Pan
+00000670: 6461 7320 6461 7461 6672 616d 6520 636f  das dataframe co
+00000680: 6e74 6169 6e69 6e67 2074 6865 2066 6f6c  ntaining the fol
+00000690: 6c6f 7769 6e67 2063 6f6c 756d 6e73 2a0a  lowing columns*.
+000006a0: 0a2a 2a70 6174 6965 6e74 5f69 645f 636f  .**patient_id_co
+000006b0: 6c2a 2a20 2d20 2a54 6869 7320 7769 6c6c  l** - *This will
+000006c0: 2072 6574 7572 6e20 6120 636f 6c75 6d6e   return a column
+000006d0: 206e 616d 6520 7265 7072 6573 656e 7469   name representi
+000006e0: 6e67 2061 2075 6e69 7175 6520 7061 7469  ng a unique pati
+000006f0: 656e 7420 6964 656e 7469 6669 6572 2061  ent identifier a
+00000700: 7320 7072 6f76 6964 6564 2069 6e20 6f72  s provided in or
+00000710: 6967 696e 616c 2069 6e70 7574 2064 6174  iginal input dat
+00000720: 6166 7261 6d65 2e20 464f 524d 4154 203d  aframe. FORMAT =
+00000730: 2053 5452 494e 472a 0a0a 2a2a 6472 7567   STRING*..**drug
+00000740: 6e61 6d65 5f63 6f6c 2a2a 202d 202a 5468  name_col** - *Th
+00000750: 6520 6e61 6d65 206f 6620 7468 6520 6472  e name of the dr
+00000760: 7567 2062 6569 6e67 2066 696c 6c65 6420  ug being filled 
+00000770: 6f72 2064 7275 6720 636c 6173 7320 6f72  or drug class or
+00000780: 2047 656e 6572 6963 206e 616d 652c 2061   Generic name, a
+00000790: 7320 7072 6f76 6964 6564 2069 6e20 6f72  s provided in or
+000007a0: 6967 696e 616c 2069 6e70 7574 2064 6174  iginal input dat
+000007b0: 6166 7261 6d65 2e2a 0a0a 2a2a 4441 5953  aframe.*..**DAYS
+000007c0: 434f 5645 5245 442a 2a2d 202a 5468 6520  COVERED**- *The 
+000007d0: 6e75 6d62 6572 206f 6620 756e 6971 7565  number of unique
+000007e0: 2064 6179 7320 6f66 2064 7275 6720 636f   days of drug co
+000007f0: 7665 7261 6765 2c20 6166 7465 7220 7368  verage, after sh
+00000800: 6966 7469 6e67 2063 6f76 6572 6167 6520  ifting coverage 
+00000810: 746f 2061 6363 6f6d 6d6f 6461 7465 2065  to accommodate e
+00000820: 6172 6c79 2072 6566 696c 6c73 2e20 464f  arly refills. FO
+00000830: 524d 4154 203d 2049 4e54 4547 4552 2a0a  RMAT = INTEGER*.
+00000840: 0a2a 2a54 4f54 414c 4441 5953 2a2a 202d  .**TOTALDAYS** -
+00000850: 202a 5468 6520 746f 7461 6c20 6e75 6d62   *The total numb
+00000860: 6572 206f 6620 6461 7973 2069 6e20 7061  er of days in pa
+00000870: 7469 656e 7420 616e 616c 7973 6973 2077  tient analysis w
+00000880: 696e 646f 772e 2053 6574 2074 6f20 3020  indow. Set to 0 
+00000890: 6966 2064 6179 7320 6f66 2063 6f76 6572  if days of cover
+000008a0: 6167 6520 6973 2030 2e20 464f 524d 4154  age is 0. FORMAT
+000008b0: 203d 2049 4e54 4547 4552 2a0a 0a2a 2a50   = INTEGER*..**P
+000008c0: 4443 5f53 434f 5245 2a2a 202d 202a 5468  DC_SCORE** - *Th
+000008d0: 6520 7061 7469 656e 7427 7320 5044 4320  e patient's PDC 
+000008e0: 7363 6f72 652c 2063 616c 6375 6c61 7465  score, calculate
+000008f0: 6420 6173 2044 4159 5343 4f56 4552 4544  d as DAYSCOVERED
+00000900: 202f 2054 4f54 414c 4441 5953 2e20 5365   / TOTALDAYS. Se
+00000910: 7420 746f 2030 2069 6620 6461 7973 206f  t to 0 if days o
+00000920: 6620 636f 7665 7261 6765 2069 7320 302e  f coverage is 0.
+00000930: 2046 4f52 4d41 5420 3d20 464c 4f41 542a   FORMAT = FLOAT*
+00000940: 0a0a 0a0a 0a0a 2323 2055 7361 6765 2045  ......## Usage E
+00000950: 7861 6d70 6c65 0a60 6060 7079 7468 6f6e  xample.```python
+00000960: 0a0a 2320 2049 6d70 6f72 7420 7265 7175  ..#  Import requ
+00000970: 6972 6564 206c 6962 7261 7269 6573 0a69  ired libraries.i
+00000980: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+00000990: 7064 0a69 6d70 6f72 7420 6e75 6d70 7920  pd.import numpy 
+000009a0: 6173 206e 700a 6672 6f6d 2070 6463 7363  as np.from pdcsc
+000009b0: 6f72 6520 696d 706f 7274 2070 6463 6361  ore import pdcca
+000009c0: 6c63 0a0a 2320 4372 6561 7465 2061 2073  lc..# Create a s
+000009d0: 616d 706c 6520 6461 7461 6672 616d 650a  ample dataframe.
+000009e0: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+000009f0: 6528 7b0a 2020 2020 274d 4349 4427 3a20  e({.    'MCID': 
+00000a00: 5b27 4127 2c20 2741 272c 2027 4127 2c20  ['A', 'A', 'A', 
+00000a10: 2742 272c 2027 4227 2c20 2742 275d 2c0a  'B', 'B', 'B'],.
+00000a20: 2020 2020 2744 5255 474e 414d 4527 3a20      'DRUGNAME': 
+00000a30: 5b27 5827 2c20 2758 272c 2027 5827 2c20  ['X', 'X', 'X', 
+00000a40: 2759 272c 2027 5927 2c20 2759 275d 2c0a  'Y', 'Y', 'Y'],.
+00000a50: 2020 2020 2752 585f 4649 4c4c 4544 5f44      'RX_FILLED_D
+00000a60: 5427 3a20 7064 2e74 6f5f 6461 7465 7469  T': pd.to_dateti
+00000a70: 6d65 285b 2732 3032 322d 3031 2d30 3127  me(['2022-01-01'
+00000a80: 2c20 2732 3032 322d 3031 2d32 3127 2c20  , '2022-01-21', 
+00000a90: 2732 3032 322d 3033 2d32 3027 2c0a 2020  '2022-03-20',.  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2732                '2
+00000ac0: 3032 322d 3031 2d30 3127 2c20 2732 3032  022-01-01', '202
+00000ad0: 322d 3032 2d30 3127 2c20 2732 3032 322d  2-02-01', '2022-
+00000ae0: 3033 2d30 3127 5d29 2c0a 2020 2020 2744  03-01']),.    'D
+00000af0: 4159 535f 5350 4c59 5f4e 4252 273a 205b  AYS_SPLY_NBR': [
+00000b00: 3330 2c20 3330 2c20 3330 2c20 3330 2c20  30, 30, 30, 30, 
+00000b10: 3330 2c20 3330 5d2c 0a20 2020 2027 5354  30, 30],.    'ST
+00000b20: 4152 545f 4454 273a 2070 642e 746f 5f64  ART_DT': pd.to_d
+00000b30: 6174 6574 696d 6528 5b27 3230 3232 2d30  atetime(['2022-0
+00000b40: 312d 3031 272c 2027 3230 3232 2d30 312d  1-01', '2022-01-
+00000b50: 3031 272c 2027 3230 3232 2d30 312d 3031  01', '2022-01-01
+00000b60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 2020 2020 2020 2020 2020 2020 2732 3032              '202
+00000b90: 322d 3032 2d30 3127 2c20 2732 3032 322d  2-02-01', '2022-
+00000ba0: 3032 2d30 3127 2c20 2732 3032 322d 3032  02-01', '2022-02
+00000bb0: 2d30 3127 5d29 2c0a 2020 2020 2745 4e44  -01']),.    'END
+00000bc0: 5f44 5427 3a20 7064 2e74 6f5f 6461 7465  _DT': pd.to_date
+00000bd0: 7469 6d65 285b 2732 3032 322d 3033 2d33  time(['2022-03-3
 00000be0: 3127 2c20 2732 3032 322d 3033 2d33 3127  1', '2022-03-31'
-00000bf0: 5d29 0a7d 290a 0a23 2049 6e73 7065 6374  ]).})..# Inspect
-00000c00: 2073 616d 706c 6520 6461 7461 0a64 662e   sample data.df.
-00000c10: 6865 6164 286e 3d6c 656e 2864 6629 290a  head(n=len(df)).
-00000c20: 0a23 2063 616c 6375 6c61 7465 2050 4443  .# calculate PDC
-00000c30: 2073 636f 7265 7320 6f6e 2074 6865 2069   scores on the i
-00000c40: 6e70 7574 2044 6174 6146 7261 6d65 0a63  nput DataFrame.c
-00000c50: 616c 6366 756e 633d 2070 6463 6361 6c63  alcfunc= pdccalc
-00000c60: 2864 6174 6166 7261 6d65 3d64 662c 2070  (dataframe=df, p
-00000c70: 6174 6965 6e74 5f69 645f 636f 6c3d 274d  atient_id_col='M
-00000c80: 4349 4427 2c20 6472 7567 6e61 6d65 5f63  CID', drugname_c
-00000c90: 6f6c 3d27 4452 5547 4e41 4d45 270a 2020  ol='DRUGNAME'.  
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 2020 202c 2066 696c 6c64 6174         , filldat
-00000cd0: 655f 636f 6c3d 2752 585f 4649 4c4c 4544  e_col='RX_FILLED
-00000ce0: 5f44 5427 2c20 7375 7070 6c79 5f64 6179  _DT', supply_day
-00000cf0: 735f 636f 6c3d 2744 4159 535f 5350 4c59  s_col='DAYS_SPLY
-00000d00: 5f4e 4252 270a 2020 2020 2020 2020 2020  _NBR'.          
+00000bf0: 2c20 2732 3032 322d 3033 2d33 3127 2c0a  , '2022-03-31',.
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2020 2020 2027 3230 3232 2d30 332d         '2022-03-
+00000c30: 3331 272c 2027 3230 3232 2d30 332d 3331  31', '2022-03-31
+00000c40: 272c 2027 3230 3232 2d30 332d 3331 275d  ', '2022-03-31']
+00000c50: 290a 7d29 0a0a 2320 496e 7370 6563 7420  ).})..# Inspect 
+00000c60: 7361 6d70 6c65 2064 6174 610a 6466 2e68  sample data.df.h
+00000c70: 6561 6428 6e3d 6c65 6e28 6466 2929 0a0a  ead(n=len(df))..
+00000c80: 2320 6361 6c63 756c 6174 6520 5044 4320  # calculate PDC 
+00000c90: 7363 6f72 6573 206f 6e20 7468 6520 696e  scores on the in
+00000ca0: 7075 7420 4461 7461 4672 616d 650a 6361  put DataFrame.ca
+00000cb0: 6c63 6675 6e63 3d20 7064 6363 616c 6328  lcfunc= pdccalc(
+00000cc0: 6461 7461 6672 616d 653d 6466 2c20 7061  dataframe=df, pa
+00000cd0: 7469 656e 745f 6964 5f63 6f6c 3d27 4d43  tient_id_col='MC
+00000ce0: 4944 272c 2064 7275 676e 616d 655f 636f  ID', drugname_co
+00000cf0: 6c3d 2744 5255 474e 414d 4527 0a20 2020  l='DRUGNAME'.   
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-00000d30: 206d 6272 5f65 6c69 675f 7374 6172 745f   mbr_elig_start_
-00000d40: 6474 5f63 6f6c 3d27 5354 4152 545f 4454  dt_col='START_DT
-00000d50: 272c 206d 6272 5f65 6c69 675f 656e 645f  ', mbr_elig_end_
-00000d60: 6474 5f63 6f6c 3d27 454e 445f 4454 2729  dt_col='END_DT')
-00000d70: 0a70 6463 5f73 636f 7265 735f 6466 203d  .pdc_scores_df =
-00000d80: 2063 616c 6366 756e 632e 6361 6c63 756c   calcfunc.calcul
-00000d90: 6174 655f 7064 6328 290a 0a23 2049 6e73  ate_pdc()..# Ins
-00000da0: 7065 6374 206f 7574 7075 740a 7064 635f  pect output.pdc_
-00000db0: 7363 6f72 6573 5f64 662e 6865 6164 2829  scores_df.head()
-00000dc0: 0a0a                                     ..
+00000d20: 2020 2020 2020 2c20 6669 6c6c 6461 7465        , filldate
+00000d30: 5f63 6f6c 3d27 5258 5f46 494c 4c45 445f  _col='RX_FILLED_
+00000d40: 4454 272c 2073 7570 706c 795f 6461 7973  DT', supply_days
+00000d50: 5f63 6f6c 3d27 4441 5953 5f53 504c 595f  _col='DAYS_SPLY_
+00000d60: 4e42 5227 0a20 2020 2020 2020 2020 2020  NBR'.           
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2c20                , 
+00000d90: 6d62 725f 656c 6967 5f73 7461 7274 5f64  mbr_elig_start_d
+00000da0: 745f 636f 6c3d 2753 5441 5254 5f44 5427  t_col='START_DT'
+00000db0: 2c20 6d62 725f 656c 6967 5f65 6e64 5f64  , mbr_elig_end_d
+00000dc0: 745f 636f 6c3d 2745 4e44 5f44 5427 290a  t_col='END_DT').
+00000dd0: 7064 635f 7363 6f72 6573 5f64 6620 3d20  pdc_scores_df = 
+00000de0: 6361 6c63 6675 6e63 2e63 616c 6375 6c61  calcfunc.calcula
+00000df0: 7465 5f70 6463 2829 0a0a 2320 496e 7370  te_pdc()..# Insp
+00000e00: 6563 7420 6f75 7470 7574 0a70 6463 5f73  ect output.pdc_s
+00000e10: 636f 7265 735f 6466 2e68 6561 6428 290a  cores_df.head().
+00000e20: 0a0a 3c62 7574 746f 6e20 636c 6173 733d  ..<button class=
+00000e30: 2262 746e 2220 6461 7461 2d63 6c69 7062  "btn" data-clipb
+00000e40: 6f61 7264 2d74 6172 6765 743d 2223 7573  oard-target="#us
+00000e50: 6167 652d 6578 616d 706c 6522 3e43 6f70  age-example">Cop
+00000e60: 793c 2f62 7574 746f 6e3e 0a0a 3c73 6372  y</button>..<scr
+00000e70: 6970 7420 7372 633d 2268 7474 7073 3a2f  ipt src="https:/
+00000e80: 2f63 646e 6a73 2e63 6c6f 7564 666c 6172  /cdnjs.cloudflar
+00000e90: 652e 636f 6d2f 616a 6178 2f6c 6962 732f  e.com/ajax/libs/
+00000ea0: 636c 6970 626f 6172 642e 6a73 2f32 2e30  clipboard.js/2.0
+00000eb0: 2e38 2f63 6c69 7062 6f61 7264 2e6d 696e  .8/clipboard.min
+00000ec0: 2e6a 7322 3e3c 2f73 6372 6970 743e 0a3c  .js"></script>.<
+00000ed0: 7363 7269 7074 3e0a 2020 7661 7220 636c  script>.  var cl
+00000ee0: 6970 626f 6172 6420 3d20 6e65 7720 436c  ipboard = new Cl
+00000ef0: 6970 626f 6172 644a 5328 272e 6274 6e27  ipboardJS('.btn'
+00000f00: 293b 0a0a 2020 636c 6970 626f 6172 642e  );..  clipboard.
+00000f10: 6f6e 2827 7375 6363 6573 7327 2c20 6675  on('success', fu
+00000f20: 6e63 7469 6f6e 2865 2920 7b0a 2020 2020  nction(e) {.    
+00000f30: 636f 6e73 6f6c 652e 6c6f 6728 2743 6f70  console.log('Cop
+00000f40: 6965 6421 2729 3b0a 2020 7d29 3b0a 0a20  ied!');.  });.. 
+00000f50: 2063 6c69 7062 6f61 7264 2e6f 6e28 2765   clipboard.on('e
+00000f60: 7272 6f72 272c 2066 756e 6374 696f 6e28  rror', function(
+00000f70: 6529 207b 0a20 2020 2063 6f6e 736f 6c65  e) {.    console
+00000f80: 2e6c 6f67 2827 4572 726f 7220 636f 7079  .log('Error copy
+00000f90: 696e 673a 2027 202b 2065 293b 0a20 207d  ing: ' + e);.  }
+00000fa0: 293b 0a3c 2f73 6372 6970 743e            );.</script>
```

### Comparing `pdcscore-1.0.4/pdcscore/pdcscore.py` & `pdcscore-1.0.5/pdcscore/pdcscore.py`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.4/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.0.5/pdcscore.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-The purpose of this package is to provide a python-native means to calculate a common industry metric for medication adherence, Proportion of Days Covered (PDC). Much of the healthcare analytics industry is transitioning from SAS and are working to replicate such fundametal metrics in new environments. The goal is to offer one less thing that needs to be rebuilt from scratch, and hopefully make work easier for business analysts in the healthcare ecosystem.
+The objective of this package is to offer a Python-based solution for computing the Proportion of Days Covered (PDC), a widely used metric in the healthcare industry to evaluate medication adherence. As the healthcare analytics sector shifts away from SAS, there is a growing need to recreate key metrics in alternative platforms. This package aims to simplify the process and reduce the workload for business analysts in the healthcare ecosystem by providing a readily available PDC calculation tool, thereby eliminating the need to build it from scratch.
 
 I followed the original implementation logic of PDC in SAS, this can be found at https://support.sas.com/resources/papers/proceedings13/167-2013.pdf 
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 Current update is optimized for multiprocessing large datasets.
 
@@ -60,15 +60,15 @@
 
 **PDC_SCORE** - *The patient's PDC score, calculated as DAYSCOVERED / TOTALDAYS. Set to 0 if days of coverage is 0. FORMAT = FLOAT*
 
 
 
 
 
-**USAGE EXAMPLE**
+## Usage Example
 ```python
 
 #  Import required libraries
 import pandas as pd
 import numpy as np
 from pdcscore import pdccalc
 
@@ -94,8 +94,22 @@
                                          , mbr_elig_start_dt_col='START_DT', mbr_elig_end_dt_col='END_DT')
 pdc_scores_df = calcfunc.calculate_pdc()
 
 # Inspect output
 pdc_scores_df.head()
 
 
+<button class="btn" data-clipboard-target="#usage-example">Copy</button>
+
+<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.8/clipboard.min.js"></script>
+<script>
+  var clipboard = new ClipboardJS('.btn');
+
+  clipboard.on('success', function(e) {
+    console.log('Copied!');
+  });
+
+  clipboard.on('error', function(e) {
+    console.log('Error copying: ' + e);
+  });
+</script>
```

### Comparing `pdcscore-1.0.4/setup.py` & `pdcscore-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.0.4',
+    version='1.0.5',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

