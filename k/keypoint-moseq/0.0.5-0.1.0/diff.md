# Comparing `tmp/keypoint-moseq-0.0.5.tar.gz` & `tmp/keypoint-moseq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.0.5.tar", last modified: Mon May  1 16:41:52 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.0.tar", last modified: Thu May  4 15:20:07 2023, max compression
```

## Comparing `keypoint-moseq-0.0.5.tar` & `keypoint-moseq-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.685750 keypoint-moseq-0.0.5/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.5/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.5/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-01 16:41:52.686016 keypoint-moseq-0.0.5/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1394 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.5/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.664846 keypoint-moseq-0.0.5/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      784 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.5/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.0.5/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17652 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17495 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32459 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    26681 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    66580 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.685314 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      136 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-05-01 16:41:52.686939 keypoint-moseq-0.0.5/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      830 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.196150 keypoint-moseq-0.1.0/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.0/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.0/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-04 15:20:07.196308 keypoint-moseq-0.1.0/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1613 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.197762 keypoint-moseq-0.1.0/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      878 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-04 15:20:07.197863 keypoint-moseq-0.1.0/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.1.0/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17369 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    32958 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27288 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    67128 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.195621 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      143 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      723 2023-05-04 15:20:07.197316 keypoint-moseq-0.1.0/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/versioneer.py
```

### Comparing `keypoint-moseq-0.0.5/LICENSE.md` & `keypoint-moseq-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.5/NOTICE.md` & `keypoint-moseq-0.1.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/__init__.py` & `keypoint-moseq-0.1.0/keypoint_moseq/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     noise_calibration,
 )
 
 from .fitting import (
     revert, 
     fit_model, 
     apply_model, 
+    extract_results,
     resume_fitting, 
     update_hypparams,
 )
 
 from .viz import (
     plot_pcs, 
     plot_scree, 
@@ -37,8 +38,10 @@
     get_group_trans_mats,
     changepoint_analysis,
 )
 
 from jax_moseq.models.keypoint_slds import (
     fit_pca, 
     init_model
-)
+)
+from . import _version
+__version__ = _version.get_versions()['version']
```

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.0/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.0/keypoint_moseq/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         colorvals = np.linspace(0,1,len(bodyparts))
         pt_data = np.append(point,colorvals[keypoint_ix])[None]
         hv_point = hv.Points(pt_data, vdims=['bodypart']).opts(
             color='bodypart', cmap='autumn', size=15, framewise=True, marker='x', line_width=3)
         
         label = f'{bodypart}, confidence = {confs[keypoint_ix]:.5f}'
         h,w = sample_images[sample_key].shape[:2]
-        rgb = hv.RGB(sample_images[sample_key][::-1], bounds=(0,0,w,h), label=label).opts(
+        rgb = hv.RGB(sample_images[sample_key], bounds=(0,2*h,w,h), label=label).opts(
             framewise=True, xaxis='bare', yaxis='bare', frame_width=250)
 
         xlim = (xys[keypoint_ix,0]-crop_size/2,xys[keypoint_ix,0]+crop_size/2)
         ylim = (xys[keypoint_ix,1]-crop_size/2,xys[keypoint_ix,1]+crop_size/2)
          
         edge_data = ((),(),())
         if len(edges)>0: 
@@ -289,15 +289,16 @@
 
                     
         sizes = np.where(np.arange(len(xys))==keypoint_ix, 10, 6)[masked_nodes]
         masked_bodyparts = [bodyparts[i] for i in masked_nodes]
         nodes = hv.Nodes((*xys[masked_nodes].T, masked_nodes, masked_bodyparts, sizes), vdims=['name','size'])        
         graph = hv.Graph((edge_data, nodes), vdims='ecolor').opts(
             node_color='name', node_cmap=keypoint_colormap, tools=[],
-            edge_color='ecolor', edge_cmap=keypoint_colormap, node_size='size')
+            edge_color='ecolor', edge_cmap=keypoint_colormap, 
+            node_size='size',  invert_yaxis=True)
 
         return (rgb*graph*hv_point).opts(data_aspect=1, xlim=xlim, ylim=ylim, toolbar=None)
     
     
     def update_estimator_text(*, slope, intercept, conf_threshold):
         lines = [f'slope: {slope:.6f}',
                  f'intercept: {intercept:.6f}',
```

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.0/keypoint_moseq/fitting.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         
     history[iteration] = model_snapshot
     return history
 
 
 def _wrapped_resample(data, model, pbar=None, **resample_options):
     try: 
-        resample_model(data, **model, **resample_options)
+        model = resample_model(data, **model, **resample_options)
     except KeyboardInterrupt: 
         print('Early termination of fitting: user interruption')
         raise StopResampling()
 
     any_nans, nan_info, messages = check_for_nans(model)
     
     if any_nans:
@@ -173,30 +173,33 @@
         if not os.path.exists(savedir): os.makedirs(savedir)
         print(fill(f'Outputs will be saved to {savedir}'))
 
     if history is None: history = {}
 
     with tqdm.trange(start_iter, num_iters+1) as pbar:
         for iteration in pbar:
+
+            try: model = _wrapped_resample(
+                data, model, pbar=pbar, ar_only=ar_only, verbose=verbose)
+            except StopResampling: break
+
             if history_every_n_iters>0 and (iteration%history_every_n_iters)==0:
                 history = _update_history(history, iteration, model, 
                                         include_states=states_in_history)
                 
             if plot_every_n_iters>0 and (iteration%plot_every_n_iters)==0:
                 plot_progress(model, data, history, iteration, name=name, 
                             savefig=save_progress_figs, project_dir=project_dir)
 
             if save_every_n_iters>0 and (iteration%save_every_n_iters)==0:
                 save_checkpoint(model, data, history, labels, iteration, name=name,
                                 project_dir=project_dir,save_history=save_history, 
                                 save_states=save_states, save_data=save_data)
                 
-            try: model = _wrapped_resample(
-                data, model, pbar=pbar, ar_only=ar_only, verbose=verbose)
-            except StopResampling: break
+
 
     return model, history, name
     
     
 def resume_fitting(*, params, hypparams, labels, iteration, mask, num_iters,
                    Y, conf, seed, noise_prior=None, states=None, **kwargs):
     """Resume fitting a model from a checkpoint."""
@@ -206,28 +209,20 @@
     model = init_model(data, states, params, hypparams,
                        noise_prior, seed, **kwargs)
 
     return fit_model(model, data, labels, start_iter=iteration+1, 
                      num_iters=num_iters, **kwargs)
 
 
-def apply_model(*, params, coordinates, confidences=None, num_iters=5, 
-                use_saved_states=True, states=None, mask=None, labels=None, 
-                noise_prior=None, ar_only=False, save_results=True, verbose=False,
-                project_dir=None, name=None, results_path=None, **kwargs): 
-    """
-    Apply a model to data.
 
-    There are two scenarios for applying this function:
-        - The model is being applied to the same data it was fit to.
-            This would useful if the the data was chunked into segments
-            to allow parallelization during fitting. In this case,
-            set `use_saved_states=True` and provide `states`.
-        - The model is being applied to new data. In this case,
-            set `use_saved_states=False`.
+def extract_results(*, params, states, labels, save_results=True, 
+                    project_dir=None, name=None, results_path=None, 
+                    **kwargs): 
+    """
+    Extract model outputs and [optionally] save them to disk.
 
     Model outputs are saved to disk as a .h5 file, either at `results_path`
     if it is specified, or at `{project_dir}/{name}/results.h5` if it is not.
     If a .h5 file with the given path already exists, the outputs will be added
     to it. The results have the following structure::
 
         results.h5
@@ -241,55 +236,24 @@
         ⋮
 
     Parameters
     ----------
     params : dict
         Model parameters.
 
-    coordinates: dict
-        Dictionary mapping filenames to keypoint coordinates as ndarrays
-        of shape (n_frames, n_bodyparts, 2)
-
-    confidences: dict, default=None
-        Dictionary mapping filenames to keypoint confidences as ndarrays
-        of shape (n_frames, n_bodyparts)
-
-    num_iters : int, default=5
-        Number of iterations to run the model. We recommend 5 iterations
-        for data the model has already been fit to, and a higher number
-        (e.g. 10-20) for new data.
-
-    use_saved_states : bool, default=True
-        If True, and `states` is provided, the model will be initialized
-        with the saved states. 
-
     states : dict, default=None
         Dictionary of saved states. 
 
-    mask: ndarray, default=None
-        Binary mask indicating areas of padding in `states`
-        (see :py:func:`keypoint_moseq.util.batch`).
-
     labels: list
-        Row labels `states`
+        Row labels for `states`
         (see :py:func:`keypoint_moseq.util.batch`).
 
-    noise_prior : ndarray, default=None
-        Prior on the noise for each observation. Should be the same shape
-        as `states['s']`.
-
-    ar_only : bool, default=False
-        See :py:func:`keypoint_moseq.fitting.fit_model`.
-
     save_results : bool, default=True
         If True, the model outputs will be saved to disk.
-
-    verbose : bool, default=False
-        Whether to print progress updates.
-
+        
     project_dir : str, default=None
         Path to the project directory. Required if `save_results=True`
         and `results_path=None`.
 
     name : str, default=None
         Name of the model. Required if `save_results=True`
         and `results_path=None`.
@@ -299,84 +263,127 @@
 
     Returns
     -------
     results_dict : dict
         Dictionary of model outputs with the same structure as the
         results `.h5` file.
     """
-    
-    kwargs['seg_length'] = None # dont separate the data into segments
-    
-    data, new_labels = format_data(
-        coordinates, confidences=confidences, **kwargs)
-    session_names = [key for key,start,end in new_labels]
-
     if save_results:
         if results_path is None: 
             assert project_dir is not None and name is not None, fill(
                 'The `save_results` option requires either a `results_path` '
                 'or the `project_dir` and `name` arguments')
             results_path = os.path.join(project_dir,name,'results.h5')
-     
-    if use_saved_states:
-        assert not (states is None or mask is None or labels is None), fill(
-            'The `use_saved_states` option requires the additional '
-            'arguments `states`, `mask` and `labels`')   
-        
-        if noise_prior is not None:
-            noise_prior = batch(unbatch(noise_prior, labels), keys=session_names)[0]
-            noise_prior = np.where(data['mask'][...,None], noise_prior, 1) 
-            
-        new_states = {}
-        for k,v in jax.device_get(states).items():
-            padding = mask.shape[1] - v.shape[1]
-            v = pad_along_axis(v, (padding, 0), axis=1, value=1)
-            v = batch(unbatch(v, labels), keys=session_names)[0]
-            new_states[k] = v[:,padding:]
-        states = new_states
-        
-    else: 
-        states = None
-        noise_prior = None
-    
-    model = init_model(data, states, params, noise_prior=noise_prior, verbose=verbose, **kwargs)
-    
-    if num_iters>0:
-        with tqdm.trange(num_iters, desc='Applying model') as pbar:
-            for iteration in pbar:
-                try: model = _wrapped_resample(
-                        data, model, pbar=pbar, ar_only=ar_only, 
-                        states_only=True, verbose=verbose)
-                except StopResampling: break
-
 
-    nlags = model['hypparams']['ar_hypparams']['nlags']
-    states = jax.device_get(model['states'])                     
-    estimated_coords = jax.device_get(estimate_coordinates(
-        **model['states'], **model['params'], **data))
-    z_reindexed = reindex_by_frequency(states['z'], np.array(data['mask']))
+    # estimate keypoint coords from latent state, centroid and heading
+    estimated_coords = jax.device_get(estimate_coordinates(**states, **params))
+    states = jax.device_get(states)
+    
+    # extract syllables; repeat first syllable an extra `nlags` times
+    nlags = states['x'].shape[1] - states['z'].shape[1]
+    lagged_labels = [(key,start+nlags,end) for key,start,end in labels]
+    syllables = unbatch(states['z'], lagged_labels)
+    syllables = {k: np.pad(z[nlags:], (nlags,0), mode='edge') for k,z in syllables.items()}
+    syllables_reindexed = reindex_by_frequency(syllables)
+    
+    # extract estimated coords, latent state, centroid, and heading
+    estimated_coords = unbatch(estimated_coords, labels)
+    latent_state = unbatch(states['x'], labels)
+    centroid = unbatch(states['v'], labels)
+    heading = unbatch(states['h'], labels)
 
-    
     results_dict = {
         session_name : {
-            'syllables' : np.pad(states['z'][i], (nlags,0), mode='edge')[m>0],
-            'syllables_reindexed' : np.pad(z_reindexed[i], (nlags,0), mode='edge')[m>0],
-            'estimated_coordinates' : estimated_coords[i][m>0],
-            'latent_state' : states['x'][i][m>0],
-            'centroid' : states['v'][i][m>0],
-            'heading' : states['h'][i][m>0],
-        } for i,(m,session_name) in enumerate(zip(data['mask'],session_names))}
+            'syllables' : syllables[session_name],
+            'syllables_reindexed' : syllables_reindexed[session_name],
+            'estimated_coordinates' : estimated_coords[session_name],
+            'latent_state' : latent_state[session_name],
+            'centroid' : centroid[session_name],
+            'heading' : heading[session_name]
+        } for session_name in syllables.keys()}
     
     if save_results: 
         save_hdf5(results_path, results_dict)
         print(fill(f'Saved results to {results_path}'))
         
     return results_dict
 
 
+def apply_model(*, params, coordinates, confidences=None, num_iters=20, 
+                ar_only=False, save_results=True, verbose=False,
+                project_dir=None, name=None, results_path=None, **kwargs): 
+    """
+    Apply a model to new data.
+
+    Parameters
+    ----------
+    params : dict
+        Model parameters.
+
+    coordinates: dict
+        Dictionary mapping filenames to keypoint coordinates as ndarrays
+        of shape (n_frames, n_bodyparts, 2)
+
+    confidences: dict, default=None
+        Dictionary mapping filenames to keypoint confidences as ndarrays
+        of shape (n_frames, n_bodyparts)
+
+    num_iters : int, default=20
+        Number of iterations to run the model. 
+
+    ar_only : bool, default=False
+        See :py:func:`keypoint_moseq.fitting.fit_model`.
+
+    save_results : bool, default=True
+        If True, the model outputs will be saved to disk (see 
+        :py:func:`keypoint_moseq.fitting.extract_results` for
+        the output format).
+
+    verbose : bool, default=False
+        Whether to print progress updates.
+
+    project_dir : str, default=None
+        Path to the project directory. Required if `save_results=True`
+        and `results_path=None`.
+
+    name : str, default=None
+        Name of the model. Required if `save_results=True`
+        and `results_path=None`.
+
+    results_path : str, default=None
+        Optional path for saving model outputs.
+
+    Returns
+    -------
+    results_dict : dict
+        Dictionary of model outputs (for results format, see
+        :py:func:`keypoint_moseq.fitting.extract_results`).
+    """
+    if save_results:
+        if results_path is None: 
+            assert project_dir is not None and name is not None, fill(
+                'The `save_results` option requires either a `results_path` '
+                'or the `project_dir` and `name` arguments')
+            results_path = os.path.join(project_dir,name,'results.h5')
+     
+    data, labels = format_data(coordinates, confidences=confidences, **kwargs)
+    model = init_model(data=data, params=params, verbose=verbose, **kwargs)
+
+    with tqdm.trange(num_iters, desc='Applying model') as pbar:
+        for iteration in pbar:
+            try: model = _wrapped_resample(
+                    data, model, pbar=pbar, ar_only=ar_only, 
+                    states_only=True, verbose=verbose)
+            except StopResampling: break
+
+    return extract_results(
+        **model, labels=labels, save_results=save_results, name=name,
+        project_dir=project_dir, results_path=results_path)
+
+
 def revert(checkpoint, iteration):
     """
     Revert a checkpoint to an earlier iteration.
 
     The checkpoint will revert to latest iteration stored in the 
     fitting history that is less than or equal to `iteration`.
     The model parameters, seed, and iteration number will be updated
```

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/io.py` & `keypoint-moseq-0.1.0/keypoint_moseq/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,22 @@
     kwargs
         Custom project settings.  
     """
     
     def _update_dict(new, original):
         return {k:new[k] if k in new else v for k,v in original.items()} 
     
-    hypperams = {k: _update_dict(kwargs,v) for k,v in {
+    hypperams = _update_dict(kwargs, {
         'error_estimator': {'slope':-.5, 'intercept':.25},
         'obs_hypparams': {'sigmasq_0':0.1, 'sigmasq_C':.1, 'nu_sigma':1e5, 'nu_s':5},
         'ar_hypparams': {'latent_dim': 10, 'nlags': 3, 'S_0_scale': 0.01, 'K_0_scale': 10.0},
         'trans_hypparams': {'num_states': 100, 'gamma': 1e3, 'alpha': 5.7, 'kappa': 1e6},
-        'cen_hypparams': {'sigmasq_loc': 0.5}
-    }.items()}
+        'cen_hypparams': {'sigmasq_loc': 0.5}})
+    
+    hypperams = {k : _update_dict(kwargs, v) for k,v in hypperams.items()}
 
     anatomy = _update_dict(kwargs, {
         'bodyparts': ['BODYPART1','BODYPART2','BODYPART3'],
         'use_bodyparts': ['BODYPART1','BODYPART2','BODYPART3'],
         'skeleton': [['BODYPART1','BODYPART2'], ['BODYPART2','BODYPART3']],
         'anterior_bodyparts': ['BODYPART1'],
         'posterior_bodyparts': ['BODYPART3']})
@@ -656,29 +657,31 @@
     if path is None: 
         assert project_dir is not None and name is not None, fill(
             '`name` and `project_dir` are required if no `path` is given.')
         path = os.path.join(project_dir,name,'results.h5')
     return load_hdf5(path)
 
 
-def _name_from_path(filepath, path_in_name, path_sep):
+def _name_from_path(filepath, path_in_name, path_sep, remove_extension):
     """
     Create a name from a filepath. Either return the name of the file
     (with the extension removed) or return the full filepath, where the
     path separators are replaced with `path_sep`.
     """
-    filepath = os.path.splitext(filepath)[0]
+    if remove_extension:
+        filepath = os.path.splitext(filepath)[0]
     if path_in_name:
         return filepath.replace(os.path.sep, path_sep)
     else:
         return os.path.basename(filepath)
 
 
 def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
-                            path_in_name=False, return_bodyparts=False):
+                            path_in_name=False, remove_extension=True, 
+                            return_bodyparts=False):
     """
     Load tracking results from deeplabcut csv or hdf5 files.
 
     Parameters
     ----------
     filepath_pattern: str or list of str
         Filepath pattern for a set of deeplabcut csv or hdf5 files, 
@@ -700,14 +703,18 @@
     path_sep: str, default='-'
         Separator to use when `path_in_name` is True. For example,
         if `path_sep` is `'-'`, then the tracking results from the
         file `/path/to/file.csv` will be named `path-to-file`. Using
         `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
+    remove_extension: bool, default=True
+        Whether to remove the file extension from the name of the tracking
+        results.
+
     return_bodyparts: bool, default=False
         Whether to return a list of bodypart names.
 
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
@@ -724,33 +731,37 @@
         filepath_pattern, ['.csv','.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No deeplabcut csv or hdf5 files found for {filepath_pattern}')
 
     coordinates,confidences = {},{}
     for filepath in tqdm.tqdm(filepaths, desc='Loading from deeplabcut'):
         try: 
-            name = _name_from_path(filepath, path_in_name, path_sep)
             ext = os.path.splitext(filepath)[1]
             if ext=='.h5': df = pd.read_hdf(filepath)
-            if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0)   
+            if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
+
             bodyparts = list(list(zip(*df.columns.to_list()))[1][::3])      
             arr = df.to_numpy().reshape(len(df), -1, 3)
+
+            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
             coordinates[name] = arr[:,:,:-1]
             confidences[name] = arr[:,:,-1]
+
         except Exception as e: 
             print(fill(f'Error loading {filepath}: {e}'))
     
     if return_bodyparts: 
         return coordinates,confidences,bodyparts
     else: return coordinates,confidences
 
 
 
 def load_sleap_results(filepath_pattern, recursive=True, path_sep='-',
-                       path_in_name=False, return_bodyparts=False):
+                       path_in_name=False, return_bodyparts=False,
+                       remove_extension=True):
     """
     Load keypoints from sleap hdf5 files.
 
     Parameters
     ----------
     filepath_pattern: str, default=None
         Filepath pattern for a set of sleap hdf5 files, or a list of 
@@ -772,14 +783,17 @@
     path_sep: str, default='-'
         Separator to use when `path_in_name` is True. For example,
         if `path_sep` is `'-'`, then the tracking results from the
         file `/path/to/file.csv` will be named `path-to-file`. Using
         `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
+    remove_extension: bool, default=True
+        Whether to remove the file extension from the name of the tracking
+        results.
     
     return_bodyparts: bool, default=False
         Whether to return a list of bodypart names.
 
     Returns
     -------
     coordinates: dict
@@ -797,15 +811,15 @@
         filepath_pattern, ['.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No sleap hdf5 files found for {filepath_pattern}.')
 
     coordinates,confidences = {},{}
     for filepath in tqdm.tqdm(filepaths, desc='Loading from sleap'):
         try: 
-            name = _name_from_path(filepath, path_in_name, path_sep)
+            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
             with h5py.File(filepath, 'r') as f:
                 coords = f['tracks'][()]
                 confs = f['point_scores'][()]
                 bodyparts = [name.decode('utf-8') for name in f['node_names']]
                 if coords.shape[0] == 1: 
                     coordinates[name] = coords[0].T
                     confidences[name] = confs[0].T
```

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/util.py` & `keypoint-moseq-0.1.0/keypoint_moseq/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,56 +125,72 @@
     """
     stateseq_flat = concatenate_stateseqs(stateseqs, mask=mask).astype(int)
     stateseq_padded = np.hstack([[-1],stateseq_flat,[-1]])
     changepoints = np.diff(stateseq_padded).nonzero()[0]
     return changepoints[1:]-changepoints[:-1]
 
 
-def get_frequencies(stateseqs, mask=None, num_states=None):
+def get_frequencies(stateseqs, mask=None, num_states=None, runlength=True):
     """
     Get state frequencies for a batch of state sequences. Each frame is
     counted separately. For a more detailed  description of the function 
     parameters, see :py:func:`keypoint_moseq.util.concatenate_stateseqs`
 
     Parameters
     ----------
     stateseqs: dict or ndarray of shape (..., t)
+
     mask: ndarray of shape (..., >=t), default=None
+
     num_states: int, default=None
         Number of different states. If None, the number of states will
         be set to `max(stateseqs)+1`.
 
+    runlength: bool, default=True
+        Whether to count frequency by the number of instances of each
+        state (True), or by the number of frames in each state (False).
+
     Returns
     -------
     frequencies: 1d array
-        Proportion of frames in each state across all state sequences
+        Frequency of each state across all state sequences
 
     Examples
     --------
     >>> stateseqs = {
         'name1': np.array([1, 1, 2, 2, 2, 3]),
-        'name2': np.array([0, 0, 0, 1])
-    }
-    >>> get_frequencies(stateseqs)
+        'name2': np.array([0, 0, 0, 1])}
+    >>> get_frequencies(stateseqs, runlength=True)
+    array([0.2, 0.4, 0.2, 0.2])
+    >>> get_frequencies(stateseqs, runlength=False)
     array([0.3, 0.3, 0.3, 0.1])
-
     """    
-    stateseq_flat = concatenate_stateseqs(stateseqs, mask=mask).astype(int)
-    return np.bincount(stateseq_flat, minlength=num_states)/len(stateseq_flat)
+    stateseq_flat = concatenate_stateseqs(
+        stateseqs, mask=mask).astype(int)
+    
+    if runlength:
+        state_onsets = np.pad(np.diff(stateseq_flat).nonzero()[0]+1, (1,0))
+        stateseq_flat = stateseq_flat[state_onsets]
+
+    counts = np.bincount(stateseq_flat, minlength=num_states)
+    frequencies = counts/counts.sum()
+    return frequencies
+
 
 def reindex_by_frequency(stateseqs, mask=None):
     """
     Reindex a sequence of syllables by frequency. The most frequent
     syllable will be assigned 0, the second most frequent 1, etc.
     For a more detailed  description of the function parameters, 
     see :py:func:`keypoint_moseq.util.concatenate_stateseqs`
 
     Parameters
     ----------
     stateseqs: dict or ndarray of shape (..., t)
+
     mask: ndarray of shape (..., >=t), default=None
 
     Returns
     -------
     stateseqs_reindexed: ndarray
         The reindexed state sequences in the same format as `stateseqs`
     """
@@ -215,14 +231,17 @@
             matches += list_files_with_exts(fp, ext_list, recursive=recursive)
         return sorted(set(matches))
     
     else:
         # make sure extensions all start with "." and are lowercase
         ext_list = ['.'+ext.strip('.').lower() for ext in ext_list]
         
+        if os.path.isdir(filepath_pattern):
+            filepath_pattern = os.path.join(filepath_pattern,'*')
+
         # find all matches (recursively)
         matches = glob.glob(filepath_pattern)
         if recursive:
             for match in list(matches):
                 matches += glob.glob(os.path.join(match, '**'), recursive=True)
 
         # filter matches by extension
@@ -715,16 +734,17 @@
     """
     Compute the filtered derivative of a signal along a given axis.
 
     When `ksize=3`, for example, the filtered derivative is
 
     .. math::
 
-        \dot{y_t} = \frac{1}{3}( x_{t+3}+x_{t+2}+x_{t+1}-x_{t-1}-x_{t-2}-x_{t-3})
+        \\dot{y_t} = \\frac{1}{3}( x_{t+3}+x_{t+2}+x_{t+1}-x_{t-1}-x_{t-2}-x_{t-3})
 
+        
     Parameters
     ----------
     Y_flat: ndarray
         The signal to differentiate
 
     ksize: int
         The size of the filter. Must be odd.
```

### Comparing `keypoint-moseq-0.0.5/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.0/keypoint_moseq/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 import logging
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.ndimage import gaussian_filter1d
 from vidio.read import OpenCVReader
 from textwrap import fill
+from PIL import Image
 plt.rcParams['figure.dpi'] = 100
 
 from keypoint_moseq.util import (
     get_edges, get_durations, get_frequencies, reindex_by_bodyparts,
     find_matching_videos, get_syllable_instances, sample_instances,
     filter_centroids_headings, get_trajectories, interpolate_keypoints,
     interpolate_along_axis
@@ -23,15 +24,14 @@
 # simple warning formatting
 warnings.formatwarning = lambda msg, *a: str(msg)
 
 # suppress warnings from imageio
 logging.getLogger().setLevel(logging.ERROR)
 
 
-
 def crop_image(image, centroid, crop_size):
     """
     Crop an image around a centroid.
 
     Parameters
     ----------
     image: ndarray of shape (height, width, 3)
@@ -267,15 +267,15 @@
     ax.set_title('Frequency distribution')
     ax.set_yticks([])
     return fig, ax
 
 
 def plot_duration_distribution(results=None, path=None, project_dir=None, 
                                name=None, use_reindexed=True, lim=None,
-                               num_bins=30, fps=None):
+                               num_bins=30, fps=None, show_median=True):
     """
     Plot a histogram showing the frequency of each syllable.
     
     Caller must provide a results dictionary, a path to a results .h5,
     or a project directory and model name, in which case the results are
     loaded from `{project_dir}/{name}/results.h5`.
 
@@ -303,14 +303,17 @@
 
     num_bins: int, default=30
         Number of bins in the histogram.
 
     fps: int, default=None
         Frames per second. Used to convert x-axis from frames to seconds.
 
+    show_median: bool, default=True
+        Whether to show the median duration as a vertical line.
+
     Returns
     -------
     fig : matplotlib.figure.Figure
         Figure containing the histogram.
     
     ax : matplotlib.axes.Axes
         Axes containing the histogram.
@@ -337,14 +340,15 @@
     fig, ax = plt.subplots()
     ax.hist(durations, range=(0,lim), bins=(int(lim/binsize)), density=True)
     ax.set_xlim([0,lim])
     ax.set_xlabel(xlabel)
     ax.set_ylabel('probability')
     ax.set_title('Duration distribution')
     ax.set_yticks([])
+    if show_median: ax.axvline(np.median(durations), color='k', linestyle='--')
     return fig, ax
         
 
 def plot_progress(model, data, history, iteration, path=None,
                   project_dir=None, name=None, savefig=True,
                   fig_size=None, seq_length=600, min_frequency=.001, 
                   min_histogram_length=10, **kwargs):
@@ -1050,14 +1054,24 @@
                 facecolor=fill_color, alpha=alpha, zorder=i*4+3, clip_on=False)
  
         if return_rasters:
             rasters.append(rasterize_figure(fig))          
 
     return fig,ax,rasters
 
+def save_gif(image_list, gif_filename, duration=0.5):
+    # Convert NumPy arrays to PIL Image objects
+    pil_images = [Image.fromarray(np.uint8(img)) for img in image_list]
+
+    # Save the PIL Images as an animated GIF
+    pil_images[0].save(gif_filename, save_all=True, append_images=pil_images[1:], 
+                       duration=int(duration*1000), loop=0)
+
+
+
 def generate_trajectory_plots(
     coordinates=None, results=None, output_dir=None, name=None, 
     project_dir=None, results_path=None, pre=5, post=15, 
     min_frequency=0.005, min_duration=3, use_reindexed=True, 
     use_estimated_coords=False, skeleton=[], bodyparts=None, 
     use_bodyparts=None, num_samples=40, keypoint_colormap='autumn',
     plot_options={}, sampling_options={'mode':'density'},
@@ -1273,17 +1287,17 @@
                     return_rasters=(save_gifs or save_mp4s),
                     **plot_options)
 
                 plt.savefig(os.path.join(output_dir, f'{title}{suffix}.pdf'))
                 plt.close(fig=fig)
 
                 if save_gifs:
-                    frame_duration = int(1000 * (pre+post) / len(rasters) / fps)
+                    frame_duration = (pre+post) / len(rasters) / fps
                     path = os.path.join(output_dir, f'{title}{suffix}.gif')
-                    imageio.mimsave(path, rasters, duration=frame_duration)
+                    save_gif(rasters, path, duration=frame_duration)
                 if save_mp4s:
                     use_fps = len(rasters)/(pre+post)*fps
                     path = os.path.join(output_dir, f'{title}{suffix}.mp4')
                     write_video_clip(rasters, path, fps=use_fps)
                     
 
         # grid plot
@@ -1292,17 +1306,17 @@
             return_rasters=(save_gifs or save_mp4s),
             **plot_options)
 
         plt.savefig(os.path.join(output_dir, f'all_trajectories{suffix}.pdf'))
         plt.show()
 
         if save_gifs:
-            frame_duration = int(1000 * (pre+post) / len(rasters) / fps)
+            frame_duration = (pre+post) / len(rasters) / fps
             path = os.path.join(output_dir, f'all_trajectories{suffix}.gif')
-            imageio.mimsave(path, rasters, duration=frame_duration)
+            save_gif(rasters, path, duration=frame_duration)
         if save_mp4s:
             use_fps = len(rasters)/(pre+post)*fps
             path = os.path.join(output_dir, f'all_trajectories{suffix}.mp4')
             write_video_clip(rasters, path, fps=use_fps)
```

