# Comparing `tmp/diambra-arena-2.1.0rc5.tar.gz` & `tmp/diambra-arena-2.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.0rc5.tar", last modified: Tue Feb 14 14:33:43 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.0rc6.tar", last modified: Thu May  4 18:11:27 2023, max compression
```

## Comparing `diambra-arena-2.1.0rc5.tar` & `diambra-arena-2.1.0rc6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.940530 diambra-arena-2.1.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-02-14 14:33:43.940530 diambra-arena-2.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.928530 diambra-arena-2.1.0rc5/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.928530 diambra-arena-2.1.0rc5/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.928530 diambra-arena-2.1.0rc5/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.932530 diambra-arena-2.1.0rc5/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.932530 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.932530 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.932530 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.936530 diambra-arena-2.1.0rc5/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    55998 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/.splashScreen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.936530 diambra-arena-2.1.0rc5/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.940530 diambra-arena-2.1.0rc5/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-02-14 14:33:43.000000 diambra-arena-2.1.0rc5/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-14 14:33:43.000000 diambra-arena-2.1.0rc5/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 14:33:43.000000 diambra-arena-2.1.0rc5/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-14 14:33:43.000000 diambra-arena-2.1.0rc5/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 14:33:43.000000 diambra-arena-2.1.0rc5/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 14:33:43.940530 diambra-arena-2.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:33:43.940530 diambra-arena-2.1.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-02-14 14:33:26.000000 diambra-arena-2.1.0rc5/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.081343 diambra-arena-2.1.0rc6/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.085343 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.089343 diambra-arena-2.1.0rc6/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    55998 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/.splashScreen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.093343 diambra-arena-2.1.0rc6/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.093343 diambra-arena-2.1.0rc6/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16900 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 18:11:27.000000 diambra-arena-2.1.0rc6/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:11:27.097343 diambra-arena-2.1.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6112 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-04 18:11:01.000000 diambra-arena-2.1.0rc6/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.0rc5/LICENSE.txt` & `diambra-arena-2.1.0rc6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/PKG-INFO` & `diambra-arena-2.1.0rc6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc5
+Version: 2.1.0rc6
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -19,74 +19,93 @@
 Provides-Extra: core
 Provides-Extra: tests
 Provides-Extra: stable-baselines
 Provides-Extra: stable-baselines3
 Provides-Extra: ray-rllib
 License-File: LICENSE.txt
 
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
-  <a href="https://discord.gg/tFDS2UN5sv">Discord</a> •
+  <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
 <a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
 </p>
 
 # DIAMBRA Arena
 
+## Index
+
+- **[Overview](#overview)**
+- **[Competition Platform](#competition-platform)**
+- **[Installation](#installation)**
+- **[Quickstart & Examples](#quickstart--examples)**
+- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
+- **[References](#references)**
+- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
+- **[Citation](#citation)**
+- **[Terms of Use](#terms-of-use)**
+
+## Overview
+
 DIAMBRA Arena is a software package featuring a collection of **high-quality environments for Reinforcement Learning research and experimentation**. It provides a standard interface to popular arcade emulated video games, offering a **Python API fully compliant with OpenAI Gym format**, that makes its adoption smooth and straightforward.
 
 It **supports all major Operating Systems** (Linux, Windows and MacOS) and **can be easily installed via Python PIP**, as described in the **[installation section](#installation)** below. It is **completely free to use**, the user only needs to <a href="https://diambra.ai/register/" target="_blank">register on the official website</a>.
 
 In addition, it comes with a <a href="https://docs.diambra.ai" target="_blank">comprehensive documentation</a>, and this repository provides a **collection of examples** covering main use cases of interest **that can be run in just a few steps**.
 
 #### Main Features
 
 All environments are episodic Reinforcement Learning tasks, with discrete actions (gamepad buttons) and observations composed by screen pixels plus additional numerical data (RAM values like characters health bars or characters stage side).
 
 They all **support both single player (1P) as well as two players (2P) mode**, making them the perfect resource to explore all the following Reinforcement Learning subfields:
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
 | :-------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
 |                                                      Standard RL                                                      |                                               Competitive<br>Multi-Agent                                                |                                               Competitive<br> Human-Agent                                                |                                                   Self-Play                                                    |                                                   Imitation Learning                                                    |                                                   Human-in-the-Loop                                                    |
 
 #### Available Games
 
 Interfaced games have been selected among the most popular fighting retro-games. While sharing the same fundamental mechanics, they provide slightly different challenges, with specific features such as different type and number of characters, how to perform combos, health bars recharging, etc.
 
 Whenever possible, games are released with all hidden/bonus characters unlocked.
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
-## Index
+## Competition Platform
 
-- **[Installation](#installation)**
-- **[Quickstart & Examples](#quickstart--examples)**
-- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
-- **[AI Tournaments](#ai-tournaments)**
-- **[References](#references)**
-- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
-- **[Citation](#citation)**
-- **[Terms of Use](#terms-of-use)**
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+
+Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
+
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
+
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+
+Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
+
+We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
@@ -97,15 +116,15 @@
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
 Check available games with the following command:
 
 ```
@@ -184,53 +203,42 @@
 - Multi Player Environment
 - Wrappers Options
 - Human Experience Recorder
 - Imitation Learning
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/github.gif" alt="diambraGif" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
 DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
 
 Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
-## AI Tournaments
-
-We are about to launch our AI Tournaments Platform, where every coder will be able to train his agents and compete.
-There will be one-to-one fights against other agents, challenges to collect accolades & bages, and matches versus human players.
-
-**<a href="https://diambra.ai/register/" target="_blank">Join us to become an early member!</a>**
-
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/WideFlyer.jpg" alt="diambraAITournament" width="100%"/>
-
-Our very first AI Tournament **has been an amazing experience!** Participants trained an AI algorithm to effectively play Dead Or Alive++. The three best algorithms participated in the final event and **competed for the 1400 CHF prize.**
-
 ## References
 
 - Documentation: <a href="https://docs.diambra.ai" target="_blank">https://docs.diambra.ai</a>
 - Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 - Website: <a href="https://diambra.ai" target="_blank">https://diambra.ai</a>
-- Discord: <a href="https://discord.gg/tFDS2UN5sv" target="_blank">https://discord.gg/tFDS2UN5sv</a>
+- Discord: <a href="https://diambra.ai/discord" target="_blank">https://diambra.ai/discord</a>
 - Linkedin: <a href="https://www.linkedin.com/company/diambra" target="_blank">https://www.linkedin.com/company/diambra</a>
 - Twitch: <a href="https://www.twitch.tv/diambra_ai" target="_blank">https://www.twitch.tv/diambra_ai</a>
 - YouTube: <a href="https://www.youtube.com/c/diambra_ai" target="_blank">https://www.youtube.com/c/diambra_ai</a>
 - Twitter: <a href="https://twitter.com/diambra_ai" target="_blank">https://twitter.com/diambra_ai</a>
 
 ## Support, Feature Requests & Bugs Reports
 
-To receive support, use the dedicated channel in our <a href="https://discord.gg/tFDS2UN5sv" target="_blank">Discord Server</a>.
+To receive support, use the dedicated channel in our <a href="https://diambra.ai/discord" target="_blank">Discord Server</a>.
 
-To request features or report bugs, use the <a href="https://github.com/diambra/diambraArena/issues" target="_blank">GitHub Issue Tracker</a>.
+To request features or report bugs, use the <a href="https://github.com/diambra/arena/issues" target="_blank">GitHub Issue Tracker</a>.
 
 ## Citation
 
 Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 
 ```LaTex
 @article{Palmas22,
@@ -248,8 +256,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Right Reserved.
+###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc5 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc6 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -10,31 +10,37 @@
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown Provides-Extra: core
 Provides-Extra: tests Provides-Extra: stable-baselines Provides-Extra: stable-
 baselines3 Provides-Extra: ray-rllib License-File: LICENSE.txt [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
-# DIAMBRA Arena DIAMBRA Arena is a software package featuring a collection of
-**high-quality environments for Reinforcement Learning research and
-experimentation**. It provides a standard interface to popular arcade emulated
-video games, offering a **Python API fully compliant with OpenAI Gym format**,
-that makes its adoption smooth and straightforward. It **supports all major
-Operating Systems** (Linux, Windows and MacOS) and **can be easily installed
-via Python PIP**, as described in the **[installation section](#installation)**
-below. It is **completely free to use**, the user only needs to register_on_the
-official_website. In addition, it comes with a comprehensive_documentation, and
-this repository provides a **collection of examples** covering main use cases
-of interest **that can be run in just a few steps**. #### Main Features All
-environments are episodic Reinforcement Learning tasks, with discrete actions
-(gamepad buttons) and observations composed by screen pixels plus additional
-numerical data (RAM values like characters health bars or characters stage
-side). They all **support both single player (1P) as well as two players (2P)
-mode**, making them the perfect resource to explore all the following
-Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
+# DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
+(#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
+Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
+Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
+(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
+feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
+Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
+a collection of **high-quality environments for Reinforcement Learning research
+and experimentation**. It provides a standard interface to popular arcade
+emulated video games, offering a **Python API fully compliant with OpenAI Gym
+format**, that makes its adoption smooth and straightforward. It **supports all
+major Operating Systems** (Linux, Windows and MacOS) and **can be easily
+installed via Python PIP**, as described in the **[installation section]
+(#installation)** below. It is **completely free to use**, the user only needs
+to register_on_the_official_website. In addition, it comes with a comprehensive
+documentation, and this repository provides a **collection of examples**
+covering main use cases of interest **that can be run in just a few steps**.
+#### Main Features All environments are episodic Reinforcement Learning tasks,
+with discrete actions (gamepad buttons) and observations composed by screen
+pixels plus additional numerical data (RAM values like characters health bars
+or characters stage side). They all **support both single player (1P) as well
+as two players (2P) mode**, making them the perfect resource to explore all the
+following Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
 [competitiveHa] | [selfPlay] | [imitationLearning] | [humanInTheLoop] | | :----
 -------------------------------------------------------------------------------
 --------------------------------: | :------------------------------------------
 ---------------------------------------------------------------------------: |
 :------------------------------------------------------------------------------
 ----------------------------------------: | :----------------------------------
 --------------------------------------------------------------------------: | :
@@ -68,31 +74,33 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Index - **[Installation]
-(#installation)** - **[Quickstart & Examples](#quickstart--examples)** - **
-[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-
-compatibility)** - **[AI Tournaments](#ai-tournaments)** - **[References]
-(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
-feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
-Use](#terms-of-use)** ## Installation - Create_an_account_on_our_website, it
-requires just a few clicks and is 100% free - Install Docker Desktop: Linux |
-Windows | MacOS - Install DIAMBRA Command Line Interface: `python3 -m pip
-install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
-arena` **Using a virtual environment to isolate your python packages
-installation is strongly suggested** ## Quickstart & Examples DIAMBRA Arena
-usage follows the standard RL interaction framework: the agent sends an action
-to the environment, which process it and performs a transition accordingly,
-from the starting state to the new state, returning the observation and the
-reward to the agent to close the interaction loop. The figure below shows this
-typical interaction scheme and data flow.
+Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Leaderboard] Our competition platform allows you to submit your agents and
+compete with other coders around the globe in epic video games tournaments! It
+features a public global leaderboard where users are ranked by the best score
+achieved by their agents in our different environments. It also offers you the
+possibility to unlock cool achievements depending on the performances of your
+agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
+are streamed on our Twitch channel. We aimed at making the submission process
+as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
+account_on_our_website, it requires just a few clicks and is 100% free -
+Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
+Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
+m pip install diambra-arena` **Using a virtual environment to isolate your
+python packages installation is strongly suggested** ## Quickstart & Examples
+DIAMBRA Arena usage follows the standard RL interaction framework: the agent
+sends an action to the environment, which process it and performs a transition
+accordingly, from the starting state to the new state, returning the
+observation and the reward to the agent to close the interaction loop. The
+figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check available games with the
 following command: ``` diambra arena list-roms ``` Output example: ```shell
 [...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
 SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
 'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
@@ -130,31 +138,24 @@
 illustrated in detail in the documentation and in the DIAMBRA_Agents
 repository. It can easily be interfaced with any other package in a similar
 way. Native interfaces, that can be installed with the dedicated options listed
 below, have been tested with the following versions: - Stable Baselines 3 |
 `pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
 Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## AI Tournaments We are about to launch our AI
-Tournaments Platform, where every coder will be able to train his agents and
-compete. There will be one-to-one fights against other agents, challenges to
-collect accolades & bages, and matches versus human players. **Join_us_to
-become_an_early_member!** [diambraAITournament] Our very first AI Tournament
-**has been an amazing experience!** Participants trained an AI algorithm to
-effectively play Dead Or Alive++. The three best algorithms participated in the
-final event and **competed for the 1400 CHF prize.** ## References -
-Documentation: https://docs.diambra.ai - Paper: https://arxiv.org/abs/
-2210.10595 - Website: https://diambra.ai - Discord: https://discord.gg/
-tFDS2UN5sv - Linkedin: https://www.linkedin.com/company/diambra - Twitch:
-https://www.twitch.tv/diambra_ai - YouTube: https://www.youtube.com/c/
-diambra_ai - Twitter: https://twitter.com/diambra_ai ## Support, Feature
-Requests & Bugs Reports To receive support, use the dedicated channel in our
-Discord_Server. To request features or report bugs, use the GitHub_Issue
-Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595 ```LaTex @article
-{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA Arena: a New
-Reinforcement Learning Platform for Research and Experimentation}", journal =
-{arXiv e-prints}, keywords = {reinforcement learning, transfer learning, multi-
-agent, games}, year = 2022, month = oct, eid = {arXiv:2210.10595}, pages =
-{arXiv:2210.10595}, archivePrefix = {arXiv}, eprint = {2210.10595},
-primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA Arena software package is
-subject to our Terms_of_Use. By using it, you accept them in full. ######
-DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All Right Reserved.
+- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
+- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
+Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
+company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
+www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
+Support, Feature Requests & Bugs Reports To receive support, use the dedicated
+channel in our Discord_Server. To request features or report bugs, use the
+GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
+```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
+Arena: a New Reinforcement Learning Platform for Research and
+Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
+learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
+= {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
+eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
+Arena software package is subject to our Terms_of_Use. By using it, you accept
+them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
+Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc5/README.md` & `diambra-arena-2.1.0rc6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,86 @@
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
-  <a href="https://discord.gg/tFDS2UN5sv">Discord</a> •
+  <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
 <a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
 </p>
 
 # DIAMBRA Arena
 
+## Index
+
+- **[Overview](#overview)**
+- **[Competition Platform](#competition-platform)**
+- **[Installation](#installation)**
+- **[Quickstart & Examples](#quickstart--examples)**
+- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
+- **[References](#references)**
+- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
+- **[Citation](#citation)**
+- **[Terms of Use](#terms-of-use)**
+
+## Overview
+
 DIAMBRA Arena is a software package featuring a collection of **high-quality environments for Reinforcement Learning research and experimentation**. It provides a standard interface to popular arcade emulated video games, offering a **Python API fully compliant with OpenAI Gym format**, that makes its adoption smooth and straightforward.
 
 It **supports all major Operating Systems** (Linux, Windows and MacOS) and **can be easily installed via Python PIP**, as described in the **[installation section](#installation)** below. It is **completely free to use**, the user only needs to <a href="https://diambra.ai/register/" target="_blank">register on the official website</a>.
 
 In addition, it comes with a <a href="https://docs.diambra.ai" target="_blank">comprehensive documentation</a>, and this repository provides a **collection of examples** covering main use cases of interest **that can be run in just a few steps**.
 
 #### Main Features
 
 All environments are episodic Reinforcement Learning tasks, with discrete actions (gamepad buttons) and observations composed by screen pixels plus additional numerical data (RAM values like characters health bars or characters stage side).
 
 They all **support both single player (1P) as well as two players (2P) mode**, making them the perfect resource to explore all the following Reinforcement Learning subfields:
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
 | :-------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
 |                                                      Standard RL                                                      |                                               Competitive<br>Multi-Agent                                                |                                               Competitive<br> Human-Agent                                                |                                                   Self-Play                                                    |                                                   Imitation Learning                                                    |                                                   Human-in-the-Loop                                                    |
 
 #### Available Games
 
 Interfaced games have been selected among the most popular fighting retro-games. While sharing the same fundamental mechanics, they provide slightly different challenges, with specific features such as different type and number of characters, how to perform combos, health bars recharging, etc.
 
 Whenever possible, games are released with all hidden/bonus characters unlocked.
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
-## Index
+## Competition Platform
 
-- **[Installation](#installation)**
-- **[Quickstart & Examples](#quickstart--examples)**
-- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
-- **[AI Tournaments](#ai-tournaments)**
-- **[References](#references)**
-- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
-- **[Citation](#citation)**
-- **[Terms of Use](#terms-of-use)**
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+
+Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
+
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
+
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+
+Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
+
+We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
@@ -72,15 +91,15 @@
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
 Check available games with the following command:
 
 ```
@@ -159,53 +178,42 @@
 - Multi Player Environment
 - Wrappers Options
 - Human Experience Recorder
 - Imitation Learning
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/github.gif" alt="diambraGif" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
 DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
 
 Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
-## AI Tournaments
-
-We are about to launch our AI Tournaments Platform, where every coder will be able to train his agents and compete.
-There will be one-to-one fights against other agents, challenges to collect accolades & bages, and matches versus human players.
-
-**<a href="https://diambra.ai/register/" target="_blank">Join us to become an early member!</a>**
-
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/WideFlyer.jpg" alt="diambraAITournament" width="100%"/>
-
-Our very first AI Tournament **has been an amazing experience!** Participants trained an AI algorithm to effectively play Dead Or Alive++. The three best algorithms participated in the final event and **competed for the 1400 CHF prize.**
-
 ## References
 
 - Documentation: <a href="https://docs.diambra.ai" target="_blank">https://docs.diambra.ai</a>
 - Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 - Website: <a href="https://diambra.ai" target="_blank">https://diambra.ai</a>
-- Discord: <a href="https://discord.gg/tFDS2UN5sv" target="_blank">https://discord.gg/tFDS2UN5sv</a>
+- Discord: <a href="https://diambra.ai/discord" target="_blank">https://diambra.ai/discord</a>
 - Linkedin: <a href="https://www.linkedin.com/company/diambra" target="_blank">https://www.linkedin.com/company/diambra</a>
 - Twitch: <a href="https://www.twitch.tv/diambra_ai" target="_blank">https://www.twitch.tv/diambra_ai</a>
 - YouTube: <a href="https://www.youtube.com/c/diambra_ai" target="_blank">https://www.youtube.com/c/diambra_ai</a>
 - Twitter: <a href="https://twitter.com/diambra_ai" target="_blank">https://twitter.com/diambra_ai</a>
 
 ## Support, Feature Requests & Bugs Reports
 
-To receive support, use the dedicated channel in our <a href="https://discord.gg/tFDS2UN5sv" target="_blank">Discord Server</a>.
+To receive support, use the dedicated channel in our <a href="https://diambra.ai/discord" target="_blank">Discord Server</a>.
 
-To request features or report bugs, use the <a href="https://github.com/diambra/diambraArena/issues" target="_blank">GitHub Issue Tracker</a>.
+To request features or report bugs, use the <a href="https://github.com/diambra/arena/issues" target="_blank">GitHub Issue Tracker</a>.
 
 ## Citation
 
 Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 
 ```LaTex
 @article{Palmas22,
@@ -223,8 +231,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Right Reserved.
+###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,28 +1,34 @@
 [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
-# DIAMBRA Arena DIAMBRA Arena is a software package featuring a collection of
-**high-quality environments for Reinforcement Learning research and
-experimentation**. It provides a standard interface to popular arcade emulated
-video games, offering a **Python API fully compliant with OpenAI Gym format**,
-that makes its adoption smooth and straightforward. It **supports all major
-Operating Systems** (Linux, Windows and MacOS) and **can be easily installed
-via Python PIP**, as described in the **[installation section](#installation)**
-below. It is **completely free to use**, the user only needs to register_on_the
-official_website. In addition, it comes with a comprehensive_documentation, and
-this repository provides a **collection of examples** covering main use cases
-of interest **that can be run in just a few steps**. #### Main Features All
-environments are episodic Reinforcement Learning tasks, with discrete actions
-(gamepad buttons) and observations composed by screen pixels plus additional
-numerical data (RAM values like characters health bars or characters stage
-side). They all **support both single player (1P) as well as two players (2P)
-mode**, making them the perfect resource to explore all the following
-Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
+# DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
+(#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
+Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
+Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
+(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
+feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
+Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
+a collection of **high-quality environments for Reinforcement Learning research
+and experimentation**. It provides a standard interface to popular arcade
+emulated video games, offering a **Python API fully compliant with OpenAI Gym
+format**, that makes its adoption smooth and straightforward. It **supports all
+major Operating Systems** (Linux, Windows and MacOS) and **can be easily
+installed via Python PIP**, as described in the **[installation section]
+(#installation)** below. It is **completely free to use**, the user only needs
+to register_on_the_official_website. In addition, it comes with a comprehensive
+documentation, and this repository provides a **collection of examples**
+covering main use cases of interest **that can be run in just a few steps**.
+#### Main Features All environments are episodic Reinforcement Learning tasks,
+with discrete actions (gamepad buttons) and observations composed by screen
+pixels plus additional numerical data (RAM values like characters health bars
+or characters stage side). They all **support both single player (1P) as well
+as two players (2P) mode**, making them the perfect resource to explore all the
+following Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
 [competitiveHa] | [selfPlay] | [imitationLearning] | [humanInTheLoop] | | :----
 -------------------------------------------------------------------------------
 --------------------------------: | :------------------------------------------
 ---------------------------------------------------------------------------: |
 :------------------------------------------------------------------------------
 ----------------------------------------: | :----------------------------------
 --------------------------------------------------------------------------: | :
@@ -56,31 +62,33 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Index - **[Installation]
-(#installation)** - **[Quickstart & Examples](#quickstart--examples)** - **
-[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-
-compatibility)** - **[AI Tournaments](#ai-tournaments)** - **[References]
-(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
-feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
-Use](#terms-of-use)** ## Installation - Create_an_account_on_our_website, it
-requires just a few clicks and is 100% free - Install Docker Desktop: Linux |
-Windows | MacOS - Install DIAMBRA Command Line Interface: `python3 -m pip
-install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
-arena` **Using a virtual environment to isolate your python packages
-installation is strongly suggested** ## Quickstart & Examples DIAMBRA Arena
-usage follows the standard RL interaction framework: the agent sends an action
-to the environment, which process it and performs a transition accordingly,
-from the starting state to the new state, returning the observation and the
-reward to the agent to close the interaction loop. The figure below shows this
-typical interaction scheme and data flow.
+Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Leaderboard] Our competition platform allows you to submit your agents and
+compete with other coders around the globe in epic video games tournaments! It
+features a public global leaderboard where users are ranked by the best score
+achieved by their agents in our different environments. It also offers you the
+possibility to unlock cool achievements depending on the performances of your
+agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
+are streamed on our Twitch channel. We aimed at making the submission process
+as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
+account_on_our_website, it requires just a few clicks and is 100% free -
+Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
+Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
+m pip install diambra-arena` **Using a virtual environment to isolate your
+python packages installation is strongly suggested** ## Quickstart & Examples
+DIAMBRA Arena usage follows the standard RL interaction framework: the agent
+sends an action to the environment, which process it and performs a transition
+accordingly, from the starting state to the new state, returning the
+observation and the reward to the agent to close the interaction loop. The
+figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check available games with the
 following command: ``` diambra arena list-roms ``` Output example: ```shell
 [...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
 SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
 'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
@@ -118,31 +126,24 @@
 illustrated in detail in the documentation and in the DIAMBRA_Agents
 repository. It can easily be interfaced with any other package in a similar
 way. Native interfaces, that can be installed with the dedicated options listed
 below, have been tested with the following versions: - Stable Baselines 3 |
 `pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
 Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## AI Tournaments We are about to launch our AI
-Tournaments Platform, where every coder will be able to train his agents and
-compete. There will be one-to-one fights against other agents, challenges to
-collect accolades & bages, and matches versus human players. **Join_us_to
-become_an_early_member!** [diambraAITournament] Our very first AI Tournament
-**has been an amazing experience!** Participants trained an AI algorithm to
-effectively play Dead Or Alive++. The three best algorithms participated in the
-final event and **competed for the 1400 CHF prize.** ## References -
-Documentation: https://docs.diambra.ai - Paper: https://arxiv.org/abs/
-2210.10595 - Website: https://diambra.ai - Discord: https://discord.gg/
-tFDS2UN5sv - Linkedin: https://www.linkedin.com/company/diambra - Twitch:
-https://www.twitch.tv/diambra_ai - YouTube: https://www.youtube.com/c/
-diambra_ai - Twitter: https://twitter.com/diambra_ai ## Support, Feature
-Requests & Bugs Reports To receive support, use the dedicated channel in our
-Discord_Server. To request features or report bugs, use the GitHub_Issue
-Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595 ```LaTex @article
-{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA Arena: a New
-Reinforcement Learning Platform for Research and Experimentation}", journal =
-{arXiv e-prints}, keywords = {reinforcement learning, transfer learning, multi-
-agent, games}, year = 2022, month = oct, eid = {arXiv:2210.10595}, pages =
-{arXiv:2210.10595}, archivePrefix = {arXiv}, eprint = {2210.10595},
-primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA Arena software package is
-subject to our Terms_of_Use. By using it, you accept them in full. ######
-DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All Right Reserved.
+- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
+- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
+Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
+company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
+www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
+Support, Feature Requests & Bugs Reports To receive support, use the dedicated
+channel in our Discord_Server. To request features or report bugs, use the
+GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
+```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
+Arena: a New Reinforcement Learning Platform for Research and
+Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
+learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
+= {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
+eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
+Arena software package is subject to our Terms_of_Use. By using it, you accept
+them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
+Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/arena_gym.py` & `diambra-arena-2.1.0rc6/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.0rc6/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/engine/interface.py` & `diambra-arena-2.1.0rc6/diambra/arena/engine/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from diambra.engine import Client, model
 import grpc
 
 CONNECTION_FAILED_ERROR_TEXT = """DIAMBRA Arena failed to connect to the Engine Server.
  - If you are running a Python script, are you running with DIAMBRA CLI: `diambra run python script.py`?
  - If you are running a Python Notebook, have you started Jupyter Notebook with DIAMBRA CLI: `diambra run jupyter notebook`?
 
-See the docs (https://docs.diambra.ai) for additional details, or join DIAMBRA Discord Server (https://discord.gg/tFDS2UN5sv) for support."""
+See the docs (https://docs.diambra.ai) for additional details, or join DIAMBRA Discord Server (https://diambra.ai/discord) for support."""
 
 # DIAMBRA Env Gym
 class DiambraEngine:
     """Diambra Environment gym interface"""
 
     def __init__(self, env_address, grpc_timeout=60):
         self.logger = logging.getLogger(__name__)
```

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/env_settings.py` & `diambra-arena-2.1.0rc6/diambra/arena/env_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/make_env.py` & `diambra-arena-2.1.0rc6/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.0rc6/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/sb_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra-arena-2.1.0rc6/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/.splashScreen.gif` & `diambra-arena-2.1.0rc6/diambra/arena/utils/.splashScreen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/controller.py` & `diambra-arena-2.1.0rc6/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.0rc6/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/integratedGames.json` & `diambra-arena-2.1.0rc6/diambra/arena/utils/integratedGames.json`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/policies.py` & `diambra-arena-2.1.0rc6/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.0rc6/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.0rc6/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.0rc6/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.0rc6/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.0rc6/diambra_arena.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc5
+Version: 2.1.0rc6
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -19,74 +19,93 @@
 Provides-Extra: core
 Provides-Extra: tests
 Provides-Extra: stable-baselines
 Provides-Extra: stable-baselines3
 Provides-Extra: ray-rllib
 License-File: LICENSE.txt
 
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/github.png" alt="diambra" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.png" alt="diambra" width="100%"/>
 
 <p align="center">
   <a href="https://docs.diambra.ai">Documentation</a> •
   <a href="https://diambra.ai/">Website</a>
 </p>
 <p align="center">
   <a href="https://www.linkedin.com/company/diambra">Linkedin</a> •
-  <a href="https://discord.gg/tFDS2UN5sv">Discord</a> •
+  <a href="https://diambra.ai/discord">Discord</a> •
   <a href="https://www.twitch.tv/diambra_ai">Twitch</a> •
   <a href="https://www.youtube.com/c/diambra_ai">YouTube</a> •
   <a href="https://twitter.com/diambra_ai">Twitter</a>
 </p>
 
 <p align="center">
 <a href="https://arxiv.org/abs/2210.10595"><img src="http://img.shields.io/badge/paper-arxiv.2210.10595-B31B1B.svg" alt="Paper"/></a>
 </p>
 
 # DIAMBRA Arena
 
+## Index
+
+- **[Overview](#overview)**
+- **[Competition Platform](#competition-platform)**
+- **[Installation](#installation)**
+- **[Quickstart & Examples](#quickstart--examples)**
+- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
+- **[References](#references)**
+- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
+- **[Citation](#citation)**
+- **[Terms of Use](#terms-of-use)**
+
+## Overview
+
 DIAMBRA Arena is a software package featuring a collection of **high-quality environments for Reinforcement Learning research and experimentation**. It provides a standard interface to popular arcade emulated video games, offering a **Python API fully compliant with OpenAI Gym format**, that makes its adoption smooth and straightforward.
 
 It **supports all major Operating Systems** (Linux, Windows and MacOS) and **can be easily installed via Python PIP**, as described in the **[installation section](#installation)** below. It is **completely free to use**, the user only needs to <a href="https://diambra.ai/register/" target="_blank">register on the official website</a>.
 
 In addition, it comes with a <a href="https://docs.diambra.ai" target="_blank">comprehensive documentation</a>, and this repository provides a **collection of examples** covering main use cases of interest **that can be run in just a few steps**.
 
 #### Main Features
 
 All environments are episodic Reinforcement Learning tasks, with discrete actions (gamepad buttons) and observations composed by screen pixels plus additional numerical data (RAM values like characters health bars or characters stage side).
 
 They all **support both single player (1P) as well as two players (2P) mode**, making them the perfect resource to explore all the following Reinforcement Learning subfields:
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsCOM.png" alt="standardRl" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsAI.png" alt="competitiveMa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/AIvsHUM.png" alt="competitiveHa" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/SP.png" alt="selfPlay" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/IL.png" alt="imitationLearning" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/HITL.png" alt="humanInTheLoop" width="125"/> |
 | :-------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: |
 |                                                      Standard RL                                                      |                                               Competitive<br>Multi-Agent                                                |                                               Competitive<br> Human-Agent                                                |                                                   Self-Play                                                    |                                                   Imitation Learning                                                    |                                                   Human-in-the-Loop                                                    |
 
 #### Available Games
 
 Interfaced games have been selected among the most popular fighting retro-games. While sharing the same fundamental mechanics, they provide slightly different challenges, with specific features such as different type and number of characters, how to perform combos, health bars recharging, etc.
 
 Whenever possible, games are released with all hidden/bonus characters unlocked.
 
 Additional details can be found in the <a href="https://docs.diambra.ai/envs/games/" target="_blank">dedicated section</a> of our Documentation.
 
-| <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
+| <img src="https://raw.githubusercontent.com/diambra/arena/main/img/doapp.jpg" alt="doapp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/sfiii3n.jpg" alt="sfiii3n" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/tektagt.jpg" alt="tektagt" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/umk3.jpg" alt="umk3" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/samsh5sp.jpg" alt="samsh6sp" width="125"/> | <img src="https://raw.githubusercontent.com/diambra/arena/main/img/kof98umh.jpg" alt="kof98umh" width="125"/> |
 | :------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: |
 |                                             Dead<br>Or<br>Alive ++                                             |                                        Street<br>Fighter III<br>3rd Strike                                         |                                              Tekken Tag<br>Tournament                                              |                                        Ultimate<br>Mortal<br>Kombat 3                                        |                                           Samurai<br>Showdown<br>5 Special                                           |                                 The King of<br>Fighers '98<br>Ultimate<br>Match Hero                                 |
 
 **Many more are coming soon...**
 
-## Index
+## Competition Platform
 
-- **[Installation](#installation)**
-- **[Quickstart & Examples](#quickstart--examples)**
-- **[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-compatibility)**
-- **[AI Tournaments](#ai-tournaments)**
-- **[References](#references)**
-- **[Support, Feature Requests & Bugs Reports](#support-feature-requests--bugs-reports)**
-- **[Citation](#citation)**
-- **[Terms of Use](#terms-of-use)**
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/leaderboard.jpg" alt="DIAMBRA Leaderboard" width="100%"/>
+
+Our competition platform allows you to submit your agents and compete with other coders around the globe in epic video games tournaments!
+
+It features a public global leaderboard where users are ranked by the best score achieved by their agents in our different environments. 
+
+It also offers you the possibility to unlock cool achievements depending on the performances of your agent. 
+
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/achievements.jpg" alt="DIAMBRA Achievements" width="100%"/>
+
+Submitted agents are evaluated and their episodes are streamed on our Twitch channel.
+
+We aimed at making the submission process as smooth as possible, **<a href="https://diambra.ai/register/" target="_blank">join us and try it now!</a>**
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
@@ -97,15 +116,15 @@
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
-<img src="https://raw.githubusercontent.com/diambra/diambraArena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
 
 #### Download Game ROM(s) and Check Validity
 
 Check available games with the following command:
 
 ```
@@ -184,53 +203,42 @@
 - Multi Player Environment
 - Wrappers Options
 - Human Experience Recorder
 - Imitation Learning
 
 These examples show how to leverage both single and two players modes, how to set up environment wrappers specifying all their options, how to record human expert demonstrations and how to load them to apply imitation learning. They can be used as templates and starting points to explore all the features of the software package.
 
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/github.gif" alt="diambraGif" width="100%"/>
+<img src="https://raw.githubusercontent.com/diambra/arena/main/img/github.gif" alt="diambraGif" width="100%"/>
 
 ## Reinforcement Learning Libs Compatibility
 
 DIAMBRA Arena is built to maximize compatibility will all major Reinforcement Learning libraries. It natively provides interfaces with the two most import packages: Stable Baselines (both version 2 and 3) and Ray RLlib. Their usage is illustrated in detail in the <a href="https://docs.diambra.ai/handsonreinforcementlearning/" target="_blank">documentation</a> and in the <a href="https://github.com/diambra/agents" target="_blank">DIAMBRA Agents repository</a>. It can easily be interfaced with any other package in a similar way.
 
 Native interfaces, that can be installed with the dedicated options listed below, have been tested with the following versions:
 
 - Stable Baselines 3 | `pip install diambra-arena[stable-baselines3]` (<a href="https://stable-baselines3.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/DLR-RM/stable-baselines3" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines3/" target="_blank">Pypi</a>): 1.6.1
 - Ray RLlib | `pip install diambra-arena[ray-rllib]` (<a href="https://docs.ray.io/en/latest/index.html" target="_blank">Docs</a> - <a href="https://github.com/ray-project/ray" target="_blank">GitHub</a> - <a href="https://pypi.org/project/ray/" target="_blank">Pypi</a>): 2.0.0
 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (<a href="https://stable-baselines.readthedocs.io/en/master/index.html" target="_blank">Docs</a> - <a href="https://github.com/hill-a/stable-baselines" target="_blank">GitHub</a> - <a href="https://pypi.org/project/stable-baselines/" target="_blank">Pypi</a>): 2.10.2
 
-## AI Tournaments
-
-We are about to launch our AI Tournaments Platform, where every coder will be able to train his agents and compete.
-There will be one-to-one fights against other agents, challenges to collect accolades & bages, and matches versus human players.
-
-**<a href="https://diambra.ai/register/" target="_blank">Join us to become an early member!</a>**
-
-<img src="https://raw.githubusercontent.com/diambra/DIAMBRAenvironment/main/img/WideFlyer.jpg" alt="diambraAITournament" width="100%"/>
-
-Our very first AI Tournament **has been an amazing experience!** Participants trained an AI algorithm to effectively play Dead Or Alive++. The three best algorithms participated in the final event and **competed for the 1400 CHF prize.**
-
 ## References
 
 - Documentation: <a href="https://docs.diambra.ai" target="_blank">https://docs.diambra.ai</a>
 - Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 - Website: <a href="https://diambra.ai" target="_blank">https://diambra.ai</a>
-- Discord: <a href="https://discord.gg/tFDS2UN5sv" target="_blank">https://discord.gg/tFDS2UN5sv</a>
+- Discord: <a href="https://diambra.ai/discord" target="_blank">https://diambra.ai/discord</a>
 - Linkedin: <a href="https://www.linkedin.com/company/diambra" target="_blank">https://www.linkedin.com/company/diambra</a>
 - Twitch: <a href="https://www.twitch.tv/diambra_ai" target="_blank">https://www.twitch.tv/diambra_ai</a>
 - YouTube: <a href="https://www.youtube.com/c/diambra_ai" target="_blank">https://www.youtube.com/c/diambra_ai</a>
 - Twitter: <a href="https://twitter.com/diambra_ai" target="_blank">https://twitter.com/diambra_ai</a>
 
 ## Support, Feature Requests & Bugs Reports
 
-To receive support, use the dedicated channel in our <a href="https://discord.gg/tFDS2UN5sv" target="_blank">Discord Server</a>.
+To receive support, use the dedicated channel in our <a href="https://diambra.ai/discord" target="_blank">Discord Server</a>.
 
-To request features or report bugs, use the <a href="https://github.com/diambra/diambraArena/issues" target="_blank">GitHub Issue Tracker</a>.
+To request features or report bugs, use the <a href="https://github.com/diambra/arena/issues" target="_blank">GitHub Issue Tracker</a>.
 
 ## Citation
 
 Paper: <a href="https://arxiv.org/abs/2210.10595" target="_blank">https://arxiv.org/abs/2210.10595</a>
 
 ```LaTex
 @article{Palmas22,
@@ -248,8 +256,8 @@
  }
 ```
 
 ## Terms of Use
 
 DIAMBRA Arena software package is subject to our <a href="https://diambra.ai/terms" target="_blank">Terms of Use</a>. By using it, you accept them in full.
 
-###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Right Reserved.
+###### DIAMBRA™ is a Trade Mark, © Copyright 2018-2023. All Rights Reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc5 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc6 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -10,31 +10,37 @@
 Entertainment Classifier: Topic :: Games/Entertainment :: Arcade Classifier:
 Topic :: Education Description-Content-Type: text/markdown Provides-Extra: core
 Provides-Extra: tests Provides-Extra: stable-baselines Provides-Extra: stable-
 baselines3 Provides-Extra: ray-rllib License-File: LICENSE.txt [diambra]
                            Documentation â¢ Website
             Linkedin â¢ Discord â¢ Twitch â¢ YouTube â¢ Twitter
                                     [Paper]
-# DIAMBRA Arena DIAMBRA Arena is a software package featuring a collection of
-**high-quality environments for Reinforcement Learning research and
-experimentation**. It provides a standard interface to popular arcade emulated
-video games, offering a **Python API fully compliant with OpenAI Gym format**,
-that makes its adoption smooth and straightforward. It **supports all major
-Operating Systems** (Linux, Windows and MacOS) and **can be easily installed
-via Python PIP**, as described in the **[installation section](#installation)**
-below. It is **completely free to use**, the user only needs to register_on_the
-official_website. In addition, it comes with a comprehensive_documentation, and
-this repository provides a **collection of examples** covering main use cases
-of interest **that can be run in just a few steps**. #### Main Features All
-environments are episodic Reinforcement Learning tasks, with discrete actions
-(gamepad buttons) and observations composed by screen pixels plus additional
-numerical data (RAM values like characters health bars or characters stage
-side). They all **support both single player (1P) as well as two players (2P)
-mode**, making them the perfect resource to explore all the following
-Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
+# DIAMBRA Arena ## Index - **[Overview](#overview)** - **[Competition Platform]
+(#competition-platform)** - **[Installation](#installation)** - **[Quickstart &
+Examples](#quickstart--examples)** - **[Reinforcement Learning Libs
+Compatibility](#reinforcement-learning-libs-compatibility)** - **[References]
+(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
+feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
+Use](#terms-of-use)** ## Overview DIAMBRA Arena is a software package featuring
+a collection of **high-quality environments for Reinforcement Learning research
+and experimentation**. It provides a standard interface to popular arcade
+emulated video games, offering a **Python API fully compliant with OpenAI Gym
+format**, that makes its adoption smooth and straightforward. It **supports all
+major Operating Systems** (Linux, Windows and MacOS) and **can be easily
+installed via Python PIP**, as described in the **[installation section]
+(#installation)** below. It is **completely free to use**, the user only needs
+to register_on_the_official_website. In addition, it comes with a comprehensive
+documentation, and this repository provides a **collection of examples**
+covering main use cases of interest **that can be run in just a few steps**.
+#### Main Features All environments are episodic Reinforcement Learning tasks,
+with discrete actions (gamepad buttons) and observations composed by screen
+pixels plus additional numerical data (RAM values like characters health bars
+or characters stage side). They all **support both single player (1P) as well
+as two players (2P) mode**, making them the perfect resource to explore all the
+following Reinforcement Learning subfields: | [standardRl] | [competitiveMa] |
 [competitiveHa] | [selfPlay] | [imitationLearning] | [humanInTheLoop] | | :----
 -------------------------------------------------------------------------------
 --------------------------------: | :------------------------------------------
 ---------------------------------------------------------------------------: |
 :------------------------------------------------------------------------------
 ----------------------------------------: | :----------------------------------
 --------------------------------------------------------------------------: | :
@@ -68,31 +74,33 @@
 Tournament | Ultimate
 Mortal
 Kombat 3 | Samurai
 Showdown
 5 Special | The King of
 Fighers '98
 Ultimate
-Match Hero | **Many more are coming soon...** ## Index - **[Installation]
-(#installation)** - **[Quickstart & Examples](#quickstart--examples)** - **
-[Reinforcement Learning Libs Compatibility](#reinforcement-learning-libs-
-compatibility)** - **[AI Tournaments](#ai-tournaments)** - **[References]
-(#references)** - **[Support, Feature Requests & Bugs Reports](#support-
-feature-requests--bugs-reports)** - **[Citation](#citation)** - **[Terms of
-Use](#terms-of-use)** ## Installation - Create_an_account_on_our_website, it
-requires just a few clicks and is 100% free - Install Docker Desktop: Linux |
-Windows | MacOS - Install DIAMBRA Command Line Interface: `python3 -m pip
-install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
-arena` **Using a virtual environment to isolate your python packages
-installation is strongly suggested** ## Quickstart & Examples DIAMBRA Arena
-usage follows the standard RL interaction framework: the agent sends an action
-to the environment, which process it and performs a transition accordingly,
-from the starting state to the new state, returning the observation and the
-reward to the agent to close the interaction loop. The figure below shows this
-typical interaction scheme and data flow.
+Match Hero | **Many more are coming soon...** ## Competition Platform [DIAMBRA
+Leaderboard] Our competition platform allows you to submit your agents and
+compete with other coders around the globe in epic video games tournaments! It
+features a public global leaderboard where users are ranked by the best score
+achieved by their agents in our different environments. It also offers you the
+possibility to unlock cool achievements depending on the performances of your
+agent. [DIAMBRA Achievements] Submitted agents are evaluated and their episodes
+are streamed on our Twitch channel. We aimed at making the submission process
+as smooth as possible, **join_us_and_try_it_now!** ## Installation - Create_an
+account_on_our_website, it requires just a few clicks and is 100% free -
+Install Docker Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line
+Interface: `python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -
+m pip install diambra-arena` **Using a virtual environment to isolate your
+python packages installation is strongly suggested** ## Quickstart & Examples
+DIAMBRA Arena usage follows the standard RL interaction framework: the agent
+sends an action to the environment, which process it and performs a transition
+accordingly, from the starting state to the new state, returning the
+observation and the reward to the agent to close the interaction loop. The
+figure below shows this typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check available games with the
 following command: ``` diambra arena list-roms ``` Output example: ```shell
 [...] Title: Dead Or Alive ++ - GameId: doapp Difficulty levels: Min 1 - Max 4
 SHA256 sum: d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e
 Original ROM name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]',
 'dead-or-alive-japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack',
@@ -130,31 +138,24 @@
 illustrated in detail in the documentation and in the DIAMBRA_Agents
 repository. It can easily be interfaced with any other package in a similar
 way. Native interfaces, that can be installed with the dedicated options listed
 below, have been tested with the following versions: - Stable Baselines 3 |
 `pip install diambra-arena[stable-baselines3]` (Docs - GitHub - Pypi): 1.6.1 -
 Ray RLlib | `pip install diambra-arena[ray-rllib]` (Docs - GitHub - Pypi):
 2.0.0 - Stable Baselines | `pip install diambra-arena[stable-baselines]` (Docs
-- GitHub - Pypi): 2.10.2 ## AI Tournaments We are about to launch our AI
-Tournaments Platform, where every coder will be able to train his agents and
-compete. There will be one-to-one fights against other agents, challenges to
-collect accolades & bages, and matches versus human players. **Join_us_to
-become_an_early_member!** [diambraAITournament] Our very first AI Tournament
-**has been an amazing experience!** Participants trained an AI algorithm to
-effectively play Dead Or Alive++. The three best algorithms participated in the
-final event and **competed for the 1400 CHF prize.** ## References -
-Documentation: https://docs.diambra.ai - Paper: https://arxiv.org/abs/
-2210.10595 - Website: https://diambra.ai - Discord: https://discord.gg/
-tFDS2UN5sv - Linkedin: https://www.linkedin.com/company/diambra - Twitch:
-https://www.twitch.tv/diambra_ai - YouTube: https://www.youtube.com/c/
-diambra_ai - Twitter: https://twitter.com/diambra_ai ## Support, Feature
-Requests & Bugs Reports To receive support, use the dedicated channel in our
-Discord_Server. To request features or report bugs, use the GitHub_Issue
-Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595 ```LaTex @article
-{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA Arena: a New
-Reinforcement Learning Platform for Research and Experimentation}", journal =
-{arXiv e-prints}, keywords = {reinforcement learning, transfer learning, multi-
-agent, games}, year = 2022, month = oct, eid = {arXiv:2210.10595}, pages =
-{arXiv:2210.10595}, archivePrefix = {arXiv}, eprint = {2210.10595},
-primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA Arena software package is
-subject to our Terms_of_Use. By using it, you accept them in full. ######
-DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All Right Reserved.
+- GitHub - Pypi): 2.10.2 ## References - Documentation: https://docs.diambra.ai
+- Paper: https://arxiv.org/abs/2210.10595 - Website: https://diambra.ai -
+Discord: https://diambra.ai/discord - Linkedin: https://www.linkedin.com/
+company/diambra - Twitch: https://www.twitch.tv/diambra_ai - YouTube: https://
+www.youtube.com/c/diambra_ai - Twitter: https://twitter.com/diambra_ai ##
+Support, Feature Requests & Bugs Reports To receive support, use the dedicated
+channel in our Discord_Server. To request features or report bugs, use the
+GitHub_Issue_Tracker. ## Citation Paper: https://arxiv.org/abs/2210.10595
+```LaTex @article{Palmas22, author = {{Palmas}, Alessandro}, title = "{DIAMBRA
+Arena: a New Reinforcement Learning Platform for Research and
+Experimentation}", journal = {arXiv e-prints}, keywords = {reinforcement
+learning, transfer learning, multi-agent, games}, year = 2022, month = oct, eid
+= {arXiv:2210.10595}, pages = {arXiv:2210.10595}, archivePrefix = {arXiv},
+eprint = {2210.10595}, primaryClass = {cs.AI} } ``` ## Terms of Use DIAMBRA
+Arena software package is subject to our Terms_of_Use. By using it, you accept
+them in full. ###### DIAMBRAâ¢ is a Trade Mark, Â© Copyright 2018-2023. All
+Rights Reserved.
```

### Comparing `diambra-arena-2.1.0rc5/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.0rc6/diambra_arena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/setup.py` & `diambra-arena-2.1.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_gym_settings.py` & `diambra-arena-2.1.0rc6/tests/test_gym_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_imitation_learning.py` & `diambra-arena-2.1.0rc6/tests/test_imitation_learning.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_integration.py` & `diambra-arena-2.1.0rc6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_random.py` & `diambra-arena-2.1.0rc6/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_recording_settings.py` & `diambra-arena-2.1.0rc6/tests/test_recording_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_speed.py` & `diambra-arena-2.1.0rc6/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc5/tests/test_wrappers_settings.py` & `diambra-arena-2.1.0rc6/tests/test_wrappers_settings.py`

 * *Files identical despite different names*

