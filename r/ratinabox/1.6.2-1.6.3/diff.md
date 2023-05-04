# Comparing `tmp/ratinabox-1.6.2.tar.gz` & `tmp/ratinabox-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.6.2.tar", last modified: Thu May  4 11:11:24 2023, max compression
+gzip compressed data, was "ratinabox-1.6.3.tar", last modified: Thu May  4 12:25:12 2023, max compression
```

## Comparing `ratinabox-1.6.2.tar` & `ratinabox-1.6.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.214889 ratinabox-1.6.2/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.2/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 11:11:24.215029 ratinabox-1.6.2/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.2/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.2/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.203653 ratinabox-1.6.2/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    43232 2023-05-04 11:09:31.000000 ratinabox-1.6.2/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.6.2/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    83295 2023-05-04 11:08:29.000000 ratinabox-1.6.2/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.2/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3874 2023-04-27 09:08:29.000000 ratinabox-1.6.2/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.206776 ratinabox-1.6.2/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.2/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.2/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.2/ratinabox/contribs/SuccessorFeatures.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.2/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.2/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.208776 ratinabox-1.6.2/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.2/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.2/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.2/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.2/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.2/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34484 2023-05-03 14:00:43.000000 ratinabox-1.6.2/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.204683 ratinabox-1.6.2/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-05-04 11:11:24.215392 ratinabox-1.6.2/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.2/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.214709 ratinabox-1.6.2/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.2/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.2/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.2/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.2/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.861111 ratinabox-1.6.3/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.3/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 12:25:12.861244 ratinabox-1.6.3/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.3/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.3/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.854160 ratinabox-1.6.3/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    43226 2023-05-04 11:27:59.000000 ratinabox-1.6.3/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.6.3/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    83295 2023-05-04 11:28:06.000000 ratinabox-1.6.3/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.3/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3874 2023-04-27 09:08:29.000000 ratinabox-1.6.3/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.856412 ratinabox-1.6.3/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.3/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.3/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.3/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.3/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.3/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.3/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.857519 ratinabox-1.6.3/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.3/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.3/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.3/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.3/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.3/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34484 2023-05-03 14:00:43.000000 ratinabox-1.6.3/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.854950 ratinabox-1.6.3/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-05-04 12:25:12.000000 ratinabox-1.6.3/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-05-04 12:25:12.861568 ratinabox-1.6.3/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.3/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 12:25:12.860995 ratinabox-1.6.3/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.3/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.3/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.3/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.3/tests/test_neurons.py
```

### Comparing `ratinabox-1.6.2/LICENSE` & `ratinabox-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/PKG-INFO` & `ratinabox-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.2
+Version: 1.6.3
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.6.2/README.md` & `ratinabox-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/Agent.py` & `ratinabox-1.6.3/ratinabox/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,33 +559,31 @@
                 self.positions = positions
                 self.times = times
                 self.imported_trajectory_id = 0
 
         return
 
     def get_history_slice(self, t_start=None, t_end=None, framerate=None):
-        """ "
+        """
         Returns a python slice() object which can be used to get a slice of history lists between t_start and t_end with framerate. Use case:
         >>> slice = get_history_slice(0,10*60,20)
         >>> t = self.history['t'][slice]
         >>> pos = self.history['pos'][slice]
         t and pos are now lists of times and positions between t_start=0 and t_end=10*60 at 20 frames per second
 
         Args:
             • t_start: start time in seconds (default = self.history['t'][0])
             • t_end: end time in seconds (default = self.history["t"][-1])
             • framerate: frames per second (default = None --> step=0 so, just whatever the data frequency (1/Ag.dt) is)
         """
 
         t = np.array(self.history["t"])
-        if t_start is None:
-            t_start = t[0]
+        t_start = (t_start or t[0])
         startid = np.nanargmin(np.abs(t - (t_start)))
-        if t_end is None:
-            t_end = t[-1]
+        t_end = (t_end or t[-1])
         endid = np.nanargmin(np.abs(t - (t_end)))
         if framerate is None:
             skiprate = 1
         else:
             skiprate = max(1, int((1 / framerate) / self.dt))
 
         return slice(startid, endid, skiprate)
@@ -637,15 +635,16 @@
             agent_list = [self]
             if color is None:
                 color = "#7b699a"
         else:
             agent_list = self.Environment.Agents
         replot_env = True
         for i, self_ in enumerate(agent_list):
-            t_end is t_end or self_.history["t"][-1]
+            t_end = t_end or self_.history["t"][-1]
+            print("t_end:", t_end)
             slice = self_.get_history_slice(
                 t_start=t_start, t_end=t_end, framerate=framerate
             )
             time = np.array(self_.history["t"])[slice]
             trajectory = np.array(self_.history["pos"])[slice]
             if color is None:
                 color_list = [f"C{i}"] * len(time)
```

### Comparing `ratinabox-1.6.2/ratinabox/Environment.py` & `ratinabox-1.6.3/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/Neurons.py` & `ratinabox-1.6.3/ratinabox/Neurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/README.md` & `ratinabox-1.6.3/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/__init__.py` & `ratinabox-1.6.3/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.6.3/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.6.3/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.6.3/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/README.md` & `ratinabox-1.6.3/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.6.3/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/SuccessorFeatures.py` & `ratinabox-1.6.3/ratinabox/contribs/SuccessorFeatures.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.6.3/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.6.3/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/data/README.md` & `ratinabox-1.6.3/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/data/rat.png` & `ratinabox-1.6.3/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/data/sargolini.npz` & `ratinabox-1.6.3/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/data/tanni.npz` & `ratinabox-1.6.3/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox/utils.py` & `ratinabox-1.6.3/ratinabox/utils.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.6.3/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.2
+Version: 1.6.3
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.6.2/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.6.3/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/setup.cfg` & `ratinabox-1.6.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.6.2
+version = 1.6.3
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.6.2/tests/test_advanced.py` & `ratinabox-1.6.3/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.2/tests/test_environment.py` & `ratinabox-1.6.3/tests/test_environment.py`

 * *Files identical despite different names*

