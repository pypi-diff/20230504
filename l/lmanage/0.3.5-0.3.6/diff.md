# Comparing `tmp/lmanage-0.3.5.tar.gz` & `tmp/lmanage-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmanage-0.3.5.tar", last modified: Wed Mar 29 22:51:30 2023, max compression
+gzip compressed data, was "lmanage-0.3.6.tar", max compression
```

## Comparing `lmanage-0.3.5.tar` & `lmanage-0.3.6.tar`

### file list

```diff
@@ -1,58 +1,63 @@
--rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.5/LICENSE
--rw-r--r--   0        0        0     3855 2023-02-07 18:38:42.538476 lmanage-0.3.5/README.md
--rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.5/lmanage/.vimspector.json
--rw-r--r--   0        0        0    36566 2022-12-15 21:59:31.550793 lmanage-0.3.5/lmanage/None
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/__init__.py
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/__init__.py
--rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/commands.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/folder_capturation/__init__.py
--rw-r--r--   0        0        0     1460 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
--rw-r--r--   0        0        0     6596 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/folder_capturation/folder_config.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_attribute_capturation/__init__.py
--rw-r--r--   0        0        0     2734 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_group_capturation/__init__.py
--rw-r--r--   0        0        0     3565 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_group_capturation/group_config.py
--rw-r--r--   0        0        0     3108 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_group_capturation/role_config.py
--rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capturator/user_group_capturation/user_permission.py
--rw-r--r--   0        0        0     3707 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/capture_instance_permission_structure.py
--rw-r--r--   0        0        0      928 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/cli.py
--rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.5/lmanage/configurator/.vimspector.json
--rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/__init__.py
--rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/commands.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/folder_configuration/__init__.py
--rw-r--r--   0        0        0    13776 2023-03-25 01:11:40.264096 lmanage-0.3.5/lmanage/configurator/folder_configuration/create_folder_permissions.py
--rw-r--r--   0        0        0     5167 2023-03-29 22:49:29.111961 lmanage-0.3.5/lmanage/configurator/folder_configuration/create_folders.py
--rw-r--r--   0        0        0     1616 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/folder_configuration/folder_config.py
--rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.5/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/user_attribute_configuration/__init__.py
--rw-r--r--   0        0        0     3774 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
--rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/configurator/user_group_configuration/__init__.py
--rw-r--r--   0        0        0     4346 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/configurator/user_group_configuration/group_config.py
--rw-r--r--   0        0        0     5801 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/configurator/user_group_configuration/role_config.py
--rw-r--r--   0        0        0     4484 2023-03-23 16:57:22.195458 lmanage-0.3.5/lmanage/configurator/user_group_configuration/user_permission.py
--rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.5/lmanage/find_replace.sh
--rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.5/lmanage/mapview/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/__init__.py
--rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/mapview/compare_content_to_lookml.py
--rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.5/lmanage/mapview/hugo.csv
--rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/instancedata.py
--rw-r--r--   0        0        0    14973 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/legacy_get_content_with_views.py
--rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/main.py
--rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/mapexplores.py
--rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/mapview/mapview_execute.py
--rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/matched_field_analysis.py
--rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.5/lmanage/mapview/pandas_multiple.xlsx
--rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/parse_sql_tables.py
--rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.5/lmanage/mapview/utils/.vimspector.json
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/utils/__init__.py
--rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/utils/create_df.py
--rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/utils/parse_lookml.py
--rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.5/lmanage/mapview/utils/parsing_sql.py
--rw-r--r--   0        0        0     3991 2023-03-29 22:49:29.111961 lmanage-0.3.5/lmanage/provision_instance_permission_structure.py
--rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/utils/__init__.py
--rw-r--r--   0        0        0      835 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/utils/errorhandling.py
--rw-r--r--   0        0        0     1253 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/utils/looker_object_constructors.py
--rw-r--r--   0        0        0     1597 2023-03-23 16:57:22.191458 lmanage-0.3.5/lmanage/utils/parse_yaml.py
--rw-r--r--   0        0        0     1165 2023-03-29 22:49:51.313995 lmanage-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5811 2023-03-29 22:51:30.237790 lmanage-0.3.5/setup.py
--rw-r--r--   0        0        0     5356 2023-03-29 22:51:30.238498 lmanage-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-07-16 17:02:14.912118 lmanage-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2695 2023-04-27 21:32:50.653908 lmanage-0.3.6/README.md
+-rw-r--r--   0        0        0      926 2022-12-15 21:59:31.502790 lmanage-0.3.6/lmanage/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/__init__.py
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/__init__.py
+-rw-r--r--   0        0        0     2063 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/capturator/content_capturation/__init__.py
+-rw-r--r--   0        0        0     2406 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/content_capturation/dashboard_capture.py
+-rw-r--r--   0        0        0     3227 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/content_capturation/look_capture.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/folder_capturation/__init__.py
+-rw-r--r--   0        0        0     1136 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/capturator/folder_capturation/create_folder_yaml_structure.py
+-rw-r--r--   0        0        0     8063 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/folder_capturation/folder_config.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/__init__.py
+-rw-r--r--   0        0        0     2341 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_group_capturation/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/capturator/user_group_capturation/group_config.py
+-rw-r--r--   0        0        0     2923 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/capturator/user_group_capturation/role_config.py
+-rw-r--r--   0        0        0     3765 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/capturator/user_group_capturation/user_permission.py
+-rw-r--r--   0        0        0     4715 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/capture_instance_permission_structure.py
+-rw-r--r--   0        0        0      928 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/cli.py
+-rw-r--r--   0        0        0      353 2022-06-24 18:34:27.402555 lmanage-0.3.6/lmanage/configurator/.vimspector.json
+-rw-r--r--   0        0        0      598 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/__init__.py
+-rw-r--r--   0        0        0     2026 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/commands.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/configurator/content_configuration/__init__.py
+-rw-r--r--   0        0        0     2167 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_content_prep.py
+-rw-r--r--   0        0        0     1045 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_dashboards.py
+-rw-r--r--   0        0        0     4072 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/configurator/content_configuration/create_looks.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/folder_configuration/__init__.py
+-rw-r--r--   0        0        0    13653 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folder_permissions.py
+-rw-r--r--   0        0        0     5786 2023-04-19 21:34:25.230519 lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folders.py
+-rw-r--r--   0        0        0     1615 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/configurator/folder_configuration/folder_config.py
+-rw-r--r--   0        0        0     5706 2023-02-07 21:50:06.720732 lmanage-0.3.6/lmanage/configurator/instance_configuration_settings/fullinstance.yaml
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/__init__.py
+-rw-r--r--   0        0        0     4072 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py
+-rw-r--r--   0        0        0        0 2023-03-23 16:57:22.195458 lmanage-0.3.6/lmanage/configurator/user_group_configuration/__init__.py
+-rw-r--r--   0        0        0     4420 2023-04-26 23:16:43.844504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/group_config.py
+-rw-r--r--   0        0        0     5978 2023-04-26 23:16:43.848504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/role_config.py
+-rw-r--r--   0        0        0     4727 2023-04-26 23:16:43.848504 lmanage-0.3.6/lmanage/configurator/user_group_configuration/user_permission.py
+-rwxr-xr-x   0        0        0      702 2022-12-15 21:59:31.634799 lmanage-0.3.6/lmanage/find_replace.sh
+-rw-r--r--   0        0        0      446 2022-06-24 18:34:27.574567 lmanage-0.3.6/lmanage/mapview/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/__init__.py
+-rw-r--r--   0        0        0     3645 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/mapview/compare_content_to_lookml.py
+-rw-r--r--   0        0        0     1873 2022-06-24 18:34:27.602569 lmanage-0.3.6/lmanage/mapview/hugo.csv
+-rw-r--r--   0        0        0     2092 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/instancedata.py
+-rw-r--r--   0        0        0    14973 2023-04-26 23:16:43.868505 lmanage-0.3.6/lmanage/mapview/legacy_get_content_with_views.py
+-rw-r--r--   0        0        0     1633 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/main.py
+-rw-r--r--   0        0        0     2773 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/mapexplores.py
+-rw-r--r--   0        0        0     1503 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/mapview/mapview_execute.py
+-rw-r--r--   0        0        0     2182 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/matched_field_analysis.py
+-rw-r--r--   0        0        0     7197 2022-06-24 18:34:27.694576 lmanage-0.3.6/lmanage/mapview/pandas_multiple.xlsx
+-rw-r--r--   0        0        0     2881 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/parse_sql_tables.py
+-rw-r--r--   0        0        0      324 2022-06-24 18:34:27.714578 lmanage-0.3.6/lmanage/mapview/utils/.vimspector.json
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/__init__.py
+-rw-r--r--   0        0        0     1234 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/create_df.py
+-rw-r--r--   0        0        0     3046 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/parse_lookml.py
+-rw-r--r--   0        0        0     5008 2023-03-23 16:57:22.187458 lmanage-0.3.6/lmanage/mapview/utils/parsing_sql.py
+-rw-r--r--   0        0        0     6375 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/provision_instance_permission_structure.py
+-rw-r--r--   0        0        0      575 2023-03-23 16:57:22.191458 lmanage-0.3.6/lmanage/utils/__init__.py
+-rw-r--r--   0        0        0     1662 2023-04-26 23:19:51.736692 lmanage-0.3.6/lmanage/utils/errorhandling.py
+-rw-r--r--   0        0        0     2643 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/utils/looker_object_constructors.py
+-rw-r--r--   0        0        0     2027 2023-04-19 21:34:25.234519 lmanage-0.3.6/lmanage/utils/parse_yaml.py
+-rw-r--r--   0        0        0     1029 2023-04-26 23:19:51.748692 lmanage-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 lmanage-0.3.6/PKG-INFO
```

### Comparing `lmanage-0.3.5/LICENSE` & `lmanage-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/README.md` & `lmanage-0.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,73 @@
-# Lmanage
+Metadata-Version: 2.1
+Name: lmanage
+Version: 0.3.6
+Summary: LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML.
+Home-page: https://github.com/looker-open-source/lmanage
+Keywords: keyword,another_keyword
+Author: hselbie
+Author-email: hselbie@gmail.com
+Requires-Python: >=3.8,<3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
+Requires-Dist: autopep8 (>=1.6.0,<2.0.0)
+Requires-Dist: click (>=7.1.2,<8.0.0)
+Requires-Dist: coloredlogger (>=1.3.12,<2.0.0)
+Requires-Dist: coloredlogs (>=15.0,<16.0)
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: ipython (>=7.20.0,<8.0.0)
+Requires-Dist: lkml (>=1.1.1,<2.0.0)
+Requires-Dist: looker-sdk (>=22.4.0,<23.0.0)
+Requires-Dist: pylint (>=2.9.5,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
+Requires-Dist: tabulate (>=0.8.8,<0.9.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: verboselogs (>=1.7,<2.0)
+Requires-Dist: yaspin (>=2.3.0,<3.0.0)
+Project-URL: Repository, https://github.com/looker-open-source/lmanage
+Description-Content-Type: text/markdown
+
+# LManage
 ## What is it.
 LManage is a collection of useful tools for [Looker](https://looker.com/) admins to help curate and cleanup content and it's associated source [LookML](https://docs.looker.com/data-modeling/learning-lookml/what-is-lookml).
 
 ## How do i Install it.
 Lmanage can be found on [pypi](#).
 ```
 pip install lmanage
 ```
 
 ## How do I Use it.
 ### Commands
 LManage will ultimately will have many different commands as development continues 
 | Status  | Command    | Rationale                                                                                                                                                                                            |
 |---------|------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Live    | [mapview](https://github.com/looker-open-source/lmanage/tree/main/instructions/mapview_README.md) | Find the LookML fields and tables that are associated with a piece of Looker content                          |
-| Live    | [capturator](https://github.com/looker-open-source/lmanage/tree/main/instructions/looker_settings_capture.md)| Capture your Looker Instance Group, Folder, Role and User Attributes into a Yaml based Config File |
-| Live    | [configurator](https://github.com/looker-open-source/lmanage/tree/main/instructions/looker_settings_capture.md)| Configure your Looker Instance Group, Folder, Role and User Attributes via a Yaml based Config File |
-| Planned | removeuser | Based on last time logged in, prune Looker users to ensure a performant, compliant Looker instance                                                                                                   |
-| Planned | dcontent   | Iterate through an input of content, delete content and back it up using [gzr](https://github.com/looker-open-source/gzr) for easy restoration                                                                                               |
-| Planned | bcontent   | Iterate through all broken content (using content validator) and email a customized message to each dashboard owner                                                                                  |
+| Live | Object Migrator Tool | Migrate Looker Objects such as Content, Folders and Permissions, User Groups, Roles and Attributes between a Looker Instance or for Version Control [instructions](https://github.com/looker-open-source/lmanage/tree/main/instructions/looker_settings_capture.md)                                                                                                |
 | Planned | scoper     | Takes in a model file, elminates the * includes, iterate through the explores and joins and creates a fully scoped model include list for validation performance and best practice code organization |
+| Planned | removeuser | Based on last time logged in, prune Looker users to ensure a performant, compliant Looker instance                                                                                                   |
+| Planned | [mapview](https://github.com/looker-open-source/lmanage/tree/main/instructions/mapview_README.md) | Find the LookML fields and tables that are associated with a piece of Looker content                          |
 
 #### help and version
 ```
 lmanage --help
 Usage: lmanage [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --version  Show the version and exit.
   --help     Show this message and exit.
 
 Commands:
-  mapview
   capturator
   configurator
 ```
-#### mapview
-The mapview command will find the etymology of the content on your dashboard, exporting a CSV that looks like [this](https://docs.google.com/spreadsheets/d/1TzeJW46ml0uzO9RdLOOLxwtvUWjhmZxoa-xq4pbznV0/edit?resourcekey=0-xbWC87hXYFNgy1As06NncA#gid=900312158).
-
-[instructions](https://github.com/looker-open-source/lmanage/tree/main/instructions/mapview_README.md)
-
-#### configurator
-The configurator command will allow you to manage your Looker security and access settings from a simple text based Yaml file. This file can be version controlled and productionalized using a gitops workflow.
-
-[instructions](https://github.com/looker-open-source/lmanage/tree/main/instructions/looker_settings_capture.md)
-
-#### capturator
-The capturator command will allow you to restore your Looker security and access settings from a simple text based Yaml file. This file can be version controlled and productionalized using a gitops workflow.
+#### Looker Object Migrator
+The object migrator allows you to preserve a point in time representation of your Looker content (Looks and Dashboards), Folder structure, Content access settings, User groups, User roles, User Attributes and preserve these as a Yaml file. This tool then lets you configure a new instance based on that Yaml file.
 
 [instructions](https://github.com/looker-open-source/lmanage/tree/main/instructions/looker_settings_capture.md)
 
 
 **This is not an officially supported Google Product.**
+
```

### Comparing `lmanage-0.3.5/lmanage/.vimspector.json` & `lmanage-0.3.6/lmanage/.vimspector.json`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/__init__.py` & `lmanage-0.3.6/lmanage/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/capturator/__init__.py` & `lmanage-0.3.6/lmanage/capturator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/capturator/commands.py` & `lmanage-0.3.6/lmanage/capturator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/capturator/folder_capturation/folder_config.py` & `lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folders.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,151 @@
 import logging
+from looker_sdk import models, error
 import coloredlogs
-from lmanage.utils import looker_object_constructors as loc
-from lmanage.utils.errorhandling import return_sleep_message
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
-coloredlogs.install(level='DEBUG')
+coloredlogs.install(level='INFO')
 logging.getLogger("requests").setLevel(logging.WARNING)
 
 
-class CaptureFolderConfig():
-    ''' Class to read in folder metadata and unested_folder_data '''
-
-    def __init__(self, sdk):
+class CreateInstanceFolders():
+    def __init__(self, folder_metadata, sdk):
         self.sdk = sdk
+        self.folder_metadata = folder_metadata
 
     def get_all_folders(self):
-        '''retriving all Looker instance folders'''
-        instance_folders = None
-        trys = 0
-        while instance_folders is None:
-            trys += 1
-            try:
-                instance_folders = self.sdk.all_folders()
-            except:
-                return_sleep_message(call_number=trys)
-        response = [
-            folder.id for folder in instance_folders if folder.parent_id != "2" if folder.parent_id != "3"]
+        instance_folders = self.sdk.all_folders()
+        response = {folder.id: folder.name for folder in instance_folders}
         return response
 
-    @staticmethod
-    def clean_folders(folder_list):
-        '''removing standard system folders from lmanage.folder list'''
-        removal_folder_id = ['1', '2', '3', '4',  'lookml', '5']
-        response = []
-        for elem in enumerate(folder_list):
-            check_value = elem[1]
-            if check_value in removal_folder_id or check_value is None:
+    def scour_folder(self):
+        exempt_folders = ['1', '2', '3', '4', 'lookml']
+        folders = self.get_all_folders()
+        error_count = 0
+        #allowed_folders = [folder_obj for folder_obj in folders.keys() if folder_obj not in exempt_folders]
+        while error_count < 1:
+            folders = self.get_all_folders()
+            x = [folder_obj for folder_obj in folders.keys(
+            ) if folder_obj not in exempt_folders]
+        #for fid in tqdm(allowed_folders):
+            try:
+                self.sdk.delete_folder(folder_id=x[0])
+                logger.debug('deleting folder %s to start afresh',
+                            folders.get(x[0]))
+            except error.SDKError as e:
+                logger.error(e)
+                error_count = 1
+
+    def unnest_folder_data(self, folder_data):
+        for d in tqdm(folder_data, desc = "Unesting Folder Data", unit=" unested", colour="#2c8558"):
+            folder_dict = d
+            metadata_list = []
+            metadata_list = self.walk_folder_structure(
+                dict_obj=folder_dict,
+                data_storage=metadata_list,
+                parent_name='1')
+
+        logger.debug('retrieved yaml folder files')
+        logger.debug('folder metadata = %s', metadata_list)
+
+        return metadata_list
+
+    def walk_folder_structure(self,
+                              dict_obj: dict,
+                              data_storage: list,
+                              parent_name: str):
+        folder_name = dict_obj.get('name')
+
+        try:
+            if parent_name == 'Shared':
                 logger.debug(
-                    'removing folder id %s from lmanage.the capturation', check_value)
+                    f'Creating folder Shared Child Folder "{folder_name}"')
+                folder = self.create_folder(
+                    folder_name=folder_name, parent_id='1')
+                new_folder_id = folder.get('id')
+            elif parent_name == '1':
+                folder = self.sdk.folder(folder_id='1')
+                new_folder_id = 'Shared'
             else:
-                response.append(elem[1])
-
-        response = sorted(response, reverse=True)
-        return response
+                folder = self.create_folder(folder_name=folder_name,
+                                            parent_id=parent_name)
+                new_folder_id = folder.get('id')
+
+            temp = {}
+            temp['name'] = folder_name
+            temp['old_folder_id'] = dict_obj.get('id')
+            temp['new_folder_id'] = new_folder_id
+            temp['content_metadata_id'] = folder.get('content_metadata_id')
+            temp['team_edit'] = dict_obj.get('team_edit')
+            temp['team_view'] = dict_obj.get('team_view')
+            logger.debug('data_structure to be appended = %s', temp)
+            data_storage.append(temp)
+        except error.SDKError as e:
+            logger.warn('error %s', e)
+            logger.warn(
+                'you have a duplicate folder called %s with the same parent, this is against best practice and LManage is ignoring it', folder_name)
+
+        if isinstance(dict_obj.get('subfolder'), list):
+            for subfolder in dict_obj.get('subfolder'):
+                self.walk_folder_structure(subfolder, data_storage,
+                                           parent_name=new_folder_id)
+
+        return data_storage
+
+    def create_folder(self,
+                      folder_name: str,
+                      parent_id: str,
+                      ):
+        logger.debug(f'Creating folder "{folder_name}"')
+        folder = self.sdk.create_folder(
+            body=models.CreateFolder(
+                name=folder_name,
+                parent_id=parent_id
+            )
+        )
+        return folder
+
+    def sync_folders(self, created_folder: list):
+        all_folders = self.sdk.all_folders()
+        created_folder_ids = [fobj.get('folder_id') for fobj in created_folder]
+        all_folder_ids = []
 
-    def get_content_access_metadata(self, cmi, root_folder: bool):
-        r = []
-        cmi_metadata = None
-        trys = 0
-        while cmi_metadata is None:
-            trys += 1
-            try:
-                if root_folder:
-                    cmi_metadata = self.sdk.all_content_metadata_accesses(
-                        content_metadata_id=1)
-                else:
-                    cmi_metadata = self.sdk.all_content_metadata_accesses(
-                        content_metadata_id=cmi)
-            except:
-                return_sleep_message(call_number=trys)
-        for cmi in cmi_metadata:
-            group_id = cmi.group_id
-            if group_id is not None:
-                permission_type = cmi.permission_type.value
-                temp = {}
-                group_meta = None
-                trys = 0
-
-                while group_meta is None:
-                    trys += 1
-                    try:
-                        group_meta = self.sdk.group(group_id=group_id)
-                    except:
-                        return_sleep_message(call_number=trys)
-                temp[permission_type] = group_meta.get('name')
-                r.append(temp)
-            else:
-                logger.info(
-                    'no group permissions set on folder, ignoring individual permissions')
+        for folder in all_folders:
+            if folder.is_personal:
+                pass
+            elif folder.parent_id is None:
                 pass
-        return r
-
-    def create_folder_objects(self, folder_list):
-        '''creating folder objects (class in utils folder)'''
-        response = {}
-        folder_list = sorted(folder_list, key=int, reverse=True)
-        for folder in folder_list:
-            f_metadata = None
-            trys = 0
-            while f_metadata is None:
-                trys = trys+1
-                try:
-                    f_metadata = self.sdk.folder(folder_id=str(folder))
-                except:
-                    return_sleep_message(call_number=trys)
-            if f_metadata.name in ['Shared', 'Users']:
-                folder_name = f_metadata.name
-                f_metadata.name = '%s_' % folder_name
-                logger.debug(f_metadata)
-
-            if f_metadata.is_personal or f_metadata.is_personal_descendant or f_metadata.is_embed:
-                logger.warn(
-                    'folder %s  will be ignored as it\'s a personal folder or embed folder', f_metadata.name)
             else:
-                content_metadata_id = f_metadata.get('content_metadata_id')
-                a_list = self.get_content_access_metadata(
-                    cmi=content_metadata_id, root_folder=False)
-
-                created_folder_object = loc.LookerFolder(
-                    id=folder, folder_metadata=f_metadata, access_list=a_list)
-                logger.info('capturing folder %s', f_metadata.get('name'))
-                response[folder] = created_folder_object
-        root_content_meta = self.get_content_access_metadata(
-            cmi=1, root_folder=True)
-        root_f_meta = None
-        trys = 0
-        while root_f_meta is None:
-            trys += 1
-            try:
-                root_f_meta = self.sdk.folder(folder_id=str(1))
-            except:
-                return_sleep_message(call_number=trys)
-
-        root_folder = loc.LookerFolder(
-            id='1', folder_metadata=root_f_meta, access_list=root_content_meta)
-        response['1'] = root_folder
-        return response
+                all_folder_ids.append(folder.id)
 
-    @ staticmethod
-    def get_highest_folders(folder_list):
-        '''helper to isolate highest level folders and return as a list'''
-        response = [
-            folder for folder in folder_list if folder.parent_id == '1']
-        return response
+        for fids in all_folder_ids:
+            if fids not in created_folder_ids:
+                try:
+                    self.sdk.delete_folder(folder_id=fids)
+                    logger.debug(
+                        'deleting folder %s to sync with yaml config', fids)
+
+                except error.SDKError as InheritanceError:
+                    logger.debug('root folder has been deleted so %s',
+                                InheritanceError)
+        return 'your folders are in sync with your yaml file'
+
+    def create_folders(self):
+        folder_metadata_list = []
+        all_folders = self.get_all_folders()
+        self.scour_folder()
+        created_folder_metadata = self.unnest_folder_data(
+            folder_data=self.folder_metadata)
+        return created_folder_metadata
+
+    def create_folder_mapping_dict(self, folder_metadata: list) -> dict:
+        '''
+        create a folder mapping dict with legacy folder id as it's key and new folder id as the value for use in content migration
+        '''
+        response = {}
+        for folder_obj in folder_metadata:
+            lid = folder_obj.get('old_folder_id')
+            fid = folder_obj.get('new_folder_id')
+            response[lid] = fid
 
-    @ staticmethod
-    def get_subfolders(folder_list, parent_id):
-        '''helper function to get all subfolders for a given parent'''
-        response = []
-        for folder in folder_list:
-            if folder.parent_id == parent_id:
-                response.append(folder)
         return response
-
-    def create_nested_folder_objects(self, folder_list):
-        '''create folder objects list with all children attached return
-        full list of instance folder structure'''
-        for f in folder_list:
-            folder = folder_list.get(f)
-            f_parent_id = folder.parent_id
-
-            if f_parent_id in list(folder_list.keys()):
-                parent_folder = folder_list.get(f_parent_id)
-                parent_folder.add_child_folder(folder)
-            else:
-                pass
-
-        # folder_list = [f for f in list(
-        #     folder_list.values()) if f.parent_id == '1']
-        folder_list = [f for f in list(folder_list.values()) if f.id == '1']
-
-        return folder_list
-
-    def execute(self):
-        '''main function to do chain all the processes'''
-        folders = self.get_all_folders()
-        clean_folders = self.clean_folders(folder_list=folders)
-        created_folder_list = self.create_folder_objects(
-            folder_list=clean_folders)
-        final_folder_list = self.create_nested_folder_objects(
-            folder_list=created_folder_list)
-        return final_folder_list
```

### Comparing `lmanage-0.3.5/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py` & `lmanage-0.3.6/lmanage/capturator/user_attribute_capturation/capture_ua_permissions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,48 @@
 import logging
 import coloredlogs
 from time import sleep
+from lmanage.utils.looker_object_constructors import LookerUserAttribute 
 from lmanage.utils.errorhandling import return_error_message, return_sleep_message
-
-logger = logging.getLogger(__name__)
-coloredlogs.install(level='DEBUG')
-
-
-class LookerUserAttribute():
-    def __init__(self, teams_val: dict, name: str, uatype: bool, hidden_value: bool, user_view, user_edit, default_value) -> object:
-        self.name = name
-        self.uatype = uatype
-        self.hidden_value = hidden_value
-        self.user_view = str(user_view)
-        self.user_edit = str(user_edit)
-        self.default_value = default_value
-        self.teams = teams_val
-
+from tqdm import tqdm
+from tenacity import retry, wait_fixed, wait_random, stop_after_attempt
 
 class ExtractUserAttributes():
     def __init__(self,  sdk):
         self.sdk = sdk
         self.user_attribute_metadata = self.existing_user_attributes()
         self.all_group_metadata = self.all_group_metadatas()
+    
+    @retry(wait=wait_fixed(3) + wait_random(0, 2), stop=stop_after_attempt(5))
+    def get_all_user_attributes(self) -> dict:
+        response = self.sdk.all_user_attributes()
+        return response
 
     def existing_user_attributes(self) -> dict:
-        ex_ua = None
-        trys = 0
-        while ex_ua is None:
-            trys += 1
-            try:
-                ex_ua = self.sdk.all_user_attributes()
-            except:
-                return_sleep_message(call_number=trys)
-        for ua in enumerate(ex_ua):
-            if ua[1].get('is_system'):
-                ua_idx = ua[0]
-                ex_ua.pop(ua_idx)
-        return ex_ua
+        ex_ua = self.get_all_user_attributes()
+        resp = [ua for ua in ex_ua if not ua.is_system]
+        return resp
 
+    @retry(wait=wait_fixed(3) + wait_random(0, 2), stop=stop_after_attempt(5))
     def all_group_metadatas(self):
-        return self.sdk.all_groups()
+        response=self.sdk.all_groups()
+        return response 
+
+    @retry(wait=wait_fixed(3) + wait_random(0, 2), stop=stop_after_attempt(5))
+    def all_user_attribute_group_value_metadata(self, uaid: int):
+        response = self.sdk.all_user_attribute_group_values(uaid)
+        return response
 
-    def create_user_attributes(self):
 
+    def create_user_attributes(self):
         group_metadata = {
             group.id: group.name for group in self.all_group_metadata}
         response = []
-        for ua in self.user_attribute_metadata:
-            group_assign = None
-            trys = 0
-            while group_assign is None:
-                trys += 1
-                try:
-                    group_assign = self.sdk.all_user_attribute_group_values(
-                        user_attribute_id=ua.id)
-                    # logger.info(
-                    #     'capturing groups associated with user attribute %s', group_assign[0].get('user_attribute_id'))
-                except:
-                    return_sleep_message(call_number=trys)
+        for ua in tqdm(self.user_attribute_metadata, desc = "User Attribute Capture", unit=" user att", colour="#2c8558"):
+            group_assign = self.all_user_attribute_group_value_metadata(uaid=ua.id)
             team_values = []
 
             for group in group_assign:
                 group_name = group_metadata.get(group.group_id)
                 teams = {}
                 teams[group_name] = group.value
                 team_values.append(teams)
```

### Comparing `lmanage-0.3.5/lmanage/capturator/user_group_capturation/group_config.py` & `lmanage-0.3.6/lmanage/capturator/user_group_capturation/group_config.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/capturator/user_group_capturation/role_config.py` & `lmanage-0.3.6/lmanage/capturator/user_group_capturation/role_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,18 @@
 import logging
 import coloredlogs
 import itertools
-from time import sleep
+from lmanage.utils.looker_object_constructors import LookerPermissionSet, LookerModelSet, LookerRoles
 from lmanage.utils import errorhandling
-from lmanage.utils.errorhandling import return_sleep_message
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 
 
-class LookerPermissionSet():
-    def __init__(self, permissions, name):
-        self.permissions = permissions
-        self.name = name
-
-
-class LookerModelSet():
-    def __init__(self, models, name):
-        self.models = models
-        self.name = name
-
-
-class LookerRoles():
-    def __init__(self, permission_set, model_set, teams, name):
-        self.permission_set = permission_set
-        self.model_set = model_set
-        self.teams = teams
-        self.name = name
-
-
 class ExtractRoleInfo():
     def __init__(self, sdk):
         self.sdk = sdk
         self.role_base = self.get_all_roles()
 
     def get_all_roles(self):
         sdk = self.sdk
@@ -43,14 +23,16 @@
                 response.pop(role[0])
 
         return response
 
     def create_list_of_permission_sets(self):
         response = []
         for role in self.role_base:
+            if role.permission_set is None:
+                raise Exception(f'role name {role.name} has no permission_set, please add one to be captured or delete the role')
             temp = {}
             temp['name'] = role.permission_set.name
             temp['permissions'] = role.permission_set.permissions
             response.append(temp)
         return response
 
     def extract_permission_sets(self):
@@ -83,23 +65,23 @@
             model_set = LookerModelSet(
                 models=role.get('models'), name=role.get('name'))
             response.append(model_set)
         return response
 
     def extract_role_info(self):
         response = []
-        for role in self.role_base:
+        for role in tqdm(self.role_base, desc = "Role Capture", unit=" roles", colour="#2c8558"):
             groups = None
             trys = 0
             while groups is None:
                 trys += 1
                 try:
                     groups = self.sdk.role_groups(role_id=role.id)
                 except:
-                    return_sleep_message(call_number=trys)
+                    errorhandling.return_sleep_message(call_number=trys)
             role_groups = [group.name for group in groups]
 
             lookerrole = LookerRoles(permission_set=role.permission_set.name,
                                      model_set=role.model_set.name, teams=role_groups, name=role.name)
             response.append(lookerrole)
 
         return response
```

### Comparing `lmanage-0.3.5/lmanage/capturator/user_group_capturation/user_permission.py` & `lmanage-0.3.6/lmanage/capturator/user_group_capturation/user_permission.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/capture_instance_permission_structure.py` & `lmanage-0.3.6/lmanage/capture_instance_permission_structure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,108 @@
 import logging
 import coloredlogs
 import looker_sdk
-import ruamel 
+import ruamel.yaml
+import json
 from lmanage.capturator.user_group_capturation import role_config as rc
 from lmanage.capturator.user_attribute_capturation import capture_ua_permissions as cup
 from lmanage.capturator.folder_capturation import folder_config as fc
 from lmanage.capturator.folder_capturation import create_folder_yaml_structure as cfp
+from lmanage.capturator.content_capturation import dashboard_capture as dc
+from lmanage.capturator.content_capturation import look_capture as lc
 from lmanage.utils import looker_object_constructors as loc
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 logging.getLogger("looker_sdk").setLevel(logging.WARNING)
 
 
 def main(**kwargs):
-    div = '-------------------------------------------------------------------'
 
     ini_file = kwargs.get("ini_file")
     yaml_path = kwargs.get("yaml_export_path")
-    logger.info(div)
+    yaml_path = yaml_path.split('.')[0]
+
     logger.info('creating yaml configuration file')
 
     if ini_file:
         sdk = looker_sdk.init40(config_file=ini_file)
     else:
         sdk = looker_sdk.init40()
 
     yaml = ruamel.yaml.YAML()
+    yaml.register_class(loc.LookerFolder)
+    yaml.register_class(loc.LookerModelSet)
+    yaml.register_class(loc.LookerPermissionSet)
+    yaml.register_class(loc.LookerRoles)
+    yaml.register_class(loc.LookerUserAttribute)
+    yaml.register_class(loc.LookObject)
+    yaml.register_class(loc.DashboardObject)
 
 ###############################################################
 # Capture Folder Config #######################################
 ###############################################################
-    folder_structurelist = fc.CaptureFolderConfig(sdk=sdk).execute()
-    yaml.register_class(loc.LookerFolder)
-    print(f'{yaml_path}')
-    with open(f'{yaml_path}', 'w') as file:
+    folder_returns = fc.CaptureFolderConfig(sdk=sdk).execute()
+    folder_structure_list = folder_returns[1]
+
+    with open(f'{yaml_path}.yaml', 'w') as file:
         fd_yml_txt = '''# FOLDER_PERMISSIONS\n# Opening Session Welcome to the Capturator, this is the Folder place\n# -----------------------------------------------------\n\n'''
         file.write(fd_yml_txt)
-        # file.write('# FOLDER_PERMISSIONS\n')
-        yaml.dump(folder_structurelist, file)
+        yaml.dump(folder_structure_list, file)
 
-    # yaml.dump(folder_structurelist, sys.stdout)
+    folder_root_dict = folder_returns[0]
 
-    logger.info(div)
 ###############################################################
 # Capture Roles ###############################################
 ###############################################################
     roles = rc.ExtractRoleInfo(sdk=sdk)
 
     looker_permission_sets = roles.extract_permission_sets()
     looker_model_sets = roles.extract_model_sets()
 
     looker_roles = roles.extract_role_info()
-    yaml.register_class(rc.LookerModelSet)
-    yaml.register_class(rc.LookerPermissionSet)
-    yaml.register_class(rc.LookerRoles)
-    with open(f'{yaml_path}', 'a') as file:
+    with open(f'{yaml_path}.yaml', 'a') as file:
         r_yml_txt = '''# Looker Role\n# Opening Session Welcome to the Capturator, this is the Role place\n# -----------------------------------------------------\n\n'''
         file.write(r_yml_txt)
 
         file.write('\n\n# PERMISSION SETS\n')
         yaml.dump(looker_permission_sets, file)
         file.write('\n\n# MODEL SETS\n')
         yaml.dump(looker_model_sets, file)
         file.write('\n\n# LOOKER ROLES\n')
         yaml.dump(looker_roles, file)
 ###############################################################
 # Capture User Attributes #####################################
 ###############################################################
     looker_ua = cup.ExtractUserAttributes(sdk=sdk).create_user_attributes()
     yaml.register_class(cup.LookerUserAttribute)
-    with open(f'{yaml_path}', 'a') as file:
+    with open(f'{yaml_path}.yaml', 'a') as file:
         file.write('\n\n# USER_ATTRIBUTES\n')
         yaml.dump(looker_ua, file)
 
+###############################################################
+# Capture Users Content #######################################
+###############################################################
+    # Capture Look Content
+    looks = lc.CaptureLookObject(sdk=sdk, folder_root=folder_root_dict).execute()
+    with open(f'{yaml_path}_content.yaml', 'w+') as file:
+        file.write('\n\n# LookData\n')
+        yaml.dump(looks, file)
+
+    # Capture Dashboard Content
+    dash_content = dc.CaptureDashboards(sdk=sdk, folder_root=folder_root_dict).execute()
+    with open(f'{yaml_path}_content.yaml', 'a') as file:
+        fd_yml_txt = '\n\n# Dashboard Content\n'
+        file.write(fd_yml_txt)
+        yaml.dump(dash_content, file)
+
+
     # FIND UNIQUE USER ATTRIBUTES AND ATTRIBUTE TO TEAM
-    logger.info('Lmanage has finished capturing your Looker instance!')
-    logger.info('please find the captured instance at %s', yaml_path)
+    logger.info('\n\n\n Lmanage has finished capturing your Looker instance!\n')
+    logger.info('\n\nplease find captured settings metadata at: \n%s.yaml \n\ncaptured content metadata at:\n%s_content.yaml', yaml_path, yaml_path)
 
 
 if __name__ == "__main__":
     instance = 'dev'
     IP = (
         f'/usr/local/google/home/hugoselbie/code_sample/py/ini/{instance}.ini')
     YP = (
```

### Comparing `lmanage-0.3.5/lmanage/cli.py` & `lmanage-0.3.6/lmanage/cli.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/configurator/__init__.py` & `lmanage-0.3.6/lmanage/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/configurator/commands.py` & `lmanage-0.3.6/lmanage/configurator/commands.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/configurator/folder_configuration/create_folder_permissions.py` & `lmanage-0.3.6/lmanage/configurator/folder_configuration/create_folder_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 import logging
 import time
 import coloredlogs
 from looker_sdk import models, error
-
 from lmanage.utils import errorhandling
+from tqdm import tqdm
+from lmanage.utils.errorhandling import return_sleep_message
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='DEBUG')
 
 
 class CreateAndProvisionInstanceFolders():
     def __init__(self, folders, sdk):
         self.sdk = sdk
         self.instance_folder_metadata = folders
 
-    def get_content_access_metadata(self, folders: list) -> list:
+    def get_content_access_metadata(self, folder: dict) -> list:
         response = []
 
         folder_list = self.sdk.all_folders()
         folder_cmaid_lookup = {
             folder.name: folder.content_metadata_id for folder in folder_list}
 
-        for folder in folders:
-            folder_name = folder.get('name')
-            cmaid = folder_cmaid_lookup.get(folder_name)
-            temp_dict = {}
-            temp_dict['name'] = folder_name
-            temp_dict['cmi'] = cmaid
-            edit_group = folder.get('team_edit')
-            view_group = folder.get('team_view')
-
-            perms = []
-            if isinstance(edit_group, list):
-                for group in edit_group:
-                    group_dict = {}
-                    egmetadata = self.sdk.search_groups(name=group)
-                    group_dict['name'] = group
-                    group_dict['id'] = egmetadata[0].id
-                    group_dict['permission'] = 'edit'
-                    perms.append(group_dict)
-            else:
+        folder_name = folder.get('name')
+        cmaid = folder_cmaid_lookup.get(folder_name)
+        temp_dict = {}
+        temp_dict['name'] = folder_name
+        temp_dict['cmi'] = cmaid
+        edit_group = folder.get('team_edit')
+        view_group = folder.get('team_view')
+
+        perms = []
+        if isinstance(edit_group, list):
+            for group in edit_group:
                 group_dict = {}
-                group_dict['name'] = 'no_name'
-                group_dict['id'] = 'no_id'
-                group_dict['permission'] = 'no_permission'
+                egmetadata = self.sdk.search_groups(name=group)
+                group_dict['name'] = group
+                group_dict['id'] = egmetadata[0].id
+                group_dict['permission'] = 'edit'
                 perms.append(group_dict)
+        else:
+            group_dict = {}
+            group_dict['name'] = 'no_name'
+            group_dict['id'] = 'no_id'
+            group_dict['permission'] = 'no_permission'
+            perms.append(group_dict)
 
-            if isinstance(view_group, list):
-                for group in view_group:
-                    group_dict = {}
-                    vgmetadata = self.sdk.search_groups(name=group)
-                    group_dict['name'] = group
-                    group_dict['id'] = vgmetadata[0].id
-                    group_dict['permission'] = 'view'
-                    perms.append(group_dict)
-            else:
+        if isinstance(view_group, list):
+            for group in view_group:
                 group_dict = {}
-                group_dict['name'] = 'no_name'
-                group_dict['id'] = 'no_id'
-                group_dict['permission'] = 'no_permission'
+                vgmetadata = self.sdk.search_groups(name=group)
+                group_dict['name'] = group
+                group_dict['id'] = vgmetadata[0].id
+                group_dict['permission'] = 'view'
                 perms.append(group_dict)
+        else:
+            group_dict = {}
+            group_dict['name'] = 'no_name'
+            group_dict['id'] = 'no_id'
+            group_dict['permission'] = 'no_permission'
+            perms.append(group_dict)
 
-            temp_dict['group_permissions'] = perms
-            response.append(temp_dict)
+        temp_dict['group_permissions'] = perms
+        response.append(temp_dict)
         return response
 
     def create_content_metadata_access(
         self,
             group_id: int,
             permission_input: str,
             content_metadata_id: int) -> dict:
@@ -77,15 +77,15 @@
                 permission_type=permission_input,
                 group_id=group_id
             )
         )
         folder = self.sdk.content_metadata(
             content_metadata_id=content_metadata_id).name
         group = self.sdk.search_groups(id=group_id)[0].name
-        logger.info(
+        logger.debug(
             f'''--> Successfully permissioned group {group} with {permission_input} access, on folder {folder}.''')
 
     def check_existing_access(self,
                               content_metadata_id: int) -> dict:
         # check for existing access to the folder
         response = {
             access.group_id: access
@@ -118,15 +118,16 @@
             if group_id not in folder_access:
                 if self.check_folder_inheritance(
                         content_metadata_id=ancestor_cmaid):
                     # N.B. when you update folder inheritance you will create a content metadata access
                     # so recheck value to prevent trying to set an already set value
                     self.update_folder_inheritance(
                         cmaid=ancestor_cmaid, inheritance=False)
-                    folder_access = self.check_existing_access(content_metadata_id=ancestor_cmaid)
+                    folder_access = self.check_existing_access(
+                        content_metadata_id=ancestor_cmaid)
                     if folder_access:
                         pass
                     else:
                         self.create_content_metadata_access(
                             group_id=group_id,
                             permission_input='view',
                             content_metadata_id=ancestor_cmaid)
@@ -159,26 +160,22 @@
 
         if 'true' in check:
             return True
         else:
             return False
 
     def update_folder_inheritance(
-        self,
-        cmaid: int,
-        inheritance: bool):
+            self,
+            cmaid: int,
+            inheritance: bool):
         # don't want to inherit access from lmanage.parent folders
         self.sdk.update_content_metadata(
             content_metadata_id=cmaid,
             body=models.WriteContentMeta(inherits=inheritance)
         )
-    # except error.SDKError as content_metadata_error:
-        #     err_msg = errorhandling.return_error_message(
-        #         content_metadata_error)
-        #     logger.warn('there might be a warning %s', err_msg)
 
     def add_content_access(
         self,
             cm_accesses: dict,
             cmaid: int,
             group_permissions: list) -> dict:
 
@@ -195,15 +192,15 @@
             )
             group_name = self.sdk.search_groups(id=group_id)[0].name
 
             if group_id in cm_accesses.keys():
                 current_access = cm_accesses.get(group_id)
 
                 if current_access.permission_type == permission:
-                    logger.info(
+                    logger.debug(
                         f'''--> Group {group_name} already has access, to folder {folder_name}
                         no changes made.''')
 
                 else:
                     try:
                         self.sdk.update_content_metadata_access(
                             content_metadata_access_id=current_access.id,
@@ -214,15 +211,15 @@
                             ))
                     except error.SDKError as foldererror:
                         logger.debug(foldererror)
                     folder_name = self.sdk.content_metadata(
                         content_metadata_id=cmaid).name
                     group_name = self.sdk.search_groups(id=group_id)[0].name
 
-                    logging.info(
+                    logger.debug(
                         f'--> Updating group id {group_name} permission type to {permission} on folder {folder_name}.')
 
             # no existing access
             # create from lmanage.scratch
             elif permission == 'no_permission':
                 pass
             else:
@@ -230,16 +227,16 @@
                     content_metadata_id=cmaid,
                     permission_input=permission,
                     group_id=group_id
                 )
 
     def provision_folders_with_group_access(self, content_access_metadata_list: list):
 
-        for folder_tree in content_access_metadata_list:
-            
+        for folder_tree in tqdm(content_access_metadata_list, desc="Folder Perms - Group Access", unit=" folders provisioned", colour="#2c8558"):
+
             for access_item in folder_tree:
                 content_metadata_id = access_item["cmi"]
 
                 self.update_folder_inheritance(
                     cmaid=content_metadata_id, inheritance=False)
 
                 gp_permissions = access_item.get('group_permissions')
@@ -253,15 +250,15 @@
         # remove all accesses
         for group_id in cm_accesses.keys():
             try:
                 delete_cmi = cm_accesses.get(group_id).id
                 self.sdk.delete_content_metadata_access(
                     content_metadata_access_id=delete_cmi)
             except error.SDKError as InheritanceError:
-                logger.warn('''You have an inheritance error in your YAML file possibly 
+                logger.debug('''You have an inheritance error in your YAML file possibly 
                             around %s, skipping group_id %s''', delete_cmi, group_id)
                 logger.debug(InheritanceError)
 
     def sync_folder_permission(
         self,
         cmaid: int,
             gp_permissions: list):
@@ -269,16 +266,17 @@
         # check for existing access to the folder
         content_metadata_accesses = self.check_existing_access(
             content_metadata_id=cmaid)
 
         # check group permissions and add back 1 by 1
         gp_permissions = [
             perms for perms in gp_permissions if perms.get('id') != 'no_id']
-        
-        logger.info('syncing folder permissions for content metadata id %s', cmaid)
+
+        logger.debug(
+            'syncing folder permissions for content metadata id %s', cmaid)
 
         if not gp_permissions:
             self.update_folder_inheritance(
                 cmaid=cmaid, inheritance=True)
             self.update_folder_inheritance(cmaid=cmaid, inheritance=False)
         else:
             # remove folder content accesses
@@ -305,15 +303,15 @@
                 body=models.ContentMetaGroupUser(
                     permission_type='view',
                     content_metadata_id=folder,
                     group_id=folder
                 )
             )
         except error.SDKError:
-            logger.info('All Users group already configured')
+            logger.debug('All Users group already configured')
         clean = list()
         for avt in content_access_metadata_list:
             temp = {}
             temp['name'] = avt[0].get('name')
             temp['cmi'] = avt[0].get('cmi')
             clean.append(temp)
         res_list = [i for n, i in enumerate(clean) if i not in clean[n + 1:]]
@@ -335,16 +333,16 @@
                     cmaid = value.id
                     self.sdk.delete_content_metadata_access(
                         content_metadata_access_id=cmaid)
 
     def execute(self):
         # CONFIGURE FOLDERS WITH EDIT AND VIEW ACCESS
         content_access_metadata = []
-        for folder_tree in self.instance_folder_metadata:
-            r = self.get_content_access_metadata(folders=folder_tree)
+        for folder_obj in tqdm(self.instance_folder_metadata, desc="Folder Perms - Edit/View Access", unit=" folders", colour="#2c8558"):
+            r = self.get_content_access_metadata(folder=folder_obj)
             content_access_metadata.append(r)
 
         # ADD AND SYNC CONTENT VIEW ACCESS WITH YAML
         self.provision_folders_with_group_access(
             content_access_metadata_list=content_access_metadata)
         self.remove_all_user_group(
             content_access_metadata_list=content_access_metadata)
```

### Comparing `lmanage-0.3.5/lmanage/configurator/folder_configuration/folder_config.py` & `lmanage-0.3.6/lmanage/configurator/folder_configuration/folder_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from os import name
 from looker_sdk import models, error
 import coloredlogs
 
 logger = logging.getLogger(__name__)
-coloredlogs.install(level='DEBUG')
+coloredlogs.install(level='INFO')
 logging.getLogger("requests").setLevel(logging.WARNING)
 
 
 class FolderConfig():
     ''' Class to read in folder metadata and unested_folder_data '''
 
     def __init__(self, folders):
```

### Comparing `lmanage-0.3.5/lmanage/configurator/instance_configuration_settings/fullinstance.yaml` & `lmanage-0.3.6/lmanage/configurator/instance_configuration_settings/fullinstance.yaml`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py` & `lmanage-0.3.6/lmanage/configurator/user_attribute_configuration/create_ua_permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import coloredlogs
 from looker_sdk import models, error
+from tqdm import tqdm
 
-logger = logging.getLogger(__name__)
-coloredlogs.install(level='DEBUG')
+#logger = logging.getLogger(__name__)
+#coloredlogs.install(level='DEBUG')
 
 
 class CreateAndAssignUserAttributes():
     def __init__(self, user_attributes, sdk):
         self.user_attribute_metadata = user_attributes
         self.sdk = sdk
 
@@ -17,37 +18,39 @@
         all_ua = {ua.name: ua.id for ua in all_instance_ua}
         return all_ua
 
     def create_user_attribute_if_not_exists(self):
         existing_ua = self.existing_user_attributes()
         yaml_user_attributes = self.user_attribute_metadata
 
-        for ua in yaml_user_attributes:
+        for ua in tqdm(yaml_user_attributes, desc = "User Attribute Creation", unit=" attributes", colour="#2c8558"):
             name = ua.get('name')
             if name in existing_ua.keys():
-                logger.warn(
+                logging.warning(
                     f'user attribute {name} already exists on this instance')
             else:
                 datatype = ua.get('uatype')
                 value_is_hidden = ua.get('hidden_value')
                 user_view = ua.get('user_view')
                 user_edit = ua.get('user_edit')
 
-                ua_permissions = models.WriteUserAttribute(
-                    name=name,
-                    label=name,
-                    type=datatype,
-                    value_is_hidden=value_is_hidden,
-                    user_can_view=user_view,
-                    user_can_edit=user_edit,
-                    default_value=ua.get('default_value')
-                )
-
-                response = self.sdk.create_user_attribute(body=ua_permissions)
-                logger.info(f'created user attribute {response.label}')
+                try:
+                    ua_permissions = models.WriteUserAttribute(
+                        name=name,
+                        label=name,
+                        type=datatype,
+                        value_is_hidden=value_is_hidden,
+                        user_can_view=user_view,
+                        user_can_edit=user_edit,
+                        default_value=ua.get('default_value')
+                    )
+                    response = self.sdk.create_user_attribute(body=ua_permissions)
+                    logging.info(f'created user attribute {response.label}')
+                except error.SDKError as err:
+                    logging.error('skipping permission because already exists')
 
     def sync_user_attributes(self):
         instance_ua = self.existing_user_attributes()
         config_ua = [ua.get('name') for ua in self.user_attribute_metadata]
         sys_default_ua = [
             'email',
             'first_name',
@@ -63,15 +66,15 @@
             if ua in instance_ua:
                 instance_ua.pop(ua, None)
 
         for ua_name in instance_ua.keys():
             if ua_name not in config_ua:
                 ua_id = instance_ua.get(ua_name)
                 self.sdk.delete_user_attribute(ua_id)
-                logger.info(
+                logging.info(
                     f'''deleting ua {ua_name} because
                     it is not listed in the yaml config''')
 
     def add_group_values_to_ua(self):
         instance_ua = self.existing_user_attributes()
         all_instance_groups = self.sdk.all_groups()
         group_metadata = {
```

### Comparing `lmanage-0.3.5/lmanage/configurator/user_group_configuration/group_config.py` & `lmanage-0.3.6/lmanage/configurator/user_group_configuration/group_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import coloredlogs
 from looker_sdk import models, error
 from lmanage.utils.errorhandling import return_error_message
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='DEBUG')
 
 
 class CreateInstanceGroups():
     def __init__(self, folders, user_attributes, roles, sdk) -> None:
@@ -25,58 +26,57 @@
                 else:
                     for team_val in team_list:
                         data_storage.append(team_val)
         return data_storage
 
     def extract_folder_teams(self, container, data_storage):
         for folder_element in container:
-            for folder in folder_element:
-                if isinstance(folder.get('team_edit'), list):
-                    edit_group = folder.get('team_edit')
+            if isinstance(folder_element.get('team_edit'), list):
+                    edit_group = folder_element.get('team_edit')
                     for group in edit_group:
                         data_storage.append(group)
-                if isinstance(folder.get('team_view'), list):
-                    view_group = folder.get('team_view')
+            if isinstance(folder_element.get('team_view'), list):
+                    view_group = folder_element.get('team_view')
                     for group in view_group:
                         data_storage.append(group)
-                else:
-                    pass
+            else:
+                pass
 
     def create_group_if_not_exists(self,
                                    sdk,
                                    group_name: str) -> dict:
         """ Create a Looker Group and add Group attributes
 
         :group_name: Name of a Looker group to create.
         :rtype: Looker Group object.
         """
         # get group if exists
         try:
-            logger.info(f'Creating group "{group_name}"')
+            logger.debug(f'Creating group "{group_name}"')
             group = sdk.create_group(
                 body=models.WriteGroup(
                     can_add_to_content_metadata=True,
                     name=group_name
                 )
             )
             return group
         except error.SDKError as grouperr:
             err_msg = return_error_message(grouperr)
-            logger.warn(
+            logger.debug(
                 'You have hit a warning creating your group; warning = %s', err_msg)
             logger.debug(grouperr)
             group = sdk.search_groups(name=group_name)
             return group[0]
 
     def get_instance_group_metadata(self,
                                     sdk,
                                     unique_group_list: list) -> list:
         group_metadata = []
 
-        for group_name in unique_group_list:
+        for group_name in tqdm(unique_group_list, desc = "Creating User Groups", unit=" user groups", colour="#2c8558"):
             group = self.create_group_if_not_exists(sdk, group_name)
             temp = {}
             temp['group_id'] = group.id
             temp['group_name'] = group.name
             group_metadata.append(temp)
 
         return group_metadata
```

### Comparing `lmanage-0.3.5/lmanage/configurator/user_group_configuration/role_config.py` & `lmanage-0.3.6/lmanage/configurator/user_group_configuration/role_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from looker_sdk import models, error
 import logging
 import coloredlogs
 from lmanage.utils import errorhandling as eh
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 
 
 class CreateRoleBase():
     def __init__(self, permissions, model_sets, sdk):
         self.permission_set_metadata = permissions
         self.model_set_metadata = model_sets
         self.sdk = sdk
 
     def create_permission_set(self, sdk, permission_set_dict: dict):
 
         final_response = []
-        for permission in permission_set_dict:
+        for permission in tqdm(permission_set_dict, desc = "Creating Permission Sets", unit=" perm sets", colour="#2c8558"):
             permission_set_name = permission.get('name')
             if permission_set_name == 'Admin':
                 pass
             else:
                 permissions = permission.get('permissions')
                 body = models.WritePermissionSet(
                     name=permission_set_name.lower(),
@@ -30,15 +31,15 @@
                     perm = sdk.create_permission_set(
                         body=body
                     )
                 except error.SDKError as permerr:
                     logger.debug(permerr)
                     err_msg = eh.return_error_message(permerr)
                     logger.debug(permerr)
-                    logger.warn(
+                    logger.debug(
                         'you have a warning permission set %s, warning = %s already exists on this instance', permission_set_name, err_msg)
 
                     perm = sdk.search_permission_sets(
                         name=permission_set_name)[0]
                     pid = perm.id
                     perm = sdk.update_permission_set(
                         permission_set_id=pid, body=body)
@@ -65,41 +66,41 @@
             if permission_set_name.lower() not in yaml_permissions:
                 permission_id = permissions_dict.get(permission_set_name)
                 sdk.delete_permission_set(permission_set_id=permission_id)
 
     def create_model_set(self, sdk, model_set_dict: list) -> list:
         final_response = []
         model_set_dict = eh.dedup_list_of_dicts(model_set_dict)
-        for model in model_set_dict:
+        for model in tqdm(model_set_dict, desc = "Creating Model Sets", unit=" model sets", colour="#2c8558"):
             model_set_name = model.get('name')
             attributed_models = model.get('models')
             body = models.WriteModelSet(
                 name=model_set_name.lower(), models=attributed_models)
             try:
                 model = sdk.create_model_set(body=body)
                 temp = {}
                 final_response.append(temp)
             except error.SDKError as modelerror:
                 err_msg = eh.return_error_message(modelerror)
-                logger.warn(
+                logger.debug(
                     'you have a warning in creating model set %s, warning = %s', model_set_name, err_msg)
                 logger.debug(modelerror)
                 model = sdk.search_model_sets(name=model_set_name)[0]
                 model_set_id = model.id
                 try:
                     model = sdk.update_model_set(
                         model_set_id=model_set_id, body=body)
 
                     temp = {}
                     temp['model_set_name'] = model.name
                     temp['model_set_id'] = model.id
                     final_response.append(temp)
                 except error.SDKError as txt:
                     err_msg = eh.return_error_message(txt)
-                    logger.warn(
+                    logger.debug(
                         'The model %s, has encountered a warning, warning = %s', model_set_name, err_msg)
                     temp = {}
                     temp['model_set_name'] = model.name
                     temp['model_set_id'] = model.id
                     final_response.append(temp)
 
         logger.debug(final_response)
```

### Comparing `lmanage-0.3.5/lmanage/configurator/user_group_configuration/user_permission.py` & `lmanage-0.3.6/lmanage/configurator/user_group_configuration/user_permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import json
 import coloredlogs
 from looker_sdk import models, error
 from lmanage.configurator.user_group_configuration.role_config import CreateRoleBase
 from lmanage.utils.errorhandling import return_error_message
+from lmanage.utils.errorhandling import return_sleep_message
+from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 
 
 class CreateInstanceRoles(CreateRoleBase):
     def __init__(self, roles, sdk):
@@ -38,15 +40,15 @@
 
     def create_instance_roles(self):
         model_lookup = self.create_model_lookup()
         permission_lookup = self.create_permission_lookup()
 
         role_output = []
 
-        for r_metadata in self.role_metadata:
+        for r_metadata in tqdm(self.role_metadata, desc = "User Role Creation", unit=" user roles", colour="#2c8558"):
             role_name = r_metadata.get('name')
             model_set_id = model_lookup.get(
                 r_metadata.get('model_set') if r_metadata.get('model_set') == 'All' else r_metadata.get('model_set').lower())
             permission_set_id = permission_lookup.get(
                 r_metadata.get('permission_set').lower())
             if role_name != 'Admin':
                 body = models.WriteRole(
@@ -57,43 +59,44 @@
                 try:
                     role = self.sdk.create_role(
                         body=body
                     )
 
                 except error.SDKError as roleerror:
                     err_msg = return_error_message(roleerror)
-                    logger.warn(
+                    logger.debug(
                         'You have hit a warning creating your role \'%s\'; warning = %s', role_name, err_msg)
                     role_id = self.sdk.search_roles(name=role_name)[0].id
                     role = self.sdk.update_role(
                         role_id=str(role_id), body=body)
+        
                 temp = {}
                 temp['role_id'] = role.id
                 temp['role_name'] = role_name
                 role_output.append(temp)
             else:
                 pass
         logger.debug(role_output)
         return role_output
 
     def set_role(self, role_id: str, group_id: list) -> str:
         try:
             self.sdk.set_role_groups(role_id, group_id)
-            return logger.info(f'attributing {group_id} permissions on instance')
+            return logger.debug(f'attributing {group_id} permissions on instance')
         except error.SDKError as role_err:
             err_msg = return_error_message(role_err)
-            logger.warn(
+            logger.debug(
                 'You have hit a warning setting your role, warning = %s', err_msg)
             logger.debug(role_err)
 
     def attribute_instance_roles(self, created_role_metadata: list):
         role_lookup = self.create_allrole_lookup()
         group_lookup = self.create_allgroup_lookup()
 
-        for r_metadata in self.role_metadata:
+        for r_metadata in tqdm(self.role_metadata, desc = "Instance Role Attribution", unit=" roles", colour="#2c8558"):
             role_name = r_metadata.get('name')
             teams = r_metadata.get('teams')
             role_id = role_lookup.get(role_name)
             group_id_list = []
             for team in teams:
                 group_id = group_lookup.get(team)
                 group_id_list.append(group_id)
```

### Comparing `lmanage-0.3.5/lmanage/find_replace.sh` & `lmanage-0.3.6/lmanage/find_replace.sh`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/__init__.py` & `lmanage-0.3.6/lmanage/mapview/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/compare_content_to_lookml.py` & `lmanage-0.3.6/lmanage/mapview/compare_content_to_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/hugo.csv` & `lmanage-0.3.6/lmanage/mapview/hugo.csv`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/instancedata.py` & `lmanage-0.3.6/lmanage/mapview/instancedata.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/legacy_get_content_with_views.py` & `lmanage-0.3.6/lmanage/mapview/legacy_get_content_with_views.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/main.py` & `lmanage-0.3.6/lmanage/mapview/main.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/mapexplores.py` & `lmanage-0.3.6/lmanage/mapview/mapexplores.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/mapview_execute.py` & `lmanage-0.3.6/lmanage/mapview/mapview_execute.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/matched_field_analysis.py` & `lmanage-0.3.6/lmanage/mapview/matched_field_analysis.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/pandas_multiple.xlsx` & `lmanage-0.3.6/lmanage/mapview/pandas_multiple.xlsx`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/parse_sql_tables.py` & `lmanage-0.3.6/lmanage/mapview/parse_sql_tables.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/utils/__init__.py` & `lmanage-0.3.6/lmanage/mapview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/utils/create_df.py` & `lmanage-0.3.6/lmanage/mapview/utils/create_df.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/utils/parse_lookml.py` & `lmanage-0.3.6/lmanage/mapview/utils/parse_lookml.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/mapview/utils/parsing_sql.py` & `lmanage-0.3.6/lmanage/mapview/utils/parsing_sql.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/utils/__init__.py` & `lmanage-0.3.6/lmanage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lmanage-0.3.5/lmanage/utils/parse_yaml.py` & `lmanage-0.3.6/lmanage/utils/parse_yaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-import yaml
+import yaml 
 import logging
 import coloredlogs
 
 logger = logging.getLogger(__name__)
 coloredlogs.install(level='INFO')
 
 
@@ -45,7 +45,21 @@
 
     def get_user_attribute_metadata(self):
         response = []
         for objects in self.parsed_yaml:
             if 'hidden_value' in list(objects.keys()):
                 response.append(objects)
         return response
+
+    def get_look_metadata(self):
+        response = []
+        for objects in self.parsed_yaml:
+            if 'query_obj' in list(objects.keys()):
+                response.append(objects)
+        return response
+    
+    def get_dash_metadata(self):
+        response = []
+        for objects in self.parsed_yaml:
+            if 'lookml' in list(objects.keys()):
+                response.append(objects)
+        return response
```

### Comparing `lmanage-0.3.5/pyproject.toml` & `lmanage-0.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 [tool.poetry]
 name = "lmanage"
-version = "0.3.05"
+version = "0.3.06"
 description = "LManage is a collection of useful tools for Looker admins to help curate and cleanup content and it's associated source LookML."
 keywords = ["keyword", "another_keyword"]
 authors = ["hselbie <hselbie@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/looker-open-source/lmanage"
 repository = "https://github.com/looker-open-source/lmanage"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
-# pandas = ">=3.8,<3.9"
 click = "^7.1.2"
-icecream = "^2.1.0"
 ipython = "^7.20.0"
 tabulate = "^0.8.8"
 coloredlogs = "^15.0"
 verboselogs = "^1.7"
 coloredlogger = "^1.3.12"
-pytest-mock = "^3.5.1"
-snoop = "^0.3.0"
-debugpy = "^1.3.0"
-pynvim = "^0.4.3"
 pylint = "^2.9.5"
 lkml = "^1.1.1"
 flake8 = "^4.0.1"
 autopep8 = "^1.6.0"
 PyYAML = "^6.0"
 looker-sdk = "^22.4.0"
 sqlparse = "^0.4.2"
 XlsxWriter = "^3.0.3"
 "ruamel.yaml" = "^0.17.21"
-pandas = "^1.5.2"
-mypy = "^0.991"
-retrying = "^1.3.4"
+tqdm = "^4.65.0"
+# poetry = "^1.4.2"
+yaspin = "^2.3.0"
+tenacity = "^8.2.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-autopep8 = "^1.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lmanage = 'lmanage.cli:lmanage'
```

