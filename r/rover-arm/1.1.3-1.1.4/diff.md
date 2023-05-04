# Comparing `tmp/rover_arm-1.1.3.tar.gz` & `tmp/rover_arm-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.1.3.tar", last modified: Wed May  3 00:13:17 2023, max compression
+gzip compressed data, was "rover_arm-1.1.4.tar", last modified: Thu May  4 06:33:10 2023, max compression
```

## Comparing `rover_arm-1.1.3.tar` & `rover_arm-1.1.4.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:17.000338 rover_arm-1.1.3/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.3/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      188 2023-03-31 22:22:55.000000 rover_arm-1.1.3/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.3/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-03 00:13:17.000198 rover_arm-1.1.3/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-03-31 23:16:16.000000 rover_arm-1.1.3/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.985662 rover_arm-1.1.3/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-31 06:14:48.000000 rover_arm-1.1.3/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      231 2023-04-27 19:25:40.000000 rover_arm-1.1.3/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.986496 rover_arm-1.1.3/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.986641 rover_arm-1.1.3/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.988144 rover_arm-1.1.3/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.996324 rover_arm-1.1.3/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.3/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.999697 rover_arm-1.1.3/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      243 2023-03-30 23:20:23.000000 rover_arm-1.1.3/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.999976 rover_arm-1.1.3/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.3/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     7093 2023-05-02 23:58:57.000000 rover_arm-1.1.3/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    11158 2023-05-03 00:12:23.000000 rover_arm-1.1.3/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.3/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.3/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.3/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-03 00:13:16.986259 rover_arm-1.1.3/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-03 00:13:16.000000 rover_arm-1.1.3/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1740 2023-05-03 00:13:16.000000 rover_arm-1.1.3/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-03 00:13:16.000000 rover_arm-1.1.3/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       27 2023-05-03 00:13:16.000000 rover_arm-1.1.3/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-03 00:13:16.000000 rover_arm-1.1.3/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-03 00:13:17.000388 rover_arm-1.1.3/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      570 2023-05-03 00:13:14.000000 rover_arm-1.1.3/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.783746 rover_arm-1.1.4/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-04-27 19:16:14.000000 rover_arm-1.1.4/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      197 2023-05-03 00:46:42.000000 rover_arm-1.1.4/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.4/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-04 06:33:10.783601 rover_arm-1.1.4/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2058 2023-05-03 22:23:09.000000 rover_arm-1.1.4/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.751054 rover_arm-1.1.4/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-05-03 22:23:09.000000 rover_arm-1.1.4/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      394 2023-05-04 06:29:52.000000 rover_arm-1.1.4/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.752760 rover_arm-1.1.4/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.753171 rover_arm-1.1.4/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.756258 rover_arm-1.1.4/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.775561 rover_arm-1.1.4/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.4/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.782423 rover_arm-1.1.4/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      302 2023-05-04 06:31:51.000000 rover_arm-1.1.4/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.783216 rover_arm-1.1.4/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-03-31 05:40:01.000000 rover_arm-1.1.4/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6675 2023-05-03 22:23:09.000000 rover_arm-1.1.4/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11158 2023-05-03 00:12:23.000000 rover_arm-1.1.4/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.4/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11158 2023-05-04 06:27:13.000000 rover_arm-1.1.4/rover_arm/envs/roverarm_env_gym.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.4/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.4/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-04 06:33:10.752227 rover_arm-1.1.4/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2236 2023-05-04 06:33:10.000000 rover_arm-1.1.4/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1775 2023-05-04 06:33:10.000000 rover_arm-1.1.4/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-04 06:33:10.000000 rover_arm-1.1.4/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       37 2023-05-04 06:33:10.000000 rover_arm-1.1.4/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-04 06:33:10.000000 rover_arm-1.1.4/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-04 06:33:10.783803 rover_arm-1.1.4/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      583 2023-05-04 06:26:10.000000 rover_arm-1.1.4/setup.py
```

### Comparing `rover_arm-1.1.3/.DS_Store` & `rover_arm-1.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/PKG-INFO` & `rover_arm-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover_arm
-Version: 1.1.3
+Version: 1.1.4
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.3/README.md` & `rover_arm-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/.DS_Store` & `rover_arm-1.1.4/rover_arm/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0010  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
 00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,86 +26,86 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
+00000210: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
+00000220: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
+00000230: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
+00000240: 0000 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
+00000250: 0061 0063 0068 0065 005f 005f 6c67 3153  .a.c.h.e._._lg1S
+00000260: 636f 6d70 0000 0000 0000 0984 0000 000b  comp............
+00000270: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000280: 0065 005f 005f 6d6f 4444 626c 6f62 0000  .e._._moDDblob..
+00000290: 0008 a125 7c7e 06eb c441 0000 000b 005f  ...%|~...A....._
+000002a0: 005f 0070 0079 0063 0061 0063 0068 0065  ._.p.y.c.a.c.h.e
+000002b0: 005f 005f 6d6f 6444 626c 6f62 0000 0008  ._._modDblob....
+000002c0: a125 7c7e 06eb c441 0000 000b 005f 005f  .%|~...A....._._
+000002d0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
+000002e0: 005f 7068 3153 636f 6d70 0000 0000 0000  ._ph1Scomp......
+000002f0: 2000 0000 0004 0064 0061 0074 0061 496c   ......d.a.t.aIl
+00000300: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
+00000310: 002e ffff ffff ffff 0000 0000 0004 0065  ...............e
+00000320: 006e 0076 0073 496c 6f63 626c 6f62 0000  .n.v.sIlocblob..
+00000330: 0010 0000 018b 0000 002e ffff ffff ffff  ................
+00000340: 0000 0000 0013 006b 0065 0079 0062 006f  .......k.e.y.b.o
+00000350: 0061 0072 0064 005f 0063 006f 006e 0074  .a.r.d._.c.o.n.t
+00000360: 0072 006f 006c 002e 0070 0079 496c 6f63  .r.o.l...p.yIloc
+00000370: 626c 6f62 0000 0010 0000 0041 0000 009e  blob.......A....
+00000380: ffff ffff ffff 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0010 0000 000b  ................
-00000410: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
-00000420: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
-00000430: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
-00000440: 0000 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
-00000450: 0061 0063 0068 0065 005f 005f 6c67 3153  .a.c.h.e._._lg1S
-00000460: 636f 6d70 0000 0000 0000 0984 0000 000b  comp............
-00000470: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000480: 0065 005f 005f 6d6f 4444 626c 6f62 0000  .e._._moDDblob..
-00000490: 0008 a125 7c7e 06eb c441 0000 000b 005f  ...%|~...A....._
-000004a0: 005f 0070 0079 0063 0061 0063 0068 0065  ._.p.y.c.a.c.h.e
-000004b0: 005f 005f 6d6f 6444 626c 6f62 0000 0008  ._._modDblob....
-000004c0: a125 7c7e 06eb c441 0000 000b 005f 005f  .%|~...A....._._
-000004d0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
-000004e0: 005f 7068 3153 636f 6d70 0000 0000 0000  ._ph1Scomp......
-000004f0: 2000 0000 0004 0064 0061 0074 0061 496c   ......d.a.t.aIl
-00000500: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
-00000510: 002e ffff ffff ffff 0000 0000 0004 0064  ...............d
-00000520: 0061 0074 0061 6c67 3153 636f 6d70 0000  .a.t.alg1Scomp..
-00000530: 0000 0095 1212 0000 0004 0064 0061 0074  ...........d.a.t
-00000540: 0061 6d6f 4444 626c 6f62 0000 0008 5fdb  .amoDDblob...._.
-00000550: 5efd 6dea c441 0000 0004 0064 0061 0074  ^.m..A.....d.a.t
-00000560: 0061 6d6f 6444 626c 6f62 0000 0008 5fdb  .amodDblob...._.
-00000570: 5efd 6dea c441 0000 0004 0064 0061 0074  ^.m..A.....d.a.t
-00000580: 0061 7068 3153 636f 6d70 0000 0000 0096  .aph1Scomp......
-00000590: 3000 0000 0004 0065 006e 0076 0073 496c  0......e.n.v.sIl
-000005a0: 6f63 626c 6f62 0000 0010 0000 018b 0000  ocblob..........
-000005b0: 002e ffff ffff ffff 0000 0000 0004 0065  ...............e
-000005c0: 006e 0076 0073 6c67 3153 636f 6d70 0000  .n.v.slg1Scomp..
-000005d0: 0000 0000 9863 0000 0004 0065 006e 0076  .....c.....e.n.v
-000005e0: 0073 6d6f 4444 626c 6f62 0000 0008 03b3  .smoDDblob......
-000005f0: 6690 28eb c441 0000 0004 0065 006e 0076  f.(..A.....e.n.v
-00000600: 0073 6d6f 6444 626c 6f62 0000 0008 03b3  .smodDblob......
-00000610: 6690 28eb c441 0000 0004 0065 006e 0076  f.(..A.....e.n.v
-00000620: 0073 7068 3153 636f 6d70 0000 0000 0000  .sph1Scomp......
-00000630: d000 0000 0013 006b 0065 0079 0062 006f  .......k.e.y.b.o
-00000640: 0061 0072 0064 005f 0063 006f 006e 0074  .a.r.d._.c.o.n.t
-00000650: 0072 006f 006c 002e 0070 0079 496c 6f63  .r.o.l...p.yIloc
-00000660: 626c 6f62 0000 0010 0000 0041 0000 009e  blob.......A....
-00000670: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -319,15 +319,15 @@
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
 00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.1.4/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.1.4/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/panda.urdf` & `rover_arm-1.1.4/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/data/rover_arm.xml` & `rover_arm-1.1.4/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.1.4/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue May  2 23:58:37 2023 UTC, .py size: 11164 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,444 +1,418 @@
-00000000: 610d 0d0a 0000 0000 ada3 5164 9c2b 0000  a.........Qd.+..
+00000000: 610d 0d0a 0000 0000 3a75 2664 9f27 0000  a.......:u&d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
-00000030: 6401 6c00 5a01 6400 6402 6c00 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
-00000060: 6401 6c08 5a09 6400 6401 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c0b 5a0b 6400 6401 6c0c 5a0d 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0e 5a0e 6400 6401 6c0f 5a0f 4700  d.l.Z.d.d.l.Z.G.
-00000090: 6404 6405 8400 6405 6501 6a10 8303 5a11  d.d...d.e.j...Z.
+00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
+00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6401 6c06 5a06 6400  m.Z...d.d.l.Z.d.
+00000060: 6401 6c07 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6401 6c0a 5a0a 6400 6401 6c0b 5a0c 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6401 6c0d 5a0d 6400 6401 6c0e 5a0e 4700  d.l.Z.d.d.l.Z.G.
+00000090: 6404 6405 8400 6405 6500 6a0f 8303 5a10  d.d...d.e.j...Z.
 000000a0: 6401 5300 2906 e900 0000 004e 2903 da05  d.S.)......N)...
 000000b0: 6572 726f 72da 0673 7061 6365 73da 0575  error..spaces..u
 000000c0: 7469 6c73 2901 da07 7365 6564 696e 6763  tils)...seedingc
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0600 0000 4000 0000 7352 0000 0065 005a  ....@...sR...e.Z
-000000f0: 0164 005a 0264 0164 0264 0365 03a0 04a1  .d.Z.d.d.d.e....
-00000100: 0064 0464 0466 0664 0564 0684 015a 0564  .d.d.f.d.d...Z.d
-00000110: 1364 0864 0984 015a 0664 0a64 0b84 005a  .d.d...Z.d.d...Z
-00000120: 0764 1464 0d64 0e84 015a 0864 0f64 1084  .d.d.d...Z.d.d..
-00000130: 005a 0964 1164 1284 005a 0a64 0c53 0029  .Z.d.d...Z.d.S.)
-00000140: 15da 0b52 6f76 6572 4172 6d45 6e76 da09  ...RoverArmEnv..
-00000150: 7267 625f 6172 7261 7969 1027 0000 4669  rgb_arrayi.'..Fi
-00000160: e001 0000 6307 0000 0000 0000 0000 0000  ....c...........
-00000170: 0008 0000 000f 0000 0043 0000 0073 8201  .........C...s..
-00000180: 0000 6401 6402 6403 6702 6901 7c00 5f00  ..d.d.d.g.i.|._.
-00000190: 7c01 7c00 5f01 7c03 7c00 5f02 6404 7c00  |.|._.|.|._.d.|.
-000001a0: 5f03 7c04 7c00 5f04 7c02 7c00 5f05 7c05  _.|.|._.|.|._.|.
-000001b0: 7c00 5f06 7c06 7c00 5f07 7c00 6a01 6402  |._.|.|._.|.j.d.
-000001c0: 6b02 7278 7408 a009 7408 6a0a a101 7d07  k.rxt...t.j...}.
-000001d0: 7c07 6405 6b00 7262 7408 a009 7408 6a0b  |.d.k.rbt...t.j.
-000001e0: a101 7d07 7408 a00c 6406 6407 6408 6700  ..}.t...d.d.d.g.
-000001f0: 6409 a201 a104 0100 6e0c 7408 a009 7408  d.......n.t...t.
-00000200: 6a0d a101 0100 640a 7c00 5f0e 640b 7c00  j.....d.|._.d.|.
-00000210: 5f0f 640c 7c00 5f10 6700 640d a201 7c00  _.d.|._.g.d...|.
-00000220: 5f11 7408 6a0c 7c00 6a0e 7c00 6a0f 7c00  _.t.j.|.j.|.j.|.
-00000230: 6a10 7c00 6a11 640e 8d04 0100 7412 a013  j.|.j.d.....t...
-00000240: 7414 a015 640f 6701 6410 1400 a101 7414  t...d.g.d.....t.
-00000250: a015 6411 6701 6410 1400 a101 a102 7c00  ..d.g.d.......|.
-00000260: 5f16 6412 7c00 5f17 7412 a013 7414 a015  _.d.|._.t...t...
-00000270: 7c00 6a17 0b00 7c00 6a17 0b00 7c00 6a17  |.j...|.j...|.j.
-00000280: 0b00 7c00 6a17 0b00 640f 6405 6405 7c00  ..|.j...d.d.d.|.
-00000290: 6a17 0b00 7c00 6a17 0b00 640f 670a a101  j...|.j...d.g...
-000002a0: 7414 a015 7c00 6a17 7c00 6a17 7c00 6a17  t...|.j.|.j.|.j.
-000002b0: 7c00 6a17 6411 6413 6413 7c00 6a17 7c00  |.j.d.d.d.|.j.|.
-000002c0: 6a17 6411 670a a101 a102 7c00 5f18 6405  j.d.g.....|._.d.
-000002d0: 6414 6702 7c00 5f19 6700 6415 a201 7c00  d.g.|._.g.d...|.
-000002e0: 5f1a 6405 7c00 5f1b 6416 7c00 5f1c 6417  _.d.|._.d.|._.d.
-000002f0: 7c00 5f1d 6418 7c00 5f1e 6419 7c00 5f1f  |._.d.|._.d.|._.
-00000300: 6400 5300 291a 4e7a 0c72 656e 6465 722e  d.S.).Nz.render.
-00000310: 6d6f 6465 73da 0568 756d 616e 7207 0000  modes..humanr...
-00000320: 0067 1111 1111 1111 713f 7201 0000 0067  .g......q?r....g
-00000330: cdcc cccc cccc f43f e9b4 0000 0069 d7ff  .......?.....i..
-00000340: ffff 2903 67a4 703d 0ad7 a3e0 3fe7 9a99  ..).g.p=....?...
-00000350: 9999 9999 c9bf 671f 85eb 51b8 1ed5 bfe9  ......g...Q.....
-00000360: 0300 0000 e766 6666 6666 66d6 bf69 ddff  .....ffffff..i..
-00000370: ffff 2903 6771 3d0a d7a3 70e5 3f72 0c00  ..).gq=...p.?r..
-00000380: 0000 679a 9999 9999 99c9 3f29 045a 0e63  ..g.......?).Z.c
-00000390: 616d 6572 6144 6973 7461 6e63 655a 0963  ameraDistanceZ.c
-000003a0: 616d 6572 6159 6177 5a0b 6361 6d65 7261  ameraYawZ.camera
-000003b0: 5069 7463 68da 1463 616d 6572 6154 6172  Pitch..cameraTar
-000003c0: 6765 7450 6f73 6974 696f 6ee9 ffff ffff  getPosition.....
-000003d0: e906 0000 00e9 0100 0000 e905 0000 00e7  ................
-000003e0: ec51 b81e 85eb b13f e902 0000 0029 0472  .Q.....?.....).r
-000003f0: 1000 0000 720b 0000 00e9 0400 0000 7211  ....r.........r.
-00000400: 0000 0067 3333 3333 3333 d33f 677b 14ae  ...g333333.?g{..
-00000410: 47e1 7a84 3fe9 c800 0000 e914 0000 0029  G.z.?..........)
-00000420: 20da 086d 6574 6164 6174 61da 0b72 656e   ..metadata..ren
-00000430: 6465 725f 6d6f 6465 5a0b 5f69 7344 6973  der_modeZ._isDis
-00000440: 6372 6574 655a 095f 7469 6d65 5374 6570  creteZ._timeStep
-00000450: da09 5f75 7264 6652 6f6f 74da 095f 6d61  .._urdfRoot.._ma
-00000460: 7853 7465 7073 da06 5f77 6964 7468 da07  xSteps.._width..
-00000470: 5f68 6569 6768 74da 0170 da07 636f 6e6e  _height..p..conn
-00000480: 6563 74da 0d53 4841 5245 445f 4d45 4d4f  ect..SHARED_MEMO
-00000490: 5259 da03 4755 49da 1a72 6573 6574 4465  RY..GUI..resetDe
-000004a0: 6275 6756 6973 7561 6c69 7a65 7243 616d  bugVisualizerCam
-000004b0: 6572 61da 0644 4952 4543 54da 095f 6361  era..DIRECT.._ca
-000004c0: 6d5f 6469 7374 da08 5f63 616d 5f79 6177  m_dist.._cam_yaw
-000004d0: da0a 5f63 616d 5f70 6974 6368 da0d 5f63  .._cam_pitch.._c
-000004e0: 616d 5f74 6172 6765 745f 7072 0300 0000  am_target_pr....
-000004f0: da03 426f 78da 026e 70da 0561 7272 6179  ..Box..np..array
-00000500: da0c 6163 7469 6f6e 5f73 7061 6365 da08  ..action_space..
-00000510: 626f 756e 6461 7279 da11 6f62 7365 7276  boundary..observ
-00000520: 6174 696f 6e5f 7370 6163 65da 0f73 7465  ation_space..ste
-00000530: 6572 696e 675f 6a6f 696e 7473 da0c 6472  ering_joints..dr
-00000540: 6976 655f 6a6f 696e 7473 da0b 6a6f 696e  ive_joints..join
-00000550: 745f 7370 6565 64da 0963 5f72 6f6c 6c69  t_speed..c_rolli
-00000560: 6e67 da06 635f 6472 6167 da0a 635f 7468  ng..c_drag..c_th
-00000570: 726f 7474 6c65 da09 4d41 585f 5350 4545  rottle..MAX_SPEE
-00000580: 4429 08da 0473 656c 6672 1800 0000 5a08  D)...selfr....Z.
-00000590: 6d61 7853 7465 7073 5a0a 6973 4469 7363  maxStepsZ.isDisc
-000005a0: 7265 7465 5a08 7572 6466 526f 6f74 da05  reteZ.urdfRoot..
-000005b0: 7769 6474 68da 0668 6569 6768 745a 0363  width..heightZ.c
-000005c0: 6964 a900 7237 0000 00fa 4e2f 5573 6572  id..r7....N/User
-000005d0: 732f 7361 6970 6861 6e69 3732 342f 4465  s/saiphani724/De
-000005e0: 736b 746f 702f 4169 2f52 6f62 6f74 6963  sktop/Ai/Robotic
-000005f0: 732f 526f 7665 7241 726d 2f72 6f76 6572  s/RoverArm/rover
-00000600: 5f61 726d 2f65 6e76 732f 726f 7665 7261  _arm/envs/rovera
-00000610: 726d 5f65 6e76 2e70 79da 085f 5f69 6e69  rm_env.py..__ini
-00000620: 745f 5f10 0000 0073 3a00 0000 0002 0e01  t__....s:.......
+000000e0: 0600 0000 4000 0000 735c 0000 0065 005a  ....@...s\...e.Z
+000000f0: 0164 005a 0264 0164 0264 0367 0269 015a  .d.Z.d.d.d.g.i.Z
+00000100: 0364 0364 0464 0565 04a0 05a1 0064 0664  .d.d.d.e.....d.d
+00000110: 0666 0664 0764 0884 015a 0664 0964 0a84  .f.d.d...Z.d.d..
+00000120: 005a 0764 0b64 0c84 005a 0864 1464 0e64  .Z.d.d...Z.d.d.d
+00000130: 0f84 015a 0964 1064 1184 005a 0a64 1264  ...Z.d.d...Z.d.d
+00000140: 1384 005a 0b64 0d53 0029 15da 0b52 6f76  ...Z.d.S.)...Rov
+00000150: 6572 4172 6d45 6e76 7a0c 7265 6e64 6572  erArmEnvz.render
+00000160: 2e6d 6f64 6573 da05 6875 6d61 6eda 0972  .modes..human..r
+00000170: 6762 5f61 7272 6179 6950 c300 0046 e930  gb_arrayiP...F.0
+00000180: 0000 0063 0700 0000 0000 0000 0000 0000  ...c............
+00000190: 0800 0000 0800 0000 4300 0000 7372 0100  ........C...sr..
+000001a0: 007c 017c 005f 007c 037c 005f 0164 017c  .|.|._.|.|._.d.|
+000001b0: 005f 027c 047c 005f 037c 027c 005f 047c  ._.|.|._.|.|._.|
+000001c0: 057c 005f 057c 067c 005f 067c 006a 0064  .|._.|.|._.|.j.d
+000001d0: 026b 0272 6a74 07a0 0874 076a 09a1 017d  .k.rjt...t.j...}
+000001e0: 077c 0764 036b 0072 5474 07a0 0874 076a  .|.d.k.rTt...t.j
+000001f0: 0aa1 017d 0774 07a0 0b64 0464 0564 0667  ...}.t...d.d.d.g
+00000200: 0064 07a2 01a1 0401 006e 0c74 07a0 0874  .d.......n.t...t
+00000210: 076a 0ca1 0101 0064 087c 005f 0d64 097c  .j.....d.|._.d.|
+00000220: 005f 0e64 0a7c 005f 0f67 0064 0ba2 017c  ._.d.|._.g.d...|
+00000230: 005f 1074 076a 0b7c 006a 0d7c 006a 0e7c  ._.t.j.|.j.|.j.|
+00000240: 006a 0f7c 006a 1064 0c8d 0401 0074 11a0  .j.|.j.d.....t..
+00000250: 1274 13a0 1464 0d64 0e67 0264 0d67 0164  .t...d.d.g.d.g.d
+00000260: 0f14 0017 00a1 0174 13a0 1464 1064 1167  .......t...d.d.g
+00000270: 0264 1067 0164 0f14 0017 00a1 01a1 027c  .d.g.d.........|
+00000280: 005f 1564 127c 005f 1674 11a0 1274 13a0  ._.d.|._.t...t..
+00000290: 147c 006a 160b 007c 006a 160b 0067 0264  .|.j...|.j...g.d
+000002a0: 0d67 0164 0814 0017 0064 0364 0367 0217  .g.d.....d.d.g..
+000002b0: 00a1 0174 13a0 147c 006a 167c 006a 1667  ...t...|.j.|.j.g
+000002c0: 0264 1067 0164 0814 0017 0064 1367 0164  .d.g.d.....d.g.d
+000002d0: 1414 0017 00a1 01a1 027c 005f 1764 0364  .........|._.d.d
+000002e0: 1467 027c 005f 1867 0064 15a2 017c 005f  .g.|._.g.d...|._
+000002f0: 1964 037c 005f 1a64 167c 005f 1b64 177c  .d.|._.d.|._.d.|
+00000300: 005f 1c64 187c 005f 1d64 197c 005f 1e64  ._.d.|._.d.|._.d
+00000310: 0053 0029 1a4e 6711 1111 1111 1171 3f72  .S.).Ng......q?r
+00000320: 0700 0000 7201 0000 0067 cdcc cccc cccc  ....r....g......
+00000330: f43f e9b4 0000 0069 d7ff ffff 2903 67a4  .?.....i....).g.
+00000340: 703d 0ad7 a3e0 3fe7 9a99 9999 9999 c9bf  p=....?.........
+00000350: 671f 85eb 51b8 1ed5 bfe9 0300 0000 e766  g...Q..........f
+00000360: 6666 6666 66d6 bf69 ddff ffff 2903 6771  fffff..i....).gq
+00000370: 3d0a d7a3 70e5 3f72 0d00 0000 679a 9999  =...p.?r....g...
+00000380: 9999 99c9 3f29 045a 0e63 616d 6572 6144  ....?).Z.cameraD
+00000390: 6973 7461 6e63 655a 0963 616d 6572 6159  istanceZ.cameraY
+000003a0: 6177 5a0b 6361 6d65 7261 5069 7463 68da  awZ.cameraPitch.
+000003b0: 1463 616d 6572 6154 6172 6765 7450 6f73  .cameraTargetPos
+000003c0: 6974 696f 6ee9 ffff ffff e733 3333 3333  ition......33333
+000003d0: 33e3 bfe9 0400 0000 e901 0000 00e7 3333  3.............33
+000003e0: 3333 3333 e33f e905 0000 00e7 ec51 b81e  3333.?.......Q..
+000003f0: 85eb b13f e902 0000 0029 0472 1200 0000  ...?.....).r....
+00000400: 720c 0000 0072 1100 0000 7214 0000 0067  r....r....r....g
+00000410: 3333 3333 3333 d33f 677b 14ae 47e1 7a84  333333.?g{..G.z.
+00000420: 3fe9 c800 0000 e914 0000 0029 1fda 0b72  ?..........)...r
+00000430: 656e 6465 725f 6d6f 6465 5a0b 5f69 7344  ender_modeZ._isD
+00000440: 6973 6372 6574 655a 095f 7469 6d65 5374  iscreteZ._timeSt
+00000450: 6570 da09 5f75 7264 6652 6f6f 74da 095f  ep.._urdfRoot.._
+00000460: 6d61 7853 7465 7073 da06 5f77 6964 7468  maxSteps.._width
+00000470: da07 5f68 6569 6768 74da 0170 da07 636f  .._height..p..co
+00000480: 6e6e 6563 745a 0d53 4841 5245 445f 4d45  nnectZ.SHARED_ME
+00000490: 4d4f 5259 5a03 4755 495a 1a72 6573 6574  MORYZ.GUIZ.reset
+000004a0: 4465 6275 6756 6973 7561 6c69 7a65 7243  DebugVisualizerC
+000004b0: 616d 6572 615a 0644 4952 4543 54da 095f  ameraZ.DIRECT.._
+000004c0: 6361 6d5f 6469 7374 da08 5f63 616d 5f79  cam_dist.._cam_y
+000004d0: 6177 da0a 5f63 616d 5f70 6974 6368 da0d  aw.._cam_pitch..
+000004e0: 5f63 616d 5f74 6172 6765 745f 7072 0300  _cam_target_pr..
+000004f0: 0000 da03 426f 78da 026e 70da 0561 7272  ....Box..np..arr
+00000500: 6179 da0c 6163 7469 6f6e 5f73 7061 6365  ay..action_space
+00000510: da08 626f 756e 6461 7279 da11 6f62 7365  ..boundary..obse
+00000520: 7276 6174 696f 6e5f 7370 6163 65da 0f73  rvation_space..s
+00000530: 7465 6572 696e 675f 6a6f 696e 7473 da0c  teering_joints..
+00000540: 6472 6976 655f 6a6f 696e 7473 da0b 6a6f  drive_joints..jo
+00000550: 696e 745f 7370 6565 64da 0963 5f72 6f6c  int_speed..c_rol
+00000560: 6c69 6e67 da06 635f 6472 6167 da0a 635f  ling..c_drag..c_
+00000570: 7468 726f 7474 6c65 da09 4d41 585f 5350  throttle..MAX_SP
+00000580: 4545 4429 08da 0473 656c 6672 1900 0000  EED)...selfr....
+00000590: 5a08 6d61 7853 7465 7073 5a0a 6973 4469  Z.maxStepsZ.isDi
+000005a0: 7363 7265 7465 5a08 7572 6466 526f 6f74  screteZ.urdfRoot
+000005b0: da05 7769 6474 68da 0668 6569 6768 745a  ..width..heightZ
+000005c0: 0363 6964 a900 7234 0000 00fa 4e2f 5573  .cid..r4....N/Us
+000005d0: 6572 732f 7361 6970 6861 6e69 3732 342f  ers/saiphani724/
+000005e0: 4465 736b 746f 702f 4169 2f52 6f62 6f74  Desktop/Ai/Robot
+000005f0: 6963 732f 526f 7665 7241 726d 2f72 6f76  ics/RoverArm/rov
+00000600: 6572 5f61 726d 2f65 6e76 732f 726f 7665  er_arm/envs/rove
+00000610: 7261 726d 5f65 6e76 2e70 79da 085f 5f69  rarm_env.py..__i
+00000620: 6e69 745f 5f11 0000 0073 3800 0000 0002  nit__....s8.....
 00000630: 0601 0601 0601 0601 0601 0601 0601 0a01  ................
 00000640: 0c01 0801 0c01 1602 0c01 0601 0601 0601  ................
-00000650: 0a02 1a01 2601 0601 6603 0a01 0a02 0602  ....&...f.......
+00000650: 0a02 1a01 3601 0601 5403 0a01 0a02 0602  ....6...T.......
 00000660: 0601 0602 0602 7a14 526f 7665 7241 726d  ......z.RoverArm
-00000670: 456e 762e 5f5f 696e 6974 5f5f e92a 0000  Env.__init__.*..
-00000680: 0063 0200 0000 0000 0000 0000 0000 1000  .c..............
-00000690: 0000 0800 0000 4300 0000 7326 0200 0074  ......C...s&...t
-000006a0: 00a0 017c 01a1 0101 0074 026a 00a0 017c  ...|.....t.j...|
-000006b0: 01a1 0101 0064 017c 005f 0374 04a0 05a1  .....d.|._.t....
-000006c0: 0001 0074 04a0 0674 046a 0764 01a1 0201  ...t...t.j.d....
-000006d0: 0074 04a0 0864 0164 0164 02a1 0301 0074  .t...d.d.d.....t
-000006e0: 046a 0974 0a6a 0ba0 0c7c 006a 0d64 03a1  .j.t.j...|.j.d..
-000006f0: 0267 0064 04a2 0164 058d 027d 0267 0064  .g.d...d...}.g.d
-00000700: 06a2 017d 0374 026a 00a0 0e74 00a0 0f64  ...}.t.j...t...d
-00000710: 0764 08a1 0274 00a0 0f64 0964 0aa1 0267  .d...t...d.d...g
-00000720: 02a1 017d 0474 00a0 0f64 0764 0ba1 027d  ...}.t...d.d...}
-00000730: 0574 10a0 11a1 0064 0119 0064 0c17 007d  .t.....d...d...}
-00000740: 0674 046a 097c 0664 0d17 007c 047c 0564  .t.j.|.d...|.|.d
-00000750: 0e67 0364 058d 027c 005f 1274 1364 0f64  .g.d...|._.t.d.d
-00000760: 1083 0244 005d 1c7d 0774 04a0 147c 006a  ...D.].}.t...|.j
-00000770: 127c 077c 037c 0764 0f18 0019 00a1 0301  .|.|.|.d........
-00000780: 0071 c674 04a0 147c 006a 1264 1164 12a1  .q.t...|.j.d.d..
-00000790: 0301 0074 04a0 147c 006a 1264 1364 12a1  ...t...|.j.d.d..
-000007a0: 0301 0074 046a 0974 0a6a 0ba0 0c7c 006a  ...t.j.t.j...|.j
-000007b0: 0d64 14a1 0267 0064 15a2 0164 1664 178d  .d...g.d...d.d..
-000007c0: 037d 0874 046a 0974 0a6a 0ba0 0c7c 006a  .}.t.j.t.j...|.j
-000007d0: 0d64 18a1 0267 0064 19a2 0164 1664 178d  .d...g.d...d.d..
-000007e0: 037d 0974 00a0 0f64 1a64 16a1 0274 00a0  .}.t...d.d...t..
-000007f0: 0f64 1b64 1ca1 0264 1d67 037d 0a74 046a  .d.d...d.g.}.t.j
-00000800: 0974 0a6a 0ba0 0c7c 006a 0d64 1ea1 027c  .t.j...|.j.d...|
-00000810: 0a64 1f64 178d 037c 005f 1574 04a0 167c  .d.d...|._.t...|
-00000820: 006a 1264 01a1 0264 0119 0064 0064 0a85  .j.d...d...d.d..
-00000830: 0219 007d 0b74 04a0 167c 006a 1264 20a1  ...}.t...|.j.d .
-00000840: 0264 0119 007d 0c74 04a0 177c 006a 1264  .d...}.t...|.j.d
-00000850: 11a1 0264 0119 0074 04a0 177c 006a 1264  ...d...t...|.j.d
-00000860: 13a1 0264 0119 0066 027d 0d74 04a0 187c  ...d...f.}.t...|
-00000870: 006a 15a1 015c 027d 0a7d 0e7c 0b7c 0c17  .j...\.}.}.|.|..
-00000880: 007c 0d17 0074 197c 0a83 0117 007c 005f  .|...t.|.....|._
-00000890: 1a74 04a0 0674 046a 0764 21a1 0201 007c  .t...t.j.d!....|
-000008a0: 0b7c 0c7c 0d7c 0a64 229c 047d 0f74 02a0  .|.|.|.d"..}.t..
-000008b0: 1b7c 006a 1aa1 01a0 1c74 026a 1da1 017c  .|.j.....t.j...|
-000008c0: 0f66 0253 0029 234e 7201 0000 0069 f6ff  .f.S.)#Nr....i..
-000008d0: ffff 7a0a 706c 616e 652e 7572 6466 2903  ..z.plane.urdf).
-000008e0: 7201 0000 0072 0100 0000 e7cd cccc cccc  r....r..........
-000008f0: cce4 bf29 01da 0c62 6173 6550 6f73 6974  ...)...basePosit
-00000900: 696f 6e29 0972 0100 0000 6785 eb51 b81e  ion).r....g..Q..
-00000910: 85cb bf72 0100 0000 678f c2f5 285c 8f04  ...r....g...(\..
-00000920: c072 0100 0000 e70c 022b 8716 d902 4072  .r.......+....@r
-00000930: 3d00 0000 e77b 14ae 47e1 7ab4 3f72 3e00  =....{..G.z.?r>.
-00000940: 0000 720e 0000 0067 3333 3333 3333 d3bf  ..r....g333333..
-00000950: 6700 0000 0000 00f4 3f72 1300 0000 6700  g.......?r....g.
-00000960: 0000 0000 0004 407a 102f 726f 7665 725f  ......@z./rover_
-00000970: 6172 6d2f 6461 7461 2f7a 0d72 6f76 6572  arm/data/z.rover
-00000980: 5f61 726d 2e78 6d6c 6700 0000 0000 00e0  _arm.xmlg.......
-00000990: bfe9 0700 0000 e90e 0000 00e9 1000 0000  ................
-000009a0: 7212 0000 00e9 1100 0000 7a10 7461 626c  r.........z.tabl
-000009b0: 652f 7461 626c 652e 7572 6466 2903 e700  e/table.urdf)...
-000009c0: 0000 0000 00e0 3f72 0100 0000 723b 0000  ......?r....r;..
-000009d0: 0072 4300 0000 2902 723c 0000 005a 0d67  .rC...).r<...Z.g
-000009e0: 6c6f 6261 6c53 6361 6c69 6e67 7a11 7472  lobalScalingz.tr
-000009f0: 6179 2f74 7261 7962 6f78 2e75 7264 6629  ay/traybox.urdf)
-00000a00: 0367 cdcc cccc cccc dc3f 7201 0000 0067  .g.......?r....g
-00000a10: 713d 0ad7 a370 d5bf 679a 9999 9999 99d9  q=...p..g.......
-00000a20: 3f67 9a99 9999 9999 a9bf e79a 9999 9999  ?g..............
-00000a30: 99a9 3f72 0a00 0000 7a19 7261 6e64 6f6d  ..?r....z.random
-00000a40: 5f75 7264 6673 2f30 3030 2f30 3030 2e75  _urdfs/000/000.u
-00000a50: 7264 6667 9a99 9999 9999 e93f e912 0000  rdfg.......?....
-00000a60: 0072 1000 0000 a904 da0b 7374 6174 655f  .r........state_
-00000a70: 726f 7665 72da 0973 7461 7465 5f61 726d  rover..state_arm
-00000a80: da0d 7374 6174 655f 6669 6e67 6572 73da  ..state_fingers.
-00000a90: 0c73 7461 7465 5f6f 626a 6563 7429 1eda  .state_object)..
-00000aa0: 0672 616e 646f 6dda 0473 6565 6472 2800  .random..seedr(.
-00000ab0: 0000 da0c 7374 6570 5f63 6f75 6e74 6572  ....step_counter
-00000ac0: 721d 0000 00da 0f72 6573 6574 5369 6d75  r......resetSimu
-00000ad0: 6c61 7469 6f6e da18 636f 6e66 6967 7572  lation..configur
-00000ae0: 6544 6562 7567 5669 7375 616c 697a 6572  eDebugVisualizer
-00000af0: da14 434f 565f 454e 4142 4c45 5f52 454e  ..COV_ENABLE_REN
-00000b00: 4445 5249 4e47 da0a 7365 7447 7261 7669  DERING..setGravi
-00000b10: 7479 da08 6c6f 6164 5552 4446 da02 6f73  ty..loadURDF..os
-00000b20: da04 7061 7468 da04 6a6f 696e 7219 0000  ..path..joinr...
-00000b30: 00da 0663 686f 6963 65da 0775 6e69 666f  ...choice..unifo
-00000b40: 726d da04 7369 7465 da0f 6765 7473 6974  rm..site..getsit
-00000b50: 6570 6163 6b61 6765 73da 0b72 6f76 6572  epackages..rover
-00000b60: 6172 6d55 6964 da05 7261 6e67 65da 0f72  armUid..range..r
-00000b70: 6573 6574 4a6f 696e 7453 7461 7465 da09  esetJointState..
-00000b80: 6f62 6a65 6374 5569 64da 0c67 6574 4c69  objectUid..getLi
-00000b90: 6e6b 5374 6174 65da 0d67 6574 4a6f 696e  nkState..getJoin
-00000ba0: 7453 7461 7465 da1d 6765 7442 6173 6550  tState..getBaseP
-00000bb0: 6f73 6974 696f 6e41 6e64 4f72 6965 6e74  ositionAndOrient
-00000bc0: 6174 696f 6eda 0574 7570 6c65 da0b 6f62  ation..tuple..ob
-00000bd0: 7365 7276 6174 696f 6e72 2900 0000 da06  servationr).....
-00000be0: 6173 7479 7065 da07 666c 6f61 7433 3229  astype..float32)
-00000bf0: 1072 3400 0000 724c 0000 005a 0870 6c61  .r4...rL...Z.pla
-00000c00: 6e65 5569 645a 0a72 6573 745f 706f 7365  neUidZ.rest_pose
-00000c10: 735a 0578 5f70 6f73 5a05 795f 706f 73da  sZ.x_posZ.y_pos.
-00000c20: 0842 4153 455f 4449 52da 0169 5a08 7461  .BASE_DIR..iZ.ta
-00000c30: 626c 6555 6964 5a07 7472 6179 5569 6472  bleUidZ.trayUidr
-00000c40: 4a00 0000 7247 0000 0072 4800 0000 7249  J...rG...rH...rI
-00000c50: 0000 00da 015f da04 696e 666f 7237 0000  ....._..infor7..
-00000c60: 0072 3700 0000 7238 0000 00da 0572 6573  .r7...r8.....res
-00000c70: 6574 3800 0000 7338 0000 0000 010a 010c  et8...s8........
-00000c80: 0206 0108 010e 020e 021e 0208 0220 010c  ............. ..
-00000c90: 0210 021a 030e 011a 0110 0110 0220 0120  ............. . 
-00000ca0: 021a 011e 021a 0112 0124 0110 0216 020e  .........$......
-00000cb0: 010e 017a 1152 6f76 6572 4172 6d45 6e76  ...z.RoverArmEnv
-00000cc0: 2e72 6573 6574 6302 0000 0000 0000 0000  .resetc.........
-00000cd0: 0000 0022 0000 0008 0000 0003 0000 0073  ..."...........s
-00000ce0: 5203 0000 7400 a001 6401 7402 6a03 0b00  R...t...d.t.j...
-00000cf0: 7402 6a03 6402 1b00 6703 a101 7d02 6403  t.j.d...g...}.d.
-00000d00: 8900 8700 6601 6404 6405 8408 7c01 6406  ....f.d.d...|.d.
-00000d10: 6407 8502 1900 4400 8301 5c03 7d03 7d04  d.....D...\.}.}.
-00000d20: 7d05 7c01 6407 1900 7d06 7404 a005 7c06  }.|.d...}.t...|.
-00000d30: 6408 6409 6702 640a 640b 6702 a103 7d06  d.d.g.d.d.g...}.
-00000d40: 7400 a006 8801 6a07 640c a102 7d07 7c07  t.....j.d...}.|.
-00000d50: 640a 1900 7d08 7c08 640a 1900 7c03 1700  d...}.|.d...|...
-00000d60: 7c08 6409 1900 7c04 1700 7c08 6406 1900  |.d...|...|.d...
-00000d70: 7c05 1700 6703 7d09 7400 a008 8801 6a07  |...g.}.t.....j.
-00000d80: 640c 7c09 7c02 a104 7d0a 7c0a 6400 640d  d.|.|...}.|.d.d.
-00000d90: 8502 1900 7c0a 640d 640e 8502 1900 0200  ....|.d.d.......
-00000da0: 7d0b 7d0c 7400 a009 8801 6a07 740a 740b  }.}.t.....j.t.t.
-00000db0: 640f 6410 8302 8301 6411 6412 6702 1700  d.d.....d.d.g...
-00000dc0: 7400 6a0c 740a 7c0c 8301 6406 7c06 6701  t.j.t.|...d.|.g.
-00000dd0: 1400 1700 a104 0100 7c01 6400 6406 8502  ........|.d.d...
-00000de0: 1900 5c02 7d0d 7d0e 740d 740e 7c0d 6408  ..\.}.}.t.t.|.d.
-00000df0: 8302 6409 8302 7d0d 7404 a005 7c0e 6408  ..d...}.t...|.d.
-00000e00: 6409 6702 6413 6414 6702 a103 7d0e 7400  d.g.d.d.g...}.t.
-00000e10: 6a09 8801 6a07 8801 6a0f 7400 6a0c 7c0e  j...j...j.t.j.|.
-00000e20: 6701 6406 1400 6415 8d04 0100 8801 6a10  g.d...d.......j.
-00000e30: 0b00 8801 6a10 8801 6a11 1400 8801 6a12  ....j...j.....j.
-00000e40: 1700 1400 7d0f 8801 6a13 7c0d 1400 7c0f  ....}...j.|...|.
-00000e50: 1700 7d10 8801 6a10 6416 7c10 1400 1700  ..}...j.d.|.....
-00000e60: 8801 5f10 740d 740e 8801 6a10 8801 6a14  .._.t.t...j...j.
-00000e70: 0b00 8302 8801 6a14 8302 8801 5f10 7400  ......j....._.t.
-00000e80: 6a09 8801 6a07 8801 6a15 7400 6a16 8801  j...j...j.t.j...
-00000e90: 6a10 6701 6417 1400 6418 6701 6417 1400  j.g.d...d.g.d...
-00000ea0: 6419 8d05 0100 7400 a017 8801 6a18 a101  d.....t.....j...
-00000eb0: 5c02 7d11 7d12 7400 a019 a100 0100 7400  \.}.}.t.......t.
-00000ec0: a017 8801 6a18 a101 5c02 7d13 7d12 7400  ....j...\.}.}.t.
-00000ed0: a006 8801 6a07 640a a102 640a 1900 6400  ....j.d...d...d.
-00000ee0: 6406 8502 1900 7d14 7400 a006 8801 6a07  d.....}.t.....j.
-00000ef0: 640c a102 640a 1900 7d15 7400 a01a 8801  d...d...}.t.....
-00000f00: 6a07 6411 a102 640a 1900 7400 a01a 8801  j.d...d...t.....
-00000f10: 6a07 6412 a102 640a 1900 6602 7d16 641a  j.d...d...f.}.d.
-00000f20: 5c02 7d17 7d18 7c13 6406 1900 640a 6b04  \.}.}.|.d...d.k.
-00000f30: 9002 725a 6409 7d19 641b 7d17 6e74 7404  ..rZd.}.d.}.ntt.
-00000f40: a01b 7404 a01c 7c08 a101 7404 a01c 7c11  ..t...|...t...|.
-00000f50: a101 1800 a101 5c03 7d1a 7d1b 7d1c 7404  ......\.}.}.}.t.
-00000f60: a01b 7404 a01c 7c15 a101 7404 a01c 7c13  ..t...|...t...|.
-00000f70: a101 1800 a101 5c03 7d1d 7d1e 7d1f 7c1a  ......\.}.}.}.|.
-00000f80: 7c1d 1800 7c1b 1700 7c1e 1800 7c1c 1700  |...|...|...|...
-00000f90: 7c1f 1800 7d19 741b 7c19 8301 641c 6b04  |...}.t.|...d.k.
-00000fa0: 9002 72ca 7c19 6418 1b00 7d19 6e04 640a  ..r.|.d...}.n.d.
-00000fb0: 7d19 8801 0400 6a1d 6409 3700 0200 5f1d  }.....j.d.7..._.
-00000fc0: 8701 6601 641d 641e 8408 7d20 7c20 7c14  ..f.d.d...} | |.
-00000fd0: 8301 9002 73fa 6408 7d19 641b 7d17 8801  ....s.d.}.d.}...
-00000fe0: 6a1d 8801 6a1e 6b04 9003 7210 640a 7d19  j...j.k...r.d.}.
-00000ff0: 641b 7d18 7c14 7c15 1700 7c16 1700 741f  d.}.|.|...|...t.
-00001000: 7c13 8301 1700 8801 5f20 7c14 7c15 7c16  |......._ |.|.|.
-00001010: 7c13 641f 9c04 7d21 7404 a01c 8801 6a20  |.d...}!t.....j 
-00001020: a101 a021 7404 6a22 a101 7c19 7c17 7c18  ...!t.j"..|.|.|.
-00001030: 7c21 6605 5300 2920 4e67 0000 0000 0000  |!f.S.) Ng......
-00001040: 0000 6700 0000 0000 0000 4072 4400 0000  ..g.......@rD...
-00001050: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001060: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
-00001070: 7c00 5d0c 7d01 7c01 8800 1400 9102 7104  |.].}.|.......q.
-00001080: 5300 7237 0000 0072 3700 0000 2902 da02  S.r7...r7...)...
-00001090: 2e30 da01 7829 01da 0264 7672 3700 0000  .0..x)...dvr7...
-000010a0: 7238 0000 00da 0a3c 6c69 7374 636f 6d70  r8.....<listcomp
-000010b0: 3e68 0000 00f3 0000 0000 7a24 526f 7665  >h........z$Rove
-000010c0: 7241 726d 456e 762e 7374 6570 2e3c 6c6f  rArmEnv.step.<lo
-000010d0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000010e0: 7213 0000 0072 1100 0000 720e 0000 0072  r....r....r....r
-000010f0: 1000 0000 7201 0000 0072 1200 0000 7245  ....r....r....rE
-00001100: 0000 0072 0f00 0000 e90d 0000 0072 3f00  ...r.........r?.
-00001110: 0000 7240 0000 0072 4100 0000 7242 0000  ..r@...rA...rB..
-00001120: 0067 3333 3333 3333 e3bf 6733 3333 3333  .g333333..g33333
-00001130: 33e3 3f29 02da 0b63 6f6e 7472 6f6c 4d6f  3.?)...controlMo
-00001140: 6465 5a0f 7461 7267 6574 506f 7369 7469  deZ.targetPositi
-00001150: 6f6e 7367 1111 1111 1111 a13f 7214 0000  onsg.......?r...
-00001160: 00e9 0a00 0000 2905 5a0c 626f 6479 556e  ......).Z.bodyUn
-00001170: 6971 7565 4964 5a0c 6a6f 696e 7449 6e64  iqueIdZ.jointInd
-00001180: 6963 6573 7270 0000 005a 1074 6172 6765  icesrp...Z.targe
-00001190: 7456 656c 6f63 6974 6965 735a 0666 6f72  tVelocitiesZ.for
-000011a0: 6365 7329 0246 4654 67fc a9f1 d24d 6250  ces).FFTg....MbP
-000011b0: 3f63 0100 0000 0000 0000 0000 0000 0400  ?c..............
-000011c0: 0000 0200 0000 1300 0000 733c 0000 007c  ..........s<...|
-000011d0: 005c 027d 017d 027c 0188 006a 000b 006b  .\.}.}.|...j...k
-000011e0: 046f 1c7c 0188 006a 006b 007d 037c 036f  .o.|...j.k.}.|.o
-000011f0: 367c 0288 006a 000b 006b 046f 367c 0288  6|...j...k.o6|..
-00001200: 006a 006b 007d 037c 0353 00a9 014e 2901  .j.k.}.|.S...N).
-00001210: 722b 0000 0029 0472 4700 0000 da02 7278  r+...).rG.....rx
-00001220: 5a02 7279 5a07 696e 426f 756e 64a9 0172  Z.ryZ.inBound..r
-00001230: 3400 0000 7237 0000 0072 3800 0000 da06  4...r7...r8.....
-00001240: 696e 4761 6d65 b000 0000 7308 0000 0000  inGame....s.....
-00001250: 0108 0116 011a 017a 2052 6f76 6572 4172  .......z RoverAr
-00001260: 6d45 6e76 2e73 7465 702e 3c6c 6f63 616c  mEnv.step.<local
-00001270: 733e 2e69 6e47 616d 6572 4600 0000 2923  s>.inGamerF...)#
-00001280: 721d 0000 00da 1667 6574 5175 6174 6572  r......getQuater
-00001290: 6e69 6f6e 4672 6f6d 4575 6c65 72da 046d  nionFromEuler..m
-000012a0: 6174 68da 0270 6972 2800 0000 da06 696e  ath..pir(.....in
-000012b0: 7465 7270 725e 0000 0072 5a00 0000 da1a  terpr^...rZ.....
-000012c0: 6361 6c63 756c 6174 6549 6e76 6572 7365  calculateInverse
-000012d0: 4b69 6e65 6d61 7469 6373 da19 7365 744a  Kinematics..setJ
-000012e0: 6f69 6e74 4d6f 746f 7243 6f6e 7472 6f6c  ointMotorControl
-000012f0: 4172 7261 79da 046c 6973 7472 5b00 0000  Array..listr[...
-00001300: da10 504f 5349 5449 4f4e 5f43 4f4e 5452  ..POSITION_CONTR
-00001310: 4f4c da03 6d69 6eda 036d 6178 722d 0000  OL..min..maxr-..
-00001320: 0072 2f00 0000 7231 0000 0072 3000 0000  .r/...r1...r0...
-00001330: 7232 0000 0072 3300 0000 722e 0000 00da  r2...r3...r.....
-00001340: 1056 454c 4f43 4954 595f 434f 4e54 524f  .VELOCITY_CONTRO
-00001350: 4c72 6000 0000 725d 0000 00da 0e73 7465  Lr`...r].....ste
-00001360: 7053 696d 756c 6174 696f 6e72 5f00 0000  pSimulationr_...
-00001370: da03 6162 7372 2900 0000 724d 0000 0072  ..absr)...rM...r
-00001380: 1a00 0000 7261 0000 0072 6200 0000 7263  ....ra...rb...rc
-00001390: 0000 0072 6400 0000 2922 7234 0000 00da  ...rd...)"r4....
-000013a0: 0661 6374 696f 6e5a 0b6f 7269 656e 7461  .actionZ.orienta
-000013b0: 7469 6f6e 5a04 6478 5f61 5a04 6479 5f61  tionZ.dx_aZ.dy_a
-000013c0: 5a04 647a 5f61 5a07 6669 6e67 6572 735a  Z.dz_aZ.fingersZ
-000013d0: 0b63 7572 7265 6e74 506f 7365 5a0f 6375  .currentPoseZ.cu
-000013e0: 7272 656e 7450 6f73 6974 696f 6e5a 0b6e  rrentPositionZ.n
-000013f0: 6577 506f 7369 7469 6f6e 5a0a 6a6f 696e  ewPositionZ.join
-00001400: 7450 6f73 6573 5a10 6a6f 696e 7450 6f73  tPosesZ.jointPos
-00001410: 6573 5f72 6f76 6572 5a0e 6a6f 696e 7450  es_roverZ.jointP
-00001420: 6f73 6573 5f61 726d 5a08 7468 726f 7474  oses_armZ.thrott
-00001430: 6c65 5a0e 7374 6565 7269 6e67 5f61 6e67  leZ.steering_ang
-00001440: 6c65 5a08 6672 6963 7469 6f6e 5a0c 6163  leZ.frictionZ.ac
-00001450: 6365 6c65 7261 7469 6f6e 5a11 7374 6174  celerationZ.stat
-00001460: 655f 6f62 6a65 6374 5f70 7265 7672 6700  e_object_prevrg.
-00001470: 0000 724a 0000 0072 4700 0000 7248 0000  ..rJ...rG...rH..
-00001480: 0072 4900 0000 da0a 7465 726d 696e 6174  .rI.....terminat
-00001490: 6564 da09 7472 756e 6361 7465 64da 0672  ed..truncated..r
-000014a0: 6577 6172 64da 0278 305a 0279 305a 027a  eward..x0Z.y0Z.z
-000014b0: 30da 0278 31da 0279 31da 027a 3172 7500  0..x1..y1..z1ru.
-000014c0: 0000 7268 0000 0072 3700 0000 2902 726c  ..rh...r7...).rl
-000014d0: 0000 0072 3400 0000 7238 0000 00da 0473  ...r4...r8.....s
-000014e0: 7465 7064 0000 0073 7a00 0000 0002 1a01  tepd...sz.......
-000014f0: 0401 2001 0801 1602 0e02 0802 0a01 0a01  .. .............
-00001500: 0afe 0403 1201 1a01 3402 1004 1001 1604  ........4.......
-00001510: 0c01 0401 08fe 0606 1001 04ff 0603 0e03  ................
-00001520: 1002 1a04 0401 0401 0401 0401 0a01 08fb  ................
-00001530: 0607 1002 0802 1001 1a01 1201 2402 0801  ............$...
-00001540: 0e01 0401 0602 2001 2001 1801 0e01 0a02  ...... . .......
-00001550: 0402 0e01 0c06 0a01 0401 0402 0e01 0401  ................
-00001560: 0402 1601 0e02 7a10 526f 7665 7241 726d  ......z.RoverArm
-00001570: 456e 762e 7374 6570 4e63 0300 0000 0000  Env.stepNc......
-00001580: 0000 0000 0000 0c00 0000 0800 0000 4300  ..............C.
-00001590: 0000 7342 0100 007c 0164 006b 0273 107c  ..sB...|.d.k.s.|
-000015a0: 0264 006b 0272 1c7c 006a 007d 017c 006a  .d.k.r.|.j.}.|.j
-000015b0: 017d 027c 006a 0264 016b 0372 2a64 0053  .}.|.j.d.k.r*d.S
-000015c0: 0074 036a 047c 006a 057c 006a 067c 006a  .t.j.|.j.|.j.|.j
-000015d0: 077c 006a 0864 0264 0364 048d 067d 0374  .|.j.d.d.d...}.t
-000015e0: 036a 0467 0064 05a2 0164 0664 0764 0864  .j.g.d...d.d.d.d
-000015f0: 0264 0364 048d 067d 0474 036a 0964 0974  .d.d...}.t.j.d.t
-00001600: 0a7c 0183 017c 021b 0064 0a64 0b64 0c8d  .|...|...d.d.d..
-00001610: 047d 0574 036a 0b7c 017c 027c 037c 0574  .}.t.j.|.|.|.|.t
-00001620: 036a 0c64 0d8d 055c 057d 067d 067d 077d  .j.d...\.}.}.}.}
-00001630: 067d 0674 036a 0b7c 017c 027c 047c 0574  .}.t.j.|.|.|.|.t
-00001640: 036a 0c64 0d8d 055c 057d 067d 067d 087d  .j.d...\.}.}.}.}
-00001650: 067d 0674 0d6a 0e7c 0774 0d6a 0f64 0e8d  .}.t.j.|.t.j.d..
-00001660: 027d 0974 0da0 107c 097c 027c 0164 0f66  .}.t...|.|.|.d.f
-00001670: 03a1 0264 0064 0085 0264 0064 0085 0264  ...d.d...d.d...d
-00001680: 0064 1085 0266 0319 007d 0974 0d6a 0e7c  .d...f...}.t.j.|
-00001690: 0874 0d6a 0f64 0e8d 027d 0a74 0da0 107c  .t.j.d...}.t...|
-000016a0: 0a7c 027c 0164 0f66 03a1 0264 0064 0085  .|.|.d.f...d.d..
-000016b0: 0264 0064 0085 0264 0064 1085 0266 0319  .d.d...d.d...f..
-000016c0: 007d 0a74 0d6a 117c 097c 0a66 0264 0364  .}.t.j.|.|.f.d.d
-000016d0: 118d 027d 0b7c 0b53 0029 124e 7207 0000  ...}.|.S.).Nr...
-000016e0: 0072 0100 0000 7213 0000 0029 0672 0d00  .r....r....).r..
-000016f0: 0000 da08 6469 7374 616e 6365 5a03 7961  ....distanceZ.ya
-00001700: 775a 0570 6974 6368 da04 726f 6c6c 5a0b  wZ.pitch..rollZ.
-00001710: 7570 4178 6973 496e 6465 7829 03e7 6666  upAxisIndex)..ff
-00001720: 6666 6666 e63f 7201 0000 0072 4400 0000  ffff.?r....rD...
-00001730: 728e 0000 00e9 5a00 0000 69ba ffff ffe9  r.....Z...i.....
-00001740: 3c00 0000 679a 9999 9999 99b9 3f67 0000  <...g.......?g..
-00001750: 0000 0000 5940 2904 5a03 666f 76da 0661  ....Y@).Z.fov..a
-00001760: 7370 6563 745a 076e 6561 7256 616c 5a06  spectZ.nearValZ.
-00001770: 6661 7256 616c 2905 7235 0000 0072 3600  farVal).r5...r6.
-00001780: 0000 5a0a 7669 6577 4d61 7472 6978 5a10  ..Z.viewMatrixZ.
-00001790: 7072 6f6a 6563 7469 6f6e 4d61 7472 6978  projectionMatrix
-000017a0: 5a08 7265 6e64 6572 6572 2901 da05 6474  Z.renderer)...dt
-000017b0: 7970 6572 1400 0000 720b 0000 0029 01da  yper....r....)..
-000017c0: 0461 7869 7329 1272 1b00 0000 721c 0000  .axis).r....r...
-000017d0: 0072 1800 0000 721d 0000 00da 2163 6f6d  .r....r.....!com
-000017e0: 7075 7465 5669 6577 4d61 7472 6978 4672  puteViewMatrixFr
-000017f0: 6f6d 5961 7750 6974 6368 526f 6c6c 7226  omYawPitchRollr&
-00001800: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00001810: 0000 da1a 636f 6d70 7574 6550 726f 6a65  ....computeProje
-00001820: 6374 696f 6e4d 6174 7269 7846 4f56 da05  ctionMatrixFOV..
-00001830: 666c 6f61 74da 0e67 6574 4361 6d65 7261  float..getCamera
-00001840: 496d 6167 65da 1945 525f 4255 4c4c 4554  Image..ER_BULLET
-00001850: 5f48 4152 4457 4152 455f 4f50 454e 474c  _HARDWARE_OPENGL
-00001860: 7228 0000 0072 2900 0000 da05 7569 6e74  r(...r).....uint
-00001870: 38da 0772 6573 6861 7065 da0b 636f 6e63  8..reshape..conc
-00001880: 6174 656e 6174 6529 0c72 3400 0000 7235  atenate).r4...r5
-00001890: 0000 0072 3600 0000 5a0c 7669 6577 5f6d  ...r6...Z.view_m
-000018a0: 6174 7269 7831 5a0c 7669 6577 5f6d 6174  atrix1Z.view_mat
-000018b0: 7269 7832 5a0b 7072 6f6a 5f6d 6174 7269  rix2Z.proj_matri
-000018c0: 7872 6700 0000 5a03 7078 315a 0370 7832  xrg...Z.px1Z.px2
-000018d0: 5a0a 7267 625f 6172 7261 7931 5a0a 7267  Z.rgb_array1Z.rg
-000018e0: 625f 6172 7261 7932 7207 0000 0072 3700  b_array2r....r7.
-000018f0: 0000 7237 0000 0072 3800 0000 da06 7265  ..r7...r8.....re
-00001900: 6e64 6572 c400 0000 7354 0000 0000 0710  nder....sT......
-00001910: 0106 0106 010a 0104 0108 0104 0104 0104  ................
-00001920: 0102 0102 fb06 060a 0102 0102 0102 0102  ................
-00001930: 0102 fb06 0606 010a 0102 0102 fd06 0506  ................
-00001940: 0102 0102 0102 0104 fc10 0606 0102 0102  ................
-00001950: 0102 0104 fc10 0610 0128 0210 0128 0312  .........(...(..
-00001960: 027a 1252 6f76 6572 4172 6d45 6e76 2e72  .z.RoverArmEnv.r
-00001970: 656e 6465 7263 0100 0000 0000 0000 0000  enderc..........
-00001980: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00001990: 0000 007c 006a 0053 0072 7200 0000 2901  ...|.j.S.rr...).
-000019a0: 7262 0000 0072 7400 0000 7237 0000 0072  rb...rt...r7...r
-000019b0: 3700 0000 7238 0000 00da 0a5f 6765 745f  7...r8....._get_
-000019c0: 7374 6174 65f8 0000 0073 0200 0000 0001  state....s......
-000019d0: 7a16 526f 7665 7241 726d 456e 762e 5f67  z.RoverArmEnv._g
-000019e0: 6574 5f73 7461 7465 6301 0000 0000 0000  et_statec.......
-000019f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001a00: 0073 0c00 0000 7400 a001 a100 0100 6400  .s....t.......d.
-00001a10: 5300 7272 0000 0029 0272 1d00 0000 da0a  S.rr...).r......
-00001a20: 6469 7363 6f6e 6e65 6374 7274 0000 0072  disconnectrt...r
-00001a30: 3700 0000 7237 0000 0072 3800 0000 da05  7...r7...r8.....
-00001a40: 636c 6f73 65fb 0000 0073 0200 0000 0001  close....s......
-00001a50: 7a11 526f 7665 7241 726d 456e 762e 636c  z.RoverArmEnv.cl
-00001a60: 6f73 6529 0172 3a00 0000 2902 4e4e 290b  ose).r:...).NN).
-00001a70: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001a80: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001a90: 6d65 5f5f da0d 7079 6275 6c6c 6574 5f64  me__..pybullet_d
-00001aa0: 6174 615a 0b67 6574 4461 7461 5061 7468  ataZ.getDataPath
-00001ab0: 7239 0000 0072 6900 0000 728b 0000 0072  r9...ri...r....r
-00001ac0: 9c00 0000 729d 0000 0072 9f00 0000 7237  ....r....r....r7
-00001ad0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-00001ae0: 0000 7206 0000 000e 0000 0073 1000 0000  ..r........s....
-00001af0: 0802 0c01 04ff 0a28 0a2c 0860 0a34 0803  .......(.,.`.4..
-00001b00: 7206 0000 0029 12da 0967 796d 6e61 7369  r....)...gymnasi
-00001b10: 756d da03 6779 6d72 0200 0000 7203 0000  um..gymr....r...
-00001b20: 0072 0400 0000 da0f 6779 6d6e 6173 6975  .r......gymnasiu
-00001b30: 6d2e 7574 696c 7372 0500 0000 7253 0000  m.utilsr....rS..
-00001b40: 00da 0870 7962 756c 6c65 7472 1d00 0000  ...pybulletr....
-00001b50: 72a3 0000 0072 7700 0000 da05 6e75 6d70  r....rw.....nump
-00001b60: 7972 2800 0000 724b 0000 0072 5800 0000  yr(...rK...rX...
-00001b70: da03 456e 7672 0600 0000 7237 0000 0072  ..Envr....r7...r
-00001b80: 3700 0000 7237 0000 0072 3800 0000 da08  7...r7...r8.....
-00001b90: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-00001ba0: 0008 0114 010c 0208 0108 0108 0108 0108  ................
-00001bb0: 0108 0108 03                             .....
+00000670: 456e 762e 5f5f 696e 6974 5f5f 6301 0000  Env.__init__c...
+00000680: 0000 0000 0000 0000 000d 0000 0008 0000  ................
+00000690: 0043 0000 0073 e601 0000 6401 7c00 5f00  .C...s....d.|._.
+000006a0: 7401 a002 a100 0100 7401 a003 7401 6a04  t.......t...t.j.
+000006b0: 6401 a102 0100 7401 a005 6401 6401 6402  d.....t...d.d.d.
+000006c0: a103 0100 7401 6a06 7407 6a08 a009 7c00  ....t.j.t.j...|.
+000006d0: 6a0a 6403 a102 6700 6404 a201 6405 8d02  j.d...g.d...d...
+000006e0: 7d01 6700 6406 a201 7d02 740b 6a0c a00d  }.g.d...}.t.j...
+000006f0: 740c a00e 6407 6408 a102 740c a00e 6409  t...d.d...t...d.
+00000700: 640a a102 6702 a101 7d03 740c a00e 6407  d...g...}.t...d.
+00000710: 640b a102 7d04 740f a010 a100 6401 1900  d...}.t.....d...
+00000720: 640c 1700 7d05 7401 6a06 7c05 640d 1700  d...}.t.j.|.d...
+00000730: 7c03 7c04 640e 6703 6405 8d02 7c00 5f11  |.|.d.g.d...|._.
+00000740: 7412 640f 6410 8302 4400 5d1c 7d06 7401  t.d.d...D.].}.t.
+00000750: a013 7c00 6a11 7c06 7c02 7c06 640f 1800  ..|.j.|.|.|.d...
+00000760: 1900 a103 0100 71b0 7401 a013 7c00 6a11  ......q.t...|.j.
+00000770: 6411 6412 a103 0100 7401 a013 7c00 6a11  d.d.....t...|.j.
+00000780: 6413 6412 a103 0100 7401 6a06 7407 6a08  d.d.....t.j.t.j.
+00000790: a009 7c00 6a0a 6414 a102 6700 6415 a201  ..|.j.d...g.d...
+000007a0: 6416 6417 8d03 7d07 7401 6a06 7407 6a08  d.d...}.t.j.t.j.
+000007b0: a009 7c00 6a0a 6418 a102 6700 6419 a201  ..|.j.d...g.d...
+000007c0: 6416 6417 8d03 7d08 740c a00e 641a 6416  d.d...}.t...d.d.
+000007d0: a102 740c a00e 641b 641c a102 641d 6703  ..t...d.d...d.g.
+000007e0: 7d09 7401 6a06 7407 6a08 a009 7c00 6a0a  }.t.j.t.j...|.j.
+000007f0: 641e a102 7c09 641f 6417 8d03 7c00 5f14  d...|.d.d...|._.
+00000800: 7401 a015 7c00 6a11 6401 a102 6401 1900  t...|.j.d...d...
+00000810: 6400 640a 8502 1900 7d0a 7401 a015 7c00  d.d.....}.t...|.
+00000820: 6a11 6420 a102 6401 1900 7d0b 7401 a016  j.d ..d...}.t...
+00000830: 7c00 6a11 6411 a102 6401 1900 7401 a016  |.j.d...d...t...
+00000840: 7c00 6a11 6413 a102 6401 1900 6602 7d0c  |.j.d...d...f.}.
+00000850: 7c0a 7c0b 1700 7c0c 1700 7c00 5f17 7401  |.|...|...|._.t.
+00000860: a003 7401 6a04 6421 a102 0100 740b a018  ..t.j.d!....t...
+00000870: 7c00 6a17 a101 a019 740b 6a1a a101 5300  |.j.....t.j...S.
+00000880: 2922 4e72 0100 0000 69f6 ffff ff7a 0a70  )"Nr....i....z.p
+00000890: 6c61 6e65 2e75 7264 6629 0372 0100 0000  lane.urdf).r....
+000008a0: 7201 0000 00e7 cdcc cccc cccc e4bf 2901  r.............).
+000008b0: da0c 6261 7365 506f 7369 7469 6f6e 2909  ..basePosition).
+000008c0: 7201 0000 0067 85eb 51b8 1e85 cbbf 7201  r....g..Q.....r.
+000008d0: 0000 0067 8fc2 f528 5c8f 04c0 7201 0000  ...g...(\...r...
+000008e0: 00e7 0c02 2b87 16d9 0240 7239 0000 00e7  ....+....@r9....
+000008f0: 7b14 ae47 e17a b43f 723a 0000 0072 0f00  {..G.z.?r:...r..
+00000900: 0000 6733 3333 3333 33d3 bf67 0000 0000  ..g333333..g....
+00000910: 0000 f43f 7216 0000 0067 0000 0000 0000  ...?r....g......
+00000920: 0440 7a10 2f72 6f76 6572 5f61 726d 2f64  .@z./rover_arm/d
+00000930: 6174 612f 7a0d 726f 7665 725f 6172 6d2e  ata/z.rover_arm.
+00000940: 786d 6c67 0000 0000 0000 e0bf e907 0000  xmlg............
+00000950: 00e9 0e00 0000 e910 0000 0072 1500 0000  ...........r....
+00000960: e911 0000 007a 1074 6162 6c65 2f74 6162  .....z.table/tab
+00000970: 6c65 2e75 7264 6629 03e7 0000 0000 0000  le.urdf)........
+00000980: e03f 7201 0000 0072 3700 0000 723f 0000  .?r....r7...r?..
+00000990: 0029 0272 3800 0000 5a0d 676c 6f62 616c  .).r8...Z.global
+000009a0: 5363 616c 696e 677a 1174 7261 792f 7472  Scalingz.tray/tr
+000009b0: 6179 626f 782e 7572 6466 2903 67cd cccc  aybox.urdf).g...
+000009c0: cccc ccdc 3f72 0100 0000 6771 3d0a d7a3  ....?r....gq=...
+000009d0: 70d5 bf67 9a99 9999 9999 d93f 679a 9999  p..g.......?g...
+000009e0: 9999 99a9 bfe7 9a99 9999 9999 a93f 720b  .............?r.
+000009f0: 0000 007a 1972 616e 646f 6d5f 7572 6466  ...z.random_urdf
+00000a00: 732f 3030 302f 3030 302e 7572 6466 679a  s/000/000.urdfg.
+00000a10: 9999 9999 99e9 3fe9 1200 0000 7212 0000  ......?.....r...
+00000a20: 0029 1bda 0c73 7465 705f 636f 756e 7465  .)...step_counte
+00000a30: 7272 1e00 0000 5a0f 7265 7365 7453 696d  rr....Z.resetSim
+00000a40: 756c 6174 696f 6e5a 1863 6f6e 6669 6775  ulationZ.configu
+00000a50: 7265 4465 6275 6756 6973 7561 6c69 7a65  reDebugVisualize
+00000a60: 725a 1443 4f56 5f45 4e41 424c 455f 5245  rZ.COV_ENABLE_RE
+00000a70: 4e44 4552 494e 475a 0a73 6574 4772 6176  NDERINGZ.setGrav
+00000a80: 6974 795a 086c 6f61 6455 5244 46da 026f  ityZ.loadURDF..o
+00000a90: 73da 0470 6174 68da 046a 6f69 6e72 1a00  s..path..joinr..
+00000aa0: 0000 7225 0000 00da 0672 616e 646f 6dda  ..r%.....random.
+00000ab0: 0663 686f 6963 65da 0775 6e69 666f 726d  .choice..uniform
+00000ac0: da04 7369 7465 da0f 6765 7473 6974 6570  ..site..getsitep
+00000ad0: 6163 6b61 6765 73da 0b72 6f76 6572 6172  ackages..roverar
+00000ae0: 6d55 6964 da05 7261 6e67 655a 0f72 6573  mUid..rangeZ.res
+00000af0: 6574 4a6f 696e 7453 7461 7465 da09 6f62  etJointState..ob
+00000b00: 6a65 6374 5569 64da 0c67 6574 4c69 6e6b  jectUid..getLink
+00000b10: 5374 6174 65da 0d67 6574 4a6f 696e 7453  State..getJointS
+00000b20: 7461 7465 da0b 6f62 7365 7276 6174 696f  tate..observatio
+00000b30: 6e72 2600 0000 da06 6173 7479 7065 da07  nr&.....astype..
+00000b40: 666c 6f61 7433 3229 0d72 3100 0000 5a08  float32).r1...Z.
+00000b50: 706c 616e 6555 6964 5a0a 7265 7374 5f70  planeUidZ.rest_p
+00000b60: 6f73 6573 5a05 785f 706f 735a 0579 5f70  osesZ.x_posZ.y_p
+00000b70: 6f73 da08 4241 5345 5f44 4952 da01 695a  os..BASE_DIR..iZ
+00000b80: 0874 6162 6c65 5569 645a 0774 7261 7955  .tableUidZ.trayU
+00000b90: 6964 da0c 7374 6174 655f 6f62 6a65 6374  id..state_object
+00000ba0: da0b 7374 6174 655f 726f 7665 72da 0973  ..state_rover..s
+00000bb0: 7461 7465 5f61 726d da0d 7374 6174 655f  tate_arm..state_
+00000bc0: 6669 6e67 6572 7372 3400 0000 7234 0000  fingersr4...r4..
+00000bd0: 0072 3500 0000 da05 7265 7365 7438 0000  .r5.....reset8..
+00000be0: 0073 3000 0000 0001 0601 0801 0e02 0e02  .s0.............
+00000bf0: 1e02 0802 2001 0c02 1001 1a03 0e01 1a01  .... ...........
+00000c00: 1001 1002 2001 2002 1a01 1e02 1a01 1201  .... . .........
+00000c10: 2402 0e02 0e01 7a11 526f 7665 7241 726d  $.....z.RoverArm
+00000c20: 456e 762e 7265 7365 7463 0200 0000 0000  Env.resetc......
+00000c30: 0000 0000 0000 1a00 0000 0800 0000 0300  ................
+00000c40: 0000 73ba 0200 0074 00a0 0164 0174 026a  ..s....t...d.t.j
+00000c50: 030b 0074 026a 0364 021b 0067 03a1 017d  ...t.j.d...g...}
+00000c60: 0264 0389 0087 0066 0164 0464 0584 087c  .d.....f.d.d...|
+00000c70: 0164 0664 0785 0219 0044 0083 015c 037d  .d.d.....D...\.}
+00000c80: 037d 047d 057c 0164 0719 007d 0674 00a0  .}.}.|.d...}.t..
+00000c90: 0488 016a 0564 08a1 027d 077c 0764 0919  ...j.d...}.|.d..
+00000ca0: 007d 087c 0864 0919 007c 0317 007c 0864  .}.|.d...|...|.d
+00000cb0: 0a19 007c 0417 007c 0864 0619 007c 0517  ...|...|.d...|..
+00000cc0: 0067 037d 0974 00a0 0688 016a 0564 087c  .g.}.t.....j.d.|
+00000cd0: 097c 02a1 047d 0a7c 0a64 0064 0b85 0219  .|...}.|.d.d....
+00000ce0: 007c 0a64 0b64 0c85 0219 0002 007d 0b7d  .|.d.d.......}.}
+00000cf0: 0c74 00a0 0788 016a 0574 0874 0964 0d64  .t.....j.t.t.d.d
+00000d00: 0e83 0283 0164 0f64 1067 0217 0074 006a  .....d.d.g...t.j
+00000d10: 0a74 087c 0c83 0164 067c 0667 0114 0017  .t.|...d.|.g....
+00000d20: 00a1 0401 007c 0164 0064 0685 0219 005c  .....|.d.d.....\
+00000d30: 027d 0d7d 0e74 0b74 0c7c 0d64 1183 0264  .}.}.t.t.|.d...d
+00000d40: 0a83 027d 0d74 0c74 0b7c 0e64 1283 0264  ...}.t.t.|.d...d
+00000d50: 1383 027d 0e74 006a 0788 016a 0588 016a  ...}.t.j...j...j
+00000d60: 0d74 006a 0a7c 0e67 0164 0614 0064 148d  .t.j.|.g.d...d..
+00000d70: 0401 0088 016a 0e0b 0088 016a 0e88 016a  .....j.....j...j
+00000d80: 0f14 0088 016a 1017 0014 007d 0f88 016a  .....j.....}...j
+00000d90: 117c 0d14 007c 0f17 007d 1088 016a 0e64  .|...|...}...j.d
+00000da0: 157c 1014 0017 0088 015f 0e74 0b74 0c88  .|......._.t.t..
+00000db0: 016a 0e88 016a 120b 0083 0288 016a 1283  .j...j.......j..
+00000dc0: 0288 015f 0e74 006a 0788 016a 0588 016a  ..._.t.j...j...j
+00000dd0: 1374 006a 1488 016a 0e67 0164 1614 0064  .t.j...j.g.d...d
+00000de0: 1767 0164 1614 0064 188d 0501 0074 00a0  .g.d...d.....t..
+00000df0: 15a1 0001 0074 00a0 1688 016a 17a1 015c  .....t.....j...\
+00000e00: 027d 117d 1274 00a0 0488 016a 0564 09a1  .}.}.t.....j.d..
+00000e10: 0264 0919 0064 0064 0685 0219 007d 1374  .d...d.d.....}.t
+00000e20: 00a0 0488 016a 0564 08a1 0264 0919 007d  .....j.d...d...}
+00000e30: 1474 00a0 1888 016a 0564 0fa1 0264 0919  .t.....j.d...d..
+00000e40: 0074 00a0 1888 016a 0564 10a1 0264 0919  .t.....j.d...d..
+00000e50: 0066 027d 157c 1164 0619 0064 096b 0490  .f.}.|.d...d.k..
+00000e60: 0272 2e64 0a7d 1664 197d 1788 01a0 19a1  .r.d.}.d.}......
+00000e70: 0001 006e 0864 097d 1664 1a7d 1788 0104  ...n.d.}.d.}....
+00000e80: 006a 1a64 0a37 0002 005f 1a87 0166 0164  .j.d.7..._...f.d
+00000e90: 1b64 1c84 087d 187c 187c 1383 0190 0273  .d...}.|.|.....s
+00000ea0: 6a64 117d 1664 197d 1788 01a0 19a1 0001  jd.}.d.}........
+00000eb0: 0088 016a 1a88 016a 1b6b 0490 0272 8864  ...j...j.k...r.d
+00000ec0: 097d 1664 197d 1788 01a0 19a1 0001 0064  .}.d.}.........d
+00000ed0: 1d7c 1169 017d 197c 137c 1417 007c 1517  .|.i.}.|.|...|..
+00000ee0: 0088 015f 1c74 1da0 1e88 016a 1ca1 01a0  ..._.t.....j....
+00000ef0: 1f74 1d6a 20a1 017c 167c 177c 1966 0453  .t.j ..|.|.|.f.S
+00000f00: 0029 1e4e 6700 0000 0000 0000 0067 0000  .).Ng........g..
+00000f10: 0000 0000 0040 7240 0000 0063 0100 0000  .....@r@...c....
+00000f20: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000f30: 1300 0000 7314 0000 0067 007c 005d 0c7d  ....s....g.|.].}
+00000f40: 017c 0188 0014 0091 0271 0453 0072 3400  .|.......q.S.r4.
+00000f50: 0000 7234 0000 0029 02da 022e 30da 0178  ..r4...)....0..x
+00000f60: 2901 da02 6476 7234 0000 0072 3500 0000  )...dvr4...r5...
+00000f70: da0a 3c6c 6973 7463 6f6d 703e 6200 0000  ..<listcomp>b...
+00000f80: f300 0000 007a 2452 6f76 6572 4172 6d45  .....z$RoverArmE
+00000f90: 6e76 2e73 7465 702e 3c6c 6f63 616c 733e  nv.step.<locals>
+00000fa0: 2e3c 6c69 7374 636f 6d70 3e72 1600 0000  .<listcomp>r....
+00000fb0: 7214 0000 0072 4100 0000 7201 0000 0072  r....rA...r....r
+00000fc0: 1200 0000 e906 0000 00e9 0d00 0000 723b  ..............r;
+00000fd0: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
+00000fe0: 0000 720f 0000 0072 1300 0000 7210 0000  ..r....r....r...
+00000ff0: 0029 02da 0b63 6f6e 7472 6f6c 4d6f 6465  .)...controlMode
+00001000: 5a0f 7461 7267 6574 506f 7369 7469 6f6e  Z.targetPosition
+00001010: 7367 1111 1111 1111 a13f 7211 0000 00e9  sg.......?r.....
+00001020: 0a00 0000 2905 5a0c 626f 6479 556e 6971  ....).Z.bodyUniq
+00001030: 7565 4964 5a0c 6a6f 696e 7449 6e64 6963  ueIdZ.jointIndic
+00001040: 6573 7261 0000 005a 1074 6172 6765 7456  esra...Z.targetV
+00001050: 656c 6f63 6974 6965 735a 0666 6f72 6365  elocitiesZ.force
+00001060: 7354 4663 0100 0000 0000 0000 0000 0000  sTFc............
+00001070: 0400 0000 0200 0000 1300 0000 733c 0000  ............s<..
+00001080: 007c 005c 027d 017d 027c 0188 006a 000b  .|.\.}.}.|...j..
+00001090: 006b 046f 1c7c 0188 006a 006b 007d 037c  .k.o.|...j.k.}.|
+000010a0: 036f 367c 0288 006a 000b 006b 046f 367c  .o6|...j...k.o6|
+000010b0: 0288 006a 006b 007d 037c 0353 00a9 014e  ...j.k.}.|.S...N
+000010c0: 2901 7228 0000 0029 0472 5600 0000 5a02  ).r(...).rV...Z.
+000010d0: 7278 5a02 7279 5a07 696e 426f 756e 64a9  rxZ.ryZ.inBound.
+000010e0: 0172 3100 0000 7234 0000 0072 3500 0000  .r1...r4...r5...
+000010f0: da06 696e 4761 6d65 9f00 0000 7308 0000  ..inGame....s...
+00001100: 0000 0108 0116 011a 017a 2052 6f76 6572  .........z Rover
+00001110: 4172 6d45 6e76 2e73 7465 702e 3c6c 6f63  ArmEnv.step.<loc
+00001120: 616c 733e 2e69 6e47 616d 655a 0f6f 626a  als>.inGameZ.obj
+00001130: 6563 745f 706f 7369 7469 6f6e 2921 721e  ect_position)!r.
+00001140: 0000 005a 1667 6574 5175 6174 6572 6e69  ...Z.getQuaterni
+00001150: 6f6e 4672 6f6d 4575 6c65 72da 046d 6174  onFromEuler..mat
+00001160: 68da 0270 6972 4e00 0000 724b 0000 005a  h..pirN...rK...Z
+00001170: 1a63 616c 6375 6c61 7465 496e 7665 7273  .calculateInvers
+00001180: 654b 696e 656d 6174 6963 735a 1973 6574  eKinematicsZ.set
+00001190: 4a6f 696e 744d 6f74 6f72 436f 6e74 726f  JointMotorContro
+000011a0: 6c41 7272 6179 da04 6c69 7374 724c 0000  lArray..listrL..
+000011b0: 005a 1050 4f53 4954 494f 4e5f 434f 4e54  .Z.POSITION_CONT
+000011c0: 524f 4cda 036d 696e da03 6d61 7872 2a00  ROL..min..maxr*.
+000011d0: 0000 722c 0000 0072 2e00 0000 722d 0000  ..r,...r....r-..
+000011e0: 0072 2f00 0000 7230 0000 0072 2b00 0000  .r/...r0...r+...
+000011f0: 5a10 5645 4c4f 4349 5459 5f43 4f4e 5452  Z.VELOCITY_CONTR
+00001200: 4f4c 5a0e 7374 6570 5369 6d75 6c61 7469  OLZ.stepSimulati
+00001210: 6f6e 5a1d 6765 7442 6173 6550 6f73 6974  onZ.getBasePosit
+00001220: 696f 6e41 6e64 4f72 6965 6e74 6174 696f  ionAndOrientatio
+00001230: 6e72 4d00 0000 724f 0000 00da 0563 6c6f  nrM...rO.....clo
+00001240: 7365 7242 0000 0072 1b00 0000 7250 0000  serB...r....rP..
+00001250: 0072 2500 0000 7226 0000 0072 5100 0000  .r%...r&...rQ...
+00001260: 7252 0000 0029 1a72 3100 0000 da06 6163  rR...).r1.....ac
+00001270: 7469 6f6e 5a0b 6f72 6965 6e74 6174 696f  tionZ.orientatio
+00001280: 6e5a 0464 785f 615a 0464 795f 615a 0464  nZ.dx_aZ.dy_aZ.d
+00001290: 7a5f 615a 0766 696e 6765 7273 5a0b 6375  z_aZ.fingersZ.cu
+000012a0: 7272 656e 7450 6f73 655a 0f63 7572 7265  rrentPoseZ.curre
+000012b0: 6e74 506f 7369 7469 6f6e 5a0b 6e65 7750  ntPositionZ.newP
+000012c0: 6f73 6974 696f 6e5a 0a6a 6f69 6e74 506f  ositionZ.jointPo
+000012d0: 7365 735a 106a 6f69 6e74 506f 7365 735f  sesZ.jointPoses_
+000012e0: 726f 7665 725a 0e6a 6f69 6e74 506f 7365  roverZ.jointPose
+000012f0: 735f 6172 6d5a 0874 6872 6f74 746c 655a  s_armZ.throttleZ
+00001300: 0e73 7465 6572 696e 675f 616e 676c 655a  .steering_angleZ
+00001310: 0866 7269 6374 696f 6e5a 0c61 6363 656c  .frictionZ.accel
+00001320: 6572 6174 696f 6e72 5500 0000 da01 5f72  erationrU....._r
+00001330: 5600 0000 7257 0000 0072 5800 0000 da06  V...rW...rX.....
+00001340: 7265 7761 7264 da04 646f 6e65 7265 0000  reward..donere..
+00001350: 00da 0469 6e66 6f72 3400 0000 2902 725c  ...infor4...).r\
+00001360: 0000 0072 3100 0000 7235 0000 00da 0473  ...r1...r5.....s
+00001370: 7465 705e 0000 0073 7200 0000 0002 1a01  tep^...sr.......
+00001380: 0401 2001 0802 0e02 0801 0a01 0a01 0afe  .. .............
+00001390: 0403 1201 1a01 3402 1004 1001 1003 0c01  ......4.........
+000013a0: 0401 08fe 0606 1001 04ff 0603 0e03 1002  ................
+000013b0: 1a04 0401 0401 0401 0401 0a01 08fb 0607  ................
+000013c0: 0802 1001 1a01 1201 2402 0e01 0401 0401  ........$.......
+000013d0: 0a02 0401 0401 0e01 0c06 0a01 0401 0401  ................
+000013e0: 0802 0e01 0401 0401 0802 0802 0e02 7a10  ..............z.
+000013f0: 526f 7665 7241 726d 456e 762e 7374 6570  RoverArmEnv.step
+00001400: 4e63 0300 0000 0000 0000 0000 0000 0c00  Nc..............
+00001410: 0000 0800 0000 4300 0000 7334 0100 007c  ......C...s4...|
+00001420: 0164 006b 0273 107c 0264 006b 0272 1c7c  .d.k.s.|.d.k.r.|
+00001430: 006a 007d 017c 006a 017d 0274 026a 037c  .j.}.|.j.}.t.j.|
+00001440: 006a 047c 006a 057c 006a 067c 006a 0764  .j.|.j.|.j.|.j.d
+00001450: 0164 0264 038d 067d 0374 026a 0367 0064  .d.d...}.t.j.g.d
+00001460: 04a2 0164 0564 0664 0764 0164 0264 038d  ...d.d.d.d.d.d..
+00001470: 067d 0474 026a 0864 0874 097c 0183 017c  .}.t.j.d.t.|...|
+00001480: 021b 0064 0964 0a64 0b8d 047d 0574 026a  ...d.d.d...}.t.j
+00001490: 0a7c 017c 027c 037c 0574 026a 0b64 0c8d  .|.|.|.|.t.j.d..
+000014a0: 055c 057d 067d 067d 077d 067d 0674 026a  .\.}.}.}.}.}.t.j
+000014b0: 0a7c 017c 027c 047c 0574 026a 0b64 0c8d  .|.|.|.|.t.j.d..
+000014c0: 055c 057d 067d 067d 087d 067d 0674 0c6a  .\.}.}.}.}.}.t.j
+000014d0: 0d7c 0774 0c6a 0e64 0d8d 027d 0974 0ca0  .|.t.j.d...}.t..
+000014e0: 0f7c 097c 027c 0164 0e66 03a1 0264 0064  .|.|.|.d.f...d.d
+000014f0: 0085 0264 0064 0085 0264 0064 0f85 0266  ...d.d...d.d...f
+00001500: 0319 007d 0974 0c6a 0d7c 0874 0c6a 0e64  ...}.t.j.|.t.j.d
+00001510: 0d8d 027d 0a74 0ca0 0f7c 0a7c 027c 0164  ...}.t...|.|.|.d
+00001520: 0e66 03a1 0264 0064 0085 0264 0064 0085  .f...d.d...d.d..
+00001530: 0264 0064 0f85 0266 0319 007d 0a74 0c6a  .d.d...f...}.t.j
+00001540: 107c 097c 0a66 0264 0164 108d 027d 0b7c  .|.|.f.d.d...}.|
+00001550: 0b53 0029 114e 7201 0000 0072 1600 0000  .S.).Nr....r....
+00001560: 2906 720e 0000 00da 0864 6973 7461 6e63  ).r......distanc
+00001570: 655a 0379 6177 5a05 7069 7463 68da 0472  eZ.yawZ.pitch..r
+00001580: 6f6c 6c5a 0b75 7041 7869 7349 6e64 6578  ollZ.upAxisIndex
+00001590: 2903 e766 6666 6666 66e6 3f72 0100 0000  )..ffffff.?r....
+000015a0: 7240 0000 0072 7400 0000 e95a 0000 0069  r@...rt....Z...i
+000015b0: baff ffff e93c 0000 0067 9a99 9999 9999  .....<...g......
+000015c0: b93f 6700 0000 0000 0059 4029 045a 0366  .?g......Y@).Z.f
+000015d0: 6f76 da06 6173 7065 6374 5a07 6e65 6172  ov..aspectZ.near
+000015e0: 5661 6c5a 0666 6172 5661 6c29 0572 3200  ValZ.farVal).r2.
+000015f0: 0000 7233 0000 005a 0a76 6965 774d 6174  ..r3...Z.viewMat
+00001600: 7269 785a 1070 726f 6a65 6374 696f 6e4d  rixZ.projectionM
+00001610: 6174 7269 785a 0872 656e 6465 7265 7229  atrixZ.renderer)
+00001620: 01da 0564 7479 7065 7211 0000 0072 0c00  ...dtyper....r..
+00001630: 0000 2901 da04 6178 6973 2911 721c 0000  ..)...axis).r...
+00001640: 0072 1d00 0000 721e 0000 005a 2163 6f6d  .r....r....Z!com
+00001650: 7075 7465 5669 6577 4d61 7472 6978 4672  puteViewMatrixFr
+00001660: 6f6d 5961 7750 6974 6368 526f 6c6c 7223  omYawPitchRollr#
+00001670: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00001680: 0000 5a1a 636f 6d70 7574 6550 726f 6a65  ..Z.computeProje
+00001690: 6374 696f 6e4d 6174 7269 7846 4f56 da05  ctionMatrixFOV..
+000016a0: 666c 6f61 745a 0e67 6574 4361 6d65 7261  floatZ.getCamera
+000016b0: 496d 6167 655a 1945 525f 4255 4c4c 4554  ImageZ.ER_BULLET
+000016c0: 5f48 4152 4457 4152 455f 4f50 454e 474c  _HARDWARE_OPENGL
+000016d0: 7225 0000 0072 2600 0000 da05 7569 6e74  r%...r&.....uint
+000016e0: 38da 0772 6573 6861 7065 da0b 636f 6e63  8..reshape..conc
+000016f0: 6174 656e 6174 6529 0c72 3100 0000 7232  atenate).r1...r2
+00001700: 0000 0072 3300 0000 5a0c 7669 6577 5f6d  ...r3...Z.view_m
+00001710: 6174 7269 7831 5a0c 7669 6577 5f6d 6174  atrix1Z.view_mat
+00001720: 7269 7832 5a0b 7072 6f6a 5f6d 6174 7269  rix2Z.proj_matri
+00001730: 7872 6d00 0000 5a03 7078 315a 0370 7832  xrm...Z.px1Z.px2
+00001740: 5a0a 7267 625f 6172 7261 7931 5a0a 7267  Z.rgb_array1Z.rg
+00001750: 625f 6172 7261 7932 7208 0000 0072 3400  b_array2r....r4.
+00001760: 0000 7234 0000 0072 3500 0000 da06 7265  ..r4...r5.....re
+00001770: 6e64 6572 b600 0000 7350 0000 0000 0710  nder....sP......
+00001780: 0106 0106 0308 0104 0104 0104 0102 0102  ................
+00001790: fb06 060a 0102 0102 0102 0102 0102 fb06  ................
+000017a0: 0606 010a 0102 0102 fd06 0506 0102 0102  ................
+000017b0: 0102 0104 fc10 0606 0102 0102 0102 0104  ................
+000017c0: fc10 0610 0128 0210 0128 0312 027a 1252  .....(...(...z.R
+000017d0: 6f76 6572 4172 6d45 6e76 2e72 656e 6465  overArmEnv.rende
+000017e0: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
+000017f0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00001800: 006a 0053 0072 6300 0000 2901 7250 0000  .j.S.rc...).rP..
+00001810: 0072 6400 0000 7234 0000 0072 3400 0000  .rd...r4...r4...
+00001820: 7235 0000 00da 0a5f 6765 745f 7374 6174  r5....._get_stat
+00001830: 65ea 0000 0073 0200 0000 0001 7a16 526f  e....s......z.Ro
+00001840: 7665 7241 726d 456e 762e 5f67 6574 5f73  verArmEnv._get_s
+00001850: 7461 7465 6301 0000 0000 0000 0000 0000  tatec...........
+00001860: 0001 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00001870: 0000 7400 a001 a100 0100 6400 5300 7263  ..t.......d.S.rc
+00001880: 0000 0029 0272 1e00 0000 5a0a 6469 7363  ...).r....Z.disc
+00001890: 6f6e 6e65 6374 7264 0000 0072 3400 0000  onnectrd...r4...
+000018a0: 7234 0000 0072 3500 0000 726b 0000 00ed  r4...r5...rk....
+000018b0: 0000 0073 0200 0000 0001 7a11 526f 7665  ...s......z.Rove
+000018c0: 7241 726d 456e 762e 636c 6f73 6529 024e  rArmEnv.close).N
+000018d0: 4e29 0cda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+000018e0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000018f0: 6c6e 616d 655f 5fda 086d 6574 6164 6174  lname__..metadat
+00001900: 61da 0d70 7962 756c 6c65 745f 6461 7461  a..pybullet_data
+00001910: 5a0b 6765 7444 6174 6150 6174 6872 3600  Z.getDataPathr6.
+00001920: 0000 7259 0000 0072 7100 0000 727e 0000  ..rY...rq...r~..
+00001930: 0072 7f00 0000 726b 0000 0072 3400 0000  .r....rk...r4...
+00001940: 7234 0000 0072 3400 0000 7235 0000 0072  r4...r4...r5...r
+00001950: 0600 0000 0e00 0000 7312 0000 0008 010c  ........s.......
+00001960: 020c 0104 ff0a 2708 2608 580a 3408 0372  ......'.&.X.4..r
+00001970: 0600 0000 2911 da03 6779 6d72 0200 0000  ....)...gymr....
+00001980: 7203 0000 0072 0400 0000 da09 6779 6d2e  r....r......gym.
+00001990: 7574 696c 7372 0500 0000 7243 0000 005a  utilsr....rC...Z
+000019a0: 0870 7962 756c 6c65 7472 1e00 0000 7284  .pybulletr....r.
+000019b0: 0000 0072 6600 0000 da05 6e75 6d70 7972  ...rf.....numpyr
+000019c0: 2500 0000 7246 0000 0072 4900 0000 da03  %...rF...rI.....
+000019d0: 456e 7672 0600 0000 7234 0000 0072 3400  Envr....r4...r4.
+000019e0: 0000 7234 0000 0072 3500 0000 da08 3c6d  ..r4...r5.....<m
+000019f0: 6f64 756c 653e 0100 0000 7314 0000 0008  odule>....s.....
+00001a00: 0114 010c 0208 0108 0108 0108 0108 0108  ................
+00001a10: 0108 03                                  ...
```

### Comparing `rover_arm-1.1.3/rover_arm/envs/roverarm_env.py` & `rover_arm-1.1.4/rover_arm/envs/roverarm_env.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.1.4/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.1.4/rover_arm/envs/roverarm_env_place.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm/keyboard_control.py` & `rover_arm-1.1.4/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.3/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.1.4/rover_arm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover-arm
-Version: 1.1.3
+Version: 1.1.4
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.3/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.1.4/rover_arm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,11 @@
 rover_arm/data/meshes/visual/link5.mtl
 rover_arm/data/meshes/visual/link5.obj
 rover_arm/data/meshes/visual/link6.mtl
 rover_arm/data/meshes/visual/link6.obj
 rover_arm/envs/__init__.py
 rover_arm/envs/roverarm_env.py
 rover_arm/envs/roverarm_env_arrange.py
+rover_arm/envs/roverarm_env_gym.py
 rover_arm/envs/roverarm_env_place.py
 rover_arm/envs/__pycache__/__init__.cpython-39.pyc
 rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
```

### Comparing `rover_arm-1.1.3/setup.py` & `rover_arm-1.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.1.3',
+    version='1.1.4',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
-    install_requires=['gym', 'pybullet'],  # And any other dependencies foo needs
+    install_requires=['gymnasium', 'pybullet', 'gym'],  # And any other dependencies foo needs
     extras_require = {
         'dev':  ['pynput']
     }
 )
```

