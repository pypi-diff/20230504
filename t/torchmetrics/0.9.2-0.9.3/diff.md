# Comparing `tmp/torchmetrics-0.9.2.tar.gz` & `tmp/torchmetrics-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchmetrics-0.9.2.tar", last modified: Wed Jun 29 22:48:43 2022, max compression
+gzip compressed data, was "dist/torchmetrics-0.9.3.tar", last modified: Sat Jul 23 21:26:43 2022, max compression
```

## Comparing `torchmetrics-0.9.2.tar` & `torchmetrics-0.9.3.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    42506 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15228 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13645 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/audio.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/audio_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/detection.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/detection_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/image.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/image_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/integrate.txt
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/text.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements/text_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4282 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/tm_examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/tm_examples/bert_score-own_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/tm_examples/detection_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/tm_examples/rouge_score-own_normalizer_and_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/audio/
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (121)     4062 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4972 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12233 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/auc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7171 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/avg_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)    13267 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/binned_precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     7808 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (121)    12869 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (121)     5206 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4986 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (121)    14054 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)     8388 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7515 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/classification/stat_scores.py
--rw-r--r--   0 runner    (1001) docker     (121)    20398 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40453 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/detection/mean_ap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (121)     7901 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (121)    11309 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18999 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4314 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/auc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12200 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10436 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     8681 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    13030 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (121)    17329 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (121)    26312 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (121)    13738 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    10661 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (121)    11841 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (121)    19215 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4999 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     4605 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/gradients.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (121)    20208 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/image/uqi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/cosine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/pairwise/manhattan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3387 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (121)     6317 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28822 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (121)     7541 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (121)    25984 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (121)    17569 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (121)    17380 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (121)    21159 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (121)    13141 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (121)     9911 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (121)    23214 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/functional/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/image/
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (121)    11943 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/inception.py
--rw-r--r--   0 runner    (1001) docker     (121)    11596 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/kid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5864 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/lpip.py
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (121)    39275 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (121)     5076 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4951 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (121)    11879 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/retrieval/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/setup_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/text/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10899 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8714 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7428 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (121)     4838 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32926 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/compute.py
--rw-r--r--   0 runner    (1001) docker     (121)     8816 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4919 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/utilities/prints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/classwise.py
--rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (121)     7423 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (121)     9558 2022-06-29 22:48:38.000000 torchmetrics-0.9.2/torchmetrics/wrappers/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15228 2022-06-29 22:48:42.000000 torchmetrics-0.9.2/torchmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7831 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 22:48:42.000000 torchmetrics-0.9.2/torchmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 22:48:42.000000 torchmetrics-0.9.2/torchmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-29 22:48:43.000000 torchmetrics-0.9.2/torchmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    43054 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12528 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10946 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/audio.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/audio_test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/detection.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/detection_test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/image.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/image_test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/integrate.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/text.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements/text_test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4282 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/tm_examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/tm_examples/bert_score-own_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/tm_examples/detection_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/tm_examples/rouge_score-own_normalizer_and_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4062 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4972 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12243 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/auc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7171 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5779 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/avg_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13267 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/binned_precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4109 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7818 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12889 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5206 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5439 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14074 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8388 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7525 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/classification/stat_scores.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20398 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40453 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/detection/mean_ap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7901 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11309 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19009 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4314 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/auc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12200 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10436 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8681 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13050 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17349 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26362 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13738 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10661 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11841 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9787 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19215 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4999 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4605 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20298 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/image/uqi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/pairwise/manhattan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3387 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6317 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3974 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28822 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7541 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25984 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17569 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17380 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21159 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13141 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9911 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23214 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/functional/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11943 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/inception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11596 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/kid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5864 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3548 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39874 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3230 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4820 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5076 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5780 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4951 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11879 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2758 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/retrieval/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/setup_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/text/
+-rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10899 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8714 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7428 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4647 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4838 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32926 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/compute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8816 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4919 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/utilities/prints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7423 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9558 2022-07-23 21:26:38.000000 torchmetrics-0.9.3/torchmetrics/wrappers/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12528 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7831 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-23 21:26:43.000000 torchmetrics-0.9.3/torchmetrics.egg-info/top_level.txt
```

### Comparing `torchmetrics-0.9.2/CHANGELOG.md` & `torchmetrics-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **Note: we move fast, but still we preserve 0.1 version (one feature release) back compatibility.**
 
 
+## [0.9.3] - 2022-08-22
+
+### Added
+
+- Added global option `sync_on_compute` to disable automatic syncronization when `compute` is called ([#1107](https://github.dev/Lightning-AI/metrics/pull/1107))
+
+### Fixed
+
+- Fixed missing reset in `ClasswiseWrapper` ([#1129](https://github.com/Lightning-AI/metrics/pull/1129))
+- Fixed JaccardIndex multi-label compute ([#1125](https://github.com/Lightning-AI/metrics/pull/1125))
+- Fix SSIM propagate device if `gaussian_kernel` is False, add test ([#1149](https://github.com/Lightning-AI/metrics/pull/1149))
+
+
 ## [0.9.2] - 2022-06-29
 
 ### Fixed
 
 - Fixed mAP calculation for areas with 0 predictions ([#1080](https://github.com/Lightning-AI/metrics/pull/1080))
 - Fixed bug where avg precision state and auroc state was not merge when using MetricCollections ([#1086](https://github.com/Lightning-AI/metrics/pull/1086))
 - Skip box conversion if no boxes are present in `MeanAveragePrecision` ([#1097](https://github.com/Lightning-AI/metrics/pull/1097))
```

### Comparing `torchmetrics-0.9.2/CITATION.cff` & `torchmetrics-0.9.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/LICENSE` & `torchmetrics-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/MANIFEST.in` & `torchmetrics-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/PKG-INFO` & `torchmetrics-0.9.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 0.9.2
+Version: 0.9.3
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/metrics
 Download-URL: https://github.com/Lightning-AI/metrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/metrics/issues
@@ -34,42 +34,42 @@
 Provides-Extra: test
 Provides-Extra: text
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/metrics/raw/v0.9.2/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/metrics/raw/v0.9.3/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/v0.9.2">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v0.9.3">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/metrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-full.yml)
-[![PyTorch & Conda](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml/badge.svg?tag=v0.9.2)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status/Lightning-AI.metrics?branchName=refs%2Ftags%2Fv0.9.2)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv0.9.2)
-[![codecov](https://codecov.io/gh/Lightning-AI/metrics/release/v0.9.2/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/metrics)
+[![PyTorch & Conda](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml/badge.svg?tag=v0.9.3)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status/Lightning-AI.metrics?branchName=refs%2Ftags%2Fv0.9.3)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv0.9.3)
+[![codecov](https://codecov.io/gh/Lightning-AI/metrics/release/v0.9.3/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/metrics)
 
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/metrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/metrics/master)
 
@@ -305,54 +305,23 @@
 acc = torchmetrics.functional.accuracy(preds, target)
 ```
 
 ### Covered domains and example metrics
 
 We currently have implemented metrics within the following domains:
 
-- Audio (
-  [ScaleInvariantSignalDistortionRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#ScaleInvariantSignalDistortionRatio),
-  [ScaleInvariantSignalNoiseRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#ScaleInvariantSignalNoiseRatio),
-  [SignalNoiseRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#SignalNoiseRatio)
-  and [few more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#audio-metrics)
-  )
-- Classification (
-  [Accuracy](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#accuracy),
-  [F1Score](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#f1score),
-  [AUROC](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#auroc)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#classification-metrics)
-  )
-- Detection (
-  [MeanAveragePrecision](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#meanaverageprecision))
-- Information Retrieval (
-  [RetrievalMAP](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalmap),
-  [RetrievalMRR](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalmrr),
-  [RetrievalNormalizedDCG](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalnormalizeddcg)
-  and [few more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrieval)
-  )
-- Image (
-  [FrechetInceptionDistance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#FrechetInceptionDistance),
-  [KernelInceptionDistance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#KernelInceptionDistance),
-  [StructuralSimilarityIndexMeasure](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#StructuralSimilarityIndexMeasure)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#image-metrics)
-  )
-- Regression (
-  [ExplainedVariance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#explainedvariance),
-  [PearsonCorrCoef](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#pearsoncorrcoef),
-  [R2Score](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#r2score)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#regression-metrics)
-  )
-- Text (
-  [BleuScore](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#bleuscore),
-  [RougeScore](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#rougescore),
-  [WordErrorRate](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#WordErrorRate)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#text)
-  )
+- Audio
+- Classification
+- Detection
+- Information Retrieval
+- Image
+- Regression
+- Text
 
-In total TorchMetrics contains 80+ metrics!
+In total TorchMetrics contains [80+ metrics](https://torchmetrics.readthedocs.io/en/v0.9.3all-metrics.html)!
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
 But we're looking for incredible contributors like you to submit new metrics
 and improve existing ones!
```

### Comparing `torchmetrics-0.9.2/README.md` & `torchmetrics-0.9.3/torchmetrics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,75 @@
+Metadata-Version: 2.1
+Name: torchmetrics
+Version: 0.9.3
+Summary: PyTorch native Metrics
+Home-page: https://github.com/Lightning-AI/metrics
+Download-URL: https://github.com/Lightning-AI/metrics/archive/master.zip
+Author: Lightning-AI et al.
+Author-email: name@pytorchlightning.ai
+License: Apache-2.0
+Project-URL: Bug Tracker, https://github.com/Lightning-AI/metrics/issues
+Project-URL: Documentation, https://torchmetrics.rtfd.io/en/latest/
+Project-URL: Source Code, https://github.com/Lightning-AI/metrics
+Keywords: deep learning,machine learning,pytorch,metrics,AI
+Classifier: Environment :: Console
+Classifier: Natural Language :: English
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: audio
+Provides-Extra: detection
+Provides-Extra: docs
+Provides-Extra: image
+Provides-Extra: integrate
+Provides-Extra: test
+Provides-Extra: text
+Provides-Extra: all
+License-File: LICENSE
+
 <div align="center">
 
-<img src="docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/metrics/raw/v0.9.3/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/stable/">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v0.9.3">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/metrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-full.yml)
-[![PyTorch & Conda](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml/badge.svg?branch=master&event=push)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status/Lightning-AI.metrics?branchName=master)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=3&branchName=master)
-[![codecov](https://codecov.io/gh/Lightning-AI/metrics/branch/master/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/metrics)
+[![PyTorch & Conda](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml/badge.svg?tag=v0.9.3)](https://github.com/Lightning-AI/metrics/actions/workflows/ci_test-conda.yml)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status/Lightning-AI.metrics?branchName=refs%2Ftags%2Fv0.9.3)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv0.9.3)
+[![codecov](https://codecov.io/gh/Lightning-AI/metrics/release/v0.9.3/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/metrics)
 
 [![Slack](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://www.pytorchlightning.ai/community)
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/metrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/metrics/master)
 
@@ -267,54 +305,23 @@
 acc = torchmetrics.functional.accuracy(preds, target)
 ```
 
 ### Covered domains and example metrics
 
 We currently have implemented metrics within the following domains:
 
-- Audio (
-  [ScaleInvariantSignalDistortionRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#ScaleInvariantSignalDistortionRatio),
-  [ScaleInvariantSignalNoiseRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#ScaleInvariantSignalNoiseRatio),
-  [SignalNoiseRatio](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#SignalNoiseRatio)
-  and [few more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#audio-metrics)
-  )
-- Classification (
-  [Accuracy](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#accuracy),
-  [F1Score](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#f1score),
-  [AUROC](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#auroc)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#classification-metrics)
-  )
-- Detection (
-  [MeanAveragePrecision](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#meanaverageprecision))
-- Information Retrieval (
-  [RetrievalMAP](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalmap),
-  [RetrievalMRR](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalmrr),
-  [RetrievalNormalizedDCG](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrievalnormalizeddcg)
-  and [few more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#retrieval)
-  )
-- Image (
-  [FrechetInceptionDistance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#FrechetInceptionDistance),
-  [KernelInceptionDistance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#KernelInceptionDistance),
-  [StructuralSimilarityIndexMeasure](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#StructuralSimilarityIndexMeasure)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#image-metrics)
-  )
-- Regression (
-  [ExplainedVariance](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#explainedvariance),
-  [PearsonCorrCoef](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#pearsoncorrcoef),
-  [R2Score](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#r2score)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#regression-metrics)
-  )
-- Text (
-  [BleuScore](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#bleuscore),
-  [RougeScore](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#rougescore),
-  [WordErrorRate](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#WordErrorRate)
-  and [many more](https://torchmetrics.readthedocs.io/en/latest/references/modules.html#text)
-  )
+- Audio
+- Classification
+- Detection
+- Information Retrieval
+- Image
+- Regression
+- Text
 
-In total TorchMetrics contains 80+ metrics!
+In total TorchMetrics contains [80+ metrics](https://torchmetrics.readthedocs.io/en/v0.9.3all-metrics.html)!
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
 But we're looking for incredible contributors like you to submit new metrics
 and improve existing ones!
```

### Comparing `torchmetrics-0.9.2/setup.cfg` & `torchmetrics-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/setup.py` & `torchmetrics-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/tm_examples/bert_score-own_model.py` & `torchmetrics-0.9.3/tm_examples/bert_score-own_model.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/tm_examples/detection_map.py` & `torchmetrics-0.9.3/tm_examples/detection_map.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/tm_examples/rouge_score-own_normalizer_and_tokenizer.py` & `torchmetrics-0.9.3/tm_examples/rouge_score-own_normalizer_and_tokenizer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/__about__.py` & `torchmetrics-0.9.3/torchmetrics/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __author__ = "Lightning-AI et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-2022, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/metrics"
 __docs__ = "PyTorch native Metrics"
 __docs_url__ = "https://torchmetrics.readthedocs.io/en/stable/"
```

### Comparing `torchmetrics-0.9.2/torchmetrics/__init__.py` & `torchmetrics-0.9.3/torchmetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/aggregation.py` & `torchmetrics-0.9.3/torchmetrics/aggregation.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/__init__.py` & `torchmetrics-0.9.3/torchmetrics/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/pesq.py` & `torchmetrics-0.9.3/torchmetrics/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/pit.py` & `torchmetrics-0.9.3/torchmetrics/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/sdr.py` & `torchmetrics-0.9.3/torchmetrics/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/snr.py` & `torchmetrics-0.9.3/torchmetrics/audio/snr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/audio/stoi.py` & `torchmetrics-0.9.3/torchmetrics/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/__init__.py` & `torchmetrics-0.9.3/torchmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/accuracy.py` & `torchmetrics-0.9.3/torchmetrics/classification/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     correct: Tensor
     total: Tensor
 
     def __init__(
         self,
         threshold: float = 0.5,
         num_classes: Optional[int] = None,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         subset_accuracy: bool = False,
         **kwargs: Any,
     ) -> None:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/auc.py` & `torchmetrics-0.9.3/torchmetrics/classification/auc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/auroc.py` & `torchmetrics-0.9.3/torchmetrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/avg_precision.py` & `torchmetrics-0.9.3/torchmetrics/classification/avg_precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         average: Optional[str] = "macro",
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
 
         self.num_classes = num_classes
         self.pos_label = pos_label
-        allowed_average = ("micro", "macro", "weighted", None)
+        allowed_average = ("micro", "macro", "weighted", "none", None)
         if average not in allowed_average:
             raise ValueError(f"Expected argument `average` to be one of {allowed_average}" f" but got {average}")
         self.average = average
 
         self.add_state("preds", default=[], dist_reduce_fx="cat")
         self.add_state("target", default=[], dist_reduce_fx="cat")
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/binned_precision_recall.py` & `torchmetrics-0.9.3/torchmetrics/classification/binned_precision_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/calibration_error.py` & `torchmetrics-0.9.3/torchmetrics/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/cohen_kappa.py` & `torchmetrics-0.9.3/torchmetrics/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/confusion_matrix.py` & `torchmetrics-0.9.3/torchmetrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/dice.py` & `torchmetrics-0.9.3/torchmetrics/classification/dice.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     full_state_update: bool = False
 
     def __init__(
         self,
         zero_division: int = 0,
         num_classes: Optional[int] = None,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = "global",
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         allowed_average = ("micro", "macro", "weighted", "samples", "none", None)
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/f_beta.py` & `torchmetrics-0.9.3/torchmetrics/classification/f_beta.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: Optional[int] = None,
         beta: float = 1.0,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         self.beta = beta
@@ -251,15 +251,15 @@
     higher_is_better: bool = True
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: Optional[int] = None,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/hamming.py` & `torchmetrics-0.9.3/torchmetrics/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/hinge.py` & `torchmetrics-0.9.3/torchmetrics/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/jaccard.py` & `torchmetrics-0.9.3/torchmetrics/classification/jaccard.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,29 @@
         )
         self.average = average
         self.ignore_index = ignore_index
         self.absent_score = absent_score
 
     def compute(self) -> Tensor:
         """Computes intersection over union (IoU)"""
-        return _jaccard_from_confmat(
-            self.confmat,
-            self.num_classes,
-            self.average,
-            self.ignore_index,
-            self.absent_score,
-        )
+
+        if self.multilabel:
+            return torch.stack(
+                [
+                    _jaccard_from_confmat(
+                        confmat,
+                        2,
+                        self.average,
+                        self.ignore_index,
+                        self.absent_score,
+                    )[1]
+                    for confmat in self.confmat
+                ]
+            )
+        else:
+            return _jaccard_from_confmat(
+                self.confmat,
+                self.num_classes,
+                self.average,
+                self.ignore_index,
+                self.absent_score,
+            )
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/kl_divergence.py` & `torchmetrics-0.9.3/torchmetrics/classification/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/matthews_corrcoef.py` & `torchmetrics-0.9.3/torchmetrics/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/precision_recall.py` & `torchmetrics-0.9.3/torchmetrics/classification/precision_recall.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     higher_is_better = True
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: Optional[int] = None,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         allowed_average = ["micro", "macro", "weighted", "samples", "none", None]
@@ -252,15 +252,15 @@
     higher_is_better: bool = True
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: Optional[int] = None,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         allowed_average = ["micro", "macro", "weighted", "samples", "none", None]
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/precision_recall_curve.py` & `torchmetrics-0.9.3/torchmetrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/ranking.py` & `torchmetrics-0.9.3/torchmetrics/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/roc.py` & `torchmetrics-0.9.3/torchmetrics/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/specificity.py` & `torchmetrics-0.9.3/torchmetrics/classification/specificity.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     higher_is_better: bool = True
     full_state_update: bool = False
 
     def __init__(
         self,
         num_classes: Optional[int] = None,
         threshold: float = 0.5,
-        average: str = "micro",
+        average: Optional[str] = "micro",
         mdmc_average: Optional[str] = None,
         ignore_index: Optional[int] = None,
         top_k: Optional[int] = None,
         multiclass: Optional[bool] = None,
         **kwargs: Any,
     ) -> None:
         allowed_average = ["micro", "macro", "weighted", "samples", "none", None]
```

### Comparing `torchmetrics-0.9.2/torchmetrics/classification/stat_scores.py` & `torchmetrics-0.9.3/torchmetrics/classification/stat_scores.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/collections.py` & `torchmetrics-0.9.3/torchmetrics/collections.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/detection/__init__.py` & `torchmetrics-0.9.3/torchmetrics/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/detection/mean_ap.py` & `torchmetrics-0.9.3/torchmetrics/detection/mean_ap.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/pesq.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/pit.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/sdr.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/snr.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/snr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/audio/stoi.py` & `torchmetrics-0.9.3/torchmetrics/functional/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/accuracy.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
     return correct.float() / total
 
 
 def accuracy(
     preds: Tensor,
     target: Tensor,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = "global",
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     subset_accuracy: bool = False,
     num_classes: Optional[int] = None,
     multiclass: Optional[bool] = None,
     ignore_index: Optional[int] = None,
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/auc.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/auc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/auroc.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/average_precision.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/calibration_error.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/cohen_kappa.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/confusion_matrix.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/dice.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/dice.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     )
 
 
 def _dice_compute(
     tp: Tensor,
     fp: Tensor,
     fn: Tensor,
-    average: str,
+    average: Optional[str],
     mdmc_average: Optional[str],
     zero_division: int = 0,
 ) -> Tensor:
     """Computes dice from the stat scores: true positives, false positives, false negatives.
 
     Args:
         tp: True positives
@@ -155,15 +155,15 @@
     )
 
 
 def dice(
     preds: Tensor,
     target: Tensor,
     zero_division: int = 0,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = "global",
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     num_classes: Optional[int] = None,
     multiclass: Optional[bool] = None,
     ignore_index: Optional[int] = None,
 ) -> Tensor:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/f_beta.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/f_beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     )
 
 
 def fbeta_score(
     preds: Tensor,
     target: Tensor,
     beta: float = 1.0,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tensor:
@@ -244,15 +244,15 @@
     return _fbeta_compute(tp, fp, tn, fn, beta, ignore_index, average, mdmc_average)
 
 
 def f1_score(
     preds: Tensor,
     target: Tensor,
     beta: float = 1.0,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tensor:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/hamming.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/hinge.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/jaccard.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/kl_divergence.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/matthews_corrcoef.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/precision_recall.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/precision_recall.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from torchmetrics.utilities.enums import AverageMethod, MDMCAverageMethod
 
 
 def _precision_compute(
     tp: Tensor,
     fp: Tensor,
     fn: Tensor,
-    average: str,
+    average: Optional[str],
     mdmc_average: Optional[str],
 ) -> Tensor:
     """Computes precision from the stat scores: true positives, false positives, true negatives, false negatives.
 
     Args:
         tp: True positives
         fp: False positives
@@ -71,15 +71,15 @@
         mdmc_average=mdmc_average,
     )
 
 
 def precision(
     preds: Tensor,
     target: Tensor,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tensor:
@@ -213,15 +213,15 @@
     return _precision_compute(tp, fp, fn, average, mdmc_average)
 
 
 def _recall_compute(
     tp: Tensor,
     fp: Tensor,
     fn: Tensor,
-    average: str,
+    average: Optional[str],
     mdmc_average: Optional[str],
 ) -> Tensor:
     """Computes precision from the stat scores: true positives, false positives, true negatives, false negatives.
 
     Args:
         tp: True positives
         fp: False positives
@@ -263,15 +263,15 @@
         mdmc_average=mdmc_average,
     )
 
 
 def recall(
     preds: Tensor,
     target: Tensor,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tensor:
@@ -405,15 +405,15 @@
 
     return _recall_compute(tp, fp, fn, average, mdmc_average)
 
 
 def precision_recall(
     preds: Tensor,
     target: Tensor,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tuple[Tensor, Tensor]:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/precision_recall_curve.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/ranking.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/roc.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/specificity.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/specificity.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def _specificity_compute(
     tp: Tensor,
     fp: Tensor,
     tn: Tensor,
     fn: Tensor,
-    average: str,
+    average: Optional[str],
     mdmc_average: Optional[str],
 ) -> Tensor:
     """Computes specificity from the stat scores: true positives, false positives, true negatives, false negatives.
 
     Args:
         tp: True positives
         fp: False positives
@@ -66,15 +66,15 @@
         mdmc_average=mdmc_average,
     )
 
 
 def specificity(
     preds: Tensor,
     target: Tensor,
-    average: str = "micro",
+    average: Optional[str] = "micro",
     mdmc_average: Optional[str] = None,
     ignore_index: Optional[int] = None,
     num_classes: Optional[int] = None,
     threshold: float = 0.5,
     top_k: Optional[int] = None,
     multiclass: Optional[bool] = None,
 ) -> Tensor:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/classification/stat_scores.py` & `torchmetrics-0.9.3/torchmetrics/functional/classification/stat_scores.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/d_lambda.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/ergas.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/gradients.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/gradients.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/helper.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/psnr.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/sam.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/ssim.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/ssim.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,17 @@
     else:
         preds = F.pad(preds, (pad_w, pad_w, pad_h, pad_h), mode="reflect")
         target = F.pad(target, (pad_w, pad_w, pad_h, pad_h), mode="reflect")
         if gaussian_kernel:
             kernel = _gaussian_kernel_2d(channel, gauss_kernel_size, sigma, dtype, device)
 
     if not gaussian_kernel:
-        kernel = torch.ones((1, 1, *kernel_size)) / torch.prod(Tensor(kernel_size))
+        kernel = torch.ones((channel, 1, *kernel_size), dtype=dtype, device=device) / torch.prod(
+            torch.tensor(kernel_size, dtype=dtype, device=device)
+        )
 
     input_list = torch.cat((preds, target, preds * preds, target * target, preds * target))  # (5 * B, C, H, W)
 
     if is_3d:
         outputs = F.conv3d(input_list, kernel, groups=channel)
     else:
         outputs = F.conv2d(input_list, kernel, groups=channel)
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/image/uqi.py` & `torchmetrics-0.9.3/torchmetrics/functional/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/cosine.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/cosine.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     reduction: Literal["mean", "sum", "none", None] = None,
     zero_diagonal: Optional[bool] = None,
 ) -> Tensor:
     r"""Calculates pairwise cosine similarity:
 
     .. math::
         s_{cos}(x,y) = \frac{<x,y>}{||x|| \cdot ||y||}
-                     = \frac{\sum_{d=1}^D x_d \cdot y_d }{\sqrt{\sum_{d=1}^D x_i^2} \cdot \sqrt{\sum_{d=1}^D x_i^2}}
+                     = \frac{\sum_{d=1}^D x_d \cdot y_d }{\sqrt{\sum_{d=1}^D x_i^2} \cdot \sqrt{\sum_{d=1}^D y_i^2}}
 
     If both :math:`x` and :math:`y` are passed in, the calculation will be performed pairwise
     between the rows of :math:`x` and :math:`y`.
     If only :math:`x` is passed in, the calculation will be performed between the rows of :math:`x`.
 
     Args:
         x: Tensor with shape ``[N, d]``
```

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/euclidean.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/euclidean.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/helpers.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/linear.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/linear.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/pairwise/manhattan.py` & `torchmetrics-0.9.3/torchmetrics/functional/pairwise/manhattan.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/cosine_similarity.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/explained_variance.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/log_mse.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/mae.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/mape.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/mse.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/pearson.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/r2.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/spearman.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/symmetric_mape.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/tweedie_deviance.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/regression/wmape.py` & `torchmetrics-0.9.3/torchmetrics/functional/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/average_precision.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/fall_out.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/hit_rate.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/ndcg.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/precision.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/precision_recall_curve.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/r_precision.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/recall.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/retrieval/reciprocal_rank.py` & `torchmetrics-0.9.3/torchmetrics/functional/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/__init__.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/bert.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/bleu.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/cer.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/chrf.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/eed.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/helper.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/mer.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/rouge.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/sacre_bleu.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/squad.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/ter.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/wer.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/wil.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/functional/text/wip.py` & `torchmetrics-0.9.3/torchmetrics/functional/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/__init__.py` & `torchmetrics-0.9.3/torchmetrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/d_lambda.py` & `torchmetrics-0.9.3/torchmetrics/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/ergas.py` & `torchmetrics-0.9.3/torchmetrics/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/fid.py` & `torchmetrics-0.9.3/torchmetrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/inception.py` & `torchmetrics-0.9.3/torchmetrics/image/inception.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/kid.py` & `torchmetrics-0.9.3/torchmetrics/image/kid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/lpip.py` & `torchmetrics-0.9.3/torchmetrics/image/lpip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/psnr.py` & `torchmetrics-0.9.3/torchmetrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/sam.py` & `torchmetrics-0.9.3/torchmetrics/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/ssim.py` & `torchmetrics-0.9.3/torchmetrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/image/uqi.py` & `torchmetrics-0.9.3/torchmetrics/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/metric.py` & `torchmetrics-0.9.3/torchmetrics/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         automatically calls ``update()`` and also returns the metric value at the current step.
 
     Args:
         kwargs: additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
             - compute_on_cpu: If metric state should be stored on CPU during computations. Only works
                 for list states.
-            - dist_sync_on_step: If metric state should synchronize on ``forward()``
-            - process_group: The process group on which the synchronization is called
-            - dist_sync_fn: function that performs the allgather option on the metric state
+            - dist_sync_on_step: If metric state should synchronize on ``forward()``. Default is ``False``
+            - process_group: The process group on which the synchronization is called. Default is the world.
+            - dist_sync_fn: function that performs the allgather option on the metric state. Default is an
+                custom implementation that calls ``torch.distributed.all_gather`` internally.
+            - sync_on_compute: If metric state should synchronize when ``compute`` is called. Default is ``True``-
     """
 
     __jit_ignored_attributes__ = ["device"]
     __jit_unused_properties__ = ["is_differentiable"]
     is_differentiable: Optional[bool] = None
     higher_is_better: Optional[bool] = None
     full_state_update: Optional[bool] = None
@@ -104,22 +106,28 @@
 
         self.dist_sync_fn = kwargs.pop("dist_sync_fn", None)
         if self.dist_sync_fn is not None and not callable(self.dist_sync_fn):
             raise ValueError(
                 f"Expected keyword argument `dist_sync_fn` to be an callable function but got {self.dist_sync_fn}"
             )
 
+        self.sync_on_compute = kwargs.pop("sync_on_compute", True)
+        if not isinstance(self.sync_on_compute, bool):
+            raise ValueError(
+                f"Expected keyword argument `sync_on_compute` to be a `bool` but got {self.sync_on_compute}"
+            )
+
         # initialize
         self._update_signature = inspect.signature(self.update)
         self.update: Callable = self._wrap_update(self.update)  # type: ignore
         self.compute: Callable = self._wrap_compute(self.compute)  # type: ignore
         self._computed = None
         self._forward_cache = None
         self._update_count = 0
-        self._to_sync = True
+        self._to_sync = self.sync_on_compute
         self._should_unsync = True
         self._enable_grad = False
 
         # initialize state
         self._defaults: Dict[str, Union[List, Tensor]] = {}
         self._persistent: Dict[str, bool] = {}
         self._reductions: Dict[str, Union[str, Callable[..., Any], None]] = {}
@@ -131,15 +139,15 @@
         if self.full_state_update is None and not is_overridden("forward", self, Metric):
             rank_zero_warn(
                 f"""Torchmetrics v0.9 introduced a new argument class property called `full_state_update` that has
                 not been set for this class ({self.__class__.__name__}). The property determines if `update` by
                 default needs access to the full metric state. If this is not the case, significant speedups can be
                 achieved and we recommend setting this to `False`.
                 We provide an checking function
-                `from torchmetrics.utilities import check_forward_no_full_state`
+                `from torchmetrics.utilities import check_forward_full_state_property`
                 that can be used to check if the `full_state_update=True` (old and potential slower behaviour,
                 default for now) or if `full_state_update=False` can be used safely.
                 """,
                 UserWarning,
             )
 
     @property
@@ -268,15 +276,15 @@
         for attr, val in cache.items():
             setattr(self, attr, val)
         self._update_count = _update_count
 
         # restore context
         self._is_synced = False
         self._should_unsync = True
-        self._to_sync = True
+        self._to_sync = self.sync_on_compute
         self._computed = None
         self._enable_grad = False
         self.compute_on_cpu = _temp_compute_on_cpu
 
         return batch_val
 
     def _forward_reduce_state_update(self, *args: Any, **kwargs: Any) -> Any:
@@ -305,15 +313,15 @@
         self._update_count = _update_count + 1
         with torch.no_grad():
             self._reduce_states(global_state)
 
         # restore context
         self._is_synced = False
         self._should_unsync = True
-        self._to_sync = True
+        self._to_sync = self.sync_on_compute
         self._computed = None
         self._enable_grad = False
         self.compute_on_cpu = _temp_compute_on_cpu
 
         return batch_val
 
     def _reduce_states(self, incoming_state: Dict[str, Any]) -> None:
```

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/__init__.py` & `torchmetrics-0.9.3/torchmetrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/cosine_similarity.py` & `torchmetrics-0.9.3/torchmetrics/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/explained_variance.py` & `torchmetrics-0.9.3/torchmetrics/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/log_mse.py` & `torchmetrics-0.9.3/torchmetrics/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/mae.py` & `torchmetrics-0.9.3/torchmetrics/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/mape.py` & `torchmetrics-0.9.3/torchmetrics/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/mse.py` & `torchmetrics-0.9.3/torchmetrics/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/pearson.py` & `torchmetrics-0.9.3/torchmetrics/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/r2.py` & `torchmetrics-0.9.3/torchmetrics/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/spearman.py` & `torchmetrics-0.9.3/torchmetrics/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/symmetric_mape.py` & `torchmetrics-0.9.3/torchmetrics/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/tweedie_deviance.py` & `torchmetrics-0.9.3/torchmetrics/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/regression/wmape.py` & `torchmetrics-0.9.3/torchmetrics/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/__init__.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/average_precision.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/base.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/fall_out.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/hit_rate.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/ndcg.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/precision.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/precision_recall_curve.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/r_precision.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/recall.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/retrieval/reciprocal_rank.py` & `torchmetrics-0.9.3/torchmetrics/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/setup_tools.py` & `torchmetrics-0.9.3/torchmetrics/setup_tools.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/__init__.py` & `torchmetrics-0.9.3/torchmetrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/bert.py` & `torchmetrics-0.9.3/torchmetrics/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/bleu.py` & `torchmetrics-0.9.3/torchmetrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/cer.py` & `torchmetrics-0.9.3/torchmetrics/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/chrf.py` & `torchmetrics-0.9.3/torchmetrics/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/eed.py` & `torchmetrics-0.9.3/torchmetrics/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/mer.py` & `torchmetrics-0.9.3/torchmetrics/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/rouge.py` & `torchmetrics-0.9.3/torchmetrics/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/sacre_bleu.py` & `torchmetrics-0.9.3/torchmetrics/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/squad.py` & `torchmetrics-0.9.3/torchmetrics/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/ter.py` & `torchmetrics-0.9.3/torchmetrics/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/wer.py` & `torchmetrics-0.9.3/torchmetrics/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/wil.py` & `torchmetrics-0.9.3/torchmetrics/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/text/wip.py` & `torchmetrics-0.9.3/torchmetrics/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/checks.py` & `torchmetrics-0.9.3/torchmetrics/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/compute.py` & `torchmetrics-0.9.3/torchmetrics/utilities/compute.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/data.py` & `torchmetrics-0.9.3/torchmetrics/utilities/data.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/distributed.py` & `torchmetrics-0.9.3/torchmetrics/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/enums.py` & `torchmetrics-0.9.3/torchmetrics/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/exceptions.py` & `torchmetrics-0.9.3/torchmetrics/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/imports.py` & `torchmetrics-0.9.3/torchmetrics/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/utilities/prints.py` & `torchmetrics-0.9.3/torchmetrics/utilities/prints.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/__init__.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/bootstrapping.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/classwise.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/classwise.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         >>> preds = torch.randn(10, 3).softmax(dim=-1)
         >>> target = torch.randint(3, (10,))
         >>> metric(preds, target)  # doctest: +NORMALIZE_WHITESPACE
         {'accuracy_horse': tensor(0.), 'accuracy_fish': tensor(0.3333), 'accuracy_dog': tensor(0.4000),
         'recall_horse': tensor(0.), 'recall_fish': tensor(0.3333), 'recall_dog': tensor(0.4000)}
     """
 
+    full_state_update: Optional[bool] = True
+
     def __init__(self, metric: Metric, labels: Optional[List[str]] = None) -> None:
         super().__init__()
         if not isinstance(metric, Metric):
             raise ValueError(f"Expected argument `metric` to be an instance of `torchmetrics.Metric` but got {metric}")
         if labels is not None and not (isinstance(labels, list) and all(isinstance(lab, str) for lab in labels)):
             raise ValueError(f"Expected argument `labels` to either be `None` or a list of strings but got {labels}")
         self.metric = metric
@@ -67,7 +69,10 @@
         return {f"{name}_{lab}": val for lab, val in zip(self.labels, x)}
 
     def update(self, *args: Any, **kwargs: Any) -> None:
         self.metric.update(*args, **kwargs)
 
     def compute(self) -> Dict[str, Tensor]:
         return self._convert(self.metric.compute())
+
+    def reset(self) -> None:
+        self.metric.reset()
```

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/minmax.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/multioutput.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/multioutput.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics/wrappers/tracker.py` & `torchmetrics-0.9.3/torchmetrics/wrappers/tracker.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics.egg-info/SOURCES.txt` & `torchmetrics-0.9.3/torchmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchmetrics-0.9.2/torchmetrics.egg-info/requires.txt` & `torchmetrics-0.9.3/torchmetrics.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,121 +3,121 @@
 packaging
 
 [:python_version < "3.8"]
 typing-extensions
 
 [all]
 pystoi
-torchvision>=0.8
 pycocotools
+torchvision>=0.8
+sphinx<5.0,>=4.0
+sphinxcontrib-fulltoc>=1.0
+sphinxcontrib-mockautodoc
+sphinx-autodoc-typehints>=1.0
 sphinx-copybutton>=0.3
-nbsphinx>=0.8
 docutils>=0.16
-sphinxcontrib-fulltoc>=1.0
+pandoc>=1.0
+nbsphinx>=0.8
+sphinx-togglebutton>=0.2
 sphinx-paramlinks>=0.5.1
-sphinx-autodoc-typehints>=1.0
-sphinx<5.0,>=4.0
 myst-parser
-sphinx-togglebutton>=0.2
-pandoc>=1.0
-sphinxcontrib-mockautodoc
-torchvision
-torch-fidelity
 lpips
+torch-fidelity
 scipy
+torchvision
 pytorch-lightning>=1.5
-mypy>=0.790
-transformers>=4.0
-pytorch_msssim
-scikit-image>0.17.1
-fast-bss-eval>=0.1.0
-rouge-score>=0.0.4
+codecov>=2.1
+check-manifest
 torch_complex
-bert_score==0.3.10
+scikit-learn<1.1.1,>1.0
 cloudpickle>=1.3
-jiwer>=2.3.0
+mir_eval>=0.6
+pytest-cov>2.10
+pytest-timeout
+scikit-image>0.17.1
+pytest==6.*
 pypesq
+transformers>=4.0
+pre-commit>=1.0
+fire
+bert_score==0.3.10
+pytorch_msssim
+psutil
 coverage>5.2
-codecov>=2.1
 huggingface-hub<0.7
-sacrebleu>=2.0.0
-pytest-cov>2.10
-psutil
-pre-commit>=1.0
+pytest-doctestplus>=0.9.0
 requests
-pytest==6.*
+rouge-score==0.0.4
+jiwer>=2.3.0
 twine>=3.2
-scikit-learn<1.1.1,>1.0
-pytest-doctestplus>=0.9.0
-pytest-timeout
+sacrebleu>=2.0.0
+fast-bss-eval>=0.1.0
 phmdoctest>=1.1.1
-check-manifest
-mir_eval>=0.6
-fire
+mypy>=0.790
 nltk>=3.6
 regex>=2021.9.24
 tqdm>=4.41.0
 
 [audio]
 pystoi
 
 [detection]
-torchvision>=0.8
 pycocotools
+torchvision>=0.8
 
 [docs]
+sphinx<5.0,>=4.0
+sphinxcontrib-fulltoc>=1.0
+sphinxcontrib-mockautodoc
+sphinx-autodoc-typehints>=1.0
 sphinx-copybutton>=0.3
-nbsphinx>=0.8
 docutils>=0.16
-sphinxcontrib-fulltoc>=1.0
+pandoc>=1.0
+nbsphinx>=0.8
+sphinx-togglebutton>=0.2
 sphinx-paramlinks>=0.5.1
-sphinx-autodoc-typehints>=1.0
-sphinx<5.0,>=4.0
 myst-parser
-sphinx-togglebutton>=0.2
-pandoc>=1.0
-sphinxcontrib-mockautodoc
 
 [image]
-torchvision
-torch-fidelity
 lpips
+torch-fidelity
 scipy
+torchvision
 
 [integrate]
 pytorch-lightning>=1.5
 
 [test]
-mypy>=0.790
-transformers>=4.0
-pytorch_msssim
-scikit-image>0.17.1
-fast-bss-eval>=0.1.0
-pycocotools
-rouge-score>=0.0.4
+codecov>=2.1
+check-manifest
 torch_complex
-bert_score==0.3.10
+scikit-learn<1.1.1,>1.0
 cloudpickle>=1.3
-jiwer>=2.3.0
+mir_eval>=0.6
+pytest-cov>2.10
+pytest-timeout
+pycocotools
+scikit-image>0.17.1
+pytest==6.*
 pypesq
+transformers>=4.0
+pre-commit>=1.0
+fire
+bert_score==0.3.10
+pytorch_msssim
+psutil
 coverage>5.2
-codecov>=2.1
 huggingface-hub<0.7
-sacrebleu>=2.0.0
-pytest-cov>2.10
-psutil
-pre-commit>=1.0
+pytest-doctestplus>=0.9.0
 requests
-pytest==6.*
+rouge-score==0.0.4
+jiwer>=2.3.0
 twine>=3.2
-scikit-learn<1.1.1,>1.0
-pytest-doctestplus>=0.9.0
-pytest-timeout
+sacrebleu>=2.0.0
+fast-bss-eval>=0.1.0
 phmdoctest>=1.1.1
-check-manifest
-mir_eval>=0.6
-fire
+mypy>=0.790
 
 [text]
 nltk>=3.6
 regex>=2021.9.24
 tqdm>=4.41.0
```

