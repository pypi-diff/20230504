# Comparing `tmp/hsmm_mvpy-0.0.8b0.tar.gz` & `tmp/hsmm_mvpy-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.0.8b0.tar", last modified: Wed Nov  2 10:46:50 2022, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0a0.tar", last modified: Thu May  4 09:29:16 2023, max compression
```

## Comparing `hsmm_mvpy-0.0.8b0.tar` & `hsmm_mvpy-0.1.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.0.8b0/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20342 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    17964 2022-11-02 10:42:51.000000 hsmm_mvpy-0.0.8b0/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      850 2022-11-02 10:46:44.000000 hsmm_mvpy-0.0.8b0/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    28600 2022-10-25 07:53:16.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     4252 2022-08-31 19:18:34.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    29003 2022-11-01 15:35:11.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    18748 2022-11-02 10:11:21.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2022-11-02 10:46:50.457785 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20342 2022-11-02 10:46:50.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2022-11-02 10:46:50.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2022-11-02 10:46:50.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       80 2022-11-02 10:46:50.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2022-11-02 10:46:50.000000 hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0a0/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20167 2023-05-04 09:20:47.000000 hsmm_mvpy-0.1.0a0/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      825 2023-05-04 09:24:53.000000 hsmm_mvpy-0.1.0a0/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57128 2023-05-04 06:34:27.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     8910 2023-05-02 16:12:55.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    36660 2023-05-04 07:49:35.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20999 2023-05-03 22:23:27.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       66 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.0.8b0/LICENSE.md` & `hsmm_mvpy-0.1.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.0.8b0/PKG-INFO` & `hsmm_mvpy-0.1.0a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,36 @@
-Metadata-Version: 2.1
-Name: hsmm_mvpy
-Version: 0.0.8b0
-Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
-Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/GWeindel/hsmm_mvpy
-Project-URL: Bug Tracker, https://github.com/GWeindel/hsmm_mvpy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-HsMM-MVpy
+HMP
 ==========
 
-hsmm_mvpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+![](plots/general_illustration.png)
+
+hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
 As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
 - Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
 
 
 # Documentation
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
-    $ conda create -n hsmm 
-    $ conda activate hsmm
-    $ conda install pip #optional for windows machine
+    $ conda create -n hmp 
+    $ conda activate hmp
+    $ conda install pip #if not already installed
     $ pip install hsmm_mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
-    import hsmm_mvpy as hsmm
+    import hsmm_mvpy as hmp
 ```
 
 For the cutting edge version (not recommended) you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
@@ -99,354 +58,401 @@
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
 
-```python
-#Development only
-import sys
-sys.path.insert(0, "/home/gweindel/owncloud/projects/RUGUU/hsmm-mvpy/src")
-%load_ext autoreload
-%autoreload 2
-```
-
 
 ```python
-import os 
+## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
-from mne import channels
+from scipy.stats import gamma
 
-## Importing 
-import hsmm_mvpy as hsmm
+## Importing HMP
+import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
+
+
 ### Simulating data
 
 In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
-_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once_
+_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
-cpus = 4 # For multiprocessing, usually a good idea to use multiple CPus as long as you have enough RAM
-path = os.path.join('simulated/')#Where simulated data will go, create that folder if you don't have it where you're executing the code
-
-n_events = 30 #Number of trials to simulate
+cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
-sources = [['lateraloccipital-lh',5e-9, [np.random.gamma,2,50]],#One source = localization, acitvation amplitude and onset latencies
-           ['postcentral-lh', 5e-9, [np.random.gamma, 2, 30]],
-           ['posteriorcingulate-rh', 5e-9, [np.random.gamma, 2,80]],
-           ['postcentral-rh', 5e-9, [np.random.gamma, 2,110]],
-           ['postcentral-lh', 1e-20, [np.random.gamma, 2,65]]] #Equivalent to a response trigger as amplitude make it hardly visible
+n_trials = 50 #Number of trials to simulate
 
-max_trial_length = 3000 #length of a trial (ISI)
+##### Here we define the sources of the brain activity (bump) for each trial
+frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
+amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+shape = 2 #shape of the gamma distribution
+means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
+         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
-bump_frequency = 10. #Frequency of the simulated bumps
-file = 'dataset_tutorial' #Name of the file to save
-mne_path = os.path.join(path+file+'_raw.fif')
+sources = []
+for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
 
-raw, generating_events = simulations.simulate(sources, n_events, max_trial_length, cpus, bump_frequency, file, path, overwrite=False)
+# Function used to generate the data
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+#Recovering sampling frequency of the simulated dataset
+sfreq = simulations.simulation_sfreq()
+#load electrode position, specific to the simulations
+positions = simulations.simulation_positions()
 ```
 
-    Aligning file name to MNE's convention
-    Loading dataset_tutorial_raw.fif no new simulation performed
+    ./dataset_README_raw.fif exists no new simulation performed
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 0 and 5.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
+#Recovering the events to epoch the data (in the number of trials defined above)
+generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
-event_id = {'stimulus':0}
+event_id = {'stimulus':1}#trigger 1 = stimulus
 resp_id = {'response':resp_trigger}
-events = generating_events[(generating_events[:,2] == 0) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
+#Keeping only stimulus and response triggers
+events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
-raw.copy().pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events);
+#Visualising the raw simulated EEG data
+import mne
+raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
+raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
-    Removing projector <Projection | PCA-v1, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v2, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v3, active : True, n_channels : 102>
-    Using matplotlib as 2D backend.
-    Opening raw-browser...
-
-
-
-    
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
 ![png](README_files/README_7_1.png)
-    
 
 
 ### Recovering number of sources as well as actual by-trial variation
 
 To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-random_source_times = np.zeros((int(len(generating_events)/(number_of_sources+1)), number_of_sources))
-
-i,x = 1,0                  
-while x < len(random_source_times):
-    for j in np.arange(number_of_sources):#recovering the individual duration- of bump onset
-        random_source_times[x,j] = generating_events[i,0] - generating_events[i-1,0]
-        i += 1
-    i += 1
-    x += 1
+#Recover the actual time of the simulated bumps
+random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
+           (n_trials, number_of_sources))
 ```
 
 ## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_dat = hsmm.utils.read_mne_EEG(mne_path, event_id, resp_id, raw.info['sfreq'], events_provided=events, verbose=False)
+eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+            events_provided=events, verbose=False)
 
 ```
 
-    Processing participant simulated/dataset_tutorial_raw.fif
-    Reading 0 ... 104999  =      0.000 ...   174.819 secs...
-    Creating epochs based on following event ID :[0 5]
+    Processing participant ./dataset_README_raw.fif
+    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
+    Creating epochs based on following event ID :[1 6]
     N trials without response event: 0
     Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    30 RTs kept of 30 clean epochs
-    30 trials were retained for participant simulated/dataset_tutorial_raw.fif
+    50 RTs kept of 50 clean epochs
+    50 trials were retained for participant ./dataset_README_raw.fif
     End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
-print(eeg_dat)
-eeg_dat.sel(epochs=0,electrodes=['EEG 001','EEG 002','EEG 003']).plot.scatter(x='samples', y='data',hue='electrodes');
+print(eeg_data)
+eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 30, electrodes: 59, samples: 1387)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
     Coordinates:
-      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 21 22 23 24 25 26 27 28 29
+      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 ... 1381 1382 1383 1384 1385 1386
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.053e-06...
+        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
         event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
     Attributes:
         sfreq:    600.614990234375
+        offset:   0
 
 
 
     
 ![png](README_files/README_13_1.png)
     
 
 
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hsmm.utils.transform_data(eeg_dat.data, apply_standard=False, single=True, n_comp=5)
-
-hsmm_dat = hsmm.utils.stack_data(hsmm_dat)
+hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
 ```
 
 # Estimating an HsMM model
 
-We know that we generate from four sources so let's just try to recover those four sources by directly estimating a 4 bump model (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-init = hsmm.models.hsmm(hsmm_dat, sf=eeg_dat.sfreq, bump_width=50, cpus=cpus)#Initialization of the model
-bests = init.backward_estimation()
-selected = bests.sel(n_bumps=number_of_sources-1)
-```
-
-    Estimating all solutions for maximal number of bumps (9) with 0 random starting points
-    Estimating parameters for 9 bumps model with 0 random starting points
-    Likelihood of uninitialized parameters has been preferred over initialized model. Consider adding starting points?
-    Parameters estimated for 9 bumps model
-    Estimating all solutions for 8 number of bumps
-    Estimating all solutions for 7 number of bumps
-    Estimating all solutions for 6 number of bumps
-    Estimating all solutions for 5 number of bumps
-    Estimating all solutions for 4 number of bumps
-    Estimating all solutions for 3 number of bumps
-    Estimating all solutions for 2 number of bumps
-    Estimating all solutions for 1 number of bumps
+%%time
+init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
+estimates = init.fit(step=10, verbose=False)
+```
 
 
-### Visualizing results of the fit
+      0%|          | 0/360 [00:00<?, ?it/s]
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
 
+    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
+    Wall time: 646 ms
 
-```python
-bump_times_selected = init.bump_times(selected.eventprobs)#computing predicted bump times
 
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location using MNE
-electrodes_selected = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at estimated bump location
-```
+### Visualizing results of the fit
+
+In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hsmm.visu.plot_topo_timecourse```
+We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
-hsmm.visu.plot_topo_timecourse(electrodes_selected, bump_times_selected, positions, 
-                               bump_size=init.bump_width_samples, magnify=5, figsize=(12,2),
-                                time_step = 1,  times_to_display = np.mean(init.ends - init.starts))
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
+                               positions, init,#position of the electrodes and initialized model
+                               magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
+                               times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_22_0.png)
+![png](README_files/README_21_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
 
 As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_selected = init.bump_times(selected.eventprobs, mean=False)#computing predicted bump times
-
-ax = hsmm.visu.plot_latencies_average(bump_times_selected, init.bump_width_samples, 1, errs='std', times_to_display = np.mean(init.ends - init.starts))
+bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
+ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_24_0.png)
+![png](README_files/README_23_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of bump onsets:
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000))
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000), survival=True);
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
+
+
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+
+
+
+
     
-![png](README_files/README_26_0.png)
+![png](README_files/README_25_1.png)
     
 
 
 
     
-![png](README_files/README_26_1.png)
+![png](README_files/README_25_2.png)
     
 
 
 As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.sel(trial_x_participant=('S0', 0)), xlims=(0,1000))
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+                            xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot:xlabel='Time (in samples)', ylabel='p(event)'>
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_28_1.png)
+![png](README_files/README_27_1.png)
     
 
 
 This then shows the likeliest bump location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-plt.scatter(np.mean(random_source_times, axis=0), selected.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
-plt.xlabel('Estimated stage duration')
-plt.ylabel('Actual stage duration')
+plt.xlabel('Simulated stage duration')
+plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_31_0.png)
+![png](README_files/README_30_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
 ```python
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location
-electrodes = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at bump location
-
-hsmm.visu.plot_topo_timecourse(electrodes, init.bump_times(selected.eventprobs), positions,#inferring electrode location, 
-        bump_size=init.bump_width_samples, time_step = 1, magnify=4, figsize=(13,2), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_33_0.png)
+![png](README_files/README_32_0.png)
     
 
 
 We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
 
 
 ```python
-fig, ax= plt.subplots(number_of_sources-1,1, figsize=(5,3.5*number_of_sources))
+fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
-gen_bump_location = np.cumsum(random_source_times[:,:-1], axis=1)
-for bump in init.bump_times(selected.eventprobs, mean=False)[:,:number_of_sources-1].T:
-    sns.regplot(x=gen_bump_location[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--')
+
+for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_36_0.png)
+![png](README_files/README_35_0.png)
     
 
 
-We see that, to the exception of the first stage (a weird result currently under investigation). Every other stage gets nicely recovered evn on a by-trial basis!
+We see that every stage gets nicely recovered even on a by-trial basis!
+
+# Beyond summary statistics for EEG analysis
+
+Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+
+We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
+
+
+```python
+import seaborn as sns
+import pandas as pd
+
+data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
+fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
+
+for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
+                     ['darkgreen','darkred','darkblue']):
+    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
+
+plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
+plt.ylabel('Volt')
+plt.xlim(0,500)
+plt.ylim(-3e-6,3e-6);
+
+```
+
+
+    
+![png](README_files/README_38_0.png)
+    
+
+
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+
+
+```python
+BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+
+fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
+ax[0].set_ylabel('Volt')
+for stage in range(number_of_sources):
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 025',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkred')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 032',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
+    plt.xlim(0,100)
+```
+
+
+    
+![png](README_files/README_40_0.png)
+    
+
+
+In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+
 
 ### Follow-up
 
 For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of bumps (tutorial 2)
 - Test for the number of bumps that best explains the data (tutorial 3)
```

### Comparing `hsmm_mvpy-0.0.8b0/README.md` & `hsmm_mvpy-0.1.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,79 @@
-HsMM-MVpy
+Metadata-Version: 2.1
+Name: hsmm_mvpy
+Version: 0.1.0a0
+Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
+Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/GWeindel/hmp
+Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+HMP
 ==========
 
-hsmm_mvpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+![](plots/general_illustration.png)
+
+hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
 As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
 - Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
 
 
 # Documentation
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
-    $ conda create -n hsmm 
-    $ conda activate hsmm
-    $ conda install pip #optional for windows machine
+    $ conda create -n hmp 
+    $ conda activate hmp
+    $ conda install pip #if not already installed
     $ pip install hsmm_mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
-    import hsmm_mvpy as hsmm
+    import hsmm_mvpy as hmp
 ```
 
 For the cutting edge version (not recommended) you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
@@ -56,354 +101,401 @@
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
 
-```python
-#Development only
-import sys
-sys.path.insert(0, "/home/gweindel/owncloud/projects/RUGUU/hsmm-mvpy/src")
-%load_ext autoreload
-%autoreload 2
-```
-
 
 ```python
-import os 
+## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
-from mne import channels
+from scipy.stats import gamma
 
-## Importing 
-import hsmm_mvpy as hsmm
+## Importing HMP
+import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
+
+
 ### Simulating data
 
 In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
-_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once_
+_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
-cpus = 4 # For multiprocessing, usually a good idea to use multiple CPus as long as you have enough RAM
-path = os.path.join('simulated/')#Where simulated data will go, create that folder if you don't have it where you're executing the code
-
-n_events = 30 #Number of trials to simulate
+cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
-sources = [['lateraloccipital-lh',5e-9, [np.random.gamma,2,50]],#One source = localization, acitvation amplitude and onset latencies
-           ['postcentral-lh', 5e-9, [np.random.gamma, 2, 30]],
-           ['posteriorcingulate-rh', 5e-9, [np.random.gamma, 2,80]],
-           ['postcentral-rh', 5e-9, [np.random.gamma, 2,110]],
-           ['postcentral-lh', 1e-20, [np.random.gamma, 2,65]]] #Equivalent to a response trigger as amplitude make it hardly visible
+n_trials = 50 #Number of trials to simulate
 
-max_trial_length = 3000 #length of a trial (ISI)
+##### Here we define the sources of the brain activity (bump) for each trial
+frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
+amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+shape = 2 #shape of the gamma distribution
+means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
+         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
-bump_frequency = 10. #Frequency of the simulated bumps
-file = 'dataset_tutorial' #Name of the file to save
-mne_path = os.path.join(path+file+'_raw.fif')
+sources = []
+for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
 
-raw, generating_events = simulations.simulate(sources, n_events, max_trial_length, cpus, bump_frequency, file, path, overwrite=False)
+# Function used to generate the data
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+#Recovering sampling frequency of the simulated dataset
+sfreq = simulations.simulation_sfreq()
+#load electrode position, specific to the simulations
+positions = simulations.simulation_positions()
 ```
 
-    Aligning file name to MNE's convention
-    Loading dataset_tutorial_raw.fif no new simulation performed
+    ./dataset_README_raw.fif exists no new simulation performed
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 0 and 5.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
+#Recovering the events to epoch the data (in the number of trials defined above)
+generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
-event_id = {'stimulus':0}
+event_id = {'stimulus':1}#trigger 1 = stimulus
 resp_id = {'response':resp_trigger}
-events = generating_events[(generating_events[:,2] == 0) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
+#Keeping only stimulus and response triggers
+events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
-raw.copy().pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events);
+#Visualising the raw simulated EEG data
+import mne
+raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
+raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
-    Removing projector <Projection | PCA-v1, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v2, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v3, active : True, n_channels : 102>
-    Using matplotlib as 2D backend.
-    Opening raw-browser...
-
-
-
-    
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
 ![png](README_files/README_7_1.png)
-    
 
 
 ### Recovering number of sources as well as actual by-trial variation
 
 To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-random_source_times = np.zeros((int(len(generating_events)/(number_of_sources+1)), number_of_sources))
-
-i,x = 1,0                  
-while x < len(random_source_times):
-    for j in np.arange(number_of_sources):#recovering the individual duration- of bump onset
-        random_source_times[x,j] = generating_events[i,0] - generating_events[i-1,0]
-        i += 1
-    i += 1
-    x += 1
+#Recover the actual time of the simulated bumps
+random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
+           (n_trials, number_of_sources))
 ```
 
 ## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_dat = hsmm.utils.read_mne_EEG(mne_path, event_id, resp_id, raw.info['sfreq'], events_provided=events, verbose=False)
+eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+            events_provided=events, verbose=False)
 
 ```
 
-    Processing participant simulated/dataset_tutorial_raw.fif
-    Reading 0 ... 104999  =      0.000 ...   174.819 secs...
-    Creating epochs based on following event ID :[0 5]
+    Processing participant ./dataset_README_raw.fif
+    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
+    Creating epochs based on following event ID :[1 6]
     N trials without response event: 0
     Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    30 RTs kept of 30 clean epochs
-    30 trials were retained for participant simulated/dataset_tutorial_raw.fif
+    50 RTs kept of 50 clean epochs
+    50 trials were retained for participant ./dataset_README_raw.fif
     End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
-print(eeg_dat)
-eeg_dat.sel(epochs=0,electrodes=['EEG 001','EEG 002','EEG 003']).plot.scatter(x='samples', y='data',hue='electrodes');
+print(eeg_data)
+eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 30, electrodes: 59, samples: 1387)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
     Coordinates:
-      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 21 22 23 24 25 26 27 28 29
+      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 ... 1381 1382 1383 1384 1385 1386
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.053e-06...
+        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
         event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
     Attributes:
         sfreq:    600.614990234375
+        offset:   0
 
 
 
     
 ![png](README_files/README_13_1.png)
     
 
 
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hsmm.utils.transform_data(eeg_dat.data, apply_standard=False, single=True, n_comp=5)
-
-hsmm_dat = hsmm.utils.stack_data(hsmm_dat)
+hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
 ```
 
 # Estimating an HsMM model
 
-We know that we generate from four sources so let's just try to recover those four sources by directly estimating a 4 bump model (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-init = hsmm.models.hsmm(hsmm_dat, sf=eeg_dat.sfreq, bump_width=50, cpus=cpus)#Initialization of the model
-bests = init.backward_estimation()
-selected = bests.sel(n_bumps=number_of_sources-1)
-```
-
-    Estimating all solutions for maximal number of bumps (9) with 0 random starting points
-    Estimating parameters for 9 bumps model with 0 random starting points
-    Likelihood of uninitialized parameters has been preferred over initialized model. Consider adding starting points?
-    Parameters estimated for 9 bumps model
-    Estimating all solutions for 8 number of bumps
-    Estimating all solutions for 7 number of bumps
-    Estimating all solutions for 6 number of bumps
-    Estimating all solutions for 5 number of bumps
-    Estimating all solutions for 4 number of bumps
-    Estimating all solutions for 3 number of bumps
-    Estimating all solutions for 2 number of bumps
-    Estimating all solutions for 1 number of bumps
+%%time
+init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
+estimates = init.fit(step=10, verbose=False)
+```
 
 
-### Visualizing results of the fit
+      0%|          | 0/360 [00:00<?, ?it/s]
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
 
+    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
+    Wall time: 646 ms
 
-```python
-bump_times_selected = init.bump_times(selected.eventprobs)#computing predicted bump times
 
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location using MNE
-electrodes_selected = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at estimated bump location
-```
+### Visualizing results of the fit
+
+In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hsmm.visu.plot_topo_timecourse```
+We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
-hsmm.visu.plot_topo_timecourse(electrodes_selected, bump_times_selected, positions, 
-                               bump_size=init.bump_width_samples, magnify=5, figsize=(12,2),
-                                time_step = 1,  times_to_display = np.mean(init.ends - init.starts))
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
+                               positions, init,#position of the electrodes and initialized model
+                               magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
+                               times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_22_0.png)
+![png](README_files/README_21_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
 
 As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_selected = init.bump_times(selected.eventprobs, mean=False)#computing predicted bump times
-
-ax = hsmm.visu.plot_latencies_average(bump_times_selected, init.bump_width_samples, 1, errs='std', times_to_display = np.mean(init.ends - init.starts))
+bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
+ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_24_0.png)
+![png](README_files/README_23_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of bump onsets:
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000))
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000), survival=True);
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
+
+
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+
+
+
+
     
-![png](README_files/README_26_0.png)
+![png](README_files/README_25_1.png)
     
 
 
 
     
-![png](README_files/README_26_1.png)
+![png](README_files/README_25_2.png)
     
 
 
 As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.sel(trial_x_participant=('S0', 0)), xlims=(0,1000))
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+                            xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot:xlabel='Time (in samples)', ylabel='p(event)'>
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_28_1.png)
+![png](README_files/README_27_1.png)
     
 
 
 This then shows the likeliest bump location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-plt.scatter(np.mean(random_source_times, axis=0), selected.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
-plt.xlabel('Estimated stage duration')
-plt.ylabel('Actual stage duration')
+plt.xlabel('Simulated stage duration')
+plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_31_0.png)
+![png](README_files/README_30_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
 ```python
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location
-electrodes = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at bump location
-
-hsmm.visu.plot_topo_timecourse(electrodes, init.bump_times(selected.eventprobs), positions,#inferring electrode location, 
-        bump_size=init.bump_width_samples, time_step = 1, magnify=4, figsize=(13,2), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_33_0.png)
+![png](README_files/README_32_0.png)
     
 
 
 We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
 
 
 ```python
-fig, ax= plt.subplots(number_of_sources-1,1, figsize=(5,3.5*number_of_sources))
+fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
-gen_bump_location = np.cumsum(random_source_times[:,:-1], axis=1)
-for bump in init.bump_times(selected.eventprobs, mean=False)[:,:number_of_sources-1].T:
-    sns.regplot(x=gen_bump_location[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--')
+
+for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_36_0.png)
+![png](README_files/README_35_0.png)
     
 
 
-We see that, to the exception of the first stage (a weird result currently under investigation). Every other stage gets nicely recovered evn on a by-trial basis!
+We see that every stage gets nicely recovered even on a by-trial basis!
+
+# Beyond summary statistics for EEG analysis
+
+Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+
+We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
+
+
+```python
+import seaborn as sns
+import pandas as pd
+
+data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
+fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
+
+for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
+                     ['darkgreen','darkred','darkblue']):
+    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
+
+plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
+plt.ylabel('Volt')
+plt.xlim(0,500)
+plt.ylim(-3e-6,3e-6);
+
+```
+
+
+    
+![png](README_files/README_38_0.png)
+    
+
+
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+
+
+```python
+BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+
+fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
+ax[0].set_ylabel('Volt')
+for stage in range(number_of_sources):
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 025',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkred')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 032',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
+    plt.xlim(0,100)
+```
+
+
+    
+![png](README_files/README_40_0.png)
+    
+
+
+In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+
 
 ### Follow-up
 
 For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of bumps (tutorial 2)
 - Test for the number of bumps that best explains the data (tutorial 3)
```

### Comparing `hsmm_mvpy-0.0.8b0/pyproject.toml` & `hsmm_mvpy-0.1.0a0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.0.8-beta"
+version = "0.1.0-alpha"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies=["mne >=1.0.0",
-"numpy >=1.20",
-"xarray >=2022.3.0, <2022.6.0",
+"numpy",
+"xarray",
 "sklearn",
 "seaborn",
 "scipy",
-"netcdf4"]
+"netcdf4",
+"xskillscore"]
 
 [project.urls]
-"Homepage" = "https://github.com/GWeindel/hsmm_mvpy"
-"Bug Tracker" = "https://github.com/GWeindel/hsmm_mvpy/issues"
+"Homepage" = "https://github.com/GWeindel/hmp"
+"Bug Tracker" = "https://github.com/GWeindel/hmp/issues"
```

### Comparing `hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 import numpy as np
 import scipy.stats as stats
 import xarray as xr
 import multiprocessing as mp
 import itertools
 import warnings
+from warnings import warn, filterwarnings
 
-warnings.filterwarnings('ignore', 'Degrees of freedom <= 0 for slice.', )#weird warning, likely due to nan in xarray, not important but better fix it later  
 
-def read_mne_EEG(pfiles, event_id, resp_id, sfreq, subj_idx=None, events_provided=None, verbose=True,
-                 tmin=-.2, tmax=5, offset_after_resp = .1, high_pass=.5, \
+filterwarnings('ignore', 'Degrees of freedom <= 0 for slice.', )#weird warning, likely due to nan in xarray, not important but better fix it later  
+
+def read_mne_EEG(pfiles, event_id, resp_id, sfreq=None, subj_idx=None, events_provided=None, verbose=True,
+                 tmin=-.2, tmax=5, offset_after_resp = 0, high_pass=.5, pick_channels = 'eeg', baseline=(None, 0),\
                  low_pass = 30, upper_limit_RT=5, lower_limit_RT=0.001, reject_threshold=None):
     ''' 
     Reads EEG data format (.fif or .bdf) using MNE's integrated function .
     
     Notes: 
     - Only EEG data are selected (other channel types are discarded)
     - All times are expressed on the second scale.
@@ -57,19 +59,23 @@
     verbose : bool
         Whether to display MNE's message
     tmin : float
         Time taken before stimulus onset to compute baseline
     tmax : float
         Time taken after stimulus onset
     offset_after_resp : float
-        Time taken after onset of the response
-    low_pass : float154,
+        Time taken after onset of the response in seconds
+    low_pass : float
         Value of the low pass filter
     high_pass : float
         Value of the high pass filter
+    pick_channels: list 
+        'eeg' (default) to keep only EEG channels or  list of channel names to keep
+    baseline : tuple
+        Time values to compute the baseline and substract to epoch data (usually some time before stimulus onset)
     upper_limit_RT : float
         Upper limit for RTs. Longer RTs are discarded
     lower_limit_RT : float
         Lower limit for RTs. Shorter RTs are discarded
     reject_threshold : float
         Rejection threshold to apply when creating epochs, expressed in microvolt
     
@@ -93,42 +99,58 @@
         print(f'Processing participant {participant}')
         if '.fif' in participant:
             data = mne.io.read_raw_fif(participant, preload=False, verbose=verbose)
         elif '.bdf' in participant:
             data = mne.io.read_raw_bdf(participant, preload=False, verbose=verbose)
         else:
             raise ValueError(f'Unknown EEG file format for participant {participant}')
-        data.load_data()
-        data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)#Filtering out frequency outside range .5 and 30Hz, as study by Anderson et al.
         # Loading events (in our case one event = one trial)
+        if sfreq is None: 
+            sfreq = data.info['sfreq']
         if events_provided is None:
-            events = mne.find_events(data, verbose=verbose, min_duration = 1 / data.info['sfreq'])
+            try:
+                events = mne.find_events(data, verbose=verbose, min_duration = 1 / data.info['sfreq'])
+            except:
+                events = mne.events_from_annotations(data, verbose=verbose)
             if events[0,1] > 0:#bug from some stim channel, should be 0 otherwise indicates offset in the trggers
                 print(f'Correcting event values as trigger channel has offset {np.unique(events[:,1])}')
                 events[:,2] = events[:,2]-events[:,1]#correction on event value                
             events_values = np.concatenate([np.array([x for x in event_id.values()]), np.array([x for x in resp_id.values()])])
             events = np.array([list(x) for x in events if x[2] in events_values])#only keeps events with stim or response
         else:
             if len(np.shape(events_provided)) == 2:
                 events_provided = events_provided[np.newaxis]
             events = events_provided[y]
+
+        if isinstance(pick_channels, list):
+               try:
+                    data = data.pick_channels(pick_channels)
+               except:
+                    raise ValueError('incorrect electrode pick specified')
+        elif pick_channels == 'eeg':
+                data = data.pick_types(meg=False, eeg=True, stim=False, eog=False, misc=False, exclude='bads') 
+        else:
+             raise ValueError('incorrect electrode pick specified')
+    
+
+        data.load_data()
+        data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)#Filtering out frequency outside range .5 and 30Hz, as study by Anderson et al.
+
         if sfreq < data.info['sfreq']:#Downsampling
             print(f'Downsampling to {sfreq} Hz')
             data, events = data.resample(sfreq, events=events)#100 Hz is the standard used for previous applications of HsMM
         
         print(f'Creating epochs based on following event ID :{np.unique(events[:,2])}')
-        #Only pick eeg electrodes
-        picks = mne.pick_types(data.info, eeg=True, stim=False, eog=False, misc=False,
-                           exclude='bads') 
-        offset_after_resp_samples = int(offset_after_resp*tstep)
+            
+        offset_after_resp_samples = int(offset_after_resp/tstep)
         metadata, meta_events, event_id = mne.epochs.make_metadata(
             events=events, event_id= event_id,
             tmin=tmin, tmax=tmax, sfreq=data.info['sfreq'])
         epochs = mne.Epochs(data, meta_events, event_id, tmin, tmax, proj=False,
-                        picks=picks, baseline=(None, 0), preload=True,
+                        baseline=baseline, preload=True,
                         verbose=verbose,detrend=1, on_missing = 'warn', event_repeated='drop',
                         metadata=metadata, reject_by_annotation=True, reject=reject_threshold)
         data_epoch = epochs.get_data()
 
         valid_epochs_idx = [x for x in np.arange(len(epochs.drop_log)) if epochs.drop_log[x] == ()]
         correct_stim_timing  = np.array([list(x) for x in events if x[2] in event_id.values()])[valid_epochs_idx,0]
         stim_events = np.array([x for x in np.arange(len(events)) if events[x,0] in correct_stim_timing])
@@ -167,22 +189,22 @@
         while np.isnan(cropped_data_epoch[-1]).all():#Weird bug I guess it is perhps due to too long epoch?
             cropped_data_epoch = cropped_data_epoch[:-1]
             x += 1
         if x > 0:
             print(f'RTs > 0 longer than expected ({x})')
         print(f'{len(cropped_data_epoch)} trials were retained for participant {participant}')
         print(f'End sampling frequency is {sfreq} Hz')
-        epoch_data.append(hsmm_data_format(cropped_data_epoch, cropped_trigger, epochs.info['sfreq'], epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names))
+        epoch_data.append(hsmm_data_format(cropped_data_epoch, cropped_trigger, epochs.info['sfreq'], offset_after_resp_samples, epochs=[int(x) for x in epochs_idx], electrodes = epochs.ch_names))
         y += 1
         
     epoch_data = xr.concat(epoch_data, dim = xr.DataArray(subj_idx, dims='participant'),
                           fill_value={'event':'', 'data':np.nan})
     return epoch_data
 
-def parsing_epoched_eeg(data, rts, conditions, sfreq, start_time=0, offset_after_resp=0):
+def parsing_epoched_eeg(data, rts, conditions, sfreq, start_time=0, offset_after_resp=0.1):
     '''
     Function to parse epochs and crop them to start_time (usually stimulus onset so 0) up to the reaction time of the trial.
     The returned object is a xarray Dataset allowing further processing using built-in methods
 
     Importantly 
     1) if you are considering some lower or upper limit on the RTs you should replace values outside of these ranges
     by np.nan (e.g. rts[rts < 200] = np.nan) or 0
@@ -261,18 +283,18 @@
     j = 0
     for epoch in np.arange(len(data)):
         #Crops the epochs up to RT
         cropped_data_epoch[j,:,:rts[epoch]+offset_after_resp_samples] = \
         (data[epoch,:,:rts[epoch]+offset_after_resp_samples])
         j += 1
     print(f'Totaling {len(cropped_data_epoch)} valid trials')
-    data_xr = hsmm_data_format(cropped_data_epoch, conditions, sfreq, epochs=epochs, electrodes = electrode_columns)
+    data_xr = hsmm_data_format(cropped_data_epoch, conditions, sfreq, offset_after_resp_samples, epochs=epochs, electrodes = electrode_columns)
     return data_xr
 
-def hsmm_data_format(data, events, sfreq, participants=[], epochs=None, electrodes=None):
+def hsmm_data_format(data, events, sfreq, offset=0, participants=[], epochs=None, electrodes=None):
     '''
     Converting 3D matrix with dimensions (participant) * trials * electrodes * sample into xarray Dataset
     
     Parameters
     ----------
     data : ndarray
         4/3D matrix with dimensions (participant) * trials * electrodes * sample  
@@ -307,29 +329,29 @@
                     "event": (["epochs"], events),
                 },
                 coords={
                     "epochs" :epochs,
                     "electrodes":  electrodes,
                     "samples": np.arange(n_samples)
                 },
-                attrs={'sfreq':sfreq}
+                attrs={'sfreq':sfreq,'offset':offset}
                 )
     else:
         data = xr.Dataset(
                 {
                     "data": (['participant',"epochs", "electrodes", "samples"],data),
                     "event": (['participant',"epochs"], events),
                 },
                 coords={
                     'participant':participants,
                     "epochs" :epochs,
                     "electrodes":  electrodes,
                     "samples": np.arange(n_samples)
                 },
-                attrs={'sfreq':sfreq}
+                attrs={'sfreq':sfreq,'offset':offset}
                 )
     return data
 
 def standardize(x):
     '''
     Scaling variances to mean variance of the group
     '''
@@ -345,15 +367,46 @@
 
 def zscore(data):
     '''
     zscore of the data
     '''
     return (data - data.mean()) / data.std()
 
-def transform_data(data, subjects_variable="participant", apply_standard=True,  apply_zscore=True, method='pca', n_comp=None, single=False, return_weights=False):
+
+def stack_data(data, subjects_variable='participant', electrode_variable='component', single=False):
+    '''
+    Stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
+    with sample indexes starts and ends to delimitate the epochs.
+    
+    
+    Parameters
+    ----------
+    data : xarray
+        unstacked xarray data from transform_data() or anyother source yielding an xarray with dimensions 
+        [participant * epochs * samples * electrodes] 
+    subjects_variable : str
+        name of the dimension for subjects ID
+    single : bool 
+        Whether participant is unique (True) or a group of participant (False)
+    
+    Returns
+    -------
+    data : xarray.Dataset
+        xarray dataset [samples * electrodes]
+    '''    
+    if isinstance(data, (xr.DataArray,xr.Dataset)) and 'component' not in data.dims:
+        data = data.rename_dims({'electrodes':'component'})
+        print(data.participant)
+    if "participant" not in data.dims:
+        data = data.expand_dims("participant")
+    data = data.stack(all_samples=['participant','epochs',"samples"]).dropna(dim="all_samples")
+    return data #xr.Dataset({'data':data, 'durations':durations})
+    #return data, durations
+
+def transform_data(data, subjects_variable="participant", apply_standard=True,  apply_zscore=True, method='pca', n_comp=None, return_weights=False):
     '''
     Adapts EEG epoched data (in xarray format) to the expected data format for hsmms. 
     First this code can apply standardization of individual variances (if apply_standard=True).
     Second, a spatial PCA on the average variance-covariance matrix is performed (if method='pca', more methods in development)
     Third,stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
     Last, performs z-scoring on each epoch and for each principal component (PC)
     
@@ -370,53 +423,45 @@
     apply_zscore : bool 
         Whether to apply z-scoring
     method : str
         Method to apply, for now limited to 'pca'
     n_comp : int
         How many components to select from the PC space, if None plots the scree plot and a prompt requires user
         to specify how many PCs should be retained
-    single : bool 
-        Whether participant is unique (True) or a group of participant (False)
 
     Returns
     -------
     data : xarray.Dataset
         xarray dataset [n_samples * n_comp] data expressed in the PC space, ready for hsMM fit
     pca_data : xarray.Dataset
         loadings of the PCA, used to retrieve electrode space
     pca.explained_variance_ : ndarray
         explained variance for each component
     means : xarray.DataArray
         means of the electrodes before PCA/zscore
     '''
-    from sklearn.decomposition import PCA
-    #var = data.var(...)
-    if apply_standard and not single:
+    if apply_standard:
         mean_std = data.groupby(subjects_variable).std(dim=...).data.mean()
         data = data.assign(mean_std=mean_std.data)
         data = data.groupby(subjects_variable).map(standardize)
     if method == 'pca':
+        from sklearn.decomposition import PCA
         var_cov_matrices = []
-        # Computing cov matrices by trial and take the average of those
-        if not single:
-            for i,trial_dat in data.stack(trial=("participant", "epochs")).groupby('trial'):
-                var_cov_matrices.append(vcov_mat(trial_dat)) #Would be nice not to have a for loop but groupby.map seem to fal
-            var_cov_matrix = np.mean(var_cov_matrices,axis=0)
-        else:
-            for i,trial_dat in data.groupby('epochs'):
-                var_cov_matrices.append(vcov_mat(trial_dat)) #Would be nice not to have a for loop but groupby.map seem to fal
-            var_cov_matrix = np.mean(var_cov_matrices,axis=0)    
-
+        if isinstance(data, xr.Dataset):
+            data = data.data
+        for i,trial_dat in data.stack(trial=("participant", "epochs")).groupby('trial'):
+            var_cov_matrices.append(vcov_mat(trial_dat)) #Would be nice not to have a for loop but groupby.map seem to fal
+        var_cov_matrix = np.mean(var_cov_matrices,axis=0)
         # Performing spatial PCA on the average var-cov matrix
         if n_comp == None:
             import matplotlib.pyplot as plt
             n_comp = np.shape(var_cov_matrix)[0]-1
             fig, ax = plt.subplots(1,2, figsize=(.2*n_comp, 4))
             pca = PCA(n_components=n_comp, svd_solver='full')#selecting Principale components (PC)
-            pca_data = pca.fit_transform(var_cov_matrix)
+            pca_data = pca.fit_transform(var_cov_matrix.T)
             var = pca.transform(var_cov_matrix)
             var = np.var(var, axis=0)
             ax[0].plot(np.arange(pca.n_components)+1, var/np.sum(var),'.-')
             ax[0].set_ylabel('Normalized explained variance')
             ax[0].set_xlabel('Component')
             ax[1].plot(np.arange(pca.n_components)+1, np.cumsum(var/np.sum(var)),'.-')
             ax[1].set_ylabel('Cumulative normalized explained variance')
@@ -431,133 +476,202 @@
         
         #Rebuilding pca PCs as xarray to ease computation
         coords = dict(electrodes=("electrodes", data.coords["electrodes"].values),
                      component=("component", np.arange(n_comp)))
         pca_data = xr.DataArray(pca_data, dims=("electrodes","component"), coords=coords)
         means = data.groupby('electrodes').mean(...)
         data = data @ pca_data
-        if apply_zscore and not single:
-            data = data.stack(trial=[subjects_variable,'epochs','component']).groupby('trial').map(zscore).unstack()
-        elif apply_zscore and single :
-            data = data.stack(trial=['epochs','component']).groupby('trial').map(zscore).unstack()
-            for comp in data.component:
-                if data.sel(component=comp).std() > 0:#corner case in  (some) simulations
-                    data.sel(component=comp).groupby('epochs').map(zscore).unstack()
-                else:
-                    data.sel(component=comp)+ 1e-10
-        if return_weights:
-            return data, pca_data, pca.explained_variance_, means
-        else:
-            return data
+
+    elif method is None:
+        data = data.rename({'electrodes':'component'})
+        data['component'] = np.arange(len(data.component ))
+    if apply_zscore:
+        data = data.stack(trial=[subjects_variable,'epochs','component']).groupby('trial').map(zscore).unstack()
+    if stack_data:
+        data = stack_data(data)
+    if return_weights:
+        return data, pca_data, pca.explained_variance_, means
     else:
         return data
     
 
-def stack_data(data, subjects_variable='participant', electrode_variable='component', single=False):
+def LOOCV(data, subject, n_bumps, initial_fit, sfreq, bump_width=50):
     '''
-    Stacks the data going from format [participant * epochs * samples * electrodes] to [samples * electrodes]
-    with sample indexes starts and ends to delimitate the epochs.
+    Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
+    compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
+    using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
-    data : xarray
-        unstacked xarray data from transform_data() or anyother source yielding an xarray with dimensions 
-        [participant * epochs * samples * electrodes] 
-    subjects_variable : str
-        name of the dimension for subjects ID
-    single : bool 
-        Whether participant is unique (True) or a group of participant (False)
+    data : xarray.Dataset
+        xarray data from transform_data() 
+    subject : str
+        name of the subject to remove
+    n_bumps : int 
+        How many bumps in the model
+    initial_fit : xarray.Dataset
+        Fit of the model with the same number of bumps and all participants
+    sfreq : float
+        Sampling frequency of the data
+    bump_width : float
+        length of the bumps in milliseconds
     
     Returns
     -------
-    data : xarray.Dataset
-        xarray dataset [samples * electrodes]
-    '''    
-    if isinstance(data, (xr.DataArray,xr.Dataset)) and 'component' not in data.dims:
-        data = data.rename_dims({'electrodes':'component'})
-        print(data.participant)
-    if "participant" not in data.dims:
-        data = data.expand_dims("participant")
-    durations = data.isel(component=0).rename({'epochs':'trials', subjects_variable:'subjects'})\
-    .stack(trial_x_participant=['subjects','trials']).dropna(dim="trial_x_participant", how="all").\
-    groupby('trial_x_participant').count(dim="samples").cumsum()
-
-    #durations = data.isel(component=0).rename({'epochs':'trials', subjects_variable:'subjects'}).stack(trial=\
-    #   ['subjects','trials']).dropna(dim="trial", how='all').\
-    #   groupby('trial').count(dim="samples").cumsum().unstack()
-
-    data = data.stack(all_samples=[subjects_variable,'epochs',"samples"]).dropna(dim="all_samples")
-    return xr.Dataset({'data':data, 'durations':durations})
-    #return data, durations
-
-
+    likelihood : float
+        likelihood computed for the left-out participant
+    subject : str
+        name of the subject to remove
+    '''
+    # warn('This method is deprecated and will be removed in future version, use loocv() instead', DeprecationWarning, stacklevel=2) 
+    from hsmm_mvpy.models import hsmm
+    #Looping over possible number of bumps
+    subjects_idx = data.participant.values
+    likelihoods_loo = []
+    #Extracting data without left out subject
+    stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
+    #Fitting the HsMM using previous estimated parameters as initial parameters
+    model_loo = hsmm(stacked_loo, sfreq=sfreq, bump_width=bump_width)
+    fit = model_loo.fit_single(n_bumps, initial_fit.magnitudes.dropna('bump').values, initial_fit.parameters, 1, verbose=False)
+    #Evaluating likelihood for left out subject
+    #Extracting data of left out subject
+    stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
+    model_left_out = hsmm(stacked_left_out, sfreq=sfreq, bump_width=bump_width)
+    likelihood = model_left_out.estim_probs(fit.magnitudes.dropna('bump').values, fit.parameters, n_bumps,True)
+    return likelihood, subject
 
-def LOOCV(data, subject, n_bumps, initial_fit, sfreq, bump_width=50):
+def loocv_estimation(data, subject, sfreq, bump_width):
     '''
     Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray
         xarray data from transform_data() 
     subject : str
         name of the subject to remove
-    n_bumps : int 
-        How many bumps in the model
-    initial_fit : xarray
-        Fit of the model with the same number of bumps and all participants
     sfreq : float
         Sampling frequency of the data
     bump_width : float
         length of the bumps in milliseconds
     
     Returns
     -------
     likelihood : float
         likelihood computed for the left-out participant
     subject : str
         name of the subject to remove
     '''    
+    print(f'Leaving out participant #{subject}')
     from hsmm_mvpy.models import hsmm
     #Looping over possible number of bumps
     subjects_idx = data.participant.values
     likelihoods_loo = []
     #Extracting data without left out subject
     stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
     #Fitting the HsMM using previous estimated parameters as initial parameters
-    model_loo = hsmm(stacked_loo, sf=sfreq, bump_width=bump_width)
-    fit = model_loo.fit_single(n_bumps, initial_fit.magnitudes, initial_fit.parameters, 1, False, verbose=False)
-
+    model_loo = hsmm(stacked_loo, sfreq=sfreq, bump_width=bump_width, cpus=1)
+    parameters, magnitudes, likelihoods = model_loo.sliding_bump(verbose=False)
+    estimates = model_loo.iterative_fit(likelihoods=likelihoods, parameters=parameters, magnitudes=magnitudes)
     #Evaluating likelihood for left out subject
     #Extracting data of left out subject
     stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
-    model_left_out = hsmm(stacked_left_out, sf=sfreq, bump_width=bump_width)
-    likelihood = model_left_out.calc_EEG_50h(fit.magnitudes, fit.parameters, n_bumps,True)
-    return likelihood, subject
+    model_left_out = hsmm(stacked_left_out, sfreq=sfreq, bump_width=bump_width, cpus=1)
+    n_bumps = int(estimates.dropna('n_bumps',how='all').n_bumps.max())
+    for n_bump in range(1,n_bumps+1):
+        likelihoods_loo.append( model_left_out.calc_EEG_50h(estimates.sel(n_bumps=n_bump).magnitudes.dropna('bump').values, estimates.sel(n_bumps=n_bump).parameters.dropna('stage').values, n_bump, True))
+    return likelihoods_loo, subject
+
+def loocv(stacked_data,sfreq, max_bump, cpus=1, bump_width=50):
+    '''
+    Performs Leave-one-out cross validation, removes one participant from data, estimate n_bumps HsMM parameters, 
+    compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
+    using initial fit as starting points for magnitudes and parameters
+    
+    
+    Parameters
+    ----------
+    data : xarray.Dataset
+        xarray data from transform_data() 
+    initial_fit : xarray.Dataset
+        Fit of the model with the same number of bumps and all participants
+    sfreq : float
+        Sampling frequency of the data
+    bump_width : float
+        length of the bumps in milliseconds
+    
+    Returns
+    -------
+    loocv
+    '''
+    unstacked_data = stacked_data.unstack()
+    #Looping over possible number of bumps
+    participants = unstacked_data.participant.data
+    likelihoods_loo = []
+    loocv = []
+    if cpus>1:
+        import multiprocessing
+        with multiprocessing.Pool(processes=cpus) as pool:
+            loo = pool.starmap(loocv_estimation, 
+                zip(itertools.repeat(unstacked_data), participants, itertools.repeat(sfreq), itertools.repeat(bump_width)))
+        loocv.append(loo)
+    else:
+        loo = []
+        for participant in participants:
+            loo.append(loocv_estimation(unstacked_data, participant,sfreq, bump_width))
+        loocv.append(loo)
+    loocv_arr = np.tile(np.nan, (max_bump, len(participants)))
+    par_arr = np.repeat(np.nan, len(participants))
+    for idx, values in enumerate(loocv[0]):
+        par_arr[idx] = np.array(values[-1])
+        values = np.array(values[:-1][0])
+        loocv_arr[:len(values), idx] = values 
+    loocv = xr.DataArray(loocv_arr, coords={"n_bump":np.arange(1,max_bump+1),
+                                                           "participants":par_arr}, name="loo_likelihood")
+    return loocv
+
 
-def loocv_mp(init, unstacked_data, bests, cpus=2, verbose=True):
+def loocv_mp(init, stacked_data, bests, func=LOOCV, cpus=2, verbose=True):
+    '''
+    multiprocessing wrapper for LOOCV()
+    
+    Parameters
+    ----------
+    init : hsmm.model
+        initialized hsmm model
+    data : xarray.Dataset
+        xarray data from transform_data() , can also be a subset, e.g. based on conditions
+    bests : xarray.Dataset
+        Fit from all possible n bump solution
+    
+    Returns
+    -------
+    loocv
+    '''
+    # warn('This method is deprecated and will be removed in future version, use loocv() instead', DeprecationWarning, stacklevel=2) 
+    unstacked_data = stacked_data.unstack()
     import multiprocessing
     import itertools
     participants = unstacked_data.participant.data
     likelihoods_loo = []
     loocv = []
-    for n_bumps in np.arange(1, init.max_bumps+1):
+    for n_bumps in bests.n_bumps.values:
         if verbose:
             print(f'LOOCV for model with {n_bumps} bump(s)')
         with multiprocessing.Pool(processes=cpus) as pool:
-            loo = pool.starmap(LOOCV, 
+            loo = pool.starmap(func, 
                 zip(itertools.repeat(unstacked_data), participants, itertools.repeat(n_bumps), 
-                    itertools.repeat(bests.sel(n_bumps=n_bumps)), itertools.repeat(init.sf)))
+                    itertools.repeat(bests.sel(n_bumps=n_bumps)), itertools.repeat(init.sfreq)))
         loocv.append(loo)
 
-    loocv = xr.DataArray(np.array(loocv)[:,:,0].astype(np.float64), coords={"n_bump":np.arange(1,init.max_bumps+1),
+    loocv = xr.DataArray(np.array(loocv)[:,:,0].astype(np.float64), coords={"n_bump":np.arange(1,bests.n_bumps.max().values+1),
                                                            "participants":np.array(loocv)[0,:,1]}, name="loo_likelihood")
     return loocv
 
 def reconstruct(magnitudes, PCs, eigen, means):
     '''
     Reconstruct electrode activity from PCA
     
@@ -624,23 +738,84 @@
     '''
     Saves eventprobs to filename csv file
     '''
     eventprobs = eventprobs.unstack()
     eventprobs.to_dataframe().to_csv(filename)
     print(f"Saved at {filename}")
 
-# def download_sample_data():
-#     import urllib.request
+def event_times(data, times, electrode, stage):
+    '''
+    Event times parses the single trial EEG signal of a given electrode in a given stage, from bump onset to the next one. If requesting the last
+    stage it is defined as the onset of the last bump until the response of the participants.
+
+    Parameters
+    ----------
+    data : xr.Dataset
+        HsMM EEG data (untransformed but with trial and participant stacked)
+    times : xr.DataArray
+        Onset times as computed using onset_times()
+    electrode : str
+        Electrode to pick for the parsing of the signal
+    stage : float | ndarray
+        Which stage to parse the signal into
+
+    Returns
+    -------
+    brp_data : ndarray
+        Matrix with trial_x_participant * samples with sample dimension given by the maximum stage duration
+    '''
+
+    brp_data = np.tile(np.nan, (len(data.trial_x_participant), int(round(max(times.sel(bump=stage+1).data- times.sel(bump=stage).data)))+1))
+    i=0
+    for trial, trial_dat in data.groupby('trial_x_participant'):
+        trial_time = slice(times.sel(bump=stage, trial_x_participant=trial), \
+                                                 times.sel(bump=stage+1, trial_x_participant=trial))
+        trial_elec = trial_dat.sel(electrodes = electrode, samples=trial_time).squeeze()
+        try:
+            brp_data[i, :len(trial_elec)] = trial_elec
+        except:
+            brp_data[i, :1] = trial_elec
+            
+        i += 1
+
+    return brp_data    
     
+def condition_selection(hsmm_data, eeg_data, condition_string):
+    unstacked = hsmm_data.unstack().where(eeg_data.event.str.contains(condition_string),drop=True)
+    stacked = stack_data(unstacked)
+    return stacked
+
     
-#         with requests.get(url, stream=True) as r:
-#         with open(path, 'wb') as f:
-#             shutil.copyfileobj(r.raw, f)
-#     import zipfile
-#     filehandle, _ = urllib.request.urlretrieve(url)
-
-#     zip_file_object = zipfile.ZipFile(filehandle, 'r')
-#     first_file = zip_file_object.namelist()[0]
-#     file = zip_file_object.open(first_file)
-#     content = file.read()
+def participant_selection(hsmm_data, eeg_data, participant):
+    unstacked = hsmm_data.unstack().sel(participant = participant)
+    stacked = stack_data(unstacked)
+    return stacked
 
-# download(link.get("href"),'./fails_data', link.text)
+def bootstrapping(init, hsmm_data, general_run, positions, eeg_data, iterations, threshold=1, verbose=True, plots=True, cpus=1):
+    from hsmm_mvpy.models import hsmm
+    from hsmm_mvpy.visu import plot_topo_timecourse
+    import xskillscore as xs
+    fitted_mags = general_run.magnitudes.values[np.unique(np.where(np.isfinite(general_run.magnitudes))[0]),:]#remove NAs
+    mags_boot_mat = np.tile(np.nan, (iterations, init.compute_max_bumps(), init.n_dims))
+    pars_boot_mat = np.tile(np.nan, (iterations, init.compute_max_bumps()+1, 2))
+
+    for i in range(iterations):
+        bootstapped = xs.resample_iterations(hsmm_data.unstack(), iterations=1, dim='epochs')
+        hsmm_data_boot = stack_data(bootstapped.squeeze())
+        init_boot = hsmm(hsmm_data_boot, sfreq=eeg_data.sfreq, bump_width=50, cpus=15)
+        estimates_boot = init_boot.fit(verbose=verbose, threshold=1)
+        mags_boot_mat[i, :len(estimates_boot.magnitudes),:] = estimates_boot.magnitudes
+        pars_boot_mat[i, :len(estimates_boot.parameters),:] = estimates_boot.parameters
+        if plots:
+            plot_topo_timecourse(eeg_data, estimates_boot, positions, init_boot)
+
+    all_pars_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in pars_boot_mat]), 2))
+    all_mags_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in mags_boot_mat]), init.n_dims))
+    for iteration, _i in enumerate(zip(pars_boot_mat, mags_boot_mat)):
+        all_pars_aligned[iteration, :len(_i[0]), :] = _i[0]
+        all_mags_aligned[iteration, :len(_i[1]), :] = _i[1]
+
+    booted = xr.Dataset({'parameters': (('iteration', 'stage','parameter'), 
+                                 all_pars_aligned),
+                        'magnitudes': (('iteration', 'bump','component'), 
+                                 all_mags_aligned)})
+    return booted
```

### Comparing `hsmm_mvpy-0.0.8b0/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/visu.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 '''
 
 import matplotlib.pyplot as plt
 import numpy as np
 from itertools import cycle
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold']
 
-def plot_topo_timecourse(electrodes, times, channel_position, time_step=1, bump_size=50,
+def plot_topo_timecourse(electrodes, estimated, channel_position, init, time_step=1, ydim=None,
                         figsize=None, dpi=100, magnify=1, times_to_display=None, cmap='Spectral_r',
-                        ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=False, sensors=True):
+                        ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=False, 
+                        sensors=False, skip_electrodes_computation=False):
     '''
     Plotting the bump topologies at the average time of the end of the previous stage.
     
     Parameters
     ----------
-    electrodes : ndarray
-        a 2D or 3D matrix of electrode activity with electrodes and bump as dimension (+ eventually a varying dimension)
-    times : ndarray
-        a 1D or 2D matrix of times with bump as dimension
+    electrodes : ndarray | xr.Dataarray 
+        a 2D or 3D matrix of electrode activity with electrodes and bump as dimension (+ eventually a varying dimension) OR
+        the original EEG data in HsMM format
+    estimated : ndarray
+        a 1D or 2D matrix of times with bump as dimension OR directly the results from a fitted hsmm 
     channel_position : ndarray
         Either a 2D array with dimension electrode and [x,y] storing electrode location in meters or an info object from
         the mne package containning digit. points for electrode location
+    init : float
+        initialized HsMM object
     time_step : float
         What unit to multiply all the times with, if you want to go on the second or millisecond scale you can provide 
         1/sf or 1000/sf where sf is the sampling frequency of the data
-    bump_size : float
-        Display size of the bump in time unit given sampling frequency, if drawing a fitted object using hsmm_mvpy you 
-        can provide the bump_width_sample of fitted hsmm (e.g. init.bump_width_sample)
     figsize : list | tuple | ndarray
         Length and heigth of the matplotlib plot
     dpi : float
         DPI of the  matplotlib plot
     magnify : float
         How much should the bumps be enlarged, useful to zoom on topologies, providing any other value than 1 will 
         however change the displayed size of the bump
@@ -60,62 +61,83 @@
     ax : matplotlib.pyplot.ax
         if ax was specified otherwise returns the plot
     '''
     
     from mne.viz import plot_topomap
     from mpl_toolkits.axes_grid1.inset_locator import inset_axes
     return_ax = True
+    if times_to_display is None:
+        times_to_display = init.mean_d*time_step
+    if 'bump' in estimated:
+        #This is to keep backward compatibility but supplyng externally computed electrodes and times will probably be
+        # DEPRECATED
+        if ydim is None and 'n_bumps' in estimated.dims:
+            if estimated.n_bumps.count() > 1:
+                ydim = 'n_bumps'
+        if ydim is not None and not skip_electrodes_computation:
+            electrodes = init.compute_topologies(electrodes, estimated, init.bump_width_samples, ydim).data
+        elif not skip_electrodes_computation:
+            electrodes = init.compute_topologies(electrodes, estimated, init.bump_width_samples).data
+        electrodes[electrodes == 0] = np.nan
+        times = init.compute_times(init, estimated, mean=True).data
+    else:#assumes times already computed
+        times = estimated
+    if len(np.shape(electrodes)) == 2:
+        electrodes = electrodes[np.newaxis]
+    n_iter = np.shape(electrodes)[0]
     if isinstance(ax, bool):
-        if not figsize:
-            figzise = (12, 2)
+        if figsize == None:
+            figsize = (12, 1*n_iter)
         fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
         return_ax = False
-
-    bump_size = bump_size*time_step*magnify
+    bump_size = init.bump_width_samples*time_step*magnify
     yoffset =.25*magnify
     axes = []
-    if len(np.shape(electrodes)) == 2:
-           electrodes = electrodes[np.newaxis]
-    n_iter = np.shape(electrodes)[0]
     if n_iter == 1:
         times = [times]
     times = np.array(times, dtype=object)
     for iteration in np.arange(n_iter):
         times_iteration = times[iteration]*time_step
         electrodes_ = electrodes[iteration,:,:]
         n_bump = int(sum(np.isfinite(electrodes_[:,0])))
         electrodes_ = electrodes_[:n_bump,:]
         for bump in np.arange(n_bump):
+            # if np.sum(electrodes_[bump,:]) != 0:
             axes.append(ax.inset_axes([times_iteration[bump],iteration-yoffset,
-                                       bump_size/2,yoffset*2], transform=ax.transData))
+                                       (bump_size),yoffset*2], transform=ax.transData))
             plot_topomap(electrodes_[bump,:], channel_position, axes=axes[-1], show=False,
-                         cmap=cmap, vmin=vmin, vmax=vmax, sensors=sensors)
+                         cmap=cmap, vlim=(vmin, vmax), sensors=sensors)
     if isinstance(ylabels, dict):
         ax.set_yticks(np.arange(len(list(ylabels.values())[0])),
                       [str(x) for x in list(ylabels.values())[0]])
         ax.set_ylabel(str(list(ylabels.keys())[0]))
     else:
         ax.set_yticks([])
-    ax.spines['top'].set_visible(False)
-    ax.spines['right'].set_visible(False)
-    ax.set_ylim(0-yoffset, n_iter-1+yoffset)
+        ax.spines['left'].set_visible(False)
     __display_times(ax, times_to_display, 0, time_step, max_time, times)
-    if time_step == 1:
-        ax.set_xlabel('Time (in samples)')
-    else:
-        ax.set_xlabel('Time')
-    if title:
-        ax.set_title(title)
+    if not return_ax:
+        ax.spines['top'].set_visible(False)
+        ax.spines['right'].set_visible(False)
+        ax.set_ylim(0-yoffset, n_iter-1+yoffset)
+        if time_step == 1:
+            ax.set_xlabel('Time (in samples)')
+        else:
+            ax.set_xlabel('Time')
+        if title:
+            ax.set_title(title)
+        if np.any(max_time) == None and np.any(times_to_display) == None:
+            ax.set_xlim(0, np.nanmax(times)+np.nanmax(times)/10)
     if return_ax:
+        ax.set_ylim(0-yoffset, n_iter-1+yoffset)
         return ax
     else:
         plt.show()    
 
 
-def plot_LOOCV(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=False):
+def plot_LOOCV(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=False, mean=False):
     '''
     Plotting the LOOCV results
     
     Parameters
     ----------
     loocv_estimates : ndarray or xarra.DataArray
         results from a call to hsmm.utils.loocv()
@@ -138,42 +160,50 @@
     '''
     if pvals:
         if test == 'sign':
             from statsmodels.stats.descriptivestats import sign_test 
         elif test == 't-test':
             from scipy.stats import ttest_1samp
         else:
-            print('Expected  t-test argument')
+            raise ValueError('Expected sign or t-test argument to test parameter')
     if isinstance(ax, bool):
         fig, ax = plt.subplots(1,2, figsize=figsize)
         return_ax = False
     else:
         return_ax = True
-        
-    ax[0].errorbar(x=np.arange(loocv_estimates.n_bump.max())+1,y=np.mean(loocv_estimates.data,axis=1),yerr=np.std(loocv_estimates.data,axis=1)/np.sqrt(len(loocv_estimates.participants))*1.96,marker='o')
+    loocv_estimates = loocv_estimates.dropna('n_bump', how='all')
+    if mean:
+        alpha = .2#for the indiv plot
+        means = np.nanmean(loocv_estimates.data,axis=1)
+        ax[0].errorbar(x=np.arange(len(means))+1, y=means, \
+                 yerr= np.nanstd(loocv_estimates.data,axis=1)/np.sqrt(len(loocv_estimates.participants))*1.96, marker='o', color='k')
+    else:
+        alpha=1
     if indiv:
         for loo in loocv_estimates.T:
-            ax[0].plot(np.arange(loocv_estimates.n_bump.max())+1,loo, alpha=.2)
+            ax[0].plot(np.arange(loocv_estimates.n_bump.max())+1,loo, alpha=alpha)
     ax[0].set_ylabel('LOOCV Loglikelihood')
     ax[0].set_xlabel('Number of bumps')
     ax[0].set_xticks(ticks=np.arange(1,loocv_estimates.n_bump.max()+1))
-
+    total_sub = len(loocv_estimates.participants)
     diffs, diff_bin, labels = [],[],[]
     for n_bump in np.arange(2,loocv_estimates.n_bump.max()+1):
         diffs.append(loocv_estimates.sel(n_bump=n_bump).data - loocv_estimates.sel(n_bump=n_bump-1).data)
         diff_bin.append([1 for x in diffs[-1] if x > 0])
         labels.append(str(n_bump-1)+'->'+str(n_bump))
         if pvals:
             pvalues = []
             if test == 'sign':
-                pvalues.append((sign_test(diffs[-1])))
+                diff_tmp = np.array(diffs)
+                diff_tmp[np.isnan(diff_tmp)] = -np.inf 
+                pvalues.append((sign_test(diff_tmp[-1])))
             elif test == 't-test':
                 pvalues.append((ttest_1samp(diffs[-1], 0, alternative='greater')))
-            mean = np.mean(loocv_estimates.sel(n_bump=n_bump).data)
-            ax[0].text(x=n_bump-.5, y=mean+mean/10, s=str(np.sum(diff_bin[-1]))+'/'+str(len(diffs[-1]))+':'+str(np.around(pvalues[-1][-1],2)))
+            mean = np.nanmean(loocv_estimates.sel(n_bump=n_bump).data)
+            ax[1].text(x=n_bump-2, y=0, s=str(int(np.nansum(diff_bin[-1])))+'/'+str(len(diffs[-1]))+':'+str(np.around(pvalues[-1][-1],3)))
     ax[1].plot(diffs,'.-', alpha=.3)
     ax[1].set_xticks(ticks=np.arange(0,loocv_estimates.n_bump.max()-1), labels=labels)
     ax[1].hlines(0,0,len(np.arange(2,loocv_estimates.n_bump.max())),color='k')
     ax[1].set_ylabel('Change in likelihood')
     ax[1].set_xlabel('')
     if return_ax:
         return ax
@@ -225,15 +255,15 @@
         n_stages = len(time[-1][np.isfinite(time[-1])])
         colors = [next(cycol) for x in np.arange(n_stages)]
         for stage in np.arange(n_stages-1,-1,-1):
             colors.append(next(cycol))
             plt.barh(j+.02*stage, np.mean(time[:,stage]), color='w', edgecolor=colors[stage])
             if errs == 'ci':
                 errorbars = np.transpose([np.nanpercentile(bootstrap(time[:,stage]), q=[2.5,97.5])])
-                errorbars = np.abs(errorbars-np.mean(time[:,stage]))
+                errorbars = np.abs(errorbars-np.mean(time[:,stage].values))
             elif errs == 'std':
                 errorbars = np.std(time[:,stage])
             else:
                 print('Unknown errorbar type')
                 errorbars = np.repeat(0,2)
             plt.errorbar(np.mean(time[:,stage]), j+.02*stage, xerr=errorbars, 
                      color=colors[stage], fmt='none', capsize=10)
@@ -291,18 +321,18 @@
     return axs
 
 def __display_times(ax, times_to_display, yoffset, time_step, max_time, times):
     n_iter = len(times)
     times = np.asarray(times,dtype=object)
     if isinstance(times_to_display, (np.ndarray, np.generic)):
         if isinstance(times_to_display, np.ndarray):
-            ax.vlines(times_to_display*time_step, yoffset-.5, yoffset+1-.5, ls='--')
+            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+1.1, ls='--')
             ax.set_xlim(-1*time_step, max(times_to_display)*time_step+((max(times_to_display)*time_step)/15))
         else:
-            ax.vlines(times_to_display*time_step, yoffset-.5, yoffset+1-.5, ls='--')
+            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+1.1, ls='--')
             ax.set_xlim(-1*time_step, times_to_display*time_step+(times_to_display*time_step)/15)
     if max_time:
         ax.set_xlim(-1*time_step, max_time)
     return ax
 
 def plot_latencies_gamma(gammas, bump_width=0, time_step=1, labels=[''], colors=default_colors, 
                          figsize=False, times_to_display=None, max_time=None, kind='bar', legend=False):
@@ -354,15 +384,15 @@
         if kind=='bar':
             axs.bar(np.arange(n_stages)+1, time[:,0] *  time[:,1], color='w', edgecolor=colors)
         elif kind == 'point':
             axs.plot(np.arange(n_stages)+1, time[:,0] * time[:,1],'o-', label=labels[j], color=colors[j])
         j += 1
     #plt.xticks(np.arange(len(labels)),labels)
     #plt.xlim(0-1,j)
-    #__display_times(axs, mean_rt, np.arange(np.shape(gammas)[0]), time_step, max_time, gammas)
+    #__display_times(axs, mean_d, np.arange(np.shape(gammas)[0]), time_step, max_time, gammas)
     axs.set_ylabel('Stages durations (Gamma)')
     axs.set_xlabel('Stage number')
     # Hide the right and top spines
     axs.spines.right.set_visible(False)
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
@@ -440,8 +470,20 @@
     axs.spines.right.set_visible(False)
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     axs.xaxis.set_ticks_position('bottom')
     if legend:
         axs.legend()
-    return axs
+    return axs
+
+def plot_iterations(iterations, eeg_data, init, positions, dims):
+    from hsmm_mvpy.models import hsmm
+    for iteration in iterations.iteration[:-1]:
+        selected = init.fit_single(iterations.sel(iteration=iteration)[dims[0]].dropna(dim='bump').bump[-1].values+1,\
+            magnitudes = iterations.sel(iteration=iteration)[dims[0]].dropna(dim='bump'),\
+            parameters = iterations.sel(iteration=iteration)[dims[1]].dropna(dim='stage'),\
+            threshold=0, verbose=False)
+
+        #Visualizing
+        plot_topo_timecourse(eeg_data, selected, positions,  init, magnify=1, sensors=False)
+
```

### Comparing `hsmm_mvpy-0.0.8b0/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.0.8b0
+Version: 0.1.0a0
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -29,49 +29,51 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: Homepage, https://github.com/GWeindel/hsmm_mvpy
-Project-URL: Bug Tracker, https://github.com/GWeindel/hsmm_mvpy/issues
+Project-URL: Homepage, https://github.com/GWeindel/hmp
+Project-URL: Bug Tracker, https://github.com/GWeindel/hmp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-HsMM-MVpy
+HMP
 ==========
 
-hsmm_mvpy is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
+![](plots/general_illustration.png)
+
+hmp is an open-source Python package to estimate Hidden Semi-Markov Models in a Multivariate Pattern Analysis (HsMM-MVPA) of electro-encephalographic (EEG) data based on the method developed by Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)), Borst & Anderson ([2021](http://jelmerborst.nl/pubs/ACTR_HsMM_MVPA_BorstAnderson_preprint.pdf)) and Weindel, van Maanen & Borst (in preparation).
 
 As a summary of the method, an HsMM-MVPA analysis parses the EEG into a number of significant cognitive event (called bumps) separated by flat period reflecting the ongoing stage initiated by a bump. Hence any reaction time can then be described by the number of bumps and stage estimated using hsmm_mvpy. The important aspect of HsMM-MVPA is that it is a whole-brain analysis (or whole scalp analysis) that estimates the onset of cognitive events on a single-trial basis. This by-trial estimations allows you then to further dig into any aspect you are interested in the EEG (or MEG) signal:
 - Describing an experiment or a clinical sample in terms of processes detected in the EEG signal
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given bump and perform classical ERPs or time-freauency analysis based on the events that are the estimated bumps
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of events in the signal,...)
 
 
 # Documentation
 
 The package is available through *pip* with the command ```pip install hsmm_mvpy```. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
-    $ conda create -n hsmm 
-    $ conda activate hsmm
-    $ conda install pip #optional for windows machine
+    $ conda create -n hmp 
+    $ conda activate hmp
+    $ conda install pip #if not already installed
     $ pip install hsmm_mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
-    import hsmm_mvpy as hsmm
+    import hsmm_mvpy as hmp
 ```
 
 For the cutting edge version (not recommended) you can clone the repository using *git*
 
 Open a terminal and type:
 
     $ git clone https://github.com/gweindel/hsmm_mvpy.git
@@ -99,354 +101,401 @@
 The following section will quickly walk you through an example usage in simulated data (using [MNE](https://mne.tools/dev/auto_examples/simulation/index.html)'s simulation functions and tutorials)
 
 First we load the libraries necessary for the demo on simulated data
 
 ### Importing libraries
 
 
-```python
-#Development only
-import sys
-sys.path.insert(0, "/home/gweindel/owncloud/projects/RUGUU/hsmm-mvpy/src")
-%load_ext autoreload
-%autoreload 2
-```
-
 
 ```python
-import os 
+## Importing these packages is specific for this simulation case
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
-from mne import channels
+from scipy.stats import gamma
 
-## Importing 
-import hsmm_mvpy as hsmm
+## Importing HMP
+import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
+    <frozen importlib._bootstrap>:241: RuntimeWarning: scipy._lib.messagestream.MessageStream size changed, may indicate binary incompatibility. Expected 56 from C header, got 64 from PyObject
+
+
 ### Simulating data
 
 In the following code block we simulate 30 trials from four known sources, this is not code you would need for your own analysis except if you want to simulate and test properties of HsM models. All these four sources are defined by a localization, an activation amplitude and a distribution (here gamma with shape and scale parameters) for the onsets of the bumps on each trial. The simulation functions are based on the [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
-_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once_
+_If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
 ```python
-cpus = 4 # For multiprocessing, usually a good idea to use multiple CPus as long as you have enough RAM
-path = os.path.join('simulated/')#Where simulated data will go, create that folder if you don't have it where you're executing the code
+cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
-n_events = 30 #Number of trials to simulate
+n_trials = 50 #Number of trials to simulate
 
-sources = [['lateraloccipital-lh',5e-9, [np.random.gamma,2,50]],#One source = localization, acitvation amplitude and onset latencies
-           ['postcentral-lh', 5e-9, [np.random.gamma, 2, 30]],
-           ['posteriorcingulate-rh', 5e-9, [np.random.gamma, 2,80]],
-           ['postcentral-rh', 5e-9, [np.random.gamma, 2,110]],
-           ['postcentral-lh', 1e-20, [np.random.gamma, 2,65]]] #Equivalent to a response trigger as amplitude make it hardly visible
+##### Here we define the sources of the brain activity (bump) for each trial
+frequency = 10.#Frequency of the bump defining its duration, half-sine of 10Hz = 50ms
+amplitude = np.array([.1e-6,.1e-6,.1e-6,.1e-6,1e-20]) #Amplitude of the bump in Volt, defining signal to noise ratio
+shape = 2 #shape of the gamma distribution
+means = np.array([60,150, 200, 100, 80])/shape #Mean duration of the stages separating bumps, in ms
+names = ['bankssts-rh','posteriorcingulate-lh','parahippocampal-lh',\
+         'pericalcarine-rh','postcentral-lh']#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
-max_trial_length = 3000 #length of a trial (ISI)
+sources = []
+for source in zip(names, amplitude, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
+    sources.append([source[0], frequency, source[1], gamma(shape, scale=source[2])])
 
-bump_frequency = 10. #Frequency of the simulated bumps
-file = 'dataset_tutorial' #Name of the file to save
-mne_path = os.path.join(path+file+'_raw.fif')
-
-raw, generating_events = simulations.simulate(sources, n_events, max_trial_length, cpus, bump_frequency, file, path, overwrite=False)
+# Function used to generate the data
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', overwrite=False)
+#Recovering sampling frequency of the simulated dataset
+sfreq = simulations.simulation_sfreq()
+#load electrode position, specific to the simulations
+positions = simulations.simulation_positions()
 ```
 
-    Aligning file name to MNE's convention
-    Loading dataset_tutorial_raw.fif no new simulation performed
+    ./dataset_README_raw.fif exists no new simulation performed
 
 
 ### Creating the event structure and plotting the raw data
 
 
-To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 0 and 5.
+To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 0 signal the onset of the stimulus and 5 the onset of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
+#Recovering the events to epoch the data (in the number of trials defined above)
+generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
-event_id = {'stimulus':0}
+event_id = {'stimulus':1}#trigger 1 = stimulus
 resp_id = {'response':resp_trigger}
-events = generating_events[(generating_events[:,2] == 0) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
+#Keeping only stimulus and response triggers
+events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
-raw.copy().pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events);
+#Visualising the raw simulated EEG data
+import mne
+raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
+raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
 
-    Removing projector <Projection | PCA-v1, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v2, active : True, n_channels : 102>
-    Removing projector <Projection | PCA-v3, active : True, n_channels : 102>
-    Using matplotlib as 2D backend.
-    Opening raw-browser...
-
-
-
-    
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
 ![png](README_files/README_7_1.png)
-    
 
 
 ### Recovering number of sources as well as actual by-trial variation
 
 To compare the by-trial duration of bumps that we will estimate later on we first recover the actual number of sources used in the simulation as well as the actual by-trial variation in the onset of the bumps. Again with a typical dataset you wouldn't need that part as you ignore the ground truth
 
 
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
-random_source_times = np.zeros((int(len(generating_events)/(number_of_sources+1)), number_of_sources))
-
-i,x = 1,0                  
-while x < len(random_source_times):
-    for j in np.arange(number_of_sources):#recovering the individual duration- of bump onset
-        random_source_times[x,j] = generating_events[i,0] - generating_events[i-1,0]
-        i += 1
-    i += 1
-    x += 1
+#Recover the actual time of the simulated bumps
+random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
+           (n_trials, number_of_sources))
 ```
 
 ## Demo of the HsMM Code for a single participant in a single condition based on the simulated data
 
 First we read the EEG data as we would for a single participant:
 
 
 ```python
 # Reading the data
-eeg_dat = hsmm.utils.read_mne_EEG(mne_path, event_id, resp_id, raw.info['sfreq'], events_provided=events, verbose=False)
+eeg_data = hmp.utils.read_mne_EEG(file[0], event_id, resp_id, sfreq, 
+            events_provided=events, verbose=False)
 
 ```
 
-    Processing participant simulated/dataset_tutorial_raw.fif
-    Reading 0 ... 104999  =      0.000 ...   174.819 secs...
-    Creating epochs based on following event ID :[0 5]
+    Processing participant ./dataset_README_raw.fif
+    Reading 0 ... 142583  =      0.000 ...   237.395 secs...
+    Creating epochs based on following event ID :[1 6]
     N trials without response event: 0
     Applying reaction time trim to keep RTs between 0.001 and 5 seconds
-    30 RTs kept of 30 clean epochs
-    30 trials were retained for participant simulated/dataset_tutorial_raw.fif
+    50 RTs kept of 50 clean epochs
+    50 trials were retained for participant ./dataset_README_raw.fif
     End sampling frequency is 600.614990234375 Hz
 
 
 The package uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
 ```python
 #example of usage of xarray
-print(eeg_dat)
-eeg_dat.sel(epochs=0,electrodes=['EEG 001','EEG 002','EEG 003']).plot.scatter(x='samples', y='data',hue='electrodes');
+print(eeg_data)
+eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 30, electrodes: 59, samples: 1387)
+    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 843)
     Coordinates:
-      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 21 22 23 24 25 26 27 28 29
+      * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
       * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 ... 1381 1382 1383 1384 1385 1386
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 836 837 838 839 840 841 842
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 2.053e-06...
+        data         (participant, epochs, electrodes, samples) float64 2.469e-06...
         event        (participant, epochs) <U8 'stimulus' 'stimulus' ... 'stimulus'
     Attributes:
         sfreq:    600.614990234375
+        offset:   0
 
 
 
     
 ![png](README_files/README_13_1.png)
     
 
 
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
-hsmm_dat = hsmm.utils.transform_data(eeg_dat.data, apply_standard=False, single=True, n_comp=5)
-
-hsmm_dat = hsmm.utils.stack_data(hsmm_dat)
+hsmm_dat = hmp.utils.transform_data(eeg_data.data, apply_standard=False, n_comp=4)
 ```
 
 # Estimating an HsMM model
 
-We know that we generate from four sources so let's just try to recover those four sources by directly estimating a 4 bump model (see tutorial 2 for the explanation of the following cell)
+We can directly fit an HsMM model without giving any info on the number of bumps (see tutorial 2 for the explanation of the following cell)
 
 
 ```python
-init = hsmm.models.hsmm(hsmm_dat, sf=eeg_dat.sfreq, bump_width=50, cpus=cpus)#Initialization of the model
-bests = init.backward_estimation()
-selected = bests.sel(n_bumps=number_of_sources-1)
-```
-
-    Estimating all solutions for maximal number of bumps (9) with 0 random starting points
-    Estimating parameters for 9 bumps model with 0 random starting points
-    Likelihood of uninitialized parameters has been preferred over initialized model. Consider adding starting points?
-    Parameters estimated for 9 bumps model
-    Estimating all solutions for 8 number of bumps
-    Estimating all solutions for 7 number of bumps
-    Estimating all solutions for 6 number of bumps
-    Estimating all solutions for 5 number of bumps
-    Estimating all solutions for 4 number of bumps
-    Estimating all solutions for 3 number of bumps
-    Estimating all solutions for 2 number of bumps
-    Estimating all solutions for 1 number of bumps
+%%time
+init = hmp.models.hsmm(hsmm_dat, eeg_data, bump_width=50, cpus=cpus)#Initialization of the model
+estimates = init.fit(step=10, verbose=False)
+```
 
 
-### Visualizing results of the fit
+      0%|          | 0/360 [00:00<?, ?it/s]
 
-In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
 
+    CPU times: user 645 ms, sys: 1.6 ms, total: 647 ms
+    Wall time: 646 ms
 
-```python
-bump_times_selected = init.bump_times(selected.eventprobs)#computing predicted bump times
 
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location using MNE
-electrodes_selected = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at estimated bump location
-```
+### Visualizing results of the fit
 
-We can directly take a look to the topologies and latencies of the bumps by calling ```hsmm.visu.plot_topo_timecourse```
+In the previous cell we initiated an HsMM model looking for 50ms bumps in the EEG signal and parsing the EEG data into a signal with 4 bumps and 5 gamma distributed stages with a fixed shape of 2 and a scale estimated by stage. We can now inspect the results of the fit
+
+We can directly take a look to the topologies and latencies of the bumps by calling ```hmp.visu.plot_topo_timecourse```
 
 
 ```python
-hsmm.visu.plot_topo_timecourse(electrodes_selected, bump_times_selected, positions, 
-                               bump_size=init.bump_width_samples, magnify=5, figsize=(12,2),
-                                time_step = 1,  times_to_display = np.mean(init.ends - init.starts))
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
+                               positions, init,#position of the electrodes and initialized model
+                               magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
+                               times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
 
     
-![png](README_files/README_22_0.png)
+![png](README_files/README_21_0.png)
     
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the bump based on the stage distributions.
 
 As we are estimating the bump onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
 ```python
-bump_times_selected = init.bump_times(selected.eventprobs, mean=False)#computing predicted bump times
-
-ax = hsmm.visu.plot_latencies_average(bump_times_selected, init.bump_width_samples, 1, errs='std', times_to_display = np.mean(init.ends - init.starts))
+bump_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('bump')#computing predicted bump times
+ax = hmp.visu.plot_latencies_average(bump_times_estimates, init.bump_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
-![png](README_files/README_24_0.png)
+![png](README_files/README_23_0.png)
     
 
 
 For the same reason we can also inspect the probability distribution of bump onsets:
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000))
-hsmm.visu.plot_distribution(selected.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,1000), survival=True);
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
+hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
+
+
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+
+
+
+
     
-![png](README_files/README_26_0.png)
+![png](README_files/README_25_1.png)
     
 
 
 
     
-![png](README_files/README_26_1.png)
+![png](README_files/README_25_2.png)
     
 
 
 As HsMM-MVPA selected those bumps onset per trial we can also look at the predicted bump onsets for a single trial
 
 
 ```python
-hsmm.visu.plot_distribution(selected.eventprobs.sel(trial_x_participant=('S0', 0)), xlims=(0,1000))
+hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 1)), 
+                            xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot:xlabel='Time (in samples)', ylabel='p(event)'>
+    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
-![png](README_files/README_28_1.png)
+![png](README_files/README_27_1.png)
     
 
 
 This then shows the likeliest bump location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HsMM-MVpy. As in the beginning, this code is specific to the case where you simulate data.
 
 
 ```python
 colors = sns.color_palette(None, number_of_sources)
-plt.scatter(np.mean(random_source_times, axis=0), selected.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+# plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(params=1)*2+np.concatenate([[0],np.repeat(init.bump_width_samples,number_of_sources-1)]), color=colors,s=50)
+plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.dropna('stage').isel(parameter=1)*2, color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
-plt.xlabel('Estimated stage duration')
-plt.ylabel('Actual stage duration')
+plt.xlabel('Simulated stage duration')
+plt.ylabel('Estimated stage duration')
 plt.show()
 
 ```
 
 
     
-![png](README_files/README_31_0.png)
+![png](README_files/README_30_0.png)
     
 
 
 Or also overlay actual bumps onset with predicted one
 
 
 ```python
-positions = np.delete(channels.layout._find_topomap_coords(raw.info, 'eeg'),52,axis=0)#inferring electrode location
-electrodes = init.compute_topo(eeg_dat, selected.eventprobs)#Computing electrode activity at bump location
-
-hsmm.visu.plot_topo_timecourse(electrodes, init.bump_times(selected.eventprobs), positions,#inferring electrode location, 
-        bump_size=init.bump_width_samples, time_step = 1, magnify=4, figsize=(13,2), title='Actual vs estimated bump onsets',
+hmp.visu.plot_topo_timecourse(eeg_data, estimates, positions, init, magnify=1, sensors=False, figsize=(13,1), title='Actual vs estimated bump onsets',
         times_to_display = np.mean(np.cumsum(random_source_times,axis=1),axis=0))
 ```
 
 
     
-![png](README_files/README_33_0.png)
+![png](README_files/README_32_0.png)
     
 
 
 We see that the HsMM-MVpy package recovers the exact average location of the bumps defined in the simulated data
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HsMM model
 
 
 ```python
-fig, ax= plt.subplots(number_of_sources-1,1, figsize=(5,3.5*number_of_sources))
+fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
-gen_bump_location = np.cumsum(random_source_times[:,:-1], axis=1)
-for bump in init.bump_times(selected.eventprobs, mean=False)[:,:number_of_sources-1].T:
-    sns.regplot(x=gen_bump_location[:,i].T, y=bump, ax=ax[i], color=colors[i])
-    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--')
+
+for bump in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
+    sns.regplot(x=random_source_times[:,i].T, y=bump, ax=ax[i], color=colors[i])
+    ax[i].plot([np.min(bump), np.max(bump)], [np.min(bump), np.max(bump)],'--', color='k')
     ax[i].set_ylabel(f'Estimated by-trial stage duration for stage {i+1}')
     ax[i].set_xlabel(f'Simulated by-trial stage duration for stage {i+1}')
     i+= 1
 ```
 
 
     
-![png](README_files/README_36_0.png)
+![png](README_files/README_35_0.png)
     
 
 
-We see that, to the exception of the first stage (a weird result currently under investigation). Every other stage gets nicely recovered evn on a by-trial basis!
+We see that every stage gets nicely recovered even on a by-trial basis!
+
+# Beyond summary statistics for EEG analysis
+
+Now the purpose, apart from determining the number and timecourse of important EEG events in the Rreaction time, is also to use the by-trial information.
+
+We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
+
+
+```python
+import seaborn as sns
+import pandas as pd
+
+data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
+fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
+
+for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
+                     ['darkgreen','darkred','darkblue']):
+    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
+
+plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
+plt.ylabel('Volt')
+plt.xlim(0,500)
+plt.ylim(-3e-6,3e-6);
+
+```
+
+
+    
+![png](README_files/README_38_0.png)
+    
+
+
+Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is very close to trqditional ERPs with very clear signal in the beginning of a trial (as events are more in sync) and summed and blurried in later stages of the reaction times (as event are off sync).
+
+Now things can get better if we first parse, by-trial, the signal into the different stages based on the HsMM estimates:
+
+
+```python
+BRP_times = init.compute_times(init, estimates.dropna('bump'), fill_value=0, add_rt=True)
+
+fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
+ax[0].set_ylabel('Volt')
+for stage in range(number_of_sources):
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkgreen')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 025',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkred')
+    BRP = hmp.utils.event_times(data, BRP_times,'EEG 032',stage=stage)
+    df = pd.DataFrame(BRP).melt(var_name='Time')
+    sns.lineplot(x="Time", y="value", data=df,ax=ax[stage], color='darkblue') 
+    plt.xlim(0,100)
+```
+
+
+    
+![png](README_files/README_40_0.png)
+    
+
+
+In this case we clearly see at each stage the half-sin (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sin). Note that the end of the stages tend to be noisier because less trial are defining the average signal (also why the confidence interval grows).
+
 
 ### Follow-up
 
 For examples on how to use the package when the number of bumps are unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of bumps (tutorial 2)
 - Test for the number of bumps that best explains the data (tutorial 3)
```

