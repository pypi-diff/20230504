# Comparing `tmp/toolium-3.0.0b1.tar.gz` & `tmp/toolium-3.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.0b1.tar", last modified: Tue Apr 25 13:22:15 2023, max compression
+gzip compressed data, was "toolium-3.0.1.dev0.tar", last modified: Thu May  4 10:44:52 2023, max compression
```

## Comparing `toolium-3.0.0b1.tar` & `toolium-3.0.1.dev0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.510889 toolium-3.0.0b1/
--rw-rw-rw-   0        0        0    29325 2023-04-25 10:06:44.000000 toolium-3.0.0b1/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.0b1/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     5523 2023-04-25 13:22:15.511892 toolium-3.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-04-04 16:24:15.000000 toolium-3.0.0b1/README.rst
--rw-rw-rw-   0        0        0        9 2023-04-15 11:17:06.000000 toolium-3.0.0b1/VERSION
--rw-rw-rw-   0        0        0      225 2023-04-11 07:34:47.000000 toolium-3.0.0b1/requirements.txt
--rw-rw-rw-   0        0        0      193 2023-04-11 07:34:47.000000 toolium-3.0.0b1/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-04-25 13:22:15.512892 toolium-3.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-04-04 16:24:15.000000 toolium-3.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.287892 toolium-3.0.0b1/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.319891 toolium-3.0.0b1/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12432 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    10586 2023-04-11 07:34:47.000000 toolium-3.0.0b1/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    21012 2023-04-17 09:39:11.000000 toolium-3.0.0b1/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/config_parser.py
--rw-rw-rw-   0        0        0    16655 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18000 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.398888 toolium-3.0.0b1/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.430889 toolium-3.0.0b1/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.0b1/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.449890 toolium-3.0.0b1/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8668 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.508891 toolium-3.0.0b1/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31093 2023-04-25 10:44:38.000000 toolium-3.0.0b1/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18455 2023-04-15 11:02:04.000000 toolium-3.0.0b1/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-03-27 14:34:03.000000 toolium-3.0.0b1/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    12916 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-04-04 16:24:15.000000 toolium-3.0.0b1/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:22:15.299890 toolium-3.0.0b1/toolium.egg-info/
--rw-rw-rw-   0        0        0     5523 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 13:22:15.000000 toolium-3.0.0b1/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.532363 toolium-3.0.1.dev0/
+-rw-rw-rw-   0        0        0    29812 2023-05-04 10:43:56.000000 toolium-3.0.1.dev0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.1.dev0/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.1.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5526 2023-05-04 10:44:52.532363 toolium-3.0.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/README.rst
+-rw-rw-rw-   0        0        0       12 2023-05-03 08:13:47.000000 toolium-3.0.1.dev0/VERSION
+-rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/requirements.txt
+-rw-rw-rw-   0        0        0      193 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-05-04 10:44:52.534369 toolium-3.0.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.301358 toolium-3.0.1.dev0/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev0/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.333359 toolium-3.0.1.dev0/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev0/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12432 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    10954 2023-05-04 10:43:56.000000 toolium-3.0.1.dev0/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21012 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.421359 toolium-3.0.1.dev0/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.451386 toolium-3.0.1.dev0/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.1.dev0/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.468364 toolium-3.0.1.dev0/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.1.dev0/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.1.dev0/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.1.dev0/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8668 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.529363 toolium-3.0.1.dev0/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    31951 2023-05-04 09:53:15.000000 toolium-3.0.1.dev0/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.1.dev0/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:44:52.315355 toolium-3.0.1.dev0/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5526 2023-05-04 10:44:52.000000 toolium-3.0.1.dev0/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-04 10:44:52.000000 toolium-3.0.1.dev0/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:44:52.000000 toolium-3.0.1.dev0/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-05-04 10:44:52.000000 toolium-3.0.1.dev0/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 10:44:52.000000 toolium-3.0.1.dev0/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.0b1/CHANGELOG.rst` & `toolium-3.0.1.dev0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Toolium Changelog
 =================
 
-v3.0.0
+v3.0.1
 ------
 
 *Release date: In development*
 
+- Allow to search in `context.storage` using `[CONTEXT:a.b.c]` replacement when `before_feature` method is not used
+- Execute after scenario methods also when a scenario is skipped to assure that scenario preconditions are cleaned
+
+v3.0.0
+------
+
+*Release date: 2023-05-03*
+
 - Add support for Python 3.11
 - Add support for Selenium 4
 - Add support for Appium-Python-Client 2
 - Visual testing comparison has changed
 
    | It only needs PIL library to compare images and generate the differences images
    | Old PerceptualDiff and Magick engines have been removed
@@ -18,19 +26,21 @@
 
 - Now `gecko_driver_path`, `chrome_driver_path`, `explorer_driver_path` and `edge_driver_path` config properties
   in [Driver] section are optional, due to new SeleniumManager feature, that downloads drivers automatically
 - New optional config property `safari_driver_path` in [Driver] section to configure Safari driver
 - New optional config property `options` in [Chrome] section to configure Chrome options instead of using old
   property `goog:chromeOptions` in [Capabilities] section.
 - New optional config property `base_path` in [Server] section to allow using old Selenium 3 or Appium 1 remote servers
-- Update [RANDOM_PHONE_NUMBER] replacement using new `DataGenerator` class
 - Remove support for lettuce tests
 - Remove deprecated parameter `context` from `map_param` and POEditor methods
 - Remove deprecated config property `restart_driver_fail` in [Driver] section
 - Remove deprecated environment variables `Section_option`, `Config_environment` and `env`
+- Update `[RANDOM_PHONE_NUMBER]` replacement using new `DataGenerator` class
+- Update `[CONTEXT:a.b.c]` replacement to search data in context, context.storage and context.feature_storage
+- Update `[CONTEXT:a.b.c]` replacement to allow dictionaries or classes in context fields
 
 v2.7.0
 ------
 
 *Release date: 2023-02-24*
 
 - Fix drivers not being closed in `after_feature` when errors occur during `before_feature` steps execution
```

### Comparing `toolium-3.0.0b1/LICENSE` & `toolium-3.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/PKG-INFO` & `toolium-3.0.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.0b1
+Version: 3.0.1.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.0b1/README.rst` & `toolium-3.0.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/setup.py` & `toolium-3.0.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/behave/env_utils.py` & `toolium-3.0.1.dev0/toolium/behave/env_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/behave/environment.py` & `toolium-3.0.1.dev0/toolium/behave/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
     if context.toolium_config.getboolean_optional('Driver', 'reuse_driver') or context.reuse_driver_from_tags:
         no_driver = 'no_driver' in feature.tags
         start_driver(context, no_driver)
 
     # Behave dynamic environment
     context.dyn_env.get_steps_from_feature_description(feature.description)
     context.dyn_env.execute_before_feature_steps(context)
+    # Dictionary to store information between steps
+    context.storage = dict()
+    # Dictionary to store information between features
+    context.feature_storage = dict()
 
 
 def before_scenario(context, scenario):
     """Scenario initialization
 
     :param context: behave context
     :param scenario: running scenario
@@ -122,14 +126,16 @@
     # Configure Jira properties
     save_jira_conf()
 
     context.logger.info("Running new scenario: %s", scenario.name)
 
     # Behave dynamic environment
     context.dyn_env.execute_before_scenario_steps(context)
+    # Make sure storage dict are empty
+    context.storage = dict()
 
 
 def create_and_configure_wrapper(context):
     """Create and configure driver wrapper in behave tests
 
     :param context: behave context
     """
@@ -197,31 +203,32 @@
 def after_scenario(context, scenario):
     """Clean method that will be executed after each scenario
 
     :param context: behave context
     :param scenario: running scenario
     """
     if scenario.status == 'skipped':
-        return
+        context.logger.info("The scenario '%s' has been skipped", scenario.name)
     elif scenario.status == 'passed':
         test_status = 'Pass'
         test_comment = None
         context.logger.info("The scenario '%s' has passed", scenario.name)
     else:
         test_status = 'Fail'
         test_comment = "The scenario '%s' has failed" % scenario.name
         context.logger.error("The scenario '%s' has failed", scenario.name)
         context.global_status['test_passed'] = False
 
     # Close drivers
-    DriverWrappersPool.close_drivers(scope='function', test_name=scenario.name, test_passed=scenario.status == 'passed',
-                                     context=context)
+    DriverWrappersPool.close_drivers(scope='function', test_name=scenario.name,
+                                     test_passed=scenario.status in ['passed', 'skipped'], context=context)
 
     # Save test status to be updated later
-    add_jira_status(get_jira_key_from_scenario(scenario), test_status, test_comment)
+    if scenario.status != 'skipped':
+        add_jira_status(get_jira_key_from_scenario(scenario), test_status, test_comment)
 
 
 def get_jira_key_from_scenario(scenario):
     """Extract Jira Test Case key from scenario tags.
     Two tag formats are allowed:
     @jira('PROJECT-32')
     @jira=PROJECT-32
```

### Comparing `toolium-3.0.0b1/toolium/config_driver.py` & `toolium-3.0.1.dev0/toolium/config_driver.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/config_files.py` & `toolium-3.0.1.dev0/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/config_parser.py` & `toolium-3.0.1.dev0/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/driver_wrapper.py` & `toolium-3.0.1.dev0/toolium/driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/driver_wrappers_pool.py` & `toolium-3.0.1.dev0/toolium/driver_wrappers_pool.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/jira.py` & `toolium-3.0.1.dev0/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/__init__.py` & `toolium-3.0.1.dev0/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/button_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/checkbox_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/group_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/input_radio_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/input_text_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/link_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/page_elements.py` & `toolium-3.0.1.dev0/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/select_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageelements/text_page_element.py` & `toolium-3.0.1.dev0/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageobjects/common_object.py` & `toolium-3.0.1.dev0/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageobjects/mobile_page_object.py` & `toolium-3.0.1.dev0/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pageobjects/page_object.py` & `toolium-3.0.1.dev0/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/pytest_fixtures.py` & `toolium-3.0.1.dev0/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/resources/VisualTests.css` & `toolium-3.0.1.dev0/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/resources/VisualTests.js` & `toolium-3.0.1.dev0/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/resources/VisualTestsTemplate.html` & `toolium-3.0.1.dev0/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/selenoid.py` & `toolium-3.0.1.dev0/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/test_cases.py` & `toolium-3.0.1.dev0/toolium/test_cases.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/data_generator.py` & `toolium-3.0.1.dev0/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/dataset.py` & `toolium-3.0.1.dev0/toolium/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import base64
+import collections
 import datetime
 import json
 import logging
 import os
 import random as r
 import re
 import string
@@ -367,15 +368,15 @@
 
     :param param: string parameter
     :return: string with the applied replacements
     """
     if not isinstance(param, str):
         return param
 
-    map_regex = r"[\[CONF:|\[LANG:|\[POE:|\[ENV:|\[BASE64:|\[TOOLIUM:|\[CONTEXT:|\[FILE:][a-zA-Z\.\:\/\_\-\ 0-9]*\]"
+    map_regex = r"[\[CONF:|\[LANG:|\[POE:|\[ENV:|\[BASE64:|\[TOOLIUM:|\[CONTEXT:|\[FILE:][^\[\]]*\]"
     map_expressions = re.compile(map_regex)
 
     mapped_param = param
     if map_expressions.split(param) == ['', '']:
         # The parameter is just one config value
         mapped_param = map_one_param(param)
     else:
@@ -569,54 +570,71 @@
         logger.error(msg)
         raise Exception(msg)
     return mapped_value
 
 
 def get_value_from_context(param, context):
     """
-    Find the value of the given param using it as a key in the context storage dictionary (context.storage) or in the
-    context object itself. The key might be comprised of dotted tokens. In such case, the searched key is the first
-    token. The rest of the tokens are considered nested properties/objects.
+    Find the value of the given param using it as a key in the context storage dictionaries (context.storage or
+    context.feature_storage) or in the context object itself. The key might be comprised of dotted tokens. In such case,
+    the searched key is the first token. The rest of the tokens are considered nested properties/objects.
     So, for example, in the basic case, "last_request_result" could be used as key that would be searched into context
-    storage or the context object itself. In a dotted case, "last_request.result" is searched as a "last_request" key
-    in the context storage or as a property of the context object whose name is last_request. In both cases, when found,
-    "result" is considered (and resolved) as a property into the returned value.
+    storages or the context object itself. In a dotted case, "last_request.result" is searched as a "last_request" key
+    in the context storages or as a property of the context object whose name is last_request. In both cases, when
+    found, "result" is considered (and resolved) as a property or a key into the returned value.
 
     There is not limit in the nested levels of dotted tokens, so a key like a.b.c.d will be tried to be resolved as:
 
     context.storage['a'].b.c.d
         or
     context.a.b.c.d
 
     :param param: key to be searched (e.g. "last_request_result" / "last_request.result")
-    :param context: Behave context object
+    :param context: behave context
     :return: mapped value
     """
     parts = param.split('.')
-    value = None
-    if context.storage and parts[0] in context.storage:
-        value = context.storage[parts[0]]
-    else:
-        logger.debug(f"'{parts[0]}' key not found in context storage, searching in context")
-        try:
-            value = getattr(context, parts[0])
-        except AttributeError:
-            msg = f"'{parts[0]}' not found neither in context storage nor in context"
-            logger.error(msg)
-            raise AttributeError(msg)
+    value = _get_initial_value_from_context(parts[0], context)
 
-    if len(parts) > 1:
-        try:
-            for part in parts[1:]:
-                value = getattr(value, part)
-        except AttributeError:
-            msg = f"'{part}' is not an attribute of {value}"
+    for part in parts[1:]:
+        if isinstance(value, dict) and part in value:
+            value = value[part]
+        elif hasattr(value, part):
+            value = getattr(value, part)
+        else:
+            if isinstance(value, dict):
+                msg = f"'{part}' key not found in {value} value in context"
+            else:
+                msg = f"'{part}' attribute not found in {type(value).__name__} class in context"
             logger.error(msg)
-            raise AttributeError(msg)
+            raise Exception(msg)
+    return value
+
 
+def _get_initial_value_from_context(initial_key, context):
+    """
+    Find the value of the given initial_key using it as a key in the context storage dictionaries (context.storage or
+    context.feature_storage) or in the context object itself.
+
+    :param initial_key: key to be searched in context
+    :param context: behave context
+    :return: mapped value
+    """
+    context_storage = context.storage if hasattr(context, 'storage') else {}
+    if hasattr(context, 'feature_storage'):
+        # context.feature_storage is initialized only when before_feature method is called
+        context_storage = collections.ChainMap(context.storage, context.feature_storage)
+    if initial_key in context_storage:
+        value = context_storage[initial_key]
+    elif hasattr(context, initial_key):
+        value = getattr(context, initial_key)
+    else:
+        msg = f"'{initial_key}' key not found in context"
+        logger.error(msg)
+        raise Exception(msg)
     return value
 
 
 def get_message_property(param, language_terms, language_key):
     """
     Return the message for the given param, using it as a key in the list of language properties.
     Dot notation is used (e.g. "home.button.send").
```

### Comparing `toolium-3.0.0b1/toolium/utils/download_files.py` & `toolium-3.0.1.dev0/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/driver_utils.py` & `toolium-3.0.1.dev0/toolium/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/driver_wait_utils.py` & `toolium-3.0.1.dev0/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/path_utils.py` & `toolium-3.0.1.dev0/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/utils/poeditor.py` & `toolium-3.0.1.dev0/toolium/utils/poeditor.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium/visual_test.py` & `toolium-3.0.1.dev0/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.0b1/toolium.egg-info/PKG-INFO` & `toolium-3.0.1.dev0/toolium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.0b1
+Version: 3.0.1.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.0b1/toolium.egg-info/SOURCES.txt` & `toolium-3.0.1.dev0/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

