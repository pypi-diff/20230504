# Comparing `tmp/HACNet-1.4.2.tar.gz` & `tmp/HACNet-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HACNet-1.4.2.tar", last modified: Tue May  2 17:55:47 2023, max compression
+gzip compressed data, was "HACNet-1.4.3.tar", last modified: Thu May  4 15:25:02 2023, max compression
```

## Comparing `HACNet-1.4.2.tar` & `HACNet-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.716149 HACNet-1.4.2/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.675258 HACNet-1.4.2/HACNet/
--rw-rw-rw-   0        0        0    14950 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/CNN.py
--rw-rw-rw-   0        0        0    15340 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/GCN.py
--rw-rw-rw-   0        0        0     8898 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/MLP.py
--rw-rw-rw-   0        0        0        2 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/__init__.py
--rw-rw-rw-   0        0        0    55401 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.710165 HACNet-1.4.2/HACNet.egg-info/
--rw-rw-rw-   0        0        0      373 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-05-02 17:55:26.000000 HACNet-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      373 2023-05-02 17:55:47.716149 HACNet-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3536 2023-05-02 17:55:26.000000 HACNet-1.4.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-02 17:55:47.720139 HACNet-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-05-02 17:55:27.000000 HACNet-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:25:02.663852 HACNet-1.4.3/
+drwxrwxrwx   0        0        0        0 2023-05-04 15:25:02.643843 HACNet-1.4.3/HACNet/
+-rw-rw-rw-   0        0        0    14950 2023-05-04 15:24:46.000000 HACNet-1.4.3/HACNet/CNN.py
+-rw-rw-rw-   0        0        0    15340 2023-05-04 15:24:46.000000 HACNet-1.4.3/HACNet/GCN.py
+-rw-rw-rw-   0        0        0     8898 2023-05-04 15:24:46.000000 HACNet-1.4.3/HACNet/MLP.py
+-rw-rw-rw-   0        0        0        2 2023-05-04 15:24:46.000000 HACNet-1.4.3/HACNet/__init__.py
+-rw-rw-rw-   0        0        0    55293 2023-05-04 15:24:46.000000 HACNet-1.4.3/HACNet/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:25:02.662852 HACNet-1.4.3/HACNet.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-05-04 15:25:02.000000 HACNet-1.4.3/HACNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-04 15:25:02.000000 HACNet-1.4.3/HACNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:25:02.000000 HACNet-1.4.3/HACNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 15:25:02.000000 HACNet-1.4.3/HACNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-05-04 15:24:47.000000 HACNet-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0      373 2023-05-04 15:25:02.663852 HACNet-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3819 2023-05-04 15:24:47.000000 HACNet-1.4.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-04 15:25:02.664882 HACNet-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-05-04 15:24:47.000000 HACNet-1.4.3/setup.py
```

### Comparing `HACNet-1.4.2/HACNet/CNN.py` & `HACNet-1.4.3/HACNet/CNN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.2/HACNet/GCN.py` & `HACNet-1.4.3/HACNet/GCN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.2/HACNet/MLP.py` & `HACNet-1.4.3/HACNet/MLP.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.2/HACNet/functions.py` & `HACNet-1.4.3/HACNet/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 """ Define a function to test HACNet, the 3D-CNN, or one of the GCN components on an HDF file """
 
 def predict_hdf(architecture, cnn_test_path, gcn0_test_path, gcn1_test_path, cnn_checkpoint_path, gcn0_checkpoint_path, gcn1_checkpoint_path):
 
     """
     Inputs:
-    1) test: either "HACNet", "cnn", "gcn0", or "gcn1"    
+    1) architecture: either "HACNet", "cnn", "gcn0", or "gcn1"    
     2) cnn_test_path: path to cnn test set npy file
     3) gcn0_test_path: path to gcn0 test set hdf file
     4) gcn1_test_path: path to gcn1 test set hdf file
     5) cnn_checkpoint_path: path to cnn checkpoint file
     6) gcn0_checkpoint_path: path to gcn0 checkpoint file
     7) gcn1_checkpoint_path: path to gcn1 checkpoint file
     Output:
@@ -79,16 +79,15 @@
         cnn_dataset = MLP_Dataset(cnn_test_path)
         # initialize data loader
         batch_count = len(cnn_dataset) // batch_size
         cnn_dataloader = DataLoader(cnn_dataset, batch_size=batch_size, shuffle=False, num_workers=0, worker_init_fn=None)
         # define model
         cnn_model = MLP(use_cuda=use_cuda)
         cnn_model.to(device)
-        if isinstance(cnn_model, (DistributedDataParallel, DataParallel)):
-            cnn_model = cnn_model.module
+
         # load checkpoint file
         cnn_checkpoint = torch.load(cnn_checkpoint_path, map_location=device)
         # model state dict
         cnn_model_state_dict = cnn_checkpoint.pop("model_state_dict")
         cnn_model.load_state_dict(cnn_model_state_dict, strict=True)
         # create empty arrays to hold predicted and true values
         y_true_cnn = np.zeros((len(cnn_dataset),), dtype=np.float32)
```

### Comparing `HACNet-1.4.2/LICENSE` & `HACNet-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.2/README.md` & `HACNet-1.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 ## Overview of Model
 
 ![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/98780179/206188596-032a4f78-4af1-48e8-8cc0-f1800587ddab.gif)
 
 HAC-Net (Hybrid Attention-Based Convolutional Neural Network) is a novel deep learning architecture for protein-ligand binding affinity prediction consisting of a 3D-CNN utilizing channel-wise attention and two GCNs utilizing attention-based aggregation of node features. This combination achieves an optimal balance between the superior performance of our GCNs and the complementary learning style of our 3D-CNN. Furthermore, the inclusion of two architecturally-identical GCNs mitigates noise resulting from the inherently-stochastic nature of the training process. By incorporating multiple forms of attention with advanced concepts from CNN and GCN architectural design, we are able to demonstrate state-of-the-art performance on the PDBbind benchmark for protein-ligand binding affinity prediction, as well the ability to generalize to complexes unlike those used for training.
 
+## Demo Video of HACNet Python Package
+https://user-images.githubusercontent.com/98780179/236011365-6597f75e-8b19-4f9e-93d6-944875227a22.mp4
+
+## Tutorial Notebook Using HACNet Python Package
+https://colab.research.google.com/github/gregory-kyro/HAC-Net/blob/main/HACNet.ipynb
+
 ## Important Files and Notebooks
 All of the:
 1) HDF files used for training, validation and testing
 2) NPY files containing 3D-CNN extracted features
 3) PT files containing model parameters
 4) IPYNB files of tutorial notebooks for training and testing
```

