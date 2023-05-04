# Comparing `tmp/diffpy.pdfgui-1.4.2.tar.gz` & `tmp/diffpy.pdfgui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffpy.pdfgui-1.4.2.tar", last modified: Wed Feb  8 03:46:52 2023, max compression
+gzip compressed data, was "diffpy.pdfgui-2.0.0.tar", last modified: Thu May  4 14:25:10 2023, max compression
```

## Comparing `diffpy.pdfgui-1.4.2.tar` & `diffpy.pdfgui-2.0.0.tar`

### file list

```diff
@@ -1,253 +1,350 @@
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.758108 diffpy.pdfgui-1.4.2/
--rw-r--r--   0 longyang   (501) staff       (20)     2145 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/AUTHORS.txt
--rw-r--r--   0 longyang   (501) staff       (20)     2597 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/LICENSE.txt
--rw-r--r--   0 longyang   (501) staff       (20)      717 2023-02-03 08:36:14.000000 diffpy.pdfgui-1.4.2/MANIFEST.in
--rw-r--r--   0 longyang   (501) staff       (20)     6658 2023-02-08 03:46:52.757913 diffpy.pdfgui-1.4.2/PKG-INFO
--rw-r--r--   0 longyang   (501) staff       (20)     5450 2022-12-29 08:11:53.000000 diffpy.pdfgui-1.4.2/README.rst
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.694684 diffpy.pdfgui-1.4.2/doc/
--rw-r--r--   0 longyang   (501) staff       (20)   576472 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/Farrow-jpcm-2007.pdf
--rw-r--r--   0 longyang   (501) staff       (20)   107401 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/Proffen-jac-1999.pdf
--rw-r--r--   0 longyang   (501) staff       (20)     7680 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/TUTORIAL.txt
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.696013 diffpy.pdfgui-1.4.2/doc/manual/
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.706819 diffpy.pdfgui-1.4.2/doc/manual/images/
--rw-r--r--   0 longyang   (501) staff       (20)     1636 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/eq-01.png
--rw-r--r--   0 longyang   (501) staff       (20)     3162 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/eq-02.png
--rw-r--r--   0 longyang   (501) staff       (20)    60550 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-01.png
--rw-r--r--   0 longyang   (501) staff       (20)    56998 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-02.png
--rw-r--r--   0 longyang   (501) staff       (20)    57963 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-03.png
--rw-r--r--   0 longyang   (501) staff       (20)    41156 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-04.png
--rw-r--r--   0 longyang   (501) staff       (20)    48960 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-05.png
--rw-r--r--   0 longyang   (501) staff       (20)    34580 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-06.png
--rw-r--r--   0 longyang   (501) staff       (20)    43240 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-07.png
--rw-r--r--   0 longyang   (501) staff       (20)    47440 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-08.png
--rw-r--r--   0 longyang   (501) staff       (20)   139699 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-09.png
--rw-r--r--   0 longyang   (501) staff       (20)    62258 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-10.png
--rw-r--r--   0 longyang   (501) staff       (20)    47464 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig2-11.png
--rw-r--r--   0 longyang   (501) staff       (20)    59512 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-01.png
--rw-r--r--   0 longyang   (501) staff       (20)    57874 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-02.png
--rw-r--r--   0 longyang   (501) staff       (20)    39343 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-03.png
--rw-r--r--   0 longyang   (501) staff       (20)    71799 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-04.png
--rw-r--r--   0 longyang   (501) staff       (20)    45670 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-05.png
--rw-r--r--   0 longyang   (501) staff       (20)    62481 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-06.png
--rw-r--r--   0 longyang   (501) staff       (20)    74614 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-07.png
--rw-r--r--   0 longyang   (501) staff       (20)    60180 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-08.png
--rw-r--r--   0 longyang   (501) staff       (20)    71868 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-09.png
--rw-r--r--   0 longyang   (501) staff       (20)   109109 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig3-10.png
--rw-r--r--   0 longyang   (501) staff       (20)    62258 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig4-01.png
--rw-r--r--   0 longyang   (501) staff       (20)    80574 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/images/fig4-02.png
--rw-r--r--   0 longyang   (501) staff       (20)   174161 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/doc/manual/pdfgui.html
--rw-r--r--   0 longyang   (501) staff       (20)  1487431 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/manual/pdfgui.pdf
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.719214 diffpy.pdfgui-1.4.2/doc/tutorial/
--rw-r--r--   0 longyang   (501) staff       (20)    74438 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/1050K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74438 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/1100K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74438 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/1150K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74440 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/300K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74446 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/550K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/650K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/700K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/720K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/730K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/740K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/750K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/800K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/880K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74436 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/980K.gr
--rw-r--r--   0 longyang   (501) staff       (20)   316322 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-3nm.gr
--rw-r--r--   0 longyang   (501) staff       (20)   316398 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-bulk.gr
--rw-r--r--   0 longyang   (501) staff       (20)  1001536 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-nano.ddp
--rw-r--r--   0 longyang   (501) staff       (20)     1856 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-wurtzite.stru
--rw-r--r--   0 longyang   (501) staff       (20)    74135 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/Ni-neutron.gr
--rw-r--r--   0 longyang   (501) staff       (20)   143812 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/Ni-xray.gr
--rw-r--r--   0 longyang   (501) staff       (20)     1830 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/Ni.stru
--rw-r--r--   0 longyang   (501) staff       (20)   130213 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/lcmo-template.ddp
--rw-r--r--   0 longyang   (501) staff       (20)    18461 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/lmo-template.ddp
--rwxr-xr-x   0 longyang   (501) staff       (20)     2572 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/doc/tutorial/tui_mno_bond_lengths.py
--rw-r--r--   0 longyang   (501) staff       (20)    72233 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x000t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x004t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x012t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x016t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x020t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x024t010q35.gr
--rw-r--r--   0 longyang   (501) staff       (20)    72203 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/doc/tutorial/x028t010q35.gr
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.722799 diffpy.pdfgui-1.4.2/icons/
--rw-r--r--   0 longyang   (501) staff       (20)     1079 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/C60_16x16.png
--rw-r--r--   0 longyang   (501) staff       (20)      196 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/calculationitem.png
--rw-r--r--   0 longyang   (501) staff       (20)     8686 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/columbia_logo.png
--rw-r--r--   0 longyang   (501) staff       (20)     9580 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/danse_logo.png
--rw-r--r--   0 longyang   (501) staff       (20)      210 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/datasetitem.png
--rw-r--r--   0 longyang   (501) staff       (20)      468 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/exportplotdata.png
--rw-r--r--   0 longyang   (501) staff       (20)      228 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/fititem.png
--rw-r--r--   0 longyang   (501) staff       (20)      540 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/fitting.png
--rw-r--r--   0 longyang   (501) staff       (20)    28660 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/logo.png
--rw-r--r--   0 longyang   (501) staff       (20)     9646 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/msu_logo.png
--rw-r--r--   0 longyang   (501) staff       (20)     2338 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/nsf_logo.png
--rw-r--r--   0 longyang   (501) staff       (20)    22382 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/pdfgui.ico
--rw-r--r--   0 longyang   (501) staff       (20)      689 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/phaseitem.png
--rw-r--r--   0 longyang   (501) staff       (20)      810 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/plotting.png
--rw-r--r--   0 longyang   (501) staff       (20)      774 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/run.png
--rw-r--r--   0 longyang   (501) staff       (20)      781 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/stop.png
--rw-r--r--   0 longyang   (501) staff       (20)    58355 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/icons/titlepage.png
--rw-r--r--   0 longyang   (501) staff       (20)       38 2023-02-08 03:46:52.758166 diffpy.pdfgui-1.4.2/setup.cfg
--rwxr-xr-x   0 longyang   (501) staff       (20)     5209 2023-02-03 08:30:26.000000 diffpy.pdfgui-1.4.2/setup.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.691016 diffpy.pdfgui-1.4.2/src/
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.723389 diffpy.pdfgui-1.4.2/src/diffpy/
--rw-r--r--   0 longyang   (501) staff       (20)      701 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/__init__.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.726219 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/
--rw-r--r--   0 longyang   (501) staff       (20)      723 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/__init__.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.726647 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/applications/
--rw-r--r--   0 longyang   (501) staff       (20)      555 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/applications/__init__.py
--rwxr-xr-x   0 longyang   (501) staff       (20)     4016 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/applications/pdfgui.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.730661 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/
--rw-r--r--   0 longyang   (501) staff       (20)      535 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/__init__.py
--rw-r--r--   0 longyang   (501) staff       (20)    11876 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/calculation.py
--rw-r--r--   0 longyang   (501) staff       (20)     5431 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/constraint.py
--rw-r--r--   0 longyang   (501) staff       (20)     2037 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/controlerrors.py
--rw-r--r--   0 longyang   (501) staff       (20)    25952 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitdataset.py
--rw-r--r--   0 longyang   (501) staff       (20)    35890 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitstructure.py
--rw-r--r--   0 longyang   (501) staff       (20)    27408 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitting.py
--rw-r--r--   0 longyang   (501) staff       (20)     9484 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/organizer.py
--rw-r--r--   0 longyang   (501) staff       (20)     6928 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/parameter.py
--rw-r--r--   0 longyang   (501) staff       (20)      837 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfcomponent.py
--rw-r--r--   0 longyang   (501) staff       (20)    12373 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfdataset.py
--rw-r--r--   0 longyang   (501) staff       (20)    18863 2023-02-03 08:30:29.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfguicontrol.py
--rw-r--r--   0 longyang   (501) staff       (20)    12929 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfguimacros.py
--rw-r--r--   0 longyang   (501) staff       (20)     3081 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdflist.py
--rw-r--r--   0 longyang   (501) staff       (20)     7100 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfstructure.py
--rw-r--r--   0 longyang   (501) staff       (20)    23156 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/plotter.py
--rw-r--r--   0 longyang   (501) staff       (20)     8448 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/structureviewer.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.742211 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/
--rw-r--r--   0 longyang   (501) staff       (20)     1324 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/DesignNotes.txt
--rw-r--r--   0 longyang   (501) staff       (20)      535 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/__init__.py
--rw-r--r--   0 longyang   (501) staff       (20)     9760 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/aboutdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     7708 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/adddatapanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     9670 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/addphasepanel.py
--rw-r--r--   0 longyang   (501) staff       (20)      918 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/blankpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     5809 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/bondangledialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     8918 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/bondlengthdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)    11146 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/calculationpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    17996 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetconfigurepanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     6368 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetconstraintpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     5006 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     4804 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetresultspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     2637 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/debugoptions.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.747240 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/
--rw-r--r--   0 longyang   (501) staff       (20)    16134 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/aboutdialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     3687 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/adddatapanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     5908 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/addphasepanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    10064 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/bondlengthdialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    15042 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/calculationpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    20525 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetconfigurepanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     4837 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetconstraintpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     4271 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     5548 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetresultspanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    11712 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/dopingseriespanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     5548 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/errorreportdialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     1871 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/fitnotebookpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     4341 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/insertrowsdialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     2849 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/journalpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)      995 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/outputpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     3437 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/parameterspanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    22763 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseconfigurepanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    22831 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseconstraintspanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    22236 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseresultspanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     5596 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/plotpanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     9528 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/preferencespanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     2254 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/resultspanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     9073 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/rseriespanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     8441 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/sgconstraindialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     7550 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/sgstructuredialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     6665 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/supercelldialog.wxg
--rw-r--r--   0 longyang   (501) staff       (20)     9775 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/temperatureseriespanel.wxg
--rw-r--r--   0 longyang   (501) staff       (20)    13799 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/dopingseriespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     8547 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorreportdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     6436 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorreportdialog_control_fix.py
--rw-r--r--   0 longyang   (501) staff       (20)     4408 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorwrapper.py
--rw-r--r--   0 longyang   (501) staff       (20)    14460 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/extendedplotframe.py
--rw-r--r--   0 longyang   (501) staff       (20)     3104 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/fitnotebookpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    35044 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/fittree.py
--rw-r--r--   0 longyang   (501) staff       (20)     3715 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/gui_organization.txt
--rw-r--r--   0 longyang   (501) staff       (20)     2494 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/insertrowsdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     4422 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/journalpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     1284 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/main.py
--rw-r--r--   0 longyang   (501) staff       (20)   100875 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/mainframe.py
--rw-r--r--   0 longyang   (501) staff       (20)     2882 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/menuitems.txt
--rw-r--r--   0 longyang   (501) staff       (20)     2238 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/outputpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     2374 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/paneltest.py
--rw-r--r--   0 longyang   (501) staff       (20)    17269 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/parameterspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     2272 2023-02-03 08:43:51.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/pdfguiglobals.py
--rw-r--r--   0 longyang   (501) staff       (20)     2049 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/pdfpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    31268 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseconfigurepanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    24844 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseconstraintspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     3826 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phasenotebookpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    11500 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phasepanelutils.py
--rw-r--r--   0 longyang   (501) staff       (20)     9724 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseresultspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)    10102 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/plotpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     7532 2023-02-01 15:33:38.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/preferencespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     3085 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/resultspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     7388 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/rseriespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     9761 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/sgconstraindialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     9206 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/sgstructuredialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     4081 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/supercelldialog.py
--rw-r--r--   0 longyang   (501) staff       (20)    13343 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/temperatureseriespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     8744 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/tooltips.py
--rw-r--r--   0 longyang   (501) staff       (20)     1652 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/welcomepanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     3558 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/windowperspective.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.748598 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/
--rw-r--r--   0 longyang   (501) staff       (20)      582 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/__init__.py
--rw-r--r--   0 longyang   (501) staff       (20)     1927 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/autowidthlabelsgrid.py
--rw-r--r--   0 longyang   (501) staff       (20)     6415 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/listctrls.py
--rw-r--r--   0 longyang   (501) staff       (20)     2275 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/paneldialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     1730 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/textctrlutils.py
--rw-r--r--   0 longyang   (501) staff       (20)     3994 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/validators.py
--rw-r--r--   0 longyang   (501) staff       (20)     2612 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/wx12.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.753168 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/
--rw-r--r--   0 longyang   (501) staff       (20)     2953 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/__init__.py
--rw-r--r--   0 longyang   (501) staff       (20)      897 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/debug.py
--rw-r--r--   0 longyang   (501) staff       (20)     1039 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/run.py
--rw-r--r--   0 longyang   (501) staff       (20)      858 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/rundeps.py
--rw-r--r--   0 longyang   (501) staff       (20)     2175 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/showphasenotebookpanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     2067 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testaboutdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     3868 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testcalculation.py
--rw-r--r--   0 longyang   (501) staff       (20)     2575 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testconstraint.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.757401 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/
--rw-r--r--   0 longyang   (501) staff       (20)    74440 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/300K.gr
--rw-r--r--   0 longyang   (501) staff       (20)    74446 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/550K.gr
--rw-r--r--   0 longyang   (501) staff       (20)     1839 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/CdSe_bulk_wur.stru
--rw-r--r--   0 longyang   (501) staff       (20)     7930 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/LaMnO3.stru
--rw-r--r--   0 longyang   (501) staff       (20)    77077 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni.dat
--rw-r--r--   0 longyang   (501) staff       (20)     1830 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni.stru
--rw-r--r--   0 longyang   (501) staff       (20)   143801 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni_2-8.chi.gr
--rw-r--r--   0 longyang   (501) staff       (20)    52256 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo.ddp
--rw-r--r--   0 longyang   (501) staff       (20)     2033 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_00.gr
--rw-r--r--   0 longyang   (501) staff       (20)     2033 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_20.gr
--rw-r--r--   0 longyang   (501) staff       (20)   744064 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_full.ddp
--rw-r--r--   0 longyang   (501) staff       (20)   102347 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/ni.ddp
--rw-r--r--   0 longyang   (501) staff       (20)     3870 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdatasetpanels.py
--rw-r--r--   0 longyang   (501) staff       (20)     1866 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdopingseriespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     2454 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testextendedplotframe.py
--rw-r--r--   0 longyang   (501) staff       (20)     9084 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testfitdataset.py
--rw-r--r--   0 longyang   (501) staff       (20)     9290 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testfitstructure.py
--rw-r--r--   0 longyang   (501) staff       (20)     1387 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testinsertrowsdialog.py
--rw-r--r--   0 longyang   (501) staff       (20)     4143 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testloadproject.py
--rw-r--r--   0 longyang   (501) staff       (20)     1911 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testmainframe.py
--rw-r--r--   0 longyang   (501) staff       (20)     2641 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testparameter.py
--rw-r--r--   0 longyang   (501) staff       (20)     4336 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testparameterspanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     3535 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfdataset.py
--rw-r--r--   0 longyang   (501) staff       (20)     1324 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfguicontrol.py
--rw-r--r--   0 longyang   (501) staff       (20)     4040 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfstructure.py
--rw-r--r--   0 longyang   (501) staff       (20)     2756 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testphaseconfigurepanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     3465 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/teststructureviewer.py
--rw-r--r--   0 longyang   (501) staff       (20)     1904 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testtemperatureseriespanel.py
--rw-r--r--   0 longyang   (501) staff       (20)     5940 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testutils.py
--rw-r--r--   0 longyang   (501) staff       (20)     4599 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tui.py
--rw-r--r--   0 longyang   (501) staff       (20)     3877 2022-12-14 06:22:33.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/utils.py
--rw-r--r--   0 longyang   (501) staff       (20)      133 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/version.cfg
--rw-r--r--   0 longyang   (501) staff       (20)     1647 2022-11-26 03:28:41.000000 diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/version.py
-drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-02-08 03:46:52.724529 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/
--rw-r--r--   0 longyang   (501) staff       (20)     6658 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/PKG-INFO
--rw-r--r--   0 longyang   (501) staff       (20)     8468 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/SOURCES.txt
--rw-r--r--   0 longyang   (501) staff       (20)        1 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/dependency_links.txt
--rw-r--r--   0 longyang   (501) staff       (20)       62 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/entry_points.txt
--rw-r--r--   0 longyang   (501) staff       (20)        1 2022-12-14 03:46:27.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/not-zip-safe
--rw-r--r--   0 longyang   (501) staff       (20)       52 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/requires.txt
--rw-r--r--   0 longyang   (501) staff       (20)        7 2023-02-08 03:46:52.000000 diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/top_level.txt
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.231887 diffpy.pdfgui-2.0.0/
+-rw-r--r--   0 longyang   (501) staff       (20)     2145 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/AUTHORS.txt
+-rw-r--r--   0 longyang   (501) staff       (20)     4383 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/LICENSE.txt
+-rw-r--r--   0 longyang   (501) staff       (20)      717 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/MANIFEST.in
+-rw-r--r--   0 longyang   (501) staff       (20)     6633 2023-05-04 14:25:10.231690 diffpy.pdfgui-2.0.0/PKG-INFO
+-rw-r--r--   0 longyang   (501) staff       (20)     5425 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/README.rst
+-rw-r--r--   0 longyang   (501) staff       (20)       38 2023-05-04 14:25:10.231948 diffpy.pdfgui-2.0.0/setup.cfg
+-rwxr-xr-x   0 longyang   (501) staff       (20)     5209 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/setup.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.146103 diffpy.pdfgui-2.0.0/src/
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.148878 diffpy.pdfgui-2.0.0/src/diffpy/
+-rw-r--r--   0 longyang   (501) staff       (20)      701 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/__init__.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.151492 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/
+-rw-r--r--   0 longyang   (501) staff       (20)      723 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/__init__.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.152215 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/applications/
+-rw-r--r--   0 longyang   (501) staff       (20)      555 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/applications/__init__.py
+-rwxr-xr-x   0 longyang   (501) staff       (20)     4017 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/applications/pdfgui.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.155303 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/
+-rw-r--r--   0 longyang   (501) staff       (20)      535 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/__init__.py
+-rw-r--r--   0 longyang   (501) staff       (20)    11876 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/calculation.py
+-rw-r--r--   0 longyang   (501) staff       (20)     5431 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/constraint.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2037 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/controlerrors.py
+-rw-r--r--   0 longyang   (501) staff       (20)    25952 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitdataset.py
+-rw-r--r--   0 longyang   (501) staff       (20)    35890 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitstructure.py
+-rw-r--r--   0 longyang   (501) staff       (20)    27409 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitting.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9484 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/organizer.py
+-rw-r--r--   0 longyang   (501) staff       (20)     6928 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/parameter.py
+-rw-r--r--   0 longyang   (501) staff       (20)      837 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfcomponent.py
+-rw-r--r--   0 longyang   (501) staff       (20)    12373 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfdataset.py
+-rw-r--r--   0 longyang   (501) staff       (20)    18864 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfguicontrol.py
+-rw-r--r--   0 longyang   (501) staff       (20)    12929 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfguimacros.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3081 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdflist.py
+-rw-r--r--   0 longyang   (501) staff       (20)     7100 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfstructure.py
+-rw-r--r--   0 longyang   (501) staff       (20)    23156 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/plotter.py
+-rw-r--r--   0 longyang   (501) staff       (20)     8448 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/structureviewer.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.156117 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/
+-rw-r--r--   0 longyang   (501) staff       (20)   576472 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/Farrow-jpcm-2007.pdf
+-rw-r--r--   0 longyang   (501) staff       (20)   107401 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/Proffen-jac-1999.pdf
+-rw-r--r--   0 longyang   (501) staff       (20)     7680 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/TUTORIAL.txt
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.156430 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/epydoc/
+-rw-r--r--   0 longyang   (501) staff       (20)      362 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/epydoc/Makefile
+-rw-r--r--   0 longyang   (501) staff       (20)     1575 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/epydoc/epydoc.cfg
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.158603 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/
+-rw-r--r--   0 longyang   (501) staff       (20)     1101 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/Makefile
+-rw-r--r--   0 longyang   (501) staff       (20)     2707 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/acknowledgements.texinfo
+-rw-r--r--   0 longyang   (501) staff       (20)      756 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/disclaimer.texinfo
+-rw-r--r--   0 longyang   (501) staff       (20)     4018 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/extractEquations.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1274 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/fixHTMLCode.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.163552 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/
+-rw-r--r--   0 longyang   (501) staff       (20)      350 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/Makefile
+-rw-r--r--   0 longyang   (501) staff       (20)     1636 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/eq-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)     3162 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/eq-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)    60550 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)    56998 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)    57963 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-03.png
+-rw-r--r--   0 longyang   (501) staff       (20)    41156 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-04.png
+-rw-r--r--   0 longyang   (501) staff       (20)    48960 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-05.png
+-rw-r--r--   0 longyang   (501) staff       (20)    34580 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-06.png
+-rw-r--r--   0 longyang   (501) staff       (20)    43240 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-07.png
+-rw-r--r--   0 longyang   (501) staff       (20)    47440 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-08.png
+-rw-r--r--   0 longyang   (501) staff       (20)   139699 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-09.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62258 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-10.png
+-rw-r--r--   0 longyang   (501) staff       (20)    47464 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-11.png
+-rw-r--r--   0 longyang   (501) staff       (20)    59512 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)    57874 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)    39343 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-03.png
+-rw-r--r--   0 longyang   (501) staff       (20)    71799 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-04.png
+-rw-r--r--   0 longyang   (501) staff       (20)    45670 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-05.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62481 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-06.png
+-rw-r--r--   0 longyang   (501) staff       (20)    74614 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-07.png
+-rw-r--r--   0 longyang   (501) staff       (20)    60180 2023-05-04 14:22:08.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-08.png
+-rw-r--r--   0 longyang   (501) staff       (20)    71868 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-09.png
+-rw-r--r--   0 longyang   (501) staff       (20)   109109 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-10.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62258 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig4-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)    80574 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig4-02.png
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.167944 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/
+-rw-r--r--   0 longyang   (501) staff       (20)    60550 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)   256387 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-01.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)    56998 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)    57963 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-03.png
+-rw-r--r--   0 longyang   (501) staff       (20)    41156 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-04.png
+-rw-r--r--   0 longyang   (501) staff       (20)    48960 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-05.png
+-rw-r--r--   0 longyang   (501) staff       (20)    34580 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-06.png
+-rw-r--r--   0 longyang   (501) staff       (20)    43240 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-07.png
+-rw-r--r--   0 longyang   (501) staff       (20)    47440 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-08.png
+-rw-r--r--   0 longyang   (501) staff       (20)   139699 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-09.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62258 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-10.png
+-rw-r--r--   0 longyang   (501) staff       (20)    47464 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig2-11.png
+-rw-r--r--   0 longyang   (501) staff       (20)    59512 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)    57874 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)    39343 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-03.png
+-rw-r--r--   0 longyang   (501) staff       (20)    71799 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-04.png
+-rw-r--r--   0 longyang   (501) staff       (20)    45670 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-05.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62481 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-06.png
+-rw-r--r--   0 longyang   (501) staff       (20)    74614 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-07.png
+-rw-r--r--   0 longyang   (501) staff       (20)    60180 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-08.png
+-rw-r--r--   0 longyang   (501) staff       (20)    71868 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-09.png
+-rw-r--r--   0 longyang   (501) staff       (20)   109109 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig3-10.png
+-rw-r--r--   0 longyang   (501) staff       (20)    62258 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig4-01.png
+-rw-r--r--   0 longyang   (501) staff       (20)    80574 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/originals/fig4-02.png
+-rw-r--r--   0 longyang   (501) staff       (20)   175869 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/pdfgui.html
+-rw-r--r--   0 longyang   (501) staff       (20)  1473422 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/pdfgui.pdf
+-rw-r--r--   0 longyang   (501) staff       (20)    87968 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/pdfgui.texinfo
+-rw-r--r--   0 longyang   (501) staff       (20)      727 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/redistribution.texinfo
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.175160 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/
+-rw-r--r--   0 longyang   (501) staff       (20)    74438 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1050K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74438 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1100K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74438 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1150K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74440 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/300K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74446 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/550K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/650K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/700K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/720K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/730K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/740K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/750K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/800K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/880K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/980K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)   316322 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-3nm.gr
+-rw-r--r--   0 longyang   (501) staff       (20)   316398 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-bulk.gr
+-rw-r--r--   0 longyang   (501) staff       (20)  1001536 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-nano.ddp
+-rw-r--r--   0 longyang   (501) staff       (20)     1856 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-wurtzite.stru
+-rw-r--r--   0 longyang   (501) staff       (20)    74135 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni-neutron.gr
+-rw-r--r--   0 longyang   (501) staff       (20)   143812 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni-xray.gr
+-rw-r--r--   0 longyang   (501) staff       (20)     1830 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni.stru
+-rw-r--r--   0 longyang   (501) staff       (20)   130213 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/lcmo-template.ddp
+-rw-r--r--   0 longyang   (501) staff       (20)    18461 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/lmo-template.ddp
+-rwxr-xr-x   0 longyang   (501) staff       (20)     2572 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/tui_mno_bond_lengths.py
+-rw-r--r--   0 longyang   (501) staff       (20)    72233 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x000t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x004t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x012t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x016t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x020t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x024t010q35.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    72203 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x028t010q35.gr
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.195735 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/
+-rw-r--r--   0 longyang   (501) staff       (20)     1324 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/DesignNotes.txt
+-rw-r--r--   0 longyang   (501) staff       (20)      535 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/__init__.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9760 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/aboutdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9760 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/aboutdialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     7403 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/adddatapanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     7403 2023-04-23 03:10:52.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/adddatapanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     9350 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/addphasepanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9670 2023-02-25 14:21:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/addphasepanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)      918 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/blankpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     5809 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/bondangledialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     8918 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/bondlengthdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     8918 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/bondlengthdialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)    10872 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/calculationpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    11146 2023-02-25 14:21:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/calculationpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)    17694 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconfigurepanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    17694 2023-02-26 10:43:36.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconfigurepanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     6368 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconstraintpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     6368 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconstraintpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     5006 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     5006 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     4506 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetresultspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4804 2023-02-25 14:21:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetresultspanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     2637 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/debugoptions.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.208576 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/
+-rw-r--r--   0 longyang   (501) staff       (20)    16134 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/aboutdialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    16134 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/aboutdialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     3649 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/adddatapanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     3649 2023-04-23 03:11:00.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/adddatapanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     5856 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/addphasepanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     5908 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/addphasepanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    10064 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/bondlengthdialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    10064 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/bondlengthdialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    15018 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/calculationpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    15042 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/calculationpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    20477 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconfigurepanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    20525 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconfigurepanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     4837 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconstraintpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     4837 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconstraintpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     4271 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     4271 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     5524 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetresultspanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     5548 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetresultspanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    11712 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/dopingseriespanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    11712 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/dopingseriespanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     5548 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/errorreportdialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     5548 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/errorreportdialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     1871 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/fitnotebookpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     1871 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/fitnotebookpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     4341 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/insertrowsdialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     4341 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/insertrowsdialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     2849 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/journalpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     2849 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/journalpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)      995 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/outputpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)      995 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/outputpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     3437 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/parameterspanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     3437 2023-04-23 02:34:14.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/parameterspanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    22763 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconfigurepanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    22763 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconfigurepanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    22831 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconstraintspanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    22831 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconstraintspanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    22236 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseresultspanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)    22236 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseresultspanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     5596 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/plotpanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     5596 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/plotpanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     9387 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/preferencespanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     9528 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/preferencespanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     2254 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/resultspanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     2254 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/resultspanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     9073 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/rseriespanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     9073 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/rseriespanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     8441 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgconstraindialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     8441 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgconstraindialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     7550 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgstructuredialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     7550 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgstructuredialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     6665 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/supercelldialog.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     6665 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/supercelldialog.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)     9775 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/temperatureseriespanel.wxg
+-rw-r--r--   0 longyang   (501) staff       (20)     9775 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/temperatureseriespanel.wxg~
+-rw-r--r--   0 longyang   (501) staff       (20)    13799 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/dopingseriespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    13799 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/dopingseriespanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     8547 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorreportdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     8547 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorreportdialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     6436 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorreportdialog_control_fix.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4408 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorwrapper.py
+-rw-r--r--   0 longyang   (501) staff       (20)    14460 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/extendedplotframe.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3104 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/fitnotebookpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3104 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/fitnotebookpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)    35044 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/fittree.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3715 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/gui_organization.txt
+-rw-r--r--   0 longyang   (501) staff       (20)     2494 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/insertrowsdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2494 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/insertrowsdialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     4422 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/journalpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4422 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/journalpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     1284 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/main.py
+-rw-r--r--   0 longyang   (501) staff       (20)   100875 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/mainframe.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2882 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/menuitems.txt
+-rw-r--r--   0 longyang   (501) staff       (20)     2238 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/outputpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2238 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/outputpanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     2374 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/paneltest.py
+-rw-r--r--   0 longyang   (501) staff       (20)    17269 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/parameterspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    17000 2023-04-23 02:34:13.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/parameterspanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     2334 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/pdfguiglobals.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2049 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/pdfpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    31268 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconfigurepanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    31268 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconfigurepanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)    24844 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconstraintspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    24844 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconstraintspanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     3826 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phasenotebookpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    11500 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phasepanelutils.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9724 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseresultspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9724 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseresultspanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     9903 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/plotpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     7153 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/preferencespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     7532 2023-02-25 14:21:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/preferencespanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     3085 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/resultspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3085 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/resultspanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     7388 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/rseriespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     7388 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/rseriespanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     9761 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgconstraindialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9761 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgconstraindialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     9206 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgstructuredialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9206 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgstructuredialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     4081 2023-04-23 03:20:19.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/supercelldialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4081 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/supercelldialog.py~
+-rw-r--r--   0 longyang   (501) staff       (20)    13343 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/temperatureseriespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)    13343 2022-12-14 06:22:33.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/temperatureseriespanel.py~
+-rw-r--r--   0 longyang   (501) staff       (20)     8744 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/tooltips.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1652 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/welcomepanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3558 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/windowperspective.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.212113 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/
+-rw-r--r--   0 longyang   (501) staff       (20)      582 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/__init__.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1927 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/autowidthlabelsgrid.py
+-rw-r--r--   0 longyang   (501) staff       (20)     6415 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/listctrls.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2275 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/paneldialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1730 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/textctrlutils.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3994 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/validators.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2612 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/wx12.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.217908 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/
+-rw-r--r--   0 longyang   (501) staff       (20)     1079 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/C60_16x16.png
+-rw-r--r--   0 longyang   (501) staff       (20)   129798 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/C60_202x202.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)     2799 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/buckyfccicon.m
+-rw-r--r--   0 longyang   (501) staff       (20)      196 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/calculationitem.png
+-rw-r--r--   0 longyang   (501) staff       (20)     8686 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/columbia_logo.png
+-rw-r--r--   0 longyang   (501) staff       (20)     9580 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/danse_logo.png
+-rw-r--r--   0 longyang   (501) staff       (20)      210 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/datasetitem.png
+-rw-r--r--   0 longyang   (501) staff       (20)      468 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/exportplotdata.png
+-rw-r--r--   0 longyang   (501) staff       (20)     1396 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/exportplotdata.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)      228 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/fititem.png
+-rw-r--r--   0 longyang   (501) staff       (20)      540 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/fitting.png
+-rw-r--r--   0 longyang   (501) staff       (20)     1980 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/fitting.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)    28660 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/logo.png
+-rw-r--r--   0 longyang   (501) staff       (20)    37614 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/logo.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)     9646 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/msu_logo.png
+-rw-r--r--   0 longyang   (501) staff       (20)     2338 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/nsf_logo.png
+-rw-r--r--   0 longyang   (501) staff       (20)    22382 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/pdfgui.ico
+-rw-r--r--   0 longyang   (501) staff       (20)   482439 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/pdfgui_512x512.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)      689 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/phaseitem.png
+-rw-r--r--   0 longyang   (501) staff       (20)      810 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/plotting.png
+-rw-r--r--   0 longyang   (501) staff       (20)     2247 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/plotting.xcf
+-rw-r--r--   0 longyang   (501) staff       (20)      774 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/run.png
+-rw-r--r--   0 longyang   (501) staff       (20)      781 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/stop.png
+-rw-r--r--   0 longyang   (501) staff       (20)    58355 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/titlepage.png
+-rw-r--r--   0 longyang   (501) staff       (20)   139478 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/titlepage.xcf
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.225864 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/
+-rw-r--r--   0 longyang   (501) staff       (20)     2953 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/__init__.py
+-rw-r--r--   0 longyang   (501) staff       (20)      897 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/debug.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1039 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/run.py
+-rw-r--r--   0 longyang   (501) staff       (20)      858 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/rundeps.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2175 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/showphasenotebookpanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2067 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testaboutdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3868 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testcalculation.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2575 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testconstraint.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.230995 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/
+-rw-r--r--   0 longyang   (501) staff       (20)    74440 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/300K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    74446 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/550K.gr
+-rw-r--r--   0 longyang   (501) staff       (20)     1839 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/CdSe_bulk_wur.stru
+-rw-r--r--   0 longyang   (501) staff       (20)     7930 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/LaMnO3.stru
+-rw-r--r--   0 longyang   (501) staff       (20)    77077 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni.dat
+-rw-r--r--   0 longyang   (501) staff       (20)     1830 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni.stru
+-rw-r--r--   0 longyang   (501) staff       (20)   143801 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni_2-8.chi.gr
+-rw-r--r--   0 longyang   (501) staff       (20)    52256 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo.ddp
+-rw-r--r--   0 longyang   (501) staff       (20)     2033 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_00.gr
+-rw-r--r--   0 longyang   (501) staff       (20)     2033 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_20.gr
+-rw-r--r--   0 longyang   (501) staff       (20)   744064 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_full.ddp
+-rw-r--r--   0 longyang   (501) staff       (20)   102347 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/ni.ddp
+-rw-r--r--   0 longyang   (501) staff       (20)     3870 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdatasetpanels.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1866 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdopingseriespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2454 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testextendedplotframe.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9084 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testfitdataset.py
+-rw-r--r--   0 longyang   (501) staff       (20)     9290 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testfitstructure.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1387 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testinsertrowsdialog.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4143 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testloadproject.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1911 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testmainframe.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2641 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testparameter.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4336 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testparameterspanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3535 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfdataset.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1324 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfguicontrol.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4040 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfstructure.py
+-rw-r--r--   0 longyang   (501) staff       (20)     2756 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testphaseconfigurepanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3465 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/teststructureviewer.py
+-rw-r--r--   0 longyang   (501) staff       (20)     1904 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testtemperatureseriespanel.py
+-rw-r--r--   0 longyang   (501) staff       (20)     5940 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testutils.py
+-rw-r--r--   0 longyang   (501) staff       (20)     4599 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tui.py
+-rw-r--r--   0 longyang   (501) staff       (20)     3877 2023-05-04 14:22:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/utils.py
+-rw-r--r--   0 longyang   (501) staff       (20)      133 2023-05-04 14:25:09.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/version.cfg
+-rw-r--r--   0 longyang   (501) staff       (20)     1647 2022-11-26 03:28:41.000000 diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/version.py
+drwxr-xr-x   0 longyang   (501) staff       (20)        0 2023-05-04 14:25:10.150278 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/
+-rw-r--r--   0 longyang   (501) staff       (20)     6633 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/PKG-INFO
+-rw-r--r--   0 longyang   (501) staff       (20)    14509 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/SOURCES.txt
+-rw-r--r--   0 longyang   (501) staff       (20)        1 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/dependency_links.txt
+-rw-r--r--   0 longyang   (501) staff       (20)       62 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/entry_points.txt
+-rw-r--r--   0 longyang   (501) staff       (20)        1 2022-12-14 03:46:27.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/not-zip-safe
+-rw-r--r--   0 longyang   (501) staff       (20)       52 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/requires.txt
+-rw-r--r--   0 longyang   (501) staff       (20)        7 2023-05-04 14:25:10.000000 diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/top_level.txt
```

### Comparing `diffpy.pdfgui-1.4.2/AUTHORS.txt` & `diffpy.pdfgui-2.0.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/MANIFEST.in` & `diffpy.pdfgui-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/PKG-INFO` & `diffpy.pdfgui-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffpy.pdfgui
-Version: 1.4.2
+Version: 2.0.0
 Summary: GUI for PDF simulation and structure refinement.
 Home-page: https://github.com/diffpy/diffpy.pdfgui
 Author: Simon J.L. Billinge
 Author-email: sb2896@columbia.edu
 Maintainer: Pavol Juhas
 Maintainer-email: pavol.juhas@gmail.com
 License: BSD
@@ -47,41 +47,31 @@
 help menu and follow the tutorial instructions.  A detailed description
 is available in the doc/Farrow-jpcm-2007.pdf paper.
 
 
 REQUIREMENTS
 ------------------------------------------------------------------------
 
-PDFgui requires Python 3.7 or later or 2.7 and several third-party
+PDFgui requires Python 3.7, 3.8, 3.9, or 2.7 and several third-party
 libraries that are used by PDFgui and its components.
 
 * setuptools   - tools for installing Python packages
 * wxpython     - graphical user interface toolkit for Python
-* NumPy        - library for scientific computing with Python
+* numpy        - library for scientific computing with Python
 * matplotlib   - Python 2D plotting library
 * diffpy.pdffit2 - computational engine for PDFgui,
   https://github.com/diffpy/diffpy.pdffit2
 * diffpy.structure - simple storage and manipulation of atomic
   structures, https://github.com/diffpy/diffpy.structure
 * diffpy.utils - shared helper utilities for wx GUI,
   https://github.com/diffpy/diffpy.utils
 
 We recommend to use `Anaconda Python <https://www.anaconda.com/download>`_
 which allows to conveniently install PDFgui and all its software
-dependencies with a single command.  For other Python distributions
-it is necessary to install the required software separately.  As an
-example, on Ubuntu Linux some of the required software can be
-installed using ::
-
-   sudo apt-get install \
-      python-setuptools python-wxtools python-numpy \
-      python-matplotlib
-
-To install the remaining packages see the installation instructions
-at their respective web pages.
+dependencies with a single command.
 
 Please note that the Python3 PDFgui will read .ddp3 files. It is also
 possible for it to read .ddp files that were saved by the Python2 PDFgui
 but it will sometimes fail to read these. We are working on a solution
 that will be available in a future version.
 
 INSTALLATION
@@ -95,18 +85,15 @@
 PDFgui can be then started from a terminal ("Anaconda Prompt" on
 Windows) by executing the "pdfgui" program.  An alternative
 method on Windows is to start PDFgui through the DiffPy start menu.
 
 If you don't use Anaconda or prefer to install from sources, make
 sure the required software is all in place ::
 
-   pip install wxpython==4.0.7
-   conda install matplotlib
-   conda install -c conda-forge diffpy.utils
-   conda install -c conda-forge install diffpy.pdffit2
+   conda install -c conda-forge diffpy.utils diffpy.pdffit2 matplotlib wxpython
 
 Then you are ready to install diffpy.pdfgui from source codes::
 
    python setup.py install
 
 By default the files are installed to standard system directories,
 which may require the use of ``sudo`` for write privileges.  If
@@ -127,21 +114,33 @@
 (`conda install python.app`), then run as follows ::
 
    python.app diffpy.pdfgui/src/diffpy/pdfgui/application/pdfgui.py
 
 With Anaconda PDFgui can be later upgraded to the latest released
 version using ::
 
-   conda update diffpy.pdfgui
+   conda update -c conda-forge diffpy.pdfgui
 
 With other Python distributions the program can be upgraded to
 the latest version as follows ::
 
    easy_install --upgrade diffpy.pdfgui
 
+If you would like to use other Python distributions except Anaconda,
+it is necessary to install the required software separately. As an
+example, on Ubuntu Linux some of the required software can be
+installed using ::
+
+   sudo apt-get install \
+      python-setuptools python-wxtools python-numpy \
+      python-matplotlib
+
+To install the remaining packages see the installation instructions
+at their respective web pages.
+
 Other software
 ````````````````````````````````````````````````````````````````````````
 
 PDFgui can use an external structure viewer for displaying analyzed
 structures.  We have tested with several structure viewers such as
 
 * AtomEye, http://li.mit.edu/A/Graphics/A/
```

### Comparing `diffpy.pdfgui-1.4.2/README.rst` & `diffpy.pdfgui-2.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,41 +16,31 @@
 help menu and follow the tutorial instructions.  A detailed description
 is available in the doc/Farrow-jpcm-2007.pdf paper.
 
 
 REQUIREMENTS
 ------------------------------------------------------------------------
 
-PDFgui requires Python 3.7 or later or 2.7 and several third-party
+PDFgui requires Python 3.7, 3.8, 3.9, or 2.7 and several third-party
 libraries that are used by PDFgui and its components.
 
 * setuptools   - tools for installing Python packages
 * wxpython     - graphical user interface toolkit for Python
-* NumPy        - library for scientific computing with Python
+* numpy        - library for scientific computing with Python
 * matplotlib   - Python 2D plotting library
 * diffpy.pdffit2 - computational engine for PDFgui,
   https://github.com/diffpy/diffpy.pdffit2
 * diffpy.structure - simple storage and manipulation of atomic
   structures, https://github.com/diffpy/diffpy.structure
 * diffpy.utils - shared helper utilities for wx GUI,
   https://github.com/diffpy/diffpy.utils
 
 We recommend to use `Anaconda Python <https://www.anaconda.com/download>`_
 which allows to conveniently install PDFgui and all its software
-dependencies with a single command.  For other Python distributions
-it is necessary to install the required software separately.  As an
-example, on Ubuntu Linux some of the required software can be
-installed using ::
-
-   sudo apt-get install \
-      python-setuptools python-wxtools python-numpy \
-      python-matplotlib
-
-To install the remaining packages see the installation instructions
-at their respective web pages.
+dependencies with a single command.
 
 Please note that the Python3 PDFgui will read .ddp3 files. It is also
 possible for it to read .ddp files that were saved by the Python2 PDFgui
 but it will sometimes fail to read these. We are working on a solution
 that will be available in a future version.
 
 INSTALLATION
@@ -64,18 +54,15 @@
 PDFgui can be then started from a terminal ("Anaconda Prompt" on
 Windows) by executing the "pdfgui" program.  An alternative
 method on Windows is to start PDFgui through the DiffPy start menu.
 
 If you don't use Anaconda or prefer to install from sources, make
 sure the required software is all in place ::
 
-   pip install wxpython==4.0.7
-   conda install matplotlib
-   conda install -c conda-forge diffpy.utils
-   conda install -c conda-forge install diffpy.pdffit2
+   conda install -c conda-forge diffpy.utils diffpy.pdffit2 matplotlib wxpython
 
 Then you are ready to install diffpy.pdfgui from source codes::
 
    python setup.py install
 
 By default the files are installed to standard system directories,
 which may require the use of ``sudo`` for write privileges.  If
@@ -96,21 +83,33 @@
 (`conda install python.app`), then run as follows ::
 
    python.app diffpy.pdfgui/src/diffpy/pdfgui/application/pdfgui.py
 
 With Anaconda PDFgui can be later upgraded to the latest released
 version using ::
 
-   conda update diffpy.pdfgui
+   conda update -c conda-forge diffpy.pdfgui
 
 With other Python distributions the program can be upgraded to
 the latest version as follows ::
 
    easy_install --upgrade diffpy.pdfgui
 
+If you would like to use other Python distributions except Anaconda,
+it is necessary to install the required software separately. As an
+example, on Ubuntu Linux some of the required software can be
+installed using ::
+
+   sudo apt-get install \
+      python-setuptools python-wxtools python-numpy \
+      python-matplotlib
+
+To install the remaining packages see the installation instructions
+at their respective web pages.
+
 Other software
 ````````````````````````````````````````````````````````````````````````
 
 PDFgui can use an external structure viewer for displaying analyzed
 structures.  We have tested with several structure viewers such as
 
 * AtomEye, http://li.mit.edu/A/Graphics/A/
```

### Comparing `diffpy.pdfgui-1.4.2/doc/Farrow-jpcm-2007.pdf` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/Farrow-jpcm-2007.pdf`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/Proffen-jac-1999.pdf` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/Proffen-jac-1999.pdf`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/TUTORIAL.txt` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/TUTORIAL.txt`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/eq-01.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/eq-01.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/eq-02.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/eq-02.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-01.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-01.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-02.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-02.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-03.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-03.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-04.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-04.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-05.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-05.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-06.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-06.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-07.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-07.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-08.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-08.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-09.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-09.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-10.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-10.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig2-11.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig2-11.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-01.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-01.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-02.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-02.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-03.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-03.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-04.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-04.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-05.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-05.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-06.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-06.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-07.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-07.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-08.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-08.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-09.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-09.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig3-10.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig3-10.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig4-01.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig4-01.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/images/fig4-02.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/images/fig4-02.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/pdfgui.html` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/pdfgui.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
 <html>
-<!-- Copyright (C) 2008-2016, Board of Trustees of Columbia University in
-the city of New York, all rights reserved.
-
-Copyright (C) 2006, 2007, Board of Trustees of Michigan State
-University, all rights reserved.
+<!-- Up to the release 1.1.2 (February 2017) the copyright was held by
+the institutions that hosted the work as follows:
+Copyright 2006-2007, Board of Trustees of Michigan State University,
+Copyright 2008-2012, Board of Trustees of Columbia University in the
+city of New York.
+Copyright 2013, Brookhaven National Laboratory (Copyright holder
+indicated in each source file).
  -->
-<!-- Created on March 4, 2016 by texi2html 5.0
+<!-- Created on April 25, 2023 by texi2html 5.0
 texi2html was written by: 
             Lionel Cons <Lionel.Cons@cern.ch> (original author)
             Karl Berry  <karl@freefriends.org>
             Olaf Bachmann <obachman@mathematik.uni-kl.de>
             and many others.
 Maintained by: Many creative people.
 Send bugs and suggestions to <texi2html-bug@nongnu.org>
 -->
 <head>
-<title>PDFgui user guide, release 1.0, March 2016</title>
+<title>PDFgui user guide, release 2.0, May 2023</title>
 
-<meta name="description" content="PDFgui user guide, release 1.0, March 2016">
-<meta name="keywords" content="PDFgui user guide, release 1.0, March 2016">
+<meta name="description" content="PDFgui user guide, release 2.0, May 2023">
+<meta name="keywords" content="PDFgui user guide, release 2.0, May 2023">
 <meta name="resource-type" content="document">
 <meta name="distribution" content="global">
 <meta name="Generator" content="texi2html 5.0">
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 <style type="text/css">
 <!--
 a.summary-letter {text-decoration: none}
@@ -53,16 +55,16 @@
 
 </head>
 
 <body lang="en" bgcolor="#FFFFFF" text="#000000" link="#0000FF" vlink="#800080" alink="#FF0000">
 
 
 <h1>PDFgui user guide</h1>
-<h3 align="right">1.1 release</h3>
-<h3 align="right">March 2016</h3>
+<h3 align="right">2.0 release</h3>
+<h3 align="right">May 2023</h3>
 <strong>C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin,</strong><br>
 <strong>J. Bloch, Th. Proffen, and S. J. L. Billinge</strong><br>
 
 
 
 <hr>
 <a name="acknowledgments"></a>
@@ -73,40 +75,62 @@
 <td valign="middle" align="left">[<a href="#SEC_Contents" title="Table of contents">Contents</a>]</td>
 <td valign="middle" align="left">[<a href="#Index" title="Index">Index</a>]</td>
 <td valign="middle" align="left">[<a href="#SEC_About" title="About (help)"> ? </a>]</td>
 </tr></table>
 <a name="Acknowledgments"></a>
 <h2 class="heading">Acknowledgments</h2>
 <a name="index-acknowledgments"></a>
-<p>PDFgui was developed as part of the Distributed Analysis of Neutron Scattering
-Data (DANSE) project which is funded by NSF under DMR-0520547.  The PDFfit2
-development was funded by NSF under contract DMR-0304391.  The program is part
-of the DiffPy and DANSE open-source projects at Columbia University and is
-available subject to the conditions and terms laid out below. Several of the
-examples in the tutorial part were made possible and benefited from samples
+<p>This software was originally developed by the Billinge group as part
+of the Distributed Data Analysis of Neutron Scattering Experiments
+(DANSE) project funded by the US National Science Foundation under
+grant DMR-0520547. Developments of PDFfit2 were funded by NSF grant
+DMR-0304391 in the Billinge group, and with support from Michigan State
+University and Columbia University. Any opinions, findings, and conclusions
+or recommendations expressed in this material are those of the author(s)
+and do not necessarily reflect the views of the respective funding bodies.
+Subsequent development was done in the Billinge group at Columbia University
+and then in collaboration between the Billinge group at Columbia and Pavol
+Juhas at Brookhaven National Laboratory. Moving forward, PDFgui will be
+maintained as a community project with contributions welcomed from many people.
+</p>
+<p>Several of the examples in the tutorial part were made possible and benefited from samples
 synthesized by J. F.  Mitchell, and from data collected and processed by M.
 Schmidt, P. G. Radaelli, and X. Qiu.
-If you use this program to do productive scientific research that leads
+</p>
+<p>If you use this program to do productive scientific research that leads
 to publication, we ask that you acknowledge use of the program by citing
 the following paper in your publication:
 </p>
 <blockquote>
 <p>C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin,
 J. Bloch, Th. Proffen and S. J. L. Billinge,
-<a href="http://stacks.iop.org/0953-8984/19/335219">PDFfit2 and PDFgui: computer programs for studying nanostructure in crystals</a>,
+<a href="https://stacks.iop.org/0953-8984/19/335219">PDFfit2 and PDFgui: computer programs for studying nanostructure in crystals</a>,
 <i>J.&nbsp;Phys.: Condens. Matter</i>, <b>19</b>, 335219 (2007)
 </p></blockquote>
 
-<p>Copyright &copy; 2008-2016, Board of Trustees of Columbia University in
-the city of New York, all rights reserved.
-</p>
-<p>Copyright &copy; 2006, 2007, Board of Trustees of Michigan State
-University, all rights reserved.
+<p>Up to the release 1.1.2 (February 2017) the copyright was held by
+the institutions that hosted the work as follows:
+Copyright 2006-2007, Board of Trustees of Michigan State University,
+Copyright 2008-2012, Board of Trustees of Columbia University in the
+city of New York.
+Copyright 2013, Brookhaven National Laboratory (Copyright holder
+indicated in each source file).
 </p><a name="index-copyright"></a>
-<p>For more information please visit <a href="http://www.diffpy.org">http://www.diffpy.org</a>
+<p>As of February 2017, and the 1.1.2 release, PDFgui has moved to a shared copyright model.
+PDFgui uses a shared copyright model. Each contributor maintains copyright over their
+contributions to PDFgui. But, it is important to note that these contributions are
+typically only changes to the repositories. Thus, the PDFgui source code, in its entirety,
+is not the copyright of any single person or institution. Instead, it is the collective
+copyright of the entire PDFgui Development Team. If individual contributors want to
+maintain a record of what changes/contributions they have specific copyright on, they
+should indicate their copyright in the commit message of the change, when they commit
+the change to one of the PDFgui repositories.
+The PDFgui Development Team is the set of all contributors to the PDFgui project.
+A full list can be obtained from the git version control logs.
+For more information please visit <a href="https://www.diffpy.org">https://www.diffpy.org</a>
 or contact Prof. Simon Billinge at <a href="mailto:sb2896@columbia.edu">sb2896@columbia.edu</a>.
 </p>
 
 
 <a name="Preface"></a>
 <h1 class="majorheading">Preface</h1>
 <a name="Using-PDFgui-and-PDFfit2"></a>
@@ -269,15 +293,15 @@
 possibility of errors. In addition, new fitting parameters for handling
 dynamic atomic correlations and experimental resolution have been introduced
 as well.
 </p>
 <p>Instead of rewriting the PDFfit command interpreter, which is used
 to define the fitting problem and to control and run the refinement,
 its functions are carried out using the Python language
-(<a href="http://www.python.org">http://www.python.org</a>). Python is a powerful, cross-platform,
+(<a href="https://www.python.org">https://www.python.org</a>). Python is a powerful, cross-platform,
 open-source interpreted programming language (i.e., it does not need
 to be compiled to run, similar to scripting) that emphasizes
 object-oriented and modular design. PDFfit2 scripts written in
 Python syntax take the place of PDFfit macros and the Python
 interpreter can handle everything that the old interpreter could,
 and more. Using Python as an interpreter allows PDFfit2 to be
 combined with and enhanced by other Python libraries.  We make use
@@ -339,15 +363,15 @@
 <p>PDFgui is written in the Python programming language. Python features a relaxed
 and friendly syntax, supports &ldquo;write once, run anywhere&rdquo; portability, and has
 extensive libraries and modules for virtually every task. Software codes
 written in a variety of programming languages can be bound into Python, which
 allows them to be used together. Python is becoming a popular choice in the
 scientific computation community.
 </p>
-<p>PDFgui&rsquo;s interface is built using wxPython (<a href="http://www.wxPython.org">http://www.wxPython.org</a>), the
+<p>PDFgui&rsquo;s interface is built using wxPython (<a href="https://www.wxpython.org">https://www.wxpython.org</a>), the
 Python package for wxWidgets, a mature cross-platform GUI library.  Graphical
 applications written in wxPython provide a look and feel native to the platform
 on which they are run.  PDFgui is designed to run on Windows, Mac OS, Linux,
 and all major Unix systems.
 </p>
 <hr>
 <a name="Capabilities"></a>
@@ -387,28 +411,28 @@
 temperature factors to keep the structure consistent with the symmetry
 requirements. This can be done either for all atoms in the structure or for an
 arbitrary subset - for example when it is known that only a certain species
 show a local distortion. The code for space group definitions was provided by
 the Python Macromolecular Library (mmLib,
 <a href="http://pymmlib.sourceforge.net">http://pymmlib.sourceforge.net</a>).  This was extened to include
 non-standard space groups using the Computational Crystallography Toolbox
-(cctbx, <a href="http://cctbx.sourceforge.net">http://cctbx.sourceforge.net</a>).  PDFgui also supports supercell
+(cctbx, <a href="https://cctbx.github.io">https://cctbx.github.io</a>).  PDFgui also supports supercell
 expansion of a normal unit cell.
 </p>
-<p>PDFgui uses the matplotlib (<a href="http://matplotlib.org">http://matplotlib.org</a>) Python
+<p>PDFgui uses the matplotlib (<a href="https://matplotlib.org">https://matplotlib.org</a>) Python
 package for 2D plotting of data and results. Matplotlib has a friendly
 interface so the user can quickly and easily view the results of a fitting.
 PDFgui lets users plot data from a series of fits and plot it against selected
 meta-data (temperature, doping, etc.), plot the results of several fits in the
 same window, plot the PDF in real time as the fitting is running, plot the
 parameters or variables in real time as the refinement evolves, and save plots
 in common image formats or export the data to a text file.  PDFgui can be
 configured to use one of many structure visualization packages, such as AtomEye
 (<a href="http://li.mit.edu/A/Graphics/A/">http://li.mit.edu/A/Graphics/A/</a>) or PyMOL
-(<a href="http://www.pymol.org">http://www.pymol.org</a>).
+(<a href="https://www.pymol.org">https://www.pymol.org</a>).
 </p>
 <p>PDFgui supports built-in macros for advanced fits. For a set of experimental
 data from one system at different temperatures or doping levels, PDFgui can
 expand a template fit to a series of related fits.  Another PDFgui macro makes
 it easy to set up boxcar fits, where the same model is fit over different
 r-ranges of the PDF data.
 </p>
@@ -433,15 +457,15 @@
 <h2 class="section">1.3 Availability</h2>
 <a name="index-availability"></a>
 
 <p>PDFfit2 and PDFgui are open source and distributed under a BSD license.  They
 run on Windows, Mac OS, Linux, and all major Unix systems. The source code is
 freely available. For more information please contact Professor Simon Billinge
 (<a href="mailto:sb2896@columbia.edu">sb2896@columbia.edu</a>) or consult the web-page
-<a href="http://www.diffpy.org">http://www.diffpy.org</a>. News of updates and releases will be posted at
+<a href="https://www.diffpy.org">https://www.diffpy.org</a>. News of updates and releases will be posted at
 this website and on the diffpy-users group at
 <a href="https://groups.google.com/d/forum/diffpy-users">https://groups.google.com/d/forum/diffpy-users</a>.
 </p>
 <hr>
 <a name="Installation"></a>
 <table class="header" cellpadding="1" cellspacing="1" border="0">
 <tr><td valign="middle" align="left">[<a href="#Introduction" title="Beginning of this chapter or previous chapter"> &lt;&lt; </a>]</td>
@@ -461,15 +485,15 @@
 <a name="Installation-1"></a>
 <h2 class="section">1.4 Installation</h2>
 <a name="index-installation"></a>
 
 <p>PDFgui is included as a part of DiffPy, a suite of Python and C++
 libraries for structure analysis from diffraction data.  For more
 information about DiffPy products visit the project homepage at
-<a href="http://www.diffpy.org">http://www.diffpy.org</a>.
+<a href="https://www.diffpy.org">https://www.diffpy.org</a>.
 </p>
 <table class="menu" border="0" cellspacing="0">
 <tr><td align="left" valign="top"><a href="#Installation-for-Anaconda-Python">1.4.1 Installation for Anaconda Python</a></td><td>&nbsp;&nbsp;</td><td align="left" valign="top">
 </td></tr>
 <tr><td align="left" valign="top"><a href="#Configuration-of-structure-viewer">1.4.2 Configuration of structure viewer</a></td><td>&nbsp;&nbsp;</td><td align="left" valign="top">
 </td></tr>
 <tr><td align="left" valign="top"><a href="#Installation-from-sources">1.4.3 Installation from sources</a></td><td>&nbsp;&nbsp;</td><td align="left" valign="top">
@@ -561,15 +585,15 @@
 <dt><em>AtomEye</em></dt>
 <dd><p>AtomEye structure viewer, XCFG format <br>
 <a href="http://li.mit.edu/A/Graphics/A/">http://li.mit.edu/A/Graphics/A/</a>
 </p>
 </dd>
 <dt><em>PyMOL</em></dt>
 <dd><p>PyMOL structure viewer, PDB format <br>
-<a href="http://www.pymol.org">http://www.pymol.org</a>
+<a href="https://www.pymol.org">https://www.pymol.org</a>
 </p></dd>
 </dl>
 
 <p><b>A note for AtomEye users:</b>
 <a name="index-AtomEye-viewer"></a>
 </p>
 <p>AtomEye requires its standard output is connected to a terminal.
@@ -830,15 +854,15 @@
 that accepts structure file as a command-line argument.
 </p>
 </dd>
 <dt><em>space group representations</em></dt>
 <dd><p>Added 249 space group
 representations in non-standard settings.  The new representations
 were generated using the
-<a href="http://cctbx.sourceforge.net">cctbx library</a> and helpful
+<a href="https://cctbx.github.io">cctbx library</a> and helpful
 hints from Ralf W. Grosse-Kunstleve.
 </p>
 </dd>
 <dt><em>symmetry constraints</em></dt>
 <dd><p>Fixed issues with generation of
 symmetry requirements for the ADP tensors.
 </p>
@@ -2018,15 +2042,15 @@
 nanoparticle data reveals nanoparticle diameter of approximately 30 Angstroms,
 as further illustrated in <a href="#fig3_002d10">Figure 3.10</a>. Enlarged values of isotropic ADPs are
 again observed, and the fit is reasonably good. Further improvements can be
 obtained by introducing anisotropic ADPs, where again values related to the
 z-direction will remain abnormally large most probably due to the stacking
 related disorder.  A detailed description of this system and successful
 PDF modeling can be found in this publication:
-<a href="http://link.aps.org/doi/10.1103/PhysRevB.76.115413">Quantitative size-dependent structure and strain determination of CdSe nanoparticles using atomic pair distribution function analysis</a>.
+<a href="https://link.aps.org/doi/10.1103/PhysRevB.76.115413">Quantitative size-dependent structure and strain determination of CdSe nanoparticles using atomic pair distribution function analysis</a>.
 </p>
 <div class="float"><a name="fig3_002d10"></a>
 <img src="images/fig3-10.png" alt="images/fig3-10">
 
 </div><p><strong>Figure 3.10: Fitting the structure of a nanoparticle: 3nm CdSe
 nanoparticle example.
 </strong>
@@ -2195,15 +2219,15 @@
 engine, such as calculation of differential PDFs, handling atoms with special
 scattering properties, etc. Advanced usage of PDFfit2 engine to resolve any
 such special modeling need that user may have is available through usage of
 Python scripts in the expert command line mode, similar to that featured in the
 PDFFIT program.  Handling these situations requires detailed knowledge of the
 PDFfit2 syntax based on Python, which is beyond the scope of this user guide
 and will be described elsewhere. Refer to the PDFfit2 API
-(<a href="http://www.diffpy.org/doc/pdffit2/">http://www.diffpy.org/doc/pdffit2/</a> and the diffpy-users
+(<a href="https://www.diffpy.org/doc/pdffit2">https://www.diffpy.org/doc/pdffit2</a> and the diffpy-users
 group (<a href="https://groups.google.com/d/forum/diffpy-users">https://groups.google.com/d/forum/diffpy-users</a>) for help with PDFfit2
 scripting.
 </p>
 <hr>
 <a name="PDFgui-reference-sheets"></a>
 <table class="header" cellpadding="1" cellspacing="1" border="0">
 <tr><td valign="middle" align="left">[<a href="#Extras" title="Beginning of this chapter or previous chapter"> &lt;&lt; </a>]</td>
@@ -2895,15 +2919,15 @@
 <td valign="middle" align="left">[<a href="#SEC_Contents" title="Table of contents">Contents</a>]</td>
 <td valign="middle" align="left">[<a href="#Index" title="Index">Index</a>]</td>
 <td valign="middle" align="left">[<a href="#SEC_About" title="About (help)"> ? </a>]</td>
 </tr></table>
 <h1>About This Document</h1>
 
 <p>
-  This document was generated on <i>March 4, 2016</i> using <a href="http://www.nongnu.org/texi2html/"><i>texi2html 5.0</i></a>.
+  This document was generated on <i>April 25, 2023</i> using <a href="http://www.nongnu.org/texi2html/"><i>texi2html 5.0</i></a>.
 </p>
 <p>
   The buttons in the navigation panels have the following meaning:
 </p>
 <table border="1">
   <tr>
     <th> Button </th>
@@ -2997,14 +3021,14 @@
     </ul>
   </li>
 </ul>
 
 <hr>
 <p>
  <font size="-1">
-  This document was generated on <i>March 4, 2016</i> using <a href="http://www.nongnu.org/texi2html/"><i>texi2html 5.0</i></a>.
+  This document was generated on <i>April 25, 2023</i> using <a href="http://www.nongnu.org/texi2html/"><i>texi2html 5.0</i></a>.
  </font>
  <br>
 
 </p>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,41 +1,61 @@
 
 
 
 
 
 
 ****** PDFgui user guide ******
-                                                          **** 1.1 release ****
-                                                           **** March 2016 ****
+                                                          **** 2.0 release ****
+                                                             **** May 2023 ****
 C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin,
 J. Bloch, Th. Proffen, and S. J. L. Billinge
 ===============================================================================
 [ < ] [>]  [Contents] [Index] [?]
 ***** Acknowledgments *****
-PDFgui was developed as part of the Distributed Analysis of Neutron Scattering
-Data (DANSE) project which is funded by NSF under DMR-0520547. The PDFfit2
-development was funded by NSF under contract DMR-0304391. The program is part
-of the DiffPy and DANSE open-source projects at Columbia University and is
-available subject to the conditions and terms laid out below. Several of the
-examples in the tutorial part were made possible and benefited from samples
-synthesized by J. F. Mitchell, and from data collected and processed by M.
-Schmidt, P. G. Radaelli, and X. Qiu. If you use this program to do productive
-scientific research that leads to publication, we ask that you acknowledge use
-of the program by citing the following paper in your publication:
+This software was originally developed by the Billinge group as part of the
+Distributed Data Analysis of Neutron Scattering Experiments (DANSE) project
+funded by the US National Science Foundation under grant DMR-0520547.
+Developments of PDFfit2 were funded by NSF grant DMR-0304391 in the Billinge
+group, and with support from Michigan State University and Columbia University.
+Any opinions, findings, and conclusions or recommendations expressed in this
+material are those of the author(s) and do not necessarily reflect the views of
+the respective funding bodies. Subsequent development was done in the Billinge
+group at Columbia University and then in collaboration between the Billinge
+group at Columbia and Pavol Juhas at Brookhaven National Laboratory. Moving
+forward, PDFgui will be maintained as a community project with contributions
+welcomed from many people.
+Several of the examples in the tutorial part were made possible and benefited
+from samples synthesized by J. F. Mitchell, and from data collected and
+processed by M. Schmidt, P. G. Radaelli, and X. Qiu.
+If you use this program to do productive scientific research that leads to
+publication, we ask that you acknowledge use of the program by citing the
+following paper in your publication:
      C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin, J. Bloch,
      Th. Proffen and S. J. L. Billinge, PDFfit2_and_PDFgui:_computer
      programs_for_studying_nanostructure_in_crystals, J. Phys.: Condens.
      Matter, 19, 335219 (2007)
-Copyright © 2008-2016, Board of Trustees of Columbia University in the city of
-New York, all rights reserved.
-Copyright © 2006, 2007, Board of Trustees of Michigan State University, all
-rights reserved.
-For more information please visit http://www.diffpy.org or contact Prof. Simon
-Billinge at sb2896@columbia.edu.
+Up to the release 1.1.2 (February 2017) the copyright was held by the
+institutions that hosted the work as follows: Copyright 2006-2007, Board of
+Trustees of Michigan State University, Copyright 2008-2012, Board of Trustees
+of Columbia University in the city of New York. Copyright 2013, Brookhaven
+National Laboratory (Copyright holder indicated in each source file).
+As of February 2017, and the 1.1.2 release, PDFgui has moved to a shared
+copyright model. PDFgui uses a shared copyright model. Each contributor
+maintains copyright over their contributions to PDFgui. But, it is important to
+note that these contributions are typically only changes to the repositories.
+Thus, the PDFgui source code, in its entirety, is not the copyright of any
+single person or institution. Instead, it is the collective copyright of the
+entire PDFgui Development Team. If individual contributors want to maintain a
+record of what changes/contributions they have specific copyright on, they
+should indicate their copyright in the commit message of the change, when they
+commit the change to one of the PDFgui repositories. The PDFgui Development
+Team is the set of all contributors to the PDFgui project. A full list can be
+obtained from the git version control logs. For more information please visit
+https://www.diffpy.org or contact Prof. Simon Billinge at sb2896@columbia.edu.
 ****** Preface ******
 ***** Using PDFgui and PDFfit2 *****
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer.
 Redistributions in binary form must reproduce the above copyright notice, this
@@ -112,15 +132,15 @@
 constraint system has also been upgraded. The program automatically computes
 the analytical derivatives of the constraints that are required by the
 minimization routine. This simplifies user input and reduces the possibility of
 errors. In addition, new fitting parameters for handling dynamic atomic
 correlations and experimental resolution have been introduced as well.
 Instead of rewriting the PDFfit command interpreter, which is used to define
 the fitting problem and to control and run the refinement, its functions are
-carried out using the Python language (http://www.python.org). Python is a
+carried out using the Python language (https://www.python.org). Python is a
 powerful, cross-platform, open-source interpreted programming language (i.e.,
 it does not need to be compiled to run, similar to scripting) that emphasizes
 object-oriented and modular design. PDFfit2 scripts written in Python syntax
 take the place of PDFfit macros and the Python interpreter can handle
 everything that the old interpreter could, and more. Using Python as an
 interpreter allows PDFfit2 to be combined with and enhanced by other Python
 libraries. We make use of this capability with PDFgui as described below.
@@ -142,15 +162,15 @@
 interface.
 PDFgui is written in the Python programming language. Python features a relaxed
 and friendly syntax, supports “write once, run anywhere” portability, and has
 extensive libraries and modules for virtually every task. Software codes
 written in a variety of programming languages can be bound into Python, which
 allows them to be used together. Python is becoming a popular choice in the
 scientific computation community.
-PDFgui’s interface is built using wxPython (http://www.wxPython.org), the
+PDFgui’s interface is built using wxPython (https://www.wxpython.org), the
 Python package for wxWidgets, a mature cross-platform GUI library. Graphical
 applications written in wxPython provide a look and feel native to the platform
 on which they are run. PDFgui is designed to run on Windows, Mac OS, Linux, and
 all major Unix systems.
 ===============================================================================
 [<<] [<] [Up] [>] [>>]     [Top] [Contents] [Index] [?]
 **** 1.2.2 Capabilities ****
@@ -171,46 +191,46 @@
 equivalent sites and generate constraint equations for their coordinates and
 temperature factors to keep the structure consistent with the symmetry
 requirements. This can be done either for all atoms in the structure or for an
 arbitrary subset - for example when it is known that only a certain species
 show a local distortion. The code for space group definitions was provided by
 the Python Macromolecular Library (mmLib, http://pymmlib.sourceforge.net). This
 was extened to include non-standard space groups using the Computational
-Crystallography Toolbox (cctbx, http://cctbx.sourceforge.net). PDFgui also
-supports supercell expansion of a normal unit cell.
-PDFgui uses the matplotlib (http://matplotlib.org) Python package for 2D
+Crystallography Toolbox (cctbx, https://cctbx.github.io). PDFgui also supports
+supercell expansion of a normal unit cell.
+PDFgui uses the matplotlib (https://matplotlib.org) Python package for 2D
 plotting of data and results. Matplotlib has a friendly interface so the user
 can quickly and easily view the results of a fitting. PDFgui lets users plot
 data from a series of fits and plot it against selected meta-data (temperature,
 doping, etc.), plot the results of several fits in the same window, plot the
 PDF in real time as the fitting is running, plot the parameters or variables in
 real time as the refinement evolves, and save plots in common image formats or
 export the data to a text file. PDFgui can be configured to use one of many
 structure visualization packages, such as AtomEye (http://li.mit.edu/A/
-Graphics/A/) or PyMOL (http://www.pymol.org).
+Graphics/A/) or PyMOL (https://www.pymol.org).
 PDFgui supports built-in macros for advanced fits. For a set of experimental
 data from one system at different temperatures or doping levels, PDFgui can
 expand a template fit to a series of related fits. Another PDFgui macro makes
 it easy to set up boxcar fits, where the same model is fit over different r-
 ranges of the PDF data.
 ===============================================================================
 [<<] [<] [Up] [>] [>>]     [Top] [Contents] [Index] [?]
 ***** 1.3 Availability *****
 PDFfit2 and PDFgui are open source and distributed under a BSD license. They
 run on Windows, Mac OS, Linux, and all major Unix systems. The source code is
 freely available. For more information please contact Professor Simon Billinge
-(sb2896@columbia.edu) or consult the web-page http://www.diffpy.org. News of
+(sb2896@columbia.edu) or consult the web-page https://www.diffpy.org. News of
 updates and releases will be posted at this website and on the diffpy-users
 group at https://groups.google.com/d/forum/diffpy-users.
 ===============================================================================
 [<<] [<] [Up] [>] [>>]     [Top] [Contents] [Index] [?]
 ***** 1.4 Installation *****
 PDFgui is included as a part of DiffPy, a suite of Python and C++ libraries for
 structure analysis from diffraction data. For more information about DiffPy
-products visit the project homepage at http://www.diffpy.org.
+products visit the project homepage at https://www.diffpy.org.
 1.4.1_Installation_for_Anaconda_Python    
 1.4.2_Configuration_of_structure_viewer   
 1.4.3_Installation_from_sources           
 ===============================================================================
 [<<] [<] [Up] [>] [>>]     [Top] [Contents] [Index] [?]
 **** 1.4.1 Installation for Anaconda Python ****
 As of version 1.1 PDFgui is distributed as a pre-built package for Anaconda
@@ -240,15 +260,15 @@
 with a suitable structure format in the “Edit → Preferences” menu in PDFgui.
 The structure plotting feature has been tested with the following programs:
   AtomEye
       AtomEye structure viewer, XCFG format
       http://li.mit.edu/A/Graphics/A/
   PyMOL
       PyMOL structure viewer, PDB format
-      http://www.pymol.org
+      https://www.pymol.org
 A note for AtomEye users:
 AtomEye requires its standard output is connected to a terminal. On Unix this
 happens when pdfgui is started from a terminal. However if you prefer to start
 PDFgui using a desktop shortcut or via “Run Application” dialog of the window
 manager, you need to put the following information to the “Edit → Preferences”
 menu of PDFgui.
 Structure viewer executable: xterm
@@ -1179,16 +1199,16 @@
 it does not encapsulate all the capabilities available within the modeling
 engine, such as calculation of differential PDFs, handling atoms with special
 scattering properties, etc. Advanced usage of PDFfit2 engine to resolve any
 such special modeling need that user may have is available through usage of
 Python scripts in the expert command line mode, similar to that featured in the
 PDFFIT program. Handling these situations requires detailed knowledge of the
 PDFfit2 syntax based on Python, which is beyond the scope of this user guide
-and will be described elsewhere. Refer to the PDFfit2 API (http://
-www.diffpy.org/doc/pdffit2/ and the diffpy-users group (https://
+and will be described elsewhere. Refer to the PDFfit2 API (https://
+www.diffpy.org/doc/pdffit2 and the diffpy-users group (https://
 groups.google.com/d/forum/diffpy-users) for help with PDFfit2 scripting.
 ===============================================================================
 [<<] [<] [Up] [>] [>>]     [Top] [Contents] [Index] [?]
 ****** 5 PDFgui reference sheets ******
 
 5.1_PDFgui_shortcut_keys        
 5.2_Command_line_arguments      
@@ -1521,15 +1541,15 @@
           o 5.2_Command_line_arguments
           o 5.3_List_of_PDFfit2_variables
           o 5.4_PDF_peak_width
     * Index
 ===============================================================================
 [Top] [Contents] [Index] [?]
 ****** About This Document ******
-This document was generated on March 4, 2016 using texi2html_5.0.
+This document was generated on April 25, 2023 using texi2html_5.0.
 The buttons in the navigation panels have the following meaning:
  _____________________________________________________________________________
 |Button____|Name_______|Go_to________________________________|From_1.2.3_go_to|
 |   [ << ] |  FastBack |Beginning of this chapter or previous|1               |
 |__________|___________|chapter______________________________|________________|
 |___[_<_]__|_____Back__|Previous_section_in_reading_order____|1.2.2___________|
 |___[_Up_]_|______Up___|Up_section___________________________|1.2_____________|
@@ -1549,8 +1569,8 @@
                 # 1.2.2 Subsubsection One-Two-Two
                 # 1.2.3 Subsubsection One-Two-Three     <== Current Position
                 # 1.2.4 Subsubsection One-Two-Four
           o 1.3 Subsection One-Three
                 # ...
           o 1.4 Subsection One-Four
 ===============================================================================
-This document was generated on March 4, 2016 using texi2html_5.0.
+This document was generated on April 25, 2023 using texi2html_5.0.
```

### Comparing `diffpy.pdfgui-1.4.2/doc/manual/pdfgui.pdf` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/manual/pdfgui.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,32 +1,49 @@
 PDFgui user guide
-1.1 release
-March 2016
+2.0 release
+May 2023
 
 C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin,
 J. Bloch, Th. Proffen, and S. J. L. Billinge
 
 Acknowledgments
-PDFgui was developed as part of the Distributed Analysis of Neutron Scattering Data
-(DANSE) project which is funded by NSF under DMR-0520547. The PDFfit2 development
-was funded by NSF under contract DMR-0304391. The program is part of the DiffPy
-and DANSE open-source projects at Columbia University and is available subject to the
-conditions and terms laid out below. Several of the examples in the tutorial part were made
-possible and benefited from samples synthesized by J. F. Mitchell, and from data collected
-and processed by M. Schmidt, P. G. Radaelli, and X. Qiu.
+This software was originally developed by the Billinge group as part of the Distributed Data
+Analysis of Neutron Scattering Experiments (DANSE) project funded by the US National
+Science Foundation under grant DMR-0520547. Developments of PDFfit2 were funded by
+NSF grant DMR-0304391 in the Billinge group, and with support from Michigan State
+University and Columbia University. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily
+reflect the views of the respective funding bodies. Subsequent development was done in
+the Billinge group at Columbia University and then in collaboration between the Billinge
+group at Columbia and Pavol Juhas at Brookhaven National Laboratory. Moving forward,
+PDFgui will be maintained as a community project with contributions welcomed from many
+people.
+Several of the examples in the tutorial part were made possible and benefited from samples
+synthesized by J. F. Mitchell, and from data collected and processed by M. Schmidt, P. G.
+Radaelli, and X. Qiu.
 If you use this program to do productive scientific research that leads to publication, we ask
 that you acknowledge use of the program by citing the following paper in your publication:
-C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin, J. Bloch, Th. Proffen and S. J. L. Billinge, PDFfit2 and PDFgui: computer programs for studying
-nanostructure in crystals (http: / / stacks . iop . org / 0953-8984 / 19 / 335219),
+C. L. Farrow, P. Juhás, J. W. Liu, D. Bryndin, E. S. Božin, J. Bloch, Th. Proffen and S. J. L. Billinge, PDFfit2 and PDFgui: computer programs for studying nanostructure in crystals (https://stacks.iop.org/0953-8984/19/335219),
 J. Phys.: Condens. Matter, 19, 335219 (2007)
-Copyright c 2008-2016, Board of Trustees of Columbia University in the city of New York,
-all rights reserved.
-Copyright c 2006, 2007, Board of Trustees of Michigan State University, all rights reserved.
-
-For more information please visit http://www.diffpy.org or contact Prof. Simon Billinge
+Up to the release 1.1.2 (February 2017) the copyright was held by the institutions that
+hosted the work as follows: Copyright 2006-2007, Board of Trustees of Michigan State
+University, Copyright 2008-2012, Board of Trustees of Columbia University in the city of
+New York. Copyright 2013, Brookhaven National Laboratory (Copyright holder indicated
+in each source file).
+As of February 2017, and the 1.1.2 release, PDFgui has moved to a shared copyright model.
+PDFgui uses a shared copyright model. Each contributor maintains copyright over their
+contributions to PDFgui. But, it is important to note that these contributions are typically
+only changes to the repositories. Thus, the PDFgui source code, in its entirety, is not the
+copyright of any single person or institution. Instead, it is the collective copyright of the
+entire PDFgui Development Team. If individual contributors want to maintain a record
+of what changes/contributions they have specific copyright on, they should indicate their
+copyright in the commit message of the change, when they commit the change to one of the
+PDFgui repositories.
+The PDFgui Development Team is the set of all contributors to the PDFgui project. A full
+list can be obtained from the git version control logs.
+For more information please visit https://www.diffpy.org or contact Prof. Simon Billinge
 at sb2896@columbia.edu.
 
 Preface
 Using PDFgui and PDFfit2
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 Redistributions of source code must retain the above copyright notice, this list of conditions
 and the following disclaimer.
@@ -49,78 +66,59 @@
 
 i
 
 Table of Contents
 1
 
 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
-1.1
-1.2
-
-PDFfit2 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
-PDFgui . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
+1.1 PDFfit2 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
+1.2 PDFgui . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
 1.2.1 Design principles . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
 1.2.2 Capabilities . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
 1.3 Availability . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
 1.4 Installation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
 1.4.1 Installation for Anaconda Python . . . . . . . . . . . . . . . . . . . . . . . . . . 3
 1.4.2 Configuration of structure viewer. . . . . . . . . . . . . . . . . . . . . . . . . . . 4
 1.4.3 Installation from sources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
 1.5 What is new . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5
 1.6 Community. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
 
 2
 
 Quick start . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
-2.1
-2.2
+2.1 PDFgui layout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
+2.2 Creating a simple fit using a preexisting structure file . . . . . . . . . . . 9
 
 3
 
-PDFgui layout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
-Creating a simple fit using a preexisting structure file . . . . . . . . . . . 9
-
 Examples and tutorials . . . . . . . . . . . . . . . . . . . . . . . . 21
-3.1
-3.2
-3.3
-
-Building structure model using crystal symmetry. . . . . . . . . . . . . . . 21
-Calculating PDF from a structure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23
-Sequential fitting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24
+3.1 Building structure model using crystal symmetry. . . . . . . . . . . . . . . 21
+3.2 Calculating PDF from a structure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 23
+3.3 Sequential fitting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24
 3.3.1 Multistage fitting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 25
 3.3.2 Sequential fitting of incremental r-series . . . . . . . . . . . . . . . . . . . 26
 3.3.3 Sequential fitting of temperature series . . . . . . . . . . . . . . . . . . . . 27
 3.3.4 Sequential fitting of doping series . . . . . . . . . . . . . . . . . . . . . . . . . 29
 3.3.5 Advanced post-processing of sequential refinement. . . . . . . . . 32
 3.4 Nanoparticle structure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 33
 
 4
 
 Extras . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
-4.1
-4.2
-4.3
+4.1 PDF plotting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
+4.2 Displaying the structure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 37
+4.3 Advanced usage and special needs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 38
 
 5
 
-PDF plotting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
-Displaying the structure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 37
-Advanced usage and special needs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 38
-
 PDFgui reference sheets . . . . . . . . . . . . . . . . . . . . . . . 39
-5.1
-5.2
-5.3
-5.4
-
-PDFgui shortcut keys . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
-Command line arguments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
-List of PDFfit2 variables. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 40
-PDF peak width . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 42
+5.1 PDFgui shortcut keys . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
+5.2 Command line arguments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
+5.3 List of PDFfit2 variables. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 40
+5.4 PDF peak width . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 42
 
 Index . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 43
 
 1
 
 1 Introduction
 PDFgui is a graphical interface built on the PDFfit2 engine, which is a program and programming library for real-space refinement of crystal structures based on the atomic pair
@@ -150,17 +148,16 @@
 C++, and many bugs have been fixed. The new engine uses dynamic memory allocation so
 that the size of the structure or extent of the fit-range of the PDF is limited only by the
 physical memory available. The constraint system has also been upgraded. The program
 automatically computes the analytical derivatives of the constraints that are required by
 the minimization routine. This simplifies user input and reduces the possibility of errors. In
 addition, new fitting parameters for handling dynamic atomic correlations and experimental
 resolution have been introduced as well.
-Instead of rewriting the PDFfit command interpreter, which is used to define the fitting
-problem and to control and run the refinement, its functions are carried out using the
-Python language (http://www.python.org). Python is a powerful, cross-platform, opensource interpreted programming language (i.e., it does not need to be compiled to run,
+Instead of rewriting the PDFfit command interpreter, which is used to define the fitting problem and to control and run the refinement, its functions are carried out using the
+Python language (https://www.python.org). Python is a powerful, cross-platform, opensource interpreted programming language (i.e., it does not need to be compiled to run,
 similar to scripting) that emphasizes object-oriented and modular design. PDFfit2 scripts
 written in Python syntax take the place of PDFfit macros and the Python interpreter can
 
 Chapter 1: Introduction
 
 2
 
@@ -180,15 +177,15 @@
 as real-time plotting. PDFgui has been designed with multitasking in mind. It is multithreaded so that the work being done by the PDFfit2 engine does not interfere with the
 tasks of the user interface.
 PDFgui is written in the Python programming language. Python features a relaxed and
 friendly syntax, supports “write once, run anywhere” portability, and has extensive libraries
 and modules for virtually every task. Software codes written in a variety of programming
 languages can be bound into Python, which allows them to be used together. Python is
 becoming a popular choice in the scientific computation community.
-PDFgui’s interface is built using wxPython (http://www.wxPython.org), the Python
+PDFgui’s interface is built using wxPython (https://www.wxpython.org), the Python
 package for wxWidgets, a mature cross-platform GUI library. Graphical applications written in wxPython provide a look and feel native to the platform on which they are run.
 PDFgui is designed to run on Windows, Mac OS, Linux, and all major Unix systems.
 
 1.2.2 Capabilities
 PDFgui contains all of the functionality of PDFfit2 along with additional enhancements for
 usability. Mundane tasks are handled by the program and difficult tasks are made simple.
 PDFgui can manage multiple fits at once. Each fit can have multiple experimental data
@@ -198,54 +195,53 @@
 be loaded on any computer. All management tasks, such as fit creation, configuration,
 modification, and visualization, can be done through the graphical interface.
 PDFgui supports space group operations. Users can define an asymmetric unit and let
 PDFgui expand it to a full cell with all symmetry related positions. PDFgui can also generate symmetry constraints for atom positions and atomic ADPs. Users just need to specify
 the space group, and the program will identify equivalent sites and generate constraint equations for their coordinates and temperature factors to keep the structure consistent with
 the symmetry requirements. This can be done either for all atoms in the structure or for an
 arbitrary subset - for example when it is known that only a certain species show a local distortion. The code for space group definitions was provided by the Python Macromolecular
-Library (mmLib, http://pymmlib.sourceforge.net). This was extened to include nonstandard space groups using the Computational Crystallography Toolbox (cctbx, http://
-cctbx.sourceforge.net). PDFgui also supports supercell expansion of a normal unit cell.
+Library (mmLib, http://pymmlib.sourceforge.net). This was extened to include nonstandard space groups using the Computational Crystallography Toolbox (cctbx, https://
+cctbx.github.io). PDFgui also supports supercell expansion of a normal unit cell.
 
 Chapter 1: Introduction
 
 3
 
-PDFgui uses the matplotlib (http://matplotlib.org) Python package for 2D plotting
+PDFgui uses the matplotlib (https://matplotlib.org) Python package for 2D plotting
 of data and results. Matplotlib has a friendly interface so the user can quickly and easily
 view the results of a fitting. PDFgui lets users plot data from a series of fits and plot it
 against selected meta-data (temperature, doping, etc.), plot the results of several fits in the
 same window, plot the PDF in real time as the fitting is running, plot the parameters or
-variables in real time as the refinement evolves, and save plots in common image formats
-or export the data to a text file. PDFgui can be configured to use one of many structure
-visualization packages, such as AtomEye (http://li.mit.edu/A/Graphics/A/) or PyMOL
-(http://www.pymol.org).
+variables in real time as the refinement evolves, and save plots in common image formats or
+export the data to a text file. PDFgui can be configured to use one of many structure visualization packages, such as AtomEye (http://li.mit.edu/A/Graphics/A/) or PyMOL
+(https://www.pymol.org).
 PDFgui supports built-in macros for advanced fits. For a set of experimental data from
 one system at different temperatures or doping levels, PDFgui can expand a template fit to
 a series of related fits. Another PDFgui macro makes it easy to set up boxcar fits, where
 the same model is fit over different r-ranges of the PDF data.
 
 1.3 Availability
 PDFfit2 and PDFgui are open source and distributed under a BSD license. They run on
 Windows, Mac OS, Linux, and all major Unix systems. The source code is freely available.
 For more information please contact Professor Simon Billinge (sb2896@columbia.edu) or
-consult the web-page http: / / www . diffpy . org. News of updates and releases will be
+consult the web-page https://www.diffpy.org. News of updates and releases will be
 posted at this website and on the diffpy-users group at https://groups.google.com/d/
 forum/diffpy-users.
 
 1.4 Installation
 PDFgui is included as a part of DiffPy, a suite of Python and C++ libraries for structure
 analysis from diffraction data. For more information about DiffPy products visit the project
-homepage at http://www.diffpy.org.
+homepage at https://www.diffpy.org.
 
 1.4.1 Installation for Anaconda Python
 As of version 1.1 PDFgui is distributed as a pre-built package for Anaconda Python
-(https://www.continuum.io). This method makes it easier to distribute software updates
+(https://www.anaconda.com). This method makes it easier to distribute software updates
 and also results in the same installation procedure on all supported platforms.
 To install PDFgui, download and install Anaconda for Python 2.7 from https://www.
-continuum.io/downloads. When ready open a terminal application (or Anaconda Command Prompt on Windows) and use the conda package manager to install PDFgui from
+anaconda.com/download. When ready open a terminal application (or Anaconda Command Prompt on Windows) and use the conda package manager to install PDFgui from
 the “diffpy” channel of Anaconda packages
 conda config --add channels diffpy
 conda install diffpy.pdfgui
 The first command instructs Anaconda system to always check the “diffpy” channel for
 any new software. Such configuration allows to obtain PDFgui updates using
 conda update diffpy.pdfgui
 It is however not strictly necessary to make the “diffpy” channel permanent. The
@@ -258,31 +254,31 @@
 
 After installation is complete PDFgui can be started from a terminal by entering pdfgui
 command or on Windows by using the DiffPy start menu. PDFgui can be also started from
 the “Launcher” program that is included with Anaconda.
 
 1.4.2 Configuration of structure viewer
 PDFgui can visualize 3D structures by displaying them with an external visualization program. The visualization program needs to be specified together with a suitable structure
-format in the “Edit 7→ Preferences” menu in PDFgui. The structure plotting feature has
+format in the “Edit → Preferences” menu in PDFgui. The structure plotting feature has
 been tested with the following programs:
 AtomEye
 
 AtomEye structure viewer, XCFG format
 http://li.mit.edu/A/Graphics/A/
 
 PyMOL
 
 PyMOL structure viewer, PDB format
-http://www.pymol.org
+https://www.pymol.org
 
 A note for AtomEye users:
 AtomEye requires its standard output is connected to a terminal. On Unix this happens
 when pdfgui is started from a terminal. However if you prefer to start PDFgui using a
 desktop shortcut or via “Run Application” dialog of the window manager, you need to put
-the following information to the “Edit 7→ Preferences” menu of PDFgui.
+the following information to the “Edit → Preferences” menu of PDFgui.
 Structure viewer executable: xterm
 Argument string: -iconic -e ATOMEYE %s
 Structure format: xcfg
 In the above, ATOMEYE is the path to the ATOMEYE executable.
 For Cygwin users, the workaround is to launch the executable from a batch file. Batch
 files can only run in a command window on Windows and so AtomEye’s requirements would
 be for sure satisfied. In addition the batch file can be used to adjust environment variables:
@@ -290,15 +286,15 @@
 -----------------------------------------------------------------------set DISPLAY=localhost:0
 set PATH=C:\cygwin\bin;C:\cygwin\usr\X11R6\bin;C:\ATOMEYE_DIR;%PATH%
 start A.exe %*
 -----------------------------------------------------------------------Here ATOMEYE_DIR needs to be replaced with a proper path. Make sure that the X-server
 application included with Cygwin is started.
 
 1.4.3 Installation from sources
-PDFgui sources are available in a public Git (https: / / git-scm . com) repository at
+PDFgui sources are available in a public Git (https://git-scm.com) repository at
 https://github.com/diffpy/diffpy.pdfgui. Feel free to fork this project on GitHub
 and contribute. To use the latest development version clone the Git repository to your
 computer and install it in a development mode so that sources are used directly rather
 than copied to a system location. It is also recommended to uninstall the Anaconda
 package for PDFgui, so that there is no confusion as to what version is the active one.
 Here are the shell commands that would do it:
 # Install PDFgui together with software dependencies.
@@ -320,15 +316,15 @@
 python setup.py develop
 To verify that PDFgui is indeed loaded from the local source repository run
 python -m pydoc diffpy.pdfgui
 and check the path displayed in the FILE section. The application integrity can be
 verified by executing all builtin tests using
 python -m diffpy.pdfgui.tests.rundeps
 Use git pull to bring your source directory into sync with the latest updates in the
-main repository. It is recommend to afterwards do ‘setup.py develop again to refresh the
+main repository. It is recommend to afterwards do `setup.py develop again to refresh the
 version metadata associated with the program:
 git pull
 python setup.py develop
 To revert PDFgui installation from the source-code installation back to the pre-built
 Anaconda package do
 pip uninstall diffpy.pdfgui
 conda install --channel=diffpy diffpy.pdfgui
@@ -369,15 +365,15 @@
 when there is some uncaught error in the at-exit cleanup functions.
 PDFgui tests
 PDFgui installation now includes built-in tests. Added facility to test PDFgui
 and all its DiffPy components. Implemented automated testing and generation
 of test coverage reports when sources on GitHub change.
 bug fixes
 
-Quite a few. Consult the code history at https: / / github . com / diffpy /
+Quite a few. Consult the code history at https://github.com/diffpy/
 diffpy.pdfgui/commits.
 
 Version 1.0, released April 2009
 This section describes improvements and modifications since the last beta-release 1.0b.1792
 from December 2007.
 updates and installation
 PDFgui can be installed or updated with a simple run of the easy install script.
@@ -407,17 +403,16 @@
 Implemented new module ‘tui’ (text user interface) for simple access to the data
 in PDFgui project files. The ‘tui’ module can be used in easy-to-understand
 Python scripts for arbitrary data extraction or conversion. It should be useful
 for project files with large temperature or compositional series of PDF refinements.
 structure visualization
 PDFgui can now show structures with any external structure viewer, that accepts structure file as a command-line argument.
 space group representations
-Added 249 space group representations in non-standard settings. The new
-representations were generated using the cctbx library (http: / / cctbx .
-sourceforge.net) and helpful hints from Ralf W. Grosse-Kunstleve.
+Added 249 space group representations in non-standard settings. The new representations were generated using the cctbx library (https://cctbx.github.
+io) and helpful hints from Ralf W. Grosse-Kunstleve.
 symmetry constraints
 Fixed issues with generation of symmetry requirements for the ADP tensors.
 default ADP tensors
 PDF contributions are not counted for atoms that have ADP tensors Uij equal
 zero. Atoms are now inserted with a non-zero Uij matrix. Added warning when
 a phase loaded from file has atoms with zero ADPs.
 temperature series macro
@@ -540,43 +535,45 @@
 tab.
 Figure 2.2 shows the PDFgui appearance at this stage of the exercise. The “Configure”
 panel displays configuration information from the data file. It should be noted that depending on the software used to prepare the experimental PDF from the raw data, the file may
 (or may not) contain meta-data reflecting the experimental conditions and configuration.
 For example, software PDFgetX2 and PDFgetN, which can be used to prepare PDFs from
 x-ray and neutron total scattering experiments respectively, supply meta-data in the header
 of the data file. PDFgui reads this information and fills the appropriate fields in the data
-set configuration panel. Caution should be exercised by the user to verify that these data
 
 Chapter 2: Quick start
 
 12
 
+set configuration panel. Caution should be exercised by the user to verify that these data
 indeed correspond to the experimental conditions. In the present example, x-ray radiation
 is used, and so the x-ray selection is turned on for the scatterer type. The data range, fit
 range, data scale factor, maximum Q value used in Fourier transform to obtain the experimental PDF and the experiment specific parameters are displayed. Parameters describing
 experimental resolution effects, Qdamp and Qbroad, and experimental conditions, such as
 temperature and doping (used for bookkeeping and for parametric plots) are also shown.
 If no meta-data are present in a data file, this information should be supplied by the user.
 Note also that the changes occurred at this stage in the plot control panel, allowing user to
 plot the data. This is achieved by selecting r in the X-choice box and Gobs (the observed
 G(r)) in the Y-list box and then pressing the “Plot” button. Since no fitting has occurred
 so far, an attempt to plot calculated PDF profile or a difference yields a blank plot. The
 data can also be displayed by clicking the rightmost “quick-plot” button in the tool bar.
 
 Figure 2.3: Adjusting data set related configuration.
+
 Having specified the initial structure to be refined, and the data set to be fit, we proceed
 to the refinement setup. First we adjust the initial parameters and variables, and set up
 the constraints. The adjustments and constraint setup are done on both the experimental
-data and the refined structure levels, toggling between the corresponding “Configure” and
-“Constraints” tabs. In the present example the data related setup will be done first.
 
 Chapter 2: Quick start
 
 13
 
+data and the refined structure levels, toggling between the corresponding “Configure” and
+“Constraints” tabs. In the present example the data related setup will be done first.
+
 Click on the data set node (Ni-xray.gr ) in the fit tree. In Figure 2.3 the “Data Set
 Configuration” panel is shown. We will adjust the fitting range, as well as other parameters
 that reflect the experimental conditions. Since there is no physical information in the region
 of r below the nearest neighbor PDF peak position (as seen in the plot), and since this region
 is often affected by noise and experimental artifacts, it is wise to exclude it from fitting.
 We therefore set the value of the lower boundary of the fitting range to 1.7. (Note that the
 units are Angstroms). In addition, we set Qdamp parameter to a more realistic starting
@@ -585,49 +582,48 @@
 Ni or Si. Next, we select the “Constraints” tab, and type @1 into the “Scale Factor” edit
 box. This will assign refinement parameter 1 to the data scale factor. Note that this is the
 syntax used for assigning the refinement parameters in PDFfit2 engine. Similarly, assign
 parameter 2 to Qdamp by inserting @2 into the appropriate edit box. This is illustrated in
 Figure Figure 2.4.
 
 Figure 2.4: Setting up the refinement parameters and constraints.
-Further, we set constraints related to the structural model, by selecting the phase node
-(Ni.stru) on the fit tree, adjusting the initial parameter values if necessary (not done here),
-and proceeding to the “Constraints” tab. We note that the phase configuration was performed automatically when the structure file was loaded. We assign the refinement parame-
 
 Chapter 2: Quick start
 
 14
 
-ter 3 to all three lattice constants, a, b, and c, reflecting the fact that the structure is cubic.
+Further, we set constraints related to the structural model, by selecting the phase node
+(Ni.stru) on the fit tree, adjusting the initial parameter values if necessary (not done here),
+and proceeding to the “Constraints” tab. We note that the phase configuration was performed automatically when the structure file was loaded. We assign the refinement parameter 3 to all three lattice constants, a, b, and c, reflecting the fact that the structure is cubic.
 Isotropic ADPs are assigned to all Ni atoms in the refined cell as refinement parameter 4.
 This can conveniently be done by highlighting the “u11”, “u22” and “u33” cells for all four
 atoms, and typing @4 and then pressing “Enter” on your keyboard. The outcome is shown
 in Figure Figure 2.5.
 
 Figure 2.5: Setting up the refinement parameters and constraints.
 Note that constrained parameters cannot be adjusted on the “Configuration” panel since
 they are no longer independent. It should also be noted that as a part of the PDFfit2 syntax
 a refinement parameter can also be defined as a math expression f(@n1,@n2,@n3,...) where
 @n1 stands for fitted parameter, and n1, n2,... are arbitrary positive integers enumerating
 the parameters. This allows simple linking of related variables. For example, since cell
 lengths a, b, and c are all expressed as @3, the refined structure will remain cubic. Also
 note that the enumeration of the parameters can be arbitrary, enumeration does not have
 to follow any particular order. The quantities within a fit that are enumerated with the
+
+Chapter 2: Quick start
+
+15
+
 same number will be assigned the same parameter, hence caution should be exercised to
 avoid unintentional assignment of the same parameter to physically different quantities.
 Automatic parameter assignment (see further below) is done in such a way as to disallow for
 such situations to happen. If assignment is done in part manually, in particular for complex
 setups, it is recommended to verify that the parameter assignment is done correctly.
 
-Chapter 2: Quick start
-
-15
-
 Figure 2.6: Reviewing the fit parameters and conditions.
-
 The setup for the present example is now completed. By selecting the fit node on the fit
 tree the current action window shows “Parameters” tab, which displays the used refinement
 parameters for review, Figure 2.6. It shows the initial values, and allows for updates and
 for refinement parameters to be released or fixed depending on whether the corresponding
 “Fixed” box is unchecked or checked, respectively. The “Refined” column, which is currently
 empty, will be populated with the refined values of the parameters with the fit completes.
 If the initial parameter values are to be changed, using “Apply parameters” button will
@@ -1047,48 +1043,46 @@
 task would be to extract bond lengths for every temperature refined in a large series. The
 GUI could supply menus for these tasks, but there are just too many options to serve them
 all. In fact, the GUI just does not seem to be suitable interface and things are much easier
 and more flexible to accomplish with Python scripts.
 The idea is to setup and run sequential refinement with PDFgui, but to do complicated
 data extractions with simple Python scripts. The PDFgui installation includes a ‘tui’ (Text
 User Interface) module that allows simple access to the data in a PDFgui project.
-As a first example, let us assume that a converged sequential refinement from
-Section 3.3.3 [Temperature series], page 27, has been saved under the same name as
-lmo-template.ddp. The following Python script extracts temperatures and refined values of
-the lattice parameter c
+As a first example, let us assume that a converged sequential refinement from Section 3.3.3 [Temperature series], page 27, has been saved under the same name as lmotemplate.ddp. The following Python script extracts temperatures and refined values of the
+lattice parameter c
 
 Chapter 3: Examples and tutorials
 
 33
 
 # python script
 from diffpy.pdfgui import tui
 # import the tui library
-prj = tui.LoadProject(’lmo-template.ddp’) # read PDFgui project file
+prj = tui.LoadProject('lmo-template.ddp') # read PDFgui project file
 temperatures = prj.getTemperatures()
 # list of temperature values
 phases = prj.getPhases()
 # list of phase objects
 tcount = len(temperatures)
 # number of temperature points
 for i in range(tcount):
 Ti = temperatures[i]
 # get the refined lattice parameter c
 ci = phases[i].refined.lattice.c
-print Ti, ci
+print(Ti, ci)
 Save the example above to a file, say “lmo refined c.py” and run it as
 python lmo_refined_c.py
 Note that the script cannot load the unmodified lmo-template.ddp file, because it does not
 have any refinement results.
 The tutorial directory contains an advanced script “tui mno bond lengths.py”, which
 extracts the shortest Mn-O bond lengths from the same PDFgui project. Please, see the
 comments in the script for detailed explanation.
 To learn more about the tui module and about the objects and functions that it returns, please see the API documentation for diffpy.pdfgui at http://docs.danse.us/
 diffraction/diffpy.pdfgui/.
-Feel free to ask at the diffpy-users (https: / / groups . google . com / d / forum /
+Feel free to ask at the diffpy-users (https://groups.google.com/d/forum/
 diffpy-users) group if you need help with data extracting scripts.
 
 3.4 Nanoparticle structure
 Determining the structure of a nanoparticle is notoriously difficult. Diffraction experiments
 on nanoparticle samples yield broad diffraction patterns that are hard to analyze using
 conventional crystallographic approaches. The PDF analysis of nanoparticles is becoming
 increasingly common. The PDF of a nanoparticle features sharp peaks conveying structural
@@ -1134,17 +1128,19 @@
 nanoparticle data reveals nanoparticle diameter of approximately 30 Angstroms, as further
 illustrated in Figure 3.10. Enlarged values of isotropic ADPs are again observed, and the
 fit is reasonably good. Further improvements can be obtained by introducing anisotropic
 ADPs, where again values related to the z-direction will remain abnormally large most
 probably due to the stacking related disorder. A detailed description of this system and
 successful PDF modeling can be found in this publication: Quantitative size-dependent
 structure and strain determination of CdSe nanoparticles using atomic pair distribution
-function analysis (http://link.aps.org/doi/10.1103/PhysRevB.76.115413).
+function analysis (https://link.aps.org/doi/10.1103/PhysRevB.76.115413).
+
+Chapter 3: Examples and tutorials
 
-35
+35
 
 Figure 3.10: Fitting the structure of a nanoparticle: 3nm CdSe nanoparticle example.
 In general, a successful fitting scenario depends on particular details of a structural problem one is determined to solve. The problem of determining the structure of a nanoparticle
 remains difficult. PDFgui is not intended to necessarily provide the solution, it is rather a
 helpful tool in the process of determining new details and exploring the space of possible
 solution candidates, yielding success in some instances.
 
@@ -1198,19 +1194,18 @@
 
 4.3 Advanced usage and special needs
 The PDFgui is designed to accommodate most common modeling situations. However,
 it does not encapsulate all the capabilities available within the modeling engine, such as
 calculation of differential PDFs, handling atoms with special scattering properties, etc.
 Advanced usage of PDFfit2 engine to resolve any such special modeling need that user
 may have is available through usage of Python scripts in the expert command line mode,
-similar to that featured in the PDFFIT program. Handling these situations requires detailed
-knowledge of the PDFfit2 syntax based on Python, which is beyond the scope of this user
-guide and will be described elsewhere. Refer to the PDFfit2 API (http://www.diffpy.
-org/doc/pdffit2/ and the diffpy-users group (https://groups.google.com/d/forum/
-diffpy-users) for help with PDFfit2 scripting.
+similar to that featured in the PDFFIT program. Handling these situations requires detailed knowledge of the PDFfit2 syntax based on Python, which is beyond the scope of
+this user guide and will be described elsewhere. Refer to the PDFfit2 API (https://
+www.diffpy.org/doc/pdffit2 and the diffpy-users group (https://groups.google.com/
+d/forum/diffpy-users) for help with PDFfit2 scripting.
 
 39
 
 5 PDFgui reference sheets
 5.1 PDFgui shortcut keys
 Fit tree
 Ctrl+A
```

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/1050K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1050K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/1100K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1100K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/1150K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/1150K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/300K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/300K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/550K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/550K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/650K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/650K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/700K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/700K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/720K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/720K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/730K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/730K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/740K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/740K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/750K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/750K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/800K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/800K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/880K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/880K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/980K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/980K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-3nm.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-3nm.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-bulk.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-bulk.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-nano.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-nano.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/CdSe-wurtzite.stru` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/CdSe-wurtzite.stru`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/Ni-neutron.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni-neutron.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/Ni-xray.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni-xray.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/Ni.stru` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/Ni.stru`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/lcmo-template.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/lcmo-template.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/lmo-template.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/lmo-template.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/tui_mno_bond_lengths.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/tui_mno_bond_lengths.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x000t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x000t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x004t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x004t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x012t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x012t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x016t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x016t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x020t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x020t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x024t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x024t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/doc/tutorial/x028t010q35.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/doc/tutorial/x028t010q35.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/C60_16x16.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/C60_16x16.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/columbia_logo.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/columbia_logo.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/danse_logo.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/danse_logo.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/fitting.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/fitting.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/logo.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/msu_logo.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/msu_logo.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/nsf_logo.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/nsf_logo.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/pdfgui.ico` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/pdfgui.ico`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/phaseitem.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/phaseitem.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/plotting.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/plotting.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/run.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/run.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/stop.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/stop.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/icons/titlepage.png` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/icons/titlepage.png`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/setup.py` & `diffpy.pdfgui-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import re
 import sys
 from setuptools import setup, find_packages
 
 # Use this version when git data are not available, like in git zip archive.
 # Update when tagging a new release.
-FALLBACK_VERSION = '1.4.2'
+FALLBACK_VERSION = '2.0.0'
 
 # determine if we run with Python 3.
 PY3 = (sys.version_info[0] == 3)
 
 # versioncfgfile holds version data for git commit hash and date.
 # It must reside in the same directory as version.py.
 MYDIR = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/applications/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/applications/pdfgui.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/applications/pdfgui.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         raise ValueError(emsg)
     # ready to go
     pdfguiglobals.cmdargs = args
     return proceed
 
 
 def main():
-    '''Main entry point to PDFgui.
+    '''Main entry point to  PDFgui.
     '''
     # process arguments
     proceed = False
     try:
         proceed = processArguments(sys.argv[1:])
     except (getopt.GetoptError, ValueError) as err:
         print(err, file=sys.stderr)
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/calculation.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/calculation.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/constraint.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/constraint.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/controlerrors.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/controlerrors.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitdataset.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitdataset.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitstructure.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitstructure.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/fitting.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,15 +549,15 @@
             self.pause(False)
 
     def isThreadRunning(self):
         """check if fitting thread is running
 
         return: True if running, False otherwise
         """
-        return self.thread is not None and self.thread.isAlive()
+        return self.thread is not None and self.thread.is_alive()
 
     def join(self):
         """wait for current fitting to finish"""
         if self.thread:
             self.thread.join()
             self.thread = None
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/organizer.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/organizer.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/parameter.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/parameter.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfcomponent.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfcomponent.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfdataset.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfdataset.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfguicontrol.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfguicontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         self.reset()
 
     def exit(self):
         """exit when program finished
         """
         self.close()
-        if self.queueManager.isAlive():
+        if self.queueManager.is_alive():
             self.queueManager.running = False
 
     def newFitting(self, name, position=None):
         """insert a new instance of Fitting
 
         name      --  unique name for this Fitting
         position  --  where Fitting is inserted, default is last place
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfguimacros.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfguimacros.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdflist.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdflist.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/pdfstructure.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/pdfstructure.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/plotter.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/plotter.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/control/structureviewer.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/control/structureviewer.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/DesignNotes.txt` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/DesignNotes.txt`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/aboutdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/adddatapanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/adddatapanel.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,46 +34,44 @@
     """
 
     def __init__(self, *args, **kwds):
         PDFPanel.__init__(self)
         # begin wxGlade: AddDataPanel.__init__
         kwds["style"] = kwds.get("style", 0) | wx.TAB_TRAVERSAL
         wx.Panel.__init__(self, *args, **kwds)
-        self.textLoadData = wx.StaticText(self, wx.ID_ANY, "Load a data set from file.")
-        self.buttonOpen = wx.Button(self, wx.ID_OPEN, "Open")
-        self.static_line_2 = wx.StaticLine(self, wx.ID_ANY)
-        self.buttonCancel = wx.Button(self, wx.ID_CANCEL, "Cancel")
 
-        self.__set_properties()
-        self.__do_layout()
+        sizer_1 = wx.BoxSizer(wx.VERTICAL)
 
-        self.Bind(wx.EVT_BUTTON, self.onOpen, self.buttonOpen)
-        self.Bind(wx.EVT_BUTTON, self.onCancel, self.buttonCancel)
-        # end wxGlade
-        self.__customProperties()
+        sizer_4 = wx.BoxSizer(wx.HORIZONTAL)
+        sizer_1.Add(sizer_4, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)
 
-    def __set_properties(self):
-        # begin wxGlade: AddDataPanel.__set_properties
+        self.textLoadData = wx.StaticText(self, wx.ID_ANY, "Load a data set from file.")
         self.textLoadData.SetFont(wx.Font(12, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_NORMAL, 0, "Sans"))
-        # end wxGlade
-
-    def __do_layout(self):
-        # begin wxGlade: AddDataPanel.__do_layout
-        sizer_1 = wx.BoxSizer(wx.VERTICAL)
-        sizer_4 = wx.BoxSizer(wx.HORIZONTAL)
         sizer_4.Add(self.textLoadData, 1, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
-        sizer_4.Add(self.buttonOpen, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.ALL, 5)
-        sizer_1.Add(sizer_4, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)
+
+        self.buttonOpen = wx.Button(self, wx.ID_OPEN, "Open")
+        sizer_4.Add(self.buttonOpen, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
+
+        self.static_line_2 = wx.StaticLine(self, wx.ID_ANY)
         sizer_1.Add(self.static_line_2, 0, wx.BOTTOM | wx.EXPAND, 10)
-        sizer_1.Add(self.buttonCancel, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.ALL, 5)
+
+        self.buttonCancel = wx.Button(self, wx.ID_CANCEL, "Cancel")
+        sizer_1.Add(self.buttonCancel, 0, wx.ALIGN_RIGHT | wx.ALL, 5)
+
         sizer_1.Add((450, 0), 0, 0, 0)
+
         self.SetSizer(sizer_1)
         sizer_1.Fit(self)
+
         self.Layout()
+
+        self.Bind(wx.EVT_BUTTON, self.onOpen, self.buttonOpen)
+        self.Bind(wx.EVT_BUTTON, self.onCancel, self.buttonCancel)
         # end wxGlade
+        self.__customProperties()
 
     # UTILITY FUNCTIONS ####
 
     def __customProperties(self):
         """Custom Properties go here."""
         self.entrypoint = None  # The entrypoint on the tree
         self.entryfit = None    # The fit under which to insert an item
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/addphasepanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/addphasepanel.py~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/blankpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/blankpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/bondangledialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/bondangledialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/bondlengthdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/bondlengthdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/calculationpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/calculationpanel.py~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetconfigurepanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconfigurepanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,115 +24,144 @@
 
 class DataSetConfigurePanel(wx.Panel, PDFPanel):
     def __init__(self, *args, **kwds):
         PDFPanel.__init__(self)
         # begin wxGlade: DataSetConfigurePanel.__init__
         kwds["style"] = kwds.get("style", 0) | wx.TAB_TRAVERSAL
         wx.Panel.__init__(self, *args, **kwds)
-        self.panelNameLabel = wx.StaticText(self, wx.ID_ANY, "Data Set Configuration")
-        self.radioBoxStype = wx.RadioBox(self, wx.ID_ANY, "Scatterer Type", choices=["Neutron", "X-ray"], majorDimension=2, style=wx.RA_SPECIFY_COLS)
-        self.radioBoxSampling = wx.RadioBox(self, wx.ID_ANY, "Data Sampling", choices=["Data", "Nyquist", "Custom"], majorDimension=3, style=wx.RA_SPECIFY_COLS)
-        self.labelDataRange = wx.StaticText(self, wx.ID_ANY, "Data Range")
-        self.textCtrlDataFrom = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
-        self.labelDataTo = wx.StaticText(self, wx.ID_ANY, "to")
-        self.textCtrlDataTo = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
-        self.labelDataStep = wx.StaticText(self, wx.ID_ANY, "spacing")
-        self.textCtrlDataStep = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
-        self.labelFitRange = wx.StaticText(self, wx.ID_ANY, "Fit Range", style=wx.ALIGN_RIGHT)
-        self.textCtrlFitFrom = wx.TextCtrl(self, wx.ID_ANY, "1.0")
-        self.labelFitTo = wx.StaticText(self, wx.ID_ANY, "to", style=wx.ALIGN_RIGHT)
-        self.textCtrlFitTo = wx.TextCtrl(self, wx.ID_ANY, "10.0")
-        self.labelFitStep = wx.StaticText(self, wx.ID_ANY, "spacing")
-        self.textCtrlFitStep = wx.TextCtrl(self, wx.ID_ANY, "0")
-        self.labelScaleFactor = wx.StaticText(self, wx.ID_ANY, "Scale Factor", style=wx.ALIGN_RIGHT)
-        self.textCtrlScaleFactor = wx.TextCtrl(self, wx.ID_ANY, "1.0")
-        self.labelQmax = wx.StaticText(self, wx.ID_ANY, "Qmax", style=wx.ALIGN_RIGHT)
-        self.textCtrlQmax = wx.TextCtrl(self, wx.ID_ANY, "25.0")
-        self.blank1_copy = wx.StaticText(self, wx.ID_ANY, "")
-        self.blank1_copy_4 = wx.StaticText(self, wx.ID_ANY, "")
-        self.labelQdamp = wx.StaticText(self, wx.ID_ANY, "Qdamp", style=wx.ALIGN_RIGHT)
-        self.textCtrlQdamp = wx.TextCtrl(self, wx.ID_ANY, "0.0")
-        self.labelQbroad = wx.StaticText(self, wx.ID_ANY, "Qbroad", style=wx.ALIGN_RIGHT)
-        self.textCtrlQbroad = wx.TextCtrl(self, wx.ID_ANY, "0.0")
-        self.blank1_copy_1 = wx.StaticText(self, wx.ID_ANY, "")
-        self.blank1_copy_5 = wx.StaticText(self, wx.ID_ANY, "")
-        self.labelTemperature = wx.StaticText(self, wx.ID_ANY, "Temperature", style=wx.ALIGN_RIGHT)
-        self.textCtrlTemperature = wx.TextCtrl(self, wx.ID_ANY, "300.0")
-        self.labelDoping = wx.StaticText(self, wx.ID_ANY, "Doping", style=wx.ALIGN_RIGHT)
-        self.textCtrlDoping = wx.TextCtrl(self, wx.ID_ANY, "1.0")
-        self.blank1_copy_3 = wx.StaticText(self, wx.ID_ANY, "")
-        self.blank1_copy_7 = wx.StaticText(self, wx.ID_ANY, "")
 
-        self.__set_properties()
-        self.__do_layout()
+        sizer_1 = wx.BoxSizer(wx.HORIZONTAL)
 
-        self.Bind(wx.EVT_RADIOBOX, self.onStype, self.radioBoxStype)
-        self.Bind(wx.EVT_RADIOBOX, self.onSampling, self.radioBoxSampling)
-        # end wxGlade
-        self.__customProperties()
+        outerSizer = wx.BoxSizer(wx.VERTICAL)
+        sizer_1.Add(outerSizer, 1, wx.EXPAND, 0)
+
+        sizer_panelname = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, ""), wx.HORIZONTAL)
+        outerSizer.Add(sizer_panelname, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
 
-    def __set_properties(self):
-        # begin wxGlade: DataSetConfigurePanel.__set_properties
+        self.panelNameLabel = wx.StaticText(self, wx.ID_ANY, "Data Set Configuration")
         self.panelNameLabel.SetFont(wx.Font(18, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_BOLD, 0, ""))
+        sizer_panelname.Add(self.panelNameLabel, 0, wx.ALIGN_CENTER_VERTICAL | wx.LEFT | wx.RIGHT, 5)
+
+        outerSizer.Add((450, 5), 0, 0, 0)
+
+        self.radioBoxStype = wx.RadioBox(self, wx.ID_ANY, "Scatterer Type", choices=["Neutron", "X-ray"], majorDimension=2, style=wx.RA_SPECIFY_COLS)
         self.radioBoxStype.SetMinSize((330, 43))
         self.radioBoxStype.SetSelection(0)
+        outerSizer.Add(self.radioBoxStype, 0, wx.ALL, 5)
+
+        self.radioBoxSampling = wx.RadioBox(self, wx.ID_ANY, "Data Sampling", choices=["Data", "Nyquist", "Custom"], majorDimension=3, style=wx.RA_SPECIFY_COLS)
         self.radioBoxSampling.SetMinSize((232, 44))
         self.radioBoxSampling.SetSelection(0)
-        self.textCtrlDataFrom.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
-        self.textCtrlDataTo.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
-        self.textCtrlDataStep.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
-        # end wxGlade
+        outerSizer.Add(self.radioBoxSampling, 0, wx.ALL, 5)
 
-    def __do_layout(self):
-        # begin wxGlade: DataSetConfigurePanel.__do_layout
-        sizer_1 = wx.BoxSizer(wx.HORIZONTAL)
-        outerSizer = wx.BoxSizer(wx.VERTICAL)
         grid_sizer_1 = wx.FlexGridSizer(5, 6, 5, 10)
-        sizer_panelname = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, ""), wx.HORIZONTAL)
-        sizer_panelname.Add(self.panelNameLabel, 0, wx.ALIGN_CENTER_VERTICAL | wx.LEFT | wx.RIGHT, 5)
-        outerSizer.Add(sizer_panelname, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
-        outerSizer.Add((450, 5), 0, 0, 0)
-        outerSizer.Add(self.radioBoxStype, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
-        outerSizer.Add(self.radioBoxSampling, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
+        outerSizer.Add(grid_sizer_1, 0, wx.ALL | wx.EXPAND, 5)
+
+        self.labelDataRange = wx.StaticText(self, wx.ID_ANY, "Data Range")
         grid_sizer_1.Add(self.labelDataRange, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 5)
+
+        self.textCtrlDataFrom = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
+        self.textCtrlDataFrom.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
         grid_sizer_1.Add(self.textCtrlDataFrom, 0, 0, 0)
+
+        self.labelDataTo = wx.StaticText(self, wx.ID_ANY, "to")
         grid_sizer_1.Add(self.labelDataTo, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlDataTo = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
+        self.textCtrlDataTo.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
         grid_sizer_1.Add(self.textCtrlDataTo, 0, 0, 0)
+
+        self.labelDataStep = wx.StaticText(self, wx.ID_ANY, "spacing")
         grid_sizer_1.Add(self.labelDataStep, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlDataStep = wx.TextCtrl(self, wx.ID_ANY, "", style=wx.TE_READONLY)
+        self.textCtrlDataStep.SetBackgroundColour(wx.SystemSettings.GetColour(wx.SYS_COLOUR_GRAYTEXT))
         grid_sizer_1.Add(self.textCtrlDataStep, 0, 0, 0)
+
+        self.labelFitRange = wx.StaticText(self, wx.ID_ANY, "Fit Range", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelFitRange, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 5)
+
+        self.textCtrlFitFrom = wx.TextCtrl(self, wx.ID_ANY, "1.0")
         grid_sizer_1.Add(self.textCtrlFitFrom, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelFitTo = wx.StaticText(self, wx.ID_ANY, "to", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelFitTo, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlFitTo = wx.TextCtrl(self, wx.ID_ANY, "10.0")
         grid_sizer_1.Add(self.textCtrlFitTo, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelFitStep = wx.StaticText(self, wx.ID_ANY, "spacing")
         grid_sizer_1.Add(self.labelFitStep, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlFitStep = wx.TextCtrl(self, wx.ID_ANY, "0")
         grid_sizer_1.Add(self.textCtrlFitStep, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelScaleFactor = wx.StaticText(self, wx.ID_ANY, "Scale Factor", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelScaleFactor, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 5)
+
+        self.textCtrlScaleFactor = wx.TextCtrl(self, wx.ID_ANY, "1.0")
         grid_sizer_1.Add(self.textCtrlScaleFactor, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelQmax = wx.StaticText(self, wx.ID_ANY, "Qmax", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelQmax, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlQmax = wx.TextCtrl(self, wx.ID_ANY, "25.0")
         grid_sizer_1.Add(self.textCtrlQmax, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.blank1_copy = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy, 0, 0, 0)
+
+        self.blank1_copy_4 = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy_4, 0, 0, 0)
+
+        self.labelQdamp = wx.StaticText(self, wx.ID_ANY, "Qdamp", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelQdamp, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 5)
+
+        self.textCtrlQdamp = wx.TextCtrl(self, wx.ID_ANY, "0.0")
         grid_sizer_1.Add(self.textCtrlQdamp, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelQbroad = wx.StaticText(self, wx.ID_ANY, "Qbroad", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelQbroad, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlQbroad = wx.TextCtrl(self, wx.ID_ANY, "0.0")
         grid_sizer_1.Add(self.textCtrlQbroad, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.blank1_copy_1 = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy_1, 0, 0, 0)
+
+        self.blank1_copy_5 = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy_5, 0, 0, 0)
+
+        self.labelTemperature = wx.StaticText(self, wx.ID_ANY, "Temperature", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelTemperature, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 5)
+
+        self.textCtrlTemperature = wx.TextCtrl(self, wx.ID_ANY, "300.0")
         grid_sizer_1.Add(self.textCtrlTemperature, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.labelDoping = wx.StaticText(self, wx.ID_ANY, "Doping", style=wx.ALIGN_RIGHT)
         grid_sizer_1.Add(self.labelDoping, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALIGN_RIGHT | wx.LEFT, 20)
+
+        self.textCtrlDoping = wx.TextCtrl(self, wx.ID_ANY, "1.0")
         grid_sizer_1.Add(self.textCtrlDoping, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        self.blank1_copy_3 = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy_3, 0, 0, 0)
+
+        self.blank1_copy_7 = wx.StaticText(self, wx.ID_ANY, "")
         grid_sizer_1.Add(self.blank1_copy_7, 0, 0, 0)
-        outerSizer.Add(grid_sizer_1, 0, wx.ALL | wx.EXPAND, 5)
-        sizer_1.Add(outerSizer, 1, wx.EXPAND, 0)
+
         self.SetSizer(sizer_1)
         sizer_1.Fit(self)
+
         self.Layout()
+
+        self.Bind(wx.EVT_RADIOBOX, self.onStype, self.radioBoxStype)
+        self.Bind(wx.EVT_RADIOBOX, self.onSampling, self.radioBoxSampling)
         # end wxGlade
+        self.__customProperties()
 
     # USER CONFIGURATION CODE #################################################
 
     def __customProperties(self):
         # Set some reasonable defaults
         self.configuration = None
         self.constraints = {}
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetconstraintpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetconstraintpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/datasetresultspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/datasetresultspanel.py~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/debugoptions.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/debugoptions.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/aboutdialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/aboutdialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/adddatapanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/adddatapanel.wxg~`

 * *Files 6% similar despite different names*

#### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/adddatapanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/adddatapanel.wxg~`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- generated by wxGlade 0.9.3 on Fri Jul 19 15:56:56 2019 -->
+<!-- generated by wxGlade 1.0.4 on Sun Apr 23 11:11:00 2023 -->
 <application encoding="ISO-8859-1" for_version="3.0" header_extension=".h" indent_amount="4" indent_symbol="space" is_template="0" language="python" mark_blocks="1" option="0" overwrite="0" path="../adddatapanel.py" source_extension=".cpp" use_gettext="0" use_new_namespace="1">
   <object class="AddDataPanel" name="panel_1" base="EditTopLevelPanel">
     <style>wxTAB_TRAVERSAL</style>
     <object class="wxBoxSizer" name="sizer_1" base="EditBoxSizer">
       <orient>wxVERTICAL</orient>
       <object class="sizeritem">
         <option>0</option>
@@ -27,15 +27,15 @@
               <label>Load a data set from file.</label>
               <attribute>1</attribute>
             </object>
           </object>
           <object class="sizeritem">
             <option>0</option>
             <border>5</border>
-            <flag>wxALL|wxALIGN_RIGHT|wxALIGN_CENTER_VERTICAL</flag>
+            <flag>wxALL|wxALIGN_CENTER_VERTICAL</flag>
             <object class="wxButton" name="buttonOpen" base="EditButton">
               <events>
                 <handler event="EVT_BUTTON">onOpen</handler>
               </events>
               <id>wx.ID_OPEN</id>
               <label>Open</label>
             </object>
@@ -50,15 +50,15 @@
           <style>wxLI_HORIZONTAL</style>
           <attribute>1</attribute>
         </object>
       </object>
       <object class="sizeritem">
         <option>0</option>
         <border>5</border>
-        <flag>wxALL|wxALIGN_RIGHT|wxALIGN_CENTER_VERTICAL</flag>
+        <flag>wxALL|wxALIGN_RIGHT</flag>
         <object class="wxButton" name="buttonCancel" base="EditButton">
           <events>
             <handler event="EVT_BUTTON">onCancel</handler>
           </events>
           <id>wx.ID_CANCEL</id>
           <label>Cancel</label>
         </object>
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/addphasepanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/addphasepanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/bondlengthdialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/bondlengthdialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/calculationpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/calculationpanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetconfigurepanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconfigurepanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetconstraintpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetconstraintpanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetpanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/datasetresultspanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/datasetresultspanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/dopingseriespanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/dopingseriespanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/errorreportdialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/errorreportdialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/fitnotebookpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/fitnotebookpanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/insertrowsdialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/insertrowsdialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/journalpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/journalpanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/outputpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/outputpanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/parameterspanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/parameterspanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseconfigurepanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconfigurepanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseconstraintspanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseconstraintspanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/phaseresultspanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/phaseresultspanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/plotpanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/plotpanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/preferencespanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/preferencespanel.wxg~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/resultspanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/resultspanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/rseriespanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/rseriespanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/sgconstraindialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgconstraindialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/sgstructuredialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/sgstructuredialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/supercelldialog.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/supercelldialog.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/design/temperatureseriespanel.wxg` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/design/temperatureseriespanel.wxg`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/dopingseriespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/dopingseriespanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorreportdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorreportdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorreportdialog_control_fix.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorreportdialog_control_fix.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/errorwrapper.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/errorwrapper.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/extendedplotframe.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/extendedplotframe.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/fitnotebookpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/fitnotebookpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/fittree.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/fittree.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/gui_organization.txt` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/gui_organization.txt`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/insertrowsdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/insertrowsdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/journalpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/journalpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/main.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/main.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/mainframe.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/mainframe.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/menuitems.txt` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/menuitems.txt`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/outputpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/outputpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/paneltest.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/paneltest.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/parameterspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/parameterspanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/pdfguiglobals.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/pdfguiglobals.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,30 +19,38 @@
 from pkg_resources import Requirement, resource_filename
 
 # Name of the program
 name = "PDFgui"
 # Maximum number of files to be remembered
 MAXMRU = 5
 # The location of the configuration file
-configfilename = os.path.expanduser("~/.pdfgui.cfg")
+configfilename = os.path.expanduser("~/.pdfgui_py3.cfg")
 # Project modification flag
 isAltered = False
 
 # Resolve APPDATADIR base path to application data files.
 _mydir = os.path.abspath(resource_filename(__name__, ''))
 _upbasedir = os.path.normpath(_mydir + '/../../..')
 _development_mode = (
     os.path.basename(_upbasedir) == "src" and
     os.path.isfile(os.path.join(_upbasedir, "../setup.py"))
 )
 
 # Requirement must have egg-info.  Do not use in _development_mode.
 _req = Requirement.parse("diffpy.pdfgui")
-APPDATADIR = (os.path.dirname(_upbasedir) if _development_mode
-              else resource_filename(_req, ""))
+
+#pavol
+# APPDATADIR = (os.path.dirname(_upbasedir) if _development_mode
+#               else resource_filename(_req, ""))
+#long
+if _development_mode:
+    APPDATADIR = os.path.dirname(_mydir)
+else:
+    APPDATADIR = os.path.join(resource_filename(_req, ""), "diffpy/pdfgui")
+
 APPDATADIR = os.path.abspath(APPDATADIR)
 
 # Location of the HTML manual
 docMainFile = os.path.join(APPDATADIR, 'doc/manual/pdfgui.html')
 
 del _upbasedir
 del _development_mode
@@ -55,19 +63,14 @@
     to custom icons.
 
     iconfilename -- icon file name without any path
 
     Return string.
     """
     rv = os.path.join(APPDATADIR, 'icons', iconfilename)
-    print("APPDATADIR")
-    print(APPDATADIR)
-    print("rv")
-    print(rv)
-    print(os.path.isfile(rv))
     assert os.path.isfile(rv), "icon file does not exist"
     return rv
 
 
 # options and arguments passed on command line
 cmdopts = []
 cmdargs = []
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/pdfpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/pdfpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseconfigurepanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconfigurepanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseconstraintspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseconstraintspanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phasenotebookpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phasenotebookpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phasepanelutils.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phasepanelutils.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/phaseresultspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/phaseresultspanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/plotpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/plotpanel.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,61 +28,63 @@
 class PlotPanel(wx.Panel, PDFPanel):
     def __init__(self, *args, **kwds):
         PDFPanel.__init__(self)
         # begin wxGlade: PlotPanel.__init__
         kwds["style"] = kwds.get("style", 0) | wx.TAB_TRAVERSAL
         wx.Panel.__init__(self, *args, **kwds)
         self.SetSize((456, 659))
+
+        sizer_1 = wx.BoxSizer(wx.VERTICAL)
+
+        sizer_3 = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, "X"), wx.HORIZONTAL)
+        sizer_1.Add(sizer_3, 0, wx.EXPAND, 0)
+
         self.xDataCombo = wx.ComboBox(self, wx.ID_ANY, choices=[], style=wx.CB_READONLY)
+        sizer_3.Add(self.xDataCombo, 1, wx.ALL, 5)
+
+        sizer_4 = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, "Y"), wx.HORIZONTAL)
+        sizer_1.Add(sizer_4, 1, wx.EXPAND, 0)
+
         self.yDataList = KeyEventsListCtrl(self, wx.ID_ANY, style=wx.BORDER_SUNKEN | wx.LC_NO_HEADER | wx.LC_REPORT)
+        sizer_4.Add(self.yDataList, 1, wx.ALL | wx.EXPAND, 5)
+
+        sizer_6 = wx.BoxSizer(wx.HORIZONTAL)
+        sizer_1.Add(sizer_6, 0, wx.EXPAND, 0)
+
         self.offsetLabel = wx.StaticText(self, wx.ID_ANY, "offset", style=wx.ALIGN_RIGHT)
+        sizer_6.Add(self.offsetLabel, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
+
         self.offsetTextCtrl = wx.TextCtrl(self, wx.ID_ANY, "-5", style=wx.TE_PROCESS_ENTER)
+        sizer_6.Add(self.offsetTextCtrl, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
+
         self.static_line_1 = wx.StaticLine(self, wx.ID_ANY)
+        sizer_1.Add(self.static_line_1, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)
+
+        sizer_2 = wx.BoxSizer(wx.HORIZONTAL)
+        sizer_1.Add(sizer_2, 0, wx.EXPAND, 0)
+
         self.plotButton = wx.Button(self, wx.ID_ANY, "Plot")
+        sizer_2.Add(self.plotButton, 0, wx.ALL, 5)
+
         self.resetButton = wx.Button(self, wx.ID_ANY, "Reset")
+        sizer_2.Add(self.resetButton, 0, wx.ALL, 5)
+
+        self.SetSizer(sizer_1)
 
-        self.__set_properties()
-        self.__do_layout()
+        self.Layout()
 
         self.Bind(wx.EVT_TEXT_ENTER, self.onEnter, self.offsetTextCtrl)
         self.Bind(wx.EVT_BUTTON, self.onPlot, self.plotButton)
         self.Bind(wx.EVT_BUTTON, self.onReset, self.resetButton)
         # end wxGlade
         self.Bind(wx.EVT_COMBOBOX, self._check, self.xDataCombo)
         self.Bind(wx.EVT_LIST_ITEM_SELECTED, self._check,  self.yDataList)
         self.Bind(wx.EVT_LIST_ITEM_DESELECTED, self._check,  self.yDataList)
         self.__customProperties()
 
-    def __set_properties(self):
-        # begin wxGlade: PlotPanel.__set_properties
-        self.SetSize((456, 659))
-        # end wxGlade
-
-    def __do_layout(self):
-        # begin wxGlade: PlotPanel.__do_layout
-        sizer_1 = wx.BoxSizer(wx.VERTICAL)
-        sizer_2 = wx.BoxSizer(wx.HORIZONTAL)
-        sizer_6 = wx.BoxSizer(wx.HORIZONTAL)
-        sizer_4 = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, "Y"), wx.HORIZONTAL)
-        sizer_3 = wx.StaticBoxSizer(wx.StaticBox(self, wx.ID_ANY, "X"), wx.HORIZONTAL)
-        sizer_3.Add(self.xDataCombo, 1, wx.ALL, 5)
-        sizer_1.Add(sizer_3, 0, wx.EXPAND, 0)
-        sizer_4.Add(self.yDataList, 1, wx.ALL | wx.EXPAND, 5)
-        sizer_1.Add(sizer_4, 1, wx.EXPAND, 0)
-        sizer_6.Add(self.offsetLabel, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
-        sizer_6.Add(self.offsetTextCtrl, 0, wx.ALIGN_CENTER_VERTICAL | wx.ALL, 5)
-        sizer_1.Add(sizer_6, 0, wx.EXPAND, 0)
-        sizer_1.Add(self.static_line_1, 0, wx.BOTTOM | wx.EXPAND | wx.TOP, 5)
-        sizer_2.Add(self.plotButton, 0, wx.ALL, 5)
-        sizer_2.Add(self.resetButton, 0, wx.ALL, 5)
-        sizer_1.Add(sizer_2, 0, wx.EXPAND, 0)
-        self.SetSizer(sizer_1)
-        self.Layout()
-        # end wxGlade
-
     # USER CONFIGURATION CODE #################################################
     def __customProperties(self):
         """Custom Properties go here."""
         self.yDataList.InsertColumn(0, "Y data")
         self.offsetTextCtrl.SetValidator(TextValidator(FLOAT_ONLY,allowNeg=True))
 
         # Define tooltips.
@@ -192,15 +194,16 @@
                 if name not in ref.getYNames(): ydata.remove(name)
 
         yvals = _represent(ydata)
 
         # Fill the List
         self.yDataList.DeleteAllItems()
         for val in yvals:
-            self.yDataList.InsertItem(sys.maxsize, str(val))
+            # self.yDataList.InsertItem(sys.maxsize, str(val)) #doesn't work for windows
+            self.yDataList.InsertItem(100000, str(val))
         self.yDataList.makeIDM()
         self.yDataList.initializeSorter()
         if yvals:
             self.yDataList.Select(0)
 
         #self.prevSelectionType = selectiontype
         self._check(None)
```

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/preferencespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/preferencespanel.py~`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/resultspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/resultspanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/rseriespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/rseriespanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/sgconstraindialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgconstraindialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/sgstructuredialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/sgstructuredialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/supercelldialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/supercelldialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/temperatureseriespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/temperatureseriespanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/tooltips.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/tooltips.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/welcomepanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/welcomepanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/windowperspective.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/windowperspective.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/autowidthlabelsgrid.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/autowidthlabelsgrid.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/listctrls.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/listctrls.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/paneldialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/paneldialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/textctrlutils.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/textctrlutils.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/validators.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/validators.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/gui/wxextensions/wx12.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/gui/wxextensions/wx12.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/__init__.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/debug.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/debug.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/run.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/run.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/rundeps.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/rundeps.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/showphasenotebookpanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/showphasenotebookpanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testaboutdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testaboutdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testcalculation.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testcalculation.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testconstraint.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testconstraint.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/300K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/300K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/550K.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/550K.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/CdSe_bulk_wur.stru` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/CdSe_bulk_wur.stru`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/LaMnO3.stru` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/LaMnO3.stru`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni.dat` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni.dat`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni.stru` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni.stru`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/Ni_2-8.chi.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/Ni_2-8.chi.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_00.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_00.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_20.gr` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_20.gr`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/lcmo_full.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/lcmo_full.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdata/ni.ddp` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdata/ni.ddp`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdatasetpanels.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdatasetpanels.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testdopingseriespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testdopingseriespanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testextendedplotframe.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testextendedplotframe.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testfitdataset.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testfitdataset.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testfitstructure.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testfitstructure.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testinsertrowsdialog.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testinsertrowsdialog.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testloadproject.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testloadproject.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testmainframe.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testmainframe.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testparameter.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testparameter.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testparameterspanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testparameterspanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfdataset.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfdataset.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfguicontrol.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfguicontrol.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testpdfstructure.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testpdfstructure.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testphaseconfigurepanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testphaseconfigurepanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/teststructureviewer.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/teststructureviewer.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testtemperatureseriespanel.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testtemperatureseriespanel.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tests/testutils.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/tui.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/tui.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/utils.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/utils.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy/pdfgui/version.py` & `diffpy.pdfgui-2.0.0/src/diffpy/pdfgui/version.py`

 * *Files identical despite different names*

### Comparing `diffpy.pdfgui-1.4.2/src/diffpy.pdfgui.egg-info/PKG-INFO` & `diffpy.pdfgui-2.0.0/src/diffpy.pdfgui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffpy.pdfgui
-Version: 1.4.2
+Version: 2.0.0
 Summary: GUI for PDF simulation and structure refinement.
 Home-page: https://github.com/diffpy/diffpy.pdfgui
 Author: Simon J.L. Billinge
 Author-email: sb2896@columbia.edu
 Maintainer: Pavol Juhas
 Maintainer-email: pavol.juhas@gmail.com
 License: BSD
@@ -47,41 +47,31 @@
 help menu and follow the tutorial instructions.  A detailed description
 is available in the doc/Farrow-jpcm-2007.pdf paper.
 
 
 REQUIREMENTS
 ------------------------------------------------------------------------
 
-PDFgui requires Python 3.7 or later or 2.7 and several third-party
+PDFgui requires Python 3.7, 3.8, 3.9, or 2.7 and several third-party
 libraries that are used by PDFgui and its components.
 
 * setuptools   - tools for installing Python packages
 * wxpython     - graphical user interface toolkit for Python
-* NumPy        - library for scientific computing with Python
+* numpy        - library for scientific computing with Python
 * matplotlib   - Python 2D plotting library
 * diffpy.pdffit2 - computational engine for PDFgui,
   https://github.com/diffpy/diffpy.pdffit2
 * diffpy.structure - simple storage and manipulation of atomic
   structures, https://github.com/diffpy/diffpy.structure
 * diffpy.utils - shared helper utilities for wx GUI,
   https://github.com/diffpy/diffpy.utils
 
 We recommend to use `Anaconda Python <https://www.anaconda.com/download>`_
 which allows to conveniently install PDFgui and all its software
-dependencies with a single command.  For other Python distributions
-it is necessary to install the required software separately.  As an
-example, on Ubuntu Linux some of the required software can be
-installed using ::
-
-   sudo apt-get install \
-      python-setuptools python-wxtools python-numpy \
-      python-matplotlib
-
-To install the remaining packages see the installation instructions
-at their respective web pages.
+dependencies with a single command.
 
 Please note that the Python3 PDFgui will read .ddp3 files. It is also
 possible for it to read .ddp files that were saved by the Python2 PDFgui
 but it will sometimes fail to read these. We are working on a solution
 that will be available in a future version.
 
 INSTALLATION
@@ -95,18 +85,15 @@
 PDFgui can be then started from a terminal ("Anaconda Prompt" on
 Windows) by executing the "pdfgui" program.  An alternative
 method on Windows is to start PDFgui through the DiffPy start menu.
 
 If you don't use Anaconda or prefer to install from sources, make
 sure the required software is all in place ::
 
-   pip install wxpython==4.0.7
-   conda install matplotlib
-   conda install -c conda-forge diffpy.utils
-   conda install -c conda-forge install diffpy.pdffit2
+   conda install -c conda-forge diffpy.utils diffpy.pdffit2 matplotlib wxpython
 
 Then you are ready to install diffpy.pdfgui from source codes::
 
    python setup.py install
 
 By default the files are installed to standard system directories,
 which may require the use of ``sudo`` for write privileges.  If
@@ -127,21 +114,33 @@
 (`conda install python.app`), then run as follows ::
 
    python.app diffpy.pdfgui/src/diffpy/pdfgui/application/pdfgui.py
 
 With Anaconda PDFgui can be later upgraded to the latest released
 version using ::
 
-   conda update diffpy.pdfgui
+   conda update -c conda-forge diffpy.pdfgui
 
 With other Python distributions the program can be upgraded to
 the latest version as follows ::
 
    easy_install --upgrade diffpy.pdfgui
 
+If you would like to use other Python distributions except Anaconda,
+it is necessary to install the required software separately. As an
+example, on Ubuntu Linux some of the required software can be
+installed using ::
+
+   sudo apt-get install \
+      python-setuptools python-wxtools python-numpy \
+      python-matplotlib
+
+To install the remaining packages see the installation instructions
+at their respective web pages.
+
 Other software
 ````````````````````````````````````````````````````````````````````````
 
 PDFgui can use an external structure viewer for displaying analyzed
 structures.  We have tested with several structure viewers such as
 
 * AtomEye, http://li.mit.edu/A/Graphics/A/
```

