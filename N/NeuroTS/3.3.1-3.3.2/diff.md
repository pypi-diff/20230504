# Comparing `tmp/NeuroTS-3.3.1.tar.gz` & `tmp/NeuroTS-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroTS-3.3.1.tar", last modified: Mon Mar 13 12:46:34 2023, max compression
+gzip compressed data, was "NeuroTS-3.3.2.tar", last modified: Thu May  4 14:13:04 2023, max compression
```

## Comparing `NeuroTS-3.3.1.tar` & `NeuroTS-3.3.2.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.541914 NeuroTS-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.auto-changelog-template.hbs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.489912 NeuroTS-3.3.1/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.489912 NeuroTS-3.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.489912 NeuroTS-3.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/workflows/my_binder-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    34394 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.493912 NeuroTS-3.3.1/NeuroTS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-03-13 12:46:34.000000 NeuroTS-3.3.1/NeuroTS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-03-13 12:46:34.000000 NeuroTS-3.3.1/NeuroTS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 12:46:34.000000 NeuroTS-3.3.1/NeuroTS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-13 12:46:34.000000 NeuroTS-3.3.1/NeuroTS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 12:46:34.000000 NeuroTS-3.3.1/NeuroTS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-03-13 12:46:34.541914 NeuroTS-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.493912 NeuroTS-3.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.493912 NeuroTS-3.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.493912 NeuroTS-3.3.1/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (123)   422700 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/logo/BBP-NeuroTS.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/docs/source/params_and_distrs.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.497913 NeuroTS-3.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.497913 NeuroTS-3.3.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/IN_distr.json
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/IN_params.json
--rw-r--r--   0 runner    (1001) docker     (123)    46640 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/PC_distr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/PC_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/bio_distr.json
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/bio_params.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.497913 NeuroTS-3.3.1/examples/data/neurons/
--rw-r--r--   0 runner    (1001) docker     (123)    53792 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/neurons/C220197A-P2.h5
--rw-r--r--   0 runner    (1001) docker     (123)    95344 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/data/neurons/Fluo55_left.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/explore_example_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/extract_synthesis_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/synthesize_neuron_external_diameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/synthesize_neuron_with_diameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/synthesize_neurons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/examples/synthesize_single_neuron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.501912 NeuroTS-3.3.1/neurots/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.501912 NeuroTS-3.3.1/neurots/astrocyte/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/grower.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/section.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/space_colonization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/tmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/astrocyte/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.505913 NeuroTS-3.3.1/neurots/extract_input/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/from_TMD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/from_diameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/from_neurom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/input_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/extract_input/input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.505913 NeuroTS-3.3.1/neurots/generate/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.509913 NeuroTS-3.3.1/neurots/generate/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/abstractgrower.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/barcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/basicgrower.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/algorithms/tmdgrower.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/grower.py
--rw-r--r--   0 runner    (1001) docker     (123)    25036 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/orientations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/section.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/soma.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/generate/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.509913 NeuroTS-3.3.1/neurots/morphmath/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/point_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/morphmath/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.509913 NeuroTS-3.3.1/neurots/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/relevance_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/preprocess/validity_checkers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.513913 NeuroTS-3.3.1/neurots/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/schemas/distributions.json
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/schemas/parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/neurots/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 12:46:34.541914 NeuroTS-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.513913 NeuroTS-3.3.1/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.513913 NeuroTS-3.3.1/test_data/bio/
--rw-r--r--   0 runner    (1001) docker     (123)    53792 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/test_data/bio/C220197A-P2.h5
--rw-r--r--   0 runner    (1001) docker     (123)    95344 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/test_data/bio/Fluo55_left.h5
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/test_data/diam_simple.swc
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/test_data/diam_simple_axon.swc
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/test_data/simple.swc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.517913 NeuroTS-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.521913 NeuroTS-3.3.1/tests/astrocyte/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.521913 NeuroTS-3.3.1/tests/astrocyte/data/
--rw-r--r--   0 runner    (1001) docker     (123)   148560 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/data/astrocyte.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/data/bio_path_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/data/bio_path_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_endfeet_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_grower.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_space_colonization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_tmd_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/astrocyte/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.537913 NeuroTS-3.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/axon_trunk_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/axon_trunk_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/axon_trunk_parameters_absolute.json
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/axon_trunk_parameters_absolute_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/axon_trunk_parameters_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_distr_breaker.json
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)  1180345 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_distribution_3d_angles.json
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_distribution_apical_point.json
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_gradient_path_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_gradient_path_params_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_parameters_3d_angles.json
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_params_breaker.json
--rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_path_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_path_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_path_params_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_path_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_radial_params.json
--rw-r--r--   0 runner    (1001) docker     (123)   138315 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_rat_L5_TPC_B_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/bio_trunk_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)    29008 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_distribution_legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_interneuron_distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_neuron.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/dummy_params_legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params1.h5
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params1_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params2.h5
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params2_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params3.h5
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params3_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params4.h5
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params4_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)   147216 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/gradient_path_grower.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/gradient_path_persistence_diagram.json
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params1_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params2_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params3_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params4.json
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/params4_orientation_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)   147216 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/path_grower.h5
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/test_axon_grower.h5
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/test_axon_grower_absolute.h5
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/test_trunk_grower.h5
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/data/trunk_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_diametrizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    32161 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_extract_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_generate_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_generate_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_morphmath_bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_morphmath_point_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_morphmath_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_neuron_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_orientations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_soma_grower.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_tmd_synthesis_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:34.537913 NeuroTS-3.3.1/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/validation/boxplot_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-13 12:46:22.000000 NeuroTS-3.3.1/validation/violin_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.839645 NeuroTS-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.auto-changelog-template.hbs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.799645 NeuroTS-3.3.2/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.799645 NeuroTS-3.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.803645 NeuroTS-3.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/workflows/my_binder-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34808 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.803645 NeuroTS-3.3.2/NeuroTS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-04 14:13:04.000000 NeuroTS-3.3.2/NeuroTS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-04 14:13:04.000000 NeuroTS-3.3.2/NeuroTS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:13:04.000000 NeuroTS-3.3.2/NeuroTS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-04 14:13:04.000000 NeuroTS-3.3.2/NeuroTS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 14:13:04.000000 NeuroTS-3.3.2/NeuroTS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-04 14:13:04.839645 NeuroTS-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.803645 NeuroTS-3.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.807645 NeuroTS-3.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.807645 NeuroTS-3.3.2/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)   422700 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/logo/BBP-NeuroTS.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/docs/source/params_and_distrs.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.807645 NeuroTS-3.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.807645 NeuroTS-3.3.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/IN_distr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/IN_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46640 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/PC_distr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/PC_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/bio_distr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/bio_params.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.811645 NeuroTS-3.3.2/examples/data/neurons/
+-rw-r--r--   0 runner    (1001) docker     (123)    53792 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/neurons/C220197A-P2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    95344 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/data/neurons/Fluo55_left.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/explore_example_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/extract_synthesis_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/synthesize_neuron_external_diameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/synthesize_neuron_with_diameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/synthesize_neurons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/examples/synthesize_single_neuron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.811645 NeuroTS-3.3.2/neurots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.811645 NeuroTS-3.3.2/neurots/astrocyte/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/grower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/space_colonization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/tmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/astrocyte/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.811645 NeuroTS-3.3.2/neurots/extract_input/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/from_TMD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/from_diameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/from_neurom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/input_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/extract_input/input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/neurots/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/neurots/generate/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/abstractgrower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/basicgrower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/algorithms/tmdgrower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/grower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25036 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/orientations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/soma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/generate/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/neurots/morphmath/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/point_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/morphmath/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/neurots/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/relevance_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/preprocess/validity_checkers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/neurots/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/schemas/distributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/schemas/parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/neurots/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:13:04.839645 NeuroTS-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.815645 NeuroTS-3.3.2/test_data/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)    53792 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/test_data/bio/C220197A-P2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    95344 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/test_data/bio/Fluo55_left.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/test_data/diam_simple.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/test_data/diam_simple_axon.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/test_data/simple.swc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.819645 NeuroTS-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.823645 NeuroTS-3.3.2/tests/astrocyte/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.823645 NeuroTS-3.3.2/tests/astrocyte/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   148560 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/data/astrocyte.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/data/bio_path_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/data/bio_path_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_endfeet_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_grower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_space_colonization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_tmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/astrocyte/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.839645 NeuroTS-3.3.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/axon_trunk_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/axon_trunk_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/axon_trunk_parameters_absolute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/axon_trunk_parameters_absolute_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/axon_trunk_parameters_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_distr_breaker.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1180345 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_distribution_3d_angles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_distribution_apical_point.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_gradient_path_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_gradient_path_params_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_parameters_3d_angles.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_params_breaker.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_path_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_path_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_path_params_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_path_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_radial_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)   138315 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_rat_L5_TPC_B_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/bio_trunk_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29008 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_distribution_legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19472 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_interneuron_distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_neuron.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/dummy_params_legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params1_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params2_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params3.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params3_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235036 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params4.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params4_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147216 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/gradient_path_grower.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/gradient_path_persistence_diagram.json
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params1_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params2_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params3_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/params4_orientation_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147216 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/path_grower.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/test_axon_grower.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/test_axon_grower_absolute.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/test_trunk_grower.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/data/trunk_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_diametrizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33022 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_extract_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_generate_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_generate_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_morphmath_bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_morphmath_point_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_morphmath_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_neuron_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_orientations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_soma_grower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_tmd_synthesis_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:13:04.839645 NeuroTS-3.3.2/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/validation/boxplot_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-04 14:12:53.000000 NeuroTS-3.3.2/validation/violin_comparison.py
```

### Comparing `NeuroTS-3.3.1/.auto-changelog` & `NeuroTS-3.3.2/.auto-changelog`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.auto-changelog-template.hbs` & `NeuroTS-3.3.2/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.copier-answers.yml` & `NeuroTS-3.3.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.github/dependabot.yml` & `NeuroTS-3.3.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.github/workflows/codeql.yml` & `NeuroTS-3.3.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.github/workflows/commitlint.yml` & `NeuroTS-3.3.2/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.github/workflows/publish-sdist.yml` & `NeuroTS-3.3.2/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.github/workflows/run-tox.yml` & `NeuroTS-3.3.2/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.pre-commit-config.yaml` & `NeuroTS-3.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/.pylintrc` & `NeuroTS-3.3.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/CHANGELOG.md` & `NeuroTS-3.3.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## [3.3.2](https://github.com/BlueBrain/NeuroTS/compare/3.3.1..3.3.2)
+
+> 4 May 2023
+
+### Fixes
+
+- Raise clear errors for empty angles (Adrien Berchet - [#65](https://github.com/BlueBrain/NeuroTS/pull/65))
+
+## [3.3.1](https://github.com/BlueBrain/NeuroTS/compare/3.3.0..3.3.1)
+
+> 13 March 2023
+
+### Fixes
+
+- Convert apical_sections to new id (Alexis Arnaudon - [#60](https://github.com/BlueBrain/NeuroTS/pull/60))
+
 ## [3.3.0](https://github.com/BlueBrain/NeuroTS/compare/3.2.0..3.3.0)
 
 > 13 March 2023
 
 ### Build
 
 - Use find_namespace_packages instead of find_packages (Adrien Berchet - [#48](https://github.com/BlueBrain/NeuroTS/pull/48))
```

### Comparing `NeuroTS-3.3.1/CITATION.cff` & `NeuroTS-3.3.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/CONTRIBUTING.md` & `NeuroTS-3.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/LICENSE.txt` & `NeuroTS-3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/NeuroTS.egg-info/PKG-INFO` & `NeuroTS-3.3.2/NeuroTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroTS
-Version: 3.3.1
+Version: 3.3.2
 Summary: Synthesis of artificial neurons using their topological profiles package.
 Home-page: https://NeuroTS.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/NeuroTS/issues
 Project-URL: Source, https://github.com/BlueBrain/NeuroTS
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NeuroTS-3.3.1/NeuroTS.egg-info/SOURCES.txt` & `NeuroTS-3.3.2/NeuroTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/PKG-INFO` & `NeuroTS-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroTS
-Version: 3.3.1
+Version: 3.3.2
 Summary: Synthesis of artificial neurons using their topological profiles package.
 Home-page: https://NeuroTS.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/NeuroTS/issues
 Project-URL: Source, https://github.com/BlueBrain/NeuroTS
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NeuroTS-3.3.1/README.md` & `NeuroTS-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/commitlint.config.js` & `NeuroTS-3.3.2/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/docs/Makefile` & `NeuroTS-3.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/docs/source/conf.py` & `NeuroTS-3.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/docs/source/logo/BBP-NeuroTS.jpg` & `NeuroTS-3.3.2/docs/source/logo/BBP-NeuroTS.jpg`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/docs/source/params_and_distrs.rst` & `NeuroTS-3.3.2/docs/source/params_and_distrs.rst`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/IN_distr.json` & `NeuroTS-3.3.2/examples/data/IN_distr.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/IN_params.json` & `NeuroTS-3.3.2/examples/data/IN_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/PC_distr.json` & `NeuroTS-3.3.2/examples/data/PC_distr.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/PC_params.json` & `NeuroTS-3.3.2/examples/data/PC_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/bio_distr.json` & `NeuroTS-3.3.2/examples/data/bio_distr.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/bio_params.json` & `NeuroTS-3.3.2/examples/data/bio_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/neurons/C220197A-P2.h5` & `NeuroTS-3.3.2/examples/data/neurons/C220197A-P2.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/data/neurons/Fluo55_left.h5` & `NeuroTS-3.3.2/examples/data/neurons/Fluo55_left.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/explore_example_results.ipynb` & `NeuroTS-3.3.2/examples/explore_example_results.ipynb`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/extract_synthesis_inputs.py` & `NeuroTS-3.3.2/examples/extract_synthesis_inputs.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/synthesize_neuron_external_diameter.py` & `NeuroTS-3.3.2/examples/synthesize_neuron_external_diameter.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/synthesize_neuron_with_diameters.py` & `NeuroTS-3.3.2/examples/synthesize_neuron_with_diameters.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/synthesize_neurons.py` & `NeuroTS-3.3.2/examples/synthesize_neurons.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/examples/synthesize_single_neuron.py` & `NeuroTS-3.3.2/examples/synthesize_single_neuron.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/__init__.py` & `NeuroTS-3.3.2/neurots/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/__init__.py` & `NeuroTS-3.3.2/neurots/astrocyte/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/context.py` & `NeuroTS-3.3.2/neurots/astrocyte/context.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/grower.py` & `NeuroTS-3.3.2/neurots/astrocyte/grower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/point_cloud.py` & `NeuroTS-3.3.2/neurots/astrocyte/point_cloud.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/section.py` & `NeuroTS-3.3.2/neurots/astrocyte/section.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/space_colonization.py` & `NeuroTS-3.3.2/neurots/astrocyte/space_colonization.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/tmd_utils.py` & `NeuroTS-3.3.2/neurots/astrocyte/tmd_utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/astrocyte/tree.py` & `NeuroTS-3.3.2/neurots/astrocyte/tree.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/basic.py` & `NeuroTS-3.3.2/neurots/basic.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/extract_input/__init__.py` & `NeuroTS-3.3.2/neurots/extract_input/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/extract_input/from_TMD.py` & `NeuroTS-3.3.2/neurots/extract_input/from_TMD.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import tmd
 
+from neurots.utils import NeuroTSError
+
 
 def persistent_homology_angles(
     pop, threshold=2, neurite_type="basal_dendrite", feature="radial_distances"
 ):
     """Add the persistent homology extracted from a population of apicals to the distr dictionary.
 
     Each tree in the population is associated with a persistence barcode (diagram)
@@ -31,14 +33,21 @@
         threshold (int): The minimum number of terminations.
         neurite_type (neurom.core.types.NeuriteType): Consider only the neurites of this type.
         feature (str): Use the specified TMD feature.
     """
     ph_ang = [
         tmd.methods.get_ph_angles(tree, feature=feature) for tree in getattr(pop, neurite_type)
     ]
+    if not ph_ang:
+        raise NeuroTSError(f"The given population does contain any tree of {neurite_type} type.")
 
     # Keep only the trees whose number of terminations is above the threshold
     # Saves the list of persistence diagrams for the selected neurite_type
     phs = [p for p in ph_ang if len(p) > threshold]
+    if not phs:
+        raise NeuroTSError(
+            "The given threshold excluded all bars of the persistence diagram, please use a "
+            "lower threshold value."
+        )
     min_bar_length = min(min(tmd.analysis.get_lengths(ph)) for ph in phs)
 
     return {"persistence_diagram": phs, "min_bar_length": min_bar_length}
```

### Comparing `NeuroTS-3.3.1/neurots/extract_input/from_diameter.py` & `NeuroTS-3.3.2/neurots/extract_input/from_diameter.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/extract_input/from_neurom.py` & `NeuroTS-3.3.2/neurots/extract_input/from_neurom.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/extract_input/input_distributions.py` & `NeuroTS-3.3.2/neurots/extract_input/input_distributions.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/extract_input/input_parameters.py` & `NeuroTS-3.3.2/neurots/extract_input/input_parameters.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/__init__.py` & `NeuroTS-3.3.2/neurots/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/__init__.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/abstractgrower.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/abstractgrower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/barcode.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/barcode.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/basicgrower.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/basicgrower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/common.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/algorithms/tmdgrower.py` & `NeuroTS-3.3.2/neurots/generate/algorithms/tmdgrower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/diametrizer.py` & `NeuroTS-3.3.2/neurots/generate/diametrizer.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/grower.py` & `NeuroTS-3.3.2/neurots/generate/grower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/orientations.py` & `NeuroTS-3.3.2/neurots/generate/orientations.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/section.py` & `NeuroTS-3.3.2/neurots/generate/section.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/soma.py` & `NeuroTS-3.3.2/neurots/generate/soma.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/generate/tree.py` & `NeuroTS-3.3.2/neurots/generate/tree.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/__init__.py` & `NeuroTS-3.3.2/neurots/morphmath/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/bifurcation.py` & `NeuroTS-3.3.2/neurots/morphmath/bifurcation.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/point_array.py` & `NeuroTS-3.3.2/neurots/morphmath/point_array.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/rotation.py` & `NeuroTS-3.3.2/neurots/morphmath/rotation.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/sample.py` & `NeuroTS-3.3.2/neurots/morphmath/sample.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/morphmath/utils.py` & `NeuroTS-3.3.2/neurots/morphmath/utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/__init__.py` & `NeuroTS-3.3.2/neurots/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/exceptions.py` & `NeuroTS-3.3.2/neurots/preprocess/exceptions.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/preprocessors.py` & `NeuroTS-3.3.2/neurots/preprocess/preprocessors.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/relevance_checkers.py` & `NeuroTS-3.3.2/neurots/preprocess/relevance_checkers.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/utils.py` & `NeuroTS-3.3.2/neurots/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/preprocess/validity_checkers.py` & `NeuroTS-3.3.2/neurots/preprocess/validity_checkers.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/schemas/distributions.json` & `NeuroTS-3.3.2/neurots/schemas/distributions.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/schemas/parameters.json` & `NeuroTS-3.3.2/neurots/schemas/parameters.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/utils.py` & `NeuroTS-3.3.2/neurots/utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/neurots/validator.py` & `NeuroTS-3.3.2/neurots/validator.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/package.json` & `NeuroTS-3.3.2/package.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/pyproject.toml` & `NeuroTS-3.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/setup.py` & `NeuroTS-3.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,32 @@
 from pathlib import Path
 
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 reqs = [
     "jsonschema>=3.0.1",
-    "matplotlib>=3.2.1",
-    "morphio>=3.3.3,<4.0",
+    "matplotlib>=3.4",
+    "morphio>=3.3.4,<4.0",
     "neurom>=3.0,<4.0",
     "numpy>=1.22.0",
     "scipy>=1.6",
-    "tmd>=2.2.0",
-    "diameter-synthesis>=0.5.2",
+    "tmd>=2.3.0",
+    "diameter-synthesis>=0.5.4",
 ]
 
 doc_reqs = [
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
     "sphinx-gallery",
     "sphinx-jsonschema",
 ]
 
 test_reqs = [
-    "diameter-synthesis>=0.5.0",
     "dictdiffer>=0.5",
     "mock>=3",
     "morph-tool>=2.9",
     "pytest>=6",
     "pytest-cov>=3",
     "pytest-html>=2",
     "pytest-xdist>=2",
```

### Comparing `NeuroTS-3.3.1/test_data/bio/C220197A-P2.h5` & `NeuroTS-3.3.2/test_data/bio/C220197A-P2.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/test_data/bio/Fluo55_left.h5` & `NeuroTS-3.3.2/test_data/bio/Fluo55_left.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/test_data/diam_simple_axon.swc` & `NeuroTS-3.3.2/test_data/diam_simple_axon.swc`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/test_data/simple.swc` & `NeuroTS-3.3.2/test_data/simple.swc`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/__init__.py` & `NeuroTS-3.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/__init__.py` & `NeuroTS-3.3.2/tests/astrocyte/__init__.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/data/astrocyte.h5` & `NeuroTS-3.3.2/tests/astrocyte/data/astrocyte.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/data/bio_path_distribution.json` & `NeuroTS-3.3.2/tests/astrocyte/data/bio_path_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/data/bio_path_params.json` & `NeuroTS-3.3.2/tests/astrocyte/data/bio_path_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_context.py` & `NeuroTS-3.3.2/tests/astrocyte/test_context.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_endfeet_targets.py` & `NeuroTS-3.3.2/tests/astrocyte/test_endfeet_targets.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_grower.py` & `NeuroTS-3.3.2/tests/astrocyte/test_grower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_point_cloud.py` & `NeuroTS-3.3.2/tests/astrocyte/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_section.py` & `NeuroTS-3.3.2/tests/astrocyte/test_section.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_space_colonization.py` & `NeuroTS-3.3.2/tests/astrocyte/test_space_colonization.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_tmd_utils.py` & `NeuroTS-3.3.2/tests/astrocyte/test_tmd_utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/astrocyte/test_tree.py` & `NeuroTS-3.3.2/tests/astrocyte/test_tree.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/axon_trunk_distribution.json` & `NeuroTS-3.3.2/tests/data/axon_trunk_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/axon_trunk_parameters.json` & `NeuroTS-3.3.2/tests/data/axon_trunk_parameters.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/axon_trunk_parameters_absolute.json` & `NeuroTS-3.3.2/tests/data/axon_trunk_parameters_absolute.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/axon_trunk_parameters_absolute_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/axon_trunk_parameters_absolute_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/axon_trunk_parameters_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/axon_trunk_parameters_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_distr_breaker.json` & `NeuroTS-3.3.2/tests/data/bio_distr_breaker.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_distribution.json` & `NeuroTS-3.3.2/tests/data/bio_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_distribution_3d_angles.json` & `NeuroTS-3.3.2/tests/data/bio_distribution_3d_angles.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_distribution_apical_point.json` & `NeuroTS-3.3.2/tests/data/bio_distribution_apical_point.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_gradient_path_params.json` & `NeuroTS-3.3.2/tests/data/bio_gradient_path_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_gradient_path_params_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/bio_gradient_path_params_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_parameters_3d_angles.json` & `NeuroTS-3.3.2/tests/data/bio_parameters_3d_angles.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_params_breaker.json` & `NeuroTS-3.3.2/tests/data/bio_params_breaker.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_path_distribution.json` & `NeuroTS-3.3.2/tests/data/bio_path_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_path_params.json` & `NeuroTS-3.3.2/tests/data/bio_path_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_path_params_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/bio_path_params_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_path_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/bio_path_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_radial_params.json` & `NeuroTS-3.3.2/tests/data/bio_radial_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_rat_L5_TPC_B_distribution.json` & `NeuroTS-3.3.2/tests/data/bio_rat_L5_TPC_B_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/bio_trunk_distribution.json` & `NeuroTS-3.3.2/tests/data/bio_trunk_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_distribution.json` & `NeuroTS-3.3.2/tests/data/dummy_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_distribution_legacy.json` & `NeuroTS-3.3.2/tests/data/dummy_distribution_legacy.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_interneuron_distribution.json` & `NeuroTS-3.3.2/tests/data/dummy_interneuron_distribution.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_neuron.asc` & `NeuroTS-3.3.2/tests/data/dummy_neuron.asc`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_params.json` & `NeuroTS-3.3.2/tests/data/dummy_params.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/dummy_params_legacy.json` & `NeuroTS-3.3.2/tests/data/dummy_params_legacy.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params1.h5` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params1.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params1_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params1_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params2.h5` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params2.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params2_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params2_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params3.h5` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params3.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params3_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params3_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params4.h5` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params4.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/expected_bio_rat_L5_TPC_B_with_params4_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/expected_bio_rat_L5_TPC_B_with_params4_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/gradient_path_grower.h5` & `NeuroTS-3.3.2/tests/data/gradient_path_grower.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/gradient_path_persistence_diagram.json` & `NeuroTS-3.3.2/tests/data/gradient_path_persistence_diagram.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params1.json` & `NeuroTS-3.3.2/tests/data/params1.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params1_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/params1_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params2.json` & `NeuroTS-3.3.2/tests/data/params2.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params2_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/params2_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params3.json` & `NeuroTS-3.3.2/tests/data/params3.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params3_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/params3_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params4.json` & `NeuroTS-3.3.2/tests/data/params4.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/params4_orientation_manager.json` & `NeuroTS-3.3.2/tests/data/params4_orientation_manager.json`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/path_grower.h5` & `NeuroTS-3.3.2/tests/data/path_grower.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/test_axon_grower.h5` & `NeuroTS-3.3.2/tests/data/test_axon_grower.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/test_axon_grower_absolute.h5` & `NeuroTS-3.3.2/tests/data/test_axon_grower_absolute.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/data/test_trunk_grower.h5` & `NeuroTS-3.3.2/tests/data/test_trunk_grower.h5`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_algo.py` & `NeuroTS-3.3.2/tests/test_algo.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_diametrizer.py` & `NeuroTS-3.3.2/tests/test_diametrizer.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_examples.py` & `NeuroTS-3.3.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_extract_input.py` & `NeuroTS-3.3.2/tests/test_extract_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,39 @@
         validator.validate_neuron_distribs(distr)
 
     def test_path_distances(self, filename):
         distr = extract_input.distributions(filename, feature="path_distances")
         assert_equal(distr["basal_dendrite"]["filtration_metric"], "path_distances")
         validator.validate_neuron_distribs(distr)
 
+    def test_threshold_too_small(self):
+        with pytest.raises(
+            NeuroTSError,
+            match=(
+                "The given threshold excluded all bars of the persistence diagram, please use a "
+                "lower threshold value."
+            ),
+        ):
+            extract_input.distributions(
+                os.path.join(_PATH, "diam_simple.swc"),
+                feature="path_distances",
+                neurite_types=["basal_dendrite"],
+            )
+
+    def test_missing_neurite_type(self):
+        with pytest.raises(
+            NeuroTSError,
+            match="The given population does contain any tree of axon type.",
+        ):
+            extract_input.distributions(
+                os.path.join(_PATH, "diam_simple.swc"),
+                feature="path_distances",
+                neurite_types=["axon"],
+            )
+
     def test_trunk_length(self, filename):
         distr = extract_input.distributions(filename, feature="trunk_length")
         assert "persistence_diagram" not in distr["basal_dendrite"]
         assert "filtration_metric" not in distr["basal_dendrite"]
         validator.validate_neuron_distribs(distr)
 
     def test_different_features(self, filename):
```

### Comparing `NeuroTS-3.3.1/tests/test_generate_section.py` & `NeuroTS-3.3.2/tests/test_generate_section.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_generate_tree.py` & `NeuroTS-3.3.2/tests/test_generate_tree.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_json_schema.py` & `NeuroTS-3.3.2/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_morphmath_bifurcation.py` & `NeuroTS-3.3.2/tests/test_morphmath_bifurcation.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_morphmath_point_array.py` & `NeuroTS-3.3.2/tests/test_morphmath_point_array.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_morphmath_utils.py` & `NeuroTS-3.3.2/tests/test_morphmath_utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_neuron_functional.py` & `NeuroTS-3.3.2/tests/test_neuron_functional.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_orientations.py` & `NeuroTS-3.3.2/tests/test_orientations.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_preprocess.py` & `NeuroTS-3.3.2/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_rotation.py` & `NeuroTS-3.3.2/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_sample.py` & `NeuroTS-3.3.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_soma_grower.py` & `NeuroTS-3.3.2/tests/test_soma_grower.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_tmd_synthesis_functionality.py` & `NeuroTS-3.3.2/tests/test_tmd_synthesis_functionality.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_utils.py` & `NeuroTS-3.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tests/test_validator.py` & `NeuroTS-3.3.2/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/tox.ini` & `NeuroTS-3.3.2/tox.ini`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/validation/boxplot_comparison.py` & `NeuroTS-3.3.2/validation/boxplot_comparison.py`

 * *Files identical despite different names*

### Comparing `NeuroTS-3.3.1/validation/violin_comparison.py` & `NeuroTS-3.3.2/validation/violin_comparison.py`

 * *Files identical despite different names*

