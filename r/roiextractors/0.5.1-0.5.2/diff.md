# Comparing `tmp/roiextractors-0.5.1.tar.gz` & `tmp/roiextractors-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roiextractors-0.5.1.tar", last modified: Tue Nov  1 14:46:49 2022, max compression
+gzip compressed data, was "roiextractors-0.5.2.tar", last modified: Thu May  4 15:25:04 2023, max compression
```

## Comparing `roiextractors-0.5.1.tar` & `roiextractors-0.5.2.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.092363 roiextractors-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-11-01 14:46:41.000000 roiextractors-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-01 14:46:41.000000 roiextractors-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9146 2022-11-01 14:46:49.092363 roiextractors-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7505 2022-11-01 14:46:41.000000 roiextractors-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-01 14:46:41.000000 roiextractors-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 14:46:49.092363 roiextractors-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-11-01 14:46:41.000000 roiextractors-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.068363 roiextractors-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.076363 roiextractors-0.5.1/src/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.080363 roiextractors-0.5.1/src/roiextractors/example_datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/example_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5597 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/example_datasets/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    20218 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extraction_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractorlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.080363 roiextractors-0.5.1/src/roiextractors/extractors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.080363 roiextractors-0.5.1/src/roiextractors/extractors/caiman/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.080363 roiextractors-0.5.1/src/roiextractors/extractors/hdf5imagingextractor/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.084363 roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/memmapextractors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.084363 roiextractors-0.5.1/src/roiextractors/extractors/numpyextractors/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/numpyextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12682 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/numpyextractors/numpyextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.084363 roiextractors-0.5.1/src/roiextractors/extractors/nwbextractors/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/nwbextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14476 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/nwbextractors/nwbextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.084363 roiextractors-0.5.1/src/roiextractors/extractors/sbximagingextractor/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/sbximagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6608 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.088363 roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6045 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)    14291 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.088363 roiextractors-0.5.1/src/roiextractors/extractors/simaextractor/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/simaextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6378 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.088363 roiextractors-0.5.1/src/roiextractors/extractors/suite2p/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8527 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.088363 roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/imagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7875 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/multiimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/multisegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)    14609 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/segmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)    16511 2022-11-01 14:46:41.000000 roiextractors-0.5.1/src/roiextractors/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 14:46:49.080363 roiextractors-0.5.1/src/roiextractors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9146 2022-11-01 14:46:48.000000 roiextractors-0.5.1/src/roiextractors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-11-01 14:46:49.000000 roiextractors-0.5.1/src/roiextractors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 14:46:48.000000 roiextractors-0.5.1/src/roiextractors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-01 14:46:48.000000 roiextractors-0.5.1/src/roiextractors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 14:46:48.000000 roiextractors-0.5.1/src/roiextractors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-04 15:25:00.000000 roiextractors-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 15:25:00.000000 roiextractors-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-04 15:25:04.979715 roiextractors-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-04 15:25:00.000000 roiextractors-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 15:25:00.000000 roiextractors-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:25:04.979715 roiextractors-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-04 15:25:00.000000 roiextractors-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.971715 roiextractors-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.975715 roiextractors-0.5.2/src/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/example_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/example_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/example_datasets/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extraction_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractorlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/caiman/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/memmapextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/numpyextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/nwbextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.979715 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/imagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/multiimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/multisegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/segmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-05-04 15:25:00.000000 roiextractors-0.5.2/src/roiextractors/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:25:04.975715 roiextractors-0.5.2/src/roiextractors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 15:25:04.000000 roiextractors-0.5.2/src/roiextractors.egg-info/top_level.txt
```

### Comparing `roiextractors-0.5.1/LICENSE.txt` & `roiextractors-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/PKG-INFO` & `roiextractors-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
 Author: Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
```

### Comparing `roiextractors-0.5.1/README.md` & `roiextractors-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/setup.py` & `roiextractors-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 gin_config_file_base = root / "base_gin_test_config.json"
 gin_config_file_local = root / "tests" / "gin_test_config.json"
 if not gin_config_file_local.exists():
     copy_file(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="roiextractors",
-    version="0.5.1",
+    version="0.5.2",
     author="Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino",
     author_email="ben.dichter@gmail.com",
     description="Python module for extracting optical physiology ROIs and traces for various file types and formats",
     url="https://github.com/catalystneuro/roiextractors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
```

### Comparing `roiextractors-0.5.1/src/roiextractors/__init__.py` & `roiextractors-0.5.2/src/roiextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/example_datasets/toy_example.py` & `roiextractors-0.5.2/src/roiextractors/example_datasets/toy_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                     raw[u_i, s : s + len(resp)] += resp
                 else:
                     raw[u_i, s:] = resp[: frames - s]
                 deconvolved[u_i, s] = 1
 
     # generate video
     video = np.zeros((frames, size_x, size_y))
-    for (rp, t) in zip(roi_pixels, raw):
+    for rp, t in zip(roi_pixels, raw):
         for r in rp:
             video[:, r[0], r[1]] += t * im[r[0], r[1]]
 
     # normalize video
     video /= np.max(video)
 
     # add noise
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extraction_tools.py` & `roiextractors-0.5.2/src/roiextractors/extraction_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         self.frame_shape[self.rows_axis] = self.num_rows
         self.frame_shape[self.columns_axis] = self.num_columns
         self.frame_shape[self.channels_axis] = self.num_channels
         self.frame_shape.pop(self.frame_axis)
         self.frame_shape = tuple(self.frame_shape)
 
     def _validate_video_structure(self) -> None:
-
         exception_message = (
             "Invalid structure: "
             f"{self.__repr__()}, "
             "each property axis should be unique value between 0 and 3 (inclusive)"
         )
 
         axis_values = set((self.rows_axis, self.columns_axis, self.channels_axis, self.frame_axis))
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractorlist.py` & `roiextractors-0.5.2/src/roiextractors/extractorlist.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,26 +8,33 @@
 from .extractors.nwbextractors import NwbImagingExtractor, NwbSegmentationExtractor
 from .extractors.schnitzerextractor import (
     CnmfeSegmentationExtractor,
     ExtractSegmentationExtractor,
 )
 from .extractors.simaextractor import SimaSegmentationExtractor
 from .extractors.suite2p import Suite2pSegmentationExtractor
-from .extractors.tiffimagingextractors import TiffImagingExtractor, ScanImageTiffImagingExtractor
+from .extractors.tiffimagingextractors import (
+    TiffImagingExtractor,
+    ScanImageTiffImagingExtractor,
+    BrukerTiffImagingExtractor,
+    MicroManagerTiffImagingExtractor,
+)
 from .extractors.sbximagingextractor import SbxImagingExtractor
 from .extractors.memmapextractors import NumpyMemmapImagingExtractor
 from .extractors.memmapextractors import MemmapImagingExtractor
 from .multisegmentationextractor import MultiSegmentationExtractor
 from .multiimagingextractor import MultiImagingExtractor
 
 imaging_extractor_full_list = [
     NumpyImagingExtractor,
     Hdf5ImagingExtractor,
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
+    BrukerTiffImagingExtractor,
+    MicroManagerTiffImagingExtractor,
     NwbImagingExtractor,
     SbxImagingExtractor,
     NumpyMemmapImagingExtractor,
     MemmapImagingExtractor,
 ]
 
 segmentation_extractor_full_list = [
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/caiman/caimansegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/caiman/caimansegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
             "channel_names": channel_names,
         }
 
     def __del__(self):
         self._file.close()
 
     def get_frames(self, frame_idxs: ArrayType, channel: Optional[int] = 0):
-
         # Fancy indexing is non performant for h5.py with long frame lists
         if frame_idxs is not None:
             slice_start = np.min(frame_idxs)
             slice_stop = min(np.max(frame_idxs) + 1, self.get_num_frames())
         else:
             slice_start = 0
             slice_stop = self.get_num_frames()
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/memmapextractors.py` & `roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/memmapextractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     PathType,
     DtypeType,
     NumpyArray,
 )
 
 
 class MemmapImagingExtractor(ImagingExtractor):
-
     extractor_name = "MemmapImagingExtractor"
 
     def __init__(
         self,
         video,
     ) -> None:
         """
@@ -73,15 +72,14 @@
         """
         return self._num_channels
 
     def get_dtype(self) -> DtypeType:
         return self.dtype
 
     def get_video_shape(self) -> Tuple[int, int, int, int]:
-
         return (self._num_frames, self._num_rows, self._num_columns, self._num_channels)
 
     @staticmethod
     def write_imaging(
         imaging_extractor: ImagingExtractor,
         save_path: PathType,
         verbose: bool = False,
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ...imagingextractor import ImagingExtractor
 from typing import Tuple, Dict
 from roiextractors.extraction_tools import read_numpy_memmap_video, VideoStructure, DtypeType, PathType
 from .memmapextractors import MemmapImagingExtractor
 
 
 class NumpyMemmapImagingExtractor(MemmapImagingExtractor):
-
     extractor_name = "NumpyMemmapImagingExtractor"
 
     def __init__(
         self,
         file_path: PathType,
         video_structure: VideoStructure,
         sampling_frequency: float,
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/numpyextractors/numpyextractors.py` & `roiextractors-0.5.2/src/roiextractors/extractors/numpyextractors/numpyextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         frames = self._video.take(indices=frame_idxs, axis=0)
         if channel is not None:
             frames = frames[..., channel].squeeze()
 
         return frames
 
     def get_video(self, start_frame=None, end_frame=None, channel: Optional[int] = 0) -> np.ndarray:
-
         return self._video[start_frame:end_frame, ..., channel]
 
     def get_image_size(self) -> Tuple[int, int]:
         return (self._num_rows, self._num_columns)
 
     def get_num_frames(self):
         return self._num_frames
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/nwbextractors/nwbextractors.py` & `roiextractors-0.5.2/src/roiextractors/extractors/nwbextractors/nwbextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
             Ophys=dict(
                 Device=[dict(name=dev) for dev in nwbfile.devices],
                 TwoPhotonSeries=[dict(name=opts.name)],
             ),
         )
 
     def get_frames(self, frame_idxs: ArrayType, channel: Optional[int] = 0):
-
         # Fancy indexing is non performant for h5.py with long frame lists
         if frame_idxs is not None:
             slice_start = np.min(frame_idxs)
             slice_stop = min(np.max(frame_idxs) + 1, self.get_num_frames())
         else:
             slice_start = 0
             slice_stop = self.get_num_frames()
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 
     def get_frames(self, frame_idxs: ArrayType, channel: int = 0) -> np.array:
         frame_out = np.iinfo("uint16").max - self._data.transpose(4, 2, 1, 0, 3)[frame_idxs, :, :, channel, 0]
 
         return frame_out
 
     def get_video(self, start_frame=None, end_frame=None, channel: Optional[int] = 0) -> np.ndarray:
-
         frame_out = np.iinfo("uint16").max - self._data[channel, :, :, 0, start_frame:end_frame]
         return frame_out.transpose(2, 1, 0)
 
     def get_image_size(self) -> Tuple[int, int]:
         return tuple(self._info["sz"])
 
     def get_num_frames(self) -> int:
```

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/imagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/multiimagingextractor.py` & `roiextractors-0.5.2/src/roiextractors/multiimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/multisegmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/multisegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/segmentationextractor.py` & `roiextractors-0.5.2/src/roiextractors/segmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.1/src/roiextractors/testing.py` & `roiextractors-0.5.2/src/roiextractors/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     has_summary_images: bool = True,
     has_raw_signal: bool = True,
     has_dff_signal: bool = True,
     has_deconvolved_signal: bool = True,
     has_neuropil_signal: bool = True,
     rejected_list: Optional[list] = None,
 ) -> SegmentationExtractor:
-
     """
     A dummy segmentation extractor for testing. The segmentation extractor is built by feeding random data into the
     `NumpySegmentationExtractor`.
 
     Note that this dummy example is meant to be a mock object with the right shape, structure and objects but does not
     contain meaningful content. That is, the image masks matrices are not plausible image mask for a roi, the raw signal
     is not a meaningful biological signal and is not related appropriately to the deconvolved signal , etc.
```

### Comparing `roiextractors-0.5.1/src/roiextractors.egg-info/PKG-INFO` & `roiextractors-0.5.2/src/roiextractors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
 Author: Heberto Mayorquin, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
```

### Comparing `roiextractors-0.5.1/src/roiextractors.egg-info/SOURCES.txt` & `roiextractors-0.5.2/src/roiextractors.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,9 +36,11 @@
 src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
 src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
 src/roiextractors/extractors/simaextractor/__init__.py
 src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
 src/roiextractors/extractors/suite2p/__init__.py
 src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
 src/roiextractors/extractors/tiffimagingextractors/__init__.py
+src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
+src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
 src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
 src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
```

