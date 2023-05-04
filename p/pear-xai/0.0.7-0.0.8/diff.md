# Comparing `tmp/pear-xai-0.0.7.tar.gz` & `tmp/pear-xai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear-xai-0.0.7.tar", last modified: Thu May  4 15:20:05 2023, max compression
+gzip compressed data, was "pear-xai-0.0.8.tar", last modified: Thu May  4 15:49:38 2023, max compression
```

## Comparing `pear-xai-0.0.7.tar` & `pear-xai-0.0.8.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.747906 pear-xai-0.0.7/
--rw-r--r--   0 avi        (501) staff       (20)     1284 2023-03-02 15:14:45.000000 pear-xai-0.0.7/.gitignore
--rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.0.7/LICENSE
--rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 15:20:05.747663 pear-xai-0.0.7/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.0.7/README.md
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.699417 pear-xai-0.0.7/captum/
--rw-rw-r--   0 avi        (501) staff       (20)      281 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.701649 pear-xai-0.0.7/captum/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    20521 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/av.py
--rw-rw-r--   0 avi        (501) staff       (20)    23939 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)    35875 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/gradient.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.702094 pear-xai-0.0.7/captum/_utils/models/
--rw-rw-r--   0 avi        (501) staff       (20)      499 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/models/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.702726 pear-xai-0.0.7/captum/_utils/models/linear_model/
--rw-rw-r--   0 avi        (501) staff       (20)      447 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/models/linear_model/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    12218 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/models/linear_model/model.py
--rw-rw-r--   0 avi        (501) staff       (20)    11959 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/models/linear_model/train.py
--rw-rw-r--   0 avi        (501) staff       (20)     2039 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/models/model.py
--rw-rw-r--   0 avi        (501) staff       (20)     5137 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/progress.py
--rw-rw-r--   0 avi        (501) staff       (20)     7142 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/sample_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)     1176 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/_utils/typing.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.702957 pear-xai-0.0.7/captum/attr/
--rw-rw-r--   0 avi        (501) staff       (20)     4660 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.707759 pear-xai-0.0.7/captum/attr/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    44110 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    29716 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)    15634 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/feature_permutation.py
--rw-rw-r--   0 avi        (501) staff       (20)    18688 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)    14436 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/guided_backprop_deconvnet.py
--rw-rw-r--   0 avi        (501) staff       (20)    11370 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/guided_grad_cam.py
--rw-rw-r--   0 avi        (501) staff       (20)     6049 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/input_x_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)    17859 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    18691 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/kernel_shap.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.710560 pear-xai-0.0.7/captum/attr/_core/layer/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    11497 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/grad_cam.py
--rw-rw-r--   0 avi        (501) staff       (20)    15299 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/internal_influence.py
--rw-rw-r--   0 avi        (501) staff       (20)     6759 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_activation.py
--rw-rw-r--   0 avi        (501) staff       (20)    18776 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_conductance.py
--rw-rw-r--   0 avi        (501) staff       (20)    33565 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    15136 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)    22549 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)     9988 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_gradient_x_activation.py
--rw-rw-r--   0 avi        (501) staff       (20)    24591 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    13021 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/layer/layer_lrp.py
--rw-rw-r--   0 avi        (501) staff       (20)    59483 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/lime.py
--rw-rw-r--   0 avi        (501) staff       (20)    18349 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/lrp.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.712176 pear-xai-0.0.7/captum/attr/_core/neuron/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    20769 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_conductance.py
--rw-rw-r--   0 avi        (501) staff       (20)    25904 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_deep_lift.py
--rw-rw-r--   0 avi        (501) staff       (20)    14914 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_feature_ablation.py
--rw-rw-r--   0 avi        (501) staff       (20)     9480 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_gradient.py
--rw-rw-r--   0 avi        (501) staff       (20)    14226 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_gradient_shap.py
--rw-rw-r--   0 avi        (501) staff       (20)    18506 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py
--rw-rw-r--   0 avi        (501) staff       (20)    14044 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/neuron/neuron_integrated_gradients.py
--rw-rw-r--   0 avi        (501) staff       (20)    19799 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/noise_tunnel.py
--rw-rw-r--   0 avi        (501) staff       (20)    19499 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/occlusion.py
--rw-rw-r--   0 avi        (501) staff       (20)     6516 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/saliency.py
--rw-rw-r--   0 avi        (501) staff       (20)    39141 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_core/shapley_value.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.712546 pear-xai-0.0.7/captum/attr/_models/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_models/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    11379 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_models/base.py
--rw-rw-r--   0 avi        (501) staff       (20)    10280 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_models/pytext.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.714502 pear-xai-0.0.7/captum/attr/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     4781 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/approximation_methods.py
--rw-rw-r--   0 avi        (501) staff       (20)    21131 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/attribution.py
--rw-rw-r--   0 avi        (501) staff       (20)     8032 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/batching.py
--rw-rw-r--   0 avi        (501) staff       (20)     3307 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/class_summarizer.py
--rw-rw-r--   0 avi        (501) staff       (20)    13033 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/custom_modules.py
--rw-rw-r--   0 avi        (501) staff       (20)     2848 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/input_layer_wrapper.py
--rw-rw-r--   0 avi        (501) staff       (20)     6309 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/lrp_rules.py
--rw-rw-r--   0 avi        (501) staff       (20)     7452 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/stat.py
--rw-rw-r--   0 avi        (501) staff       (20)     8021 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/summarizer.py
--rw-rw-r--   0 avi        (501) staff       (20)    35661 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/attr/_utils/visualization.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.714699 pear-xai-0.0.7/captum/concept/
--rw-rw-r--   0 avi        (501) staff       (20)      283 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.715378 pear-xai-0.0.7/captum/concept/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     7169 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_core/cav.py
--rw-rw-r--   0 avi        (501) staff       (20)     3206 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_core/concept.py
--rw-rw-r--   0 avi        (501) staff       (20)    33484 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_core/tcav.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.716452 pear-xai-0.0.7/captum/concept/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     8960 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_utils/classifier.py
--rw-rw-r--   0 avi        (501) staff       (20)      726 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)     1919 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/concept/_utils/data_iterator.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.716736 pear-xai-0.0.7/captum/influence/
--rw-rw-r--   0 avi        (501) staff       (20)      512 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.717732 pear-xai-0.0.7/captum/influence/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     1768 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_core/influence.py
--rw-rw-r--   0 avi        (501) staff       (20)    14113 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_core/similarity_influence.py
--rw-rw-r--   0 avi        (501) staff       (20)    71547 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_core/tracincp.py
--rw-rw-r--   0 avi        (501) staff       (20)    85758 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_core/tracincp_fast_rand_proj.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.718501 pear-xai-0.0.7/captum/influence/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    23003 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_utils/common.py
--rw-rw-r--   0 avi        (501) staff       (20)    10067 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/influence/_utils/nearest_neighbors.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.718839 pear-xai-0.0.7/captum/insights/
--rw-rw-r--   0 avi        (501) staff       (20)       84 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.719154 pear-xai-0.0.7/captum/insights/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/_utils/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.720592 pear-xai-0.0.7/captum/insights/attr_vis/
--rw-rw-r--   0 avi        (501) staff       (20)       78 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.720927 pear-xai-0.0.7/captum/insights/attr_vis/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)      303 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/_utils/transforms.py
--rw-rw-r--   0 avi        (501) staff       (20)    19467 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/app.py
--rw-rw-r--   0 avi        (501) staff       (20)     6733 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/attribution_calculation.py
--rw-rw-r--   0 avi        (501) staff       (20)     2308 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/config.py
--rw-rw-r--   0 avi        (501) staff       (20)     2584 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/example.py
--rw-rw-r--   0 avi        (501) staff       (20)    11895 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/features.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.721699 pear-xai-0.0.7/captum/insights/attr_vis/frontend/
--rw-rw-r--   0 avi        (501) staff       (20)      213 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/README.md
--rw-rw-r--   0 avi        (501) staff       (20)     1262 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/package.json
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.723097 pear-xai-0.0.7/captum/insights/attr_vis/frontend/public/
--rw-rw-r--   0 avi        (501) staff       (20)      316 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/public/index.html
--rw-rw-r--   0 avi        (501) staff       (20)      459 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/tsconfig.json
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.723303 pear-xai-0.0.7/captum/insights/attr_vis/frontend/widget/
--rw-rw-r--   0 avi        (501) staff       (20)     2236 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/widget/webpack.config.js
--rw-rw-r--   0 avi        (501) staff       (20)   480930 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/frontend/yarn.lock
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.723458 pear-xai-0.0.7/captum/insights/attr_vis/models/
--rw-rw-r--   0 avi        (501) staff       (20)   249703 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/models/cifar_torchvision.pt
--rw-rw-r--   0 avi        (501) staff       (20)     3331 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/server.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.725715 pear-xai-0.0.7/captum/insights/attr_vis/widget/
--rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/widget/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)      312 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/widget/_version.py
--rw-rw-r--   0 avi        (501) staff       (20)       77 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/widget/jupyter-captum-insights.json
--rw-rw-r--   0 avi        (501) staff       (20)     2057 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/attr_vis/widget/widget.py
--rw-rw-r--   0 avi        (501) staff       (20)      208 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/insights/example.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.725946 pear-xai-0.0.7/captum/log/
--rw-rw-r--   0 avi        (501) staff       (20)     1193 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/log/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.726157 pear-xai-0.0.7/captum/metrics/
--rw-rw-r--   0 avi        (501) staff       (20)      204 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.726740 pear-xai-0.0.7/captum/metrics/_core/
--rw-rw-r--   0 avi        (501) staff       (20)       23 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    26077 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/_core/infidelity.py
--rw-rw-r--   0 avi        (501) staff       (20)    13251 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/_core/sensitivity.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.727000 pear-xai-0.0.7/captum/metrics/_utils/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/_utils/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     3261 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/metrics/_utils/batching.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.727621 pear-xai-0.0.7/captum/module/
--rw-rw-r--   0 avi        (501) staff       (20)      266 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/module/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    10241 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/module/binary_concrete_stochastic_gates.py
--rw-rw-r--   0 avi        (501) staff       (20)     6914 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/module/gaussian_stochastic_gates.py
--rw-rw-r--   0 avi        (501) staff       (20)     8721 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/module/stochastic_gates_base.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.727765 pear-xai-0.0.7/captum/robust/
--rw-rw-r--   0 avi        (501) staff       (20)      372 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.728568 pear-xai-0.0.7/captum/robust/_core/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     8725 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/fgsm.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.729138 pear-xai-0.0.7/captum/robust/_core/metrics/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/metrics/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)    19665 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/metrics/attack_comparator.py
--rw-rw-r--   0 avi        (501) staff       (20)    18858 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/metrics/min_param_perturbation.py
--rw-rw-r--   0 avi        (501) staff       (20)     1435 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/perturbation.py
--rw-rw-r--   0 avi        (501) staff       (20)    10165 2023-02-27 18:57:42.000000 pear-xai-0.0.7/captum/robust/_core/pgd.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.730208 pear-xai-0.0.7/fast_soft_sort/
--rw-rw-r--   0 avi        (501) staff       (20)        0 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     3724 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/jax_ops.py
--rw-rw-r--   0 avi        (501) staff       (20)    12504 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/numpy_ops.py
--rw-rw-r--   0 avi        (501) staff       (20)     3680 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/pytorch_ops.py
--rw-rw-r--   0 avi        (501) staff       (20)     3607 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/tf_ops.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.730647 pear-xai-0.0.7/fast_soft_sort/third_party/
--rw-rw-r--   0 avi        (501) staff       (20)     1570 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/third_party/LICENSE
--rw-rw-r--   0 avi        (501) staff       (20)        0 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/third_party/__init__.py
--rw-rw-r--   0 avi        (501) staff       (20)     5576 2020-07-28 17:20:24.000000 pear-xai-0.0.7/fast_soft_sort/third_party/isotonic.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.731115 pear-xai-0.0.7/notebooks/
--rw-r--r--   0 avi        (501) staff       (20)    23795 2023-05-04 15:18:23.000000 pear-xai-0.0.7/notebooks/pear-training-experiment.ipynb
--rw-r--r--   0 avi        (501) staff       (20)    11180 2023-03-02 01:56:26.000000 pear-xai-0.0.7/notebooks/quickstart.ipynb
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.732734 pear-xai-0.0.7/pear/
--rw-r--r--   0 avi        (501) staff       (20)      757 2023-05-03 18:30:29.000000 pear-xai-0.0.7/pear/__init__.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.697762 pear-xai-0.0.7/pear/datasets/
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.733666 pear-xai-0.0.7/pear/datasets/bankmarketing/
--rw-r--r--   0 avi        (501) staff       (20)    76729 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/bankmarketing/bankmarketing-test.csv
--rw-r--r--   0 avi        (501) staff       (20)   230362 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/bankmarketing/bankmarketing-train.csv
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.736580 pear-xai-0.0.7/pear/datasets/californiahousing/
--rw-r--r--   0 avi        (501) staff       (20)   441167 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/californiahousing/californiahousing-test.csv
--rw-r--r--   0 avi        (501) staff       (20)  1325430 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/californiahousing/californiahousing-train.csv
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.743817 pear-xai-0.0.7/pear/datasets/electricity/
--rw-r--r--   0 avi        (501) staff       (20)   636732 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/electricity/electricity-test.csv
--rw-r--r--   0 avi        (501) staff       (20)  1909510 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/datasets/electricity/electricity-train.csv
--rw-r--r--   0 avi        (501) staff       (20)     2901 2023-05-04 15:16:13.000000 pear-xai-0.0.7/pear/disagreement_loss.py
--rw-r--r--   0 avi        (501) staff       (20)    11118 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/disagreement_metrics.py
--rw-r--r--   0 avi        (501) staff       (20)     5571 2023-05-03 20:35:26.000000 pear-xai-0.0.7/pear/example.py
--rw-r--r--   0 avi        (501) staff       (20)     7939 2023-05-03 18:30:45.000000 pear-xai-0.0.7/pear/explainers.py
--rw-r--r--   0 avi        (501) staff       (20)     9559 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/models.py
--rw-r--r--   0 avi        (501) staff       (20)     4577 2023-03-02 01:56:26.000000 pear-xai-0.0.7/pear/tools.py
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:20:05.747418 pear-xai-0.0.7/pear_xai.egg-info/
--rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 15:20:05.000000 pear-xai-0.0.7/pear_xai.egg-info/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     5639 2023-05-04 15:20:05.000000 pear-xai-0.0.7/pear_xai.egg-info/SOURCES.txt
--rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-04 15:20:05.000000 pear-xai-0.0.7/pear_xai.egg-info/dependency_links.txt
--rw-r--r--   0 avi        (501) staff       (20)      187 2023-05-04 15:20:05.000000 pear-xai-0.0.7/pear_xai.egg-info/requires.txt
--rw-r--r--   0 avi        (501) staff       (20)       42 2023-05-04 15:20:05.000000 pear-xai-0.0.7/pear_xai.egg-info/top_level.txt
--rw-r--r--   0 avi        (501) staff       (20)     1457 2023-05-04 15:19:52.000000 pear-xai-0.0.7/pyproject.toml
--rw-r--r--   0 avi        (501) staff       (20)      171 2023-05-04 15:14:19.000000 pear-xai-0.0.7/requirements.txt
--rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-04 15:20:05.747950 pear-xai-0.0.7/setup.cfg
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.183510 pear-xai-0.0.8/
+-rw-r--r--   0 avi        (501) staff       (20)     1284 2023-03-02 15:14:45.000000 pear-xai-0.0.8/.gitignore
+-rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.0.8/LICENSE
+-rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 15:49:38.183335 pear-xai-0.0.8/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.0.8/README.md
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.139538 pear-xai-0.0.8/captum/
+-rw-rw-r--   0 avi        (501) staff       (20)      281 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.141712 pear-xai-0.0.8/captum/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20521 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/av.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23939 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35875 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/gradient.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.142061 pear-xai-0.0.8/captum/_utils/models/
+-rw-rw-r--   0 avi        (501) staff       (20)      499 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/models/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.142586 pear-xai-0.0.8/captum/_utils/models/linear_model/
+-rw-rw-r--   0 avi        (501) staff       (20)      447 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/models/linear_model/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    12218 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/models/linear_model/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11959 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/models/linear_model/train.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2039 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/models/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)     5137 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/progress.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7142 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/sample_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1176 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/_utils/typing.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.142742 pear-xai-0.0.8/captum/attr/
+-rw-rw-r--   0 avi        (501) staff       (20)     4660 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.147655 pear-xai-0.0.8/captum/attr/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    44110 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    29716 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15634 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/feature_permutation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18688 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14436 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11370 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/guided_grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6049 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/input_x_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    17859 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18691 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/kernel_shap.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.150299 pear-xai-0.0.8/captum/attr/_core/layer/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11497 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15299 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/internal_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6759 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18776 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33565 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15136 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    22549 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9988 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_gradient_x_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    24591 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13021 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/layer/layer_lrp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    59483 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/lime.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18349 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/lrp.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.151995 pear-xai-0.0.8/captum/attr/_core/neuron/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20769 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    25904 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14914 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9480 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14226 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18506 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14044 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/neuron/neuron_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19799 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/noise_tunnel.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19499 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/occlusion.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6516 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/saliency.py
+-rw-rw-r--   0 avi        (501) staff       (20)    39141 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_core/shapley_value.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.152383 pear-xai-0.0.8/captum/attr/_models/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_models/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11379 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_models/base.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10280 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_models/pytext.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.154397 pear-xai-0.0.8/captum/attr/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     4781 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/approximation_methods.py
+-rw-rw-r--   0 avi        (501) staff       (20)    21131 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/attribution.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8032 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/batching.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3307 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/class_summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13033 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/custom_modules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2848 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/input_layer_wrapper.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6309 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/lrp_rules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7452 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/stat.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8021 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35661 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/attr/_utils/visualization.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.154702 pear-xai-0.0.8/captum/concept/
+-rw-rw-r--   0 avi        (501) staff       (20)      283 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.155352 pear-xai-0.0.8/captum/concept/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7169 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_core/cav.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3206 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_core/concept.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33484 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_core/tcav.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.156091 pear-xai-0.0.8/captum/concept/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8960 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_utils/classifier.py
+-rw-rw-r--   0 avi        (501) staff       (20)      726 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1919 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/concept/_utils/data_iterator.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.156347 pear-xai-0.0.8/captum/influence/
+-rw-rw-r--   0 avi        (501) staff       (20)      512 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.157514 pear-xai-0.0.8/captum/influence/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1768 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_core/influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14113 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_core/similarity_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    71547 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_core/tracincp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    85758 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_core/tracincp_fast_rand_proj.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.158361 pear-xai-0.0.8/captum/influence/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23003 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10067 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/influence/_utils/nearest_neighbors.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.158653 pear-xai-0.0.8/captum/insights/
+-rw-rw-r--   0 avi        (501) staff       (20)       84 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.158871 pear-xai-0.0.8/captum/insights/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/_utils/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.159969 pear-xai-0.0.8/captum/insights/attr_vis/
+-rw-rw-r--   0 avi        (501) staff       (20)       78 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.160290 pear-xai-0.0.8/captum/insights/attr_vis/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      303 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/_utils/transforms.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19467 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/app.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6733 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/attribution_calculation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2308 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/config.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2584 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/example.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11895 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/features.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.160881 pear-xai-0.0.8/captum/insights/attr_vis/frontend/
+-rw-rw-r--   0 avi        (501) staff       (20)      213 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/README.md
+-rw-rw-r--   0 avi        (501) staff       (20)     1262 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/package.json
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.162218 pear-xai-0.0.8/captum/insights/attr_vis/frontend/public/
+-rw-rw-r--   0 avi        (501) staff       (20)      316 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/public/index.html
+-rw-rw-r--   0 avi        (501) staff       (20)      459 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/tsconfig.json
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.162368 pear-xai-0.0.8/captum/insights/attr_vis/frontend/widget/
+-rw-rw-r--   0 avi        (501) staff       (20)     2236 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/widget/webpack.config.js
+-rw-rw-r--   0 avi        (501) staff       (20)   480930 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/frontend/yarn.lock
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.162522 pear-xai-0.0.8/captum/insights/attr_vis/models/
+-rw-rw-r--   0 avi        (501) staff       (20)   249703 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/models/cifar_torchvision.pt
+-rw-rw-r--   0 avi        (501) staff       (20)     3331 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/server.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.165644 pear-xai-0.0.8/captum/insights/attr_vis/widget/
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/widget/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      312 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/widget/_version.py
+-rw-rw-r--   0 avi        (501) staff       (20)       77 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/widget/jupyter-captum-insights.json
+-rw-rw-r--   0 avi        (501) staff       (20)     2057 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/attr_vis/widget/widget.py
+-rw-rw-r--   0 avi        (501) staff       (20)      208 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/insights/example.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.165797 pear-xai-0.0.8/captum/log/
+-rw-rw-r--   0 avi        (501) staff       (20)     1193 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/log/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.165954 pear-xai-0.0.8/captum/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)      204 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.166442 pear-xai-0.0.8/captum/metrics/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)       23 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    26077 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/_core/infidelity.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13251 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/_core/sensitivity.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.166681 pear-xai-0.0.8/captum/metrics/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3261 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/metrics/_utils/batching.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.167274 pear-xai-0.0.8/captum/module/
+-rw-rw-r--   0 avi        (501) staff       (20)      266 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/module/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10241 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/module/binary_concrete_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6914 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/module/gaussian_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8721 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/module/stochastic_gates_base.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.167417 pear-xai-0.0.8/captum/robust/
+-rw-rw-r--   0 avi        (501) staff       (20)      372 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.168167 pear-xai-0.0.8/captum/robust/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8725 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/fgsm.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.168601 pear-xai-0.0.8/captum/robust/_core/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/metrics/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19665 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/metrics/attack_comparator.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18858 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/metrics/min_param_perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1435 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10165 2023-02-27 18:57:42.000000 pear-xai-0.0.8/captum/robust/_core/pgd.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.169505 pear-xai-0.0.8/fast_soft_sort/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3724 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/jax_ops.py
+-rw-rw-r--   0 avi        (501) staff       (20)    12504 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/numpy_ops.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3680 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/pytorch_ops.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3607 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/tf_ops.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.169891 pear-xai-0.0.8/fast_soft_sort/third_party/
+-rw-rw-r--   0 avi        (501) staff       (20)     1570 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/third_party/LICENSE
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/third_party/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     5576 2020-07-28 17:20:24.000000 pear-xai-0.0.8/fast_soft_sort/third_party/isotonic.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.170158 pear-xai-0.0.8/notebooks/
+-rw-r--r--   0 avi        (501) staff       (20)    20209 2023-05-04 15:21:57.000000 pear-xai-0.0.8/notebooks/pear-training-experiment.ipynb
+-rw-r--r--   0 avi        (501) staff       (20)    11179 2023-05-04 15:49:12.000000 pear-xai-0.0.8/notebooks/quickstart.ipynb
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.172177 pear-xai-0.0.8/pear/
+-rw-r--r--   0 avi        (501) staff       (20)      757 2023-05-03 18:30:29.000000 pear-xai-0.0.8/pear/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.138102 pear-xai-0.0.8/pear/datasets/
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.173145 pear-xai-0.0.8/pear/datasets/bankmarketing/
+-rw-r--r--   0 avi        (501) staff       (20)    76729 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/bankmarketing/bankmarketing-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)   230362 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/bankmarketing/bankmarketing-train.csv
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.174804 pear-xai-0.0.8/pear/datasets/californiahousing/
+-rw-r--r--   0 avi        (501) staff       (20)   441167 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/californiahousing/californiahousing-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)  1325430 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/californiahousing/californiahousing-train.csv
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.179611 pear-xai-0.0.8/pear/datasets/electricity/
+-rw-r--r--   0 avi        (501) staff       (20)   636732 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/electricity/electricity-test.csv
+-rw-r--r--   0 avi        (501) staff       (20)  1909510 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/datasets/electricity/electricity-train.csv
+-rw-r--r--   0 avi        (501) staff       (20)     2901 2023-05-04 15:16:13.000000 pear-xai-0.0.8/pear/disagreement_loss.py
+-rw-r--r--   0 avi        (501) staff       (20)    11118 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/disagreement_metrics.py
+-rw-r--r--   0 avi        (501) staff       (20)     5571 2023-05-03 20:35:26.000000 pear-xai-0.0.8/pear/example.py
+-rw-r--r--   0 avi        (501) staff       (20)     7939 2023-05-03 18:30:45.000000 pear-xai-0.0.8/pear/explainers.py
+-rw-r--r--   0 avi        (501) staff       (20)     9559 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/models.py
+-rw-r--r--   0 avi        (501) staff       (20)     4577 2023-03-02 01:56:26.000000 pear-xai-0.0.8/pear/tools.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-04 15:49:38.183142 pear-xai-0.0.8/pear_xai.egg-info/
+-rw-r--r--   0 avi        (501) staff       (20)     2395 2023-05-04 15:49:38.000000 pear-xai-0.0.8/pear_xai.egg-info/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     5639 2023-05-04 15:49:38.000000 pear-xai-0.0.8/pear_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-04 15:49:38.000000 pear-xai-0.0.8/pear_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 avi        (501) staff       (20)      187 2023-05-04 15:49:38.000000 pear-xai-0.0.8/pear_xai.egg-info/requires.txt
+-rw-r--r--   0 avi        (501) staff       (20)       42 2023-05-04 15:49:38.000000 pear-xai-0.0.8/pear_xai.egg-info/top_level.txt
+-rw-r--r--   0 avi        (501) staff       (20)     1423 2023-05-04 15:49:12.000000 pear-xai-0.0.8/pyproject.toml
+-rw-r--r--   0 avi        (501) staff       (20)      171 2023-05-04 15:14:19.000000 pear-xai-0.0.8/requirements.txt
+-rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-04 15:49:38.183555 pear-xai-0.0.8/setup.cfg
```

### Comparing `pear-xai-0.0.7/.gitignore` & `pear-xai-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/LICENSE` & `pear-xai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/PKG-INFO` & `pear-xai-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.0.7
+Version: 0.0.8
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Author-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 Maintainer-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 License: BSD-3-Clause
 Project-URL: homepage, https://arthur.ai
 Project-URL: repository, https://github.com/aks2203/pear-xai
 Project-URL: documentation, https://github.com/aks2203/pear-xai
```

### Comparing `pear-xai-0.0.7/README.md` & `pear-xai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/av.py` & `pear-xai-0.0.8/captum/_utils/av.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/common.py` & `pear-xai-0.0.8/captum/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/gradient.py` & `pear-xai-0.0.8/captum/_utils/gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/models/linear_model/model.py` & `pear-xai-0.0.8/captum/_utils/models/linear_model/model.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/models/linear_model/train.py` & `pear-xai-0.0.8/captum/_utils/models/linear_model/train.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/models/model.py` & `pear-xai-0.0.8/captum/_utils/models/model.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/progress.py` & `pear-xai-0.0.8/captum/_utils/progress.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/sample_gradient.py` & `pear-xai-0.0.8/captum/_utils/sample_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/_utils/typing.py` & `pear-xai-0.0.8/captum/_utils/typing.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/__init__.py` & `pear-xai-0.0.8/captum/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/deep_lift.py` & `pear-xai-0.0.8/captum/attr/_core/deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/feature_ablation.py` & `pear-xai-0.0.8/captum/attr/_core/feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/feature_permutation.py` & `pear-xai-0.0.8/captum/attr/_core/feature_permutation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/gradient_shap.py` & `pear-xai-0.0.8/captum/attr/_core/gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/guided_backprop_deconvnet.py` & `pear-xai-0.0.8/captum/attr/_core/guided_backprop_deconvnet.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/guided_grad_cam.py` & `pear-xai-0.0.8/captum/attr/_core/guided_grad_cam.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/input_x_gradient.py` & `pear-xai-0.0.8/captum/attr/_core/input_x_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/integrated_gradients.py` & `pear-xai-0.0.8/captum/attr/_core/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/kernel_shap.py` & `pear-xai-0.0.8/captum/attr/_core/kernel_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/grad_cam.py` & `pear-xai-0.0.8/captum/attr/_core/layer/grad_cam.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/internal_influence.py` & `pear-xai-0.0.8/captum/attr/_core/layer/internal_influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_activation.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_activation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_conductance.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_conductance.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_deep_lift.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_feature_ablation.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_gradient_shap.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_gradient_x_activation.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_gradient_x_activation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_integrated_gradients.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/layer/layer_lrp.py` & `pear-xai-0.0.8/captum/attr/_core/layer/layer_lrp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/lime.py` & `pear-xai-0.0.8/captum/attr/_core/lime.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/lrp.py` & `pear-xai-0.0.8/captum/attr/_core/lrp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_conductance.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_conductance.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_deep_lift.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_deep_lift.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_feature_ablation.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_feature_ablation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_gradient.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_gradient.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_gradient_shap.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_gradient_shap.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/neuron/neuron_integrated_gradients.py` & `pear-xai-0.0.8/captum/attr/_core/neuron/neuron_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/noise_tunnel.py` & `pear-xai-0.0.8/captum/attr/_core/noise_tunnel.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/occlusion.py` & `pear-xai-0.0.8/captum/attr/_core/occlusion.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/saliency.py` & `pear-xai-0.0.8/captum/attr/_core/saliency.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_core/shapley_value.py` & `pear-xai-0.0.8/captum/attr/_core/shapley_value.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_models/base.py` & `pear-xai-0.0.8/captum/attr/_models/base.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_models/pytext.py` & `pear-xai-0.0.8/captum/attr/_models/pytext.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/approximation_methods.py` & `pear-xai-0.0.8/captum/attr/_utils/approximation_methods.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/attribution.py` & `pear-xai-0.0.8/captum/attr/_utils/attribution.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/batching.py` & `pear-xai-0.0.8/captum/attr/_utils/batching.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/class_summarizer.py` & `pear-xai-0.0.8/captum/attr/_utils/class_summarizer.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/common.py` & `pear-xai-0.0.8/captum/attr/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/input_layer_wrapper.py` & `pear-xai-0.0.8/captum/attr/_utils/input_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/lrp_rules.py` & `pear-xai-0.0.8/captum/attr/_utils/lrp_rules.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/stat.py` & `pear-xai-0.0.8/captum/attr/_utils/stat.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/summarizer.py` & `pear-xai-0.0.8/captum/attr/_utils/summarizer.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/attr/_utils/visualization.py` & `pear-xai-0.0.8/captum/attr/_utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_core/cav.py` & `pear-xai-0.0.8/captum/concept/_core/cav.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_core/concept.py` & `pear-xai-0.0.8/captum/concept/_core/concept.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_core/tcav.py` & `pear-xai-0.0.8/captum/concept/_core/tcav.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_utils/classifier.py` & `pear-xai-0.0.8/captum/concept/_utils/classifier.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_utils/common.py` & `pear-xai-0.0.8/captum/concept/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/concept/_utils/data_iterator.py` & `pear-xai-0.0.8/captum/concept/_utils/data_iterator.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/__init__.py` & `pear-xai-0.0.8/captum/influence/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_core/influence.py` & `pear-xai-0.0.8/captum/influence/_core/influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_core/similarity_influence.py` & `pear-xai-0.0.8/captum/influence/_core/similarity_influence.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_core/tracincp.py` & `pear-xai-0.0.8/captum/influence/_core/tracincp.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_core/tracincp_fast_rand_proj.py` & `pear-xai-0.0.8/captum/influence/_core/tracincp_fast_rand_proj.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_utils/common.py` & `pear-xai-0.0.8/captum/influence/_utils/common.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/influence/_utils/nearest_neighbors.py` & `pear-xai-0.0.8/captum/influence/_utils/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/app.py` & `pear-xai-0.0.8/captum/insights/attr_vis/app.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/attribution_calculation.py` & `pear-xai-0.0.8/captum/insights/attr_vis/attribution_calculation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/config.py` & `pear-xai-0.0.8/captum/insights/attr_vis/config.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/example.py` & `pear-xai-0.0.8/captum/insights/attr_vis/example.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/features.py` & `pear-xai-0.0.8/captum/insights/attr_vis/features.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/frontend/package.json` & `pear-xai-0.0.8/captum/insights/attr_vis/frontend/package.json`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/frontend/widget/webpack.config.js` & `pear-xai-0.0.8/captum/insights/attr_vis/frontend/widget/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/frontend/yarn.lock` & `pear-xai-0.0.8/captum/insights/attr_vis/frontend/yarn.lock`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/models/cifar_torchvision.pt` & `pear-xai-0.0.8/captum/insights/attr_vis/models/cifar_torchvision.pt`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/server.py` & `pear-xai-0.0.8/captum/insights/attr_vis/server.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/insights/attr_vis/widget/widget.py` & `pear-xai-0.0.8/captum/insights/attr_vis/widget/widget.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/log/__init__.py` & `pear-xai-0.0.8/captum/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/metrics/_core/infidelity.py` & `pear-xai-0.0.8/captum/metrics/_core/infidelity.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/metrics/_core/sensitivity.py` & `pear-xai-0.0.8/captum/metrics/_core/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/metrics/_utils/batching.py` & `pear-xai-0.0.8/captum/metrics/_utils/batching.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/module/binary_concrete_stochastic_gates.py` & `pear-xai-0.0.8/captum/module/binary_concrete_stochastic_gates.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/module/gaussian_stochastic_gates.py` & `pear-xai-0.0.8/captum/module/gaussian_stochastic_gates.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/module/stochastic_gates_base.py` & `pear-xai-0.0.8/captum/module/stochastic_gates_base.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/robust/_core/fgsm.py` & `pear-xai-0.0.8/captum/robust/_core/fgsm.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/robust/_core/metrics/attack_comparator.py` & `pear-xai-0.0.8/captum/robust/_core/metrics/attack_comparator.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/robust/_core/metrics/min_param_perturbation.py` & `pear-xai-0.0.8/captum/robust/_core/metrics/min_param_perturbation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/robust/_core/perturbation.py` & `pear-xai-0.0.8/captum/robust/_core/perturbation.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/captum/robust/_core/pgd.py` & `pear-xai-0.0.8/captum/robust/_core/pgd.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/jax_ops.py` & `pear-xai-0.0.8/fast_soft_sort/jax_ops.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/numpy_ops.py` & `pear-xai-0.0.8/fast_soft_sort/numpy_ops.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/pytorch_ops.py` & `pear-xai-0.0.8/fast_soft_sort/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/tf_ops.py` & `pear-xai-0.0.8/fast_soft_sort/tf_ops.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/third_party/LICENSE` & `pear-xai-0.0.8/fast_soft_sort/third_party/LICENSE`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/fast_soft_sort/third_party/isotonic.py` & `pear-xai-0.0.8/fast_soft_sort/third_party/isotonic.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/notebooks/quickstart.ipynb` & `pear-xai-0.0.8/notebooks/quickstart.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -692,8 +692,8 @@
 00002b30: 6578 706f 7274 6572 223a 2022 7079 7468  exporter": "pyth
 00002b40: 6f6e 222c 0a20 2020 2270 7967 6d65 6e74  on",.   "pygment
 00002b50: 735f 6c65 7865 7222 3a20 2269 7079 7468  s_lexer": "ipyth
 00002b60: 6f6e 3322 2c0a 2020 2022 7665 7273 696f  on3",.   "versio
 00002b70: 6e22 3a20 2233 2e31 302e 3422 0a20 207d  n": "3.10.4".  }
 00002b80: 0a20 7d2c 0a20 226e 6266 6f72 6d61 7422  . },. "nbformat"
 00002b90: 3a20 342c 0a20 226e 6266 6f72 6d61 745f  : 4,. "nbformat_
-00002ba0: 6d69 6e6f 7222 3a20 310a 7d0a            minor": 1.}.
+00002ba0: 6d69 6e6f 7222 3a20 310a 7d              minor": 1.}
```

### Comparing `pear-xai-0.0.7/pear/__init__.py` & `pear-xai-0.0.8/pear/__init__.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/bankmarketing/bankmarketing-test.csv` & `pear-xai-0.0.8/pear/datasets/bankmarketing/bankmarketing-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/bankmarketing/bankmarketing-train.csv` & `pear-xai-0.0.8/pear/datasets/bankmarketing/bankmarketing-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/californiahousing/californiahousing-test.csv` & `pear-xai-0.0.8/pear/datasets/californiahousing/californiahousing-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/californiahousing/californiahousing-train.csv` & `pear-xai-0.0.8/pear/datasets/californiahousing/californiahousing-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/electricity/electricity-test.csv` & `pear-xai-0.0.8/pear/datasets/electricity/electricity-test.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/datasets/electricity/electricity-train.csv` & `pear-xai-0.0.8/pear/datasets/electricity/electricity-train.csv`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/disagreement_loss.py` & `pear-xai-0.0.8/pear/disagreement_loss.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/disagreement_metrics.py` & `pear-xai-0.0.8/pear/disagreement_metrics.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/example.py` & `pear-xai-0.0.8/pear/example.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/explainers.py` & `pear-xai-0.0.8/pear/explainers.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/models.py` & `pear-xai-0.0.8/pear/models.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear/tools.py` & `pear-xai-0.0.8/pear/tools.py`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pear_xai.egg-info/PKG-INFO` & `pear-xai-0.0.8/pear_xai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.0.7
+Version: 0.0.8
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Author-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 Maintainer-email: Avi Schwarzschild <avi1@umd.edu>, Max Cembalest <max.cembalest@arthur.ai>, Karthik Rao <karthik@arthur.ai>
 License: BSD-3-Clause
 Project-URL: homepage, https://arthur.ai
 Project-URL: repository, https://github.com/aks2203/pear-xai
 Project-URL: documentation, https://github.com/aks2203/pear-xai
```

### Comparing `pear-xai-0.0.7/pear_xai.egg-info/SOURCES.txt` & `pear-xai-0.0.8/pear_xai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pear-xai-0.0.7/pyproject.toml` & `pear-xai-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm", "torch==1.11.0", "numpy==1.23.2"]
+requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pear-xai"
 description = "PEAR: Post-hoc Explainer Agreement Regularization"
 readme = "README.md"
 authors = [ {name="Avi Schwarzschild", email="avi1@umd.edu"}, {name="Max Cembalest", email="max.cembalest@arthur.ai"},
@@ -22,15 +22,15 @@
                 "scikit-learn==1.2.2",
                 "seaborn==0.12.2",
                 "shap==0.41.0",
                 "sklearn==0.0",
                 "tabulate==0.8.10",
                 "torchvision==0.12.0",
                 "tqdm==4.64.0"]
-version = "0.0.7"
+version = "0.0.8"
 
 [tools.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages]
 find = {}
```

