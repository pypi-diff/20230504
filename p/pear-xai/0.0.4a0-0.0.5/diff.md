# Comparing `tmp/pear-xai-0.0.4a0.tar.gz` & `tmp/pear-xai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear-xai-0.0.4a0.tar", last modified: Thu May  4 13:17:12 2023, max compression
+gzip compressed data, was "pear-xai-0.0.5.tar", last modified: Thu May  4 13:44:02 2023, max compression
```

## Comparing `pear-xai-0.0.4a0.tar` & `pear-xai-0.0.5.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.454664 pear-xai-0.0.4a0/
--rw-r--r--   0 avi        (501) staff       (20)     1284 2023-03-02 15:14:45.000000 pear-xai-0.0.4a0/.gitignore
--rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.0.4a0/LICENSE
--rw-r--r--   0 avi        (501) staff       (20)     2397 2023-05-04 13:17:12.454492 pear-xai-0.0.4a0/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.0.4a0/README.md
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.409150 pear-xai-0.0.4a0/captum/
--rw-rw-r--   0 avi        (501) staff       (20)      281 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.410956 pear-xai-0.0.4a0/captum/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    20521 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/av.py
--rw-rw-r--   0 avi        (501) staff       (20)    23939 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)    35875 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/gradient.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.411268 pear-xai-0.0.4a0/captum/_utils/models/
--rw-rw-r--   0 avi        (501) staff       (20)      499 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/models/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.411678 pear-xai-0.0.4a0/captum/_utils/models/linear_model/
--rw-rw-r--   0 avi        (501) staff       (20)      447 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/models/linear_model/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    12218 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/models/linear_model/model.py
--rw-rw-r--   0 avi        (501) staff       (20)    11959 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/models/linear_model/train.py
--rw-rw-r--   0 avi        (501) staff       (20)     2039 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/models/model.py
--rw-rw-r--   0 avi        (501) staff       (20)     5137 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/progress.py
--rw-rw-r--   0 avi        (501) staff       (20)     7142 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/sample_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)     1176 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/_utils/typing.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.411814 pear-xai-0.0.4a0/captum/attr/
--rw-rw-r--   0 avi        (501) staff       (20)     4660 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.416263 pear-xai-0.0.4a0/captum/attr/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    44110 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    29716 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)    15634 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/feature_permutation.py
--rw-rw-r--   0 avi        (501) staff       (20)    18688 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)    14436 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/guided_backprop_deconvnet.py
--rw-rw-r--   0 avi        (501) staff       (20)    11370 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/guided_grad_cam.py
--rw-rw-r--   0 avi        (501) staff       (20)     6049 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/input_x_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)    17859 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    18691 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/kernel_shap.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.419179 pear-xai-0.0.4a0/captum/attr/_core/layer/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    11497 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/grad_cam.py
--rw-rw-r--   0 avi        (501) staff       (20)    15299 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/internal_influence.py
--rw-rw-r--   0 avi        (501) staff       (20)     6759 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_activation.py
--rw-rw-r--   0 avi        (501) staff       (20)    18776 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_conductance.py
--rw-rw-r--   0 avi        (501) staff       (20)    33565 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    15136 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)    22549 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)     9988 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_gradient_x_activation.py
--rw-rw-r--   0 avi        (501) staff       (20)    24591 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    13021 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/layer/layer_lrp.py
--rw-rw-r--   0 avi        (501) staff       (20)    59483 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/lime.py
--rw-rw-r--   0 avi        (501) staff       (20)    18349 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/lrp.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.420771 pear-xai-0.0.4a0/captum/attr/_core/neuron/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    20769 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_conductance.py
--rw-rw-r--   0 avi        (501) staff       (20)    25904 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    14914 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)     9480 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)    14226 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)    18506 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py
--rw-rw-r--   0 avi        (501) staff       (20)    14044 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    19799 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/noise_tunnel.py
--rw-rw-r--   0 avi        (501) staff       (20)    19499 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/occlusion.py
--rw-rw-r--   0 avi        (501) staff       (20)     6516 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/saliency.py
--rw-rw-r--   0 avi        (501) staff       (20)    39141 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_core/shapley_value.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.421148 pear-xai-0.0.4a0/captum/attr/_models/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_models/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    11379 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_models/base.py
--rw-rw-r--   0 avi        (501) staff       (20)    10280 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_models/pytext.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.423806 pear-xai-0.0.4a0/captum/attr/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     4781 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/approximation_methods.py
--rw-rw-r--   0 avi        (501) staff       (20)    21131 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/attribution.py
--rw-rw-r--   0 avi        (501) staff       (20)     8032 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/batching.py
--rw-rw-r--   0 avi        (501) staff       (20)     3307 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/class_summarizer.py
--rw-rw-r--   0 avi        (501) staff       (20)    13033 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/custom_modules.py
--rw-rw-r--   0 avi        (501) staff       (20)     2848 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/input_layer_wrapper.py
--rw-rw-r--   0 avi        (501) staff       (20)     6309 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/lrp_rules.py
--rw-rw-r--   0 avi        (501) staff       (20)     7452 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/stat.py
--rw-rw-r--   0 avi        (501) staff       (20)     8021 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/summarizer.py
--rw-rw-r--   0 avi        (501) staff       (20)    35661 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/attr/_utils/visualization.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.424045 pear-xai-0.0.4a0/captum/concept/
--rw-rw-r--   0 avi        (501) staff       (20)      283 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.424601 pear-xai-0.0.4a0/captum/concept/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     7169 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_core/cav.py
--rw-rw-r--   0 avi        (501) staff       (20)     3206 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_core/concept.py
--rw-rw-r--   0 avi        (501) staff       (20)    33484 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_core/tcav.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.425356 pear-xai-0.0.4a0/captum/concept/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     8960 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_utils/classifier.py
--rw-rw-r--   0 avi        (501) staff       (20)      726 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)     1919 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/concept/_utils/data_iterator.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.425646 pear-xai-0.0.4a0/captum/influence/
--rw-rw-r--   0 avi        (501) staff       (20)      512 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.426617 pear-xai-0.0.4a0/captum/influence/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     1768 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_core/influence.py
--rw-rw-r--   0 avi        (501) staff       (20)    14113 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_core/similarity_influence.py
--rw-rw-r--   0 avi        (501) staff       (20)    71547 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_core/tracincp.py
--rw-rw-r--   0 avi        (501) staff       (20)    85758 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_core/tracincp_fast_rand_proj.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.427338 pear-xai-0.0.4a0/captum/influence/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    23003 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)    10067 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/influence/_utils/nearest_neighbors.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.427673 pear-xai-0.0.4a0/captum/insights/
--rw-rw-r--   0 avi        (501) staff       (20)       84 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.427902 pear-xai-0.0.4a0/captum/insights/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/_utils/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.428964 pear-xai-0.0.4a0/captum/insights/attr_vis/
--rw-rw-r--   0 avi        (501) staff       (20)       78 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.429271 pear-xai-0.0.4a0/captum/insights/attr_vis/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)      303 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/_utils/transforms.py
--rw-rw-r--   0 avi        (501) staff       (20)    19467 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/app.py
--rw-rw-r--   0 avi        (501) staff       (20)     6733 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/attribution_calculation.py
--rw-rw-r--   0 avi        (501) staff       (20)     2308 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/config.py
--rw-rw-r--   0 avi        (501) staff       (20)     2584 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/example.py
--rw-rw-r--   0 avi        (501) staff       (20)    11895 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/features.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.429877 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/
--rw-rw-r--   0 avi        (501) staff       (20)      213 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/README.md
--rw-rw-r--   0 avi        (501) staff       (20)     1262 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/package.json
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.431159 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/public/
--rw-rw-r--   0 avi        (501) staff       (20)      316 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/public/index.html
--rw-rw-r--   0 avi        (501) staff       (20)      459 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/tsconfig.json
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.431320 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/widget/
--rw-rw-r--   0 avi        (501) staff       (20)     2236 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/widget/webpack.config.js
--rw-rw-r--   0 avi        (501) staff       (20)   480930 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/yarn.lock
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.431454 pear-xai-0.0.4a0/captum/insights/attr_vis/models/
--rw-rw-r--   0 avi        (501) staff       (20)   249703 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/models/cifar_torchvision.pt
--rw-rw-r--   0 avi        (501) staff       (20)     3331 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/server.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.432951 pear-xai-0.0.4a0/captum/insights/attr_vis/widget/
--rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/widget/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)      312 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/widget/_version.py
--rw-rw-r--   0 avi        (501) staff       (20)       77 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/widget/jupyter-captum-insights.json
--rw-rw-r--   0 avi        (501) staff       (20)     2057 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/attr_vis/widget/widget.py
--rw-rw-r--   0 avi        (501) staff       (20)      208 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/insights/example.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.433085 pear-xai-0.0.4a0/captum/log/
--rw-rw-r--   0 avi        (501) staff       (20)     1193 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/log/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.433225 pear-xai-0.0.4a0/captum/metrics/
--rw-rw-r--   0 avi        (501) staff       (20)      204 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.433664 pear-xai-0.0.4a0/captum/metrics/_core/
--rw-rw-r--   0 avi        (501) staff       (20)       23 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    26077 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/_core/infidelity.py
--rw-rw-r--   0 avi        (501) staff       (20)    13251 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/_core/sensitivity.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.433894 pear-xai-0.0.4a0/captum/metrics/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     3261 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/metrics/_utils/batching.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.434450 pear-xai-0.0.4a0/captum/module/
--rw-rw-r--   0 avi        (501) staff       (20)      266 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/module/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    10241 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/module/binary_concrete_stochastic_gates.py
--rw-rw-r--   0 avi        (501) staff       (20)     6914 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/module/gaussian_stochastic_gates.py
--rw-rw-r--   0 avi        (501) staff       (20)     8721 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/module/stochastic_gates_base.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.434596 pear-xai-0.0.4a0/captum/robust/
--rw-rw-r--   0 avi        (501) staff       (20)      372 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.435343 pear-xai-0.0.4a0/captum/robust/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     8725 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/fgsm.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.435754 pear-xai-0.0.4a0/captum/robust/_core/metrics/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/metrics/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    19665 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/metrics/attack_comparator.py
--rw-rw-r--   0 avi        (501) staff       (20)    18858 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/metrics/min_param_perturbation.py
--rw-rw-r--   0 avi        (501) staff       (20)     1435 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/perturbation.py
--rw-rw-r--   0 avi        (501) staff       (20)    10165 2023-02-27 18:57:42.000000 pear-xai-0.0.4a0/captum/robust/_core/pgd.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.437739 pear-xai-0.0.4a0/notebooks/
--rw-r--r--   0 avi        (501) staff       (20)   302629 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/notebooks/pear-training-experiment.ipynb
--rw-r--r--   0 avi        (501) staff       (20)    11180 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/notebooks/quickstart.ipynb
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.440067 pear-xai-0.0.4a0/pear/
--rw-r--r--   0 avi        (501) staff       (20)      757 2023-05-03 18:30:29.000000 pear-xai-0.0.4a0/pear/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.407934 pear-xai-0.0.4a0/pear/datasets/
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.441022 pear-xai-0.0.4a0/pear/datasets/bankmarketing/
--rw-r--r--   0 avi        (501) staff       (20)    76729 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/bankmarketing/bankmarketing-test.csv
--rw-r--r--   0 avi        (501) staff       (20)   230362 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/bankmarketing/bankmarketing-train.csv
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.444736 pear-xai-0.0.4a0/pear/datasets/californiahousing/
--rw-r--r--   0 avi        (501) staff       (20)   441167 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/californiahousing/californiahousing-test.csv
--rw-r--r--   0 avi        (501) staff       (20)  1325430 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/californiahousing/californiahousing-train.csv
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.450841 pear-xai-0.0.4a0/pear/datasets/electricity/
--rw-r--r--   0 avi        (501) staff       (20)   636732 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/electricity/electricity-test.csv
--rw-r--r--   0 avi        (501) staff       (20)  1909510 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/datasets/electricity/electricity-train.csv
--rw-r--r--   0 avi        (501) staff       (20)     2870 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/disagreement_loss.py
--rw-r--r--   0 avi        (501) staff       (20)    11118 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/disagreement_metrics.py
--rw-r--r--   0 avi        (501) staff       (20)     5571 2023-05-03 20:35:26.000000 pear-xai-0.0.4a0/pear/example.py
--rw-r--r--   0 avi        (501) staff       (20)     7939 2023-05-03 18:30:45.000000 pear-xai-0.0.4a0/pear/explainers.py
--rw-r--r--   0 avi        (501) staff       (20)     9559 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/models.py
--rw-r--r--   0 avi        (501) staff       (20)     4577 2023-03-02 01:56:26.000000 pear-xai-0.0.4a0/pear/tools.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:17:12.454304 pear-xai-0.0.4a0/pear_xai.egg-info/
--rw-r--r--   0 avi        (501) staff       (20)     2397 2023-05-04 13:17:12.000000 pear-xai-0.0.4a0/pear_xai.egg-info/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     5390 2023-05-04 13:17:12.000000 pear-xai-0.0.4a0/pear_xai.egg-info/SOURCES.txt
--rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-04 13:17:12.000000 pear-xai-0.0.4a0/pear_xai.egg-info/dependency_links.txt
--rw-r--r--   0 avi        (501) staff       (20)      204 2023-05-04 13:17:12.000000 pear-xai-0.0.4a0/pear_xai.egg-info/requires.txt
--rw-r--r--   0 avi        (501) staff       (20)       27 2023-05-04 13:17:12.000000 pear-xai-0.0.4a0/pear_xai.egg-info/top_level.txt
--rw-r--r--   0 avi        (501) staff       (20)     1460 2023-05-04 13:17:06.000000 pear-xai-0.0.4a0/pyproject.toml
--rw-r--r--   0 avi        (501) staff       (20)      188 2023-05-04 13:13:52.000000 pear-xai-0.0.4a0/requirements.txt
--rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-04 13:17:12.454705 pear-xai-0.0.4a0/setup.cfg
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.231462 pear-xai-0.0.5/
+-rw-r--r--   0 avi        (501) staff       (20)     1284 2023-03-02 15:14:45.000000 pear-xai-0.0.5/.gitignore
+-rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.0.5/LICENSE
+-rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 13:44:02.231289 pear-xai-0.0.5/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.0.5/README.md
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.180971 pear-xai-0.0.5/captum/
+-rw-rw-r--   0 avi        (501) staff       (20)      281 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.182792 pear-xai-0.0.5/captum/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20521 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/av.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23939 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35875 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/gradient.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.183093 pear-xai-0.0.5/captum/_utils/models/
+-rw-rw-r--   0 avi        (501) staff       (20)      499 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/models/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.183520 pear-xai-0.0.5/captum/_utils/models/linear_model/
+-rw-rw-r--   0 avi        (501) staff       (20)      447 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/models/linear_model/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    12218 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/models/linear_model/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11959 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/models/linear_model/train.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2039 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/models/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)     5137 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/progress.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7142 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/sample_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1176 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/_utils/typing.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.183668 pear-xai-0.0.5/captum/attr/
+-rw-rw-r--   0 avi        (501) staff       (20)     4660 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.188262 pear-xai-0.0.5/captum/attr/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    44110 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    29716 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15634 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/feature_permutation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18688 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14436 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11370 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/guided_grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6049 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/input_x_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    17859 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18691 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/kernel_shap.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.191117 pear-xai-0.0.5/captum/attr/_core/layer/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11497 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15299 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/internal_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6759 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18776 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33565 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15136 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    22549 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9988 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_gradient_x_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    24591 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13021 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/layer/layer_lrp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    59483 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/lime.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18349 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/lrp.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.192932 pear-xai-0.0.5/captum/attr/_core/neuron/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20769 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    25904 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14914 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9480 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14226 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18506 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14044 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/neuron/neuron_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19799 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/noise_tunnel.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19499 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/occlusion.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6516 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/saliency.py
+-rw-rw-r--   0 avi        (501) staff       (20)    39141 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_core/shapley_value.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.193344 pear-xai-0.0.5/captum/attr/_models/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_models/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11379 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_models/base.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10280 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_models/pytext.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.195552 pear-xai-0.0.5/captum/attr/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     4781 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/approximation_methods.py
+-rw-rw-r--   0 avi        (501) staff       (20)    21131 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/attribution.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8032 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/batching.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3307 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/class_summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13033 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/custom_modules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2848 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/input_layer_wrapper.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6309 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/lrp_rules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7452 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/stat.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8021 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35661 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/attr/_utils/visualization.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.195787 pear-xai-0.0.5/captum/concept/
+-rw-rw-r--   0 avi        (501) staff       (20)      283 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.196429 pear-xai-0.0.5/captum/concept/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7169 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_core/cav.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3206 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_core/concept.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33484 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_core/tcav.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.197356 pear-xai-0.0.5/captum/concept/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8960 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_utils/classifier.py
+-rw-rw-r--   0 avi        (501) staff       (20)      726 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1919 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/concept/_utils/data_iterator.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.197624 pear-xai-0.0.5/captum/influence/
+-rw-rw-r--   0 avi        (501) staff       (20)      512 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.198541 pear-xai-0.0.5/captum/influence/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1768 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_core/influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14113 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_core/similarity_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    71547 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_core/tracincp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    85758 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_core/tracincp_fast_rand_proj.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.199420 pear-xai-0.0.5/captum/influence/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23003 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10067 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/influence/_utils/nearest_neighbors.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.199857 pear-xai-0.0.5/captum/insights/
+-rw-rw-r--   0 avi        (501) staff       (20)       84 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.200146 pear-xai-0.0.5/captum/insights/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/_utils/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.201454 pear-xai-0.0.5/captum/insights/attr_vis/
+-rw-rw-r--   0 avi        (501) staff       (20)       78 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.201765 pear-xai-0.0.5/captum/insights/attr_vis/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      303 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/_utils/transforms.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19467 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/app.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6733 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/attribution_calculation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2308 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/config.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2584 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/example.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11895 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/features.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.202426 pear-xai-0.0.5/captum/insights/attr_vis/frontend/
+-rw-rw-r--   0 avi        (501) staff       (20)      213 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/README.md
+-rw-rw-r--   0 avi        (501) staff       (20)     1262 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/package.json
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.204279 pear-xai-0.0.5/captum/insights/attr_vis/frontend/public/
+-rw-rw-r--   0 avi        (501) staff       (20)      316 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/public/index.html
+-rw-rw-r--   0 avi        (501) staff       (20)      459 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/tsconfig.json
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.204446 pear-xai-0.0.5/captum/insights/attr_vis/frontend/widget/
+-rw-rw-r--   0 avi        (501) staff       (20)     2236 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/widget/webpack.config.js
+-rw-rw-r--   0 avi        (501) staff       (20)   480930 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/frontend/yarn.lock
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.204593 pear-xai-0.0.5/captum/insights/attr_vis/models/
+-rw-rw-r--   0 avi        (501) staff       (20)   249703 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/models/cifar_torchvision.pt
+-rw-rw-r--   0 avi        (501) staff       (20)     3331 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/server.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.207070 pear-xai-0.0.5/captum/insights/attr_vis/widget/
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/widget/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      312 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/widget/_version.py
+-rw-rw-r--   0 avi        (501) staff       (20)       77 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/widget/jupyter-captum-insights.json
+-rw-rw-r--   0 avi        (501) staff       (20)     2057 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/attr_vis/widget/widget.py
+-rw-rw-r--   0 avi        (501) staff       (20)      208 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/insights/example.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.207220 pear-xai-0.0.5/captum/log/
+-rw-rw-r--   0 avi        (501) staff       (20)     1193 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/log/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.207394 pear-xai-0.0.5/captum/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)      204 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.207923 pear-xai-0.0.5/captum/metrics/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)       23 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    26077 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/_core/infidelity.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13251 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/_core/sensitivity.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.208186 pear-xai-0.0.5/captum/metrics/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3261 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/metrics/_utils/batching.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.208826 pear-xai-0.0.5/captum/module/
+-rw-rw-r--   0 avi        (501) staff       (20)      266 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/module/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10241 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/module/binary_concrete_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6914 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/module/gaussian_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8721 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/module/stochastic_gates_base.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.208986 pear-xai-0.0.5/captum/robust/
+-rw-rw-r--   0 avi        (501) staff       (20)      372 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.209802 pear-xai-0.0.5/captum/robust/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8725 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/fgsm.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.210696 pear-xai-0.0.5/captum/robust/_core/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/metrics/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19665 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/metrics/attack_comparator.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18858 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/metrics/min_param_perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1435 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10165 2023-02-27 18:57:42.000000 pear-xai-0.0.5/captum/robust/_core/pgd.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.212724 pear-xai-0.0.5/notebooks/
+-rw-r--r--   0 avi        (501) staff       (20)   302629 2023-03-02 01:56:26.000000 pear-xai-0.0.5/notebooks/pear-training-experiment.ipynb
+-rw-r--r--   0 avi        (501) staff       (20)    11180 2023-03-02 01:56:26.000000 pear-xai-0.0.5/notebooks/quickstart.ipynb
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.214771 pear-xai-0.0.5/pear/
+-rw-r--r--   0 avi        (501) staff       (20)      757 2023-05-03 18:30:29.000000 pear-xai-0.0.5/pear/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.179654 pear-xai-0.0.5/pear/datasets/
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.215595 pear-xai-0.0.5/pear/datasets/bankmarketing/
+-rw-r--r--   0 avi        (501) staff       (20)    76729 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/bankmarketing/bankmarketing-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)   230362 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/bankmarketing/bankmarketing-train.csv
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.219925 pear-xai-0.0.5/pear/datasets/californiahousing/
+-rw-r--r--   0 avi        (501) staff       (20)   441167 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/californiahousing/californiahousing-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)  1325430 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/californiahousing/californiahousing-train.csv
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.226942 pear-xai-0.0.5/pear/datasets/electricity/
+-rw-r--r--   0 avi        (501) staff       (20)   636732 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/electricity/electricity-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)  1909510 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/datasets/electricity/electricity-train.csv
+-rw-r--r--   0 avi        (501) staff       (20)     2870 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/disagreement_loss.py
+-rw-r--r--   0 avi        (501) staff       (20)    11118 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/disagreement_metrics.py
+-rw-r--r--   0 avi        (501) staff       (20)     5571 2023-05-03 20:35:26.000000 pear-xai-0.0.5/pear/example.py
+-rw-r--r--   0 avi        (501) staff       (20)     7939 2023-05-03 18:30:45.000000 pear-xai-0.0.5/pear/explainers.py
+-rw-r--r--   0 avi        (501) staff       (20)     9559 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/models.py
+-rw-r--r--   0 avi        (501) staff       (20)     4577 2023-03-02 01:56:26.000000 pear-xai-0.0.5/pear/tools.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 13:44:02.231077 pear-xai-0.0.5/pear_xai.egg-info/
+-rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 13:44:02.000000 pear-xai-0.0.5/pear_xai.egg-info/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     5390 2023-05-04 13:44:02.000000 pear-xai-0.0.5/pear_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-04 13:44:02.000000 pear-xai-0.0.5/pear_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 avi        (501) staff       (20)      204 2023-05-04 13:44:02.000000 pear-xai-0.0.5/pear_xai.egg-info/requires.txt
+-rw-r--r--   0 avi        (501) staff       (20)       27 2023-05-04 13:44:02.000000 pear-xai-0.0.5/pear_xai.egg-info/top_level.txt
+-rw-r--r--   0 avi        (501) staff       (20)     1476 2023-05-04 13:43:52.000000 pear-xai-0.0.5/pyproject.toml
+-rw-r--r--   0 avi        (501) staff       (20)      188 2023-05-04 13:13:52.000000 pear-xai-0.0.5/requirements.txt
+-rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-04 13:44:02.231507 pear-xai-0.0.5/setup.cfg
```

### Comparing `pear-xai-0.0.4a0/.gitignore` & `pear-xai-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/LICENSE` & `pear-xai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/PKG-INFO` & `pear-xai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.0.4a0
+Version: 0.0.5
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Author-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 Maintainer-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 License: BSD-3-Clause
 Project-URL: homepage, https://arthur.ai
 Project-URL: repository, https://github.com/aks2203/pear-xai
 Project-URL: documentation, https://github.com/aks2203/pear-xai
```

### Comparing `pear-xai-0.0.4a0/README.md` & `pear-xai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/av.py` & `pear-xai-0.0.5/captum/_utils/av.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/common.py` & `pear-xai-0.0.5/captum/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/gradient.py` & `pear-xai-0.0.5/captum/_utils/gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/models/linear_model/model.py` & `pear-xai-0.0.5/captum/_utils/models/linear_model/model.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/models/linear_model/train.py` & `pear-xai-0.0.5/captum/_utils/models/linear_model/train.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/models/model.py` & `pear-xai-0.0.5/captum/_utils/models/model.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/progress.py` & `pear-xai-0.0.5/captum/_utils/progress.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/sample_gradient.py` & `pear-xai-0.0.5/captum/_utils/sample_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/_utils/typing.py` & `pear-xai-0.0.5/captum/_utils/typing.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/__init__.py` & `pear-xai-0.0.5/captum/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/deep_lift.py` & `pear-xai-0.0.5/captum/attr/_core/deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/feature_ablation.py` & `pear-xai-0.0.5/captum/attr/_core/feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/feature_permutation.py` & `pear-xai-0.0.5/captum/attr/_core/feature_permutation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/gradient_shap.py` & `pear-xai-0.0.5/captum/attr/_core/gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/guided_backprop_deconvnet.py` & `pear-xai-0.0.5/captum/attr/_core/guided_backprop_deconvnet.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/guided_grad_cam.py` & `pear-xai-0.0.5/captum/attr/_core/guided_grad_cam.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/input_x_gradient.py` & `pear-xai-0.0.5/captum/attr/_core/input_x_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/integrated_gradients.py` & `pear-xai-0.0.5/captum/attr/_core/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/kernel_shap.py` & `pear-xai-0.0.5/captum/attr/_core/kernel_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/grad_cam.py` & `pear-xai-0.0.5/captum/attr/_core/layer/grad_cam.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/internal_influence.py` & `pear-xai-0.0.5/captum/attr/_core/layer/internal_influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_activation.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_activation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_conductance.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_conductance.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_deep_lift.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_feature_ablation.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_gradient_shap.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_gradient_x_activation.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_gradient_x_activation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_integrated_gradients.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/layer/layer_lrp.py` & `pear-xai-0.0.5/captum/attr/_core/layer/layer_lrp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/lime.py` & `pear-xai-0.0.5/captum/attr/_core/lime.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/lrp.py` & `pear-xai-0.0.5/captum/attr/_core/lrp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_conductance.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_conductance.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_deep_lift.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_feature_ablation.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_gradient.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_gradient_shap.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/neuron/neuron_integrated_gradients.py` & `pear-xai-0.0.5/captum/attr/_core/neuron/neuron_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/noise_tunnel.py` & `pear-xai-0.0.5/captum/attr/_core/noise_tunnel.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/occlusion.py` & `pear-xai-0.0.5/captum/attr/_core/occlusion.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/saliency.py` & `pear-xai-0.0.5/captum/attr/_core/saliency.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_core/shapley_value.py` & `pear-xai-0.0.5/captum/attr/_core/shapley_value.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_models/base.py` & `pear-xai-0.0.5/captum/attr/_models/base.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_models/pytext.py` & `pear-xai-0.0.5/captum/attr/_models/pytext.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/approximation_methods.py` & `pear-xai-0.0.5/captum/attr/_utils/approximation_methods.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/attribution.py` & `pear-xai-0.0.5/captum/attr/_utils/attribution.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/batching.py` & `pear-xai-0.0.5/captum/attr/_utils/batching.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/class_summarizer.py` & `pear-xai-0.0.5/captum/attr/_utils/class_summarizer.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/common.py` & `pear-xai-0.0.5/captum/attr/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/input_layer_wrapper.py` & `pear-xai-0.0.5/captum/attr/_utils/input_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/lrp_rules.py` & `pear-xai-0.0.5/captum/attr/_utils/lrp_rules.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/stat.py` & `pear-xai-0.0.5/captum/attr/_utils/stat.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/summarizer.py` & `pear-xai-0.0.5/captum/attr/_utils/summarizer.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/attr/_utils/visualization.py` & `pear-xai-0.0.5/captum/attr/_utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_core/cav.py` & `pear-xai-0.0.5/captum/concept/_core/cav.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_core/concept.py` & `pear-xai-0.0.5/captum/concept/_core/concept.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_core/tcav.py` & `pear-xai-0.0.5/captum/concept/_core/tcav.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_utils/classifier.py` & `pear-xai-0.0.5/captum/concept/_utils/classifier.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_utils/common.py` & `pear-xai-0.0.5/captum/concept/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/concept/_utils/data_iterator.py` & `pear-xai-0.0.5/captum/concept/_utils/data_iterator.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/__init__.py` & `pear-xai-0.0.5/captum/influence/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_core/influence.py` & `pear-xai-0.0.5/captum/influence/_core/influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_core/similarity_influence.py` & `pear-xai-0.0.5/captum/influence/_core/similarity_influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_core/tracincp.py` & `pear-xai-0.0.5/captum/influence/_core/tracincp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_core/tracincp_fast_rand_proj.py` & `pear-xai-0.0.5/captum/influence/_core/tracincp_fast_rand_proj.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_utils/common.py` & `pear-xai-0.0.5/captum/influence/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/influence/_utils/nearest_neighbors.py` & `pear-xai-0.0.5/captum/influence/_utils/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/app.py` & `pear-xai-0.0.5/captum/insights/attr_vis/app.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/attribution_calculation.py` & `pear-xai-0.0.5/captum/insights/attr_vis/attribution_calculation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/config.py` & `pear-xai-0.0.5/captum/insights/attr_vis/config.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/example.py` & `pear-xai-0.0.5/captum/insights/attr_vis/example.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/features.py` & `pear-xai-0.0.5/captum/insights/attr_vis/features.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/package.json` & `pear-xai-0.0.5/captum/insights/attr_vis/frontend/package.json`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/widget/webpack.config.js` & `pear-xai-0.0.5/captum/insights/attr_vis/frontend/widget/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/frontend/yarn.lock` & `pear-xai-0.0.5/captum/insights/attr_vis/frontend/yarn.lock`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/models/cifar_torchvision.pt` & `pear-xai-0.0.5/captum/insights/attr_vis/models/cifar_torchvision.pt`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/server.py` & `pear-xai-0.0.5/captum/insights/attr_vis/server.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/insights/attr_vis/widget/widget.py` & `pear-xai-0.0.5/captum/insights/attr_vis/widget/widget.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/log/__init__.py` & `pear-xai-0.0.5/captum/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/metrics/_core/infidelity.py` & `pear-xai-0.0.5/captum/metrics/_core/infidelity.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/metrics/_core/sensitivity.py` & `pear-xai-0.0.5/captum/metrics/_core/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/metrics/_utils/batching.py` & `pear-xai-0.0.5/captum/metrics/_utils/batching.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/module/binary_concrete_stochastic_gates.py` & `pear-xai-0.0.5/captum/module/binary_concrete_stochastic_gates.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/module/gaussian_stochastic_gates.py` & `pear-xai-0.0.5/captum/module/gaussian_stochastic_gates.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/module/stochastic_gates_base.py` & `pear-xai-0.0.5/captum/module/stochastic_gates_base.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/robust/_core/fgsm.py` & `pear-xai-0.0.5/captum/robust/_core/fgsm.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/robust/_core/metrics/attack_comparator.py` & `pear-xai-0.0.5/captum/robust/_core/metrics/attack_comparator.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/robust/_core/metrics/min_param_perturbation.py` & `pear-xai-0.0.5/captum/robust/_core/metrics/min_param_perturbation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/robust/_core/perturbation.py` & `pear-xai-0.0.5/captum/robust/_core/perturbation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/captum/robust/_core/pgd.py` & `pear-xai-0.0.5/captum/robust/_core/pgd.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/notebooks/pear-training-experiment.ipynb` & `pear-xai-0.0.5/notebooks/pear-training-experiment.ipynb`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/notebooks/quickstart.ipynb` & `pear-xai-0.0.5/notebooks/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/__init__.py` & `pear-xai-0.0.5/pear/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/bankmarketing/bankmarketing-test.csv` & `pear-xai-0.0.5/pear/datasets/bankmarketing/bankmarketing-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/bankmarketing/bankmarketing-train.csv` & `pear-xai-0.0.5/pear/datasets/bankmarketing/bankmarketing-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/californiahousing/californiahousing-test.csv` & `pear-xai-0.0.5/pear/datasets/californiahousing/californiahousing-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/californiahousing/californiahousing-train.csv` & `pear-xai-0.0.5/pear/datasets/californiahousing/californiahousing-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/electricity/electricity-test.csv` & `pear-xai-0.0.5/pear/datasets/electricity/electricity-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/datasets/electricity/electricity-train.csv` & `pear-xai-0.0.5/pear/datasets/electricity/electricity-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/disagreement_loss.py` & `pear-xai-0.0.5/pear/disagreement_loss.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/disagreement_metrics.py` & `pear-xai-0.0.5/pear/disagreement_metrics.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/example.py` & `pear-xai-0.0.5/pear/example.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/explainers.py` & `pear-xai-0.0.5/pear/explainers.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/models.py` & `pear-xai-0.0.5/pear/models.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear/tools.py` & `pear-xai-0.0.5/pear/tools.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pear_xai.egg-info/PKG-INFO` & `pear-xai-0.0.5/pear_xai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.0.4a0
+Version: 0.0.5
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Author-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 Maintainer-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 License: BSD-3-Clause
 Project-URL: homepage, https://arthur.ai
 Project-URL: repository, https://github.com/aks2203/pear-xai
 Project-URL: documentation, https://github.com/aks2203/pear-xai
```

### Comparing `pear-xai-0.0.4a0/pear_xai.egg-info/SOURCES.txt` & `pear-xai-0.0.5/pear_xai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.4a0/pyproject.toml` & `pear-xai-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "setuptools-scm", "torch==1.11.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pear-xai"
 description = "PEAR: Post-hoc Explainer Agreement Regularization"
 readme = "README.md"
 authors = [ {name="Avi Schwarzschild", email="avi1@umd.edu"}, {name="Max Cembalest", email="max.cembalest@arthur.ai"},
@@ -23,15 +23,15 @@
                 "seaborn==0.12.2",
                 "shap==0.41.0",
                 "sklearn==0.0",
                 "tabulate==0.8.10",
                 "torchvision==0.12.0",
                 "torchsort==0.1.9",
                 "tqdm==4.64.0"]
-version = "0.0.4a"
+version = "0.0.5"
 
 [tools.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages]
 find = {}
```

