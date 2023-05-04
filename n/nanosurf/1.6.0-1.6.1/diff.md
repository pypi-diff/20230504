# Comparing `tmp/nanosurf-1.6.0.tar.gz` & `tmp/nanosurf-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanosurf-1.6.0.tar", last modified: Wed May  3 09:26:08 2023, max compression
+gzip compressed data, was "nanosurf-1.6.1.tar", last modified: Thu May  4 07:50:21 2023, max compression
```

## Comparing `nanosurf-1.6.0.tar` & `nanosurf-1.6.1.tar`

### file list

```diff
@@ -1,254 +1,269 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.411955 nanosurf-1.6.0/
--rw-rw-rw-   0        0        0     1067 2022-02-08 08:13:22.000000 nanosurf-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     6618 2023-05-03 09:26:08.411955 nanosurf-1.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.224955 nanosurf-1.6.0/nanosurf/
--rw-rw-rw-   0        0        0     1774 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-03 08:56:58.000000 nanosurf-1.6.0/nanosurf/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.211956 nanosurf-1.6.0/nanosurf/app/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.239957 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.240956 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/
--rw-rw-rw-   0        0        0      566 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.249956 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/
--rw-rw-rw-   0        0        0     2294 2023-02-17 17:06:00.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc
--rw-rw-rw-   0        0        0     2285 2023-04-14 11:38:45.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc
--rw-rw-rw-   0        0        0     2364 2023-05-03 07:22:11.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc
--rw-rw-rw-   0        0        0     1853 2023-02-17 16:53:51.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     1822 2023-05-03 07:22:11.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     1523 2023-02-17 17:00:32.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1361 2023-05-03 07:22:11.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     3319 2023-02-17 17:12:09.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc
--rw-rw-rw-   0        0        0     3400 2023-05-03 07:22:11.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc
--rw-rw-rw-   0        0        0     2670 2023-02-16 15:52:16.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     2086 2023-05-03 07:19:15.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py
--rw-rw-rw-   0        0        0     1843 2023-05-03 07:17:37.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py
--rw-rw-rw-   0        0        0      740 2023-05-03 07:16:24.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py
--rw-rw-rw-   0        0        0      893 2023-05-03 07:17:37.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py
--rw-rw-rw-   0        0        0     4204 2023-05-03 07:20:07.000000 nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.250954 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.251955 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json
--rw-rw-rw-   0        0        0     1462 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.255955 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.265954 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/
--rw-rw-rw-   0        0        0      195 2022-12-14 07:35:47.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      193 2022-09-19 09:03:09.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9770 2023-03-09 15:52:53.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9831 2023-04-14 09:26:40.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     5198 2023-03-09 15:52:53.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     4006 2023-04-14 09:26:21.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     5181 2023-02-03 08:34:04.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     5236 2023-04-14 09:26:21.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1930 2022-12-14 07:35:47.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1768 2023-04-14 09:09:22.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0    13848 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py
--rw-rw-rw-   0        0        0     4907 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py
--rw-rw-rw-   0        0        0     5067 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py
--rw-rw-rw-   0        0        0     1310 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.266955 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.267957 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.272955 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.283955 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/
--rw-rw-rw-   0        0        0      194 2022-12-16 09:42:02.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      192 2022-09-16 14:32:05.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5443 2023-03-09 14:29:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc
--rw-rw-rw-   0        0        0     5291 2023-04-14 12:04:20.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc
--rw-rw-rw-   0        0        0     9703 2023-03-09 14:29:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9667 2023-04-14 12:04:20.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     9829 2023-02-08 13:02:32.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc
--rw-rw-rw-   0        0        0     9723 2023-04-14 12:06:14.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3005 2023-02-08 13:02:33.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2991 2023-04-14 12:01:18.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     5067 2023-03-09 14:29:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3662 2023-04-14 12:04:20.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     7030 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py
--rw-rw-rw-   0        0        0    13971 2023-05-03 08:56:03.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py
--rw-rw-rw-   0        0        0    10552 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py
--rw-rw-rw-   0        0        0     2397 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py
--rw-rw-rw-   0        0        0     3943 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py
--rw-rw-rw-   0        0        0     1580 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.284955 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.285955 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/.vscode/
--rw-rw-rw-   0        0        0      566 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json
--rw-rw-rw-   0        0        0     1431 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.290954 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.299955 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/
--rw-rw-rw-   0        0        0      199 2022-12-16 13:29:49.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      197 2022-11-15 07:27:23.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9252 2023-02-16 16:05:23.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     9276 2023-04-14 12:27:20.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     6662 2023-02-16 16:05:23.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     6564 2023-04-14 12:24:00.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     2314 2023-01-25 08:22:47.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2322 2023-04-14 12:24:00.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     4594 2023-03-13 14:19:52.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3455 2023-04-14 12:24:00.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc
--rw-rw-rw-   0        0        0    13358 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py
--rw-rw-rw-   0        0        0     7055 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py
--rw-rw-rw-   0        0        0     4533 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.300955 nanosurf-1.6.0/nanosurf/app/app_template/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.301954 nanosurf-1.6.0/nanosurf/app/app_template/.vscode/
--rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/app/app_template/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.306955 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.318955 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/
--rw-rw-rw-   0        0        0      176 2022-12-16 15:19:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      192 2023-01-25 09:01:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      174 2022-09-19 08:10:48.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6384 2023-02-07 10:44:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0    13859 2023-01-25 09:01:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc
--rw-rw-rw-   0        0        0     6336 2023-04-14 08:47:57.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     5392 2023-02-09 07:59:12.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     9403 2023-01-25 09:01:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc
--rw-rw-rw-   0        0        0     5327 2023-04-14 08:43:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1797 2022-12-16 15:19:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     2652 2023-01-25 09:01:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc
--rw-rw-rw-   0        0        0     1634 2023-04-14 08:43:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     2896 2023-02-07 10:44:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     5326 2023-01-25 09:01:50.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc
--rw-rw-rw-   0        0        0     2570 2023-04-14 08:47:57.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     7820 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/gui.py
--rw-rw-rw-   0        0        0     5134 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/module.py
--rw-rw-rw-   0        0        0     1160 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/settings.py
--rw-rw-rw-   0        0        0     2617 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/demo_module/worker_task.py
--rw-rw-rw-   0        0        0     1673 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/app_template/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.320954 nanosurf-1.6.0/nanosurf/app/demo_creating_spec_pos_table_with_smiley/
--rw-rw-rw-   0        0        0     4446 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb
--rw-rw-rw-   0        0        0     2457 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.322955 nanosurf-1.6.0/nanosurf/app/demo_lateral_force_signal_calibration/
--rw-rw-rw-   0        0        0    54597 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.323955 nanosurf-1.6.0/nanosurf/app/demo_move_sample_stage/
--rw-rw-rw-   0        0        0     7665 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.325954 nanosurf-1.6.0/nanosurf/app/demo_spec_setup_and_data_plotting/
--rw-rw-rw-   0        0        0   121398 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb
--rw-rw-rw-   0        0        0     2294 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.326956 nanosurf-1.6.0/nanosurf/app/demo_studio_scripting/
--rw-rw-rw-   0        0        0     4735 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py
--rw-rw-rw-   0        0        0     1817 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.330955 nanosurf-1.6.0/nanosurf/app/spm_template/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.331954 nanosurf-1.6.0/nanosurf/app/spm_template/.vscode/
--rw-rw-rw-   0        0        0      566 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/.vscode/launch.json
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.341954 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/
--rw-rw-rw-   0        0        0     7537 2023-03-22 08:49:37.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc
--rw-rw-rw-   0        0        0     7506 2023-04-14 11:57:53.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc
--rw-rw-rw-   0        0        0     3307 2023-03-22 08:30:27.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     3320 2023-04-14 09:59:56.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc
--rw-rw-rw-   0        0        0     6030 2023-03-22 08:48:33.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc
--rw-rw-rw-   0        0        0     5992 2023-04-14 12:53:50.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1702 2023-03-22 08:30:27.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc
--rw-rw-rw-   0        0        0     1690 2023-04-14 09:52:09.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc
--rw-rw-rw-   0        0        0     5903 2023-03-21 09:02:18.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc
--rw-rw-rw-   0        0        0     3297 2023-03-22 08:21:12.000000 nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc
--rw-rw-rw-   0        0        0     9589 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/gui.py
--rw-rw-rw-   0        0        0      698 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/main.py
--rw-rw-rw-   0        0        0     3962 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/measure_task.py
--rw-rw-rw-   0        0        0     7804 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/module.py
--rw-rw-rw-   0        0        0     1210 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/app/spm_template/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.343954 nanosurf-1.6.0/nanosurf/doc/
--rw-rw-rw-   0        0        0   797639 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/doc/Nanosurf Python Library Overview.pdf
--rw-rw-rw-   0        0        0     6199 2023-05-03 09:25:07.000000 nanosurf-1.6.0/nanosurf/doc/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.344955 nanosurf-1.6.0/nanosurf/lib/
--rw-rw-rw-   0        0        0        0 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.348955 nanosurf-1.6.0/nanosurf/lib/datatypes/
--rw-rw-rw-   0        0        0       52 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/__init__.py
--rw-rw-rw-   0        0        0     6982 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/prop_val.py
--rw-rw-rw-   0        0        0      856 2023-05-02 06:53:23.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_channel.py
--rw-rw-rw-   0        0        0     5185 2023-05-03 06:11:08.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_stream.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.350955 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/
--rw-rw-rw-   0        0        0     8641 2023-03-30 14:33:28.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/__init__.py
--rw-rw-rw-   0        0        0     9607 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/convert.py
--rw-rw-rw-   0        0        0     4102 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/unit_prefix.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.352954 nanosurf-1.6.0/nanosurf/lib/devices/
--rw-rw-rw-   0        0        0      192 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.352954 nanosurf-1.6.0/nanosurf/lib/devices/accessory_interface/
--rw-rw-rw-   0        0        0    13063 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/accessory_interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.359956 nanosurf-1.6.0/nanosurf/lib/devices/i2c/
--rw-rw-rw-   0        0        0      469 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/__init__.py
--rw-rw-rw-   0        0        0     7187 2022-11-08 07:40:33.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/bus_master.py
--rw-rw-rw-   0        0        0     2375 2022-11-08 07:40:33.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_24LC32A.py
--rw-rw-rw-   0        0        0     1123 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_PCA9534.py
--rw-rw-rw-   0        0        0     2830 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TCN75.py
--rw-rw-rw-   0        0        0    14497 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TMC5031.py
--rw-rw-rw-   0        0        0     3543 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TMP42x.py
--rw-rw-rw-   0        0        0     8324 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/devices/trinamic_motor_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.360955 nanosurf-1.6.0/nanosurf/lib/frameworks/
--rw-rw-rw-   0        0        0      225 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.365955 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/
--rw-rw-rw-   0        0        0      225 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/__init__.py
--rw-rw-rw-   0        0        0     6750 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/app_base.py
--rw-rw-rw-   0        0        0      195 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/app_common.py
--rw-rw-rw-   0        0        0     7474 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/app_gui.py
--rw-rw-rw-   0        0        0     2271 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/module_base.py
--rw-rw-rw-   0        0        0    13694 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/nsf_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.374954 nanosurf-1.6.0/nanosurf/lib/gui/
--rw-rw-rw-   0        0        0      781 2023-01-23 12:51:02.000000 nanosurf-1.6.0/nanosurf/lib/gui/__init__.py
--rw-rw-rw-   0        0        0     4528 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/gui/bind_gui.py
--rw-rw-rw-   0        0        0     1224 2023-02-02 07:32:08.000000 nanosurf-1.6.0/nanosurf/lib/gui/import_helper.py
--rw-rw-rw-   0        0        0      301 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_colors.py
--rw-rw-rw-   0        0        0     5545 2023-02-02 07:32:08.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_combobox.py
--rw-rw-rw-   0        0        0     5287 2023-02-02 07:32:08.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_edit.py
--rw-rw-rw-   0        0        0     1710 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_info_box.py
--rw-rw-rw-   0        0        0    16496 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_plots.py
--rw-rw-rw-   0        0        0    26594 2023-02-02 07:32:08.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_sci_edit.py
--rw-rw-rw-   0        0        0     6083 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_tables.py
--rw-rw-rw-   0        0        0      282 2022-12-14 14:12:12.000000 nanosurf-1.6.0/nanosurf/lib/gui/nsf_widgets_common.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.377955 nanosurf-1.6.0/nanosurf/lib/math/
--rw-rw-rw-   0        0        0       56 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/math/__init__.py
--rw-rw-rw-   0        0        0     5577 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/math/iir_filter.py
--rw-rw-rw-   0        0        0    19882 2023-05-03 06:11:08.000000 nanosurf-1.6.0/nanosurf/lib/math/sci_math.py
--rw-rw-rw-   0        0        0    12709 2023-05-03 06:11:08.000000 nanosurf-1.6.0/nanosurf/lib/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.379955 nanosurf-1.6.0/nanosurf/lib/spm/
--rw-rw-rw-   0        0        0      943 2023-02-24 14:35:46.000000 nanosurf-1.6.0/nanosurf/lib/spm/__init__.py
--rw-rw-rw-   0        0        0    17724 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/com_proxy.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.386956 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/
--rw-rw-rw-   0        0        0     4755 2023-03-10 16:14:57.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/__init__.py
--rw-rw-rw-   0        0        0      808 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/check.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.393955 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/
--rw-rw-rw-   0        0        0     1777 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py
--rw-rw-rw-   0        0        0     2342 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py
--rw-rw-rw-   0        0        0     6090 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py
--rw-rw-rw-   0        0        0     6502 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py
--rw-rw-rw-   0        0        0     1260 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py
--rw-rw-rw-   0        0        0     4528 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py
--rw-rw-rw-   0        0        0     6009 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py
--rw-rw-rw-   0        0        0     5016 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py
--rw-rw-rw-   0        0        0     7234 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/data_buffer.py
--rw-rw-rw-   0        0        0     5943 2023-05-03 08:56:03.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/data_buffer_interface.py
--rw-rw-rw-   0        0        0     3516 2023-04-12 16:19:57.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/iir_filter.py
--rw-rw-rw-   0        0        0    10920 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/logical_unit_interface.py
--rw-rw-rw-   0        0        0     6353 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py
--rw-rw-rw-   0        0        0     4227 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/manager_mock.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.397955 nanosurf-1.6.0/nanosurf/lib/spm/scanhead/
--rw-rw-rw-   0        0        0     1698 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/scanhead/__init__.py
--rw-rw-rw-   0        0        0     8222 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/spm/scanhead/drive_afm.py
--rw-rw-rw-   0        0        0    18954 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/spm/scanhead/motor_control.py
--rw-rw-rw-   0        0        0    12254 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/scanhead/studio_motor_control.py
--rw-rw-rw-   0        0        0     1634 2023-04-14 12:55:54.000000 nanosurf-1.6.0/nanosurf/lib/spm/spm_app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.398955 nanosurf-1.6.0/nanosurf/lib/spm/studio/
--rw-rw-rw-   0        0        0    22149 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/studio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.404954 nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/
--rw-rw-rw-   0        0        0    21945 2023-03-27 12:25:59.000000 nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/__init__.py
--rw-rw-rw-   0        0        0  2934958 2023-04-14 08:23:25.000000 nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py
--rw-rw-rw-   0        0        0  2796278 2023-04-14 08:23:25.000000 nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.408954 nanosurf-1.6.0/nanosurf/lib/spm/workflow/
--rw-rw-rw-   0        0        0      129 2022-12-20 08:45:27.000000 nanosurf-1.6.0/nanosurf/lib/spm/workflow/__init__.py
--rw-rw-rw-   0        0        0    56054 2023-05-03 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/spm/workflow/frequency_sweep.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.410956 nanosurf-1.6.0/nanosurf/lib/util/
--rw-rw-rw-   0        0        0      177 2022-11-08 07:07:44.000000 nanosurf-1.6.0/nanosurf/lib/util/__init__.py
--rw-rw-rw-   0        0        0     2140 2022-09-05 14:31:09.000000 nanosurf-1.6.0/nanosurf/lib/util/dataexport.py
--rw-rw-rw-   0        0        0     2561 2022-12-14 14:12:12.000000 nanosurf-1.6.0/nanosurf/lib/util/fileutil.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:26:08.231955 nanosurf-1.6.0/nanosurf.egg-info/
--rw-rw-rw-   0        0        0     6618 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11702 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 09:26:07.000000 nanosurf-1.6.0/nanosurf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       78 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 09:26:08.000000 nanosurf-1.6.0/nanosurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-09-05 14:31:09.000000 nanosurf-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 09:26:08.411955 nanosurf-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2055 2023-03-27 11:54:31.000000 nanosurf-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.501716 nanosurf-1.6.1/
+-rw-rw-rw-   0        0        0     1067 2022-02-08 08:13:22.000000 nanosurf-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     6686 2023-05-04 07:50:21.501716 nanosurf-1.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.313560 nanosurf-1.6.1/nanosurf/
+-rw-rw-rw-   0        0        0     1774 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-04 07:46:30.000000 nanosurf-1.6.1/nanosurf/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.303562 nanosurf-1.6.1/nanosurf/app/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/
+-rw-rw-rw-   0        0        0      566 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/
+-rw-rw-rw-   0        0        0     2294 2023-02-17 17:06:00.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2285 2023-04-14 11:38:45.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2364 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1853 2023-02-17 16:53:51.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1822 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1523 2023-02-17 17:00:32.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1361 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3319 2023-02-17 17:12:09.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3400 2023-05-03 07:22:11.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2670 2023-02-16 15:52:16.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2086 2023-05-03 07:19:15.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py
+-rw-rw-rw-   0        0        0     1843 2023-05-03 07:17:37.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py
+-rw-rw-rw-   0        0        0      740 2023-05-03 07:16:24.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py
+-rw-rw-rw-   0        0        0      893 2023-05-03 07:17:37.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py
+-rw-rw-rw-   0        0        0     4204 2023-05-03 07:20:07.000000 nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.334572 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1462 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.344581 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/
+-rw-rw-rw-   0        0        0      195 2022-12-14 07:35:47.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      193 2022-09-19 09:03:09.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9770 2023-03-09 15:52:53.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9831 2023-04-14 09:26:40.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5198 2023-03-09 15:52:53.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4006 2023-04-14 09:26:21.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5181 2023-02-03 08:34:04.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5236 2023-04-14 09:26:21.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1930 2022-12-14 07:35:47.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1768 2023-04-14 09:09:22.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13848 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py
+-rw-rw-rw-   0        0        0     4907 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py
+-rw-rw-rw-   0        0        0     5067 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py
+-rw-rw-rw-   0        0        0     1310 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.354580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/
+-rw-rw-rw-   0        0        0      194 2022-12-16 09:42:02.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      192 2022-09-16 14:32:05.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5443 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5291 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9703 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9667 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9829 2023-02-08 13:02:32.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9723 2023-04-14 12:06:14.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3005 2023-02-08 13:02:33.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2991 2023-04-14 12:01:18.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5067 2023-03-09 14:29:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3662 2023-04-14 12:04:20.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7030 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py
+-rw-rw-rw-   0        0        0    13971 2023-05-03 08:56:03.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py
+-rw-rw-rw-   0        0        0    10552 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py
+-rw-rw-rw-   0        0        0     2397 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py
+-rw-rw-rw-   0        0        0     3943 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py
+-rw-rw-rw-   0        0        0     1580 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.364580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1431 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.374582 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/
+-rw-rw-rw-   0        0        0      199 2022-12-16 13:29:49.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      197 2022-11-15 07:27:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9252 2023-02-16 16:05:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9276 2023-04-14 12:27:20.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6662 2023-02-16 16:05:23.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6564 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2314 2023-01-25 08:22:47.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2322 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4594 2023-03-13 14:19:52.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3455 2023-04-14 12:24:00.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13358 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py
+-rw-rw-rw-   0        0        0     7055 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py
+-rw-rw-rw-   0        0        0     4533 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/.vscode/
+-rw-rw-rw-   0        0        0      566 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/app/app_template/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.384580 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/
+-rw-rw-rw-   0        0        0        0 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/
+-rw-rw-rw-   0        0        0      176 2022-12-16 15:19:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      192 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      174 2022-09-19 08:10:48.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6384 2023-02-07 10:44:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0    13859 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6336 2023-04-14 08:47:57.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5392 2023-02-09 07:59:12.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9403 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5327 2023-04-14 08:43:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1797 2022-12-16 15:19:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2652 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1634 2023-04-14 08:43:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2896 2023-02-07 10:44:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5326 2023-01-25 09:01:50.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2570 2023-04-14 08:47:57.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7820 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/gui.py
+-rw-rw-rw-   0        0        0     5134 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/module.py
+-rw-rw-rw-   0        0        0     1160 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/settings.py
+-rw-rw-rw-   0        0        0     2617 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/demo_module/worker_task.py
+-rw-rw-rw-   0        0        0     1673 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/app_template/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/
+-rw-rw-rw-   0        0        0     4446 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb
+-rw-rw-rw-   0        0        0     2457 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/
+-rw-rw-rw-   0        0        0    54597 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.397103 nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/
+-rw-rw-rw-   0        0        0     7665 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/
+-rw-rw-rw-   0        0        0   121398 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb
+-rw-rw-rw-   0        0        0     2294 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/
+-rw-rw-rw-   0        0        0     4735 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py
+-rw-rw-rw-   0        0        0     1817 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/spm_template/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.407112 nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/
+-rw-rw-rw-   0        0        0      566 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/launch.json
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.417110 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/
+-rw-rw-rw-   0        0        0     7537 2023-03-22 08:49:37.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7506 2023-04-14 11:57:53.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3307 2023-03-22 08:30:27.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3320 2023-04-14 09:59:56.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6030 2023-03-22 08:48:33.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5992 2023-04-14 12:53:50.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1702 2023-03-22 08:30:27.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1690 2023-04-14 09:52:09.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5903 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3297 2023-03-22 08:21:12.000000 nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9589 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/gui.py
+-rw-rw-rw-   0        0        0      698 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/main.py
+-rw-rw-rw-   0        0        0     3962 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/measure_task.py
+-rw-rw-rw-   0        0        0     7804 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/module.py
+-rw-rw-rw-   0        0        0     1210 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/app/spm_template/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.417110 nanosurf-1.6.1/nanosurf/doc/
+-rw-rw-rw-   0        0        0   797639 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/doc/Nanosurf Python Library Overview.pdf
+-rw-rw-rw-   0        0        0     6267 2023-05-04 07:47:12.000000 nanosurf-1.6.1/nanosurf/doc/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/datatypes/
+-rw-rw-rw-   0        0        0       52 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/__init__.py
+-rw-rw-rw-   0        0        0     6982 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/prop_val.py
+-rw-rw-rw-   0        0        0      856 2023-05-02 06:53:23.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_channel.py
+-rw-rw-rw-   0        0        0     5185 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_stream.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/
+-rw-rw-rw-   0        0        0     8641 2023-03-30 14:33:28.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/__init__.py
+-rw-rw-rw-   0        0        0     9607 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/convert.py
+-rw-rw-rw-   0        0        0     4102 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/unit_prefix.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/devices/
+-rw-rw-rw-   0        0        0      192 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.427110 nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/
+-rw-rw-rw-   0        0        0    13063 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.437112 nanosurf-1.6.1/nanosurf/lib/devices/i2c/
+-rw-rw-rw-   0        0        0      469 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/__init__.py
+-rw-rw-rw-   0        0        0     7187 2022-11-08 07:40:33.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/bus_master.py
+-rw-rw-rw-   0        0        0     2375 2022-11-08 07:40:33.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_24LC32A.py
+-rw-rw-rw-   0        0        0     1123 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_PCA9534.py
+-rw-rw-rw-   0        0        0     2830 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TCN75.py
+-rw-rw-rw-   0        0        0    14497 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMC5031.py
+-rw-rw-rw-   0        0        0     3543 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMP42x.py
+-rw-rw-rw-   0        0        0     8324 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/devices/trinamic_motor_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.437112 nanosurf-1.6.1/nanosurf/lib/frameworks/
+-rw-rw-rw-   0        0        0      225 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.447111 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/
+-rw-rw-rw-   0        0        0      225 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.457113 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/
+-rw-rw-rw-   0        0        0      405 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      443 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7123 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7469 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc
+-rw-rw-rw-   0        0        0      509 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-310.pyc
+-rw-rw-rw-   0        0        0      505 2023-03-27 12:29:07.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7873 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7979 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3149 2023-03-21 09:02:18.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3341 2023-04-17 12:02:23.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12941 2023-03-23 07:32:45.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12980 2023-03-27 12:29:07.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6750 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_base.py
+-rw-rw-rw-   0        0        0      195 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_common.py
+-rw-rw-rw-   0        0        0     7474 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_gui.py
+-rw-rw-rw-   0        0        0   166135 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_icon.ico
+-rw-rw-rw-   0        0        0     6279 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_stylesheet.qss
+-rw-rw-rw-   0        0        0     2271 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/module_base.py
+-rw-rw-rw-   0        0        0    13694 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/nsf_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.459619 nanosurf-1.6.1/nanosurf/lib/gui/
+-rw-rw-rw-   0        0        0      781 2023-01-23 12:51:02.000000 nanosurf-1.6.1/nanosurf/lib/gui/__init__.py
+-rw-rw-rw-   0        0        0     4528 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/bind_gui.py
+-rw-rw-rw-   0        0        0     1224 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/import_helper.py
+-rw-rw-rw-   0        0        0      301 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_colors.py
+-rw-rw-rw-   0        0        0     5545 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_combobox.py
+-rw-rw-rw-   0        0        0     5287 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_edit.py
+-rw-rw-rw-   0        0        0     1710 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_info_box.py
+-rw-rw-rw-   0        0        0    16496 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_plots.py
+-rw-rw-rw-   0        0        0    26594 2023-02-02 07:32:08.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_sci_edit.py
+-rw-rw-rw-   0        0        0     6083 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_tables.py
+-rw-rw-rw-   0        0        0      282 2022-12-14 14:12:12.000000 nanosurf-1.6.1/nanosurf/lib/gui/nsf_widgets_common.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/math/
+-rw-rw-rw-   0        0        0       56 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/math/__init__.py
+-rw-rw-rw-   0        0        0     5577 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/math/iir_filter.py
+-rw-rw-rw-   0        0        0    19882 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/math/sci_math.py
+-rw-rw-rw-   0        0        0    12709 2023-05-03 06:11:08.000000 nanosurf-1.6.1/nanosurf/lib/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/spm/
+-rw-rw-rw-   0        0        0      943 2023-02-24 14:35:46.000000 nanosurf-1.6.1/nanosurf/lib/spm/__init__.py
+-rw-rw-rw-   0        0        0    17724 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/com_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.469626 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/
+-rw-rw-rw-   0        0        0     4755 2023-03-10 16:14:57.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/__init__.py
+-rw-rw-rw-   0        0        0      808 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/check.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/
+-rw-rw-rw-   0        0        0     1777 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py
+-rw-rw-rw-   0        0        0     2342 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py
+-rw-rw-rw-   0        0        0     6090 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py
+-rw-rw-rw-   0        0        0     6502 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py
+-rw-rw-rw-   0        0        0     1260 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py
+-rw-rw-rw-   0        0        0     4528 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py
+-rw-rw-rw-   0        0        0     6009 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py
+-rw-rw-rw-   0        0        0     5016 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py
+-rw-rw-rw-   0        0        0     7234 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer.py
+-rw-rw-rw-   0        0        0     5943 2023-05-03 08:56:03.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer_interface.py
+-rw-rw-rw-   0        0        0     3516 2023-04-12 16:19:57.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/iir_filter.py
+-rw-rw-rw-   0        0        0    10920 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface.py
+-rw-rw-rw-   0        0        0     6353 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py
+-rw-rw-rw-   0        0        0     4227 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/manager_mock.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/
+-rw-rw-rw-   0        0        0     1698 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/__init__.py
+-rw-rw-rw-   0        0        0     8222 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/drive_afm.py
+-rw-rw-rw-   0        0        0    18954 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/motor_control.py
+-rw-rw-rw-   0        0        0    12254 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/scanhead/studio_motor_control.py
+-rw-rw-rw-   0        0        0     1634 2023-04-14 12:55:54.000000 nanosurf-1.6.1/nanosurf/lib/spm/spm_app.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.479626 nanosurf-1.6.1/nanosurf/lib/spm/studio/
+-rw-rw-rw-   0        0        0    22149 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.489626 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/
+-rw-rw-rw-   0        0        0    21945 2023-03-27 12:25:59.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/__init__.py
+-rw-rw-rw-   0        0        0  2934958 2023-04-14 08:23:25.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py
+-rw-rw-rw-   0        0        0  2796278 2023-04-14 08:23:25.000000 nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.489626 nanosurf-1.6.1/nanosurf/lib/spm/workflow/
+-rw-rw-rw-   0        0        0      129 2022-12-20 08:45:27.000000 nanosurf-1.6.1/nanosurf/lib/spm/workflow/__init__.py
+-rw-rw-rw-   0        0        0    56054 2023-05-03 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/spm/workflow/frequency_sweep.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.499627 nanosurf-1.6.1/nanosurf/lib/util/
+-rw-rw-rw-   0        0        0      177 2022-11-08 07:07:44.000000 nanosurf-1.6.1/nanosurf/lib/util/__init__.py
+-rw-rw-rw-   0        0        0     2140 2022-09-05 14:31:09.000000 nanosurf-1.6.1/nanosurf/lib/util/dataexport.py
+-rw-rw-rw-   0        0        0     2561 2022-12-14 14:12:12.000000 nanosurf-1.6.1/nanosurf/lib/util/fileutil.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:50:21.323562 nanosurf-1.6.1/nanosurf.egg-info/
+-rw-rw-rw-   0        0        0     6686 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12618 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:50:20.000000 nanosurf-1.6.1/nanosurf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       78 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 07:50:21.000000 nanosurf-1.6.1/nanosurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-09-05 14:31:09.000000 nanosurf-1.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:50:21.501716 nanosurf-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-05-04 07:42:37.000000 nanosurf-1.6.1/setup.py
```

### Comparing `nanosurf-1.6.0/LICENSE` & `nanosurf-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/PKG-INFO` & `nanosurf-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosurf
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python API for Nanosurf controllers
 Author: Nanosurf AG
 Author-email: scripting@nanosurf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -145,14 +145,17 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.1
+  * Bugfix: pip packaging did not copy framework files
+
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
   * New: demo_lateral_force_signal_calibration. This demo shows how to calibrate the lateral force signal
   * New: nanosurf.plot. A package to easily plot data array from lists, numpy array, SciChannel and SciStream
   * New: nanosurf.spm.lowlevel.DataSamplerAccess. A class to make data sampling easier for CX/Studio
```

### Comparing `nanosurf-1.6.0/nanosurf/__init__.py` & `nanosurf-1.6.1/nanosurf/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_stm_addon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/device_tip_current_addon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/device_tip_current_addon.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py` & `nanosurf-1.6.1/nanosurf/app/app_DriveAFM_Tip_Current_Addon/worker.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/main.py` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/imaging_task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/imaging_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py` & `nanosurf-1.6.1/nanosurf/app/app_demo_scanning_and_lib_usage/scan_module/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_fit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/__pycache__/sweep_task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_fit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/frequency_sweep_module/sweep_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_frequency_sweep/main.py` & `nanosurf-1.6.1/nanosurf/app/app_frequency_sweep/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/main.py` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/__pycache__/worker_task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py` & `nanosurf-1.6.1/nanosurf/app/app_switching_spectrocopy/switching_spec_module/worker_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/app_template/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/__pycache__/worker_task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/gui.py` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/module.py` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/settings.py` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/demo_module/worker_task.py` & `nanosurf-1.6.1/nanosurf/app/app_template/demo_module/worker_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/app_template/main.py` & `nanosurf-1.6.1/nanosurf/app/app_template/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb` & `nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py` & `nanosurf-1.6.1/nanosurf/app/demo_creating_spec_pos_table_with_smiley/spectroscopy_demo_creating_a_smiley.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb` & `nanosurf-1.6.1/nanosurf/app/demo_lateral_force_signal_calibration/demo_lfm_calibration.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py` & `nanosurf-1.6.1/nanosurf/app/demo_move_sample_stage/demo_move_sample_stage.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb` & `nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.ipynb`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py` & `nanosurf-1.6.1/nanosurf/app/demo_spec_setup_and_data_plotting/spec_demo.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py` & `nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_demo_data_sampling.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py` & `nanosurf-1.6.1/nanosurf/app/demo_studio_scripting/studio_scripting_demo.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/.vscode/launch.json` & `nanosurf-1.6.1/nanosurf/app/spm_template/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/measure_task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc` & `nanosurf-1.6.1/nanosurf/app/spm_template/__pycache__/worker_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/gui.py` & `nanosurf-1.6.1/nanosurf/app/spm_template/gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/main.py` & `nanosurf-1.6.1/nanosurf/app/spm_template/main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/measure_task.py` & `nanosurf-1.6.1/nanosurf/app/spm_template/measure_task.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/module.py` & `nanosurf-1.6.1/nanosurf/app/spm_template/module.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/app/spm_template/settings.py` & `nanosurf-1.6.1/nanosurf/app/spm_template/settings.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/doc/Nanosurf Python Library Overview.pdf` & `nanosurf-1.6.1/nanosurf/doc/Nanosurf Python Library Overview.pdf`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/doc/README.md` & `nanosurf-1.6.1/nanosurf/doc/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,17 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.1
+  * Bugfix: pip packaging did not copy framework files
+
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
   * New: demo_lateral_force_signal_calibration. This demo shows how to calibrate the lateral force signal
   * New: nanosurf.plot. A package to easily plot data array from lists, numpy array, SciChannel and SciStream
   * New: nanosurf.spm.lowlevel.DataSamplerAccess. A class to make data sampling easier for CX/Studio
```

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/prop_val.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/prop_val.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/sci_channel.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_channel.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/sci_stream.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_stream.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/convert.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/convert.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/datatypes/sci_val/unit_prefix.py` & `nanosurf-1.6.1/nanosurf/lib/datatypes/sci_val/unit_prefix.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/accessory_interface/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/devices/accessory_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/bus_master.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/bus_master.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_24LC32A.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_24LC32A.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_PCA9534.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_PCA9534.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TCN75.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TCN75.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TMC5031.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMC5031.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/i2c/chip_TMP42x.py` & `nanosurf-1.6.1/nanosurf/lib/devices/i2c/chip_TMP42x.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/devices/trinamic_motor_controller.py` & `nanosurf-1.6.1/nanosurf/lib/devices/trinamic_motor_controller.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/app_base.py` & `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_base.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/app_gui.py` & `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/app_gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/module_base.py` & `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/module_base.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/frameworks/qt_app/nsf_thread.py` & `nanosurf-1.6.1/nanosurf/lib/frameworks/qt_app/nsf_thread.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/bind_gui.py` & `nanosurf-1.6.1/nanosurf/lib/gui/bind_gui.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/import_helper.py` & `nanosurf-1.6.1/nanosurf/lib/gui/import_helper.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_combobox.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_combobox.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_edit.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_edit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_info_box.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_info_box.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_plots.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_plots.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_sci_edit.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_sci_edit.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/gui/nsf_tables.py` & `nanosurf-1.6.1/nanosurf/lib/gui/nsf_tables.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/math/iir_filter.py` & `nanosurf-1.6.1/nanosurf/lib/math/iir_filter.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/math/sci_math.py` & `nanosurf-1.6.1/nanosurf/lib/math/sci_math.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/plot.py` & `nanosurf-1.6.1/nanosurf/lib/plot.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/com_proxy.py` & `nanosurf-1.6.1/nanosurf/lib/spm/com_proxy.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/check.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/check.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/adc.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/analyzer.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/capture.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/channelmux.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/dac.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/factory.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/ctrlunits/sampler.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/data_buffer.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/data_buffer_interface.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/data_buffer_interface.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/iir_filter.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/iir_filter.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/logical_unit_interface.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/logical_unit_interface_parser.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/lowlevel/manager_mock.py` & `nanosurf-1.6.1/nanosurf/lib/spm/lowlevel/manager_mock.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/scanhead/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/scanhead/drive_afm.py` & `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/drive_afm.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/scanhead/motor_control.py` & `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/motor_control.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/scanhead/studio_motor_control.py` & `nanosurf-1.6.1/nanosurf/lib/spm/scanhead/studio_motor_control.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/spm_app.py` & `nanosurf-1.6.1/nanosurf/lib/spm/spm_app.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/studio/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/__init__.py` & `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py` & `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_main.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py` & `nanosurf-1.6.1/nanosurf/lib/spm/studio/wrapper/cmd_tree_spm.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/spm/workflow/frequency_sweep.py` & `nanosurf-1.6.1/nanosurf/lib/spm/workflow/frequency_sweep.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/util/dataexport.py` & `nanosurf-1.6.1/nanosurf/lib/util/dataexport.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf/lib/util/fileutil.py` & `nanosurf-1.6.1/nanosurf/lib/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `nanosurf-1.6.0/nanosurf.egg-info/PKG-INFO` & `nanosurf-1.6.1/nanosurf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanosurf
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python API for Nanosurf controllers
 Author: Nanosurf AG
 Author-email: scripting@nanosurf.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -145,14 +145,17 @@
 
 Full list of objects and methods can be found in the Scripting Manual
 in Nanosurf controller software under Help tab:
 Help -> Manuals -> Script Programmers Manual, or [here](https://www.nanosurf.com/downloads/programmers-manual.pdf).
 
 ## Library Version History
 
+* v1.6.1
+  * Bugfix: pip packaging did not copy framework files
+
 * v1.6.0
   * New: spm_template: A new template to demonstrate simple connection to CX/Studio and measure some data
   * New: app_DriveAFM_Tip_Current_Addon this app controls the amplifier of the Tip-Current Addon
   * New: demo_move_sample_stage. This demo shows basic stage movements
   * New: demo_lateral_force_signal_calibration. This demo shows how to calibrate the lateral force signal
   * New: nanosurf.plot. A package to easily plot data array from lists, numpy array, SciChannel and SciStream
   * New: nanosurf.spm.lowlevel.DataSamplerAccess. A class to make data sampling easier for CX/Studio
```

### Comparing `nanosurf-1.6.0/nanosurf.egg-info/SOURCES.txt` & `nanosurf-1.6.1/nanosurf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -148,16 +148,30 @@
 nanosurf/lib/devices/i2c/chip_TMC5031.py
 nanosurf/lib/devices/i2c/chip_TMP42x.py
 nanosurf/lib/frameworks/__init__.py
 nanosurf/lib/frameworks/qt_app/__init__.py
 nanosurf/lib/frameworks/qt_app/app_base.py
 nanosurf/lib/frameworks/qt_app/app_common.py
 nanosurf/lib/frameworks/qt_app/app_gui.py
+nanosurf/lib/frameworks/qt_app/app_icon.ico
+nanosurf/lib/frameworks/qt_app/app_stylesheet.qss
 nanosurf/lib/frameworks/qt_app/module_base.py
 nanosurf/lib/frameworks/qt_app/nsf_thread.py
+nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/__init__.cpython-39.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_base.cpython-39.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_common.cpython-39.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/app_gui.cpython-39.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/module_base.cpython-39.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-310.pyc
+nanosurf/lib/frameworks/qt_app/__pycache__/nsf_thread.cpython-39.pyc
 nanosurf/lib/gui/__init__.py
 nanosurf/lib/gui/bind_gui.py
 nanosurf/lib/gui/import_helper.py
 nanosurf/lib/gui/nsf_colors.py
 nanosurf/lib/gui/nsf_combobox.py
 nanosurf/lib/gui/nsf_edit.py
 nanosurf/lib/gui/nsf_info_box.py
```

### Comparing `nanosurf-1.6.0/setup.py` & `nanosurf-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     return paths
 
 package_data_files = []
 package_data_files += package_files('nanosurf/app')
 package_data_files += package_files('nanosurf/doc')
 package_data_files += package_files('nanosurf_internal/app')
 package_data_files += package_files('nanosurf_internal/doc')
+package_data_files += package_files('nanosurf/lib/frameworks/qt_app')
 
 long_description_file = load_doc_file('nanosurf/doc/README.md')
 
 setup(
     name='nanosurf',
     version=load_version('nanosurf/_version.py'),
     author='Nanosurf AG',
```

