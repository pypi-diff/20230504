# Comparing `tmp/scmrepo-1.0.2.tar.gz` & `tmp/scmrepo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-1.0.2.tar", last modified: Tue Apr 18 08:01:26 2023, max compression
+gzip compressed data, was "scmrepo-1.0.3.tar", last modified: Thu May  4 08:20:10 2023, max compression
```

## Comparing `scmrepo-1.0.2.tar` & `scmrepo-1.0.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.903019 scmrepo-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.895018 scmrepo-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.895018 scmrepo-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-18 08:01:03.000000 scmrepo-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-18 08:01:03.000000 scmrepo-1.0.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 08:01:03.000000 scmrepo-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-18 08:01:03.000000 scmrepo-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-18 08:01:26.903019 scmrepo-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-18 08:01:03.000000 scmrepo-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-18 08:01:03.000000 scmrepo-1.0.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-18 08:01:03.000000 scmrepo-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-18 08:01:26.903019 scmrepo-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.895018 scmrepo-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-18 08:01:03.000000 scmrepo-1.0.2/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.899019 scmrepo-1.0.2/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 08:01:26.000000 scmrepo-1.0.2/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.903019 scmrepo-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:26.903019 scmrepo-1.0.2/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-18 08:01:03.000000 scmrepo-1.0.2/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.903702 scmrepo-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.903702 scmrepo-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 08:19:43.000000 scmrepo-1.0.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-04 08:19:43.000000 scmrepo-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 08:19:43.000000 scmrepo-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 08:20:10.911702 scmrepo-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-04 08:19:43.000000 scmrepo-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 08:19:43.000000 scmrepo-1.0.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-04 08:19:43.000000 scmrepo-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 08:20:10.911702 scmrepo-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.899701 scmrepo-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/user.key.pub
```

### Comparing `scmrepo-1.0.2/.cruft.json` & `scmrepo-1.0.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/.github/dependabot.yml` & `scmrepo-1.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/.github/workflows/release.yaml` & `scmrepo-1.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/.github/workflows/tests.yaml` & `scmrepo-1.0.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/.gitignore` & `scmrepo-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/.pre-commit-config.yaml` & `scmrepo-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/CODE_OF_CONDUCT.rst` & `scmrepo-1.0.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/CONTRIBUTING.rst` & `scmrepo-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/LICENSE` & `scmrepo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/PKG-INFO` & `scmrepo-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.2
+Version: 1.0.3
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.2/README.rst` & `scmrepo-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/noxfile.py` & `scmrepo-1.0.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/pyproject.toml` & `scmrepo-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/setup.cfg` & `scmrepo-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 python_requires = >=3.8
 zip_safe = False
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	gitpython>3
-	dulwich>=0.20.49
+	dulwich>=0.21.5
 	pygit2>=1.10.0
 	pygtrie>=2.3.2
 	fsspec>=2021.7.0
 	pathspec>=0.9.0
 	asyncssh>=2.13.1,<3
 	funcy>=1.14
 	shortuuid>=0.5.0
```

### Comparing `scmrepo-1.0.2/src/scmrepo/asyn.py` & `scmrepo-1.0.3/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/base.py` & `scmrepo-1.0.3/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/exceptions.py` & `scmrepo-1.0.3/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/fs.py` & `scmrepo-1.0.3/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/__init__.py` & `scmrepo-1.0.3/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/base.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,24 +610,25 @@
         progress: Callable[["GitProgressEvent"], None] = None,
         **kwargs,
     ) -> Mapping[str, SyncStatus]:
         from dulwich.client import get_transport_and_path
         from dulwich.errors import NotGitRepository
         from dulwich.objectspec import parse_reftuples
         from dulwich.porcelain import DivergedBranches, check_diverged, get_remote_repo
+        from dulwich.refs import DictRefsContainer
 
         fetch_refs = []
 
         def determine_wants(
             remote_refs: Dict[bytes, bytes],
             depth: Optional[int] = None,  # pylint: disable=unused-argument
         ) -> List[bytes]:
             fetch_refs.extend(
                 parse_reftuples(
-                    remote_refs,
+                    DictRefsContainer(remote_refs),
                     self.repo.refs,
                     os.fsencode(refspecs)
                     if isinstance(refspecs, str)
                     else [os.fsencode(refspec) for refspec in refspecs],
                     force=force,
                 )
             )
```

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/gitpython.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/credentials.py` & `scmrepo-1.0.3/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/objects.py` & `scmrepo-1.0.3/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/git/stash.py` & `scmrepo-1.0.3/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/progress.py` & `scmrepo-1.0.3/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo/utils.py` & `scmrepo-1.0.3/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-1.0.3/src/scmrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.2
+Version: 1.0.3
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.2/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-1.0.3/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/src/scmrepo.egg-info/requires.txt` & `scmrepo-1.0.3/src/scmrepo.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 gitpython>3
-dulwich>=0.20.49
+dulwich>=0.21.5
 pygit2>=1.10.0
 pygtrie>=2.3.2
 fsspec>=2021.7.0
 pathspec>=0.9.0
 asyncssh<3,>=2.13.1
 funcy>=1.14
 shortuuid>=0.5.0
```

### Comparing `scmrepo-1.0.2/tests/conftest.py` & `scmrepo-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_credentials.py` & `scmrepo-1.0.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_dulwich.py` & `scmrepo-1.0.3/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_fs.py` & `scmrepo-1.0.3/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_git.py` & `scmrepo-1.0.3/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_noscm.py` & `scmrepo-1.0.3/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_pygit2.py` & `scmrepo-1.0.3/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_scmrepo.py` & `scmrepo-1.0.3/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/test_stash.py` & `scmrepo-1.0.3/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.2/tests/user.key` & `scmrepo-1.0.3/tests/user.key`

 * *Files identical despite different names*

