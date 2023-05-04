# Comparing `tmp/pretext-1.5.3.dev20230503.tar.gz` & `tmp/pretext-1.5.3.dev20230504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230503.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230504.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230503.tar` & `pretext-1.5.3.dev20230504.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/README.md
--rw-r--r--   0        0        0     1440 2023-05-03 06:19:02.091902 pretext-1.5.3.dev20230503/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/core/__init__.py
--rw-r--r--   0        0        0   173946 2023-05-03 06:19:07.099965 pretext-1.5.3.dev20230503/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/core/resources.py
--rw-r--r--   0        0        0  1049746 2023-05-03 06:19:07.099965 pretext-1.5.3.dev20230503/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-03 06:18:25.851449 pretext-1.5.3.dev20230503/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-03 06:18:25.855449 pretext-1.5.3.dev20230503/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-03 06:18:25.855449 pretext-1.5.3.dev20230503/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-03 06:19:07.143966 pretext-1.5.3.dev20230503/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-03 06:19:07.163966 pretext-1.5.3.dev20230503/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-03 06:19:07.159966 pretext-1.5.3.dev20230503/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-03 06:19:07.163966 pretext-1.5.3.dev20230503/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-03 06:19:07.167966 pretext-1.5.3.dev20230503/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-03 06:18:25.855449 pretext-1.5.3.dev20230503/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-03 06:19:02.095902 pretext-1.5.3.dev20230503/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230503/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-04 06:18:25.287603 pretext-1.5.3.dev20230504/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-04 06:18:25.287603 pretext-1.5.3.dev20230504/README.md
+-rw-r--r--   0        0        0     1440 2023-05-04 06:19:14.204128 pretext-1.5.3.dev20230504/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/core/__init__.py
+-rw-r--r--   0        0        0   173946 2023-05-04 06:19:19.480521 pretext-1.5.3.dev20230504/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/core/resources.py
+-rw-r--r--   0        0        0  1053177 2023-05-04 06:19:19.480521 pretext-1.5.3.dev20230504/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-04 06:19:19.540525 pretext-1.5.3.dev20230504/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-04 06:19:19.564527 pretext-1.5.3.dev20230504/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-04 06:19:19.560527 pretext-1.5.3.dev20230504/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-04 06:19:19.568527 pretext-1.5.3.dev20230504/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-04 06:19:14.204128 pretext-1.5.3.dev20230504/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230504/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230503/LICENSE` & `pretext-1.5.3.dev20230504/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/README.md` & `pretext-1.5.3.dev20230504/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/__init__.py` & `pretext-1.5.3.dev20230504/pretext/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = 'ac678fb59bbd8e8640e39034258b8a20d027f687'
+CORE_COMMIT = 'f509db302370e65a3da303230e4ce7cd03c3fb8d'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230503/pretext/build.py` & `pretext-1.5.3.dev20230504/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/cli.py` & `pretext-1.5.3.dev20230504/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/codechat.py` & `pretext-1.5.3.dev20230504/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230504/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/core/pretext.py` & `pretext-1.5.3.dev20230504/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/core/resources.py` & `pretext-1.5.3.dev20230504/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/core/resources.zip` & `pretext-1.5.3.dev20230504/pretext/core/resources.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 1049746 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/utilities/
--rw-r--r--  2.0 unx    11766 b- defN 23-May-03 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx   262590 b- defN 23-May-03 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-03 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-03 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-03 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-03 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-03 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-May-03 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-03 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-03 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-03 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    69315 b- defN 23-May-03 06:19 xsl/pretext-braille.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-03 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   544147 b- defN 23-May-03 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    55600 b- defN 23-May-03 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-03 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-03 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-03 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-03 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-03 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-03 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139661 b- defN 23-May-03 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-03 06:19 xsl/README.md
--rw-r--r--  2.0 unx     2740 b- defN 23-May-03 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   608699 b- defN 23-May-03 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-May-03 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx     2846 b- defN 23-May-03 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-03 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-03 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-03 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   541182 b- defN 23-May-03 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-03 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-03 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    39922 b- defN 23-May-03 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-03 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-03 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-03 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-03 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-03 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-03 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-May-03 06:19 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-May-03 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-03 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-May-03 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-03 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    17285 b- defN 23-May-03 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-03 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-May-03 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-03 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-03 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-03 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-03 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-03 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-03 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-03 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx     2227 b- defN 23-May-03 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-03 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-03 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-03 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-May-03 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-03 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-03 06:19 xsl/localizations/pt-PT.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx     5800 b- defN 23-May-03 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-03 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-03 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-May-03 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-May-03 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx      486 b- defN 23-May-03 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5241 b- defN 23-May-03 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-May-03 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-May-03 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-May-03 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     3024 b- defN 23-May-03 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-03 06:19 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-03 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-03 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-03 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx   133917 b- defN 23-May-03 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx   124561 b- defN 23-May-03 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-May-03 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx      326 b- defN 23-May-03 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    57960 b- defN 23-May-03 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-May-03 06:19 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 23-May-03 06:19 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-May-03 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    25290 b- defN 23-May-03 06:19 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-May-03 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   101402 b- defN 23-May-03 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx     2446 b- defN 23-May-03 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-03 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-03 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-03 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     1280 b- defN 23-May-03 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-03 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-03 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-03 06:19 css/setcolors.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-03 06:19 css/README.md
--rw-r--r--  2.0 unx     4021 b- defN 23-May-03 06:19 css/update_css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-03 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-03 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-03 06:19 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-03 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-03 06:19 css/style_default.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-03 06:19 css/epub.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-03 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-03 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-03 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-03 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-03 06:19 css/kindle.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-03 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1276 b- defN 23-May-03 06:19 css/colors_maroon_grey.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 script/braille/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-03 06:19 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-03 06:19 script/mbx
--rw-r--r--  2.0 unx     2573 b- defN 23-May-03 06:19 script/braille/pretext-symbol.dis
--rw-r--r--  2.0 unx     8913 b- defN 23-May-03 06:19 script/braille/pretext.sem
--rw-r--r--  2.0 unx      735 b- defN 23-May-03 06:19 script/braille/README.md
--rw-r--r--  2.0 unx     6616 b- defN 23-May-03 06:19 script/braille/pretext-liblouis.cfg
--rw-r--r--  2.0 unx     1011 b- defN 23-May-03 06:19 script/braille/pretext-liblouis-emboss.cfg
--rw-r--r--  2.0 unx      490 b- defN 23-May-03 06:19 script/braille/pretext-liblouis-electronic.cfg
--rw-r--r--  2.0 unx      481 b- defN 23-May-03 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-May-03 06:19 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-May-03 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx     2566 b- defN 23-May-03 06:19 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-May-03 06:19 pretext/README.md
--rw-r--r--  2.0 unx   173946 b- defN 23-May-03 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx    29600 b- defN 23-May-03 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-03 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx    31361 b- defN 23-May-03 06:19 pretext/pretext
-148 files, 4868819 bytes uncompressed, 1031322 bytes compressed:  78.8%
+Zip file size: 1053177 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/utilities/
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-04 06:19 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx   262590 b- defN 23-May-04 06:19 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-04 06:19 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-04 06:19 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-04 06:19 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-04 06:19 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-04 06:19 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-04 06:19 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-04 06:19 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-04 06:19 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-04 06:19 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    69315 b- defN 23-May-04 06:19 xsl/pretext-braille.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-04 06:19 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   544147 b- defN 23-May-04 06:19 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    64782 b- defN 23-May-04 06:19 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-04 06:19 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-04 06:19 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-04 06:19 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-04 06:19 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-04 06:19 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-04 06:19 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139661 b- defN 23-May-04 06:19 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-04 06:19 xsl/README.md
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-04 06:19 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   608699 b- defN 23-May-04 06:19 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-04 06:19 xsl/entities.ent
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-04 06:19 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-04 06:19 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-04 06:19 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-04 06:19 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   541182 b- defN 23-May-04 06:19 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-04 06:19 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-04 06:19 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    39922 b- defN 23-May-04 06:19 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-04 06:19 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-04 06:19 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-04 06:19 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-04 06:19 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-04 06:19 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-04 06:19 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-04 06:19 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-May-04 06:19 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-04 06:19 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-04 06:19 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-04 06:19 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-04 06:19 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-04 06:19 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-04 06:19 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-04 06:19 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-04 06:19 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-04 06:19 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-04 06:19 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-04 06:19 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-04 06:19 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-04 06:19 xsl/localizations/README.md
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-04 06:19 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-04 06:19 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-04 06:19 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-04 06:19 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-04 06:19 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-04 06:19 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-04 06:19 xsl/localizations/pt-PT.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-04 06:19 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-04 06:19 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-04 06:19 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-04 06:19 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-May-04 06:19 xsl/support/README.md
+-rw-r--r--  2.0 unx      486 b- defN 23-May-04 06:19 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-04 06:19 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-May-04 06:19 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-04 06:19 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-04 06:19 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx   133917 b- defN 23-May-04 06:19 schema/pretext.xml
+-rw-r--r--  2.0 unx   124561 b- defN 23-May-04 06:19 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-04 06:19 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx      326 b- defN 23-May-04 06:19 schema/xml.xsd
+-rw-r--r--  2.0 unx    57960 b- defN 23-May-04 06:19 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-04 06:19 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-04 06:19 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-04 06:19 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-04 06:19 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-04 06:19 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   101402 b- defN 23-May-04 06:19 schema/pretext.rng
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-04 06:19 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-04 06:19 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-04 06:19 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-04 06:19 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-04 06:19 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-04 06:19 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-04 06:19 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-04 06:19 css/setcolors.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-04 06:19 css/README.md
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-04 06:19 css/update_css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-04 06:19 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-04 06:19 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-04 06:19 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-04 06:19 css/style_default.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-04 06:19 css/epub.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-04 06:19 css/colors_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-04 06:19 css/style_soundwriting.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-04 06:19 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-04 06:19 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-04 06:19 css/kindle.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-04 06:19 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-04 06:19 css/colors_maroon_grey.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/braille/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-04 06:19 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-04 06:19 script/mbx
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-04 06:19 script/braille/pretext-symbol.dis
+-rw-r--r--  2.0 unx     8913 b- defN 23-May-04 06:19 script/braille/pretext.sem
+-rw-r--r--  2.0 unx      735 b- defN 23-May-04 06:19 script/braille/README.md
+-rw-r--r--  2.0 unx     6616 b- defN 23-May-04 06:19 script/braille/pretext-liblouis.cfg
+-rw-r--r--  2.0 unx     1011 b- defN 23-May-04 06:19 script/braille/pretext-liblouis-emboss.cfg
+-rw-r--r--  2.0 unx      490 b- defN 23-May-04 06:19 script/braille/pretext-liblouis-electronic.cfg
+-rw-r--r--  2.0 unx      481 b- defN 23-May-04 06:19 script/mjsre/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 06:19 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-04 06:19 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-May-04 06:19 script/mjsre/package.json
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-04 06:19 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-04 06:19 pretext/README.md
+-rw-r--r--  2.0 unx   173946 b- defN 23-May-04 06:19 pretext/pretext.py
+-rw-r--r--  2.0 unx    34807 b- defN 23-May-04 06:19 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 06:19 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-04 06:19 pretext/module-test.py
+-rw-r--r--  2.0 unx    31361 b- defN 23-May-04 06:19 pretext/pretext
+148 files, 4883208 bytes uncompressed, 1034753 bytes compressed:  78.8%
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -29,15 +29,28 @@
 <!-- derivatives, such as HTML destined for EPUB output -->
 <!-- xmlns="http://www.w3.org/1999/xhtml"               -->
 <xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:pi="http://pretextbook.org/2020/pretext/internal" xmlns:exsl="http://exslt.org/common" xmlns:date="http://exslt.org/dates-and-times" xmlns:str="http://exslt.org/strings" version="1.0" extension-element-prefixes="pi exsl date str">
   <!-- Standard conversion groundwork -->
   <xsl:import href="./publisher-variables.xsl"/>
   <xsl:import href="./pretext-assembly.xsl"/>
   <xsl:import href="./pretext-common.xsl"/>
-  <xsl:output method="xml" indent="yes" encoding="UTF-8"/>
+  <!-- With @indent="yes" the (intermediate) file is much easier to study    -->
+  <!-- and debug, but it introduces whitespace we can not (or do not want    -->
+  <!-- to) control for.  The situation is a single isolated sentence that    -->
+  <!-- is entirely a font change.  Here "isolated" means it becomes an       -->
+  <!-- entire "segment", such as being between two "displays" when breaking  -->
+  <!-- up a paragraph.  For example, an entire sentence could be in italics, -->
+  <!-- thus leading to a "segment" with a child "italic" and nothing else.   -->
+  <!-- The indentation provided introduces whitespace where we are expecting -->
+  <!-- mixed content.  In old parlance, we expect a "segment" to be "tight". -->
+  <!-- We saw this just twice in all of AATA (2023-04-07) where a lone "m"   -->
+  <!-- (plus absorbed punctuation) was caught between displays in a          -->
+  <!-- paragraph, and the whitespace bled into a diff when the previous      -->
+  <!-- commit led to the @indent suddenly being effective.                   -->
+  <xsl:output method="xml" indent="no" encoding="UTF-8"/>
   <xsl:variable name="exercise-style" select="'static'"/>
   <!-- Not so much "include" as "manipulate"            -->
   <xsl:param name="math.punctuation.include" select="'all'"/>
   <!-- ############################## -->
   <!-- Incorporate (Meld) Mathematics -->
   <!-- ############################## -->
   <!-- We do a pass (similar to those in the "pretext-assembly.xsl"   -->
@@ -149,14 +162,55 @@
       <xsl:apply-templates select="@*" mode="meld-runin"/>
       <xsl:apply-templates select="$adjacent-runin/@indentation|$adjacent-runin/@lines-before" mode="meld-runin"/>
       <xsl:apply-templates select="$adjacent-runin/node()" mode="meld-runin"/>
       <xsl:value-of select="$adjacent-runin/@separator"/>
       <xsl:apply-templates select="node()" mode="meld-runin"/>
     </xsl:copy>
   </xsl:template>
+  <!-- It is entirely possible for a segment to be preceded by     -->
+  <!-- consecutive "runin" elements.  Three examples:              -->
+  <!--                                                             -->
+  <!--   "proof" then "case"                                       -->
+  <!--   "hint" then "li" (and other SOLUTION-LIKE)                -->
+  <!--   "exercise" then "li" (but should probably be "task"?)     -->
+  <!--                                                             -->
+  <!-- Likely a structure with an immediate "p" with an immediate  -->
+  <!-- list could result in a run-in title for the structure and   -->
+  <!-- a run-in title for the first list item.  Experimentation on -->
+  <!-- 2023-04-05 with Judson's AATA did not reveal any runs of    -->
+  <!-- three (or more) consecutive "runin" elements.  So our       -->
+  <!-- solution is ad-hoc for the double case, with a bug report   -->
+  <!-- for three or more.                                          -->
+  <!-- We convert the first "runin" to a "segment" (rather than    -->
+  <!-- killing it) and let the second "runin" get absorbed by the  -->
+  <!-- subsequent "segment".                                       -->
+  <xsl:template match="runin[following-sibling::*[1][self::runin]]" mode="meld-runin">
+    <segment>
+      <xsl:apply-templates select="@*|node()" mode="meld-runin"/>
+    </segment>
+    <xsl:if test="following-sibling::*[2][self::runin]">
+      <xsl:message>BUG: the braille conversion has encountered three &quot;run-in&quot; titles in a row,</xsl:message>
+      <xsl:message>which we had not expected.  Please report me.  Thank-you.</xsl:message>
+      <xsl:message>
+        First:
+        <xsl:value-of select="."/>
+      </xsl:message>
+      <xsl:message>
+        Second:
+        <xsl:value-of select="following-sibling::*[1][self::runin]"/>
+      </xsl:message>
+      <xsl:message>
+        Third:
+        <xsl:value-of select="following-sibling::*[2][self::runin]"/>
+      </xsl:message>
+    </xsl:if>
+  </xsl:template>
+  <!-- Every "runin" has been absorbed into a trailing "segment" or -->
+  <!-- perhaps converted into a "segment".  This will prevent the   -->
+  <!-- absorbed ones from persisting.                               -->
   <xsl:template match="runin" mode="meld-runin"/>
   <!-- Xerox machine -->
   <xsl:template match="@*|node()" mode="meld-runin">
     <xsl:copy>
       <xsl:apply-templates select="@*|node()" mode="meld-runin"/>
     </xsl:copy>
   </xsl:template>
@@ -323,14 +377,20 @@
             <xsl:text>0</xsl:text>
           </xsl:when>
           <xsl:when test="$heading-style = 'cell7'">
             <xsl:text>0</xsl:text>
           </xsl:when>
         </xsl:choose>
       </xsl:attribute>
+      <!-- division headings go to the Table of Contents -->
+      <xsl:attribute name="heading-id">
+        <xsl:apply-templates select="." mode="internal-id"/>
+      </xsl:attribute>
+      <!-- TODO: record heading levels for indentation/runover in ToC -->
+      <!--  -->
       <!-- Finally, the heading content itself -->
       <xsl:variable name="the-number">
         <xsl:apply-templates select="." mode="number"/>
       </xsl:variable>
       <xsl:if test="not($the-number = '')">
         <xsl:value-of select="$the-number"/>
         <xsl:text/>
@@ -448,15 +508,15 @@
   <!--                                                              -->
   <!-- We handle the title as a heading of sorts, which might not   -->
   <!-- cross a page boundary, and which might be "stuck" on a       -->
   <!-- certain number of following lines.  See the discussion below -->
   <!-- about titles.                                                -->
   <!-- "Regular" blocks, including inline "exercise" (aka "Checkpoint") -->
   <xsl:template match="|||||||||exercise[]">
-    <block box="standard" lines-before="1" lines-after="1">
+    <block breakable="no" box="standard" lines-before="1" lines-after="1">
       <xsl:apply-templates select="." mode="block-title"/>
       <xsl:apply-templates select="*[not(self::title)]"/>
     </block>
   </xsl:template>
   <!-- "Other" exercises (in "exercises" divisions, in "reading questions", -->
   <!-- in worksheets) are not as prominent and have run-in titles           -->
   <xsl:template match="exercise[not()]">
@@ -466,14 +526,21 @@
   <!-- The appendages are not yet blocks, they live inside blocks           -->
   <!-- NOTE: if these become contained blocks, that is a structural change  -->
   <!-- that will require changes in the Python lxml which assumes otherwise -->
   <xsl:template match="||">
     <xsl:apply-templates select="." mode="block-title"/>
     <xsl:apply-templates select="*[not(self::title)]"/>
   </xsl:template>
+  <!-- A "case" is a further division of a PROOF-LIKE -->
+  <xsl:template match="case">
+    <runin indentation="2" separator="  ">
+      <xsl:apply-templates select="." mode="title-full"/>
+    </runin>
+    <xsl:apply-templates select="*"/>
+  </xsl:template>
   <!-- Titles of blocks can be an entire "segment" if they finish with a  -->
   <!-- newline.  Other titles are "runin" and are consolidated in a final -->
   <!-- post-processing step.                                              -->
   <xsl:template match="|||||||||exercise[]" mode="block-title">
     <segment lines-before="0">
       <!--  -->
       <xsl:apply-templates select="." mode="type-name"/>
@@ -548,43 +615,64 @@
       <!--  -->
     </runin>
   </xsl:template>
   <!-- TODO: GOAL-LIKE -->
   <!-- ########### -->
   <!-- FIGURE-LIKE -->
   <!-- ########### -->
-  <!-- Figures are only implemented for the case where their contents are   -->
+  <!-- [BANA, 2016] 6.2.2(e) -->
+  <!-- When both a print caption and a transcriber-generated description    -->
+  <!-- are needed, begin the description (enclosed in transcriber's note    -->
+  <!-- indicators) on the line following the caption.                       -->
+  <!-- Figures are treated different for the case where their contents are  -->
   <!-- images (thus requiring a tactile graphic page to follow the figure). -->
   <xsl:template match="figure[image]">
-    <block box="standard">
-      <xsl:apply-templates select="image" mode="braille-representation"/>
+    <block breakable="no" box="standard">
       <segment>
         <xsl:apply-templates select="." mode="block-title"/>
       </segment>
+      <xsl:apply-templates select="*[not(self::image)]"/>
+      <xsl:apply-templates select="image" mode="braille-representation"/>
     </block>
     <!-- Form a page to be replaced by tactile version -->
     <segment ownpage="yes">
       <xsl:apply-templates select="." mode="block-title"/>
     </segment>
   </xsl:template>
-  <!-- Caption, with label, number, etc.  "caption" element   -->
-  <!-- is metadata, killed in -common, obtained as needed via -->
-  <!-- modal template (much like a title).                    -->
-  <xsl:template match="figure" mode="block-title">
+  <!-- Other FIGURE-LIKE can be handled together -->
+  <xsl:template match="figure|listing|table|list">
+    <block breakable="no" box="standard">
+      <segment>
+        <xsl:apply-templates select="." mode="block-title"/>
+      </segment>
+      <xsl:apply-templates/>
+    </block>
+  </xsl:template>
+  <!-- Caption/title, with label, number, etc.  "caption" and -->
+  <!-- "title" elements are metadata, killed in -common,      -->
+  <!-- obtained as needed via modal templates.                -->
+  <xsl:template match="figure|listing|table|list" mode="block-title">
     <xsl:apply-templates select="." mode="type-name"/>
     <!--  -->
     <xsl:variable name="the-number">
       <xsl:apply-templates select="." mode="number"/>
     </xsl:variable>
     <xsl:if test="not($the-number = '')">
       <xsl:text/>
       <xsl:value-of select="$the-number"/>
     </xsl:if>
     <xsl:text>.</xsl:text>
-    <xsl:apply-templates select="." mode="caption-full"/>
+    <xsl:choose>
+      <xsl:when test="self::figure|self::listing">
+        <xsl:apply-templates select="." mode="caption-full"/>
+      </xsl:when>
+      <xsl:when test="self::table|self::list">
+        <xsl:apply-templates select="." mode="title-full"/>
+      </xsl:when>
+    </xsl:choose>
   </xsl:template>
   <!-- ###### -->
   <!-- Images -->
   <!-- ###### -->
   <!-- A bare image becomes a transcriber note with a small amount -->
   <!-- of identification, and then generates a replacement page.   -->
   <xsl:template match="image">
@@ -681,14 +769,107 @@
   <!-- A "stack" is strictly a side-by-side panel and we just -->
   <!-- process its children.  No need to get carried away for -->
   <!-- braille, and maybe an "apply-imports" (or nothing at   -->
   <!-- all) is the right thing to do.                         -->
   <xsl:template match="stack">
     <xsl:apply-templates select="*"/>
   </xsl:template>
+  <!-- ##### -->
+  <!-- Lists -->
+  <!-- ##### -->
+  <!-- Lists are containers full of list items.  All by   -->
+  <!-- themselves they have no real impact on the braille -->
+  <!-- output.  The list items are another matter.        -->
+  <!-- 2023-04-06: very prelimnary, e.g. no runover       -->
+  <xsl:template match="ul|ol|dl">
+    <!-- <segment>LIST</segment> -->
+    <xsl:apply-templates select="li"/>
+  </xsl:template>
+  <xsl:template match="li">
+    <!-- Marker as a "runin" element -->
+    <runin indentation="0" separator="  ">
+      <xsl:choose>
+        <xsl:when test="parent::ol">
+          <xsl:apply-templates select="." mode="item-number"/>
+          <xsl:text>.</xsl:text>
+        </xsl:when>
+        <xsl:when test="parent::ul">
+          <xsl:apply-templates select="." mode="unicode-list-marker"/>
+          <xsl:text>.</xsl:text>
+        </xsl:when>
+        <xsl:when test="parent::dl">
+          <xsl:apply-templates select="." mode="title-full"/>
+        </xsl:when>
+      </xsl:choose>
+    </runin>
+    <xsl:apply-templates select="node()"/>
+  </xsl:template>
+  <xsl:template match="ul/li" mode="unicode-list-marker">
+    <xsl:variable name="format-code">
+      <xsl:apply-templates select="parent::ul" mode="format-code"/>
+    </xsl:variable>
+    <!-- The list label.  The file  en-ueb-chardefs.uti        -->
+    <!-- associates these Unicode values with the indicated    -->
+    <!-- dot patterns.  This jibes with [BANA-2016, 8.6.2],    -->
+    <!-- which says the open circle needs a Grade 1 indicator. -->
+    <!-- The file  en-ueb-g2.ctb  lists  x25cb  and  x24a0  as -->
+    <!-- both being "contraction" and so needing a             -->
+    <!-- Grade 1 indicator.                                    -->
+    <xsl:choose>
+      <!-- Unicode Character 'BULLET' (U+2022)       -->
+      <!-- Dot pattern: 456-256                      -->
+      <xsl:when test="$format-code = 'disc'">
+        <xsl:text>•</xsl:text>
+      </xsl:when>
+      <!-- Unicode Character 'WHITE CIRCLE' (U+25CB) -->
+      <!-- Dot pattern: 1246-123456                  -->
+      <xsl:when test="$format-code = 'circle'">
+        <xsl:text>○</xsl:text>
+      </xsl:when>
+      <!-- Unicode Character 'BLACK SQUARE' (U+25A0) -->
+      <!-- Dot pattern: 456-1246-3456-145            -->
+      <xsl:when test="$format-code = 'square'">
+        <xsl:text>■</xsl:text>
+      </xsl:when>
+      <!-- a bad idea for Braille -->
+      <xsl:when test="$format-code = 'none'">
+        <xsl:text/>
+      </xsl:when>
+    </xsl:choose>
+  </xsl:template>
+  <!-- ########## -->
+  <!-- References -->
+  <!-- ########## -->
+  <!-- Bibliography [BANA-2016, 22.2.1]                           -->
+  <!-- Bibliographic items in a "references" division have a      -->
+  <!-- bracketed number leading each new entry, then two spaces   -->
+  <!-- of indentation for the remainder .                         -->
+  <!-- TODO: expand to accomodate annotations ("note"), BANA 22.3 -->
+  <xsl:template match="biblio[@type='raw']">
+    <runin indentation="0" separator="  ">
+      <xsl:text>[</xsl:text>
+      <xsl:apply-templates select="." mode="serial-number"/>
+      <xsl:text>]</xsl:text>
+    </runin>
+    <segment indentation="0" runover="2">
+      <xsl:apply-templates/>
+    </segment>
+  </xsl:template>
+  <!-- Override usual killing of title, but perhaps a generic -->
+  <!-- template (without punctuation!) would be saner?        -->
+  <xsl:template match="biblio/title">
+    <italic>
+      <xsl:apply-templates/>
+    </italic>
+  </xsl:template>
+  <xsl:template match="volume">
+    <bold>
+      <xsl:apply-templates/>
+    </bold>
+  </xsl:template>
   <!-- Generators -->
   <xsl:template match="pretext">
     <xsl:text>PreTeXt</xsl:text>
   </xsl:template>
   <xsl:template match="tex">
     <xsl:text>TeX</xsl:text>
   </xsl:template>
@@ -800,23 +981,21 @@
   <xsl:template match="attr">
     <xsl:text>@</xsl:text>
     <xsl:value-of select="."/>
   </xsl:template>
   <!-- #### -->
   <!-- Math -->
   <!-- #### -->
-  <xsl:template match="m">
+  <xsl:template match="m[not(contains(math-nemeth, '
+'))]">
     <!-- Unicode braille cells from Speech Rule Engine (SRE)   -->
     <!-- Not expecting any markup, so "value-of" is everything -->
     <xsl:variable name="raw-braille">
       <xsl:value-of select="math-nemeth"/>
     </xsl:variable>
-    <!-- inline vs. spatial makes a difference -->
-    <xsl:variable name="b-multiline" select="contains($raw-braille, '
-')"/>
     <!-- We investigate actual source for very simple math   -->
     <!-- such as one-letter variable names as Latin letters  -->
     <!-- or positive integers, so we process the orginal     -->
     <!-- content outside of a MathJax/SRE translation (which -->
     <!-- could have "xref", etc)                             -->
     <xsl:variable name="content">
       <xsl:value-of select="math-original/node()"/>
@@ -844,46 +1023,41 @@
       <!-- Test is true for non-negative integers, which we drop into -->
       <!-- the stream as if they were never authored as math anyway   -->
       <xsl:when test="translate($original-content,  ,'') = ''">
         <xsl:value-of select="$original-content"/>
         <!-- restore clause-ending punctuation -->
         <xsl:value-of select="$clause-ending-mark"/>
       </xsl:when>
-      <!-- We construct a fragment for teh Python formatter.   -->
+      <!-- We construct a fragment for the Python formatter.   -->
       <!-- SRE may convert inline "m" into a spatial layout,   -->
       <!-- such as a fraction or column vector authored inline -->
-      <!-- We ignore this situation for now                    -->
-      <xsl:when test="not($b-multiline)">
+      <!-- We treat this elsewhere, more like "md" elements    -->
+      <xsl:otherwise>
         <math>
           <!-- Add punctuation as an attribute conditionally. -->
           <!-- We could probably just add an empty string     -->
           <!-- routinely and push that through to the closing -->
           <!-- Nemeth indicator, but we take a bit more care. -->
           <xsl:if test="not($clause-ending-mark = '')">
             <xsl:attribute name="punctuation">
               <xsl:value-of select="$clause-ending-mark"/>
             </xsl:attribute>
           </xsl:if>
           <xsl:value-of select="$raw-braille"/>
         </math>
-      </xsl:when>
-      <xsl:otherwise>
-        <!-- TEMPORARY: Multi-line case -->
-        <xsl:text>INLINE MATH (RENDERED WITH NEWLINES)</xsl:text>
-        <!-- restore clause-ending punctuation -->
-        <xsl:value-of select="$clause-ending-mark"/>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
-  <xsl:template match="me|men|md|mdn">
+  <xsl:template match="m[contains(math-nemeth, '
+')]|me|men|md|mdn">
     <xsl:variable name="nemeth">
       <xsl:value-of select="math-nemeth"/>
       <xsl:text/>
     </xsl:variable>
-    <block box="nemeth">
+    <block breakable="no" box="nemeth">
       <xsl:attribute name="punctuation">
         <xsl:apply-templates select="." mode="get-clause-punctuation-mark"/>
       </xsl:attribute>
       <xsl:call-template name="segmentize-display-math">
         <xsl:with-param name="display-math" select="$nemeth"/>
       </xsl:call-template>
     </block>
@@ -1012,18 +1186,20 @@
   </xsl:template>
   <!-- Two-dimensional displayed itmes will get their own segment and   -->
   <!-- we will explode the rest of a "p" into pieces that are segments. -->
   <!-- But with indentation only on the first piece.                    -->
   <!-- Note: leading with a display in a "p" means no indentation.      -->
   <!-- Note: this is derived from a similar template in the HTML        -->
   <!-- conversion.                                                      -->
-  <xsl:template match="p[ol|ul|dl|me|men|md|mdn|cd]">
+  <xsl:template match="p[ol|ul|dl|m[contains(math-nemeth, '
+')]|me|men|md|mdn|cd]">
     <!-- will later loop over displays within paragraph      -->
     <!-- match guarantees at least one for $initial variable -->
-    <xsl:variable name="displays" select="ul|ol|dl|me|men|md|mdn|cd"/>
+    <xsl:variable name="displays" select="ul|ol|dl|m[contains(math-nemeth, '
+')]|me|men|md|mdn|cd"/>
     <!-- content prior to first display is exceptional, but if empty,   -->
     <!-- as indicated by $initial, we do not produce an empty paragraph -->
     <!--                                                                -->
     <!-- all interesting nodes of paragraph, before first display       -->
     <xsl:variable name="initial" select="$displays[1]/preceding-sibling::node()"/>
     <xsl:variable name="initial-content">
       <xsl:apply-templates select="$initial"/>
@@ -1035,15 +1211,16 @@
     </xsl:if>
     <!-- for each display, output the display, plus trailing content -->
     <xsl:for-each select="$displays">
       <!-- do the display proper -->
       <xsl:apply-templates select="."/>
       <!-- look through remainder, all element and text nodes, and the next display -->
       <xsl:variable name="rightward" select="following-sibling::node()"/>
-      <xsl:variable name="next-display" select="following-sibling::*[self::ul or self::ol or self::dl or self::me or self::men or self::md or self::mdn or self::cd][1]"/>
+      <xsl:variable name="next-display" select="following-sibling::*[self::ul or self::ol or self::dl or self::m[contains(math-nemeth, '
+')] or self::me or self::men or self::md or self::mdn or self::cd][1]"/>
       <xsl:choose>
         <xsl:when test="$next-display">
           <xsl:variable name="leftward" select="$next-display/preceding-sibling::node()"/>
           <!-- device below forms set intersection -->
           <xsl:variable name="common" select="$rightward[count(. | $leftward) = count($leftward)]"/>
           <!-- Careful, punctuation after display math      -->
           <!-- gets absorbed into display and so is a node  -->
@@ -1068,18 +1245,14 @@
             </segment>
           </xsl:if>
         </xsl:otherwise>
       </xsl:choose>
     </xsl:for-each>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
-  <xsl:template match="ol|ul|dl">
-    <segment>LIST</segment>
-  </xsl:template>
-  <!-- segment with placeholder content at this stage -->
   <xsl:template match="cd">
     <segment>CODE DISPLAY</segment>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
   <xsl:template match="tabular">
     <segment>TABULAR</segment>
   </xsl:template>
@@ -1087,14 +1260,34 @@
   <xsl:template match="pre">
     <segment>PREFORMATTED TEXT</segment>
   </xsl:template>
   <!-- segment with placeholder content at this stage -->
   <xsl:template match="program">
     <segment>PROGRAM</segment>
   </xsl:template>
+  <!-- We support books and articles, though nothing in particular -->
+  <!-- needs to be done at these root elements.  Yet?              -->
+  <xsl:template match="book|article">
+    <xsl:apply-templates select="*"/>
+  </xsl:template>
+  <!-- "docinfo" should *always* be mined directly for pieces that affect output -->
+  <xsl:template match="docinfo"/>
+  <!-- Many pieces of the "frontmatter" have templates designed for divisions -->
+  <xsl:template match="frontmatter">
+    <xsl:apply-templates select="*"/>
+  </xsl:template>
+  <!-- The "titlepage" and front "colophon" should be mined to form front -->
+  <!-- matter material in the right places, etc.  We kill them for now so -->
+  <!-- we don't see their children being overlooked.                      -->
+  <xsl:template match="titlepage"/>
+  <xsl:template match="frontmatter/colophon"/>
+  <!-- Many pieces of the "backmatter" have templates designed for divisions -->
+  <xsl:template match="backmatter">
+    <xsl:apply-templates select="*"/>
+  </xsl:template>
   <!-- ############ -->
   <!-- EXPERIMENTAL -->
   <!-- ############ -->
   <!-- Uncaught elements for debugging reporting                     -->
   <!-- These elements have full implementations in -common, or       -->
   <!-- partial/abstract implementations which we extend hee.         -->
   <!-- So we just hit them with "apply-imports" so they do not       -->
@@ -1105,22 +1298,25 @@
   <xsl:template match="nbsp|ndash|mdash|xref">
     <xsl:apply-imports/>
   </xsl:template>
   <!-- titles get killed in -common so we don't need to see them here -->
   <xsl:template match="title|subtitle|shorttitle|plaintitle|creator">
     <xsl:apply-imports/>
   </xsl:template>
+  <!-- captions get killed in -common so we don't need to see them here -->
+  <xsl:template match="caption">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- *Every* element needs an implementation, or it ends up here being -->
+  <!-- reported as overlooked.  This is temporary during development.    -->
   <xsl:template match="*">
-    <!-- target informative messages to "blocks" being considered -->
-    <!-- <xsl:if test="ancestor::p"> -->
     <xsl:message>
-      Pass:
+      Overlooked:
       <xsl:value-of select="local-name()"/>
     </xsl:message>
-    <!-- </xsl:if> -->
     <!-- recurse into child elements to find more "missing" elements -->
     <xsl:apply-templates select="*"/>
   </xsl:template>
   <!-- ######### -->
   <!-- Utilities -->
   <!-- ######### -->
   <!-- Transcriber Notes -->
```

#### pretext/braille_format.py

```diff
@@ -242,33 +242,59 @@
             self.lines_after = 0
 
         if "lines-following" in attrs:
             self.lines_following = int(attrs["lines-following"])
         else:
             self.lines_following = 0
 
+        if "heading-id" in attrs:
+            self.heading_id = attrs["heading-id"]
+        else:
+            self.heading_id = None
+
+
 class Block:
 
     def __init__(self, b):
 
         self.xml = b
 
         # decipher, record attributes
         attrs = b.attrib
 
+        if ("newpage" in attrs) and (attrs["newpage"] == "yes"):
+            self.newpage = True
+        else:
+            self.newpage = False
+
+        if ("ownpage" in attrs) and (attrs["ownpage"] == "yes"):
+            self.ownpage = True
+        else:
+            self.ownpage = False
+
+        if ("breakable" in attrs) and (attrs["breakable"] == "no"):
+            self.breakable = False
+        else:
+            self.breakable = True
+
         if "lines-before" in attrs:
             self.lines_before = int(attrs["lines-before"])
         else:
             self.lines_before = 0
 
         if "lines-after" in attrs:
             self.lines_after = int(attrs["lines-after"])
         else:
             self.lines_after = 0
 
+        if "lines-following" in attrs:
+            self.lines_following = int(attrs["lines-following"])
+        else:
+            self.lines_following = 0
+
         if "box" in attrs:
             self.box = attrs["box"]
         else:
             self.box = None
 
         if "punctuation" in attrs:
             self.punctuation = attrs["punctuation"]
@@ -289,82 +315,123 @@
     # "en-ueb-g1.ctb" table with a typeform bit we can use to switch
     # to this variant when we translate inline code phrases
     trans1_bit = louis.getTypeformForEmphClass(["en-ueb-g2.ctb"], 'trans1')
 
     def __init__(self, page_format, width, height):
         self.out_buffer = ''
         self.accumulator = []
+        self.toc_dict = {}
+        self.toc_mode = False
         self.cursor = Cursor(width, height, page_format)
         self.line_buffer = LineBuffer(width)
 
     # Properties (boolean functions) reported
     # by the current line buffer or default/embedded cursor
 
     def is_room_on_line(self, text):
         return self.line_buffer.is_room(text)
 
     def at_line_start(self):
         return self.line_buffer.is_empty()
 
-    # Designed for "short" segments, to avoid poor placement near
-    # a page break.  A segment longer than a page will *always*
-    # provoke a page advance (which might not be desired).
+    # Designed for segments and blocks, to avoid poor placement
+    # near a page break.  Key is a trial/sandbox BRF object and
+    # its associated cursor.
+    #
+    #  * Trial does not provoke a page break.  Good.
+    #  * Trial provokes two page breaks.  Too bad, nothing to be done.
+    #  * Trial provokes exactly one page break.
+    #     - if content is more than a page, that's life
+    #     - see if content fits on a page, recommend a page advance
+    #
+    # Note: this is a bit disingenuous.  This allows both a segment
+    # and a block as an argument, on the assumption they have common
+    # attributes employed here.  Really they should be derived from
+    # a common object.  A switch on object type is necessary to call
+    # the two different BRF "process" methods, no matter what.
     def needs_page_advance(self, seg):
         import copy
 
         # A "page" only makes sense if embossing
         if not(self.cursor.embossing()):
             return False
 
         # If segment explicitly creates a new page,
         # then the question of space is moot
         if seg.ownpage or seg.newpage:
             return False
 
+        # Line numbers could be actual line numbers for first and
+        # last line of content produced by the sandbox BRF.
+        # Formula would be
+        #
+        #     line-number = page-height - remaining-lines + 1
+        #
+        # We will subtract the starting line from the finishing line,
+        # so the page-heights and the "+1" will cancel out.  Thus
+        # definitions are just the negatives of the remaining lines.
+        #
+        # Segment processing always ends on a new line, so the finishing
+        # line has a "-1" to walk it back a line (and if the segment reset
+        # goes to a new page, then the remaining lines would be zero on
+        # the previous page, set to negative zero here).
+
         orginal_cursor = self.cursor
         start_page = orginal_cursor.page_number()
-
+        start_line = -orginal_cursor.remaining_lines()
         # all changes (cursor movement, text-wrapping) will
         # occur in the temporary/sandbox/throwaway cursor
         sandbox_brf = copy.deepcopy(self)
         sandbox_cursor = sandbox_brf.cursor
         # Do the deal, in a sandbox
-        sandbox_brf.process_segment(seg)
+        # Type will be "Block" or "Segment"
+        if type(seg) == Segment:
+            sandbox_brf.process_segment(seg)
+        else:
+            sandbox_brf.process_block(seg)
         # Attach some lines of content, virtually
         for i in range(seg.lines_following):
             sandbox_cursor.advance_line()
 
         finish_page = sandbox_cursor.page_number()
+        finish_line = -sandbox_cursor.remaining_lines() - 1
         # Except, segment finishes ready-to-go,
         # which could be the tip-top of the next page.
         if sandbox_cursor.at_page_start():
             finish_page -= 1
+            finish_line = -0
 
-        # For a block (not implemented yet), when it breaks, we want
-        # to do another simulation: advance a page, see if that stays
-        # on a page.  If not, there is no point in a page advance.
-        # Note: we can't just "size" the first simulation, since the
-        # location of a page break affects a line that reserves space
-        # for a page number.
-
-        # Maybe return the value of boolean expression,
-        # once extended to blocks
-        if finish_page > start_page:
-            return True
-        else:
+        # Fine as-is, no page boundary has been broached
+        if (finish_page - start_page) == 0:
+            return False
+        # Really long, hopeless, a break doesn't help
+        elif (finish_page - start_page) > 1:
+            return False
+        # Exactly one page-break, so look to line numbers
+        # More than a page-full, since finish is later
+        elif finish_line - start_line >= 0:
             return False
+        # There would be a break, and content would fit on the next
+        # page, so go for it and report the need for a page advance
+        else:
+            return True
+
 
     # Actions
 
     def adjust_text_width(self, adjustment):
         # Temporarily adjust the width of a page
-        # For example, to construct a centered heading
-        # Argument is an adjustment to current (negative, then positive?)
-        # Do not call while mid-line, only when at the start of a line
-        assert self.at_line_start(), "BUG: adjusting text width, when not at a line start"
+        # For example, to construct a centered heading,
+        # or to reserve space for a trailing page number.
+        # Argument is an adjustment to the current width
+        # (reduce with negative, then quickly restore with positive).
+        # A reduction must be while preparing a line, the ensuing
+        # expansion can (and often will) occur while mid-line.
+        if (adjustment < 0):
+            assert self.at_line_start(), "BUG: reducing text width, when not at a line start"
         self.cursor.adjust_text_width(adjustment)
         self.line_buffer.adjust_text_width(adjustment)
 
     def write(self, text):
         self.out_buffer += text
 
     def advance_one_line(self):
@@ -560,35 +627,67 @@
             self.advance_page()
 
         # Lines before (but not if at the start of a page)
         if not(self.cursor.at_page_start()):
             for i in range(s.lines_before):
                 self.blank_line()
 
+        # Any page adjustments are now concluded, including a sandbox
+        # trial that may have necessitated a move to a new page.  If
+        # the segment is a heading it is about to be written on the
+        # page and the cursor knows the page number
+        if s.heading_id and self.cursor.embossing() and not(self.toc_mode):
+            self.toc_dict[s.heading_id] = self.cursor.page_number()
+
         # Centered
         # [BANA 2016],  4.4.2
         # At least three blank cells must precede and follow a centered heading.
         #
         # So shrink line buffer to get extra space
         if s.centered:
             self.adjust_text_width(-6)
 
+        # If making segments/headings into ToC entries, then
+        # reserve 6 spaces to the right at all times, until
+        # just about to write the guide dots and page number
+        if self.toc_mode:
+            self.adjust_text_width(-6)
+
         sxml = s.xml
         if sxml.text:
             self.write_fragment("text", sxml.text, None, s)
         children = list(sxml)
         for c in children:
             if c.text:
                 if 'punctuation' in c.attrib:
                     math_punctuation = c.attrib['punctuation']
                 else:
                     math_punctuation = None
                 self.write_fragment(c.tag, c.text, math_punctuation, s)
             if c.tail:
                 self.write_fragment("text", c.tail, None, s)
+
+        # Release width restriction to finish ToC entry
+        if self.toc_mode:
+            self.adjust_text_width(6)
+            # Page numbers iff embossing
+            if self.cursor.embossing():
+                page_num = str(self.toc_dict[s.heading_id])
+                guide_dots = self.cursor.remaining_characters() - (1 + len(page_num))
+                guide = ['', '', '']
+                if guide_dots > 0:
+                    guide[0] = ' '
+                    guide_dots -= 1
+                if guide_dots > 0:
+                    guide[2] = ' '
+                    guide_dots -= 1
+                if guide_dots > 0:
+                    guide[1] = '\u2810' * guide_dots
+                self.write_fragment("text", ''.join(guide) + page_num, None, s)
+
         # finished with a segment
         # flush buffer, move to new line, maybe a new page
         # BUT not if we landed in this state anyway
         if not(self.at_line_start()):
             self.advance_one_line()
         # Necessary to restore for subsequent centering
         if s.centered:
@@ -644,15 +743,15 @@
 
         # Unicode characters translate, one for one, into BRF
         # characters and we assume punctuation does the same.
         # If not, we could map a few punctuation marks to Unicode.
         # Or perhaps set argument to do uncontracted braille.
         return louis.translateString(["en-ueb-g2.ctb"], aline, None, 0)
 
-    def write_block(self, blk):
+    def process_block(self, blk):
 
         # Lines before (but not if at the start of a page)
         if not(self.cursor.at_page_start()):
             for i in range(blk.lines_before):
                 self.blank_line()
 
         if blk.box == "standard":
@@ -690,24 +789,33 @@
             self.advance_one_line()
 
         # Lines after
         for i in range(blk.lines_after):
             self.blank_line()
             self.flush()
 
-        self.flush()
-
+    # The next two "write" routines simply check if a page advance
+    # is necessary/desirable for the block or segment in question,
+    # and then call the "process" versions, where the real action
+    # happens.  Then a flush.
 
     def write_segment(self, seg):
         # See if a page advance will improve awkward page breaks
         if not(seg.breakable) and self.needs_page_advance(seg):
             self.advance_page()
         self.process_segment(seg)
         self.flush()
 
+    def write_block(self, blk):
+        # See if a page advance will improve awkward page breaks
+        if not(blk.breakable) and self.needs_page_advance(blk):
+            self.advance_page()
+        self.process_block(blk)
+        self.flush()
+
     def flush(self):
         # The `accumulator` *is* the final document, as a list of
         # strings, so here we move the (completed) string for the
         # segment into the list that will be concatenated.  And
         # prepare the `out_buffer` for the next segment.
         self.accumulator.append(self.out_buffer)
         self.out_buffer = ''
@@ -774,12 +882,34 @@
             seg = Segment(elt)
             brf.write_segment(seg)
         elif elt.tag == "block":
             blk = Block(elt)
             brf.write_block(blk)
         brf.flush()
 
+    # Prepare a new BRF object, but copy out ToC page numbers
+    front = BRF(page_format, 40,25)
+    front.toc_mode = True
+    front.toc_dict = brf.toc_dict
+
+    headings = src_tree.xpath("/brf/segment[@heading-id]")
+    for head in headings:
+        seg = Segment(head)
+        seg.newpage = False
+        seg.ownpage = False
+        seg.centered = False
+        seg.breakable = False
+        # indentation, runover
+        seg.lines_before = 0
+        seg.lines_after = 0
+        seg.lines_following = 0
+        front.write_segment(seg)
+    # Fill out frontmatter final page
+    if page_format == 'emboss':
+        front.advance_page()
+
     # We assume `out_file` has been error-checked
     # It would be better to use a context manager
     brf_file = open(out_file, "w")
+    brf_file.write(front.get_brf())
     brf_file.write(brf.get_brf())
     brf_file.close()
```

### Comparing `pretext-1.5.3.dev20230503/pretext/generate.py` & `pretext-1.5.3.dev20230504/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/project.py` & `pretext-1.5.3.dev20230504/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230504/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230504/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230504/pretext/templates/resources/article.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-03 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-03 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-03 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-03 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-03 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-May-03 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx      630 b- defN 23-May-03 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-03 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      449 b- defN 23-May-03 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-03 06:18 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-03 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-04 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-04 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-04 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      449 b- defN 23-May-04 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-04 06:18 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-04 06:18 source/main.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230504/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-03 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-03 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-03 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-03 06:19 .gitignore
--rw-r--r--  2.0 unx     6114 b- defN 23-May-03 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-03 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-03 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-May-03 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-04 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-04 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-04 06:18 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230504/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-03 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-03 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-03 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-03 06:19 .gitignore
--rw-r--r--  2.0 unx     6092 b- defN 23-May-03 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-03 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-03 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx      630 b- defN 23-May-03 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-03 06:19 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-May-03 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-03 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-03 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-03 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-May-03 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-03 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-03 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-03 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-03 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-03 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-03 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-03 06:18 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-03 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-03 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-03 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-03 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-May-03 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-03 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-03 06:18 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 23-May-03 06:18 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-04 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-04 06:18 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-04 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-04 06:18 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-May-04 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-04 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-04 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-04 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-May-04 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-04 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-04 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-04 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-04 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-04 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-04 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-04 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-04 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-04 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-04 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-04 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-May-04 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-04 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-04 06:18 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 23-May-04 06:18 source/images/sageplot2d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230504/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230504/pretext/templates/resources/hello.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-03 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-May-03 06:18 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-03 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-03 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-03 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-03 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-03 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-May-03 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-May-04 06:18 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-04 06:18 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-04 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-May-04 06:18 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230504/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230504/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230504/pretext/templates/resources/slideshow.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-03 06:18 xsl/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-03 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-May-03 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-03 06:19 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-May-03 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-03 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-03 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-03 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx    11200 b- defN 23-May-03 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 xsl/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-May-04 06:18 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-May-04 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-04 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-04 06:18 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

### Comparing `pretext-1.5.3.dev20230503/pretext/utils.py` & `pretext-1.5.3.dev20230504/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230503/pyproject.toml` & `pretext-1.5.3.dev20230504/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230503"
+version = "1.5.3.dev20230504"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230503/PKG-INFO` & `pretext-1.5.3.dev20230504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230503
+Version: 1.5.3.dev20230504
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

