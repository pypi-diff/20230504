# Comparing `tmp/zahner_analysis-1.0.4.tar.gz` & `tmp/zahner_analysis-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zahner_analysis-1.0.4.tar", last modified: Thu Apr 13 11:03:47 2023, max compression
+gzip compressed data, was "zahner_analysis-1.0.5.tar", last modified: Thu May  4 14:05:06 2023, max compression
```

## Comparing `zahner_analysis-1.0.4.tar` & `zahner_analysis-1.0.5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.089647 zahner_analysis-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/BasicIntroduction/
--rw-r--r--   0 runner    (1001) docker     (123)   459849 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/AnalysisScreenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)   152479 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/
--rw-r--r--   0 runner    (1001) docker     (123)   105801 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.png
--rw-r--r--   0 runner    (1001) docker     (123)   100508 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.svg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted_simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-data.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)   374829 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/
--rw-r--r--   0 runner    (1001) docker     (123)    89466 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132610 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png
--rw-r--r--   0 runner    (1001) docker     (123)    79494 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism
--rw-r--r--   0 runner    (1001) docker     (123)    45584 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-battery.ism
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/
--rw-r--r--   0 runner    (1001) docker     (123)    61065 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py
--rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.093647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.097647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.101647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.105647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/Examples/ZHIT/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/RC-R-L.isfx
--rw-r--r--   0 runner    (1001) docker     (123)   434541 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ism
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/Examples/ZHIT/drift.ism
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/jupyter
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/matplotlib
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/numpy
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/requests
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/LICENSES/scipy
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/analysis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29914 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/eis_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/analysis_tools/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/zahner_analysis/file_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/impedance_model_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/isc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/ism_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/iss_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/seqtxt_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/file_import/thales_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.113647 zahner_analysis-1.0.4/zahner_analysis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-04-13 11:03:39.000000 zahner_analysis-1.0.4/zahner_analysis/plotting/impedance_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:47.109647 zahner_analysis-1.0.4/zahner_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 11:03:47.000000 zahner_analysis-1.0.4/zahner_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.175227 zahner_analysis-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/BasicIntroduction/
+-rw-r--r--   0 runner    (1001) docker     (123)   459849 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/AnalysisScreenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   152479 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/
+-rw-r--r--   0 runner    (1001) docker     (123)   105801 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100508 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-data.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)   374829 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    89466 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132610 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79494 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism
+-rw-r--r--   0 runner    (1001) docker     (123)    45584 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-battery.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    61065 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.179227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.183227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.187227 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/Examples/ZHIT/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/RC-R-L.isfx
+-rw-r--r--   0 runner    (1001) docker     (123)   434541 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/Examples/ZHIT/drift.ism
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/jupyter
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/matplotlib
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/numpy
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/requests
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/LICENSES/scipy
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/analysis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29914 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/eis_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/analysis_tools/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/zahner_analysis/file_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/impedance_model_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/isc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/ism_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/iss_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/seqtxt_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/file_import/thales_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.195227 zahner_analysis-1.0.5/zahner_analysis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-05-04 14:04:50.000000 zahner_analysis-1.0.5/zahner_analysis/plotting/impedance_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:05:06.191228 zahner_analysis-1.0.5/zahner_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 14:05:06.000000 zahner_analysis-1.0.5/zahner_analysis.egg-info/top_level.txt
```

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/AnalysisScreenshot.png` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/AnalysisScreenshot.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.ipynb` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/BasicIntroduction.py` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/BasicIntroduction.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.png` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/bode.svg` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/bode.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_result.json` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted.isfx` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/fit_results/simulated.ism` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/fit_results/simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-data.ism` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-data.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/BasicIntroduction/rc-model.isfx` & `zahner_analysis-1.0.5/Examples/BasicIntroduction/rc-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/ComplexFitConfigurations.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode.svg` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.pdf`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_fitted.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/bode_not_fitted.png`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_result.json` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/fit_result/nyquist.jpg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-battery.ism` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-battery.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ComplexFitConfigurations/li-ion-model.isfx` & `zahner_analysis-1.0.5/Examples/ComplexFitConfigurations/li-ion-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/ImpedanceVsVoltageSeriesFit.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/RvsU.svg`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/diode-ac-model.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/000_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/025_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/050_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/075_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/100_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/125_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/150_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/175_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/200_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/225_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/250_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/275_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_result.json`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fit_samples.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/fitted_spectras/300_mvdc/fitted_simulated.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/000_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/025_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/050_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/075_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/100_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/125_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/150_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/175_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/200_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/225_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/250_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/275_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism` & `zahner_analysis-1.0.5/Examples/ImpedanceVsVoltageSeriesFit/measured_spectras/300_mvdc.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ZHIT/RC-R-L.isfx` & `zahner_analysis-1.0.5/Examples/ZHIT/RC-R-L.isfx`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ipynb` & `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ipynb`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.ism` & `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ZHIT/ZHIT.py` & `zahner_analysis-1.0.5/Examples/ZHIT/ZHIT.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/Examples/ZHIT/drift.ism` & `zahner_analysis-1.0.5/Examples/ZHIT/drift.ism`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSE` & `zahner_analysis-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSES/jupyter` & `zahner_analysis-1.0.5/LICENSES/jupyter`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSES/matplotlib` & `zahner_analysis-1.0.5/LICENSES/matplotlib`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSES/numpy` & `zahner_analysis-1.0.5/LICENSES/numpy`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSES/requests` & `zahner_analysis-1.0.5/LICENSES/requests`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/LICENSES/scipy` & `zahner_analysis-1.0.5/LICENSES/scipy`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/PKG-INFO` & `zahner_analysis-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zahner_analysis
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for the analysis of electrochemical impedance spectra.
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
         Copyright (c) 2022 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -141,15 +141,15 @@
 ## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
 
 * Fit the model to the data
 * Load the data and the model
 * Perform ZHIT evaluation
 * Plot the result
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
```

### Comparing `zahner_analysis-1.0.4/README.md` & `zahner_analysis-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 ## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
 
 * Fit the model to the data
 * Load the data and the model
 * Perform ZHIT evaluation
 * Plot the result
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
```

### Comparing `zahner_analysis-1.0.4/openapi.yaml` & `zahner_analysis-1.0.5/openapi.yaml`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/pyproject.toml` & `zahner_analysis-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/analysis_tools/analysis_connection.py` & `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/analysis_connection.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/analysis_tools/eis_fitting.py` & `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/eis_fitting.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/analysis_tools/error.py` & `zahner_analysis-1.0.5/zahner_analysis/analysis_tools/error.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/file_import/impedance_model_import.py` & `zahner_analysis-1.0.5/zahner_analysis/file_import/impedance_model_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/file_import/isc_import.py` & `zahner_analysis-1.0.5/zahner_analysis/file_import/isc_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/file_import/iss_import.py` & `zahner_analysis-1.0.5/zahner_analysis/file_import/iss_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/file_import/seqtxt_import.py` & `zahner_analysis-1.0.5/zahner_analysis/file_import/seqtxt_import.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis/file_import/thales_file_utils.py` & `zahner_analysis-1.0.5/zahner_analysis/file_import/thales_file_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     return np.ndarray(shape=(length,), dtype=">f8", buffer=file.read(8 * length))
 
 
 def readI2FromFile(file):
     return int.from_bytes(file.read(2), "big", signed=True)
 
 
+def peekI2FromFile(file):
+    return int.from_bytes(file.peek(2), "big", signed=True)
+
+
 def readI2ArrayFromFile(file, length):
     return np.ndarray(shape=(length,), dtype=">i2", buffer=file.read(2 * length))
 
 
 def readI6FromFile(file):
     return int.from_bytes(file.read(6), "big", signed=True)
```

### Comparing `zahner_analysis-1.0.4/zahner_analysis/plotting/impedance_plot.py` & `zahner_analysis-1.0.5/zahner_analysis/plotting/impedance_plot.py`

 * *Files identical despite different names*

### Comparing `zahner_analysis-1.0.4/zahner_analysis.egg-info/PKG-INFO` & `zahner_analysis-1.0.5/zahner_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zahner-analysis
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python package for the analysis of electrochemical impedance spectra.
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
         Copyright (c) 2022 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -141,15 +141,15 @@
 ## [ZHIT.ipynb](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/blob/main/Examples/ZHIT/ZHIT.ipynb)
 
 * Fit the model to the data
 * Load the data and the model
 * Perform ZHIT evaluation
 * Plot the result
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an [mail](mailto:support@zahner.de?subject=Zahner-Analysis-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Analysis-Python](https://github.com/Zahner-elektrik/Zahner-Analysis-Python/issues) repository.  
 If you already found a solution to your problem, **we would love to review your pull request**!
```

### Comparing `zahner_analysis-1.0.4/zahner_analysis.egg-info/SOURCES.txt` & `zahner_analysis-1.0.5/zahner_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

