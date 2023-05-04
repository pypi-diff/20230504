# Comparing `tmp/urgxy_env-0.1.6.tar.gz` & `tmp/urgxy_env-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.6.tar", last modified: Thu May  4 07:03:03 2023, max compression
+gzip compressed data, was "urgxy_env-0.1.7.tar", last modified: Thu May  4 09:04:56 2023, max compression
```

## Comparing `urgxy_env-0.1.6.tar` & `urgxy_env-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.633360 urgxy_env-0.1.6/
--rw-rw-rw-   0        0        0      175 2023-05-04 07:03:03.632362 urgxy_env-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-04 07:03:03.633360 urgxy_env-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-05-04 07:02:59.000000 urgxy_env-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.607358 urgxy_env-0.1.6/urgxy_env/
--rw-rw-rw-   0        0        0      131 2023-05-04 07:02:59.000000 urgxy_env-0.1.6/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.630360 urgxy_env-0.1.6/urgxy_env/envs/
--rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.6/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0     8857 2023-05-04 06:57:29.000000 urgxy_env-0.1.6/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.625364 urgxy_env-0.1.6/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      175 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.712963 urgxy_env-0.1.7/
+-rw-rw-rw-   0        0        0      175 2023-05-04 09:04:56.711963 urgxy_env-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:04:56.712963 urgxy_env-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-05-04 09:04:51.000000 urgxy_env-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.675908 urgxy_env-0.1.7/urgxy_env/
+-rw-rw-rw-   0        0        0      131 2023-05-04 09:04:51.000000 urgxy_env-0.1.7/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.710965 urgxy_env-0.1.7/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.7/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     9099 2023-05-04 09:03:09.000000 urgxy_env-0.1.7/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.703963 urgxy_env-0.1.7/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.6/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.1.7/urgxy_env/envs/env_urgxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import gym
 from gym import error, spaces, utils
 from gym.utils import seeding
-
+import csv
 import os
 import pybullet as p
 import pybullet_data
 import math
 import numpy as np
 import random
 
@@ -52,14 +52,15 @@
         # p.setJointMotorControl2(self.pandaUid, 20,  p.POSITION_CONTROL, jointPoses[11])
         p.setJointMotorControlArray(self.pandaUid, [15,16,17,18,19,20], p.POSITION_CONTROL, [jointPoses[6],jointPoses[7],jointPoses[8],jointPoses[9],jointPoses[10],jointPoses[11]])
         p.stepSimulation()
         state_robot = p.getLinkState(self.pandaUid, 20)[0]  #得到位置
 
         done = False
         goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
+        goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
         current = np.array( [state_robot[0],state_robot[1],state_robot[2]] )
         reward = -np.linalg.norm( current-goal )
         self.score = self.score + reward
         # reward = 0
         # if action[0]>0 and state_robot[0]-(-0.8746627265025098) < 0:
         #     reward += 1
         #     done = False
@@ -98,16 +99,19 @@
         # if action[2]<0 and state_robot[2]-0.23835711380789043 < 0:
         #     reward -= 1
         #     done = False
 
         self.step_counter += 1
 
         if self.step_counter > MAX_EPISODE_LEN:
-            file = open('test.csv', 'a+')
-            file.write(str(self.score))
+            list_score = [self.score]
+            np_score = np.array(list_score,'float')
+            file = open('test.csv', 'a+', newline='')
+            writer = csv.writer(file)
+            writer.writerow(np_score)
             file.close()
             reward = 0
             done = True
 
         #info = {'object_position': state_object}
         info = {'robot_position':state_robot}
         self.observation = state_robot
```

