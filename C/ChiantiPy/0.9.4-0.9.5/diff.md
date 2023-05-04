# Comparing `tmp/ChiantiPy-0.9.4.tar.gz` & `tmp/ChiantiPy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ChiantiPy-0.9.4.tar", last modified: Sat Feb  1 17:27:02 2020, max compression
+gzip compressed data, was "dist/ChiantiPy-0.9.5.tar", last modified: Wed Feb 19 17:05:48 2020, max compression
```

## Comparing `ChiantiPy-0.9.4.tar` & `ChiantiPy-0.9.5.tar`

### file list

```diff
@@ -1,502 +1,510 @@
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/
--rw-r--r--   0 ken       (1000) users      (100)      264 2016-08-05 15:20:54.000000 ChiantiPy-0.9.4/.editorconfig
--rw-r--r--   0 ken       (1000) users      (100)      721 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/.gitignore
--rw-r--r--   0 ken       (1000) users      (100)        0 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/.gitmodules
--rw-r--r--   0 ken       (1000) users      (100)      119 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/.travis.yml
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/
--rw-r--r--   0 ken       (1000) users      (100)      792 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/__init__.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_cl/
--rw-r--r--   0 ken       (1000) users      (100)       95 2016-08-05 15:20:54.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_cl/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     2910 2020-01-23 15:07:23.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_cl/gui.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/
--rw-r--r--   0 ken       (1000) users      (100)      156 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     6963 2020-01-23 15:07:23.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/gui.py
--rw-r--r--   0 ken       (1000) users      (100)     4826 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/ui.py
--rw-r--r--   0 ken       (1000) users      (100)      314 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     1293 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/__init__gh.py
--rw-r--r--   0 ken       (1000) users      (100)     1476 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/__init__kpd.py
--rw-r--r--   0 ken       (1000) users      (100)     1476 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/__init_kpd__.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/base/
--rw-r--r--   0 ken       (1000) users      (100)    28044 2020-01-23 15:07:23.000000 ChiantiPy-0.9.4/ChiantiPy/base/_IonTrails.py
--rw-r--r--   0 ken       (1000) users      (100)     1786 2019-06-15 16:22:29.000000 ChiantiPy-0.9.4/ChiantiPy/base/_IoneqOne.py
--rw-r--r--   0 ken       (1000) users      (100)    16095 2019-10-24 14:33:01.000000 ChiantiPy-0.9.4/ChiantiPy/base/_SpecTrails.py
--rw-r--r--   0 ken       (1000) users      (100)      163 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/base/__init__.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/core/
--rw-r--r--   0 ken       (1000) users      (100)    52510 2019-10-19 15:24:58.000000 ChiantiPy-0.9.4/ChiantiPy/core/Continuum.py
--rw-r--r--   0 ken       (1000) users      (100)   135704 2020-01-31 17:17:13.000000 ChiantiPy-0.9.4/ChiantiPy/core/Ion.py
--rw-r--r--   0 ken       (1000) users      (100)    11294 2020-01-23 15:07:24.000000 ChiantiPy-0.9.4/ChiantiPy/core/Ioneq.py
--rw-r--r--   0 ken       (1000) users      (100)    13216 2020-01-23 15:07:24.000000 ChiantiPy-0.9.4/ChiantiPy/core/IpyMspectrum.py
--rw-r--r--   0 ken       (1000) users      (100)    12026 2019-10-24 14:33:01.000000 ChiantiPy-0.9.4/ChiantiPy/core/Mspectrum.py
--rw-r--r--   0 ken       (1000) users      (100)     8601 2019-07-02 15:16:12.000000 ChiantiPy-0.9.4/ChiantiPy/core/RadLoss.py
--rw-r--r--   0 ken       (1000) users      (100)    16742 2020-01-23 15:07:24.000000 ChiantiPy-0.9.4/ChiantiPy/core/Spectrum.py
--rw-r--r--   0 ken       (1000) users      (100)      397 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/core/__init__.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/
--rw-r--r--   0 ken       (1000) users      (100)        0 2016-11-29 15:11:26.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     3080 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Continuum.py
--rw-r--r--   0 ken       (1000) users      (100)     3317 2020-02-01 16:59:21.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Ion.py
--rw-r--r--   0 ken       (1000) users      (100)     1318 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Ioneq.py
--rw-r--r--   0 ken       (1000) users      (100)     1251 2019-06-17 20:06:11.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Spectrum.py
--rw-r--r--   0 ken       (1000) users      (100)     5964 2020-02-01 17:05:57.000000 ChiantiPy-0.9.4/ChiantiPy/core/tests/test_spectrum_api.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/
--rw-r--r--   0 ken       (1000) users      (100)     1076 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/COPYING.txt
--rw-r--r--   0 ken       (1000) users      (100)     2221 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/FortranRecordReader.py
--rw-r--r--   0 ken       (1000) users      (100)     2002 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/FortranRecordWriter.py
--rw-r--r--   0 ken       (1000) users      (100)      466 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     8928 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_edit_descriptors.py
--rw-r--r--   0 ken       (1000) users      (100)       45 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_exceptions.py
--rw-r--r--   0 ken       (1000) users      (100)    13551 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_input.py
--rw-r--r--   0 ken       (1000) users      (100)     6105 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_lexer.py
--rw-r--r--   0 ken       (1000) users      (100)     1468 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_misc.py
--rw-r--r--   0 ken       (1000) users      (100)    24967 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_output.py
--rw-r--r--   0 ken       (1000) users      (100)    14687 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/_parser.py
--rw-r--r--   0 ken       (1000) users      (100)     2199 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/ChiantiPy/fortranformat/config.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/model/
--rw-r--r--   0 ken       (1000) users      (100)    60779 2020-01-23 15:07:24.000000 ChiantiPy-0.9.4/ChiantiPy/model/Maker.py
--rw-r--r--   0 ken       (1000) users      (100)       84 2019-10-12 15:19:11.000000 ChiantiPy-0.9.4/ChiantiPy/model/__init__.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/tests/
--rw-r--r--   0 ken       (1000) users      (100)      121 2016-07-13 15:31:44.000000 ChiantiPy-0.9.4/ChiantiPy/tests/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)      588 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/ChiantiPy/tests/coveragerc
--rw-r--r--   0 ken       (1000) users      (100)       96 2016-07-13 15:31:44.000000 ChiantiPy-0.9.4/ChiantiPy/tests/setup_package.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy/tools/
--rw-r--r--   0 ken       (1000) users      (100)       52 2016-07-09 15:28:24.000000 ChiantiPy-0.9.4/ChiantiPy/tools/__init__.py
--rw-r--r--   0 ken       (1000) users      (100)     8958 2019-10-09 15:14:16.000000 ChiantiPy-0.9.4/ChiantiPy/tools/archival.py
--rw-r--r--   0 ken       (1000) users      (100)     3867 2019-06-15 16:29:52.000000 ChiantiPy-0.9.4/ChiantiPy/tools/constants.py
--rw-r--r--   0 ken       (1000) users      (100)     2600 2019-08-14 16:01:00.000000 ChiantiPy-0.9.4/ChiantiPy/tools/data.py
--rw-r--r--   0 ken       (1000) users      (100)     3868 2019-06-15 16:31:55.000000 ChiantiPy-0.9.4/ChiantiPy/tools/filters.py
--rw-r--r--   0 ken       (1000) users      (100)    64551 2020-01-23 15:07:24.000000 ChiantiPy-0.9.4/ChiantiPy/tools/io.py
--rw-r--r--   0 ken       (1000) users      (100)     2831 2019-06-26 17:34:30.000000 ChiantiPy-0.9.4/ChiantiPy/tools/mputil.py
--rw-r--r--   0 ken       (1000) users      (100)     2624 2016-08-05 15:20:54.000000 ChiantiPy-0.9.4/ChiantiPy/tools/sources.py
--rw-r--r--   0 ken       (1000) users      (100)    20329 2019-10-11 16:01:36.000000 ChiantiPy-0.9.4/ChiantiPy/tools/util.py
--rw-r--r--   0 ken       (1000) users      (100)      128 2020-02-01 17:14:03.000000 ChiantiPy-0.9.4/ChiantiPy/version.py
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy.egg-info/
--rw-r--r--   0 ken       (1000) users      (100)     5104 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) users      (100)    17466 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy.egg-info/SOURCES.txt
--rw-r--r--   0 ken       (1000) users      (100)        1 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) users      (100)       10 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/ChiantiPy.egg-info/top_level.txt
--rw-r--r--   0 ken       (1000) users      (100)     1247 2016-07-14 14:32:13.000000 ChiantiPy-0.9.4/MANIFEST.in
--rw-r--r--   0 ken       (1000) users      (100)     5104 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/PKG-INFO
--rw-r--r--   0 ken       (1000) users      (100)     3146 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/README
--rw-r--r--   0 ken       (1000) users      (100)     3273 2020-02-01 17:13:17.000000 ChiantiPy-0.9.4/README.md
--rw-r--r--   0 ken       (1000) users      (100)     3571 2020-02-01 17:13:28.000000 ChiantiPy-0.9.4/README.rst
--rw-r--r--   0 ken       (1000) users      (100)      410 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/chiantirc
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/
--rw-r--r--   0 ken       (1000) users      (100)      629 2019-08-09 20:18:58.000000 ChiantiPy-0.9.4/docs/0-notes.txt
--rw-r--r--   0 ken       (1000) users      (100)      610 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/Makefile
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/
--rw-r--r--   0 ken       (1000) users      (100)      230 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/.buildinfo
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/.doctrees/
--rw-r--r--   0 ken       (1000) users      (100)    18877 2019-10-19 15:58:21.000000 ChiantiPy-0.9.4/docs/build/.doctrees/IDL_intro.doctree
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/
--rw-r--r--   0 ken       (1000) users      (100)     3739 2019-10-19 15:58:21.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.doctree
--rw-r--r--   0 ken       (1000) users      (100)    12491 2019-10-19 15:58:22.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.gui_cl.doctree
--rw-r--r--   0 ken       (1000) users      (100)    27285 2019-10-19 15:58:22.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.gui_qt5.doctree
--rw-r--r--   0 ken       (1000) users      (100)    59681 2019-10-19 15:58:22.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.base.doctree
--rw-r--r--   0 ken       (1000) users      (100)   283729 2019-10-19 15:58:24.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.core.doctree
--rw-r--r--   0 ken       (1000) users      (100)    27043 2019-10-19 15:58:26.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.core.tests.doctree
--rw-r--r--   0 ken       (1000) users      (100)     5174 2019-10-19 15:58:21.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.doctree
--rw-r--r--   0 ken       (1000) users      (100)    24905 2019-10-19 15:58:26.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.fortranformat.doctree
--rw-r--r--   0 ken       (1000) users      (100)     5397 2019-10-19 15:58:26.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.tests.doctree
--rw-r--r--   0 ken       (1000) users      (100)   340761 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.tools.doctree
--rw-r--r--   0 ken       (1000) users      (100)     4846 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/index.doctree
--rw-r--r--   0 ken       (1000) users      (100)     2572 2018-10-15 17:33:01.000000 ChiantiPy-0.9.4/docs/build/.doctrees/api/modules.doctree
--rw-r--r--   0 ken       (1000) users      (100)     3895 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/bugs.doctree
--rw-r--r--   0 ken       (1000) users      (100)    31624 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/changelog.doctree
--rw-r--r--   0 ken       (1000) users      (100)  1721327 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 ken       (1000) users      (100)    25181 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/getting_started.doctree
--rw-r--r--   0 ken       (1000) users      (100)     9421 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/index.doctree
--rw-r--r--   0 ken       (1000) users      (100)    34877 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/notes.doctree
--rw-r--r--   0 ken       (1000) users      (100)    70646 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/quick_start.doctree
--rw-r--r--   0 ken       (1000) users      (100)     3525 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/resources.doctree
--rw-r--r--   0 ken       (1000) users      (100)    53512 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.doctrees/tutorial.doctree
--rw-r--r--   0 ken       (1000) users      (100)        0 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/.nojekyll
--rw-r--r--   0 ken       (1000) users      (100)    15354 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/IDL_intro.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/_images/
--rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/2.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/bunch_selector.png
--rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/continuum_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt.png
--rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt_alternate.png
--rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.int.ratio.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.int.ratio.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.int.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.int.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.popplot.png
--rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.rel.emiss.png
--rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum2.png
--rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum_label.png
--rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14_intensity_plot_log.png
--rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe14_intensity_plot_log_index2.png
--rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe_12_wvlranges_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_images/fe_13_14_15_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/fe_25_ff_fb_tp_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_images/fe_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_t_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_t_ratio_top7.png
--rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/radloss.png
--rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_10_20.png
--rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_3panel.png
--rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_integrated.png
--rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_w_si_9.png
--rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_images/spectrum_2e7_1.84_1.90.png
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/_sources/
--rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.4/docs/build/_sources/IDL_intro.rst.txt
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/_sources/api/
--rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.Gui.gui_cl.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.Gui.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.base.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.core.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.core.tests.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.fortranformat.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      487 2018-10-08 17:02:15.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.tests.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.tools.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.4/docs/build/_sources/api/index.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)       64 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/_sources/api/modules.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.4/docs/build/_sources/bugs.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     6736 2019-10-19 15:57:58.000000 ChiantiPy-0.9.4/docs/build/_sources/changelog.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     4921 2018-10-21 16:22:58.000000 ChiantiPy-0.9.4/docs/build/_sources/getting_started.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1633 2019-10-19 15:51:11.000000 ChiantiPy-0.9.4/docs/build/_sources/index.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.4/docs/build/_sources/notes.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_sources/quick_start.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      284 2018-10-08 17:17:38.000000 ChiantiPy-0.9.4/docs/build/_sources/resources.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.4/docs/build/_sources/tutorial.rst.txt
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/_static/
--rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/2.selector.png
--rw-r--r--   0 ken       (1000) users      (100)      673 2017-08-29 15:11:19.000000 ChiantiPy-0.9.4/docs/build/_static/ajax-loader.gif
--rw-r--r--   0 ken       (1000) users      (100)    10716 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/_static/basic.css
--rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/bunch_selector.png
--rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/chiantipy_logo.png
--rw-r--r--   0 ken       (1000) users      (100)      756 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/comment-bright.png
--rw-r--r--   0 ken       (1000) users      (100)      829 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/comment-close.png
--rw-r--r--   0 ken       (1000) users      (100)      641 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/comment.png
--rw-r--r--   0 ken       (1000) users      (100)      107 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/contents.png
--rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/continuum_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)     9224 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/_static/doctools.js
--rw-r--r--   0 ken       (1000) users      (100)      275 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/_static/documentation_options.js
--rw-r--r--   0 ken       (1000) users      (100)      222 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/down-pressed.png
--rw-r--r--   0 ken       (1000) users      (100)      202 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/down.png
--rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt.png
--rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt_alternate.png
--rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.int.ratio.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.int.ratio.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.int.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.int.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.popplot.png
--rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.rel.emiss.png
--rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum2.png
--rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum_label.png
--rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14_intensity_plot_log.png
--rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe14_intensity_plot_log_index2.png
--rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe_12_wvlranges_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_static/fe_13_14_15_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/fe_25_ff_fb_tp_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_static/fe_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)      286 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/file.png
--rw-r--r--   0 ken       (1000) users      (100)   263767 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/jquery-3.1.0.js
--rw-r--r--   0 ken       (1000) users      (100)   268039 2018-07-16 07:59:17.000000 ChiantiPy-0.9.4/docs/build/_static/jquery-3.2.1.js
--rw-r--r--   0 ken       (1000) users      (100)    86659 2019-03-18 15:58:41.000000 ChiantiPy-0.9.4/docs/build/_static/jquery.js
--rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/minus.png
--rw-r--r--   0 ken       (1000) users      (100)      120 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/navigation.png
--rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_t_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_t_ratio_top7.png
--rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/plus.png
--rw-r--r--   0 ken       (1000) users      (100)     4395 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/_static/pygments.css
--rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/radloss.png
--rw-r--r--   0 ken       (1000) users      (100)    25449 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/_static/searchtools.js
--rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_10_20.png
--rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_3panel.png
--rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_integrated.png
--rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_w_si_9.png
--rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/spectrum_2e7_1.84_1.90.png
--rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/_static/sphinxdoc.css
--rw-r--r--   0 ken       (1000) users      (100)      707 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/_static/theme.conf
--rw-r--r--   0 ken       (1000) users      (100)    35168 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/underscore-1.3.1.js
--rw-r--r--   0 ken       (1000) users      (100)    12140 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/underscore.js
--rw-r--r--   0 ken       (1000) users      (100)      214 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/up-pressed.png
--rw-r--r--   0 ken       (1000) users      (100)      203 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/_static/up.png
--rw-r--r--   0 ken       (1000) users      (100)    25355 2018-07-16 07:59:17.000000 ChiantiPy-0.9.4/docs/build/_static/websupport.js
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/api/
--rw-r--r--   0 ken       (1000) users      (100)     8727 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.gui_cl.html
--rw-r--r--   0 ken       (1000) users      (100)    13441 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.gui_qt5.html
--rw-r--r--   0 ken       (1000) users      (100)     6942 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.html
--rw-r--r--   0 ken       (1000) users      (100)    20146 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.base.html
--rw-r--r--   0 ken       (1000) users      (100)    95842 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.core.html
--rw-r--r--   0 ken       (1000) users      (100)    14706 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.core.tests.html
--rw-r--r--   0 ken       (1000) users      (100)    15673 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.fortranformat.html
--rw-r--r--   0 ken       (1000) users      (100)    14013 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.html
--rw-r--r--   0 ken       (1000) users      (100)     6404 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.tests.html
--rw-r--r--   0 ken       (1000) users      (100)   101217 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/ChiantiPy.tools.html
--rw-r--r--   0 ken       (1000) users      (100)    11624 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/api/index.html
--rw-r--r--   0 ken       (1000) users      (100)    11149 2018-10-22 16:42:30.000000 ChiantiPy-0.9.4/docs/build/api/modules.html
--rw-r--r--   0 ken       (1000) users      (100)     4509 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/bugs.html
--rw-r--r--   0 ken       (1000) users      (100)    15005 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/changelog.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/doctrees/
--rw-r--r--   0 ken       (1000) users      (100)    18877 2019-10-19 16:01:56.000000 ChiantiPy-0.9.4/docs/build/doctrees/IDL_intro.doctree
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/
--rw-r--r--   0 ken       (1000) users      (100)     3739 2019-10-19 16:01:56.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.doctree
--rw-r--r--   0 ken       (1000) users      (100)    12491 2019-10-19 16:01:56.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.gui_cl.doctree
--rw-r--r--   0 ken       (1000) users      (100)    27285 2019-10-19 16:01:56.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.gui_qt5.doctree
--rw-r--r--   0 ken       (1000) users      (100)    59681 2019-10-19 16:01:57.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.base.doctree
--rw-r--r--   0 ken       (1000) users      (100)   283729 2019-10-19 16:01:59.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.core.doctree
--rw-r--r--   0 ken       (1000) users      (100)    27043 2019-10-19 16:02:00.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.core.tests.doctree
--rw-r--r--   0 ken       (1000) users      (100)     5201 2019-10-19 16:07:37.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.doctree
--rw-r--r--   0 ken       (1000) users      (100)    24905 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.fortranformat.doctree
--rw-r--r--   0 ken       (1000) users      (100)    48348 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.model.doctree
--rw-r--r--   0 ken       (1000) users      (100)     5397 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.tests.doctree
--rw-r--r--   0 ken       (1000) users      (100)   340761 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.tools.doctree
--rw-r--r--   0 ken       (1000) users      (100)     4846 2019-10-19 16:07:39.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/index.doctree
--rw-r--r--   0 ken       (1000) users      (100)     2572 2018-10-15 17:37:49.000000 ChiantiPy-0.9.4/docs/build/doctrees/api/modules.doctree
--rw-r--r--   0 ken       (1000) users      (100)     3895 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/bugs.doctree
--rw-r--r--   0 ken       (1000) users      (100)    31624 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/changelog.doctree
--rw-r--r--   0 ken       (1000) users      (100)  1727541 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/doctrees/environment.pickle
--rw-r--r--   0 ken       (1000) users      (100)    25181 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/getting_started.doctree
--rw-r--r--   0 ken       (1000) users      (100)     9421 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/index.doctree
--rw-r--r--   0 ken       (1000) users      (100)    34877 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/notes.doctree
--rw-r--r--   0 ken       (1000) users      (100)    70646 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/quick_start.doctree
--rw-r--r--   0 ken       (1000) users      (100)     3525 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/resources.doctree
--rw-r--r--   0 ken       (1000) users      (100)    53512 2019-10-19 16:02:01.000000 ChiantiPy-0.9.4/docs/build/doctrees/tutorial.doctree
--rw-r--r--   0 ken       (1000) users      (100)    42811 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/genindex.html
--rw-r--r--   0 ken       (1000) users      (100)    13411 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/getting_started.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/
--rw-r--r--   0 ken       (1000) users      (100)      230 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/.buildinfo
--rw-r--r--   0 ken       (1000) users      (100)        0 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/.nojekyll
--rw-r--r--   0 ken       (1000) users      (100)    15354 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/IDL_intro.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/_images/
--rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/2.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/bunch_selector.png
--rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/continuum_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt.png
--rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt_alternate.png
--rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.ratio.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.ratio.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.popplot.png
--rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.rel.emiss.png
--rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum2.png
--rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum_label.png
--rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14_intensity_plot_log.png
--rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe14_intensity_plot_log_index2.png
--rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe_12_wvlranges_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe_13_14_15_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe_25_ff_fb_tp_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_images/fe_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_t_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_t_ratio_top7.png
--rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/radloss.png
--rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_10_20.png
--rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_3panel.png
--rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_integrated.png
--rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_w_si_9.png
--rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_images/spectrum_2e7_1.84_1.90.png
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/_sources/
--rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.4/docs/build/html/_sources/IDL_intro.rst.txt
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/
--rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.Gui.gui_cl.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.Gui.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.base.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.core.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.core.tests.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.fortranformat.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      352 2019-10-19 16:23:55.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.model.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      507 2019-10-19 16:05:27.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.tests.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.tools.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/index.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)       64 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/api/modules.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.4/docs/build/html/_sources/bugs.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     6736 2019-10-19 15:57:58.000000 ChiantiPy-0.9.4/docs/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     4921 2018-10-21 16:22:58.000000 ChiantiPy-0.9.4/docs/build/html/_sources/getting_started.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     1633 2019-10-19 15:51:11.000000 ChiantiPy-0.9.4/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.4/docs/build/html/_sources/notes.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_sources/quick_start.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)      284 2018-10-08 17:17:38.000000 ChiantiPy-0.9.4/docs/build/html/_sources/resources.rst.txt
--rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.4/docs/build/html/_sources/tutorial.rst.txt
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/_static/
--rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/2.selector.png
--rw-r--r--   0 ken       (1000) users      (100)      673 2017-08-29 15:11:19.000000 ChiantiPy-0.9.4/docs/build/html/_static/ajax-loader.gif
--rw-r--r--   0 ken       (1000) users      (100)    10716 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/basic.css
--rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/bunch_selector.png
--rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/chiantipy_logo.png
--rw-r--r--   0 ken       (1000) users      (100)      756 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/comment-bright.png
--rw-r--r--   0 ken       (1000) users      (100)      829 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/comment-close.png
--rw-r--r--   0 ken       (1000) users      (100)      641 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/comment.png
--rw-r--r--   0 ken       (1000) users      (100)      107 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/contents.png
--rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/continuum_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)     9224 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/doctools.js
--rw-r--r--   0 ken       (1000) users      (100)      275 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 ken       (1000) users      (100)      222 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/down-pressed.png
--rw-r--r--   0 ken       (1000) users      (100)      202 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/down.png
--rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt.png
--rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt_alternate.png
--rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.ratio.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.ratio.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.popplot.png
--rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.rel.emiss.png
--rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum2.png
--rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum_label.png
--rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14_intensity_plot_log.png
--rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe14_intensity_plot_log_index2.png
--rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe_12_wvlranges_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe_13_14_15_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe_25_ff_fb_tp_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/fe_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)      286 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/file.png
--rw-r--r--   0 ken       (1000) users      (100)   263767 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/jquery-3.1.0.js
--rw-r--r--   0 ken       (1000) users      (100)   268039 2018-07-16 07:59:17.000000 ChiantiPy-0.9.4/docs/build/html/_static/jquery-3.2.1.js
--rw-r--r--   0 ken       (1000) users      (100)    86659 2019-03-18 15:58:41.000000 ChiantiPy-0.9.4/docs/build/html/_static/jquery.js
--rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/minus.png
--rw-r--r--   0 ken       (1000) users      (100)      120 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/navigation.png
--rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_t_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_t_ratio_top7.png
--rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/plus.png
--rw-r--r--   0 ken       (1000) users      (100)     4395 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/pygments.css
--rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/radloss.png
--rw-r--r--   0 ken       (1000) users      (100)    25449 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/searchtools.js
--rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_10_20.png
--rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_3panel.png
--rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_integrated.png
--rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_w_si_9.png
--rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/spectrum_2e7_1.84_1.90.png
--rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/build/html/_static/sphinxdoc.css
--rw-r--r--   0 ken       (1000) users      (100)      707 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/build/html/_static/theme.conf
--rw-r--r--   0 ken       (1000) users      (100)    35168 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 ken       (1000) users      (100)    12140 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/underscore.js
--rw-r--r--   0 ken       (1000) users      (100)      214 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/up-pressed.png
--rw-r--r--   0 ken       (1000) users      (100)      203 2017-10-22 11:19:57.000000 ChiantiPy-0.9.4/docs/build/html/_static/up.png
--rw-r--r--   0 ken       (1000) users      (100)    25355 2018-07-16 07:59:17.000000 ChiantiPy-0.9.4/docs/build/html/_static/websupport.js
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/build/html/api/
--rw-r--r--   0 ken       (1000) users      (100)     8727 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.gui_cl.html
--rw-r--r--   0 ken       (1000) users      (100)    13441 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.gui_qt5.html
--rw-r--r--   0 ken       (1000) users      (100)     6942 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.html
--rw-r--r--   0 ken       (1000) users      (100)    20146 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.base.html
--rw-r--r--   0 ken       (1000) users      (100)    95842 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.core.html
--rw-r--r--   0 ken       (1000) users      (100)    14706 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.core.tests.html
--rw-r--r--   0 ken       (1000) users      (100)    15673 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.fortranformat.html
--rw-r--r--   0 ken       (1000) users      (100)    14525 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.html
--rw-r--r--   0 ken       (1000) users      (100)    19240 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.model.html
--rw-r--r--   0 ken       (1000) users      (100)     6404 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.tests.html
--rw-r--r--   0 ken       (1000) users      (100)   101217 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.tools.html
--rw-r--r--   0 ken       (1000) users      (100)    11990 2019-10-19 16:07:39.000000 ChiantiPy-0.9.4/docs/build/html/api/index.html
--rw-r--r--   0 ken       (1000) users      (100)    10213 2018-10-22 16:22:47.000000 ChiantiPy-0.9.4/docs/build/html/api/modules.html
--rw-r--r--   0 ken       (1000) users      (100)     4509 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/bugs.html
--rw-r--r--   0 ken       (1000) users      (100)    15005 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/changelog.html
--rw-r--r--   0 ken       (1000) users      (100)  3563520 2018-10-08 17:48:45.000000 ChiantiPy-0.9.4/docs/build/html/chiantdoc-0.8.0.tar
--rw-r--r--   0 ken       (1000) users      (100)    46780 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/genindex.html
--rw-r--r--   0 ken       (1000) users      (100)    13411 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/getting_started.html
--rw-r--r--   0 ken       (1000) users      (100)    12415 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/index.html
--rw-r--r--   0 ken       (1000) users      (100)    11820 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/notes.html
--rw-r--r--   0 ken       (1000) users      (100)     2383 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/objects.inv
--rw-r--r--   0 ken       (1000) users      (100)    13536 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/py-modindex.html
--rw-r--r--   0 ken       (1000) users      (100)    88264 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/quick_start.html
--rw-r--r--   0 ken       (1000) users      (100)     5055 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/resources.html
--rw-r--r--   0 ken       (1000) users      (100)     4060 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/search.html
--rw-r--r--   0 ken       (1000) users      (100)    34448 2019-10-19 16:24:03.000000 ChiantiPy-0.9.4/docs/build/html/searchindex.js
--rw-r--r--   0 ken       (1000) users      (100)    31792 2019-10-19 16:02:02.000000 ChiantiPy-0.9.4/docs/build/html/tutorial.html
--rw-r--r--   0 ken       (1000) users      (100)    12415 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/index.html
--rw-r--r--   0 ken       (1000) users      (100)    11820 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/notes.html
--rw-r--r--   0 ken       (1000) users      (100)     2185 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/objects.inv
--rw-r--r--   0 ken       (1000) users      (100)    13090 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/py-modindex.html
--rw-r--r--   0 ken       (1000) users      (100)    88264 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/quick_start.html
--rw-r--r--   0 ken       (1000) users      (100)     5055 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/resources.html
--rw-r--r--   0 ken       (1000) users      (100)     4060 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/search.html
--rw-r--r--   0 ken       (1000) users      (100)    33059 2019-10-19 15:58:28.000000 ChiantiPy-0.9.4/docs/build/searchindex.js
--rw-r--r--   0 ken       (1000) users      (100)    31792 2019-10-19 15:58:27.000000 ChiantiPy-0.9.4/docs/build/tutorial.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/
--rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.4/docs/source/IDL_intro.rst
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/_static/
--rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/2.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/bunch_selector.png
--rw-r--r--   0 ken       (1000) users      (100)    26923 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/source/_static/chiantipy_logo.png
--rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/continuum_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt.png
--rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt.selector.png
--rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt_alternate.png
--rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.int.ratio.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.int.ratio.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.int.vs.d.png
--rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.int.vs.t.png
--rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.popplot.png
--rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.rel.emiss.png
--rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum2.png
--rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum_label.png
--rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14_intensity_plot_log.png
--rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe14_intensity_plot_log_index2.png
--rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe_12_wvlranges_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/source/_static/fe_13_14_15_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/fe_25_ff_fb_tp_2e7_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/source/_static/fe_ioneq.png
--rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_spectrum.png
--rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_t_ratio.png
--rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_t_ratio_top7.png
--rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/radloss.png
--rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_10_20.png
--rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_1_10.png
--rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_3panel.png
--rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_integrated.png
--rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_w_si_9.png
--rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.4/docs/source/_static/spectrum_2e7_1.84_1.90.png
--rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/source/_static/sphinxdoc.css
--rw-r--r--   0 ken       (1000) users      (100)      707 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/source/_static/theme.conf
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/_templates/
--rw-r--r--   0 ken       (1000) users      (100)      411 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/source/_templates/layout.html
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/api/
--rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.Gui.gui_cl.rst
--rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.Gui.gui_qt5.rst
--rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.Gui.rst
--rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.base.rst
--rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.core.rst
--rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.core.tests.rst
--rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.fortranformat.rst
--rw-r--r--   0 ken       (1000) users      (100)      352 2019-10-19 16:23:55.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.model.rst
--rw-r--r--   0 ken       (1000) users      (100)      507 2019-10-19 16:05:27.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.rst
--rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.tests.rst
--rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.4/docs/source/api/ChiantiPy.tools.rst
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/api/_static/
--rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-24 16:45:03.000000 ChiantiPy-0.9.4/docs/source/api/_static/chiantipy_logo.png
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/docs/source/api/_templates/
--rw-r--r--   0 ken       (1000) users      (100)      411 2018-10-24 16:48:23.000000 ChiantiPy-0.9.4/docs/source/api/_templates/layout.html
--rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.4/docs/source/api/index.rst
--rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.4/docs/source/bugs.rst
--rw-r--r--   0 ken       (1000) users      (100)     7635 2020-02-01 17:17:39.000000 ChiantiPy-0.9.4/docs/source/changelog.rst
--rw-r--r--   0 ken       (1000) users      (100)     5525 2020-02-01 17:16:00.000000 ChiantiPy-0.9.4/docs/source/conf.py
--rw-r--r--   0 ken       (1000) users      (100)     4921 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/source/getting_started.rst
--rw-r--r--   0 ken       (1000) users      (100)     1633 2020-02-01 17:15:29.000000 ChiantiPy-0.9.4/docs/source/index.rst
--rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.4/docs/source/notes.rst
--rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.4/docs/source/quick_start.rst
--rw-r--r--   0 ken       (1000) users      (100)      284 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/docs/source/resources.rst
--rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.4/docs/source/tutorial.rst
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/jupyter_notebooks/
--rw-r--r--   0 ken       (1000) users      (100)   278737 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/jupyter_notebooks/QuickStart.html
--rw-r--r--   0 ken       (1000) users      (100)    41104 2019-08-29 15:43:16.000000 ChiantiPy-0.9.4/jupyter_notebooks/QuickStart.ipynb
-drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/licenses/
--rw-r--r--   0 ken       (1000) users      (100)      768 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/licenses/LICENSE
--rw-r--r--   0 ken       (1000) users      (100)     1075 2016-07-14 19:28:36.000000 ChiantiPy-0.9.4/licenses/LICENSE.fortranformat
--rw-r--r--   0 ken       (1000) users      (100)       59 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/pytest.ini
--rw-r--r--   0 ken       (1000) users      (100)       81 2017-02-18 15:57:42.000000 ChiantiPy-0.9.4/readthedocs.yml
--rw-r--r--   0 ken       (1000) users      (100)       35 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/requirements.txt
--rw-r--r--   0 ken       (1000) users      (100)      146 2019-06-11 16:14:41.000000 ChiantiPy-0.9.4/rtd_environment.yml
--rw-r--r--   0 ken       (1000) users      (100)      543 2020-02-01 17:27:02.000000 ChiantiPy-0.9.4/setup.cfg
--rw-r--r--   0 ken       (1000) users      (100)      909 2020-02-01 17:13:42.000000 ChiantiPy-0.9.4/setup.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/
+-rw-r--r--   0 ken       (1000) users      (100)      264 2016-08-05 15:20:54.000000 ChiantiPy-0.9.5/.editorconfig
+-rw-r--r--   0 ken       (1000) users      (100)      756 2020-02-19 16:16:54.000000 ChiantiPy-0.9.5/.gitignore
+-rw-r--r--   0 ken       (1000) users      (100)        0 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/.gitmodules
+-rw-r--r--   0 ken       (1000) users      (100)      119 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/.travis.yml
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/
+-rw-r--r--   0 ken       (1000) users      (100)      792 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/__init__.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_cl/
+-rw-r--r--   0 ken       (1000) users      (100)       95 2016-08-05 15:20:54.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_cl/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     2910 2020-01-23 15:07:23.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_cl/gui.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/
+-rw-r--r--   0 ken       (1000) users      (100)      156 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     6963 2020-01-23 15:07:23.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/gui.py
+-rw-r--r--   0 ken       (1000) users      (100)     4826 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/ui.py
+-rw-r--r--   0 ken       (1000) users      (100)      314 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     1293 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/__init__gh.py
+-rw-r--r--   0 ken       (1000) users      (100)     1476 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/__init__kpd.py
+-rw-r--r--   0 ken       (1000) users      (100)     1476 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/__init_kpd__.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/base/
+-rw-r--r--   0 ken       (1000) users      (100)    27946 2020-02-18 17:46:31.000000 ChiantiPy-0.9.5/ChiantiPy/base/_IonTrails.py
+-rw-r--r--   0 ken       (1000) users      (100)     1786 2019-06-15 16:22:29.000000 ChiantiPy-0.9.5/ChiantiPy/base/_IoneqOne.py
+-rw-r--r--   0 ken       (1000) users      (100)    16095 2019-10-24 14:33:01.000000 ChiantiPy-0.9.5/ChiantiPy/base/_SpecTrails.py
+-rw-r--r--   0 ken       (1000) users      (100)      163 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/base/__init__.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/core/
+-rw-r--r--   0 ken       (1000) users      (100)    52510 2019-10-19 15:24:58.000000 ChiantiPy-0.9.5/ChiantiPy/core/Continuum.py
+-rw-r--r--   0 ken       (1000) users      (100)   135704 2020-01-31 17:17:13.000000 ChiantiPy-0.9.5/ChiantiPy/core/Ion.py
+-rw-r--r--   0 ken       (1000) users      (100)    11294 2020-01-23 15:07:24.000000 ChiantiPy-0.9.5/ChiantiPy/core/Ioneq.py
+-rw-r--r--   0 ken       (1000) users      (100)    13216 2020-01-23 15:07:24.000000 ChiantiPy-0.9.5/ChiantiPy/core/IpyMspectrum.py
+-rw-r--r--   0 ken       (1000) users      (100)    12026 2019-10-24 14:33:01.000000 ChiantiPy-0.9.5/ChiantiPy/core/Mspectrum.py
+-rw-r--r--   0 ken       (1000) users      (100)     8601 2019-07-02 15:16:12.000000 ChiantiPy-0.9.5/ChiantiPy/core/RadLoss.py
+-rw-r--r--   0 ken       (1000) users      (100)    16742 2020-01-23 15:07:24.000000 ChiantiPy-0.9.5/ChiantiPy/core/Spectrum.py
+-rw-r--r--   0 ken       (1000) users      (100)      397 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/core/__init__.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/
+-rw-r--r--   0 ken       (1000) users      (100)        0 2016-11-29 15:11:26.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     3080 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Continuum.py
+-rw-r--r--   0 ken       (1000) users      (100)     3317 2020-02-01 16:59:21.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Ion.py
+-rw-r--r--   0 ken       (1000) users      (100)     1318 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Ioneq.py
+-rw-r--r--   0 ken       (1000) users      (100)     1251 2019-06-17 20:06:11.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Spectrum.py
+-rw-r--r--   0 ken       (1000) users      (100)     5964 2020-02-01 17:05:57.000000 ChiantiPy-0.9.5/ChiantiPy/core/tests/test_spectrum_api.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/
+-rw-r--r--   0 ken       (1000) users      (100)     1076 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/COPYING.txt
+-rw-r--r--   0 ken       (1000) users      (100)     2221 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/FortranRecordReader.py
+-rw-r--r--   0 ken       (1000) users      (100)     2002 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/FortranRecordWriter.py
+-rw-r--r--   0 ken       (1000) users      (100)      466 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     8928 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_edit_descriptors.py
+-rw-r--r--   0 ken       (1000) users      (100)       45 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_exceptions.py
+-rw-r--r--   0 ken       (1000) users      (100)    13551 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_input.py
+-rw-r--r--   0 ken       (1000) users      (100)     6105 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_lexer.py
+-rw-r--r--   0 ken       (1000) users      (100)     1468 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_misc.py
+-rw-r--r--   0 ken       (1000) users      (100)    24967 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_output.py
+-rw-r--r--   0 ken       (1000) users      (100)    14687 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/_parser.py
+-rw-r--r--   0 ken       (1000) users      (100)     2199 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/ChiantiPy/fortranformat/config.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/model/
+-rw-r--r--   0 ken       (1000) users      (100)    60779 2020-01-23 15:07:24.000000 ChiantiPy-0.9.5/ChiantiPy/model/Maker.py
+-rw-r--r--   0 ken       (1000) users      (100)       84 2019-10-12 15:19:11.000000 ChiantiPy-0.9.5/ChiantiPy/model/__init__.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/tests/
+-rw-r--r--   0 ken       (1000) users      (100)      121 2016-07-13 15:31:44.000000 ChiantiPy-0.9.5/ChiantiPy/tests/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)      588 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/ChiantiPy/tests/coveragerc
+-rw-r--r--   0 ken       (1000) users      (100)       96 2016-07-13 15:31:44.000000 ChiantiPy-0.9.5/ChiantiPy/tests/setup_package.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy/tools/
+-rw-r--r--   0 ken       (1000) users      (100)       52 2016-07-09 15:28:24.000000 ChiantiPy-0.9.5/ChiantiPy/tools/__init__.py
+-rw-r--r--   0 ken       (1000) users      (100)     8958 2019-10-09 15:14:16.000000 ChiantiPy-0.9.5/ChiantiPy/tools/archival.py
+-rw-r--r--   0 ken       (1000) users      (100)     3867 2019-06-15 16:29:52.000000 ChiantiPy-0.9.5/ChiantiPy/tools/constants.py
+-rw-r--r--   0 ken       (1000) users      (100)     2600 2019-08-14 16:01:00.000000 ChiantiPy-0.9.5/ChiantiPy/tools/data.py
+-rw-r--r--   0 ken       (1000) users      (100)     3868 2019-06-15 16:31:55.000000 ChiantiPy-0.9.5/ChiantiPy/tools/filters.py
+-rw-r--r--   0 ken       (1000) users      (100)    64551 2020-01-23 15:07:24.000000 ChiantiPy-0.9.5/ChiantiPy/tools/io.py
+-rw-r--r--   0 ken       (1000) users      (100)     2831 2019-06-26 17:34:30.000000 ChiantiPy-0.9.5/ChiantiPy/tools/mputil.py
+-rw-r--r--   0 ken       (1000) users      (100)     2624 2016-08-05 15:20:54.000000 ChiantiPy-0.9.5/ChiantiPy/tools/sources.py
+-rw-r--r--   0 ken       (1000) users      (100)    20329 2019-10-11 16:01:36.000000 ChiantiPy-0.9.5/ChiantiPy/tools/util.py
+-rw-r--r--   0 ken       (1000) users      (100)      128 2020-02-19 16:35:11.000000 ChiantiPy-0.9.5/ChiantiPy/version.py
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy.egg-info/
+-rw-r--r--   0 ken       (1000) users      (100)     5104 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy.egg-info/PKG-INFO
+-rw-r--r--   0 ken       (1000) users      (100)    17796 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ken       (1000) users      (100)        1 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ken       (1000) users      (100)       10 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/ChiantiPy.egg-info/top_level.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1247 2016-07-14 14:32:13.000000 ChiantiPy-0.9.5/MANIFEST.in
+-rw-r--r--   0 ken       (1000) users      (100)     5104 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/PKG-INFO
+-rw-r--r--   0 ken       (1000) users      (100)     3146 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/README
+-rw-r--r--   0 ken       (1000) users      (100)     3273 2020-02-19 16:20:37.000000 ChiantiPy-0.9.5/README.md
+-rw-r--r--   0 ken       (1000) users      (100)     3571 2020-02-01 17:13:28.000000 ChiantiPy-0.9.5/README.rst
+-rw-r--r--   0 ken       (1000) users      (100)      410 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/chiantirc
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/
+-rw-r--r--   0 ken       (1000) users      (100)      629 2019-08-09 20:18:58.000000 ChiantiPy-0.9.5/docs/0-notes.txt
+-rw-r--r--   0 ken       (1000) users      (100)      610 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/Makefile
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/
+-rw-r--r--   0 ken       (1000) users      (100)      230 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/.buildinfo
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/.doctrees/
+-rw-r--r--   0 ken       (1000) users      (100)    18877 2020-02-19 16:35:45.000000 ChiantiPy-0.9.5/docs/build/.doctrees/IDL_intro.doctree
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/
+-rw-r--r--   0 ken       (1000) users      (100)     3739 2020-02-19 16:35:45.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    12491 2020-02-19 16:35:45.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.gui_cl.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    27285 2020-02-19 16:35:45.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.gui_qt5.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    59681 2020-02-19 16:35:46.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.base.doctree
+-rw-r--r--   0 ken       (1000) users      (100)   283729 2020-02-19 16:35:48.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.core.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    27043 2020-02-19 16:35:50.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.core.tests.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     5201 2020-02-19 16:35:45.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    24905 2020-02-19 16:35:50.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.fortranformat.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    48348 2020-02-19 16:35:50.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.model.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     5397 2020-02-19 16:35:50.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.tests.doctree
+-rw-r--r--   0 ken       (1000) users      (100)   340761 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.tools.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     4846 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/index.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     2572 2018-10-15 17:33:01.000000 ChiantiPy-0.9.5/docs/build/.doctrees/api/modules.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     3895 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/bugs.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    36733 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/.doctrees/changelog.doctree
+-rw-r--r--   0 ken       (1000) users      (100)  1730708 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/.doctrees/environment.pickle
+-rw-r--r--   0 ken       (1000) users      (100)    25181 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/getting_started.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     9421 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/index.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    34877 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/notes.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    70646 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/quick_start.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     3525 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/resources.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    53512 2020-02-19 16:35:51.000000 ChiantiPy-0.9.5/docs/build/.doctrees/tutorial.doctree
+-rw-r--r--   0 ken       (1000) users      (100)        0 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/.nojekyll
+-rw-r--r--   0 ken       (1000) users      (100)    15354 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/IDL_intro.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/_images/
+-rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/2.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/bunch_selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/continuum_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt.png
+-rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt_alternate.png
+-rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.int.ratio.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.int.ratio.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.int.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.int.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.popplot.png
+-rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.rel.emiss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum2.png
+-rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum_label.png
+-rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14_intensity_plot_log.png
+-rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe14_intensity_plot_log_index2.png
+-rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe_12_wvlranges_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_images/fe_13_14_15_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/fe_25_ff_fb_tp_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_images/fe_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_t_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_t_ratio_top7.png
+-rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/radloss.png
+-rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_10_20.png
+-rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_3panel.png
+-rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_integrated.png
+-rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_w_si_9.png
+-rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_images/spectrum_2e7_1.84_1.90.png
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/_sources/
+-rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.5/docs/build/_sources/IDL_intro.rst.txt
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/_sources/api/
+-rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.Gui.gui_cl.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.Gui.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.base.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.core.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.core.tests.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.fortranformat.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      352 2019-10-19 16:23:55.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.model.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      507 2019-10-19 16:05:27.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.tests.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.tools.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.5/docs/build/_sources/api/index.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)       64 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/_sources/api/modules.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.5/docs/build/_sources/bugs.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     8017 2020-02-19 16:44:39.000000 ChiantiPy-0.9.5/docs/build/_sources/changelog.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     4921 2018-10-21 16:22:58.000000 ChiantiPy-0.9.5/docs/build/_sources/getting_started.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1633 2020-02-19 16:33:55.000000 ChiantiPy-0.9.5/docs/build/_sources/index.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.5/docs/build/_sources/notes.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_sources/quick_start.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      284 2018-10-08 17:17:38.000000 ChiantiPy-0.9.5/docs/build/_sources/resources.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.5/docs/build/_sources/tutorial.rst.txt
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/_static/
+-rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/2.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)      673 2017-08-29 15:11:19.000000 ChiantiPy-0.9.5/docs/build/_static/ajax-loader.gif
+-rw-r--r--   0 ken       (1000) users      (100)    10716 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/_static/basic.css
+-rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/bunch_selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/chiantipy_logo.png
+-rw-r--r--   0 ken       (1000) users      (100)      756 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/comment-bright.png
+-rw-r--r--   0 ken       (1000) users      (100)      829 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/comment-close.png
+-rw-r--r--   0 ken       (1000) users      (100)      641 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/comment.png
+-rw-r--r--   0 ken       (1000) users      (100)      107 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/contents.png
+-rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/continuum_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)     9224 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/_static/doctools.js
+-rw-r--r--   0 ken       (1000) users      (100)      275 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/_static/documentation_options.js
+-rw-r--r--   0 ken       (1000) users      (100)      222 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/down-pressed.png
+-rw-r--r--   0 ken       (1000) users      (100)      202 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/down.png
+-rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt.png
+-rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt_alternate.png
+-rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.int.ratio.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.int.ratio.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.int.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.int.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.popplot.png
+-rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.rel.emiss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum2.png
+-rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum_label.png
+-rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14_intensity_plot_log.png
+-rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe14_intensity_plot_log_index2.png
+-rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe_12_wvlranges_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_static/fe_13_14_15_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/fe_25_ff_fb_tp_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_static/fe_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)      286 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/file.png
+-rw-r--r--   0 ken       (1000) users      (100)   263767 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/jquery-3.1.0.js
+-rw-r--r--   0 ken       (1000) users      (100)   268039 2018-07-16 07:59:17.000000 ChiantiPy-0.9.5/docs/build/_static/jquery-3.2.1.js
+-rw-r--r--   0 ken       (1000) users      (100)    86659 2019-03-18 15:58:41.000000 ChiantiPy-0.9.5/docs/build/_static/jquery.js
+-rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/minus.png
+-rw-r--r--   0 ken       (1000) users      (100)      120 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/navigation.png
+-rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_t_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_t_ratio_top7.png
+-rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/plus.png
+-rw-r--r--   0 ken       (1000) users      (100)     4395 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/_static/pygments.css
+-rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/radloss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25449 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/_static/searchtools.js
+-rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_10_20.png
+-rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_3panel.png
+-rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_integrated.png
+-rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_w_si_9.png
+-rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/spectrum_2e7_1.84_1.90.png
+-rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/_static/sphinxdoc.css
+-rw-r--r--   0 ken       (1000) users      (100)      707 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/_static/theme.conf
+-rw-r--r--   0 ken       (1000) users      (100)    35168 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/underscore-1.3.1.js
+-rw-r--r--   0 ken       (1000) users      (100)    12140 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/underscore.js
+-rw-r--r--   0 ken       (1000) users      (100)      214 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/up-pressed.png
+-rw-r--r--   0 ken       (1000) users      (100)      203 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/_static/up.png
+-rw-r--r--   0 ken       (1000) users      (100)    25355 2018-07-16 07:59:17.000000 ChiantiPy-0.9.5/docs/build/_static/websupport.js
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/api/
+-rw-r--r--   0 ken       (1000) users      (100)     8727 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.gui_cl.html
+-rw-r--r--   0 ken       (1000) users      (100)    13441 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.gui_qt5.html
+-rw-r--r--   0 ken       (1000) users      (100)     6942 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.html
+-rw-r--r--   0 ken       (1000) users      (100)    20146 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.base.html
+-rw-r--r--   0 ken       (1000) users      (100)    95842 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.core.html
+-rw-r--r--   0 ken       (1000) users      (100)    14706 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.core.tests.html
+-rw-r--r--   0 ken       (1000) users      (100)    15665 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.fortranformat.html
+-rw-r--r--   0 ken       (1000) users      (100)    14525 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.html
+-rw-r--r--   0 ken       (1000) users      (100)    19240 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.model.html
+-rw-r--r--   0 ken       (1000) users      (100)     6332 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.tests.html
+-rw-r--r--   0 ken       (1000) users      (100)   101217 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/ChiantiPy.tools.html
+-rw-r--r--   0 ken       (1000) users      (100)    12136 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/api/index.html
+-rw-r--r--   0 ken       (1000) users      (100)    11149 2018-10-22 16:42:30.000000 ChiantiPy-0.9.5/docs/build/api/modules.html
+-rw-r--r--   0 ken       (1000) users      (100)     4509 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/bugs.html
+-rw-r--r--   0 ken       (1000) users      (100)    17202 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/changelog.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/doctrees/
+-rw-r--r--   0 ken       (1000) users      (100)    18877 2019-10-19 16:01:56.000000 ChiantiPy-0.9.5/docs/build/doctrees/IDL_intro.doctree
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:47.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/
+-rw-r--r--   0 ken       (1000) users      (100)     3739 2019-10-19 16:01:56.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    12491 2019-10-19 16:01:56.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.gui_cl.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    27285 2019-10-19 16:01:56.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.gui_qt5.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    59681 2019-10-19 16:01:57.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.base.doctree
+-rw-r--r--   0 ken       (1000) users      (100)   283729 2019-10-19 16:01:59.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.core.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    27043 2019-10-19 16:02:00.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.core.tests.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     5201 2019-10-19 16:07:37.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    24905 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.fortranformat.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    48348 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.model.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     5397 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.tests.doctree
+-rw-r--r--   0 ken       (1000) users      (100)   340761 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.tools.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     4846 2019-10-19 16:07:39.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/index.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     2572 2018-10-15 17:37:49.000000 ChiantiPy-0.9.5/docs/build/doctrees/api/modules.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     3895 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/bugs.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    31624 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/changelog.doctree
+-rw-r--r--   0 ken       (1000) users      (100)  1727541 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 ken       (1000) users      (100)    25181 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/getting_started.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     9421 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/index.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    34877 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/notes.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    70646 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/quick_start.doctree
+-rw-r--r--   0 ken       (1000) users      (100)     3525 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/resources.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    53512 2019-10-19 16:02:01.000000 ChiantiPy-0.9.5/docs/build/doctrees/tutorial.doctree
+-rw-r--r--   0 ken       (1000) users      (100)    46780 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/genindex.html
+-rw-r--r--   0 ken       (1000) users      (100)    13411 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/getting_started.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/
+-rw-r--r--   0 ken       (1000) users      (100)      230 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/.buildinfo
+-rw-r--r--   0 ken       (1000) users      (100)        0 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/.nojekyll
+-rw-r--r--   0 ken       (1000) users      (100)    15354 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/IDL_intro.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/_images/
+-rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/2.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/bunch_selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/continuum_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt.png
+-rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt_alternate.png
+-rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.ratio.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.ratio.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.popplot.png
+-rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.rel.emiss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum2.png
+-rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum_label.png
+-rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14_intensity_plot_log.png
+-rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe14_intensity_plot_log_index2.png
+-rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe_12_wvlranges_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe_13_14_15_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe_25_ff_fb_tp_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_images/fe_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_t_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_t_ratio_top7.png
+-rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/radloss.png
+-rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_10_20.png
+-rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_3panel.png
+-rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_integrated.png
+-rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_w_si_9.png
+-rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_images/spectrum_2e7_1.84_1.90.png
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/_sources/
+-rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.5/docs/build/html/_sources/IDL_intro.rst.txt
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/
+-rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.Gui.gui_cl.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.Gui.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.base.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.core.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.core.tests.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.fortranformat.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      352 2019-10-19 16:23:55.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.model.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      507 2019-10-19 16:05:27.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.tests.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.tools.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/index.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)       64 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/api/modules.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.5/docs/build/html/_sources/bugs.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     6736 2019-10-19 15:57:58.000000 ChiantiPy-0.9.5/docs/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     4921 2018-10-21 16:22:58.000000 ChiantiPy-0.9.5/docs/build/html/_sources/getting_started.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     1633 2019-10-19 15:51:11.000000 ChiantiPy-0.9.5/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.5/docs/build/html/_sources/notes.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_sources/quick_start.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)      284 2018-10-08 17:17:38.000000 ChiantiPy-0.9.5/docs/build/html/_sources/resources.rst.txt
+-rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.5/docs/build/html/_sources/tutorial.rst.txt
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/_static/
+-rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/2.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)      673 2017-08-29 15:11:19.000000 ChiantiPy-0.9.5/docs/build/html/_static/ajax-loader.gif
+-rw-r--r--   0 ken       (1000) users      (100)    10716 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/basic.css
+-rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/bunch_selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/chiantipy_logo.png
+-rw-r--r--   0 ken       (1000) users      (100)      756 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/comment-bright.png
+-rw-r--r--   0 ken       (1000) users      (100)      829 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/comment-close.png
+-rw-r--r--   0 ken       (1000) users      (100)      641 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/comment.png
+-rw-r--r--   0 ken       (1000) users      (100)      107 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/contents.png
+-rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/continuum_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)     9224 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/doctools.js
+-rw-r--r--   0 ken       (1000) users      (100)      275 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 ken       (1000) users      (100)      222 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/down-pressed.png
+-rw-r--r--   0 ken       (1000) users      (100)      202 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/down.png
+-rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt.png
+-rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt_alternate.png
+-rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.ratio.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.ratio.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.popplot.png
+-rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.rel.emiss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum2.png
+-rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum_label.png
+-rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14_intensity_plot_log.png
+-rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe14_intensity_plot_log_index2.png
+-rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe_12_wvlranges_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe_13_14_15_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe_25_ff_fb_tp_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/fe_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)      286 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/file.png
+-rw-r--r--   0 ken       (1000) users      (100)   263767 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/jquery-3.1.0.js
+-rw-r--r--   0 ken       (1000) users      (100)   268039 2018-07-16 07:59:17.000000 ChiantiPy-0.9.5/docs/build/html/_static/jquery-3.2.1.js
+-rw-r--r--   0 ken       (1000) users      (100)    86659 2019-03-18 15:58:41.000000 ChiantiPy-0.9.5/docs/build/html/_static/jquery.js
+-rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/minus.png
+-rw-r--r--   0 ken       (1000) users      (100)      120 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/navigation.png
+-rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_t_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_t_ratio_top7.png
+-rw-r--r--   0 ken       (1000) users      (100)       90 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/plus.png
+-rw-r--r--   0 ken       (1000) users      (100)     4395 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/pygments.css
+-rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/radloss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25449 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_10_20.png
+-rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_3panel.png
+-rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_integrated.png
+-rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_w_si_9.png
+-rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/spectrum_2e7_1.84_1.90.png
+-rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/build/html/_static/sphinxdoc.css
+-rw-r--r--   0 ken       (1000) users      (100)      707 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/build/html/_static/theme.conf
+-rw-r--r--   0 ken       (1000) users      (100)    35168 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 ken       (1000) users      (100)    12140 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/underscore.js
+-rw-r--r--   0 ken       (1000) users      (100)      214 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/up-pressed.png
+-rw-r--r--   0 ken       (1000) users      (100)      203 2017-10-22 11:19:57.000000 ChiantiPy-0.9.5/docs/build/html/_static/up.png
+-rw-r--r--   0 ken       (1000) users      (100)    25355 2018-07-16 07:59:17.000000 ChiantiPy-0.9.5/docs/build/html/_static/websupport.js
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/build/html/api/
+-rw-r--r--   0 ken       (1000) users      (100)     8727 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.gui_cl.html
+-rw-r--r--   0 ken       (1000) users      (100)    13441 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.gui_qt5.html
+-rw-r--r--   0 ken       (1000) users      (100)     6942 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.html
+-rw-r--r--   0 ken       (1000) users      (100)    20146 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.base.html
+-rw-r--r--   0 ken       (1000) users      (100)    95842 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.core.html
+-rw-r--r--   0 ken       (1000) users      (100)    14706 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.core.tests.html
+-rw-r--r--   0 ken       (1000) users      (100)    15673 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.fortranformat.html
+-rw-r--r--   0 ken       (1000) users      (100)    14525 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.html
+-rw-r--r--   0 ken       (1000) users      (100)    19240 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.model.html
+-rw-r--r--   0 ken       (1000) users      (100)     6404 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.tests.html
+-rw-r--r--   0 ken       (1000) users      (100)   101217 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.tools.html
+-rw-r--r--   0 ken       (1000) users      (100)    11990 2019-10-19 16:07:39.000000 ChiantiPy-0.9.5/docs/build/html/api/index.html
+-rw-r--r--   0 ken       (1000) users      (100)    10213 2018-10-22 16:22:47.000000 ChiantiPy-0.9.5/docs/build/html/api/modules.html
+-rw-r--r--   0 ken       (1000) users      (100)     4509 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/bugs.html
+-rw-r--r--   0 ken       (1000) users      (100)    15005 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/changelog.html
+-rw-r--r--   0 ken       (1000) users      (100)  3563520 2018-10-08 17:48:45.000000 ChiantiPy-0.9.5/docs/build/html/chiantdoc-0.8.0.tar
+-rw-r--r--   0 ken       (1000) users      (100)    46780 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/genindex.html
+-rw-r--r--   0 ken       (1000) users      (100)    13411 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/getting_started.html
+-rw-r--r--   0 ken       (1000) users      (100)    12415 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/index.html
+-rw-r--r--   0 ken       (1000) users      (100)    11820 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/notes.html
+-rw-r--r--   0 ken       (1000) users      (100)     2383 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/objects.inv
+-rw-r--r--   0 ken       (1000) users      (100)    13536 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/py-modindex.html
+-rw-r--r--   0 ken       (1000) users      (100)    88264 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/quick_start.html
+-rw-r--r--   0 ken       (1000) users      (100)     5055 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/resources.html
+-rw-r--r--   0 ken       (1000) users      (100)     4060 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/search.html
+-rw-r--r--   0 ken       (1000) users      (100)    34448 2019-10-19 16:24:03.000000 ChiantiPy-0.9.5/docs/build/html/searchindex.js
+-rw-r--r--   0 ken       (1000) users      (100)    31792 2019-10-19 16:02:02.000000 ChiantiPy-0.9.5/docs/build/html/tutorial.html
+-rw-r--r--   0 ken       (1000) users      (100)    13255 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/index.html
+-rw-r--r--   0 ken       (1000) users      (100)    11820 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/notes.html
+-rw-r--r--   0 ken       (1000) users      (100)     2383 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/objects.inv
+-rw-r--r--   0 ken       (1000) users      (100)    13536 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/py-modindex.html
+-rw-r--r--   0 ken       (1000) users      (100)    88264 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/quick_start.html
+-rw-r--r--   0 ken       (1000) users      (100)     5055 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/resources.html
+-rw-r--r--   0 ken       (1000) users      (100)     4060 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/search.html
+-rw-r--r--   0 ken       (1000) users      (100)    34868 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/searchindex.js
+-rw-r--r--   0 ken       (1000) users      (100)    31792 2020-02-19 16:54:41.000000 ChiantiPy-0.9.5/docs/build/tutorial.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/
+-rw-r--r--   0 ken       (1000) users      (100)     5226 2018-10-08 15:11:34.000000 ChiantiPy-0.9.5/docs/source/IDL_intro.rst
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/_static/
+-rw-r--r--   0 ken       (1000) users      (100)    19274 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/2.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    37785 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/bunch_selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    26923 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/source/_static/chiantipy_logo.png
+-rw-r--r--   0 ken       (1000) users      (100)    38813 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/continuum_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    37901 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt.png
+-rw-r--r--   0 ken       (1000) users      (100)     6173 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt.selector.png
+-rw-r--r--   0 ken       (1000) users      (100)    24645 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt_alternate.png
+-rw-r--r--   0 ken       (1000) users      (100)    27494 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.int.ratio.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    22706 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.int.ratio.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    89576 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.int.vs.d.png
+-rw-r--r--   0 ken       (1000) users      (100)    67386 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.int.vs.t.png
+-rw-r--r--   0 ken       (1000) users      (100)    40463 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.popplot.png
+-rw-r--r--   0 ken       (1000) users      (100)    34091 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.rel.emiss.png
+-rw-r--r--   0 ken       (1000) users      (100)    25939 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    34024 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum2.png
+-rw-r--r--   0 ken       (1000) users      (100)    43293 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum_label.png
+-rw-r--r--   0 ken       (1000) users      (100)    22888 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14_intensity_plot_log.png
+-rw-r--r--   0 ken       (1000) users      (100)    23256 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe14_intensity_plot_log_index2.png
+-rw-r--r--   0 ken       (1000) users      (100)    25159 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe_12_wvlranges_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    40658 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/source/_static/fe_13_14_15_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    37501 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/fe_25_ff_fb_tp_2e7_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    85621 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/source/_static/fe_ioneq.png
+-rw-r--r--   0 ken       (1000) users      (100)    34099 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_spectrum.png
+-rw-r--r--   0 ken       (1000) users      (100)    28764 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_t_ratio.png
+-rw-r--r--   0 ken       (1000) users      (100)    76222 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_t_ratio_top7.png
+-rw-r--r--   0 ken       (1000) users      (100)    26739 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/radloss.png
+-rw-r--r--   0 ken       (1000) users      (100)    45710 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_10_20.png
+-rw-r--r--   0 ken       (1000) users      (100)    30420 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_1_10.png
+-rw-r--r--   0 ken       (1000) users      (100)    65623 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_3panel.png
+-rw-r--r--   0 ken       (1000) users      (100)    37348 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_integrated.png
+-rw-r--r--   0 ken       (1000) users      (100)    47899 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_w_si_9.png
+-rw-r--r--   0 ken       (1000) users      (100)    32532 2018-10-08 15:12:33.000000 ChiantiPy-0.9.5/docs/source/_static/spectrum_2e7_1.84_1.90.png
+-rw-r--r--   0 ken       (1000) users      (100)     6228 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/source/_static/sphinxdoc.css
+-rw-r--r--   0 ken       (1000) users      (100)      707 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/source/_static/theme.conf
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/_templates/
+-rw-r--r--   0 ken       (1000) users      (100)      411 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/source/_templates/layout.html
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/api/
+-rw-r--r--   0 ken       (1000) users      (100)      388 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.Gui.gui_cl.rst
+-rw-r--r--   0 ken       (1000) users      (100)      566 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.Gui.gui_qt5.rst
+-rw-r--r--   0 ken       (1000) users      (100)      258 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.Gui.rst
+-rw-r--r--   0 ken       (1000) users      (100)      539 2018-10-14 17:58:17.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.base.rst
+-rw-r--r--   0 ken       (1000) users      (100)     1405 2018-10-08 16:43:30.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.core.rst
+-rw-r--r--   0 ken       (1000) users      (100)     1001 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.core.tests.rst
+-rw-r--r--   0 ken       (1000) users      (100)      857 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.fortranformat.rst
+-rw-r--r--   0 ken       (1000) users      (100)      352 2019-10-19 16:23:55.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.model.rst
+-rw-r--r--   0 ken       (1000) users      (100)      507 2019-10-19 16:05:27.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.rst
+-rw-r--r--   0 ken       (1000) users      (100)      382 2018-10-08 16:29:38.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.tests.rst
+-rw-r--r--   0 ken       (1000) users      (100)     1491 2019-08-11 15:27:08.000000 ChiantiPy-0.9.5/docs/source/api/ChiantiPy.tools.rst
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/api/_static/
+-rw-r--r--   0 ken       (1000) users      (100)    26923 2018-10-24 16:45:03.000000 ChiantiPy-0.9.5/docs/source/api/_static/chiantipy_logo.png
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/docs/source/api/_templates/
+-rw-r--r--   0 ken       (1000) users      (100)      411 2018-10-24 16:48:23.000000 ChiantiPy-0.9.5/docs/source/api/_templates/layout.html
+-rw-r--r--   0 ken       (1000) users      (100)      451 2018-10-08 17:16:04.000000 ChiantiPy-0.9.5/docs/source/api/index.rst
+-rw-r--r--   0 ken       (1000) users      (100)      343 2018-10-08 15:11:15.000000 ChiantiPy-0.9.5/docs/source/bugs.rst
+-rw-r--r--   0 ken       (1000) users      (100)     8017 2020-02-19 16:44:39.000000 ChiantiPy-0.9.5/docs/source/changelog.rst
+-rw-r--r--   0 ken       (1000) users      (100)     5525 2020-02-19 16:34:33.000000 ChiantiPy-0.9.5/docs/source/conf.py
+-rw-r--r--   0 ken       (1000) users      (100)     4921 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/source/getting_started.rst
+-rw-r--r--   0 ken       (1000) users      (100)     1633 2020-02-19 16:33:55.000000 ChiantiPy-0.9.5/docs/source/index.rst
+-rw-r--r--   0 ken       (1000) users      (100)     2947 2018-10-08 15:11:41.000000 ChiantiPy-0.9.5/docs/source/notes.rst
+-rw-r--r--   0 ken       (1000) users      (100)    22159 2019-10-08 17:17:03.000000 ChiantiPy-0.9.5/docs/source/quick_start.rst
+-rw-r--r--   0 ken       (1000) users      (100)      284 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/docs/source/resources.rst
+-rw-r--r--   0 ken       (1000) users      (100)    13575 2018-10-08 15:12:03.000000 ChiantiPy-0.9.5/docs/source/tutorial.rst
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/jupyter_notebooks/
+-rw-r--r--   0 ken       (1000) users      (100)   278737 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/jupyter_notebooks/QuickStart.html
+-rw-r--r--   0 ken       (1000) users      (100)    41104 2019-08-29 15:43:16.000000 ChiantiPy-0.9.5/jupyter_notebooks/QuickStart.ipynb
+-rw-r--r--   0 ken       (1000) users      (100)     1138 2020-02-18 17:48:14.000000 ChiantiPy-0.9.5/jupyter_notebooks/README.txt
+-rw-r--r--   0 ken       (1000) users      (100)    39643 2020-02-12 15:35:41.000000 ChiantiPy-0.9.5/jupyter_notebooks/fe_13_demo_chi2.ipynb
+-rw-r--r--   0 ken       (1000) users      (100)    13083 2020-02-12 15:35:10.000000 ChiantiPy-0.9.5/jupyter_notebooks/fe_13_demo_make_model.ipynb
+-rw-r--r--   0 ken       (1000) users      (100)    43489 2020-02-12 15:35:19.000000 ChiantiPy-0.9.5/jupyter_notebooks/fe_13_demo_mcmc.ipynb
+-rw-r--r--   0 ken       (1000) users      (100)      790 2020-02-12 15:34:55.000000 ChiantiPy-0.9.5/jupyter_notebooks/tab2_1993_qs_fe_13.json
+drwxr-xr-x   0 ken       (1000) users      (100)        0 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/licenses/
+-rw-r--r--   0 ken       (1000) users      (100)      768 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/licenses/LICENSE
+-rw-r--r--   0 ken       (1000) users      (100)     1075 2016-07-14 19:28:36.000000 ChiantiPy-0.9.5/licenses/LICENSE.fortranformat
+-rw-r--r--   0 ken       (1000) users      (100)       59 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/pytest.ini
+-rw-r--r--   0 ken       (1000) users      (100)       81 2017-02-18 15:57:42.000000 ChiantiPy-0.9.5/readthedocs.yml
+-rw-r--r--   0 ken       (1000) users      (100)       35 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/requirements.txt
+-rw-r--r--   0 ken       (1000) users      (100)      146 2019-06-11 16:14:41.000000 ChiantiPy-0.9.5/rtd_environment.yml
+-rw-r--r--   0 ken       (1000) users      (100)      543 2020-02-19 17:05:48.000000 ChiantiPy-0.9.5/setup.cfg
+-rw-r--r--   0 ken       (1000) users      (100)      909 2020-02-19 16:34:54.000000 ChiantiPy-0.9.5/setup.py
```

### Comparing `ChiantiPy-0.9.4/.gitignore` & `ChiantiPy-0.9.5/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # Other generated files
 */cython_version.py
 htmlcov
 .coverage
 MANIFEST
 
 # Sphinx
-docs/source/api
+# kpd commented out the api stuff
+#docs/source/api
 docs/_build
 
 # Eclipse editor project files
 .project
 .pydevproject
 .settings
```

### Comparing `ChiantiPy-0.9.4/ChiantiPy/Gui/__init__.py` & `ChiantiPy-0.9.5/ChiantiPy/Gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/Gui/gui_cl/gui.py` & `ChiantiPy-0.9.5/ChiantiPy/Gui/gui_cl/gui.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/gui.py` & `ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/gui.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/Gui/gui_qt5/ui.py` & `ChiantiPy-0.9.5/ChiantiPy/Gui/gui_qt5/ui.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/__init__gh.py` & `ChiantiPy-0.9.5/ChiantiPy/__init__gh.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/__init__kpd.py` & `ChiantiPy-0.9.5/ChiantiPy/__init__kpd.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/__init_kpd__.py` & `ChiantiPy-0.9.5/ChiantiPy/__init_kpd__.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/base/_IonTrails.py` & `ChiantiPy-0.9.5/ChiantiPy/base/_IonTrails.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,18 +496,14 @@
         # need to make sure there are no negative values before plotting
         good = intensity > 0.
         intensMin = intensity[good].min()
         bad = intensity <= 0.
         intensity[bad] = intensMin
 
         ylabel='Intensity relative to '+maxWvl
-        if ionNum == 1:
-            title=self.Spectroscopic
-        else:
-            title = ''
 
         if ndens==1 and ntemp==1:
             print(' only a single temperature and eDensity')
             return
         elif ndens == 1:
             xlbl='Temperature (K)'
             xvalues=self.Temperature
```

### Comparing `ChiantiPy-0.9.4/ChiantiPy/base/_IoneqOne.py` & `ChiantiPy-0.9.5/ChiantiPy/base/_IoneqOne.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/base/_SpecTrails.py` & `ChiantiPy-0.9.5/ChiantiPy/base/_SpecTrails.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/Continuum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/Continuum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/Ion.py` & `ChiantiPy-0.9.5/ChiantiPy/core/Ion.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/Ioneq.py` & `ChiantiPy-0.9.5/ChiantiPy/core/Ioneq.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/IpyMspectrum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/IpyMspectrum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/Mspectrum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/Mspectrum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/RadLoss.py` & `ChiantiPy-0.9.5/ChiantiPy/core/RadLoss.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/Spectrum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/Spectrum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Continuum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Continuum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Ion.py` & `ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Ion.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Ioneq.py` & `ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Ioneq.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/tests/test_Spectrum.py` & `ChiantiPy-0.9.5/ChiantiPy/core/tests/test_Spectrum.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/core/tests/test_spectrum_api.py` & `ChiantiPy-0.9.5/ChiantiPy/core/tests/test_spectrum_api.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/COPYING.txt` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/COPYING.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/FortranRecordReader.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/FortranRecordReader.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/FortranRecordWriter.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/FortranRecordWriter.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_edit_descriptors.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_edit_descriptors.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_input.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_input.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_lexer.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_lexer.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_misc.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_misc.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_output.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_output.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/_parser.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/_parser.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/fortranformat/config.py` & `ChiantiPy-0.9.5/ChiantiPy/fortranformat/config.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/model/Maker.py` & `ChiantiPy-0.9.5/ChiantiPy/model/Maker.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tests/coveragerc` & `ChiantiPy-0.9.5/ChiantiPy/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/archival.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/archival.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/constants.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/constants.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/data.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/data.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/filters.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/filters.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/io.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/io.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/mputil.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/mputil.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/sources.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/sources.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy/tools/util.py` & `ChiantiPy-0.9.5/ChiantiPy/tools/util.py`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/ChiantiPy.egg-info/PKG-INFO` & `ChiantiPy-0.9.5/ChiantiPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ChiantiPy
-Version: 0.9.4
+Version: 0.9.5
 Summary: a Python interface to the CHIANTI atomic database for astrophysical spectroscopy
 Home-page: https://github.com/chianti-atomic/ChiantiPy
 Author: Ken Dere
 Author-email: kdere@gmu.edu
 License: ISC
 Description: ChiantiPy - Version 0.9.4
         =========================
```

### Comparing `ChiantiPy-0.9.4/ChiantiPy.egg-info/SOURCES.txt` & `ChiantiPy-0.9.5/ChiantiPy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 docs/build/.doctrees/api/ChiantiPy.Gui.gui_cl.doctree
 docs/build/.doctrees/api/ChiantiPy.Gui.gui_qt5.doctree
 docs/build/.doctrees/api/ChiantiPy.base.doctree
 docs/build/.doctrees/api/ChiantiPy.core.doctree
 docs/build/.doctrees/api/ChiantiPy.core.tests.doctree
 docs/build/.doctrees/api/ChiantiPy.doctree
 docs/build/.doctrees/api/ChiantiPy.fortranformat.doctree
+docs/build/.doctrees/api/ChiantiPy.model.doctree
 docs/build/.doctrees/api/ChiantiPy.tests.doctree
 docs/build/.doctrees/api/ChiantiPy.tools.doctree
 docs/build/.doctrees/api/index.doctree
 docs/build/.doctrees/api/modules.doctree
 docs/build/_images/2.selector.png
 docs/build/_images/bunch_selector.png
 docs/build/_images/continuum_2e7_1_10.png
@@ -155,14 +156,15 @@
 docs/build/_sources/api/ChiantiPy.Gui.gui_cl.rst.txt
 docs/build/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt
 docs/build/_sources/api/ChiantiPy.Gui.rst.txt
 docs/build/_sources/api/ChiantiPy.base.rst.txt
 docs/build/_sources/api/ChiantiPy.core.rst.txt
 docs/build/_sources/api/ChiantiPy.core.tests.rst.txt
 docs/build/_sources/api/ChiantiPy.fortranformat.rst.txt
+docs/build/_sources/api/ChiantiPy.model.rst.txt
 docs/build/_sources/api/ChiantiPy.rst.txt
 docs/build/_sources/api/ChiantiPy.tests.rst.txt
 docs/build/_sources/api/ChiantiPy.tools.rst.txt
 docs/build/_sources/api/index.rst.txt
 docs/build/_sources/api/modules.rst.txt
 docs/build/_static/2.selector.png
 docs/build/_static/ajax-loader.gif
@@ -226,14 +228,15 @@
 docs/build/api/ChiantiPy.Gui.gui_qt5.html
 docs/build/api/ChiantiPy.Gui.html
 docs/build/api/ChiantiPy.base.html
 docs/build/api/ChiantiPy.core.html
 docs/build/api/ChiantiPy.core.tests.html
 docs/build/api/ChiantiPy.fortranformat.html
 docs/build/api/ChiantiPy.html
+docs/build/api/ChiantiPy.model.html
 docs/build/api/ChiantiPy.tests.html
 docs/build/api/ChiantiPy.tools.html
 docs/build/api/index.html
 docs/build/api/modules.html
 docs/build/doctrees/IDL_intro.doctree
 docs/build/doctrees/bugs.doctree
 docs/build/doctrees/changelog.doctree
@@ -455,9 +458,14 @@
 docs/source/api/ChiantiPy.tests.rst
 docs/source/api/ChiantiPy.tools.rst
 docs/source/api/index.rst
 docs/source/api/_static/chiantipy_logo.png
 docs/source/api/_templates/layout.html
 jupyter_notebooks/QuickStart.html
 jupyter_notebooks/QuickStart.ipynb
+jupyter_notebooks/README.txt
+jupyter_notebooks/fe_13_demo_chi2.ipynb
+jupyter_notebooks/fe_13_demo_make_model.ipynb
+jupyter_notebooks/fe_13_demo_mcmc.ipynb
+jupyter_notebooks/tab2_1993_qs_fe_13.json
 licenses/LICENSE
 licenses/LICENSE.fortranformat
```

### Comparing `ChiantiPy-0.9.4/MANIFEST.in` & `ChiantiPy-0.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/PKG-INFO` & `ChiantiPy-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ChiantiPy
-Version: 0.9.4
+Version: 0.9.5
 Summary: a Python interface to the CHIANTI atomic database for astrophysical spectroscopy
 Home-page: https://github.com/chianti-atomic/ChiantiPy
 Author: Ken Dere
 Author-email: kdere@gmu.edu
 License: ISC
 Description: ChiantiPy - Version 0.9.4
         =========================
```

### Comparing `ChiantiPy-0.9.4/README` & `ChiantiPy-0.9.5/README`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/README.md` & `ChiantiPy-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ChiantiPy - Version 0.9.4
+# ChiantiPy - Version 0.9.5
 [![Documentation Status](http://readthedocs.org/projects/chiantipy/badge/?version=latest)](http://chiantipy.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/chianti-atomic/ChiantiPy/badge.svg?branch=master)](https://coveralls.io/github/chianti-atomic/ChiantiPy?branch=master)
 [![ascl:1308.017](https://img.shields.io/badge/ascl-1308.017-blue.svg?colorB=262255)](http://ascl.net/1308.017)
 
 ChiantiPy is the Python interface to the [CHIANTI atomic database](http://www.chiantidatabase.org) for astrophysical spectroscopy.  It provides the capability to calculate the emission line and continuum spectrum of an optically thin plasma based on the data in the CHIANTI database.
 
 ## What is CHIANTI?
```

### Comparing `ChiantiPy-0.9.4/README.rst` & `ChiantiPy-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/0-notes.txt` & `ChiantiPy-0.9.5/docs/0-notes.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/Makefile` & `ChiantiPy-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/IDL_intro.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/IDL_intro.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.gui_cl.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.gui_cl.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.Gui.gui_qt5.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.Gui.gui_qt5.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.base.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.base.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.core.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.core.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.core.tests.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.core.tests.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.doctree`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 952b 1400 0000 0000 008c 0e64 6f63  ...+.........doc
+00000000: 8004 9546 1400 0000 0000 008c 0e64 6f63  ...F.........doc
 00000010: 7574 696c 732e 6e6f 6465 7394 8c08 646f  utils.nodes...do
 00000020: 6375 6d65 6e74 9493 9429 8194 7d94 288c  cument...)..}.(.
 00000030: 0972 6177 736f 7572 6365 948c 0094 8c08  .rawsource......
 00000040: 6368 696c 6472 656e 945d 9468 008c 0773  children.].h...s
 00000050: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000060: 0568 0668 075d 9428 6800 8c05 7469 746c  .h.h.].(h...titl
 00000070: 6594 9394 2981 947d 9428 6805 8c11 4368  e...)..}.(h...Ch
@@ -41,284 +41,286 @@
 00000280: 7394 5d94 284e 8c11 6170 692f 4368 6961  s.].(N..api/Chia
 00000290: 6e74 6950 792e 4775 6994 8694 4e8c 1261  ntiPy.Gui...N..a
 000002a0: 7069 2f43 6869 616e 7469 5079 2e62 6173  pi/ChiantiPy.bas
 000002b0: 6594 8694 4e8c 1261 7069 2f43 6869 616e  e...N..api/Chian
 000002c0: 7469 5079 2e63 6f72 6594 8694 4e8c 1b61  tiPy.core...N..a
 000002d0: 7069 2f43 6869 616e 7469 5079 2e66 6f72  pi/ChiantiPy.for
 000002e0: 7472 616e 666f 726d 6174 9486 944e 8c13  tranformat...N..
-000002f0: 6170 692f 4368 6961 6e74 6950 792e 7465  api/ChiantiPy.te
-00000300: 7374 7394 8694 4e8c 1361 7069 2f43 6869  sts...N..api/Chi
-00000310: 616e 7469 5079 2e74 6f6f 6c73 9486 9465  antiPy.tools...e
-00000320: 8c0c 696e 636c 7564 6566 696c 6573 945d  ..includefiles.]
-00000330: 9428 6850 6852 6854 6856 6858 685a 658c  .(hPhRhThVhXhZe.
-00000340: 086d 6178 6465 7074 6894 4aff ffff ff8c  .maxdepth.J.....
-00000350: 0763 6170 7469 6f6e 944e 8c04 676c 6f62  .caption.N..glob
-00000360: 9489 8c06 6869 6464 656e 9489 8c0d 696e  ....hidden....in
-00000370: 636c 7564 6568 6964 6465 6e94 898c 086e  cludehidden....n
-00000380: 756d 6265 7265 6494 4b00 8c0a 7469 746c  umbered.K...titl
-00000390: 6573 6f6e 6c79 9489 7568 2968 4268 1b68  esonly..uh)hBh.h
-000003a0: 2a68 1c4b 0768 1a68 3e75 6261 681d 7d94  *h.K.h.h>ubah.}.
-000003b0: 2868 1f5d 9468 215d 948c 0f74 6f63 7472  (h.].h!]...toctr
-000003c0: 6565 2d77 7261 7070 6572 9461 6823 5d94  ee-wrapper.ah#].
-000003d0: 6825 5d94 6827 5d94 7568 2968 3c68 1a68  h%].h'].uh)h<h.h
-000003e0: 2b68 0168 0368 1b68 2a68 1c4b 0f75 6265  +h.h.h.h*h.K.ube
-000003f0: 681d 7d94 2868 1f5d 948c 0b73 7562 7061  h.}.(h.]...subpa
-00000400: 636b 6167 6573 9461 6821 5d94 6823 5d94  ckages.ah!].h#].
-00000410: 8c0b 7375 6270 6163 6b61 6765 7394 6168  ..subpackages.ah
-00000420: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
-00000430: 6801 6803 681b 682a 681c 4b05 7562 680a  h.h.h.h*h.K.ubh.
-00000440: 2981 947d 9428 6805 6806 6807 5d94 680f  )..}.(h.h.h.].h.
-00000450: 2981 947d 9428 6805 8c0a 5375 626d 6f64  )..}.(h...Submod
-00000460: 756c 6573 9468 075d 9468 158c 0a53 7562  ules.h.].h...Sub
-00000470: 6d6f 6475 6c65 7394 8594 8194 7d94 2868  modules.....}.(h
-00000480: 0568 7968 1a68 7768 0168 0368 1b4e 681c  .hyh.hwh.h.h.Nh.
-00000490: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
-000004a0: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-000004b0: 680e 681a 6874 6801 6803 681b 682a 681c  h.h.hth.h.h.h*h.
-000004c0: 4b11 7562 6168 1d7d 9428 681f 5d94 8c0a  K.ubah.}.(h.]...
-000004d0: 7375 626d 6f64 756c 6573 9461 6821 5d94  submodules.ah!].
-000004e0: 6823 5d94 8c0a 7375 626d 6f64 756c 6573  h#]...submodules
-000004f0: 9461 6825 5d94 6827 5d94 7568 2968 0968  .ah%].h'].uh)h.h
-00000500: 1a68 0b68 0168 0368 1b68 2a68 1c4b 1175  .h.h.h.h.h*h.K.u
-00000510: 6268 0a29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-00000520: 9428 680f 2981 947d 9428 6805 8c19 4368  .(h.)..}.(h...Ch
-00000530: 6961 6e74 6950 795c 2e76 6572 7369 6f6e  iantiPy\.version
-00000540: 206d 6f64 756c 6594 6807 5d94 6815 8c18   module.h.].h...
-00000550: 4368 6961 6e74 6950 792e 7665 7273 696f  ChiantiPy.versio
-00000560: 6e20 6d6f 6475 6c65 9485 9481 947d 9428  n module.....}.(
-00000570: 6805 8c19 4368 6961 6e74 6950 795c 2e76  h...ChiantiPy\.v
-00000580: 6572 7369 6f6e 206d 6f64 756c 6594 681a  ersion module.h.
-00000590: 6890 6801 6803 681b 4e68 1c4e 7562 6168  h.h.h.h.Nh.Nubah
-000005a0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-000005b0: 6825 5d94 6827 5d94 7568 2968 0e68 1a68  h%].h'].uh)h.h.h
-000005c0: 8d68 0168 0368 1b68 2a68 1c4b 1575 6268  .h.h.h.h*h.K.ubh
-000005d0: 418c 0569 6e64 6578 9493 9429 8194 7d94  A..index...)..}.
-000005e0: 2868 0568 0668 075d 9468 1d7d 9428 681f  (h.h.h.].h.}.(h.
-000005f0: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00000600: 5d94 8c07 656e 7472 6965 7394 5d94 288c  ]...entries.].(.
-00000610: 0673 696e 676c 6594 8c1a 4368 6961 6e74  .single...Chiant
-00000620: 6950 792e 7665 7273 696f 6e20 286d 6f64  iPy.version (mod
-00000630: 756c 6529 948c 186d 6f64 756c 652d 4368  ule)...module-Ch
-00000640: 6961 6e74 6950 792e 7665 7273 696f 6e94  iantiPy.version.
-00000650: 6806 4e74 9461 7568 2968 9f68 1a68 8d68  h.Nt.auh)h.h.h.h
-00000660: 0168 0368 1b8c 472f 6461 7461 322f 6768  .h.h..G/data2/gh
-00000670: 2f43 6869 616e 7469 5079 2f43 6869 616e  /ChiantiPy/Chian
-00000680: 7469 5079 2f76 6572 7369 6f6e 2e70 793a  tiPy/version.py:
-00000690: 646f 6373 7472 696e 6720 6f66 2043 6869  docstring of Chi
-000006a0: 616e 7469 5079 2e76 6572 7369 6f6e 9468  antiPy.version.h
-000006b0: 1c4b 0175 6268 008c 0970 6172 6167 7261  .K.ubh...paragra
-000006c0: 7068 9493 9429 8194 7d94 2868 058c 2c74  ph...)..}.(h..,t
-000006d0: 6865 2063 7572 7265 6e74 2076 6572 7369  he current versi
-000006e0: 6f6e 206f 6620 7468 6520 4368 6961 6e74  on of the Chiant
-000006f0: 6950 7920 7061 636b 6167 6594 6807 5d94  iPy package.h.].
-00000700: 6815 8c2c 7468 6520 6375 7272 656e 7420  h..,the current 
-00000710: 7665 7273 696f 6e20 6f66 2074 6865 2043  version of the C
-00000720: 6869 616e 7469 5079 2070 6163 6b61 6765  hiantiPy package
-00000730: 9485 9481 947d 9428 6805 68b5 681a 68b3  .....}.(h.h.h.h.
-00000740: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
-00000750: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00000760: 5d94 6827 5d94 7568 2968 b168 1b8c 472f  ].h'].uh)h.h..G/
-00000770: 6461 7461 322f 6768 2f43 6869 616e 7469  data2/gh/Chianti
-00000780: 5079 2f43 6869 616e 7469 5079 2f76 6572  Py/ChiantiPy/ver
-00000790: 7369 6f6e 2e70 793a 646f 6373 7472 696e  sion.py:docstrin
-000007a0: 6720 6f66 2043 6869 616e 7469 5079 2e76  g of ChiantiPy.v
-000007b0: 6572 7369 6f6e 9468 1c4b 0168 1a68 8d68  ersion.h.K.h.h.h
-000007c0: 0168 0375 6265 681d 7d94 2868 1f5d 9428  .h.ubeh.}.(h.].(
-000007d0: 8c18 6d6f 6475 6c65 2d43 6869 616e 7469  ..module-Chianti
-000007e0: 5079 2e76 6572 7369 6f6e 948c 1863 6869  Py.version...chi
-000007f0: 616e 7469 7079 2d76 6572 7369 6f6e 2d6d  antipy-version-m
-00000800: 6f64 756c 6594 6568 215d 9468 235d 948c  odule.eh!].h#]..
-00000810: 1863 6869 616e 7469 7079 2e76 6572 7369  .chiantipy.versi
-00000820: 6f6e 206d 6f64 756c 6594 6168 255d 9468  on module.ah%].h
-00000830: 275d 9475 6829 6809 681a 680b 6801 6803  '].uh)h.h.h.h.h.
-00000840: 681b 682a 681c 4b15 7562 680a 2981 947d  h.h*h.K.ubh.)..}
-00000850: 9428 6805 6806 6807 5d94 2868 0f29 8194  .(h.h.h.].(h.)..
-00000860: 7d94 2868 058c 0f4d 6f64 756c 6520 636f  }.(h...Module co
-00000870: 6e74 656e 7473 9468 075d 9468 158c 0f4d  ntents.h.].h...M
-00000880: 6f64 756c 6520 636f 6e74 656e 7473 9485  odule contents..
-00000890: 9481 947d 9428 6805 68d0 681a 68ce 6801  ...}.(h.h.h.h.h.
-000008a0: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
-000008b0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
-000008c0: 6827 5d94 7568 2968 0e68 1a68 cb68 0168  h'].uh)h.h.h.h.h
-000008d0: 0368 1b68 2a68 1c4b 1e75 6268 a029 8194  .h.h*h.K.ubh.)..
-000008e0: 7d94 2868 0568 0668 075d 9468 1d7d 9428  }.(h.h.h.].h.}.(
-000008f0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
-00000900: 6827 5d94 8c07 656e 7472 6965 7394 5d94  h']...entries.].
-00000910: 2868 ac8c 1243 6869 616e 7469 5079 2028  (h...ChiantiPy (
-00000920: 6d6f 6475 6c65 2994 8c10 6d6f 6475 6c65  module)...module
-00000930: 2d43 6869 616e 7469 5079 9468 064e 7494  -ChiantiPy.h.Nt.
-00000940: 6175 6829 689f 681a 68cb 6801 6803 681b  auh)h.h.h.h.h.h.
-00000950: 8c40 2f64 6174 6132 2f67 682f 4368 6961  .@/data2/gh/Chia
-00000960: 6e74 6950 792f 4368 6961 6e74 6950 792f  ntiPy/ChiantiPy/
-00000970: 5f5f 696e 6974 5f5f 2e70 793a 646f 6373  __init__.py:docs
-00000980: 7472 696e 6720 6f66 2043 6869 616e 7469  tring of Chianti
-00000990: 5079 9468 1c4b 0175 6268 b229 8194 7d94  Py.h.K.ubh.)..}.
-000009a0: 2868 058c 9d43 6869 616e 7469 5079 202d  (h...ChiantiPy -
-000009b0: 2043 4849 414e 5449 2050 7974 686f 6e20   CHIANTI Python 
-000009c0: 7061 636b 6167 6520 4361 6c63 756c 6174  package Calculat
-000009d0: 6573 2076 6172 696f 7573 2061 7370 6563  es various aspec
-000009e0: 7473 206f 6620 656d 6973 7369 6f6e 206c  ts of emission l
-000009f0: 696e 6573 0a61 6e64 2063 6f6e 7469 6e75  ines.and continu
-00000a00: 6120 6672 6f6d 2074 6865 2043 4849 414e  a from the CHIAN
-00000a10: 5449 2061 746f 6d69 6320 6461 7461 6261  TI atomic databa
-00000a20: 7365 2066 6f72 2061 7374 726f 7068 7973  se for astrophys
-00000a30: 6963 616c 2073 7065 6374 726f 7363 6f70  ical spectroscop
-00000a40: 792e 9468 075d 9468 158c 9d43 6869 616e  y..h.].h...Chian
-00000a50: 7469 5079 202d 2043 4849 414e 5449 2050  tiPy - CHIANTI P
-00000a60: 7974 686f 6e20 7061 636b 6167 6520 4361  ython package Ca
-00000a70: 6c63 756c 6174 6573 2076 6172 696f 7573  lculates various
-00000a80: 2061 7370 6563 7473 206f 6620 656d 6973   aspects of emis
-00000a90: 7369 6f6e 206c 696e 6573 0a61 6e64 2063  sion lines.and c
-00000aa0: 6f6e 7469 6e75 6120 6672 6f6d 2074 6865  ontinua from the
-00000ab0: 2043 4849 414e 5449 2061 746f 6d69 6320   CHIANTI atomic 
-00000ac0: 6461 7461 6261 7365 2066 6f72 2061 7374  database for ast
-00000ad0: 726f 7068 7973 6963 616c 2073 7065 6374  rophysical spect
-00000ae0: 726f 7363 6f70 792e 9485 9481 947d 9428  roscopy......}.(
-00000af0: 6805 68ed 681a 68eb 6801 6803 681b 4e68  h.h.h.h.h.h.h.Nh
-00000b00: 1c4e 7562 6168 1d7d 9428 681f 5d94 6821  .Nubah.}.(h.].h!
-00000b10: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00000b20: 2968 b168 1b8c 402f 6461 7461 322f 6768  )h.h..@/data2/gh
-00000b30: 2f43 6869 616e 7469 5079 2f43 6869 616e  /ChiantiPy/Chian
-00000b40: 7469 5079 2f5f 5f69 6e69 745f 5f2e 7079  tiPy/__init__.py
-00000b50: 3a64 6f63 7374 7269 6e67 206f 6620 4368  :docstring of Ch
-00000b60: 6961 6e74 6950 7994 681c 4b01 681a 68cb  iantiPy.h.K.h.h.
-00000b70: 6801 6803 7562 6568 1d7d 9428 681f 5d94  h.h.ubeh.}.(h.].
-00000b80: 288c 106d 6f64 756c 652d 4368 6961 6e74  (..module-Chiant
-00000b90: 6950 7994 8c0f 6d6f 6475 6c65 2d63 6f6e  iPy...module-con
-00000ba0: 7465 6e74 7394 6568 215d 9468 235d 948c  tents.eh!].h#]..
-00000bb0: 0f6d 6f64 756c 6520 636f 6e74 656e 7473  .module contents
-00000bc0: 9461 6825 5d94 6827 5d94 7568 2968 0968  .ah%].h'].uh)h.h
-00000bd0: 1a68 0b68 0168 0368 1b68 2a68 1c4b 1e75  .h.h.h.h.h*h.K.u
-00000be0: 6265 681d 7d94 2868 1f5d 948c 1163 6869  beh.}.(h.]...chi
-00000bf0: 616e 7469 7079 2d70 6163 6b61 6765 9461  antipy-package.a
-00000c00: 6821 5d94 6823 5d94 8c11 6368 6961 6e74  h!].h#]...chiant
-00000c10: 6970 7920 7061 636b 6167 6594 6168 255d  ipy package.ah%]
-00000c20: 9468 275d 9475 6829 6809 681a 6803 6801  .h'].uh)h.h.h.h.
-00000c30: 6803 681b 682a 681c 4b02 7562 6168 1d7d  h.h.h*h.K.ubah.}
-00000c40: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00000c50: 5d94 6827 5d94 8c06 736f 7572 6365 9468  ].h']...source.h
-00000c60: 2a75 6829 6801 8c0e 6375 7272 656e 745f  *uh)h...current_
-00000c70: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
-00000c80: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
-00000c90: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
-00000ca0: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
-00000cb0: 9394 2981 947d 9428 680e 4e8c 0967 656e  ..)..}.(h.N..gen
-00000cc0: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
-00000cd0: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
-00000ce0: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
-00000cf0: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
-00000d00: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
-00000d10: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
-00000d20: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
-00000d30: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
-00000d40: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
-00000d50: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
-00000d60: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
-00000d70: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
-00000d80: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
-00000d90: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
-00000da0: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
-00000db0: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
-00000dc0: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
-00000dd0: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
-00000de0: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
-00000df0: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
-00000e00: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00000e10: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
-00000e20: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
-00000e30: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
-00000e40: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
-00000e50: 7294 6a2e 0100 008c 0e65 7272 6f72 5f65  r.j......error_e
-00000e60: 6e63 6f64 696e 6794 8c05 5554 462d 3894  ncoding...UTF-8.
-00000e70: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
-00000e80: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
-00000e90: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
-00000ea0: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
-00000eb0: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
-00000ec0: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
-00000ed0: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
-00000ee0: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
-00000ef0: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
-00000f00: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
-00000f10: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
-00000f20: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
-00000f30: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
-00000f40: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
-00000f50: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
-00000f60: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
-00000f70: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
-00000f80: 5f73 6f75 7263 6594 682a 8c0c 5f64 6573  _source.h*.._des
-00000f90: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
-00000fa0: 6669 675f 6669 6c65 7394 5d94 8c0e 7065  fig_files.]...pe
-00000fb0: 705f 7265 6665 7265 6e63 6573 944e 8c0c  p_references.N..
-00000fc0: 7065 705f 6261 7365 5f75 726c 948c 2068  pep_base_url.. h
-00000fd0: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
-00000fe0: 6e2e 6f72 672f 6465 762f 7065 7073 2f94  n.org/dev/peps/.
-00000ff0: 8c15 7065 705f 6669 6c65 5f75 726c 5f74  ..pep_file_url_t
-00001000: 656d 706c 6174 6594 8c08 7065 702d 2530  emplate...pep-%0
-00001010: 3464 948c 0e72 6663 5f72 6566 6572 656e  4d...rfc_referen
-00001020: 6365 7394 4e8c 0c72 6663 5f62 6173 655f  ces.N..rfc_base_
-00001030: 7572 6c94 8c1c 6874 7470 733a 2f2f 746f  url...https://to
-00001040: 6f6c 732e 6965 7466 2e6f 7267 2f68 746d  ols.ietf.org/htm
-00001050: 6c2f 948c 0974 6162 5f77 6964 7468 944b  l/...tab_width.K
-00001060: 088c 1d74 7269 6d5f 666f 6f74 6e6f 7465  ...trim_footnote
-00001070: 5f72 6566 6572 656e 6365 5f73 7061 6365  _reference_space
-00001080: 9489 8c16 6669 6c65 5f69 6e73 6572 7469  ....file_inserti
-00001090: 6f6e 5f65 6e61 626c 6564 9488 8c0b 7261  on_enabled....ra
-000010a0: 775f 656e 6162 6c65 6494 4b01 8c10 7379  w_enabled.K...sy
-000010b0: 6e74 6178 5f68 6967 686c 6967 6874 948c  ntax_highlight..
-000010c0: 046c 6f6e 6794 8c0c 736d 6172 745f 7175  .long...smart_qu
-000010d0: 6f74 6573 9488 8c13 736d 6172 7471 756f  otes....smartquo
-000010e0: 7465 735f 6c6f 6361 6c65 7394 4e8c 1d63  tes_locales.N..c
-000010f0: 6861 7261 6374 6572 5f6c 6576 656c 5f69  haracter_level_i
-00001100: 6e6c 696e 655f 6d61 726b 7570 9489 8c0e  nline_markup....
-00001110: 646f 6374 6974 6c65 5f78 666f 726d 9489  doctitle_xform..
-00001120: 8c0d 646f 6369 6e66 6f5f 7866 6f72 6d94  ..docinfo_xform.
-00001130: 4b01 8c12 7365 6374 7375 6274 6974 6c65  K...sectsubtitle
-00001140: 5f78 666f 726d 9489 8c10 656d 6265 645f  _xform....embed_
-00001150: 7374 796c 6573 6865 6574 9489 8c15 636c  stylesheet....cl
-00001160: 6f61 6b5f 656d 6169 6c5f 6164 6472 6573  oak_email_addres
-00001170: 7365 7394 888c 0365 6e76 944e 8c0f 6765  ses....env.N..ge
-00001180: 7474 6578 745f 636f 6d70 6163 7494 8875  ttext_compact..u
-00001190: 628c 0872 6570 6f72 7465 7294 4e8c 1069  b..reporter.N..i
-000011a0: 6e64 6972 6563 745f 7461 7267 6574 7394  ndirect_targets.
-000011b0: 5d94 8c11 7375 6273 7469 7475 7469 6f6e  ]...substitution
-000011c0: 5f64 6566 7394 7d94 8c12 7375 6273 7469  _defs.}...substi
-000011d0: 7475 7469 6f6e 5f6e 616d 6573 947d 948c  tution_names.}..
-000011e0: 0872 6566 6e61 6d65 7394 7d94 8c06 7265  .refnames.}...re
-000011f0: 6669 6473 947d 948c 076e 616d 6569 6473  fids.}...nameids
-00001200: 947d 9428 6a08 0100 006a 0501 0000 6871  .}.(j....j....hq
-00001210: 686e 688a 6887 68c8 68c5 6a00 0100 0068  hnh.h.h.h.j....h
-00001220: fd75 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
-00001230: 286a 0801 0000 4e68 714e 688a 4e68 c84e  (j....NhqNh.Nh.N
-00001240: 6a00 0100 004e 7568 1f7d 9428 6a05 0100  j....Nuh.}.(j...
-00001250: 0068 0b68 6e68 2b68 8768 7468 c568 8d68  .h.hnh+h.hth.h.h
-00001260: c468 008c 0674 6172 6765 7494 9394 2981  .h...target...).
-00001270: 947d 9428 6805 6806 6807 5d94 681d 7d94  .}.(h.h.h.].h.}.
-00001280: 2868 1f5d 9468 c461 6821 5d94 6823 5d94  (h.].h.ah!].h#].
-00001290: 6825 5d94 6827 5d94 8c05 6973 6d6f 6494  h%].h']...ismod.
-000012a0: 8875 6829 6a70 0100 0068 1a68 8d68 0168  .uh)jp...h.h.h.h
-000012b0: 0368 1b68 b068 1c4b 0175 6268 fd68 cb68  .h.h.h.K.ubh.h.h
-000012c0: fc6a 7101 0000 2981 947d 9428 6805 6806  .jq...)..}.(h.h.
-000012d0: 6807 5d94 681d 7d94 2868 1f5d 9468 fc61  h.].h.}.(h.].h.a
-000012e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000012f0: 8c05 6973 6d6f 6494 8875 6829 6a70 0100  ..ismod..uh)jp..
-00001300: 0068 1a68 cb68 0168 0368 1b68 ea68 1c4b  .h.h.h.h.h.h.h.K
-00001310: 0175 6275 8c0d 666f 6f74 6e6f 7465 5f72  .ubu..footnote_r
-00001320: 6566 7394 7d94 8c0d 6369 7461 7469 6f6e  efs.}...citation
-00001330: 5f72 6566 7394 7d94 8c0d 6175 746f 666f  _refs.}...autofo
-00001340: 6f74 6e6f 7465 7394 5d94 8c11 6175 746f  otnotes.]...auto
-00001350: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
-00001360: 8c10 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00001370: 6573 945d 948c 1473 796d 626f 6c5f 666f  es.]...symbol_fo
-00001380: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c09  otnote_refs.]...
-00001390: 666f 6f74 6e6f 7465 7394 5d94 8c09 6369  footnotes.]...ci
-000013a0: 7461 7469 6f6e 7394 5d94 8c12 6175 746f  tations.]...auto
-000013b0: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-000013c0: 018c 1573 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
-000013d0: 7465 5f73 7461 7274 944b 008c 0869 645f  te_start.K...id_
-000013e0: 7374 6172 7494 4b01 8c0e 7061 7273 655f  start.K...parse_
-000013f0: 6d65 7373 6167 6573 945d 948c 1274 7261  messages.]...tra
-00001400: 6e73 666f 726d 5f6d 6573 7361 6765 7394  nsform_messages.
-00001410: 5d94 8c0b 7472 616e 7366 6f72 6d65 7294  ]...transformer.
-00001420: 4e8c 0a64 6563 6f72 6174 696f 6e94 4e68  N..decoration.Nh
-00001430: 0168 0375 622e                           .h.ub.
+000002f0: 6170 692f 4368 6961 6e74 6950 792e 6d6f  api/ChiantiPy.mo
+00000300: 6465 6c94 8694 4e8c 1361 7069 2f43 6869  del...N..api/Chi
+00000310: 616e 7469 5079 2e74 6573 7473 9486 944e  antiPy.tests...N
+00000320: 8c13 6170 692f 4368 6961 6e74 6950 792e  ..api/ChiantiPy.
+00000330: 746f 6f6c 7394 8694 658c 0c69 6e63 6c75  tools...e..inclu
+00000340: 6465 6669 6c65 7394 5d94 2868 5068 5268  defiles.].(hPhRh
+00000350: 5468 5668 5868 5a68 5c65 8c08 6d61 7864  ThVhXhZh\e..maxd
+00000360: 6570 7468 944a ffff ffff 8c07 6361 7074  epth.J......capt
+00000370: 696f 6e94 4e8c 0467 6c6f 6294 898c 0668  ion.N..glob....h
+00000380: 6964 6465 6e94 898c 0d69 6e63 6c75 6465  idden....include
+00000390: 6869 6464 656e 9489 8c08 6e75 6d62 6572  hidden....number
+000003a0: 6564 944b 008c 0a74 6974 6c65 736f 6e6c  ed.K...titlesonl
+000003b0: 7994 8975 6829 6842 681b 682a 681c 4b07  y..uh)hBh.h*h.K.
+000003c0: 681a 683e 7562 6168 1d7d 9428 681f 5d94  h.h>ubah.}.(h.].
+000003d0: 6821 5d94 8c0f 746f 6374 7265 652d 7772  h!]...toctree-wr
+000003e0: 6170 7065 7294 6168 235d 9468 255d 9468  apper.ah#].h%].h
+000003f0: 275d 9475 6829 683c 681a 682b 6801 6803  '].uh)h<h.h+h.h.
+00000400: 681b 682a 681c 4b10 7562 6568 1d7d 9428  h.h*h.K.ubeh.}.(
+00000410: 681f 5d94 8c0b 7375 6270 6163 6b61 6765  h.]...subpackage
+00000420: 7394 6168 215d 9468 235d 948c 0b73 7562  s.ah!].h#]...sub
+00000430: 7061 636b 6167 6573 9461 6825 5d94 6827  packages.ah%].h'
+00000440: 5d94 7568 2968 0968 1a68 0b68 0168 0368  ].uh)h.h.h.h.h.h
+00000450: 1b68 2a68 1c4b 0575 6268 0a29 8194 7d94  .h*h.K.ubh.)..}.
+00000460: 2868 0568 0668 075d 9468 0f29 8194 7d94  (h.h.h.].h.)..}.
+00000470: 2868 058c 0a53 7562 6d6f 6475 6c65 7394  (h...Submodules.
+00000480: 6807 5d94 6815 8c0a 5375 626d 6f64 756c  h.].h...Submodul
+00000490: 6573 9485 9481 947d 9428 6805 687b 681a  es.....}.(h.h{h.
+000004a0: 6879 6801 6803 681b 4e68 1c4e 7562 6168  hyh.h.h.Nh.Nubah
+000004b0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+000004c0: 6825 5d94 6827 5d94 7568 2968 0e68 1a68  h%].h'].uh)h.h.h
+000004d0: 7668 0168 0368 1b68 2a68 1c4b 1275 6261  vh.h.h.h*h.K.uba
+000004e0: 681d 7d94 2868 1f5d 948c 0a73 7562 6d6f  h.}.(h.]...submo
+000004f0: 6475 6c65 7394 6168 215d 9468 235d 948c  dules.ah!].h#]..
+00000500: 0a73 7562 6d6f 6475 6c65 7394 6168 255d  .submodules.ah%]
+00000510: 9468 275d 9475 6829 6809 681a 680b 6801  .h'].uh)h.h.h.h.
+00000520: 6803 681b 682a 681c 4b12 7562 680a 2981  h.h.h*h.K.ubh.).
+00000530: 947d 9428 6805 6806 6807 5d94 2868 0f29  .}.(h.h.h.].(h.)
+00000540: 8194 7d94 2868 058c 1943 6869 616e 7469  ..}.(h...Chianti
+00000550: 5079 5c2e 7665 7273 696f 6e20 6d6f 6475  Py\.version modu
+00000560: 6c65 9468 075d 9468 158c 1843 6869 616e  le.h.].h...Chian
+00000570: 7469 5079 2e76 6572 7369 6f6e 206d 6f64  tiPy.version mod
+00000580: 756c 6594 8594 8194 7d94 2868 058c 1943  ule.....}.(h...C
+00000590: 6869 616e 7469 5079 5c2e 7665 7273 696f  hiantiPy\.versio
+000005a0: 6e20 6d6f 6475 6c65 9468 1a68 9268 0168  n module.h.h.h.h
+000005b0: 0368 1b4e 681c 4e75 6261 681d 7d94 2868  .h.Nh.Nubah.}.(h
+000005c0: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+000005d0: 275d 9475 6829 680e 681a 688f 6801 6803  '].uh)h.h.h.h.h.
+000005e0: 681b 682a 681c 4b16 7562 6841 8c05 696e  h.h*h.K.ubhA..in
+000005f0: 6465 7894 9394 2981 947d 9428 6805 6806  dex...)..}.(h.h.
+00000600: 6807 5d94 681d 7d94 2868 1f5d 9468 215d  h.].h.}.(h.].h!]
+00000610: 9468 235d 9468 255d 9468 275d 948c 0765  .h#].h%].h']...e
+00000620: 6e74 7269 6573 945d 9428 8c06 7369 6e67  ntries.].(..sing
+00000630: 6c65 948c 1a43 6869 616e 7469 5079 2e76  le...ChiantiPy.v
+00000640: 6572 7369 6f6e 2028 6d6f 6475 6c65 2994  ersion (module).
+00000650: 8c18 6d6f 6475 6c65 2d43 6869 616e 7469  ..module-Chianti
+00000660: 5079 2e76 6572 7369 6f6e 9468 064e 7494  Py.version.h.Nt.
+00000670: 6175 6829 68a1 681a 688f 6801 6803 681b  auh)h.h.h.h.h.h.
+00000680: 8c47 2f64 6174 6132 2f67 682f 4368 6961  .G/data2/gh/Chia
+00000690: 6e74 6950 792f 4368 6961 6e74 6950 792f  ntiPy/ChiantiPy/
+000006a0: 7665 7273 696f 6e2e 7079 3a64 6f63 7374  version.py:docst
+000006b0: 7269 6e67 206f 6620 4368 6961 6e74 6950  ring of ChiantiP
+000006c0: 792e 7665 7273 696f 6e94 681c 4b01 7562  y.version.h.K.ub
+000006d0: 6800 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
+000006e0: 2981 947d 9428 6805 8c2c 7468 6520 6375  )..}.(h..,the cu
+000006f0: 7272 656e 7420 7665 7273 696f 6e20 6f66  rrent version of
+00000700: 2074 6865 2043 6869 616e 7469 5079 2070   the ChiantiPy p
+00000710: 6163 6b61 6765 9468 075d 9468 158c 2c74  ackage.h.].h..,t
+00000720: 6865 2063 7572 7265 6e74 2076 6572 7369  he current versi
+00000730: 6f6e 206f 6620 7468 6520 4368 6961 6e74  on of the Chiant
+00000740: 6950 7920 7061 636b 6167 6594 8594 8194  iPy package.....
+00000750: 7d94 2868 0568 b768 1a68 b568 0168 0368  }.(h.h.h.h.h.h.h
+00000760: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+00000770: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00000780: 9475 6829 68b3 681b 8c47 2f64 6174 6132  .uh)h.h..G/data2
+00000790: 2f67 682f 4368 6961 6e74 6950 792f 4368  /gh/ChiantiPy/Ch
+000007a0: 6961 6e74 6950 792f 7665 7273 696f 6e2e  iantiPy/version.
+000007b0: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
+000007c0: 4368 6961 6e74 6950 792e 7665 7273 696f  ChiantiPy.versio
+000007d0: 6e94 681c 4b01 681a 688f 6801 6803 7562  n.h.K.h.h.h.h.ub
+000007e0: 6568 1d7d 9428 681f 5d94 288c 186d 6f64  eh.}.(h.].(..mod
+000007f0: 756c 652d 4368 6961 6e74 6950 792e 7665  ule-ChiantiPy.ve
+00000800: 7273 696f 6e94 8c18 6368 6961 6e74 6970  rsion...chiantip
+00000810: 792d 7665 7273 696f 6e2d 6d6f 6475 6c65  y-version-module
+00000820: 9465 6821 5d94 6823 5d94 8c18 6368 6961  .eh!].h#]...chia
+00000830: 6e74 6970 792e 7665 7273 696f 6e20 6d6f  ntipy.version mo
+00000840: 6475 6c65 9461 6825 5d94 6827 5d94 7568  dule.ah%].h'].uh
+00000850: 2968 0968 1a68 0b68 0168 0368 1b68 2a68  )h.h.h.h.h.h.h*h
+00000860: 1c4b 1675 6268 0a29 8194 7d94 2868 0568  .K.ubh.)..}.(h.h
+00000870: 0668 075d 9428 680f 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000880: 8c0f 4d6f 6475 6c65 2063 6f6e 7465 6e74  ..Module content
+00000890: 7394 6807 5d94 6815 8c0f 4d6f 6475 6c65  s.h.].h...Module
+000008a0: 2063 6f6e 7465 6e74 7394 8594 8194 7d94   contents.....}.
+000008b0: 2868 0568 d268 1a68 d068 0168 0368 1b4e  (h.h.h.h.h.h.h.N
+000008c0: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+000008d0: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+000008e0: 6829 680e 681a 68cd 6801 6803 681b 682a  h)h.h.h.h.h.h.h*
+000008f0: 681c 4b1f 7562 68a2 2981 947d 9428 6805  h.K.ubh.)..}.(h.
+00000900: 6806 6807 5d94 681d 7d94 2868 1f5d 9468  h.h.].h.}.(h.].h
+00000910: 215d 9468 235d 9468 255d 9468 275d 948c  !].h#].h%].h']..
+00000920: 0765 6e74 7269 6573 945d 9428 68ae 8c12  .entries.].(h...
+00000930: 4368 6961 6e74 6950 7920 286d 6f64 756c  ChiantiPy (modul
+00000940: 6529 948c 106d 6f64 756c 652d 4368 6961  e)...module-Chia
+00000950: 6e74 6950 7994 6806 4e74 9461 7568 2968  ntiPy.h.Nt.auh)h
+00000960: a168 1a68 cd68 0168 0368 1b8c 402f 6461  .h.h.h.h.h..@/da
+00000970: 7461 322f 6768 2f43 6869 616e 7469 5079  ta2/gh/ChiantiPy
+00000980: 2f43 6869 616e 7469 5079 2f5f 5f69 6e69  /ChiantiPy/__ini
+00000990: 745f 5f2e 7079 3a64 6f63 7374 7269 6e67  t__.py:docstring
+000009a0: 206f 6620 4368 6961 6e74 6950 7994 681c   of ChiantiPy.h.
+000009b0: 4b01 7562 68b4 2981 947d 9428 6805 8c9d  K.ubh.)..}.(h...
+000009c0: 4368 6961 6e74 6950 7920 2d20 4348 4941  ChiantiPy - CHIA
+000009d0: 4e54 4920 5079 7468 6f6e 2070 6163 6b61  NTI Python packa
+000009e0: 6765 2043 616c 6375 6c61 7465 7320 7661  ge Calculates va
+000009f0: 7269 6f75 7320 6173 7065 6374 7320 6f66  rious aspects of
+00000a00: 2065 6d69 7373 696f 6e20 6c69 6e65 730a   emission lines.
+00000a10: 616e 6420 636f 6e74 696e 7561 2066 726f  and continua fro
+00000a20: 6d20 7468 6520 4348 4941 4e54 4920 6174  m the CHIANTI at
+00000a30: 6f6d 6963 2064 6174 6162 6173 6520 666f  omic database fo
+00000a40: 7220 6173 7472 6f70 6879 7369 6361 6c20  r astrophysical 
+00000a50: 7370 6563 7472 6f73 636f 7079 2e94 6807  spectroscopy..h.
+00000a60: 5d94 6815 8c9d 4368 6961 6e74 6950 7920  ].h...ChiantiPy 
+00000a70: 2d20 4348 4941 4e54 4920 5079 7468 6f6e  - CHIANTI Python
+00000a80: 2070 6163 6b61 6765 2043 616c 6375 6c61   package Calcula
+00000a90: 7465 7320 7661 7269 6f75 7320 6173 7065  tes various aspe
+00000aa0: 6374 7320 6f66 2065 6d69 7373 696f 6e20  cts of emission 
+00000ab0: 6c69 6e65 730a 616e 6420 636f 6e74 696e  lines.and contin
+00000ac0: 7561 2066 726f 6d20 7468 6520 4348 4941  ua from the CHIA
+00000ad0: 4e54 4920 6174 6f6d 6963 2064 6174 6162  NTI atomic datab
+00000ae0: 6173 6520 666f 7220 6173 7472 6f70 6879  ase for astrophy
+00000af0: 7369 6361 6c20 7370 6563 7472 6f73 636f  sical spectrosco
+00000b00: 7079 2e94 8594 8194 7d94 2868 0568 ef68  py......}.(h.h.h
+00000b10: 1a68 ed68 0168 0368 1b4e 681c 4e75 6261  .h.h.h.h.Nh.Nuba
+00000b20: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00000b30: 9468 255d 9468 275d 9475 6829 68b3 681b  .h%].h'].uh)h.h.
+00000b40: 8c40 2f64 6174 6132 2f67 682f 4368 6961  .@/data2/gh/Chia
+00000b50: 6e74 6950 792f 4368 6961 6e74 6950 792f  ntiPy/ChiantiPy/
+00000b60: 5f5f 696e 6974 5f5f 2e70 793a 646f 6373  __init__.py:docs
+00000b70: 7472 696e 6720 6f66 2043 6869 616e 7469  tring of Chianti
+00000b80: 5079 9468 1c4b 0168 1a68 cd68 0168 0375  Py.h.K.h.h.h.h.u
+00000b90: 6265 681d 7d94 2868 1f5d 9428 8c10 6d6f  beh.}.(h.].(..mo
+00000ba0: 6475 6c65 2d43 6869 616e 7469 5079 948c  dule-ChiantiPy..
+00000bb0: 0f6d 6f64 756c 652d 636f 6e74 656e 7473  .module-contents
+00000bc0: 9465 6821 5d94 6823 5d94 8c0f 6d6f 6475  .eh!].h#]...modu
+00000bd0: 6c65 2063 6f6e 7465 6e74 7394 6168 255d  le contents.ah%]
+00000be0: 9468 275d 9475 6829 6809 681a 680b 6801  .h'].uh)h.h.h.h.
+00000bf0: 6803 681b 682a 681c 4b1f 7562 6568 1d7d  h.h.h*h.K.ubeh.}
+00000c00: 9428 681f 5d94 8c11 6368 6961 6e74 6970  .(h.]...chiantip
+00000c10: 792d 7061 636b 6167 6594 6168 215d 9468  y-package.ah!].h
+00000c20: 235d 948c 1163 6869 616e 7469 7079 2070  #]...chiantipy p
+00000c30: 6163 6b61 6765 9461 6825 5d94 6827 5d94  ackage.ah%].h'].
+00000c40: 7568 2968 0968 1a68 0368 0168 0368 1b68  uh)h.h.h.h.h.h.h
+00000c50: 2a68 1c4b 0275 6261 681d 7d94 2868 1f5d  *h.K.ubah.}.(h.]
+00000c60: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00000c70: 948c 0673 6f75 7263 6594 682a 7568 2968  ...source.h*uh)h
+00000c80: 018c 0e63 7572 7265 6e74 5f73 6f75 7263  ...current_sourc
+00000c90: 6594 4e8c 0c63 7572 7265 6e74 5f6c 696e  e.N..current_lin
+00000ca0: 6594 4e8c 0873 6574 7469 6e67 7394 8c11  e.N..settings...
+00000cb0: 646f 6375 7469 6c73 2e66 726f 6e74 656e  docutils.fronten
+00000cc0: 6494 8c06 5661 6c75 6573 9493 9429 8194  d...Values...)..
+00000cd0: 7d94 2868 0e4e 8c09 6765 6e65 7261 746f  }.(h.N..generato
+00000ce0: 7294 4e8c 0964 6174 6573 7461 6d70 944e  r.N..datestamp.N
+00000cf0: 8c0b 736f 7572 6365 5f6c 696e 6b94 4e8c  ..source_link.N.
+00000d00: 0a73 6f75 7263 655f 7572 6c94 4e8c 0d74  .source_url.N..t
+00000d10: 6f63 5f62 6163 6b6c 696e 6b73 948c 0565  oc_backlinks...e
+00000d20: 6e74 7279 948c 1266 6f6f 746e 6f74 655f  ntry...footnote_
+00000d30: 6261 636b 6c69 6e6b 7394 4b01 8c0d 7365  backlinks.K...se
+00000d40: 6374 6e75 6d5f 7866 6f72 6d94 4b01 8c0e  ctnum_xform.K...
+00000d50: 7374 7269 705f 636f 6d6d 656e 7473 944e  strip_comments.N
+00000d60: 8c1b 7374 7269 705f 656c 656d 656e 7473  ..strip_elements
+00000d70: 5f77 6974 685f 636c 6173 7365 7394 4e8c  _with_classes.N.
+00000d80: 0d73 7472 6970 5f63 6c61 7373 6573 944e  .strip_classes.N
+00000d90: 8c0c 7265 706f 7274 5f6c 6576 656c 944b  ..report_level.K
+00000da0: 028c 0a68 616c 745f 6c65 7665 6c94 4b05  ...halt_level.K.
+00000db0: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
+00000dc0: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
+00000dd0: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
+00000de0: 4e8c 0974 7261 6365 6261 636b 9488 8c0e  N..traceback....
+00000df0: 696e 7075 745f 656e 636f 6469 6e67 948c  input_encoding..
+00000e00: 0975 7466 2d38 2d73 6967 948c 1c69 6e70  .utf-8-sig...inp
+00000e10: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+00000e20: 725f 6861 6e64 6c65 7294 8c06 7374 7269  r_handler...stri
+00000e30: 6374 948c 0f6f 7574 7075 745f 656e 636f  ct...output_enco
+00000e40: 6469 6e67 948c 0575 7466 2d38 948c 1d6f  ding...utf-8...o
+00000e50: 7574 7075 745f 656e 636f 6469 6e67 5f65  utput_encoding_e
+00000e60: 7272 6f72 5f68 616e 646c 6572 946a 3001  rror_handler.j0.
+00000e70: 0000 8c0e 6572 726f 725f 656e 636f 6469  ....error_encodi
+00000e80: 6e67 948c 0555 5446 2d38 948c 1c65 7272  ng...UTF-8...err
+00000e90: 6f72 5f65 6e63 6f64 696e 675f 6572 726f  or_encoding_erro
+00000ea0: 725f 6861 6e64 6c65 7294 8c10 6261 636b  r_handler...back
+00000eb0: 736c 6173 6872 6570 6c61 6365 948c 0d6c  slashreplace...l
+00000ec0: 616e 6775 6167 655f 636f 6465 948c 0265  anguage_code...e
+00000ed0: 6e94 8c13 7265 636f 7264 5f64 6570 656e  n...record_depen
+00000ee0: 6465 6e63 6965 7394 4e8c 0663 6f6e 6669  dencies.N..confi
+00000ef0: 6794 4e8c 0969 645f 7072 6566 6978 9468  g.N..id_prefix.h
+00000f00: 068c 0e61 7574 6f5f 6964 5f70 7265 6669  ...auto_id_prefi
+00000f10: 7894 8c02 6964 948c 0d64 756d 705f 7365  x...id...dump_se
+00000f20: 7474 696e 6773 944e 8c0e 6475 6d70 5f69  ttings.N..dump_i
+00000f30: 6e74 6572 6e61 6c73 944e 8c0f 6475 6d70  nternals.N..dump
+00000f40: 5f74 7261 6e73 666f 726d 7394 4e8c 0f64  _transforms.N..d
+00000f50: 756d 705f 7073 6575 646f 5f78 6d6c 944e  ump_pseudo_xml.N
+00000f60: 8c10 6578 706f 7365 5f69 6e74 6572 6e61  ..expose_interna
+00000f70: 6c73 944e 8c0e 7374 7269 6374 5f76 6973  ls.N..strict_vis
+00000f80: 6974 6f72 944e 8c0f 5f64 6973 6162 6c65  itor.N.._disable
+00000f90: 5f63 6f6e 6669 6794 4e8c 075f 736f 7572  _config.N.._sour
+00000fa0: 6365 9468 2a8c 0c5f 6465 7374 696e 6174  ce.h*.._destinat
+00000fb0: 696f 6e94 4e8c 0d5f 636f 6e66 6967 5f66  ion.N.._config_f
+00000fc0: 696c 6573 945d 948c 0e70 6570 5f72 6566  iles.]...pep_ref
+00000fd0: 6572 656e 6365 7394 4e8c 0c70 6570 5f62  erences.N..pep_b
+00000fe0: 6173 655f 7572 6c94 8c20 6874 7470 733a  ase_url.. https:
+00000ff0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00001000: 2f64 6576 2f70 6570 732f 948c 1570 6570  /dev/peps/...pep
+00001010: 5f66 696c 655f 7572 6c5f 7465 6d70 6c61  _file_url_templa
+00001020: 7465 948c 0870 6570 2d25 3034 6494 8c0e  te...pep-%04d...
+00001030: 7266 635f 7265 6665 7265 6e63 6573 944e  rfc_references.N
+00001040: 8c0c 7266 635f 6261 7365 5f75 726c 948c  ..rfc_base_url..
+00001050: 1c68 7474 7073 3a2f 2f74 6f6f 6c73 2e69  .https://tools.i
+00001060: 6574 662e 6f72 672f 6874 6d6c 2f94 8c09  etf.org/html/...
+00001070: 7461 625f 7769 6474 6894 4b08 8c1d 7472  tab_width.K...tr
+00001080: 696d 5f66 6f6f 746e 6f74 655f 7265 6665  im_footnote_refe
+00001090: 7265 6e63 655f 7370 6163 6594 898c 1666  rence_space....f
+000010a0: 696c 655f 696e 7365 7274 696f 6e5f 656e  ile_insertion_en
+000010b0: 6162 6c65 6494 888c 0b72 6177 5f65 6e61  abled....raw_ena
+000010c0: 626c 6564 944b 018c 1073 796e 7461 785f  bled.K...syntax_
+000010d0: 6869 6768 6c69 6768 7494 8c04 6c6f 6e67  highlight...long
+000010e0: 948c 0c73 6d61 7274 5f71 756f 7465 7394  ...smart_quotes.
+000010f0: 888c 1373 6d61 7274 7175 6f74 6573 5f6c  ...smartquotes_l
+00001100: 6f63 616c 6573 944e 8c1d 6368 6172 6163  ocales.N..charac
+00001110: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
+00001120: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
+00001130: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
+00001140: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
+00001150: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
+00001160: 6d94 898c 1065 6d62 6564 5f73 7479 6c65  m....embed_style
+00001170: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
+00001180: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
+00001190: 8c03 656e 7694 4e8c 0f67 6574 7465 7874  ..env.N..gettext
+000011a0: 5f63 6f6d 7061 6374 9488 7562 8c08 7265  _compact..ub..re
+000011b0: 706f 7274 6572 944e 8c10 696e 6469 7265  porter.N..indire
+000011c0: 6374 5f74 6172 6765 7473 945d 948c 1173  ct_targets.]...s
+000011d0: 7562 7374 6974 7574 696f 6e5f 6465 6673  ubstitution_defs
+000011e0: 947d 948c 1273 7562 7374 6974 7574 696f  .}...substitutio
+000011f0: 6e5f 6e61 6d65 7394 7d94 8c08 7265 666e  n_names.}...refn
+00001200: 616d 6573 947d 948c 0672 6566 6964 7394  ames.}...refids.
+00001210: 7d94 8c07 6e61 6d65 6964 7394 7d94 286a  }...nameids.}.(j
+00001220: 0a01 0000 6a07 0100 0068 7368 7068 8c68  ....j....hshph.h
+00001230: 8968 ca68 c76a 0201 0000 68ff 758c 096e  .h.h.j....h.u..n
+00001240: 616d 6574 7970 6573 947d 9428 6a0a 0100  ametypes.}.(j...
+00001250: 004e 6873 4e68 8c4e 68ca 4e6a 0201 0000  .NhsNh.Nh.Nj....
+00001260: 4e75 681f 7d94 286a 0701 0000 680b 6870  Nuh.}.(j....h.hp
+00001270: 682b 6889 6876 68c7 688f 68c6 6800 8c06  h+h.hvh.h.h.h...
+00001280: 7461 7267 6574 9493 9429 8194 7d94 2868  target...)..}.(h
+00001290: 0568 0668 075d 9468 1d7d 9428 681f 5d94  .h.h.].h.}.(h.].
+000012a0: 68c6 6168 215d 9468 235d 9468 255d 9468  h.ah!].h#].h%].h
+000012b0: 275d 948c 0569 736d 6f64 9488 7568 296a  ']...ismod..uh)j
+000012c0: 7201 0000 681a 688f 6801 6803 681b 68b2  r...h.h.h.h.h.h.
+000012d0: 681c 4b01 7562 68ff 68cd 68fe 6a73 0100  h.K.ubh.h.h.js..
+000012e0: 0029 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
+000012f0: 1d7d 9428 681f 5d94 68fe 6168 215d 9468  .}.(h.].h.ah!].h
+00001300: 235d 9468 255d 9468 275d 948c 0569 736d  #].h%].h']...ism
+00001310: 6f64 9488 7568 296a 7201 0000 681a 68cd  od..uh)jr...h.h.
+00001320: 6801 6803 681b 68ec 681c 4b01 7562 758c  h.h.h.h.h.K.ubu.
+00001330: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
+00001340: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
+00001350: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
+00001360: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
+00001370: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
+00001380: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
+00001390: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
+000013a0: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
+000013b0: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
+000013c0: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
+000013d0: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
+000013e0: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
+000013f0: 6172 7494 4b00 8c08 6964 5f73 7461 7274  art.K...id_start
+00001400: 944b 018c 0e70 6172 7365 5f6d 6573 7361  .K...parse_messa
+00001410: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
+00001420: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
+00001430: 7261 6e73 666f 726d 6572 944e 8c0a 6465  ransformer.N..de
+00001440: 636f 7261 7469 6f6e 944e 6801 6803 7562  coration.Nh.h.ub
+00001450: 2e                                       .
```

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.fortranformat.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.fortranformat.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.tests.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.tests.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/ChiantiPy.tools.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.tools.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/index.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/index.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/api/modules.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/bugs.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/bugs.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/changelog.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/getting_started.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/getting_started.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/index.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/notes.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/notes.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/quick_start.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/quick_start.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/resources.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/resources.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/.doctrees/tutorial.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/IDL_intro.html` & `ChiantiPy-0.9.5/docs/build/html/IDL_intro.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/2.selector.png` & `ChiantiPy-0.9.5/docs/build/_images/2.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/bunch_selector.png` & `ChiantiPy-0.9.5/docs/build/_images/bunch_selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/continuum_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/_images/continuum_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt.selector.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.gofnt_alternate.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.gofnt_alternate.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.int.ratio.vs.d.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.int.ratio.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.int.ratio.vs.t.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.int.ratio.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.int.vs.d.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.int.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.int.vs.t.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.int.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.popplot.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.popplot.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.rel.emiss.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.rel.emiss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum2.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14.spectrum_label.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14.spectrum_label.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14_intensity_plot_log.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14_intensity_plot_log.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe14_intensity_plot_log_index2.png` & `ChiantiPy-0.9.5/docs/build/_images/fe14_intensity_plot_log_index2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe_12_wvlranges_ratio.png` & `ChiantiPy-0.9.5/docs/build/_images/fe_12_wvlranges_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe_13_14_15_ioneq.png` & `ChiantiPy-0.9.5/docs/build/_images/fe_13_14_15_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe_25_ff_fb_tp_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/_images/fe_25_ff_fb_tp_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/fe_ioneq.png` & `ChiantiPy-0.9.5/docs/build/_images/fe_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_spectrum.png` & `ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_t_ratio.png` & `ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_t_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/ne6_mg6_t_ratio_top7.png` & `ChiantiPy-0.9.5/docs/build/_images/ne6_mg6_t_ratio_top7.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/radloss.png` & `ChiantiPy-0.9.5/docs/build/_images/radloss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_10_20.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_10_20.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_1_10.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_3panel.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_3panel.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_integrated.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_integrated.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_200_300_w_si_9.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_200_300_w_si_9.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_images/spectrum_2e7_1.84_1.90.png` & `ChiantiPy-0.9.5/docs/build/_images/spectrum_2e7_1.84_1.90.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/IDL_intro.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/IDL_intro.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.base.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.base.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.core.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.core.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.core.tests.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.core.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.fortranformat.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.fortranformat.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/api/ChiantiPy.tools.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/api/ChiantiPy.tools.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/changelog.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/changelog.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/getting_started.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/getting_started.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/index.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/notes.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/notes.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/quick_start.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/quick_start.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_sources/tutorial.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/2.selector.png` & `ChiantiPy-0.9.5/docs/build/_static/2.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/ajax-loader.gif` & `ChiantiPy-0.9.5/docs/build/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/basic.css` & `ChiantiPy-0.9.5/docs/build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/bunch_selector.png` & `ChiantiPy-0.9.5/docs/build/_static/bunch_selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/chiantipy_logo.png` & `ChiantiPy-0.9.5/docs/build/_static/chiantipy_logo.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/comment-bright.png` & `ChiantiPy-0.9.5/docs/build/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/comment-close.png` & `ChiantiPy-0.9.5/docs/build/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/comment.png` & `ChiantiPy-0.9.5/docs/build/_static/comment.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/continuum_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/_static/continuum_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/doctools.js` & `ChiantiPy-0.9.5/docs/build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt.selector.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.gofnt_alternate.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.gofnt_alternate.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.int.ratio.vs.d.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.int.ratio.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.int.ratio.vs.t.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.int.ratio.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.int.vs.d.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.int.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.int.vs.t.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.int.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.popplot.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.popplot.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.rel.emiss.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.rel.emiss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum2.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14.spectrum_label.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14.spectrum_label.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14_intensity_plot_log.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14_intensity_plot_log.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe14_intensity_plot_log_index2.png` & `ChiantiPy-0.9.5/docs/build/_static/fe14_intensity_plot_log_index2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe_12_wvlranges_ratio.png` & `ChiantiPy-0.9.5/docs/build/_static/fe_12_wvlranges_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe_13_14_15_ioneq.png` & `ChiantiPy-0.9.5/docs/build/_static/fe_13_14_15_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe_25_ff_fb_tp_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/_static/fe_25_ff_fb_tp_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/fe_ioneq.png` & `ChiantiPy-0.9.5/docs/build/_static/fe_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/jquery-3.1.0.js` & `ChiantiPy-0.9.5/docs/build/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/jquery-3.2.1.js` & `ChiantiPy-0.9.5/docs/build/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/jquery.js` & `ChiantiPy-0.9.5/docs/build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_spectrum.png` & `ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_t_ratio.png` & `ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_t_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/ne6_mg6_t_ratio_top7.png` & `ChiantiPy-0.9.5/docs/build/_static/ne6_mg6_t_ratio_top7.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/pygments.css` & `ChiantiPy-0.9.5/docs/build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/radloss.png` & `ChiantiPy-0.9.5/docs/build/_static/radloss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/searchtools.js` & `ChiantiPy-0.9.5/docs/build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_10_20.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_10_20.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_1_10.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_3panel.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_3panel.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_integrated.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_integrated.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_200_300_w_si_9.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_200_300_w_si_9.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/spectrum_2e7_1.84_1.90.png` & `ChiantiPy-0.9.5/docs/build/_static/spectrum_2e7_1.84_1.90.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/sphinxdoc.css` & `ChiantiPy-0.9.5/docs/build/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/theme.conf` & `ChiantiPy-0.9.5/docs/build/_static/theme.conf`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/underscore-1.3.1.js` & `ChiantiPy-0.9.5/docs/build/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/underscore.js` & `ChiantiPy-0.9.5/docs/build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/_static/websupport.js` & `ChiantiPy-0.9.5/docs/build/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.gui_cl.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.gui_cl.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.gui_qt5.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.gui_qt5.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.Gui.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.Gui.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.base.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.base.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.core.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.core.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.core.tests.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.core.tests.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.fortranformat.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.fortranformat.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.html" title="ChiantiPy.Gui package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="ChiantiPy’s API documentation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">ChiantiPy’s API documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="index.html"
@@ -134,14 +134,20 @@
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.fortranformat.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordReader">ChiantiPy.fortranformat.FortranRecordReader module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordWriter">ChiantiPy.fortranformat.FortranRecordWriter module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.config">ChiantiPy.fortranformat.config module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat">Module contents</a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="ChiantiPy.model.html">ChiantiPy.Gui package</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="ChiantiPy.model.html#submodules">Submodules</a></li>
+<li class="toctree-l2"><a class="reference internal" href="ChiantiPy.model.html#module-ChiantiPy.model.Maker">ChiantiPy.model.Maker module</a></li>
+<li class="toctree-l2"><a class="reference internal" href="ChiantiPy.model.html#module-ChiantiPy.model">Module contents</a></li>
+</ul>
+</li>
 <li class="toctree-l1"><a class="reference internal" href="ChiantiPy.tests.html">ChiantiPy.tests package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.tests.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests.setup_package">ChiantiPy.tests.setup_package module</a></li>
 <li class="toctree-l2"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="ChiantiPy.tools.html">ChiantiPy.tools package</a><ul>
@@ -191,23 +197,23 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.html" title="ChiantiPy.Gui package"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="ChiantiPy’s API documentation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
 *** Previous topic ***
 ChiantiPyâs_API_documentation
 *** Next topic ***
 ChiantiPy.Gui_package
 **** Quick search ****
 [q                   ] [Go]
@@ -58,14 +58,18 @@
           o Module_contents
     * ChiantiPy.fortranformat_package
           o Submodules
           o ChiantiPy.fortranformat.FortranRecordReader_module
           o ChiantiPy.fortranformat.FortranRecordWriter_module
           o ChiantiPy.fortranformat.config_module
           o Module_contents
+    * ChiantiPy.Gui_package
+          o Submodules
+          o ChiantiPy.model.Maker_module
+          o Module_contents
     * ChiantiPy.tests_package
           o Submodules
           o ChiantiPy.tests.setup_package_module
           o Module_contents
     * ChiantiPy.tools_package
           o Submodules
           o ChiantiPy.tools.archival_module
@@ -84,10 +88,10 @@
 ChiantiPy - CHIANTI Python package Calculates various aspects of emission lines
 and continua from the CHIANTI atomic database for astrophysical spectroscopy.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.tests.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.tests.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/ChiantiPy.tools.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.tools.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/api/index.html` & `ChiantiPy-0.9.5/docs/build/html/api/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,19 @@
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#submodules">Submodules</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordReader">ChiantiPy.fortranformat.FortranRecordReader module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordWriter">ChiantiPy.fortranformat.FortranRecordWriter module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.config">ChiantiPy.fortranformat.config module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat">Module contents</a></li>
 </ul>
 </li>
+<li class="toctree-l3"><a class="reference internal" href="ChiantiPy.model.html">ChiantiPy.Gui package</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#subpackages">Subpackages</a></li>
+<li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#module-ChiantiPy.model">Module contents</a></li>
+</ul>
+</li>
 <li class="toctree-l3"><a class="reference internal" href="ChiantiPy.tests.html">ChiantiPy.tests package</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#submodules">Submodules</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests.setup_package">ChiantiPy.tests.setup_package module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="ChiantiPy.tools.html">ChiantiPy.tools package</a><ul>
```

#### html2text {}

```diff
@@ -43,14 +43,17 @@
                       # Module_contents
                 # ChiantiPy.fortranformat_package
                       # Submodules
                       # ChiantiPy.fortranformat.FortranRecordReader_module
                       # ChiantiPy.fortranformat.FortranRecordWriter_module
                       # ChiantiPy.fortranformat.config_module
                       # Module_contents
+                # ChiantiPy.Gui_package
+                      # Subpackages
+                      # Module_contents
                 # ChiantiPy.tests_package
                       # Submodules
                       # ChiantiPy.tests.setup_package_module
                       # Module_contents
                 # ChiantiPy.tools_package
                       # Submodules
                       # ChiantiPy.tools.archival_module
```

### Comparing `ChiantiPy-0.9.4/docs/build/api/modules.html` & `ChiantiPy-0.9.5/docs/build/api/modules.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/bugs.html` & `ChiantiPy-0.9.5/docs/build/html/bugs.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/changelog.html` & `ChiantiPy-0.9.5/docs/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/IDL_intro.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/IDL_intro.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.gui_cl.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.gui_cl.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.Gui.gui_qt5.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.Gui.gui_qt5.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.base.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.base.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.core.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.core.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.core.tests.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.core.tests.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.fortranformat.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.fortranformat.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.model.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/api/ChiantiPy.model.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.tests.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.tests.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/ChiantiPy.tools.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/ChiantiPy.tools.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/index.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/index.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/api/modules.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/api/modules.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/bugs.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/bugs.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/changelog.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/changelog.doctree`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 957d 7b00 0000 0000 008c 0e64 6f63  ...}{........doc
+00000000: 8004 9572 8f00 0000 0000 008c 0e64 6f63  ...r.........doc
 00000010: 7574 696c 732e 6e6f 6465 7394 8c08 646f  utils.nodes...do
 00000020: 6375 6d65 6e74 9493 9429 8194 7d94 288c  cument...)..}.(.
 00000030: 0972 6177 736f 7572 6365 948c 0094 8c08  .rawsource......
 00000040: 6368 696c 6472 656e 945d 9468 008c 0773  children.].h...s
 00000050: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000060: 0568 0668 075d 9428 6800 8c05 7469 746c  .h.h.].(h...titl
 00000070: 6594 9394 2981 947d 9428 6805 8c09 4368  e...)..}.(h...Ch
@@ -19,1959 +19,2278 @@
 00000120: 6e61 6d65 9468 0e68 1a68 0b68 0168 0368  name.h.h.h.h.h.h
 00000130: 1b8c 2d2f 6461 7461 322f 6768 2f43 6869  ..-/data2/gh/Chi
 00000140: 616e 7469 5079 2f64 6f63 732f 736f 7572  antiPy/docs/sour
 00000150: 6365 2f63 6861 6e67 656c 6f67 2e72 7374  ce/changelog.rst
 00000160: 9468 1c4b 0375 6268 0a29 8194 7d94 2868  .h.K.ubh.)..}.(h
 00000170: 0568 0668 075d 9428 680f 2981 947d 9428  .h.h.].(h.)..}.(
 00000180: 6805 8c1b 4368 616e 6765 7320 6672 6f6d  h...Changes from
-00000190: 2030 2e38 2e37 2074 6f20 302e 392e 3094   0.8.7 to 0.9.0.
+00000190: 2030 2e39 2e34 2074 6f20 302e 392e 3594   0.9.4 to 0.9.5.
 000001a0: 6807 5d94 6815 8c1b 4368 616e 6765 7320  h.].h...Changes 
-000001b0: 6672 6f6d 2030 2e38 2e37 2074 6f20 302e  from 0.8.7 to 0.
-000001c0: 392e 3094 8594 8194 7d94 2868 0568 3068  9.0.....}.(h.h0h
+000001b0: 6672 6f6d 2030 2e39 2e34 2074 6f20 302e  from 0.9.4 to 0.
+000001c0: 392e 3594 8594 8194 7d94 2868 0568 3068  9.5.....}.(h.h0h
 000001d0: 1a68 2e68 0168 0368 1b4e 681c 4e75 6261  .h.h.h.h.Nh.Nuba
 000001e0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
 000001f0: 9468 255d 9468 275d 9475 6829 680e 681a  .h%].h'].uh)h.h.
-00000200: 682b 6801 6803 681b 682a 681c 4b06 7562  h+h.h.h.h*h.K.ub
+00000200: 682b 6801 6803 681b 682a 681c 4b07 7562  h+h.h.h.h*h.K.ub
 00000210: 6800 8c09 7061 7261 6772 6170 6894 9394  h...paragraph...
-00000220: 2981 947d 9428 6805 8c27 6120 6e65 7720  )..}.(h..'a new 
-00000230: 6d6f 6475 6c65 206d 6f64 656c 2e6d 616b  module model.mak
-00000240: 6572 2068 6173 2062 6565 6e20 6164 6465  er has been adde
-00000250: 6494 6807 5d94 6815 8c27 6120 6e65 7720  d.h.].h..'a new 
-00000260: 6d6f 6475 6c65 206d 6f64 656c 2e6d 616b  module model.mak
-00000270: 6572 2068 6173 2062 6565 6e20 6164 6465  er has been adde
-00000280: 6494 8594 8194 7d94 2868 0568 4068 1a68  d.....}.(h.h@h.h
-00000290: 3e68 0168 0368 1b4e 681c 4e75 6261 681d  >h.h.h.Nh.Nubah.
-000002a0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-000002b0: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
-000002c0: 681c 4b08 681a 682b 6801 6803 7562 6800  h.K.h.h+h.h.ubh.
-000002d0: 8c0d 6c69 7465 7261 6c5f 626c 6f63 6b94  ..literal_block.
-000002e0: 9394 2981 947d 9428 6805 8c36 696d 706f  ..)..}.(h..6impo
-000002f0: 7274 2043 6869 616e 7469 5079 2e6d 6f64  rt ChiantiPy.mod
-00000300: 656c 2061 7320 6d64 6c0a 6d79 6d6f 6465  el as mdl.mymode
-00000310: 6c20 3d20 6d64 6c2e 6d61 6b65 7228 2e2e  l = mdl.maker(..
-00000320: 2e29 9468 075d 9468 158c 3669 6d70 6f72  .).h.].h..6impor
-00000330: 7420 4368 6961 6e74 6950 792e 6d6f 6465  t ChiantiPy.mode
-00000340: 6c20 6173 206d 646c 0a6d 796d 6f64 656c  l as mdl.mymodel
-00000350: 203d 206d 646c 2e6d 616b 6572 282e 2e2e   = mdl.maker(...
-00000360: 2994 8594 8194 7d94 2868 0568 0668 1a68  ).....}.(h.h.h.h
-00000370: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
-00000380: 9468 235d 9468 255d 9468 275d 948c 0978  .h#].h%].h']...x
-00000390: 6d6c 3a73 7061 6365 948c 0870 7265 7365  ml:space...prese
-000003a0: 7276 6594 7568 2968 4c68 1c4b 0c68 1a68  rve.uh)hLh.K.h.h
-000003b0: 2b68 0168 0368 1b68 2a75 6268 3d29 8194  +h.h.h.h*ubh=)..
-000003c0: 7d94 2868 058c 5961 2073 6572 696f 7573  }.(h..Ya serious
-000003d0: 2062 7567 2069 6e20 6368 2e66 7265 6542   bug in ch.freeB
-000003e0: 6f75 6e64 2077 6173 2066 6978 6564 202d  ound was fixed -
-000003f0: 2074 6865 2075 7365 206f 6620 6120 7369   the use of a si
-00000400: 6e67 6c65 2074 656d 7065 7261 7475 7265  ngle temperature
-00000410: 2077 6173 2070 726f 626c 656d 6174 6963   was problematic
-00000420: 9468 075d 9468 158c 5961 2073 6572 696f  .h.].h..Ya serio
-00000430: 7573 2062 7567 2069 6e20 6368 2e66 7265  us bug in ch.fre
-00000440: 6542 6f75 6e64 2077 6173 2066 6978 6564  eBound was fixed
-00000450: 202d 2074 6865 2075 7365 206f 6620 6120   - the use of a 
-00000460: 7369 6e67 6c65 2074 656d 7065 7261 7475  single temperatu
-00000470: 7265 2077 6173 2070 726f 626c 656d 6174  re was problemat
-00000480: 6963 9485 9481 947d 9428 6805 6860 681a  ic.....}.(h.h`h.
-00000490: 685e 6801 6803 681b 4e68 1c4e 7562 6168  h^h.h.h.Nh.Nubah
-000004a0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-000004b0: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
-000004c0: 2a68 1c4b 1068 1a68 2b68 0168 0375 6265  *h.K.h.h+h.h.ube
-000004d0: 681d 7d94 2868 1f5d 948c 1b63 6861 6e67  h.}.(h.]...chang
-000004e0: 6573 2d66 726f 6d2d 302d 382d 372d 746f  es-from-0-8-7-to
-000004f0: 2d30 2d39 2d30 9461 6821 5d94 6823 5d94  -0-9-0.ah!].h#].
-00000500: 8c1b 6368 616e 6765 7320 6672 6f6d 2030  ..changes from 0
-00000510: 2e38 2e37 2074 6f20 302e 392e 3094 6168  .8.7 to 0.9.0.ah
-00000520: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
-00000530: 6801 6803 681b 682a 681c 4b06 7562 680a  h.h.h.h*h.K.ubh.
-00000540: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-00000550: 0f29 8194 7d94 2868 058c 1b43 6861 6e67  .)..}.(h...Chang
-00000560: 6573 2066 726f 6d20 302e 382e 3620 746f  es from 0.8.6 to
-00000570: 2030 2e38 2e37 9468 075d 9468 158c 1b43   0.8.7.h.].h...C
-00000580: 6861 6e67 6573 2066 726f 6d20 302e 382e  hanges from 0.8.
-00000590: 3620 746f 2030 2e38 2e37 9485 9481 947d  6 to 0.8.7.....}
-000005a0: 9428 6805 6879 681a 6877 6801 6803 681b  .(h.hyh.hwh.h.h.
-000005b0: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
-000005c0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000005d0: 7568 2968 0e68 1a68 7468 0168 0368 1b68  uh)h.h.hth.h.h.h
-000005e0: 2a68 1c4b 1375 6268 3d29 8194 7d94 2868  *h.K.ubh=)..}.(h
-000005f0: 058c 1663 6f6e 7469 6e75 6564 2063 6f64  ...continued cod
-00000600: 6520 636c 6561 6e75 7094 6807 5d94 6815  e cleanup.h.].h.
-00000610: 8c16 636f 6e74 696e 7565 6420 636f 6465  ..continued code
-00000620: 2063 6c65 616e 7570 9485 9481 947d 9428   cleanup.....}.(
-00000630: 6805 6887 681a 6885 6801 6803 681b 4e68  h.h.h.h.h.h.h.Nh
-00000640: 1c4e 7562 6168 1d7d 9428 681f 5d94 6821  .Nubah.}.(h.].h!
-00000650: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00000660: 2968 3c68 1b68 2a68 1c4b 1568 1a68 7468  )h<h.h*h.K.h.hth
-00000670: 0168 0375 6265 681d 7d94 2868 1f5d 948c  .h.ubeh.}.(h.]..
-00000680: 1b63 6861 6e67 6573 2d66 726f 6d2d 302d  .changes-from-0-
-00000690: 382d 362d 746f 2d30 2d38 2d37 9461 6821  8-6-to-0-8-7.ah!
-000006a0: 5d94 6823 5d94 8c1b 6368 616e 6765 7320  ].h#]...changes 
-000006b0: 6672 6f6d 2030 2e38 2e36 2074 6f20 302e  from 0.8.6 to 0.
-000006c0: 382e 3794 6168 255d 9468 275d 9475 6829  8.7.ah%].h'].uh)
-000006d0: 6809 681a 680b 6801 6803 681b 682a 681c  h.h.h.h.h.h.h*h.
-000006e0: 4b13 7562 680a 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
-000006f0: 6807 5d94 2868 0f29 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00000700: 1b43 6861 6e67 6573 2066 726f 6d20 302e  .Changes from 0.
-00000710: 382e 3520 746f 2030 2e38 2e36 9468 075d  8.5 to 0.8.6.h.]
-00000720: 9468 158c 1b43 6861 6e67 6573 2066 726f  .h...Changes fro
-00000730: 6d20 302e 382e 3520 746f 2030 2e38 2e36  m 0.8.5 to 0.8.6
-00000740: 9485 9481 947d 9428 6805 68a0 681a 689e  .....}.(h.h.h.h.
-00000750: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
-00000760: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00000770: 5d94 6827 5d94 7568 2968 0e68 1a68 9b68  ].h'].uh)h.h.h.h
-00000780: 0168 0368 1b68 2a68 1c4b 1975 6268 3d29  .h.h.h*h.K.ubh=)
-00000790: 8194 7d94 2868 058c 1761 6e6f 7468 6572  ..}.(h...another
-000007a0: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
-000007b0: 9468 075d 9468 158c 1761 6e6f 7468 6572  .h.].h...another
-000007c0: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
-000007d0: 9485 9481 947d 9428 6805 68ae 681a 68ac  .....}.(h.h.h.h.
-000007e0: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
-000007f0: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00000800: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
-00000810: 1c4b 1b68 1a68 9b68 0168 0375 6268 3d29  .K.h.h.h.h.ubh=)
-00000820: 8194 7d94 2868 058c 6a61 6464 6564 2061  ..}.(h..jadded a
-00000830: 7267 4368 6563 6b20 6d65 7468 6f64 2074  rgCheck method t
-00000840: 6f20 6d61 6b65 2073 7572 6520 7468 6174  o make sure that
-00000850: 2073 697a 6573 206f 6620 7465 6d70 6572   sizes of temper
-00000860: 6174 7572 652c 2064 656e 7369 7479 2061  ature, density a
-00000870: 6e64 2065 6d69 7373 696f 6e20 6d65 6173  nd emission meas
-00000880: 7572 6520 7765 7265 2063 6f6d 7061 7469  ure were compati
-00000890: 626c 6594 6807 5d94 6815 8c6a 6164 6465  ble.h.].h..jadde
-000008a0: 6420 6172 6743 6865 636b 206d 6574 686f  d argCheck metho
-000008b0: 6420 746f 206d 616b 6520 7375 7265 2074  d to make sure t
-000008c0: 6861 7420 7369 7a65 7320 6f66 2074 656d  hat sizes of tem
-000008d0: 7065 7261 7475 7265 2c20 6465 6e73 6974  perature, densit
-000008e0: 7920 616e 6420 656d 6973 7369 6f6e 206d  y and emission m
-000008f0: 6561 7375 7265 2077 6572 6520 636f 6d70  easure were comp
-00000900: 6174 6962 6c65 9485 9481 947d 9428 6805  atible.....}.(h.
-00000910: 68bc 681a 68ba 6801 6803 681b 4e68 1c4e  h.h.h.h.h.h.Nh.N
-00000920: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-00000930: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-00000940: 3c68 1b68 2a68 1c4b 1d68 1a68 9b68 0168  <h.h*h.K.h.h.h.h
-00000950: 0375 6265 681d 7d94 2868 1f5d 948c 1b63  .ubeh.}.(h.]...c
-00000960: 6861 6e67 6573 2d66 726f 6d2d 302d 382d  hanges-from-0-8-
-00000970: 352d 746f 2d30 2d38 2d36 9461 6821 5d94  5-to-0-8-6.ah!].
-00000980: 6823 5d94 8c1b 6368 616e 6765 7320 6672  h#]...changes fr
-00000990: 6f6d 2030 2e38 2e35 2074 6f20 302e 382e  om 0.8.5 to 0.8.
-000009a0: 3694 6168 255d 9468 275d 9475 6829 6809  6.ah%].h'].uh)h.
-000009b0: 681a 680b 6801 6803 681b 682a 681c 4b19  h.h.h.h.h.h*h.K.
-000009c0: 7562 680a 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-000009d0: 5d94 680f 2981 947d 9428 6805 8c1b 4368  ].h.)..}.(h...Ch
-000009e0: 616e 6765 7320 6672 6f6d 2030 2e38 2e34  anges from 0.8.4
-000009f0: 2074 6f20 302e 382e 3594 6807 5d94 6815   to 0.8.5.h.].h.
+00000220: 2981 947d 9428 6805 8c1a 7468 6973 2069  )..}.(h...this i
+00000230: 7320 6120 6275 672d 6669 7820 7265 6c65  s a bug-fix rele
+00000240: 6173 652e 9468 075d 9468 158c 1a74 6869  ase..h.].h...thi
+00000250: 7320 6973 2061 2062 7567 2d66 6978 2072  s is a bug-fix r
+00000260: 656c 6561 7365 2e94 8594 8194 7d94 2868  elease......}.(h
+00000270: 0568 4068 1a68 3e68 0168 0368 1b4e 681c  .h@h.h>h.h.h.Nh.
+00000280: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+00000290: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+000002a0: 683c 681b 682a 681c 4b09 681a 682b 6801  h<h.h*h.K.h.h+h.
+000002b0: 6803 7562 683d 2981 947d 9428 6805 8c6d  h.ubh=)..}.(h..m
+000002c0: 6120 6275 6720 696e 2074 6865 2069 6e68  a bug in the inh
+000002d0: 6572 6974 6564 206d 6574 686f 6420 6261  erited method ba
+000002e0: 7365 2e5f 496e 7465 6e73 6974 7952 6174  se._IntensityRat
+000002f0: 696f 2829 2068 6164 2061 2070 726f 626c  io() had a probl
+00000300: 656d 2069 6620 6c69 6e65 7320 7765 7265  em if lines were
+00000310: 2073 656c 6563 7465 6420 6672 6f6d 2064   selected from d
+00000320: 6966 6665 7265 6e74 2069 6f6e 7394 6807  ifferent ions.h.
+00000330: 5d94 6815 8c6d 6120 6275 6720 696e 2074  ].h..ma bug in t
+00000340: 6865 2069 6e68 6572 6974 6564 206d 6574  he inherited met
+00000350: 686f 6420 6261 7365 2e5f 496e 7465 6e73  hod base._Intens
+00000360: 6974 7952 6174 696f 2829 2068 6164 2061  ityRatio() had a
+00000370: 2070 726f 626c 656d 2069 6620 6c69 6e65   problem if line
+00000380: 7320 7765 7265 2073 656c 6563 7465 6420  s were selected 
+00000390: 6672 6f6d 2064 6966 6665 7265 6e74 2069  from different i
+000003a0: 6f6e 7394 8594 8194 7d94 2868 0568 4e68  ons.....}.(h.hNh
+000003b0: 1a68 4c68 0168 0368 1b4e 681c 4e75 6261  .hLh.h.h.Nh.Nuba
+000003c0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+000003d0: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+000003e0: 682a 681c 4b0b 681a 682b 6801 6803 7562  h*h.K.h.h+h.h.ub
+000003f0: 6568 1d7d 9428 681f 5d94 8c1b 6368 616e  eh.}.(h.]...chan
+00000400: 6765 732d 6672 6f6d 2d30 2d39 2d34 2d74  ges-from-0-9-4-t
+00000410: 6f2d 302d 392d 3594 6168 215d 9468 235d  o-0-9-5.ah!].h#]
+00000420: 948c 1b63 6861 6e67 6573 2066 726f 6d20  ...changes from 
+00000430: 302e 392e 3420 746f 2030 2e39 2e35 9461  0.9.4 to 0.9.5.a
+00000440: 6825 5d94 6827 5d94 7568 2968 0968 1a68  h%].h'].uh)h.h.h
+00000450: 0b68 0168 0368 1b68 2a68 1c4b 0775 6268  .h.h.h.h*h.K.ubh
+00000460: 0a29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00000470: 680f 2981 947d 9428 6805 8c1b 4368 616e  h.)..}.(h...Chan
+00000480: 6765 7320 6672 6f6d 2030 2e39 2e33 2074  ges from 0.9.3 t
+00000490: 6f20 302e 392e 3494 6807 5d94 6815 8c1b  o 0.9.4.h.].h...
+000004a0: 4368 616e 6765 7320 6672 6f6d 2030 2e39  Changes from 0.9
+000004b0: 2e33 2074 6f20 302e 392e 3494 8594 8194  .3 to 0.9.4.....
+000004c0: 7d94 2868 0568 6768 1a68 6568 0168 0368  }.(h.hgh.heh.h.h
+000004d0: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+000004e0: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+000004f0: 9475 6829 680e 681a 6862 6801 6803 681b  .uh)h.h.hbh.h.h.
+00000500: 682a 681c 4b0f 7562 683d 2981 947d 9428  h*h.K.ubh=)..}.(
+00000510: 6805 8c1a 7468 6973 2069 7320 6120 6275  h...this is a bu
+00000520: 672d 6669 7820 7265 6c65 6173 652e 9468  g-fix release..h
+00000530: 075d 9468 158c 1a74 6869 7320 6973 2061  .].h...this is a
+00000540: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
+00000550: 2e94 8594 8194 7d94 2868 0568 7568 1a68  ......}.(h.huh.h
+00000560: 7368 0168 0368 1b4e 681c 4e75 6261 681d  sh.h.h.Nh.Nubah.
+00000570: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00000580: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
+00000590: 681c 4b11 681a 6862 6801 6803 7562 683d  h.K.h.hbh.h.ubh=
+000005a0: 2981 947d 9428 6805 8c60 6368 616e 6765  )..}.(h..`change
+000005b0: 7320 696e 2076 6572 7369 6f6e 2030 2e39  s in version 0.9
+000005c0: 2e32 2063 6f6e 7469 6e75 6564 2074 6f20  .2 continued to 
+000005d0: 6769 7665 2070 726f 626c 656d 7320 7769  give problems wi
+000005e0: 7468 2069 6f6e 7320 7468 6174 2069 6e63  th ions that inc
+000005f0: 6c75 6465 6420 6175 746f 696f 6e69 7a61  luded autoioniza
+00000600: 7469 6f6e 2072 6174 6573 9468 075d 9468  tion rates.h.].h
+00000610: 158c 6063 6861 6e67 6573 2069 6e20 7665  ..`changes in ve
+00000620: 7273 696f 6e20 302e 392e 3220 636f 6e74  rsion 0.9.2 cont
+00000630: 696e 7565 6420 746f 2067 6976 6520 7072  inued to give pr
+00000640: 6f62 6c65 6d73 2077 6974 6820 696f 6e73  oblems with ions
+00000650: 2074 6861 7420 696e 636c 7564 6564 2061   that included a
+00000660: 7574 6f69 6f6e 697a 6174 696f 6e20 7261  utoionization ra
+00000670: 7465 7394 8594 8194 7d94 2868 0568 8368  tes.....}.(h.h.h
+00000680: 1a68 8168 0168 0368 1b4e 681c 4e75 6261  .h.h.h.h.Nh.Nuba
+00000690: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+000006a0: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+000006b0: 682a 681c 4b13 681a 6862 6801 6803 7562  h*h.K.h.hbh.h.ub
+000006c0: 6568 1d7d 9428 681f 5d94 8c1b 6368 616e  eh.}.(h.]...chan
+000006d0: 6765 732d 6672 6f6d 2d30 2d39 2d33 2d74  ges-from-0-9-3-t
+000006e0: 6f2d 302d 392d 3494 6168 215d 9468 235d  o-0-9-4.ah!].h#]
+000006f0: 948c 1b63 6861 6e67 6573 2066 726f 6d20  ...changes from 
+00000700: 302e 392e 3320 746f 2030 2e39 2e34 9461  0.9.3 to 0.9.4.a
+00000710: 6825 5d94 6827 5d94 7568 2968 0968 1a68  h%].h'].uh)h.h.h
+00000720: 0b68 0168 0368 1b68 2a68 1c4b 0f75 6268  .h.h.h.h*h.K.ubh
+00000730: 0a29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00000740: 680f 2981 947d 9428 6805 8c1b 4368 616e  h.)..}.(h...Chan
+00000750: 6765 7320 6672 6f6d 2030 2e39 2e33 2074  ges from 0.9.3 t
+00000760: 6f20 302e 392e 3394 6807 5d94 6815 8c1b  o 0.9.3.h.].h...
+00000770: 4368 616e 6765 7320 6672 6f6d 2030 2e39  Changes from 0.9
+00000780: 2e33 2074 6f20 302e 392e 3394 8594 8194  .3 to 0.9.3.....
+00000790: 7d94 2868 0568 9c68 1a68 9a68 0168 0368  }.(h.h.h.h.h.h.h
+000007a0: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+000007b0: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+000007c0: 9475 6829 680e 681a 6897 6801 6803 681b  .uh)h.h.h.h.h.h.
+000007d0: 682a 681c 4b17 7562 683d 2981 947d 9428  h*h.K.ubh=)..}.(
+000007e0: 6805 8c1a 7468 6973 2069 7320 6120 6275  h...this is a bu
+000007f0: 672d 6669 7820 7265 6c65 6173 652e 9468  g-fix release..h
+00000800: 075d 9468 158c 1a74 6869 7320 6973 2061  .].h...this is a
+00000810: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
+00000820: 2e94 8594 8194 7d94 2868 0568 aa68 1a68  ......}.(h.h.h.h
+00000830: a868 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
+00000840: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00000850: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
+00000860: 681c 4b19 681a 6897 6801 6803 7562 683d  h.K.h.h.h.h.ubh=
+00000870: 2981 947d 9428 6805 8c53 6368 616e 6765  )..}.(h..Schange
+00000880: 7320 696e 2076 6572 7369 6f6e 2030 2e39  s in version 0.9
+00000890: 2e32 2067 6176 6520 7072 6f62 6c65 6d73  .2 gave problems
+000008a0: 2077 6974 6820 696f 6e73 2074 6861 7420   with ions that 
+000008b0: 696e 636c 7564 6564 2061 7574 6f69 6f6e  included autoion
+000008c0: 697a 6174 696f 6e20 7261 7465 7394 6807  ization rates.h.
+000008d0: 5d94 6815 8c53 6368 616e 6765 7320 696e  ].h..Schanges in
+000008e0: 2076 6572 7369 6f6e 2030 2e39 2e32 2067   version 0.9.2 g
+000008f0: 6176 6520 7072 6f62 6c65 6d73 2077 6974  ave problems wit
+00000900: 6820 696f 6e73 2074 6861 7420 696e 636c  h ions that incl
+00000910: 7564 6564 2061 7574 6f69 6f6e 697a 6174  uded autoionizat
+00000920: 696f 6e20 7261 7465 7394 8594 8194 7d94  ion rates.....}.
+00000930: 2868 0568 b868 1a68 b668 0168 0368 1b4e  (h.h.h.h.h.h.h.N
+00000940: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00000950: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00000960: 6829 683c 681b 682a 681c 4b1b 681a 6897  h)h<h.h*h.K.h.h.
+00000970: 6801 6803 7562 6568 1d7d 9428 681f 5d94  h.h.ubeh.}.(h.].
+00000980: 8c1b 6368 616e 6765 732d 6672 6f6d 2d30  ..changes-from-0
+00000990: 2d39 2d33 2d74 6f2d 302d 392d 3394 6168  -9-3-to-0-9-3.ah
+000009a0: 215d 9468 235d 948c 1b63 6861 6e67 6573  !].h#]...changes
+000009b0: 2066 726f 6d20 302e 392e 3320 746f 2030   from 0.9.3 to 0
+000009c0: 2e39 2e33 9461 6825 5d94 6827 5d94 7568  .9.3.ah%].h'].uh
+000009d0: 2968 0968 1a68 0b68 0168 0368 1b68 2a68  )h.h.h.h.h.h.h*h
+000009e0: 1c4b 1775 6268 0a29 8194 7d94 2868 0568  .K.ubh.)..}.(h.h
+000009f0: 0668 075d 9428 680f 2981 947d 9428 6805  .h.].(h.)..}.(h.
 00000a00: 8c1b 4368 616e 6765 7320 6672 6f6d 2030  ..Changes from 0
-00000a10: 2e38 2e34 2074 6f20 302e 382e 3594 8594  .8.4 to 0.8.5...
-00000a20: 8194 7d94 2868 0568 d568 1a68 d368 0168  ..}.(h.h.h.h.h.h
-00000a30: 0368 1b4e 681c 4e75 6261 681d 7d94 2868  .h.Nh.Nubah.}.(h
-00000a40: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-00000a50: 275d 9475 6829 680e 681a 68d0 6801 6803  '].uh)h.h.h.h.h.
-00000a60: 681b 682a 681c 4b20 7562 6168 1d7d 9428  h.h*h.K ubah.}.(
-00000a70: 681f 5d94 8c1b 6368 616e 6765 732d 6672  h.]...changes-fr
-00000a80: 6f6d 2d30 2d38 2d34 2d74 6f2d 302d 382d  om-0-8-4-to-0-8-
-00000a90: 3594 6168 215d 9468 235d 948c 1b63 6861  5.ah!].h#]...cha
-00000aa0: 6e67 6573 2066 726f 6d20 302e 382e 3420  nges from 0.8.4 
-00000ab0: 746f 2030 2e38 2e35 9461 6825 5d94 6827  to 0.8.5.ah%].h'
-00000ac0: 5d94 7568 2968 0968 1a68 0b68 0168 0368  ].uh)h.h.h.h.h.h
-00000ad0: 1b68 2a68 1c4b 2075 6268 0a29 8194 7d94  .h*h.K ubh.)..}.
-00000ae0: 2868 0568 0668 075d 9428 680f 2981 947d  (h.h.h.].(h.)..}
-00000af0: 9428 6805 8c20 5468 6973 2069 7320 6120  .(h.. This is a 
-00000b00: 6d61 6a6f 7220 6275 672d 6669 7820 7265  major bug-fix re
-00000b10: 6c65 6173 652e 9468 075d 9468 158c 2054  lease..h.].h.. T
-00000b20: 6869 7320 6973 2061 206d 616a 6f72 2062  his is a major b
-00000b30: 7567 2d66 6978 2072 656c 6561 7365 2e94  ug-fix release..
-00000b40: 8594 8194 7d94 2868 0568 ee68 1a68 ec68  ....}.(h.h.h.h.h
-00000b50: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
-00000b60: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-00000b70: 9468 275d 9475 6829 680e 681a 68e9 6801  .h'].uh)h.h.h.h.
-00000b80: 6803 681b 682a 681c 4b23 7562 683d 2981  h.h.h*h.K#ubh=).
-00000b90: 947d 9428 6805 8c36 4572 726f 7273 2069  .}.(h..6Errors i
-00000ba0: 6e20 6361 6c63 756c 6174 696e 6720 7468  n calculating th
-00000bb0: 6520 7072 6f74 6f6e 2072 6174 6573 2077  e proton rates w
-00000bc0: 6572 6520 636f 7272 6563 7465 642e 9468  ere corrected..h
-00000bd0: 075d 9468 158c 3645 7272 6f72 7320 696e  .].h..6Errors in
-00000be0: 2063 616c 6375 6c61 7469 6e67 2074 6865   calculating the
-00000bf0: 2070 726f 746f 6e20 7261 7465 7320 7765   proton rates we
-00000c00: 7265 2063 6f72 7265 6374 6564 2e94 8594  re corrected....
-00000c10: 8194 7d94 2868 0568 fc68 1a68 fa68 0168  ..}.(h.h.h.h.h.h
-00000c20: 0368 1b4e 681c 4e75 6261 681d 7d94 2868  .h.Nh.Nubah.}.(h
-00000c30: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-00000c40: 275d 9475 6829 683c 681b 682a 681c 4b25  '].uh)h<h.h*h.K%
-00000c50: 681a 68e9 6801 6803 7562 683d 2981 947d  h.h.h.h.ubh=)..}
-00000c60: 9428 6805 8c33 416c 6c20 7465 6d70 6572  .(h..3All temper
-00000c70: 6174 7572 6573 2061 6e64 2064 656e 7369  atures and densi
-00000c80: 7469 6573 2061 7265 206e 6f77 206e 756d  ties are now num
-00000c90: 7079 2061 7272 6179 7394 6807 5d94 6815  py arrays.h.].h.
-00000ca0: 8c33 416c 6c20 7465 6d70 6572 6174 7572  .3All temperatur
-00000cb0: 6573 2061 6e64 2064 656e 7369 7469 6573  es and densities
-00000cc0: 2061 7265 206e 6f77 206e 756d 7079 2061   are now numpy a
-00000cd0: 7272 6179 7394 8594 8194 7d94 2868 056a  rrays.....}.(h.j
-00000ce0: 0a01 0000 681a 6a08 0100 0068 0168 0368  ....h.j....h.h.h
-00000cf0: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
-00000d00: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
-00000d10: 9475 6829 683c 681b 682a 681c 4b27 681a  .uh)h<h.h*h.K'h.
-00000d20: 68e9 6801 6803 7562 6568 1d7d 9428 681f  h.h.h.ubeh.}.(h.
-00000d30: 5d94 8c1f 7468 6973 2d69 732d 612d 6d61  ]...this-is-a-ma
-00000d40: 6a6f 722d 6275 672d 6669 782d 7265 6c65  jor-bug-fix-rele
-00000d50: 6173 6594 6168 215d 9468 235d 9468 255d  ase.ah!].h#].h%]
-00000d60: 948c 2074 6869 7320 6973 2061 206d 616a  .. this is a maj
-00000d70: 6f72 2062 7567 2d66 6978 2072 656c 6561  or bug-fix relea
-00000d80: 7365 2e94 6168 275d 9475 6829 6809 681a  se..ah'].uh)h.h.
-00000d90: 680b 6801 6803 681b 682a 681c 4b23 8c0a  h.h.h.h.h*h.K#..
-00000da0: 7265 6665 7265 6e63 6564 944b 0175 6268  referenced.K.ubh
-00000db0: 0a29 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
-00000dc0: 0f29 8194 7d94 2868 058c 1b43 6861 6e67  .)..}.(h...Chang
-00000dd0: 6573 2066 726f 6d20 302e 382e 3320 746f  es from 0.8.3 to
-00000de0: 2030 2e38 2e34 9468 075d 9468 158c 1b43   0.8.4.h.].h...C
-00000df0: 6861 6e67 6573 2066 726f 6d20 302e 382e  hanges from 0.8.
-00000e00: 3320 746f 2030 2e38 2e34 9485 9481 947d  3 to 0.8.4.....}
-00000e10: 9428 6805 6a24 0100 0068 1a6a 2201 0000  .(h.j$...h.j"...
-00000e20: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
-00000e30: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00000e40: 5d94 6827 5d94 7568 2968 0e68 1a6a 1f01  ].h'].uh)h.h.j..
-00000e50: 0000 6801 6803 681b 682a 681c 4b2b 7562  ..h.h.h.h*h.K+ub
-00000e60: 6168 1d7d 9428 681f 5d94 8c1b 6368 616e  ah.}.(h.]...chan
-00000e70: 6765 732d 6672 6f6d 2d30 2d38 2d33 2d74  ges-from-0-8-3-t
-00000e80: 6f2d 302d 382d 3494 6168 215d 9468 235d  o-0-8-4.ah!].h#]
-00000e90: 948c 1b63 6861 6e67 6573 2066 726f 6d20  ...changes from 
-00000ea0: 302e 382e 3320 746f 2030 2e38 2e34 9461  0.8.3 to 0.8.4.a
-00000eb0: 6825 5d94 6827 5d94 7568 2968 0968 1a68  h%].h'].uh)h.h.h
-00000ec0: 0b68 0168 0368 1b68 2a68 1c4b 2b75 6268  .h.h.h.h*h.K+ubh
-00000ed0: 0a29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00000ee0: 680f 2981 947d 9428 6805 8c20 5468 6973  h.)..}.(h.. This
-00000ef0: 2069 7320 6120 6d61 6a6f 7220 6275 672d   is a major bug-
-00000f00: 6669 7820 7265 6c65 6173 652e 9468 075d  fix release..h.]
-00000f10: 9468 158c 2054 6869 7320 6973 2061 206d  .h.. This is a m
-00000f20: 616a 6f72 2062 7567 2d66 6978 2072 656c  ajor bug-fix rel
-00000f30: 6561 7365 2e94 8594 8194 7d94 2868 056a  ease......}.(h.j
-00000f40: 3d01 0000 681a 6a3b 0100 0068 0168 0368  =...h.j;...h.h.h
-00000f50: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
-00000f60: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
-00000f70: 9475 6829 680e 681a 6a38 0100 0068 0168  .uh)h.h.j8...h.h
-00000f80: 0368 1b68 2a68 1c4b 2e75 6268 3d29 8194  .h.h*h.K.ubh=)..
-00000f90: 7d94 2868 058c 4741 6e6f 7468 6572 2073  }.(h..GAnother s
-00000fa0: 6967 6e69 6669 6361 6e74 2062 7567 2077  ignificant bug w
-00000fb0: 6173 2066 6978 6564 2069 6e20 7468 6520  as fixed in the 
-00000fc0: 696d 706f 7274 616e 7420 696f 6e2e 706f  important ion.po
-00000fd0: 7075 6c61 7465 206d 6574 686f 642e 9468  pulate method..h
-00000fe0: 075d 9468 158c 4741 6e6f 7468 6572 2073  .].h..GAnother s
-00000ff0: 6967 6e69 6669 6361 6e74 2062 7567 2077  ignificant bug w
-00001000: 6173 2066 6978 6564 2069 6e20 7468 6520  as fixed in the 
-00001010: 696d 706f 7274 616e 7420 696f 6e2e 706f  important ion.po
-00001020: 7075 6c61 7465 206d 6574 686f 642e 9485  pulate method...
-00001030: 9481 947d 9428 6805 6a4b 0100 0068 1a6a  ...}.(h.jK...h.j
-00001040: 4901 0000 6801 6803 681b 4e68 1c4e 7562  I...h.h.h.Nh.Nub
-00001050: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-00001060: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
-00001070: 1b68 2a68 1c4b 3068 1a6a 3801 0000 6801  .h*h.K0h.j8...h.
-00001080: 6803 7562 6568 1d7d 9428 681f 5d94 8c03  h.ubeh.}.(h.]...
-00001090: 6964 3194 6168 215d 9468 235d 9468 255d  id1.ah!].h#].h%]
-000010a0: 946a 1c01 0000 6168 275d 9475 6829 6809  .j....ah'].uh)h.
-000010b0: 681a 680b 6801 6803 681b 682a 681c 4b2e  h.h.h.h.h.h*h.K.
-000010c0: 6a1e 0100 004b 0175 6268 0a29 8194 7d94  j....K.ubh.)..}.
-000010d0: 2868 0568 0668 075d 9468 0f29 8194 7d94  (h.h.h.].h.)..}.
-000010e0: 2868 058c 1b43 6861 6e67 6573 2066 726f  (h...Changes fro
-000010f0: 6d20 302e 372e 3120 746f 2030 2e38 2e33  m 0.7.1 to 0.8.3
-00001100: 9468 075d 9468 158c 1b43 6861 6e67 6573  .h.].h...Changes
-00001110: 2066 726f 6d20 302e 372e 3120 746f 2030   from 0.7.1 to 0
-00001120: 2e38 2e33 9485 9481 947d 9428 6805 6a63  .8.3.....}.(h.jc
-00001130: 0100 0068 1a6a 6101 0000 6801 6803 681b  ...h.ja...h.h.h.
-00001140: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
-00001150: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001160: 7568 2968 0e68 1a6a 5e01 0000 6801 6803  uh)h.h.j^...h.h.
-00001170: 681b 682a 681c 4b34 7562 6168 1d7d 9428  h.h*h.K4ubah.}.(
-00001180: 681f 5d94 8c1b 6368 616e 6765 732d 6672  h.]...changes-fr
-00001190: 6f6d 2d30 2d37 2d31 2d74 6f2d 302d 382d  om-0-7-1-to-0-8-
-000011a0: 3394 6168 215d 9468 235d 948c 1b63 6861  3.ah!].h#]...cha
-000011b0: 6e67 6573 2066 726f 6d20 302e 372e 3120  nges from 0.7.1 
-000011c0: 746f 2030 2e38 2e33 9461 6825 5d94 6827  to 0.8.3.ah%].h'
-000011d0: 5d94 7568 2968 0968 1a68 0b68 0168 0368  ].uh)h.h.h.h.h.h
-000011e0: 1b68 2a68 1c4b 3475 6268 0a29 8194 7d94  .h*h.K4ubh.)..}.
-000011f0: 2868 0568 0668 075d 9428 680f 2981 947d  (h.h.h.].(h.)..}
-00001200: 9428 6805 8c20 5468 6973 2069 7320 6120  .(h.. This is a 
-00001210: 6d61 6a6f 7220 6275 672d 6669 7820 7265  major bug-fix re
-00001220: 6c65 6173 652e 9468 075d 9468 158c 2054  lease..h.].h.. T
-00001230: 6869 7320 6973 2061 206d 616a 6f72 2062  his is a major b
-00001240: 7567 2d66 6978 2072 656c 6561 7365 2e94  ug-fix release..
-00001250: 8594 8194 7d94 2868 056a 7c01 0000 681a  ....}.(h.j|...h.
-00001260: 6a7a 0100 0068 0168 0368 1b4e 681c 4e75  jz...h.h.h.Nh.Nu
-00001270: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
-00001280: 235d 9468 255d 9468 275d 9475 6829 680e  #].h%].h'].uh)h.
-00001290: 681a 6a77 0100 0068 0168 0368 1b68 2a68  h.jw...h.h.h.h*h
-000012a0: 1c4b 3775 6268 3d29 8194 7d94 2868 058c  .K7ubh=)..}.(h..
-000012b0: 4661 2073 6d61 6c6c 2062 7574 206d 6967  Fa small but mig
-000012c0: 6874 7920 6275 6720 7761 7320 666f 756e  hty bug was foun
-000012d0: 6420 696e 2074 6865 2069 6d70 6f72 7461  d in the importa
-000012e0: 6e74 2069 6f6e 2e70 6f70 756c 6174 6520  nt ion.populate 
-000012f0: 6d65 7468 6f64 2e94 6807 5d94 6815 8c46  method..h.].h..F
-00001300: 6120 736d 616c 6c20 6275 7420 6d69 6768  a small but migh
-00001310: 7479 2062 7567 2077 6173 2066 6f75 6e64  ty bug was found
-00001320: 2069 6e20 7468 6520 696d 706f 7274 616e   in the importan
-00001330: 7420 696f 6e2e 706f 7075 6c61 7465 206d  t ion.populate m
-00001340: 6574 686f 642e 9485 9481 947d 9428 6805  ethod......}.(h.
-00001350: 6a8a 0100 0068 1a6a 8801 0000 6801 6803  j....h.j....h.h.
-00001360: 681b 4e68 1c4e 7562 6168 1d7d 9428 681f  h.Nh.Nubah.}.(h.
-00001370: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00001380: 5d94 7568 2968 3c68 1b68 2a68 1c4b 3968  ].uh)h<h.h*h.K9h
-00001390: 1a6a 7701 0000 6801 6803 7562 6568 1d7d  .jw...h.h.ubeh.}
-000013a0: 9428 681f 5d94 8c03 6964 3294 6168 215d  .(h.]...id2.ah!]
-000013b0: 9468 235d 9468 255d 948c 2074 6869 7320  .h#].h%].. this 
-000013c0: 6973 2061 206d 616a 6f72 2062 7567 2d66  is a major bug-f
-000013d0: 6978 2072 656c 6561 7365 2e94 6168 275d  ix release..ah']
-000013e0: 9475 6829 6809 681a 680b 6801 6803 681b  .uh)h.h.h.h.h.h.
-000013f0: 682a 681c 4b37 6a1e 0100 004b 0175 6268  h*h.K7j....K.ubh
-00001400: 0a29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00001410: 680f 2981 947d 9428 6805 8c52 5665 7273  h.)..}.(h..RVers
-00001420: 696f 6e20 302e 382e 7820 6669 6c65 7320  ion 0.8.x files 
-00001430: 6172 6520 6e65 6365 7373 6172 7920 746f  are necessary to
-00001440: 2075 7365 2077 6974 6820 7468 6520 6e65   use with the ne
-00001450: 7720 4348 4941 4e54 4920 5665 7273 696f  w CHIANTI Versio
-00001460: 6e20 392e 3020 6461 7461 6261 7365 9468  n 9.0 database.h
-00001470: 075d 9468 158c 5256 6572 7369 6f6e 2030  .].h..RVersion 0
-00001480: 2e38 2e78 2066 696c 6573 2061 7265 206e  .8.x files are n
-00001490: 6563 6573 7361 7279 2074 6f20 7573 6520  ecessary to use 
-000014a0: 7769 7468 2074 6865 206e 6577 2043 4849  with the new CHI
-000014b0: 414e 5449 2056 6572 7369 6f6e 2039 2e30  ANTI Version 9.0
-000014c0: 2064 6174 6162 6173 6594 8594 8194 7d94   database.....}.
-000014d0: 2868 056a a301 0000 681a 6aa1 0100 0068  (h.j....h.j....h
-000014e0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
-000014f0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-00001500: 9468 275d 9475 6829 680e 681a 6a9e 0100  .h'].uh)h.h.j...
-00001510: 0068 0168 0368 1b68 2a68 1c4b 3c75 6268  .h.h.h.h*h.K<ubh
-00001520: 3d29 8194 7d94 2868 058c 7e43 6861 6e67  =)..}.(h..~Chang
-00001530: 6573 2068 6176 6520 6265 656e 206d 6164  es have been mad
-00001540: 6520 746f 2074 616b 6520 696e 746f 2061  e to take into a
-00001550: 6363 6f75 6e74 2074 6865 206e 6577 2077  ccount the new w
-00001560: 6179 2074 6861 7420 4348 4941 4e54 4920  ay that CHIANTI 
-00001570: 6973 2068 616e 646c 696e 6720 6469 656c  is handling diel
-00001580: 6563 7472 6f6e 6963 2072 6563 6f6d 6269  ectronic recombi
-00001590: 6e61 7469 6f6e 2061 6e64 2061 7574 6f69  nation and autoi
-000015a0: 6f6e 697a 6174 696f 6e94 6807 5d94 6815  onization.h.].h.
-000015b0: 8c7e 4368 616e 6765 7320 6861 7665 2062  .~Changes have b
-000015c0: 6565 6e20 6d61 6465 2074 6f20 7461 6b65  een made to take
-000015d0: 2069 6e74 6f20 6163 636f 756e 7420 7468   into account th
-000015e0: 6520 6e65 7720 7761 7920 7468 6174 2043  e new way that C
-000015f0: 4849 414e 5449 2069 7320 6861 6e64 6c69  HIANTI is handli
-00001600: 6e67 2064 6965 6c65 6374 726f 6e69 6320  ng dielectronic 
-00001610: 7265 636f 6d62 696e 6174 696f 6e20 616e  recombination an
-00001620: 6420 6175 746f 696f 6e69 7a61 7469 6f6e  d autoionization
-00001630: 9485 9481 947d 9428 6805 6ab1 0100 0068  .....}.(h.j....h
-00001640: 1a6a af01 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-00001650: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-00001660: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-00001670: 3c68 1b68 2a68 1c4b 3e68 1a6a 9e01 0000  <h.h*h.K>h.j....
-00001680: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
-00001690: 8c4c 5468 6520 7265 6c65 6173 6520 6973  .LThe release is
-000016a0: 2061 6c73 6f20 6176 6169 6c61 626c 6520   also available 
-000016b0: 6f6e 205b 5079 5049 5d28 6874 7470 733a  on [PyPI](https:
-000016c0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000016d0: 6374 2f43 6869 616e 7469 5079 2f29 9468  ct/ChiantiPy/).h
-000016e0: 075d 9428 6815 8c28 5468 6520 7265 6c65  .].(h..(The rele
-000016f0: 6173 6520 6973 2061 6c73 6f20 6176 6169  ase is also avai
-00001700: 6c61 626c 6520 6f6e 205b 5079 5049 5d28  lable on [PyPI](
-00001710: 9485 9481 947d 9428 6805 8c28 5468 6520  .....}.(h..(The 
-00001720: 7265 6c65 6173 6520 6973 2061 6c73 6f20  release is also 
-00001730: 6176 6169 6c61 626c 6520 6f6e 205b 5079  available on [Py
-00001740: 5049 5d28 9468 1a6a bd01 0000 6801 6803  PI](.h.j....h.h.
-00001750: 681b 4e68 1c4e 7562 6800 8c09 7265 6665  h.Nh.Nubh...refe
-00001760: 7265 6e63 6594 9394 2981 947d 9428 6805  rence...)..}.(h.
-00001770: 8c23 6874 7470 733a 2f2f 7079 7069 2e6f  .#https://pypi.o
-00001780: 7267 2f70 726f 6a65 6374 2f43 6869 616e  rg/project/Chian
-00001790: 7469 5079 2f94 6807 5d94 6815 8c23 6874  tiPy/.h.].h..#ht
-000017a0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000017b0: 726f 6a65 6374 2f43 6869 616e 7469 5079  roject/ChiantiPy
-000017c0: 2f94 8594 8194 7d94 2868 0568 0668 1a6a  /.....}.(h.h.h.j
-000017d0: c801 0000 7562 6168 1d7d 9428 681f 5d94  ....ubah.}.(h.].
-000017e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000017f0: 8c06 7265 6675 7269 946a ca01 0000 7568  ..refuri.j....uh
-00001800: 296a c601 0000 681a 6abd 0100 0075 6268  )j....h.j....ubh
-00001810: 158c 0129 9485 9481 947d 9428 6805 8c01  ...).....}.(h...
-00001820: 2994 681a 6abd 0100 0068 0168 0368 1b4e  ).h.j....h.h.h.N
-00001830: 681c 4e75 6265 681d 7d94 2868 1f5d 9468  h.Nubeh.}.(h.].h
-00001840: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
-00001850: 6829 683c 681b 682a 681c 4b40 681a 6a9e  h)h<h.h*h.K@h.j.
-00001860: 0100 0068 0168 0375 6268 3d29 8194 7d94  ...h.h.ubh=)..}.
-00001870: 2868 058c 4c44 6f63 756d 656e 7461 7469  (h..LDocumentati
-00001880: 6f6e 2069 7320 6176 6169 6c61 626c 6520  on is available 
-00001890: 6f6e 205b 6769 7468 7562 2e69 6f5d 2868  on [github.io](h
-000018a0: 7474 7073 3a2f 2f63 6869 616e 7469 2d61  ttps://chianti-a
-000018b0: 746f 6d69 632e 6769 7468 7562 2e69 6f2f  tomic.github.io/
-000018c0: 2994 6807 5d94 2868 158c 2a44 6f63 756d  ).h.].(h..*Docum
-000018d0: 656e 7461 7469 6f6e 2069 7320 6176 6169  entation is avai
-000018e0: 6c61 626c 6520 6f6e 205b 6769 7468 7562  lable on [github
-000018f0: 2e69 6f5d 2894 8594 8194 7d94 2868 058c  .io](.....}.(h..
-00001900: 2a44 6f63 756d 656e 7461 7469 6f6e 2069  *Documentation i
-00001910: 7320 6176 6169 6c61 626c 6520 6f6e 205b  s available on [
-00001920: 6769 7468 7562 2e69 6f5d 2894 681a 6ae2  github.io](.h.j.
-00001930: 0100 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
-00001940: c701 0000 2981 947d 9428 6805 8c21 6874  ....)..}.(h..!ht
-00001950: 7470 733a 2f2f 6368 6961 6e74 692d 6174  tps://chianti-at
-00001960: 6f6d 6963 2e67 6974 6875 622e 696f 2f94  omic.github.io/.
-00001970: 6807 5d94 6815 8c21 6874 7470 733a 2f2f  h.].h..!https://
-00001980: 6368 6961 6e74 692d 6174 6f6d 6963 2e67  chianti-atomic.g
-00001990: 6974 6875 622e 696f 2f94 8594 8194 7d94  ithub.io/.....}.
-000019a0: 2868 0568 0668 1a6a eb01 0000 7562 6168  (h.h.h.j....ubah
-000019b0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-000019c0: 6825 5d94 6827 5d94 8c06 7265 6675 7269  h%].h']...refuri
-000019d0: 946a ed01 0000 7568 296a c601 0000 681a  .j....uh)j....h.
-000019e0: 6ae2 0100 0075 6268 158c 0129 9485 9481  j....ubh...)....
-000019f0: 947d 9428 6805 6adb 0100 0068 1a6a e201  .}.(h.j....h.j..
-00001a00: 0000 6801 6803 681b 4e68 1c4e 7562 6568  ..h.h.h.Nh.Nubeh
-00001a10: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-00001a20: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
-00001a30: 2a68 1c4b 4268 1a6a 9e01 0000 6801 6803  *h.KBh.j....h.h.
-00001a40: 7562 683d 2981 947d 9428 6805 8c4e 616e  ubh=)..}.(h..Nan
-00001a50: 6420 6f6e 205b 5265 6164 5468 6544 6f63  d on [ReadTheDoc
-00001a60: 735d 2868 7474 7073 3a2f 2f63 6869 616e  s](https://chian
-00001a70: 7469 7079 2e72 6561 6474 6865 646f 6373  tipy.readthedocs
-00001a80: 2e69 6f2f 656e 2f6c 6174 6573 742f 3f62  .io/en/latest/?b
-00001a90: 6164 6765 3d6c 6174 6573 7429 9468 075d  adge=latest).h.]
-00001aa0: 9428 6815 8c15 616e 6420 6f6e 205b 5265  .(h...and on [Re
-00001ab0: 6164 5468 6544 6f63 735d 2894 8594 8194  adTheDocs](.....
-00001ac0: 7d94 2868 058c 1561 6e64 206f 6e20 5b52  }.(h...and on [R
-00001ad0: 6561 6454 6865 446f 6373 5d28 9468 1a6a  eadTheDocs](.h.j
-00001ae0: 0402 0000 6801 6803 681b 4e68 1c4e 7562  ....h.h.h.Nh.Nub
-00001af0: 6ac7 0100 0029 8194 7d94 2868 058c 3868  j....)..}.(h..8h
-00001b00: 7474 7073 3a2f 2f63 6869 616e 7469 7079  ttps://chiantipy
-00001b10: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00001b20: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-00001b30: 3d6c 6174 6573 7494 6807 5d94 6815 8c38  =latest.h.].h..8
-00001b40: 6874 7470 733a 2f2f 6368 6961 6e74 6970  https://chiantip
-00001b50: 792e 7265 6164 7468 6564 6f63 732e 696f  y.readthedocs.io
-00001b60: 2f65 6e2f 6c61 7465 7374 2f3f 6261 6467  /en/latest/?badg
-00001b70: 653d 6c61 7465 7374 9485 9481 947d 9428  e=latest.....}.(
-00001b80: 6805 6806 681a 6a0d 0200 0075 6261 681d  h.h.h.j....ubah.
-00001b90: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00001ba0: 255d 9468 275d 948c 0672 6566 7572 6994  %].h']...refuri.
-00001bb0: 6a0f 0200 0075 6829 6ac6 0100 0068 1a6a  j....uh)j....h.j
-00001bc0: 0402 0000 7562 6815 8c01 2994 8594 8194  ....ubh...).....
-00001bd0: 7d94 2868 056a db01 0000 681a 6a04 0200  }.(h.j....h.j...
-00001be0: 0068 0168 0368 1b4e 681c 4e75 6265 681d  .h.h.h.Nh.Nubeh.
-00001bf0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00001c00: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
-00001c10: 681c 4b44 681a 6a9e 0100 0068 0168 0375  h.KDh.j....h.h.u
-00001c20: 6265 681d 7d94 2868 1f5d 948c 5276 6572  beh.}.(h.]..Rver
-00001c30: 7369 6f6e 2d30 2d38 2d78 2d66 696c 6573  sion-0-8-x-files
-00001c40: 2d61 7265 2d6e 6563 6573 7361 7279 2d74  -are-necessary-t
-00001c50: 6f2d 7573 652d 7769 7468 2d74 6865 2d6e  o-use-with-the-n
-00001c60: 6577 2d63 6869 616e 7469 2d76 6572 7369  ew-chianti-versi
-00001c70: 6f6e 2d39 2d30 2d64 6174 6162 6173 6594  on-9-0-database.
-00001c80: 6168 215d 9468 235d 948c 5276 6572 7369  ah!].h#]..Rversi
-00001c90: 6f6e 2030 2e38 2e78 2066 696c 6573 2061  on 0.8.x files a
-00001ca0: 7265 206e 6563 6573 7361 7279 2074 6f20  re necessary to 
-00001cb0: 7573 6520 7769 7468 2074 6865 206e 6577  use with the new
-00001cc0: 2063 6869 616e 7469 2076 6572 7369 6f6e   chianti version
-00001cd0: 2039 2e30 2064 6174 6162 6173 6594 6168   9.0 database.ah
-00001ce0: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
-00001cf0: 6801 6803 681b 682a 681c 4b3c 7562 680a  h.h.h.h*h.K<ubh.
-00001d00: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
-00001d10: 0f29 8194 7d94 2868 058c 1b63 6861 6e67  .)..}.(h...chang
-00001d20: 6573 2066 726f 6d20 302e 372e 3120 746f  es from 0.7.1 to
-00001d30: 2030 2e38 2e30 9468 075d 9468 158c 1b63   0.8.0.h.].h...c
-00001d40: 6861 6e67 6573 2066 726f 6d20 302e 372e  hanges from 0.7.
-00001d50: 3120 746f 2030 2e38 2e30 9485 9481 947d  1 to 0.8.0.....}
-00001d60: 9428 6805 6a33 0200 0068 1a6a 3102 0000  .(h.j3...h.j1...
-00001d70: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
-00001d80: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00001d90: 5d94 6827 5d94 7568 2968 0e68 1a6a 2e02  ].h'].uh)h.h.j..
-00001da0: 0000 6801 6803 681b 682a 681c 4b48 7562  ..h.h.h.h*h.KHub
-00001db0: 683d 2981 947d 9428 6805 8c58 4368 6961  h=)..}.(h..XChia
-00001dc0: 6e74 6950 7920 6973 206e 6f77 206f 6e6c  ntiPy is now onl
-00001dd0: 7920 636f 6d70 6c69 616e 7420 7769 7468  y compliant with
-00001de0: 2050 7974 686f 6e20 332e 2020 4465 7665   Python 3.  Deve
-00001df0: 6c6f 706d 656e 7420 6973 2063 7572 7265  lopment is curre
-00001e00: 6e74 6c79 2077 6974 6820 5079 7468 6f6e  ntly with Python
-00001e10: 2033 2e36 9468 075d 9468 158c 5843 6869   3.6.h.].h..XChi
-00001e20: 616e 7469 5079 2069 7320 6e6f 7720 6f6e  antiPy is now on
-00001e30: 6c79 2063 6f6d 706c 6961 6e74 2077 6974  ly compliant wit
-00001e40: 6820 5079 7468 6f6e 2033 2e20 2044 6576  h Python 3.  Dev
-00001e50: 656c 6f70 6d65 6e74 2069 7320 6375 7272  elopment is curr
-00001e60: 656e 746c 7920 7769 7468 2050 7974 686f  ently with Pytho
-00001e70: 6e20 332e 3694 8594 8194 7d94 2868 056a  n 3.6.....}.(h.j
-00001e80: 4102 0000 681a 6a3f 0200 0068 0168 0368  A...h.j?...h.h.h
-00001e90: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
-00001ea0: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
-00001eb0: 9475 6829 683c 681b 682a 681c 4b4a 681a  .uh)h<h.h*h.KJh.
-00001ec0: 6a2e 0200 0068 0168 0375 6268 3d29 8194  j....h.h.ubh=)..
-00001ed0: 7d94 2868 058c 5354 6865 2075 7365 206f  }.(h..SThe use o
-00001ee0: 6620 7468 6520 5079 5174 3420 616e 6420  f the PyQt4 and 
-00001ef0: 5778 5769 6467 6574 7320 7061 636b 6167  WxWidgets packag
-00001f00: 6573 2068 6176 6520 6265 656e 2064 726f  es have been dro
-00001f10: 7070 6564 2061 6e64 2050 7951 7435 2069  pped and PyQt5 i
-00001f20: 7320 6e6f 7720 7573 6564 9468 075d 9468  s now used.h.].h
-00001f30: 158c 5354 6865 2075 7365 206f 6620 7468  ..SThe use of th
-00001f40: 6520 5079 5174 3420 616e 6420 5778 5769  e PyQt4 and WxWi
-00001f50: 6467 6574 7320 7061 636b 6167 6573 2068  dgets packages h
-00001f60: 6176 6520 6265 656e 2064 726f 7070 6564  ave been dropped
-00001f70: 2061 6e64 2050 7951 7435 2069 7320 6e6f   and PyQt5 is no
-00001f80: 7720 7573 6564 9485 9481 947d 9428 6805  w used.....}.(h.
-00001f90: 6a4f 0200 0068 1a6a 4d02 0000 6801 6803  jO...h.jM...h.h.
-00001fa0: 681b 4e68 1c4e 7562 6168 1d7d 9428 681f  h.Nh.Nubah.}.(h.
-00001fb0: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00001fc0: 5d94 7568 2968 3c68 1b68 2a68 1c4b 4c68  ].uh)h<h.h*h.KLh
-00001fd0: 1a6a 2e02 0000 6801 6803 7562 683d 2981  .j....h.h.ubh=).
-00001fe0: 947d 9428 6805 8c41 5468 6520 646f 6375  .}.(h..AThe docu
-00001ff0: 6d65 6e74 6174 696f 6e20 6973 206e 6f77  mentation is now
-00002000: 2061 7661 696c 6162 6c65 206f 6e20 6769   available on gi
-00002010: 7468 7562 2e69 6f5f 2061 6e64 2052 6561  thub.io_ and Rea
-00002020: 6454 6865 446f 6373 5f94 6807 5d94 2868  dTheDocs_.h.].(h
-00002030: 158c 2654 6865 2064 6f63 756d 656e 7461  ..&The documenta
-00002040: 7469 6f6e 2069 7320 6e6f 7720 6176 6169  tion is now avai
-00002050: 6c61 626c 6520 6f6e 2094 8594 8194 7d94  lable on .....}.
-00002060: 2868 058c 2654 6865 2064 6f63 756d 656e  (h..&The documen
-00002070: 7461 7469 6f6e 2069 7320 6e6f 7720 6176  tation is now av
-00002080: 6169 6c61 626c 6520 6f6e 2094 681a 6a5b  ailable on .h.j[
-00002090: 0200 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
-000020a0: c701 0000 2981 947d 9428 6805 8c0a 6769  ....)..}.(h...gi
-000020b0: 7468 7562 2e69 6f5f 9468 075d 9468 158c  thub.io_.h.].h..
-000020c0: 0967 6974 6875 622e 696f 9485 9481 947d  .github.io.....}
-000020d0: 9428 6805 6806 681a 6a64 0200 0075 6261  .(h.h.h.jd...uba
-000020e0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-000020f0: 9468 255d 9468 275d 948c 046e 616d 6594  .h%].h']...name.
-00002100: 8c09 6769 7468 7562 2e69 6f94 8c06 7265  ..github.io...re
-00002110: 6675 7269 948c 2168 7474 7073 3a2f 2f63  furi..!https://c
-00002120: 6869 616e 7469 2d61 746f 6d69 632e 6769  hianti-atomic.gi
-00002130: 7468 7562 2e69 6f2f 9475 6829 6ac6 0100  thub.io/.uh)j...
-00002140: 0068 1a6a 5b02 0000 8c08 7265 736f 6c76  .h.j[.....resolv
-00002150: 6564 944b 0175 6268 158c 0520 616e 6420  ed.K.ubh... and 
-00002160: 9485 9481 947d 9428 6805 8c05 2061 6e64  .....}.(h... and
-00002170: 2094 681a 6a5b 0200 0068 0168 0368 1b4e   .h.j[...h.h.h.N
-00002180: 681c 4e75 626a c701 0000 2981 947d 9428  h.Nubj....)..}.(
-00002190: 6805 8c0c 5265 6164 5468 6544 6f63 735f  h...ReadTheDocs_
-000021a0: 9468 075d 9468 158c 0b52 6561 6454 6865  .h.].h...ReadThe
-000021b0: 446f 6373 9485 9481 947d 9428 6805 6806  Docs.....}.(h.h.
-000021c0: 681a 6a7c 0200 0075 6261 681d 7d94 2868  h.j|...ubah.}.(h
-000021d0: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-000021e0: 275d 948c 046e 616d 6594 8c0b 5265 6164  ']...name...Read
-000021f0: 5468 6544 6f63 7394 6a74 0200 008c 3868  TheDocs.jt....8h
-00002200: 7474 7073 3a2f 2f63 6869 616e 7469 7079  ttps://chiantipy
-00002210: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00002220: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-00002230: 3d6c 6174 6573 7494 7568 296a c601 0000  =latest.uh)j....
-00002240: 681a 6a5b 0200 006a 7602 0000 4b01 7562  h.j[...jv...K.ub
-00002250: 6568 1d7d 9428 681f 5d94 6821 5d94 6823  eh.}.(h.].h!].h#
-00002260: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
-00002270: 1b68 2a68 1c4b 4e68 1a6a 2e02 0000 6801  .h*h.KNh.j....h.
-00002280: 6803 7562 6800 8c06 7461 7267 6574 9493  h.ubh...target..
-00002290: 9429 8194 7d94 2868 058c 312e 2e20 5f67  .)..}.(h..1.. _g
-000022a0: 6974 6875 622e 696f 3a20 2068 7474 7073  ithub.io:  https
-000022b0: 3a2f 2f63 6869 616e 7469 2d61 746f 6d69  ://chianti-atomi
-000022c0: 632e 6769 7468 7562 2e69 6f2f 9468 075d  c.github.io/.h.]
-000022d0: 9468 1d7d 9428 681f 5d94 8c09 6769 7468  .h.}.(h.]...gith
-000022e0: 7562 2d69 6f94 6168 215d 9468 235d 948c  ub-io.ah!].h#]..
-000022f0: 0967 6974 6875 622e 696f 9461 6825 5d94  .github.io.ah%].
-00002300: 6827 5d94 6a74 0200 006a 7502 0000 7568  h'].jt...ju...uh
-00002310: 296a 9302 0000 681c 4b50 681a 6a2e 0200  )j....h.KPh.j...
-00002320: 0068 0168 0368 1b68 2a6a 1e01 0000 4b01  .h.h.h.h*j....K.
-00002330: 7562 6a94 0200 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-00002340: 4a2e 2e20 5f52 6561 6454 6865 446f 6373  J.. _ReadTheDocs
-00002350: 3a20 2068 7474 7073 3a2f 2f63 6869 616e  :  https://chian
-00002360: 7469 7079 2e72 6561 6474 6865 646f 6373  tipy.readthedocs
-00002370: 2e69 6f2f 656e 2f6c 6174 6573 742f 3f62  .io/en/latest/?b
-00002380: 6164 6765 3d6c 6174 6573 7494 6807 5d94  adge=latest.h.].
-00002390: 681d 7d94 2868 1f5d 948c 0b72 6561 6474  h.}.(h.]...readt
-000023a0: 6865 646f 6373 9461 6821 5d94 6823 5d94  hedocs.ah!].h#].
-000023b0: 8c0b 7265 6164 7468 6564 6f63 7394 6168  ..readthedocs.ah
-000023c0: 255d 9468 275d 946a 7402 0000 6a8c 0200  %].h'].jt...j...
-000023d0: 0075 6829 6a93 0200 0068 1c4b 5268 1a6a  .uh)j....h.KRh.j
-000023e0: 2e02 0000 6801 6803 681b 682a 6a1e 0100  ....h.h.h.h*j...
-000023f0: 004b 0175 6265 681d 7d94 2868 1f5d 948c  .K.ubeh.}.(h.]..
-00002400: 1b63 6861 6e67 6573 2d66 726f 6d2d 302d  .changes-from-0-
-00002410: 372d 312d 746f 2d30 2d38 2d30 9461 6821  7-1-to-0-8-0.ah!
-00002420: 5d94 6823 5d94 8c1b 6368 616e 6765 7320  ].h#]...changes 
-00002430: 6672 6f6d 2030 2e37 2e31 2074 6f20 302e  from 0.7.1 to 0.
-00002440: 382e 3094 6168 255d 9468 275d 9475 6829  8.0.ah%].h'].uh)
-00002450: 6809 681a 680b 6801 6803 681b 682a 681c  h.h.h.h.h.h.h*h.
-00002460: 4b48 7562 680a 2981 947d 9428 6805 6806  KHubh.)..}.(h.h.
-00002470: 6807 5d94 2868 0f29 8194 7d94 2868 058c  h.].(h.)..}.(h..
-00002480: 1b63 6861 6e67 6573 2066 726f 6d20 302e  .changes from 0.
-00002490: 372e 3020 746f 2030 2e37 2e31 9468 075d  7.0 to 0.7.1.h.]
-000024a0: 9468 158c 1b63 6861 6e67 6573 2066 726f  .h...changes fro
-000024b0: 6d20 302e 372e 3020 746f 2030 2e37 2e31  m 0.7.0 to 0.7.1
-000024c0: 9485 9481 947d 9428 6805 6aba 0200 0068  .....}.(h.j....h
-000024d0: 1a6a b802 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-000024e0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-000024f0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-00002500: 0e68 1a6a b502 0000 6801 6803 681b 682a  .h.j....h.h.h.h*
-00002510: 681c 4b55 7562 683d 2981 947d 9428 6805  h.KUubh=)..}.(h.
-00002520: 8cb0 7665 7273 696f 6e20 302e 372e 3020  ..version 0.7.0 
-00002530: 696e 636c 7564 6564 2073 6f6d 6520 6368  included some ch
-00002540: 616e 6765 7320 696e 2074 6865 2043 6869  anges in the Chi
-00002550: 616e 7469 5079 206e 616d 696e 6720 636f  antiPy naming co
-00002560: 6e76 656e 7469 6f6e 732c 206c 6172 6765  nventions, large
-00002570: 6c79 2069 6e20 7468 6520 636f 6e74 696e  ly in the contin
-00002580: 7575 6d20 636c 6173 732e 2020 5468 6573  uum class.  Thes
-00002590: 6520 6172 6520 6265 696e 6720 7265 7665  e are being reve
-000025a0: 7274 6564 2074 6f20 7468 6520 6f72 6967  rted to the orig
-000025b0: 696e 616c 2043 6869 616e 7469 5079 206e  inal ChiantiPy n
-000025c0: 616d 696e 6720 636f 6e76 656e 7469 6f6e  aming convention
-000025d0: 732e 9468 075d 9468 158c b076 6572 7369  s..h.].h...versi
-000025e0: 6f6e 2030 2e37 2e30 2069 6e63 6c75 6465  on 0.7.0 include
-000025f0: 6420 736f 6d65 2063 6861 6e67 6573 2069  d some changes i
-00002600: 6e20 7468 6520 4368 6961 6e74 6950 7920  n the ChiantiPy 
-00002610: 6e61 6d69 6e67 2063 6f6e 7665 6e74 696f  naming conventio
-00002620: 6e73 2c20 6c61 7267 656c 7920 696e 2074  ns, largely in t
-00002630: 6865 2063 6f6e 7469 6e75 756d 2063 6c61  he continuum cla
-00002640: 7373 2e20 2054 6865 7365 2061 7265 2062  ss.  These are b
-00002650: 6569 6e67 2072 6576 6572 7465 6420 746f  eing reverted to
-00002660: 2074 6865 206f 7269 6769 6e61 6c20 4368   the original Ch
-00002670: 6961 6e74 6950 7920 6e61 6d69 6e67 2063  iantiPy naming c
-00002680: 6f6e 7665 6e74 696f 6e73 2e94 8594 8194  onventions......
-00002690: 7d94 2868 056a c802 0000 681a 6ac6 0200  }.(h.j....h.j...
-000026a0: 0068 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
-000026b0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-000026c0: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
-000026d0: 681c 4b57 681a 6ab5 0200 0068 0168 0375  h.KWh.j....h.h.u
-000026e0: 6268 3d29 8194 7d94 2868 058c 6474 6865  bh=)..}.(h..dthe
-000026f0: 2069 6f6e 2e66 7265 6542 6f75 6e64 7878   ion.freeBoundxx
-00002700: 7820 6d65 7468 6f64 7320 6861 7665 2062  x methods have b
-00002710: 6565 6e20 6669 7865 6420 616e 6420 7468  een fixed and th
-00002720: 6973 2061 6c73 6f20 6669 7865 7320 7468  is also fixes th
-00002730: 6520 7072 6f62 6c65 6d20 7769 7468 2074  e problem with t
-00002740: 6865 2052 6164 4c6f 7373 2063 6c61 7373  he RadLoss class
-00002750: 2e94 6807 5d94 6815 8c64 7468 6520 696f  ..h.].h..dthe io
-00002760: 6e2e 6672 6565 426f 756e 6478 7878 206d  n.freeBoundxxx m
-00002770: 6574 686f 6473 2068 6176 6520 6265 656e  ethods have been
-00002780: 2066 6978 6564 2061 6e64 2074 6869 7320   fixed and this 
-00002790: 616c 736f 2066 6978 6573 2074 6865 2070  also fixes the p
-000027a0: 726f 626c 656d 2077 6974 6820 7468 6520  roblem with the 
-000027b0: 5261 644c 6f73 7320 636c 6173 732e 9485  RadLoss class...
-000027c0: 9481 947d 9428 6805 6ad6 0200 0068 1a6a  ...}.(h.j....h.j
-000027d0: d402 0000 6801 6803 681b 4e68 1c4e 7562  ....h.h.h.Nh.Nub
-000027e0: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-000027f0: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
-00002800: 1b68 2a68 1c4b 5968 1a6a b502 0000 6801  .h*h.KYh.j....h.
-00002810: 6803 7562 683d 2981 947d 9428 6805 8c35  h.ubh=)..}.(h..5
-00002820: 6120 7073 6575 646f 2d76 6f69 6774 2066  a pseudo-voigt f
-00002830: 696c 7465 7220 6861 7320 6265 656e 2061  ilter has been a
-00002840: 6464 6564 2074 6f20 746f 6f6c 732e 6669  dded to tools.fi
-00002850: 6c74 6572 7394 6807 5d94 6815 8c35 6120  lters.h.].h..5a 
-00002860: 7073 6575 646f 2d76 6f69 6774 2066 696c  pseudo-voigt fil
-00002870: 7465 7220 6861 7320 6265 656e 2061 6464  ter has been add
-00002880: 6564 2074 6f20 746f 6f6c 732e 6669 6c74  ed to tools.filt
-00002890: 6572 7394 8594 8194 7d94 2868 056a e402  ers.....}.(h.j..
-000028a0: 0000 681a 6ae2 0200 0068 0168 0368 1b4e  ..h.j....h.h.h.N
-000028b0: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
-000028c0: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
-000028d0: 6829 683c 681b 682a 681c 4b5b 681a 6ab5  h)h<h.h*h.K[h.j.
-000028e0: 0200 0068 0168 0375 6268 3d29 8194 7d94  ...h.h.ubh=)..}.
-000028f0: 2868 058c 5b74 6865 206b 6579 776f 7264  (h..[the keyword
-00002900: 2061 7267 756d 656e 7420 7776 6c52 616e   argument wvlRan
-00002910: 6765 2068 6173 2062 6565 6e20 7265 6d6f  ge has been remo
-00002920: 7665 6420 6672 6f6d 2074 6865 2069 6f6e  ved from the ion
-00002930: 2e65 6d69 7373 2061 6e64 2069 6f6e 2e69  .emiss and ion.i
-00002940: 6e74 656e 7369 7479 206d 6574 686f 6473  ntensity methods
-00002950: 9468 075d 9468 158c 5b74 6865 206b 6579  .h.].h..[the key
-00002960: 776f 7264 2061 7267 756d 656e 7420 7776  word argument wv
-00002970: 6c52 616e 6765 2068 6173 2062 6565 6e20  lRange has been 
-00002980: 7265 6d6f 7665 6420 6672 6f6d 2074 6865  removed from the
-00002990: 2069 6f6e 2e65 6d69 7373 2061 6e64 2069   ion.emiss and i
-000029a0: 6f6e 2e69 6e74 656e 7369 7479 206d 6574  on.intensity met
-000029b0: 686f 6473 9485 9481 947d 9428 6805 6af2  hods.....}.(h.j.
-000029c0: 0200 0068 1a6a f002 0000 6801 6803 681b  ...h.j....h.h.h.
-000029d0: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
-000029e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000029f0: 7568 2968 3c68 1b68 2a68 1c4b 5d68 1a6a  uh)h<h.h*h.K]h.j
-00002a00: b502 0000 6801 6803 7562 683d 2981 947d  ....h.h.ubh=)..}
-00002a10: 9428 6805 8cbd 7468 6520 6b65 7977 6f72  .(h...the keywor
-00002a20: 6420 6172 6775 6d65 6e74 2066 6f72 2074  d argument for t
-00002a30: 6865 2045 6d69 7373 696f 6e20 4d65 6173  he Emission Meas
-00002a40: 7572 652c 2065 6d2c 2068 6173 2062 6565  ure, em, has bee
-00002a50: 6e20 7265 6d6f 7665 6420 6672 6f6d 2074  n removed from t
-00002a60: 6865 2069 6f6e 2e69 6e74 656e 7369 7479  he ion.intensity
-00002a70: 2061 6e64 2073 696d 696c 6172 206d 6574   and similar met
-00002a80: 686f 6473 2e20 2049 7420 6973 206e 6f77  hods.  It is now
-00002a90: 206e 6563 6573 7361 7279 2074 6f20 7370   necessary to sp
-00002aa0: 6563 6966 790a 7468 6520 656d 6973 7369  ecify.the emissi
-00002ab0: 6f6e 2077 6865 6e20 7468 6520 6f62 6a65  on when the obje
-00002ac0: 6374 2069 7320 696e 7374 616e 7469 6174  ct is instantiat
-00002ad0: 6564 2e94 6807 5d94 6815 8cbd 7468 6520  ed..h.].h...the 
-00002ae0: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-00002af0: 2066 6f72 2074 6865 2045 6d69 7373 696f   for the Emissio
-00002b00: 6e20 4d65 6173 7572 652c 2065 6d2c 2068  n Measure, em, h
-00002b10: 6173 2062 6565 6e20 7265 6d6f 7665 6420  as been removed 
-00002b20: 6672 6f6d 2074 6865 2069 6f6e 2e69 6e74  from the ion.int
-00002b30: 656e 7369 7479 2061 6e64 2073 696d 696c  ensity and simil
-00002b40: 6172 206d 6574 686f 6473 2e20 2049 7420  ar methods.  It 
-00002b50: 6973 206e 6f77 206e 6563 6573 7361 7279  is now necessary
-00002b60: 2074 6f20 7370 6563 6966 790a 7468 6520   to specify.the 
-00002b70: 656d 6973 7369 6f6e 2077 6865 6e20 7468  emission when th
-00002b80: 6520 6f62 6a65 6374 2069 7320 696e 7374  e object is inst
-00002b90: 616e 7469 6174 6564 2e94 8594 8194 7d94  antiated......}.
-00002ba0: 2868 056a 0003 0000 681a 6afe 0200 0068  (h.j....h.j....h
-00002bb0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
-00002bc0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-00002bd0: 9468 275d 9475 6829 683c 681b 682a 681c  .h'].uh)h<h.h*h.
-00002be0: 4b5f 681a 6ab5 0200 0068 0168 0375 6268  K_h.j....h.h.ubh
-00002bf0: 3d29 8194 7d94 2868 058c 4d61 2073 6574  =)..}.(h..Ma set
-00002c00: 206f 6620 5079 5174 3520 6469 616c 6f67   of PyQt5 dialog
-00002c10: 7320 6861 7665 2062 6565 6e20 6465 7665  s have been deve
-00002c20: 6c6f 7065 6420 6279 202a 2a6b 7472 6974  loped by **ktrit
-00002c30: 7a2a 2a20 616e 6420 6172 6520 6e6f 7720  z** and are now 
-00002c40: 696e 636c 7564 6564 9468 075d 9428 6815  included.h.].(h.
-00002c50: 8c2e 6120 7365 7420 6f66 2050 7951 7435  ..a set of PyQt5
-00002c60: 2064 6961 6c6f 6773 2068 6176 6520 6265   dialogs have be
-00002c70: 656e 2064 6576 656c 6f70 6564 2062 7920  en developed by 
-00002c80: 9485 9481 947d 9428 6805 8c2e 6120 7365  .....}.(h...a se
-00002c90: 7420 6f66 2050 7951 7435 2064 6961 6c6f  t of PyQt5 dialo
-00002ca0: 6773 2068 6176 6520 6265 656e 2064 6576  gs have been dev
-00002cb0: 656c 6f70 6564 2062 7920 9468 1a6a 0c03  eloped by .h.j..
-00002cc0: 0000 6801 6803 681b 4e68 1c4e 7562 6800  ..h.h.h.Nh.Nubh.
-00002cd0: 8c06 7374 726f 6e67 9493 9429 8194 7d94  ..strong...)..}.
-00002ce0: 2868 058c 0a2a 2a6b 7472 6974 7a2a 2a94  (h...**ktritz**.
-00002cf0: 6807 5d94 6815 8c06 6b74 7269 747a 9485  h.].h...ktritz..
-00002d00: 9481 947d 9428 6805 6806 681a 6a17 0300  ...}.(h.h.h.j...
-00002d10: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
-00002d20: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-00002d30: 6a15 0300 0068 1a6a 0c03 0000 7562 6815  j....h.j....ubh.
-00002d40: 8c15 2061 6e64 2061 7265 206e 6f77 2069  .. and are now i
-00002d50: 6e63 6c75 6465 6494 8594 8194 7d94 2868  ncluded.....}.(h
-00002d60: 058c 1520 616e 6420 6172 6520 6e6f 7720  ... and are now 
-00002d70: 696e 636c 7564 6564 9468 1a6a 0c03 0000  included.h.j....
-00002d80: 6801 6803 681b 4e68 1c4e 7562 6568 1d7d  h.h.h.Nh.Nubeh.}
-00002d90: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00002da0: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
-00002db0: 1c4b 6268 1a6a b502 0000 6801 6803 7562  .Kbh.j....h.h.ub
-00002dc0: 683d 2981 947d 9428 6805 8c46 7468 6973  h=)..}.(h..Fthis
-00002dd0: 2069 7320 7468 6520 6c61 7374 2072 656c   is the last rel
-00002de0: 6561 7365 2074 6861 7420 7769 6c6c 2075  ease that will u
-00002df0: 7365 2074 6865 2050 7951 7434 2077 6964  se the PyQt4 wid
-00002e00: 6765 7473 2061 7320 616e 206f 7074 696f  gets as an optio
-00002e10: 6e2e 9468 075d 9468 158c 4674 6869 7320  n..h.].h..Fthis 
-00002e20: 6973 2074 6865 206c 6173 7420 7265 6c65  is the last rele
-00002e30: 6173 6520 7468 6174 2077 696c 6c20 7573  ase that will us
-00002e40: 6520 7468 6520 5079 5174 3420 7769 6467  e the PyQt4 widg
-00002e50: 6574 7320 6173 2061 6e20 6f70 7469 6f6e  ets as an option
-00002e60: 2e94 8594 8194 7d94 2868 056a 3203 0000  ......}.(h.j2...
-00002e70: 681a 6a30 0300 0068 0168 0368 1b4e 681c  h.j0...h.h.h.Nh.
-00002e80: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
-00002e90: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-00002ea0: 683c 681b 682a 681c 4b64 681a 6ab5 0200  h<h.h*h.Kdh.j...
-00002eb0: 0068 0168 0375 6268 3d29 8194 7d94 2868  .h.h.ubh=)..}.(h
-00002ec0: 058c 8f74 6865 206d 6574 686f 6420 2a2a  ...the method **
-00002ed0: 696f 6e65 714f 6e65 2a2a 2069 7320 7573  ioneqOne** is us
-00002ee0: 6564 2062 7920 626f 7468 2074 6865 2049  ed by both the I
-00002ef0: 6f6e 2061 6e64 2043 6f6e 7469 6e75 756d  on and Continuum
-00002f00: 2063 6c61 7373 2e20 2049 7420 6861 7320   class.  It has 
-00002f10: 6265 656e 206d 6f76 6564 2074 6f20 6120  been moved to a 
-00002f20: 7369 6e67 6c65 205f 496f 6e65 714f 6e65  single _IoneqOne
-00002f30: 2e70 7920 6669 6c65 2069 6e20 7468 6520  .py file in the 
-00002f40: 2a2a 6261 7365 2a2a 2064 6972 6563 746f  **base** directo
-00002f50: 7279 9468 075d 9428 6815 8c0b 7468 6520  ry.h.].(h...the 
-00002f60: 6d65 7468 6f64 2094 8594 8194 7d94 2868  method .....}.(h
-00002f70: 058c 0b74 6865 206d 6574 686f 6420 9468  ...the method .h
-00002f80: 1a6a 3e03 0000 6801 6803 681b 4e68 1c4e  .j>...h.h.h.Nh.N
-00002f90: 7562 6a16 0300 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-00002fa0: 0c2a 2a69 6f6e 6571 4f6e 652a 2a94 6807  .**ioneqOne**.h.
-00002fb0: 5d94 6815 8c08 696f 6e65 714f 6e65 9485  ].h...ioneqOne..
-00002fc0: 9481 947d 9428 6805 6806 681a 6a47 0300  ...}.(h.h.h.jG..
-00002fd0: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
-00002fe0: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-00002ff0: 6a15 0300 0068 1a6a 3e03 0000 7562 6815  j....h.j>...ubh.
-00003000: 8c66 2069 7320 7573 6564 2062 7920 626f  .f is used by bo
-00003010: 7468 2074 6865 2049 6f6e 2061 6e64 2043  th the Ion and C
-00003020: 6f6e 7469 6e75 756d 2063 6c61 7373 2e20  ontinuum class. 
-00003030: 2049 7420 6861 7320 6265 656e 206d 6f76   It has been mov
-00003040: 6564 2074 6f20 6120 7369 6e67 6c65 205f  ed to a single _
-00003050: 496f 6e65 714f 6e65 2e70 7920 6669 6c65  IoneqOne.py file
-00003060: 2069 6e20 7468 6520 9485 9481 947d 9428   in the .....}.(
-00003070: 6805 8c66 2069 7320 7573 6564 2062 7920  h..f is used by 
-00003080: 626f 7468 2074 6865 2049 6f6e 2061 6e64  both the Ion and
-00003090: 2043 6f6e 7469 6e75 756d 2063 6c61 7373   Continuum class
-000030a0: 2e20 2049 7420 6861 7320 6265 656e 206d  .  It has been m
-000030b0: 6f76 6564 2074 6f20 6120 7369 6e67 6c65  oved to a single
-000030c0: 205f 496f 6e65 714f 6e65 2e70 7920 6669   _IoneqOne.py fi
-000030d0: 6c65 2069 6e20 7468 6520 9468 1a6a 3e03  le in the .h.j>.
-000030e0: 0000 6801 6803 681b 4e68 1c4e 7562 6a16  ..h.h.h.Nh.Nubj.
-000030f0: 0300 0029 8194 7d94 2868 058c 082a 2a62  ...)..}.(h...**b
-00003100: 6173 652a 2a94 6807 5d94 6815 8c04 6261  ase**.h.].h...ba
-00003110: 7365 9485 9481 947d 9428 6805 6806 681a  se.....}.(h.h.h.
-00003120: 6a5a 0300 0075 6261 681d 7d94 2868 1f5d  jZ...ubah.}.(h.]
-00003130: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
-00003140: 9475 6829 6a15 0300 0068 1a6a 3e03 0000  .uh)j....h.j>...
-00003150: 7562 6815 8c0a 2064 6972 6563 746f 7279  ubh... directory
-00003160: 9485 9481 947d 9428 6805 8c0a 2064 6972  .....}.(h... dir
-00003170: 6563 746f 7279 9468 1a6a 3e03 0000 6801  ectory.h.j>...h.
-00003180: 6803 681b 4e68 1c4e 7562 6568 1d7d 9428  h.h.Nh.Nubeh.}.(
-00003190: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
-000031a0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
-000031b0: 6668 1a6a b502 0000 6801 6803 7562 6568  fh.j....h.h.ubeh
-000031c0: 1d7d 9428 681f 5d94 8c1b 6368 616e 6765  .}.(h.]...change
-000031d0: 732d 6672 6f6d 2d30 2d37 2d30 2d74 6f2d  s-from-0-7-0-to-
-000031e0: 302d 372d 3194 6168 215d 9468 235d 948c  0-7-1.ah!].h#]..
-000031f0: 1b63 6861 6e67 6573 2066 726f 6d20 302e  .changes from 0.
-00003200: 372e 3020 746f 2030 2e37 2e31 9461 6825  7.0 to 0.7.1.ah%
-00003210: 5d94 6827 5d94 7568 2968 0968 1a68 0b68  ].h'].uh)h.h.h.h
-00003220: 0168 0368 1b68 2a68 1c4b 5575 6268 0a29  .h.h.h*h.KUubh.)
-00003230: 8194 7d94 2868 0568 0668 075d 9428 680f  ..}.(h.h.h.].(h.
-00003240: 2981 947d 9428 6805 8c1b 6368 616e 6765  )..}.(h...change
-00003250: 7320 6672 6f6d 2030 2e36 2e35 2074 6f20  s from 0.6.5 to 
-00003260: 302e 372e 3094 6807 5d94 6815 8c1b 6368  0.7.0.h.].h...ch
-00003270: 616e 6765 7320 6672 6f6d 2030 2e36 2e35  anges from 0.6.5
-00003280: 2074 6f20 302e 372e 3094 8594 8194 7d94   to 0.7.0.....}.
-00003290: 2868 056a 8003 0000 681a 6a7e 0300 0068  (h.j....h.j~...h
-000032a0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
-000032b0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-000032c0: 9468 275d 9475 6829 680e 681a 6a7b 0300  .h'].uh)h.h.j{..
-000032d0: 0068 0168 0368 1b68 2a68 1c4b 6a75 6268  .h.h.h.h*h.Kjubh
-000032e0: 3d29 8194 7d94 2868 058c 4754 6865 2070  =)..}.(h..GThe p
-000032f0: 7269 6d61 7279 2063 6861 6e67 6520 6973  rimary change is
-00003300: 2074 6861 7420 636f 6465 2064 6576 656c   that code devel
-00003310: 6f70 656d 656e 7420 6861 7320 6265 656e  opement has been
-00003320: 206d 6f76 6564 2074 6f20 4769 7468 7562   moved to Github
-00003330: 5f2e 9468 075d 9428 6815 8c3f 5468 6520  _..h.].(h..?The 
-00003340: 7072 696d 6172 7920 6368 616e 6765 2069  primary change i
-00003350: 7320 7468 6174 2063 6f64 6520 6465 7665  s that code deve
-00003360: 6c6f 7065 6d65 6e74 2068 6173 2062 6565  lopement has bee
-00003370: 6e20 6d6f 7665 6420 746f 2094 8594 8194  n moved to .....
-00003380: 7d94 2868 058c 3f54 6865 2070 7269 6d61  }.(h..?The prima
-00003390: 7279 2063 6861 6e67 6520 6973 2074 6861  ry change is tha
-000033a0: 7420 636f 6465 2064 6576 656c 6f70 656d  t code developem
-000033b0: 656e 7420 6861 7320 6265 656e 206d 6f76  ent has been mov
-000033c0: 6564 2074 6f20 9468 1a6a 8c03 0000 6801  ed to .h.j....h.
-000033d0: 6803 681b 4e68 1c4e 7562 6ac7 0100 0029  h.h.Nh.Nubj....)
-000033e0: 8194 7d94 2868 058c 0747 6974 6875 625f  ..}.(h...Github_
-000033f0: 9468 075d 9468 158c 0647 6974 6875 6294  .h.].h...Github.
-00003400: 8594 8194 7d94 2868 0568 0668 1a6a 9503  ....}.(h.h.h.j..
-00003410: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-00003420: 5d94 6823 5d94 6825 5d94 6827 5d94 8c04  ].h#].h%].h']...
-00003430: 6e61 6d65 948c 0647 6974 6875 6294 6a74  name...Github.jt
-00003440: 0200 008c 2b68 7474 7073 3a2f 2f67 6974  ....+https://git
-00003450: 6875 622e 636f 6d2f 6368 6961 6e74 692d  hub.com/chianti-
-00003460: 6174 6f6d 6963 2f43 6869 616e 7469 5079  atomic/ChiantiPy
-00003470: 9475 6829 6ac6 0100 0068 1a6a 8c03 0000  .uh)j....h.j....
-00003480: 6a76 0200 004b 0175 6268 158c 012e 9485  jv...K.ubh......
-00003490: 9481 947d 9428 6805 8c01 2e94 681a 6a8c  ...}.(h.....h.j.
-000034a0: 0300 0068 0168 0368 1b4e 681c 4e75 6265  ...h.h.h.Nh.Nube
-000034b0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-000034c0: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
-000034d0: 682a 681c 4b6c 681a 6a7b 0300 0068 0168  h*h.Klh.j{...h.h
-000034e0: 0375 626a 9402 0000 2981 947d 9428 6805  .ubj....)..}.(h.
-000034f0: 8c38 2e2e 205f 4769 7468 7562 3a20 2068  .8.. _Github:  h
-00003500: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003510: 6d2f 6368 6961 6e74 692d 6174 6f6d 6963  m/chianti-atomic
-00003520: 2f43 6869 616e 7469 5079 9468 075d 9468  /ChiantiPy.h.].h
-00003530: 1d7d 9428 681f 5d94 8c06 6769 7468 7562  .}.(h.]...github
-00003540: 9461 6821 5d94 6823 5d94 8c06 6769 7468  .ah!].h#]...gith
-00003550: 7562 9461 6825 5d94 6827 5d94 6a74 0200  ub.ah%].h'].jt..
-00003560: 006a a503 0000 7568 296a 9302 0000 681c  .j....uh)j....h.
-00003570: 4b6e 681a 6a7b 0300 0068 0168 0368 1b68  Knh.j{...h.h.h.h
-00003580: 2a6a 1e01 0000 4b01 7562 683d 2981 947d  *j....K.ubh=)..}
-00003590: 9428 6805 8c98 416c 736f 2c20 696e 206f  .(h...Also, in o
-000035a0: 7264 6572 2074 6f20 6265 206d 6f72 6520  rder to be more 
-000035b0: 636f 6d70 6c69 616e 7420 7769 7468 206f  compliant with o
-000035c0: 7468 6572 2061 7374 726f 7068 7973 6963  ther astrophysic
-000035d0: 616c 2070 6163 6b61 6765 7320 6f6e 2047  al packages on G
-000035e0: 6974 6875 6220 2841 7374 726f 7079 5f20  ithub (Astropy_ 
-000035f0: 616e 6420 5375 6e50 795f 2920 7468 6520  and SunPy_) the 
-00003600: 6469 7265 6374 6f72 7920 6c61 796f 7574  directory layout
-00003610: 2068 6173 2062 6565 6e20 6368 616e 6765   has been change
-00003620: 6420 616e 6420 7265 6e61 6d65 642e 9468  d and renamed..h
-00003630: 075d 9428 6815 8c51 416c 736f 2c20 696e  .].(h..QAlso, in
-00003640: 206f 7264 6572 2074 6f20 6265 206d 6f72   order to be mor
-00003650: 6520 636f 6d70 6c69 616e 7420 7769 7468  e compliant with
-00003660: 206f 7468 6572 2061 7374 726f 7068 7973   other astrophys
-00003670: 6963 616c 2070 6163 6b61 6765 7320 6f6e  ical packages on
-00003680: 2047 6974 6875 6220 2894 8594 8194 7d94   Github (.....}.
-00003690: 2868 058c 5141 6c73 6f2c 2069 6e20 6f72  (h..QAlso, in or
-000036a0: 6465 7220 746f 2062 6520 6d6f 7265 2063  der to be more c
-000036b0: 6f6d 706c 6961 6e74 2077 6974 6820 6f74  ompliant with ot
-000036c0: 6865 7220 6173 7472 6f70 6879 7369 6361  her astrophysica
-000036d0: 6c20 7061 636b 6167 6573 206f 6e20 4769  l packages on Gi
-000036e0: 7468 7562 2028 9468 1a6a bd03 0000 6801  thub (.h.j....h.
-000036f0: 6803 681b 4e68 1c4e 7562 6ac7 0100 0029  h.h.Nh.Nubj....)
-00003700: 8194 7d94 2868 058c 0841 7374 726f 7079  ..}.(h...Astropy
-00003710: 5f94 6807 5d94 6815 8c07 4173 7472 6f70  _.h.].h...Astrop
-00003720: 7994 8594 8194 7d94 2868 0568 0668 1a6a  y.....}.(h.h.h.j
-00003730: c603 0000 7562 6168 1d7d 9428 681f 5d94  ....ubah.}.(h.].
-00003740: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00003750: 8c04 6e61 6d65 948c 0741 7374 726f 7079  ..name...Astropy
-00003760: 946a 7402 0000 8c18 6874 7470 732f 6769  .jt.....https/gi
-00003770: 7468 7562 2e63 6f6d 2f61 7374 726f 7079  thub.com/astropy
-00003780: 9475 6829 6ac6 0100 0068 1a6a bd03 0000  .uh)j....h.j....
-00003790: 6a76 0200 004b 0175 6268 158c 0520 616e  jv...K.ubh... an
-000037a0: 6420 9485 9481 947d 9428 6805 8c05 2061  d .....}.(h... a
-000037b0: 6e64 2094 681a 6abd 0300 0068 0168 0368  nd .h.j....h.h.h
-000037c0: 1b4e 681c 4e75 626a c701 0000 2981 947d  .Nh.Nubj....)..}
-000037d0: 9428 6805 8c06 5375 6e50 795f 9468 075d  .(h...SunPy_.h.]
-000037e0: 9468 158c 0553 756e 5079 9485 9481 947d  .h...SunPy.....}
-000037f0: 9428 6805 6806 681a 6adc 0300 0075 6261  .(h.h.h.j....uba
-00003800: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-00003810: 9468 255d 9468 275d 948c 046e 616d 6594  .h%].h']...name.
-00003820: 8c05 5375 6e50 7994 6a74 0200 008c 1e68  ..SunPy.jt.....h
-00003830: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003840: 6d2f 7375 6e70 792f 7375 6e70 7994 7568  m/sunpy/sunpy.uh
-00003850: 296a c601 0000 681a 6abd 0300 006a 7602  )j....h.j....jv.
-00003860: 0000 4b01 7562 6815 8c34 2920 7468 6520  ..K.ubh..4) the 
-00003870: 6469 7265 6374 6f72 7920 6c61 796f 7574  directory layout
-00003880: 2068 6173 2062 6565 6e20 6368 616e 6765   has been change
-00003890: 6420 616e 6420 7265 6e61 6d65 642e 9485  d and renamed...
-000038a0: 9481 947d 9428 6805 8c34 2920 7468 6520  ...}.(h..4) the 
-000038b0: 6469 7265 6374 6f72 7920 6c61 796f 7574  directory layout
-000038c0: 2068 6173 2062 6565 6e20 6368 616e 6765   has been change
-000038d0: 6420 616e 6420 7265 6e61 6d65 642e 9468  d and renamed..h
-000038e0: 1a6a bd03 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-000038f0: 7562 6568 1d7d 9428 681f 5d94 6821 5d94  ubeh.}.(h.].h!].
-00003900: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-00003910: 3c68 1b68 2a68 1c4b 7068 1a6a 7b03 0000  <h.h*h.Kph.j{...
-00003920: 6801 6803 7562 6a94 0200 0029 8194 7d94  h.h.ubj....)..}.
-00003930: 2868 058c 262e 2e20 5f41 7374 726f 7079  (h..&.. _Astropy
-00003940: 3a20 2068 7474 7073 2f67 6974 6875 622e  :  https/github.
-00003950: 636f 6d2f 6173 7472 6f70 7994 6807 5d94  com/astropy.h.].
-00003960: 681d 7d94 2868 1f5d 948c 0761 7374 726f  h.}.(h.]...astro
-00003970: 7079 9461 6821 5d94 6823 5d94 8c07 6173  py.ah!].h#]...as
-00003980: 7472 6f70 7994 6168 255d 9468 275d 946a  tropy.ah%].h'].j
-00003990: 7402 0000 6ad6 0300 0075 6829 6a93 0200  t...j....uh)j...
-000039a0: 0068 1c4b 7368 1a6a 7b03 0000 6801 6803  .h.Ksh.j{...h.h.
-000039b0: 681b 682a 6a1e 0100 004b 0175 626a 9402  h.h*j....K.ubj..
-000039c0: 0000 2981 947d 9428 6805 8c2a 2e2e 205f  ..)..}.(h..*.. _
-000039d0: 5375 6e50 793a 2020 6874 7470 733a 2f2f  SunPy:  https://
-000039e0: 6769 7468 7562 2e63 6f6d 2f73 756e 7079  github.com/sunpy
-000039f0: 2f73 756e 7079 9468 075d 9468 1d7d 9428  /sunpy.h.].h.}.(
-00003a00: 681f 5d94 8c05 7375 6e70 7994 6168 215d  h.]...sunpy.ah!]
-00003a10: 9468 235d 948c 0573 756e 7079 9461 6825  .h#]...sunpy.ah%
-00003a20: 5d94 6827 5d94 6a74 0200 006a ec03 0000  ].h'].jt...j....
-00003a30: 7568 296a 9302 0000 681c 4b74 681a 6a7b  uh)j....h.Kth.j{
-00003a40: 0300 0068 0168 0368 1b68 2a6a 1e01 0000  ...h.h.h.h*j....
-00003a50: 4b01 7562 683d 2981 947d 9428 6805 8c25  K.ubh=)..}.(h..%
-00003a60: 5468 6520 636f 7265 2072 6f75 7469 6e65  The core routine
-00003a70: 7320 6172 6520 6e6f 7720 696d 706f 7274  s are now import
-00003a80: 6564 2061 7394 6807 5d94 6815 8c25 5468  ed as.h.].h..%Th
-00003a90: 6520 636f 7265 2072 6f75 7469 6e65 7320  e core routines 
-00003aa0: 6172 6520 6e6f 7720 696d 706f 7274 6564  are now imported
-00003ab0: 2061 7394 8594 8194 7d94 2868 056a 1204   as.....}.(h.j..
-00003ac0: 0000 681a 6a10 0400 0068 0168 0368 1b4e  ..h.j....h.h.h.N
-00003ad0: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
-00003ae0: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
-00003af0: 6829 683c 681b 682a 681c 4b76 681a 6a7b  h)h<h.h*h.Kvh.j{
-00003b00: 0300 0068 0168 0375 6268 4d29 8194 7d94  ...h.h.ubhM)..}.
-00003b10: 2868 058c 1b69 6d70 6f72 7420 4368 6961  (h...import Chia
-00003b20: 6e74 6950 792e 636f 7265 2061 7320 6368  ntiPy.core as ch
-00003b30: 9468 075d 9468 158c 1b69 6d70 6f72 7420  .h.].h...import 
-00003b40: 4368 6961 6e74 6950 792e 636f 7265 2061  ChiantiPy.core a
-00003b50: 7320 6368 9485 9481 947d 9428 6805 6806  s ch.....}.(h.h.
-00003b60: 681a 6a1e 0400 0075 6261 681d 7d94 2868  h.j....ubah.}.(h
-00003b70: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-00003b80: 275d 9468 5c68 5d75 6829 684c 681c 4b7a  '].h\h]uh)hLh.Kz
-00003b90: 681a 6a7b 0300 0068 0168 0368 1b68 2a75  h.j{...h.h.h.h*u
-00003ba0: 6268 3d29 8194 7d94 2868 058c 2d74 6869  bh=)..}.(h..-thi
-00003bb0: 7320 6769 7665 2061 6363 6573 7320 746f  s give access to
-00003bc0: 2063 682e 696f 6e2c 2063 682e 7370 6563   ch.ion, ch.spec
-00003bd0: 7472 756d 2c20 6574 632e 9468 075d 9468  trum, etc..h.].h
-00003be0: 158c 2d74 6869 7320 6769 7665 2061 6363  ..-this give acc
-00003bf0: 6573 7320 746f 2063 682e 696f 6e2c 2063  ess to ch.ion, c
-00003c00: 682e 7370 6563 7472 756d 2c20 6574 632e  h.spectrum, etc.
-00003c10: 9485 9481 947d 9428 6805 6a2e 0400 0068  .....}.(h.j....h
-00003c20: 1a6a 2c04 0000 6801 6803 681b 4e68 1c4e  .j,...h.h.h.Nh.N
-00003c30: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-00003c40: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-00003c50: 3c68 1b68 2a68 1c4b 7c68 1a6a 7b03 0000  <h.h*h.K|h.j{...
-00003c60: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
-00003c70: 8c96 496e 2074 6572 6d73 206f 6620 6275  ..In terms of bu
-00003c80: 672d 6669 7865 732c 2074 6865 2063 616c  g-fixes, the cal
-00003c90: 6375 6c61 7469 6f6e 206f 6620 6578 6369  culation of exci
-00003ca0: 7461 7469 6f6e 2d61 7574 6f69 6f6e 697a  tation-autoioniz
-00003cb0: 6174 696f 6e20 6372 6f73 732d 7365 6374  ation cross-sect
-00003cc0: 696f 6e73 2061 6e64 2072 6174 6573 2068  ions and rates h
-00003cd0: 6176 6520 6265 656e 2063 6f72 7265 6374  ave been correct
-00003ce0: 6564 2069 6e20 7468 6520 6561 4372 6f73  ed in the eaCros
-00003cf0: 7328 2920 616e 6420 6561 5261 7465 2829  s() and eaRate()
-00003d00: 206d 6574 686f 6473 9468 075d 9468 158c   methods.h.].h..
-00003d10: 9649 6e20 7465 726d 7320 6f66 2062 7567  .In terms of bug
-00003d20: 2d66 6978 6573 2c20 7468 6520 6361 6c63  -fixes, the calc
-00003d30: 756c 6174 696f 6e20 6f66 2065 7863 6974  ulation of excit
-00003d40: 6174 696f 6e2d 6175 746f 696f 6e69 7a61  ation-autoioniza
-00003d50: 7469 6f6e 2063 726f 7373 2d73 6563 7469  tion cross-secti
-00003d60: 6f6e 7320 616e 6420 7261 7465 7320 6861  ons and rates ha
-00003d70: 7665 2062 6565 6e20 636f 7272 6563 7465  ve been correcte
-00003d80: 6420 696e 2074 6865 2065 6143 726f 7373  d in the eaCross
-00003d90: 2829 2061 6e64 2065 6152 6174 6528 2920  () and eaRate() 
-00003da0: 6d65 7468 6f64 7394 8594 8194 7d94 2868  methods.....}.(h
-00003db0: 056a 3c04 0000 681a 6a3a 0400 0068 0168  .j<...h.j:...h.h
-00003dc0: 0368 1b4e 681c 4e75 6261 681d 7d94 2868  .h.Nh.Nubah.}.(h
-00003dd0: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-00003de0: 275d 9475 6829 683c 681b 682a 681c 4b7e  '].uh)h<h.h*h.K~
-00003df0: 681a 6a7b 0300 0068 0168 0375 6268 3d29  h.j{...h.h.ubh=)
-00003e00: 8194 7d94 2868 058c 2643 7572 7265 6e74  ..}.(h..&Current
-00003e10: 2064 6576 656c 6f70 6d65 6e74 2069 7320   development is 
-00003e20: 7769 7468 2050 7974 686f 6e20 332e 3494  with Python 3.4.
-00003e30: 6807 5d94 6815 8c26 4375 7272 656e 7420  h.].h..&Current 
-00003e40: 6465 7665 6c6f 706d 656e 7420 6973 2077  development is w
-00003e50: 6974 6820 5079 7468 6f6e 2033 2e34 9485  ith Python 3.4..
-00003e60: 9481 947d 9428 6805 6a4a 0400 0068 1a6a  ...}.(h.jJ...h.j
-00003e70: 4804 0000 6801 6803 681b 4e68 1c4e 7562  H...h.h.h.Nh.Nub
-00003e80: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-00003e90: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
-00003ea0: 1b68 2a68 1c4b 8068 1a6a 7b03 0000 6801  .h*h.K.h.j{...h.
-00003eb0: 6803 7562 6568 1d7d 9428 681f 5d94 8c1b  h.ubeh.}.(h.]...
-00003ec0: 6368 616e 6765 732d 6672 6f6d 2d30 2d36  changes-from-0-6
-00003ed0: 2d35 2d74 6f2d 302d 372d 3094 6168 215d  -5-to-0-7-0.ah!]
-00003ee0: 9468 235d 948c 1b63 6861 6e67 6573 2066  .h#]...changes f
-00003ef0: 726f 6d20 302e 362e 3520 746f 2030 2e37  rom 0.6.5 to 0.7
-00003f00: 2e30 9461 6825 5d94 6827 5d94 7568 2968  .0.ah%].h'].uh)h
-00003f10: 0968 1a68 0b68 0168 0368 1b68 2a68 1c4b  .h.h.h.h.h.h*h.K
-00003f20: 6a75 6268 0a29 8194 7d94 2868 0568 0668  jubh.)..}.(h.h.h
-00003f30: 075d 9428 680f 2981 947d 9428 6805 8c1b  .].(h.)..}.(h...
-00003f40: 6368 616e 6765 7320 6672 6f6d 2030 2e36  changes from 0.6
-00003f50: 2e30 2074 6f20 302e 362e 3594 6807 5d94  .0 to 0.6.5.h.].
-00003f60: 6815 8c1b 6368 616e 6765 7320 6672 6f6d  h...changes from
-00003f70: 2030 2e36 2e30 2074 6f20 302e 362e 3594   0.6.0 to 0.6.5.
-00003f80: 8594 8194 7d94 2868 056a 6304 0000 681a  ....}.(h.jc...h.
-00003f90: 6a61 0400 0068 0168 0368 1b4e 681c 4e75  ja...h.h.h.Nh.Nu
-00003fa0: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
-00003fb0: 235d 9468 255d 9468 275d 9475 6829 680e  #].h%].h'].uh)h.
-00003fc0: 681a 6a5e 0400 0068 0168 0368 1b68 2a68  h.j^...h.h.h.h*h
-00003fd0: 1c4b 8375 6268 3d29 8194 7d94 2868 058c  .K.ubh=)..}.(h..
-00003fe0: 2e6d 6174 706c 6f74 6c69 622e 7079 706c  .matplotlib.pypl
-00003ff0: 6f74 2069 7320 6e6f 7720 696d 706f 7274  ot is now import
-00004000: 6564 2066 6f72 2070 6c6f 7474 696e 6794  ed for plotting.
-00004010: 6807 5d94 6815 8c2e 6d61 7470 6c6f 746c  h.].h...matplotl
-00004020: 6962 2e70 7970 6c6f 7420 6973 206e 6f77  ib.pyplot is now
-00004030: 2069 6d70 6f72 7465 6420 666f 7220 706c   imported for pl
-00004040: 6f74 7469 6e67 9485 9481 947d 9428 6805  otting.....}.(h.
-00004050: 6a71 0400 0068 1a6a 6f04 0000 6801 6803  jq...h.jo...h.h.
-00004060: 681b 4e68 1c4e 7562 6168 1d7d 9428 681f  h.Nh.Nubah.}.(h.
-00004070: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00004080: 5d94 7568 2968 3c68 1b68 2a68 1c4b 8568  ].uh)h<h.h*h.K.h
-00004090: 1a6a 5e04 0000 6801 6803 7562 683d 2981  .j^...h.h.ubh=).
-000040a0: 947d 9428 6805 8c8c 4950 7974 686f 6e20  .}.(h...IPython 
-000040b0: 7665 7273 696f 6e20 3420 2f20 4a75 7079  version 4 / Jupy
-000040c0: 7465 7220 6973 206e 6f77 206c 6973 7465  ter is now liste
-000040d0: 6420 6173 2061 2070 7265 7265 7175 6973  d as a prerequis
-000040e0: 6974 652e 2020 486f 7765 7665 722c 2076  ite.  However, v
-000040f0: 302e 362e 3420 6361 6e20 6265 206d 6164  0.6.4 can be mad
-00004100: 6520 636f 6d70 6174 6962 6c65 2077 6974  e compatible wit
-00004110: 6820 4950 7974 686f 6e20 3220 6f72 2033  h IPython 2 or 3
-00004120: 2077 6974 6820 6120 7369 6d70 6c65 2065   with a simple e
-00004130: 6469 742e 9468 075d 9468 158c 8c49 5079  dit..h.].h...IPy
-00004140: 7468 6f6e 2076 6572 7369 6f6e 2034 202f  thon version 4 /
-00004150: 204a 7570 7974 6572 2069 7320 6e6f 7720   Jupyter is now 
-00004160: 6c69 7374 6564 2061 7320 6120 7072 6572  listed as a prer
-00004170: 6571 7569 7369 7465 2e20 2048 6f77 6576  equisite.  Howev
-00004180: 6572 2c20 7630 2e36 2e34 2063 616e 2062  er, v0.6.4 can b
-00004190: 6520 6d61 6465 2063 6f6d 7061 7469 626c  e made compatibl
-000041a0: 6520 7769 7468 2049 5079 7468 6f6e 2032  e with IPython 2
-000041b0: 206f 7220 3320 7769 7468 2061 2073 696d   or 3 with a sim
-000041c0: 706c 6520 6564 6974 2e94 8594 8194 7d94  ple edit......}.
-000041d0: 2868 056a 7f04 0000 681a 6a7d 0400 0068  (h.j....h.j}...h
-000041e0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
-000041f0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-00004200: 9468 275d 9475 6829 683c 681b 682a 681c  .h'].uh)h<h.h*h.
-00004210: 4b87 681a 6a5e 0400 0068 0168 0375 6268  K.h.j^...h.h.ubh
-00004220: 3d29 8194 7d94 2868 058c 3e41 6e20 6572  =)..}.(h..>An er
-00004230: 726f 7220 696e 2063 616c 6375 6c61 7469  ror in calculati
-00004240: 6e67 2074 6865 2070 726f 746f 6e20 6578  ng the proton ex
-00004250: 6369 7461 7469 6f6e 2072 6174 6573 2077  citation rates w
-00004260: 6173 2066 6978 6564 2e94 6807 5d94 6815  as fixed..h.].h.
-00004270: 8c3e 416e 2065 7272 6f72 2069 6e20 6361  .>An error in ca
-00004280: 6c63 756c 6174 696e 6720 7468 6520 7072  lculating the pr
-00004290: 6f74 6f6e 2065 7863 6974 6174 696f 6e20  oton excitation 
-000042a0: 7261 7465 7320 7761 7320 6669 7865 642e  rates was fixed.
-000042b0: 9485 9481 947d 9428 6805 6a8d 0400 0068  .....}.(h.j....h
-000042c0: 1a6a 8b04 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-000042d0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-000042e0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
-000042f0: 3c68 1b68 2a68 1c4b 8968 1a6a 5e04 0000  <h.h*h.K.h.j^...
-00004300: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
-00004310: 8c63 5468 6520 636f 6465 2068 6173 2062  .cThe code has b
-00004320: 6565 6e20 6564 6974 6564 2074 6f20 6d61  een edited to ma
-00004330: 6b65 2069 7420 636f 6d70 6174 6962 6c65  ke it compatible
-00004340: 2077 6974 6820 5079 7468 6f6e 2033 2061   with Python 3 a
-00004350: 6e64 2068 6173 2062 6565 6e20 7465 7374  nd has been test
-00004360: 6564 2061 6761 696e 7374 2050 7974 686f  ed against Pytho
-00004370: 6e20 332e 3394 6807 5d94 6815 8c63 5468  n 3.3.h.].h..cTh
-00004380: 6520 636f 6465 2068 6173 2062 6565 6e20  e code has been 
-00004390: 6564 6974 6564 2074 6f20 6d61 6b65 2069  edited to make i
-000043a0: 7420 636f 6d70 6174 6962 6c65 2077 6974  t compatible wit
-000043b0: 6820 5079 7468 6f6e 2033 2061 6e64 2068  h Python 3 and h
-000043c0: 6173 2062 6565 6e20 7465 7374 6564 2061  as been tested a
-000043d0: 6761 696e 7374 2050 7974 686f 6e20 332e  gainst Python 3.
-000043e0: 3394 8594 8194 7d94 2868 056a 9b04 0000  3.....}.(h.j....
-000043f0: 681a 6a99 0400 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
-00004400: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
-00004410: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-00004420: 683c 681b 682a 681c 4b8b 681a 6a5e 0400  h<h.h*h.K.h.j^..
-00004430: 0068 0168 0375 6265 681d 7d94 2868 1f5d  .h.h.ubeh.}.(h.]
-00004440: 948c 1b63 6861 6e67 6573 2d66 726f 6d2d  ...changes-from-
-00004450: 302d 362d 302d 746f 2d30 2d36 2d35 9461  0-6-0-to-0-6-5.a
-00004460: 6821 5d94 6823 5d94 8c1b 6368 616e 6765  h!].h#]...change
-00004470: 7320 6672 6f6d 2030 2e36 2e30 2074 6f20  s from 0.6.0 to 
-00004480: 302e 362e 3594 6168 255d 9468 275d 9475  0.6.5.ah%].h'].u
-00004490: 6829 6809 681a 680b 6801 6803 681b 682a  h)h.h.h.h.h.h.h*
-000044a0: 681c 4b83 7562 680a 2981 947d 9428 6805  h.K.ubh.)..}.(h.
-000044b0: 6806 6807 5d94 2868 0f29 8194 7d94 2868  h.h.].(h.)..}.(h
-000044c0: 058c 1b63 6861 6e67 6573 2066 726f 6d20  ...changes from 
-000044d0: 302e 352e 3320 746f 2030 2e36 2e30 9468  0.5.3 to 0.6.0.h
-000044e0: 075d 9468 158c 1b63 6861 6e67 6573 2066  .].h...changes f
-000044f0: 726f 6d20 302e 352e 3320 746f 2030 2e36  rom 0.5.3 to 0.6
-00004500: 2e30 9485 9481 947d 9428 6805 6ab4 0400  .0.....}.(h.j...
-00004510: 0068 1a6a b204 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
-00004520: 1c4e 7562 6168 1d7d 9428 681f 5d94 6821  .Nubah.}.(h.].h!
-00004530: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00004540: 2968 0e68 1a6a af04 0000 6801 6803 681b  )h.h.j....h.h.h.
-00004550: 682a 681c 4b8e 7562 683d 2981 947d 9428  h*h.K.ubh=)..}.(
-00004560: 6805 8c18 5468 6973 2069 7320 6120 6d61  h...This is a ma
-00004570: 6a6f 7220 7265 6c65 6173 652e 9468 075d  jor release..h.]
-00004580: 9468 158c 1854 6869 7320 6973 2061 206d  .h...This is a m
-00004590: 616a 6f72 2072 656c 6561 7365 2e94 8594  ajor release....
-000045a0: 8194 7d94 2868 056a c204 0000 681a 6ac0  ..}.(h.j....h.j.
-000045b0: 0400 0068 0168 0368 1b4e 681c 4e75 6261  ...h.h.h.Nh.Nuba
-000045c0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-000045d0: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
-000045e0: 682a 681c 4b90 681a 6aaf 0400 0068 0168  h*h.K.h.j....h.h
-000045f0: 0375 6268 3d29 8194 7d94 2868 0558 3c01  .ubh=)..}.(h.X<.
-00004600: 0000 4669 7273 742c 2043 6869 616e 7469  ..First, Chianti
-00004610: 5079 2030 2e36 2e30 2069 7320 636f 6d70  Py 0.6.0 is comp
-00004620: 6174 6962 6c65 2077 6974 6820 7468 6520  atible with the 
-00004630: 6d6f 7374 2072 6563 656e 746c 7920 7265  most recently re
-00004640: 6c65 6173 6564 2043 4849 414e 5449 2064  leased CHIANTI d
-00004650: 6174 6162 6173 6520 7665 7273 696f 6e20  atabase version 
-00004660: 382e 302e 2020 4974 2061 6c73 6f20 6669  8.0.  It also fi
-00004670: 7865 7320 736f 6d65 206d 616a 6f72 2062  xes some major b
-00004680: 7567 7320 696e 2074 6865 2070 7265 7669  ugs in the previ
-00004690: 6f75 7320 7665 7273 696f 6e2e 2020 446f  ous version.  Do
-000046a0: 6375 6d65 6e74 6174 696f 6e20 6861 7320  cumentation has 
-000046b0: 6265 656e 2069 6d70 726f 7665 6420 616e  been improved an
-000046c0: 6420 6120 4950 7974 686f 6e20 6e6f 7465  d a IPython note
-000046d0: 626f 6f6b 202a 2a51 7569 636b 5374 6172  book **QuickStar
-000046e0: 742e 6970 796e 622a 2a2c 2074 6861 7420  t.ipynb**, that 
-000046f0: 6c61 7267 656c 7920 666f 6c6c 6f77 7320  largely follows 
-00004700: 7468 6520 2751 7569 636b 2053 7461 7274  the 'Quick Start
-00004710: 2720 646f 6375 6d65 6e74 6174 696f 6e20  ' documentation 
-00004720: 7061 6765 732c 2068 6173 2061 6c73 6f20  pages, has also 
-00004730: 6265 656e 2069 6e63 6c75 6465 642e 9468  been included..h
-00004740: 075d 9428 6815 8cd3 4669 7273 742c 2043  .].(h...First, C
-00004750: 6869 616e 7469 5079 2030 2e36 2e30 2069  hiantiPy 0.6.0 i
-00004760: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
-00004770: 6820 7468 6520 6d6f 7374 2072 6563 656e  h the most recen
-00004780: 746c 7920 7265 6c65 6173 6564 2043 4849  tly released CHI
-00004790: 414e 5449 2064 6174 6162 6173 6520 7665  ANTI database ve
-000047a0: 7273 696f 6e20 382e 302e 2020 4974 2061  rsion 8.0.  It a
-000047b0: 6c73 6f20 6669 7865 7320 736f 6d65 206d  lso fixes some m
-000047c0: 616a 6f72 2062 7567 7320 696e 2074 6865  ajor bugs in the
-000047d0: 2070 7265 7669 6f75 7320 7665 7273 696f   previous versio
-000047e0: 6e2e 2020 446f 6375 6d65 6e74 6174 696f  n.  Documentatio
-000047f0: 6e20 6861 7320 6265 656e 2069 6d70 726f  n has been impro
-00004800: 7665 6420 616e 6420 6120 4950 7974 686f  ved and a IPytho
-00004810: 6e20 6e6f 7465 626f 6f6b 2094 8594 8194  n notebook .....
-00004820: 7d94 2868 058c d346 6972 7374 2c20 4368  }.(h...First, Ch
-00004830: 6961 6e74 6950 7920 302e 362e 3020 6973  iantiPy 0.6.0 is
-00004840: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-00004850: 2074 6865 206d 6f73 7420 7265 6365 6e74   the most recent
-00004860: 6c79 2072 656c 6561 7365 6420 4348 4941  ly released CHIA
-00004870: 4e54 4920 6461 7461 6261 7365 2076 6572  NTI database ver
-00004880: 7369 6f6e 2038 2e30 2e20 2049 7420 616c  sion 8.0.  It al
-00004890: 736f 2066 6978 6573 2073 6f6d 6520 6d61  so fixes some ma
-000048a0: 6a6f 7220 6275 6773 2069 6e20 7468 6520  jor bugs in the 
-000048b0: 7072 6576 696f 7573 2076 6572 7369 6f6e  previous version
-000048c0: 2e20 2044 6f63 756d 656e 7461 7469 6f6e  .  Documentation
-000048d0: 2068 6173 2062 6565 6e20 696d 7072 6f76   has been improv
-000048e0: 6564 2061 6e64 2061 2049 5079 7468 6f6e  ed and a IPython
-000048f0: 206e 6f74 6562 6f6f 6b20 9468 1a6a ce04   notebook .h.j..
-00004900: 0000 6801 6803 681b 4e68 1c4e 7562 6a16  ..h.h.h.Nh.Nubj.
-00004910: 0300 0029 8194 7d94 2868 058c 142a 2a51  ...)..}.(h...**Q
-00004920: 7569 636b 5374 6172 742e 6970 796e 622a  uickStart.ipynb*
-00004930: 2a94 6807 5d94 6815 8c10 5175 6963 6b53  *.h.].h...QuickS
-00004940: 7461 7274 2e69 7079 6e62 9485 9481 947d  tart.ipynb.....}
-00004950: 9428 6805 6806 681a 6ad7 0400 0075 6261  .(h.h.h.j....uba
-00004960: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-00004970: 9468 255d 9468 275d 9475 6829 6a15 0300  .h%].h'].uh)j...
-00004980: 0068 1a6a ce04 0000 7562 6815 8c59 2c20  .h.j....ubh..Y, 
-00004990: 7468 6174 206c 6172 6765 6c79 2066 6f6c  that largely fol
-000049a0: 6c6f 7773 2074 6865 20e2 8098 5175 6963  lows the ...Quic
-000049b0: 6b20 5374 6172 74e2 8099 2064 6f63 756d  k Start... docum
-000049c0: 656e 7461 7469 6f6e 2070 6167 6573 2c20  entation pages, 
-000049d0: 6861 7320 616c 736f 2062 6565 6e20 696e  has also been in
-000049e0: 636c 7564 6564 2e94 8594 8194 7d94 2868  cluded......}.(h
-000049f0: 058c 552c 2074 6861 7420 6c61 7267 656c  ..U, that largel
-00004a00: 7920 666f 6c6c 6f77 7320 7468 6520 2751  y follows the 'Q
-00004a10: 7569 636b 2053 7461 7274 2720 646f 6375  uick Start' docu
-00004a20: 6d65 6e74 6174 696f 6e20 7061 6765 732c  mentation pages,
-00004a30: 2068 6173 2061 6c73 6f20 6265 656e 2069   has also been i
-00004a40: 6e63 6c75 6465 642e 9468 1a6a ce04 0000  ncluded..h.j....
-00004a50: 6801 6803 681b 4e68 1c4e 7562 6568 1d7d  h.h.h.Nh.Nubeh.}
-00004a60: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00004a70: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
-00004a80: 1c4b 9268 1a6a af04 0000 6801 6803 7562  .K.h.j....h.h.ub
-00004a90: 683d 2981 947d 9428 6805 586e 0100 0054  h=)..}.(h.Xn...T
-00004aa0: 6865 7265 2061 7265 2074 776f 206e 6577  here are two new
-00004ab0: 206d 756c 7469 2d69 6f6e 2063 6c61 7373   multi-ion class
-00004ac0: 6573 3a20 202a 2a62 756e 6368 2a2a 2061  es:  **bunch** a
-00004ad0: 6e64 202a 2a69 7079 6d73 7065 6374 7275  nd **ipymspectru
-00004ae0: 6d2a 2a2e 2020 2a2a 6275 6e63 682a 2a20  m**.  **bunch** 
-00004af0: 616c 6c6f 7773 2074 6865 2075 7365 7220  allows the user 
-00004b00: 746f 2063 616c 6375 6c61 7465 206c 696e  to calculate lin
-00004b10: 6520 696e 7465 6e73 6974 6965 7320 666f  e intensities fo
-00004b20: 7220 6120 7370 6563 6966 6965 6420 7365  r a specified se
-00004b30: 7420 6f66 2065 6c65 6d65 6e74 7320 6f72  t of elements or
-00004b40: 2069 6e64 6976 6964 7561 6c20 696f 6e73   individual ions
-00004b50: 2061 7320 6120 6675 6e63 7469 6f6e 206f   as a function o
-00004b60: 6620 7465 6d70 6572 6174 7572 6520 6f72  f temperature or
-00004b70: 2064 656e 7369 7479 2e20 204f 6e65 2061   density.  One a
-00004b80: 6476 616e 7461 6765 206f 6620 2a2a 6275  dvantage of **bu
-00004b90: 6e63 682a 2a20 6973 2074 6865 2061 6269  nch** is the abi
-00004ba0: 6c69 7479 2074 6f20 6361 6c63 756c 6174  lity to calculat
-00004bb0: 6520 7468 6520 696e 7465 6e73 6974 7920  e the intensity 
-00004bc0: 7261 7469 6f20 6f66 206c 696e 6573 206f  ratio of lines o
-00004bd0: 6620 7477 6f20 6469 6666 6572 656e 7420  f two different 
-00004be0: 696f 6e73 2061 7320 6120 6675 6e63 7469  ions as a functi
-00004bf0: 6f6e 206f 6620 7465 6d70 6572 6174 7572  on of temperatur
-00004c00: 6520 6f72 2064 656e 7369 7479 2e94 6807  e or density..h.
-00004c10: 5d94 2868 158c 2654 6865 7265 2061 7265  ].(h..&There are
-00004c20: 2074 776f 206e 6577 206d 756c 7469 2d69   two new multi-i
-00004c30: 6f6e 2063 6c61 7373 6573 3a20 2094 8594  on classes:  ...
-00004c40: 8194 7d94 2868 058c 2654 6865 7265 2061  ..}.(h..&There a
-00004c50: 7265 2074 776f 206e 6577 206d 756c 7469  re two new multi
-00004c60: 2d69 6f6e 2063 6c61 7373 6573 3a20 2094  -ion classes:  .
-00004c70: 681a 6af0 0400 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
-00004c80: 4e75 626a 1603 0000 2981 947d 9428 6805  Nubj....)..}.(h.
-00004c90: 8c09 2a2a 6275 6e63 682a 2a94 6807 5d94  ..**bunch**.h.].
-00004ca0: 6815 8c05 6275 6e63 6894 8594 8194 7d94  h...bunch.....}.
-00004cb0: 2868 0568 0668 1a6a f904 0000 7562 6168  (h.h.h.j....ubah
-00004cc0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-00004cd0: 6825 5d94 6827 5d94 7568 296a 1503 0000  h%].h'].uh)j....
-00004ce0: 681a 6af0 0400 0075 6268 158c 0520 616e  h.j....ubh... an
-00004cf0: 6420 9485 9481 947d 9428 6805 8c05 2061  d .....}.(h... a
-00004d00: 6e64 2094 681a 6af0 0400 0068 0168 0368  nd .h.j....h.h.h
-00004d10: 1b4e 681c 4e75 626a 1603 0000 2981 947d  .Nh.Nubj....)..}
-00004d20: 9428 6805 8c10 2a2a 6970 796d 7370 6563  .(h...**ipymspec
-00004d30: 7472 756d 2a2a 9468 075d 9468 158c 0c69  trum**.h.].h...i
-00004d40: 7079 6d73 7065 6374 7275 6d94 8594 8194  pymspectrum.....
-00004d50: 7d94 2868 0568 0668 1a6a 0c05 0000 7562  }.(h.h.h.j....ub
-00004d60: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-00004d70: 5d94 6825 5d94 6827 5d94 7568 296a 1503  ].h%].h'].uh)j..
-00004d80: 0000 681a 6af0 0400 0075 6268 158c 032e  ..h.j....ubh....
-00004d90: 2020 9485 9481 947d 9428 6805 8c03 2e20    .....}.(h.... 
-00004da0: 2094 681a 6af0 0400 0068 0168 0368 1b4e   .h.j....h.h.h.N
-00004db0: 681c 4e75 626a 1603 0000 2981 947d 9428  h.Nubj....)..}.(
-00004dc0: 6805 8c09 2a2a 6275 6e63 682a 2a94 6807  h...**bunch**.h.
-00004dd0: 5d94 6815 8c05 6275 6e63 6894 8594 8194  ].h...bunch.....
-00004de0: 7d94 2868 0568 0668 1a6a 1f05 0000 7562  }.(h.h.h.j....ub
-00004df0: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-00004e00: 5d94 6825 5d94 6827 5d94 7568 296a 1503  ].h%].h'].uh)j..
-00004e10: 0000 681a 6af0 0400 0075 6268 158c 9d20  ..h.j....ubh... 
-00004e20: 616c 6c6f 7773 2074 6865 2075 7365 7220  allows the user 
-00004e30: 746f 2063 616c 6375 6c61 7465 206c 696e  to calculate lin
-00004e40: 6520 696e 7465 6e73 6974 6965 7320 666f  e intensities fo
-00004e50: 7220 6120 7370 6563 6966 6965 6420 7365  r a specified se
-00004e60: 7420 6f66 2065 6c65 6d65 6e74 7320 6f72  t of elements or
-00004e70: 2069 6e64 6976 6964 7561 6c20 696f 6e73   individual ions
-00004e80: 2061 7320 6120 6675 6e63 7469 6f6e 206f   as a function o
-00004e90: 6620 7465 6d70 6572 6174 7572 6520 6f72  f temperature or
-00004ea0: 2064 656e 7369 7479 2e20 204f 6e65 2061   density.  One a
-00004eb0: 6476 616e 7461 6765 206f 6620 9485 9481  dvantage of ....
-00004ec0: 947d 9428 6805 8c9d 2061 6c6c 6f77 7320  .}.(h... allows 
-00004ed0: 7468 6520 7573 6572 2074 6f20 6361 6c63  the user to calc
-00004ee0: 756c 6174 6520 6c69 6e65 2069 6e74 656e  ulate line inten
-00004ef0: 7369 7469 6573 2066 6f72 2061 2073 7065  sities for a spe
-00004f00: 6369 6669 6564 2073 6574 206f 6620 656c  cified set of el
-00004f10: 656d 656e 7473 206f 7220 696e 6469 7669  ements or indivi
-00004f20: 6475 616c 2069 6f6e 7320 6173 2061 2066  dual ions as a f
-00004f30: 756e 6374 696f 6e20 6f66 2074 656d 7065  unction of tempe
-00004f40: 7261 7475 7265 206f 7220 6465 6e73 6974  rature or densit
-00004f50: 792e 2020 4f6e 6520 6164 7661 6e74 6167  y.  One advantag
-00004f60: 6520 6f66 2094 681a 6af0 0400 0068 0168  e of .h.j....h.h
-00004f70: 0368 1b4e 681c 4e75 626a 1603 0000 2981  .h.Nh.Nubj....).
-00004f80: 947d 9428 6805 8c09 2a2a 6275 6e63 682a  .}.(h...**bunch*
-00004f90: 2a94 6807 5d94 6815 8c05 6275 6e63 6894  *.h.].h...bunch.
-00004fa0: 8594 8194 7d94 2868 0568 0668 1a6a 3205  ....}.(h.h.h.j2.
-00004fb0: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-00004fc0: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00004fd0: 296a 1503 0000 681a 6af0 0400 0075 6268  )j....h.j....ubh
-00004fe0: 158c 7820 6973 2074 6865 2061 6269 6c69  ..x is the abili
-00004ff0: 7479 2074 6f20 6361 6c63 756c 6174 6520  ty to calculate 
-00005000: 7468 6520 696e 7465 6e73 6974 7920 7261  the intensity ra
-00005010: 7469 6f20 6f66 206c 696e 6573 206f 6620  tio of lines of 
-00005020: 7477 6f20 6469 6666 6572 656e 7420 696f  two different io
-00005030: 6e73 2061 7320 6120 6675 6e63 7469 6f6e  ns as a function
-00005040: 206f 6620 7465 6d70 6572 6174 7572 6520   of temperature 
-00005050: 6f72 2064 656e 7369 7479 2e94 8594 8194  or density......
-00005060: 7d94 2868 058c 7820 6973 2074 6865 2061  }.(h..x is the a
-00005070: 6269 6c69 7479 2074 6f20 6361 6c63 756c  bility to calcul
-00005080: 6174 6520 7468 6520 696e 7465 6e73 6974  ate the intensit
-00005090: 7920 7261 7469 6f20 6f66 206c 696e 6573  y ratio of lines
-000050a0: 206f 6620 7477 6f20 6469 6666 6572 656e   of two differen
-000050b0: 7420 696f 6e73 2061 7320 6120 6675 6e63  t ions as a func
-000050c0: 7469 6f6e 206f 6620 7465 6d70 6572 6174  tion of temperat
-000050d0: 7572 6520 6f72 2064 656e 7369 7479 2e94  ure or density..
-000050e0: 681a 6af0 0400 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
-000050f0: 4e75 6265 681d 7d94 2868 1f5d 9468 215d  Nubeh.}.(h.].h!]
-00005100: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
-00005110: 683c 681b 682a 681c 4b94 681a 6aaf 0400  h<h.h*h.K.h.j...
-00005120: 0068 0168 0375 6268 3d29 8194 7d94 2868  .h.h.ubh=)..}.(h
-00005130: 0558 6301 0000 2a2a 6970 796d 7370 6563  .Xc...**ipymspec
-00005140: 7472 756d 2a2a 2069 7320 6d75 6368 206c  trum** is much l
-00005150: 696b 6520 7468 6520 6578 6973 7469 6e67  ike the existing
-00005160: 202a 2a73 7065 6374 7275 6d2a 2a20 616e   **spectrum** an
-00005170: 6420 2a2a 6d73 7065 6374 7275 6d2a 2a20  d **mspectrum** 
-00005180: 636c 6173 7365 732e 2020 2a2a 6d73 7065  classes.  **mspe
-00005190: 6374 7275 6d2a 2a20 616c 6c6f 7773 2074  ctrum** allows t
-000051a0: 6865 2075 7365 206f 6620 7468 6520 5079  he use of the Py
-000051b0: 7468 6f6e 202a 2a6d 756c 7469 7072 6f63  thon **multiproc
-000051c0: 6573 7369 6e67 2a2a 206d 6f64 756c 6520  essing** module 
-000051d0: 746f 2073 7065 6564 2075 7020 7370 6563  to speed up spec
-000051e0: 7472 616c 2063 616c 6375 6c61 7469 6f6e  tral calculation
-000051f0: 732e 2020 5468 6520 2a2a 6970 796d 7370  s.  The **ipymsp
-00005200: 6563 7472 756d 2a2a 2063 6c61 7373 2075  ectrum** class u
-00005210: 7365 7320 7468 6520 4950 7974 686f 6e20  ses the IPython 
-00005220: 2a2a 7061 7261 6c6c 656c 2a2a 206d 6f64  **parallel** mod
-00005230: 756c 6520 736f 2074 6861 7420 6d75 6c74  ule so that mult
-00005240: 6970 726f 6365 7373 696e 6720 7370 6563  iprocessing spec
-00005250: 7472 616c 2063 616c 6375 6c61 7469 6f6e  tral calculation
-00005260: 7320 6361 6e20 6265 2070 6572 666f 726d  s can be perform
-00005270: 6564 2069 6e20 7468 6520 4950 7974 686f  ed in the IPytho
-00005280: 6e20 5174 436f 6e73 6f6c 6520 616e 6420  n QtConsole and 
-00005290: 4e6f 7465 626f 6f6b 2e94 6807 5d94 286a  Notebook..h.].(j
-000052a0: 1603 0000 2981 947d 9428 6805 8c10 2a2a  ....)..}.(h...**
-000052b0: 6970 796d 7370 6563 7472 756d 2a2a 9468  ipymspectrum**.h
-000052c0: 075d 9468 158c 0c69 7079 6d73 7065 6374  .].h...ipymspect
-000052d0: 7275 6d94 8594 8194 7d94 2868 0568 0668  rum.....}.(h.h.h
-000052e0: 1a6a 4f05 0000 7562 6168 1d7d 9428 681f  .jO...ubah.}.(h.
-000052f0: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00005300: 5d94 7568 296a 1503 0000 681a 6a4b 0500  ].uh)j....h.jK..
-00005310: 0075 6268 158c 1b20 6973 206d 7563 6820  .ubh... is much 
-00005320: 6c69 6b65 2074 6865 2065 7869 7374 696e  like the existin
-00005330: 6720 9485 9481 947d 9428 6805 8c1b 2069  g .....}.(h... i
-00005340: 7320 6d75 6368 206c 696b 6520 7468 6520  s much like the 
-00005350: 6578 6973 7469 6e67 2094 681a 6a4b 0500  existing .h.jK..
-00005360: 0068 0168 0368 1b4e 681c 4e75 626a 1603  .h.h.h.Nh.Nubj..
-00005370: 0000 2981 947d 9428 6805 8c0c 2a2a 7370  ..)..}.(h...**sp
-00005380: 6563 7472 756d 2a2a 9468 075d 9468 158c  ectrum**.h.].h..
-00005390: 0873 7065 6374 7275 6d94 8594 8194 7d94  .spectrum.....}.
-000053a0: 2868 0568 0668 1a6a 6205 0000 7562 6168  (h.h.h.jb...ubah
-000053b0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
-000053c0: 6825 5d94 6827 5d94 7568 296a 1503 0000  h%].h'].uh)j....
-000053d0: 681a 6a4b 0500 0075 6268 158c 0520 616e  h.jK...ubh... an
-000053e0: 6420 9485 9481 947d 9428 6805 8c05 2061  d .....}.(h... a
-000053f0: 6e64 2094 681a 6a4b 0500 0068 0168 0368  nd .h.jK...h.h.h
-00005400: 1b4e 681c 4e75 626a 1603 0000 2981 947d  .Nh.Nubj....)..}
-00005410: 9428 6805 8c0d 2a2a 6d73 7065 6374 7275  .(h...**mspectru
-00005420: 6d2a 2a94 6807 5d94 6815 8c09 6d73 7065  m**.h.].h...mspe
-00005430: 6374 7275 6d94 8594 8194 7d94 2868 0568  ctrum.....}.(h.h
-00005440: 0668 1a6a 7505 0000 7562 6168 1d7d 9428  .h.ju...ubah.}.(
-00005450: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
-00005460: 6827 5d94 7568 296a 1503 0000 681a 6a4b  h'].uh)j....h.jK
-00005470: 0500 0075 6268 158c 0b20 636c 6173 7365  ...ubh... classe
-00005480: 732e 2020 9485 9481 947d 9428 6805 8c0b  s.  .....}.(h...
-00005490: 2063 6c61 7373 6573 2e20 2094 681a 6a4b   classes.  .h.jK
-000054a0: 0500 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
-000054b0: 1603 0000 2981 947d 9428 6805 8c0d 2a2a  ....)..}.(h...**
-000054c0: 6d73 7065 6374 7275 6d2a 2a94 6807 5d94  mspectrum**.h.].
-000054d0: 6815 8c09 6d73 7065 6374 7275 6d94 8594  h...mspectrum...
-000054e0: 8194 7d94 2868 0568 0668 1a6a 8805 0000  ..}.(h.h.h.j....
-000054f0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
-00005500: 6823 5d94 6825 5d94 6827 5d94 7568 296a  h#].h%].h'].uh)j
-00005510: 1503 0000 681a 6a4b 0500 0075 6268 158c  ....h.jK...ubh..
-00005520: 1e20 616c 6c6f 7773 2074 6865 2075 7365  . allows the use
-00005530: 206f 6620 7468 6520 5079 7468 6f6e 2094   of the Python .
-00005540: 8594 8194 7d94 2868 058c 1e20 616c 6c6f  ....}.(h... allo
-00005550: 7773 2074 6865 2075 7365 206f 6620 7468  ws the use of th
-00005560: 6520 5079 7468 6f6e 2094 681a 6a4b 0500  e Python .h.jK..
-00005570: 0068 0168 0368 1b4e 681c 4e75 626a 1603  .h.h.h.Nh.Nubj..
-00005580: 0000 2981 947d 9428 6805 8c13 2a2a 6d75  ..)..}.(h...**mu
-00005590: 6c74 6970 726f 6365 7373 696e 672a 2a94  ltiprocessing**.
-000055a0: 6807 5d94 6815 8c0f 6d75 6c74 6970 726f  h.].h...multipro
-000055b0: 6365 7373 696e 6794 8594 8194 7d94 2868  cessing.....}.(h
-000055c0: 0568 0668 1a6a 9b05 0000 7562 6168 1d7d  .h.h.j....ubah.}
-000055d0: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-000055e0: 5d94 6827 5d94 7568 296a 1503 0000 681a  ].h'].uh)j....h.
-000055f0: 6a4b 0500 0075 6268 158c 3020 6d6f 6475  jK...ubh..0 modu
-00005600: 6c65 2074 6f20 7370 6565 6420 7570 2073  le to speed up s
-00005610: 7065 6374 7261 6c20 6361 6c63 756c 6174  pectral calculat
-00005620: 696f 6e73 2e20 2054 6865 2094 8594 8194  ions.  The .....
-00005630: 7d94 2868 058c 3020 6d6f 6475 6c65 2074  }.(h..0 module t
-00005640: 6f20 7370 6565 6420 7570 2073 7065 6374  o speed up spect
-00005650: 7261 6c20 6361 6c63 756c 6174 696f 6e73  ral calculations
-00005660: 2e20 2054 6865 2094 681a 6a4b 0500 0068  .  The .h.jK...h
-00005670: 0168 0368 1b4e 681c 4e75 626a 1603 0000  .h.h.Nh.Nubj....
-00005680: 2981 947d 9428 6805 8c10 2a2a 6970 796d  )..}.(h...**ipym
-00005690: 7370 6563 7472 756d 2a2a 9468 075d 9468  spectrum**.h.].h
-000056a0: 158c 0c69 7079 6d73 7065 6374 7275 6d94  ...ipymspectrum.
-000056b0: 8594 8194 7d94 2868 0568 0668 1a6a ae05  ....}.(h.h.h.j..
-000056c0: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-000056d0: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-000056e0: 296a 1503 0000 681a 6a4b 0500 0075 6268  )j....h.jK...ubh
-000056f0: 158c 1820 636c 6173 7320 7573 6573 2074  ... class uses t
-00005700: 6865 2049 5079 7468 6f6e 2094 8594 8194  he IPython .....
-00005710: 7d94 2868 058c 1820 636c 6173 7320 7573  }.(h... class us
-00005720: 6573 2074 6865 2049 5079 7468 6f6e 2094  es the IPython .
-00005730: 681a 6a4b 0500 0068 0168 0368 1b4e 681c  h.jK...h.h.h.Nh.
-00005740: 4e75 626a 1603 0000 2981 947d 9428 6805  Nubj....)..}.(h.
-00005750: 8c0c 2a2a 7061 7261 6c6c 656c 2a2a 9468  ..**parallel**.h
-00005760: 075d 9468 158c 0870 6172 616c 6c65 6c94  .].h...parallel.
-00005770: 8594 8194 7d94 2868 0568 0668 1a6a c105  ....}.(h.h.h.j..
-00005780: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-00005790: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-000057a0: 296a 1503 0000 681a 6a4b 0500 0075 6268  )j....h.jK...ubh
-000057b0: 158c 6d20 6d6f 6475 6c65 2073 6f20 7468  ..m module so th
-000057c0: 6174 206d 756c 7469 7072 6f63 6573 7369  at multiprocessi
-000057d0: 6e67 2073 7065 6374 7261 6c20 6361 6c63  ng spectral calc
-000057e0: 756c 6174 696f 6e73 2063 616e 2062 6520  ulations can be 
-000057f0: 7065 7266 6f72 6d65 6420 696e 2074 6865  performed in the
-00005800: 2049 5079 7468 6f6e 2051 7443 6f6e 736f   IPython QtConso
-00005810: 6c65 2061 6e64 204e 6f74 6562 6f6f 6b2e  le and Notebook.
-00005820: 9485 9481 947d 9428 6805 8c6d 206d 6f64  .....}.(h..m mod
-00005830: 756c 6520 736f 2074 6861 7420 6d75 6c74  ule so that mult
-00005840: 6970 726f 6365 7373 696e 6720 7370 6563  iprocessing spec
-00005850: 7472 616c 2063 616c 6375 6c61 7469 6f6e  tral calculation
-00005860: 7320 6361 6e20 6265 2070 6572 666f 726d  s can be perform
-00005870: 6564 2069 6e20 7468 6520 4950 7974 686f  ed in the IPytho
-00005880: 6e20 5174 436f 6e73 6f6c 6520 616e 6420  n QtConsole and 
-00005890: 4e6f 7465 626f 6f6b 2e94 681a 6a4b 0500  Notebook..h.jK..
-000058a0: 0068 0168 0368 1b4e 681c 4e75 6265 681d  .h.h.h.Nh.Nubeh.
-000058b0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-000058c0: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
-000058d0: 681c 4b96 681a 6aaf 0400 0068 0168 0375  h.K.h.j....h.h.u
-000058e0: 6268 3d29 8194 7d94 2868 0558 2e01 0000  bh=)..}.(h.X....
-000058f0: 4120 6e65 7720 6d65 7468 6f64 202a 2a69  A new method **i
-00005900: 6e74 656e 7369 7479 4c69 7374 2a2a 2068  ntensityList** h
-00005910: 6173 2062 6565 6e20 6465 7665 6c6f 7065  as been develope
-00005920: 6420 746f 2061 6c6c 6f77 2074 6865 2075  d to allow the u
-00005930: 7365 7220 746f 206c 6973 7420 7468 6520  ser to list the 
-00005940: 6d6f 7374 2069 6e74 656e 7365 206c 696e  most intense lin
-00005950: 6573 2077 6974 6869 6e20 6120 6769 7665  es within a give
-00005960: 6e20 7761 7665 6c65 6e67 7468 2072 616e  n wavelength ran
-00005970: 6765 2e20 2054 6869 7320 6e65 7720 6d65  ge.  This new me
-00005980: 7468 6f64 732c 2074 6f67 6574 6865 7220  thods, together 
-00005990: 7769 7468 2070 7265 7669 6f75 736c 7920  with previously 
-000059a0: 6578 6973 7469 6e67 202a 2a69 6e74 656e  existing **inten
-000059b0: 7369 7479 5261 7469 6f2a 2a20 616e 6420  sityRatio** and 
-000059c0: 2a2a 696e 7465 6e73 6974 7952 6174 696f  **intensityRatio
-000059d0: 5361 7665 2a2a 2061 7265 2061 6c6c 206e  Save** are all n
-000059e0: 6f77 2069 6e68 6572 6974 6564 2062 7920  ow inherited by 
-000059f0: 7468 6520 2a2a 696f 6e2a 2a20 636c 6173  the **ion** clas
-00005a00: 7373 2061 6e64 2074 6865 2020 6d75 6c74  ss and the  mult
-00005a10: 692d 696f 6e20 636c 6173 7365 732e 9468  i-ion classes..h
-00005a20: 075d 9428 6815 8c0d 4120 6e65 7720 6d65  .].(h...A new me
-00005a30: 7468 6f64 2094 8594 8194 7d94 2868 058c  thod .....}.(h..
-00005a40: 0d41 206e 6577 206d 6574 686f 6420 9468  .A new method .h
-00005a50: 1a6a da05 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-00005a60: 7562 6a16 0300 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-00005a70: 112a 2a69 6e74 656e 7369 7479 4c69 7374  .**intensityList
-00005a80: 2a2a 9468 075d 9468 158c 0d69 6e74 656e  **.h.].h...inten
-00005a90: 7369 7479 4c69 7374 9485 9481 947d 9428  sityList.....}.(
-00005aa0: 6805 6806 681a 6ae3 0500 0075 6261 681d  h.h.h.j....ubah.
-00005ab0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00005ac0: 255d 9468 275d 9475 6829 6a15 0300 0068  %].h'].uh)j....h
-00005ad0: 1a6a da05 0000 7562 6815 8c9b 2068 6173  .j....ubh... has
-00005ae0: 2062 6565 6e20 6465 7665 6c6f 7065 6420   been developed 
-00005af0: 746f 2061 6c6c 6f77 2074 6865 2075 7365  to allow the use
-00005b00: 7220 746f 206c 6973 7420 7468 6520 6d6f  r to list the mo
-00005b10: 7374 2069 6e74 656e 7365 206c 696e 6573  st intense lines
-00005b20: 2077 6974 6869 6e20 6120 6769 7665 6e20   within a given 
-00005b30: 7761 7665 6c65 6e67 7468 2072 616e 6765  wavelength range
-00005b40: 2e20 2054 6869 7320 6e65 7720 6d65 7468  .  This new meth
-00005b50: 6f64 732c 2074 6f67 6574 6865 7220 7769  ods, together wi
-00005b60: 7468 2070 7265 7669 6f75 736c 7920 6578  th previously ex
-00005b70: 6973 7469 6e67 2094 8594 8194 7d94 2868  isting .....}.(h
-00005b80: 058c 9b20 6861 7320 6265 656e 2064 6576  ... has been dev
-00005b90: 656c 6f70 6564 2074 6f20 616c 6c6f 7720  eloped to allow 
-00005ba0: 7468 6520 7573 6572 2074 6f20 6c69 7374  the user to list
-00005bb0: 2074 6865 206d 6f73 7420 696e 7465 6e73   the most intens
-00005bc0: 6520 6c69 6e65 7320 7769 7468 696e 2061  e lines within a
-00005bd0: 2067 6976 656e 2077 6176 656c 656e 6774   given wavelengt
-00005be0: 6820 7261 6e67 652e 2020 5468 6973 206e  h range.  This n
-00005bf0: 6577 206d 6574 686f 6473 2c20 746f 6765  ew methods, toge
-00005c00: 7468 6572 2077 6974 6820 7072 6576 696f  ther with previo
-00005c10: 7573 6c79 2065 7869 7374 696e 6720 9468  usly existing .h
-00005c20: 1a6a da05 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-00005c30: 7562 6a16 0300 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-00005c40: 122a 2a69 6e74 656e 7369 7479 5261 7469  .**intensityRati
-00005c50: 6f2a 2a94 6807 5d94 6815 8c0e 696e 7465  o**.h.].h...inte
-00005c60: 6e73 6974 7952 6174 696f 9485 9481 947d  nsityRatio.....}
-00005c70: 9428 6805 6806 681a 6af6 0500 0075 6261  .(h.h.h.j....uba
-00005c80: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-00005c90: 9468 255d 9468 275d 9475 6829 6a15 0300  .h%].h'].uh)j...
-00005ca0: 0068 1a6a da05 0000 7562 6815 8c05 2061  .h.j....ubh... a
-00005cb0: 6e64 2094 8594 8194 7d94 2868 058c 0520  nd .....}.(h... 
-00005cc0: 616e 6420 9468 1a6a da05 0000 6801 6803  and .h.j....h.h.
-00005cd0: 681b 4e68 1c4e 7562 6a16 0300 0029 8194  h.Nh.Nubj....)..
-00005ce0: 7d94 2868 058c 162a 2a69 6e74 656e 7369  }.(h...**intensi
-00005cf0: 7479 5261 7469 6f53 6176 652a 2a94 6807  tyRatioSave**.h.
-00005d00: 5d94 6815 8c12 696e 7465 6e73 6974 7952  ].h...intensityR
-00005d10: 6174 696f 5361 7665 9485 9481 947d 9428  atioSave.....}.(
-00005d20: 6805 6806 681a 6a09 0600 0075 6261 681d  h.h.h.j....ubah.
-00005d30: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00005d40: 255d 9468 275d 9475 6829 6a15 0300 0068  %].h'].uh)j....h
-00005d50: 1a6a da05 0000 7562 6815 8c1e 2061 7265  .j....ubh... are
-00005d60: 2061 6c6c 206e 6f77 2069 6e68 6572 6974   all now inherit
-00005d70: 6564 2062 7920 7468 6520 9485 9481 947d  ed by the .....}
-00005d80: 9428 6805 8c1e 2061 7265 2061 6c6c 206e  .(h... are all n
-00005d90: 6f77 2069 6e68 6572 6974 6564 2062 7920  ow inherited by 
-00005da0: 7468 6520 9468 1a6a da05 0000 6801 6803  the .h.j....h.h.
-00005db0: 681b 4e68 1c4e 7562 6a16 0300 0029 8194  h.Nh.Nubj....)..
-00005dc0: 7d94 2868 058c 072a 2a69 6f6e 2a2a 9468  }.(h...**ion**.h
-00005dd0: 075d 9468 158c 0369 6f6e 9485 9481 947d  .].h...ion.....}
-00005de0: 9428 6805 6806 681a 6a1c 0600 0075 6261  .(h.h.h.j....uba
-00005df0: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
-00005e00: 9468 255d 9468 275d 9475 6829 6a15 0300  .h%].h'].uh)j...
-00005e10: 0068 1a6a da05 0000 7562 6815 8c23 2063  .h.j....ubh..# c
-00005e20: 6c61 7373 7320 616e 6420 7468 6520 206d  lasss and the  m
-00005e30: 756c 7469 2d69 6f6e 2063 6c61 7373 6573  ulti-ion classes
-00005e40: 2e94 8594 8194 7d94 2868 058c 2320 636c  ......}.(h..# cl
-00005e50: 6173 7373 2061 6e64 2074 6865 2020 6d75  asss and the  mu
-00005e60: 6c74 692d 696f 6e20 636c 6173 7365 732e  lti-ion classes.
-00005e70: 9468 1a6a da05 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
-00005e80: 1c4e 7562 6568 1d7d 9428 681f 5d94 6821  .Nubeh.}.(h.].h!
-00005e90: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00005ea0: 2968 3c68 1b68 2a68 1c4b 9868 1a6a af04  )h<h.h*h.K.h.j..
-00005eb0: 0000 6801 6803 7562 683d 2981 947d 9428  ..h.h.ubh=)..}.(
-00005ec0: 6805 8cbf 5468 6520 2a2a 696f 6e2a 2a20  h...The **ion** 
-00005ed0: 616e 6420 6d75 6c74 692d 696f 6e20 636c  and multi-ion cl
-00005ee0: 6173 7365 7320 6e6f 7720 6163 6365 7074  asses now accept
-00005ef0: 2074 6865 206b 6579 776f 7264 2061 7267   the keyword arg
-00005f00: 756d 656e 7420 2a2a 6162 756e 6461 6e63  ument **abundanc
-00005f10: 654e 616d 652a 2a20 7468 6174 2061 6c6c  eName** that all
-00005f20: 6f77 2074 6865 2075 7365 7220 746f 2073  ow the user to s
-00005f30: 7065 6369 6679 2074 6865 2073 6574 206f  pecify the set o
-00005f40: 6620 656c 656d 656e 7461 6c20 6162 756e  f elemental abun
-00005f50: 6461 6e63 6573 2072 6174 6865 7220 7468  dances rather th
-00005f60: 616e 206a 7573 7420 7468 6520 6465 6661  an just the defa
-00005f70: 756c 7420 6162 756e 6461 6e63 6520 6669  ult abundance fi
-00005f80: 6c65 2e94 6807 5d94 2868 158c 0454 6865  le..h.].(h...The
-00005f90: 2094 8594 8194 7d94 2868 058c 0454 6865   .....}.(h...The
-00005fa0: 2094 681a 6a35 0600 0068 0168 0368 1b4e   .h.j5...h.h.h.N
-00005fb0: 681c 4e75 626a 1603 0000 2981 947d 9428  h.Nubj....)..}.(
-00005fc0: 6805 8c07 2a2a 696f 6e2a 2a94 6807 5d94  h...**ion**.h.].
-00005fd0: 6815 8c03 696f 6e94 8594 8194 7d94 2868  h...ion.....}.(h
-00005fe0: 0568 0668 1a6a 3e06 0000 7562 6168 1d7d  .h.h.j>...ubah.}
-00005ff0: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
-00006000: 5d94 6827 5d94 7568 296a 1503 0000 681a  ].h'].uh)j....h.
-00006010: 6a35 0600 0075 6268 158c 3720 616e 6420  j5...ubh..7 and 
-00006020: 6d75 6c74 692d 696f 6e20 636c 6173 7365  multi-ion classe
-00006030: 7320 6e6f 7720 6163 6365 7074 2074 6865  s now accept the
-00006040: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00006050: 7420 9485 9481 947d 9428 6805 8c37 2061  t .....}.(h..7 a
-00006060: 6e64 206d 756c 7469 2d69 6f6e 2063 6c61  nd multi-ion cla
-00006070: 7373 6573 206e 6f77 2061 6363 6570 7420  sses now accept 
-00006080: 7468 6520 6b65 7977 6f72 6420 6172 6775  the keyword argu
-00006090: 6d65 6e74 2094 681a 6a35 0600 0068 0168  ment .h.j5...h.h
-000060a0: 0368 1b4e 681c 4e75 626a 1603 0000 2981  .h.Nh.Nubj....).
-000060b0: 947d 9428 6805 8c11 2a2a 6162 756e 6461  .}.(h...**abunda
-000060c0: 6e63 654e 616d 652a 2a94 6807 5d94 6815  nceName**.h.].h.
-000060d0: 8c0d 6162 756e 6461 6e63 654e 616d 6594  ..abundanceName.
-000060e0: 8594 8194 7d94 2868 0568 0668 1a6a 5106  ....}.(h.h.h.jQ.
-000060f0: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-00006100: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
-00006110: 296a 1503 0000 681a 6a35 0600 0075 6268  )j....h.j5...ubh
-00006120: 158c 6c20 7468 6174 2061 6c6c 6f77 2074  ..l that allow t
-00006130: 6865 2075 7365 7220 746f 2073 7065 6369  he user to speci
-00006140: 6679 2074 6865 2073 6574 206f 6620 656c  fy the set of el
-00006150: 656d 656e 7461 6c20 6162 756e 6461 6e63  emental abundanc
-00006160: 6573 2072 6174 6865 7220 7468 616e 206a  es rather than j
-00006170: 7573 7420 7468 6520 6465 6661 756c 7420  ust the default 
-00006180: 6162 756e 6461 6e63 6520 6669 6c65 2e94  abundance file..
-00006190: 8594 8194 7d94 2868 058c 6c20 7468 6174  ....}.(h..l that
-000061a0: 2061 6c6c 6f77 2074 6865 2075 7365 7220   allow the user 
-000061b0: 746f 2073 7065 6369 6679 2074 6865 2073  to specify the s
-000061c0: 6574 206f 6620 656c 656d 656e 7461 6c20  et of elemental 
-000061d0: 6162 756e 6461 6e63 6573 2072 6174 6865  abundances rathe
-000061e0: 7220 7468 616e 206a 7573 7420 7468 6520  r than just the 
-000061f0: 6465 6661 756c 7420 6162 756e 6461 6e63  default abundanc
-00006200: 6520 6669 6c65 2e94 681a 6a35 0600 0068  e file..h.j5...h
-00006210: 0168 0368 1b4e 681c 4e75 6265 681d 7d94  .h.h.Nh.Nubeh.}.
-00006220: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
-00006230: 9468 275d 9475 6829 683c 681b 682a 681c  .h'].uh)h<h.h*h.
-00006240: 4b9a 681a 6aaf 0400 0068 0168 0375 6268  K.h.j....h.h.ubh
-00006250: 3d29 8194 7d94 2868 0558 0d01 0000 4164  =)..}.(h.X....Ad
-00006260: 6469 7469 6f6e 616c 2077 6520 6861 7665  ditional we have
-00006270: 2072 6570 6c61 6365 6420 7468 6520 466f   replaced the Fo
-00006280: 7274 7261 6e46 6f72 6d61 7420 6d6f 6475  rtranFormat modu
-00006290: 6c65 206f 6620 5363 6965 6e74 6966 6963  le of Scientific
-000062a0: 2050 7974 686f 6e20 6279 204b 6f6e 7261   Python by Konra
-000062b0: 6420 4869 6e73 656e 2077 6974 6820 7468  d Hinsen with th
-000062c0: 6520 2a2a 666f 7274 7261 6e66 6f72 6d61  e **fortranforma
-000062d0: 742a 2a20 6d6f 6475 6c65 206f 6620 4272  t** module of Br
-000062e0: 656e 6461 6e20 4172 6e6f 6c64 2061 7420  endan Arnold at 
-000062f0: 6874 7470 3a2f 2f62 6974 6275 636b 6574  http://bitbucket
-00006300: 2e6f 7267 2f62 7265 6e64 616e 6172 6e6f  .org/brendanarno
-00006310: 6c64 2f70 792d 666f 7274 7261 6e66 6f72  ld/py-fortranfor
-00006320: 6d61 742e 2020 4920 6861 7665 2073 6c69  mat.  I have sli
-00006330: 6768 746c 7920 6d6f 6469 6669 6564 2066  ghtly modified f
-00006340: 6f72 7472 616e 666f 726d 6174 2074 6f20  ortranformat to 
-00006350: 6d61 6b65 2069 7420 5079 7468 6f6e 2033  make it Python 3
-00006360: 2063 6f6d 706c 6961 6e74 2e94 6807 5d94   compliant..h.].
-00006370: 2868 158c 6441 6464 6974 696f 6e61 6c20  (h..dAdditional 
-00006380: 7765 2068 6176 6520 7265 706c 6163 6564  we have replaced
-00006390: 2074 6865 2046 6f72 7472 616e 466f 726d   the FortranForm
-000063a0: 6174 206d 6f64 756c 6520 6f66 2053 6369  at module of Sci
-000063b0: 656e 7469 6669 6320 5079 7468 6f6e 2062  entific Python b
-000063c0: 7920 4b6f 6e72 6164 2048 696e 7365 6e20  y Konrad Hinsen 
-000063d0: 7769 7468 2074 6865 2094 8594 8194 7d94  with the .....}.
-000063e0: 2868 058c 6441 6464 6974 696f 6e61 6c20  (h..dAdditional 
-000063f0: 7765 2068 6176 6520 7265 706c 6163 6564  we have replaced
-00006400: 2074 6865 2046 6f72 7472 616e 466f 726d   the FortranForm
-00006410: 6174 206d 6f64 756c 6520 6f66 2053 6369  at module of Sci
-00006420: 656e 7469 6669 6320 5079 7468 6f6e 2062  entific Python b
-00006430: 7920 4b6f 6e72 6164 2048 696e 7365 6e20  y Konrad Hinsen 
-00006440: 7769 7468 2074 6865 2094 681a 6a6a 0600  with the .h.jj..
-00006450: 0068 0168 0368 1b4e 681c 4e75 626a 1603  .h.h.h.Nh.Nubj..
-00006460: 0000 2981 947d 9428 6805 8c11 2a2a 666f  ..)..}.(h...**fo
-00006470: 7274 7261 6e66 6f72 6d61 742a 2a94 6807  rtranformat**.h.
-00006480: 5d94 6815 8c0d 666f 7274 7261 6e66 6f72  ].h...fortranfor
-00006490: 6d61 7494 8594 8194 7d94 2868 0568 0668  mat.....}.(h.h.h
-000064a0: 1a6a 7306 0000 7562 6168 1d7d 9428 681f  .js...ubah.}.(h.
-000064b0: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-000064c0: 5d94 7568 296a 1503 0000 681a 6a6a 0600  ].uh)j....h.jj..
-000064d0: 0075 6268 158c 1d20 6d6f 6475 6c65 206f  .ubh... module o
-000064e0: 6620 4272 656e 6461 6e20 4172 6e6f 6c64  f Brendan Arnold
-000064f0: 2061 7420 9485 9481 947d 9428 6805 8c1d   at .....}.(h...
-00006500: 206d 6f64 756c 6520 6f66 2042 7265 6e64   module of Brend
-00006510: 616e 2041 726e 6f6c 6420 6174 2094 681a  an Arnold at .h.
-00006520: 6a6a 0600 0068 0168 0368 1b4e 681c 4e75  jj...h.h.h.Nh.Nu
-00006530: 626a c701 0000 2981 947d 9428 6805 8c33  bj....)..}.(h..3
-00006540: 6874 7470 3a2f 2f62 6974 6275 636b 6574  http://bitbucket
-00006550: 2e6f 7267 2f62 7265 6e64 616e 6172 6e6f  .org/brendanarno
-00006560: 6c64 2f70 792d 666f 7274 7261 6e66 6f72  ld/py-fortranfor
-00006570: 6d61 7494 6807 5d94 6815 8c33 6874 7470  mat.h.].h..3http
-00006580: 3a2f 2f62 6974 6275 636b 6574 2e6f 7267  ://bitbucket.org
-00006590: 2f62 7265 6e64 616e 6172 6e6f 6c64 2f70  /brendanarnold/p
-000065a0: 792d 666f 7274 7261 6e66 6f72 6d61 7494  y-fortranformat.
-000065b0: 8594 8194 7d94 2868 0568 0668 1a6a 8606  ....}.(h.h.h.j..
-000065c0: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
-000065d0: 5d94 6823 5d94 6825 5d94 6827 5d94 8c06  ].h#].h%].h']...
-000065e0: 7265 6675 7269 946a 8806 0000 7568 296a  refuri.j....uh)j
-000065f0: c601 0000 681a 6a6a 0600 0075 6268 158c  ....h.jj...ubh..
-00006600: 482e 2020 4920 6861 7665 2073 6c69 6768  H.  I have sligh
-00006610: 746c 7920 6d6f 6469 6669 6564 2066 6f72  tly modified for
-00006620: 7472 616e 666f 726d 6174 2074 6f20 6d61  tranformat to ma
-00006630: 6b65 2069 7420 5079 7468 6f6e 2033 2063  ke it Python 3 c
-00006640: 6f6d 706c 6961 6e74 2e94 8594 8194 7d94  ompliant......}.
-00006650: 2868 058c 482e 2020 4920 6861 7665 2073  (h..H.  I have s
-00006660: 6c69 6768 746c 7920 6d6f 6469 6669 6564  lightly modified
-00006670: 2066 6f72 7472 616e 666f 726d 6174 2074   fortranformat t
-00006680: 6f20 6d61 6b65 2069 7420 5079 7468 6f6e  o make it Python
-00006690: 2033 2063 6f6d 706c 6961 6e74 2e94 681a   3 compliant..h.
-000066a0: 6a6a 0600 0068 0168 0368 1b4e 681c 4e75  jj...h.h.h.Nh.Nu
-000066b0: 6265 681d 7d94 2868 1f5d 9468 215d 9468  beh.}.(h.].h!].h
-000066c0: 235d 9468 255d 9468 275d 9475 6829 683c  #].h%].h'].uh)h<
-000066d0: 681b 682a 681c 4b9c 681a 6aaf 0400 0068  h.h*h.K.h.j....h
-000066e0: 0168 0375 6268 3d29 8194 7d94 2868 058c  .h.ubh=)..}.(h..
-000066f0: c746 6f72 2074 6865 2066 7574 7572 652c  .For the future,
-00006700: 2049 2070 6c61 6e20 746f 206d 616b 6520   I plan to make 
-00006710: 4368 6961 6e74 6950 7920 636f 6d70 6c69  ChiantiPy compli
-00006720: 616e 7420 7769 7468 2062 6f74 6820 5079  ant with both Py
-00006730: 7468 6f6e 2032 2e37 2061 6e64 2074 6865  thon 2.7 and the
-00006740: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
-00006750: 206f 6620 5079 7468 6f6e 2033 2028 6e6f   of Python 3 (no
-00006760: 7720 332e 3429 2c20 696d 7072 6f76 6520  w 3.4), improve 
-00006770: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00006780: 6e20 616e 6420 6d6f 7665 2074 6865 2070  n and move the p
-00006790: 726f 6a65 6320 746f 2067 6974 6875 622c  rojec to github,
-000067a0: 2069 6e20 6e6f 2070 6172 7469 6375 6c61   in no particula
-000067b0: 7220 6f72 6465 722e 9468 075d 9468 158c  r order..h.].h..
-000067c0: c746 6f72 2074 6865 2066 7574 7572 652c  .For the future,
-000067d0: 2049 2070 6c61 6e20 746f 206d 616b 6520   I plan to make 
-000067e0: 4368 6961 6e74 6950 7920 636f 6d70 6c69  ChiantiPy compli
-000067f0: 616e 7420 7769 7468 2062 6f74 6820 5079  ant with both Py
-00006800: 7468 6f6e 2032 2e37 2061 6e64 2074 6865  thon 2.7 and the
-00006810: 2063 7572 7265 6e74 2076 6572 7369 6f6e   current version
-00006820: 206f 6620 5079 7468 6f6e 2033 2028 6e6f   of Python 3 (no
-00006830: 7720 332e 3429 2c20 696d 7072 6f76 6520  w 3.4), improve 
-00006840: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00006850: 6e20 616e 6420 6d6f 7665 2074 6865 2070  n and move the p
-00006860: 726f 6a65 6320 746f 2067 6974 6875 622c  rojec to github,
-00006870: 2069 6e20 6e6f 2070 6172 7469 6375 6c61   in no particula
-00006880: 7220 6f72 6465 722e 9485 9481 947d 9428  r order......}.(
-00006890: 6805 6aa2 0600 0068 1a6a a006 0000 6801  h.j....h.j....h.
-000068a0: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
-000068b0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
-000068c0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
-000068d0: 9e68 1a6a af04 0000 6801 6803 7562 683d  .h.j....h.h.ubh=
-000068e0: 2981 947d 9428 6805 581a 0100 0043 6869  )..}.(h.X....Chi
-000068f0: 616e 7469 5079 2069 7320 6e6f 7720 7265  antiPy is now re
-00006900: 6c65 6173 6564 2075 6e64 6572 2061 206e  leased under a n
-00006910: 6577 206c 6963 656e 7365 2c20 7468 6520  ew license, the 
-00006920: 4f53 4920 6170 7072 6f76 6564 2049 5343  OSI approved ISC
-00006930: 4c20 6c69 6365 6e73 652e 2020 4672 6f6d  L license.  From
-00006940: 2057 696b 6970 6564 6961 5f20 2a54 6865   Wikipedia_ *The
-00006950: 2049 5343 4c20 6c69 6365 6e73 6520 6973   ISCL license is
-00006960: 2061 2070 6572 6d69 7373 6976 6520 6672   a permissive fr
-00006970: 6565 2073 6f66 7477 6172 6520 6c69 6365  ee software lice
-00006980: 6e73 6520 7772 6974 7465 6e20 6279 2074  nse written by t
-00006990: 6865 2049 6e74 6572 6e65 7420 536f 6674  he Internet Soft
-000069a0: 7761 7265 2043 6f6e 736f 7274 6975 6d20  ware Consortium 
-000069b0: 2849 5343 292e 2049 7420 6973 2066 756e  (ISC). It is fun
-000069c0: 6374 696f 6e61 6c6c 7920 6571 7569 7661  ctionally equiva
-000069d0: 6c65 6e74 2074 6f20 7468 6520 7369 6d70  lent to the simp
-000069e0: 6c69 6669 6564 2042 5344 2061 6e64 204d  lified BSD and M
-000069f0: 4954 2f45 7870 6174 206c 6963 656e 7365  IT/Expat license
-00006a00: 732c 202e 2e2e 2a94 6807 5d94 2868 158c  s, ...*.h.].(h..
-00006a10: 5443 6869 616e 7469 5079 2069 7320 6e6f  TChiantiPy is no
-00006a20: 7720 7265 6c65 6173 6564 2075 6e64 6572  w released under
-00006a30: 2061 206e 6577 206c 6963 656e 7365 2c20   a new license, 
-00006a40: 7468 6520 4f53 4920 6170 7072 6f76 6564  the OSI approved
-00006a50: 2049 5343 4c20 6c69 6365 6e73 652e 2020   ISCL license.  
-00006a60: 4672 6f6d 2094 8594 8194 7d94 2868 058c  From .....}.(h..
-00006a70: 5443 6869 616e 7469 5079 2069 7320 6e6f  TChiantiPy is no
-00006a80: 7720 7265 6c65 6173 6564 2075 6e64 6572  w released under
-00006a90: 2061 206e 6577 206c 6963 656e 7365 2c20   a new license, 
-00006aa0: 7468 6520 4f53 4920 6170 7072 6f76 6564  the OSI approved
-00006ab0: 2049 5343 4c20 6c69 6365 6e73 652e 2020   ISCL license.  
-00006ac0: 4672 6f6d 2094 681a 6aae 0600 0068 0168  From .h.j....h.h
-00006ad0: 0368 1b4e 681c 4e75 626a c701 0000 2981  .h.Nh.Nubj....).
-00006ae0: 947d 9428 6805 8c0a 5769 6b69 7065 6469  .}.(h...Wikipedi
-00006af0: 615f 9468 075d 9468 158c 0957 696b 6970  a_.h.].h...Wikip
-00006b00: 6564 6961 9485 9481 947d 9428 6805 6806  edia.....}.(h.h.
-00006b10: 681a 6ab7 0600 0075 6261 681d 7d94 2868  h.j....ubah.}.(h
-00006b20: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
-00006b30: 275d 948c 046e 616d 6594 8c09 5769 6b69  ']...name...Wiki
-00006b40: 7065 6469 6194 6a74 0200 008c 4668 7474  pedia.jt....Fhtt
-00006b50: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-00006b60: 612e 6f72 672f 772f 696e 6465 782e 7068  a.org/w/index.ph
-00006b70: 703f 7469 746c 653d 4953 435f 6c69 6365  p?title=ISC_lice
-00006b80: 6e73 6526 6f6c 6469 643d 3636 3436 3936  nse&oldid=664696
-00006b90: 3939 3394 7568 296a c601 0000 681a 6aae  993.uh)j....h.j.
-00006ba0: 0600 006a 7602 0000 4b01 7562 6815 8c01  ...jv...K.ubh...
-00006bb0: 2094 8594 8194 7d94 2868 058c 0120 9468   .....}.(h... .h
-00006bc0: 1a6a ae06 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
-00006bd0: 7562 6800 8c08 656d 7068 6173 6973 9493  ubh...emphasis..
-00006be0: 9429 8194 7d94 2868 058c bb2a 5468 6520  .)..}.(h...*The 
-00006bf0: 4953 434c 206c 6963 656e 7365 2069 7320  ISCL license is 
-00006c00: 6120 7065 726d 6973 7369 7665 2066 7265  a permissive fre
-00006c10: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
-00006c20: 7365 2077 7269 7474 656e 2062 7920 7468  se written by th
-00006c30: 6520 496e 7465 726e 6574 2053 6f66 7477  e Internet Softw
-00006c40: 6172 6520 436f 6e73 6f72 7469 756d 2028  are Consortium (
-00006c50: 4953 4329 2e20 4974 2069 7320 6675 6e63  ISC). It is func
-00006c60: 7469 6f6e 616c 6c79 2065 7175 6976 616c  tionally equival
-00006c70: 656e 7420 746f 2074 6865 2073 696d 706c  ent to the simpl
-00006c80: 6966 6965 6420 4253 4420 616e 6420 4d49  ified BSD and MI
-00006c90: 542f 4578 7061 7420 6c69 6365 6e73 6573  T/Expat licenses
-00006ca0: 2c20 2e2e 2e2a 9468 075d 9468 158c b954  , ...*.h.].h...T
-00006cb0: 6865 2049 5343 4c20 6c69 6365 6e73 6520  he ISCL license 
-00006cc0: 6973 2061 2070 6572 6d69 7373 6976 6520  is a permissive 
-00006cd0: 6672 6565 2073 6f66 7477 6172 6520 6c69  free software li
-00006ce0: 6365 6e73 6520 7772 6974 7465 6e20 6279  cense written by
-00006cf0: 2074 6865 2049 6e74 6572 6e65 7420 536f   the Internet So
-00006d00: 6674 7761 7265 2043 6f6e 736f 7274 6975  ftware Consortiu
-00006d10: 6d20 2849 5343 292e 2049 7420 6973 2066  m (ISC). It is f
-00006d20: 756e 6374 696f 6e61 6c6c 7920 6571 7569  unctionally equi
-00006d30: 7661 6c65 6e74 2074 6f20 7468 6520 7369  valent to the si
-00006d40: 6d70 6c69 6669 6564 2042 5344 2061 6e64  mplified BSD and
-00006d50: 204d 4954 2f45 7870 6174 206c 6963 656e   MIT/Expat licen
-00006d60: 7365 732c 20e2 80a6 9485 9481 947d 9428  ses, ........}.(
-00006d70: 6805 6806 681a 6acf 0600 0075 6261 681d  h.h.h.j....ubah.
-00006d80: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00006d90: 255d 9468 275d 9475 6829 6acd 0600 0068  %].h'].uh)j....h
-00006da0: 1a6a ae06 0000 7562 6568 1d7d 9428 681f  .j....ubeh.}.(h.
-00006db0: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
-00006dc0: 5d94 7568 2968 3c68 1b68 2a68 1c4b a068  ].uh)h<h.h*h.K.h
-00006dd0: 1a6a af04 0000 6801 6803 7562 6a94 0200  .j....h.h.ubj...
-00006de0: 0029 8194 7d94 2868 058c 552e 2e20 5f57  .)..}.(h..U.. _W
-00006df0: 696b 6970 6564 6961 3a20 6874 7470 733a  ikipedia: https:
-00006e00: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00006e10: 7267 2f77 2f69 6e64 6578 2e70 6870 3f74  rg/w/index.php?t
-00006e20: 6974 6c65 3d49 5343 5f6c 6963 656e 7365  itle=ISC_license
-00006e30: 266f 6c64 6964 3d36 3634 3639 3639 3933  &oldid=664696993
-00006e40: 9468 075d 9468 1d7d 9428 681f 5d94 8c09  .h.].h.}.(h.]...
-00006e50: 7769 6b69 7065 6469 6194 6168 215d 9468  wikipedia.ah!].h
-00006e60: 235d 948c 0977 696b 6970 6564 6961 9461  #]...wikipedia.a
-00006e70: 6825 5d94 6827 5d94 6a74 0200 006a c706  h%].h'].jt...j..
-00006e80: 0000 7568 296a 9302 0000 681c 4ba2 681a  ..uh)j....h.K.h.
-00006e90: 6aaf 0400 0068 0168 0368 1b68 2a6a 1e01  j....h.h.h.h*j..
-00006ea0: 0000 4b01 7562 6568 1d7d 9428 681f 5d94  ..K.ubeh.}.(h.].
-00006eb0: 8c1b 6368 616e 6765 732d 6672 6f6d 2d30  ..changes-from-0
-00006ec0: 2d35 2d33 2d74 6f2d 302d 362d 3094 6168  -5-3-to-0-6-0.ah
-00006ed0: 215d 9468 235d 948c 1b63 6861 6e67 6573  !].h#]...changes
-00006ee0: 2066 726f 6d20 302e 352e 3320 746f 2030   from 0.5.3 to 0
-00006ef0: 2e36 2e30 9461 6825 5d94 6827 5d94 7568  .6.0.ah%].h'].uh
-00006f00: 2968 0968 1a68 0b68 0168 0368 1b68 2a68  )h.h.h.h.h.h.h*h
-00006f10: 1c4b 8e75 6265 681d 7d94 2868 1f5d 948c  .K.ubeh.}.(h.]..
-00006f20: 0963 6861 6e67 656c 6f67 9461 6821 5d94  .changelog.ah!].
-00006f30: 6823 5d94 8c09 6368 616e 6765 6c6f 6794  h#]...changelog.
-00006f40: 6168 255d 9468 275d 9475 6829 6809 681a  ah%].h'].uh)h.h.
-00006f50: 6803 6801 6803 681b 682a 681c 4b03 7562  h.h.h.h.h*h.K.ub
-00006f60: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
-00006f70: 5d94 6825 5d94 6827 5d94 8c06 736f 7572  ].h%].h']...sour
-00006f80: 6365 9468 2a75 6829 6801 8c0e 6375 7272  ce.h*uh)h...curr
-00006f90: 656e 745f 736f 7572 6365 944e 8c0c 6375  ent_source.N..cu
-00006fa0: 7272 656e 745f 6c69 6e65 944e 8c08 7365  rrent_line.N..se
-00006fb0: 7474 696e 6773 948c 1164 6f63 7574 696c  ttings...docutil
-00006fc0: 732e 6672 6f6e 7465 6e64 948c 0656 616c  s.frontend...Val
-00006fd0: 7565 7394 9394 2981 947d 9428 680e 4e8c  ues...)..}.(h.N.
-00006fe0: 0967 656e 6572 6174 6f72 944e 8c09 6461  .generator.N..da
-00006ff0: 7465 7374 616d 7094 4e8c 0b73 6f75 7263  testamp.N..sourc
-00007000: 655f 6c69 6e6b 944e 8c0a 736f 7572 6365  e_link.N..source
-00007010: 5f75 726c 944e 8c0d 746f 635f 6261 636b  _url.N..toc_back
-00007020: 6c69 6e6b 7394 8c05 656e 7472 7994 8c12  links...entry...
-00007030: 666f 6f74 6e6f 7465 5f62 6163 6b6c 696e  footnote_backlin
-00007040: 6b73 944b 018c 0d73 6563 746e 756d 5f78  ks.K...sectnum_x
-00007050: 666f 726d 944b 018c 0e73 7472 6970 5f63  form.K...strip_c
-00007060: 6f6d 6d65 6e74 7394 4e8c 1b73 7472 6970  omments.N..strip
-00007070: 5f65 6c65 6d65 6e74 735f 7769 7468 5f63  _elements_with_c
-00007080: 6c61 7373 6573 944e 8c0d 7374 7269 705f  lasses.N..strip_
-00007090: 636c 6173 7365 7394 4e8c 0c72 6570 6f72  classes.N..repor
-000070a0: 745f 6c65 7665 6c94 4b02 8c0a 6861 6c74  t_level.K...halt
-000070b0: 5f6c 6576 656c 944b 058c 1165 7869 745f  _level.K...exit_
-000070c0: 7374 6174 7573 5f6c 6576 656c 944b 058c  status_level.K..
-000070d0: 0564 6562 7567 944e 8c0e 7761 726e 696e  .debug.N..warnin
-000070e0: 675f 7374 7265 616d 944e 8c09 7472 6163  g_stream.N..trac
-000070f0: 6562 6163 6b94 888c 0e69 6e70 7574 5f65  eback....input_e
-00007100: 6e63 6f64 696e 6794 8c09 7574 662d 382d  ncoding...utf-8-
-00007110: 7369 6794 8c1c 696e 7075 745f 656e 636f  sig...input_enco
-00007120: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
-00007130: 6572 948c 0673 7472 6963 7494 8c0f 6f75  er...strict...ou
-00007140: 7470 7574 5f65 6e63 6f64 696e 6794 8c05  tput_encoding...
-00007150: 7574 662d 3894 8c1d 6f75 7470 7574 5f65  utf-8...output_e
-00007160: 6e63 6f64 696e 675f 6572 726f 725f 6861  ncoding_error_ha
-00007170: 6e64 6c65 7294 6a22 0700 008c 0e65 7272  ndler.j".....err
-00007180: 6f72 5f65 6e63 6f64 696e 6794 8c05 5554  or_encoding...UT
-00007190: 462d 3894 8c1c 6572 726f 725f 656e 636f  F-8...error_enco
-000071a0: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
-000071b0: 6572 948c 1062 6163 6b73 6c61 7368 7265  er...backslashre
-000071c0: 706c 6163 6594 8c0d 6c61 6e67 7561 6765  place...language
-000071d0: 5f63 6f64 6594 8c02 656e 948c 1372 6563  _code...en...rec
-000071e0: 6f72 645f 6465 7065 6e64 656e 6369 6573  ord_dependencies
-000071f0: 944e 8c06 636f 6e66 6967 944e 8c09 6964  .N..config.N..id
-00007200: 5f70 7265 6669 7894 6806 8c0e 6175 746f  _prefix.h...auto
-00007210: 5f69 645f 7072 6566 6978 948c 0269 6494  _id_prefix...id.
-00007220: 8c0d 6475 6d70 5f73 6574 7469 6e67 7394  ..dump_settings.
-00007230: 4e8c 0e64 756d 705f 696e 7465 726e 616c  N..dump_internal
-00007240: 7394 4e8c 0f64 756d 705f 7472 616e 7366  s.N..dump_transf
-00007250: 6f72 6d73 944e 8c0f 6475 6d70 5f70 7365  orms.N..dump_pse
-00007260: 7564 6f5f 786d 6c94 4e8c 1065 7870 6f73  udo_xml.N..expos
-00007270: 655f 696e 7465 726e 616c 7394 4e8c 0e73  e_internals.N..s
-00007280: 7472 6963 745f 7669 7369 746f 7294 4e8c  trict_visitor.N.
-00007290: 0f5f 6469 7361 626c 655f 636f 6e66 6967  ._disable_config
-000072a0: 944e 8c07 5f73 6f75 7263 6594 682a 8c0c  .N.._source.h*..
-000072b0: 5f64 6573 7469 6e61 7469 6f6e 944e 8c0d  _destination.N..
-000072c0: 5f63 6f6e 6669 675f 6669 6c65 7394 5d94  _config_files.].
-000072d0: 8c0e 7065 705f 7265 6665 7265 6e63 6573  ..pep_references
-000072e0: 944e 8c0c 7065 705f 6261 7365 5f75 726c  .N..pep_base_url
-000072f0: 948c 2068 7474 7073 3a2f 2f77 7777 2e70  .. https://www.p
-00007300: 7974 686f 6e2e 6f72 672f 6465 762f 7065  ython.org/dev/pe
-00007310: 7073 2f94 8c15 7065 705f 6669 6c65 5f75  ps/...pep_file_u
-00007320: 726c 5f74 656d 706c 6174 6594 8c08 7065  rl_template...pe
-00007330: 702d 2530 3464 948c 0e72 6663 5f72 6566  p-%04d...rfc_ref
-00007340: 6572 656e 6365 7394 4e8c 0c72 6663 5f62  erences.N..rfc_b
-00007350: 6173 655f 7572 6c94 8c1c 6874 7470 733a  ase_url...https:
-00007360: 2f2f 746f 6f6c 732e 6965 7466 2e6f 7267  //tools.ietf.org
-00007370: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
-00007380: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
-00007390: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
-000073a0: 7061 6365 9489 8c16 6669 6c65 5f69 6e73  pace....file_ins
-000073b0: 6572 7469 6f6e 5f65 6e61 626c 6564 9488  ertion_enabled..
-000073c0: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
-000073d0: 8c10 7379 6e74 6178 5f68 6967 686c 6967  ..syntax_highlig
-000073e0: 6874 948c 046c 6f6e 6794 8c0c 736d 6172  ht...long...smar
-000073f0: 745f 7175 6f74 6573 9488 8c13 736d 6172  t_quotes....smar
-00007400: 7471 756f 7465 735f 6c6f 6361 6c65 7394  tquotes_locales.
-00007410: 4e8c 1d63 6861 7261 6374 6572 5f6c 6576  N..character_lev
-00007420: 656c 5f69 6e6c 696e 655f 6d61 726b 7570  el_inline_markup
-00007430: 9489 8c0e 646f 6374 6974 6c65 5f78 666f  ....doctitle_xfo
-00007440: 726d 9489 8c0d 646f 6369 6e66 6f5f 7866  rm....docinfo_xf
-00007450: 6f72 6d94 4b01 8c12 7365 6374 7375 6274  orm.K...sectsubt
-00007460: 6974 6c65 5f78 666f 726d 9489 8c10 656d  itle_xform....em
-00007470: 6265 645f 7374 796c 6573 6865 6574 9489  bed_stylesheet..
-00007480: 8c15 636c 6f61 6b5f 656d 6169 6c5f 6164  ..cloak_email_ad
-00007490: 6472 6573 7365 7394 888c 0365 6e76 944e  dresses....env.N
-000074a0: 8c0f 6765 7474 6578 745f 636f 6d70 6163  ..gettext_compac
-000074b0: 7494 8875 628c 0872 6570 6f72 7465 7294  t..ub..reporter.
-000074c0: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-000074d0: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-000074e0: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
-000074f0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
-00007500: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
-00007510: 288c 0967 6974 6875 622e 696f 945d 946a  (..github.io.].j
-00007520: 6402 0000 618c 0b72 6561 6474 6865 646f  d...a..readthedo
-00007530: 6373 945d 946a 7c02 0000 618c 0667 6974  cs.].j|...a..git
-00007540: 6875 6294 5d94 6a95 0300 0061 8c07 6173  hub.].j....a..as
-00007550: 7472 6f70 7994 5d94 6ac6 0300 0061 8c05  tropy.].j....a..
-00007560: 7375 6e70 7994 5d94 6adc 0300 0061 8c09  sunpy.].j....a..
-00007570: 7769 6b69 7065 6469 6194 5d94 6ab7 0600  wikipedia.].j...
-00007580: 0061 758c 0672 6566 6964 7394 7d94 8c07  .au..refids.}...
-00007590: 6e61 6d65 6964 7394 7d94 286a fc06 0000  nameids.}.(j....
-000075a0: 6af9 0600 0068 7168 6e68 9868 9568 cd68  j....hqhnh.h.h.h
-000075b0: ca68 e668 e38c 2074 6869 7320 6973 2061  .h.h.. this is a
-000075c0: 206d 616a 6f72 2062 7567 2d66 6978 2072   major bug-fix r
-000075d0: 656c 6561 7365 2e94 4e6a 3501 0000 6a32  elease..Nj5...j2
-000075e0: 0100 006a 7401 0000 6a71 0100 006a 2b02  ...jt...jq...j+.
-000075f0: 0000 6a28 0200 006a b202 0000 6aaf 0200  ..j(...j....j...
-00007600: 006a 9e02 0000 6a9b 0200 006a aa02 0000  .j....j....j....
-00007610: 6aa7 0200 006a 7803 0000 6a75 0300 006a  j....jx...ju...j
-00007620: 5b04 0000 6a58 0400 006a ba03 0000 6ab7  [...jX...j....j.
-00007630: 0300 006a 0104 0000 6afe 0300 006a 0d04  ...j....j....j..
-00007640: 0000 6a0a 0400 006a ac04 0000 6aa9 0400  ..j....j....j...
-00007650: 006a f406 0000 6af1 0600 006a ec06 0000  .j....j....j....
-00007660: 6ae9 0600 0075 8c09 6e61 6d65 7479 7065  j....u..nametype
-00007670: 7394 7d94 286a fc06 0000 4e68 714e 6898  s.}.(j....NhqNh.
-00007680: 4e68 cd4e 68e6 4e6a 6d07 0000 4e6a 3501  Nh.Nh.Njm...Nj5.
-00007690: 0000 4e6a 7401 0000 4e6a 2b02 0000 4e6a  ..Njt...Nj+...Nj
-000076a0: b202 0000 4e6a 9e02 0000 886a aa02 0000  ....Nj.....j....
-000076b0: 886a 7803 0000 4e6a 5b04 0000 4e6a ba03  .jx...Nj[...Nj..
-000076c0: 0000 886a 0104 0000 886a 0d04 0000 886a  ...j.....j.....j
-000076d0: ac04 0000 4e6a f406 0000 4e6a ec06 0000  ....Nj....Nj....
-000076e0: 8875 681f 7d94 286a f906 0000 680b 686e  .uh.}.(j....h.hn
-000076f0: 682b 6895 6874 68ca 689b 68e3 68d0 6a18  h+h.hth.h.h.h.j.
-00007700: 0100 0068 e96a 3201 0000 6a1f 0100 006a  ...h.j2...j....j
-00007710: 5901 0000 6a38 0100 006a 7101 0000 6a5e  Y...j8...jq...j^
-00007720: 0100 006a 9801 0000 6a77 0100 006a 2802  ...j....jw...j(.
-00007730: 0000 6a9e 0100 006a af02 0000 6a2e 0200  ..j....j....j...
-00007740: 006a 9b02 0000 6a95 0200 006a a702 0000  .j....j....j....
-00007750: 6aa1 0200 006a 7503 0000 6ab5 0200 006a  j....ju...j....j
-00007760: 5804 0000 6a7b 0300 006a b703 0000 6ab1  X...j{...j....j.
-00007770: 0300 006a fe03 0000 6af8 0300 006a 0a04  ...j....j....j..
-00007780: 0000 6a04 0400 006a a904 0000 6a5e 0400  ..j....j....j^..
-00007790: 006a f106 0000 6aaf 0400 006a e906 0000  .j....j....j....
-000077a0: 6ae3 0600 0075 8c0d 666f 6f74 6e6f 7465  j....u..footnote
-000077b0: 5f72 6566 7394 7d94 8c0d 6369 7461 7469  _refs.}...citati
-000077c0: 6f6e 5f72 6566 7394 7d94 8c0d 6175 746f  on_refs.}...auto
-000077d0: 666f 6f74 6e6f 7465 7394 5d94 8c11 6175  footnotes.]...au
-000077e0: 746f 666f 6f74 6e6f 7465 5f72 6566 7394  tofootnote_refs.
-000077f0: 5d94 8c10 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
-00007800: 6f74 6573 945d 948c 1473 796d 626f 6c5f  otes.]...symbol_
-00007810: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
-00007820: 8c09 666f 6f74 6e6f 7465 7394 5d94 8c09  ..footnotes.]...
-00007830: 6369 7461 7469 6f6e 7394 5d94 8c12 6175  citations.]...au
-00007840: 746f 666f 6f74 6e6f 7465 5f73 7461 7274  tofootnote_start
-00007850: 944b 018c 1573 796d 626f 6c5f 666f 6f74  .K...symbol_foot
-00007860: 6e6f 7465 5f73 7461 7274 944b 008c 0869  note_start.K...i
-00007870: 645f 7374 6172 7494 4b03 8c0e 7061 7273  d_start.K...pars
-00007880: 655f 6d65 7373 6167 6573 945d 9428 6800  e_messages.].(h.
-00007890: 8c0e 7379 7374 656d 5f6d 6573 7361 6765  ..system_message
-000078a0: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-000078b0: 9468 3d29 8194 7d94 2868 058c 4344 7570  .h=)..}.(h..CDup
-000078c0: 6c69 6361 7465 2069 6d70 6c69 6369 7420  licate implicit 
-000078d0: 7461 7267 6574 206e 616d 653a 2022 7468  target name: "th
-000078e0: 6973 2069 7320 6120 6d61 6a6f 7220 6275  is is a major bu
-000078f0: 672d 6669 7820 7265 6c65 6173 652e 222e  g-fix release.".
-00007900: 9468 075d 9468 158c 4744 7570 6c69 6361  .h.].h..GDuplica
-00007910: 7465 2069 6d70 6c69 6369 7420 7461 7267  te implicit targ
-00007920: 6574 206e 616d 653a 20e2 809c 7468 6973  et name: ...this
-00007930: 2069 7320 6120 6d61 6a6f 7220 6275 672d   is a major bug-
-00007940: 6669 7820 7265 6c65 6173 652e e280 9d2e  fix release.....
-00007950: 9485 9481 947d 9428 6805 6806 681a 6a8b  .....}.(h.h.h.j.
-00007960: 0700 0075 6261 681d 7d94 2868 1f5d 9468  ...ubah.}.(h.].h
-00007970: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
-00007980: 6829 683c 681a 6a88 0700 0075 6261 681d  h)h<h.j....ubah.
-00007990: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-000079a0: 255d 9468 275d 946a 5901 0000 618c 056c  %].h'].jY...a..l
-000079b0: 6576 656c 944b 018c 0474 7970 6594 8c04  evel.K...type...
-000079c0: 494e 464f 948c 0673 6f75 7263 6594 682a  INFO...source.h*
-000079d0: 8c04 6c69 6e65 944b 2e75 6829 6a86 0700  ..line.K.uh)j...
-000079e0: 0068 1a6a 3801 0000 6801 6803 681b 682a  .h.j8...h.h.h.h*
-000079f0: 681c 4b2e 7562 6a87 0700 0029 8194 7d94  h.K.ubj....)..}.
-00007a00: 2868 0568 0668 075d 9468 3d29 8194 7d94  (h.h.h.].h=)..}.
-00007a10: 2868 058c 4344 7570 6c69 6361 7465 2069  (h..CDuplicate i
-00007a20: 6d70 6c69 6369 7420 7461 7267 6574 206e  mplicit target n
-00007a30: 616d 653a 2022 7468 6973 2069 7320 6120  ame: "this is a 
-00007a40: 6d61 6a6f 7220 6275 672d 6669 7820 7265  major bug-fix re
-00007a50: 6c65 6173 652e 222e 9468 075d 9468 158c  lease."..h.].h..
-00007a60: 4744 7570 6c69 6361 7465 2069 6d70 6c69  GDuplicate impli
-00007a70: 6369 7420 7461 7267 6574 206e 616d 653a  cit target name:
-00007a80: 20e2 809c 7468 6973 2069 7320 6120 6d61   ...this is a ma
-00007a90: 6a6f 7220 6275 672d 6669 7820 7265 6c65  jor bug-fix rele
-00007aa0: 6173 652e e280 9d2e 9485 9481 947d 9428  ase..........}.(
-00007ab0: 6805 6806 681a 6aa7 0700 0075 6261 681d  h.h.h.j....ubah.
-00007ac0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
-00007ad0: 255d 9468 275d 9475 6829 683c 681a 6aa4  %].h'].uh)h<h.j.
-00007ae0: 0700 0075 6261 681d 7d94 2868 1f5d 9468  ...ubah.}.(h.].h
-00007af0: 215d 9468 235d 9468 255d 9468 275d 946a  !].h#].h%].h'].j
-00007b00: 9801 0000 618c 056c 6576 656c 944b 018c  ....a..level.K..
-00007b10: 0474 7970 6594 6aa1 0700 008c 0673 6f75  .type.j......sou
-00007b20: 7263 6594 682a 8c04 6c69 6e65 944b 3775  rce.h*..line.K7u
-00007b30: 6829 6a86 0700 0068 1a6a 7701 0000 6801  h)j....h.jw...h.
-00007b40: 6803 681b 682a 681c 4b37 7562 658c 1274  h.h.h*h.K7ube..t
-00007b50: 7261 6e73 666f 726d 5f6d 6573 7361 6765  ransform_message
-00007b60: 7394 5d94 8c0b 7472 616e 7366 6f72 6d65  s.]...transforme
-00007b70: 7294 4e8c 0a64 6563 6f72 6174 696f 6e94  r.N..decoration.
-00007b80: 4e68 0168 0375 622e                      Nh.h.ub.
+00000a10: 2e39 2e32 2074 6f20 302e 392e 3394 6807  .9.2 to 0.9.3.h.
+00000a20: 5d94 6815 8c1b 4368 616e 6765 7320 6672  ].h...Changes fr
+00000a30: 6f6d 2030 2e39 2e32 2074 6f20 302e 392e  om 0.9.2 to 0.9.
+00000a40: 3394 8594 8194 7d94 2868 0568 d168 1a68  3.....}.(h.h.h.h
+00000a50: cf68 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
+00000a60: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00000a70: 255d 9468 275d 9475 6829 680e 681a 68cc  %].h'].uh)h.h.h.
+00000a80: 6801 6803 681b 682a 681c 4b20 7562 683d  h.h.h.h*h.K ubh=
+00000a90: 2981 947d 9428 6805 8c1a 7468 6973 2069  )..}.(h...this i
+00000aa0: 7320 6120 6275 672d 6669 7820 7265 6c65  s a bug-fix rele
+00000ab0: 6173 652e 9468 075d 9468 158c 1a74 6869  ase..h.].h...thi
+00000ac0: 7320 6973 2061 2062 7567 2d66 6978 2072  s is a bug-fix r
+00000ad0: 656c 6561 7365 2e94 8594 8194 7d94 2868  elease......}.(h
+00000ae0: 0568 df68 1a68 dd68 0168 0368 1b4e 681c  .h.h.h.h.h.h.Nh.
+00000af0: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+00000b00: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00000b10: 683c 681b 682a 681c 4b22 681a 68cc 6801  h<h.h*h.K"h.h.h.
+00000b20: 6803 7562 683d 2981 947d 9428 6805 8c60  h.ubh=)..}.(h..`
+00000b30: 6368 616e 6765 7320 696e 2076 6572 7369  changes in versi
+00000b40: 6f6e 2030 2e39 2e32 206c 6564 2074 6f20  on 0.9.2 led to 
+00000b50: 616e 2065 7272 6f72 2077 6865 7265 2069  an error where i
+00000b60: 6f6e 2e72 6563 6f6d 6252 6174 6520 6469  on.recombRate di
+00000b70: 6420 6e6f 7420 776f 726b 2e20 2054 6869  d not work.  Thi
+00000b80: 7320 6861 7320 6265 656e 2066 6978 6564  s has been fixed
+00000b90: 9468 075d 9468 158c 6063 6861 6e67 6573  .h.].h..`changes
+00000ba0: 2069 6e20 7665 7273 696f 6e20 302e 392e   in version 0.9.
+00000bb0: 3220 6c65 6420 746f 2061 6e20 6572 726f  2 led to an erro
+00000bc0: 7220 7768 6572 6520 696f 6e2e 7265 636f  r where ion.reco
+00000bd0: 6d62 5261 7465 2064 6964 206e 6f74 2077  mbRate did not w
+00000be0: 6f72 6b2e 2020 5468 6973 2068 6173 2062  ork.  This has b
+00000bf0: 6565 6e20 6669 7865 6494 8594 8194 7d94  een fixed.....}.
+00000c00: 2868 0568 ed68 1a68 eb68 0168 0368 1b4e  (h.h.h.h.h.h.h.N
+00000c10: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00000c20: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00000c30: 6829 683c 681b 682a 681c 4b24 681a 68cc  h)h<h.h*h.K$h.h.
+00000c40: 6801 6803 7562 6568 1d7d 9428 681f 5d94  h.h.ubeh.}.(h.].
+00000c50: 8c1b 6368 616e 6765 732d 6672 6f6d 2d30  ..changes-from-0
+00000c60: 2d39 2d32 2d74 6f2d 302d 392d 3394 6168  -9-2-to-0-9-3.ah
+00000c70: 215d 9468 235d 948c 1b63 6861 6e67 6573  !].h#]...changes
+00000c80: 2066 726f 6d20 302e 392e 3220 746f 2030   from 0.9.2 to 0
+00000c90: 2e39 2e33 9461 6825 5d94 6827 5d94 7568  .9.3.ah%].h'].uh
+00000ca0: 2968 0968 1a68 0b68 0168 0368 1b68 2a68  )h.h.h.h.h.h.h*h
+00000cb0: 1c4b 2075 6268 0a29 8194 7d94 2868 0568  .K ubh.)..}.(h.h
+00000cc0: 0668 075d 9428 680f 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00000cd0: 8c1b 4368 616e 6765 7320 6672 6f6d 2030  ..Changes from 0
+00000ce0: 2e39 2e31 2074 6f20 302e 392e 3294 6807  .9.1 to 0.9.2.h.
+00000cf0: 5d94 6815 8c1b 4368 616e 6765 7320 6672  ].h...Changes fr
+00000d00: 6f6d 2030 2e39 2e31 2074 6f20 302e 392e  om 0.9.1 to 0.9.
+00000d10: 3294 8594 8194 7d94 2868 056a 0601 0000  2.....}.(h.j....
+00000d20: 681a 6a04 0100 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+00000d30: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+00000d40: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00000d50: 680e 681a 6a01 0100 0068 0168 0368 1b68  h.h.j....h.h.h.h
+00000d60: 2a68 1c4b 2875 6268 3d29 8194 7d94 2868  *h.K(ubh=)..}.(h
+00000d70: 058c 1a74 6869 7320 6973 2061 2062 7567  ...this is a bug
+00000d80: 2d66 6978 2072 656c 6561 7365 2e94 6807  -fix release..h.
+00000d90: 5d94 6815 8c1a 7468 6973 2069 7320 6120  ].h...this is a 
+00000da0: 6275 672d 6669 7820 7265 6c65 6173 652e  bug-fix release.
+00000db0: 9485 9481 947d 9428 6805 6a14 0100 0068  .....}.(h.j....h
+00000dc0: 1a6a 1201 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+00000dd0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00000de0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+00000df0: 3c68 1b68 2a68 1c4b 2a68 1a6a 0101 0000  <h.h*h.K*h.j....
+00000e00: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
+00000e10: 8c6b 6368 616e 6765 7320 696e 2076 6572  .kchanges in ver
+00000e20: 7369 6f6e 2030 2e39 2e31 206c 6561 6420  sion 0.9.1 lead 
+00000e30: 746f 2061 6e20 6572 726f 7220 7768 6572  to an error wher
+00000e40: 6520 6120 6261 7265 2069 6f6e 2068 6173  e a bare ion has
+00000e50: 206e 6f74 2072 6563 6f6d 6269 6e61 7469   not recombinati
+00000e60: 6f6e 2072 6174 652e 2020 5468 6973 2068  on rate.  This h
+00000e70: 6173 2062 6565 6e20 6669 7865 6494 6807  as been fixed.h.
+00000e80: 5d94 6815 8c6b 6368 616e 6765 7320 696e  ].h..kchanges in
+00000e90: 2076 6572 7369 6f6e 2030 2e39 2e31 206c   version 0.9.1 l
+00000ea0: 6561 6420 746f 2061 6e20 6572 726f 7220  ead to an error 
+00000eb0: 7768 6572 6520 6120 6261 7265 2069 6f6e  where a bare ion
+00000ec0: 2068 6173 206e 6f74 2072 6563 6f6d 6269   has not recombi
+00000ed0: 6e61 7469 6f6e 2072 6174 652e 2020 5468  nation rate.  Th
+00000ee0: 6973 2068 6173 2062 6565 6e20 6669 7865  is has been fixe
+00000ef0: 6494 8594 8194 7d94 2868 056a 2201 0000  d.....}.(h.j"...
+00000f00: 681a 6a20 0100 0068 0168 0368 1b4e 681c  h.j ...h.h.h.Nh.
+00000f10: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+00000f20: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00000f30: 683c 681b 682a 681c 4b2c 681a 6a01 0100  h<h.h*h.K,h.j...
+00000f40: 0068 0168 0375 6265 681d 7d94 2868 1f5d  .h.h.ubeh.}.(h.]
+00000f50: 948c 1b63 6861 6e67 6573 2d66 726f 6d2d  ...changes-from-
+00000f60: 302d 392d 312d 746f 2d30 2d39 2d32 9461  0-9-1-to-0-9-2.a
+00000f70: 6821 5d94 6823 5d94 8c1b 6368 616e 6765  h!].h#]...change
+00000f80: 7320 6672 6f6d 2030 2e39 2e31 2074 6f20  s from 0.9.1 to 
+00000f90: 302e 392e 3294 6168 255d 9468 275d 9475  0.9.2.ah%].h'].u
+00000fa0: 6829 6809 681a 680b 6801 6803 681b 682a  h)h.h.h.h.h.h.h*
+00000fb0: 681c 4b28 7562 680a 2981 947d 9428 6805  h.K(ubh.)..}.(h.
+00000fc0: 6806 6807 5d94 2868 0f29 8194 7d94 2868  h.h.].(h.)..}.(h
+00000fd0: 058c 1b43 6861 6e67 6573 2066 726f 6d20  ...Changes from 
+00000fe0: 302e 392e 3020 746f 2030 2e39 2e31 9468  0.9.0 to 0.9.1.h
+00000ff0: 075d 9468 158c 1b43 6861 6e67 6573 2066  .].h...Changes f
+00001000: 726f 6d20 302e 392e 3020 746f 2030 2e39  rom 0.9.0 to 0.9
+00001010: 2e31 9485 9481 947d 9428 6805 6a3b 0100  .1.....}.(h.j;..
+00001020: 0068 1a6a 3901 0000 6801 6803 681b 4e68  .h.j9...h.h.h.Nh
+00001030: 1c4e 7562 6168 1d7d 9428 681f 5d94 6821  .Nubah.}.(h.].h!
+00001040: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
+00001050: 2968 0e68 1a6a 3601 0000 6801 6803 681b  )h.h.j6...h.h.h.
+00001060: 682a 681c 4b30 7562 683d 2981 947d 9428  h*h.K0ubh=)..}.(
+00001070: 6805 8c1a 7468 6973 2069 7320 6120 6275  h...this is a bu
+00001080: 672d 6669 7820 7265 6c65 6173 652e 9468  g-fix release..h
+00001090: 075d 9468 158c 1a74 6869 7320 6973 2061  .].h...this is a
+000010a0: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
+000010b0: 2e94 8594 8194 7d94 2868 056a 4901 0000  ......}.(h.jI...
+000010c0: 681a 6a47 0100 0068 0168 0368 1b4e 681c  h.jG...h.h.h.Nh.
+000010d0: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+000010e0: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+000010f0: 683c 681b 682a 681c 4b32 681a 6a36 0100  h<h.h*h.K2h.j6..
+00001100: 0068 0168 0375 6268 3d29 8194 7d94 2868  .h.h.ubh=)..}.(h
+00001110: 058c 8869 6e20 6361 7365 7320 7768 656e  ...in cases when
+00001120: 2069 7420 6973 206e 6f74 2070 6f73 7369   it is not possi
+00001130: 626c 6520 746f 2063 616c 6375 6c61 7465  ble to calculate
+00001140: 2074 6865 2066 7265 652d 626f 756e 6420   the free-bound 
+00001150: 636f 6e74 696e 7575 6d20 666f 7220 736f  continuum for so
+00001160: 6d65 2069 6f6e 2c20 6d73 7065 6374 7275  me ion, mspectru
+00001170: 6d20 6469 6420 6e6f 7420 6861 6e64 6c65  m did not handle
+00001180: 2074 6869 7320 636f 7272 6563 746c 7920   this correctly 
+00001190: 616e 6420 6372 6173 6865 6494 6807 5d94  and crashed.h.].
+000011a0: 6815 8c88 696e 2063 6173 6573 2077 6865  h...in cases whe
+000011b0: 6e20 6974 2069 7320 6e6f 7420 706f 7373  n it is not poss
+000011c0: 6962 6c65 2074 6f20 6361 6c63 756c 6174  ible to calculat
+000011d0: 6520 7468 6520 6672 6565 2d62 6f75 6e64  e the free-bound
+000011e0: 2063 6f6e 7469 6e75 756d 2066 6f72 2073   continuum for s
+000011f0: 6f6d 6520 696f 6e2c 206d 7370 6563 7472  ome ion, mspectr
+00001200: 756d 2064 6964 206e 6f74 2068 616e 646c  um did not handl
+00001210: 6520 7468 6973 2063 6f72 7265 6374 6c79  e this correctly
+00001220: 2061 6e64 2063 7261 7368 6564 9485 9481   and crashed....
+00001230: 947d 9428 6805 6a57 0100 0068 1a6a 5501  .}.(h.jW...h.jU.
+00001240: 0000 6801 6803 681b 4e68 1c4e 7562 6168  ..h.h.h.Nh.Nubah
+00001250: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00001260: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
+00001270: 2a68 1c4b 3468 1a6a 3601 0000 6801 6803  *h.K4h.j6...h.h.
+00001280: 7562 683d 2981 947d 9428 6805 8c7a 616c  ubh=)..}.(h..zal
+00001290: 736f 2c20 7468 6520 696f 6e20 7a6e 5f33  so, the ion zn_3
+000012a0: 3120 285a 6e20 5858 5849 2920 6973 2061  1 (Zn XXXI) is a
+000012b0: 2062 6172 6520 696f 6e20 616e 6420 6861   bare ion and ha
+000012c0: 7320 6e6f 2069 6f6e 697a 6174 696f 6e20  s no ionization 
+000012d0: 706f 7465 6e74 6961 6c20 2849 5029 2061  potential (IP) a
+000012e0: 6e64 206c 6f6f 6b69 6e67 2069 7420 7570  nd looking it up
+000012f0: 2063 6175 7365 6420 696e 6465 7869 6e67   caused indexing
+00001300: 2065 7272 6f72 732e 9468 075d 9468 158c   errors..h.].h..
+00001310: 7a61 6c73 6f2c 2074 6865 2069 6f6e 207a  zalso, the ion z
+00001320: 6e5f 3331 2028 5a6e 2058 5858 4929 2069  n_31 (Zn XXXI) i
+00001330: 7320 6120 6261 7265 2069 6f6e 2061 6e64  s a bare ion and
+00001340: 2068 6173 206e 6f20 696f 6e69 7a61 7469   has no ionizati
+00001350: 6f6e 2070 6f74 656e 7469 616c 2028 4950  on potential (IP
+00001360: 2920 616e 6420 6c6f 6f6b 696e 6720 6974  ) and looking it
+00001370: 2075 7020 6361 7573 6564 2069 6e64 6578   up caused index
+00001380: 696e 6720 6572 726f 7273 2e94 8594 8194  ing errors......
+00001390: 7d94 2868 056a 6501 0000 681a 6a63 0100  }.(h.je...h.jc..
+000013a0: 0068 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
+000013b0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+000013c0: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
+000013d0: 681c 4b36 681a 6a36 0100 0068 0168 0375  h.K6h.j6...h.h.u
+000013e0: 6265 681d 7d94 2868 1f5d 948c 1b63 6861  beh.}.(h.]...cha
+000013f0: 6e67 6573 2d66 726f 6d2d 302d 392d 302d  nges-from-0-9-0-
+00001400: 746f 2d30 2d39 2d31 9461 6821 5d94 6823  to-0-9-1.ah!].h#
+00001410: 5d94 8c1b 6368 616e 6765 7320 6672 6f6d  ]...changes from
+00001420: 2030 2e39 2e30 2074 6f20 302e 392e 3194   0.9.0 to 0.9.1.
+00001430: 6168 255d 9468 275d 9475 6829 6809 681a  ah%].h'].uh)h.h.
+00001440: 680b 6801 6803 681b 682a 681c 4b30 7562  h.h.h.h.h*h.K0ub
+00001450: 680a 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+00001460: 2868 0f29 8194 7d94 2868 058c 1b43 6861  (h.)..}.(h...Cha
+00001470: 6e67 6573 2066 726f 6d20 302e 382e 3720  nges from 0.8.7 
+00001480: 746f 2030 2e39 2e30 9468 075d 9468 158c  to 0.9.0.h.].h..
+00001490: 1b43 6861 6e67 6573 2066 726f 6d20 302e  .Changes from 0.
+000014a0: 382e 3720 746f 2030 2e39 2e30 9485 9481  8.7 to 0.9.0....
+000014b0: 947d 9428 6805 6a7e 0100 0068 1a6a 7c01  .}.(h.j~...h.j|.
+000014c0: 0000 6801 6803 681b 4e68 1c4e 7562 6168  ..h.h.h.Nh.Nubah
+000014d0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+000014e0: 6825 5d94 6827 5d94 7568 2968 0e68 1a6a  h%].h'].uh)h.h.j
+000014f0: 7901 0000 6801 6803 681b 682a 681c 4b3a  y...h.h.h.h*h.K:
+00001500: 7562 683d 2981 947d 9428 6805 8c27 6120  ubh=)..}.(h..'a 
+00001510: 6e65 7720 6d6f 6475 6c65 206d 6f64 656c  new module model
+00001520: 2e6d 616b 6572 2068 6173 2062 6565 6e20  .maker has been 
+00001530: 6164 6465 6494 6807 5d94 6815 8c27 6120  added.h.].h..'a 
+00001540: 6e65 7720 6d6f 6475 6c65 206d 6f64 656c  new module model
+00001550: 2e6d 616b 6572 2068 6173 2062 6565 6e20  .maker has been 
+00001560: 6164 6465 6494 8594 8194 7d94 2868 056a  added.....}.(h.j
+00001570: 8c01 0000 681a 6a8a 0100 0068 0168 0368  ....h.j....h.h.h
+00001580: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+00001590: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+000015a0: 9475 6829 683c 681b 682a 681c 4b3c 681a  .uh)h<h.h*h.K<h.
+000015b0: 6a79 0100 0068 0168 0375 6268 008c 0d6c  jy...h.h.ubh...l
+000015c0: 6974 6572 616c 5f62 6c6f 636b 9493 9429  iteral_block...)
+000015d0: 8194 7d94 2868 058c 3669 6d70 6f72 7420  ..}.(h..6import 
+000015e0: 4368 6961 6e74 6950 792e 6d6f 6465 6c20  ChiantiPy.model 
+000015f0: 6173 206d 646c 0a6d 796d 6f64 656c 203d  as mdl.mymodel =
+00001600: 206d 646c 2e6d 616b 6572 282e 2e2e 2994   mdl.maker(...).
+00001610: 6807 5d94 6815 8c36 696d 706f 7274 2043  h.].h..6import C
+00001620: 6869 616e 7469 5079 2e6d 6f64 656c 2061  hiantiPy.model a
+00001630: 7320 6d64 6c0a 6d79 6d6f 6465 6c20 3d20  s mdl.mymodel = 
+00001640: 6d64 6c2e 6d61 6b65 7228 2e2e 2e29 9485  mdl.maker(...)..
+00001650: 9481 947d 9428 6805 6806 681a 6a9a 0100  ...}.(h.h.h.j...
+00001660: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
+00001670: 9468 235d 9468 255d 9468 275d 948c 0978  .h#].h%].h']...x
+00001680: 6d6c 3a73 7061 6365 948c 0870 7265 7365  ml:space...prese
+00001690: 7276 6594 7568 296a 9801 0000 681c 4b40  rve.uh)j....h.K@
+000016a0: 681a 6a79 0100 0068 0168 0368 1b68 2a75  h.jy...h.h.h.h*u
+000016b0: 6268 3d29 8194 7d94 2868 058c 5961 2073  bh=)..}.(h..Ya s
+000016c0: 6572 696f 7573 2062 7567 2069 6e20 6368  erious bug in ch
+000016d0: 2e66 7265 6542 6f75 6e64 2077 6173 2066  .freeBound was f
+000016e0: 6978 6564 202d 2074 6865 2075 7365 206f  ixed - the use o
+000016f0: 6620 6120 7369 6e67 6c65 2074 656d 7065  f a single tempe
+00001700: 7261 7475 7265 2077 6173 2070 726f 626c  rature was probl
+00001710: 656d 6174 6963 9468 075d 9468 158c 5961  ematic.h.].h..Ya
+00001720: 2073 6572 696f 7573 2062 7567 2069 6e20   serious bug in 
+00001730: 6368 2e66 7265 6542 6f75 6e64 2077 6173  ch.freeBound was
+00001740: 2066 6978 6564 202d 2074 6865 2075 7365   fixed - the use
+00001750: 206f 6620 6120 7369 6e67 6c65 2074 656d   of a single tem
+00001760: 7065 7261 7475 7265 2077 6173 2070 726f  perature was pro
+00001770: 626c 656d 6174 6963 9485 9481 947d 9428  blematic.....}.(
+00001780: 6805 6aac 0100 0068 1a6a aa01 0000 6801  h.j....h.j....h.
+00001790: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
+000017a0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+000017b0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
+000017c0: 4468 1a6a 7901 0000 6801 6803 7562 6568  Dh.jy...h.h.ubeh
+000017d0: 1d7d 9428 681f 5d94 8c1b 6368 616e 6765  .}.(h.]...change
+000017e0: 732d 6672 6f6d 2d30 2d38 2d37 2d74 6f2d  s-from-0-8-7-to-
+000017f0: 302d 392d 3094 6168 215d 9468 235d 948c  0-9-0.ah!].h#]..
+00001800: 1b63 6861 6e67 6573 2066 726f 6d20 302e  .changes from 0.
+00001810: 382e 3720 746f 2030 2e39 2e30 9461 6825  8.7 to 0.9.0.ah%
+00001820: 5d94 6827 5d94 7568 2968 0968 1a68 0b68  ].h'].uh)h.h.h.h
+00001830: 0168 0368 1b68 2a68 1c4b 3a75 6268 0a29  .h.h.h*h.K:ubh.)
+00001840: 8194 7d94 2868 0568 0668 075d 9428 680f  ..}.(h.h.h.].(h.
+00001850: 2981 947d 9428 6805 8c1b 4368 616e 6765  )..}.(h...Change
+00001860: 7320 6672 6f6d 2030 2e38 2e36 2074 6f20  s from 0.8.6 to 
+00001870: 302e 382e 3794 6807 5d94 6815 8c1b 4368  0.8.7.h.].h...Ch
+00001880: 616e 6765 7320 6672 6f6d 2030 2e38 2e36  anges from 0.8.6
+00001890: 2074 6f20 302e 382e 3794 8594 8194 7d94   to 0.8.7.....}.
+000018a0: 2868 056a c501 0000 681a 6ac3 0100 0068  (h.j....h.j....h
+000018b0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
+000018c0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
+000018d0: 9468 275d 9475 6829 680e 681a 6ac0 0100  .h'].uh)h.h.j...
+000018e0: 0068 0168 0368 1b68 2a68 1c4b 4775 6268  .h.h.h.h*h.KGubh
+000018f0: 3d29 8194 7d94 2868 058c 1663 6f6e 7469  =)..}.(h...conti
+00001900: 6e75 6564 2063 6f64 6520 636c 6561 6e75  nued code cleanu
+00001910: 7094 6807 5d94 6815 8c16 636f 6e74 696e  p.h.].h...contin
+00001920: 7565 6420 636f 6465 2063 6c65 616e 7570  ued code cleanup
+00001930: 9485 9481 947d 9428 6805 6ad3 0100 0068  .....}.(h.j....h
+00001940: 1a6a d101 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+00001950: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00001960: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+00001970: 3c68 1b68 2a68 1c4b 4968 1a6a c001 0000  <h.h*h.KIh.j....
+00001980: 6801 6803 7562 6568 1d7d 9428 681f 5d94  h.h.ubeh.}.(h.].
+00001990: 8c1b 6368 616e 6765 732d 6672 6f6d 2d30  ..changes-from-0
+000019a0: 2d38 2d36 2d74 6f2d 302d 382d 3794 6168  -8-6-to-0-8-7.ah
+000019b0: 215d 9468 235d 948c 1b63 6861 6e67 6573  !].h#]...changes
+000019c0: 2066 726f 6d20 302e 382e 3620 746f 2030   from 0.8.6 to 0
+000019d0: 2e38 2e37 9461 6825 5d94 6827 5d94 7568  .8.7.ah%].h'].uh
+000019e0: 2968 0968 1a68 0b68 0168 0368 1b68 2a68  )h.h.h.h.h.h.h*h
+000019f0: 1c4b 4775 6268 0a29 8194 7d94 2868 0568  .KGubh.)..}.(h.h
+00001a00: 0668 075d 9428 680f 2981 947d 9428 6805  .h.].(h.)..}.(h.
+00001a10: 8c1b 4368 616e 6765 7320 6672 6f6d 2030  ..Changes from 0
+00001a20: 2e38 2e35 2074 6f20 302e 382e 3694 6807  .8.5 to 0.8.6.h.
+00001a30: 5d94 6815 8c1b 4368 616e 6765 7320 6672  ].h...Changes fr
+00001a40: 6f6d 2030 2e38 2e35 2074 6f20 302e 382e  om 0.8.5 to 0.8.
+00001a50: 3694 8594 8194 7d94 2868 056a ec01 0000  6.....}.(h.j....
+00001a60: 681a 6aea 0100 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+00001a70: 4e75 6261 681d 7d94 2868 1f5d 9468 215d  Nubah.}.(h.].h!]
+00001a80: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00001a90: 680e 681a 6ae7 0100 0068 0168 0368 1b68  h.h.j....h.h.h.h
+00001aa0: 2a68 1c4b 4d75 6268 3d29 8194 7d94 2868  *h.KMubh=)..}.(h
+00001ab0: 058c 1761 6e6f 7468 6572 2062 7567 2d66  ...another bug-f
+00001ac0: 6978 2072 656c 6561 7365 9468 075d 9468  ix release.h.].h
+00001ad0: 158c 1761 6e6f 7468 6572 2062 7567 2d66  ...another bug-f
+00001ae0: 6978 2072 656c 6561 7365 9485 9481 947d  ix release.....}
+00001af0: 9428 6805 6afa 0100 0068 1a6a f801 0000  .(h.j....h.j....
+00001b00: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
+00001b10: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
+00001b20: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
+00001b30: 1c4b 4f68 1a6a e701 0000 6801 6803 7562  .KOh.j....h.h.ub
+00001b40: 683d 2981 947d 9428 6805 8c6a 6164 6465  h=)..}.(h..jadde
+00001b50: 6420 6172 6743 6865 636b 206d 6574 686f  d argCheck metho
+00001b60: 6420 746f 206d 616b 6520 7375 7265 2074  d to make sure t
+00001b70: 6861 7420 7369 7a65 7320 6f66 2074 656d  hat sizes of tem
+00001b80: 7065 7261 7475 7265 2c20 6465 6e73 6974  perature, densit
+00001b90: 7920 616e 6420 656d 6973 7369 6f6e 206d  y and emission m
+00001ba0: 6561 7375 7265 2077 6572 6520 636f 6d70  easure were comp
+00001bb0: 6174 6962 6c65 9468 075d 9468 158c 6a61  atible.h.].h..ja
+00001bc0: 6464 6564 2061 7267 4368 6563 6b20 6d65  dded argCheck me
+00001bd0: 7468 6f64 2074 6f20 6d61 6b65 2073 7572  thod to make sur
+00001be0: 6520 7468 6174 2073 697a 6573 206f 6620  e that sizes of 
+00001bf0: 7465 6d70 6572 6174 7572 652c 2064 656e  temperature, den
+00001c00: 7369 7479 2061 6e64 2065 6d69 7373 696f  sity and emissio
+00001c10: 6e20 6d65 6173 7572 6520 7765 7265 2063  n measure were c
+00001c20: 6f6d 7061 7469 626c 6594 8594 8194 7d94  ompatible.....}.
+00001c30: 2868 056a 0802 0000 681a 6a06 0200 0068  (h.j....h.j....h
+00001c40: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
+00001c50: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
+00001c60: 9468 275d 9475 6829 683c 681b 682a 681c  .h'].uh)h<h.h*h.
+00001c70: 4b51 681a 6ae7 0100 0068 0168 0375 6265  KQh.j....h.h.ube
+00001c80: 681d 7d94 2868 1f5d 948c 1b63 6861 6e67  h.}.(h.]...chang
+00001c90: 6573 2d66 726f 6d2d 302d 382d 352d 746f  es-from-0-8-5-to
+00001ca0: 2d30 2d38 2d36 9461 6821 5d94 6823 5d94  -0-8-6.ah!].h#].
+00001cb0: 8c1b 6368 616e 6765 7320 6672 6f6d 2030  ..changes from 0
+00001cc0: 2e38 2e35 2074 6f20 302e 382e 3694 6168  .8.5 to 0.8.6.ah
+00001cd0: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
+00001ce0: 6801 6803 681b 682a 681c 4b4d 7562 680a  h.h.h.h*h.KMubh.
+00001cf0: 2981 947d 9428 6805 6806 6807 5d94 680f  )..}.(h.h.h.].h.
+00001d00: 2981 947d 9428 6805 8c1b 4368 616e 6765  )..}.(h...Change
+00001d10: 7320 6672 6f6d 2030 2e38 2e34 2074 6f20  s from 0.8.4 to 
+00001d20: 302e 382e 3594 6807 5d94 6815 8c1b 4368  0.8.5.h.].h...Ch
+00001d30: 616e 6765 7320 6672 6f6d 2030 2e38 2e34  anges from 0.8.4
+00001d40: 2074 6f20 302e 382e 3594 8594 8194 7d94   to 0.8.5.....}.
+00001d50: 2868 056a 2102 0000 681a 6a1f 0200 0068  (h.j!...h.j....h
+00001d60: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
+00001d70: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
+00001d80: 9468 275d 9475 6829 680e 681a 6a1c 0200  .h'].uh)h.h.j...
+00001d90: 0068 0168 0368 1b68 2a68 1c4b 5475 6261  .h.h.h.h*h.KTuba
+00001da0: 681d 7d94 2868 1f5d 948c 1b63 6861 6e67  h.}.(h.]...chang
+00001db0: 6573 2d66 726f 6d2d 302d 382d 342d 746f  es-from-0-8-4-to
+00001dc0: 2d30 2d38 2d35 9461 6821 5d94 6823 5d94  -0-8-5.ah!].h#].
+00001dd0: 8c1b 6368 616e 6765 7320 6672 6f6d 2030  ..changes from 0
+00001de0: 2e38 2e34 2074 6f20 302e 382e 3594 6168  .8.4 to 0.8.5.ah
+00001df0: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
+00001e00: 6801 6803 681b 682a 681c 4b54 7562 680a  h.h.h.h*h.KTubh.
+00001e10: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00001e20: 0f29 8194 7d94 2868 058c 2054 6869 7320  .)..}.(h.. This 
+00001e30: 6973 2061 206d 616a 6f72 2062 7567 2d66  is a major bug-f
+00001e40: 6978 2072 656c 6561 7365 2e94 6807 5d94  ix release..h.].
+00001e50: 6815 8c20 5468 6973 2069 7320 6120 6d61  h.. This is a ma
+00001e60: 6a6f 7220 6275 672d 6669 7820 7265 6c65  jor bug-fix rele
+00001e70: 6173 652e 9485 9481 947d 9428 6805 6a3a  ase......}.(h.j:
+00001e80: 0200 0068 1a6a 3802 0000 6801 6803 681b  ...h.j8...h.h.h.
+00001e90: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
+00001ea0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00001eb0: 7568 2968 0e68 1a6a 3502 0000 6801 6803  uh)h.h.j5...h.h.
+00001ec0: 681b 682a 681c 4b57 7562 683d 2981 947d  h.h*h.KWubh=)..}
+00001ed0: 9428 6805 8c36 4572 726f 7273 2069 6e20  .(h..6Errors in 
+00001ee0: 6361 6c63 756c 6174 696e 6720 7468 6520  calculating the 
+00001ef0: 7072 6f74 6f6e 2072 6174 6573 2077 6572  proton rates wer
+00001f00: 6520 636f 7272 6563 7465 642e 9468 075d  e corrected..h.]
+00001f10: 9468 158c 3645 7272 6f72 7320 696e 2063  .h..6Errors in c
+00001f20: 616c 6375 6c61 7469 6e67 2074 6865 2070  alculating the p
+00001f30: 726f 746f 6e20 7261 7465 7320 7765 7265  roton rates were
+00001f40: 2063 6f72 7265 6374 6564 2e94 8594 8194   corrected......
+00001f50: 7d94 2868 056a 4802 0000 681a 6a46 0200  }.(h.jH...h.jF..
+00001f60: 0068 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
+00001f70: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00001f80: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
+00001f90: 681c 4b59 681a 6a35 0200 0068 0168 0375  h.KYh.j5...h.h.u
+00001fa0: 6268 3d29 8194 7d94 2868 058c 3341 6c6c  bh=)..}.(h..3All
+00001fb0: 2074 656d 7065 7261 7475 7265 7320 616e   temperatures an
+00001fc0: 6420 6465 6e73 6974 6965 7320 6172 6520  d densities are 
+00001fd0: 6e6f 7720 6e75 6d70 7920 6172 7261 7973  now numpy arrays
+00001fe0: 9468 075d 9468 158c 3341 6c6c 2074 656d  .h.].h..3All tem
+00001ff0: 7065 7261 7475 7265 7320 616e 6420 6465  peratures and de
+00002000: 6e73 6974 6965 7320 6172 6520 6e6f 7720  nsities are now 
+00002010: 6e75 6d70 7920 6172 7261 7973 9485 9481  numpy arrays....
+00002020: 947d 9428 6805 6a56 0200 0068 1a6a 5402  .}.(h.jV...h.jT.
+00002030: 0000 6801 6803 681b 4e68 1c4e 7562 6168  ..h.h.h.Nh.Nubah
+00002040: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00002050: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
+00002060: 2a68 1c4b 5b68 1a6a 3502 0000 6801 6803  *h.K[h.j5...h.h.
+00002070: 7562 6568 1d7d 9428 681f 5d94 8c1f 7468  ubeh.}.(h.]...th
+00002080: 6973 2d69 732d 612d 6d61 6a6f 722d 6275  is-is-a-major-bu
+00002090: 672d 6669 782d 7265 6c65 6173 6594 6168  g-fix-release.ah
+000020a0: 215d 9468 235d 9468 255d 948c 2074 6869  !].h#].h%].. thi
+000020b0: 7320 6973 2061 206d 616a 6f72 2062 7567  s is a major bug
+000020c0: 2d66 6978 2072 656c 6561 7365 2e94 6168  -fix release..ah
+000020d0: 275d 9475 6829 6809 681a 680b 6801 6803  '].uh)h.h.h.h.h.
+000020e0: 681b 682a 681c 4b57 8c0a 7265 6665 7265  h.h*h.KW..refere
+000020f0: 6e63 6564 944b 0175 6268 0a29 8194 7d94  nced.K.ubh.)..}.
+00002100: 2868 0568 0668 075d 9468 0f29 8194 7d94  (h.h.h.].h.)..}.
+00002110: 2868 058c 1b43 6861 6e67 6573 2066 726f  (h...Changes fro
+00002120: 6d20 302e 382e 3320 746f 2030 2e38 2e34  m 0.8.3 to 0.8.4
+00002130: 9468 075d 9468 158c 1b43 6861 6e67 6573  .h.].h...Changes
+00002140: 2066 726f 6d20 302e 382e 3320 746f 2030   from 0.8.3 to 0
+00002150: 2e38 2e34 9485 9481 947d 9428 6805 6a70  .8.4.....}.(h.jp
+00002160: 0200 0068 1a6a 6e02 0000 6801 6803 681b  ...h.jn...h.h.h.
+00002170: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
+00002180: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00002190: 7568 2968 0e68 1a6a 6b02 0000 6801 6803  uh)h.h.jk...h.h.
+000021a0: 681b 682a 681c 4b5f 7562 6168 1d7d 9428  h.h*h.K_ubah.}.(
+000021b0: 681f 5d94 8c1b 6368 616e 6765 732d 6672  h.]...changes-fr
+000021c0: 6f6d 2d30 2d38 2d33 2d74 6f2d 302d 382d  om-0-8-3-to-0-8-
+000021d0: 3494 6168 215d 9468 235d 948c 1b63 6861  4.ah!].h#]...cha
+000021e0: 6e67 6573 2066 726f 6d20 302e 382e 3320  nges from 0.8.3 
+000021f0: 746f 2030 2e38 2e34 9461 6825 5d94 6827  to 0.8.4.ah%].h'
+00002200: 5d94 7568 2968 0968 1a68 0b68 0168 0368  ].uh)h.h.h.h.h.h
+00002210: 1b68 2a68 1c4b 5f75 6268 0a29 8194 7d94  .h*h.K_ubh.)..}.
+00002220: 2868 0568 0668 075d 9428 680f 2981 947d  (h.h.h.].(h.)..}
+00002230: 9428 6805 8c20 5468 6973 2069 7320 6120  .(h.. This is a 
+00002240: 6d61 6a6f 7220 6275 672d 6669 7820 7265  major bug-fix re
+00002250: 6c65 6173 652e 9468 075d 9468 158c 2054  lease..h.].h.. T
+00002260: 6869 7320 6973 2061 206d 616a 6f72 2062  his is a major b
+00002270: 7567 2d66 6978 2072 656c 6561 7365 2e94  ug-fix release..
+00002280: 8594 8194 7d94 2868 056a 8902 0000 681a  ....}.(h.j....h.
+00002290: 6a87 0200 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+000022a0: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
+000022b0: 235d 9468 255d 9468 275d 9475 6829 680e  #].h%].h'].uh)h.
+000022c0: 681a 6a84 0200 0068 0168 0368 1b68 2a68  h.j....h.h.h.h*h
+000022d0: 1c4b 6275 6268 3d29 8194 7d94 2868 058c  .Kbubh=)..}.(h..
+000022e0: 4741 6e6f 7468 6572 2073 6967 6e69 6669  GAnother signifi
+000022f0: 6361 6e74 2062 7567 2077 6173 2066 6978  cant bug was fix
+00002300: 6564 2069 6e20 7468 6520 696d 706f 7274  ed in the import
+00002310: 616e 7420 696f 6e2e 706f 7075 6c61 7465  ant ion.populate
+00002320: 206d 6574 686f 642e 9468 075d 9468 158c   method..h.].h..
+00002330: 4741 6e6f 7468 6572 2073 6967 6e69 6669  GAnother signifi
+00002340: 6361 6e74 2062 7567 2077 6173 2066 6978  cant bug was fix
+00002350: 6564 2069 6e20 7468 6520 696d 706f 7274  ed in the import
+00002360: 616e 7420 696f 6e2e 706f 7075 6c61 7465  ant ion.populate
+00002370: 206d 6574 686f 642e 9485 9481 947d 9428   method......}.(
+00002380: 6805 6a97 0200 0068 1a6a 9502 0000 6801  h.j....h.j....h.
+00002390: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
+000023a0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+000023b0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
+000023c0: 6468 1a6a 8402 0000 6801 6803 7562 6568  dh.j....h.h.ubeh
+000023d0: 1d7d 9428 681f 5d94 8c03 6964 3194 6168  .}.(h.]...id1.ah
+000023e0: 215d 9468 235d 9468 255d 946a 6802 0000  !].h#].h%].jh...
+000023f0: 6168 275d 9475 6829 6809 681a 680b 6801  ah'].uh)h.h.h.h.
+00002400: 6803 681b 682a 681c 4b62 6a6a 0200 004b  h.h.h*h.Kbjj...K
+00002410: 0175 6268 0a29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
+00002420: 075d 9468 0f29 8194 7d94 2868 058c 1b43  .].h.)..}.(h...C
+00002430: 6861 6e67 6573 2066 726f 6d20 302e 372e  hanges from 0.7.
+00002440: 3120 746f 2030 2e38 2e33 9468 075d 9468  1 to 0.8.3.h.].h
+00002450: 158c 1b43 6861 6e67 6573 2066 726f 6d20  ...Changes from 
+00002460: 302e 372e 3120 746f 2030 2e38 2e33 9485  0.7.1 to 0.8.3..
+00002470: 9481 947d 9428 6805 6aaf 0200 0068 1a6a  ...}.(h.j....h.j
+00002480: ad02 0000 6801 6803 681b 4e68 1c4e 7562  ....h.h.h.Nh.Nub
+00002490: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+000024a0: 5d94 6825 5d94 6827 5d94 7568 2968 0e68  ].h%].h'].uh)h.h
+000024b0: 1a6a aa02 0000 6801 6803 681b 682a 681c  .j....h.h.h.h*h.
+000024c0: 4b68 7562 6168 1d7d 9428 681f 5d94 8c1b  Khubah.}.(h.]...
+000024d0: 6368 616e 6765 732d 6672 6f6d 2d30 2d37  changes-from-0-7
+000024e0: 2d31 2d74 6f2d 302d 382d 3394 6168 215d  -1-to-0-8-3.ah!]
+000024f0: 9468 235d 948c 1b63 6861 6e67 6573 2066  .h#]...changes f
+00002500: 726f 6d20 302e 372e 3120 746f 2030 2e38  rom 0.7.1 to 0.8
+00002510: 2e33 9461 6825 5d94 6827 5d94 7568 2968  .3.ah%].h'].uh)h
+00002520: 0968 1a68 0b68 0168 0368 1b68 2a68 1c4b  .h.h.h.h.h.h*h.K
+00002530: 6875 6268 0a29 8194 7d94 2868 0568 0668  hubh.)..}.(h.h.h
+00002540: 075d 9428 680f 2981 947d 9428 6805 8c20  .].(h.)..}.(h.. 
+00002550: 5468 6973 2069 7320 6120 6d61 6a6f 7220  This is a major 
+00002560: 6275 672d 6669 7820 7265 6c65 6173 652e  bug-fix release.
+00002570: 9468 075d 9468 158c 2054 6869 7320 6973  .h.].h.. This is
+00002580: 2061 206d 616a 6f72 2062 7567 2d66 6978   a major bug-fix
+00002590: 2072 656c 6561 7365 2e94 8594 8194 7d94   release......}.
+000025a0: 2868 056a c802 0000 681a 6ac6 0200 0068  (h.j....h.j....h
+000025b0: 0168 0368 1b4e 681c 4e75 6261 681d 7d94  .h.h.Nh.Nubah.}.
+000025c0: 2868 1f5d 9468 215d 9468 235d 9468 255d  (h.].h!].h#].h%]
+000025d0: 9468 275d 9475 6829 680e 681a 6ac3 0200  .h'].uh)h.h.j...
+000025e0: 0068 0168 0368 1b68 2a68 1c4b 6b75 6268  .h.h.h.h*h.Kkubh
+000025f0: 3d29 8194 7d94 2868 058c 4661 2073 6d61  =)..}.(h..Fa sma
+00002600: 6c6c 2062 7574 206d 6967 6874 7920 6275  ll but mighty bu
+00002610: 6720 7761 7320 666f 756e 6420 696e 2074  g was found in t
+00002620: 6865 2069 6d70 6f72 7461 6e74 2069 6f6e  he important ion
+00002630: 2e70 6f70 756c 6174 6520 6d65 7468 6f64  .populate method
+00002640: 2e94 6807 5d94 6815 8c46 6120 736d 616c  ..h.].h..Fa smal
+00002650: 6c20 6275 7420 6d69 6768 7479 2062 7567  l but mighty bug
+00002660: 2077 6173 2066 6f75 6e64 2069 6e20 7468   was found in th
+00002670: 6520 696d 706f 7274 616e 7420 696f 6e2e  e important ion.
+00002680: 706f 7075 6c61 7465 206d 6574 686f 642e  populate method.
+00002690: 9485 9481 947d 9428 6805 6ad6 0200 0068  .....}.(h.j....h
+000026a0: 1a6a d402 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+000026b0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+000026c0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+000026d0: 3c68 1b68 2a68 1c4b 6d68 1a6a c302 0000  <h.h*h.Kmh.j....
+000026e0: 6801 6803 7562 6568 1d7d 9428 681f 5d94  h.h.ubeh.}.(h.].
+000026f0: 8c03 6964 3294 6168 215d 9468 235d 9468  ..id2.ah!].h#].h
+00002700: 255d 948c 2074 6869 7320 6973 2061 206d  %].. this is a m
+00002710: 616a 6f72 2062 7567 2d66 6978 2072 656c  ajor bug-fix rel
+00002720: 6561 7365 2e94 6168 275d 9475 6829 6809  ease..ah'].uh)h.
+00002730: 681a 680b 6801 6803 681b 682a 681c 4b6b  h.h.h.h.h.h*h.Kk
+00002740: 6a6a 0200 004b 0175 6268 0a29 8194 7d94  jj...K.ubh.)..}.
+00002750: 2868 0568 0668 075d 9428 680f 2981 947d  (h.h.h.].(h.)..}
+00002760: 9428 6805 8c52 5665 7273 696f 6e20 302e  .(h..RVersion 0.
+00002770: 382e 7820 6669 6c65 7320 6172 6520 6e65  8.x files are ne
+00002780: 6365 7373 6172 7920 746f 2075 7365 2077  cessary to use w
+00002790: 6974 6820 7468 6520 6e65 7720 4348 4941  ith the new CHIA
+000027a0: 4e54 4920 5665 7273 696f 6e20 392e 3020  NTI Version 9.0 
+000027b0: 6461 7461 6261 7365 9468 075d 9468 158c  database.h.].h..
+000027c0: 5256 6572 7369 6f6e 2030 2e38 2e78 2066  RVersion 0.8.x f
+000027d0: 696c 6573 2061 7265 206e 6563 6573 7361  iles are necessa
+000027e0: 7279 2074 6f20 7573 6520 7769 7468 2074  ry to use with t
+000027f0: 6865 206e 6577 2043 4849 414e 5449 2056  he new CHIANTI V
+00002800: 6572 7369 6f6e 2039 2e30 2064 6174 6162  ersion 9.0 datab
+00002810: 6173 6594 8594 8194 7d94 2868 056a ef02  ase.....}.(h.j..
+00002820: 0000 681a 6aed 0200 0068 0168 0368 1b4e  ..h.j....h.h.h.N
+00002830: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00002840: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00002850: 6829 680e 681a 6aea 0200 0068 0168 0368  h)h.h.j....h.h.h
+00002860: 1b68 2a68 1c4b 7075 6268 3d29 8194 7d94  .h*h.Kpubh=)..}.
+00002870: 2868 058c 7e43 6861 6e67 6573 2068 6176  (h..~Changes hav
+00002880: 6520 6265 656e 206d 6164 6520 746f 2074  e been made to t
+00002890: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
+000028a0: 2074 6865 206e 6577 2077 6179 2074 6861   the new way tha
+000028b0: 7420 4348 4941 4e54 4920 6973 2068 616e  t CHIANTI is han
+000028c0: 646c 696e 6720 6469 656c 6563 7472 6f6e  dling dielectron
+000028d0: 6963 2072 6563 6f6d 6269 6e61 7469 6f6e  ic recombination
+000028e0: 2061 6e64 2061 7574 6f69 6f6e 697a 6174   and autoionizat
+000028f0: 696f 6e94 6807 5d94 6815 8c7e 4368 616e  ion.h.].h..~Chan
+00002900: 6765 7320 6861 7665 2062 6565 6e20 6d61  ges have been ma
+00002910: 6465 2074 6f20 7461 6b65 2069 6e74 6f20  de to take into 
+00002920: 6163 636f 756e 7420 7468 6520 6e65 7720  account the new 
+00002930: 7761 7920 7468 6174 2043 4849 414e 5449  way that CHIANTI
+00002940: 2069 7320 6861 6e64 6c69 6e67 2064 6965   is handling die
+00002950: 6c65 6374 726f 6e69 6320 7265 636f 6d62  lectronic recomb
+00002960: 696e 6174 696f 6e20 616e 6420 6175 746f  ination and auto
+00002970: 696f 6e69 7a61 7469 6f6e 9485 9481 947d  ionization.....}
+00002980: 9428 6805 6afd 0200 0068 1a6a fb02 0000  .(h.j....h.j....
+00002990: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
+000029a0: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
+000029b0: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
+000029c0: 1c4b 7268 1a6a ea02 0000 6801 6803 7562  .Krh.j....h.h.ub
+000029d0: 683d 2981 947d 9428 6805 8c4c 5468 6520  h=)..}.(h..LThe 
+000029e0: 7265 6c65 6173 6520 6973 2061 6c73 6f20  release is also 
+000029f0: 6176 6169 6c61 626c 6520 6f6e 205b 5079  available on [Py
+00002a00: 5049 5d28 6874 7470 733a 2f2f 7079 7069  PI](https://pypi
+00002a10: 2e6f 7267 2f70 726f 6a65 6374 2f43 6869  .org/project/Chi
+00002a20: 616e 7469 5079 2f29 9468 075d 9428 6815  antiPy/).h.].(h.
+00002a30: 8c28 5468 6520 7265 6c65 6173 6520 6973  .(The release is
+00002a40: 2061 6c73 6f20 6176 6169 6c61 626c 6520   also available 
+00002a50: 6f6e 205b 5079 5049 5d28 9485 9481 947d  on [PyPI](.....}
+00002a60: 9428 6805 8c28 5468 6520 7265 6c65 6173  .(h..(The releas
+00002a70: 6520 6973 2061 6c73 6f20 6176 6169 6c61  e is also availa
+00002a80: 626c 6520 6f6e 205b 5079 5049 5d28 9468  ble on [PyPI](.h
+00002a90: 1a6a 0903 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+00002aa0: 7562 6800 8c09 7265 6665 7265 6e63 6594  ubh...reference.
+00002ab0: 9394 2981 947d 9428 6805 8c23 6874 7470  ..)..}.(h..#http
+00002ac0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00002ad0: 6a65 6374 2f43 6869 616e 7469 5079 2f94  ject/ChiantiPy/.
+00002ae0: 6807 5d94 6815 8c23 6874 7470 733a 2f2f  h.].h..#https://
+00002af0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00002b00: 2f43 6869 616e 7469 5079 2f94 8594 8194  /ChiantiPy/.....
+00002b10: 7d94 2868 0568 0668 1a6a 1403 0000 7562  }.(h.h.h.j....ub
+00002b20: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+00002b30: 5d94 6825 5d94 6827 5d94 8c06 7265 6675  ].h%].h']...refu
+00002b40: 7269 946a 1603 0000 7568 296a 1203 0000  ri.j....uh)j....
+00002b50: 681a 6a09 0300 0075 6268 158c 0129 9485  h.j....ubh...)..
+00002b60: 9481 947d 9428 6805 8c01 2994 681a 6a09  ...}.(h...).h.j.
+00002b70: 0300 0068 0168 0368 1b4e 681c 4e75 6265  ...h.h.h.Nh.Nube
+00002b80: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00002b90: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+00002ba0: 682a 681c 4b74 681a 6aea 0200 0068 0168  h*h.Kth.j....h.h
+00002bb0: 0375 6268 3d29 8194 7d94 2868 058c 4c44  .ubh=)..}.(h..LD
+00002bc0: 6f63 756d 656e 7461 7469 6f6e 2069 7320  ocumentation is 
+00002bd0: 6176 6169 6c61 626c 6520 6f6e 205b 6769  available on [gi
+00002be0: 7468 7562 2e69 6f5d 2868 7474 7073 3a2f  thub.io](https:/
+00002bf0: 2f63 6869 616e 7469 2d61 746f 6d69 632e  /chianti-atomic.
+00002c00: 6769 7468 7562 2e69 6f2f 2994 6807 5d94  github.io/).h.].
+00002c10: 2868 158c 2a44 6f63 756d 656e 7461 7469  (h..*Documentati
+00002c20: 6f6e 2069 7320 6176 6169 6c61 626c 6520  on is available 
+00002c30: 6f6e 205b 6769 7468 7562 2e69 6f5d 2894  on [github.io](.
+00002c40: 8594 8194 7d94 2868 058c 2a44 6f63 756d  ....}.(h..*Docum
+00002c50: 656e 7461 7469 6f6e 2069 7320 6176 6169  entation is avai
+00002c60: 6c61 626c 6520 6f6e 205b 6769 7468 7562  lable on [github
+00002c70: 2e69 6f5d 2894 681a 6a2e 0300 0068 0168  .io](.h.j....h.h
+00002c80: 0368 1b4e 681c 4e75 626a 1303 0000 2981  .h.Nh.Nubj....).
+00002c90: 947d 9428 6805 8c21 6874 7470 733a 2f2f  .}.(h..!https://
+00002ca0: 6368 6961 6e74 692d 6174 6f6d 6963 2e67  chianti-atomic.g
+00002cb0: 6974 6875 622e 696f 2f94 6807 5d94 6815  ithub.io/.h.].h.
+00002cc0: 8c21 6874 7470 733a 2f2f 6368 6961 6e74  .!https://chiant
+00002cd0: 692d 6174 6f6d 6963 2e67 6974 6875 622e  i-atomic.github.
+00002ce0: 696f 2f94 8594 8194 7d94 2868 0568 0668  io/.....}.(h.h.h
+00002cf0: 1a6a 3703 0000 7562 6168 1d7d 9428 681f  .j7...ubah.}.(h.
+00002d00: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
+00002d10: 5d94 8c06 7265 6675 7269 946a 3903 0000  ]...refuri.j9...
+00002d20: 7568 296a 1203 0000 681a 6a2e 0300 0075  uh)j....h.j....u
+00002d30: 6268 158c 0129 9485 9481 947d 9428 6805  bh...).....}.(h.
+00002d40: 6a27 0300 0068 1a6a 2e03 0000 6801 6803  j'...h.j....h.h.
+00002d50: 681b 4e68 1c4e 7562 6568 1d7d 9428 681f  h.Nh.Nubeh.}.(h.
+00002d60: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
+00002d70: 5d94 7568 2968 3c68 1b68 2a68 1c4b 7668  ].uh)h<h.h*h.Kvh
+00002d80: 1a6a ea02 0000 6801 6803 7562 683d 2981  .j....h.h.ubh=).
+00002d90: 947d 9428 6805 8c4e 616e 6420 6f6e 205b  .}.(h..Nand on [
+00002da0: 5265 6164 5468 6544 6f63 735d 2868 7474  ReadTheDocs](htt
+00002db0: 7073 3a2f 2f63 6869 616e 7469 7079 2e72  ps://chiantipy.r
+00002dc0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00002dd0: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
+00002de0: 6174 6573 7429 9468 075d 9428 6815 8c15  atest).h.].(h...
+00002df0: 616e 6420 6f6e 205b 5265 6164 5468 6544  and on [ReadTheD
+00002e00: 6f63 735d 2894 8594 8194 7d94 2868 058c  ocs](.....}.(h..
+00002e10: 1561 6e64 206f 6e20 5b52 6561 6454 6865  .and on [ReadThe
+00002e20: 446f 6373 5d28 9468 1a6a 5003 0000 6801  Docs](.h.jP...h.
+00002e30: 6803 681b 4e68 1c4e 7562 6a13 0300 0029  h.h.Nh.Nubj....)
+00002e40: 8194 7d94 2868 058c 3868 7474 7073 3a2f  ..}.(h..8https:/
+00002e50: 2f63 6869 616e 7469 7079 2e72 6561 6474  /chiantipy.readt
+00002e60: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00002e70: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00002e80: 7494 6807 5d94 6815 8c38 6874 7470 733a  t.h.].h..8https:
+00002e90: 2f2f 6368 6961 6e74 6970 792e 7265 6164  //chiantipy.read
+00002ea0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00002eb0: 7465 7374 2f3f 6261 6467 653d 6c61 7465  test/?badge=late
+00002ec0: 7374 9485 9481 947d 9428 6805 6806 681a  st.....}.(h.h.h.
+00002ed0: 6a59 0300 0075 6261 681d 7d94 2868 1f5d  jY...ubah.}.(h.]
+00002ee0: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00002ef0: 948c 0672 6566 7572 6994 6a5b 0300 0075  ...refuri.j[...u
+00002f00: 6829 6a12 0300 0068 1a6a 5003 0000 7562  h)j....h.jP...ub
+00002f10: 6815 8c01 2994 8594 8194 7d94 2868 056a  h...).....}.(h.j
+00002f20: 2703 0000 681a 6a50 0300 0068 0168 0368  '...h.jP...h.h.h
+00002f30: 1b4e 681c 4e75 6265 681d 7d94 2868 1f5d  .Nh.Nubeh.}.(h.]
+00002f40: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00002f50: 9475 6829 683c 681b 682a 681c 4b78 681a  .uh)h<h.h*h.Kxh.
+00002f60: 6aea 0200 0068 0168 0375 6265 681d 7d94  j....h.h.ubeh.}.
+00002f70: 2868 1f5d 948c 5276 6572 7369 6f6e 2d30  (h.]..Rversion-0
+00002f80: 2d38 2d78 2d66 696c 6573 2d61 7265 2d6e  -8-x-files-are-n
+00002f90: 6563 6573 7361 7279 2d74 6f2d 7573 652d  ecessary-to-use-
+00002fa0: 7769 7468 2d74 6865 2d6e 6577 2d63 6869  with-the-new-chi
+00002fb0: 616e 7469 2d76 6572 7369 6f6e 2d39 2d30  anti-version-9-0
+00002fc0: 2d64 6174 6162 6173 6594 6168 215d 9468  -database.ah!].h
+00002fd0: 235d 948c 5276 6572 7369 6f6e 2030 2e38  #]..Rversion 0.8
+00002fe0: 2e78 2066 696c 6573 2061 7265 206e 6563  .x files are nec
+00002ff0: 6573 7361 7279 2074 6f20 7573 6520 7769  essary to use wi
+00003000: 7468 2074 6865 206e 6577 2063 6869 616e  th the new chian
+00003010: 7469 2076 6572 7369 6f6e 2039 2e30 2064  ti version 9.0 d
+00003020: 6174 6162 6173 6594 6168 255d 9468 275d  atabase.ah%].h']
+00003030: 9475 6829 6809 681a 680b 6801 6803 681b  .uh)h.h.h.h.h.h.
+00003040: 682a 681c 4b70 7562 680a 2981 947d 9428  h*h.Kpubh.)..}.(
+00003050: 6805 6806 6807 5d94 2868 0f29 8194 7d94  h.h.h.].(h.)..}.
+00003060: 2868 058c 1b63 6861 6e67 6573 2066 726f  (h...changes fro
+00003070: 6d20 302e 372e 3120 746f 2030 2e38 2e30  m 0.7.1 to 0.8.0
+00003080: 9468 075d 9468 158c 1b63 6861 6e67 6573  .h.].h...changes
+00003090: 2066 726f 6d20 302e 372e 3120 746f 2030   from 0.7.1 to 0
+000030a0: 2e38 2e30 9485 9481 947d 9428 6805 6a7f  .8.0.....}.(h.j.
+000030b0: 0300 0068 1a6a 7d03 0000 6801 6803 681b  ...h.j}...h.h.h.
+000030c0: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
+000030d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000030e0: 7568 2968 0e68 1a6a 7a03 0000 6801 6803  uh)h.h.jz...h.h.
+000030f0: 681b 682a 681c 4b7c 7562 683d 2981 947d  h.h*h.K|ubh=)..}
+00003100: 9428 6805 8c58 4368 6961 6e74 6950 7920  .(h..XChiantiPy 
+00003110: 6973 206e 6f77 206f 6e6c 7920 636f 6d70  is now only comp
+00003120: 6c69 616e 7420 7769 7468 2050 7974 686f  liant with Pytho
+00003130: 6e20 332e 2020 4465 7665 6c6f 706d 656e  n 3.  Developmen
+00003140: 7420 6973 2063 7572 7265 6e74 6c79 2077  t is currently w
+00003150: 6974 6820 5079 7468 6f6e 2033 2e36 9468  ith Python 3.6.h
+00003160: 075d 9468 158c 5843 6869 616e 7469 5079  .].h..XChiantiPy
+00003170: 2069 7320 6e6f 7720 6f6e 6c79 2063 6f6d   is now only com
+00003180: 706c 6961 6e74 2077 6974 6820 5079 7468  pliant with Pyth
+00003190: 6f6e 2033 2e20 2044 6576 656c 6f70 6d65  on 3.  Developme
+000031a0: 6e74 2069 7320 6375 7272 656e 746c 7920  nt is currently 
+000031b0: 7769 7468 2050 7974 686f 6e20 332e 3694  with Python 3.6.
+000031c0: 8594 8194 7d94 2868 056a 8d03 0000 681a  ....}.(h.j....h.
+000031d0: 6a8b 0300 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+000031e0: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
+000031f0: 235d 9468 255d 9468 275d 9475 6829 683c  #].h%].h'].uh)h<
+00003200: 681b 682a 681c 4b7e 681a 6a7a 0300 0068  h.h*h.K~h.jz...h
+00003210: 0168 0375 6268 3d29 8194 7d94 2868 058c  .h.ubh=)..}.(h..
+00003220: 5354 6865 2075 7365 206f 6620 7468 6520  SThe use of the 
+00003230: 5079 5174 3420 616e 6420 5778 5769 6467  PyQt4 and WxWidg
+00003240: 6574 7320 7061 636b 6167 6573 2068 6176  ets packages hav
+00003250: 6520 6265 656e 2064 726f 7070 6564 2061  e been dropped a
+00003260: 6e64 2050 7951 7435 2069 7320 6e6f 7720  nd PyQt5 is now 
+00003270: 7573 6564 9468 075d 9468 158c 5354 6865  used.h.].h..SThe
+00003280: 2075 7365 206f 6620 7468 6520 5079 5174   use of the PyQt
+00003290: 3420 616e 6420 5778 5769 6467 6574 7320  4 and WxWidgets 
+000032a0: 7061 636b 6167 6573 2068 6176 6520 6265  packages have be
+000032b0: 656e 2064 726f 7070 6564 2061 6e64 2050  en dropped and P
+000032c0: 7951 7435 2069 7320 6e6f 7720 7573 6564  yQt5 is now used
+000032d0: 9485 9481 947d 9428 6805 6a9b 0300 0068  .....}.(h.j....h
+000032e0: 1a6a 9903 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+000032f0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00003300: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+00003310: 3c68 1b68 2a68 1c4b 8068 1a6a 7a03 0000  <h.h*h.K.h.jz...
+00003320: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
+00003330: 8c41 5468 6520 646f 6375 6d65 6e74 6174  .AThe documentat
+00003340: 696f 6e20 6973 206e 6f77 2061 7661 696c  ion is now avail
+00003350: 6162 6c65 206f 6e20 6769 7468 7562 2e69  able on github.i
+00003360: 6f5f 2061 6e64 2052 6561 6454 6865 446f  o_ and ReadTheDo
+00003370: 6373 5f94 6807 5d94 2868 158c 2654 6865  cs_.h.].(h..&The
+00003380: 2064 6f63 756d 656e 7461 7469 6f6e 2069   documentation i
+00003390: 7320 6e6f 7720 6176 6169 6c61 626c 6520  s now available 
+000033a0: 6f6e 2094 8594 8194 7d94 2868 058c 2654  on .....}.(h..&T
+000033b0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+000033c0: 2069 7320 6e6f 7720 6176 6169 6c61 626c   is now availabl
+000033d0: 6520 6f6e 2094 681a 6aa7 0300 0068 0168  e on .h.j....h.h
+000033e0: 0368 1b4e 681c 4e75 626a 1303 0000 2981  .h.Nh.Nubj....).
+000033f0: 947d 9428 6805 8c0a 6769 7468 7562 2e69  .}.(h...github.i
+00003400: 6f5f 9468 075d 9468 158c 0967 6974 6875  o_.h.].h...githu
+00003410: 622e 696f 9485 9481 947d 9428 6805 6806  b.io.....}.(h.h.
+00003420: 681a 6ab0 0300 0075 6261 681d 7d94 2868  h.j....ubah.}.(h
+00003430: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+00003440: 275d 948c 046e 616d 6594 8c09 6769 7468  ']...name...gith
+00003450: 7562 2e69 6f94 8c06 7265 6675 7269 948c  ub.io...refuri..
+00003460: 2168 7474 7073 3a2f 2f63 6869 616e 7469  !https://chianti
+00003470: 2d61 746f 6d69 632e 6769 7468 7562 2e69  -atomic.github.i
+00003480: 6f2f 9475 6829 6a12 0300 0068 1a6a a703  o/.uh)j....h.j..
+00003490: 0000 8c08 7265 736f 6c76 6564 944b 0175  ....resolved.K.u
+000034a0: 6268 158c 0520 616e 6420 9485 9481 947d  bh... and .....}
+000034b0: 9428 6805 8c05 2061 6e64 2094 681a 6aa7  .(h... and .h.j.
+000034c0: 0300 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
+000034d0: 1303 0000 2981 947d 9428 6805 8c0c 5265  ....)..}.(h...Re
+000034e0: 6164 5468 6544 6f63 735f 9468 075d 9468  adTheDocs_.h.].h
+000034f0: 158c 0b52 6561 6454 6865 446f 6373 9485  ...ReadTheDocs..
+00003500: 9481 947d 9428 6805 6806 681a 6ac8 0300  ...}.(h.h.h.j...
+00003510: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
+00003520: 9468 235d 9468 255d 9468 275d 948c 046e  .h#].h%].h']...n
+00003530: 616d 6594 8c0b 5265 6164 5468 6544 6f63  ame...ReadTheDoc
+00003540: 7394 6ac0 0300 008c 3868 7474 7073 3a2f  s.j.....8https:/
+00003550: 2f63 6869 616e 7469 7079 2e72 6561 6474  /chiantipy.readt
+00003560: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00003570: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00003580: 7494 7568 296a 1203 0000 681a 6aa7 0300  t.uh)j....h.j...
+00003590: 006a c203 0000 4b01 7562 6568 1d7d 9428  .j....K.ubeh.}.(
+000035a0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+000035b0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
+000035c0: 8268 1a6a 7a03 0000 6801 6803 7562 6800  .h.jz...h.h.ubh.
+000035d0: 8c06 7461 7267 6574 9493 9429 8194 7d94  ..target...)..}.
+000035e0: 2868 058c 312e 2e20 5f67 6974 6875 622e  (h..1.. _github.
+000035f0: 696f 3a20 2068 7474 7073 3a2f 2f63 6869  io:  https://chi
+00003600: 616e 7469 2d61 746f 6d69 632e 6769 7468  anti-atomic.gith
+00003610: 7562 2e69 6f2f 9468 075d 9468 1d7d 9428  ub.io/.h.].h.}.(
+00003620: 681f 5d94 8c09 6769 7468 7562 2d69 6f94  h.]...github-io.
+00003630: 6168 215d 9468 235d 948c 0967 6974 6875  ah!].h#]...githu
+00003640: 622e 696f 9461 6825 5d94 6827 5d94 6ac0  b.io.ah%].h'].j.
+00003650: 0300 006a c103 0000 7568 296a df03 0000  ...j....uh)j....
+00003660: 681c 4b84 681a 6a7a 0300 0068 0168 0368  h.K.h.jz...h.h.h
+00003670: 1b68 2a6a 6a02 0000 4b01 7562 6ae0 0300  .h*jj...K.ubj...
+00003680: 0029 8194 7d94 2868 058c 4a2e 2e20 5f52  .)..}.(h..J.. _R
+00003690: 6561 6454 6865 446f 6373 3a20 2068 7474  eadTheDocs:  htt
+000036a0: 7073 3a2f 2f63 6869 616e 7469 7079 2e72  ps://chiantipy.r
+000036b0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+000036c0: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
+000036d0: 6174 6573 7494 6807 5d94 681d 7d94 2868  atest.h.].h.}.(h
+000036e0: 1f5d 948c 0b72 6561 6474 6865 646f 6373  .]...readthedocs
+000036f0: 9461 6821 5d94 6823 5d94 8c0b 7265 6164  .ah!].h#]...read
+00003700: 7468 6564 6f63 7394 6168 255d 9468 275d  thedocs.ah%].h']
+00003710: 946a c003 0000 6ad8 0300 0075 6829 6adf  .j....j....uh)j.
+00003720: 0300 0068 1c4b 8668 1a6a 7a03 0000 6801  ...h.K.h.jz...h.
+00003730: 6803 681b 682a 6a6a 0200 004b 0175 6265  h.h.h*jj...K.ube
+00003740: 681d 7d94 2868 1f5d 948c 1b63 6861 6e67  h.}.(h.]...chang
+00003750: 6573 2d66 726f 6d2d 302d 372d 312d 746f  es-from-0-7-1-to
+00003760: 2d30 2d38 2d30 9461 6821 5d94 6823 5d94  -0-8-0.ah!].h#].
+00003770: 8c1b 6368 616e 6765 7320 6672 6f6d 2030  ..changes from 0
+00003780: 2e37 2e31 2074 6f20 302e 382e 3094 6168  .7.1 to 0.8.0.ah
+00003790: 255d 9468 275d 9475 6829 6809 681a 680b  %].h'].uh)h.h.h.
+000037a0: 6801 6803 681b 682a 681c 4b7c 7562 680a  h.h.h.h*h.K|ubh.
+000037b0: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+000037c0: 0f29 8194 7d94 2868 058c 1b63 6861 6e67  .)..}.(h...chang
+000037d0: 6573 2066 726f 6d20 302e 372e 3020 746f  es from 0.7.0 to
+000037e0: 2030 2e37 2e31 9468 075d 9468 158c 1b63   0.7.1.h.].h...c
+000037f0: 6861 6e67 6573 2066 726f 6d20 302e 372e  hanges from 0.7.
+00003800: 3020 746f 2030 2e37 2e31 9485 9481 947d  0 to 0.7.1.....}
+00003810: 9428 6805 6a06 0400 0068 1a6a 0404 0000  .(h.j....h.j....
+00003820: 6801 6803 681b 4e68 1c4e 7562 6168 1d7d  h.h.h.Nh.Nubah.}
+00003830: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
+00003840: 5d94 6827 5d94 7568 2968 0e68 1a6a 0104  ].h'].uh)h.h.j..
+00003850: 0000 6801 6803 681b 682a 681c 4b89 7562  ..h.h.h.h*h.K.ub
+00003860: 683d 2981 947d 9428 6805 8cb0 7665 7273  h=)..}.(h...vers
+00003870: 696f 6e20 302e 372e 3020 696e 636c 7564  ion 0.7.0 includ
+00003880: 6564 2073 6f6d 6520 6368 616e 6765 7320  ed some changes 
+00003890: 696e 2074 6865 2043 6869 616e 7469 5079  in the ChiantiPy
+000038a0: 206e 616d 696e 6720 636f 6e76 656e 7469   naming conventi
+000038b0: 6f6e 732c 206c 6172 6765 6c79 2069 6e20  ons, largely in 
+000038c0: 7468 6520 636f 6e74 696e 7575 6d20 636c  the continuum cl
+000038d0: 6173 732e 2020 5468 6573 6520 6172 6520  ass.  These are 
+000038e0: 6265 696e 6720 7265 7665 7274 6564 2074  being reverted t
+000038f0: 6f20 7468 6520 6f72 6967 696e 616c 2043  o the original C
+00003900: 6869 616e 7469 5079 206e 616d 696e 6720  hiantiPy naming 
+00003910: 636f 6e76 656e 7469 6f6e 732e 9468 075d  conventions..h.]
+00003920: 9468 158c b076 6572 7369 6f6e 2030 2e37  .h...version 0.7
+00003930: 2e30 2069 6e63 6c75 6465 6420 736f 6d65  .0 included some
+00003940: 2063 6861 6e67 6573 2069 6e20 7468 6520   changes in the 
+00003950: 4368 6961 6e74 6950 7920 6e61 6d69 6e67  ChiantiPy naming
+00003960: 2063 6f6e 7665 6e74 696f 6e73 2c20 6c61   conventions, la
+00003970: 7267 656c 7920 696e 2074 6865 2063 6f6e  rgely in the con
+00003980: 7469 6e75 756d 2063 6c61 7373 2e20 2054  tinuum class.  T
+00003990: 6865 7365 2061 7265 2062 6569 6e67 2072  hese are being r
+000039a0: 6576 6572 7465 6420 746f 2074 6865 206f  everted to the o
+000039b0: 7269 6769 6e61 6c20 4368 6961 6e74 6950  riginal ChiantiP
+000039c0: 7920 6e61 6d69 6e67 2063 6f6e 7665 6e74  y naming convent
+000039d0: 696f 6e73 2e94 8594 8194 7d94 2868 056a  ions......}.(h.j
+000039e0: 1404 0000 681a 6a12 0400 0068 0168 0368  ....h.j....h.h.h
+000039f0: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+00003a00: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00003a10: 9475 6829 683c 681b 682a 681c 4b8b 681a  .uh)h<h.h*h.K.h.
+00003a20: 6a01 0400 0068 0168 0375 6268 3d29 8194  j....h.h.ubh=)..
+00003a30: 7d94 2868 058c 6474 6865 2069 6f6e 2e66  }.(h..dthe ion.f
+00003a40: 7265 6542 6f75 6e64 7878 7820 6d65 7468  reeBoundxxx meth
+00003a50: 6f64 7320 6861 7665 2062 6565 6e20 6669  ods have been fi
+00003a60: 7865 6420 616e 6420 7468 6973 2061 6c73  xed and this als
+00003a70: 6f20 6669 7865 7320 7468 6520 7072 6f62  o fixes the prob
+00003a80: 6c65 6d20 7769 7468 2074 6865 2052 6164  lem with the Rad
+00003a90: 4c6f 7373 2063 6c61 7373 2e94 6807 5d94  Loss class..h.].
+00003aa0: 6815 8c64 7468 6520 696f 6e2e 6672 6565  h..dthe ion.free
+00003ab0: 426f 756e 6478 7878 206d 6574 686f 6473  Boundxxx methods
+00003ac0: 2068 6176 6520 6265 656e 2066 6978 6564   have been fixed
+00003ad0: 2061 6e64 2074 6869 7320 616c 736f 2066   and this also f
+00003ae0: 6978 6573 2074 6865 2070 726f 626c 656d  ixes the problem
+00003af0: 2077 6974 6820 7468 6520 5261 644c 6f73   with the RadLos
+00003b00: 7320 636c 6173 732e 9485 9481 947d 9428  s class......}.(
+00003b10: 6805 6a22 0400 0068 1a6a 2004 0000 6801  h.j"...h.j ...h.
+00003b20: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
+00003b30: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00003b40: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
+00003b50: 8d68 1a6a 0104 0000 6801 6803 7562 683d  .h.j....h.h.ubh=
+00003b60: 2981 947d 9428 6805 8c35 6120 7073 6575  )..}.(h..5a pseu
+00003b70: 646f 2d76 6f69 6774 2066 696c 7465 7220  do-voigt filter 
+00003b80: 6861 7320 6265 656e 2061 6464 6564 2074  has been added t
+00003b90: 6f20 746f 6f6c 732e 6669 6c74 6572 7394  o tools.filters.
+00003ba0: 6807 5d94 6815 8c35 6120 7073 6575 646f  h.].h..5a pseudo
+00003bb0: 2d76 6f69 6774 2066 696c 7465 7220 6861  -voigt filter ha
+00003bc0: 7320 6265 656e 2061 6464 6564 2074 6f20  s been added to 
+00003bd0: 746f 6f6c 732e 6669 6c74 6572 7394 8594  tools.filters...
+00003be0: 8194 7d94 2868 056a 3004 0000 681a 6a2e  ..}.(h.j0...h.j.
+00003bf0: 0400 0068 0168 0368 1b4e 681c 4e75 6261  ...h.h.h.Nh.Nuba
+00003c00: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00003c10: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+00003c20: 682a 681c 4b8f 681a 6a01 0400 0068 0168  h*h.K.h.j....h.h
+00003c30: 0375 6268 3d29 8194 7d94 2868 058c 5b74  .ubh=)..}.(h..[t
+00003c40: 6865 206b 6579 776f 7264 2061 7267 756d  he keyword argum
+00003c50: 656e 7420 7776 6c52 616e 6765 2068 6173  ent wvlRange has
+00003c60: 2062 6565 6e20 7265 6d6f 7665 6420 6672   been removed fr
+00003c70: 6f6d 2074 6865 2069 6f6e 2e65 6d69 7373  om the ion.emiss
+00003c80: 2061 6e64 2069 6f6e 2e69 6e74 656e 7369   and ion.intensi
+00003c90: 7479 206d 6574 686f 6473 9468 075d 9468  ty methods.h.].h
+00003ca0: 158c 5b74 6865 206b 6579 776f 7264 2061  ..[the keyword a
+00003cb0: 7267 756d 656e 7420 7776 6c52 616e 6765  rgument wvlRange
+00003cc0: 2068 6173 2062 6565 6e20 7265 6d6f 7665   has been remove
+00003cd0: 6420 6672 6f6d 2074 6865 2069 6f6e 2e65  d from the ion.e
+00003ce0: 6d69 7373 2061 6e64 2069 6f6e 2e69 6e74  miss and ion.int
+00003cf0: 656e 7369 7479 206d 6574 686f 6473 9485  ensity methods..
+00003d00: 9481 947d 9428 6805 6a3e 0400 0068 1a6a  ...}.(h.j>...h.j
+00003d10: 3c04 0000 6801 6803 681b 4e68 1c4e 7562  <...h.h.h.Nh.Nub
+00003d20: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+00003d30: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
+00003d40: 1b68 2a68 1c4b 9168 1a6a 0104 0000 6801  .h*h.K.h.j....h.
+00003d50: 6803 7562 683d 2981 947d 9428 6805 8cbd  h.ubh=)..}.(h...
+00003d60: 7468 6520 6b65 7977 6f72 6420 6172 6775  the keyword argu
+00003d70: 6d65 6e74 2066 6f72 2074 6865 2045 6d69  ment for the Emi
+00003d80: 7373 696f 6e20 4d65 6173 7572 652c 2065  ssion Measure, e
+00003d90: 6d2c 2068 6173 2062 6565 6e20 7265 6d6f  m, has been remo
+00003da0: 7665 6420 6672 6f6d 2074 6865 2069 6f6e  ved from the ion
+00003db0: 2e69 6e74 656e 7369 7479 2061 6e64 2073  .intensity and s
+00003dc0: 696d 696c 6172 206d 6574 686f 6473 2e20  imilar methods. 
+00003dd0: 2049 7420 6973 206e 6f77 206e 6563 6573   It is now neces
+00003de0: 7361 7279 2074 6f20 7370 6563 6966 790a  sary to specify.
+00003df0: 7468 6520 656d 6973 7369 6f6e 2077 6865  the emission whe
+00003e00: 6e20 7468 6520 6f62 6a65 6374 2069 7320  n the object is 
+00003e10: 696e 7374 616e 7469 6174 6564 2e94 6807  instantiated..h.
+00003e20: 5d94 6815 8cbd 7468 6520 6b65 7977 6f72  ].h...the keywor
+00003e30: 6420 6172 6775 6d65 6e74 2066 6f72 2074  d argument for t
+00003e40: 6865 2045 6d69 7373 696f 6e20 4d65 6173  he Emission Meas
+00003e50: 7572 652c 2065 6d2c 2068 6173 2062 6565  ure, em, has bee
+00003e60: 6e20 7265 6d6f 7665 6420 6672 6f6d 2074  n removed from t
+00003e70: 6865 2069 6f6e 2e69 6e74 656e 7369 7479  he ion.intensity
+00003e80: 2061 6e64 2073 696d 696c 6172 206d 6574   and similar met
+00003e90: 686f 6473 2e20 2049 7420 6973 206e 6f77  hods.  It is now
+00003ea0: 206e 6563 6573 7361 7279 2074 6f20 7370   necessary to sp
+00003eb0: 6563 6966 790a 7468 6520 656d 6973 7369  ecify.the emissi
+00003ec0: 6f6e 2077 6865 6e20 7468 6520 6f62 6a65  on when the obje
+00003ed0: 6374 2069 7320 696e 7374 616e 7469 6174  ct is instantiat
+00003ee0: 6564 2e94 8594 8194 7d94 2868 056a 4c04  ed......}.(h.jL.
+00003ef0: 0000 681a 6a4a 0400 0068 0168 0368 1b4e  ..h.jJ...h.h.h.N
+00003f00: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00003f10: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00003f20: 6829 683c 681b 682a 681c 4b93 681a 6a01  h)h<h.h*h.K.h.j.
+00003f30: 0400 0068 0168 0375 6268 3d29 8194 7d94  ...h.h.ubh=)..}.
+00003f40: 2868 058c 4d61 2073 6574 206f 6620 5079  (h..Ma set of Py
+00003f50: 5174 3520 6469 616c 6f67 7320 6861 7665  Qt5 dialogs have
+00003f60: 2062 6565 6e20 6465 7665 6c6f 7065 6420   been developed 
+00003f70: 6279 202a 2a6b 7472 6974 7a2a 2a20 616e  by **ktritz** an
+00003f80: 6420 6172 6520 6e6f 7720 696e 636c 7564  d are now includ
+00003f90: 6564 9468 075d 9428 6815 8c2e 6120 7365  ed.h.].(h...a se
+00003fa0: 7420 6f66 2050 7951 7435 2064 6961 6c6f  t of PyQt5 dialo
+00003fb0: 6773 2068 6176 6520 6265 656e 2064 6576  gs have been dev
+00003fc0: 656c 6f70 6564 2062 7920 9485 9481 947d  eloped by .....}
+00003fd0: 9428 6805 8c2e 6120 7365 7420 6f66 2050  .(h...a set of P
+00003fe0: 7951 7435 2064 6961 6c6f 6773 2068 6176  yQt5 dialogs hav
+00003ff0: 6520 6265 656e 2064 6576 656c 6f70 6564  e been developed
+00004000: 2062 7920 9468 1a6a 5804 0000 6801 6803   by .h.jX...h.h.
+00004010: 681b 4e68 1c4e 7562 6800 8c06 7374 726f  h.Nh.Nubh...stro
+00004020: 6e67 9493 9429 8194 7d94 2868 058c 0a2a  ng...)..}.(h...*
+00004030: 2a6b 7472 6974 7a2a 2a94 6807 5d94 6815  *ktritz**.h.].h.
+00004040: 8c06 6b74 7269 747a 9485 9481 947d 9428  ..ktritz.....}.(
+00004050: 6805 6806 681a 6a63 0400 0075 6261 681d  h.h.h.jc...ubah.
+00004060: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00004070: 255d 9468 275d 9475 6829 6a61 0400 0068  %].h'].uh)ja...h
+00004080: 1a6a 5804 0000 7562 6815 8c15 2061 6e64  .jX...ubh... and
+00004090: 2061 7265 206e 6f77 2069 6e63 6c75 6465   are now include
+000040a0: 6494 8594 8194 7d94 2868 058c 1520 616e  d.....}.(h... an
+000040b0: 6420 6172 6520 6e6f 7720 696e 636c 7564  d are now includ
+000040c0: 6564 9468 1a6a 5804 0000 6801 6803 681b  ed.h.jX...h.h.h.
+000040d0: 4e68 1c4e 7562 6568 1d7d 9428 681f 5d94  Nh.Nubeh.}.(h.].
+000040e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000040f0: 7568 2968 3c68 1b68 2a68 1c4b 9668 1a6a  uh)h<h.h*h.K.h.j
+00004100: 0104 0000 6801 6803 7562 683d 2981 947d  ....h.h.ubh=)..}
+00004110: 9428 6805 8c46 7468 6973 2069 7320 7468  .(h..Fthis is th
+00004120: 6520 6c61 7374 2072 656c 6561 7365 2074  e last release t
+00004130: 6861 7420 7769 6c6c 2075 7365 2074 6865  hat will use the
+00004140: 2050 7951 7434 2077 6964 6765 7473 2061   PyQt4 widgets a
+00004150: 7320 616e 206f 7074 696f 6e2e 9468 075d  s an option..h.]
+00004160: 9468 158c 4674 6869 7320 6973 2074 6865  .h..Fthis is the
+00004170: 206c 6173 7420 7265 6c65 6173 6520 7468   last release th
+00004180: 6174 2077 696c 6c20 7573 6520 7468 6520  at will use the 
+00004190: 5079 5174 3420 7769 6467 6574 7320 6173  PyQt4 widgets as
+000041a0: 2061 6e20 6f70 7469 6f6e 2e94 8594 8194   an option......
+000041b0: 7d94 2868 056a 7e04 0000 681a 6a7c 0400  }.(h.j~...h.j|..
+000041c0: 0068 0168 0368 1b4e 681c 4e75 6261 681d  .h.h.h.Nh.Nubah.
+000041d0: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+000041e0: 255d 9468 275d 9475 6829 683c 681b 682a  %].h'].uh)h<h.h*
+000041f0: 681c 4b98 681a 6a01 0400 0068 0168 0375  h.K.h.j....h.h.u
+00004200: 6268 3d29 8194 7d94 2868 058c 8f74 6865  bh=)..}.(h...the
+00004210: 206d 6574 686f 6420 2a2a 696f 6e65 714f   method **ioneqO
+00004220: 6e65 2a2a 2069 7320 7573 6564 2062 7920  ne** is used by 
+00004230: 626f 7468 2074 6865 2049 6f6e 2061 6e64  both the Ion and
+00004240: 2043 6f6e 7469 6e75 756d 2063 6c61 7373   Continuum class
+00004250: 2e20 2049 7420 6861 7320 6265 656e 206d  .  It has been m
+00004260: 6f76 6564 2074 6f20 6120 7369 6e67 6c65  oved to a single
+00004270: 205f 496f 6e65 714f 6e65 2e70 7920 6669   _IoneqOne.py fi
+00004280: 6c65 2069 6e20 7468 6520 2a2a 6261 7365  le in the **base
+00004290: 2a2a 2064 6972 6563 746f 7279 9468 075d  ** directory.h.]
+000042a0: 9428 6815 8c0b 7468 6520 6d65 7468 6f64  .(h...the method
+000042b0: 2094 8594 8194 7d94 2868 058c 0b74 6865   .....}.(h...the
+000042c0: 206d 6574 686f 6420 9468 1a6a 8a04 0000   method .h.j....
+000042d0: 6801 6803 681b 4e68 1c4e 7562 6a62 0400  h.h.h.Nh.Nubjb..
+000042e0: 0029 8194 7d94 2868 058c 0c2a 2a69 6f6e  .)..}.(h...**ion
+000042f0: 6571 4f6e 652a 2a94 6807 5d94 6815 8c08  eqOne**.h.].h...
+00004300: 696f 6e65 714f 6e65 9485 9481 947d 9428  ioneqOne.....}.(
+00004310: 6805 6806 681a 6a93 0400 0075 6261 681d  h.h.h.j....ubah.
+00004320: 7d94 2868 1f5d 9468 215d 9468 235d 9468  }.(h.].h!].h#].h
+00004330: 255d 9468 275d 9475 6829 6a61 0400 0068  %].h'].uh)ja...h
+00004340: 1a6a 8a04 0000 7562 6815 8c66 2069 7320  .j....ubh..f is 
+00004350: 7573 6564 2062 7920 626f 7468 2074 6865  used by both the
+00004360: 2049 6f6e 2061 6e64 2043 6f6e 7469 6e75   Ion and Continu
+00004370: 756d 2063 6c61 7373 2e20 2049 7420 6861  um class.  It ha
+00004380: 7320 6265 656e 206d 6f76 6564 2074 6f20  s been moved to 
+00004390: 6120 7369 6e67 6c65 205f 496f 6e65 714f  a single _IoneqO
+000043a0: 6e65 2e70 7920 6669 6c65 2069 6e20 7468  ne.py file in th
+000043b0: 6520 9485 9481 947d 9428 6805 8c66 2069  e .....}.(h..f i
+000043c0: 7320 7573 6564 2062 7920 626f 7468 2074  s used by both t
+000043d0: 6865 2049 6f6e 2061 6e64 2043 6f6e 7469  he Ion and Conti
+000043e0: 6e75 756d 2063 6c61 7373 2e20 2049 7420  nuum class.  It 
+000043f0: 6861 7320 6265 656e 206d 6f76 6564 2074  has been moved t
+00004400: 6f20 6120 7369 6e67 6c65 205f 496f 6e65  o a single _Ione
+00004410: 714f 6e65 2e70 7920 6669 6c65 2069 6e20  qOne.py file in 
+00004420: 7468 6520 9468 1a6a 8a04 0000 6801 6803  the .h.j....h.h.
+00004430: 681b 4e68 1c4e 7562 6a62 0400 0029 8194  h.Nh.Nubjb...)..
+00004440: 7d94 2868 058c 082a 2a62 6173 652a 2a94  }.(h...**base**.
+00004450: 6807 5d94 6815 8c04 6261 7365 9485 9481  h.].h...base....
+00004460: 947d 9428 6805 6806 681a 6aa6 0400 0075  .}.(h.h.h.j....u
+00004470: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
+00004480: 235d 9468 255d 9468 275d 9475 6829 6a61  #].h%].h'].uh)ja
+00004490: 0400 0068 1a6a 8a04 0000 7562 6815 8c0a  ...h.j....ubh...
+000044a0: 2064 6972 6563 746f 7279 9485 9481 947d   directory.....}
+000044b0: 9428 6805 8c0a 2064 6972 6563 746f 7279  .(h... directory
+000044c0: 9468 1a6a 8a04 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
+000044d0: 1c4e 7562 6568 1d7d 9428 681f 5d94 6821  .Nubeh.}.(h.].h!
+000044e0: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
+000044f0: 2968 3c68 1b68 2a68 1c4b 9a68 1a6a 0104  )h<h.h*h.K.h.j..
+00004500: 0000 6801 6803 7562 6568 1d7d 9428 681f  ..h.h.ubeh.}.(h.
+00004510: 5d94 8c1b 6368 616e 6765 732d 6672 6f6d  ]...changes-from
+00004520: 2d30 2d37 2d30 2d74 6f2d 302d 372d 3194  -0-7-0-to-0-7-1.
+00004530: 6168 215d 9468 235d 948c 1b63 6861 6e67  ah!].h#]...chang
+00004540: 6573 2066 726f 6d20 302e 372e 3020 746f  es from 0.7.0 to
+00004550: 2030 2e37 2e31 9461 6825 5d94 6827 5d94   0.7.1.ah%].h'].
+00004560: 7568 2968 0968 1a68 0b68 0168 0368 1b68  uh)h.h.h.h.h.h.h
+00004570: 2a68 1c4b 8975 6268 0a29 8194 7d94 2868  *h.K.ubh.)..}.(h
+00004580: 0568 0668 075d 9428 680f 2981 947d 9428  .h.h.].(h.)..}.(
+00004590: 6805 8c1b 6368 616e 6765 7320 6672 6f6d  h...changes from
+000045a0: 2030 2e36 2e35 2074 6f20 302e 372e 3094   0.6.5 to 0.7.0.
+000045b0: 6807 5d94 6815 8c1b 6368 616e 6765 7320  h.].h...changes 
+000045c0: 6672 6f6d 2030 2e36 2e35 2074 6f20 302e  from 0.6.5 to 0.
+000045d0: 372e 3094 8594 8194 7d94 2868 056a cc04  7.0.....}.(h.j..
+000045e0: 0000 681a 6aca 0400 0068 0168 0368 1b4e  ..h.j....h.h.h.N
+000045f0: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00004600: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00004610: 6829 680e 681a 6ac7 0400 0068 0168 0368  h)h.h.j....h.h.h
+00004620: 1b68 2a68 1c4b 9e75 6268 3d29 8194 7d94  .h*h.K.ubh=)..}.
+00004630: 2868 058c 4754 6865 2070 7269 6d61 7279  (h..GThe primary
+00004640: 2063 6861 6e67 6520 6973 2074 6861 7420   change is that 
+00004650: 636f 6465 2064 6576 656c 6f70 656d 656e  code developemen
+00004660: 7420 6861 7320 6265 656e 206d 6f76 6564  t has been moved
+00004670: 2074 6f20 4769 7468 7562 5f2e 9468 075d   to Github_..h.]
+00004680: 9428 6815 8c3f 5468 6520 7072 696d 6172  .(h..?The primar
+00004690: 7920 6368 616e 6765 2069 7320 7468 6174  y change is that
+000046a0: 2063 6f64 6520 6465 7665 6c6f 7065 6d65   code developeme
+000046b0: 6e74 2068 6173 2062 6565 6e20 6d6f 7665  nt has been move
+000046c0: 6420 746f 2094 8594 8194 7d94 2868 058c  d to .....}.(h..
+000046d0: 3f54 6865 2070 7269 6d61 7279 2063 6861  ?The primary cha
+000046e0: 6e67 6520 6973 2074 6861 7420 636f 6465  nge is that code
+000046f0: 2064 6576 656c 6f70 656d 656e 7420 6861   developement ha
+00004700: 7320 6265 656e 206d 6f76 6564 2074 6f20  s been moved to 
+00004710: 9468 1a6a d804 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
+00004720: 1c4e 7562 6a13 0300 0029 8194 7d94 2868  .Nubj....)..}.(h
+00004730: 058c 0747 6974 6875 625f 9468 075d 9468  ...Github_.h.].h
+00004740: 158c 0647 6974 6875 6294 8594 8194 7d94  ...Github.....}.
+00004750: 2868 0568 0668 1a6a e104 0000 7562 6168  (h.h.h.j....ubah
+00004760: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00004770: 6825 5d94 6827 5d94 8c04 6e61 6d65 948c  h%].h']...name..
+00004780: 0647 6974 6875 6294 6ac0 0300 008c 2b68  .Github.j.....+h
+00004790: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000047a0: 6d2f 6368 6961 6e74 692d 6174 6f6d 6963  m/chianti-atomic
+000047b0: 2f43 6869 616e 7469 5079 9475 6829 6a12  /ChiantiPy.uh)j.
+000047c0: 0300 0068 1a6a d804 0000 6ac2 0300 004b  ...h.j....j....K
+000047d0: 0175 6268 158c 012e 9485 9481 947d 9428  .ubh.........}.(
+000047e0: 6805 8c01 2e94 681a 6ad8 0400 0068 0168  h.....h.j....h.h
+000047f0: 0368 1b4e 681c 4e75 6265 681d 7d94 2868  .h.Nh.Nubeh.}.(h
+00004800: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+00004810: 275d 9475 6829 683c 681b 682a 681c 4ba0  '].uh)h<h.h*h.K.
+00004820: 681a 6ac7 0400 0068 0168 0375 626a e003  h.j....h.h.ubj..
+00004830: 0000 2981 947d 9428 6805 8c38 2e2e 205f  ..)..}.(h..8.. _
+00004840: 4769 7468 7562 3a20 2068 7474 7073 3a2f  Github:  https:/
+00004850: 2f67 6974 6875 622e 636f 6d2f 6368 6961  /github.com/chia
+00004860: 6e74 692d 6174 6f6d 6963 2f43 6869 616e  nti-atomic/Chian
+00004870: 7469 5079 9468 075d 9468 1d7d 9428 681f  tiPy.h.].h.}.(h.
+00004880: 5d94 8c06 6769 7468 7562 9461 6821 5d94  ]...github.ah!].
+00004890: 6823 5d94 8c06 6769 7468 7562 9461 6825  h#]...github.ah%
+000048a0: 5d94 6827 5d94 6ac0 0300 006a f104 0000  ].h'].j....j....
+000048b0: 7568 296a df03 0000 681c 4ba2 681a 6ac7  uh)j....h.K.h.j.
+000048c0: 0400 0068 0168 0368 1b68 2a6a 6a02 0000  ...h.h.h.h*jj...
+000048d0: 4b01 7562 683d 2981 947d 9428 6805 8c98  K.ubh=)..}.(h...
+000048e0: 416c 736f 2c20 696e 206f 7264 6572 2074  Also, in order t
+000048f0: 6f20 6265 206d 6f72 6520 636f 6d70 6c69  o be more compli
+00004900: 616e 7420 7769 7468 206f 7468 6572 2061  ant with other a
+00004910: 7374 726f 7068 7973 6963 616c 2070 6163  strophysical pac
+00004920: 6b61 6765 7320 6f6e 2047 6974 6875 6220  kages on Github 
+00004930: 2841 7374 726f 7079 5f20 616e 6420 5375  (Astropy_ and Su
+00004940: 6e50 795f 2920 7468 6520 6469 7265 6374  nPy_) the direct
+00004950: 6f72 7920 6c61 796f 7574 2068 6173 2062  ory layout has b
+00004960: 6565 6e20 6368 616e 6765 6420 616e 6420  een changed and 
+00004970: 7265 6e61 6d65 642e 9468 075d 9428 6815  renamed..h.].(h.
+00004980: 8c51 416c 736f 2c20 696e 206f 7264 6572  .QAlso, in order
+00004990: 2074 6f20 6265 206d 6f72 6520 636f 6d70   to be more comp
+000049a0: 6c69 616e 7420 7769 7468 206f 7468 6572  liant with other
+000049b0: 2061 7374 726f 7068 7973 6963 616c 2070   astrophysical p
+000049c0: 6163 6b61 6765 7320 6f6e 2047 6974 6875  ackages on Githu
+000049d0: 6220 2894 8594 8194 7d94 2868 058c 5141  b (.....}.(h..QA
+000049e0: 6c73 6f2c 2069 6e20 6f72 6465 7220 746f  lso, in order to
+000049f0: 2062 6520 6d6f 7265 2063 6f6d 706c 6961   be more complia
+00004a00: 6e74 2077 6974 6820 6f74 6865 7220 6173  nt with other as
+00004a10: 7472 6f70 6879 7369 6361 6c20 7061 636b  trophysical pack
+00004a20: 6167 6573 206f 6e20 4769 7468 7562 2028  ages on Github (
+00004a30: 9468 1a6a 0905 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
+00004a40: 1c4e 7562 6a13 0300 0029 8194 7d94 2868  .Nubj....)..}.(h
+00004a50: 058c 0841 7374 726f 7079 5f94 6807 5d94  ...Astropy_.h.].
+00004a60: 6815 8c07 4173 7472 6f70 7994 8594 8194  h...Astropy.....
+00004a70: 7d94 2868 0568 0668 1a6a 1205 0000 7562  }.(h.h.h.j....ub
+00004a80: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+00004a90: 5d94 6825 5d94 6827 5d94 8c04 6e61 6d65  ].h%].h']...name
+00004aa0: 948c 0741 7374 726f 7079 946a c003 0000  ...Astropy.j....
+00004ab0: 8c18 6874 7470 732f 6769 7468 7562 2e63  ..https/github.c
+00004ac0: 6f6d 2f61 7374 726f 7079 9475 6829 6a12  om/astropy.uh)j.
+00004ad0: 0300 0068 1a6a 0905 0000 6ac2 0300 004b  ...h.j....j....K
+00004ae0: 0175 6268 158c 0520 616e 6420 9485 9481  .ubh... and ....
+00004af0: 947d 9428 6805 8c05 2061 6e64 2094 681a  .}.(h... and .h.
+00004b00: 6a09 0500 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+00004b10: 626a 1303 0000 2981 947d 9428 6805 8c06  bj....)..}.(h...
+00004b20: 5375 6e50 795f 9468 075d 9468 158c 0553  SunPy_.h.].h...S
+00004b30: 756e 5079 9485 9481 947d 9428 6805 6806  unPy.....}.(h.h.
+00004b40: 681a 6a28 0500 0075 6261 681d 7d94 2868  h.j(...ubah.}.(h
+00004b50: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+00004b60: 275d 948c 046e 616d 6594 8c05 5375 6e50  ']...name...SunP
+00004b70: 7994 6ac0 0300 008c 1e68 7474 7073 3a2f  y.j......https:/
+00004b80: 2f67 6974 6875 622e 636f 6d2f 7375 6e70  /github.com/sunp
+00004b90: 792f 7375 6e70 7994 7568 296a 1203 0000  y/sunpy.uh)j....
+00004ba0: 681a 6a09 0500 006a c203 0000 4b01 7562  h.j....j....K.ub
+00004bb0: 6815 8c34 2920 7468 6520 6469 7265 6374  h..4) the direct
+00004bc0: 6f72 7920 6c61 796f 7574 2068 6173 2062  ory layout has b
+00004bd0: 6565 6e20 6368 616e 6765 6420 616e 6420  een changed and 
+00004be0: 7265 6e61 6d65 642e 9485 9481 947d 9428  renamed......}.(
+00004bf0: 6805 8c34 2920 7468 6520 6469 7265 6374  h..4) the direct
+00004c00: 6f72 7920 6c61 796f 7574 2068 6173 2062  ory layout has b
+00004c10: 6565 6e20 6368 616e 6765 6420 616e 6420  een changed and 
+00004c20: 7265 6e61 6d65 642e 9468 1a6a 0905 0000  renamed..h.j....
+00004c30: 6801 6803 681b 4e68 1c4e 7562 6568 1d7d  h.h.h.Nh.Nubeh.}
+00004c40: 9428 681f 5d94 6821 5d94 6823 5d94 6825  .(h.].h!].h#].h%
+00004c50: 5d94 6827 5d94 7568 2968 3c68 1b68 2a68  ].h'].uh)h<h.h*h
+00004c60: 1c4b a468 1a6a c704 0000 6801 6803 7562  .K.h.j....h.h.ub
+00004c70: 6ae0 0300 0029 8194 7d94 2868 058c 262e  j....)..}.(h..&.
+00004c80: 2e20 5f41 7374 726f 7079 3a20 2068 7474  . _Astropy:  htt
+00004c90: 7073 2f67 6974 6875 622e 636f 6d2f 6173  ps/github.com/as
+00004ca0: 7472 6f70 7994 6807 5d94 681d 7d94 2868  tropy.h.].h.}.(h
+00004cb0: 1f5d 948c 0761 7374 726f 7079 9461 6821  .]...astropy.ah!
+00004cc0: 5d94 6823 5d94 8c07 6173 7472 6f70 7994  ].h#]...astropy.
+00004cd0: 6168 255d 9468 275d 946a c003 0000 6a22  ah%].h'].j....j"
+00004ce0: 0500 0075 6829 6adf 0300 0068 1c4b a768  ...uh)j....h.K.h
+00004cf0: 1a6a c704 0000 6801 6803 681b 682a 6a6a  .j....h.h.h.h*jj
+00004d00: 0200 004b 0175 626a e003 0000 2981 947d  ...K.ubj....)..}
+00004d10: 9428 6805 8c2a 2e2e 205f 5375 6e50 793a  .(h..*.. _SunPy:
+00004d20: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+00004d30: 2e63 6f6d 2f73 756e 7079 2f73 756e 7079  .com/sunpy/sunpy
+00004d40: 9468 075d 9468 1d7d 9428 681f 5d94 8c05  .h.].h.}.(h.]...
+00004d50: 7375 6e70 7994 6168 215d 9468 235d 948c  sunpy.ah!].h#]..
+00004d60: 0573 756e 7079 9461 6825 5d94 6827 5d94  .sunpy.ah%].h'].
+00004d70: 6ac0 0300 006a 3805 0000 7568 296a df03  j....j8...uh)j..
+00004d80: 0000 681c 4ba8 681a 6ac7 0400 0068 0168  ..h.K.h.j....h.h
+00004d90: 0368 1b68 2a6a 6a02 0000 4b01 7562 683d  .h.h*jj...K.ubh=
+00004da0: 2981 947d 9428 6805 8c25 5468 6520 636f  )..}.(h..%The co
+00004db0: 7265 2072 6f75 7469 6e65 7320 6172 6520  re routines are 
+00004dc0: 6e6f 7720 696d 706f 7274 6564 2061 7394  now imported as.
+00004dd0: 6807 5d94 6815 8c25 5468 6520 636f 7265  h.].h..%The core
+00004de0: 2072 6f75 7469 6e65 7320 6172 6520 6e6f   routines are no
+00004df0: 7720 696d 706f 7274 6564 2061 7394 8594  w imported as...
+00004e00: 8194 7d94 2868 056a 5e05 0000 681a 6a5c  ..}.(h.j^...h.j\
+00004e10: 0500 0068 0168 0368 1b4e 681c 4e75 6261  ...h.h.h.Nh.Nuba
+00004e20: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00004e30: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+00004e40: 682a 681c 4baa 681a 6ac7 0400 0068 0168  h*h.K.h.j....h.h
+00004e50: 0375 626a 9901 0000 2981 947d 9428 6805  .ubj....)..}.(h.
+00004e60: 8c1b 696d 706f 7274 2043 6869 616e 7469  ..import Chianti
+00004e70: 5079 2e63 6f72 6520 6173 2063 6894 6807  Py.core as ch.h.
+00004e80: 5d94 6815 8c1b 696d 706f 7274 2043 6869  ].h...import Chi
+00004e90: 616e 7469 5079 2e63 6f72 6520 6173 2063  antiPy.core as c
+00004ea0: 6894 8594 8194 7d94 2868 0568 0668 1a6a  h.....}.(h.h.h.j
+00004eb0: 6a05 0000 7562 6168 1d7d 9428 681f 5d94  j...ubah.}.(h.].
+00004ec0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00004ed0: 6aa8 0100 006a a901 0000 7568 296a 9801  j....j....uh)j..
+00004ee0: 0000 681c 4bae 681a 6ac7 0400 0068 0168  ..h.K.h.j....h.h
+00004ef0: 0368 1b68 2a75 6268 3d29 8194 7d94 2868  .h.h*ubh=)..}.(h
+00004f00: 058c 2d74 6869 7320 6769 7665 2061 6363  ..-this give acc
+00004f10: 6573 7320 746f 2063 682e 696f 6e2c 2063  ess to ch.ion, c
+00004f20: 682e 7370 6563 7472 756d 2c20 6574 632e  h.spectrum, etc.
+00004f30: 9468 075d 9468 158c 2d74 6869 7320 6769  .h.].h..-this gi
+00004f40: 7665 2061 6363 6573 7320 746f 2063 682e  ve access to ch.
+00004f50: 696f 6e2c 2063 682e 7370 6563 7472 756d  ion, ch.spectrum
+00004f60: 2c20 6574 632e 9485 9481 947d 9428 6805  , etc......}.(h.
+00004f70: 6a7a 0500 0068 1a6a 7805 0000 6801 6803  jz...h.jx...h.h.
+00004f80: 681b 4e68 1c4e 7562 6168 1d7d 9428 681f  h.Nh.Nubah.}.(h.
+00004f90: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
+00004fa0: 5d94 7568 2968 3c68 1b68 2a68 1c4b b068  ].uh)h<h.h*h.K.h
+00004fb0: 1a6a c704 0000 6801 6803 7562 683d 2981  .j....h.h.ubh=).
+00004fc0: 947d 9428 6805 8c96 496e 2074 6572 6d73  .}.(h...In terms
+00004fd0: 206f 6620 6275 672d 6669 7865 732c 2074   of bug-fixes, t
+00004fe0: 6865 2063 616c 6375 6c61 7469 6f6e 206f  he calculation o
+00004ff0: 6620 6578 6369 7461 7469 6f6e 2d61 7574  f excitation-aut
+00005000: 6f69 6f6e 697a 6174 696f 6e20 6372 6f73  oionization cros
+00005010: 732d 7365 6374 696f 6e73 2061 6e64 2072  s-sections and r
+00005020: 6174 6573 2068 6176 6520 6265 656e 2063  ates have been c
+00005030: 6f72 7265 6374 6564 2069 6e20 7468 6520  orrected in the 
+00005040: 6561 4372 6f73 7328 2920 616e 6420 6561  eaCross() and ea
+00005050: 5261 7465 2829 206d 6574 686f 6473 9468  Rate() methods.h
+00005060: 075d 9468 158c 9649 6e20 7465 726d 7320  .].h...In terms 
+00005070: 6f66 2062 7567 2d66 6978 6573 2c20 7468  of bug-fixes, th
+00005080: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
+00005090: 2065 7863 6974 6174 696f 6e2d 6175 746f   excitation-auto
+000050a0: 696f 6e69 7a61 7469 6f6e 2063 726f 7373  ionization cross
+000050b0: 2d73 6563 7469 6f6e 7320 616e 6420 7261  -sections and ra
+000050c0: 7465 7320 6861 7665 2062 6565 6e20 636f  tes have been co
+000050d0: 7272 6563 7465 6420 696e 2074 6865 2065  rrected in the e
+000050e0: 6143 726f 7373 2829 2061 6e64 2065 6152  aCross() and eaR
+000050f0: 6174 6528 2920 6d65 7468 6f64 7394 8594  ate() methods...
+00005100: 8194 7d94 2868 056a 8805 0000 681a 6a86  ..}.(h.j....h.j.
+00005110: 0500 0068 0168 0368 1b4e 681c 4e75 6261  ...h.h.h.Nh.Nuba
+00005120: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00005130: 9468 255d 9468 275d 9475 6829 683c 681b  .h%].h'].uh)h<h.
+00005140: 682a 681c 4bb2 681a 6ac7 0400 0068 0168  h*h.K.h.j....h.h
+00005150: 0375 6268 3d29 8194 7d94 2868 058c 2643  .ubh=)..}.(h..&C
+00005160: 7572 7265 6e74 2064 6576 656c 6f70 6d65  urrent developme
+00005170: 6e74 2069 7320 7769 7468 2050 7974 686f  nt is with Pytho
+00005180: 6e20 332e 3494 6807 5d94 6815 8c26 4375  n 3.4.h.].h..&Cu
+00005190: 7272 656e 7420 6465 7665 6c6f 706d 656e  rrent developmen
+000051a0: 7420 6973 2077 6974 6820 5079 7468 6f6e  t is with Python
+000051b0: 2033 2e34 9485 9481 947d 9428 6805 6a96   3.4.....}.(h.j.
+000051c0: 0500 0068 1a6a 9405 0000 6801 6803 681b  ...h.j....h.h.h.
+000051d0: 4e68 1c4e 7562 6168 1d7d 9428 681f 5d94  Nh.Nubah.}.(h.].
+000051e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000051f0: 7568 2968 3c68 1b68 2a68 1c4b b468 1a6a  uh)h<h.h*h.K.h.j
+00005200: c704 0000 6801 6803 7562 6568 1d7d 9428  ....h.h.ubeh.}.(
+00005210: 681f 5d94 8c1b 6368 616e 6765 732d 6672  h.]...changes-fr
+00005220: 6f6d 2d30 2d36 2d35 2d74 6f2d 302d 372d  om-0-6-5-to-0-7-
+00005230: 3094 6168 215d 9468 235d 948c 1b63 6861  0.ah!].h#]...cha
+00005240: 6e67 6573 2066 726f 6d20 302e 362e 3520  nges from 0.6.5 
+00005250: 746f 2030 2e37 2e30 9461 6825 5d94 6827  to 0.7.0.ah%].h'
+00005260: 5d94 7568 2968 0968 1a68 0b68 0168 0368  ].uh)h.h.h.h.h.h
+00005270: 1b68 2a68 1c4b 9e75 6268 0a29 8194 7d94  .h*h.K.ubh.)..}.
+00005280: 2868 0568 0668 075d 9428 680f 2981 947d  (h.h.h.].(h.)..}
+00005290: 9428 6805 8c1b 6368 616e 6765 7320 6672  .(h...changes fr
+000052a0: 6f6d 2030 2e36 2e30 2074 6f20 302e 362e  om 0.6.0 to 0.6.
+000052b0: 3594 6807 5d94 6815 8c1b 6368 616e 6765  5.h.].h...change
+000052c0: 7320 6672 6f6d 2030 2e36 2e30 2074 6f20  s from 0.6.0 to 
+000052d0: 302e 362e 3594 8594 8194 7d94 2868 056a  0.6.5.....}.(h.j
+000052e0: af05 0000 681a 6aad 0500 0068 0168 0368  ....h.j....h.h.h
+000052f0: 1b4e 681c 4e75 6261 681d 7d94 2868 1f5d  .Nh.Nubah.}.(h.]
+00005300: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00005310: 9475 6829 680e 681a 6aaa 0500 0068 0168  .uh)h.h.j....h.h
+00005320: 0368 1b68 2a68 1c4b b775 6268 3d29 8194  .h.h*h.K.ubh=)..
+00005330: 7d94 2868 058c 2e6d 6174 706c 6f74 6c69  }.(h...matplotli
+00005340: 622e 7079 706c 6f74 2069 7320 6e6f 7720  b.pyplot is now 
+00005350: 696d 706f 7274 6564 2066 6f72 2070 6c6f  imported for plo
+00005360: 7474 696e 6794 6807 5d94 6815 8c2e 6d61  tting.h.].h...ma
+00005370: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
+00005380: 6973 206e 6f77 2069 6d70 6f72 7465 6420  is now imported 
+00005390: 666f 7220 706c 6f74 7469 6e67 9485 9481  for plotting....
+000053a0: 947d 9428 6805 6abd 0500 0068 1a6a bb05  .}.(h.j....h.j..
+000053b0: 0000 6801 6803 681b 4e68 1c4e 7562 6168  ..h.h.h.Nh.Nubah
+000053c0: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+000053d0: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
+000053e0: 2a68 1c4b b968 1a6a aa05 0000 6801 6803  *h.K.h.j....h.h.
+000053f0: 7562 683d 2981 947d 9428 6805 8c8c 4950  ubh=)..}.(h...IP
+00005400: 7974 686f 6e20 7665 7273 696f 6e20 3420  ython version 4 
+00005410: 2f20 4a75 7079 7465 7220 6973 206e 6f77  / Jupyter is now
+00005420: 206c 6973 7465 6420 6173 2061 2070 7265   listed as a pre
+00005430: 7265 7175 6973 6974 652e 2020 486f 7765  requisite.  Howe
+00005440: 7665 722c 2076 302e 362e 3420 6361 6e20  ver, v0.6.4 can 
+00005450: 6265 206d 6164 6520 636f 6d70 6174 6962  be made compatib
+00005460: 6c65 2077 6974 6820 4950 7974 686f 6e20  le with IPython 
+00005470: 3220 6f72 2033 2077 6974 6820 6120 7369  2 or 3 with a si
+00005480: 6d70 6c65 2065 6469 742e 9468 075d 9468  mple edit..h.].h
+00005490: 158c 8c49 5079 7468 6f6e 2076 6572 7369  ...IPython versi
+000054a0: 6f6e 2034 202f 204a 7570 7974 6572 2069  on 4 / Jupyter i
+000054b0: 7320 6e6f 7720 6c69 7374 6564 2061 7320  s now listed as 
+000054c0: 6120 7072 6572 6571 7569 7369 7465 2e20  a prerequisite. 
+000054d0: 2048 6f77 6576 6572 2c20 7630 2e36 2e34   However, v0.6.4
+000054e0: 2063 616e 2062 6520 6d61 6465 2063 6f6d   can be made com
+000054f0: 7061 7469 626c 6520 7769 7468 2049 5079  patible with IPy
+00005500: 7468 6f6e 2032 206f 7220 3320 7769 7468  thon 2 or 3 with
+00005510: 2061 2073 696d 706c 6520 6564 6974 2e94   a simple edit..
+00005520: 8594 8194 7d94 2868 056a cb05 0000 681a  ....}.(h.j....h.
+00005530: 6ac9 0500 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+00005540: 6261 681d 7d94 2868 1f5d 9468 215d 9468  bah.}.(h.].h!].h
+00005550: 235d 9468 255d 9468 275d 9475 6829 683c  #].h%].h'].uh)h<
+00005560: 681b 682a 681c 4bbb 681a 6aaa 0500 0068  h.h*h.K.h.j....h
+00005570: 0168 0375 6268 3d29 8194 7d94 2868 058c  .h.ubh=)..}.(h..
+00005580: 3e41 6e20 6572 726f 7220 696e 2063 616c  >An error in cal
+00005590: 6375 6c61 7469 6e67 2074 6865 2070 726f  culating the pro
+000055a0: 746f 6e20 6578 6369 7461 7469 6f6e 2072  ton excitation r
+000055b0: 6174 6573 2077 6173 2066 6978 6564 2e94  ates was fixed..
+000055c0: 6807 5d94 6815 8c3e 416e 2065 7272 6f72  h.].h..>An error
+000055d0: 2069 6e20 6361 6c63 756c 6174 696e 6720   in calculating 
+000055e0: 7468 6520 7072 6f74 6f6e 2065 7863 6974  the proton excit
+000055f0: 6174 696f 6e20 7261 7465 7320 7761 7320  ation rates was 
+00005600: 6669 7865 642e 9485 9481 947d 9428 6805  fixed......}.(h.
+00005610: 6ad9 0500 0068 1a6a d705 0000 6801 6803  j....h.j....h.h.
+00005620: 681b 4e68 1c4e 7562 6168 1d7d 9428 681f  h.Nh.Nubah.}.(h.
+00005630: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
+00005640: 5d94 7568 2968 3c68 1b68 2a68 1c4b bd68  ].uh)h<h.h*h.K.h
+00005650: 1a6a aa05 0000 6801 6803 7562 683d 2981  .j....h.h.ubh=).
+00005660: 947d 9428 6805 8c63 5468 6520 636f 6465  .}.(h..cThe code
+00005670: 2068 6173 2062 6565 6e20 6564 6974 6564   has been edited
+00005680: 2074 6f20 6d61 6b65 2069 7420 636f 6d70   to make it comp
+00005690: 6174 6962 6c65 2077 6974 6820 5079 7468  atible with Pyth
+000056a0: 6f6e 2033 2061 6e64 2068 6173 2062 6565  on 3 and has bee
+000056b0: 6e20 7465 7374 6564 2061 6761 696e 7374  n tested against
+000056c0: 2050 7974 686f 6e20 332e 3394 6807 5d94   Python 3.3.h.].
+000056d0: 6815 8c63 5468 6520 636f 6465 2068 6173  h..cThe code has
+000056e0: 2062 6565 6e20 6564 6974 6564 2074 6f20   been edited to 
+000056f0: 6d61 6b65 2069 7420 636f 6d70 6174 6962  make it compatib
+00005700: 6c65 2077 6974 6820 5079 7468 6f6e 2033  le with Python 3
+00005710: 2061 6e64 2068 6173 2062 6565 6e20 7465   and has been te
+00005720: 7374 6564 2061 6761 696e 7374 2050 7974  sted against Pyt
+00005730: 686f 6e20 332e 3394 8594 8194 7d94 2868  hon 3.3.....}.(h
+00005740: 056a e705 0000 681a 6ae5 0500 0068 0168  .j....h.j....h.h
+00005750: 0368 1b4e 681c 4e75 6261 681d 7d94 2868  .h.Nh.Nubah.}.(h
+00005760: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+00005770: 275d 9475 6829 683c 681b 682a 681c 4bbf  '].uh)h<h.h*h.K.
+00005780: 681a 6aaa 0500 0068 0168 0375 6265 681d  h.j....h.h.ubeh.
+00005790: 7d94 2868 1f5d 948c 1b63 6861 6e67 6573  }.(h.]...changes
+000057a0: 2d66 726f 6d2d 302d 362d 302d 746f 2d30  -from-0-6-0-to-0
+000057b0: 2d36 2d35 9461 6821 5d94 6823 5d94 8c1b  -6-5.ah!].h#]...
+000057c0: 6368 616e 6765 7320 6672 6f6d 2030 2e36  changes from 0.6
+000057d0: 2e30 2074 6f20 302e 362e 3594 6168 255d  .0 to 0.6.5.ah%]
+000057e0: 9468 275d 9475 6829 6809 681a 680b 6801  .h'].uh)h.h.h.h.
+000057f0: 6803 681b 682a 681c 4bb7 7562 680a 2981  h.h.h*h.K.ubh.).
+00005800: 947d 9428 6805 6806 6807 5d94 2868 0f29  .}.(h.h.h.].(h.)
+00005810: 8194 7d94 2868 058c 1b63 6861 6e67 6573  ..}.(h...changes
+00005820: 2066 726f 6d20 302e 352e 3320 746f 2030   from 0.5.3 to 0
+00005830: 2e36 2e30 9468 075d 9468 158c 1b63 6861  .6.0.h.].h...cha
+00005840: 6e67 6573 2066 726f 6d20 302e 352e 3320  nges from 0.5.3 
+00005850: 746f 2030 2e36 2e30 9485 9481 947d 9428  to 0.6.0.....}.(
+00005860: 6805 6a00 0600 0068 1a6a fe05 0000 6801  h.j....h.j....h.
+00005870: 6803 681b 4e68 1c4e 7562 6168 1d7d 9428  h.h.Nh.Nubah.}.(
+00005880: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00005890: 6827 5d94 7568 2968 0e68 1a6a fb05 0000  h'].uh)h.h.j....
+000058a0: 6801 6803 681b 682a 681c 4bc2 7562 683d  h.h.h.h*h.K.ubh=
+000058b0: 2981 947d 9428 6805 8c18 5468 6973 2069  )..}.(h...This i
+000058c0: 7320 6120 6d61 6a6f 7220 7265 6c65 6173  s a major releas
+000058d0: 652e 9468 075d 9468 158c 1854 6869 7320  e..h.].h...This 
+000058e0: 6973 2061 206d 616a 6f72 2072 656c 6561  is a major relea
+000058f0: 7365 2e94 8594 8194 7d94 2868 056a 0e06  se......}.(h.j..
+00005900: 0000 681a 6a0c 0600 0068 0168 0368 1b4e  ..h.j....h.h.h.N
+00005910: 681c 4e75 6261 681d 7d94 2868 1f5d 9468  h.Nubah.}.(h.].h
+00005920: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00005930: 6829 683c 681b 682a 681c 4bc4 681a 6afb  h)h<h.h*h.K.h.j.
+00005940: 0500 0068 0168 0375 6268 3d29 8194 7d94  ...h.h.ubh=)..}.
+00005950: 2868 0558 3c01 0000 4669 7273 742c 2043  (h.X<...First, C
+00005960: 6869 616e 7469 5079 2030 2e36 2e30 2069  hiantiPy 0.6.0 i
+00005970: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
+00005980: 6820 7468 6520 6d6f 7374 2072 6563 656e  h the most recen
+00005990: 746c 7920 7265 6c65 6173 6564 2043 4849  tly released CHI
+000059a0: 414e 5449 2064 6174 6162 6173 6520 7665  ANTI database ve
+000059b0: 7273 696f 6e20 382e 302e 2020 4974 2061  rsion 8.0.  It a
+000059c0: 6c73 6f20 6669 7865 7320 736f 6d65 206d  lso fixes some m
+000059d0: 616a 6f72 2062 7567 7320 696e 2074 6865  ajor bugs in the
+000059e0: 2070 7265 7669 6f75 7320 7665 7273 696f   previous versio
+000059f0: 6e2e 2020 446f 6375 6d65 6e74 6174 696f  n.  Documentatio
+00005a00: 6e20 6861 7320 6265 656e 2069 6d70 726f  n has been impro
+00005a10: 7665 6420 616e 6420 6120 4950 7974 686f  ved and a IPytho
+00005a20: 6e20 6e6f 7465 626f 6f6b 202a 2a51 7569  n notebook **Qui
+00005a30: 636b 5374 6172 742e 6970 796e 622a 2a2c  ckStart.ipynb**,
+00005a40: 2074 6861 7420 6c61 7267 656c 7920 666f   that largely fo
+00005a50: 6c6c 6f77 7320 7468 6520 2751 7569 636b  llows the 'Quick
+00005a60: 2053 7461 7274 2720 646f 6375 6d65 6e74   Start' document
+00005a70: 6174 696f 6e20 7061 6765 732c 2068 6173  ation pages, has
+00005a80: 2061 6c73 6f20 6265 656e 2069 6e63 6c75   also been inclu
+00005a90: 6465 642e 9468 075d 9428 6815 8cd3 4669  ded..h.].(h...Fi
+00005aa0: 7273 742c 2043 6869 616e 7469 5079 2030  rst, ChiantiPy 0
+00005ab0: 2e36 2e30 2069 7320 636f 6d70 6174 6962  .6.0 is compatib
+00005ac0: 6c65 2077 6974 6820 7468 6520 6d6f 7374  le with the most
+00005ad0: 2072 6563 656e 746c 7920 7265 6c65 6173   recently releas
+00005ae0: 6564 2043 4849 414e 5449 2064 6174 6162  ed CHIANTI datab
+00005af0: 6173 6520 7665 7273 696f 6e20 382e 302e  ase version 8.0.
+00005b00: 2020 4974 2061 6c73 6f20 6669 7865 7320    It also fixes 
+00005b10: 736f 6d65 206d 616a 6f72 2062 7567 7320  some major bugs 
+00005b20: 696e 2074 6865 2070 7265 7669 6f75 7320  in the previous 
+00005b30: 7665 7273 696f 6e2e 2020 446f 6375 6d65  version.  Docume
+00005b40: 6e74 6174 696f 6e20 6861 7320 6265 656e  ntation has been
+00005b50: 2069 6d70 726f 7665 6420 616e 6420 6120   improved and a 
+00005b60: 4950 7974 686f 6e20 6e6f 7465 626f 6f6b  IPython notebook
+00005b70: 2094 8594 8194 7d94 2868 058c d346 6972   .....}.(h...Fir
+00005b80: 7374 2c20 4368 6961 6e74 6950 7920 302e  st, ChiantiPy 0.
+00005b90: 362e 3020 6973 2063 6f6d 7061 7469 626c  6.0 is compatibl
+00005ba0: 6520 7769 7468 2074 6865 206d 6f73 7420  e with the most 
+00005bb0: 7265 6365 6e74 6c79 2072 656c 6561 7365  recently release
+00005bc0: 6420 4348 4941 4e54 4920 6461 7461 6261  d CHIANTI databa
+00005bd0: 7365 2076 6572 7369 6f6e 2038 2e30 2e20  se version 8.0. 
+00005be0: 2049 7420 616c 736f 2066 6978 6573 2073   It also fixes s
+00005bf0: 6f6d 6520 6d61 6a6f 7220 6275 6773 2069  ome major bugs i
+00005c00: 6e20 7468 6520 7072 6576 696f 7573 2076  n the previous v
+00005c10: 6572 7369 6f6e 2e20 2044 6f63 756d 656e  ersion.  Documen
+00005c20: 7461 7469 6f6e 2068 6173 2062 6565 6e20  tation has been 
+00005c30: 696d 7072 6f76 6564 2061 6e64 2061 2049  improved and a I
+00005c40: 5079 7468 6f6e 206e 6f74 6562 6f6f 6b20  Python notebook 
+00005c50: 9468 1a6a 1a06 0000 6801 6803 681b 4e68  .h.j....h.h.h.Nh
+00005c60: 1c4e 7562 6a62 0400 0029 8194 7d94 2868  .Nubjb...)..}.(h
+00005c70: 058c 142a 2a51 7569 636b 5374 6172 742e  ...**QuickStart.
+00005c80: 6970 796e 622a 2a94 6807 5d94 6815 8c10  ipynb**.h.].h...
+00005c90: 5175 6963 6b53 7461 7274 2e69 7079 6e62  QuickStart.ipynb
+00005ca0: 9485 9481 947d 9428 6805 6806 681a 6a23  .....}.(h.h.h.j#
+00005cb0: 0600 0075 6261 681d 7d94 2868 1f5d 9468  ...ubah.}.(h.].h
+00005cc0: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00005cd0: 6829 6a61 0400 0068 1a6a 1a06 0000 7562  h)ja...h.j....ub
+00005ce0: 6815 8c59 2c20 7468 6174 206c 6172 6765  h..Y, that large
+00005cf0: 6c79 2066 6f6c 6c6f 7773 2074 6865 20e2  ly follows the .
+00005d00: 8098 5175 6963 6b20 5374 6172 74e2 8099  ..Quick Start...
+00005d10: 2064 6f63 756d 656e 7461 7469 6f6e 2070   documentation p
+00005d20: 6167 6573 2c20 6861 7320 616c 736f 2062  ages, has also b
+00005d30: 6565 6e20 696e 636c 7564 6564 2e94 8594  een included....
+00005d40: 8194 7d94 2868 058c 552c 2074 6861 7420  ..}.(h..U, that 
+00005d50: 6c61 7267 656c 7920 666f 6c6c 6f77 7320  largely follows 
+00005d60: 7468 6520 2751 7569 636b 2053 7461 7274  the 'Quick Start
+00005d70: 2720 646f 6375 6d65 6e74 6174 696f 6e20  ' documentation 
+00005d80: 7061 6765 732c 2068 6173 2061 6c73 6f20  pages, has also 
+00005d90: 6265 656e 2069 6e63 6c75 6465 642e 9468  been included..h
+00005da0: 1a6a 1a06 0000 6801 6803 681b 4e68 1c4e  .j....h.h.h.Nh.N
+00005db0: 7562 6568 1d7d 9428 681f 5d94 6821 5d94  ubeh.}.(h.].h!].
+00005dc0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+00005dd0: 3c68 1b68 2a68 1c4b c668 1a6a fb05 0000  <h.h*h.K.h.j....
+00005de0: 6801 6803 7562 683d 2981 947d 9428 6805  h.h.ubh=)..}.(h.
+00005df0: 586e 0100 0054 6865 7265 2061 7265 2074  Xn...There are t
+00005e00: 776f 206e 6577 206d 756c 7469 2d69 6f6e  wo new multi-ion
+00005e10: 2063 6c61 7373 6573 3a20 202a 2a62 756e   classes:  **bun
+00005e20: 6368 2a2a 2061 6e64 202a 2a69 7079 6d73  ch** and **ipyms
+00005e30: 7065 6374 7275 6d2a 2a2e 2020 2a2a 6275  pectrum**.  **bu
+00005e40: 6e63 682a 2a20 616c 6c6f 7773 2074 6865  nch** allows the
+00005e50: 2075 7365 7220 746f 2063 616c 6375 6c61   user to calcula
+00005e60: 7465 206c 696e 6520 696e 7465 6e73 6974  te line intensit
+00005e70: 6965 7320 666f 7220 6120 7370 6563 6966  ies for a specif
+00005e80: 6965 6420 7365 7420 6f66 2065 6c65 6d65  ied set of eleme
+00005e90: 6e74 7320 6f72 2069 6e64 6976 6964 7561  nts or individua
+00005ea0: 6c20 696f 6e73 2061 7320 6120 6675 6e63  l ions as a func
+00005eb0: 7469 6f6e 206f 6620 7465 6d70 6572 6174  tion of temperat
+00005ec0: 7572 6520 6f72 2064 656e 7369 7479 2e20  ure or density. 
+00005ed0: 204f 6e65 2061 6476 616e 7461 6765 206f   One advantage o
+00005ee0: 6620 2a2a 6275 6e63 682a 2a20 6973 2074  f **bunch** is t
+00005ef0: 6865 2061 6269 6c69 7479 2074 6f20 6361  he ability to ca
+00005f00: 6c63 756c 6174 6520 7468 6520 696e 7465  lculate the inte
+00005f10: 6e73 6974 7920 7261 7469 6f20 6f66 206c  nsity ratio of l
+00005f20: 696e 6573 206f 6620 7477 6f20 6469 6666  ines of two diff
+00005f30: 6572 656e 7420 696f 6e73 2061 7320 6120  erent ions as a 
+00005f40: 6675 6e63 7469 6f6e 206f 6620 7465 6d70  function of temp
+00005f50: 6572 6174 7572 6520 6f72 2064 656e 7369  erature or densi
+00005f60: 7479 2e94 6807 5d94 2868 158c 2654 6865  ty..h.].(h..&The
+00005f70: 7265 2061 7265 2074 776f 206e 6577 206d  re are two new m
+00005f80: 756c 7469 2d69 6f6e 2063 6c61 7373 6573  ulti-ion classes
+00005f90: 3a20 2094 8594 8194 7d94 2868 058c 2654  :  .....}.(h..&T
+00005fa0: 6865 7265 2061 7265 2074 776f 206e 6577  here are two new
+00005fb0: 206d 756c 7469 2d69 6f6e 2063 6c61 7373   multi-ion class
+00005fc0: 6573 3a20 2094 681a 6a3c 0600 0068 0168  es:  .h.j<...h.h
+00005fd0: 0368 1b4e 681c 4e75 626a 6204 0000 2981  .h.Nh.Nubjb...).
+00005fe0: 947d 9428 6805 8c09 2a2a 6275 6e63 682a  .}.(h...**bunch*
+00005ff0: 2a94 6807 5d94 6815 8c05 6275 6e63 6894  *.h.].h...bunch.
+00006000: 8594 8194 7d94 2868 0568 0668 1a6a 4506  ....}.(h.h.h.jE.
+00006010: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
+00006020: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
+00006030: 296a 6104 0000 681a 6a3c 0600 0075 6268  )ja...h.j<...ubh
+00006040: 158c 0520 616e 6420 9485 9481 947d 9428  ... and .....}.(
+00006050: 6805 8c05 2061 6e64 2094 681a 6a3c 0600  h... and .h.j<..
+00006060: 0068 0168 0368 1b4e 681c 4e75 626a 6204  .h.h.h.Nh.Nubjb.
+00006070: 0000 2981 947d 9428 6805 8c10 2a2a 6970  ..)..}.(h...**ip
+00006080: 796d 7370 6563 7472 756d 2a2a 9468 075d  ymspectrum**.h.]
+00006090: 9468 158c 0c69 7079 6d73 7065 6374 7275  .h...ipymspectru
+000060a0: 6d94 8594 8194 7d94 2868 0568 0668 1a6a  m.....}.(h.h.h.j
+000060b0: 5806 0000 7562 6168 1d7d 9428 681f 5d94  X...ubah.}.(h.].
+000060c0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000060d0: 7568 296a 6104 0000 681a 6a3c 0600 0075  uh)ja...h.j<...u
+000060e0: 6268 158c 032e 2020 9485 9481 947d 9428  bh....  .....}.(
+000060f0: 6805 8c03 2e20 2094 681a 6a3c 0600 0068  h....  .h.j<...h
+00006100: 0168 0368 1b4e 681c 4e75 626a 6204 0000  .h.h.Nh.Nubjb...
+00006110: 2981 947d 9428 6805 8c09 2a2a 6275 6e63  )..}.(h...**bunc
+00006120: 682a 2a94 6807 5d94 6815 8c05 6275 6e63  h**.h.].h...bunc
+00006130: 6894 8594 8194 7d94 2868 0568 0668 1a6a  h.....}.(h.h.h.j
+00006140: 6b06 0000 7562 6168 1d7d 9428 681f 5d94  k...ubah.}.(h.].
+00006150: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00006160: 7568 296a 6104 0000 681a 6a3c 0600 0075  uh)ja...h.j<...u
+00006170: 6268 158c 9d20 616c 6c6f 7773 2074 6865  bh... allows the
+00006180: 2075 7365 7220 746f 2063 616c 6375 6c61   user to calcula
+00006190: 7465 206c 696e 6520 696e 7465 6e73 6974  te line intensit
+000061a0: 6965 7320 666f 7220 6120 7370 6563 6966  ies for a specif
+000061b0: 6965 6420 7365 7420 6f66 2065 6c65 6d65  ied set of eleme
+000061c0: 6e74 7320 6f72 2069 6e64 6976 6964 7561  nts or individua
+000061d0: 6c20 696f 6e73 2061 7320 6120 6675 6e63  l ions as a func
+000061e0: 7469 6f6e 206f 6620 7465 6d70 6572 6174  tion of temperat
+000061f0: 7572 6520 6f72 2064 656e 7369 7479 2e20  ure or density. 
+00006200: 204f 6e65 2061 6476 616e 7461 6765 206f   One advantage o
+00006210: 6620 9485 9481 947d 9428 6805 8c9d 2061  f .....}.(h... a
+00006220: 6c6c 6f77 7320 7468 6520 7573 6572 2074  llows the user t
+00006230: 6f20 6361 6c63 756c 6174 6520 6c69 6e65  o calculate line
+00006240: 2069 6e74 656e 7369 7469 6573 2066 6f72   intensities for
+00006250: 2061 2073 7065 6369 6669 6564 2073 6574   a specified set
+00006260: 206f 6620 656c 656d 656e 7473 206f 7220   of elements or 
+00006270: 696e 6469 7669 6475 616c 2069 6f6e 7320  individual ions 
+00006280: 6173 2061 2066 756e 6374 696f 6e20 6f66  as a function of
+00006290: 2074 656d 7065 7261 7475 7265 206f 7220   temperature or 
+000062a0: 6465 6e73 6974 792e 2020 4f6e 6520 6164  density.  One ad
+000062b0: 7661 6e74 6167 6520 6f66 2094 681a 6a3c  vantage of .h.j<
+000062c0: 0600 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
+000062d0: 6204 0000 2981 947d 9428 6805 8c09 2a2a  b...)..}.(h...**
+000062e0: 6275 6e63 682a 2a94 6807 5d94 6815 8c05  bunch**.h.].h...
+000062f0: 6275 6e63 6894 8594 8194 7d94 2868 0568  bunch.....}.(h.h
+00006300: 0668 1a6a 7e06 0000 7562 6168 1d7d 9428  .h.j~...ubah.}.(
+00006310: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00006320: 6827 5d94 7568 296a 6104 0000 681a 6a3c  h'].uh)ja...h.j<
+00006330: 0600 0075 6268 158c 7820 6973 2074 6865  ...ubh..x is the
+00006340: 2061 6269 6c69 7479 2074 6f20 6361 6c63   ability to calc
+00006350: 756c 6174 6520 7468 6520 696e 7465 6e73  ulate the intens
+00006360: 6974 7920 7261 7469 6f20 6f66 206c 696e  ity ratio of lin
+00006370: 6573 206f 6620 7477 6f20 6469 6666 6572  es of two differ
+00006380: 656e 7420 696f 6e73 2061 7320 6120 6675  ent ions as a fu
+00006390: 6e63 7469 6f6e 206f 6620 7465 6d70 6572  nction of temper
+000063a0: 6174 7572 6520 6f72 2064 656e 7369 7479  ature or density
+000063b0: 2e94 8594 8194 7d94 2868 058c 7820 6973  ......}.(h..x is
+000063c0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
+000063d0: 6361 6c63 756c 6174 6520 7468 6520 696e  calculate the in
+000063e0: 7465 6e73 6974 7920 7261 7469 6f20 6f66  tensity ratio of
+000063f0: 206c 696e 6573 206f 6620 7477 6f20 6469   lines of two di
+00006400: 6666 6572 656e 7420 696f 6e73 2061 7320  fferent ions as 
+00006410: 6120 6675 6e63 7469 6f6e 206f 6620 7465  a function of te
+00006420: 6d70 6572 6174 7572 6520 6f72 2064 656e  mperature or den
+00006430: 7369 7479 2e94 681a 6a3c 0600 0068 0168  sity..h.j<...h.h
+00006440: 0368 1b4e 681c 4e75 6265 681d 7d94 2868  .h.Nh.Nubeh.}.(h
+00006450: 1f5d 9468 215d 9468 235d 9468 255d 9468  .].h!].h#].h%].h
+00006460: 275d 9475 6829 683c 681b 682a 681c 4bc8  '].uh)h<h.h*h.K.
+00006470: 681a 6afb 0500 0068 0168 0375 6268 3d29  h.j....h.h.ubh=)
+00006480: 8194 7d94 2868 0558 6301 0000 2a2a 6970  ..}.(h.Xc...**ip
+00006490: 796d 7370 6563 7472 756d 2a2a 2069 7320  ymspectrum** is 
+000064a0: 6d75 6368 206c 696b 6520 7468 6520 6578  much like the ex
+000064b0: 6973 7469 6e67 202a 2a73 7065 6374 7275  isting **spectru
+000064c0: 6d2a 2a20 616e 6420 2a2a 6d73 7065 6374  m** and **mspect
+000064d0: 7275 6d2a 2a20 636c 6173 7365 732e 2020  rum** classes.  
+000064e0: 2a2a 6d73 7065 6374 7275 6d2a 2a20 616c  **mspectrum** al
+000064f0: 6c6f 7773 2074 6865 2075 7365 206f 6620  lows the use of 
+00006500: 7468 6520 5079 7468 6f6e 202a 2a6d 756c  the Python **mul
+00006510: 7469 7072 6f63 6573 7369 6e67 2a2a 206d  tiprocessing** m
+00006520: 6f64 756c 6520 746f 2073 7065 6564 2075  odule to speed u
+00006530: 7020 7370 6563 7472 616c 2063 616c 6375  p spectral calcu
+00006540: 6c61 7469 6f6e 732e 2020 5468 6520 2a2a  lations.  The **
+00006550: 6970 796d 7370 6563 7472 756d 2a2a 2063  ipymspectrum** c
+00006560: 6c61 7373 2075 7365 7320 7468 6520 4950  lass uses the IP
+00006570: 7974 686f 6e20 2a2a 7061 7261 6c6c 656c  ython **parallel
+00006580: 2a2a 206d 6f64 756c 6520 736f 2074 6861  ** module so tha
+00006590: 7420 6d75 6c74 6970 726f 6365 7373 696e  t multiprocessin
+000065a0: 6720 7370 6563 7472 616c 2063 616c 6375  g spectral calcu
+000065b0: 6c61 7469 6f6e 7320 6361 6e20 6265 2070  lations can be p
+000065c0: 6572 666f 726d 6564 2069 6e20 7468 6520  erformed in the 
+000065d0: 4950 7974 686f 6e20 5174 436f 6e73 6f6c  IPython QtConsol
+000065e0: 6520 616e 6420 4e6f 7465 626f 6f6b 2e94  e and Notebook..
+000065f0: 6807 5d94 286a 6204 0000 2981 947d 9428  h.].(jb...)..}.(
+00006600: 6805 8c10 2a2a 6970 796d 7370 6563 7472  h...**ipymspectr
+00006610: 756d 2a2a 9468 075d 9468 158c 0c69 7079  um**.h.].h...ipy
+00006620: 6d73 7065 6374 7275 6d94 8594 8194 7d94  mspectrum.....}.
+00006630: 2868 0568 0668 1a6a 9b06 0000 7562 6168  (h.h.h.j....ubah
+00006640: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00006650: 6825 5d94 6827 5d94 7568 296a 6104 0000  h%].h'].uh)ja...
+00006660: 681a 6a97 0600 0075 6268 158c 1b20 6973  h.j....ubh... is
+00006670: 206d 7563 6820 6c69 6b65 2074 6865 2065   much like the e
+00006680: 7869 7374 696e 6720 9485 9481 947d 9428  xisting .....}.(
+00006690: 6805 8c1b 2069 7320 6d75 6368 206c 696b  h... is much lik
+000066a0: 6520 7468 6520 6578 6973 7469 6e67 2094  e the existing .
+000066b0: 681a 6a97 0600 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+000066c0: 4e75 626a 6204 0000 2981 947d 9428 6805  Nubjb...)..}.(h.
+000066d0: 8c0c 2a2a 7370 6563 7472 756d 2a2a 9468  ..**spectrum**.h
+000066e0: 075d 9468 158c 0873 7065 6374 7275 6d94  .].h...spectrum.
+000066f0: 8594 8194 7d94 2868 0568 0668 1a6a ae06  ....}.(h.h.h.j..
+00006700: 0000 7562 6168 1d7d 9428 681f 5d94 6821  ..ubah.}.(h.].h!
+00006710: 5d94 6823 5d94 6825 5d94 6827 5d94 7568  ].h#].h%].h'].uh
+00006720: 296a 6104 0000 681a 6a97 0600 0075 6268  )ja...h.j....ubh
+00006730: 158c 0520 616e 6420 9485 9481 947d 9428  ... and .....}.(
+00006740: 6805 8c05 2061 6e64 2094 681a 6a97 0600  h... and .h.j...
+00006750: 0068 0168 0368 1b4e 681c 4e75 626a 6204  .h.h.h.Nh.Nubjb.
+00006760: 0000 2981 947d 9428 6805 8c0d 2a2a 6d73  ..)..}.(h...**ms
+00006770: 7065 6374 7275 6d2a 2a94 6807 5d94 6815  pectrum**.h.].h.
+00006780: 8c09 6d73 7065 6374 7275 6d94 8594 8194  ..mspectrum.....
+00006790: 7d94 2868 0568 0668 1a6a c106 0000 7562  }.(h.h.h.j....ub
+000067a0: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+000067b0: 5d94 6825 5d94 6827 5d94 7568 296a 6104  ].h%].h'].uh)ja.
+000067c0: 0000 681a 6a97 0600 0075 6268 158c 0b20  ..h.j....ubh... 
+000067d0: 636c 6173 7365 732e 2020 9485 9481 947d  classes.  .....}
+000067e0: 9428 6805 8c0b 2063 6c61 7373 6573 2e20  .(h... classes. 
+000067f0: 2094 681a 6a97 0600 0068 0168 0368 1b4e   .h.j....h.h.h.N
+00006800: 681c 4e75 626a 6204 0000 2981 947d 9428  h.Nubjb...)..}.(
+00006810: 6805 8c0d 2a2a 6d73 7065 6374 7275 6d2a  h...**mspectrum*
+00006820: 2a94 6807 5d94 6815 8c09 6d73 7065 6374  *.h.].h...mspect
+00006830: 7275 6d94 8594 8194 7d94 2868 0568 0668  rum.....}.(h.h.h
+00006840: 1a6a d406 0000 7562 6168 1d7d 9428 681f  .j....ubah.}.(h.
+00006850: 5d94 6821 5d94 6823 5d94 6825 5d94 6827  ].h!].h#].h%].h'
+00006860: 5d94 7568 296a 6104 0000 681a 6a97 0600  ].uh)ja...h.j...
+00006870: 0075 6268 158c 1e20 616c 6c6f 7773 2074  .ubh... allows t
+00006880: 6865 2075 7365 206f 6620 7468 6520 5079  he use of the Py
+00006890: 7468 6f6e 2094 8594 8194 7d94 2868 058c  thon .....}.(h..
+000068a0: 1e20 616c 6c6f 7773 2074 6865 2075 7365  . allows the use
+000068b0: 206f 6620 7468 6520 5079 7468 6f6e 2094   of the Python .
+000068c0: 681a 6a97 0600 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+000068d0: 4e75 626a 6204 0000 2981 947d 9428 6805  Nubjb...)..}.(h.
+000068e0: 8c13 2a2a 6d75 6c74 6970 726f 6365 7373  ..**multiprocess
+000068f0: 696e 672a 2a94 6807 5d94 6815 8c0f 6d75  ing**.h.].h...mu
+00006900: 6c74 6970 726f 6365 7373 696e 6794 8594  ltiprocessing...
+00006910: 8194 7d94 2868 0568 0668 1a6a e706 0000  ..}.(h.h.h.j....
+00006920: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00006930: 6823 5d94 6825 5d94 6827 5d94 7568 296a  h#].h%].h'].uh)j
+00006940: 6104 0000 681a 6a97 0600 0075 6268 158c  a...h.j....ubh..
+00006950: 3020 6d6f 6475 6c65 2074 6f20 7370 6565  0 module to spee
+00006960: 6420 7570 2073 7065 6374 7261 6c20 6361  d up spectral ca
+00006970: 6c63 756c 6174 696f 6e73 2e20 2054 6865  lculations.  The
+00006980: 2094 8594 8194 7d94 2868 058c 3020 6d6f   .....}.(h..0 mo
+00006990: 6475 6c65 2074 6f20 7370 6565 6420 7570  dule to speed up
+000069a0: 2073 7065 6374 7261 6c20 6361 6c63 756c   spectral calcul
+000069b0: 6174 696f 6e73 2e20 2054 6865 2094 681a  ations.  The .h.
+000069c0: 6a97 0600 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+000069d0: 626a 6204 0000 2981 947d 9428 6805 8c10  bjb...)..}.(h...
+000069e0: 2a2a 6970 796d 7370 6563 7472 756d 2a2a  **ipymspectrum**
+000069f0: 9468 075d 9468 158c 0c69 7079 6d73 7065  .h.].h...ipymspe
+00006a00: 6374 7275 6d94 8594 8194 7d94 2868 0568  ctrum.....}.(h.h
+00006a10: 0668 1a6a fa06 0000 7562 6168 1d7d 9428  .h.j....ubah.}.(
+00006a20: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00006a30: 6827 5d94 7568 296a 6104 0000 681a 6a97  h'].uh)ja...h.j.
+00006a40: 0600 0075 6268 158c 1820 636c 6173 7320  ...ubh... class 
+00006a50: 7573 6573 2074 6865 2049 5079 7468 6f6e  uses the IPython
+00006a60: 2094 8594 8194 7d94 2868 058c 1820 636c   .....}.(h... cl
+00006a70: 6173 7320 7573 6573 2074 6865 2049 5079  ass uses the IPy
+00006a80: 7468 6f6e 2094 681a 6a97 0600 0068 0168  thon .h.j....h.h
+00006a90: 0368 1b4e 681c 4e75 626a 6204 0000 2981  .h.Nh.Nubjb...).
+00006aa0: 947d 9428 6805 8c0c 2a2a 7061 7261 6c6c  .}.(h...**parall
+00006ab0: 656c 2a2a 9468 075d 9468 158c 0870 6172  el**.h.].h...par
+00006ac0: 616c 6c65 6c94 8594 8194 7d94 2868 0568  allel.....}.(h.h
+00006ad0: 0668 1a6a 0d07 0000 7562 6168 1d7d 9428  .h.j....ubah.}.(
+00006ae0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00006af0: 6827 5d94 7568 296a 6104 0000 681a 6a97  h'].uh)ja...h.j.
+00006b00: 0600 0075 6268 158c 6d20 6d6f 6475 6c65  ...ubh..m module
+00006b10: 2073 6f20 7468 6174 206d 756c 7469 7072   so that multipr
+00006b20: 6f63 6573 7369 6e67 2073 7065 6374 7261  ocessing spectra
+00006b30: 6c20 6361 6c63 756c 6174 696f 6e73 2063  l calculations c
+00006b40: 616e 2062 6520 7065 7266 6f72 6d65 6420  an be performed 
+00006b50: 696e 2074 6865 2049 5079 7468 6f6e 2051  in the IPython Q
+00006b60: 7443 6f6e 736f 6c65 2061 6e64 204e 6f74  tConsole and Not
+00006b70: 6562 6f6f 6b2e 9485 9481 947d 9428 6805  ebook......}.(h.
+00006b80: 8c6d 206d 6f64 756c 6520 736f 2074 6861  .m module so tha
+00006b90: 7420 6d75 6c74 6970 726f 6365 7373 696e  t multiprocessin
+00006ba0: 6720 7370 6563 7472 616c 2063 616c 6375  g spectral calcu
+00006bb0: 6c61 7469 6f6e 7320 6361 6e20 6265 2070  lations can be p
+00006bc0: 6572 666f 726d 6564 2069 6e20 7468 6520  erformed in the 
+00006bd0: 4950 7974 686f 6e20 5174 436f 6e73 6f6c  IPython QtConsol
+00006be0: 6520 616e 6420 4e6f 7465 626f 6f6b 2e94  e and Notebook..
+00006bf0: 681a 6a97 0600 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+00006c00: 4e75 6265 681d 7d94 2868 1f5d 9468 215d  Nubeh.}.(h.].h!]
+00006c10: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00006c20: 683c 681b 682a 681c 4bca 681a 6afb 0500  h<h.h*h.K.h.j...
+00006c30: 0068 0168 0375 6268 3d29 8194 7d94 2868  .h.h.ubh=)..}.(h
+00006c40: 0558 2e01 0000 4120 6e65 7720 6d65 7468  .X....A new meth
+00006c50: 6f64 202a 2a69 6e74 656e 7369 7479 4c69  od **intensityLi
+00006c60: 7374 2a2a 2068 6173 2062 6565 6e20 6465  st** has been de
+00006c70: 7665 6c6f 7065 6420 746f 2061 6c6c 6f77  veloped to allow
+00006c80: 2074 6865 2075 7365 7220 746f 206c 6973   the user to lis
+00006c90: 7420 7468 6520 6d6f 7374 2069 6e74 656e  t the most inten
+00006ca0: 7365 206c 696e 6573 2077 6974 6869 6e20  se lines within 
+00006cb0: 6120 6769 7665 6e20 7761 7665 6c65 6e67  a given waveleng
+00006cc0: 7468 2072 616e 6765 2e20 2054 6869 7320  th range.  This 
+00006cd0: 6e65 7720 6d65 7468 6f64 732c 2074 6f67  new methods, tog
+00006ce0: 6574 6865 7220 7769 7468 2070 7265 7669  ether with previ
+00006cf0: 6f75 736c 7920 6578 6973 7469 6e67 202a  ously existing *
+00006d00: 2a69 6e74 656e 7369 7479 5261 7469 6f2a  *intensityRatio*
+00006d10: 2a20 616e 6420 2a2a 696e 7465 6e73 6974  * and **intensit
+00006d20: 7952 6174 696f 5361 7665 2a2a 2061 7265  yRatioSave** are
+00006d30: 2061 6c6c 206e 6f77 2069 6e68 6572 6974   all now inherit
+00006d40: 6564 2062 7920 7468 6520 2a2a 696f 6e2a  ed by the **ion*
+00006d50: 2a20 636c 6173 7373 2061 6e64 2074 6865  * classs and the
+00006d60: 2020 6d75 6c74 692d 696f 6e20 636c 6173    multi-ion clas
+00006d70: 7365 732e 9468 075d 9428 6815 8c0d 4120  ses..h.].(h...A 
+00006d80: 6e65 7720 6d65 7468 6f64 2094 8594 8194  new method .....
+00006d90: 7d94 2868 058c 0d41 206e 6577 206d 6574  }.(h...A new met
+00006da0: 686f 6420 9468 1a6a 2607 0000 6801 6803  hod .h.j&...h.h.
+00006db0: 681b 4e68 1c4e 7562 6a62 0400 0029 8194  h.Nh.Nubjb...)..
+00006dc0: 7d94 2868 058c 112a 2a69 6e74 656e 7369  }.(h...**intensi
+00006dd0: 7479 4c69 7374 2a2a 9468 075d 9468 158c  tyList**.h.].h..
+00006de0: 0d69 6e74 656e 7369 7479 4c69 7374 9485  .intensityList..
+00006df0: 9481 947d 9428 6805 6806 681a 6a2f 0700  ...}.(h.h.h.j/..
+00006e00: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
+00006e10: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+00006e20: 6a61 0400 0068 1a6a 2607 0000 7562 6815  ja...h.j&...ubh.
+00006e30: 8c9b 2068 6173 2062 6565 6e20 6465 7665  .. has been deve
+00006e40: 6c6f 7065 6420 746f 2061 6c6c 6f77 2074  loped to allow t
+00006e50: 6865 2075 7365 7220 746f 206c 6973 7420  he user to list 
+00006e60: 7468 6520 6d6f 7374 2069 6e74 656e 7365  the most intense
+00006e70: 206c 696e 6573 2077 6974 6869 6e20 6120   lines within a 
+00006e80: 6769 7665 6e20 7761 7665 6c65 6e67 7468  given wavelength
+00006e90: 2072 616e 6765 2e20 2054 6869 7320 6e65   range.  This ne
+00006ea0: 7720 6d65 7468 6f64 732c 2074 6f67 6574  w methods, toget
+00006eb0: 6865 7220 7769 7468 2070 7265 7669 6f75  her with previou
+00006ec0: 736c 7920 6578 6973 7469 6e67 2094 8594  sly existing ...
+00006ed0: 8194 7d94 2868 058c 9b20 6861 7320 6265  ..}.(h... has be
+00006ee0: 656e 2064 6576 656c 6f70 6564 2074 6f20  en developed to 
+00006ef0: 616c 6c6f 7720 7468 6520 7573 6572 2074  allow the user t
+00006f00: 6f20 6c69 7374 2074 6865 206d 6f73 7420  o list the most 
+00006f10: 696e 7465 6e73 6520 6c69 6e65 7320 7769  intense lines wi
+00006f20: 7468 696e 2061 2067 6976 656e 2077 6176  thin a given wav
+00006f30: 656c 656e 6774 6820 7261 6e67 652e 2020  elength range.  
+00006f40: 5468 6973 206e 6577 206d 6574 686f 6473  This new methods
+00006f50: 2c20 746f 6765 7468 6572 2077 6974 6820  , together with 
+00006f60: 7072 6576 696f 7573 6c79 2065 7869 7374  previously exist
+00006f70: 696e 6720 9468 1a6a 2607 0000 6801 6803  ing .h.j&...h.h.
+00006f80: 681b 4e68 1c4e 7562 6a62 0400 0029 8194  h.Nh.Nubjb...)..
+00006f90: 7d94 2868 058c 122a 2a69 6e74 656e 7369  }.(h...**intensi
+00006fa0: 7479 5261 7469 6f2a 2a94 6807 5d94 6815  tyRatio**.h.].h.
+00006fb0: 8c0e 696e 7465 6e73 6974 7952 6174 696f  ..intensityRatio
+00006fc0: 9485 9481 947d 9428 6805 6806 681a 6a42  .....}.(h.h.h.jB
+00006fd0: 0700 0075 6261 681d 7d94 2868 1f5d 9468  ...ubah.}.(h.].h
+00006fe0: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00006ff0: 6829 6a61 0400 0068 1a6a 2607 0000 7562  h)ja...h.j&...ub
+00007000: 6815 8c05 2061 6e64 2094 8594 8194 7d94  h... and .....}.
+00007010: 2868 058c 0520 616e 6420 9468 1a6a 2607  (h... and .h.j&.
+00007020: 0000 6801 6803 681b 4e68 1c4e 7562 6a62  ..h.h.h.Nh.Nubjb
+00007030: 0400 0029 8194 7d94 2868 058c 162a 2a69  ...)..}.(h...**i
+00007040: 6e74 656e 7369 7479 5261 7469 6f53 6176  ntensityRatioSav
+00007050: 652a 2a94 6807 5d94 6815 8c12 696e 7465  e**.h.].h...inte
+00007060: 6e73 6974 7952 6174 696f 5361 7665 9485  nsityRatioSave..
+00007070: 9481 947d 9428 6805 6806 681a 6a55 0700  ...}.(h.h.h.jU..
+00007080: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
+00007090: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+000070a0: 6a61 0400 0068 1a6a 2607 0000 7562 6815  ja...h.j&...ubh.
+000070b0: 8c1e 2061 7265 2061 6c6c 206e 6f77 2069  .. are all now i
+000070c0: 6e68 6572 6974 6564 2062 7920 7468 6520  nherited by the 
+000070d0: 9485 9481 947d 9428 6805 8c1e 2061 7265  .....}.(h... are
+000070e0: 2061 6c6c 206e 6f77 2069 6e68 6572 6974   all now inherit
+000070f0: 6564 2062 7920 7468 6520 9468 1a6a 2607  ed by the .h.j&.
+00007100: 0000 6801 6803 681b 4e68 1c4e 7562 6a62  ..h.h.h.Nh.Nubjb
+00007110: 0400 0029 8194 7d94 2868 058c 072a 2a69  ...)..}.(h...**i
+00007120: 6f6e 2a2a 9468 075d 9468 158c 0369 6f6e  on**.h.].h...ion
+00007130: 9485 9481 947d 9428 6805 6806 681a 6a68  .....}.(h.h.h.jh
+00007140: 0700 0075 6261 681d 7d94 2868 1f5d 9468  ...ubah.}.(h.].h
+00007150: 215d 9468 235d 9468 255d 9468 275d 9475  !].h#].h%].h'].u
+00007160: 6829 6a61 0400 0068 1a6a 2607 0000 7562  h)ja...h.j&...ub
+00007170: 6815 8c23 2063 6c61 7373 7320 616e 6420  h..# classs and 
+00007180: 7468 6520 206d 756c 7469 2d69 6f6e 2063  the  multi-ion c
+00007190: 6c61 7373 6573 2e94 8594 8194 7d94 2868  lasses......}.(h
+000071a0: 058c 2320 636c 6173 7373 2061 6e64 2074  ..# classs and t
+000071b0: 6865 2020 6d75 6c74 692d 696f 6e20 636c  he  multi-ion cl
+000071c0: 6173 7365 732e 9468 1a6a 2607 0000 6801  asses..h.j&...h.
+000071d0: 6803 681b 4e68 1c4e 7562 6568 1d7d 9428  h.h.Nh.Nubeh.}.(
+000071e0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+000071f0: 6827 5d94 7568 2968 3c68 1b68 2a68 1c4b  h'].uh)h<h.h*h.K
+00007200: cc68 1a6a fb05 0000 6801 6803 7562 683d  .h.j....h.h.ubh=
+00007210: 2981 947d 9428 6805 8cbf 5468 6520 2a2a  )..}.(h...The **
+00007220: 696f 6e2a 2a20 616e 6420 6d75 6c74 692d  ion** and multi-
+00007230: 696f 6e20 636c 6173 7365 7320 6e6f 7720  ion classes now 
+00007240: 6163 6365 7074 2074 6865 206b 6579 776f  accept the keywo
+00007250: 7264 2061 7267 756d 656e 7420 2a2a 6162  rd argument **ab
+00007260: 756e 6461 6e63 654e 616d 652a 2a20 7468  undanceName** th
+00007270: 6174 2061 6c6c 6f77 2074 6865 2075 7365  at allow the use
+00007280: 7220 746f 2073 7065 6369 6679 2074 6865  r to specify the
+00007290: 2073 6574 206f 6620 656c 656d 656e 7461   set of elementa
+000072a0: 6c20 6162 756e 6461 6e63 6573 2072 6174  l abundances rat
+000072b0: 6865 7220 7468 616e 206a 7573 7420 7468  her than just th
+000072c0: 6520 6465 6661 756c 7420 6162 756e 6461  e default abunda
+000072d0: 6e63 6520 6669 6c65 2e94 6807 5d94 2868  nce file..h.].(h
+000072e0: 158c 0454 6865 2094 8594 8194 7d94 2868  ...The .....}.(h
+000072f0: 058c 0454 6865 2094 681a 6a81 0700 0068  ...The .h.j....h
+00007300: 0168 0368 1b4e 681c 4e75 626a 6204 0000  .h.h.Nh.Nubjb...
+00007310: 2981 947d 9428 6805 8c07 2a2a 696f 6e2a  )..}.(h...**ion*
+00007320: 2a94 6807 5d94 6815 8c03 696f 6e94 8594  *.h.].h...ion...
+00007330: 8194 7d94 2868 0568 0668 1a6a 8a07 0000  ..}.(h.h.h.j....
+00007340: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00007350: 6823 5d94 6825 5d94 6827 5d94 7568 296a  h#].h%].h'].uh)j
+00007360: 6104 0000 681a 6a81 0700 0075 6268 158c  a...h.j....ubh..
+00007370: 3720 616e 6420 6d75 6c74 692d 696f 6e20  7 and multi-ion 
+00007380: 636c 6173 7365 7320 6e6f 7720 6163 6365  classes now acce
+00007390: 7074 2074 6865 206b 6579 776f 7264 2061  pt the keyword a
+000073a0: 7267 756d 656e 7420 9485 9481 947d 9428  rgument .....}.(
+000073b0: 6805 8c37 2061 6e64 206d 756c 7469 2d69  h..7 and multi-i
+000073c0: 6f6e 2063 6c61 7373 6573 206e 6f77 2061  on classes now a
+000073d0: 6363 6570 7420 7468 6520 6b65 7977 6f72  ccept the keywor
+000073e0: 6420 6172 6775 6d65 6e74 2094 681a 6a81  d argument .h.j.
+000073f0: 0700 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
+00007400: 6204 0000 2981 947d 9428 6805 8c11 2a2a  b...)..}.(h...**
+00007410: 6162 756e 6461 6e63 654e 616d 652a 2a94  abundanceName**.
+00007420: 6807 5d94 6815 8c0d 6162 756e 6461 6e63  h.].h...abundanc
+00007430: 654e 616d 6594 8594 8194 7d94 2868 0568  eName.....}.(h.h
+00007440: 0668 1a6a 9d07 0000 7562 6168 1d7d 9428  .h.j....ubah.}.(
+00007450: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00007460: 6827 5d94 7568 296a 6104 0000 681a 6a81  h'].uh)ja...h.j.
+00007470: 0700 0075 6268 158c 6c20 7468 6174 2061  ...ubh..l that a
+00007480: 6c6c 6f77 2074 6865 2075 7365 7220 746f  llow the user to
+00007490: 2073 7065 6369 6679 2074 6865 2073 6574   specify the set
+000074a0: 206f 6620 656c 656d 656e 7461 6c20 6162   of elemental ab
+000074b0: 756e 6461 6e63 6573 2072 6174 6865 7220  undances rather 
+000074c0: 7468 616e 206a 7573 7420 7468 6520 6465  than just the de
+000074d0: 6661 756c 7420 6162 756e 6461 6e63 6520  fault abundance 
+000074e0: 6669 6c65 2e94 8594 8194 7d94 2868 058c  file......}.(h..
+000074f0: 6c20 7468 6174 2061 6c6c 6f77 2074 6865  l that allow the
+00007500: 2075 7365 7220 746f 2073 7065 6369 6679   user to specify
+00007510: 2074 6865 2073 6574 206f 6620 656c 656d   the set of elem
+00007520: 656e 7461 6c20 6162 756e 6461 6e63 6573  ental abundances
+00007530: 2072 6174 6865 7220 7468 616e 206a 7573   rather than jus
+00007540: 7420 7468 6520 6465 6661 756c 7420 6162  t the default ab
+00007550: 756e 6461 6e63 6520 6669 6c65 2e94 681a  undance file..h.
+00007560: 6a81 0700 0068 0168 0368 1b4e 681c 4e75  j....h.h.h.Nh.Nu
+00007570: 6265 681d 7d94 2868 1f5d 9468 215d 9468  beh.}.(h.].h!].h
+00007580: 235d 9468 255d 9468 275d 9475 6829 683c  #].h%].h'].uh)h<
+00007590: 681b 682a 681c 4bce 681a 6afb 0500 0068  h.h*h.K.h.j....h
+000075a0: 0168 0375 6268 3d29 8194 7d94 2868 0558  .h.ubh=)..}.(h.X
+000075b0: 0d01 0000 4164 6469 7469 6f6e 616c 2077  ....Additional w
+000075c0: 6520 6861 7665 2072 6570 6c61 6365 6420  e have replaced 
+000075d0: 7468 6520 466f 7274 7261 6e46 6f72 6d61  the FortranForma
+000075e0: 7420 6d6f 6475 6c65 206f 6620 5363 6965  t module of Scie
+000075f0: 6e74 6966 6963 2050 7974 686f 6e20 6279  ntific Python by
+00007600: 204b 6f6e 7261 6420 4869 6e73 656e 2077   Konrad Hinsen w
+00007610: 6974 6820 7468 6520 2a2a 666f 7274 7261  ith the **fortra
+00007620: 6e66 6f72 6d61 742a 2a20 6d6f 6475 6c65  nformat** module
+00007630: 206f 6620 4272 656e 6461 6e20 4172 6e6f   of Brendan Arno
+00007640: 6c64 2061 7420 6874 7470 3a2f 2f62 6974  ld at http://bit
+00007650: 6275 636b 6574 2e6f 7267 2f62 7265 6e64  bucket.org/brend
+00007660: 616e 6172 6e6f 6c64 2f70 792d 666f 7274  anarnold/py-fort
+00007670: 7261 6e66 6f72 6d61 742e 2020 4920 6861  ranformat.  I ha
+00007680: 7665 2073 6c69 6768 746c 7920 6d6f 6469  ve slightly modi
+00007690: 6669 6564 2066 6f72 7472 616e 666f 726d  fied fortranform
+000076a0: 6174 2074 6f20 6d61 6b65 2069 7420 5079  at to make it Py
+000076b0: 7468 6f6e 2033 2063 6f6d 706c 6961 6e74  thon 3 compliant
+000076c0: 2e94 6807 5d94 2868 158c 6441 6464 6974  ..h.].(h..dAddit
+000076d0: 696f 6e61 6c20 7765 2068 6176 6520 7265  ional we have re
+000076e0: 706c 6163 6564 2074 6865 2046 6f72 7472  placed the Fortr
+000076f0: 616e 466f 726d 6174 206d 6f64 756c 6520  anFormat module 
+00007700: 6f66 2053 6369 656e 7469 6669 6320 5079  of Scientific Py
+00007710: 7468 6f6e 2062 7920 4b6f 6e72 6164 2048  thon by Konrad H
+00007720: 696e 7365 6e20 7769 7468 2074 6865 2094  insen with the .
+00007730: 8594 8194 7d94 2868 058c 6441 6464 6974  ....}.(h..dAddit
+00007740: 696f 6e61 6c20 7765 2068 6176 6520 7265  ional we have re
+00007750: 706c 6163 6564 2074 6865 2046 6f72 7472  placed the Fortr
+00007760: 616e 466f 726d 6174 206d 6f64 756c 6520  anFormat module 
+00007770: 6f66 2053 6369 656e 7469 6669 6320 5079  of Scientific Py
+00007780: 7468 6f6e 2062 7920 4b6f 6e72 6164 2048  thon by Konrad H
+00007790: 696e 7365 6e20 7769 7468 2074 6865 2094  insen with the .
+000077a0: 681a 6ab6 0700 0068 0168 0368 1b4e 681c  h.j....h.h.h.Nh.
+000077b0: 4e75 626a 6204 0000 2981 947d 9428 6805  Nubjb...)..}.(h.
+000077c0: 8c11 2a2a 666f 7274 7261 6e66 6f72 6d61  ..**fortranforma
+000077d0: 742a 2a94 6807 5d94 6815 8c0d 666f 7274  t**.h.].h...fort
+000077e0: 7261 6e66 6f72 6d61 7494 8594 8194 7d94  ranformat.....}.
+000077f0: 2868 0568 0668 1a6a bf07 0000 7562 6168  (h.h.h.j....ubah
+00007800: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00007810: 6825 5d94 6827 5d94 7568 296a 6104 0000  h%].h'].uh)ja...
+00007820: 681a 6ab6 0700 0075 6268 158c 1d20 6d6f  h.j....ubh... mo
+00007830: 6475 6c65 206f 6620 4272 656e 6461 6e20  dule of Brendan 
+00007840: 4172 6e6f 6c64 2061 7420 9485 9481 947d  Arnold at .....}
+00007850: 9428 6805 8c1d 206d 6f64 756c 6520 6f66  .(h... module of
+00007860: 2042 7265 6e64 616e 2041 726e 6f6c 6420   Brendan Arnold 
+00007870: 6174 2094 681a 6ab6 0700 0068 0168 0368  at .h.j....h.h.h
+00007880: 1b4e 681c 4e75 626a 1303 0000 2981 947d  .Nh.Nubj....)..}
+00007890: 9428 6805 8c33 6874 7470 3a2f 2f62 6974  .(h..3http://bit
+000078a0: 6275 636b 6574 2e6f 7267 2f62 7265 6e64  bucket.org/brend
+000078b0: 616e 6172 6e6f 6c64 2f70 792d 666f 7274  anarnold/py-fort
+000078c0: 7261 6e66 6f72 6d61 7494 6807 5d94 6815  ranformat.h.].h.
+000078d0: 8c33 6874 7470 3a2f 2f62 6974 6275 636b  .3http://bitbuck
+000078e0: 6574 2e6f 7267 2f62 7265 6e64 616e 6172  et.org/brendanar
+000078f0: 6e6f 6c64 2f70 792d 666f 7274 7261 6e66  nold/py-fortranf
+00007900: 6f72 6d61 7494 8594 8194 7d94 2868 0568  ormat.....}.(h.h
+00007910: 0668 1a6a d207 0000 7562 6168 1d7d 9428  .h.j....ubah.}.(
+00007920: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00007930: 6827 5d94 8c06 7265 6675 7269 946a d407  h']...refuri.j..
+00007940: 0000 7568 296a 1203 0000 681a 6ab6 0700  ..uh)j....h.j...
+00007950: 0075 6268 158c 482e 2020 4920 6861 7665  .ubh..H.  I have
+00007960: 2073 6c69 6768 746c 7920 6d6f 6469 6669   slightly modifi
+00007970: 6564 2066 6f72 7472 616e 666f 726d 6174  ed fortranformat
+00007980: 2074 6f20 6d61 6b65 2069 7420 5079 7468   to make it Pyth
+00007990: 6f6e 2033 2063 6f6d 706c 6961 6e74 2e94  on 3 compliant..
+000079a0: 8594 8194 7d94 2868 058c 482e 2020 4920  ....}.(h..H.  I 
+000079b0: 6861 7665 2073 6c69 6768 746c 7920 6d6f  have slightly mo
+000079c0: 6469 6669 6564 2066 6f72 7472 616e 666f  dified fortranfo
+000079d0: 726d 6174 2074 6f20 6d61 6b65 2069 7420  rmat to make it 
+000079e0: 5079 7468 6f6e 2033 2063 6f6d 706c 6961  Python 3 complia
+000079f0: 6e74 2e94 681a 6ab6 0700 0068 0168 0368  nt..h.j....h.h.h
+00007a00: 1b4e 681c 4e75 6265 681d 7d94 2868 1f5d  .Nh.Nubeh.}.(h.]
+00007a10: 9468 215d 9468 235d 9468 255d 9468 275d  .h!].h#].h%].h']
+00007a20: 9475 6829 683c 681b 682a 681c 4bd0 681a  .uh)h<h.h*h.K.h.
+00007a30: 6afb 0500 0068 0168 0375 6268 3d29 8194  j....h.h.ubh=)..
+00007a40: 7d94 2868 058c c746 6f72 2074 6865 2066  }.(h...For the f
+00007a50: 7574 7572 652c 2049 2070 6c61 6e20 746f  uture, I plan to
+00007a60: 206d 616b 6520 4368 6961 6e74 6950 7920   make ChiantiPy 
+00007a70: 636f 6d70 6c69 616e 7420 7769 7468 2062  compliant with b
+00007a80: 6f74 6820 5079 7468 6f6e 2032 2e37 2061  oth Python 2.7 a
+00007a90: 6e64 2074 6865 2063 7572 7265 6e74 2076  nd the current v
+00007aa0: 6572 7369 6f6e 206f 6620 5079 7468 6f6e  ersion of Python
+00007ab0: 2033 2028 6e6f 7720 332e 3429 2c20 696d   3 (now 3.4), im
+00007ac0: 7072 6f76 6520 7468 6520 646f 6375 6d65  prove the docume
+00007ad0: 6e74 6174 696f 6e20 616e 6420 6d6f 7665  ntation and move
+00007ae0: 2074 6865 2070 726f 6a65 6320 746f 2067   the projec to g
+00007af0: 6974 6875 622c 2069 6e20 6e6f 2070 6172  ithub, in no par
+00007b00: 7469 6375 6c61 7220 6f72 6465 722e 9468  ticular order..h
+00007b10: 075d 9468 158c c746 6f72 2074 6865 2066  .].h...For the f
+00007b20: 7574 7572 652c 2049 2070 6c61 6e20 746f  uture, I plan to
+00007b30: 206d 616b 6520 4368 6961 6e74 6950 7920   make ChiantiPy 
+00007b40: 636f 6d70 6c69 616e 7420 7769 7468 2062  compliant with b
+00007b50: 6f74 6820 5079 7468 6f6e 2032 2e37 2061  oth Python 2.7 a
+00007b60: 6e64 2074 6865 2063 7572 7265 6e74 2076  nd the current v
+00007b70: 6572 7369 6f6e 206f 6620 5079 7468 6f6e  ersion of Python
+00007b80: 2033 2028 6e6f 7720 332e 3429 2c20 696d   3 (now 3.4), im
+00007b90: 7072 6f76 6520 7468 6520 646f 6375 6d65  prove the docume
+00007ba0: 6e74 6174 696f 6e20 616e 6420 6d6f 7665  ntation and move
+00007bb0: 2074 6865 2070 726f 6a65 6320 746f 2067   the projec to g
+00007bc0: 6974 6875 622c 2069 6e20 6e6f 2070 6172  ithub, in no par
+00007bd0: 7469 6375 6c61 7220 6f72 6465 722e 9485  ticular order...
+00007be0: 9481 947d 9428 6805 6aee 0700 0068 1a6a  ...}.(h.j....h.j
+00007bf0: ec07 0000 6801 6803 681b 4e68 1c4e 7562  ....h.h.h.Nh.Nub
+00007c00: 6168 1d7d 9428 681f 5d94 6821 5d94 6823  ah.}.(h.].h!].h#
+00007c10: 5d94 6825 5d94 6827 5d94 7568 2968 3c68  ].h%].h'].uh)h<h
+00007c20: 1b68 2a68 1c4b d268 1a6a fb05 0000 6801  .h*h.K.h.j....h.
+00007c30: 6803 7562 683d 2981 947d 9428 6805 581a  h.ubh=)..}.(h.X.
+00007c40: 0100 0043 6869 616e 7469 5079 2069 7320  ...ChiantiPy is 
+00007c50: 6e6f 7720 7265 6c65 6173 6564 2075 6e64  now released und
+00007c60: 6572 2061 206e 6577 206c 6963 656e 7365  er a new license
+00007c70: 2c20 7468 6520 4f53 4920 6170 7072 6f76  , the OSI approv
+00007c80: 6564 2049 5343 4c20 6c69 6365 6e73 652e  ed ISCL license.
+00007c90: 2020 4672 6f6d 2057 696b 6970 6564 6961    From Wikipedia
+00007ca0: 5f20 2a54 6865 2049 5343 4c20 6c69 6365  _ *The ISCL lice
+00007cb0: 6e73 6520 6973 2061 2070 6572 6d69 7373  nse is a permiss
+00007cc0: 6976 6520 6672 6565 2073 6f66 7477 6172  ive free softwar
+00007cd0: 6520 6c69 6365 6e73 6520 7772 6974 7465  e license writte
+00007ce0: 6e20 6279 2074 6865 2049 6e74 6572 6e65  n by the Interne
+00007cf0: 7420 536f 6674 7761 7265 2043 6f6e 736f  t Software Conso
+00007d00: 7274 6975 6d20 2849 5343 292e 2049 7420  rtium (ISC). It 
+00007d10: 6973 2066 756e 6374 696f 6e61 6c6c 7920  is functionally 
+00007d20: 6571 7569 7661 6c65 6e74 2074 6f20 7468  equivalent to th
+00007d30: 6520 7369 6d70 6c69 6669 6564 2042 5344  e simplified BSD
+00007d40: 2061 6e64 204d 4954 2f45 7870 6174 206c   and MIT/Expat l
+00007d50: 6963 656e 7365 732c 202e 2e2e 2a94 6807  icenses, ...*.h.
+00007d60: 5d94 2868 158c 5443 6869 616e 7469 5079  ].(h..TChiantiPy
+00007d70: 2069 7320 6e6f 7720 7265 6c65 6173 6564   is now released
+00007d80: 2075 6e64 6572 2061 206e 6577 206c 6963   under a new lic
+00007d90: 656e 7365 2c20 7468 6520 4f53 4920 6170  ense, the OSI ap
+00007da0: 7072 6f76 6564 2049 5343 4c20 6c69 6365  proved ISCL lice
+00007db0: 6e73 652e 2020 4672 6f6d 2094 8594 8194  nse.  From .....
+00007dc0: 7d94 2868 058c 5443 6869 616e 7469 5079  }.(h..TChiantiPy
+00007dd0: 2069 7320 6e6f 7720 7265 6c65 6173 6564   is now released
+00007de0: 2075 6e64 6572 2061 206e 6577 206c 6963   under a new lic
+00007df0: 656e 7365 2c20 7468 6520 4f53 4920 6170  ense, the OSI ap
+00007e00: 7072 6f76 6564 2049 5343 4c20 6c69 6365  proved ISCL lice
+00007e10: 6e73 652e 2020 4672 6f6d 2094 681a 6afa  nse.  From .h.j.
+00007e20: 0700 0068 0168 0368 1b4e 681c 4e75 626a  ...h.h.h.Nh.Nubj
+00007e30: 1303 0000 2981 947d 9428 6805 8c0a 5769  ....)..}.(h...Wi
+00007e40: 6b69 7065 6469 615f 9468 075d 9468 158c  kipedia_.h.].h..
+00007e50: 0957 696b 6970 6564 6961 9485 9481 947d  .Wikipedia.....}
+00007e60: 9428 6805 6806 681a 6a03 0800 0075 6261  .(h.h.h.j....uba
+00007e70: 681d 7d94 2868 1f5d 9468 215d 9468 235d  h.}.(h.].h!].h#]
+00007e80: 9468 255d 9468 275d 948c 046e 616d 6594  .h%].h']...name.
+00007e90: 8c09 5769 6b69 7065 6469 6194 6ac0 0300  ..Wikipedia.j...
+00007ea0: 008c 4668 7474 7073 3a2f 2f65 6e2e 7769  ..Fhttps://en.wi
+00007eb0: 6b69 7065 6469 612e 6f72 672f 772f 696e  kipedia.org/w/in
+00007ec0: 6465 782e 7068 703f 7469 746c 653d 4953  dex.php?title=IS
+00007ed0: 435f 6c69 6365 6e73 6526 6f6c 6469 643d  C_license&oldid=
+00007ee0: 3636 3436 3936 3939 3394 7568 296a 1203  664696993.uh)j..
+00007ef0: 0000 681a 6afa 0700 006a c203 0000 4b01  ..h.j....j....K.
+00007f00: 7562 6815 8c01 2094 8594 8194 7d94 2868  ubh... .....}.(h
+00007f10: 058c 0120 9468 1a6a fa07 0000 6801 6803  ... .h.j....h.h.
+00007f20: 681b 4e68 1c4e 7562 6800 8c08 656d 7068  h.Nh.Nubh...emph
+00007f30: 6173 6973 9493 9429 8194 7d94 2868 058c  asis...)..}.(h..
+00007f40: bb2a 5468 6520 4953 434c 206c 6963 656e  .*The ISCL licen
+00007f50: 7365 2069 7320 6120 7065 726d 6973 7369  se is a permissi
+00007f60: 7665 2066 7265 6520 736f 6674 7761 7265  ve free software
+00007f70: 206c 6963 656e 7365 2077 7269 7474 656e   license written
+00007f80: 2062 7920 7468 6520 496e 7465 726e 6574   by the Internet
+00007f90: 2053 6f66 7477 6172 6520 436f 6e73 6f72   Software Consor
+00007fa0: 7469 756d 2028 4953 4329 2e20 4974 2069  tium (ISC). It i
+00007fb0: 7320 6675 6e63 7469 6f6e 616c 6c79 2065  s functionally e
+00007fc0: 7175 6976 616c 656e 7420 746f 2074 6865  quivalent to the
+00007fd0: 2073 696d 706c 6966 6965 6420 4253 4420   simplified BSD 
+00007fe0: 616e 6420 4d49 542f 4578 7061 7420 6c69  and MIT/Expat li
+00007ff0: 6365 6e73 6573 2c20 2e2e 2e2a 9468 075d  censes, ...*.h.]
+00008000: 9468 158c b954 6865 2049 5343 4c20 6c69  .h...The ISCL li
+00008010: 6365 6e73 6520 6973 2061 2070 6572 6d69  cense is a permi
+00008020: 7373 6976 6520 6672 6565 2073 6f66 7477  ssive free softw
+00008030: 6172 6520 6c69 6365 6e73 6520 7772 6974  are license writ
+00008040: 7465 6e20 6279 2074 6865 2049 6e74 6572  ten by the Inter
+00008050: 6e65 7420 536f 6674 7761 7265 2043 6f6e  net Software Con
+00008060: 736f 7274 6975 6d20 2849 5343 292e 2049  sortium (ISC). I
+00008070: 7420 6973 2066 756e 6374 696f 6e61 6c6c  t is functionall
+00008080: 7920 6571 7569 7661 6c65 6e74 2074 6f20  y equivalent to 
+00008090: 7468 6520 7369 6d70 6c69 6669 6564 2042  the simplified B
+000080a0: 5344 2061 6e64 204d 4954 2f45 7870 6174  SD and MIT/Expat
+000080b0: 206c 6963 656e 7365 732c 20e2 80a6 9485   licenses, .....
+000080c0: 9481 947d 9428 6805 6806 681a 6a1b 0800  ...}.(h.h.h.j...
+000080d0: 0075 6261 681d 7d94 2868 1f5d 9468 215d  .ubah.}.(h.].h!]
+000080e0: 9468 235d 9468 255d 9468 275d 9475 6829  .h#].h%].h'].uh)
+000080f0: 6a19 0800 0068 1a6a fa07 0000 7562 6568  j....h.j....ubeh
+00008100: 1d7d 9428 681f 5d94 6821 5d94 6823 5d94  .}.(h.].h!].h#].
+00008110: 6825 5d94 6827 5d94 7568 2968 3c68 1b68  h%].h'].uh)h<h.h
+00008120: 2a68 1c4b d468 1a6a fb05 0000 6801 6803  *h.K.h.j....h.h.
+00008130: 7562 6ae0 0300 0029 8194 7d94 2868 058c  ubj....)..}.(h..
+00008140: 552e 2e20 5f57 696b 6970 6564 6961 3a20  U.. _Wikipedia: 
+00008150: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00008160: 6564 6961 2e6f 7267 2f77 2f69 6e64 6578  edia.org/w/index
+00008170: 2e70 6870 3f74 6974 6c65 3d49 5343 5f6c  .php?title=ISC_l
+00008180: 6963 656e 7365 266f 6c64 6964 3d36 3634  icense&oldid=664
+00008190: 3639 3639 3933 9468 075d 9468 1d7d 9428  696993.h.].h.}.(
+000081a0: 681f 5d94 8c09 7769 6b69 7065 6469 6194  h.]...wikipedia.
+000081b0: 6168 215d 9468 235d 948c 0977 696b 6970  ah!].h#]...wikip
+000081c0: 6564 6961 9461 6825 5d94 6827 5d94 6ac0  edia.ah%].h'].j.
+000081d0: 0300 006a 1308 0000 7568 296a df03 0000  ...j....uh)j....
+000081e0: 681c 4bd6 681a 6afb 0500 0068 0168 0368  h.K.h.j....h.h.h
+000081f0: 1b68 2a6a 6a02 0000 4b01 7562 6568 1d7d  .h*jj...K.ubeh.}
+00008200: 9428 681f 5d94 8c1b 6368 616e 6765 732d  .(h.]...changes-
+00008210: 6672 6f6d 2d30 2d35 2d33 2d74 6f2d 302d  from-0-5-3-to-0-
+00008220: 362d 3094 6168 215d 9468 235d 948c 1b63  6-0.ah!].h#]...c
+00008230: 6861 6e67 6573 2066 726f 6d20 302e 352e  hanges from 0.5.
+00008240: 3320 746f 2030 2e36 2e30 9461 6825 5d94  3 to 0.6.0.ah%].
+00008250: 6827 5d94 7568 2968 0968 1a68 0b68 0168  h'].uh)h.h.h.h.h
+00008260: 0368 1b68 2a68 1c4b c275 6265 681d 7d94  .h.h*h.K.ubeh.}.
+00008270: 2868 1f5d 948c 0963 6861 6e67 656c 6f67  (h.]...changelog
+00008280: 9461 6821 5d94 6823 5d94 8c09 6368 616e  .ah!].h#]...chan
+00008290: 6765 6c6f 6794 6168 255d 9468 275d 9475  gelog.ah%].h'].u
+000082a0: 6829 6809 681a 6803 6801 6803 681b 682a  h)h.h.h.h.h.h.h*
+000082b0: 681c 4b03 7562 6168 1d7d 9428 681f 5d94  h.K.ubah.}.(h.].
+000082c0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000082d0: 8c06 736f 7572 6365 9468 2a75 6829 6801  ..source.h*uh)h.
+000082e0: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
+000082f0: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
+00008300: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
+00008310: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
+00008320: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
+00008330: 9428 680e 4e8c 0967 656e 6572 6174 6f72  .(h.N..generator
+00008340: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
+00008350: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
+00008360: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
+00008370: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
+00008380: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
+00008390: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
+000083a0: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
+000083b0: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
+000083c0: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
+000083d0: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
+000083e0: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
+000083f0: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
+00008400: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
+00008410: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
+00008420: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
+00008430: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
+00008440: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
+00008450: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
+00008460: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
+00008470: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
+00008480: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
+00008490: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
+000084a0: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
+000084b0: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
+000084c0: 726f 725f 6861 6e64 6c65 7294 6a6e 0800  ror_handler.jn..
+000084d0: 008c 0e65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
+000084e0: 6794 8c05 5554 462d 3894 8c1c 6572 726f  g...UTF-8...erro
+000084f0: 725f 656e 636f 6469 6e67 5f65 7272 6f72  r_encoding_error
+00008500: 5f68 616e 646c 6572 948c 1062 6163 6b73  _handler...backs
+00008510: 6c61 7368 7265 706c 6163 6594 8c0d 6c61  lashreplace...la
+00008520: 6e67 7561 6765 5f63 6f64 6594 8c02 656e  nguage_code...en
+00008530: 948c 1372 6563 6f72 645f 6465 7065 6e64  ...record_depend
+00008540: 656e 6369 6573 944e 8c06 636f 6e66 6967  encies.N..config
+00008550: 944e 8c09 6964 5f70 7265 6669 7894 6806  .N..id_prefix.h.
+00008560: 8c0e 6175 746f 5f69 645f 7072 6566 6978  ..auto_id_prefix
+00008570: 948c 0269 6494 8c0d 6475 6d70 5f73 6574  ...id...dump_set
+00008580: 7469 6e67 7394 4e8c 0e64 756d 705f 696e  tings.N..dump_in
+00008590: 7465 726e 616c 7394 4e8c 0f64 756d 705f  ternals.N..dump_
+000085a0: 7472 616e 7366 6f72 6d73 944e 8c0f 6475  transforms.N..du
+000085b0: 6d70 5f70 7365 7564 6f5f 786d 6c94 4e8c  mp_pseudo_xml.N.
+000085c0: 1065 7870 6f73 655f 696e 7465 726e 616c  .expose_internal
+000085d0: 7394 4e8c 0e73 7472 6963 745f 7669 7369  s.N..strict_visi
+000085e0: 746f 7294 4e8c 0f5f 6469 7361 626c 655f  tor.N.._disable_
+000085f0: 636f 6e66 6967 944e 8c07 5f73 6f75 7263  config.N.._sourc
+00008600: 6594 682a 8c0c 5f64 6573 7469 6e61 7469  e.h*.._destinati
+00008610: 6f6e 944e 8c0d 5f63 6f6e 6669 675f 6669  on.N.._config_fi
+00008620: 6c65 7394 5d94 8c0e 7065 705f 7265 6665  les.]...pep_refe
+00008630: 7265 6e63 6573 944e 8c0c 7065 705f 6261  rences.N..pep_ba
+00008640: 7365 5f75 726c 948c 2068 7474 7073 3a2f  se_url.. https:/
+00008650: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
+00008660: 6465 762f 7065 7073 2f94 8c15 7065 705f  dev/peps/...pep_
+00008670: 6669 6c65 5f75 726c 5f74 656d 706c 6174  file_url_templat
+00008680: 6594 8c08 7065 702d 2530 3464 948c 0e72  e...pep-%04d...r
+00008690: 6663 5f72 6566 6572 656e 6365 7394 4e8c  fc_references.N.
+000086a0: 0c72 6663 5f62 6173 655f 7572 6c94 8c1c  .rfc_base_url...
+000086b0: 6874 7470 733a 2f2f 746f 6f6c 732e 6965  https://tools.ie
+000086c0: 7466 2e6f 7267 2f68 746d 6c2f 948c 0974  tf.org/html/...t
+000086d0: 6162 5f77 6964 7468 944b 088c 1d74 7269  ab_width.K...tri
+000086e0: 6d5f 666f 6f74 6e6f 7465 5f72 6566 6572  m_footnote_refer
+000086f0: 656e 6365 5f73 7061 6365 9489 8c16 6669  ence_space....fi
+00008700: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+00008710: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+00008720: 6c65 6494 4b01 8c10 7379 6e74 6178 5f68  led.K...syntax_h
+00008730: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
+00008740: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
+00008750: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
+00008760: 6361 6c65 7394 4e8c 1d63 6861 7261 6374  cales.N..charact
+00008770: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+00008780: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+00008790: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+000087a0: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+000087b0: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+000087c0: 9489 8c10 656d 6265 645f 7374 796c 6573  ....embed_styles
+000087d0: 6865 6574 9489 8c15 636c 6f61 6b5f 656d  heet....cloak_em
+000087e0: 6169 6c5f 6164 6472 6573 7365 7394 888c  ail_addresses...
+000087f0: 0365 6e76 944e 8c0f 6765 7474 6578 745f  .env.N..gettext_
+00008800: 636f 6d70 6163 7494 8875 628c 0872 6570  compact..ub..rep
+00008810: 6f72 7465 7294 4e8c 1069 6e64 6972 6563  orter.N..indirec
+00008820: 745f 7461 7267 6574 7394 5d94 8c11 7375  t_targets.]...su
+00008830: 6273 7469 7475 7469 6f6e 5f64 6566 7394  bstitution_defs.
+00008840: 7d94 8c12 7375 6273 7469 7475 7469 6f6e  }...substitution
+00008850: 5f6e 616d 6573 947d 948c 0872 6566 6e61  _names.}...refna
+00008860: 6d65 7394 7d94 288c 0967 6974 6875 622e  mes.}.(..github.
+00008870: 696f 945d 946a b003 0000 618c 0b72 6561  io.].j....a..rea
+00008880: 6474 6865 646f 6373 945d 946a c803 0000  dthedocs.].j....
+00008890: 618c 0667 6974 6875 6294 5d94 6ae1 0400  a..github.].j...
+000088a0: 0061 8c07 6173 7472 6f70 7994 5d94 6a12  .a..astropy.].j.
+000088b0: 0500 0061 8c05 7375 6e70 7994 5d94 6a28  ...a..sunpy.].j(
+000088c0: 0500 0061 8c09 7769 6b69 7065 6469 6194  ...a..wikipedia.
+000088d0: 5d94 6a03 0800 0061 758c 0672 6566 6964  ].j....au..refid
+000088e0: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
+000088f0: 286a 4808 0000 6a45 0800 0068 5f68 5c68  (jH...jE...h_h\h
+00008900: 9468 9168 c968 c668 fe68 fb6a 3301 0000  .h.h.h.h.h.j3...
+00008910: 6a30 0100 006a 7601 0000 6a73 0100 006a  j0...jv...js...j
+00008920: bd01 0000 6aba 0100 006a e401 0000 6ae1  ....j....j....j.
+00008930: 0100 006a 1902 0000 6a16 0200 006a 3202  ...j....j....j2.
+00008940: 0000 6a2f 0200 008c 2074 6869 7320 6973  ..j/.... this is
+00008950: 2061 206d 616a 6f72 2062 7567 2d66 6978   a major bug-fix
+00008960: 2072 656c 6561 7365 2e94 4e6a 8102 0000   release..Nj....
+00008970: 6a7e 0200 006a c002 0000 6abd 0200 006a  j~...j....j....j
+00008980: 7703 0000 6a74 0300 006a fe03 0000 6afb  w...jt...j....j.
+00008990: 0300 006a ea03 0000 6ae7 0300 006a f603  ...j....j....j..
+000089a0: 0000 6af3 0300 006a c404 0000 6ac1 0400  ..j....j....j...
+000089b0: 006a a705 0000 6aa4 0500 006a 0605 0000  .j....j....j....
+000089c0: 6a03 0500 006a 4d05 0000 6a4a 0500 006a  j....jM...jJ...j
+000089d0: 5905 0000 6a56 0500 006a f805 0000 6af5  Y...jV...j....j.
+000089e0: 0500 006a 4008 0000 6a3d 0800 006a 3808  ...j@...j=...j8.
+000089f0: 0000 6a35 0800 0075 8c09 6e61 6d65 7479  ..j5...u..namety
+00008a00: 7065 7394 7d94 286a 4808 0000 4e68 5f4e  pes.}.(jH...Nh_N
+00008a10: 6894 4e68 c94e 68fe 4e6a 3301 0000 4e6a  h.Nh.Nh.Nj3...Nj
+00008a20: 7601 0000 4e6a bd01 0000 4e6a e401 0000  v...Nj....Nj....
+00008a30: 4e6a 1902 0000 4e6a 3202 0000 4e6a b908  Nj....Nj2...Nj..
+00008a40: 0000 4e6a 8102 0000 4e6a c002 0000 4e6a  ..Nj....Nj....Nj
+00008a50: 7703 0000 4e6a fe03 0000 4e6a ea03 0000  w...Nj....Nj....
+00008a60: 886a f603 0000 886a c404 0000 4e6a a705  .j.....j....Nj..
+00008a70: 0000 4e6a 0605 0000 886a 4d05 0000 886a  ..Nj.....jM....j
+00008a80: 5905 0000 886a f805 0000 4e6a 4008 0000  Y....j....Nj@...
+00008a90: 4e6a 3808 0000 8875 681f 7d94 286a 4508  Nj8....uh.}.(jE.
+00008aa0: 0000 680b 685c 682b 6891 6862 68c6 6897  ..h.h\h+h.hbh.h.
+00008ab0: 68fb 68cc 6a30 0100 006a 0101 0000 6a73  h.h.j0...j....js
+00008ac0: 0100 006a 3601 0000 6aba 0100 006a 7901  ...j6...j....jy.
+00008ad0: 0000 6ae1 0100 006a c001 0000 6a16 0200  ..j....j....j...
+00008ae0: 006a e701 0000 6a2f 0200 006a 1c02 0000  .j....j/...j....
+00008af0: 6a64 0200 006a 3502 0000 6a7e 0200 006a  jd...j5...j~...j
+00008b00: 6b02 0000 6aa5 0200 006a 8402 0000 6abd  k...j....j....j.
+00008b10: 0200 006a aa02 0000 6ae4 0200 006a c302  ...j....j....j..
+00008b20: 0000 6a74 0300 006a ea02 0000 6afb 0300  ..jt...j....j...
+00008b30: 006a 7a03 0000 6ae7 0300 006a e103 0000  .jz...j....j....
+00008b40: 6af3 0300 006a ed03 0000 6ac1 0400 006a  j....j....j....j
+00008b50: 0104 0000 6aa4 0500 006a c704 0000 6a03  ....j....j....j.
+00008b60: 0500 006a fd04 0000 6a4a 0500 006a 4405  ...j....jJ...jD.
+00008b70: 0000 6a56 0500 006a 5005 0000 6af5 0500  ..jV...jP...j...
+00008b80: 006a aa05 0000 6a3d 0800 006a fb05 0000  .j....j=...j....
+00008b90: 6a35 0800 006a 2f08 0000 758c 0d66 6f6f  j5...j/...u..foo
+00008ba0: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+00008bb0: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+00008bc0: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+00008bd0: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00008be0: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+00008bf0: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+00008c00: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+00008c10: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+00008c20: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+00008c30: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00008c40: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+00008c50: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+00008c60: 4b00 8c08 6964 5f73 7461 7274 944b 038c  K...id_start.K..
+00008c70: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
+00008c80: 5d94 2868 008c 0e73 7973 7465 6d5f 6d65  ].(h...system_me
+00008c90: 7373 6167 6594 9394 2981 947d 9428 6805  ssage...)..}.(h.
+00008ca0: 6806 6807 5d94 683d 2981 947d 9428 6805  h.h.].h=)..}.(h.
+00008cb0: 8c43 4475 706c 6963 6174 6520 696d 706c  .CDuplicate impl
+00008cc0: 6963 6974 2074 6172 6765 7420 6e61 6d65  icit target name
+00008cd0: 3a20 2274 6869 7320 6973 2061 206d 616a  : "this is a maj
+00008ce0: 6f72 2062 7567 2d66 6978 2072 656c 6561  or bug-fix relea
+00008cf0: 7365 2e22 2e94 6807 5d94 6815 8c47 4475  se."..h.].h..GDu
+00008d00: 706c 6963 6174 6520 696d 706c 6963 6974  plicate implicit
+00008d10: 2074 6172 6765 7420 6e61 6d65 3a20 e280   target name: ..
+00008d20: 9c74 6869 7320 6973 2061 206d 616a 6f72  .this is a major
+00008d30: 2062 7567 2d66 6978 2072 656c 6561 7365   bug-fix release
+00008d40: 2ee2 809d 2e94 8594 8194 7d94 2868 0568  ..........}.(h.h
+00008d50: 0668 1a6a d708 0000 7562 6168 1d7d 9428  .h.j....ubah.}.(
+00008d60: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00008d70: 6827 5d94 7568 2968 3c68 1a6a d408 0000  h'].uh)h<h.j....
+00008d80: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00008d90: 6823 5d94 6825 5d94 6827 5d94 6aa5 0200  h#].h%].h'].j...
+00008da0: 0061 8c05 6c65 7665 6c94 4b01 8c04 7479  .a..level.K...ty
+00008db0: 7065 948c 0449 4e46 4f94 8c06 736f 7572  pe...INFO...sour
+00008dc0: 6365 9468 2a8c 046c 696e 6594 4b62 7568  ce.h*..line.Kbuh
+00008dd0: 296a d208 0000 681a 6a84 0200 0068 0168  )j....h.j....h.h
+00008de0: 0368 1b68 2a68 1c4b 6275 626a d308 0000  .h.h*h.Kbubj....
+00008df0: 2981 947d 9428 6805 6806 6807 5d94 683d  )..}.(h.h.h.].h=
+00008e00: 2981 947d 9428 6805 8c43 4475 706c 6963  )..}.(h..CDuplic
+00008e10: 6174 6520 696d 706c 6963 6974 2074 6172  ate implicit tar
+00008e20: 6765 7420 6e61 6d65 3a20 2274 6869 7320  get name: "this 
+00008e30: 6973 2061 206d 616a 6f72 2062 7567 2d66  is a major bug-f
+00008e40: 6978 2072 656c 6561 7365 2e22 2e94 6807  ix release."..h.
+00008e50: 5d94 6815 8c47 4475 706c 6963 6174 6520  ].h..GDuplicate 
+00008e60: 696d 706c 6963 6974 2074 6172 6765 7420  implicit target 
+00008e70: 6e61 6d65 3a20 e280 9c74 6869 7320 6973  name: ...this is
+00008e80: 2061 206d 616a 6f72 2062 7567 2d66 6978   a major bug-fix
+00008e90: 2072 656c 6561 7365 2ee2 809d 2e94 8594   release........
+00008ea0: 8194 7d94 2868 0568 0668 1a6a f308 0000  ..}.(h.h.h.j....
+00008eb0: 7562 6168 1d7d 9428 681f 5d94 6821 5d94  ubah.}.(h.].h!].
+00008ec0: 6823 5d94 6825 5d94 6827 5d94 7568 2968  h#].h%].h'].uh)h
+00008ed0: 3c68 1a6a f008 0000 7562 6168 1d7d 9428  <h.j....ubah.}.(
+00008ee0: 681f 5d94 6821 5d94 6823 5d94 6825 5d94  h.].h!].h#].h%].
+00008ef0: 6827 5d94 6ae4 0200 0061 8c05 6c65 7665  h'].j....a..leve
+00008f00: 6c94 4b01 8c04 7479 7065 946a ed08 0000  l.K...type.j....
+00008f10: 8c06 736f 7572 6365 9468 2a8c 046c 696e  ..source.h*..lin
+00008f20: 6594 4b6b 7568 296a d208 0000 681a 6ac3  e.Kkuh)j....h.j.
+00008f30: 0200 0068 0168 0368 1b68 2a68 1c4b 6b75  ...h.h.h.h*h.Kku
+00008f40: 6265 8c12 7472 616e 7366 6f72 6d5f 6d65  be..transform_me
+00008f50: 7373 6167 6573 945d 948c 0b74 7261 6e73  ssages.]...trans
+00008f60: 666f 726d 6572 944e 8c0a 6465 636f 7261  former.N..decora
+00008f70: 7469 6f6e 944e 6801 6803 7562 2e         tion.Nh.h.ub.
```

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/environment.pickle` & `ChiantiPy-0.9.5/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/getting_started.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/getting_started.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/index.doctree` & `ChiantiPy-0.9.5/docs/build/.doctrees/index.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -120,37 +120,37 @@
 00000770: 9468 1568 3f68 0168 0368 254e 6827 4e75  .h.h?h.h.h%Nh'Nu
 00000780: 6265 6816 7d94 2868 185d 9468 1a5d 9468  beh.}.(h.].h.].h
 00000790: 1c5d 9468 1e5d 9468 205d 9475 6824 683d  .].h.].h ].uh$h=
 000007a0: 6825 6826 6827 4b09 6815 682a 6801 6803  h%h&h'K.h.h*h.h.
 000007b0: 7562 683e 2981 947d 9428 6805 8c89 5468  ubh>)..}.(h...Th
 000007c0: 6520 6c61 7465 7374 2076 6572 7369 6f6e  e latest version
 000007d0: 206f 6620 4368 6961 6e74 6950 7920 6973   of ChiantiPy is
-000007e0: 2030 2e39 2e30 2061 6e64 2069 7320 636f   0.9.0 and is co
+000007e0: 2030 2e39 2e35 2061 6e64 2069 7320 636f   0.9.5 and is co
 000007f0: 6d70 6174 6962 6c65 2077 6974 6820 4348  mpatible with CH
 00000800: 4941 4e54 4920 6461 7461 6261 7365 2076  IANTI database v
 00000810: 6572 7369 6f6e 2039 2e30 2e20 4974 2069  ersion 9.0. It i
 00000820: 7320 6e6f 7420 636f 6d70 6174 6962 6c65  s not compatible
 00000830: 2077 6974 6820 7072 6576 696f 7573 2076   with previous v
 00000840: 6572 7369 6f6e 7394 6807 5d94 6810 8c89  ersions.h.].h...
 00000850: 5468 6520 6c61 7465 7374 2076 6572 7369  The latest versi
 00000860: 6f6e 206f 6620 4368 6961 6e74 6950 7920  on of ChiantiPy 
-00000870: 6973 2030 2e39 2e30 2061 6e64 2069 7320  is 0.9.0 and is 
+00000870: 6973 2030 2e39 2e35 2061 6e64 2069 7320  is 0.9.5 and is 
 00000880: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
 00000890: 4348 4941 4e54 4920 6461 7461 6261 7365  CHIANTI database
 000008a0: 2076 6572 7369 6f6e 2039 2e30 2e20 4974   version 9.0. It
 000008b0: 2069 7320 6e6f 7420 636f 6d70 6174 6962   is not compatib
 000008c0: 6c65 2077 6974 6820 7072 6576 696f 7573  le with previous
 000008d0: 2076 6572 7369 6f6e 7394 8594 8194 7d94   versions.....}.
 000008e0: 2868 0568 7968 1568 7768 0168 0368 254e  (h.hyh.hwh.h.h%N
 000008f0: 6827 4e75 6261 6816 7d94 2868 185d 9468  h'Nubah.}.(h.].h
 00000900: 1a5d 9468 1c5d 9468 1e5d 9468 205d 9475  .].h.].h.].h ].u
 00000910: 6824 683d 6825 6826 6827 4b0b 6815 682a  h$h=h%h&h'K.h.h*
 00000920: 6801 6803 7562 683e 2981 947d 9428 6805  h.h.ubh>)..}.(h.
 00000930: 5855 0100 0043 6869 616e 7469 5079 2076  XU...ChiantiPy v
-00000940: 302e 392e 3020 6973 2072 656c 6561 7365  0.9.0 is release
+00000940: 302e 392e 3520 6973 2072 656c 6561 7365  0.9.5 is release
 00000950: 6420 756e 6465 7220 7468 6520 4f53 4920  d under the OSI 
 00000960: 6170 7072 6f76 6564 2049 5343 206c 6963  approved ISC lic
 00000970: 656e 7365 2e20 4672 6f6d 2060 5769 6b69  ense. From `Wiki
 00000980: 7065 6469 6120 3c68 7474 7073 3a2f 2f65  pedia <https://e
 00000990: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
 000009a0: 772f 696e 6465 782e 7068 703f 7469 746c  w/index.php?titl
 000009b0: 653d 4953 435f 6c69 6365 6e73 6526 6f6c  e=ISC_license&ol
@@ -164,20 +164,20 @@
 00000a30: 6975 6d20 2849 5343 292e 2049 7420 6973  ium (ISC). It is
 00000a40: 2066 756e 6374 696f 6e61 6c6c 7920 6571   functionally eq
 00000a50: 7569 7661 6c65 6e74 2074 6f20 7468 6520  uivalent to the 
 00000a60: 7369 6d70 6c69 6669 6564 2042 5344 2061  simplified BSD a
 00000a70: 6e64 204d 4954 2f45 7870 6174 206c 6963  nd MIT/Expat lic
 00000a80: 656e 7365 732c 202e 2e2e 9468 075d 9428  enses, ....h.].(
 00000a90: 6810 8c46 4368 6961 6e74 6950 7920 7630  h..FChiantiPy v0
-00000aa0: 2e39 2e30 2069 7320 7265 6c65 6173 6564  .9.0 is released
+00000aa0: 2e39 2e35 2069 7320 7265 6c65 6173 6564  .9.5 is released
 00000ab0: 2075 6e64 6572 2074 6865 204f 5349 2061   under the OSI a
 00000ac0: 7070 726f 7665 6420 4953 4320 6c69 6365  pproved ISC lice
 00000ad0: 6e73 652e 2046 726f 6d20 9485 9481 947d  nse. From .....}
 00000ae0: 9428 6805 8c46 4368 6961 6e74 6950 7920  .(h..FChiantiPy 
-00000af0: 7630 2e39 2e30 2069 7320 7265 6c65 6173  v0.9.0 is releas
+00000af0: 7630 2e39 2e35 2069 7320 7265 6c65 6173  v0.9.5 is releas
 00000b00: 6564 2075 6e64 6572 2074 6865 204f 5349  ed under the OSI
 00000b10: 2061 7070 726f 7665 6420 4953 4320 6c69   approved ISC li
 00000b20: 6365 6e73 652e 2046 726f 6d20 9468 1568  cense. From .h.h
 00000b30: 8568 0168 0368 254e 6827 4e75 6268 4929  .h.h.h%Nh'NubhI)
 00000b40: 8194 7d94 2868 058c 5560 5769 6b69 7065  ..}.(h..U`Wikipe
 00000b50: 6469 6120 3c68 7474 7073 3a2f 2f65 6e2e  dia <https://en.
 00000b60: 7769 6b69 7065 6469 612e 6f72 672f 772f  wikipedia.org/w/
```

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/notes.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/notes.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/quick_start.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/quick_start.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/resources.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/resources.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/doctrees/tutorial.doctree` & `ChiantiPy-0.9.5/docs/build/doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/genindex.html` & `ChiantiPy-0.9.5/docs/build/genindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Index &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Index &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -30,15 +30,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
 <div id="searchbox" style="display: none" role="search">
   <h3>Quick search</h3>
     <div class="searchformwrapper">
@@ -96,15 +96,19 @@
       <ul>
         <li><a href="api/ChiantiPy.Gui.gui_qt5.html#ChiantiPy.Gui.gui_qt5.gui.selectorDialog.accept">(ChiantiPy.Gui.gui_qt5.gui.selectorDialog method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.base.html#ChiantiPy.base._IonTrails.ionTrails.argCheck">argCheck() (ChiantiPy.base._IonTrails.ionTrails method)</a>
+
+      <ul>
+        <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.argCheck">(ChiantiPy.model.Maker.maker method)</a>
 </li>
+      </ul></li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.autoRead">autoRead() (in module ChiantiPy.tools.io)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.autoWrite">autoWrite() (in module ChiantiPy.tools.io)</a>
 </li>
   </ul></td>
 </tr></table>
 
@@ -177,24 +181,28 @@
 </li>
       <li><a href="api/ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordWriter">ChiantiPy.fortranformat.FortranRecordWriter (module)</a>
 </li>
       <li><a href="api/ChiantiPy.Gui.html#module-ChiantiPy.Gui">ChiantiPy.Gui (module)</a>
 </li>
       <li><a href="api/ChiantiPy.Gui.gui_cl.html#module-ChiantiPy.Gui.gui_cl">ChiantiPy.Gui.gui_cl (module)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.Gui.gui_cl.html#module-ChiantiPy.Gui.gui_cl.gui">ChiantiPy.Gui.gui_cl.gui (module)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.Gui.gui_qt5.html#module-ChiantiPy.Gui.gui_qt5">ChiantiPy.Gui.gui_qt5 (module)</a>
 </li>
       <li><a href="api/ChiantiPy.Gui.gui_qt5.html#module-ChiantiPy.Gui.gui_qt5.gui">ChiantiPy.Gui.gui_qt5.gui (module)</a>
 </li>
       <li><a href="api/ChiantiPy.Gui.gui_qt5.html#module-ChiantiPy.Gui.gui_qt5.ui">ChiantiPy.Gui.gui_qt5.ui (module)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#module-ChiantiPy.model">ChiantiPy.model (module)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#module-ChiantiPy.model.Maker">ChiantiPy.model.Maker (module)</a>
+</li>
       <li><a href="api/ChiantiPy.tests.html#module-ChiantiPy.tests">ChiantiPy.tests (module)</a>
 </li>
       <li><a href="api/ChiantiPy.tests.html#module-ChiantiPy.tests.setup_package">ChiantiPy.tests.setup_package (module)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#module-ChiantiPy.tools">ChiantiPy.tools (module)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#module-ChiantiPy.tools.archival">ChiantiPy.tools.archival (module)</a>
@@ -247,24 +255,30 @@
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.descale_bt">descale_bt() (in module ChiantiPy.tools.util)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.descale_bti">descale_bti() (in module ChiantiPy.tools.util)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.diCross">diCross() (ChiantiPy.core.Ion.ion method)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.diffPrintChi">diffPrintChi() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.diffPrintMc">diffPrintMc() (ChiantiPy.model.Maker.maker method)</a>
+</li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.dilute">dilute() (in module ChiantiPy.tools.util)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.diRate">diRate() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.diRead">diRead() (in module ChiantiPy.tools.io)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.IpyMspectrum.doAll">doAll() (in module ChiantiPy.core.IpyMspectrum)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.doDemGofntQ">doDemGofntQ() (in module ChiantiPy.model.Maker)</a>
+</li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.mputil.doFbQ">doFbQ() (in module ChiantiPy.tools.mputil)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.mputil.doFfQ">doFfQ() (in module ChiantiPy.tools.mputil)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.mputil.doIonQ">doIonQ() (in module ChiantiPy.tools.mputil)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.drPopulate">drPopulate() (ChiantiPy.core.Ion.ion method)</a>
@@ -293,52 +307,72 @@
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.archival.elvlcRead">elvlcRead() (in module ChiantiPy.tools.archival)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.elvlcRead">(in module ChiantiPy.tools.io)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.archival.elvlcWrite">elvlcWrite() (in module ChiantiPy.tools.archival)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.elvlcWrite">(in module ChiantiPy.tools.io)</a>
 </li>
       </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.emFitPlot">emFitPlot() (ChiantiPy.model.Maker.maker method)</a>
+</li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.emiss">emiss() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.emissList">emissList() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.emissPlot">emissPlot() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.emissRatio">emissRatio() (ChiantiPy.core.Ion.ion method)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.emNtSetIndices">emNtSetIndices() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.emPlot">emPlot() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.emSet">emSet() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.emSetIndices">emSetIndices() (ChiantiPy.model.Maker.maker method)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="F">F</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.fblvlRead">fblvlRead() (in module ChiantiPy.tools.io)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.findMinMaxIndices">findMinMaxIndices() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.fit1t">fit1t() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.fitFunc1t">fitFunc1t() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.fitFuncNt">fitFuncNt() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.fitNt">fitNt() (ChiantiPy.model.Maker.maker method)</a>
+</li>
       <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader.format">format (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader attribute)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter.format">(ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter attribute)</a>
 </li>
       </ul></li>
       <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader">FortranRecordReader (class in ChiantiPy.fortranformat.FortranRecordReader)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter">FortranRecordWriter (class in ChiantiPy.fortranformat.FortranRecordWriter)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.free_free_loss">free_free_loss() (ChiantiPy.core.Continuum.continuum method)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.freeBound">freeBound() (ChiantiPy.core.Continuum.continuum method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.freeBoundEmiss">freeBoundEmiss() (ChiantiPy.core.Continuum.continuum method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.freeBoundLoss">freeBoundLoss() (ChiantiPy.core.Continuum.continuum method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.freeBoundLossMewe">freeBoundLossMewe() (ChiantiPy.core.Continuum.continuum method)</a>
@@ -361,24 +395,34 @@
 </li>
       <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader.get_format">get_format() (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader method)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter.get_format">(ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter method)</a>
 </li>
       </ul></li>
+      <li><a href="api/ChiantiPy.tests.html#ChiantiPy.tests.setup_package.get_package_data">get_package_data() (in module ChiantiPy.tests.setup_package)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.getChisq">getChisq() (ChiantiPy.model.Maker.maker method)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="api/ChiantiPy.tests.html#ChiantiPy.tests.setup_package.get_package_data">get_package_data() (in module ChiantiPy.tests.setup_package)</a>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.getNormalizedChisq">getNormalizedChisq() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.getWeightedDiff">getWeightedDiff() (ChiantiPy.model.Maker.maker method)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.gffintRead">gffintRead() (in module ChiantiPy.tools.io)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.gffRead">gffRead() (in module ChiantiPy.tools.io)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.gofnt">gofnt() (ChiantiPy.core.Ion.ion method)</a>
+
+      <ul>
+        <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.gofnt">(ChiantiPy.model.Maker.maker method)</a>
 </li>
+      </ul></li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.grndLevelsRead">grndLevelsRead() (in module ChiantiPy.tools.io)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -463,24 +507,30 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="M">M</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.makeMatchPkl">makeMatchPkl() (in module ChiantiPy.model.Maker)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker">maker (class in ChiantiPy.model.Maker)</a>
+</li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.masterListInfo">masterListInfo() (in module ChiantiPy.tools.io)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.masterListRead">masterListRead() (in module ChiantiPy.tools.io)</a>
 </li>
-      <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader.match">match() (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader method)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader.match">match() (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader method)</a>
+</li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Continuum.continuum.mewe_gaunt_factor">mewe_gaunt_factor() (ChiantiPy.core.Continuum.continuum method)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.mgofnt">mgofnt() (ChiantiPy.model.Maker.maker method)</a>
+</li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.filters.moffat">moffat() (in module ChiantiPy.tools.filters)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Mspectrum.mspectrum">mspectrum (class in ChiantiPy.core.Mspectrum)</a>
 </li>
   </ul></td>
 </tr></table>
 
@@ -497,22 +547,28 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.p2eRatio">p2eRatio() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.photoxRead">photoxRead() (in module ChiantiPy.tools.io)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ioneq.ioneq.plot">plot() (ChiantiPy.core.Ioneq.ioneq method)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ioneq.ioneq.plotRatio">plotRatio() (ChiantiPy.core.Ioneq.ioneq method)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.popPlot">popPlot() (ChiantiPy.core.Ion.ion method)</a>
 </li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.populate">populate() (ChiantiPy.core.Ion.ion method)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.predict">predict() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.predictPrint">predictPrint() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.predictPrint1d">predictPrint1d() (ChiantiPy.model.Maker.maker method)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="Q">Q</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.qrp">qrp() (in module ChiantiPy.tools.util)</a>
@@ -567,32 +623,36 @@
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.scale_bti">scale_bti() (in module ChiantiPy.tools.util)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.util.scale_classical">scale_classical() (in module ChiantiPy.tools.util)</a>
 </li>
       <li><a href="api/ChiantiPy.tools.html#ChiantiPy.tools.io.scupsRead">scupsRead() (in module ChiantiPy.tools.io)</a>
 </li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.search1dSpace">search1dSpace() (ChiantiPy.model.Maker.maker method)</a>
+</li>
+      <li><a href="api/ChiantiPy.model.html#ChiantiPy.model.Maker.maker.search1tEmSpace">search1tEmSpace() (ChiantiPy.model.Maker.maker method)</a>
+</li>
       <li><a href="api/ChiantiPy.Gui.gui_cl.html#ChiantiPy.Gui.gui_cl.gui.selectorDialog">selectorDialog (class in ChiantiPy.Gui.gui_cl.gui)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.Gui.gui_qt5.html#ChiantiPy.Gui.gui_qt5.gui.selectorDialog">(class in ChiantiPy.Gui.gui_qt5.gui)</a>
 </li>
       </ul></li>
       <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader.set_format">set_format() (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader method)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.fortranformat.html#ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter.set_format">(ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter method)</a>
 </li>
       </ul></li>
       <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.setup">setup() (ChiantiPy.core.Ion.ion method)</a>
 </li>
-      <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.setupIonrec">setupIonrec() (ChiantiPy.core.Ion.ion method)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api/ChiantiPy.core.html#ChiantiPy.core.Ion.ion.setupIonrec">setupIonrec() (ChiantiPy.core.Ion.ion method)</a>
+</li>
       <li><a href="api/ChiantiPy.Gui.gui_qt5.html#ChiantiPy.Gui.gui_qt5.ui.Ui_choice2DialogForm.setupUi">setupUi() (ChiantiPy.Gui.gui_qt5.ui.Ui_choice2DialogForm method)</a>
 
       <ul>
         <li><a href="api/ChiantiPy.Gui.gui_qt5.html#ChiantiPy.Gui.gui_qt5.ui.Ui_selectorDialogForm.setupUi">(ChiantiPy.Gui.gui_qt5.ui.Ui_selectorDialogForm method)</a>
 </li>
       </ul></li>
       <li><a href="api/ChiantiPy.base.html#ChiantiPy.base._SpecTrails.specTrails">specTrails (class in ChiantiPy.base._SpecTrails)</a>
@@ -756,22 +816,22 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,134 +3,152 @@
 
 
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 **** Quick search ****
 [q                   ] [Go]
 ****** Index ******
 A | B | C | D | E | F | G | I | K | L | M | O | P | Q | R | S | T | U | V | W |
 Z
 ***** A *****
-    * abundanceRead()_(in_module_ChiantiPy.tools.io)      * argCheck()_
-    * accept()_                                             (ChiantiPy.base._IonTrails.ionTrails
-      (ChiantiPy.Gui.gui_qt5.gui.choice2Dialog              method)
-      method)                                             * autoRead()_(in_module
-          o (ChiantiPy.Gui.gui_qt5.gui.selectorDialog       ChiantiPy.tools.io)
-            method)                                       * autoWrite()_(in_module
+                                                          * argCheck()_
+    * abundanceRead()_(in_module_ChiantiPy.tools.io)        (ChiantiPy.base._IonTrails.ionTrails
+    * accept()_                                             method)
+      (ChiantiPy.Gui.gui_qt5.gui.choice2Dialog                  o (ChiantiPy.model.Maker.maker
+      method)                                                     method)
+          o (ChiantiPy.Gui.gui_qt5.gui.selectorDialog     * autoRead()_(in_module
+            method)                                         ChiantiPy.tools.io)
+                                                          * autoWrite()_(in_module
                                                             ChiantiPy.tools.io)
 ***** B *****
     * between()_(in_module         * boundBoundLoss()_(ChiantiPy.core.Ion.ion
       ChiantiPy.tools.util)          method)
     * blackbody()_(in_module       * boxcar()_(in_module
       ChiantiPy.tools.sources)       ChiantiPy.tools.filters)
     * blackStar_(class_in          * bunch_(class_in_ChiantiPy.core.Spectrum)
       ChiantiPy.tools.sources)
 ***** C *****
-                                                      * ChiantiPy.Gui.gui_cl.gui_(module)
                                                       * ChiantiPy.Gui.gui_qt5_(module)
-    * calculate()_(ChiantiPy.core.Ioneq.ioneq         * ChiantiPy.Gui.gui_qt5.gui_(module)
-      method)                                         * ChiantiPy.Gui.gui_qt5.ui_(module)
-    * calculate_free_bound_loss()_                    * ChiantiPy.tests_(module)
-      (ChiantiPy.core.Continuum.continuum_method)     * ChiantiPy.tests.setup_package_(module)
-    * ChiantiPy_(module)                              * ChiantiPy.tools_(module)
-    * ChiantiPy.base_(module)                         * ChiantiPy.tools.archival_(module)
-    * ChiantiPy.base._IonTrails_(module)              * ChiantiPy.tools.constants_(module)
-    * ChiantiPy.base._SpecTrails_(module)             * ChiantiPy.tools.data_(module)
-    * ChiantiPy.core_(module)                         * ChiantiPy.tools.filters_(module)
-    * ChiantiPy.core.Continuum_(module)               * ChiantiPy.tools.io_(module)
-    * ChiantiPy.core.Ion_(module)                     * ChiantiPy.tools.mputil_(module)
-    * ChiantiPy.core.Ioneq_(module)                   * ChiantiPy.tools.sources_(module)
-    * ChiantiPy.core.IpyMspectrum_(module)            * ChiantiPy.tools.util_(module)
-    * ChiantiPy.core.Mspectrum_(module)               * ChiantiPy.version_(module)
-    * ChiantiPy.core.RadLoss_(module)                 * choice2Dialog_(class_in
-    * ChiantiPy.core.Spectrum_(module)                  ChiantiPy.Gui.gui_cl.gui)
-    * ChiantiPy.core.tests_(module)                         o (class_in
-    * ChiantiPy.core.tests.test_Continuum_                    ChiantiPy.Gui.gui_qt5.gui)
-      (module)                                        * chpicker_(class_in
-    * ChiantiPy.core.tests.test_Ion_(module)            ChiantiPy.Gui.gui_qt5.gui)
-    * ChiantiPy.core.tests.test_Ioneq_(module)        * chpicker()_(in_module
-    * ChiantiPy.core.tests.test_Spectrum_(module)       ChiantiPy.Gui.gui_cl.gui)
-    * ChiantiPy.fortranformat_(module)                * cireclvlRead()_(in_module
-    * ChiantiPy.fortranformat.config_(module)           ChiantiPy.tools.io)
-    * ChiantiPy.fortranformat.FortranRecordReader     * continuum_(class_in
-      (module)                                          ChiantiPy.core.Continuum)
-    * ChiantiPy.fortranformat.FortranRecordWriter     * convertName()_(in_module
-      (module)                                          ChiantiPy.tools.io)
-    * ChiantiPy.Gui_(module)                                o (in_module_ChiantiPy.tools.util)
-    * ChiantiPy.Gui.gui_cl_(module)                   * convolve()_
+                                                      * ChiantiPy.Gui.gui_qt5.gui_(module)
+    * calculate()_(ChiantiPy.core.Ioneq.ioneq         * ChiantiPy.Gui.gui_qt5.ui_(module)
+      method)                                         * ChiantiPy.model_(module)
+    * calculate_free_bound_loss()_                    * ChiantiPy.model.Maker_(module)
+      (ChiantiPy.core.Continuum.continuum_method)     * ChiantiPy.tests_(module)
+    * ChiantiPy_(module)                              * ChiantiPy.tests.setup_package_(module)
+    * ChiantiPy.base_(module)                         * ChiantiPy.tools_(module)
+    * ChiantiPy.base._IonTrails_(module)              * ChiantiPy.tools.archival_(module)
+    * ChiantiPy.base._SpecTrails_(module)             * ChiantiPy.tools.constants_(module)
+    * ChiantiPy.core_(module)                         * ChiantiPy.tools.data_(module)
+    * ChiantiPy.core.Continuum_(module)               * ChiantiPy.tools.filters_(module)
+    * ChiantiPy.core.Ion_(module)                     * ChiantiPy.tools.io_(module)
+    * ChiantiPy.core.Ioneq_(module)                   * ChiantiPy.tools.mputil_(module)
+    * ChiantiPy.core.IpyMspectrum_(module)            * ChiantiPy.tools.sources_(module)
+    * ChiantiPy.core.Mspectrum_(module)               * ChiantiPy.tools.util_(module)
+    * ChiantiPy.core.RadLoss_(module)                 * ChiantiPy.version_(module)
+    * ChiantiPy.core.Spectrum_(module)                * choice2Dialog_(class_in
+    * ChiantiPy.core.tests_(module)                     ChiantiPy.Gui.gui_cl.gui)
+    * ChiantiPy.core.tests.test_Continuum_                  o (class_in
+      (module)                                                ChiantiPy.Gui.gui_qt5.gui)
+    * ChiantiPy.core.tests.test_Ion_(module)          * chpicker_(class_in
+    * ChiantiPy.core.tests.test_Ioneq_(module)          ChiantiPy.Gui.gui_qt5.gui)
+    * ChiantiPy.core.tests.test_Spectrum_(module)     * chpicker()_(in_module
+    * ChiantiPy.fortranformat_(module)                  ChiantiPy.Gui.gui_cl.gui)
+    * ChiantiPy.fortranformat.config_(module)         * cireclvlRead()_(in_module
+    * ChiantiPy.fortranformat.FortranRecordReader       ChiantiPy.tools.io)
+      (module)                                        * continuum_(class_in
+    * ChiantiPy.fortranformat.FortranRecordWriter       ChiantiPy.core.Continuum)
+      (module)                                        * convertName()_(in_module
+    * ChiantiPy.Gui_(module)                            ChiantiPy.tools.io)
+    * ChiantiPy.Gui.gui_cl_(module)                         o (in_module_ChiantiPy.tools.util)
+    * ChiantiPy.Gui.gui_cl.gui_(module)               * convolve()_
                                                         (ChiantiPy.base._SpecTrails.specTrails
                                                         method)
 ***** D *****
-                                            * doAll()_(in_module
-    * defaultsRead()_(in_module               ChiantiPy.core.IpyMspectrum)
-      ChiantiPy.tools.io)                   * doFbQ()_(in_module
-    * descale_bt()_(in_module                 ChiantiPy.tools.mputil)
-      ChiantiPy.tools.util)                 * doFfQ()_(in_module
-    * descale_bti()_(in_module                ChiantiPy.tools.mputil)
-      ChiantiPy.tools.util)                 * doIonQ()_(in_module
+    * defaultsRead()_(in_module
+      ChiantiPy.tools.io)                   * doAll()_(in_module
+    * descale_bt()_(in_module                 ChiantiPy.core.IpyMspectrum)
+      ChiantiPy.tools.util)                 * doDemGofntQ()_(in_module
+    * descale_bti()_(in_module                ChiantiPy.model.Maker)
+      ChiantiPy.tools.util)                 * doFbQ()_(in_module
     * diCross()_(ChiantiPy.core.Ion.ion       ChiantiPy.tools.mputil)
-      method)                               * drPopulate()_
-    * dilute()_(in_module                     (ChiantiPy.core.Ion.ion_method)
-      ChiantiPy.tools.util)                 * drRate()_(ChiantiPy.core.Ion.ion
-    * diRate()_(ChiantiPy.core.Ion.ion        method)
-      method)                               * drRateLvl()_
-    * diRead()_(in_module                     (ChiantiPy.core.Ion.ion_method)
-      ChiantiPy.tools.io)                   * drRead()_(in_module
-                                              ChiantiPy.tools.io)
+      method)                               * doFfQ()_(in_module
+    * diffPrintChi()_                         ChiantiPy.tools.mputil)
+      (ChiantiPy.model.Maker.maker          * doIonQ()_(in_module
+      method)                                 ChiantiPy.tools.mputil)
+    * diffPrintMc()_                        * drPopulate()_
+      (ChiantiPy.model.Maker.maker            (ChiantiPy.core.Ion.ion_method)
+      method)                               * drRate()_(ChiantiPy.core.Ion.ion
+    * dilute()_(in_module                     method)
+      ChiantiPy.tools.util)                 * drRateLvl()_
+    * diRate()_(ChiantiPy.core.Ion.ion        (ChiantiPy.core.Ion.ion_method)
+      method)                               * drRead()_(in_module
+    * diRead()_(in_module                     ChiantiPy.tools.io)
+      ChiantiPy.tools.io)
 ***** E *****
-    * eaCross()_(ChiantiPy.core.Ion.ion
-      method)                               * elvlcWrite()_(in_module
-    * eaDescale()_                            ChiantiPy.tools.archival)
-      (ChiantiPy.core.Ion.ion_method)             o (in_module
-    * eaRate()_(ChiantiPy.core.Ion.ion              ChiantiPy.tools.io)
+                                            * emFitPlot()_
+                                              (ChiantiPy.model.Maker.maker
+    * eaCross()_(ChiantiPy.core.Ion.ion       method)
       method)                               * emiss()_(ChiantiPy.core.Ion.ion
-    * eaRead()_(in_module                     method)
-      ChiantiPy.tools.io)                   * emissList()_
+    * eaDescale()_                            method)
+      (ChiantiPy.core.Ion.ion_method)       * emissList()_
+    * eaRate()_(ChiantiPy.core.Ion.ion        (ChiantiPy.core.Ion.ion_method)
+      method)                               * emissPlot()_
+    * eaRead()_(in_module                     (ChiantiPy.core.Ion.ion_method)
+      ChiantiPy.tools.io)                   * emissRatio()_
     * el2z()_(in_module                       (ChiantiPy.core.Ion.ion_method)
-      ChiantiPy.tools.util)                 * emissPlot()_
-    * elvlcRead()_(in_module                  (ChiantiPy.core.Ion.ion_method)
-      ChiantiPy.tools.archival)             * emissRatio()_
-          o (in_module                        (ChiantiPy.core.Ion.ion_method)
-            ChiantiPy.tools.io)
+      ChiantiPy.tools.util)                 * emNtSetIndices()_
+    * elvlcRead()_(in_module                  (ChiantiPy.model.Maker.maker
+      ChiantiPy.tools.archival)               method)
+          o (in_module                      * emPlot()_
+            ChiantiPy.tools.io)               (ChiantiPy.model.Maker.maker
+    * elvlcWrite()_(in_module                 method)
+      ChiantiPy.tools.archival)             * emSet()_
+          o (in_module                        (ChiantiPy.model.Maker.maker
+            ChiantiPy.tools.io)               method)
+                                            * emSetIndices()_
+                                              (ChiantiPy.model.Maker.maker
+                                              method)
 ***** F *****
-                                                                                 * freeBound()_
-                                                                                   (ChiantiPy.core.Continuum.continuum
-                                                                                   method)
-                                                                                 * freeBoundEmiss()_
-                                                                                   (ChiantiPy.core.Continuum.continuum
-    * fblvlRead()_(in_module_ChiantiPy.tools.io)                                   method)
+                                                                                 * FortranRecordWriter_(class_in
+                                                                                   ChiantiPy.fortranformat.FortranRecordWriter)
+    * fblvlRead()_(in_module_ChiantiPy.tools.io)                                 * free_free_loss()_
+    * findMinMaxIndices()_(ChiantiPy.model.Maker.maker_method)                     (ChiantiPy.core.Continuum.continuum_method)
+    * fit1t()_(ChiantiPy.model.Maker.maker_method)                               * freeBound()_
+    * fitFunc1t()_(ChiantiPy.model.Maker.maker_method)                             (ChiantiPy.core.Continuum.continuum_method)
+    * fitFuncNt()_(ChiantiPy.model.Maker.maker_method)                           * freeBoundEmiss()_
+    * fitNt()_(ChiantiPy.model.Maker.maker_method)                                 (ChiantiPy.core.Continuum.continuum_method)
     * format_                                                                    * freeBoundLoss()_
-      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader             (ChiantiPy.core.Continuum.continuum
-      attribute)                                                                   method)
-          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter     * freeBoundLossMewe()_
-            attribute)                                                             (ChiantiPy.core.Continuum.continuum
-    * FortranRecordReader_(class_in                                                method)
-      ChiantiPy.fortranformat.FortranRecordReader)                               * freeBoundwB()_
-    * FortranRecordWriter_(class_in                                                (ChiantiPy.core.Continuum.continuum
-      ChiantiPy.fortranformat.FortranRecordWriter)                                 method)
-    * free_free_loss()_(ChiantiPy.core.Continuum.continuum_method)               * freeFree()_
-                                                                                   (ChiantiPy.core.Continuum.continuum
-                                                                                   method)
+      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader             (ChiantiPy.core.Continuum.continuum_method)
+      attribute)                                                                 * freeBoundLossMewe()_
+          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter       (ChiantiPy.core.Continuum.continuum_method)
+            attribute)                                                           * freeBoundwB()_
+    * FortranRecordReader_(class_in                                                (ChiantiPy.core.Continuum.continuum_method)
+      ChiantiPy.fortranformat.FortranRecordReader)                               * freeFree()_
+                                                                                   (ChiantiPy.core.Continuum.continuum_method)
                                                                                  * freeFreeLoss()_
-                                                                                   (ChiantiPy.core.Continuum.continuum
-                                                                                   method)
+                                                                                   (ChiantiPy.core.Continuum.continuum_method)
 ***** G *****
-                                                                                 * get_package_data()_(in_module
-                                                                                   ChiantiPy.tests.setup_package)
-    * gaussian()_(in_module_ChiantiPy.tools.filters)                             * gffintRead()_(in_module
-    * gaussianR()_(in_module_ChiantiPy.tools.filters)                              ChiantiPy.tools.io)
-    * get_format()_                                                              * gffRead()_(in_module
-      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader             ChiantiPy.tools.io)
-      method)                                                                    * gofnt()_
-          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter       (ChiantiPy.core.Ion.ion
-            method)                                                                method)
+                                                                                 * getNormalizedChisq()_
+                                                                                   (ChiantiPy.model.Maker.maker
+                                                                                   method)
+    * gaussian()_(in_module_ChiantiPy.tools.filters)                             * getWeightedDiff()_
+    * gaussianR()_(in_module_ChiantiPy.tools.filters)                              (ChiantiPy.model.Maker.maker
+    * get_format()_                                                                method)
+      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader           * gffintRead()_(in_module
+      method)                                                                      ChiantiPy.tools.io)
+          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter     * gffRead()_(in_module
+            method)                                                                ChiantiPy.tools.io)
+    * get_package_data()_(in_module_ChiantiPy.tests.setup_package)               * gofnt()_(ChiantiPy.core.Ion.ion
+    * getChisq()_(ChiantiPy.model.Maker.maker_method)                              method)
+                                                                                       o (ChiantiPy.model.Maker.maker
+                                                                                         method)
                                                                                  * grndLevelsRead()_(in_module
                                                                                    ChiantiPy.tools.io)
 ***** I *****
     * incident()_                              * ioneq_one()_
       (ChiantiPy.tools.sources.blackStar         (ChiantiPy.core.Continuum.continuum
       method)                                    method)
     * initUI()_                                * ioneqOne()_
@@ -168,60 +186,71 @@
     * lineSpectrumPlot()_                          ChiantiPy.tools.util)
       (ChiantiPy.base._SpecTrails.specTrails     * load()_
       method)                                      (ChiantiPy.core.Ioneq.ioneq
     * listFiles()_(in_module                       method)
       ChiantiPy.tools.util)                      * lorentz()_(in_module
                                                    ChiantiPy.tools.filters)
 ***** M *****
-                                                                           * mewe_gaunt_factor()_
-    * masterListInfo()_(in_module_ChiantiPy.tools.io)                        (ChiantiPy.core.Continuum.continuum
-    * masterListRead()_(in_module_ChiantiPy.tools.io)                        method)
-    * match()_                                                             * moffat()_(in_module
-      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader       ChiantiPy.tools.filters)
-      method)                                                              * mspectrum_(class_in
-                                                                             ChiantiPy.core.Mspectrum)
+    * makeMatchPkl()_(in
+      module
+      ChiantiPy.model.Maker)     * match()_
+    * maker_(class_in              (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader
+      ChiantiPy.model.Maker)       method)
+    * masterListInfo()_(in       * mewe_gaunt_factor()_(ChiantiPy.core.Continuum.continuum_method)
+      module                     * mgofnt()_(ChiantiPy.model.Maker.maker_method)
+      ChiantiPy.tools.io)        * moffat()_(in_module_ChiantiPy.tools.filters)
+    * masterListRead()_(in       * mspectrum_(class_in_ChiantiPy.core.Mspectrum)
+      module
+      ChiantiPy.tools.io)
 ***** O *****
     * openFileNameDialog()_(ChiantiPy.Gui.gui_qt5.gui.chpicker_method)
 ***** P *****
-    * p2eRatio()_                         * plotRatio()_
-      (ChiantiPy.core.Ion.ion_method)       (ChiantiPy.core.Ioneq.ioneq
+                                          * popPlot()_(ChiantiPy.core.Ion.ion
+    * p2eRatio()_                           method)
+      (ChiantiPy.core.Ion.ion_method)     * populate()_(ChiantiPy.core.Ion.ion
     * photoxRead()_(in_module               method)
-      ChiantiPy.tools.io)                 * popPlot()_(ChiantiPy.core.Ion.ion
-    * plot()_                               method)
-      (ChiantiPy.core.Ioneq.ioneq         * populate()_(ChiantiPy.core.Ion.ion
-      method)                               method)
+      ChiantiPy.tools.io)                 * predict()_
+    * plot()_                               (ChiantiPy.model.Maker.maker
+      (ChiantiPy.core.Ioneq.ioneq           method)
+      method)                             * predictPrint()_
+    * plotRatio()_                          (ChiantiPy.model.Maker.maker
+      (ChiantiPy.core.Ioneq.ioneq           method)
+      method)                             * predictPrint1d()_
+                                            (ChiantiPy.model.Maker.maker
+                                            method)
 ***** Q *****
     * qrp()_(in_module_ChiantiPy.tools.util)
 ***** R *****
                                                                            * reset()_(in_module_ChiantiPy.fortranformat.config)
     * radLoss_(class_in_ChiantiPy.core.RadLoss)                            * retranslateUi()_
     * radLossPlot()_(ChiantiPy.core.RadLoss.radLoss_method)                  (ChiantiPy.Gui.gui_qt5.ui.Ui_choice2DialogForm
     * read()_                                                                method)
       (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader           o (ChiantiPy.Gui.gui_qt5.ui.Ui_selectorDialogForm
       method)                                                                      method)
     * recombRate()_(ChiantiPy.core.Ion.ion_method)                         * rrLossRead()_(in_module_ChiantiPy.tools.io)
     * reject()_(ChiantiPy.Gui.gui_qt5.gui.choice2Dialog_method)            * rrlvlDescale()_(ChiantiPy.core.Ion.ion_method)
           o (ChiantiPy.Gui.gui_qt5.gui.selectorDialog_method)              * rrRate()_(ChiantiPy.core.Ion.ion_method)
                                                                            * rrRead()_(in_module_ChiantiPy.tools.io)
 ***** S *****
-                                                                                 * setupUi()_
-    * scale_bt()_(in_module_ChiantiPy.tools.util)                                  (ChiantiPy.Gui.gui_qt5.ui.Ui_choice2DialogForm
-    * scale_bt_rate()_(in_module_ChiantiPy.tools.util)                             method)
-    * scale_bti()_(in_module_ChiantiPy.tools.util)                                     o (ChiantiPy.Gui.gui_qt5.ui.Ui_selectorDialogForm
-    * scale_classical()_(in_module_ChiantiPy.tools.util)                                 method)
-    * scupsRead()_(in_module_ChiantiPy.tools.io)                                 * specTrails_(class_in_ChiantiPy.base._SpecTrails)
-    * selectorDialog_(class_in_ChiantiPy.Gui.gui_cl.gui)                         * spectroscopic2name()_(in_module_ChiantiPy.tools.util)
-          o (class_in_ChiantiPy.Gui.gui_qt5.gui)                                 * spectrum_(class_in_ChiantiPy.core.Spectrum)
-    * set_format()_                                                              * spectrum()_(ChiantiPy.core.Ion.ion_method)
-      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader           * spectrumPlot()_(ChiantiPy.base._SpecTrails.specTrails
-      method)                                                                      method)
-          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter     * splomDescale()_(in_module_ChiantiPy.tools.util)
-            method)                                                              * splomRead()_(in_module_ChiantiPy.tools.io)
-    * setup()_(ChiantiPy.core.Ion.ion_method)                                    * splupsRead()_(in_module_ChiantiPy.tools.io)
-    * setupIonrec()_(ChiantiPy.core.Ion.ion_method)                              * sutherland_gaunt_factor()_
+                                                                                 * setupIonrec()_(ChiantiPy.core.Ion.ion_method)
+    * scale_bt()_(in_module_ChiantiPy.tools.util)                                * setupUi()_
+    * scale_bt_rate()_(in_module_ChiantiPy.tools.util)                             (ChiantiPy.Gui.gui_qt5.ui.Ui_choice2DialogForm
+    * scale_bti()_(in_module_ChiantiPy.tools.util)                                 method)
+    * scale_classical()_(in_module_ChiantiPy.tools.util)                               o (ChiantiPy.Gui.gui_qt5.ui.Ui_selectorDialogForm
+    * scupsRead()_(in_module_ChiantiPy.tools.io)                                         method)
+    * search1dSpace()_(ChiantiPy.model.Maker.maker_method)                       * specTrails_(class_in_ChiantiPy.base._SpecTrails)
+    * search1tEmSpace()_(ChiantiPy.model.Maker.maker_method)                     * spectroscopic2name()_(in_module_ChiantiPy.tools.util)
+    * selectorDialog_(class_in_ChiantiPy.Gui.gui_cl.gui)                         * spectrum_(class_in_ChiantiPy.core.Spectrum)
+          o (class_in_ChiantiPy.Gui.gui_qt5.gui)                                 * spectrum()_(ChiantiPy.core.Ion.ion_method)
+    * set_format()_                                                              * spectrumPlot()_(ChiantiPy.base._SpecTrails.specTrails
+      (ChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader             method)
+      method)                                                                    * splomDescale()_(in_module_ChiantiPy.tools.util)
+          o (ChiantiPy.fortranformat.FortranRecordWriter.FortranRecordWriter     * splomRead()_(in_module_ChiantiPy.tools.io)
+            method)                                                              * splupsRead()_(in_module_ChiantiPy.tools.io)
+    * setup()_(ChiantiPy.core.Ion.ion_method)                                    * sutherland_gaunt_factor()_
                                                                                    (ChiantiPy.core.Continuum.continuum_method)
 ***** T *****
                                                * test_load_ioneq_alternate_file()_(in
     * test_abundance()_(in_module                module
       ChiantiPy.core.tests.test_Ion)             ChiantiPy.core.tests.test_Ioneq)
     * test_bunch()_(in_module                  * test_spectrum_array()_(in_module
       ChiantiPy.core.tests.test_Spectrum)        ChiantiPy.core.tests.test_Spectrum)
@@ -269,9 +298,9 @@
       ChiantiPy.tools.util)            ChiantiPy.tools.io)
     * zion2filename()_(in_module           o (in_module_ChiantiPy.tools.util)
       ChiantiPy.tools.util)          * zion2spectroscopic()_(in_module
                                        ChiantiPy.tools.util)
 **** Navigation ****
     * index
     * modules |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/getting_started.html` & `ChiantiPy-0.9.5/docs/build/html/getting_started.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/IDL_intro.html` & `ChiantiPy-0.9.5/docs/build/IDL_intro.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Intro for CHIANTI IDL Users &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Intro for CHIANTI IDL Users &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="resources.html" title="Resources for ChiantiPy Users"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="notes.html" title="Notes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="notes.html"
                         title="previous chapter">Notes</a></p>
@@ -242,22 +242,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="resources.html" title="Resources for ChiantiPy Users"
              >next</a> |</li>
         <li class="right" >
           <a href="notes.html" title="Notes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Notes
 *** Next topic ***
 Resources_for_ChiantiPy_Users
 **** Quick search ****
 [q                   ] [Go]
 ****** Intro for CHIANTI IDL UsersÂ¶ ******
@@ -188,9 +188,9 @@
 Lutz and the handy Python Pocket Reference, also by Mark Lutz. The first one is
 alway in reach and copies of the latter is on all of my computer desks.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/2.selector.png` & `ChiantiPy-0.9.5/docs/build/html/_images/2.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/bunch_selector.png` & `ChiantiPy-0.9.5/docs/build/html/_images/bunch_selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/continuum_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_images/continuum_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt.selector.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.gofnt_alternate.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.gofnt_alternate.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.ratio.vs.d.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.ratio.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.ratio.vs.t.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.ratio.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.vs.d.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.int.vs.t.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.int.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.popplot.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.popplot.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.rel.emiss.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.rel.emiss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum2.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14.spectrum_label.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14.spectrum_label.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14_intensity_plot_log.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14_intensity_plot_log.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe14_intensity_plot_log_index2.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe14_intensity_plot_log_index2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe_12_wvlranges_ratio.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe_12_wvlranges_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe_13_14_15_ioneq.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe_13_14_15_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe_25_ff_fb_tp_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe_25_ff_fb_tp_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/fe_ioneq.png` & `ChiantiPy-0.9.5/docs/build/html/_images/fe_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_spectrum.png` & `ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_t_ratio.png` & `ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_t_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/ne6_mg6_t_ratio_top7.png` & `ChiantiPy-0.9.5/docs/build/html/_images/ne6_mg6_t_ratio_top7.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/radloss.png` & `ChiantiPy-0.9.5/docs/build/html/_images/radloss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_10_20.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_10_20.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_3panel.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_3panel.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_integrated.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_integrated.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_200_300_w_si_9.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_200_300_w_si_9.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_images/spectrum_2e7_1.84_1.90.png` & `ChiantiPy-0.9.5/docs/build/html/_images/spectrum_2e7_1.84_1.90.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/IDL_intro.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/IDL_intro.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.Gui.gui_qt5.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.base.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.base.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.core.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.core.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.core.tests.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.core.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.fortranformat.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.fortranformat.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/api/ChiantiPy.tools.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/api/ChiantiPy.tools.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/changelog.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/changelog.rst.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,63 @@
 ===========
 Changelog
 ===========
 
+
+Changes from 0.9.4 to 0.9.5
+===========================
+
+this is a bug-fix release.
+
+a bug in the inherited method base._IntensityRatio() had a problem if lines were selected from different ions
+
+
+Changes from 0.9.3 to 0.9.4
+===========================
+
+this is a bug-fix release.
+
+changes in version 0.9.2 continued to give problems with ions that included autoionization rates
+
+
+Changes from 0.9.3 to 0.9.3
+===========================
+
+this is a bug-fix release.
+
+changes in version 0.9.2 gave problems with ions that included autoionization rates
+
+
+
+Changes from 0.9.2 to 0.9.3
+===========================
+
+this is a bug-fix release.
+
+changes in version 0.9.2 led to an error where ion.recombRate did not work.  This has been fixed
+
+
+Changes from 0.9.1 to 0.9.2
+===========================
+
+this is a bug-fix release.
+
+changes in version 0.9.1 lead to an error where a bare ion has not recombination rate.  This has been fixed
+
+
+Changes from 0.9.0 to 0.9.1
+===========================
+
+this is a bug-fix release.
+
+in cases when it is not possible to calculate the free-bound continuum for some ion, mspectrum did not handle this correctly and crashed
+
+also, the ion zn_31 (Zn XXXI) is a bare ion and has no ionization potential (IP) and looking it up caused indexing errors.
+
+
 Changes from 0.8.7 to 0.9.0
 ===========================
 
 a new module model.maker has been added
 
 ::
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/getting_started.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/getting_started.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/index.rst.txt` & `ChiantiPy-0.9.5/docs/build/_sources/index.rst.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
    contain the root `toctree` directive.
 
 ChiantiPy Documentation
 =======================
 
 Welcome to the ChiantiPy documentation. ChiantiPy is a pure Python package for performing calculations of astrophysical spectra using the `CHIANTI atomic database <http://www.chiantidatabase.org/>`_.
 
-The latest version of ChiantiPy is 0.9.0 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions
+The latest version of ChiantiPy is 0.9.5 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions
 
-ChiantiPy v0.9.0 is released under the OSI approved ISC license. From `Wikipedia <https://en.wikipedia.org/w/index.php?title=ISC_license&oldid=664696993>`_: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, ...
+ChiantiPy v0.9.5 is released under the OSI approved ISC license. From `Wikipedia <https://en.wikipedia.org/w/index.php?title=ISC_license&oldid=664696993>`_: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, ...
 
 `CHIANTI <http://www.chiantidatabase.org/>`_ consists of a database of atomic data that can be used to interpret spectral lines and continua emitted from high-temperature, optically-thin astrophysical sources.
 
 CHIANTI is developed and maintained by scientists at George Mason University (USA), the University of Michigan (USA), and the University of Cambridge (UK). The first version of CHIANTI was released in 1997 and version 9.0 in 2019.
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/notes.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/notes.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/quick_start.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/quick_start.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_sources/tutorial.rst.txt` & `ChiantiPy-0.9.5/docs/build/html/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/2.selector.png` & `ChiantiPy-0.9.5/docs/build/html/_static/2.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/ajax-loader.gif` & `ChiantiPy-0.9.5/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/basic.css` & `ChiantiPy-0.9.5/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/bunch_selector.png` & `ChiantiPy-0.9.5/docs/build/html/_static/bunch_selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/chiantipy_logo.png` & `ChiantiPy-0.9.5/docs/build/html/_static/chiantipy_logo.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/comment-bright.png` & `ChiantiPy-0.9.5/docs/build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/comment-close.png` & `ChiantiPy-0.9.5/docs/build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/comment.png` & `ChiantiPy-0.9.5/docs/build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/continuum_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_static/continuum_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/doctools.js` & `ChiantiPy-0.9.5/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt.selector.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.gofnt_alternate.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.gofnt_alternate.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.ratio.vs.d.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.ratio.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.ratio.vs.t.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.ratio.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.vs.d.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.int.vs.t.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.int.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.popplot.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.popplot.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.rel.emiss.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.rel.emiss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum2.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14.spectrum_label.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14.spectrum_label.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14_intensity_plot_log.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14_intensity_plot_log.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe14_intensity_plot_log_index2.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe14_intensity_plot_log_index2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe_12_wvlranges_ratio.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe_12_wvlranges_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe_13_14_15_ioneq.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe_13_14_15_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe_25_ff_fb_tp_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe_25_ff_fb_tp_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/fe_ioneq.png` & `ChiantiPy-0.9.5/docs/build/html/_static/fe_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/jquery-3.1.0.js` & `ChiantiPy-0.9.5/docs/build/html/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/jquery-3.2.1.js` & `ChiantiPy-0.9.5/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/jquery.js` & `ChiantiPy-0.9.5/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_spectrum.png` & `ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_t_ratio.png` & `ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_t_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/ne6_mg6_t_ratio_top7.png` & `ChiantiPy-0.9.5/docs/build/html/_static/ne6_mg6_t_ratio_top7.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/pygments.css` & `ChiantiPy-0.9.5/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/radloss.png` & `ChiantiPy-0.9.5/docs/build/html/_static/radloss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/searchtools.js` & `ChiantiPy-0.9.5/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_10_20.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_10_20.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_1_10.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_3panel.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_3panel.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_integrated.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_integrated.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_200_300_w_si_9.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_200_300_w_si_9.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/spectrum_2e7_1.84_1.90.png` & `ChiantiPy-0.9.5/docs/build/html/_static/spectrum_2e7_1.84_1.90.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/sphinxdoc.css` & `ChiantiPy-0.9.5/docs/build/html/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/theme.conf` & `ChiantiPy-0.9.5/docs/build/html/_static/theme.conf`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/underscore-1.3.1.js` & `ChiantiPy-0.9.5/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/underscore.js` & `ChiantiPy-0.9.5/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/_static/websupport.js` & `ChiantiPy-0.9.5/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.gui_cl.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.gui_cl.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.Gui.gui_cl package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.Gui.gui_cl package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_qt5.html" title="ChiantiPy.Gui.gui_qt5 package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.html" title="ChiantiPy.Gui package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.Gui.html" accesskey="U">ChiantiPy.Gui package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
@@ -134,25 +134,25 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_qt5.html" title="ChiantiPy.Gui.gui_qt5 package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.html" title="ChiantiPy.Gui package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.Gui.html" >ChiantiPy.Gui package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.Gui_package »
 *** Previous topic ***
 ChiantiPy.Gui_package
 *** Next topic ***
 ChiantiPy.Gui.gui_qt5_package
@@ -45,12 +45,12 @@
 ***** Module contentsÂ¶ *****
 command-line selection dialogs
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.Gui_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.gui_qt5.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.gui_qt5.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.Gui.gui_qt5 package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.Gui.gui_qt5 package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.base.html" title="ChiantiPy.base package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_cl.html" title="ChiantiPy.Gui.gui_cl package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.Gui.html" accesskey="U">ChiantiPy.Gui package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
@@ -198,25 +198,25 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.base.html" title="ChiantiPy.base package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_cl.html" title="ChiantiPy.Gui.gui_cl package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.Gui.html" >ChiantiPy.Gui package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.Gui_package »
 *** Previous topic ***
 ChiantiPy.Gui.gui_cl_package
 *** Next topic ***
 ChiantiPy.base_package
@@ -60,12 +60,12 @@
 ***** Module contentsÂ¶ *****
 PyQt5 selection dialog widgets
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.Gui_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.Gui.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.Gui.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.Gui package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.Gui package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_cl.html" title="ChiantiPy.Gui.gui_cl package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.html" title="ChiantiPy package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
@@ -119,24 +119,24 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_cl.html" title="ChiantiPy.Gui.gui_cl package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.html" title="ChiantiPy package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
 ChiantiPy_package
 *** Next topic ***
 ChiantiPy.Gui.gui_cl_package
 **** Quick search ****
@@ -34,11 +34,11 @@
 ***** Module contentsÂ¶ *****
 Select GUI package
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.base.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.base.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.base package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.base package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.html" title="ChiantiPy.core package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_qt5.html" title="ChiantiPy.Gui.gui_qt5 package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
@@ -304,24 +304,24 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.html" title="ChiantiPy.core package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.Gui.gui_qt5.html" title="ChiantiPy.Gui.gui_qt5 package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
 ChiantiPy.Gui.gui_qt5_package
 *** Next topic ***
 ChiantiPy.core_package
 **** Quick search ****
@@ -162,11 +162,11 @@
 ***** Module contentsÂ¶ *****
 Base classes for ion- and spectrum-related objects.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.core.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.core.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.core package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.core package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.tests.html" title="ChiantiPy.core.tests package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.base.html" title="ChiantiPy.base package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
@@ -1208,24 +1208,24 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.tests.html" title="ChiantiPy.core.tests package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.base.html" title="ChiantiPy.base package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
 ChiantiPy.base_package
 *** Next topic ***
 ChiantiPy.core.tests_package
 **** Quick search ****
@@ -831,11 +831,11 @@
 This software is distributed under the terms of the ISC Software License that
 is found in the LICENSE file
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.core.tests.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.core.tests.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.core.tests package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.core.tests package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.fortranformat.html" title="ChiantiPy.fortranformat package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.html" title="ChiantiPy.core package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.core.html" accesskey="U">ChiantiPy.core package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
@@ -208,25 +208,25 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.fortranformat.html" title="ChiantiPy.fortranformat package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.html" title="ChiantiPy.core package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li>
           <li class="nav-item nav-item-3"><a href="ChiantiPy.core.html" >ChiantiPy.core package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.core_package »
 *** Previous topic ***
 ChiantiPy.core_package
 *** Next topic ***
 ChiantiPy.fortranformat_package
@@ -51,12 +51,12 @@
   ChiantiPy.core.tests.test_Spectrum.test_spectrum_scalar()Â¶
 ***** Module contentsÂ¶ *****
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
     * ChiantiPy.core_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.fortranformat.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.fortranformat.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.fortranformat package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.fortranformat package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="ChiantiPy.tests package" href="ChiantiPy.tests.html" />
+    <link rel="next" title="ChiantiPy.Gui package" href="ChiantiPy.model.html" />
     <link rel="prev" title="ChiantiPy.core.tests package" href="ChiantiPy.core.tests.html" /> 
   </head><body>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 <a href="">
 <img border="0" alt="chiantipy" src="_static/chiantipy_logo.png"/>
 </a>
 </div>
@@ -32,32 +32,32 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="ChiantiPy.tests.html" title="ChiantiPy.tests package"
+          <a href="ChiantiPy.model.html" title="ChiantiPy.Gui package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.tests.html" title="ChiantiPy.core.tests package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="ChiantiPy.core.tests.html"
                         title="previous chapter">ChiantiPy.core.tests package</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="ChiantiPy.tests.html"
-                        title="next chapter">ChiantiPy.tests package</a></p>
+  <p class="topless"><a href="ChiantiPy.model.html"
+                        title="next chapter">ChiantiPy.Gui package</a></p>
 <div id="searchbox" style="display: none" role="search">
   <h3>Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" />
       <input type="submit" value="Go" />
       <input type="hidden" name="check_keywords" value="yes" />
@@ -201,29 +201,29 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="ChiantiPy.tests.html" title="ChiantiPy.tests package"
+          <a href="ChiantiPy.model.html" title="ChiantiPy.Gui package"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.core.tests.html" title="ChiantiPy.core.tests package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
 ChiantiPy.core.tests_package
 *** Next topic ***
-ChiantiPy.tests_package
+ChiantiPy.Gui_package
 **** Quick search ****
 [q                   ] [Go]
 ****** ChiantiPy.fortranformat packageÂ¶ ******
 ***** SubmodulesÂ¶ *****
 ***** ChiantiPy.fortranformat.FortranRecordReader moduleÂ¶ *****
   classChiantiPy.fortranformat.FortranRecordReader.FortranRecordReader
   (format)Â¶
@@ -73,11 +73,11 @@
   ChiantiPy.fortranformat.config.reset()Â¶
 ***** Module contentsÂ¶ *****
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.model.html` & `ChiantiPy-0.9.5/docs/build/html/api/ChiantiPy.model.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.tests.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.tests.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.tests package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.tests package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
     <link rel="next" title="ChiantiPy.tools package" href="ChiantiPy.tools.html" />
-    <link rel="prev" title="ChiantiPy.fortranformat package" href="ChiantiPy.fortranformat.html" /> 
+    <link rel="prev" title="ChiantiPy.Gui package" href="ChiantiPy.model.html" /> 
   </head><body>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 <a href="">
 <img border="0" alt="chiantipy" src="_static/chiantipy_logo.png"/>
 </a>
 </div>
     
@@ -35,26 +35,26 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.tools.html" title="ChiantiPy.tools package"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="ChiantiPy.fortranformat.html" title="ChiantiPy.fortranformat package"
+          <a href="ChiantiPy.model.html" title="ChiantiPy.Gui package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
-  <p class="topless"><a href="ChiantiPy.fortranformat.html"
-                        title="previous chapter">ChiantiPy.fortranformat package</a></p>
+  <p class="topless"><a href="ChiantiPy.model.html"
+                        title="previous chapter">ChiantiPy.Gui package</a></p>
   <h4>Next topic</h4>
   <p class="topless"><a href="ChiantiPy.tools.html"
                         title="next chapter">ChiantiPy.tools package</a></p>
 <div id="searchbox" style="display: none" role="search">
   <h3>Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="../search.html" method="get">
@@ -108,26 +108,26 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.tools.html" title="ChiantiPy.tools package"
              >next</a> |</li>
         <li class="right" >
-          <a href="ChiantiPy.fortranformat.html" title="ChiantiPy.fortranformat package"
+          <a href="ChiantiPy.model.html" title="ChiantiPy.Gui package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,19 +7,19 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
-ChiantiPy.fortranformat_package
+ChiantiPy.Gui_package
 *** Next topic ***
 ChiantiPy.tools_package
 **** Quick search ****
 [q                   ] [Go]
 ****** ChiantiPy.tests packageÂ¶ ******
 ***** SubmodulesÂ¶ *****
 ***** ChiantiPy.tests.setup_package moduleÂ¶ *****
@@ -27,11 +27,11 @@
 ***** Module contentsÂ¶ *****
 This packages contains affiliated package tests.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/ChiantiPy.tools.html` & `ChiantiPy-0.9.5/docs/build/api/ChiantiPy.tools.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy.tools package &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy.tools package &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../notes.html" title="Notes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.tests.html" title="ChiantiPy.tests package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" accesskey="U">ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
@@ -1687,24 +1687,24 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../notes.html" title="Notes"
              >next</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.tests.html" title="ChiantiPy.tests package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >ChiantiPy’s API documentation</a> &#187;</li>
           <li class="nav-item nav-item-2"><a href="ChiantiPy.html" >ChiantiPy package</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
 *** Previous topic ***
 ChiantiPy.tests_package
 *** Next topic ***
 Notes
 **** Quick search ****
@@ -692,11 +692,11 @@
 ***** Module contentsÂ¶ *****
 Basic tools and utilities used in ChiantiPy
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
     * ChiantiPyâs_API_documentation »
     * ChiantiPy_package »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/index.html` & `ChiantiPy-0.9.5/docs/build/api/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy’s API documentation &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy’s API documentation &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="../_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="../" src="../_static/documentation_options.js"></script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.html" title="ChiantiPy package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="../tutorial.html" title="Tutorial"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="../tutorial.html"
                         title="previous chapter">Tutorial</a></p>
@@ -111,15 +111,16 @@
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordReader">ChiantiPy.fortranformat.FortranRecordReader module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.FortranRecordWriter">ChiantiPy.fortranformat.FortranRecordWriter module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat.config">ChiantiPy.fortranformat.config module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.fortranformat.html#module-ChiantiPy.fortranformat">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="ChiantiPy.model.html">ChiantiPy.Gui package</a><ul>
-<li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#subpackages">Subpackages</a></li>
+<li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#submodules">Submodules</a></li>
+<li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#module-ChiantiPy.model.Maker">ChiantiPy.model.Maker module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.model.html#module-ChiantiPy.model">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="ChiantiPy.tests.html">ChiantiPy.tests package</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#submodules">Submodules</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests.setup_package">ChiantiPy.tests.setup_package module</a></li>
 <li class="toctree-l4"><a class="reference internal" href="ChiantiPy.tests.html#module-ChiantiPy.tests">Module contents</a></li>
@@ -174,22 +175,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ChiantiPy.html" title="ChiantiPy package"
              >next</a> |</li>
         <li class="right" >
           <a href="../tutorial.html" title="Tutorial"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="../index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Tutorial
 *** Next topic ***
 ChiantiPy_package
 **** Quick search ****
 [q                   ] [Go]
 ****** ChiantiPyâs API documentationÂ¶ ******
@@ -44,15 +44,16 @@
                 # ChiantiPy.fortranformat_package
                       # Submodules
                       # ChiantiPy.fortranformat.FortranRecordReader_module
                       # ChiantiPy.fortranformat.FortranRecordWriter_module
                       # ChiantiPy.fortranformat.config_module
                       # Module_contents
                 # ChiantiPy.Gui_package
-                      # Subpackages
+                      # Submodules
+                      # ChiantiPy.model.Maker_module
                       # Module_contents
                 # ChiantiPy.tests_package
                       # Submodules
                       # ChiantiPy.tests.setup_package_module
                       # Module_contents
                 # ChiantiPy.tools_package
                       # Submodules
@@ -73,9 +74,9 @@
     * Module_Index
     * Search_Page
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/api/modules.html` & `ChiantiPy-0.9.5/docs/build/html/api/modules.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/bugs.html` & `ChiantiPy-0.9.5/docs/build/bugs.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Reporting Bugs &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Reporting Bugs &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -33,15 +33,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="changelog.html"
                         title="previous chapter">Changelog</a></p>
@@ -84,22 +84,22 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,22 +5,22 @@
 
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Changelog
 **** Quick search ****
 [q                   ] [Go]
 ****** Reporting BugsÂ¶ ******
 All bugs are kept track of on the GitHub_issue_tracker. If you run into any
 unexpected behavior or have a question please send_an_email or add an issue
 directly to the issue tracker.
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/changelog.html` & `ChiantiPy-0.9.5/docs/build/changelog.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Changelog &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Changelog &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="bugs.html" title="Reporting Bugs"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="resources.html" title="Resources for ChiantiPy Users"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="resources.html"
                         title="previous chapter">Resources for ChiantiPy Users</a></p>
@@ -70,14 +70,45 @@
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <div class="section" id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this headline">¶</a></h1>
+<div class="section" id="changes-from-0-9-4-to-0-9-5">
+<h2>Changes from 0.9.4 to 0.9.5<a class="headerlink" href="#changes-from-0-9-4-to-0-9-5" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>a bug in the inherited method base._IntensityRatio() had a problem if lines were selected from different ions</p>
+</div>
+<div class="section" id="changes-from-0-9-3-to-0-9-4">
+<h2>Changes from 0.9.3 to 0.9.4<a class="headerlink" href="#changes-from-0-9-3-to-0-9-4" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>changes in version 0.9.2 continued to give problems with ions that included autoionization rates</p>
+</div>
+<div class="section" id="changes-from-0-9-3-to-0-9-3">
+<h2>Changes from 0.9.3 to 0.9.3<a class="headerlink" href="#changes-from-0-9-3-to-0-9-3" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>changes in version 0.9.2 gave problems with ions that included autoionization rates</p>
+</div>
+<div class="section" id="changes-from-0-9-2-to-0-9-3">
+<h2>Changes from 0.9.2 to 0.9.3<a class="headerlink" href="#changes-from-0-9-2-to-0-9-3" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>changes in version 0.9.2 led to an error where ion.recombRate did not work.  This has been fixed</p>
+</div>
+<div class="section" id="changes-from-0-9-1-to-0-9-2">
+<h2>Changes from 0.9.1 to 0.9.2<a class="headerlink" href="#changes-from-0-9-1-to-0-9-2" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>changes in version 0.9.1 lead to an error where a bare ion has not recombination rate.  This has been fixed</p>
+</div>
+<div class="section" id="changes-from-0-9-0-to-0-9-1">
+<h2>Changes from 0.9.0 to 0.9.1<a class="headerlink" href="#changes-from-0-9-0-to-0-9-1" title="Permalink to this headline">¶</a></h2>
+<p>this is a bug-fix release.</p>
+<p>in cases when it is not possible to calculate the free-bound continuum for some ion, mspectrum did not handle this correctly and crashed</p>
+<p>also, the ion zn_31 (Zn XXXI) is a bare ion and has no ionization potential (IP) and looking it up caused indexing errors.</p>
+</div>
 <div class="section" id="changes-from-0-8-7-to-0-9-0">
 <h2>Changes from 0.8.7 to 0.9.0<a class="headerlink" href="#changes-from-0-8-7-to-0-9-0" title="Permalink to this headline">¶</a></h2>
 <p>a new module model.maker has been added</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">ChiantiPy.model</span> <span class="k">as</span> <span class="nn">mdl</span>
 <span class="n">mymodel</span> <span class="o">=</span> <span class="n">mdl</span><span class="o">.</span><span class="n">maker</span><span class="p">(</span><span class="o">...</span><span class="p">)</span>
 </pre></div>
 </div>
@@ -189,22 +220,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="bugs.html" title="Reporting Bugs"
              >next</a> |</li>
         <li class="right" >
           <a href="resources.html" title="Resources for ChiantiPy Users"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,48 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Resources_for_ChiantiPy_Users
 *** Next topic ***
 Reporting_Bugs
 **** Quick search ****
 [q                   ] [Go]
 ****** ChangelogÂ¶ ******
+***** Changes from 0.9.4 to 0.9.5Â¶ *****
+this is a bug-fix release.
+a bug in the inherited method base._IntensityRatio() had a problem if lines
+were selected from different ions
+***** Changes from 0.9.3 to 0.9.4Â¶ *****
+this is a bug-fix release.
+changes in version 0.9.2 continued to give problems with ions that included
+autoionization rates
+***** Changes from 0.9.3 to 0.9.3Â¶ *****
+this is a bug-fix release.
+changes in version 0.9.2 gave problems with ions that included autoionization
+rates
+***** Changes from 0.9.2 to 0.9.3Â¶ *****
+this is a bug-fix release.
+changes in version 0.9.2 led to an error where ion.recombRate did not work.
+This has been fixed
+***** Changes from 0.9.1 to 0.9.2Â¶ *****
+this is a bug-fix release.
+changes in version 0.9.1 lead to an error where a bare ion has not
+recombination rate. This has been fixed
+***** Changes from 0.9.0 to 0.9.1Â¶ *****
+this is a bug-fix release.
+in cases when it is not possible to calculate the free-bound continuum for some
+ion, mspectrum did not handle this correctly and crashed
+also, the ion zn_31 (Zn XXXI) is a bare ion and has no ionization potential
+(IP) and looking it up caused indexing errors.
 ***** Changes from 0.8.7 to 0.9.0Â¶ *****
 a new module model.maker has been added
 import ChiantiPy.model as mdl
 mymodel = mdl.maker(...)
 a serious bug in ch.freeBound was fixed - the use of a single temperature was
 problematic
 ***** Changes from 0.8.6 to 0.8.7Â¶ *****
@@ -123,9 +149,9 @@
 by the Internet Software Consortium (ISC). It is functionally equivalent to the
 simplified BSD and MIT/Expat licenses, â¦
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/chiantdoc-0.8.0.tar` & `ChiantiPy-0.9.5/docs/build/html/chiantdoc-0.8.0.tar`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/genindex.html` & `ChiantiPy-0.9.5/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/getting_started.html` & `ChiantiPy-0.9.5/docs/build/getting_started.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Getting started with ChiantiPy &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Getting started with ChiantiPy &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="quick_start.html" title="Quick Start"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="ChiantiPy Documentation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="index.html"
                         title="previous chapter">ChiantiPy Documentation</a></p>
@@ -194,22 +194,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="quick_start.html" title="Quick Start"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="ChiantiPy Documentation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 ChiantiPy_Documentation
 *** Next topic ***
 Quick_Start
 **** Quick search ****
 [q                   ] [Go]
 ****** Getting started with ChiantiPyÂ¶ ******
@@ -98,9 +98,9 @@
 ChiantiPy has mostly been tested with the Qt5 backend for Matplotlib and using
 the ChiantiPy Qt5 widgets.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/html/index.html` & `ChiantiPy-0.9.5/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/notes.html` & `ChiantiPy-0.9.5/docs/build/html/notes.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/objects.inv` & `ChiantiPy-0.9.5/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/py-modindex.html` & `ChiantiPy-0.9.5/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/quick_start.html` & `ChiantiPy-0.9.5/docs/build/html/quick_start.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/resources.html` & `ChiantiPy-0.9.5/docs/build/html/resources.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/search.html` & `ChiantiPy-0.9.5/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/searchindex.js` & `ChiantiPy-0.9.5/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/html/tutorial.html` & `ChiantiPy-0.9.5/docs/build/html/tutorial.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/build/index.html` & `ChiantiPy-0.9.5/docs/build/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>ChiantiPy Documentation &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>ChiantiPy Documentation &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -33,15 +33,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="getting_started.html" title="Getting started with ChiantiPy"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="#">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Next topic</h4>
   <p class="topless"><a href="getting_started.html"
                         title="next chapter">Getting started with ChiantiPy</a></p>
@@ -64,16 +64,16 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <div class="section" id="chiantipy-documentation">
 <h1>ChiantiPy Documentation<a class="headerlink" href="#chiantipy-documentation" title="Permalink to this headline">¶</a></h1>
 <p>Welcome to the ChiantiPy documentation. ChiantiPy is a pure Python package for performing calculations of astrophysical spectra using the <a class="reference external" href="http://www.chiantidatabase.org/">CHIANTI atomic database</a>.</p>
-<p>The latest version of ChiantiPy is 0.9.0 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions</p>
-<p>ChiantiPy v0.9.0 is released under the OSI approved ISC license. From <a class="reference external" href="https://en.wikipedia.org/w/index.php?title=ISC_license&amp;oldid=664696993">Wikipedia</a>: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, …</p>
+<p>The latest version of ChiantiPy is 0.9.5 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions</p>
+<p>ChiantiPy v0.9.5 is released under the OSI approved ISC license. From <a class="reference external" href="https://en.wikipedia.org/w/index.php?title=ISC_license&amp;oldid=664696993">Wikipedia</a>: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, …</p>
 <p><a class="reference external" href="http://www.chiantidatabase.org/">CHIANTI</a> consists of a database of atomic data that can be used to interpret spectral lines and continua emitted from high-temperature, optically-thin astrophysical sources.</p>
 <p>CHIANTI is developed and maintained by scientists at George Mason University (USA), the University of Michigan (USA), and the University of Cambridge (UK). The first version of CHIANTI was released in 1997 and version 9.0 in 2019.</p>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting started with ChiantiPy</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="getting_started.html#prerequisites">Prerequisites</a></li>
 <li class="toctree-l2"><a class="reference internal" href="getting_started.html#install-the-chianti-database">Install the CHIANTI database</a></li>
@@ -113,14 +113,20 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="IDL_intro.html">Intro for CHIANTI IDL Users</a></li>
 <li class="toctree-l1"><a class="reference internal" href="resources.html">Resources for ChiantiPy Users</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="resources.html#forums">Forums</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-4-to-0-9-5">Changes from 0.9.4 to 0.9.5</a></li>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-3-to-0-9-4">Changes from 0.9.3 to 0.9.4</a></li>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-3-to-0-9-3">Changes from 0.9.3 to 0.9.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-2-to-0-9-3">Changes from 0.9.2 to 0.9.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-1-to-0-9-2">Changes from 0.9.1 to 0.9.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-9-0-to-0-9-1">Changes from 0.9.0 to 0.9.1</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-8-7-to-0-9-0">Changes from 0.8.7 to 0.9.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-8-6-to-0-8-7">Changes from 0.8.6 to 0.8.7</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-8-5-to-0-8-6">Changes from 0.8.5 to 0.8.6</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-8-4-to-0-8-5">Changes from 0.8.4 to 0.8.5</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#this-is-a-major-bug-fix-release">This is a major bug-fix release.</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#changes-from-0-8-3-to-0-8-4">Changes from 0.8.3 to 0.8.4</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#id1">This is a major bug-fix release.</a></li>
@@ -161,22 +167,22 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="getting_started.html" title="Getting started with ChiantiPy"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="#">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,26 +5,26 @@
 
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Next topic ***
 Getting_started_with_ChiantiPy
 **** Quick search ****
 [q                   ] [Go]
 ****** ChiantiPy DocumentationÂ¶ ******
 Welcome to the ChiantiPy documentation. ChiantiPy is a pure Python package for
 performing calculations of astrophysical spectra using the CHIANTI_atomic
 database.
-The latest version of ChiantiPy is 0.9.0 and is compatible with CHIANTI
+The latest version of ChiantiPy is 0.9.5 and is compatible with CHIANTI
 database version 9.0. It is not compatible with previous versions
-ChiantiPy v0.9.0 is released under the OSI approved ISC license. From
+ChiantiPy v0.9.5 is released under the OSI approved ISC license. From
 Wikipedia: The ISC license is a permissive free software license written by the
 Internet Software Consortium (ISC). It is functionally equivalent to the
 simplified BSD and MIT/Expat licenses, â¦
 CHIANTI consists of a database of atomic data that can be used to interpret
 spectral lines and continua emitted from high-temperature, optically-thin
 astrophysical sources.
 CHIANTI is developed and maintained by scientists at George Mason University
@@ -57,14 +57,20 @@
     * Notes
           o Setting_default_values
           o Setting_minAbund_in_spectrum_calculations
     * Intro_for_CHIANTI_IDL_Users
     * Resources_for_ChiantiPy_Users
           o Forums
     * Changelog
+          o Changes_from_0.9.4_to_0.9.5
+          o Changes_from_0.9.3_to_0.9.4
+          o Changes_from_0.9.3_to_0.9.3
+          o Changes_from_0.9.2_to_0.9.3
+          o Changes_from_0.9.1_to_0.9.2
+          o Changes_from_0.9.0_to_0.9.1
           o Changes_from_0.8.7_to_0.9.0
           o Changes_from_0.8.6_to_0.8.7
           o Changes_from_0.8.5_to_0.8.6
           o Changes_from_0.8.4_to_0.8.5
           o This_is_a_major_bug-fix_release.
           o Changes_from_0.8.3_to_0.8.4
           o This_is_a_major_bug-fix_release.
@@ -82,9 +88,9 @@
     * Index
     * Module_Index
     * Search_Page
 **** Navigation ****
     * index
     * modules |
     * next |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/notes.html` & `ChiantiPy-0.9.5/docs/build/notes.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Notes &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Notes &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="IDL_intro.html" title="Intro for CHIANTI IDL Users"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="api/ChiantiPy.tools.html" title="ChiantiPy.tools package"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="api/ChiantiPy.tools.html"
                         title="previous chapter">ChiantiPy.tools package</a></p>
@@ -405,22 +405,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="IDL_intro.html" title="Intro for CHIANTI IDL Users"
              >next</a> |</li>
         <li class="right" >
           <a href="api/ChiantiPy.tools.html" title="ChiantiPy.tools package"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 ChiantiPy.tools_package
 *** Next topic ***
 Intro_for_CHIANTI_IDL_Users
 **** Quick search ****
 [q                   ] [Go]
 ****** NotesÂ¶ ******
@@ -83,9 +83,9 @@
 It shoud be noted that CHIANTI does not include a complete set of data for
 every ion of every element in this list.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/py-modindex.html` & `ChiantiPy-0.9.5/docs/build/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Python Module Index &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Python Module Index &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -32,15 +32,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
 <div id="searchbox" style="display: none" role="search">
   <h3>Quick search</h3>
     <div class="searchformwrapper">
@@ -207,14 +207,24 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/ChiantiPy.Gui.gui_qt5.html#module-ChiantiPy.Gui.gui_qt5.ui"><code class="xref">ChiantiPy.Gui.gui_qt5.ui</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="api/ChiantiPy.model.html#module-ChiantiPy.model"><code class="xref">ChiantiPy.model</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/ChiantiPy.model.html#module-ChiantiPy.model.Maker"><code class="xref">ChiantiPy.model.Maker</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="api/ChiantiPy.tests.html#module-ChiantiPy.tests"><code class="xref">ChiantiPy.tests</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/ChiantiPy.tests.html#module-ChiantiPy.tests.setup_package"><code class="xref">ChiantiPy.tests.setup_package</code></a></td><td>
        <em></em></td></tr>
@@ -281,22 +291,22 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 **** Quick search ****
 [q                   ] [Go]
 ****** Python Module Index ******
 c
      
     c
 [-] ChiantiPy
@@ -37,14 +37,16 @@
         ChiantiPy.fortranformat.FortranRecordWriter
         ChiantiPy.Gui
         ChiantiPy.Gui.gui_cl
         ChiantiPy.Gui.gui_cl.gui
         ChiantiPy.Gui.gui_qt5
         ChiantiPy.Gui.gui_qt5.gui
         ChiantiPy.Gui.gui_qt5.ui
+        ChiantiPy.model
+        ChiantiPy.model.Maker
         ChiantiPy.tests
         ChiantiPy.tests.setup_package
         ChiantiPy.tools
         ChiantiPy.tools.archival
         ChiantiPy.tools.constants
         ChiantiPy.tools.data
         ChiantiPy.tools.filters
@@ -52,9 +54,9 @@
         ChiantiPy.tools.mputil
         ChiantiPy.tools.sources
         ChiantiPy.tools.util
         ChiantiPy.version
 **** Navigation ****
     * index
     * modules |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/quick_start.html` & `ChiantiPy-0.9.5/docs/build/quick_start.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Quick Start &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Quick Start &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="getting_started.html" title="Getting started with ChiantiPy"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="getting_started.html"
                         title="previous chapter">Getting started with ChiantiPy</a></p>
@@ -532,22 +532,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              >next</a> |</li>
         <li class="right" >
           <a href="getting_started.html" title="Getting started with ChiantiPy"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Getting_started_with_ChiantiPy
 *** Next topic ***
 Tutorial
 **** Quick search ****
 [q                   ] [Go]
 ****** Quick StartÂ¶ ******
@@ -451,9 +451,9 @@
 if abundance=âabcâ, or some name that does not match an abundance name, a
 dialog will come up so that a abundance file can be selected
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/resources.html` & `ChiantiPy-0.9.5/docs/build/resources.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Resources for ChiantiPy Users &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Resources for ChiantiPy Users &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="IDL_intro.html" title="Intro for CHIANTI IDL Users"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="IDL_intro.html"
                         title="previous chapter">Intro for CHIANTI IDL Users</a></p>
@@ -98,22 +98,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="IDL_intro.html" title="Intro for CHIANTI IDL Users"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Intro_for_CHIANTI_IDL_Users
 *** Next topic ***
 Changelog
 **** Quick search ****
 [q                   ] [Go]
 ****** Resources for ChiantiPy UsersÂ¶ ******
@@ -23,9 +23,9 @@
 The_CHIANTI_Google_group
 Github
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/build/search.html` & `ChiantiPy-0.9.5/docs/build/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Search &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Search &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
         </div>
       </div>
 
@@ -88,22 +88,22 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

### Comparing `ChiantiPy-0.9.4/docs/build/tutorial.html` & `ChiantiPy-0.9.5/docs/build/tutorial.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Tutorial &#8212; ChiantiPy 0.9.0 documentation</title>
+    <title>Tutorial &#8212; ChiantiPy 0.9.5 documentation</title>
     <link rel="stylesheet" href="_static/sphinxdoc.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
@@ -37,15 +37,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api/index.html" title="ChiantiPy’s API documentation"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="quick_start.html" title="Quick Start"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="quick_start.html"
                         title="previous chapter">Quick Start</a></p>
@@ -302,22 +302,22 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api/index.html" title="ChiantiPy’s API documentation"
              >next</a> |</li>
         <li class="right" >
           <a href="quick_start.html" title="Quick Start"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.0 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">ChiantiPy 0.9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
 <div style="padding: 20px 10px 10px 40px; background-color: #fff8d3; text-align: left;">
 
 
 </div>
     
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2019, Ken Dere.
+        &#169; Copyright 2020, Ken Dere.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.6.
     </div>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 [chiantipy]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
+    * ChiantiPy_0.9.5_documentation »
 *** Previous topic ***
 Quick_Start
 *** Next topic ***
 ChiantiPyâs_API_documentation
 **** Quick search ****
 [q                   ] [Go]
 ****** TutorialÂ¶ ******
@@ -312,9 +312,9 @@
 2.00e+6
 to be continued
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * ChiantiPy_0.9.0_documentation »
-© Copyright 2019, Ken Dere. Created using Sphinx 1.7.6.
+    * ChiantiPy_0.9.5_documentation »
+© Copyright 2020, Ken Dere. Created using Sphinx 1.7.6.
```

### Comparing `ChiantiPy-0.9.4/docs/source/IDL_intro.rst` & `ChiantiPy-0.9.5/docs/source/IDL_intro.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/2.selector.png` & `ChiantiPy-0.9.5/docs/source/_static/2.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/bunch_selector.png` & `ChiantiPy-0.9.5/docs/source/_static/bunch_selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/chiantipy_logo.png` & `ChiantiPy-0.9.5/docs/source/_static/chiantipy_logo.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/continuum_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/source/_static/continuum_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt.selector.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt.selector.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.gofnt_alternate.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.gofnt_alternate.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.int.ratio.vs.d.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.int.ratio.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.int.ratio.vs.t.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.int.ratio.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.int.vs.d.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.int.vs.d.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.int.vs.t.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.int.vs.t.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.popplot.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.popplot.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.rel.emiss.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.rel.emiss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum2.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14.spectrum_label.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14.spectrum_label.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14_intensity_plot_log.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14_intensity_plot_log.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe14_intensity_plot_log_index2.png` & `ChiantiPy-0.9.5/docs/source/_static/fe14_intensity_plot_log_index2.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe_12_wvlranges_ratio.png` & `ChiantiPy-0.9.5/docs/source/_static/fe_12_wvlranges_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe_13_14_15_ioneq.png` & `ChiantiPy-0.9.5/docs/source/_static/fe_13_14_15_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe_25_ff_fb_tp_2e7_1_10.png` & `ChiantiPy-0.9.5/docs/source/_static/fe_25_ff_fb_tp_2e7_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/fe_ioneq.png` & `ChiantiPy-0.9.5/docs/source/_static/fe_ioneq.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_spectrum.png` & `ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_spectrum.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_t_ratio.png` & `ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_t_ratio.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/ne6_mg6_t_ratio_top7.png` & `ChiantiPy-0.9.5/docs/source/_static/ne6_mg6_t_ratio_top7.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/radloss.png` & `ChiantiPy-0.9.5/docs/source/_static/radloss.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_10_20.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_10_20.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_1_10.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_1_10.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_3panel.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_3panel.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_integrated.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_integrated.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_200_300_w_si_9.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_200_300_w_si_9.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/spectrum_2e7_1.84_1.90.png` & `ChiantiPy-0.9.5/docs/source/_static/spectrum_2e7_1.84_1.90.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/sphinxdoc.css` & `ChiantiPy-0.9.5/docs/source/_static/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/_static/theme.conf` & `ChiantiPy-0.9.5/docs/source/_static/theme.conf`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.Gui.gui_qt5.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.Gui.gui_qt5.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.base.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.base.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.core.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.core.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.core.tests.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.core.tests.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.fortranformat.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.fortranformat.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/ChiantiPy.tools.rst` & `ChiantiPy-0.9.5/docs/source/api/ChiantiPy.tools.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/api/_static/chiantipy_logo.png` & `ChiantiPy-0.9.5/docs/source/api/_static/chiantipy_logo.png`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/changelog.rst` & `ChiantiPy-0.9.5/docs/source/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 ===========
 Changelog
 ===========
 
+
+Changes from 0.9.4 to 0.9.5
+===========================
+
+this is a bug-fix release.
+
+a bug in the inherited method base._IntensityRatio() had a problem if lines were selected from different ions
+
+
+Changes from 0.9.3 to 0.9.4
+===========================
+
+this is a bug-fix release.
+
+changes in version 0.9.2 continued to give problems with ions that included autoionization rates
+
+
 Changes from 0.9.3 to 0.9.3
 ===========================
 
 this is a bug-fix release.
 
 changes in version 0.9.2 gave problems with ions that included autoionization rates
```

### Comparing `ChiantiPy-0.9.4/docs/source/conf.py` & `ChiantiPy-0.9.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 author = 'Ken Dere'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.9.4'
+version = '0.9.5'
 # The full version, including alpha/beta/rc tags.
-release = '0.9.4'
+release = '0.9.5'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `ChiantiPy-0.9.4/docs/source/getting_started.rst` & `ChiantiPy-0.9.5/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/index.rst` & `ChiantiPy-0.9.5/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
    contain the root `toctree` directive.
 
 ChiantiPy Documentation
 =======================
 
 Welcome to the ChiantiPy documentation. ChiantiPy is a pure Python package for performing calculations of astrophysical spectra using the `CHIANTI atomic database <http://www.chiantidatabase.org/>`_.
 
-The latest version of ChiantiPy is 0.9.4 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions
+The latest version of ChiantiPy is 0.9.5 and is compatible with CHIANTI database version 9.0. It is not compatible with previous versions
 
-ChiantiPy v0.9.4 is released under the OSI approved ISC license. From `Wikipedia <https://en.wikipedia.org/w/index.php?title=ISC_license&oldid=664696993>`_: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, ...
+ChiantiPy v0.9.5 is released under the OSI approved ISC license. From `Wikipedia <https://en.wikipedia.org/w/index.php?title=ISC_license&oldid=664696993>`_: The ISC license is a permissive free software license written by the Internet Software Consortium (ISC). It is functionally equivalent to the simplified BSD and MIT/Expat licenses, ...
 
 `CHIANTI <http://www.chiantidatabase.org/>`_ consists of a database of atomic data that can be used to interpret spectral lines and continua emitted from high-temperature, optically-thin astrophysical sources.
 
 CHIANTI is developed and maintained by scientists at George Mason University (USA), the University of Michigan (USA), and the University of Cambridge (UK). The first version of CHIANTI was released in 1997 and version 9.0 in 2019.
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `ChiantiPy-0.9.4/docs/source/notes.rst` & `ChiantiPy-0.9.5/docs/source/notes.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/quick_start.rst` & `ChiantiPy-0.9.5/docs/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/docs/source/tutorial.rst` & `ChiantiPy-0.9.5/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/jupyter_notebooks/QuickStart.html` & `ChiantiPy-0.9.5/jupyter_notebooks/QuickStart.html`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/jupyter_notebooks/QuickStart.ipynb` & `ChiantiPy-0.9.5/jupyter_notebooks/QuickStart.ipynb`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/licenses/LICENSE` & `ChiantiPy-0.9.5/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/licenses/LICENSE.fortranformat` & `ChiantiPy-0.9.5/licenses/LICENSE.fortranformat`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/setup.cfg` & `ChiantiPy-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ChiantiPy-0.9.4/setup.py` & `ChiantiPy-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.rst", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setup(name = 'ChiantiPy',
     description = 'a Python interface to the CHIANTI atomic database for astrophysical spectroscopy',
     long_description = long_description,
-    version = '0.9.4',
+    version = '0.9.5',
     author = 'Ken Dere',
     author_email = 'kdere@gmu.edu',
     url = 'https://github.com/chianti-atomic/ChiantiPy',
     packages = find_packages(),
     classifiers = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

