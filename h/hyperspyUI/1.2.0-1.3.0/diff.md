# Comparing `tmp/hyperspyUI-1.2.0.tar.gz` & `tmp/hyperspyUI-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperspyUI-1.2.0.tar", last modified: Thu Mar 16 18:15:46 2023, max compression
+gzip compressed data, was "hyperspyUI-1.3.0.tar", last modified: Thu May  4 17:18:15 2023, max compression
```

## Comparing `hyperspyUI-1.2.0.tar` & `hyperspyUI-1.3.0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.599427 hyperspyUI-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/DEV-README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-16 18:15:46.599427 hyperspyUI-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.579427 hyperspyUI-1.2.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/bin/hyperspyui_reg_linux_extensions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/bin/win_bundle_install.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.583427 hyperspyUI-1.2.0/hyperspyUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 18:15:46.000000 hyperspyUI-1.2.0/hyperspyUI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.583427 hyperspyUI-1.2.0/hyperspyui/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.587427 hyperspyUI-1.2.0/hyperspyui/_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/figuretool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/gaussiantool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/hometool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/linetool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/multiselectiontool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/pointertool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/selectiontool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/signalfiguretool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/_tools/zoompan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/actionable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/advancedaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/bindinglist.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/desktop_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/desktop_integration_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/desktop_integration_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/hooksignal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/hooktraitsui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.591426 hyperspyUI-1.2.0/hyperspyui/images/
--rw-r--r--   0 runner    (1001) docker     (123)   178565 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/3d.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/Hypercube.svg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/align2d.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/align_horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/align_manual.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/align_vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/align_zero_loss.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/analysis.svg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/attributions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/bss.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/candlestick.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/chart.svg
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/chart_column.svg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/chart_horz.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/chart_stacked_column.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/close_window.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/close_windows.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/divide.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/fft.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/fft_capital_f.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/fourier_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/gaussian.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/gaussian_bare.svg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/hyperspy.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/hyperspy_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.595426 hyperspyUI-1.2.0/hyperspyui/images/icon/
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy.ico
--rw-r--r--   0 runner    (1001) docker     (123)    23546 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy128.png
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy16.png
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy22.png
--rw-r--r--   0 runner    (1001) docker     (123)    55171 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy256.png
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy48.png
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy64.png
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/ifft.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/infft.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/intersection.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/line_plot.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/live_fft.png
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/live_fft.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/magnifier.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/max.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/mean.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/min.svg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/mirror.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/move.svg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/move2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/multiply.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/new_file.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/nfft.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/open.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/panzoom.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/panzoom2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/pca.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/periodic_table.svg
--rw-r--r--   0 runner    (1001) docker     (123)    66092 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/periodic_table2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/photo_contrast.svg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/photo_contrast2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/picker.svg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/pointer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/power_law.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/rebin.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/regression.svg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/renko.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/rotate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/ruler.svg
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/save.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/scatter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/segmentation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/slider.svg
--rw-r--r--   0 runner    (1001) docker     (123)    65768 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/splash.png
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/spline_chart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/stddev.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/subtract.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/sum.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/t_over_lambda.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/testing_icon_coloring.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/text_field.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/variance.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/visibility_off.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/visibility_off2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/visibility_on.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/visibility_on2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/zero_loss.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/images/zoom.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.595426 hyperspyUI-1.2.0/hyperspyui/ipython_profile/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/ipython_profile/ipython_embedded_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/mainwindowbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/mainwindowhyperspy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/mainwindowutillayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/mdi_mpl_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/modelwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugincreator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/pluginmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.595426 hyperspyUI-1.2.0/hyperspyui/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/alignzlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/axesconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/axesorderwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/basicsignal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/basicspectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/cmappicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/croptool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/dataastext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/dmannotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/eelsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/gaussianfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/gitgetter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/imagerotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/linemeasure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/metadataeditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/mirrorplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/moviesaver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/mva.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/plotutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/rebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/recorderwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/tightlayout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/plugins/virtual_aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/signalwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/singleapplication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/smartcolorsvgiconengine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.595426 hyperspyUI-1.2.0/hyperspyui/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/single_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tests/test_single_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/uiprogressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 18:15:45.000000 hyperspyUI-1.2.0/hyperspyui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:46.599427 hyperspyUI-1.2.0/hyperspyui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/_editor_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/axespicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/colorpicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/consolewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    17230 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/dataviewwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/editorwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/elementpicker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/extendedqwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/flowlayout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/periodictable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/pickxsignals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/pluginmanagerwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/settingsdialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/signallist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/stringinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/hyperspyui/widgets/traitswidget.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 18:15:46.599427 hyperspyUI-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-03-16 18:15:36.000000 hyperspyUI-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.828379 hyperspyUI-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/DEV-README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-04 17:18:15.828379 hyperspyUI-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.808379 hyperspyUI-1.3.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/bin/hyperspyui_reg_linux_extensions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/bin/win_bundle_install.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.808379 hyperspyUI-1.3.0/hyperspyUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 17:18:15.000000 hyperspyUI-1.3.0/hyperspyUI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.812379 hyperspyUI-1.3.0/hyperspyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.812379 hyperspyUI-1.3.0/hyperspyui/_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/figuretool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/gaussiantool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/hometool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/linetool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/multiselectiontool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/pointertool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/selectiontool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/signalfiguretool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/_tools/zoompan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/actionable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/advancedaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/bindinglist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/desktop_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/desktop_integration_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/desktop_integration_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/hooksignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/hooktraitsui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.820379 hyperspyUI-1.3.0/hyperspyui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   178565 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/3d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/Hypercube.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/align2d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/align_horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/align_manual.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/align_vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/align_zero_loss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/analysis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/attributions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/bss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/candlestick.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/chart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/chart_column.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/chart_horz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/chart_stacked_column.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/close_window.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/close_windows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/divide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/fft.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/fft_capital_f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/fourier_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/gaussian.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/gaussian_bare.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/hyperspy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/hyperspy_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.820379 hyperspyUI-1.3.0/hyperspyui/images/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    23546 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy22.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55171 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/ifft.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/infft.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/intersection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/line_plot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/live_fft.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/live_fft.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/magnifier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/max.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/mean.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/mirror.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/move.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/move2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/multiply.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/new_file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/nfft.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/open.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/panzoom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/panzoom2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/pca.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/periodic_table.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    66092 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/periodic_table2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/photo_contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/photo_contrast2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/picker.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/pointer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/power_law.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/rebin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/regression.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/renko.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/rotate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/ruler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/scatter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/segmentation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    65768 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/splash.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/spline_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/stddev.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/subtract.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/sum.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/t_over_lambda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/testing_icon_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/text_field.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/variance.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/visibility_off.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/visibility_off2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/visibility_on.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/visibility_on2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/zero_loss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/images/zoom.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.820379 hyperspyUI-1.3.0/hyperspyui/ipython_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/ipython_profile/ipython_embedded_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/mainwindowbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/mainwindowhyperspy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/mainwindowutillayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/mdi_mpl_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/modelwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugincreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/pluginmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.824380 hyperspyUI-1.3.0/hyperspyui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/alignzlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/axesconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/axesorderwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/basicsignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/basicspectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/cmappicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/croptool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/dataastext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/dmannotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/eelsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/gaussianfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/gitgetter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/imagerotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/linemeasure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/metadataeditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/mirrorplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/moviesaver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/mva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/plotutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/rebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/recorderwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/tightlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/plugins/virtual_aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/signalwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/singleapplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/smartcolorsvgiconengine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.824380 hyperspyUI-1.3.0/hyperspyui/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/single_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tests/test_single_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/uiprogressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 17:18:10.000000 hyperspyUI-1.3.0/hyperspyui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:18:15.828379 hyperspyUI-1.3.0/hyperspyui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/_editor_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/axespicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/colorpicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/consolewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17230 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/dataviewwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/editorwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14464 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/elementpicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/extendedqwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/flowlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/periodictable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/pickxsignals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/pluginmanagerwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/settingsdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/signallist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/stringinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/hyperspyui/widgets/traitswidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:18:15.828379 hyperspyUI-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-04 17:17:59.000000 hyperspyUI-1.3.0/setup.py
```

### Comparing `hyperspyUI-1.2.0/CHANGES.rst` & `hyperspyUI-1.3.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 
 Changelog
 *********
 
+v1.3.0 (2023-05-04)
++++++++++++++++++++
+- Update release workflow to remove deprecated github actions and use pypi API token instead of user/password (`#211 <https://github.com/hyperspy/hyperspyUI/pull/211>`_)
+- Fix dependabot error when parsing github workflow  (`#212 <https://github.com/hyperspy/hyperspyUI/pull/212>`_)
+- Fix import marker hyperspy 2.0  (`#216 <https://github.com/hyperspy/hyperspyUI/pull/216>`_)
+- Add explicit support for python 3.11 (`#218 <https://github.com/hyperspy/hyperspyUI/pull/218>`_)
+- Bump version of pyqode dependencies to support pyflakes >=2.5 (`#218 <https://github.com/hyperspy/hyperspyUI/pull/218>`_)
+
+
 v1.2.0 (2023-03-16)
 +++++++++++++++++++
 - Pin third party action and fix tests and documentation GitHub workflow (`#206 <https://github.com/hyperspy/hyperspyUI/pull/206>`_)
 - Pin pyflakes to 2.4 to keep pyqode.python working (`#206 <https://github.com/hyperspy/hyperspyUI/pull/206>`_)
 - Add support for HyperSpy 2.0 (`#207 <https://github.com/hyperspy/hyperspyUI/pull/207>`_)
 - Improve code quality using GitHub CodeQL and fix bugs (`#208 <https://github.com/hyperspy/hyperspyUI/pull/208>`_)
```

### Comparing `hyperspyUI-1.2.0/COPYING.txt` & `hyperspyUI-1.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/DEV-README.txt` & `hyperspyUI-1.3.0/DEV-README.txt`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/PKG-INFO` & `hyperspyUI-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperspyUI
-Version: 1.2.0
+Version: 1.3.0
 Summary: Hyperspy Graphical User Interface
 Home-page: http://github.com/hyperspy/hyperspyUI/
 Author: Vidar Tonaas Fauske
 Author-email: vidartf+hyperspyui@gmail.com
 License: GPLv3
-Description: HyperSpyUI
-        ==========
-        
-        |pypi_version|_ |anaconda_cloud|_ |tests|_ |python_version|_
-        
-        .. |pypi_version| image:: https://img.shields.io/pypi/v/hyperspyui.svg
-        .. _pypi_version: https://pypi.python.org/pypi/hyperspyui
-        
-        .. |anaconda_cloud| image:: https://anaconda.org/conda-forge/hyperspyui/badges/version.svg
-        .. _anaconda_cloud: https://anaconda.org/conda-forge/hyperspyui
-        
-        .. |tests| image:: https://github.com/hyperspy/hyperspyUI/workflows/Tests/badge.svg
-        .. _tests: https://github.com/hyperspy/hyperspyUI/actions
-        
-        .. |python_version| image:: https://img.shields.io/pypi/pyversions/hyperspyui.svg?style=flat
-        .. _python_version: https://pypi.python.org/pypi/hyperspyui
-        
-        HyperSpyUI tries to bring a streamlined user interface to the powerful
-        multi-dimensional analysis capabilities of HyperSpy_. HyperSpy is an open
-        source Python library which provides tools to facilitate data analysis of
-        multidimensional datasets.
-        
-        HyperSpy aims at making it easy and natural to apply analytical procedures
-        that operate on an individual signal to multidimensional arrays, as well as
-        providing easy access to analytical tools that exploit the multidimensionality
-        of the dataset.
-        
-        While the UI tries to create a simple and intuitive interface to HyperSpy, it
-        still retains the raw power of HyperSpy via the UI’s built in IPython console,
-        which runs on the same Python kernel as the UI.
-        
-        Documentation
-        =============
-        
-        For an introduction to HyperSpyUI, see the documentation_.
-        
-        
-        Installation
-        ============
-        There are several ways to install HyperSpyUI. The application itself is rather
-        simple to install, but its dependencies can be a bit more tricky. From version
-        1.1, HyperSpyUI supports both PyQt4 and PyQt5.
-        
-        HyperSpy Bundle Installer
-        -------------------------
-        The quickest way to get set up is to download and install
-        the `HyperSpy bundle`_ installer, which includes HyperSpyUI.
-        
-        .. _HyperSpy bundle: https://github.com/hyperspy/hyperspy-bundle
-        
-        Anaconda/Miniconda/Miniforge
-        ----------------------------
-        
-        Download and install the `Miniforge`_ (`Miniconda`_ or `Anaconda`_) distribution
-        and run the following command in the anaconda prompt:
-        
-        .. code-block:: bash
-        
-            conda install -c conda-forge hyperspyui
-        
-        .. _Miniforge: https://github.com/conda-forge/miniforge#download
-        .. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-        .. _Anaconda: https://www.anaconda.com/products/individual
-        
-        Installation via pip
-        --------------------
-        
-        HyperSpyUI can be intall from pip. Depending on your python distribution you may
-        need to have C compiler on your system to install some of the dependencies.
-        
-        .. code-block:: bash
-        
-            pip install hyperspyui
-        
-        If pyqt is not installed, run:
-        
-        .. code-block:: bash
-        
-            pip install PyQt5 PyQtWebEngine
-        
-        
-        Run HyperSpyUI
-        ==============
-        
-        After installation, you can run HyperSpyUI from the command prompt with:
-        
-        .. code-block:: bash
-        
-            hyperspyui
-        
-        or
-        
-        .. code-block:: bash
-        
-            python -m hyperspyui
-        
-        
-        For further information, see the full documentation_.
-        
-        .. _HyperSpy: https://hyperspy.org
-        .. _documentation: https://hyperspy.org/hyperspyUI/
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -124,7 +22,110 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: build-doc
+License-File: COPYING.txt
+
+HyperSpyUI
+==========
+
+|pypi_version|_ |anaconda_cloud|_ |tests|_ |python_version|_
+
+.. |pypi_version| image:: https://img.shields.io/pypi/v/hyperspyui.svg
+.. _pypi_version: https://pypi.python.org/pypi/hyperspyui
+
+.. |anaconda_cloud| image:: https://anaconda.org/conda-forge/hyperspyui/badges/version.svg
+.. _anaconda_cloud: https://anaconda.org/conda-forge/hyperspyui
+
+.. |tests| image:: https://github.com/hyperspy/hyperspyUI/workflows/Tests/badge.svg
+.. _tests: https://github.com/hyperspy/hyperspyUI/actions
+
+.. |python_version| image:: https://img.shields.io/pypi/pyversions/hyperspyui.svg?style=flat
+.. _python_version: https://pypi.python.org/pypi/hyperspyui
+
+HyperSpyUI tries to bring a streamlined user interface to the powerful
+multi-dimensional analysis capabilities of HyperSpy_. HyperSpy is an open
+source Python library which provides tools to facilitate data analysis of
+multidimensional datasets.
+
+HyperSpy aims at making it easy and natural to apply analytical procedures
+that operate on an individual signal to multidimensional arrays, as well as
+providing easy access to analytical tools that exploit the multidimensionality
+of the dataset.
+
+While the UI tries to create a simple and intuitive interface to HyperSpy, it
+still retains the raw power of HyperSpy via the UI’s built in IPython console,
+which runs on the same Python kernel as the UI.
+
+Documentation
+=============
+
+For an introduction to HyperSpyUI, see the documentation_.
+
+
+Installation
+============
+There are several ways to install HyperSpyUI. The application itself is rather
+simple to install, but its dependencies can be a bit more tricky. From version
+1.1, HyperSpyUI supports both PyQt4 and PyQt5.
+
+HyperSpy Bundle Installer
+-------------------------
+The quickest way to get set up is to download and install
+the `HyperSpy bundle`_ installer, which includes HyperSpyUI.
+
+.. _HyperSpy bundle: https://github.com/hyperspy/hyperspy-bundle
+
+Anaconda/Miniconda/Miniforge
+----------------------------
+
+Download and install the `Miniforge`_ (`Miniconda`_ or `Anaconda`_) distribution
+and run the following command in the anaconda prompt:
+
+.. code-block:: bash
+
+    conda install -c conda-forge hyperspyui
+
+.. _Miniforge: https://github.com/conda-forge/miniforge#download
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _Anaconda: https://www.anaconda.com/products/individual
+
+Installation via pip
+--------------------
+
+HyperSpyUI can be intall from pip. Depending on your python distribution you may
+need to have C compiler on your system to install some of the dependencies.
+
+.. code-block:: bash
+
+    pip install hyperspyui
+
+If pyqt is not installed, run:
+
+.. code-block:: bash
+
+    pip install PyQt5 PyQtWebEngine
+
+
+Run HyperSpyUI
+==============
+
+After installation, you can run HyperSpyUI from the command prompt with:
+
+.. code-block:: bash
+
+    hyperspyui
+
+or
+
+.. code-block:: bash
+
+    python -m hyperspyui
+
+
+For further information, see the full documentation_.
+
+.. _HyperSpy: https://hyperspy.org
+.. _documentation: https://hyperspy.org/hyperspyUI/
```

### Comparing `hyperspyUI-1.2.0/README.rst` & `hyperspyUI-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/bin/hyperspyui_reg_linux_extensions.sh` & `hyperspyUI-1.3.0/bin/hyperspyui_reg_linux_extensions.sh`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyUI.egg-info/PKG-INFO` & `hyperspyUI-1.3.0/hyperspyUI.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperspyUI
-Version: 1.2.0
+Version: 1.3.0
 Summary: Hyperspy Graphical User Interface
 Home-page: http://github.com/hyperspy/hyperspyUI/
 Author: Vidar Tonaas Fauske
 Author-email: vidartf+hyperspyui@gmail.com
 License: GPLv3
-Description: HyperSpyUI
-        ==========
-        
-        |pypi_version|_ |anaconda_cloud|_ |tests|_ |python_version|_
-        
-        .. |pypi_version| image:: https://img.shields.io/pypi/v/hyperspyui.svg
-        .. _pypi_version: https://pypi.python.org/pypi/hyperspyui
-        
-        .. |anaconda_cloud| image:: https://anaconda.org/conda-forge/hyperspyui/badges/version.svg
-        .. _anaconda_cloud: https://anaconda.org/conda-forge/hyperspyui
-        
-        .. |tests| image:: https://github.com/hyperspy/hyperspyUI/workflows/Tests/badge.svg
-        .. _tests: https://github.com/hyperspy/hyperspyUI/actions
-        
-        .. |python_version| image:: https://img.shields.io/pypi/pyversions/hyperspyui.svg?style=flat
-        .. _python_version: https://pypi.python.org/pypi/hyperspyui
-        
-        HyperSpyUI tries to bring a streamlined user interface to the powerful
-        multi-dimensional analysis capabilities of HyperSpy_. HyperSpy is an open
-        source Python library which provides tools to facilitate data analysis of
-        multidimensional datasets.
-        
-        HyperSpy aims at making it easy and natural to apply analytical procedures
-        that operate on an individual signal to multidimensional arrays, as well as
-        providing easy access to analytical tools that exploit the multidimensionality
-        of the dataset.
-        
-        While the UI tries to create a simple and intuitive interface to HyperSpy, it
-        still retains the raw power of HyperSpy via the UI’s built in IPython console,
-        which runs on the same Python kernel as the UI.
-        
-        Documentation
-        =============
-        
-        For an introduction to HyperSpyUI, see the documentation_.
-        
-        
-        Installation
-        ============
-        There are several ways to install HyperSpyUI. The application itself is rather
-        simple to install, but its dependencies can be a bit more tricky. From version
-        1.1, HyperSpyUI supports both PyQt4 and PyQt5.
-        
-        HyperSpy Bundle Installer
-        -------------------------
-        The quickest way to get set up is to download and install
-        the `HyperSpy bundle`_ installer, which includes HyperSpyUI.
-        
-        .. _HyperSpy bundle: https://github.com/hyperspy/hyperspy-bundle
-        
-        Anaconda/Miniconda/Miniforge
-        ----------------------------
-        
-        Download and install the `Miniforge`_ (`Miniconda`_ or `Anaconda`_) distribution
-        and run the following command in the anaconda prompt:
-        
-        .. code-block:: bash
-        
-            conda install -c conda-forge hyperspyui
-        
-        .. _Miniforge: https://github.com/conda-forge/miniforge#download
-        .. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-        .. _Anaconda: https://www.anaconda.com/products/individual
-        
-        Installation via pip
-        --------------------
-        
-        HyperSpyUI can be intall from pip. Depending on your python distribution you may
-        need to have C compiler on your system to install some of the dependencies.
-        
-        .. code-block:: bash
-        
-            pip install hyperspyui
-        
-        If pyqt is not installed, run:
-        
-        .. code-block:: bash
-        
-            pip install PyQt5 PyQtWebEngine
-        
-        
-        Run HyperSpyUI
-        ==============
-        
-        After installation, you can run HyperSpyUI from the command prompt with:
-        
-        .. code-block:: bash
-        
-            hyperspyui
-        
-        or
-        
-        .. code-block:: bash
-        
-            python -m hyperspyui
-        
-        
-        For further information, see the full documentation_.
-        
-        .. _HyperSpy: https://hyperspy.org
-        .. _documentation: https://hyperspy.org/hyperspyUI/
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -124,7 +22,110 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: build-doc
+License-File: COPYING.txt
+
+HyperSpyUI
+==========
+
+|pypi_version|_ |anaconda_cloud|_ |tests|_ |python_version|_
+
+.. |pypi_version| image:: https://img.shields.io/pypi/v/hyperspyui.svg
+.. _pypi_version: https://pypi.python.org/pypi/hyperspyui
+
+.. |anaconda_cloud| image:: https://anaconda.org/conda-forge/hyperspyui/badges/version.svg
+.. _anaconda_cloud: https://anaconda.org/conda-forge/hyperspyui
+
+.. |tests| image:: https://github.com/hyperspy/hyperspyUI/workflows/Tests/badge.svg
+.. _tests: https://github.com/hyperspy/hyperspyUI/actions
+
+.. |python_version| image:: https://img.shields.io/pypi/pyversions/hyperspyui.svg?style=flat
+.. _python_version: https://pypi.python.org/pypi/hyperspyui
+
+HyperSpyUI tries to bring a streamlined user interface to the powerful
+multi-dimensional analysis capabilities of HyperSpy_. HyperSpy is an open
+source Python library which provides tools to facilitate data analysis of
+multidimensional datasets.
+
+HyperSpy aims at making it easy and natural to apply analytical procedures
+that operate on an individual signal to multidimensional arrays, as well as
+providing easy access to analytical tools that exploit the multidimensionality
+of the dataset.
+
+While the UI tries to create a simple and intuitive interface to HyperSpy, it
+still retains the raw power of HyperSpy via the UI’s built in IPython console,
+which runs on the same Python kernel as the UI.
+
+Documentation
+=============
+
+For an introduction to HyperSpyUI, see the documentation_.
+
+
+Installation
+============
+There are several ways to install HyperSpyUI. The application itself is rather
+simple to install, but its dependencies can be a bit more tricky. From version
+1.1, HyperSpyUI supports both PyQt4 and PyQt5.
+
+HyperSpy Bundle Installer
+-------------------------
+The quickest way to get set up is to download and install
+the `HyperSpy bundle`_ installer, which includes HyperSpyUI.
+
+.. _HyperSpy bundle: https://github.com/hyperspy/hyperspy-bundle
+
+Anaconda/Miniconda/Miniforge
+----------------------------
+
+Download and install the `Miniforge`_ (`Miniconda`_ or `Anaconda`_) distribution
+and run the following command in the anaconda prompt:
+
+.. code-block:: bash
+
+    conda install -c conda-forge hyperspyui
+
+.. _Miniforge: https://github.com/conda-forge/miniforge#download
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _Anaconda: https://www.anaconda.com/products/individual
+
+Installation via pip
+--------------------
+
+HyperSpyUI can be intall from pip. Depending on your python distribution you may
+need to have C compiler on your system to install some of the dependencies.
+
+.. code-block:: bash
+
+    pip install hyperspyui
+
+If pyqt is not installed, run:
+
+.. code-block:: bash
+
+    pip install PyQt5 PyQtWebEngine
+
+
+Run HyperSpyUI
+==============
+
+After installation, you can run HyperSpyUI from the command prompt with:
+
+.. code-block:: bash
+
+    hyperspyui
+
+or
+
+.. code-block:: bash
+
+    python -m hyperspyui
+
+
+For further information, see the full documentation_.
+
+.. _HyperSpy: https://hyperspy.org
+.. _documentation: https://hyperspy.org/hyperspyUI/
```

### Comparing `hyperspyUI-1.2.0/hyperspyUI.egg-info/SOURCES.txt` & `hyperspyUI-1.3.0/hyperspyUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/__init__.py` & `hyperspyUI-1.3.0/hyperspyui/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/__main__.py` & `hyperspyUI-1.3.0/hyperspyui/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_elements.py` & `hyperspyUI-1.3.0/hyperspyui/_elements.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/__init__.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/figuretool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/figuretool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/gaussiantool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/gaussiantool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/hometool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/hometool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/linetool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/linetool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/multiselectiontool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/multiselectiontool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/pointertool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/pointertool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/selectiontool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/selectiontool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/signalfiguretool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/signalfiguretool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/tool.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/tool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/_tools/zoompan.py` & `hyperspyUI-1.3.0/hyperspyui/_tools/zoompan.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/actionable.py` & `hyperspyUI-1.3.0/hyperspyui/actionable.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/advancedaction.py` & `hyperspyUI-1.3.0/hyperspyui/advancedaction.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/bindinglist.py` & `hyperspyUI-1.3.0/hyperspyui/bindinglist.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/desktop_integration.py` & `hyperspyUI-1.3.0/hyperspyui/desktop_integration.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/desktop_integration_linux.py` & `hyperspyUI-1.3.0/hyperspyui/desktop_integration_linux.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/desktop_integration_windows.py` & `hyperspyUI-1.3.0/hyperspyui/desktop_integration_windows.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/exceptions.py` & `hyperspyUI-1.3.0/hyperspyui/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/hooksignal.py` & `hyperspyUI-1.3.0/hyperspyui/hooksignal.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/hooktraitsui.py` & `hyperspyUI-1.3.0/hyperspyui/hooktraitsui.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/3d.svg` & `hyperspyUI-1.3.0/hyperspyui/images/3d.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/Hypercube.svg` & `hyperspyUI-1.3.0/hyperspyui/images/Hypercube.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/add.svg` & `hyperspyUI-1.3.0/hyperspyui/images/add.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/align2d.svg` & `hyperspyUI-1.3.0/hyperspyui/images/align2d.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/align_horizontal.svg` & `hyperspyUI-1.3.0/hyperspyui/images/align_horizontal.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/align_manual.svg` & `hyperspyUI-1.3.0/hyperspyui/images/align_manual.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/align_vertical.svg` & `hyperspyUI-1.3.0/hyperspyui/images/align_vertical.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/align_zero_loss.svg` & `hyperspyUI-1.3.0/hyperspyui/images/align_zero_loss.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/analysis.svg` & `hyperspyUI-1.3.0/hyperspyui/images/analysis.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/attributions.txt` & `hyperspyUI-1.3.0/hyperspyui/images/attributions.txt`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/bss.svg` & `hyperspyUI-1.3.0/hyperspyui/images/bss.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/candlestick.svg` & `hyperspyUI-1.3.0/hyperspyui/images/candlestick.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/chart.svg` & `hyperspyUI-1.3.0/hyperspyui/images/chart.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/chart_column.svg` & `hyperspyUI-1.3.0/hyperspyui/images/chart_column.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/chart_horz.svg` & `hyperspyUI-1.3.0/hyperspyui/images/chart_horz.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/chart_stacked_column.svg` & `hyperspyUI-1.3.0/hyperspyui/images/chart_stacked_column.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/close.svg` & `hyperspyUI-1.3.0/hyperspyui/images/close.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/close_window.svg` & `hyperspyUI-1.3.0/hyperspyui/images/close_window.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/close_windows.svg` & `hyperspyUI-1.3.0/hyperspyui/images/close_windows.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/console.svg` & `hyperspyUI-1.3.0/hyperspyui/images/console.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/crop.svg` & `hyperspyUI-1.3.0/hyperspyui/images/crop.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/divide.svg` & `hyperspyUI-1.3.0/hyperspyui/images/divide.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/download.svg` & `hyperspyUI-1.3.0/hyperspyui/images/download.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/fft.svg` & `hyperspyUI-1.3.0/hyperspyui/images/fft.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/fft_capital_f.svg` & `hyperspyUI-1.3.0/hyperspyui/images/fft_capital_f.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/fourier_ratio.svg` & `hyperspyUI-1.3.0/hyperspyui/images/fourier_ratio.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/gaussian.svg` & `hyperspyUI-1.3.0/hyperspyui/images/gaussian.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/gaussian_bare.svg` & `hyperspyUI-1.3.0/hyperspyui/images/gaussian_bare.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/home.svg` & `hyperspyUI-1.3.0/hyperspyui/images/home.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/hyperspy.svg` & `hyperspyUI-1.3.0/hyperspyui/images/hyperspy.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/hyperspy_logo.png` & `hyperspyUI-1.3.0/hyperspyui/images/hyperspy_logo.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy.ico` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy.ico`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy128.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy128.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy16.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy16.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy22.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy22.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy256.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy256.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy32.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy32.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy48.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy48.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/icon/hyperspy64.png` & `hyperspyUI-1.3.0/hyperspyui/images/icon/hyperspy64.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/ifft.svg` & `hyperspyUI-1.3.0/hyperspyui/images/ifft.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/infft.svg` & `hyperspyUI-1.3.0/hyperspyui/images/infft.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/intersection.svg` & `hyperspyUI-1.3.0/hyperspyui/images/intersection.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/line_plot.svg` & `hyperspyUI-1.3.0/hyperspyui/images/line_plot.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/live_fft.png` & `hyperspyUI-1.3.0/hyperspyui/images/live_fft.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/live_fft.svg` & `hyperspyUI-1.3.0/hyperspyui/images/live_fft.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/magnifier.svg` & `hyperspyUI-1.3.0/hyperspyui/images/magnifier.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/max.svg` & `hyperspyUI-1.3.0/hyperspyui/images/max.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/mean.svg` & `hyperspyUI-1.3.0/hyperspyui/images/mean.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/min.svg` & `hyperspyUI-1.3.0/hyperspyui/images/min.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/mirror.svg` & `hyperspyUI-1.3.0/hyperspyui/images/mirror.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/move.svg` & `hyperspyUI-1.3.0/hyperspyui/images/move.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/move2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/move2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/multiply.svg` & `hyperspyUI-1.3.0/hyperspyui/images/multiply.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/new_file.svg` & `hyperspyUI-1.3.0/hyperspyui/images/new_file.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/nfft.svg` & `hyperspyUI-1.3.0/hyperspyui/images/nfft.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/open.svg` & `hyperspyUI-1.3.0/hyperspyui/images/open.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/panzoom.svg` & `hyperspyUI-1.3.0/hyperspyui/images/panzoom.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/panzoom2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/panzoom2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/pca.svg` & `hyperspyUI-1.3.0/hyperspyui/images/pca.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/periodic_table.svg` & `hyperspyUI-1.3.0/hyperspyui/images/periodic_table.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/periodic_table2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/periodic_table2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/photo_contrast.svg` & `hyperspyUI-1.3.0/hyperspyui/images/photo_contrast.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/photo_contrast2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/photo_contrast2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/picker.svg` & `hyperspyUI-1.3.0/hyperspyui/images/picker.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/pointer.svg` & `hyperspyUI-1.3.0/hyperspyui/images/pointer.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/power_law.svg` & `hyperspyUI-1.3.0/hyperspyui/images/power_law.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/rebin.svg` & `hyperspyUI-1.3.0/hyperspyui/images/rebin.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/regression.svg` & `hyperspyUI-1.3.0/hyperspyui/images/regression.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/renko.svg` & `hyperspyUI-1.3.0/hyperspyui/images/renko.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/rotate.svg` & `hyperspyUI-1.3.0/hyperspyui/images/rotate.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/ruler.svg` & `hyperspyUI-1.3.0/hyperspyui/images/ruler.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/save.svg` & `hyperspyUI-1.3.0/hyperspyui/images/save.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/scatter.svg` & `hyperspyUI-1.3.0/hyperspyui/images/scatter.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/segmentation.svg` & `hyperspyUI-1.3.0/hyperspyui/images/segmentation.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/slider.svg` & `hyperspyUI-1.3.0/hyperspyui/images/slider.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/splash.png` & `hyperspyUI-1.3.0/hyperspyui/images/splash.png`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/spline_chart.svg` & `hyperspyUI-1.3.0/hyperspyui/images/spline_chart.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/stddev.svg` & `hyperspyUI-1.3.0/hyperspyui/images/stddev.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/subtract.svg` & `hyperspyUI-1.3.0/hyperspyui/images/subtract.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/sum.svg` & `hyperspyUI-1.3.0/hyperspyui/images/sum.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/t_over_lambda.svg` & `hyperspyUI-1.3.0/hyperspyui/images/t_over_lambda.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/temperature.svg` & `hyperspyUI-1.3.0/hyperspyui/images/temperature.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/testing_icon_coloring.py` & `hyperspyUI-1.3.0/hyperspyui/images/testing_icon_coloring.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/text_field.svg` & `hyperspyUI-1.3.0/hyperspyui/images/text_field.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/variance.svg` & `hyperspyUI-1.3.0/hyperspyui/images/variance.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/video.svg` & `hyperspyUI-1.3.0/hyperspyui/images/video.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/visibility_off.svg` & `hyperspyUI-1.3.0/hyperspyui/images/visibility_off.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/visibility_off2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/visibility_off2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/visibility_on.svg` & `hyperspyUI-1.3.0/hyperspyui/images/visibility_on.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/visibility_on2.svg` & `hyperspyUI-1.3.0/hyperspyui/images/visibility_on2.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/zero_loss.svg` & `hyperspyUI-1.3.0/hyperspyui/images/zero_loss.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/images/zoom.svg` & `hyperspyUI-1.3.0/hyperspyui/images/zoom.svg`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/log.py` & `hyperspyUI-1.3.0/hyperspyui/log.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/mainwindow.py` & `hyperspyUI-1.3.0/hyperspyui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/mainwindowbase.py` & `hyperspyUI-1.3.0/hyperspyui/mainwindowbase.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/mainwindowhyperspy.py` & `hyperspyUI-1.3.0/hyperspyui/mainwindowhyperspy.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/mainwindowutillayer.py` & `hyperspyUI-1.3.0/hyperspyui/mainwindowutillayer.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/mdi_mpl_backend.py` & `hyperspyUI-1.3.0/hyperspyui/mdi_mpl_backend.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/modelwrapper.py` & `hyperspyUI-1.3.0/hyperspyui/modelwrapper.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/overrides.py` & `hyperspyUI-1.3.0/hyperspyui/overrides.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugincreator.py` & `hyperspyUI-1.3.0/hyperspyui/plugincreator.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/pluginmanager.py` & `hyperspyUI-1.3.0/hyperspyui/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/__init__.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/align.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/align.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/alignzlp.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/alignzlp.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/axesconf.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/axesconf.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/axesorderwidget.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/axesorderwidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/basicsignal.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/basicsignal.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/basicspectrum.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/basicspectrum.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/cmappicker.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/cmappicker.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/croptool.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/croptool.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/dataastext.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/dataastext.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/dmannotations.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/dmannotations.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/eelsdb.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/eelsdb.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/fft.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/fft.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/fitting.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/fitting.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 
 import os
 from scipy import stats
 import numpy as np
 
 from hyperspyui.tools import SelectionTool
 from hyperspy.roi import BaseInteractiveROI
-from hyperspy.utils.markers import line_segment, text
+try: 
+    from hyperspy.utils.markers import LineSegment, Text
+except ImportError:
+    from hyperspy.utils.markers import line_segment as LineSegment
+    from hyperspy.utils.markers import text as Text
 
 
 class FittingPlugin(Plugin):
     name = "Fitting plugin"
 
     def create_tools(self):
         self.reg_tool = RegressionTool()
@@ -64,17 +68,17 @@
         y = signal.data[tuple(slices)]
         x = axes[0].axis[slices[i_ax]]
 
         # TODO: If in signal dim, iterate through navigation space
         reg = stats.linregress(x, y)
         x1, x2 = np.min(x), np.max(x)
         y1, y2 = np.array([x1, x2]) * reg[0] + reg[1]
-        m_l = line_segment(x1, y1, x2, y2)
+        m_l = LineSegment(x1, y1, x2, y2)
         signal.add_marker(m_l)
-        m_t = text((x2+x1)*0.5, (y2+y1)*0.5,
+        m_t = Text((x2+x1)*0.5, (y2+y1)*0.5,
                    "y = %.4gx + %.4g, R=%.4g" % reg[0:3])
         signal.add_marker(m_t)
 
         self.record_code("signal = ui.get_selected_signal()")
         self.record_code("axes = " +
                          str(tuple([sig_axes.index(a) for a in axes])))
         self.record_code("roi = utils.roi." + str(roi))
```

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/gaussianfilter.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/gaussianfilter.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/gitgetter.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/gitgetter.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/imagerotation.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/imagerotation.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/linemeasure.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/linemeasure.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/metadataeditor.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/metadataeditor.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/mirrorplot.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/mirrorplot.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/moviesaver.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/moviesaver.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/mva.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/mva.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/plotutils.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/plotutils.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/plugin.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/rebin.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/rebin.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/recorderwidget.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/recorderwidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/segmentation.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/segmentation.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/stylesheet.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/stylesheet.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/tightlayout.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/tightlayout.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/plugins/virtual_aperture.py` & `hyperspyUI-1.3.0/hyperspyui/plugins/virtual_aperture.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/recorder.py` & `hyperspyUI-1.3.0/hyperspyui/recorder.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/settings.py` & `hyperspyUI-1.3.0/hyperspyui/settings.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/signalwrapper.py` & `hyperspyUI-1.3.0/hyperspyui/signalwrapper.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/singleapplication.py` & `hyperspyUI-1.3.0/hyperspyui/singleapplication.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/smartcolorsvgiconengine.py` & `hyperspyUI-1.3.0/hyperspyui/smartcolorsvgiconengine.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/tests/conftest.py` & `hyperspyUI-1.3.0/hyperspyui/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/tests/test_backend.py` & `hyperspyUI-1.3.0/hyperspyui/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/tests/test_plotting.py` & `hyperspyUI-1.3.0/hyperspyui/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/tests/test_single_application.py` & `hyperspyUI-1.3.0/hyperspyui/tests/test_single_application.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/threaded.py` & `hyperspyUI-1.3.0/hyperspyui/threaded.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/tools.py` & `hyperspyUI-1.3.0/hyperspyui/tools.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/uiprogressbar.py` & `hyperspyUI-1.3.0/hyperspyui/uiprogressbar.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/util.py` & `hyperspyUI-1.3.0/hyperspyui/util.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/__init__.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/_editor_server.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/_editor_server.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/axespicker.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/axespicker.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/colorpicker.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/colorpicker.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/consolewidget.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/consolewidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/dataviewwidget.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/dataviewwidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/editorwidget.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/editorwidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/elementpicker.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/elementpicker.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/extendedqwidgets.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/extendedqwidgets.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/flowlayout.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/flowlayout.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/periodictable.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/periodictable.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/pickxsignals.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/pickxsignals.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/pluginmanagerwidget.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/pluginmanagerwidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/settingsdialog.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/signallist.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/signallist.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/stringinput.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/stringinput.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/hyperspyui/widgets/traitswidget.py` & `hyperspyUI-1.3.0/hyperspyui/widgets/traitswidget.py`

 * *Files identical despite different names*

### Comparing `hyperspyUI-1.2.0/setup.py` & `hyperspyUI-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,18 @@
     python_requires='~=3.7',
     install_requires=[
         # Add rosettasciio when it is released
         'hyperspy >= 1.7.2',
         'hyperspy-gui-traitsui >= 1.3.1',
         'matplotlib >= 3.0.3',
         'packaging',
-        'pyqode.python >= 2.6.0',
+        'pyqode.python >= 4.0.2',
+        'pyqode.core >= 4.0.10',
         'pyface >=6.0.0',
-        'pyflakes <2.5', # for pyqode.python
+        'pyflakes',
         'autopep8',
         'traits',
         'traitsui >=5.2.0',
         'qtconsole >=5.2.0',
         'ipykernel >=5.2.0',
         'qtpy',
         ],
@@ -93,14 +94,15 @@
     ],
     classifiers=[
 
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Environment :: MacOS X",
         "Environment :: Win32 (MS Windows)",
         "Environment :: X11 Applications :: Qt",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

