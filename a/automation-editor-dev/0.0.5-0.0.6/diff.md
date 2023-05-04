# Comparing `tmp/automation_editor_dev-0.0.5.tar.gz` & `tmp/automation_editor_dev-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor_dev-0.0.5.tar", last modified: Tue May  2 12:49:39 2023, max compression
+gzip compressed data, was "automation_editor_dev-0.0.6.tar", last modified: Thu May  4 06:31:53 2023, max compression
```

## Comparing `automation_editor_dev-0.0.5.tar` & `automation_editor_dev-0.0.6.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.706597 automation_editor_dev-0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5889 2023-05-02 12:49:39.704603 automation_editor_dev-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-04-29 11:09:10.000000 automation_editor_dev-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:38.950587 automation_editor_dev-0.0.5/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:38.981504 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.046837 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-05-02 10:51:41.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.103685 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.175999 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.202927 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.251306 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.272250 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.286213 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.322623 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.325615 automation_editor_dev-0.0.5/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.334591 automation_editor_dev-0.0.5/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.401413 automation_editor_dev-0.0.5/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.446292 automation_editor_dev-0.0.5/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.5/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.458262 automation_editor_dev-0.0.5/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-05-02 10:51:41.000000 automation_editor_dev-0.0.5/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.477210 automation_editor_dev-0.0.5/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.481199 automation_editor_dev-0.0.5/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.540042 automation_editor_dev-0.0.5/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor_dev-0.0.5/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.573953 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.584922 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.607861 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.614842 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.621823 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.5/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:49:39.701610 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     5889 2023-05-02 12:49:38.000000 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2951 2023-05-02 12:49:38.000000 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:49:38.000000 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-02 12:49:38.000000 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-02 12:49:38.000000 automation_editor_dev-0.0.5/automation_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1272 2023-05-02 12:46:22.000000 automation_editor_dev-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 12:49:39.707594 automation_editor_dev-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.420542 automation_editor_dev-0.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5889 2023-05-04 06:31:53.419541 automation_editor_dev-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.228871 automation_editor_dev-0.0.6/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.231869 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.238874 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-03 02:40:57.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.245181 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.250268 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     4000 2023-05-03 02:40:57.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.260270 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-05-03 02:33:10.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.266186 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+-rw-rw-rw-   0        0        0     2927 2023-05-03 09:50:43.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.275185 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4163 2023-05-03 02:40:57.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.282186 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-05-03 02:39:24.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.290188 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.302188 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.306204 automation_editor_dev-0.0.6/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.312188 automation_editor_dev-0.0.6/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.314701 automation_editor_dev-0.0.6/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.324703 automation_editor_dev-0.0.6/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.6/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.330740 automation_editor_dev-0.0.6/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor_dev-0.0.6/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.337704 automation_editor_dev-0.0.6/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.340768 automation_editor_dev-0.0.6/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.346706 automation_editor_dev-0.0.6/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor_dev-0.0.6/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.357706 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.363703 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.369703 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.376705 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.384051 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.6/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-04 06:31:53.416546 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     5889 2023-05-04 06:31:53.000000 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3099 2023-05-04 06:31:53.000000 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 06:31:53.000000 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-04 06:31:53.000000 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-04 06:31:53.000000 automation_editor_dev-0.0.6/automation_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1272 2023-05-04 06:31:36.000000 automation_editor_dev-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 06:31:53.421627 automation_editor_dev-0.0.6/setup.cfg
```

### Comparing `automation_editor_dev-0.0.5/LICENSE` & `automation_editor_dev-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/PKG-INFO` & `automation_editor_dev-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_editor_dev
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor_dev-0.0.5/README.md` & `automation_editor_dev-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import sys
 
 from PySide6.QtWidgets import QApplication
-from je_editor import EditorMain
+from je_editor import EditorMain, shell_manager
 from qt_material import apply_stylesheet
 
 from automation_editor.automation_editor_ui. \
     menu.api_testka_menu.build_api_testka_menu import set_apitestka_menu
 from automation_editor.automation_editor_ui. \
     menu.auto_control_menu.build_autocontrol_menu import set_autocontrol_menu
+from automation_editor.automation_editor_ui.menu.install_menu.build_install_menu import set_install_menu
 from automation_editor.automation_editor_ui.menu. \
     load_density_menu.build_load_density_menu import set_load_density_menu
 from automation_editor.automation_editor_ui \
     .menu.web_runner_menu.build_webrunner_menu import set_web_runner_menu
 from automation_editor.automation_editor_ui.syntax.syntax_extend import \
     syntax_extend_package
 
 
-class ITE(EditorMain):
+class AutomationEditor(EditorMain):
 
     def __init__(self):
         super().__init__()
         self.current_run_code_window = list()
         self.help_menu.deleteLater()
         set_autocontrol_menu(self)
         set_apitestka_menu(self)
         set_load_density_menu(self)
         set_web_runner_menu(self)
+        set_install_menu(self)
         syntax_extend_package(self)
+        shell_manager.main_window = self
+        shell_manager.later_init()
         self.setWindowTitle("Automation Editor")
 
 
 def start_editor():
     new_editor = QApplication(sys.argv)
-    window = ITE()
+    window = AutomationEditor()
     apply_stylesheet(new_editor, theme='dark_amber.xml')
-    window.show()
+    window.showMaximized()
+    try:
+        window.startup_setting()
+    except Exception as error:
+        print(repr(error))
     sys.exit(new_editor.exec())
```

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,7 +87,8 @@
     webbrowser.open(url=url)
 
 
 def create_project():
     package = package_manager.installed_package_dict.get("je_api_testka", None)
     if package is not None:
         package.create_project_dir()
+
```

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,8 @@
 def open_web_browser(url: str):
     webbrowser.open(url=url)
 
 
 def create_project():
     package = package_manager.installed_package_dict.get("je_load_density", None)
     if package is not None:
-        package.create_project_dir()
+        package.create_project_dir()
```

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor_dev-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor_dev-0.0.6/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/exception/exception_tags.py` & `automation_editor_dev-0.0.6/automation_editor/utils/exception/exception_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 web_runner_test_executor_exception_tag: str = "can't run WebRunner"
 load_density_test_executor_exception_tag: str = "can't run LoadDensity"
 # Install
 not_install_exception: str = "Please install package first, Can't find package"
 # ui exception
 wrong_test_data_format_exception_tag: str = "get the wrong test data format"
 # exec exception
-exec_error: str = "ITE exec error"
+exec_error: str = "AutomationEditor exec error"
 file_not_fond_error: str = "File not found"
 compiler_not_found_error: str = "Compiler not found"
 not_install_package_error: str = "not install required package"
 # json exception
 cant_reformat_json_error: str = "Can't reformat json is type right?"
 wrong_json_data_error: str = "Can't parser json"
 # XML
```

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/exception/exceptions.py` & `automation_editor_dev-0.0.6/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor_dev-0.0.6/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/json_format/json_process.py` & `automation_editor_dev-0.0.6/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor_dev-0.0.6/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor_dev-0.0.6/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor_dev-0.0.6/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor_dev-0.0.6/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+import os
 import queue
 import shutil
 import subprocess
+import sys
 import threading
 import typing
+from pathlib import Path
 from queue import Queue
 from threading import Thread
 
 from PySide6.QtCore import QTimer
 from PySide6.QtWidgets import QTextEdit, QWidget
 from je_editor import error_color, output_color
 
+from automation_editor.utils.exception.exception_tags import compiler_not_found_error
+from automation_editor.utils.exception.exceptions import ITEExecException
+
 
 class TaskProcessManager(object):
     def __init__(
             self,
             main_window,
             task_done_trigger_function: typing.Callable = None,
             error_trigger_function: typing.Callable = None,
@@ -33,17 +39,39 @@
         self.process: [subprocess.Popen, None] = None
         self.task_done_trigger_function: typing.Callable = task_done_trigger_function
         self.error_trigger_function: typing.Callable = error_trigger_function
         self.program_buffer_size = program_buffer_size
 
     def start_test_process(self, package: str, exec_str: str):
         # try to find file and compiler
-        compiler_path = shutil.which("python")
+        if sys.platform in ["win32", "cygwin", "msys"]:
+            venv_path = Path(os.getcwd() + "/venv/Scripts")
+        else:
+            venv_path = Path(os.getcwd() + "/venv/bin")
+        if venv_path.is_dir() and venv_path.exists():
+            compiler_path = shutil.which(
+                cmd="python3",
+                path=str(venv_path)
+            )
+        else:
+            compiler_path = shutil.which(cmd="python3")
+        if compiler_path is None:
+            if sys.platform in ["win32", "cygwin", "msys"]:
+                venv_path = Path(os.getcwd() + "/venv/Scripts")
+            else:
+                venv_path = Path(os.getcwd() + "/venv/bin")
+            if venv_path.is_dir() and venv_path.exists():
+                compiler_path = shutil.which(
+                    cmd="python",
+                    path=str(venv_path)
+                )
+            else:
+                compiler_path = shutil.which(cmd="python")
         if compiler_path is None:
-            compiler_path = shutil.which("python3")
+            raise ITEExecException(compiler_not_found_error)
         self.process = subprocess.Popen(
             [
                 compiler_path,
                 "-m",
                 package,
                 "--execute_str",
                 exec_str
@@ -87,32 +115,35 @@
                 output_message = self.run_output_queue.get_nowait()
                 output_message = str(output_message).strip()
                 if output_message:
                     self.code_result.append(output_message)
         except queue.Empty:
             pass
         if self.process.returncode == 0:
+            self.timer.stop()
             self.exit_program()
         elif self.process.returncode is not None:
-            self.exit_program()
             self.timer.stop()
+            self.exit_program()
         if self.still_run_program:
             # poll return code
             self.process.poll()
 
     # exit program change run flag to false and clean read thread and queue and process
     def exit_program(self):
         self.still_run_program = False
         if self.read_program_output_from_thread is not None:
             self.read_program_output_from_thread = None
         if self.read_program_error_output_from_thread is not None:
             self.read_program_error_output_from_thread = None
         self.print_and_clear_queue()
         if self.process is not None:
             self.process.terminate()
+            print(f"Task exit with code {self.process.returncode}")
+            self.process = None
 
     def print_and_clear_queue(self):
         try:
             for std_output in iter(self.run_output_queue.get_nowait, None):
                 std_output = str(std_output).strip()
                 if std_output:
                     self.code_result.append(std_output)
```

### Comparing `automation_editor_dev-0.0.5/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor_dev-0.0.6/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.5/automation_editor_dev.egg-info/PKG-INFO` & `automation_editor_dev-0.0.6/automation_editor_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-editor-dev
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor_dev-0.0.5/automation_editor_dev.egg-info/SOURCES.txt` & `automation_editor_dev-0.0.6/automation_editor_dev.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 automation_editor/automation_editor_ui/editor_main/__init__.py
 automation_editor/automation_editor_ui/editor_main/main_ui.py
 automation_editor/automation_editor_ui/menu/__init__.py
 automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
 automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
 automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
 automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
 automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
 automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
 automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
 automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
 automation_editor/automation_editor_ui/show_code_window/__init__.py
 automation_editor/automation_editor_ui/show_code_window/code_window.py
 automation_editor/automation_editor_ui/syntax/__init__.py
```

### Comparing `automation_editor_dev-0.0.5/pyproject.toml` & `automation_editor_dev-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor_dev"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
-    "je-editor"
+    "je-editor", "je_auto_control", "je_web_runner",
+    "je_load_density", "je_api_testka"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Win32 (MS Windows)",
     "Environment :: MacOS X",
     "Environment :: X11 Applications",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [project.optional-dependencies]
 full_extension = [
-    "je-mail-thunder", "je_auto_control", "je_web_runner",
-    "je_load_density", "je_api_testka"
+    "je-mail-thunder"
 ]
 
 [project.urls]
 Homepage = "https://github.com/Intergration-Automation-Testing/AutomationEditor"
 Code = "https://github.com/Intergration-Automation-Testing/AutomationEditor"
 
 [project.readme]
```

