# Comparing `tmp/modular_rl-0.1.1.dev0.tar.gz` & `tmp/modular_rl-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.1.1.dev0.tar", last modified: Thu May  4 10:19:00 2023, max compression
+gzip compressed data, was "modular_rl-0.1.2.dev0.tar", last modified: Thu May  4 12:25:42 2023, max compression
```

## Comparing `modular_rl-0.1.1.dev0.tar` & `modular_rl-0.1.2.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.748791 modular_rl-0.1.1.dev0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.1.dev0/LICENSE
--rw-rw-rw-   0        0        0     3477 2023-05-04 10:19:00.747342 modular_rl-0.1.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2099 2023-05-04 06:34:40.000000 modular_rl-0.1.1.dev0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.729224 modular_rl-0.1.1.dev0/modular_rl/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.743354 modular_rl-0.1.1.dev0/modular_rl/agents/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    17011 2023-05-04 10:15:10.000000 modular_rl-0.1.1.dev0/modular_rl/agents/agent_ppo.py
--rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.1.dev0/modular_rl/networks.py
--rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.1.dev0/modular_rl/settings.py
--rw-rw-rw-   0        0        0     2073 2023-05-04 09:57:12.000000 modular_rl-0.1.1.dev0/modular_rl/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.739282 modular_rl-0.1.1.dev0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     3477 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 10:19:00.000000 modular_rl-0.1.1.dev0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1425 2023-05-04 10:18:38.000000 modular_rl-0.1.1.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 10:19:00.748791 modular_rl-0.1.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-05-04 10:18:45.000000 modular_rl-0.1.1.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:00.746157 modular_rl-0.1.1.dev0/tests/
--rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.1.dev0/tests/test.py
--rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.1.dev0/tests/test_modular.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.706752 modular_rl-0.1.2.dev0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0     3622 2023-05-04 12:25:42.705753 modular_rl-0.1.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2244 2023-05-04 10:23:00.000000 modular_rl-0.1.2.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.687035 modular_rl-0.1.2.dev0/modular_rl/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.700076 modular_rl-0.1.2.dev0/modular_rl/agents/
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0    17011 2023-05-04 10:15:10.000000 modular_rl-0.1.2.dev0/modular_rl/agents/agent_ppo.py
+-rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.2.dev0/modular_rl/networks.py
+-rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.2.dev0/modular_rl/settings.py
+-rw-rw-rw-   0        0        0     2073 2023-05-04 09:57:12.000000 modular_rl-0.1.2.dev0/modular_rl/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.697076 modular_rl-0.1.2.dev0/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     3622 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 12:25:42.000000 modular_rl-0.1.2.dev0/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1425 2023-05-04 12:25:23.000000 modular_rl-0.1.2.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 12:25:42.706752 modular_rl-0.1.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-05-04 12:25:17.000000 modular_rl-0.1.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:25:42.703723 modular_rl-0.1.2.dev0/tests/
+-rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.2.dev0/tests/test.py
+-rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.2.dev0/tests/test_modular.py
```

### Comparing `modular_rl-0.1.1.dev0/LICENSE` & `modular_rl-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.1.dev0/PKG-INFO` & `modular_rl-0.1.2.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.1.1.dev0
+Version: 0.1.2.dev0
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -76,15 +76,20 @@
     env.learn_reset()
     action, reward, is_done = env.learn_next()
     env.learn_check()
     env.update()
 
     env.reset()
     env.learn_reset()
-    action, reward, is_done = env.learn_next()
+
+    # Proceed with the learning manually.
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+    env.update_step(initial_state, dist, action, -1)
+
     env.learn_check()
     env.update()
 
     env.learn_close()
 
 
 init_modular()
```

### Comparing `modular_rl-0.1.1.dev0/README.md` & `modular_rl-0.1.2.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,20 @@
     env.learn_reset()
     action, reward, is_done = env.learn_next()
     env.learn_check()
     env.update()
 
     env.reset()
     env.learn_reset()
-    action, reward, is_done = env.learn_next()
+
+    # Proceed with the learning manually.
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+    env.update_step(initial_state, dist, action, -1)
+
     env.learn_check()
     env.update()
 
     env.learn_close()
 
 
 init_modular()
```

### Comparing `modular_rl-0.1.1.dev0/modular_rl/agents/agent_ppo.py` & `modular_rl-0.1.2.dev0/modular_rl/agents/agent_ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.1.dev0/modular_rl/networks.py` & `modular_rl-0.1.2.dev0/modular_rl/networks.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.1.dev0/modular_rl/settings.py` & `modular_rl-0.1.2.dev0/modular_rl/settings.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.1.dev0/modular_rl/tester.py` & `modular_rl-0.1.2.dev0/modular_rl/tester.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.1.dev0/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.1.2.dev0/modular_rl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.1.1.dev0
+Version: 0.1.2.dev0
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments.
 Home-page: https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -76,15 +76,20 @@
     env.learn_reset()
     action, reward, is_done = env.learn_next()
     env.learn_check()
     env.update()
 
     env.reset()
     env.learn_reset()
-    action, reward, is_done = env.learn_next()
+
+    # Proceed with the learning manually.
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+    env.update_step(initial_state, dist, action, -1)
+
     env.learn_check()
     env.update()
 
     env.learn_close()
 
 
 init_modular()
```

### Comparing `modular_rl-0.1.1.dev0/pyproject.toml` & `modular_rl-0.1.2.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.1.1.dev"
+version = "0.1.2.dev"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.1.1.dev0/setup.py` & `modular_rl-0.1.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.1.1.dev',
+    version='0.1.2.dev',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

