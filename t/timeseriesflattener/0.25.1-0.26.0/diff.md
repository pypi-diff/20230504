# Comparing `tmp/timeseriesflattener-0.25.1.tar.gz` & `tmp/timeseriesflattener-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-0.25.1.tar", last modified: Tue May  2 09:05:59 2023, max compression
+gzip compressed data, was "timeseriesflattener-0.26.0.tar", last modified: Thu May  4 07:54:51 2023, max compression
```

## Comparing `timeseriesflattener-0.25.1.tar` & `timeseriesflattener-0.26.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.032437 timeseriesflattener-0.25.1/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.000437 timeseriesflattener-0.25.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:58.996436 timeseriesflattener-0.25.1/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.000437 timeseriesflattener-0.25.1/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.000437 timeseriesflattener-0.25.1/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.004437 timeseriesflattener-0.25.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      877 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    54022 2023-05-02 09:05:49.000000 timeseriesflattener-0.25.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/Makefile
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-02 09:05:59.032437 timeseriesflattener-0.25.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/README.md
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.004437 timeseriesflattener-0.25.1/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.004437 timeseriesflattener-0.25.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.008437 timeseriesflattener-0.25.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   130812 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    68248 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    77800 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.008437 timeseriesflattener-0.25.1/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.008437 timeseriesflattener-0.25.1/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-02 09:05:49.000000 timeseriesflattener-0.25.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 09:05:59.032437 timeseriesflattener-0.25.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:58.996436 timeseriesflattener-0.25.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/cache_to_disk.py
--rw-r--r--   0 root         (0) root         (0)    40328 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     5387 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/resolve_multiple_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3168 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/testing/load_synth_data.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/testing/utils_for_testing.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/src/timeseriesflattener/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-02 09:05:58.000000 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3857 2023-05-02 09:05:58.000000 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:05:58.000000 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-02 09:05:58.000000 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-02 09:05:58.000000 timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9157 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:58.996436 timeseriesflattener-0.25.1/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:58.996436 timeseriesflattener-0.25.1/tests/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.012437 timeseriesflattener-0.25.1/tests/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.016437 timeseriesflattener-0.25.1/tests/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.028437 timeseriesflattener-0.25.1/tests/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      779 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_data/raw/synth_text_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.028437 timeseriesflattener-0.25.1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.028437 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7778 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:05:59.028437 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     6598 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)    16795 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_resolve_multiple.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-02 09:05:48.000000 timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:50.998711 timeseriesflattener-0.26.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      896 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/cruft.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      877 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    54558 2023-05-04 07:54:41.000000 timeseriesflattener-0.26.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.006712 timeseriesflattener-0.26.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   811066 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   130812 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    68248 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    77800 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      370 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)    49714 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-04 07:54:41.000000 timeseriesflattener-0.26.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.010712 timeseriesflattener-0.26.0/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+-rw-r--r--   0 root         (0) root         (0)    43524 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/feature_spec_objects.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/resolve_multiple_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/load_synth_data.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/testing/utils_for_testing.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/text_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/src/timeseriesflattener/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11584 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-04 07:54:50.000000 timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9179 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/tests/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.002712 timeseriesflattener-0.26.0/tests/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.014711 timeseriesflattener-0.26.0/tests/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   248865 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_data/raw/synth_text_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.026712 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 07:54:51.030712 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     6598 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16795 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_resolve_multiple.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-04 07:54:40.000000 timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_utils.py
```

### Comparing `timeseriesflattener-0.25.1/.cruft.json` & `timeseriesflattener-0.26.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/actions/test/action.yml` & `timeseriesflattener-0.26.0/.github/actions/test/action.yml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
       with:
         path: |
           .tox
         key: ${{ runner.os }}-${{ matrix.python-version }}
 
     - name: Set up Python
       uses: actions/setup-python@v4
-      if: steps.cache_tox.outputs.cache-hit != 'true'
       with:
         python-version: ${{ inputs.python-version }}
 
     - name: Install dependencies
       shell: bash
       run: |
         pip install invoke tox
```

### Comparing `timeseriesflattener-0.25.1/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-0.26.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/dependabot.yml` & `timeseriesflattener-0.26.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/recommended_repo_setup.md` & `timeseriesflattener-0.26.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/check_for_rej.yml` & `timeseriesflattener-0.26.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/cruft.yml` & `timeseriesflattener-0.26.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-0.26.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/documentation.yml` & `timeseriesflattener-0.26.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-0.26.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-0.26.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/pre-commit.yml` & `timeseriesflattener-0.26.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/stalebot.yml` & `timeseriesflattener-0.26.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.github/workflows/static_type_checks.yml` & `timeseriesflattener-0.26.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.gitignore` & `timeseriesflattener-0.26.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.pre-commit-config.yaml` & `timeseriesflattener-0.26.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/.zenodo.json` & `timeseriesflattener-0.26.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/CHANGELOG.md` & `timeseriesflattener-0.26.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.26.0 (2023-05-04)
+### Feature
+* Add group spec for text predictor spec ([`75a0112`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/75a0112f7c2717d16e1996d5087d993ba7f75cc4))
+
+### Fix
+* Update type hints ([`887bc06`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/887bc062bf970690077fea105b5ca77018049e6d))
+* Incorrect naming of resolve_multiple_fn ([`0a4607e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0a4607ee48e9dd6227205bca09ab123b6d30504a))
+
 ## v0.25.1 (2023-05-02)
 ### Fix
 * Bump version to generate new release ([`2316b38`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/2316b388aa71573aceeeba3f899037a93c71cb4f))
 
 ## v0.25.0 (2023-04-26)
 ### Feature
 * Add type-token-ratio resolve multiple fn ([`12be531`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/12be531382e1702fe21d9698dfa3ecaf256be8bb))
```

### Comparing `timeseriesflattener-0.25.1/CODE_OF_CONDUCT.md` & `timeseriesflattener-0.26.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/CONTRIBUTING.md` & `timeseriesflattener-0.26.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/LICENSE` & `timeseriesflattener-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/PKG-INFO` & `timeseriesflattener-0.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.25.1
+Version: 0.26.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.25.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.26.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.25.1/README.md` & `timeseriesflattener-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/citation.cff` & `timeseriesflattener-0.26.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/Makefile` & `timeseriesflattener-0.26.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/_static/favicon.ico` & `timeseriesflattener-0.26.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/_static/icon.png` & `timeseriesflattener-0.26.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/_static/icon_dark.png` & `timeseriesflattener-0.26.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/_static/terminology_figure.png` & `timeseriesflattener-0.26.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/conf.py` & `timeseriesflattener-0.26.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/faq.rst` & `timeseriesflattener-0.26.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/index.rst` & `timeseriesflattener-0.26.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-0.26.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-0.26.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/03_text.ipynb` & `timeseriesflattener-0.26.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/img/term_a.png` & `timeseriesflattener-0.26.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/img/term_b.png` & `timeseriesflattener-0.26.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/img/term_c.png` & `timeseriesflattener-0.26.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/docs/tutorials/img/term_d.png` & `timeseriesflattener-0.26.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/icon.png` & `timeseriesflattener-0.26.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/paper/paper.bib` & `timeseriesflattener-0.26.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/paper/paper.md` & `timeseriesflattener-0.26.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/pyproject.toml` & `timeseriesflattener-0.26.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "0.25.1"
+version = "0.26.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
```

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/feature_spec_objects.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/feature_spec_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -994,7 +994,74 @@
 
     def create_combinations(self) -> List[OutcomeSpec]:
         """Create all combinations from the group spec."""
         return create_specs_from_group(  # type: ignore
             feature_group_spec=self,
             output_class=OutcomeSpec,  # type: ignore
         )
+
+
+class TextPredictorGroupSpec(PredictorGroupSpec):
+    """Specification for a group of text predictors.
+    Fields:
+        values_loader (Optional[Sequence[str]]):
+            Loader for the df. Tries to resolve from the data_loaders
+            registry, then calls the function which should return a dataframe.
+        values_name (Optional[List[str]]):
+            List of strings that corresponds to a key in a dictionary
+            of multiple dataframes that correspods to a name of a type of values.
+        values_df (Optional[DataFrame]):
+            Dataframe with the values.
+        input_col_name_override (Optional[str]):
+            Override for the column name to use as values in df.
+        output_col_name_override (Optional[str]):
+            Override for the column name to use as values in the
+            output df.
+        resolve_multiple_fn (List[Union[Callable, str]]):
+            A function used for resolving multiple values within the
+            interval_days, i.e. how to combine texts within the lookbehind window.
+            Defaults to: 'concatenate'. Other possible options are 'latest' and
+            'earliest'.
+        fallback (Sequence[Union[Callable, str, float]]):
+            Which value to use if no values are found within interval_days.
+        allowed_nan_value_prop (List[float]):
+            If NaN is higher than this in the input dataframe during
+            resolution, raise an error. Defaults to: [0.0].
+        prefix (str):
+            Prefix for column name, e,g, <prefix>_<feature_name>. Defaults to: pred.
+        loader_kwargs (Optional[List[Dict[str, Any]]]):
+            Optional kwargs for the values_loader.
+        lookbehind_days (List[float]):
+            How far behind to look for values
+        embedding_fn (List[Callable]):
+            A function used for embedding the text. Should take a
+        pandas series of strings and return a pandas dataframe of embeddings.
+        embedding_fn_kwargs (Optional[List[dict]]):
+            Optional kwargs passed onto the embedding_fn.
+    """
+
+    class Doc:
+        short_description = """Specification for a group of text predictors."""
+
+    embedding_fn: List[Callable] = Field(
+        description="""A function used for embedding the text. Should take a
+        pandas series of strings and return a pandas dataframe of embeddings.
+        Defaults to: None.""",
+    )
+    embedding_fn_kwargs: Optional[List[dict]] = Field(
+        default=None,
+        description="""Optional kwargs passed onto the embedding_fn.""",
+    )
+    resolve_multiple_fn: List[Union[Callable, str]] = Field(
+        default=["concatenate"],
+        description="""A function used for resolving multiple values within the
+        interval_days, i.e. how to combine texts within the lookbehind window.
+        Defaults to: 'concatenate'. Other possible options are 'latest' and
+        'earliest'.""",
+    )
+
+    def create_combinations(self) -> List[TextPredictorSpec]:
+        """Create all combinations from the group spec."""
+        return create_specs_from_group(  # type: ignore
+            feature_group_spec=self,
+            output_class=TextPredictorSpec,  # type: ignore
+        )
```

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/logger.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/resolve_multiple_functions.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/resolve_multiple_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     return grouped_df.apply(
         lambda x: Series(
             {"value": " ".join(x.value)},
         ),
     )
 
 
-@resolve_multiple_fns.register("mean_len")
+@resolve_multiple_fns.register("mean_number_of_characters")
 def mean_number_of_characters(grouped_df: DataFrame) -> DataFrame:
     """Returns the mean length of values. This is useful for text data.
 
     Args:
         grouped_df (DataFrame): A dataframe sorted by descending timestamp, grouped by citizen.
 
     Returns:
```

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener/utils.py` & `timeseriesflattener-0.26.0/src/timeseriesflattener/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.25.1
+Version: 0.26.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.25.1 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.26.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-0.26.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tasks.py` & `timeseriesflattener-0.26.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
             line_sans_prefix = line[line.find("test_") :]
 
             # Keep only that after ::
             line_sans_suffix = line_sans_prefix[line_sans_prefix.find("::") + 2 :]
             print(f"FAILED {Emo.FAIL} #{line_sans_suffix}     ")
 
     if test_result.return_code != 0:
-        exit(0)
+        exit(test_result.return_code)
 
 
 def test_for_rej():
     # Get all paths in current directory or subdirectories that end in .rej
     rej_files = list(Path(".").rglob("*.rej"))
 
     if len(rej_files) > 0:
```

### Comparing `timeseriesflattener-0.25.1/tests/conftest.py` & `timeseriesflattener-0.26.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-0.26.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-0.26.0/tests/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-0.26.0/tests/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-0.26.0/tests/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/create_synth_sex.py` & `timeseriesflattener-0.26.0/tests/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_sex.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_data/raw/synth_text_data.csv` & `timeseriesflattener-0.26.0/tests/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-0.26.0/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 from timeseriesflattener.feature_spec_objects import (
     BaseModel,
     OutcomeGroupSpec,
     OutcomeSpec,
     PredictorGroupSpec,
     PredictorSpec,
     TemporalSpec,
+    TextPredictorGroupSpec,
     TextPredictorSpec,
     _AnySpec,
     check_that_col_names_in_kwargs_exist_in_df,
     generate_docstring_from_attributes,
 )
 from timeseriesflattener.resolve_multiple_functions import maximum
 from timeseriesflattener.testing.load_synth_data import (
     load_synth_predictor_float,
+    load_synth_text,
     synth_predictor_binary,
 )
+from timeseriesflattener.testing.text_embedding_functions import bow_test_embedding
+from timeseriesflattener.text_embedding_functions import sklearn_embedding
 from timeseriesflattener.utils import split_df_and_register_to_dict
 
 
 def test_anyspec_init():
     """Test that AnySpec initialises correctly."""
     values_loader_name = "synth_predictor_float"
 
@@ -245,7 +249,33 @@
         lookbehind_days=[10],
     )
 
     combinations = spec.create_combinations()
 
     pd.testing.assert_frame_equal(binary_100_rows, combinations[0].values_df)
     pd.testing.assert_frame_equal(float_100_rows, combinations[1].values_df)
+
+
+def test_textpredictorgroupspec_combinations_loader_kwargs():
+    """Test that loader kwargs are used correctly in TextPredictorGroupSpec combinations."""
+
+    text_10_rows = load_synth_text(n_rows=10)
+    text_100_rows = load_synth_text(n_rows=100)
+
+    df = load_synth_text()
+    bow_model = bow_test_embedding(df["text"])
+
+    spec = TextPredictorGroupSpec(
+        values_loader=("synth_text",),
+        loader_kwargs=[{"n_rows": 10}, {"n_rows": 100}],
+        prefix="test_",
+        resolve_multiple_fn=["concatenate"],
+        fallback=[0],
+        lookbehind_days=[10],
+        embedding_fn=[sklearn_embedding],
+        embedding_fn_kwargs=[{"model": bow_model}],
+    )
+
+    combinations = spec.create_combinations()
+
+    pd.testing.assert_frame_equal(text_10_rows, combinations[0].values_df)
+    pd.testing.assert_frame_equal(text_100_rows, combinations[1].values_df)
```

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_resolve_multiple.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_resolve_multiple.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.25.1/tests/test_timeseriesflattener/test_utils.py` & `timeseriesflattener-0.26.0/tests/test_timeseriesflattener/test_utils.py`

 * *Files identical despite different names*

