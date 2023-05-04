# Comparing `tmp/ratinabox-1.6.1.tar.gz` & `tmp/ratinabox-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.6.1.tar", last modified: Tue Apr 25 13:21:58 2023, max compression
+gzip compressed data, was "ratinabox-1.6.2.tar", last modified: Thu May  4 11:11:24 2023, max compression
```

## Comparing `ratinabox-1.6.1.tar` & `ratinabox-1.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.286319 ratinabox-1.6.1/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.1/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-04-25 13:21:58.286433 ratinabox-1.6.1/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.1/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.1/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.269757 ratinabox-1.6.1/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    42379 2023-04-24 16:38:06.000000 ratinabox-1.6.1/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    32365 2023-04-25 13:14:08.000000 ratinabox-1.6.1/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    82493 2023-04-25 10:36:34.000000 ratinabox-1.6.1/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.1/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.6.1/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.276147 ratinabox-1.6.1/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.1/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.1/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.1/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.1/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.1/ratinabox/contribs/SuccessorFeatures.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.1/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.1/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.1/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.280090 ratinabox-1.6.1/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.1/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.1/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.1/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.1/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.1/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34247 2023-04-23 10:24:42.000000 ratinabox-1.6.1/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.272788 ratinabox-1.6.1/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-04-25 13:21:58.000000 ratinabox-1.6.1/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-04-25 13:21:58.000000 ratinabox-1.6.1/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-25 13:21:58.000000 ratinabox-1.6.1/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-25 13:21:58.000000 ratinabox-1.6.1/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-25 13:21:58.000000 ratinabox-1.6.1/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-25 13:21:58.286759 ratinabox-1.6.1/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.1/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 13:21:58.286200 ratinabox-1.6.1/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.1/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.1/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.1/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.1/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.214889 ratinabox-1.6.2/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.2/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 11:11:24.215029 ratinabox-1.6.2/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.2/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.2/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.203653 ratinabox-1.6.2/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    43232 2023-05-04 11:09:31.000000 ratinabox-1.6.2/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.6.2/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    83295 2023-05-04 11:08:29.000000 ratinabox-1.6.2/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.2/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3874 2023-04-27 09:08:29.000000 ratinabox-1.6.2/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.206776 ratinabox-1.6.2/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.2/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.2/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.2/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.2/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.2/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.2/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.208776 ratinabox-1.6.2/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.2/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.2/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.2/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.2/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.2/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34484 2023-05-03 14:00:43.000000 ratinabox-1.6.2/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.204683 ratinabox-1.6.2/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-05-04 11:11:24.000000 ratinabox-1.6.2/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-05-04 11:11:24.215392 ratinabox-1.6.2/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.2/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-05-04 11:11:24.214709 ratinabox-1.6.2/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.2/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.2/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.2/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.2/tests/test_neurons.py
```

### Comparing `ratinabox-1.6.1/LICENSE` & `ratinabox-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/PKG-INFO` & `ratinabox-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.1
+Version: 1.6.2
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.6.1/README.md` & `ratinabox-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/Agent.py` & `ratinabox-1.6.2/ratinabox/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 Other plotting functions are available."""
             )
         return
 
     @classmethod
     def get_all_default_params(cls, verbose=False):
         """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
-        all_default_params = utils.collect_all_default_params(cls)
+        all_default_params = utils.collect_all_params(cls, dict_name="default_params")
         if verbose:
             pprint.pprint(all_default_params)
         return all_default_params
 
     def update(self, dt=None, drift_velocity=None, drift_to_random_strength_ratio=1):
         """Movement policy update.
         In principle this does a very simple thing:
@@ -558,14 +558,42 @@
             else:
                 self.positions = positions
                 self.times = times
                 self.imported_trajectory_id = 0
 
         return
 
+    def get_history_slice(self, t_start=None, t_end=None, framerate=None):
+        """ "
+        Returns a python slice() object which can be used to get a slice of history lists between t_start and t_end with framerate. Use case:
+        >>> slice = get_history_slice(0,10*60,20)
+        >>> t = self.history['t'][slice]
+        >>> pos = self.history['pos'][slice]
+        t and pos are now lists of times and positions between t_start=0 and t_end=10*60 at 20 frames per second
+
+        Args:
+            • t_start: start time in seconds (default = self.history['t'][0])
+            • t_end: end time in seconds (default = self.history["t"][-1])
+            • framerate: frames per second (default = None --> step=0 so, just whatever the data frequency (1/Ag.dt) is)
+        """
+
+        t = np.array(self.history["t"])
+        if t_start is None:
+            t_start = t[0]
+        startid = np.nanargmin(np.abs(t - (t_start)))
+        if t_end is None:
+            t_end = t[-1]
+        endid = np.nanargmin(np.abs(t - (t_end)))
+        if framerate is None:
+            skiprate = 1
+        else:
+            skiprate = max(1, int((1 / framerate) / self.dt))
+
+        return slice(startid, endid, skiprate)
+
     def plot_trajectory(
         self,
         t_start=0,
         t_end=None,
         framerate=10,
         fig=None,
         ax=None,
@@ -585,15 +613,15 @@
         """Plots the trajectory between t_start (seconds) and t_end (defaulting to the last time available)
         Args:
             • t_start: start time in seconds
             • t_end: end time in seconds (default = self.history["t"][-1])
             • framerate: how many scatter points / per second of motion to display
             • fig, ax: the fig, ax to plot on top of, optional, if not provided used self.Environment.plot_Environment().
               This can be used to plot trajectory on top of receptive fields etc.
-            • plot_all_agents: if True, this will plot the trajectory of all agents in the list Environment.Agents
+            • plot_all_agents: if True, this will plot the trajectory of all agents in the list self.Environment.Agents
             • point_size: size of scatter points
             • decay_point_size: decay trajectory point size over time (recent times = largest)
             • decay_point_timescale: if decay_point_size is True, this is the timescale over which sizes decay
             • plot_agent: dedicated point show agent current position
             • color: plot point color, if color == 'changing' will smoothly change trajectory color from start to finish
             • alpha: plot point opaqness
             • xlim: In 1D, forces the xlim to be a certain time (minutes) (useful if animating this function)
@@ -609,27 +637,20 @@
             agent_list = [self]
             if color is None:
                 color = "#7b699a"
         else:
             agent_list = self.Environment.Agents
         replot_env = True
         for i, self_ in enumerate(agent_list):
-            dt = self_.dt
-            t, pos = np.array(self_.history["t"]), np.array(self_.history["pos"])
-            if t_end == None:
-                t_end = t[-1]
-            startid = np.nanargmin(np.abs(t - (t_start)))
-            endid = np.nanargmin(np.abs(t - (t_end)))
-            if self_.Environment.dimensionality == "2D":
-                skiprate = max(1, int((1 / framerate) / dt))
-                trajectory = pos[startid:endid, :][::skiprate]
-            if self_.Environment.dimensionality == "1D":
-                skiprate = max(1, int((1 / framerate) / dt))
-                trajectory = pos[startid:endid][::skiprate]
-            time = t[startid:endid][::skiprate]
+            t_end is t_end or self_.history["t"][-1]
+            slice = self_.get_history_slice(
+                t_start=t_start, t_end=t_end, framerate=framerate
+            )
+            time = np.array(self_.history["t"])[slice]
+            trajectory = np.array(self_.history["pos"])[slice]
             if color is None:
                 color_list = [f"C{i}"] * len(time)
             elif color == "changing":
                 trajectory_cmap = matplotlib.colormaps["viridis_r"]
                 color_list = [trajectory_cmap(t / len(time)) for t in range(len(time))]
                 decay_point_size = (
                     False  # if changing colour, may as well show WHOLE trajectory
```

### Comparing `ratinabox-1.6.1/ratinabox/Environment.py` & `ratinabox-1.6.2/ratinabox/Environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             )
 
         return
 
     @classmethod
     def get_all_default_params(cls, verbose=False):
         """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
-        all_default_params = utils.collect_all_default_params(cls)
+        all_default_params = utils.collect_all_params(cls, dict_name="default_params")
         if verbose:
             pprint.pprint(all_default_params)
         return all_default_params
 
     def add_wall(self, wall):
         """Add a wall to the (2D) environment.
         Extends self.walls array to include one new wall.
@@ -226,15 +226,21 @@
             autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
         Returns:
             fig, ax: the environment figures, can be used for further downstream plotting.
         """
 
         if self.dimensionality == "1D":
             extent = self.extent
-            fig, ax = plt.subplots(figsize=(2 * (extent[1] - extent[0]), (5.5 / 25)))
+            if fig is None and ax is None:
+                fig, ax = plt.subplots(
+                    figsize=(
+                        ratinabox.MOUNTAIN_PLOT_WIDTH_MM / 25 * (extent[1] - extent[0]),
+                        1,
+                    )
+                )
             ax.set_xlim(left=extent[0], right=extent[1])
             ax.spines["left"].set_color("none")
             ax.spines["right"].set_color("none")
             ax.spines["bottom"].set_position("zero")
             ax.spines["top"].set_color("none")
             ax.set_yticks([])
             ax.set_xticks([extent[0], extent[1]])
```

### Comparing `ratinabox-1.6.1/ratinabox/Neurons.py` & `ratinabox-1.6.2/ratinabox/Neurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,29 +110,28 @@
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
         self.firingrate = np.zeros(self.n)
         self.noise = np.zeros(self.n)
-
         self.history = {}
         self.history["t"] = []
         self.history["firingrate"] = []
         self.history["spikes"] = []
 
         if ratinabox.verbose is True:
             print(
                 f"\nA Neurons() class has been initialised with parameters f{self.params}. Use Neurons.update() to update the firing rate of the Neurons to correspond with the Agent.Firing rates and spikes are saved into the Agent.history dictionary. Plot a timeseries of the rate using Neurons.plot_rate_timeseries(). Plot a rate map of the Neurons using Neurons.plot_rate_map()."
             )
 
     @classmethod
     def get_all_default_params(cls, verbose=False):
         """Returns a dictionary of all the default parameters of the class, including those inherited from its parents."""
-        all_default_params = utils.collect_all_default_params(cls)
+        all_default_params = utils.collect_all_params(cls, dict_name="default_params")
         if verbose:
             pprint.pprint(all_default_params)
         return all_default_params
 
     def update(self):
         # update noise vector
         dnoise = utils.ornstein_uhlenbeck(
@@ -153,15 +152,15 @@
         self.firingrate = self.firingrate + self.noise
         if self.save_history is True:
             self.save_to_history()
         return
 
     def plot_rate_timeseries(
         self,
-        t_start=None,
+        t_start=0,
         t_end=None,
         chosen_neurons="all",
         spikes=False,
         imshow=False,
         fig=None,
         ax=None,
         xlim=None,
@@ -175,45 +174,41 @@
         Args:
             • t_start (int, optional): _description_. Defaults to start of data, probably 0.
             • t_end (int, optional): _description_. Defaults to end of data.
             • chosen_neurons: Which neurons to plot. string "10" or 10 will plot ten of them, "all" will plot all of them, "12rand" will plot 12 random ones. A list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "all".
             chosen_neurons (str, optional): Which neurons to plot. string "10" will plot 10 of them, "all" will plot all of them, a list like [1,4,5] will plot cells indexed 1, 4 and 5. Defaults to "10".
             • spikes (bool, optional): If True, scatters exact spike times underneath each curve of firing rate. Defaults to True.
             the below params I just added for help with animations
-            • imshow - if True will not dispaly as mountain plot but as an image (plt.imshow)
+            • imshow - if True will not dispaly as mountain plot but as an image (plt.imshow). Thee "extent" will be (t_start, t_end, 0, 1) in case you want to plot on top of this
             • fig, ax: the figure, axis to plot on (can be None)
             xlim: fix xlim of plot irrespective of how much time you're plotting
             • color: color of the line, if None, defaults to cell class default (probalby "C1")
             • background_color: color of the background if not matplotlib default (probably white)
             • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             • kwargs sent to mountain plot function, you can ignore these
 
         Returns:
             fig, ax
         """
         t = np.array(self.history["t"])
-        # times to plot
-        if t_start is None:
-            t_start = t[0]
-        if t_end is None:
-            t_end = t[-1]
-        startid = np.argmin(np.abs(t - (t_start)))
-        endid = np.argmin(np.abs(t - (t_end)))
-        rate_timeseries = np.array(self.history["firingrate"][startid:endid])
-        spike_data = np.array(self.history["spikes"][startid:endid])
-        t = t[startid:endid]
+        t_end = t_end or t[-1]
+        slice = self.Agent.get_history_slice(t_start, t_end)
+        rate_timeseries = np.array(self.history["firingrate"][slice])
+        spike_data = np.array(self.history["spikes"][slice])
+        t = t[slice]
 
         # neurons to plot
         chosen_neurons = self.return_list_of_neurons(chosen_neurons)
         n_neurons_to_plot = len(chosen_neurons)
-        if ("shift" not in kwargs.keys()) and ("overlap" not in kwargs.keys()):
-            kwargs["shift"] = 2
-            kwargs["overlap"] = 2.2
-        spike_data = spike_data[startid:endid, chosen_neurons]
+        spike_data = spike_data[slice, chosen_neurons]
         rate_timeseries = rate_timeseries[:, chosen_neurons]
+
+        was_fig, was_ax = (fig is None), (
+            ax is None
+        )  # remember whether a fig or ax was provided as xlims depend on this
         if color is None:
             color = self.color
         if imshow == False:
             firingrates = rate_timeseries.T
             fig, ax = utils.mountain_plot(
                 X=t / 60,
                 NbyX=firingrates,
@@ -235,16 +230,16 @@
                         h,
                         color=(self.color or "C1"),
                         alpha=0.5,
                         s=5,
                         linewidth=0,
                     )
 
-            xmin = min(t_start / 60, ax.get_xlim()[0])
-            xmax = max(t_end / 60, ax.get_xlim()[1])
+            xmin = t_start / 60 if was_fig else min(t_start / 60, ax.get_xlim()[0])
+            xmax = t_end / 60 if was_fig else max(t_end / 60, ax.get_xlim()[1])
             ax.set_xlim(
                 left=xmin,
                 right=xmax,
             )
             ax.set_xticks([xmin, xmax])
             ax.set_xticklabels([round(xmin, 2), round(xmax, 2)])
             if xlim is not None:
@@ -254,22 +249,32 @@
 
             if background_color is not None:
                 ax.set_facecolor(background_color)
                 fig.patch.set_facecolor(background_color)
 
         elif imshow == True:
             if fig is None and ax is None:
-                fig, ax = plt.subplots(figsize=(8, 4))
+                fig, ax = plt.subplots(
+                    figsize=(
+                        ratinabox.MOUNTAIN_PLOT_WIDTH_MM / 25,
+                        0.5 * ratinabox.MOUNTAIN_PLOT_WIDTH_MM / 25,
+                    )
+                )
             data = rate_timeseries.T
-            ax.imshow(data[::-1], aspect=0.3 * data.shape[1] / data.shape[0])
+            ax.imshow(
+                data[::-1],
+                aspect="auto",
+                # aspect=0.5 * data.shape[1] / data.shape[0],
+                extent=(t_start, t_end, 0, 1),
+            )
             ax.spines["top"].set_visible(False)
             ax.spines["right"].set_visible(False)
             ax.spines["left"].set_visible(False)
             ax.set_xlabel("Time / min")
-            ax.set_xticks([0 - 0.5, len(t) + 0.5])
+            ax.set_xticks([t_start, t_end])
             ax.set_xticklabels([round(t_start / 60, 2), round(t_end / 60, 2)])
             ax.set_yticks([])
             ax.set_ylabel("Neurons")
 
         ratinabox.utils.save_figure(fig, self.name + "_firingrate", save=autosave)
         return fig, ax
 
@@ -325,35 +330,35 @@
             # times to plot
             if len(t) == 0:
                 print(
                     "Can't plot rate map by method='history' since there is no available data to plot. "
                 )
                 return
             t_end = t_end or t[-1]
-            startid = np.argmin(np.abs(t - (t_start)))
-            endid = np.argmin(np.abs(t - (t_end)))
-            pos = np.array(self.Agent.history["pos"])[startid:endid]
-            t = t[startid:endid]
+            slice = self.Agent.get_history_slice(t_start, t_end)
+            pos = np.array(self.Agent.history["pos"])[slice]
+            t = t[slice]
 
             if method == "history":
-                rate_timeseries = np.array(self.history["firingrate"])[startid:endid].T
+                rate_timeseries = np.array(self.history["firingrate"])[slice].T
                 if len(rate_timeseries) == 0:
                     print("No historical data with which to calculate ratemap.")
             if spikes == True:
-                spike_data = np.array(self.history["spikes"])[startid:endid].T
+                spike_data = np.array(self.history["spikes"])[slice].T
                 if len(spike_data) == 0:
                     print("No historical data with which to plot spikes.")
 
         if self.color == None:
             coloralpha = None
         else:
             coloralpha = list(matplotlib.colors.to_rgba(self.color))
             coloralpha[-1] = 0.5
 
         chosen_neurons = self.return_list_of_neurons(chosen_neurons=chosen_neurons)
+        N_neurons = len(chosen_neurons)
 
         # PLOT 2D
         if self.Agent.Environment.dimensionality == "2D":
             from mpl_toolkits.axes_grid1 import ImageGrid
 
             if fig is None and ax is None:
                 if shape is None:
@@ -471,22 +476,25 @@
                         norm_by_bincount=True,
                     )
                     x, rate_map = utils.interpolate_and_smooth(x, rate_map, sigma=0.03)
                     rate_maps.append(rate_map)
                 rate_maps = np.array(rate_maps)
 
             if fig is None and ax is None:
+                fig, ax = plt.subplots(
+                    figsize=(
+                        ratinabox.MOUNTAIN_PLOT_WIDTH_MM / 25,
+                        N_neurons * ratinabox.MOUNTAIN_PLOT_SHIFT_MM / 25,
+                    )
+                )
                 fig, ax = self.Agent.Environment.plot_environment(
-                    autosave=False,
+                    autosave=False, fig=fig, ax=ax
                 )
 
             if method != "neither":
-                if ("shift" not in kwargs.keys()) and ("overlap" not in kwargs.keys()):
-                    kwargs["shift"] = 2
-                    kwargs["overlap"] = 2.2
                 fig, ax = utils.mountain_plot(
                     X=x, NbyX=rate_maps, color=self.color, fig=fig, ax=ax, **kwargs
                 )
 
             if spikes is True:
                 for i in range(len(chosen_neurons)):
                     pos_ = pos[:, 0]
@@ -685,28 +693,38 @@
         """
 
         self.Agent = Agent
 
         self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
-        super().__init__(Agent, self.params)
-
-        if self.place_cell_centres is None:
-            self.place_cell_centres = self.Agent.Environment.sample_positions(
-                n=self.n, method="uniform_jitter"
+        if self.params["place_cell_centres"] is None:
+            self.params["place_cell_centres"] = self.Agent.Environment.sample_positions(
+                n=self.params["n"], method="uniform_jitter"
             )
-        elif type(self.place_cell_centres) is str:
-            if self.place_cell_centres in ["random", "uniform", "uniform_jitter"]:
-                self.place_cell_centres = self.Agent.Environment.sample_positions(
-                    n=self.n, method=self.place_cell_centres
+        elif type(self.params["place_cell_centres"]) is str:
+            if self.params["place_cell_centres"] in [
+                "random",
+                "uniform",
+                "uniform_jitter",
+            ]:
+                self.params[
+                    "place_cell_centres"
+                ] = self.Agent.Environment.sample_positions(
+                    n=self.params["n"], method=self.params["place_cell_centres"]
+                )
+            else:
+                raise ValueError(
+                    "self.params['place_cell_centres'] must be None, an array of locations or one of the instructions ['random', 'uniform', 'uniform_jitter']"
                 )
         else:
-            self.n = self.place_cell_centres.shape[0]
-        self.place_cell_widths = self.widths * np.ones(self.n)
+            self.params["n"] = self.params["place_cell_centres"].shape[0]
+        self.place_cell_widths = self.params["widths"] * np.ones(self.params["n"])
+
+        super().__init__(Agent, self.params)
 
         # Assertions (some combinations of boundary condition and wall geometries aren't allowed)
         if self.Agent.Environment.dimensionality == "2D":
             if all(
                 [
                     (
                         (self.wall_geometry == "line_of_sight")
```

### Comparing `ratinabox-1.6.1/ratinabox/README.md` & `ratinabox-1.6.2/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/__init__.py` & `ratinabox-1.6.2/ratinabox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 figure_directory = "undefined"  # where to save figures, must be a director i.e. end in "/", for example "../figures/"
 
 _save_plot_warnings_on = True  # whether to warn that autosave is turned off
 _stylize_plot_warnings_on = (
     True  # whether to warn that rcParams haven't been set to make plots look good
 )
 _stylized_plots = False  # whether rcParams have been set to make plots look good
+
+MOUNTAIN_PLOT_WIDTH_MM = (
+    4 * 25
+)  # width of mountain plots (e.g rate timeseries plots and 1D ratemaps)
+MOUNTAIN_PLOT_SHIFT_MM = 2  # this is the shift between the nth mountain plot line and the (n+1)th mountain plot line
+MOUNTAIN_PLOT_OVERLAP = 2.2  # this is the max fraction the nth mountain plot line will over lap into the (n+1)th mountain plot line
+
 from .Environment import *
 from .Agent import *
 from .Neurons import *
 
 from . import contribs
 
 
@@ -91,12 +98,7 @@
             "#e97670",
             "#f6d444",
             "#9a539b",
         ],
     )
 
     ratinabox._stylized_plots = True
-
-
-# print(
-#     "RatInABox successfully imported.\n    (optional) To automatically format and save RatInABox figures \n           • set  `ratinabox.autosave_plots = True`\n           • set  `ratinabox.figure_directory = 'path/to/figures/'`\n           • call `ratinabox.stylize_plots()`",end="\n\n"
-# )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ratinabox-1.6.1/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.6.2/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.6.2/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.6.2/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/README.md` & `ratinabox-1.6.2/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.6.2/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/SuccessorFeatures.py` & `ratinabox-1.6.2/ratinabox/contribs/SuccessorFeatures.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.6.2/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.6.2/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/data/README.md` & `ratinabox-1.6.2/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/data/rat.png` & `ratinabox-1.6.2/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/data/sargolini.npz` & `ratinabox-1.6.2/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/data/tanni.npz` & `ratinabox-1.6.2/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/ratinabox/utils.py` & `ratinabox-1.6.2/ratinabox/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from datetime import datetime
 from scipy import stats as stats
 import ratinabox
 
 """OTHER USEFUL FUNCTIONS"""
 """Geometry functions"""
 
-
 def get_perpendicular(a=None):
     """Given 2-vector, a, returns its perpendicular
     Args:
         a (array, optional): 2-vector direction. Defaults to None.
     Returns:
         array: perpendicular to a
     """
@@ -436,14 +435,15 @@
         (heatmap): if 2D
     """
     if len(extent) == 2:  # dimensionality = "1D"
         bins = np.arange(extent[0], extent[1] + dx, dx)
         heatmap, xedges = np.histogram(data, bins=bins, weights=weights)
         if norm_by_bincount:
             bincount = np.histogram(data, bins=bins)[0]
+            bincount[bincount == 0] = 1
             heatmap = heatmap / bincount
         centres = (xedges[1:] + xedges[:-1]) / 2
         return (heatmap, centres)
 
     elif len(extent) == 4:  # dimensionality = "2D"
         bins_x = np.arange(extent[0], extent[1] + dx, dx)
         bins_y = np.arange(extent[2], extent[3] + dx, dx)
@@ -466,16 +466,17 @@
     color="C0",
     xlabel="",
     ylabel="",
     xlim=None,
     fig=None,
     ax=None,
     norm_by="max",
-    overlap=0.8,
-    shift=4,
+    width=ratinabox.MOUNTAIN_PLOT_WIDTH_MM,
+    overlap=ratinabox.MOUNTAIN_PLOT_OVERLAP,
+    shift=ratinabox.MOUNTAIN_PLOT_SHIFT_MM,
     **kwargs,
 ):
     """Make a mountain plot.
     NbyX is an N by X array of all the plots to display.
     The nth plot is shown at height n, line are scaled so the maximum value across all of them is 0.7,
     then they are all seperated by 1 (sot they don't overlap)
 
@@ -496,21 +497,18 @@
     Returns:
         fig, ax: _description_
     """
     c = color or "C1"
     c = np.array(matplotlib.colors.to_rgb(c))
     fc = 0.3 * c + (1 - 0.3) * np.array([1, 1, 1])  # convert rgb+alpha to rgb
 
-    if norm_by == "max":
-        NbyX = overlap * NbyX / np.max(np.abs(NbyX))
-    else:
-        NbyX = overlap * NbyX / norm_by
+    NbyX = overlap * NbyX / (np.max(np.abs(NbyX)) if norm_by=="max" else norm_by)
     if fig is None and ax is None:
         fig, ax = plt.subplots()
-        fig.set_size_inches(4, len(NbyX) * shift / 25)
+        fig.set_size_inches(width / 25, len(NbyX) * shift / 25)
 
     zorder = 1
     for i in range(len(NbyX)):
         ax.plot(X, NbyX[i] + i + 1, c=c, zorder=zorder)
         zorder -= 0.01
         ax.fill_between(
             X, NbyX[i] + i + 1, i + 1, color=fc, zorder=zorder, alpha=0.8, linewidth=0
@@ -654,72 +652,76 @@
     All parameters found in params will be updated to new value
     Args:
         params (dict): dictionary of parameters to change
         initialise (bool, optional): [description]. Defaults to False.
     """
 
     if get_all_defaults:
-        all_default_params = collect_all_default_params(Class.__class__)
+        all_default_params = collect_all_params(Class.__class__)
         all_default_params.update(params)
         params = all_default_params
 
     for key, value in params.items():
         setattr(Class, key, value)
 
 
-def collect_all_default_params(obj_class, keys_only=False):
-    """Collects all the default_params dictionaries from the current class, including those inherited from its parent classes and its parents parents etc.
+def collect_all_params(obj_class, keys_only=False, dict_name="default_params"):
+    """Collects all the params dictionaries from the current class, including those inherited from its parent classes and its parents parents etc.
 
     Args:
-        obj_class (class): object class for which to collect the default_params dictionaries
-        keys_only (bool, optional): If True, only returns the keys of the default_params dictionaries. Defaults to False.
+        obj_class (class): object class for which to collect the params dictionaries
+        keys_only (bool, optional): If True, only returns the keys of the params dictionaries. Defaults to False.
+        dict_name (str, optional): The name of the class attribute that contains the params dictionary to be collected. Defaults to "default_params".
 
     Returns:
         dict or list:
-            If keys_only == False, returns a dictionary of all the default_params values from the current class, including those inherited from its parent classes.
-            If keys_only == True, returns a list of all the keys of the default_params dictionaries from  the current class and its parent classes.
+            If keys_only == False, returns a dictionary of all the params values from the current class, including those inherited from its parent classes.
+            If keys_only == True, returns a list of all the keys of the params dictionaries from  the current class and its parent classes.
     """
 
     if not inspect.isclass(obj_class):
         raise ValueError("obj_class must be a class object.")
 
-    if not "default_params" in obj_class.__dict__:
+    if not dict_name in obj_class.__dict__.keys():
         warnings.warn(
-            f"Cannot collect the default params dictionaries, as {obj_class} does not "
-            "have a class attribute 'default_params' defined in its preamble. "
-            "(Can be just an empty dictionary, i.e.: default_params = dict().)"
+            f"Cannot collect the {dict_name} dictionaries, as {obj_class.__name__} does not "
+            f"have the class attribute '{dict_name}' defined in its preamble. "
+            f"(Can be just an empty dictionary, i.e.: {dict_name} = dict().)"
         )
-        return
+        if keys_only:
+            return list()
+        else:
+            return dict()
 
     if keys_only:
-        all_default_param_keys = list()
+        all_param_keys = list()
     else:
-        all_default_params_dicts = list()
-        all_default_params = dict()
+        all_params_dicts = list()
+        all_params = dict()
 
-    while hasattr(obj_class, "default_params"):
+    while hasattr(obj_class, dict_name):
         if keys_only:
-            all_default_param_keys.extend(obj_class.default_params.keys())
+            all_param_keys.extend(getattr(obj_class, dict_name).keys())
         else:
-            all_default_params_dicts.append(obj_class.default_params)
+            all_params_dicts.append(getattr(obj_class, dict_name))
         if len(obj_class.__bases__):
             obj_class = obj_class.__bases__[0]
         else:
             break
 
     if keys_only:
-        all_default_param_keys = sorted(set(all_default_param_keys))
-        return all_default_param_keys
+        all_param_keys = sorted(set(all_param_keys))
+        return all_param_keys
 
-    for default_params_dict in all_default_params_dicts[
+    for params_dict in all_params_dicts[
         ::-1
     ]:  # update in reverse (from parents to child class)
-        all_default_params.update(default_params_dict)
+        all_params.update(params_dict)
 
-    return all_default_params
+    return all_params
 
 
 def check_params(Obj, param_keys):
     """Given an object and a list of keys, checks whether the keys are all in
     the object's default_params dictionary.
 
     Args:
@@ -738,15 +740,17 @@
         warnings.warn(
             f"Cannot check the keys in the params dictionary, as {obj_class} does not "
             "have a class attribute 'default_params' defined in its preamble. "
             "(Can be just an empty dictionary, i.e.: default_params = dict().)"
         )
         return
 
-    all_default_param_keys = collect_all_default_params(obj_class, keys_only=True)
+    all_default_param_keys = collect_all_params(
+        obj_class, keys_only=True, dict_name="default_params"
+    )
 
     unexpected_keys = [key for key in param_keys if key not in all_default_param_keys]
 
     if len(unexpected_keys):
         num = len(unexpected_keys)
         unexpected_keys = ", ".join([f"'{attr}'" for attr in unexpected_keys])
```

### Comparing `ratinabox-1.6.1/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.6.2/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.6.1
+Version: 1.6.2
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.6.1/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.6.2/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/setup.cfg` & `ratinabox-1.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.6.1
+version = 1.6.2
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.6.1/tests/test_advanced.py` & `ratinabox-1.6.2/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.6.1/tests/test_environment.py` & `ratinabox-1.6.2/tests/test_environment.py`

 * *Files identical despite different names*

