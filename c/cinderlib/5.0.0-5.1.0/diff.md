# Comparing `tmp/cinderlib-5.0.0.tar.gz` & `tmp/cinderlib-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinderlib-5.0.0.tar", last modified: Fri Dec 16 09:04:06 2022, max compression
+gzip compressed data, was "cinderlib-5.1.0.tar", last modified: Thu May  4 09:40:56 2023, max compression
```

## Comparing `cinderlib-5.0.0.tar` & `cinderlib-5.1.0.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.417819 cinderlib-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-12-16 09:03:40.000000 cinderlib-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3860 2022-12-16 09:03:40.000000 cinderlib-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2022-12-16 09:04:06.000000 cinderlib-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-12-16 09:03:40.000000 cinderlib-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9788 2022-12-16 09:04:06.000000 cinderlib-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2022-12-16 09:03:40.000000 cinderlib-5.0.0/DESCRIPTION.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2267 2022-12-16 09:03:40.000000 cinderlib-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-12-16 09:03:40.000000 cinderlib-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2022-12-16 09:04:06.417819 cinderlib-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2022-12-16 09:03:40.000000 cinderlib-5.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-12-16 09:03:40.000000 cinderlib-5.0.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2022-12-16 09:03:40.000000 cinderlib-5.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.401819 cinderlib-5.0.0/cinderlib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5911 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/_fake_packages.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.401819 cinderlib-5.0.0/cinderlib/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/bin/venv-privsep-helper
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23748 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/cinderlib.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.401819 cinderlib-5.0.0/cinderlib/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/cmd/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2164 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/cmd/cinder_cfg_to_python.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2666 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/cmd/cinder_to_yaml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35336 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/objects.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/persistence/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9872 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16312 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/persistence/dbms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3912 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/persistence/memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10209 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/functional/base_tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/functional/ceph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/functional/lvm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10353 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/functional/test_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13133 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/objects/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7245 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/objects/test_snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24950 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/objects/test_volume.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.405819 cinderlib-5.0.0/cinderlib/tests/unit/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25023 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4706 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12026 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/test_dbms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3817 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/persistence/test_memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33080 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/test_cinderlib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/test_serialization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/tests/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2022-12-16 09:03:40.000000 cinderlib-5.0.0/cinderlib/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.401819 cinderlib-5.0.0/cinderlib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4399 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2022-12-16 09:04:06.000000 cinderlib-5.0.0/cinderlib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2022-12-16 09:03:40.000000 cinderlib-5.0.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-12-16 09:03:40.000000 cinderlib-5.0.0/devstack/override-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2022-12-16 09:03:40.000000 cinderlib-5.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-12-16 09:03:40.000000 cinderlib-5.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/_extra/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/_static/.placeholder
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9275 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14681 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/limitations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6465 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/make.bat
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/doc/source/topics/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13567 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/backends.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11991 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/connections.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7081 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/initialization.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9395 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/metadata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8624 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/serialization.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/snapshots.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/tracking.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9630 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/topics/volumes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7264 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/validated.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19481 2022-12-16 09:03:40.000000 cinderlib-5.0.0/doc/source/validating.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.409819 cinderlib-5.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-12-16 09:03:40.000000 cinderlib-5.0.0/playbooks/cinder-gate-run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2022-12-16 09:03:40.000000 cinderlib-5.0.0/playbooks/required-projects-bindeps.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2022-12-16 09:03:40.000000 cinderlib-5.0.0/playbooks/setup-ceph.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2411 2022-12-16 09:03:40.000000 cinderlib-5.0.0/playbooks/setup-lvm.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.397819 cinderlib-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/IBM-SVC-667322aa2b4ac24d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/accept-template-values-e228d065800ac5b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/attach_mode-0cc9cec91dff0fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/backend-same-name-86a06844b57600a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/cinderlib-a458b8e23b6d35f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/datetime-subsecond-e123e8d2dda707ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/drop-py2-a56fb12674516c67.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/enhance-extend-687d8e9c4a58e517.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fake-packages-7d5c55e6169f1096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fix-clone-28b18ddb420ff676.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fix-lvm-extend-e46b0eadf1cd59ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fix-mysql-vol-delete-f675778ea150cb9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fix-not-local-a8cf22a2092c8a98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/fix-privsep-venv-2ae8ce791136ae73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/improve-list-drivers-9bd501689d5eeb27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/mysql-db-sync-8a9e50a12bbe724d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/privsep-support-acbc955b9845a6ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/rbd-improve-containerized-detection-2bd8a2f995215cdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/rbd-missing-file-or-directory-c835abac22f6b32e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/rbd-non-root-ac971f51461d4d6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/snapshot-vol-type-20e4403ed5a8b0a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/support-comple-config-options-39ba50c6c9165cc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/notes/zed-release-7b57944880235392.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1734 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-12-16 09:03:40.000000 cinderlib-5.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-12-16 09:03:40.000000 cinderlib-5.0.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.397819 cinderlib-5.0.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/roles/run-cinderlib-tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2022-12-16 09:03:40.000000 cinderlib-5.0.0/roles/run-cinderlib-tests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/roles/run-cinderlib-tests/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2022-12-16 09:03:40.000000 cinderlib-5.0.0/roles/run-cinderlib-tests/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/roles/run-cinderlib-tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2022-12-16 09:03:40.000000 cinderlib-5.0.0/roles/run-cinderlib-tests/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2022-12-16 09:04:06.417819 cinderlib-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-12-16 09:03:40.000000 cinderlib-5.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-12-16 09:03:40.000000 cinderlib-5.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-12-16 09:04:06.413819 cinderlib-5.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1267 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2499 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/generate_uc.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      222 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/lvm-prepare.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      741 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/special_install.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      691 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tools/virtualenv-sudo.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7079 2022-12-16 09:03:40.000000 cinderlib-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.353150 cinderlib-5.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-04 09:40:27.000000 cinderlib-5.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4416 2023-05-04 09:40:27.000000 cinderlib-5.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2023-05-04 09:40:56.000000 cinderlib-5.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2023-05-04 09:40:27.000000 cinderlib-5.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10091 2023-05-04 09:40:56.000000 cinderlib-5.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2023-05-04 09:40:27.000000 cinderlib-5.1.0/DESCRIPTION.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2267 2023-05-04 09:40:27.000000 cinderlib-5.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-04 09:40:27.000000 cinderlib-5.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2023-05-04 09:40:56.353150 cinderlib-5.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2023-05-04 09:40:27.000000 cinderlib-5.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-05-04 09:40:27.000000 cinderlib-5.1.0/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2023-05-04 09:40:27.000000 cinderlib-5.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.325152 cinderlib-5.1.0/cinderlib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5911 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/_fake_packages.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.325152 cinderlib-5.1.0/cinderlib/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      348 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/bin/venv-privsep-helper
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23748 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/cinderlib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.325152 cinderlib-5.1.0/cinderlib/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/cmd/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2164 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/cmd/cinder_cfg_to_python.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2666 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/cmd/cinder_to_yaml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1243 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35336 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/objects.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.329151 cinderlib-5.1.0/cinderlib/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/persistence/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9872 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17513 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/persistence/dbms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3912 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/persistence/memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.329151 cinderlib-5.1.0/cinderlib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.329151 cinderlib-5.1.0/cinderlib/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10209 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/functional/base_tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/functional/ceph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/functional/lvm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10353 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/functional/test_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.333151 cinderlib-5.1.0/cinderlib/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.333151 cinderlib-5.1.0/cinderlib/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13133 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/objects/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7245 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/objects/test_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24950 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/objects/test_volume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.333151 cinderlib-5.1.0/cinderlib/tests/unit/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24900 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7019 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/test_dbms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3817 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/persistence/test_memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33082 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/test_cinderlib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/test_serialization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/tests/unit/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-05-04 09:40:27.000000 cinderlib-5.1.0/cinderlib/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.325152 cinderlib-5.1.0/cinderlib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-05-04 09:40:56.000000 cinderlib-5.1.0/cinderlib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.333151 cinderlib-5.1.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2023-05-04 09:40:27.000000 cinderlib-5.1.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-04 09:40:27.000000 cinderlib-5.1.0/devstack/override-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-05-04 09:40:27.000000 cinderlib-5.1.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-04 09:40:27.000000 cinderlib-5.1.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.337151 cinderlib-5.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.337151 cinderlib-5.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.337151 cinderlib-5.1.0/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/_extra/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.337151 cinderlib-5.1.0/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/_static/.placeholder
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9274 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.337151 cinderlib-5.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14633 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/limitations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6465 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/make.bat
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.341150 cinderlib-5.1.0/doc/source/topics/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13567 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/backends.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11991 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/connections.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7081 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/initialization.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9395 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/metadata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8624 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/serialization.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/snapshots.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/tracking.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9630 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/topics/volumes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7264 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/validated.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19481 2023-05-04 09:40:27.000000 cinderlib-5.1.0/doc/source/validating.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.341150 cinderlib-5.1.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-05-04 09:40:27.000000 cinderlib-5.1.0/playbooks/cinder-gate-run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-05-04 09:40:27.000000 cinderlib-5.1.0/playbooks/required-projects-bindeps.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-05-04 09:40:27.000000 cinderlib-5.1.0/playbooks/setup-ceph.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2411 2023-05-04 09:40:27.000000 cinderlib-5.1.0/playbooks/setup-lvm.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.317152 cinderlib-5.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.349150 cinderlib-5.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/IBM-SVC-667322aa2b4ac24d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/accept-template-values-e228d065800ac5b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/attach_mode-0cc9cec91dff0fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/backend-same-name-86a06844b57600a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/cinderlib-a458b8e23b6d35f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/datetime-subsecond-e123e8d2dda707ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/drop-py2-a56fb12674516c67.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/enhance-extend-687d8e9c4a58e517.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fake-packages-7d5c55e6169f1096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fix-clone-28b18ddb420ff676.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fix-lvm-extend-e46b0eadf1cd59ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fix-mysql-vol-delete-f675778ea150cb9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fix-not-local-a8cf22a2092c8a98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/fix-privsep-venv-2ae8ce791136ae73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/improve-list-drivers-9bd501689d5eeb27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/mysql-db-sync-8a9e50a12bbe724d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/privsep-support-acbc955b9845a6ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/rbd-improve-containerized-detection-2bd8a2f995215cdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/rbd-missing-file-or-directory-c835abac22f6b32e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/rbd-non-root-ac971f51461d4d6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/snapshot-vol-type-20e4403ed5a8b0a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/support-comple-config-options-39ba50c6c9165cc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/notes/zed-release-7b57944880235392.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.349150 cinderlib-5.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1734 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-04 09:40:27.000000 cinderlib-5.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-04 09:40:27.000000 cinderlib-5.1.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.317152 cinderlib-5.1.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.349150 cinderlib-5.1.0/roles/run-cinderlib-tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-05-04 09:40:27.000000 cinderlib-5.1.0/roles/run-cinderlib-tests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.353150 cinderlib-5.1.0/roles/run-cinderlib-tests/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-04 09:40:27.000000 cinderlib-5.1.0/roles/run-cinderlib-tests/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.353150 cinderlib-5.1.0/roles/run-cinderlib-tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-05-04 09:40:27.000000 cinderlib-5.1.0/roles/run-cinderlib-tests/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2023-05-04 09:40:56.357149 cinderlib-5.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-05-04 09:40:27.000000 cinderlib-5.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-05-04 09:40:27.000000 cinderlib-5.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 09:40:56.353150 cinderlib-5.1.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1267 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/fast8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2499 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/generate_uc.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      222 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/lvm-prepare.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      741 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/special_install.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      691 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tools/virtualenv-sudo.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6730 2023-05-04 09:40:27.000000 cinderlib-5.1.0/tox.ini
```

### Comparing `cinderlib-5.0.0/AUTHORS` & `cinderlib-5.1.0/AUTHORS`

 * *Files 7% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 Sahid Orentino Ferdjaoui <sahid.ferdjaoui@canonical.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Stephen Finucane <stephenfin@redhat.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Takashi Natsume <takanattie@gmail.com>
 Walter A. Boring IV <waboring@hemna.com>
 karmab <karimboumedhel@gmail.com>
+niuke <niuke19970315@163.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 tushargite96 <tushargite96@gmail.com>
 whoami-rajat <rajatdhasmana@gmail.com>
 xuanyandong <xuanyandong@inspur.com>
```

### Comparing `cinderlib-5.0.0/CONTRIBUTING.rst` & `cinderlib-5.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/ChangeLog` & `cinderlib-5.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 CHANGES
 =======
 
+5.1.0
+-----
+
+* Continue 2023.1 (Antelope) development
+* Don't use deprecated config opt name in unit test
+* Fix DBMS storage plugin
+* Fix tox.ini
+* Remove unnecessary #egg= URL fragment
+* Open cinderlib for 2023.1 (Antelope) development
+* Update master for stable/zed
+
 5.0.0
 -----
 
 * Add Zed release note
 * Support driver's setup method
 * Remove six
 * Don't limit use of importlib-metadata to Python < 3.8
 * Fix py310 unit tests
 * Open cinderlib for zed development
 * Fix cinderlib tests
 * Fix ValueError when running with zed cinder
 * Fix wrong assertion methods in unit tests
 * Update metadata in setup.cfg
+* remove unicode prefix from code
 * Update deprecated zuul syntax
 * Don't use yum to install ceph
 * [docs] add zuul.yaml maintenance tasks
 * Update master for stable/yoga
 
 4.2.0
 -----
```

### Comparing `cinderlib-5.0.0/DESCRIPTION.rst` & `cinderlib-5.1.0/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/HACKING.rst` & `cinderlib-5.1.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/LICENSE` & `cinderlib-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/PKG-INFO` & `cinderlib-5.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cinderlib
-Version: 5.0.0
+Version: 5.1.0
 Summary: Direct usage of Cinder Block Storage drivers without the services
 Home-page: https://docs.openstack.org/cinderlib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Direct usage of Cinder Block Storage drivers without the services
 Platform: UNKNOWN
@@ -16,8 +16,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `cinderlib-5.0.0/README.rst` & `cinderlib-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/bindep.txt` & `cinderlib-5.1.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/__init__.py` & `cinderlib-5.1.0/cinderlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/_fake_packages.py` & `cinderlib-5.1.0/cinderlib/_fake_packages.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/cinderlib.py` & `cinderlib-5.1.0/cinderlib/cinderlib.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/cmd/cinder_cfg_to_python.py` & `cinderlib-5.1.0/cinderlib/cmd/cinder_cfg_to_python.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/cmd/cinder_to_yaml.py` & `cinderlib-5.1.0/cinderlib/cmd/cinder_to_yaml.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/exception.py` & `cinderlib-5.1.0/cinderlib/exception.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/objects.py` & `cinderlib-5.1.0/cinderlib/objects.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/persistence/__init__.py` & `cinderlib-5.1.0/cinderlib/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/persistence/base.py` & `cinderlib-5.1.0/cinderlib/persistence/base.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/persistence/dbms.py` & `cinderlib-5.1.0/cinderlib/persistence/dbms.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,39 @@
 
 from cinderlib import objects
 from cinderlib.persistence import base as persistence_base
 
 LOG = log.getLogger(__name__)
 
 
+def db_writer(func):
+    """Decorator to start a DB writing transaction.
+
+    With the new Oslo DB Transaction Sessions everything needs to use the
+    sessions of the enginefacade using the function decorator or the context
+    manager approach: https://docs.openstack.org/oslo.db/ocata/usage.html
+
+    This plugin cannot use the decorator form because its fuctions don't
+    receive a Context objects that the decorator can find and use, so we use
+    this decorator instead.
+
+    Cinder DB API methods already have a decorator, so methods calling them
+    don't require this decorator, but methods that directly call the DB using
+    sqlalchemy or using the model_query method do.
+
+    Using this decorator at this level also allows us to enclose everything in
+    a single transaction, and it doesn't have any problems with the existing
+    Cinder decorators.
+    """
+    def wrapper(*args, **kwargs):
+        with sqla_api.main_context_manager.writer.using(objects.CONTEXT):
+            return func(*args, **kwargs)
+    return wrapper
+
+
 class KeyValue(models.BASE, oslo_db_models.ModelBase, objects.KeyValue):
     __tablename__ = 'cinderlib_persistence_key_value'
     key = sa.Column(sa.String(255), primary_key=True)
     value = sa.Column(sa.Text)
 
 
 class DBPersistence(persistence_base.PersistenceDriverBase):
@@ -175,28 +200,29 @@
         ovos = cinder_objs.VolumeAttachmentList.get_all(objects.CONTEXT,
                                                         filters)
         # Leverage lazy loading of the volume and backend in Connection
         result = [objects.Connection(None, volume=None, __ovo=ovo)
                   for ovo in ovos.objects]
         return result
 
-    def _get_kv(self, key=None, session=None):
-        session = objects.CONTEXT.session
+    def _get_kv(self, session, key=None):
         query = session.query(KeyValue)
         if key is not None:
             query = query.filter_by(key=key)
         res = query.all()
         # If we want to use the result as an ORM
         if session:
             return res
         return [objects.KeyValue(r.key, r.value) for r in res]
 
     def get_key_values(self, key=None):
-        return self._get_kv(key)
+        with sqla_api.main_context_manager.reader.using(objects.CONTEXT) as s:
+            return self._get_kv(s, key)
 
+    @db_writer
     def set_volume(self, volume):
         changed = self.get_changed_fields(volume)
         if not changed:
             changed = self.get_fields(volume)
 
         extra_specs = changed.pop('extra_specs', None)
         qos_specs = changed.pop('qos_specs', None)
@@ -251,14 +277,15 @@
                 del changed['id']
 
         if changed:
             LOG.debug('set_volume updating %s', changed)
             self.db.volume_update(objects.CONTEXT, volume.id, changed)
         super(DBPersistence, self).set_volume(volume)
 
+    @db_writer
     def set_snapshot(self, snapshot):
         changed = self.get_changed_fields(snapshot)
         if not changed:
             changed = self.get_fields(snapshot)
 
         # Create
         if 'id' in changed:
@@ -270,14 +297,15 @@
                 del changed['id']
 
         if changed:
             LOG.debug('set_snapshot updating %s', changed)
             self.db.snapshot_update(objects.CONTEXT, snapshot.id, changed)
         super(DBPersistence, self).set_snapshot(snapshot)
 
+    @db_writer
     def set_connection(self, connection):
         changed = self.get_changed_fields(connection)
         if not changed:
             changed = self.get_fields(connection)
 
         if 'connection_info' in changed:
             connection._convert_connection_info_to_db_format(changed)
@@ -296,21 +324,23 @@
 
         if changed:
             LOG.debug('set_connection updating %s', changed)
             self.db.volume_attachment_update(objects.CONTEXT, connection.id,
                                              changed)
         super(DBPersistence, self).set_connection(connection)
 
+    @db_writer
     def set_key_value(self, key_value):
         session = objects.CONTEXT.session
-        kv = self._get_kv(key_value.key, session)
+        kv = self._get_kv(session, key_value.key)
         kv = kv[0] if kv else KeyValue(key=key_value.key)
         kv.value = key_value.value
         session.add(kv)
 
+    @db_writer
     def delete_volume(self, volume):
         delete_type = (volume.volume_type_id != self.DEFAULT_TYPE.id
                        and volume.volume_type_id)
         if self.soft_deletes:
             LOG.debug('soft deleting volume %s', volume.id)
             self.db.volume_destroy(objects.CONTEXT, volume.id)
             if delete_type:
@@ -345,35 +375,38 @@
                 if qos_id:
                     query.filter(sqla_api.or_(
                         models.QualityOfServiceSpecs.id == qos_id,
                         models.QualityOfServiceSpecs.specs_id == qos_id
                     )).delete()
         super(DBPersistence, self).delete_volume(volume)
 
+    @db_writer
     def delete_snapshot(self, snapshot):
         if self.soft_deletes:
             LOG.debug('soft deleting snapshot %s', snapshot.id)
             self.db.snapshot_destroy(objects.CONTEXT, snapshot.id)
         else:
             LOG.debug('hard deleting snapshot %s', snapshot.id)
             query = sqla_api.model_query(objects.CONTEXT, models.Snapshot)
             query.filter_by(id=snapshot.id).delete()
         super(DBPersistence, self).delete_snapshot(snapshot)
 
+    @db_writer
     def delete_connection(self, connection):
         if self.soft_deletes:
             LOG.debug('soft deleting connection %s', connection.id)
             self.db.attachment_destroy(objects.CONTEXT, connection.id)
         else:
             LOG.debug('hard deleting connection %s', connection.id)
             query = sqla_api.model_query(objects.CONTEXT,
                                          models.VolumeAttachment)
             query.filter_by(id=connection.id).delete()
         super(DBPersistence, self).delete_connection(connection)
 
+    @db_writer
     def delete_key_value(self, key_value):
         session = objects.CONTEXT.session
         query = session.query(KeyValue)
         query.filter_by(key=key_value.key).delete()
 
 
 class MemoryDBPersistence(DBPersistence):
```

### Comparing `cinderlib-5.0.0/cinderlib/persistence/memory.py` & `cinderlib-5.1.0/cinderlib/persistence/memory.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/serialization.py` & `cinderlib-5.1.0/cinderlib/serialization.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/functional/base_tests.py` & `cinderlib-5.1.0/cinderlib/tests/functional/base_tests.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/functional/test_basic.py` & `cinderlib-5.1.0/cinderlib/tests/functional/test_basic.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/base.py` & `cinderlib-5.1.0/cinderlib/tests/unit/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class BaseTest(unittest.TestCase):
     PERSISTENCE_CFG = None
 
     def setUp(self):
         if not self.PERSISTENCE_CFG:
             cfg = {'storage': utils.get_mock_persistence()}
             cinderlib.Backend.set_persistence(cfg)
-        self.backend_name = 'fake_backend_%s' % id(self)
+        self.backend_name = 'fake_backend'
         self.backend = utils.FakeBackend(volume_backend_name=self.backend_name)
         self.persistence = self.backend.persistence
         cinderlib.Backend._volumes_inflight = {}
 
     def tearDown(self):
         # Clear all existing backends
         cinderlib.Backend.backends = {}
```

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/objects/test_connection.py` & `cinderlib-5.1.0/cinderlib/tests/unit/objects/test_connection.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/objects/test_snapshot.py` & `cinderlib-5.1.0/cinderlib/tests/unit/objects/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/objects/test_volume.py` & `cinderlib-5.1.0/cinderlib/tests/unit/objects/test_volume.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/persistence/base.py` & `cinderlib-5.1.0/cinderlib/tests/unit/persistence/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 from cinderlib.tests.unit import utils
 
 
 class BasePersistenceTest(helper.TestHelper):
 
     def setUp(self):
         super(BasePersistenceTest, self).setUp()
-        self.backend_name = 'fake_backend'
-        self.backend = utils.FakeBackend(volume_backend_name=self.backend_name)
 
     def assertListEqualObj(self, expected, actual):
         exp = [self._convert_to_dict(e) for e in expected]
         act = [self._convert_to_dict(a) for a in actual]
         self.assertListEqual(exp, act)
 
     def assertEqualObj(self, expected, actual):
```

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/persistence/helper.py` & `cinderlib-5.1.0/cinderlib/tests/unit/persistence/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,23 @@
         cinderlib.Backend.global_initialization = False
         cinderlib.setup(persistence_config=cls.PERSISTENCE_CFG)
 
     @classmethod
     def tearDownClass(cls):
         volume_cmd.session.IMPL = cls.original_impl
         cinderlib.Backend.global_initialization = False
-        api.main_context_manager = api.enginefacade.transaction_context()
+
+        # Cannot just replace the context manager itself because it is already
+        # decorating cinder DB methods and those would continue accessing the
+        # old database, so we replace the existing CM'sinternal transaction
+        # factory, efectively "reseting" the context manager.
+        cm = api.main_context_manager
+        if cm.is_started:
+            cm._root_factory = api.enginefacade._TransactionFactory()
+
         for ovo_name, methods in cls.ovo_methods.items():
             ovo_cls = getattr(objects, ovo_name)
             for method_name, method in methods.items():
                 if method:
                     setattr(ovo_cls, method_name, method)
 
     def setUp(self):
@@ -65,20 +73,15 @@
 
     def create_volumes(self, data, sort=True):
         vols = []
         for d in data:
             d.setdefault('backend_or_vol', self.backend)
             vol = cinderlib.Volume(**d)
             vols.append(vol)
-            # db_instance is a property of DBMS plugin
-            if hasattr(self.persistence, 'db_instance'):
-                with api.main_context_manager.writer.using(self.context):
-                    self.persistence.set_volume(vol)
-            else:
-                self.persistence.set_volume(vol)
+            self.persistence.set_volume(vol)
         if sort:
             return self.sorted(vols)
         return vols
 
     def create_snapshots(self):
         vols = self.create_n_volumes(2)
         snaps = []
@@ -99,20 +102,15 @@
         return self.sorted(conns)
 
     def create_key_values(self):
         kvs = []
         for i in range(2):
             kv = cinderlib.KeyValue(key='key%i' % i, value='value%i' % i)
             kvs.append(kv)
-            # db_instance is a property of DBMS plugin
-            if hasattr(self.persistence, 'db_instance'):
-                with api.main_context_manager.writer.using(self.context):
-                    self.persistence.set_key_value(kv)
-            else:
-                self.persistence.set_key_value(kv)
+            self.persistence.set_key_value(kv)
         return kvs
 
     def _convert_to_dict(self, obj):
         if isinstance(obj, models.BASE):
             return dict(obj)
 
         if not isinstance(obj, cinderlib.objects.Object):
```

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/persistence/test_base.py` & `cinderlib-5.1.0/cinderlib/tests/unit/persistence/test_base.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/persistence/test_memory.py` & `cinderlib-5.1.0/cinderlib/tests/unit/persistence/test_memory.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/test_cinderlib.py` & `cinderlib-5.1.0/cinderlib/tests/unit/test_cinderlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,26 +282,26 @@
         # Global values overrides are left
         self.assertIs(True, cfg.CONF.debug)
         self.assertEqual(['a', 'b', 'c'], cfg.CONF.osapi_volume_extension)
 
         cinder_cfg = {
             'volume_driver': 'cinder.volume.drivers.lvm.LVMVolumeDriver',
             'volume_group': 'lvm-volumes',
-            'iscsi_secondary_ip_addresses': ['w.x.y.z', 'a.b.c.d'],
+            'target_secondary_ip_addresses': ['w.x.y.z', 'a.b.c.d'],
             'target_port': 12345,
         }
         expected_cfg = cinder_cfg.copy()
 
         # Test driver options with String, ListOpt, PortOpt
         self.backend._validate_and_set_options(cinder_cfg)
         # Non global value overrides have been cleaned up
         self.assertEqual('cinder-volumes',
                          cfg.CONF.backend_defaults.volume_group)
         self.assertEqual(
-            [], cfg.CONF.backend_defaults.iscsi_secondary_ip_addresses)
+            [], cfg.CONF.backend_defaults.target_secondary_ip_addresses)
         self.assertEqual(3260, cfg.CONF.backend_defaults.target_port)
         self.assertEqual(expected_cfg, cinder_cfg)
 
         warning_mock.assert_not_called()
 
     @mock.patch('cinderlib.cinderlib.LOG.warning')
     def test__validate_and_set_options_rbd(self, warning_mock):
```

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/test_serialization.py` & `cinderlib-5.1.0/cinderlib/tests/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/tests/unit/utils.py` & `cinderlib-5.1.0/cinderlib/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib/utils.py` & `cinderlib-5.1.0/cinderlib/utils.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/cinderlib.egg-info/PKG-INFO` & `cinderlib-5.1.0/cinderlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cinderlib
-Version: 5.0.0
+Version: 5.1.0
 Summary: Direct usage of Cinder Block Storage drivers without the services
 Home-page: https://docs.openstack.org/cinderlib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Direct usage of Cinder Block Storage drivers without the services
 Platform: UNKNOWN
@@ -16,8 +16,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `cinderlib-5.0.0/cinderlib.egg-info/SOURCES.txt` & `cinderlib-5.1.0/cinderlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
+releasenotes/source/zed.rst
 roles/run-cinderlib-tests/README.rst
 roles/run-cinderlib-tests/defaults/main.yaml
 roles/run-cinderlib-tests/tasks/main.yaml
 tools/coding-checks.sh
 tools/fast8.sh
 tools/generate_uc.sh
 tools/lvm-prepare.sh
```

### Comparing `cinderlib-5.0.0/devstack/README.rst` & `cinderlib-5.1.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/devstack/plugin.sh` & `cinderlib-5.1.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/Makefile` & `cinderlib-5.1.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/conf.py` & `cinderlib-5.1.0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 master_doc = 'index'
 
 # List of directories, relative to source directory, that shouldn't be searched
 # for source files.
 exclude_trees = []
 
 # General information about the project.
-copyright = u"2017, Cinder Developers"
+copyright = "2017, Cinder Developers"
 
 # openstackdocstheme options
 openstackdocs_repo_name = 'openstack/cinderlib'
 openstackdocs_pdf_link = True
 openstackdocs_bug_project = 'cinderlib'
 openstackdocs_bug_tag = ''
```

### Comparing `cinderlib-5.0.0/doc/source/contributor/contributing.rst` & `cinderlib-5.1.0/doc/source/contributor/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -112,27 +112,27 @@
      # Use cinder and os-brick from the appropriate development branch instead of
      # from PyPi.  Defining the egg name we won't overwrite the package installed
      # by Zuul on jobs supporting cross-project dependencies (include Cinder in
      # required-projects).  This allows us to also run local tests against the
      # latest cinder/brick code instead of released code.
      # NOTE: Functional tests may fail if host is missing bindeps from deps projects
      deps= -r{toxinidir}/test-requirements.txt
-           git+https://opendev.org/openstack/os-brick#egg=os-brick
-           git+https://opendev.org/openstack/cinder#egg=cinder
+           git+https://opendev.org/openstack/os-brick
+           git+https://opendev.org/openstack/cinder
 
 * When the coordinated release for cycle 'n' has occurred, cinderlib's
   ``tox.ini`` in master must be modified so that cinderlib is being tested
   against cinder and os-brick from the stable branches for the 'n' release (in
   this example, stable/yoga):
 
   .. code-block::
 
      deps = -r{toxinidir}/test-requirements.txt
-            git+https://opendev.org/openstack/os-brick@stable/yoga#egg=os-brick
-            git+https://opendev.org/openstack/cinder@stable/yoga#egg=cinder
+            git+https://opendev.org/openstack/os-brick@stable/yoga
+            git+https://opendev.org/openstack/cinder@stable/yoga
 
 * After the 'n' release of cinderlib occurs (and the stable/n branch is cut),
   all of cinder, os-brick, and cinderlib master branches are all 'n+1' cycle
   development branches, so:
 
   * The base testenv in ``tox.ini`` in master must be modified to use cinder
     and os-brick from master for testing, reverting the first code block change
```

### Comparing `cinderlib-5.0.0/doc/source/index.rst` & `cinderlib-5.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/installation.rst` & `cinderlib-5.1.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/limitations.rst` & `cinderlib-5.1.0/doc/source/limitations.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/make.bat` & `cinderlib-5.1.0/doc/source/make.bat`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/backends.rst` & `cinderlib-5.1.0/doc/source/topics/backends.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/connections.rst` & `cinderlib-5.1.0/doc/source/topics/connections.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/initialization.rst` & `cinderlib-5.1.0/doc/source/topics/initialization.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/metadata.rst` & `cinderlib-5.1.0/doc/source/topics/metadata.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/serialization.rst` & `cinderlib-5.1.0/doc/source/topics/serialization.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/snapshots.rst` & `cinderlib-5.1.0/doc/source/topics/snapshots.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/tracking.rst` & `cinderlib-5.1.0/doc/source/topics/tracking.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/topics/volumes.rst` & `cinderlib-5.1.0/doc/source/topics/volumes.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/usage.rst` & `cinderlib-5.1.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/validated.rst` & `cinderlib-5.1.0/doc/source/validated.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/doc/source/validating.rst` & `cinderlib-5.1.0/doc/source/validating.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/playbooks/required-projects-bindeps.yaml` & `cinderlib-5.1.0/playbooks/required-projects-bindeps.yaml`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/playbooks/setup-ceph.yaml` & `cinderlib-5.1.0/playbooks/setup-ceph.yaml`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/playbooks/setup-lvm.yaml` & `cinderlib-5.1.0/playbooks/setup-lvm.yaml`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/releasenotes/notes/cinderlib-a458b8e23b6d35f4.yaml` & `cinderlib-5.1.0/releasenotes/notes/cinderlib-a458b8e23b6d35f4.yaml`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/releasenotes/notes/fake-packages-7d5c55e6169f1096.yaml` & `cinderlib-5.1.0/releasenotes/notes/fake-packages-7d5c55e6169f1096.yaml`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/releasenotes/source/conf.py` & `cinderlib-5.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/roles/run-cinderlib-tests/README.rst` & `cinderlib-5.1.0/roles/run-cinderlib-tests/README.rst`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/setup.cfg` & `cinderlib-5.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	cinderlib
 package_data = 
 	cinderlib.bin = *
```

### Comparing `cinderlib-5.0.0/setup.py` & `cinderlib-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/test-requirements.txt` & `cinderlib-5.1.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tools/coding-checks.sh` & `cinderlib-5.1.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tools/fast8.sh` & `cinderlib-5.1.0/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tools/generate_uc.sh` & `cinderlib-5.1.0/tools/generate_uc.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tools/special_install.sh` & `cinderlib-5.1.0/tools/special_install.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tools/virtualenv-sudo.sh` & `cinderlib-5.1.0/tools/virtualenv-sudo.sh`

 * *Files identical despite different names*

### Comparing `cinderlib-5.0.0/tox.ini` & `cinderlib-5.1.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 [tox]
 minversion = 3.18.0
+# Tox 4 gives errors as if the entry_points of setup.cfg were not available
+# during tests.
+requires =
+  virtualenv>=20.4.2
+  tox<4
 # python runtimes: https://governance.openstack.org/tc/reference/project-testing-interface.html#tested-runtimes
 envlist = py3,pep8
 skipsdist = True
 # setting ignore_basepython_conflict allows tox to infer the base python
 # from the environment name and override any basepython configured in this file
 ignore_basepython_conflict=true
 
@@ -13,61 +18,66 @@
          OS_STDERR_CAPTURE=1
          OS_TEST_TIMEOUT=60
          OS_TEST_PATH=./cinderlib/tests/unit
          VIRTUAL_ENV={envdir}
          TOX_INI_DIR={toxinidir}
          # make sure this is accurate for current development, both here
          # and in [testenv:functional]
-         CINDERLIB_RELEASE=zed
+         CINDERLIB_RELEASE=2023.1
 usedevelop=True
 
 # note: cannot set the special local install command here because it is also
 # applied if tox has to update itself to meet the minversion specified above
 
 # Use cinder and os-brick from the appropriate development branch instead of
 # from PyPi.  Defining the egg name we won't overwrite the package installed
 # by Zuul on jobs supporting cross-project dependencies (include Cinder in
 # required-projects).  This allows us to also run local tests against the
 # latest cinder/brick code instead of released code.
 # NOTE: Functional tests may fail if host is missing bindeps from deps projects
 deps =
     -r{toxinidir}/test-requirements.txt
-    git+https://opendev.org/openstack/os-brick@stable/zed#egg=os-brick
-    git+https://opendev.org/openstack/cinder@stable/zed#egg=cinder
+    git+https://opendev.org/openstack/os-brick@stable/2023.1
+    git+https://opendev.org/openstack/cinder@stable/2023.1
 
 commands =
     find . -ignore_readdir_race -type f -name "*.pyc" -delete
-    # FIXME: figure out why these need to be run in extreme isolation
-    stestr run --exclude-regex cinderlib.tests.unit.persistence.test_dbms {posargs}
-    stestr run --combine {posargs} cinderlib.tests.unit.persistence.test_dbms.TestDBPersistence
-    stestr run --combine {posargs} cinderlib.tests.unit.persistence.test_dbms.TestMemoryDBPersistence
-    # TODO: figure out how to arrange the above so that you can run a
-    # a single test.  For example, invoking
-    #   tox -e py310 -- cinderlib.tests.unit.test_cinderlib.TestCinderlib.test__set_priv_helper
-    # runs that test and then TestDBPersistence tests and then TestMemoryDBPersistence tests
+    stestr run {posargs}
     stestr slowest
 
 allowlist_externals =
   bash
   find
-passenv = *_proxy *_PROXY CINDERLIB_CONSTRAINTS_FILE
+passenv =
+  *_proxy
+  *_PROXY
+  CINDERLIB_CONSTRAINTS_FILE
+
+[testenv:py{3,38,39,310,311}]
+allowlist_externals =
+  {[testenv]allowlist_externals}
+  {toxinidir}/tools/special_install.sh
+  {toxinidir}/tools/generate_uc.sh
 
-[testenv:py{3,38,39,310}]
 install_command = {toxinidir}/tools/special_install.sh {env:PIP_OPTIONS:} {opts} {packages}
 
 [testenv:functional]
 install_command = {[testenv:py3]install_command}
 usedevelop=True
-passenv = CL_FTEST_POOL_NAME CL_FTEST_LOGGING CL_FTEST_DEBUG CINDERLIB_CONSTRAINTS_FILE
+passenv =
+  CL_FTEST_POOL_NAME
+  CL_FTEST_LOGGING
+  CL_FTEST_DEBUG
+  CINDERLIB_CONSTRAINTS_FILE
 setenv = OS_TEST_PATH=./cinderlib/tests/functional
          CL_FTEST_CFG={env:CL_FTEST_CFG:{toxinidir}/cinderlib/tests/functional/lvm.yaml}
          CL_FTEST_ROOT_HELPER={env:CL_FTEST_ROOT_HELPER:{toxinidir}/tools/virtualenv-sudo.sh}
          TOX_INI_DIR={toxinidir}
          # make sure this is accurate for current development
-         CINDERLIB_RELEASE=zed
+         CINDERLIB_RELEASE=2023.1
 
 sitepackages = True
 # Not reusing py37's env due to https://github.com/tox-dev/tox/issues/477
 # envdir = {toxworkdir}/py37
 
 # Must run serially or test_stats_with_creation may fail occasionally
 commands =
@@ -75,18 +85,18 @@
     # run stestr through python -m so that the python from the virtualenv
     # is used; stestr's shebang may point to system python, thus breaking
     # the lookup of modules from the venv.
     python -m stestr run --serial {posargs}
     python -m stestr slowest
 
 allowlist_externals =
-  {[testenv]allowlist_externals}
+  {[testenv:py3]allowlist_externals}
   stestr
 
-[testenv:functional-py{38,39,310}]
+[testenv:functional-py{38,39,310,311}]
 install_command = {[testenv:functional]install_command}
 usedevelop=True
 passenv =
   {[testenv:functional]passenv}
 setenv =
   {[testenv:functional]setenv}
 sitepackages = True
@@ -103,15 +113,15 @@
   -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:docs]
 # yes, we want the constraint in the install_command, not deps, so that
 # https://review.opendev.org/c/openstack/glance/+/839786 does not happen
 # to us
-install_command = python -m pip install -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/zed} {opts} {packages}
+install_command = python -m pip install -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1} {opts} {packages}
 deps =
   -r{toxinidir}/doc/requirements.txt
 commands =
   doc8 --ignore D001 --ignore-path .tox --ignore-path *.egg-info --ignore-path doc/build --ignore-path .eggs/*/EGG-INFO/*.txt -e txt -e rst
   rm -rf doc/build .autogenerated doc/source/api
   sphinx-build -W -b html doc/source doc/build/html
   rm -rf api-ref/build
@@ -177,8 +187,9 @@
     -r{toxinidir}/test-requirements.txt
 
 [testenv:fast8]
 # Not reusing Flake8's env due to https://github.com/tox-dev/tox/issues/477
 # envdir = {toxworkdir}/flake8
 install_command = {[testenv:docs]install_command}
 commands={toxinidir}/tools/fast8.sh
-passenv = FAST8_NUM_COMMITS
+passenv =
+  FAST8_NUM_COMMITS
```

