# Comparing `tmp/satsim-0.14.0.tar.gz` & `tmp/satsim-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsim-0.14.0.tar", last modified: Thu Apr 13 09:49:43 2023, max compression
+gzip compressed data, was "satsim-0.15.0.tar", last modified: Thu May  4 05:43:55 2023, max compression
```

## Comparing `satsim-0.14.0.tar` & `satsim-0.15.0.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-22 19:32:02.000000 satsim-0.14.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3255 2023-02-17 19:27:57.000000 satsim-0.14.0/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     6666 2023-04-13 09:36:02.000000 satsim-0.14.0/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)      291 2022-07-22 19:32:02.000000 satsim-0.14.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8291 2023-04-13 09:49:43.543551 satsim-0.14.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-04-13 09:42:46.000000 satsim-0.14.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.523551 satsim-0.14.0/docs/
--rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.523551 satsim-0.14.0/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)    14813 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/css/
--rw-r--r--   0 root         (0) root         (0)     3229 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 root         (0) root         (0)   165742 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)   135235 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     4472 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/file.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/js/
--rw-r--r--   0 root         (0) root         (0)      934 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 root         (0) root         (0)     4370 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 root         (0) root         (0)     2734 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 root         (0) root         (0)     5023 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)     4758 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4846 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18215 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     4712 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/api/
--rw-r--r--   0 root         (0) root         (0)    10121 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.dataset.html
--rw-r--r--   0 root         (0) root         (0)    10056 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.generator.html
--rw-r--r--   0 root         (0) root         (0)    59162 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.generator.obs.html
--rw-r--r--   0 root         (0) root         (0)   106508 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.geometry.html
--rw-r--r--   0 root         (0) root         (0)   159519 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.html
--rw-r--r--   0 root         (0) root         (0)    91650 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.image.html
--rw-r--r--   0 root         (0) root         (0)    34797 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.io.html
--rw-r--r--   0 root         (0) root         (0)    33473 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.math.html
--rw-r--r--   0 root         (0) root         (0)    14551 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.pipeline.html
--rw-r--r--   0 root         (0) root         (0)    19353 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.time.html
--rw-r--r--   0 root         (0) root         (0)    24310 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.util.html
--rw-r--r--   0 root         (0) root         (0)   404446 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/api/satsim.vecmath.html
--rw-r--r--   0 root         (0) root         (0)   122444 2023-04-13 09:49:40.000000 satsim-0.14.0/docs/_build/html/api.html
--rw-r--r--   0 root         (0) root         (0)     5491 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/authors.html
--rw-r--r--   0 root         (0) root         (0)    13939 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/contributing.html
--rw-r--r--   0 root         (0) root         (0)    95348 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/genindex.html
--rw-r--r--   0 root         (0) root         (0)    17468 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/history.html
--rw-r--r--   0 root         (0) root         (0)     9440 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/index.html
--rw-r--r--   0 root         (0) root         (0)     7750 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/installation.html
--rw-r--r--   0 root         (0) root         (0)    17277 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 root         (0) root         (0)     4196 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/search.html
--rw-r--r--   0 root         (0) root         (0)   121517 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/searchindex.js
--rw-r--r--   0 root         (0) root         (0)    37538 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)      310 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.dataset.rst
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.generator.obs.rst
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.generator.rst
--rw-r--r--   0 root         (0) root         (0)     1872 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.geometry.rst
--rw-r--r--   0 root         (0) root         (0)     1004 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.image.rst
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.io.rst
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.math.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.pipeline.rst
--rw-r--r--   0 root         (0) root         (0)      730 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.rst
--rw-r--r--   0 root         (0) root         (0)      123 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.time.rst
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.util.rst
--rw-r--r--   0 root         (0) root         (0)     1276 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.vecmath.rst
--rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/api.rst
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)     4906 2023-04-13 09:36:02.000000 satsim-0.14.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/history.rst
--rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-17 19:27:57.000000 satsim-0.14.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/
--rw-r--r--   0 root         (0) root         (0)      264 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4131 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/cli.py
--rw-r--r--   0 root         (0) root         (0)    20530 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/dataset/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/generator/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/generator/obs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12937 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/breakup.py
--rw-r--r--   0 root         (0) root         (0)     2330 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/cso.py
--rw-r--r--   0 root         (0) root         (0)     6239 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/geometry.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/io.py
--rw-r--r--   0 root         (0) root         (0)     3703 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/rpo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/geometry/
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20912 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/geometry/astrometric.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/csvsc.py
--rw-r--r--   0 root         (0) root         (0)     5268 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/draw.py
--rw-r--r--   0 root         (0) root         (0)     3404 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/ephemeris.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/random.py
--rw-r--r--   0 root         (0) root         (0)     1150 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/sgp4.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/sprite.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/sstr7.py
--rw-r--r--   0 root         (0) root         (0)     4340 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/transform.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/twobody.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-02-17 00:02:42.000000 satsim-0.14.0/satsim/geometry/wcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/image/
--rw-r--r--   0 root         (0) root         (0)       58 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9793 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/augment.py
--rw-r--r--   0 root         (0) root         (0)    16529 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/image/fpa.py
--rw-r--r--   0 root         (0) root         (0)     5359 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/image/model.py
--rw-r--r--   0 root         (0) root         (0)     2842 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/noise.py
--rw-r--r--   0 root         (0) root         (0)     6166 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/psf.py
--rw-r--r--   0 root         (0) root         (0)    10401 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/io/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13925 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/io/czml.py
--rw-r--r--   0 root         (0) root         (0)     4319 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/fits.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 01:56:05.000000 satsim-0.14.0/satsim/io/image.py
--rw-r--r--   0 root         (0) root         (0)     7122 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/satnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/math/
--rw-r--r--   0 root         (0) root         (0)       81 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-04-05 08:00:38.000000 satsim-0.14.0/satsim/math/angle.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/math/const.py
--rw-r--r--   0 root         (0) root         (0)      951 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/conv.py
--rw-r--r--   0 root         (0) root         (0)     5551 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/fft.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/math/interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/math/random.py
--rw-r--r--   0 root         (0) root         (0)      590 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1087 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41936 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/satsim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/time/
--rw-r--r--   0 root         (0) root         (0)     4259 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/util/
--rw-r--r--   0 root         (0) root         (0)      130 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2542 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/system.py
--rw-r--r--   0 root         (0) root         (0)     3271 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/vecmath/
--rw-r--r--   0 root         (0) root         (0)    17668 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian2.py
--rw-r--r--   0 root         (0) root         (0)    20896 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian3.py
--rw-r--r--   0 root         (0) root         (0)    18429 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian4.py
--rw-r--r--   0 root         (0) root         (0)    21727 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix2.py
--rw-r--r--   0 root         (0) root         (0)    42567 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix3.py
--rw-r--r--   0 root         (0) root         (0)    73877 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix4.py
--rw-r--r--   0 root         (0) root         (0)    25251 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Quaternion.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8291 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3994 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      539 2023-04-13 09:49:43.543551 satsim-0.14.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1796 2023-04-13 09:36:02.000000 satsim-0.14.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/tests/
--rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.14.0/tests/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.635508 satsim-0.15.0/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-07-22 19:32:02.000000 satsim-0.15.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-02-17 19:27:57.000000 satsim-0.15.0/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-05-04 05:31:05.000000 satsim-0.15.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)      291 2022-07-22 19:32:02.000000 satsim-0.15.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8582 2023-05-04 05:43:55.635508 satsim-0.15.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-05-04 05:31:05.000000 satsim-0.15.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)    14813 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/css/
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.615508 satsim-0.15.0/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)   135235 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/file.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/_build/html/_static/js/
+-rw-r--r--   0 root         (0) root         (0)      934 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-05-04 05:40:36.000000 satsim-0.15.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    18215 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-05-04 05:40:35.000000 satsim-0.15.0/docs/_build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/_build/html/api/
+-rw-r--r--   0 root         (0) root         (0)    10121 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.dataset.html
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.generator.html
+-rw-r--r--   0 root         (0) root         (0)    59162 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.generator.obs.html
+-rw-r--r--   0 root         (0) root         (0)   106508 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.geometry.html
+-rw-r--r--   0 root         (0) root         (0)   159759 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api/satsim.html
+-rw-r--r--   0 root         (0) root         (0)    91699 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.image.html
+-rw-r--r--   0 root         (0) root         (0)    37488 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.io.html
+-rw-r--r--   0 root         (0) root         (0)    33473 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.math.html
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.pipeline.html
+-rw-r--r--   0 root         (0) root         (0)    19353 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.time.html
+-rw-r--r--   0 root         (0) root         (0)    24867 2023-05-04 05:43:53.000000 satsim-0.15.0/docs/_build/html/api/satsim.util.html
+-rw-r--r--   0 root         (0) root         (0)   404446 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/api/satsim.vecmath.html
+-rw-r--r--   0 root         (0) root         (0)   122688 2023-05-04 05:43:52.000000 satsim-0.15.0/docs/_build/html/api.html
+-rw-r--r--   0 root         (0) root         (0)     5491 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/authors.html
+-rw-r--r--   0 root         (0) root         (0)    13939 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/contributing.html
+-rw-r--r--   0 root         (0) root         (0)    95509 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/genindex.html
+-rw-r--r--   0 root         (0) root         (0)    18083 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/history.html
+-rw-r--r--   0 root         (0) root         (0)     9534 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/index.html
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/installation.html
+-rw-r--r--   0 root         (0) root         (0)    17277 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/py-modindex.html
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/search.html
+-rw-r--r--   0 root         (0) root         (0)   122825 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/searchindex.js
+-rw-r--r--   0 root         (0) root         (0)    37538 2023-05-04 05:43:54.000000 satsim-0.15.0/docs/_build/html/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.dataset.rst
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.generator.obs.rst
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.generator.rst
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.geometry.rst
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.image.rst
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.io.rst
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.math.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.pipeline.rst
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.time.rst
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.util.rst
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-05-04 05:43:42.000000 satsim-0.15.0/docs/api/satsim.vecmath.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-05-04 05:31:05.000000 satsim-0.15.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/history.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-02-17 19:27:57.000000 satsim-0.15.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:32:02.000000 satsim-0.15.0/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/cli.py
+-rw-r--r--   0 root         (0) root         (0)    20530 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/dataset/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/generator/obs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/breakup.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/cso.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/io.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/generator/obs/rpo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/geometry/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20912 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/geometry/astrometric.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/csvsc.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/draw.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/ephemeris.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/random.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/sgp4.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/sprite.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/sstr7.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/geometry/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/geometry/twobody.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-02-17 00:02:42.000000 satsim-0.15.0/satsim/geometry/wcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/image/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/augment.py
+-rw-r--r--   0 root         (0) root         (0)    16625 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/image/fpa.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/image/model.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/image/noise.py
+-rw-r--r--   0 root         (0) root         (0)     6166 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/psf.py
+-rw-r--r--   0 root         (0) root         (0)    10401 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/image/render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14550 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/czml.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/fits.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 01:56:05.000000 satsim-0.15.0/satsim/io/image.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/io/satnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/math/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-04-05 08:00:38.000000 satsim-0.15.0/satsim/math/angle.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/math/const.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/conv.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/fft.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/math/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-02-17 19:27:57.000000 satsim-0.15.0/satsim/math/random.py
+-rw-r--r--   0 root         (0) root         (0)      590 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/math/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42871 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/satsim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/time/
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/util/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-05-04 05:31:05.000000 satsim-0.15.0/satsim/util/system.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-07-22 19:32:02.000000 satsim-0.15.0/satsim/util/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim/vecmath/
+-rw-r--r--   0 root         (0) root         (0)    17668 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian2.py
+-rw-r--r--   0 root         (0) root         (0)    20896 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian3.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Cartesian4.py
+-rw-r--r--   0 root         (0) root         (0)    21727 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix2.py
+-rw-r--r--   0 root         (0) root         (0)    42567 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix3.py
+-rw-r--r--   0 root         (0) root         (0)    73877 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Matrix4.py
+-rw-r--r--   0 root         (0) root         (0)    25251 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/Quaternion.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-13 09:36:02.000000 satsim-0.15.0/satsim/vecmath/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/satsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8582 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 05:43:55.000000 satsim-0.15.0/satsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-05-04 05:43:55.635508 satsim-0.15.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-05-04 05:31:05.000000 satsim-0.15.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 05:43:55.625508 satsim-0.15.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.15.0/tests/README.md
```

### Comparing `satsim-0.14.0/CONTRIBUTING.rst` & `satsim-0.15.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/HISTORY.md` & `satsim-0.15.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 History
 =======
 
+0.15.0
+---------------------
+
+* Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
+* Add support for running on CPU with no GPU acceleration.
+* Add CZML options for sensor visualization and object billboard image.
+
+
 0.14.0
 ---------------------
 
-Add vector math library.
-Add CZML output for sensor visualization.
-Fix objects not updating properly when image renderer is off.
+* Add vector math library.
+* Add CZML output for sensor visualization.
+* Fix objects not updating properly when image renderer is off.
 
 
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
```

### Comparing `satsim-0.14.0/PKG-INFO` & `satsim-0.15.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.14.0
+Version: 0.15.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,20 +37,28 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.15.0
+---------------------
+
+* Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
+* Add support for running on CPU with no GPU acceleration.
+* Add CZML options for sensor visualization and object billboard image.
+
+
 0.14.0
 ---------------------
 
-Add vector math library.
-Add CZML output for sensor visualization.
-Fix objects not updating properly when image renderer is off.
+* Add vector math library.
+* Add CZML output for sensor visualization.
+* Fix objects not updating properly when image renderer is off.
 
 
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
```

### Comparing `satsim-0.14.0/README.md` & `satsim-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/Makefile` & `satsim-0.15.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/basic.css` & `satsim-0.15.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/badge_only.css` & `satsim-0.15.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `satsim-0.15.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/css/theme.css` & `satsim-0.15.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/doctools.js` & `satsim-0.15.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/js/badge_only.js` & `satsim-0.15.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `satsim-0.15.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/js/html5shiv.min.js` & `satsim-0.15.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/js/theme.js` & `satsim-0.15.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/language_data.js` & `satsim-0.15.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/pygments.css` & `satsim-0.15.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/searchtools.js` & `satsim-0.15.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/_static/sphinx_highlight.js` & `satsim-0.15.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.dataset.html` & `satsim-0.15.0/docs/_build/html/api/satsim.dataset.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.dataset package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.dataset package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.generator.html` & `satsim-0.15.0/docs/_build/html/api/satsim.generator.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.generator package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.generator.obs.html` & `satsim-0.15.0/docs/_build/html/api/satsim.generator.obs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator.obs package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.generator.obs package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.geometry.html` & `satsim-0.15.0/docs/_build/html/api/satsim.geometry.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.geometry package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.geometry package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.html` & `satsim-0.15.0/docs/_build/html/api/satsim.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -382,14 +382,15 @@
 <li class="toctree-l1"><a class="reference internal" href="satsim.util.html">satsim.util package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="satsim.util.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.util.html#module-satsim.util.system">satsim.util.system module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_eager"><code class="docutils literal notranslate"><span class="pre">configure_eager()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_multi_gpu"><code class="docutils literal notranslate"><span class="pre">configure_multi_gpu()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_single_gpu"><code class="docutils literal notranslate"><span class="pre">configure_single_gpu()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.get_semantic_version"><code class="docutils literal notranslate"><span class="pre">get_semantic_version()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.is_tensorflow_running_on_cpu"><code class="docutils literal notranslate"><span class="pre">is_tensorflow_running_on_cpu()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.util.html#module-satsim.util.thread">satsim.util.thread module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.thread.MultithreadedTaskQueue"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue</span></code></a><ul>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.has_tag"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.has_tag()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.stop"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.stop()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.task"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.task()</span></code></a></li>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -228,14 +228,15 @@
     * satsim.util_package
           o Submodules
           o satsim.util.system_module
                 # configure_eager()
                 # configure_multi_gpu()
                 # configure_single_gpu()
                 # get_semantic_version()
+                # is_tensorflow_running_on_cpu()
           o satsim.util.thread_module
                 # MultithreadedTaskQueue
                       # MultithreadedTaskQueue.has_tag()
                       # MultithreadedTaskQueue.stop()
                       # MultithreadedTaskQueue.task()
                       # MultithreadedTaskQueue.waitUntilEmpty()
                 # ThreadedTaskQueue
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.image.html` & `satsim-0.15.0/docs/_build/html/api/satsim.image.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.image package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.image package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -721,15 +721,16 @@
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>fpa</strong> – <cite>Tensor</cite>, input image as a 2D tensor in real pixels (not oversampled).</p></li>
 <li><p><strong>rn</strong> – <cite>float</cite>, electrons RMS value of the read noise.</p></li>
 <li><p><strong>en</strong> – <cite>float</cite>, electrons RMS value of the electronic noise.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>A <cite>Tensor</cite>, the 2D tensor with read noise applied.</p>
+<dd class="field-even"><p>A <cite>Tensor</cite>, the 2D tensor with read noise applied.
+A <cite>Tensor</cite>, the 2D tensor read noise.</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
 <section id="module-satsim.image.psf">
 <span id="satsim-image-psf-module"></span><h2>satsim.image.psf module<a class="headerlink" href="#module-satsim.image.psf" title="Permalink to this heading"></a></h2>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -452,15 +452,16 @@
       fpa_with_read_noise = add_read_noise(fpa, 15)
         Parameters:
                 * fpa âTensor, input image as a 2D tensor in real pixels (not
                   oversampled).
                 * rn âfloat, electrons RMS value of the read noise.
                 * en âfloat, electrons RMS value of the electronic noise.
         Returns:
-            ATensor, the 2D tensor with read noise applied.
+            ATensor, the 2D tensor with read noise applied. ATensor, the 2D
+            tensor read noise.
 
 ***** satsim.image.psf moduleï *****
   satsim.image.psf.eod_to_sigma(eod, osf)ï
       Calculates the sigma of a 2D Gaussian required to get a maximum energy on
       a detector (EOD) or single pixel. EOD is specified as a fraction (0 < EOD
       < 1). The 2D Gaussian is assumed to be centered on a real pixel.
         Parameters:
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.io.html` & `satsim-0.15.0/docs/_build/html/api/satsim.io.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.io package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.io package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -111,15 +111,15 @@
 <dl class="py class">
 <dt class="sig sig-object py" id="satsim.io.czml.CZMLExtractor">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">satsim.io.czml.</span></span><span class="sig-name descname"><span class="pre">CZMLExtractor</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">start_epoch</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_epoch</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">multiplier</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">60</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>A class for extracting SatSim data to Cesium</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="satsim.io.czml.CZMLExtractor.add_ground_station">
-<span class="sig-name descname"><span class="pre">add_ground_station</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">pos</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sensor</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_ground_station" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">add_ground_station</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">pos</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sensor</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">billboard_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">billboard_image</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACvSURBVDhPrZDRDcMgDAU9GqN0lIzijw6SUbJJygUeNQgSqepJTyHG91LVVpwDdfxM3T9TSl1EXZvDwii471fivK73cBFFQNTT/d2KoGpfGOpSIkhUpgUMxq9DFEsWv4IXhlyCnhBFnZcFEEuYqbiUlNwWgMTdrZ3JbQFoEVG53rd8ztG9aPJMnBUQf/VFraBJeWnLS0RfjbKyLJA8FkT5seDYS1Qwyv8t0B/5C2ZmH2/eTGNNBgMmAAAAAElFTkSuQmCC'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cone_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">64]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cone_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_ground_station" title="Permalink to this definition"></a></dt>
 <dd><p>Adds a ground station</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>pos</strong> – <cite>list [~astropy.units]</cite>, coordinates of ground station (i.e. latitude, longitude, altitude)</p></li>
 <li><p><strong>id_description</strong> – <cite>str</cite>, Set ground station description</p></li>
 <li><p><strong>label_fill_color</strong> – <cite>list (int)</cite>, Fill Color in rgba format</p></li>
@@ -130,15 +130,15 @@
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="satsim.io.czml.CZMLExtractor.add_object">
-<span class="sig-name descname"><span class="pre">add_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sat</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">N</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">10</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_width</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_interval</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_interval</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_available</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_available</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">billboard_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_object" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">add_object</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sat</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">N</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">10</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_width</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">path_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_interval</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_interval</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_available</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_available</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">billboard_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">billboard_image</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAADJSURBVDhPnZHRDcMgEEMZjVEYpaNklIzSEfLfD4qNnXAJSFWfhO7w2Zc0Tf9QG2rXrEzSUeZLOGm47WoH95x3Hl3jEgilvDgsOQUTqsNl68ezEwn1vae6lceSEEYvvWNT/Rxc4CXQNGadho1NXoJ+9iaqc2xi2xbt23PJCDIB6TQjOC6Bho/sDy3fBQT8PrVhibU7yBFcEPaRxOoeTwbwByCOYf9VGp1BYI1BA+EeHhmfzKbBoJEQwn1yzUZtyspIQUha85MpkNIXB7GizqDEECsAAAAASUVORK5CYII='</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_object" title="Permalink to this definition"></a></dt>
 <dd><p>Adds a SatSim Skyfield object</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>sat</strong> – <cite>object</cite>, SatSim Skyfield object</p></li>
 <li><p><strong>N</strong> – <cite>int</cite>, Number of sample points</p></li>
 <li><p><strong>id_name</strong> – <cite>str</cite>, Set orbit name</p></li>
@@ -188,23 +188,23 @@
 </dd></dl>
 
 </section>
 <section id="module-satsim.io.fits">
 <span id="satsim-io-fits-module"></span><h2>satsim.io.fits module<a class="headerlink" href="#module-satsim.io.fits" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.fits.save">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">4,</span> <span class="pre">13,</span> <span class="pre">9,</span> <span class="pre">49,</span> <span class="pre">34,</span> <span class="pre">855695)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">4,</span> <span class="pre">5,</span> <span class="pre">43,</span> <span class="pre">45,</span> <span class="pre">661952)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
 <dd><p>Save a SatNet compatible FITS file.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>filename</strong> – <cite>string</cite>, the FITS filename.</p></li>
 <li><p><strong>fpa</strong> – <cite>np.array</cite>, input image as a 2D numpy array.</p></li>
 <li><p><strong>exposure_time</strong> – <cite>float</cite>, exposure time for header.</p></li>
-<li><p><strong>dt_start</strong> – <cite>datatime</cite>, datetime of start of exposure.</p></li>
+<li><p><strong>dt_start</strong> – <cite>datetime</cite>, datetime of start of exposure.</p></li>
 <li><p><strong>header</strong> – <cite>dict</cite>, placeholder, not implemented</p></li>
 <li><p><strong>overwrite</strong> – <cite>boolean</cite>, if True overwrite file if it exists</p></li>
 <li><p><strong>dtype</strong> – <cite>string</cite>, ‘int16’, ‘uint16’, ‘int32’, ‘uint32’, or ‘float32’. default: ‘int16’</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
@@ -302,29 +302,32 @@
 <dd class="field-even"><p>A <cite>dict</cite>, the data object for <cite>set_frame_annotation</cite></p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.satnet.write_frame">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.satnet.</span></span><span class="sig-name descname"><span class="pre">write_frame</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dir_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sat_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa_digital</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">meta_data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">frame_num</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_stamp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">show_obs_boxes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_pickle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.satnet.write_frame" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.satnet.</span></span><span class="sig-name descname"><span class="pre">write_frame</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dir_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sat_name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa_digital</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">meta_data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">frame_num</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_stamp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">show_obs_boxes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_pickle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">save_jpeg</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ground_truth_min</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.satnet.write_frame" title="Permalink to this definition"></a></dt>
 <dd><p>Write image and annotation files compatible with SatNet. In addition,
 writes annotated images and SatSim configuration file for reference.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>dir_name</strong> – <cite>string</cite>, directory to save files to</p></li>
 <li><p><strong>sat_name</strong> – <cite>string</cite>, satellite name</p></li>
 <li><p><strong>fpa_digital</strong> – <cite>array</cite>, image as a numpy array</p></li>
 <li><p><strong>meta_data</strong> – <cite>dict</cite>, annotation data generated by <cite>init_annotation</cite></p></li>
 <li><p><strong>frame_num</strong> – <cite>int</cite>, current frame number in set</p></li>
 <li><p><strong>exposure_time</strong> – <cite>float</cite>, current frame exposure time in seconds</p></li>
 <li><p><strong>time_stamp</strong> – <cite>datetime</cite>, reference time</p></li>
 <li><p><strong>ssp</strong> – <cite>dict</cite>: SatSim parameters to be saved to JSON file</p></li>
 <li><p><strong>dtype</strong> – <cite>string</cite>: Data type to save FITS pixel data as</p></li>
+<li><p><strong>save_jpeg</strong> – <cite>boolean</cite>: specify to save a JPEG annotated image</p></li>
+<li><p><strong>ground_truth</strong> – <cite>OrderedDict</cite>: an ordered dictionary of arrays or numbers</p></li>
+<li><p><strong>ground_truth_min</strong> – <cite>float</cite>, set any value less than this number in ground_truth to 0</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
 </section>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -43,15 +43,21 @@
 ***** satsim.io.czml moduleï *****
   classsatsim.io.czml.CZMLExtractor(start_epoch, end_epoch, multiplier=60)ï
       Bases: object
       A class for extracting SatSim data to Cesium
         add_ground_station(pos, sensor, id_name=None, id_description=None,
         label_fill_color=[255, 255, 0, 255], label_outline_color=[255, 255, 0,
         255], label_font='16pt Lucida Console', label_text=None,
-        label_show=False)ï
+        label_show=False, billboard_show=True, billboard_image='data:image/
+        png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/
+        9hAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAACvSURBVDhPrZDRDcMgDAU9GqN0lIzijw6SUbJJygUeNQgSqepJTyHG91LVVpwDdfxM3T9TSl1EXZvDwii471fivK73cBFFQNTT/
+        d2KoGpfGOpSIkhUpgUMxq9DFEsWv4IXhlyCnhBFnZcFEEuYqbiUlNwWgMTdrZ3JbQFoEVG53rd8ztG9aPJMnBUQf/
+        VFraBJeWnLS0RfjbKyLJA8FkT5seDYS1Qwyv8t0B/5C2ZmH2/
+        eTGNNBgMmAAAAAElFTkSuQmCC', cone_color=[255, 255, 0, 64],
+        cone_show=True)ï
             Adds a ground station
               Parameters:
                       * pos âlist [~astropy.units], coordinates of ground
                         station (i.e. latitude, longitude, altitude)
                       * id_description âstr, Set ground station description
                       * label_fill_color âlist (int), Fill Color in rgba
                         format
@@ -63,15 +69,20 @@
                       * label_show âbool, Indicates whether the label is
                         visible
         add_object(sat, N=10, id_name=None, id_description=None,
         path_width=None, path_show=None, path_color=[255, 255, 0],
         label_fill_color=[255, 255, 0, 255], label_outline_color=[255, 255, 0,
         255], label_font='16pt Lucida Console', label_text=None,
         label_show=False, start_interval=None, end_interval=None,
-        start_available=None, end_available=None, billboard_show=True)ï
+        start_available=None, end_available=None, billboard_show=True,
+        billboard_image='data:image/
+        png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/
+        9hAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAADJSURBVDhPnZHRDcMgEEMZjVEYpaNklIzSEfLfD4qNnXAJSFWfhO7w2Zc0Tf9QG2rXrEzSUeZLOGm47WoH95x3Hl3jEgilvDgsOQUTqsNl68ezEwn1vae6lceSEEYvvWNT/
+        Rxc4CXQNGadho1NXoJ+9iaqc2xi2xbt23PJCDIB6TQjOC6Bho/
+        sDy3fBQT8PrVhibU7yBFcEPaRxOoeTwbwByCOYf9VGp1BYI1BA+EeHhmfzKbBoJEQwn1yzUZtyspIQUha85MpkNIXB7GizqDEECsAAAAASUVORK5CYII=')ï
             Adds a SatSim Skyfield object
               Parameters:
                       * sat âobject, SatSim Skyfield object
                       * N âint, Number of sample points
                       * id_name âstr, Set orbit name
                       * id_description âstr, Set orbit description
                       * path_width âint, Path width
@@ -98,22 +109,22 @@
                 * obs_cache âlist, list of SatSim Skyfield objects.
                 * filename âstr, if not None, save czml output. default=None
         Returns:
             Adict, the CZML output
 
 ***** satsim.io.fits moduleï *****
   satsim.io.fits.save(filename, fpa, exposure_time=0,
-  dt_start=datetime.datetime(2023, 4, 13, 9, 49, 34, 855695), header={},
+  dt_start=datetime.datetime(2023, 5, 4, 5, 43, 45, 661952), header={},
   overwrite=False, dtype='uint16', astrometrics=None)ï
       Save a SatNet compatible FITS file.
         Parameters:
                 * filename âstring, the FITS filename.
                 * fpa ânp.array, input image as a 2D numpy array.
                 * exposure_time âfloat, exposure time for header.
-                * dt_start âdatatime, datetime of start of exposure.
+                * dt_start âdatetime, datetime of start of exposure.
                 * header âdict, placeholder, not implemented
                 * overwrite âboolean, if True overwrite file if it exists
                 * dtype âstring, âint16â, âuint16â, âint32â,
                   âuint32â, or âfloat32â. default: âint16â
 
 ***** satsim.io.image moduleï *****
   satsim.io.image.save(filename, fpa, vauto=False, vmin=None, vmax=None,
@@ -173,27 +184,33 @@
                 * box_pad âint, amount of pad to add to each side of box
                 * filter_ob âboolean, bounds min and max and remove out of
                   bounds
         Returns:
             Adict, the data object forset_frame_annotation
   satsim.io.satnet.write_frame(dir_name, sat_name, fpa_digital, meta_data,
   frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True,
-  astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True)ï
+  astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True,
+  ground_truth=None, ground_truth_min=0)ï
       Write image and annotation files compatible with SatNet. In addition,
       writes annotated images and SatSim configuration file for reference.
         Parameters:
                 * dir_name âstring, directory to save files to
                 * sat_name âstring, satellite name
                 * fpa_digital âarray, image as a numpy array
                 * meta_data âdict, annotation data generated
                   byinit_annotation
                 * frame_num âint, current frame number in set
                 * exposure_time âfloat, current frame exposure time in
                   seconds
                 * time_stamp âdatetime, reference time
                 * ssp âdict: SatSim parameters to be saved to JSON file
                 * dtype âstring: Data type to save FITS pixel data as
+                * save_jpeg âboolean: specify to save a JPEG annotated image
+                * ground_truth âOrderedDict: an ordered dictionary of arrays
+                  or numbers
+                * ground_truth_min âfloat, set any value less than this
+                  number in ground_truth to 0
 
 Previous Next
 ===============================================================================
 © Copyright 2023, Space Force.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.math.html` & `satsim-0.15.0/docs/_build/html/api/satsim.math.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.math package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.math package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.pipeline.html` & `satsim-0.15.0/docs/_build/html/api/satsim.pipeline.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.pipeline package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.pipeline package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.time.html` & `satsim-0.15.0/docs/_build/html/api/satsim.time.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.time package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.time package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.util.html` & `satsim-0.15.0/docs/_build/html/api/satsim.util.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.util package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.util package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -175,14 +175,20 @@
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><strong>module</strong> – <cite>object</cite>, a module which has __version__ as a string in semantic format</p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py function">
+<dt class="sig sig-object py" id="satsim.util.system.is_tensorflow_running_on_cpu">
+<span class="sig-prename descclassname"><span class="pre">satsim.util.system.</span></span><span class="sig-name descname"><span class="pre">is_tensorflow_running_on_cpu</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#satsim.util.system.is_tensorflow_running_on_cpu" title="Permalink to this definition"></a></dt>
+<dd><p>Returns True if TensorFlow is running on the CPU.</p>
+</dd></dl>
+
 </section>
 <section id="module-satsim.util.thread">
 <span id="satsim-util-thread-module"></span><h2>satsim.util.thread module<a class="headerlink" href="#module-satsim.util.thread" title="Permalink to this heading"></a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="satsim.util.thread.MultithreadedTaskQueue">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">satsim.util.thread.</span></span><span class="sig-name descname"><span class="pre">MultithreadedTaskQueue</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">num_threads</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">5</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.util.thread.MultithreadedTaskQueue" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -77,14 +77,16 @@
 
       ver = get_semantic_version(tf)
 
       # example ver == [2,0,0]
         Parameters:
             module âobject, a module which has __version__ as a string in
             semantic format
+  satsim.util.system.is_tensorflow_running_on_cpu()ï
+      Returns True if TensorFlow is running on the CPU.
 
 ***** satsim.util.thread moduleï *****
   classsatsim.util.thread.MultithreadedTaskQueue(num_threads=5)ï
       Bases: object
       Class to run functions round robin.
         has_tag(tag)ï
         stop()ï
```

### Comparing `satsim-0.14.0/docs/_build/html/api/satsim.vecmath.html` & `satsim-0.15.0/docs/_build/html/api/satsim.vecmath.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.vecmath package &mdash; SatSim 0.14.0 documentation</title>
+  <title>satsim.vecmath package &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
```

### Comparing `satsim-0.14.0/docs/_build/html/api.html` & `satsim-0.15.0/docs/_build/html/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>API Documentation &mdash; SatSim 0.14.0 documentation</title>
+  <title>API Documentation &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -358,14 +358,15 @@
 <li class="toctree-l3"><a class="reference internal" href="api/satsim.util.html">satsim.util package</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#submodules">Submodules</a></li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#module-satsim.util.system">satsim.util.system module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_eager"><code class="docutils literal notranslate"><span class="pre">configure_eager()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_multi_gpu"><code class="docutils literal notranslate"><span class="pre">configure_multi_gpu()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_single_gpu"><code class="docutils literal notranslate"><span class="pre">configure_single_gpu()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.get_semantic_version"><code class="docutils literal notranslate"><span class="pre">get_semantic_version()</span></code></a></li>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.is_tensorflow_running_on_cpu"><code class="docutils literal notranslate"><span class="pre">is_tensorflow_running_on_cpu()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#module-satsim.util.thread">satsim.util.thread module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.thread.MultithreadedTaskQueue"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue</span></code></a><ul>
 <li class="toctree-l6"><a class="reference internal" href="api/satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.has_tag"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.has_tag()</span></code></a></li>
 <li class="toctree-l6"><a class="reference internal" href="api/satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.stop"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.stop()</span></code></a></li>
 <li class="toctree-l6"><a class="reference internal" href="api/satsim.util.html#satsim.util.thread.MultithreadedTaskQueue.task"><code class="docutils literal notranslate"><span class="pre">MultithreadedTaskQueue.task()</span></code></a></li>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -203,14 +203,15 @@
                 # satsim.util_package
                       # Submodules
                       # satsim.util.system_module
                             # configure_eager()
                             # configure_multi_gpu()
                             # configure_single_gpu()
                             # get_semantic_version()
+                            # is_tensorflow_running_on_cpu()
                       # satsim.util.thread_module
                             # MultithreadedTaskQueue
                                   # MultithreadedTaskQueue.has_tag()
                                   # MultithreadedTaskQueue.stop()
                                   # MultithreadedTaskQueue.task()
                                   # MultithreadedTaskQueue.waitUntilEmpty()
                             # ThreadedTaskQueue
```

### Comparing `satsim-0.14.0/docs/_build/html/authors.html` & `satsim-0.15.0/docs/_build/html/authors.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Credits &mdash; SatSim 0.14.0 documentation</title>
+  <title>Credits &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.14.0/docs/_build/html/contributing.html` & `satsim-0.15.0/docs/_build/html/contributing.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Contributing &mdash; SatSim 0.14.0 documentation</title>
+  <title>Contributing &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
           o Getting_Started_for_Developers
           o Merge_Request_Guidelines
```

### Comparing `satsim-0.14.0/docs/_build/html/genindex.html` & `satsim-0.15.0/docs/_build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; SatSim 0.14.0 documentation</title>
+  <title>Index &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -753,14 +753,16 @@
 </li>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Matrix3.Matrix3.inverseTranspose">inverseTranspose() (satsim.vecmath.Matrix3.Matrix3 static method)</a>
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Matrix4.Matrix4.inverseTranspose">(satsim.vecmath.Matrix4.Matrix4 static method)</a>
 </li>
       </ul></li>
+      <li><a href="api/satsim.util.html#satsim.util.system.is_tensorflow_running_on_cpu">is_tensorflow_running_on_cpu() (in module satsim.util.system)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="L">L</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/satsim.math.html#satsim.math.interpolate.lagrange">lagrange() (in module satsim.math.interpolate)</a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
@@ -302,28 +302,30 @@
 ***** H *****
                                 * has_tag()_
     * has_key_deep()_(in          (satsim.util.thread.MultithreadedTaskQueue
       module_satsim.config)       method)
                                       o (satsim.util.thread.ThreadedTaskQueue
                                         method)
 ***** I *****
-    * IDENTITY()_                               * inverse()_(satsim.vecmath.Matrix3.Matrix3
-      (satsim.vecmath.Matrix2.Matrix2             static_method)
-      static_method)                                  o (satsim.vecmath.Matrix4.Matrix4
-          o (satsim.vecmath.Matrix3.Matrix3             static_method)
-            static_method)                            o (satsim.vecmath.Quaternion.Quaternion
-          o (satsim.vecmath.Matrix4.Matrix4             static_method)
-            static_method)                      * inverseTransformation()_
-    * image_generator()_(in_module                (satsim.vecmath.Matrix4.Matrix4_static
-      satsim.satsim)                              method)
-    * init_annotation()_(in_module              * inverseTranspose()_
-      satsim.io.satnet)                           (satsim.vecmath.Matrix3.Matrix3_static
-    * interp_degrees()_(in_module                 method)
-      satsim.math.angle)                              o (satsim.vecmath.Matrix4.Matrix4
-                                                        static_method)
+                                                * inverse()_(satsim.vecmath.Matrix3.Matrix3
+    * IDENTITY()_                                 static_method)
+      (satsim.vecmath.Matrix2.Matrix2                 o (satsim.vecmath.Matrix4.Matrix4
+      static_method)                                    static_method)
+          o (satsim.vecmath.Matrix3.Matrix3           o (satsim.vecmath.Quaternion.Quaternion
+            static_method)                              static_method)
+          o (satsim.vecmath.Matrix4.Matrix4     * inverseTransformation()_
+            static_method)                        (satsim.vecmath.Matrix4.Matrix4_static
+    * image_generator()_(in_module                method)
+      satsim.satsim)                            * inverseTranspose()_
+    * init_annotation()_(in_module                (satsim.vecmath.Matrix3.Matrix3_static
+      satsim.io.satnet)                           method)
+    * interp_degrees()_(in_module                     o (satsim.vecmath.Matrix4.Matrix4
+      satsim.math.angle)                                static_method)
+                                                * is_tensorflow_running_on_cpu()_(in_module
+                                                  satsim.util.system)
 ***** L *****
     * lagrange()_(in_module                           * load_json()_(in_module_satsim.config)
       satsim.math.interpolate)                        * load_moon()_(in_module
     * lambertian_sphere_to_mv()_(in_module              satsim.geometry.astrometric)
       satsim.geometry.astrometric)                    * load_sprite_from_file()_(in_module
     * lerp()_                                           satsim.geometry.sprite)
       (satsim.vecmath.Cartesian2.Cartesian2           * load_stars_for_zone()_(in_module
```

### Comparing `satsim-0.14.0/docs/_build/html/history.html` & `satsim-0.15.0/docs/_build/html/history.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>History &mdash; SatSim 0.14.0 documentation</title>
+  <title>History &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -46,37 +46,38 @@
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="contributing.html">Contributing</a></li>
 <li class="toctree-l1"><a class="reference internal" href="api.html">API Documentation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#id1">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id2">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id3">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id4">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id5">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id6">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id7">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id8">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id9">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id10">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id12">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id13">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id14">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id15">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id16">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id17">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id18">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id19">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id20">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id21">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id22">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id23">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id1">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id2">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id3">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id4">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id5">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id6">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id7">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id8">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id9">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id10">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id12">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id13">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id14">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id15">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id16">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id17">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id18">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id19">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id20">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id21">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id22">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id23">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id24">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -100,218 +101,228 @@
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="history">
 <h1>History<a class="headerlink" href="#history" title="Permalink to this heading"></a></h1>
 <section id="id1">
-<h2>0.14.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
-<p>Add vector math library.
-Add CZML output for sensor visualization.
-Fix objects not updating properly when image renderer is off.</p>
+<h2>0.15.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<ul class="simple">
+<li><p>Add support to save ground truth image data to the Annotations directory. Set sim option <cite>save_ground_truth</cite> to <cite>true</cite>.</p></li>
+<li><p>Add support for running on CPU with no GPU acceleration.</p></li>
+<li><p>Add CZML options for sensor visualization and object billboard image.</p></li>
+</ul>
 </section>
 <section id="id2">
-<h2>0.13.1<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
+<h2>0.14.0<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
+<ul class="simple">
+<li><p>Add vector math library.</p></li>
+<li><p>Add CZML output for sensor visualization.</p></li>
+<li><p>Fix objects not updating properly when image renderer is off.</p></li>
+</ul>
+</section>
+<section id="id3">
+<h2>0.13.1<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add argument to set folder name in <cite>gen_multi</cite>.</p></li>
 <li><p>Add environment variable, <cite>SATSIM_SKYFIELD_LOAD_DIR</cite>, to specify location of Skyfield ephemeris files.</p></li>
 <li><p>Fix incorrect CZML output when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id3">
-<h2>0.13.0<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
+<section id="id4">
+<h2>0.13.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add ephemeris objects that are propagated with the Lagrange interpolator.</p></li>
 <li><p>Add Cesium CZML output. Set sim option <cite>save_czml</cite> to <cite>false</cite> to disable.</p></li>
 <li><p>Add CSV text file star catalog loader. This feature is useful for small catalogs such as Hipparcos and simulating wide FOV sensors.</p></li>
 <li><p>Add multiplier and clipping for radial cosine.</p></li>
 <li><p>Add option to skip image rendering. Set sim option <cite>mode</cite> to <cite>none</cite> to bypass image rendering.</p></li>
 <li><p>Update interfaces for newest version of Skyfield, Poliastro, POPPY, and AstroPy.</p></li>
 <li><p>Fix star renderer issue removing stars in field of view for non-square arrays.</p></li>
 </ul>
 </section>
-<section id="id4">
-<h2>0.12.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
+<section id="id5">
+<h2>0.12.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add augmentation of SatNet <cite>tf.data.Dataset</cite>. This feature allows injecting synthetic targets into real data during training.</p></li>
 <li><p>Add FFT convolution to <cite>add_patch</cite> sprite render and <cite>scatter_shift</cite> image augmenter for speed improvement.</p></li>
 <li><p>Add cache last PSF FFT to <cite>fftconv2p</cite> for speed improvement for static PSFs.</p></li>
 <li><p>Add two-body state vector as a trackable target.</p></li>
 <li><p>Add moon and sun model and misc methods to calculate phase angle and target brightness.</p></li>
 </ul>
 </section>
-<section id="id5">
-<h2>0.11.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
+<section id="id6">
+<h2>0.11.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to render star motion with FFT. Set sim option <cite>star_render_mode</cite> to <cite>fft</cite>.</p></li>
 <li><p>Add option to sample photon noise multiple times. Set sim option <cite>num_shot_noise_samples</cite> to integer number.</p></li>
 <li><p>Add support to render a satellite as a sprite. Set <cite>model</cite> option in obs.</p></li>
 <li><p>Add support to load and augment sprite model with <cite>$pipeline</cite> operator.</p></li>
 <li><p>Add cropped POPPY PSF generation.</p></li>
 <li><p>Fix GreatCircle propagator tracking offset.</p></li>
 <li><p>Fix runtime exception when site and track_mode are not defined.</p></li>
 <li><p>Add TensorFlow 2.6 and update TensorFlow 2.2 and 2.4 Docker build file.</p></li>
 </ul>
 </section>
-<section id="id6">
-<h2>0.10.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
+<section id="id7">
+<h2>0.10.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for piecewise rendering. Set sim option <cite>render_size</cite> to enable. For example, [256, 256].</p></li>
 <li><p>Add <cite>fixed</cite> tracking mode with mount azimuth and elevation.</p></li>
 <li><p>Add great circle propagator for targets.</p></li>
 <li><p>Add in-memory image generation. See generator function <cite>image_generator</cite>.</p></li>
 <li><p>Fix missing stars when FOV crosses zero degree RA.</p></li>
 <li><p>Add curved targets using bezier curve raster. Enabled by default. Set sim option <cite>num_target_samples</cite> to 2 to enable linear raster.</p></li>
 <li><p>Add LRU cache to star catalog reader.</p></li>
 <li><p>Add option to turn off SNR calculation. Set sim option <cite>calculate_snr</cite> to false will render targets and stars together.</p></li>
 <li><p>Handle unstable SGP4 TLEs.</p></li>
 <li><p>Add TensorFlow 2.4 Docker build file.</p></li>
 <li><p>Add debug output for pristine images of targets and stars.</p></li>
 </ul>
 </section>
-<section id="id7">
-<h2>0.9.1<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
+<section id="id8">
+<h2>0.9.1<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Calculate POPPY input wavefront resolution to avoid PSF aliasing.</p></li>
 <li><p>Add support for additional FITS image data types (<cite>int16</cite>, <cite>uint16</cite>, <cite>int32</cite>, <cite>uint32</cite>, <cite>float32</cite>).</p></li>
 <li><p>Add batch processing to <cite>transform_and_add_counts</cite> to support batch processing of stars.</p></li>
 <li><p>Add <cite>auto</cite> option to calculate temporal oversample factor based on star velocities.</p></li>
 <li><p>Add option to turn off serializing config data to pickle file (<cite>save_pickle</cite>).</p></li>
 <li><p>Add option to turn off png movie output (<cite>save_movie</cite>).</p></li>
 <li><p>Add <cite>crop_and_resize</cite> and <cite>flip</cite> image augmentation.</p></li>
 <li><p>Set pixels with values beyond the pixel data type’s capacity to the maximum value for that data type.</p></li>
 <li><p>Add <cite>lognormal</cite> function to generate a distribution with a true target mean.</p></li>
 <li><p>Fix issue with sidereal track.</p></li>
 <li><p>Fix issue with fragment velocity not being randomly sampled.</p></li>
 </ul>
 </section>
-<section id="id8">
-<h2>0.9.0<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
+<section id="id9">
+<h2>0.9.0<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add Physical Optics Propagation in Python (POPPY) PSF generation.</p></li>
 <li><p>Add PSF augmentation with <cite>$pipeline</cite> replacement key.</p></li>
 <li><p>Add <cite>$function</cite> and <cite>$compound</cite> replacement key.</p></li>
 <li><p>Add ability to generate stray light from a <cite>$function</cite> replacement key.</p></li>
 <li><p>Add built-in 2D polynomial image generator for stray light, <cite>polygrid2d</cite>.</p></li>
 <li><p>Add built-in cosine fourth image generator for irradiance falloff, <cite>radial_cos2d</cite>.</p></li>
 <li><p>Add built-in sine wave image generator for fix pattern noise, <cite>sin2d</cite>.</p></li>
 <li><p>Add built-in image generator from AstroPy model, <cite>astropy_model2d</cite>.</p></li>
 <li><p>Add built-in image augmentation, <cite>scatter_shift</cite> and <cite>scatter_shift_polar</cite>.</p></li>
 <li><p>Add <cite>$cache</cite> replacement key (caching works for PSF and <cite>$function</cite>).</p></li>
 </ul>
 </section>
-<section id="id9">
-<h2>0.8.3<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
+<section id="id10">
+<h2>0.8.3<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix new Skyfield incompatibility.</p></li>
 </ul>
 </section>
-<section id="id10">
-<h2>0.8.2<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
+<section id="id11">
+<h2>0.8.2<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Prefix replacement keys with <cite>$</cite> in SatSim configuration file.</p></li>
 <li><p>Add option to scale collision fragments by cosine of the exit angle.</p></li>
 </ul>
 </section>
-<section id="id11">
-<h2>0.8.1<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
+<section id="id12">
+<h2>0.8.1<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add astrometric metadata into FITS header</p></li>
 <li><p>Refactor WCS library</p></li>
 <li><p>Add option to flip images about x or y axis</p></li>
 <li><p>Add option to refresh stars for each frame</p></li>
 <li><p>Add RPO from TLE generator</p></li>
 </ul>
 </section>
-<section id="id12">
-<h2>0.8.0<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
+<section id="id13">
+<h2>0.8.0<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add two body propagator</p></li>
 <li><p>Add object <cite>create</cite>, <cite>delete</cite>, and <cite>update</cite> events</p></li>
 <li><p>Add collision generator</p></li>
 <li><p>Add breakup generator</p></li>
 <li><p>Add <cite>ref</cite> keyword to configuration</p></li>
 <li><p>Add <cite>key</cite> keyword to <cite>import</cite> configuration</p></li>
 <li><p>Refactor astrometric library</p></li>
 </ul>
 </section>
-<section id="id13">
-<h2>0.7.2<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
+<section id="id14">
+<h2>0.7.2<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to specify star and obs velocity in polar coordinates</p></li>
 </ul>
 </section>
-<section id="id14">
-<h2>0.7.1<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
+<section id="id15">
+<h2>0.7.1<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to turn off shot noise: <cite>sim.enable_shot_noise: true</cite></p></li>
 <li><p>Add option to turn off annotation boxes in image: <cite>sim.show_obs_boxes: true</cite></p></li>
 <li><p>Add option to specify velocity in arcseconds: <cite>sim.velocity_units: arcsec</cite></p></li>
 <li><p>Fix PNG output threading issue</p></li>
 </ul>
 </section>
-<section id="id15">
-<h2>0.7.0<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
+<section id="id16">
+<h2>0.7.0<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add function pipelines to support variable target brightness</p></li>
 </ul>
 </section>
-<section id="id16">
-<h2>0.6.1<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
+<section id="id17">
+<h2>0.6.1<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix built-in generators not included in distribution</p></li>
 <li><p>Add dockerfile</p></li>
 </ul>
 </section>
-<section id="id17">
-<h2>0.6.0<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
+<section id="id18">
+<h2>0.6.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add configuration import.</p></li>
 <li><p>Add configuration generator functions.</p></li>
 <li><p>Add built-in generator for breakups.</p></li>
 <li><p>Add built-in generator for CSOs.</p></li>
 <li><p>Add built-in generator for loading TLE files.</p></li>
 </ul>
 </section>
-<section id="id18">
-<h2>0.5.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
+<section id="id19">
+<h2>0.5.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Runtime optimization.</p></li>
 <li><p>Add parallel processing and multi-gpu utilization.</p></li>
 <li><p>Add option to limit gpu memory usage.</p></li>
 </ul>
 </section>
-<section id="id19">
-<h2>0.4.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
+<section id="id20">
+<h2>0.4.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add signal to noise calculation for target pixels.</p></li>
 </ul>
 </section>
-<section id="id20">
-<h2>0.3.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
+<section id="id21">
+<h2>0.3.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for two line element set SGP4 satellite propagator.</p></li>
 <li><p>Add support for rate and sidereal track from topocentric site.</p></li>
 </ul>
 </section>
-<section id="id21">
-<h2>0.2.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
+<section id="id22">
+<h2>0.2.0<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for SSTR7 star catalog.</p></li>
 </ul>
 </section>
-<section id="id22">
-<h2>0.1.1<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
+<section id="id23">
+<h2>0.1.1<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add target position to annotation file.</p></li>
 <li><p>Updates to run GitLab CI.</p></li>
 </ul>
 </section>
-<section id="id23">
-<h2>0.1.0<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
+<section id="id24">
+<h2>0.1.0<a class="headerlink" href="#id24" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>First release.</p></li>
 </ul>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
     * History
+          o 0.15.0
           o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
           o 0.9.1
@@ -38,17 +39,24 @@
           o 0.1.1
           o 0.1.0
    SatSim
     * History
     * View_page_source
 ===============================================================================
 ****** Historyï ******
+***** 0.15.0ï *****
+    * Add support to save ground truth image data to the Annotations directory.
+      Set sim optionsave_ground_truthtotrue.
+    * Add support for running on CPU with no GPU acceleration.
+    * Add CZML options for sensor visualization and object billboard image.
+
 ***** 0.14.0ï *****
-Add vector math library. Add CZML output for sensor visualization. Fix objects
-not updating properly when image renderer is off.
+    * Add vector math library.
+    * Add CZML output for sensor visualization.
+    * Fix objects not updating properly when image renderer is off.
 
 ***** 0.13.1ï *****
     * Add argument to set folder name ingen_multi.
     * Add environment variable,SATSIM_SKYFIELD_LOAD_DIR, to specify location of
       Skyfield ephemeris files.
     * Fix incorrect CZML output when image renderer is off.
```

### Comparing `satsim-0.14.0/docs/_build/html/index.html` & `satsim-0.15.0/docs/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Documentation for SatSim &mdash; SatSim 0.14.0 documentation</title>
+  <title>Documentation for SatSim &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -106,37 +106,38 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#development-lead">Development Lead</a></li>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#contributors">Contributors</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id24">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
@@ -35,14 +35,15 @@
           o Other_Ways_of_Contributing
     * API_Documentation
           o satsim_package
     * Credits
           o Development_Lead
           o Contributors
     * History
+          o 0.15.0
           o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
           o 0.9.1
```

### Comparing `satsim-0.14.0/docs/_build/html/installation.html` & `satsim-0.15.0/docs/_build/html/installation.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; SatSim 0.14.0 documentation</title>
+  <title>Installation &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
           o Stable_Release
           o From_Sources
     * Usage
     * Contributing
```

### Comparing `satsim-0.14.0/docs/_build/html/py-modindex.html` & `satsim-0.15.0/docs/_build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; SatSim 0.14.0 documentation</title>
+  <title>Python Module Index &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.14.0/docs/_build/html/search.html` & `satsim-0.15.0/docs/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; SatSim 0.14.0 documentation</title>
+  <title>Search &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.14.0/docs/_build/html/searchindex.js` & `satsim-0.15.0/docs/_build/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -124,15 +124,15 @@
         "czml": [0, 1, 15],
         "czmlextractor": [0, 1, 7],
         "add_ground_st": [0, 1, 7],
         "add_object": [0, 1, 7],
         "get_docu": [0, 1, 7],
         "save_czml": [0, 1, 7, 15],
         "fit": [0, 1, 5, 6, 8, 15],
-        "save": [0, 1, 7],
+        "save": [0, 1, 7, 15],
         "save_apng": [0, 1, 7],
         "satnet": [0, 1, 2, 15, 18],
         "init_annot": [0, 1, 7],
         "set_frame_annot": [0, 1, 7],
         "write_fram": [0, 1, 7],
         "math": [0, 1, 15],
         "angl": [0, 1, 4, 5, 6, 12, 15],
@@ -175,14 +175,15 @@
         "utc_from_list_or_scalar": [0, 1, 10],
         "util": [0, 1, 15, 18],
         "system": [0, 1, 5, 6, 14],
         "configure_eag": [0, 1, 11],
         "configure_multi_gpu": [0, 1, 11],
         "configure_single_gpu": [0, 1, 11],
         "get_semantic_vers": [0, 1, 11],
+        "is_tensorflow_running_on_cpu": [0, 1, 11],
         "thread": [0, 1, 15],
         "multithreadedtaskqueu": [0, 1, 11],
         "has_tag": [0, 1, 11],
         "stop": [0, 1, 5, 11],
         "task": [0, 1, 11],
         "waituntilempti": [0, 1, 11],
         "threadedtaskqueu": [0, 1, 11],
@@ -367,15 +368,15 @@
         "param": [1, 6],
         "onto": [1, 2, 5, 12],
         "which": [1, 5, 6, 8, 11, 12, 18],
         "execut": [1, 11],
         "d": [1, 5],
         "check": [1, 14, 18],
         "see": [1, 5, 6, 8, 15, 17, 18],
-        "dictionari": [1, 5, 6, 11, 18],
+        "dictionari": [1, 5, 6, 7, 11, 18],
         "ha": [1, 5, 6, 11],
         "paramet": [1, 2, 4, 5, 6, 7, 8, 10, 11, 12, 16],
         "list": [1, 2, 4, 5, 6, 7, 8, 10, 11, 12, 18],
         "str": [1, 4, 5, 7, 11],
         "name": [1, 5, 7, 8, 11, 14, 15],
         "filenam": [1, 2, 4, 5, 6, 7, 18],
         "open": 1,
@@ -427,29 +428,29 @@
         "string": [1, 2, 4, 5, 6, 7, 8, 11],
         "option": [1, 15, 18],
         "dirnam": [1, 7],
         "none": [1, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 15, 17, 18],
         "run_gener": 1,
         "eval_python": 1,
         "run_compound": 1,
-        "ani": [1, 6, 12, 14, 17, 18],
+        "ani": [1, 6, 7, 12, 14, 17, 18],
         "children": 1,
         "sampl": [1, 4, 6, 7, 8, 10, 15, 18],
         "content": [1, 11],
         "pickl": [1, 15],
         "els": 1,
         "special": 1,
         "ar": [1, 2, 4, 5, 6, 8, 11, 12, 14, 15, 18],
         "found": 1,
         "root": [1, 5, 6],
-        "directori": [1, 5, 7, 14, 17, 18],
+        "directori": [1, 5, 7, 14, 15, 17, 18],
         "referenc": 1,
         "evalu": [1, 6],
         "dure": [1, 5, 6, 15],
-        "thi": [1, 4, 5, 6, 8, 10, 11, 12, 14, 15, 17, 18],
+        "thi": [1, 4, 5, 6, 7, 8, 10, 11, 12, 14, 15, 17, 18],
         "pass": [1, 5, 12, 14],
         "origin": [1, 4, 5, 6, 14, 18],
         "format": [1, 5, 6, 7, 11],
         "distribut": [1, 4, 6, 8, 15, 18],
         "where": [1, 5, 6, 11, 12],
         "numpi": [1, 5, 6, 7, 8, 18],
         "p": [1, 5],
@@ -692,15 +693,15 @@
         "507130983802519": 4,
         "09979647598905288": 4,
         "1819183509832407": 4,
         "26064801046837316": 4,
         "2893265228436015": 4,
         "1736509022094605": 4,
         "22670133968196546": 4,
-        "15": [4, 6, 12, 18],
+        "15": [4, 6, 12, 16, 18],
         "16": [4, 12, 18],
         "separ": 4,
         "space": [4, 6, 8, 10, 12],
         "per": [4, 5, 6, 8, 18],
         "mode": [4, 5, 6, 11, 15, 18],
         "05": 4,
         "95": 4,
@@ -886,19 +887,19 @@
         "across": [5, 6],
         "inject": [5, 15],
         "move": 5,
         "oversampl": [5, 6, 15],
         "sec": [5, 6, 18],
         "g": [5, 6, 8],
         "larger": [5, 6, 8],
-        "than": [5, 6, 8, 12],
+        "than": [5, 6, 7, 8, 12],
         "segment": [5, 8],
         "5120": 5,
         "bottom": [5, 12],
-        "order": [5, 6, 8, 12],
+        "order": [5, 6, 7, 8, 12],
         "vectorfunct": 5,
         "399": 5,
         "itrf": 5,
         "6045": 5,
         "3490": 5,
         "2500": 5,
         "457": 5,
@@ -937,15 +938,15 @@
         "60": [5, 7, 18],
         "numdeczon": 5,
         "1800": 5,
         "sstrc": 5,
         "index": [5, 11, 12, 16],
         "entri": [5, 14],
         "differ": [5, 6, 8, 12],
-        "acceler": 5,
+        "acceler": [5, 15],
         "zone": 5,
         "store": [5, 12],
         "unsign": [5, 12],
         "integ": [5, 11, 15],
         "po": [5, 7],
         "currentzon": 5,
         "region": 5,
@@ -1179,15 +1180,15 @@
         "secondary_radiu": 6,
         "110": [6, 18],
         "n_support": 6,
         "support_width": 6,
         "010": 6,
         "zernikewf": 6,
         "100e": 6,
-        "9": [6, 7, 12, 16, 18],
+        "9": [6, 12, 16, 18],
         "300e": 6,
         "600e": 6,
         "900e": 6,
         "11": [6, 12, 16, 18],
         "512": [6, 18],
         "shape": [6, 8],
         "h_fpa_o": 6,
@@ -1242,15 +1243,28 @@
         "label_outline_color": 7,
         "label_font": 7,
         "16pt": 7,
         "lucida": 7,
         "consol": 7,
         "label_text": 7,
         "label_show": 7,
-        "ground": 7,
+        "billboard_show": 7,
+        "billboard_imag": 7,
+        "png": [7, 15],
+        "base64": 7,
+        "ivborw0kggoaaaansuheugaaabaaaaaqcayaaaaf8": 7,
+        "9haaaaaxnsr0iars4c6qaaaarnqu1baacxjwv8yquaaaajcehzcwaadsmaaa7dacdvqgqaaacvsurbvdhprzdrdcmgdau9gqn0lizijw6subjjyguenqgsqepjtyhg91lvvpwddfxm3t9tsl1exzvdwii471fivk73cbffqntt": 7,
+        "d2kogpfgopsikhupgumxq9dfeswv4ixhlycnhbfnzcfeeuyqbiulnwwgmtdrz3jbqfoevg53rd8ztg9apjmnbuqf": 7,
+        "vfrabjewnls0rfjbkylja8fkt5sedys1qwyv8t0b": 7,
+        "5c2zmh2": 7,
+        "etgnnbgmmaaaaaelftksuqmcc": 7,
+        "cone_color": 7,
+        "64": 7,
+        "cone_show": 7,
+        "ground": [7, 15],
         "station": 7,
         "unit": [7, 12],
         "altitud": [7, 18],
         "descript": [7, 14],
         "fill": 7,
         "color": 7,
         "rgba": 7,
@@ -1267,32 +1281,34 @@
         "path_width": 7,
         "path_show": 7,
         "path_color": 7,
         "start_interv": 7,
         "end_interv": 7,
         "start_avail": 7,
         "end_avail": 7,
-        "billboard_show": 7,
+        "9haaaaaxnsr0iars4c6qaaaarnqu1baacxjwv8yquaaaajcehzcwaadsmaaa7dacdvqgqaaadjsurbvdhpnzhrdcmgeemzjveypanklizseflfd4qnnxajsfwfho7w2zc0tf9qg2rxrezsuezlogm47woh95x3hl3jegilvdgsoqutqsnl68ezewn1vae6lceseeyvvwnt": 7,
+        "rxc4cxqngadho1nxoj": 7,
+        "9iaqc2xi2xbt23pjcdib6tqjoc6bho": 7,
+        "sdy3fbqt8prvhibu7ybfceparxooetwbwbycoyf9vgp1byi1ba": 7,
+        "eehhmfzkbbojeqwn1yzuztyspiquha85mpknixb7gizqdeecsaaaaasuvork5cyii": 7,
         "retriev": [7, 12],
         "document": 7,
         "obs_cach": 7,
         "scenario": 7,
         "exposure_tim": 7,
         "dt_start": 7,
         "datetim": 7,
         "2023": 7,
-        "13": [7, 12, 16, 18],
-        "49": 7,
-        "34": 7,
-        "855695": 7,
+        "43": 7,
+        "45": 7,
+        "661952": 7,
         "header": [7, 15],
         "overwrit": 7,
         "np": 7,
         "exposur": [7, 18],
-        "datatim": 7,
         "placehold": [7, 18],
         "implement": [7, 10, 12, 14],
         "exist": [7, 12],
         "int16": [7, 15],
         "int32": [7, 15],
         "uint32": [7, 15],
         "vauto": 7,
@@ -1303,26 +1319,30 @@
         "show_obs_box": [7, 15],
         "median": [7, 8],
         "colormap": 7,
         "limit": [7, 11, 15],
         "arr": 7,
         "regist": 7,
         "jpg": 7,
-        "png": [7, 15],
         "anim": 7,
         "web": [7, 14],
         "browser": 7,
         "sequenc": 7,
         "init": 7,
         "box_siz": 7,
         "dir_nam": 7,
         "sat_nam": 7,
         "meta_data": 7,
         "time_stamp": 7,
         "save_jpeg": 7,
+        "ground_truth": 7,
+        "ground_truth_min": 7,
+        "jpeg": 7,
+        "ordereddict": 7,
+        "less": [7, 12],
         "a0": 8,
         "a1": 8,
         "max_diff": 8,
         "180": [8, 18],
         "crossov": 8,
         "concid": 8,
         "opposit": 8,
@@ -1397,14 +1417,15 @@
         "semat": 11,
         "version": [11, 14, 15, 17, 18],
         "non": [11, 12, 15],
         "charact": 11,
         "ver": 11,
         "__version__": 11,
         "semant": 11,
+        "cpu": [11, 15],
         "num_thread": 11,
         "round": 11,
         "robin": 11,
         "tag": [11, 14],
         "next": 11,
         "keyword": [11, 15, 18],
         "block": 11,
@@ -1493,14 +1514,15 @@
         "2by2": 12,
         "schur": 12,
         "decomposit": 12,
         "largest": 12,
         "help": [12, 14, 18],
         "reduc": 12,
         "4x4": 12,
+        "13": [12, 16, 18],
         "14": [12, 16, 18],
         "infinit": 12,
         "perspect": 12,
         "below": 12,
         "abov": 12,
         "far": 12,
         "look": 12,
@@ -1521,15 +1543,14 @@
         "except": [12, 15, 18],
         "thrown": 12,
         "proper": 12,
         "rigid": 12,
         "link": 12,
         "verifi": 12,
         "optim": [12, 15],
-        "less": 12,
         "arithmet": 12,
         "implicit": 12,
         "rightmost": 12,
         "q0": 12,
         "q1": 12,
         "q2": 12,
         "inner": 12,
@@ -1636,14 +1657,17 @@
         "send": 14,
         "propos": 14,
         "explain": 14,
         "keep": 14,
         "scope": 14,
         "narrow": 14,
         "easier": 14,
+        "truth": 15,
+        "save_ground_truth": 15,
+        "billboard": 15,
         "librari": 15,
         "properli": 15,
         "satsim_skyfield_load_dir": 15,
         "incorrect": 15,
         "csv": 15,
         "loader": 15,
         "small": 15,
@@ -2124,15 +2148,16 @@
             [11, 0, 0, "-", "thread"],
             [11, 0, 0, "-", "timer"]
         ],
         "satsim.util.system": [
             [11, 1, 1, "", "configure_eager"],
             [11, 1, 1, "", "configure_multi_gpu"],
             [11, 1, 1, "", "configure_single_gpu"],
-            [11, 1, 1, "", "get_semantic_version"]
+            [11, 1, 1, "", "get_semantic_version"],
+            [11, 1, 1, "", "is_tensorflow_running_on_cpu"]
         ],
         "satsim.util.thread": [
             [11, 2, 1, "", "MultithreadedTaskQueue"],
             [11, 2, 1, "", "ThreadedTaskQueue"]
         ],
         "satsim.util.thread.MultithreadedTaskQueue": [
             [11, 4, 1, "", "has_tag"],
@@ -2585,14 +2610,15 @@
         "report": 14,
         "bug": 14,
         "write": 14,
         "submit": 14,
         "feedback": 14,
         "histori": 15,
         "0": 15,
+        "15": 15,
         "14": 15,
         "13": 15,
         "1": 15,
         "12": 15,
         "11": 15,
         "10": 15,
         "9": 15,
@@ -2863,83 +2889,86 @@
         ],
         "Submit Feedback": [
             [14, "submit-feedback"]
         ],
         "History": [
             [15, "history"]
         ],
-        "0.14.0": [
+        "0.15.0": [
             [15, "id1"]
         ],
-        "0.13.1": [
+        "0.14.0": [
             [15, "id2"]
         ],
-        "0.13.0": [
+        "0.13.1": [
             [15, "id3"]
         ],
-        "0.12.0": [
+        "0.13.0": [
             [15, "id4"]
         ],
-        "0.11.0": [
+        "0.12.0": [
             [15, "id5"]
         ],
-        "0.10.0": [
+        "0.11.0": [
             [15, "id6"]
         ],
-        "0.9.1": [
+        "0.10.0": [
             [15, "id7"]
         ],
-        "0.9.0": [
+        "0.9.1": [
             [15, "id8"]
         ],
-        "0.8.3": [
+        "0.9.0": [
             [15, "id9"]
         ],
-        "0.8.2": [
+        "0.8.3": [
             [15, "id10"]
         ],
-        "0.8.1": [
+        "0.8.2": [
             [15, "id11"]
         ],
-        "0.8.0": [
+        "0.8.1": [
             [15, "id12"]
         ],
-        "0.7.2": [
+        "0.8.0": [
             [15, "id13"]
         ],
-        "0.7.1": [
+        "0.7.2": [
             [15, "id14"]
         ],
-        "0.7.0": [
+        "0.7.1": [
             [15, "id15"]
         ],
-        "0.6.1": [
+        "0.7.0": [
             [15, "id16"]
         ],
-        "0.6.0": [
+        "0.6.1": [
             [15, "id17"]
         ],
-        "0.5.0": [
+        "0.6.0": [
             [15, "id18"]
         ],
-        "0.4.0": [
+        "0.5.0": [
             [15, "id19"]
         ],
-        "0.3.0": [
+        "0.4.0": [
             [15, "id20"]
         ],
-        "0.2.0": [
+        "0.3.0": [
             [15, "id21"]
         ],
-        "0.1.1": [
+        "0.2.0": [
             [15, "id22"]
         ],
-        "0.1.0": [
+        "0.1.1": [
             [15, "id23"]
         ],
+        "0.1.0": [
+            [15, "id24"]
+        ],
         "Documentation for SatSim": [
             [16, "documentation-for-satsim"]
         ],
         "Contents:": [
             [16, null]
         ],
         "Indices and tables": [
@@ -3628,14 +3657,17 @@
         ],
         "has_tag() (satsim.util.thread.multithreadedtaskqueue method)": [
             [11, "satsim.util.thread.MultithreadedTaskQueue.has_tag"]
         ],
         "has_tag() (satsim.util.thread.threadedtaskqueue method)": [
             [11, "satsim.util.thread.ThreadedTaskQueue.has_tag"]
         ],
+        "is_tensorflow_running_on_cpu() (in module satsim.util.system)": [
+            [11, "satsim.util.system.is_tensorflow_running_on_cpu"]
+        ],
         "satsim.util": [
             [11, "module-satsim.util"]
         ],
         "satsim.util.system": [
             [11, "module-satsim.util.system"]
         ],
         "satsim.util.thread": [
```

### Comparing `satsim-0.14.0/docs/_build/html/usage.html` & `satsim-0.15.0/docs/_build/html/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Usage &mdash; SatSim 0.14.0 documentation</title>
+  <title>Usage &mdash; SatSim 0.15.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.14.0
+                0.15.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.14.0
+0.15.0
 [q                   ]
 Contents:
     * Installation
     * Usage
           o Python_Module
           o Command_Line_Interface
           o Parameters_and_Configuration
```

### Comparing `satsim-0.14.0/docs/api/satsim.generator.obs.rst` & `satsim-0.15.0/docs/api/satsim.generator.obs.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.geometry.rst` & `satsim-0.15.0/docs/api/satsim.geometry.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.image.rst` & `satsim-0.15.0/docs/api/satsim.image.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.io.rst` & `satsim-0.15.0/docs/api/satsim.io.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.math.rst` & `satsim-0.15.0/docs/api/satsim.math.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.rst` & `satsim-0.15.0/docs/api/satsim.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.util.rst` & `satsim-0.15.0/docs/api/satsim.util.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/api/satsim.vecmath.rst` & `satsim-0.15.0/docs/api/satsim.vecmath.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/conf.py` & `satsim-0.15.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 author = u"Alex Cabello"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '0.14.0'
+version = '0.15.0'
 # The full version, including alpha/beta/rc tags.
-release = '0.14.0'
+release = '0.15.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `satsim-0.14.0/docs/installation.rst` & `satsim-0.15.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/make.bat` & `satsim-0.15.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/docs/usage.rst` & `satsim-0.15.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/cli.py` & `satsim-0.15.0/satsim/cli.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/config.py` & `satsim-0.15.0/satsim/config.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/dataset/augment.py` & `satsim-0.15.0/satsim/dataset/augment.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         x_fov = ssp['fpa']['x_fov']
         box_pad = box_pad / w
 
         sspc = transform(copy.deepcopy(ssp), '.')
         sspc['augment']['image']['post'] = tf.squeeze(image)
 
         ig = image_generator(sspc, with_meta=True)
-        fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, num_shot_noise_samples, obs_cache = ig.__next__()
+        fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, num_shot_noise_samples, obs_cache, ground_truth = ig.__next__()
 
         anno = init_annotation('.', 0, h, w, y_fov, x_fov)
         snr = signal_to_noise_ratio(fpa_conv_targ, tf.squeeze(image) * a2d_gain, rn)
         set_frame_annotation(anno, ['null'], h * s_osf, w * s_osf, obs_os_pix, snr=snr)
 
         unbboxs = tf.unstack(bboxs)
         for ii in range(len(unbboxs)):
```

### Comparing `satsim-0.14.0/satsim/generator/obs/breakup.py` & `satsim-0.15.0/satsim/generator/obs/breakup.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/generator/obs/cso.py` & `satsim-0.15.0/satsim/generator/obs/cso.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/generator/obs/geometry.py` & `satsim-0.15.0/satsim/generator/obs/geometry.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/generator/obs/io.py` & `satsim-0.15.0/satsim/generator/obs/io.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/generator/obs/rpo.py` & `satsim-0.15.0/satsim/generator/obs/rpo.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/astrometric.py` & `satsim-0.15.0/satsim/geometry/astrometric.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/csvsc.py` & `satsim-0.15.0/satsim/geometry/csvsc.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/draw.py` & `satsim-0.15.0/satsim/geometry/draw.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/ephemeris.py` & `satsim-0.15.0/satsim/geometry/ephemeris.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/random.py` & `satsim-0.15.0/satsim/geometry/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/sgp4.py` & `satsim-0.15.0/satsim/geometry/sgp4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/sprite.py` & `satsim-0.15.0/satsim/geometry/sprite.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/sstr7.py` & `satsim-0.15.0/satsim/geometry/sstr7.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/transform.py` & `satsim-0.15.0/satsim/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/twobody.py` & `satsim-0.15.0/satsim/geometry/twobody.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/geometry/wcs.py` & `satsim-0.15.0/satsim/geometry/wcs.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/image/augment.py` & `satsim-0.15.0/satsim/image/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/image/fpa.py` & `satsim-0.15.0/satsim/image/fpa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import division, print_function, absolute_import
 
 import tensorflow as tf
 import numpy as np
 
 from satsim.geometry.transform import rotate_and_translate
-from satsim.util import get_semantic_version
+from satsim.util import get_semantic_version, is_tensorflow_running_on_cpu
 from satsim.math import fftconv2p
 
 
 MAX_PIXEL_VALUE = {
     'int8': 127.0,
     'uint8': 255.0,
     'int16': 32767.0,
@@ -249,27 +249,26 @@
             image pad.
         c_offset: `int`, offset to add to `c` values. Useful to account for
             image pad.
 
     Returns:
         A `Tensor`, a reference to the modified input `fpa` image
     """
-    r = tf.cast(r, tf.int32)
-    c = tf.cast(c, tf.int32)
+    r = tf.cast(r, tf.int32) + tf.cast(r_offset, tf.int32)
+    c = tf.cast(c, tf.int32) + tf.cast(c_offset, tf.int32)
 
-    # TODO no bounds checking in TF-GPU if fpa is int32 type
-    # h,w = fpa.get_shape().as_list()
-    # valid = (r >= 0) & (r < h) & (c >= 0) & (c < w)
-    # r = tf.boolean_mask(r, valid)
-    # c = tf.boolean_mask(c, valid)
-    # cnt = tf.boolean_mask(tf.convert_to_tensor(cnt, dtype=fpa.dtype), valid)
-
-    # r_offset = r_offset
-    # c_offset = c_offset
-    rc = tf.stack([r + r_offset, c + c_offset], axis=1)
+    # fix for no bounds checking if fpa is int32 or if running CPU
+    if is_tensorflow_running_on_cpu() or fpa.dtype == 'int32':
+        h, w = fpa.get_shape().as_list()
+        valid = (r >= 0) & (r < h) & (c >= 0) & (c < w)
+        r = tf.boolean_mask(r, valid)
+        c = tf.boolean_mask(c, valid)
+        cnt = tf.boolean_mask(tf.convert_to_tensor(cnt, dtype=fpa.dtype), valid)
+
+    rc = tf.stack([r, c], axis=1)
     return tf.compat.v1.tensor_scatter_nd_add(fpa, rc, cnt)
 
 
 def transform_and_fft(fpa, r, c, cnt, t_start, t_end, t_osf, rotation, translation):
     """Applies discrete rotation and translation transformations to the center
     point and applies the smear to all other points with an FFT. This has the
     effect of  "smearing" or "streaking" the point between times `t_start` and
```

### Comparing `satsim-0.14.0/satsim/image/model.py` & `satsim-0.15.0/satsim/image/model.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/image/noise.py` & `satsim-0.15.0/satsim/image/noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,12 +53,13 @@
     Args:
         fpa: `Tensor`, input image as a 2D tensor in real pixels (not oversampled).
         rn: `float`, electrons RMS value of the read noise.
         en: `float`, electrons RMS value of the electronic noise.
 
     Returns:
         A `Tensor`, the 2D tensor with read noise applied.
+        A `Tensor`, the 2D tensor read noise.
     """
     rn = tf.cast(rn, tf.float32)
     en = tf.cast(rn, tf.float32)
     noise = tf.random.normal(tf.shape(fpa)) * tf.math.sqrt(rn * rn + en * en)
-    return fpa + noise
+    return fpa + noise, noise
```

### Comparing `satsim-0.14.0/satsim/image/psf.py` & `satsim-0.15.0/satsim/image/psf.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/image/render.py` & `satsim-0.15.0/satsim/image/render.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/io/czml.py` & `satsim-0.15.0/satsim/io/czml.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,28 +67,34 @@
     if 'site' in ssp['geometry']:
         site = ssp['geometry']['site']
         latitude = _ltude(site['lat'], 'latitude', 'N', 'S') * u.deg
         longitude = _ltude(site['lon'], 'longitude', 'E', 'W') * u.deg
         alt = site['alt'] * u.m
 
         name = site['name'] if 'name' in site else None
-        label_show = False
 
-        if 'czml' in site:
-            label_show = site['czml'].get('path_show', label_show)
+        # czml
+        czml_config = site['czml'] if 'czml' in site else {}
+        label_show = czml_config.get('label_show', False)
+        cone_show = czml_config.get('cone_show', True)
+        cone_color = czml_config.get('cone_color', [255, 255, 0, 64])
+        billboard_show = czml_config.get('billboard_show', True)
+        billboard_image = czml_config.get('billboard_image', PIC_GROUNDSTATION)
 
         sensor = {
             'y_fov': astrometrics[0]['y_fov'],
             'x_fov': astrometrics[0]['x_fov'],
             'time': [x['time'] for x in astrometrics],
             'quat': [list(_equatorial_to_ecr_quaternion(x['ra'], x['dec'], 0.0, x['time'])) for x in astrometrics],
             'range': [x['range'] for x in astrometrics],
         }
 
-        extractor.add_ground_station([latitude, longitude, alt], sensor, label_text=name, label_show=label_show)
+        extractor.add_ground_station([latitude, longitude, alt], sensor, label_text=name, label_show=label_show,
+                                     cone_show=cone_show, cone_color=cone_color, billboard_show=billboard_show,
+                                     billboard_image=billboard_image)
 
     # extract objects data
     for i, o in enumerate(ssp['geometry']['obs']['list']):
 
         ts_start_ob = t0
         ts_end_ob = t2
         if 'events' in o:
@@ -98,35 +104,32 @@
                 ts_end_ob = time.utc_from_list_or_scalar(o['events']['delete'], default_t=tt)
 
         if obs_cache[i] is not None:
             sat = obs_cache[i][0]
 
             name = o['name'] if 'name' in o else None
 
-            path_show = (ts_start_ob == t0)
-            path_color = [255, 255, 0]
-            billboard_show = True
             start_interval = time.to_astropy(t0)
             end_interval = time.to_astropy(t2)
-            label_show = False
 
-            if 'czml' in o:
-                label_show = o['czml'].get('label_show', label_show)
-                path_show = o['czml'].get('path_show', path_show)
-                path_color = o['czml'].get('path_color', path_color)
-                billboard_show = o['czml'].get('billboard_show', billboard_show)
-                if 'start_interval' in o['czml']:
-                    start_interval = time.to_astropy(time.utc_from_list_or_scalar(o['czml']['start_interval']))
-                if 'end_interval' in o['czml']:
-                    end_interval = time.to_astropy(time.utc_from_list_or_scalar(o['czml']['end_interval']))
+            # czml
+            czml_config = o['czml'] if 'czml' in o else {}
+            label_show = czml_config.get('label_show', False)
+            path_show = czml_config.get('path_show', (ts_start_ob == t0))
+            path_color = czml_config.get('path_color', [255, 255, 0])
+            billboard_show = czml_config.get('billboard_show', True)
+            billboard_image = czml_config.get('billboard_image', PIC_SATELLITE)
 
-            extractor.add_object(sat, N=N, label_text=name, label_show=label_show,
-                                 start_interval=start_interval, end_interval=end_interval,
+            start_interval = time.to_astropy(time.utc_from_list_or_scalar(o['czml']['start_interval'])) if 'start_interval' in czml_config else time.to_astropy(t0)
+            end_interval = time.to_astropy(time.utc_from_list_or_scalar(o['czml']['end_interval'])) if 'end_interval' in czml_config else time.to_astropy(t2)
+
+            extractor.add_object(sat, N=N, label_text=name, start_interval=start_interval, end_interval=end_interval,
                                  start_available=time.to_astropy(ts_start_ob), end_available=time.to_astropy(ts_end_ob),
-                                 path_show=path_show, id_name=name, billboard_show=billboard_show, path_color=path_color)
+                                 label_show=label_show, path_show=path_show, path_color=path_color, billboard_show=billboard_show,
+                                 billboard_image=billboard_image)
 
     # convert document to json
     j = extractor.get_document().dumps()
     if filename is not None:
         with open(filename, "w") as outfile:
             outfile.write(j)
 
@@ -204,15 +207,19 @@
         sensor,
         id_name=None,
         id_description=None,
         label_fill_color=[255, 255, 0, 255],
         label_outline_color=[255, 255, 0, 255],
         label_font="16pt Lucida Console",
         label_text=None,
-        label_show=False
+        label_show=False,
+        billboard_show=True,
+        billboard_image=PIC_GROUNDSTATION,
+        cone_color=[255, 255, 0, 64],
+        cone_show=True,
     ):
         """
         Adds a ground station
 
         Args:
             pos: `list [~astropy.units]`, coordinates of ground station (i.e. latitude, longitude, altitude)
             id_description: `str`, Set ground station description
@@ -231,15 +238,15 @@
             name=id_name,
             description=id_description,
             availability=TimeInterval(start=self.start_epoch, end=self.end_epoch),
             position=Position(cartesian=pos),
             label=Label(
                 show=True,
             ),
-            billboard=Billboard(image=PIC_GROUNDSTATION, show=True),
+            billboard=Billboard(image=billboard_image, show=True),
         )
 
         self.packets.append(pckt)
         self.num_gs += 1
 
         N = len(sensor['quat'])
         quat = []
@@ -259,21 +266,21 @@
                 interpolationDegree=1,
                 interpolationAlgorithm=InterpolationAlgorithms.LINEAR,
                 epoch=self.start_epoch.datetime.replace(tzinfo=timezone.utc),
                 forwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE,
                 backwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE
             ),
             agi_rectangularSensor=RectangularSensor(
-                show=True,
+                show=cone_show,
                 showIntersection=False,
                 intersectionColor=Color(rgba=[255, 255, 255, 255]),
                 intersectionWidth=2,
                 portionToDisplay="COMPLETE",
-                lateralSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=[255, 255, 0, 128]))),
-                domeSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=[255, 255, 0, 128]))),
+                lateralSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=cone_color))),
+                domeSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=cone_color))),
                 xHalfAngle=np.radians(sensor['x_fov'] / 2),
                 yHalfAngle=np.radians(sensor['y_fov'] / 2),
                 radius=Double(
                     number=radius,
                     interpolationDegree=1,
                     interpolationAlgorithm=InterpolationAlgorithms.LINEAR,
                     epoch=self.start_epoch.datetime.replace(tzinfo=timezone.utc),
@@ -298,15 +305,16 @@
         label_font="16pt Lucida Console",
         label_text=None,
         label_show=False,
         start_interval=None,
         end_interval=None,
         start_available=None,
         end_available=None,
-        billboard_show=True
+        billboard_show=True,
+        billboard_image=PIC_SATELLITE,
     ):
         """
         Adds a SatSim Skyfield object
 
         Args:
             sat: `object`, SatSim Skyfield object
             N: `int`, Number of sample points
@@ -368,15 +376,15 @@
             label=Label(
                 text=label_text,
                 font=label_font,
                 show=label_show,
                 fillColor=Color(rgba=label_fill_color),
                 outlineColor=Color(rgba=label_outline_color),
             ),
-            billboard=Billboard(image=PIC_SATELLITE, show=billboard_show),
+            billboard=Billboard(image=billboard_image, show=billboard_show),
         )
 
         self.packets.append(pckt)
 
         self.num_objects += 1
 
     def get_document(self):
```

### Comparing `satsim-0.14.0/satsim/io/fits.py` & `satsim-0.15.0/satsim/io/fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def save(filename, fpa, exposure_time=0, dt_start=datetime.now(), header={}, overwrite=False, dtype='uint16', astrometrics=None):
     """Save a SatNet compatible FITS file.
 
     Args:
         filename: `string`, the FITS filename.
         fpa: `np.array`, input image as a 2D numpy array.
         exposure_time: `float`, exposure time for header.
-        dt_start: `datatime`, datetime of start of exposure.
+        dt_start: `datetime`, datetime of start of exposure.
         header: `dict`, placeholder, not implemented
         overwrite: `boolean`, if True overwrite file if it exists
         dtype: `string`, 'int16', 'uint16', 'int32', 'uint32', or 'float32'. default: 'int16'
     """
     
     ver = 'SATSIM {}'.format(__version__)
```

### Comparing `satsim-0.14.0/satsim/io/image.py` & `satsim-0.15.0/satsim/io/image.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/io/satnet.py` & `satsim-0.15.0/satsim/io/satnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import json
 from pathlib import Path
 from collections import OrderedDict
 
 import numpy as np
+import tifffile
 
 from satsim.io import fits, image
 from satsim.config import save_json
 
 
 def init_annotation(dirname, sequence, height, width, y_ifov, x_ifov):
     """Init annotation object for SatNet.
@@ -152,28 +153,31 @@
             'pixels': opix,
             'snr': osnr,
         }))
 
     return data
 
 
-def write_frame(dir_name, sat_name, fpa_digital, meta_data, frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True, astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True):
+def write_frame(dir_name, sat_name, fpa_digital, meta_data, frame_num, exposure_time, time_stamp, ssp, show_obs_boxes=True, astrometrics=None, save_pickle=False, dtype='uint16', save_jpeg=True, ground_truth=None, ground_truth_min=0):
     """Write image and annotation files compatible with SatNet. In addition,
     writes annotated images and SatSim configuration file for reference.
 
     Args:
         dir_name: `string`, directory to save files to
         sat_name: `string`, satellite name
         fpa_digital: `array`, image as a numpy array
         meta_data: `dict`, annotation data generated by `init_annotation`
         frame_num: `int`, current frame number in set
         exposure_time: `float`, current frame exposure time in seconds
         time_stamp: `datetime`, reference time
         ssp: `dict`: SatSim parameters to be saved to JSON file
         dtype: `string`: Data type to save FITS pixel data as
+        save_jpeg: `boolean`: specify to save a JPEG annotated image
+        ground_truth: `OrderedDict`: an ordered dictionary of arrays or numbers
+        ground_truth_min: `float`, set any value less than this number in ground_truth to 0
     """
 
     file_name = '{}.{:04d}'.format(sat_name, frame_num)
 
     meta_data['data']['file']['dirname'] = Path(dir_name).name
     meta_data['data']['file']['filename'] = '{}.fits'.format(file_name)
 
@@ -197,7 +201,24 @@
 
     # save annotated images
     if save_jpeg:
         image.save(os.path.join(annotatedimg_dir, '{}.jpg'.format(file_name)), fpa_digital, vauto=True, annotation=meta_data['data']['objects'], show_obs_boxes=show_obs_boxes)
 
     # save sim config
     save_json(os.path.join(dir_name,'config.json'), ssp, save_pickle=save_pickle)
+
+    # save ground truth
+    if ground_truth is not None:
+
+        keys = ','.join(ground_truth.keys())
+
+        # broadcast scalars
+        def f(x):
+            return x if x.shape == fpa_digital.shape else np.resize(x, fpa_digital.shape)
+
+        ground_truth = np.stack(list(map(f, ground_truth.values())))
+
+        # clip values
+        ground_truth[ground_truth < ground_truth_min] = 0
+
+        tifffile.imwrite(os.path.join(annotation_dir, '{}.tiff'.format(file_name)), np.stack(ground_truth), dtype='float32', bigtiff=True, compression='lzw',
+                         metadata={'ImageDescription': keys})
```

### Comparing `satsim-0.14.0/satsim/math/angle.py` & `satsim-0.15.0/satsim/math/angle.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/const.py` & `satsim-0.15.0/satsim/math/const.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/conv.py` & `satsim-0.15.0/satsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/fft.py` & `satsim-0.15.0/satsim/math/fft.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/interpolate.py` & `satsim-0.15.0/satsim/math/interpolate.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/random.py` & `satsim-0.15.0/satsim/math/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/math/stats.py` & `satsim-0.15.0/satsim/math/stats.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/pipeline/__init__.py` & `satsim-0.15.0/satsim/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/satsim.py` & `satsim-0.15.0/satsim/satsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import copy
 from datetime import datetime
 import pickle
 import json
 import math
 from time import sleep
+from collections import OrderedDict
 
 import pydash
 import tensorflow as tf
 import numpy as np
 from astropy import units as u
 
 from satsim.math import signal_to_noise_ratio, mean_degrees, diff_degrees, interp_degrees
@@ -149,15 +150,15 @@
         ['{}.{:04d}.json'.format(set_name,x) for x in range(num_frames)],
         ssp['fpa']['height'],
         ssp['fpa']['width'],
         y_ifov,
         x_ifov)
 
     astrometrics_list = []
-    for fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, num_shot_noise_samples, obs_cache in image_generator(ssp, output_dir, output_debug, dir_debug, with_meta=True, num_sets=1):
+    for fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, num_shot_noise_samples, obs_cache, ground_truth in image_generator(ssp, output_dir, output_debug, dir_debug, with_meta=True, num_sets=1):
         astrometrics_list.append(astrometrics)
         if fpa_digital is not None:
             snr = signal_to_noise_ratio(fpa_conv_targ, fpa_conv_star + bg_tf + dc_tf, rn_tf)
             if num_shot_noise_samples is not None:
                 snr = snr * np.sqrt(num_shot_noise_samples)
             meta_data = set_frame_annotation(meta_data, frame_num, h_fpa_os, w_fpa_os, obs_os_pix, [20 * s_osf, 20 * s_osf], snr=snr)
             if queue is not None:
@@ -171,14 +172,15 @@
                     'time_stamp': dt,
                     'ssp': ssp_orig,
                     'show_obs_boxes': ssp['sim']['show_obs_boxes'],
                     'astrometrics': astrometrics,
                     'save_pickle': ssp['sim']['save_pickle'],
                     'dtype': a2d_dtype,
                     'save_jpeg': ssp['sim']['save_jpeg'],
+                    'ground_truth': ground_truth,
                 }, tag=dir_name)
             if output_debug:
                 with open(os.path.join(dir_debug, 'metadata_{}.json'.format(frame_num)), 'w') as jsonfile:
                     json.dump(meta_data, jsonfile, indent=2)
 
             logger.debug('Finished frame {} of {} in {} sec.'.format(frame_num + 1, num_frames, toc('gen_frame', frame_num)))
         else:
@@ -374,14 +376,17 @@
 
     if 'save_movie' not in ssp['sim']:
         ssp['sim']['save_movie'] = ssp['sim']['save_jpeg']
 
     if 'save_czml' not in ssp['sim']:
         ssp['sim']['save_czml'] = True
 
+    if 'save_ground_truth' not in ssp['sim']:
+        ssp['sim']['save_ground_truth'] = False
+
     if 'mode' not in ssp['sim']:
         ssp['sim']['mode'] = 'fftconv2p'
 
     if 'save_pickle' not in ssp['sim']:
         ssp['sim']['save_pickle'] = False
 
     if star_mode == 'bins':
@@ -756,15 +761,15 @@
 
                 # if image rendering is disabled, then propagate objects and return
                 if ssp['sim']['mode'] == 'none':
                     r_obs_os, c_obs_os, pe_obs_os, obs_os_pix, obs_model = gen_objects(obs, t_start, t_end)
                     if track_mode is not None:
                         star_ra, star_dec, star_tran_os, star_rot_rate = calculate_star_position_and_motion(ts_start, ts_end, star_rot, track_mode)
                     if with_meta:
-                        yield None, frame_num, astrometrics.copy(), None, None, None, None, None, None, None, obs_cache
+                        yield None, frame_num, astrometrics.copy(), None, None, None, None, None, None, None, obs_cache, None
                     else:
                         yield None
                     continue
 
                 # refresh catalog stars
                 # TODO should save stars and transform to FPA again on every frame
                 if (star_mode == 'sstr7' or star_mode == 'csv') and (ssp['sim']['star_catalog_query_mode'] == 'frame' or frame_num == 0):
@@ -814,28 +819,41 @@
 
                 # add noise
                 fpa_conv = (fpa_conv_star + fpa_conv_targ + bg_tf) * gain_tf + dc_tf
                 if ssp['sim']['enable_shot_noise'] is True:
                     fpa_conv_noise = add_photon_noise(fpa_conv, ssp['sim']['num_shot_noise_samples'])
                 else:
                     fpa_conv_noise = fpa_conv
-                fpa = add_read_noise(fpa_conv_noise, rn, en)
+                fpa, rn_gt = add_read_noise(fpa_conv_noise, rn, en)
 
                 # analog to digital
                 fpa_digital = analog_to_digital(fpa + bias_tf, a2d_gain, a2d_fwc, a2d_bias, dtype=a2d_dtype)
 
                 # augment TODO abstract this
                 if pydash.objects.has(ssp, 'augment.image'):
                     if ssp['augment']['image']['post'] is None:
                         pass
                     elif callable(ssp['augment']['image']['post']):
                         fpa_digital = ssp['augment']['image']['post'](fpa_digital)
                     else:
                         fpa_digital = fpa_digital + ssp['augment']['image']['post']
 
+                if ssp['sim']['save_ground_truth']:
+                    ground_truth = OrderedDict()
+                    ground_truth['target_pe'] = fpa_conv_targ.numpy()
+                    ground_truth['star_pe'] = fpa_conv_star.numpy()
+                    ground_truth['background_pe'] = bg_tf.numpy()
+                    ground_truth['dark_current_pe'] = dc_tf.numpy()
+                    ground_truth['photon_noise_pe'] = (fpa_conv_noise - fpa_conv).numpy()
+                    ground_truth['read_noise_pe'] = rn_gt.numpy()
+                    ground_truth['gain'] = gain_tf.numpy()
+                    ground_truth['bias_pe'] = bias_tf.numpy()
+                else:
+                    ground_truth = None
+
                 if output_debug:
                     if fpa_os_w_targets is not None:
                         with open(os.path.join(dir_debug, 'fpa_os_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                             pickle.dump(fpa_os_w_targets.numpy(), picklefile)
                     if fpa_conv_os is not None:
                         with open(os.path.join(dir_debug, 'fpa_conv_os_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                             pickle.dump(fpa_conv_os.numpy(), picklefile)
@@ -854,10 +872,10 @@
                         pickle.dump(fpa.numpy(), picklefile)
                     with open(os.path.join(dir_debug, 'fpa_digital_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                         pickle.dump(fpa_digital.numpy(), picklefile)
                     with open(os.path.join(dir_debug, 'stars_os_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                         pickle.dump([r_stars_os.numpy(), c_stars_os.numpy(), pe_stars_os.numpy(), t_start_star, t_end_star, t_osf, star_rot_rate, star_tran_os], picklefile)
 
                 if with_meta:
-                    yield fpa_digital, frame_num, astrometrics.copy(), obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, ssp['sim']['num_shot_noise_samples'], obs_cache
+                    yield fpa_digital, frame_num, astrometrics.copy(), obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, ssp['sim']['num_shot_noise_samples'], obs_cache, ground_truth
                 else:
                     yield fpa_digital
```

### Comparing `satsim-0.14.0/satsim/time/__init__.py` & `satsim-0.15.0/satsim/time/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/util/system.py` & `satsim-0.15.0/satsim/util/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import division, print_function, absolute_import
 
 import re
 import tensorflow as tf
 import logging
 
 logger = logging.getLogger(__name__)
+IS_CPU = len(tf.config.list_physical_devices('GPU')) == 0
 
 
 def get_semantic_version(module):
     """Gets the sematic version from a module as an array of integers. Non digit characters
     will be removed.
 
     Example::
@@ -61,14 +62,17 @@
     Returns:
         gpus: `string`, a list of logical gpu names
     """
     gpus = tf.config.experimental.list_physical_devices('GPU')
 
     logger.debug('Visible gpus: {}'.format(gpus))
 
+    if len(gpus) == 0:
+        return gpus
+
     tf.config.experimental.set_visible_devices([gpus[i] for i in gpu_ids], 'GPU')
 
     logger.debug('Configuring GPU device {} with {} MB'.format(gpu_ids, memory))
 
     if memory is not None:
         for gpu_id in gpu_ids:
             tf.config.experimental.set_virtual_device_configuration(
@@ -77,7 +81,12 @@
             )
 
     gpus = tf.config.experimental.list_logical_devices('GPU')
 
     logger.debug('Logical gpus: {}'.format(gpus))
 
     return gpus
+
+
+def is_tensorflow_running_on_cpu():
+    """Returns True if TensorFlow is running on the CPU. """
+    return IS_CPU
```

### Comparing `satsim-0.14.0/satsim/util/thread.py` & `satsim-0.15.0/satsim/util/thread.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/util/timer.py` & `satsim-0.15.0/satsim/util/timer.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Cartesian2.py` & `satsim-0.15.0/satsim/vecmath/Cartesian2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Cartesian3.py` & `satsim-0.15.0/satsim/vecmath/Cartesian3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Cartesian4.py` & `satsim-0.15.0/satsim/vecmath/Cartesian4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Matrix2.py` & `satsim-0.15.0/satsim/vecmath/Matrix2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Matrix3.py` & `satsim-0.15.0/satsim/vecmath/Matrix3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Matrix4.py` & `satsim-0.15.0/satsim/vecmath/Matrix4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim/vecmath/Quaternion.py` & `satsim-0.15.0/satsim/vecmath/Quaternion.py`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/satsim.egg-info/PKG-INFO` & `satsim-0.15.0/satsim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.14.0
+Version: 0.15.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,20 +37,28 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.15.0
+---------------------
+
+* Add support to save ground truth image data to the Annotations directory. Set sim option `save_ground_truth` to `true`.
+* Add support for running on CPU with no GPU acceleration.
+* Add CZML options for sensor visualization and object billboard image.
+
+
 0.14.0
 ---------------------
 
-Add vector math library.
-Add CZML output for sensor visualization.
-Fix objects not updating properly when image renderer is off.
+* Add vector math library.
+* Add CZML output for sensor visualization.
+* Fix objects not updating properly when image renderer is off.
 
 
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
```

### Comparing `satsim-0.14.0/satsim.egg-info/SOURCES.txt` & `satsim-0.15.0/satsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satsim-0.14.0/setup.cfg` & `satsim-0.15.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.14.0
+current_version = 0.15.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `satsim-0.14.0/setup.py` & `satsim-0.15.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,10 +63,10 @@
     keywords='satsim',
     name='satsim',
     packages=find_packages(include=['satsim', 'satsim.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ssc-ai/satsim',
-    version='0.14.0',
+    version='0.15.0',
     zip_safe=False,
 )
```

