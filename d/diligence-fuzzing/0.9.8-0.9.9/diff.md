# Comparing `tmp/diligence-fuzzing-0.9.8.tar.gz` & `tmp/diligence-fuzzing-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/diligence-fuzzing-0.9.8.tar", last modified: Thu Aug 25 07:47:58 2022, max compression
+gzip compressed data, was "dist/diligence-fuzzing-0.9.9.tar", last modified: Thu Aug 25 10:42:15 2022, max compression
```

## Comparing `diligence-fuzzing-0.9.8.tar` & `diligence-fuzzing-0.9.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/arm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/pytimer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/template.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/disarm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/faas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/fuzzing_lessons.py
--rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/generate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/brownie.py
--rw-r--r--   0 runner    (1001) docker     (121)     6707 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/dapptools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5617 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/hardhat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/truffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/lessons/
--rw-r--r--   0 runner    (1001) docker     (121)     4860 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/lessons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11494 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/pytimer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck_lib/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10024 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck_lib/quickcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck_lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9249 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/scribble.py
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/solidity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/ide.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/lessons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/fuzzing_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/interactive_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_arm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5883 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_disarm.py
--rw-r--r--   0 runner    (1001) docker     (121)    12900 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_generate_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_lessons.py
--rw-r--r--   0 runner    (1001) docker     (121)     5967 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_login.py
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_quickcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)    23447 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_fuzz_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    13115 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_get_corpus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_incremental_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/test_truffle_ide.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (121)   140639 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie-artifact.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    44175 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    17016 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)     6350 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/contracts.json
--rw-r--r--   0 runner    (1001) docker     (121)   321465 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/brownie_project/processed_payload.json
--rw-r--r--   0 runner    (1001) docker     (121)  1168713 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_artifact.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    35617 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    22639 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/contracts.json
--rw-r--r--   0 runner    (1001) docker     (121)   341683 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/processed_payload.json
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/ganache-all-blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat-artifact-different-contract-name.json
--rw-r--r--   0 runner    (1001) docker     (121)    51124 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat-artifact.json
--rw-r--r--   0 runner    (1001) docker     (121)     9625 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat-build-info-artifact-1.json
--rw-r--r--   0 runner    (1001) docker     (121)   239539 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat-build-info-artifact.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   147643 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     5576 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/contracts.json
--rw-r--r--   0 runner    (1001) docker     (121)    10547 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/lessons.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   175321 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    22847 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)    12056 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/contracts.json
--rw-r--r--   0 runner    (1001) docker     (121)   337261 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/processed_payload.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/
--rw-r--r--   0 runner    (1001) docker     (121)   144723 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)   144865 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts_annotated.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)   146248 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts_armed.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)   167783 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/combined_compilation_artifacts.json
--rw-r--r--   0 runner    (1001) docker     (121)   161762 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/combined_processed_payload.json
--rw-r--r--   0 runner    (1001) docker     (121)    90272 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/first_contract_compilation_artifacts.json
--rw-r--r--   0 runner    (1001) docker     (121)    86435 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/first_contract_processed_payload.json
--rw-r--r--   0 runner    (1001) docker     (121)    86897 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/second_contract_compilation_artifacts.json
--rw-r--r--   0 runner    (1001) docker     (121)    83148 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/second_contract_processed_payload.json
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/scribble_project/
--rw-r--r--   0 runner    (1001) docker     (121)   134079 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/scribble_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    27614 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle-artifact.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 07:47:58.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   200579 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/artifacts.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    27603 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/blocks.json
--rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/contracts.json
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)   343981 2022-08-25 07:47:37.000000 diligence-fuzzing-0.9.8/tests/testdata/truffle_project/processed_payload.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4387 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/arm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/pytimer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/disarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/faas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/fuzzing_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8583 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/generate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/brownie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6707 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/dapptools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5617 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/hardhat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/truffle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/lessons/
+-rw-r--r--   0 runner    (1001) docker     (121)     4860 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/lessons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11494 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/pytimer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck_lib/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10024 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck_lib/quickcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck_lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9249 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4689 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/scribble.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/solidity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/ide.py
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/lessons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/fuzzing_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/interactive_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_arm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5883 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_disarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12900 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5967 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_login.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_quickcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23615 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_fuzz_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13115 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_get_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_incremental_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/test_truffle_ide.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (121)   140639 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie-artifact.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    44175 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    17016 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6350 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/contracts.json
+-rw-r--r--   0 runner    (1001) docker     (121)   321465 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/brownie_project/processed_payload.json
+-rw-r--r--   0 runner    (1001) docker     (121)  1168713 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_artifact.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35617 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    22639 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/contracts.json
+-rw-r--r--   0 runner    (1001) docker     (121)   341683 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/processed_payload.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/ganache-all-blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat-artifact-different-contract-name.json
+-rw-r--r--   0 runner    (1001) docker     (121)    51124 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat-artifact.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9625 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat-build-info-artifact-1.json
+-rw-r--r--   0 runner    (1001) docker     (121)   239539 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat-build-info-artifact.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   147643 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     5576 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/contracts.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10547 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/lessons.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   175321 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    22847 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)    12056 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/contracts.json
+-rw-r--r--   0 runner    (1001) docker     (121)   337261 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/processed_payload.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/
+-rw-r--r--   0 runner    (1001) docker     (121)   144723 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   144865 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts_annotated.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   146248 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts_armed.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   167783 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/combined_compilation_artifacts.json
+-rw-r--r--   0 runner    (1001) docker     (121)   161762 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/combined_processed_payload.json
+-rw-r--r--   0 runner    (1001) docker     (121)    90272 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/first_contract_compilation_artifacts.json
+-rw-r--r--   0 runner    (1001) docker     (121)    86435 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/first_contract_processed_payload.json
+-rw-r--r--   0 runner    (1001) docker     (121)    86897 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/second_contract_compilation_artifacts.json
+-rw-r--r--   0 runner    (1001) docker     (121)    83148 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/second_contract_processed_payload.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/scribble_project/
+-rw-r--r--   0 runner    (1001) docker     (121)   134079 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/scribble_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    27614 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle-artifact.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 10:42:15.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   200579 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/artifacts.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    27603 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/contracts.json
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)   343981 2022-08-25 10:41:53.000000 diligence-fuzzing-0.9.9/tests/testdata/truffle_project/processed_payload.json
```

### Comparing `diligence-fuzzing-0.9.8/CONTRIBUTING.rst` & `diligence-fuzzing-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/HISTORY.rst` & `diligence-fuzzing-0.9.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/LICENSE` & `diligence-fuzzing-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/PKG-INFO` & `diligence-fuzzing-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diligence-fuzzing
-Version: 0.9.8
+Version: 0.9.9
 Summary: A command line interface for the Diligence Fuzzing API
 Home-page: https://github.com/ConsenSys/diligence-fuzzing
 Author: Dominik Muhs, João Santos
 Author-email: joao.santos@consensys.net
 License: Apache-2.0 License
 Keywords: diligence-fuzzing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `diligence-fuzzing-0.9.8/README.rst` & `diligence-fuzzing-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/PKG-INFO` & `diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diligence-fuzzing
-Version: 0.9.8
+Version: 0.9.9
 Summary: A command line interface for the Diligence Fuzzing API
 Home-page: https://github.com/ConsenSys/diligence-fuzzing
 Author: Dominik Muhs, João Santos
 Author-email: joao.santos@consensys.net
 License: Apache-2.0 License
 Keywords: diligence-fuzzing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `diligence-fuzzing-0.9.8/diligence_fuzzing.egg-info/SOURCES.txt` & `diligence-fuzzing-0.9.9/diligence_fuzzing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/cli.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/cli.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/arm.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/arm.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/options.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/options.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/pytimer.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/pytimer.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/template.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/template.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/config/utils.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/config/utils.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/disarm.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/disarm.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/exceptions.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/exceptions.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/faas.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/faas.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             "corpus": seed_state["analysis-setup"],
             "sources": campaign_data.sources,
             "contracts": campaign_data.contracts,
             "quickCheck": self.quick_check,
         }
 
         if self.project is not None:
-            api_payload["project"] = (self.project,)
+            api_payload["project"] = self.project
 
         if self.time_limit is not None:
             api_payload["timeLimit"] = self.time_limit
 
         try:
             instr_meta = ScribbleMixin.get_arming_instr_meta()
             if instr_meta is not None:
```

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/fuzzing_lessons.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/fuzzing_lessons.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/generate_config.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/generate_config.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/__init__.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/__init__.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/brownie.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/brownie.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/dapptools.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/dapptools.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/generic.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/generic.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/hardhat.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/hardhat.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/repository.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/repository.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/ide/truffle.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/ide/truffle.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/lessons/__init__.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/lessons/__init__.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/pytimer.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/pytimer.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/quickcheck_lib/quickcheck.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/quickcheck_lib/quickcheck.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/generic.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/generic.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/rpc/rpc.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/run.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/run.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/scribble.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/scribble.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/solidity.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/solidity.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/fuzz/types/rpc.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/fuzz/types/rpc.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/fuzzing_cli/util.py` & `diligence-fuzzing-0.9.9/fuzzing_cli/util.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/setup.py` & `diligence-fuzzing-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     keywords="diligence-fuzzing",
     name="diligence-fuzzing",
     packages=find_packages(exclude=["tests"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ConsenSys/diligence-fuzzing",
-    version="0.9.8",
+    version="0.9.9",
     zip_safe=False,
 )
```

### Comparing `diligence-fuzzing-0.9.8/tests/common.py` & `diligence-fuzzing-0.9.9/tests/common.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/conftest.py` & `diligence-fuzzing-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_arm.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_arm.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_disarm.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_disarm.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_generate_config.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_generate_config.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_lessons.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_lessons.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_login.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_login.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_quickcheck.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_quickcheck.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_fuzz_run.py` & `diligence-fuzzing-0.9.9/tests/test_fuzz_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,28 +323,33 @@
     )
 
     start_faas_campaign_mock.assert_not_called()
 
 
 @pytest.mark.parametrize("ide", [lazy_fixture("hardhat_project")])
 @pytest.mark.parametrize(
-    "corpus_target, time_limit",
-    [(None, None), ("cmp_9e931b147e7143a8b53041c708d5474e", "15mins")],
+    "corpus_target, time_limit, project",
+    [
+        (None, None, None),
+        ("cmp_9e931b147e7143a8b53041c708d5474e", "15mins", "Test Project 1"),
+    ],
 )
 def test_fuzz_parameters(
     tmp_path,
     ide: Dict[str, any],
     corpus_target: Optional[str],
     time_limit: Optional[str],
+    project: Optional[str],
 ):
     write_config(
         config_path=f"{tmp_path}/.fuzz.yml",
         base_path=str(tmp_path),
         **ide,
         time_limit=time_limit,
+        project=project,
     )
 
     IDE_NAME = ide["ide"]
     blocks = get_test_case(f"testdata/{IDE_NAME}_project/blocks.json")
     codes = {
         contract["address"].lower(): contract["deployedBytecode"]
         for contract in get_test_case(
@@ -372,14 +377,15 @@
     )
 
     start_faas_campaign_mock.assert_called_once()
     payload = start_faas_campaign_mock.call_args[0][0]
 
     assert payload["corpus"].get("target", None) == corpus_target
     assert payload.get("timeLimit", None) == (900 if time_limit else None)
+    assert payload.get("project", None) == project or None
 
 
 def test_rpc_not_running(tmp_path):
     write_config(base_path=str(tmp_path))
 
     with patch.object(requests, "request") as mocker:
         mocker.side_effect = RequestException()
```

### Comparing `diligence-fuzzing-0.9.8/tests/test_get_corpus.py` & `diligence-fuzzing-0.9.9/tests/test_get_corpus.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_incremental_fuzzing.py` & `diligence-fuzzing-0.9.9/tests/test_incremental_fuzzing.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/test_truffle_ide.py` & `diligence-fuzzing-0.9.9/tests/test_truffle_ide.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie-artifact.json` & `diligence-fuzzing-0.9.9/tests/testdata/brownie-artifact.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie_project/README.md` & `diligence-fuzzing-0.9.9/tests/testdata/brownie_project/README.md`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/brownie_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie_project/blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/brownie_project/blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie_project/contracts.json` & `diligence-fuzzing-0.9.9/tests/testdata/brownie_project/contracts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/brownie_project/processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/brownie_project/processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_artifact.json` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_artifact.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/README.md` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/README.md`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/contracts.json` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/contracts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/dapptools_project/processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/dapptools_project/processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/ganache-all-blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/ganache-all-blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat-artifact-different-contract-name.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat-artifact-different-contract-name.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat-artifact.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat-artifact.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat-build-info-artifact-1.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat-build-info-artifact-1.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat-build-info-artifact.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat-build-info-artifact.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/README.md` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/README.md`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/contracts.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/contracts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_fuzzing_lessons_project/lessons.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_fuzzing_lessons_project/lessons.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/README.md` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/README.md`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/contracts.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/contracts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/hardhat_project/processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/hardhat_project/processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts_annotated.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts_annotated.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/artifacts_armed.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/artifacts_armed.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/combined_compilation_artifacts.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/combined_compilation_artifacts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/combined_processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/combined_processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/first_contract_compilation_artifacts.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/first_contract_compilation_artifacts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/first_contract_processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/first_contract_processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/second_contract_compilation_artifacts.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/second_contract_compilation_artifacts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/second_contract_processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/second_contract_processed_payload.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/quickcheck_project/echidna/utils.py` & `diligence-fuzzing-0.9.9/tests/testdata/quickcheck_project/echidna/utils.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/scribble_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/scribble_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle-artifact.json` & `diligence-fuzzing-0.9.9/tests/testdata/truffle-artifact.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/README.md` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/README.md`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/artifacts.tar.gz` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/artifacts.tar.gz`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/blocks.json` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/blocks.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/contracts.json` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/contracts.json`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/mocks.py` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/mocks.py`

 * *Files identical despite different names*

### Comparing `diligence-fuzzing-0.9.8/tests/testdata/truffle_project/processed_payload.json` & `diligence-fuzzing-0.9.9/tests/testdata/truffle_project/processed_payload.json`

 * *Files identical despite different names*

