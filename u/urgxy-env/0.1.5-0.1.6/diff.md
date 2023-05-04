# Comparing `tmp/urgxy_env-0.1.5.tar.gz` & `tmp/urgxy_env-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.5.tar", last modified: Wed Apr 26 10:59:30 2023, max compression
+gzip compressed data, was "urgxy_env-0.1.6.tar", last modified: Thu May  4 07:03:03 2023, max compression
```

## Comparing `urgxy_env-0.1.5.tar` & `urgxy_env-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/
--rw-rw-rw-   0        0        0      172 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-26 10:59:30.550740 urgxy_env-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.513991 urgxy_env-0.1.5/urgxy_env/
--rw-rw-rw-   0        0        0      127 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.548740 urgxy_env-0.1.5/urgxy_env/envs/
--rw-rw-rw-   0        0        0       45 2023-04-25 15:35:12.000000 urgxy_env-0.1.5/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0     8671 2023-04-26 10:59:26.000000 urgxy_env-0.1.5/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:59:30.540740 urgxy_env-0.1.5/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      172 2023-04-26 10:59:29.000000 urgxy_env-0.1.5/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:59:29.000000 urgxy_env-0.1.5/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 10:59:30.000000 urgxy_env-0.1.5/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.633360 urgxy_env-0.1.6/
+-rw-rw-rw-   0        0        0      175 2023-05-04 07:03:03.632362 urgxy_env-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:03:03.633360 urgxy_env-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-05-04 07:02:59.000000 urgxy_env-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.607358 urgxy_env-0.1.6/urgxy_env/
+-rw-rw-rw-   0        0        0      131 2023-05-04 07:02:59.000000 urgxy_env-0.1.6/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.630360 urgxy_env-0.1.6/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.6/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     8857 2023-05-04 06:57:29.000000 urgxy_env-0.1.6/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:03:03.625364 urgxy_env-0.1.6/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 07:03:03.000000 urgxy_env-0.1.6/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.5/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.1.6/urgxy_env/envs/env_urgxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import numpy as np
 import random
 
 
 MAX_EPISODE_LEN = 20*100
 
 class UrgxyEnv(gym.Env):
-    metadata = {'render.modes': ['human']}
 
+    metadata = {'render.modes': ['human']}
     def __init__(self):
+        self.score = 0
         self.step_counter = 0
         p.connect(p.GUI)
         p.resetDebugVisualizerCamera(cameraDistance=1.5, cameraYaw=0, cameraPitch=-40, cameraTargetPosition=[0.55,-0.35,0.2])
         # self.action_space = spaces.Box(np.array([-1]*4), np.array([1]*4))
         #         # self.observation_space = spaces.Box(np.array([-1]*5), np.array([1]*5))
         self.action_space = spaces.Box(np.array([-1] * 3), np.array([1] * 3))
         self.observation_space = spaces.Box(np.array([-1] * 3), np.array([1] * 3))
-
     def step(self, action):
         p.configureDebugVisualizer(p.COV_ENABLE_SINGLE_STEP_RENDERING)
         #orientation = p.getQuaternionFromEuler([0.,-math.pi,math.pi/2.])
         dv = 0.05
         dx = action[0] * dv
         dy = action[1] * dv
         dz = action[2] * dv
@@ -54,15 +54,15 @@
         p.stepSimulation()
         state_robot = p.getLinkState(self.pandaUid, 20)[0]  #得到位置
 
         done = False
         goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
         current = np.array( [state_robot[0],state_robot[1],state_robot[2]] )
         reward = -np.linalg.norm( current-goal )
-
+        self.score = self.score + reward
         # reward = 0
         # if action[0]>0 and state_robot[0]-(-0.8746627265025098) < 0:
         #     reward += 1
         #     done = False
         #
         # if action[0]<0 and state_robot[0]-(-0.8746627265025098) > 0:
         #     reward += 1
@@ -98,23 +98,26 @@
         # if action[2]<0 and state_robot[2]-0.23835711380789043 < 0:
         #     reward -= 1
         #     done = False
 
         self.step_counter += 1
 
         if self.step_counter > MAX_EPISODE_LEN:
+            file = open('test.csv', 'a+')
+            file.write(str(self.score))
+            file.close()
             reward = 0
             done = True
 
         #info = {'object_position': state_object}
         info = {'robot_position':state_robot}
         self.observation = state_robot
         return np.array(self.observation).astype(np.float32), reward, done, info
-
     def reset(self):
+        self.score=0
         self.step_counter = 0
         p.resetSimulation()
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,0) # we will enable rendering after we loaded everything
         urdfRootPath=pybullet_data.getDataPath()
         #p.setGravity(0,0,-10)
 
         planeUid = p.loadURDF(os.path.join(urdfRootPath,"plane.urdf"), basePosition=[0,0,-0.65])
@@ -148,15 +151,14 @@
         #state_object= [random.uniform(0.5,0.8),random.uniform(-0.2,0.2),0.05]
         #self.objectUid = p.loadURDF(os.path.join(urdfRootPath, "random_urdfs/000/000.urdf"), basePosition=state_object)
         state_robot = p.getLinkState(self.pandaUid, 20)[0]
         #state_fingers = (p.getJointState(self.pandaUid,9)[0], p.getJointState(self.pandaUid, 10)[0])
         self.observation = state_robot
         p.configureDebugVisualizer(p.COV_ENABLE_RENDERING,1)
         return np.array(self.observation).astype(np.float32)
-
     def render(self, mode='human'):
         view_matrix = p.computeViewMatrixFromYawPitchRoll(cameraTargetPosition=[0.7,0,0.05],
                                                             distance=.7,
                                                             yaw=90,
                                                             pitch=-70,
                                                             roll=0,
                                                             upAxisIndex=2)
@@ -171,13 +173,11 @@
                                               renderer=p.ER_BULLET_HARDWARE_OPENGL)
 
         rgb_array = np.array(px, dtype=np.uint8)
         rgb_array = np.reshape(rgb_array, (720,960, 4))
 
         rgb_array = rgb_array[:, :, :3]
         return rgb_array
-
     def _get_state(self):
         return self.observation
-
     def close(self):
         p.disconnect()
```

