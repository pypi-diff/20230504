# Comparing `tmp/Rare-1.9.4.tar.gz` & `tmp/Rare-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rare-1.9.4.tar", last modified: Thu Dec  8 20:37:38 2022, max compression
+gzip compressed data, was "Rare-1.9.5.tar", last modified: Sun Jan 22 20:27:47 2023, max compression
```

## Comparing `Rare-1.9.4.tar` & `Rare-1.9.5.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.106340 Rare-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-08 20:37:27.000000 Rare-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-08 20:37:27.000000 Rare-1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2022-12-08 20:37:38.106340 Rare-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2022-12-08 20:37:27.000000 Rare-1.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.058342 Rare-1.9.4/Rare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-08 20:37:37.000000 Rare-1.9.4/Rare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2022-12-08 20:37:27.000000 Rare-1.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19122 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/install_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/launch_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/dialogs/login/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/login/browser_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/login/import_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/path_input_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/dialogs/uninstall_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/tabs/account/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/tabs/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/downloads/dl_queue_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/downloads/download_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.062341 Rare-1.9.4/rare/components/tabs/games/
--rw-r--r--   0 runner    (1001) docker     (123)    21029 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/cloud_save_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.066341 Rare-1.9.4/rare/components/tabs/games/game_info/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/game_dlc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16073 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/game_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/game_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/move_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_info/uninstalled_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.066341 Rare-1.9.4/rare/components/tabs/games/game_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/base_installed_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/base_uninstalled_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/installed_icon_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/installed_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/installing_game_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/library_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/uninstalled_icon_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/game_widgets/uninstalled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/head_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.070341 Rare-1.9.4/rare/components/tabs/games/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/integrations/egl_sync_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/integrations/eos_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/integrations/import_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/games/integrations/ubisoft_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.070341 Rare-1.9.4/rare/components/tabs/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/about.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/default_game_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/legendary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/rare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.074341 Rare-1.9.4/rare/components/tabs/settings/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/dxvk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/mangohud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/overlay_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/pre_launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/proton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/settings/widgets/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.074341 Rare-1.9.4/rare/components/tabs/shop/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/game_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/game_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/search_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/shop_api_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/shop_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/shop_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/shop/wishlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tabs/tab_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/components/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/game_launch_helper/
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/game_launch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/game_launch_helper/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/game_launch_helper/lgd_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/game_launch_helper/message_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/lgndr/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31922 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/lgndr/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/lgndr/downloader/mp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/downloader/mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/downloader/mp/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/lgndr/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/glue/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/glue/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/glue/monkeys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/lgndr/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/lgndr/models/downloading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/models/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/models/apiresults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/models/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/models/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.078341 Rare-1.9.4/rare/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.086341 Rare-1.9.4/rare/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   448256 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/Rare.icns
--rw-r--r--   0 runner    (1001) docker     (123)    66369 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/Rare.ico
--rw-r--r--   0 runner    (1001) docker     (123)   235555 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/Rare.png
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/Rare.svg
--rw-r--r--   0 runner    (1001) docker     (123)   211364 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/Rare_nonsquared.png
--rw-r--r--   0 runner    (1001) docker     (123)   314684 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/cover.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/images/loader.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/resources/languages/
--rw-r--r--   0 runner    (1001) docker     (123)    43582 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/ca.qm
--rw-r--r--   0 runner    (1001) docker     (123)   126107 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/ca.ts
--rw-r--r--   0 runner    (1001) docker     (123)    52079 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/de.qm
--rw-r--r--   0 runner    (1001) docker     (123)   126428 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)   118406 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)    42139 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/pt_BR.qm
--rw-r--r--   0 runner    (1001) docker     (123)   124861 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/pt_BR.ts
--rw-r--r--   0 runner    (1001) docker     (123)   220467 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/qt_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/qt_pt_BR.qm
--rw-r--r--   0 runner    (1001) docker     (123)    42252 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/ru.qm
--rw-r--r--   0 runner    (1001) docker     (123)   131093 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/ru.ts
--rw-r--r--   0 runner    (1001) docker     (123)    44190 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/tr.qm
--rw-r--r--   0 runner    (1001) docker     (123)   125780 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/tr.ts
--rw-r--r--   0 runner    (1001) docker     (123)   129286 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/translation_source.ts
--rw-r--r--   0 runner    (1001) docker     (123)    56577 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/uk.qm
--rw-r--r--   0 runner    (1001) docker     (123)   136295 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/uk.ts
--rw-r--r--   0 runner    (1001) docker     (123)    29603 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/zh-Hans.qm
--rw-r--r--   0 runner    (1001) docker     (123)   122527 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/zh-Hans.ts
--rw-r--r--   0 runner    (1001) docker     (123)    29635 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/zh_TW.qm
--rw-r--r--   0 runner    (1001) docker     (123)   122696 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/languages/zh_TW.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1004931 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/resources/stylesheets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/resources/stylesheets/ChildOfMetropolis/
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/stylesheets/ChildOfMetropolis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/resources/stylesheets/RareStyle/
--rw-r--r--   0 runner    (1001) docker     (123)    27029 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/stylesheets/RareStyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/resources/stylesheets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/shared/image_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/shared/rare_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.094341 Rare-1.9.4/rare/ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/install_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/install_dialog_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/launch_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/dialogs/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/login/browser_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/login/import_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/login/landing_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/login/login_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/dialogs/sync_save_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/extra/console_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/tabs/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/downloads/downloads_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/tabs/games/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/tabs/games/game_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/game_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_dlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_dlc_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.098341 Rare-1.9.4/rare/ui/components/tabs/games/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/integrations/egl_sync_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/integrations/egl_sync_list_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/integrations/eos_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/games/integrations/import_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.102341 Rare-1.9.4/rare/ui/components/tabs/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/legendary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/proton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/rare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.102341 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/dxvk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/settings/widgets/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.102341 Rare-1.9.4/rare/ui/components/tabs/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/browse_games.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/shop_game_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/wishlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/components/tabs/store/wishlist_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.102341 Rare-1.9.4/rare/ui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/ui/utils/pathedit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.106340 Rare-1.9.4/rare/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17693 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/extra_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/legendary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13502 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/qt_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/utils/steam_grades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:37:38.106340 Rare-1.9.4/rare/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/collapsible_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/elide_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/flow_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/library_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/rare_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2022-12-08 20:37:27.000000 Rare-1.9.4/rare/widgets/sliding_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 20:37:38.106340 Rare-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2022-12-08 20:37:27.000000 Rare-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.520541 Rare-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-22 20:27:36.000000 Rare-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-22 20:27:36.000000 Rare-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-01-22 20:27:47.520541 Rare-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-01-22 20:27:36.000000 Rare-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/Rare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-22 20:27:47.000000 Rare-1.9.5/Rare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-01-22 20:27:36.000000 Rare-1.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19122 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/install_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/launch_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/dialogs/login/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/login/browser_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/login/import_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/path_input_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/dialogs/uninstall_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/tabs/account/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/tabs/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/downloads/dl_queue_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/downloads/download_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/tabs/games/
+-rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/cloud_save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.496539 Rare-1.9.5/rare/components/tabs/games/game_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/game_dlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/game_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/move_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_info/uninstalled_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.500539 Rare-1.9.5/rare/components/tabs/games/game_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/base_installed_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/base_uninstalled_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/installed_icon_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/installed_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/installing_game_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/library_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/uninstalled_icon_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/game_widgets/uninstalled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/head_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.500539 Rare-1.9.5/rare/components/tabs/games/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/integrations/egl_sync_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/integrations/eos_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/integrations/import_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/games/integrations/ubisoft_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.500539 Rare-1.9.5/rare/components/tabs/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/default_game_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/legendary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/rare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.500539 Rare-1.9.5/rare/components/tabs/settings/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/dxvk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/mangohud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/overlay_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/pre_launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/proton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/settings/widgets/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.500539 Rare-1.9.5/rare/components/tabs/shop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/game_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/shop_api_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/shop_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/shop_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/shop/wishlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tabs/tab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/components/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/game_launch_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/game_launch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/game_launch_helper/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/game_launch_helper/lgd_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/game_launch_helper/message_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/lgndr/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/lgndr/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/lgndr/downloader/mp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/downloader/mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/downloader/mp/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/lgndr/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/glue/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/glue/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/glue/monkeys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/lgndr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/lgndr/models/downloading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/models/apiresults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/models/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/models/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.504539 Rare-1.9.5/rare/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.508540 Rare-1.9.5/rare/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   448256 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/Rare.icns
+-rw-r--r--   0 runner    (1001) docker     (123)    66369 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/Rare.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   235555 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/Rare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/Rare.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   211364 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/Rare_nonsquared.png
+-rw-r--r--   0 runner    (1001) docker     (123)   314684 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/cover.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/images/loader.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/resources/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)    43582 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/ca.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   126107 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/ca.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52079 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   126428 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   118406 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    42139 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/pt_BR.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   124861 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/pt_BR.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   220467 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/qt_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/qt_pt_BR.qm
+-rw-r--r--   0 runner    (1001) docker     (123)    42252 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/ru.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   131093 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/ru.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    44190 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/tr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   125780 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/tr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   129286 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/translation_source.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    56577 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/uk.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   136295 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/uk.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    29603 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/zh-Hans.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   122527 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/zh-Hans.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    29635 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/zh_TW.qm
+-rw-r--r--   0 runner    (1001) docker     (123)   122696 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/languages/zh_TW.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1004931 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/resources/stylesheets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/resources/stylesheets/ChildOfMetropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/stylesheets/ChildOfMetropolis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/resources/stylesheets/RareStyle/
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/stylesheets/RareStyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/resources/stylesheets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/shared/image_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/shared/rare_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/install_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/install_dialog_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/launch_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/dialogs/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/login/browser_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/login/import_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/login/landing_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/login/login_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/dialogs/sync_save_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/extra/console_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/tabs/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/downloads/downloads_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.512540 Rare-1.9.5/rare/ui/components/tabs/games/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/components/tabs/games/game_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/game_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_dlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_dlc_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/components/tabs/games/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/integrations/egl_sync_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/integrations/egl_sync_list_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/integrations/eos_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/games/integrations/import_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/components/tabs/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/legendary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/proton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/rare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/dxvk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/settings/widgets/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/components/tabs/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/browse_games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/shop_game_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/wishlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/components/tabs/store/wishlist_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.516540 Rare-1.9.5/rare/ui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/ui/utils/pathedit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.520541 Rare-1.9.5/rare/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17693 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/extra_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/legendary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/qt_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/utils/steam_grades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 20:27:47.520541 Rare-1.9.5/rare/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/collapsible_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/elide_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/flow_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/library_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/rare_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-01-22 20:27:36.000000 Rare-1.9.5/rare/widgets/sliding_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 20:27:47.520541 Rare-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-01-22 20:27:36.000000 Rare-1.9.5/setup.py
```

### Comparing `Rare-1.9.4/LICENSE` & `Rare-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/PKG-INFO` & `Rare-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rare
-Version: 1.9.4
+Version: 1.9.5
 Summary: A gui for Legendary
 Home-page: https://github.com/Dummerle/Rare
 Author: Dummerle
 License: GPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -87,18 +87,20 @@
 **Note**: When you launch it, you will see an error, that the package is from an unknown source. You have to enable it
 manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper will block Rare from running.
 
 You can also use `pip`.
 
 ### Windows
 
-Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
+- There is a small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/RareUpdater), which installs and updates rare with a single click
+
+- Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
 You can install rare with the following one-liner:
 
-`choco install rare`
+    `choco install rare`
 
 ### Packages
 
 In [releases page](https://github.com/Dummerle/Rare/releases), AppImages are available for Linux, a .msi file for windows and a .dmg
 file for macOS.
 
 ### Latest packages
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Rare Version: 1.9.4 Summary: A gui for Legendary
+Metadata-Version: 2.1 Name: Rare Version: 1.9.5 Summary: A gui for Legendary
 Home-page: https://github.com/Dummerle/Rare Author: Dummerle License: GPL-
 3 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown Provides-Extra: webview Provides-Extra:
@@ -32,15 +32,17 @@
 package. You can install it from [DUR](https://mpr.hunterwittenborn.com/
 packages/python3-pypresence) or with pip. - Do not wonder if some icons look
 strange, because the official python3-qtawesome package is too old. Many icons
 were replaced. ### macOS There is a .dmg file available in [releases page]
 (https://github.com/Dummerle/Rare/releases). **Note**: When you launch it, you
 will see an error, that the package is from an unknown source. You have to
 enable it manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper
-will block Rare from running. You can also use `pip`. ### Windows Rare is
+will block Rare from running. You can also use `pip`. ### Windows - There is a
+small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/
+RareUpdater), which installs and updates rare with a single click - Rare is
 available as a [Chocolatey package](https://community.chocolatey.org/packages/
 rare) on Windows. You can install rare with the following one-liner: `choco
 install rare` ### Packages In [releases page](https://github.com/Dummerle/Rare/
 releases), AppImages are available for Linux, a .msi file for windows and a
 .dmg file for macOS. ### Latest packages In the [actions](https://github.com/
 Dummerle/Rare/actions) tab you can find packages for the latest commits.
 **Note**: They might be unstable. ### Installation via pip (platform
```

### Comparing `Rare-1.9.4/README.md` & `Rare-1.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,20 @@
 **Note**: When you launch it, you will see an error, that the package is from an unknown source. You have to enable it
 manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper will block Rare from running.
 
 You can also use `pip`.
 
 ### Windows
 
-Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
+- There is a small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/RareUpdater), which installs and updates rare with a single click
+
+- Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
 You can install rare with the following one-liner:
 
-`choco install rare`
+    `choco install rare`
 
 ### Packages
 
 In [releases page](https://github.com/Dummerle/Rare/releases), AppImages are available for Linux, a .msi file for windows and a .dmg
 file for macOS.
 
 ### Latest packages
```

#### html2text {}

```diff
@@ -24,15 +24,17 @@
 package. You can install it from [DUR](https://mpr.hunterwittenborn.com/
 packages/python3-pypresence) or with pip. - Do not wonder if some icons look
 strange, because the official python3-qtawesome package is too old. Many icons
 were replaced. ### macOS There is a .dmg file available in [releases page]
 (https://github.com/Dummerle/Rare/releases). **Note**: When you launch it, you
 will see an error, that the package is from an unknown source. You have to
 enable it manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper
-will block Rare from running. You can also use `pip`. ### Windows Rare is
+will block Rare from running. You can also use `pip`. ### Windows - There is a
+small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/
+RareUpdater), which installs and updates rare with a single click - Rare is
 available as a [Chocolatey package](https://community.chocolatey.org/packages/
 rare) on Windows. You can install rare with the following one-liner: `choco
 install rare` ### Packages In [releases page](https://github.com/Dummerle/Rare/
 releases), AppImages are available for Linux, a .msi file for windows and a
 .dmg file for macOS. ### Latest packages In the [actions](https://github.com/
 Dummerle/Rare/actions) tab you can find packages for the latest commits.
 **Note**: They might be unstable. ### Installation via pip (platform
```

### Comparing `Rare-1.9.4/Rare.egg-info/PKG-INFO` & `Rare-1.9.5/Rare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rare
-Version: 1.9.4
+Version: 1.9.5
 Summary: A gui for Legendary
 Home-page: https://github.com/Dummerle/Rare
 Author: Dummerle
 License: GPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -87,18 +87,20 @@
 **Note**: When you launch it, you will see an error, that the package is from an unknown source. You have to enable it
 manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper will block Rare from running.
 
 You can also use `pip`.
 
 ### Windows
 
-Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
+- There is a small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/RareUpdater), which installs and updates rare with a single click
+
+- Rare is available as a [Chocolatey package](https://community.chocolatey.org/packages/rare) on Windows.
 You can install rare with the following one-liner:
 
-`choco install rare`
+    `choco install rare`
 
 ### Packages
 
 In [releases page](https://github.com/Dummerle/Rare/releases), AppImages are available for Linux, a .msi file for windows and a .dmg
 file for macOS.
 
 ### Latest packages
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Rare Version: 1.9.4 Summary: A gui for Legendary
+Metadata-Version: 2.1 Name: Rare Version: 1.9.5 Summary: A gui for Legendary
 Home-page: https://github.com/Dummerle/Rare Author: Dummerle License: GPL-
 3 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown Provides-Extra: webview Provides-Extra:
@@ -32,15 +32,17 @@
 package. You can install it from [DUR](https://mpr.hunterwittenborn.com/
 packages/python3-pypresence) or with pip. - Do not wonder if some icons look
 strange, because the official python3-qtawesome package is too old. Many icons
 were replaced. ### macOS There is a .dmg file available in [releases page]
 (https://github.com/Dummerle/Rare/releases). **Note**: When you launch it, you
 will see an error, that the package is from an unknown source. You have to
 enable it manually in `Settings -> Security and Privacy`. Otherwise, Gatekeeper
-will block Rare from running. You can also use `pip`. ### Windows Rare is
+will block Rare from running. You can also use `pip`. ### Windows - There is a
+small beta tool for Windows: [Rare Updater](https://github.com/Dummerle/
+RareUpdater), which installs and updates rare with a single click - Rare is
 available as a [Chocolatey package](https://community.chocolatey.org/packages/
 rare) on Windows. You can install rare with the following one-liner: `choco
 install rare` ### Packages In [releases page](https://github.com/Dummerle/Rare/
 releases), AppImages are available for Linux, a .msi file for windows and a
 .dmg file for macOS. ### Latest packages In the [actions](https://github.com/
 Dummerle/Rare/actions) tab you can find packages for the latest commits.
 **Note**: They might be unstable. ### Installation via pip (platform
```

### Comparing `Rare-1.9.4/Rare.egg-info/SOURCES.txt` & `Rare-1.9.5/Rare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/pyproject.toml` & `Rare-1.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     | rare/legendary
     | rare/resources
 )/
 '''
 
 [tool.poetry]
 name = "rare"
-version = "1.9.4"
+version = "1.9.5"
 description = "A GUI for Legendary"
 authors = ["Dummerle"]
 license = "GPL3"
 readme = "README.md"
 repository = "https://github.com/Dummerle/Rare"
 
 [tool.poetry.dependencies]
@@ -26,15 +26,15 @@
 QtAwesome = "^1.1.1"
 pypresence = { version = "^4.2.1", optional = true }
 pywin32 = { version = "^304", markers = "platform_system == 'Windows'" }
 pywebview = [
     { version = "^3.6.3", extras = ["cef"], platform = "windows", optional = true },
     { version = "^3.6.3", extras = ["gtk"], platform = "linux", optional = true },
 ]
-legendary-gl = "^0.20.31"
+legendary-gl = "^0.20.32"
 typing-extensions = "^4.3.0"
 
 [tool.poetry.scripts]
 start = "rare.__main__:main"
 
 [tool.poetry.dev-dependencies]
 Nuitka = "^1.0.6"
```

### Comparing `Rare-1.9.4/rare/__main__.py` & `Rare-1.9.5/rare/__main__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/app.py` & `Rare-1.9.5/rare/app.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/install_dialog.py` & `Rare-1.9.5/rare/components/dialogs/install_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/launch_dialog.py` & `Rare-1.9.5/rare/components/dialogs/launch_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/login/__init__.py` & `Rare-1.9.5/rare/components/dialogs/login/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/login/browser_login.py` & `Rare-1.9.5/rare/components/dialogs/login/browser_login.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/login/import_login.py` & `Rare-1.9.5/rare/components/dialogs/login/import_login.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/path_input_dialog.py` & `Rare-1.9.5/rare/components/dialogs/path_input_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/dialogs/uninstall_dialog.py` & `Rare-1.9.5/rare/components/dialogs/uninstall_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/main_window.py` & `Rare-1.9.5/rare/components/main_window.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/__init__.py` & `Rare-1.9.5/rare/components/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/account/__init__.py` & `Rare-1.9.5/rare/components/tabs/account/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     logout: pyqtSignal = pyqtSignal()
 
     def __init__(self, parent):
         super(AccountWidget, self).__init__(parent=parent)
         self.core = LegendaryCoreSingleton()
         self.signals = GlobalSignalsSingleton()
 
-        username = self.core.lgd.userdata.get("display_name")
+        username = self.core.lgd.userdata.get("displayName")
         if not username:
             username = "Offline"
 
         self.open_browser = QPushButton(icon("fa.external-link"), self.tr("Account settings"))
         self.open_browser.clicked.connect(
             lambda: webbrowser.open(
                 "https://www.epicgames.com/account/personal?productName=epicgames"
```

### Comparing `Rare-1.9.4/rare/components/tabs/downloads/__init__.py` & `Rare-1.9.5/rare/components/tabs/downloads/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/downloads/dl_queue_widget.py` & `Rare-1.9.5/rare/components/tabs/downloads/dl_queue_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/downloads/download_thread.py` & `Rare-1.9.5/rare/components/tabs/downloads/download_thread.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/__init__.py` & `Rare-1.9.5/rare/components/tabs/games/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/cloud_save_utils.py` & `Rare-1.9.5/rare/components/tabs/games/cloud_save_utils.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/__init__.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/game_dlc.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/game_dlc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/game_info.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/game_info.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/game_settings.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/game_settings.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/move_game.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/move_game.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_info/uninstalled_info.py` & `Rare-1.9.5/rare/components/tabs/games/game_info/uninstalled_info.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_utils.py` & `Rare-1.9.5/rare/components/tabs/games/game_utils.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/base_installed_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/base_installed_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/base_uninstalled_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/base_uninstalled_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/installed_icon_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/installed_icon_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/installed_list_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/installed_list_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/installing_game_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/installing_game_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/library_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/library_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/uninstalled_icon_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/uninstalled_icon_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/game_widgets/uninstalled_list_widget.py` & `Rare-1.9.5/rare/components/tabs/games/game_widgets/uninstalled_list_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/head_bar.py` & `Rare-1.9.5/rare/components/tabs/games/head_bar.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/integrations/__init__.py` & `Rare-1.9.5/rare/components/tabs/games/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/integrations/egl_sync_group.py` & `Rare-1.9.5/rare/components/tabs/games/integrations/egl_sync_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/integrations/eos_group.py` & `Rare-1.9.5/rare/components/tabs/games/integrations/eos_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/integrations/import_group.py` & `Rare-1.9.5/rare/components/tabs/games/integrations/import_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/games/integrations/ubisoft_group.py` & `Rare-1.9.5/rare/components/tabs/games/integrations/ubisoft_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/__init__.py` & `Rare-1.9.5/rare/components/tabs/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/about.py` & `Rare-1.9.5/rare/components/tabs/settings/about.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/debug.py` & `Rare-1.9.5/rare/components/tabs/settings/debug.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/default_game_settings.py` & `Rare-1.9.5/rare/components/tabs/settings/default_game_settings.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/legendary.py` & `Rare-1.9.5/rare/components/tabs/settings/legendary.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/rare.py` & `Rare-1.9.5/rare/components/tabs/settings/rare.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/dxvk.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/dxvk.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/env_vars.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/env_vars.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/linux.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/linux.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/mangohud.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/mangohud.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/overlay_settings.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/overlay_settings.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/pre_launch.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/pre_launch.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/proton.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/proton.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/rpc.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/rpc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/settings/widgets/wrapper.py` & `Rare-1.9.5/rare/components/tabs/settings/widgets/wrapper.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/__init__.py` & `Rare-1.9.5/rare/components/tabs/shop/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/constants.py` & `Rare-1.9.5/rare/components/tabs/shop/constants.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/game_info.py` & `Rare-1.9.5/rare/components/tabs/shop/game_info.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/game_widgets.py` & `Rare-1.9.5/rare/components/tabs/shop/game_widgets.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/search_results.py` & `Rare-1.9.5/rare/components/tabs/shop/search_results.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/shop_api_core.py` & `Rare-1.9.5/rare/components/tabs/shop/shop_api_core.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/shop_models.py` & `Rare-1.9.5/rare/components/tabs/shop/shop_models.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/shop_widget.py` & `Rare-1.9.5/rare/components/tabs/shop/shop_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/shop/wishlist.py` & `Rare-1.9.5/rare/components/tabs/shop/wishlist.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tabs/tab_utils.py` & `Rare-1.9.5/rare/components/tabs/tab_utils.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/components/tray_icon.py` & `Rare-1.9.5/rare/components/tray_icon.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/game_launch_helper/__init__.py` & `Rare-1.9.5/rare/game_launch_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
 import logging
+import platform
+import subprocess
 import sys
 import time
 import traceback
 from argparse import Namespace
 from logging import getLogger
 from typing import Union, Optional
 
@@ -16,14 +18,18 @@
 from rare.widgets.rare_app import RareApp
 from .console import Console
 from .lgd_helper import get_launch_args, InitArgs, get_configured_process, LaunchArgs, GameArgsError
 from .message_models import ErrorModel, Actions, FinishedModel, BaseModel, StateChangedModel
 
 logger = logging.getLogger("RareLauncher")
 
+DETACHED_APP_NAMES = [
+    "0a2d9f6403244d12969e11da6713137b"
+]
+
 
 class PreLaunchThread(QRunnable):
     class Signals(QObject):
         ready_to_launch = pyqtSignal(LaunchArgs)
         started_pre_launch_command = pyqtSignal()
         pre_launch_command_finished = pyqtSignal(int)  # exit_code
         error_occurred = pyqtSignal(str)
@@ -170,14 +176,22 @@
         # send start message after process started
         self.game_process.started.connect(lambda: self.send_message(
             StateChangedModel(
                 action=Actions.state_update, app_name=self.app_name,
                 new_state=StateChangedModel.States.started
             )
         ))
+        if self.app_name in DETACHED_APP_NAMES and platform.system() == "Windows":
+            self.game_process.deleteLater()
+            subprocess.Popen([args.executable] + args.args, cwd=args.cwd,
+                             env={i: args.env.value(i) for i in args.env.keys()})
+            if self.console:
+                self.console.log("Launching game detached")
+            self.stop()
+            return
         self.game_process.start(args.executable, args.args)
 
     def error_occurred(self, error_str: str):
         self.logger.warning(error_str)
         if self.console:
             self.console.on_process_exit(self.core.get_game(self.app_name).app_title, error_str)
         self.send_message(ErrorModel(
@@ -209,14 +223,16 @@
             self.server.close()
             self.server.deleteLater()
         except RuntimeError:
             pass
         self.processEvents()
         if not self.console:
             self.exit()
+        else:
+            self.console.on_process_exit(self.app_name, 0)
 
 
 def start_game(args: Namespace):
     args = InitArgs.from_argparse(args)
 
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
```

### Comparing `Rare-1.9.4/rare/game_launch_helper/console.py` & `Rare-1.9.5/rare/game_launch_helper/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         self.setReadOnly(True)
         font = QFont("Monospace")
         font.setStyleHint(QFont.Monospace)
         self.setFont(font)
         self._cursor_output = self.textCursor()
 
     def log(self, text):
-        html = f"<p style=\"color:#999;white-space:pre\">{text}</p>"
+        html = f"<p style=\"color:#BBB;white-space:pre\">{text}</p>"
         self._cursor_output.insertHtml(html)
         self.scroll_to_last_line()
 
     def error(self, text):
         html = f"<p style=\"color:#eee;white-space:pre\">{text}</p>"
         self._cursor_output.insertHtml(html)
         self.scroll_to_last_line()
```

### Comparing `Rare-1.9.4/rare/game_launch_helper/lgd_helper.py` & `Rare-1.9.5/rare/game_launch_helper/lgd_helper.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/game_launch_helper/message_models.py` & `Rare-1.9.5/rare/game_launch_helper/message_models.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/cli.py` & `Rare-1.9.5/rare/lgndr/cli.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/core.py` & `Rare-1.9.5/rare/lgndr/core.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/downloader/mp/manager.py` & `Rare-1.9.5/rare/lgndr/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/glue/arguments.py` & `Rare-1.9.5/rare/lgndr/glue/arguments.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/glue/exception.py` & `Rare-1.9.5/rare/lgndr/glue/exception.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/glue/monkeys.py` & `Rare-1.9.5/rare/lgndr/glue/monkeys.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/lgndr/models/downloading.py` & `Rare-1.9.5/rare/lgndr/models/downloading.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/models/apiresults.py` & `Rare-1.9.5/rare/models/apiresults.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/models/install.py` & `Rare-1.9.5/rare/models/install.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/models/signals.py` & `Rare-1.9.5/rare/models/signals.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/Rare.icns` & `Rare-1.9.5/rare/resources/images/Rare.icns`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/Rare.ico` & `Rare-1.9.5/rare/resources/images/Rare.ico`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/Rare.png` & `Rare-1.9.5/rare/resources/images/Rare.png`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/Rare.svg` & `Rare-1.9.5/rare/resources/images/Rare.svg`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/Rare_nonsquared.png` & `Rare-1.9.5/rare/resources/images/Rare_nonsquared.png`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/cover.png` & `Rare-1.9.5/rare/resources/images/cover.png`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/images/loader.gif` & `Rare-1.9.5/rare/resources/images/loader.gif`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/ca.qm` & `Rare-1.9.5/rare/resources/languages/ca.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/ca.ts` & `Rare-1.9.5/rare/resources/languages/ca.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/de.qm` & `Rare-1.9.5/rare/resources/languages/de.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/de.ts` & `Rare-1.9.5/rare/resources/languages/de.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/fr.qm` & `Rare-1.9.5/rare/resources/languages/fr.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/fr.ts` & `Rare-1.9.5/rare/resources/languages/fr.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/pt_BR.qm` & `Rare-1.9.5/rare/resources/languages/pt_BR.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/pt_BR.ts` & `Rare-1.9.5/rare/resources/languages/pt_BR.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/qt_de.qm` & `Rare-1.9.5/rare/resources/languages/qt_de.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/ru.qm` & `Rare-1.9.5/rare/resources/languages/ru.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/ru.ts` & `Rare-1.9.5/rare/resources/languages/ru.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/tr.qm` & `Rare-1.9.5/rare/resources/languages/tr.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/tr.ts` & `Rare-1.9.5/rare/resources/languages/tr.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/translation_source.ts` & `Rare-1.9.5/rare/resources/languages/translation_source.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/uk.qm` & `Rare-1.9.5/rare/resources/languages/uk.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/uk.ts` & `Rare-1.9.5/rare/resources/languages/uk.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/zh-Hans.qm` & `Rare-1.9.5/rare/resources/languages/zh-Hans.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/zh-Hans.ts` & `Rare-1.9.5/rare/resources/languages/zh-Hans.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/zh_TW.qm` & `Rare-1.9.5/rare/resources/languages/zh_TW.qm`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/languages/zh_TW.ts` & `Rare-1.9.5/rare/resources/languages/zh_TW.ts`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/resources.py` & `Rare-1.9.5/rare/resources/resources.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/stylesheets/ChildOfMetropolis/__init__.py` & `Rare-1.9.5/rare/resources/stylesheets/ChildOfMetropolis/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/resources/stylesheets/RareStyle/__init__.py` & `Rare-1.9.5/rare/resources/stylesheets/RareStyle/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/shared/__init__.py` & `Rare-1.9.5/rare/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/shared/image_manager.py` & `Rare-1.9.5/rare/shared/image_manager.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/shared/rare_core.py` & `Rare-1.9.5/rare/shared/rare_core.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/install_dialog.py` & `Rare-1.9.5/rare/ui/components/dialogs/install_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/install_dialog_advanced.py` & `Rare-1.9.5/rare/ui/components/dialogs/install_dialog_advanced.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/launch_dialog.py` & `Rare-1.9.5/rare/ui/components/dialogs/launch_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/login/browser_login.py` & `Rare-1.9.5/rare/ui/components/dialogs/login/browser_login.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/login/import_login.py` & `Rare-1.9.5/rare/ui/components/dialogs/login/import_login.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/login/landing_page.py` & `Rare-1.9.5/rare/ui/components/dialogs/login/landing_page.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/login/login_dialog.py` & `Rare-1.9.5/rare/ui/components/dialogs/login/login_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/dialogs/sync_save_dialog.py` & `Rare-1.9.5/rare/ui/components/dialogs/sync_save_dialog.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/extra/console_env.py` & `Rare-1.9.5/rare/ui/components/extra/console_env.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/downloads/downloads_tab.py` & `Rare-1.9.5/rare/ui/components/tabs/downloads/downloads_tab.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_dlc.py` & `Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_dlc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_dlc_widget.py` & `Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_dlc_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_info.py` & `Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_info.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/game_info/game_settings.py` & `Rare-1.9.5/rare/ui/components/tabs/games/game_info/game_settings.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/integrations/egl_sync_group.py` & `Rare-1.9.5/rare/ui/components/tabs/games/integrations/egl_sync_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/integrations/egl_sync_list_group.py` & `Rare-1.9.5/rare/ui/components/tabs/games/integrations/egl_sync_list_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/integrations/eos_widget.py` & `Rare-1.9.5/rare/ui/components/tabs/games/integrations/eos_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/games/integrations/import_group.py` & `Rare-1.9.5/rare/ui/components/tabs/games/integrations/import_group.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/about.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/about.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/legendary.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/legendary.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/linux.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/linux.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/proton.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/proton.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/rare.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/rare.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/widgets/dxvk.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/widgets/dxvk.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/widgets/env_vars.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/widgets/env_vars.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/widgets/overlay.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/widgets/overlay.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/widgets/rpc.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/widgets/rpc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/settings/widgets/wrapper.py` & `Rare-1.9.5/rare/ui/components/tabs/settings/widgets/wrapper.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/store/browse_games.py` & `Rare-1.9.5/rare/ui/components/tabs/store/browse_games.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/store/shop_game_info.py` & `Rare-1.9.5/rare/ui/components/tabs/store/shop_game_info.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/store/store.py` & `Rare-1.9.5/rare/ui/components/tabs/store/store.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/store/wishlist.py` & `Rare-1.9.5/rare/ui/components/tabs/store/wishlist.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/components/tabs/store/wishlist_widget.py` & `Rare-1.9.5/rare/ui/components/tabs/store/wishlist_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/ui/utils/pathedit.py` & `Rare-1.9.5/rare/ui/utils/pathedit.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/config_helper.py` & `Rare-1.9.5/rare/utils/config_helper.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/extra_widgets.py` & `Rare-1.9.5/rare/utils/extra_widgets.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/json_formatter.py` & `Rare-1.9.5/rare/utils/json_formatter.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/legendary_utils.py` & `Rare-1.9.5/rare/utils/legendary_utils.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/meta.py` & `Rare-1.9.5/rare/utils/meta.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/misc.py` & `Rare-1.9.5/rare/utils/misc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/models.py` & `Rare-1.9.5/rare/utils/models.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/paths.py` & `Rare-1.9.5/rare/utils/paths.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/qt_requests.py` & `Rare-1.9.5/rare/utils/qt_requests.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/rpc.py` & `Rare-1.9.5/rare/utils/rpc.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/singleton.py` & `Rare-1.9.5/rare/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/utils/steam_grades.py` & `Rare-1.9.5/rare/utils/steam_grades.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/collapsible_widget.py` & `Rare-1.9.5/rare/widgets/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/elide_label.py` & `Rare-1.9.5/rare/widgets/elide_label.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/flow_layout.py` & `Rare-1.9.5/rare/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/image_widget.py` & `Rare-1.9.5/rare/widgets/image_widget.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/library_layout.py` & `Rare-1.9.5/rare/widgets/library_layout.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/rare_app.py` & `Rare-1.9.5/rare/widgets/rare_app.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/rare/widgets/sliding_stack.py` & `Rare-1.9.5/rare/widgets/sliding_stack.py`

 * *Files identical despite different names*

### Comparing `Rare-1.9.4/setup.py` & `Rare-1.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rare import __version__ as version
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [
     "requests<3.0",
-    "legendary-gl==0.20.31",
+    "legendary-gl==0.20.32",
     "setuptools",
     "wheel",
     "PyQt5",
     "QtAwesome",
     'pywin32; platform_system == "Windows"',
     "typing_extensions"
 ]
```

