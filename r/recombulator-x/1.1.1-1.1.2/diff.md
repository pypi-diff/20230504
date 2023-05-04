# Comparing `tmp/recombulator-x-1.1.1.tar.gz` & `tmp/recombulator-x-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recombulator-x-1.1.1.tar", last modified: Fri Mar 31 14:34:24 2023, max compression
+gzip compressed data, was "recombulator-x-1.1.2.tar", last modified: Thu May  4 13:36:34 2023, max compression
```

## Comparing `recombulator-x-1.1.1.tar` & `recombulator-x-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-03-31 14:34:24.551122 recombulator-x-1.1.1/
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     1069 2023-03-13 11:45:39.000000 recombulator-x-1.1.1/LICENSE.md
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     7189 2023-03-31 14:34:24.551122 recombulator-x-1.1.1/PKG-INFO
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     5826 2023-03-16 16:18:07.000000 recombulator-x-1.1.1/README.md
-drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-03-31 14:34:24.551122 recombulator-x-1.1.1/recombulator_x.egg-info/
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     7189 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/PKG-INFO
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      499 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/SOURCES.txt
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)        1 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/dependency_links.txt
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       59 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/entry_points.txt
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      103 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/requires.txt
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       14 2023-03-31 14:34:24.000000 recombulator-x-1.1.1/recombulator_x.egg-info/top_level.txt
-drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-03-31 14:34:24.551122 recombulator-x-1.1.1/recombulatorx/
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      154 2023-03-29 12:14:12.000000 recombulator-x-1.1.1/recombulatorx/__init__.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     3122 2023-03-29 15:18:25.000000 recombulator-x-1.1.1/recombulatorx/cli.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     6409 2023-03-16 14:34:49.000000 recombulator-x-1.1.1/recombulatorx/estimate.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    11981 2023-03-31 14:18:56.000000 recombulator-x-1.1.1/recombulatorx/families.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     5016 2023-03-16 14:34:49.000000 recombulator-x-1.1.1/recombulatorx/io.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    14346 2023-03-29 14:34:30.000000 recombulator-x-1.1.1/recombulatorx/likelihood.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    11307 2023-03-16 14:34:49.000000 recombulator-x-1.1.1/recombulatorx/likelihood_direct.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    13669 2023-03-16 14:34:49.000000 recombulator-x-1.1.1/recombulatorx/testing.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      182 2023-03-31 14:17:25.000000 recombulator-x-1.1.1/recombulatorx/types.py
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      993 2023-03-31 14:34:24.691122 recombulator-x-1.1.1/setup.cfg
--rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       38 2023-03-13 11:45:39.000000 recombulator-x-1.1.1/setup.py
+drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-05-04 13:36:34.072407 recombulator-x-1.1.2/
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     1069 2023-03-13 11:45:39.000000 recombulator-x-1.1.2/LICENSE.md
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     6642 2023-05-04 13:36:34.072407 recombulator-x-1.1.2/PKG-INFO
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     5885 2023-05-04 13:18:53.000000 recombulator-x-1.1.2/README.md
+drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-05-04 13:36:34.068407 recombulator-x-1.1.2/recombulator_x.egg-info/
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     6642 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/PKG-INFO
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      499 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)        1 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       58 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/entry_points.txt
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      103 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/requires.txt
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       14 2023-05-04 13:36:34.000000 recombulator-x-1.1.2/recombulator_x.egg-info/top_level.txt
+drwxrwxr-x   0 gbirolo   (1002) gbirolo   (1002)        0 2023-05-04 13:36:34.072407 recombulator-x-1.1.2/recombulatorx/
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      154 2023-03-29 12:14:12.000000 recombulator-x-1.1.2/recombulatorx/__init__.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     6209 2023-05-04 13:17:16.000000 recombulator-x-1.1.2/recombulatorx/cli.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     6409 2023-03-16 14:34:49.000000 recombulator-x-1.1.2/recombulatorx/estimate.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    11981 2023-03-31 14:18:56.000000 recombulator-x-1.1.2/recombulatorx/families.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)     5016 2023-03-16 14:34:49.000000 recombulator-x-1.1.2/recombulatorx/io.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    14346 2023-03-29 14:34:30.000000 recombulator-x-1.1.2/recombulatorx/likelihood.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    11307 2023-03-16 14:34:49.000000 recombulator-x-1.1.2/recombulatorx/likelihood_direct.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)    13669 2023-03-16 14:34:49.000000 recombulator-x-1.1.2/recombulatorx/testing.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      182 2023-03-31 14:17:25.000000 recombulator-x-1.1.2/recombulatorx/types.py
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)      993 2023-05-04 13:36:34.100407 recombulator-x-1.1.2/setup.cfg
+-rw-rw-r--   0 gbirolo   (1002) gbirolo   (1002)       38 2023-03-13 11:45:39.000000 recombulator-x-1.1.2/setup.py
```

### Comparing `recombulator-x-1.1.1/LICENSE.md` & `recombulator-x-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/PKG-INFO` & `recombulator-x-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: recombulator-x
-Version: 1.1.1
+Version: 1.1.2
 Summary: estimation of recombination rates between short tandem repeats (STRs) or other polymorphisms (SNP/indels) along the X chromosome
 Home-page: https://serena-aneli.github.io/recombulator-x/
 Author: Serena Aneli
 Author-email: serena.aneli@unito.it
 License: MIT
-Description: # RECOMBULATOR-X
-        
-        <p align="center">
-          <img align="left" width="300" height="300"  src="docs/assets/images/LOGO.png">
-        </p>
-        <br/>
-        <br/>
-        recombulator-x is a Python module and command line tool for computing the recombination rates between short tandem repeats (STRs) markers and other polymorphisms (SNPs and INDELs) along the X chromosome starting from pedigree data in forensic genetics.
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        
-        :open_book: [Documentation website](https://serena-aneli.github.io/recombulator-x/)
-        
-        :page_facing_up: Please cite [Paper]()
-        
-        <br/>
-        <br/>
-        
-        recombulator-x is written in Python (3.7) and can be used either as a module or as a command-line tool. 
-        It is the first open source implementation of the estimation method introduced in [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub), which is the gold-standard for the estimation of recombination rates for X-chromosomal markers. We designed recombulator-x to solve some practical issues with the original R implementation. Its main advantages are:
-        
-        * performance: much faster than the original implementation, thanks to algorithmic improvements (dynamic programming)
-        * open source: full source code and documentation available from github
-        * input parsing: reads pedigree data in standard (PED) format
-        * user friendly: easy installation (via pip) and usage with a simple command-line tool
-        * comprehensive toolkit: it can deal with short tandem repeats, SNPs and INDELs. 
-        
-        We thank Prof. Michael Nothnagel for kindly sharing the original R implementation with us, which was an important reference for the development.
-        
-        ## :open_book: Documentation
-        Full documentation is available online at the :open_book: [dedicated website](https://serena-aneli.github.io/recombulator-x/), or in this repository under ```docs```.
-        
-        
-        ## :wrench: Installation
-        
-        You can install recombulator-x via the **pip** command from the standard PyPI repository:
-        
-        ```bash
-        pip install recombulator-x
-        ```
-        
-        ## :mortar_board: Overview
-        
-        STRs located on the X chromosome are a valuable resource for solving complex kinship cases in forensic genetics thanks to their peculiar inheritance mode. At the same time, the usage of multiple markers linked along the same chromosome, while increasing the evidential weight, also requires proper consideration of the recombination rates between markers in the biostatistical evaluation of kinship.
-        
-        For more details on X-STR kinship analyses in forensic see [Gomes et al., 2020](https://www.frontiersin.org/articles/10.3389/fgene.2020.00926/full) and [Tillmar et al., 2017](https://www.sciencedirect.com/science/article/pii/S1872497317301126?via%3Dihub).
-        
-        In the case of forensic X-STRs, recombination rates have been either inferred from population samples through high-density multi-point single nucleotide polymorphism (SNP) data or directly estimated in large pedigree-based studies.
-        
-        The main statistical approach for the estimation of recombination rates from pedigrees computes the likelihood of kinship by taking into account all possible recombinations within the maternal haplotype, thus resorting to the exponential complexity of the underlying algorithm (see [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub) for a thorough description of the likelihood computation). Despite a computational update in C++ allowing multi-core parallelization, this approach is expected to be unsuitable when panels of more than 15 X-STRs are considered ([Diegoli et al., 2016](https://www.sciencedirect.com/science/article/pii/S1872497316301247?via%3Dihub)).
-        
-        We developed recombulator-x to overcome this issue. Built upon the same statistical framework of the previous work (Nothnagel et al., 2012), recombulator-x uses a new computational strategy to infer recombination rates for X-STRs, while taking also the probability of mutation into account. 
-        
-        ## :boom: Additional features
-        
-        - Recombulator-X can analyse also SNPs and INDELs.
-        - Data consistency checks
-        - Automatic family preprocessing and informative family extraction 
-        - Multiple likelihood implementations included
-        - Accelerated likelihood computation with the JIT Python compiler Numba
-        - Mutation rates can be estimated for each marker separately or as a unique parameter 
-        - Simulation of pedigrees typed with STRs
-        
-        ## :rocket: Benchmark
-        
-        recombulator-x far exceeds the computational speed of the previous approach and it is scalable to many more markers.  
-        Indeed, performance has been the main focus of recombulator-x: in a test with simulated data of the same size as the two previous works, the time necessary for the likelihood computation of a single family drops from "several months" on 32 cores of a HPC node for the previous approach to 20 minutes on a single core with recombulator-x. This is due to algorithmic improvement time complexity going from exponential to linear with our approach. Conversely, even though the algorithm time complexity is still exponential for type II families, the speed improvement is substantial with respect to the the previous implementation. Moreover, its capacity of dealing with SNPs and INDELs makes it a comprehensive toolkit for addressing linked markers in forensics. 
-        
-        ## :computer: Usage
-        
-        recombulator-x uses the PED files based on [PLINK](https://www.cog-genomics.org/plink/) pedigree files as input. The PED file format stores sample pedigree information (i.e., the familial relationships between samples) and the genotypes. More information on the input file can be found in this repository under ```docs/3_usage.md```.
-        
-        The program can be used both as a Python module or a command-line tool. A detailed notebook for the Python module can be found [here](https://github.com/serena-aneli/recombulator-x/blob/gh-pages/Estimation%20Example.ipynb). 
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: jit
-Provides-Extra: plot
+Provides-Extra: JIT
+Provides-Extra: PLOT
+License-File: LICENSE.md
+
+# RECOMBULATOR-X
+
+<p align="center">
+  <img align="left" width="300" height="300"  src="docs/assets/images/LOGO.png">
+</p>
+<br/>
+<br/>
+recombulator-x is a Python module and command line tool for computing the recombination rates between short tandem repeats (STRs) markers and other polymorphisms (SNPs and INDELs) along the X chromosome starting from pedigree data in forensic genetics.
+<br/>
+<br/>
+<br/>
+<br/>
+
+:open_book: [Documentation website](https://serena-aneli.github.io/recombulator-x/)
+
+:page_facing_up: Please cite [Paper](https://www.biorxiv.org/content/10.1101/2023.03.31.535050v1)
+
+<br/>
+<br/>
+
+recombulator-x is written in Python (3.7) and can be used either as a module or as a command-line tool. 
+It is the first open source implementation of the estimation method introduced in [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub), which is the gold-standard for the estimation of recombination rates for X-chromosomal markers. We designed recombulator-x to solve some practical issues with the original R implementation. Its main advantages are:
+
+* performance: much faster than the original implementation, thanks to algorithmic improvements (dynamic programming)
+* open source: full source code and documentation available from github
+* input parsing: reads pedigree data in standard (PED) format
+* user friendly: easy installation (via pip) and usage with a simple command-line tool
+* comprehensive toolkit: it can deal with short tandem repeats, SNPs and INDELs. 
+
+We thank Prof. Michael Nothnagel for kindly sharing the original R implementation with us, which was an important reference for the development.
+
+## :open_book: Documentation
+Full documentation is available online at the :open_book: [dedicated website](https://serena-aneli.github.io/recombulator-x/), or in this repository under ```docs```.
+
+
+## :wrench: Installation
+
+You can install recombulator-x via the **pip** command from the standard PyPI repository:
+
+```bash
+pip install recombulator-x
+```
+
+## :mortar_board: Overview
+
+STRs located on the X chromosome are a valuable resource for solving complex kinship cases in forensic genetics thanks to their peculiar inheritance mode. At the same time, the usage of multiple markers linked along the same chromosome, while increasing the evidential weight, also requires proper consideration of the recombination rates between markers in the biostatistical evaluation of kinship.
+
+For more details on X-STR kinship analyses in forensic see [Gomes et al., 2020](https://www.frontiersin.org/articles/10.3389/fgene.2020.00926/full) and [Tillmar et al., 2017](https://www.sciencedirect.com/science/article/pii/S1872497317301126?via%3Dihub).
+
+In the case of forensic X-STRs, recombination rates have been either inferred from population samples through high-density multi-point single nucleotide polymorphism (SNP) data or directly estimated in large pedigree-based studies.
+
+The main statistical approach for the estimation of recombination rates from pedigrees computes the likelihood of kinship by taking into account all possible recombinations within the maternal haplotype, thus resorting to the exponential complexity of the underlying algorithm (see [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub) for a thorough description of the likelihood computation). Despite a computational update in C++ allowing multi-core parallelization, this approach is expected to be unsuitable when panels of more than 15 X-STRs are considered ([Diegoli et al., 2016](https://www.sciencedirect.com/science/article/pii/S1872497316301247?via%3Dihub)).
+
+We developed recombulator-x to overcome this issue. Built upon the same statistical framework of the previous work (Nothnagel et al., 2012), recombulator-x uses a new computational strategy to infer recombination rates for X-STRs, while taking also the probability of mutation into account. 
+
+## :boom: Additional features
+
+- Recombulator-X can analyse also SNPs and INDELs.
+- Data consistency checks
+- Automatic family preprocessing and informative family extraction 
+- Multiple likelihood implementations included
+- Accelerated likelihood computation with the JIT Python compiler Numba
+- Mutation rates can be estimated for each marker separately or as a unique parameter 
+- Simulation of pedigrees typed with STRs
+
+## :rocket: Benchmark
+
+recombulator-x far exceeds the computational speed of the previous approach and it is scalable to many more markers.  
+Indeed, performance has been the main focus of recombulator-x: in a test with simulated data of the same size as the two previous works, the time necessary for the likelihood computation of a single family drops from "several months" on 32 cores of a HPC node for the previous approach to 20 minutes on a single core with recombulator-x. This is due to algorithmic improvement time complexity going from exponential to linear with our approach. Conversely, even though the algorithm time complexity is still exponential for type II families, the speed improvement is substantial with respect to the the previous implementation. Moreover, its capacity of dealing with SNPs and INDELs makes it a comprehensive toolkit for addressing linked markers in forensics. 
+
+## :computer: Usage
+
+recombulator-x uses the PED files based on [PLINK](https://www.cog-genomics.org/plink/) pedigree files as input. The PED file format stores sample pedigree information (i.e., the familial relationships between samples) and the genotypes. More information on the input file can be found in this repository under ```docs/3_usage.md```.
+
+The program can be used both as a Python module or a command-line tool. A detailed notebook for the Python module can be found [here](https://github.com/serena-aneli/recombulator-x/blob/gh-pages/Estimation%20Example.ipynb).
```

### Comparing `recombulator-x-1.1.1/README.md` & `recombulator-x-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 <br/>
 <br/>
 <br/>
 <br/>
 
 :open_book: [Documentation website](https://serena-aneli.github.io/recombulator-x/)
 
-:page_facing_up: Please cite [Paper]()
+:page_facing_up: Please cite [Paper](https://www.biorxiv.org/content/10.1101/2023.03.31.535050v1)
 
 <br/>
 <br/>
 
 recombulator-x is written in Python (3.7) and can be used either as a module or as a command-line tool. 
 It is the first open source implementation of the estimation method introduced in [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub), which is the gold-standard for the estimation of recombination rates for X-chromosomal markers. We designed recombulator-x to solve some practical issues with the original R implementation. Its main advantages are:
```

### Comparing `recombulator-x-1.1.1/recombulator_x.egg-info/PKG-INFO` & `recombulator-x-1.1.2/recombulator_x.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 Metadata-Version: 2.1
 Name: recombulator-x
-Version: 1.1.1
+Version: 1.1.2
 Summary: estimation of recombination rates between short tandem repeats (STRs) or other polymorphisms (SNP/indels) along the X chromosome
 Home-page: https://serena-aneli.github.io/recombulator-x/
 Author: Serena Aneli
 Author-email: serena.aneli@unito.it
 License: MIT
-Description: # RECOMBULATOR-X
-        
-        <p align="center">
-          <img align="left" width="300" height="300"  src="docs/assets/images/LOGO.png">
-        </p>
-        <br/>
-        <br/>
-        recombulator-x is a Python module and command line tool for computing the recombination rates between short tandem repeats (STRs) markers and other polymorphisms (SNPs and INDELs) along the X chromosome starting from pedigree data in forensic genetics.
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        
-        :open_book: [Documentation website](https://serena-aneli.github.io/recombulator-x/)
-        
-        :page_facing_up: Please cite [Paper]()
-        
-        <br/>
-        <br/>
-        
-        recombulator-x is written in Python (3.7) and can be used either as a module or as a command-line tool. 
-        It is the first open source implementation of the estimation method introduced in [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub), which is the gold-standard for the estimation of recombination rates for X-chromosomal markers. We designed recombulator-x to solve some practical issues with the original R implementation. Its main advantages are:
-        
-        * performance: much faster than the original implementation, thanks to algorithmic improvements (dynamic programming)
-        * open source: full source code and documentation available from github
-        * input parsing: reads pedigree data in standard (PED) format
-        * user friendly: easy installation (via pip) and usage with a simple command-line tool
-        * comprehensive toolkit: it can deal with short tandem repeats, SNPs and INDELs. 
-        
-        We thank Prof. Michael Nothnagel for kindly sharing the original R implementation with us, which was an important reference for the development.
-        
-        ## :open_book: Documentation
-        Full documentation is available online at the :open_book: [dedicated website](https://serena-aneli.github.io/recombulator-x/), or in this repository under ```docs```.
-        
-        
-        ## :wrench: Installation
-        
-        You can install recombulator-x via the **pip** command from the standard PyPI repository:
-        
-        ```bash
-        pip install recombulator-x
-        ```
-        
-        ## :mortar_board: Overview
-        
-        STRs located on the X chromosome are a valuable resource for solving complex kinship cases in forensic genetics thanks to their peculiar inheritance mode. At the same time, the usage of multiple markers linked along the same chromosome, while increasing the evidential weight, also requires proper consideration of the recombination rates between markers in the biostatistical evaluation of kinship.
-        
-        For more details on X-STR kinship analyses in forensic see [Gomes et al., 2020](https://www.frontiersin.org/articles/10.3389/fgene.2020.00926/full) and [Tillmar et al., 2017](https://www.sciencedirect.com/science/article/pii/S1872497317301126?via%3Dihub).
-        
-        In the case of forensic X-STRs, recombination rates have been either inferred from population samples through high-density multi-point single nucleotide polymorphism (SNP) data or directly estimated in large pedigree-based studies.
-        
-        The main statistical approach for the estimation of recombination rates from pedigrees computes the likelihood of kinship by taking into account all possible recombinations within the maternal haplotype, thus resorting to the exponential complexity of the underlying algorithm (see [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub) for a thorough description of the likelihood computation). Despite a computational update in C++ allowing multi-core parallelization, this approach is expected to be unsuitable when panels of more than 15 X-STRs are considered ([Diegoli et al., 2016](https://www.sciencedirect.com/science/article/pii/S1872497316301247?via%3Dihub)).
-        
-        We developed recombulator-x to overcome this issue. Built upon the same statistical framework of the previous work (Nothnagel et al., 2012), recombulator-x uses a new computational strategy to infer recombination rates for X-STRs, while taking also the probability of mutation into account. 
-        
-        ## :boom: Additional features
-        
-        - Recombulator-X can analyse also SNPs and INDELs.
-        - Data consistency checks
-        - Automatic family preprocessing and informative family extraction 
-        - Multiple likelihood implementations included
-        - Accelerated likelihood computation with the JIT Python compiler Numba
-        - Mutation rates can be estimated for each marker separately or as a unique parameter 
-        - Simulation of pedigrees typed with STRs
-        
-        ## :rocket: Benchmark
-        
-        recombulator-x far exceeds the computational speed of the previous approach and it is scalable to many more markers.  
-        Indeed, performance has been the main focus of recombulator-x: in a test with simulated data of the same size as the two previous works, the time necessary for the likelihood computation of a single family drops from "several months" on 32 cores of a HPC node for the previous approach to 20 minutes on a single core with recombulator-x. This is due to algorithmic improvement time complexity going from exponential to linear with our approach. Conversely, even though the algorithm time complexity is still exponential for type II families, the speed improvement is substantial with respect to the the previous implementation. Moreover, its capacity of dealing with SNPs and INDELs makes it a comprehensive toolkit for addressing linked markers in forensics. 
-        
-        ## :computer: Usage
-        
-        recombulator-x uses the PED files based on [PLINK](https://www.cog-genomics.org/plink/) pedigree files as input. The PED file format stores sample pedigree information (i.e., the familial relationships between samples) and the genotypes. More information on the input file can be found in this repository under ```docs/3_usage.md```.
-        
-        The program can be used both as a Python module or a command-line tool. A detailed notebook for the Python module can be found [here](https://github.com/serena-aneli/recombulator-x/blob/gh-pages/Estimation%20Example.ipynb). 
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: jit
-Provides-Extra: plot
+Provides-Extra: JIT
+Provides-Extra: PLOT
+License-File: LICENSE.md
+
+# RECOMBULATOR-X
+
+<p align="center">
+  <img align="left" width="300" height="300"  src="docs/assets/images/LOGO.png">
+</p>
+<br/>
+<br/>
+recombulator-x is a Python module and command line tool for computing the recombination rates between short tandem repeats (STRs) markers and other polymorphisms (SNPs and INDELs) along the X chromosome starting from pedigree data in forensic genetics.
+<br/>
+<br/>
+<br/>
+<br/>
+
+:open_book: [Documentation website](https://serena-aneli.github.io/recombulator-x/)
+
+:page_facing_up: Please cite [Paper](https://www.biorxiv.org/content/10.1101/2023.03.31.535050v1)
+
+<br/>
+<br/>
+
+recombulator-x is written in Python (3.7) and can be used either as a module or as a command-line tool. 
+It is the first open source implementation of the estimation method introduced in [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub), which is the gold-standard for the estimation of recombination rates for X-chromosomal markers. We designed recombulator-x to solve some practical issues with the original R implementation. Its main advantages are:
+
+* performance: much faster than the original implementation, thanks to algorithmic improvements (dynamic programming)
+* open source: full source code and documentation available from github
+* input parsing: reads pedigree data in standard (PED) format
+* user friendly: easy installation (via pip) and usage with a simple command-line tool
+* comprehensive toolkit: it can deal with short tandem repeats, SNPs and INDELs. 
+
+We thank Prof. Michael Nothnagel for kindly sharing the original R implementation with us, which was an important reference for the development.
+
+## :open_book: Documentation
+Full documentation is available online at the :open_book: [dedicated website](https://serena-aneli.github.io/recombulator-x/), or in this repository under ```docs```.
+
+
+## :wrench: Installation
+
+You can install recombulator-x via the **pip** command from the standard PyPI repository:
+
+```bash
+pip install recombulator-x
+```
+
+## :mortar_board: Overview
+
+STRs located on the X chromosome are a valuable resource for solving complex kinship cases in forensic genetics thanks to their peculiar inheritance mode. At the same time, the usage of multiple markers linked along the same chromosome, while increasing the evidential weight, also requires proper consideration of the recombination rates between markers in the biostatistical evaluation of kinship.
+
+For more details on X-STR kinship analyses in forensic see [Gomes et al., 2020](https://www.frontiersin.org/articles/10.3389/fgene.2020.00926/full) and [Tillmar et al., 2017](https://www.sciencedirect.com/science/article/pii/S1872497317301126?via%3Dihub).
+
+In the case of forensic X-STRs, recombination rates have been either inferred from population samples through high-density multi-point single nucleotide polymorphism (SNP) data or directly estimated in large pedigree-based studies.
+
+The main statistical approach for the estimation of recombination rates from pedigrees computes the likelihood of kinship by taking into account all possible recombinations within the maternal haplotype, thus resorting to the exponential complexity of the underlying algorithm (see [Nothnagel et al., 2012](https://www.sciencedirect.com/science/article/pii/S1872497312000713?via%3Dihub) for a thorough description of the likelihood computation). Despite a computational update in C++ allowing multi-core parallelization, this approach is expected to be unsuitable when panels of more than 15 X-STRs are considered ([Diegoli et al., 2016](https://www.sciencedirect.com/science/article/pii/S1872497316301247?via%3Dihub)).
+
+We developed recombulator-x to overcome this issue. Built upon the same statistical framework of the previous work (Nothnagel et al., 2012), recombulator-x uses a new computational strategy to infer recombination rates for X-STRs, while taking also the probability of mutation into account. 
+
+## :boom: Additional features
+
+- Recombulator-X can analyse also SNPs and INDELs.
+- Data consistency checks
+- Automatic family preprocessing and informative family extraction 
+- Multiple likelihood implementations included
+- Accelerated likelihood computation with the JIT Python compiler Numba
+- Mutation rates can be estimated for each marker separately or as a unique parameter 
+- Simulation of pedigrees typed with STRs
+
+## :rocket: Benchmark
+
+recombulator-x far exceeds the computational speed of the previous approach and it is scalable to many more markers.  
+Indeed, performance has been the main focus of recombulator-x: in a test with simulated data of the same size as the two previous works, the time necessary for the likelihood computation of a single family drops from "several months" on 32 cores of a HPC node for the previous approach to 20 minutes on a single core with recombulator-x. This is due to algorithmic improvement time complexity going from exponential to linear with our approach. Conversely, even though the algorithm time complexity is still exponential for type II families, the speed improvement is substantial with respect to the the previous implementation. Moreover, its capacity of dealing with SNPs and INDELs makes it a comprehensive toolkit for addressing linked markers in forensics. 
+
+## :computer: Usage
+
+recombulator-x uses the PED files based on [PLINK](https://www.cog-genomics.org/plink/) pedigree files as input. The PED file format stores sample pedigree information (i.e., the familial relationships between samples) and the genotypes. More information on the input file can be found in this repository under ```docs/3_usage.md```.
+
+The program can be used both as a Python module or a command-line tool. A detailed notebook for the Python module can be found [here](https://github.com/serena-aneli/recombulator-x/blob/gh-pages/Estimation%20Example.ipynb).
```

### Comparing `recombulator-x-1.1.1/recombulatorx/estimate.py` & `recombulator-x-1.1.2/recombulatorx/estimate.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/recombulatorx/families.py` & `recombulator-x-1.1.2/recombulatorx/families.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/recombulatorx/io.py` & `recombulator-x-1.1.2/recombulatorx/io.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/recombulatorx/likelihood.py` & `recombulator-x-1.1.2/recombulatorx/likelihood.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/recombulatorx/likelihood_direct.py` & `recombulator-x-1.1.2/recombulatorx/likelihood_direct.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/recombulatorx/testing.py` & `recombulator-x-1.1.2/recombulatorx/testing.py`

 * *Files identical despite different names*

### Comparing `recombulator-x-1.1.1/setup.cfg` & `recombulator-x-1.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = recombulator-x
 author = Serena Aneli
 author_email = serena.aneli@unito.it
 url = https://serena-aneli.github.io/recombulator-x/
 description = estimation of recombination rates between short tandem repeats (STRs) or other polymorphisms (SNP/indels) along the X chromosome
-version = 1.1.1
+version = 1.1.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Science/Research
@@ -22,17 +22,17 @@
 install_requires = 
 	numpy >= 1.15.4
 	scipy >= 1.2.0
 	networkx >= 2.0
 	pandas >= 0.23.4
 
 [options.extras_require]
-jit = 
+JIT = 
 	numba >= 0.49.0
-plot = 
+PLOT = 
 	matplotlib >= 3.0.0
 
 [options.entry_points]
 console_scripts = 
 	recombulator-x = recombulatorx.cli:main
 
 [egg_info]
```

