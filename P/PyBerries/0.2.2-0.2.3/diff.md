# Comparing `tmp/PyBerries-0.2.2.tar.gz` & `tmp/PyBerries-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.2.tar", last modified: Wed May  3 11:08:58 2023, max compression
+gzip compressed data, was "PyBerries-0.2.3.tar", last modified: Thu May  4 12:43:29 2023, max compression
```

## Comparing `PyBerries-0.2.2.tar` & `PyBerries-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.428418 PyBerries-0.2.2/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    14455 2023-05-03 11:08:58.427415 PyBerries-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.397766 PyBerries-0.2.2/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    14455 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 11:08:58.000000 PyBerries-0.2.2/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14137 2023-05-02 10:54:16.000000 PyBerries-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.398766 PyBerries-0.2.2/pyberries/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.405766 PyBerries-0.2.2/pyberries/File_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.2/pyberries/File_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.2/pyberries/File_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.409764 PyBerries-0.2.2/pyberries/Metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.2/pyberries/Metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.425390 PyBerries-0.2.2/pyberries/Plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.2/pyberries/Plots/Fits.py
--rw-rw-rw-   0        0        0     4132 2023-05-02 15:52:54.000000 PyBerries-0.2.2/pyberries/Plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.2/pyberries/Plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.2/pyberries/Plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/Plots/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-02 10:54:16.000000 PyBerries-0.2.2/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:08:58.418765 PyBerries-0.2.2/pyberries/data/
--rw-rw-rw-   0        0        0    15559 2023-05-03 11:07:36.000000 PyBerries-0.2.2/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1922 2023-05-02 15:22:46.000000 PyBerries-0.2.2/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.2/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.2/pyberries/data/util.py
--rw-rw-rw-   0        0        0       42 2023-05-03 11:08:58.428418 PyBerries-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-05-03 11:06:25.000000 PyBerries-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.310075 PyBerries-0.2.3/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    14421 2023-05-04 12:43:29.308076 PyBerries-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.275576 PyBerries-0.2.3/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    14421 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1062 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.276576 PyBerries-0.2.3/pyberries/
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.284576 PyBerries-0.2.3/pyberries/File_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.3/pyberries/File_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.288576 PyBerries-0.2.3/pyberries/Metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/Metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.3/pyberries/Metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.3/pyberries/Metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.307079 PyBerries-0.2.3/pyberries/Plots/
+-rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.3/pyberries/Plots/Fits.py
+-rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.3/pyberries/Plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.3/pyberries/Plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.3/pyberries/Plots/Plots.py
+-rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/Plots/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.299579 PyBerries-0.2.3/pyberries/data/
+-rw-rw-rw-   0        0        0    16099 2023-05-04 10:24:24.000000 PyBerries-0.2.3/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.3/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.3/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.3/pyberries/data/util.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 12:43:29.310075 PyBerries-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-05-04 12:40:58.000000 PyBerries-0.2.3/setup.py
```

### Comparing `PyBerries-0.2.2/LICENSE` & `PyBerries-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/PKG-INFO` & `PyBerries-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.2
+Version: 0.2.3
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -69,15 +69,15 @@
 - If you change plot options, re-run the corresponding cell to update the plot
 - When running your mouse over a plot, a "save" button should appear
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
-`python -m pip install git+https://gitlab.com/MEKlab/pyberries.git`
+`python -m pip install PyBerries`
 
 ### Creating a DatasetPool
 
 ðŸ“– [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
```

### Comparing `PyBerries-0.2.2/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.3/PyBerries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.2
+Version: 0.2.3
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -69,15 +69,15 @@
 - If you change plot options, re-run the corresponding cell to update the plot
 - When running your mouse over a plot, a "save" button should appear
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
-`python -m pip install git+https://gitlab.com/MEKlab/pyberries.git`
+`python -m pip install PyBerries`
 
 ### Creating a DatasetPool
 
 ðŸ“– [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
```

### Comparing `PyBerries-0.2.2/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.3/PyBerries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/README.md` & `PyBerries-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 - If you change plot options, re-run the corresponding cell to update the plot
 - When running your mouse over a plot, a "save" button should appear
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
-`python -m pip install git+https://gitlab.com/MEKlab/pyberries.git`
+`python -m pip install PyBerries`
 
 ### Creating a DatasetPool
 
 📖 [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
```

### Comparing `PyBerries-0.2.2/pyberries/File_utilities/Filename_utils.py` & `PyBerries-0.2.3/pyberries/File_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/File_utilities/Stack_tiffs.py` & `PyBerries-0.2.3/pyberries/File_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/File_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.3/pyberries/File_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/Metrics/Metrics.py` & `PyBerries-0.2.3/pyberries/Metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/Metrics/Time_metrics.py` & `PyBerries-0.2.3/pyberries/Metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/Plots/Fits.py` & `PyBerries-0.2.3/pyberries/Plots/Fits.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/Plots/Plot_presets.py` & `PyBerries-0.2.3/pyberries/Plots/Plot_presets.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,20 +61,31 @@
 
 def plot_boxenplot(df, ax, log:bool=False, **kwargs):
     ax = pyb.plots.boxenplot(df, dodge=True, ax=ax, **kwargs)
     if log: plt.yscale('log')
     return ax
 
 def plot_histogram_fit(df_in, hist, model, ax, fit_results:dict, **kwargs):
-    groupby = kwargs.get('hue','Dataset')
+    groupby = kwargs.get('hue','Group')
     fit_df = pd.DataFrame(columns=['x','Fit',groupby])
     for grp, data in hist.groupby(groupby, sort=False):
         x_model = np.linspace(data.bins.iloc[0], data.bins.iloc[-1], 300)
         df = pd.DataFrame({'x':x_model, 'Fit':model(x_model, *fit_results[grp]), groupby:grp})
         fit_df = pd.concat([fit_df, df], axis=0)
     ax = pyb.plots.histplot(df_in, ax=ax, **kwargs)
     ax = sns.lineplot(data=fit_df, x='x', y='Fit', hue=groupby, legend=False, ax=ax, linestyle='dashed')
 
+def plot_line_fit(df_in, model, ax, fit_results:dict, **kwargs):
+    groupby = kwargs.get('hue','Group')
+    x = kwargs.get('x', 'Frame')
+    fit_df = pd.DataFrame(columns=['x','Fit',groupby])
+    for grp, data in df_in.groupby(groupby, sort=False):
+        x_model = np.linspace(data[x].iloc[0], data[x].iloc[-1], 300)
+        df = pd.DataFrame({'x':x_model, 'Fit':model(x_model, *fit_results[grp]), groupby:grp})
+        fit_df = pd.concat([fit_df, df], axis=0)
+    ax = pyb.plots.lineplot(df_in, ax=ax, **kwargs)
+    ax = sns.lineplot(data=fit_df, x='x', y='Fit', hue=groupby, hue_order=fit_df[groupby].unique(), legend=False, ax=ax, linestyle='dashed')
+
 def plot_rates_summary(rates, ax, **kwargs):
     df = rates.astype({'Group':'category', 'Rate type':'category', 'Rate':'float64'})
-    ax = pyb.plots.stripplot(df, ax=ax, **kwargs)
+    ax = pyb.plots.stripplot(df, ax=ax, jitter=False, **kwargs)
     sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1), labelspacing=1)
```

### Comparing `PyBerries-0.2.2/pyberries/Plots/Plots.py` & `PyBerries-0.2.3/pyberries/Plots/Plots.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/pyberries/data/DatasetPool.py` & `PyBerries-0.2.3/pyberries/data/DatasetPool.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,30 +42,41 @@
             cf = join(ds_path, ds, f"{ds}_config.json")
             with open(cf, errors='ignore') as f:
                 conf = json.load(f)
                 object_class_names = [c["name"] for c in conf["structures"]["list"]]
                 object_parents = [c["segmentationParent"] for c in conf["structures"]["list"]]
                 channel_images = [c["channelImage"] for c in conf["structures"]["list"]]
 
+            # Add Viewfield object if measurement table is available
+            if exists(join(ds_path, ds, f"{ds}_{-1}.csv")):
+                object_class_names.insert(0, 'Viewfield')
+                object_parents.insert(0, [])
+                channel_images.insert(0, [-1])
+                start_table = -1
+            else:
+                start_table = 0
+
             # Load data tables
-            for j, obj in enumerate(object_class_names):
+            k = 0
+            for j, obj in enumerate(object_class_names, start_table):
                 df_in = pd.read_csv(join(ds_path, ds, f"{ds}_{j}.csv"), sep=';', low_memory=False)
                 df_in['Dataset'] = ds
                 df_in['Group'] = groups[i] if groups else i
                 df_in[['Dataset', 'Group']] = df_in[['Dataset', 'Group']].astype('category')
                 if obj in preprocessing.keys():
                     if len(preprocessing[obj]) == 1:
                         df_in = df_in.transform(preprocessing[obj][0])
                     elif len(preprocessing[obj]) > 1:
                         assert len(preprocessing[obj]) == len(self.dsList), 'If multiple pre-processings are provided, there should be one per dataset'
                         if preprocessing[obj][i]:
                             df_in = df_in.transform(preprocessing[obj][i])
                 self.table[obj] = df_in if obj not in self.table.keys() else pd.concat([self.table[obj], df_in], axis=0)
-                self.parent[obj] = object_class_names[object_parents[j][0]] if object_parents[j] else None
-                self.channel[obj] = channel_images[j][0]
+                self.parent[obj] = object_class_names[object_parents[k][0]+1] if object_parents[k] else 'Viewfield'
+                self.channel[obj] = channel_images[k][0]
+                k+=1
             print(f'Dataset {ds}: loaded objects {object_class_names}')
         self.objects = self.table.keys()
         for data in self.table.values():
             data.reset_index(drop=True, inplace=True)
 
         self.add_metadata(metadata)
         self.apply_filters(filters)
@@ -107,15 +118,15 @@
                     if var == 'DateTime':
                         df['TimeDelta'] = 0
                         df['Time_min'] = 0
                     for i, ds in enumerate(self.dsList):
                         ds_path = self.path[0] if len(self.path) == 1 else self.path[i]
                         for pos in df.loc[df['Dataset'] == ds].Position.unique():
                             # Open metadata file
-                            with open(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c{channel}.txt')) as f:
+                            with open(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c{channel}_t0.txt')) as f:
                                 value = next((line for line in f if var in line), None)
                                 # Add metadata value to the current dataset and position
                                 df.loc[(df['Position'] == pos) & (df['Dataset'] == ds), var.replace(' ', '_')] = value.split('=')[-1][:-1] # Remove line break (last character)
                         if 'DateTime' in df.columns:
                             df.loc[df['Dataset'] == ds] = (df.loc[df['Dataset'] == ds]
                                                             .assign(DateTime = lambda df: pd.to_datetime(df.DateTime, format='%Y%m%d %H:%M:%S.%f'),
                                                                     TimeDelta = lambda df: df.DateTime - df.DateTime.iloc[0],
@@ -268,14 +279,16 @@
             ax = pyb.plots.plot_histogram(df_in, ax=ax, **kwargs)
         elif preset == 'histogram_fit':
             ax = pyb.plots.plot_histogram_fit(df_in, ax=ax, **kwargs)
         elif preset == 'bar':
             ax = pyb.plots.barplot(df_in, ax=ax, **kwargs)
         elif preset == 'line':
             ax = pyb.plots.lineplot(df_in, ax=ax, **kwargs)
+        elif preset == 'line_fit':
+            ax = pyb.plots.plot_line_fit(df_in, ax=ax, **kwargs)
         elif preset == 'scatter':
             ax = pyb.plots.scatterplot(df_in, ax=ax, **kwargs)
         elif preset == 'datapoints_and_mean':
             ax = pyb.plots.plot_datapoints_and_mean(df_in, dsList=self.dsList, ax=ax, **kwargs)
         elif preset == 'heatmap':
             ax = pyb.plots.plot_heatmap(df_in, ax=ax, **kwargs)
         elif preset == 'timeseries':
```

### Comparing `PyBerries-0.2.2/pyberries/data/Fitting.py` & `PyBerries-0.2.3/pyberries/data/Fitting.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,27 +7,24 @@
 def get_model(model_type=''):
     if model_type == 'monoexp_decay':
         def model(x, a, b):
             return a*np.exp(-b*x, dtype='float64')
     elif model_type == 'biexp_decay':
         def model(x, a, b, c, d):
             return a*np.exp(-b*x, dtype='float64') + c*np.exp(-d*x, dtype='float64')
+    elif model_type == 'monoexp_decay_offset':
+        def model(x, a, b, c):
+            return a*np.exp(-b*x) + c
     return model
 
-def fit_exp_decay_histogram(hist, model, groupby:str='Dataset'):
+def make_fit(df_in, x:str, y:str, model, groupby:str='Group', p0=None):
     fit_results = dict()
-    if len(inspect.getfullargspec(model).args) == 3:
-        p0 = [hist.bins.iloc[0], 1]
-    elif len(inspect.getfullargspec(model).args) == 5:
-        p0=[hist.bins.iloc[0], 1, hist.bins.iloc[0]/10, 0.1]
-    else:
-        ValueError('Unrecognised model function')
-    for name, data in hist.groupby(groupby, sort=False):
+    for name, data in df_in.groupby(groupby, sort=False):
         try:
-            popt,_ = curve_fit(model, data.bins, data.height, p0=p0)
+            popt,_ = curve_fit(model, data[x], data[y], p0=p0)
             fit_results[name] = popt
         except:
             print(f'Fit for dataset {name} failed')
     return fit_results
 
 def get_rates(fit_results, model, dt=1):
     dt = arg_to_list(dt)
@@ -40,8 +37,9 @@
             rates.loc[i] = {'Group':grp, 'Rate type':1, 'Rate':popt[1]/dt_grp, 'Population':1}
             i+=1
         elif len(inspect.getfullargspec(model).args) == 5:
             rates.loc[i] = {'Group':grp, 'Rate type':'Fast', 'Rate':popt[1]/dt_grp, 'Population':popt[0]/(popt[0]+popt[2])}
             i+=1
             rates.loc[i] = {'Group':grp, 'Rate type':'Slow', 'Rate':popt[3]/dt_grp, 'Population':popt[2]/(popt[0]+popt[2])}
             i+=1
+    rates = rates.astype({'Group':'category', 'Rate type':'category', 'Rate':'float64', 'Population':'float64'})
     return rates
```

### Comparing `PyBerries-0.2.2/pyberries/data/util.py` & `PyBerries-0.2.3/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.2/setup.py` & `PyBerries-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.2",
+    version="0.2.3",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
```

