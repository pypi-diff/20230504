# Comparing `tmp/acconeer-exptool-6.0.4.tar.gz` & `tmp/acconeer-exptool-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-6.0.4.tar", last modified: Thu Apr  6 09:52:44 2023, max compression
+gzip compressed data, was "acconeer-exptool-6.0.5.tar", last modified: Thu May  4 12:03:06 2023, max compression
```

## Comparing `acconeer-exptool-6.0.4.tar` & `acconeer-exptool-6.0.5.tar`

### file list

```diff
@@ -1,595 +1,607 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.899983 acconeer-exptool-6.0.4/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13026 2023-04-06 09:47:13.000000 acconeer-exptool-6.0.4/CHANGELOG.md
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-04-06 09:34:49.000000 acconeer-exptool-6.0.4/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/docker/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.903983 acconeer-exptool-6.0.4/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/bilateration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/breathing/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/breathing/breathing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/distance/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/distance/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/phase_tracking/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5806 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/phase_tracking/phase_tracking.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/presence/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/record_data/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      921 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/record_data/barebones.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1092 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/record_data/with_cli.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/smart_presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/smart_presence/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/smart_presence/ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/stress.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8536 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/surface_velocity/example_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8910 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/touchless_button/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/examples/a121/vibration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/gui/main.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/portable/package/update.bat
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/pyproject.toml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2434 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.903983 acconeer-exptool-6.0.4/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.911983 acconeer-exptool-6.0.4/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25124 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.915984 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.919983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      671 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.923983 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:58:10.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      592 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4585 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      822 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6962 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4129 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15712 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11468 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      229 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7651 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2820 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11206 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3854 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4082 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.927984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      646 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4002 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7344 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8243 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7079 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7327 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25658 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-04-06 09:38:16.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    57805 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24685 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14290 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26195 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22272 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.931984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10510 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22205 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13898 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26782 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:11.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14570 2023-04-06 09:38:16.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7398 2023-02-03 12:56:48.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      971 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27938 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2840 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1986 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_message.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4896 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1515 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.935984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2183 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      524 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10472 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/connection_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    32628 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/flash_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3472 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/main_window.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10087 2022-12-22 09:46:27.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6298 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:51.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3829 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25589 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13395 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5574 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8590 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1909 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      298 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12123 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4629 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/recording_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9485 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/status_bar.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1227 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84288 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/modules.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10741 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.907983 acconeer-exptool-6.0.4/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.939984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8950 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.943984 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.4/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24849 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      476 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-04-06 09:52:44.000000 acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/tools/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3347 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/tools/check_permissions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-05 21:07:58.000000 acconeer-exptool-6.0.4/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-04-06 09:52:44.947984 acconeer-exptool-6.0.4/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.4/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13506 2023-05-04 11:32:49.000000 acconeer-exptool-6.0.5/CHANGELOG.md
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-04 11:32:49.000000 acconeer-exptool-6.0.5/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/docker/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/bilateration/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/breathing/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/breathing/breathing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/distance/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/distance/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/phase_tracking/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/phase_tracking/phase_tracking.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/presence/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/record_data/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      921 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/record_data/barebones.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1092 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/record_data/with_cli.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/smart_presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/smart_presence/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/smart_presence/ref_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/stress.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/surface_velocity/example_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/touchless_button/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/examples/a121/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/gui/main.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/portable/package/update.bat
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.378632 acconeer-exptool-6.0.5/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.386632 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-04 11:25:32.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.390632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.394632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.398632 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      671 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:58:10.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      592 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4585 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      822 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6962 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4129 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15712 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.402633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:57.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11468 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      229 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7651 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2820 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11206 2023-05-04 11:00:03.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3854 2023-05-04 10:56:45.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4082 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      646 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7322 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6492 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7327 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24882 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      376 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59249 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24069 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_processors.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.406633 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14290 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25641 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21666 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:19.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11412 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21651 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25992 2023-04-26 11:57:07.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:11.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14570 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7398 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.410632 acconeer-exptool-6.0.5/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27938 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2840 2023-05-03 13:30:39.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5135 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1857 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_message.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4896 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_model.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2222 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.414633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/icons.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:51.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:17.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:18.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:02.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-04 11:26:07.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-04 11:25:32.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.382632 acconeer-exptool-6.0.5/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.418633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/mpl_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.422633 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-04-03 13:53:22.000000 acconeer-exptool-6.0.5/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25411 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-04 12:03:05.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-05-04 12:03:06.000000 acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/tools/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3715 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_permissions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-25 21:08:06.000000 acconeer-exptool-6.0.5/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-04 12:03:06.426633 acconeer-exptool-6.0.5/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-21 10:06:47.000000 acconeer-exptool-6.0.5/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-6.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-6.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/CHANGELOG.md` & `acconeer-exptool-6.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v6.0.5
+
+### Added
+- A121: Surface velocity: Validation added to check that start point is
+  larger than the surface distance
+- Tabs in the A121 Application
+
+### Changed
+- A121: Surface velocity: Remove unused sensor angle from processing config
+
+### Fixed
+- A111: Perform handshake on multiple baudrate even when overriding baudrate
+- A111: Fix bug with not being able to untick override baudrate option
+- A111: Bug in acconeer.exptool.app --purge-config which caused a crash
+
 ## v6.0.4
 
 ### Changed
 - Pin PySide version, which evades some problems with its latest release
 
 ## v6.0.1
```

### Comparing `acconeer-exptool-6.0.4/Jenkinsfile` & `acconeer-exptool-6.0.5/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/LICENSE.md` & `acconeer-exptool-6.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/PKG-INFO` & `acconeer-exptool-6.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 6.0.4
+Version: 6.0.5
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-6.0.4/README.md` & `acconeer-exptool-6.0.5/README.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/docker/Dockerfile` & `acconeer-exptool-6.0.5/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/dodo.py` & `acconeer-exptool-6.0.5/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/basic.py` & `acconeer-exptool-6.0.5/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/basic_continuous.py` & `acconeer-exptool-6.0.5/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/load_record.py` & `acconeer-exptool-6.0.5/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/load_record_h5.m` & `acconeer-exptool-6.0.5/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-6.0.5/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/record_data/barebones.py` & `acconeer-exptool-6.0.5/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-6.0.5/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/record_data/with_cli.py` & `acconeer-exptool-6.0.5/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/services/envelope.py` & `acconeer-exptool-6.0.5/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/services/iq.py` & `acconeer-exptool-6.0.5/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/services/power_bins.py` & `acconeer-exptool-6.0.5/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/services/sparse.py` & `acconeer-exptool-6.0.5/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/utils/ping.py` & `acconeer-exptool-6.0.5/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a111/utils/test_throughput.py` & `acconeer-exptool-6.0.5/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/basic.py` & `acconeer-exptool-6.0.5/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-6.0.5/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/breathing/breathing.py` & `acconeer-exptool-6.0.5/examples/a121/breathing/breathing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/distance/detector.py` & `acconeer-exptool-6.0.5/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/distance/processor.py` & `acconeer-exptool-6.0.5/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/extended_config.py` & `acconeer-exptool-6.0.5/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/load_record.py` & `acconeer-exptool-6.0.5/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/load_record_h5.m` & `acconeer-exptool-6.0.5/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-6.0.5/examples/a121/phase_tracking/phase_tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             self.argument_vertical_line.setValue(peak_loc)
             self.sweep_vertical_line.show()
             self.argument_vertical_line.show()
         else:
             self.sweep_vertical_line.hide()
             self.argument_vertical_line.hide()
 
-        if history is not None:
+        if history.shape[0] != 0:
             # update history plot
             self.history_curve.setData(rel_time_stamps, history)
             lims = self.distance_hist_smooth_lim.update(history)
             self.history_plot.setYRange(lims[0], lims[1])
         self.history_plot.setXRange(-Processor.TIME_HORIZON_S, 0)
```

### Comparing `acconeer-exptool-6.0.4/examples/a121/plot.py` & `acconeer-exptool-6.0.5/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/presence/detector.py` & `acconeer-exptool-6.0.5/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/presence/processor.py` & `acconeer-exptool-6.0.5/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/record_data/barebones.py` & `acconeer-exptool-6.0.5/examples/a121/record_data/barebones.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from acconeer.exptool import a121
 
 
-# Here we create a H5Recorder.
-# The H5Recorder is an object that saves frames directly to a H5-file.
-filename = "data.h5"
-h5_recorder = a121.H5Recorder(filename)
-
 # Client creation
 client = a121.Client.open(ip_address="192.168.0.1")
 
 # Session setup, just like the other examples.
 config = a121.SessionConfig()
 client.setup_session(config)
 
+# Here we create a H5Recorder.
+# The H5Recorder is an object that saves frames directly to a H5-file.
+filename = "data.h5"
+h5_recorder = a121.H5Recorder(filename)
+
 # Here we send the H5Recorder to the Client.
 # After this call, the client is responsible for the H5Recorder.
 # The Client will automatically close the file when
 # "stop_session" is called.
 client.start_session(recorder=h5_recorder)
 
 n = 10
```

### Comparing `acconeer-exptool-6.0.4/examples/a121/record_data/with_cli.py` & `acconeer-exptool-6.0.5/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/reuse_calibration.py` & `acconeer-exptool-6.0.5/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/smart_presence/processor.py` & `acconeer-exptool-6.0.5/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-6.0.5/examples/a121/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/stress.py` & `acconeer-exptool-6.0.5/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/subsweeps.py` & `acconeer-exptool-6.0.5/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-6.0.5/examples/a121/surface_velocity/example_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from acconeer.exptool.a121.algo.surface_velocity import ExampleApp, ExampleAppConfig
 
 
 def main():
     args = a121.ExampleArgumentParser().parse_args()
     et.utils.config_logging(args)
 
-    client = a121.Client(**a121.get_client_args(args))
-    client.connect()
+    client = a121.Client.open(**a121.get_client_args(args))
 
     example_app_config = ExampleAppConfig(
         surface_distance=0.40,
         sensor_angle=35,
         num_points=4,
         step_length=6,
         hwaas=16,
@@ -62,15 +61,15 @@
         try:
             pg_process.put_data(example_app_result)
         except et.PGProccessDiedException:
             break
 
     print("Disconnecting...")
     pg_process.close()
-    client.disconnect()
+    client.close()
 
 
 class PGUpdater:
 
     _VELOCITY_Y_SCALE_MARGIN_M = 0.25
 
     def __init__(
```

### Comparing `acconeer-exptool-6.0.4/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-6.0.5/examples/a121/surface_velocity/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from acconeer.exptool.a121.algo.surface_velocity._processor import Processor, ProcessorConfig
 
 
 def main():
     args = a121.ExampleArgumentParser().parse_args()
     et.utils.config_logging(args)
 
-    client = a121.Client(**a121.get_client_args(args))
-    client.connect()
+    client = a121.Client.open(**a121.get_client_args(args))
 
     sensor_config = a121.SensorConfig(
         profile=a121.Profile.PROFILE_3,
         start_point=180,
         num_points=4,
         step_length=6,
         hwaas=16,
@@ -36,15 +35,14 @@
         inter_sweep_idle_state=a121.IdleState.READY,
     )
 
     metadata = client.setup_session(sensor_config)
 
     processor_config = ProcessorConfig(
         surface_distance=0.40,
-        sensor_angle=35,
         time_series_length=1024,
     )
 
     processor = Processor(
         sensor_config=sensor_config,
         metadata=metadata,
         processor_config=processor_config,
@@ -76,15 +74,15 @@
         try:
             pg_process.put_data(processor_result)
         except et.PGProccessDiedException:
             break
 
     print("Disconnecting...")
     pg_process.close()
-    client.disconnect()
+    client.close()
 
 
 class PGUpdater:
 
     _VELOCITY_Y_SCALE_MARGIN_M = 0.25
 
     def __init__(
```

### Comparing `acconeer-exptool-6.0.4/examples/a121/touchless_button/processor.py` & `acconeer-exptool-6.0.5/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/examples/a121/vibration/vibration.py` & `acconeer-exptool-6.0.5/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/gui/main.py` & `acconeer-exptool-6.0.5/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/noxfile.py` & `acconeer-exptool-6.0.5/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 nox.options.stop_on_first_error = True
 nox.options.reuse_existing_virtualenvs = True
 
 
 BLACK_SPEC = "black==22.12.0"
 ISORT_SPEC = "isort==5.6.3"
 RUFF_SPEC = "ruff==0.0.260"
-MYPY_SPEC = "mypy==1.0.1"
+MYPY_SPEC = "mypy==1.2.0"
 PIP_SPEC = "pip>=21.3"
 PYTEST_MOCK_SPEC = "pytest-mock==3.3.1"
 PYTEST_SPEC = "pytest==7.2"
 PYTEST_XDIST_SPEC = "pytest-xdist==3.1.0"
 DIRTY_EQUALS_SPEC = "dirty-equals==0.5.0"
 
 SPHINX_SOURCE_DIR = "docs"
@@ -99,16 +99,16 @@
 def reformat(session):
     session.install(
         BLACK_SPEC,
         ISORT_SPEC,
         RUFF_SPEC,
     )
     session.run("python", "tools/check_copyright.py", "--update-year")
-    session.run("python", "-m", "ruff", "--fix", ".")
     session.run("python", "-m", "black", ".")
+    session.run("python", "-m", "ruff", "--fix", ".")
     session.run("python", "-m", "isort", ".")
 
 
 @nox.session
 @nox.parametrize("python", ["3.7"])
 def mypy(session):
     session.install("-e", ".", MYPY_SPEC, PYTEST_SPEC)
```

### Comparing `acconeer-exptool-6.0.4/portable/make.py` & `acconeer-exptool-6.0.5/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/portable/package/tools/update.py` & `acconeer-exptool-6.0.5/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/pyproject.toml` & `acconeer-exptool-6.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/setup.cfg` & `acconeer-exptool-6.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 [options.extras_require]
 algo = 
 	scipy
 app = 
 	bs4
 	docutils>=0.17,!=0.18
-	matplotlib>=3.5.0
+	matplotlib>3.5.1
 	platformdirs
 	psutil
 	pyperclip
 	pyside6!=6.3.0,!=6.3.2,<6.5
 	pyqtdarktheme
 	pyqtgraph>=0.12.4
 	qtawesome
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 import abc
 import logging
 import multiprocessing as mp
 import platform
 import queue
@@ -181,54 +181,51 @@
             self._link = links.SerialLink(port)
         else:
             self._link = links.SerialProcessLink(port)
 
     def _connect(self):
         self._link.timeout = self.CONNECT_ROUTINE_TIMEOUT
 
-        if self.override_baudrate:
-            self._link.baudrate = self.override_baudrate
-            self._link.connect()
+        baudrates = [int(3e6), int(1e6)]
+        if self.override_baudrate is not None:
+            baudrates.append(self.override_baudrate)
+        baudrates.append(self.DEFAULT_BASE_BAUDRATE)
+        baudrates = sorted(list(set(baudrates)))
+
+        self._link.baudrate = baudrates[0]
+        self._link.connect()
+
+        for i, baudrate in enumerate(baudrates):
+            if i != 0:
+                self._link.baudrate = baudrate
+                sleep(0.2)
 
             try:
                 self._handshake()
-            except links.LinkError as e:
-                raise ClientError("could not connect, no response") from e
-        else:
-            baudrates = [int(3e6), int(1e6)]
-            baudrates.append(self.DEFAULT_BASE_BAUDRATE)
-            baudrates = sorted(list(set(baudrates)))
-
-            self._link.baudrate = baudrates[0]
-            self._link.connect()
-
-            for i, baudrate in enumerate(baudrates):
-                if i != 0:
-                    self._link.baudrate = baudrate
-                    sleep(0.2)
-
-                try:
-                    self._handshake()
-                except links.LinkError:
-                    log.debug("handshake failed at {} baud".format(baudrate))
-                else:
-                    log.debug("handshake succeeded at {} baud".format(baudrate))
-                    break
+            except links.LinkError:
+                log.debug("handshake failed at {} baud".format(baudrate))
             else:
-                raise ClientError("could not connect, no response")
-
-            product_max_baudrate = self._read_reg("product_max_uart_baudrate")
+                log.debug("handshake succeeded at {} baud".format(baudrate))
+                break
+        else:
+            raise ClientError("could not connect, no response")
 
-            if baudrate != product_max_baudrate:
-                log.debug("switching to {} baud...".format(product_max_baudrate))
-                self._write_reg("uart_baudrate", product_max_baudrate)
-                self._link.baudrate = product_max_baudrate
-                sleep(0.2)
-                self._handshake()
-                log.debug("handshake succeeded at {} baud".format(product_max_baudrate))
+        use_baudrate = (
+            self.override_baudrate
+            if self.override_baudrate is not None
+            else self._read_reg("product_max_uart_baudrate")
+        )
+
+        if baudrate != use_baudrate:
+            log.debug("switching to {} baud...".format(use_baudrate))
+            self._write_reg("uart_baudrate", use_baudrate)
+            self._link.baudrate = use_baudrate
+            sleep(0.2)
+            self._handshake()
+            log.debug("handshake succeeded at {} baud".format(use_baudrate))
 
         self._link.timeout = self._link.DEFAULT_TIMEOUT
 
         version_buffer = self._read_buf_raw()
         version_info = decode_version_buffer(version_buffer)
 
         info = {}
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
 import json
-from typing import Any, List, Optional, Type, Union
+from typing import Any, ClassVar, List, Optional, Type, Union
 
 import attrs
 
 from acconeer.exptool.a121._core.utils import pretty_dict_line_strs
 
 
 class ClientInfoCreationError(Exception):
     pass
 
 
+@attrs.frozen(slots=False)
 class ConnectionTypeBase(abc.ABC):
 
-    __registry: List[Type[ConnectionTypeBase]] = []
+    __registry: ClassVar[List[Type[ConnectionTypeBase]]] = []
 
     @classmethod
     def _register(cls, subclass: Type[ConnectionTypeBase]) -> Type[ConnectionTypeBase]:
         """Registers a subclass"""
         if not issubclass(subclass, cls):
             raise TypeError(f"{subclass.__name__!r} needs to be a subclass of {cls.__name__}.")
         cls.__registry.append(subclass)
@@ -62,15 +63,15 @@
 
     @property
     def mock(self) -> Optional[MockInfo]:
         return None
 
 
 @ConnectionTypeBase._register
-@attrs.frozen(kw_only=True)
+@attrs.frozen(kw_only=True, slots=False)
 class SerialInfo(ConnectionTypeBase):
     port: str
     override_baudrate: Optional[int] = None
     serial_number: Optional[str] = None
 
     @classmethod
     def _from_open(
@@ -91,15 +92,15 @@
 
     @property
     def serial(self) -> SerialInfo:
         return self
 
 
 @ConnectionTypeBase._register
-@attrs.frozen(kw_only=True)
+@attrs.frozen(kw_only=True, slots=False)
 class USBInfo(ConnectionTypeBase):
     vid: Optional[int] = None
     pid: Optional[int] = None
     serial_number: Optional[str] = None
 
     @classmethod
     def _from_open(
@@ -124,15 +125,15 @@
 
     @property
     def usb(self) -> USBInfo:
         return self
 
 
 @ConnectionTypeBase._register
-@attrs.frozen(kw_only=True)
+@attrs.frozen(kw_only=True, slots=False)
 class SocketInfo(ConnectionTypeBase):
     ip_address: str
     tcp_port: Optional[int]
 
     @classmethod
     def _from_open(
         cls,
@@ -150,15 +151,15 @@
 
     @property
     def socket(self) -> SocketInfo:
         return self
 
 
 @ConnectionTypeBase._register
-@attrs.frozen(kw_only=True)
+@attrs.frozen(kw_only=True, slots=True)
 class MockInfo(ConnectionTypeBase):
     @classmethod
     def _from_open(
         cls,
         ip_address: Optional[str] = None,
         tcp_port: Optional[int] = None,
         serial_port: Optional[str] = None,
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/mediators/recorder.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/mediators/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         ...
 
     @abc.abstractmethod
     def stop(self) -> Any:
         ...
 
 
+@attrs.mutable(slots=False)
 class AlgoBase:
     def to_dict(self) -> dict[str, Any]:
         return attrs.asdict(self)
 
     @classmethod
     def from_dict(cls: type[AlgoBaseT], d: dict[str, Any]) -> AlgoBaseT:
         return cls(**d)
@@ -81,14 +82,15 @@
         return json.dumps(self.to_dict(), cls=EntityJSONEncoder)
 
     @classmethod
     def from_json(cls: type[AlgoBaseT], json_str: str) -> AlgoBaseT:
         return cls.from_dict(json.loads(json_str))
 
 
+@attrs.mutable(slots=False)
 class AlgoConfigBase(AlgoBase, abc.ABC):
     def validate(self) -> None:
         """Performs self-validation
 
         :raises ValidationError: If anything is invalid.
         """
         for validation_result in self._collect_validation_results():
@@ -98,14 +100,15 @@
                 warnings.warn(vw.message)
 
     @abc.abstractmethod
     def _collect_validation_results(self) -> list[a121.ValidationResult]:
         pass
 
 
+@attrs.mutable(slots=False)
 class AlgoProcessorConfigBase(AlgoBase, abc.ABC):
     def validate(self, config: Union[a121.SensorConfig, a121.SessionConfig]) -> None:
         """Performs self-validation and validation of its session config
 
         :raises ValidationError: If anything is invalid.
         """
         if isinstance(config, a121.SensorConfig):
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,30 +65,30 @@
             raise HandledException("Could not load from file") from exc
 
         self._replaying_client = ApplicationClient.wrap(replaying_client, self.callback)
 
         self.start_session(with_recorder=False)
 
         self.send_status_message(f"<b>Replaying from {path.name}</b>")
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @abc.abstractmethod
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         pass
 
     @is_task
     def load_from_cache(self) -> None:
         try:
             with self.h5_cache_file() as f:
                 self._load_from_cache(f)
         except FileNotFoundError:
             pass
 
         self._sync_sensor_ids()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @abc.abstractmethod
     def _load_from_cache(self, file: h5py.File) -> None:
         pass
 
     @abc.abstractmethod
     def get_next(self) -> None:
@@ -126,15 +126,15 @@
     @abc.abstractmethod
     def _sync_sensor_ids(self) -> None:
         pass
 
     def attach_client(self, *, client: a121.Client) -> None:
         self._live_client = ApplicationClient.wrap(client, self.callback)
         self._sync_sensor_ids()
-        self.broadcast(True)
+        self.broadcast()
 
     def detach_client(self) -> None:
         self._live_client = None
 
     @abc.abstractmethod
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         pass
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,23 +199,23 @@
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = ProcessorBackendPluginSharedState(
             session_config=a121.SessionConfig(self.get_default_sensor_config()),
             processor_config=self.get_processor_config_cls()(),
         )
 
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         processor_preset = preset_config()
         self.shared_state.session_config = processor_preset.session_config
         self.shared_state.processor_config = processor_preset.processor_config
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def get_next(self) -> None:
         if self._processor_instance is None:
             raise RuntimeError("Processor is None. 'start' needs to be called before 'get_next'")
 
         assert self.client
         result = self.client.get_next()
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 
 from __future__ import annotations
 
 import abc
 import logging
 from typing import Generic, Optional, Type
 
-import qtawesome as qta
-
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo._base import ProcessorConfigT
 from acconeer.exptool.a121.algo._plugins._a121 import A121ViewPluginBase
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
-    GeneralMessage,
     GridGroupBox,
     MiscErrorView,
     PidgetFactoryMapping,
     PluginState,
     SessionConfigEditor,
     SmartMetadataView,
     SmartPerfCalcView,
+    icons,
 )
 
 from .backend_plugin import ProcessorBackendPluginSharedState
 
 
 log = logging.getLogger(__name__)
 
@@ -39,24 +36,16 @@
         super().__init__(app_model=app_model, view_widget=view_widget)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.start_button.clicked.connect(self._send_start_request)
         self.stop_button.clicked.connect(self._send_stop_request)
 
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
@@ -98,23 +87,14 @@
         )
 
     def _on_processor_config_update(self, processor_config: ProcessorConfigT) -> None:
         self.app_model.put_backend_plugin_task(
             "update_processor_config", {"processor_config": processor_config}
         )
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            log.debug(f"{type(self).__name__} syncing")
-
-            self.session_config_editor.sync()
-            self.processor_config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def on_backend_state_update(
         self,
         backend_plugin_state: Optional[
             ProcessorBackendPluginSharedState[ProcessorConfigT, a121.Metadata]
         ],
     ) -> None:
         if backend_plugin_state is None:
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 from enum import Enum, auto
 from typing import Any, Callable, Dict, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
@@ -30,15 +29,14 @@
     DetectorConfig,
     DetectorContext,
     DetectorResult,
 )
 from acconeer.exptool.a121.algo.distance._detector import _load_algo_data
 from acconeer.exptool.a121.algo.distance._detector_plugin import ViewPlugin as DistanceViewPlugin
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
     ConnectionState,
     GeneralMessage,
     GridGroupBox,
     HandledException,
     Message,
@@ -46,14 +44,15 @@
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     PluginStateMessage,
     TwoSensorIdsEditor,
+    icons,
     is_task,
     pidgets,
 )
 
 from ._configs import get_default_detector_config
 from ._processor import Processor, ProcessorConfig, ProcessorResult
 
@@ -134,15 +133,15 @@
             file["bilateration_config"][()]
         )
         self.shared_state.context = DetectorContext.from_h5(file["context"])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState(config=get_default_detector_config())
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             # Try to use the sensor ids from the last calibration
             if self.shared_state.context.sensor_ids:
@@ -168,15 +167,15 @@
         self.broadcast()
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config.detector_config
         self.shared_state.bilateration_config = preset_config.bilateration_config
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
         _create_h5_string_dataset(
             file, "bilateration_config", self.shared_state.bilateration_config.to_json()
         )
         context_group = file.create_group("context")
@@ -446,44 +445,28 @@
         super().__init__(app_model=app_model, view_widget=view_widget)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        self.calibrate_detector_button = QPushButton(
-            qta.icon("fa.circle", color=BUTTON_ICON_COLOR),
-            "Calibrate detector",
-            self.sticky_widget,
-        )
+        self.calibrate_detector_button = QPushButton(icons.CALIBRATE(), "Calibrate detector")
         self.calibrate_detector_button.clicked.connect(self._on_calibrate_detector)
 
-        self.defaults_button = QPushButton(
-            qta.icon("mdi6.restore", color=BUTTON_ICON_COLOR),
-            "Reset settings and calibrations",
-            self.sticky_widget,
-        )
+        self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
@@ -615,23 +598,14 @@
 
     def _on_processor_config_update(self, config: ProcessorConfig) -> None:
         self.app_model.put_backend_plugin_task("update_processor_config", {"config": config})
 
     def _on_sensor_ids_update(self, sensor_ids: list[int]) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_ids", {"sensor_ids": sensor_ids})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            log.debug(f"{type(self).__name__} syncing")
-
-            self.config_editor.sync()
-            self.bilateration_config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def _on_calibrate_detector(self) -> None:
         self.app_model.put_backend_plugin_task("calibrate_detector")
 
     def _send_defaults_request(self) -> None:
         self.app_model.put_backend_plugin_task("restore_defaults")
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,14 +284,25 @@
     """Used to limit step length. If no argument is provided, the step length is automatically
     calculated based on the profile."""
 
     max_profile: a121.Profile = attrs.field(default=a121.Profile.PROFILE_5, converter=a121.Profile)
     """Specifies the longest allowed profile. If no argument is provided, the highest possible
     profile without interference of direct leakage is used to maximize SNR."""
 
+    close_range_leakage_cancellation: bool = attrs.field(default=True)
+    """Enable close range leakage cancellation logic.
+
+    Close range leakage cancellation refers to the process of measuring close to the
+    sensor(<100mm) by first characterizing the direct leakage, and then subtracting it
+    from the measured sweep in order to isolate the signal component of interest.
+
+    The close range leakage cancellation process requires the sensor to be installed in its
+    intended geometry with free space in front of the sensor during detector calibration.
+    """
+
     signal_quality: float = attrs.field(default=15.0)
     """Signal quality. High quality equals higher HWAAS and better SNR but increase power
     consumption."""
 
     threshold_method: ThresholdMethod = attrs.field(
         default=ThresholdMethod.CFAR,
         converter=ThresholdMethod,
@@ -1016,15 +1027,15 @@
 
         # Determine shortest direct leakage free distance per profile
         min_dist_m = cls._calc_leakage_free_min_dist(config)
 
         close_range_transition_m = min_dist_m[a121.Profile.PROFILE_1]
 
         # Add close range group plan if applicable
-        if config.start_m < close_range_transition_m:
+        if config.close_range_leakage_cancellation and config.start_m < close_range_transition_m:
             plans[MeasurementType.CLOSE_RANGE] = cls._get_close_range_group_plan(
                 close_range_transition_m, config
             )
 
         # Define transition group plans
         transition_subgroup_plans = cls._get_transition_group_plans(
             config, min_dist_m, MeasurementType.CLOSE_RANGE in plans
@@ -1057,20 +1068,27 @@
         cls, transition_m: float, config: DetectorConfig
     ) -> list[SubsweepGroupPlan]:
         """Define the group plan for close range measurements.
 
         The close range measurement always use profile 1 to minimize direct leakage region.
         """
         profile = a121.Profile.PROFILE_1
+        # Select the end point as the shorter of the user provided end point or the transition
+        # point.
+        close_range_group_end_m = min(transition_m, config.end_m)
         # No left neighbour as this is the first subsweep when close range measurement is
         # applicable.
         has_neighbour = (False, transition_m < config.end_m)
         return [
             cls._create_group_plan(
-                profile, config, [config.start_m, transition_m], has_neighbour, True
+                profile,
+                config,
+                [config.start_m, close_range_group_end_m],
+                has_neighbour,
+                True,
             )
         ]
 
     @classmethod
     def _get_transition_group_plans(
         cls,
         config: DetectorConfig,
@@ -1082,33 +1100,48 @@
         The purpose of the transition group is to bridge the gap between the start point of the
         far measurement region and the point where max_profile can be used without interference
         of direct leakage.
 
         The transition region can consist of maximum two subsweeps, where the first utilize profile
         1 and the second profile 3. Whether both, one or none is used depends on the user provided
         detector config.
+
+        If close_range_leakage_cancellation is set to False, the first group plan should use
+        the user provided starting point as start, as there is no close range leakage cancellation
+        measurement.
         """
         transition_profiles = [
             profile
             for profile in [a121.Profile.PROFILE_1, a121.Profile.PROFILE_3]
             if profile.value < config.max_profile.value
         ]
         transition_profiles.append(config.max_profile)
 
         transition_subgroup_plans: list[SubsweepGroupPlan] = []
 
         for i in range(len(transition_profiles) - 1):
             profile = transition_profiles[i]
             next_profile = transition_profiles[i + 1]
 
-            if config.start_m < min_dist_m[next_profile] and min_dist_m[profile] < config.end_m:
+            is_first_group_plan = len(transition_subgroup_plans) == 0
+            start_m = None
+            if (
+                not config.close_range_leakage_cancellation
+                and is_first_group_plan
+                and config.start_m < min_dist_m[next_profile]
+            ):
+                start_m = config.start_m
+
+            elif config.start_m < min_dist_m[next_profile] and min_dist_m[profile] < config.end_m:
                 start_m = max(min_dist_m[profile], config.start_m)
+
+            if start_m is not None:
                 end_m = min(config.end_m, min_dist_m[next_profile])
                 has_neighbour = (
-                    has_close_range_measurement or len(transition_subgroup_plans) != 0,
+                    has_close_range_measurement or not is_first_group_plan,
                     min_dist_m[next_profile] < end_m,
                 )
 
                 transition_subgroup_plans.append(
                     cls._create_group_plan(profile, config, [start_m, end_m], has_neighbour, False)
                 )
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional, cast
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6.QtWidgets import QLabel, QPushButton, QTabWidget, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GridGroupBox,
     HandledException,
     Message,
@@ -38,14 +36,15 @@
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     PluginStateMessage,
     VerticalGroupBox,
+    icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components import CollapsibleWidget, SensorConfigEditor
 from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import (
     disable_if,
     enable_if,
@@ -70,22 +69,22 @@
 class SharedState:
     sensor_ids: list[int] = attrs.field(factory=lambda: [1])
     config: DetectorConfig = attrs.field(factory=DetectorConfig)
     context: DetectorContext = attrs.field(factory=DetectorContext)
 
 
 class PluginPresetId(Enum):
-    DEFAULT = auto()
+    BALANCED = auto()
     HIGH_ACCURACY = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
     PLUGIN_PRESETS: Mapping[int, Callable[[], DetectorConfig]] = {
-        PluginPresetId.DEFAULT.value: lambda: DetectorConfig(),
+        PluginPresetId.BALANCED.value: lambda: DetectorConfig(),
         PluginPresetId.HIGH_ACCURACY.value: lambda: get_high_accuracy_detector_config(),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
@@ -97,15 +96,15 @@
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = DetectorConfig.from_json(file["config"][()])
         self.shared_state.context = DetectorContext.from_h5(file["context"])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             # Try to use the sensor ids from the last calibration
             if self.shared_state.context.sensor_ids:
@@ -125,15 +124,15 @@
         self.shared_state.sensor_ids = sensor_ids
         self.broadcast()
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
         context_group = file.create_group("context")
         self.shared_state.context.to_h5(context_group)
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
@@ -327,44 +326,28 @@
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        self.calibrate_detector_button = QPushButton(
-            qta.icon("fa.circle", color=BUTTON_ICON_COLOR),
-            "Calibrate detector",
-            self.sticky_widget,
-        )
+        self.calibrate_detector_button = QPushButton(icons.CALIBRATE(), "Calibrate detector")
         self.calibrate_detector_button.clicked.connect(self._on_calibrate_detector)
 
-        self.defaults_button = QPushButton(
-            qta.icon("mdi6.restore", color=BUTTON_ICON_COLOR),
-            "Reset settings and calibrations",
-            self.sticky_widget,
-        )
+        self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
@@ -378,15 +361,15 @@
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
         sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
-        self.sensor_id_pidget.sig_parameter_changed.connect(self._on_sensor_id_update)
+        self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.config_editor = AttrsConfigEditor[DetectorConfig](
             title="Detector parameters",
             factory_mapping=self.get_pidget_mapping(),
             parent=self.scrolly_widget,
@@ -422,14 +405,17 @@
                 decimals=3,
             ),
             "end_m": pidgets.FloatPidgetFactory(
                 name_label_text="Range end",
                 suffix=" m",
                 decimals=3,
             ),
+            "close_range_leakage_cancellation": pidgets.CheckboxPidgetFactory(
+                name_label_text="Enable close range leakage cancellation"
+            ),
             "max_step_length": pidgets.OptionalIntPidgetFactory(
                 name_label_text="Max step length",
                 checkbox_label_text="Set",
                 limits=(1, None),
                 init_set_value=12,
             ),
             "max_profile": pidgets.EnumPidgetFactory(
@@ -537,15 +523,14 @@
             tab_visible = [False, False]
             for group in session_config.groups:
                 for _, sensor_config in group.items():
                     index = 0 if sensor_config.subsweeps[0].enable_loopback else 1
                     tab_visible[index] = True
                     sensor_config_editor = self.sensor_config_editors[index]
                     sensor_config_editor.set_data(sensor_config)
-                    sensor_config_editor.sync()
 
             for i, sensor_config_editor in enumerate(self.sensor_config_editors):
                 index = self.sensor_config_editor_tabs.indexOf(sensor_config_editor)
                 self.sensor_config_editor_tabs.setTabVisible(index, tab_visible[i])
 
             self.collapsible_widget.widget = self.sensor_config_editor_tabs
 
@@ -586,21 +571,14 @@
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_ids", {"sensor_ids": [sensor_id]})
 
     def _on_config_update(self, config: DetectorConfig) -> None:
         self.app_model.put_backend_plugin_task("update_config", {"config": config})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            self._log.debug(f"{type(self).__name__} syncing")
-            self.config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def _on_calibrate_detector(self) -> None:
         self.app_model.put_backend_plugin_task(
             "calibrate_detector", on_error=self.app_model.emit_error
         )
 
     def _send_defaults_request(self) -> None:
         self.app_model.put_backend_plugin_task("restore_defaults")
@@ -624,12 +602,12 @@
 DISTANCE_DETECTOR_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
     key="distance_detector",
     title="Distance detector",
     description="Easily measure distance to objects.",
     family=PluginFamily.DETECTOR,
     presets=[
-        PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
+        PluginPresetBase(name="Balanced", preset_id=PluginPresetId.BALANCED),
         PluginPresetBase(name="High accuracy", preset_id=PluginPresetId.HIGH_ACCURACY),
     ],
-    default_preset_id=PluginPresetId.DEFAULT,
+    default_preset_id=PluginPresetId.BALANCED,
 )
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/distance/_serializers.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/distance/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6 import QtCore
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
@@ -22,29 +21,29 @@
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GridGroupBox,
     Message,
     MiscErrorView,
     PidgetGroupFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     VerticalGroupBox,
+    icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import disable_if, parameter_is
 
 from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
 from ._detector import Detector, DetectorConfig, DetectorMetadata, DetectorResult, _load_algo_data
@@ -83,20 +82,20 @@
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = DetectorConfig.from_json(file["config"][()])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
@@ -109,15 +108,15 @@
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
@@ -409,28 +408,20 @@
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
@@ -440,15 +431,15 @@
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
         sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
-        self.sensor_id_pidget.sig_parameter_changed.connect(self._on_sensor_id_update)
+        self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.config_editor = AttrsConfigEditor[DetectorConfig](
             title="Detector parameters",
             factory_mapping=self._get_pidget_mapping(),
             parent=self.scrolly_widget,
@@ -633,22 +624,14 @@
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: DetectorConfig) -> None:
         self.app_model.put_backend_plugin_task("update_config", {"config": config})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            self._log.debug(f"{type(self).__name__} syncing")
-
-            self.config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def _send_defaults_request(self) -> None:
         self.app_model.put_backend_plugin_task("restore_defaults")
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/presence/_serializers.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/presence/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6 import QtCore
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
@@ -25,29 +24,29 @@
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
 from acconeer.exptool.a121.algo.presence._detector import Detector
 from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GridGroupBox,
     Message,
     MiscErrorView,
     PidgetGroupFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     VerticalGroupBox,
+    icons,
     is_task,
     pidgets,
 )
 
 from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
 from ._ref_app import RefApp, RefAppConfig, RefAppResult, _load_algo_data
 
@@ -95,25 +94,25 @@
 
         show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
         self.shared_state.config.show_all_detected_zones = show_all_detected_zones
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @is_task
     def update_plot_config(self, *, config: PlotConfig) -> None:
         self.shared_state.plot_config = config
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
@@ -128,15 +127,15 @@
         _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
         self.shared_state.plot_config = PlotConfig()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
@@ -402,28 +401,20 @@
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
@@ -433,15 +424,15 @@
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
         sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
-        self.sensor_id_pidget.sig_parameter_changed.connect(self._on_sensor_id_update)
+        self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.config_editor = AttrsConfigEditor[RefAppConfig](
             title="Ref App parameters",
             factory_mapping=self._get_pidget_mapping(),
             parent=self.scrolly_widget,
@@ -518,23 +509,14 @@
 
     def _on_config_update(self, config: RefAppConfig) -> None:
         self.app_model.put_backend_plugin_task("update_config", {"config": config})
 
     def _on_plot_config_update(self, config: PlotConfig) -> None:
         self.app_model.put_backend_plugin_task("update_plot_config", {"config": config})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            self._log.debug(f"{type(self).__name__} syncing")
-
-            self.config_editor.sync()
-            self.plot_config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def _send_defaults_request(self) -> None:
         self.app_model.put_backend_plugin_task("restore_defaults")
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files 15% similar despite different names*

```diff
@@ -133,16 +133,45 @@
             if not (
                 is_divisor_of(SPARSE_IQ_PPC, step_length)
                 or is_multiple_of(SPARSE_IQ_PPC, step_length)
             ):
                 raise ValueError(f"step_length must be a divisor or multiple of {SPARSE_IQ_PPC}")
 
     def _collect_validation_results(self) -> list[a121.ValidationResult]:
+        validation_results: list[a121.ValidationResult] = []
 
-        return []
+        if not self.sensor_angle < 90 or not self.sensor_angle > 0:
+            validation_results.append(
+                a121.ValidationError(
+                    self,
+                    "sensor_angle",
+                    "Sensor angle must be between 0 and 90 degrees",
+                )
+            )
+
+        optimal_distance = self.surface_distance / np.cos(np.radians(self.sensor_angle))
+        optimal_point = int(np.ceil(optimal_distance / APPROX_BASE_STEP_LENGTH_M))
+
+        start_point = int(
+            np.around(optimal_point - np.floor((self.num_points - 1) / 2) * self.step_length)
+        )
+
+        if start_point * APPROX_BASE_STEP_LENGTH_M <= self.surface_distance:
+            validation_results.append(
+                a121.ValidationError(
+                    self,
+                    "sensor_angle",
+                    (
+                        "Start point must be > surface distance. Increase sensor angle, "
+                        "decrease step length or decrease number of distance points"
+                    ),
+                )
+            )
+
+        return validation_results
 
 
 @attrs.frozen(kw_only=True)
 class ExampleAppResult:
     velocity: float = attrs.field()
     """Estimated velocity."""
 
@@ -214,25 +243,20 @@
         self.client.start_session(recorder)
 
         self.started = True
 
     @classmethod
     def _get_sensor_config(cls, config: ExampleAppConfig) -> a121.SensorConfig:
         optimal_distance = config.surface_distance / np.cos(np.radians(config.sensor_angle))
-        optimal_point = int(np.floor(optimal_distance / APPROX_BASE_STEP_LENGTH_M))
+        optimal_point = int(np.ceil(optimal_distance / APPROX_BASE_STEP_LENGTH_M))
 
-        start_point = int(np.around(optimal_point - (config.num_points / 2) * config.step_length))
-        if np.mod(config.num_points, 2) == 0:
-            end_point = int(
-                np.around(optimal_point + (config.num_points / 2 - 1) * config.step_length)
-            )
-        else:
-            end_point = int(
-                np.around(optimal_point + (config.num_points / 2) * config.step_length)
-            )
+        start_point = int(
+            np.around(optimal_point - np.floor((config.num_points - 1) / 2) * config.step_length)
+        )
+        end_point = start_point + (config.num_points - 1) * config.step_length
 
         if config.profile is not None:
             profile = config.profile
         else:
             viable_profiles = [
                 k
                 for k, v in cls.MIN_DIST_M.items()
@@ -256,15 +280,14 @@
             inter_sweep_idle_state=config.inter_sweep_idle_state,
         )
 
     @classmethod
     def _get_processor_config(cls, config: ExampleAppConfig) -> ProcessorConfig:
         return ProcessorConfig(
             surface_distance=config.surface_distance,
-            sensor_angle=config.sensor_angle,
             time_series_length=config.time_series_length,
             slow_zone=config.slow_zone,
             psd_lp_coeff=config.psd_lp_coeff,
             cfar_guard=config.cfar_guard,
             cfar_win=config.cfar_win,
             cfar_sensitivity=config.cfar_sensitivity,
             velocity_lp_coeff=config.velocity_lp_coeff,
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
     GridGroupBox,
     Message,
     MiscErrorView,
     PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     VerticalGroupBox,
+    icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 
 from ._example_app import ExampleApp, ExampleAppConfig, ExampleAppResult, _load_algo_data
 
@@ -77,20 +76,20 @@
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = ExampleAppConfig.from_json(file["config"][()])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
@@ -103,15 +102,15 @@
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
@@ -331,28 +330,20 @@
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
@@ -362,15 +353,15 @@
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
         sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
-        self.sensor_id_pidget.sig_parameter_changed.connect(self._on_sensor_id_update)
+        self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.range_helper = RangeHelpView()
         scrolly_layout.addWidget(self.range_helper)
 
         self.config_editor = AttrsConfigEditor[ExampleAppConfig](
@@ -542,22 +533,14 @@
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: ExampleAppConfig) -> None:
         self.app_model.put_backend_plugin_task("update_config", {"config": config})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            self._log.debug(f"{type(self).__name__} syncing")
-
-            self.config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     def _send_defaults_request(self) -> None:
         self.app_model.put_backend_plugin_task("restore_defaults")
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 import numpy as np
 import numpy.typing as npt
 import scipy
 from scipy.signal import welch
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo import AlgoProcessorConfigBase, ProcessorBase
-from acconeer.exptool.a121.algo._utils import PERCEIVED_WAVELENGTH, find_peaks, get_distances_m
+from acconeer.exptool.a121.algo._utils import (
+    APPROX_BASE_STEP_LENGTH_M,
+    PERCEIVED_WAVELENGTH,
+    find_peaks,
+    get_distances_m,
+)
 
 
 @attrs.mutable(kw_only=True)
 class ProcessorConfig(AlgoProcessorConfigBase):
     surface_distance: float = attrs.field(default=1)
-    sensor_angle: float = attrs.field(default=45)
     time_series_length: int = attrs.field(default=512)
     slow_zone: int = attrs.field(default=3)
     psd_lp_coeff: float = attrs.field(default=0.75)
     cfar_guard: int = attrs.field(default=6)
     cfar_win: int = attrs.field(default=6)
     cfar_sensitivity: float = attrs.field(default=0.15)
     velocity_lp_coeff: float = attrs.field(default=0.95)
@@ -48,14 +52,23 @@
                 a121.ValidationError(
                     config.sensor_config,
                     "sweep_rate",
                     "Must be set",
                 )
             )
 
+        if config.sensor_config.start_point * APPROX_BASE_STEP_LENGTH_M <= self.surface_distance:
+            validation_results.append(
+                a121.ValidationError(
+                    self,
+                    "start_point",
+                    "Start point must be > surface distance",
+                )
+            )
+
         return validation_results
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorContext:
     ...
 
@@ -122,15 +135,14 @@
             self.time_series_length = processor_config.time_series_length
 
         self.time_series = np.zeros(
             [self.time_series_length, self.num_distances], dtype=np.complex_
         )
 
         self.surface_distance = processor_config.surface_distance
-        self.sensor_angle = processor_config.sensor_angle
 
         if sensor_config.frame_rate is None:
             estimated_frame_rate = self.sweep_rate / self.sweeps_per_frame
         else:
             estimated_frame_rate = sensor_config.frame_rate
 
         self.max_peak_interval_n = processor_config.max_peak_interval_s * estimated_frame_rate
@@ -191,19 +203,17 @@
             freqs = scipy.fft.fftshift(freqs)
             psd = scipy.fft.fftshift(psd)
             psds.append(psd)
 
         return np.array(psds).T, freqs
 
     def get_angle_correction(self, distance: float) -> float:
-        if (self.surface_distance / distance) < 1 and (self.surface_distance / distance) > -1:
-            insonation_angle = np.arcsin(self.surface_distance / distance)
-            angle_correction = 1 / np.cos(insonation_angle)
-        else:
-            angle_correction = 1
+        # distanca > self.surface_distance is checked in sensor config
+        insonation_angle = np.arcsin(self.surface_distance / distance)
+        angle_correction = 1 / np.cos(insonation_angle)
 
         return angle_correction  # type: ignore[no-any-return]
 
     def get_distance_idx(self, psds: npt.NDArray[np.float_]) -> int:
         max_negative_side = np.max(psds[self.middle_idx + self.slow_zone :, :], axis=0)
         max_positive_side = np.max(psds[: self.middle_idx - self.slow_zone, :], axis=0)
         max_amps = np.maximum(max_negative_side, max_positive_side)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
-import qtawesome as qta
 
 from PySide6.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
@@ -36,38 +35,39 @@
     RefApp,
     RefAppConfig,
     RefAppContext,
     RefAppResult,
     _load_algo_data,
 )
 from acconeer.exptool.app.new import (
-    BUTTON_ICON_COLOR,
     AppModel,
     BackendLogger,
     GeneralMessage,
     HandledException,
     Message,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     PluginStateMessage,
     VerticalGroupBox,
+    icons,
     is_task,
 )
 from acconeer.exptool.app.new.ui.plugin_components import (
     AttrsConfigEditor,
     GridGroupBox,
     PidgetFactoryMapping,
     pidgets,
 )
 
 
 NO_DETECTION_TIMEOUT = 50
+TIME_HISTORY_S = 30
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
     config: RefAppConfig = attrs.field(factory=RefAppConfig)
     context: RefAppContext = attrs.field(factory=RefAppContext)
@@ -113,15 +113,15 @@
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = RefAppConfig.from_json(file["config"][()])
         self.shared_state.context = RefAppContext.from_h5(file["context"])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState(config=get_small_config())
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
@@ -136,15 +136,15 @@
         self.shared_state.sensor_id = sensor_id
         self.broadcast()
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config.config
-        self.broadcast(sync=True)
+        self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
         context_group = file.create_group("context")
         self.shared_state.context.to_h5(context_group)
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
@@ -392,31 +392,32 @@
 
         self.sweep_plot.setYRange(0, self.sweep_smooth_max.update(max_val_in_plot))
         self.vertical_line_start.setValue(self.start_m)
         self.vertical_line_end.setValue(self.end_m)
         self.vertical_line_start.show()
         self.vertical_line_end.show()
 
+        # update level history plot
+        if any(~np.isnan(time_and_level_dict["level"])):
+            self.level_history_curve.setData(
+                time_and_level_dict["time"], time_and_level_dict["level"] * 100
+            )
+            self.level_history_plot.setXRange(-TIME_HISTORY_S + 1, 0)
+            self.level_history_plot.setYRange(0, (self.end_m - self.start_m + 0.01) * 100)
+
+        # update level plot
         if (
             result.level is not None
             and result.peak_detected is not None
             and result.peak_status is not None
         ):
             current_level = result.level
             peak_detected = result.peak_detected
             peak_status = result.peak_status
-            # update level history plot
-            if any(~np.isnan(time_and_level_dict["level"])):
-                self.level_history_curve.setData(
-                    time_and_level_dict["time"], time_and_level_dict["level"] * 100
-                )
-                self.level_history_plot.setXRange(-30 + 1, 0)
-                self.level_history_plot.setYRange(0, (self.end_m - self.start_m + 0.01) * 100)
 
-            # update level plot
             level_text = self.STATUS_MSG_MAP[peak_status]
             if peak_status == ProcessorLevelStatus.OVERFLOW:
                 for rect in self.rects:
                     rect.setBrush(et.utils.pg_brush_cycler(0))
             elif peak_detected and (peak_status == ProcessorLevelStatus.IN_RANGE):
                 self.bar_loc = round(current_level / (self.end_m - self.start_m) * self.num_rects)
                 for rect in self.rects[: self.bar_loc]:
@@ -470,44 +471,28 @@
         self._log = logging.getLogger(__name__)
 
         sticky_layout = QVBoxLayout()
         sticky_layout.setContentsMargins(0, 0, 0, 0)
         scrolly_layout = QVBoxLayout()
         scrolly_layout.setContentsMargins(0, 0, 0, 0)
 
-        self.start_button = QPushButton(
-            qta.icon("fa5s.play-circle", color=BUTTON_ICON_COLOR),
-            "Start measurement",
-            self.sticky_widget,
-        )
+        self.start_button = QPushButton(icons.PLAY(), "Start measurement")
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.start_button.clicked.connect(self._send_start_request)
 
-        self.stop_button = QPushButton(
-            qta.icon("fa5s.stop-circle", color=BUTTON_ICON_COLOR),
-            "Stop",
-            self.sticky_widget,
-        )
+        self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        self.calibrate_detector_button = QPushButton(
-            qta.icon("fa.circle", color=BUTTON_ICON_COLOR),
-            "Calibrate detector",
-            self.sticky_widget,
-        )
+        self.calibrate_detector_button = QPushButton(icons.CALIBRATE(), "Calibrate detector")
         self.calibrate_detector_button.clicked.connect(self._on_calibrate_detector)
 
-        self.defaults_button = QPushButton(
-            qta.icon("mdi6.restore", color=BUTTON_ICON_COLOR),
-            "Reset settings and calibrations",
-            self.sticky_widget,
-        )
+        self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
         button_group = GridGroupBox("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
@@ -518,15 +503,15 @@
 
         sticky_layout.addWidget(button_group)
 
         sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
-        self.sensor_id_pidget.sig_parameter_changed.connect(self._on_sensor_id_update)
+        self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.tank_level_config_editor = AttrsConfigEditor[RefAppConfig](
             title="Tank level indicator parameters",
             factory_mapping=self._get_processor_pidget_mapping(),
             parent=self.scrolly_widget,
@@ -669,23 +654,14 @@
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
 
     def _on_config_update(self, config: RefAppConfig) -> None:
         self.app_model.put_backend_plugin_task("update_config", {"config": config})
 
-    def handle_message(self, message: GeneralMessage) -> None:
-        if message.name == "sync":
-            self._log.debug(f"{type(self).__name__} syncing")
-
-            self.config_editor.sync()
-            self.tank_level_config_editor.sync()
-        else:
-            raise RuntimeError("Unknown message")
-
     # TODO: move to detector base (?)
     def _send_start_request(self) -> None:
         self.app_model.put_backend_plugin_task(
             "start_session",
             {"with_recorder": self.app_model.recording_enabled},
             on_error=self.app_model.emit_error,
         )
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/tank_level/_serializer.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/tank_level/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,21 +20,21 @@
     Message,
     PluginStateMessage,
     is_task,
 )
 from .pluginbase import PlotPluginBase, PluginPresetBase, PluginSpecBase, ViewPluginBase
 from .storage import get_temp_dir, get_temp_h5_path
 from .ui import (
-    BUTTON_ICON_COLOR,
     AttrsConfigEditor,
     GridGroupBox,
     HorizontalGroupBox,
     MiscErrorView,
     PidgetFactoryMapping,
     PidgetGroupFactoryMapping,
     SessionConfigEditor,
     SmartMetadataView,
     SmartPerfCalcView,
     TwoSensorIdsEditor,
     VerticalGroupBox,
+    icons,
     pidgets,
 )
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
 from contextlib import contextmanager
 from typing import Any, Callable, Generic, Optional, TypeVar
 
 import h5py
 
 from acconeer.exptool.app.new import PluginGeneration
 from acconeer.exptool.app.new.storage import get_config_dir
 
-from ._message import BackendPluginStateMessage, GeneralMessage, Message, StatusMessage
+from ._message import BackendPluginStateMessage, Message, StatusMessage
 
 
 StateT = TypeVar("StateT")
 
 
 class BackendPlugin(abc.ABC, Generic[StateT]):
     shared_state: StateT
@@ -62,15 +62,12 @@
     def teardown(self) -> None:
         pass
 
     @abc.abstractmethod
     def set_preset(self, preset_id: int) -> None:
         pass
 
-    def broadcast(self, sync: bool = False) -> None:
+    def broadcast(self) -> None:
         self.callback(BackendPluginStateMessage(state=self.shared_state))
 
-        if sync:
-            self.callback(GeneralMessage(name="sync", recipient="view_plugin"))
-
     def send_status_message(self, message: Optional[str]) -> None:
         self.callback(StatusMessage(status=message))
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,21 @@
     from acconeer.exptool.a121.algo.surface_velocity._example_app_plugin import (
         SURFACE_VELOCITY_PLUGIN,
     )
     from acconeer.exptool.a121.algo.tank_level._plugin import TANK_LEVEL_PLUGIN
     from acconeer.exptool.a121.algo.touchless_button._plugin import TOUCHLESS_BUTTON_PLUGIN
     from acconeer.exptool.a121.algo.vibration._plugin import VIBRATION_PLUGIN
 
+    # Please keep in lexicographical order
     return [
-        SPARSE_IQ_PLUGIN,
+        BILATERATION_PLUGIN,
+        BREATHING_PLUGIN,
         DISTANCE_DETECTOR_PLUGIN,
         PHASE_TRACKING_PLUGIN,
         PRESENCE_DETECTOR_PLUGIN,
-        TOUCHLESS_BUTTON_PLUGIN,
-        VIBRATION_PLUGIN,
-        BILATERATION_PLUGIN,
-        BREATHING_PLUGIN,
         SMART_PRESENCE_PLUGIN,
-        TANK_LEVEL_PLUGIN,
+        SPARSE_IQ_PLUGIN,
         SURFACE_VELOCITY_PLUGIN,
+        TANK_LEVEL_PLUGIN,
+        TOUCHLESS_BUTTON_PLUGIN,
+        VIBRATION_PLUGIN,
     ]
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,17 +46,16 @@
         return self._sticky_widget
 
     @property
     def scrolly_widget(self) -> QWidget:
         """The scrolly widget. The scrolly area is located below the sticky area"""
         return self._scrolly_widget
 
-    @abc.abstractmethod
     def handle_message(self, message: GeneralMessage) -> None:
-        pass
+        raise RuntimeError("ViewPlugins does not expect any messages ATM.")
 
     def _send_start_request(self) -> None:
         self.app_model.put_backend_plugin_task(
             "start_session",
             {"with_recorder": self.app_model.recording_enabled},
             on_error=self.app_model.emit_error,
         )
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/connection_widget.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-import qtawesome as qta
-
 from PySide6 import QtCore
 from PySide6.QtGui import QRegularExpressionValidator
 from PySide6.QtWidgets import (
     QCheckBox,
     QComboBox,
     QDialog,
     QHBoxLayout,
@@ -19,16 +17,16 @@
     QVBoxLayout,
     QWidget,
 )
 
 from acconeer.exptool.app.new._enums import ConnectionInterface, ConnectionState
 from acconeer.exptool.app.new.app_model import AppModel
 from acconeer.exptool.app.new.qt_subclasses import AppModelAwareWidget
-
-from .misc import BUTTON_ICON_COLOR, SerialPortComboBox, USBDeviceComboBox
+from acconeer.exptool.app.new.ui.device_comboboxes import SerialPortComboBox, USBDeviceComboBox
+from acconeer.exptool.app.new.ui.icons import COG, LINK, UNLINK
 
 
 class _ConnectAndDisconnectButton(QPushButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.app_model = app_model
@@ -52,33 +50,33 @@
             ConnectionState.DISCONNECTED: "Connect",
             ConnectionState.CONNECTING: "Connecting...",
             ConnectionState.CONNECTED: "Disconnect",
             ConnectionState.DISCONNECTING: "Disconnecting...",
         }
         ENABLED_STATES = {ConnectionState.CONNECTED, ConnectionState.DISCONNECTED}
         ICONS = {
-            ConnectionState.DISCONNECTED: "fa5s.link",
-            ConnectionState.CONNECTING: "fa5s.link",
-            ConnectionState.CONNECTED: "fa5s.unlink",
-            ConnectionState.DISCONNECTING: "fa5s.unlink",
+            ConnectionState.DISCONNECTED: LINK(),
+            ConnectionState.CONNECTING: LINK(),
+            ConnectionState.CONNECTED: UNLINK(),
+            ConnectionState.DISCONNECTING: UNLINK(),
         }
         TOOLTIPS = {
             ConnectionState.DISCONNECTED: "Connect to device using specified interface",
             ConnectionState.CONNECTING: "Connecting...",
             ConnectionState.CONNECTED: "Disconnect the device",
             ConnectionState.DISCONNECTING: "Disconnecting...",
         }
 
         self.setText(TEXTS[app_model.connection_state])
         self.setEnabled(
             app_model.connection_state in ENABLED_STATES
             and app_model.plugin_state.is_steady
             and app_model.is_connect_ready()
         )
-        self.setIcon(qta.icon(ICONS[app_model.connection_state], color=BUTTON_ICON_COLOR))
+        self.setIcon(ICONS[app_model.connection_state])
         self.setToolTip(TOOLTIPS[app_model.connection_state])
 
 
 class _SocketConnectionWidget(AppModelAwareWidget):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(app_model, parent)
         self.app_model = app_model
@@ -117,15 +115,15 @@
 
 
 class _ConnectSettingsButton(QPushButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent, flat=True)
         self.app_model = app_model
 
-        self.setIcon(qta.icon("fa5s.cog", color=BUTTON_ICON_COLOR))
+        self.setIcon(COG())
         self.setToolTip("Advanced settings")
 
         self.settings_dialog = _ConnectSettingsDialog(app_model, self)
 
         app_model.sig_notify.connect(self._on_app_model_update)
         self.clicked.connect(self._on_click)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
-from typing import Optional
-
-from PySide6.QtWidgets import QFrame, QHBoxLayout, QMainWindow, QSplitter, QVBoxLayout, QWidget
+from PySide6.QtWidgets import QFrame, QHBoxLayout, QSplitter, QVBoxLayout, QWidget
 
 from acconeer.exptool.app.new.app_model import AppModel
+from acconeer.exptool.app.new.ui.misc import VerticalSeparator
 
 from .connection_widget import ClientConnectionWidget, GenerationSelection
-from .flash_widget import FlashButton
-from .misc import ExceptionWidget, HintWidget, VerticalSeparator
+from .hints import HintWidget
 from .plugin_widget import PluginControlArea, PluginPlotArea, PluginSelectionArea
 from .recording_widget import RecordingWidget
-from .status_bar import StatusBar
-
-
-class MainWindow(QMainWindow):
-    def __init__(self, app_model: AppModel) -> None:
-        super().__init__()
-
-        self.resize(1280, 720)
 
-        self.setCentralWidget(MainWindowCentralWidget(app_model, self))
-        self.setStatusBar(StatusBar(app_model, self))
-        self.setWindowTitle("Acconeer Exploration Tool")
-        self.moveEvent = lambda _: self.saveGeometry()
 
-        app_model.sig_error.connect(self.on_app_model_error)
-
-    def on_app_model_error(self, exception: Exception, traceback_str: Optional[str]) -> None:
-        ExceptionWidget(self, exc=exception, traceback_str=traceback_str).exec()
-
-
-class MainWindowCentralWidget(QWidget):
+class StreamingMainWidget(QWidget):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(0)
 
@@ -59,16 +39,14 @@
         self.setStyleSheet("QFrame#TopBar {background: #ebebeb;}")
 
         self.setLayout(QHBoxLayout(self))
 
         self.layout().addWidget(GenerationSelection(app_model, self))
         self.layout().addWidget(VerticalSeparator(self))
         self.layout().addWidget(ClientConnectionWidget(app_model, self))
-        self.layout().addWidget(VerticalSeparator(self))
-        self.layout().addWidget(FlashButton(app_model, self))
         self.layout().addWidget(HintWidget(app_model, self))
         self.layout().addStretch(1)
         self.layout().addWidget(RecordingWidget(app_model, self))
 
 
 class WorkingArea(QSplitter):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,318 +1,298 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-import abc
-import platform
-import webbrowser
-from typing import List, Optional
+import threading
+from typing import Optional
 
-import pyperclip
+import numpy as np
 import qtawesome as qta
 
-from PySide6 import QtCore, QtGui
+from PySide6 import QtCore
+from PySide6.QtGui import QPainter, QPaintEvent, QTextDocument
 from PySide6.QtWidgets import (
-    QComboBox,
-    QFrame,
     QHBoxLayout,
     QLabel,
-    QMessageBox,
-    QPushButton,
+    QMainWindow,
+    QStatusBar,
+    QStyle,
+    QStyleOption,
+    QTextBrowser,
     QWidget,
 )
 
-from acconeer.exptool.app.new._enums import ConnectionInterface
-from acconeer.exptool.app.new._exceptions import HandledException
+import acconeer.exptool
+from acconeer.exptool.app.new import check_package_outdated, get_latest_changelog
 from acconeer.exptool.app.new.app_model import AppModel
-from acconeer.exptool.utils import CommDevice  # type: ignore[import]
+from acconeer.exptool.utils import get_module_version  # type: ignore[import]
 
+from .icons import BUTTON_ICON_COLOR, REFRESH
 
-BUTTON_ICON_COLOR = "#0081db"
 
-
-class ExceptionWidget(QMessageBox):
-    def __init__(
-        self,
-        parent: QWidget,
-        *,
-        exc: Exception,
-        traceback_str: Optional[str] = None,
-        title: str = "Error",
-    ) -> None:
+class FrameCountLabel(QLabel):
+    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
-        self.setIcon(QMessageBox.Warning)
-        self.setStandardButtons(QMessageBox.Ok)
+        self.setToolTip("Number of received frames")
 
-        self.setWindowTitle(title)
-        self.setText(str(exc))
+        app_model.sig_frame_count.connect(self._on_app_model_frame_count)
+        self._on_app_model_frame_count(None)
 
-        try:
-            raise exc
-        except HandledException:
-            pass
-        except Exception:
-            self.setInformativeText("<b>Unhandled error - please file a bug</b>")
-
-        if traceback_str:
-            self.setDetailedText(traceback_str)
-            copy_button = QPushButton(self)
-            copy_button.setText("Copy details")
-            self.addButton(copy_button, QMessageBox.ButtonRole.ActionRole)
-            copy_button.clicked.disconnect()
-            copy_button.clicked.connect(self._on_copy_clicked)
-
-    def resizeEvent(self, event: QtGui.QResizeEvent) -> None:
-        super().resizeEvent(event)
-        self.setFixedWidth(500)
-
-    def _on_copy_clicked(self) -> None:
-        detailed_text = self.detailedText()
-        if detailed_text:
-            pyperclip.copy(detailed_text)
+    def _on_app_model_frame_count(self, frame_count: Optional[int]) -> None:
+        if frame_count is None:
+            css = "color: #888;"
+            text = "Frames: -    "
+        else:
+            css = ""
+            text = f"Frames: {frame_count:5}"
 
-    def closeEvent(self, event: QtGui.QCloseEvent) -> None:
-        self.close()
+        self.setStyleSheet(f"QWidget{{{css}}}")
+        self.setText(text)
 
 
-class VerticalSeparator(QWidget):
-    def __init__(self, parent: QWidget) -> None:
+class RateStatsLabel(QLabel):
+    _FPS: int = 10
+
+    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
-        self.setLayout(QHBoxLayout(self))
-        self.layout().setContentsMargins(5, 5, 5, 5)
+        self.setToolTip("Reported update rate")
 
-        frame = QFrame(self)
-        frame.setFrameShape(QFrame.VLine)
-        self.layout().addWidget(frame)
+        self.rate = np.nan
+        self.rate_warning = False
 
+        self.startTimer(int(1000 / self._FPS))
 
-class CommDeviceComboBox(QComboBox):
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
-        self.app_model = app_model
-        app_model.sig_notify.connect(self._on_app_model_update)
-        self.currentTextChanged.connect(self._on_change)
-        self.setMinimumWidth(175)
+        app_model.sig_rate_stats.connect(self._on_app_model_rate_stats)
 
-    def _on_app_model_update(self, app_model: AppModel) -> None:
-        devices = self._get_available_devices()
+    def timerEvent(self, event: QtCore.QTimerEvent) -> None:
+        if np.isnan(self.rate):
+            css = "color: #888;"
+            text = "     - Hz"
+        else:
+            css = "color: #FD5200;" if self.rate_warning else ""
+            text = f"{self.rate:>6.1f} Hz"
 
-        view_ports = [self.itemData(i) for i in range(self.count())]
+        self.setStyleSheet(f"QWidget{{{css}}}")
+        self.setText(text)
 
-        with QtCore.QSignalBlocker(self):
-            if devices != view_ports:
-                self.clear()
-                for device in devices:
-                    self.addItem(device.display_name(), device)
+    def _on_app_model_rate_stats(
+        self,
+        rate: float,
+        rate_warning: bool,
+        jitter: float,
+        jitter_warning: bool,
+    ) -> None:
+        self.rate = rate
+        self.rate_warning = rate_warning
 
-            current_device = self._get_current_device()
 
-            # QComboBox.findData can't be used since since it doesn't
-            # always match different but content wise identical objects.
-            index = -1
-            for i in range(self.count()):
-                if self.itemData(i) == current_device:
-                    index = i
-                    break
-            self.setCurrentIndex(index)
+class JitterStatsLabel(QLabel):
+    _FPS: int = 10
 
-            self.setEnabled(self.count() > 0)
-            if self.count() == 0:
-                self.addItem("No device available")
+    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
+        super().__init__(parent)
 
-    @abc.abstractmethod
-    def _on_change(self) -> None:
-        pass
+        self.setToolTip("Reported jitter")
 
-    @abc.abstractmethod
-    def _get_available_devices(self) -> List[CommDevice]:
-        pass
+        self.jitter = np.nan
+        self.jitter_warning = False
 
-    @abc.abstractmethod
-    def _get_current_device(self) -> Optional[CommDevice]:
-        pass
+        self.startTimer(int(1000 / self._FPS))
 
+        app_model.sig_rate_stats.connect(self._on_app_model_rate_stats)
 
-class SerialPortComboBox(CommDeviceComboBox):
-    def _on_change(self) -> None:
-        self.app_model.set_serial_connection_device(self.currentData())
+    def timerEvent(self, event: QtCore.QTimerEvent) -> None:
+        if np.isnan(self.jitter):
+            css = "color: #888;"
+            text = "    - ms"
+        else:
+            css = "color: #FD5200;" if self.jitter_warning else ""
+            text = f"{self.jitter * 1e3:5.1f} ms"
 
-    def _get_available_devices(self) -> List[CommDevice]:
-        return self.app_model.available_serial_devices
+        self.setStyleSheet(f"QWidget{{{css}}}")
+        self.setText(text)
 
-    def _get_current_device(self) -> Optional[CommDevice]:
-        return self.app_model.serial_connection_device
+    def _on_app_model_rate_stats(
+        self,
+        rate: float,
+        rate_warning: bool,
+        jitter: float,
+        jitter_warning: bool,
+    ) -> None:
+        self.jitter = jitter
+        self.jitter_warning = jitter_warning
 
 
-class USBDeviceComboBox(CommDeviceComboBox):
-    def _on_change(self) -> None:
-        self.app_model.set_usb_connection_device(self.currentData())
+class BackendCPUPercentLabel(QLabel):
+    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
+        super().__init__(parent)
 
-    def _get_available_devices(self) -> List[CommDevice]:
-        return self.app_model.available_usb_devices
+        self.setToolTip("Client process CPU load")
 
-    def _get_current_device(self) -> Optional[CommDevice]:
-        return self.app_model.usb_connection_device
+        app_model.sig_backend_cpu_percent.connect(self._on_app_model_backend_cpu_percent)
 
+        self._on_app_model_backend_cpu_percent(0)
 
-class HintObject:
-    def __init__(self, warning: str, tooltip: str, how_to_fix_url: str) -> None:
-        self.warning = warning
-        self.tooltip = tooltip
-        self.how_to_fix_url = how_to_fix_url
+    def _on_app_model_backend_cpu_percent(self, cpu_percent: int) -> None:
+        self.setText(f"CPU: {cpu_percent:3}%")
 
-    @staticmethod
-    @abc.abstractmethod
-    def _should_show(app_model: AppModel) -> bool:
-        pass
+        css = "color: #FD5200;" if cpu_percent >= 85 else ""
+        self.setStyleSheet(f"QWidget{{{css}}}")
 
 
-class UserHintWidget(QWidget):
+class RSSVersionLabel(QLabel):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
-        app_model.sig_notify.connect(self._on_app_model_update)
 
-        self._hints: List[HintObject] = []
-        self._how_to_fix_url: Optional[str] = None
+        app_model.sig_notify.connect(self._on_app_model_update)
 
-        self.setLayout(QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
+    def _on_app_model_update(self, app_model: AppModel) -> None:
+        if app_model.rss_version is None:
+            css = "color: #888;"
+            text = "RSS: <not connected>"
+            tooltip = ""
+        else:
+            text = f"RSS: {app_model.rss_version}"
+
+            if app_model.connection_warning:
+                css = "background-color: #D78100; color: #e2e2e2;"
+                tooltip = app_model.connection_warning
+            else:
+                css = ""
+                tooltip = ""
+
+        self.setToolTip(tooltip)
+        self.setStyleSheet(f"QWidget{{{css}}}")
+        self.setText(text)
 
-        self.icon = qta.IconWidget()
-        self.icon.setHidden(True)
-        self.icon.setIcon(qta.icon("fa.warning", color="#ff9e00"))
-        self.layout().addWidget(self.icon)
-
-        self.label = QLabel(self)
-        self.label.setHidden(True)
-        self.layout().addWidget(self.label)
-
-        self.button = QPushButton(self)
-        self.button.setIcon(qta.icon("fa5s.external-link-alt", color=BUTTON_ICON_COLOR))
-        self.button.setText("How to fix")
-        self.button.clicked.connect(self._on_click)
-        self.button.setHidden(True)
-        self.layout().addWidget(self.button)
 
-    def add_hint(self, hint: HintObject) -> None:
-        self._hints.append(hint)
+class VersionLabel(QWidget):
+    sig_version_outdated = QtCore.Signal()
 
-    def _on_app_model_update(self, app_model: AppModel) -> None:
-        for hint in self._hints:
-            if hint._should_show(app_model):
-                self.label.setText(hint.warning)
-                self.label.setToolTip(hint.tooltip)
-                self.icon.setToolTip(hint.tooltip)
-                self._how_to_fix_url = hint.how_to_fix_url
-                self.icon.setHidden(False)
-                self.label.setHidden(False)
-                if self._how_to_fix_url is not None:
-                    self.button.setHidden(False)
-                return
-
-        self.icon.setHidden(True)
-        self.label.setHidden(True)
-        self.button.setHidden(True)
-
-    def _on_click(self) -> None:
-        if self._how_to_fix_url is not None:
-            webbrowser.open_new_tab(self._how_to_fix_url)
-
-
-class ConnectionHint(HintObject):
-    def __init__(self) -> None:
-        super().__init__(
-            "Stability warning",
-            "You may experience stability issues due to windows serial port driver",
-            r"https://docs.acconeer.com/en/latest/evk_setup/xc120_xe121.html",
-        )
-
-    @staticmethod
-    def _should_show(app_model: AppModel) -> bool:
-        if platform.system().lower() != "windows":
-            return False
-
-        if (
-            app_model.serial_connection_device is not None
-            and app_model.connection_interface == ConnectionInterface.SERIAL
-        ):
-            if app_model.serial_connection_device.name is not None:
-                if app_model.serial_connection_device.unflashed:
-                    return False
-                return "xc120" in app_model.serial_connection_device.name.lower()
-
-        return False
-
-
-class UnflashedDeviceHint(HintObject):
-    def __init__(self) -> None:
-        super().__init__(
-            "Unflashed device",
-            "The device needs to be flashed with exploration server firmware",
-            r"https://docs.acconeer.com/en/latest/evk_setup/xc120_xe121.html",
-        )
-
-    @staticmethod
-    def _should_show(app_model: AppModel) -> bool:
-        if app_model.connection_interface not in [
-            ConnectionInterface.SERIAL,
-            ConnectionInterface.USB,
-        ]:
-            return False
-
-        if (
-            app_model.serial_connection_device is not None
-            and app_model.connection_interface == ConnectionInterface.SERIAL
-            and app_model.serial_connection_device.unflashed
-        ):
-            return True
-
-        if (
-            app_model.usb_connection_device is not None
-            and app_model.connection_interface == ConnectionInterface.USB
-            and app_model.usb_connection_device.unflashed
-        ):
-            return True
-
-        return False
-
-
-class InaccessibleDeviceHint(HintObject):
-    def __init__(self) -> None:
-        super().__init__(
-            "Device permissions",
-            "The USB device permissions needs to be setup, "
-            "update USB permissions or use Serial Port",
-            r"https://docs.acconeer.com/en/latest/exploration_tool/"
-            "installation_and_setup.html#linux-setup",
-        )
-
-    @staticmethod
-    def _should_show(app_model: AppModel) -> bool:
-        if (
-            app_model.usb_connection_device is not None
-            and app_model.connection_interface == ConnectionInterface.USB
-            and not app_model.usb_connection_device.accessible
-        ):
-            return True
+    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
+        super().__init__(parent)
 
-        return False
+        self.parent = parent
+        h_layout = QHBoxLayout()
+        self.setLayout(h_layout)
+        h_layout.setContentsMargins(0, 0, 0, 0)
+        h_layout.setSpacing(0)
+
+        et_version = get_module_version(acconeer.exptool)
+        et_version_text = f"ET: {et_version}"
+        et_version_label = QLabel(et_version_text, self)
+        h_layout.addWidget(et_version_label)
+
+        def version_check(et_version: str) -> None:
+            version_outdated, latest_v = check_package_outdated("acconeer-exptool", et_version)
+            self.changelog = None
+
+            if version_outdated:
+                self.changelog = get_latest_changelog()
+                self.setStyleSheet(
+                    f"QWidget{{background-color: {BUTTON_ICON_COLOR}; color: #e2e2e2}}"
+                )
+
+                self.setToolTip(
+                    "There is a new software version available!\n"
+                    f"The latest version is: {latest_v}. \n"
+                    "Click to view changelog."
+                )
+                self.sig_version_outdated.emit()
+                self.mousePressEvent = self._toggle_changelog
+
+        self.sig_version_outdated.connect(self._create_changelog_window)
+        self.sig_version_outdated.connect(lambda: self._add_icon_to_version_label(self))
+
+        version_thread = threading.Thread(target=lambda: version_check(et_version))
+        version_thread.start()
+
+    def _create_changelog_window(self) -> None:
+        if self.changelog is not None:
+            self.cl_window = ChangelogWindow(self)
+            self.cl_window.set_text(self.changelog)
+
+    def _add_icon_to_version_label(self, version_widget: QWidget) -> None:
+        layout = version_widget.layout()
+        icon_widget = qta.IconWidget()
+        icon_widget.setIcon(REFRESH(color="#e2e2e2"))
+        layout.addWidget(icon_widget)
+
+    def _toggle_changelog(self, label: QLabel) -> None:
+        if self.changelog is not None:
+            self.cl_window.setVisible(not self.cl_window.isVisible())
+
+    def paintEvent(self, pe: QPaintEvent) -> None:
+        o = QStyleOption()
+        o.initFrom(self)
+        p = QPainter(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, o, p, self)
 
 
-class HintWidget(QWidget):
+class StatusBar(QStatusBar):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
-        self.setLayout(QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
 
-        hint_widget = UserHintWidget(app_model, self)
-        self.layout().addWidget(hint_widget)
+        self.parent = parent
+
+        app_model.sig_status_message.connect(self._on_app_model_status_message)
 
-        # Prioritized hint order:
-        # The first will have priority over the second
-        # The second will have priority over the third...
-        hint_widget.add_hint(InaccessibleDeviceHint())
-        hint_widget.add_hint(UnflashedDeviceHint())
-        hint_widget.add_hint(ConnectionHint())
+        self.message_timer = QtCore.QTimer(self)
+        self.message_timer.setInterval(3000)
+        self.message_timer.setSingleShot(True)
+        self.message_timer.timeout.connect(self._on_timer)
+
+        self.message_widget = QLabel(self)
+        self.addWidget(self.message_widget)
+
+        self.addPermanentWidget(FrameCountLabel(app_model, self))
+        self.addPermanentWidget(RateStatsLabel(app_model, self))
+        self.addPermanentWidget(JitterStatsLabel(app_model, self))
+        self.addPermanentWidget(BackendCPUPercentLabel(app_model, self))
+        self.addPermanentWidget(RSSVersionLabel(app_model, self))
+        self.addPermanentWidget(VersionLabel(app_model, self))
+
+        font_families = [
+            "Consolas",  # Windows
+            "Droid Sans Mono",  # Ubuntu
+            "DejaVu Sans Mono",  # Ubuntu, backup
+            "SF Mono",  # Mac
+        ]
+        font_family = ", ".join(f'"{ff}"' for ff in font_families)
+        self.setStyleSheet(f"QWidget{{font-family: {font_family};}}")
+
+    def _on_app_model_status_message(self, message: Optional[str]) -> None:
+        self.message_timer.stop()
+
+        if message:
+            self.message_widget.setText(message)
+            self.message_timer.start()
+        else:
+            self.message_widget.clear()
+
+    def _on_timer(self) -> None:
+        self.message_widget.clear()
+
+
+class ChangelogWindow(QMainWindow):
+    def __init__(self, parent: QWidget = None) -> None:
+        super().__init__()
+
+        self.setWindowTitle("Changelog")
+        self.text_browser = QTextBrowser()
+        self.setCentralWidget(self.text_browser)
+        self.set_center(parent.parent.parent)
+        self.showEvent = lambda _: self.set_center(parent.parent.parent)
+
+    def set_text(self, text: str) -> None:
+        document = QTextDocument()
+        document.setMarkdown(text)
+        self.text_browser.setDocument(document)
+
+    def set_center(self, main_window: QMainWindow) -> None:
+        fg = self.frameGeometry()
+        fg.moveCenter(main_window.geometry().center())
+        self.move(fg.topLeft())
+        self.resize(500, 400)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from . import pidgets
 from .attrs_config_editor import AttrsConfigEditor
 from .collapsible_widget import CollapsibleWidget
+from .data_editor import DataEditor
 from .metadata_view import ExtendedMetadataView, MetadataView, SmartMetadataView
 from .misc_error_view import MiscErrorView
 from .perf_calc_view import ExtendedPerfCalcView, PerfCalcView, SmartPerfCalcView
 from .sensor_config_editor import SensorConfigEditor
 from .session_config_editor import SessionConfigEditor
+from .subsweep_config_editor import SubsweepConfigEditor
 from .two_sensor_ids_editor import TwoSensorIdsEditor
 from .types import PidgetFactoryMapping, PidgetGroupFactoryMapping
 from .utils import GridGroupBox, HorizontalGroupBox, VerticalGroupBox
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import copy
 from functools import partial
-from typing import Any, Generic, Optional, Sequence, TypeVar, Union, cast
+from typing import Any, Optional, Sequence, TypeVar, Union, cast
 
 import attrs
 
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
+from .data_editor import DataEditor
 from .pidgets import FlatPidgetGroup, Pidget, PidgetGroup, PidgetGroupHook, PidgetHook
 from .types import PidgetFactoryMapping, PidgetGroupFactoryMapping
 from .utils import VerticalGroupBox
 
 
 T = TypeVar("T")
 
@@ -43,15 +45,15 @@
         return {FlatPidgetGroup(): cast(PidgetFactoryMapping, factory_mapping)}
 
     raise RuntimeError(
         "factory_mapping was neither a PidgetFactoryMappingi nor a PidgetGroupFactoryMapping"
     )
 
 
-class AttrsConfigEditor(QWidget, Generic[T]):
+class AttrsConfigEditor(DataEditor[Optional[T]]):
     _config: Optional[T]
     _erroneous_aspects: set[str]
 
     sig_update = Signal(object)
 
     def __init__(
         self,
@@ -73,27 +75,54 @@
         self._group_hooks: list[Sequence[PidgetGroupHook]] = []
         self._erroneous_aspects = set()
 
         for pidget_group, factory_mapping in _to_group_factory_mapping(factory_mapping).items():
             pidgets = []
             for aspect, factory in factory_mapping.items():
                 pidget = factory.create(group_box)
-                pidget.sig_parameter_changed.connect(partial(self._update_config_aspect, aspect))
+                pidget.sig_update.connect(partial(self._update_config_aspect, aspect))
 
                 self._pidget_mapping[aspect] = pidget
                 self._pidget_hooks[aspect] = factory.hooks
 
                 pidgets.append(pidget)
 
             group_widget = pidget_group.get_container(pidgets)
             group_box.layout().addWidget(group_widget)
 
             self._group_widgets.append(group_widget)
             self._group_hooks.append(pidget_group.hooks)
 
+    def set_data(self, config: Optional[T]) -> None:
+        if self._config == config:
+            return
+
+        self._config = config
+        self.setEnabled(config is not None)
+
+        if self._config is None:
+            return
+
+        for aspect, pidget in self._pidget_mapping.items():
+            if aspect in self._erroneous_aspects:
+                continue
+            config_value = getattr(self._config, aspect)
+            pidget.set_data(config_value)
+
+        for aspect, hooks in self._pidget_hooks.items():
+            for hook in hooks:
+                hook(self._pidget_mapping[aspect], self._pidget_mapping)
+
+        for group_widget, hooks in zip(self._group_widgets, self._group_hooks):
+            for hook in hooks:
+                hook(group_widget, self._pidget_mapping)
+
+    def get_data(self) -> Optional[T]:
+        return copy.deepcopy(self._config)
+
     def handle_validation_results(
         self, results: list[a121.ValidationResult]
     ) -> list[a121.ValidationResult]:
         for aspect, pidget in self._pidget_mapping.items():
             if aspect not in self._erroneous_aspects:
                 pidget.set_note_text("")
 
@@ -105,37 +134,14 @@
 
         return unhandled_results
 
     @property
     def is_ready(self) -> bool:
         return self._erroneous_aspects == set()
 
-    def set_data(self, config: Optional[T]) -> None:
-        self._config = config
-        self._run_pidget_hooks()
-
-    def _run_pidget_hooks(self) -> None:
-        for aspect, hooks in self._pidget_hooks.items():
-            for hook in hooks:
-                hook(self._pidget_mapping[aspect], self._pidget_mapping)
-
-        for group_widget, hooks in zip(self._group_widgets, self._group_hooks):
-            for hook in hooks:
-                hook(group_widget, self._pidget_mapping)
-
-    def sync(self) -> None:
-        self._update_pidgets()
-        self._run_pidget_hooks()
-
-    def setEnabled(self, enabled: bool) -> None:
-        super().setEnabled(enabled and self._config is not None)
-
-    def _broadcast(self) -> None:
-        self.sig_update.emit(self._config)
-
     def _handle_validation_result(self, result: a121.ValidationResult) -> bool:
         if result.aspect is None:
             return False
 
         if result.aspect in self._erroneous_aspects:
             # If there is an erroneous aspect in the GUI, we do not want to overwrite that.
             # Once the erroneous aspect is handled with, the same validation result will
@@ -150,30 +156,29 @@
                     self._pidget_mapping[result.aspect].set_note_text(
                         result.message, result.criticality
                     )
                     result_handled = True
 
         return result_handled
 
-    def _update_pidgets(self) -> None:
-        if self._config is None:
-            return
-
-        for aspect, pidget in self._pidget_mapping.items():
-            config_value = getattr(self._config, aspect)
-            pidget.set_parameter(config_value)
-
     def _update_config_aspect(self, aspect: str, value: Any) -> None:
         if self._config is None:
             return
 
         try:
-            self._config = attrs.evolve(self._config, **{aspect: value})
+            # The passing of "self._config: T" is not type safe. We cannot know
+            # if "T" is an attrs class in the scope of this class without binding
+            # "T" to a common superclass.
+            # "AlgoConfigBase" is a candidate, but that is part of the algo-package.
+            config = attrs.evolve(self._config, **{aspect: value})  # type: ignore[misc]
         except Exception as e:
             self._erroneous_aspects.add(aspect)
             self._pidget_mapping[aspect].set_note_text(e.args[0], Criticality.ERROR)
+
+            # this emit needs to be done to signal that "is_ready" has changed.
+            self.sig_update.emit(self.get_data())
         else:
             self._pidget_mapping[aspect].set_note_text(None)
-            if aspect in self._erroneous_aspects:
-                self._erroneous_aspects.remove(aspect)
+            self._erroneous_aspects.discard(aspect)
 
-        self._broadcast()
+            self.set_data(config)
+            self.sig_update.emit(config)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,36 +79,36 @@
 PidgetMappingPredicate = t.Callable[[PidgetMapping], bool]
 
 
 def parameter_equals(aspect: str, value: t.Any) -> PidgetMappingPredicate:
     """Checks whether the parameter of the pidget assigned to aspect is equal to value"""
 
     def inner(mapping: PidgetMapping) -> bool:
-        return bool(mapping[aspect].get_parameter() == value)
+        return bool(mapping[aspect].get_data() == value)
 
     return inner
 
 
 def parameter_is(aspect: str, value: t.Any) -> PidgetMappingPredicate:
     """Checks whether the parameter of the pidget assigned to aspect "is" passed value
     Should be used with singletons like "True", "False", "None", etc.
     """
 
     def inner(mapping: PidgetMapping) -> bool:
-        return mapping[aspect].get_parameter() is value
+        return mapping[aspect].get_data() is value
 
     return inner
 
 
 def parameter_within(aspect: str, range: t.Tuple[float, float]) -> PidgetMappingPredicate:
     """Checks whether the parameter of the pidget assigned to aspect is in range"""
 
     def inner(mapping: PidgetMapping) -> bool:
         lower, higher = range
-        return bool(lower < mapping[aspect].get_parameter() < higher)
+        return bool(lower < mapping[aspect].get_data() < higher)
 
     return inner
 
 
 def enable_if(predicate: PidgetMappingPredicate) -> GeneralHook:
     """Enables the instance this hook is assigned to if the predicate evaluates to "True" """
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     QSlider,
     QSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
 from acconeer.exptool.a121._core.entities import Criticality
+from acconeer.exptool.app.new.ui.plugin_components.data_editor import DataEditor
 
 from .common import MaybeIterable, as_sequence
 
 
 def widget_wrap_layout(layout: QLayout) -> QWidget:
     dummy = QWidget()
     dummy.setLayout(layout)
@@ -53,22 +54,22 @@
     hooks: Sequence[PidgetHook] = attrs.field(factory=tuple, converter=_hooks_converter)
 
     @abc.abstractmethod
     def create(self, parent: QWidget) -> Pidget:
         ...
 
 
-class Pidget(QWidget):
+class Pidget(DataEditor[Any]):
     """Base class for a parameter-bound widget.
 
     A ``Pidget`` comes with a
     ``name`` label and an ``note`` label by default.
     """
 
-    sig_parameter_changed = QtCore.Signal(object)
+    sig_update = QtCore.Signal(object)
 
     def __init__(self, factory: PidgetFactory, parent: QWidget) -> None:
         super().__init__(parent=parent)
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
@@ -112,54 +113,58 @@
         self.__note_widget.show()
         self.__note_widget.setText(message)
         self.__note_widget.setStyleSheet(
             f"background-color: {COLOR_MAP[criticality]}; color: white; font: bold italic;"
         )
 
     @abc.abstractmethod
-    def set_parameter(self, value: Any) -> None:
+    def set_data(self, value: Any) -> None:
         pass
 
     @abc.abstractmethod
-    def get_parameter(self) -> Any:
+    def get_data(self) -> Any:
         pass
 
+    @property
+    def is_ready(self) -> bool:
+        return not self.__note_widget.isVisible()
+
 
 @attrs.frozen(kw_only=True, slots=False)
 class IntPidgetFactory(PidgetFactory):
     limits: Optional[Tuple[Optional[int], Optional[int]]] = None
     suffix: Optional[str] = None
 
     def create(self, parent: QWidget) -> IntPidget:
         return IntPidget(self, parent)
 
 
 class IntPidget(Pidget):
     def __init__(self, factory: IntPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
-        self.__spin_box = _PidgetSpinBox(
+        self._spin_box = _PidgetSpinBox(
             self._body_widget,
             limits=factory.limits,
             suffix=factory.suffix,
         )
-        self.__spin_box.valueChanged.connect(self.__on_changed)
-        self._body_layout.addWidget(self.__spin_box)
+        self._spin_box.valueChanged.connect(self.__on_changed)
+        self._body_layout.addWidget(self._spin_box)
 
-    def set_parameter(self, value: Any) -> None:
+    def set_data(self, value: Any) -> None:
         assert isinstance(value, int)
 
         with QtCore.QSignalBlocker(self):
-            self.__spin_box.setValue(value)
+            self._spin_box.setValue(value)
 
-    def get_parameter(self) -> int:
-        return int(self.__spin_box.value())
+    def get_data(self) -> int:
+        return int(self._spin_box.value())
 
     def __on_changed(self) -> None:
-        self.sig_parameter_changed.emit(self.__spin_box.value())
+        self.sig_update.emit(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class FloatPidgetFactory(PidgetFactory):
     limits: Optional[Tuple[Optional[float], Optional[float]]] = None
     suffix: Optional[str] = None
     decimals: int = 1
@@ -168,34 +173,34 @@
         return FloatPidget(self, parent)
 
 
 class FloatPidget(Pidget):
     def __init__(self, factory: FloatPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
-        self.__spin_box = _PidgetDoubleSpinBox(
+        self._spin_box = _PidgetDoubleSpinBox(
             self._body_widget,
             limits=factory.limits,
             suffix=factory.suffix,
             decimals=factory.decimals,
         )
-        self.__spin_box.valueChanged.connect(self.__on_changed)
-        self._body_layout.addWidget(self.__spin_box)
+        self._spin_box.valueChanged.connect(self.__on_changed)
+        self._body_layout.addWidget(self._spin_box)
 
-    def set_parameter(self, value: Any) -> None:
+    def set_data(self, value: Any) -> None:
         assert isinstance(value, (int, float))
 
         with QtCore.QSignalBlocker(self):
-            self.__spin_box.setValue(value)
+            self._spin_box.setValue(value)
 
-    def get_parameter(self) -> float:
-        return float(self.__spin_box.value())
+    def get_data(self) -> float:
+        return float(self._spin_box.value())
 
     def __on_changed(self) -> None:
-        self.sig_parameter_changed.emit(self.__spin_box.value())
+        self.sig_update.emit(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class FloatSliderPidgetFactory(FloatPidgetFactory):
     limits: Tuple[float, float]
     log_scale: bool = False
     show_limit_values: bool = True
@@ -228,22 +233,22 @@
         slider_widget.setLayout(QHBoxLayout(slider_widget))
         slider_widget.layout().setContentsMargins(11, 6, 11, 0)
 
         lower_limit, upper_limit = factory.limits
         if factory.show_limit_values:
             slider_widget.layout().addWidget(QLabel(str(lower_limit), slider_widget))
 
-        self.__slider = _PidgetFloatSlider(
+        self._slider = _PidgetFloatSlider(
             slider_widget,
             limits=factory.limits,
             decimals=factory.decimals,
             log_scale=factory.log_scale,
         )
-        self.__slider.wrapped_value_changed.connect(self.__on_slider_changed)
-        slider_widget.layout().addWidget(self.__slider)
+        self._slider.wrapped_value_changed.connect(self.__on_slider_changed)
+        slider_widget.layout().addWidget(self._slider)
 
         if factory.show_limit_values:
             slider_widget.layout().addWidget(QLabel(str(upper_limit), slider_widget))
 
         if factory.limit_texts is not None:
             label_text_widget = QWidget(self._body_widget)
             self._body_layout.addWidget(label_text_widget, 2, 0, 1, -1)
@@ -268,35 +273,35 @@
 
         layout = QGridLayout(self._body_widget)
         layout.setContentsMargins(0, 0, 0, 6)
         layout.setSpacing(0)
         layout.addWidget(note_label_widget, 0, 0)
         return layout
 
-    def set_parameter(self, value: Any) -> None:
+    def set_data(self, value: Any) -> None:
         assert isinstance(value, (int, float))
 
         with QtCore.QSignalBlocker(self):
             self.__spin_box.setValue(value)
-            self.__slider.wrapped_set_value(value)
+            self._slider.wrapped_set_value(value)
 
-    def get_parameter(self) -> float:
+    def get_data(self) -> float:
         return float(self.__spin_box.value())
 
     def __on_spin_box_changed(self, value: float) -> None:
         with QtCore.QSignalBlocker(self):
-            self.__slider.wrapped_set_value(value)
+            self._slider.wrapped_set_value(value)
 
-        self.sig_parameter_changed.emit(value)
+        self.sig_update.emit(value)
 
     def __on_slider_changed(self, value: float) -> None:
         with QtCore.QSignalBlocker(self):
             self.__spin_box.setValue(value)
 
-        self.sig_parameter_changed.emit(value)
+        self.sig_update.emit(value)
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalPidgetFactory(PidgetFactory):
     checkbox_label_text: Optional[str] = None
 
 
@@ -320,20 +325,20 @@
 
         layout = QHBoxLayout(self._optional_widget)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addStretch(1)
         layout.addWidget(none_checkbox)
         return layout
 
-    def set_parameter(self, value: Any) -> None:
+    def set_data(self, value: Any) -> None:
         with QtCore.QSignalBlocker(self):
             self._none_checkbox.setChecked(value is not None)
 
     @abc.abstractmethod
-    def get_parameter(self) -> Optional[Any]:
+    def get_data(self) -> Optional[Any]:
         pass
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalIntPidgetFactory(OptionalPidgetFactory, IntPidgetFactory):
     init_set_value: Optional[int] = None
 
@@ -341,137 +346,137 @@
         return OptionalIntPidget(self, parent)
 
 
 class OptionalIntPidget(OptionalPidget):
     def __init__(self, factory: OptionalIntPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
-        self.__spin_box = _PidgetSpinBox(
+        self._spin_box = _PidgetSpinBox(
             self._optional_widget,
             limits=factory.limits,
             suffix=factory.suffix,
             init_set_value=factory.init_set_value,
         )
-        self._optional_layout.addWidget(self.__spin_box)
+        self._optional_layout.addWidget(self._spin_box)
 
         self._none_checkbox.stateChanged.connect(self.__on_changed)
-        self.__spin_box.valueChanged.connect(self.__on_changed)
+        self._spin_box.valueChanged.connect(self.__on_changed)
 
     def __on_changed(self) -> None:
         checked = self._none_checkbox.isChecked()
 
         with QtCore.QSignalBlocker(self):
-            self.__spin_box.setEnabled(checked)
+            self._spin_box.setEnabled(checked)
 
-        value = self.__spin_box.value() if checked else None
-        self.sig_parameter_changed.emit(value)
+        value = self._spin_box.value() if checked else None
+        self.sig_update.emit(value)
 
-    def set_parameter(self, value: Any) -> None:
-        super().set_parameter(value)
+    def set_data(self, value: Any) -> None:
+        super().set_data(value)
 
         with QtCore.QSignalBlocker(self):
             if value is None:
-                self.__spin_box.setEnabled(False)
+                self._spin_box.setEnabled(False)
             else:
-                self.__spin_box.setValue(value)
-                self.__spin_box.setEnabled(True)
+                self._spin_box.setValue(value)
+                self._spin_box.setEnabled(True)
 
-    def get_parameter(self) -> Optional[int]:
+    def get_data(self) -> Optional[int]:
         if not self._none_checkbox.isChecked():
             return None
         else:
-            return int(self.__spin_box.value())
+            return int(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalFloatPidgetFactory(OptionalPidgetFactory, FloatPidgetFactory):
     init_set_value: Optional[float] = None
 
     def create(self, parent: QWidget) -> OptionalFloatPidget:
         return OptionalFloatPidget(self, parent)
 
 
 class OptionalFloatPidget(OptionalPidget):
     def __init__(self, factory: OptionalFloatPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
-        self.__spin_box = _PidgetDoubleSpinBox(
+        self._spin_box = _PidgetDoubleSpinBox(
             self._optional_widget,
             decimals=factory.decimals,
             limits=factory.limits,
             suffix=factory.suffix,
             init_set_value=factory.init_set_value,
         )
-        self._optional_layout.addWidget(self.__spin_box)
+        self._optional_layout.addWidget(self._spin_box)
 
         self._none_checkbox.stateChanged.connect(self.__on_changed)
-        self.__spin_box.valueChanged.connect(self.__on_changed)
+        self._spin_box.valueChanged.connect(self.__on_changed)
 
     def __on_changed(self) -> None:
         checked = self._none_checkbox.isChecked()
 
         with QtCore.QSignalBlocker(self):
-            self.__spin_box.setEnabled(checked)
+            self._spin_box.setEnabled(checked)
 
-        value = self.__spin_box.value() if checked else None
-        self.sig_parameter_changed.emit(value)
+        value = self._spin_box.value() if checked else None
+        self.sig_update.emit(value)
 
-    def set_parameter(self, value: Any) -> None:
-        super().set_parameter(value)
+    def set_data(self, value: Any) -> None:
+        super().set_data(value)
 
         with QtCore.QSignalBlocker(self):
             if value is None:
-                self.__spin_box.setEnabled(False)
+                self._spin_box.setEnabled(False)
             else:
-                self.__spin_box.setValue(value)
-                self.__spin_box.setEnabled(True)
+                self._spin_box.setValue(value)
+                self._spin_box.setEnabled(True)
 
-    def get_parameter(self) -> Optional[float]:
+    def get_data(self) -> Optional[float]:
         if not self._none_checkbox.isChecked():
             return None
         else:
-            return float(self.__spin_box.value())
+            return float(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class CheckboxPidgetFactory(PidgetFactory):
     def create(self, parent: QWidget) -> CheckboxPidget:
         return CheckboxPidget(self, parent)
 
 
 class CheckboxPidget(Pidget):
     def __init__(self, factory: CheckboxPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
         assert isinstance(self._body_layout, QGridLayout)
 
-        self.__checkbox = QCheckBox(self._body_widget)
-        self.__checkbox.clicked.connect(self.__on_checkbox_click)
-        self._body_layout.addWidget(self.__checkbox, 0, 0)
+        self._checkbox = QCheckBox(self._body_widget)
+        self._checkbox.clicked.connect(self.__on_checkbox_click)
+        self._body_layout.addWidget(self._checkbox, 0, 0)
         self._body_layout.setColumnStretch(0, 0)
         self._body_layout.setColumnStretch(1, 1)
 
     def _create_body_layout(self, note_label_widget: QWidget) -> QLayout:
         """Called by Pidget.__init__"""
 
         layout = QGridLayout(self._body_widget)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
         layout.addWidget(note_label_widget, 0, 1)
         return layout
 
     def __on_checkbox_click(self, checked: bool) -> None:
-        self.sig_parameter_changed.emit(checked)
+        self.sig_update.emit(checked)
 
-    def set_parameter(self, param: Any) -> None:
+    def set_data(self, param: Any) -> None:
         with QtCore.QSignalBlocker(self):
-            self.__checkbox.setChecked(bool(param))
+            self._checkbox.setChecked(bool(param))
 
-    def get_parameter(self) -> bool:
-        return bool(self.__checkbox.isChecked())
+    def get_data(self) -> bool:
+        return bool(self._checkbox.isChecked())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class ComboboxPidgetFactory(PidgetFactory, Generic[T]):
     items: list[tuple[str, T]]
 
     def create(self, parent: QWidget) -> ComboboxPidget[T]:
@@ -488,24 +493,24 @@
         for displayed_text, user_data in factory.items:
             self._combobox.addItem(displayed_text, user_data)
 
         self._combobox.currentIndexChanged.connect(self.__emit_data_of_combobox_item)
 
     def __emit_data_of_combobox_item(self, index: int) -> None:
         data = self._combobox.itemData(index)
-        self.sig_parameter_changed.emit(data)
+        self.sig_update.emit(data)
 
-    def set_parameter(self, param: Any) -> None:
+    def set_data(self, param: Any) -> None:
         with QtCore.QSignalBlocker(self):
             index = self._combobox.findData(param)
             if index == -1:
                 raise ValueError(f"Data item {param} could not be found in {self}.")
             self._combobox.setCurrentIndex(index)
 
-    def get_parameter(self) -> T:
+    def get_data(self) -> T:
         return cast(T, self._combobox.currentData())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class SensorIdPidgetFactory(ComboboxPidgetFactory[int]):
     name_label_text: str = attrs.field(default="Sensor:")
     name_label_tooltip: str = attrs.field(default="The sensor to use in session")
@@ -532,15 +537,15 @@
 
     def set_selected_sensor(self, sensor_id: Optional[int], sensor_list: list[int]) -> None:
         if sensor_list != self._sensor_list:
             self._sensor_list = sensor_list
             self._update_items([(str(i), i) for i in sensor_list])
 
         try:
-            super().set_parameter(sensor_id)
+            super().set_data(sensor_id)
         except ValueError:
             self.setEnabled(False)
         else:
             self.setEnabled(True)
 
 
 @attrs.frozen(kw_only=True, slots=False)
@@ -591,30 +596,30 @@
         self._none_checkbox.stateChanged.connect(self.__emit_data_of_combobox_or_none)
         self._none_checkbox.stateChanged.connect(self.__enable_combobox_if_checked)
         self._combobox.currentIndexChanged.connect(self.__emit_data_of_combobox_or_none)
 
     def __emit_data_of_combobox_or_none(self) -> None:
         if self._none_checkbox.isChecked():
             data = self._combobox.currentData()
-            self.sig_parameter_changed.emit(data)
+            self.sig_update.emit(data)
         else:
-            self.sig_parameter_changed.emit(None)
+            self.sig_update.emit(None)
 
     def __enable_combobox_if_checked(self) -> None:
         self._combobox.setEnabled(self._none_checkbox.isChecked())
 
-    def set_parameter(self, value: Any) -> None:
-        super().set_parameter(value)
+    def set_data(self, value: Any) -> None:
+        super().set_data(value)
         if value is not None:
             self.set_enum_parameter(value)
             self._combobox.setEnabled(True)
         else:
             self._combobox.setEnabled(False)
 
-    def get_parameter(self) -> Optional[Enum]:
+    def get_data(self) -> Optional[Enum]:
         if not self._none_checkbox.isChecked():
             return None
         else:
             return cast(Enum, self._combobox.currentData())
 
     def set_enum_parameter(self, param: Any) -> None:
         with QtCore.QSignalBlocker(self):
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import copy
 import logging
 from functools import partial
-from typing import Any, Optional
+from typing import Any, Iterator, Optional
 
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QTabWidget, QToolButton, QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from . import pidgets
+from .data_editor import DataEditor
 from .subsweep_config_editor import SubsweepConfigEditor
 from .types import PidgetFactoryMapping
 from .utils import VerticalGroupBox
 
 
 log = logging.getLogger(__name__)
 
 
-class SensorConfigEditor(QWidget):
+class SensorConfigEditor(DataEditor[Optional[a121.SensorConfig]]):
     sig_update = Signal(object)
 
     _sensor_config: Optional[a121.SensorConfig]
-    _subsweep_config_editors: list[SubsweepConfigEditor]
 
     _sensor_config_pidgets: dict[str, pidgets.Pidget]
     _erroneous_aspects: set[str]
     _read_only: bool
     _supports_multiple_subsweeps: bool
 
     SPACING = 15
@@ -131,15 +132,14 @@
     ) -> None:
         super().__init__(parent=parent)
 
         self._sensor_config_pidgets = {}
         self._erroneous_aspects = set()
 
         self._sensor_config = None
-        self._subsweep_config_editors = []
 
         self._read_only = False
         self._supports_multiple_subsweeps = supports_multiple_subsweeps
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
@@ -147,17 +147,15 @@
         self.sensor_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.sensor_group_box)
 
         for aspect, factory in self.SENSOR_CONFIG_FACTORIES.items():
             pidget = factory.create(self.sensor_group_box)
             self.sensor_group_box.layout().addWidget(pidget)
 
-            pidget.sig_parameter_changed.connect(
-                partial(self._update_sensor_config_aspect, aspect)
-            )
+            pidget.sig_update.connect(partial(self._update_sensor_config_aspect, aspect))
 
             self._sensor_config_pidgets[aspect] = pidget
 
         self.subsweep_group_box = VerticalGroupBox("Subsweep parameters", parent=self)
         self.subsweep_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.subsweep_group_box)
 
@@ -172,120 +170,62 @@
             self._plus_button = QToolButton(self)
             self._plus_button.setText("+")
             self.layout().addWidget(self._plus_button)
             self._plus_button.clicked.connect(self._add_subsweep_config)
             self._tab_widget.setCornerWidget(self._plus_button)
             self._tab_widget.cornerWidget().setMinimumSize(self._plus_button.sizeHint())
 
-    def _add_subsweep_config(self) -> None:
-        if self._sensor_config is None:
-            return
-        if self._tab_widget.count() > 3:
-            return
-        subsweep_config = a121.SubsweepConfig()
-        self._sensor_config._subsweeps.append(subsweep_config)
-        self._broadcast()
-        subsweep_config_editor = self._add_subsweep_config_editor()
-        subsweep_config_editor.set_data(subsweep_config)
-        subsweep_config_editor.sync()
-
-    def _add_tabs(self, tabs_needed: int) -> None:
-        while self._tab_widget.count() < tabs_needed:
-            self._add_subsweep_config_editor()
-
-    def _add_subsweep_config_editor(self) -> SubsweepConfigEditor:
-        subsweep_config_editor = SubsweepConfigEditor(self)
-        subsweep_config_editor.sig_update.connect(self._broadcast)
-        subsweep_config_editor.set_read_only(self._read_only)
-        self._subsweep_config_editors.append(subsweep_config_editor)
-        self._tab_widget.addTab(subsweep_config_editor, str(len(self._subsweep_config_editors)))
-        self._update_tab_labels()
-        return subsweep_config_editor
-
-    def _remove_subsweep_config(self, idx: int) -> None:
-        if self._sensor_config is None:
-            return
-        if self._tab_widget.count() < 2:
-            return
-        self._sensor_config.subsweeps.pop(idx)
-        self._broadcast()
-        self._remove_subsweep_config_editor(idx)
-
-    def _remove_tabs(self, tabs_needed: int) -> None:
-        while self._tab_widget.count() > tabs_needed:
-            self._remove_subsweep_config_editor(0)
-
-    def _remove_subsweep_config_editor(self, idx: int) -> None:
-        self._tab_widget.removeTab(idx)
-        self._subsweep_config_editors.pop(idx)
-        self._update_tab_labels()
-
-    def _update_tab_labels(self) -> None:
-        for tab_idx in range(self._tab_widget.count()):
-            self._tab_widget.setTabText(tab_idx, f"{tab_idx + 1}      ")
-
-    def _update_ui(self) -> None:
-        if self._sensor_config is None:
-            log.debug("could not update ui as SensorConfig is None")
-            return
-
-        self._sensor_config_pidgets["sweeps_per_frame"].set_parameter(
-            self._sensor_config.sweeps_per_frame
-        )
-        self._sensor_config_pidgets["sweep_rate"].set_parameter(self._sensor_config.sweep_rate)
-        self._sensor_config_pidgets["frame_rate"].set_parameter(self._sensor_config.frame_rate)
-        self._sensor_config_pidgets["continuous_sweep_mode"].set_parameter(
-            self._sensor_config.continuous_sweep_mode
-        )
-        self._sensor_config_pidgets["double_buffering"].set_parameter(
-            self._sensor_config.double_buffering
-        )
-        self._sensor_config_pidgets["inter_frame_idle_state"].set_parameter(
-            self._sensor_config.inter_frame_idle_state
-        )
-        self._sensor_config_pidgets["inter_sweep_idle_state"].set_parameter(
-            self._sensor_config.inter_sweep_idle_state
-        )
-
-    def set_data(self, sensor_config: Optional[a121.SensorConfig]) -> None:
-        self._sensor_config = sensor_config
-        if sensor_config is None:
-            return
-        tabs_needed = len(sensor_config.subsweeps)
-        self._remove_tabs(tabs_needed)
-        self._add_tabs(tabs_needed)
-        for i, subsweep in enumerate(sensor_config.subsweeps):
-            self._subsweep_config_editors[i].set_data(subsweep)
-
-    @property
-    def is_ready(self) -> bool:
-        return self._erroneous_aspects == set() and all(
-            se.is_ready for se in self._subsweep_config_editors
-        )
-
     def set_read_only(self, read_only: bool) -> None:
         self._read_only = read_only
 
         for pidget in self._sensor_config_pidgets.values():
             pidget.setEnabled(not read_only)
 
         if self._supports_multiple_subsweeps:
             self._tab_widget.setTabsClosable(not read_only)
             self._plus_button.setEnabled(not read_only)
 
         for editor in self._subsweep_config_editors:
             editor.set_read_only(read_only)
 
-    def sync(self) -> None:
-        self._update_ui()
-        for subsweep_config_editor in self._subsweep_config_editors:
-            subsweep_config_editor.sync()
+    def set_data(self, sensor_config: Optional[a121.SensorConfig]) -> None:
+        if self._sensor_config == sensor_config:
+            return
 
-    def _broadcast(self) -> None:
-        self.sig_update.emit(self._sensor_config)
+        self._sensor_config = sensor_config
+
+        self.setEnabled(sensor_config is not None)
+        if self._sensor_config is None:
+            log.debug("could not update ui as SensorConfig is None")
+            return
+
+        for aspect, pidget in self._sensor_config_pidgets.items():
+            if aspect in self._erroneous_aspects:
+                continue
+            pidget.set_data(getattr(self._sensor_config, aspect))
+
+        while self._tab_widget.count() > self._sensor_config.num_subsweeps:
+            self._tab_widget.removeTab(0)
+
+        while self._tab_widget.count() < self._sensor_config.num_subsweeps:
+            new_tab_idx = self._tab_widget.count()
+            self._tab_widget.addTab(self._create_subsweep_config_editor(new_tab_idx), "")
+
+        for tab_idx, subsweep_editor in enumerate(self._subsweep_config_editors):
+            self._tab_widget.setTabText(tab_idx, f"{tab_idx + 1}      ")
+            subsweep_editor.sig_update.disconnect()
+            subsweep_editor.sig_update.connect(
+                partial(self._update_subsweep_config_at_index, tab_idx)
+            )
+
+        for subsweep, editor in zip(self._sensor_config.subsweeps, self._subsweep_config_editors):
+            editor.set_data(subsweep)
+
+    def get_data(self) -> Optional[a121.SensorConfig]:
+        return copy.deepcopy(self._sensor_config)
 
     def handle_validation_results(
         self, results: list[a121.ValidationResult]
     ) -> list[a121.ValidationResult]:
         for aspect, pidget in self._sensor_config_pidgets.items():
             if aspect not in self._erroneous_aspects:
                 pidget.set_note_text("")
@@ -297,14 +237,20 @@
                 unhandled_results.append(result)
 
         for subsweep_config_editor in self._subsweep_config_editors:
             unhandled_results = subsweep_config_editor.handle_validation_results(unhandled_results)
 
         return unhandled_results
 
+    @property
+    def is_ready(self) -> bool:
+        return self._erroneous_aspects == set() and all(
+            se.is_ready for se in self._subsweep_config_editors
+        )
+
     def _handle_validation_result(self, result: a121.ValidationResult) -> bool:
         if result.aspect is None or self._sensor_config is None:
             return False
 
         if result.aspect in self._erroneous_aspects:
             # If there is an erroneous aspect in the GUI, we do not want to overwrite that.
             # Once the erroneous aspect is handled with, the same validation result will
@@ -317,21 +263,68 @@
             for aspect, pidget in self._sensor_config_pidgets.items():
                 if result.aspect == aspect:
                     pidget.set_note_text(result.message, result.criticality)
                     result_handled = True
 
         return result_handled
 
+    def _create_subsweep_config_editor(self, index: int) -> SubsweepConfigEditor:
+        e = SubsweepConfigEditor()
+        e.sig_update.connect(lambda ssc: self._update_subsweep_config_at_index(index, ssc))
+        e.set_read_only(self._read_only)
+        return e
+
+    @property
+    def _subsweep_config_editors(self) -> Iterator[SubsweepConfigEditor]:
+        for tab_idx in range(self._tab_widget.count()):
+            tab_widget = self._tab_widget.widget(tab_idx)
+            assert isinstance(tab_widget, SubsweepConfigEditor)
+            yield tab_widget
+
+    def _add_subsweep_config(self) -> None:
+        if self._sensor_config is None or self._sensor_config.num_subsweeps >= 4:
+            return
+
+        config = copy.deepcopy(self._sensor_config)
+        config._subsweeps.append(a121.SubsweepConfig())
+        self.set_data(config)
+        self.sig_update.emit(config)
+
+    def _remove_subsweep_config(self, idx: int) -> None:
+        if self._sensor_config is None or len(self._sensor_config.subsweeps) <= 1:
+            return
+
+        config = copy.deepcopy(self._sensor_config)
+        config._subsweeps.pop(idx)
+        self.set_data(config)
+        self.sig_update.emit(config)
+
+    def _update_subsweep_config_at_index(
+        self, index: int, subsweep_config: a121.SubsweepConfig
+    ) -> None:
+        if self._sensor_config is None or index not in range(self._sensor_config.num_subsweeps):
+            return
+
+        config = copy.deepcopy(self._sensor_config)
+        config._subsweeps[index] = subsweep_config
+        self.set_data(config)
+        self.sig_update.emit(config)
+
     def _update_sensor_config_aspect(self, aspect: str, value: Any) -> None:
         if self._sensor_config is None:
             raise TypeError("SensorConfig is None")
 
+        config = copy.deepcopy(self._sensor_config)
+
         try:
-            setattr(self._sensor_config, aspect, value)
+            setattr(config, aspect, value)
         except Exception as e:
             self._sensor_config_pidgets[aspect].set_note_text(e.args[0], Criticality.ERROR)
             self._erroneous_aspects.add(aspect)
+
+            # this emit needs to be done to signal that "is_ready" has changed.
+            self.sig_update.emit(self.get_data())
         else:
-            if aspect in self._erroneous_aspects:
-                self._erroneous_aspects.remove(aspect)
+            self._erroneous_aspects.discard(aspect)
 
-        self._broadcast()
+            self.set_data(config)
+            self.sig_update.emit(config)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,106 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import copy
 import logging
 from typing import Any, Optional
 
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from . import pidgets
+from .data_editor import DataEditor
 from .sensor_config_editor import SensorConfigEditor
 from .utils import VerticalGroupBox
 
 
 log = logging.getLogger(__name__)
 
 
-class SessionConfigEditor(QWidget):
+class SessionConfigEditor(DataEditor[Optional[a121.SessionConfig]]):
     _session_config: Optional[a121.SessionConfig]
     _server_info: Optional[a121.ServerInfo]
-
     _sensor_id_pidget: pidgets.SensorIdPidget
 
+    _update_rate_erroneous: bool
+
     sig_update = Signal(object)
 
     SPACING = 15
 
     def __init__(
         self, supports_multiple_subsweeps: bool = False, parent: Optional[QWidget] = None
     ) -> None:
         super().__init__(parent=parent)
 
         self._server_info = None
 
         self._session_config = None
+        self._update_rate_erroneous = False
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         self.session_group_box = VerticalGroupBox("Session parameters", parent=self)
         self.session_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.session_group_box)
 
         self._sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(self)
-        self._sensor_id_pidget.sig_parameter_changed.connect(self._update_sensor_id)
+        self._sensor_id_pidget.sig_update.connect(self._update_sole_sensor_id)
         self.session_group_box.layout().addWidget(self._sensor_id_pidget)
 
         self._update_rate_pidget = pidgets.OptionalFloatPidgetFactory(
             name_label_text="Update rate:",
             name_label_tooltip=(
                 "Set an update rate limit on the server.\n"
                 "If 'Limit' is unchecked, the server will run as fast as possible."
             ),
             limits=(0.1, 1e4),
             decimals=1,
             init_set_value=10.0,
             suffix="Hz",
             checkbox_label_text="Limit",
         ).create(self)
-        self._update_rate_pidget.sig_parameter_changed.connect(self._update_update_rate)
+        self._update_rate_pidget.sig_update.connect(self._update_update_rate)
         self.session_group_box.layout().addWidget(self._update_rate_pidget)
 
         self._sensor_config_editor = SensorConfigEditor(supports_multiple_subsweeps, self)
-        self._sensor_config_editor.sig_update.connect(self._broadcast)
+        self._sensor_config_editor.sig_update.connect(self._update_sole_sensor_config)
         self.layout().addWidget(self._sensor_config_editor)
 
-    @property
-    def is_ready(self) -> bool:
-        return self._sensor_config_editor.is_ready
-
-    def set_data(self, session_config: Optional[a121.SessionConfig]) -> None:
-        self._session_config = session_config
-        if session_config is not None:
-            self._sensor_config_editor.set_data(session_config.sensor_config)
+    def set_selected_sensor(self, sensor_id: Optional[int], sensor_list: list[int]) -> None:
+        self._sensor_id_pidget.set_selected_sensor(sensor_id, sensor_list)
 
     def set_read_only(self, read_only: bool) -> None:
         self._sensor_id_pidget.setEnabled(not read_only)
         self._update_rate_pidget.setEnabled(not read_only)
         self._sensor_config_editor.set_read_only(read_only)
 
-    def sync(self) -> None:
-        self._update_ui()
-        self._sensor_config_editor.sync()
+    def set_data(self, session_config: Optional[a121.SessionConfig]) -> None:
+        if self._session_config == session_config:
+            return
+
+        self._session_config = session_config
+        self.setEnabled(session_config is not None)
+
+        if self._session_config is None:
+            log.debug("could not update ui as SessionConfig is None")
+            return
 
-    def setEnabled(self, enabled: bool) -> None:
-        super().setEnabled(enabled and self._session_config is not None)
+        self._update_rate_pidget.set_data(self._session_config.update_rate)
+        self._sensor_config_editor.set_data(self._session_config.sensor_config)
 
-    def _broadcast(self) -> None:
-        self.sig_update.emit(self._session_config)
+    def get_data(self) -> Optional[a121.SessionConfig]:
+        return copy.deepcopy(self._session_config)
 
     def handle_validation_results(
         self, results: list[a121.ValidationResult]
     ) -> list[a121.ValidationResult]:
         self._update_rate_pidget.set_note_text(None)
         self._sensor_id_pidget.set_note_text(None)
 
@@ -105,14 +110,18 @@
             if not self._handle_validation_result(result):
                 unhandled_results.append(result)
 
         unhandled_results = self._sensor_config_editor.handle_validation_results(unhandled_results)
 
         return unhandled_results
 
+    @property
+    def is_ready(self) -> bool:
+        return not self._update_rate_erroneous and self._sensor_config_editor.is_ready
+
     def _handle_validation_result(self, result: a121.ValidationResult) -> bool:
         if self._session_config is None:
             raise RuntimeError(
                 "SessionConfigEditor's config is None while ValidationResults are being handled."
             )
 
         result_handled = False
@@ -126,34 +135,48 @@
 
         return result_handled
 
     def _update_update_rate(self, value: Any) -> None:
         if self._session_config is None:
             raise TypeError("SessionConfig is None")
 
+        config = copy.deepcopy(self._session_config)
+
         try:
-            self._session_config.update_rate = value
+            config.update_rate = value
         except Exception as e:
+            self._update_rate_erroneous = True
             self._update_rate_pidget.set_note_text(e.args[0], Criticality.ERROR)
 
-        self._broadcast()
+            # this emit needs to be done to signal that "is_ready" has changed.
+            self.sig_update.emit(self.get_data())
+        else:
+            self._update_rate_erroneous = False
 
-    def _update_sensor_id(self, value: Any) -> None:
+            self.set_data(config)
+            self.sig_update.emit(config)
+
+    def _update_sole_sensor_id(self, value: Any) -> None:
         if self._session_config is None:
             raise TypeError("SessionConfig is None")
 
+        config = copy.deepcopy(self._session_config)
+
         try:
-            self._session_config.sensor_id = value
+            config.sensor_id = value
         except Exception as e:
             self._sensor_id_pidget.set_note_text(e.args[0], Criticality.ERROR)
 
-        self._broadcast()
+        self.set_data(config)
+        self.sig_update.emit(config)
 
-    def _update_ui(self) -> None:
+    def _update_sole_sensor_config(self, sensor_config: a121.SensorConfig) -> None:
         if self._session_config is None:
-            log.debug("could not update ui as SessionConfig is None")
-            return
+            raise RuntimeError
 
-        self._update_rate_pidget.set_parameter(self._session_config.update_rate)
-
-    def set_selected_sensor(self, sensor_id: Optional[int], sensor_list: list[int]) -> None:
-        self._sensor_id_pidget.set_selected_sensor(sensor_id, sensor_list)
+        config = a121.SessionConfig(
+            {self._session_config.sensor_id: sensor_config},
+            update_rate=self._session_config.update_rate,
+            extended=self._session_config.extended,
+        )
+        self.set_data(config)
+        self.sig_update.emit(config)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import copy
 import logging
 from functools import partial
 from typing import Any, Optional
 
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from . import pidgets
 from .collapsible_widget import CollapsibleWidget
+from .data_editor import DataEditor
 from .range_help_view import RangeHelpView
 from .types import PidgetFactoryMapping
 
 
 log = logging.getLogger(__name__)
 
 
-class SubsweepConfigEditor(QWidget):
+class SubsweepConfigEditor(DataEditor[Optional[a121.SubsweepConfig]]):
     sig_update = Signal(object)
 
     _subsweep_config: Optional[a121.SubsweepConfig]
 
     _subsweep_config_pidgets: dict[str, pidgets.Pidget]
     _erroneous_aspects: set[str]
 
@@ -124,86 +126,52 @@
             pidget = factory.create(self)
 
             if aspect in self.ADVANCED_PARAMETERS:
                 collapsible_layout.addWidget(pidget)
             else:
                 self.layout().addWidget(pidget)
 
-            pidget.sig_parameter_changed.connect(
-                partial(self._update_subsweep_config_aspect, aspect)
-            )
+            pidget.sig_update.connect(partial(self._update_subsweep_config_aspect, aspect))
 
             self._subsweep_config_pidgets[aspect] = pidget
 
         # Some left margin here will show the hierarchy
         collapsible_layout.setContentsMargins(11, 0, 0, 0)
         dummy = QWidget()
         dummy.setLayout(collapsible_layout)
         self.layout().addWidget(
             CollapsibleWidget(
                 label="Advanced",
                 widget=dummy,
             )
         )
 
-    def sync(self) -> None:
-        self._update_ui()
+    def set_read_only(self, read_only: bool) -> None:
+        for pidget in self._subsweep_config_pidgets.values():
+            pidget.setEnabled(not read_only)
 
-    def _update_ui(self) -> None:
-        if self._subsweep_config is None:
-            log.debug("could not update ui as SubsweepConfig is None")
+    def set_data(self, subsweep_config: Optional[a121.SubsweepConfig]) -> None:
+        if self._subsweep_config == subsweep_config:
             return
 
-        self._subsweep_config_pidgets["start_point"].set_parameter(
-            self._subsweep_config.start_point
-        )
-        self._subsweep_config_pidgets["num_points"].set_parameter(self._subsweep_config.num_points)
-        self._subsweep_config_pidgets["step_length"].set_parameter(
-            self._subsweep_config.step_length
-        )
-        self._subsweep_config_pidgets["profile"].set_parameter(self._subsweep_config.profile)
-        self._subsweep_config_pidgets["hwaas"].set_parameter(self._subsweep_config.hwaas)
-        self._subsweep_config_pidgets["receiver_gain"].set_parameter(
-            self._subsweep_config.receiver_gain
-        )
-        self._subsweep_config_pidgets["enable_tx"].set_parameter(self._subsweep_config.enable_tx)
-        self._subsweep_config_pidgets["enable_loopback"].set_parameter(
-            self._subsweep_config.enable_loopback
-        )
-        self._subsweep_config_pidgets["phase_enhancement"].set_parameter(
-            self._subsweep_config.phase_enhancement
-        )
-        self._subsweep_config_pidgets["prf"].set_parameter(self._subsweep_config.prf)
-
-    def set_data(self, subsweep_config: Optional[a121.SubsweepConfig]) -> None:
         self.range_help_view.update(subsweep_config)
         self._subsweep_config = subsweep_config
 
-    @property
-    def is_ready(self) -> bool:
-        return self._erroneous_aspects == set()
-
-    def set_read_only(self, read_only: bool) -> None:
-        for pidget in self._subsweep_config_pidgets.values():
-            pidget.setEnabled(not read_only)
-
-    def _update_subsweep_config_aspect(self, aspect: str, value: Any) -> None:
+        self.setEnabled(self._subsweep_config is not None)
         if self._subsweep_config is None:
-            raise TypeError("SubsweepConfig is None")
+            log.debug("could not update ui as SubsweepConfig is None")
+            return
 
-        try:
-            setattr(self._subsweep_config, aspect, value)
-        except Exception as e:
-            self._erroneous_aspects.add(aspect)
-            self._subsweep_config_pidgets[aspect].set_note_text(e.args[0], Criticality.ERROR)
-        else:
+        for aspect, pidget in self._subsweep_config_pidgets.items():
             if aspect in self._erroneous_aspects:
-                self._erroneous_aspects.remove(aspect)
+                continue
+            pidget.set_data(getattr(self._subsweep_config, aspect))
 
-        self._broadcast()
+    def get_data(self) -> Optional[a121.SubsweepConfig]:
+        return copy.deepcopy(self._subsweep_config)
 
     def handle_validation_results(
         self, results: list[a121.ValidationResult]
     ) -> list[a121.ValidationResult]:
         for aspect, pidget in self._subsweep_config_pidgets.items():
             if aspect not in self._erroneous_aspects:
                 pidget.set_note_text("")
@@ -212,14 +180,18 @@
 
         for result in results:
             if not self._handle_validation_result(result):
                 unhandled_results.append(result)
 
         return unhandled_results
 
+    @property
+    def is_ready(self) -> bool:
+        return self._erroneous_aspects == set()
+
     def _handle_validation_result(self, result: a121.ValidationResult) -> bool:
         if result.aspect is None or self._subsweep_config is None:
             return False
 
         if result.aspect in self._erroneous_aspects:
             # If there is an erroneous aspect in the GUI, we do not want to overwrite that.
             # Once the erroneous aspect is handled with, the same validation result will
@@ -232,9 +204,25 @@
             self._subsweep_config_pidgets[result.aspect].set_note_text(
                 result.message, result.criticality
             )
             result_handled = True
 
         return result_handled
 
-    def _broadcast(self) -> None:
-        self.sig_update.emit(self._subsweep_config)
+    def _update_subsweep_config_aspect(self, aspect: str, value: Any) -> None:
+        if self._subsweep_config is None:
+            raise TypeError("SubsweepConfig is None")
+
+        config = copy.deepcopy(self._subsweep_config)
+
+        try:
+            setattr(config, aspect, value)
+        except Exception as e:
+            self._erroneous_aspects.add(aspect)
+            self._subsweep_config_pidgets[aspect].set_note_text(e.args[0], Criticality.ERROR)
+
+            # this emit needs to be done to signal that "is_ready" has changed.
+            self.sig_update.emit(self.get_data())
+        else:
+            self._erroneous_aspects.discard(aspect)
+            self.set_data(config)
+            self.sig_update.emit(config)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
         self.setLayout(QHBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         self.layout().addWidget(self._sensor_id_pidget_1)
         self.layout().addWidget(self._sensor_id_pidget_2)
 
-        self._sensor_id_pidget_1.sig_parameter_changed.connect(
+        self._sensor_id_pidget_1.sig_update.connect(
             lambda sensor_id: self.handle_pidget_signal(sensor_id, sensor_id_position=0)
         )
-        self._sensor_id_pidget_2.sig_parameter_changed.connect(
+        self._sensor_id_pidget_2.sig_update.connect(
             lambda sensor_id: self.handle_pidget_signal(sensor_id, sensor_id_position=1)
         )
         self.sensor_ids = None
 
     def set_selected_sensors(
         self, sensor_ids: t.Optional[list[int]], sensor_list: list[int]
     ) -> None:
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_components/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/plugin_components/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/plugin_widget.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import importlib.resources
 import logging
 from enum import Enum
@@ -28,17 +28,21 @@
 
 import pyqtgraph as pg
 
 from acconeer.exptool.app import resources  # type: ignore[attr-defined]
 from acconeer.exptool.app.new._enums import PluginFamily
 from acconeer.exptool.app.new.app_model import AppModel, PluginPresetSpec, PluginSpec
 from acconeer.exptool.app.new.pluginbase import PlotPluginBase, PluginSpecBase
-
-from .plugin_components.utils import VerticalGroupBox
-from .utils import HorizontalSeparator, ScrollAreaDecorator, TopAlignDecorator
+from acconeer.exptool.app.new.ui.icons import ARROW_LEFT_BOLD
+from acconeer.exptool.app.new.ui.plugin_components.utils import VerticalGroupBox
+from acconeer.exptool.app.new.ui.utils import (
+    HorizontalSeparator,
+    ScrollAreaDecorator,
+    TopAlignDecorator,
+)
 
 
 log = logging.getLogger(__name__)
 
 
 class PluginSelectionButton(QPushButton):
     plugin: PluginSpec
@@ -213,15 +217,15 @@
 
     def _select_module_text(self) -> QHBoxLayout:
         h_box = QHBoxLayout()
         h_box.addStretch(1)
 
         icon_widget = qta.IconWidget()
         icon_widget.setIconSize(QtCore.QSize(36, 36))
-        icon_widget.setIcon(qta.icon("ph.arrow-left-bold", color="#4d5157"))
+        icon_widget.setIcon(ARROW_LEFT_BOLD(color="#4d5157"))
 
         label = QLabel("Select a module to begin", self)
         label.setStyleSheet("font-size: 20px;")
         label.setAlignment(QtCore.Qt.AlignCenter)
 
         h_box.addWidget(icon_widget)
         h_box.addWidget(label)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/recording_widget.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Optional
 
-import qtawesome as qta
-
 from PySide6 import QtCore, QtGui
 from PySide6.QtWidgets import QCheckBox, QFileDialog, QHBoxLayout, QPushButton, QWidget
 
 from acconeer.exptool.app.new.app_model import AppModel
-
-from .misc import BUTTON_ICON_COLOR
+from acconeer.exptool.app.new.ui.icons import FOLDER_OPEN, SAVE
 
 
 class RecordingWidget(QWidget):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setLayout(QHBoxLayout(self))
@@ -83,15 +80,15 @@
 
 
 class LoadFileButton(FileButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(
             app_model,
             "Load from file",
-            qta.icon("fa.folder-open", color=BUTTON_ICON_COLOR),
+            FOLDER_OPEN(),
             "Ctrl+o",
             "Load a previously recorded and saved session and play it back",
             parent,
         )
         app_model.sig_notify.connect(self._on_app_model_update)
 
     def _on_app_model_update(self, app_model: AppModel) -> None:
@@ -112,15 +109,15 @@
 
 
 class SaveFileButton(FileButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(
             app_model,
             "Save to file",
-            qta.icon("mdi.content-save", color=BUTTON_ICON_COLOR),
+            SAVE(),
             "Ctrl+s",
             "Save the current session",
             parent,
         )
         app_model.sig_notify.connect(self._on_app_model_update)
 
     def _on_app_model_update(self, app_model: AppModel) -> None:
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,298 +1,351 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
-from __future__ import annotations
+from collections import namedtuple
 
-import threading
-from typing import Optional
-
-import numpy as np
-import qtawesome as qta
-
-from PySide6 import QtCore
-from PySide6.QtGui import QPainter, QPaintEvent, QTextDocument
+from PySide6 import QtCore, QtWidgets
+from PySide6.QtGui import QPixmap
 from PySide6.QtWidgets import (
+    QCheckBox,
+    QDialog,
+    QFrame,
+    QGridLayout,
     QHBoxLayout,
     QLabel,
-    QMainWindow,
-    QStatusBar,
-    QStyle,
-    QStyleOption,
-    QTextBrowser,
+    QPushButton,
+    QSpinBox,
+    QToolButton,
+    QVBoxLayout,
     QWidget,
 )
 
-import acconeer.exptool
-from acconeer.exptool.app.new import check_package_outdated, get_latest_changelog
-from acconeer.exptool.app.new.app_model import AppModel
-from acconeer.exptool.utils import get_module_version  # type: ignore[import]
-
-from .misc import BUTTON_ICON_COLOR
-
 
-class FrameCountLabel(QLabel):
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
+class AdvancedSerialDialog(QDialog):
+    def __init__(self, state, parent):
         super().__init__(parent)
 
-        self.setToolTip("Number of received frames")
+        self.setMinimumWidth(350)
+        self.setModal(True)
+        self.setWindowTitle("Advanced serial settings")
+
+        layout = QVBoxLayout()
+        self.setLayout(layout)
+
+        texts = [
+            "Please note:",
+            (
+                "Overriding the baud rate disables automatic"
+                " detection and negotiation of baud rate."
+            ),
+            "Only use on special hardware.",
+        ]
 
-        app_model.sig_frame_count.connect(self._on_app_model_frame_count)
-        self._on_app_model_frame_count(None)
+        for text in texts:
+            lbl = QLabel(text, self)
+            lbl.setWordWrap(True)
+            layout.addWidget(lbl)
 
-    def _on_app_model_frame_count(self, frame_count: Optional[int]) -> None:
-        if frame_count is None:
-            css = "color: #888;"
-            text = "Frames: -    "
-        else:
-            css = ""
-            text = f"Frames: {frame_count:5}"
+        layout.addStretch(1)
 
-        self.setStyleSheet(f"QWidget{{{css}}}")
-        self.setText(text)
+        self.cb = QCheckBox("Override baud rate", self)
+        self.cb.stateChanged.connect(self.cb_state_changed)
+        layout.addWidget(self.cb)
 
+        self.sb = QSpinBox(self)
+        self.sb.setRange(1, int(3e6))
+        layout.addWidget(self.sb)
 
-class RateStatsLabel(QLabel):
-    _FPS: int = 10
+        layout.addStretch(1)
 
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
+        buttons_widget = QWidget(self)
+        layout.addWidget(buttons_widget)
+        hbox = QHBoxLayout()
+        buttons_widget.setLayout(hbox)
+        hbox.addStretch(1)
+        cancel_btn = QPushButton("Cancel")
+        cancel_btn.clicked.connect(self.reject)
+        hbox.addWidget(cancel_btn)
+        save_btn = QPushButton("Save")
+        save_btn.setDefault(True)
+        save_btn.clicked.connect(self.accept)
+        hbox.addWidget(save_btn)
 
-        self.setToolTip("Reported update rate")
+        self.set_state(state)
 
-        self.rate = np.nan
-        self.rate_warning = False
+    def cb_state_changed(self, state):
+        self.sb.setEnabled(bool(state))
 
-        self.startTimer(int(1000 / self._FPS))
+    def set_state(self, state):
+        checked = state is not None
+        self.cb.setChecked(checked)
+        self.cb_state_changed(checked)
+        self.sb.setValue(state if checked else 115200)
 
-        app_model.sig_rate_stats.connect(self._on_app_model_rate_stats)
+    def get_state(self):
+        return self.sb.value() if self.cb.isChecked() else None
 
-    def timerEvent(self, event: QtCore.QTimerEvent) -> None:
-        if np.isnan(self.rate):
-            css = "color: #888;"
-            text = "     - Hz"
-        else:
-            css = "color: #FD5200;" if self.rate_warning else ""
-            text = f"{self.rate:>6.1f} Hz"
 
-        self.setStyleSheet(f"QWidget{{{css}}}")
-        self.setText(text)
+class BiggerMessageBox(QtWidgets.QMessageBox):
+    def resizeEvent(self, event):
+        result = super().resizeEvent(event)
+        self.setFixedWidth(500)
+        return result
 
-    def _on_app_model_rate_stats(
-        self,
-        rate: float,
-        rate_warning: bool,
-        jitter: float,
-        jitter_warning: bool,
-    ) -> None:
-        self.rate = rate
-        self.rate_warning = rate_warning
 
+class Label(QLabel):
+    def __init__(self, img, img_scale=0.7):
+        super(Label, self).__init__()
 
-class JitterStatsLabel(QLabel):
-    _FPS: int = 10
+        self.img_scale = img_scale
+        self.pixmap = QPixmap(img)
 
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
-
-        self.setToolTip("Reported jitter")
+        self.setMinimumSize(1, 1)
+        self.setAlignment(QtCore.Qt.AlignVCenter | QtCore.Qt.AlignHCenter)
+        self.setPixmap(self.pixmap)
 
-        self.jitter = np.nan
-        self.jitter_warning = False
+    def resizeEvent(self, event):
+        w = int(round(self.size().width() * self.img_scale))
+        h = int(round(self.size().height() * self.img_scale))
+        scaled_size = QtCore.QSize(w, h)
 
-        self.startTimer(int(1000 / self._FPS))
+        scaled_pixmap = self.pixmap.scaled(
+            scaled_size,
+            QtCore.Qt.KeepAspectRatio,
+            QtCore.Qt.SmoothTransformation,
+        )
 
-        app_model.sig_rate_stats.connect(self._on_app_model_rate_stats)
-
-    def timerEvent(self, event: QtCore.QTimerEvent) -> None:
-        if np.isnan(self.jitter):
-            css = "color: #888;"
-            text = "    - ms"
-        else:
-            css = "color: #FD5200;" if self.jitter_warning else ""
-            text = f"{self.jitter * 1e3:5.1f} ms"
+        self.setPixmap(scaled_pixmap)
 
-        self.setStyleSheet(f"QWidget{{{css}}}")
-        self.setText(text)
 
-    def _on_app_model_rate_stats(
-        self,
-        rate: float,
-        rate_warning: bool,
-        jitter: float,
-        jitter_warning: bool,
-    ) -> None:
-        self.jitter = jitter
-        self.jitter_warning = jitter_warning
+class CollapsibleSection(QFrame):
+    def __init__(self, header_text, init_collapsed=False, is_top=False):
+        super().__init__()
 
+        if not is_top:
+            self.setObjectName("CollapsibleSection")
+            self.setStyleSheet("#CollapsibleSection{border-top: 1px solid lightgrey;}")
+
+        self._layout = QVBoxLayout(self)
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self._layout.setSpacing(0)
+        self.setLayout(self._layout)
+        self._header_widget = QWidget()
+        self.body_widget = QWidget()
+        self._layout.addWidget(self._header_widget)
+        self._layout.addWidget(self.body_widget)
+
+        self.grid = QGridLayout(self.body_widget)
+        self.grid.setContentsMargins(9, 0, 9, 9)
+        self.grid.setColumnStretch(0, 1)
+        self.grid.setColumnStretch(1, 1)
+
+        self._header_widget_layout = QHBoxLayout(self._header_widget)
+        self._header_widget_layout.setContentsMargins(7, 7, 7, 7)
+        self._header_widget.setLayout(self._header_widget_layout)
+
+        self._button = QToolButton()
+        self._button.setText(header_text)
+        self._button.setCheckable(True)
+        self._button.setStyleSheet("QToolButton { border: none; }")
+        self._button.setToolButtonStyle(QtCore.Qt.ToolButtonTextBesideIcon)
+        self._button.pressed.connect(self.button_event)
+        self.button_event(override=init_collapsed)
+        self._header_widget_layout.addWidget(self._button)
+        self._header_widget_layout.addStretch()
+
+    def button_event(self, override=None):
+        if override is None:
+            checked = not self._button.isChecked()
+        else:
+            checked = override
+            self._button.setChecked(checked)
 
-class BackendCPUPercentLabel(QLabel):
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
+        if checked:  # collapsed
+            self._button.setArrowType(QtCore.Qt.ArrowType.RightArrow)
+            self.body_widget.hide()
+        else:
+            self._button.setArrowType(QtCore.Qt.ArrowType.DownArrow)
+            self.body_widget.show()
 
-        self.setToolTip("Client process CPU load")
 
-        app_model.sig_backend_cpu_percent.connect(self._on_app_model_backend_cpu_percent)
+class SensorSelection(QFrame):
+    def __init__(self, multi_sensors=False, error_handler=None, callback=None):
+        super().__init__()
 
-        self._on_app_model_backend_cpu_percent(0)
+        self.error_handler = error_handler
+        self.callback = callback
 
-    def _on_app_model_backend_cpu_percent(self, cpu_percent: int) -> None:
-        self.setText(f"CPU: {cpu_percent:3}%")
+        self.drawing = False
+        self.selected = [1]
+        self.sources = None
+        self.module_multi_sensor_support = multi_sensors
+
+        self.grid = QtWidgets.QGridLayout(self)
+        self.grid.setContentsMargins(0, 0, 0, 0)
+
+        self.checkboxes = []
+        self.radio_buttons = []
+        for i in range(4):
+            s = i + 1
+
+            cb = QCheckBox(str(s), self)
+            cb.stateChanged.connect(lambda val, cb=cb: self.checkbox_event_handler(val, cb))
+            self.checkboxes.append(cb)
+            self.grid.addWidget(cb, 0, i)
+
+            rb = QtWidgets.QRadioButton(str(s), self)
+            rb.toggled.connect(lambda val, rb=rb: self.radio_button_event_handler(val, rb))
+            self.radio_buttons.append(rb)
+            self.grid.addWidget(rb, 1, i)
+
+        self.draw()
+
+    def checkbox_event_handler(self, state, cb):
+        if self.drawing:
+            return
+
+        s = int(cb.text())
+
+        if state:  # checked
+            if s not in self.selected:
+                self.selected.insert(0, s)
+        else:
+            if s in self.selected:
+                self.selected.remove(s)
 
-        css = "color: #FD5200;" if cpu_percent >= 85 else ""
-        self.setStyleSheet(f"QWidget{{{css}}}")
+        self.draw()
 
+    def radio_button_event_handler(self, selected, rb):
+        if self.drawing or not selected:
+            return
 
-class RSSVersionLabel(QLabel):
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
+        s = int(rb.text())
+        self.selected = [s]
+        self.draw()
 
-        app_model.sig_notify.connect(self._on_app_model_update)
+    def draw(self):
+        self.drawing = True
 
-    def _on_app_model_update(self, app_model: AppModel) -> None:
-        if app_model.rss_version is None:
-            css = "color: #888;"
-            text = "RSS: <not connected>"
-            tooltip = ""
-        else:
-            text = f"RSS: {app_model.rss_version}"
+        for i, (cb, rb) in enumerate(zip(self.checkboxes, self.radio_buttons)):
+            s = i + 1
 
-            if app_model.connection_warning:
-                css = "background-color: #D78100; color: #e2e2e2;"
-                tooltip = app_model.connection_warning
+            if self.sources:
+                enabled = s in self.sources
             else:
-                css = ""
-                tooltip = ""
-
-        self.setToolTip(tooltip)
-        self.setStyleSheet(f"QWidget{{{css}}}")
-        self.setText(text)
-
+                enabled = True
 
-class VersionLabel(QWidget):
-    sig_version_outdated = QtCore.Signal()
+            cb.setEnabled(enabled)
+            rb.setEnabled(enabled)
 
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
-
-        self.parent = parent
-        h_layout = QHBoxLayout()
-        self.setLayout(h_layout)
-        h_layout.setContentsMargins(0, 0, 0, 0)
-        h_layout.setSpacing(0)
-
-        et_version = get_module_version(acconeer.exptool)
-        et_version_text = f"ET: {et_version}"
-        et_version_label = QLabel(et_version_text, self)
-        h_layout.addWidget(et_version_label)
-
-        def version_check(et_version: str) -> None:
-            version_outdated, latest_v = check_package_outdated("acconeer-exptool", et_version)
-            self.changelog = None
-
-            if version_outdated:
-                self.changelog = get_latest_changelog()
-                self.setStyleSheet(
-                    f"QWidget{{background-color: {BUTTON_ICON_COLOR}; color: #e2e2e2}}"
-                )
-
-                self.setToolTip(
-                    "There is a new software version available!\n"
-                    f"The latest version is: {latest_v}. \n"
-                    "Click to view changelog."
-                )
-                self.sig_version_outdated.emit()
-                self.mousePressEvent = self._toggle_changelog
-
-        self.sig_version_outdated.connect(self._create_changelog_window)
-        self.sig_version_outdated.connect(lambda: self._add_icon_to_version_label(self))
-
-        version_thread = threading.Thread(target=lambda: version_check(et_version))
-        version_thread.start()
-
-    def _create_changelog_window(self) -> None:
-        if self.changelog is not None:
-            self.cl_window = ChangelogWindow(self)
-            self.cl_window.set_text(self.changelog)
-
-    def _add_icon_to_version_label(self, version_widget: QWidget) -> None:
-        layout = version_widget.layout()
-        icon_widget = qta.IconWidget()
-        icon_widget.setIcon(qta.icon("fa.refresh", color="#e2e2e2"))
-        layout.addWidget(icon_widget)
-
-    def _toggle_changelog(self, label: QLabel) -> None:
-        if self.changelog is not None:
-            self.cl_window.setVisible(not self.cl_window.isVisible())
-
-    def paintEvent(self, pe: QPaintEvent) -> None:
-        o = QStyleOption()
-        o.initFrom(self)
-        p = QPainter(self)
-        self.style().drawPrimitive(QStyle.PE_Widget, o, p, self)
+            cb.setVisible(bool(self.module_multi_sensor_support))
+            rb.setVisible(not bool(self.module_multi_sensor_support))
 
+        for i, cb in enumerate(self.checkboxes):
+            s = i + 1
+            cb.setChecked(s in self.selected)
+            rb.setChecked(False)
 
-class StatusBar(QStatusBar):
-    def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent)
+        if self.selected:
+            self.radio_buttons[self.selected[0] - 1].setChecked(True)
 
-        self.parent = parent
+        self.drawing = False
 
-        app_model.sig_status_message.connect(self._on_app_model_status_message)
+        if self.callback is not None:
+            self.callback()
 
-        self.message_timer = QtCore.QTimer(self)
-        self.message_timer.setInterval(3000)
-        self.message_timer.setSingleShot(True)
-        self.message_timer.timeout.connect(self._on_timer)
-
-        self.message_widget = QLabel(self)
-        self.addWidget(self.message_widget)
-
-        self.addPermanentWidget(FrameCountLabel(app_model, self))
-        self.addPermanentWidget(RateStatsLabel(app_model, self))
-        self.addPermanentWidget(JitterStatsLabel(app_model, self))
-        self.addPermanentWidget(BackendCPUPercentLabel(app_model, self))
-        self.addPermanentWidget(RSSVersionLabel(app_model, self))
-        self.addPermanentWidget(VersionLabel(app_model, self))
-
-        font_families = [
-            "Consolas",  # Windows
-            "Droid Sans Mono",  # Ubuntu
-            "DejaVu Sans Mono",  # Ubuntu, backup
-            "SF Mono",  # Mac
-        ]
-        font_family = ", ".join(f'"{ff}"' for ff in font_families)
-        self.setStyleSheet(f"QWidget{{font-family: {font_family};}}")
+    def sanitize(self):
+        if self.sources:
+            self.selected = [s for s in self.selected if s in self.sources]
 
-    def _on_app_model_status_message(self, message: Optional[str]) -> None:
-        self.message_timer.stop()
-
-        if message:
-            self.message_widget.setText(message)
-            self.message_timer.start()
+        if self.module_multi_sensor_support:
+            if isinstance(self.module_multi_sensor_support, list):
+                lim = self.module_multi_sensor_support[1]
+                self.selected = self.selected[:lim]
         else:
-            self.message_widget.clear()
+            if self.selected:
+                self.selected = [self.selected[0]]
 
-    def _on_timer(self) -> None:
-        self.message_widget.clear()
+    def get_sensors(self):
+        return list(sorted(self.selected))
 
+    def set_sensors(self, sensors):
+        self.selected = sensors
+        self.sanitize()
+        self.draw()
+
+    def set_multi_sensor_support(self, sources, module_multi_sensor_support):
+        self.sources = sources
+        self.module_multi_sensor_support = module_multi_sensor_support
+        self.sanitize()
+        self.draw()
+
+
+class SessionInfoView(QWidget):
+    Field = namedtuple("Field", ["label", "unit", "fmt_str", "get_fun"])
+
+    FIELDS = [
+        Field("Actual range start", "m", "{:.3f}", lambda d: d["range_start_m"]),
+        Field("Actual range length", "m", "{:.3f}", lambda d: d["range_length_m"]),
+        Field(
+            "Actual range end",
+            "m",
+            "{:.3f}",
+            lambda d: d["range_start_m"] + d["range_length_m"],
+        ),
+        Field("Step length", "mm", "{:.2f}", lambda d: d["step_length_m"] * 1e3),
+        Field("Number of data points", "", "{}", lambda d: d["data_length"]),
+        Field("Sweep rate", "Hz", "{:.0f}", lambda d: d["sweep_rate"]),
+        Field("Stitch count", "", "{}", lambda d: d["stitch_count"]),
+        Field("Depth LPF cutoff ratio", "", "{:.6f}", lambda d: d["depth_lowpass_cutoff_ratio"]),
+    ]
 
-class ChangelogWindow(QMainWindow):
-    def __init__(self, parent: QWidget = None) -> None:
-        super().__init__()
+    def __init__(self, parent):
+        super().__init__(parent)
 
-        self.setWindowTitle("Changelog")
-        self.text_browser = QTextBrowser()
-        self.setCentralWidget(self.text_browser)
-        self.set_center(parent.parent.parent)
-        self.showEvent = lambda _: self.set_center(parent.parent.parent)
-
-    def set_text(self, text: str) -> None:
-        document = QTextDocument()
-        document.setMarkdown(text)
-        self.text_browser.setDocument(document)
-
-    def set_center(self, main_window: QMainWindow) -> None:
-        fg = self.frameGeometry()
-        fg.moveCenter(main_window.geometry().center())
-        self.move(fg.topLeft())
-        self.resize(500, 400)
+        grid = QGridLayout(self)
+        grid.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(grid)
+
+        self.field_widgets = []
+        for i, field in enumerate(self.FIELDS):
+            key_lbl = QLabel(field.label, self)
+            val_lbl = QLabel("", self)
+            unit_lbl = QLabel(field.unit, self)
+            grid.addWidget(key_lbl, i, 0)
+            grid.addWidget(val_lbl, i, 1, QtCore.Qt.AlignRight)
+            grid.addWidget(unit_lbl, i, 2)
+            self.field_widgets.append((key_lbl, val_lbl, unit_lbl))
+
+        self.no_info_lbl = QLabel("No active or buffered session", self)
+        grid.addWidget(self.no_info_lbl, i + 1, 0, 1, 3)
+
+        self.update()
+
+    def update(self, info=None):
+        self.no_info_lbl.setVisible(not info)
+
+        for field, widgets in zip(self.FIELDS, self.field_widgets):
+            try:
+                val = field.get_fun(info)
+                text = field.fmt_str.format(val)
+            except Exception:
+                text = None
+
+            for w in widgets:
+                w.setVisible(bool(text))
+
+            widgets[1].setText(str(text))
+
+
+class QHLine(QFrame):
+    def __init__(self):
+        super(QHLine, self).__init__()
+        self.setFrameShape(QFrame.HLine)
+        self.setFrameShadow(QFrame.Sunken)
+
+
+class QVLine(QFrame):
+    def __init__(self):
+        super(QVLine, self).__init__()
+        self.setFrameShape(QFrame.VLine)
+        self.setFrameShadow(QFrame.Sunken)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 from __future__ import annotations
 
 from typing import Optional
 
 from PySide6 import QtCore
-from PySide6.QtWidgets import QFrame, QScrollArea, QVBoxLayout, QWidget
+from PySide6.QtWidgets import QFrame, QLayout, QScrollArea, QVBoxLayout, QWidget
 
 
 class ScrollAreaDecorator(QScrollArea):
     def __init__(self, decoratee: QWidget) -> None:
         """Puts `decoratee` in a frameless QScrollArea with no horizontal scroll."""
         super().__init__()
 
@@ -30,11 +30,17 @@
         self.setLayout(layout)
 
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(decoratee)
         layout.addStretch(1)
 
 
+class LayoutWrapper(QWidget):
+    def __init__(self, wrappee: QLayout) -> None:
+        super().__init__()
+        self.setLayout(wrappee)
+
+
 class HorizontalSeparator(QFrame):
     def __init__(self, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
         self.setFrameShape(QFrame.HLine)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import importlib.resources
 import json
 import logging
@@ -2197,52 +2197,45 @@
 def watchdog(event):
     flag = event.wait(1)
     if not flag:
         print("\nforcing exit...")
         os._exit(1)
 
 
-def remove_user_data_files():
-    """Removes all files under USER_DATA_DIR interactively"""
-    user_data_dir = pathlib.Path(USER_DATA_DIR)
-    if not user_data_dir.exists():
-        print(f'Config folder ("{user_data_dir}") does not exists.')
+def remove_last_config():
+    """Interacively removes last_config.npy from user data dirs"""
+    file = pathlib.Path(LAST_CONF_FILENAME)
+    if not file.exists():
+        print(f'Config file ("{file}") does not exists.')
         print("Nothing will be done.")
         return
 
-    if not any(user_data_dir.iterdir()):
-        print(f'There exists no files under "{user_data_dir}".')
-        print("Nothing will be done.")
-        return
-
-    print("Proceeding will remove the following files:\n")
-    for file in user_data_dir.iterdir():
-        print(f"    * {file}")
+    print("Proceeding will remove the following file:\n")
+    print(f"    * {file}")
     print()
 
     choice = input("Continue? [y/N] ")
     should_remove = choice.lower().startswith("y")
     if should_remove:
-        for file in user_data_dir.iterdir():
-            file.unlink()  # unlink <=> rm
-            print(f'Removed "{file}"')
+        file.unlink()  # unlink <=> rm
+        print(f'Removed "{file}"')
     else:
         print("Nothing was removed.")
 
 
 def main():
     et.utils.config_logging(level=logging.INFO)
 
     # Enable warnings to be printed to the log, e.g. DeprecationWarning
     warnings.simplefilter("module")
 
     args = ExptoolArgumentParser().parse_args()
 
     if args.purge_config:
-        remove_user_data_files()
+        remove_last_config()
         sys.exit(0)
 
     if args.use_last_config:
         if not os.path.exists(USER_DATA_DIR):
             log.info(f"Creating folder {USER_DATA_DIR}")
 
         os.makedirs(USER_DATA_DIR, exist_ok=True)
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-6.0.5/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-6.0.5/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,24 +221,41 @@
                     break
                 retries -= 1
 
             if not device_found:
                 raise ValueError("DFU device not found")
 
     @staticmethod
+    def _try_open_port(serial_port):
+        retries = 5
+        ser = None
+        while retries > 0 and ser is None:
+            try:
+                ser = serial.Serial(serial_port, exclusive=True)
+            except SerialException:
+                ser = None
+                time.sleep(0.2)
+                retries -= 1
+
+        if ser is None:
+            raise ValueError(f"Flash failed, {serial_port} cannot be opened")
+
+        return ser
+
+    @staticmethod
     def flash(device_port, device_name, image_path, progress_callback=None):
         """Flash an firmware image to the device"""
         BootloaderTool.enter_dfu(device_port)
         dfu_port = BootloaderTool._find_port(
             ACCONEER_VID, ACCONEER_XC120_BOOTLOADER_PID, device_port
         )
         usb_dfu = BootloaderTool._find_usb_dfu_device()
         serial_dev = None
         if dfu_port is not None:
-            serial_dev = serial.Serial(dfu_port, exclusive=True)
+            serial_dev = BootloaderTool._try_open_port(dfu_port)
         elif usb_dfu is not None and ComPort is not None:
             serial_dev = ComPort(
                 vid=usb_dfu.vid,
                 pid=usb_dfu.pid,
             )
         else:
             raise ValueError("Flash failed, device not found")
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer/exptool/utils.py` & `acconeer-exptool-6.0.5/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 6.0.4
+Version: 6.0.5
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-6.0.4/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-6.0.5/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -380,25 +380,29 @@
 src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
 src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
 src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
 src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
 src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
 src/acconeer/exptool/app/new/ui/__init__.py
 src/acconeer/exptool/app/new/ui/app_model_viewer.py
-src/acconeer/exptool/app/new/ui/connection_widget.py
-src/acconeer/exptool/app/new/ui/flash_widget.py
+src/acconeer/exptool/app/new/ui/device_comboboxes.py
+src/acconeer/exptool/app/new/ui/help_tab.py
+src/acconeer/exptool/app/new/ui/icons.py
 src/acconeer/exptool/app/new/ui/main_window.py
 src/acconeer/exptool/app/new/ui/misc.py
-src/acconeer/exptool/app/new/ui/plugin_widget.py
-src/acconeer/exptool/app/new/ui/recording_widget.py
 src/acconeer/exptool/app/new/ui/status_bar.py
 src/acconeer/exptool/app/new/ui/utils.py
+src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
 src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
 src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
@@ -406,14 +410,20 @@
 src/acconeer/exptool/app/new/ui/plugin_components/types.py
 src/acconeer/exptool/app/new/ui/plugin_components/utils.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
 src/acconeer/exptool/app/old/__init__.py
 src/acconeer/exptool/app/old/__main__.py
 src/acconeer/exptool/app/old/app.py
 src/acconeer/exptool/app/old/data_processing.py
 src/acconeer/exptool/app/old/elements/__init__.py
 src/acconeer/exptool/app/old/elements/helper.py
 src/acconeer/exptool/app/old/elements/modules.py
```

### Comparing `acconeer-exptool-6.0.4/tools/check_changelog.py` & `acconeer-exptool-6.0.5/tools/check_changelog.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,46 @@
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 from packaging.version import Version
 
 
-def utf8_subprocess_output(*args: str):
+VERSION_PATTERN = r"v?\d+\.\d+\.\d+"
+
+
+def utf8_subprocess_output(*args: str) -> str:
     return subprocess.check_output(args, encoding="utf-8").strip()
 
 
-def get_commit_sha_of_git_tag(git_tag: str):
+def get_commit_sha_of_git_tag(git_tag: str) -> str:
     return utf8_subprocess_output("git", "rev-list", "-n", "1", git_tag)
 
 
-def get_current_commit_sha():
+def get_current_commit_sha() -> str:
     return utf8_subprocess_output("git", "rev-parse", "--verify", "HEAD")
 
 
-def get_most_recent_git_tag():
+def get_current_commit_prepare_release_version() -> Optional[str]:
+    commit_title = utf8_subprocess_output("git", "log", "-n1", "--pretty=format:%s")
+    match = re.match(rf"Prepare release ({VERSION_PATTERN})", commit_title)
+    return None if match is None else match.groups()[0]
+
+
+def get_most_recent_git_tag() -> str:
     return utf8_subprocess_output("git", "describe", "--abbrev=0", "--tags")
 
 
+def get_current_commit_tag() -> Optional[str]:
+    recent_tag = get_most_recent_git_tag()
+    return (
+        recent_tag if get_current_commit_sha() == get_commit_sha_of_git_tag(recent_tag) else None
+    )
+
+
 def get_first_match_in_string(pattern: str, string: str, *, group: int = 0) -> Optional[str]:
     """
     Searches for the first match of `pattern` in `string`. Returns `group`:th group (default 0)
     """
     valid_group_numbers = range(0, re.compile(pattern).groups + 1)
 
     if group not in valid_group_numbers:
@@ -47,55 +63,50 @@
 
 def get_number_of_matches_in_string(pattern: str, string: str) -> int:
     match = re.findall(pattern, string)
 
     return len(match)
 
 
-def main():
-    VERSION_PATTERN = r"v?\d+\.\d+\.\d+"
+def main() -> None:
     FILE_PATH = "CHANGELOG.md"
     UNRELEASED_FILE_PATH = "UNRELEASED_CHANGELOG.md"
-    status = True
 
     changelog = Path(FILE_PATH)
     unreleased_changelog = Path(UNRELEASED_FILE_PATH)
 
+    status = True
+
     if get_number_of_matches_in_string(r"## Unreleased", changelog.read_text()) > 0:
         print("Changelog contains illegal 'Unreleased' headline")
         status = False
 
     if (
         get_number_of_matches_in_string(r"## " + VERSION_PATTERN, unreleased_changelog.read_text())
         > 0
     ):
-        print("Unreleased contains illegal version tag headline")
+        print("Unreleased Changelog contains illegal version tag headline")
         status = False
 
-    most_recent_tag = get_most_recent_git_tag()
-    most_recent_tag_commit_sha = get_commit_sha_of_git_tag(most_recent_tag)
-    current_commit_sha = get_current_commit_sha()
-
-    is_current_commit_tagged = most_recent_tag_commit_sha == current_commit_sha
-    if not is_current_commit_tagged:
-        exit(0 if status else 1)
+    # First, we check if this is a "Prepare release" commit.
+    # If it's not, we check if the current commit is tagged.
+    current_tag = get_current_commit_prepare_release_version() or get_current_commit_tag()
 
-    if Version(most_recent_tag).is_prerelease:
+    if current_tag is None or Version(current_tag).is_prerelease:
         exit(0 if status else 1)
 
-    print(f"Current commit ({current_commit_sha[:7]}) is tagged ({most_recent_tag}).")
+    print(f"Current commit is tagged ({current_tag}).")
 
     first_match = get_first_match_in_string(VERSION_PATTERN, changelog.read_text())
     print(f'Found "{first_match}" in {FILE_PATH}', end=" ... ")
 
-    is_exact_match = first_match == most_recent_tag
-    if is_exact_match:
-        print(f"Which matches {most_recent_tag} exactly.")
+    if first_match == current_tag:
+        print(f"Which matches {current_tag} exactly.")
     else:
-        print(f'Which does not match "{most_recent_tag}".')
+        print(f'Which does not match "{current_tag}".')
         status = False
 
     empty_unreleased_changelog = (
         "# Unreleased Changelog\n\n## Unreleased\n\n### Added\n\n### Changed\n\n### Fixed\n"
     )
 
     if unreleased_changelog.read_text() != empty_unreleased_changelog:
```

### Comparing `acconeer-exptool-6.0.4/tools/check_copyright.py` & `acconeer-exptool-6.0.5/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/tools/check_line_length.py` & `acconeer-exptool-6.0.5/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/tools/check_permissions.py` & `acconeer-exptool-6.0.5/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/tools/check_sdk_mentions.py` & `acconeer-exptool-6.0.5/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/tools/check_whitespace.py` & `acconeer-exptool-6.0.5/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/tools/update_regmap.py` & `acconeer-exptool-6.0.5/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-6.0.4/utils/convert_to_csv.py` & `acconeer-exptool-6.0.5/utils/convert_to_csv.py`

 * *Files identical despite different names*

