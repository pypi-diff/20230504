# Comparing `tmp/iDeLUCS-0.0.3.tar.gz` & `tmp/idelucs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iDeLUCS-0.0.3.tar", last modified: Thu Mar 23 21:35:35 2023, max compression
+gzip compressed data, was "idelucs-0.1.0.tar", last modified: Wed May  3 22:02:02 2023, max compression
```

## Comparing `iDeLUCS-0.0.3.tar` & `idelucs-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 shaneding   (501) staff       (20)        0 2023-03-23 21:35:35.190777 iDeLUCS-0.0.3/
--rw-r--r--   0 shaneding   (501) staff       (20)     1074 2023-03-09 01:20:17.000000 iDeLUCS-0.0.3/LICENCE.md
--rw-r--r--   0 shaneding   (501) staff       (20)      487 2023-03-23 21:35:35.190652 iDeLUCS-0.0.3/PKG-INFO
--rw-r--r--   0 shaneding   (501) staff       (20)     5274 2023-03-09 21:29:10.000000 iDeLUCS-0.0.3/README.md
-drwxr-xr-x   0 shaneding   (501) staff       (20)        0 2023-03-23 21:35:35.188376 iDeLUCS-0.0.3/iDeLUCS.egg-info/
--rw-r--r--   0 shaneding   (501) staff       (20)      487 2023-03-23 21:35:35.000000 iDeLUCS-0.0.3/iDeLUCS.egg-info/PKG-INFO
--rw-r--r--   0 shaneding   (501) staff       (20)      365 2023-03-23 21:35:35.000000 iDeLUCS-0.0.3/iDeLUCS.egg-info/SOURCES.txt
--rw-r--r--   0 shaneding   (501) staff       (20)        1 2023-03-23 21:35:35.000000 iDeLUCS-0.0.3/iDeLUCS.egg-info/dependency_links.txt
--rw-r--r--   0 shaneding   (501) staff       (20)       84 2023-03-23 21:35:35.000000 iDeLUCS-0.0.3/iDeLUCS.egg-info/requires.txt
--rw-r--r--   0 shaneding   (501) staff       (20)       16 2023-03-23 21:35:35.000000 iDeLUCS-0.0.3/iDeLUCS.egg-info/top_level.txt
--rw-r--r--   0 shaneding   (501) staff       (20)     8442 2023-03-23 21:05:51.000000 iDeLUCS-0.0.3/iDeLUCS.py
-drwxr-xr-x   0 shaneding   (501) staff       (20)        0 2023-03-23 21:35:35.190353 iDeLUCS-0.0.3/idelucs/
--rw-r--r--   0 shaneding   (501) staff       (20)     3104 2023-01-25 02:07:01.000000 iDeLUCS-0.0.3/idelucs/LossFunctions.py
--rw-r--r--   0 shaneding   (501) staff       (20)     2584 2023-01-25 02:07:01.000000 iDeLUCS-0.0.3/idelucs/PytorchUtils.py
--rw-r--r--   0 shaneding   (501) staff       (20)     7722 2023-03-09 01:20:17.000000 iDeLUCS-0.0.3/idelucs/ResNet.py
--rw-r--r--   0 shaneding   (501) staff       (20)        0 2023-03-23 21:07:06.000000 iDeLUCS-0.0.3/idelucs/__init__.py
--rw-r--r--   0 shaneding   (501) staff       (20)     2065 2023-03-16 00:15:47.000000 iDeLUCS-0.0.3/idelucs/kmers_non_cython.py
--rw-r--r--   0 shaneding   (501) staff       (20)     7650 2023-03-23 21:08:41.000000 iDeLUCS-0.0.3/idelucs/models.py
--rw-r--r--   0 shaneding   (501) staff       (20)    19569 2023-03-23 21:05:48.000000 iDeLUCS-0.0.3/idelucs/utils.py
--rw-r--r--   0 shaneding   (501) staff       (20)     2821 2023-01-25 02:07:01.000000 iDeLUCS-0.0.3/idelucs/utils_GUI.py
--rw-r--r--   0 shaneding   (501) staff       (20)       38 2023-03-23 21:35:35.190812 iDeLUCS-0.0.3/setup.cfg
--rw-r--r--   0 shaneding   (501) staff       (20)     1251 2023-03-23 21:34:22.000000 iDeLUCS-0.0.3/setup.py
+drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:02:02.797364 idelucs-0.1.0/
+-rw-rw-r--   0 loan      (1000) loan      (1000)      556 2023-05-03 22:02:02.793364 idelucs-0.1.0/PKG-INFO
+drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:02:02.793364 idelucs-0.1.0/idelucs/
+-rw-rw-r--   0 loan      (1000) loan      (1000)     3104 2022-09-27 18:27:35.000000 idelucs-0.1.0/idelucs/LossFunctions.py
+-rw-r-----   0 loan      (1000) loan      (1000)     2584 2023-04-13 16:42:44.000000 idelucs-0.1.0/idelucs/PytorchUtils.py
+-rw-r-----   0 loan      (1000) loan      (1000)     7524 2023-04-13 16:42:44.000000 idelucs-0.1.0/idelucs/ResNet.py
+-rw-rw-r--   0 loan      (1000) loan      (1000)      355 2023-05-01 17:45:48.000000 idelucs-0.1.0/idelucs/__init__.py
+-rw-r-----   0 loan      (1000) loan      (1000)    11548 2023-05-03 21:30:28.000000 idelucs-0.1.0/idelucs/__main__.py
+-rw-r-----   0 loan      (1000) loan      (1000)     6731 2023-05-03 21:33:54.000000 idelucs-0.1.0/idelucs/models.py
+-rw-r-----   0 loan      (1000) loan      (1000)    20627 2023-05-03 20:34:29.000000 idelucs-0.1.0/idelucs/utils.py
+-rw-r-----   0 loan      (1000) loan      (1000)     2949 2023-05-03 21:28:49.000000 idelucs-0.1.0/idelucs/utils_GUI.py
+drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:02:02.793364 idelucs-0.1.0/idelucs.egg-info/
+-rw-rw-r--   0 loan      (1000) loan      (1000)      556 2023-05-03 22:02:02.000000 idelucs-0.1.0/idelucs.egg-info/PKG-INFO
+-rw-rw-r--   0 loan      (1000) loan      (1000)      325 2023-05-03 22:02:02.000000 idelucs-0.1.0/idelucs.egg-info/SOURCES.txt
+-rw-rw-r--   0 loan      (1000) loan      (1000)        1 2023-05-03 22:02:02.000000 idelucs-0.1.0/idelucs.egg-info/dependency_links.txt
+-rw-rw-r--   0 loan      (1000) loan      (1000)        1 2023-05-03 21:54:29.000000 idelucs-0.1.0/idelucs.egg-info/not-zip-safe
+-rw-rw-r--   0 loan      (1000) loan      (1000)        8 2023-05-03 22:02:02.000000 idelucs-0.1.0/idelucs.egg-info/top_level.txt
+-rw-rw-r--   0 loan      (1000) loan      (1000)       38 2023-05-03 22:02:02.797364 idelucs-0.1.0/setup.cfg
+-rw-rw-r--   0 loan      (1000) loan      (1000)     1531 2023-05-03 22:02:00.000000 idelucs-0.1.0/setup.py
```

### Comparing `iDeLUCS-0.0.3/iDeLUCS.py` & `idelucs-0.1.0/idelucs/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,231 +1,302 @@
+#!/usr/bin/env python3
+
+import sys
 import pandas as pd
 import os
-from idelucs import models
 import numpy as np
 import matplotlib.pyplot as plt
 
+
 from idelucs.utils import SummaryFasta, plot_confusion_matrix, \
-                      label_features, compute_results, generate_csv_mapping
+                      label_features, compute_results
+
+from idelucs import models
 
 import argparse
 import torch
 import sys
 import time
-from datetime import datetime
-from resource import *
-import csv
-import tracemalloc
-
-def save_results_in_file(dataset_name, model_name, model_parameters, results,file_name):
-    # Create the file if it does not exitst and write first file with column names
-    with open(file_name, mode='a', newline='') as file:
-        writer = csv.writer(file, delimiter='\t')
-        if file.tell() == 0:
-            writer.writerow(['Dataset', 'Model', 'Parameters'] + list(results.keys()))
-
-        # Write the new row
-        row = [dataset_name, model_name, model_parameters] + list(results.values())
-        writer.writerow(row)
-        
 
+import csv
+#-------------------------------
+import hdbscan
 
 def weights_init(m):
     """
     Kaiming initialization of the weights
     :param m: Layer
     :return:
     """
     if isinstance(m, torch.nn.Linear):
         torch.nn.init.kaiming_normal_(m.weight)
         torch.nn.init.zeros_(m.bias)
-    elif hasattr(m, 'reset_parameters'):
-        m.reset_parameters()          
+        
+def save_results_in_file(dataset_name, model_name, model_parameters, results, time, memory, file_name):
+    # Create the file if it does not exitst and write first file with column names
+    with open(file_name, mode='a', newline='') as file:
+        writer = csv.writer(file, delimiter='\t')
+        if file.tell() == 0:
+            writer.writerow(['Dataset', 'Model', 'Parameters'] + list(results.keys()) + ['Time', 'Memory'])
+
+        # Write the new row
+        row = [dataset_name, model_name, model_parameters] + list(results.values()) + [time, memory]
+        writer.writerow(row)
+
 
 def run(args):
-    # starting memory monitoring
-    tracemalloc.start()
-    
-    
+
+    start_time = time.time()
     now = time.asctime()
     time_stamp = now.split(' ')
     hour = now.split(' ')[3]
     time_stamp[3] = '-'.join(hour.split(':'))
-    time_stamp = '_'.join(time_stamp[1:4])
-
+    
+    time_stamp = '_'.join(time_stamp[1:-1])
+    
     folder_name = os.getcwd()
-    folder_name = f"{folder_name}/Results"
+    folder_name = f'{folder_name}/Results'
+    
+    use_hdbscan = False
 
     if not os.path.isdir(folder_name):
         os.mkdir(folder_name)
 
-    if not os.path.isdir(f'{folder_name}/{time_stamp}'):
-        os.mkdir(f'{folder_name}/{time_stamp}')
+    results_folder = f'{folder_name}/{(args["sequence_file"]).split("/")[-1].split(".")[0]}'
+    
+    if not os.path.isdir(f'{results_folder}'):
+        os.mkdir(f'{results_folder}')
+    
+    os.mkdir(f'{results_folder}/{time_stamp}')
 
+    if args['n_clusters'] == 0:
+        args['n_clusters'], use_hdbscan = 200, True
+        
     model = models.IID_model(args)
     model.names, model.lengths, model.GT, model.cluster_dis = SummaryFasta(model.sequence_file,
                                                                            model.GT_file)
+    
+    if use_hdbscan:
+        clusterer = hdbscan.HDBSCAN(min_cluster_size=len(model.names)//100 + 1, gen_min_span_tree=True, prediction_data=True)
+    
     print(model.cluster_dis)
     stats = {"n_seq": len(model.lengths),
             "min_len": np.min(model.lengths),
             "max_len": np.max(model.lengths),
             "avg_len": np.mean(model.lengths)}
 
     print( f'No. Sequences: \t {stats["n_seq"]:,}')
     print(f'Min. Length: \t {stats["min_len"]:,}')
     print(f'Max. Length: \t {stats["max_len"]:,}')
     print(f'Avg. Length: \t {round(stats["avg_len"],2):,}')
     model.build_dataloader()
     predictions = []
+    min_loss = np.inf
     
     training_figure, display_training = plt.subplots(nrows=1, ncols=1)
     display_training.grid(True)
     display_training.set_title("Learning Curves")
     display_training.set_xlabel("Epoch")
     display_training.set_ylabel("Training Loss")
 
-    start_time = datetime.now()
+
     for voter in range(args['n_voters']):
         sys.stdout.write(f"\r........... Training Model ({voter+1}/{ args['n_voters']})................")
         sys.stdout.flush()
         model.net.apply(weights_init)
         model.epoch = 0
         model_loss = []
+        model_min_loss=np.inf
+
         for i in range(args['n_epochs']):
             loss = model.contrastive_training_epoch()
-            # loss = 10
-            print(f"Epoch: {i}, Loss: {loss}, n_voter: {voter}")
+            model_min_loss = min(model_min_loss, loss)
             model_loss.append(loss)
 
         length = len(model.names)
         y_pred, probabilities, latent = model.predict()
-        y_pred = y_pred.astype(np.int32)
+
+        if model_min_loss < min_loss:
+            model_latent = latent
         
-        d = {}
-        count = 0
-        for i in range(y_pred.shape[0]):
-            if y_pred[i] in d:
-                y_pred[i] = d[y_pred[i]]
-            else:
-                d[y_pred[i]] = count
-                y_pred[i] = count
-                count += 1
-        predictions.append(y_pred)
+        if not use_hdbscan:
+            y_pred = y_pred.astype(np.int32)
+            
+            d = {}
+            count = 0
+            for i in range(y_pred.shape[0]):
+                if y_pred[i] in d:
+                    y_pred[i] = d[y_pred[i]]
+                else:
+                    d[y_pred[i]] = count
+                    y_pred[i] = count
+                    count += 1
+            predictions.append(y_pred)
 
         display_training.plot(model_loss, label=f'Model {voter+1}')
         display_training.axes.legend(loc=1)
-        training_figure.savefig(f'{folder_name}/{time_stamp}/training_plots.jpg')
+        training_figure.savefig(f'{results_folder}/{time_stamp}/training_plots.jpg')
+                                                                
+
+    if not use_hdbscan:
+        y_pred, probabilities = label_features(np.array(predictions), args['n_clusters'])
+        
+    else:
+        clusterer.fit(latent )
+        y_pred = clusterer.labels_ + 1
+        probabilities = clusterer.probabilities_
+        args['n_clusters'] = np.max(y_pred) + 1
         
-        print("Memory Usage:", tracemalloc.get_traced_memory())
 
-    y_pred, probabilities = label_features(np.array(predictions), args['n_clusters'])
-    end_time = datetime.now()
-    time_taken = end_time - start_time
-    print("Training took:", time_taken)
-    print("Memory Usage Summary:", tracemalloc.get_traced_memory())
-    
-    
     #--------------------- Computing and Saving the Results
     sys.stdout.write(f"\r........... Computing Results ................")
     sys.stdout.flush()
     
     if args['GT_file'] != None:
         unique_labels = list(np.unique(model.GT))
         numClasses = len(unique_labels)
         y = np.array(list(map(lambda x: unique_labels.index(x), model.GT)))
         results, ind = compute_results(y_pred, latent, y)
 
         d = {}
         for i, j in ind:
             d[i] = j
-        w = np.zeros((numClasses, args['n_clusters']), dtype=np.int64)
         
+        if -1 in y_pred:
+            d[-1] = 0
+        
+        w = np.zeros((numClasses, max(max(y_pred) + 1, max(y) + 1)), dtype=np.int64)
         clustered = np.zeros_like(y, dtype=bool)
-        for i in range(length):
+        for i in range(y.shape[0]):
             w[y[i], d[y_pred[i]]] += 1
 
             if y[i] == d[y_pred[i]]:
                 clustered[i] = True
-
-        fig, new_ax = plt.subplots( nrows=1, ncols=1 )  # create figure & 1 axis
-        if len(unique_labels) < 16:
+         
+        if args['n_clusters'] < 16:
+            fig, new_ax = plt.subplots( nrows=1, ncols=1)  # create figure & 1 axis
             plot_confusion_matrix(w, unique_labels, ax=new_ax, normalize=False)
-            fig.savefig(f'{folder_name}/{time_stamp}/contingency_matrix.jpg')
+            fig.savefig(f'{results_folder}/{time_stamp}/contingency_matrix.jpg')
         else:
             # generating a csv mapping
-            generate_csv_mapping(w, unique_labels)
+            #generate_csv_mapping(w, unique_labels)
+            w_df = pd.DataFrame(w)
+            w_df.index = unique_labels
+            w_df.to_csv(f'{results_folder}/{time_stamp}/contingency_matrix.tsv',sep='\t')
+
     else:
         results, ind = compute_results(y_pred, latent)
-        clustered = (probabilities >= 0.9)
-       
-    results["time taken"] = time_taken
-    results["memory usage"] = tracemalloc.get_traced_memory()
+        #clustered = (probabilities >= 0.9)
+        clustered = (probabilities >= 0.0)
     
+    print(results)
     sys.stdout.write(f"\r........ Saving Results ..............")
     sys.stdout.flush()
     
+    
+    
     dataset_name = args['sequence_file'].split('/')[-1]
-    save_results_in_file(dataset_name, "iDeLUCS", args, results, "ALL_RESULTS.tsv")
+    del args['sequence_file']
+    del args['GT_file']
+    
 
+    _time = (time.time() - start_time) #running_info.ru_utime + running_info.ru_stime
+    hour = _time // 3600
+    minutes = (_time  - (3600 * hour)) // 60
+    seconds = _time - (hour * 3600) - (minutes * 60)
+    memory = "" #(running_info.ru_maxrss/1e6)
+    print("") #running_info)
+    
     names = np.array(model.names)
     data = np.concatenate((names[:,np.newaxis],
                               y_pred[:,np.newaxis],
                               probabilities[:,np.newaxis]), axis=1)
 
     df = pd.DataFrame(data, columns=['sequence_id','assignment','confidence_score'])
-    df.to_csv(f'{folder_name}/{time_stamp}/assignments.tsv',sep='\t')
+    df.to_csv(f'{results_folder}/{time_stamp}/assignments.tsv',sep='\t')
 
     df=pd.Series(results, name='Value')
-    df.to_csv(f'{folder_name}/{time_stamp}/metrics.tsv',sep='\t')
+    df.to_csv(f'{results_folder}/{time_stamp}/metrics.tsv',sep='\t')
+    
+    save_results_in_file(dataset_name, "iDeLUCS", args, results, 
+                         f'{hour}:{minutes}:{seconds}', 
+                         memory, f'{os.getcwd()}/ALL_RESULTS.tsv')
 
     # ------------------------------- Computing and Saving the Representations
-    
-    sys.stdout.write(f"\r........... Computing Representations................")
-    sys.stdout.flush()
+    if args['plot']:
+        sys.stdout.write(f"\r........... Computing Representations................")
+        sys.stdout.flush()
 
-    import umap
-    embedding = umap.UMAP(random_state=42).fit_transform(latent)
-    fig, ax = plt.subplots(nrows=1, ncols=1) 
-    ax.set_title("Representation of the Latent Space")
-    ax.set_xlabel("UMAP 1")
-    ax.set_ylabel("UMAP 2")
-    
-    ax.scatter(embedding[~clustered, 0],
-                embedding[~clustered, 1],
-                c = np.atleast_2d([0.5, 0.5, 0.5]),
-                s=1,
-                alpha=0.5)
-    ax.scatter(embedding[clustered, 0],
-               embedding[clustered, 1],
-               c=y_pred[clustered],
-               s=1,
-               cmap='Spectral')
-    plt.show()
-    fig.savefig(f'{folder_name}/{time_stamp}/learned_representation.jpg')
-    tracemalloc.stop()
+        import umap
+        n_samples = len(model.names)
+        mask = np.full(n_samples, True)
+        MAX_SAMPLES = 1000
+        if n_samples > MAX_SAMPLES :
+            mask = np.full(n_samples, False)
+            mask[:MAX_SAMPLES] = True
+            np.random.shuffle(mask)
+
+        embedding = umap.UMAP(random_state=42).fit_transform(latent)
+        fig, ax = plt.subplots(nrows=1, ncols=1) 
+        ax.set_title("Representation of the Latent Space")
+        ax.set_xlabel("UMAP 1")
+        ax.set_ylabel("UMAP 2")
+
+        ax.scatter(embedding[mask & ~clustered, 0],
+                   embedding[mask & ~clustered, 1],
+                   c = np.atleast_2d([0.5, 0.5, 0.5]),
+                   s=1,
+                   alpha=0.5)
+        ax.scatter(embedding[mask & clustered, 0],
+                  embedding[mask & clustered, 1],
+                  c=y[mask & clustered],  #y_pred[mask & clustered]
+                  s=1,
+                  cmap='Spectral')
+        fig.savefig(f'{results_folder}/{time_stamp}/learned_representation.jpg', dpi=150)
+    
 def main():
     parser= argparse.ArgumentParser()
     parser.add_argument('--sequence_file', action='store',type=str)
-    parser.add_argument('--n_clusters', action='store',type=int,default=5)
-    parser.add_argument('--n_epochs', action='store',type=int,default=100)
-    parser.add_argument('--n_mimics', action='store',type=int,default=3)
+    parser.add_argument('--n_clusters', action='store',type=int,default=0,
+                        help='Expected or maximum number of clusters to find. \n'
+                            'It should be equal or greater than n_true_clusters \n'
+                            'when GT is provided. \n'
+                            'NOTE: Use 0 for automatically finding fine-grained \n'
+                            'clusters')
+    parser.add_argument('--n_epochs', action='store',type=int,default=100,
+                        help='Number of training epochs. An epoch is defined \n' 
+                             'as a training iteration over all the training pairs.')
+    parser.add_argument('--n_mimics', action='store',type=int,default=3, 
+                        help='Number of data augmentations per sequence \n' 
+                            'that will be considered during training.')
     parser.add_argument('--batch_sz', action='store',type=int,default=256)
     parser.add_argument('--GT_file', action='store',type=str,default=None)
-    parser.add_argument('--k', action='store',type=int,default=6)
+    parser.add_argument('--k', action='store',type=int,default=6, help="k-mer length")
     parser.add_argument('--optimizer', action='store',type=str,default="RMSprop")
     parser.add_argument('--scheduler', action='store',type=str,default="None")
-    parser.add_argument('--weight', action='store',type=float,default=0.25)
-    parser.add_argument('--lambda', action='store',type=float,default=2.8)
-    parser.add_argument('--lr', action='store',type=float,default=1e-3)
-    parser.add_argument('--n_voters', action='store',type=int, default=5)
-    parser.add_argument('--model_size', action='store',type=str,default="linear")
 
+    parser.add_argument('--weight', action='store',type=float,default=0.25,
+                        help='Relative importance of the contrastive objective on \n'
+                            'the final loss. Use a higher value when low intra- \n'
+                            'cluster distance is expected and a lower value when \n'
+                            'high intra-cluster variability is expected')
+    
+    parser.add_argument('--lambda', action='store',type=float,default=2.8,
+                        help='Hyperparameter to control cluster balance. \n'
+                            'Use lambda: 1.2 when unbalanced clusters are expected \n'
+                            'Use lambda: 2.8 when perfectly balanced clusters are expected \n')
+    parser.add_argument('--lr', action='store',type=float,default=1e-3, help="Learning Rate")
+    parser.add_argument('--n_voters', action='store',type=int, default=5, help="Number of Voters")
+    parser.add_argument('--model_size', action='store',type=str,default="linear", help="Selection of 'conv', 'small', 'linear' or 'full'")
+    parser.add_argument('--plot', action='store',type=bool, default=False, help="Set to True to plot the final output representation")
+    
     args = vars(parser.parse_args())
 
     print("\nTraining Parameters:")
     for key in args:
         print(f'{key} \t -> {args[key]}')
     
     run(args)
 
+
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `iDeLUCS-0.0.3/idelucs/LossFunctions.py` & `idelucs-0.1.0/idelucs/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `iDeLUCS-0.0.3/idelucs/PytorchUtils.py` & `idelucs-0.1.0/idelucs/PytorchUtils.py`

 * *Files identical despite different names*

### Comparing `iDeLUCS-0.0.3/idelucs/ResNet.py` & `idelucs-0.1.0/idelucs/ResNet.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,40 +150,33 @@
         super(ConvNet,self).__init__()
         self.num_classes = num_classes
         self.layers = nn.Sequential(
                 nn.Conv2d(img_channel, 16, 5, 1, 2),
                 nn.BatchNorm2d(16),
                 nn.ReLU(),
                 nn.AvgPool2d(3,2,1),
-                nn.Dropout(p=0.2),
                 nn.Conv2d(16,32,3,1,1),
                 nn.BatchNorm2d(32),
                 nn.ReLU(),
                 nn.MaxPool2d(3,2,1),
-                nn.Dropout(p=0.2),
                 nn.Conv2d(32,64,3,1,1),
                 nn.BatchNorm2d(64),
                 nn.ReLU(),
                 nn.MaxPool2d(3,2,1),
-                nn.Dropout(p=0.2),
                 nn.Conv2d(64,64,3,1,1),
                 nn.AdaptiveAvgPool2d((1,1))
         )
-        
-        self.classifier = nn.Sequential(
-            nn.ReLU(),
-            nn.Dropout(p=0.5),
-            nn.Linear(64, num_classes),  
-            nn.Softmax(dim=1)
-        )
+
+        self.fc = nn.Linear(64, num_classes)
+        self.softmax = nn.Softmax(dim=1)
     
     def forward(self, x):
         latent = self.layers(x)
         latent = latent.reshape(latent.shape[0], -1)
-        out = self.classifier(latent)
+        out = self.softmax(self.fc(latent))
 
         return out, latent 
 
 
 class ConvNet_k_5( nn.Module):
     def __init__(self, img_channel = 1, num_classes=10):
         super(ConvNet_k_5,self).__init__()
```

### Comparing `iDeLUCS-0.0.3/idelucs/models.py` & `idelucs-0.1.0/idelucs/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import sys
 import torch
 import random
 import numpy as np
 import torch.nn as nn
 import torch.optim as optim
+from torch.utils.data import DataLoader
 
 sys.path.append('src/')
 sys.path.append('../src/')
 
-from idelucs.LossFunctions import IID_loss, info_nce_loss
-from torch.utils.data import DataLoader
-from idelucs.PytorchUtils import NetLinear, myNet
-from idelucs.ResNet import ResNet18, ConvNet
-
-from idelucs.utils import SequenceDataset, create_dataloader
+from .LossFunctions import IID_loss, info_nce_loss
+from .PytorchUtils import NetLinear, myNet
+from .ResNet import ResNet18
+from .utils import SequenceDataset, create_dataloader
 
 # Random Seeds for reproducibility.
 torch.manual_seed(0)
 torch.cuda.manual_seed(0)
 np.random.seed(0)
 random.seed(0)
 
@@ -48,32 +47,30 @@
     def __init__(self, args: dict):
 
         self.sequence_file = args['sequence_file']
         self.GT_file = args['GT_file']
 
         self.n_clusters = args['n_clusters']
         self.k = args['k']
-        self.model_type = args['model_size']
-
-        if self.model_type == 'linear':
+        
+        if args['model_size'] == 'linear':
             self.n_features = 4**self.k
             self.net = NetLinear(self.n_features, args['n_clusters'])
             self.reduce = False
             
-        elif self.model_type == 'small':
-            d = {4: 135, 5: 511, 6: 2079}
-            self.n_features = d[args['k']]
+        elif args['model_size'] == 'small':
+            if self.k % 2 == 0: n_in = (4**self.k + 4**(self.k//2))//2 
+            else: n_in = (4**self.k)//2
+            #d = {4: 135, 5: 511, 6: 2079}
+            self.n_features = n_in
             self.net = myNet(self.n_features, args['n_clusters'])
             self.reduce = True
             
-        elif self.model_type == 'full':
+        elif args['model_size'] == 'full':
             self.net = ResNet18(1, args['n_clusters'])
-        elif self.model_type == 'conv':
-            self.net = ConvNet(1, args['n_clusters'])
-            self.reduce = False
         else:
             raise ValueError("Invalid Model Type")
         
         self.net.apply(weights_init)
         self.net.to(device)
         self.epoch = 0
         self.EPS = sys.float_info.epsilon
@@ -101,45 +98,39 @@
         elif self.schedule == 'Triangle':
             self.scheduler = optim.lr_scheduler.CyclicLR(self.optimizer, base_lr=0.001, max_lr=0.1,step_size_up=5, mode="triangular2")
         
     def build_dataloader(self):
         #Data Files
         data_path = self.sequence_file
         GT_file = self.GT_file
-        representation = 'fcgr' if self.model_type in ('conv') else 'vector'
                 
         self.dataloader = create_dataloader(data_path, 
                                              self.n_mimics, 
                                              k=self.k, 
                                              batch_size=self.batch_sz, 
                                              GT_file=GT_file,
-                                             reduce=self.reduce,
-                                             representation=representation)
+                                             reduce=self.reduce)
 
     def contrastive_training_epoch(self):
         self.net.train()
         running_loss = 0.0
 
         for i_batch, sample_batched in enumerate(self.dataloader):
-
-            if self.model_type not in ('conv'):
-                sample = sample_batched['true'].view(-1, 1, self.n_features).type(dtype)
-                modified_sample = sample_batched['modified'].view(-1, 1, self.n_features).type(dtype)
-            else:
-                sample = sample_batched['true'][:, np.newaxis, ...].type(dtype)
-                modified_sample = sample_batched['modified'][:, np.newaxis, ...].type(dtype)
+            sample = sample_batched['true'].view(-1, 1, self.n_features).type(dtype)
+            modified_sample = sample_batched['modified'].view(-1, 1, self.n_features).type(dtype)
             
             # zero the gradients
             self.optimizer.zero_grad()
 
             # forward + backward + optimize
             z1, h1 = self.net(sample)
             z2, h2 = self.net(modified_sample)
 
             loss = (1-self.weight)*info_nce_loss(h1, h2, 0.85) + (self.weight)*IID_loss(z1, z2, lamb=self.l)
+            
             loss.backward()
             self.optimizer.step()
 
             running_loss += loss
             
         running_loss /= i_batch
 
@@ -148,61 +139,57 @@
         elif self.schedule == 'Triangle':
             self.scheduler.step()
         self.epoch += 1
 
         return running_loss.item()
 
     def predict(self, data=None):
-        representation = 'fcgr' if self.model_type in ('conv') else 'vector'
-        test_dataset = SequenceDataset(self.sequence_file, k=self.k, transform=None, GT_file=self.GT_file, reduce=self.reduce, representation=representation)
+        
+        n_features = self.n_features
+        test_dataset = SequenceDataset(self.sequence_file, k=self.k, transform=None, GT_file=self.GT_file, reduce=self.reduce)
         test_dataloader = DataLoader(test_dataset, 
                              batch_size=self.batch_sz,
                              shuffle=False,
                              num_workers=0,
                              drop_last=False)
         y_pred = []
         probabilities = []
         latent = []
 
         with torch.no_grad():
             self.net.eval()
             
             for test in test_dataloader:
-                if self.model_type not in ('conv'):
-                    kmers = test['kmer'].view(-1, 1, self.n_features).type(dtype)
-                else:
-                    #kmers = test['kmer'][:, np.newaxis, ...].type(dtype)
-                    kmers = test['kmer'].type(dtype)
+                
+                kmers = test['kmer'].view(-1, 1, self.n_features).type(dtype)
                 outputs, logits = self.net(kmers)
                 probs,  predicted = torch.max(outputs, 1)
 
                 #Extend our list with predictions and groud truth
                 y_pred.extend(predicted.cpu().tolist())
                 probabilities.extend(probs.cpu().tolist())
                 latent.extend(logits.cpu().tolist())
-                
-        return np.array(y_pred), np.array(probabilities), np.array(latent) 
+        
+        return np.array(y_pred), np.array(probabilities), np.array(latent)
+        #return np.array(y_pred), np.array(probabilities), kmers
 
     def calculate_probs(self, data=None):
+        
         n_features = self.n_features
-        representation = 'fcgr' if self.model_type in ('conv') else 'vector'
-        test_dataset = SequenceDataset(self.sequence_file, k=self.k, transform=None, GT_file=self.GT_file, reduce=self.reduce, representation=representation)
+        test_dataset = SequenceDataset(self.sequence_file, k=self.k, transform=None, GT_file=self.GT_file, reduce=self.reduce)
         test_dataloader = DataLoader(test_dataset, 
                              batch_size=self.batch_sz,
                              shuffle=False,
                              num_workers=0,
                              drop_last=False)
  
         probabilities = []
         with torch.no_grad():
             self.net.eval()
             for test in test_dataloader:
-                if self.model_type not in ('conv'):
-                    kmers = test['kmer'].view(-1, 1, n_features).type(dtype)
-                else:
-                    kmers = test['kmer'][:, np.newaxis, ...].type(dtype)
+                kmers = test['kmer'].view(-1, 1, n_features).type(dtype)
 
                 #calculate the prediction by running through the network
                 outputs, logits = self.net(kmers)
                 probabilities.extend(outputs.cpu().tolist())
 
         return np.array(probabilities)
```

### Comparing `iDeLUCS-0.0.3/idelucs/utils.py` & `idelucs-0.1.0/idelucs/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import sys
-sys.path.append('src/')
 import pyximport 
 pyximport.install()
 
-# from kmers import kmer_counts
-from idelucs.kmers_non_cython import kmer_counts
+from .kmers import kmer_counts
 
 import random, itertools
 import numpy as np
 import pandas as pd
 import sklearn.metrics.cluster as metrics
 from sklearn.cluster import KMeans
 
@@ -43,53 +41,17 @@
 
     masked = seq.translate(basemask, b' \t\n\r')
     stripped = masked.translate(None, b'ACGTN')
     if len(stripped) > 0:
         bad_character = chr(stripped[0])
         msg = "Invalid DNA byte in sequence {}: '{}'"
         raise ValueError(msg.format(header, bad_character))
-
-def pos_gen(kmer):
-    """
-    Find the position of a particular kmer in the CGR.
-    :param kmer: string with the kmer.
-    :return: position in the CGR.
-    """
-    k = len(kmer)
-    posx = 2 ** k
-    posy = 2 ** k
-    for i in range(1, k + 1):
-        bp = kmer[-i]
-        # print(posx, posy)
-        if bp == 'C':
-            posx = posx - 2 ** (k - i)
-            posy = posy - 2 ** (k - i)
-        elif bp == 'A':
-            posx = posx - 2 ** (k - i)
-        elif bp == 'G':
-            posy = posy - 2 ** (k - i)
-    return int(posx - 1), int(posy - 1)
-
-def cgr_gen(probs, k):
-    """
-    Generate CGR from the kmer counts for a given value of k.
-    :param probs: array with the normalized kmer counts
-    :param k:
-    :return: 2D - CGR pattern.
-    """
-    from itertools import product
-    kamers = product(*(["ACTG"] * k))
-    mat = np.zeros((2 ** k, 2 ** k))
-    for i, kmer in enumerate(kamers):
-        x, y = pos_gen(kmer)
-        # print(x, y)
-        mat[y][x] = probs[i]
-    return mat
-
-
+    return masked
+    
+    
 class transition(object):
     """
     Mutate Genomic sequence using transitions only.
     :param seq: Original Genomic Sequence.
     :param threshold: probability of Transition.
     :return: Mutated Sequence.
     """
@@ -190,15 +152,15 @@
         elif line.startswith(b'>'):
             if seq_id != "":
                 seq = bytearray().join(lines)
 
                 if (GT_file and not seq_id in GT_dict):
                     raise ValueError('Check GT for sequence {}'.format(seq_id))
 
-                check_sequence(seq_id, seq)
+                seq = check_sequence(seq_id, seq)
                 names.append(seq_id)
                 lengths.append(len(seq))
 
                 if GT_file:
                     ground_truth.append(GT_dict[seq_id])
 
                 lines = []
@@ -209,25 +171,58 @@
         else:
             lines += [line.strip()]
   
     if (GT_file and not seq_id in GT_dict):
         raise ValueError('Check GT for sequence {}'.format(seq_id))
 
     seq = bytearray().join(lines)
-    check_sequence(seq_id, seq)
+    seq = check_sequence(seq_id, seq)
     names.append(seq_id) 
     lengths.append(len(seq))
 
     if GT_file:
         ground_truth.append(GT_dict[seq_id])
 
     return names, lengths, ground_truth, cluster_dis
 
 
-def kmersFasta(fname, k=6, transform=None, reduce=False, representation='vector'):
+def reverse_complement(x, k):
+    numbits = 2*k  
+    mask = 0xAAAAAAAA
+    x = ((x >> 1) & (mask>>1)) | ((x<< 1) & mask)
+    x = (1 << numbits) - 1 - x
+    rev = 0
+
+    size = 2**numbits-1
+    while(size > 0):
+        rev <<= 1
+        if x & 1 == 1:
+            rev ^= 1
+        x >>=1
+        size >>= 1
+
+    return rev
+
+def kmer_rev_comp(kmer_counts, k):
+    index=[]
+    for kmer in range(4**k):
+        revcomp = reverse_complement(kmer,k)
+
+        # Only look at canonical kmers - this makes no difference
+        if kmer <= revcomp:
+            index.append(kmer)
+            kmer_counts[kmer] += kmer_counts[revcomp]
+            kmer_counts[kmer] *= 0.5
+        #else:
+        #    kmer_counts[kmer] = kmer_counts[revcomp]
+
+    return kmer_counts[index]
+
+
+def kmersFasta(fname, k=6, transform=None, reduce=False):
     lines = list()
     seq_id = ""
     names, kmers = [], []
 
     for line in open(fname, "rb"):
         if line.startswith(b'#'):
             pass
@@ -237,21 +232,20 @@
                 seq = bytearray().join(lines)
                 names.append(seq_id)  
                             
                 if transform:
                     transform(seq)
                     
                 counts = np.ones(4**k, dtype=np.int32)
-                if representation == 'vector':
-                    kmer_counts(seq, k, counts)
-                else:
-                    # cgr(seq, k, counts)
-                    kmer_counts(seq, k, counts)
-                    counts = cgr_gen(counts, k)
-                    # counts = counts.reshape((2**k, 2**k))
+                kmer_counts(seq, k, counts)
+                #cgr(seq, k, counts)
+
+                if reduce:
+                    counts = kmer_rev_comp(counts,k)
+
 
                 kmers.append(counts / np.sum(counts))
                 
                 lines = []
                 seq_id = line[1:-1].decode()  # Modify this according to your labels.  
             seq_id = line[1:-1].decode()
         
@@ -260,90 +254,116 @@
   
     seq = bytearray().join(lines)
     names.append(seq_id)
     if transform:
         transform(seq)
         
     counts = np.ones(4**k, dtype=np.int32)
-    if representation == 'vector':
-        kmer_counts(seq, k, counts)
-    else:
-        kmer_counts(seq, k, counts)
-        counts = cgr_gen(counts, k)
+    kmer_counts(seq, k, counts)
+    #cgr(seq, k, counts)
+    if reduce:
+        counts = kmer_rev_comp(counts,k)
+    kmers.append(counts / np.sum(counts))
+    
+    #if reduce:
+    #    K_file = np.load(open(f'kernels/kernel{k}.npz','rb'))
+    #    KERNEL = K_file['arr_0']
+    #    return names, np.dot(np.array(kmers), KERNEL)
+        
+    return names, np.array(kmers)
 
+def cgrFasta(fname, k=6, transform=None):
+    lines = list()
+    seq_id = ""
+    names, kmers = [], []
+
+    for line in open(fname, "rb"):
+        if line.startswith(b'#'):
+            pass
+
+        elif line.startswith(b'>'):
+            if seq_id != "":
+                seq = bytearray().join(lines)
+                names.append(seq_id)  
+                            
+                if transform:
+                    transform(seq)
+                    
+                counts = np.ones(4**k, dtype=np.int32)
+                #kmer_counts(seq, k, counts)
+                cgr(seq, k, counts)
+                kmers.append(counts / np.sum(counts))
+                
+                lines = []
+                seq_id = line[1:-1].decode()  # Modify this according to your labels.  
+            seq_id = line[1:-1].decode()
+        
+        else:
+            lines += [line.strip()]
+  
+    seq = bytearray().join(lines)
+    names.append(seq_id)
+    if transform:
+        transform(seq)
+        
+    counts = np.ones(4**k, dtype=np.int32)
+    #kmer_counts(seq, k, counts)
+    cgr(seq, k, counts)
     kmers.append(counts / np.sum(counts))
+    return names, np.array(kmers)
 
-    result_array = np.array(kmers)
-    if reduce:
-        K_file = np.load(open(f'kernels/kernel{k}.npz','rb'))
-        KERNEL = K_file['arr_0']
-        result_array = np.dot(result_array, KERNEL)
-        # return names, [:, np.newaxis, ...]
-    
-    #if representation == 'vector':
-    #    return names, result_array
-    #else:
-    return names, result_array[:, np.newaxis, ...]
  
 import time 
-def AugmentFasta(sequence_file, n_mimics, k=6, reduce=False, representation='vector'):
+def AugmentFasta(sequence_file, n_mimics, k=6, reduce=False):
+
     train_features = []
+    start = time.time()
 
     # Compute Features and save original data for testing.
-    sys.stdout.write(f'\r............computing augmentations (0/{n_mimics})................')
-    sys.stdout.flush()
-    _, t_norm = kmersFasta(sequence_file, k=k, transform=transition_transversion(1e-2, 0.5e-2), reduce=reduce, representation=representation)
-    # t_norm = t_norm[:, np.newaxis, ...]
-    # print("Norm:", t_norm.shape)
-    #t_norm.resize(t_norm.shape[0],1,t_norm.shape[1])
-    #print("Current:", t_norm.shape)
+    #sys.stdout.write(f'\r............computing augmentations (0/{n_mimics})................')
+    #sys.stdout.flush()
+    
+    _, t_norm = kmersFasta(sequence_file, k=k, transform=transition_transversion(1e-2, 0.5e-2), reduce=reduce)
+    t_norm.resize(t_norm.shape[0],1,t_norm.shape[1])
     
     
-    sys.stdout.write(f'\r............computing augmentations (1/{n_mimics})................')
-    sys.stdout.flush()
-    _, t_mutated = kmersFasta(sequence_file, k=k, transform=transition(1e-2), reduce=reduce, representation=representation)
-    #t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
+    #sys.stdout.write(f'\r............computing augmentations (1/{n_mimics})................')
+    #sys.stdout.flush()
+    _, t_mutated = kmersFasta(sequence_file, k=k, transform=transition(1e-2), reduce=reduce)
+    t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
     train_features.extend(np.concatenate((t_norm, t_mutated), axis=1))
     
-    sys.stdout.write(f'\r............computing augmentations (2/{n_mimics})................')
-    sys.stdout.flush()
-    _, t_mutated = kmersFasta(sequence_file, k=k, transform=transversion(0.5e-2), reduce=reduce, representation=representation)
-    #t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
+    #sys.stdout.write(f'\r............computing augmentations (2/{n_mimics})................')
+    #sys.stdout.flush()
+    _, t_mutated = kmersFasta(sequence_file, k=k, transform=transversion(0.5e-2), reduce=reduce)
+    t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
     train_features.extend(np.concatenate((t_norm, t_mutated), axis=1))
     
     for j in range(n_mimics-2):
-        sys.stdout.write(f'\r............computing augmentations ({3+j}/{n_mimics})................')
-        sys.stdout.flush()
-        _, t_mutated = kmersFasta(sequence_file, k=k, transform=Random_N(20), reduce=reduce, representation=representation)
-        #t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
+        #sys.stdout.write(f'\r............computing augmentations ({3+j}/{n_mimics})................')
+        #sys.stdout.flush()
+        _, t_mutated = kmersFasta(sequence_file, k=k, transform=Random_N(20), reduce=reduce)
+        t_mutated.resize(t_mutated.shape[0], 1, t_mutated.shape[1])
         train_features.extend(np.concatenate((t_norm, t_mutated), axis=1)) 
 
     x_train = np.array(train_features).astype('float32')
     x_test = np.reshape(t_norm, (-1, t_norm.shape[-1])).astype('float32')
     #print("\n Elapsed Time:", time.time()-start)
 
     # scaling the data.
-    if representation not in ("fcgr"):
-        scaler = StandardScaler()
-        scaler.fit(x_test)
-
-        x_train_1 = scaler.transform(x_train[:, 0, :])
-        x_train_2 = scaler.transform(x_train[:, 1, :])
-        x_test = scaler.transform(x_test)
+    scaler = StandardScaler()
+    scaler.fit(x_test)
 
-        x_train[:, 0, :] = x_train_1
-        x_train[:, 1, :] = x_train_2
-    else:
-        x_train_1 = x_train[:, 0, :]
-        x_train_2 = x_train[:, 1, :]
-        x_train_1 = (x_train_1 - np.mean(x_train_1)) / np.std(x_train_1)
-        x_train_2 = (x_train_2 - np.mean(x_train_2)) / np.std(x_train_2)
-        x_train[:, 0, :] = x_train_1
-        x_train[:, 1, :] = x_train_2
+    x_train_1 = scaler.transform(x_train[:, 0, :])
+    x_train_2 = scaler.transform(x_train[:, 1, :])
+    x_test = scaler.transform(x_test)
 
+    x_train[:, 0, :] = x_train_1
+    x_train[:, 1, :] = x_train_2
+    
     return x_train
 
 class AugmentedDataset(Dataset):
     """ 
     Dataset creation directly from fasta file.
     """
 
@@ -356,38 +376,33 @@
     def __len__(self):
         return self.data.shape[0]
 
     def __getitem__(self, idx):
         if torch.is_tensor(idx):
             idx = idx.tolist()
         
-        sample = {'true': self.data[idx, 0, ...], 'modified': self.data[idx, 1, ...]}  #<--- We can enforce the prediction of same vector
+        sample = {'true': self.data[idx, 0, :], 'modified': self.data[idx, 1, :]}  #<--- We can enforce the prediction of same vector
         return sample
 
 class SequenceDataset(Dataset):
     """ Dataset creation directly from fasta file"""
     
-    def __init__(self, fasta_file, k=6, transform=None, GT_file=None, reduce=False, representation='vector'):
+    def __init__(self, fasta_file, k=6, transform=None, GT_file=None, reduce=False):
         """ Args:
             fasta_file (string): Path to te fasta file
             transform (callable, optional): Optional transform to be applied on a 
                                             sequence. Function computing the mimics 
         """
         self.names, self.lengths, self.GT, self.cluster_dis = SummaryFasta(fasta_file, GT_file)
-        _, self.kmers = kmersFasta(fasta_file, k, transform, reduce=reduce, representation=representation)
+        _, self.kmers = kmersFasta(fasta_file, k, transform, reduce=reduce)
 
         # scaling the data.
-        if representation == 'vector':
-            scaler = StandardScaler()
-            self.kmers = self.kmers[:, 0, :]
-            self.kmers = scaler.fit_transform(self.kmers)
-        else:
-            self.kmers = self.kmers[:, 0, :]
-            self.kmers = (self.kmers - np.mean(self.kmers)) / np.std(self.kmers)
-            self.kmers = self.kmers[:, np.newaxis, :, :]
+        scaler = StandardScaler()
+        self.kmers = scaler.fit_transform(self.kmers)
+
         
     def __len__(self):
         return len(self.lengths)
 
     def __getitem__(self, idx):
         if torch.is_tensor(idx):
             idx = idx.tolist()
@@ -395,18 +410,19 @@
         if self.GT:           
             sample = {'kmer':self.kmers[idx,:],'name':self.names[idx], 'cluster_id':self.GT[idx]}
         else:
             sample = {'kmer':self.kmers[idx,:],'name':self.names[idx]}
             
         return sample
 
-def create_dataloader(sequence_file, n_mimics, k=6, batch_size=512, GT_file=None, reduce=False, representation='vector'):
-    train_data = AugmentFasta(sequence_file, n_mimics, k=k, reduce=reduce, representation=representation)
+def create_dataloader(sequence_file, n_mimics, k=6, batch_size=512, GT_file=None, reduce=False):
+
+    train_data = AugmentFasta(sequence_file, n_mimics, k=k, reduce=reduce)
     training_set = AugmentedDataset(train_data)
-    return DataLoader(training_set, batch_size=batch_size, shuffle=True, num_workers=4)
+    return DataLoader(training_set, batch_size=batch_size, shuffle=True, num_workers=0) #num_workers=4
 
 
 #-------------------- The following couple of functions are for plotting and saving the point cloud during training-----
 
 def get_coord(probs, num_classes):
     # computes coordinate for 1 sample based on probability distribution over c
   
@@ -482,28 +498,28 @@
     ind = np.asarray(ind)
     ind = np.transpose(ind)
     return ind, sum([w[i, j] for i, j in ind]) * 1.0 / y_pred.size
 
 def generate_csv_mapping(cm, target_names):
     result_dict = {}
     for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):  
-        result_dict[(target_names[i], target_names[j])] = cm[i, j]
+        result_dict[(target_names[i], j)] = cm[i, j]
     pandas_dict = {
         "Predicted": [],
         "Actual": [],
         "Count": []
     }
     for (target1, target2), count in result_dict.items():
-        pandas_dict["Predicted"].append(target1)
-        pandas_dict["Actual"].append(target2)
+        pandas_dict["Predicted"].append(target2)
+        pandas_dict["Actual"].append(target1)
         pandas_dict["Count"].append(count)
     
     result_pd = pd.DataFrame(pandas_dict)
     result_pd.to_csv('confusion_matrix.csv')
-    
+
 def plot_confusion_matrix(cm,
                           target_names,
                           pairs = None,
                           title='Confusion matrix',
                           cmap=None,
                           normalize=False,
                           ax=None):
@@ -577,18 +593,66 @@
 def compute_results(y_pred, data, y_true=None):
     d = {}
 
     d['Davies-Boulding'] = metrics.davies_bouldin_score(data, y_pred)
     d['Silhouette-Score'] = metrics.silhouette_score(data, y_pred)
 
     if not y_true is None:
-        #d['NMI'] = metrics.adjusted_mutual_info_score(y_true, y_pred)
-        #d['ARI'] = metrics.adjusted_rand_score(y_true, y_pred)
+        d['NMI'] = metrics.adjusted_mutual_info_score(y_true, y_pred)
+        d['ARI'] = metrics.adjusted_rand_score(y_true, y_pred)
+        d['Homogeneity'] = metrics.homogeneity_score(y_true, y_pred)
+        d['Completeness'] = metrics.completeness_score(y_true, y_pred)
 
         ind, acc = cluster_acc(y_true, y_pred)
         d['ACC'] = acc
     
         return d, ind
 
     return d, None
 
+
+
         
+from itertools import permutations, product
+import sys
+
+def modified_Hungarian(test):
+    rows, cols = linear_sum_assignment(test)
+    new_cols = np.array(list(set(range(test.shape[1])).difference(cols)))
+
+    if new_cols.shape[0] != 0:
+        minval = sys.maxsize
+
+        for i in permutations(new_cols, len(new_cols)):
+            for j in product(rows, repeat=len(new_cols)):
+                _sum = sum(test[j,i])
+                if _sum < minval:
+                    good_assignment = (j,i)
+
+                minval = min(minval, _sum)
+
+        full_rows = np.array(list(rows) + list(good_assignment[0]))
+        full_cols = np.array(list(cols) + list(good_assignment[1]))
+    else:
+        full_rows, full_cols = rows, cols
+
+    return full_rows, full_cols
+
+def modified_cluster_acc(y_true, y_pred):
+    """
+    Calculate clustering accuracy with more predicted clusters than true labels
+    :param y_true: true labels, numpy.array with shape `(n_samples,)`
+    :param y_pred: predicted labels, numpy.array with shape `(n_samples,)`
+    :return:  accuracy, in [0,1]
+    """
+
+    y_true = y_true.astype(np.int64)
+    w = np.zeros((y_true.max() + 1, y_pred.max() + 1), dtype=np.int64)
+
+    for i in range(y_pred.size):
+        w[y_true[i], y_pred[i]] += 1
+    
+    #print(w)
+
+    ind = modified_Hungarian(w.max() - w)
+    ind = np.asarray(ind).T
+    return ind, sum([w[i, j] for i, j in ind]) * 1.0 / y_pred.size
```

### Comparing `iDeLUCS-0.0.3/idelucs/utils_GUI.py` & `idelucs-0.1.0/idelucs/utils_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
     GUI.input_n_epochs.setToolTip('Number of training epochs. An epoch is defined \n' 
                                  'as a training iteration over all the training pairs.')
 
     GUI.input_n_clusters.setToolTip('Expected or maximum number of clusters to find. \n'
                                     'It should be equal or greater than n_true_clusters \n'
-                                    'when GT is provided')
+                                    'when GT is provided. \n'
+                                    'NOTE: Use 0 for automatically finding fine-grained \n'
+                                    'clusters')
 
     GUI.input_scheduler.setToolTip('Learning rate schedule to train the neural network.')
 
     GUI.input_batch_sz.setToolTip('Number of data pairs that the network will receive \n'
                                   'simultaneouly during training. A larger batch may \n'
                                   'improve convergence but it may harm the accuracy \n')
 
@@ -41,14 +43,8 @@
                             ' assignment of each sequence with the assignment \n'
                             'of the closest sequence assigned to a different cluster. \n'
                             'Range: [-1,1]')
 
     GUI.DB_Index.setToolTip('Lower is better - Measures the average distance between \n'
                             'clusters, relative to their sizes. Range: [0,2] \n')                         
 
-    GUI.Submit_Button.setToolTip('Parse training Information')
-    
-
-    
-
-
-
+    GUI.Submit_Button.setToolTip('Parse training Information')
```

