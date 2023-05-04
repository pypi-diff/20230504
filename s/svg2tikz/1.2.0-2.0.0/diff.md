# Comparing `tmp/svg2tikz-1.2.0.tar.gz` & `tmp/svg2tikz-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg2tikz-1.2.0.tar", max compression
+gzip compressed data, was "svg2tikz-2.0.0.tar", max compression
```

## Comparing `svg2tikz-1.2.0.tar` & `svg2tikz-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,9 @@
--rw-r--r--   0        0        0      716 2023-01-14 23:09:49.196517 svg2tikz-1.2.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-02-16 21:32:18.842017 svg2tikz-1.2.0/README.md
--rw-r--r--   0        0        0      535 2023-02-16 21:32:18.842017 svg2tikz-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0       69 2023-01-14 23:09:49.200518 svg2tikz-1.2.0/svg2tikz/__init__.py
--rwxr-xr-x   0        0        0        0 2023-01-14 23:09:49.200518 svg2tikz-1.2.0/svg2tikz/extensions/__init__.py
--rw-r--r--   0        0        0    60464 2023-02-16 21:32:18.842017 svg2tikz-1.2.0/svg2tikz/extensions/tikz_export.py
--rw-r--r--   0        0        0     2281 2023-01-14 23:18:52.476540 svg2tikz-1.2.0/svg2tikz/extensions/tikz_export_effect.inx
--rw-r--r--   0        0        0     2202 2023-01-14 23:18:52.476540 svg2tikz-1.2.0/svg2tikz/extensions/tikz_export_output.inx
--rw-r--r--   0        0        0      749 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/__init__.py
--rw-r--r--   0        0        0    12798 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/base.py
--rw-r--r--   0        0        0    13862 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/bezier.py
--rw-r--r--   0        0        0    15545 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/colors.py
--rw-r--r--   0        0        0     7564 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/command.py
--rw-r--r--   0        0        0    14766 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/deprecated.py
--rw-r--r--   0        0        0      965 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/__init__.py
--rw-r--r--   0        0        0    19787 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_base.py
--rw-r--r--   0        0        0     9176 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_filters.py
--rw-r--r--   0        0        0     3439 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_groups.py
--rw-r--r--   0        0        0      972 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_image.py
--rw-r--r--   0        0        0     4935 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_meta.py
--rw-r--r--   0        0        0     8021 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_polygons.py
--rw-r--r--   0        0        0     5943 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_selected.py
--rw-r--r--   0        0        0     7897 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_svg.py
--rw-r--r--   0        0        0     5190 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_text.py
--rw-r--r--   0        0        0     2365 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/elements/_use.py
--rw-r--r--   0        0        0    13206 2023-01-14 23:18:52.480540 svg2tikz-1.2.0/svg2tikz/inkex/extensions.py
--rw-r--r--   0        0        0     1817 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/inkscape_env.py
--rw-r--r--   0        0        0     8016 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/inx.py
--rw-r--r--   0        0        0     2526 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/localization.py
--rw-r--r--   0        0        0    52479 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/paths.py
--rw-r--r--   0        0        0     3664 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/ports.py
--rw-r--r--   0        0        0    14243 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/styles.py
--rw-r--r--   0        0        0    15961 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/__init__.py
--rw-r--r--   0        0        0      261 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/decorators.py
--rw-r--r--   0        0        0     4668 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/filters.py
--rw-r--r--   0        0        0     3719 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/inx.py
--rw-r--r--   0        0        0    17135 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/mock.py
--rw-r--r--   0        0        0     1665 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/svg.py
--rw-r--r--   0        0        0      825 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/word.py
--rw-r--r--   0        0        0     4062 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tester/xmldiff.py
--rw-r--r--   0        0        0    38109 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/transforms.py
--rw-r--r--   0        0        0     3213 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/turtle.py
--rw-r--r--   0        0        0     2677 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/tween.py
--rw-r--r--   0        0        0     4052 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/units.py
--rw-r--r--   0        0        0    10513 2023-01-14 23:18:52.484540 svg2tikz-1.2.0/svg2tikz/inkex/utils.py
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 svg2tikz-1.2.0/setup.py
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 svg2tikz-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      716 2023-01-12 15:48:31.564669 svg2tikz-2.0.0/LICENSE
+-rw-r--r--   0        0        0      959 2023-04-16 09:59:38.443314 svg2tikz-2.0.0/README.md
+-rw-r--r--   0        0        0      622 2023-05-04 20:55:55.730797 svg2tikz-2.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-03-07 07:24:39.159976 svg2tikz-2.0.0/svg2tikz/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-01-12 15:48:31.564669 svg2tikz-2.0.0/svg2tikz/extensions/__init__.py
+-rw-r--r--   0        0        0    63530 2023-05-04 20:56:35.394203 svg2tikz-2.0.0/svg2tikz/extensions/tikz_export.py
+-rw-r--r--   0        0        0     4757 2023-05-02 14:51:46.206058 svg2tikz-2.0.0/svg2tikz/extensions/tikz_export_effect.inx
+-rw-r--r--   0        0        0     4741 2023-05-02 14:51:46.206058 svg2tikz-2.0.0/svg2tikz/extensions/tikz_export_output.inx
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 svg2tikz-2.0.0/PKG-INFO
```

### Comparing `svg2tikz-1.2.0/LICENSE` & `svg2tikz-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2tikz-1.2.0/svg2tikz/extensions/tikz_export.py` & `svg2tikz-2.0.0/svg2tikz/extensions/tikz_export.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 import platform
 
-__version__ = '1.2.0'
-__author__ = 'Kjell Magne Fauske'
+__version__ = "2.0.0"
+__author__ = "Devillez Louis, Kjell Magne Fauske"
+__maintainer__ = "Deville Louis"
+__email__ = "louis.devillez@gmail.com"
 
 # Todo:
 # Basic functionality:
 
 # Stroke properties
 # - markers (map from Inkscape to TikZ arrow styles. No 1:1 mapping)
 # Fill properties
@@ -50,39 +52,54 @@
 # - Better output code formatting!
 # - Add a + prefix to coordinates to speed up pgf parsing
 # - Transformations
 #   - default property values.The initial fill property is set to 'black'.
 #     This is currently not handled.
 # - ConTeXt template support.
 
-
 import sys
 
 from textwrap import wrap
 from copy import deepcopy
 import codecs
 import io
 import copy
 import os
 from subprocess import Popen, PIPE
-from lxml import etree
-
-import inkex
 
 import re
 import math
 
 from math import sin, cos, atan2
+from math import pi as mpi
+
 import logging
 
+from urllib.request import urlopen
+
+from dataclasses import dataclass
+import ctypes
+import inkex
+from lxml import etree
+
+
 #### Utility functions and classes
 
-SPECIAL_TEX_CHARS = ['$', '\\', '%', '_', '#', '{', r'}', '^', '&']
-SPECIAL_TEX_CHARS_REPLACE = [r'\$', r'$\backslash$', r'\%', r'\_', r'\#',
-                             r'\{', r'\}', r'\^{}', r'\&']
+SPECIAL_TEX_CHARS = ["$", "\\", "%", "_", "#", "{", r"}", "^", "&"]
+SPECIAL_TEX_CHARS_REPLACE = [
+    r"\$",
+    r"$\backslash$",
+    r"\%",
+    r"\_",
+    r"\#",
+    r"\{",
+    r"\}",
+    r"\^{}",
+    r"\&",
+]
 _tex_charmap = dict(list(zip(SPECIAL_TEX_CHARS, SPECIAL_TEX_CHARS_REPLACE)))
 
 
 def escape_texchars(input_string):
     r"""Escape the special LaTeX-chars %{}_^
 
     Examples:
@@ -91,951 +108,1108 @@
     '10\\%'
     >>> escape_texchars('%{}_^\\$')
     '\\%\\{\\}\\_\\^{}$\\backslash$\\$'
     """
     return "".join([_tex_charmap.get(c, c) for c in input_string])
 
 
-class Bunch(object):
-    def __init__(self, **kwds):
-        self.__dict__.update(kwds)
-
-    def __str__(self):
-        return self.__dict__.__str__()
-
-    def __repr__(self):
-        return self.__dict__.__repr__()
-
-
 def copy_to_clipboard(text):
     """Copy text to the clipboard
 
     Returns True if successful. False otherwise.
     """
 
-    import sys
-    if sys.version < '3':
-        text_type = unicode
-    else:
-        text_type = str
+    text_type = str
 
     def _do_windows_clipboard(text):
         # from http://pylabeditor.svn.sourceforge.net/viewvc/pylabeditor/trunk/src/shells.py?revision=82&view=markup
-        import ctypes
 
-        CF_UNICODETEXT = 13
-        GHND = 66
+        cf_unicode_text = 13
+        ghnd = 66
 
         ctypes.windll.kernel32.GlobalAlloc.restype = ctypes.c_void_p
         ctypes.windll.kernel32.GlobalLock.restype = ctypes.c_void_p
 
-        text = text_type(text, 'utf8')
-        bufferSize = (len(text)+1)*2
-        hGlobalMem = ctypes.windll.kernel32.GlobalAlloc(ctypes.c_uint(GHND), ctypes.c_size_t(bufferSize))
-        lpGlobalMem = ctypes.windll.kernel32.GlobalLock(ctypes.c_void_p(hGlobalMem))
-        ctypes.cdll.msvcrt.memcpy( ctypes.c_void_p(lpGlobalMem), ctypes.c_wchar_p(text), ctypes.c_int(bufferSize))
-        ctypes.windll.kernel32.GlobalUnlock(ctypes.c_void_p(hGlobalMem))
+        text = text_type(text, "utf8")
+        buffer_size = (len(text) + 1) * 2
+        h_global_mem = ctypes.windll.kernel32.GlobalAlloc(
+            ctypes.c_uint(ghnd), ctypes.c_size_t(buffer_size)
+        )
+        lp_global_mem = ctypes.windll.kernel32.GlobalLock(ctypes.c_void_p(h_global_mem))
+        ctypes.cdll.msvcrt.memcpy(
+            ctypes.c_void_p(lp_global_mem),
+            ctypes.c_wchar_p(text),
+            ctypes.c_int(buffer_size),
+        )
+        ctypes.windll.kernel32.GlobalUnlock(ctypes.c_void_p(h_global_mem))
         if ctypes.windll.user32.OpenClipboard(0):
-           ctypes.windll.user32.EmptyClipboard()
-           ctypes.windll.user32.SetClipboardData( ctypes.c_int(CF_UNICODETEXT), ctypes.c_void_p(hGlobalMem) )
-           ctypes.windll.user32.CloseClipboard()
-           return True
-        else:
-           return False
+            ctypes.windll.user32.EmptyClipboard()
+            ctypes.windll.user32.SetClipboardData(
+                ctypes.c_int(cf_unicode_text), ctypes.c_void_p(h_global_mem)
+            )
+            ctypes.windll.user32.CloseClipboard()
+            return True
+        return False
 
     def _call_command(command, text):
         # see https://bugs.launchpad.net/ubuntu/+source/inkscape/+bug/781397/comments/2
         try:
             devnull = os.open(os.devnull, os.O_RDWR)
-            p = Popen(command, stdin=PIPE, stdout=devnull, stderr=devnull)
-            out, err = p.communicate(text)
-            if not p.returncode:
-                return True
+            with Popen(command, stdin=PIPE, stdout=devnull, stderr=devnull) as proc:
+                proc.communicate(text)
+                if not proc.returncode:
+                    return True
 
         except OSError:
             pass
         return False
 
     def _do_linux_clipboard(text):
         # try xclip first, then xsel
-        xclip_cmd = ['xclip', '-selection', 'clipboard']
+        xclip_cmd = ["xclip", "-selection", "clipboard"]
         success = _call_command(xclip_cmd, text)
         if success:
             return True
 
-        xsel_cmd = ['xsel']
+        xsel_cmd = ["xsel"]
         success = _call_command(xsel_cmd, text)
         return success
 
     def _do_osx_clipboard(text):
-        pbcopy_cmd = ['pbcopy']
+        pbcopy_cmd = ["pbcopy"]
         return _call_command(pbcopy_cmd, text)
         # try os /linux
 
-    if os.name == 'nt' or platform.system() == 'Windows':
+    if os.name == "nt" or platform.system() == "Windows":
         return _do_windows_clipboard(text)
-    elif os.name == 'mac' or platform.system() == 'Darwin':
+    if os.name == "mac" or platform.system() == "Darwin":
         return _do_osx_clipboard(text)
-    else:
-        return _do_linux_clipboard(text)
+    return _do_linux_clipboard(text)
 
 
-def nsplit(seq, n=2):
+def nsplit(seq, n_split=2):
     """Split a sequence into pieces of length n
 
     If the length of the sequence isn't a multiple of n, the rest is discarded.
     Note that nsplit will strings into individual characters.
 
     Examples:
     >>> nsplit('aabbcc')
     [('a', 'a'), ('b', 'b'), ('c', 'c')]
-    >>> nsplit('aabbcc',n=3)
+    >>> nsplit('aabbcc',n_split=3)
     [('a', 'a', 'b'), ('b', 'c', 'c')]
 
     # Note that cc is discarded
-    >>> nsplit('aabbcc',n=4)
+    >>> nsplit('aabbcc',n_split=4)
     [('a', 'a', 'b', 'b')]
     """
-    return [xy for xy in zip(*[iter(seq)] * n)]
+    return list(zip(*[iter(seq)] * n_split))
 
 
-def chunks(s, cl):
-    """Split a string or sequence into pieces of length cl and return an iterator
-    """
-    for i in range(0, len(s), cl):
-        yield s[i:i + cl]
+def chunks(string, c_l):
+    """Split a string or sequence into pieces of length c_l and return an iterator"""
+    for i in range(0, len(string), c_l):
+        yield string[i : i + c_l]
 
 
 # Adapted from Mark Pilgrim's Dive into Python book
 # http://diveintopython.org/scripts_and_streams/index.html#kgp.openanything
 def open_anything(source):
-    # try to open with urllib (if source is http, ftp, or file URL)
-    try:
-        from urllib import urlopen
-        to_unicode = unicode
-    except ImportError:  # Python3
-        from urllib.request import urlopen
-        import urllib.error
-        to_unicode = str
+    """doc to complete"""
 
     try:
         return urlopen(source)
     except (IOError, OSError, ValueError):
         pass
-
         # try to open with native open function (if source is pathname)
     try:
-        return open(source)
+        return open(source, encoding="utf8")
     except (IOError, OSError):
         pass
 
-        # treat source as string
-    import io
+    return io.StringIO(str(source))
 
-    return io.StringIO(to_unicode(source))
 
-
-def _ns(element_name, name_space='svg'):
+def _ns(element_name, name_space="svg"):
     return inkex.addNS(element_name, name_space)
 
 
+@dataclass
+class Point:
+    """Docstring"""
+
+    # pylint: disable=invalid-name
+    x: float
+    y: float
+
+
 #### Output configuration section
 
 TEXT_INDENT = "  "
 
 CROP_TEMPLATE = r"""
 \usepackage[active,tightpage]{preview}
 \PreviewEnvironment{tikzpicture}
 """
 
 # Templates
-STANDALONE_TEMPLATE = r"""
+STANDALONE_TEMPLATE = (
+    r"""
 \documentclass{article}
 \usepackage[utf8]{inputenc}
 \usepackage{tikz}
 %(cropcode)s
 \begin{document}
 %(colorcode)s
 %(gradientcode)s
 \def \globalscale {%(scale)f}
-\begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=\globalscale, xscale=\globalscale, inner sep=0pt, outer sep=0pt%(extraoptions)s]
+\begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=%(ysign)s\globalscale,"""
+    r"""xscale=\globalscale, inner sep=0pt, outer sep=0pt%(extraoptions)s]
 %(pathcode)s
 \end{tikzpicture}
 \end{document}
 """
+)
 
-FIG_TEMPLATE = r"""
+FIG_TEMPLATE = (
+    r"""
 %(colorcode)s
 %(gradientcode)s
 \def \globalscale {%(scale)f}
-\begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=\globalscale, xscale=\globalscale, inner sep=0pt, outer sep=0pt%(extraoptions)s]
+\begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=%(ysign)s\globalscale,"""
+    r"""xscale=\globalscale, inner sep=0pt, outer sep=0pt%(extraoptions)s]
 %(pathcode)s
 \end{tikzpicture}
 """
+)
 
-SCALE = 'scale'
-DICT = 'dict'
-DIMENSION = 'dimension'
-FACTOR = 'factor'  # >= 1
+SCALE = "scale"
+DICT = "dict"
+DIMENSION = "dimension"
+FACTOR = "factor"  # >= 1
 
 # Map Inkscape/SVG stroke and fill properties to corresponding TikZ options.
 # Format:
 #   'svg_name' : ('tikz_name', value_type, data)
 PROPERTIES_MAP = {
-    'opacity': ('opacity', SCALE, ''),
+    "opacity": ("opacity", SCALE, ""),
     # filling
-    'fill-opacity': ('fill opacity', SCALE, ''),
-    'fill-rule': ('', DICT,
-                  dict(nonzero='nonzero rule', evenodd='even odd rule')),
+    "fill-opacity": ("fill opacity", SCALE, ""),
+    "fill-rule": ("", DICT, {"nonzero": "nonzero rule", "evenodd": "even odd rule"}),
     # stroke
-    'stroke-opacity': ('draw opacity', SCALE, ''),
-    'stroke-linecap': ('line cap', DICT,
-                       dict(butt='butt', round='round', square='rect')),
-    'stroke-linejoin': ('line join', DICT,
-                        dict(miter='miter', round='round', bevel='bevel')),
-    'stroke-width': ('line width', DIMENSION, ''),
-    'stroke-miterlimit': ('miter limit', FACTOR, ''),
-    'stroke-dashoffset': ('dash phase', DIMENSION, '0')
+    "stroke-opacity": ("draw opacity", SCALE, ""),
+    "stroke-linecap": (
+        "line cap",
+        DICT,
+        {"butt": "butt", "round": "round", "rect": "rect"},
+    ),
+    "stroke-linejoin": (
+        "line join",
+        DICT,
+        {
+            "miter": "miter",
+            "round": "round",
+            "bevel": "bevel",
+        },
+    ),
+    "stroke-width": ("line width", DIMENSION, ""),
+    "stroke-miterlimit": ("miter limit", FACTOR, ""),
+    "stroke-dashoffset": ("dash phase", DIMENSION, "0"),
 }
 
 # default values according to the SVG spec.
 DEFAULT_PAINTING_VALUES = {
     # fill
-    'fill': 'black',
-    'fill-rule': 'nonzero',
-    'fill-opacity': 1,
+    "fill": "black",
+    "fill-rule": "nonzero",
+    "fill-opacity": 1,
     # stroke
-    'stroke': 'none',
-    'stroke-width': 1,
-    'stroke-linecap': 'butt',
-    'stroke-linejoin': 'miter',
-    'stroke-miterlimit': 4,
-    'stroke-dasharray': 'none',
-    'stroke-dashoffset': 0,
-    'stroke-opacity': 1,
+    "stroke": "none",
+    "stroke-width": 1,
+    "stroke-linecap": "butt",
+    "stroke-linejoin": "miter",
+    "stroke-miterlimit": 4,
+    "stroke-dasharray": "none",
+    "stroke-dashoffset": 0,
+    "stroke-opacity": 1,
 }
 
-STROKE_PROPERTIES = set([
-    'stroke', 'stroke-width', 'stroke-linecap',
-    'stroke-linejoin', 'stroke-miterlimit',
-    'stroke-dasharray', 'stroke-dashoffset',
-    'stroke-opacity',
-])
-
-FILL_PROPERTIES = set([
-    'fill', 'fill-rule', 'fill-opacity',
-])
-
-
-# The calc_arc function is based on the calc_arc function in the
-# paths_svg2obj.py script bundled with Blender 3D
-# Copyright (c) jm soler juillet/novembre 2004-april 2007,
-def calc_arc(cpx, cpy, rx, ry, ang, fa, fs, x, y):
+STROKE_PROPERTIES = set(
+    [
+        "stroke",
+        "stroke-width",
+        "stroke-linecap",
+        "stroke-linejoin",
+        "stroke-miterlimit",
+        "stroke-dasharray",
+        "stroke-dashoffset",
+        "stroke-opacity",
+    ]
+)
+
+FILL_PROPERTIES = set(
+    [
+        "fill",
+        "fill-rule",
+        "fill-opacity",
+    ]
+)
+
+
+def calc_arc(cp: Point, r_i: Point, ang, fa, fs, pos: Point):
     """
     Calc arc paths
+
+    It computes the start and end angle for a non rotated ellipse
+
+    cp: initial control point
+    r_i: x and y radius
+    ang: x-axis-rotation
+    fa: sweep flag
+    fs: large sweep flag
+    pos: final control point
+
+    The calc_arc function is based on the calc_arc function in the
+    paths_svg2obj.py script bundled with Blender 3D
+    Copyright (c) jm soler juillet/novembre 2004-april 2007,
+    Resource: https://developer.mozilla.org/fr/docs/Web/SVG/Tutorial/Paths#elliptical_arc (in french)
     """
-    PI = math.pi
     ang = math.radians(ang)
-    rx = abs(rx)
-    ry = abs(ry)
-    px = abs((cos(ang) * (cpx - x) + sin(ang) * (cpy - y)) * 0.5) ** 2.0
-    py = abs((cos(ang) * (cpy - y) - sin(ang) * (cpx - x)) * 0.5) ** 2.0
-    rpx = rpy = 0.0
-    if abs(rx) > 0.0:
-        rpx = px / (rx ** 2.0)
-    if abs(ry) > 0.0:
-        rpy = py / (ry ** 2.0)
-    pl = rpx + rpy
-    if pl > 1.0:
-        pl = pl ** 0.5
-        rx *= pl
-        ry *= pl
-    carx = sarx = cary = sary = 0.0
-    if abs(rx) > 0.0:
-        carx = cos(ang) / rx
-        sarx = sin(ang) / rx
-    if abs(ry) > 0.0:
-        cary = cos(ang) / ry
-        sary = sin(ang) / ry
-    x0 = carx * cpx + sarx * cpy
-    y0 = (-sary) * cpx + cary * cpy
-    x1 = carx * x + sarx * y
-    y1 = (-sary) * x + cary * y
-    d = (x1 - x0) * (x1 - x0) + (y1 - y0) * (y1 - y0)
-    if abs(d) > 0.0:
-        sq = 1.0 / d - 0.25
+
+    r = Point(abs(r_i.x), abs(r_i.y))
+    p_pos = Point(
+        abs((cos(ang) * (cp.x - pos.x) + sin(ang) * (cp.y - pos.y)) * 0.5) ** 2.0,
+        abs((cos(ang) * (cp.y - pos.y) - sin(ang) * (cp.x - pos.x)) * 0.5) ** 2.0,
+    )
+    rp = Point(
+        p_pos.x / (r.x**2.0) if abs(r.x) > 0.0 else 0.0,
+        p_pos.y / (r.y**2.0) if abs(r.y) > 0.0 else 0.0,
+    )
+
+    p_l = rp.x + rp.y
+    if p_l > 1.0:
+        p_l = p_l**0.5
+        r.x *= p_l
+        r.y *= p_l
+
+    car = Point(
+        cos(ang) / r.x if abs(r.x) > 0.0 else 0.0,
+        cos(ang) / r.y if abs(r.y) > 0.0 else 0.0,
+    )
+
+    sar = Point(
+        sin(ang) / r.x if abs(r.x) > 0.0 else 0.0,
+        sin(ang) / r.y if abs(r.y) > 0.0 else 0.0,
+    )
+
+    p0 = Point(car.x * cp.x + sar.x * cp.y, (-sar.y) * cp.x + car.y * cp.y)
+    p1 = Point(car.x * pos.x + sar.x * pos.y, (-sar.y) * pos.x + car.y * pos.y)
+
+    hyp = (p1.x - p0.x) ** 2 + (p1.y - p0.y) ** 2
+
+    if abs(hyp) > 0.0:
+        s_q = 1.0 / hyp - 0.25
     else:
-        sq = -0.25
-    if sq < 0.0:
-        sq = 0.0
-    sf = sq ** 0.5
+        s_q = -0.25
+
+    s_f = max(0.0, s_q) ** 0.5
     if fs == fa:
-        sf = -sf
-    xc = 0.5 * (x0 + x1) - sf * (y1 - y0)
-    yc = 0.5 * (y0 + y1) + sf * (x1 - x0)
-    ang_0 = atan2(y0 - yc, x0 - xc)
-    ang_1 = atan2(y1 - yc, x1 - xc)
+        s_f *= -1
+    c = Point(
+        0.5 * (p0.x + p1.x) - s_f * (p1.y - p0.y),
+        0.5 * (p0.y + p1.y) + s_f * (p1.x - p0.x),
+    )
+    ang_0 = atan2(p0.y - c.y, p0.x - c.x)
+    ang_1 = atan2(p1.y - c.y, p1.x - c.x)
     ang_arc = ang_1 - ang_0
     if ang_arc < 0.0 and fs == 1:
-        ang_arc += 2.0 * PI
+        ang_arc += 2.0 * mpi
     elif ang_arc > 0.0 and fs == 0:
-        ang_arc -= 2.0 * PI
+        ang_arc -= 2.0 * mpi
 
     ang0 = math.degrees(ang_0)
     ang1 = math.degrees(ang_1)
 
     if ang_arc > 0:
         if ang_0 < ang_1:
             pass
         else:
             ang0 -= 360
     else:
         if ang_0 < ang_1:
             ang1 -= 360
 
-    return ang0, ang1, rx, ry
+    return ang0, ang1, r
 
 
 def parse_transform(transform):
     """Parse a transformation attribute and return a list of transformations"""
     # Based on the code in parseTransform in the simpletransform.py module.
     # Copyright (C) 2006 Jean-Francois Barraud
     # Reimplemented here due to several bugs in the version shipped with
     # Inkscape 0.46
+    # TODO could we reuse the one here from inkex ?
+    # If not we should correct it to be in line with pylint
+    # pylint: disable=too-many-branches
 
     if not transform:
         return []
     stripped_transform = transform.strip()
-    result = re.match("(translate|scale|rotate|skewX|skewY|matrix)\s*\(([^)]*)\)\s*,?", stripped_transform)
+    result = re.match(
+        r"(translate|scale|rotate|skewX|skewY|matrix)\s*\(([^)]*)\)\s*,?",
+        stripped_transform,
+    )
     if result is None:
         raise SyntaxError("Invalid transformation " + transform)
 
     transforms = []
     # -- translate --
     if result.group(1) == "translate":
-        args = result.group(2).replace(',', ' ').split()
-        dx = float(args[0])
+        args = result.group(2).replace(",", " ").split()
+        d_x = float(args[0])
         if len(args) == 1:
-            dy = 0.0
+            d_y = 0.0
         else:
-            dy = float(args[1])
-        matrix = [[1, 0, dx], [0, 1, dy]]
-        transforms.append(['translate', (dx, dy)])
-        # -- scale --
+            d_y = float(args[1])
+        # matrix = [[1, 0, d_x], [0, 1, d_y]]
+        transforms.append(["translate", (d_x, d_y)])
+
+    # -- scale --
     if result.group(1) == "scale":
-        args = result.group(2).replace(',', ' ').split()
-        sx = float(args[0])
+        args = result.group(2).replace(",", " ").split()
+        s_x = float(args[0])
         if len(args) == 1:
-            sy = sx
+            s_y = s_x
         else:
-            sy = float(args[1])
-        matrix = [[sx, 0, 0], [0, sy, 0]]
-        transforms.append(['scale', (sx, sy)])
-        # -- rotate --
+            s_y = float(args[1])
+        # matrix = [[s_x, 0, 0], [0, s_y, 0]]
+        transforms.append(["scale", (s_x, s_y)])
+
+    # -- rotate --
     if result.group(1) == "rotate":
-        args = result.group(2).replace(',', ' ').split()
-        a = float(args[0])  # *math.pi/180
+        args = result.group(2).replace(",", " ").split()
+        ang = float(args[0])  # *math.pi/180
         if len(args) == 1:
-            cx, cy = (0.0, 0.0)
+            c_x, c_y = (0.0, 0.0)
         else:
-            cx, cy = list(map(float, args[1:]))
-        matrix = [[math.cos(a), -math.sin(a), cx], [math.sin(a), math.cos(a), cy]]
-        transforms.append(['rotate', (a, cx, cy)])
+            c_x, c_y = list(map(float, args[1:]))
+        # matrix = [[math.cos(ang), -math.sin(ang), c_x],
+        #           [math.sin(ang), math.cos(ang), c_y]]
+        transforms.append(["rotate", (ang, c_x, c_y)])
         # -- skewX --
     if result.group(1) == "skewX":
-        a = float(result.group(2))  # "*math.pi/180
-        matrix = [[1, math.tan(a), 0], [0, 1, 0]]
-        transforms.append(['skewX', (a,)])
+        ang = float(result.group(2))  # "*math.pi/180
+        # matrix = [[1, math.tan(ang), 0], [0, 1, 0]]
+        transforms.append(["skewX", (ang,)])
         # -- skewY --
     if result.group(1) == "skewY":
-        a = float(result.group(2))  # *math.pi/180
-        matrix = [[1, 0, 0], [math.tan(a), 1, 0]]
-        transforms.append(['skewY', (a,)])
+        ang = float(result.group(2))  # *math.pi/180
+        # matrix = [[1, 0, 0], [math.tan(ang), 1, 0]]
+        transforms.append(["skewY", (ang,)])
         # -- matrix --
     if result.group(1) == "matrix":
         # a11,a21,a12,a22,v1,v2=result.group(2).replace(' ',',').split(",")
-        matrix_params = tuple(map(float, result.group(2).replace(',', ' ').split()))
-        a11, a21, a12, a22, v1, v2 = matrix_params
-        matrix = [[a11, a12, v1], [a21, a22, v2]]
-        transforms.append(['matrix', matrix_params])
+        matrix_params = tuple(map(float, result.group(2).replace(",", " ").split()))
+        # a11, a21, a12, a22, v_1, v_2 = matrix_params
+        # matrix = [[a11, a12, v_1], [a21, a22, v_2]]
+        transforms.append(["matrix", matrix_params])
 
     if result.end() < len(stripped_transform):
-        return transforms + parse_transform(stripped_transform[result.end():])
-    else:
-        return transforms
+        return transforms + parse_transform(stripped_transform[result.end() :])
+    return transforms
 
 
-def parse_color(c):
+def parse_color(col):
     """Creates a rgb int array"""
     # Based on the code in parseColor in the simplestyle.py module
     # Fixes a few bugs. Should be removed when fixed upstreams.
-    if c in list(inkex.colors.SVG_COLOR.keys()):
-        c = inkex.colors.SVG_COLOR[c]
+    if col in inkex.colors.SVG_COLOR:
+        col = inkex.colors.SVG_COLOR[col]
         # need to handle 'currentColor'
-    if c.startswith('#') and len(c) == 4:
-        c = '#' + c[1:2] + c[1:2] + c[2:3] + c[2:3] + c[3:] + c[3:]
-    elif c.startswith('rgb('):
+    if col.startswith("#") and len(col) == 4:
+        col = "#" + col[1:2] + col[1:2] + col[2:3] + col[2:3] + col[3:] + col[3:]
+    elif col.startswith("rgb("):
         # remove the rgb(...) stuff
-        tmp = c.strip()[4:-1]
-        numbers = [number.strip() for number in tmp.split(',')]
-        converted_numbers = []
+        tmp = col.strip()[4:-1]
+        numbers = [number.strip() for number in tmp.split(",")]
         if len(numbers) == 3:
+            converted_numbers = []
             for num in numbers:
-                if num.endswith(r'%'):
+                if num.endswith(r"%"):
                     converted_numbers.append(int(float(num[0:-1]) * 255 / 100))
                 else:
                     converted_numbers.append(int(num))
             return tuple(converted_numbers)
-        else:
-            return 0, 0, 0
+        return 0, 0, 0
     try:
-        r = int(c[1:3], 16)
-        g = int(c[3:5], 16)
-        b = int(c[5:], 16)
+        r_col = int(col[1:3], 16)
+        g_col = int(col[3:5], 16)
+        b_col = int(col[5:], 16)
     except ValueError:
         return 0, 0, 0
-    return r, g, b
+    return r_col, g_col, b_col
 
 
-def parse_style(s):
+def parse_style(string):
     """Create a dictionary from the value of an inline style attribute"""
     # This version strips leading and trailing whitespace from keys and values
-    if s:
-        return dict( (_.strip() for _ in kv.split(':')) for kv in (_.strip() for _ in s.split(';')) if len(kv) )
-    else:
-        return {}
+    if string:
+        return dict(
+            (_.strip() for _ in kv.split(":"))
+            for kv in (_.strip() for _ in string.split(";"))
+            if len(kv)
+        )
+    return {}
 
 
-def convert_arrow_style(arrow_name):
-    strip_name = arrow_name.split("start")[0].split("end")[0][5:-1]
+def parse_arrow_style(arrow_name):
+    """Docstring"""
+    strip_name = arrow_name.split("url")[1][3:-2]
 
     if "Arrow1" in strip_name:
         return "latex"
-    elif "Arrow2" in strip_name:
+    if "Arrow2" in strip_name:
         return "stealth"
-    elif "Stop" in strip_name:
+    if "Stop" in strip_name:
         return "|"
-    else:
-        return "latex"
+    return "latex"
+
 
+def marking_interpret(marker):
+    """Docstring"""
+    raw_marker = ""
+    if marker:
+        arrow_style = parse_arrow_style(marker)
+        raw_marker = arrow_style[:]
+        if "end" in marker:
+            raw_marker += " reversed"
+    return raw_marker
 
-class GraphicsState(object):
+
+class GraphicsState:
     """A class for handling the graphics state of an SVG element
 
     The graphics state includes fill, stroke and transformations.
     """
+
     fill = {}
     stroke = {}
     is_visible = True
     transform = []
     color = None
     opacity = 1
-    marker_start = None
-    marker_mid = None
-    marker_end = None
+
+    marker = [None, None, None]
 
     def __init__(self, svg_node):
         self.svg_node = svg_node
         self._parent_states = None
         self._get_graphics_state(svg_node)
 
     def _get_graphics_state(self, node):
         """Return the painting state of the node SVG element"""
         if node is None:
             return
-        style = parse_style(node.get('style', ''))
+        style = parse_style(node.get("style", ""))
         # get stroke and fill properties
         stroke = {}
         fill = {}
 
         for stroke_property in STROKE_PROPERTIES:
             stroke_val = style.get(stroke_property) or node.get(stroke_property)
             if stroke_val:
                 stroke[stroke_property] = stroke_val
 
         for fill_property in FILL_PROPERTIES:
             fill_val = style.get(fill_property) or node.get(fill_property)
             if fill_val:
                 fill[fill_property] = fill_val
 
-        display = style.get('display') or node.get('display')
-        visibility = style.get('visibility') or node.get('visibility')
-        if display == 'none' or visibility == 'hidden':
+        display = style.get("display") or node.get("display")
+        visibility = style.get("visibility") or node.get("visibility")
+        if display == "none" or visibility == "hidden":
             is_visible = False
         else:
             is_visible = True
 
-        self.color = style.get('color') or node.get('color')
+        self.color = style.get("color") or node.get("color")
         self.stroke = stroke
         self.fill = fill
         self.is_visible = is_visible
-        opacity = style.get('opacity') or node.get('opacity')
+        opacity = style.get("opacity") or node.get("opacity")
         self.opacity = opacity or 1
-        transform = node.get('transform', '')
+        transform = node.get("transform", "")
         if transform:
             self.transform = parse_transform(transform)
         else:
             self.transform = []
 
-        self.marker_start = style.get('marker-start') or node.get('marker-start')
-        self.marker_mid = style.get('marker-mid') or node.get('marker-mid')
-        self.marker_end = style.get('marker-end') or node.get('marker-end')
+        self.marker[0] = style.get("marker-start") or node.get("marker-start")
+        self.marker[1] = style.get("marker-mid") or node.get("marker-mid")
+        self.marker[2] = style.get("marker-end") or node.get("marker-end")
 
     def _get_parent_states(self, node=None):
         """Returns the parent's graphics states as a list"""
         if node is None:
             node = self.svg_node
         parent_node = node.getparent()
-        if not parent_node:
+        if len(parent_node):
             return None
         parents_state = []
-        while parent_node:
+        while len(parent_node):
             parents_state.append(GraphicsState(parents_state))
             parent_node = parent_node.getparent()
         return parents_state
 
     parent_states = property(fget=_get_parent_states)
 
     def accumulate(self, state):
+        """Docstring"""
         new_state = GraphicsState(None)
         new_state.fill = copy.copy(self.fill)
         new_state.stroke = copy.copy(self.stroke)
         new_state.transform = copy.copy(self.transform)
         new_state.opacity = copy.copy(self.opacity)
-        new_state.marker_start = copy.copy(self.marker_start)
-        new_state.marker_end = copy.copy(self.marker_end)
-        new_state.marker_mid = copy.copy(self.marker_mid)
+        new_state.marker = copy.copy(self.marker)
         new_state.fill.update(state.fill)
         new_state.stroke.update(state.stroke)
-        if new_state.stroke.get('stroke', '') == 'none':
-            del new_state.stroke['stroke']
-        if new_state.fill.get('fill', '') == 'none':
-            del new_state.fill['fill']
+        if new_state.stroke.get("stroke", "") == "none":
+            del new_state.stroke["stroke"]
+        if new_state.fill.get("fill", "") == "none":
+            del new_state.fill["fill"]
         new_state.transform += state.transform
         new_state.is_visible = self.is_visible and state.is_visible
         if state.color:
             new_state.color = state.color
 
         new_state.opacity *= state.opacity
-        new_state.marker_start = state.marker_start
-        new_state.marker_mid = state.marker_mid
-        new_state.marker_end = state.marker_end
+        # There were string before so reference is crossing now
+        new_state.marker = state.marker
         return new_state
 
     def __str__(self):
-        return "fill %s\nstroke: %s\nvisible: %s\ntransformations: %s\nmarker-start: %s\nmarker-mid: %s\nmarker-end: %s" % \
-               (self.fill, self.stroke, self.is_visible, self.transform, self.marker_start, self.marker_mid,
-                self.marker_end)
+        return f"""fill {self.fill}
+stroke: {self.stroke}
+visible: {self.is_visible}
+transformations: {self.transform}
+marker-start: {self.marker[0]}
+marker-mid: {self.marker[1]}
+marker-end: {self.marker[2]}"""
+
 
+# pylint: disable=too-many-ancestors
+class TikZPathExporter(inkex.Effect, inkex.EffectExtension):
+    """Class to export a svg to tikz code"""
 
-class TikZPathExporter(inkex.Effect):
     def __init__(self, inkscape_mode=True):
         self.inkscape_mode = inkscape_mode
         inkex.Effect.__init__(self)
+        inkex.EffectExtension.__init__(self)
         self._set_up_options()
 
-        self.text_indent = ''
-        self.x_o = self.y_o = 0.0
-        # px -> cm scale factors
-        self.x_scale = 0.02822219
-        # SVG has its origin in the upper left corner, while TikZ' origin is
-        # in the lower left corner. We therefore have to reverse the y-axis.
-        self.y_scale = -0.02822219
+        self.text_indent = ""
         self.colors = {}
         self.color_code = ""
         self.gradient_code = ""
         self.output_code = ""
         self.used_gradients = set()
         self.selected_sorted = []
+        self.height = 0
 
     def _set_up_options(self):
         parser = self.arg_parser
-        parser.set_defaults(codeoutput='standalone', crop=False, clipboard=False,
-                            wrap=False, indent=True, returnstring=False, scale=1,
-                            mode='effect', notext=False, verbose=False, texmode='escape', markings='ignore')
-        parser.add_argument('--codeoutput', dest='codeoutput',
-                          choices=('standalone', 'codeonly', 'figonly'),
-                          help="Amount of boilerplate code (standalone, figonly, codeonly).")
-        parser.add_argument('-t', '--texmode', dest='texmode', default='escape',
-                          choices=('math', 'escape', 'raw'),
-                          help="Set text mode (escape, math, raw). Defaults to 'escape'")
-        parser.add_argument('--markings', dest='markings', default='arrow',
-                          choices=('ignore', 'include', 'interpret', 'arrows'),
-                          help="Set markings mode (ignore, translate, interpret, arrows). Defaults to 'ignore'")
-        parser.add_argument('--arrow', dest='arrow', default='latex',
-                          choices=('latex', 'stealth', 'to', '>'),
-                          help="Set arrow style (latex, stealth, to, >) for markings mode arrow. Defaults to 'latex'")
-        parser.add_argument('--output-unit', dest='output_unit', default='cm',
-                          choices=('mm','cm','m', 'in', 'pt', 'px', 'Q', 'pc'),
-                          help="Set output units. Defaults to 'cm'")
-        parser.add_argument('--input-unit', dest='input_unit', default='mm',
-                          choices=('mm','cm','m', 'in', 'pt', 'px', 'Q', 'pc'),
-                          help="Set input units. Defaults to 'mm'")
-        self._add_booloption(parser, '--crop',
-                             dest="crop",
-                             help="Use the preview package to crop the tikzpicture")
-        self._add_booloption(parser, '--clipboard',
-                             dest="clipboard",
-                             help="Export to clipboard")
-        self._add_booloption(parser, '--wrap',
-                             dest="wrap",
-                             help="Wrap long lines")
-        self._add_booloption(parser, '--indent', default=True)
-        parser.add_argument('-to', '--tikzoutput',  type=str,
-                          dest='outputfile', default=None,
-                          help="")
-
-        self._add_booloption(parser, '--latexpathtype', dest="latexpathtype", default=True)
-        self._add_booloption(parser, '--noreversey',
-                             dest="noreversey",
-                             help="Do not reverse the y axis (origin is the same as inkscape but all height value are reversed)",
-                             default=False)
-
-        parser.add_argument('-r', '--removeabsolute',
-                          dest='removeabsolute', default=None,
-                          help="")
+        parser.set_defaults(
+            codeoutput="standalone",
+            crop=False,
+            clipboard=False,
+            wrap=False,
+            indent=True,
+            returnstring=False,
+            scale=1,
+            mode="effect",
+            notext=False,
+            verbose=False,
+            texmode="escape",
+            markings="ignore",
+        )
+        parser.add_argument(
+            "--codeoutput",
+            dest="codeoutput",
+            choices=("standalone", "codeonly", "figonly"),
+            help="Amount of boilerplate code (standalone, figonly, codeonly).",
+        )
+        parser.add_argument(
+            "-t",
+            "--texmode",
+            dest="texmode",
+            default="escape",
+            choices=("math", "escape", "raw"),
+            help="Set text mode (escape, math, raw). Defaults to 'escape'",
+        )
+        parser.add_argument(
+            "--markings",
+            dest="markings",
+            default="arrow",
+            choices=("ignore", "include", "interpret", "arrows"),
+            help="Set markings mode. Defaults to 'ignore'",
+        )
+        parser.add_argument(
+            "--arrow",
+            dest="arrow",
+            default="latex",
+            choices=("latex", "stealth", "to", ">"),
+            help="Set arrow style for markings mode arrow. Defaults to 'latex'",
+        )
+        parser.add_argument(
+            "--output-unit",
+            dest="output_unit",
+            default="cm",
+            choices=("mm", "cm", "m", "in", "pt", "px", "Q", "pc"),
+            help="Set output units. Defaults to 'cm'",
+        )
+        parser.add_argument(
+            "--input-unit",
+            dest="input_unit",
+            default="mm",
+            choices=("mm", "cm", "m", "in", "pt", "px", "Q", "pc"),
+            help="Set input units. Defaults to 'mm'",
+        )
+        self._add_booloption(
+            parser,
+            "--crop",
+            dest="crop",
+            help="Use the preview package to crop the tikzpicture",
+        )
+        self._add_booloption(
+            parser, "--clipboard", dest="clipboard", help="Export to clipboard"
+        )
+        self._add_booloption(parser, "--wrap", dest="wrap", help="Wrap long lines")
+        self._add_booloption(parser, "--indent", default=True, help="Indent lines")
+
+        self._add_booloption(
+            parser,
+            "--latexpathtype",
+            dest="latexpathtype",
+            default=True,
+            help="Allow path modification for image",
+        )
+        self._add_booloption(
+            parser,
+            "--noreversey",
+            dest="noreversey",
+            help="Do not reverse the y axis (Inkscape axis)",
+            default=False,
+        )
+
+        parser.add_argument(
+            "--removeabsolute",
+            dest="removeabsolute",
+            default=None,
+            help="Remove the value of removeabsolute from image path",
+        )
 
         if self.inkscape_mode:
-            parser.add_argument('--returnstring', action='store_true', dest='returnstring',
-                              help="Return as string")
-            parser.add_argument("--tab")  # Dummy option. Needed because Inkscape passes the notebook
+            parser.add_argument(
+                "--returnstring",
+                action="store_true",
+                dest="returnstring",
+                help="Return as string",
+            )
+            parser.add_argument(
+                "--tab"
+            )  # Dummy option. Needed because Inkscape passes the notebook
             # tab as an option.
-        parser.add_argument('-m', '--mode', dest='mode',
-                          choices=('output', 'effect', 'cli'), help="Extension mode (effect default)")
-        self._add_booloption(parser, '--notext', dest='ignore_text', default=False,
-                             help="Ignore all text")
+
+        # utility ?
+        parser.add_argument(
+            "-m",
+            "--mode",
+            dest="mode",
+            choices=("output", "effect", "cli"),
+            help="Extension mode (effect default)",
+        )
+        self._add_booloption(
+            parser,
+            "--notext",
+            dest="ignore_text",
+            default=False,
+            help="Ignore all text",
+        )
+        parser.add_argument(
+            "--scale",
+            dest="scale",
+            type=float,
+            help="Apply scale to resulting image, defaults to 1.0",
+        )
         if not self.inkscape_mode:
-            parser.add_argument('--standalone', dest='codeoutput',
-                              action='store_const', const='standalone',
-                              help="Generate a standalone document")
-            parser.add_argument('--figonly', dest='codeoutput',
-                              action='store_const', const='figonly',
-                              help="Generate figure only")
-            parser.add_argument('--codeonly', dest='codeoutput',
-                              action='store_const', const='codeonly',
-                              help="Generate drawing code only")
-            parser.add_argument('--scale', dest='scale', type=float,
-                              help="Apply scale to resulting image, defaults to 1.0")
-            parser.add_argument('-V', '--version', dest='printversion', action='store_true',
-                              help="Print version information and exit", default=False),
-        self._add_booloption(parser, '--verbose', dest='verbose', default=False,
-                             help="Verbose output (useful for debugging)")
+            parser.add_argument(
+                "--standalone",
+                dest="codeoutput",
+                action="store_const",
+                const="standalone",
+                help="Generate a standalone document",
+            )
+            parser.add_argument(
+                "--figonly",
+                dest="codeoutput",
+                action="store_const",
+                const="figonly",
+                help="Generate figure only",
+            )
+            parser.add_argument(
+                "--codeonly",
+                dest="codeoutput",
+                action="store_const",
+                const="codeonly",
+                help="Generate drawing code only",
+            )
+            parser.add_argument(
+                "-V",
+                "--version",
+                dest="printversion",
+                action="store_true",
+                help="Print version information and exit",
+                default=False,
+            )
+        self._add_booloption(
+            parser,
+            "--verbose",
+            dest="verbose",
+            default=False,
+            help="Verbose output (useful for debugging)",
+        )
 
     def parse(self, file_or_string=None):
         """Parse document in specified file or on stdin"""
         try:
             if file_or_string:
                 try:
-                    stream = open(file_or_string, 'r')
+                    with open(file_or_string, "r", encoding="utf8") as stream:
+                        self.document = etree.parse(stream)
+                        stream.close()
+
                 except (IOError, OSError):
                     stream = io.BytesIO(file_or_string.encode("utf-8"))
+                    self.document = etree.parse(stream)
+                    stream.close()
             else:
-                stream = open(self.args[-1], 'r')
-        except:
+                with open(self.args[-1], "r", encoding="utf8") as stream:
+                    self.document = etree.parse(stream)
+        except (IOError, OSError):
             stream = sys.stdin
-        self.document = etree.parse(stream)
-        stream.close()
+            self.document = etree.parse(stream)
+            stream.close()
 
     def _add_booloption(self, parser, *args, **kwargs):
         if self.inkscape_mode:
-            kwargs['action'] = 'store'
-            kwargs['type'] = inkex.Boolean
+            kwargs["action"] = "store"
+            kwargs["type"] = inkex.Boolean
             parser.add_argument(*args, **kwargs)
         else:
-            kwargs['action'] = 'store_true'
+            kwargs["action"] = "store_true"
             parser.add_argument(*args, **kwargs)
 
-    def convert_unit(self,value):
-        return inkex.units.convert_unit(value,self.options.output_unit,self.options.input_unit)
+    def convert_unit(self, value):
+        """Convert value from the input unit to the output unit which are options"""
+        return inkex.units.convert_unit(
+            value, self.options.output_unit, self.options.input_unit
+        )
 
-    def update_height(self,y):
+    def update_height(self, y_val):
+        """Compute the distance between the point and the bottom of the document"""
         if not self.options.noreversey:
-            return self.height - y
-        return y
+            return self.height - y_val
+        return y_val
 
-
-    def getselected(self):
+    def get_selected(self):
         """Get selected nodes in document order
 
         The nodes are stored in the selected dictionary and as a list of
         nodes in selected_sorted.
         """
+
         self.selected_sorted = []
         if len(self.options.ids) == 0:
             return
             # Iterate over every element in the document
 
         for node in self.document.getiterator():
-            node_id = node.get('id', '')
+            node_id = node.get("id", "")
             if node_id in self.options.ids:
-                # self.svg.selected[node_id] = node # useless for now and clash with property setting and setters of selected
+                # useless for now and clash with property setting
+                # and setters of selected
+
+                # self.svg.selected[node_id] = node
                 self.selected_sorted.append(node)
 
     def get_node_from_id(self, node_ref):
-        if node_ref.startswith('url('):
-            node_id = re.findall(r'url\((.*?)\)', node_ref)
+        """Return the node with the id node_ref. If there is none return None"""
+        if node_ref.startswith("url("):
+            node_id = re.findall(r"url\((.*?)\)", node_ref)
             if len(node_id) > 0:
                 ref_id = node_id[0]
         else:
             ref_id = node_ref
-        if ref_id.startswith('#'):
+        if ref_id.startswith("#"):
             ref_id = ref_id[1:]
 
-        ref_node = self.document.xpath('//*[@id="%s"]' % ref_id,
-                                       namespaces=inkex.NSS)
+        ref_node = self.document.xpath(f'//*[@id="{ref_id}"]', namespaces=inkex.NSS)
         if len(ref_node) == 1:
             return ref_node[0]
-        else:
-            return None
+        return None
 
     def transform(self, coord_list, cmd=None):
         """Apply transformations to input coordinates"""
         coord_transformed = []
-        # TEMP:
-        if cmd == 'Q':
+
+        if cmd == "Q":
             return tuple(coord_list)
-        try:
-            if not len(coord_list) % 2:
-                for x, y in nsplit(coord_list, 2):
-                    # coord_transformed.append("%.4fcm" % ((x-self.x_o)*self.x_scale))
-                    # oord_transformed.append("%.4fcm" % ((y-self.y_o)*self.y_scale))
-                    coord_transformed.append("%.4f" % x)
-                    coord_transformed.append("%.4f" % y)
-            elif len(coord_list) == 1:
-                coord_transformed = ["%.4fcm" % (coord_list[0] * self.x_scale)]
-            else:
-                coord_transformed = coord_list
-        except:
+
+        if not isinstance(coord_list, list):
+            coord_transformed = coord_list
+        elif not len(coord_list) % 2:
+            for x_pos, y_pos in nsplit(coord_list, 2):
+                coord_transformed.append(f"{x_pos:.4f}")
+                coord_transformed.append(f"{y_pos:.4f}")
+        elif len(coord_list) == 1:
+            coord_transformed = [f"{coord_list[0]:.4f}cm"]
+        else:
             coord_transformed = coord_list
-        return tuple(coord_transformed)
 
-    def pxToPt(self, pixels):
-        return pixels * 0.8;
+        return tuple(coord_transformed)
 
     def get_color(self, color):
         """Return a valid xcolor color name and store color"""
 
         if color in self.colors:
             return self.colors[color]
-        else:
-            r, g, b = parse_color(color)
-            if not (r or g or b):
-                return "black"
-            if color.startswith('rgb'):
-                xcolorname = "c%02x%02x%02x" % (r, g, b)
-            else:
-                xcolorname = color.replace('#', 'c')
-            self.colors[color] = xcolorname
-            self.color_code += "\\definecolor{%s}{RGB}{%s,%s,%s}\n" \
-                               % (xcolorname, r, g, b)
-            return xcolorname
+
+        r, g, *b = parse_color(color)
+        if isinstance(b, list):
+            b = b[0]
+        if not (r or g or b):
+            return "black"
+        if color.startswith("rgb"):
+            xcolorname = f"c{r:02x}{g:02x}{b:02x}"
+        else:
+            xcolorname = color.replace("#", "c")
+        self.colors[color] = xcolorname
+        self.color_code += "\\definecolor{" + f"{xcolorname}" + "}{RGB}{"
+        self.color_code += f"{r},{g},{b}" + "}\n"
+        return xcolorname
 
     def _convert_gradient(self, gradient_node, gradient_tikzname):
         """Convert an SVG gradient to a PGF gradient"""
 
         # http://www.w3.org/TR/SVG/pservers.html
         def bpunit(offset):
             bp_unit = ""
             if offset.endswith("%"):
                 bp_unit = offset[0:-1]
             else:
                 bp_unit = str(int(round((float(offset)) * 100)))
             return bp_unit
 
-        if gradient_node.tag == _ns('linearGradient'):
+        if gradient_node.tag == _ns("linearGradient"):
             c = ""
-            c += "\pgfdeclarehorizontalshading{%s}{100bp}{\n" % gradient_tikzname
+            c += (
+                r"\pgfdeclarehorizontalshading{"
+                + f"{gradient_tikzname}"
+                + "}{100bp}{\n"
+            )
             stops = []
             for n in gradient_node:
-                if n.tag == _ns('stop'):
-                    stops.append("color(%spt)=(%s)" % (bpunit(n.get("offset")), self.get_color(n.get("stop-color"))))
+                if n.tag == _ns("stop"):
+                    stops.append(
+                        f"color({bpunit(n.get('offset'))}pt)="
+                        f"({self.get_color(n.get('stop-color'))})"
+                    )
             c += ";".join(stops)
             c += "\n}\n"
             return c
 
-        else:
-            return ""
+        return ""
 
-    def _handle_gradient(self, gradient_ref, node=None):
+    def _handle_gradient(self, gradient_ref):
         grad_node = self.get_node_from_id(gradient_ref)
-        gradient_id = grad_node.get('id')
+        gradient_id = grad_node.get("id")
         if grad_node is None:
             return []
         gradient_tikzname = gradient_id
         if gradient_id not in self.used_gradients:
             grad_code = self._convert_gradient(grad_node, gradient_tikzname)
             if grad_code:
                 self.gradient_code += grad_code
                 self.used_gradients.add(gradient_id)
         if gradient_id in self.used_gradients:
-            return ['shade', 'shading=%s' % gradient_tikzname]
-        else:
-            return []
+            return ["shade", f"shading={gradient_tikzname}"]
+        return []
 
-    def _handle_markers(self, state, accumulated_state):
+    def _handle_markers(self, state, _):
         # http://www.w3.org/TR/SVG/painting.html#MarkerElement
 
         # Avoid options "-" on empty path
-        if not state.marker_start and not state.marker_end:
+        if not state.marker[0] and not state.marker[2]:
             return []
 
-        if self.options.markings == 'ignore':
+        if self.options.markings == "ignore":
             return []
 
-        elif self.options.markings == "include":
+        if self.options.markings == "include":
             # TODO to implement:
             # Include arrow as path object
             # Define custom arrow and use them
-            pass
+            return []
 
-        elif self.options.markings == "interpret":
-            start_arrow = ""
-            end_arrow = ""
-            if state.marker_start:
-                arrow_style = convert_arrow_style(state.marker_start)
-                start_arrow = arrow_style[:]
-                if "end" in state.marker_start:
-                    start_arrow +=  " reversed"
-
-            if state.marker_end:
-                arrow_style = convert_arrow_style(state.marker_end)
-                end_arrow = arrow_style[:]
-                if "start" in state.marker_end:
-                    end_arrow +=  " reversed"
+        if self.options.markings == "interpret":
+            start_arrow = marking_interpret(state.marker[0])
+            end_arrow = marking_interpret(state.marker[2])
 
             return [start_arrow + "-" + end_arrow]
 
-        elif self.options.markings == "arrows":
-            start_arrow = ""
-            end_arrow = ""
-            if state.marker_start:
-                start_arrow = self.options.arrow[:]
-                if "end" in state.marker_start:
-                    start_arrow +=  " reversed"
-
-                if ">" == self.options.arrow:
-                    if "end" in state.marker_start:
-                        start_arrow = ">"
-                    else:
-                        start_arrow = "<"
-
-            if state.marker_end:
-                end_arrow = self.options.arrow[:]
-                if "start" in state.marker_end:
-                    end_arrow +=  " reversed"
-
-                if ">" == self.options.arrow:
-                    if "start" in state.marker_end:
-                        end_arrow = "<"
-                    else:
-                        end_arrow = ">"
+        if self.options.markings == "arrows":
+            start_arrow = self.options.arrow[:] if state.marker[0] else ""
+            # TODO check first that is not None
+            if state.marker[0] and "end" in state.marker[0]:
+                start_arrow += " reversed"
+
+            if start_arrow == self.options.arrow:
+                start_arrow = "<"
+                if "end" in state.marker[0]:
+                    start_arrow = ">"
+
+            end_arrow = self.options.arrow[:] if state.marker[2] else ""
+            if state.marker[2] and "start" in state.marker[2]:
+                end_arrow += " reversed"
+
+            if end_arrow == self.options.arrow:
+                end_arrow = ">"
+                if "start" in state.marker[2]:
+                    end_arrow = "<"
 
             return [start_arrow + "-" + end_arrow]
-
+        return []
 
     def convert_svgstate_to_tikz(self, state, accumulated_state=None, node=None):
         """Return a node's SVG styles as a list of TikZ options"""
+        # TODO should be reworked to follow pylint
+        # pylint: disable=too-many-branches
+        # pylint: disable=too-many-statements
         if not state.is_visible:
             return [], []
 
         options = []
         transform = []
 
         if state.color:
-            options.append('color=%s' % self.get_color(state.color))
+            options.append(f"color={self.get_color(state.color)}")
 
-        stroke = state.stroke.get('stroke', '')
-        if stroke != 'none':
+        stroke = state.stroke.get("stroke", "")
+        if stroke != "none":
             if stroke:
-                if stroke == 'currentColor':
-                    options.append('draw')
+                if stroke == "currentColor":
+                    options.append("draw")
                 else:
-                    options.append('draw=%s' % self.get_color(stroke))
+                    options.append(f"draw={self.get_color(stroke)}")
             else:
                 # need to check if parent element has stroke set
-                if 'stroke' in accumulated_state.stroke:
-                    options.append('draw')
+                if "stroke" in accumulated_state.stroke:
+                    options.append("draw")
 
-        fill = state.fill.get('fill')
-        if fill != 'none':
+        fill = state.fill.get("fill")
+        if fill != "none":
             if fill:
-                if fill == 'currentColor':
-                    options.append('fill')
-                elif fill.startswith('url('):
+                if fill == "currentColor":
+                    options.append("fill")
+                elif fill.startswith("url("):
                     pass
                     # shadeoptions = self._handle_gradient(fill)
                     # options.extend(shadeoptions)
                 else:
-                    options.append('fill=%s' % self.get_color(fill))
+                    options.append(f"fill={self.get_color(fill)}")
             else:
                 # Shapes are defined as in SVG standard
                 # https://www.w3.org/TR/2011/REC-SVG11-20110816/intro.html#TermShape
-                shapes = ('path', 'rect', 'circle', 'ellipse',
-                    'line', 'polyline', 'polygon')
+                shapes = (
+                    "path",
+                    "rect",
+                    "circle",
+                    "ellipse",
+                    "line",
+                    "polyline",
+                    "polygon",
+                )
                 shapes = [_ns(x) for x in shapes]
 
-                if 'fill' in accumulated_state.fill:
-                    options.append('fill')
+                if "fill" in accumulated_state.fill:
+                    options.append("fill")
                 elif node.tag in shapes:
                     # svg shapes with no fill option should fill by black
                     # https://www.w3.org/TR/2011/REC-SVG11-20110816/painting.html#FillProperty
                     # tikz automatically does fill=black if fill is empty
-                    options.append('fill')
+                    options.append("fill")
 
         marker_options = self._handle_markers(state, accumulated_state)
         if marker_options:
             options += marker_options
 
         # dash pattern has to come before dash phase. This is a bug in TikZ 2.0
         # Fixed in CVS.
 
         # TODO: dash phase is not the same between tikz and inkscape for rectangle.
-        dasharray = state.stroke.get('stroke-dasharray')
-        if dasharray and dasharray != 'none':
-            lengths = list(map(self.convert_unit, [i.strip() for i in dasharray.split(',')]))
+        dasharray = state.stroke.get("stroke-dasharray")
+        if dasharray and dasharray != "none":
+            split_str = ","
+            if split_str not in dasharray:
+                split_str = " "
+            lengths = list(
+                map(self.convert_unit, [i.strip() for i in dasharray.split(split_str)])
+            )
             dashes = []
             for idx, length in enumerate(lengths):
                 # There was a 0.8 factor here (maybe from unit change in inkscape)
-                lenstr = "%0.3f%s" % (length * self.options.scale, self.options.output_unit)
+                lenstr = f"{length * self.options.scale:0.3f}{self.options.output_unit}"
                 if idx % 2:
-                    dashes.append("off %s" % lenstr)
+                    dashes.append(f"off {lenstr}")
                 else:
-                    dashes.append("on %s" % lenstr)
-            options.append('dash pattern=%s' % " ".join(dashes))
+                    dashes.append(f"on {lenstr}")
+            options.append(f"dash pattern={' '.join(dashes)}")
 
-        try:
+        if hasattr(state, "opacity"):
             opacity = float(state.opacity)
             if opacity < 1.0:
-                options.append('opacity=%.03f' % opacity)
-        except:
-            pass
+                options.append(f"opacity={opacity:.03f}")
 
         for svgname, tikzdata in PROPERTIES_MAP.items():
             tikzname, valuetype, data = tikzdata
             value = state.fill.get(svgname) or state.stroke.get(svgname)
             if not value:
                 continue
             if valuetype == SCALE:
                 val = float(value)
-                if not val == 1:
-                    options.append('%s=%.3f' % (tikzname, float(value)))
+                if val != 1:
+                    options.append(f"{tikzname}={float(value):.3f}")
             elif valuetype == DICT:
                 if tikzname:
-                    options.append('%s=%s' % (tikzname, data.get(value, '')))
+                    options.append(f"{tikzname}={data.get(value,'')}")
                 else:
-                    options.append('%s' % data.get(value, ''))
+                    options.append(data.get(value, ""))
             elif valuetype == DIMENSION:
                 if value and value != data:
                     # There was a 0.8 factor here (maybe from unit change in inkscape)
-                    options.append('%s=%.3f%s' % (tikzname, self.convert_unit(value) * self.options.scale, self.options.output_unit)),
+                    options.append(
+                        f"{tikzname}="
+                        f"{self.convert_unit(value) * self.options.scale:.3f}"
+                        f"{self.options.output_unit}"
+                    )
             elif valuetype == FACTOR:
                 try:
                     val = float(value)
                     if val >= 1.0:
-                        options.append('%s=%.2f' % (tikzname, val))
+                        options.append(f"{tikzname}={val:.2f}")
                 except ValueError:
                     pass
 
         if len(state.transform) > 0:
             transform = self._convert_transform_to_tikz(state.transform)
         else:
             transform = []
@@ -1046,545 +1220,615 @@
         """Convert a SVG transform attribute to a list of TikZ transformations"""
         # return ""
         if not transform:
             return []
 
         options = []
         for cmd, params in transform:
-            if cmd == 'translate':
-
-                # TODO here
+            if cmd == "translate":
                 x, y = [self.convert_unit(str(val)) for val in params]
-                y = self.update_height(y)
-                options.append("shift={(%s,%s)}" % (x or '0', y or '0'))
+                if not self.options.noreversey:
+                    y *= (
+                        -1
+                    )  # Update height reverse the sign of y so it should also be the case for a translation
+                # y = self.update_height(y)
+                options.append("shift={" + f"({x or '0'},{y or '0'})" + "}")
 
                 # There is bug somewere.
                 # shift=(400,0) is not equal to xshift=400
 
-            elif cmd == 'rotate':
+            elif cmd == "rotate":
                 # Still needed or inside matrix transform ?
                 if params[1] or params[2]:
-                    options.append("rotate around={%s:(%s,%s)}" % params)
+                    options.append(
+                        "rotate around={" f"{params[0]}:({params[1]},{params[2]})" + "}"
+                    )
                 else:
-                    options.append("rotate=%s" % params[0])
-            elif cmd == 'matrix':
-
+                    options.append(f"rotate={params[0]}")
+            elif cmd == "matrix":
                 tx = self.convert_unit(params[4])
                 ty = self.update_height(self.convert_unit(params[5]))
-                options.append(f"cm={{ {params[0]},{params[1]},{params[2]},{params[3]},({tx},{ty})}}")
-            elif cmd == 'skewX':
-                options.append("xslant=%s" % math.tan(params[0] * math.pi / 180))
-            elif cmd == 'skewY':
-                options.append("yslant=%s" % math.tan(params[0] * math.pi / 180))
-            elif cmd == 'scale':
+                options.append(
+                    f"cm={{ {params[0]},{params[1]},{params[2]}"
+                    f",{params[3]},({tx},{ty})}}"
+                )
+            elif cmd == "skewX":
+                options.append(f"xslant={math.tan(params[0] * math.pi / 180)}")
+            elif cmd == "skewY":
+                options.append(f"yslant={math.tan(params[0] * math.pi / 180)}")
+            elif cmd == "scale":
                 if params[0] == params[1]:
-                    options.append("scale=%s" % params[0])
+                    options.append(f"scale={params[0]}")
                 else:
-                    options.append("xscale=%s,yscale=%s" % params)
+                    options.append(f"xscale={params[0]},yscale={params[1]}")
 
         return options
 
     def _handle_group(self, groupnode, graphics_state, accumulated_state):
         s = ""
         tmp = self.text_indent
 
         self.text_indent += TEXT_INDENT
-        group_id = groupnode.get('id')
-        code = self._output_group(groupnode, accumulated_state.accumulate(graphics_state))
+        group_id = groupnode.get("id")
+        code = self._output_group(
+            groupnode, accumulated_state.accumulate(graphics_state)
+        )
         self.text_indent = tmp
         if self.options.verbose and group_id:
-            extra = "%% %s" % group_id
+            extra = f"%% {group_id}"
         else:
-            extra = ''
-        goptions, transformation = self.convert_svgstate_to_tikz(graphics_state, graphics_state, groupnode)
+            extra = ""
+        goptions, transformation = self.convert_svgstate_to_tikz(
+            graphics_state, graphics_state, groupnode
+        )
         options = transformation + goptions
         if len(options) > 0:
-            pstyles = [','.join(options)]
-            if 'opacity' in pstyles[0]:
-                pstyles.append('transparency group')
+            pstyles = [",".join(options)]
+            if "opacity" in pstyles[0]:
+                pstyles.append("transparency group")
 
             if self.options.indent:
-                s += "%s\\begin{scope}[%s]%s\n%s%s\\end{scope}\n" % \
-                     (self.text_indent, ",".join(pstyles), extra,
-                      code, self.text_indent)
+                s += self.text_indent + "\\begin{scope}"
+                s += f"[{','.join(pstyles)}]{extra}\n{code}{self.text_indent}"
+                s += "\\end{scope}\n"
             else:
-                s += "\\begin{scope}[%s]%s\n%s\\end{scope}\n" % \
-                     (",".join(pstyles), extra, code)
+                s += "\\begin{scope}"
+                s += f"[{','.join(pstyles)}]{extra}\n{code}"
+                s += "\\end{scope}\n"
         elif self.options.verbose:
             if self.options.indent:
-                s += "%s\\begin{scope}%s\n%s%s\\end{scope}\n" % \
-                     (self.text_indent, extra, code, self.text_indent)
+                s += self.text_indent + "\\begin{scope}"
+                s += f"{extra}\n{code}{self.text_indent}"
+                s += "\\end{scope}\n"
             else:
-                s += "\\begin{scope}\n%s\\end{scope}\n" % \
-                     (code,)
+                s += "\\begin{scope}" + f"{code}" + "\\end{scope}\n"
         else:
             s += code
         return s
 
     def _handle_image(self, node):
         """Handles the image tag and returns a code, options tuple"""
         # http://www.w3.org/TR/SVG/struct.html#ImageElement
         # http://www.w3.org/TR/SVG/coords.html#PreserveAspectRatioAttribute
         #         Convert the pixel values to pt first based on http://www.endmemo.com/sconvert/pixelpoint.php
-        x = self.convert_unit(node.get('x', '0'));
-        y = self.update_height(self.convert_unit(node.get('y', '0')));
-
-        width = self.pxToPt(self.convert_unit(node.get('width', '0')));
-        height = self.pxToPt(self.convert_unit(node.get('height', '0')));
+        x = self.convert_unit(node.get("x", "0"))
+        y = self.update_height(self.convert_unit(node.get("y", "0")))
 
-        href = node.get(_ns('href', 'xlink'));
-        isvalidhref = 'data:image/png;base64' not in href;
-        if (self.options.latexpathtype and isvalidhref):
-            href = href.replace(self.options.removeabsolute, '');
-        if (not isvalidhref):
-            href = 'base64 still not supported';
-            # print (" x:%s, y:%s, w:%s, h:%s, %% Href %s," % (x, y,width, height,  node.get(_ns('href', 'xlink'))));
+        # TODO test that
+        width = inkex.units.convert_unit(
+            self.convert_unit(node.get("width", "0")), "pt", "px"
+        )
+        height = inkex.units.convert_unit(
+            self.convert_unit(node.get("height", "0")), "pt", "px"
+        )
+
+        href = node.get(_ns("href", "xlink"))
+        isvalidhref = "data:image/png;base64" not in href
+        if self.options.latexpathtype and isvalidhref:
+            href = href.replace(self.options.removeabsolute, "")
+        if not isvalidhref:
+            href = "base64 still not supported"
+            # print (" x:%s, y:%s, w:%s, h:%s, %% Href %s," %
+            # (x, y,width, height,  node.get(_ns('href', 'xlink'))));
         # return None, []
-        return ('image', (x, y, width, height, href)), []
+        return ("image", (x, y, width, height, href)), []
 
     def _handle_path(self, node):
         try:
-            raw_path = node.get('d')
-            #p = simplepath.parsePath(raw_path)
+            raw_path = node.get("d")
+            # p = simplepath.parsePath(raw_path)
             p = inkex.Path(raw_path).to_arrays()
 
             #             logging.warning('Path Values %s'%(len(p)),);
             for path_punches in p:
-                #                 Scale, and 0.8 has to be applied to the path values
                 try:
-                    cmd, xy = path_punches;
-                    path_punches[1] = [self.convert_unit(str(val)) for val in xy];
-                    path_punches[1][1] = self.update_height(path_punches[1][1])
+                    _, xy = path_punches
+                    path_punches[1] = [self.convert_unit(str(val)) for val in xy]
+
+                    if path_punches[0] == "A":
+                        path_punches[1][6] = self.update_height(path_punches[1][6])
+                    else:
+                        for i in range(int(len(path_punches[1]) / 2)):
+                            path_punches[1][1 + 2 * i] = self.update_height(
+                                path_punches[1][1 + 2 * i]
+                            )
+
                 except ValueError:
-                    pass;
-        except:
-            e = sys.exc_info()[0];
-            logging.warning('Failed to parse path %s, will ignore it', raw_path)
-            logging.warning('Exception %s' % (e), );
-            logging.warning('Values %s' % (path_punches));
+                    pass
+
+        except ValueError:
+            e = sys.exc_info()[0]
+            logging.warning("Failed to parse path %s, will ignore it", raw_path)
+            logging.warning("Exception %s", e)
+            logging.warning("Values %s", path_punches)
             p = None
         return p, []
 
     def _handle_shape(self, node):
         """Extract shape data from node"""
         options = []
-        if node.tag == _ns('rect'):
-            inset = node.get('rx', '0') or node.get('ry', '0')
+        if node.tag == _ns("rect"):
+            inset = node.get("rx", "0") or node.get("ry", "0")
             # TODO: ry <> rx is not supported by TikZ. Convert to path?
-            x = self.convert_unit(node.get('x','0'))
-            y = self.update_height(self.convert_unit(node.get('y','0')))
+            x = self.convert_unit(node.get("x", "0"))
+            y = self.update_height(self.convert_unit(node.get("y", "0")))
 
             # map from svg to tikz
-            width = self.convert_unit(node.get('width', '0'))
-            height = self.convert_unit(node.get('height', '0'))
+            width = self.convert_unit(node.get("width", "0"))
+            height = self.convert_unit(node.get("height", "0"))
+            if not self.options.noreversey:
+                height *= -1  # y direction should be reversed
             if width == 0.0 or height == 0.0:
                 return None, []
             if inset:
-                # TODO: corner radius is not scaled by PGF. Find a better way to fix this.
-                options = ["rounded corners=%s" % self.transform([self.convert_unit(inset) * 0.8 * self.options.scale])]
-            return ('rect', (x, y, width + x, height + y)), options
-
-        elif node.tag in [_ns('polyline'),
-                          _ns('polygon')]:
-            points = node.get('points', '').replace(',', ' ')
-            # TODO here
+                # TODO: corner radius is not scaled by PGF.
+                unit_to_scale = self.convert_unit(inset) * self.options.scale
+                round_corners = self.transform([unit_to_scale])
+                options = [f"rounded corners={round_corners[0]}"]
+            return ("rect", (x, y, width + x, height + y)), options
+
+        if node.tag in [_ns("polyline"), _ns("polygon")]:
+            points = node.get("points", "").replace(",", " ")
 
             points = list(map(self.convert_unit, points.split()))
-            if node.tag == _ns('polyline'):
-                cmd = 'polyline'
+            if node.tag == _ns("polyline"):
+                cmd = "polyline"
             else:
-                cmd = 'polygon'
+                cmd = "polygon"
 
             return (cmd, points), options
-        elif node.tag in _ns('line'):
-            points = [node.get('x1'), node.get('y1'),
-                      node.get('x2'), node.get('y2')]
-            # TODO here
+        if node.tag in _ns("line"):
+            points = [node.get("x1"), node.get("y1"), node.get("x2"), node.get("y2")]
             points = list(map(self.convert_unit, points))
             # check for zero lenght line
             if not ((points[0] == points[2]) and (points[1] == points[3])):
                 points[1] = self.update_height(points[1])
                 points[3] = self.update_height(points[3])
-                return ('polyline', points), options
+                return ("polyline", points), options
 
-        if node.tag == _ns('circle'):
+        if node.tag == _ns("circle"):
             # ugly code...
-            center = list(map(self.convert_unit, [node.get('cx', '0'), node.get('cy', '0')]))
+            center = list(
+                map(self.convert_unit, [node.get("cx", "0"), node.get("cy", "0")])
+            )
             center[1] = self.update_height(center[1])
-            r = self.convert_unit(node.get('r', '0'))
+            r = self.convert_unit(node.get("r", "0"))
             if r > 0.0:
-                return ('circle', self.transform(center) + self.transform([r])), options
+                return ("circle", self.transform(center) + self.transform([r])), options
 
-        elif node.tag == _ns('ellipse'):
-            center = list(map(self.convert_unit, [node.get('cx', '0'), node.get('cy', '0')]))
+        if node.tag == _ns("ellipse"):
+            center = list(
+                map(self.convert_unit, [node.get("cx", "0"), node.get("cy", "0")])
+            )
             center[1] = self.update_height(center[1])
-            rx = self.convert_unit(node.get('rx', '0'))
-            ry = self.convert_unit(node.get('ry', '0'))
+            rx = self.convert_unit(node.get("rx", "0"))
+            ry = self.convert_unit(node.get("ry", "0"))
             if rx > 0.0 and ry > 0.0:
-                return ('ellipse', self.transform(center) + self.transform([rx])
-                        + self.transform([ry])), options
-        else:
-            return None, options
+                return (
+                    "ellipse",
+                    self.transform(center)
+                    + self.transform([rx])
+                    + self.transform([ry]),
+                ), options
 
         return None, options
 
     def _handle_text(self, node):
         if self.options.ignore_text:
             return None, []
         raw_textstr = self.get_text(node).strip()
-        if self.options.texmode == 'raw':
+        if self.options.texmode == "raw":
             textstr = raw_textstr
-        elif self.options.texmode == 'math':
-            textstr = "$%s$" % raw_textstr
+        elif self.options.texmode == "math":
+            textstr = f"${raw_textstr}$"
         else:
             textstr = escape_texchars(raw_textstr)
 
-        x = self.convert_unit(node.get('x', '0'))
-        y = self.update_height(self.convert_unit(node.get('y', '0')))
-        p = [('M', [x, y]), ('TXT', textstr)]
+        x = self.convert_unit(node.get("x", "0"))
+        y = self.update_height(self.convert_unit(node.get("y", "0")))
+        p = [("M", [x, y]), ("TXT", textstr)]
         return p, []
 
-    def _handle_use(self, node, graphics_state, accumulated_state=None):
+    def _handle_use(self, node, _, accumulated_state=None):
         # Find the id of the use element link
-        ref_id = node.get(_ns('href', 'xlink'))
-        if ref_id.startswith('#'):
+        ref_id = node.get(_ns("href", "xlink"))
+        if ref_id.startswith("#"):
             ref_id = ref_id[1:]
 
-        use_ref_node = self.document.xpath('//*[@id="%s"]' % ref_id,
-                                           namespaces=inkex.NSS)
+        use_ref_node = self.document.xpath(f'//*[@id="{ref_id}"]', namespaces=inkex.NSS)
         if len(use_ref_node) > 0:
             # len(use_ref_node) > 1 means that there are several elements with the
             # same id. According to the XML spec the value should be unique.
-            # SVG generated by some tools (for instance Matplotlib) does not obey this rule,
+            # SVG generated by some tools (e.g. Matplotlib) does not obey this rule,
             # so we just pick the first one. Should probably generate a warning as well.
             use_ref_node = use_ref_node[0]
         else:
             return ""
 
         # create a temp group
-        g_wrapper = etree.Element(_ns('g'))
-        use_g = etree.SubElement(g_wrapper, _ns('g'))
+        g_wrapper = etree.Element(_ns("g"))
+        use_g = etree.SubElement(g_wrapper, _ns("g"))
 
         # transfer attributes from use element to new group except
         # x, y, width, height and href
         for key in list(node.keys()):
-            if key not in ('x', 'y', 'width', 'height',
-                           _ns('href', 'xlink')):
+            if key not in ("x", "y", "width", "height", _ns("href", "xlink")):
                 use_g.set(key, node.get(key))
-        if node.get('x') or node.get('y'):
-            transform = node.get('transform', '')
-            transform += ' translate(%s,%s) ' \
-                         % (self.convert_unit(node.get('x', 0)), self.update_height(self.convert_unit(node.get('y', 0))))
-            use_g.set('transform', transform)
+        if node.get("x") or node.get("y"):
+            transform = node.get("transform", "")
+            transform += (
+                f" translate({self.convert_unit(node.get('x', 0))}"
+                f",{self.update_height(self.convert_unit(node.get('y', 0)))})"
+            )
+            use_g.set("transform", transform)
             #
         use_g.append(deepcopy(use_ref_node))
         return self._output_group(g_wrapper, accumulated_state)
 
     def _write_tikz_path(self, pathdata, options=None, node=None):
         """Convert SVG paths, shapes and text to TikZ paths"""
+
+        # TODO should be reworked to follow pylint
+        # pylint: disable=too-many-locals
+        # pylint: disable=too-many-branches
+        # pylint: disable=too-many-statements
+
         s = pic = pathcode = imagecode = ""
         # print "Pathdata %s" % pathdata
         if not pathdata or len(pathdata) == 0:
             return ""
         if node is not None:
-            node_id = node.get('id', '')
+            node_id = node.get("id", "")
         else:
-            node_id = ''
+            node_id = ""
 
         current_pos = [0.0, 0.0]
         for cmd, params in pathdata:
             # transform coordinates
             tparams = self.transform(params, cmd)
             # SVG paths
             # moveto
-            if cmd == 'M':
-                s += "(%s,%s)" % tparams
+            if cmd == "M":
+                s += f"({tparams[0]},{tparams[1]})"
                 current_pos = params[-2:]
             # lineto
-            elif cmd == 'L':
-                s += " -- (%s,%s)" % tparams
+            elif cmd == "L":
+                s += f" -- ({tparams[0]},{tparams[1]})"
                 current_pos = params[-2:]
             # cubic bezier curve
-            elif cmd == 'C':
-                s += " .. controls (%s,%s) and (%s,%s) .. (%s,%s)" % tparams
+            elif cmd == "C":
+                s += (
+                    f" .. controls ({tparams[0]}, {tparams[1]})"
+                    f" and ({tparams[2]}, {tparams[3]}) .. ({tparams[4]}, {tparams[5]})"
+                )
                 current_pos = params[-2:]
             # quadratic bezier curve
-            elif cmd == 'Q':
+            elif cmd == "Q":
                 # need to convert to cubic spline
                 # CP1 = QP0 + 2/3 *(QP1-QP0)
                 # CP2 = CP1 + 1/3 *(QP2-QP0)
                 # http://fontforge.sourceforge.net/bezier.html
                 qp0x, qp0y = current_pos
                 qp1x, qp1y, qp2x, qp2y = tparams
                 cp1x = qp0x + (2.0 / 3.0) * (qp1x - qp0x)
                 cp1y = qp0y + (2.0 / 3.0) * (qp1y - qp0y)
                 cp2x = cp1x + (qp2x - qp0x) / 3.0
                 cp2y = cp1y + (qp2y - qp0y) / 3.0
-                s += " .. controls (%.4f,%.4f) and (%.4f,%.4f) .. (%.4f,%.4f)" \
-                     % (cp1x, cp1y, cp2x, cp2y, qp2x, qp2y)
+                s += (
+                    f" .. controls ({cp1x:.4f}, {cp1y:.4f}) and ({cp2x:.4f},"
+                    f" {cp2y:.4f}) .. ({qp2x:.4f}, {qp2y:.4f})"
+                )
                 current_pos = params[-2:]
             # close path
-            elif cmd == 'Z':
+            elif cmd == "Z":
                 s += " -- cycle"
-                closed_path = True
             # arc
-            elif cmd == 'A':
-                start_ang_o, end_ang_o, rx, ry = calc_arc(current_pos[0], current_pos[1], *params)
+            elif cmd == "A":
+                cp = Point(current_pos[0], current_pos[1])
+                r = Point(tparams[0], tparams[1])
+                pos = Point(tparams[5], tparams[6])
+                start_ang_o, end_ang_o, r = calc_arc(cp, r, *params[2:5], pos)
+
                 # pgf 2.0 does not like angles larger than 360
                 # make sure it is in the +- 360 range
                 start_ang = start_ang_o % 360
                 end_ang = end_ang_o % 360
-                if start_ang_o < end_ang_o and not (start_ang < end_ang):
+                if start_ang_o < end_ang_o and not start_ang < end_ang:
                     start_ang -= 360
-                elif start_ang_o > end_ang_o and not (start_ang > end_ang):
+                elif start_ang_o > end_ang_o and not start_ang > end_ang:
                     end_ang -= 360
                 ang = params[2]
-                if rx == ry:
+                if r.x == r.y:
                     # Todo: Transform radi
-                    radi = "%.3f" % rx
+                    radi = f"{r.x:.3f}"
                 else:
-                    radi = "%3f and %.3f" % (rx, ry)
+                    radi = f"{r.x:3f} and {r.y:.3f}"
                 if ang != 0.0:
-                    s += "{[rotate=%s] arc(%.3f:%.3f:%s)}" % (ang, start_ang, end_ang, radi)
+                    s += (
+                        "{" + f"[rotate={ang}] arc({start_ang:.3f}"
+                        ":{end_ang:.3f}:{radi})" + "}"
+                    )
                 else:
-                    s += "arc(%.3f:%.3f:%s)" % (start_ang, end_ang, radi)
+                    s += f"arc({start_ang:.3f}:{end_ang:.3f}:{radi})"
                 current_pos = params[-2:]
-                pass
-            elif cmd == 'TXT':
-                s += " node[above right] (%s) {%s}" % (node_id, params)
+            elif cmd == "TXT":
+                s += f" node[above right] ({node_id})" + "{" + f"{params}" + "}"
             # Shapes
-            elif cmd == 'rect':
-                # print(tparams, params)
-                s += "(%s,%s) rectangle (%s,%s)" % tparams
-                closed_path = True
-            elif cmd in ['polyline', 'polygon']:
-                points = ["(%s,%s)" % (x, y) for x, y in chunks(tparams, 2)]
-                if cmd == 'polygon':
-                    points.append('cycle')
-                    closed_path = True
+            elif cmd == "rect":
+                s += f"({tparams[0]}, {tparams[1]}) rectangle ({tparams[2]}, {tparams[3]})"
+            elif cmd in ["polyline", "polygon"]:
+                points = [f"({x}, {y})" for x, y in chunks(tparams, 2)]
+                if cmd == "polygon":
+                    points.append("cycle")
                 s += " -- ".join(points)
-            # circle and ellipse does not use the transformed parameters
-            elif cmd == 'circle':
-                s += "(%s,%s) circle (%s)" % params
-                closed_path = True
-            elif cmd == 'ellipse':
-                s += "(%s,%s) ellipse (%s and %s)" % params
-                closed_path = True
-            elif cmd == 'image':
-                closed_path = False;
-                pic += "\\node[anchor=north west,inner sep=0, scale=\globalscale] (image) at (%s,%s) {\includegraphics[width=%spt,height=%spt]{%s}}" % params;
+            elif cmd == "circle":
+                s += f"({tparams[0]}, {tparams[1]}) circle ({tparams[2]})"
+            elif cmd == "ellipse":
+                s += f"({tparams[0]}, {tparams[1]}) ellipse ({tparams[2]} and {tparams[3]})"
+            elif cmd == "image":
+                pic += (
+                    rf"\\node[anchor=north west,inner sep=0, scale=\globalscale]"
+                    f" (image) at ({params[0]}, {params[1]}) "
+                    + r"{\includegraphics[width="
+                    f"{params[2]}pt,height={params[3]}pt]" + "{" + f"{params[4]}" + "}"
+                )
         #                 pic += "\draw (%s,%s) node[below right]  {\includegraphics[width=%spt,height=%spt]{%s}}" % params;
 
         if options:
-            optionscode = "[%s]" % ','.join(options)
+            optionscode = f"[{','.join(options)}]"
         else:
             optionscode = ""
 
-        if (s != ''):
-            pathcode = "\\path%s %s;" % (optionscode, s)
-        if (pic != ''):
-            imagecode = "%s;" % (pic)
+        if s != "":
+            pathcode = f"\\path{optionscode} {s};"
+        if pic != "":
+            imagecode = f"{pic};"
         if self.options.wrap:
-            pathcode = "\n".join(wrap(pathcode, 80, subsequent_indent="  ", break_long_words=False))
-            imagecode = "\n".join(wrap(imagecode, 80, subsequent_indent="  ", break_long_words=False))
+            pathcode = "\n".join(
+                wrap(pathcode, 80, subsequent_indent="  ", break_long_words=False)
+            )
+            imagecode = "\n".join(
+                wrap(imagecode, 80, subsequent_indent="  ", break_long_words=False)
+            )
         if self.options.indent:
-            pathcode = "\n".join([self.text_indent + line for line in pathcode.splitlines(False)]) + "\n"
-            imagecode = "\n".join([self.text_indent + line for line in imagecode.splitlines(False)]) + "\n"
+            pathcode = (
+                "\n".join(
+                    [self.text_indent + line for line in pathcode.splitlines(False)]
+                )
+                + "\n"
+            )
+            imagecode = (
+                "\n".join(
+                    [self.text_indent + line for line in imagecode.splitlines(False)]
+                )
+                + "\n"
+            )
         if self.options.verbose and node_id:
-            pathcode = "%s%% %s\n%s\n" % (self.text_indent, node_id, pathcode)
-            imagecode = "%s%% %s\n%s\n" % (self.text_indent, node_id, imagecode)
-        return pathcode + '\n' + imagecode + '\n';
+            pathcode = f"{self.text_indent}% {node_id}\n{pathcode}\n"
+            imagecode = f"{self.text_indent}% {node_id}\n{imagecode}\n"
+        return pathcode + "\n" + imagecode + "\n"
 
     def get_text(self, node):
         """Return content of a text node as string"""
-        # For recent versions of lxml we can simply write:
-        # return etree.tostring(node,method="text")
-        text = ""
-        if node.text is not None:
-            text += node.text
-        for child in node:
-            text += self.get_text(child)
-        if node.tail:
-            text += node.tail
-        return text
+        return etree.tostring(node, method="text").decode("utf-8")
 
     def _output_group(self, group, accumulated_state=None):
         """Process a group of SVG nodes and return corresponding TikZ code
 
         The group is processed recursively if it contains sub groups.
         """
-        s = ""
+        string = ""
         options = []
-        transform = []
+        # transform = []
         for node in group:
             pathdata = None
             options = []
             graphics_state = GraphicsState(node)
-            node_id = node.get('id')
-
+            # node_id = node.get("id")
 
-            if node.tag == _ns('path'):
+            if node.tag == _ns("path"):
                 pathdata, options = self._handle_path(node)
 
             # is it a shape?
-            elif node.tag in [_ns('rect'),
-                              _ns('polyline'),
-                              _ns('polygon'),
-                              _ns('line'),
-                              _ns('circle'),
-                              _ns('ellipse'), ]:
+            elif node.tag in [
+                _ns("rect"),
+                _ns("polyline"),
+                _ns("polygon"),
+                _ns("line"),
+                _ns("circle"),
+                _ns("ellipse"),
+            ]:
                 shapedata, options = self._handle_shape(node)
                 if shapedata:
                     pathdata = [shapedata]
-            elif node.tag == _ns('image'):
+            elif node.tag == _ns("image"):
                 # pathdata, options = self._handle_image(node)
                 imagedata, options = self._handle_image(node)
                 if imagedata:
                     pathdata = [imagedata]
 
             # group node
-            elif node.tag == _ns('g'):
-                s += self._handle_group(node, graphics_state, accumulated_state)
+            elif node.tag == _ns("g"):
+                string += self._handle_group(node, graphics_state, accumulated_state)
                 continue
 
-            elif node.tag == _ns('text') or node.tag == _ns('flowRoot'):
+            elif node.tag == _ns("text") or node.tag == _ns("flowRoot"):
                 pathdata, options = self._handle_text(node)
 
-            elif node.tag == _ns('use'):
-                s += self._handle_use(node, graphics_state, accumulated_state)
+            elif node.tag == _ns("use"):
+                string += self._handle_use(node, graphics_state, accumulated_state)
 
-            # TODO: handle symbol as reusable code ?
+            # to implement: handle symbol as reusable code
             elif node.tag == _ns("symbol"):
-                s += self._handle_group(node, graphics_state, accumulated_state)
+                string += self._handle_group(node, graphics_state, accumulated_state)
 
             else:
                 logging.debug("Unhandled element %s", node.tag)
 
-            goptions, transformation = self.convert_svgstate_to_tikz(graphics_state, accumulated_state, node)
+            goptions, transformation = self.convert_svgstate_to_tikz(
+                graphics_state, accumulated_state, node
+            )
             options = transformation + goptions + options
-            s += self._write_tikz_path(pathdata, options, node)
-        return s
+            string += self._write_tikz_path(pathdata, options, node)
+        return string
 
     def effect(self):
-        s = ""
-        nodes = self.selected_sorted
-        # If no nodes is selected convert whole document.
+        """Apply the conversion on the svg and fill the template"""
+        string = ""
+        if self.inkscape_mode:
+            nodes = self.svg.selected
+        else:
+            nodes = self.selected_sorted
 
+        # If no nodes is selected convert whole document.
 
-        self.height = 0
         root = self.document.getroot()
         if "height" in root.attrib:
             self.height = self.convert_unit(root.attrib["height"])
         if len(nodes) == 0:
             nodes = self.document.getroot()
             graphics_state = GraphicsState(nodes)
         else:
             graphics_state = GraphicsState(None)
-        goptions, transformation = self.convert_svgstate_to_tikz(graphics_state, graphics_state,
-                                                                 self.document.getroot())
+        goptions, transformation = self.convert_svgstate_to_tikz(
+            graphics_state, graphics_state, self.document.getroot()
+        )
         options = transformation + goptions
         # Recursively process list of nodes or root node
-        s = self._output_group(nodes, graphics_state)
+        string = self._output_group(nodes, graphics_state)
 
         # Add necessary boiling plate code to the generated TikZ code.
         codeoutput = self.options.codeoutput
         if len(options) > 0:
-            extraoptions = ',\n%s' % ','.join(options)
+            extraoptions = f",\n{','.join(options)}"
         else:
-            extraoptions = ''
+            extraoptions = ""
         if not self.options.crop:
             cropcode = ""
         else:
             cropcode = CROP_TEMPLATE
-        if codeoutput == 'standalone':
-            output = STANDALONE_TEMPLATE % dict(pathcode=s,
-                                                unit=self.options.output_unit,
-                                                colorcode=self.color_code,
-                                                cropcode=cropcode,
-                                                extraoptions=extraoptions,
-                                                gradientcode=self.gradient_code,
-                                                scale=self.options.scale)
-        elif codeoutput == 'figonly':
-            output = FIG_TEMPLATE % dict(pathcode=s,
-                                         colorcode=self.color_code,
-                                         unit=self.options.output_unit,
-                                         extraoptions=extraoptions,
-                                         gradientcode=self.gradient_code,
-                                         scale=self.options.scale)
+        if codeoutput == "standalone":
+            output = STANDALONE_TEMPLATE % {
+                "pathcode": string,
+                "colorcode": self.color_code,
+                "unit": self.options.output_unit,
+                "ysign": "-" if self.options.noreversey else "",
+                "cropcode": cropcode,
+                "extraoptions": extraoptions,
+                "gradientcode": self.gradient_code,
+                "scale": self.options.scale,
+            }
+        elif codeoutput == "figonly":
+            output = FIG_TEMPLATE % {
+                "pathcode": string,
+                "colorcode": self.color_code,
+                "unit": self.options.output_unit,
+                "ysign": "-" if self.options.noreversey else "",
+                "extraoptions": extraoptions,
+                "gradientcode": self.gradient_code,
+                "scale": self.options.scale,
+            }
         else:
-            output = s
+            output = string
 
         self.output_code = output
         if self.options.returnstring:
             return output
+        return ""
 
-    def save_raw(self, output_code):
+    def save_raw(self, _):
+        """Save the file from the save as menu from inkscape"""
         if self.options.clipboard:
-            success = copy_to_clipboard(self.output_code.encode('utf8'))
+            success = copy_to_clipboard(self.output_code.encode("utf8"))
             if not success:
-                logging.error('Failed to put output on clipboard')
-        if self.options.mode == 'effect':
-            if self.options.outputfile and not self.options.clipboard:
-                print(self.options.outputfile)
-                f = codecs.open(self.options.outputfile, 'w', 'utf8')
-                f.write(self.output_code)
-                f.close()
+                logging.error("Failed to put output on clipboard")
+
+        if self.options.mode == "effect":
+            if self.options.output and not self.options.clipboard:
+                with codecs.open(self.options.output, "w", "utf8") as file:
+                    file.write(self.output_code)
                 # Serialize document into XML on stdout
-            self.document.write(sys.stdout.buffer)
 
-        if self.options.mode == 'output':
-            print(self.output_code.encode('utf8'))
+            # Not sure this is needed
+            else:
+                self.document.write(sys.stdout.buffer)
+
+        if self.options.mode == "output":
+            print(self.output_code)
 
     def convert(self, svg_file, cmd_line_mode=False, **kwargs):
+        """Convert SVG file to tikz path"""
         self.options = self.arg_parser.parse_args()
 
         if self.options.printversion:
             print_version_info()
-            return
+            return ""
+
         self.options.returnstring = True
         self.options.__dict__.update(kwargs)
         if self.options.scale is None:
             self.options.scale = 1
         if cmd_line_mode:
             if self.options.input_file is not None and len(self.options.input_file) > 0:
                 if os.path.exists(self.options.input_file):
                     svg_file = self.options.input_file
                 else:
-                    logging.error('Input file %s does not exists', self.args[0])
-                    return
+                    logging.error("Input file %s does not exists", self.args[0])
+                    return ""
             else:
                 # Correct ?
-                logging.error('No file were specified')
-                return
+                logging.error("No file were specified")
+                return ""
 
         self.parse(svg_file)
-        self.getselected()
+        self.get_selected()
         self.svg.get_ids()
         output = self.effect()
         if self.options.clipboard:
-            success = copy_to_clipboard(self.output_code.encode('utf8'))
+            success = copy_to_clipboard(self.output_code.encode("utf8"))
             if not success:
-                logging.error('Failed to put output on clipboard')
+                logging.error("Failed to put output on clipboard")
             output = ""
 
-        if self.options.outputfile:
-            f = codecs.open(self.options.outputfile, 'w', 'utf8')
-            f.write(self.output_code)
-            f.close()
-            output = ""
+        if self.options.output:
+            with codecs.open(self.options.output, "w", "utf8") as file:
+                file.write(self.output_code)
+                output = ""
 
         return output
 
 
 def convert_file(svg_file, **kwargs):
+    """Convert SVG file to tikz code"""
     effect = TikZPathExporter(inkscape_mode=False)
     return effect.convert(svg_file, **kwargs)
 
 
 def convert_svg(svg_source, **kwargs):
+    """Convert any SVG source to tikz code"""
     effect = TikZPathExporter(inkscape_mode=False)
     source = open_anything(svg_source)
     tikz_code = effect.convert(source.read(), **kwargs)
     source.close()
     return tikz_code
 
 
@@ -1592,20 +1836,21 @@
     """Inkscape interface"""
     # Create effect instance and apply it.
     effect = TikZPathExporter(inkscape_mode=True)
     effect.run()
 
 
 def print_version_info():
-    print("svg2tikz version % s" % __version__)
+    """Print the version of svg2tikz"""
+    print(f"svg2tikz version {__version__}")
 
 
 def main_cmdline(**kwargs):
     """Main command line interface"""
     effect = TikZPathExporter(inkscape_mode=False)
     tikz_code = effect.convert(svg_file=None, cmd_line_mode=True, **kwargs)
     if tikz_code:
         print(tikz_code)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main_inkscape()
```

