# Comparing `tmp/jaxsim-0.1.dev149.tar.gz` & `tmp/jaxsim-0.1.dev151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev149.tar", last modified: Wed May  3 16:14:47 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev151.tar", last modified: Thu May  4 08:06:03 2023, max compression
```

## Comparing `jaxsim-0.1.dev149.tar` & `jaxsim-0.1.dev151.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.990727 jaxsim-0.1.dev149/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.994727 jaxsim-0.1.dev149/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.990727 jaxsim-0.1.dev149/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.002728 jaxsim-0.1.dev149/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.006729 jaxsim-0.1.dev149/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.006729 jaxsim-0.1.dev149/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:47.010729 jaxsim-0.1.dev149/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-03 16:14:28.000000 jaxsim-0.1.dev149/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:46.998728 jaxsim-0.1.dev149/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 16:14:46.000000 jaxsim-0.1.dev149/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.444613 jaxsim-0.1.dev151/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.428613 jaxsim-0.1.dev151/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.432613 jaxsim-0.1.dev151/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-04 08:06:03.444613 jaxsim-0.1.dev151/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 08:06:03.444613 jaxsim-0.1.dev151/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.428613 jaxsim-0.1.dev151/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.432613 jaxsim-0.1.dev151/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.432613 jaxsim-0.1.dev151/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37704 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.436613 jaxsim-0.1.dev151/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.436613 jaxsim-0.1.dev151/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.436613 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.436613 jaxsim-0.1.dev151/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.436613 jaxsim-0.1.dev151/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.440613 jaxsim-0.1.dev151/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.440613 jaxsim-0.1.dev151/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.440613 jaxsim-0.1.dev151/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.440613 jaxsim-0.1.dev151/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-04 08:05:43.000000 jaxsim-0.1.dev151/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:03.432613 jaxsim-0.1.dev151/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 08:06:03.000000 jaxsim-0.1.dev151/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev149/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev151/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/.github/workflows/style.yml` & `jaxsim-0.1.dev151/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/.gitignore` & `jaxsim-0.1.dev151/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/LICENSE` & `jaxsim-0.1.dev151/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/PKG-INFO` & `jaxsim-0.1.dev151/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev149
+Version: 0.1.dev151
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev149/README.md` & `jaxsim-0.1.dev151/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/setup.cfg` & `jaxsim-0.1.dev151/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/__init__.py` & `jaxsim-0.1.dev151/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev151/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev151/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev151/src/jaxsim/high_level/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/logging.py` & `jaxsim-0.1.dev151/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev151/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev151/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev151/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev151/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev151/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev151/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev151/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev151/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev151/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/rod/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev151/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev151/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import jax_dataclasses
 
 import jaxsim.high_level
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.physics
 import jaxsim.simulation.simulator_callbacks as scb
 import jaxsim.typing as jtp
+from jaxsim import logging
 from jaxsim.high_level.common import VelRepr
 from jaxsim.high_level.model import Model, StepData
 from jaxsim.physics.algos.soft_contacts import SoftContactsParams
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.physics.model.physics_model import PhysicsModel
 from jaxsim.simulation import ode_integration
 from jaxsim.utils import JaxsimDataclass
@@ -214,37 +215,36 @@
         self.data.gravity = gravity
 
         for model_name, model in self.data.models.items():
             model.physics_model.set_gravity(gravity=gravity)
 
         self._set_mutability(self._mutability())
 
-    def insert_model_from_sdf(
+    def insert_model_from_description(
         self,
-        sdf: Union[pathlib.Path, str],
-        model_name: str = None,
-        considered_joints: List[str] = None,
+        model_description: Union[pathlib.Path, str],
+        model_name: Optional[str] = None,
+        considered_joints: Optional[List[str]] = None,
     ) -> Model:
         """
-        Insert a model from an SDF resource.
+        Insert a model from a model description.
 
         Args:
-            sdf: The SDF resource.
-            model_name: Optional name of the model to insert.
-                        It defaults to the name of the model found in the SDF resource.
+            model_description: Either a path to a file or a string containing the URDF/SDF description.
+            model_name: The optional name of the model that overrides the one in the description.
             considered_joints: Optional list of joints to consider.
                                It is also useful to specify the joint serialization.
 
         Returns:
             The newly inserted model.
         """
 
-        # Build the model from the input SDF resource
-        model = jaxsim.high_level.model.Model.build_from_sdf(
-            sdf=sdf,
+        # Build the model from the given model description
+        model = jaxsim.high_level.model.Model.build_from_model_description(
+            model_description=model_description,
             model_name=model_name,
             vel_repr=self.velocity_representation,
             considered_joints=considered_joints,
         )
 
         # Make sure the model is not already part of the simulation
         if model.name() in self.model_names():
@@ -257,14 +257,35 @@
         # Propagate the current mutability property to make sure that also the
         # newly inserted model matches the mutability of the simulator
         self._set_mutability(self._mutability())
 
         # Return the newly inserted model
         return self.data.models[model.name()]
 
+    def insert_model_from_sdf(
+        self,
+        sdf: Union[pathlib.Path, str],
+        model_name: str = None,
+        considered_joints: List[str] = None,
+    ) -> Model:
+        """
+        Insert a model from an SDF resource.
+        """
+
+        msg = "JaxSim.{} is deprecated, use JaxSim.{} instead."
+        logging.warning(
+            msg=msg.format("insert_model_from_sdf", "insert_model_from_description")
+        )
+
+        return self.insert_model_from_description(
+            model_description=sdf,
+            model_name=model_name,
+            considered_joints=considered_joints,
+        )
+
     def insert_model(
         self, model_description: descriptions.ModelDescription, model_name: str = None
     ) -> Model:
         """
         Insert a model from a model description object.
 
         Args:
```

### Comparing `jaxsim-0.1.dev149/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev151/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/typing.py` & `jaxsim-0.1.dev151/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim/utils.py` & `jaxsim-0.1.dev151/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev149/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev151/src/jaxsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev149
+Version: 0.1.dev151
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev149/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev151/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

