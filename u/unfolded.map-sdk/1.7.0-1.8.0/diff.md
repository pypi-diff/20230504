# Comparing `tmp/unfolded.map-sdk-1.7.0.tar.gz` & `tmp/unfolded.map-sdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfolded.map-sdk-1.7.0.tar", last modified: Tue Apr 25 04:18:29 2023, max compression
+gzip compressed data, was "unfolded.map-sdk-1.8.0.tar", last modified: Thu May  4 15:49:07 2023, max compression
```

## Comparing `unfolded.map-sdk-1.7.0.tar` & `unfolded.map-sdk-1.8.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.933024 unfolded.map-sdk-1.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-04-25 04:15:59.000000 unfolded.map-sdk-1.7.0/docs/source/_static/embed-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.933024 unfolded.map-sdk-1.7.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/scripts/rename_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.933024 unfolded.map-sdk-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.933024 unfolded.map-sdk-1.7.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/api/test_dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/api/test_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/api/test_layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/api/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/fixtures/dataset_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/tests/fixtures/raster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/fixtures/raster/collection/
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/fixtures/raster/item/
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/fixtures/raster/item/sentinel-2-l2a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/fixtures/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/mocks/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_iframe_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_template_rendering/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/test_html_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/test_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/test_widget_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.929024 unfolded.map-sdk-1.7.0/unfolded/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/_async_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/create_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/dataset_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/event_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/layer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/colab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/4.1d6b2ee6b4adaa5011d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/480.07947b701030e20bd6a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/568.c4c2c97499e36629de31.js
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/747.52c1033b21b19cfefa35.js
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/remoteEntry.fd6179891fa0411b63ce.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 04:18:27.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-04-25 04:18:24.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/templates/html_map_sdk.j2
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transfer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.941024 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/action_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:18:29.937024 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 04:18:29.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/unfolded.map_sdk.json
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-25 04:10:16.000000 unfolded.map-sdk-1.7.0/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.961337 unfolded.map-sdk-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 15:49:07.961337 unfolded.map-sdk-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    25658 2023-05-04 15:46:38.000000 unfolded.map-sdk-1.8.0/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/scripts/rename_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-04 15:49:07.961337 unfolded.map-sdk-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/api/test_dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/api/test_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/api/test_layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/api/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/fixtures/dataset_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/tests/fixtures/raster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/fixtures/raster/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/fixtures/raster/item/
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/fixtures/raster/item/sentinel-2-l2a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/fixtures/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/mocks/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_iframe_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_template_rendering/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/test_html_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/test_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/test_widget_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.949337 unfolded.map-sdk-1.8.0/unfolded/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/_async_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/create_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/dataset_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/event_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17979 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/layer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21910 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/colab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/4.73406aceb9bb0a52322f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17474 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/480.f1b7298a86c01bc22dff.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/568.60f49bd7c7010d71ba45.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/remoteEntry.39a2d353490d0e44cd24.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 15:49:05.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-05-04 15:49:02.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/templates/html_map_sdk.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transfer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.957337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.961337 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/action_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:49:07.953337 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 15:49:07.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/unfolded.map_sdk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-04 15:41:14.000000 unfolded.map-sdk-1.8.0/webpack.config.js
```

### Comparing `unfolded.map-sdk-1.7.0/MANIFEST.in` & `unfolded.map-sdk-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/PKG-INFO` & `unfolded.map-sdk-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.7.0
+Version: 1.8.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.7.0/docs/source/_static/embed-bundle.js` & `unfolded.map-sdk-1.8.0/docs/source/_static/embed-bundle.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,135 +2,137 @@
     var t = {
             889: (e, t, n) => {
                 (t = n(352)(!1)).push([e.id, ".unfolded-widget iframe {\n    border: none;\n}\n", ""]), e.exports = t
             },
             848: (e, t, n) => {
                 "use strict";
                 n.r(t), n.d(t, {
-                    MapError: () => a,
-                    createMap: () => i
+                    EventType: () => r,
+                    MapError: () => i,
+                    createMap: () => d
                 });
-                var s = (e, t, n) => new Promise(((s, a) => {
+                var a, s = (e, t, n) => new Promise(((a, s) => {
                         var r = e => {
                                 try {
                                     o(n.next(e))
                                 } catch (e) {
-                                    a(e)
+                                    s(e)
                                 }
                             },
                             i = e => {
                                 try {
                                     o(n.throw(e))
                                 } catch (e) {
-                                    a(e)
+                                    s(e)
                                 }
                             },
-                            o = e => e.done ? s(e.value) : Promise.resolve(e.value).then(r, i);
+                            o = e => e.done ? a(e.value) : Promise.resolve(e.value).then(r, i);
                         o((n = n.apply(e, t)).next())
                     })),
-                    a = class extends Error {
+                    r = ((a = r || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
+                    i = class extends Error {
                         constructor(e) {
-                            super(e), Object.setPrototypeOf(this, a.prototype)
+                            super(e), Object.setPrototypeOf(this, i.prototype)
                         }
                     },
-                    r = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
+                    o = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
-                function i() {
+                function d() {
                     return s(this, arguments, (function*(e = {}, t) {
-                        let n, s = "https://studio.foursquare.com/studio-bundle.js";
-                        d(t) && (s = t.url, n = t.namespace);
+                        let n, a = "https://studio.foursquare.com/studio-bundle.js";
+                        c(t) && (a = t.url, n = t.namespace);
                         let {
-                            showPlaceholder: a = !0
+                            showPlaceholder: s = !0
                         } = e;
-                        return e.container && a && (e.container.innerHTML = r), (yield l({
-                            url: s,
+                        return e.container && s && (e.container.innerHTML = o), (yield u({
+                            url: a,
                             namespace: n
                         }))(e)
                     }))
                 }
-                var o = {};
+                var l = {};
 
-                function d(e) {
+                function c(e) {
                     return "object" == typeof e && null !== e && "url" in e && ("string" == typeof e.namespace || void 0 === e.namespace)
                 }
 
-                function l(e) {
+                function u(e) {
                     let {
                         url: t,
                         namespace: n = "Unfolded.SDK.v1"
                     } = e, a = `${t}::${n}`;
-                    if (void 0 !== o[a]) return o[a];
+                    if (void 0 !== l[a]) return l[a];
                     let r = document.createElement("script");
-                    o[a] = new Promise(((e, a) => {
+                    l[a] = new Promise(((e, a) => {
                         r.onload = () => s(this, null, (function*() {
                             var s;
                             let r = null == (s = function(e, t) {
                                 return t.split(".").reduce(((e, t) => {
                                     if (e && "object" == typeof e && t in e) return e[t]
                                 }), e)
                             }(globalThis, n)) ? void 0 : s.createMap;
                             r ? e(r) : a(new Error(`Failed to load map interface from ${t}`))
                         })), r.onerror = a
                     })), r.type = "text/javascript", r.src = t;
                     let i = document.querySelector("head");
-                    return null == i || i.appendChild(r), o[a]
+                    return null == i || i.appendChild(r), l[a]
                 }
             },
             352: e => {
                 "use strict";
                 e.exports = function(e) {
                     var t = [];
                     return t.toString = function() {
                         return this.map((function(t) {
                             var n = function(e, t) {
-                                var n, s, a, r = e[1] || "",
+                                var n, a, s, r = e[1] || "",
                                     i = e[3];
                                 if (!i) return r;
                                 if (t && "function" == typeof btoa) {
-                                    var o = (n = i, s = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), a = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(s), "/*# ".concat(a, " */")),
+                                    var o = (n = i, a = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(a), "/*# ".concat(s, " */")),
                                         d = i.sources.map((function(e) {
                                             return "/*# sourceURL=".concat(i.sourceRoot || "").concat(e, " */")
                                         }));
                                     return [r].concat(d).concat([o]).join("\n")
                                 }
                                 return [r].join("\n")
                             }(t, e);
                             return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                         })).join("")
-                    }, t.i = function(e, n, s) {
+                    }, t.i = function(e, n, a) {
                         "string" == typeof e && (e = [
                             [null, e, ""]
                         ]);
-                        var a = {};
-                        if (s)
+                        var s = {};
+                        if (a)
                             for (var r = 0; r < this.length; r++) {
                                 var i = this[r][0];
-                                null != i && (a[i] = !0)
+                                null != i && (s[i] = !0)
                             }
                         for (var o = 0; o < e.length; o++) {
                             var d = [].concat(e[o]);
-                            s && a[d[0]] || (n && (d[2] ? d[2] = "".concat(n, " and ").concat(d[2]) : d[2] = n), t.push(d))
+                            a && s[d[0]] || (n && (d[2] ? d[2] = "".concat(n, " and ").concat(d[2]) : d[2] = n), t.push(d))
                         }
                     }, t
                 }
             },
             204: (e, t, n) => {
-                var s = n(379),
-                    a = n(889);
-                "string" == typeof(a = a.__esModule ? a.default : a) && (a = [
-                    [e.id, a, ""]
+                var a = n(379),
+                    s = n(889);
+                "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
+                    [e.id, s, ""]
                 ]);
-                s(a, {
+                a(s, {
                     insert: "head",
                     singleton: !1
-                }), e.exports = a.locals || {}
+                }), e.exports = s.locals || {}
             },
             379: (e, t, n) => {
                 "use strict";
-                var s, a = function() {
+                var a, s = function() {
                         var e = {};
                         return function(t) {
                             if (void 0 === e[t]) {
                                 var n = document.querySelector(t);
                                 if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                                     n = n.contentDocument.head
                                 } catch (e) {
@@ -148,189 +150,189 @@
                         if (r[n].identifier === e) {
                             t = n;
                             break
                         } return t
                 }
 
                 function o(e, t) {
-                    for (var n = {}, s = [], a = 0; a < e.length; a++) {
-                        var o = e[a],
+                    for (var n = {}, a = [], s = 0; s < e.length; s++) {
+                        var o = e[s],
                             d = t.base ? o[0] + t.base : o[0],
                             l = n[d] || 0,
                             c = "".concat(d, " ").concat(l);
                         n[d] = l + 1;
                         var u = i(c),
                             p = {
                                 css: o[1],
                                 media: o[2],
                                 sourceMap: o[3]
                             }; - 1 !== u ? (r[u].references++, r[u].updater(p)) : r.push({
                             identifier: c,
                             updater: _(p, t),
                             references: 1
-                        }), s.push(c)
+                        }), a.push(c)
                     }
-                    return s
+                    return a
                 }
 
                 function d(e) {
                     var t = document.createElement("style"),
-                        s = e.attributes || {};
-                    if (void 0 === s.nonce) {
+                        a = e.attributes || {};
+                    if (void 0 === a.nonce) {
                         var r = n.nc;
-                        r && (s.nonce = r)
+                        r && (a.nonce = r)
                     }
-                    if (Object.keys(s).forEach((function(e) {
-                            t.setAttribute(e, s[e])
+                    if (Object.keys(a).forEach((function(e) {
+                            t.setAttribute(e, a[e])
                         })), "function" == typeof e.insert) e.insert(t);
                     else {
-                        var i = a(e.insert || "head");
+                        var i = s(e.insert || "head");
                         if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                         i.appendChild(t)
                     }
                     return t
                 }
                 var l, c = (l = [], function(e, t) {
                     return l[e] = t, l.filter(Boolean).join("\n")
                 });
 
-                function u(e, t, n, s) {
-                    var a = n ? "" : s.media ? "@media ".concat(s.media, " {").concat(s.css, "}") : s.css;
-                    if (e.styleSheet) e.styleSheet.cssText = c(t, a);
+                function u(e, t, n, a) {
+                    var s = n ? "" : a.media ? "@media ".concat(a.media, " {").concat(a.css, "}") : a.css;
+                    if (e.styleSheet) e.styleSheet.cssText = c(t, s);
                     else {
-                        var r = document.createTextNode(a),
+                        var r = document.createTextNode(s),
                             i = e.childNodes;
                         i[t] && e.removeChild(i[t]), i.length ? e.insertBefore(r, i[t]) : e.appendChild(r)
                     }
                 }
 
                 function p(e, t, n) {
-                    var s = n.css,
-                        a = n.media,
+                    var a = n.css,
+                        s = n.media,
                         r = n.sourceMap;
-                    if (a ? e.setAttribute("media", a) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = s;
+                    if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = a;
                     else {
                         for (; e.firstChild;) e.removeChild(e.firstChild);
-                        e.appendChild(document.createTextNode(s))
+                        e.appendChild(document.createTextNode(a))
                     }
                 }
                 var f = null,
                     m = 0;
 
                 function _(e, t) {
-                    var n, s, a;
+                    var n, a, s;
                     if (t.singleton) {
                         var r = m++;
-                        n = f || (f = d(t)), s = u.bind(null, n, r, !1), a = u.bind(null, n, r, !0)
-                    } else n = d(t), s = p.bind(null, n, t), a = function() {
+                        n = f || (f = d(t)), a = u.bind(null, n, r, !1), s = u.bind(null, n, r, !0)
+                    } else n = d(t), a = p.bind(null, n, t), s = function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(n)
                     };
-                    return s(e),
+                    return a(e),
                         function(t) {
                             if (t) {
                                 if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                                s(e = t)
-                            } else a()
+                                a(e = t)
+                            } else s()
                         }
                 }
                 e.exports = function(e, t) {
-                    (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === s && (s = Boolean(window && document && document.all && !window.atob)), s));
+                    (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === a && (a = Boolean(window && document && document.all && !window.atob)), a));
                     var n = o(e = e || [], t);
                     return function(e) {
                         if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                            for (var s = 0; s < n.length; s++) {
-                                var a = i(n[s]);
-                                r[a].references--
+                            for (var a = 0; a < n.length; a++) {
+                                var s = i(n[a]);
+                                r[s].references--
                             }
                             for (var d = o(e, t), l = 0; l < n.length; l++) {
                                 var c = i(n[l]);
                                 0 === r[c].references && (r[c].updater(), r.splice(c, 1))
                             }
                             n = d
                         }
                     }
                 }
             },
             607: function(e, t, n) {
                 "use strict";
-                var s = this && this.__createBinding || (Object.create ? function(e, t, n, s) {
-                        void 0 === s && (s = n);
-                        var a = Object.getOwnPropertyDescriptor(t, n);
-                        a && !("get" in a ? !t.__esModule : a.writable || a.configurable) || (a = {
+                var a = this && this.__createBinding || (Object.create ? function(e, t, n, a) {
+                        void 0 === a && (a = n);
+                        var s = Object.getOwnPropertyDescriptor(t, n);
+                        s && !("get" in s ? !t.__esModule : s.writable || s.configurable) || (s = {
                             enumerable: !0,
                             get: function() {
                                 return t[n]
                             }
-                        }), Object.defineProperty(e, s, a)
-                    } : function(e, t, n, s) {
-                        void 0 === s && (s = n), e[s] = t[n]
+                        }), Object.defineProperty(e, a, s)
+                    } : function(e, t, n, a) {
+                        void 0 === a && (a = n), e[a] = t[n]
                     }),
-                    a = this && this.__exportStar || function(e, t) {
-                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || s(t, e, n)
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || a(t, e, n)
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), a(n(412), t), a(n(862), t), a(n(467), t)
+                }), s(n(412), t), s(n(862), t), s(n(467), t)
             },
             944: function(e, t, n) {
                 "use strict";
-                var s = this && this.__awaiter || function(e, t, n, s) {
-                    return new(n || (n = Promise))((function(a, r) {
+                var a = this && this.__awaiter || function(e, t, n, a) {
+                    return new(n || (n = Promise))((function(s, r) {
                         function i(e) {
                             try {
-                                d(s.next(e))
+                                d(a.next(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function o(e) {
                             try {
-                                d(s.throw(e))
+                                d(a.throw(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function d(e) {
                             var t;
-                            e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                            e.done ? s(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(i, o)
                         }
-                        d((s = s.apply(e, t || [])).next())
+                        d((a = a.apply(e, t || [])).next())
                     }))
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 });
-                const a = n(855);
+                const s = n(855);
                 var r;
                 ! function(e) {
                     e.EVENT = "event", e.SUCCESS = "response", e.ERROR = "error"
                 }(r || (r = {})), t.default = class {
                     constructor(e) {
                         this.queue = new Array, this.mapReady = !1, this.destroyed = !1, this.finalize = () => {
                             this.destroyed = !0, this.model.off("msg:custom", this.messageReceived), this.model.stopListening(this.model, "destroy", this.finalize);
                             const e = this.model.map();
                             e && (e.eventHandlers = {})
                         }, this.enableCallbacks = (e, t) => {
                             const n = [];
                             for (const e of t)
-                                if ((0, a.isEventType)(e)) {
-                                    const t = a.eventNamesMap[e];
+                                if ((0, s.isEventType)(e)) {
+                                    const t = s.eventNamesMap[e];
                                     n.push(t)
-                                } const s = {};
-                            for (const e of n) s[e] = t => this.sendCallbackEventToJupyter(a.reverseEventNamesMap[e], t);
-                            e.eventHandlers = Object.assign(Object.assign({}, e.eventHandlers), s)
+                                } const a = {};
+                            for (const e of n) a[e] = t => this.sendCallbackEventToJupyter(s.reverseEventNamesMap[e], t);
+                            e.eventHandlers = Object.assign(Object.assign({}, e.eventHandlers), a)
                         }, this.disableCallbacks = (e, t) => {
-                            for (const n of t) delete e.eventHandlers[a.eventNamesMap[n]]
+                            for (const n of t) delete e.eventHandlers[s.eventNamesMap[n]]
                         }, this.messageReceived = e => {
                             this.destroyed || (this.mapReady ? this.callSDKFunction(e) : this.queue.push(e))
                         }, this.sendResponseToJupyter = (e, t = null) => {
                             if (this.destroyed) return;
                             const n = {
                                 type: r.SUCCESS,
                                 messageId: e,
@@ -354,52 +356,52 @@
                             this.model.send(n, [])
                         }, this.model = e, this.model.on("msg:custom", this.messageReceived), this.model.listenTo(this.model, "destroy", this.finalize)
                     }
                     setMapReady(e) {
                         if (this.mapReady = e, this.mapReady) {
                             let e;
                             for (; void 0 !== (e = this.queue.shift());) this.callSDKFunction(e);
-                            this.sendCallbackEventToJupyter(a.ExtraEventType.ON_LOAD, {})
+                            this.sendCallbackEventToJupyter(s.ExtraEventType.ON_LOAD, {})
                         }
                     }
                     callSDKFunction(e) {
-                        return s(this, void 0, void 0, (function*() {
+                        return a(this, void 0, void 0, (function*() {
                             const {
                                 messageId: t,
                                 type: n,
-                                args: s,
+                                args: a,
                                 options: r
                             } = e, i = this.model.map();
                             if (!i) throw new Error("Cannot call functions before map is rendered");
                             try {
-                                if (n === a.ExtraActionType.SET_EVENT_HANDLERS) return this.enableCallbacks(i, s[0]), this.sendResponseToJupyter(t);
-                                if (n === a.ExtraActionType.REMOVE_EVENT_HANDLERS) return this.disableCallbacks(i, s[0]), this.sendResponseToJupyter(t); {
-                                    const e = a.funcNamesMap[n];
+                                if (n === s.ExtraActionType.SET_EVENT_HANDLERS) return this.enableCallbacks(i, a[0]), this.sendResponseToJupyter(t);
+                                if (n === s.ExtraActionType.REMOVE_EVENT_HANDLERS) return this.disableCallbacks(i, a[0]), this.sendResponseToJupyter(t); {
+                                    const e = s.funcNamesMap[n];
                                     if ("function" == typeof i[e]) {
-                                        const n = yield i[e](...s, r);
+                                        const n = yield i[e](...a, r);
                                         return this.sendResponseToJupyter(t, n)
                                     }
                                 }
                                 throw new Error(`Function ${n} not found`)
                             } catch (e) {
                                 e instanceof Error && this.sendErrorToJupyter(t, e)
                             }
                         }))
                     }
                 }
             },
             855: (e, t) => {
                 "use strict";
-                var n, s, a;
+                var n, a, s;
                 Object.defineProperty(t, "__esModule", {
                         value: !0
                     }), t.isEventType = t.reverseEventNamesMap = t.eventNamesMap = t.ExtraEventType = t.EventType = t.funcNamesMap = t.ExtraActionType = t.ActionType = void 0,
                     function(e) {
                         e.GET_VIEW = "v1/map-sdk-get-view", e.SET_VIEW = "v1/map-sdk-set-view", e.GET_VIEW_LIMITS = "v1/map-sdk-get-view-limits", e.SET_VIEW_LIMITS = "v1/map-sdk-set-view-limits", e.GET_MAP_CONTROL_VISIBILITY = "v1/map-sdk-get-map-control-visibility", e.SET_MAP_CONTROL_VISIBILITY = "v1/map-sdk-set-map-control-visibility", e.GET_SPLIT_MODE = "v1/map-sdk-get-split-mode", e.SET_SPLIT_MODE = "v1/map-sdk-set-split-mode", e.SET_THEME = "v1/map-set-theme", e.GET_MAP_CONFIG = "v1/map-sdk-get-map-config", e.SET_MAP_CONFIG = "v1/map-sdk-set-map-config", e.GET_MAP_STYLES = "v1/map-sdk-get-map-styles", e.GET_FILTERS = "v1/map-sdk-get-filters", e.GET_FILTER_BY_ID = "v1/map-sdk-get-filter-by-id", e.ADD_FILTER = "v1/map-sdk-add-filter", e.UPDATE_FILTER = "v1/map-sdk-update-filter", e.REMOVE_FILTER = "v1/map-sdk-remove-filter", e.UPDATE_TIMELINE = "v1/map-sdk-update-timeline", e.GET_DATASETS = "v1/map-sdk-get-datasets", e.GET_DATASET_BY_ID = "v1/map-sdk-get-dataset-by-id", e.ADD_DATASET = "v1/map-sdk-add-dataset", e.ADD_TILE_DATASET = "v1/map-sdk-add-tile-dataset", e.UPDATE_DATASET = "v1/map-sdk-update-dataset", e.REMOVE_DATASET = "v1/map-sdk-remove-dataset", e.REPLACE_DATASET = "v1/map-sdk-replace-dataset", e.GET_DATASET_WITH_DATA = "v1/map-sdk-get-dataset-with-data", e.GET_LAYERS = "v1/map-sdk-get-layers", e.GET_LAYER_BY_ID = "v1/map-sdk-get-layer-by-id", e.ADD_LAYER = "v1/map-sdk-add-layer", e.UPDATE_LAYER = "v1/map-sdk-update-layer", e.REMOVE_LAYER = "v1/map-sdk-remove-layer", e.GET_LAYER_GROUPS = "v1/map-sdk-get-layer-groups", e.GET_LAYER_GROUP_BY_ID = "v1/map-sdk-get-layer-group-by-id", e.ADD_LAYER_GROUP = "v1/map-sdk-add-layer-group", e.UPDATE_LAYER_GROUP = "v1/map-sdk-update-layer-group", e.REMOVE_LAYER_GROUP = "v1/map-sdk-remove-layer-group", e.GET_LAYER_TIMELINE = "v1/map-sdk-get-layer-timeline", e.UPDATE_LAYER_TIMELINE = "v1/map-sdk-update-layer-timeline"
-                    }(n = t.ActionType || (t.ActionType = {})), (a = t.ExtraActionType || (t.ExtraActionType = {})).SET_EVENT_HANDLERS = "v1/map-sdk-set-event-handlers", a.REMOVE_EVENT_HANDLERS = "v1/map-sdk-remove-event-handlers", t.funcNamesMap = {
+                    }(n = t.ActionType || (t.ActionType = {})), (s = t.ExtraActionType || (t.ExtraActionType = {})).SET_EVENT_HANDLERS = "v1/map-sdk-set-event-handlers", s.REMOVE_EVENT_HANDLERS = "v1/map-sdk-remove-event-handlers", t.funcNamesMap = {
                         [n.GET_VIEW]: "getView",
                         [n.SET_VIEW]: "setView",
                         [n.GET_VIEW_LIMITS]: "getViewLimits",
                         [n.SET_VIEW_LIMITS]: "setViewLimits",
                         [n.GET_MAP_CONTROL_VISIBILITY]: "getMapControlVisibility",
                         [n.SET_MAP_CONTROL_VISIBILITY]: "setMapControlVisibility",
                         [n.GET_SPLIT_MODE]: "getSplitMode",
@@ -433,47 +435,47 @@
                         [n.UPDATE_LAYER_GROUP]: "updateLayerGroup",
                         [n.REMOVE_LAYER_GROUP]: "removeLayerGroup",
                         [n.GET_LAYER_TIMELINE]: "getLayerTimeline",
                         [n.UPDATE_LAYER_TIMELINE]: "updateLayerTimeline"
                     },
                     function(e) {
                         e.ON_CLICK = "v1/map-sdk-on-click", e.ON_HOVER = "v1/map-sdk-on-hover", e.ON_VIEW_UPDATE = "v1/map-sdk-on-view-update", e.ON_GEOMETRY_SELECTION = "v1/map-sdk-on-geometry-selection", e.ON_LAYER_TIMELINE_UPDATE = "v1/map-sdk-on-layer-timeline-update", e.ON_FILTER_UPDATE = "v1/map-sdk-on-filter-update"
-                    }(s = t.EventType || (t.EventType = {})), (t.ExtraEventType || (t.ExtraEventType = {})).ON_LOAD = "v1/map-sdk-on-load", t.eventNamesMap = {
-                        [s.ON_CLICK]: "onClick",
-                        [s.ON_HOVER]: "onHover",
-                        [s.ON_VIEW_UPDATE]: "onViewUpdate",
-                        [s.ON_GEOMETRY_SELECTION]: "onGeometrySelection",
-                        [s.ON_LAYER_TIMELINE_UPDATE]: "onLayerTimelineUpdate",
-                        [s.ON_FILTER_UPDATE]: "onFilterUpdate"
+                    }(a = t.EventType || (t.EventType = {})), (t.ExtraEventType || (t.ExtraEventType = {})).ON_LOAD = "v1/map-sdk-on-load", t.eventNamesMap = {
+                        [a.ON_CLICK]: "onClick",
+                        [a.ON_HOVER]: "onHover",
+                        [a.ON_VIEW_UPDATE]: "onViewUpdate",
+                        [a.ON_GEOMETRY_SELECTION]: "onGeometrySelection",
+                        [a.ON_LAYER_TIMELINE_UPDATE]: "onLayerTimelineUpdate",
+                        [a.ON_FILTER_UPDATE]: "onFilterUpdate"
                     }, t.reverseEventNamesMap = Object.entries(t.eventNamesMap).reduce(((e, [t, n]) => (e[n] = t, e)), {}), t.isEventType = function(e) {
-                        return Object.values(s).includes(e)
+                        return Object.values(a).includes(e)
                     }
             },
             412: (e, t, n) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-                const s = n(147);
-                t.MODULE_VERSION = s.version, t.MODULE_NAME = s.name
+                const a = n(147);
+                t.MODULE_VERSION = a.version, t.MODULE_NAME = a.name
             },
             862: function(e, t, n) {
                 "use strict";
-                var s = this && this.__importDefault || function(e) {
+                var a = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.UnfoldedMapModel = void 0;
-                const a = n(146),
-                    r = s(n(944)),
+                const s = n(146),
+                    r = a(n(944)),
                     i = n(412);
-                class o extends a.DOMWidgetModel {
+                class o extends s.DOMWidgetModel {
                     constructor() {
                         super(...arguments), this.transport = new r.default(this)
                     }
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: o.model_name,
                             _model_module: o.model_module,
@@ -506,55 +508,55 @@
                         const e = this.get("urls");
                         return this.objectOrUndefined(e)
                     }
                     _internal() {
                         return this.get("_internal")
                     }
                 }
-                o.serializers = Object.assign({}, a.DOMWidgetModel.serializers), o.model_name = "UnfoldedMapModel", o.model_module = i.MODULE_NAME, o.model_module_version = i.MODULE_VERSION, o.view_name = "UnfoldedMapView", o.view_module = i.MODULE_NAME, o.view_module_version = i.MODULE_VERSION, t.UnfoldedMapModel = o
+                o.serializers = Object.assign({}, s.DOMWidgetModel.serializers), o.model_name = "UnfoldedMapModel", o.model_module = i.MODULE_NAME, o.model_module_version = i.MODULE_VERSION, o.view_name = "UnfoldedMapView", o.view_module = i.MODULE_NAME, o.view_module_version = i.MODULE_VERSION, t.UnfoldedMapModel = o
             },
             467: function(e, t, n) {
                 "use strict";
-                var s = this && this.__awaiter || function(e, t, n, s) {
-                    return new(n || (n = Promise))((function(a, r) {
+                var a = this && this.__awaiter || function(e, t, n, a) {
+                    return new(n || (n = Promise))((function(s, r) {
                         function i(e) {
                             try {
-                                d(s.next(e))
+                                d(a.next(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function o(e) {
                             try {
-                                d(s.throw(e))
+                                d(a.throw(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function d(e) {
                             var t;
-                            e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                            e.done ? s(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(i, o)
                         }
-                        d((s = s.apply(e, t || [])).next())
+                        d((a = a.apply(e, t || [])).next())
                     }))
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.UnfoldedMapView = void 0;
-                const a = n(146),
+                const s = n(146),
                     r = n(848);
                 n(204);
                 const i = "unfolded-widget";
-                class o extends a.DOMWidgetView {
+                class o extends s.DOMWidgetView {
                     initialize() {
-                        return s(this, void 0, void 0, (function*() {
+                        return a(this, void 0, void 0, (function*() {
                             const e = {
                                 style: this.model.style(),
                                 basemaps: this.model.basemaps(),
                                 raster: this.model.raster(),
                                 urls: this.model.urls()
                             };
                             if (!this.model.map()) {
@@ -574,35 +576,35 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.7.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.7.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@babel/core":"^7.16.0","@babel/preset-env":"^7.16.0","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
-    function s(e) {
-        var a = n[e];
-        if (void 0 !== a) return a.exports;
+    function a(e) {
+        var s = n[e];
+        if (void 0 !== s) return s.exports;
         var r = n[e] = {
             id: e,
             exports: {}
         };
-        return t[e].call(r.exports, r, r.exports, s), r.exports
+        return t[e].call(r.exports, r, r.exports, a), r.exports
     }
-    return s.d = (e, t) => {
-        for (var n in t) s.o(t, n) && !s.o(e, n) && Object.defineProperty(e, n, {
+    return a.d = (e, t) => {
+        for (var n in t) a.o(t, n) && !a.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
-    }, s.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), s.r = e => {
+    }, a.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), a.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, s(607)
+    }, a(607)
 })()));
 //# sourceMappingURL=embed-bundle.js.map
```

### Comparing `unfolded.map-sdk-1.7.0/package.json` & `unfolded.map-sdk-1.8.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9569869614512471%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.8.0'}",*

 * * "'devDependencies'": "{delete: ['@babel/core', '@babel/preset-env']}",*

 * * "'scripts'": "{'generate-licenses': 'node -r esbuild-register ../../../scripts/get-licenses.ts -p "*

 * *              ". -o ./dist/LICENSES.md'}",*

 * * "'version'": "'1.8.0'"}*

```diff
@@ -5,23 +5,21 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.7.0",
+        "@unfolded/map-sdk": "^1.8.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
-        "@babel/core": "^7.16.0",
-        "@babel/preset-env": "^7.16.0",
         "@jupyterlab/builder": "^3.0.0",
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "css-loader": "^3.2.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "npm-run-all": "^4.1.3",
@@ -66,24 +64,24 @@
         "build:nbextension": "webpack --mode production",
         "build:nbextension:dev": "webpack --mode development",
         "build:prod": "yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension",
         "clean": "yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension",
         "clean:labextension": "rimraf unfolded/map_sdk/labextension",
         "clean:lib": "rimraf lib",
         "clean:nbextension": "rimraf 'unfolded/map_sdk/nbextension/index.js*'",
-        "generate-licenses": "node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md",
+        "generate-licenses": "node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md",
         "lint": "eslint --max-warnings 0 src",
         "prepack": "yarn run build:prod",
         "start": "yarn run watch",
         "test": "jest",
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.7.0",
+    "version": "1.8.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.7.0/scripts/rename_package.py` & `unfolded.map-sdk-1.8.0/scripts/rename_package.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/setup.cfg` & `unfolded.map-sdk-1.8.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.7.0
+current_version = 1.8.0
 commit = True
 message = chore(map-sdk): Bump version {current_version} → {new_version}
 tag = False
 tag_name = map-sdk/{new_version}
 
 [bdist_wheel]
 universal = 1
```

### Comparing `unfolded.map-sdk-1.7.0/setup.py` & `unfolded.map-sdk-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/_utils.py` & `unfolded.map-sdk-1.8.0/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/api/test_dataset_api.py` & `unfolded.map-sdk-1.8.0/tests/api/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/api/test_filter_api.py` & `unfolded.map-sdk-1.8.0/tests/api/test_filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/api/test_layer_api.py` & `unfolded.map-sdk-1.8.0/tests/api/test_layer_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/api/test_map_api.py` & `unfolded.map-sdk-1.8.0/tests/api/test_map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/conftest.py` & `unfolded.map-sdk-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/fixtures/dataset_api.py` & `unfolded.map-sdk-1.8.0/tests/fixtures/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json` & `unfolded.map-sdk-1.8.0/tests/fixtures/raster/collection/sentinel-s2-l2a-cogs.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/fixtures/raster/item/sentinel-2-l2a.json` & `unfolded.map-sdk-1.8.0/tests/fixtures/raster/item/sentinel-2-l2a.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/fixtures/test_data.py` & `unfolded.map-sdk-1.8.0/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/mocks/transport.py` & `unfolded.map-sdk-1.8.0/tests/mocks/transport.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html` & `unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_iframe_template_rendering/iframe_map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/snapshots/test_html_map/test_template_rendering/map.html` & `unfolded.map-sdk-1.8.0/tests/snapshots/test_html_map/test_template_rendering/map.html`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/test_html_map.py` & `unfolded.map-sdk-1.8.0/tests/test_html_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/test_serialization.py` & `unfolded.map-sdk-1.8.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/test_subclass.py` & `unfolded.map-sdk-1.8.0/tests/test_subclass.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/test_widget_map.py` & `unfolded.map-sdk-1.8.0/tests/test_widget_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tests/utils/test_validators.py` & `unfolded.map-sdk-1.8.0/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/tsconfig.json` & `unfolded.map-sdk-1.8.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/__init__.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/_async_thread.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/_async_thread.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/_poll_v56/_poll.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/_poll_v56/_poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/base.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/create_map.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/create_map.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/dataset_api.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/enums.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/enums.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/event_api.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/event_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/filter_api.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/filter_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/layer_api.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/layer_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/api/map_api.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/api/map_api.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/environment.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/package.json` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.956391723356009%*

 * *Differences: {"'dependencies'": "{'@unfolded/map-sdk': '^1.8.0'}",*

 * * "'devDependencies'": "{delete: ['@babel/core', '@babel/preset-env']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.39a2d353490d0e44cd24.js'}}",*

 * * "'scripts'": "{'generate-licenses': 'node -r esbuild-register ../../../scripts/get-licenses.ts -p "*

 * *              ". -o ./dist/LICENSES.md'}",*

 * * "'version'": "'1.8.0'"}*

```diff
@@ -5,23 +5,21 @@
     },
     "dependencies": {
         "@aws-amplify/core": "^4.2.9",
         "@jupyter-widgets/base": "^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0",
         "@jupyterlab/rendermime-interfaces": "^1.3.0 || ^2.0.0 || ^3.0.0",
         "@lumino/application": "^1.16.0",
         "@lumino/widgets": "^1.30.0",
-        "@unfolded/map-sdk": "^1.7.0",
+        "@unfolded/map-sdk": "^1.8.0",
         "aws-sdk": "^2.988.0",
         "csstype": "^3.1.0",
         "global": "^4.3.0"
     },
     "description": "JavaScript bindings for Unfolded's Jupyter Map SDK",
     "devDependencies": {
-        "@babel/core": "^7.16.0",
-        "@babel/preset-env": "^7.16.0",
         "@jupyterlab/builder": "^3.0.0",
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "css-loader": "^3.2.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "npm-run-all": "^4.1.3",
@@ -37,15 +35,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fd6179891fa0411b63ce.js",
+            "load": "static/remoteEntry.39a2d353490d0e44cd24.js",
             "mimeExtension": "./mimeExtension"
         },
         "extension": "lib/plugin",
         "mimeExtension": "lib/javascript-renderer-extension.js",
         "outputDir": "unfolded/map_sdk/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -71,24 +69,24 @@
         "build:nbextension": "webpack --mode production",
         "build:nbextension:dev": "webpack --mode development",
         "build:prod": "yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension",
         "clean": "yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension",
         "clean:labextension": "rimraf unfolded/map_sdk/labextension",
         "clean:lib": "rimraf lib",
         "clean:nbextension": "rimraf 'unfolded/map_sdk/nbextension/index.js*'",
-        "generate-licenses": "node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md",
+        "generate-licenses": "node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md",
         "lint": "eslint --max-warnings 0 src",
         "prepack": "yarn run build:prod",
         "start": "yarn run watch",
         "test": "jest",
         "typecheck": "tsc",
         "typescript": "yarn run -T tsc --noEmit",
         "watch": "npm-run-all -p watch:*",
         "watch:lib": "yarn run -T tsc -w",
         "watch:nbextension": "webpack --watch --mode development"
     },
     "types": "lib/index.d.ts",
-    "version": "1.7.0",
+    "version": "1.8.0",
     "volta": {
         "extends": "../../../package.json"
     }
 }
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/4.1d6b2ee6b4adaa5011d0.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/4.73406aceb9bb0a52322f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -29,15 +29,15 @@
                     d((o = o.apply(e, n || [])).next())
                 }))
             };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             }), n.unfoldedRendererFactory = void 0;
             const s = t(832),
-                r = t(253),
+                r = t(782),
                 i = "application/geo+json",
                 a = "text/csv",
                 d = [i, a];
             class u extends s.Widget {
                 constructor(e) {
                     super(), this.addClass("unfolded-rendermime"), this.options = e
                 }
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/480.07947b701030e20bd6a5.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/480.f1b7298a86c01bc22dff.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -337,15 +337,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(253);
+                i = n(782);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -547,11 +547,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.7.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.7.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@babel/core":"^7.16.0","@babel/preset-env":"^7.16.0","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/568.c4c2c97499e36629de31.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/568.60f49bd7c7010d71ba45.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -288,15 +288,15 @@
                     d((s = s.apply(e, t || [])).next())
                 }))
             };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UnfoldedMapView = void 0;
             const a = n(565),
-                i = n(253);
+                i = n(782);
             n(204);
             const r = "unfolded-widget";
             class o extends a.DOMWidgetView {
                 initialize() {
                     return s(this, void 0, void 0, (function*() {
                         const e = {
                             style: this.model.style(),
@@ -498,11 +498,11 @@
                         n = d
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.7.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.7.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@babel/core":"^7.16.0","@babel/preset-env":"^7.16.0","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+            e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/747.52c1033b21b19cfefa35.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,76 +1,78 @@
 "use strict";
 (self.webpackChunk_unfolded_jupyter_map_sdk = self.webpackChunk_unfolded_jupyter_map_sdk || []).push([
     [747], {
-        747: (n, t, e) => {
-            e.r(t), e.d(t, {
-                MapError: () => r,
-                createMap: () => o
+        747: (n, e, t) => {
+            t.r(e), t.d(e, {
+                EventType: () => s,
+                MapError: () => o,
+                createMap: () => f
             });
-            var a = (n, t, e) => new Promise(((a, r) => {
+            var a, r = (n, e, t) => new Promise(((a, r) => {
                     var s = n => {
                             try {
-                                i(e.next(n))
+                                i(t.next(n))
                             } catch (n) {
                                 r(n)
                             }
                         },
                         o = n => {
                             try {
-                                i(e.throw(n))
+                                i(t.throw(n))
                             } catch (n) {
                                 r(n)
                             }
                         },
                         i = n => n.done ? a(n.value) : Promise.resolve(n.value).then(s, o);
-                    i((e = e.apply(n, t)).next())
+                    i((t = t.apply(n, e)).next())
                 })),
-                r = class extends Error {
+                s = ((a = s || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
+                o = class extends Error {
                     constructor(n) {
-                        super(n), Object.setPrototypeOf(this, r.prototype)
+                        super(n), Object.setPrototypeOf(this, o.prototype)
                     }
                 },
-                s = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
+                i = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
-            function o() {
-                return a(this, arguments, (function*(n = {}, t) {
-                    let e, a = "https://studio.foursquare.com/studio-bundle.js";
-                    f(t) && (a = t.url, e = t.namespace);
+            function f() {
+                return r(this, arguments, (function*(n = {}, e) {
+                    let t, a = "https://studio.foursquare.com/studio-bundle.js";
+                    d(e) && (a = e.url, t = e.namespace);
                     let {
                         showPlaceholder: r = !0
                     } = n;
-                    return n.container && r && (n.container.innerHTML = s), (yield l({
+                    return n.container && r && (n.container.innerHTML = i), (yield c({
                         url: a,
-                        namespace: e
+                        namespace: t
                     }))(n)
                 }))
             }
-            var i = {};
+            var l = {};
 
-            function f(n) {
+            function d(n) {
                 return "object" == typeof n && null !== n && "url" in n && ("string" == typeof n.namespace || void 0 === n.namespace)
             }
 
-            function l(n) {
+            function c(n) {
                 let {
-                    url: t,
-                    namespace: e = "Unfolded.SDK.v1"
-                } = n, r = `${t}::${e}`;
-                if (void 0 !== i[r]) return i[r];
+                    url: e,
+                    namespace: t = "Unfolded.SDK.v1"
+                } = n, a = `${e}::${t}`;
+                if (void 0 !== l[a]) return l[a];
                 let s = document.createElement("script");
-                i[r] = new Promise(((n, r) => {
-                    s.onload = () => a(this, null, (function*() {
-                        var a;
-                        let s = null == (a = function(n, t) {
-                            return t.split(".").reduce(((n, t) => {
-                                if (n && "object" == typeof n && t in n) return n[t]
+                l[a] = new Promise(((n, a) => {
+                    s.onload = () => r(this, null, (function*() {
+                        var r;
+                        let s = null == (r = function(n, e) {
+                            return e.split(".").reduce(((n, e) => {
+                                if (n && "object" == typeof n && e in n) return n[e]
                             }), n)
-                        }(globalThis, e)) ? void 0 : a.createMap;
-                        s ? n(s) : r(new Error(`Failed to load map interface from ${t}`))
-                    })), s.onerror = r
-                })), s.type = "text/javascript", s.src = t;
+                        }(globalThis, t)) ? void 0 : r.createMap;
+                        s ? n(s) : a(new Error(`Failed to load map interface from ${e}`))
+                    })), s.onerror = a
+                })), s.type = "text/javascript", s.src = e;
                 let o = document.querySelector("head");
-                return null == o || o.appendChild(s), i[r]
+                return null == o || o.appendChild(s), l[a]
             }
         }
     }
 ]);
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/remoteEntry.fd6179891fa0411b63ce.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/remoteEntry.39a2d353490d0e44cd24.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, d, l, f, s, p, c, h, v, m, g, b = {
+    var e, r, t, n, o, a, i, u, d, l, s, f, p, c, h, v, m, b, g = {
             768: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(253), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(253), t.e(565), t.e(480)]).then((() => () => t(480))),
-                        "./mimeExtension": () => Promise.all([t.e(253), t.e(4)]).then((() => () => t(4)))
+                        "./index": () => Promise.all([t.e(782), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(782), t.e(565), t.e(480)]).then((() => () => t(480))),
+                        "./mimeExtension": () => Promise.all([t.e(782), t.e(4)]).then((() => () => t(4)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = t.S.default,
@@ -30,65 +30,65 @@
     function w(e) {
         var r = y[e];
         if (void 0 !== r) return r.exports;
         var t = y[e] = {
             id: e,
             exports: {}
         };
-        return b[e].call(t.exports, t, t.exports, w), t.exports
+        return g[e].call(t.exports, t, t.exports, w), t.exports
     }
-    w.m = b, w.c = y, w.d = (e, r) => {
+    w.m = g, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        4: "1d6b2ee6b4adaa5011d0",
-        253: "0ecc373f65ef8d5920de",
-        480: "07947b701030e20bd6a5",
+        4: "73406aceb9bb0a52322f",
+        480: "f1b7298a86c01bc22dff",
         565: "6aa0248333a228f5539f",
-        568: "c4c2c97499e36629de31",
-        747: "52c1033b21b19cfefa35"
+        568: "60f49bd7c7010d71ba45",
+        747: "488cf0ee36d815959581",
+        782: "d313a04c73596eda42d2"
     } [e] + ".js?v=" + {
-        4: "1d6b2ee6b4adaa5011d0",
-        253: "0ecc373f65ef8d5920de",
-        480: "07947b701030e20bd6a5",
+        4: "73406aceb9bb0a52322f",
+        480: "f1b7298a86c01bc22dff",
         565: "6aa0248333a228f5539f",
-        568: "c4c2c97499e36629de31",
-        747: "52c1033b21b19cfefa35"
+        568: "60f49bd7c7010d71ba45",
+        747: "488cf0ee36d815959581",
+        782: "d313a04c73596eda42d2"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@unfolded/jupyter-map-sdk:", w.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var d = document.getElementsByTagName("script"), l = 0; l < d.length; l++) {
-                    var f = d[l];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                    var s = d[l];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -110,15 +110,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     d = [];
-                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.7.0", (() => Promise.all([w.e(253), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.7.0", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@unfolded/jupyter-map-sdk", "1.8.0", (() => Promise.all([w.e(782), w.e(568)]).then((() => () => w(568))))), u("@unfolded/map-sdk", "1.8.0", (() => w.e(747).then((() => () => w(747)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,33 +167,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, d = !0;; u++, i++) {
-                var l, f, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(l = r[i]))[0])) return !d || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == f) {
-                    if (!d || "u" != s) return !1
+                var l, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !d || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
+                    if (!d || "u" != f) return !1
                 } else if (d)
-                    if (s == f)
+                    if (f == s)
                         if (u <= n) {
                             if (l != e[u]) return !1
                         } else {
                             if (o ? l > e[u] : l < e[u]) return !1;
                             l != e[u] && (d = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     d = !1, u--
                 } else {
-                    if (u <= n || f < s != o) return !1;
+                    if (u <= n || s < f != o) return !1;
                     d = !1
-                } else "s" != s && "n" != s && (d = !1, u--)
+                } else "s" != f && "n" != f && (d = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -204,39 +204,39 @@
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), s(e[t][o])
-    }, f = (e, r, t) => {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(d(e, t, o, n)), f(e[t][o])
+    }, s = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
         var a = w.I(r);
         return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && f(r, t, n);
-        return a ? s(a) : o()
+        var a = r && w.o(r, t) && s(r, t, n);
+        return a ? f(a) : o()
     })), v = {}, m = {
-        253: () => h("default", "@unfolded/map-sdk", [1, 1, 7, 0], (() => w.e(747).then((() => () => w(747))))),
+        782: () => h("default", "@unfolded/map-sdk", [1, 1, 8, 0], (() => w.e(747).then((() => () => w(747))))),
         565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ]),
         832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
-    }, g = {
+    }, b = {
         4: [832],
-        253: [253],
         565: [565],
-        568: [565]
+        568: [565],
+        782: [782]
     }, w.f.consumes = (e, r) => {
-        w.o(g, e) && g[e].forEach((e => {
+        w.o(b, e) && b[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
@@ -255,15 +255,15 @@
         var e = {
             754: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(253|565)$/.test(r)) e[r] = 0;
+                else if (/^(565|782)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
                 var a = w.p + w.u(r),
                     i = new Error;
                 w.l(a, (t => {
                     if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/labextension/static/third-party-licenses.json` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '1.8.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "UNLICENSED",
             "name": "@unfolded/map-sdk",
-            "versionInfo": "1.7.0"
+            "versionInfo": "1.8.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "3.6.0"
         },
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/base.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/html.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/map/widget.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/map/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/nbextension/index.js` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/nbextension/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,135 +2,137 @@
     var t = {
             889: (e, t, n) => {
                 (t = n(352)(!1)).push([e.id, ".unfolded-widget iframe {\n    border: none;\n}\n", ""]), e.exports = t
             },
             848: (e, t, n) => {
                 "use strict";
                 n.r(t), n.d(t, {
-                    MapError: () => a,
-                    createMap: () => i
+                    EventType: () => r,
+                    MapError: () => i,
+                    createMap: () => d
                 });
-                var s = (e, t, n) => new Promise(((s, a) => {
+                var a, s = (e, t, n) => new Promise(((a, s) => {
                         var r = e => {
                                 try {
                                     o(n.next(e))
                                 } catch (e) {
-                                    a(e)
+                                    s(e)
                                 }
                             },
                             i = e => {
                                 try {
                                     o(n.throw(e))
                                 } catch (e) {
-                                    a(e)
+                                    s(e)
                                 }
                             },
-                            o = e => e.done ? s(e.value) : Promise.resolve(e.value).then(r, i);
+                            o = e => e.done ? a(e.value) : Promise.resolve(e.value).then(r, i);
                         o((n = n.apply(e, t)).next())
                     })),
-                    a = class extends Error {
+                    r = ((a = r || {}).REMOVE_DATASET = "remove-dataset", a.ADD_LAYER = "add-layer", a.REMOVE_LAYER = "remove-layer", a.ADD_LAYER_GROUP = "add-layer-group", a.REMOVE_LAYER_GROUP = "remove-layer-group", a.ACTIVATE_MAP_CONTROL = "activate-map-control", a.CHANGE_SIDE_PANEL_SECTION = "change-side-panel-section", a),
+                    i = class extends Error {
                         constructor(e) {
-                            super(e), Object.setPrototypeOf(this, a.prototype)
+                            super(e), Object.setPrototypeOf(this, i.prototype)
                         }
                     },
-                    r = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
+                    o = '<div class="map-placeholder">\n  <style>\n    .map-placeholder {\n      position: absolute;\n      top: 0;\n      left: 0;\n      right: 0;\n      width: 100%;\n      height: 100%;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .scene {\n      width: 50px;\n      height: 50px;\n      transform-style: preserve-3d;\n      transform: rotateY(0deg) rotateX(56deg) rotateZ(-45deg);\n    }\n\n    @keyframes fsq-rotate {\n      0% {\n        transform: rotateY(0deg);\n      }\n      5%, 25% {\n        transform: rotateX(-90deg);\n      }\n      30%, 50% {\n        transform: rotateX(-90deg) rotateY(-90deg);\n      }\n      55%, 75% {\n        transform: rotateX(-90deg) rotateY(-90deg) rotateX(-90deg);\n      }\n      80%, 100% {\n        transform: rotateX(-90deg) rotateY(0deg) rotateX(-90deg);\n      }\n    }\n\n    .fsq {\n      width: 50px;\n      height: 50px;\n      position: relative;\n      transform-style: preserve-3d;\n      transition: transform 1s;\n      animation-name: fsq-rotate;\n      animation-iteration-count: infinite;\n      animation-duration: 6s;\n      animation-timing-function: ease;\n    }\n\n    .fsq__face {\n      position: absolute;\n      width: 50px;\n      height: 50px;\n      display: flex;\n      align-items: center;\n      justify-content: center;\n    }\n\n    .fsq__face--front-f {\n      background: #000;\n      transform: rotateY(0deg) translateZ(25px);\n    }\n\n    .fsq__face--back-f {\n      background: #000;\n      transform: rotateZ(-180deg) rotateY(180deg) translateZ(25px);\n    }\n\n    .fsq__face--right-s {\n      background: #fff;\n      transform: rotateY(90deg) translateZ(25px);\n    }\n\n    .fsq__face--left-s {\n      background: #fff;\n      transform: rotateX(-90deg) rotateY(-90deg) rotateZ(180deg) translateZ(25px);\n    }\n\n    .fsq__face--top-q {\n      background: #3545f5;\n      transform: rotateX(90deg) translateZ(25px);\n    }\n\n    .fsq__face--bottom-q {\n      background: #3545f5;\n      transform: rotateX(-90deg) translateZ(25px);\n    }\n  </style>\n\n\n  <div class="scene">\n    <div class="fsq">\n      <div class="fsq__face fsq__face--front-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--back-f">\n        <svg\n            width="11"\n            height="16"\n            viewBox="0 0 22 33"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0 0.753143H21.6663V4.48508H3.76033V14.2084H19.6551V17.9404H3.76033V32.2673H0V0.753143Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--right-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--left-s">\n        <svg\n            width="13"\n            height="17"\n            viewBox="0 0 25 34"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.865906 23.2463L4.63468 22.4932C5.38674 26.9783 8.23446 29.2801 12.9581 29.2801C17.5212 29.2801 20.6985 27.1052 20.6985 23.9995C20.6985 21.2746 18.231 19.3875 12.206 17.6357C4.88819 15.537 1.74472 12.4398 1.74472 8.08163C1.74472 3.09725 5.84306 0 12.4088 0C18.8056 0 22.6589 2.93647 23.9518 8.54707L20.0647 9.38485C19.2281 5.6106 16.7184 3.73194 12.3243 3.73194C8.22601 3.73194 5.67406 5.32288 5.67406 8.04778C5.67406 10.5611 7.80349 12.279 13.7862 14.1238C21.6533 16.5102 24.5771 19.6075 24.5771 24.008C24.5771 29.5001 20.0985 33.0543 13.1525 33.0543C6.20641 33.0543 1.91373 29.6185 0.865906 23.2463Z"\n              fill="#000"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--top-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n      <div class="fsq__face fsq__face--bottom-q">\n        <svg\n            width="16"\n            height="17"\n            viewBox="0 0 32 35"\n            fill="none"\n            xmlns="http://www.w3.org/2000/svg"\n        >\n          <path\n              d="M0.881409 16.6287C0.881409 7.28616 6.99088 0 16.3621 0C25.6911 0 31.7161 7.32848 31.7161 16.6287C31.7161 21.2407 30.212 25.2604 27.6178 28.1461C28.8769 29.3985 30.0852 30.6594 31.2598 31.9542L28.5811 34.5945C27.3643 33.2997 26.0714 31.9542 24.7701 30.6171C22.3871 32.1657 19.5394 33.0458 16.3621 33.0458C7.32889 33.0543 0.881409 26.0982 0.881409 16.6287ZM21.9223 27.8584C20.6633 26.6821 19.4549 25.5143 18.1958 24.4226L20.8323 21.7823C22.1674 22.9586 23.511 24.1687 24.8039 25.3873C26.6038 23.1702 27.6938 20.1491 27.6938 16.5864C27.6938 9.30023 23.2575 3.76579 16.3537 3.76579C9.44989 3.76579 4.97129 9.29176 4.97129 16.5864C4.97129 24.0418 9.77944 29.3224 16.3537 29.3224C18.4155 29.3224 20.2915 28.8231 21.9223 27.8584Z"\n              fill="white"\n          />\n        </svg>\n      </div>\n    </div>\n  </div>\n</div>';
 
-                function i() {
+                function d() {
                     return s(this, arguments, (function*(e = {}, t) {
-                        let n, s = "https://studio.foursquare.com/studio-bundle.js";
-                        d(t) && (s = t.url, n = t.namespace);
+                        let n, a = "https://studio.foursquare.com/studio-bundle.js";
+                        c(t) && (a = t.url, n = t.namespace);
                         let {
-                            showPlaceholder: a = !0
+                            showPlaceholder: s = !0
                         } = e;
-                        return e.container && a && (e.container.innerHTML = r), (yield l({
-                            url: s,
+                        return e.container && s && (e.container.innerHTML = o), (yield u({
+                            url: a,
                             namespace: n
                         }))(e)
                     }))
                 }
-                var o = {};
+                var l = {};
 
-                function d(e) {
+                function c(e) {
                     return "object" == typeof e && null !== e && "url" in e && ("string" == typeof e.namespace || void 0 === e.namespace)
                 }
 
-                function l(e) {
+                function u(e) {
                     let {
                         url: t,
                         namespace: n = "Unfolded.SDK.v1"
                     } = e, a = `${t}::${n}`;
-                    if (void 0 !== o[a]) return o[a];
+                    if (void 0 !== l[a]) return l[a];
                     let r = document.createElement("script");
-                    o[a] = new Promise(((e, a) => {
+                    l[a] = new Promise(((e, a) => {
                         r.onload = () => s(this, null, (function*() {
                             var s;
                             let r = null == (s = function(e, t) {
                                 return t.split(".").reduce(((e, t) => {
                                     if (e && "object" == typeof e && t in e) return e[t]
                                 }), e)
                             }(globalThis, n)) ? void 0 : s.createMap;
                             r ? e(r) : a(new Error(`Failed to load map interface from ${t}`))
                         })), r.onerror = a
                     })), r.type = "text/javascript", r.src = t;
                     let i = document.querySelector("head");
-                    return null == i || i.appendChild(r), o[a]
+                    return null == i || i.appendChild(r), l[a]
                 }
             },
             352: e => {
                 "use strict";
                 e.exports = function(e) {
                     var t = [];
                     return t.toString = function() {
                         return this.map((function(t) {
                             var n = function(e, t) {
-                                var n, s, a, r = e[1] || "",
+                                var n, a, s, r = e[1] || "",
                                     i = e[3];
                                 if (!i) return r;
                                 if (t && "function" == typeof btoa) {
-                                    var o = (n = i, s = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), a = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(s), "/*# ".concat(a, " */")),
+                                    var o = (n = i, a = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(a), "/*# ".concat(s, " */")),
                                         d = i.sources.map((function(e) {
                                             return "/*# sourceURL=".concat(i.sourceRoot || "").concat(e, " */")
                                         }));
                                     return [r].concat(d).concat([o]).join("\n")
                                 }
                                 return [r].join("\n")
                             }(t, e);
                             return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                         })).join("")
-                    }, t.i = function(e, n, s) {
+                    }, t.i = function(e, n, a) {
                         "string" == typeof e && (e = [
                             [null, e, ""]
                         ]);
-                        var a = {};
-                        if (s)
+                        var s = {};
+                        if (a)
                             for (var r = 0; r < this.length; r++) {
                                 var i = this[r][0];
-                                null != i && (a[i] = !0)
+                                null != i && (s[i] = !0)
                             }
                         for (var o = 0; o < e.length; o++) {
                             var d = [].concat(e[o]);
-                            s && a[d[0]] || (n && (d[2] ? d[2] = "".concat(n, " and ").concat(d[2]) : d[2] = n), t.push(d))
+                            a && s[d[0]] || (n && (d[2] ? d[2] = "".concat(n, " and ").concat(d[2]) : d[2] = n), t.push(d))
                         }
                     }, t
                 }
             },
             204: (e, t, n) => {
-                var s = n(379),
-                    a = n(889);
-                "string" == typeof(a = a.__esModule ? a.default : a) && (a = [
-                    [e.id, a, ""]
+                var a = n(379),
+                    s = n(889);
+                "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
+                    [e.id, s, ""]
                 ]);
-                s(a, {
+                a(s, {
                     insert: "head",
                     singleton: !1
-                }), e.exports = a.locals || {}
+                }), e.exports = s.locals || {}
             },
             379: (e, t, n) => {
                 "use strict";
-                var s, a = function() {
+                var a, s = function() {
                         var e = {};
                         return function(t) {
                             if (void 0 === e[t]) {
                                 var n = document.querySelector(t);
                                 if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                                     n = n.contentDocument.head
                                 } catch (e) {
@@ -148,210 +150,210 @@
                         if (r[n].identifier === e) {
                             t = n;
                             break
                         } return t
                 }
 
                 function o(e, t) {
-                    for (var n = {}, s = [], a = 0; a < e.length; a++) {
-                        var o = e[a],
+                    for (var n = {}, a = [], s = 0; s < e.length; s++) {
+                        var o = e[s],
                             d = t.base ? o[0] + t.base : o[0],
                             l = n[d] || 0,
                             c = "".concat(d, " ").concat(l);
                         n[d] = l + 1;
                         var u = i(c),
                             p = {
                                 css: o[1],
                                 media: o[2],
                                 sourceMap: o[3]
                             }; - 1 !== u ? (r[u].references++, r[u].updater(p)) : r.push({
                             identifier: c,
-                            updater: _(p, t),
+                            updater: m(p, t),
                             references: 1
-                        }), s.push(c)
+                        }), a.push(c)
                     }
-                    return s
+                    return a
                 }
 
                 function d(e) {
                     var t = document.createElement("style"),
-                        s = e.attributes || {};
-                    if (void 0 === s.nonce) {
+                        a = e.attributes || {};
+                    if (void 0 === a.nonce) {
                         var r = n.nc;
-                        r && (s.nonce = r)
+                        r && (a.nonce = r)
                     }
-                    if (Object.keys(s).forEach((function(e) {
-                            t.setAttribute(e, s[e])
+                    if (Object.keys(a).forEach((function(e) {
+                            t.setAttribute(e, a[e])
                         })), "function" == typeof e.insert) e.insert(t);
                     else {
-                        var i = a(e.insert || "head");
+                        var i = s(e.insert || "head");
                         if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                         i.appendChild(t)
                     }
                     return t
                 }
                 var l, c = (l = [], function(e, t) {
                     return l[e] = t, l.filter(Boolean).join("\n")
                 });
 
-                function u(e, t, n, s) {
-                    var a = n ? "" : s.media ? "@media ".concat(s.media, " {").concat(s.css, "}") : s.css;
-                    if (e.styleSheet) e.styleSheet.cssText = c(t, a);
+                function u(e, t, n, a) {
+                    var s = n ? "" : a.media ? "@media ".concat(a.media, " {").concat(a.css, "}") : a.css;
+                    if (e.styleSheet) e.styleSheet.cssText = c(t, s);
                     else {
-                        var r = document.createTextNode(a),
+                        var r = document.createTextNode(s),
                             i = e.childNodes;
                         i[t] && e.removeChild(i[t]), i.length ? e.insertBefore(r, i[t]) : e.appendChild(r)
                     }
                 }
 
                 function p(e, t, n) {
-                    var s = n.css,
-                        a = n.media,
+                    var a = n.css,
+                        s = n.media,
                         r = n.sourceMap;
-                    if (a ? e.setAttribute("media", a) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = s;
+                    if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = a;
                     else {
                         for (; e.firstChild;) e.removeChild(e.firstChild);
-                        e.appendChild(document.createTextNode(s))
+                        e.appendChild(document.createTextNode(a))
                     }
                 }
                 var f = null,
-                    m = 0;
+                    _ = 0;
 
-                function _(e, t) {
-                    var n, s, a;
+                function m(e, t) {
+                    var n, a, s;
                     if (t.singleton) {
-                        var r = m++;
-                        n = f || (f = d(t)), s = u.bind(null, n, r, !1), a = u.bind(null, n, r, !0)
-                    } else n = d(t), s = p.bind(null, n, t), a = function() {
+                        var r = _++;
+                        n = f || (f = d(t)), a = u.bind(null, n, r, !1), s = u.bind(null, n, r, !0)
+                    } else n = d(t), a = p.bind(null, n, t), s = function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(n)
                     };
-                    return s(e),
+                    return a(e),
                         function(t) {
                             if (t) {
                                 if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                                s(e = t)
-                            } else a()
+                                a(e = t)
+                            } else s()
                         }
                 }
                 e.exports = function(e, t) {
-                    (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === s && (s = Boolean(window && document && document.all && !window.atob)), s));
+                    (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === a && (a = Boolean(window && document && document.all && !window.atob)), a));
                     var n = o(e = e || [], t);
                     return function(e) {
                         if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                            for (var s = 0; s < n.length; s++) {
-                                var a = i(n[s]);
-                                r[a].references--
+                            for (var a = 0; a < n.length; a++) {
+                                var s = i(n[a]);
+                                r[s].references--
                             }
                             for (var d = o(e, t), l = 0; l < n.length; l++) {
                                 var c = i(n[l]);
                                 0 === r[c].references && (r[c].updater(), r.splice(c, 1))
                             }
                             n = d
                         }
                     }
                 }
             },
             112: function(e, t, n) {
                 "use strict";
-                var s = this && this.__createBinding || (Object.create ? function(e, t, n, s) {
-                        void 0 === s && (s = n);
-                        var a = Object.getOwnPropertyDescriptor(t, n);
-                        a && !("get" in a ? !t.__esModule : a.writable || a.configurable) || (a = {
+                var a = this && this.__createBinding || (Object.create ? function(e, t, n, a) {
+                        void 0 === a && (a = n);
+                        var s = Object.getOwnPropertyDescriptor(t, n);
+                        s && !("get" in s ? !t.__esModule : s.writable || s.configurable) || (s = {
                             enumerable: !0,
                             get: function() {
                                 return t[n]
                             }
-                        }), Object.defineProperty(e, s, a)
-                    } : function(e, t, n, s) {
-                        void 0 === s && (s = n), e[s] = t[n]
+                        }), Object.defineProperty(e, a, s)
+                    } : function(e, t, n, a) {
+                        void 0 === a && (a = n), e[a] = t[n]
                     }),
-                    a = this && this.__exportStar || function(e, t) {
-                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || s(t, e, n)
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || a(t, e, n)
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), window.__webpack_public_path__ = `${document.querySelector("body").getAttribute("data-base-url")}nbextensions/unfolded/map_sdk`, a(n(607), t)
+                }), window.__webpack_public_path__ = `${document.querySelector("body").getAttribute("data-base-url")}nbextensions/unfolded/map_sdk`, s(n(607), t)
             },
             607: function(e, t, n) {
                 "use strict";
-                var s = this && this.__createBinding || (Object.create ? function(e, t, n, s) {
-                        void 0 === s && (s = n);
-                        var a = Object.getOwnPropertyDescriptor(t, n);
-                        a && !("get" in a ? !t.__esModule : a.writable || a.configurable) || (a = {
+                var a = this && this.__createBinding || (Object.create ? function(e, t, n, a) {
+                        void 0 === a && (a = n);
+                        var s = Object.getOwnPropertyDescriptor(t, n);
+                        s && !("get" in s ? !t.__esModule : s.writable || s.configurable) || (s = {
                             enumerable: !0,
                             get: function() {
                                 return t[n]
                             }
-                        }), Object.defineProperty(e, s, a)
-                    } : function(e, t, n, s) {
-                        void 0 === s && (s = n), e[s] = t[n]
+                        }), Object.defineProperty(e, a, s)
+                    } : function(e, t, n, a) {
+                        void 0 === a && (a = n), e[a] = t[n]
                     }),
-                    a = this && this.__exportStar || function(e, t) {
-                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || s(t, e, n)
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || a(t, e, n)
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), a(n(412), t), a(n(862), t), a(n(467), t)
+                }), s(n(412), t), s(n(862), t), s(n(467), t)
             },
             944: function(e, t, n) {
                 "use strict";
-                var s = this && this.__awaiter || function(e, t, n, s) {
-                    return new(n || (n = Promise))((function(a, r) {
+                var a = this && this.__awaiter || function(e, t, n, a) {
+                    return new(n || (n = Promise))((function(s, r) {
                         function i(e) {
                             try {
-                                d(s.next(e))
+                                d(a.next(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function o(e) {
                             try {
-                                d(s.throw(e))
+                                d(a.throw(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function d(e) {
                             var t;
-                            e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                            e.done ? s(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(i, o)
                         }
-                        d((s = s.apply(e, t || [])).next())
+                        d((a = a.apply(e, t || [])).next())
                     }))
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 });
-                const a = n(855);
+                const s = n(855);
                 var r;
                 ! function(e) {
                     e.EVENT = "event", e.SUCCESS = "response", e.ERROR = "error"
                 }(r || (r = {})), t.default = class {
                     constructor(e) {
                         this.queue = new Array, this.mapReady = !1, this.destroyed = !1, this.finalize = () => {
                             this.destroyed = !0, this.model.off("msg:custom", this.messageReceived), this.model.stopListening(this.model, "destroy", this.finalize);
                             const e = this.model.map();
                             e && (e.eventHandlers = {})
                         }, this.enableCallbacks = (e, t) => {
                             const n = [];
                             for (const e of t)
-                                if ((0, a.isEventType)(e)) {
-                                    const t = a.eventNamesMap[e];
+                                if ((0, s.isEventType)(e)) {
+                                    const t = s.eventNamesMap[e];
                                     n.push(t)
-                                } const s = {};
-                            for (const e of n) s[e] = t => this.sendCallbackEventToJupyter(a.reverseEventNamesMap[e], t);
-                            e.eventHandlers = Object.assign(Object.assign({}, e.eventHandlers), s)
+                                } const a = {};
+                            for (const e of n) a[e] = t => this.sendCallbackEventToJupyter(s.reverseEventNamesMap[e], t);
+                            e.eventHandlers = Object.assign(Object.assign({}, e.eventHandlers), a)
                         }, this.disableCallbacks = (e, t) => {
-                            for (const n of t) delete e.eventHandlers[a.eventNamesMap[n]]
+                            for (const n of t) delete e.eventHandlers[s.eventNamesMap[n]]
                         }, this.messageReceived = e => {
                             this.destroyed || (this.mapReady ? this.callSDKFunction(e) : this.queue.push(e))
                         }, this.sendResponseToJupyter = (e, t = null) => {
                             if (this.destroyed) return;
                             const n = {
                                 type: r.SUCCESS,
                                 messageId: e,
@@ -375,52 +377,52 @@
                             this.model.send(n, [])
                         }, this.model = e, this.model.on("msg:custom", this.messageReceived), this.model.listenTo(this.model, "destroy", this.finalize)
                     }
                     setMapReady(e) {
                         if (this.mapReady = e, this.mapReady) {
                             let e;
                             for (; void 0 !== (e = this.queue.shift());) this.callSDKFunction(e);
-                            this.sendCallbackEventToJupyter(a.ExtraEventType.ON_LOAD, {})
+                            this.sendCallbackEventToJupyter(s.ExtraEventType.ON_LOAD, {})
                         }
                     }
                     callSDKFunction(e) {
-                        return s(this, void 0, void 0, (function*() {
+                        return a(this, void 0, void 0, (function*() {
                             const {
                                 messageId: t,
                                 type: n,
-                                args: s,
+                                args: a,
                                 options: r
                             } = e, i = this.model.map();
                             if (!i) throw new Error("Cannot call functions before map is rendered");
                             try {
-                                if (n === a.ExtraActionType.SET_EVENT_HANDLERS) return this.enableCallbacks(i, s[0]), this.sendResponseToJupyter(t);
-                                if (n === a.ExtraActionType.REMOVE_EVENT_HANDLERS) return this.disableCallbacks(i, s[0]), this.sendResponseToJupyter(t); {
-                                    const e = a.funcNamesMap[n];
+                                if (n === s.ExtraActionType.SET_EVENT_HANDLERS) return this.enableCallbacks(i, a[0]), this.sendResponseToJupyter(t);
+                                if (n === s.ExtraActionType.REMOVE_EVENT_HANDLERS) return this.disableCallbacks(i, a[0]), this.sendResponseToJupyter(t); {
+                                    const e = s.funcNamesMap[n];
                                     if ("function" == typeof i[e]) {
-                                        const n = yield i[e](...s, r);
+                                        const n = yield i[e](...a, r);
                                         return this.sendResponseToJupyter(t, n)
                                     }
                                 }
                                 throw new Error(`Function ${n} not found`)
                             } catch (e) {
                                 e instanceof Error && this.sendErrorToJupyter(t, e)
                             }
                         }))
                     }
                 }
             },
             855: (e, t) => {
                 "use strict";
-                var n, s, a;
+                var n, a, s;
                 Object.defineProperty(t, "__esModule", {
                         value: !0
                     }), t.isEventType = t.reverseEventNamesMap = t.eventNamesMap = t.ExtraEventType = t.EventType = t.funcNamesMap = t.ExtraActionType = t.ActionType = void 0,
                     function(e) {
                         e.GET_VIEW = "v1/map-sdk-get-view", e.SET_VIEW = "v1/map-sdk-set-view", e.GET_VIEW_LIMITS = "v1/map-sdk-get-view-limits", e.SET_VIEW_LIMITS = "v1/map-sdk-set-view-limits", e.GET_MAP_CONTROL_VISIBILITY = "v1/map-sdk-get-map-control-visibility", e.SET_MAP_CONTROL_VISIBILITY = "v1/map-sdk-set-map-control-visibility", e.GET_SPLIT_MODE = "v1/map-sdk-get-split-mode", e.SET_SPLIT_MODE = "v1/map-sdk-set-split-mode", e.SET_THEME = "v1/map-set-theme", e.GET_MAP_CONFIG = "v1/map-sdk-get-map-config", e.SET_MAP_CONFIG = "v1/map-sdk-set-map-config", e.GET_MAP_STYLES = "v1/map-sdk-get-map-styles", e.GET_FILTERS = "v1/map-sdk-get-filters", e.GET_FILTER_BY_ID = "v1/map-sdk-get-filter-by-id", e.ADD_FILTER = "v1/map-sdk-add-filter", e.UPDATE_FILTER = "v1/map-sdk-update-filter", e.REMOVE_FILTER = "v1/map-sdk-remove-filter", e.UPDATE_TIMELINE = "v1/map-sdk-update-timeline", e.GET_DATASETS = "v1/map-sdk-get-datasets", e.GET_DATASET_BY_ID = "v1/map-sdk-get-dataset-by-id", e.ADD_DATASET = "v1/map-sdk-add-dataset", e.ADD_TILE_DATASET = "v1/map-sdk-add-tile-dataset", e.UPDATE_DATASET = "v1/map-sdk-update-dataset", e.REMOVE_DATASET = "v1/map-sdk-remove-dataset", e.REPLACE_DATASET = "v1/map-sdk-replace-dataset", e.GET_DATASET_WITH_DATA = "v1/map-sdk-get-dataset-with-data", e.GET_LAYERS = "v1/map-sdk-get-layers", e.GET_LAYER_BY_ID = "v1/map-sdk-get-layer-by-id", e.ADD_LAYER = "v1/map-sdk-add-layer", e.UPDATE_LAYER = "v1/map-sdk-update-layer", e.REMOVE_LAYER = "v1/map-sdk-remove-layer", e.GET_LAYER_GROUPS = "v1/map-sdk-get-layer-groups", e.GET_LAYER_GROUP_BY_ID = "v1/map-sdk-get-layer-group-by-id", e.ADD_LAYER_GROUP = "v1/map-sdk-add-layer-group", e.UPDATE_LAYER_GROUP = "v1/map-sdk-update-layer-group", e.REMOVE_LAYER_GROUP = "v1/map-sdk-remove-layer-group", e.GET_LAYER_TIMELINE = "v1/map-sdk-get-layer-timeline", e.UPDATE_LAYER_TIMELINE = "v1/map-sdk-update-layer-timeline"
-                    }(n = t.ActionType || (t.ActionType = {})), (a = t.ExtraActionType || (t.ExtraActionType = {})).SET_EVENT_HANDLERS = "v1/map-sdk-set-event-handlers", a.REMOVE_EVENT_HANDLERS = "v1/map-sdk-remove-event-handlers", t.funcNamesMap = {
+                    }(n = t.ActionType || (t.ActionType = {})), (s = t.ExtraActionType || (t.ExtraActionType = {})).SET_EVENT_HANDLERS = "v1/map-sdk-set-event-handlers", s.REMOVE_EVENT_HANDLERS = "v1/map-sdk-remove-event-handlers", t.funcNamesMap = {
                         [n.GET_VIEW]: "getView",
                         [n.SET_VIEW]: "setView",
                         [n.GET_VIEW_LIMITS]: "getViewLimits",
                         [n.SET_VIEW_LIMITS]: "setViewLimits",
                         [n.GET_MAP_CONTROL_VISIBILITY]: "getMapControlVisibility",
                         [n.SET_MAP_CONTROL_VISIBILITY]: "setMapControlVisibility",
                         [n.GET_SPLIT_MODE]: "getSplitMode",
@@ -454,47 +456,47 @@
                         [n.UPDATE_LAYER_GROUP]: "updateLayerGroup",
                         [n.REMOVE_LAYER_GROUP]: "removeLayerGroup",
                         [n.GET_LAYER_TIMELINE]: "getLayerTimeline",
                         [n.UPDATE_LAYER_TIMELINE]: "updateLayerTimeline"
                     },
                     function(e) {
                         e.ON_CLICK = "v1/map-sdk-on-click", e.ON_HOVER = "v1/map-sdk-on-hover", e.ON_VIEW_UPDATE = "v1/map-sdk-on-view-update", e.ON_GEOMETRY_SELECTION = "v1/map-sdk-on-geometry-selection", e.ON_LAYER_TIMELINE_UPDATE = "v1/map-sdk-on-layer-timeline-update", e.ON_FILTER_UPDATE = "v1/map-sdk-on-filter-update"
-                    }(s = t.EventType || (t.EventType = {})), (t.ExtraEventType || (t.ExtraEventType = {})).ON_LOAD = "v1/map-sdk-on-load", t.eventNamesMap = {
-                        [s.ON_CLICK]: "onClick",
-                        [s.ON_HOVER]: "onHover",
-                        [s.ON_VIEW_UPDATE]: "onViewUpdate",
-                        [s.ON_GEOMETRY_SELECTION]: "onGeometrySelection",
-                        [s.ON_LAYER_TIMELINE_UPDATE]: "onLayerTimelineUpdate",
-                        [s.ON_FILTER_UPDATE]: "onFilterUpdate"
+                    }(a = t.EventType || (t.EventType = {})), (t.ExtraEventType || (t.ExtraEventType = {})).ON_LOAD = "v1/map-sdk-on-load", t.eventNamesMap = {
+                        [a.ON_CLICK]: "onClick",
+                        [a.ON_HOVER]: "onHover",
+                        [a.ON_VIEW_UPDATE]: "onViewUpdate",
+                        [a.ON_GEOMETRY_SELECTION]: "onGeometrySelection",
+                        [a.ON_LAYER_TIMELINE_UPDATE]: "onLayerTimelineUpdate",
+                        [a.ON_FILTER_UPDATE]: "onFilterUpdate"
                     }, t.reverseEventNamesMap = Object.entries(t.eventNamesMap).reduce(((e, [t, n]) => (e[n] = t, e)), {}), t.isEventType = function(e) {
-                        return Object.values(s).includes(e)
+                        return Object.values(a).includes(e)
                     }
             },
             412: (e, t, n) => {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-                const s = n(147);
-                t.MODULE_VERSION = s.version, t.MODULE_NAME = s.name
+                const a = n(147);
+                t.MODULE_VERSION = a.version, t.MODULE_NAME = a.name
             },
             862: function(e, t, n) {
                 "use strict";
-                var s = this && this.__importDefault || function(e) {
+                var a = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.UnfoldedMapModel = void 0;
-                const a = n(146),
-                    r = s(n(944)),
+                const s = n(146),
+                    r = a(n(944)),
                     i = n(412);
-                class o extends a.DOMWidgetModel {
+                class o extends s.DOMWidgetModel {
                     constructor() {
                         super(...arguments), this.transport = new r.default(this)
                     }
                     defaults() {
                         return Object.assign(Object.assign({}, super.defaults()), {
                             _model_name: o.model_name,
                             _model_module: o.model_module,
@@ -527,55 +529,55 @@
                         const e = this.get("urls");
                         return this.objectOrUndefined(e)
                     }
                     _internal() {
                         return this.get("_internal")
                     }
                 }
-                o.serializers = Object.assign({}, a.DOMWidgetModel.serializers), o.model_name = "UnfoldedMapModel", o.model_module = i.MODULE_NAME, o.model_module_version = i.MODULE_VERSION, o.view_name = "UnfoldedMapView", o.view_module = i.MODULE_NAME, o.view_module_version = i.MODULE_VERSION, t.UnfoldedMapModel = o
+                o.serializers = Object.assign({}, s.DOMWidgetModel.serializers), o.model_name = "UnfoldedMapModel", o.model_module = i.MODULE_NAME, o.model_module_version = i.MODULE_VERSION, o.view_name = "UnfoldedMapView", o.view_module = i.MODULE_NAME, o.view_module_version = i.MODULE_VERSION, t.UnfoldedMapModel = o
             },
             467: function(e, t, n) {
                 "use strict";
-                var s = this && this.__awaiter || function(e, t, n, s) {
-                    return new(n || (n = Promise))((function(a, r) {
+                var a = this && this.__awaiter || function(e, t, n, a) {
+                    return new(n || (n = Promise))((function(s, r) {
                         function i(e) {
                             try {
-                                d(s.next(e))
+                                d(a.next(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function o(e) {
                             try {
-                                d(s.throw(e))
+                                d(a.throw(e))
                             } catch (e) {
                                 r(e)
                             }
                         }
 
                         function d(e) {
                             var t;
-                            e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                            e.done ? s(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(i, o)
                         }
-                        d((s = s.apply(e, t || [])).next())
+                        d((a = a.apply(e, t || [])).next())
                     }))
                 };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.UnfoldedMapView = void 0;
-                const a = n(146),
+                const s = n(146),
                     r = n(848);
                 n(204);
                 const i = "unfolded-widget";
-                class o extends a.DOMWidgetView {
+                class o extends s.DOMWidgetView {
                     initialize() {
-                        return s(this, void 0, void 0, (function*() {
+                        return a(this, void 0, void 0, (function*() {
                             const e = {
                                 style: this.model.style(),
                                 basemaps: this.model.basemaps(),
                                 raster: this.model.raster(),
                                 urls: this.model.urls()
                             };
                             if (!this.model.map()) {
@@ -595,34 +597,34 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.7.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . > ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.7.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@babel/core":"^7.16.0","@babel/preset-env":"^7.16.0","@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
+                e.exports = JSON.parse('{"name":"@unfolded/jupyter-map-sdk","version":"1.8.0","description":"JavaScript bindings for Unfolded\'s Jupyter Map SDK","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"license":"(c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/","author":{"name":"Foursquare Labs","email":"info-studio@foursquare.com"},"main":"lib/index.js","types":"lib/index.d.ts","scripts":{"start":"yarn run watch","build":"yarn run clean && yarn run build:lib && yarn run build:nbextension:dev && yarn run build:labextension:dev","build:prod":"yarn run clean && yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"yarn run -T tsc && rimraf lib/__tests__","build:nbextension":"webpack --mode production","build:nbextension:dev":"webpack --mode development","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf unfolded/map_sdk/labextension","clean:nbextension":"rimraf \'unfolded/map_sdk/nbextension/index.js*\'","lint":"eslint --max-warnings 0 src","typecheck":"tsc","prepack":"yarn run build:prod","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"yarn run -T tsc -w","watch:nbextension":"webpack --watch --mode development","typescript":"yarn run -T tsc --noEmit","generate-licenses":"node -r esbuild-register ../../../scripts/get-licenses.ts -p . -o ./dist/LICENSES.md"},"dependencies":{"@aws-amplify/core":"^4.2.9","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","@jupyterlab/rendermime-interfaces":"^1.3.0 || ^2.0.0 || ^3.0.0","@lumino/application":"^1.16.0","@lumino/widgets":"^1.30.0","@unfolded/map-sdk":"^1.8.0","aws-sdk":"^2.988.0","csstype":"^3.1.0","global":"^4.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","css-loader":"^3.2.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","npm-run-all":"^4.1.3","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^9.3.1","webpack":"^5.64.1","webpack-cli":"^4.9.1"},"jupyterlab":{"extension":"lib/plugin","outputDir":"unfolded/map_sdk/labextension/","mimeExtension":"lib/javascript-renderer-extension.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"volta":{"extends":"../../../package.json"}}')
             }
         },
         n = {};
 
-    function s(e) {
-        var a = n[e];
-        if (void 0 !== a) return a.exports;
+    function a(e) {
+        var s = n[e];
+        if (void 0 !== s) return s.exports;
         var r = n[e] = {
             id: e,
             exports: {}
         };
-        return t[e].call(r.exports, r, r.exports, s), r.exports
+        return t[e].call(r.exports, r, r.exports, a), r.exports
     }
-    return s.d = (e, t) => {
-        for (var n in t) s.o(t, n) && !s.o(e, n) && Object.defineProperty(e, n, {
+    return a.d = (e, t) => {
+        for (var n in t) a.o(t, n) && !a.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
-    }, s.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), s.r = e => {
+    }, a.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), a.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, s(112)
+    }, a(112)
 })()));
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/poll.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/poll.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/templates/html_map_sdk.j2` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/templates/html_map_sdk.j2`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/transfer_utils.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/transfer_utils.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/base.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/base.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/html.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/html.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/transport/widget.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/transport/widget.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/types.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/types.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/action_type_mapping.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/action_type_mapping.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/encoders.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/serialization.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded/map_sdk/utils/validators.py` & `unfolded.map-sdk-1.8.0/unfolded/map_sdk/utils/validators.py`

 * *Files identical despite different names*

### Comparing `unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/PKG-INFO` & `unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfolded.map-sdk
-Version: 1.7.0
+Version: 1.8.0
 Summary: Jupyter Widget for Foursquare Studio Maps
 Author: Foursquare Labs
 Author-email: info-studio@foursquare.com
 License: (c) 2022 Foursquare Labs, Inc. Terms available at https://location.foursquare.com/legal/terms/foursquarestudio-terms-of-service/
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `unfolded.map-sdk-1.7.0/unfolded.map_sdk.egg-info/SOURCES.txt` & `unfolded.map-sdk-1.8.0/unfolded.map_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 unfolded/map_sdk/api/dataset_api.py
 unfolded/map_sdk/api/enums.py
 unfolded/map_sdk/api/event_api.py
 unfolded/map_sdk/api/filter_api.py
 unfolded/map_sdk/api/layer_api.py
 unfolded/map_sdk/api/map_api.py
 unfolded/map_sdk/labextension/package.json
-unfolded/map_sdk/labextension/static/4.1d6b2ee6b4adaa5011d0.js
-unfolded/map_sdk/labextension/static/480.07947b701030e20bd6a5.js
-unfolded/map_sdk/labextension/static/568.c4c2c97499e36629de31.js
-unfolded/map_sdk/labextension/static/747.52c1033b21b19cfefa35.js
-unfolded/map_sdk/labextension/static/remoteEntry.fd6179891fa0411b63ce.js
+unfolded/map_sdk/labextension/static/4.73406aceb9bb0a52322f.js
+unfolded/map_sdk/labextension/static/480.f1b7298a86c01bc22dff.js
+unfolded/map_sdk/labextension/static/568.60f49bd7c7010d71ba45.js
+unfolded/map_sdk/labextension/static/747.488cf0ee36d815959581.js
+unfolded/map_sdk/labextension/static/remoteEntry.39a2d353490d0e44cd24.js
 unfolded/map_sdk/labextension/static/style.js
 unfolded/map_sdk/labextension/static/third-party-licenses.json
 unfolded/map_sdk/map/__init__.py
 unfolded/map_sdk/map/base.py
 unfolded/map_sdk/map/html.py
 unfolded/map_sdk/map/widget.py
 unfolded/map_sdk/nbextension/extension.js
```

### Comparing `unfolded.map-sdk-1.7.0/webpack.config.js` & `unfolded.map-sdk-1.8.0/webpack.config.js`

 * *Files identical despite different names*

