# Comparing `tmp/image-similarity-measures-0.3.5.tar.gz` & `tmp/image_similarity_measures-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-similarity-measures-0.3.5.tar", last modified: Mon Feb  8 12:40:01 2021, max compression
+gzip compressed data, was "image_similarity_measures-0.3.6.tar", max compression
```

## Comparing `image-similarity-measures-0.3.5.tar` & `image_similarity_measures-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxr-xr-x   0 nikoo.ekhtiari   (501) staff       (20)        0 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)     4536 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/PKG-INFO
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)     3226 2021-02-08 12:03:49.000000 image-similarity-measures-0.3.5/README.md
-drwxr-xr-x   0 nikoo.ekhtiari   (501) staff       (20)        0 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures/
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)        0 2021-02-08 12:03:49.000000 image-similarity-measures-0.3.5/image_similarity_measures/__init__.py
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)     2094 2021-02-08 12:03:49.000000 image-similarity-measures-0.3.5/image_similarity_measures/evaluate.py
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)    10922 2021-02-08 12:03:49.000000 image-similarity-measures-0.3.5/image_similarity_measures/quality_metrics.py
-drwxr-xr-x   0 nikoo.ekhtiari   (501) staff       (20)        0 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)     4536 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/PKG-INFO
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)      435 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/SOURCES.txt
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)        1 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/dependency_links.txt
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)       87 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/entry_points.txt
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)       59 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/requires.txt
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)       26 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/image_similarity_measures.egg-info/top_level.txt
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)       38 2021-02-08 12:40:01.000000 image-similarity-measures-0.3.5/setup.cfg
--rw-r--r--   0 nikoo.ekhtiari   (501) staff       (20)     1049 2021-02-08 12:37:44.000000 image-similarity-measures-0.3.5/setup.py
+-rw-r--r--   0        0        0     1061 2023-03-31 11:57:19.364261 image_similarity_measures-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3003 2023-04-14 11:41:10.868827 image_similarity_measures-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 11:57:19.392036 image_similarity_measures-0.3.6/image_similarity_measures/__init__.py
+-rw-r--r--   0        0        0     2311 2023-03-31 11:57:19.393397 image_similarity_measures-0.3.6/image_similarity_measures/evaluate.py
+-rw-r--r--   0        0        0    12094 2023-05-04 09:05:07.324153 image_similarity_measures-0.3.6/image_similarity_measures/quality_metrics.py
+-rw-r--r--   0        0        0      960 2023-05-04 13:37:40.239610 image_similarity_measures-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 image_similarity_measures-0.3.6/setup.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 image_similarity_measures-0.3.6/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `image-similarity-measures-0.3.5/PKG-INFO` & `image_similarity_measures-0.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,107 @@
 Metadata-Version: 2.1
 Name: image-similarity-measures
-Version: 0.3.5
+Version: 0.3.6
 Summary: Evaluation metrics to assess the similarity between two images.
-Home-page: https://github.com/up42/image-similarity-measures
+License: MIT
 Author: UP42
 Author-email: support@up42.com
-License: MIT
-Description: # Image Similarity Measures
-        
-        Implementation of eight evaluation metrics to access the similarity between two images. The eight metrics are as follows:
-        
-         * <i><a href="https://en.wikipedia.org/wiki/Root-mean-square_deviation">Root mean square error (RMSE)</a></i>,
-         * <i><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio (PSNR)</a></i>,
-         * <i><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural Similarity Index (SSIM)</a></i>,
-         * <i><a href="https://www4.comp.polyu.edu.hk/~cslzhang/IQA/TIP_IQA_FSIM.pdf">Feature-based similarity index (FSIM)</a></i>,
-         * <i><a href="https://www.tandfonline.com/doi/full/10.1080/22797254.2019.1628617">Information theoretic-based Statistic Similarity Measure (ISSM)</a></i>,
-         * <i><a href="https://www.sciencedirect.com/science/article/abs/pii/S0924271618302636">Signal to reconstruction error ratio (SRE)</a></i>,
-         * <i><a href="https://ntrs.nasa.gov/citations/19940012238">Spectral angle mapper (SAM)</a></i>, and
-         * <i><a href="https://ece.uwaterloo.ca/~z70wang/publications/quality_2c.pdf">Universal image quality index (UIQ)</a></i>
-        
-        ## Instructions
-        
-        The following step-by-step instructions will guide you through installing this package and run evaluation using the command line tool.
-        
-        **Note:** Supported python versions are 3.6, 3.7, 3.8, and 3.9.
-        
-        ### Install package
-        ```bash
-        pip install image-similarity-measures
-        ```
-        
-        ### Usage
-        #### Parameters
-        ```
-          --org_img_path FILE   Path to original input image
-          --pred_img_path FILE  Path to predicted image
-          --metric METRIC       select an evaluation metric (fsim, issm, psnr, rmse,
-                                sam, sre, ssim, uiq, all) (can be repeated)
-        ```
-        
-        #### Evaluation
-        For doing the evaluation, you can easily run the following command:
-        
-        ```bash
-        image-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif
-        ```
-        The results are printed in machine-readable JSON, so you can redirect the output of the command into a file.
-        
-        **Note** that images that are used for evaluation should be **channel last**.
-        
-        #### Usage in python
-        ```bash
-        import image_similarity_measures
-        from image_similarity_measures.quality_metrics import rmse, psnr
-        ```
-        
-        ### Install package from source
-        
-        #### Clone the repository
-        
-        ```bash
-        git clone https://github.com/up42/image-similarity-measures.git
-        cd image-similarity-measures
-        ```
-        
-        Then navigate to the folder via `cd image-similarity-measures`.
-        
-        #### Installing the required libraries
-        
-        First create a new virtual environment called `similarity-measures`, for example by using
-        [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/):
-        
-        ```bash
-        mkvirtualenv --python=$(which python3.7) similarity-measures
-        ```
-        
-        Activate the new environment:
-        
-        ```bash
-        workon similarity-measures
-        ```
-        
-        Install the necessary Python libraries via:
-        
-        ```bash
-        bash setup.sh
-        ```
-        
-        ## Citation
-        Please use the following for citation purposes of this codebase:
-        
-        <strong>Müller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF MULTISPECTRAL
-        SATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann. Photogramm. Remote Sens.
-        Spatial Inf. Sci., V-1-2020, 33–40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.</strong>
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: rasterio
+Provides-Extra: speedups
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: phasepack (>=1.5,<2.0)
+Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
+
+# Image Similarity Measures
+
+Python package and commandline tool to evaluate the similarity between two images with eight evaluation metrics:
+
+ * <i><a href="https://en.wikipedia.org/wiki/Root-mean-square_deviation">Root mean square error (RMSE)</a></i>
+ * <i><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio (PSNR)</a></i>
+ * <i><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural Similarity Index (SSIM)</a></i>
+ * <i><a href="https://www4.comp.polyu.edu.hk/~cslzhang/IQA/TIP_IQA_FSIM.pdf">Feature-based similarity index (FSIM)</a></i>
+ * <i><a href="https://www.tandfonline.com/doi/full/10.1080/22797254.2019.1628617">Information theoretic-based Statistic Similarity Measure (ISSM)</a></i>
+ * <i><a href="https://www.sciencedirect.com/science/article/abs/pii/S0924271618302636">Signal to reconstruction error ratio (SRE)</a></i>
+ * <i><a href="https://ntrs.nasa.gov/citations/19940012238">Spectral angle mapper (SAM)</a></i>
+ * <i><a href="https://ece.uwaterloo.ca/~z70wang/publications/quality_2c.pdf">Universal image quality index (UIQ)</a></i>
+
+## Installation
+
+Supports Python >=3.8.
+
+```bash
+pip install image-similarity-measures
+```
+
+*Optional*: For faster evaluation of the FSIM metric, the `pyfftw` package is required, install via:
+
+```bash
+pip install image-similarity-measures[speedups]
+```
+
+*Optional*: For reading TIFF images with `rasterio` instead of `OpenCV`, install:
+
+```bash
+pip install image-similarity-measures[rasterio]
+```
+
+
+## Usage on commandline
+
+To evaluate the similarity beteween two images, run on the commandline:
+
+```bash
+image-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif
+```
+
+**Note** that images that are used for evaluation should be **channel last**. The results are printed in 
+machine-readable JSON, so you can redirect the output of the command into a file.
+
+#### Parameters
+```
+  --org_img_path FILE   Path to original input image
+  --pred_img_path FILE  Path to predicted image
+  --metric METRIC       select an evaluation metric (fsim, issm, psnr, rmse,
+                        sam, sre, ssim, uiq, all) (can be repeated)
+```
+
+## Usage in Python
+
+```bash
+from image_similarity_measures.evaluate import evaluation
+
+evaluation(org_img_path="example/lafayette_org.tif", 
+           pred_img_path="example/lafayette_pred.tif", 
+           metrics=["rmse", "psnr"])
+```
+
+```bash
+from image_similarity_measures.quality_metrics import rmse
+
+rmse(org_img=np.random.rand(3,2,1), pred_img=np.random.rand(3,2,1))
+```
+
+## Contribute
+
+Contributions are welcome! Please see README-dev.md for instructions.
+
+
+## Citation
+Please use the following for citation purposes of this codebase:
+
+<strong>Müller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF MULTISPECTRAL
+SATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann. Photogramm. Remote Sens.
+Spatial Inf. Sci., V-1-2020, 33–40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.</strong>
+
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
-Metadata-Version: 2.1 Name: image-similarity-measures Version: 0.3.5 Summary:
-Evaluation metrics to assess the similarity between two images. Home-page:
-https://github.com/up42/image-similarity-measures Author: UP42 Author-email:
-support@up42.com License: MIT Description: # Image Similarity Measures
-Implementation of eight evaluation metrics to access the similarity between two
-images. The eight metrics are as follows: * Root_mean_square_error_(RMSE), *
-Peak_signal-to-noise_ratio_(PSNR), * Structural_Similarity_Index_(SSIM), *
-Feature-based_similarity_index_(FSIM), * Information_theoretic-based_Statistic
-Similarity_Measure_(ISSM), * Signal_to_reconstruction_error_ratio_(SRE), *
-Spectral_angle_mapper_(SAM), and * Universal_image_quality_index_(UIQ) ##
-Instructions The following step-by-step instructions will guide you through
-installing this package and run evaluation using the command line tool. **Note:
-** Supported python versions are 3.6, 3.7, 3.8, and 3.9. ### Install package
-```bash pip install image-similarity-measures ``` ### Usage #### Parameters ```
+Metadata-Version: 2.1 Name: image-similarity-measures Version: 0.3.6 Summary:
+Evaluation metrics to assess the similarity between two images. License: MIT
+Author: UP42 Author-email: support@up42.com Requires-Python: >=3.8 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Provides-Extra: rasterio Provides-Extra: speedups
+Requires-Dist: numpy (>=1.24.2,<2.0.0) Requires-Dist: opencv-python
+(>=4.7.0.72,<5.0.0.0) Requires-Dist: phasepack (>=1.5,<2.0) Requires-Dist:
+scikit-image (>=0.20.0,<0.21.0) Description-Content-Type: text/markdown # Image
+Similarity Measures Python package and commandline tool to evaluate the
+similarity between two images with eight evaluation metrics: * Root_mean_square
+error_(RMSE) * Peak_signal-to-noise_ratio_(PSNR) * Structural_Similarity_Index_
+(SSIM) * Feature-based_similarity_index_(FSIM) * Information_theoretic-based
+Statistic_Similarity_Measure_(ISSM) * Signal_to_reconstruction_error_ratio_
+(SRE) * Spectral_angle_mapper_(SAM) * Universal_image_quality_index_(UIQ) ##
+Installation Supports Python >=3.8. ```bash pip install image-similarity-
+measures ``` *Optional*: For faster evaluation of the FSIM metric, the `pyfftw`
+package is required, install via: ```bash pip install image-similarity-measures
+[speedups] ``` *Optional*: For reading TIFF images with `rasterio` instead of
+`OpenCV`, install: ```bash pip install image-similarity-measures[rasterio] ```
+## Usage on commandline To evaluate the similarity beteween two images, run on
+the commandline: ```bash image-similarity-measures --org_img_path=a.tif --
+pred_img_path=b.tif ``` **Note** that images that are used for evaluation
+should be **channel last**. The results are printed in machine-readable JSON,
+so you can redirect the output of the command into a file. #### Parameters ```
 --org_img_path FILE Path to original input image --pred_img_path FILE Path to
 predicted image --metric METRIC select an evaluation metric (fsim, issm, psnr,
-rmse, sam, sre, ssim, uiq, all) (can be repeated) ``` #### Evaluation For doing
-the evaluation, you can easily run the following command: ```bash image-
-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif ``` The results
-are printed in machine-readable JSON, so you can redirect the output of the
-command into a file. **Note** that images that are used for evaluation should
-be **channel last**. #### Usage in python ```bash import
-image_similarity_measures from image_similarity_measures.quality_metrics import
-rmse, psnr ``` ### Install package from source #### Clone the repository
-```bash git clone https://github.com/up42/image-similarity-measures.git cd
-image-similarity-measures ``` Then navigate to the folder via `cd image-
-similarity-measures`. #### Installing the required libraries First create a new
-virtual environment called `similarity-measures`, for example by using
-[virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/):
-```bash mkvirtualenv --python=$(which python3.7) similarity-measures ```
-Activate the new environment: ```bash workon similarity-measures ``` Install
-the necessary Python libraries via: ```bash bash setup.sh ``` ## Citation
-Please use the following for citation purposes of this codebase: MÃ¼ller, M.
-U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF
-MULTISPECTRAL SATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann.
-Photogramm. Remote Sens. Spatial Inf. Sci., V-1-2020, 33â40, https://doi.org/
-10.5194/isprs-annals-V-1-2020-33-2020, 2020. Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Intended
-Audience :: Science/Research Classifier: Development Status :: 5 - Production/
-Stable Requires-Python: >=3.6, <3.10 Description-Content-Type: text/markdown
+rmse, sam, sre, ssim, uiq, all) (can be repeated) ``` ## Usage in Python
+```bash from image_similarity_measures.evaluate import evaluation evaluation
+(org_img_path="example/lafayette_org.tif", pred_img_path="example/
+lafayette_pred.tif", metrics=["rmse", "psnr"]) ``` ```bash from
+image_similarity_measures.quality_metrics import rmse rmse
+(org_img=np.random.rand(3,2,1), pred_img=np.random.rand(3,2,1)) ``` ##
+Contribute Contributions are welcome! Please see README-dev.md for
+instructions. ## Citation Please use the following for citation purposes of
+this codebase: MÃ¼ller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke, C.:
+SUPER-RESOLUTION OF MULTISPECTRAL SATELLITE IMAGES USING CONVOLUTIONAL NEURAL
+NETWORKS, ISPRS Ann. Photogramm. Remote Sens. Spatial Inf. Sci., V-1-2020,
+33â40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.
```

### Comparing `image-similarity-measures-0.3.5/image_similarity_measures/evaluate.py` & `image_similarity_measures-0.3.6/image_similarity_measures/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import argparse
 import json
 import logging
 import os
+from typing import List
 
 import cv2
 import numpy as np
-import rasterio as rio
+
+try:
+    import rasterio
+except ImportError:
+    rasterio = None
 
 from image_similarity_measures.quality_metrics import metric_functions
 
 logger = logging.getLogger(__name__)
 
 
-def read_image(path):
-    logger.info("Reading image %s", os.path.basename(path))
-    if path.endswith(".tif") or path.endswith(".tiff"):
-        return np.rollaxis(rio.open(path).read(), 0, 3)
+def read_image(path: str):
+    logger.info(f"Reading image {os.path.basename(path)}")
+    if rasterio and (path.endswith(".tif") or path.endswith(".tiff")):
+        return np.rollaxis(rasterio.open(path).read(), 0, 3)
     return cv2.imread(path)
 
 
-def evaluation(org_img_path, pred_img_path, metrics):
+def evaluation(org_img_path: str, pred_img_path: str, metrics: List[str]):
     output_dict = {}
     org_img = read_image(org_img_path)
     pred_img = read_image(pred_img_path)
 
     for metric in metrics:
         metric_func = metric_functions[metric]
         out_value = float(metric_func(org_img, pred_img))
@@ -34,30 +39,48 @@
 
 def main():
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
         level=logging.INFO,
     )
     all_metrics = sorted(metric_functions.keys())
-    parser = argparse.ArgumentParser(description="Evaluates an Image Super Resolution Model")
-    parser.add_argument("--org_img_path", help="Path to original input image", required=True, metavar="FILE")
-    parser.add_argument("--pred_img_path", help="Path to predicted image", required=True, metavar="FILE")
-    parser.add_argument("--metric", dest="metrics", action="append",
-                        choices=all_metrics + ['all'], metavar="METRIC",
-                        help="select an evaluation metric (%(choices)s) (can be repeated)")
+    parser = argparse.ArgumentParser(
+        description="Evaluates an Image Super Resolution Model"
+    )
+    parser.add_argument(
+        "--org_img_path",
+        help="Path to original input image",
+        required=True,
+        metavar="FILE",
+    )
+    parser.add_argument(
+        "--pred_img_path", help="Path to predicted image", required=True, metavar="FILE"
+    )
+    parser.add_argument(
+        "--metric",
+        dest="metrics",
+        action="append",
+        choices=all_metrics + ["all"],
+        metavar="METRIC",
+        help="select an evaluation metric (%(choices)s) (can be repeated)",
+    )
     args = parser.parse_args()
     if not args.metrics:
         args.metrics = ["psnr"]
     if "all" in args.metrics:
         args.metrics = all_metrics
 
     metric_values = evaluation(
         org_img_path=args.org_img_path,
         pred_img_path=args.pred_img_path,
         metrics=args.metrics,
     )
-    result_dict = {"image1": args.org_img_path, "image2": args.pred_img_path, "metrics": metric_values}
+    result_dict = {
+        "image1": args.org_img_path,
+        "image2": args.pred_img_path,
+        "metrics": metric_values,
+    }
     print(json.dumps(result_dict, sort_keys=True))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `image-similarity-measures-0.3.5/image_similarity_measures/quality_metrics.py` & `image_similarity_measures-0.3.6/image_similarity_measures/quality_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,100 @@
 """
 This module is a collection of metrics to assess the similarity between two images.
-PSNR, SSIM, FSIM and ISSM are the current metrics that are implemented in this module.
+Currently implemented metrics are FSIM, ISSM, PSNR, RMSE, SAM, SRE, SSIM, UIQ.
 """
+
 import math
 
 import numpy as np
 from skimage.metrics import structural_similarity
 import phasepack.phasecong as pc
 import cv2
 
 
 def _assert_image_shapes_equal(org_img: np.ndarray, pred_img: np.ndarray, metric: str):
-    msg = (f"Cannot calculate {metric}. Input shapes not identical. y_true shape ="
-           f"{str(org_img.shape)}, y_pred shape = {str(pred_img.shape)}")
+    # shape of the image should be like this (rows, cols, bands)
+    # Please note that: The interpretation of a 3-dimension array read from rasterio is: (bands, rows, columns) while
+    # image processing software like scikit-image, pillow and matplotlib are generally ordered: (rows, columns, bands)
+    # in order efficiently swap the axis order one can use reshape_as_raster, reshape_as_image from rasterio.plot
+    msg = (
+        f"Cannot calculate {metric}. Input shapes not identical. y_true shape ="
+        f"{str(org_img.shape)}, y_pred shape = {str(pred_img.shape)}"
+    )
 
     assert org_img.shape == pred_img.shape, msg
 
-def rmse(org_img: np.ndarray, pred_img: np.ndarray, max_p=4095) -> float:
+
+def rmse(org_img: np.ndarray, pred_img: np.ndarray, max_p: int = 4095) -> float:
     """
     Root Mean Squared Error
 
     Calculated individually for all bands, then averaged
     """
     _assert_image_shapes_equal(org_img, pred_img, "RMSE")
 
     org_img = org_img.astype(np.float32)
-
+    
+    # if image is a gray image - add empty 3rd dimension for the .shape[2] to exist
+    if org_img.ndim == 2:
+        org_img = np.expand_dims(org_img, axis=-1)
+    
     rmse_bands = []
-    for i in range(org_img.shape[2]):
-        dif = np.subtract(org_img, pred_img)
-        m = np.mean(np.square( dif / max_p))
-        s = np.sqrt(m)
-        rmse_bands.append(s)
-
+    diff = org_img - pred_img
+    mse_bands = np.mean(np.square(diff / max_p), axis=(0, 1))
+    rmse_bands = np.sqrt(mse_bands)
     return np.mean(rmse_bands)
 
 
-def psnr(org_img: np.ndarray, pred_img: np.ndarray, max_p=4095) -> float:
+def psnr(org_img: np.ndarray, pred_img: np.ndarray, max_p: int = 4095) -> float:
     """
     Peek Signal to Noise Ratio, implemented as mean squared error converted to dB.
 
     It can be calculated as
     PSNR = 20 * log10(MAXp) - 10 * log10(MSE)
 
     When using 12-bit imagery MaxP is 4095, for 8-bit imagery 255. For floating point imagery using values between
     0 and 1 (e.g. unscaled reflectance) the first logarithmic term can be dropped as it becomes 0
     """
     _assert_image_shapes_equal(org_img, pred_img, "PSNR")
 
     org_img = org_img.astype(np.float32)
+    
+    # if image is a gray image - add empty 3rd dimension for the .shape[2] to exist
+    if org_img.ndim == 2:
+        org_img = np.expand_dims(org_img, axis=-1)
+        
+    mse_bands = np.mean(np.square(org_img - pred_img), axis=(0, 1))
+    mse = np.mean(mse_bands)
+    return 20 * np.log10(max_p / np.sqrt(mse))
 
-    mse_bands = []
-    for i in range(org_img.shape[2]):
-        mse_bands.append(np.mean(np.square(org_img[:, :, i] - pred_img[:, :, i])))
-
-    return 20 * np.log10(max_p) - 10. * np.log10(np.mean(mse_bands))
 
-
-def _similarity_measure(x, y, constant):
+def _similarity_measure(x: np.array, y: np.array, constant: float):
     """
     Calculate feature similarity measurement between two images
     """
-    numerator = 2 * x * y + constant
-    denominator = x ** 2 + y ** 2 + constant
+    numerator = 2 * np.multiply(x, y) + constant
+    denominator = np.add(np.square(x), np.square(y)) + constant
 
-    return numerator / denominator
+    return np.divide(numerator, denominator)
 
 
-def _gradient_magnitude(img: np.ndarray, img_depth):
+def _gradient_magnitude(img: np.ndarray, img_depth: int):
     """
-    Calculate gradient magnitude based on Scharr operator
+    Calculate gradient magnitude based on Scharr operator.
     """
     scharrx = cv2.Scharr(img, img_depth, 1, 0)
     scharry = cv2.Scharr(img, img_depth, 0, 1)
 
-    return np.sqrt(scharrx ** 2 + scharry ** 2)
+    return np.sqrt(scharrx**2 + scharry**2)
 
 
-def fsim(org_img: np.ndarray, pred_img: np.ndarray, T1=0.85, T2=160) -> float:
+def fsim(
+    org_img: np.ndarray, pred_img: np.ndarray, T1: float = 0.85, T2: float = 160
+) -> float:
     """
     Feature-based similarity index, based on phase congruency (PC) and image gradient magnitude (GM)
 
     There are different ways to implement PC, the authors of the original FSIM paper use the method
     defined by Kovesi (1999). The Python phasepack project fortunately provides an implementation
     of the approach.
 
@@ -98,71 +111,83 @@
     Args:
         org_img -- numpy array containing the original image
         pred_img -- predicted image
         T1 -- constant based on the dynamic range of PC values
         T2 -- constant based on the dynamic range of GM values
     """
     _assert_image_shapes_equal(org_img, pred_img, "FSIM")
-
-    alpha = beta = 1  # parameters used to adjust the relative importance of PC and GM features
+    
+    # if image is a gray image - add empty 3rd dimension for the .shape[2] to exist
+    if org_img.ndim == 2:
+        org_img = np.expand_dims(org_img, axis=-1)
+
+    alpha = (
+        beta
+    ) = 1  # parameters used to adjust the relative importance of PC and GM features
     fsim_list = []
     for i in range(org_img.shape[2]):
         # Calculate the PC for original and predicted images
-        pc1_2dim = pc(org_img[:, :, i], nscale=4, minWaveLength=6, mult=2, sigmaOnf=0.5978)
-        pc2_2dim = pc(pred_img[:, :, i], nscale=4, minWaveLength=6, mult=2, sigmaOnf=0.5978)
+        pc1_2dim = pc(
+            org_img[:, :, i], nscale=4, minWaveLength=6, mult=2, sigmaOnf=0.5978
+        )
+        pc2_2dim = pc(
+            pred_img[:, :, i], nscale=4, minWaveLength=6, mult=2, sigmaOnf=0.5978
+        )
 
         # pc1_2dim and pc2_2dim are tuples with the length 7, we only need the 4th element which is the PC.
         # The PC itself is a list with the size of 6 (number of orientation). Therefore, we need to
         # calculate the sum of all these 6 arrays.
         pc1_2dim_sum = np.zeros((org_img.shape[0], org_img.shape[1]), dtype=np.float64)
-        pc2_2dim_sum = np.zeros((pred_img.shape[0], pred_img.shape[1]), dtype=np.float64)
+        pc2_2dim_sum = np.zeros(
+            (pred_img.shape[0], pred_img.shape[1]), dtype=np.float64
+        )
         for orientation in range(6):
             pc1_2dim_sum += pc1_2dim[4][orientation]
             pc2_2dim_sum += pc2_2dim[4][orientation]
 
         # Calculate GM for original and predicted images based on Scharr operator
         gm1 = _gradient_magnitude(org_img[:, :, i], cv2.CV_16U)
         gm2 = _gradient_magnitude(pred_img[:, :, i], cv2.CV_16U)
 
         # Calculate similarity measure for PC1 and PC2
         S_pc = _similarity_measure(pc1_2dim_sum, pc2_2dim_sum, T1)
         # Calculate similarity measure for GM1 and GM2
         S_g = _similarity_measure(gm1, gm2, T2)
 
-        S_l = (S_pc ** alpha) * (S_g ** beta)
+        S_l = (S_pc**alpha) * (S_g**beta)
 
         numerator = np.sum(S_l * np.maximum(pc1_2dim_sum, pc2_2dim_sum))
         denominator = np.sum(np.maximum(pc1_2dim_sum, pc2_2dim_sum))
         fsim_list.append(numerator / denominator)
 
     return np.mean(fsim_list)
 
 
-def _ehs(x, y):
+def _ehs(x: np.ndarray, y: np.ndarray):
     """
     Entropy-Histogram Similarity measure
     """
     H = (np.histogram2d(x.flatten(), y.flatten()))[0]
 
     return -np.sum(np.nan_to_num(H * np.log2(H)))
 
 
-def _edge_c(x, y):
+def _edge_c(x: np.ndarray, y: np.ndarray):
     """
     Edge correlation coefficient based on Canny detector
     """
     # Use 100 and 200 as thresholds, no indication in the paper what was used
     g = cv2.Canny((x * 0.0625).astype(np.uint8), 100, 200)
     h = cv2.Canny((y * 0.0625).astype(np.uint8), 100, 200)
 
     g0 = np.mean(g)
     h0 = np.mean(h)
 
     numerator = np.sum((g - g0) * (h - h0))
-    denominator = np.sqrt(np.sum(np.square(g-g0)) * np.sum(np.square(h-h0)))
+    denominator = np.sqrt(np.sum(np.square(g - g0)) * np.sum(np.square(h - h0)))
 
     return numerator / denominator
 
 
 def issm(org_img: np.ndarray, pred_img: np.ndarray) -> float:
     """
     Information theoretic-based Statistic Similarity Measure
@@ -184,110 +209,126 @@
 
     numerator = canny_val * ehs_val * (A + B) + math.e
     denominator = A * canny_val * ehs_val + B * ehs_val + C * ssim(x, y) + math.e
 
     return np.nan_to_num(numerator / denominator)
 
 
-def ssim(org_img: np.ndarray, pred_img: np.ndarray, max_p=4095) -> float:
+def ssim(org_img: np.ndarray, pred_img: np.ndarray, max_p: int = 4095) -> float:
     """
-    Structural SIMularity index
+    Structural Simularity Index
     """
     _assert_image_shapes_equal(org_img, pred_img, "SSIM")
 
-    return structural_similarity(org_img, pred_img, data_range=max_p, multichannel=True)
+    return structural_similarity(org_img, pred_img, data_range=max_p, channel_axis=2)
 
 
-def sliding_window(image, stepSize, windowSize):
+def sliding_window(image: np.ndarray, stepSize: int, windowSize: int):
     # slide a window across the image
     for y in range(0, image.shape[0], stepSize):
         for x in range(0, image.shape[1], stepSize):
             # yield the current window
-            yield (x, y, image[y:y + windowSize[1], x:x + windowSize[0]])
+            yield (x, y, image[y : y + windowSize[1], x : x + windowSize[0]])
 
 
-def uiq(org_img: np.ndarray, pred_img: np.ndarray, step_size=1, window_size=8):
+def uiq(
+    org_img: np.ndarray, pred_img: np.ndarray, step_size: int = 1, window_size: int = 8
+) -> float:
     """
     Universal Image Quality index
     """
-    # TODO: Apply optimization, right now it is very slow
     _assert_image_shapes_equal(org_img, pred_img, "UIQ")
 
     org_img = org_img.astype(np.float32)
     pred_img = pred_img.astype(np.float32)
 
     q_all = []
-    for (x, y, window_org), (x, y, window_pred) in zip(sliding_window(org_img, stepSize=step_size,
-                                                                      windowSize=(window_size, window_size)),
-                                                       sliding_window(pred_img, stepSize=step_size,
-                                                                      windowSize=(window_size, window_size))):
+    for (x, y, window_org), (x, y, window_pred) in zip(
+        sliding_window(
+            org_img, stepSize=step_size, windowSize=(window_size, window_size)
+        ),
+        sliding_window(
+            pred_img, stepSize=step_size, windowSize=(window_size, window_size)
+        ),
+    ):
         # if the window does not meet our desired window size, ignore it
         if window_org.shape[0] != window_size or window_org.shape[1] != window_size:
             continue
-
-        for i in range(org_img.shape[2]):
-            org_band = window_org[:, :, i]
-            pred_band = window_pred[:, :, i]
-            org_band_mean = np.mean(org_band)
-            pred_band_mean = np.mean(pred_band)
-            org_band_variance = np.var(org_band)
-            pred_band_variance = np.var(pred_band)
-            org_pred_band_variance = np.mean((org_band - org_band_mean) * (pred_band - pred_band_mean))
-
-            numerator = 4 * org_pred_band_variance * org_band_mean * pred_band_mean
-            denominator = (org_band_variance + pred_band_variance) * (org_band_mean**2 + pred_band_mean**2)
-
-            if denominator != 0.0:
-                q = numerator / denominator
-                q_all.append(q)
-
-    if not np.any(q_all):
-        raise ValueError(f"Window size ({window_size}) is too big for image with shape "
-                         f"{org_img.shape[0:2]}, please use a smaller window size.")
+        
+        # if image is a gray image - add empty 3rd dimension for the .shape[2] to exist
+        if org_img.ndim == 2:
+            org_img = np.expand_dims(org_img, axis=-1)
+
+        org_band = window_org.transpose(2, 0, 1).reshape(-1, window_size ** 2)
+        pred_band = window_pred.transpose(2, 0, 1).reshape(-1, window_size ** 2)
+        org_band_mean = np.mean(org_band, axis=1, keepdims=True)
+        pred_band_mean = np.mean(pred_band, axis=1, keepdims=True)
+        org_band_variance = np.var(org_band, axis=1, keepdims=True)
+        pred_band_variance = np.var(pred_band, axis=1, keepdims=True)
+        org_pred_band_variance = np.mean(
+            (org_band - org_band_mean) * (pred_band - pred_band_mean), axis=1, keepdims=True
+        )
+
+        numerator = 4 * org_pred_band_variance * org_band_mean * pred_band_mean
+        denominator = (org_band_variance + pred_band_variance) * (
+            org_band_mean**2 + pred_band_mean**2
+        )
+
+        q = np.nan_to_num(numerator / denominator)
+        q_all.extend(q.tolist())
+
+    if not q_all:
+        raise ValueError(
+            f"Window size ({window_size}) is too big for image with shape "
+            f"{org_img.shape[0:2]}, please use a smaller window size."
+        )
 
     return np.mean(q_all)
 
 
-def sam(org_img: np.ndarray, pred_img: np.ndarray, convert_to_degree=True):
+
+def sam(org_img: np.ndarray, pred_img: np.ndarray, convert_to_degree: bool = True) -> float:
     """
     Spectral Angle Mapper which defines the spectral similarity between two spectra
     """
-
     _assert_image_shapes_equal(org_img, pred_img, "SAM")
 
-    # Spectral angles are first computed for each pair of pixels
-    numerator = np.sum(np.multiply(pred_img, org_img), axis=2)
-    denominator = np.linalg.norm(org_img, axis=2) * np.linalg.norm(pred_img, axis=2)
+    numerator = np.sum(np.multiply(pred_img, org_img), axis=-1)
+    denominator = np.linalg.norm(org_img, axis=-1) * np.linalg.norm(pred_img, axis=-1)
     val = np.clip(numerator / denominator, -1, 1)
     sam_angles = np.arccos(val)
     if convert_to_degree:
-        sam_angles = sam_angles * 180.0 / np.pi
+        sam_angles = np.rad2deg(sam_angles)
 
-    # The original paper states that SAM values are expressed as radians, while e.g. Lanares
-    # et al. (2018) use degrees. We therefore made this configurable, with degree the default
-    return np.mean(np.nan_to_num(sam_angles))
+    return np.nan_to_num(np.mean(sam_angles))
 
 
 def sre(org_img: np.ndarray, pred_img: np.ndarray):
     """
-    signal to reconstruction error ratio
+    Signal to Reconstruction Error Ratio
     """
     _assert_image_shapes_equal(org_img, pred_img, "SRE")
 
     org_img = org_img.astype(np.float32)
+    
+    # if image is a gray image - add empty 3rd dimension for the .shape[2] to exist
+    if org_img.ndim == 2:
+        org_img = np.expand_dims(org_img, axis=-1)
 
     sre_final = []
     for i in range(org_img.shape[2]):
         numerator = np.square(np.mean(org_img[:, :, i]))
-        denominator = (np.linalg.norm(org_img[:, :, i] - pred_img[:, :, i])) /\
-                      (org_img.shape[0] * org_img.shape[1])
-        sre_final.append(numerator/denominator)
+        denominator = (np.linalg.norm(org_img[:, :, i] - pred_img[:, :, i])) / (
+            org_img.shape[0] * org_img.shape[1]
+        )
+        sre_final.append(numerator / denominator)
 
     return 10 * np.log10(np.mean(sre_final))
 
+
 metric_functions = {
     "fsim": fsim,
     "issm": issm,
     "psnr": psnr,
     "rmse": rmse,
     "sam": sam,
     "sre": sre,
```

### Comparing `image-similarity-measures-0.3.5/image_similarity_measures.egg-info/PKG-INFO` & `image_similarity_measures-0.3.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,33 @@
-Metadata-Version: 2.1
-Name: image-similarity-measures
-Version: 0.3.5
-Summary: Evaluation metrics to assess the similarity between two images.
-Home-page: https://github.com/up42/image-similarity-measures
-Author: UP42
-Author-email: support@up42.com
-License: MIT
-Description: # Image Similarity Measures
-        
-        Implementation of eight evaluation metrics to access the similarity between two images. The eight metrics are as follows:
-        
-         * <i><a href="https://en.wikipedia.org/wiki/Root-mean-square_deviation">Root mean square error (RMSE)</a></i>,
-         * <i><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio (PSNR)</a></i>,
-         * <i><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural Similarity Index (SSIM)</a></i>,
-         * <i><a href="https://www4.comp.polyu.edu.hk/~cslzhang/IQA/TIP_IQA_FSIM.pdf">Feature-based similarity index (FSIM)</a></i>,
-         * <i><a href="https://www.tandfonline.com/doi/full/10.1080/22797254.2019.1628617">Information theoretic-based Statistic Similarity Measure (ISSM)</a></i>,
-         * <i><a href="https://www.sciencedirect.com/science/article/abs/pii/S0924271618302636">Signal to reconstruction error ratio (SRE)</a></i>,
-         * <i><a href="https://ntrs.nasa.gov/citations/19940012238">Spectral angle mapper (SAM)</a></i>, and
-         * <i><a href="https://ece.uwaterloo.ca/~z70wang/publications/quality_2c.pdf">Universal image quality index (UIQ)</a></i>
-        
-        ## Instructions
-        
-        The following step-by-step instructions will guide you through installing this package and run evaluation using the command line tool.
-        
-        **Note:** Supported python versions are 3.6, 3.7, 3.8, and 3.9.
-        
-        ### Install package
-        ```bash
-        pip install image-similarity-measures
-        ```
-        
-        ### Usage
-        #### Parameters
-        ```
-          --org_img_path FILE   Path to original input image
-          --pred_img_path FILE  Path to predicted image
-          --metric METRIC       select an evaluation metric (fsim, issm, psnr, rmse,
-                                sam, sre, ssim, uiq, all) (can be repeated)
-        ```
-        
-        #### Evaluation
-        For doing the evaluation, you can easily run the following command:
-        
-        ```bash
-        image-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif
-        ```
-        The results are printed in machine-readable JSON, so you can redirect the output of the command into a file.
-        
-        **Note** that images that are used for evaluation should be **channel last**.
-        
-        #### Usage in python
-        ```bash
-        import image_similarity_measures
-        from image_similarity_measures.quality_metrics import rmse, psnr
-        ```
-        
-        ### Install package from source
-        
-        #### Clone the repository
-        
-        ```bash
-        git clone https://github.com/up42/image-similarity-measures.git
-        cd image-similarity-measures
-        ```
-        
-        Then navigate to the folder via `cd image-similarity-measures`.
-        
-        #### Installing the required libraries
-        
-        First create a new virtual environment called `similarity-measures`, for example by using
-        [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/):
-        
-        ```bash
-        mkvirtualenv --python=$(which python3.7) similarity-measures
-        ```
-        
-        Activate the new environment:
-        
-        ```bash
-        workon similarity-measures
-        ```
-        
-        Install the necessary Python libraries via:
-        
-        ```bash
-        bash setup.sh
-        ```
-        
-        ## Citation
-        Please use the following for citation purposes of this codebase:
-        
-        <strong>Müller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF MULTISPECTRAL
-        SATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann. Photogramm. Remote Sens.
-        Spatial Inf. Sci., V-1-2020, 33–40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.</strong>
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.10
-Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*-
+from setuptools import setup
+
+packages = \
+['image_similarity_measures']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['numpy>=1.24.2,<2.0.0',
+ 'opencv-python>=4.7.0.72,<5.0.0.0',
+ 'phasepack>=1.5,<2.0',
+ 'scikit-image>=0.20.0,<0.21.0']
+
+setup_kwargs = {
+    'name': 'image-similarity-measures',
+    'version': '0.3.6',
+    'description': 'Evaluation metrics to assess the similarity between two images.',
+    'long_description': '# Image Similarity Measures\n\nPython package and commandline tool to evaluate the similarity between two images with eight evaluation metrics:\n\n * <i><a href="https://en.wikipedia.org/wiki/Root-mean-square_deviation">Root mean square error (RMSE)</a></i>\n * <i><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio (PSNR)</a></i>\n * <i><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural Similarity Index (SSIM)</a></i>\n * <i><a href="https://www4.comp.polyu.edu.hk/~cslzhang/IQA/TIP_IQA_FSIM.pdf">Feature-based similarity index (FSIM)</a></i>\n * <i><a href="https://www.tandfonline.com/doi/full/10.1080/22797254.2019.1628617">Information theoretic-based Statistic Similarity Measure (ISSM)</a></i>\n * <i><a href="https://www.sciencedirect.com/science/article/abs/pii/S0924271618302636">Signal to reconstruction error ratio (SRE)</a></i>\n * <i><a href="https://ntrs.nasa.gov/citations/19940012238">Spectral angle mapper (SAM)</a></i>\n * <i><a href="https://ece.uwaterloo.ca/~z70wang/publications/quality_2c.pdf">Universal image quality index (UIQ)</a></i>\n\n## Installation\n\nSupports Python >=3.8.\n\n```bash\npip install image-similarity-measures\n```\n\n*Optional*: For faster evaluation of the FSIM metric, the `pyfftw` package is required, install via:\n\n```bash\npip install image-similarity-measures[speedups]\n```\n\n*Optional*: For reading TIFF images with `rasterio` instead of `OpenCV`, install:\n\n```bash\npip install image-similarity-measures[rasterio]\n```\n\n\n## Usage on commandline\n\nTo evaluate the similarity beteween two images, run on the commandline:\n\n```bash\nimage-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif\n```\n\n**Note** that images that are used for evaluation should be **channel last**. The results are printed in \nmachine-readable JSON, so you can redirect the output of the command into a file.\n\n#### Parameters\n```\n  --org_img_path FILE   Path to original input image\n  --pred_img_path FILE  Path to predicted image\n  --metric METRIC       select an evaluation metric (fsim, issm, psnr, rmse,\n                        sam, sre, ssim, uiq, all) (can be repeated)\n```\n\n## Usage in Python\n\n```bash\nfrom image_similarity_measures.evaluate import evaluation\n\nevaluation(org_img_path="example/lafayette_org.tif", \n           pred_img_path="example/lafayette_pred.tif", \n           metrics=["rmse", "psnr"])\n```\n\n```bash\nfrom image_similarity_measures.quality_metrics import rmse\n\nrmse(org_img=np.random.rand(3,2,1), pred_img=np.random.rand(3,2,1))\n```\n\n## Contribute\n\nContributions are welcome! Please see README-dev.md for instructions.\n\n\n## Citation\nPlease use the following for citation purposes of this codebase:\n\n<strong>Müller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF MULTISPECTRAL\nSATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann. Photogramm. Remote Sens.\nSpatial Inf. Sci., V-1-2020, 33–40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.</strong>\n',
+    'author': 'UP42',
+    'author_email': 'support@up42.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8',
+}
+
+
+setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: image-similarity-measures Version: 0.3.5 Summary:
-Evaluation metrics to assess the similarity between two images. Home-page:
-https://github.com/up42/image-similarity-measures Author: UP42 Author-email:
-support@up42.com License: MIT Description: # Image Similarity Measures
-Implementation of eight evaluation metrics to access the similarity between two
-images. The eight metrics are as follows: * Root_mean_square_error_(RMSE), *
-Peak_signal-to-noise_ratio_(PSNR), * Structural_Similarity_Index_(SSIM), *
-Feature-based_similarity_index_(FSIM), * Information_theoretic-based_Statistic
-Similarity_Measure_(ISSM), * Signal_to_reconstruction_error_ratio_(SRE), *
-Spectral_angle_mapper_(SAM), and * Universal_image_quality_index_(UIQ) ##
-Instructions The following step-by-step instructions will guide you through
-installing this package and run evaluation using the command line tool. **Note:
-** Supported python versions are 3.6, 3.7, 3.8, and 3.9. ### Install package
-```bash pip install image-similarity-measures ``` ### Usage #### Parameters ```
---org_img_path FILE Path to original input image --pred_img_path FILE Path to
-predicted image --metric METRIC select an evaluation metric (fsim, issm, psnr,
-rmse, sam, sre, ssim, uiq, all) (can be repeated) ``` #### Evaluation For doing
-the evaluation, you can easily run the following command: ```bash image-
-similarity-measures --org_img_path=a.tif --pred_img_path=b.tif ``` The results
-are printed in machine-readable JSON, so you can redirect the output of the
-command into a file. **Note** that images that are used for evaluation should
-be **channel last**. #### Usage in python ```bash import
-image_similarity_measures from image_similarity_measures.quality_metrics import
-rmse, psnr ``` ### Install package from source #### Clone the repository
-```bash git clone https://github.com/up42/image-similarity-measures.git cd
-image-similarity-measures ``` Then navigate to the folder via `cd image-
-similarity-measures`. #### Installing the required libraries First create a new
-virtual environment called `similarity-measures`, for example by using
-[virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/):
-```bash mkvirtualenv --python=$(which python3.7) similarity-measures ```
-Activate the new environment: ```bash workon similarity-measures ``` Install
-the necessary Python libraries via: ```bash bash setup.sh ``` ## Citation
-Please use the following for citation purposes of this codebase: MÃ¼ller, M.
-U., Ekhtiari, N., Almeida, R. M., and Rieke, C.: SUPER-RESOLUTION OF
-MULTISPECTRAL SATELLITE IMAGES USING CONVOLUTIONAL NEURAL NETWORKS, ISPRS Ann.
-Photogramm. Remote Sens. Spatial Inf. Sci., V-1-2020, 33â40, https://doi.org/
-10.5194/isprs-annals-V-1-2020-33-2020, 2020. Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Intended
-Audience :: Science/Research Classifier: Development Status :: 5 - Production/
-Stable Requires-Python: >=3.6, <3.10 Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*- from setuptools import setup packages = \
+['image_similarity_measures'] package_data = \ {'': ['*']} install_requires = \
+['numpy>=1.24.2,<2.0.0', 'opencv-python>=4.7.0.72,<5.0.0.0',
+'phasepack>=1.5,<2.0', 'scikit-image>=0.20.0,<0.21.0'] setup_kwargs = { 'name':
+'image-similarity-measures', 'version': '0.3.6', 'description': 'Evaluation
+metrics to assess the similarity between two images.', 'long_description': '#
+Image Similarity Measures\n\nPython package and commandline tool to evaluate
+the similarity between two images with eight evaluation metrics:\n\n * Root
+mean_square_error_(RMSE)\n * Peak_signal-to-noise_ratio_(PSNR)\n * Structural
+Similarity_Index_(SSIM)\n * Feature-based_similarity_index_(FSIM)\n *
+Information_theoretic-based_Statistic_Similarity_Measure_(ISSM)\n * Signal_to
+reconstruction_error_ratio_(SRE)\n * Spectral_angle_mapper_(SAM)\n * Universal
+image_quality_index_(UIQ)\n\n## Installation\n\nSupports Python
+>=3.8.\n\n```bash\npip install image-similarity-measures\n```\n\n*Optional*:
+For faster evaluation of the FSIM metric, the `pyfftw` package is required,
+install via:\n\n```bash\npip install image-similarity-measures
+[speedups]\n```\n\n*Optional*: For reading TIFF images with `rasterio` instead
+of `OpenCV`, install:\n\n```bash\npip install image-similarity-measures
+[rasterio]\n```\n\n\n## Usage on commandline\n\nTo evaluate the similarity
+beteween two images, run on the commandline:\n\n```bash\nimage-similarity-
+measures --org_img_path=a.tif --pred_img_path=b.tif\n```\n\n**Note** that
+images that are used for evaluation should be **channel last**. The results are
+printed in \nmachine-readable JSON, so you can redirect the output of the
+command into a file.\n\n#### Parameters\n```\n --org_img_path FILE Path to
+original input image\n --pred_img_path FILE Path to predicted image\n --metric
+METRIC select an evaluation metric (fsim, issm, psnr, rmse,\n sam, sre, ssim,
+uiq, all) (can be repeated)\n```\n\n## Usage in Python\n\n```bash\nfrom
+image_similarity_measures.evaluate import evaluation\n\nevaluation
+(org_img_path="example/lafayette_org.tif", \n pred_img_path="example/
+lafayette_pred.tif", \n metrics=["rmse", "psnr"])\n```\n\n```bash\nfrom
+image_similarity_measures.quality_metrics import rmse\n\nrmse
+(org_img=np.random.rand(3,2,1), pred_img=np.random.rand(3,2,1))\n```\n\n##
+Contribute\n\nContributions are welcome! Please see README-dev.md for
+instructions.\n\n\n## Citation\nPlease use the following for citation purposes
+of this codebase:\n\nMÃ¼ller, M. U., Ekhtiari, N., Almeida, R. M., and Rieke,
+C.: SUPER-RESOLUTION OF MULTISPECTRAL\nSATELLITE IMAGES USING CONVOLUTIONAL
+NEURAL NETWORKS, ISPRS Ann. Photogramm. Remote Sens.\nSpatial Inf. Sci., V-1-
+2020, 33â40, https://doi.org/10.5194/isprs-annals-V-1-2020-33-2020, 2020.\n',
+'author': 'UP42', 'author_email': 'support@up42.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.8', } setup(**setup_kwargs)
```

