# Comparing `tmp/modular_rl-0.1.2.dev0.tar.gz` & `tmp/modular_rl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.1.2.dev0.tar", last modified: Thu May  4 12:25:42 2023, max compression
+gzip compressed data, was "modular_rl-0.1.3.tar", last modified: Thu May  4 14:22:10 2023, max compression
```

## Comparing `modular_rl-0.1.2.dev0.tar` & `modular_rl-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.706752 modular_rl-0.1.2.dev0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.2.dev0/LICENSE
--rw-rw-rw-   0        0        0     3622 2023-05-04 12:25:42.705753 modular_rl-0.1.2.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2244 2023-05-04 10:23:00.000000 modular_rl-0.1.2.dev0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.687035 modular_rl-0.1.2.dev0/modular_rl/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.700076 modular_rl-0.1.2.dev0/modular_rl/agents/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    17011 2023-05-04 10:15:10.000000 modular_rl-0.1.2.dev0/modular_rl/agents/agent_ppo.py
--rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/networks.py
--rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.2.dev0/modular_rl/settings.py
--rw-rw-rw-   0        0        0     2073 2023-05-04 09:57:12.000000 modular_rl-0.1.2.dev0/modular_rl/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.697076 modular_rl-0.1.2.dev0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     3622 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1425 2023-05-04 12:25:23.000000 modular_rl-0.1.2.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 12:25:42.706752 modular_rl-0.1.2.dev0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-05-04 12:25:17.000000 modular_rl-0.1.2.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.703723 modular_rl-0.1.2.dev0/tests/
--rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.2.dev0/tests/test.py
--rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.2.dev0/tests/test_modular.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:22:10.232549 modular_rl-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3617 2023-05-04 14:22:10.231549 modular_rl-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2244 2023-05-04 10:23:00.000000 modular_rl-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:22:10.211277 modular_rl-0.1.3/modular_rl/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.3/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:22:10.226211 modular_rl-0.1.3/modular_rl/agents/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.3/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0    17172 2023-05-04 14:16:43.000000 modular_rl-0.1.3/modular_rl/agents/agent_ppo.py
+-rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.3/modular_rl/networks.py
+-rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.3/modular_rl/settings.py
+-rw-rw-rw-   0        0        0     2070 2023-05-04 14:19:25.000000 modular_rl-0.1.3/modular_rl/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:22:10.222488 modular_rl-0.1.3/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     3617 2023-05-04 14:22:09.000000 modular_rl-0.1.3/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-04 14:22:10.000000 modular_rl-0.1.3/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:22:09.000000 modular_rl-0.1.3/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 14:22:09.000000 modular_rl-0.1.3/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 14:22:09.000000 modular_rl-0.1.3/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1421 2023-05-04 14:21:37.000000 modular_rl-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:22:10.232549 modular_rl-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      956 2023-05-04 14:21:32.000000 modular_rl-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:22:10.229537 modular_rl-0.1.3/tests/
+-rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.3/tests/test.py
+-rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.3/tests/test_modular.py
```

### Comparing `modular_rl-0.1.2.dev0/LICENSE` & `modular_rl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.2.dev0/PKG-INFO` & `modular_rl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.1.2.dev0
+Version: 0.1.3
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
```

### Comparing `modular_rl-0.1.2.dev0/README.md` & `modular_rl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.2.dev0/modular_rl/agents/agent_ppo.py` & `modular_rl-0.1.3/modular_rl/agents/agent_ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,25 @@
         self.gamma = setting.get('gamma', 0.99)
         self.lam = setting.get('lam', 0.95)
         self.clip_param = setting.get('clip_param', 0.2)
         self.early_stop_threshold = setting.get('early_stop_threshold', -1)
         self.done_loop_end = setting.get('done_loop_end', False)
         self.reward_print = setting.get('reward_print', True)
 
-        self.state = None
-
-        # Set learning episode parameters
+        # Set learn episode parameters
         self.episode_reward = 0
         self.total_reward = 0
         self.prev_reward = 0
         self.episode = 0
         self.avg_reward = 0
 
+        # Set learn modular parameters
+        self.state = None
+        self.dist = None
+
     # Implement PPO algorithm
     def compute_advantages(self, rewards, values, done, gamma=0.99, lam=0.95):
         """
         Compute advantages given the rewards, values, done flags, and discount factors.
 
         :param rewards: The rewards obtained from the environment.
         :type rewards: numpy.ndarray
@@ -176,14 +178,15 @@
         """
 
         state = self._check_state(self.state)
         state_tensor = torch.tensor(state, dtype=torch.float32)
         with torch.no_grad():
             action_probs = self.policy_net(state_tensor)
         dist = Categorical(action_probs)
+        self.dist = dist
         action = dist.sample()
         return action, dist
 
     def learn_step(self, state, timestep):
         """
         Takes a step in the environment and updates the PPO algorithm with the resulting state, reward, and action.
 
@@ -213,14 +216,17 @@
         :type reaction: tuple
         :param timestep: The current timestep of the training process.
         :type timestep: int
         :return: The resulting reward and whether the episode is done or not.
         :rtype: tuple(float, bool)
         """
 
+        if dist == None and self.dist:
+            dist = self.dist
+
         step_output = self.env.step(action.item())
         step_output_num = len(step_output)
 
         if step_output_num == 4:
             next_state, reward, is_done, _ = self.env.step(action.item())
         elif step_output_num == 5:
             next_state, reward, is_done, _, _ = self.env.step(action.item())
```

### Comparing `modular_rl-0.1.2.dev0/modular_rl/networks.py` & `modular_rl-0.1.3/modular_rl/networks.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.2.dev0/modular_rl/settings.py` & `modular_rl-0.1.3/modular_rl/settings.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.2.dev0/modular_rl/tester.py` & `modular_rl-0.1.3/modular_rl/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     env.learn_close()
 
     # env.save_model('test.pth')
 
 
 def manual_step(env):
     initial_state = env.learn_reset()
-    action, dist = env.select_action(initial_state)
-    env.update_step(initial_state, dist, action, -1)
+    action, _ = env.select_action(initial_state)
+    env.update_step(initial_state, None, action, -1)
```

### Comparing `modular_rl-0.1.2.dev0/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.1.3/modular_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.1.2.dev0
+Version: 0.1.3
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
```

### Comparing `modular_rl-0.1.2.dev0/pyproject.toml` & `modular_rl-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.1.2.dev"
+version = "0.1.3"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.1.2.dev0/setup.py` & `modular_rl-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.1.2.dev',
+    version='0.1.3',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

