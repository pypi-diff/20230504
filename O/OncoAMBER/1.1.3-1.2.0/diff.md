# Comparing `tmp/OncoAMBER-1.1.3.tar.gz` & `tmp/OncoAMBER-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OncoAMBER-1.1.3.tar", last modified: Mon May  1 16:41:24 2023, max compression
+gzip compressed data, was "OncoAMBER-1.2.0.tar", last modified: Thu May  4 19:47:57 2023, max compression
```

## Comparing `OncoAMBER-1.1.3.tar` & `OncoAMBER-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.273994 OncoAMBER-1.1.3/
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.218954 OncoAMBER-1.1.3/OncoAMBER.egg-info/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)      613 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/SOURCES.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/dependency_links.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/not-zip-safe
--rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/requires.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-01 16:41:24.000000 OncoAMBER-1.1.3/OncoAMBER.egg-info/top_level.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-01 16:41:24.273658 OncoAMBER-1.1.3/PKG-INFO
--rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/README.md
-drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-01 16:41:24.272187 OncoAMBER-1.1.3/amber/
--rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/BasicGeometries.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/amber/BetaDistributionCalibration.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5291 2023-04-27 16:58:04.000000 OncoAMBER-1.1.3/amber/CONFIG_default.txt
--rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Cell.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    21348 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Process.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.1.3/amber/ReadAndWrite.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/ScalarField.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/Terminal.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    14247 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Vessel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)     5487 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/Voxel.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    21621 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/World.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/__init__.py
--rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/amber/config.py
--rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/save_alpha_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.1.3/amber/save_beta_dataframe6.csv
--rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-01 16:41:24.274087 OncoAMBER-1.1.3/setup.cfg
--rw-r--r--   0 louiskunz   (501) staff       (20)     3009 2023-05-01 16:41:03.000000 OncoAMBER-1.1.3/setup.py
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.678350 OncoAMBER-1.2.0/
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.600067 OncoAMBER-1.2.0/OncoAMBER.egg-info/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)      588 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/SOURCES.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/dependency_links.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        1 2023-04-21 16:40:31.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/not-zip-safe
+-rw-r--r--   0 louiskunz   (501) staff       (20)       47 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/requires.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)        6 2023-05-04 19:47:57.000000 OncoAMBER-1.2.0/OncoAMBER.egg-info/top_level.txt
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2758 2023-05-04 19:47:57.678104 OncoAMBER-1.2.0/PKG-INFO
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2002 2023-04-27 16:58:04.000000 OncoAMBER-1.2.0/README.md
+drwxr-xr-x   0 louiskunz   (501) staff       (20)        0 2023-05-04 19:47:57.676799 OncoAMBER-1.2.0/amber/
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2239 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/BasicGeometries.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     6028 2023-04-27 16:58:04.000000 OncoAMBER-1.2.0/amber/BetaDistributionCalibration.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     2055 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/Cell.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    22475 2023-05-04 19:20:45.000000 OncoAMBER-1.2.0/amber/Process.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     1606 2023-04-21 19:04:46.000000 OncoAMBER-1.2.0/amber/ReadAndWrite.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3438 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/ScalarField.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      744 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/Terminal.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    14625 2023-05-04 19:06:01.000000 OncoAMBER-1.2.0/amber/Vessel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)     5571 2023-05-03 20:48:53.000000 OncoAMBER-1.2.0/amber/Voxel.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    24068 2023-05-04 15:26:46.000000 OncoAMBER-1.2.0/amber/World.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      308 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/__init__.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)      211 2023-05-01 16:41:03.000000 OncoAMBER-1.2.0/amber/config.py
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17301 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/save_alpha_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)    17411 2023-04-21 16:39:43.000000 OncoAMBER-1.2.0/amber/save_beta_dataframe6.csv
+-rw-r--r--   0 louiskunz   (501) staff       (20)       38 2023-05-04 19:47:57.678422 OncoAMBER-1.2.0/setup.cfg
+-rw-r--r--   0 louiskunz   (501) staff       (20)     3010 2023-05-04 19:41:40.000000 OncoAMBER-1.2.0/setup.py
```

### Comparing `OncoAMBER-1.1.3/OncoAMBER.egg-info/PKG-INFO` & `OncoAMBER-1.2.0/OncoAMBER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.3
+Version: 1.2.0
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.1.3/OncoAMBER.egg-info/SOURCES.txt` & `OncoAMBER-1.2.0/OncoAMBER.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 OncoAMBER.egg-info/SOURCES.txt
 OncoAMBER.egg-info/dependency_links.txt
 OncoAMBER.egg-info/not-zip-safe
 OncoAMBER.egg-info/requires.txt
 OncoAMBER.egg-info/top_level.txt
 amber/BasicGeometries.py
 amber/BetaDistributionCalibration.py
-amber/CONFIG_default.txt
 amber/Cell.py
 amber/Process.py
 amber/ReadAndWrite.py
 amber/ScalarField.py
 amber/Terminal.py
 amber/Vessel.py
 amber/Voxel.py
```

### Comparing `OncoAMBER-1.1.3/PKG-INFO` & `OncoAMBER-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OncoAMBER
-Version: 1.1.3
+Version: 1.2.0
 Summary: Agent-based model of tumor growth and response to radiation therapy
 Home-page: https://github.com/lvkunz/AMBER
 Author: Louis Kunz
 Author-email: lvkunz@mgh.harvard.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `OncoAMBER-1.1.3/README.md` & `OncoAMBER-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/BasicGeometries.py` & `OncoAMBER-1.2.0/amber/BasicGeometries.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/BetaDistributionCalibration.py` & `OncoAMBER-1.2.0/amber/BetaDistributionCalibration.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/Cell.py` & `OncoAMBER-1.2.0/amber/Cell.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/Process.py` & `OncoAMBER-1.2.0/amber/Process.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 
     def __init__(self, config, list_of_process : list, finish_time, dt):
         self.list_of_process = list_of_process
         self.finish_time = finish_time
         self.dt = dt
         self.time = 0
         self.config = config
-    def show_cell_and_tumor_volume(self, number_tumor_cells, number_necrotic_cells, tumor_size, times):
+    def show_cell_and_tumor_volume(self, number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, times):
         # plot number of cells evolution
-        plt.plot(times, number_tumor_cells, 'purple')
-        plt.plot(times, number_necrotic_cells, 'black')
+        plt.plot(times, number_tumor_cells, 'blue', label='All cells')
+        plt.plot(times, number_cycling_cells, 'red', label='Cycling cells')
+        plt.plot(times, number_quiescent_cells, 'green', label='Quiescent cells')
+        plt.plot(times, number_necrotic_cells, 'black', label='Necrotic cells')
         plt.title('Number of cells evolution')
         plt.xlabel('Time')
         plt.ylabel('Number of cells')
         plt.grid(True)
+        plt.legend()
         plt.savefig('Plots/Number_cells_evolution.png')
         plt.show()
 
         # plot tumor size evolution
         fig = plt.figure()
         plt.plot(times, tumor_size, 'red')
         plt.title('Tumor volume evolution')
@@ -42,14 +45,16 @@
             os.makedirs('Plots/CurrentPlotting/')
 
         print('Graphics : ', self.config.show_tumor_and_vessels_3D, self.config.show_slices)
 
         DPI = 100
         size = world.half_length
 
+        if self.config.show_angiogenesis_metrics:
+            world.show_angiogenesis_metrics(False)
         #plot vasculature
         if self.config.show_tumor_and_vessels_3D:
             fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(25, 25), dpi=150, subplot_kw={'projection': '3d'})
             fig.suptitle('Visualization at time t = ' + str(t) + ' hours', fontsize=16)
             axes.set_xlim(-size, size)
             axes.set_ylim(-size, size)
             axes.set_zlim(-size, size)
@@ -119,15 +124,16 @@
         process_local = [process for process in self.list_of_process if not process.is_global]
         process_global = [process for process in self.list_of_process if process.is_global]
 
         irradiations_times = [self.config.first_irradiation_time + i * self.config.time_between_fractions for i in
                               range(self.config.number_fractions)]
         applied_fractions = 0
 
-        number_tumor_cells = []; number_necrotic_cells = []; tumor_size = []; times = []
+        number_cycling_cells = []; number_quiescent_cells = []; number_necrotic_cells = []; tumor_size = []; times = [];
+        number_tumor_cells = []
 
         while self.time < self.finish_time:
             print(f'\033[1;31;47mTime: {self.time} hours / {self.finish_time} hours\033[0m')
             if video:
                 self.show(world, self.time)
 
             if applied_fractions < self.config.number_fractions and self.time >= irradiations_times[applied_fractions]:
@@ -139,32 +145,46 @@
             for voxel in world.voxel_list:
                 for process in process_local:
                     process(voxel)
             for process in process_global:
                 print('Currently running global process:', process.name)
                 process(world)
 
-
-
-            number_tumor_cells.append(sum([voxel.number_of_tumor_cells() for voxel in world.voxel_list]))
-            number_necrotic_cells.append(sum([voxel.number_of_necrotic_cells() for voxel in world.voxel_list]))
+            cycling_cells = 0
+            quiescent_cells = 0
+            necrotic_cells = 0
+            for voxel in world.voxel_list:
+                necrotic_cells += voxel.number_of_necrotic_cells()
+                for cell in voxel.list_of_cells:
+                    if cell.type == 'TumorCell':
+                        if cell.vitality() > self.config.vitality_cycling_threshold:
+                            cycling_cells += 1
+                        else:
+                            quiescent_cells += 1
+
+            number_cycling_cells.append(cycling_cells)
+            number_quiescent_cells.append(quiescent_cells)
+            number_necrotic_cells.append(necrotic_cells)
+            number_tumor_cells.append(cycling_cells + quiescent_cells + necrotic_cells)
             tumor_size_ = world.measure_tumor_volume()
-            tumor_size.append(tumor_size_ * 1000)
+            tumor_size.append(tumor_size_)
             times.append(self.time)
 
             if not os.path.exists('DataOutput/'):
                 os.makedirs('DataOutput/')
 
             np.save('DataOutput/number_tumor_cells.npy', number_tumor_cells)
             np.save('DataOutput/number_necrotic_cells.npy', number_necrotic_cells)
+            np.save('DataOutput/number_cycling_cells.npy', number_cycling_cells)
+            np.save('DataOutput/number_quiescent_cells.npy', number_quiescent_cells)
             np.save('DataOutput/tumor_size.npy', tumor_size)
             np.save('DataOutput/times.npy', times)
 
             if self.config.show_cell_and_tumor_volume:
-                self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, tumor_size, times)
+                self.show_cell_and_tumor_volume(number_tumor_cells, number_necrotic_cells, number_quiescent_cells, number_cycling_cells, tumor_size, times)
 
             self.time += self.dt
 
         print('Simulation finished')
 
         if self.config.show_final:
             self.show(world, self.time)
@@ -276,15 +296,15 @@
                 for cell in list_of_moving_cells:
                     if neighbor.add_cell(cell):
                         voxel.remove_cell(cell)
 
 class UpdateCellOxygen(Process):
     def __init__(self, config, name, dt, voxel_half_length, effective_vessel_radius):
         super().__init__(config, 'UpdateState', dt)
-        self.voxel_side = int(voxel_half_length*200) #um/100
+        self.voxel_side = int(voxel_half_length*20) #um/100
         self.effective_vessel_radius = effective_vessel_radius
 
         amber_dir = os.path.abspath(os.path.dirname(__file__))
 
         alpha_file_name = 'save_alpha_dataframe' + str(self.voxel_side) + '.csv'
         beta_file_name = 'save_beta_dataframe' + str(self.voxel_side) + '.csv'
         alpha_file_name = os.path.join(amber_dir, alpha_file_name)
@@ -435,15 +455,14 @@
             os.rename('TopasSimulation/MyScorer.csv', 'TopasSimulation/' + topas_file + '.csv')
         _, self.doses = rw.DoseOnWorld('TopasSimulation/' + topas_file + '.csv')
         world.update_dose(self.doses)
 
         # plot the simulation
         fig = plt.figure(figsize=(10, 10))
         ax = fig.add_subplot(111, projection='3d')
-        world.show_voxels_centers_dose(ax, fig, slice=True)
         plt.show()
     def __call__(self, world: World):
         for voxel in world.voxel_list:
             count = 0
             probability = self.doses[voxel.voxel_number]*self.irradiation_intensity*self.config.radiosensitivity
             for cell in voxel.list_of_cells:
                 if random.random() < probability:
```

### Comparing `OncoAMBER-1.1.3/amber/ReadAndWrite.py` & `OncoAMBER-1.2.0/amber/ReadAndWrite.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/ScalarField.py` & `OncoAMBER-1.2.0/amber/ScalarField.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/Terminal.py` & `OncoAMBER-1.2.0/amber/Terminal.py`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/Vessel.py` & `OncoAMBER-1.2.0/amber/Vessel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import random
+
+import numpy as np
+
 from amber.BasicGeometries import *
 import sys
 
 sys.setrecursionlimit(1500)
 
 class Vessel:
     def __init__(self, path, radius, step_size, parent_id=None, children_ids=None, in_growth=True):
@@ -97,25 +100,27 @@
 
     def volume_per_point(self):
         return np.pi * self.radius ** 2 * self.step_size
 
     def plot(self,fig, ax, color='crimson'):
         if self.visible:
             if self.in_growth:
-                ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color=color, alpha=0.7, linewidth= self.radius*300)
+                ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color=color, alpha=0.7, linewidth= self.radius*30)
             else:
-                ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color='mediumblue', alpha=0.1, linewidth= self.radius*300)
+                ax.plot(self.path[:, 0], self.path[:, 1], self.path[:, 2], color='mediumblue', alpha=0.1, linewidth= self.radius*30)
         return fig, ax
+
     def choose_random_point(self, seed):
-        rng = np.random.default_rng(seed)
-        #choose random point on the path, not the first or last point
+        # choose random point on the path, not the first or last point
         if len(self.path) < 3:
             print(self.path)
             raise ValueError("The vessel path is too short to choose a random point")
-        return rng.choice(self.path[1:-1])
+        random_index = random.randint(1, len(self.path) - 2)
+        return self.path[random_index]
+
     def mean_pressure(self, pressure):
         if len(self.path) < 2:
             return 0
         else:
             return np.mean([pressure(point) for point in self.path])
 
     def max_pressure(self, pressure):
@@ -260,15 +265,19 @@
         for vessel in self.list_of_vessels:
             vessel.plot(fig, ax, color)
         return fig, ax
 
 
     def grow_and_split(self, dt, splitting_rate, vegf_gradient, pressure, macro_steps=1, micro_steps=10, weight_direction=0.5, weight_vegf=0.5, weight_pressure=0.5):
         micro_steps = micro_steps
-        for i in range(macro_steps * dt):
+        macro_steps = int(macro_steps * dt)
+        if macro_steps == 0:
+            ValueError("Macro steps must be at least 1")
+            macro_steps = 1
+        for i in range(macro_steps):
             print("Macro step {}".format(i))
             j = 0
             for vessel in self.list_of_vessels:
                 splitting_rate_ = splitting_rate
                 if j % 1000 == 0: print('current number of vessels {}'.format(len(self.list_of_vessels)))
                 if vessel.in_growth:
                     total_path_length = vessel.step_size * micro_steps
@@ -294,7 +303,13 @@
         root_vessels = [v for v in vessels if v.parent_id is None]
 
         # recursively print the vessel tree
         for root_vessel in root_vessels:
             print(' ' * indent, f"ID: {root_vessel.id}  Radius: {root_vessel.radius:.5f}")
             if root_vessel.children_ids:
                 self.print_vessel_tree_recursive(vessels, root_vessel.children_ids, indent + 2)
+
+    def compute_VSL(self):
+        list_VSL = np.array([])
+        for vessel in self.list_of_vessels:
+            list_VSL = np.append(list_VSL, vessel.length())
+        return list_VSL
```

### Comparing `OncoAMBER-1.1.3/amber/Voxel.py` & `OncoAMBER-1.2.0/amber/Voxel.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
                 self.voxel_number = voxel_number
                 self.dose = 0
                 self.molecular_factors = {'EGF': 0, 'FGF': 0, 'HGF': 0, 'IGF': 0, 'TGF': 0, 'VEGF': 0, 'WNT': 0}
                 # if np.linalg.norm(self.position) < 5:
                 #         self.molecular_factors['VEGF'] = 1.0
                 self.viscosity = viscosity
                 self.vessel_volume = 0
+                self.vessel_length = 0
+                self.bifurcation_density = 0
 
         def number_of_tumor_cells(self):
                 number = 0
                 for cell in self.list_of_cells:
                         if cell.type == 'TumorCell':
                                 number = number + 1
                 return number
```

### Comparing `OncoAMBER-1.1.3/amber/World.py` & `OncoAMBER-1.2.0/amber/World.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from amber.voxel import *
 from amber.vessel import *
 from amber.ScalarField import *
 from amber.BasicGeometries import *
 #np.set_printoptions(threshold=sys.maxsize)
 # from scipy.stats import qmc
 import matplotlib.tri as mtri
+import matplotlib.pyplot as plt
 import scipy.sparse as sparse
 
 class World:
     def __init__(self, config):
         print('Initializing world')
         print(config.voxel_per_side, config.half_length_world)
         self.half_length = config.half_length_world
@@ -56,15 +57,15 @@
     def generate_healthy_vasculature(self, initial_vessel_number, splitting_rate =0.3, mult_macro_steps=1, micro_steps=8, weight_direction=3.0, weight_vegf=1.0, weight_pressure=0.0, extra_step = True):
         initial_vessel_number = int(initial_vessel_number * 4 * self.half_length ** 2)
         # sampler = qmc.Halton(2, seed=config.seed)
         # points_z = (sampler.random(initial_vessel_number)[:,0] - 0.5) * self.half_length*2
         # points_y = (sampler.random(initial_vessel_number)[:,1] - 0.5) * self.half_length*2
         points_z = np.random.uniform(-self.half_length, self.half_length, initial_vessel_number)
         points_y = np.random.uniform(-self.half_length, self.half_length, initial_vessel_number)
-        points_x = np.append(self.half_length * np.ones(initial_vessel_number//2), -self.half_length * np.ones(initial_vessel_number//2))
+        points_x = -self.half_length * np.ones(initial_vessel_number)
         points = []
         for i in range(len(points_x)):
             points.append([points_x[i], points_y[i], points_z[i]])
         points = np.array(points)
         points2 = []
         for i in range(len(points)):
             if points[i][0] == self.half_length:
@@ -75,45 +76,33 @@
         print('Initial vessels: ', points[0], points2[0])
 
         list_of_vessels = []
         for j in range(len(points)):
             list_of_vessels.append(Vessel([points[j], points2[j]], 0.5, step_size=self.config.vessel_step_size))
         self.initiate_vasculature(list_of_vessels)
         def pressure(point):
-            return (self.half_length - abs(point[0]))*0.3
+            return (self.half_length - abs(point[0]))*0.06
         def vegf_gradient(point):
-            if point[0] > 0:
-                return np.array([-point[0],0,0])*0.1
-            else:
-                return np.array([-point[0],0,0])*0.1
+            return np.array([1,0,0])
+            # if point[0] > 0:
+            #     return np.array([-point[0],0,0])
+            # else:
+            #     return np.array([point[0],0,0])
 
         self.vasculature.grow_and_split(
             dt=1,
             splitting_rate=splitting_rate,
             vegf_gradient= vegf_gradient,
             pressure= pressure,
-            macro_steps=int(9*self.half_length*mult_macro_steps),
+            macro_steps=int(0.9*self.half_length*mult_macro_steps),
             micro_steps=micro_steps,
             weight_direction=weight_direction,
             weight_vegf=weight_vegf,
             weight_pressure=weight_pressure
         )
-        if extra_step:
-            self.vasculature.grow_and_split(
-                dt=1,
-                splitting_rate=splitting_rate,
-                vegf_gradient=vegf_gradient,
-                pressure=pressure,
-                macro_steps=1,
-                micro_steps=micro_steps,
-                weight_direction=weight_direction,
-                weight_vegf=0.1,
-                weight_pressure=0.0
-            )
-
 
         self.vasculature.update_vessels_radius_from_last(self.config.radius_root_vessels, False, pressure)
         for vessel in self.vasculature.list_of_vessels:
             vessel.in_growth = False
             vessel.visible = self.config.visible_original_vessels
         return
 
@@ -137,27 +126,40 @@
                     points.append(voxel.random_points_in_voxel(1)[0])
         points = points[0:num_points]
         points = np.array(points)
         np.random.shuffle(points)
         return points
 
     def update_volume_occupied_by_vessels(self):
-        scorer = np.zeros((self.total_number_of_voxels))
-        print('-- Computing volume occupied by vessels in each voxel')
+        volume_score = np.zeros(self.total_number_of_voxels)
+        bifurcation_score = np.zeros(self.total_number_of_voxels)
+        length_score = np.zeros(self.total_number_of_voxels)
+        print('-- Computing volume and length occupied by vessels in each voxel')
         for vessel in self.vasculature.list_of_vessels:
-            for point in vessel.path:
-                voxel_n = self.find_voxel_number(point)
-                if voxel_n == -1:
+            if len(vessel.path) > 0:
+                voxel_n_ = self.find_voxel_number(vessel.path[0])
+                bifurcation_score[voxel_n_] += 1
+            for i in range(1, len(vessel.path)):
+                start_point = vessel.path[i - 1]
+                end_point = vessel.path[i]
+                start_voxel = self.find_voxel_number(start_point)
+                if start_voxel == -1:
                     continue
-                scorer[voxel_n] += vessel.volume_per_point()
-        print('-- Finishing up -- CHECK IF NECESSARY')
+                line_segment = end_point - start_point
+                line_segment_length = np.linalg.norm(line_segment)
+                length_score[start_voxel] += line_segment_length
+                volume_score[start_voxel] += vessel.volume_per_point()
+        print('-- Finishing up')
         for voxel in self.voxel_list:
-            voxel.vessel_volume = scorer[voxel.voxel_number]
+            voxel.vessel_volume = volume_score[voxel.voxel_number]
+            voxel.bifurcation_density = bifurcation_score[voxel.voxel_number]
+            voxel.vessel_length = length_score[voxel.voxel_number]
         return
 
+
     def update_biology_after_RT(self):
         print('-- Updating biology after RT')
         for voxel in self.voxel_list:
             voxel.update_cells_afterRT()
         #self.vessels_killed_by_dose()
         #self.update_oxygen()
     def vessels_killed(self, radius_threshold = 1e-3, length_threshold = 0):
@@ -280,14 +282,15 @@
             voxel.dose = doses[voxel.voxel_number]
         return
 
     def update_oxygen(self, o2_per_volume=1, diffusion_number=5):
         print('-- Computing oxygen map')
         for voxel in self.voxel_list:
             voxel.oxygen = int((voxel.vessel_volume * o2_per_volume) / (np.pi * self.config.effective_vessel_radius**2 * voxel.half_length * 2))
+            voxel.bifurcation_density += voxel.oxygen
         for i in range(diffusion_number):
             new_oxygen_map = np.zeros(self.total_number_of_voxels)
             print('--- o2 map computing', i, 'out of', diffusion_number)
             for voxel in self.voxel_list:
                 sum = voxel.oxygen
                 for neighbor in self.find_neighbors(voxel):
                     sum += neighbor.oxygen
@@ -469,10 +472,54 @@
     def measure_tumor_volume(self):
         volume = 0
         for voxel in self.voxel_list:
             if voxel.number_of_tumor_cells() > 3:
                 volume += voxel.volume
         return volume
 
+    def show_angiogenesis_metrics(self, real = True):
+        # Extract the voxel values for each parameter
+        volume = self.voxel_list[0].volume
+        side = self.voxel_list[0].half_length*2
+        if real:
+            volume_values = [voxel.vessel_volume/volume for voxel in self.voxel_list]
+            length_values = [voxel.vessel_length/volume for voxel in self.voxel_list]
+
+        else:
+            capillary_volume = side*np.pi*self.config.effective_vessel_radius**2
+            volume_values = [voxel.oxygen*capillary_volume/volume for voxel in self.voxel_list]
+            length_values = [voxel.oxygen*side/volume for voxel in self.voxel_list]
+
+        bifurcation_values = [voxel.bifurcation_density / volume for voxel in self.voxel_list]
+        VSL_values = self.vasculature.compute_VSL()
+        # Calculate mean and median values
+        volume_mean = np.mean(volume_values)
+        volume_median = np.median(volume_values)
+        length_mean = np.mean(length_values)
+        length_median = np.median(length_values)
+        bifurcation_mean = np.mean(bifurcation_values)
+        bifurcation_median = np.median(bifurcation_values)
+        VSL_mean = np.mean(VSL_values)
+        VSL_median = np.median(VSL_values)
+
+        # Plot histograms for each parameter
+        fig, axes = plt.subplots(2, 2, figsize=(10, 8))
+        axes[0, 0].hist(volume_values, bins=20, color='blue')
+        axes[0, 0].set_title(f'Vessel volume density, mean: {volume_mean:.2f}, median: {volume_median:.2f}')
+        axes[0, 1].hist(length_values, bins=20, color='green')
+        axes[0, 1].set_title(f'Vessel length density, mean: {length_mean:.2f}, median: {length_median:.2f}')
+        axes[1, 0].hist(bifurcation_values, bins=20, color='red')
+        axes[1, 0].set_title(
+            f'Voxel bifurcation density, mean: {bifurcation_mean:.2f}, median: {bifurcation_median:.2f}')
+        axes[1, 1].hist(VSL_values, bins=20, color='purple')
+        axes[1, 1].set_title(f'Vessel segment length, mean: {VSL_mean:.2f}, median: {VSL_median:.2f}')
+        plt.show()
+
+
+
+
+
+
+
```

### Comparing `OncoAMBER-1.1.3/amber/save_alpha_dataframe6.csv` & `OncoAMBER-1.2.0/amber/save_alpha_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/amber/save_beta_dataframe6.csv` & `OncoAMBER-1.2.0/amber/save_beta_dataframe6.csv`

 * *Files identical despite different names*

### Comparing `OncoAMBER-1.1.3/setup.py` & `OncoAMBER-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Package meta-data
 NAME = 'OncoAMBER'
 DESCRIPTION = 'Agent-based model of tumor growth and response to radiation therapy'
 URL = 'https://github.com/lvkunz/AMBER'
 EMAIL = 'lvkunz@mgh.harvard.edu'
 AUTHOR = 'Louis Kunz'
 REQUIRES_PYTHON = '>=3.8.2'
-VERSION = '1.1.3'
+VERSION = '1.2.0'
 
 # Required packages for this module to be executed
 REQUIRED = ['numpy', 'pandas', 'scipy']
 
 # Optional packages
 EXTRAS = { 'plots' :['matplotlib', 'seaborn'] }
 
@@ -90,12 +90,12 @@
     packages=find_packages(),
     package_data={'': ['*.txt', '*.csv'],},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     # include_package_data=True,
     zip_safe=False,
     license='MIT',
-    classifiers=[  'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
+    classifiers=[   'License :: OSI Approved :: MIT License',    'Operating System :: MacOS',    'Operating System :: Microsoft :: Windows',    'Programming Language :: Python',    'Programming Language :: Python :: 3',    'Programming Language :: Python :: 3.6',    'Programming Language :: Python :: Implementation :: CPython',    'Programming Language :: Python :: Implementation :: PyPy'],
     cmdclass={
         'upload' : UploadCommand,
     }
 )
```

