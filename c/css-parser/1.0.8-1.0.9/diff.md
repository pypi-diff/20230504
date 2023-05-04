# Comparing `tmp/css-parser-1.0.8.tar.gz` & `tmp/css-parser-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "css-parser-1.0.8.tar", last modified: Mon Sep 26 09:21:24 2022, max compression
+gzip compressed data, was "css-parser-1.0.9.tar", last modified: Thu May  4 03:54:13 2023, max compression
```

## Comparing `css-parser-1.0.8.tar` & `css-parser-1.0.9.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.018535 css-parser-1.0.8/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    35821 2019-06-03 11:54:12.000000 css-parser-1.0.8/COPYING
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7802 2019-06-03 11:54:12.000000 css-parser-1.0.8/COPYING.LESSER
--rw-r--r--   0 kovid     (1000) kovid     (1000)       90 2019-06-03 11:54:12.000000 css-parser-1.0.8/MANIFEST.in
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1684 2022-09-26 09:21:24.018535 css-parser-1.0.8/PKG-INFO
--rw-r--r--   0 kovid     (1000) kovid     (1000)      674 2021-06-26 06:23:57.000000 css-parser-1.0.8/README.md
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.008535 css-parser-1.0.8/css_parser_tests/
--rw-r--r--   0 kovid     (1000) kovid     (1000)       67 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10973 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/basetest.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.015202 css-parser-1.0.8/css_parser_tests/sheets/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4249 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/096.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4249 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/097.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       59 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       71 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1ascii.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       55 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1import.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       32 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1inherit-ascii.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       68 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1inherit-iso.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       30 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1inherit-utf8.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       65 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/1utf.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       39 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/2inherit-iso.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       36 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/2resolve.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9502 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/acid2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      264 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/all.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      137 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/atrule.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       73 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/bad.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       98 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/basic.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)   208303 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/bundle.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       83 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/cases.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       97 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/csscombine-1.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      111 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/csscombine-2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      220 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/csscombine-proxy.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3851 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/cthedot_default.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2797 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/default_html4.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      733 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/hacks.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      124 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/html.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1503 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/html20.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4274 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/html40.css
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.015202 css-parser-1.0.8/css_parser_tests/sheets/import/
--rw-r--r--   0 kovid     (1000) kovid     (1000)       88 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/import/import-impossible.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      427 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/import/import2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      113 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/import.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      307 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/import3.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9402 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/ll.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)    97995 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/ll2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       29 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/multiple-values.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       41 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/page_test.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)    17998 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/sample_5.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7662 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/sample_7.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      305 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/simple.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      113 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/single-color.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18645 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/slashcode.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      677 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/t-HACKS.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9268 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/test-unicode.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4369 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/test.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8665 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/tigris.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9082 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/tigris2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      296 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/u_simple.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       29 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/v_simple.css
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.015202 css-parser-1.0.8/css_parser_tests/sheets/var/
--rw-r--r--   0 kovid     (1000) kovid     (1000)      133 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/var/start.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      290 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/var/use.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       41 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/var/vars.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)       33 2019-06-03 12:00:28.000000 css-parser-1.0.8/css_parser_tests/sheets/var/vars2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      222 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/vars.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      254 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/varsimport.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4910 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/xhtml2.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4825 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/xhtml22.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)      117 2019-06-03 11:59:20.000000 css-parser-1.0.8/css_parser_tests/sheets/yuck.css
--rw-r--r--   0 kovid     (1000) kovid     (1000)    15611 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_codec.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4699 2022-05-21 15:29:25.000000 css-parser-1.0.8/css_parser_tests/test_csscharsetrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2283 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_csscomment.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8689 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssfontfacerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18701 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssimportrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18120 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssmediarule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9135 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssnamespacerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    14414 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_csspagerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2693 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_cssproperties.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8533 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_cssrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1211 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_cssrulelist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    23740 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssstyledeclaration.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9392 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssstylerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    34556 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssstylesheet.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5328 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssunknownrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18245 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssutils.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      715 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_cssutilsimport.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    33573 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_cssvalue.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    10677 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssvariablesdeclaration.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5402 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_cssvariablesrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1573 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_domimplementation.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    17162 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_encutils.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4703 2019-06-11 14:40:06.000000 css-parser-1.0.8/css_parser_tests/test_errorhandler.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3204 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_helper.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3430 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_marginrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7391 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_medialist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3635 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_mediaquery.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    20054 2020-01-08 04:18:04.000000 css-parser-1.0.8/css_parser_tests/test_parse.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    15475 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_prodparser.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    23338 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_profiles.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8410 2020-01-08 03:47:45.000000 css-parser-1.0.8/css_parser_tests/test_properties.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9366 2022-05-21 15:29:25.000000 css-parser-1.0.8/css_parser_tests/test_property.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2876 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_scripts_csscombine.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    16609 2022-05-21 15:29:25.000000 css-parser-1.0.8/css_parser_tests/test_selector.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4676 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_selectorlist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    29725 2022-09-26 09:11:15.000000 css-parser-1.0.8/css_parser_tests/test_serialize.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      958 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_settings.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1725 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_stylesheet.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    34664 2019-07-20 03:34:04.000000 css-parser-1.0.8/css_parser_tests/test_tokenize2.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    20296 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_util.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    45845 2021-12-31 00:13:24.000000 css-parser-1.0.8/css_parser_tests/test_value.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2188 2019-06-03 11:57:56.000000 css-parser-1.0.8/css_parser_tests/test_x.py
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     3394 2020-11-06 16:06:00.000000 css-parser-1.0.8/run_tests.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      129 2022-09-26 09:21:24.018535 css-parser-1.0.8/setup.cfg
--rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2424 2020-11-06 15:18:45.000000 css-parser-1.0.8/setup.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.005202 css-parser-1.0.8/src/
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.015202 css-parser-1.0.8/src/css_parser/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    16095 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    23783 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/_codec2.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    24413 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/_codec3.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2245 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/_fetch.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2674 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/_fetchgae.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      463 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/codec.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.018535 css-parser-1.0.8/src/css_parser/css/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2229 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/css/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6568 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/colors.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     6131 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/csscharsetrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2942 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/csscomment.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7177 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssfontfacerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    15119 2020-10-24 06:51:40.000000 css-parser-1.0.8/src/css_parser/css/cssimportrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    12909 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssmediarule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    11613 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssnamespacerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    16273 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/css/csspagerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5205 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssproperties.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    12361 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/css/cssrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2111 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssrulelist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    27508 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssstyledeclaration.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9606 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssstylerule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    34158 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/css/cssstylesheet.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8738 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssunknownrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    52667 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssvalue.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    12248 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssvariablesdeclaration.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7861 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/cssvariablesrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     7661 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/marginrule.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    18923 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/property.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    32793 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/selector.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8716 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/css/selectorlist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    38556 2020-10-24 06:54:44.000000 css-parser-1.0.8/src/css_parser/css/value.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4929 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/cssproductions.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.018535 css-parser-1.0.8/src/css_parser/encutils/
--rw-r--r--   0 kovid     (1000) kovid     (1000)    22996 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/encutils/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4218 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/errorhandler.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     4018 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/helper.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     8803 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/parse.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    28332 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/prodparser.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    35605 2020-01-08 03:39:16.000000 css-parser-1.0.8/src/css_parser/profiles.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    17366 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/sac.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    13146 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/script.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.018535 css-parser-1.0.8/src/css_parser/scripts/
--rw-r--r--   0 kovid     (1000) kovid     (1000)      170 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/scripts/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2438 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/scripts/csscapture.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     3183 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/scripts/csscombine.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     2170 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/scripts/cssparse.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    43022 2022-09-26 09:13:20.000000 css-parser-1.0.8/src/css_parser/serialize.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      631 2019-06-03 11:59:20.000000 css-parser-1.0.8/src/css_parser/settings.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.018535 css-parser-1.0.8/src/css_parser/stylesheets/
--rw-r--r--   0 kovid     (1000) kovid     (1000)      491 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/stylesheets/__init__.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9506 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/stylesheets/medialist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     9326 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/stylesheets/mediaquery.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5760 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/stylesheets/stylesheet.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1255 2019-06-03 12:00:28.000000 css-parser-1.0.8/src/css_parser/stylesheets/stylesheetlist.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    11880 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/tokenize2.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)    37174 2022-07-31 15:13:26.000000 css-parser-1.0.8/src/css_parser/util.py
--rw-r--r--   0 kovid     (1000) kovid     (1000)      214 2022-09-26 09:14:57.000000 css-parser-1.0.8/src/css_parser/version.py
-drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2022-09-26 09:21:24.015202 css-parser-1.0.8/src/css_parser.egg-info/
--rw-r--r--   0 kovid     (1000) kovid     (1000)     1684 2022-09-26 09:21:23.000000 css-parser-1.0.8/src/css_parser.egg-info/PKG-INFO
--rw-r--r--   0 kovid     (1000) kovid     (1000)     5623 2022-09-26 09:21:23.000000 css-parser-1.0.8/src/css_parser.egg-info/SOURCES.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2022-09-26 09:21:23.000000 css-parser-1.0.8/src/css_parser.egg-info/dependency_links.txt
--rw-r--r--   0 kovid     (1000) kovid     (1000)       11 2022-09-26 09:21:23.000000 css-parser-1.0.8/src/css_parser.egg-info/top_level.txt
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    35821 2019-06-03 11:54:12.000000 css-parser-1.0.9/COPYING
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7802 2019-06-03 11:54:12.000000 css-parser-1.0.9/COPYING.LESSER
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       90 2019-06-03 11:54:12.000000 css-parser-1.0.9/MANIFEST.in
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1684 2023-05-04 03:54:13.707885 css-parser-1.0.9/PKG-INFO
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      674 2021-06-26 06:23:57.000000 css-parser-1.0.9/README.md
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.704552 css-parser-1.0.9/css_parser_tests/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       67 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10973 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/basetest.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.704552 css-parser-1.0.9/css_parser_tests/sheets/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4249 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/096.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4249 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/097.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       59 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       71 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1ascii.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       55 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1import.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       32 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1inherit-ascii.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       68 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1inherit-iso.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       30 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1inherit-utf8.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       65 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/1utf.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       39 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/2inherit-iso.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       36 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/2resolve.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9502 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/acid2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      264 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/all.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      137 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/atrule.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       73 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/bad.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       98 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/basic.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)   208303 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/bundle.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       83 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/cases.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       97 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/csscombine-1.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      111 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/csscombine-2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      220 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/csscombine-proxy.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3851 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/cthedot_default.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2797 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/default_html4.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      733 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/hacks.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      124 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/html.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1503 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/html20.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4274 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/html40.css
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.704552 css-parser-1.0.9/css_parser_tests/sheets/import/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       88 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/import/import-impossible.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      427 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/import/import2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      113 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/import.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      307 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/import3.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9402 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/ll.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    97995 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/ll2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       29 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/multiple-values.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       41 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/page_test.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    17998 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/sample_5.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7662 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/sample_7.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      305 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/simple.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      113 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/single-color.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18645 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/slashcode.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      677 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/t-HACKS.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9268 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/test-unicode.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4369 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/test.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8665 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/tigris.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9082 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/tigris2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      296 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/u_simple.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       29 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/v_simple.css
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/css_parser_tests/sheets/var/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      133 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/var/start.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      290 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/var/use.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       41 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/var/vars.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       33 2019-06-03 12:00:28.000000 css-parser-1.0.9/css_parser_tests/sheets/var/vars2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      222 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/vars.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      254 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/varsimport.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4910 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/xhtml2.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4825 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/xhtml22.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      117 2019-06-03 11:59:20.000000 css-parser-1.0.9/css_parser_tests/sheets/yuck.css
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    15611 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_codec.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4699 2022-05-21 15:29:25.000000 css-parser-1.0.9/css_parser_tests/test_csscharsetrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2283 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_csscomment.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8689 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssfontfacerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18701 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssimportrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18120 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssmediarule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9135 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssnamespacerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    14414 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_csspagerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2693 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_cssproperties.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8533 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_cssrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1211 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_cssrulelist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    23740 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssstyledeclaration.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9392 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssstylerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    34556 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssstylesheet.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5328 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssunknownrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18245 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssutils.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      715 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_cssutilsimport.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    33573 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_cssvalue.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    10677 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssvariablesdeclaration.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5402 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_cssvariablesrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1573 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_domimplementation.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    17162 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_encutils.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4703 2019-06-11 14:40:06.000000 css-parser-1.0.9/css_parser_tests/test_errorhandler.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3204 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_helper.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3430 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_marginrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7391 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_medialist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3635 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_mediaquery.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    20054 2020-01-08 04:18:04.000000 css-parser-1.0.9/css_parser_tests/test_parse.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    15475 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_prodparser.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    23338 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_profiles.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8410 2020-01-08 03:47:45.000000 css-parser-1.0.9/css_parser_tests/test_properties.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9366 2022-05-21 15:29:25.000000 css-parser-1.0.9/css_parser_tests/test_property.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2876 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_scripts_csscombine.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    16609 2022-05-21 15:29:25.000000 css-parser-1.0.9/css_parser_tests/test_selector.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4676 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_selectorlist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    29725 2022-09-26 09:11:15.000000 css-parser-1.0.9/css_parser_tests/test_serialize.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      958 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_settings.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1725 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_stylesheet.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    34664 2019-07-20 03:34:04.000000 css-parser-1.0.9/css_parser_tests/test_tokenize2.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    20351 2023-05-04 03:31:56.000000 css-parser-1.0.9/css_parser_tests/test_util.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    45845 2021-12-31 00:13:24.000000 css-parser-1.0.9/css_parser_tests/test_value.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2188 2019-06-03 11:57:56.000000 css-parser-1.0.9/css_parser_tests/test_x.py
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     3394 2020-11-06 16:06:00.000000 css-parser-1.0.9/run_tests.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      129 2023-05-04 03:54:13.707885 css-parser-1.0.9/setup.cfg
+-rwxr-xr-x   0 kovid     (1000) kovid     (1000)     2424 2020-11-06 15:18:45.000000 css-parser-1.0.9/setup.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.701218 css-parser-1.0.9/src/
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    16095 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    23783 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/_codec2.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    24413 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/_codec3.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2245 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/_fetch.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2715 2023-05-04 03:28:03.000000 css-parser-1.0.9/src/css_parser/_fetchgae.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      463 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/codec.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser/css/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2229 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/css/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6568 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/colors.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     6131 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/csscharsetrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2942 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/csscomment.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7177 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssfontfacerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    15119 2020-10-24 06:51:40.000000 css-parser-1.0.9/src/css_parser/css/cssimportrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    12909 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssmediarule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    11613 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssnamespacerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    16273 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/css/csspagerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5205 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssproperties.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    12361 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/css/cssrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2111 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssrulelist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    27508 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssstyledeclaration.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9606 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssstylerule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    34158 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/css/cssstylesheet.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8738 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssunknownrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    52667 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssvalue.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    12248 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssvariablesdeclaration.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7861 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/cssvariablesrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     7661 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/marginrule.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    18923 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/property.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    32793 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/selector.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8716 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/css/selectorlist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    38556 2020-10-24 06:54:44.000000 css-parser-1.0.9/src/css_parser/css/value.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4929 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/cssproductions.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser/encutils/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    23145 2023-05-04 03:30:33.000000 css-parser-1.0.9/src/css_parser/encutils/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4218 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/errorhandler.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     4018 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/helper.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     8803 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/parse.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    28332 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/prodparser.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    35605 2020-01-08 03:39:16.000000 css-parser-1.0.9/src/css_parser/profiles.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    17366 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/sac.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    13146 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/script.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser/scripts/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      170 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/scripts/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2438 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/scripts/csscapture.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     3183 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/scripts/csscombine.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     2170 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/scripts/cssparse.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    43022 2022-09-26 09:13:20.000000 css-parser-1.0.9/src/css_parser/serialize.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      631 2019-06-03 11:59:20.000000 css-parser-1.0.9/src/css_parser/settings.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser/stylesheets/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      491 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/stylesheets/__init__.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9506 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/stylesheets/medialist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     9326 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/stylesheets/mediaquery.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5760 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/stylesheets/stylesheet.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1255 2019-06-03 12:00:28.000000 css-parser-1.0.9/src/css_parser/stylesheets/stylesheetlist.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    11880 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/tokenize2.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)    37174 2022-07-31 15:13:26.000000 css-parser-1.0.9/src/css_parser/util.py
+-rw-r--r--   0 kovid     (1000) kovid     (1000)      214 2023-05-04 03:53:44.000000 css-parser-1.0.9/src/css_parser/version.py
+drwxr-xr-x   0 kovid     (1000) kovid     (1000)        0 2023-05-04 03:54:13.707885 css-parser-1.0.9/src/css_parser.egg-info/
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     1684 2023-05-04 03:54:13.000000 css-parser-1.0.9/src/css_parser.egg-info/PKG-INFO
+-rw-r--r--   0 kovid     (1000) kovid     (1000)     5623 2023-05-04 03:54:13.000000 css-parser-1.0.9/src/css_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)        1 2023-05-04 03:54:13.000000 css-parser-1.0.9/src/css_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 kovid     (1000) kovid     (1000)       11 2023-05-04 03:54:13.000000 css-parser-1.0.9/src/css_parser.egg-info/top_level.txt
```

### Comparing `css-parser-1.0.8/COPYING` & `css-parser-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/COPYING.LESSER` & `css-parser-1.0.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/PKG-INFO` & `css-parser-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: css-parser
-Version: 1.0.8
+Version: 1.0.9
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/ebook-utils/css-parser
 Author: Various People
 Author-email: redacted@anonymous.net
 License: LGPL 3.0 or later
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `css-parser-1.0.8/README.md` & `css-parser-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/basetest.py` & `css-parser-1.0.9/css_parser_tests/basetest.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/096.css` & `css-parser-1.0.9/css_parser_tests/sheets/096.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/097.css` & `css-parser-1.0.9/css_parser_tests/sheets/097.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/acid2.css` & `css-parser-1.0.9/css_parser_tests/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/bundle.css` & `css-parser-1.0.9/css_parser_tests/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/cthedot_default.css` & `css-parser-1.0.9/css_parser_tests/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/default_html4.css` & `css-parser-1.0.9/css_parser_tests/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/hacks.css` & `css-parser-1.0.9/css_parser_tests/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/html20.css` & `css-parser-1.0.9/css_parser_tests/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/html40.css` & `css-parser-1.0.9/css_parser_tests/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/ll.css` & `css-parser-1.0.9/css_parser_tests/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/ll2.css` & `css-parser-1.0.9/css_parser_tests/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/sample_5.css` & `css-parser-1.0.9/css_parser_tests/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/sample_7.css` & `css-parser-1.0.9/css_parser_tests/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/slashcode.css` & `css-parser-1.0.9/css_parser_tests/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/t-HACKS.css` & `css-parser-1.0.9/css_parser_tests/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/test-unicode.css` & `css-parser-1.0.9/css_parser_tests/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/test.css` & `css-parser-1.0.9/css_parser_tests/sheets/test.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/tigris.css` & `css-parser-1.0.9/css_parser_tests/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/tigris2.css` & `css-parser-1.0.9/css_parser_tests/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/xhtml2.css` & `css-parser-1.0.9/css_parser_tests/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/sheets/xhtml22.css` & `css-parser-1.0.9/css_parser_tests/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_codec.py` & `css-parser-1.0.9/css_parser_tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_csscharsetrule.py` & `css-parser-1.0.9/css_parser_tests/test_csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_csscomment.py` & `css-parser-1.0.9/css_parser_tests/test_csscomment.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssfontfacerule.py` & `css-parser-1.0.9/css_parser_tests/test_cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssimportrule.py` & `css-parser-1.0.9/css_parser_tests/test_cssimportrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssmediarule.py` & `css-parser-1.0.9/css_parser_tests/test_cssmediarule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssnamespacerule.py` & `css-parser-1.0.9/css_parser_tests/test_cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_csspagerule.py` & `css-parser-1.0.9/css_parser_tests/test_csspagerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssproperties.py` & `css-parser-1.0.9/css_parser_tests/test_cssproperties.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssrule.py` & `css-parser-1.0.9/css_parser_tests/test_cssrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssrulelist.py` & `css-parser-1.0.9/css_parser_tests/test_cssrulelist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssstyledeclaration.py` & `css-parser-1.0.9/css_parser_tests/test_cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssstylerule.py` & `css-parser-1.0.9/css_parser_tests/test_cssstylerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssstylesheet.py` & `css-parser-1.0.9/css_parser_tests/test_cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssunknownrule.py` & `css-parser-1.0.9/css_parser_tests/test_cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssutils.py` & `css-parser-1.0.9/css_parser_tests/test_cssutils.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssutilsimport.py` & `css-parser-1.0.9/css_parser_tests/test_cssutilsimport.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssvalue.py` & `css-parser-1.0.9/css_parser_tests/test_cssvalue.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssvariablesdeclaration.py` & `css-parser-1.0.9/css_parser_tests/test_cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_cssvariablesrule.py` & `css-parser-1.0.9/css_parser_tests/test_cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_domimplementation.py` & `css-parser-1.0.9/css_parser_tests/test_domimplementation.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_encutils.py` & `css-parser-1.0.9/css_parser_tests/test_encutils.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_errorhandler.py` & `css-parser-1.0.9/css_parser_tests/test_errorhandler.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_helper.py` & `css-parser-1.0.9/css_parser_tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_marginrule.py` & `css-parser-1.0.9/css_parser_tests/test_marginrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_medialist.py` & `css-parser-1.0.9/css_parser_tests/test_medialist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_mediaquery.py` & `css-parser-1.0.9/css_parser_tests/test_mediaquery.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_parse.py` & `css-parser-1.0.9/css_parser_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_prodparser.py` & `css-parser-1.0.9/css_parser_tests/test_prodparser.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_profiles.py` & `css-parser-1.0.9/css_parser_tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_properties.py` & `css-parser-1.0.9/css_parser_tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_property.py` & `css-parser-1.0.9/css_parser_tests/test_property.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_scripts_csscombine.py` & `css-parser-1.0.9/css_parser_tests/test_scripts_csscombine.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_selector.py` & `css-parser-1.0.9/css_parser_tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_selectorlist.py` & `css-parser-1.0.9/css_parser_tests/test_selectorlist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_serialize.py` & `css-parser-1.0.9/css_parser_tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_settings.py` & `css-parser-1.0.9/css_parser_tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_stylesheet.py` & `css-parser-1.0.9/css_parser_tests/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_tokenize2.py` & `css-parser-1.0.9/css_parser_tests/test_tokenize2.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_util.py` & `css-parser-1.0.9/css_parser_tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, unicode_literals, with_statement
 
-import cgi
 import re
 import sys
 from contextlib import contextmanager
+from email.message import Message
 
 from css_parser.util import Base, LazyRegex, ListSeq, _defaultFetcher, _readUrl
 
 from . import basetest
 
 if sys.version_info.major > 2:
     from urllib.error import URLError, HTTPError
@@ -301,17 +301,18 @@
 
         class Response(object):
             """urllib2.Reponse mock"""
 
             def __init__(self, url, contenttype, content, exception=None, args=None):
                 self.url = url
 
-                mt, params = cgi.parse_header(contenttype)
-                self.mimetype = mt
-                self.charset = params.get('charset', None)
+                m = Message()
+                m['content-type'] = contenttype
+                self.mimetype = m.get_params()[0][0]
+                self.charset = m.get_param('charset')
 
                 self.text = content
 
                 self.exception = exception
                 self.args = args
 
             def geturl(self):
```

### Comparing `css-parser-1.0.8/css_parser_tests/test_value.py` & `css-parser-1.0.9/css_parser_tests/test_value.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/css_parser_tests/test_x.py` & `css-parser-1.0.9/css_parser_tests/test_x.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/run_tests.py` & `css-parser-1.0.9/run_tests.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/setup.py` & `css-parser-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/__init__.py` & `css-parser-1.0.9/src/css_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/_codec2.py` & `css-parser-1.0.9/src/css_parser/_codec2.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/_codec3.py` & `css-parser-1.0.9/src/css_parser/_codec3.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/_fetch.py` & `css-parser-1.0.9/src/css_parser/_fetch.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/_fetchgae.py` & `css-parser-1.0.9/src/css_parser/_fetchgae.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import unicode_literals, division, absolute_import, print_function
 from . import errorhandler
-import cgi
+from email.message import Message
 from google.appengine.api import urlfetch
+import sys
 """GAE specific URL reading functions"""
 
 
-import sys
 PY3 = sys.version_info[0] >= 3
 
 __all__ = ['_defaultFetcher']
 __docformat__ = 'restructuredtext'
 __version__ = '$Id: tokenize2.py 1547 2008-12-10 20:42:26Z cthedot $'
 
 # raises ImportError of not on GAE
@@ -56,16 +56,17 @@
         log.warn('Error opening url=%r: %s' % (url, e),
                  error=IOError)
     else:
         if r.status_code == 200:
             # find mimetype and encoding
             mimetype = 'application/octet-stream'
             try:
-                mimetype, params = cgi.parse_header(r.headers['content-type'])
-                encoding = params['charset']
+                m = Message()
+                m['content-type'] = r.headers['content-type']
+                encoding = m.get_param('charset')
             except KeyError:
                 encoding = None
             if mimetype != 'text/css':
                 log.error('Expected "text/css" mime type for url %r but found: %r' %
                           (url, mimetype), error=ValueError)
             return encoding, r.content
         else:
```

### Comparing `css-parser-1.0.8/src/css_parser/css/__init__.py` & `css-parser-1.0.9/src/css_parser/css/__init__.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/colors.py` & `css-parser-1.0.9/src/css_parser/css/colors.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/csscharsetrule.py` & `css-parser-1.0.9/src/css_parser/css/csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/csscomment.py` & `css-parser-1.0.9/src/css_parser/css/csscomment.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssfontfacerule.py` & `css-parser-1.0.9/src/css_parser/css/cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssimportrule.py` & `css-parser-1.0.9/src/css_parser/css/cssimportrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssmediarule.py` & `css-parser-1.0.9/src/css_parser/css/cssmediarule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssnamespacerule.py` & `css-parser-1.0.9/src/css_parser/css/cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/csspagerule.py` & `css-parser-1.0.9/src/css_parser/css/csspagerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssproperties.py` & `css-parser-1.0.9/src/css_parser/css/cssproperties.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssrule.py` & `css-parser-1.0.9/src/css_parser/css/cssrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssrulelist.py` & `css-parser-1.0.9/src/css_parser/css/cssrulelist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssstyledeclaration.py` & `css-parser-1.0.9/src/css_parser/css/cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssstylerule.py` & `css-parser-1.0.9/src/css_parser/css/cssstylerule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssstylesheet.py` & `css-parser-1.0.9/src/css_parser/css/cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssunknownrule.py` & `css-parser-1.0.9/src/css_parser/css/cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssvalue.py` & `css-parser-1.0.9/src/css_parser/css/cssvalue.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssvariablesdeclaration.py` & `css-parser-1.0.9/src/css_parser/css/cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/cssvariablesrule.py` & `css-parser-1.0.9/src/css_parser/css/cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/marginrule.py` & `css-parser-1.0.9/src/css_parser/css/marginrule.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/property.py` & `css-parser-1.0.9/src/css_parser/css/property.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/selector.py` & `css-parser-1.0.9/src/css_parser/css/selector.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/selectorlist.py` & `css-parser-1.0.9/src/css_parser/css/selectorlist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/css/value.py` & `css-parser-1.0.9/src/css_parser/css/value.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/cssproductions.py` & `css-parser-1.0.9/src/css_parser/cssproductions.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/encutils/__init__.py` & `css-parser-1.0.9/src/css_parser/encutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
     'detectXMLEncoding', 'getEncodingInfo', 'tryEncodings', 'EncodingInfo'
 ]
 __docformat__ = 'restructuredtext'
 __author__ = 'Christof Hoeke, Robert Siemer, Fredrik Hedman'
 __version__ = '$Id$'
 
 import sys
-import cgi
 import re
 import types
+from email.message import Message
 
 PY2x = sys.version_info < (3, 0)
 
 if PY2x:
     from StringIO import StringIO as io_StringIO
     from HTMLParser import HTMLParser as htmlparser_HTMLParser
     from HTMLParser import HTMLParseError as htmlparser_HTMLParseError
@@ -336,20 +336,25 @@
 
     try:
         p.feed(text)
     except htmlparser_HTMLParseError:
         pass
 
     if p.content_type:
-        media_type, params = cgi.parse_header(p.content_type)
-        encoding = params.get('charset')  # defaults to None
+        m = Message()
+        m['content-type'] = p.content_type
+        encoding = m.get_param('charset')  # defaults to None
         if encoding:
             encoding = encoding.lower()
         if log:
-            log.info('HTML META media_type: %s', media_type)
+            try:
+                media_type = m.get_params()[0][0]
+                log.info('HTML META media_type: %s', media_type)
+            except Exception:
+                pass
             log.info('HTML META encoding: %s', encoding)
     else:
         media_type = encoding = None
 
     return media_type, encoding
```

### Comparing `css-parser-1.0.8/src/css_parser/errorhandler.py` & `css-parser-1.0.9/src/css_parser/errorhandler.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/helper.py` & `css-parser-1.0.9/src/css_parser/helper.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/parse.py` & `css-parser-1.0.9/src/css_parser/parse.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/prodparser.py` & `css-parser-1.0.9/src/css_parser/prodparser.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/profiles.py` & `css-parser-1.0.9/src/css_parser/profiles.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/sac.py` & `css-parser-1.0.9/src/css_parser/sac.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/script.py` & `css-parser-1.0.9/src/css_parser/script.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/scripts/csscapture.py` & `css-parser-1.0.9/src/css_parser/scripts/csscapture.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/scripts/csscombine.py` & `css-parser-1.0.9/src/css_parser/scripts/csscombine.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/scripts/cssparse.py` & `css-parser-1.0.9/src/css_parser/scripts/cssparse.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/serialize.py` & `css-parser-1.0.9/src/css_parser/serialize.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/settings.py` & `css-parser-1.0.9/src/css_parser/settings.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/stylesheets/medialist.py` & `css-parser-1.0.9/src/css_parser/stylesheets/medialist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/stylesheets/mediaquery.py` & `css-parser-1.0.9/src/css_parser/stylesheets/mediaquery.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/stylesheets/stylesheet.py` & `css-parser-1.0.9/src/css_parser/stylesheets/stylesheet.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/stylesheets/stylesheetlist.py` & `css-parser-1.0.9/src/css_parser/stylesheets/stylesheetlist.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/tokenize2.py` & `css-parser-1.0.9/src/css_parser/tokenize2.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser/util.py` & `css-parser-1.0.9/src/css_parser/util.py`

 * *Files identical despite different names*

### Comparing `css-parser-1.0.8/src/css_parser.egg-info/PKG-INFO` & `css-parser-1.0.9/src/css_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: css-parser
-Version: 1.0.8
+Version: 1.0.9
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/ebook-utils/css-parser
 Author: Various People
 Author-email: redacted@anonymous.net
 License: LGPL 3.0 or later
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `css-parser-1.0.8/src/css_parser.egg-info/SOURCES.txt` & `css-parser-1.0.9/src/css_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

