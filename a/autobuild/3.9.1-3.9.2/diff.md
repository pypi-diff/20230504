# Comparing `tmp/autobuild-3.9.1.tar.gz` & `tmp/autobuild-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobuild-3.9.1.tar", last modified: Fri Mar 31 20:40:39 2023, max compression
+gzip compressed data, was "/home/runner/work/autobuild/autobuild/dist/.tmp-mbl2th7a/autobuild-3.9.2.tar", last modified: Thu May  4 18:52:58 2023, max compression
```

## Comparing `autobuild-3.9.1.tar` & `autobuild-3.9.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.431591 autobuild-3.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.403591 autobuild-3.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-31 20:40:05.000000 autobuild-3.9.1/.github/dependabot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-31 20:40:05.000000 autobuild-3.9.1/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.403591 autobuild-3.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-31 20:40:05.000000 autobuild-3.9.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-31 20:40:05.000000 autobuild-3.9.1/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-31 20:40:05.000000 autobuild-3.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-31 20:40:05.000000 autobuild-3.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-31 20:40:05.000000 autobuild-3.9.1/BuildParams
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 20:40:05.000000 autobuild-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 20:40:05.000000 autobuild-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-31 20:40:39.431591 autobuild-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-31 20:40:05.000000 autobuild-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.411591 autobuild-3.9.1/autobuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/archive_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_installables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_source_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/autobuild_tool_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/build_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    33521 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/hash_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.415591 autobuild-3.9.1/autobuild/scm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/scm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/scm/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-03-31 20:40:05.000000 autobuild-3.9.1/autobuild/update.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.415591 autobuild-3.9.1/autobuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 20:40:39.000000 autobuild-3.9.1/autobuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 20:40:39.431591 autobuild-3.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-03-31 20:40:05.000000 autobuild-3.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.419592 autobuild-3.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/baseline_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/basetest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.419592 autobuild-3.9.1/tests/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/bin/autobuild
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/bin/autobuild.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.427591 autobuild-3.9.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/archive.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/archive.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/archive.tar.zst
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/archive.zip
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/argparse-1.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/autobuild-package-config.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/autobuild-package-disallowedpath-config.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/autobuild-package-missing-config.xml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bad_assignment
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bad_substitution
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bad_variable
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bingo-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.zst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.1-common-111.zip
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bogus-0.2-common-222.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/bongo-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/config_test_0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/config_test_1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/config_test_2.xml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/config_test_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/config_test_3.xml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/conflict-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/darwin
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/dependencies_test_packages.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/empty
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/good_variable
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/manifest_test_0.xml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/nolicense-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/nolicense-install.xml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/nometa-0.1-common-111.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/nourl-install.xml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/only_comments
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-conflict.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.427591 autobuild-3.9.1/tests/data/package-test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.427591 autobuild-3.9.1/tests/data/package-test/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-test/LICENSES/test1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-test/autobuild-package.xml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-test/file2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.427591 autobuild-3.9.1/tests/data/package-test/include/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-test/include/file1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.427591 autobuild-3.9.1/tests/data/package-test/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-test/lib/file3
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/package-update-install.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/packages-failures.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/data/packages-install.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 20:40:39.431591 autobuild-3.9.1/tests/executables/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/executables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/executables/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/executables/envtest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/executables/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_autobuild_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_build_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    40998 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_installables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_scm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_scm_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_source_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-31 20:40:05.000000 autobuild-3.9.1/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 18:52:24.000000 autobuild-3.9.2/.github/dependabot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 18:52:24.000000 autobuild-3.9.2/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-04 18:52:24.000000 autobuild-3.9.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-04 18:52:24.000000 autobuild-3.9.2/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 18:52:24.000000 autobuild-3.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 18:52:24.000000 autobuild-3.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 18:52:24.000000 autobuild-3.9.2/BuildParams
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 18:52:24.000000 autobuild-3.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 18:52:24.000000 autobuild-3.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-04 18:52:58.000000 autobuild-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 18:52:24.000000 autobuild-3.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/archive_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_installables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_source_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/autobuild_tool_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/build_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33521 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/hash_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/scm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/scm/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-04 18:52:24.000000 autobuild-3.9.2/autobuild/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 18:52:58.000000 autobuild-3.9.2/autobuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:52:58.000000 autobuild-3.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-04 18:52:24.000000 autobuild-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/baseline_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/basetest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/bin/autobuild
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/bin/autobuild.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/archive.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/archive.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/archive.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/archive.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/argparse-1.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/autobuild-package-config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/autobuild-package-disallowedpath-config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/autobuild-package-missing-config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bad_assignment
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bad_substitution
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bad_variable
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bingo-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.1-common-111.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bogus-0.2-common-222.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/bongo-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/config_test_0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/config_test_1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/config_test_2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/config_test_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/config_test_3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/conflict-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/darwin
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/dependencies_test_packages.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/empty
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/good_variable
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/manifest_test_0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/nolicense-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/nolicense-install.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/nometa-0.1-common-111.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/nourl-install.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/only_comments
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-conflict.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/data/package-test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/data/package-test/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-test/LICENSES/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-test/autobuild-package.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-test/file2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/data/package-test/include/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-test/include/file1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/data/package-test/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-test/lib/file3
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/package-update-install.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/packages-failures.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/data/packages-install.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:58.000000 autobuild-3.9.2/tests/executables/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/executables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/executables/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/executables/envtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/executables/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_autobuild_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_build_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_installables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_scm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_scm_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_source_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-04 18:52:24.000000 autobuild-3.9.2/tests/test_update.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `autobuild-3.9.1/.github/workflows/ci.yaml` & `autobuild-3.9.2/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     name: Test & Build
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.11"]
         include:
           - os: ubuntu-latest
+            python-version: "3.7"
+          - os: ubuntu-latest
             python-version: "3.8"
           - os: ubuntu-latest
             python-version: "3.9"
           - os: ubuntu-latest
             python-version: "3.10"
     env:
       OS: ${{ matrix.os }}
@@ -57,25 +59,24 @@
           name: dist-${{ matrix.os }}
           path: dist
 
   publish:
     name: Publish to PyPI
     needs: build
     runs-on: [ubuntu-latest]
+    permissions:
+      id-token: write
     if: github.event_name != 'pull_request'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: dist-ubuntu-latest
           path: dist
 
       - name: Test Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.SHARED_PYPI_TEST_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
 
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         if: startsWith(github.event.ref, 'refs/tags/v')
-        with:
-          password: ${{ secrets.SHARED_PYPI_TOKEN }}
```

### Comparing `autobuild-3.9.1/.github/workflows/cla.yaml` & `autobuild-3.9.2/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/LICENSE` & `autobuild-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/PKG-INFO` & `autobuild-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobuild
-Version: 3.9.1
+Version: 3.9.2
 Summary: Linden Lab Automated Package Management and Build System
 Home-page: http://wiki.secondlife.com/wiki/Autobuild
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `autobuild-3.9.1/README.md` & `autobuild-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/archive_utils.py` & `autobuild-3.9.2/autobuild/archive_utils.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_base.py` & `autobuild-3.9.2/autobuild/autobuild_base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_main.py` & `autobuild-3.9.2/autobuild/autobuild_main.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_build.py` & `autobuild-3.9.2/autobuild/autobuild_tool_build.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_configure.py` & `autobuild-3.9.2/autobuild/autobuild_tool_configure.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_edit.py` & `autobuild-3.9.2/autobuild/autobuild_tool_edit.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_graph.py` & `autobuild-3.9.2/autobuild/autobuild_tool_graph.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_install.py` & `autobuild-3.9.2/autobuild/autobuild_tool_install.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_installables.py` & `autobuild-3.9.2/autobuild/autobuild_tool_installables.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_manifest.py` & `autobuild-3.9.2/autobuild/autobuild_tool_manifest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_package.py` & `autobuild-3.9.2/autobuild/autobuild_tool_package.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_print.py` & `autobuild-3.9.2/autobuild/autobuild_tool_print.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_source_environment.py` & `autobuild-3.9.2/autobuild/autobuild_tool_source_environment.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/autobuild_tool_uninstall.py` & `autobuild-3.9.2/autobuild/autobuild_tool_uninstall.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/build_id.py` & `autobuild-3.9.2/autobuild/build_id.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/common.py` & `autobuild-3.9.2/autobuild/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,20 +322,20 @@
 
 
 def compute_hash(path: str, hash: Callable[[], hashlib._Hash]):
     """
     Compute a hash for a file effeciently by streaming it into the hash algorithm
     """
     h = hash()
-    b = bytearray(128*1024)
-    mv = memoryview(b)
     try:
         with open(path, 'rb') as f:
-            while n := f.readinto(mv):
-                h.update(mv[:n])
+            chunk = f.read(8192)
+            while chunk:
+                h.update(chunk)
+                chunk = f.read(8192)
             return h.hexdigest()
     except IOError as err:
         raise AutobuildError(f"Can't compute {h.name} for {path}: {err}")
 
 
 compute_md5 = partial(compute_hash, hash=hashlib.md5)
 compute_blake2b = partial(compute_hash, hash=hashlib.blake2b)
```

### Comparing `autobuild-3.9.1/autobuild/configfile.py` & `autobuild-3.9.2/autobuild/configfile.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/executable.py` & `autobuild-3.9.2/autobuild/executable.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/hash_algorithms.py` & `autobuild-3.9.2/autobuild/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/interactive.py` & `autobuild-3.9.2/autobuild/interactive.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/scm/base.py` & `autobuild-3.9.2/autobuild/scm/base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/scm/git.py` & `autobuild-3.9.2/autobuild/scm/git.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild/update.py` & `autobuild-3.9.2/autobuild/update.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/autobuild.egg-info/PKG-INFO` & `autobuild-3.9.2/autobuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobuild
-Version: 3.9.1
+Version: 3.9.2
 Summary: Linden Lab Automated Package Management and Build System
 Home-page: http://wiki.secondlife.com/wiki/Autobuild
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `autobuild-3.9.1/autobuild.egg-info/SOURCES.txt` & `autobuild-3.9.2/autobuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/setup.py` & `autobuild-3.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/baseline_compare.py` & `autobuild-3.9.2/tests/baseline_compare.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/basetest.py` & `autobuild-3.9.2/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/argparse-1.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/argparse-1.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/autobuild-package-config.xml` & `autobuild-3.9.2/tests/data/autobuild-package-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/autobuild-package-disallowedpath-config.xml` & `autobuild-3.9.2/tests/data/autobuild-package-disallowedpath-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/autobuild-package-missing-config.xml` & `autobuild-3.9.2/tests/data/autobuild-package-missing-config.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bingo-0.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/bingo-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.gz` & `autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.gz`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.xz` & `autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.xz`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.1-common-111.tar.zst` & `autobuild-3.9.2/tests/data/bogus-0.1-common-111.tar.zst`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.1-common-111.zip` & `autobuild-3.9.2/tests/data/bogus-0.1-common-111.zip`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bogus-0.2-common-222.tar.bz2` & `autobuild-3.9.2/tests/data/bogus-0.2-common-222.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/bongo-0.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/bongo-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/config_test_0.xml` & `autobuild-3.9.2/tests/data/config_test_0.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/config_test_1.xml` & `autobuild-3.9.2/tests/data/config_test_1.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/config_test_2.xml` & `autobuild-3.9.2/tests/data/config_test_2.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/config_test_3.txt` & `autobuild-3.9.2/tests/data/config_test_3.txt`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/config_test_3.xml` & `autobuild-3.9.2/tests/data/config_test_3.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/conflict-0.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/conflict-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/dependencies_test_packages.xml` & `autobuild-3.9.2/tests/data/dependencies_test_packages.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/manifest_test_0.xml` & `autobuild-3.9.2/tests/data/manifest_test_0.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/nolicense-0.1-common-111.tar.bz2` & `autobuild-3.9.2/tests/data/nolicense-0.1-common-111.tar.bz2`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/nolicense-install.xml` & `autobuild-3.9.2/tests/data/nolicense-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/nourl-install.xml` & `autobuild-3.9.2/tests/data/nourl-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/package-conflict.xml` & `autobuild-3.9.2/tests/data/package-conflict.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/package-test/autobuild-package.xml` & `autobuild-3.9.2/tests/data/package-test/autobuild-package.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/package-update-install.xml` & `autobuild-3.9.2/tests/data/package-update-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/packages-failures.xml` & `autobuild-3.9.2/tests/data/packages-failures.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/data/packages-install.xml` & `autobuild-3.9.2/tests/data/packages-install.xml`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/executables/__init__.py` & `autobuild-3.9.2/tests/executables/__init__.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/executables/envtest.py` & `autobuild-3.9.2/tests/executables/envtest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/patch.py` & `autobuild-3.9.2/tests/patch.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_autobuild_main.py` & `autobuild-3.9.2/tests/test_autobuild_main.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_build.py` & `autobuild-3.9.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_build_id.py` & `autobuild-3.9.2/tests/test_build_id.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_configfile.py` & `autobuild-3.9.2/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_configure.py` & `autobuild-3.9.2/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_edit.py` & `autobuild-3.9.2/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_executable.py` & `autobuild-3.9.2/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_filetype.py` & `autobuild-3.9.2/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_graph.py` & `autobuild-3.9.2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_install.py` & `autobuild-3.9.2/tests/test_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,34 +747,37 @@
 class TestDownloadPackage(unittest.TestCase):
     @patch("urllib.request.urlopen")
     def test_download(self, mock_urlopen: MagicMock):
         mock_urlopen.return_value = None
         with envvar("AUTOBUILD_GITHUB_TOKEN", None):
             autobuild_tool_install.download_package("https://example.org/foo.tar.bz2")
             mock_urlopen.assert_called()
-            got_req = mock_urlopen.mock_calls[0].args[0]
+            _, args, _ = mock_urlopen.mock_calls[0]
+            got_req = args[0]
             self.assertIsNone(got_req.unredirected_hdrs.get("Authorization"))
 
     @patch("urllib.request.urlopen")
     def test_download_github(self, mock_urlopen: MagicMock):
         mock_urlopen.return_value = None
         with envvar("AUTOBUILD_GITHUB_TOKEN", "token-123"):
             autobuild_tool_install.download_package("https://example.org/foo.tar.bz2", creds="github")
             mock_urlopen.assert_called()
-            got_req = mock_urlopen.mock_calls[0].args[0]
+            _, args, _ = mock_urlopen.mock_calls[0]
+            got_req = args[0]
             self.assertEqual(got_req.unredirected_hdrs["Authorization"], "Bearer token-123")
             self.assertEqual(got_req.unredirected_hdrs["Accept"], "application/octet-stream")
 
     @patch("urllib.request.urlopen")
     def test_download_gitlab(self, mock_urlopen: MagicMock):
         mock_urlopen.return_value = None
         with envvar("AUTOBUILD_GITLAB_TOKEN", "token-123"):
             autobuild_tool_install.download_package("https://example.org/foo.tar.bz2", creds="gitlab")
             mock_urlopen.assert_called()
-            got_req = mock_urlopen.mock_calls[0].args[0]
+            _, args, _ = mock_urlopen.mock_calls[0]
+            got_req = args[0]
             self.assertEqual(got_req.unredirected_hdrs["Authorization"], "Bearer token-123")
 
     @patch("urllib.request.urlopen")
     def test_download_github_without_creds(self, mock_urlopen: MagicMock):
         mock_urlopen.return_value = None
         with envvar("AUTOBUILD_GITHUB_TOKEN", None):
             with self.assertRaises(CredentialsNotFoundError):
```

### Comparing `autobuild-3.9.1/tests/test_installables.py` & `autobuild-3.9.2/tests/test_installables.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_manifest.py` & `autobuild-3.9.2/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_package.py` & `autobuild-3.9.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_scm_base.py` & `autobuild-3.9.2/tests/test_scm_base.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_scm_git.py` & `autobuild-3.9.2/tests/test_scm_git.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_source_environment.py` & `autobuild-3.9.2/tests/test_source_environment.py`

 * *Files identical despite different names*

### Comparing `autobuild-3.9.1/tests/test_update.py` & `autobuild-3.9.2/tests/test_update.py`

 * *Files identical despite different names*

