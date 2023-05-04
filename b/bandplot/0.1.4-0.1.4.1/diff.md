# Comparing `tmp/bandplot-0.1.4-py3-none-any.whl.zip` & `tmp/bandplot-0.1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9430 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       24 b- defN 23-May-03 20:15 bandplot/__init__.py
--rw-rw-r--  2.0 unx    28110 b- defN 23-May-03 20:15 bandplot/plots.py
--rw-rw-r--  2.0 unx     5809 b- defN 23-May-03 20:15 bandplot/readdata.py
--rw-rw-r--  2.0 unx    15171 b- defN 23-May-03 20:15 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2899 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      701 b- defN 23-May-03 20:16 bandplot-0.1.4.dist-info/RECORD
-9 files, 52901 bytes uncompressed, 8226 bytes compressed:  84.5%
+Zip file size: 9590 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       26 b- defN 23-May-04 03:00 bandplot/__init__.py
+-rw-rw-r--  2.0 unx    28110 b- defN 23-May-04 03:00 bandplot/plots.py
+-rw-rw-r--  2.0 unx     6111 b- defN 23-May-04 03:00 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    15554 b- defN 23-May-04 03:00 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2901 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 23-May-04 03:00 bandplot-0.1.4.1.dist-info/RECORD
+9 files, 53600 bytes uncompressed, 8366 bytes compressed:  84.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.4.dist-info/METADATA
+Filename: bandplot-0.1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.4.dist-info/WHEEL
+Filename: bandplot-0.1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.4.dist-info/entry_points.txt
+Filename: bandplot-0.1.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.4.dist-info/top_level.txt
+Filename: bandplot-0.1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.4.dist-info/RECORD
+Filename: bandplot-0.1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.4"
+__version__ = "0.1.4.1"
```

## bandplot/readdata.py

```diff
@@ -5,14 +5,22 @@
     with open(KLABELS, "r") as main_file:
         lines = main_file.readlines()[1:]
     LABELS = [line.split() for line in lines if len(line.split()) == 2]
     ticks  = [float(label[1]) for label in LABELS]
     labels = [label[0] for label in LABELS]
     return ticks, labels
 
+def bandset(bandconf):
+    with open(bandconf, "r") as main_file:
+        lines = main_file.readlines()
+    LABELS = [line for line in lines if line.strip().startswith('BAND_LABELS')]
+    if LABELS:
+        LABELS = LABELS[-1].split("=")[-1].replace('\\','').upper().split()
+    return LABELS
+
 def dos(DOS):
     ARR = []
     ELE = []
     s_elements = []
     for pdos in DOS:
         with open(pdos, "r") as main_file:
             lines = main_file.readlines()
```

## bandplot/wrapper.py

```diff
@@ -35,15 +35,15 @@
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
     parser.add_argument('-i', "--input",      type=str,             help="plot figure from .dat file, default: BAND.dat", default="BAND.dat")
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
-    parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS", default="KLABELS")
+    parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-r', "--wratios",    type=float,           help='width ratio for DOS subplot')
@@ -175,14 +175,15 @@
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
     parser.add_argument('-i', "--input",      type=str,             help="plot figure from .dat file, default: BAND.dat", default="BAND.dat")
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
+    parser.add_argument('-j', "--bandconf",   type=str,             help="filename of band setting file, default: band.conf", default="band.conf")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-p', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
@@ -248,14 +249,19 @@
     if width_ratios >= 1 or width_ratios <= 0:
         width_ratios = 0.5
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
                     color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
     if os.path.exists(args.input):
         arr, fre, ticks = readdata.pbands(args.input)
+        klabels = []
+        if os.path.exists(args.bandconf):
+            klabels = readdata.bandset(args.bandconf)
+        if len(labels) == 0:
+            labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
         if len(ticks) > len(labels):
             labels = labels + [''] * (len(ticks) - len(labels))
         elif len(ticks) < len(labels):
             labels = labels[:len(ticks)]
         if args.dos is None:
             if args.broken is None:
                 plots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
```

## Comparing `bandplot-0.1.4.dist-info/METADATA` & `bandplot-0.1.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
```

## Comparing `bandplot-0.1.4.dist-info/RECORD` & `bandplot-0.1.4.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-bandplot/__init__.py,sha256=DkDHsaNkZtxTqAYgO8ZitcZnQvVk6hBU5j7RkfnE4OI,24
+bandplot/__init__.py,sha256=2YJzDUEgy4EdzNq-NeipKYBWNUNyf1I25QNJm2IQ2cU,26
 bandplot/plots.py,sha256=KiipL3uohkgg9L0CJKftx5NllMwmtl5UKxrv4_fYnRM,28110
-bandplot/readdata.py,sha256=perJzlojUpEHArzro_gM-oh1wMRuNyAOOC1z1cvORPE,5809
-bandplot/wrapper.py,sha256=TcF8xvPRpjtFDGSiFXKT6SE0E4mA7GRZhq3FCvv2fc8,15171
-bandplot-0.1.4.dist-info/METADATA,sha256=_w1BIgKKGMa5jcSXY4GOgEyF-KRQ-HnY-STc6hdvkn4,2899
-bandplot-0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bandplot-0.1.4.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
-bandplot-0.1.4.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
-bandplot-0.1.4.dist-info/RECORD,,
+bandplot/readdata.py,sha256=sW5TZ9oGXoWKlHkV-A8uTM2lQLzl8f1iia2GosxYGzs,6111
+bandplot/wrapper.py,sha256=FA7iKfBXw-VryiQQTWfCpllg7-YC8halNOYbVjT812k,15554
+bandplot-0.1.4.1.dist-info/METADATA,sha256=A7szgMArFUpypnCD0X4CZyNbxXacgpBGhPrB3h8swxA,2901
+bandplot-0.1.4.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bandplot-0.1.4.1.dist-info/entry_points.txt,sha256=1iTM_knGcHWOG7xxwvloJo_nbjS8WKTPOHP_HIKQr7k,86
+bandplot-0.1.4.1.dist-info/top_level.txt,sha256=SMQlf9lMS_nlhnQduityQVcU231XkEEvM7Z0n9gB0JE,9
+bandplot-0.1.4.1.dist-info/RECORD,,
```

