# Comparing `tmp/modular_rl-0.1.0.dev0.tar.gz` & `tmp/modular_rl-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.1.0.dev0.tar", last modified: Thu May  4 06:32:37 2023, max compression
+gzip compressed data, was "modular_rl-0.1.1.dev0.tar", last modified: Thu May  4 10:19:00 2023, max compression
```

## Comparing `modular_rl-0.1.0.dev0.tar` & `modular_rl-0.1.1.dev0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 06:32:37.152915 modular_rl-0.1.0.dev0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.0.dev0/LICENSE
--rw-rw-rw-   0        0        0     3486 2023-05-04 06:32:37.151915 modular_rl-0.1.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2108 2023-05-04 06:14:59.000000 modular_rl-0.1.0.dev0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 06:32:37.136374 modular_rl-0.1.0.dev0/modular_rl/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:32:37.148615 modular_rl-0.1.0.dev0/modular_rl/agents/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    16022 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/agents/agent_ppo.py
--rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/networks.py
--rw-rw-rw-   0        0        0     2570 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/settings.py
--rw-rw-rw-   0        0        0     1785 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/modular_rl/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-04 06:32:37.146131 modular_rl-0.1.0.dev0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     3486 2023-05-04 06:32:36.000000 modular_rl-0.1.0.dev0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-05-04 06:32:36.000000 modular_rl-0.1.0.dev0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 06:32:36.000000 modular_rl-0.1.0.dev0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 06:32:36.000000 modular_rl-0.1.0.dev0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 06:32:36.000000 modular_rl-0.1.0.dev0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1425 2023-05-04 06:32:25.000000 modular_rl-0.1.0.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 06:32:37.152915 modular_rl-0.1.0.dev0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-05-04 06:12:40.000000 modular_rl-0.1.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.748791 modular_rl-0.1.1.dev0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.1.dev0/LICENSE
+-rw-rw-rw-   0        0        0     3477 2023-05-04 10:19:00.747342 modular_rl-0.1.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2099 2023-05-04 06:34:40.000000 modular_rl-0.1.1.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.729224 modular_rl-0.1.1.dev0/modular_rl/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.743354 modular_rl-0.1.1.dev0/modular_rl/agents/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0    17011 2023-05-04 10:15:10.000000 modular_rl-0.1.1.dev0/modular_rl/agents/agent_ppo.py
+-rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/networks.py
+-rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.1.dev0/modular_rl/settings.py
+-rw-rw-rw-   0        0        0     2073 2023-05-04 09:57:12.000000 modular_rl-0.1.1.dev0/modular_rl/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.739282 modular_rl-0.1.1.dev0/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     3477 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1425 2023-05-04 10:18:38.000000 modular_rl-0.1.1.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:19:00.748791 modular_rl-0.1.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-05-04 10:18:45.000000 modular_rl-0.1.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.746157 modular_rl-0.1.1.dev0/tests/
+-rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.1.dev0/tests/test.py
+-rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.1.dev0/tests/test_modular.py
```

### Comparing `modular_rl-0.1.0.dev0/LICENSE` & `modular_rl-0.1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.0.dev0/PKG-INFO` & `modular_rl-0.1.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.1.0.dev0
+Version: 0.1.1.dev0
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ModularRL
-=======
 
 ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. 
 The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 
 ## Installation
 
 ```powershell
```

### Comparing `modular_rl-0.1.0.dev0/README.md` & `modular_rl-0.1.1.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # ModularRL
-=======
 
 ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. 
 The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 
 ## Installation
 
 ```powershell
```

### Comparing `modular_rl-0.1.0.dev0/modular_rl/agents/agent_ppo.py` & `modular_rl-0.1.1.dev0/modular_rl/agents/agent_ppo.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.ppo_epochs = setting.get('ppo_epochs', 4)
         self.mini_batch_size = setting.get('mini_batch_size', 64)
         self.gamma = setting.get('gamma', 0.99)
         self.lam = setting.get('lam', 0.95)
         self.clip_param = setting.get('clip_param', 0.2)
         self.early_stop_threshold = setting.get('early_stop_threshold', -1)
         self.done_loop_end = setting.get('done_loop_end', False)
+        self.reward_print = setting.get('reward_print', True)
 
         self.state = None
 
         # Set learning episode parameters
         self.episode_reward = 0
         self.total_reward = 0
         self.prev_reward = 0
@@ -160,24 +161,25 @@
                 policy_loss = -torch.min(surr1, surr2).mean()
 
                 value_loss = (return_ - self.value_net(state)).pow(2).mean()
                 self.value_optimizer.zero_grad()
                 value_loss.backward()
                 self.value_optimizer.step()
 
-    def predict_action(self, state):
+    def select_action(self, state):
         """
-        Predicts an action based on the given state and the current policy.
+        Selects an action based on the given state and the current policy.
 
-        :param state: The state to use for predicting an action.
+        :param state: The state to use for selecting an action.
         :type state: numpy.ndarray
-        :return: The predicted action and its corresponding probability distribution.
+        :return: The selected action and its corresponding probability distribution.
         :rtype: tuple(torch.Tensor, torch.distributions.Categorical)
         """
 
+        state = self._check_state(self.state)
         state_tensor = torch.tensor(state, dtype=torch.float32)
         with torch.no_grad():
             action_probs = self.policy_net(state_tensor)
         dist = Categorical(action_probs)
         action = dist.sample()
         return action, dist
 
@@ -189,32 +191,50 @@
         :type state: numpy.ndarray
         :param timestep: The current timestep of the training process.
         :type timestep: int
         :return: The action taken, the resulting reward, and whether the episode is done or not.
         :rtype: tuple(torch.Tensor, float, bool)
         """
 
-        state_num = len(state)
-        if state_num == 1:
-            state = state  # Unpack the tuple
-        elif state_num == 2:
-            state, _ = state  # Unpack the tuple
-        # state_tensor = torch.tensor(state, dtype=torch.float32)
-        action, dist = self.predict_action(state)
-        # dist = Categorical(self.policy_net(state_tensor))
-        # action = dist.sample()
+        action, dist = self.select_action(state)
+
+        return self.update_step(state, dist, action, timestep)
+
+    def update_step(self, state, dist, action, timestep):
+        """
+        Takes a step in the environment with a given action and updates the PPO algorithm with the resulting state, reward, and action.
+
+        :param state: The current state of the environment.
+        :type state: numpy.ndarray
+        :param dist: The corresponding probability distribution.
+        :type dist: torch.distributions.Categorical
+        :param action: The action taken by the agent.
+        :type action: int
+        :param reaction: The reaction of the opponent after the agent's action.
+        :type reaction: tuple
+        :param timestep: The current timestep of the training process.
+        :type timestep: int
+        :return: The resulting reward and whether the episode is done or not.
+        :rtype: tuple(float, bool)
+        """
 
         step_output = self.env.step(action.item())
         step_output_num = len(step_output)
 
         if step_output_num == 4:
             next_state, reward, is_done, _ = self.env.step(action.item())
         elif step_output_num == 5:
             next_state, reward, is_done, _, _ = self.env.step(action.item())
 
+        self.episode_reward += reward
+        self.total_reward += reward
+        self.prev_reward = reward
+
+        state = self._check_state(state)
+
         self.states.append(state)
         self.actions.append(action)
         self.rewards.append(reward)
         self.next_states.append(next_state)
         self.done.append(is_done)
         self.log_probs.append(dist.log_prob(action))
 
@@ -228,15 +248,14 @@
 
         return action, reward, is_done
 
     def update(self):
         """
         Perform an update of the PPO algorithm, using the stored information about the environment from the previous learning iterations.
         """
-
         states_tensor = torch.tensor(np.array(self.states, dtype=np.float32))
         actions_tensor = torch.tensor(np.array(self.actions))
         rewards_tensor = torch.tensor(np.array(self.rewards, dtype=np.float32))
         next_states_tensor = torch.tensor(
             np.array(self.next_states, dtype=np.float32))
         done_tensor = torch.tensor(np.array(self.done, dtype=np.float32))
         log_probs_tensor = torch.stack(self.log_probs)
@@ -274,27 +293,28 @@
             for episode in range(self.max_episodes):
                 self.reset()
                 self.learn_reset()
                 reward = 0
 
                 for t in range(self.max_timesteps):
                     _, reward, is_done = self.learn_step(self.state, timestep)
-                    self.episode_reward += reward
                     if is_done:
                         break
 
                 self.total_reward += self.episode_reward
 
                 avg_reward = self.total_reward / (episode + 1)
-                print(
-                    f'Episode: {episode}, Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Reward: {avg_reward}')
+                if self.reward_print:
+                    print(
+                        f'Episode: {episode}, Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Reward: {avg_reward}')
 
                 if avg_reward >= self.early_stop_threshold > 0:
-                    print(
-                        f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {episode}')
+                    if self.reward_print:
+                        print(
+                            f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {episode}')
                     break
                 if is_done and self.done_loop_end:
                     break
 
                 if episode + 1 >= self.max_episodes:
                     break
 
@@ -316,28 +336,26 @@
 
     def learn_reset(self):
         """
         Reset the agent's state and episode reward.
         """
 
         self.state = self.env.reset()
-        self.episode_reward = 0
+
+        return self._check_state(self.state)
 
     def learn_next(self):
         """
         Perform a single learning step and update the episode and total rewards.
 
         :return: The action taken, the resulting reward, and whether the episode is done or not.
         :rtype: tuple(torch.Tensor, float, bool)
         """
 
         action, reward, is_done = self.learn_step(self.state, -1)
-        self.episode_reward += reward
-        self.total_reward += reward
-        self.prev_reward = reward
 
         return action, reward, is_done
 
     def learn_close(self):
         """
         Close the environment and reset the agent's total reward, episode count, and episode reward.
         """
@@ -349,16 +367,23 @@
 
     def learn_check(self):
         """
         Print the episode count, previous reward, episode reward, total reward, and average episode reward.
         """
 
         avg_reward = self.total_reward / (self.episode + 1)
-        print(
-            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
+        if self.reward_print:
+            print(
+                f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
+
+    def _check_state(self, state):
+        state_num = len(state)
+        if state_num == 2:
+            state, _ = state  # Unpack the tuple
+        return state
 
     def save(self, file_name):
         """
         Initialize the AgentPPO class with the specified environment and settings.
 
         :param env: The environment to use for training.
         :type env: gym.Env or None
```

### Comparing `modular_rl-0.1.0.dev0/modular_rl/networks.py` & `modular_rl-0.1.1.dev0/modular_rl/networks.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.0.dev0/modular_rl/settings.py` & `modular_rl-0.1.1.dev0/modular_rl/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         'optimizer_speed': 3e-4,  # Learning rate for the optimizer
         'gamma': 0.99,  # Discount factor
         'lam': 0.95,  # Lambda parameter for GAE
         'clip_param': 0.2,  # Clipping parameter for PPO
         # If the average reward is greater than or equal to this value, training is stopped early
         'early_stop_threshold': -1,
         'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,
     }
 
     default_modular = {
         # Maximum number of episodes for training (-1 for no limit)
         'max_episodes': -1,
         # Maximum number of timesteps for each episode (-1 for no limit)
         'max_timesteps': -1,
@@ -43,8 +44,9 @@
         'networks': 'medium',  # Size of the hidden layer in neural networks
         'optimizer_speed': 3e-4,  # Learning rate for the optimizer
         'gamma': 0.99,  # Discount factor
         'lam': 0.95,  # Lambda parameter for GAE
         'clip_param': 0.2,  # Clipping parameter for PPO
         # If the average reward is greater than or equal to this value, training is stopped early
         'early_stop_threshold': -1,
+        'reward_print': True,
     }
```

### Comparing `modular_rl-0.1.0.dev0/modular_rl/tester.py` & `modular_rl-0.1.1.dev0/modular_rl/tester.py`

 * *Files 27% similar despite different names*

```diff
@@ -39,23 +39,34 @@
     env.learn_next()
     env.learn_check()
     env.learn_next()
     env.learn_check()
     env.update()
 
     env.reset()
-    env.learn_reset()
-    env.learn_next()
-    env.learn_next()
-    env.learn_next()
-    env.learn_next()
-    env.learn_next()
+    manual_step(env)
     env.learn_check()
-    env.learn_next()
-    env.learn_next()
-    env.learn_next()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
+    env.learn_check()
+    manual_step(env)
     env.learn_check()
     env.update()
 
     env.learn_close()
 
     # env.save_model('test.pth')
+
+
+def manual_step(env):
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+    env.update_step(initial_state, dist, action, -1)
```

### Comparing `modular_rl-0.1.0.dev0/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.1.1.dev0/modular_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.1.0.dev0
+Version: 0.1.1.dev0
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ModularRL
-=======
 
 ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. 
 The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 
 ## Installation
 
 ```powershell
```

### Comparing `modular_rl-0.1.0.dev0/pyproject.toml` & `modular_rl-0.1.1.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.1.0.dev"
+version = "0.1.1.dev"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.1.0.dev0/setup.py` & `modular_rl-0.1.1.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.1.0.dev',
+    version='0.1.1.dev',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

