# Comparing `tmp/pyminflux-0.1.0.tar.gz` & `tmp/pyminflux-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyminflux-0.1.0.tar", max compression
+gzip compressed data, was "pyminflux-0.1.1.tar", max compression
```

## Comparing `pyminflux-0.1.0.tar` & `pyminflux-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0    11358 2023-05-02 11:32:56.697662 pyminflux-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1658 2023-05-02 16:46:37.537523 pyminflux-0.1.0/README.md
--rw-r--r--   0        0        0      778 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/__init__.py
--rw-r--r--   0        0        0      817 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/analysis/__init__.py
--rw-r--r--   0        0        0    14408 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/analysis/_analysis.py
--rw-r--r--   0        0        0      638 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/base/__init__.py
--rw-r--r--   0        0        0      918 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/base/_base.py
--rw-r--r--   0        0        0     1055 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/main.py
--rw-r--r--   0        0        0      650 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/processor/__init__.py
--rw-r--r--   0        0        0    27101 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/processor/_processor.py
--rw-r--r--   0        0        0      644 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/reader/__init__.py
--rw-r--r--   0        0        0    20253 2023-05-02 11:32:56.701662 pyminflux-0.1.0/pyminflux/reader/_reader.py
--rw-r--r--   0        0        0   139482 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/resources.py
--rw-r--r--   0        0        0      747 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/resources.qrc
--rw-r--r--   0        0        0      641 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/settings/__init__.py
--rw-r--r--   0        0        0     1679 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/settings/_settings.py
--rw-r--r--   0        0        0      646 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/state/__init__.py
--rw-r--r--   0        0        0     5478 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/state/_state.py
--rw-r--r--   0        0        0      633 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/threads/__init__.py
--rw-r--r--   0        0        0      875 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/threads/_threads.py
--rw-r--r--   0        0        0      608 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/ui/__init__.py
--rw-r--r--   0        0        0    31339 2023-05-02 11:32:56.705662 pyminflux-0.1.0/pyminflux/ui/analyzer.py
--rw-r--r--   0        0        0     9313 2023-04-26 08:29:10.930459 pyminflux-0.1.0/pyminflux/ui/analyzer.ui
--rw-r--r--   0        0        0   216854 2023-05-02 11:32:56.857662 pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.icns
--rw-r--r--   0        0        0  1143198 2023-05-02 11:32:56.861662 pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.ico
--rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.png
--rwxr-xr-x   0        0        0      670 2023-05-02 11:32:56.709662 pyminflux-0.1.0/pyminflux/ui/assets/create_resources.sh
--rwxr-xr-x   0        0        0     1805 2023-05-02 11:32:56.709662 pyminflux-0.1.0/pyminflux/ui/assets/png_to_icns.sh
--rw-r--r--   0        0        0    10867 2023-05-02 11:32:56.709662 pyminflux-0.1.0/pyminflux/ui/color_unmixer.py
--rw-r--r--   0        0        0     8738 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/color_unmixer.ui
--rw-r--r--   0        0        0     2561 2023-05-02 11:57:29.698894 pyminflux-0.1.0/pyminflux/ui/dataviewer.py
--rw-r--r--   0        0        0     1008 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/emittingstream.py
--rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.0/pyminflux/ui/icons/icon.png
--rw-r--r--   0        0        0    30661 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/main_window.py
--rw-r--r--   0        0        0     4252 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/main_window.ui
--rw-r--r--   0        0        0    14348 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/options.py
--rw-r--r--   0        0        0     9054 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/options.ui
--rw-r--r--   0        0        0     2057 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/pandas_datamodel.py
--rw-r--r--   0        0        0    13746 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/plotter.py
--rw-r--r--   0        0        0     3477 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/plotter_3d.py
--rw-r--r--   0        0        0      544 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/plotter_3d.ui
--rw-r--r--   0        0        0     4775 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/plotter_toolbar.py
--rw-r--r--   0        0        0     3254 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/plotter_toolbar.ui
--rw-r--r--   0        0        0     4125 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/roi_ranges.py
--rw-r--r--   0        0        0     4422 2023-04-26 08:29:10.942459 pyminflux-0.1.0/pyminflux/ui/roi_ranges.ui
--rw-r--r--   0        0        0    17807 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/time_inspector.py
--rw-r--r--   0        0        0     3128 2023-04-26 08:29:10.942459 pyminflux-0.1.0/pyminflux/ui/time_inspector.ui
--rw-r--r--   0        0        0    11656 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/ui_analyzer.py
--rw-r--r--   0        0        0    10455 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/ui_color_unmixer.py
--rw-r--r--   0        0        0     8035 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/ui_main_window.py
--rw-r--r--   0        0        0    12416 2023-05-02 11:32:56.713662 pyminflux-0.1.0/pyminflux/ui/ui_options.py
--rw-r--r--   0        0        0     2276 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/ui_plotter_3d.py
--rw-r--r--   0        0        0     5670 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/ui_plotter_toolbar.py
--rw-r--r--   0        0        0     5773 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/ui_roi_ranges.py
--rw-r--r--   0        0        0     5795 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/ui_time_inspector.py
--rw-r--r--   0        0        0    12468 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/ui_wizard.py
--rw-r--r--   0        0        0    12564 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/wizard.py
--rw-r--r--   0        0        0     9022 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/ui/wizard.ui
--rw-r--r--   0        0        0      677 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/utils/__init__.py
--rw-r--r--   0        0        0     2614 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/utils/_utils.py
--rw-r--r--   0        0        0      644 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/writer/__init__.py
--rw-r--r--   0        0        0     1851 2023-05-02 11:32:56.717662 pyminflux-0.1.0/pyminflux/writer/_writer.py
--rw-r--r--   0        0        0      908 2023-05-02 15:39:00.461716 pyminflux-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 pyminflux-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-02 11:32:56.697662 pyminflux-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2262 2023-05-04 13:54:57.119239 pyminflux-0.1.1/README.md
+-rw-r--r--   0        0        0      778 2023-05-03 09:52:34.888791 pyminflux-0.1.1/pyminflux/__init__.py
+-rw-r--r--   0        0        0      817 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/analysis/__init__.py
+-rw-r--r--   0        0        0    14408 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/analysis/_analysis.py
+-rw-r--r--   0        0        0      638 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/base/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/base/_base.py
+-rw-r--r--   0        0        0     1081 2023-05-03 07:24:53.358703 pyminflux-0.1.1/pyminflux/main.py
+-rw-r--r--   0        0        0      650 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/processor/__init__.py
+-rw-r--r--   0        0        0    27101 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/processor/_processor.py
+-rw-r--r--   0        0        0      644 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/reader/__init__.py
+-rw-r--r--   0        0        0    20253 2023-05-02 11:32:56.701662 pyminflux-0.1.1/pyminflux/reader/_reader.py
+-rw-r--r--   0        0        0   139482 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/resources.py
+-rw-r--r--   0        0        0      747 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/resources.qrc
+-rw-r--r--   0        0        0      641 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/settings/__init__.py
+-rw-r--r--   0        0        0     1679 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/settings/_settings.py
+-rw-r--r--   0        0        0      646 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/state/__init__.py
+-rw-r--r--   0        0        0     5478 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/state/_state.py
+-rw-r--r--   0        0        0      633 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/threads/__init__.py
+-rw-r--r--   0        0        0      875 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/threads/_threads.py
+-rw-r--r--   0        0        0      608 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/ui/__init__.py
+-rw-r--r--   0        0        0    31339 2023-05-02 11:32:56.705662 pyminflux-0.1.1/pyminflux/ui/analyzer.py
+-rw-r--r--   0        0        0     9313 2023-04-26 08:29:10.930459 pyminflux-0.1.1/pyminflux/ui/analyzer.ui
+-rw-r--r--   0        0        0   216854 2023-05-02 11:32:56.857662 pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.icns
+-rw-r--r--   0        0        0  1143198 2023-05-02 11:32:56.861662 pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.ico
+-rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.png
+-rw-r--r--   0        0        0     8998 2023-05-03 14:33:18.090905 pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3_small.png
+-rwxr-xr-x   0        0        0      670 2023-05-02 11:32:56.709662 pyminflux-0.1.1/pyminflux/ui/assets/create_resources.sh
+-rwxr-xr-x   0        0        0     1805 2023-05-02 11:32:56.709662 pyminflux-0.1.1/pyminflux/ui/assets/png_to_icns.sh
+-rw-r--r--   0        0        0    10867 2023-05-02 11:32:56.709662 pyminflux-0.1.1/pyminflux/ui/color_unmixer.py
+-rw-r--r--   0        0        0     8738 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/color_unmixer.ui
+-rw-r--r--   0        0        0     2561 2023-05-02 11:57:29.698894 pyminflux-0.1.1/pyminflux/ui/dataviewer.py
+-rw-r--r--   0        0        0     1008 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/emittingstream.py
+-rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.1/pyminflux/ui/icons/icon.png
+-rw-r--r--   0        0        0    30661 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/main_window.py
+-rw-r--r--   0        0        0     4252 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/main_window.ui
+-rw-r--r--   0        0        0    14348 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/options.py
+-rw-r--r--   0        0        0     9054 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/options.ui
+-rw-r--r--   0        0        0     2057 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/pandas_datamodel.py
+-rw-r--r--   0        0        0    13746 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/plotter.py
+-rw-r--r--   0        0        0     3477 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/plotter_3d.py
+-rw-r--r--   0        0        0      544 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/plotter_3d.ui
+-rw-r--r--   0        0        0     4775 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/plotter_toolbar.py
+-rw-r--r--   0        0        0     3254 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/plotter_toolbar.ui
+-rw-r--r--   0        0        0     4125 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/roi_ranges.py
+-rw-r--r--   0        0        0     4422 2023-04-26 08:29:10.942459 pyminflux-0.1.1/pyminflux/ui/roi_ranges.ui
+-rw-r--r--   0        0        0    17807 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/time_inspector.py
+-rw-r--r--   0        0        0     3128 2023-04-26 08:29:10.942459 pyminflux-0.1.1/pyminflux/ui/time_inspector.ui
+-rw-r--r--   0        0        0    11656 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/ui_analyzer.py
+-rw-r--r--   0        0        0    10455 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/ui_color_unmixer.py
+-rw-r--r--   0        0        0     8035 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/ui_main_window.py
+-rw-r--r--   0        0        0    12416 2023-05-02 11:32:56.713662 pyminflux-0.1.1/pyminflux/ui/ui_options.py
+-rw-r--r--   0        0        0     2276 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/ui_plotter_3d.py
+-rw-r--r--   0        0        0     5670 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/ui_plotter_toolbar.py
+-rw-r--r--   0        0        0     5773 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/ui_roi_ranges.py
+-rw-r--r--   0        0        0     5795 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/ui_time_inspector.py
+-rw-r--r--   0        0        0    12468 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/ui_wizard.py
+-rw-r--r--   0        0        0    12564 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/wizard.py
+-rw-r--r--   0        0        0     9022 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/ui/wizard.ui
+-rw-r--r--   0        0        0      677 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/utils/__init__.py
+-rw-r--r--   0        0        0     2614 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/utils/_utils.py
+-rw-r--r--   0        0        0      644 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/writer/__init__.py
+-rw-r--r--   0        0        0     1851 2023-05-02 11:32:56.717662 pyminflux-0.1.1/pyminflux/writer/_writer.py
+-rw-r--r--   0        0        0     1880 2023-05-04 08:03:45.223174 pyminflux-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 pyminflux-0.1.1/PKG-INFO
```

### Comparing `pyminflux-0.1.0/LICENSE.txt` & `pyminflux-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/README.md` & `pyminflux-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,65 @@
-# pyMINFLUX
+# ![](pyminflux/ui/assets/Logo_v3_small.png)&nbsp;&nbsp;&nbsp;pyMINFLUX
 
 Reader, analyzer, and viewer of MINFLUX raw data.
 
 ## Installation
 
-Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](#). 
+### Apps
+
+Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](https://github.com/bsse-scf/pyMINFLUX/releases/latest). 
 
 **Please note**: since pyMINFLUX on macOS comes from an *unidentified developer*, you might need to make an exception in the macOS security settings when launching it for the first time. To do this, right-click on the application icon and select `Open`. After this initial setup, you can simply double-click the icon to launch pyMINFLUX normally.
 
+### pip
+
+The latest version of pyMINFLUX can also be installed from [pypi.org](https://pypi.org/project/pyminflux/). pyMINFLUX is compatible with and tested on Python 3.10 and 3.11. It is recommended to install pyMINFLUX in editable mode in a conda environment as follows:
+
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ pip install --upgrade pyminflux
+```
+
+pyMINFLUX can then be easily run from the command line:
+
+```sh
+$ pyminflux
+```
+
 ## For developers and tinkerers
 
 pyMINFLUX is compatible with and tested on Python 3.10 and 3.11. For development, it is recommended to install pyMINFLUX in editable mode in a [conda](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links) environment as follows:
 
 ### Windows and Linux
 
-```bash
-conda create -n pyminflux-env python=3.10  # or 3.11
-conda activate pyminflux-env
-git clone https://git.bsse.ethz.ch/pontia/pyminflux ${/path/to/pyminflux}
-cd ${/path/to/pyminflux}
-python -m pip install -e .
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
+$ cd /path/to/pyminflux
+$ python -m pip install -e .
 ```
 
 ### macOS
 
 openGL support in recent macOS requires `pyopengl` to be installed with `conda` instead of `pip`.
 
-```bash
-conda create -n pyminflux-env python=3.10  # or 3.11
-conda activate pyminflux-env
-git clone https://git.bsse.ethz.ch/pontia/pyminflux ${/path/to/pyminflux}
-cd ${/path/to/pyminflux}
-conda install pyopengl       # This is specific to macOS
-python -m pip install -e .
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
+$ cd /path/to/pyminflux
+$ conda install pyopengl       # This is specific to macOS
+$ python -m pip install -e .
 ```
 
 ### Running pyMinFlux from console
 
-```bash
-cd ${/path/to/pyminflux}
-python pyminflux/main.py
+```sh
+$ cd /path/to/pyminflux
+$ python pyminflux/main.py
 ```
 
 ## Official website and documentation
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
```

### Comparing `pyminflux-0.1.0/pyminflux/__init__.py` & `pyminflux-0.1.1/pyminflux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import pyqtgraph as pg
 
 __APP_NAME__ = "pyMINFLUX"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # PyQtGraph settings
 pg.setConfigOption("imageAxisOrder", "row-major")  # For best performance
```

### Comparing `pyminflux-0.1.0/pyminflux/analysis/__init__.py` & `pyminflux-0.1.1/pyminflux/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/analysis/_analysis.py` & `pyminflux-0.1.1/pyminflux/analysis/_analysis.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/base/__init__.py` & `pyminflux-0.1.1/pyminflux/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/base/_base.py` & `pyminflux-0.1.1/pyminflux/base/_base.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/main.py` & `pyminflux-0.1.1/pyminflux/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication
 
 import pyminflux.resources
 from pyminflux.ui.main_window import PyMinFluxMainWindow
 
-if __name__ == "__main__":
+
+def main():
     app = QApplication(sys.argv)
     if sys.platform.startswith("linux"):
         app.setStyle("fusion")
     main = PyMinFluxMainWindow()
 
     icon = QIcon(":/icons/icon.png")
     app.setWindowIcon(icon)
     main.show()
 
     sys.exit(app.exec())
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyminflux-0.1.0/pyminflux/processor/__init__.py` & `pyminflux-0.1.1/pyminflux/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/processor/_processor.py` & `pyminflux-0.1.1/pyminflux/processor/_processor.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/reader/__init__.py` & `pyminflux-0.1.1/pyminflux/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/reader/_reader.py` & `pyminflux-0.1.1/pyminflux/reader/_reader.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/resources.py` & `pyminflux-0.1.1/pyminflux/resources.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/resources.qrc` & `pyminflux-0.1.1/pyminflux/resources.qrc`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/settings/__init__.py` & `pyminflux-0.1.1/pyminflux/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/settings/_settings.py` & `pyminflux-0.1.1/pyminflux/settings/_settings.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/state/__init__.py` & `pyminflux-0.1.1/pyminflux/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/state/_state.py` & `pyminflux-0.1.1/pyminflux/state/_state.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/threads/__init__.py` & `pyminflux-0.1.1/pyminflux/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/threads/_threads.py` & `pyminflux-0.1.1/pyminflux/threads/_threads.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/__init__.py` & `pyminflux-0.1.1/pyminflux/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/analyzer.py` & `pyminflux-0.1.1/pyminflux/ui/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/analyzer.ui` & `pyminflux-0.1.1/pyminflux/ui/analyzer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.icns` & `pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.icns`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.ico` & `pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.ico`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/assets/Logo_v3.png` & `pyminflux-0.1.1/pyminflux/ui/assets/Logo_v3.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/assets/create_resources.sh` & `pyminflux-0.1.1/pyminflux/ui/assets/create_resources.sh`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/assets/png_to_icns.sh` & `pyminflux-0.1.1/pyminflux/ui/assets/png_to_icns.sh`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/color_unmixer.py` & `pyminflux-0.1.1/pyminflux/ui/color_unmixer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/color_unmixer.ui` & `pyminflux-0.1.1/pyminflux/ui/color_unmixer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/dataviewer.py` & `pyminflux-0.1.1/pyminflux/ui/dataviewer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/emittingstream.py` & `pyminflux-0.1.1/pyminflux/ui/emittingstream.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/icons/icon.png` & `pyminflux-0.1.1/pyminflux/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/main_window.py` & `pyminflux-0.1.1/pyminflux/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/main_window.ui` & `pyminflux-0.1.1/pyminflux/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/options.py` & `pyminflux-0.1.1/pyminflux/ui/options.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/options.ui` & `pyminflux-0.1.1/pyminflux/ui/options.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/pandas_datamodel.py` & `pyminflux-0.1.1/pyminflux/ui/pandas_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/plotter.py` & `pyminflux-0.1.1/pyminflux/ui/plotter.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/plotter_3d.py` & `pyminflux-0.1.1/pyminflux/ui/plotter_3d.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/plotter_3d.ui` & `pyminflux-0.1.1/pyminflux/ui/plotter_3d.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/plotter_toolbar.py` & `pyminflux-0.1.1/pyminflux/ui/plotter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/plotter_toolbar.ui` & `pyminflux-0.1.1/pyminflux/ui/plotter_toolbar.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/roi_ranges.py` & `pyminflux-0.1.1/pyminflux/ui/roi_ranges.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/roi_ranges.ui` & `pyminflux-0.1.1/pyminflux/ui/roi_ranges.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/time_inspector.py` & `pyminflux-0.1.1/pyminflux/ui/time_inspector.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/time_inspector.ui` & `pyminflux-0.1.1/pyminflux/ui/time_inspector.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_analyzer.py` & `pyminflux-0.1.1/pyminflux/ui/ui_analyzer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_color_unmixer.py` & `pyminflux-0.1.1/pyminflux/ui/ui_color_unmixer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_main_window.py` & `pyminflux-0.1.1/pyminflux/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_options.py` & `pyminflux-0.1.1/pyminflux/ui/ui_options.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_plotter_3d.py` & `pyminflux-0.1.1/pyminflux/ui/ui_plotter_3d.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_plotter_toolbar.py` & `pyminflux-0.1.1/pyminflux/ui/ui_plotter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_roi_ranges.py` & `pyminflux-0.1.1/pyminflux/ui/ui_roi_ranges.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_time_inspector.py` & `pyminflux-0.1.1/pyminflux/ui/ui_time_inspector.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/ui_wizard.py` & `pyminflux-0.1.1/pyminflux/ui/ui_wizard.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/wizard.py` & `pyminflux-0.1.1/pyminflux/ui/wizard.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/ui/wizard.ui` & `pyminflux-0.1.1/pyminflux/ui/wizard.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/utils/__init__.py` & `pyminflux-0.1.1/pyminflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/utils/_utils.py` & `pyminflux-0.1.1/pyminflux/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/writer/__init__.py` & `pyminflux-0.1.1/pyminflux/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/pyminflux/writer/_writer.py` & `pyminflux-0.1.1/pyminflux/writer/_writer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.0/PKG-INFO` & `pyminflux-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,101 @@
 Metadata-Version: 2.1
 Name: pyminflux
-Version: 0.1.0
+Version: 0.1.1
 Summary: Reader, processor, and viewer of MINFLUX raw data.
+Home-page: https://github.com/bsse-scf/pyMINFLUX
 License: Apache-2.0
+Keywords: MINFLUX,Visualization,Filtering,Analysis,Python
 Author: Aaron Ponti
 Author-email: aaron.ponti@bsse.ethz.ch
 Requires-Python: >=3.10,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pyopengl (>=3.1.6,<4.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
 Requires-Dist: pyside6 (>=6.4.0.1,<6.5)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/bsse-scf/pyMINFLUX/issues
+Project-URL: Documentation, https://github.com/bsse-scf/pyMINFLUX/wiki
+Project-URL: Repository, https://github.com/bsse-scf/pyMINFLUX
 Description-Content-Type: text/markdown
 
-# pyMINFLUX
+# ![](pyminflux/ui/assets/Logo_v3_small.png)&nbsp;&nbsp;&nbsp;pyMINFLUX
 
 Reader, analyzer, and viewer of MINFLUX raw data.
 
 ## Installation
 
-Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](#). 
+### Apps
+
+Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](https://github.com/bsse-scf/pyMINFLUX/releases/latest). 
 
 **Please note**: since pyMINFLUX on macOS comes from an *unidentified developer*, you might need to make an exception in the macOS security settings when launching it for the first time. To do this, right-click on the application icon and select `Open`. After this initial setup, you can simply double-click the icon to launch pyMINFLUX normally.
 
+### pip
+
+The latest version of pyMINFLUX can also be installed from [pypi.org](https://pypi.org/project/pyminflux/). pyMINFLUX is compatible with and tested on Python 3.10 and 3.11. It is recommended to install pyMINFLUX in editable mode in a conda environment as follows:
+
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ pip install --upgrade pyminflux
+```
+
+pyMINFLUX can then be easily run from the command line:
+
+```sh
+$ pyminflux
+```
+
 ## For developers and tinkerers
 
 pyMINFLUX is compatible with and tested on Python 3.10 and 3.11. For development, it is recommended to install pyMINFLUX in editable mode in a [conda](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links) environment as follows:
 
 ### Windows and Linux
 
-```bash
-conda create -n pyminflux-env python=3.10  # or 3.11
-conda activate pyminflux-env
-git clone https://git.bsse.ethz.ch/pontia/pyminflux ${/path/to/pyminflux}
-cd ${/path/to/pyminflux}
-python -m pip install -e .
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
+$ cd /path/to/pyminflux
+$ python -m pip install -e .
 ```
 
 ### macOS
 
 openGL support in recent macOS requires `pyopengl` to be installed with `conda` instead of `pip`.
 
-```bash
-conda create -n pyminflux-env python=3.10  # or 3.11
-conda activate pyminflux-env
-git clone https://git.bsse.ethz.ch/pontia/pyminflux ${/path/to/pyminflux}
-cd ${/path/to/pyminflux}
-conda install pyopengl       # This is specific to macOS
-python -m pip install -e .
+```sh
+$ conda create -n pyminflux-env python=3.11  # or 3.10
+$ conda activate pyminflux-env
+$ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
+$ cd /path/to/pyminflux
+$ conda install pyopengl       # This is specific to macOS
+$ python -m pip install -e .
 ```
 
 ### Running pyMinFlux from console
 
-```bash
-cd ${/path/to/pyminflux}
-python pyminflux/main.py
+```sh
+$ cd /path/to/pyminflux
+$ python pyminflux/main.py
 ```
 
 ## Official website and documentation
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
```

