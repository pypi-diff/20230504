# Comparing `tmp/potatorch-0.0.1.tar.gz` & `tmp/potatorch-0.0.2.tar.gz`

## Comparing `potatorch-0.0.1.tar` & `potatorch-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.1/.dockerignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.1/Dockerfile.gpu
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.1/build.sh
--rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.1/potatorch.png
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.1/run.sh
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.1/setup.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.1/examples/grid_search.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 potatorch-0.0.1/examples/mlp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/__init__.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/callbacks.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/training.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/datasets/FilteredDataset.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/datasets/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/datasets/utils.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/losses/MSRELoss.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/losses/WDLLoss.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/losses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/models/__init__.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/models/cnn.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/optimization/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/optimization/bayesian_optimizer.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.1/src/potatorch/optimization/tuning.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.1/LICENSE
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 potatorch-0.0.1/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 potatorch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.2/.dockerignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.2/Dockerfile.gpu
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.2/build.sh
+-rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.2/potatorch.png
+-rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.2/run.sh
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.2/setup.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.2/examples/grid_search.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 potatorch-0.0.2/examples/mlp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/__init__.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/callbacks.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/training.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/FilteredDataset.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/utils.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/MSRELoss.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/WDLLoss.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/models/__init__.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/models/cnn.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/bayesian_optimizer.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/tuning.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 potatorch-0.0.2/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 potatorch-0.0.2/PKG-INFO
```

### Comparing `potatorch-0.0.1/potatorch.png` & `potatorch-0.0.2/potatorch.png`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/examples/grid_search.py` & `potatorch-0.0.2/examples/grid_search.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/examples/mlp.py` & `potatorch-0.0.2/examples/mlp.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/callbacks.py` & `potatorch-0.0.2/src/potatorch/callbacks.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/training.py` & `potatorch-0.0.2/src/potatorch/training.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/datasets/FilteredDataset.py` & `potatorch-0.0.2/src/potatorch/datasets/FilteredDataset.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/datasets/utils.py` & `potatorch-0.0.2/src/potatorch/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/losses/MSRELoss.py` & `potatorch-0.0.2/src/potatorch/losses/MSRELoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/losses/WDLLoss.py` & `potatorch-0.0.2/src/potatorch/losses/WDLLoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/models/cnn.py` & `potatorch-0.0.2/src/potatorch/models/cnn.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/optimization/bayesian_optimizer.py` & `potatorch-0.0.2/src/potatorch/optimization/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/src/potatorch/optimization/tuning.py` & `potatorch-0.0.2/src/potatorch/optimization/tuning.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/.gitignore` & `potatorch-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/LICENSE` & `potatorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.1/README.md` & `potatorch-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,44 @@
+Metadata-Version: 2.1
+Name: potatorch
+Version: 0.0.2
+Summary: Lightweight high-level PyTorch framework that runs on potato machines
+Project-URL: Homepage, https://github.com/crybot/potatorch
+Project-URL: Bug Tracker, https://github.com/crybot/potatorch/issues
+Author-email: Marco Pampaloni <marco.pampaloni1@gmail.com>
+License-File: LICENSE
+Keywords: deep learning,framework,limited resources,machine learning,python,pytorch
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 
 <div align="center">
 
 # PotaTorch
 
 <img src="https://raw.githubusercontent.com/crybot/potatorch/main/potatorch.png" width="200" height="200" role="img">
 
 **PotaTorch is a lightweight PyTorch framework specifically designed to run on hardware with limited resources.**
 
 **WIP:**
 ______________________________________________________________________
 </div>
 
 ### Install PotaTorch
-PotaTorch is not currently on PyPI, so you'll have to install it from sources:
+PotaTorch is published on PyPI, you can install it through pip:
+```bash
+pip install potatorch
+```
+
+or you can install it from sources:
 ```bash
-git clone https://github.com/crybot/potatorch
+git clone --single-branch -b main https://github.com/crybot/potatorch
 pip install -e potatorch
 ````
 ______________________________________________________________________
 
 ### Minimal Working Example
 You can run the following example directly from `examples/mlp.py` if you already have pytorch installed, or you can run it with docker through the provided scripts:
 ```bash
@@ -78,39 +98,32 @@
         )
 # Run the training loop
 model = training_loop.run(model, epochs=epochs)
 ```
 ______________________________________________________________________
 
 ### Automatic Hyperparameters Optimization
-PotaTorch provides a basic set of utilities to perform hyperparameters optimization. You can choose among **grid search**, **random search** and **bayesian search**. All of them are provided by `potatorch.optimization.tuning.HyperOptimizer`. The following is a working example of a simple grid search on a toy problem. You can find the full script under `exampled/grid_search.py`
+PotaTorch provides a basic set of utilities to perform hyperparameters optimization. You can choose among **grid search**, **random search** and **bayesian search**. All of them are provided by `potatorch.optimization.tuning.HyperOptimizer`. The following is a working example of a simple grid search on a toy problem. You can find the full script under `examples/grid_search.py`
 
 ```python
 def train(dataset, device, config):
     """ Your usual training function that runs a TrainingLoop instance """
-    # Fix a seed for TrainingLoop to make non-deterministic operations such as
-    # shuffling reproducible
     SEED = 42
-    # NOTE: `epochs` is a fixed hyperparameter; it won't change among runs
+    # `epochs` is a fixed hyperparameter; it won't change among runs
     epochs = config['epochs']
 
     # Define your model as a pytorch Module
     model = nn.Sequential(nn.Linear(1, 128), nn.ReLU(), 
             nn.Linear(128, 128), nn.ReLU(),
             nn.Linear(128, 1))
 
     loss_fn = torch.nn.MSELoss()
-    # Provide a loss function and an optimizer
-    # NOTE: `lr` is a dynamic hyperparameter; it will change among runs
+    # `lr` is a dynamic hyperparameter; it will change among runs
     optimizer = make_optimizer(torch.optim.Adam, lr=config['lr'])
 
-    # Construct a TrainingLoop object.
-    # TrainingLoop handles the initialization of dataloaders, dataset splitting,
-    # shuffling, mixed precision training, etc.
-    # You can provide callback handles through the `callbacks` argument.
     training_loop = TrainingLoop(
             dataset,
             loss_fn,
             optimizer,
             train_p=0.8,
             val_p=0.1,
             test_p=0.1,
@@ -121,15 +134,14 @@
             num_workers=0,
             seed=SEED,
             val_metrics={'l1': nn.L1Loss(), 'mse': nn.MSELoss()},
             callbacks=[
                 ProgressbarCallback(epochs=epochs, width=20),
                 ]
             )
-    # Run the training loop
     model = training_loop.run(model, epochs=epochs, verbose=1)
     # Return a dictionary containing the training and validation metrics 
     # calculated during the last epoch of the loop
     return training_loop.get_last_metrics()
 
 # Define your search configuration
 search_config = {
@@ -146,15 +158,14 @@
         'fixed': {      # fixed hyperparameters that won't change among runs
             'epochs': 200
         }
     }
 
 def main():
     device = 'cuda'
-    # Create your dataset as a torch.data.Dataset
     dataset = TensorDataset(torch.arange(1000).view(1000, 1), torch.sin(torch.arange(1000)))
     # Apply additional parameters to the train function to have f(config) -> {}
     score_function = partial(train, dataset, device)
     # Construct the hyperparameters optimizer
     hyperoptimizer = HyperOptimizer(search_config)
     # Run the optimization over the hyperparameters space
     config, error = hyperoptimizer.optimize(score_function, return_error=True)
```

### Comparing `potatorch-0.0.1/pyproject.toml` & `potatorch-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "potatorch"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marco Pampaloni", email="marco.pampaloni1@gmail.com" },
 ]
 description = "Lightweight high-level PyTorch framework that runs on potato machines"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `potatorch-0.0.1/PKG-INFO` & `potatorch-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-Metadata-Version: 2.1
-Name: potatorch
-Version: 0.0.1
-Summary: Lightweight high-level PyTorch framework that runs on potato machines
-Project-URL: Homepage, https://github.com/crybot/potatorch
-Project-URL: Bug Tracker, https://github.com/crybot/potatorch/issues
-Author-email: Marco Pampaloni <marco.pampaloni1@gmail.com>
-License-File: LICENSE
-Keywords: deep learning,framework,limited resources,machine learning,python,pytorch
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 
 <div align="center">
 
 # PotaTorch
 
 <img src="https://raw.githubusercontent.com/crybot/potatorch/main/potatorch.png" width="200" height="200" role="img">
 
 **PotaTorch is a lightweight PyTorch framework specifically designed to run on hardware with limited resources.**
 
 **WIP:**
 ______________________________________________________________________
 </div>
 
 ### Install PotaTorch
-PotaTorch is not currently on PyPI, so you'll have to install it from sources:
+PotaTorch is published on PyPI, you can install it through pip:
+```bash
+pip install potatorch
+```
+
+or you can install it from sources:
 ```bash
-git clone https://github.com/crybot/potatorch
+git clone --single-branch -b main https://github.com/crybot/potatorch
 pip install -e potatorch
 ````
 ______________________________________________________________________
 
 ### Minimal Working Example
 You can run the following example directly from `examples/mlp.py` if you already have pytorch installed, or you can run it with docker through the provided scripts:
 ```bash
@@ -93,39 +83,32 @@
         )
 # Run the training loop
 model = training_loop.run(model, epochs=epochs)
 ```
 ______________________________________________________________________
 
 ### Automatic Hyperparameters Optimization
-PotaTorch provides a basic set of utilities to perform hyperparameters optimization. You can choose among **grid search**, **random search** and **bayesian search**. All of them are provided by `potatorch.optimization.tuning.HyperOptimizer`. The following is a working example of a simple grid search on a toy problem. You can find the full script under `exampled/grid_search.py`
+PotaTorch provides a basic set of utilities to perform hyperparameters optimization. You can choose among **grid search**, **random search** and **bayesian search**. All of them are provided by `potatorch.optimization.tuning.HyperOptimizer`. The following is a working example of a simple grid search on a toy problem. You can find the full script under `examples/grid_search.py`
 
 ```python
 def train(dataset, device, config):
     """ Your usual training function that runs a TrainingLoop instance """
-    # Fix a seed for TrainingLoop to make non-deterministic operations such as
-    # shuffling reproducible
     SEED = 42
-    # NOTE: `epochs` is a fixed hyperparameter; it won't change among runs
+    # `epochs` is a fixed hyperparameter; it won't change among runs
     epochs = config['epochs']
 
     # Define your model as a pytorch Module
     model = nn.Sequential(nn.Linear(1, 128), nn.ReLU(), 
             nn.Linear(128, 128), nn.ReLU(),
             nn.Linear(128, 1))
 
     loss_fn = torch.nn.MSELoss()
-    # Provide a loss function and an optimizer
-    # NOTE: `lr` is a dynamic hyperparameter; it will change among runs
+    # `lr` is a dynamic hyperparameter; it will change among runs
     optimizer = make_optimizer(torch.optim.Adam, lr=config['lr'])
 
-    # Construct a TrainingLoop object.
-    # TrainingLoop handles the initialization of dataloaders, dataset splitting,
-    # shuffling, mixed precision training, etc.
-    # You can provide callback handles through the `callbacks` argument.
     training_loop = TrainingLoop(
             dataset,
             loss_fn,
             optimizer,
             train_p=0.8,
             val_p=0.1,
             test_p=0.1,
@@ -136,15 +119,14 @@
             num_workers=0,
             seed=SEED,
             val_metrics={'l1': nn.L1Loss(), 'mse': nn.MSELoss()},
             callbacks=[
                 ProgressbarCallback(epochs=epochs, width=20),
                 ]
             )
-    # Run the training loop
     model = training_loop.run(model, epochs=epochs, verbose=1)
     # Return a dictionary containing the training and validation metrics 
     # calculated during the last epoch of the loop
     return training_loop.get_last_metrics()
 
 # Define your search configuration
 search_config = {
@@ -161,15 +143,14 @@
         'fixed': {      # fixed hyperparameters that won't change among runs
             'epochs': 200
         }
     }
 
 def main():
     device = 'cuda'
-    # Create your dataset as a torch.data.Dataset
     dataset = TensorDataset(torch.arange(1000).view(1000, 1), torch.sin(torch.arange(1000)))
     # Apply additional parameters to the train function to have f(config) -> {}
     score_function = partial(train, dataset, device)
     # Construct the hyperparameters optimizer
     hyperoptimizer = HyperOptimizer(search_config)
     # Run the optimization over the hyperparameters space
     config, error = hyperoptimizer.optimize(score_function, return_error=True)
```

