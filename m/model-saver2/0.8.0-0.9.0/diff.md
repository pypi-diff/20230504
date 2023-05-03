# Comparing `tmp/model_saver2-0.8.0.tar.gz` & `tmp/model_saver2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_saver2-0.8.0.tar", last modified: Wed May  3 22:14:15 2023, max compression
+gzip compressed data, was "model_saver2-0.9.0.tar", last modified: Wed May  3 22:16:39 2023, max compression
```

## Comparing `model_saver2-0.8.0.tar` & `model_saver2-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 22:14:15.081689 model_saver2-0.8.0/
--rw-rw-rw-   0        0        0     1069 2023-05-03 20:54:23.000000 model_saver2-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     1798 2023-05-03 22:14:14.988691 model_saver2-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-03 22:13:33.000000 model_saver2-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 22:14:14.984690 model_saver2-0.8.0/model_saver2.egg-info/
--rw-rw-rw-   0        0        0     1798 2023-05-03 22:14:12.000000 model_saver2-0.8.0/model_saver2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-03 22:14:13.000000 model_saver2-0.8.0/model_saver2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 22:14:13.000000 model_saver2-0.8.0/model_saver2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 22:14:13.000000 model_saver2-0.8.0/model_saver2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 22:14:15.082689 model_saver2-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      636 2023-05-03 22:13:53.000000 model_saver2-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:16:39.161692 model_saver2-0.9.0/
+-rw-rw-rw-   0        0        0     1069 2023-05-03 20:54:23.000000 model_saver2-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2412 2023-05-03 22:16:39.157688 model_saver2-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-05-03 22:16:30.000000 model_saver2-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 22:16:39.154690 model_saver2-0.9.0/model_saver2.egg-info/
+-rw-rw-rw-   0        0        0     2412 2023-05-03 22:16:38.000000 model_saver2-0.9.0/model_saver2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-03 22:16:38.000000 model_saver2-0.9.0/model_saver2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:16:38.000000 model_saver2-0.9.0/model_saver2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:16:38.000000 model_saver2-0.9.0/model_saver2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 22:16:39.161692 model_saver2-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      636 2023-05-03 22:15:13.000000 model_saver2-0.9.0/setup.py
```

### Comparing `model_saver2-0.8.0/LICENSE` & `model_saver2-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_saver2-0.8.0/PKG-INFO` & `model_saver2-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_saver2
-Version: 0.8.0
+Version: 0.9.0
 Summary: A class for saving and loading machine learning models
 Home-page: https://github.com/somkietacode/modelSaver
 Author: somkietacode
 Author-email: s.r.a.ouedraogo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,33 +14,58 @@
 ## Class ModelSaver
 The ModelSaver class is a utility for saving and loading trained machine learning models in Python. It allows you to save any Python object as a binary file, which can be loaded later to restore the original object. This class is especially useful for saving trained models, as you can save the entire model architecture and trained parameters in a single file, which can be loaded and used to make predictions later.
 
 ## Installation
 You can install the ModelSaver class using pip. Simply run the following command:
 
 ```
-pip install model-saver
+pip install model-saver2
 ```
 ## Usage
 To use the ModelSaver class, you first need to import it in your Python script:
 
 ```python
 from model_saver2 import ModelSaver
 Then, you can create an instance of the class and use it to save your trained model:
 ```
 
 ```python
 my_model = ...  # Trained model object
-saver = ModelSaver('my_model.model')
-saver.save(my_model)
+saver = ModelSaver()
+saver.save(my_model,'my_model.model')
 This will save the my_model object to a file named my_model.model in binary format.
 ```
 To load the saved model, you can use the load method of the ModelSaver class:
 
 ```python
-saver = ModelSaver('my_model.model')
-my_model = saver.load()
+saver = ModelSaver()
+my_model = saver.load('my_model.model')
 This will load the my_model object from the file my_model.model.
 ```
 
+## Exemple
+
+```python
+from model_saver2 import ModelSaver
+import numpy as np
+from sklearn.linear_model import LinearRegression
+
+# Train a linear regression model on some data
+X = np.array([[1, 1], [1, 2], [2, 2], [2, 3]])
+y = np.dot(X, np.array([1, 2])) + 3
+model = LinearRegression().fit(X, y)
+
+# Save the model to a file
+saver = ModelSaver('models', 'my_model')
+saver.save(model)
+
+# Load the model from the file
+loaded_model = saver.load()
+
+# Use the loaded model to make predictions
+new_X = np.array([[3, 5], [4, 6]])
+predictions = loaded_model.predict(new_X)
+print(predictions)
+```
+
 ## License
 This project is licensed under the MIT License - see the LICENSE.md file for details.
```

### Comparing `model_saver2-0.8.0/model_saver2.egg-info/PKG-INFO` & `model_saver2-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-Metadata-Version: 2.1
-Name: model-saver2
-Version: 0.8.0
-Summary: A class for saving and loading machine learning models
-Home-page: https://github.com/somkietacode/modelSaver
-Author: somkietacode
-Author-email: s.r.a.ouedraogo@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Class ModelSaver
-The ModelSaver class is a utility for saving and loading trained machine learning models in Python. It allows you to save any Python object as a binary file, which can be loaded later to restore the original object. This class is especially useful for saving trained models, as you can save the entire model architecture and trained parameters in a single file, which can be loaded and used to make predictions later.
-
-## Installation
-You can install the ModelSaver class using pip. Simply run the following command:
-
-```
-pip install model-saver
-```
-## Usage
-To use the ModelSaver class, you first need to import it in your Python script:
-
-```python
-from model_saver2 import ModelSaver
-Then, you can create an instance of the class and use it to save your trained model:
-```
-
-```python
-my_model = ...  # Trained model object
-saver = ModelSaver('my_model.model')
-saver.save(my_model)
-This will save the my_model object to a file named my_model.model in binary format.
-```
-To load the saved model, you can use the load method of the ModelSaver class:
-
-```python
-saver = ModelSaver('my_model.model')
-my_model = saver.load()
-This will load the my_model object from the file my_model.model.
-```
-
-## License
-This project is licensed under the MIT License - see the LICENSE.md file for details.
+## Class ModelSaver
+The ModelSaver class is a utility for saving and loading trained machine learning models in Python. It allows you to save any Python object as a binary file, which can be loaded later to restore the original object. This class is especially useful for saving trained models, as you can save the entire model architecture and trained parameters in a single file, which can be loaded and used to make predictions later.
+
+## Installation
+You can install the ModelSaver class using pip. Simply run the following command:
+
+```
+pip install model-saver2
+```
+## Usage
+To use the ModelSaver class, you first need to import it in your Python script:
+
+```python
+from model_saver2 import ModelSaver
+Then, you can create an instance of the class and use it to save your trained model:
+```
+
+```python
+my_model = ...  # Trained model object
+saver = ModelSaver()
+saver.save(my_model,'my_model.model')
+This will save the my_model object to a file named my_model.model in binary format.
+```
+To load the saved model, you can use the load method of the ModelSaver class:
+
+```python
+saver = ModelSaver()
+my_model = saver.load('my_model.model')
+This will load the my_model object from the file my_model.model.
+```
+
+## Exemple
+
+```python
+from model_saver2 import ModelSaver
+import numpy as np
+from sklearn.linear_model import LinearRegression
+
+# Train a linear regression model on some data
+X = np.array([[1, 1], [1, 2], [2, 2], [2, 3]])
+y = np.dot(X, np.array([1, 2])) + 3
+model = LinearRegression().fit(X, y)
+
+# Save the model to a file
+saver = ModelSaver('models', 'my_model')
+saver.save(model)
+
+# Load the model from the file
+loaded_model = saver.load()
+
+# Use the loaded model to make predictions
+new_X = np.array([[3, 5], [4, 6]])
+predictions = loaded_model.predict(new_X)
+print(predictions)
+```
+
+## License
+This project is licensed under the MIT License - see the LICENSE.md file for details.
```

### Comparing `model_saver2-0.8.0/setup.py` & `model_saver2-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='model_saver2',
-    version='0.8.0',
+    version='0.9.0',
     packages=find_packages(),
     author='somkietacode',
     author_email='s.r.a.ouedraogo@gmail.com',
     description='A class for saving and loading machine learning models',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/somkietacode/modelSaver',
```

