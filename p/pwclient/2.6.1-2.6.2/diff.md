# Comparing `tmp/pwclient-2.6.1.tar.gz` & `tmp/pwclient-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwclient-2.6.1.tar", last modified: Tue May  2 10:42:05 2023, max compression
+gzip compressed data, was "pwclient-2.6.2.tar", last modified: Thu May  4 10:00:26 2023, max compression
```

## Comparing `pwclient-2.6.1.tar` & `pwclient-2.6.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.216703 pwclient-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 10:41:53.000000 pwclient-2.6.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-02 10:41:53.000000 pwclient-2.6.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-02 10:41:53.000000 pwclient-2.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 10:42:05.000000 pwclient-2.6.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-02 10:41:53.000000 pwclient-2.6.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-02 10:42:05.000000 pwclient-2.6.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-02 10:42:05.216703 pwclient-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-02 10:41:53.000000 pwclient-2.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/man/
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-02 10:41:53.000000 pwclient-2.6.1/man/pwclient.1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/pwclient/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/xmlrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/pwclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 10:41:53.000000 pwclient-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 10:41:53.000000 pwclient-2.6.1/readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-long-opts-4611e7cce3993f08.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-python3-10-drop-python-3-6-support-32b91d5753adfc29.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-python3-11-support-eb86886925d2e5ec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-get-4f010b2c4fdcd55c.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-list-create-help-94ccb51660af1138.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/drop-pypy-support-17f1f95b9394b257.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/drop-python2-support-0351245b41052e20.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/git-am--m-flag-190f3a7e17cec6f4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/initial-release-eb74a7ae0ce3b1fb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/issue-1-c7e4c3e4e57c1c22.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/list--hash-option-ebb96d3a70920cf5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/pwclientrc-environment-variable-e070047b82e3b77f.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/version-2-2-0d142cb0ab85eb67.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/version-2-3-fd18e538b15396d8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 10:41:53.000000 pwclient-2.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-02 10:42:05.216703 pwclient-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 10:41:53.000000 pwclient-2.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 10:41:53.000000 pwclient-2.6.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.216703 pwclient-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_states.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 10:41:53.000000 pwclient-2.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.572744 pwclient-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 10:00:15.000000 pwclient-2.6.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.560744 pwclient-2.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.564744 pwclient-2.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-04 10:00:15.000000 pwclient-2.6.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 10:00:15.000000 pwclient-2.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-04 10:00:26.000000 pwclient-2.6.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-04 10:00:15.000000 pwclient-2.6.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-04 10:00:26.000000 pwclient-2.6.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-04 10:00:26.572744 pwclient-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-04 10:00:15.000000 pwclient-2.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.564744 pwclient-2.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 10:00:15.000000 pwclient-2.6.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.564744 pwclient-2.6.2/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-04 10:00:15.000000 pwclient-2.6.2/man/pwclient.1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.568744 pwclient-2.6.2/pwclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-04 10:00:15.000000 pwclient-2.6.2/pwclient/xmlrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.568744 pwclient-2.6.2/pwclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 10:00:26.000000 pwclient-2.6.2/pwclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 10:00:15.000000 pwclient-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 10:00:15.000000 pwclient-2.6.2/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.568744 pwclient-2.6.2/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.572744 pwclient-2.6.2/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/add-long-opts-4611e7cce3993f08.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/add-python3-10-drop-python-3-6-support-32b91d5753adfc29.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/add-python3-11-support-eb86886925d2e5ec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/check-get-4f010b2c4fdcd55c.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/check-list-create-help-94ccb51660af1138.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/drop-pypy-support-17f1f95b9394b257.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/drop-python2-support-0351245b41052e20.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/git-am--m-flag-190f3a7e17cec6f4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/initial-release-eb74a7ae0ce3b1fb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/issue-1-c7e4c3e4e57c1c22.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/list--hash-option-ebb96d3a70920cf5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/pwclientrc-environment-variable-e070047b82e3b77f.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/version-2-2-0d142cb0ab85eb67.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 10:00:15.000000 pwclient-2.6.2/releasenotes/notes/version-2-3-fd18e538b15396d8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 10:00:15.000000 pwclient-2.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 10:00:26.576744 pwclient-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 10:00:15.000000 pwclient-2.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 10:00:15.000000 pwclient-2.6.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:26.572744 pwclient-2.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-04 10:00:15.000000 pwclient-2.6.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 10:00:15.000000 pwclient-2.6.2/tox.ini
```

### Comparing `pwclient-2.6.1/.github/workflows/ci.yaml` & `pwclient-2.6.2/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -102,10 +102,10 @@
         id: upload-release-asset
         if: startsWith(github.ref, 'refs/tags')
         uses: actions/upload-release-asset@v1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           upload_url: ${{ steps.create_release.outputs.upload_url }}
-          asset_path: ./dist/git-pw-${{ github.ref }}.tar.gz
-          asset_name: git-pw-${{ github.ref }}.tar.gz
+          asset_path: ./dist/pwclient-${{ github.ref }}.tar.gz
+          asset_name: pwclient-${{ github.ref }}.tar.gz
           asset_content_type: application/gzip
```

### Comparing `pwclient-2.6.1/.pre-commit-config.yaml` & `pwclient-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/AUTHORS` & `pwclient-2.6.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/COPYING` & `pwclient-2.6.2/COPYING`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/ChangeLog` & `pwclient-2.6.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.6.2
+-----
+
+* Release 2.6.2
+* Don't expect return value from API.patch\_set
+* CI: Correct copy-pasta
+
 2.6.1
 -----
 
 * Release 2.6.1
 * xmlrpc: Enable 'allow\_none'
 * CI: Enable releases
 * CI: Don't put to test-pypi on release
```

### Comparing `pwclient-2.6.1/PKG-INFO` & `pwclient-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwclient
-Version: 2.6.1
+Version: 2.6.2
 Summary: The command-line client for the Patchwork patch tracking tool
 Home-page: https://github.com/getpatchwork/pwclient
 Author: Nate Case
 Author-email: ncase@xes-inc.com
 Maintainer: Stephen Finucane
 Maintainer-email: stephen@that.guru
 License: GPL v2
```

### Comparing `pwclient-2.6.1/README.rst` & `pwclient-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/docs/conf.py` & `pwclient-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/docs/configuration.rst` & `pwclient-2.6.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/man/pwclient.1` & `pwclient-2.6.2/man/pwclient.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH PWCLIENT "1" "2023\-05\-02" "pwclient" "Generated Python Manual"
+.TH PWCLIENT "1" "2023\-05\-04" "pwclient" "Generated Python Manual"
 .SH NAME
 pwclient
 .SH SYNOPSIS
 .B pwclient
 [-h] {apply,git-am,get,info,projects,check-get,check-list,check-info,check-create,states,view,update,list,search} ...
 
 .SH
```

### Comparing `pwclient-2.6.1/pwclient/api.py` & `pwclient-2.6.2/pwclient/api.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/checks.py` & `pwclient-2.6.2/pwclient/checks.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/parser.py` & `pwclient-2.6.2/pwclient/parser.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/patches.py` & `pwclient-2.6.2/pwclient/patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,20 +221,17 @@
     # ensure the patch actually exists first
     try:
         api.patch_get(patch_id)
     except Exception as exc:
         print(str(exc), file=sys.stderr)
         sys.exit(1)
 
-    success = False
     try:
-        success = api.patch_set(
+        api.patch_set(
             patch_id,
             state=state,
             archived=archived,
             commit_ref=commit_ref,
         )
     except Exception as exc:
         print(str(exc), file=sys.stderr)
-
-    if not success:
-        print('Patch not updated', file=sys.stderr)
+        sys.exit(1)
```

### Comparing `pwclient-2.6.1/pwclient/projects.py` & `pwclient-2.6.2/pwclient/projects.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/shell.py` & `pwclient-2.6.2/pwclient/shell.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/utils.py` & `pwclient-2.6.2/pwclient/utils.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient/xmlrpc.py` & `pwclient-2.6.2/pwclient/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/pwclient.egg-info/PKG-INFO` & `pwclient-2.6.2/pwclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwclient
-Version: 2.6.1
+Version: 2.6.2
 Summary: The command-line client for the Patchwork patch tracking tool
 Home-page: https://github.com/getpatchwork/pwclient
 Author: Nate Case
 Author-email: ncase@xes-inc.com
 Maintainer: Stephen Finucane
 Maintainer-email: stephen@that.guru
 License: GPL v2
```

### Comparing `pwclient-2.6.1/pwclient.egg-info/SOURCES.txt` & `pwclient-2.6.2/pwclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml` & `pwclient-2.6.2/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml` & `pwclient-2.6.2/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/setup.cfg` & `pwclient-2.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tests/fakes.py` & `pwclient-2.6.2/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tests/test_api.py` & `pwclient-2.6.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tests/test_checks.py` & `pwclient-2.6.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tests/test_patches.py` & `pwclient-2.6.2/tests/test_patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -515,40 +515,23 @@
 
 
 def test_action_update__error(capsys):
     api = mock.Mock()
     api.patch_get.return_value = fakes.fake_patches()[0]
     api.patch_set.side_effect = exceptions.APIError('foo')
 
-    patches.action_update(api, 1157169)
+    with pytest.raises(SystemExit):
+        patches.action_update(api, 1157169)
 
     api.patch_set.assert_called_once_with(
         1157169, archived=None, commit_ref=None, state=None
     )
 
     captured = capsys.readouterr()
 
     assert captured.out == ''
     assert (
         captured.err
         == """\
 foo
-Patch not updated
 """
     )
-
-
-def test_action_update__no_updates(capsys):
-    api = mock.Mock()
-    api.patch_get.return_value = fakes.fake_patches()[0]
-    api.patch_set.return_value = None
-
-    patches.action_update(api, 1157169)
-
-    api.patch_set.assert_called_once_with(
-        1157169, archived=None, commit_ref=None, state=None
-    )
-
-    captured = capsys.readouterr()
-
-    assert captured.out == ''
-    assert captured.err == 'Patch not updated\n'
```

### Comparing `pwclient-2.6.1/tests/test_shell.py` & `pwclient-2.6.2/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tests/test_utils.py` & `pwclient-2.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.1/tox.ini` & `pwclient-2.6.2/tox.ini`

 * *Files identical despite different names*

