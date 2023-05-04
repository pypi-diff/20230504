# Comparing `tmp/reportlab-3.6.9.tar.gz` & `tmp/reportlab-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-3.6.9.tar", last modified: Fri Mar 25 10:55:02 2022, max compression
+gzip compressed data, was "reportlab-4.0.0.tar", last modified: Thu May  4 10:31:54 2023, max compression
```

## Comparing `reportlab-3.6.9.tar` & `reportlab-4.0.0.tar`

### file list

```diff
@@ -1,900 +1,655 @@
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/
--rw-r--r--   0 robin     (1000) robin     (1000)    46400 2022-03-22 08:37:04.000000 reportlab-3.6.9/CHANGES.md
--rw-r--r--   0 robin     (1000) robin     (1000)       53 2019-10-12 07:24:05.000000 reportlab-3.6.9/INSTALL.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.9/LICENSE.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      595 2022-03-02 12:17:05.000000 reportlab-3.6.9/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1052 2022-03-25 10:55:02.782211 reportlab-3.6.9/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     7506 2022-03-02 12:17:05.000000 reportlab-3.6.9/README.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       72 2019-10-12 07:24:05.000000 reportlab-3.6.9/VERSION.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.675542 reportlab-3.6.9/demos/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/colors/
--rw-r--r--   0 robin     (1000) robin     (1000)     2728 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/colors/colortest.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/gadflypaper/
--rw-r--r--   0 robin     (1000) robin     (1000)      105 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/gadflypaper/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    32486 2022-01-24 09:42:51.000000 reportlab-3.6.9/demos/gadflypaper/gfe.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/demos/odyssey/
--rw-r--r--   0 robin     (1000) robin     (1000)     2098 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/odyssey/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     7649 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/odyssey/dodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4580 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/odyssey/fodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4235 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/odyssey/odyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10950 2020-10-29 09:10:51.000000 reportlab-3.6.9/demos/odyssey/odyssey.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/rlzope/
--rw-r--r--   0 robin     (1000) robin     (1000)     2538 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/rlzope/readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     6791 2022-03-02 12:17:05.000000 reportlab-3.6.9/demos/rlzope/rlzope.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/stdfonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/stdfonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     2381 2021-06-01 15:46:32.000000 reportlab-3.6.9/demos/stdfonts/stdfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/demos/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      525 2019-10-12 07:24:05.000000 reportlab-3.6.9/demos/tests/testdemos.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/docs/
--rw-r--r--   0 robin     (1000) robin     (1000)      313 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     3136 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/Makefile
--rwxr-xr-x   0 robin     (1000) robin     (1000)     1497 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/genAll.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)      143 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/gen_epydoc
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.682209 reportlab-3.6.9/docs/images/
--rw-r--r--   0 robin     (1000) robin     (1000)     9685 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Edit_Prefs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    28106 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Python_21.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    29117 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/Python_21_HINT.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    37812 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/fileExchange.gif
--rw-r--r--   0 robin     (1000) robin     (1000)   533144 2021-05-05 14:45:00.000000 reportlab-3.6.9/docs/images/jpegrgb_dissected.png
--rw-r--r--   0 robin     (1000) robin     (1000)    10513 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/jpn.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33898 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/jpnchars.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)      393 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/redsquare.png
--rw-r--r--   0 robin     (1000) robin     (1000)    26548 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/replogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)    16583 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/replogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      924 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/images/testimg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3081 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/make.bat
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/reference/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      110 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/build.bat
--rw-r--r--   0 robin     (1000) robin     (1000)     1206 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/genreference.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9927 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/reference/reference.yml
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/_static/
--rw-r--r--   0 robin     (1000) robin     (1000)      252 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_static/basic.css
--rw-r--r--   0 robin     (1000) robin     (1000)    16419 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_static/default.css
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.685542 reportlab-3.6.9/docs/source/_templates/
--rw-r--r--   0 robin     (1000) robin     (1000)      167 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_templates/layout.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/_templates/page.html
--rw-r--r--   0 robin     (1000) robin     (1000)     6427 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/conf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1345 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/graphics.rst
--rw-r--r--   0 robin     (1000) robin     (1000)     1049 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/index.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      885 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/lib.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      238 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/pdfgen.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      984 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/source/platypus.rst
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/docs/userguide/
--rw-r--r--   0 robin     (1000) robin     (1000)     4494 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/app_demos.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17692 2022-03-02 12:17:05.000000 reportlab-3.6.9/docs/userguide/ch1_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45531 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch2_graphics.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19934 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch2a_fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30547 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch3_pdffeatures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19315 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch4_platypus_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    23044 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch5_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34555 2022-01-24 09:42:51.000000 reportlab-3.6.9/docs/userguide/ch6_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2643 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/ch7_custom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-03-02 12:17:05.000000 reportlab-3.6.9/docs/userguide/genuserguide.py
--rw-r--r--   0 robin     (1000) robin     (1000)    52769 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      490 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12403 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13522 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/graph_widgets.py
--rw-r--r--   0 robin     (1000) robin     (1000)      112 2019-10-12 07:24:05.000000 reportlab-3.6.9/docs/userguide/testfile.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      254 2022-03-25 10:55:02.782211 reportlab-3.6.9/setup.cfg
--rw-r--r--   0 robin     (1000) robin     (1000)    31084 2022-03-22 12:49:38.000000 reportlab-3.6.9/setup.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.678876 reportlab-3.6.9/src/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/src/reportlab/
--rw-r--r--   0 robin     (1000) robin     (1000)      185 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1320 2022-03-22 08:57:03.000000 reportlab-3.6.9/src/reportlab/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.692209 reportlab-3.6.9/src/reportlab/fonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      318 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      504 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-changelog.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    17976 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1318 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     4122 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden-readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)   519634 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGarden.sfd
--rw-r--r--   0 robin     (1000) robin     (1000)    10351 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    79824 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    65932 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/Vera.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63208 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraBI.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    58716 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraBd.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63684 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/VeraIt.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    32084 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_a______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    31966 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ab_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32019 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_abi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32115 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ai_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35377 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_eb_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    38543 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ebi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    37518 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_ei_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35380 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/_er_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)     5954 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/fonts/bitstream-vera-license.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     8318 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/callig15.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    59663 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/callig15.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35500 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/cob_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    50532 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/cobo____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34585 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/com_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    48468 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/coo_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34705 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/sy______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    49593 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zd______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    75573 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zx______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    96418 2022-03-25 10:55:01.000000 reportlab-3.6.9/src/reportlab/fonts/zy______.pfb
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.695542 reportlab-3.6.9/src/reportlab/graphics/
--rw-r--r--   0 robin     (1000) robin     (1000)      274 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.695542 reportlab-3.6.9/src/reportlab/graphics/barcode/
--rw-r--r--   0 robin     (1000) robin     (1000)     1741 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/README
--rw-r--r--   0 robin     (1000) robin     (1000)      915 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/TODO
--rw-r--r--   0 robin     (1000) robin     (1000)     5886 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18451 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code128.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9799 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code39.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9077 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/code93.py
--rw-r--r--   0 robin     (1000) robin     (1000)    23636 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/common.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7872 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/dmtx.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18922 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/eanbc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17884 2020-09-29 08:33:07.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/ecc200datamatrix.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3746 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/fourstate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7377 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/lto.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6266 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/qr.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34117 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/qrencoder.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11516 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/test.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8076 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/usps.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15554 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/usps4s.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17139 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/barcode/widgets.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.698876 reportlab-3.6.9/src/reportlab/graphics/charts/
--rw-r--r--   0 robin     (1000) robin     (1000)      234 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/charts/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4405 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/areas.py
--rw-r--r--   0 robin     (1000) robin     (1000)    91512 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/axes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    72283 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/barcharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6628 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/dotbox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18834 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/doughnut.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25533 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/legends.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27178 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/linecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    49394 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/lineplots.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1739 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    66610 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/piecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8548 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15692 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/spider.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22693 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11556 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7194 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/charts/utils3d.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15155 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPDF.py
--rw-r--r--   0 robin     (1000) robin     (1000)    28772 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPM.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37937 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37686 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12828 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/renderbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.702209 reportlab-3.6.9/src/reportlab/graphics/samples/
--rw-r--r--   0 robin     (1000) robin     (1000)       69 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/samples/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3584 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/bubble.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4241 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/clustered_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4188 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/clustered_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1947 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/excelcolors.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3126 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/exploded_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2691 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/filled_radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4267 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/line_chart.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5007 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/linechart_with_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3244 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1957 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/runall.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3566 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4164 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2933 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/simple_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4284 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/stacked_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4230 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/samples/stacked_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)    59326 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9433 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/testdrawings.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17242 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/testshapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1943 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/transform.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4606 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25552 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgetbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.702209 reportlab-3.6.9/src/reportlab/graphics/widgets/
--rw-r--r--   0 robin     (1000) robin     (1000)      242 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3920 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/adjustableArrow.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13073 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/eventcal.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30233 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/flags.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17504 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8424 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    31655 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/signsandsymbols.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6932 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/graphics/widgets/table.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.705543 reportlab-3.6.9/src/reportlab/lib/
--rw-r--r--   0 robin     (1000) robin     (1000)     4972 2022-01-21 12:16:59.000000 reportlab-3.6.9/src/reportlab/lib/PyFontify.py
--rw-r--r--   0 robin     (1000) robin     (1000)      256 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1122 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/abag.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7272 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/arciv.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5770 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/attrmap.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2927 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/boxstuff.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13051 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/codecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    36654 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27141 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/corp.py
--rw-r--r--   0 robin     (1000) robin     (1000)      296 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/enums.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2226 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/extformat.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13369 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/fontfinder.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3503 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3804 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/formatters.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1163 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1747 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/logger.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22017 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/normalDate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2001 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/pagesizes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30680 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2509 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/pygments2xpre.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22859 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/randomtext.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12606 2022-03-21 15:35:15.000000 reportlab-3.6.9/src/reportlab/lib/rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37051 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1121 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/rltempfile.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17803 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/rparsexml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9647 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/lib/sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16783 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/styles.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12251 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/testutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9723 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/textsplit.py
--rw-r--r--   0 robin     (1000) robin     (1000)      917 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/units.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45361 2022-03-02 12:17:06.000000 reportlab-3.6.9/src/reportlab/lib/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11310 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/lib/validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5717 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/lib/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/reportlab/license.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.708876 reportlab-3.6.9/src/reportlab/pdfbase/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      275 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfbase/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1794 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/_can_cmap_data.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32044 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_cidfontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10141 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2934 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2308 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1829 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_standard.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3187 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2222 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courier.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3367 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3672 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3668 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3665 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3667 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2732 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)   108467 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/pdfbase/_glyphlist.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45680 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/acroform.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18821 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/cidfonts.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    90151 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15704 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfform.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    29935 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3763 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfpattern.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    10135 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    56426 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/pdfbase/rl_codecs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    53122 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfbase/ttfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/reportlab/pdfgen/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      270 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/__init__.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    81667 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/canvas.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5737 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/pathobject.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     2980 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/pdfgen/pdfgeom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8269 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/pdfimages.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    19531 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/pdfgen/textobject.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/reportlab/platypus/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      502 2020-07-24 11:15:51.000000 reportlab-3.6.9/src/reportlab/platypus/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    54601 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/platypus/doctemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18313 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/platypus/figures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    95657 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/flowables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11246 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/frames.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2753 2020-07-24 11:13:36.000000 reportlab-3.6.9/src/reportlab/platypus/multicol.py
--rw-r--r--   0 robin     (1000) robin     (1000)    93001 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/platypus/para.py
--rw-r--r--   0 robin     (1000) robin     (1000)   117624 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/paragraph.py
--rw-r--r--   0 robin     (1000) robin     (1000)   213795 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)    21268 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/tableofcontents.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    80184 2022-03-22 08:49:11.000000 reportlab-3.6.9/src/reportlab/platypus/tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12947 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/platypus/xpreformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4411 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/reportlab/rl_config.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14759 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/reportlab/rl_settings.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.688876 reportlab-3.6.9/src/reportlab.egg-info/
--rw-r--r--   0 robin     (1000) robin     (1000)     1052 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)    35671 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/SOURCES.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/dependency_links.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       44 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/requires.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       10 2022-03-25 10:55:02.000000 reportlab-3.6.9/src/reportlab.egg-info/top_level.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.712209 reportlab-3.6.9/src/rl_addons/
--rw-r--r--   0 robin     (1000) robin     (1000)      326 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/README
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.715543 reportlab-3.6.9/src/rl_addons/renderPM/
--rw-r--r--   0 robin     (1000) robin     (1000)    59470 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/_renderPM.c
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.715543 reportlab-3.6.9/src/rl_addons/renderPM/gt1/
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.c
--rw-r--r--   0 robin     (1000) robin     (1000)      847 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-dict.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1125 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-misc.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6380 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.c
--rw-r--r--   0 robin     (1000) robin     (1000)      796 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-namecontext.h
--rw-r--r--   0 robin     (1000) robin     (1000)    68782 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1115 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-parset1.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2249 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-region.c
--rw-r--r--   0 robin     (1000) robin     (1000)      271 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-region.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1185 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/gt1-value.h
--rw-r--r--   0 robin     (1000) robin     (1000)    45589 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.c
--rw-r--r--   0 robin     (1000) robin     (1000)    11656 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/gt1/parseAFM.h
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.725543 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/
--rw-r--r--   0 robin     (1000) robin     (1000)       27 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/AUTHORS
--rw-r--r--   0 robin     (1000) robin     (1000)    25292 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/COPYING
--rw-r--r--   0 robin     (1000) robin     (1000)    41340 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/ChangeLog
--rw-r--r--   0 robin     (1000) robin     (1000)     3608 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/Makefile.am
--rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/NEWS
--rw-r--r--   0 robin     (1000) robin     (1000)      682 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/README
--rw-r--r--   0 robin     (1000) robin     (1000)      455 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/README.CVS
--rw-r--r--   0 robin     (1000) robin     (1000)       30 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/acconfig.h
--rw-r--r--   0 robin     (1000) robin     (1000)    12103 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2656 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2547 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1424 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_alphagamma.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2470 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1560 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_bpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)      294 2022-03-25 10:55:00.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_config.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2394 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_filterlevel.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3357 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1338 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_gray_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2134 2021-01-17 17:34:27.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.c
--rw-r--r--   0 robin     (1000) robin     (1000)     3078 2020-09-16 15:20:01.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_misc.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1131 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pathcode.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9103 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2937 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_pixbuf.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1110 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_point.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6364 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2303 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2243 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1387 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3927 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1277 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rect_uta.h
--rw-r--r--   0 robin     (1000) robin     (1000)    35686 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.c
--rw-r--r--   0 robin     (1000) robin     (1000)     4702 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render.h
--rw-r--r--   0 robin     (1000) robin     (1000)    19265 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2327 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_gradient.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4190 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1368 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_mask.h
--rw-r--r--   0 robin     (1000) robin     (1000)    10028 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1357 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_render_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4420 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1220 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4548 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1531 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_a_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3647 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1487 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3363 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1209 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_affine_private.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6151 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1578 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_bitmap_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3471 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1570 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_pixbuf_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4451 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1535 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_rgba_affine.h
--rw-r--r--   0 robin     (1000) robin     (1000)    11735 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1581 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgb_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6720 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1391 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_rgba.h
--rw-r--r--   0 robin     (1000) robin     (1000)     4417 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1736 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)    45995 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1925 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_intersect.h
--rw-r--r--   0 robin     (1000) robin     (1000)    11788 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1434 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_ops.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3404 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1305 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_point.h
--rw-r--r--   0 robin     (1000) robin     (1000)    13258 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1935 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_render_aa.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5575 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1282 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)    21659 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1959 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_vpath_stroke.h
--rw-r--r--   0 robin     (1000) robin     (1000)    40901 2021-02-08 17:02:15.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1517 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_svp_wind.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2354 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1926 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3433 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1217 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_ops.h
--rw-r--r--   0 robin     (1000) robin     (1000)     3464 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1225 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_rect.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1636 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1289 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9925 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1454 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_uta_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6178 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1906 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     9617 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1447 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_bpath.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5262 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1372 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_dash.h
--rw-r--r--   0 robin     (1000) robin     (1000)     5064 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1301 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/art_vpath_svp.h
--rw-r--r--   0 robin     (1000) robin     (1000)     1530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/autogen.sh
--rw-r--r--   0 robin     (1000) robin     (1000)      696 2022-01-24 09:42:51.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/config.h
--rw-r--r--   0 robin     (1000) robin     (1000)     2694 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/configure.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1238 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/gen_art_config.c
--rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-2.0.pc.in
--rw-r--r--   0 robin     (1000) robin     (1000)      976 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-config.in
--rw-r--r--   0 robin     (1000) robin     (1000)      366 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-features.c
--rw-r--r--   0 robin     (1000) robin     (1000)      696 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart-features.h.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1351 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.h
--rw-r--r--   0 robin     (1000) robin     (1000)     6262 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libart.m4
--rw-r--r--   0 robin     (1000) robin     (1000)      176 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/libartConf.sh.in
--rw-r--r--   0 robin     (1000) robin     (1000)     8530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/test_gradient.c
--rw-r--r--   0 robin     (1000) robin     (1000)    14315 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testart.c
--rw-r--r--   0 robin     (1000) robin     (1000)     5652 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/libart_lgpl/testuta.c
--rw-r--r--   0 robin     (1000) robin     (1000)    24390 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/pfm.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17530 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/test_renderPM.py
--rw-r--r--   0 robin     (1000) robin     (1000)      587 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/renderPM/tr.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.728876 reportlab-3.6.9/src/rl_addons/rl_accel/
--rw-r--r--   0 robin     (1000) robin     (1000)      469 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/README.extensions
--rw-r--r--   0 robin     (1000) robin     (1000)    39181 2022-03-25 08:39:56.000000 reportlab-3.6.9/src/rl_addons/rl_accel/_rl_accel.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.c
--rw-r--r--   0 robin     (1000) robin     (1000)     1543 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hnjalloc.h
--rw-r--r--   0 robin     (1000) robin     (1000)    13502 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.c
--rw-r--r--   0 robin     (1000) robin     (1000)     2130 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.h
--rw-r--r--   0 robin     (1000) robin     (1000)    36457 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/hyphen.mashed
--rw-r--r--   0 robin     (1000) robin     (1000)     9150 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/pyHnjmodule.c
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.728876 reportlab-3.6.9/src/rl_addons/rl_accel/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      669 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/getrc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1378 2022-03-02 12:17:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t0.py
--rw-r--r--   0 robin     (1000) robin     (1000)      723 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t1.py
--rw-r--r--   0 robin     (1000) robin     (1000)      747 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1875 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1687 2019-10-12 07:24:05.000000 reportlab-3.6.9/src/rl_addons/rl_accel/tests/t5.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.738877 reportlab-3.6.9/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      913 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      540 2021-05-05 14:58:39.000000 reportlab-3.6.9/tests/7x11.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)       99 2021-05-05 14:57:42.000000 reportlab-3.6.9/tests/7x11.png
--rw-r--r--   0 robin     (1000) robin     (1000)       80 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2022-03-25 08:40:21.000000 reportlab-3.6.9/tests/_i_am_actually_a_gif.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2022-03-25 08:40:21.000000 reportlab-3.6.9/tests/_i_am_actually_a_jpeg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3813 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/alpha_test.png
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.742210 reportlab-3.6.9/tests/barcode-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     1091 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Codabar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1458 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1309 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code128.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1457 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Code128Auto.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3014 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN13.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1769 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2385 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/EAN8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3091 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/ECC200DataMatrix.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1562 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Extended39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1906 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Extended93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1080 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/FIM.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1114 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/I2of5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3631 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/ISBN.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1119 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/MSI.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1530 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/POSTNET.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2767 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/QR.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3229 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/QR_with_comma.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1565 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Standard39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1234 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/Standard93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2933 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/UPCA.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1589 2022-03-25 08:40:22.000000 reportlab-3.6.9/tests/barcode-out/USPS_4State.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2388 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2210 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.png
--rw-r--r--   0 robin     (1000) robin     (1000)    12180 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/barcode-out/test_cbcim.tiff
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.768877 reportlab-3.6.9/tests/charts-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     1643 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1506 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1480 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1168 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4004 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3240 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2807 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3742 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2267 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2347 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3630 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2274 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1883 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1846 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2267 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2291 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2332 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3616 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2288 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2277 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2700 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3743 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2681 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3727 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2685 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3734 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2712 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3807 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2756 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2753 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3728 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2734 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3776 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2766 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1724 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1872 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3516 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13857 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6784 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15564 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7126 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15568 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8113 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2619 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3383 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5299 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3071 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4033 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3120 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2287 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2868 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5477 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9274 2022-03-25 08:40:25.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4218 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7323 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4289 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7447 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4952 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9053 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4741 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6406 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3050 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3287 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4149 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2884 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3669 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2807 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3020 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3887 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5378 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3956 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5381 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3464 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5290 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3459 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5291 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3575 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5286 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3389 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5293 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6675 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    48255 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7857 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46272 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3139 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4036 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3029 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3116 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2291 2022-03-25 08:40:26.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5932 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9403 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4468 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7338 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4473 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7450 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5370 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9105 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6379 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3140 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4004 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3206 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4118 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2891 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3654 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2924 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4572 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5412 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4853 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5422 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4426 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5332 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4437 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4602 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4455 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5859 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1492 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6451 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2174 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7297 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7278 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2471 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2843 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2512 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2847 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2080 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2483 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2100 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2508 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3628 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3344 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6052 2022-03-25 08:40:27.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13106 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6759 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    14174 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6782 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    62954 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7754 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41220 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2447 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8150 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5435 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33385 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4772 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10135 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4632 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9133 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6048 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10000 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3585 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7027 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2352 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2420 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4239 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2775 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5724 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3940 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3533 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1272 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4024 2022-03-25 08:40:28.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2052 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6870 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5057 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6126 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5182 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16767 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    23088 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9369 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12584 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10699 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12623 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4504 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7899 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4376 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8690 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4678 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10059 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3914 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3805 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4889 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6410 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6996 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8945 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9425 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8676 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4865 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6067 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8486 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12166 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5283 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6357 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1765 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1182 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4283 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7687 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6776 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5397 2022-03-25 08:40:30.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8883 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4414 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11410 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10045 2022-03-25 08:40:29.000000 reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2979 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/encryption.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1908 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/gray-alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/pythonpowered-gs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/pythonpowered.gif
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tests/render-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     2589 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/410.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1362 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/410.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3229 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5106 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2850 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1020 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing01.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2560 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5750 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2739 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.png
--rw-r--r--   0 robin     (1000) robin     (1000)      846 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing02.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8923 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8747 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    14798 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1327 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing03.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2369 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2785 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2765 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.png
--rw-r--r--   0 robin     (1000) robin     (1000)      858 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing04.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3163 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3729 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4721 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1393 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing05.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6353 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10726 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12964 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing06.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3929 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5433 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     7028 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.png
--rw-r--r--   0 robin     (1000) robin     (1000)     8298 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing07.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3428 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6355 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4097 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.png
--rw-r--r--   0 robin     (1000) robin     (1000)    10846 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing08.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7990 2022-03-25 08:40:23.000000 reportlab-3.6.9/tests/render-out/Drawing09.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8280 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    15924 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1339 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing09.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3154 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5783 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2910 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2163 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing10.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2189 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2915 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     3105 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7969 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing11.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17038 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    16031 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    28701 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1219 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing12.py
--rw-r--r--   0 robin     (1000) robin     (1000)    40966 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    51523 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    72941 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.png
--rw-r--r--   0 robin     (1000) robin     (1000)     4246 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing13.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1374 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2183 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)      882 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1064 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/Drawing14.py
--rw-r--r--   0 robin     (1000) robin     (1000)      342 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-none.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1011 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-none.py
--rw-r--r--   0 robin     (1000) robin     (1000)      336 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-pdf.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)      352 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-svg.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/autoclose-svg.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11577 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-even-odd.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-even-odd.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11621 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-non-zero.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/fillmode-non-zero.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14199 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/hatch.png
--rw-r--r--   0 robin     (1000) robin     (1000)     6477 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/hatch.py
--rw-r--r--   0 robin     (1000) robin     (1000)      879 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/svglib-issue104.png
--rw-r--r--   0 robin     (1000) robin     (1000)    24350 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/textmode.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2027 2022-03-25 08:40:24.000000 reportlab-3.6.9/tests/render-out/textmode.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6504 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/rltw-icon-tr.png
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5209 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/runAll.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2402 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/solid_red_alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/tall_red.png
--rw-r--r--   0 robin     (1000) robin     (1000)      288 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-cross.tiff
--rw-r--r--   0 robin     (1000) robin     (1000)      168 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-indexed.png
--rw-r--r--   0 robin     (1000) robin     (1000)      157 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test-rgba.png
--rw-r--r--   0 robin     (1000) robin     (1000)     9464 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_charts_textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6252 2019-11-23 12:29:07.000000 reportlab-3.6.9/tests/test_crypto_algorithms.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1462 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_docs_build.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6506 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_docstrings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_extra.py
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14652 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_barcode.py
--rw-r--r--   0 robin     (1000) robin     (1000)    41317 2022-02-03 15:17:16.000000 reportlab-3.6.9/tests/test_graphics_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32774 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images-cairo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46849 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images-cairo.png
--rw-r--r--   0 robin     (1000) robin     (1000)    16209 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    21349 2022-03-25 08:40:40.000000 reportlab-3.6.9/tests/test_graphics_images.png
--rw-r--r--   0 robin     (1000) robin     (1000)     3766 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2523 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_graphics_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15789 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_graphics_render.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2628 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_graphics_speed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1893 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_hello.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2662 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2511 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_invariant.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4214 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_issues.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8276 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_lib_colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11916 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_normaldate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6062 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6780 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_lib_rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3748 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_lib_sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13278 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_lib_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5592 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_lib_validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2448 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_chs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4973 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_cht.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25468 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_multibyte_jpn.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6658 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_multibyte_kor.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34098 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10715 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_encodings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3875 2020-01-26 19:46:34.000000 reportlab-3.6.9/tests/test_pdfbase_fontembed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2713 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18606 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfform.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4120 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1609 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_pdfbase_pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfbase_postscript.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19727 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pdfbase_ttfonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      989 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_callback.py
--rw-r--r--   0 robin     (1000) robin     (1000)    48259 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pdfgen_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6925 2021-07-06 13:47:00.000000 reportlab-3.6.9/tests/test_pdfgen_links.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3133 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_overprint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1850 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_pdfgen_pagemodes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3168 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_platypus_accum.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27202 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_breaking.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5973 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_cjk_wrap.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34433 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4226 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8549 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_indents.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5383 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_platypus_index.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6293 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_leftright.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10786 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_lists.py
--rw-r--r--   0 robin     (1000) robin     (1000)   113010 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5094 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_platypus_paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9402 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_pleaseturnover.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8635 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_preformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7373 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_programming.py
--rw-r--r--   0 robin     (1000) robin     (1000)    53423 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12590 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_toc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3773 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_wrapping.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5183 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_platypus_xref.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4762 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_pyfiles.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7690 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9773 2022-03-02 12:17:05.000000 reportlab-3.6.9/tests/test_renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10617 2022-03-24 13:23:54.000000 reportlab-3.6.9/tests/test_rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3423 2022-01-24 09:42:51.000000 reportlab-3.6.9/tests/test_source_chars.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19261 2022-03-22 08:49:11.000000 reportlab-3.6.9/tests/test_table_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1244 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_tools_pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1353 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4890 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_widgetbase_tpc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15476 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/test_widgets_grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.9/tests/unimportable.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/
--rw-r--r--   0 robin     (1000) robin     (1000)      193 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/README
--rw-r--r--   0 robin     (1000) robin     (1000)      160 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/docco/
--rw-r--r--   0 robin     (1000) robin     (1000)      292 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/README
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7791 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/codegrab.py
--rw-r--r--   0 robin     (1000) robin     (1000)    41170 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/docpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    29268 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/docco/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32661 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/graphdocpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13738 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/rl_doc_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5898 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/rltemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6939 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/stylesheet.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9899 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/t_parse.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7023 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3284 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/docco/yaml2pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1056 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pdfpath.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.778877 reportlab-3.6.9/tools/pythonpoint/
--rw-r--r--   0 robin     (1000) robin     (1000)     1099 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/README
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8840 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/customshapes.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/pythonpoint/demos/
--rw-r--r--   0 robin     (1000) robin     (1000)    26656 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/figures.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     4859 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/htu.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     3008 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)     2198 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    11730 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/monterey.xml
--rw-r--r--   0 robin     (1000) robin     (1000)    12918 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/outline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3429 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/pplogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)   125666 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/python.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41307 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/pythonpoint.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     1704 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1855 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/spectrum.png
--rw-r--r--   0 robin     (1000) robin     (1000)    20910 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/demos/vertpython.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7920 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/pythonpoint.dtd
--rw-r--r--   0 robin     (1000) robin     (1000)    34726 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)    28933 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/stdparser.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/pythonpoint/styles/
--rw-r--r--   0 robin     (1000) robin     (1000)      179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/horrible.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5079 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/htu.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3692 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/modern.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3215 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/projection.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/pythonpoint/styles/standard.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2022-03-25 10:55:02.782211 reportlab-3.6.9/tools/utils/
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2022-03-02 12:17:05.000000 reportlab-3.6.9/tools/utils/add_bleed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1891 2019-10-12 07:24:05.000000 reportlab-3.6.9/tools/utils/dumpttf.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.197729 reportlab-4.0.0/
+-rw-rw-r--   0 andy      (1000) andy      (1000)    48584 2023-05-04 09:53:56.000000 reportlab-4.0.0/CHANGES.md
+-rw-rw-r--   0 andy      (1000) andy      (1000)       53 2023-03-07 11:06:02.000000 reportlab-4.0.0/INSTALL.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1707 2023-05-04 09:52:31.000000 reportlab-4.0.0/LICENSE
+-rw-rw-r--   0 andy      (1000) andy      (1000)      468 2023-05-04 09:52:31.000000 reportlab-4.0.0/MANIFEST.in
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1055 2023-05-04 10:31:54.197729 reportlab-4.0.0/PKG-INFO
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4994 2023-05-04 09:52:31.000000 reportlab-4.0.0/README.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       72 2023-03-07 11:06:02.000000 reportlab-4.0.0/VERSION.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.021736 reportlab-4.0.0/demos/
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.025735 reportlab-4.0.0/demos/colors/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2728 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/colors/colortest.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.025735 reportlab-4.0.0/demos/gadflypaper/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      105 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/gadflypaper/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32486 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/gadflypaper/gfe.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.029735 reportlab-4.0.0/demos/odyssey/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2098 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/odyssey/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7649 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/odyssey/dodyssey.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4580 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/odyssey/fodyssey.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4235 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/odyssey/odyssey.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10950 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/odyssey/odyssey.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.029735 reportlab-4.0.0/demos/rlzope/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2538 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/rlzope/readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6791 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/rlzope/rlzope.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.029735 reportlab-4.0.0/demos/stdfonts/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      229 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/stdfonts/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2381 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/stdfonts/stdfonts.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.029735 reportlab-4.0.0/demos/tests/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      525 2023-03-07 11:06:02.000000 reportlab-4.0.0/demos/tests/testdemos.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.029735 reportlab-4.0.0/docs/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      313 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3136 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/Makefile
+-rwxrwxr-x   0 andy      (1000) andy      (1000)     1497 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/genAll.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)      143 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/gen_epydoc
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.033735 reportlab-4.0.0/docs/images/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9685 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/Edit_Prefs.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    28106 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/Python_21.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    29117 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/Python_21_HINT.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    37812 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/fileExchange.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10513 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/jpn.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    33898 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/jpnchars.jpg
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12463 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/lj8100.jpg
+-rw-rw-r--   0 andy      (1000) andy      (1000)      393 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/redsquare.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)    26548 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/replogo.a85
+-rw-rw-r--   0 andy      (1000) andy      (1000)    16583 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/replogo.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)      924 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/images/testimg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3081 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/make.bat
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.037735 reportlab-4.0.0/docs/reference/
+-rwxrwxr-x   0 andy      (1000) andy      (1000)      110 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/reference/build.bat
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1206 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/reference/genreference.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9927 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/reference/reference.yml
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.037735 reportlab-4.0.0/docs/source/
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.037735 reportlab-4.0.0/docs/source/_static/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      252 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/_static/basic.css
+-rw-rw-r--   0 andy      (1000) andy      (1000)    16419 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/_static/default.css
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.037735 reportlab-4.0.0/docs/source/_templates/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      167 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/_templates/layout.html
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1431 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/_templates/page.html
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6427 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/conf.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1345 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/graphics.rst
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1049 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/index.rst
+-rw-rw-r--   0 andy      (1000) andy      (1000)      885 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/lib.rst
+-rw-rw-r--   0 andy      (1000) andy      (1000)      238 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/pdfgen.rst
+-rw-rw-r--   0 andy      (1000) andy      (1000)      984 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/source/platypus.rst
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.045735 reportlab-4.0.0/docs/userguide/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4494 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/app_demos.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17692 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch1_intro.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    45531 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch2_graphics.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    19934 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch2a_fonts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    30547 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch3_pdffeatures.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    19314 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch4_platypus_concepts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    23044 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch5_paragraphs.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34555 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch6_tables.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2643 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/ch7_custom.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3575 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/genuserguide.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    52769 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/graph_charts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11788 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/graph_concepts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      490 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/graph_intro.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12403 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/graph_shapes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13522 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/graph_widgets.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      112 2023-03-07 11:06:02.000000 reportlab-4.0.0/docs/userguide/testfile.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       89 2023-05-04 09:52:31.000000 reportlab-4.0.0/pyproject.toml
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-05-04 10:31:54.197729 reportlab-4.0.0/setup.cfg
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11833 2023-05-04 09:54:37.000000 reportlab-4.0.0/setup.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.021736 reportlab-4.0.0/src/
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.045735 reportlab-4.0.0/src/reportlab/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      185 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/MANIFEST.in
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1320 2023-05-04 09:55:26.000000 reportlab-4.0.0/src/reportlab/__init__.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.057734 reportlab-4.0.0/src/reportlab/fonts/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      318 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)      504 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGarden-changelog.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17976 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGarden-copying-gpl.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1318 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGarden-copying.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4122 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGarden-readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)   519634 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGarden.sfd
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10351 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGardenMK.afm
+-rw-rw-r--   0 andy      (1000) andy      (1000)    79824 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/DarkGardenMK.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    65932 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/Vera.ttf
+-rw-rw-r--   0 andy      (1000) andy      (1000)    63208 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/VeraBI.ttf
+-rw-rw-r--   0 andy      (1000) andy      (1000)    58716 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/VeraBd.ttf
+-rw-rw-r--   0 andy      (1000) andy      (1000)    63684 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/VeraIt.ttf
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32084 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_a______.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    31966 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_ab_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32019 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_abi____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32115 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_ai_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    35377 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_eb_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    38543 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_ebi____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    37518 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_ei_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    35380 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/_er_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5954 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/fonts/bitstream-vera-license.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8318 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/callig15.afm
+-rw-rw-r--   0 andy      (1000) andy      (1000)    59663 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/callig15.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    35500 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/cob_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    50532 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/cobo____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34585 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/com_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    48468 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/coo_____.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34705 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/sy______.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    49593 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/zd______.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    75573 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/zx______.pfb
+-rw-rw-r--   0 andy      (1000) andy      (1000)    96418 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab/fonts/zy______.pfb
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.061734 reportlab-4.0.0/src/reportlab/graphics/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      274 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/__init__.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.069733 reportlab-4.0.0/src/reportlab/graphics/barcode/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1741 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/README
+-rw-rw-r--   0 andy      (1000) andy      (1000)      915 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/TODO
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5886 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18451 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/code128.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9799 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/code39.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9077 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/code93.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    24345 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/common.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7872 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/dmtx.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18922 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/eanbc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17884 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/ecc200datamatrix.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3746 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/fourstate.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7377 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/lto.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6266 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/qr.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34117 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/qrencoder.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11765 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/test.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8076 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/usps.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15554 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/usps4s.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17499 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/barcode/widgets.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.073733 reportlab-4.0.0/src/reportlab/graphics/charts/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      234 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4405 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/areas.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    91512 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/axes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    72283 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/barcharts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6628 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/dotbox.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18834 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/doughnut.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    25533 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/legends.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    27178 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/linecharts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    49394 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/lineplots.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1739 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/markers.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    66610 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/piecharts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8548 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/slidebox.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15692 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/spider.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    22693 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/textlabels.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11556 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7194 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/charts/utils3d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15155 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/renderPDF.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    29010 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/graphics/renderPM.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    37937 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/renderPS.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    37686 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/renderSVG.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12828 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/renderbase.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.081733 reportlab-4.0.0/src/reportlab/graphics/samples/
+-rw-rw-r--   0 andy      (1000) andy      (1000)       69 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3584 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/bubble.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4241 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/clustered_bar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4188 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/clustered_column.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1947 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/excelcolors.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3126 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/exploded_pie.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2691 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/filled_radar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4267 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/line_chart.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5007 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/linechart_with_markers.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3244 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/radar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1957 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/runall.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3566 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/scatter.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4164 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/scatter_lines.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3766 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/scatter_lines_markers.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2933 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/simple_pie.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4284 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/stacked_bar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4230 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/samples/stacked_column.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    59326 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/shapes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9433 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/testdrawings.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17237 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/testshapes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1956 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/transform.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12499 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/graphics/utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    25552 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgetbase.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.081733 reportlab-4.0.0/src/reportlab/graphics/widgets/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      242 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3920 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/adjustableArrow.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13073 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/eventcal.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    30233 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/flags.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    17504 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/grids.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8424 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/markers.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    31655 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/signsandsymbols.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6932 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/graphics/widgets/table.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.089733 reportlab-4.0.0/src/reportlab/lib/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4972 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/PyFontify.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      256 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1122 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/abag.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7272 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/arciv.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5770 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/attrmap.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2927 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/boxstuff.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13051 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/lib/codecharts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    39074 2023-05-04 09:52:42.000000 reportlab-4.0.0/src/reportlab/lib/colors.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    27141 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/corp.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      296 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/enums.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2226 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/extformat.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13369 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/fontfinder.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3503 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/fonts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3804 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/formatters.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1163 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/geomutils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1747 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/logger.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    22017 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/normalDate.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2001 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/pagesizes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    30699 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/pdfencrypt.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2509 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/pygments2xpre.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    22859 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/randomtext.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12592 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/lib/rl_accel.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    39558 2023-05-04 09:52:42.000000 reportlab-4.0.0/src/reportlab/lib/rl_safe_eval.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1121 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/rltempfile.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18422 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/rparsexml.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9647 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/sequencer.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    16783 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/styles.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12251 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/testutils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9723 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/textsplit.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      917 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/units.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    43246 2023-05-04 08:37:21.000000 reportlab-4.0.0/src/reportlab/lib/utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11310 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/validators.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5717 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/lib/yaml.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.101732 reportlab-4.0.0/src/reportlab/pdfbase/
+-rwxrwxr-x   0 andy      (1000) andy      (1000)      275 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1794 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_can_cmap_data.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32044 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_cidfontdata.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10141 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3058 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2934 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_macroman.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2308 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1829 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_standard.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3187 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_symbol.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3003 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_winansi.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2222 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3664 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courier.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3664 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3664 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3664 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3671 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3670 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3670 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3671 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3367 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_symbol.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3672 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3668 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3665 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3667 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2732 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)   108467 2023-03-07 11:46:17.000000 reportlab-4.0.0/src/reportlab/pdfbase/_glyphlist.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    45680 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/acroform.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18768 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/cidfonts.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)    90182 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/pdfbase/pdfdoc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15704 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/pdfform.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)    29935 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/pdfmetrics.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3763 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/pdfpattern.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)    10135 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/pdfutils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    56426 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/rl_codecs.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    53122 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfbase/ttfonts.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.101732 reportlab-4.0.0/src/reportlab/pdfgen/
+-rwxrwxr-x   0 andy      (1000) andy      (1000)      270 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfgen/__init__.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)    82046 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/pdfgen/canvas.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)     5737 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfgen/pathobject.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)     2980 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfgen/pdfgeom.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8422 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/pdfgen/pdfimages.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)    19531 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/pdfgen/textobject.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.105732 reportlab-4.0.0/src/reportlab/platypus/
+-rwxrwxr-x   0 andy      (1000) andy      (1000)      502 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    54690 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/doctemplate.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18313 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/figures.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    95757 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/platypus/flowables.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11246 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/frames.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2753 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/multicol.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    93001 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/para.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)   117624 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/paragraph.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)   213795 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/paraparser.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    21268 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/tableofcontents.py
+-rwxrwxr-x   0 andy      (1000) andy      (1000)   112658 2023-05-04 09:57:28.000000 reportlab-4.0.0/src/reportlab/platypus/tables.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12947 2023-03-07 11:06:02.000000 reportlab-4.0.0/src/reportlab/platypus/xpreformatted.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4930 2023-05-04 09:52:31.000000 reportlab-4.0.0/src/reportlab/rl_config.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    14802 2023-05-04 09:52:42.000000 reportlab-4.0.0/src/reportlab/rl_settings.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.049734 reportlab-4.0.0/src/reportlab.egg-info/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1055 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab.egg-info/PKG-INFO
+-rw-rw-r--   0 andy      (1000) andy      (1000)    26142 2023-05-04 10:31:54.000000 reportlab-4.0.0/src/reportlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)      130 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab.egg-info/requires.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       10 2023-05-04 10:31:53.000000 reportlab-4.0.0/src/reportlab.egg-info/top_level.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.129731 reportlab-4.0.0/tests/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      913 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/00readme.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       80 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1077 2023-05-04 09:13:02.000000 reportlab-4.0.0/tests/_i_am_actually_a_gif.jpg
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12463 2023-05-04 09:13:02.000000 reportlab-4.0.0/tests/_i_am_actually_a_jpeg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3813 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/alpha_test.png
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.185729 reportlab-4.0.0/tests/charts-out/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1644 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1506 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1094 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1168 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4004 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3240 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2789 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3742 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2261 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3552 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2333 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3630 2023-05-04 09:09:45.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2272 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3546 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1876 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1846 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2269 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3560 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2281 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3552 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2314 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3616 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2294 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3560 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2272 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3546 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2681 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3743 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2674 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3727 2023-05-04 09:09:46.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2681 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3734 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2714 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3807 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2763 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3744 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2758 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3728 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2730 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3776 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2760 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3744 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1336 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7542 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1473 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7542 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3533 2023-05-04 09:09:47.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13857 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6765 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15564 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7070 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15568 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7526 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2619 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample_hatching.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3374 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5299 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3053 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4033 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2873 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3120 2023-05-04 09:09:48.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1889 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2868 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5422 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9274 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4179 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7323 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4250 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7447 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4902 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9053 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4754 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6406 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3043 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4003 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3256 2023-05-04 09:09:49.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4149 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2884 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3669 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2807 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3020 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3880 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5378 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3929 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5381 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3440 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5290 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3443 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5291 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3557 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5286 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3374 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5293 2023-05-04 09:09:50.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6746 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    48255 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7900 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    46272 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3121 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4036 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3023 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3116 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2278 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2886 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5870 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9403 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4426 2023-05-04 09:09:51.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7338 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4441 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7450 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5323 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9105 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4561 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6379 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3134 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4004 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3206 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4118 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2884 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3654 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2900 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3003 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4468 2023-05-04 09:09:52.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5412 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4780 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5422 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4408 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5332 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4426 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5333 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4579 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5333 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4444 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5333 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5913 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1492 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6454 2023-05-04 09:09:53.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2174 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7275 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4062 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7275 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample4.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4062 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample4.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2473 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample1c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2843 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample1c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2509 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample2c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2847 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample2c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2078 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2483 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2096 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2508 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3599 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample4a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3344 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample4a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6096 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13106 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6805 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    14174 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6839 2023-05-04 09:09:54.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    62954 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7830 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    41220 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2026 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8150 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5337 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    33385 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4702 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10135 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4572 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9133 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1c.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5909 2023-05-04 09:09:55.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10000 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3576 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7027 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2509 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)      841 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0a.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2586 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)      841 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0b.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4233 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2775 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5670 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3940 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3440 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1272 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3899 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample4.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2052 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample4.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6790 2023-05-04 09:09:56.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample5.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5057 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample5.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5997 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample6.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5182 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample6.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    16677 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample7.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    23088 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample7.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9327 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample8.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12584 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample8.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10679 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample9.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12623 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample9.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4522 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_bcleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7899 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_bcleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4414 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_hlcleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8690 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_hlcleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4681 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_lpleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10059 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_lpleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3956 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_pcleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3805 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_pcleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4985 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_plpleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6410 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_plpleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7147 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1bar.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8888 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1bar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9287 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1barline.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8676 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1barline.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4907 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1line.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6067 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1line.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8790 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2bar.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12069 2023-05-04 09:09:59.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2bar.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5362 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2line.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6357 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2line.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1766 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample3.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1182 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample3.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4272 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample4pie.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7677 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample4pie.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6644 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_scleg.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5397 2023-05-04 09:10:00.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_scleg.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8850 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample1.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4414 2023-05-04 09:09:57.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample1.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11209 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample2.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10045 2023-05-04 09:09:58.000000 reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample2.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2979 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/encryption.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1908 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/gray-alpha.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1894 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/pythonpowered-gs.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1077 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/pythonpowered.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6504 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/rltw-icon-tr.png
+-rwxrwxr-x   0 andy      (1000) andy      (1000)     5570 2023-05-04 09:52:42.000000 reportlab-4.0.0/tests/runAll.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2402 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/solid_red_alpha.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)      172 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/tall_red.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)      288 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test-cross.tiff
+-rw-rw-r--   0 andy      (1000) andy      (1000)      168 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test-indexed.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)      157 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test-rgba.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9464 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_charts_textlabels.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6252 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_crypto_algorithms.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1462 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_docs_build.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6506 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_docstrings.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3058 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_extra.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      954 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_geomutils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    14648 2023-05-04 09:52:31.000000 reportlab-4.0.0/tests/test_graphics_barcode.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    41435 2023-05-04 09:52:42.000000 reportlab-4.0.0/tests/test_graphics_charts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32774 2023-05-04 09:09:39.000000 reportlab-4.0.0/tests/test_graphics_images.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    46849 2023-05-04 09:09:39.000000 reportlab-4.0.0/tests/test_graphics_images.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3832 2023-05-04 09:52:31.000000 reportlab-4.0.0/tests/test_graphics_images.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2523 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_graphics_layout.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15782 2023-05-04 09:52:31.000000 reportlab-4.0.0/tests/test_graphics_render.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2628 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_graphics_speed.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1893 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_hello.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2609 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_images.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2530 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_invariant.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4214 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_issues.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8276 2023-05-04 09:52:31.000000 reportlab-4.0.0/tests/test_lib_colors.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11916 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_lib_normaldate.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6062 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_lib_pdfencrypt.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9595 2023-05-04 09:52:42.000000 reportlab-4.0.0/tests/test_lib_rl_safe_eval.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3748 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_lib_sequencer.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13279 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_lib_utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5592 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_lib_validators.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2448 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_multibyte_chs.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4973 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_multibyte_cht.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    25468 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_multibyte_jpn.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6658 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_multibyte_kor.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34098 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_paragraphs.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10715 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_encodings.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3875 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_fontembed.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2713 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_pdfdoc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    18606 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_pdfform.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4120 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_pdfmetrics.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1609 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_pdfutils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3179 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_postscript.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    19727 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfbase_ttfonts.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      989 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfgen_callback.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    47316 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfgen_general.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6925 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfgen_links.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3133 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfgen_overprint.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1850 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pdfgen_pagemodes.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3168 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_accum.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    27202 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_breaking.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5973 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_cjk_wrap.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34369 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_general.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4149 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_images.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8549 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_indents.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5383 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_index.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6293 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_leftright.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10786 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_lists.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)   113010 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_paragraphs.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5094 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_paraparser.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9402 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_pleaseturnover.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8635 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_preformatted.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7373 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_programming.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    53423 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_tables.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13445 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_toc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3773 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_wrapping.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5183 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_platypus_xref.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4762 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_pyfiles.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7690 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_renderPS.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9773 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_renderSVG.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    10617 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_rl_accel.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3423 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_source_chars.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    16158 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_table_inrowsplit.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34217 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_table_layout.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1244 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_tools_pythonpoint.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1353 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4890 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_widgetbase_tpc.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    15476 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/test_widgets_grids.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)      166 2023-03-07 11:06:02.000000 reportlab-4.0.0/tests/unimportable.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.185729 reportlab-4.0.0/tools/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      193 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/README
+-rw-rw-r--   0 andy      (1000) andy      (1000)      160 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/__init__.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.189729 reportlab-4.0.0/tools/docco/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      292 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/README
+-rw-rw-r--   0 andy      (1000) andy      (1000)      166 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7791 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/codegrab.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    41170 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/docpy.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    29268 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/examples.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    32661 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/graphdocpy.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    13738 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/rl_doc_utils.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5898 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/rltemplate.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6939 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/stylesheet.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     9899 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/t_parse.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7023 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/yaml.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3284 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/docco/yaml2pdf.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1056 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pdfpath.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.189729 reportlab-4.0.0/tools/pythonpoint/
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1099 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/README
+-rw-rw-r--   0 andy      (1000) andy      (1000)      172 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     8840 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/customshapes.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.193729 reportlab-4.0.0/tools/pythonpoint/demos/
+-rw-rw-r--   0 andy      (1000) andy      (1000)    26616 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/examples.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3670 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/figures.xml
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4859 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/htu.xml
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3008 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/leftlogo.a85
+-rw-rw-r--   0 andy      (1000) andy      (1000)     2198 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/leftlogo.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12463 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/lj8100.jpg
+-rw-rw-r--   0 andy      (1000) andy      (1000)    11730 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/monterey.xml
+-rw-rw-r--   0 andy      (1000) andy      (1000)    12918 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/outline.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3429 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/pplogo.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)   125666 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/python.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)    41307 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/pythonpoint.xml
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1704 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/slidebox.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1855 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/spectrum.png
+-rw-rw-r--   0 andy      (1000) andy      (1000)    20910 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/demos/vertpython.gif
+-rw-rw-r--   0 andy      (1000) andy      (1000)     7920 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/pythonpoint.dtd
+-rw-rw-r--   0 andy      (1000) andy      (1000)    34726 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/pythonpoint.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)    28933 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/stdparser.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.193729 reportlab-4.0.0/tools/pythonpoint/styles/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      179 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/__init__.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3179 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/horrible.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     5079 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/htu.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3692 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/modern.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     3215 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/projection.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     4003 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/pythonpoint/styles/standard.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-05-04 10:31:54.197729 reportlab-4.0.0/tools/utils/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      954 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/utils/add_bleed.py
+-rw-rw-r--   0 andy      (1000) andy      (1000)     1891 2023-03-07 11:06:02.000000 reportlab-4.0.0/tools/utils/dumpttf.py
```

### Comparing `reportlab-3.6.9/CHANGES.md` & `reportlab-4.0.0/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,61 @@
 E.g. to retrieve the changes made between release 3.4 and release 3.5, type::
 
   $ hg log -r 54ce2469ba5c
 
 The contributors lists are in no order and apologies to those accidentally not
 mentioned. If we missed you, please let us know!
 
+CHANGES  4.0.0a3 18/04/2023
+---------------------------
+	* initial support for rml ul ol dl tagging
+    * added support for an ol/ul/dl caption paragraph
+	* implement a safer toColor with rl_config.toColorCanUse option and rl_extended_literal_eval
+
+CHANGES  4.0.0a2 14/03/2023
+---------------------------
+	* added _ExpandedCellTupleEx for more tagging support
+
+CHANGES  4.0.0a1 08/03/2023
+---------------------------
+	* release 4.0.0a1 with support for rlextra pluscode
+
+CHANGES  3.6.13  24/04/2023
+---------------------------
+	* fixes for python 3.12.0a1
+	* tables.py error improvement
+	* allow exclusions in tests in runAll.py and setup.py; allows for coverage.py importing failures.
+	* implement a safer toColor with rl_config.toColorCanUse option and rl_extended_literal_eval
+
+CHANGES  3.6.12  25/10/2022
+---------------------------
+	* fix dpi handling in renderPM.py; bug found by Terry Zhao Terry dot Zhao at fil dot com
+	* attempt fix in rparsexml.py
+	* add rl_settings.xmlParser with default 'lxml'
+	* nano RHEL related fix to setup.py contributed by James Brown jbrown at easypost dot com
+	* minor speedup in reportlab.graphics.transform functions
+	* allow usage of freetype testpaths via rl_config/rl_settings textPaths
+	* _renderPM.c remove parse_utf8, make pict_putrow same as for rlPyCairo
+
+CHANGES  3.6.11  24/06/2022
+---------------------------
+	* support HORIZONTAL2 & VERTICAL2 table cell backgrounds; as suggested by Sina Khelil < sina at khelil dot com >
+	* support general LINEAR & RADIAL gradient table cell backgrounds
+	* support ShowBoundaryValue in canv.drawImage
+
+CHANGES  3.6.10  31/05/2022
+---------------------------
+	* fix symlink looping in setup.py reported by Michał Górny &lt; mgorny at gentoo dot org &gt;
+	* allow bearerBox attribute for some barcodes
+	* require pillow>=9.0.0 patch contributed by Claude Paroz claude at 2xlibre.net
+	* Apply Claude Paroz  < claude at 2xlibre dot net > patch to assume hashlib md5 exists
+	* ImageReader updated to allow deepcopy; similarly for doctemplate.onDrawStr
+	* fix 3.11.0b2 regression in rl_safe_eval.
+	* apply massive contribution for Table inRowSplit from Lennart Regebro < lregebro at shoobx dot com >
+
 CHANGES  3.6.9   22/03/2022
 ---------------------------
 	* fix up _rl_accel.c 0.81 to allow better error messages and support python 3.11.0a6
 	* change the cibuildwheel setup to support macos M1 build
 
 CHANGES  3.6.8   28/02/2022
 ---------------------------
```

### Comparing `reportlab-3.6.9/LICENSE.txt` & `reportlab-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/PKG-INFO` & `reportlab-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 3.6.9
+Version: 4.0.0
 Summary: The Reportlab Toolkit
 Home-page: http://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
-License: BSD license (see license.txt for details), Copyright (c) 2000-2018, ReportLab Inc.
-Platform: UNKNOWN
+License: BSD license (see license.txt for details), Copyright (c) 2000-2022, ReportLab Inc.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Printing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7, <4
-Provides-Extra: RLPYCAIRO
-License-File: LICENSE.txt
+Requires-Python: >=3.7,<4
+Provides-Extra: RL_ACCEL
+Provides-Extra: RL_RENDERPM
+License-File: LICENSE
 
 The ReportLab Toolkit. An Open Source Python library for generating PDFs and graphics.
-
```

### Comparing `reportlab-3.6.9/demos/colors/colortest.py` & `reportlab-4.0.0/demos/colors/colortest.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/gadflypaper/gfe.py` & `reportlab-4.0.0/demos/gadflypaper/gfe.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/odyssey/00readme.txt` & `reportlab-4.0.0/demos/odyssey/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/odyssey/dodyssey.py` & `reportlab-4.0.0/demos/odyssey/dodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/odyssey/fodyssey.py` & `reportlab-4.0.0/demos/odyssey/fodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/odyssey/odyssey.py` & `reportlab-4.0.0/demos/odyssey/odyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/odyssey/odyssey.txt` & `reportlab-4.0.0/demos/odyssey/odyssey.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/rlzope/readme.txt` & `reportlab-4.0.0/demos/rlzope/readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/rlzope/rlzope.py` & `reportlab-4.0.0/demos/rlzope/rlzope.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/stdfonts/stdfonts.py` & `reportlab-4.0.0/demos/stdfonts/stdfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/demos/tests/testdemos.py` & `reportlab-4.0.0/demos/tests/testdemos.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/Makefile` & `reportlab-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/genAll.py` & `reportlab-4.0.0/docs/genAll.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/Edit_Prefs.gif` & `reportlab-4.0.0/docs/images/Edit_Prefs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/Python_21.gif` & `reportlab-4.0.0/docs/images/Python_21.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/Python_21_HINT.gif` & `reportlab-4.0.0/docs/images/Python_21_HINT.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/fileExchange.gif` & `reportlab-4.0.0/docs/images/fileExchange.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/jpn.gif` & `reportlab-4.0.0/docs/images/jpn.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/jpnchars.jpg` & `reportlab-4.0.0/docs/images/jpnchars.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/lj8100.jpg` & `reportlab-4.0.0/docs/images/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/replogo.a85` & `reportlab-4.0.0/docs/images/replogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/replogo.gif` & `reportlab-4.0.0/docs/images/replogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/images/testimg.gif` & `reportlab-4.0.0/docs/images/testimg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/make.bat` & `reportlab-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/reference/genreference.py` & `reportlab-4.0.0/docs/reference/genreference.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/reference/reference.yml` & `reportlab-4.0.0/docs/reference/reference.yml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/_static/default.css` & `reportlab-4.0.0/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/_templates/page.html` & `reportlab-4.0.0/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/conf.py` & `reportlab-4.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/graphics.rst` & `reportlab-4.0.0/docs/source/graphics.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/index.rst` & `reportlab-4.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/lib.rst` & `reportlab-4.0.0/docs/source/lib.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/source/platypus.rst` & `reportlab-4.0.0/docs/source/platypus.rst`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/app_demos.py` & `reportlab-4.0.0/docs/userguide/app_demos.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch1_intro.py` & `reportlab-4.0.0/docs/userguide/ch1_intro.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch2_graphics.py` & `reportlab-4.0.0/docs/userguide/ch2_graphics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch2a_fonts.py` & `reportlab-4.0.0/docs/userguide/ch2a_fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch3_pdffeatures.py` & `reportlab-4.0.0/docs/userguide/ch3_pdffeatures.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch4_platypus_concepts.py` & `reportlab-4.0.0/docs/userguide/ch4_platypus_concepts.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 paragraph style.  We are only using two types of flowables here
 -- $Spacers$ and $Paragraphs$.  The first $Spacer$ ensures that the
 Paragraphs skip past the title string.
 """)
 
 disc("""
 To see the output of this example program run the module
-$docs/userguide/examples.py$ (from the ReportLab $docs$ distribution)
+$tools/docco/examples.py$ (from the ReportLab $source$ distribution)
 as a "top level script".  The script interpretation $python examples.py$ will
 generate the Platypus output $phello.pdf$.
 """)
 
 
 heading2("$Flowables$")
 disc("""
```

### Comparing `reportlab-3.6.9/docs/userguide/ch5_paragraphs.py` & `reportlab-4.0.0/docs/userguide/ch5_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch6_tables.py` & `reportlab-4.0.0/docs/userguide/ch6_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/ch7_custom.py` & `reportlab-4.0.0/docs/userguide/ch7_custom.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/genuserguide.py` & `reportlab-4.0.0/docs/userguide/genuserguide.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/graph_charts.py` & `reportlab-4.0.0/docs/userguide/graph_charts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/graph_concepts.py` & `reportlab-4.0.0/docs/userguide/graph_concepts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/graph_shapes.py` & `reportlab-4.0.0/docs/userguide/graph_shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/docs/userguide/graph_widgets.py` & `reportlab-4.0.0/docs/userguide/graph_widgets.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/__init__.py` & `reportlab-4.0.0/src/reportlab/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#Copyright ReportLab Europe Ltd. 2000-2021
+#Copyright ReportLab Europe Ltd. 2000-2023
 #see license.txt for license details
 __doc__="""The Reportlab PDF generation library."""
-Version = "3.6.9"
+Version = "4.0.0"
 __version__=Version
-__date__='20220322'
+__date__='20230504'
 
 import sys, os
 
 __min_python_version__ = (3,7)
 if sys.version_info< __min_python_version__:
     raise ImportError("""reportlab requires %s.%s+; other versions are unsupported.
 If you want to try with other python versions edit line 10 of reportlab/__init__
```

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt` & `reportlab-4.0.0/src/reportlab/fonts/DarkGarden-copying-gpl.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-copying.txt` & `reportlab-4.0.0/src/reportlab/fonts/DarkGarden-copying.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGarden-readme.txt` & `reportlab-4.0.0/src/reportlab/fonts/DarkGarden-readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGarden.sfd` & `reportlab-4.0.0/src/reportlab/fonts/DarkGarden.sfd`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.afm` & `reportlab-4.0.0/src/reportlab/fonts/DarkGardenMK.afm`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/DarkGardenMK.pfb` & `reportlab-4.0.0/src/reportlab/fonts/DarkGardenMK.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/Vera.ttf` & `reportlab-4.0.0/src/reportlab/fonts/Vera.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/VeraBI.ttf` & `reportlab-4.0.0/src/reportlab/fonts/VeraBI.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/VeraBd.ttf` & `reportlab-4.0.0/src/reportlab/fonts/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/VeraIt.ttf` & `reportlab-4.0.0/src/reportlab/fonts/VeraIt.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_a______.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_a______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_ab_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_ab_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_abi____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_abi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_ai_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_ai_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_eb_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_eb_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_ebi____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_ebi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_ei_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_ei_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/_er_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/_er_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/bitstream-vera-license.txt` & `reportlab-4.0.0/src/reportlab/fonts/bitstream-vera-license.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/callig15.afm` & `reportlab-4.0.0/src/reportlab/fonts/callig15.afm`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/callig15.pfb` & `reportlab-4.0.0/src/reportlab/fonts/callig15.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/cob_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/cob_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/cobo____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/cobo____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/com_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/com_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/coo_____.pfb` & `reportlab-4.0.0/src/reportlab/fonts/coo_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/sy______.pfb` & `reportlab-4.0.0/src/reportlab/fonts/sy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/zd______.pfb` & `reportlab-4.0.0/src/reportlab/fonts/zd______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/zx______.pfb` & `reportlab-4.0.0/src/reportlab/fonts/zx______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/fonts/zy______.pfb` & `reportlab-4.0.0/src/reportlab/fonts/zy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/README` & `reportlab-4.0.0/src/reportlab/graphics/barcode/README`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/TODO` & `reportlab-4.0.0/src/reportlab/graphics/barcode/TODO`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/__init__.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/__init__.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/code128.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/code128.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/code39.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/code39.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/code93.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/code93.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/common.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,29 @@
                 self.rect(left, bb, barWidth, tb)
                 left = left + barWidth
             elif c == 'B':
                 self.rect(left, bb, wx, tb)
                 left = left + wx
 
         if self.bearers:
-            self.rect(self.lquiet, 0, \
-                self._width - (self.lquiet + self.rquiet), b)
-            self.rect(self.lquiet, self.barHeight - b, \
-                self._width - (self.lquiet + self.rquiet), b)
+            if getattr(self,'bearerBox', None):
+                canv = self.canv
+                if hasattr(canv,'_Gadd'):
+                    #this is a widget rect takes other arguments
+                    canv.rect(bb, bb, self.width, self.barHeight-b,
+                            strokeWidth=b, strokeColor=self.barFillColor or self.barStrokeColor, fillColor=None)
+                else:
+                    canv.saveState()
+                    canv.setLineWidth(b)
+                    canv.rect(bb, bb, self.width, self.barHeight-b, stroke=1, fill=0)
+                    canv.restoreState()
+            else:
+                w = self._width - (self.lquiet + self.rquiet)
+                self.rect(self.lquiet, 0, w, b)
+                self.rect(self.lquiet, self.barHeight - b, w, b)
 
         self.drawHumanReadable()
 
     def drawHumanReadable(self):
         if self.humanReadable:
             #we have text
             from reportlab.pdfbase.pdfmetrics import getAscent, stringWidth
@@ -256,14 +267,17 @@
 
         bearers (float, in units of barWidth. default 3.0):
             Height of bearer bars (horizontal bars along the top and
             bottom of the barcode). Default is 3 x-dimensions.
             Set to zero for no bearer bars. (Bearer bars help detect
             misscans, so it is suggested to leave them on).
 
+        bearerBox (bool default False)
+            if true draw a  true rectangle of width bearers around the barcode.
+
         quiet (bool, default 1):
             Whether to include quiet zones in the symbol.
 
         lquiet (float, see default below):
             Quiet zone size to left of code, if quiet is true.
             Default is the greater of .25 inch, or .15 times the symbol's
             length.
@@ -300,14 +314,15 @@
     }
 
     barHeight = None
     barWidth = inch * 0.0075
     ratio = 2.2
     checksum = 1
     bearers = 3.0
+    bearerBox = False
     quiet = 1
     lquiet = None
     rquiet = None
     stop = 1
 
     def __init__(self, value='', **args):
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/dmtx.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/dmtx.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/eanbc.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/eanbc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/ecc200datamatrix.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/ecc200datamatrix.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/fourstate.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/fourstate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/lto.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/lto.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/qr.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/qr.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/qrencoder.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/qrencoder.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/test.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,19 @@
     styleN = styles['Normal']
     styleH = styles['Heading1']
     story = []
     storyAdd = story.append
 
     #for codeNames in code
     storyAdd(Paragraph('I2of5', styleN))
-    storyAdd(I2of5(1234, barWidth = inch*0.02, checksum=0))
+    storyAdd(I2of5('05400141288766', barWidth = inch*0.02, checksum=0))
+    storyAdd(I2of5('0001234567890', barWidth = inch*0.02, checksum=1))
+    storyAdd(I2of5('00012345678905', barWidth = inch*0.02, checksum=0))
+    storyAdd(I2of5('0001234567890', barWidth = inch*0.02, checksum=1, bearerBox = True))
+    
 
     storyAdd(Paragraph('MSI', styleN))
     storyAdd(MSI(1234))
 
     storyAdd(Paragraph('Codabar', styleN))
     storyAdd(Codabar("A012345B", barWidth = inch*0.02))
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/usps.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/usps.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/usps4s.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/usps4s.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/barcode/widgets.py` & `reportlab-4.0.0/src/reportlab/graphics/barcode/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,21 @@
         if 'width' in self.__dict__: del self.__dict__['width']
         if 'height' in self.__dict__: del self.__dict__['height']
         self.x = self.y = 0
         kw.setdefault('value',_value)
         self._BCC.__init__(self,**kw)
 
     def rect(self,x,y,w,h,**kw):
-        self._Gadd(Rect(self.x+x,self.y+y,w,h,
-                    strokeColor=self.barStrokeColor,strokeWidth=self.barStrokeWidth, fillColor=self.barFillColor))
+        #this allows the base code to draw rectangles for us using self.rect
+        #using direct keyword argument overrides see eg common.py line 140 on
+        for k,v in (('strokeColor',self.barStrokeColor),
+                    ('strokeWidth',self.barStrokeWidth),
+                    ('fillColor',self.barFillColor)):
+            kw.setdefault(k,v)
+        self._Gadd(Rect(self.x+x,self.y+y,w,h, **kw))
 
     def draw(self):
         if not self._BCC: raise NotImplementedError("Abstract class %s cannot be drawn" % self.__class__.__name__)
         self.canv = self
         G = Group()
         self._Gadd = G.add
         self._Gadd(Rect(self.x,self.y,self.width,self.height,fillColor=None,strokeColor=None,strokeWidth=0.0001))
@@ -133,14 +138,16 @@
         checksum = AttrMapValue(isBoolean,'''(bool, default 1):
             Whether to compute and include the check digit'''),
         bearers = AttrMapValue(isNumber,'''(float, in units of barWidth. default 3.0):
             Height of bearer bars (horizontal bars along the top and
             bottom of the barcode). Default is 3 x-dimensions.
             Set to zero for no bearer bars. (Bearer bars help detect
             misscans, so it is suggested to leave them on).'''),
+        bearerBox = AttrMapValue(isBoolean,'''(bool, default 0):
+            if True turn bearers into a box'''),
         quiet = AttrMapValue(isBoolean,'''(bool, default 1):
             Whether to include quiet zones in the symbol.'''),
 
         lquiet = AttrMapValue(isNumber,'''(float, see default below):
             Quiet zone size to left of code, if quiet is true.
             Default is the greater of .25 inch, or .15 times the symbol's
             length.'''),
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/areas.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/areas.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/axes.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/axes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/barcharts.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/barcharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/dotbox.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/dotbox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/doughnut.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/doughnut.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/legends.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/legends.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/linecharts.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/linecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/lineplots.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/lineplots.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/markers.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/piecharts.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/piecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/slidebox.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/spider.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/spider.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/textlabels.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/utils.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/charts/utils3d.py` & `reportlab-4.0.0/src/reportlab/graphics/charts/utils3d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/renderPDF.py` & `reportlab-4.0.0/src/reportlab/graphics/renderPDF.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/renderPM.py` & `reportlab-4.0.0/src/reportlab/graphics/renderPM.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,37 @@
 from reportlab import rl_config
 from .utils import setFont as _setFont, RenderPMError
 
 import os, sys
 from io import BytesIO, StringIO
 from math import sin, cos, pi, ceil
 
-try:
-    from reportlab.graphics import _renderPM
-except ImportError as errMsg:
-    raise ImportError("""No module named _renderPM\nit may be badly or not installed!
+def _getPMBackend(backend=None):
+    if not backend: backend = rl_config.renderPMBackend
+    if backend=='_renderPM':
+        try:
+            import _rl_renderPM as M
+        except ImportError as errMsg:
+            raise ImportError("""No module named _rl_renderPM
+it may be badly or not installed!
 You may need to install development tools
 or seek advice at the users list see
 https://pairlist2.pair.net/mailman/listinfo/reportlab-users""")
+    elif 'cairo' in backend.lower():
+        try:
+            import rlPyCairo as M
+        except ImportError as errMsg:
+            raise ImportError("""cannot import desired renderPM backend rlPyCairo
+Seek advice at the users list see
+https://pairlist2.pair.net/mailman/listinfo/reportlab-users""")
+    else:
+        raise RenderPMError(f'Invalid renderPM backend, {backend}')
+    return M
+
+_pmBackend = _getPMBackend(rl_config.renderPMBackend)
 
 def _getImage():
     try:
         from PIL import Image
     except ImportError:
         import Image
     return Image
@@ -88,15 +104,15 @@
         if alpha is not None:
             self._canvas.fillOpacity = alpha
         self._canvas.setFillColor(s['fillColor'])
         self._canvas.setFont(s['fontName'], s['fontSize'])
 
     def initState(self,x,y):
         deltas = self._tracker._combined[-1]
-        deltas['transform'] = self._canvas._baseCTM[0:4]+(x,y)
+        deltas['transform'] = deltas['ctm'] = self._canvas._baseCTM[0:4]+(x,y)
         self._tracker.push(deltas)
         self.applyState()
 
     def drawNode(self, node):
         """This is the recursive method called for each node
         in the tree"""
 
@@ -253,72 +269,67 @@
 
 def _convert2pil1(im):
     return im.convert("1")
 
 def _saveAsPICT(im,fn,fmt,transparent=None):
     im = _convert2pilp(im)
     cols, rows = im.size
-    #s = _renderPM.pil2pict(cols,rows,im.tostring(),im.im.getpalette(),transparent is not None and Color2Hex(transparent) or -1)
-    s = _renderPM.pil2pict(cols,rows,(im.tobytes if hasattr(im,'tobytes') else im.tostring)(),im.im.getpalette())
+    s = _pmBackend.pil2pict(cols,rows,(im.tobytes if hasattr(im,'tobytes') else im.tostring)(),im.im.getpalette())
     if not hasattr(fn,'write'):
         with open(os.path.splitext(fn)[0]+'.'+fmt.lower(),'wb') as f:
             f.write(s)
         if os.name=='mac':
             from reportlab.lib.utils import markfilename
             markfilename(fn,ext='PICT')
     else:
         fn.write(s)
 
 BEZIER_ARC_MAGIC = 0.5522847498     #constant for drawing circular arcs w/ Beziers
 class PMCanvas:
-    def __init__(self,w,h,dpi=72,bg=0xffffff,configPIL=None,backend=rl_config.renderPMBackend):
+    def __init__(self,w,h,dpi=72,bg=0xffffff,configPIL=None,backend=rl_config.renderPMBackend,
+                    backendFmt='RGB'):
         '''configPIL dict is passed to image save method'''
         scale = dpi/72.0
         w = int(w*scale+0.5)
         h = int(h*scale+0.5)
         self.__dict__['_gs'] = self._getGState(w,h,bg,backend)
         self.__dict__['_bg'] = bg
         self.__dict__['_baseCTM'] = (scale,0,0,scale,0,0)
         self.__dict__['_clipPaths'] = []
         self.__dict__['configPIL'] = configPIL
         self.__dict__['_dpi'] = dpi
         self.__dict__['_backend'] = backend
+        self.__dict__['_backendfmt'] = backendFmt
         self.ctm = self._baseCTM
 
     @staticmethod
-    def _getGState(w, h, bg, backend='_renderPM', fmt='RGB24'):
+    def _getGState(w, h, bg, backend=None, fmt='RGB24'):
+        mod = _getPMBackend(backend)
         if backend=='_renderPM':
-            return _renderPM.gstate(w,h,bg=bg)
-        elif backend=='rlPyCairo':
-            try:
-                from rlPyCairo import GState
-            except ImportError:
-                raise RenderPMError('cannot import rlPyCairo; perhaps it needs to be installed!')
-            else:
-                return GState(w,h,bg,fmt=fmt)
-        else:
-            raise RenderPMError('Invalid backend, %r, given to PMCanvas' % backend)
+            return mod.gstate(w,h,bg=bg)
+        elif 'cairo' in backend.lower():
+            return mod.GState(w,h,bg,fmt=fmt)
 
     def _drawTimeResize(self,w,h,bg=None):
         if bg is None: bg = self._bg
         self._drawing.width, self._drawing.height = w, h
         A = {'ctm':None, 'strokeWidth':None, 'strokeColor':None, 'lineCap':None, 'lineJoin':None, 'dashArray':None, 'fillColor':None}
         gs = self._gs
         fN,fS = gs.fontName, gs.fontSize
         for k in A.keys():
             A[k] = getattr(gs,k)
         del gs, self._gs
-        gs = self.__dict__['_gs'] = _renderPM.gstate(w,h,bg=bg)
+        gs = self.__dict__['_gs'] = _pmBackend.gstate(w,h,bg=bg)
         for k in A.keys():
             setattr(self,k,A[k])
         gs.setFont(fN,fS)
 
     def toPIL(self):
         im = _getImage().new('RGB', size=(self._gs.width, self._gs.height))
-        (getattr(im,'frombytes',None) or getattr(im,'fromstring'))(self._gs.pixBuf)
+        im.frombytes(self._gs.pixBuf)
         return im
 
     def saveToFile(self,fn,fmt=None):
         im = self.toPIL()
         if fmt is None:
             if not isinstance(fn,str):
                 raise ValueError("Invalid value '%s' for fn when fmt is None" % ascii(fn))
@@ -728,15 +739,15 @@
         if shout or verbose>2: print(msg)
         errs.append('<br/><h2 style="color:red">%s</h2>' % msg)
         buf = StringIO()
         traceback.print_exc(file=buf)
         errs.append('<pre>%s</pre>' % escape(buf.getvalue()))
 
     #print in a loop, with their doc strings
-    for (drawing, docstring, name) in getAllTestDrawings(doTTF=hasattr(_renderPM,'ft_get_face')):
+    for (drawing, docstring, name) in getAllTestDrawings(doTTF=hasattr(_pmBackend,'ft_get_face')):
         i = names[name] = names.setdefault(name,0)+1
         if i>1: name += '.%02d' % (i-1)
         if argv and name not in argv: continue
         fnRoot = name
         w = int(drawing.width)
         h = int(drawing.height)
         html.append('<hr><h2>Drawing %s</h2>\n<pre>%s</pre>' % (name, docstring))
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/renderPS.py` & `reportlab-4.0.0/src/reportlab/graphics/renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/renderSVG.py` & `reportlab-4.0.0/src/reportlab/graphics/renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/renderbase.py` & `reportlab-4.0.0/src/reportlab/graphics/renderbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/bubble.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/bubble.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/clustered_bar.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/clustered_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/clustered_column.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/clustered_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/excelcolors.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/excelcolors.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/exploded_pie.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/exploded_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/filled_radar.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/filled_radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/line_chart.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/line_chart.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/linechart_with_markers.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/linechart_with_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/radar.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/runall.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/runall.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/scatter.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/scatter.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/scatter_lines.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/scatter_lines_markers.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/scatter_lines_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/simple_pie.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/simple_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/stacked_bar.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/samples/stacked_column.py` & `reportlab-4.0.0/src/reportlab/graphics/samples/stacked_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/shapes.py` & `reportlab-4.0.0/src/reportlab/graphics/shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/testdrawings.py` & `reportlab-4.0.0/src/reportlab/graphics/testdrawings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/testshapes.py` & `reportlab-4.0.0/src/reportlab/graphics/testshapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,16 +411,16 @@
     g = Group(transform=(2,0,0,2,0,0))
     return D
 
 
 def getDrawing12():
     """Text strings in a non-standard font.
     All that is required is to place the .afm and .pfb files
-    on the font patch given in rl_config.py,
-    for example in reportlab/lib/fonts/.
+    on the font path given in rl_config.py,
+    for example in reportlab/fonts/.
     """
     faceName = "DarkGardenMK"
     D = Drawing(400, 200)
     for size in range(12, 36, 4):
         D.add(String(10+size*2,
                      10+size*2,
                      'Hello World',
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/transform.py` & `reportlab-4.0.0/src/reportlab/graphics/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,37 +9,37 @@
     'mmult',
     'inverse',
     'zTransformPoint',
     'transformPoint',
     'transformPoints',
     'zTransformPoints',
     )
-from math import pi, cos, sin, tan
+from math import cos, sin, tan, radians
 
 # constructors for matrices:
 def nullTransform():
     return (1, 0, 0, 1, 0, 0)
 
 def translate(dx, dy):
     return (1, 0, 0, 1, dx, dy)
 
 def scale(sx, sy):
     return (sx, 0, 0, sy, 0, 0)
 
 def rotate(angle):
-    a = angle * pi/180
-    return (cos(a), sin(a), -sin(a), cos(a), 0, 0)
+    a = radians(angle)
+    sina = sin(a)
+    cosa = cos(a)
+    return (cosa, sina, -sina, cosa, 0, 0)
 
 def skewX(angle):
-    a = angle * pi/180
-    return (1, 0, tan(a), 1, 0, 0)
+    return (1, 0, tan(radians(angle)), 1, 0, 0)
 
 def skewY(angle):
-    a = angle * pi/180
-    return (1, tan(a), 0, 1, 0, 0)
+    return (1, tan(radians(angle)), 0, 1, 0, 0)
 
 def mmult(A, B):
     "A postmultiplied by B"
     # I checked this RGB
     # [a0 a2 a4]    [b0 b2 b4]
     # [a1 a3 a5] *  [b1 b3 b5]
     # [      1 ]    [      1 ]
```

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgetbase.py` & `reportlab-4.0.0/src/reportlab/graphics/widgetbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/adjustableArrow.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/adjustableArrow.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/eventcal.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/eventcal.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/flags.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/flags.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/grids.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/markers.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/signsandsymbols.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/signsandsymbols.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/graphics/widgets/table.py` & `reportlab-4.0.0/src/reportlab/graphics/widgets/table.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/PyFontify.py` & `reportlab-4.0.0/src/reportlab/lib/PyFontify.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/abag.py` & `reportlab-4.0.0/src/reportlab/lib/abag.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/arciv.py` & `reportlab-4.0.0/src/reportlab/lib/arciv.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/attrmap.py` & `reportlab-4.0.0/src/reportlab/lib/attrmap.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/boxstuff.py` & `reportlab-4.0.0/src/reportlab/lib/boxstuff.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/codecharts.py` & `reportlab-4.0.0/src/reportlab/lib/codecharts.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         self.encodingName = encodingName
 
         try:
             # the dependent files might not be available
             font = cidfonts.CIDFont(self.faceName, self.encodingName)
             pdfmetrics.registerFont(font)
         except:
-            # fall back to English and at least shwo we can draw the boxes
+            # fall back to English and at least show we can draw the boxes
             self.faceName = 'Helvetica'
             self.encodingName = 'WinAnsiEncoding'
         self.fontName = self.faceName + '-' + self.encodingName
         self.calcLayout()
 
     def makeRow(self, row):
         """Works out the character values for this kuten row"""
@@ -248,15 +248,15 @@
         self.encodingName = encodingName
         self.rowLabels = ['4','5','6','7','A','B','C','D','E','F']
         try:
             # the dependent files might not be available
             font = cidfonts.CIDFont(self.faceName, self.encodingName)
             pdfmetrics.registerFont(font)
         except:
-            # fall back to English and at least shwo we can draw the boxes
+            # fall back to English and at least show we can draw the boxes
             self.faceName = 'Helvetica'
             self.encodingName = 'WinAnsiEncoding'
         self.fontName = self.faceName + '-' + self.encodingName
         self.calcLayout()
 
     def makeRow(self, row):
         """Works out the character values for this Big5 row.
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/colors.py` & `reportlab-4.0.0/src/reportlab/lib/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 >>> toColor('pcmyka(100,0,0,0)')
 Traceback (most recent call last):
     ....
 ValueError: css color 'pcmyka(100,0,0,0)' has wrong number of components
 '''
 import math, re, functools
 from reportlab.lib.rl_accel import fp_str
-from reportlab.lib.utils import asNative, isStr, rl_safe_eval
+from reportlab.lib.utils import asNative, isStr, rl_safe_eval, rl_extended_literal_eval
+from reportlab import rl_config
 from ast import literal_eval
 
 class Color:
     """This class is used to represent color.  Components red, green, blue
     are in the range 0 (dark) to 1 (full intensity)."""
 
     def __init__(self, red=0, green=0, blue=0, alpha=1):
@@ -831,14 +832,25 @@
                 R,G,B = list(map('%' in n[0] and self.rgbPcVal or self.rgbVal,n))
 
             return Color(R,G,B,a)
 
 cssParse=cssParse()
 
 class toColor:
+    """Accepot an expression returnng a Color subclass.
+
+    This used to accept arbitrary Python expressions, which resulted in increasngly devilish CVEs and
+    security holes from tie to time.  In April 2023 we are creating explicit, "dumb" parsing code to
+    replace this.  Acceptable patterns are
+
+    a Color instance passed in by the Python programmer
+    a named list of colours ('pink' etc')
+    list of 3 or 4 numbers
+    all CSS colour expression
+    """
     _G = {} #globals we like (eventually)
 
     def __init__(self):
         self.extraColorsNS = {} #used for overriding/adding to existing color names
                                 #make case insensitive if that's your wish
 
     def setExtraColorsNameSpace(self,NS):
@@ -856,29 +868,66 @@
             arg = asNative(arg)
             C = cssParse(arg)
             if C: return C
             if arg in self.extraColorsNS: return self.extraColorsNS[arg]
             C = getAllNamedColors()
             s = arg.lower()
             if s in C: return C[s]
-            G = C.copy()
-            G.update(self.extraColorsNS)
-            if not self._G:
-                C = globals()
-                self._G = {s:C[s] for s in '''Blacker CMYKColor CMYKColorSep Color ColorType HexColor PCMYKColor PCMYKColorSep Whiter
-                    _chooseEnforceColorSpace _enforceCMYK _enforceError _enforceRGB _enforceSEP _enforceSEP_BLACK
-                    _enforceSEP_CMYK _namedColors _re_css asNative cmyk2rgb cmykDistance color2bw colorDistance
-                    cssParse describe fade fp_str getAllNamedColors hsl2rgb hue2rgb isStr linearlyInterpolatedColor
-                    literal_eval obj_R_G_B opaqueColor rgb2cmyk setColors toColor toColorOrNone'''.split()}
-            G.update(self._G)
+
+
+            # allow expressions like 'Blacker(red, 0.5)'
+            # >>> re.compile(r"(Blacker|Whiter)\((\w+)\,\s?([0-9.]+)\)").match(msg).groups()
+            # ('Blacker', 'red', '0.5')
+            # >>> 
+            pat = re.compile(r"(Blacker|Whiter)\((\w+)\,\s?([0-9.]+)\)")
+            m = pat.match(arg)
+            if m:
+                funcname, rootcolor, num = m.groups()
+                if funcname == 'Blacker':
+                    return Blacker(rootcolor, float(num))
+                else:
+                    return Whiter(rootcolor, float(num))
+
             try:
-                return toColor(rl_safe_eval(arg,g=G,l={}))
-            except:
+                import ast
+                expr = ast.literal_eval(arg)    #safe probably only a tuple or list of values
+                return toColor(expr)
+            except (SyntaxError, ValueError):
                 pass
 
+            if rl_config.toColorCanUse=='rl_safe_eval':
+                #the most dangerous option
+                G = C.copy()
+                G.update(self.extraColorsNS)
+                if not self._G:
+                    C = globals()
+                    self._G = {s:C[s] for s in '''Blacker CMYKColor CMYKColorSep Color ColorType HexColor PCMYKColor PCMYKColorSep Whiter
+                        _chooseEnforceColorSpace _enforceCMYK _enforceError _enforceRGB _enforceSEP _enforceSEP_BLACK
+                        _enforceSEP_CMYK _namedColors _re_css asNative cmyk2rgb cmykDistance color2bw colorDistance
+                        cssParse describe fade fp_str getAllNamedColors hsl2rgb hue2rgb isStr linearlyInterpolatedColor
+                        literal_eval obj_R_G_B opaqueColor rgb2cmyk setColors toColor toColorOrNone'''.split()}
+                G.update(self._G)
+                try:
+                    return toColor(rl_safe_eval(arg,g=G,l={}))
+                except:
+                    pass
+            elif rl_config.toColorCanUse=='rl_extended_literal_eval':
+                C = globals()
+                S = getAllNamedColors().copy()
+                C = {k:C[k] for k in '''Blacker CMYKColor CMYKColorSep Color ColorType HexColor PCMYKColor PCMYKColorSep Whiter
+                        _chooseEnforceColorSpace _enforceCMYK _enforceError _enforceRGB _enforceSEP _enforceSEP_BLACK
+                        _enforceSEP_CMYK _namedColors _re_css asNative cmyk2rgb cmykDistance color2bw colorDistance
+                        cssParse describe fade fp_str getAllNamedColors hsl2rgb hue2rgb linearlyInterpolatedColor
+                        obj_R_G_B opaqueColor rgb2cmyk setColors toColor toColorOrNone'''.split()
+                        if callable(C.get(k,None))}
+                try:
+                    return rl_extended_literal_eval(arg,C,S)
+                except (ValueError, SyntaxError):
+                    pass
+
         try:
             return HexColor(arg)
         except:
             if default is None:
                 raise ValueError('Invalid color value %r' % arg)
             return default
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/corp.py` & `reportlab-4.0.0/src/reportlab/lib/corp.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/extformat.py` & `reportlab-4.0.0/src/reportlab/lib/extformat.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/fontfinder.py` & `reportlab-4.0.0/src/reportlab/lib/fontfinder.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/fonts.py` & `reportlab-4.0.0/src/reportlab/lib/fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/formatters.py` & `reportlab-4.0.0/src/reportlab/lib/formatters.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/geomutils.py` & `reportlab-4.0.0/src/reportlab/lib/geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/logger.py` & `reportlab-4.0.0/src/reportlab/lib/logger.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/normalDate.py` & `reportlab-4.0.0/src/reportlab/lib/normalDate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/pagesizes.py` & `reportlab-4.0.0/src/reportlab/lib/pagesizes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/pdfencrypt.py` & `reportlab-4.0.0/src/reportlab/lib/pdfencrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #copyright ReportLab Europe Limited. 2000-2016
 #see license.txt for license details
 __version__='3.3.0'
 
 """helpers for pdf encryption/decryption"""
 import sys, os
 from binascii import hexlify, unhexlify
+from hashlib import md5
 from io import BytesIO
 
-from reportlab.lib.utils import md5, asBytes, int2Byte, rawBytes, asNative
+from reportlab.lib.utils import asBytes, int2Byte, rawBytes, asNative
 from reportlab.pdfgen.canvas import Canvas
 from reportlab.pdfbase.pdfdoc import PDFObject
 from reportlab.platypus.flowables import Flowable
 from reportlab import rl_config
 
 try:
     import pyaes
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/pygments2xpre.py` & `reportlab-4.0.0/src/reportlab/lib/pygments2xpre.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/randomtext.py` & `reportlab-4.0.0/src/reportlab/lib/randomtext.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/rl_accel.py` & `reportlab-4.0.0/src/reportlab/lib/rl_accel.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import reportlab
 testing = getattr(reportlab,'_rl_testing',False)
 del reportlab
 
 for fn in __all__:
     D={}
     try:
-        exec('from reportlab.lib._rl_accel import %s as f' % fn,D)
+        exec('from _rl_accel import %s as f' % fn,D)
         _c_funcs[fn] = D['f']
         if testing: _py_funcs[fn] = None
     except ImportError:
         _py_funcs[fn] = None
     del D
 
 if _py_funcs:
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/rl_safe_eval.py` & `reportlab-4.0.0/src/reportlab/lib/rl_safe_eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #this code is copied/stolen/borrowed/modified from various sources including
 #https://github.com/zopefoundation/AccessControl
 #https://github.com/zopefoundation/RestrictedPython
 #https://github.com/danthedeckie/simpleeval
 #hopefully we are standing on giants' shoulders
-import sys, os, ast, re, weakref, time, copy, math
+import sys, os, ast, re, weakref, time, copy, math, types
 eval_debug = int(os.environ.get('EVAL_DEBUG','0'))
 strTypes = (bytes,str)
 isPy39 = sys.version_info[:2]>=(3,9)
 
 haveNameConstant = hasattr(ast,'NameConstant')
 import textwrap
 
@@ -49,21 +49,23 @@
 						co_lnotab co_name co_names co_nlocals co_posonlyargcount co_stacksize
 						co_varnames cr_await cr_code cr_frame cr_origin cr_running __defaults__
 						f_back f_builtins f_code f_exc_traceback f_exc_type f_exc_value f_globals
 						f_lasti f_lineno f_locals f_restricted f_trace __func__ func_code func_defaults
 						func_doc func_globals func_name gi_code gi_frame gi_running gi_yieldfrom
 						__globals__ im_class im_func im_self __iter__ __kwdefaults__ __module__
 						__name__ next __qualname__ __self__ tb_frame tb_lasti tb_lineno tb_next
-						globals vars locals'''.split()
+						globals vars locals
+						type eval exec aiter anext compile open
+						dir print classmethod staticmethod __import__ super property'''.split()
 						)
 __rl_unsafe_re__ = re.compile(r'\b(?:%s)' % '|'.join(__rl_unsafe__),re.M)
 
+
 def copy_locations(new_node, old_node):
-	new_node.lineno = old_node.lineno
-	new_node.col_offset = old_node.col_offset
+	ast.copy_location(new_node, old_node)
 	ast.fix_missing_locations(new_node)
 
 class UntrustedAstTransformer(ast.NodeTransformer):
 
 	def __init__(self, names_seen=None, nameIsAllowed=None):
 		super(UntrustedAstTransformer, self).__init__()
 		self.names_seen = {} if names_seen is None else names_seen
@@ -1200,9 +1202,74 @@
 		return self.env.__rl_safe_eval__(expr, g, l, self.mode, timeout=timeout,
 			allowed_magic_methods=allowed_magic_methods,
 			__frame_depth__=2)
 
 class __rl_safe_exec__(__rl_safe_eval__):
 	mode = 'exec'
 
+def rl_extended_literal_eval(expr, safe_callables=None, safe_names=None):
+	if safe_callables is None:
+		safe_callables = {}
+	if safe_names is None:
+		safe_names = {}
+	safe_names = safe_names.copy()
+	safe_names.update({'None': None, 'True': True, 'False': False})
+	#make these readonly with MappingProxyType
+	safe_names = types.MappingProxyType(safe_names)
+	safe_callables = types.MappingProxyType(safe_callables)
+	if isinstance(expr, str):
+		expr = ast.parse(expr, mode='eval')
+	if isinstance(expr, ast.Expression):
+		expr = expr.body
+	try:
+		# Python 3.4 and up
+		ast.NameConstant
+		safe_test = lambda n: isinstance(n, ast.NameConstant) or isinstance(n,ast.Name) and n.id in safe_names
+		safe_extract = lambda n: n.value if isinstance(n,ast.NameConstant) else safe_names[n.id]
+	except AttributeError:
+		# Everything before
+		safe_test = lambda n: isinstance(n, ast.Name) and n.id in safe_names
+		safe_extract = lambda n: safe_names[n.id]
+	def _convert(node):
+		if isinstance(node, (ast.Str, ast.Bytes)):
+			return node.s
+		elif isinstance(node, ast.Num):
+			return node.n
+		elif isinstance(node, ast.Tuple):
+			return tuple(map(_convert, node.elts))
+		elif isinstance(node, ast.List):
+			return list(map(_convert, node.elts))
+		elif isinstance(node, ast.Dict):
+			return dict((_convert(k), _convert(v)) for k, v
+						in zip(node.keys, node.values))
+		elif safe_test(node):
+			return safe_extract(node)
+		elif isinstance(node, ast.UnaryOp) and \
+			 isinstance(node.op, (ast.UAdd, ast.USub)) and \
+			 isinstance(node.operand, (ast.Num, ast.UnaryOp, ast.BinOp)):
+			operand = _convert(node.operand)
+			if isinstance(node.op, ast.UAdd):
+				return + operand
+			else:
+				return - operand
+		elif isinstance(node, ast.BinOp) and \
+			 isinstance(node.op, (ast.Add, ast.Sub)) and \
+			 isinstance(node.right, (ast.Num, ast.UnaryOp, ast.BinOp)) and \
+			 isinstance(node.right.n, complex) and \
+			 isinstance(node.left, (ast.Num, ast.UnaryOp, astBinOp)):
+			left = _convert(node.left)
+			right = _convert(node.right)
+			if isinstance(node.op, ast.Add):
+				return left + right
+			else:
+				return left - right
+		elif isinstance(node, ast.Call) and \
+			 isinstance(node.func, ast.Name) and \
+			 node.func.id in safe_callables:
+			return safe_callables[node.func.id](
+				*[_convert(n) for n in node.args],
+				**{kw.arg: _convert(kw.value) for kw in node.keywords})
+		raise ValueError('Bad expression')
+	return _convert(expr)
+
 rl_safe_exec = __rl_safe_exec__()
 rl_safe_eval = __rl_safe_eval__()
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/rltempfile.py` & `reportlab-4.0.0/src/reportlab/lib/rltempfile.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/rparsexml.py` & `reportlab-4.0.0/src/reportlab/lib/rparsexml.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,28 @@
     def parsexml(xmlText, oneOutermostTag=0,eoCB=None,entityReplacer=None,parseOpts={}):
         pyRXP_parser.eoCB = eoCB
         p = pyRXP_parser.parse(xmlText,**parseOpts)
         return oneOutermostTag and p or ('',None,[p],None)
 except ImportError:
     simpleparse = 1
 
+class smartDecode:
+    @staticmethod
+    def __call__(s):
+        print('initial')
+        import chardet
+        def __call__(s):
+            if isinstance(s,str): return s
+            cdd = chardet.detect(s)
+            print('final')
+            return s.decode(cdd["encoding"])
+        smartDecode.__class__.__call__ = staticmethod(__call__)
+        return  __call__(s)
+smartDecode = smartDecode()
+
 NONAME = ""
 NAMEKEY = 0
 CONTENTSKEY = 1
 CDATAMARKER = "<![CDATA["
 LENCDATAMARKER = len(CDATAMARKER)
 CDATAENDMARKER = "]]>"
 replacelist = [("&lt;", "<"), ("&gt;", ">"), ("&amp;", "&")] # amp must be last
@@ -142,14 +156,15 @@
         entityReplacer=unEscapeContentList,
         #len=len, None=None
         #LENCDATAMARKER=LENCDATAMARKER, CDATAMARKER=CDATAMARKER
         ):
     """simple recursive descent xml parser...
        return (dictionary, endcharacter)
        special case: comment returns (None, endcharacter)"""
+    xmltext = smartDecode(xmltext)
     #print "parsexml0", repr(xmltext[startingat: startingat+10])
     # DEFAULTS
     NameString = NONAME
     ContentList = AttDict = ExtraStuff = None
     if toplevel is not None:
         #if verbose: print "at top level"
         #if startingat!=0:
@@ -366,16 +381,15 @@
     if ContentList:
         if entityReplacer: ContentList = entityReplacer(ContentList)
     t = (NameString, AttDict, ContentList, ExtraStuff)
     return (t, cursor)
 
 def pprettyprint(parsedxml):
     """pretty printer mainly for testing"""
-    st = bytes
-    if type(parsedxml) is st:
+    if isinstance(parsedxml,(str,bytes)):
         return parsedxml
     (name, attdict, textlist, extra) = parsedxml
     if not attdict: attdict={}
     attlist = []
     for k in attdict.keys():
         v = attdict[k]
         attlist.append("%s=%s" % (k, repr(v)))
@@ -391,45 +405,48 @@
         # indent it
         nllist = textpprint.split("\n")
         textpprint = "   "+ ("\n   ".join(nllist))
         return "<%s %s>\n%s\n</%s>" % (name, attributes, textpprint, name)
     # otherwise must be a simple tag
     return "<%s %s/>" % (name, attributes)
 
-dump = 0
-def testparse(s):
+def testparse(s,dump=0):
     from time import time
     from pprint import pprint
     now = time()
-    D = parsexmlSimple(s)
+    breakpoint()
+    D = parsexmlSimple(s,oneOutermostTag=1)
     print("DONE", time()-now)
     if dump&4:
         pprint(D)
     #pprint(D)
     if dump&1:
         print("============== reformatting")
         p = pprettyprint(D)
         print(p)
 
-def test():
+def test(dump=0):
     testparse("""<this type="xml">text &lt;&gt;<b>in</b> <funnytag foo="bar"/> xml</this>
                  <!-- comment -->
                  <![CDATA[
                  <this type="xml">text <b>in</b> xml</this> ]]>
                  <tag with="<brackets in values>">just testing brackets feature</tag>
-                 """)
-
-filenames = [ #"../../reportlab/demos/pythonpoint/pythonpoint.xml",
-              "samples/hamlet.xml"]
-
-#filenames = ["moa.xml"]
+                 """,dump=dump)
 
-dump=1
 if __name__=="__main__":
-    test()
+    test(dump=1)
+    import sys, os
     from time import time
+    import reportlab
     now = time()
-    for f in filenames:
-        t = open(f).read()
-        print("parsing", f)
-        testparse(t)
-    print("elapsed", time()-now)
+    seen = 0
+    for f in sys.argv[1:]:
+        if not os.path.isfile(f):
+            print("!!!!! no file at {f!r}")
+        else:
+            with open(f) as _f:
+                t = _f.read()
+            print(f"parsing {f!r} |t|={len(t)}")
+            testparse(t,dump=1)
+            seen += 1
+    if seen:
+        print(f"timed at {time()-now:.2f} secs.")
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/sequencer.py` & `reportlab-4.0.0/src/reportlab/lib/sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/styles.py` & `reportlab-4.0.0/src/reportlab/lib/styles.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/testutils.py` & `reportlab-4.0.0/src/reportlab/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/textsplit.py` & `reportlab-4.0.0/src/reportlab/lib/textsplit.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/units.py` & `reportlab-4.0.0/src/reportlab/lib/units.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/utils.py` & `reportlab-4.0.0/src/reportlab/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 __version__='3.5.34'
 __doc__='''Gazillions of miscellaneous internal utility functions'''
 
 import os, pickle, sys, time, types, datetime, importlib
 from ast import literal_eval
 from base64 import decodebytes as base64_decodebytes, encodebytes as base64_encodebytes
 from io import BytesIO
+from hashlib import md5
 
 from reportlab.lib.rltempfile import get_rl_tempfile, get_rl_tempdir
-from . rl_safe_eval import rl_safe_exec, rl_safe_eval, safer_globals
+from . rl_safe_eval import rl_safe_exec, rl_safe_eval, safer_globals, rl_extended_literal_eval
+from PIL import Image
 
 class __UNSET__:
     @staticmethod
     def __bool__():
         return False
     @staticmethod
     def __str__():
         return '__UNSET__'
     __repr__ = __str__
 __UNSET__ = __UNSET__()
 
 try:
-    from hashlib import md5
-except ImportError:
-    import md5
-
-try:
     import platform
     isPyPy = platform.python_implementation()=='PyPy'
 except:
     isPyPy = False
 
 def isFunction(v):
     return type(v) == type(isFunction)
@@ -385,25 +382,14 @@
                 str(sys.exc_info()[1]), modulename,sys.path,os.getcwd()))
     finally:
         sys.path = opath
         _importlib_invalidate_caches()
         if debug:
             print('===== restore sys.path=%s' % repr(opath))
 
-# Image Capability Detection.  Set a flag haveImages
-# to tell us if PIL library is present.
-# define PIL_Image as either None, or an alias for the PIL.Image
-# module, as there are 2 ways to import it
-try:
-    from PIL import Image
-except ImportError:
-    try:
-        import Image
-    except ImportError:
-        Image = None
 haveImages = Image is not None
 
 class ArgvDictValue:
     '''A type to allow clients of getArgvDict to specify a conversion function'''
     def __init__(self,value,func):
         self.value = value
         self.func = func
@@ -648,54 +634,27 @@
             try:
                 self.fileName = self._image.fileName
             except AttributeError:
                 self.fileName = 'PILIMAGE_%d' % id(self)
         else:
             try:
                 from reportlab.rl_config import imageReaderFlags
-                self.fp = open_for_read(fileName,'b')
-                if isinstance(self.fp, BytesIO): imageReaderFlags=0 #avoid messing with already internal files
-                if imageReaderFlags>0:  #interning
-                    data = self.fp.read()
-                    if imageReaderFlags&2:  #autoclose
-                        try:
-                            self.fp.close()
-                        except:
-                            pass
-                    if imageReaderFlags&4:  #cache the data
-                        if not self._cache:
-                            from rl_config import register_reset
-                            register_reset(self._cache.clear)
-                        data=self._cache.setdefault(_digester(data),data)
-                    self.fp=BytesIO(data)
-                elif imageReaderFlags==-1 and isinstance(fileName,str):
-                    #try Ralf Schmitt's re-opening technique of avoiding too many open files
-                    self.fp.close()
-                    del self.fp #will become a property in the next statement
-                    self.__class__=LazyImageReader
-                if haveImages:
-                    #detect which library we are using and open the image
-                    if not self._image:
-                        self._image = self._read_image(self.fp)
-                        self.check_pil_image_size(self._image)
-                    if getattr(self._image,'format',None)=='JPEG': self.jpeg_fh = self._jpeg_fh
-                else:
-                    from reportlab.pdfbase.pdfutils import readJPEGInfo
-                    try:
-                        self._width,self._height, c, dpi = readJPEGInfo(self.fp)
-                    except:
-                        annotateException('\nImaging Library not available, unable to import bitmaps only jpegs\nfileName=%r identity=%s'%(fileName,self.identity()))
-                    size = self._width*self._height*c
-                    if self._max_image_size is not None and size>self._max+image_size:
-                        raise MemoryError('JPEG %s color %s x %s image would use %s > %s bytes'
-                                            %(c,self._width,self._height,size,self._max_image_size))
+                if imageReaderFlags != 0:
+                    raise ValueError('imageReaderFlags values other than 0 are no longer supported; all images are interned now')
+                fp = open_for_read(fileName,'b')
+                if not isinstance(fp, BytesIO):
+                    tfp, fp = fp, BytesIO(fp.read())
+                    tfp.close()
+                    del tfp
+                self.fp = fp
+                self._image = self._read_image(self.fp)
+                self._image.fileName = fileName if isinstance(fileName,str) else repr(fileName)
+                self.check_pil_image_size(self._image)
+                if getattr(self._image,'format',None)=='JPEG':
                     self.jpeg_fh = self._jpeg_fh
-                    self._data = self.fp.read()
-                    self._dataA=None
-                    self.fp.seek(0)
             except:
                 annotateException('\nfileName=%r identity=%s'%(fileName,self.identity()))
 
     def identity(self):
         '''try to return information that will identify the instance'''
         fn = self.fileName
         if not isStr(fn):
@@ -779,21 +738,15 @@
                 except:
                     return None
             return palette[transparency:transparency+3]
         else:
             return None
 
 class LazyImageReader(ImageReader): 
-    def fp(self): 
-        return open_for_read(self.fileName, 'b') 
-    fp=property(fp) 
-
-    def _image(self):
-        return self._read_image(self.fp)
-    _image=property(_image) 
+    pass #now same as base class since we intern everything
 
 def getImageData(imageFileName):
     "Get width, height and RGB pixels from image file.  Wraps PIL"
     try:
         return imageFileName.getImageData()
     except AttributeError:
         return ImageReader(imageFileName).getImageData()
```

### Comparing `reportlab-3.6.9/src/reportlab/lib/validators.py` & `reportlab-4.0.0/src/reportlab/lib/validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/lib/yaml.py` & `reportlab-4.0.0/src/reportlab/lib/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_can_cmap_data.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_can_cmap_data.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_cidfontdata.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_cidfontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_macexpert.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_macroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_standard.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_winansi.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courier.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courier.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courierbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helvetica.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_timesroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/_glyphlist.py` & `reportlab-4.0.0/src/reportlab/pdfbase/_glyphlist.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/acroform.py` & `reportlab-4.0.0/src/reportlab/pdfbase/acroform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/cidfonts.py` & `reportlab-4.0.0/src/reportlab/pdfbase/cidfonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 
 This defines classes to represent CID fonts.  They know how to calculate
 their own width and how to write themselves into PDF files."""
 
 import os
 import marshal
 import time
-try:
-    from hashlib import md5
-except ImportError:
-    from md5 import md5
+from hashlib import md5
 
 from reportlab.pdfbase import pdfmetrics
 from reportlab.pdfbase._cidfontdata import allowedTypeFaces, allowedEncodings, CIDFontInfo, \
      defaultUnicodeEncodings, widthsByUnichar
 from reportlab.pdfgen.canvas import Canvas
 from reportlab.pdfbase import pdfdoc
 from reportlab.lib.rl_accel import escapePDF
```

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/pdfdoc.py` & `reportlab-4.0.0/src/reportlab/pdfbase/pdfdoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#Copyright ReportLab Europe Ltd. 2000-2017
+#Copyright ReportLab Europe Ltd. 2000-2023
 #see license.txt for license details
 #history https://hg.reportlab.com/hg-public/reportlab/log/tip/src/reportlab/pdfbase/pdfdoc.py
-__version__='3.4.1'
+__version__='3.6.0'
 __doc__="""
 The module pdfdoc.py handles the 'outer structure' of PDF documents, ensuring that
 all objects are properly cross-referenced and indexed to the nearest byte.  The
 'inner structure' - the page descriptions - are presumed to be generated before
 each page is saved.
 pdfgen.py calls this and provides a 'canvas' object to handle page marking operators.
 piddlePDF calls pdfgen and offers a high-level interface.
@@ -994,15 +994,16 @@
     # to override, set as attributes
     __Defaults__ = {"Type": PDFName("Catalog"),
                 "PageMode": PDFName("UseNone"),
                 "Lang": None,
                 }
     __NoDefault__ = """
         Dests Outlines Pages Threads AcroForm Names OpenAction PageMode URI
-        ViewerPreferences PageLabels PageLayout JavaScript StructTreeRoot SpiderInfo""".split()
+        ViewerPreferences PageLabels PageLayout JavaScript StructTreeRoot SpiderInfo
+        MarkInfo Metadata Tabs""".split()
     __Refs__ = __NoDefault__
 
     def format(self, document):
         self.check_format(document)
         defaults = self.__Defaults__
         Refs = self.__Refs__
         D = {}
```

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/pdfform.py` & `reportlab-4.0.0/src/reportlab/pdfbase/pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/pdfmetrics.py` & `reportlab-4.0.0/src/reportlab/pdfbase/pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/pdfpattern.py` & `reportlab-4.0.0/src/reportlab/pdfbase/pdfpattern.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/pdfutils.py` & `reportlab-4.0.0/src/reportlab/pdfbase/pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/rl_codecs.py` & `reportlab-4.0.0/src/reportlab/pdfbase/rl_codecs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfbase/ttfonts.py` & `reportlab-4.0.0/src/reportlab/pdfbase/ttfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfgen/canvas.py` & `reportlab-4.0.0/src/reportlab/pdfgen/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,21 @@
     def pushCopy(self):
         '''the states must be shared across push/pop, but the values not'''
         x = self.__class__()
         x._d = self._d.copy()
         x._c = self._c
         return x
 
+def _gradientExtendStr(extend):
+    if isinstance(extend,(list,tuple)):
+        if len(extend)!=2:
+            raise ValueError('wrong length for extend argument' % extend)
+        return "[%s %s]" % ['true' if _ else 'false' for _ in extend]
+    return "[true true]" if extend else "[false false]"
+
 class Canvas(_PDFColorSetter):
     """This class is the programmer's interface to the PDF file format.  Methods
     are (or will be) provided here to do just about everything PDF can do.
 
     The underlying model to the canvas concept is that of a graphics state machine
     that at any given point in time has a current font, fill color (for figure
     interiors), stroke color (for figure borders), line width and geometric transform, among
@@ -863,15 +870,16 @@
 
     ######################################################
     #
     #   Image routines
     #
     ######################################################
     def drawInlineImage(self, image, x,y, width=None,height=None,
-            preserveAspectRatio=False,anchor='c', anchorAtXY=False, showBoundary=False):
+            preserveAspectRatio=False,anchor='c', anchorAtXY=False, showBoundary=False,
+            extraReturn=None):
         """See drawImage, which should normally be used instead... 
         
         drawInlineImage behaves like drawImage, but stores the image content
         within the graphics stream for the page.  This means that the mask
         parameter for transparency is not available.  It also means that there 
         is no saving in file size or time if the same image is reused.  
         
@@ -882,19 +890,21 @@
         """
     
         self._currentPageHasImages = 1
         from reportlab.pdfgen.pdfimages import PDFImage
         img_obj = PDFImage(image, x,y, width, height)
         img_obj.drawInlineImage(self,
             preserveAspectRatio=preserveAspectRatio, 
-            anchor=anchor,anchorAtXY=anchorAtXY,showBoundary=showBoundary)
+            anchor=anchor,anchorAtXY=anchorAtXY,showBoundary=showBoundary,
+            extraReturn=extraReturn)
         return (img_obj.width, img_obj.height)
 
     def drawImage(self, image, x, y, width=None, height=None, mask=None, 
-            preserveAspectRatio=False, anchor='c', anchorAtXY=False, showBoundary=False):
+            preserveAspectRatio=False, anchor='c', anchorAtXY=False, showBoundary=False,
+            extraReturn=None):
         """Draws the image (ImageReader object or filename) as specified.
 
         "image" may be an image filename or an ImageReader object. 
  
         x and y define the lower left corner of the image you wish to
         draw (or of its bounding box, if using preserveAspectRation below).
          
@@ -999,18 +1009,22 @@
         # scale and draw
         self.saveState()
         self.translate(x, y)
         self.scale(width, height)
         self._code.append("/%s Do" % regName)
         self.restoreState()
         if showBoundary:
-            self.rect(x,y,width,height,stroke=1,fill=0)
+            #self.rect(x,y,width,height,stroke=1,fill=0)
+            self.drawBoundary(showBoundary,x,y,width,height)
 
         # track what's been used on this page
         self._formsinuse.append(name)
+        if extraReturn:
+            for k in extraReturn.keys():
+                extraReturn[k] = vars()[k]
 
         return (imgObj.width, imgObj.height)
 
     def _restartAccumulators(self):
         if self._codeStack:
             # restore the saved code
             self._code, self._formsinuse, self._annotationrefs, self._formData,self._colorsUsed, self._shadingUsed = self._codeStack.pop(-1)
@@ -1553,33 +1567,25 @@
         self._code.append('/%s sh' % name)
 
     def linearGradient(self, x0, y0, x1, y1, colors, positions=None, extend=True):
         #this code contributed by Peter Johnson <johnson.peter@gmail.com>
         from reportlab.pdfbase.pdfdoc import PDFAxialShading
         colorSpace, ncolors = _normalizeColors(colors)
         fcn = _buildColorFunction(ncolors, positions)
-        if extend:
-            extendStr = "[true true]"
-        else:
-            extendStr = "[false false]"
         shading = PDFAxialShading(x0, y0, x1, y1, Function=fcn,
-                ColorSpace=colorSpace, Extend=extendStr)
+                ColorSpace=colorSpace, Extend=_gradientExtendStr(extend))
         self.shade(shading)
 
     def radialGradient(self, x, y, radius, colors, positions=None, extend=True):
         #this code contributed by Peter Johnson <johnson.peter@gmail.com>
         from reportlab.pdfbase.pdfdoc import PDFRadialShading
         colorSpace, ncolors = _normalizeColors(colors)
         fcn = _buildColorFunction(ncolors, positions)
-        if extend:
-            extendStr = "[true true]"
-        else:
-            extendStr = "[false false]"
         shading = PDFRadialShading(x, y, 0.0, x, y, radius, Function=fcn,
-                ColorSpace=colorSpace, Extend=extendStr)
+                ColorSpace=colorSpace, Extend=_gradientExtendStr(extend))
         self.shade(shading)
 
         ##################################################
         #
         #  Text methods
         #
         # As with graphics, a separate object ensures that
```

### Comparing `reportlab-3.6.9/src/reportlab/pdfgen/pathobject.py` & `reportlab-4.0.0/src/reportlab/pdfgen/pathobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfgen/pdfgeom.py` & `reportlab-4.0.0/src/reportlab/pdfgen/pdfgeom.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/pdfgen/pdfimages.py` & `reportlab-4.0.0/src/reportlab/pdfgen/pdfimages.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import os
 import reportlab
 from reportlab import rl_config
 from reportlab.pdfbase import pdfutils
 from reportlab.pdfbase import pdfdoc
-from reportlab.lib.utils import haveImages, isStr
+from reportlab.lib.utils import isStr
 from reportlab.lib.rl_accel import fp_str, asciiBase85Encode
 from reportlab.lib.boxstuff import aspectRatioFix
 
 
 class PDFImage:
     """Wrapper around different "image sources".  You can make images
     from a PIL Image object, a filename (in which case it uses PIL),
@@ -70,15 +70,14 @@
         pdfutils._chunker(data,imagedata)
         imagedata.append('EI')
         return (imagedata, imgwidth, imgheight)
 
     def cache_imagedata(self):
         image = self.image
         if not pdfutils.cachedImageExists(image):
-            if not haveImages: return
             pdfutils.cacheImageFile(image)
 
         #now we have one cached, slurp it in
         cachedname = os.path.splitext(image)[0] + (rl_config.useA85 and '.a85' or '.bin')
         imagedata = open(cachedname,'rb').readlines()
         #trim off newlines...
         imagedata = list(map(str.strip, imagedata))
@@ -157,32 +156,38 @@
             imagedata, imgwidth, imgheight = self.PIL_imagedata()
         self.imageData = imagedata
         self.imgwidth = imgwidth
         self.imgheight = imgheight
         self.width = self.width or imgwidth
         self.height = self.height or imgheight
 
-    def drawInlineImage(self, canvas, preserveAspectRatio=False,anchor='sw', anchorAtXY=False, showBoundary=False):
+    def drawInlineImage(self, canvas, preserveAspectRatio=False,anchor='sw', anchorAtXY=False,
+                     showBoundary=False, extraReturn=None):
         """Draw an Image into the specified rectangle.  If width and
         height are omitted, they are calculated from the image size.
         Also allow file names as well as images.  This allows a
         caching mechanism"""
         width = self.width
         height = self.height
         if width<1e-6 or height<1e-6: return False
         x,y,self.width,self.height, scaled = aspectRatioFix(preserveAspectRatio,anchor,self.x,self.y,width,height,self.imgwidth,self.imgheight,anchorAtXY)
         # this says where and how big to draw it
         if not canvas.bottomup: y = y+height
         canvas._code.append('q %s 0 0 %s cm' % (fp_str(self.width), fp_str(self.height, x, y)))
+        width = self.width
+        height = self.height
         # self._code.extend(imagedata) if >=python-1.5.2
         for line in self.imageData:
             canvas._code.append(line)
         canvas._code.append('Q')
         if showBoundary:
             canvas.drawBoundary(showBoundary,x,y,width,height)
+        if extraReturn:
+            for k in extraReturn.keys():
+                extraReturn[k] = vars()[k]
         return True
 
     def format(self, document):
         """Allow it to be used within pdfdoc framework.  This only
         defines how it is stored, not how it is drawn later."""
 
         dict = pdfdoc.PDFDictionary()
```

### Comparing `reportlab-3.6.9/src/reportlab/pdfgen/textobject.py` & `reportlab-4.0.0/src/reportlab/pdfgen/textobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/doctemplate.py` & `reportlab-4.0.0/src/reportlab/platypus/doctemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,17 @@
     def __new__(cls,value,onDraw,label,kind=None):
         self = str.__new__(cls,value)
         self.onDraw = onDraw
         self.kind = kind
         self.label = label
         return self
 
+    def __getnewargs__(self):
+        return str(self),self.onDraw,self.label,self.kind
+
 class PageAccumulator:
     '''gadget to accumulate information in a page
     and then allow it to be interrogated at the end
     of the page'''
     _count = 0
     def __init__(self,name=None):
         if name is None:
```

### Comparing `reportlab-3.6.9/src/reportlab/platypus/figures.py` & `reportlab-4.0.0/src/reportlab/platypus/figures.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/flowables.py` & `reportlab-4.0.0/src/reportlab/platypus/flowables.py`

 * *Files 1% similar despite different names*

```diff
@@ -690,15 +690,15 @@
         if not hasattr(KeepTogether,'NullActionFlowable'):
             #cache these on the class
             from reportlab.platypus.doctemplate import NullActionFlowable
             from reportlab.platypus.doctemplate import FrameBreak
             from reportlab.lib.utils import annotateException
             KeepTogether.NullActionFlowable = NullActionFlowable
             KeepTogether.FrameBreak = FrameBreak
-            KeepTogether.annotateException = annotateException
+            self.annotateException = annotateException
 
         if not flowables:
             flowables = [self.NullActionFlowable()]
         self._content = _flowableSublist(flowables)
         self._maxHeight = maxHeight
 
     def __repr__(self):
@@ -1277,15 +1277,15 @@
         return W, H-pS, F, []
 
     def _getContent(self,content=None):
         F = []
         C = content if content is not None else self._content
         for f in C:
             if isinstance(f,ListFlowable):
-                F.extend(self._getContent(f._content))
+                F.extend(f._getContent())
             else:
                 F.append(f)
         return F
 
 class ImageAndFlowables(_Container,_FindSplitterMixin,Flowable):
     '''combine a list of flowables and an Image'''
     def __init__(self,I,F,imageLeftPadding=0,imageRightPadding=3,imageTopPadding=0,imageBottomPadding=3,
@@ -2052,15 +2052,15 @@
 
     def __getattr__(self,a):
         if a in self._IndenterAttrs:
             try:
                 return self.__dict__[a]
             except KeyError:
                 if a not in ('spaceBefore','spaceAfter'):
-                    raise AttributeError('%r has no attribute %s' % (self,a))
+                    raise AttributeError(f'{self!r} has no attribute {a} dict={self.__dict__}')
         return getattr(self._flowable,a)
 
     def __setattr__(self,a,v):
         if a in self._IndenterAttrs:
             self.__dict__[a] = v
         else:
             setattr(self._flowable,a,v)
@@ -2209,14 +2209,15 @@
                     if v not in self._numberStyles:
                         raise ValueError('invalid bullettype=%r' % self._bulletType)
         self._start = start
         self._auto = auto or isinstance(start,(list,tuple))
 
         self._list_content = None
         self._dims = None
+        self._caption = kwds.pop('caption',None)
 
     @property
     def _content(self):
         if self._list_content is None:
             self._list_content = self._getContent()
             del self._flowables
         return self._list_content
@@ -2399,14 +2400,17 @@
             else:
                 aS(self._makeLIIndenter(f,bullet=None,params=fparams))
 
         spaceAfter = getattr(self,'spaceAfter',None)
         if spaceAfter is not None:
             f=S[-1]
             f.__dict__['spaceAfter'] = max(f.__dict__.get('spaceAfter',0),spaceAfter)
+
+        if self._caption: S.insert(0,self._caption)
+
         return S
 
 class TopPadder(Flowable):
     '''wrap a single flowable so that its first bit will be
     padded to fill out the space so that it appears at the
     bottom of its frame'''
     def __init__(self,f):
```

### Comparing `reportlab-3.6.9/src/reportlab/platypus/frames.py` & `reportlab-4.0.0/src/reportlab/platypus/frames.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/multicol.py` & `reportlab-4.0.0/src/reportlab/platypus/multicol.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/para.py` & `reportlab-4.0.0/src/reportlab/platypus/para.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/paragraph.py` & `reportlab-4.0.0/src/reportlab/platypus/paragraph.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/paraparser.py` & `reportlab-4.0.0/src/reportlab/platypus/paraparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -3159,15 +3159,15 @@
             self._iReset()
         else:
             fragList = bFragList = None
 
         return style, fragList, bFragList
 
     def _tt_handle(self,tt):
-        "Iterate through a pre-parsed tuple tree (e.g. from pyRXP)"
+        "Iterate through a pre-parsed tuple tree (e.g. from pyrxp)"
         #import pprint
         #pprint.pprint(tt)
         #find the corresponding start_tagname and end_tagname methods.
         #These must be defined.
         tag = tt[0]
         try:
             start = getattr(self,'start_'+tag)
```

### Comparing `reportlab-3.6.9/src/reportlab/platypus/tableofcontents.py` & `reportlab-4.0.0/src/reportlab/platypus/tableofcontents.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/platypus/tables.py` & `reportlab-4.0.0/src/reportlab/platypus/tables.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,16 +56,17 @@
     destination = None
     def __init__(self, name, parent=None):
         self.name = name
         if parent is not None:
             parent.copy(self)
     def copy(self, result=None):
         if result is None:
-            result = CellStyle()
+            result = CellStyle(self.name)
         for name in dir(self):
+            if name.startswith('_'): continue
             setattr(result, name, getattr(self, name))
         return result
 
 class TableStyle:
     def __init__(self, cmds=None, parent=None, **kw):
         #handle inheritance from parent first.
         if parent:
@@ -165,15 +166,15 @@
     elif xpos=='left' and ypos=='top': #top left
         xlo,yhi = corner
         P = [(xlo + r, yhi),(xlo + t, yhi), (xlo, yhi - t), (xlo, yhi - r)]
     elif xpos=='left' and ypos=='bottom': #bottom left
         xlo,ylo = corner
         P = [(xlo, ylo + r),(xlo, ylo + t), (xlo + t, ylo), (xlo + r, ylo)]
     else:
-        raise ValueError('Unknown quadrant position %s' % repr((xpos,ypos)))
+        raise ValueError(f'Unknown quadrant position (xpos,ypos)={(xpos,ypos)!r}')
     if direction=='left-right' and P[0][0]>P[-1][0] or direction=='bottom-top' and P[0][1]>P[-1][1]:
         P.reverse()
     P = _calcBezierPoints(P, kind)
     return P
 
 def _hLine(canvLine, scp, ecp, y, hBlocks, FUZZ=rl_config._FUZZ):
     '''
@@ -210,15 +211,15 @@
         return map[value]
     except KeyError:
         try:
             ivalue = int(value)
             if low<=ivalue<=high: return ivalue
         except:
             pass
-    raise ValueError('Bad %s value %s in %s'%(name,value,ascii(cmd)))
+    raise ValueError(f'Bad {name} value {value} in {cmd!a}')
 
 def _endswith(obj,s):
     try:
         return obj.endswith(s)
     except:
         return 0
 
@@ -241,55 +242,64 @@
             M[x] = M.get(x,0)+v
     for x,v in M.items():
         V[x] += v
 
 class _ExpandedCellTuple(tuple):
     pass
 
+class _ExpandedCellTupleEx(tuple):
+    def __new__(cls,seq,tagType,altText,extras):
+        self = tuple.__new__(cls,seq)
+        self.tagType = tagType
+        self.altText = altText
+        self.extras = extras
+        return self
 
 RoundingRectDef = namedtuple('RoundingRectDefs','x0 y0 w h x1 y1 ar SL')
 RoundingRectLine = namedtuple('RoundingRectLine','xs ys xe ye weight color cap dash join')
 
 class Table(Flowable):
     def __init__(self, data, colWidths=None, rowHeights=None, style=None,
-                repeatRows=0, repeatCols=0, splitByRow=1, emptyTableAction=None, ident=None,
+                repeatRows=0, repeatCols=0, splitByRow=1, splitInRow=0, emptyTableAction=None, ident=None,
                 hAlign=None,vAlign=None, normalizedData=0, cellStyles=None, rowSplitRange=None,
                 spaceBefore=None,spaceAfter=None, longTableOptimize=None, minRowHeights=None,
                 cornerRadii=__UNSET__, #or [topLeft, topRight, bottomLeft bottomRight]
+                renderCB=None,
                 ):
         self.ident = ident
         self.hAlign = hAlign or 'CENTER'
         self.vAlign = vAlign or 'MIDDLE'
         if not isinstance(data,(tuple,list)):
             raise ValueError("%s invalid data type" % self.identity())
+        self._renderCB = renderCB
         self._nrows = nrows = len(data)
         self._cellvalues = []
         _seqCW = isinstance(colWidths,(tuple,list))
         _seqRH = isinstance(rowHeights,(tuple,list))
         if nrows: self._ncols = ncols = max(list(map(_rowLen,data)))
         elif colWidths and _seqCW: ncols = len(colWidths)
         else: ncols = 0
         if not emptyTableAction: emptyTableAction = rl_config.emptyTableAction
         self._longTableOptimize = (getattr(self,'_longTableOptimize',rl_config.longTableOptimize)
                                     if longTableOptimize is None else longTableOptimize)
         if not (nrows and ncols):
             if emptyTableAction=='error':
-                raise ValueError("%s must have at least a row and column" % self.identity())
+                raise ValueError(f'{self.identity()} must have at least a row and column')
             elif emptyTableAction=='indicate':
                 self.__class__ = Preformatted
                 global _emptyTableStyle
                 if '_emptyTableStyle' not in list(globals().keys()):
                     _emptyTableStyle = ParagraphStyle('_emptyTableStyle')
                     _emptyTableStyle.textColor = colors.red
                     _emptyTableStyle.backColor = colors.yellow
                 Preformatted.__init__(self,'%s(%d,%d)' % (self.__class__.__name__,nrows,ncols), _emptyTableStyle)
             elif emptyTableAction=='ignore':
                 self.__class__ = NullActionFlowable
             else:
-                raise ValueError('%s bad emptyTableAction: "%s"' % (self.identity(),emptyTableAction))
+                raise ValueError(f'{self.identitiy()} bad emptyTableAction: {emptyTableAction!a}')
             return
 
         # we need a cleanup pass to ensure data is strings - non-unicode and non-null
         if normalizedData:
             self._cellvalues = data
         else:
             self._cellvalues = data = self.normalizeData(data)
@@ -298,25 +308,25 @@
             if rl_config.allowShortTableRows and isinstance(colWidths,list):
                 n = len(colWidths)
                 if n<ncols:
                     colWidths[n:] = (ncols-n)*[colWidths[-1]]
                 else:
                     colWidths = colWidths[:ncols]
             else:
-                raise ValueError("%s data error - %d columns in data but %d in column widths" % (self.identity(),ncols, len(colWidths)))
+                raise ValueError(f'{self.identity()} data error - {ncols} columns in data but {len(colWidths)} column widths')
         if not _seqRH: rowHeights = nrows*[rowHeights]
         elif len(rowHeights) != nrows:
-            raise ValueError("%s data error - %d rows in data but %d in row heights" % (self.identity(),nrows, len(rowHeights)))
+            raise ValueError(f'{self.identity()} data error - {nrows} rows in data but {len(rowHeights)} row heights')
         for i,d in enumerate(data):
             n = len(d)
             if n!=ncols:
                 if rl_config.allowShortTableRows and isinstance(d,list):
                     d[n:] = (ncols-n)*['']
                 else:
-                    raise ValueError("%s expected %d not %d columns in row %d!" % (self.identity(),ncols,n,i))
+                    raise ValueError(f'{self.identity()} expected {ncols} not {n} columns in row {i}!')
         self._rowHeights = self._argH = rowHeights
         self._colWidths = self._argW = colWidths
         if cellStyles is None:
             cellrows = []
             for i in range(nrows):
                 cellcols = []
                 for j in range(ncols):
@@ -332,14 +342,15 @@
         self._nosplitCmds = []
         self._srflcmds = []
         # NB repeatRows can be a list or tuple eg (1,) repeats only the second row of a table
         # or an integer eg 2 to repeat both rows 0 & 1
         self.repeatRows = repeatRows
         self.repeatCols = repeatCols
         self.splitByRow = splitByRow
+        self.splitInRow = splitInRow
 
         if style:
             self.setStyle(style)
 
         if cornerRadii is not __UNSET__:    #instance argument overrides
             self._setCornerRadii(cornerRadii)
 
@@ -348,15 +359,15 @@
             self.spaceBefore = spaceBefore
         if spaceAfter is not None:
             self.spaceAfter = spaceAfter
             
         if minRowHeights != None:
             lmrh = len(minRowHeights)
             if not lmrh:
-                raise ValueError("%s Supplied mismatching minimum row heights of length %d" % (self.identity(),lmrh))
+                raise ValueError('{self.idenity()} Supplied mismatching minimum row heights of length {lmrh}')
             elif lmrh<nrows:
                 minRowHeights = minRowHeights+(nrows-lmrh)*minRowHeights.__class__((0,))
         self._minRowHeights = minRowHeights
 
 
     def __repr__(self):
         "incomplete, but better than nothing"
@@ -433,41 +444,52 @@
         for c in C:
             if getattr(c,'__split_only__',None):
                 for d in c.splitOn(canv,aW,aH):
                     yield d
             else:
                 yield c
 
-    def _cellListProcess(self,C,aW,aH):
-        if not isinstance(C,_ExpandedCellTuple):
+    def _cellListProcess(self,v,aW,aH):
+        if isinstance(v,_ExpandedCellTuple):
+            C = v
+        else:
+            C = (v,) if isinstance(v,Flowable) else flatten(v)
             frame = None
             R = [].append
             for c in self._cellListIter(C,aW,aH):
                 if isinstance(c,Indenter):
                     if not frame:
                         frame = CellFrame(_leftExtraIndent=0,_rightExtraIndent=0)
                     c.frameAction(frame)
                     if frame._leftExtraIndent<1e-8 and frame._rightExtraIndent<1e-8:
                         frame = None
                     continue
                 if frame:
                     R(LIIndenter(c,leftIndent=frame._leftExtraIndent,rightIndent=frame._rightExtraIndent))
                 else:
                     R(c)
-            C = _ExpandedCellTuple(R.__self__)
+            if hasattr(v,'tagType'):
+                C = _ExpandedCellTupleEx(R.__self__,v.tagType,v.altText,v.extras)
+            else:
+                C = _ExpandedCellTuple(R.__self__)
+
         return C
 
     def _listCellGeom(self, V,w,s,W=None,H=None,aH=72000):
         if not V: return 0,0
         aW = w - s.leftPadding - s.rightPadding
         aH = aH - s.topPadding - s.bottomPadding
         t = 0
         w = 0
         canv = getattr(self,'canv',None)
         sb0 = None
+        if isinstance(V, str):
+            vw = self._elementWidth(V, s)
+            vh = len(V.split('\n'))*s.fontsize*1.2
+            return max(w, vw), vh
         for v in V:
             vw, vh = v.wrapOn(canv, aW, aH)
             sb = v.getSpaceBefore()
             sa = v.getSpaceAfter()
             if W is not None: W.append(vw)
             if H is not None: H.append(vh)
             w = max(w,vw)
@@ -513,15 +535,15 @@
                     ji = j,i
                     span = spanRanges.get(ji,None)
                     if ji in colSpanCells and not span: #if the current cell is part of a spanned region,
                         t = 0.0                         #assume a zero size.
                     else:#work out size
                         t = self._elementWidth(v,s)
                         if t is None:
-                            raise ValueError("Flowable %s in cell(%d,%d) can't have auto width\n%s" % (v.identity(30),i,j,self.identity(30)))
+                            raise ValueError(f'Flowable {v.identity()} in cell({i},{j}) can\'t have auto width\n{self.identity(30)}')
                         t += s.leftPadding+s.rightPadding
                         if span:
                             c0 = span[0]
                             c1 = span[2]
                             if c0!=c1:
                                 x = c0,c1
                                 spanCons[x] = max(spanCons.get(x,t),t)
@@ -618,19 +640,17 @@
                 for j,(v, s, w) in enumerate(list(zip(V, S, W))): # value, style, width (lengths must match)
                     ji = j,i
                     span = spanRanges.get(ji,None)
                     if ji in rowSpanCells and not span:
                         continue # don't count it, it's either occluded or unreliable
                     else:
                         if isinstance(v,(tuple,list,Flowable)):
-                            if isinstance(v,Flowable): v = (v,)
-                            else: v = flatten(v)
                             v = V[j] = self._cellListProcess(v,w,None)
                             if w is None and not self._canGetWidth(v):
-                                raise ValueError("Flowable %s in cell(%d,%d) can't have auto width in\n%s" % (v[0].identity(30),i,j,self.identity(30)))
+                                raise ValueError(f'Flowable {v[0].identity()} in cell({i},{j}) can\'t have auto width\n{self.identity(30)}')
                             if canv: canv._fontname, canv._fontsize, canv._leading = s.fontname, s.fontsize, s.leading or 1.2*s.fontsize
                             if ji in colSpanCells:
                                 if not span: continue
                                 w = max(colpositions[span[2]+1]-colpositions[span[0]],w or 0)
                             dW,t = self._listCellGeom(v,w or self._listValueWidth(v),s)
                             if canv: canv._fontname, canv._fontsize, canv._leading = saved
                             dW = dW + s.leftPadding + s.rightPadding
@@ -1104,15 +1124,15 @@
             self._spanCmds.append(cmd)
         elif cmd[0] == 'NOSPLIT':
             # we expect op, start, stop
             self._nosplitCmds.append(cmd)
         elif _isLineCommand(cmd):
             # we expect op, start, stop, weight, colour, cap, dashes, join
             cmd = list(cmd)
-            if len(cmd)<5: raise ValueError('bad line command '+ascii(cmd))
+            if len(cmd)<5: raise ValueError(f'bad line command {cmd!a}')
 
             #determine line cap value at position 5. This can be str or numeric.
             if len(cmd)<6:
                 cmd.append(1)
             else:
                 cap = _convert2int(cmd[5], LINECAPS, 0, 2, 'cap', cmd)
                 cmd[5] = cap
@@ -1195,24 +1215,24 @@
                     cdash = dash
                 if join is not None and cjoin!=join:
                     canv.setLineJoin(join)
                     cjoin = join
                 sc, ec, sr, er = self.normCellRange(sc,ec,sr,er)
                 getattr(self,_LineOpMap.get(op, '_drawUnknown' ))( (sc, sr), (ec, er), weight, color, count, space)
         finally:
-            if rrd: 
+            if rrd:
                 canv.line = ocanvline
         canv.restoreState()
         self._curcolor = None
 
     def _drawUnknown(self,  start, end, weight, color, count, space):
         #we are only called from _drawLines which is one level up
         import sys
         op = sys._getframe(1).f_locals['op']
-        raise ValueError("Unknown line command '%s'" % op)
+        raise ValueError(f'Unknown line command {op!a}')
 
     def _drawGrid(self, start, end, weight, color, count, space):
         self._drawBox( start, end, weight, color, count, space)
         self._drawInnerGrid( start, end, weight, color, count, space)
 
     def _drawBox(self,  start, end, weight, color, count, space):
         sc,sr = start
@@ -1352,52 +1372,105 @@
                 sr = er = n
             if er>=0 and er<n: continue
             if sr>=0 and sr<n: sr=0
             if sr>=n: sr -= n
             if er>=n: er -= n
             self._addCommand((c[0],)+((sc, sr), (ec, er))+tuple(c[3:]))
 
-    def _splitRows(self,availHeight):
-        n=self._getFirstPossibleSplitRowPosition(availHeight)
-        repeatRows = self.repeatRows
-        if n<= (repeatRows if isinstance(repeatRows,int) else (max(repeatRows)+1)): return []
-        lim = len(self._rowHeights)
-        if n==lim: return [self]
+    def _splitCell(self, value, style, oldHeight, newHeight, width):
+        # Content height of the new top row
+        height0 = newHeight - style.topPadding
+        # Content height of the new bottom row
+        height1 = oldHeight - (style.topPadding + newHeight)
+
+        if isinstance(value, (tuple, list)):
+            newCellContent = []
+            postponedContent = []
+            split = False
+            cellHeight = self._listCellGeom(value, width, style)[1]
+
+            if style.valign == "MIDDLE":
+                usedHeight = (oldHeight - cellHeight) / 2
+            else:
+                usedHeight = 0
+
+            for flowable in value:
+                if split:
+                    if flowable.height <= height1:
+                        postponedContent.append(flowable)
+                        # Shrink the available height:
+                        height1 -= flowable.height
+                    else:
+                        # The content doesn't fit after the split:
+                        return []
+                elif usedHeight + flowable.height <= height0:
+                    newCellContent.append(flowable)
+                    usedHeight += flowable.height
+                else:
+                    # This is where we need to split
+                    splits = flowable.split(width, height0-usedHeight)
+                    if splits:
+                        newCellContent.append(splits[0])
+                        postponedContent.append(splits[1])
+                    else:
+                        # We couldn't split this flowable at the desired
+                        # point. If we already has added previous paragraphs
+                        # to the content, just add everything after the split.
+                        # Also try adding it after the split if valign isn't TOP
+                        if newCellContent or style.valign != "TOP":
+                            if flowable.height <= height1:
+                                postponedContent.append(flowable)
+                                # Shrink the available height:
+                                height1 -= flowable.height
+                            else:
+                                # The content doesn't fit after the split:
+                                return []
+                        else:
+                            # We could not split this, so we fail:
+                            return []
 
-        lo = self._rowSplitRange
-        if lo:
-            lo, hi = lo
-            if lo<0: lo += lim
-            if hi<0: hi += lim
-            if n>hi:
-                return self._splitRows(availHeight - sum(self._rowHeights[hi:n]))
-            elif n<lo:
+                    split = True
+
+            return (tuple(newCellContent), tuple(postponedContent))
+
+        elif isinstance(value, str):
+            rows = value.split("\n")
+            lineHeight = 1.2 * style.fontsize
+            contentHeight = (style.leading or lineHeight) * len(rows)
+            if style.valign == "TOP" and contentHeight <= height0:
+                # This fits in the first cell, all is good
+                return (value, '')
+            elif style.valign == "BOTTOM" and contentHeight <= height1:
+                # This fits in the second cell, all is good
+                return ('', value)
+            elif style.valign == "MIDDLE":
+                # Put it in the largest cell:
+                if height1 > height0:
+                    return ('', value)
+                else:
+                    return (value, '')
+
+            elif len(rows) < 2:
+                # It doesn't fit, and there's nothing to split: Fail
                 return []
+            # We need to split this, and there are multiple lines, so we can
+            if style.valign == "TOP":
+                splitPoint = height0 // lineHeight
+            elif style.valign == "BOTTOM":
+                splitPoint = len(rows) - (height1 // lineHeight)
+            else:  # MID
+                splitPoint = (height0 - height1 + contentHeight) // (2 * lineHeight)
 
-        repeatCols = self.repeatCols
-        splitByRow = self.splitByRow
-        data = self._cellvalues
+            splitPoint = int(splitPoint)
+            return ('\n'.join(rows[:splitPoint]), '\n'.join(rows[splitPoint:]))
 
-        #we're going to split into two superRows
-        ident = self.ident
-        if ident: ident = IdentStr(ident)
-        lto = self._longTableOptimize
-        if lto:
-            splitH = self._rowHeights
-        else:
-            splitH = self._argH
-        cornerRadii = getattr(self,'_cornerRadii',None)
-        R0 = self.__class__( data[:n], colWidths=self._colWidths, rowHeights=splitH[:n],
-                repeatRows=repeatRows, repeatCols=repeatCols,
-                splitByRow=splitByRow, normalizedData=1, cellStyles=self._cellStyles[:n],
-                ident=ident,
-                spaceBefore=getattr(self,'spaceBefore',None),
-                longTableOptimize=lto,
-                cornerRadii=cornerRadii[:2] if cornerRadii else None)
+        # No content
+        return ('', '')
 
+    def _splitLineCmds(self, n, doInRowSplit=0):
         nrows = self._nrows
         ncols = self._ncols
         #copy the commands
         A = []
         # hack up the line commands
         for op, (sc,sr), (ec,er), weight, color, cap, dash, join, count, space in self._linecmds:
             if isinstance(sr,strTypes) and sr.startswith('split'):
@@ -1410,101 +1483,565 @@
 
             if sc < 0: sc += ncols
             if ec < 0: ec += ncols
             if sr < 0: sr += nrows
             if er < 0: er += nrows
 
             if op in ('BOX','OUTLINE','GRID'):
-                if sr<n and er>=n:
+                if (sr<n and er>=n) or (doInRowSplit and sr==n):
                     # we have to split the BOX
                     A.append(('LINEABOVE',(sc,sr), (ec,sr), weight, color, cap, dash, join, count, space))
                     A.append(('LINEBEFORE',(sc,sr), (sc,er), weight, color, cap, dash, join, count, space))
                     A.append(('LINEAFTER',(ec,sr), (ec,er), weight, color, cap, dash, join, count, space))
                     A.append(('LINEBELOW',(sc,er), (ec,er), weight, color, cap, dash, join, count, space))
                     if op=='GRID':
-                        A.append(('LINEBELOW',(sc,n-1), (ec,n-1), weight, color, cap, dash, join, count, space))
-                        A.append(('LINEABOVE',(sc,n), (ec,n), weight, color, cap, dash, join, count, space))
-                        A.append(('INNERGRID',(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
+                        if doInRowSplit:
+                            A.append(('INNERGRID',(sc,sr), (ec,n-1), weight, color, cap, dash, join, count, space))
+                            A.append(('INNERGRID',(sc,n), (ec,er), weight, color, cap, dash, join, count, space))
+                        else:
+                            A.append(('LINEBELOW',(sc,n-1), (ec,n-1), weight, color, cap, dash, join, count, space))
+                            A.append(('LINEABOVE',(sc,n), (ec,n), weight, color, cap, dash, join, count, space))
+                            A.append(('INNERGRID',(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
                 else:
                     A.append((op,(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
             elif op == 'INNERGRID':
-                if sr<n and er>=n:
+                if sr<n and er>=n and not doInRowSplit:
                     A.append(('LINEBELOW',(sc,n-1), (ec,n-1), weight, color, cap, dash, join, count, space))
                     A.append(('LINEABOVE',(sc,n), (ec,n), weight, color, cap, dash, join, count, space))
                 A.append((op,(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
             elif op == 'LINEBELOW':
                 if sr<n and er>=(n-1):
                     A.append(('LINEABOVE',(sc,n), (ec,n), weight, color, cap, dash, join, count, space))
                 A.append((op,(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
             elif op == 'LINEABOVE':
                 if sr<=n and er>=n:
                     A.append(('LINEBELOW',(sc,n-1), (ec,n-1), weight, color, cap, dash, join, count, space))
                 A.append((op,(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
             else:
                 A.append((op,(sc,sr), (ec,er), weight, color, cap, dash, join, count, space))
 
-        R0._cr_0(n,A,nrows)
-        R0._cr_0(n,self._bkgrndcmds,nrows,_srflMode=True)
-        R0._cr_0(n,self._spanCmds,nrows)
-        R0._cr_0(n,self._nosplitCmds,nrows)
-        for c in self._srflcmds:
+        return A
+
+    def _stretchCommands(self, n, cmds, oldrowcount):
+        """Stretches the commands when a row is split
+
+        The row start is sr, the row end is er.
+
+         sr   | er  | result
+        ---------------------------------------------------------------------
+          <n  |  <n | Do nothing.
+              | >=n | A command that spans the break, extend end.
+        ---------------------------------------------------------------------
+         ==n  | ==n | Zero height. Extend the end, unless it's a LINEABOVE
+              |     | commands, it's between rows so do nothing.
+              |     | For LINEBELOW increase both.
+              |  >n | A command that spans the break, extend end.
+        ---------------------------------------------------------------------
+          >n  |  >n | This command comes after the break, increase both.
+        ---------------------------------------------------------------------
+
+        Summary:
+        1. If er > n then increase er
+        2. If sr > n then increase sr
+        3. If er == n and sr < n, increase er
+        4. If er == sr == n and cmd is not line, increase er
+
+        """
+        stretched = []
+        for c in cmds:
+            cmd, (sc,sr), (ec,er) = c[0:3]
+
+            if sr in ("splitlast", "splitfirst") or er in ("splitlast", "splitfirst"):
+                stretched.append(c)
+                continue
+
+            if er < 0:
+                er += oldrowcount
+            if sr < 0:
+                sr += oldrowcount
+
+            if er > n:
+                er += 1
+            elif  er == n:
+                if sr < n or (sr == n and cmd != "LINEABOVE"):
+                    er += 1
+
+            if sr > n or (sr == n and cmd == "LINEBELOW"):
+                sr += 1
+
+            stretched.append((c[0], (sc,sr), (ec,er)) + c[3:])
+
+        return stretched
+
+    def _splitRows(self,availHeight,doInRowSplit=0):
+        # Get the split position. if we split between rows (doInRowSplit=0),
+        # then n will be the first row after the split. If we split a row,
+        # then n is the row we split in two.
+        n=self._getFirstPossibleSplitRowPosition(availHeight,ignoreSpans=doInRowSplit)
+
+        # We can't split before or in the repeatRows/headers
+        repeatRows = self.repeatRows
+        maxrepeat = repeatRows if isinstance(repeatRows,int) else max(repeatRows)+1
+        if doInRowSplit and n<maxrepeat or not doInRowSplit and n<=maxrepeat:
+            return []
+
+        # If the whole table fits, return it
+        lim = len(self._rowHeights)
+        if n==lim: return [self]
+
+        lo = self._rowSplitRange
+        if lo:
+            lo, hi = lo
+            if lo<0: lo += lim
+            if hi<0: hi += lim
+            if n>hi:
+                return self._splitRows(availHeight - sum(self._rowHeights[hi:n]), doInRowSplit=doInRowSplit)
+            elif n<lo:
+                return []
+
+        repeatCols = self.repeatCols
+
+        if not doInRowSplit:
+            T = self
+            data = self._cellvalues
+        else:
+            data = [_[:] for _ in self._cellvalues]
+            # We are splitting the n row into two, if possible.
+            # We can't split if the available height is less than the minimum set:
+            if self._minRowHeights and availHeight < self._minRowHeights[n]:
+                return []
+
+            usedHeights = sum(self._rowHeights[:n])
+
+            cellvalues = self._cellvalues[n]
+            cellStyles = self._cellStyles[n]
+            cellWidths = self._colWidths
+            curRowHeight = self._rowHeights[n]
+
+            # First find the min/max split point
+            minSplit = 0  # Counted from top
+            maxSplit = 0  # Counted from bottom
+            maxHeight = 0
+
+            for column, (value, style, width) in enumerate(zip(cellvalues, cellStyles, cellWidths)):
+                if self._spanCmds and self._spanRanges.get((column, n), None) is None:
+                    # This is part of another cell span, the value will not be displayed
+                    continue
+
+                if isinstance(value, (tuple, list)):
+                    # A sequence of flowables:
+                    w, height = self._listCellGeom(value, width, style)
+                    height += style.topPadding + style.bottomPadding
+                    if height > maxHeight:
+                        maxHeight = height
+                elif isinstance(value, str):
+                    rows = value.split("\n")
+                    lineHeight = 1.2 * style.fontsize
+                    height = lineHeight * len(rows) + style.topPadding + style.bottomPadding
+
+                    # Make sure we don't try to split in the middle of the first or last line
+                    minSplit = max(minSplit, lineHeight + style.topPadding)
+                    maxSplit = max(maxSplit, lineHeight + style.bottomPadding)
+
+                    if height > maxHeight:
+                        maxHeight = height
+
+            if ((minSplit + maxSplit > curRowHeight) or
+                 (minSplit > (availHeight - usedHeights))):
+                # We can't split this row. So we should fail, and let the split get retried
+                # with splitInRow = 0. However, if there is a spanned row that will also
+                # fail. So first we need to check if any cell in the current row is spanned.
+                if not self._spanCmds:
+                    # There are no spans to look at, so we can skip this and fail directly
+                    return []
+
+                splitCells = set()
+                for column in range(self._ncols):
+                    cell = (column, n)
+                    if (cell in self._rowSpanCells and
+                        self._spanRanges.get((column, n), None) is None):
+                        # This cell is a part of a rowSpan, and not the main cell.
+                        # Find the real cell and cell value
+                        for cell, span in self._spanRanges.items():
+                            if span is None:
+                                continue
+                            start_col, start_row, end_col, end_row = span
+                            if (column >= start_col and
+                                column <= end_col and
+                                n > start_row and
+                                n <= end_row):
+                                splitCells.add(cell)
+                                break
+
+                if not splitCells:
+                    # There were no spanned rows that could be split, so we fail.
+                    return []
+
+                spanCmds = []
+                for cmd, (sc, sr), (ec, er) in self._spanCmds:
+                    # -1 means last row/column, handle that here.
+                    if sc < 0:
+                        sc += self._ncols
+                    if ec < 0:
+                        ec += self._ncols
+                    if sr < 0:
+                        sr += self._nrows
+                    if er < 0:
+                        er += self._nrows
+                    spanCmds.append((cmd, (sc, sr), (ec, er)))
+
+                newCellStyles = [_[:] for _ in self._cellStyles]
+                bkgrndcmds = self._bkgrndcmds
+
+                # There are cells spanning the rows we want to split. They can be split,
+                # because the  _getFirstPossibleSplitRowPosition() call above checked
+                # that they are not in a nosplit range, so let's split them.
+                for cell in splitCells:
+                    span_sc, span_sr, span_ec, span_er = self._spanRanges[cell]
+                    spanRect = self._spanRects[cell]
+                    oldHeight = spanRect[3]
+                    newHeight = sum(self._rowHeights[span_sr:n])
+
+                    # Copy the style:
+                    oldStyle = newCellStyles[span_sr][span_sc]
+
+                    res = self._splitCell(self._cellvalues[span_sr][span_sc],
+                                          oldStyle, oldHeight, newHeight, width)
+                    if not res:
+                        # Could not split
+                        return []
+
+                    # Replace the data values:
+                    data[span_sr][span_sc] = res[0]
+                    data[n][span_sc] = res[1]
+
+                    # Now get replace the rowspan with two new rowspans, or
+                    # remove the spans if no span remains
+
+                    newSpanCmds = []
+                    for cmd, start, end in spanCmds:
+                        if ((span_sc, span_sr) == start and
+                            (span_ec, span_er) == end):
+                            # Modify this:
+                            if n-1 > span_sr or span_sc != span_ec:
+                                newSpanCmds.append((cmd, (span_sc, span_sr), (span_ec, n-1)))
+                            if n < span_er or span_sc != span_ec:
+                                newSpanCmds.append((cmd, (span_sc, n), (span_ec, span_er)))
+                        else:
+                            newSpanCmds.append((cmd, start, end))
+
+                    spanCmds = newSpanCmds
+
+                    newbkgrndcmds = []
+                    for cmd, start, end, color in bkgrndcmds:
+                        if start == (span_sc, span_sr):
+                            # The cell we are splitting has a background color command.
+                            # Add commands for the new split cells:
+                            newbkgrndcmds.append((cmd, start, (end[0], n-1), color))
+                            newbkgrndcmds.append((cmd, (start[0], n), (end[0], n), color))
+                        else:
+                            newbkgrndcmds.append((cmd, start, end, color))
+
+                    bkgrndcmds = newbkgrndcmds
+
+                    # And adjust the style
+                    newStyle = oldStyle.copy()
+                    if oldStyle.valign == "MIDDLE":
+                        # Adjust margins
+                        if res[0] and res[1]:
+                            # We split the content, so fix up the valign:
+                            oldStyle.valign = "BOTTOM"
+                            newStyle.valign = "TOP"
+                        else:
+                            # Adjust the margins to push it towards the true middle
+                            h = self._listCellGeom(v[0] or v[1], width, oldStyle)[1]
+                            margin = (curRowHeight - h) / 2
+                            if v[0]:
+                                oldStyle.topPadding += margin
+                            elif v[1]:
+                                newStyle.bottomPadding += margin
+                    newCellStyles[n][span_sc] = newStyle
+
+                # Make a new table here
+                T = self.__class__( data, colWidths=self._colWidths,
+                    rowHeights=self._rowHeights, repeatRows=self.repeatRows,
+                    repeatCols=self.repeatCols, splitByRow=self.splitByRow,
+                    splitInRow=self.splitInRow, normalizedData=1,
+                    cellStyles=newCellStyles, ident=self.ident,
+                    spaceBefore=getattr(self,'spaceBefore',None),
+                    longTableOptimize=self._longTableOptimize,
+                    cornerRadii=getattr(self,'_cornerRadii',None),
+                    renderCB=getattr(self,'_renderCB',None),
+                    )
+
+                T._bkgrndcmds = bkgrndcmds
+                T._spanCmds = spanCmds
+                T._nosplitCmds = self._nosplitCmds
+                T._srflcmds = self._srflcmds
+                T._colpositions = self._colpositions
+                T._rowpositions = self._rowpositions
+
+                T._calcNoSplitRanges()
+                T._calcSpanRanges()
+                T._calcSpanRects()
+
+                # And then, remove any lines that now appear that were inside
+                # the spanning cell before the split. First, we need to split
+                # the grids, and convert the bit of the grid that spans the
+                # split to a line.
+                newlinecmds = []
+                for linecmd in self._linecmds:
+                    op, (sc,sr), (ec,er), weight, color, cap, dash, join, count, space = linecmd
+                    # -1 means "to the end", so we handle that here
+                    if er < 0:
+                        er += T._nrows
+                    if ec < 0:
+                        ec += T._ncols
+
+                    if ((op == 'BOX') or (op == 'GRID' and (sr <= n or er >=n)) or
+                        (op == 'INNERGRID' and (sr < n or er > n))):
+
+                        if op in ('GRID', 'INNERGRID'):
+                            newlinecmds.append(('INNERGRID',(sc,sr), (ec,n-1), weight, color, cap, dash, join, count, space))
+                            newlinecmds.append(('INNERGRID',(sc,n), (ec,er), weight, color, cap, dash, join, count, space))
+                            newlinecmds.append(('LINEBELOW',(sc,n-1), (ec,n-1), weight, color, cap, dash, join, count, space))
+                        if op in ('GRID', 'BOX'):
+                            # The box must be made of lines, because  otherwise
+                            # it might not get split where it should, below.
+                            newlinecmds.append(('LINEABOVE', (sc,sr), (ec,sr), weight, color, cap, dash, join, count, space))
+                            newlinecmds.append(('LINEBELOW', (sc,er), (ec,er), weight, color, cap, dash, join, count, space))
+                            newlinecmds.append(('LINEBEFORE', (sc,sr), (sc,er), weight, color, cap, dash, join, count, space))
+                            newlinecmds.append(('LINEAFTER', (ec,sr), (ec,er), weight, color, cap, dash, join, count, space))
+                    else:
+                        newlinecmds.append(linecmd)
+                        continue
+
+                # Then secondly split any LINEABOVE and LINEBELOW so that the
+                # split cells don't get them.
+                for cell in splitCells:
+
+                    moddedcmds = []
+                    for linecmd in newlinecmds:
+                        op, (sc,sr), (ec,er), weight, color, cap, dash, join, count, space = linecmd
+                        span_sc, span_sr, span_ec, span_er = self._spanRanges[cell]
+
+                        if (((op == "LINEABOVE" and er > span_sr and sr <= span_er) or
+                           (op == "LINEBELOW" and er >= span_sr and sr < span_er)) and
+                           (sc <= span_ec and ec >= span_sc)):
+                            # This needs handling of some sort
+
+                            if op == "LINEABOVE":
+                                startrow = span_sr
+                                endrow = span_er + 1
+                            else:
+                                startrow = span_sr - 1
+                                endrow = span_er
+
+                            if sr <= startrow:
+                                # Anything before the span should be unaffected:
+                                moddedcmds.append(
+                                    (op, (sc, sr), (ec, startrow), weight, color, cap, dash, join, count, space)
+                                )
+
+                            # For any lines in between we need to remove the split cell
+                            if span_sc > sc:
+                                # The start column of the span is higher than the start column of
+                                # the line. So we need a line up until but not including the start column
+                                moddedcmds.append(
+                                    (op, (sc, max(startrow, sr)), (span_sc-1, min(er, endrow)), weight, color, cap, dash, join, count, space)
+                                )
+                            if span_ec < ec:
+                                # The start column of the span is lower than the end column of
+                                # the line. So we need a line up starting after but not including the end column
+                                moddedcmds.append(
+                                    (op, (span_ec+1, max(startrow, sr)), (ec, min(er, endrow)), weight, color, cap, dash, join, count, space)
+                                )
+
+                            if er >= endrow:
+                                moddedcmds.append(
+                                    (op, (sc, endrow), (ec, er), weight, color, cap, dash, join, count, space)
+                                )
+                                # Anything after the span should be unaffected:
+
+                        else:
+                            moddedcmds.append(linecmd)
+
+                    newlinecmds = moddedcmds
+
+                T._linecmds = newlinecmds
+
+                return T._splitRows(availHeight,doInRowSplit=False)
+
+            # This is where we split the row:
+            splitPoint = min(availHeight - usedHeights, maxHeight - maxSplit)
+            if splitPoint+1 < self.splitInRow:
+                # The height of the split is smaller than the minimum.
+                # Fail, and the whole table will be moved to the next page.
+                return []
+
+            remaining = self._height - splitPoint
+            if remaining < self.splitInRow:
+                # The remaining height of the table is smaller than the minimum.
+                # Fail, and the whole table will be moved to the next page.
+                return []
+
+            R0 = []  # Top half of the row
+            R0Height = 0  # Minimum height
+            R1 = []  # Bottom half of the row
+            R1Height = 0  # Minimum height
+            R1Styles = []
+            for (value, style, width) in zip(cellvalues, cellStyles, cellWidths):
+                v = self._splitCell(value, style, curRowHeight, splitPoint, width)
+                if not v:
+                    # Splitting the table failed
+                    return []
+
+                newStyle = style.copy()
+                if style.valign == "MIDDLE":
+                    # Adjust margins
+                    if v[0] and v[1]:
+                        # We split the content, so fix up the valign:
+                        style.valign = "BOTTOM"
+                        newStyle.valign = "TOP"
+                    else:
+                        # Adjust the margins to push it towards the true middle
+                        h = self._listCellGeom(v[0] or v[1], width, style)[1]
+                        margin = (curRowHeight - h) / 2
+                        if v[0]:
+                            style.topPadding += margin
+                        elif v[1]:
+                            newStyle.bottomPadding += margin
+                R0.append(v[0])
+                R1.append(v[1])
+                h0 = self._listCellGeom(v[0], width, style)[1] + style.topPadding + style.bottomPadding
+                R0Height = max(R0Height, h0)
+                h1 = self._listCellGeom(v[1], width, style)[1] + style.topPadding + style.bottomPadding
+                R1Height = max(R1Height, h1)
+                R1Styles.append(newStyle)
+
+            # Make a new table with the row split into two:
+            usedHeight = min(splitPoint, R0Height)
+            newRowHeight = max(R1Height, self._rowHeights[n] - usedHeight)
+            newRowHeights = self._rowHeights[:]
+            newRowHeights.insert(n + 1, newRowHeight)
+            newRowHeights[n] = usedHeight
+            newCellStyles = self._cellStyles[:]
+            newCellStyles.insert(n + 1, R1Styles)
+
+            data = data[:n] + [R0] + [R1] + data[n+1:]
+
+            T = self.__class__( data, colWidths=self._colWidths,
+                rowHeights=newRowHeights, repeatRows=self.repeatRows,
+                repeatCols=self.repeatCols, splitByRow=self.splitByRow,
+                splitInRow=self.splitInRow, normalizedData=1,
+                cellStyles=newCellStyles, ident=self.ident,
+                spaceBefore=getattr(self,'spaceBefore',None),
+                longTableOptimize=self._longTableOptimize,
+                cornerRadii=getattr(self,'_cornerRadii',None),
+                renderCB=getattr(self,'_renderCB',None),
+                )
+
+            T._linecmds = self._stretchCommands(n, self._linecmds, lim)
+            T._bkgrndcmds = self._stretchCommands(n, self._bkgrndcmds, lim)
+            T._spanCmds = self._stretchCommands(n, self._spanCmds, lim)
+            T._nosplitCmds = self._stretchCommands(n, self._nosplitCmds, lim)
+            T._srflcmds = self._stretchCommands(n, self._srflcmds, lim)
+            n = n + 1
+
+        #we're going to split into two superRows
+        ident = self.ident
+        if ident: ident = IdentStr(ident)
+        lto = T._longTableOptimize
+        if lto:
+            splitH = T._rowHeights
+        else:
+            splitH = T._argH
+
+        cornerRadii = getattr(self,'_cornerRadii',None)
+        renderCB = getattr(self,'_renderCB',None)
+        R0 = self.__class__( data[:n], colWidths=T._colWidths, rowHeights=splitH[:n],
+                repeatRows=repeatRows, repeatCols=repeatCols, splitByRow=self.splitByRow,
+                splitInRow=self.splitInRow, normalizedData=1, cellStyles=T._cellStyles[:n],
+                ident=ident,
+                spaceBefore=getattr(self,'spaceBefore',None),
+                longTableOptimize=lto,
+                cornerRadii=cornerRadii[:2] if cornerRadii else None,
+                renderCB=renderCB,
+                )
+
+        nrows = T._nrows
+        ncols = T._ncols
+
+        _linecmds = T._splitLineCmds(n, doInRowSplit=doInRowSplit)
+
+        R0._cr_0(n,_linecmds,nrows)
+        R0._cr_0(n,T._bkgrndcmds,nrows,_srflMode=True)
+        R0._cr_0(n,T._spanCmds,nrows)
+        R0._cr_0(n,T._nosplitCmds,nrows)
+
+        for c in T._srflcmds:
             R0._addCommand(c)
             if c[1][1]!='splitlast': continue
             (sc,sr), (ec,er) = c[1:3]
             R0._addCommand((c[0],)+((sc, n-1), (ec, n-1))+tuple(c[3:]))
 
         if ident: ident = IdentStr(ident)
         if repeatRows:
             if isinstance(repeatRows,int):
                 iRows = data[:repeatRows]
                 iRowH = splitH[:repeatRows]
-                iCS = self._cellStyles[:repeatRows]
+                iCS = T._cellStyles[:repeatRows]
                 repeatRows = list(range(repeatRows))
             else:
                 #we have a list of repeated rows eg (1,3)
                 repeatRows = list(sorted(repeatRows))
                 iRows = [data[i] for i in repeatRows]
                 iRowH = [splitH[i] for i in repeatRows]
-                iCS = [self._cellStyles[i] for i in repeatRows]
-            R1 = self.__class__(iRows+data[n:],colWidths=self._colWidths,
+                iCS = [T._cellStyles[i] for i in repeatRows]
+            R1 = self.__class__(iRows+data[n:],colWidths=T._colWidths,
                     rowHeights=iRowH+splitH[n:],
                     repeatRows=len(repeatRows), repeatCols=repeatCols,
-                    splitByRow=splitByRow, normalizedData=1,
-                    cellStyles=iCS+self._cellStyles[n:],
+                    splitByRow=self.splitByRow, splitInRow=self.splitInRow,
+                    normalizedData=1,
+                    cellStyles=iCS+T._cellStyles[n:],
                     ident=ident,
                     spaceAfter=getattr(self,'spaceAfter',None),
                     longTableOptimize=lto,
                     cornerRadii = cornerRadii,
+                    renderCB = renderCB,
                     )
-            R1._cr_1_1(n,nrows,repeatRows,A) #linecommands
-            R1._cr_1_1(n,nrows,repeatRows,self._bkgrndcmds,_srflMode=True)
-            R1._cr_1_1(n,nrows,repeatRows,self._spanCmds)
-            R1._cr_1_1(n,nrows,repeatRows,self._nosplitCmds)
+            R1._cr_1_1(n,nrows,repeatRows,_linecmds)
+            R1._cr_1_1(n,nrows,repeatRows,T._bkgrndcmds,_srflMode=True)
+            R1._cr_1_1(n,nrows,repeatRows,T._spanCmds)
+            R1._cr_1_1(n,nrows,repeatRows,T._nosplitCmds)
         else:
             #R1 = slelf.__class__(data[n:], self._argW, self._argH[n:],
-            R1 = self.__class__(data[n:], colWidths=self._colWidths, rowHeights=splitH[n:],
+            R1 = self.__class__(data[n:], colWidths=T._colWidths, rowHeights=splitH[n:],
                     repeatRows=repeatRows, repeatCols=repeatCols,
-                    splitByRow=splitByRow, normalizedData=1, cellStyles=self._cellStyles[n:],
+                    splitByRow=self.splitByRow, splitInRow=self.splitInRow,
+                    normalizedData=1, cellStyles=T._cellStyles[n:],
                     ident=ident,
                     spaceAfter=getattr(self,'spaceAfter',None),
                     longTableOptimize=lto,
                     cornerRadii = ([0,0] + cornerRadii[2:]) if cornerRadii else None,
+                    renderCB = renderCB,
                     )
-            R1._cr_1_0(n,A)
-            R1._cr_1_0(n,self._bkgrndcmds,_srflMode=True)
-            R1._cr_1_0(n,self._spanCmds)
-            R1._cr_1_0(n,self._nosplitCmds)
-        for c in self._srflcmds:
+
+            R1._cr_1_0(n,_linecmds)
+            R1._cr_1_0(n,T._bkgrndcmds,_srflMode=True)
+            R1._cr_1_0(n,T._spanCmds)
+            R1._cr_1_0(n,T._nosplitCmds)
+        for c in T._srflcmds:
             R1._addCommand(c)
             if c[1][1]!='splitfirst': continue
             (sc,sr), (ec,er) = c[1:3]
             R1._addCommand((c[0],)+((sc, 0), (ec, 0))+tuple(c[3:]))
 
-        R0.hAlign = R1.hAlign = self.hAlign
-        R0.vAlign = R1.vAlign = self.vAlign
+        R0.hAlign = R1.hAlign = T.hAlign
+        R0.vAlign = R1.vAlign = T.vAlign
         self.onSplit(R0)
         self.onSplit(R1)
         return [R0,R1]
 
     def _getRowImpossible(impossible,cells,ranges):
         for xy in cells:
             r=ranges[xy]
@@ -1516,17 +2053,19 @@
                     y=ymin+1
                     while 1:
                         if y>ymax: break
                         impossible[y]=None #split at position y is impossible because of overlapping rowspan
                         y+=1
     _getRowImpossible=staticmethod(_getRowImpossible)
 
-    def _getFirstPossibleSplitRowPosition(self,availHeight):
+    def _getFirstPossibleSplitRowPosition(self,availHeight,ignoreSpans=0):
+        # Returns the LAST possible split row position
         impossible={}
-        if self._spanCmds:
+        # With inRowSplits we ignore spans
+        if self._spanCmds and not ignoreSpans:
             self._getRowImpossible(impossible,self._rowSpanCells,self._spanRanges)
         if self._nosplitCmds:
             self._getRowImpossible(impossible,self._rowNoSplitCells,self._nosplitRanges)
         h = 0
         n = 1
         split_at = 0 # from this point of view 0 is the first position where the table may *always* be splitted
         for rh in self._rowHeights:
@@ -1536,27 +2075,39 @@
                 split_at=n
             h=h+rh
             n=n+1
         return split_at
 
     def split(self, availWidth, availHeight):
         self._calc(availWidth, availHeight)
-        if self.splitByRow:
+        if self.splitByRow or self.splitInRow:
             if not rl_config.allowTableBoundsErrors and self._width>availWidth: return []
-            return self._splitRows(availHeight)
-        else:
-            raise NotImplementedError
+
+            # If self.splitByRow is true, first try with doInRowSplit as false.
+            # Otherwise, first try with doInRowSplit as true
+            result = self._splitRows(availHeight, doInRowSplit=not self.splitByRow)
+            if result:
+                # That worked, return that:
+                return result
+
+            # The first attempt did NOT succeed, now try with the flag flipped
+            # (unless self.splitInRow is false)
+            if self.splitInRow:
+                return self._splitRows(availHeight, doInRowSplit=self.splitByRow)
+
+        # We can't split this table in any way, raise an error:
+        return []
 
     def _makeRoundedCornersClip(self, FUZZ=rl_config._FUZZ):
         self._roundingRectDef = None
         cornerRadii = getattr(self,'_cornerRadii',None)
         if not cornerRadii or max(cornerRadii)<=FUZZ: return
         nrows = self._nrows
         ncols = self._ncols
-        ar = [min(self._rowHeights[i],self._colWidths[j],cornerRadii[k]) for 
+        ar = [min(self._rowHeights[i],self._colWidths[j],cornerRadii[k]) for
                 k,(i,j) in enumerate((
                     (0,0),
                     (0,ncols-1),
                     (nrows-1,0),
                     (nrows-1, ncols-1),
                     ))]
         rp = self._rowpositions
@@ -1652,34 +2203,66 @@
                 P.curveTo(c1[1][0],c1[1][1],c1[2][0],c1[2][1], c1[3][0],c1[3][1])
             canv.drawPath(P, stroke=1, fill=0)
         canv.restoreState()
 
     def draw(self):
         c = self.canv
         c.saveState()
-        self._makeRoundedCornersClip()
         self._curweight = self._curcolor = self._curcellstyle = None
+        renderCB = getattr(self,'_renderCB')
+        if renderCB:
+            renderCB(self,'startTable')
+            renderCB(self,'startBG')
+        self._makeRoundedCornersClip()
         self._drawBkgrnd()
+        if renderCB: renderCB(self,'endBG')
         if not self._spanCmds:
             # old fashioned case, no spanning, steam on and do each cell
-            for row, rowstyle, rowpos, rowheight in zip(self._cellvalues, self._cellStyles, self._rowpositions[1:], self._rowHeights):
-                for cellval, cellstyle, colpos, colwidth in zip(row, rowstyle, self._colpositions[:-1], self._colWidths):
-                    self._drawCell(cellval, cellstyle, (colpos, rowpos), (colwidth, rowheight))
+            if renderCB:
+                for rowNo, (row, rowstyle, rowpos, rowheight) in enumerate(zip(self._cellvalues, self._cellStyles, self._rowpositions[1:], self._rowHeights)):
+                    renderCB(self,'startRow',rowNo)
+                    for colNo, (cellval, cellstyle, colpos, colwidth) in enumerate(zip(row, rowstyle, self._colpositions[:-1], self._colWidths)):
+                        renderCB(self,'startCell', rowNo, colNo, cellval, cellstyle, (colpos, rowpos), (colwidth, rowheight))
+                        self._drawCell(cellval, cellstyle, (colpos, rowpos), (colwidth, rowheight))
+                        renderCB(self,'endCell')
+                    renderCB(self,'endRow')
+            else:
+                for row, rowstyle, rowpos, rowheight in zip(self._cellvalues, self._cellStyles, self._rowpositions[1:], self._rowHeights):
+                    for colNo, (cellval, cellstyle, colpos, colwidth) in enumerate(zip(row, rowstyle, self._colpositions[:-1], self._colWidths)):
+                        self._drawCell(cellval, cellstyle, (colpos, rowpos), (colwidth, rowheight))
         else:
             # we have some row or col spans, need a more complex algorithm
             # to find the rect for each
-            for rowNo in range(self._nrows):
-                for colNo in range(self._ncols):
-                    cellRect = self._spanRects[colNo, rowNo]
-                    if cellRect is not None:
-                        (x, y, width, height) = cellRect
-                        cellval = self._cellvalues[rowNo][colNo]
-                        cellstyle = self._cellStyles[rowNo][colNo]
-                        self._drawCell(cellval, cellstyle, (x, y), (width, height))
+            if renderCB:
+                for rowNo in range(self._nrows):
+                    renderCB(self,'startRow',rowNo)
+                    for colNo in range(self._ncols):
+                        cellRect = self._spanRects[colNo, rowNo]
+                        if cellRect is not None:
+                            (x, y, width, height) = cellRect
+                            cellval = self._cellvalues[rowNo][colNo]
+                            cellstyle = self._cellStyles[rowNo][colNo]
+                            renderCB(self,'startCell', rowNo, colNo, cellval, cellstyle, (x, y), (width, height))
+                            self._drawCell(cellval, cellstyle, (x, y), (width, height))
+                            renderCB(self,'endCell')
+                    renderCB(self,'endRow')
+            else:
+                for rowNo in range(self._nrows):
+                    for colNo in range(self._ncols):
+                        cellRect = self._spanRects[colNo, rowNo]
+                        if cellRect is not None:
+                            (x, y, width, height) = cellRect
+                            cellval = self._cellvalues[rowNo][colNo]
+                            cellstyle = self._cellStyles[rowNo][colNo]
+                            self._drawCell(cellval, cellstyle, (x, y), (width, height))
+        if renderCB: renderCB(self,'startLines')
         self._drawLines()
+        if renderCB:
+            renderCB(self,'endLines')
+            renderCB(self,'endTable')
         c.restoreState()
         if self._roundingRectDef:
             self._restoreRoundingObscuredLines()
 
     def _drawBkgrnd(self):
         nrows = self._nrows
         ncols = self._ncols
@@ -1726,37 +2309,95 @@
                     color = colorCycle[i%count]
                     w = colWidths[sc + i]
                     if color:
                         canv.setFillColor(color)
                         canv.rect(x0, y0, w, h, stroke=0,fill=1)
                     x0 = x0 +w
             else:   #cmd=='BACKGROUND'
-                if arg and isinstance(arg,(list,tuple)) and arg[0] in ('VERTICAL','HORIZONTAL'):
+                if (arg and isinstance(arg,(list,tuple))
+                        and arg[0] in ('VERTICAL','HORIZONTAL', 'VERTICAL2', 'HORIZONTAL2',
+                                'LINEARGRADIENT', 'RADIALGRADIENT')):
+                    if ec==sc and er==sr and spanRects:
+                        xywh = spanRects.get((sc,sr))
+                        if xywh:
+                            #it's a single spanned cell
+                            x0, y0, w, h = xywh
+                    arg0, arg = arg[0], arg[1:]
                     #
-                    # Arg is a list, assume we are going for a gradient fill
+                    # arg is a list, assume we are going for a gradient fill
                     # where we expect a containing a direction for the gradient
                     # and the starting an final gradient colors. For example:
                     # ['HORIZONTAL', colors.white, colors.grey]   or
                     # ['VERTICAL', colors.red, colors.blue]
                     #
                     canv.saveState()
-
-                    if ec==sc and er==sr and spanRects:
-                        xywh = spanRects.get((sc,sr))
-                        if xywh:
-                            #it's a single cell
-                            x0, y0, w, h = xywh
                     p = canv.beginPath()
                     p.rect(x0, y0, w, h)
                     canv.clipPath(p, stroke=0)
-                    direction=arg[0]
-                    if direction=="HORIZONTAL":
-                        canv.linearGradient(x0,y0,x0+w,y0,arg[1:],extend=False)
-                    else:   #VERTICAL
-                        canv.linearGradient(x0,y0,x0,y0+h,arg[1:],extend=False)
+                    if arg0=="HORIZONTAL":
+                        canv.linearGradient(x0,y0,x0+w,y0,arg,extend=False)
+                    elif arg0 == "HORIZONTAL2":
+                        xh = x0 + w/2.0
+                        canv.linearGradient(x0, y0, xh, y0, arg, extend=False)
+                        canv.linearGradient(xh, y0, x0 + w, y0, arg[::-1], extend=False)
+                        #canv.linearGradient(x0, y0, x0 + w, y0, arg+arg[1::-1], extend=False)
+                    elif arg0 == "VERTICAL2":
+                        yh = y0 + h/2.0
+                        canv.linearGradient(x0, y0, x0, yh, arg, extend=False)
+                        canv.linearGradient(x0, yh, x0, y0 + h, arg[::-1], extend=False)
+                        #canv.linearGradient(x0, y0, x0, y0 + h, arg+arg[1::-1], extend=False)
+                    elif arg0=="VERTICAL":
+                        canv.linearGradient(x0, y0, x0, y0 + h, arg, extend=False)
+                    elif arg0=='LINEARGRADIENT':
+                        # the remaining arguments define the axis, extend, colors, stops as
+                        # axis = (x0,y0, x1, y1)    given as fractions of width / height
+                        # extend = bool or [bool, bool]
+                        # colors a sequence/list of colors
+                        # stops an optional sequence of fractions 0 - 1
+                        if 4<=len(arg)<=5:
+                            (ax0, ay0), (ax1, ay1) = arg[:2]
+                            ax0 = x0 + ax0*w
+                            ax1 = x0 + ax1*w
+                            ay0 = y0 + ay0*h
+                            ay1 = y0 + ay1*h
+                            extend = arg[2]
+                            C = arg[3]
+                            P = arg[4] if len(arg)==4 else None
+                            canv.linearGradient(ax0, ay0, ax1, ay1, C, positions=P, extend=extend)
+                        else:
+                            raise ValueError(f'Wrong length for {op!a} arguments {arg!a}')
+                    elif arg0=='RADIALGRADIENT':
+                        # the remaining arguments define the centre, radius, extend, colors, stops as
+                        # center = (xc,yc) given as fractions of width / height
+                        # radius = (r,'ref') op in ('width','height','min','max')
+                        # extend = bool or [bool, bool]
+                        # colors a sequence/list of colors
+                        # stops an optional sequence of fractions 0 - 1
+                        if 4<=len(arg)<=5:
+                            xc, yc = arg[0]
+                            xc = x0 + xc*w
+                            yc = y0 + yc*h
+                            r, ref = arg[1]
+                            if ref=='width':
+                                ref = w
+                            elif ref=='height':
+                                ref = h
+                            elif ref=='min':
+                                ref = min (w,h)
+                            elif ref=='max':
+                                ref = max(w,h)
+                            else:
+                                raise ValueError(f'Bad radius, {arg[1]!a}, for {op!a} arguments {arg!r}')
+                            r *= ref
+                            extend = arg[2]
+                            C = arg[3]
+                            P = arg[4] if len(arg)==4 else None
+                            canv.radialGradient(xc, yc, r, C, positions=P, extend=extend)
+                        else:
+                            raise ValueError(f'Wrong length for {op!a} arguments {arg}')
                     canv.restoreState()
                 else:
                     color = colors.toColorOrNone(arg)
                     if color:
                         if ec==sc and er==sr and spanRects:
                             xywh = spanRects.get((sc,sr))
                             if xywh:
@@ -1793,15 +2434,15 @@
             if cellval: y += cellval[0].getSpaceBefore()
             for v, w, h in zip(cellval,W,H):
                 if just=='LEFT': x = colpos+cellstyle.leftPadding
                 elif just=='RIGHT': x = colpos+colwidth-cellstyle.rightPadding - w
                 elif just in ('CENTRE', 'CENTER'):
                     x = colpos+(colwidth+cellstyle.leftPadding-cellstyle.rightPadding-w)/2.0
                 else:
-                    raise ValueError('Invalid justification %s' % just)
+                    raise ValueError(f'Invalid justification {just!a} for {type(v)}')
                 y -= v.getSpaceBefore()
                 y -= h
                 v.drawOn(self.canv,x,y)
                 y -= v.getSpaceAfter()
         else:
             if just == 'LEFT':
                 draw = self.canv.drawString
@@ -1812,28 +2453,28 @@
             elif just == 'RIGHT':
                 draw = self.canv.drawRightString
                 x = colpos + colwidth - cellstyle.rightPadding
             elif just == 'DECIMAL':
                 draw = self.canv.drawAlignedString
                 x = colpos + colwidth - cellstyle.rightPadding
             else:
-                raise ValueError('Invalid justification %s' % just)
+                raise ValueError(f'Invalid justification {just!a}')
             vals = str(cellval).split("\n")
             n = len(vals)
             leading = cellstyle.leading
             fontsize = cellstyle.fontsize
             if valign=='BOTTOM':
                 y = rowpos + cellstyle.bottomPadding+n*leading-fontsize
             elif valign=='TOP':
                 y = rowpos + rowheight - cellstyle.topPadding - fontsize
             elif valign=='MIDDLE':
                 #tim roberts pointed out missing fontsize correction 2004-10-04
                 y = rowpos + (cellstyle.bottomPadding + rowheight-cellstyle.topPadding+n*leading)/2.0 - fontsize
             else:
-                raise ValueError("Bad valign: '%s'" % str(valign))
+                raise ValueError(f'Bad valign: {valign!a}')
 
             for v in vals:
                 draw(x, y, v)
                 y -= leading
             onDraw = getattr(cellval,'onDraw',None)
             if onDraw:
                 onDraw(self.canv,cellval.kind,cellval.label)
@@ -1845,15 +2486,15 @@
             #external hyperlink
             self.canv.linkRect("", cellstyle.destination, Rect=(colpos, rowpos, colpos + colwidth, rowpos + rowheight), relative=1)
 
     def _setCornerRadii(self, cornerRadii):
         if isListOfNumbersOrNone(cornerRadii):
             self._cornerRadii = None if not cornerRadii else list(cornerRadii) + (max(4-len(cornerRadii),0)*[0])
         else:
-            raise ValueError('cornerRadii should be None or a list/tuple of numeric radii')
+            raise ValueError(f'cornerRadii should be None or a list/tuple of numeric radii\nnot {cornerRadii!a}')
 
 _LineOpMap = {  'GRID':'_drawGrid',
                 'BOX':'_drawBox',
                 'OUTLINE':'_drawBox',
                 'INNERGRID':'_drawInnerGrid',
                 'LINEBELOW':'_drawHLinesB',
                 'LINEABOVE':'_drawHLines',
@@ -1862,14 +2503,42 @@
 
 class LongTable(Table):
     '''Henning von Bargen's changes will be active'''
     _longTableOptimize = 1
 
 LINECOMMANDS = list(_LineOpMap.keys())
 
+class TableRenderCB:
+    '''table render callback abstract base klass to be called in Table.draw'''
+    def __call__(self,T,cmd,*args):
+        if not isinstance(T,Table): raise ValueError(f'TableRenderCB first argument, {repr(T)} is not a Table')
+        meth = getattr(self,cmd,None)
+        if not meth: raise ValueError(f'invalid TablerenderCB cmd {cmd}')
+        meth(T,*args)
+    def startTable(self,T):
+        raise NotImplementedError('startTable')
+    def startBG(self,T):
+        raise NotImplementedError('startBG')
+    def endBG(self,T):
+        raise NotImplementedError('endBG')
+    def startRow(self,T,rowNo):
+        raise NotImplementedError('startRow')
+    def startCell(self,T,rowNo, colNo, cellval, cellstyle, pos, size):
+        raise NotImplementedError('startCell')
+    def endCell(self,T):
+        raise NotImplementedError('endCell')
+    def endRow(self,T):
+        raise NotImplementedError('endRow')
+    def startLines(self,T):
+        raise NotImplementedError('startLines')
+    def endLines(self,T):
+        raise NotImplementedError('endLines')
+    def endTable(self,T):
+        raise NotImplementedError('endTable')
+
 def _isLineCommand(cmd):
     return cmd[0] in LINECOMMANDS
 
 def _setCellStyle(cellStyles, i, j, op, values):
     #new = CellStyle('<%d, %d>' % (i,j), cellStyles[i][j])
     #cellStyles[i][j] = new
     ## modify in place!!!
```

### Comparing `reportlab-3.6.9/src/reportlab/platypus/xpreformatted.py` & `reportlab-4.0.0/src/reportlab/platypus/xpreformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/src/reportlab/rl_config.py` & `reportlab-4.0.0/src/reportlab/rl_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,22 +43,35 @@
     return _DEFAULTS
 
 _DEFAULTS=_defaults_init()
 
 _SAVED = {}
 sys_version=None
 
+def _enumChk(name,value,allowed=()):
+    if value not in allowed:
+        raise ValueError(f'invalid value {value!r} for rl_config.{name}\nneed one of {allowed}')
+
+from functools import partial
+_rlChecks=dict(
+        renderPMBackend = partial(_enumChk,allowed=('rlPyCairo','_renderPM')),
+        xmlParser = partial(_enumChk,allowed=('lxml','pyrxp')),
+        textPaths = partial(_enumChk,allowed=('freetype','_renderPM','backend')),
+        )
+
 #this is used to set the options from
-def _setOpt(name, value, conv=None):
+def _setOpt(name, value, conv=None, chk=None):
     '''set a module level value from environ/default'''
     from os import environ
     ename = 'RL_'+name
     if ename in environ:
         value = environ[ename]
     if conv: value = conv(value)
+    chk = _rlChecks.get(name,None)
+    if chk: chk(name,value)
     globals()[name] = value
 
 def _startUp():
     '''This function allows easy resetting to the global defaults
     If the environment contains 'RL_xxx' then we use the value
     else we use the given default'''
     import os, sys
```

### Comparing `reportlab-3.6.9/src/reportlab/rl_settings.py` & `reportlab-4.0.0/src/reportlab/rl_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,18 @@
 embeddedHyphenation
 hyphenationMinWordLength
 reserveTTFNotdef
 documentLang
 encryptionStrength
 trustedHosts
 trustedSchemes
-renderPMBackend'''.split())
+renderPMBackend
+xmlParser
+textPaths
+toColorCanUse'''.split())
 
 allowTableBoundsErrors =    1 # set to 0 to die on too large elements in tables in debug (recommend 1 for production use)
 shapeChecking =             1
 defaultEncoding =           'WinAnsiEncoding'       # 'WinAnsi' or 'MacRoman'
 defaultGraphicsFontName=    'Times-Roman'           #initializer for STATE_DEFAULTS in shapes.py
 pageCompression =           1                       # default page compression mode
 useA85 =                    1                       #set to 0 to disable Ascii Base 85 stream filters
@@ -97,19 +100,15 @@
 platypus_link_underline=    0                       #paragraph links etc underlined if true
 canvas_basefontname=        'Helvetica'             #this is used to initialize the canvas; if you override to make
                                                     #something else you are responsible for ensuring the font is registered etc etc
                                                     #this will be used everywhere and the font family connections will be made
                                                     #if the bold/italic/bold italic fonts are also registered and defined as a family.
 
 allowShortTableRows=1                               #allows some rows in a table to be short
-imageReaderFlags=0                                  #attempt to convert images into internal memory files to reduce
-                                                    #the number of open files (see lib.utils.ImageReader)
-                                                    #if imageReaderFlags&2 then attempt autoclosing of those files
-                                                    #if imageReaderFlags&4 then cache data 
-                                                    #if imageReaderFlags==-1 then use Ralf Schmitt's re-opening approach
+imageReaderFlags=0                                  #no longer in use
 paraFontSizeHeightOffset=   1                       #if true paragraphs start at height-fontSize
 canvas_baseColor=           None                    #initialize the canvas fill and stroke colors if this is set
 ignoreContainerActions=     1                       #if true then action flowables in flowable _Containers will be ignored
 ttfAsciiReadable=           1                       #smaller subsets when set to 0
 pdfMultiLine=               0                       #use more lines in pdf etc
 pdfComments=                0                       #put in pdf comments
 debug=                      0                       #for debugging code
@@ -156,15 +155,20 @@
 documentLang=None                                   #pdf document catalog Lang value xx-xx not ee_xx
 encryptionStrength=40                               #the bits for standard encryption 40, 128 or 256 (AES)
 trustedHosts=None                                   #set to a list of trusted for access hosts None means
                                                     #all are trusted glob patterns eg *.reportlab.com are
                                                     #allowed. In environment use a comma separated string.
 trustedSchemes=['file', 'rml', 'data', 'https',     #these url schemes are trusted
                 'http', 'ftp']
-renderPMBackend='_renderPM'                         #or 'rlPyCairo' if available
+renderPMBackend='rlPyCairo'                         #or '_renderPM' if available
+xmlParser='lxml'                                    #or 'pyrxp' for preferred xml parsing
+textPaths='freetype'                                #freetype or _renderPM or backend
+                                                    #determines what code is used to create Paths from str
+                                                    #see reportlab/graphics/utils.py for full horror
+toColorCanUse='rl_extended_literal_eval'            #change to None or 'rl_safe_eval' depending on trust
 
 # places to look for T1Font information
 T1SearchPath =  (
                 'c:/Program Files/Adobe/Acrobat 9.0/Resource/Font', 
                 'c:/Program Files/Adobe/Acrobat 8.0/Resource/Font', 
                 'c:/Program Files/Adobe/Acrobat 7.0/Resource/Font', 
                 'c:/Program Files/Adobe/Acrobat 6.0/Resource/Font', #Win32, Acrobat 6
```

### Comparing `reportlab-3.6.9/src/reportlab.egg-info/PKG-INFO` & `reportlab-4.0.0/src/reportlab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 3.6.9
+Version: 4.0.0
 Summary: The Reportlab Toolkit
 Home-page: http://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
-License: BSD license (see license.txt for details), Copyright (c) 2000-2018, ReportLab Inc.
-Platform: UNKNOWN
+License: BSD license (see license.txt for details), Copyright (c) 2000-2022, ReportLab Inc.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Printing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7, <4
-Provides-Extra: RLPYCAIRO
-License-File: LICENSE.txt
+Requires-Python: >=3.7,<4
+Provides-Extra: RL_ACCEL
+Provides-Extra: RL_RENDERPM
+License-File: LICENSE
 
 The ReportLab Toolkit. An Open Source Python library for generating PDFs and graphics.
-
```

### Comparing `reportlab-3.6.9/tests/00readme.txt` & `reportlab-4.0.0/tests/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/_i_am_actually_a_gif.jpg` & `reportlab-4.0.0/tests/_i_am_actually_a_gif.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/_i_am_actually_a_jpeg.gif` & `reportlab-4.0.0/tests/_i_am_actually_a_jpeg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/alpha_test.png` & `reportlab-4.0.0/tests/alpha_test.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample0c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4c1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample4d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample5d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample5d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample6d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample6d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample7d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample7d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample8b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample8b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample9c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample9c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_axes_sample_hatching.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_doughnut_sample4.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_doughnut_sample4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample1c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample1c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample2c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample2c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample3a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample3a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_legends_sample4a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_legends_sample4a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample1a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sample3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample1c.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sample2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample2.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample4.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample4.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample5.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample5.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample6.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample6.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample7.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample7.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample8.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample8.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_piecharts_sample9.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_piecharts_sample9.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_bcleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_bcleg.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,15,80.83333)
 		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,15,95)
 		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_hlcleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_hlcleg.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,15,80.83333)
 		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,15,95)
 		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_lpleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,90 +1,75 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, PolyLine, Polygon
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Polygon, PolyLine, Line, Circle, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=300,height=150,*args,**kw):
+	def __init__(self,width=400,height=400,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,10,50,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(80,10,80,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(140,10,140,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(170,10,170,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,20,5)
-		v0.add(String(-2.5,-10,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,5)
-		v0.add(String(-6.25,-10,'1.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,5)
-		v0.add(String(-2.5,-10,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,110,5)
-		v0.add(String(-6.25,-10,'2.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,140,5)
-		v0.add(String(-2.5,-10,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,170,5)
-		v0.add(String(-6.25,-10,'3.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,5)
-		v0.add(String(-2.5,-10,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,27,15,27,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,44,15,44,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,61,15,61,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,78,15,78,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,10)
-		v0.add(String(-5,-4,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,27)
-		v0.add(String(-5,-4,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,44)
-		v0.add(String(-5,-4,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,61)
-		v0.add(String(-5,-4,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,78)
-		v0.add(String(-5,-4,'5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,95)
-		v0.add(String(-5,-4,'6',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(PolyLine(points=[20,10,80,27,110,10,140,44,200,78],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[20,27,80,44,110,27,140,61,200,95],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[17,10,20,13,23,10,20,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[77,27,80,30,83,27,80,24],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[107,10,110,13,113,10,110,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[137,44,140,47,143,44,140,41],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[197,78,200,81,203,78,200,75],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(17.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(77.5,41.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(107.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(137.5,58.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(197.5,92.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[108.3032,252.9412,200,288.2353,291.6968,252.9412,306.9796,138.2353,200,58.82353,93.02039,138.2353,108.3032,252.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[85.37899,266.1765,200,252.9412,261.1312,235.2941,276.414,155.8824,200,94.11765,131.2274,160.2941,85.37899,266.1765],fillColor=Color(.678431,.847059,.901961,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[138.8688,235.2941,200,261.7647,261.1312,235.2941,329.9038,125,200,164.7059,108.3032,147.0588,138.8688,235.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[108.3032,252.9412,200,288.2353,291.6968,252.9412,306.9796,138.2353,200,58.82353,93.02039,138.2353,108.3032,252.9412],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[85.37899,266.1765,200,252.9412,261.1312,235.2941,276.414,155.8824,200,94.11765,131.2274,160.2941,85.37899,266.1765],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[138.8688,235.2941,200,261.7647,261.1312,235.2941,329.9038,125,200,164.7059,108.3032,147.0588,138.8688,235.2941],strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,200,350,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,329.9038,275,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,329.9038,125,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,200,50,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,70.09619,125,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,200,70.09619,275,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,288.2353,200,291.2353,203,288.2353,200,285.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[288.6968,252.9412,291.6968,255.9412,294.6968,252.9412,291.6968,249.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[303.9796,138.2353,306.9796,141.2353,309.9796,138.2353,306.9796,135.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,58.82353,200,61.82353,203,58.82353,200,55.82353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[90.02039,138.2353,93.02039,141.2353,96.02039,138.2353,93.02039,135.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[105.3032,252.9412,108.3032,255.9412,111.3032,252.9412,108.3032,249.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(200,252.9412,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(261.1312,235.2941,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(276.414,155.8824,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(200,94.11765,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(131.2274,160.2941,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(85.37899,266.1765,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,261.7647,200,264.7647,203,261.7647,200,258.7647],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[258.1312,235.2941,261.1312,238.2941,264.1312,235.2941,261.1312,232.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[326.9038,125,329.9038,128,332.9038,125,329.9038,122],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,164.7059,200,167.7059,203,164.7059,200,161.7059],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[105.3032,147.0588,108.3032,150.0588,111.3032,147.0588,108.3032,144.0588],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[135.8688,235.2941,138.8688,238.2941,141.8688,235.2941,138.8688,232.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,357.5)
+		v0.add(String(-3.61,-4,'U',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,336.399,278.75)
+		v0.add(String(-3.61,-4,'V',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,336.399,121.25)
+		v0.add(String(-4.72,-4,'W',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,42.5)
+		v0.add(String(-3.61,-4,'X',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,63.601,121.25)
+		v0.add(String(-3.61,-4,'Y',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,63.601,278.75)
+		v0.add(String(-3.055,-4,'Z',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,283.2353)
+		v0.add(String(-8.605,-4,'zero',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,287.3667,250.4412)
+		v0.add(String(-7.22,-4,'one',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,63.82353)
+		v0.add(String(-13.885,-4,'special',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,247.9412)
+		v0.add(String(-10.83,-4,'Earth',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,325.5737,127.5)
+		v0.add(String(-10.275,-4,'Mars',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_pcleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_pcleg.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
 		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(50,50,50,50.86957,90,yradius=50,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(50,50,50,-39.13043,50.86957,yradius=50,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(50,50,50,-105.6522,-39.13043,yradius=50,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(50,50,50,-270,-105.6522,yradius=50,annular=False,fillColor=Color(0,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_plpleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_plpleg.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 		v0.transform = (1,0,0,1,131.35,41.07216)
 		v0.add(Rect(0,-6,4.44,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		v0.add(String(0,-4,'c',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,131.35,6)
 		v0.add(Rect(0,-6,5,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		v0.add(String(0,-4,'d',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1bar.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1bar.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,70 +13,70 @@
 		self.add(Rect(168.75,50,25,45.83333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(206.25,50,25,77.08333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(243.75,50,25,93.75,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(281.25,50,25,39.58333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(318.75,50,25,8.333333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,68.75,77.08333)
-		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,106.25,60.41667)
-		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,143.75,91.66667)
-		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,181.25,95.83333)
-		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,218.75,127.0833)
-		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,256.25,143.75)
-		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,293.75,89.58333)
-		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,331.25,58.33333)
-		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
-		v0.add(String(-30.57,-10,'Jän-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-31.74805,-10,'Jän-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
-		v0.add(String(-31.68,-10,'Feb-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-34.58496,-10,'Feb-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
-		v0.add(String(-31.67,-10,'Mär-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-35.2002,-10,'Mär-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
-		v0.add(String(-30.01,-10,'Äpr-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-33.63281,-10,'Äpr-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
-		v0.add(String(-33.34,-10,'Mäy-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-37.00684,-10,'Mäy-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
-		v0.add(String(-30.57,-10,'Jün-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-31.95801,-10,'Jün-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
-		v0.add(String(-27.23,-10,'Jül-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-28.39844,-10,'Jül-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
-		v0.add(String(-32.24,-10,'Äüg-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-35.85938,-10,'Äüg-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1barline.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1barline.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample1line.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample1line.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2bar.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,94 +21,94 @@
 		self.add(Rect(181.25,50,15,47.91667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(218.75,50,15,79.16667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(256.25,50,15,95.83333,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(293.75,50,15,41.66667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Rect(331.25,50,15,10.41667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,61.25,77.08333)
-		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,98.75,60.41667)
-		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,136.25,91.66667)
-		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,173.75,95.83333)
-		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,211.25,127.0833)
-		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,248.75,143.75)
-		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,286.25,89.58333)
-		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,323.75,58.33333)
-		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,76.25,79.16667)
-		v0.add(String(0,-4,'Å14',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å14',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,113.75,62.5)
-		v0.add(String(0,-4,'Å6',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å6',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,151.25,93.75)
-		v0.add(String(0,-4,'Å21',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å21',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,188.75,97.91667)
-		v0.add(String(0,-4,'Å23',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å23',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,226.25,129.1667)
-		v0.add(String(0,-4,'Å38',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å38',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,263.75,145.8333)
-		v0.add(String(0,-4,'Å46',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å46',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,301.25,91.66667)
-		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,338.75,60.41667)
-		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
-		v0.add(String(-30.57,-10,'Jän-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-31.74805,-10,'Jän-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
-		v0.add(String(-31.68,-10,'Feb-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-34.58496,-10,'Feb-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
-		v0.add(String(-31.67,-10,'Mär-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-35.2002,-10,'Mär-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
-		v0.add(String(-30.01,-10,'Äpr-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-33.63281,-10,'Äpr-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
-		v0.add(String(-33.34,-10,'Mäy-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-37.00684,-10,'Mäy-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
-		v0.add(String(-30.57,-10,'Jün-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-31.95801,-10,'Jün-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
-		v0.add(String(-27.23,-10,'Jül-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-28.39844,-10,'Jül-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
-		v0.add(String(-32.24,-10,'Äüg-99',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-35.85938,-10,'Äüg-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample2line.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample2line.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample3.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample3.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_sample4pie.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_sample4pie.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 		self.add(Wedge(200,100,50,-67.75281,-22.80899,yradius=50,annular=False,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(200,100,50,-112.6966,-67.75281,yradius=50,annular=False,fillColor=Color(1,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(200,100,50,-157.6404,-112.6966,yradius=50,annular=False,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(200,100,50,-202.5843,-157.6404,yradius=50,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(200,100,50,-247.5281,-202.5843,yradius=50,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Wedge(200,100,50,-270,-247.5281,yradius=50,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(String(200.2353,159.9995,'0',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(String(212.1523,158.7565,'ä',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(212.1523,158.7565,'ä',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(242.7166,142.1342,'b',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(307.4981,99.36757,'c',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
 		self.add(String(242.2179,57.3661,'d',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(199.7647,40.00046,'e',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(157.449,57.69858,'f',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(140.0001,100.1177,'g',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(String(157.6152,142.468,'h',textAnchor='middle',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(157.6152,142.468,'h',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(String(188.309,158.85,'i',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Rect(310,140,20,5,rx=0,ry=0,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(String(295,139.085,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Rect(310,120,20,5,rx=0,ry=0,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(String(295,119.085,'ä',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Rect(310,100,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(String(295,99.085,'b',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_special_scleg.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_scleg.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 		v0.add(String(-2.5,-4,'d',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,18.1606,52.75)
 		v0.add(String(-2.22,-4,'e',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,18.1606,147.25)
 		v0.add(String(-1.665,-4,'f',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.91,'röt',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.91,'blue',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(182.78,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.91,'green',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.91,'pink',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(257.78,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.91,'yellow',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample1.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_spider_sample1.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/charts-out/test_graphics_charts_spider_sample2.py` & `reportlab-4.0.0/tests/charts-out/test_graphics_charts_special_lpleg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,90 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Polygon, PolyLine, Line, Circle, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, PolyLine, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=400,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Polygon(points=[108.3032,252.9412,200,288.2353,291.6968,252.9412,306.9796,138.2353,200,58.82353,93.02039,138.2353,108.3032,252.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[85.37899,266.1765,200,252.9412,261.1312,235.2941,276.414,155.8824,200,94.11765,131.2274,160.2941,85.37899,266.1765],fillColor=Color(.678431,.847059,.901961,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[138.8688,235.2941,200,261.7647,261.1312,235.2941,329.9038,125,200,164.7059,108.3032,147.0588,138.8688,235.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=None,strokeWidth=0,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[108.3032,252.9412,200,288.2353,291.6968,252.9412,306.9796,138.2353,200,58.82353,93.02039,138.2353,108.3032,252.9412],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[85.37899,266.1765,200,252.9412,261.1312,235.2941,276.414,155.8824,200,94.11765,131.2274,160.2941,85.37899,266.1765],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[138.8688,235.2941,200,261.7647,261.1312,235.2941,329.9038,125,200,164.7059,108.3032,147.0588,138.8688,235.2941],strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,200,350,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,329.9038,275,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,329.9038,125,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,200,50,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,70.09619,125,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,200,70.09619,275,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[197,288.2353,200,291.2353,203,288.2353,200,285.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[288.6968,252.9412,291.6968,255.9412,294.6968,252.9412,291.6968,249.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[303.9796,138.2353,306.9796,141.2353,309.9796,138.2353,306.9796,135.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[197,58.82353,200,61.82353,203,58.82353,200,55.82353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[90.02039,138.2353,93.02039,141.2353,96.02039,138.2353,93.02039,135.2353],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[105.3032,252.9412,108.3032,255.9412,111.3032,252.9412,108.3032,249.9412],fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(200,252.9412,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(261.1312,235.2941,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(276.414,155.8824,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(200,94.11765,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(131.2274,160.2941,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(85.37899,266.1765,2.5,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[197,261.7647,200,264.7647,203,261.7647,200,258.7647],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[258.1312,235.2941,261.1312,238.2941,264.1312,235.2941,261.1312,232.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[326.9038,125,329.9038,128,332.9038,125,329.9038,122],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[197,164.7059,200,167.7059,203,164.7059,200,161.7059],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[105.3032,147.0588,108.3032,150.0588,111.3032,147.0588,108.3032,144.0588],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[135.8688,235.2941,138.8688,238.2941,141.8688,235.2941,138.8688,232.2941],fillColor=Color(.596078,.984314,.596078,1),fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,357.5)
-		v0.add(String(-3.61,-4,'U',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,336.399,278.75)
-		v0.add(String(-3.61,-4,'V',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,336.399,121.25)
-		v0.add(String(-4.72,-4,'W',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,42.5)
-		v0.add(String(-3.61,-4,'X',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,63.601,121.25)
-		v0.add(String(-3.61,-4,'Y',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,63.601,278.75)
-		v0.add(String(-3.055,-4,'Z',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,283.2353)
-		v0.add(String(-8.605,-4,'zero',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,287.3667,250.4412)
-		v0.add(String(-7.22,-4,'one',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,63.82353)
-		v0.add(String(-13.885,-4,'special',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,247.9412)
-		v0.add(String(-10.83,-4,'Earth',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,325.5737,127.5)
-		v0.add(String(-10.275,-4,'Mars',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,10,50,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(80,10,80,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(140,10,140,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(170,10,170,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,20,5)
+		v0.add(String(-2.5,-10,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,50,5)
+		v0.add(String(-6.25,-10,'1.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,80,5)
+		v0.add(String(-2.5,-10,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,110,5)
+		v0.add(String(-6.25,-10,'2.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,140,5)
+		v0.add(String(-2.5,-10,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,170,5)
+		v0.add(String(-6.25,-10,'3.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,5)
+		v0.add(String(-2.5,-10,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,27,15,27,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,44,15,44,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,61,15,61,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,78,15,78,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,10)
+		v0.add(String(-5,-4,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,27)
+		v0.add(String(-5,-4,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,44)
+		v0.add(String(-5,-4,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,61)
+		v0.add(String(-5,-4,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,78)
+		v0.add(String(-5,-4,'5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,95)
+		v0.add(String(-5,-4,'6',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(PolyLine(points=[20,10,80,27,110,10,140,44,200,78],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[20,27,80,44,110,27,140,61,200,95],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[17,10,20,13,23,10,20,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[77,27,80,30,83,27,80,24],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[107,10,110,13,113,10,110,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[137,44,140,47,143,44,140,41],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,78,200,81,203,78,200,75],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(17.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(77.5,41.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(107.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(137.5,58.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(197.5,92.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-3.6.9/tests/encryption.gif` & `reportlab-4.0.0/tests/encryption.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/gray-alpha.png` & `reportlab-4.0.0/tests/gray-alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/pythonpowered-gs.gif` & `reportlab-4.0.0/tests/pythonpowered-gs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/pythonpowered.gif` & `reportlab-4.0.0/tests/pythonpowered.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/rltw-icon-tr.png` & `reportlab-4.0.0/tests/rltw-icon-tr.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/runAll.py` & `reportlab-4.0.0/tests/runAll.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,17 +100,23 @@
     # all PDF & log files before starting run.  You don't
     # want this if reusing runAll anywhere else.
     if os.sep+'tests' in folder: cleanup(folder)
     cleanup(outputfile(''))
     NI = []
     cleanOnly = '--clean' in sys.argv
     verbosity = [_ for _ in sys.argv if _.startswith('--verbosity=')]
-    verbosity = int(verbosity[-1][12:]) if verbosity else 1
+    if not verbosity: verbosity = [f'''--verbosity={os.environ.get('RL_testVerbosity','1')}''']
+    verbosity = int(verbosity[-1][12:])
     if not cleanOnly:
-        testSuite = makeSuite(folder,nonImportable=NI,pattern=pattern+(not haveSRC and 'c' or ''))
+        exclude = sum([
+                    [os.path.splitext(os.path.basename(_.strip()))[0]
+                            for _ in a[10:].split(',') if _.strip()]
+                                for a in sys.argv if a.startswith('--exclude=')
+                    ],[])
+        testSuite = makeSuite(folder,nonImportable=NI,exclude=exclude,pattern=pattern+(not haveSRC and 'c' or ''))
         result = unittest.TextTestRunner(verbosity=verbosity).run(testSuite)
     else:
         result = None
 
     if haveSRC: cleanup(folder,patterns=('*.pyc','*.pyo'))
     if not cleanOnly:
         if NI:
```

### Comparing `reportlab-3.6.9/tests/solid_red_alpha.png` & `reportlab-4.0.0/tests/solid_red_alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_charts_textlabels.py` & `reportlab-4.0.0/tests/test_charts_textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_crypto_algorithms.py` & `reportlab-4.0.0/tests/test_crypto_algorithms.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_docs_build.py` & `reportlab-4.0.0/tests/test_docs_build.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_docstrings.py` & `reportlab-4.0.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_extra.py` & `reportlab-4.0.0/tests/test_extra.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_geomutils.py` & `reportlab-4.0.0/tests/test_geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_graphics_barcode.py` & `reportlab-4.0.0/tests/test_graphics_barcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,31 +263,31 @@
                 s.append(Spacer(36, 12))
             s.append(Paragraph('Barcode should say: ' + dr._bc.value, styleN))
             story.append(KeepTogether(s))
 
     SimpleDocTemplate(fileName).build(story)
 
 try:
-    from reportlab.graphics import _renderPM
+    from reportlab.graphics import renderPM
 except ImportError:
-    _renderPM = None
+    renderPM = None
 
 class BarcodeWidgetTestCase(unittest.TestCase):
     "Test barcode classes."
 
     @classmethod
     def setUpClass(cls):
         cls.outDir = outDir = outputfile('barcode-out')
         cls.makeFn = lambda _, fn: os.path.join(outDir,fn)
         if not os.path.isdir(outDir):
             os.makedirs(outDir)
         for x in glob.glob(os.path.join(outDir,'*')):
             os.remove(x)
 
-    @unittest.skipIf(not _renderPM,'no _renderPM')
+    @unittest.skipIf(not renderPM,'no renderPM')
     def test0(self):
         from reportlab.graphics.shapes import Drawing
         outDir = self.outDir
         html = ['<html><head></head><body>']
         a = html.append
         formats = ['gif','pict','pdf']
         from reportlab.graphics.barcode import getCodes
```

### Comparing `reportlab-3.6.9/tests/test_graphics_charts.py` & `reportlab-4.0.0/tests/test_graphics_charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from reportlab.graphics.charts.piecharts import Pie
 from reportlab.graphics.charts.legends import Legend
 from reportlab.graphics.charts.spider import SpiderChart
 from reportlab.graphics.widgets.markers import makeMarker
 from reportlab.graphics.widgets.adjustableArrow import AdjustableArrowDrawing
 
 try:
-    from reportlab.graphics import _renderPM
+    from reportlab.graphics import renderPM
 except ImportError:
-    _renderPM = None
+    renderPM = None
 
 def getFontName():
     try:
         from reportlab.pdfbase.pdfmetrics import registerFont
         from reportlab.pdfbase.ttfonts import TTFont
         fontName = 'Vera'
         registerFont(TTFont(fontName, "Vera.ttf"))
@@ -327,18 +327,25 @@
     except ImportError:
         return []
     else:
         return ['eps']
 
 def run_samples(L):
     outDir = outputfile('charts-out')
-    for k,f,kind in L:
-        d = f()
-        if not isinstance(d,Drawing): continue
-        d.save(formats=['pdf', 'gif', 'svg', 'ps', 'py']+eps(),outDir=outDir, fnRoot='test_graphics_charts_%s_%s' % (kind,k))
+    global fontName
+    oFontName = fontName
+    def innerRun(formats):
+        for k,f,kind in L:
+            d = f()
+            if not isinstance(d,Drawing): continue
+            d.save(formats=formats,outDir=outDir, fnRoot='test_graphics_charts_%s_%s' % (kind,k))
+    innerRun(['pdf', 'gif', 'svg', 'py']+eps())
+    fontName = 'Helvetica'
+    innerRun(['ps'])
+    fontName = oFontName
 
 class ChartTestCase(unittest.TestCase):
     "Test chart classes."
 
     @classmethod
     def setUpClass(cls):
         "Hook method for setting up the test fixture before exercising it."
@@ -349,16 +356,14 @@
     def tearDownClass(cls):
         "Hook method for deconstructing the test fixture after testing it."
 
         path=outputfile('test_graphics_charts.pdf')
         doc = MyDocTemplate(path)
         doc.build(cls.story)
 
-        global fontName
-        fontName = 'Helvetica'
         run_samples([(k,v,'special') for k,v in globals().items() if k.lower().startswith('sample')
                             or k in ('lpleg', 'hlcleg', 'bcleg', 'pcleg', 'scleg', 'plpleg')
                             ])
 
     def test0(self):
         "Test bar charts."
 
@@ -515,15 +520,15 @@
         A = makeArrow()
         bb = A.getBounds()
         deltax = 2 + max(bb[2]-bb[0],bb[3]-bb[1])
         for i,angle in enumerate((0, 10, 20, 60, 90, 120, 180, 270, 315)):
             story.append(makeArrow(y=-10,x=deltax*i,angle=angle,strokeColor=colors.black,strokeWidth=0.5,headSweep=-i*0.6))
         story.append(Spacer(0,1*cm))
 
-    @unittest.skipIf(not _renderPM,'no _renderPM')
+    @unittest.skipIf(not renderPM,'no renderPM')
     def test8(self):
         '''text _text2Path'''
         story = self.story
         story.append(Paragraph('Texts drawn using a Path', h3))
         story.append(Spacer(0,0.5*cm))
         P=_text2Path('Hello World from font Times-Roman!',x=10,y=20,fontName='Times-Roman',fontSize=20,strokeColor=colors.blue,strokeWidth=0.1,fillColor=colors.red)
         d = Drawing(400,50)
```

### Comparing `reportlab-3.6.9/tests/test_graphics_images-cairo.gif` & `reportlab-4.0.0/tests/test_graphics_images.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_graphics_images-cairo.png` & `reportlab-4.0.0/tests/test_graphics_images.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_graphics_images.py` & `reportlab-4.0.0/tests/test_graphics_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,24 @@
         assert os.path.exists(outPath)
 
         try:
             import rlPyCairo
         except ImportError:
             rlPyCairo = None
 
+        try:
+            import _rl_renderPM
+        except ImportError:
+            _rl_renderPM = None
+
         from reportlab.rl_config import renderPMBackend
-        d.save(formats=['png', 'gif', 'ps','svg'],outDir=os.path.dirname(outPath), fnRoot='test_graphics_images', _renderPM_backend='_renderPM')
         if rlPyCairo:
-            d.save(formats=['png', 'gif'],outDir=os.path.dirname(outPath), fnRoot='test_graphics_images-cairo',
-                    **(dict(_renderPM_backend='rlPyCairo') if renderPMBackend=='_renderPM' else {}))
+            d.save(formats=['png', 'gif', 'ps','svg'],outDir=os.path.dirname(outPath), fnRoot='test_graphics_images', _renderPM_backend='rlPyCairo')
+        if _rl_renderPM:
+            d.save(formats=['png', 'gif'],outDir=os.path.dirname(outPath), fnRoot='test_graphics_images-libart', _renderPM_backend='_renderPM')
 
 
     def test0(self):
         "Test convert a bitmap file as Image shape into a tmp. PDF file."
 
         d = Drawing(110, 44)
         inPath = IMAGENAME
```

### Comparing `reportlab-3.6.9/tests/test_graphics_layout.py` & `reportlab-4.0.0/tests/test_graphics_layout.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_graphics_render.py` & `reportlab-4.0.0/tests/test_graphics_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 Tests for renderers
 """
 from reportlab.lib.testutils import setOutDir,makeSuiteForClasses, outputfile, printLocation
 setOutDir(__name__)
 import unittest, os, sys, glob
 try:
-    from reportlab.graphics import _renderPM
+    from reportlab.graphics import renderPM
 except:
-    _renderPM = None
+    renderPM = None
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Path, String, Polygon, Hatching, Line, definePath
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor, toColor
 
 class FillModeDrawing(_DrawingEditorMixin,Drawing):
     def __init__(self,width=600.0,height=200.0,fillMode='even-odd',*args,**kw):
         Drawing.__init__(self,width,height,*args,**kw)
         self.transform = (1,0,0,1,0,0)
@@ -145,34 +145,34 @@
         from reportlab.graphics.renderPS import test
         assert test(self.outDir) is None
 
     def test1(self):
         from reportlab.graphics.renderPDF import test
         assert test(self.outDir) is None
 
-    @unittest.skipIf(not _renderPM,'no _renderPM')
+    @unittest.skipIf(not renderPM,'no renderPM')
     def test2(self):
         from reportlab.graphics.renderPM import test
         assert test(self.outDir) is None
 
     def test3(self):
         from reportlab.graphics.renderSVG import test
         assert test(self.outDir) is None
 
     def test4(self):
-        formats = ('pdf svg ps py' + (' png' if _renderPM else '')).split()
+        formats = ('pdf svg ps py' + (' png' if renderPM else '')).split()
         for fm in (0,1):
             FillModeDrawing(fillMode=fm).save(formats=formats,outDir=self.outDir,fnRoot='fillmode-'+('non-zero' if fm else 'even-odd'))
         _410Drawing().save(formats=formats,outDir=self.outDir,fnRoot='410')
         for ac in (None,'pdf','svg'):
             AutoCloseDrawing(autoclose=ac).save(formats=formats,outDir=self.outDir,fnRoot='autoclose-'+(ac or 'none'))
         HatchDrawing().save(formats=formats,outDir=self.outDir,fnRoot='hatch')
         TextRenderModeDrawing().save(formats=formats,outDir=self.outDir,fnRoot='textmode')
 
-    @unittest.skipIf(not _renderPM,'no _renderPM')
+    @unittest.skipIf(not renderPM,'no renderPM')
     def testSVGLibIssues(self):
         SVGLibIssue104().save(formats=['pdf','png'],outDir=self.outDir, fnRoot='svglib-issue104')
         from PIL import Image
         im = Image.open(os.path.join(self.outDir,'svglib-issue104.png'))
         lastColWhite = [y for y in range(124) if im.getpixel((223,y))==(255,255,255)]
         self.assertEqual(len(lastColWhite),124)
```

### Comparing `reportlab-3.6.9/tests/test_graphics_speed.py` & `reportlab-4.0.0/tests/test_graphics_speed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_hello.py` & `reportlab-4.0.0/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_images.py` & `reportlab-4.0.0/tests/test_images.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 __version__='3.3.0'
 __doc__="""Tests to do with image handling.
 
 Most of them make use of test\\pythonpowereed.gif."""
 from reportlab.lib.testutils import setOutDir,makeSuiteForClasses, printLocation
 setOutDir(__name__)
 import os
-try:
-    from hashlib import md5
-except ImportError:
-    from md5 import md5
 import unittest
+from hashlib import md5
 from reportlab.lib.utils import ImageReader
 
 
 """To avoid depending on external stuff, I made a small 5x5 image and
 attach its 'file contents' here in several formats.
 
 The image looks like this, with K=black, R=red, G=green, B=blue, W=white.
```

### Comparing `reportlab-3.6.9/tests/test_invariant.py` & `reportlab-4.0.0/tests/test_invariant.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,19 +53,20 @@
     return makeSuiteForClasses(InvarTestCase)
 
 
 #noruntests
 if __name__ == "__main__":
     # add some diagnostics, useful in invariant tests
     import sys, os
-    from reportlab.lib.utils import md5, bytestr
+    from hashlib import md5
+    from reportlab.lib.utils import bytestr
     verbose = ('-v' in sys.argv)
     unittest.TextTestRunner().run(makeSuite())
     if verbose:
         #tell us about the file we produced
         fileSize = os.stat(filename)[6]
         raw = open(filename,'rb').read()
-        digest = md5.md5(bytestr(raw)).hexdigest()
+        digest = md5(bytestr(raw)).hexdigest()
         major, minor = sys.version_info[0:2]
         print('%s on %s (Python %d.%d):\n    %d bytes, digest %s' % (
             filename,sys.platform, major, minor, fileSize, digest))
     printLocation()
```

### Comparing `reportlab-3.6.9/tests/test_issues.py` & `reportlab-4.0.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_lib_colors.py` & `reportlab-4.0.0/tests/test_lib_colors.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_lib_normaldate.py` & `reportlab-4.0.0/tests/test_lib_normaldate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_lib_pdfencrypt.py` & `reportlab-4.0.0/tests/test_lib_pdfencrypt.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_lib_sequencer.py` & `reportlab-4.0.0/tests/test_lib_sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_lib_utils.py` & `reportlab-4.0.0/tests/test_lib_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         self.myAssertRaisesRegex(AttributeError,r"asUnicode\(.*'list' object has no attribute 'decode'", asUnicode,['abc'])
         self.assertEqual(asUnicodeEx(u'abc'),u'abc')
         self.assertEqual(asUnicodeEx(b'abc'),u'abc')
         self.assertEqual(asUnicodeEx(123),u'123')
         self.assertEqual(asBytes(u'abc'),b'abc')
         self.assertEqual(asBytes(b'abc'),b'abc')
         self.assertRaises(AttributeError,asBytes,['abc'])
-        self.myAssertRaisesRegex(AttributeError,"asBytes\(.*'list' object has no attribute 'encode'", asBytes,['abc'])
+        self.myAssertRaisesRegex(AttributeError,r"asBytes\(.*'list' object has no attribute 'encode'", asBytes,['abc'])
 
 class RaccessTest:
     l = [1, 2]
     a = [0, [1, 2, [3,4]]]
     b = {'x': {'y': 'y'}, 'z': [1, 2]}
     z = 'z'
```

### Comparing `reportlab-3.6.9/tests/test_lib_validators.py` & `reportlab-4.0.0/tests/test_lib_validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_multibyte_chs.py` & `reportlab-4.0.0/tests/test_multibyte_chs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_multibyte_cht.py` & `reportlab-4.0.0/tests/test_multibyte_cht.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_multibyte_jpn.py` & `reportlab-4.0.0/tests/test_multibyte_jpn.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_multibyte_kor.py` & `reportlab-4.0.0/tests/test_multibyte_kor.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_paragraphs.py` & `reportlab-4.0.0/tests/test_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_encodings.py` & `reportlab-4.0.0/tests/test_pdfbase_encodings.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_fontembed.py` & `reportlab-4.0.0/tests/test_pdfbase_fontembed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_pdfdoc.py` & `reportlab-4.0.0/tests/test_pdfbase_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_pdfform.py` & `reportlab-4.0.0/tests/test_pdfbase_pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_pdfmetrics.py` & `reportlab-4.0.0/tests/test_pdfbase_pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_pdfutils.py` & `reportlab-4.0.0/tests/test_pdfbase_pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_postscript.py` & `reportlab-4.0.0/tests/test_pdfbase_postscript.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfbase_ttfonts.py` & `reportlab-4.0.0/tests/test_pdfbase_ttfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfgen_callback.py` & `reportlab-4.0.0/tests/test_pdfgen_callback.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfgen_general.py` & `reportlab-4.0.0/tests/test_pdfgen_general.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setOutDir(__name__)
 import os
 import unittest
 from io import BytesIO
 from reportlab.pdfgen import canvas   # gmcm 2000/10/13, pdfgen now a package
 from reportlab.lib.units import inch, cm
 from reportlab.lib import colors
-from reportlab.lib.utils import haveImages, fileName2FSEnc
+from reportlab.lib.utils import fileName2FSEnc
 from reportlab.lib.boxstuff import rectCorner
 
 #################################################################
 #
 #  first some drawing utilities
 #
 #
@@ -715,81 +715,62 @@
 #
 #  Page 8 - images
 #
 #########################################################################
     framePage(c, "Images")
     c.setFont('Times-Roman', 12)
     t = c.beginText(inch, 10 * inch)
-    if not haveImages:
-        c.drawString(inch, 11*inch,
-                     "Python Imaging Library not found! Below you see rectangles instead of images.")
 
     t.textLines("""PDFgen uses the Python Imaging Library
         to process a very wide variety of image formats.
         This page shows image capabilities.  If I've done things right, the bitmap should have
         its bottom left corner aligned with the crosshairs.
         There are two methods for drawing images.  The recommended use is to call drawImage.
         This produces the smallest PDFs and the fastest generation times as each image's binary data is
         only embedded once in the file.  Also you can use advanced features like transparency masks.
         You can also use drawInlineImage, which puts images in the page stream directly.
         This is slightly faster for Acrobat to render or for very small images, but wastes
         space if you use images more than once.""")
 
     c.drawText(t)
 
-    if haveImages:
-        from reportlab.lib.testutils import testsFolder
-        gif = os.path.join(testsFolder,'pythonpowered.gif')
-        c.drawInlineImage(gif,2*inch, 7*inch)
-        c.drawInlineImage(os.path.join(testsFolder,'pythonpowered-gs.gif'),4*inch, 7.5*inch)
-        tif = os.path.join(testsFolder,'test-cross.tiff')   #example of a mode '1' image
-        c.drawInlineImage(tif,1*inch, 1*inch)
-        from reportlab.lib.utils import Image as PilImage
-        if PilImage:
-            c.drawInlineImage(PilImage.open(tif),1.25*inch, 1*inch)
-    else:
-        c.rect(2*inch, 7*inch, 110, 44)
-        c.rect(4*inch, 7*inch, 110, 44)
+    from reportlab.lib.testutils import testsFolder
+    gif = os.path.join(testsFolder,'pythonpowered.gif')
+    c.drawInlineImage(gif,2*inch, 7*inch)
+    c.drawInlineImage(os.path.join(testsFolder,'pythonpowered-gs.gif'),4*inch, 7.5*inch)
+    tif = os.path.join(testsFolder,'test-cross.tiff')   #example of a mode '1' image
+    c.drawInlineImage(tif,1*inch, 1*inch)
+    from reportlab.lib.utils import Image as PilImage
+    c.drawInlineImage(PilImage.open(tif),1.25*inch, 1*inch)
 
     c.line(1.5*inch, 7*inch, 4*inch, 7*inch)
     c.line(2*inch, 6.5*inch, 2*inch, 8*inch)
     c.drawString(4.5 * inch, 7.25*inch, 'inline image drawn at natural size')
 
-    if haveImages:
-        c.drawInlineImage(gif,2*inch, 5*inch, inch, inch)
-    else:
-        c.rect(2*inch, 5*inch, inch, inch)
+    c.drawInlineImage(gif,2*inch, 5*inch, inch, inch)
 
     c.line(1.5*inch, 5*inch, 4*inch, 5*inch)
     c.line(2*inch, 4.5*inch, 2*inch, 6*inch)
     c.drawString(4.5 * inch, 5.25*inch, 'inline image distorted to fit box')
 
     c.drawString(1.5 * inch, 4*inch, 'Image XObjects can be defined once in the file and drawn many times.')
     c.drawString(1.5 * inch, 3.75*inch, 'This results in faster generation and much smaller files.')
 
     for i in range(5):
-        if haveImages:
-            (w, h) = c.drawImage(gif, (1.5 + i)*inch, 3*inch)
-        else:
-            (w, h) = (144, 10)
-            c.rect((1.5 + i)*inch, 3*inch, 110, 44)
+        (w, h) = c.drawImage(gif, (1.5 + i)*inch, 3*inch)
 
     myMask = [254,255,222,223,0,1]
     c.drawString(1.5 * inch, 2.5*inch, "The optional 'mask' parameter lets you define transparent colors. We used a color picker")
     c.drawString(1.5 * inch, 2.3*inch, "to determine that the yellow in the image above is RGB=(225,223,0).  We then define a mask")
     c.drawString(1.5 * inch, 2.1*inch, "spanning these RGB values:  %s.  The background vanishes!!" % myMask)
     c.drawString(2.5*inch, 1.2*inch, 'This would normally be obscured')
-    if haveImages:
-        c.drawImage(gif, 1*inch, 1.2*inch, w, h, mask=myMask)
-        c.drawImage(gif, 3*inch, 1.2*inch, w, h, mask='auto')
-        c.drawImage(os.path.join(testsFolder,'test-rgba.png'),5*inch,1.2*inch,width=10,height=10,mask='auto')
-        c.drawImage(os.path.join(testsFolder,'test-indexed.png'),5.5*inch,1.2*inch,width=10,height=10,mask='auto')
-    else:
-        c.rect(1*inch, 1.2*inch, w, h)
-        c.rect(3*inch, 1.2*inch, w, h)
+    c.drawImage(gif, 1*inch, 1.2*inch, w, h, mask=myMask)
+    c.drawImage(gif, 3*inch, 1.2*inch, w, h, mask='auto')
+    c.drawImage(os.path.join(testsFolder,'test-rgba.png'),5*inch,1.2*inch,width=10,height=10,mask='auto')
+    c.drawImage(os.path.join(testsFolder,'test-indexed.png'),5.5*inch,1.2*inch,width=10,height=10,mask='auto')
 
     c.showPage()
     c.drawString(1*inch, 10.25*inch, "For rgba type images we can use the alpha channel if we set mask='auto'.")
     c.drawString(1*inch, 10.25*inch-14.4, "The first image is solid red with variable alpha.")
     c.drawString(1*inch, 10.25*inch-2*14.4, "The second image is white alpha=0% to purple=100%")
 
 
@@ -800,122 +781,120 @@
         c.drawString(3*inch,6*inch+i*14.4,"mask='auto' Line %d"%i)
     w = 100
     h = 75
     c.rect(1*inch, 8+14.4*inch, w, h)
     c.rect(3*inch, 8+14.4*inch, w, h)
     c.rect(1*inch, 6+14.4*inch, w, h)
     c.rect(3*inch, 6+14.4*inch, w, h)
-    if haveImages:
-        from reportlab.lib.testutils import testsFolder
-        png = os.path.join(testsFolder,'solid_red_alpha.png')
-        c.drawImage(png, 1*inch, 8*inch+14.4, w, h, mask=None)
-        c.drawImage(png, 3*inch, 8*inch+14.4, w, h, mask='auto')
-        png = os.path.join(testsFolder,'alpha_test.png')
-        c.drawImage(png, 1*inch, 6*inch+14.4, w, h, mask=None)
-        c.drawImage(png, 3*inch, 6*inch+14.4, w, h, mask='auto')
-    c.showPage()
-
-    if haveImages:
-        import shutil
-        c.drawString(1*inch, 10.25*inch, 'This jpeg is actually a gif')
-        jpg = outputfile('_i_am_actually_a_gif.jpg')
-        shutil.copyfile(gif,jpg)
-        c.drawImage(jpg, 1*inch, 9.25*inch, w, h, mask='auto')
-        tjpg = os.path.join(os.path.dirname(os.path.dirname(gif)),'docs','images','lj8100.jpg')
-        if os.path.isfile(tjpg):
-            c.drawString(4*inch, 10.25*inch, 'This gif is actually a jpeg')
-            tgif = outputfile(os.path.basename('_i_am_actually_a_jpeg.gif'))
-            shutil.copyfile(tjpg,tgif)
-            c.drawImage(tgif, 4*inch, 9.25*inch, w, h, mask='auto')
-
-        c.drawString(inch, 9.0*inch, 'Image positioning tests with preserveAspectRatio')
-
-        #preserveAspectRatio test
-        c.drawString(inch, 8.8*inch, 'Both of these should appear within the boxes, vertically centered')
-
-
-        x, y, w, h = inch, 6.75* inch, 2*inch, 2*inch
-        c.rect(x, y, w, h)
-        (w2, h2) = c.drawImage(gif,  #anchor southwest, drawImage
-                    x, y, width=w, height=h,
-                    preserveAspectRatio=True,
-                    anchor='c'
-                    )
-
-        #now test drawInlineImage across the page
-        x = 5 * inch
-        c.rect(x, y, w, h)
-        (w2, h2) = c.drawInlineImage(gif,  #anchor southwest, drawInlineImage
-                    x, y, width=w, height=h,
-                    preserveAspectRatio=True,
-                    anchor='c'
-                    )
-
-        c.drawString(inch, 5.75*inch,
-        'anchored by respective corners - use both a wide and a tall one as tests')
-        x = 0.25 * inch
-        y = 5*inch
-        for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
-            x += 0.75*inch
-            c.rect(x, y, 0.6*inch, 0.6*inch)
-            c.drawImage(
-                    gif, x, y,
-                    width=0.6*inch, height=0.6*inch,
-                    preserveAspectRatio=True,
-                    anchor=anchor
-                    )
-            c.drawString(x, y-0.1*inch, anchor)
-
-        x = 0.25 * inch
-        y = 4*inch
-        tall_red = os.path.join(testsFolder,'tall_red.png')
-        for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
-            x += 0.75*inch
-            c.rect(x, y, 0.6*inch, 0.6*inch)
-            c.drawImage(
-                    tall_red, x, y,
-                    width=0.6*inch, height=0.6*inch,
-                    preserveAspectRatio=True,
-                    anchor=anchor
-                    )
-            c.drawString(x, y-0.1*inch, anchor)
-
-        #Andy's positioning code fails for this case when the image is not reaching the limit
-        x = 0.25 * inch
-        y = 3*inch
-        tall_red = os.path.join(testsFolder,'tall_red.png')
-        for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
-            x += 0.75*inch
-            c.rect(x, 3*inch, 0.7*inch, 0.7*inch)
-            c.drawImage(
-                    tall_red, x, 3*inch,
-                    width=0.6*inch, height=0.6*inch,
-                    preserveAspectRatio=True,
-                    anchor=anchor
-                    )
-            c.drawString(x, y-0.1*inch, anchor)
-
-        #fix by using anchorAtXY
-        x = 0.25 * inch
-        y = 2*inch
-        tall_red = os.path.join(testsFolder,'tall_red.png')
-        for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
-            x += 0.75*inch
-            c.rect(x, y, 0.7*inch, 0.7*inch)
-            ax, ay = rectCorner(x, y, 0.7*inch, 0.7*inch, anchor)
-            c.drawImage(
-                    tall_red, ax, ay,
-                    width=0.6*inch, height=0.6*inch,
-                    preserveAspectRatio=True,
-                    anchor=anchor,
-                    anchorAtXY=True,
-                    )
-            c.drawString(x, y-0.1*inch, anchor)
+    from reportlab.lib.testutils import testsFolder
+    png = os.path.join(testsFolder,'solid_red_alpha.png')
+    c.drawImage(png, 1*inch, 8*inch+14.4, w, h, mask=None)
+    c.drawImage(png, 3*inch, 8*inch+14.4, w, h, mask='auto')
+    png = os.path.join(testsFolder,'alpha_test.png')
+    c.drawImage(png, 1*inch, 6*inch+14.4, w, h, mask=None)
+    c.drawImage(png, 3*inch, 6*inch+14.4, w, h, mask='auto')
+    c.showPage()
+
+    import shutil
+    c.drawString(1*inch, 10.25*inch, 'This jpeg is actually a gif')
+    jpg = outputfile('_i_am_actually_a_gif.jpg')
+    shutil.copyfile(gif,jpg)
+    c.drawImage(jpg, 1*inch, 9.25*inch, w, h, mask='auto')
+    tjpg = os.path.join(os.path.dirname(os.path.dirname(gif)),'docs','images','lj8100.jpg')
+    if os.path.isfile(tjpg):
+        c.drawString(4*inch, 10.25*inch, 'This gif is actually a jpeg')
+        tgif = outputfile(os.path.basename('_i_am_actually_a_jpeg.gif'))
+        shutil.copyfile(tjpg,tgif)
+        c.drawImage(tgif, 4*inch, 9.25*inch, w, h, mask='auto')
+
+    c.drawString(inch, 9.0*inch, 'Image positioning tests with preserveAspectRatio')
+
+    #preserveAspectRatio test
+    c.drawString(inch, 8.8*inch, 'Both of these should appear within the boxes, vertically centered')
+
+
+    x, y, w, h = inch, 6.75* inch, 2*inch, 2*inch
+    c.rect(x, y, w, h)
+    (w2, h2) = c.drawImage(gif,  #anchor southwest, drawImage
+                x, y, width=w, height=h,
+                preserveAspectRatio=True,
+                anchor='c'
+                )
+
+    #now test drawInlineImage across the page
+    x = 5 * inch
+    c.rect(x, y, w, h)
+    (w2, h2) = c.drawInlineImage(gif,  #anchor southwest, drawInlineImage
+                x, y, width=w, height=h,
+                preserveAspectRatio=True,
+                anchor='c'
+                )
+
+    c.drawString(inch, 5.75*inch,
+    'anchored by respective corners - use both a wide and a tall one as tests')
+    x = 0.25 * inch
+    y = 5*inch
+    for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
+        x += 0.75*inch
+        c.rect(x, y, 0.6*inch, 0.6*inch)
+        c.drawImage(
+                gif, x, y,
+                width=0.6*inch, height=0.6*inch,
+                preserveAspectRatio=True,
+                anchor=anchor
+                )
+        c.drawString(x, y-0.1*inch, anchor)
+
+    x = 0.25 * inch
+    y = 4*inch
+    tall_red = os.path.join(testsFolder,'tall_red.png')
+    for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
+        x += 0.75*inch
+        c.rect(x, y, 0.6*inch, 0.6*inch)
+        c.drawImage(
+                tall_red, x, y,
+                width=0.6*inch, height=0.6*inch,
+                preserveAspectRatio=True,
+                anchor=anchor
+                )
+        c.drawString(x, y-0.1*inch, anchor)
+
+    #Andy's positioning code fails for this case when the image is not reaching the limit
+    x = 0.25 * inch
+    y = 3*inch
+    tall_red = os.path.join(testsFolder,'tall_red.png')
+    for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
+        x += 0.75*inch
+        c.rect(x, 3*inch, 0.7*inch, 0.7*inch)
+        c.drawImage(
+                tall_red, x, 3*inch,
+                width=0.6*inch, height=0.6*inch,
+                preserveAspectRatio=True,
+                anchor=anchor
+                )
+        c.drawString(x, y-0.1*inch, anchor)
+
+    #fix by using anchorAtXY
+    x = 0.25 * inch
+    y = 2*inch
+    tall_red = os.path.join(testsFolder,'tall_red.png')
+    for anchor in ('nw','n','ne','w','c','e','sw','s','se'):
+        x += 0.75*inch
+        c.rect(x, y, 0.7*inch, 0.7*inch)
+        ax, ay = rectCorner(x, y, 0.7*inch, 0.7*inch, anchor)
+        c.drawImage(
+                tall_red, ax, ay,
+                width=0.6*inch, height=0.6*inch,
+                preserveAspectRatio=True,
+                anchor=anchor,
+                anchorAtXY=True,
+                )
+        c.drawString(x, y-0.1*inch, anchor)
 
-        c.showPage()
+    c.showPage()
 
 
 #########################################################################
 #
 #  Page 9 - Forms and simple links
 #
 #########################################################################
@@ -976,25 +955,27 @@
 
     ############# colour gradients
     title = 'Gradients code contributed by Peter Johnson <johnson.peter@gmail.com>'
     c.drawString(1*inch,10.8*inch,title)
     c.addOutlineEntry(title+" section", title, level=0, closed=True)
     c.bookmarkHorizontalAbsolute(title, 10.8*inch)
 
+    c.drawString(0.75*inch, 2.25*inch, "This is the End my only Friend the End and I like it :)")
     c.saveState()
     p = c.beginPath()
     p.moveTo(1*inch,2*inch)
     p.lineTo(1.5*inch,2.5*inch)
     p.curveTo(2*inch,3*inch,3.0*inch,3*inch,4*inch,2.9*inch)
     p.lineTo(5.5*inch,2.1*inch)
     p.close()
-    c.clipPath(p)
+    c.clipPath(p, stroke=0)
 
     # Draw a linear gradient from (0, 2*inch) to (5*inch, 3*inch), from orange to white.
     # The gradient will extend past the endpoints (so you probably want a clip path in place)
+    c._setFillAlpha(0.8)
     c.linearGradient(1*inch, 2*inch, 6*inch, 3*inch, (red, blue))
     c.restoreState()
 
     # Draw a radial gradient with a radius of 3 inches.
     # The color starts orange and stays orange until 20% of the radius,
     # then fades to white at 80%, and ends up green at 3 inches from the center.
     # Since extend is false, the gradient stops drawing at the edge of the circle.
```

### Comparing `reportlab-3.6.9/tests/test_pdfgen_links.py` & `reportlab-4.0.0/tests/test_pdfgen_links.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfgen_overprint.py` & `reportlab-4.0.0/tests/test_pdfgen_overprint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pdfgen_pagemodes.py` & `reportlab-4.0.0/tests/test_pdfgen_pagemodes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_accum.py` & `reportlab-4.0.0/tests/test_platypus_accum.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_breaking.py` & `reportlab-4.0.0/tests/test_platypus_breaking.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_cjk_wrap.py` & `reportlab-4.0.0/tests/test_platypus_cjk_wrap.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_general.py` & `reportlab-4.0.0/tests/test_platypus_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,22 @@
 from reportlab.platypus import BaseDocTemplate, PageTemplate, Flowable, FrameBreak, KeepTogether, PageBreak, Spacer
 from reportlab.platypus import Paragraph, Preformatted
 from reportlab.platypus import SimpleDocTemplate
 from reportlab.lib.units import inch, cm
 from reportlab.lib.styles import PropertySet, getSampleStyleSheet, ParagraphStyle
 from reportlab.lib import colors
 from reportlab.rl_config import defaultPageSize
-from reportlab.lib.utils import haveImages, _RL_DIR, rl_isfile, open_for_read, fileName2FSEnc, asNative
+from reportlab.lib.utils import _RL_DIR, rl_isfile, open_for_read, fileName2FSEnc, asNative
 import unittest
 from reportlab.lib.testutils import testsFolder
-if haveImages:
-    _GIF = os.path.join(testsFolder,'pythonpowered.gif')
-    if not rl_isfile(_GIF): _GIF = None
-    _GAPNG = os.path.join(testsFolder,'gray-alpha.png')
-    if not rl_isfile(_GAPNG): _GAPNG = None
-else:
-    _GIF = None
+
+_GIF = os.path.join(testsFolder,'pythonpowered.gif')
+if not rl_isfile(_GIF): _GIF = None
+_GAPNG = os.path.join(testsFolder,'gray-alpha.png')
+if not rl_isfile(_GAPNG): _GAPNG = None
 if _GIF: _GIFFSEnc=fileName2FSEnc(_GIF)
 if _GAPNG: _GAPNGFSEnc=fileName2FSEnc(_GAPNG)
 
 _JPG = os.path.join(testsFolder,'..','docs','images','lj8100.jpg')
 if not rl_isfile(_JPG): _JPG = None
 
 def getFurl(fn):
```

### Comparing `reportlab-3.6.9/tests/test_platypus_images.py` & `reportlab-4.0.0/tests/test_platypus_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,21 @@
     return 'file://'+furl
 
 def run():
     from reportlab.platypus import  BaseDocTemplate, PageTemplate, Image, Frame, PageTemplate, \
                                     ShowBoundaryValue, SimpleDocTemplate, FrameBG, Paragraph, \
                                     FrameBreak
     from reportlab.lib.colors import toColor
-    from reportlab.lib.utils import haveImages, _RL_DIR, rl_isfile, open_for_read, fileName2FSEnc, asNative
+    from reportlab.lib.utils import _RL_DIR, rl_isfile, open_for_read, fileName2FSEnc, asNative
     from reportlab.lib.styles import getSampleStyleSheet
     styleSheet = getSampleStyleSheet()
-    if haveImages:
-        _GIF = os.path.join(testsFolder,'pythonpowered.gif')
-        if not rl_isfile(_GIF): _GIF = None
-        _GAPNG = os.path.join(testsFolder,'gray-alpha.png')
-        if not rl_isfile(_GAPNG): _GAPNG = None
-    else:
-        _GIF = None
+    _GIF = os.path.join(testsFolder,'pythonpowered.gif')
+    if not rl_isfile(_GIF): _GIF = None
+    _GAPNG = os.path.join(testsFolder,'gray-alpha.png')
+    if not rl_isfile(_GAPNG): _GAPNG = None
     if _GIF: _GIFFSEnc=fileName2FSEnc(_GIF)
     if _GAPNG: _GAPNGFSEnc=fileName2FSEnc(_GAPNG)
 
     _JPG = os.path.join(testsFolder,'..','docs','images','lj8100.jpg')
     if not rl_isfile(_JPG): _JPG = None
```

### Comparing `reportlab-3.6.9/tests/test_platypus_indents.py` & `reportlab-4.0.0/tests/test_platypus_indents.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_index.py` & `reportlab-4.0.0/tests/test_platypus_index.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_leftright.py` & `reportlab-4.0.0/tests/test_platypus_leftright.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_lists.py` & `reportlab-4.0.0/tests/test_platypus_lists.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_paragraphs.py` & `reportlab-4.0.0/tests/test_platypus_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_paraparser.py` & `reportlab-4.0.0/tests/test_platypus_paraparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_pleaseturnover.py` & `reportlab-4.0.0/tests/test_platypus_pleaseturnover.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_preformatted.py` & `reportlab-4.0.0/tests/test_platypus_preformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_programming.py` & `reportlab-4.0.0/tests/test_platypus_programming.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_tables.py` & `reportlab-4.0.0/tests/test_platypus_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_toc.py` & `reportlab-4.0.0/tests/test_platypus_toc.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,32 +33,35 @@
     "The page frame used for all PDF documents."
 
     canvas.saveState()
 
     canvas.rect(2.5*cm, 2.5*cm, 15*cm, 25*cm)
     canvas.setFont('Times-Roman', 12)
     pageNumber = canvas.getPageNumber()
-    canvas.drawString(10*cm, cm, str(pageNumber))
+    if doc.rLPN:
+        pns = 'page %d of %d' % (pageNumber,doc._lpn0)
+    else:
+        pns = str(pageNumber)
+    canvas.drawCentredString(10*cm, cm, pns)
 
     canvas.restoreState()
 
-
 class MyDocTemplate(BaseDocTemplate):
     "The document template used for all PDF documents."
 
     _invalidInitArgs = ('pageTemplates',)
+    rLPN = False    #record last page number
 
     def __init__(self, filename, **kw):
         frame1 = Frame(2.5*cm, 2.5*cm, 15*cm, 25*cm, id='F1')
         self.allowSplitting = 0
         BaseDocTemplate.__init__(self, filename, **kw)
         template = PageTemplate('normal', [frame1], myMainPageFrame)
         self.addPageTemplates(template)
 
-
     def afterFlowable(self, flowable):
         "Registers TOC entries."
 
         if flowable.__class__.__name__ == 'Paragraph':
             styleName = flowable.style.name
             if styleName[:7] == 'Heading':
                 key = str(hash(flowable))
@@ -71,14 +74,30 @@
                 # Try calling this with and without a key to test both
                 # Entries of every second level will have links, others won't
                 if level % 2 == 1:
                     self.notify('TOCEntry', (level, text, pageNum, key))
                 else:
                     self.notify('TOCEntry', (level, text, pageNum))
 
+    def beforeDocument(self):
+        if self.rLPN:
+            self._lpn0 = getattr(self,'_lpn',-100)
+            self._lpn = 0
+        super().beforeDocument()
+
+    def beforePage(self):
+        if self.rLPN:
+            self._lpn = self.canv.getPageNumber()
+        super().beforePage()
+
+    def _allSatisfied(self):
+        r = super()._allSatisfied()
+        if r and self.rLPN:
+            r = self._lpn0==self._lpn
+        return r
 
 def makeHeaderStyle(level, fontName='Times-Roman'):
     "Make a header style for different levels."
 
     assert level >= 0, "Level must be >= 0."
 
     PS = ParagraphStyle
@@ -130,55 +149,57 @@
         Features to be visually confirmed by a human being are:
 
             1. TOC lines are indented in multiples of 1 cm.
             2. Wrapped TOC lines continue with additional 0.5 cm indentation.
             3. Only entries of every second level has links
             ...
         """
-        if rl_invariant: random.seed(2077179149)
-        maxLevels = 12
-
-        # Create styles to be used for document headers
-        # on differnet levels.
-        headerLevelStyles = []
-        for i in range(maxLevels):
-            headerLevelStyles.append(makeHeaderStyle(i))
-
-        # Create styles to be used for TOC entry lines
-        # for headers on differnet levels.
-        tocLevelStyles = []
-        d, e = tableofcontents.delta, tableofcontents.epsilon
-        for i in range(maxLevels):
-            tocLevelStyles.append(makeTocHeaderStyle(i, d, e))
-
-        # Build story.
-        story = []
-        styleSheet = getSampleStyleSheet()
-        bt = styleSheet['BodyText']
-
-        description = '<font color=red>%s</font>' % self.test0.__doc__
-        story.append(XPreformatted(description, bt))
-
-        toc = tableofcontents.TableOfContents(dotsMinLevel=1)
-        toc.levelStyles = tocLevelStyles
-        story.append(toc)
-
-        for i in range(maxLevels):
-            story.append(Paragraph('HEADER, LEVEL %d' % i,
-                                   headerLevelStyles[i]))
-            #now put some body stuff in.
-            txt = xmlEscape(randomtext.randomText(randomtext.PYTHON, 5))
-            para = Paragraph(txt, makeBodyStyle())
-            story.append(para)
-
-        path = outputfile('test_platypus_toc.pdf')
-        doc = MyDocTemplate(path)
-        doc.multiBuild(story)
-
-
+        def doTest(rLPN=False):
+            if rl_invariant: random.seed(2077179149)
+            maxLevels = 12
+
+            # Create styles to be used for document headers
+            # on differnet levels.
+            headerLevelStyles = []
+            for i in range(maxLevels):
+                headerLevelStyles.append(makeHeaderStyle(i))
+
+            # Create styles to be used for TOC entry lines
+            # for headers on differnet levels.
+            tocLevelStyles = []
+            d, e = tableofcontents.delta, tableofcontents.epsilon
+            for i in range(maxLevels):
+                tocLevelStyles.append(makeTocHeaderStyle(i, d, e))
+
+            # Build story.
+            story = []
+            styleSheet = getSampleStyleSheet()
+            bt = styleSheet['BodyText']
+
+            description = '<font color=red>%s</font>' % self.test0.__doc__
+            story.append(XPreformatted(description, bt))
+
+            toc = tableofcontents.TableOfContents(dotsMinLevel=1)
+            toc.levelStyles = tocLevelStyles
+            story.append(toc)
+
+            for i in range(maxLevels):
+                story.append(Paragraph('HEADER, LEVEL %d' % i,
+                                       headerLevelStyles[i]))
+                #now put some body stuff in.
+                txt = xmlEscape(randomtext.randomText(randomtext.PYTHON, 5))
+                para = Paragraph(txt, makeBodyStyle())
+                story.append(para)
+
+            path = outputfile('test_platypus_toc%s.pdf' % ('_page_x_of_y' if rLPN else ''))
+            doc = MyDocTemplate(path)
+            doc.rLPN = rLPN
+            doc.multiBuild(story)
+        doTest(False)
+        doTest(True)
 
     def test1(self):
         """This shows a table which would take more than one page,
         and need multiple passes to render.  But we preload it
         with the right headings to make it go faster.  We used
         a simple 100-chapter document with one level.
         """
```

### Comparing `reportlab-3.6.9/tests/test_platypus_wrapping.py` & `reportlab-4.0.0/tests/test_platypus_wrapping.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_platypus_xref.py` & `reportlab-4.0.0/tests/test_platypus_xref.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_pyfiles.py` & `reportlab-4.0.0/tests/test_pyfiles.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_renderPS.py` & `reportlab-4.0.0/tests/test_renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_renderSVG.py` & `reportlab-4.0.0/tests/test_renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_rl_accel.py` & `reportlab-4.0.0/tests/test_rl_accel.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_source_chars.py` & `reportlab-4.0.0/tests/test_source_chars.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_tools_pythonpoint.py` & `reportlab-4.0.0/tests/test_tools_pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_utils.py` & `reportlab-4.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_widgetbase_tpc.py` & `reportlab-4.0.0/tests/test_widgetbase_tpc.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tests/test_widgets_grids.py` & `reportlab-4.0.0/tests/test_widgets_grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/codegrab.py` & `reportlab-4.0.0/tools/docco/codegrab.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/docpy.py` & `reportlab-4.0.0/tools/docco/docpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/examples.py` & `reportlab-4.0.0/tools/docco/examples.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/graphdocpy.py` & `reportlab-4.0.0/tools/docco/graphdocpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/rl_doc_utils.py` & `reportlab-4.0.0/tools/docco/rl_doc_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/rltemplate.py` & `reportlab-4.0.0/tools/docco/rltemplate.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/stylesheet.py` & `reportlab-4.0.0/tools/docco/stylesheet.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/t_parse.py` & `reportlab-4.0.0/tools/docco/t_parse.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/yaml.py` & `reportlab-4.0.0/tools/docco/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/docco/yaml2pdf.py` & `reportlab-4.0.0/tools/docco/yaml2pdf.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pdfpath.py` & `reportlab-4.0.0/tools/pdfpath.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/README` & `reportlab-4.0.0/tools/pythonpoint/README`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/customshapes.py` & `reportlab-4.0.0/tools/pythonpoint/customshapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/examples.py` & `reportlab-4.0.0/tools/pythonpoint/demos/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     canvas.setSubject("How to Generate PDF files using the ReportLab modules")
 """
 
 # magic function making module
 
 test1 = """
 def f(a,b):
-    print "it worked", a, b
+    print("it worked", a, b)
     return a+b
 """
 
 test2 = """
 def g(n):
     if n==0: return 1
     else: return n*g(n-1)
-    """
+"""
 
 testhello = """
 def hello(c):
     from reportlab.lib.units import inch
     # move the origin up and to the left
     c.translate(inch,inch)
     # define a large font
@@ -777,29 +777,26 @@
 ##        drawing = testdrawings.getDrawing3()
 ##        canvas.saveState()
 ##        canvas.scale(self.scale, self.scale)
 ##        pingopdf.draw(drawing, canvas, self.x, self.y)
 ##        canvas.restoreState()
 
 # D = dir()
-g = globals()
-Dprime = {}
-for a,b in list(g.items()):
-    if a[:4]=="test" and isinstance(b,str):
-        #print 'for', a
-        #print b
+TESTS=[(a,b) for a, b in globals().items() if a.startswith('test')]
+for a,b in TESTS:
+    if isinstance(b,str):
         b = b.strip()
         exec(b+'\n')
 
 platypussetup = """
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer
 from reportlab.lib.styles import getSampleStyleSheet
-from reportlab.lib.pagesizes import DEFAULT_PAGE_SIZE
+from reportlab.rl_config import defaultPageSize
 from reportlab.lib.units import inch
-PAGE_HEIGHT=DEFAULT_PAGE_SIZE[1]; PAGE_WIDTH=DEFAULT_PAGE_SIZE[0]
+PAGE_HEIGHT=defaultPageSize[1]; PAGE_WIDTH=defaultPageSize[0]
 styles = getSampleStyleSheet()
 """
 platypusfirstpage = """
 Title = "Hello world"
 pageinfo = "platypus example"
 def myFirstPage(canvas, doc):
     canvas.saveState()
```

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/figures.xml` & `reportlab-4.0.0/tools/pythonpoint/demos/figures.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/htu.xml` & `reportlab-4.0.0/tools/pythonpoint/demos/htu.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.a85` & `reportlab-4.0.0/tools/pythonpoint/demos/leftlogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/leftlogo.gif` & `reportlab-4.0.0/tools/pythonpoint/demos/leftlogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/lj8100.jpg` & `reportlab-4.0.0/tools/pythonpoint/demos/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/monterey.xml` & `reportlab-4.0.0/tools/pythonpoint/demos/monterey.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/outline.gif` & `reportlab-4.0.0/tools/pythonpoint/demos/outline.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/pplogo.gif` & `reportlab-4.0.0/tools/pythonpoint/demos/pplogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/python.gif` & `reportlab-4.0.0/tools/pythonpoint/demos/python.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/pythonpoint.xml` & `reportlab-4.0.0/tools/pythonpoint/demos/pythonpoint.xml`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/slidebox.py` & `reportlab-4.0.0/tools/pythonpoint/demos/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/spectrum.png` & `reportlab-4.0.0/tools/pythonpoint/demos/spectrum.png`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/demos/vertpython.gif` & `reportlab-4.0.0/tools/pythonpoint/demos/vertpython.gif`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/pythonpoint.dtd` & `reportlab-4.0.0/tools/pythonpoint/pythonpoint.dtd`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/pythonpoint.py` & `reportlab-4.0.0/tools/pythonpoint/pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/stdparser.py` & `reportlab-4.0.0/tools/pythonpoint/stdparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/styles/horrible.py` & `reportlab-4.0.0/tools/pythonpoint/styles/horrible.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/styles/htu.py` & `reportlab-4.0.0/tools/pythonpoint/styles/htu.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/styles/modern.py` & `reportlab-4.0.0/tools/pythonpoint/styles/modern.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/styles/projection.py` & `reportlab-4.0.0/tools/pythonpoint/styles/projection.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/pythonpoint/styles/standard.py` & `reportlab-4.0.0/tools/pythonpoint/styles/standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/utils/add_bleed.py` & `reportlab-4.0.0/tools/utils/add_bleed.py`

 * *Files identical despite different names*

### Comparing `reportlab-3.6.9/tools/utils/dumpttf.py` & `reportlab-4.0.0/tools/utils/dumpttf.py`

 * *Files identical despite different names*

