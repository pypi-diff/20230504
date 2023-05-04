# Comparing `tmp/zpretty-3.0.4.tar.gz` & `tmp/zpretty-3.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpretty-3.0.4.tar", last modified: Thu Apr 20 13:32:40 2023, max compression
+gzip compressed data, was "zpretty-3.1.0a1.tar", last modified: Thu May  4 07:33:37 2023, max compression
```

## Comparing `zpretty-3.0.4.tar` & `zpretty-3.1.0a1.tar`

### file list

```diff
@@ -1,57 +1,92 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/
--rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-04-20 13:32:40.000000 zpretty-3.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-04-20 13:32:40.000000 zpretty-3.0.4/.pre-commit-hooks.yaml
--rw-rw-r--   0 ale       (1000) ale       (1000)     3785 2023-04-20 13:32:40.000000 zpretty-3.0.4/HISTORY.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-04-20 13:32:40.000000 zpretty-3.0.4/LICENSE
--rw-rw-r--   0 ale       (1000) ale       (1000)      196 2023-04-20 13:32:40.000000 zpretty-3.0.4/MANIFEST.in
--rw-rw-r--   0 ale       (1000) ale       (1000)      808 2023-04-20 13:32:40.000000 zpretty-3.0.4/Makefile
--rw-rw-r--   0 ale       (1000) ale       (1000)     8453 2023-04-20 13:32:40.178341 zpretty-3.0.4/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     3760 2023-04-20 13:32:40.000000 zpretty-3.0.4/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-04-20 13:32:40.000000 zpretty-3.0.4/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements-dev.txt
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.174341 zpretty-3.0.4/requirements.d/
--rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements.d/requirements-dev-37.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-04-20 13:32:40.000000 zpretty-3.0.4/requirements.d/requirements-dev.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-04-20 13:32:40.178341 zpretty-3.0.4/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1563 2023-04-20 13:32:40.000000 zpretty-3.0.4/setup.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-04-20 13:32:40.000000 zpretty-3.0.4/tox.ini
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7077 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4537 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     5242 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/prettifier.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/broken/
--rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/broken/broken.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/mock.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty/tests/original/
--rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample.zcml
--rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_dtml.dtml
--rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html4.html
--rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
--rw-rw-r--   0 ale       (1000) ale       (1000)     1283 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_pt.pt
--rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/sample_xml.xml
--rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/original/text_with_markup.md
--rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_attributes.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3241 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_cli.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_elements.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_functions.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_readme.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_zcml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     7763 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/tests/test_zpretty.py
--rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/text.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/xml.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty/zcml.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-04-20 13:32:40.178341 zpretty-3.0.4/zpretty.egg-info/
--rw-rw-r--   0 ale       (1000) ale       (1000)     8453 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1290 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/entry_points.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-04-20 13:32:40.000000 zpretty-3.0.4/zpretty.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      565 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/.pre-commit-config.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      176 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/.pre-commit-hooks.yaml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4014 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/HISTORY.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1387 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/LICENSE
+-rw-rw-r--   0 ale       (1000) ale       (1000)      238 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)      808 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/Makefile
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10506 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5582 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)      325 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      106 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements-dev.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/requirements.d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      865 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements.d/requirements-dev-37.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1036 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/requirements.d/requirements-dev.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      289 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1565 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/setup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      863 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/tox.ini
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7728 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     8249 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13179 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5242 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/prettifier.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/broken/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/broken/broken.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/.venv/foo.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/foo/bar/foo.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/bar.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/include-exclude/venv/foo.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      175 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/mock.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.714950 zpretty-3.1.0a1/zpretty/tests/original/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       47 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1587 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      272 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_dtml.dtml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1890 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1938 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html4.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)      366 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_html_with_preprocessing_instruction.html
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1504 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_pt.pt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      667 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/sample_xml.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      126 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/original/text_with_markup.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2728 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_attributes.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7639 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_cli.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4423 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_elements.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      952 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_functions.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1908 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_readme.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1399 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7715 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_zcml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7763 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/tests/test_zpretty.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      943 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/text.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2580 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/xml.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    24594 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty/zcml.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-05-04 07:33:37.710950 zpretty-3.1.0a1/zpretty.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10506 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2626 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       44 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2023-05-04 07:33:37.000000 zpretty-3.1.0a1/zpretty.egg-info/top_level.txt
```

### Comparing `zpretty-3.0.4/.pre-commit-config.yaml` & `zpretty-3.1.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/HISTORY.md` & `zpretty-3.1.0a1/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 3.1.0a1 (2023-05-04)
+
+- Add command line parameters to include/exclude files and folders
+  (Implements #96)
+  [ale-rt]  
+- Be tolerant with characters forbidden in XML when dealing with tal attributes
+  (See #125)
+  [ale-rt]
+
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
   (Fixes #116)
   [ale-rt]
 
 ## 3.0.3 (2023-03-26)
```

### Comparing `zpretty-3.0.4/LICENSE` & `zpretty-3.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/Makefile` & `zpretty-3.1.0a1/Makefile`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/PKG-INFO` & `zpretty-3.1.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.0.4
+Version: 3.1.0a1
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,29 +84,57 @@
 # USAGE
 
 Basic usage:
 
 ```console
 $ zpretty -h
 usage: zpretty [-h] [--encoding ENCODING] [-i] [-v] [-x] [-z] [--check]
+               [--include INCLUDE] [--exclude EXCLUDE]
+               [--extend-exclude EXTEND_EXCLUDE]
                [paths ...]
 
 positional arguments:
-    paths                The list of paths to prettify (defaults to stdin)
+  paths                 The list of files or directory to prettify (defaults to
+                        stdin). If a directory is passed, all files and
+                        directories matching the regular expression passed to
+                        --include will be prettified.
 
 options:
-    -h, --help           show this help message and exit
-    --encoding ENCODING  The file encoding (defaults to utf8)
-    -i, --inplace        Format files in place (overwrite existing file)
-    -v, --version        Show zpretty version number
-    -x, --xml            Treat the input file(s) as XML
-    -z, --zcml           Treat the input file(s) as XML. Follow the ZCML
+  -h, --help            show this help message and exit
+  --encoding ENCODING   The file encoding (defaults to utf8)
+  -i, --inplace         Format files in place (overwrite existing file)
+  -v, --version         Show zpretty version number
+  -x, --xml             Treat the input file(s) as XML
+  -z, --zcml            Treat the input file(s) as XML. Follow the ZCML
                         styleguide
-    --check              Return code 0 if nothing would be changed, 1 if some
+  --check               Return code 0 if nothing would be changed, 1 if some
                         files would be reformatted
+  --include INCLUDE     A regular expression that matches files and directories
+                        that should be included on recursive searches. An empty
+                        value means all files are included regardless of the
+                        name. Use forward slashes for directories on all
+                        platforms (Windows, too). Exclusions are calculated
+                        first, inclusions later. [default:
+                        \.(html|pt|xml|zcml)$]
+  --exclude EXCLUDE     A regular expression that matches files and directories
+                        that should be excluded on recursive searches. An empty
+                        value means no paths are excluded. Use forward slashes
+                        for directories on all platforms (Windows, too).
+                        Exclusions are calculated first, inclusions later.
+                        [default: /(\.direnv|\.eggs|\.git|\.hg|\.mypy_cache|\.no
+                        x|\.tox|\.venv|venv|\.svn|\.ipynb_checkpoints|_build|buc
+                        k-out|build|dist|__pypackages__)/]
+  --extend-exclude EXTEND_EXCLUDE
+                        Like --exclude, but adds additional files and
+                        directories on top of the excluded ones. (Useful if you
+                        simply want to add to the default)
+
+The default exclude pattern is: `/(\.direnv|\.eggs|\.git|\.hg|\.mypy_cache|\.nox
+|\.tox|\.venv|venv|\.svn|\.ipynb_checkpoints|_build|buck-
+out|build|dist|__pypackages__)/`
 ```
 
 Without parameters constraining the file type (e.g. `-x`, `-z`, \...)
 `zpretty` will try to guess the right options for you.
 
 Example:
 
@@ -146,14 +174,23 @@
 
 ```bash
 make test
 ```
 
 # Changelog
 
+## 3.1.0a1 (2023-05-04)
+
+- Add command line parameters to include/exclude files and folders
+  (Implements #96)
+  [ale-rt]  
+- Be tolerant with characters forbidden in XML when dealing with tal attributes
+  (See #125)
+  [ale-rt]
+
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
   (Fixes #116)
   [ale-rt]
 
 ## 3.0.3 (2023-03-26)
```

### Comparing `zpretty-3.0.4/requirements.d/requirements-dev-37.txt` & `zpretty-3.1.0a1/requirements.d/requirements-dev-37.txt`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/requirements.d/requirements-dev.txt` & `zpretty-3.1.0a1/requirements.d/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/setup.py` & `zpretty-3.1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name="zpretty",
-    version="3.0.4",
+    version="3.1.0a1",
     description="An opinionated HTML/XML soup formatter",
     keywords=["Formatter", "HTML", "Prettifier", "Pretty print", "TAL", "XML", "ZPT"],
     long_description="\n".join((read("README.md"), read("HISTORY.md"))),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `zpretty-3.0.4/tox.ini` & `zpretty-3.1.0a1/tox.ini`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/attributes.py` & `zpretty-3.1.0a1/zpretty/attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,34 @@
         # ... and at the end dedent
         lines.append(line_prefix[:-2])
 
         new_value = "\n".join(lines)
         # restore ';;'
         return new_value.replace("<>", ";;")
 
+    def is_tal_attribute(self, name):
+        """Check if the attribute is a tal attribute"""
+        if name.startswith("tal:"):
+            return True
+        try:
+            if not self.element.context.name.startswith("tal:"):
+                return False
+        except AttributeError:
+            return False
+        if f"tal:{name}" in self._tal_attribute_order:
+            return True
+
+    def maybe_escape(self, name, value):
+        """Escape the value if needed"""
+        if self.is_tal_attribute(name):
+            # Never escape what we have in tal attributes
+            return value
+
+        return escape(value, quote=False)
+
     def can_be_valueless(self, name):
         """Check if the attribute name can be without a value"""
         if not self._boolean_attributes_are_allowed:
             return False
         if name.startswith("data-"):
             return True
         if name in self._known_boolean_attributes:
@@ -207,16 +227,17 @@
             if not value and self.can_be_valueless(name):
                 line = name
             else:
                 if '"' in value:
                     quote = "'"
                 else:
                     quote = '"'
+
                 line = self._attribute_template.format(
-                    name=name, quote=quote, value=escape(value, quote=False)
+                    name=name, quote=quote, value=self.maybe_escape(name, value)
                 )
             lines.append(line)
         return lines
 
     def lstrip(self):
         """This returns the attributes with the left spaces removed"""
         return self().lstrip()
```

### Comparing `zpretty-3.0.4/zpretty/elements.py` & `zpretty-3.1.0a1/zpretty/elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/prettifier.py` & `zpretty-3.1.0a1/zpretty/prettifier.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/original/sample.zcml` & `zpretty-3.1.0a1/zpretty/tests/original/sample.zcml`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/original/sample_html.html` & `zpretty-3.1.0a1/zpretty/tests/original/sample_html.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/original/sample_html4.html` & `zpretty-3.1.0a1/zpretty/tests/original/sample_html4.html`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/original/sample_pt.pt` & `zpretty-3.1.0a1/zpretty/tests/original/sample_pt.pt`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,20 @@
         "<c href="#">whatever</c>"
         <pre>
           Foo
             Bar
         </pre>
         <span tal:define="
                 foo python: 1 &gt; 2 and 1 &lt; 2 and &amp;;
+                bar python: 1 > 2 and 1 < 2 and &;
               "></span>
+        <tal:span define="
+                    foo python: 1 &gt; 2 and 1 &lt; 2 and &amp;;
+                    bar python: 1 > 2 and 1 < 2 and &;
+                  " />
       </metal:content-core>
     </metal:main>
     <![CDATA[
       This
         should
           be
```

### Comparing `zpretty-3.0.4/zpretty/tests/original/sample_xml.xml` & `zpretty-3.1.0a1/zpretty/tests/original/sample_xml.xml`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_attributes.py` & `zpretty-3.1.0a1/zpretty/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_elements.py` & `zpretty-3.1.0a1/zpretty/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_functions.py` & `zpretty-3.1.0a1/zpretty/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_readme.py` & `zpretty-3.1.0a1/zpretty/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_xml.py` & `zpretty-3.1.0a1/zpretty/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_zcml.py` & `zpretty-3.1.0a1/zpretty/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/tests/test_zpretty.py` & `zpretty-3.1.0a1/zpretty/tests/test_zpretty.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/text.py` & `zpretty-3.1.0a1/zpretty/text.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/xml.py` & `zpretty-3.1.0a1/zpretty/xml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty/zcml.py` & `zpretty-3.1.0a1/zpretty/zcml.py`

 * *Files identical despite different names*

### Comparing `zpretty-3.0.4/zpretty.egg-info/PKG-INFO` & `zpretty-3.1.0a1/zpretty.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpretty
-Version: 3.0.4
+Version: 3.1.0a1
 Summary: An opinionated HTML/XML soup formatter
 Home-page: https://github.com/collective/zpretty
 Author: Alessandro Pisa
 Author-email: alessandro.pisa@gmail.com
 License: BSD
 Keywords: Formatter,HTML,Prettifier,Pretty print,TAL,XML,ZPT
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,29 +84,57 @@
 # USAGE
 
 Basic usage:
 
 ```console
 $ zpretty -h
 usage: zpretty [-h] [--encoding ENCODING] [-i] [-v] [-x] [-z] [--check]
+               [--include INCLUDE] [--exclude EXCLUDE]
+               [--extend-exclude EXTEND_EXCLUDE]
                [paths ...]
 
 positional arguments:
-    paths                The list of paths to prettify (defaults to stdin)
+  paths                 The list of files or directory to prettify (defaults to
+                        stdin). If a directory is passed, all files and
+                        directories matching the regular expression passed to
+                        --include will be prettified.
 
 options:
-    -h, --help           show this help message and exit
-    --encoding ENCODING  The file encoding (defaults to utf8)
-    -i, --inplace        Format files in place (overwrite existing file)
-    -v, --version        Show zpretty version number
-    -x, --xml            Treat the input file(s) as XML
-    -z, --zcml           Treat the input file(s) as XML. Follow the ZCML
+  -h, --help            show this help message and exit
+  --encoding ENCODING   The file encoding (defaults to utf8)
+  -i, --inplace         Format files in place (overwrite existing file)
+  -v, --version         Show zpretty version number
+  -x, --xml             Treat the input file(s) as XML
+  -z, --zcml            Treat the input file(s) as XML. Follow the ZCML
                         styleguide
-    --check              Return code 0 if nothing would be changed, 1 if some
+  --check               Return code 0 if nothing would be changed, 1 if some
                         files would be reformatted
+  --include INCLUDE     A regular expression that matches files and directories
+                        that should be included on recursive searches. An empty
+                        value means all files are included regardless of the
+                        name. Use forward slashes for directories on all
+                        platforms (Windows, too). Exclusions are calculated
+                        first, inclusions later. [default:
+                        \.(html|pt|xml|zcml)$]
+  --exclude EXCLUDE     A regular expression that matches files and directories
+                        that should be excluded on recursive searches. An empty
+                        value means no paths are excluded. Use forward slashes
+                        for directories on all platforms (Windows, too).
+                        Exclusions are calculated first, inclusions later.
+                        [default: /(\.direnv|\.eggs|\.git|\.hg|\.mypy_cache|\.no
+                        x|\.tox|\.venv|venv|\.svn|\.ipynb_checkpoints|_build|buc
+                        k-out|build|dist|__pypackages__)/]
+  --extend-exclude EXTEND_EXCLUDE
+                        Like --exclude, but adds additional files and
+                        directories on top of the excluded ones. (Useful if you
+                        simply want to add to the default)
+
+The default exclude pattern is: `/(\.direnv|\.eggs|\.git|\.hg|\.mypy_cache|\.nox
+|\.tox|\.venv|venv|\.svn|\.ipynb_checkpoints|_build|buck-
+out|build|dist|__pypackages__)/`
 ```
 
 Without parameters constraining the file type (e.g. `-x`, `-z`, \...)
 `zpretty` will try to guess the right options for you.
 
 Example:
 
@@ -146,14 +174,23 @@
 
 ```bash
 make test
 ```
 
 # Changelog
 
+## 3.1.0a1 (2023-05-04)
+
+- Add command line parameters to include/exclude files and folders
+  (Implements #96)
+  [ale-rt]  
+- Be tolerant with characters forbidden in XML when dealing with tal attributes
+  (See #125)
+  [ale-rt]
+
 ## 3.0.4 (2023-04-20)
 
 - Fix bogus ampersands in attributes
   (Fixes #116)
   [ale-rt]
 
 ## 3.0.3 (2023-03-26)
```

