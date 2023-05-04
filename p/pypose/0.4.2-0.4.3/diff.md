# Comparing `tmp/pypose-0.4.2.tar.gz` & `tmp/pypose-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.4.2.tar", last modified: Wed Apr 12 04:19:37 2023, max compression
+gzip compressed data, was "pypose-0.4.3.tar", last modified: Thu May  4 17:45:27 2023, max compression
```

## Comparing `pypose-0.4.2.tar` & `pypose-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.694546 pypose-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-12 04:19:20.000000 pypose-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-12 04:19:37.694546 pypose-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-04-12 04:19:20.000000 pypose-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose/function/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/function/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/pnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.690546 pypose-0.4.2/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-04-12 04:19:20.000000 pypose-0.4.2/pypose/utils/collect_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.686546 pypose-0.4.2/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:19:37.000000 pypose-0.4.2/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:19:37.694546 pypose-0.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 04:19:20.000000 pypose-0.4.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 04:19:20.000000 pypose-0.4.2/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:19:37.694546 pypose-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-12 04:19:20.000000 pypose-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-04 17:45:11.000000 pypose-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-04 17:45:27.624483 pypose-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-04 17:45:11.000000 pypose-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/function/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-04 17:45:11.000000 pypose-0.4.3/pypose/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.620483 pypose-0.4.3/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:45:27.000000 pypose-0.4.3/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:45:27.624483 pypose-0.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 17:45:11.000000 pypose-0.4.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 17:45:11.000000 pypose-0.4.3/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:45:27.624483 pypose-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-04 17:45:11.000000 pypose-0.4.3/setup.py
```

### Comparing `pypose-0.4.2/LICENSE` & `pypose-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/PKG-INFO` & `pypose-0.4.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.2
+Version: 0.4.3
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang
 Author-email: chenwang@dr.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
@@ -52,16 +52,19 @@
 ##### [LieTensor](https://pypose.org/docs/main/modules/)
 
 - Lie group: [`SO3`](https://pypose.org/docs/main/generated/pypose.SO3/), [`SE3`](https://pypose.org/docs/main/generated/pypose.SE3/), [`Sim3`](https://pypose.org/docs/main/generated/pypose.Sim3/), [`RxSO3`](https://pypose.org/docs/main/generated/pypose.RxSO3/)
 - Lie algebra: [`so3`](https://pypose.org/docs/main/generated/pypose.so3/), [`se3`](https://pypose.org/docs/main/generated/pypose.se3/), [`sim3`](https://pypose.org/docs/main/generated/pypose.sim3/), [`rxso3`](https://pypose.org/docs/main/generated/pypose.rxso3/)
 
 ##### [Modules](https://pypose.org/docs/main/modules/)
 
-- [`System`](https://pypose.org/docs/main/generated/pypose.module.System)
-- [`IMUPreintegration`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
+- System: [`LTI`](https://pypose.org/docs/main/generated/pypose.module.LTI), [`LTV`](https://pypose.org/docs/main/generated/pypose.module.LTV), [`NLS`](https://pypose.org/docs/main/generated/pypose.module.NLS)
+- Filter: [`EKF`](https://pypose.org/docs/main/generated/pypose.module.EKF/), [`UKF`](https://pypose.org/docs/main/generated/pypose.module.UKF/), [`PF`](https://pypose.org/docs/main/generated/pypose.module.PF/)
+- PnP Solver: [`EPnP`](https://pypose.org/docs/main/generated/pypose.module.EPnP/)
+- Linear Quadratic Regulator: [`LQR`](https://pypose.org/docs/main/generated/pypose.module.LQR/)
+- IMU Preintegration: [`IMUPreintegrator`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
 - ......
 
 ##### [Second-order Optimizers](https://pypose.org/docs/main/optim/)
 
 - [`GaussNewton`](https://pypose.org/docs/main/generated/pypose.optim.GaussNewton)
 - [`LevenbergMarquardt`](https://pypose.org/docs/main/generated/pypose.optim.LevenbergMarquardt/)
 - ......
```

### Comparing `pypose-0.4.2/README.md` & `pypose-0.4.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 ##### [LieTensor](https://pypose.org/docs/main/modules/)
 
 - Lie group: [`SO3`](https://pypose.org/docs/main/generated/pypose.SO3/), [`SE3`](https://pypose.org/docs/main/generated/pypose.SE3/), [`Sim3`](https://pypose.org/docs/main/generated/pypose.Sim3/), [`RxSO3`](https://pypose.org/docs/main/generated/pypose.RxSO3/)
 - Lie algebra: [`so3`](https://pypose.org/docs/main/generated/pypose.so3/), [`se3`](https://pypose.org/docs/main/generated/pypose.se3/), [`sim3`](https://pypose.org/docs/main/generated/pypose.sim3/), [`rxso3`](https://pypose.org/docs/main/generated/pypose.rxso3/)
 
 ##### [Modules](https://pypose.org/docs/main/modules/)
 
-- [`System`](https://pypose.org/docs/main/generated/pypose.module.System)
-- [`IMUPreintegration`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
+- System: [`LTI`](https://pypose.org/docs/main/generated/pypose.module.LTI), [`LTV`](https://pypose.org/docs/main/generated/pypose.module.LTV), [`NLS`](https://pypose.org/docs/main/generated/pypose.module.NLS)
+- Filter: [`EKF`](https://pypose.org/docs/main/generated/pypose.module.EKF/), [`UKF`](https://pypose.org/docs/main/generated/pypose.module.UKF/), [`PF`](https://pypose.org/docs/main/generated/pypose.module.PF/)
+- PnP Solver: [`EPnP`](https://pypose.org/docs/main/generated/pypose.module.EPnP/)
+- Linear Quadratic Regulator: [`LQR`](https://pypose.org/docs/main/generated/pypose.module.LQR/)
+- IMU Preintegration: [`IMUPreintegrator`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
 - ......
 
 ##### [Second-order Optimizers](https://pypose.org/docs/main/optim/)
 
 - [`GaussNewton`](https://pypose.org/docs/main/generated/pypose.optim.GaussNewton)
 - [`LevenbergMarquardt`](https://pypose.org/docs/main/generated/pypose.optim.LevenbergMarquardt/)
 - ......
```

### Comparing `pypose-0.4.2/pypose/__init__.py` & `pypose-0.4.3/pypose/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/basics/ops.py` & `pypose-0.4.3/pypose/basics/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/function/linalg.py` & `pypose-0.4.3/pypose/function/linalg.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/__init__.py` & `pypose-0.4.3/pypose/lietensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/basics.py` & `pypose-0.4.3/pypose/lietensor/basics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/convert.py` & `pypose-0.4.3/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/lietensor.py` & `pypose-0.4.3/pypose/lietensor/lietensor.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/operation.py` & `pypose-0.4.3/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/lietensor/utils.py` & `pypose-0.4.3/pypose/lietensor/utils.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/dynamics.py` & `pypose-0.4.3/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/ekf.py` & `pypose-0.4.3/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/imu_preintegrator.py` & `pypose-0.4.3/pypose/module/imu_preintegrator.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/lqr.py` & `pypose-0.4.3/pypose/module/lqr.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/pf.py` & `pypose-0.4.3/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/module/pnp.py` & `pypose-0.4.3/pypose/module/pnp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import torch
 from torch.linalg import vecdot
 from torch import broadcast_shapes
 
-from .. import mat2SE3
-from .. import bmv, bvv
+from .. import bmv
 from ..optim import GaussNewton
 from ..optim.solver import LSTSQ
 from ..optim.scheduler import StopOnPlateau
-from ..function import reprojerr, cart2homo
+from ..function import reprojerr, cart2homo, svdtf
 
 
 class BetaObjective(torch.nn.Module):
     # Optimize the beta according to the objective in the ePnP paper.
     def __init__(self, beta):
         super().__init__()
         self.beta = torch.nn.Parameter(beta)
@@ -167,15 +166,15 @@
             pose, scale = self._compute_solution(beta, nullv, alpha, points)
 
         return pose
 
     def _compute_solution(self, beta, nullv, alpha, points):
         bases = bmv(nullv.mT, beta)
         bases, transp, scale = self._compute_scale(bases, alpha, points)
-        pose = self._points_transform(points, transp)
+        pose = svdtf(points, transp)
         return pose, scale
 
     @staticmethod
     def _best_solution(errors, poses, betas, scales):
         _, idx = torch.min(errors.mean(dim=-1, keepdim=True), dim=0, keepdim=True)
         pose = poses.gather(0, index=idx.tile(poses.size(-1))).squeeze(0)
         beta = betas.gather(0, index=idx.tile(betas.size(-1))).squeeze(0)
@@ -285,24 +284,7 @@
         bases = bases * scale[..., None, None] # the real position
         scalep = alpha @ bases # scaled transformed points
         mask = torch.any(scalep[..., 2] < 0, dim=-1) # negate when z < 0
         sign = torch.ones_like(scale) - mask * 2     # 1 or -1
         scalep = sign[..., None, None] * scalep
         scale = (sign * scale).unsqueeze(-1)
         return bases, scalep, scale
-
-    @staticmethod
-    def _points_transform(pts_w, pts_c):
-        # Get transform for two associated batched point sets.
-        Cw = pts_w.mean(dim=-2, keepdim=True)
-        Pw = pts_w - Cw
-        Cc = pts_c.mean(dim=-2, keepdim=True)
-        Pc = pts_c - Cc
-        M = bvv(Pc, Pw).sum(dim=-3)
-        U, S, Vh = torch.linalg.svd(M)
-        R = U @ Vh
-        # mirror improper rotation that det(R) = -1
-        mask = (R.det() + 1).abs() < 1e-6
-        R[mask] = - R[mask]
-        t = Cc.mT - R @ Cw.mT
-        T = torch.cat((R, t), dim=-1)
-        return mat2SE3(T, check=False)
```

### Comparing `pypose-0.4.2/pypose/module/ukf.py` & `pypose-0.4.3/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/corrector.py` & `pypose-0.4.3/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/functional.py` & `pypose-0.4.3/pypose/optim/functional.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/kernel.py` & `pypose-0.4.3/pypose/optim/kernel.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/optimizer.py` & `pypose-0.4.3/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/scheduler.py` & `pypose-0.4.3/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/solver.py` & `pypose-0.4.3/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/optim/strategy.py` & `pypose-0.4.3/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose/utils/collect_env.py` & `pypose-0.4.3/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.2/pypose.egg-info/PKG-INFO` & `pypose-0.4.3/pypose.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.2
+Version: 0.4.3
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang
 Author-email: chenwang@dr.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
@@ -52,16 +52,19 @@
 ##### [LieTensor](https://pypose.org/docs/main/modules/)
 
 - Lie group: [`SO3`](https://pypose.org/docs/main/generated/pypose.SO3/), [`SE3`](https://pypose.org/docs/main/generated/pypose.SE3/), [`Sim3`](https://pypose.org/docs/main/generated/pypose.Sim3/), [`RxSO3`](https://pypose.org/docs/main/generated/pypose.RxSO3/)
 - Lie algebra: [`so3`](https://pypose.org/docs/main/generated/pypose.so3/), [`se3`](https://pypose.org/docs/main/generated/pypose.se3/), [`sim3`](https://pypose.org/docs/main/generated/pypose.sim3/), [`rxso3`](https://pypose.org/docs/main/generated/pypose.rxso3/)
 
 ##### [Modules](https://pypose.org/docs/main/modules/)
 
-- [`System`](https://pypose.org/docs/main/generated/pypose.module.System)
-- [`IMUPreintegration`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
+- System: [`LTI`](https://pypose.org/docs/main/generated/pypose.module.LTI), [`LTV`](https://pypose.org/docs/main/generated/pypose.module.LTV), [`NLS`](https://pypose.org/docs/main/generated/pypose.module.NLS)
+- Filter: [`EKF`](https://pypose.org/docs/main/generated/pypose.module.EKF/), [`UKF`](https://pypose.org/docs/main/generated/pypose.module.UKF/), [`PF`](https://pypose.org/docs/main/generated/pypose.module.PF/)
+- PnP Solver: [`EPnP`](https://pypose.org/docs/main/generated/pypose.module.EPnP/)
+- Linear Quadratic Regulator: [`LQR`](https://pypose.org/docs/main/generated/pypose.module.LQR/)
+- IMU Preintegration: [`IMUPreintegrator`](https://pypose.org/docs/main/generated/pypose.module.IMUPreintegrator/)
 - ......
 
 ##### [Second-order Optimizers](https://pypose.org/docs/main/optim/)
 
 - [`GaussNewton`](https://pypose.org/docs/main/generated/pypose.optim.GaussNewton)
 - [`LevenbergMarquardt`](https://pypose.org/docs/main/generated/pypose.optim.LevenbergMarquardt/)
 - ......
```

### Comparing `pypose-0.4.2/pypose.egg-info/SOURCES.txt` & `pypose-0.4.3/pypose.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 pypose/lietensor/convert.py
 pypose/lietensor/lietensor.py
 pypose/lietensor/operation.py
 pypose/lietensor/utils.py
 pypose/module/__init__.py
 pypose/module/dynamics.py
 pypose/module/ekf.py
+pypose/module/icp.py
 pypose/module/imu_preintegrator.py
 pypose/module/lqr.py
 pypose/module/pf.py
 pypose/module/pnp.py
 pypose/module/ukf.py
 pypose/optim/__init__.py
 pypose/optim/corrector.py
@@ -34,9 +35,10 @@
 pypose/optim/kernel.py
 pypose/optim/optimizer.py
 pypose/optim/scheduler.py
 pypose/optim/solver.py
 pypose/optim/strategy.py
 pypose/utils/__init__.py
 pypose/utils/collect_env.py
+pypose/utils/stepper.py
 requirements/docs.txt
 requirements/runtime.txt
```

### Comparing `pypose-0.4.2/setup.py` & `pypose-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         license_files = ('LICENSE',),
         description = 'To connect classic robotics with modern learning methods.',
         long_description=long_description,
         long_description_content_type='text/markdown',
         python_requires='>=3.6',
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
-        packages=find_packages(exclude=('docs', 'test', 'examples')),
+        packages=find_packages(exclude=('docs', 'tests', 'examples')),
         data_files=[('', ['requirements/runtime.txt', 'requirements/docs.txt'])],
         zip_safe=True,
         install_requires = load_requirements("requirements/runtime.txt"),
         extras_require = requirements_extras,
         keywords=['robotics', 'deep learning', 'pytorch'],
         project_urls={
             "Bug Tracker": "https://github.com/pypose/pypose/issues",
```

