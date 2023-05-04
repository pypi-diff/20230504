# Comparing `tmp/docutils-0.9.tar.gz` & `tmp/docutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docutils-0.9.tar", last modified: Wed May  2 18:31:33 2012, max compression, from Unix
+gzip compressed data, was "docutils-0.9.1.tar", last modified: Sun Jun 17 22:07:23 2012, max compression, from Unix
```

## Comparing `docutils-0.9.tar` & `docutils-0.9.1.tar`

### file list

```diff
@@ -1,628 +1,628 @@
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:29.000000 docutils-0.9/docs/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:29.000000 docutils-0.9/docs/api/
--rw-r--r--   0 bert      (1001) bert      (1001)     2327 2012-01-03 19:23:53.000000 docutils-0.9/docs/api/cmdline-tool.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    10584 2012-01-03 19:23:53.000000 docutils-0.9/docs/api/publisher.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     8186 2012-01-03 19:23:53.000000 docutils-0.9/docs/api/runtime-settings.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/dev/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/dev/rst/
--rw-r--r--   0 bert      (1001) bert      (1001)   113248 2012-03-19 17:04:49.000000 docutils-0.9/docs/dev/rst/alternatives.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    35546 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/rst/problems.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4048 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/distributing.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    17005 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/enthought-plan.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4522 2005-10-30 14:23:25.000000 docutils-0.9/docs/dev/enthought-rfp.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     9218 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/hacking.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    24730 2012-03-10 22:46:07.000000 docutils-0.9/docs/dev/policies.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7385 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/pysource.dtd
--rw-r--r--   0 bert      (1001) bert      (1001)     4433 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/pysource.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     5368 2012-05-02 07:22:20.000000 docutils-0.9/docs/dev/release.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6161 2012-01-26 09:57:04.000000 docutils-0.9/docs/dev/repository.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4564 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/semantics.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7960 2011-12-02 00:43:32.000000 docutils-0.9/docs/dev/testing.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    93495 2012-02-27 11:15:38.000000 docutils-0.9/docs/dev/todo.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3316 2012-01-03 19:23:53.000000 docutils-0.9/docs/dev/website.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/howto/
--rw-r--r--   0 bert      (1001) bert      (1001)     3340 2012-01-03 19:23:53.000000 docutils-0.9/docs/howto/html-stylesheets.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7451 2012-01-03 19:23:53.000000 docutils-0.9/docs/howto/i18n.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    16395 2012-01-03 19:23:53.000000 docutils-0.9/docs/howto/rst-directives.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     8683 2012-01-03 19:23:53.000000 docutils-0.9/docs/howto/rst-roles.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     5831 2012-01-03 19:23:53.000000 docutils-0.9/docs/howto/security.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/peps/
--rw-r--r--   0 bert      (1001) bert      (1001)    10405 2006-05-21 20:44:42.000000 docutils-0.9/docs/peps/pep-0256.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    11738 2006-05-21 20:44:42.000000 docutils-0.9/docs/peps/pep-0257.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    36245 2009-10-05 19:08:10.000000 docutils-0.9/docs/peps/pep-0258.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    32597 2006-05-21 20:44:42.000000 docutils-0.9/docs/peps/pep-0287.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/ref/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/ref/rst/
--rw-r--r--   0 bert      (1001) bert      (1001)     7669 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/rst/definitions.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    59068 2012-01-06 11:11:51.000000 docutils-0.9/docs/ref/rst/directives.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    14090 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/rst/introduction.txt
--rw-r--r--   0 bert      (1001) bert      (1001)   106881 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/rst/restructuredtext.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    10218 2012-01-06 11:11:51.000000 docutils-0.9/docs/ref/rst/roles.txt
--rw-r--r--   0 bert      (1001) bert      (1001)   117426 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/doctree.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    16728 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/docutils.dtd
--rw-r--r--   0 bert      (1001) bert      (1001)    12744 2002-04-20 03:01:52.000000 docutils-0.9/docs/ref/soextblx.dtd
--rw-r--r--   0 bert      (1001) bert      (1001)     3780 2012-01-03 19:23:53.000000 docutils-0.9/docs/ref/transforms.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/user/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/user/images/
--rw-r--r--   0 bert      (1001) bert      (1001)    19823 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/big-black.png
--rw-r--r--   0 bert      (1001) bert      (1001)    25697 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/big-white.png
--rw-r--r--   0 bert      (1001) bert      (1001)    59358 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/default.png
--rw-r--r--   0 bert      (1001) bert      (1001)     5202 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/happy_monkey.png
--rw-r--r--   0 bert      (1001) bert      (1001)    24021 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/medium-black.png
--rw-r--r--   0 bert      (1001) bert      (1001)    33756 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/medium-white.png
--rw-r--r--   0 bert      (1001) bert      (1001)    32565 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-all.png
--rw-r--r--   0 bert      (1001) bert      (1001)    17754 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-breaks.png
--rw-r--r--   0 bert      (1001) bert      (1001)    19080 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-covers.png
--rw-r--r--   0 bert      (1001) bert      (1001)    20751 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-cuts.png
--rw-r--r--   0 bert      (1001) bert      (1001)     4900 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-empty.png
--rw-r--r--   0 bert      (1001) bert      (1001)    21291 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/rsp-objects.png
--rw-r--r--   0 bert      (1001) bert      (1001)    49418 2005-11-29 01:48:42.000000 docutils-0.9/docs/user/images/rsp.svg
--rw-r--r--   0 bert      (1001) bert      (1001)    25404 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/s5-files.png
--rw-r--r--   0 bert      (1001) bert      (1001)    39029 2005-12-03 02:24:44.000000 docutils-0.9/docs/user/images/s5-files.svg
--rw-r--r--   0 bert      (1001) bert      (1001)    41144 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/small-black.png
--rw-r--r--   0 bert      (1001) bert      (1001)    41120 2005-12-08 04:43:13.000000 docutils-0.9/docs/user/images/small-white.png
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/user/rst/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docs/user/rst/images/
--rw-r--r--   0 bert      (1001) bert      (1001)     4361 2005-07-07 23:47:11.000000 docutils-0.9/docs/user/rst/images/ball1.gif
--rw-r--r--   0 bert      (1001) bert      (1001)     7646 2010-03-02 00:24:53.000000 docutils-0.9/docs/user/rst/images/biohazard-scaling.svg
--rw-r--r--   0 bert      (1001) bert      (1001)      179 2005-07-07 23:47:11.000000 docutils-0.9/docs/user/rst/images/biohazard.png
--rw-r--r--   0 bert      (1001) bert      (1001)     7609 2010-03-02 11:51:33.000000 docutils-0.9/docs/user/rst/images/biohazard.svg
--rw-r--r--   0 bert      (1001) bert      (1001)     1307 2010-03-09 14:42:58.000000 docutils-0.9/docs/user/rst/images/biohazard.swf
--rw-r--r--   0 bert      (1001) bert      (1001)     2609 2010-03-02 00:24:53.000000 docutils-0.9/docs/user/rst/images/title-scaling.svg
--rw-r--r--   0 bert      (1001) bert      (1001)     1155 2009-05-11 14:41:43.000000 docutils-0.9/docs/user/rst/images/title.png
--rw-r--r--   0 bert      (1001) bert      (1001)     2580 2010-03-02 00:24:53.000000 docutils-0.9/docs/user/rst/images/title.svg
--rw-r--r--   0 bert      (1001) bert      (1001)     6982 2011-06-17 10:50:48.000000 docutils-0.9/docs/user/rst/cheatsheet.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    14680 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/rst/demo.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    52658 2009-07-14 14:05:34.000000 docutils-0.9/docs/user/rst/quickref.html
--rw-r--r--   0 bert      (1001) bert      (1001)    11275 2008-12-07 14:15:30.000000 docutils-0.9/docs/user/rst/quickstart.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      224 2006-01-05 12:56:20.000000 docutils-0.9/docs/user/Makefile.docutils-update
--rw-r--r--   0 bert      (1001) bert      (1001)    48092 2012-02-26 19:13:26.000000 docutils-0.9/docs/user/config.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    21537 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/docutils-05-compat.sty.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    22304 2010-06-17 20:16:08.000000 docutils-0.9/docs/user/emacs.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    57844 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/latex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    12652 2012-02-13 16:55:05.000000 docutils-0.9/docs/user/links.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     5488 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/mailing-lists.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     5113 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/manpage.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    37993 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/odt.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    25328 2006-03-30 14:29:59.000000 docutils-0.9/docs/user/slide-shows.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    12451 2012-01-03 19:23:53.000000 docutils-0.9/docs/user/tools.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     8267 2012-01-03 19:23:53.000000 docutils-0.9/docs/index.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/languages/
--rw-r--r--   0 bert      (1001) bert      (1001)     1332 2011-09-16 19:24:51.000000 docutils-0.9/docutils/languages/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1824 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/af.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1940 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/ca.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1928 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/cs.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1722 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/de.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1848 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/en.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1948 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/eo.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1962 2006-05-25 20:48:37.000000 docutils-0.9/docutils/languages/es.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2026 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/fi.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1893 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/fr.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2040 2008-09-05 15:07:51.000000 docutils-0.9/docutils/languages/gl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2683 2006-12-26 09:59:41.000000 docutils-0.9/docutils/languages/he.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1808 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/it.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1942 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/ja.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3856 2010-10-29 22:07:34.000000 docutils-0.9/docutils/languages/lt.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1865 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/nl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1900 2008-08-25 13:07:53.000000 docutils-0.9/docutils/languages/pl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1982 2008-06-03 01:11:03.000000 docutils-0.9/docutils/languages/pt_br.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2155 2011-09-16 18:36:18.000000 docutils-0.9/docutils/languages/ru.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1860 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/sk.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2072 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/sv.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2026 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/zh_cn.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2771 2006-05-21 20:44:42.000000 docutils-0.9/docutils/languages/zh_tw.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/math/
--rw-r--r--   0 bert      (1001) bert      (1001)     1683 2011-11-08 17:42:40.000000 docutils-0.9/docutils/math/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)    17206 2011-11-08 17:42:40.000000 docutils-0.9/docutils/math/latex2mathml.py
--rw-r--r--   0 bert      (1001) bert      (1001)   174390 2011-07-07 19:01:56.000000 docutils-0.9/docutils/math/math2html.py
--rw-r--r--   0 bert      (1001) bert      (1001)    35108 2011-11-08 17:42:40.000000 docutils-0.9/docutils/math/tex2unichar.py
--rw-r--r--   0 bert      (1001) bert      (1001)    17590 2011-11-08 17:42:40.000000 docutils-0.9/docutils/math/unichar2tex.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/parsers/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/parsers/rst/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/parsers/rst/directives/
--rw-r--r--   0 bert      (1001) bert      (1001)    13382 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/directives/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2273 2011-07-06 15:52:30.000000 docutils-0.9/docutils/parsers/rst/directives/admonitions.py
--rw-r--r--   0 bert      (1001) bert      (1001)     9243 2011-12-20 14:14:21.000000 docutils-0.9/docutils/parsers/rst/directives/body.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3098 2012-01-19 22:33:02.000000 docutils-0.9/docutils/parsers/rst/directives/html.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6769 2011-12-14 23:53:38.000000 docutils-0.9/docutils/parsers/rst/directives/images.py
--rw-r--r--   0 bert      (1001) bert      (1001)    21825 2012-01-27 08:41:35.000000 docutils-0.9/docutils/parsers/rst/directives/misc.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4251 2012-01-06 12:08:43.000000 docutils-0.9/docutils/parsers/rst/directives/parts.py
--rw-r--r--   0 bert      (1001) bert      (1001)      831 2011-06-30 22:14:29.000000 docutils-0.9/docutils/parsers/rst/directives/references.py
--rw-r--r--   0 bert      (1001) bert      (1001)    20048 2012-01-27 08:41:35.000000 docutils-0.9/docutils/parsers/rst/directives/tables.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/parsers/rst/include/
--rw-r--r--   0 bert      (1001) bert      (1001)      666 2005-06-12 20:34:06.000000 docutils-0.9/docutils/parsers/rst/include/README.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    10925 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamsa.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7242 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamsb.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1723 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamsc.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6721 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamsn.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3825 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamso.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    11763 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isoamsr.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3101 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isobox.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4241 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isocyr1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1882 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isocyr2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      869 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isodia.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3010 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isogrk1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1705 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isogrk2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     2880 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isogrk3.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3035 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      372 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isogrk4.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4397 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isolat1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     8466 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isolat2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3334 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      519 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomfrk.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1931 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomopf-wide.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      639 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomopf.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3231 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomscr-wide.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      776 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isomscr.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4066 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isonum.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     4613 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isopub.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     9726 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/isotech.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    45428 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/mmlalias.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     9010 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6800 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/mmlextra.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1036 2006-02-26 16:16:59.000000 docutils-0.9/docutils/parsers/rst/include/s5defs.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6112 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1945 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/xhtml1-special.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7028 2005-06-12 16:40:14.000000 docutils-0.9/docutils/parsers/rst/include/xhtml1-symbol.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/parsers/rst/languages/
--rw-r--r--   0 bert      (1001) bert      (1001)      800 2010-09-17 21:38:29.000000 docutils-0.9/docutils/parsers/rst/languages/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3677 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/af.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4467 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/ca.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4857 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/cs.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3465 2011-11-21 16:43:06.000000 docutils-0.9/docutils/parsers/rst/languages/de.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3317 2011-10-15 22:06:45.000000 docutils-0.9/docutils/parsers/rst/languages/en.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3898 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/eo.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4261 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/es.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3661 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/fi.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3709 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/fr.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3711 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/gl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3640 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/he.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3270 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/it.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3863 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/ja.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3583 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/lt.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3708 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/nl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3427 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/pl.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3992 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/pt_br.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3306 2011-09-12 08:28:31.000000 docutils-0.9/docutils/parsers/rst/languages/ru.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3979 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/sk.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4166 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/sv.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4007 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/zh_cn.py
--rw-r--r--   0 bert      (1001) bert      (1001)     5172 2011-09-02 13:00:23.000000 docutils-0.9/docutils/parsers/rst/languages/zh_tw.py
--rw-r--r--   0 bert      (1001) bert      (1001)    14890 2012-01-19 22:33:02.000000 docutils-0.9/docutils/parsers/rst/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)    14712 2012-01-09 15:01:15.000000 docutils-0.9/docutils/parsers/rst/roles.py
--rw-r--r--   0 bert      (1001) bert      (1001)   128822 2012-02-20 21:31:48.000000 docutils-0.9/docutils/parsers/rst/states.py
--rw-r--r--   0 bert      (1001) bert      (1001)    21007 2012-01-19 22:33:02.000000 docutils-0.9/docutils/parsers/rst/tableparser.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1457 2008-07-28 08:37:32.000000 docutils-0.9/docutils/parsers/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)      445 2006-05-21 20:44:42.000000 docutils-0.9/docutils/parsers/null.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/readers/
--rw-r--r--   0 bert      (1001) bert      (1001)     3265 2008-07-28 08:37:32.000000 docutils-0.9/docutils/readers/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1607 2006-05-21 20:44:42.000000 docutils-0.9/docutils/readers/doctree.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1555 2012-01-19 22:33:02.000000 docutils-0.9/docutils/readers/pep.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2340 2006-11-12 18:02:17.000000 docutils-0.9/docutils/readers/standalone.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/transforms/
--rw-r--r--   0 bert      (1001) bert      (1001)     6505 2010-09-28 08:21:25.000000 docutils-0.9/docutils/transforms/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1993 2006-05-21 20:44:42.000000 docutils-0.9/docutils/transforms/components.py
--rw-r--r--   0 bert      (1001) bert      (1001)    18879 2008-07-28 08:37:32.000000 docutils-0.9/docutils/transforms/frontmatter.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4882 2010-04-26 10:04:17.000000 docutils-0.9/docutils/transforms/misc.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6980 2009-08-06 12:21:10.000000 docutils-0.9/docutils/transforms/parts.py
--rw-r--r--   0 bert      (1001) bert      (1001)    11065 2010-09-28 08:21:25.000000 docutils-0.9/docutils/transforms/peps.py
--rw-r--r--   0 bert      (1001) bert      (1001)    36093 2012-01-19 22:33:02.000000 docutils-0.9/docutils/transforms/references.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6577 2009-09-03 07:27:59.000000 docutils-0.9/docutils/transforms/universal.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2609 2012-01-19 22:33:02.000000 docutils-0.9/docutils/transforms/writer_aux.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/utils/
--rw-r--r--   0 bert      (1001) bert      (1001)    26763 2012-02-03 12:22:14.000000 docutils-0.9/docutils/utils/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4871 2011-12-20 14:14:21.000000 docutils-0.9/docutils/utils/code_analyzer.py
--rw-r--r--   0 bert      (1001) bert      (1001)     9473 2012-05-01 09:50:02.000000 docutils-0.9/docutils/utils/punctuation_chars.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2687 2011-12-20 16:39:10.000000 docutils-0.9/docutils/utils/roman.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/html4css1/
--rw-r--r--   0 bert      (1001) bert      (1001)    65633 2012-01-27 08:41:35.000000 docutils-0.9/docutils/writers/html4css1/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6063 2011-06-17 10:50:48.000000 docutils-0.9/docutils/writers/html4css1/html4css1.css
--rw-r--r--   0 bert      (1001) bert      (1001)     4720 2011-06-27 11:38:56.000000 docutils-0.9/docutils/writers/html4css1/math.css
--rw-r--r--   0 bert      (1001) bert      (1001)      114 2006-03-31 03:36:28.000000 docutils-0.9/docutils/writers/html4css1/template.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/latex2e/
--rw-r--r--   0 bert      (1001) bert      (1001)   121530 2012-03-30 11:58:21.000000 docutils-0.9/docutils/writers/latex2e/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)      476 2010-09-20 13:07:30.000000 docutils-0.9/docutils/writers/latex2e/default.tex
--rw-r--r--   0 bert      (1001) bert      (1001)    22419 2011-12-02 00:43:32.000000 docutils-0.9/docutils/writers/latex2e/docutils-05-compat.sty
--rw-r--r--   0 bert      (1001) bert      (1001)      534 2010-09-15 11:09:45.000000 docutils-0.9/docutils/writers/latex2e/titlepage.tex
--rw-r--r--   0 bert      (1001) bert      (1001)      515 2010-10-16 18:49:04.000000 docutils-0.9/docutils/writers/latex2e/xelatex.tex
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/odf_odt/
--rw-r--r--   0 bert      (1001) bert      (1001)   124720 2012-03-20 00:22:38.000000 docutils-0.9/docutils/writers/odf_odt/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4671 2009-01-19 21:02:02.000000 docutils-0.9/docutils/writers/odf_odt/pygmentsformatter.py
--rw-r--r--   0 bert      (1001) bert      (1001)    16500 2011-06-27 05:39:48.000000 docutils-0.9/docutils/writers/odf_odt/styles.odt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/pep_html/
--rw-r--r--   0 bert      (1001) bert      (1001)     3583 2010-05-23 21:20:29.000000 docutils-0.9/docutils/writers/pep_html/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6367 2006-05-21 20:44:42.000000 docutils-0.9/docutils/writers/pep_html/pep.css
--rw-r--r--   0 bert      (1001) bert      (1001)     1294 2006-03-31 03:36:28.000000 docutils-0.9/docutils/writers/pep_html/template.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/big-black/
--rw-r--r--   0 bert      (1001) bert      (1001)       38 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/big-black/__base__
--rw-r--r--   0 bert      (1001) bert      (1001)      911 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/big-black/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     3606 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/big-black/pretty.css
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/big-white/
--rw-r--r--   0 bert      (1001) bert      (1001)      906 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/big-white/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     3566 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/big-white/pretty.css
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/default/
--rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/blank.gif
--rw-r--r--   0 bert      (1001) bert      (1001)     1003 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     1190 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/iepngfix.htc
--rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/opera.css
--rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 02:21:46.000000 docutils-0.9/docutils/writers/s5_html/themes/default/outline.css
--rw-r--r--   0 bert      (1001) bert      (1001)     4384 2005-12-13 00:30:07.000000 docutils-0.9/docutils/writers/s5_html/themes/default/pretty.css
--rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 02:21:46.000000 docutils-0.9/docutils/writers/s5_html/themes/default/print.css
--rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/s5-core.css
--rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/default/slides.css
--rw-r--r--   0 bert      (1001) bert      (1001)    15800 2006-01-05 12:55:51.000000 docutils-0.9/docutils/writers/s5_html/themes/default/slides.js
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-black/
--rw-r--r--   0 bert      (1001) bert      (1001)       41 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-black/__base__
--rw-r--r--   0 bert      (1001) bert      (1001)     4031 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-black/pretty.css
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-white/
--rw-r--r--   0 bert      (1001) bert      (1001)      944 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     3991 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/medium-white/pretty.css
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/small-black/
--rw-r--r--   0 bert      (1001) bert      (1001)       40 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/small-black/__base__
--rw-r--r--   0 bert      (1001) bert      (1001)     4030 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/small-black/pretty.css
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/s5_html/themes/small-white/
--rw-r--r--   0 bert      (1001) bert      (1001)      941 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/small-white/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     4001 2007-04-09 15:15:57.000000 docutils-0.9/docutils/writers/s5_html/themes/small-white/pretty.css
--rw-r--r--   0 bert      (1001) bert      (1001)      301 2005-12-08 04:43:13.000000 docutils-0.9/docutils/writers/s5_html/themes/README.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    14394 2012-01-19 22:33:02.000000 docutils-0.9/docutils/writers/s5_html/__init__.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/docutils/writers/xetex/
--rw-r--r--   0 bert      (1001) bert      (1001)     5079 2012-03-30 11:58:21.000000 docutils-0.9/docutils/writers/xetex/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4283 2012-01-19 11:55:26.000000 docutils-0.9/docutils/writers/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6271 2012-01-18 10:16:20.000000 docutils-0.9/docutils/writers/docutils_xml.py
--rw-r--r--   0 bert      (1001) bert      (1001)    34888 2012-01-20 06:50:44.000000 docutils-0.9/docutils/writers/manpage.py
--rw-r--r--   0 bert      (1001) bert      (1001)      450 2006-05-21 20:44:42.000000 docutils-0.9/docutils/writers/null.py
--rw-r--r--   0 bert      (1001) bert      (1001)      772 2012-01-19 22:33:02.000000 docutils-0.9/docutils/writers/pseudoxml.py
--rw-r--r--   0 bert      (1001) bert      (1001)     7425 2012-05-02 17:06:37.000000 docutils-0.9/docutils/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1183 2012-01-19 11:31:58.000000 docutils-0.9/docutils/_compat.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4544 2009-08-28 18:43:52.000000 docutils-0.9/docutils/_string_template_compat.py
--rw-r--r--   0 bert      (1001) bert      (1001)    29656 2012-03-19 22:59:09.000000 docutils-0.9/docutils/core.py
--rw-r--r--   0 bert      (1001) bert      (1001)      151 2005-09-26 17:54:39.000000 docutils-0.9/docutils/docutils.conf
--rw-r--r--   0 bert      (1001) bert      (1001)     7676 2012-01-19 11:31:58.000000 docutils-0.9/docutils/error_reporting.py
--rw-r--r--   0 bert      (1001) bert      (1001)     3959 2012-01-19 22:33:02.000000 docutils-0.9/docutils/examples.py
--rw-r--r--   0 bert      (1001) bert      (1001)    34078 2012-02-03 12:23:27.000000 docutils-0.9/docutils/frontend.py
--rw-r--r--   0 bert      (1001) bert      (1001)    16488 2012-03-19 22:59:09.000000 docutils-0.9/docutils/io.py
--rw-r--r--   0 bert      (1001) bert      (1001)    65462 2012-01-19 22:33:02.000000 docutils-0.9/docutils/nodes.py
--rw-r--r--   0 bert      (1001) bert      (1001)    57566 2012-01-19 22:33:02.000000 docutils-0.9/docutils/statemachine.py
--rw-r--r--   0 bert      (1001) bert      (1001)     6277 2006-05-21 20:44:42.000000 docutils-0.9/docutils/urischemes.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/licenses/
--rw-r--r--   0 bert      (1001) bert      (1001)     1318 2011-06-27 11:38:56.000000 docutils-0.9/licenses/BSD-2-Clause.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      151 2003-09-01 15:03:56.000000 docutils-0.9/licenses/docutils.conf
--rw-r--r--   0 bert      (1001) bert      (1001)    35147 2011-05-24 12:33:32.000000 docutils-0.9/licenses/gpl-3-0.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    11814 2003-06-16 03:16:59.000000 docutils-0.9/licenses/python-2-1-1.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/data/
--rw-r--r--   0 bert      (1001) bert      (1001)      397 2006-11-12 18:02:17.000000 docutils-0.9/test/data/config_1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      139 2004-10-17 23:19:34.000000 docutils-0.9/test/data/config_2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       39 2003-09-01 15:07:11.000000 docutils-0.9/test/data/config_error_handler.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      307 2011-11-22 14:48:14.000000 docutils-0.9/test/data/config_list.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       95 2011-11-22 14:48:14.000000 docutils-0.9/test/data/config_list_2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      266 2005-03-14 16:45:09.000000 docutils-0.9/test/data/config_old.txt
--rw-r--r--   0 bert      (1001) bert      (1001)        9 2004-09-30 10:49:47.000000 docutils-0.9/test/data/csv_data.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       38 2004-09-30 10:49:47.000000 docutils-0.9/test/data/csv_dep.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      707 2011-12-14 23:53:38.000000 docutils-0.9/test/data/dependencies.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      958 2006-03-31 03:36:28.000000 docutils-0.9/test/data/full-template.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       42 2008-12-06 21:01:57.000000 docutils-0.9/test/data/ham.css
--rw-r--r--   0 bert      (1001) bert      (1001)       33 2009-04-21 10:05:36.000000 docutils-0.9/test/data/ham.tex
--rw-r--r--   0 bert      (1001) bert      (1001)       19 2004-09-30 10:49:47.000000 docutils-0.9/test/data/include.txt
--rw-r--r--   0 bert      (1001) bert      (1001)        6 2011-11-08 17:15:46.000000 docutils-0.9/test/data/latin1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)        0 2004-09-30 10:49:47.000000 docutils-0.9/test/data/raw.txt
--rw-r--r--   0 bert      (1001) bert      (1001)        0 2004-09-30 10:49:47.000000 docutils-0.9/test/data/stylesheet.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/expected/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:29.000000 docutils-0.9/test/functional/expected/ui/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/expected/ui/default/
--rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/blank.gif
--rw-r--r--   0 bert      (1001) bert      (1001)     1003 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     1190 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/iepngfix.htc
--rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/opera.css
--rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 14:30:56.000000 docutils-0.9/test/functional/expected/ui/default/outline.css
--rw-r--r--   0 bert      (1001) bert      (1001)     4384 2005-12-13 00:31:31.000000 docutils-0.9/test/functional/expected/ui/default/pretty.css
--rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 14:30:56.000000 docutils-0.9/test/functional/expected/ui/default/print.css
--rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/s5-core.css
--rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/default/slides.css
--rw-r--r--   0 bert      (1001) bert      (1001)    15800 2006-01-05 19:30:30.000000 docutils-0.9/test/functional/expected/ui/default/slides.js
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/expected/ui/small-black/
--rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/blank.gif
--rw-r--r--   0 bert      (1001) bert      (1001)      941 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/framing.css
--rw-r--r--   0 bert      (1001) bert      (1001)     1194 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/iepngfix.htc
--rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/opera.css
--rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 14:30:56.000000 docutils-0.9/test/functional/expected/ui/small-black/outline.css
--rw-r--r--   0 bert      (1001) bert      (1001)     4030 2005-12-13 00:31:31.000000 docutils-0.9/test/functional/expected/ui/small-black/pretty.css
--rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 14:30:56.000000 docutils-0.9/test/functional/expected/ui/small-black/print.css
--rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/s5-core.css
--rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9/test/functional/expected/ui/small-black/slides.css
--rw-r--r--   0 bert      (1001) bert      (1001)    15812 2006-01-05 19:30:30.000000 docutils-0.9/test/functional/expected/ui/small-black/slides.js
--rw-r--r--   0 bert      (1001) bert      (1001)     1799 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/compact_lists.html
--rw-r--r--   0 bert      (1001) bert      (1001)     1765 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/expected/cyrillic.tex
--rw-r--r--   0 bert      (1001) bert      (1001)     2507 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/dangerous.html
--rw-r--r--   0 bert      (1001) bert      (1001)     1229 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/field_name_limit.html
--rw-r--r--   0 bert      (1001) bert      (1001)     1011 2010-10-27 09:19:58.000000 docutils-0.9/test/functional/expected/latex_docinfo.tex
--rw-r--r--   0 bert      (1001) bert      (1001)    12008 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/math_output_html.html
--rw-r--r--   0 bert      (1001) bert      (1001)     5413 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/math_output_latex.html
--rw-r--r--   0 bert      (1001) bert      (1001)     6000 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/math_output_mathjax.html
--rw-r--r--   0 bert      (1001) bert      (1001)    10314 2011-11-08 17:42:40.000000 docutils-0.9/test/functional/expected/math_output_mathml.xhtml
--rw-r--r--   0 bert      (1001) bert      (1001)     1189 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/misc_rst_html4css1.html
--rw-r--r--   0 bert      (1001) bert      (1001)     8721 2011-02-23 19:48:20.000000 docutils-0.9/test/functional/expected/odt_basic.odt
--rw-r--r--   0 bert      (1001) bert      (1001)     8999 2011-02-23 19:48:20.000000 docutils-0.9/test/functional/expected/odt_custom_headfoot.odt
--rw-r--r--   0 bert      (1001) bert      (1001)    10848 2011-03-04 23:41:40.000000 docutils-0.9/test/functional/expected/odt_tables1.odt
--rw-r--r--   0 bert      (1001) bert      (1001)     4773 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/pep_html.html
--rw-r--r--   0 bert      (1001) bert      (1001)    58051 2011-11-25 07:07:10.000000 docutils-0.9/test/functional/expected/standalone_rst_html4css1.html
--rw-r--r--   0 bert      (1001) bert      (1001)    56446 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/expected/standalone_rst_latex.tex
--rw-r--r--   0 bert      (1001) bert      (1001)     2560 2012-01-20 06:50:44.000000 docutils-0.9/test/functional/expected/standalone_rst_manpage.man
--rw-r--r--   0 bert      (1001) bert      (1001)    94985 2012-02-20 21:31:48.000000 docutils-0.9/test/functional/expected/standalone_rst_pseudoxml.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6371 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/standalone_rst_s5_html_1.html
--rw-r--r--   0 bert      (1001) bert      (1001)     6286 2011-08-30 08:12:05.000000 docutils-0.9/test/functional/expected/standalone_rst_s5_html_2.html
--rw-r--r--   0 bert      (1001) bert      (1001)    52259 2012-03-30 11:58:21.000000 docutils-0.9/test/functional/expected/standalone_rst_xetex.tex
--rw-r--r--   0 bert      (1001) bert      (1001)      618 2012-03-01 05:45:45.000000 docutils-0.9/test/functional/expected/stylesheet_path_html4css1.html
--rw-r--r--   0 bert      (1001) bert      (1001)     1818 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/expected/xetex-cyrillic.tex
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/input/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/input/data/
--rw-r--r--   0 bert      (1001) bert      (1001)      990 2010-11-09 22:53:56.000000 docutils-0.9/test/functional/input/data/custom_roles.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1505 2010-10-11 12:32:33.000000 docutils-0.9/test/functional/input/data/custom_roles_latex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      253 2004-06-22 21:24:21.000000 docutils-0.9/test/functional/input/data/errors.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       56 2005-04-07 19:36:11.000000 docutils-0.9/test/functional/input/data/header_footer.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      777 2010-02-05 14:16:25.000000 docutils-0.9/test/functional/input/data/hyperlinking.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     6585 2009-05-06 11:32:43.000000 docutils-0.9/test/functional/input/data/latex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1217 2010-05-05 12:08:10.000000 docutils-0.9/test/functional/input/data/latex_encoding.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      454 2005-04-05 02:55:06.000000 docutils-0.9/test/functional/input/data/list_table.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3106 2011-09-17 21:03:28.000000 docutils-0.9/test/functional/input/data/math.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      397 2004-09-27 18:30:29.000000 docutils-0.9/test/functional/input/data/nonalphanumeric.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      476 2009-01-30 13:37:26.000000 docutils-0.9/test/functional/input/data/option_lists.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      460 2012-02-26 21:26:12.000000 docutils-0.9/test/functional/input/data/section_titles.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    21529 2011-09-17 21:03:28.000000 docutils-0.9/test/functional/input/data/standard.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1831 2010-03-02 11:51:33.000000 docutils-0.9/test/functional/input/data/svg_images.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      648 2011-07-25 23:50:34.000000 docutils-0.9/test/functional/input/data/swf_images.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      287 2004-06-22 21:24:21.000000 docutils-0.9/test/functional/input/data/table_colspan.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1080 2004-06-22 21:24:21.000000 docutils-0.9/test/functional/input/data/table_complex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      679 2005-05-25 12:01:41.000000 docutils-0.9/test/functional/input/data/table_rowspan.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1196 2010-12-30 23:00:58.000000 docutils-0.9/test/functional/input/data/tables_latex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     2355 2010-05-05 12:08:10.000000 docutils-0.9/test/functional/input/data/unicode.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1764 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/input/data/urls.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      893 2005-12-15 14:32:01.000000 docutils-0.9/test/functional/input/compact_lists.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      711 2011-08-24 13:31:05.000000 docutils-0.9/test/functional/input/cyrillic.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      351 2005-05-03 11:12:11.000000 docutils-0.9/test/functional/input/dangerous.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      198 2005-04-04 17:05:37.000000 docutils-0.9/test/functional/input/field_list.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      247 2005-01-15 22:03:25.000000 docutils-0.9/test/functional/input/latex_docinfo.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      571 2009-10-09 06:44:02.000000 docutils-0.9/test/functional/input/link_in_substitution.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       58 2008-12-26 22:36:46.000000 docutils-0.9/test/functional/input/odt_basic.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      164 2009-12-29 19:45:17.000000 docutils-0.9/test/functional/input/odt_custom_headfoot.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     7017 2008-12-26 22:36:46.000000 docutils-0.9/test/functional/input/odt_tables1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      558 2005-04-22 23:57:18.000000 docutils-0.9/test/functional/input/pep_html.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       13 2005-02-26 18:49:25.000000 docutils-0.9/test/functional/input/simple.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      741 2010-11-09 22:53:56.000000 docutils-0.9/test/functional/input/standalone_rst_html4css1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      915 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/input/standalone_rst_latex.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1894 2010-11-05 22:09:32.000000 docutils-0.9/test/functional/input/standalone_rst_manpage.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      237 2005-12-31 02:39:07.000000 docutils-0.9/test/functional/input/standalone_rst_pseudoxml.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     2527 2005-12-08 05:37:32.000000 docutils-0.9/test/functional/input/standalone_rst_s5_html.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     1501 2012-01-26 13:08:04.000000 docutils-0.9/test/functional/input/standalone_rst_xetex.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/output/
--rw-r--r--   0 bert      (1001) bert      (1001)      130 2004-06-22 21:24:21.000000 docutils-0.9/test/functional/output/README.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/functional/tests/
--rw-r--r--   0 bert      (1001) bert      (1001)      247 2012-01-19 22:33:02.000000 docutils-0.9/test/functional/tests/_default.py
--rw-r--r--   0 bert      (1001) bert      (1001)      198 2011-09-02 21:09:13.000000 docutils-0.9/test/functional/tests/_standalone_rst_defaults.py
--rw-r--r--   0 bert      (1001) bert      (1001)      267 2005-12-15 14:32:01.000000 docutils-0.9/test/functional/tests/compact_lists.py
--rw-r--r--   0 bert      (1001) bert      (1001)      324 2012-01-19 22:33:02.000000 docutils-0.9/test/functional/tests/dangerous.py
--rw-r--r--   0 bert      (1001) bert      (1001)      335 2012-01-19 22:33:02.000000 docutils-0.9/test/functional/tests/field_name_limit.py
--rw-r--r--   0 bert      (1001) bert      (1001)      430 2011-08-24 13:31:05.000000 docutils-0.9/test/functional/tests/latex_cyrillic.py
--rw-r--r--   0 bert      (1001) bert      (1001)      295 2005-01-14 14:34:05.000000 docutils-0.9/test/functional/tests/latex_docinfo.py
--rw-r--r--   0 bert      (1001) bert      (1001)      431 2011-04-15 09:42:41.000000 docutils-0.9/test/functional/tests/math_output_html.py
--rw-r--r--   0 bert      (1001) bert      (1001)      292 2011-04-15 09:42:41.000000 docutils-0.9/test/functional/tests/math_output_latex.py
--rw-r--r--   0 bert      (1001) bert      (1001)      296 2011-04-15 09:42:41.000000 docutils-0.9/test/functional/tests/math_output_mathjax.py
--rw-r--r--   0 bert      (1001) bert      (1001)      290 2011-04-15 09:42:41.000000 docutils-0.9/test/functional/tests/math_output_mathml.py
--rw-r--r--   0 bert      (1001) bert      (1001)      429 2012-01-19 22:33:02.000000 docutils-0.9/test/functional/tests/misc_rst_html4css1.py
--rw-r--r--   0 bert      (1001) bert      (1001)      430 2005-11-30 00:06:38.000000 docutils-0.9/test/functional/tests/pep_html.py
--rw-r--r--   0 bert      (1001) bert      (1001)      323 2008-07-28 08:37:32.000000 docutils-0.9/test/functional/tests/standalone_rst_html4css1.py
--rw-r--r--   0 bert      (1001) bert      (1001)      259 2008-07-28 08:37:32.000000 docutils-0.9/test/functional/tests/standalone_rst_latex.py
--rw-r--r--   0 bert      (1001) bert      (1001)      265 2009-08-18 18:39:39.000000 docutils-0.9/test/functional/tests/standalone_rst_manpage.py
--rw-r--r--   0 bert      (1001) bert      (1001)      372 2012-02-20 21:31:48.000000 docutils-0.9/test/functional/tests/standalone_rst_pseudoxml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2409 2012-02-03 08:16:53.000000 docutils-0.9/test/functional/tests/standalone_rst_s5_html_1.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      309 2008-07-28 08:37:32.000000 docutils-0.9/test/functional/tests/standalone_rst_s5_html_2.py
--rw-r--r--   0 bert      (1001) bert      (1001)      259 2010-09-20 21:26:33.000000 docutils-0.9/test/functional/tests/standalone_rst_xetex.py
--rw-r--r--   0 bert      (1001) bert      (1001)      485 2012-03-01 05:45:45.000000 docutils-0.9/test/functional/tests/stylesheet_path_html4css1.py
--rw-r--r--   0 bert      (1001) bert      (1001)      465 2010-11-18 21:50:54.000000 docutils-0.9/test/functional/tests/xetex_cyrillic.py
--rw-r--r--   0 bert      (1001) bert      (1001)      167 2004-06-25 12:56:28.000000 docutils-0.9/test/functional/README.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/includes/
--rw-r--r--   0 bert      (1001) bert      (1001)       75 2003-01-10 02:20:18.000000 docutils-0.9/test/test_parsers/test_rst/includes/include9.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/more/
--rw-r--r--   0 bert      (1001) bert      (1001)       68 2003-01-10 02:25:51.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/more/include6.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/sibling/
--rw-r--r--   0 bert      (1001) bert      (1001)       33 2003-01-10 02:20:18.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/sibling/include7.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       52 2002-11-19 02:37:35.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/include4.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       57 2002-11-19 02:37:35.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/includes/include5.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)        0 2005-02-22 01:26:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/empty.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       10 2005-03-15 00:37:51.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include 11.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       67 2002-10-02 03:09:55.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include1.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      952 2010-04-26 10:04:17.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include10.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      169 2007-03-12 20:25:40.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include12.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      166 2007-03-12 20:25:40.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include13.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      113 2003-07-05 19:43:13.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include2.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       52 2002-11-19 02:38:28.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include3.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       55 2003-01-10 02:20:18.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include8.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      102 2009-10-25 20:47:22.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/include_literal.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       50 2002-10-02 03:09:55.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/raw1.txt
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5054 2012-02-08 19:46:11.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_admonitions.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1580 2007-05-31 00:01:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_block_quotes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1082 2007-05-31 00:01:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_class.py
--rw-r--r--   0 bert      (1001) bert      (1001)     5434 2011-12-20 14:14:21.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_code.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2414 2011-12-20 14:14:21.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_code_long.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1688 2011-11-15 07:49:01.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_code_none.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2647 2011-07-06 15:52:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_compound.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1868 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_container.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6242 2009-04-01 20:00:21.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_contents.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1301 2006-07-12 21:40:56.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_date.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1847 2006-07-12 21:40:56.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_decorations.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1806 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_default_role.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7300 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_figures.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10818 2012-02-08 19:46:11.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_images.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    28447 2012-03-19 22:59:09.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_include.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2085 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_line_blocks.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1488 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_math.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6072 2006-07-12 21:40:56.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_meta.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1708 2011-07-06 15:52:30.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_parsed_literals.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     4985 2012-03-19 22:59:09.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_raw.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     3908 2011-04-29 23:20:54.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_replace.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1744 2011-04-29 23:20:54.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_replace_fr.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6149 2010-09-18 10:43:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_role.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1766 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_rubrics.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1077 2007-05-31 00:01:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_sectnum.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1905 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_sidebars.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    30924 2012-01-19 11:31:58.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_tables.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1717 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_target_notes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5883 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_test_directives.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      624 2007-05-31 00:01:52.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_title.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5059 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_topics.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5423 2009-04-01 20:00:21.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_unicode.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2392 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/test_unknown.py
--rw-r--r--   0 bert      (1001) bert      (1001)      386 2004-09-12 21:21:50.000000 docutils-0.9/test/test_parsers/test_rst/test_directives/utf-16.csv
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_parsers/test_rst/__init__.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     3358 2012-01-11 20:28:57.000000 docutils-0.9/test/test_parsers/test_rst/test_SimpleTableParser.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6099 2012-01-11 20:28:57.000000 docutils-0.9/test/test_parsers/test_rst/test_TableParser.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6665 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_block_quotes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     3903 2006-06-04 21:38:21.000000 docutils-0.9/test/test_parsers/test_rst/test_bullet_lists.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     4231 2008-02-15 09:23:07.000000 docutils-0.9/test/test_parsers/test_rst/test_citations.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6595 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_comments.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    11375 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_definition_lists.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1388 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_doctest_blocks.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     9370 2012-01-11 20:28:57.000000 docutils-0.9/test/test_parsers/test_rst/test_east_asian_text.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    20470 2007-03-21 19:51:22.000000 docutils-0.9/test/test_parsers/test_rst/test_enumerated_lists.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    13445 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_field_lists.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     9448 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_footnotes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1041 2012-02-03 08:16:53.000000 docutils-0.9/test/test_parsers/test_rst/test_functions.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    41730 2011-12-05 19:35:32.000000 docutils-0.9/test/test_parsers/test_rst/test_inline_markup.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10216 2011-12-20 14:14:21.000000 docutils-0.9/test/test_parsers/test_rst/test_interpreted.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1316 2011-04-25 23:07:32.000000 docutils-0.9/test/test_parsers/test_rst/test_interpreted_fr.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7057 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_line_blocks.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6929 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_literal_blocks.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    20371 2011-09-17 18:00:35.000000 docutils-0.9/test/test_parsers/test_rst/test_option_lists.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2001 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_outdenting.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1329 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_paragraphs.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    20420 2010-11-10 13:43:50.000000 docutils-0.9/test/test_parsers/test_rst/test_section_headers.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     8883 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_substitutions.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    37488 2012-01-11 20:28:57.000000 docutils-0.9/test/test_parsers/test_rst/test_tables.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    13765 2011-06-30 22:14:29.000000 docutils-0.9/test/test_parsers/test_rst/test_targets.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5276 2006-05-21 20:44:42.000000 docutils-0.9/test/test_parsers/test_rst/test_transitions.py
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_parsers/__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1214 2009-04-01 20:00:21.000000 docutils-0.9/test/test_parsers/test_parser.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_readers/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_readers/test_pep/
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_readers/test_pep/__init__.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     3252 2006-05-21 20:44:42.000000 docutils-0.9/test/test_readers/test_pep/test_inline_markup.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6073 2006-05-21 20:44:42.000000 docutils-0.9/test/test_readers/test_pep/test_rfc2822.py
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_readers/__init__.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_transforms/
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_transforms/__init__.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1136 2007-05-31 00:01:52.000000 docutils-0.9/test/test_transforms/test___init__.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     4087 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_class.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10659 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_contents.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     9313 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_docinfo.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     4784 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_doctitle.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      988 2007-05-31 00:01:52.000000 docutils-0.9/test/test_transforms/test_expose_internals.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      908 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_filter.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    15793 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_footnotes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    23349 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_hyperlinks.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1858 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_messages.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1698 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_peps.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     9336 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_sectnum.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      948 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_strip_comments.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10096 2010-07-03 14:19:09.000000 docutils-0.9/test/test_transforms/test_substitutions.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2301 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_target_notes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7537 2006-05-21 20:44:42.000000 docutils-0.9/test/test_transforms/test_transitions.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1705 2007-05-31 00:01:52.000000 docutils-0.9/test/test_transforms/test_writer_aux.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/test/test_writers/
--rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9/test/test_writers/__init__.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5871 2012-01-18 10:16:20.000000 docutils-0.9/test/test_writers/test_docutils_xml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1088 2012-01-19 22:33:02.000000 docutils-0.9/test/test_writers/test_html4css1_misc.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10449 2010-12-13 22:06:48.000000 docutils-0.9/test/test_writers/test_html4css1_parts.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5006 2010-07-19 16:07:19.000000 docutils-0.9/test/test_writers/test_html4css1_template.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    12141 2012-01-26 13:08:04.000000 docutils-0.9/test/test_writers/test_latex2e.py
--rw-r--r--   0 bert      (1001) bert      (1001)     4674 2012-01-20 06:50:44.000000 docutils-0.9/test/test_writers/test_manpage.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      528 2007-05-31 00:01:52.000000 docutils-0.9/test/test_writers/test_null.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6437 2012-02-03 08:16:53.000000 docutils-0.9/test/test_writers/test_odt.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      898 2007-05-31 00:01:52.000000 docutils-0.9/test/test_writers/test_pseudoxml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     4364 2010-07-19 16:07:19.000000 docutils-0.9/test/test_writers/test_s5.py
--rw-r--r--   0 bert      (1001) bert      (1001)    32002 2012-05-01 08:34:41.000000 docutils-0.9/test/DocutilsTestSupport.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2601 2011-06-05 13:12:06.000000 docutils-0.9/test/alltests.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1306 2008-03-30 09:05:39.000000 docutils-0.9/test/coverage.sh
--rw-r--r--   0 bert      (1001) bert      (1001)      382 2004-06-25 22:12:37.000000 docutils-0.9/test/docutils.conf
--rw-r--r--   0 bert      (1001) bert      (1001)     5347 2012-01-19 22:33:02.000000 docutils-0.9/test/package_unittest.py
--rw-r--r--   0 bert      (1001) bert      (1001)      763 2012-02-03 08:16:53.000000 docutils-0.9/test/test__init__.py
--rw-r--r--   0 bert      (1001) bert      (1001)     1495 2011-12-05 21:20:43.000000 docutils-0.9/test/test_command_line.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     5294 2012-05-01 16:07:54.000000 docutils-0.9/test/test_dependencies.py
--rw-r--r--   0 bert      (1001) bert      (1001)    12397 2012-02-03 08:16:53.000000 docutils-0.9/test/test_error_reporting.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     8279 2012-02-03 08:16:53.000000 docutils-0.9/test/test_functional.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     3370 2012-05-01 08:34:41.000000 docutils-0.9/test/test_io.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7886 2010-09-28 08:21:25.000000 docutils-0.9/test/test_language.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    24938 2012-05-01 08:34:41.000000 docutils-0.9/test/test_nodes.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      772 2012-02-03 08:16:53.000000 docutils-0.9/test/test_pickle.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6172 2012-03-19 22:59:09.000000 docutils-0.9/test/test_publisher.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7965 2012-05-01 08:34:41.000000 docutils-0.9/test/test_settings.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    10992 2012-05-01 08:34:41.000000 docutils-0.9/test/test_statemachine.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2200 2012-05-01 08:34:41.000000 docutils-0.9/test/test_traversals.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)    11491 2012-02-03 12:22:14.000000 docutils-0.9/test/test_utils.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     7262 2012-05-01 08:34:41.000000 docutils-0.9/test/test_viewlist.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/dev/
--rw-r--r--   0 bert      (1001) bert      (1001)       22 2005-06-15 23:54:52.000000 docutils-0.9/tools/dev/README.txt
--rwxr-xr-x   0 bert      (1001) bert      (1001)     2663 2007-05-31 00:01:52.000000 docutils-0.9/tools/dev/create_unimap.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      923 2008-07-28 08:37:32.000000 docutils-0.9/tools/dev/profile_docutils.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6630 2008-07-28 08:37:32.000000 docutils-0.9/tools/dev/unicode2rstsubs.py
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/editors/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/editors/emacs/
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/editors/emacs/tests/
--rw-r--r--   0 bert      (1001) bert      (1001)      334 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/Makefile
--rw-r--r--   0 bert      (1001) bert      (1001)      566 2010-12-12 18:32:18.000000 docutils-0.9/tools/editors/emacs/tests/README.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     9192 2010-12-22 19:50:48.000000 docutils-0.9/tools/editors/emacs/tests/adjust-section.el
--rw-r--r--   0 bert      (1001) bert      (1001)    13397 2011-01-23 12:38:49.000000 docutils-0.9/tools/editors/emacs/tests/adornment.el
--rw-r--r--   0 bert      (1001) bert      (1001)     3282 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/comment.el
--rw-r--r--   0 bert      (1001) bert      (1001)     9290 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/ert-support.el
--rw-r--r--   0 bert      (1001) bert      (1001)    10305 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/fill.el
--rw-r--r--   0 bert      (1001) bert      (1001)     3117 2012-04-29 14:50:25.000000 docutils-0.9/tools/editors/emacs/tests/font-lock.el
--rw-r--r--   0 bert      (1001) bert      (1001)     4853 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/indent.el
--rw-r--r--   0 bert      (1001) bert      (1001)     4273 2010-12-12 18:32:18.000000 docutils-0.9/tools/editors/emacs/tests/items.el
--rw-r--r--   0 bert      (1001) bert      (1001)     3665 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/movement.el
--rw-r--r--   0 bert      (1001) bert      (1001)    32165 2012-04-29 14:50:25.000000 docutils-0.9/tools/editors/emacs/tests/re.el
--rw-r--r--   0 bert      (1001) bert      (1001)    11853 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/shift.el
--rw-r--r--   0 bert      (1001) bert      (1001)     3689 2011-03-20 17:20:36.000000 docutils-0.9/tools/editors/emacs/tests/support.el
--rw-r--r--   0 bert      (1001) bert      (1001)     3335 2010-12-12 18:32:18.000000 docutils-0.9/tools/editors/emacs/tests/toc.el
--rw-r--r--   0 bert      (1001) bert      (1001)     7460 2012-04-29 14:50:25.000000 docutils-0.9/tools/editors/emacs/IDEAS.rst
--rw-r--r--   0 bert      (1001) bert      (1001)     1097 2008-11-26 18:07:47.000000 docutils-0.9/tools/editors/emacs/README.txt
--rw-r--r--   0 bert      (1001) bert      (1001)       34 2005-03-15 00:43:13.000000 docutils-0.9/tools/editors/emacs/docutils.conf
--rw-r--r--   0 bert      (1001) bert      (1001)   143978 2012-04-29 15:01:05.000000 docutils-0.9/tools/editors/emacs/rst.el
--rw-r--r--   0 bert      (1001) bert      (1001)      873 2006-08-14 16:08:29.000000 docutils-0.9/tools/editors/README.txt
-drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-05-02 18:31:30.000000 docutils-0.9/tools/test/
--rw-r--r--   0 bert      (1001) bert      (1001)     3008 2010-07-10 06:57:08.000000 docutils-0.9/tools/test/test_buildhtml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     9897 2012-01-23 20:57:29.000000 docutils-0.9/tools/buildhtml.py
--rw-r--r--   0 bert      (1001) bert      (1001)      327 2005-12-12 00:05:55.000000 docutils-0.9/tools/docutils.conf
--rwxr-xr-x   0 bert      (1001) bert      (1001)     6832 2010-03-09 14:53:16.000000 docutils-0.9/tools/quicktest.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      597 2006-05-21 20:44:42.000000 docutils-0.9/tools/rst2html.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      794 2009-04-16 12:04:49.000000 docutils-0.9/tools/rst2latex.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      603 2009-08-18 18:39:39.000000 docutils-0.9/tools/rst2man.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      767 2009-01-07 19:09:28.000000 docutils-0.9/tools/rst2odt.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)     1701 2009-01-07 19:09:28.000000 docutils-0.9/tools/rst2odt_prepstyles.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      604 2006-05-21 20:44:42.000000 docutils-0.9/tools/rst2pseudoxml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      640 2006-05-21 20:44:42.000000 docutils-0.9/tools/rst2s5.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      789 2011-05-19 09:12:02.000000 docutils-0.9/tools/rst2xetex.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      605 2006-05-21 20:44:42.000000 docutils-0.9/tools/rst2xml.py
--rwxr-xr-x   0 bert      (1001) bert      (1001)      673 2006-05-21 20:44:42.000000 docutils-0.9/tools/rstpep2html.py
--rw-r--r--   0 bert      (1001) bert      (1001)     9629 2012-01-04 14:20:52.000000 docutils-0.9/BUGS.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     5056 2011-12-31 14:22:16.000000 docutils-0.9/COPYING.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    48256 2012-02-16 17:15:55.000000 docutils-0.9/FAQ.txt
--rw-r--r--   0 bert      (1001) bert      (1001)   103376 2012-05-02 17:13:41.000000 docutils-0.9/HISTORY.txt
--rw-r--r--   0 bert      (1001) bert      (1001)      293 2010-03-05 09:34:44.000000 docutils-0.9/MANIFEST.in
--rw-r--r--   0 bert      (1001) bert      (1001)    11187 2012-02-28 16:39:05.000000 docutils-0.9/README.txt
--rw-r--r--   0 bert      (1001) bert      (1001)    13052 2012-05-02 17:13:41.000000 docutils-0.9/RELEASE-NOTES.txt
--rw-r--r--   0 bert      (1001) bert      (1001)     3174 2008-08-25 13:07:53.000000 docutils-0.9/THANKS.txt
--rwxr-xr-x   0 bert      (1001) bert      (1001)      685 2004-07-13 15:57:13.000000 docutils-0.9/install.py
--rw-r--r--   0 bert      (1001) bert      (1001)      217 2011-07-07 06:59:46.000000 docutils-0.9/setup.cfg
--rwxr-xr-x   0 bert      (1001) bert      (1001)     8408 2011-12-20 16:39:10.000000 docutils-0.9/setup.py
--rw-r--r--   0 bert      (1001) bert      (1001)     2170 2012-05-02 18:31:30.000000 docutils-0.9/PKG-INFO
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/api/
+-rw-r--r--   0 bert      (1001) bert      (1001)     2327 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/api/cmdline-tool.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    10584 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/api/publisher.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     8186 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/api/runtime-settings.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/dev/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/dev/rst/
+-rw-r--r--   0 bert      (1001) bert      (1001)   113248 2012-03-19 17:04:49.000000 docutils-0.9.1/docs/dev/rst/alternatives.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    35546 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/rst/problems.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4048 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/distributing.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    17005 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/enthought-plan.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4522 2005-10-30 14:23:25.000000 docutils-0.9.1/docs/dev/enthought-rfp.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     9218 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/hacking.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    24730 2012-03-10 22:46:07.000000 docutils-0.9.1/docs/dev/policies.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7385 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/pysource.dtd
+-rw-r--r--   0 bert      (1001) bert      (1001)     4433 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/pysource.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     5368 2012-05-02 07:22:20.000000 docutils-0.9.1/docs/dev/release.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6161 2012-01-26 09:57:04.000000 docutils-0.9.1/docs/dev/repository.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4564 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/semantics.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7960 2011-12-02 00:43:32.000000 docutils-0.9.1/docs/dev/testing.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    93495 2012-02-27 11:15:38.000000 docutils-0.9.1/docs/dev/todo.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3316 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/dev/website.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/howto/
+-rw-r--r--   0 bert      (1001) bert      (1001)     3340 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/howto/html-stylesheets.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7451 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/howto/i18n.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    16395 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/howto/rst-directives.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     8683 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/howto/rst-roles.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     5831 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/howto/security.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/peps/
+-rw-r--r--   0 bert      (1001) bert      (1001)    10405 2006-05-21 20:44:42.000000 docutils-0.9.1/docs/peps/pep-0256.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    11738 2006-05-21 20:44:42.000000 docutils-0.9.1/docs/peps/pep-0257.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    36245 2009-10-05 19:08:10.000000 docutils-0.9.1/docs/peps/pep-0258.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    32597 2006-05-21 20:44:42.000000 docutils-0.9.1/docs/peps/pep-0287.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/ref/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/ref/rst/
+-rw-r--r--   0 bert      (1001) bert      (1001)     7669 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/rst/definitions.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    59068 2012-01-06 11:11:51.000000 docutils-0.9.1/docs/ref/rst/directives.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    14090 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/rst/introduction.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)   106881 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/rst/restructuredtext.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    10218 2012-01-06 11:11:51.000000 docutils-0.9.1/docs/ref/rst/roles.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)   117426 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/doctree.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    16728 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/docutils.dtd
+-rw-r--r--   0 bert      (1001) bert      (1001)    12744 2002-04-20 03:01:52.000000 docutils-0.9.1/docs/ref/soextblx.dtd
+-rw-r--r--   0 bert      (1001) bert      (1001)     3780 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/ref/transforms.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/user/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/user/images/
+-rw-r--r--   0 bert      (1001) bert      (1001)    19823 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/big-black.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    25697 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/big-white.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    59358 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/default.png
+-rw-r--r--   0 bert      (1001) bert      (1001)     5202 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/happy_monkey.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    24021 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/medium-black.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    33756 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/medium-white.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    32565 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-all.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    17754 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-breaks.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    19080 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-covers.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    20751 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-cuts.png
+-rw-r--r--   0 bert      (1001) bert      (1001)     4900 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-empty.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    21291 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/rsp-objects.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    49418 2005-11-29 01:48:42.000000 docutils-0.9.1/docs/user/images/rsp.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)    25404 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/s5-files.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    39029 2005-12-03 02:24:44.000000 docutils-0.9.1/docs/user/images/s5-files.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)    41144 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/small-black.png
+-rw-r--r--   0 bert      (1001) bert      (1001)    41120 2005-12-08 04:43:13.000000 docutils-0.9.1/docs/user/images/small-white.png
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/user/rst/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docs/user/rst/images/
+-rw-r--r--   0 bert      (1001) bert      (1001)     4361 2005-07-07 23:47:11.000000 docutils-0.9.1/docs/user/rst/images/ball1.gif
+-rw-r--r--   0 bert      (1001) bert      (1001)     7646 2010-03-02 00:24:53.000000 docutils-0.9.1/docs/user/rst/images/biohazard-scaling.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)      179 2005-07-07 23:47:11.000000 docutils-0.9.1/docs/user/rst/images/biohazard.png
+-rw-r--r--   0 bert      (1001) bert      (1001)     7609 2010-03-02 11:51:33.000000 docutils-0.9.1/docs/user/rst/images/biohazard.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)     1307 2010-03-09 14:42:58.000000 docutils-0.9.1/docs/user/rst/images/biohazard.swf
+-rw-r--r--   0 bert      (1001) bert      (1001)     2609 2010-03-02 00:24:53.000000 docutils-0.9.1/docs/user/rst/images/title-scaling.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)     1155 2009-05-11 14:41:43.000000 docutils-0.9.1/docs/user/rst/images/title.png
+-rw-r--r--   0 bert      (1001) bert      (1001)     2580 2010-03-02 00:24:53.000000 docutils-0.9.1/docs/user/rst/images/title.svg
+-rw-r--r--   0 bert      (1001) bert      (1001)     6982 2011-06-17 10:50:48.000000 docutils-0.9.1/docs/user/rst/cheatsheet.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    14680 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/rst/demo.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    52658 2009-07-14 14:05:34.000000 docutils-0.9.1/docs/user/rst/quickref.html
+-rw-r--r--   0 bert      (1001) bert      (1001)    11275 2008-12-07 14:15:30.000000 docutils-0.9.1/docs/user/rst/quickstart.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      224 2006-01-05 12:56:20.000000 docutils-0.9.1/docs/user/Makefile.docutils-update
+-rw-r--r--   0 bert      (1001) bert      (1001)    48092 2012-02-26 19:13:26.000000 docutils-0.9.1/docs/user/config.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    21537 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/docutils-05-compat.sty.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    22304 2010-06-17 20:16:08.000000 docutils-0.9.1/docs/user/emacs.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    57844 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/latex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    12652 2012-02-13 16:55:05.000000 docutils-0.9.1/docs/user/links.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     5488 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/mailing-lists.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     5113 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/manpage.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    37993 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/odt.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    25328 2006-03-30 14:29:59.000000 docutils-0.9.1/docs/user/slide-shows.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    12451 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/user/tools.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     8267 2012-01-03 19:23:53.000000 docutils-0.9.1/docs/index.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/languages/
+-rw-r--r--   0 bert      (1001) bert      (1001)     1332 2011-09-16 19:24:51.000000 docutils-0.9.1/docutils/languages/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1824 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/af.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1940 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/ca.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1928 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/cs.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1722 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/de.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1848 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/en.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1948 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/eo.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1962 2006-05-25 20:48:37.000000 docutils-0.9.1/docutils/languages/es.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2026 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/fi.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1893 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/fr.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2040 2008-09-05 15:07:51.000000 docutils-0.9.1/docutils/languages/gl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2683 2006-12-26 09:59:41.000000 docutils-0.9.1/docutils/languages/he.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1808 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/it.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1942 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/ja.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3856 2010-10-29 22:07:34.000000 docutils-0.9.1/docutils/languages/lt.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1865 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/nl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1900 2008-08-25 13:07:53.000000 docutils-0.9.1/docutils/languages/pl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1982 2008-06-03 01:11:03.000000 docutils-0.9.1/docutils/languages/pt_br.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2155 2011-09-16 18:36:18.000000 docutils-0.9.1/docutils/languages/ru.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1860 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/sk.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2072 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/sv.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2026 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/zh_cn.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2771 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/languages/zh_tw.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/math/
+-rw-r--r--   0 bert      (1001) bert      (1001)     1683 2011-11-08 17:42:40.000000 docutils-0.9.1/docutils/math/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    17206 2011-11-08 17:42:40.000000 docutils-0.9.1/docutils/math/latex2mathml.py
+-rw-r--r--   0 bert      (1001) bert      (1001)   174454 2012-05-03 11:26:37.000000 docutils-0.9.1/docutils/math/math2html.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    35108 2011-11-08 17:42:40.000000 docutils-0.9.1/docutils/math/tex2unichar.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    17590 2011-11-08 17:42:40.000000 docutils-0.9.1/docutils/math/unichar2tex.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/parsers/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/parsers/rst/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/parsers/rst/directives/
+-rw-r--r--   0 bert      (1001) bert      (1001)    13382 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/directives/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2273 2011-07-06 15:52:30.000000 docutils-0.9.1/docutils/parsers/rst/directives/admonitions.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     9243 2011-12-20 14:14:21.000000 docutils-0.9.1/docutils/parsers/rst/directives/body.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3098 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/parsers/rst/directives/html.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6769 2011-12-14 23:53:38.000000 docutils-0.9.1/docutils/parsers/rst/directives/images.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    22117 2012-05-11 21:03:07.000000 docutils-0.9.1/docutils/parsers/rst/directives/misc.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4251 2012-01-06 12:08:43.000000 docutils-0.9.1/docutils/parsers/rst/directives/parts.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      831 2011-06-30 22:14:29.000000 docutils-0.9.1/docutils/parsers/rst/directives/references.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    20048 2012-01-27 08:41:35.000000 docutils-0.9.1/docutils/parsers/rst/directives/tables.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/parsers/rst/include/
+-rw-r--r--   0 bert      (1001) bert      (1001)      666 2005-06-12 20:34:06.000000 docutils-0.9.1/docutils/parsers/rst/include/README.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    10925 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamsa.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7242 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamsb.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1723 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamsc.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6721 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamsn.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3825 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamso.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    11763 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isoamsr.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3101 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isobox.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4241 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isocyr1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1882 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isocyr2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      869 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isodia.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3010 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isogrk1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1705 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isogrk2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     2880 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isogrk3.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3035 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isogrk4-wide.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      372 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isogrk4.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4397 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isolat1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     8466 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isolat2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3334 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomfrk-wide.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      519 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomfrk.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1931 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomopf-wide.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      639 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomopf.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3231 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomscr-wide.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      776 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isomscr.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4066 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isonum.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4613 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isopub.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     9726 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/isotech.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    45428 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/mmlalias.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     9010 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/mmlextra-wide.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6800 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/mmlextra.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1036 2006-02-26 16:16:59.000000 docutils-0.9.1/docutils/parsers/rst/include/s5defs.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6112 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1945 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/xhtml1-special.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7028 2005-06-12 16:40:14.000000 docutils-0.9.1/docutils/parsers/rst/include/xhtml1-symbol.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/parsers/rst/languages/
+-rw-r--r--   0 bert      (1001) bert      (1001)      800 2010-09-17 21:38:29.000000 docutils-0.9.1/docutils/parsers/rst/languages/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3677 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/af.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4467 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/ca.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4857 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/cs.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3465 2011-11-21 16:43:06.000000 docutils-0.9.1/docutils/parsers/rst/languages/de.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3317 2011-10-15 22:06:45.000000 docutils-0.9.1/docutils/parsers/rst/languages/en.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3898 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/eo.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4261 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/es.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3661 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/fi.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3709 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/fr.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3711 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/gl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3640 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/he.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3270 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/it.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3863 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/ja.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3583 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/lt.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3708 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/nl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3427 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/pl.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3992 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/pt_br.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3306 2011-09-12 08:28:31.000000 docutils-0.9.1/docutils/parsers/rst/languages/ru.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3979 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/sk.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4166 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/sv.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4007 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/zh_cn.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     5172 2011-09-02 13:00:23.000000 docutils-0.9.1/docutils/parsers/rst/languages/zh_tw.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    14890 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/parsers/rst/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    14712 2012-01-09 15:01:15.000000 docutils-0.9.1/docutils/parsers/rst/roles.py
+-rw-r--r--   0 bert      (1001) bert      (1001)   128822 2012-02-20 21:31:48.000000 docutils-0.9.1/docutils/parsers/rst/states.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    21007 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/parsers/rst/tableparser.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1457 2008-07-28 08:37:32.000000 docutils-0.9.1/docutils/parsers/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      445 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/parsers/null.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/readers/
+-rw-r--r--   0 bert      (1001) bert      (1001)     3265 2008-07-28 08:37:32.000000 docutils-0.9.1/docutils/readers/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1607 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/readers/doctree.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1555 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/readers/pep.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2340 2006-11-12 18:02:17.000000 docutils-0.9.1/docutils/readers/standalone.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/transforms/
+-rw-r--r--   0 bert      (1001) bert      (1001)     6505 2010-09-28 08:21:25.000000 docutils-0.9.1/docutils/transforms/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1993 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/transforms/components.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    18879 2008-07-28 08:37:32.000000 docutils-0.9.1/docutils/transforms/frontmatter.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4882 2010-04-26 10:04:17.000000 docutils-0.9.1/docutils/transforms/misc.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6980 2009-08-06 12:21:10.000000 docutils-0.9.1/docutils/transforms/parts.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    11065 2010-09-28 08:21:25.000000 docutils-0.9.1/docutils/transforms/peps.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    36093 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/transforms/references.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6577 2009-09-03 07:27:59.000000 docutils-0.9.1/docutils/transforms/universal.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2609 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/transforms/writer_aux.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/utils/
+-rw-r--r--   0 bert      (1001) bert      (1001)    26763 2012-02-03 12:22:14.000000 docutils-0.9.1/docutils/utils/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4871 2011-12-20 14:14:21.000000 docutils-0.9.1/docutils/utils/code_analyzer.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     9473 2012-05-01 09:50:02.000000 docutils-0.9.1/docutils/utils/punctuation_chars.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2687 2011-12-20 16:39:10.000000 docutils-0.9.1/docutils/utils/roman.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/html4css1/
+-rw-r--r--   0 bert      (1001) bert      (1001)    65633 2012-01-27 08:41:35.000000 docutils-0.9.1/docutils/writers/html4css1/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6164 2012-05-11 21:06:27.000000 docutils-0.9.1/docutils/writers/html4css1/html4css1.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     4720 2011-06-27 11:38:56.000000 docutils-0.9.1/docutils/writers/html4css1/math.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      114 2006-03-31 03:36:28.000000 docutils-0.9.1/docutils/writers/html4css1/template.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/latex2e/
+-rw-r--r--   0 bert      (1001) bert      (1001)   121530 2012-03-30 11:58:21.000000 docutils-0.9.1/docutils/writers/latex2e/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      476 2010-09-20 13:07:30.000000 docutils-0.9.1/docutils/writers/latex2e/default.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)    22419 2011-12-02 00:43:32.000000 docutils-0.9.1/docutils/writers/latex2e/docutils-05-compat.sty
+-rw-r--r--   0 bert      (1001) bert      (1001)      534 2010-09-15 11:09:45.000000 docutils-0.9.1/docutils/writers/latex2e/titlepage.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)      515 2010-10-16 18:49:04.000000 docutils-0.9.1/docutils/writers/latex2e/xelatex.tex
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/odf_odt/
+-rw-r--r--   0 bert      (1001) bert      (1001)   124894 2012-05-03 10:55:30.000000 docutils-0.9.1/docutils/writers/odf_odt/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4671 2009-01-19 21:02:02.000000 docutils-0.9.1/docutils/writers/odf_odt/pygmentsformatter.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    16500 2011-06-27 05:39:48.000000 docutils-0.9.1/docutils/writers/odf_odt/styles.odt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/pep_html/
+-rw-r--r--   0 bert      (1001) bert      (1001)     3583 2010-05-23 21:20:29.000000 docutils-0.9.1/docutils/writers/pep_html/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6367 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/writers/pep_html/pep.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     1294 2006-03-31 03:36:28.000000 docutils-0.9.1/docutils/writers/pep_html/template.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-black/
+-rw-r--r--   0 bert      (1001) bert      (1001)       38 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-black/__base__
+-rw-r--r--   0 bert      (1001) bert      (1001)      911 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     3606 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-black/pretty.css
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-white/
+-rw-r--r--   0 bert      (1001) bert      (1001)      906 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     3566 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/big-white/pretty.css
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/
+-rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/blank.gif
+-rw-r--r--   0 bert      (1001) bert      (1001)     1003 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     1190 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/iepngfix.htc
+-rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/opera.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 02:21:46.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/outline.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     4384 2005-12-13 00:30:07.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/pretty.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 02:21:46.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/print.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/slides.css
+-rw-r--r--   0 bert      (1001) bert      (1001)    15800 2006-01-05 12:55:51.000000 docutils-0.9.1/docutils/writers/s5_html/themes/default/slides.js
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-black/
+-rw-r--r--   0 bert      (1001) bert      (1001)       41 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-black/__base__
+-rw-r--r--   0 bert      (1001) bert      (1001)     4031 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-black/pretty.css
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-white/
+-rw-r--r--   0 bert      (1001) bert      (1001)      944 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     3991 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/medium-white/pretty.css
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-black/
+-rw-r--r--   0 bert      (1001) bert      (1001)       40 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-black/__base__
+-rw-r--r--   0 bert      (1001) bert      (1001)     4030 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-black/pretty.css
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-white/
+-rw-r--r--   0 bert      (1001) bert      (1001)      941 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     4001 2007-04-09 15:15:57.000000 docutils-0.9.1/docutils/writers/s5_html/themes/small-white/pretty.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      301 2005-12-08 04:43:13.000000 docutils-0.9.1/docutils/writers/s5_html/themes/README.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    14394 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/writers/s5_html/__init__.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/docutils/writers/xetex/
+-rw-r--r--   0 bert      (1001) bert      (1001)     5079 2012-03-30 11:58:21.000000 docutils-0.9.1/docutils/writers/xetex/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4283 2012-01-19 11:55:26.000000 docutils-0.9.1/docutils/writers/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6271 2012-01-18 10:16:20.000000 docutils-0.9.1/docutils/writers/docutils_xml.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    34888 2012-01-20 06:50:44.000000 docutils-0.9.1/docutils/writers/manpage.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      450 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/writers/null.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      772 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/writers/pseudoxml.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     7427 2012-06-17 20:47:10.000000 docutils-0.9.1/docutils/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1183 2012-01-19 11:31:58.000000 docutils-0.9.1/docutils/_compat.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4544 2009-08-28 18:43:52.000000 docutils-0.9.1/docutils/_string_template_compat.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    29656 2012-03-19 22:59:09.000000 docutils-0.9.1/docutils/core.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      151 2005-09-26 17:54:39.000000 docutils-0.9.1/docutils/docutils.conf
+-rw-r--r--   0 bert      (1001) bert      (1001)     7612 2012-05-03 11:01:54.000000 docutils-0.9.1/docutils/error_reporting.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     3959 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/examples.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    34078 2012-02-03 12:23:27.000000 docutils-0.9.1/docutils/frontend.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    17891 2012-06-13 14:14:12.000000 docutils-0.9.1/docutils/io.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    65462 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/nodes.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    57566 2012-01-19 22:33:02.000000 docutils-0.9.1/docutils/statemachine.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     6277 2006-05-21 20:44:42.000000 docutils-0.9.1/docutils/urischemes.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/licenses/
+-rw-r--r--   0 bert      (1001) bert      (1001)     1318 2011-06-27 11:38:56.000000 docutils-0.9.1/licenses/BSD-2-Clause.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      151 2003-09-01 15:03:56.000000 docutils-0.9.1/licenses/docutils.conf
+-rw-r--r--   0 bert      (1001) bert      (1001)    35147 2011-05-24 12:33:32.000000 docutils-0.9.1/licenses/gpl-3-0.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    11814 2003-06-16 03:16:59.000000 docutils-0.9.1/licenses/python-2-1-1.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/data/
+-rw-r--r--   0 bert      (1001) bert      (1001)      397 2006-11-12 18:02:17.000000 docutils-0.9.1/test/data/config_1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      139 2004-10-17 23:19:34.000000 docutils-0.9.1/test/data/config_2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       39 2003-09-01 15:07:11.000000 docutils-0.9.1/test/data/config_error_handler.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      307 2011-11-22 14:48:14.000000 docutils-0.9.1/test/data/config_list.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       95 2011-11-22 14:48:14.000000 docutils-0.9.1/test/data/config_list_2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      266 2005-03-14 16:45:09.000000 docutils-0.9.1/test/data/config_old.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)        9 2004-09-30 10:49:47.000000 docutils-0.9.1/test/data/csv_data.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       38 2004-09-30 10:49:47.000000 docutils-0.9.1/test/data/csv_dep.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      707 2011-12-14 23:53:38.000000 docutils-0.9.1/test/data/dependencies.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      958 2006-03-31 03:36:28.000000 docutils-0.9.1/test/data/full-template.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       42 2008-12-06 21:01:57.000000 docutils-0.9.1/test/data/ham.css
+-rw-r--r--   0 bert      (1001) bert      (1001)       33 2009-04-21 10:05:36.000000 docutils-0.9.1/test/data/ham.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)       19 2004-09-30 10:49:47.000000 docutils-0.9.1/test/data/include.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)        6 2011-11-08 17:15:46.000000 docutils-0.9.1/test/data/latin1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)        0 2004-09-30 10:49:47.000000 docutils-0.9.1/test/data/raw.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)        0 2004-09-30 10:49:47.000000 docutils-0.9.1/test/data/stylesheet.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/expected/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/expected/ui/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/expected/ui/default/
+-rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/blank.gif
+-rw-r--r--   0 bert      (1001) bert      (1001)     1003 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     1190 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/iepngfix.htc
+-rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/opera.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 14:30:56.000000 docutils-0.9.1/test/functional/expected/ui/default/outline.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     4384 2005-12-13 00:31:31.000000 docutils-0.9.1/test/functional/expected/ui/default/pretty.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 14:30:56.000000 docutils-0.9.1/test/functional/expected/ui/default/print.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/s5-core.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/default/slides.css
+-rw-r--r--   0 bert      (1001) bert      (1001)    15800 2006-01-05 19:30:30.000000 docutils-0.9.1/test/functional/expected/ui/default/slides.js
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/expected/ui/small-black/
+-rw-r--r--   0 bert      (1001) bert      (1001)       49 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/blank.gif
+-rw-r--r--   0 bert      (1001) bert      (1001)      941 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/framing.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     1194 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/iepngfix.htc
+-rw-r--r--   0 bert      (1001) bert      (1001)      261 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/opera.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      648 2005-12-13 14:30:56.000000 docutils-0.9.1/test/functional/expected/ui/small-black/outline.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     4030 2005-12-13 00:31:31.000000 docutils-0.9.1/test/functional/expected/ui/small-black/pretty.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      818 2005-12-13 14:30:56.000000 docutils-0.9.1/test/functional/expected/ui/small-black/print.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      451 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/s5-core.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      283 2005-12-08 04:43:13.000000 docutils-0.9.1/test/functional/expected/ui/small-black/slides.css
+-rw-r--r--   0 bert      (1001) bert      (1001)    15812 2006-01-05 19:30:30.000000 docutils-0.9.1/test/functional/expected/ui/small-black/slides.js
+-rw-r--r--   0 bert      (1001) bert      (1001)     1779 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/compact_lists.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     1765 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/expected/cyrillic.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)     2487 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/dangerous.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     1209 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/field_name_limit.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     1011 2010-10-27 09:19:58.000000 docutils-0.9.1/test/functional/expected/latex_docinfo.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)    11966 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/math_output_html.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     5393 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/math_output_latex.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     5980 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/math_output_mathjax.html
+-rw-r--r--   0 bert      (1001) bert      (1001)    10294 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/math_output_mathml.xhtml
+-rw-r--r--   0 bert      (1001) bert      (1001)     1191 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/misc_rst_html4css1.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     8721 2011-02-23 19:48:20.000000 docutils-0.9.1/test/functional/expected/odt_basic.odt
+-rw-r--r--   0 bert      (1001) bert      (1001)     8999 2011-02-23 19:48:20.000000 docutils-0.9.1/test/functional/expected/odt_custom_headfoot.odt
+-rw-r--r--   0 bert      (1001) bert      (1001)    10848 2011-03-04 23:41:40.000000 docutils-0.9.1/test/functional/expected/odt_tables1.odt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4760 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/pep_html.html
+-rw-r--r--   0 bert      (1001) bert      (1001)    58031 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/standalone_rst_html4css1.html
+-rw-r--r--   0 bert      (1001) bert      (1001)    56446 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/expected/standalone_rst_latex.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)     2560 2012-01-20 06:50:44.000000 docutils-0.9.1/test/functional/expected/standalone_rst_manpage.man
+-rw-r--r--   0 bert      (1001) bert      (1001)    94985 2012-02-20 21:31:48.000000 docutils-0.9.1/test/functional/expected/standalone_rst_pseudoxml.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6351 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_1.html
+-rw-r--r--   0 bert      (1001) bert      (1001)     6266 2012-06-17 20:47:10.000000 docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_2.html
+-rw-r--r--   0 bert      (1001) bert      (1001)    52259 2012-03-30 11:58:21.000000 docutils-0.9.1/test/functional/expected/standalone_rst_xetex.tex
+-rw-r--r--   0 bert      (1001) bert      (1001)     1818 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/expected/xetex-cyrillic.tex
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/input/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/input/data/
+-rw-r--r--   0 bert      (1001) bert      (1001)      990 2010-11-09 22:53:56.000000 docutils-0.9.1/test/functional/input/data/custom_roles.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1505 2010-10-11 12:32:33.000000 docutils-0.9.1/test/functional/input/data/custom_roles_latex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      253 2004-06-22 21:24:21.000000 docutils-0.9.1/test/functional/input/data/errors.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       56 2005-04-07 19:36:11.000000 docutils-0.9.1/test/functional/input/data/header_footer.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6164 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/input/data/html4css1.css
+-rw-r--r--   0 bert      (1001) bert      (1001)      777 2010-02-05 14:16:25.000000 docutils-0.9.1/test/functional/input/data/hyperlinking.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     6585 2009-05-06 11:32:43.000000 docutils-0.9.1/test/functional/input/data/latex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1217 2010-05-05 12:08:10.000000 docutils-0.9.1/test/functional/input/data/latex_encoding.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      454 2005-04-05 02:55:06.000000 docutils-0.9.1/test/functional/input/data/list_table.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     4720 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/input/data/math.css
+-rw-r--r--   0 bert      (1001) bert      (1001)     3106 2011-09-17 21:03:28.000000 docutils-0.9.1/test/functional/input/data/math.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      397 2004-09-27 18:30:29.000000 docutils-0.9.1/test/functional/input/data/nonalphanumeric.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      476 2009-01-30 13:37:26.000000 docutils-0.9.1/test/functional/input/data/option_lists.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      460 2012-02-26 21:26:12.000000 docutils-0.9.1/test/functional/input/data/section_titles.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    21529 2011-09-17 21:03:28.000000 docutils-0.9.1/test/functional/input/data/standard.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1831 2010-03-02 11:51:33.000000 docutils-0.9.1/test/functional/input/data/svg_images.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      648 2011-07-25 23:50:34.000000 docutils-0.9.1/test/functional/input/data/swf_images.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      287 2004-06-22 21:24:21.000000 docutils-0.9.1/test/functional/input/data/table_colspan.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1080 2004-06-22 21:24:21.000000 docutils-0.9.1/test/functional/input/data/table_complex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      679 2005-05-25 12:01:41.000000 docutils-0.9.1/test/functional/input/data/table_rowspan.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1196 2010-12-30 23:00:58.000000 docutils-0.9.1/test/functional/input/data/tables_latex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     2355 2010-05-05 12:08:10.000000 docutils-0.9.1/test/functional/input/data/unicode.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1764 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/input/data/urls.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      893 2005-12-15 14:32:01.000000 docutils-0.9.1/test/functional/input/compact_lists.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      711 2011-08-24 13:31:05.000000 docutils-0.9.1/test/functional/input/cyrillic.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      351 2005-05-03 11:12:11.000000 docutils-0.9.1/test/functional/input/dangerous.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      198 2005-04-04 17:05:37.000000 docutils-0.9.1/test/functional/input/field_list.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      247 2005-01-15 22:03:25.000000 docutils-0.9.1/test/functional/input/latex_docinfo.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      571 2009-10-09 06:44:02.000000 docutils-0.9.1/test/functional/input/link_in_substitution.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       58 2008-12-26 22:36:46.000000 docutils-0.9.1/test/functional/input/odt_basic.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      164 2009-12-29 19:45:17.000000 docutils-0.9.1/test/functional/input/odt_custom_headfoot.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     7017 2008-12-26 22:36:46.000000 docutils-0.9.1/test/functional/input/odt_tables1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      558 2005-04-22 23:57:18.000000 docutils-0.9.1/test/functional/input/pep_html.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       13 2005-02-26 18:49:25.000000 docutils-0.9.1/test/functional/input/simple.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      741 2010-11-09 22:53:56.000000 docutils-0.9.1/test/functional/input/standalone_rst_html4css1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      915 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/input/standalone_rst_latex.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1894 2010-11-05 22:09:32.000000 docutils-0.9.1/test/functional/input/standalone_rst_manpage.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      237 2005-12-31 02:39:07.000000 docutils-0.9.1/test/functional/input/standalone_rst_pseudoxml.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     2527 2005-12-08 05:37:32.000000 docutils-0.9.1/test/functional/input/standalone_rst_s5_html.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     1501 2012-01-26 13:08:04.000000 docutils-0.9.1/test/functional/input/standalone_rst_xetex.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/output/
+-rw-r--r--   0 bert      (1001) bert      (1001)      130 2004-06-22 21:24:21.000000 docutils-0.9.1/test/functional/output/README.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/functional/tests/
+-rw-r--r--   0 bert      (1001) bert      (1001)      247 2012-01-19 22:33:02.000000 docutils-0.9.1/test/functional/tests/_default.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      198 2011-09-02 21:09:13.000000 docutils-0.9.1/test/functional/tests/_standalone_rst_defaults.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      359 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/compact_lists.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      446 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/dangerous.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      457 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/field_name_limit.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      430 2011-08-24 13:31:05.000000 docutils-0.9.1/test/functional/tests/latex_cyrillic.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      295 2005-01-14 14:34:05.000000 docutils-0.9.1/test/functional/tests/latex_docinfo.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      431 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/math_output_html.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      405 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/math_output_latex.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      412 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/math_output_mathjax.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      406 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/math_output_mathml.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      429 2012-01-19 22:33:02.000000 docutils-0.9.1/test/functional/tests/misc_rst_html4css1.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      552 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/pep_html.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      478 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/standalone_rst_html4css1.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      259 2008-07-28 08:37:32.000000 docutils-0.9.1/test/functional/tests/standalone_rst_latex.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      265 2009-08-18 18:39:39.000000 docutils-0.9.1/test/functional/tests/standalone_rst_manpage.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      372 2012-02-20 21:31:48.000000 docutils-0.9.1/test/functional/tests/standalone_rst_pseudoxml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2531 2012-06-04 20:14:08.000000 docutils-0.9.1/test/functional/tests/standalone_rst_s5_html_1.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      309 2008-07-28 08:37:32.000000 docutils-0.9.1/test/functional/tests/standalone_rst_s5_html_2.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      259 2010-09-20 21:26:33.000000 docutils-0.9.1/test/functional/tests/standalone_rst_xetex.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      465 2010-11-18 21:50:54.000000 docutils-0.9.1/test/functional/tests/xetex_cyrillic.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      167 2004-06-25 12:56:28.000000 docutils-0.9.1/test/functional/README.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/includes/
+-rw-r--r--   0 bert      (1001) bert      (1001)       75 2003-01-10 02:20:18.000000 docutils-0.9.1/test/test_parsers/test_rst/includes/include9.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/more/
+-rw-r--r--   0 bert      (1001) bert      (1001)       68 2003-01-10 02:25:51.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/more/include6.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/sibling/
+-rw-r--r--   0 bert      (1001) bert      (1001)       33 2003-01-10 02:20:18.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/sibling/include7.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       52 2002-11-19 02:37:35.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/include4.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       57 2002-11-19 02:37:35.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/includes/include5.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)        0 2005-02-22 01:26:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/empty.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       10 2005-03-15 00:37:51.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include 11.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       67 2002-10-02 03:09:55.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include1.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      952 2010-04-26 10:04:17.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include10.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      169 2007-03-12 20:25:40.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include12.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      166 2007-03-12 20:25:40.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include13.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      113 2003-07-05 19:43:13.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include2.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       52 2002-11-19 02:38:28.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include3.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       55 2003-01-10 02:20:18.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include8.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      102 2009-10-25 20:47:22.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/include_literal.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       50 2002-10-02 03:09:55.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/raw1.txt
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5054 2012-02-08 19:46:11.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_admonitions.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1580 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_block_quotes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1082 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_class.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     5434 2011-12-20 14:14:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2414 2011-12-20 14:14:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code_long.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1688 2011-11-15 07:49:01.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code_none.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2647 2011-07-06 15:52:30.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_compound.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1868 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_container.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6242 2009-04-01 20:00:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_contents.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1301 2006-07-12 21:40:56.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_date.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1847 2006-07-12 21:40:56.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_decorations.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1806 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_default_role.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7300 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_figures.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10818 2012-02-08 19:46:11.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_images.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    28755 2012-05-11 21:03:07.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_include.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2085 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_line_blocks.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1488 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_math.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6072 2006-07-12 21:40:56.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_meta.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1708 2011-07-06 15:52:30.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_parsed_literals.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4985 2012-03-19 22:59:09.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_raw.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     3908 2011-04-29 23:20:54.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_replace.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1744 2011-04-29 23:20:54.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_replace_fr.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6149 2010-09-18 10:43:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_role.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1766 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_rubrics.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1077 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_sectnum.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1905 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_sidebars.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    30924 2012-01-19 11:31:58.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_tables.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1717 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_target_notes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5883 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_test_directives.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      624 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_title.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5059 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_topics.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5423 2009-04-01 20:00:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_unicode.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2392 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_unknown.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      386 2004-09-12 21:21:50.000000 docutils-0.9.1/test/test_parsers/test_rst/test_directives/utf-16.csv
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_parsers/test_rst/__init__.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     3358 2012-01-11 20:28:57.000000 docutils-0.9.1/test/test_parsers/test_rst/test_SimpleTableParser.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6099 2012-01-11 20:28:57.000000 docutils-0.9.1/test/test_parsers/test_rst/test_TableParser.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6665 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_block_quotes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     3903 2006-06-04 21:38:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_bullet_lists.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4231 2008-02-15 09:23:07.000000 docutils-0.9.1/test/test_parsers/test_rst/test_citations.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6595 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_comments.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    11375 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_definition_lists.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1388 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_doctest_blocks.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     9370 2012-01-11 20:28:57.000000 docutils-0.9.1/test/test_parsers/test_rst/test_east_asian_text.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    20470 2007-03-21 19:51:22.000000 docutils-0.9.1/test/test_parsers/test_rst/test_enumerated_lists.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    13445 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_field_lists.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     9448 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_footnotes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1041 2012-02-03 08:16:53.000000 docutils-0.9.1/test/test_parsers/test_rst/test_functions.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    41730 2011-12-05 19:35:32.000000 docutils-0.9.1/test/test_parsers/test_rst/test_inline_markup.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10216 2011-12-20 14:14:21.000000 docutils-0.9.1/test/test_parsers/test_rst/test_interpreted.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1316 2011-04-25 23:07:32.000000 docutils-0.9.1/test/test_parsers/test_rst/test_interpreted_fr.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7057 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_line_blocks.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6929 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_literal_blocks.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    20371 2011-09-17 18:00:35.000000 docutils-0.9.1/test/test_parsers/test_rst/test_option_lists.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2001 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_outdenting.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1329 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_paragraphs.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    20420 2010-11-10 13:43:50.000000 docutils-0.9.1/test/test_parsers/test_rst/test_section_headers.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     8883 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_substitutions.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    37488 2012-01-11 20:28:57.000000 docutils-0.9.1/test/test_parsers/test_rst/test_tables.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    13765 2011-06-30 22:14:29.000000 docutils-0.9.1/test/test_parsers/test_rst/test_targets.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5276 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_parsers/test_rst/test_transitions.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_parsers/__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1214 2009-04-01 20:00:21.000000 docutils-0.9.1/test/test_parsers/test_parser.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_readers/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_readers/test_pep/
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_readers/test_pep/__init__.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     3252 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_readers/test_pep/test_inline_markup.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6073 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_readers/test_pep/test_rfc2822.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_readers/__init__.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_transforms/
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_transforms/__init__.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1136 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_transforms/test___init__.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4087 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_class.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10659 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_contents.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     9313 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_docinfo.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4784 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_doctitle.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      988 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_transforms/test_expose_internals.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      908 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_filter.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    15793 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_footnotes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    23349 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_hyperlinks.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1858 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_messages.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1698 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_peps.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     9336 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_sectnum.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      948 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_strip_comments.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10096 2010-07-03 14:19:09.000000 docutils-0.9.1/test/test_transforms/test_substitutions.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2301 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_target_notes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7537 2006-05-21 20:44:42.000000 docutils-0.9.1/test/test_transforms/test_transitions.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1705 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_transforms/test_writer_aux.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/test/test_writers/
+-rw-r--r--   0 bert      (1001) bert      (1001)      306 2005-06-17 22:24:13.000000 docutils-0.9.1/test/test_writers/__init__.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5871 2012-01-18 10:16:20.000000 docutils-0.9.1/test/test_writers/test_docutils_xml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1088 2012-01-19 22:33:02.000000 docutils-0.9.1/test/test_writers/test_html4css1_misc.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10449 2010-12-13 22:06:48.000000 docutils-0.9.1/test/test_writers/test_html4css1_parts.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4984 2012-06-04 20:14:08.000000 docutils-0.9.1/test/test_writers/test_html4css1_template.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    12141 2012-01-26 13:08:04.000000 docutils-0.9.1/test/test_writers/test_latex2e.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     4674 2012-01-20 06:50:44.000000 docutils-0.9.1/test/test_writers/test_manpage.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      528 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_writers/test_null.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6437 2012-02-03 08:16:53.000000 docutils-0.9.1/test/test_writers/test_odt.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      898 2007-05-31 00:01:52.000000 docutils-0.9.1/test/test_writers/test_pseudoxml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     4342 2012-06-04 20:14:08.000000 docutils-0.9.1/test/test_writers/test_s5.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    32313 2012-06-13 14:14:12.000000 docutils-0.9.1/test/DocutilsTestSupport.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2842 2012-05-11 21:03:07.000000 docutils-0.9.1/test/alltests.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1306 2008-03-30 09:05:39.000000 docutils-0.9.1/test/coverage.sh
+-rw-r--r--   0 bert      (1001) bert      (1001)      382 2004-06-25 22:12:37.000000 docutils-0.9.1/test/docutils.conf
+-rw-r--r--   0 bert      (1001) bert      (1001)     5347 2012-01-19 22:33:02.000000 docutils-0.9.1/test/package_unittest.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      763 2012-02-03 08:16:53.000000 docutils-0.9.1/test/test__init__.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     1495 2011-12-05 21:20:43.000000 docutils-0.9.1/test/test_command_line.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     5352 2012-06-04 20:14:08.000000 docutils-0.9.1/test/test_dependencies.py
+-rw-r--r--   0 bert      (1001) bert      (1001)    12491 2012-06-13 14:14:12.000000 docutils-0.9.1/test/test_error_reporting.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     8279 2012-02-03 08:16:53.000000 docutils-0.9.1/test/test_functional.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7049 2012-06-13 14:14:12.000000 docutils-0.9.1/test/test_io.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7886 2010-09-28 08:21:25.000000 docutils-0.9.1/test/test_language.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    24938 2012-05-01 08:34:41.000000 docutils-0.9.1/test/test_nodes.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      772 2012-02-03 08:16:53.000000 docutils-0.9.1/test/test_pickle.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6172 2012-03-19 22:59:09.000000 docutils-0.9.1/test/test_publisher.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7965 2012-05-01 08:34:41.000000 docutils-0.9.1/test/test_settings.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    10992 2012-05-01 08:34:41.000000 docutils-0.9.1/test/test_statemachine.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2200 2012-05-01 08:34:41.000000 docutils-0.9.1/test/test_traversals.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)    11491 2012-02-03 12:22:14.000000 docutils-0.9.1/test/test_utils.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     7262 2012-05-01 08:34:41.000000 docutils-0.9.1/test/test_viewlist.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/dev/
+-rw-r--r--   0 bert      (1001) bert      (1001)       22 2005-06-15 23:54:52.000000 docutils-0.9.1/tools/dev/README.txt
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     2793 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/dev/create_unimap.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      926 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/dev/profile_docutils.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6726 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/dev/unicode2rstsubs.py
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/editors/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/editors/emacs/
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/editors/emacs/tests/
+-rw-r--r--   0 bert      (1001) bert      (1001)      618 2012-06-16 09:41:40.000000 docutils-0.9.1/tools/editors/emacs/tests/Makefile
+-rw-r--r--   0 bert      (1001) bert      (1001)      566 2010-12-12 18:32:18.000000 docutils-0.9.1/tools/editors/emacs/tests/README.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     9192 2010-12-22 19:50:48.000000 docutils-0.9.1/tools/editors/emacs/tests/adjust-section.el
+-rw-r--r--   0 bert      (1001) bert      (1001)    13397 2011-01-23 12:38:49.000000 docutils-0.9.1/tools/editors/emacs/tests/adornment.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     3282 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/comment.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     9290 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/ert-support.el
+-rw-r--r--   0 bert      (1001) bert      (1001)    10305 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/fill.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     3117 2012-04-29 14:50:25.000000 docutils-0.9.1/tools/editors/emacs/tests/font-lock.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     4853 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/indent.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     4273 2010-12-12 18:32:18.000000 docutils-0.9.1/tools/editors/emacs/tests/items.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     3665 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/movement.el
+-rw-r--r--   0 bert      (1001) bert      (1001)    32235 2012-06-16 09:41:40.000000 docutils-0.9.1/tools/editors/emacs/tests/re.el
+-rw-r--r--   0 bert      (1001) bert      (1001)    11853 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/shift.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     3689 2011-03-20 17:20:36.000000 docutils-0.9.1/tools/editors/emacs/tests/support.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     3335 2010-12-12 18:32:18.000000 docutils-0.9.1/tools/editors/emacs/tests/toc.el
+-rw-r--r--   0 bert      (1001) bert      (1001)     7993 2012-06-16 09:41:40.000000 docutils-0.9.1/tools/editors/emacs/IDEAS.rst
+-rw-r--r--   0 bert      (1001) bert      (1001)     1097 2008-11-26 18:07:47.000000 docutils-0.9.1/tools/editors/emacs/README.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)       34 2005-03-15 00:43:13.000000 docutils-0.9.1/tools/editors/emacs/docutils.conf
+-rw-r--r--   0 bert      (1001) bert      (1001)   149461 2012-06-16 09:41:40.000000 docutils-0.9.1/tools/editors/emacs/rst.el
+-rw-r--r--   0 bert      (1001) bert      (1001)      873 2006-08-14 16:08:29.000000 docutils-0.9.1/tools/editors/README.txt
+drwxr-xr-x   0 bert      (1001) bert      (1001)        0 2012-06-17 22:07:19.000000 docutils-0.9.1/tools/test/
+-rw-r--r--   0 bert      (1001) bert      (1001)     3458 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/test/test_buildhtml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     9956 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/buildhtml.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      327 2005-12-12 00:05:55.000000 docutils-0.9.1/tools/docutils.conf
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     6858 2012-06-13 23:27:03.000000 docutils-0.9.1/tools/quicktest.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      597 2006-05-21 20:44:42.000000 docutils-0.9.1/tools/rst2html.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      794 2009-04-16 12:04:49.000000 docutils-0.9.1/tools/rst2latex.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      603 2009-08-18 18:39:39.000000 docutils-0.9.1/tools/rst2man.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      767 2009-01-07 19:09:28.000000 docutils-0.9.1/tools/rst2odt.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     1701 2009-01-07 19:09:28.000000 docutils-0.9.1/tools/rst2odt_prepstyles.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      604 2006-05-21 20:44:42.000000 docutils-0.9.1/tools/rst2pseudoxml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      640 2006-05-21 20:44:42.000000 docutils-0.9.1/tools/rst2s5.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      789 2011-05-19 09:12:02.000000 docutils-0.9.1/tools/rst2xetex.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      605 2006-05-21 20:44:42.000000 docutils-0.9.1/tools/rst2xml.py
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      673 2006-05-21 20:44:42.000000 docutils-0.9.1/tools/rstpep2html.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     9629 2012-01-04 14:20:52.000000 docutils-0.9.1/BUGS.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     5056 2011-12-31 14:22:16.000000 docutils-0.9.1/COPYING.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    48256 2012-02-16 17:15:55.000000 docutils-0.9.1/FAQ.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)   104806 2012-06-17 20:47:44.000000 docutils-0.9.1/HISTORY.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)      293 2010-03-05 09:34:44.000000 docutils-0.9.1/MANIFEST.in
+-rw-r--r--   0 bert      (1001) bert      (1001)    11646 2012-06-13 23:27:03.000000 docutils-0.9.1/README.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)    13653 2012-06-17 22:05:00.000000 docutils-0.9.1/RELEASE-NOTES.txt
+-rw-r--r--   0 bert      (1001) bert      (1001)     3174 2008-08-25 13:07:53.000000 docutils-0.9.1/THANKS.txt
+-rwxr-xr-x   0 bert      (1001) bert      (1001)      685 2004-07-13 15:57:13.000000 docutils-0.9.1/install.py
+-rw-r--r--   0 bert      (1001) bert      (1001)      336 2012-06-13 23:27:03.000000 docutils-0.9.1/setup.cfg
+-rwxr-xr-x   0 bert      (1001) bert      (1001)     8391 2012-06-17 20:47:10.000000 docutils-0.9.1/setup.py
+-rw-r--r--   0 bert      (1001) bert      (1001)     2181 2012-06-17 22:07:19.000000 docutils-0.9.1/PKG-INFO
```

### Comparing `docutils-0.9/docs/api/cmdline-tool.txt` & `docutils-0.9.1/docs/api/cmdline-tool.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/api/publisher.txt` & `docutils-0.9.1/docs/api/publisher.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/api/runtime-settings.txt` & `docutils-0.9.1/docs/api/runtime-settings.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/rst/alternatives.txt` & `docutils-0.9.1/docs/dev/rst/alternatives.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/rst/problems.txt` & `docutils-0.9.1/docs/dev/rst/problems.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/distributing.txt` & `docutils-0.9.1/docs/dev/distributing.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/enthought-plan.txt` & `docutils-0.9.1/docs/dev/enthought-plan.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/enthought-rfp.txt` & `docutils-0.9.1/docs/dev/enthought-rfp.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/hacking.txt` & `docutils-0.9.1/docs/dev/hacking.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/policies.txt` & `docutils-0.9.1/docs/dev/policies.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/pysource.dtd` & `docutils-0.9.1/docs/dev/pysource.dtd`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/pysource.txt` & `docutils-0.9.1/docs/dev/pysource.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/release.txt` & `docutils-0.9.1/docs/dev/release.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/repository.txt` & `docutils-0.9.1/docs/dev/repository.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/semantics.txt` & `docutils-0.9.1/docs/dev/semantics.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/testing.txt` & `docutils-0.9.1/docs/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/todo.txt` & `docutils-0.9.1/docs/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/dev/website.txt` & `docutils-0.9.1/docs/dev/website.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/howto/html-stylesheets.txt` & `docutils-0.9.1/docs/howto/html-stylesheets.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/howto/i18n.txt` & `docutils-0.9.1/docs/howto/i18n.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/howto/rst-directives.txt` & `docutils-0.9.1/docs/howto/rst-directives.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/howto/rst-roles.txt` & `docutils-0.9.1/docs/howto/rst-roles.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/howto/security.txt` & `docutils-0.9.1/docs/howto/security.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/peps/pep-0256.txt` & `docutils-0.9.1/docs/peps/pep-0256.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/peps/pep-0257.txt` & `docutils-0.9.1/docs/peps/pep-0257.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/peps/pep-0258.txt` & `docutils-0.9.1/docs/peps/pep-0258.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/peps/pep-0287.txt` & `docutils-0.9.1/docs/peps/pep-0287.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/rst/definitions.txt` & `docutils-0.9.1/docs/ref/rst/definitions.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/rst/directives.txt` & `docutils-0.9.1/docs/ref/rst/directives.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/rst/introduction.txt` & `docutils-0.9.1/docs/ref/rst/introduction.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/rst/restructuredtext.txt` & `docutils-0.9.1/docs/ref/rst/restructuredtext.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/rst/roles.txt` & `docutils-0.9.1/docs/ref/rst/roles.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/doctree.txt` & `docutils-0.9.1/docs/ref/doctree.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/docutils.dtd` & `docutils-0.9.1/docs/ref/docutils.dtd`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/soextblx.dtd` & `docutils-0.9.1/docs/ref/soextblx.dtd`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/ref/transforms.txt` & `docutils-0.9.1/docs/ref/transforms.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/big-black.png` & `docutils-0.9.1/docs/user/images/big-black.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/big-white.png` & `docutils-0.9.1/docs/user/images/big-white.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/default.png` & `docutils-0.9.1/docs/user/images/default.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/happy_monkey.png` & `docutils-0.9.1/docs/user/images/happy_monkey.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/medium-black.png` & `docutils-0.9.1/docs/user/images/medium-black.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/medium-white.png` & `docutils-0.9.1/docs/user/images/medium-white.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-all.png` & `docutils-0.9.1/docs/user/images/rsp-all.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-breaks.png` & `docutils-0.9.1/docs/user/images/rsp-breaks.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-covers.png` & `docutils-0.9.1/docs/user/images/rsp-covers.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-cuts.png` & `docutils-0.9.1/docs/user/images/rsp-cuts.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-empty.png` & `docutils-0.9.1/docs/user/images/rsp-empty.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp-objects.png` & `docutils-0.9.1/docs/user/images/rsp-objects.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/rsp.svg` & `docutils-0.9.1/docs/user/images/rsp.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/s5-files.png` & `docutils-0.9.1/docs/user/images/s5-files.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/s5-files.svg` & `docutils-0.9.1/docs/user/images/s5-files.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/small-black.png` & `docutils-0.9.1/docs/user/images/small-black.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/images/small-white.png` & `docutils-0.9.1/docs/user/images/small-white.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/ball1.gif` & `docutils-0.9.1/docs/user/rst/images/ball1.gif`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/biohazard-scaling.svg` & `docutils-0.9.1/docs/user/rst/images/biohazard-scaling.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/biohazard.svg` & `docutils-0.9.1/docs/user/rst/images/biohazard.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/biohazard.swf` & `docutils-0.9.1/docs/user/rst/images/biohazard.swf`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/title-scaling.svg` & `docutils-0.9.1/docs/user/rst/images/title-scaling.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/title.png` & `docutils-0.9.1/docs/user/rst/images/title.png`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/images/title.svg` & `docutils-0.9.1/docs/user/rst/images/title.svg`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/cheatsheet.txt` & `docutils-0.9.1/docs/user/rst/cheatsheet.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/demo.txt` & `docutils-0.9.1/docs/user/rst/demo.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/quickref.html` & `docutils-0.9.1/docs/user/rst/quickref.html`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/rst/quickstart.txt` & `docutils-0.9.1/docs/user/rst/quickstart.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/config.txt` & `docutils-0.9.1/docs/user/config.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/docutils-05-compat.sty.txt` & `docutils-0.9.1/docs/user/docutils-05-compat.sty.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/emacs.txt` & `docutils-0.9.1/docs/user/emacs.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/latex.txt` & `docutils-0.9.1/docs/user/latex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/links.txt` & `docutils-0.9.1/docs/user/links.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/mailing-lists.txt` & `docutils-0.9.1/docs/user/mailing-lists.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/manpage.txt` & `docutils-0.9.1/docs/user/manpage.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/odt.txt` & `docutils-0.9.1/docs/user/odt.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/slide-shows.txt` & `docutils-0.9.1/docs/user/slide-shows.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/user/tools.txt` & `docutils-0.9.1/docs/user/tools.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docs/index.txt` & `docutils-0.9.1/docs/index.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/__init__.py` & `docutils-0.9.1/docutils/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/af.py` & `docutils-0.9.1/docutils/languages/af.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/ca.py` & `docutils-0.9.1/docutils/languages/ca.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/cs.py` & `docutils-0.9.1/docutils/languages/cs.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/de.py` & `docutils-0.9.1/docutils/languages/de.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/en.py` & `docutils-0.9.1/docutils/languages/en.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/eo.py` & `docutils-0.9.1/docutils/languages/eo.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/es.py` & `docutils-0.9.1/docutils/languages/es.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/fi.py` & `docutils-0.9.1/docutils/languages/fi.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/fr.py` & `docutils-0.9.1/docutils/languages/fr.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/gl.py` & `docutils-0.9.1/docutils/languages/gl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/he.py` & `docutils-0.9.1/docutils/languages/he.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/it.py` & `docutils-0.9.1/docutils/languages/it.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/ja.py` & `docutils-0.9.1/docutils/languages/ja.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/lt.py` & `docutils-0.9.1/docutils/languages/lt.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/nl.py` & `docutils-0.9.1/docutils/languages/nl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/pl.py` & `docutils-0.9.1/docutils/languages/pl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/pt_br.py` & `docutils-0.9.1/docutils/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/ru.py` & `docutils-0.9.1/docutils/languages/ru.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/sk.py` & `docutils-0.9.1/docutils/languages/sk.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/sv.py` & `docutils-0.9.1/docutils/languages/sv.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/zh_cn.py` & `docutils-0.9.1/docutils/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/languages/zh_tw.py` & `docutils-0.9.1/docutils/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/math/__init__.py` & `docutils-0.9.1/docutils/math/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/math/latex2mathml.py` & `docutils-0.9.1/docutils/math/latex2mathml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/math/math2html.py` & `docutils-0.9.1/docutils/math/math2html.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,16 @@
   def fatal(cls, message):
     "Show an error message and terminate"
     Trace.error('FATAL: ' + message)
     exit(-1)
 
   def show(cls, message, channel):
     "Show a message out of a channel"
-    message = message.encode('utf-8')
+    if sys.version_info < (3,0):
+      message = message.encode('utf-8')
     channel.write(message + '\n')
 
   debug = classmethod(debug)
   message = classmethod(message)
   error = classmethod(error)
   fatal = classmethod(fatal)
   show = classmethod(show)
@@ -1697,15 +1698,15 @@
         return
       self.writestring(string)
 
   def writestring(self, string):
     "Write a string"
     if not self.file:
       self.file = codecs.open(self.filename, 'w', "utf-8")
-    if self.file == sys.stdout:
+    if self.file == sys.stdout and sys.version_info < (3,0):
       string = string.encode('utf-8')
     self.file.write(string)
 
   def writeline(self, line):
     "Write a line to file"
     self.writestring(line + '\n')
```

### Comparing `docutils-0.9/docutils/math/tex2unichar.py` & `docutils-0.9.1/docutils/math/tex2unichar.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/math/unichar2tex.py` & `docutils-0.9.1/docutils/math/unichar2tex.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/__init__.py` & `docutils-0.9.1/docutils/parsers/rst/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/admonitions.py` & `docutils-0.9.1/docutils/parsers/rst/directives/admonitions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/body.py` & `docutils-0.9.1/docutils/parsers/rst/directives/body.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/html.py` & `docutils-0.9.1/docutils/parsers/rst/directives/html.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/images.py` & `docutils-0.9.1/docutils/parsers/rst/directives/images.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/misc.py` & `docutils-0.9.1/docutils/parsers/rst/directives/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# $Id: misc.py 7328 2012-01-27 08:41:35Z milde $
+# $Id: misc.py 7433 2012-05-11 21:03:07Z milde $
 # Authors: David Goodger <goodger@python.org>; Dethe Elza
 # Copyright: This module has been placed in the public domain.
 
 """Miscellaneous directives."""
 
 __docformat__ = 'reStructuredText'
 
@@ -69,14 +69,19 @@
         try:
             self.state.document.settings.record_dependencies.add(path)
             include_file = io.FileInput(
                 source_path=path, encoding=encoding,
                 error_handler=(self.state.document.settings.\
                                input_encoding_error_handler),
                 handle_io_errors=None)
+        except UnicodeEncodeError, error:
+            raise self.severe(u'Problems with "%s" directive path:\n'
+                              'Cannot encode input file path "%s" '
+                              '(wrong locale?).' %
+                              (self.name, SafeString(path)))
         except IOError, error:
             raise self.severe(u'Problems with "%s" directive path:\n%s.' %
                       (self.name, ErrorString(error)))
         startline = self.options.get('start-line', None)
         endline = self.options.get('end-line', None)
         try:
             if startline or (endline is not None):
```

### Comparing `docutils-0.9/docutils/parsers/rst/directives/parts.py` & `docutils-0.9.1/docutils/parsers/rst/directives/parts.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/references.py` & `docutils-0.9.1/docutils/parsers/rst/directives/references.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/directives/tables.py` & `docutils-0.9.1/docutils/parsers/rst/directives/tables.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/README.txt` & `docutils-0.9.1/docutils/parsers/rst/include/README.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamsa.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamsa.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamsb.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamsb.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamsc.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamsc.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamsn.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamsn.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamso.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamso.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isoamsr.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isoamsr.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isobox.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isobox.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isocyr1.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isocyr1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isocyr2.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isocyr2.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isodia.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isodia.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isogrk1.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isogrk1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isogrk2.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isogrk2.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isogrk3.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isogrk3.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isogrk4-wide.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isogrk4-wide.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isolat1.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isolat1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isolat2.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isolat2.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomfrk-wide.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomfrk-wide.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomfrk.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomfrk.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomopf-wide.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomopf-wide.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomopf.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomopf.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomscr-wide.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomscr-wide.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isomscr.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isomscr.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isonum.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isonum.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isopub.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isopub.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/isotech.txt` & `docutils-0.9.1/docutils/parsers/rst/include/isotech.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/mmlalias.txt` & `docutils-0.9.1/docutils/parsers/rst/include/mmlalias.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/mmlextra-wide.txt` & `docutils-0.9.1/docutils/parsers/rst/include/mmlextra-wide.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/mmlextra.txt` & `docutils-0.9.1/docutils/parsers/rst/include/mmlextra.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/s5defs.txt` & `docutils-0.9.1/docutils/parsers/rst/include/s5defs.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/xhtml1-lat1.txt` & `docutils-0.9.1/docutils/parsers/rst/include/xhtml1-lat1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/xhtml1-special.txt` & `docutils-0.9.1/docutils/parsers/rst/include/xhtml1-special.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/include/xhtml1-symbol.txt` & `docutils-0.9.1/docutils/parsers/rst/include/xhtml1-symbol.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/__init__.py` & `docutils-0.9.1/docutils/parsers/rst/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/af.py` & `docutils-0.9.1/docutils/parsers/rst/languages/af.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/ca.py` & `docutils-0.9.1/docutils/parsers/rst/languages/ca.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/cs.py` & `docutils-0.9.1/docutils/parsers/rst/languages/cs.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/de.py` & `docutils-0.9.1/docutils/parsers/rst/languages/de.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/en.py` & `docutils-0.9.1/docutils/parsers/rst/languages/en.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/eo.py` & `docutils-0.9.1/docutils/parsers/rst/languages/eo.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/es.py` & `docutils-0.9.1/docutils/parsers/rst/languages/es.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/fi.py` & `docutils-0.9.1/docutils/parsers/rst/languages/fi.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/fr.py` & `docutils-0.9.1/docutils/parsers/rst/languages/fr.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/gl.py` & `docutils-0.9.1/docutils/parsers/rst/languages/gl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/he.py` & `docutils-0.9.1/docutils/parsers/rst/languages/he.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/it.py` & `docutils-0.9.1/docutils/parsers/rst/languages/it.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/ja.py` & `docutils-0.9.1/docutils/parsers/rst/languages/ja.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/lt.py` & `docutils-0.9.1/docutils/parsers/rst/languages/lt.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/nl.py` & `docutils-0.9.1/docutils/parsers/rst/languages/nl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/pl.py` & `docutils-0.9.1/docutils/parsers/rst/languages/pl.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/pt_br.py` & `docutils-0.9.1/docutils/parsers/rst/languages/pt_br.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/ru.py` & `docutils-0.9.1/docutils/parsers/rst/languages/ru.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/sk.py` & `docutils-0.9.1/docutils/parsers/rst/languages/sk.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/sv.py` & `docutils-0.9.1/docutils/parsers/rst/languages/sv.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/zh_cn.py` & `docutils-0.9.1/docutils/parsers/rst/languages/zh_cn.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/languages/zh_tw.py` & `docutils-0.9.1/docutils/parsers/rst/languages/zh_tw.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/__init__.py` & `docutils-0.9.1/docutils/parsers/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/roles.py` & `docutils-0.9.1/docutils/parsers/rst/roles.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/states.py` & `docutils-0.9.1/docutils/parsers/rst/states.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/rst/tableparser.py` & `docutils-0.9.1/docutils/parsers/rst/tableparser.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/parsers/__init__.py` & `docutils-0.9.1/docutils/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/readers/__init__.py` & `docutils-0.9.1/docutils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/readers/doctree.py` & `docutils-0.9.1/docutils/readers/doctree.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/readers/pep.py` & `docutils-0.9.1/docutils/readers/pep.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/readers/standalone.py` & `docutils-0.9.1/docutils/readers/standalone.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/__init__.py` & `docutils-0.9.1/docutils/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/components.py` & `docutils-0.9.1/docutils/transforms/components.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/frontmatter.py` & `docutils-0.9.1/docutils/transforms/frontmatter.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/misc.py` & `docutils-0.9.1/docutils/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/parts.py` & `docutils-0.9.1/docutils/transforms/parts.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/peps.py` & `docutils-0.9.1/docutils/transforms/peps.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/references.py` & `docutils-0.9.1/docutils/transforms/references.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/universal.py` & `docutils-0.9.1/docutils/transforms/universal.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/transforms/writer_aux.py` & `docutils-0.9.1/docutils/transforms/writer_aux.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/utils/__init__.py` & `docutils-0.9.1/docutils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/utils/code_analyzer.py` & `docutils-0.9.1/docutils/utils/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/utils/punctuation_chars.py` & `docutils-0.9.1/docutils/utils/punctuation_chars.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/utils/roman.py` & `docutils-0.9.1/docutils/utils/roman.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/html4css1/__init__.py` & `docutils-0.9.1/docutils/writers/html4css1/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/html4css1/html4css1.css` & `docutils-0.9.1/test/functional/input/data/html4css1.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 :Author: David Goodger (goodger@python.org)
-:Id: $Id: html4css1.css 7056 2011-06-17 10:50:48Z milde $
+:Id: $Id: html4css1.css 7437 2012-06-04 20:14:08Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
 
 See http://docutils.sf.net/docs/howto/html-stylesheets.html for how to
 customize this style sheet.
 */
@@ -236,18 +236,26 @@
   font-weight: bold }
 
 pre.address {
   margin-bottom: 0 ;
   margin-top: 0 ;
   font: inherit }
 
-pre.literal-block, pre.doctest-block, pre.math {
+pre.literal-block, pre.doctest-block, pre.math, pre.code {
   margin-left: 2em ;
   margin-right: 2em }
 
+pre.code .ln { /* line numbers */
+  color: grey;
+}
+
+.code {
+  background-color: #eeeeee
+}
+
 span.classifier {
   font-family: sans-serif ;
   font-style: oblique }
 
 span.classifier-delimiter {
   font-family: sans-serif ;
   font-weight: bold }
```

### Comparing `docutils-0.9/docutils/writers/html4css1/math.css` & `docutils-0.9.1/docutils/writers/html4css1/math.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/latex2e/__init__.py` & `docutils-0.9.1/docutils/writers/latex2e/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/latex2e/docutils-05-compat.sty` & `docutils-0.9.1/docutils/writers/latex2e/docutils-05-compat.sty`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/latex2e/titlepage.tex` & `docutils-0.9.1/docutils/writers/latex2e/titlepage.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/latex2e/xelatex.tex` & `docutils-0.9.1/docutils/writers/latex2e/xelatex.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/odf_odt/__init__.py` & `docutils-0.9.1/docutils/writers/odf_odt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# $Id: __init__.py 7385 2012-03-20 00:22:38Z dkuhlman $
+# $Id: __init__.py 7422 2012-05-03 10:55:30Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 Open Document Format (ODF) Writer.
 
 """
@@ -60,20 +60,23 @@
     import pygments
     import pygments.lexers
     from pygmentsformatter import OdtPygmentsProgFormatter, \
         OdtPygmentsLaTeXFormatter
 except ImportError, exp:
     pygments = None
 
-#
-# Is the PIL imaging library installed?
-try:
-    import Image
-except ImportError, exp:
-    Image = None
+try: # check for the Python Imaging Library
+    import PIL
+except ImportError:
+    try:  # sometimes PIL modules are put in PYTHONPATH's root
+        import Image
+        class PIL(object): pass  # dummy wrapper
+        PIL.Image = Image
+    except ImportError:
+        PIL = None
 
 ## import warnings
 ## warnings.warn('importing IPShellEmbed', UserWarning)
 ## from IPython.Shell import IPShellEmbed
 ## args = ['-pdb', '-pi1', 'In <\\#>: ', '-pi2', '   .\\D.: ',
 ##         '-po', 'Out<\\#>: ', '-nosep']
 ## ipshell = IPShellEmbed(args,
@@ -2119,17 +2122,17 @@
 
     def get_image_scaled_width_height(self, node, source):
         scale = self.get_image_scale(node)
         width = self.get_image_width_height(node, 'width')
         height = self.get_image_width_height(node, 'height')
 
         dpi = (72, 72)
-        if Image is not None and source in self.image_dict:
+        if PIL is not None and source in self.image_dict:
             filename, destination = self.image_dict[source]
-            imageobj = Image.open(filename, 'r')
+            imageobj = PIL.Image.open(filename, 'r')
             dpi = imageobj.info.get('dpi', dpi)
             # dpi information can be (xdpi, ydpi) or xydpi
             try: iter(dpi)
             except: dpi = (dpi, dpi)
         else:
             imageobj = None
```

### Comparing `docutils-0.9/docutils/writers/odf_odt/pygmentsformatter.py` & `docutils-0.9.1/docutils/writers/odf_odt/pygmentsformatter.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/odf_odt/styles.odt` & `docutils-0.9.1/docutils/writers/odf_odt/styles.odt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/pep_html/__init__.py` & `docutils-0.9.1/docutils/writers/pep_html/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/pep_html/pep.css` & `docutils-0.9.1/docutils/writers/pep_html/pep.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/pep_html/template.txt` & `docutils-0.9.1/docutils/writers/pep_html/template.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/big-black/framing.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/big-black/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/big-black/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/big-black/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/big-white/framing.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/big-white/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/big-white/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/big-white/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/framing.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/iepngfix.htc` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/outline.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/outline.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/print.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/print.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/default/slides.js` & `docutils-0.9.1/docutils/writers/s5_html/themes/default/slides.js`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/medium-black/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/medium-black/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/medium-white/framing.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/medium-white/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/medium-white/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/medium-white/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/small-black/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/small-black/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/small-white/framing.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/small-white/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/themes/small-white/pretty.css` & `docutils-0.9.1/docutils/writers/s5_html/themes/small-white/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/s5_html/__init__.py` & `docutils-0.9.1/docutils/writers/s5_html/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/xetex/__init__.py` & `docutils-0.9.1/docutils/writers/xetex/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/__init__.py` & `docutils-0.9.1/docutils/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/docutils_xml.py` & `docutils-0.9.1/docutils/writers/docutils_xml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/manpage.py` & `docutils-0.9.1/docutils/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/writers/pseudoxml.py` & `docutils-0.9.1/docutils/writers/pseudoxml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/__init__.py` & `docutils-0.9.1/docutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# $Id: __init__.py 7409 2012-05-02 17:06:37Z grubert $
+# $Id: __init__.py 7446 2012-06-17 20:47:10Z grubert $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 This is the Docutils (Python Documentation Utilities) package.
 
 Package Structure
@@ -45,15 +45,15 @@
   utilities used by readers, writers, and transforms.
 
 - writers: Format-specific output translators.
 """
 
 __docformat__ = 'reStructuredText'
 
-__version__ = '0.9'
+__version__ = '0.9.1'
 """``major.minor.micro`` version number.  The micro number is bumped for API
 changes, for new functionality, and for interim project releases.  The minor
 number is bumped whenever there is a significant project release.  The major
 number will be bumped when the project is feature-complete, and perhaps if
 there is a major change in the design."""
 
 __version_details__ = 'release'
```

### Comparing `docutils-0.9/docutils/_compat.py` & `docutils-0.9.1/docutils/_compat.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/_string_template_compat.py` & `docutils-0.9.1/docutils/_string_template_compat.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/core.py` & `docutils-0.9.1/docutils/core.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/error_reporting.py` & `docutils-0.9.1/docutils/error_reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 
-# :Id: $Id: error_reporting.py 7316 2012-01-19 11:31:58Z milde $
+# :Id: $Id: error_reporting.py 7423 2012-05-03 11:01:54Z milde $
 # :Copyright: © 2011 Günter Milde.
 # :License: Released under the terms of the `2-Clause BSD license`_, in short:
 #
 #    Copying and distribution of this file, with or without modification,
 #    are permitted in any medium without royalty provided the copyright
 #    notice and this notice are preserved.
 #    This file is offered as-is, without any warranty.
@@ -136,19 +136,18 @@
     """
 
     def __init__(self, stream=None, encoding=None,
                  encoding_errors='backslashreplace',
                  decoding_errors='replace'):
         """
         :Parameters:
-            - `stream`: a file-like object (which is written to),
-                        a string (opended as a file),
-                        `None` (bind to `sys.stderr`; default).
-                        If evaluating to `False` (but not `None`),
-                        write() requests are ignored.
+            - `stream`: a file-like object,
+                        a string (path to a file),
+                        `None` (write to `sys.stderr`, default), or
+                        evaluating to `False` (write() requests are ignored).
             - `encoding`: `stream` text encoding. Guessed if None.
             - `encoding_errors`: how to treat encoding errors.
         """
         if stream is None:
             stream = sys.stderr
         elif not(stream):
             stream = False
```

### Comparing `docutils-0.9/docutils/examples.py` & `docutils-0.9.1/docutils/examples.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/frontend.py` & `docutils-0.9.1/docutils/frontend.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/io.py` & `docutils-0.9.1/docutils/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# $Id: io.py 7384 2012-03-19 22:59:09Z milde $
+# $Id: io.py 7440 2012-06-13 14:14:12Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 I/O classes provide a uniform API for low-level input and output.  Subclasses
 will exist for a variety of input/output mechanisms.
 """
@@ -17,14 +17,29 @@
 from docutils._compat import b
 from docutils.error_reporting import locale_encoding, ErrorString, ErrorOutput
 
 
 class InputError(IOError): pass
 class OutputError(IOError): pass
 
+def check_encoding(stream, encoding):
+    """Test, whether the encoding of `stream` matches `encoding`.
+
+    Returns
+
+    :None:  if `encoding` or `stream.encoding` are not a valid encoding
+            argument (e.g. ``None``) or `stream.encoding is missing.
+    :True:  if the encoding argument resolves to the same value as `encoding`,
+    :False: if the encodings differ.
+    """
+    try:
+        return codecs.lookup(stream.encoding) == codecs.lookup(encoding)
+    except (LookupError, AttributeError, TypeError):
+        return None
+
 
 class Input(TransformSpec):
 
     """
     Abstract base class for input wrappers.
     """
 
@@ -227,18 +242,15 @@
                             u'Unable to open source file for reading ("%s").'
                             u'Exiting.' % source_path)
                         sys.exit(1)
                     raise InputError(error.errno, error.strerror, source_path)
             else:
                 self.source = sys.stdin
         elif (sys.version_info >= (3,0) and
-              self.encoding and hasattr(self.source, 'encoding') and
-              self.encoding != self.source.encoding and
-              codecs.lookup(self.encoding) !=
-              codecs.lookup(self.source.encoding)):
+              check_encoding(self.source, self.encoding) is False):
             # TODO: re-open, warn or raise error?
             raise UnicodeError('Encoding clash: encoding given is "%s" '
                                'but source is opened with encoding "%s".' %
                                (self.encoding, self.source.encoding))
         if not source_path:
             try:
                 self.source_path = self.source.name
@@ -324,19 +336,40 @@
             self.mode = mode
         self._stderr = ErrorOutput()
         if destination is None:
             if destination_path:
                 self.opened = False
             else:
                 self.destination = sys.stdout
+        elif (# destination is file-type object -> check mode:
+              mode and hasattr(self.destination, 'mode')
+              and mode != self.destination.mode):
+                print >>self._stderr, ('Destination mode "%s" '
+                               'differs from specified mode "%s"' %
+                               (self.destination.mode, mode))
         if not destination_path:
             try:
                 self.destination_path = self.destination.name
             except AttributeError:
                 pass
+        # Special cases under Python 3: different encoding or binary output
+        if sys.version_info >= (3,0):
+            if ('b' in self.mode
+                and self.destination in (sys.stdout, sys.stderr)
+               ):
+                self.destination = self.destination.buffer
+            if check_encoding(self.destination, self.encoding) is False:
+                if self.destination in (sys.stdout, sys.stderr):
+                    self.destination = self.destination.buffer
+                else:  # TODO: try the `write to .buffer` scheme instead?
+                    raise ValueError('Encoding of %s (%s) differs \n'
+                                     '  from specified encoding (%s)' %
+                                     (self.destination_path or 'destination',
+                                      destination.encoding, encoding))
+
 
     def open(self):
         # Specify encoding in Python 3.
         if sys.version_info >= (3,0):
             kwargs = {'encoding': self.encoding,
                       'errors': self.error_handler}
         else:
@@ -345,42 +378,38 @@
             self.destination = open(self.destination_path, self.mode, **kwargs)
         except IOError, error:
             if self.handle_io_errors:
                 print >>self._stderr, ErrorString(error)
                 print >>self._stderr, (u'Unable to open destination file'
                     u" for writing ('%s').  Exiting." % self.destination_path)
                 sys.exit(1)
-            raise OutputError(error.errno, error.strerror, 
+            raise OutputError(error.errno, error.strerror,
                               self.destination_path)
         self.opened = True
 
     def write(self, data):
         """Encode `data`, write it to a single file, and return it.
 
-        In Python 3, `data` is returned unchanged.
+        With Python 3 or binary output mode, `data` is returned unchanged,
+        except when specified encoding and output encoding differ.
         """
-        if sys.version_info < (3,0):
-            data = self.encode(data)
         if not self.opened:
             self.open()
         try: # In Python < 2.5, try...except has to be nested in try...finally.
             try:
-                if (sys.version_info >= (3,0) and self.encoding and
-                    hasattr(self.destination,'encoding') and
-                    self.encoding != self.destination.encoding and
-                    codecs.lookup(self.encoding) !=
-                    codecs.lookup(self.destination.encoding)):
-                    # encode self, write bytes
-                    bdata = self.encode(data)
-                    if os.linesep != '\n':
-                        bdata = bdata.replace('\n', os.linesep)
-                    sys.stdout.buffer.write(bdata)
-                else:
-                    self.destination.write(data)
-            except (UnicodeError, LookupError), err: # can only happen in py3k
+                if 'b' not in self.mode and (sys.version_info < (3,0) or
+                   check_encoding(self.destination, self.encoding) is False):
+                    data = self.encode(data)
+                    if sys.version_info >= (3,0) and os.linesep != '\n':
+                        # writing as binary data -> fix endings
+                        data = data.replace('\n', os.linesep)
+
+                self.destination.write(data)
+
+            except (UnicodeError, LookupError), err:
                 raise UnicodeError(
                     'Unable to encode output data. output-encoding is: '
                     '%s.\n(%s)' % (self.encoding, ErrorString(err)))
         finally:
             if self.autoclose:
                 self.close()
         return data
```

### Comparing `docutils-0.9/docutils/nodes.py` & `docutils-0.9.1/docutils/nodes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/statemachine.py` & `docutils-0.9.1/docutils/statemachine.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/docutils/urischemes.py` & `docutils-0.9.1/docutils/urischemes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/licenses/BSD-2-Clause.txt` & `docutils-0.9.1/licenses/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/licenses/gpl-3-0.txt` & `docutils-0.9.1/licenses/gpl-3-0.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/licenses/python-2-1-1.txt` & `docutils-0.9.1/licenses/python-2-1-1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/data/dependencies.txt` & `docutils-0.9.1/test/data/dependencies.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/data/full-template.txt` & `docutils-0.9.1/test/data/full-template.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/framing.css` & `docutils-0.9.1/test/functional/expected/ui/default/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/iepngfix.htc` & `docutils-0.9.1/test/functional/expected/ui/default/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/outline.css` & `docutils-0.9.1/test/functional/expected/ui/default/outline.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/pretty.css` & `docutils-0.9.1/test/functional/expected/ui/default/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/print.css` & `docutils-0.9.1/test/functional/expected/ui/default/print.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/default/slides.js` & `docutils-0.9.1/test/functional/expected/ui/default/slides.js`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/framing.css` & `docutils-0.9.1/test/functional/expected/ui/small-black/framing.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/iepngfix.htc` & `docutils-0.9.1/test/functional/expected/ui/small-black/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/outline.css` & `docutils-0.9.1/test/functional/expected/ui/small-black/outline.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/pretty.css` & `docutils-0.9.1/test/functional/expected/ui/small-black/pretty.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/print.css` & `docutils-0.9.1/test/functional/expected/ui/small-black/print.css`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/ui/small-black/slides.js` & `docutils-0.9.1/test/functional/expected/ui/small-black/slides.js`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/compact_lists.html` & `docutils-0.9.1/test/functional/expected/compact_lists.html`

 * *Files 5% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/compact_lists.html` & `docutils-0.9.1/test/functional/expected/compact_lists.html`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document">
       <ul class="simple">
         <li>This is an ordinary simple bullet list.</li>
         <li>It should be made compact (&lt;p&gt; &amp; &lt;/p&gt; tags omitted).</li>
       </ul>
```

### Comparing `docutils-0.9/test/functional/expected/cyrillic.tex` & `docutils-0.9.1/test/functional/expected/cyrillic.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/dangerous.html` & `docutils-0.9.1/test/functional/expected/dangerous.html`

 * *Files 2% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/dangerous.html` & `docutils-0.9.1/test/functional/expected/dangerous.html`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document">
       <p>Potentially dangerous features (security holes):</p>
       <div class="system-message">
         <p class="system-message-title">
           System Message: WARNING/2 (
```

### Comparing `docutils-0.9/test/functional/expected/field_name_limit.html` & `docutils-0.9.1/test/functional/expected/field_name_limit.html`

 * *Files 2% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/field_name_limit.html` & `docutils-0.9.1/test/functional/expected/field_name_limit.html`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document">
       <table class="docutils field-list" frame="void" rules="none">
         <col class="field-name"/>
         <col class="field-body"/>
         <tbody valign="top">
```

### Comparing `docutils-0.9/test/functional/expected/latex_docinfo.tex` & `docutils-0.9.1/test/functional/expected/latex_docinfo.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/math_output_html.html` & `docutils-0.9.1/test/functional/expected/math_output_html.html`

 * *Files 2% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/math_output_html.html` & `docutils-0.9.1/test/functional/expected/math_output_html.html`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>Mathematics</title>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/math.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/math.css" type="text/css"/>
   </head>
   <body>
     <div class="document" id="mathematics">
       <h1 class="title">Mathematics</h1>
       <p>
         Docutils supports inline math with the prefix or postfix
         <tt class="docutils literal">:math:</tt>
```

### Comparing `docutils-0.9/test/functional/expected/math_output_latex.html` & `docutils-0.9.1/test/functional/expected/math_output_latex.html`

 * *Files 2% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/math_output_latex.html` & `docutils-0.9.1/test/functional/expected/math_output_latex.html`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>Mathematics</title>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document" id="mathematics">
       <h1 class="title">Mathematics</h1>
       <p>
         Docutils supports inline math with the prefix or postfix
         <tt class="docutils literal">:math:</tt>
```

### Comparing `docutils-0.9/test/functional/expected/math_output_mathjax.html` & `docutils-0.9.1/test/functional/expected/math_output_mathjax.html`

 * *Files 1% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/math_output_mathjax.html` & `docutils-0.9.1/test/functional/expected/math_output_mathjax.html`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>Mathematics</title>
     <script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document" id="mathematics">
       <h1 class="title">Mathematics</h1>
       <p>
         Docutils supports inline math with the prefix or postfix
         <tt class="docutils literal">:math:</tt>
```

### Comparing `docutils-0.9/test/functional/expected/math_output_mathml.xhtml` & `docutils-0.9.1/test/functional/expected/math_output_mathml.xhtml`

 * *Files 0% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/math_output_mathml.xhtml` & `docutils-0.9.1/test/functional/expected/math_output_mathml.xhtml`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="application/xhtml+xml; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>Mathematics</title>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="document" id="mathematics">
       <h1 class="title">Mathematics</h1>
       <p>
         Docutils supports inline math with the prefix or postfix
         <tt class="docutils literal">:math:</tt>
```

### Comparing `docutils-0.9/test/functional/expected/misc_rst_html4css1.html` & `docutils-0.9.1/test/functional/expected/misc_rst_html4css1.html`

 * *Files 8% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/misc_rst_html4css1.html` & `docutils-0.9.1/test/functional/expected/misc_rst_html4css1.html`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title/>
     <link rel="stylesheet" href="foo&amp;bar.css" type="text/css"/>
   </head>
   <body>
     <div class="document">
       <p>Test the interaction of transforms.references.Substitutions and
 transforms.references.ExternalLinks.</p>
```

### Comparing `docutils-0.9/test/functional/expected/odt_basic.odt` & `docutils-0.9.1/test/functional/expected/odt_basic.odt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/odt_custom_headfoot.odt` & `docutils-0.9.1/test/functional/expected/odt_custom_headfoot.odt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/odt_tables1.odt` & `docutils-0.9.1/test/functional/expected/odt_tables1.odt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/pep_html.html` & `docutils-0.9.1/test/functional/expected/pep_html.html`

 * *Files 2% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/pep_html.html` & `docutils-0.9.1/test/functional/expected/pep_html.html`

```diff
@@ -6,17 +6,17 @@
   <!--
 This HTML is auto-generated.  DO NOT EDIT THIS FILE!  If you are writing a new
 PEP, see http://www.python.org/dev/peps/pep-0001 for instructions and links
 to templates.  DO NOT USE THIS HTML FILE AS YOUR TEMPLATE!
 -->
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>PEP 100 -- Test PEP</title>
-    <link rel="stylesheet" href="../../../docutils/writers/pep_html/pep.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body bgcolor="white">
     <table class="navigation" cellpadding="0" cellspacing="0" width="100%" border="0">
       <tr>
         <td class="navicon" width="150" height="35">
           <a href="http://www.python.org/" title="Python Home Page">
             <img src="http://www.python.org/pics/PyBanner000.gif" alt="[Python]" border="0" width="150" height="35"/>
```

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_html4css1.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_html4css1.html`

 * *Files 0% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/standalone_rst_html4css1.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_html4css1.html`

```diff
@@ -1,25 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <title>reStructuredText Test Document</title>
     <meta name="author" content="David Goodger"/>
     <meta name="authors" content="Me  Myself  I"/>
     <meta name="organization" content="humankind"/>
     <meta name="date" content="Now, or yesterday.  Or maybe even before yesterday."/>
     <meta name="copyright" content="This document has been placed in the public domain. You may do with it as you wish. You may copy, modify, redistribute, reattribute, sell, buy, rent, lease, destroy, or improve it, quote it at length, excerpt, incorporate, collate, fold, staple, or mutilate it, or do anything else to it that your or anyone else's heart desires."/>
     <meta content="reStructuredText, test, parser" name="keywords"/>
     <meta content="A test document, containing at least one example of each reStructuredText construct." lang="en" name="description"/>
     <script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
   </head>
   <body>
     <div class="header">
       Document header
       <hr class="header"/>
     </div>
     <div class="document" id="restructuredtext-test-document">
```

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_latex.tex` & `docutils-0.9.1/test/functional/expected/standalone_rst_latex.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_manpage.man` & `docutils-0.9.1/test/functional/expected/standalone_rst_manpage.man`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_pseudoxml.txt` & `docutils-0.9.1/test/functional/expected/standalone_rst_pseudoxml.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_s5_html_1.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_1.html`

 * *Files 1% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/standalone_rst_s5_html_1.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_1.html`

```diff
@@ -1,20 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <meta name="version" content="S5 1.1"/>
     <title>Slide Shows</title>
     <meta name="author" content="David Goodger"/>
     <meta name="date" content="2005-11-28"/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
     <!-- configuration parameters -->
     <meta name="defaultView" content="slideshow"/>
     <meta name="controlVis" content="hidden"/>
     <!-- style sheet links -->
     <script src="ui/small-black/slides.js" type="text/javascript"/>
     <link rel="stylesheet" href="ui/small-black/slides.css" type="text/css" media="projection" id="slideProj"/>
     <link rel="stylesheet" href="ui/small-black/outline.css" type="text/css" media="screen" id="outlineStyle"/>
```

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_s5_html_2.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_2.html`

 * *Files 1% similar despite different names*

#### Comparing `docutils-0.9/test/functional/expected/standalone_rst_s5_html_2.html` & `docutils-0.9.1/test/functional/expected/standalone_rst_s5_html_2.html`

```diff
@@ -1,20 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.9: http://docutils.sourceforge.net/"/>
+    <meta name="generator" content="Docutils 0.9.1: http://docutils.sourceforge.net/"/>
     <meta name="version" content="S5 1.1"/>
     <title>Slide Shows</title>
     <meta name="author" content="David Goodger"/>
     <meta name="date" content="2005-11-28"/>
-    <link rel="stylesheet" href="../../../docutils/writers/html4css1/html4css1.css" type="text/css"/>
+    <link rel="stylesheet" href="../input/data/html4css1.css" type="text/css"/>
     <!-- configuration parameters -->
     <meta name="defaultView" content="slideshow"/>
     <meta name="controlVis" content="hidden"/>
     <!-- style sheet links -->
     <script src="ui/default/slides.js" type="text/javascript"/>
     <link rel="stylesheet" href="ui/default/slides.css" type="text/css" media="projection" id="slideProj"/>
     <link rel="stylesheet" href="ui/default/outline.css" type="text/css" media="screen" id="outlineStyle"/>
```

### Comparing `docutils-0.9/test/functional/expected/standalone_rst_xetex.tex` & `docutils-0.9.1/test/functional/expected/standalone_rst_xetex.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/expected/xetex-cyrillic.tex` & `docutils-0.9.1/test/functional/expected/xetex-cyrillic.tex`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/custom_roles.txt` & `docutils-0.9.1/test/functional/input/data/custom_roles.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/custom_roles_latex.txt` & `docutils-0.9.1/test/functional/input/data/custom_roles_latex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/hyperlinking.txt` & `docutils-0.9.1/test/functional/input/data/hyperlinking.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/latex.txt` & `docutils-0.9.1/test/functional/input/data/latex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/latex_encoding.txt` & `docutils-0.9.1/test/functional/input/data/latex_encoding.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/math.txt` & `docutils-0.9.1/test/functional/input/data/math.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/standard.txt` & `docutils-0.9.1/test/functional/input/data/standard.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/svg_images.txt` & `docutils-0.9.1/test/functional/input/data/svg_images.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/swf_images.txt` & `docutils-0.9.1/test/functional/input/data/swf_images.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/table_complex.txt` & `docutils-0.9.1/test/functional/input/data/table_complex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/table_rowspan.txt` & `docutils-0.9.1/test/functional/input/data/table_rowspan.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/tables_latex.txt` & `docutils-0.9.1/test/functional/input/data/tables_latex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/unicode.txt` & `docutils-0.9.1/test/functional/input/data/unicode.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/data/urls.txt` & `docutils-0.9.1/test/functional/input/data/urls.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/compact_lists.txt` & `docutils-0.9.1/test/functional/input/compact_lists.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/cyrillic.txt` & `docutils-0.9.1/test/functional/input/cyrillic.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/link_in_substitution.txt` & `docutils-0.9.1/test/functional/input/link_in_substitution.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/odt_tables1.txt` & `docutils-0.9.1/test/functional/input/odt_tables1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/pep_html.txt` & `docutils-0.9.1/test/functional/input/pep_html.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/standalone_rst_html4css1.txt` & `docutils-0.9.1/test/functional/input/standalone_rst_html4css1.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/standalone_rst_latex.txt` & `docutils-0.9.1/test/functional/input/standalone_rst_latex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/standalone_rst_manpage.txt` & `docutils-0.9.1/test/functional/input/standalone_rst_manpage.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/standalone_rst_s5_html.txt` & `docutils-0.9.1/test/functional/input/standalone_rst_s5_html.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/input/standalone_rst_xetex.txt` & `docutils-0.9.1/test/functional/input/standalone_rst_xetex.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/functional/tests/standalone_rst_s5_html_1.py` & `docutils-0.9.1/test/functional/tests/standalone_rst_s5_html_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 test_destination = 'standalone_rst_s5_html_1.html'
 
 # Keyword parameters passed to publish_file:
 writer_name = 's5_html'
 
 # Settings:
 settings_overrides['theme'] = 'small-black'
+# local copy of default stylesheet:
+settings_overrides['stylesheet_path'] = ( 
+    'functional/input/data/html4css1.css')
 
 
 # Extra functional tests.
 # Prefix all names with '_' to avoid confusing `docutils.core.publish_file`.
 
 import filecmp as _filecmp
```

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/include10.txt` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/include10.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_admonitions.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_admonitions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_block_quotes.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_block_quotes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_class.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_class.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_code.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_code_long.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code_long.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_code_none.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_code_none.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_compound.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_compound.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_container.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_container.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_contents.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_contents.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_date.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_date.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_decorations.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_decorations.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_default_role.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_default_role.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_figures.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_figures.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_images.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_images.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_include.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_include.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 
-# $Id: test_include.py 7384 2012-03-19 22:59:09Z milde $
+# $Id: test_include.py 7433 2012-05-11 21:03:07Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 Tests for misc.py "include" directive.
 """
 
@@ -46,14 +46,26 @@
                         "Tried the following encodings: 'ascii'.\n"
                         "            (%s)" % utf_16_error_str)
 nonexistent = os.path.join(os.path.dirname(states.__file__),
                            'include', 'nonexistent')
 nonexistent_rel = DocutilsTestSupport.utils.relative_path(
     os.path.join(DocutilsTestSupport.testroot, 'dummy'), nonexistent)
 
+# Different error for path with 8bit chars with locale == C or None:
+try:
+    open(u'\u043c\u0438\u0440.txt')
+except UnicodeEncodeError:
+    errstr_8bit_path = u"""\
+Cannot encode input file path "\u043c\u0438\u0440.txt" (wrong locale?).\
+"""
+except:
+    errstr_8bit_path = u"""\
+InputError: [Errno 2] No such file or directory: '\u043c\u0438\u0440.txt'.\
+"""
+
 totest = {}
 
 totest['include'] = [
 ["""\
 Include Test
 ============
 
@@ -410,18 +422,18 @@
 u"""\
 <document source="test data">
     <paragraph>
         cyrillic filename:
     <system_message level="4" line="3" source="test data" type="SEVERE">
         <paragraph>
             Problems with "include" directive path:
-            InputError: [Errno 2] No such file or directory: '\u043c\u0438\u0440.txt'.
+            %s
         <literal_block xml:space="preserve">
             .. include:: \u043c\u0438\u0440.txt
-"""],
+""" % errstr_8bit_path],
 ["""\
 Testing errors in included file:
 
 .. include:: %s
 """ % include10,
 """\
 <document source="test data">
```

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_line_blocks.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_line_blocks.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_math.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_math.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_meta.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_meta.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_parsed_literals.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_parsed_literals.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_raw.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_raw.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_replace.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_replace.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_replace_fr.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_replace_fr.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_role.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_role.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_rubrics.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_rubrics.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_sectnum.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_sectnum.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_sidebars.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_sidebars.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_tables.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_tables.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_target_notes.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_target_notes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_test_directives.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_test_directives.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_title.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_title.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_topics.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_topics.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_unicode.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_unicode.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_directives/test_unknown.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_directives/test_unknown.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_SimpleTableParser.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_SimpleTableParser.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_TableParser.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_TableParser.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_block_quotes.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_block_quotes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_bullet_lists.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_bullet_lists.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_citations.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_citations.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_comments.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_comments.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_definition_lists.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_definition_lists.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_doctest_blocks.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_doctest_blocks.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_east_asian_text.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_east_asian_text.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_enumerated_lists.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_enumerated_lists.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_field_lists.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_field_lists.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_footnotes.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_functions.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_functions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_inline_markup.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_inline_markup.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_interpreted.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_interpreted.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_interpreted_fr.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_interpreted_fr.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_line_blocks.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_line_blocks.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_literal_blocks.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_literal_blocks.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_option_lists.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_option_lists.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_outdenting.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_outdenting.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_paragraphs.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_paragraphs.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_section_headers.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_section_headers.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_substitutions.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_tables.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_tables.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_targets.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_targets.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_rst/test_transitions.py` & `docutils-0.9.1/test/test_parsers/test_rst/test_transitions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_parsers/test_parser.py` & `docutils-0.9.1/test/test_parsers/test_parser.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_readers/test_pep/test_inline_markup.py` & `docutils-0.9.1/test/test_readers/test_pep/test_inline_markup.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_readers/test_pep/test_rfc2822.py` & `docutils-0.9.1/test/test_readers/test_pep/test_rfc2822.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test___init__.py` & `docutils-0.9.1/test/test_transforms/test___init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_class.py` & `docutils-0.9.1/test/test_transforms/test_class.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_contents.py` & `docutils-0.9.1/test/test_transforms/test_contents.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_docinfo.py` & `docutils-0.9.1/test/test_transforms/test_docinfo.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_doctitle.py` & `docutils-0.9.1/test/test_transforms/test_doctitle.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_expose_internals.py` & `docutils-0.9.1/test/test_transforms/test_expose_internals.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_filter.py` & `docutils-0.9.1/test/test_transforms/test_filter.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_footnotes.py` & `docutils-0.9.1/test/test_transforms/test_footnotes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_hyperlinks.py` & `docutils-0.9.1/test/test_transforms/test_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_messages.py` & `docutils-0.9.1/test/test_transforms/test_messages.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_peps.py` & `docutils-0.9.1/test/test_transforms/test_peps.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_sectnum.py` & `docutils-0.9.1/test/test_transforms/test_sectnum.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_strip_comments.py` & `docutils-0.9.1/test/test_transforms/test_strip_comments.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_substitutions.py` & `docutils-0.9.1/test/test_transforms/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_target_notes.py` & `docutils-0.9.1/test/test_transforms/test_target_notes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_transitions.py` & `docutils-0.9.1/test/test_transforms/test_transitions.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_transforms/test_writer_aux.py` & `docutils-0.9.1/test/test_transforms/test_writer_aux.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_docutils_xml.py` & `docutils-0.9.1/test/test_writers/test_docutils_xml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_html4css1_misc.py` & `docutils-0.9.1/test/test_writers/test_html4css1_misc.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_html4css1_parts.py` & `docutils-0.9.1/test/test_writers/test_html4css1_parts.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_html4css1_template.py` & `docutils-0.9.1/test/test_writers/test_html4css1_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 
-# $Id: test_html4css1_template.py 6379 2010-07-19 16:07:19Z goodger $
+# $Id: test_html4css1_template.py 7437 2012-06-04 20:14:08Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 Tests for the HTML writer.
 """
 
 import os
 from __init__ import DocutilsTestSupport
 
 
 def suite():
     settings = {'template': os.path.join(DocutilsTestSupport.testroot,
                                          'data', 'full-template.txt'),
+                'stylesheet_path': '/test.css',
                 'embed_stylesheet': 0,}
     s = DocutilsTestSupport.PublishTestSuite('html', suite_settings=settings)
     s.generateTests(totest)
     return s
 
 totest = {}
 
@@ -51,15 +52,15 @@
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
 <meta name="generator" content="Docutils %(version)s: http://docutils.sourceforge.net/" />
 <title>Document Title</title>
 <meta name="author" content="Me" />"""
 
 
 stylesheet = """\
-<link rel="stylesheet" href="../docutils/writers/html4css1/html4css1.css" type="text/css" />"""
+<link rel="stylesheet" href="/test.css" type="text/css" />"""
 
 
 body_prefix = """\
 </head>
 <body>
 <div class="document" id="document-title">"""
 
@@ -108,15 +109,15 @@
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
 <meta name="generator" content="Docutils %(version)s: http://docutils.sourceforge.net/" />
 <title>Document Title</title>
 <meta name="author" content="Me" />"""
 
 
 stylesheet = """\
-<link rel="stylesheet" href="../docutils/writers/html4css1/html4css1.css" type="text/css" />"""
+<link rel="stylesheet" href="/test.css" type="text/css" />"""
 
 
 body_prefix = """\
 </head>
 <body>
 <div class="document" id="document-title">"""
```

### Comparing `docutils-0.9/test/test_writers/test_latex2e.py` & `docutils-0.9.1/test/test_writers/test_latex2e.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_manpage.py` & `docutils-0.9.1/test/test_writers/test_manpage.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_null.py` & `docutils-0.9.1/test/test_writers/test_null.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_odt.py` & `docutils-0.9.1/test/test_writers/test_odt.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_pseudoxml.py` & `docutils-0.9.1/test/test_writers/test_pseudoxml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_writers/test_s5.py` & `docutils-0.9.1/test/test_writers/test_s5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 
-# $Id: test_s5.py 6379 2010-07-19 16:07:19Z goodger $
+# $Id: test_s5.py 7437 2012-06-04 20:14:08Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 Tests for the S5/HTML writer.
 """
 
 import os
 from __init__ import DocutilsTestSupport
 
 
 def suite():
-    settings = {'embed_stylesheet': 0,}
+    settings = {'stylesheet_path': '/test.css',
+                'embed_stylesheet': 0,}
     s = DocutilsTestSupport.PublishTestSuite('s5', suite_settings=settings)
     s.generateTests(totest_1)
     settings['hidden_controls'] = 0
     settings['view_mode'] = 'outline'
     s.generateTests(totest_2)
     return s
 
@@ -44,15 +45,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
 <meta name="generator" content="Docutils %(version)s: http://docutils.sourceforge.net/" />
 <meta name="version" content="S5 1.1" />
 <title>Show Title</title>
-<link rel="stylesheet" href="../docutils/writers/html4css1/html4css1.css" type="text/css" />
+<link rel="stylesheet" href="/test.css" type="text/css" />
 <!-- configuration parameters -->
 <meta name="defaultView" content="slideshow" />
 <meta name="controlVis" content="hidden" />
 <!-- style sheet links -->
 <script src="ui/default/slides.js" type="text/javascript"></script>
 <link rel="stylesheet" href="ui/default/slides.css"
       type="text/css" media="projection" id="slideProj" />
@@ -109,15 +110,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
 <meta name="generator" content="Docutils %(version)s: http://docutils.sourceforge.net/" />
 <meta name="version" content="S5 1.1" />
 <title>Bogus Slide Show</title>
-<link rel="stylesheet" href="../docutils/writers/html4css1/html4css1.css" type="text/css" />
+<link rel="stylesheet" href="/test.css" type="text/css" />
 <!-- configuration parameters -->
 <meta name="defaultView" content="outline" />
 <meta name="controlVis" content="visible" />
 <!-- style sheet links -->
 <script src="ui/default/slides.js" type="text/javascript"></script>
 <link rel="stylesheet" href="ui/default/slides.css"
       type="text/css" media="projection" id="slideProj" />
```

### Comparing `docutils-0.9/test/DocutilsTestSupport.py` & `docutils-0.9.1/test/DocutilsTestSupport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# $Id: DocutilsTestSupport.py 7400 2012-05-01 08:34:41Z grubert $
+# $Id: DocutilsTestSupport.py 7440 2012-06-13 14:14:12Z milde $
 # Authors: David Goodger <goodger@python.org>;
 #          Garth Kidd <garth@deadlybloodyserious.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 Exports the following:
 
@@ -46,17 +46,23 @@
 import re
 import inspect
 import traceback
 from pprint import pformat
 
 testroot = os.path.abspath(os.path.dirname(__file__) or os.curdir)
 os.chdir(testroot)
-sys.path.insert(0, os.path.normpath(os.path.join(testroot, '..')))
+if sys.version_info >= (3,0):
+    sys.path.insert(0, os.path.normpath(os.path.join(testroot,
+                                                     '..', 'build', 'lib')))
+    sys.path.append(os.path.normpath(os.path.join(testroot, '..',
+                                                  'build', 'lib', 'extras')))
+else:
+    sys.path.insert(0, os.path.normpath(os.path.join(testroot, '..')))
+    sys.path.append(os.path.normpath(os.path.join(testroot, '..', 'extras')))
 sys.path.insert(0, testroot)
-sys.path.append(os.path.normpath(os.path.join(testroot, '..', 'extras')))
 
 try:
     import difflib
     import package_unittest
     import docutils
     import docutils.core
     from docutils import frontend, nodes, statemachine, urischemes, utils
@@ -125,21 +131,21 @@
 
     # python 2.3
     if not hasattr(unittest.TestCase, "assertTrue"):
         assertTrue = unittest.TestCase.failUnless
 
     # aliases for assertion methods, deprecated since Python 2.7
 
-    failUnlessEqual = assertEquals = assertEqual 
+    failUnlessEqual = assertEquals = assertEqual
 
     assertNotEquals = failIfEqual = assertNotEqual
 
 
 class CustomTestCase(StandardTestCase):
-    
+
     """
     Helper class, providing extended functionality over unittest.TestCase.
 
     The methods assertEqual and assertNotEqual have been overwritten
     to provide better support for multi-line strings.  Furthermore,
     see the compare_output method and the parameter list of __init__.
     """
@@ -162,15 +168,15 @@
         suite_settings -- settings overrides for this test suite.
         """
         self.id = id
         self.input = input
         self.expected = expected
         self.run_in_debugger = run_in_debugger
         self.suite_settings = suite_settings.copy() or {}
-        
+
         # Ring your mother.
         unittest.TestCase.__init__(self, method_name)
 
     def __str__(self):
         """
         Return string conversion. Overridden to give test id, in addition to
         method name.
@@ -787,15 +793,15 @@
             writer_name=self.writer_name,
             settings_spec=self,
             settings_overrides=self.suite_settings)
         output = self.format_output(parts)
         # interpolate standard variables:
         expected = self.expected % {'version': docutils.__version__}
         self.compare_output(self.input, output, expected)
-    
+
     standard_content_type_template = ('<meta http-equiv="Content-Type"'
                                       ' content="text/html; charset=%s" />\n')
     standard_generator_template = (
         '<meta name="generator"'
         ' content="Docutils %s: http://docutils.sourceforge.net/" />\n')
     standard_html_meta_value = (
         standard_content_type_template
@@ -871,15 +877,15 @@
         'foo  \nbar\n\nbaz'
 
     This is a helper function for CustomTestCase.
     """
     return_tuple = []
     for i in args:
         r = repr(i)
-        if ( (isinstance(i, str) or isinstance(i, unicode))
+        if ( (isinstance(i, bytes) or isinstance(i, unicode))
              and '\n' in i):
             stripped = ''
             if isinstance(i, unicode) and r.startswith('u'):
                 stripped = r[0]
                 r = r[1:]
             elif isinstance(i, bytes) and r.startswith('b'):
                 stripped = r[0]
```

### Comparing `docutils-0.9/test/alltests.py` & `docutils-0.9.1/test/alltests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/sh
 ''''exec python -u "$0" "$@" #'''
 
-# $Id: alltests.py 7052 2011-06-05 13:12:06Z grubert $
+# $Id: alltests.py 7433 2012-05-11 21:03:07Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 __doc__ = \
 """
 All modules named 'test_*.py' in the current directory, and recursively in
 subdirectories (packages) called 'test_*', are loaded and test suites within
@@ -29,16 +29,21 @@
 
     def __init__(self, filename, stream=sys.__stdout__):
         self.file = open(filename, 'w')
         self.stream = stream
         self.encoding = getattr(stream, 'encoding', None)
 
     def write(self, string):
-        self.stream.write(string)
-        self.file.write(string)
+        try:
+            self.stream.write(string)
+            self.file.write(string)
+        except UnicodeEncodeError:   # Py3k writing to "ascii" stream/file
+            string = string.encode('raw_unicode_escape').decode('ascii')
+            self.stream.write(string)
+            self.file.write(string)
 
     def flush(self):
         self.stream.flush()
         self.file.flush()
 
 
 def pformat(suite):
```

### Comparing `docutils-0.9/test/coverage.sh` & `docutils-0.9.1/test/coverage.sh`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/package_unittest.py` & `docutils-0.9.1/test/package_unittest.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test__init__.py` & `docutils-0.9.1/test/test__init__.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_command_line.py` & `docutils-0.9.1/test/test_command_line.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_dependencies.py` & `docutils-0.9.1/test/test_dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 
-# $Id: test_dependencies.py 7404 2012-05-01 16:07:54Z grubert $
+# $Id: test_dependencies.py 7437 2012-06-04 20:14:08Z milde $
 # Author: Lea Wiemann <LeWiemann@gmail.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 Test module for the --record-dependencies option.
 """
 
@@ -20,15 +20,14 @@
 # docutils.utils.DependencyList records POSIX paths,
 # i.e. "/" as a path separator even on Windows (not os.path.join).
 paths = {'include': u'data/include.txt',  # included rst file
          'raw':     u'data/raw.txt',      # included raw "HTML file"
          'scaled-image': u'../docs/user/rst/images/biohazard.png',
          'figure-image': u'../docs/user/rst/images/title.png',
          'stylesheet':   u'data/stylesheet.txt',
-         'default-stylesheet': u'../docutils/writers/html4css1/html4css1.css',
         }
 
 
 class RecordDependenciesTests(unittest.TestCase):
 
     # python 2.3
     if not hasattr(unittest.TestCase, "assertTrue"):
@@ -67,19 +66,21 @@
         record = self.get_record(writer_name='xml')
         # the order of the files is arbitrary
         record.sort()
         expected.sort()
         self.assertEqual(record, expected)
 
     def test_dependencies_html(self):
-        keys = ['include', 'raw', 'default-stylesheet']
+        keys = ['include', 'raw']
         if PIL:
             keys += ['figure-image', 'scaled-image']
         expected = [paths[key] for key in keys]
-        record = self.get_record(writer_name='html')
+        # stylesheets are tested separately in test_stylesheet_dependencies():
+        so = {'stylesheet_path': None, 'stylesheet': None}
+        record = self.get_record(writer_name='html', settings_overrides=so)
         # the order of the files is arbitrary
         record.sort()
         expected.sort()
         self.assertEqual(record, expected)
 
     def test_dependencies_latex(self):
         # since 0.9, the latex writer records only really accessed files, too
```

### Comparing `docutils-0.9/test/test_error_reporting.py` & `docutils-0.9.1/test/test_error_reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 # .. coding: utf8
-# $Id: test_error_reporting.py 7337 2012-02-03 08:16:53Z milde $
+# $Id: test_error_reporting.py 7440 2012-06-13 14:14:12Z milde $
 # Author: Günter Milde <milde@users.sourceforge.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 Test `EnvironmentError` reporting.
 
 In some locales, the `errstr` argument of IOError and OSError contains
@@ -154,22 +154,22 @@
                          unicode(ErrorString(ImportError(self.bs))))
 
 
 # ErrorOutput tests
 # -----------------
 
 # Stub: Buffer with 'strict' auto-conversion of input to byte string:
-class BBuf(BytesIO, object):
+class BBuf(BytesIO, object): # super class object required by Python <= 2.5
     def write(self, data):
         if isinstance(data, unicode):
             data.encode('ascii', 'strict')
         super(BBuf, self).write(data)
 
 # Stub: Buffer expecting unicode string:
-class UBuf(StringIO, object):
+class UBuf(StringIO, object): # super class object required by Python <= 2.5
     def write(self, data):
         # emulate Python 3 handling of stdout, stderr
         if isinstance(data, bytes):
             raise TypeError('must be unicode, not bytes')
         super(UBuf, self).write(data)
 
 class ErrorOutputTests(unittest.TestCase):
```

### Comparing `docutils-0.9/test/test_functional.py` & `docutils-0.9.1/test/test_functional.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_language.py` & `docutils-0.9.1/test/test_language.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_nodes.py` & `docutils-0.9.1/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_pickle.py` & `docutils-0.9.1/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_publisher.py` & `docutils-0.9.1/test/test_publisher.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_settings.py` & `docutils-0.9.1/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_statemachine.py` & `docutils-0.9.1/test/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_traversals.py` & `docutils-0.9.1/test/test_traversals.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_utils.py` & `docutils-0.9.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/test/test_viewlist.py` & `docutils-0.9.1/test/test_viewlist.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/dev/create_unimap.py` & `docutils-0.9.1/tools/dev/create_unimap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #!/usr/bin/env python
 
-# $Id: create_unimap.py 5174 2007-05-31 00:01:52Z wiemann $
+# $Id: create_unimap.py 7442 2012-06-13 23:27:03Z milde $
 # Author: Lea Wiemann <LeWiemann@gmail.com>
 # Copyright: This file has been placed in the public domain.
 
 # Call: create_unimap.py < unicode.xml > unicode_latex.py
 #
 # Get unicode.xml from
 # <http://www.w3.org/2003/entities/xml/unicode.xml>.
 
 from xml.dom import minidom
 import sys
 import pprint
 
+if sys.version_info >= (3,0):
+    unicode = str
+else:
+    bytes = str
+    chr = unichr
+
+
 def w(s):
-    if isinstance(s, unicode):
+    if sys.version_info >= (3,0) and isinstance(s, unicode):
         s = s.encode('utf8')
     sys.stdout.write(s)
 
 text_map = {}
 math_map = {}
 
 class Visitor:
@@ -35,17 +42,17 @@
                     continue
                 if int(code) < 128:
                     # Wrong (maps "-" to "$-$", which is too wide) and
                     # unnecessary (maps "a" to "{a}").
                     continue
                 latex_code = n.childNodes[0].nodeValue.encode('ascii').strip()
                 if node.attributes['mode'].value == 'math':
-                    math_map[unichr(int(code))] = '$%s$' % latex_code
+                    math_map[chr(int(code))] = '$%s$' % latex_code
                 else:
-                    text_map[unichr(int(code))] = '{%s}' % latex_code
+                    text_map[chr(int(code))] = '{%s}' % latex_code
 
 def call_visitor(node, visitor=Visitor()):
     if isinstance(node, minidom.Text):
         name = 'Text'
     else:
         name = node.nodeName.replace('#', '_')
     if hasattr(visitor, 'visit_' + name):
@@ -59,20 +66,20 @@
 call_visitor(document)
 
 unicode_map = math_map
 unicode_map.update(text_map)
 # Now unicode_map contains the text entries plus dollar-enclosed math
 # entries for those chars for which no text entry exists.
 
-print '# $%s$' % 'Id'
-print '# Author: Lea Wiemann <LeWiemann@gmail.com>'
-print '# Copyright: This file has been placed in the public domain.'
-print
-print '# This is a mapping of Unicode characters to LaTeX equivalents.'
-print '# The information has been extracted from'
-print '# <http://www.w3.org/2003/entities/xml/unicode.xml>, written by'
-print '# David Carlisle and Sebastian Rahtz.'
-print '#'
-print '# The extraction has been done by the "create_unimap.py" script'
-print '# located at <http://docutils.sf.net/tools/dev/create_unimap.py>.'
-print
-print 'unicode_map = %s' % pprint.pformat(unicode_map, indent=0)
+print('# $%s$' % 'Id')
+print('# Author: Lea Wiemann <LeWiemann@gmail.com>')
+print('# Copyright: This file has been placed in the public domain.')
+print('')
+print('# This is a mapping of Unicode characters to LaTeX equivalents.')
+print('# The information has been extracted from')
+print('# <http://www.w3.org/2003/entities/xml/unicode.xml>, written by')
+print('# David Carlisle and Sebastian Rahtz.')
+print('#')
+print('# The extraction has been done by the "create_unimap.py" script')
+print('# located at <http://docutils.sf.net/tools/dev/create_unimap.py>.')
+print('')
+print('unicode_map = %s' % pprint.pformat(unicode_map, indent=0))
```

### Comparing `docutils-0.9/tools/dev/profile_docutils.py` & `docutils-0.9.1/tools/dev/profile_docutils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/python -i
 
-# $Id: profile_docutils.py 5618 2008-07-28 08:37:32Z strank $
+# $Id: profile_docutils.py 7442 2012-06-13 23:27:03Z milde $
 # Author: Lea Wiemann <LeWiemann@gmail.com>
 # Copyright: This script has been placed in the public domain.
 
 import os.path
 import docutils.core
 import hotshot.stats
 
-print 'Profiler started.'
+print('Profiler started.')
 
 os.chdir(os.path.join(os.path.dirname(docutils.__file__), '..'))
 
-print 'Profiling...'
+print('Profiling...')
 
 prof = hotshot.Profile('docutils.prof')
 prof.runcall(docutils.core.publish_file, source_path='HISTORY.txt',
              destination_path='prof.HISTORY.html', writer_name='html')
 prof.close()
 
-print 'Loading statistics...'
+print('Loading statistics...')
 
-print """
+print("""
 stats = hotshot.stats.load('docutils.prof')
 stats.strip_dirs()
 stats.sort_stats('time')  # 'cumulative'; 'calls'
 stats.print_stats(40)
-"""
+""")
 
 stats = hotshot.stats.load('docutils.prof')
 stats.strip_dirs()
 stats.sort_stats('time')
 stats.print_stats(40)
 
 try:
```

### Comparing `docutils-0.9/tools/dev/unicode2rstsubs.py` & `docutils-0.9.1/tools/dev/unicode2rstsubs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 
-# $Id: unicode2rstsubs.py 5618 2008-07-28 08:37:32Z strank $
+# $Id: unicode2rstsubs.py 7442 2012-06-13 23:27:03Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This program has been placed in the public domain.
 
 """
 unicode2subfiles.py -- produce character entity files (reSructuredText
 substitutions) from the W3C master unicode.xml file.
 
@@ -23,35 +23,38 @@
 import sys
 import os
 import optparse
 import re
 from xml.parsers.expat import ParserCreate
 
 
-usage_msg = """Usage: %s [unicode.xml]"""
+usage_msg = """Usage: %s [unicode.xml]\n"""
 
 def usage(prog, status=0, msg=None):
-    print >>sys.stderr, usage_msg % prog
+    sys.stderr.write(usage_msg % prog)
     if msg:
-        print >>sys.stderr, msg
+        sys.stderr.write(msg + '\n')
     sys.exit(status)
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
     if len(argv) == 2:
         inpath = argv[1]
     elif len(argv) > 2:
         usage(argv[0], 2,
               'Too many arguments (%s): only 1 expected.' % (len(argv) - 1))
     else:
         inpath = 'unicode.xml'
     if not os.path.isfile(inpath):
         usage(argv[0], 1, 'No such file: "%s".' % inpath)
-    infile = open(inpath)
+    if sys.version_info >= (3,0):
+        infile = open(inpath, mode='rb')
+    else:
+        infile = open(inpath)
     process(infile)
 
 def process(infile):
     grouper = CharacterEntitySetExtractor(infile)
     grouper.group()
     grouper.write_sets()
 
@@ -126,15 +129,15 @@
         self.charid = attributes['id']
 
     def entity_start(self, name, attributes):
         set = self.entity_set_name(attributes['set'])
         if not set:
             return
         if set not in self.sets:
-            print 'bad set: %r' % set
+            print('bad set: %r' % set)
             return
         entity = attributes['id']
         assert (entity not in self.sets[set]
                 or self.sets[set][entity] == self.charid), \
                 ('sets[%r][%r] == %r (!= %r)'
                  % (set, entity, self.sets[set][entity], self.charid))
         self.sets[set][entity] = self.charid
@@ -155,27 +158,27 @@
         name = match.group(1).lower()
         if name in self.unwanted_entity_sets:
             return None
         self.sets.setdefault(name, {})
         return name
 
     def write_sets(self):
-        sets = self.sets.keys()
+        sets = list(self.sets.keys())
         sets.sort()
         for set_name in sets:
             self.write_set(set_name)
 
     def write_set(self, set_name, wide=None):
         if wide:
             outname = set_name + '-wide.txt'
         else:
             outname = set_name + '.txt'
         outfile = open(outname, 'w')
-        print 'writing file "%s"' % outname
-        print >>outfile, self.header
+        print('writing file "%s"' % outname)
+        outfile.write(self.header + '\n')
         set = self.sets[set_name]
         entities = [(e.lower(), e) for e in set.keys()]
         entities.sort()
         longest = 0
         for _, entity_name in entities:
             longest = max(longest, len(entity_name))
         has_wide = None
@@ -189,14 +192,14 @@
                      wide=None):
         charid = set[entity_name]
         if not wide:
             for code in charid[1:].split('-'):
                 if int(code, 16) > 0xFFFF:
                     return 1            # wide-Unicode character
         codes = ' '.join(['U+%s' % code for code in charid[1:].split('-')])
-        print >>outfile, ('.. %-*s unicode:: %s .. %s'
-                          % (longest + 2, '|' + entity_name + '|',
-                             codes, self.descriptions[charid]))
+        outfile.write('.. %-*s unicode:: %s .. %s\n'
+                      % (longest + 2, '|' + entity_name + '|',
+                         codes, self.descriptions[charid]))
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `docutils-0.9/tools/editors/emacs/tests/README.txt` & `docutils-0.9.1/tools/editors/emacs/tests/README.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/adjust-section.el` & `docutils-0.9.1/tools/editors/emacs/tests/adjust-section.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/adornment.el` & `docutils-0.9.1/tools/editors/emacs/tests/adornment.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/comment.el` & `docutils-0.9.1/tools/editors/emacs/tests/comment.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/ert-support.el` & `docutils-0.9.1/tools/editors/emacs/tests/ert-support.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/fill.el` & `docutils-0.9.1/tools/editors/emacs/tests/fill.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/font-lock.el` & `docutils-0.9.1/tools/editors/emacs/tests/font-lock.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/indent.el` & `docutils-0.9.1/tools/editors/emacs/tests/indent.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/items.el` & `docutils-0.9.1/tools/editors/emacs/tests/items.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/movement.el` & `docutils-0.9.1/tools/editors/emacs/tests/movement.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/re.el` & `docutils-0.9.1/tools/editors/emacs/tests/re.el`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,16 @@
 		   (cons 1 1)
 		   (cons 2 2)
 		   (cons 4 3))
 	     (cons "\\\\(|" "\\(?:|") ;; Make a group shy
 	     (cons "\\[^|\n]\\+" "\\(?:\\S \\|\\S \\(?:[^|\\\n]\\|\\\\.\\)\\{0,1000\\}[^	 |\\]\\)"
 		   ) ;; Symbol name more sophisticated
 	     (cons (regexp-quote "\\(\\sw\\|\\s_\\)+")
-		   "\\(?:\\sw+\\(?:\\s_\\sw+\\)*\\)") ;; New syntax for symbols
+		   "\\(?:\\sw+\\(?:[-+.:_]\\sw+\\)*\\)") ;; New syntax for
+							 ;; symbols
 	     (cons "\\\\(\\[\t " "\\(?:[\t ") ;; Make a group shy
 	     ))
     (should (re-equal-matches
 	     ;; `Hyperlink Targets`_
 	     (concat re-bol "\\(" re-ems "_\\([^:\\`\n]\\|\\\\.\\|`[^`\n]+`\\)+:\\)"
 		     re-blksep1)
 	     "=== rst.el.~rst_el_1_68~:3049"
@@ -758,17 +759,19 @@
 		   (cons 8 3))
 	     (cons "^\\\\(" "\\(?:") ;; Make a group shy
 	     (cons "\\\\(\\\\S" "\\(?:\\S") ;; Make a group shy
 	     (cons "\\\\(\\[^" "\\(?:[^") ;; Make a group shy
 	     (cons "\\\\(:" "\\(?::") ;; Make a group shy
 	     (cons "\\\\(:" "\\(?::") ;; Make a group shy
 	     (cons (regexp-quote "\\(\\sw\\|\\s_\\)+")
-		   "\\(?:\\sw+\\(?:\\s_\\sw+\\)*\\)") ;; New syntax for symbols
+		   "\\(?:\\sw+\\(?:[-+.:_]\\sw+\\)*\\)") ;; New syntax for
+							 ;; symbols
 	     (cons (regexp-quote "\\(\\sw\\|\\s_\\)+")
-		   "\\(?:\\sw+\\(?:\\s_\\sw+\\)*\\)") ;; New syntax for symbols
+		   "\\(?:\\sw+\\(?:[-+.:_]\\sw+\\)*\\)") ;; New syntax for
+							 ;; symbols
 	     (cons (regexp-quote "\\\\]") "\\]") ;; Remove superfluous quote
 	     (cons (regexp-quote "\\|$") "")
 	     (cons (regexp-quote "\\([\t ]")
 		   "\\(?:$\\|[\t ]") ;; Move "$" in regex and make a group shy
 	     ))
     (should (re-equal-matches
 	     ;; `Footnote References`_ / `Citation References`_
@@ -819,17 +822,19 @@
 	     (concat re-imp1 "\\(" re-sym1 "+@" re-sym1 "+\\)" re-ims1)
 	     "=== rst.el.~rst_el_1_68~:3102"
 	     (rst-re 'ilm-pfx '(:grp sym-tag "@" sym-tag ) 'ilm-sfx)
 	     (list "someone@example"
 		   (cons 2 1))
 	     (cons "^\\\\(" "\\(?:") ;; Make a group shy
 	     (cons (regexp-quote "\\(\\sw\\|\\s_\\)+")
-		   "\\(?:\\sw+\\(?:\\s_\\sw+\\)*\\)") ;; New syntax for symbols
+		   "\\(?:\\sw+\\(?:[-+.:_]\\sw+\\)*\\)") ;; New syntax for
+							 ;; symbols
 	     (cons (regexp-quote "\\(\\sw\\|\\s_\\)+")
-		   "\\(?:\\sw+\\(?:\\s_\\sw+\\)*\\)") ;; New syntax for symbols
+		   "\\(?:\\sw+\\(?:[-+.:_]\\sw+\\)*\\)") ;; New syntax for
+							 ;; symbols
 	     (cons (regexp-quote "\\|$") "")
 	     (cons (regexp-quote "\\([\t ]")
 		   "\\(?:$\\|[\t ]") ;; Move "$" in regex and make a group shy
 	     ))
     (should (re-equal
 	     ;; Sections_ / Transitions_
 	     re-ado2
```

### Comparing `docutils-0.9/tools/editors/emacs/tests/shift.el` & `docutils-0.9.1/tools/editors/emacs/tests/shift.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/support.el` & `docutils-0.9.1/tools/editors/emacs/tests/support.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/tests/toc.el` & `docutils-0.9.1/tools/editors/emacs/tests/toc.el`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/IDEAS.rst` & `docutils-0.9.1/tools/editors/emacs/IDEAS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -157,21 +157,43 @@
 * Imenu could be supported
 
   * See `(elisp)Imenu`
 
 Outline support
 ===============
 
-* Support for `outline-mode' / `allout-mode' would be nice
+* Support for `outline-mode` / `allout-mode` would be nice
 
   * Should consider section titles
 
-* May be folding is also possible
+    * May be item lists can also be included
 
-  * For item lists
+  * Using `allout-mode` is difficult
+
+    * It's not customizable enough for the complex syntax of
+      reStructuredText
+
+    * However, some commands make sense
+
+      * Motion commands
+
+      * Exposure commands
+
+      * Some alteration commands
+
+    * Should be reimplemented
+
+      * Key bindings need to be reused
+
+	* However, care must be taken if a file uses `allout-mode` for
+	  instance by comment strings
+
+	* In this case key bindings must not be overridden
+
+  * A command adding / updating `allout-mode` tags could be a solution
 
 Sophisticated filling
 =====================
 
 * These things must be filled special:
 
   * Definitions
```

### Comparing `docutils-0.9/tools/editors/emacs/README.txt` & `docutils-0.9.1/tools/editors/emacs/README.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/editors/emacs/rst.el` & `docutils-0.9.1/tools/editors/emacs/rst.el`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ;;; rst.el --- Mode for viewing and editing reStructuredText-documents.
 
 ;; Copyright (C) 2003-2012  Free Software Foundation, Inc.
 
 ;; Maintainer: Stefan Merten <smerten@oekonux.de>
-;; Author: Martin Blais <blais@furius.ca>,
+;; Author: Stefan Merten <smerten@oekonux.de>,
+;;         Martin Blais <blais@furius.ca>,
 ;;         David Goodger <goodger@python.org>,
 ;;         Wei-Wei Guo <wwguocn@gmail.com>
 
 ;; This file is part of GNU Emacs.
 
 ;; GNU Emacs is free software: you can redistribute it and/or modify
 ;; it under the terms of the GNU General Public License as published by
@@ -21,18 +22,18 @@
 
 ;; You should have received a copy of the GNU General Public License
 ;; along with GNU Emacs.  If not, see <http://www.gnu.org/licenses/>.
 
 ;;; Commentary:
 
 ;; This package provides major mode rst-mode, which supports documents marked
-;; up using the reStructuredText format. Support includes font locking as well
-;; as a lot of convenience functions for editing. It does this by defining a
-;; Emacs major mode: rst-mode (ReST). This mode is derived from text-mode. This
-;; package also contains:
+;; up using the reStructuredText format.  Support includes font locking as well
+;; as a lot of convenience functions for editing.  It does this by defining a
+;; Emacs major mode: rst-mode (ReST).  This mode is derived from text-mode.
+;; This package also contains:
 ;;
 ;; - Functions to automatically adjust and cycle the section underline
 ;;   adornments;
 ;; - A mode that displays the table of contents and allows you to jump anywhere
 ;;   from it;
 ;; - Functions to insert and automatically update a TOC in your source
 ;;   document;
@@ -49,32 +50,32 @@
 ;; For more information about reStructuredText, see
 ;; http://docutils.sourceforge.net/rst.html
 ;;
 ;; For full details on how to use the contents of this file, see
 ;; http://docutils.sourceforge.net/docs/user/emacs.html
 ;;
 ;;
-;; There are a number of convenient keybindings provided by rst-mode.
+;; There are a number of convenient key bindings provided by rst-mode.
 ;; For more on bindings, see rst-mode-map below.  There are also many variables
 ;; that can be customized, look for defcustom in this file.
 ;;
 ;; If you use the table-of-contents feature, you may want to add a hook to
-;; update the TOC automatically everytime you adjust a section title::
+;; update the TOC automatically every time you adjust a section title::
 ;;
 ;;   (add-hook 'rst-adjust-hook 'rst-toc-update)
 ;;
 ;; Syntax highlighting: font-lock is enabled by default.  If you want to turn
 ;; off syntax highlighting to rst-mode, you can use the following::
 ;;
 ;;   (setq font-lock-global-modes '(not rst-mode ...))
 ;;
 ;;
 ;;
 ;; Customization is done by customizable variables contained in customization
-;; group "rst" and subgroups. Group "rst" is contained in the "wp" group.
+;; group "rst" and subgroups.  Group "rst" is contained in the "wp" group.
 ;;
 
 ;;; DOWNLOAD
 
 ;; The latest release of this file lies in the docutils source code repository:
 ;;   http://docutils.svn.sourceforge.net/svnroot/docutils/trunk/docutils/tools/editors/emacs/rst.el
 
@@ -91,84 +92,136 @@
 ;;
 ;;    .. -*- mode: rst -*-
 ;;
 ;; in the very first line of your file.  The following code is useful if you
 ;; want automatically enter rst-mode from any file with compatible extensions:
 ;;
 ;; (setq auto-mode-alist
-;;       (append '(("\\.txt$" . rst-mode)
-;;                 ("\\.rst$" . rst-mode)
-;;                 ("\\.rest$" . rst-mode)) auto-mode-alist))
+;;       (append '(("\\.txt\\'" . rst-mode)
+;;                 ("\\.rst\\'" . rst-mode)
+;;                 ("\\.rest\\'" . rst-mode)) auto-mode-alist))
 ;;
 
 ;;; Code:
 
-(require 'cl)
+;; FIXME: When 24.1 is common place remove use of `lexical-let' and put "-*-
+;;        lexical-binding: t -*-" in the first line.
+
+;; Only use of macros is allowed - may be replaced by `cl-lib' some time.
+(eval-when-compile
+  (require 'cl))
+
+;; Redefine some functions from `cl.el' in a proper namespace until they may be
+;; used from there.
+
+(defun rst-signum (x)
+  "Return 1 if X is positive, -1 if negative, 0 if zero."
+  (cond
+   ((> x 0) 1)
+   ((< x 0) -1)
+   (t 0)))
+
+(defun rst-some (seq &optional pred)
+  "Return non-nil if any element of SEQ yields non-nil when PRED is applied.
+Apply PRED to each element of list SEQ until the first non-nil
+result is yielded and return this result. PRED defaults to
+`identity'."
+  (unless pred
+    (setq pred 'identity))
+  (catch 'rst-some
+    (dolist (elem seq)
+      (let ((r (funcall pred elem)))
+	(when r
+	  (throw 'rst-some r))))))
+
+(defun rst-position-if (pred seq)
+  "Return position of first element satisfying PRED in list SEQ or nil."
+  (catch 'rst-position-if
+    (let ((i 0))
+      (dolist (elem seq)
+	(when (funcall pred elem)
+	  (throw 'rst-position-if i))
+	(incf i)))))
+
+(defun rst-position (elem seq)
+  "Return position of ELEM in list SEQ or nil.
+Comparison done with `equal'."
+  ;; Create a closure containing `elem' so the `lambda' always sees our
+  ;; parameter instead of an `elem' which may be in dynamic scope at the time
+  ;; of execution of the `lambda'.
+  (lexical-let ((elem elem))
+    (rst-position-if (function (lambda (e)
+				 (equal elem e)))
+		     seq)))
+
+;; FIXME: Embed complicated `defconst's in `eval-when-compile'.
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Versions
 
 (defun rst-extract-version (delim-re head-re re tail-re var &optional default)
-  "Return the version matching RE after regex DELIM-RE and HEAD-RE
-and before TAIL-RE and DELIM-RE in VAR or DEFAULT for no match"
+  "Extract the version from a variable according to the given regexes.
+Return the version after regex DELIM-RE and HEAD-RE matching RE
+and before TAIL-RE and DELIM-RE in VAR or DEFAULT for no match."
   (if (string-match
        (concat delim-re head-re "\\(" re "\\)" tail-re delim-re)
        var)
       (match-string 1 var)
     default))
 
 ;; Use CVSHeader to really get information from CVS and not other version
-;; control systems
+;; control systems.
 (defconst rst-cvs-header
-  "$CVSHeader: sm/rst_el/rst.el,v 1.256 2012-04-29 15:00:50 stefan Exp $")
+  "$CVSHeader: sm/rst_el/rst.el,v 1.286 2012-06-16 09:41:21 stefan Exp $")
 (defconst rst-cvs-rev
   (rst-extract-version "\\$" "CVSHeader: \\S + " "[0-9]+\\(?:\\.[0-9]+\\)+"
 		       " .*" rst-cvs-header "0.0")
-  "The CVS revision of this file. CVS revision is the development revision.")
+  "The CVS revision of this file.  CVS revision is the development revision.")
 (defconst rst-cvs-timestamp
   (rst-extract-version "\\$" "CVSHeader: \\S + \\S + "
 		       "[0-9]+-[0-9]+-[0-9]+ [0-9]+:[0-9]+:[0-9]+" " .*"
 		       rst-cvs-header "1970-01-01 00:00:00")
-  "The CVS timestamp of this file.")
+  "The CVS time stamp of this file.")
 
-;; Use LastChanged... to really get information from SVN
+;; Use LastChanged... to really get information from SVN.
 (defconst rst-svn-rev
   (rst-extract-version "\\$" "LastChangedRevision: " "[0-9]+" " "
-		       "$LastChangedRevision: 7399 $")
+		       "$LastChangedRevision: 7444 $")
   "The SVN revision of this file.
 SVN revision is the upstream (docutils) revision.")
 (defconst rst-svn-timestamp
   (rst-extract-version "\\$" "LastChangedDate: " ".+?+" " "
-		       "$LastChangedDate: 2012-04-29 17:01:05 +0200 (Son, 29 Apr 2012) $")
-  "The SVN timestamp of this file.")
+		       "$LastChangedDate: 2012-06-16 11:41:40 +0200 (Sam, 16 Jun 2012) $")
+  "The SVN time stamp of this file.")
 
-;; Maintained by the release process
+;; Maintained by the release process.
 (defconst rst-official-version
   (rst-extract-version "%" "OfficialVersion: " "[0-9]+\\(?:\\.[0-9]+\\)+" " "
-		       "%OfficialVersion: 1.2.1 %")
+		       "%OfficialVersion: 1.3.0 %")
   "Official version of the package.")
 (defconst rst-official-cvs-rev
   (rst-extract-version "[%$]" "Revision: " "[0-9]+\\(?:\\.[0-9]+\\)+" " "
-		       "%Revision: 1.256 %")
+		       "$Revision: 7444 $")
   "CVS revision of this file in the official version.")
 
 (defconst rst-version
   (if (equal rst-official-cvs-rev rst-cvs-rev)
       rst-official-version
     (format "%s (development %s [%s])" rst-official-version
 	    rst-cvs-rev rst-cvs-timestamp))
   "The version string.
-Starts with the current official version. For developer versions
-in parentheses follows the development revision and the timestamp.")
+Starts with the current official version.  For developer versions
+in parentheses follows the development revision and the time stamp.")
 
 (defconst rst-package-emacs-version-alist
-  '(("1.0.0" . "24.0")
-    ("1.1.0" . "24.0")
-    ("1.2.0" . "24.0")
-    ("1.2.1" . "24.0")))
+  '(("1.0.0" . "24.2")
+    ("1.1.0" . "24.2")
+    ("1.2.0" . "24.2")
+    ("1.2.1" . "24.2")
+    ("1.3.0" . "24.2")))
 
 (unless (assoc rst-official-version rst-package-emacs-version-alist)
   (error "Version %s not listed in `rst-package-emacs-version-alist'"
 	 rst-version))
 
 (add-to-list 'customize-package-emacs-version-alist
 	     (cons 'ReST rst-package-emacs-version-alist))
@@ -183,287 +236,289 @@
   :link '(url-link "http://docutils.sourceforge.net/rst.html"))
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Facilities for regular expressions used everywhere
 
 ;; The trailing numbers in the names give the number of referenceable regex
-;; groups contained in the regex
+;; groups contained in the regex.
 
 ;; Used to be customizable but really is not customizable but fixed by the reST
-;; syntax
+;; syntax.
 (defconst rst-bullets
-  ;; Sorted so they can form a character class when concatenated
+  ;; Sorted so they can form a character class when concatenated.
   '(?- ?* ?+ ?\u2022 ?\u2023 ?\u2043)
   "List of all possible bullet characters for bulleted lists.")
 
 (defconst rst-uri-schemes
   '("acap" "cid" "data" "dav" "fax" "file" "ftp" "gopher" "http" "https" "imap"
     "ldap" "mailto" "mid" "modem" "news" "nfs" "nntp" "pop" "prospero" "rtsp"
     "service" "sip" "tel" "telnet" "tip" "urn" "vemmi" "wais")
   "Supported URI schemes.")
 
 (defconst rst-adornment-chars
-  ;; Sorted so they can form a character class when concatenated
+  ;; Sorted so they can form a character class when concatenated.
   '(?\]
     ?! ?\" ?# ?$ ?% ?& ?' ?\( ?\) ?* ?+ ?, ?. ?/ ?: ?\; ?< ?= ?> ?? ?@ ?\[ ?\\
     ?^ ?_ ?` ?{ ?| ?} ?~
     ?-)
   "Characters which may be used in adornments for sections and transitions.")
 
 (defconst rst-max-inline-length
   1000
   "Maximum length of inline markup to recognize.")
 
 (defconst rst-re-alist-def
-  ;; `*-beg' matches * at the beginning of a line
-  ;; `*-end' matches * at the end of a line
-  ;; `*-prt' matches a part of *
-  ;; `*-tag' matches *
-  ;; `*-sta' matches the start of * which may be followed by respective content
-  ;; `*-pfx' matches the delimiter left of *
-  ;; `*-sfx' matches the delimiter right of *
-  ;; `*-hlp' helper for *
+  ;; `*-beg' matches * at the beginning of a line.
+  ;; `*-end' matches * at the end of a line.
+  ;; `*-prt' matches a part of *.
+  ;; `*-tag' matches *.
+  ;; `*-sta' matches the start of * which may be followed by respective content.
+  ;; `*-pfx' matches the delimiter left of *.
+  ;; `*-sfx' matches the delimiter right of *.
+  ;; `*-hlp' helper for *.
   ;;
   ;; A trailing number says how many referenceable groups are contained.
   `(
 
     ;; Horizontal white space (`hws')
     (hws-prt "[\t ]")
-    (hws-tag hws-prt "*") ; Optional sequence of horizontal white space
-    (hws-sta hws-prt "+") ; Mandatory sequence of horizontal white space
+    (hws-tag hws-prt "*") ; Optional sequence of horizontal white space.
+    (hws-sta hws-prt "+") ; Mandatory sequence of horizontal white space.
 
     ;; Lines (`lin')
-    (lin-beg "^" hws-tag) ; Beginning of a possibly indented line
-    (lin-end hws-tag "$") ; End of a line with optional trailing white space
-    (linemp-tag "^" hws-tag "$") ; Empty line with optional white space
+    (lin-beg "^" hws-tag) ; Beginning of a possibly indented line.
+    (lin-end hws-tag "$") ; End of a line with optional trailing white space.
+    (linemp-tag "^" hws-tag "$") ; Empty line with optional white space.
 
     ;; Various tags and parts
     (ell-tag "\\.\\.\\.") ; Ellipsis
-    (bul-tag ,(concat "[" rst-bullets "]")) ; A bullet
-    (ltr-tag "[a-zA-Z]") ; A letter enumerator tag
-    (num-prt "[0-9]") ; A number enumerator part
-    (num-tag num-prt "+") ; A number enumerator tag
-    (rom-prt "[IVXLCDMivxlcdm]") ; A roman enumerator part
-    (rom-tag rom-prt "+") ; A roman enumerator tag
-    (aut-tag "#") ; An automatic enumerator tag
-    (dcl-tag "::") ; Double colon
+    (bul-tag ,(concat "[" rst-bullets "]")) ; A bullet.
+    (ltr-tag "[a-zA-Z]") ; A letter enumerator tag.
+    (num-prt "[0-9]") ; A number enumerator part.
+    (num-tag num-prt "+") ; A number enumerator tag.
+    (rom-prt "[IVXLCDMivxlcdm]") ; A roman enumerator part.
+    (rom-tag rom-prt "+") ; A roman enumerator tag.
+    (aut-tag "#") ; An automatic enumerator tag.
+    (dcl-tag "::") ; Double colon.
 
     ;; Block lead in (`bli')
     (bli-sfx (:alt hws-sta "$")) ; Suffix of a block lead-in with *optional*
-				 ; immediate content
+				 ; immediate content.
 
     ;; Various starts
-    (bul-sta bul-tag bli-sfx) ; Start of a bulleted item
+    (bul-sta bul-tag bli-sfx) ; Start of a bulleted item.
 
     ;; Explicit markup tag (`exm')
     (exm-tag "\\.\\.")
     (exm-sta exm-tag hws-sta)
     (exm-beg lin-beg exm-sta)
 
     ;; Counters in enumerations (`cnt')
-    (cntany-tag (:alt ltr-tag num-tag rom-tag aut-tag)) ; An arbitrary counter
-    (cntexp-tag (:alt ltr-tag num-tag rom-tag)) ; An arbitrary explicit counter
+    (cntany-tag (:alt ltr-tag num-tag rom-tag aut-tag)) ; An arbitrary counter.
+    (cntexp-tag (:alt ltr-tag num-tag rom-tag)) ; An arbitrary explicit counter.
 
     ;; Enumerator (`enm')
     (enmany-tag (:alt
 		 (:seq cntany-tag "\\.")
-		 (:seq "(?" cntany-tag ")"))) ; An arbitrary enumerator
+		 (:seq "(?" cntany-tag ")"))) ; An arbitrary enumerator.
     (enmexp-tag (:alt
 		 (:seq cntexp-tag "\\.")
 		 (:seq "(?" cntexp-tag ")"))) ; An arbitrary explicit
-					      ; enumerator
+					      ; enumerator.
     (enmaut-tag (:alt
 		 (:seq aut-tag "\\.")
-		 (:seq "(?" aut-tag ")"))) ; An automatic enumerator
-    (enmany-sta enmany-tag bli-sfx) ; An arbitrary enumerator start
-    (enmexp-sta enmexp-tag bli-sfx) ; An arbitrary explicit enumerator start
+		 (:seq "(?" aut-tag ")"))) ; An automatic enumerator.
+    (enmany-sta enmany-tag bli-sfx) ; An arbitrary enumerator start.
+    (enmexp-sta enmexp-tag bli-sfx) ; An arbitrary explicit enumerator start.
     (enmexp-beg lin-beg enmexp-sta) ; An arbitrary explicit enumerator start
-				    ; at the beginning of a line
+				    ; at the beginning of a line.
 
     ;; Items may be enumerated or bulleted (`itm')
-    (itmany-tag (:alt enmany-tag bul-tag)) ; An arbitrary item tag
+    (itmany-tag (:alt enmany-tag bul-tag)) ; An arbitrary item tag.
     (itmany-sta-1 (:grp itmany-tag) bli-sfx) ; An arbitrary item start, group
-					     ; is the item tag
+					     ; is the item tag.
     (itmany-beg-1 lin-beg itmany-sta-1) ; An arbitrary item start at the
 				        ; beginning of a line, group is the
-				        ; item tag
+				        ; item tag.
 
     ;; Inline markup (`ilm')
     (ilm-pfx (:alt "^" hws-prt "[-'\"([{<\u2018\u201c\u00ab\u2019/:]"))
     (ilm-sfx (:alt "$" hws-prt "[]-'\")}>\u2019\u201d\u00bb/:.,;!?\\]"))
 
     ;; Inline markup content (`ilc')
-    (ilcsgl-tag "\\S ") ; A single non-white character
-    (ilcast-prt (:alt "[^*\\]" "\\\\.")) ; Part of non-asterisk content
-    (ilcbkq-prt (:alt "[^`\\]" "\\\\.")) ; Part of non-backquote content
+    (ilcsgl-tag "\\S ") ; A single non-white character.
+    (ilcast-prt (:alt "[^*\\]" "\\\\.")) ; Part of non-asterisk content.
+    (ilcbkq-prt (:alt "[^`\\]" "\\\\.")) ; Part of non-backquote content.
     (ilcbkqdef-prt (:alt "[^`\\\n]" "\\\\.")) ; Part of non-backquote
-					      ; definition
-    (ilcbar-prt (:alt "[^|\\]" "\\\\.")) ; Part of non-vertical-bar content
+					      ; definition.
+    (ilcbar-prt (:alt "[^|\\]" "\\\\.")) ; Part of non-vertical-bar content.
     (ilcbardef-prt (:alt "[^|\\\n]" "\\\\.")) ; Part of non-vertical-bar
-					      ; definition
-    (ilcast-sfx "[^\t *\\]") ; Suffix of non-asterisk content
-    (ilcbkq-sfx "[^\t `\\]") ; Suffix of non-backquote content
-    (ilcbar-sfx "[^\t |\\]") ; Suffix of non-vertical-bar content
-    (ilcrep-hlp ,(format "\\{0,%d\\}" rst-max-inline-length)) ; Repeat count
+					      ; definition.
+    (ilcast-sfx "[^\t *\\]") ; Suffix of non-asterisk content.
+    (ilcbkq-sfx "[^\t `\\]") ; Suffix of non-backquote content.
+    (ilcbar-sfx "[^\t |\\]") ; Suffix of non-vertical-bar content.
+    (ilcrep-hlp ,(format "\\{0,%d\\}" rst-max-inline-length)) ; Repeat count.
     (ilcast-tag (:alt ilcsgl-tag
 		      (:seq ilcsgl-tag
 			    ilcast-prt ilcrep-hlp
-			    ilcast-sfx))) ; Non-asterisk content
+			    ilcast-sfx))) ; Non-asterisk content.
     (ilcbkq-tag (:alt ilcsgl-tag
 		      (:seq ilcsgl-tag
 			    ilcbkq-prt ilcrep-hlp
-			    ilcbkq-sfx))) ; Non-backquote content
+			    ilcbkq-sfx))) ; Non-backquote content.
     (ilcbkqdef-tag (:alt ilcsgl-tag
 			 (:seq ilcsgl-tag
 			       ilcbkqdef-prt ilcrep-hlp
-			       ilcbkq-sfx))) ; Non-backquote definition
+			       ilcbkq-sfx))) ; Non-backquote definition.
     (ilcbar-tag (:alt ilcsgl-tag
 		      (:seq ilcsgl-tag
 			    ilcbar-prt ilcrep-hlp
-			    ilcbar-sfx))) ; Non-vertical-bar content
+			    ilcbar-sfx))) ; Non-vertical-bar content.
     (ilcbardef-tag (:alt ilcsgl-tag
 			 (:seq ilcsgl-tag
 			       ilcbardef-prt ilcrep-hlp
-			       ilcbar-sfx))) ; Non-vertical-bar definition
+			       ilcbar-sfx))) ; Non-vertical-bar definition.
 
     ;; Fields (`fld')
-    (fldnam-prt (:alt "[^:\n]" "\\\\:")) ; Part of a field name
-    (fldnam-tag fldnam-prt "+") ; A field name
-    (fld-tag ":" fldnam-tag ":") ; A field marker
+    (fldnam-prt (:alt "[^:\n]" "\\\\:")) ; Part of a field name.
+    (fldnam-tag fldnam-prt "+") ; A field name.
+    (fld-tag ":" fldnam-tag ":") ; A field marker.
 
     ;; Options (`opt')
-    (optsta-tag (:alt "[-+/]" "--")) ; Start of an option
-    (optnam-tag "\\sw" (:alt "-" "\\sw") "*") ; Name of an option
-    (optarg-tag (:shy "[ =]\\S +")) ; Option argument
-    (optsep-tag (:shy "," hws-prt)) ; Separator between options
-    (opt-tag (:shy optsta-tag optnam-tag optarg-tag "?")) ; A complete option
+    (optsta-tag (:alt "[-+/]" "--")) ; Start of an option.
+    (optnam-tag "\\sw" (:alt "-" "\\sw") "*") ; Name of an option.
+    (optarg-tag (:shy "[ =]\\S +")) ; Option argument.
+    (optsep-tag (:shy "," hws-prt)) ; Separator between options.
+    (opt-tag (:shy optsta-tag optnam-tag optarg-tag "?")) ; A complete option.
 
     ;; Footnotes and citations (`fnc')
-    (fncnam-prt "[^\]\n]") ; Part of a footnote or citation name
-    (fncnam-tag fncnam-prt "+") ; A footnote or citation name
-    (fnc-tag "\\[" fncnam-tag "]") ; A complete footnote or citation tag
+    (fncnam-prt "[^\]\n]") ; Part of a footnote or citation name.
+    (fncnam-tag fncnam-prt "+") ; A footnote or citation name.
+    (fnc-tag "\\[" fncnam-tag "]") ; A complete footnote or citation tag.
     (fncdef-tag-2 (:grp exm-sta)
 		  (:grp fnc-tag)) ; A complete footnote or citation definition
-				  ; tag; first group is the explicit markup
+				  ; tag.  First group is the explicit markup
 				  ; start, second group is the footnote /
-				  ; citation tag
+				  ; citation tag.
     (fnc-sta-2 fncdef-tag-2 bli-sfx) ; Start of a footnote or citation
-				     ; definition; first group is the explicit
+				     ; definition.  First group is the explicit
 				     ; markup start, second group is the
-				     ; footnote / citation tag
+				     ; footnote / citation tag.
 
     ;; Substitutions (`sub')
-    (sub-tag "|" ilcbar-tag "|") ; A complete substitution tag
+    (sub-tag "|" ilcbar-tag "|") ; A complete substitution tag.
     (subdef-tag "|" ilcbardef-tag "|") ; A complete substitution definition
-				       ; tag
+				       ; tag.
 
     ;; Symbol (`sym')
-    (sym-tag (:shy "\\sw+" (:shy "\\s_\\sw+") "*"))
+    (sym-prt "[-+.:_]") ; Non-word part of a symbol.
+    (sym-tag (:shy "\\sw+" (:shy sym-prt "\\sw+") "*"))
 
     ;; URIs (`uri')
     (uri-tag (:alt ,@rst-uri-schemes))
 
     ;; Adornment (`ado')
     (ado-prt "[" ,(concat rst-adornment-chars) "]")
     (adorep3-hlp "\\{3,\\}") ; There must be at least 3 characters because
 			     ; otherwise explicit markup start would be
-			     ; recognized
+			     ; recognized.
     (adorep2-hlp "\\{2,\\}") ; As `adorep3-hlp' but when the first of three
-			     ; characters is matched differently
+			     ; characters is matched differently.
     (ado-tag-1-1 (:grp ado-prt)
 		 "\\1" adorep2-hlp) ; A complete adornment, group is the first
 				    ; adornment character and MUST be the FIRST
-				    ; group in the whole expression
+				    ; group in the whole expression.
     (ado-tag-1-2 (:grp ado-prt)
 		 "\\2" adorep2-hlp) ; A complete adornment, group is the first
 				    ; adornment character and MUST be the
-				    ; SECOND group in the whole expression
+				    ; SECOND group in the whole expression.
     (ado-beg-2-1 "^" (:grp ado-tag-1-2)
 		 lin-end) ; A complete adornment line; first group is the whole
 			  ; adornment and MUST be the FIRST group in the whole
 			  ; expression; second group is the first adornment
-			  ; character
+			  ; character.
 
     ;; Titles (`ttl')
-    (ttl-tag "\\S *\\w\\S *") ; A title text
-    (ttl-beg lin-beg ttl-tag) ; A title text at the beginning of a line
+    (ttl-tag "\\S *\\w\\S *") ; A title text.
+    (ttl-beg lin-beg ttl-tag) ; A title text at the beginning of a line.
 
     ;; Directives and substitution definitions (`dir')
     (dir-tag-3 (:grp exm-sta)
 	       (:grp (:shy subdef-tag hws-sta) "?")
 	       (:grp sym-tag dcl-tag)) ; A directive or substitution definition
-				       ; tag; first group is explicit markup
+				       ; tag.  First group is explicit markup
 				       ; start, second group is a possibly
 				       ; empty substitution tag, third group is
 				       ; the directive tag including the double
-				       ; colon
+				       ; colon.
     (dir-sta-3 dir-tag-3 bli-sfx) ; Start of a directive or substitution
-				  ; definition; groups are as in dir-tag-3
+				  ; definition.  Groups are as in dir-tag-3.
 
     ;; Literal block (`lit')
     (lit-sta-2 (:grp (:alt "[^.\n]" "\\.[^.\n]") ".*") "?"
-	       (:grp dcl-tag) "$") ; Start of a literal block; first group is
+	       (:grp dcl-tag) "$") ; Start of a literal block.  First group is
 				   ; any text before the double colon tag which
 				   ; may not exist, second group is the double
-				   ; colon tag
+				   ; colon tag.
 
     ;; Comments (`cmt')
     (cmt-sta-1 (:grp exm-sta) "[^\[|_\n]"
 	       (:alt "[^:\n]" (:seq ":" (:alt "[^:\n]" "$")))
 	       "*$") ; Start of a comment block; first group is explicit markup
-		     ; start
+		     ; start.
 
     ;; Paragraphs (`par')
     (par-tag- (:alt itmany-tag fld-tag opt-tag fncdef-tag-2 dir-tag-3 exm-tag)
 	      ) ; Tag at the beginning of a paragraph; there may be groups in
-		; certain cases
+		; certain cases.
     )
   "Definition alist of relevant regexes.
 Each entry consists of the symbol naming the regex and an
 argument list for `rst-re'.")
 
-;; FIXME: Use `sregex` or `rx` instead of re-inventing the wheel
+(defvar rst-re-alist) ; Forward declare to use it in `rst-re'.
+
+;; FIXME: Use `sregex` or `rx` instead of re-inventing the wheel.
 (defun rst-re (&rest args)
   "Interpret ARGS as regular expressions and return a regex string.
 Each element of ARGS may be one of the following:
 
 A string which is inserted unchanged.
 
 A character which is resolved to a quoted regex.
 
 A symbol which is resolved to a string using `rst-re-alist-def'.
 
-A list with a keyword in the car. Each element of the cdr of such
-a list is recursively interpreted as ARGS. The results of this
+A list with a keyword in the car.  Each element of the cdr of such
+a list is recursively interpreted as ARGS.  The results of this
 interpretation are concatenated according to the keyword.
 
 For the keyword `:seq' the results are simply concatenated.
 
 For the keyword `:shy' the results are concatenated and
 surrounded by a shy-group (\"\\(?:...\\)\").
 
 For the keyword `:alt' the results form an alternative (\"\\|\")
 which is shy-grouped (\"\\(?:...\\)\").
 
 For the keyword `:grp' the results are concatenated and form a
-referencable grouped (\"\\(...\\)\").
+referenceable group (\"\\(...\\)\").
 
 After interpretation of ARGS the results are concatenated as for
-`:seq'.
-"
+`:seq'."
   (apply 'concat
 	 (mapcar
 	  (lambda (re)
 	    (cond
 	     ((stringp re)
 	      re)
 	     ((symbolp re)
 	      (cadr (assoc re rst-re-alist)))
-	     ((char-valid-p re)
+	     ((characterp re)
 	      (regexp-quote (char-to-string re)))
 	     ((listp re)
 	      (let ((nested
 		     (mapcar (lambda (elt)
 			       (rst-re elt))
 			     (cdr re))))
 		(cond
@@ -477,154 +532,138 @@
 		  (concat "\\(?:" (mapconcat 'identity nested "\\|") "\\)"))
 		 (t
 		  (error "Unknown list car: %s" (car re))))))
 	     (t
 	      (error "Unknown object type for building regex: %s" re))))
 	  args)))
 
-(defconst rst-re-alist
-  ;; Shadow global value we are just defining so we can construct it step by
-  ;; step
-  (let (rst-re-alist)
-    (dolist (re rst-re-alist-def)
-      (setq rst-re-alist
-	    (nconc rst-re-alist
-		   (list (list (car re) (apply 'rst-re (cdr re)))))))
-    rst-re-alist)
-  "Alist mapping symbols from `rst-re-alist-def' to regex strings.")
+;; FIXME: Remove circular dependency between `rst-re' and `rst-re-alist'.
+(with-no-warnings ; Silence byte-compiler about this construction.
+  (defconst rst-re-alist
+    ;; Shadow global value we are just defining so we can construct it step by
+    ;; step.
+    (let (rst-re-alist)
+      (dolist (re rst-re-alist-def rst-re-alist)
+	(setq rst-re-alist
+	      (nconc rst-re-alist
+		     (list (list (car re) (apply 'rst-re (cdr re))))))))
+    "Alist mapping symbols from `rst-re-alist-def' to regex strings."))
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
-;; Mode definition.
-
-(defvar rst-deprecated-keys nil
-  "Alist mapping deprecated keys to the new key to use and the definition.")
-
-(require 'edmacro)
-
-(defun rst-call-deprecated ()
-  (interactive)
-  (let* ((dep-key (this-command-keys-vector))
-	 (dep-key-s (format-kbd-macro dep-key))
-	 (fnd (assoc dep-key rst-deprecated-keys)))
-    (if (not fnd)
-	;; Exact key sequence not found. Maybe a deprecated key sequence has
-	;; been followed by another key.
-	(let* ((dep-key-pfx (butlast (append dep-key nil) 1))
-	       (dep-key-def (vconcat dep-key-pfx '(t)))
-	       (fnd-def (assoc dep-key-def rst-deprecated-keys)))
-	  (if (not fnd-def)
-	      (error "Unknown deprecated key sequence %s" dep-key-s)
-	    ;; Don't execute the command in this case
-	    (message "[Deprecated use of key %s; use key %s instead]"
-		     (format-kbd-macro dep-key-pfx)
-		     (format-kbd-macro (second fnd-def)))))
-      (message "[Deprecated use of key %s; use key %s instead]"
-	       dep-key-s (format-kbd-macro (second fnd)))
-      (call-interactively (third fnd)))))
+;; Mode definition
 
 (defun rst-define-key (keymap key def &rest deprecated)
-  "Bind like `define-key' using DEPRECATED as deprecated key definitions.
-DEPRECATED key definitions should be in vector notation. These
-are defined as well but give an additional message."
+  "Bind like `define-key' but add deprecated key definitions.
+KEYMAP, KEY, and DEF are as in `define-key'.  DEPRECATED key
+definitions should be in vector notation.  These are defined as
+well but give an additional message."
   (define-key keymap key def)
   (dolist (dep-key deprecated)
-    (push (list dep-key key def) rst-deprecated-keys)
-    (define-key keymap dep-key 'rst-call-deprecated)))
+    (define-key keymap dep-key
+      `(lambda ()
+         ,(format "Deprecated binding for %s, use \\[%s] instead." def def)
+	 (interactive)
+	 (call-interactively ',def)
+	 (message "[Deprecated use of key %s; use key %s instead]"
+		  (key-description (this-command-keys))
+		  (key-description ,key))))))
 
 ;; Key bindings.
 (defvar rst-mode-map
   (let ((map (make-sparse-keymap)))
 
-    ;; \C-c is the general keymap
+    ;; \C-c is the general keymap.
     (rst-define-key map [?\C-c ?\C-h] 'describe-prefix-bindings)
 
     ;;
-    ;; Section Adornments.
+    ;; Section Adornments
     ;;
     ;; The adjustment function that adorns or rotates a section title.
     (rst-define-key map [?\C-c ?\C-=] 'rst-adjust [?\C-c ?\C-a t])
     (rst-define-key map [?\C-=] 'rst-adjust) ; (Does not work on the Mac OSX.)
 
-    ;; \C-c \C-a is the keymap for adornments
+    ;; \C-c \C-a is the keymap for adornments.
     (rst-define-key map [?\C-c ?\C-a ?\C-h] 'describe-prefix-bindings)
-    ;; Display the hierarchy of adornments implied by the current document contents.
+    ;; Display the hierarchy of adornments implied by the current document
+    ;; contents.
     (rst-define-key map [?\C-c ?\C-a ?\C-d] 'rst-display-adornments-hierarchy)
     ;; Homogenize the adornments in the document.
     (rst-define-key map [?\C-c ?\C-a ?\C-s] 'rst-straighten-adornments
 		    [?\C-c ?\C-s])
 
     ;;
-    ;; Section Movement and Selection.
+    ;; Section Movement and Selection
     ;;
     ;; Mark the subsection where the cursor is.
     (rst-define-key map [?\C-\M-h] 'rst-mark-section
-		    ;; same as mark-defun sgml-mark-current-element
+		    ;; Same as mark-defun sgml-mark-current-element.
 		    [?\C-c ?\C-m])
-    ;; Move forward/backward between section titles.
-    (rst-define-key map [?\C-\M-a] 'rst-forward-section
-		    ;; same as beginning-of-defun
+    ;; Move backward/forward between section titles.
+    ;; FIXME: Also bind similar to outline mode.
+    (rst-define-key map [?\C-\M-a] 'rst-backward-section
+		    ;; Same as beginning-of-defun.
 		    [?\C-c ?\C-n])
-    (rst-define-key map [?\C-\M-e] 'rst-backward-section
-		    ;; same as end-of-defun
+    (rst-define-key map [?\C-\M-e] 'rst-forward-section
+		    ;; Same as end-of-defun.
 		    [?\C-c ?\C-p])
 
     ;;
-    ;; Operating on regions.
+    ;; Operating on regions
     ;;
-    ;; \C-c \C-r is the keymap for regions
+    ;; \C-c \C-r is the keymap for regions.
     (rst-define-key map [?\C-c ?\C-r ?\C-h] 'describe-prefix-bindings)
     ;; Makes region a line-block.
     (rst-define-key map [?\C-c ?\C-r ?\C-l] 'rst-line-block-region
 		    [?\C-c ?\C-d])
-    ;; Shift region left or right according to tabs
+    ;; Shift region left or right according to tabs.
     (rst-define-key map [?\C-c ?\C-r tab] 'rst-shift-region
 		    [?\C-c ?\C-r t] [?\C-c ?\C-l t])
 
     ;;
-    ;; Operating on lists.
+    ;; Operating on lists
     ;;
-    ;; \C-c \C-l is the keymap for lists
+    ;; \C-c \C-l is the keymap for lists.
     (rst-define-key map [?\C-c ?\C-l ?\C-h] 'describe-prefix-bindings)
     ;; Makes paragraphs in region as a bullet list.
     (rst-define-key map [?\C-c ?\C-l ?\C-b] 'rst-bullet-list-region
 		    [?\C-c ?\C-b])
     ;; Makes paragraphs in region as a enumeration.
     (rst-define-key map [?\C-c ?\C-l ?\C-e] 'rst-enumerate-region
 		    [?\C-c ?\C-e])
     ;; Converts bullets to an enumeration.
     (rst-define-key map [?\C-c ?\C-l ?\C-c] 'rst-convert-bullets-to-enumeration
 		    [?\C-c ?\C-v])
     ;; Make sure that all the bullets in the region are consistent.
     (rst-define-key map [?\C-c ?\C-l ?\C-s] 'rst-straighten-bullets-region
 		    [?\C-c ?\C-w])
-    ;; Insert a list item
+    ;; Insert a list item.
     (rst-define-key map [?\C-c ?\C-l ?\C-i] 'rst-insert-list)
 
     ;;
-    ;; Table-of-Contents Features.
+    ;; Table-of-Contents Features
     ;;
-    ;; \C-c \C-t is the keymap for table of contents
+    ;; \C-c \C-t is the keymap for table of contents.
     (rst-define-key map [?\C-c ?\C-t ?\C-h] 'describe-prefix-bindings)
     ;; Enter a TOC buffer to view and move to a specific section.
     (rst-define-key map [?\C-c ?\C-t ?\C-t] 'rst-toc)
     ;; Insert a TOC here.
     (rst-define-key map [?\C-c ?\C-t ?\C-i] 'rst-toc-insert
 		    [?\C-c ?\C-i])
     ;; Update the document's TOC (without changing the cursor position).
     (rst-define-key map [?\C-c ?\C-t ?\C-u] 'rst-toc-update
 		    [?\C-c ?\C-u])
-    ;; Got to the section under the cursor (cursor must be in TOC).
+    ;; Go to the section under the cursor (cursor must be in TOC).
     (rst-define-key map [?\C-c ?\C-t ?\C-j] 'rst-goto-section
 		    [?\C-c ?\C-f])
 
     ;;
-    ;; Converting Documents from Emacs.
+    ;; Converting Documents from Emacs
     ;;
-    ;; \C-c \C-c is the keymap for compilation
+    ;; \C-c \C-c is the keymap for compilation.
     (rst-define-key map [?\C-c ?\C-c ?\C-h] 'describe-prefix-bindings)
     ;; Run one of two pre-configured toolset commands on the document.
     (rst-define-key map [?\C-c ?\C-c ?\C-c] 'rst-compile
 		    [?\C-c ?1])
     (rst-define-key map [?\C-c ?\C-c ?\C-a] 'rst-compile-alt-toolset
 		    [?\C-c ?2])
     ;; Convert the active region to pseudo-xml using the docutils tools.
@@ -639,46 +678,43 @@
 
     map)
   "Keymap for reStructuredText mode commands.
 This inherits from Text mode.")
 
 
 ;; Abbrevs.
-(defvar rst-mode-abbrev-table nil
-  "Abbrev table used while in `rst-mode'.")
 (define-abbrev-table 'rst-mode-abbrev-table
   (mapcar (lambda (x) (append x '(nil 0 system)))
           '(("contents" ".. contents::\n..\n   ")
             ("con" ".. contents::\n..\n   ")
             ("cont" "[...]")
             ("skip" "\n\n[...]\n\n  ")
             ("seq" "\n\n[...]\n\n  ")
             ;; FIXME: Add footnotes, links, and more.
-            )))
+            ))
+  "Abbrev table used while in `rst-mode'.")
 
 
 ;; Syntax table.
 (defvar rst-mode-syntax-table
   (let ((st (copy-syntax-table text-mode-syntax-table)))
-
     (modify-syntax-entry ?$ "." st)
     (modify-syntax-entry ?% "." st)
     (modify-syntax-entry ?& "." st)
     (modify-syntax-entry ?' "." st)
     (modify-syntax-entry ?* "." st)
-    (modify-syntax-entry ?+ "_" st)
-    (modify-syntax-entry ?. "_" st)
+    (modify-syntax-entry ?+ "." st)
+    (modify-syntax-entry ?- "." st)
     (modify-syntax-entry ?/ "." st)
-    (modify-syntax-entry ?: "_" st)
     (modify-syntax-entry ?< "." st)
     (modify-syntax-entry ?= "." st)
     (modify-syntax-entry ?> "." st)
     (modify-syntax-entry ?\\ "\\" st)
+    (modify-syntax-entry ?_ "." st)
     (modify-syntax-entry ?| "." st)
-    (modify-syntax-entry ?_ "_" st)
     (modify-syntax-entry ?\u00ab "." st)
     (modify-syntax-entry ?\u00bb "." st)
     (modify-syntax-entry ?\u2018 "." st)
     (modify-syntax-entry ?\u2019 "." st)
     (modify-syntax-entry ?\u201c "." st)
     (modify-syntax-entry ?\u201d "." st)
 
@@ -688,14 +724,16 @@
 
 (defcustom rst-mode-hook nil
   "Hook run when `rst-mode' is turned on.
 The hook for `text-mode' is run before this one."
   :group 'rst
   :type '(hook))
 
+;; Pull in variable definitions silencing byte-compiler.
+(require 'newcomment)
 
 ;; Use rst-mode for *.rst and *.rest files.  Many ReStructured-Text files
 ;; use *.txt, but this is too generic to be set as a default.
 ;;;###autoload (add-to-list 'auto-mode-alist (purecopy '("\\.re?st\\'" . rst-mode)))
 ;;;###autoload
 (define-derived-mode rst-mode text-mode "ReST"
   "Major mode for editing reStructuredText documents.
@@ -706,71 +744,67 @@
 highlighting.
 
 \\{rst-mode-map}"
   :abbrev-table rst-mode-abbrev-table
   :syntax-table rst-mode-syntax-table
   :group 'rst
 
-  ;; Paragraph recognition
+  ;; Paragraph recognition.
   (set (make-local-variable 'paragraph-separate)
        (rst-re '(:alt
 		 "\f"
 		 lin-end)))
   (set (make-local-variable 'paragraph-start)
        (rst-re '(:alt
 		 "\f"
 		 lin-end
 		 (:seq hws-tag par-tag- bli-sfx))))
 
-  ;; Indenting and filling
+  ;; Indenting and filling.
   (set (make-local-variable 'indent-line-function) 'rst-indent-line)
   (set (make-local-variable 'adaptive-fill-mode) t)
   (set (make-local-variable 'adaptive-fill-regexp)
        (rst-re 'hws-tag 'par-tag- "?" 'hws-tag))
   (set (make-local-variable 'adaptive-fill-function) 'rst-adaptive-fill)
   (set (make-local-variable 'fill-paragraph-handle-comment) nil)
 
-  ;; Comments
+  ;; Comments.
   (set (make-local-variable 'comment-start) ".. ")
   (set (make-local-variable 'comment-start-skip)
        (rst-re 'lin-beg 'exm-tag 'bli-sfx))
   (set (make-local-variable 'comment-continue) "   ")
   (set (make-local-variable 'comment-multi-line) t)
   (set (make-local-variable 'comment-use-syntax) nil)
   ;; reStructuredText has not really a comment ender but nil is not really a
-  ;; permissible value
+  ;; permissible value.
   (set (make-local-variable 'comment-end) "")
   (set (make-local-variable 'comment-end-skip) nil)
 
+  ;; Commenting in reStructuredText is very special so use our own set of
+  ;; functions.
   (set (make-local-variable 'comment-line-break-function)
        'rst-comment-line-break)
   (set (make-local-variable 'comment-indent-function)
        'rst-comment-indent)
   (set (make-local-variable 'comment-insert-comment-function)
        'rst-comment-insert-comment)
   (set (make-local-variable 'comment-region-function)
        'rst-comment-region)
   (set (make-local-variable 'uncomment-region-function)
        'rst-uncomment-region)
 
-  ;; Font lock
-  (setq font-lock-defaults
-	'(rst-font-lock-keywords
-	  t nil nil nil
-	  (font-lock-multiline . t)
-	  (font-lock-mark-block-function . mark-paragraph)
-	  ;; rst-mode does not need font-lock-support-mode because it's fast
-	  ;; enough. In fact using `jit-lock-mode` slows things down
-	  ;; considerably even if `rst-font-lock-extend-region` is in place and
-	  ;; compiled.
-	  ;;(font-lock-support-mode . nil)
-	  ))
+  ;; Font lock.
+  (set (make-local-variable 'font-lock-defaults)
+       '(rst-font-lock-keywords
+	 t nil nil nil
+	 (font-lock-multiline . t)
+	 (font-lock-mark-block-function . mark-paragraph)))
   (add-hook 'font-lock-extend-region-functions 'rst-font-lock-extend-region t)
 
-  ;; Text after a changed line may need new fontification
+  ;; Text after a changed line may need new fontification.
   (set (make-local-variable 'jit-lock-contextually) t))
 
 ;;;###autoload
 (define-minor-mode rst-minor-mode
   "Toggle ReST minor mode.
 With a prefix argument ARG, enable ReST minor mode if ARG is
 positive, and disable it otherwise.  If called from Lisp, enable
@@ -784,16 +818,16 @@
  ;; The indicator for the mode line.
  " ReST"
  ;; The minor mode bindings.
  rst-mode-map
  :group 'rst)
 
 ;; FIXME: can I somehow install these too?
-;;  :abbrev-table rst-mode-abbrev-table
-;;  :syntax-table rst-mode-syntax-table
+;;        :abbrev-table rst-mode-abbrev-table
+;;        :syntax-table rst-mode-syntax-table
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Section Adornment Adjustment
 ;; ============================
 ;;
 ;; The following functions implement a smart automatic title sectioning feature.
@@ -866,30 +900,30 @@
 
 (defgroup rst-adjust nil
   "Settings for adjustment and cycling of section title adornments."
   :group 'rst
   :version "21.1")
 
 (define-obsolete-variable-alias
-  'rst-preferred-decorations 'rst-preferred-adornments "r6506")
+  'rst-preferred-decorations 'rst-preferred-adornments "1.0.0")
 (defcustom rst-preferred-adornments '((?= over-and-under 1)
 				      (?= simple 0)
 				      (?- simple 0)
 				      (?~ simple 0)
 				      (?+ simple 0)
 				      (?` simple 0)
 				      (?# simple 0)
 				      (?@ simple 0))
   "Preferred hierarchy of section title adornments.
 
 A list consisting of lists of the form (CHARACTER STYLE INDENT).
-CHARACTER is the character used. STYLE is one of the symbols
-OVER-AND-UNDER or SIMPLE. INDENT is an integer giving the wanted
-indentation for STYLE OVER-AND-UNDER. CHARACTER and STYLE are
-always used when a section adornment is described. In other
+CHARACTER is the character used.  STYLE is one of the symbols
+OVER-AND-UNDER or SIMPLE.  INDENT is an integer giving the wanted
+indentation for STYLE OVER-AND-UNDER.  CHARACTER and STYLE are
+always used when a section adornment is described.  In other
 places t instead of a list stands for a transition.
 
 This sequence is consulted to offer a new adornment suggestion
 when we rotate the underlines at the end of the existing
 hierarchy of characters, or when there is no existing section
 title in the file.
 
@@ -986,268 +1020,268 @@
 If there are existing overline and/or underline from the
 existing adornment, they are removed before adding the
 requested adornment."
   (end-of-line)
   (let ((marker (point-marker))
         len)
 
-      ;; Fixup whitespace at the beginning and end of the line
+      ;; Fixup whitespace at the beginning and end of the line.
       (if (or (null indent) (eq style 'simple))
           (setq indent 0))
       (beginning-of-line)
       (delete-horizontal-space)
       (insert (make-string indent ? ))
 
       (end-of-line)
       (delete-horizontal-space)
 
-      ;; Set the current column, we're at the end of the title line
+      ;; Set the current column, we're at the end of the title line.
       (setq len (+ (current-column) indent))
 
-      ;; Remove previous line if it is an adornment
+      ;; Remove previous line if it is an adornment.
       (save-excursion
         (forward-line -1)
 	(if (and (looking-at (rst-re 'ado-beg-2-1))
 		 ;; Avoid removing the underline of a title right above us.
 		 (save-excursion (forward-line -1)
 				 (not (looking-at (rst-re 'ttl-beg)))))
 	    (rst-delete-entire-line)))
 
-      ;; Remove following line if it is an adornment
+      ;; Remove following line if it is an adornment.
       (save-excursion
         (forward-line +1)
         (if (looking-at (rst-re 'ado-beg-2-1))
 	    (rst-delete-entire-line))
         ;; Add a newline if we're at the end of the buffer, for the subsequence
-        ;; inserting of the underline
+        ;; inserting of the underline.
         (if (= (point) (buffer-end 1))
             (newline 1)))
 
-      ;; Insert overline
+      ;; Insert overline.
       (if (eq style 'over-and-under)
           (save-excursion
             (beginning-of-line)
             (open-line 1)
             (insert (make-string len char))))
 
-      ;; Insert underline
+      ;; Insert underline.
       (forward-line +1)
       (open-line 1)
       (insert (make-string len char))
 
       (forward-line +1)
       (goto-char marker)
       ))
 
 (defun rst-classify-adornment (adornment end)
   "Classify adornment for section titles and transitions.
 ADORNMENT is the complete adornment string as found in the buffer
-with optional trailing whitespace. END is the point after the
+with optional trailing whitespace.  END is the point after the
 last character of ADORNMENT.
 
-Return a list. The first entry is t for a transition or a
-cons (CHARACTER . STYLE). Check `rst-preferred-adornments' for
+Return a list.  The first entry is t for a transition or a
+cons (CHARACTER . STYLE).  Check `rst-preferred-adornments' for
 the meaning of CHARACTER and STYLE.
 
 The remaining list forms four match groups as returned by
-`match-data'. Match group 0 matches the whole construct. Match
-group 1 matches the overline adornment if present. Match group 2
-matches the section title text or the transition. Match group 3
+`match-data'.  Match group 0 matches the whole construct.  Match
+group 1 matches the overline adornment if present.  Match group 2
+matches the section title text or the transition.  Match group 3
 matches the underline adornment.
 
 Return nil if no syntactically valid adornment is found."
   (save-excursion
     (save-match-data
       (when (string-match (rst-re 'ado-beg-2-1) adornment)
 	(goto-char end)
 	(let* ((ado-ch (string-to-char (match-string 2 adornment)))
 	       (ado-re (rst-re ado-ch 'adorep3-hlp))
 	       (end-pnt (point))
 	       (beg-pnt (progn
 			  (forward-line 0)
 			  (point)))
-	       (nxt-emp ; Next line inexistant or empty
+	       (nxt-emp ; Next line nonexistent or empty
 		(save-excursion
 		  (or (not (zerop (forward-line 1)))
 		      (looking-at (rst-re 'lin-end)))))
-	       (prv-emp ; Previous line inexistant or empty
+	       (prv-emp ; Previous line nonexistent or empty
 		(save-excursion
 		  (or (not (zerop (forward-line -1)))
 		      (looking-at (rst-re 'lin-end)))))
-	       (ttl-blw ; Title found below starting here
+	       (ttl-blw ; Title found below starting here.
 		(save-excursion
 		  (and
 		   (zerop (forward-line 1))
 		   (looking-at (rst-re 'ttl-beg))
 		   (point))))
-	       (ttl-abv ; Title found above starting here
+	       (ttl-abv ; Title found above starting here.
 		(save-excursion
 		  (and
 		   (zerop (forward-line -1))
 		   (looking-at (rst-re 'ttl-beg))
 		   (point))))
-	       (und-fnd ; Matching underline found starting here
+	       (und-fnd ; Matching underline found starting here.
 		(save-excursion
 		  (and ttl-blw
 		   (zerop (forward-line 2))
 		   (looking-at (rst-re ado-re 'lin-end))
 		   (point))))
-	       (ovr-fnd ; Matching overline found starting here
+	       (ovr-fnd ; Matching overline found starting here.
 		(save-excursion
 		  (and ttl-abv
 		   (zerop (forward-line -2))
 		   (looking-at (rst-re ado-re 'lin-end))
 		   (point))))
 	       key beg-ovr end-ovr beg-txt end-txt beg-und end-und)
 	  (cond
 	   ((and nxt-emp prv-emp)
-	    ;; A transition
+	    ;; A transition.
 	    (setq key t
 		  beg-txt beg-pnt
 		  end-txt end-pnt))
 	   ((or und-fnd ovr-fnd)
-	    ;; An overline with an underline
+	    ;; An overline with an underline.
 	    (setq key (cons ado-ch 'over-and-under))
-	    (let (;; Prefer overline match over underline match
+	    (let (;; Prefer overline match over underline match.
 		  (und-pnt (if ovr-fnd beg-pnt und-fnd))
 		  (ovr-pnt (if ovr-fnd ovr-fnd beg-pnt))
 		  (txt-pnt (if ovr-fnd ttl-abv ttl-blw)))
 	      (goto-char ovr-pnt)
 	      (setq beg-ovr (point)
 		    end-ovr (line-end-position))
 	      (goto-char txt-pnt)
 	      (setq beg-txt (point)
 		    end-txt (line-end-position))
 	      (goto-char und-pnt)
 	      (setq beg-und (point)
 		    end-und (line-end-position))))
 	   (ttl-abv
-	    ;; An underline
+	    ;; An underline.
 	    (setq key (cons ado-ch 'simple)
 		  beg-und beg-pnt
 		  end-und end-pnt)
 	    (goto-char ttl-abv)
 	    (setq beg-txt (point)
 		  end-txt (line-end-position)))
 	   (t
-	    ;; Invalid adornment
+	    ;; Invalid adornment.
 	    (setq key nil)))
 	  (if key
 	      (list key
 		    (or beg-ovr beg-txt beg-und)
 		    (or end-und end-txt end-ovr)
 		    beg-ovr end-ovr beg-txt end-txt beg-und end-und)))))))
 
 (defun rst-find-title-line ()
   "Find a section title line around point and return its characteristics.
 If the point is on an adornment line find the respective title
-line. If the point is on an empty line check previous or next
-line whether it is a suitable title line and use it if so. If
+line.  If the point is on an empty line check previous or next
+line whether it is a suitable title line and use it if so.  If
 point is on a suitable title line use it.
 
 If no title line is found return nil.
 
-Otherwise return as `rst-classify-adornment' does. However, if
+Otherwise return as `rst-classify-adornment' does.  However, if
 the title line has no syntactically valid adornment STYLE is nil
-in the first element. If there is no adornment around the title
+in the first element.  If there is no adornment around the title
 CHARACTER is also nil and match groups for overline and underline
 are nil."
   (save-excursion
     (forward-line 0)
     (let ((orig-pnt (point))
 	  (orig-end (line-end-position)))
       (cond
        ((looking-at (rst-re 'ado-beg-2-1))
 	(let ((char (string-to-char (match-string-no-properties 2)))
 	      (r (rst-classify-adornment (match-string-no-properties 0)
 					 (match-end 0))))
 	  (cond
 	   ((not r)
-	    ;; Invalid adornment - check whether this is an incomplete overline
+	    ;; Invalid adornment - check whether this is an incomplete overline.
 	    (if (and
 		 (zerop (forward-line 1))
 		 (looking-at (rst-re 'ttl-beg)))
 		(list (cons char nil) orig-pnt (line-end-position)
 		      orig-pnt orig-end (point) (line-end-position) nil nil)))
 	   ((consp (car r))
-	    ;; A section title - not a transition
+	    ;; A section title - not a transition.
 	    r))))
        ((looking-at (rst-re 'lin-end))
 	(or
 	 (save-excursion
 	   (if (and (zerop (forward-line -1))
 		    (looking-at (rst-re 'ttl-beg)))
 	       (list (cons nil nil) (point) (line-end-position)
 		     nil nil (point) (line-end-position) nil nil)))
 	 (save-excursion
 	   (if (and (zerop (forward-line 1))
 		    (looking-at (rst-re 'ttl-beg)))
 	       (list (cons nil nil) (point) (line-end-position)
 		     nil nil (point) (line-end-position) nil nil)))))
        ((looking-at (rst-re 'ttl-beg))
-	;; Try to use the underline
+	;; Try to use the underline.
 	(let ((r (rst-classify-adornment
-		  (buffer-substring-no-properties 
+		  (buffer-substring-no-properties
 		   (line-beginning-position 2) (line-end-position 2))
 		  (line-end-position 2))))
 	  (if r
 	      r
-	    ;; No valid adornment found
+	    ;; No valid adornment found.
 	    (list (cons nil nil) (point) (line-end-position)
 		  nil nil (point) (line-end-position) nil nil))))))))
 
 ;; The following function and variables are used to maintain information about
 ;; current section adornment in a buffer local cache. Thus they can be used for
 ;; font-locking and manipulation commands.
 
-(defun rst-reset-section-caches ()
-  "Reset all section cache variables.
-Should be called by interactive functions which deal with sections."
-  (setq rst-all-sections nil
-	rst-section-hierarchy nil))
-
 (defvar rst-all-sections nil
   "All section adornments in the buffer as found by `rst-find-all-adornments'.
 t when no section adornments were found.")
 (make-variable-buffer-local 'rst-all-sections)
 
 ;; FIXME: If this variable is set to a different value font-locking of section
-;; headers is wrong
+;;        headers is wrong.
 (defvar rst-section-hierarchy nil
   "Section hierarchy in the buffer as determined by `rst-get-hierarchy'.
-t when no section adornments were found. Value depends on
+t when no section adornments were found.  Value depends on
 `rst-all-sections'.")
 (make-variable-buffer-local 'rst-section-hierarchy)
 
+(defun rst-reset-section-caches ()
+  "Reset all section cache variables.
+Should be called by interactive functions which deal with sections."
+  (setq rst-all-sections nil
+	rst-section-hierarchy nil))
+
 (defun rst-find-all-adornments ()
   "Return all the section adornments in the current buffer.
 Return a list of (LINE . ADORNMENT) with ascending LINE where
-LINE is the line containing the section title. ADORNMENT consists
+LINE is the line containing the section title.  ADORNMENT consists
 of a (CHARACTER STYLE INDENT) triple as described for
 `rst-preferred-adornments'.
 
 Uses and sets `rst-all-sections'."
   (unless rst-all-sections
     (let (positions)
       ;; Iterate over all the section titles/adornments in the file.
       (save-excursion
 	(goto-char (point-min))
 	(while (re-search-forward (rst-re 'ado-beg-2-1) nil t)
 	  (let ((ado-data (rst-classify-adornment
 			   (match-string-no-properties 0) (point))))
 	    (when (and ado-data
-		       (consp (car ado-data))) ; Ignore transitions
+		       (consp (car ado-data))) ; Ignore transitions.
 	      (set-match-data (cdr ado-data))
-	      (goto-char (match-beginning 2)) ; Goto the title start
+	      (goto-char (match-beginning 2)) ; Goto the title start.
 	      (push (cons (1+ (count-lines (point-min) (point)))
 			  (list (caar ado-data)
 				(cdar ado-data)
 				(current-indentation)))
 		    positions)
-	      (goto-char (match-end 0))))) ; Go beyond the whole thing
+	      (goto-char (match-end 0))))) ; Go beyond the whole thing.
 	(setq positions (nreverse positions))
 	(setq rst-all-sections (or positions t)))))
   (if (eq rst-all-sections t)
       nil
     rst-all-sections))
 
 (defun rst-infer-hierarchy (adornments)
@@ -1269,16 +1303,16 @@
 	  (push (cons (cons char style) x) hierarchy-alist))))
     (mapcar 'cdr (nreverse hierarchy-alist))))
 
 (defun rst-get-hierarchy (&optional ignore)
   "Return the hierarchy of section titles in the file.
 
 Return a list of adornments that represents the hierarchy of
-section titles in the file. Each element consists of (CHARACTER
-STYLE INDENT) as described for `rst-find-all-adornments'. If the
+section titles in the file.  Each element consists of (CHARACTER
+STYLE INDENT) as described for `rst-find-all-adornments'.  If the
 line number in IGNORE is specified, a possibly adornment found on
 that line is not taken into account when building the hierarchy.
 
 Uses and sets `rst-section-hierarchy' unless IGNORE is given."
   (if (and (not ignore) rst-section-hierarchy)
       (if (eq rst-section-hierarchy t)
 	  nil
@@ -1287,15 +1321,15 @@
 	      (mapcar 'cdr
 		      (assq-delete-all
 		       ignore
 		       (rst-find-all-adornments))))))
       (setq rst-section-hierarchy
 	    (if ignore
 		;; Clear cache reflecting that a possible update is not
-		;; reflected
+		;; reflected.
 		nil
 	      (or r t)))
       r)))
 
 (defun rst-get-adornments-around ()
   "Return the adornments around point.
 Return a list of the previous and next adornments."
@@ -1373,40 +1407,40 @@
         cur))
 
      ;; If not found, take the first of all adornments.
      suggestion
      )))
 
 
-;; FIXME: A line "``/`` full" is not accepted as a section title
+;; FIXME: A line "``/`` full" is not accepted as a section title.
 (defun rst-adjust (pfxarg)
   "Auto-adjust the adornment around point.
 
-Adjust/rotate the section adornment for the section title
-around point or promote/demote the adornments inside the region,
+Adjust/rotate the section adornment for the section title around
+point or promote/demote the adornments inside the region,
 depending on if the region is active.  This function is meant to
 be invoked possibly multiple times, and can vary its behavior
-with a positive prefix argument (toggle style), or with a
-negative prefix argument (alternate behavior).
+with a positive PFXARG (toggle style), or with a negative
+PFXARG (alternate behavior).
 
-This function is a bit of a swiss knife. It is meant to adjust
-the adornments of a section title in reStructuredText. It tries
+This function is a bit of a swiss knife.  It is meant to adjust
+the adornments of a section title in reStructuredText.  It tries
 to deal with all the possible cases gracefully and to do `the
 right thing' in all cases.
 
 See the documentations of `rst-adjust-adornment-work' and
 `rst-promote-region' for full details.
 
 Prefix Arguments
 ================
 
 The method can take either (but not both) of
 
 a. a (non-negative) prefix argument, which means to toggle the
-   adornment style.  Invoke with a prefix arg for example;
+   adornment style.  Invoke with a prefix argument for example;
 
 b. a negative numerical argument, which generally inverts the
    direction of search in the file or hierarchy.  Invoke with C--
    prefix for example."
   (interactive "P")
 
   (let* (;; Save our original position on the current line.
@@ -1442,15 +1476,16 @@
 	  (const :tag "Same level as previous one" nil)
 	  (const :tag "One level down relative to the previous one" t))
   :package-version '(rst . "1.1.0"))
 
 (defun rst-adjust-adornment (pfxarg)
   "Call `rst-adjust-adornment-work' interactively.
 
-Keep this for compatibility for older bindings (are there any?)."
+Keep this for compatibility for older bindings (are there any?).
+Argument PFXARG has the same meaning as for `rst-adjust'."
   (interactive "P")
 
   (let* ((reverse-direction (and pfxarg (< (prefix-numeric-value pfxarg) 0)))
          (toggle-style (and pfxarg (not reverse-direction))))
     (rst-adjust-adornment-work toggle-style reverse-direction)))
 
 (defun rst-adjust-adornment-work (toggle-style reverse-direction)
@@ -1656,15 +1691,15 @@
 	      ;; Simply switch the style of the current adornment.
 	      (setq char-new char
 		    style-new (if (eq style 'simple) 'over-and-under 'simple)
 		    indent-new rst-default-indent)
 	    ;; Else, we rotate, ignoring the adornment around the current
 	    ;; line...
 	    (let* ((hier (rst-get-hierarchy (line-number-at-pos)))
-		   ;; Suggestion, in case we need to come up with something new
+		   ;; Suggestion, in case we need to come up with something new.
 		   (suggestion (rst-suggest-new-adornment
 				hier
 				(car (rst-get-adornments-around))))
 		   (nextado (rst-get-next-adornment
 			     curado hier suggestion reverse-direction)))
 	      ;; Indent, if present, always overrides the prescribed indent.
 	      (setq char-new (car nextado)
@@ -1698,15 +1733,15 @@
 
          (region-begin-line (line-number-at-pos (region-beginning)))
          (region-end-line (line-number-at-pos (region-end)))
 
          marker-list
          )
 
-    ;; Skip the markers that come before the region beginning
+    ;; Skip the markers that come before the region beginning.
     (while (and cur (< (caar cur) region-begin-line))
       (setq cur (cdr cur)))
 
     ;; Create a list of markers for all the adornments which are found within
     ;; the region.
     (save-excursion
       (let (line)
@@ -1750,58 +1785,53 @@
           (apply 'rst-update-section x)
           (goto-char (point-max))
           (insert "\n")
           (incf level)
           ))
     )))
 
-(defun rst-position (elem list)
-  "Return position of ELEM in LIST or nil."
-  (let ((tail (member elem list)))
-    (if tail (- (length list) (length tail)))))
-
 (defun rst-straighten-adornments ()
   "Redo all the adornments in the current buffer.
 This is done using our preferred set of adornments.  This can be
 used, for example, when using somebody else's copy of a document,
 in order to adapt it to our preferred style."
   (interactive)
   (rst-reset-section-caches)
   (save-excursion
-    (let (;; Get a list of pairs of (level . marker)
+    (let (;; Get a list of pairs of (level . marker).
 	  (levels-and-markers (mapcar
 			       (lambda (ado)
 				 (cons (rst-position (cdr ado)
 						     (rst-get-hierarchy))
 				       (progn
 					 (goto-char (point-min))
 					 (forward-line (1- (car ado)))
 					 (point-marker))))
 			       (rst-find-all-adornments))))
       (dolist (lm levels-and-markers)
-	;; Go to the appropriate position
+	;; Go to the appropriate position.
 	(goto-char (cdr lm))
 
-	;; Apply the new styule
+	;; Apply the new style.
 	(apply 'rst-update-section (nth (car lm) rst-preferred-adornments))
 
-	;; Reset the market to avoid slowing down editing until it gets GC'ed
+	;; Reset the marker to avoid slowing down editing until it gets GC'ed.
 	(set-marker (cdr lm) nil)
 	)
     )))
 
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Insert list items
 ;; =================
 
 
 ;=================================================
-; Borrowed from a2r.el (version 1.3), by Lawrence Mitchell <wence@gmx.li>
+; Borrowed from a2r.el (version 1.3), by Lawrence Mitchell <wence@gmx.li>.
 ; I needed to make some tiny changes to the functions, so I put it here.
 ; -- Wei-Wei Guo
 
 (defconst rst-arabic-to-roman
   '((1000 .   "M") (900  .  "CM") (500  .   "D") (400  .  "CD")
     (100  .   "C") (90   .  "XC") (50   .   "L") (40   .  "XL")
     (10   .   "X") (9    .  "IX") (5    .   "V") (4    .  "IV")
@@ -1844,17 +1874,17 @@
                 string (replace-match "" nil t string))
         (setq map (cdr map))))
     res))
 ;=================================================
 
 (defun rst-find-pfx-in-region (beg end pfx-re)
   "Find all the positions of prefixes in region between BEG and END.
-This is used to find bullets and enumerated list items. PFX-RE is
+This is used to find bullets and enumerated list items.  PFX-RE is
 a regular expression for matching the lines after indentation
-with items. Returns a list of cons cells consisting of the point
+with items.  Returns a list of cons cells consisting of the point
 and the column of the point."
   (let ((pfx ()))
     (save-excursion
       (goto-char beg)
       (while (< (point) end)
 	(back-to-indentation)
 	(when (and
@@ -1862,22 +1892,22 @@
 	       (let ((pfx-col (current-column)))
 		 (save-excursion
 		   (forward-line -1) ; ...previous line is...
 		   (back-to-indentation)
 		   (or (looking-at (rst-re 'lin-end)) ; ...empty,
 		       (> (current-column) pfx-col) ; ...deeper level, or
 		       (and (= (current-column) pfx-col)
-			    (looking-at pfx-re)))))) ; ...pfx at same level
+			    (looking-at pfx-re)))))) ; ...pfx at same level.
 	  (push (cons (point) (current-column))
                 pfx))
 	(forward-line 1)) )
     (nreverse pfx)))
 
 (defun rst-insert-list-pos (newitem)
-  "Arrange relative position of a newly inserted list item.
+  "Arrange relative position of a newly inserted list item of style NEWITEM.
 
 Adding a new list might consider three situations:
 
  (a) Current line is a blank line.
  (b) Previous line is a blank line.
  (c) Following line is a blank line.
 
@@ -1896,48 +1926,50 @@
             (forward-line -1)
             (looking-at (rst-re 'lin-end)))
           (insert newitem " ")
         (insert "\n" newitem " "))
     (end-of-line)
     (insert "\n\n" newitem " ")))
 
+;; FIXME: Isn't this a `defconst'?
 (defvar rst-initial-enums
   (let (vals)
     (dolist (fmt '("%s." "(%s)" "%s)"))
       (dolist (c '("1" "a" "A" "I" "i"))
         (push (format fmt c) vals)))
     (cons "#." (nreverse vals)))
   "List of initial enumerations.")
 
+;; FIXME: Isn't this a `defconst'?
 (defvar rst-initial-items
   (append (mapcar 'char-to-string rst-bullets) rst-initial-enums)
   "List of initial items.  It's collection of bullets and enumerations.")
 
 (defun rst-insert-list-new-item ()
   "Insert a new list item.
 
 User is asked to select the item style first, for example (a), i), +.  Use TAB
-for completition and choices.
+for completion and choices.
 
 If user selects bullets or #, it's just added with position arranged by
 `rst-insert-list-pos'.
 
-If user selects enumerations, a further prompt is given. User need to input a
+If user selects enumerations, a further prompt is given.  User need to input a
 starting item, for example 'e' for 'A)' style.  The position is also arranged by
 `rst-insert-list-pos'."
   (interactive)
-  ;; FIXME: Make this comply to `interactive' standards
+  ;; FIXME: Make this comply to `interactive' standards.
   (let* ((itemstyle (completing-read
 		     "Select preferred item style [#.]: "
 		     rst-initial-items nil t nil nil "#."))
 	 (cnt (if (string-match (rst-re 'cntexp-tag) itemstyle)
 		  (match-string 0 itemstyle)))
 	 (no
 	  (save-match-data
-	    ;; FIXME: Make this comply to `interactive' standards
+	    ;; FIXME: Make this comply to `interactive' standards.
 	    (cond
 	     ((equal cnt "a")
 	      (let ((itemno (read-string "Give starting value [a]: "
 					 nil nil "a")))
 		(downcase (substring itemno 0 1))))
 	     ((equal cnt "A")
 	      (let ((itemno (read-string "Give starting value [A]: "
@@ -1964,39 +1996,40 @@
 	  (choice ,@(mapcar (lambda (char)
 			      (list 'const
 				    :tag (char-to-string char) char))
 			    rst-bullets)))
   :package-version '(rst . "1.1.0"))
 
 (defun rst-insert-list-continue (curitem prefer-roman)
-  "Insert a list item with list start CURITEM including its indentation level."
+  "Insert a list item with list start CURITEM including its indentation level.
+If PREFER-ROMAN roman numbering is preferred over using letters."
   (end-of-line)
   (insert
-   "\n" ; FIXME: Separating lines must be possible
+   "\n" ; FIXME: Separating lines must be possible.
    (cond
     ((string-match (rst-re '(:alt enmaut-tag
 				  bul-tag)) curitem)
      curitem)
     ((string-match (rst-re 'num-tag) curitem)
      (replace-match (number-to-string
 		     (1+ (string-to-number (match-string 0 curitem))))
 		    nil nil curitem))
     ((and (string-match (rst-re 'rom-tag) curitem)
 	  (save-match-data
-	    (if (string-match (rst-re 'ltr-tag) curitem) ; Also a letter tag
+	    (if (string-match (rst-re 'ltr-tag) curitem) ; Also a letter tag.
 		(save-excursion
 		  ;; FIXME: Assumes one line list items without separating
-		  ;; empty lines
+		  ;;        empty lines.
 		  (if (and (zerop (forward-line -1))
 			   (looking-at (rst-re 'enmexp-beg)))
 		      (string-match
 		       (rst-re 'rom-tag)
-		       (match-string 0)) ; Previous was a roman tag
-		    prefer-roman)) ; Don't know - use flag
-	      t))) ; Not a letter tag
+		       (match-string 0)) ; Previous was a roman tag.
+		    prefer-roman)) ; Don't know - use flag.
+	      t))) ; Not a letter tag.
      (replace-match
       (let* ((old (match-string 0 curitem))
 	     (new (save-match-data
 		    (rst-arabic-to-roman
 		     (1+ (rst-roman-to-arabic
 			  (upcase old)))))))
 	(if (equal old (upcase old))
@@ -2008,22 +2041,22 @@
 		     (1+ (string-to-char (match-string 0 curitem))))
 		    nil nil curitem)))))
 
 
 (defun rst-insert-list (&optional prefer-roman)
   "Insert a list item at the current point.
 
-The command can insert a new list or a continuing list. When it is called at a
-non-list line, it will promote to insert new list. When it is called at a list
+The command can insert a new list or a continuing list.  When it is called at a
+non-list line, it will promote to insert new list.  When it is called at a list
 line, it will insert a list with the same list style.
 
 1. When inserting a new list:
 
-User is asked to select the item style first, for example (a), i), +. Use TAB
-for completition and choices.
+User is asked to select the item style first, for example (a), i), +.  Use TAB
+for completion and choices.
 
  (a) If user selects bullets or #, it's just added.
  (b) If user selects enumerations, a further prompt is given.  User needs to
      input a starting item, for example 'e' for 'A)' style.
 
 The position of the new list is arranged according to whether or not the
 current line and the previous line are blank lines.
@@ -2031,15 +2064,15 @@
 2. When continuing a list, one thing need to be noticed:
 
 List style alphabetical list, such as 'a.', and roman numerical list, such as
 'i.', have some overlapping items, for example 'v.' The function can deal with
 the problem elegantly in most situations.  But when those overlapped list are
 preceded by a blank line, it is hard to determine which type to use
 automatically.  The function uses alphabetical list by default.  If you want
-roman numerical list, just use a prefix (\\[universal-argument])."
+roman numerical list, just use a prefix to set PREFER-ROMAN."
   (interactive "P")
   (beginning-of-line)
   (if (looking-at (rst-re 'itmany-beg-1))
       (rst-insert-list-continue (match-string 0) prefer-roman)
     (rst-insert-list-new-item)))
 
 (defun rst-straighten-bullets-region (beg end)
@@ -2089,26 +2122,26 @@
   (buffer-substring-no-properties (match-beginning 0)
                                   (match-end 0)) )
 
 (defun rst-section-tree ()
   "Get the hierarchical tree of section titles.
 
 Returns a hierarchical tree of the sections titles in the
-document. This can be used to generate a table of contents for
-the document. The top node will always be a nil node, with the
+document.  This can be used to generate a table of contents for
+the document.  The top node will always be a nil node, with the
 top level titles as children (there may potentially be more than
 one).
 
 Each section title consists in a cons of the stripped title
 string and a marker to the section in the original text document.
 
 If there are missing section levels, the section titles are
 inserted automatically, and the title string is set to nil, and
 the marker set to the first non-nil child of itself.
-Conceptually, the nil nodes--i.e. those which have no title--are
+Conceptually, the nil nodes--i.e.\ those which have no title--are
 to be considered as being the same line as their first non-nil
 child.  This has advantages later in processing the graph."
 
   (let ((hier (rst-get-hierarchy))
 	(levels (make-hash-table :test 'equal :size 10))
 	lines)
 
@@ -2143,22 +2176,22 @@
 pair of the subtree that was built.  This treats the ADOS
 list destructively."
 
   (let ((nado (cadr ados))
         node
         children)
 
-    ;; If the next adornment matches our level
+    ;; If the next adornment matches our level.
     (when (and nado (= (car nado) lev))
-      ;; Pop the next adornment and create the current node with it
+      ;; Pop the next adornment and create the current node with it.
       (setcdr ados (cddr ados))
       (setq node (cdr nado)) )
     ;; Else we let the node title/marker be unset.
 
-    ;; Build the child nodes
+    ;; Build the child nodes.
     (while (and (cdr ados) (> (caadr ados) lev))
       (setq children
             (cons (rst-section-tree-rec ados (1+ lev))
                   children)))
     (setq children (reverse children))
 
     ;; If node is still unset, we use the marker of the first child.
@@ -2170,15 +2203,15 @@
     ))
 
 
 (defun rst-section-tree-point (node &optional point)
   "Find tree node at point.
 Given a computed and valid section tree in NODE and a point
 POINT (default being the current point in the current buffer),
-find and return the node within the sectree where the cursor
+find and return the node within the section tree where the cursor
 lives.
 
 Return values: a pair of (parent path, container subtree).
 The parent path is simply a list of the nodes above the
 container subtree node that we're returning."
 
   (let (path outtree)
@@ -2251,15 +2284,15 @@
 
 If a numeric prefix argument PFXARG is given, insert the TOC up
 to the specified level.
 
 The TOC is inserted indented at the current column."
   (interactive "P")
   (rst-reset-section-caches)
-  (let* (;; Check maximum level override
+  (let* (;; Check maximum level override.
          (rst-toc-insert-max-level
           (if (and (integerp pfxarg) (> (prefix-numeric-value pfxarg) 0))
               (prefix-numeric-value pfxarg) rst-toc-insert-max-level))
 
          ;; Get the section tree for the current cursor point.
          (sectree-pair
 	  (rst-section-tree-point
@@ -2328,15 +2361,15 @@
 
     (if (or (eq rst-toc-insert-max-level nil)
             (< level rst-toc-insert-max-level))
         (let ((do-child-numbering (>= level 0))
               fmt)
           (if do-child-numbering
               (progn
-                ;; Add a separating dot if there is already a prefix
+                ;; Add a separating dot if there is already a prefix.
                 (when (> (length pfx) 0)
 		  (string-match (rst-re "[ \t\n]*\\'") pfx)
 		  (setq pfx (concat (replace-match "" t t pfx) ".")))
 
                 ;; Calculate the amount of space that the prefix will require
                 ;; for the numbers.
                 (if (cdr node)
@@ -2380,17 +2413,17 @@
 	  last-real)
       (when beg
 	;; Look for the first line that starts at the first column.
 	(forward-line 1)
 	(while (and
 		(< (point) (point-max))
 		(or (if (looking-at
-			 (rst-re 'hws-sta "\\S ")) ; indented content
+			 (rst-re 'hws-sta "\\S ")) ; indented content.
 			(setq last-real (point)))
-		    (looking-at (rst-re 'lin-end)))) ; empty line
+		    (looking-at (rst-re 'lin-end)))) ; empty line.
 	  (forward-line 1))
 	(if last-real
 	    (progn
 	      (goto-char last-real)
 	      (end-of-line)
 	      (delete-region beg (point)))
 	  (goto-char beg))
@@ -2512,20 +2545,22 @@
       (error "No section on this line"))
     (unless (buffer-live-p (marker-buffer pos))
       (error "Buffer for this section was killed"))
     pos))
 
 ;; FIXME: Cursor before or behind the list must be handled properly; before the
 ;;        list should jump to the top and behind the list to the last normal
-;;        paragraph
+;;        paragraph.
 (defun rst-goto-section (&optional kill)
-  "Go to the section the current line describes."
+  "Go to the section the current line describes.
+If KILL a toc buffer is destroyed."
   (interactive)
   (let ((pos (rst-toc-mode-find-section)))
     (when kill
+      ;; FIXME: This should rather go to `rst-toc-mode-goto-section'.
       (set-window-configuration (car rst-toc-return-wincfg))
       (kill-buffer (get-buffer rst-toc-buffer-name)))
     (pop-to-buffer (marker-buffer pos))
     (goto-char pos)
     ;; FIXME: make the recentering conditional on scroll.
     (recenter 5)))
 
@@ -2544,15 +2579,16 @@
 	     (goto-char (posn-point (event-end event)))
              (rst-toc-mode-find-section)))))
     (pop-to-buffer (marker-buffer pos))
     (goto-char pos)
     (recenter 5)))
 
 (defun rst-toc-mode-mouse-goto-kill (event)
-  "Same as `rst-toc-mode-mouse-goto', but kill TOC buffer as well."
+  "Same as `rst-toc-mode-mouse-goto', but kill TOC buffer as well.
+EVENT is the input event."
   (interactive "e")
   (call-interactively 'rst-toc-mode-mouse-goto event)
   (kill-buffer (get-buffer rst-toc-buffer-name)))
 
 (defun rst-toc-quit-window ()
   "Leave the current TOC buffer."
   (interactive)
@@ -2577,15 +2613,14 @@
 (define-derived-mode rst-toc-mode nil "ReST-TOC"
   "Major mode for output from \\[rst-toc], the table-of-contents for the document."
   (setq buffer-read-only t))
 
 ;; Note: use occur-mode (replace.el) as a good example to complete missing
 ;; features.
 
-
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Section movement commands
 ;; =========================
 
 (defun rst-forward-section (&optional offset)
   "Skip to the next reStructuredText section title.
 OFFSET specifies how many titles to skip.  Use a negative OFFSET to move
@@ -2628,33 +2663,36 @@
     ))
 
 (defun rst-backward-section ()
   "Like `rst-forward-section', except move back one title."
   (interactive)
   (rst-forward-section -1))
 
-(defun rst-mark-section (&optional arg allow-extend)
-  "Select the section that point is currently in."
+;; FIXME: What is `allow-extend' for?
+(defun rst-mark-section (&optional count allow-extend)
+  "Select COUNT sections around point.
+Mark following sections for positive COUNT or preceding sections
+for negative COUNT."
   ;; Cloned from mark-paragraph.
   (interactive "p\np")
-  (unless arg (setq arg 1))
-  (when (zerop arg)
+  (unless count (setq count 1))
+  (when (zerop count)
     (error "Cannot mark zero sections"))
   (cond ((and allow-extend
 	      (or (and (eq last-command this-command) (mark t))
 		  (rst-portable-mark-active-p)))
 	 (set-mark
 	  (save-excursion
 	    (goto-char (mark))
-	    (rst-forward-section arg)
+	    (rst-forward-section count)
 	    (point))))
 	(t
-	 (rst-forward-section arg)
+	 (rst-forward-section count)
 	 (push-mark nil t t)
-	 (rst-forward-section (- arg)))))
+	 (rst-forward-section (- count)))))
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Functions to work on item lists (e.g. indent/dedent, enumerate), which are
 ;; always 2 or 3 characters apart horizontally with rest.
 
 (defun rst-find-leftmost-column (beg end)
@@ -2667,29 +2705,29 @@
         (unless (looking-at (rst-re 'lin-end))
 	  (setq mincol (if mincol
 			   (min mincol (current-column))
 			 (current-column))))
         (forward-line 1)))
     mincol))
 
+;; FIXME: This definition is old and deprecated.  We need to move to the newer
+;;        version below.
 (defmacro rst-iterate-leftmost-paragraphs
   (beg end first-only body-consequent body-alternative)
-  "FIXME This definition is old and deprecated / we need to move
-to the newer version below:
-
-Call FUN at the beginning of each line, with an argument that
+  ;; FIXME: The following comment is pretty useless.
+  "Call FUN at the beginning of each line, with an argument that
 specifies whether we are at the first line of a paragraph that
 starts at the leftmost column of the given region BEG and END.
 Set FIRST-ONLY to true if you want to callback on the first line
 of each paragraph only."
   `(save-excursion
     (let ((leftcol (rst-find-leftmost-column ,beg ,end))
 	  (endm (copy-marker ,end)))
 
-      (do* (;; Iterate lines
+      (do* (;; Iterate lines.
 	    (l (progn (goto-char ,beg) (back-to-indentation))
 	       (progn (forward-line 1) (back-to-indentation)))
 
 	    (previous nil valid)
 
  	    (curcol (current-column)
 		    (current-column))
@@ -2705,28 +2743,30 @@
 		(and valid (not previous))
 	      valid)
 	    ,body-consequent
 	  ,body-alternative)
 
 	))))
 
+;; FIXME: This needs to be refactored. Probably this is simply a function
+;;        applying BODY rather than a macro.
 (defmacro rst-iterate-leftmost-paragraphs-2 (spec &rest body)
   "Evaluate BODY for each line in region defined by BEG END.
 LEFTMOST is set to true if the line is one of the leftmost of the
 entire paragraph.  PARABEGIN is set to true if the line is the
 first of a paragraph."
   (declare (indent 1) (debug (sexp body)))
   (destructuring-bind
       (beg end parabegin leftmost isleftmost isempty) spec
 
   `(save-excursion
      (let ((,leftmost (rst-find-leftmost-column ,beg ,end))
 	   (endm (copy-marker ,end)))
 
-      (do* (;; Iterate lines
+      (do* (;; Iterate lines.
 	    (l (progn (goto-char ,beg) (back-to-indentation))
 	       (progn (forward-line 1) (back-to-indentation)))
 
  	    (empty-line-previous nil ,isempty)
 
 	    (,isempty (looking-at (rst-re 'lin-end))
 			(looking-at (rst-re 'lin-end)))
@@ -2746,108 +2786,106 @@
 
 	)))))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Indentation
 
 ;; FIXME: At the moment only block comments with leading empty comment line are
-;; supported; comment lines with leading comment markup should be also
-;; supported; may be a customizable option could control which style to prefer
+;;        supported.  Comment lines with leading comment markup should be also
+;;        supported.  May be a customizable option could control which style to
+;;        prefer.
 
-(defgroup rst-indent nil "Settings for indendation in reStructuredText.
+(defgroup rst-indent nil "Settings for indentation in reStructuredText.
 
-In reStructuredText indendation points are usually determined by
+In reStructuredText indentation points are usually determined by
 preceding lines. Sometimes the syntax allows arbitrary
-indendation points such as where to start the first line
+indentation points such as where to start the first line
 following a directive. These indentation widths can be customized
 here."
   :group 'rst
   :package-version '(rst . "1.1.0"))
 
 (define-obsolete-variable-alias
-  'rst-shift-basic-offset 'rst-indent-width "r6713")
+  'rst-shift-basic-offset 'rst-indent-width "1.0.0")
 (defcustom rst-indent-width 2
   "Indentation when there is no more indentation point given."
   :group 'rst-indent
   :type '(integer))
 
 (defcustom rst-indent-field 3
-  "Default indendation for first line after a field or 0 to always indent for
-content."
+  "Indentation for first line after a field or 0 to always indent for content."
   :group 'rst-indent
   :type '(integer))
 
 (defcustom rst-indent-literal-normal 3
-  "Default indendation for literal block after a markup on an own
-line."
+  "Default indentation for literal block after a markup on an own line."
   :group 'rst-indent
   :type '(integer))
 
 (defcustom rst-indent-literal-minimized 2
-  "Default indendation for literal block after a minimized
-markup."
+  "Default indentation for literal block after a minimized markup."
   :group 'rst-indent
   :type '(integer))
 
 (defcustom rst-indent-comment 3
-  "Default indendation for first line of a comment."
+  "Default indentation for first line of a comment."
   :group 'rst-indent
   :type '(integer))
 
 ;; FIXME: Must consider other tabs:
-;; * Line blocks
-;; * Definition lists
-;; * Option lists
+;;        * Line blocks
+;;        * Definition lists
+;;        * Option lists
 (defun rst-line-tabs ()
   "Return tabs of the current line or nil for no tab.
 The list is sorted so the tab where writing continues most likely
-is the first one. Each tab is of the form (COLUMN . INNER).
-COLUMN is the column of the tab. INNER is non-nil if this is an
-inner tab. I.e. a tab which does come from the basic indentation
+is the first one.  Each tab is of the form (COLUMN . INNER).
+COLUMN is the column of the tab.  INNER is non-nil if this is an
+inner tab.  I.e. a tab which does come from the basic indentation
 and not from inner alignment points."
   (save-excursion
     (forward-line 0)
     (save-match-data
       (unless (looking-at (rst-re 'lin-end))
 	(back-to-indentation)
-	;; Current indendation is always the least likely tab
+	;; Current indendation is always the least likely tab.
 	(let ((tabs (list (list (point) 0 nil)))) ; (POINT OFFSET INNER)
-	  ;; Push inner tabs more likely to continue writing
+	  ;; Push inner tabs more likely to continue writing.
 	  (cond
-	   ;; Item
+	   ;; Item.
 	   ((looking-at (rst-re '(:grp itmany-tag hws-sta) '(:grp "\\S ") "?"))
 	    (when (match-string 2)
 	      (push (list (match-beginning 2) 0 t) tabs)))
-	   ;; Field
+	   ;; Field.
 	   ((looking-at (rst-re '(:grp fld-tag) '(:grp hws-tag)
 				'(:grp "\\S ") "?"))
 	    (unless (zerop rst-indent-field)
 	      (push (list (match-beginning 1) rst-indent-field t) tabs))
 	    (if (match-string 3)
 		(push (list (match-beginning 3) 0 t) tabs)
 	      (if (zerop rst-indent-field)
 		  (push (list (match-end 2)
 			      (if (string= (match-string 2) "") 1 0)
 			      t) tabs))))
-	   ;; Directive
+	   ;; Directive.
 	   ((looking-at (rst-re 'dir-sta-3 '(:grp "\\S ") "?"))
 	    (push (list (match-end 1) 0 t) tabs)
 	    (unless (string= (match-string 2) "")
 	      (push (list (match-end 2) 0 t) tabs))
 	    (when (match-string 4)
 	      (push (list (match-beginning 4) 0 t) tabs)))
-	   ;; Footnote or citation definition
+	   ;; Footnote or citation definition.
 	   ((looking-at (rst-re 'fnc-sta-2 '(:grp "\\S ") "?"))
 	    (push (list (match-end 1) 0 t) tabs)
 	    (when (match-string 3)
 	      (push (list (match-beginning 3) 0 t) tabs)))
-	   ;; Comment
+	   ;; Comment.
 	   ((looking-at (rst-re 'cmt-sta-1))
 	    (push (list (point) rst-indent-comment t) tabs)))
-	  ;; Start of literal block
+	  ;; Start of literal block.
 	  (when (looking-at (rst-re 'lit-sta-2))
 	    (let ((tab0 (first tabs)))
 	      (push (list (first tab0)
 			  (+ (second tab0)
 			     (if (match-string 1)
 				 rst-indent-literal-minimized
 			       rst-indent-literal-normal))
@@ -2856,30 +2894,30 @@
 		    (goto-char (first tab))
 		    (cons (+ (current-column) (second tab)) (third tab)))
 		  tabs))))))
 
 (defun rst-compute-tabs (pt)
   "Build the list of possible tabs for all lines above.
 Search backwards from point PT to build the list of possible
-tabs. Return a list of tabs sorted by likeliness to continue
-writing like `rst-line-tabs'. Nearer lines have generally a
-higher likeliness than farer lines. Return nil if no tab is found
+tabs.  Return a list of tabs sorted by likeliness to continue
+writing like `rst-line-tabs'.  Nearer lines have generally a
+higher likeliness than farther lines.  Return nil if no tab is found
 in the text above."
   (save-excursion
     (goto-char pt)
-    (let (leftmost ; Leftmost column found so far
-	  innermost ; Leftmost column for inner tab
+    (let (leftmost ; Leftmost column found so far.
+	  innermost ; Leftmost column for inner tab.
 	  tablist)
       (while (and (zerop (forward-line -1))
 		  (or (not leftmost)
 		      (> leftmost 0)))
 	(let* ((tabs (rst-line-tabs))
 	       (leftcol (if tabs (apply 'min (mapcar 'car tabs)))))
 	  (when tabs
-	    ;; Consider only lines indented less or same if not INNERMOST
+	    ;; Consider only lines indented less or same if not INNERMOST.
 	    (when (or (not leftmost)
 		      (< leftcol leftmost)
 		      (and (not innermost) (= leftcol leftmost)))
 	      (dolist (tab tabs)
 		(let ((inner (cdr tab))
 		      (newcol (car tab)))
 		  (when (and
@@ -2888,37 +2926,36 @@
 			       (or (not leftmost)
 				   (< newcol leftmost)))
 			  (and inner
 			       (or (not innermost)
 				   (< newcol innermost))))
 			 (not (memq newcol tablist)))
 		    (push newcol tablist))))
-	      (setq innermost (if (some 'identity
-					(mapcar 'cdr tabs)) ; Has inner
+	      (setq innermost (if (rst-some (mapcar 'cdr tabs)) ; Has inner.
 				  leftcol
 				innermost))
 	      (setq leftmost leftcol)))))
       (nreverse tablist))))
 
 (defun rst-indent-line (&optional dflt)
   "Indent current line to next best reStructuredText tab.
 The next best tab is taken from the tab list returned by
-`rst-compute-tabs' which is used in a cyclic manner. If the
-current indentation does not end on a tab use the first one. If
-the current indentation is on a tab use the next tab. This allows
+`rst-compute-tabs' which is used in a cyclic manner.  If the
+current indentation does not end on a tab use the first one.  If
+the current indentation is on a tab use the next tab.  This allows
 a repeated use of \\[indent-for-tab-command] to cycle through all
-possible tabs. If no indentation is possible return `noindent' or
-use DFLT. Return the indentation indented to. When point is in
-indentation it ends up at its end. Otherwise the point is kept
+possible tabs.  If no indentation is possible return `noindent' or
+use DFLT.  Return the indentation indented to.  When point is in
+indentation it ends up at its end.  Otherwise the point is kept
 relative to the content."
   (let* ((pt (point-marker))
 	 (cur (current-indentation))
 	 (clm (current-column))
 	 (tabs (rst-compute-tabs (point)))
-	 (fnd (position cur tabs))
+	 (fnd (rst-position cur tabs))
 	 ind)
     (if (and (not tabs) (not dflt))
 	'noindent
       (if (not tabs)
 	  (setq ind dflt)
 	(if (not fnd)
 	    (setq fnd 0)
@@ -2931,78 +2968,81 @@
 	  (goto-char pt))
       (set-marker pt nil)
       ind)))
 
 (defun rst-shift-region (beg end cnt)
   "Shift region BEG to END by CNT tabs.
 Shift by one tab to the right (CNT > 0) or left (CNT < 0) or
-remove all indentation (CNT = 0). An tab is taken from the text
-above. If no suitable tab is found `rst-indent-width' is used."
+remove all indentation (CNT = 0).  A tab is taken from the text
+above.  If no suitable tab is found `rst-indent-width' is used."
   (interactive "r\np")
   (let ((tabs (sort (rst-compute-tabs beg) (lambda (x y) (<= x y))))
 	(leftmostcol (rst-find-leftmost-column beg end)))
     (when (or (> leftmostcol 0) (> cnt 0))
-      ;; Apply the indent
+      ;; Apply the indent.
       (indent-rigidly
        beg end
        (if (zerop cnt)
 	   (- leftmostcol)
-	 ;; Find the next tab after the leftmost column
+	 ;; Find the next tab after the leftmost column.
 	 (let* ((cmp (if (> cnt 0) '> '<))
 		(tabs (if (> cnt 0) tabs (reverse tabs)))
 		(len (length tabs))
-		(dir (signum cnt)) ; Direction to take
-		(abs (abs cnt)) ; Absolute number of steps to take
-		;; Get the position of the first tab beyond leftmostcol
-		(fnd (position-if (lambda (elt)
-				    (funcall cmp elt leftmostcol))
-				  tabs))
-		;; Virtual position of tab
+		(dir (rst-signum cnt)) ; Direction to take.
+		(abs (abs cnt)) ; Absolute number of steps to take.
+		;; Get the position of the first tab beyond leftmostcol.
+		(fnd (lexical-let ((cmp cmp)
+				   (leftmostcol leftmostcol)) ; Create closure.
+		       (rst-position-if (lambda (elt)
+					  (funcall cmp elt leftmostcol))
+					tabs)))
+		;; Virtual position of tab.
 		(pos (+ (or fnd len) (1- abs)))
 		(tab (if (< pos len)
-			 ;; Tab exists - use it
+			 ;; Tab exists - use it.
 			 (nth pos tabs)
-		       ;; Column needs to be computed
+		       ;; Column needs to be computed.
 		       (let ((col (+ (or (car (last tabs)) leftmostcol)
-				     ;; Base on last known column
-				     (* (- pos (1- len)) ; Distance left
-					dir ; Direction to take
+				     ;; Base on last known column.
+				     (* (- pos (1- len)) ; Distance left.
+					dir ; Direction to take.
 					rst-indent-width))))
 			 (if (< col 0) 0 col)))))
 	   (- tab leftmostcol)))))))
 
 ;; FIXME: A paragraph with an (incorrectly) indented second line is not filled
-;; correctly::
+;;        correctly::
 ;;
-;;   Some start
-;;     continued wrong
+;;          Some start
+;;            continued wrong
 (defun rst-adaptive-fill ()
   "Return fill prefix found at point.
 Value for `adaptive-fill-function'."
   (let ((fnd (if (looking-at adaptive-fill-regexp)
 		 (match-string-no-properties 0))))
     (if (save-match-data
 	  (not (string-match comment-start-skip fnd)))
-	;; An non-comment prefix is fine
+	;; An non-comment prefix is fine.
 	fnd
-      ;; Matches a comment - return whitespace instead
+      ;; Matches a comment - return whitespace instead.
       (make-string (-
 		    (save-excursion
 		      (goto-char (match-end 0))
 		      (current-column))
 		    (save-excursion
 		      (goto-char (match-beginning 0))
 		      (current-column))) ? ))))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Comments
 
 (defun rst-comment-line-break (&optional soft)
   "Break line and indent, continuing reStructuredText comment if within one.
-Value for `comment-line-break-function'."
+Value for `comment-line-break-function'.  If SOFT use soft
+newlines as mandated by `comment-line-break-function'."
   (if soft
       (insert-and-inherit ?\n)
     (newline 1))
   (save-excursion
     (forward-char -1)
     (delete-horizontal-space))
   (delete-horizontal-space)
@@ -3016,15 +3056,16 @@
 
 (defun rst-comment-insert-comment ()
   "Insert a comment in the current line."
   (rst-indent-line 0)
   (insert comment-start))
 
 (defun rst-comment-region (beg end &optional arg)
-  "Comment the current region or uncomment it if ARG is \\[universal-argument]."
+  "Comment or uncomment the current region.
+Region is from from BEG to END.  Uncomment if ARG."
   (save-excursion
     (if (consp arg)
 	(rst-uncomment-region beg end arg)
       (goto-char beg)
       (let ((ind (current-indentation))
 	    bol)
 	(forward-line 0)
@@ -3033,30 +3074,30 @@
 	(goto-char bol)
 	(open-line 1)
 	(indent-line-to ind)
 	(insert (comment-string-strip comment-start t t))))))
 
 (defun rst-uncomment-region (beg end &optional arg)
   "Uncomment the current region.
-ARG is ignored"
+Region is from BEG to END.  ARG is ignored"
   (save-excursion
     (let (bol eol)
       (goto-char beg)
       (forward-line 0)
       (setq bol (point))
       (forward-line 1)
       (setq eol (point))
       (indent-rigidly eol end (- rst-indent-comment))
       (delete-region bol eol))))
 
 ;;------------------------------------------------------------------------------
 
-;; FIXME: these next functions should become part of a larger effort to redo the
-;; bullets in bulleted lists.  The enumerate would just be one of the possible
-;; outputs.
+;; FIXME: These next functions should become part of a larger effort to redo
+;;        the bullets in bulleted lists.  The enumerate would just be one of
+;;        the possible outputs.
 ;;
 ;; FIXME: We need to do the enumeration removal as well.
 
 (defun rst-enumerate-region (beg end all)
   "Add enumeration to all the leftmost paragraphs in the given region.
 The region is specified between BEG and END.  With ALL,
 do all lines instead of just paragraphs."
@@ -3078,20 +3119,20 @@
   (interactive "r\nP")
   (rst-iterate-leftmost-paragraphs
    beg end (not all)
    (insert (car rst-preferred-bullets) " ")
    (insert "  ")
    ))
 
-;; FIXME: Does not deal with a varying number of digits appropriately
-;; FIXME: Does not deal with multiple levels independently
-;; FIXME: Does not indent a multiline item correctly
+;; FIXME: Does not deal with a varying number of digits appropriately.
+;; FIXME: Does not deal with multiple levels independently.
+;; FIXME: Does not indent a multiline item correctly.
 (defun rst-convert-bullets-to-enumeration (beg end)
   "Convert the bulleted and enumerated items in the region to enumerated lists.
-Renumber as necessary."
+Renumber as necessary.  Region is from BEG to END."
   (interactive "r")
   (let* (;; Find items and convert the positions to markers.
 	 (items (mapcar
 		 (lambda (x)
 		   (cons (copy-marker (car x))
 			 (cdr x)))
 		 (rst-find-pfx-in-region beg end (rst-re 'itmany-sta-1))))
@@ -3108,15 +3149,15 @@
 
 
 
 ;;------------------------------------------------------------------------------
 
 (defun rst-line-block-region (rbeg rend &optional pfxarg)
   "Toggle line block prefixes for a region.
-With prefix argument set the empty lines too."
+Region is from RBEG to REND.  With PFXARG set the empty lines too."
   (interactive "r\nP")
   (let ((comment-start "| ")
 	(comment-end "")
 	(comment-start-skip "| ")
 	(comment-style 'indent)
 	(force (not (not pfxarg))))
     (rst-iterate-leftmost-paragraphs-2
@@ -3130,15 +3171,18 @@
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Font lock
 ;; =========
 
 (require 'font-lock)
 
-;; FIXME: The obsolete variables need to disappear
+;; FIXME: The obsolete variables need to disappear.
+
+;; The following versions have been done inside Emacs and should not be
+;; replaced by `:package-version' attributes until a change.
 
 (defgroup rst-faces nil "Faces used in Rst Mode."
   :group 'rst
   :group 'faces
   :version "21.1")
 
 (defface rst-block '((t :inherit font-lock-keyword-face))
@@ -3264,48 +3308,76 @@
   :version "24.1"
   :group 'rst-faces
   :type '(face))
 (make-obsolete-variable 'rst-reference-face
                         "customize the face `rst-reference' instead."
                         "24.1")
 
+(defface rst-transition '((t :inherit font-lock-keyword-face))
+  "Face used for a transition."
+  :package-version '(rst . "1.3.0")
+  :group 'rst-faces)
+
+(defface rst-adornment '((t :inherit font-lock-keyword-face))
+  "Face used for the adornment of a section header."
+  :package-version '(rst . "1.3.0")
+  :group 'rst-faces)
+
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
+;; FIXME LEVEL-FACE: May be this complicated mechanism should be replaced
+;;                   simply by a number of customizable faces `rst-header-%d'
+;;                   which by default are set properly for dark and light
+;;                   background.  Initialization should come from the old
+;;                   variables if they exist.  A maximum level of 6 should
+;;                   suffice - after that the last level should be repeated.
+;;                   Only `rst-adornment-faces-alist' is needed outside this
+;;                   block.  Would also fix docutils-Bugs-3479594.
+
 (defgroup rst-faces-defaults nil
   "Values used to generate default faces for section titles on all levels.
 Tweak these if you are content with how section title faces are built in
 general but you do not like the details."
   :group 'rst-faces
   :version "21.1")
 
 (defun rst-set-level-default (sym val)
-  "Set custom var SYM affecting section title text face and recompute the faces."
+  "Set custom variable SYM affecting section title text face.
+Recompute the faces.  VAL is the value to set."
   (custom-set-default sym val)
-  ;; Also defines the faces initially when all values are available
+  ;; Also defines the faces initially when all values are available.
   (and (boundp 'rst-level-face-max)
        (boundp 'rst-level-face-format-light)
        (boundp 'rst-level-face-base-color)
        (boundp 'rst-level-face-step-light)
        (boundp 'rst-level-face-base-light)
        (fboundp 'rst-define-level-faces)
        (rst-define-level-faces)))
 
-;; Faces for displaying items on several levels; these definitions define
-;; different shades of gray where the lightest one (i.e. least contrasting) is
-;; used for level 1
+;; Faces for displaying items on several levels.  These definitions define
+;; different shades of gray where the lightest one (i.e. least contrasting on a
+;; light background) is used for level 1.
 (defcustom rst-level-face-max 6
   "Maximum depth of levels for which section title faces are defined."
   :group 'rst-faces-defaults
   :type '(integer)
   :set 'rst-set-level-default)
+;; FIXME: It should be possible to give "#RRGGBB" type of color values.
+;;        Together with a `rst-level-face-end-light' this could be used for
+;;        computing steps.
+;; FIXME: This variable should be combined with `rst-level-face-format-light'
+;;        to a single string.
 (defcustom rst-level-face-base-color "grey"
   "Base name of the color for creating background colors in section title faces."
   :group 'rst-faces-defaults
   :type '(string)
   :set 'rst-set-level-default)
+;; FIXME LEVEL-FACE: This needs to be done differently: The faces must specify
+;;                   how they behave for dark and light background using the
+;;                   relevant options explained in `defface'.
 (defcustom rst-level-face-base-light
   (if (eq frame-background-mode 'dark)
       15
     85)
   "The lightness factor for the base color.  This value is used for level 1.
 The default depends on whether the value of `frame-background-mode' is
 `dark' or not."
@@ -3314,14 +3386,20 @@
   :set 'rst-set-level-default)
 (defcustom rst-level-face-format-light "%2d"
   "The format for the lightness factor appended to the base name of the color.
 This value is expanded by `format' with an integer."
   :group 'rst-faces-defaults
   :type '(string)
   :set 'rst-set-level-default)
+;; FIXME LEVEL-FACE: This needs to be done differently: The faces must specify
+;;                   how they behave for dark and light background using the
+;;                   relevant options explained in `defface'.
+;; FIXME: Alternatively there could be a customizable variable
+;;        `rst-level-face-end-light' which defines the end value and steps are
+;;        computed
 (defcustom rst-level-face-step-light
   (if (eq frame-background-mode 'dark)
       7
     -7)
   "The step width to use for the next color.
 The formula
 
@@ -3333,89 +3411,95 @@
 This color is used as background for section title text on level
 `rst-level-face-max'."
   :group 'rst-faces-defaults
   :type '(integer)
   :set 'rst-set-level-default)
 
 (defcustom rst-adornment-faces-alist
-  (let ((alist '((t . font-lock-keyword-face)
-		 (nil . font-lock-keyword-face)))
+  ;; FIXME LEVEL-FACE: Must be redone if `rst-level-face-max' is changed
+  (let ((alist (copy-list '((t . rst-transition)
+			    (nil . rst-adornment))))
 	(i 1))
     (while (<= i rst-level-face-max)
       (nconc alist (list (cons i (intern (format "rst-level-%d-face" i)))))
       (setq i (1+ i)))
     alist)
   "Faces for the various adornment types.
-Key is a number (for the section title text of that level),
-t (for transitions) or nil (for section title adornment).
-If you generally do not like how section title text faces are
-set up tweak here.  If the general idea is ok for you but you do not like the
-details check the Rst Faces Defaults group."
+Key is a number (for the section title text of that level
+starting with 1), t (for transitions) or nil (for section title
+adornment).  If you generally do not like how section title text
+faces are set up tweak here.  If the general idea is ok for you
+but you do not like the details check the Rst Faces Defaults
+group."
   :group 'rst-faces
   :type '(alist
 	  :key-type
 	  (choice
-	   (integer
-	    :tag
-	    "Section level (may not be bigger than `rst-level-face-max')")
-	   (boolean :tag "transitions (on) / section title adornment (off)"))
+	   (integer :tag "Section level")
+	   (const :tag "transitions" t)
+	   (const :tag "section title adornment" nil))
 	  :value-type (face))
   :set-after '(rst-level-face-max))
 
-;; FIXME: It should be possible to give "#RRGGBB" type of color values
 (defun rst-define-level-faces ()
   "Define the faces for the section title text faces from the values."
-  ;; All variables used here must be checked in `rst-set-level-default'
+  ;; All variables used here must be checked in `rst-set-level-default'.
   (let ((i 1))
     (while (<= i rst-level-face-max)
       (let ((sym (intern (format "rst-level-%d-face" i)))
-	    (doc (format "Face for showing section title text at level %d" i))
+	    (doc (format "Default face for showing section title text at level %d.
+This symbol is *not* meant for customization but modified if a
+variable of the `rst-faces-defaults' group is customized. Use
+`rst-adornment-faces-alist' for customization instead." i))
 	    (col (format (concat "%s" rst-level-face-format-light)
 			 rst-level-face-base-color
 			 (+ (* (1- i) rst-level-face-step-light)
 			    rst-level-face-base-light))))
-        (unless (facep sym)
-          (make-empty-face sym)
-          (set-face-doc-string sym doc)
-          (set-face-background sym col)
-          (set sym sym))
+	(make-empty-face sym)
+	(set-face-doc-string sym doc)
+	(set-face-background sym col)
+	(set sym sym)
 	(setq i (1+ i))))))
 
+;; FIXME LEVEL-FACE: This is probably superfluous since it is done by the
+;;                   customization / `rst-set-level-default'.
 (rst-define-level-faces)
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
 (defvar rst-font-lock-keywords
   ;; The reST-links in the comments below all relate to sections in
-  ;; http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html
+  ;; http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html.
   `(;; FIXME: Block markup is not recognized in blocks after explicit markup
-    ;; start
+    ;;        start.
 
     ;; Simple `Body Elements`_
     ;; `Bullet Lists`_
-    ;; FIXME: A bullet directly after a field name is not recognized
+    ;; FIXME: A bullet directly after a field name is not recognized.
     (,(rst-re 'lin-beg '(:grp bul-sta))
      1 rst-block-face)
     ;; `Enumerated Lists`_
     (,(rst-re 'lin-beg '(:grp enmany-sta))
      1 rst-block-face)
-    ;; `Definition Lists`_ FIXME: missing
+    ;; `Definition Lists`_
+    ;; FIXME: missing.
     ;; `Field Lists`_
     (,(rst-re 'lin-beg '(:grp fld-tag) 'bli-sfx)
      1 rst-external-face)
     ;; `Option Lists`_
     (,(rst-re 'lin-beg '(:grp opt-tag (:shy optsep-tag opt-tag) "*")
 	      '(:alt "$" (:seq hws-prt "\\{2\\}")))
      1 rst-block-face)
     ;; `Line Blocks`_
-    ;; Only for lines containing no more bar - to distinguish from tables
+    ;; Only for lines containing no more bar - to distinguish from tables.
     (,(rst-re 'lin-beg '(:grp "|" bli-sfx) "[^|\n]*$")
      1 rst-block-face)
 
-    ;; `Tables`_ FIXME: missing
+    ;; `Tables`_
+    ;; FIXME: missing
 
     ;; All the `Explicit Markup Blocks`_
     ;; `Footnotes`_ / `Citations`_
     (,(rst-re 'lin-beg 'fnc-sta-2)
      (1 rst-definition-face)
      (2 rst-definition-face))
     ;; `Directives`_ / `Substitution Definitions`_
@@ -3429,34 +3513,34 @@
 				  (:seq "`" ilcbkqdef-tag "`")
 				  (:seq (:alt "[^:\\\n]" "\\\\.") "+")) ":")
 	      'bli-sfx)
      1 rst-definition-face)
     (,(rst-re 'lin-beg '(:grp "__") 'bli-sfx)
      1 rst-definition-face)
 
-    ;; All `Inline Markup`_ - most of them may be multiline though this is
-    ;; uninteresting
+    ;; All `Inline Markup`_
+    ;; Most of them may be multiline though this is uninteresting.
 
     ;; FIXME: Condition 5 preventing fontification of e.g. "*" not implemented
-    ;; `Strong Emphasis`_
+    ;;        `Strong Emphasis`_.
     (,(rst-re 'ilm-pfx '(:grp "\\*\\*" ilcast-tag "\\*\\*") 'ilm-sfx)
      1 rst-emphasis2-face)
     ;; `Emphasis`_
     (,(rst-re 'ilm-pfx '(:grp "\\*" ilcast-tag "\\*") 'ilm-sfx)
      1 rst-emphasis1-face)
     ;; `Inline Literals`_
     (,(rst-re 'ilm-pfx '(:grp "``" ilcbkq-tag "``") 'ilm-sfx)
      1 rst-literal-face)
     ;; `Inline Internal Targets`_
     (,(rst-re 'ilm-pfx '(:grp "_`" ilcbkq-tag "`") 'ilm-sfx)
      1 rst-definition-face)
     ;; `Hyperlink References`_
-    ;; FIXME: `Embedded URIs`_ not considered
-    ;; FIXME: Directly adjacing marked up words are not fontified correctly
-    ;;        unless they are not separated by two spaces: foo_ bar_
+    ;; FIXME: `Embedded URIs`_ not considered.
+    ;; FIXME: Directly adjacent marked up words are not fontified correctly
+    ;;        unless they are not separated by two spaces: foo_ bar_.
     (,(rst-re 'ilm-pfx '(:grp (:alt (:seq "`" ilcbkq-tag "`")
 				    (:seq "\\sw" (:alt "\\sw" "-") "+\\sw"))
 			      "__?") 'ilm-sfx)
      1 rst-reference-face)
     ;; `Interpreted Text`_
     (,(rst-re 'ilm-pfx '(:grp (:shy ":" sym-tag ":") "?")
 	      '(:grp "`" ilcbkq-tag "`")
@@ -3465,46 +3549,48 @@
      (2 rst-external-face)
      (3 rst-directive-face))
     ;; `Footnote References`_ / `Citation References`_
     (,(rst-re 'ilm-pfx '(:grp fnc-tag "_") 'ilm-sfx)
      1 rst-reference-face)
     ;; `Substitution References`_
     ;; FIXME: References substitutions like |this|_ or |this|__ are not
-    ;;        fontified correctly
+    ;;        fontified correctly.
     (,(rst-re 'ilm-pfx '(:grp sub-tag) 'ilm-sfx)
      1 rst-reference-face)
     ;; `Standalone Hyperlinks`_
-    ;; FIXME: This takes it easy by using a whitespace as delimiter
+    ;; FIXME: This takes it easy by using a whitespace as delimiter.
     (,(rst-re 'ilm-pfx '(:grp uri-tag ":\\S +") 'ilm-sfx)
      1 rst-definition-face)
     (,(rst-re 'ilm-pfx '(:grp sym-tag "@" sym-tag ) 'ilm-sfx)
      1 rst-definition-face)
 
-    ;; Do all block fontification as late as possible so 'append works
+    ;; Do all block fontification as late as possible so 'append works.
 
-    ;; Sections_ / Transitions_ - for sections this is multiline
+    ;; Sections_ / Transitions_
+    ;; For sections this is multiline.
     (,(rst-re 'ado-beg-2-1)
      (rst-font-lock-handle-adornment-matcher
       (rst-font-lock-handle-adornment-pre-match-form
        (match-string-no-properties 1) (match-end 1))
       nil
       (1 (cdr (assoc nil rst-adornment-faces-alist)) append t)
       (2 (cdr (assoc rst-font-lock-adornment-level
 		     rst-adornment-faces-alist)) append t)
       (3 (cdr (assoc nil rst-adornment-faces-alist)) append t)))
 
     ;; FIXME: FACESPEC could be used instead of ordinary faces to set
     ;;        properties on comments and literal blocks so they are *not*
-    ;;        inline fontified; see (elisp)Search-based Fontification
+    ;;        inline fontified.  See (elisp)Search-based Fontification.
 
     ;; FIXME: And / or use `syntax-propertize` functions as in `octave-mod.el`
-    ;;        and other V24 modes; may make `font-lock-extend-region`
-    ;;        superfluous
+    ;;        and other V24 modes.  May make `font-lock-extend-region`
+    ;;        superfluous.
 
-    ;; `Comments`_ - this is multiline
+    ;; `Comments`_
+    ;; This is multiline.
     (,(rst-re 'lin-beg 'cmt-sta-1)
      (1 rst-comment-face)
      (rst-font-lock-find-unindented-line-match
       (rst-font-lock-find-unindented-line-limit (match-end 1))
       nil
       (0 rst-comment-face append)))
     (,(rst-re 'lin-beg '(:grp exm-tag) '(:grp hws-tag) "$")
@@ -3512,17 +3598,17 @@
      (2 rst-comment-face)
      (rst-font-lock-find-unindented-line-match
       (rst-font-lock-find-unindented-line-limit 'next)
       nil
       (0 rst-comment-face append)))
 
     ;; FIXME: This is not rendered as comment::
-    ;; .. .. list-table::
-    ;;       :stub-columns: 1
-    ;;       :header-rows: 1
+    ;;        .. .. list-table::
+    ;;              :stub-columns: 1
+    ;;              :header-rows: 1
 
     ;; FIXME: This is rendered wrong::
     ;;
     ;; 	 xxx yyy::
     ;;
     ;; 	 			----|> KKKKK <|----
     ;; 	 		       /	     	    \
@@ -3530,23 +3616,25 @@
     ;; 	    |			   |	     	 |     	       	       	 |
     ;; 	    |			   |		 |			 |
     ;; 	    PPPPPP     PPPPPPDDDDDDD             BBBBBBB     PPPPPPBBBBBBB
     ;;
     ;; Indentation needs to be taken from the line with the ``::`` and not from
     ;; the first content line.
 
-    ;; `Indented Literal Blocks`_ - this is multiline
+    ;; `Indented Literal Blocks`_
+    ;; This is multiline.
     (,(rst-re 'lin-beg 'lit-sta-2)
      (2 rst-block-face)
      (rst-font-lock-find-unindented-line-match
       (rst-font-lock-find-unindented-line-limit t)
       nil
       (0 rst-literal-face append)))
 
-    ;; FIXME: `Quoted Literal Blocks`_ missing - this is multiline
+    ;; FIXME: `Quoted Literal Blocks`_ missing.
+    ;; This is multiline.
 
     ;; `Doctest Blocks`_
     ;; FIXME: This is wrong according to the specification:
     ;;
     ;;   Doctest blocks are text blocks which begin with ">>> ", the Python
     ;;   interactive interpreter main prompt, and end with a blank line.
     ;;   Doctest blocks are treated as a special case of literal blocks,
@@ -3567,90 +3655,97 @@
     ;;   Indentation is not required for doctest blocks.
     (,(rst-re 'lin-beg '(:grp (:alt ">>>" ell-tag)) '(:grp ".+"))
      (1 rst-block-face)
      (2 rst-literal-face))
     )
   "Keywords to highlight in rst mode.")
 
+(defvar font-lock-beg)
+(defvar font-lock-end)
+
 (defun rst-font-lock-extend-region ()
-  "Extend the region `font-lock-beg' / `font-lock-end' iff it may
-be in the middle of a multiline construct and return non-nil if so."
+  "Extend the font-lock region if it might be in a multi-line construct.
+Return non-nil if so.  Font-lock region is from `font-lock-beg'
+to `font-lock-end'."
   (let ((r (rst-font-lock-extend-region-internal font-lock-beg font-lock-end)))
     (when r
       (setq font-lock-beg (car r))
       (setq font-lock-end (cdr r))
       t)))
 
 (defun rst-font-lock-extend-region-internal (beg end)
-  "Check the region BEG / END for being in the middle of a multiline construct.
+  "Check the region BEG / END for being in the middle of a multi-line construct.
 Return nil if not or a cons with new values for BEG / END"
   (let ((nbeg (rst-font-lock-extend-region-extend beg -1))
 	(nend (rst-font-lock-extend-region-extend end 1)))
     (if (or nbeg nend)
 	(cons (or nbeg beg) (or nend end)))))
 
 (defun rst-forward-line (&optional n)
-  "Like `forward-line' but always end up in column 0 and return accordingly."
+  "Like `forward-line' but always end up in column 0 and return accordingly.
+Move N lines forward just as `forward-line'."
   (let ((moved (forward-line n)))
     (if (bolp)
 	moved
       (forward-line 0)
-      (- moved (signum n)))))
+      (- moved (rst-signum n)))))
 
+;; FIXME: If a single line is made a section header by `rst-adjust' the header
+;;        is not always fontified immediately.
 (defun rst-font-lock-extend-region-extend (pt dir)
   "Extend the region starting at point PT and extending in direction DIR.
 Return extended point or nil if not moved."
   ;; There are many potential multiline constructs but there are two groups
   ;; which are really relevant. The first group consists of
   ;;
   ;; * comment lines without leading explicit markup tag and
   ;;
   ;; * literal blocks following "::"
   ;;
-  ;; which are both indented. Thus indendation is the first thing recognized
+  ;; which are both indented. Thus indentation is the first thing recognized
   ;; here. The second criteria is an explicit markup tag which may be a comment
   ;; or a double colon at the end of a line.
   ;;
   ;; The second group consists of the adornment cases.
   (if (not (get-text-property pt 'font-lock-multiline))
-      ;; Move only if we don't start inside a multiline construct already
+      ;; Move only if we don't start inside a multiline construct already.
       (save-excursion
-	(let (;; non-empty non-indented line, explicit markup tag or literal
-	      ;; block tag
+	(let (;; Non-empty non-indented line, explicit markup tag or literal
+	      ;; block tag.
 	      (stop-re (rst-re '(:alt "[^ \t\n]"
 				      (:seq hws-tag exm-tag)
 				      (:seq ".*" dcl-tag lin-end)))))
-	  ;; The comments below are for dir == -1 / dir == 1
+	  ;; The comments below are for dir == -1 / dir == 1.
 	  (goto-char pt)
 	  (forward-line 0)
 	  (setq pt (point))
 	  (while (and (not (looking-at stop-re))
 		      (zerop (rst-forward-line dir)))) ; try previous / next
-						       ; line if it exists
+						       ; line if it exists.
 	  (if (looking-at (rst-re 'ado-beg-2-1)) ; may be an underline /
-						 ; overline
+						 ; overline.
 	      (if (zerop (rst-forward-line dir))
 		  (if (looking-at (rst-re 'ttl-beg)) ; title found, i.e.
 						     ; underline / overline
-						     ; found
+						     ; found.
 		      (if (zerop (rst-forward-line dir))
 			  (if (not
 			       (looking-at (rst-re 'ado-beg-2-1))) ; no
 								   ; overline /
-								   ; underline
+								   ; underline.
 			      (rst-forward-line (- dir)))) ; step back to title
-							   ; / adornment
-		    (if (< dir 0) ; keep downward adornment
-			(rst-forward-line (- dir))))) ; step back to adornment
-	    (if (looking-at (rst-re 'ttl-beg)) ; may be a title
+							   ; / adornment.
+		    (if (< dir 0) ; keep downward adornment.
+			(rst-forward-line (- dir))))) ; step back to adornment.
+	    (if (looking-at (rst-re 'ttl-beg)) ; may be a title.
 		(if (zerop (rst-forward-line dir))
 		    (if (not
 			 (looking-at (rst-re 'ado-beg-2-1))) ; no overline /
-							     ; underline
-			(rst-forward-line (- dir)))))) ; step back to line
+							     ; underline.
+			(rst-forward-line (- dir)))))) ; step back to line.
 	  (if (not (= (point) pt))
 	      (point))))))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Indented blocks
 
 (defun rst-forward-indented-block (&optional column limit)
@@ -3668,150 +3763,160 @@
 	(setq limit (point-max)))
     (save-match-data
       (while (and (not fnd) (< (point) limit))
 	(forward-line 1)
 	(when (< (point) limit)
 	  (setq beg (point))
 	  (if (looking-at (rst-re 'lin-end))
-	      (setq cand (or cand beg)) ; An empty line is a candidate
+	      (setq cand (or cand beg)) ; An empty line is a candidate.
 	    (move-to-column clm)
 	    ;; FIXME: No indentation [(zerop clm)] must be handled in some
-	    ;; useful way - though it is not clear what this should mean at all
+	    ;;        useful way - though it is not clear what this should mean
+	    ;;        at all.
 	    (if (string-match
 		 (rst-re 'linemp-tag)
 		 (buffer-substring-no-properties beg (point)))
-		(setq cand nil) ; An indented line resets a candidate
+		(setq cand nil) ; An indented line resets a candidate.
 	      (setq fnd (or cand beg)))))))
     (goto-char (or fnd start))
     fnd))
 
 (defvar rst-font-lock-find-unindented-line-begin nil
-  "Beginning of the match if `rst-font-lock-find-unindented-line-end'")
+  "Beginning of the match if `rst-font-lock-find-unindented-line-end'.")
 
 (defvar rst-font-lock-find-unindented-line-end nil
   "End of the match as determined by `rst-font-lock-find-unindented-line-limit'.
 Also used as a trigger for
 `rst-font-lock-find-unindented-line-match'.")
 
 (defun rst-font-lock-find-unindented-line-limit (ind-pnt)
-  "Find the next unindented line relative to indenation at IND-PNT.
+  "Find the next unindented line relative to indentation at IND-PNT.
 Return this point, the end of the buffer or nil if nothing found.
 If IND-PNT is `next' take the indentation from the next line if
-this is not empty and indented more than the current one. If
+this is not empty and indented more than the current one.  If
 IND-PNT is non-nil but not a number take the indentation from the
 next non-empty line if this is indented more than the current
 one."
   (setq rst-font-lock-find-unindented-line-begin ind-pnt)
   (setq rst-font-lock-find-unindented-line-end
 	(save-excursion
 	  (when (not (numberp ind-pnt))
-	    ;; Find indentation point in next line if any
+	    ;; Find indentation point in next line if any.
 	    (setq ind-pnt
 		  ;; FIXME: Should be refactored to two different functions
 		  ;;        giving their result to this function, may be
-		  ;;        integrated in caller
+		  ;;        integrated in caller.
 		  (save-match-data
 		    (let ((cur-ind (current-indentation)))
 		      (if (eq ind-pnt 'next)
 			  (when (and (zerop (forward-line 1))
 				     (< (point) (point-max)))
-			    ;; Not at EOF
+			    ;; Not at EOF.
 			    (setq rst-font-lock-find-unindented-line-begin
 				  (point))
 			    (when (and (not (looking-at (rst-re 'lin-end)))
 				       (> (current-indentation) cur-ind))
-			        ;; Use end of indentation if non-empty line
+			        ;; Use end of indentation if non-empty line.
 				(looking-at (rst-re 'hws-tag))
 				(match-end 0)))
-			;; Skip until non-empty line or EOF
+			;; Skip until non-empty line or EOF.
 			(while (and (zerop (forward-line 1))
 				    (< (point) (point-max))
 				    (looking-at (rst-re 'lin-end))))
 			(when (< (point) (point-max))
-			  ;; Not at EOF
+			  ;; Not at EOF.
 			  (setq rst-font-lock-find-unindented-line-begin
 				(point))
 			  (when (> (current-indentation) cur-ind)
-			    ;; Indentation bigger than line of departure
+			    ;; Indentation bigger than line of departure.
 			    (looking-at (rst-re 'hws-tag))
 			    (match-end 0))))))))
 	  (when ind-pnt
 	    (goto-char ind-pnt)
 	    (or (rst-forward-indented-block nil (point-max))
 		(point-max))))))
 
 (defun rst-font-lock-find-unindented-line-match (limit)
-  "Set the match found by
+  "Set the match found earlier if match were found.
+Match has been found by
 `rst-font-lock-find-unindented-line-limit' the first time called
-or nil."
+or no match is found.  Return non-nil if match was found.  LIMIT
+is not used but mandated by the caller."
   (when rst-font-lock-find-unindented-line-end
     (set-match-data
      (list rst-font-lock-find-unindented-line-begin
 	   rst-font-lock-find-unindented-line-end))
     (put-text-property rst-font-lock-find-unindented-line-begin
 		       rst-font-lock-find-unindented-line-end
 		       'font-lock-multiline t)
-    ;; Make sure this is called only once
+    ;; Make sure this is called only once.
     (setq rst-font-lock-find-unindented-line-end nil)
     t))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Adornments
 
 (defvar rst-font-lock-adornment-level nil
   "Storage for `rst-font-lock-handle-adornment-matcher'.
 Either section level of the current adornment or t for a transition.")
 
 (defun rst-adornment-level (key)
   "Return section level for adornment KEY.
 KEY is the first element of the return list of
-`rst-classify-adornment'. If KEY is not a cons return it. If KEY is found
-in the hierarchy return its level. Otherwise return a level one
+`rst-classify-adornment'.  If KEY is not a cons return it.  If KEY is found
+in the hierarchy return its level.  Otherwise return a level one
 beyond the existing hierarchy."
   (if (not (consp key))
       key
     (let* ((hier (rst-get-hierarchy))
 	   (char (car key))
 	   (style (cdr key)))
-      (1+ (or (position-if (lambda (elt)
-			     (and (equal (car elt) char)
-				  (equal (cadr elt) style))) hier)
+      (1+ (or (lexical-let ((char char)
+			    (style style)
+			    (hier hier)) ; Create closure.
+		(rst-position-if (lambda (elt)
+				   (and (equal (car elt) char)
+					(equal (cadr elt) style))) hier))
 	      (length hier))))))
 
 (defvar rst-font-lock-adornment-match nil
   "Storage for match for current adornment.
-Set by `rst-font-lock-handle-adornment-pre-match-form'. Also used
+Set by `rst-font-lock-handle-adornment-pre-match-form'.  Also used
 as a trigger for `rst-font-lock-handle-adornment-matcher'.")
 
 (defun rst-font-lock-handle-adornment-pre-match-form (ado ado-end)
-  "Determine limit for adornments for font-locking section titles and transitions.
-In fact determine all things necessary and put the result to
+  "Determine limit for adornments.
+Determine all things necessary for font-locking section titles
+and transitions and put the result to
 `rst-font-lock-adornment-match' and
-`rst-font-lock-adornment-level'. ADO is the complete adornment
-matched. ADO-END is the point where ADO ends. Return the point
+`rst-font-lock-adornment-level'.  ADO is the complete adornment
+matched.  ADO-END is the point where ADO ends.  Return the point
 where the whole adorned construct ends.
 
 Called as a PRE-MATCH-FORM in the sense of `font-lock-keywords'."
   (let ((ado-data (rst-classify-adornment ado ado-end)))
     (if (not ado-data)
 	(setq rst-font-lock-adornment-level nil
 	      rst-font-lock-adornment-match nil)
       (setq rst-font-lock-adornment-level
 	    (rst-adornment-level (car ado-data)))
       (setq rst-font-lock-adornment-match (cdr ado-data))
-      (goto-char (nth 1 ado-data)) ; Beginning of construct
-      (nth 2 ado-data)))) ; End of construct
+      (goto-char (nth 1 ado-data)) ; Beginning of construct.
+      (nth 2 ado-data)))) ; End of construct.
 
 (defun rst-font-lock-handle-adornment-matcher (limit)
-  "Set the match found by `rst-font-lock-handle-adornment-pre-match-form'
-the first time called or nil.
+  "Set the match found earlier if match were found.
+Match has been found by
+`rst-font-lock-handle-adornment-pre-match-form' the first time
+called or no match is found.  Return non-nil if match was found.
 
-Called as a MATCHER in the sense of `font-lock-keywords'."
+Called as a MATCHER in the sense of `font-lock-keywords'.
+LIMIT is not used but mandated by the caller."
   (let ((match rst-font-lock-adornment-match))
-    ;; May run only once - enforce this
+    ;; May run only once - enforce this.
     (setq rst-font-lock-adornment-match nil)
     (when match
       (set-match-data match)
       (goto-char (match-end 0))
       (put-text-property (match-beginning 0) (match-end 0)
 			 'font-lock-multiline t)
       t)))
@@ -3839,38 +3944,38 @@
                ".xml" nil)
     (xml ,(if (executable-find "rst2xml.py") "rst2xml.py" "rst2xml")
          ".xml" nil)
     (pdf ,(if (executable-find "rst2pdf.py") "rst2pdf.py" "rst2pdf")
          ".pdf" nil)
     (s5 ,(if (executable-find "rst2s5.py") "rst2s5.py" "rst2s5")
         ".html" nil))
-  "Table describing the command to use for each toolset.
-An association list of the toolset to a list of the (command to use,
+  "Table describing the command to use for each tool-set.
+An association list of the tool-set to a list of the (command to use,
 extension of produced filename, options to the tool (nil or a
 string)) to be used for converting the document."
   ;; FIXME: These are not options but symbols which may be referenced by
-  ;; `rst-compile-*-toolset` below
+  ;;        `rst-compile-*-toolset` below.
   :type '(alist :options (html latex newlatex pseudoxml xml pdf s5)
                 :key-type symbol
                 :value-type (list :tag "Specification"
                              (file :tag "Command")
                              (string :tag "File extension")
                              (choice :tag "Command options"
                                      (const :tag "No options" nil)
                                      (string :tag "Options"))))
   :group 'rst
-  :version "24.1")
+  :package-version "1.2.0")
 
-;; FIXME: Must be `defcustom`
+;; FIXME: Must be `defcustom`.
 (defvar rst-compile-primary-toolset 'html
-  "The default toolset for `rst-compile'.")
+  "The default tool-set for `rst-compile'.")
 
-;; FIXME: Must be `defcustom`
+;; FIXME: Must be `defcustom`.
 (defvar rst-compile-secondary-toolset 'latex
-  "The default toolset for `rst-compile' with a prefix argument.")
+  "The default tool-set for `rst-compile' with a prefix argument.")
 
 (defun rst-compile-find-conf ()
   "Look for the configuration file in the parents of the current path."
   (interactive)
   (let ((file-name "docutils.conf")
         (buffer-file (buffer-file-name)))
     ;; Move up in the dir hierarchy till we find a change log file.
@@ -3892,15 +3997,15 @@
 
 (require 'compile)
 
 (defun rst-compile (&optional use-alt)
   "Compile command to convert reST document into some output file.
 Attempts to find configuration file, if it can, overrides the
 options.  There are two commands to choose from, with USE-ALT,
-select the alternative toolset."
+select the alternative tool-set."
   (interactive "P")
   ;; Note: maybe we want to check if there is a Makefile too and not do anything
   ;; if that is the case.  I dunno.
   (let* ((toolset (cdr (assq (if use-alt
 				 rst-compile-secondary-toolset
 			       rst-compile-primary-toolset)
 			rst-compile-toolsets)))
@@ -3926,30 +4031,32 @@
     ;; Invoke the compile command.
     (if (or compilation-read-command use-alt)
         (call-interactively 'compile)
       (compile compile-command))
     ))
 
 (defun rst-compile-alt-toolset ()
-  "Compile command with the alternative toolset."
+  "Compile command with the alternative tool-set."
   (interactive)
   (rst-compile t))
 
 (defun rst-compile-pseudo-region ()
-  "Show the pseudo-XML rendering of the current active region,
-or of the entire buffer, if the region is not selected."
+  "Show pseudo-XML rendering.
+Rendering is done of the current active region, or of the entire
+buffer, if the region is not selected."
+  ;; FIXME: The region should be given interactively.
   (interactive)
   (with-output-to-temp-buffer "*pseudoxml*"
     (shell-command-on-region
      (if mark-active (region-beginning) (point-min))
      (if mark-active (region-end) (point-max))
      (cadr (assq 'pseudoxml rst-compile-toolsets))
      standard-output)))
 
-;; FIXME: Should be `defcustom`
+;; FIXME: Should be `defcustom`.
 (defvar rst-pdf-program "xpdf"
   "Program used to preview PDF files.")
 
 (defun rst-compile-pdf-preview ()
   "Convert the document to a PDF file and launch a preview program."
   (interactive)
   (let* ((tmp-filename (make-temp-file "rst_el" nil ".pdf"))
@@ -3958,15 +4065,15 @@
 			  buffer-file-name tmp-filename
 			  rst-pdf-program tmp-filename tmp-filename)))
     (start-process-shell-command "rst-pdf-preview" nil command)
     ;; Note: you could also use (compile command) to view the compilation
     ;; output.
     ))
 
-;; FIXME: Should be `defcustom` or use something like `browse-url`
+;; FIXME: Should be `defcustom` or use something like `browse-url`.
 (defvar rst-slides-program "firefox"
   "Program used to preview S5 slides.")
 
 (defun rst-compile-slides-preview ()
   "Convert the document to an S5 slide presentation and launch a preview program."
   (interactive)
   (let* ((tmp-filename (make-temp-file "rst_el" nil ".html"))
@@ -3979,56 +4086,55 @@
     ;; output.
     ))
 
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Generic text functions that are more convenient than the defaults.
 
-;; FIXME: Unbound command - should be bound or removed
+;; FIXME: Unbound command - should be bound or removed.
 (defun rst-replace-lines (fromchar tochar)
-  "Replace flush-left lines, consisting of multiple FROMCHAR characters,
-with equal-length lines of TOCHAR."
+  "Replace flush-left lines of FROMCHAR with equal-length lines of TOCHAR."
   (interactive "\
 cSearch for flush-left lines of char:
 cand replace with char: ")
   (save-excursion
     (let ((searchre (rst-re "^" fromchar "+\\( *\\)$"))
           (found 0))
       (while (search-forward-regexp searchre nil t)
         (setq found (1+ found))
         (goto-char (match-beginning 1))
         (let ((width (current-column)))
           (rst-delete-entire-line)
           (insert-char tochar width)))
       (message (format "%d lines replaced." found)))))
 
-;; FIXME: Unbound command - should be bound or removed
+;; FIXME: Unbound command - should be bound or removed.
 (defun rst-join-paragraph ()
   "Join lines in current paragraph into one line, removing end-of-lines."
   (interactive)
-  (let ((fill-column 65000)) ; some big number
+  (let ((fill-column 65000)) ; Some big number.
     (call-interactively 'fill-paragraph)))
 
-;; FIXME: Unbound command - should be bound or removed
+;; FIXME: Unbound command - should be bound or removed.
 (defun rst-force-fill-paragraph ()
   "Fill paragraph at point, first joining the paragraph's lines into one.
 This is useful for filling list item paragraphs."
   (interactive)
   (rst-join-paragraph)
   (fill-paragraph nil))
 
 
-;; FIXME: Unbound command - should be bound or removed
+;; FIXME: Unbound command - should be bound or removed.
 ;; Generic character repeater function.
 ;; For sections, better to use the specialized function above, but this can
 ;; be useful for creating separators.
 (defun rst-repeat-last-character (use-next)
-  "Fill the current line up to the length of the preceding line (if not
-empty), using the last character on the current line.  If the preceding line is
-empty, we use the `fill-column'.
+  "Fill the current line using the last character on the current line.
+Fill up to the length of the preceding line or up to
+`fill-column' if preceding line is empty.
 
 If USE-NEXT, use the next line rather than the preceding line.
 
 If the current line is longer than the desired length, shave the characters off
 the current line to fit the desired length.
 
 As an added convenience, if the command is repeated immediately, the alternative
@@ -4050,27 +4156,38 @@
           (cond ((equal last-command 'rst-repeat-last-character)
                  (if (= curcol fill-column) prevcol fill-column))
                 (t (save-excursion
                      (if (zerop prevcol) fill-column prevcol)))
                 )) )
     (end-of-line)
     (if (> (current-column) rightmost-column)
-        ;; shave characters off the end
+        ;; Shave characters off the end.
         (delete-region (- (point)
                           (- (current-column) rightmost-column))
                        (point))
-      ;; fill with last characters
+      ;; Fill with last characters.
       (insert-char (preceding-char)
                    (- rightmost-column (current-column))))
     ))
 
 
 (defun rst-portable-mark-active-p ()
-  "A portable function that returns non-nil if the mark is active."
+  "Return non-nil if the mark is active.
+This is a portable function."
   (cond
    ((fboundp 'region-active-p) (region-active-p))
    ((boundp 'transient-mark-mode) (and transient-mark-mode mark-active))
    (t mark-active)))
 
 
+
+;; LocalWords:  docutils http sourceforge rst html wp svn svnroot txt reST regex
+;; LocalWords:  regexes alist seq alt grp keymap abbrev overline overlines toc
+;; LocalWords:  XML PNT propertized
+
+;; Local Variables:
+;;   sentence-end-double-space: t
+;; End:
+
 (provide 'rst)
+
 ;;; rst.el ends here
```

### Comparing `docutils-0.9/tools/editors/README.txt` & `docutils-0.9.1/tools/editors/README.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/test/test_buildhtml.py` & `docutils-0.9.1/tools/test/test_buildhtml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# $Id: test_buildhtml.py 6370 2010-07-10 06:57:08Z grubert $
+# $Id: test_buildhtml.py 7442 2012-06-13 23:27:03Z milde $
 # Author: engelbert gruber <grubert@users.sourceforge.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 test buildhtml options, because ``--local`` is broken.
 
 Build-HTML Options
@@ -21,26 +21,39 @@
 --silent                Work silently (no progress messages).  Independent of
                         "--quiet".
 """
 
 import unittest
 import os
 import re
+try:
+    import tempfile
+except ImportError:
+    pass
+try:
+    from subprocess import Popen, PIPE, STDOUT
+except ImportError:
+    pass
 
 def process_and_return_filelist(options):
     dirs = []
     files = []
-    cin, cout = os.popen4("../buildhtml.py "+options)
+    try:
+        p = Popen("../buildhtml.py "+options, shell=True, 
+                  stdin=PIPE, stdout=PIPE, stderr=STDOUT, close_fds=True)
+        (cin, cout) = (p.stdin, p.stdout)
+    except NameError:
+        cin, cout = os.popen4("../buildhtml.py "+options)
     while 1:
-        ln = cout.readline()
-        if not ln:
+        line = cout.readline()
+        if not line:
             break
         # BUG no colon in filename/path allowed
-        item = ln.split(":")[-1].strip()
-        if ln.startswith(" "):
+        item = line.split(":")[-1].strip()
+        if line.startswith(" "):
             files.append(item)
         else:
             dirs.append(item)
     return (dirs, files)
 
 class BuildHtmlTests(unittest.TestCase):
     tree = ( "_tmp_test_tree",
@@ -54,16 +67,20 @@
              "_tmp_test_tree/dir2/two.txt", 
              "_tmp_test_tree/dir2/sub", 
              "_tmp_test_tree/dir2/sub/one.txt", 
              "_tmp_test_tree/dir2/sub/two.txt", 
              )
 
     def setUp(self):
-        self.root = os.tempnam()
-        os.mkdir(self.root)
+        try:
+            self.root = tempfile.mkdtemp()
+        except NameError:
+            self.root = os.tempnam()
+            os.mkdir(self.root)
+        
         for s in self.tree:
             s = os.path.join(self.root, s)
             if not "." in s:
                 os.mkdir(s)
             else:
                 open(s, "w").write("dummy")
```

### Comparing `docutils-0.9/tools/buildhtml.py` & `docutils-0.9.1/tools/buildhtml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# $Id: buildhtml.py 7323 2012-01-23 20:57:29Z goodger $
+# $Id: buildhtml.py 7442 2012-06-13 23:27:03Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 Generates .html from all the .txt files in a directory.
 
 Ordinary .txt files are understood to be standalone reStructuredText.
@@ -196,21 +196,21 @@
                     del dirs[:]
                 self.visit(root, files, dirs)
 
     def visit(self, directory, names, subdirectories):
         settings = self.get_settings('', directory)
         errout = ErrorOutput(encoding=settings.error_encoding)
         if settings.prune and (os.path.abspath(directory) in settings.prune):
-            print >>errout, ('/// ...Skipping directory (pruned): %s' %
-                              directory)
+            errout.write('/// ...Skipping directory (pruned): %s\n' %
+                         directory)
             sys.stderr.flush()
             del subdirectories[:]
             return
         if not self.initial_settings.silent:
-            print >>errout, '/// Processing directory: %s' % directory
+            errout.write('/// Processing directory: %s' % directory)
             sys.stderr.flush()
         # settings.ignore grows many duplicate entries as we recurse
         # if we add patterns in config files or on the command line.
         for pattern in utils.uniq(settings.ignore):
             for i in range(len(names) - 1, -1, -1):
                 if fnmatch(names[i], pattern):
                     # Modify in place!
@@ -226,23 +226,24 @@
             publisher = '.txt'
         settings = self.get_settings(publisher, directory)
         errout = ErrorOutput(encoding=settings.error_encoding)
         pub_struct = self.publishers[publisher]
         settings._source = os.path.normpath(os.path.join(directory, name))
         settings._destination = settings._source[:-4]+'.html'
         if not self.initial_settings.silent:
-            print >>errout, '    ::: Processing: %s' % name
+            errout.write('    ::: Processing: %s\n' % name)
             sys.stderr.flush()
         try:
             if not settings.dry_run:
                 core.publish_file(source_path=settings._source,
                               destination_path=settings._destination,
                               reader_name=pub_struct.reader_name,
                               parser_name='restructuredtext',
                               writer_name=pub_struct.writer_name,
                               settings=settings)
-        except ApplicationError, error:
-            print >>errout, '        %s' % ErrorString(error)
+        except ApplicationError:
+            error = sys.exc_info()[1] # get exception in Python <2.6 and 3.x
+            errout.write('        %s\n' % ErrorString(error))
 
 
 if __name__ == "__main__":
     Builder().run()
```

### Comparing `docutils-0.9/tools/quicktest.py` & `docutils-0.9.1/tools/quicktest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# $Id: quicktest.py 6262 2010-03-09 14:53:16Z milde $
+# $Id: quicktest.py 7442 2012-06-13 23:27:03Z milde $
 # Authors: Garth Kidd <garth@deadlybloodyserious.com>;
 #          David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
@@ -48,29 +48,29 @@
            ('debug', 'd', 'debug mode (lots of output)'),
            ('version', 'V', 'show Docutils version then exit'),
            ('help', 'h', 'show help text then exit')]
 """See ``distutils.fancy_getopt.FancyGetopt.__init__`` for a description of
 the data structure: (long option, short option, description)."""
 
 def usage():
-    print usage_header
+    print(usage_header)
     for longopt, shortopt, description in options:
         if longopt[-1:] == '=':
             opts = '-%s arg, --%sarg' % (shortopt, longopt)
         else:
             opts = '-%s, --%s' % (shortopt, longopt)
-        print '%-15s' % opts,
+        sys.stdout.write('%-15s' % opts)
         if len(opts) > 14:
-            print '%-16s' % '\n',
+            sys.stdout.write('%-16s' % '\n')
         while len(description) > 60:
             limit = description.rindex(' ', 0, 60)
-            print description[:limit].strip()
+            print(description[:limit].strip())
             description = description[limit + 1:]
-            print '%-15s' % ' ',
-        print description
+            sys.stdout.write('%-15s' % ' ')
+        print(description)
 
 def _pretty(input, document, optargs):
     return document.pformat()
 
 def _rawxml(input, document, optargs):
     return document.asdom().toxml()
 
@@ -138,17 +138,17 @@
         sys.exit(2)
     optargs = {'debug': 0, 'attributes': 0}
     for o, a in opts:
         if o in ['-h', '--help']:
             usage()
             sys.exit()
         elif o in ['-V', '--version']:
-            print >>sys.stderr, ('quicktest.py (Docutils %s [%s])'
-                                 % (docutils.__version__,
-                                    docutils.__version_details__))
+            sys.stderr.write('quicktest.py (Docutils %s [%s])\n' %
+                             (docutils.__version__, 
+                              docutils.__version_details__))
             sys.exit()
         elif o in ['-r', '--rawxml']:
             outputFormat = 'rawxml'
         elif o in ['-s', '--styledxml']:
             outputFormat = 'styledxml'
             optargs['styledxml'] = a
         elif o in ['-x', '--xml']:
@@ -158,17 +158,17 @@
         elif o in ['-t', '--test']:
             outputFormat = 'test'
         elif o in ['--attributes', '-A']:
             optargs['attributes'] = 1
         elif o in ['-d', '--debug']:
             optargs['debug'] = 1
         else:
-            raise getopt.GetoptError, "getopt should have saved us!"
+            raise getopt.GetoptError("getopt should have saved us!")
     if len(args) > 2:
-        print 'Maximum 2 arguments allowed.'
+        print('Maximum 2 arguments allowed.')
         usage()
         sys.exit(1)
     inputFile = sys.stdin
     outputFile = sys.stdout
     if args:
         inputFile = open(args.pop(0))
     if args:
```

### Comparing `docutils-0.9/tools/rst2html.py` & `docutils-0.9.1/tools/rst2html.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2latex.py` & `docutils-0.9.1/tools/rst2latex.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2man.py` & `docutils-0.9.1/tools/rst2man.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2odt.py` & `docutils-0.9.1/tools/rst2odt.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2odt_prepstyles.py` & `docutils-0.9.1/tools/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2pseudoxml.py` & `docutils-0.9.1/tools/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2s5.py` & `docutils-0.9.1/tools/rst2s5.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2xetex.py` & `docutils-0.9.1/tools/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rst2xml.py` & `docutils-0.9.1/tools/rst2xml.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/tools/rstpep2html.py` & `docutils-0.9.1/tools/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/BUGS.txt` & `docutils-0.9.1/BUGS.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/COPYING.txt` & `docutils-0.9.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/FAQ.txt` & `docutils-0.9.1/FAQ.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/HISTORY.txt` & `docutils-0.9.1/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,73 @@
 
 ==================
  Docutils History
 ==================
 
 :Author: David Goodger; open to all Docutils developers
 :Contact: goodger@python.org
-:Date: $Date: 2012-05-02 19:13:41 +0200 (Mit, 02 Mai 2012) $
-:Revision: $Revision: 7410 $
+:Date: $Date: 2012-06-17 22:47:44 +0200 (Son, 17 Jun 2012) $
+:Revision: $Revision: 7447 $
 :Web site: http://docutils.sourceforge.net/
 :Copyright: This document has been placed in the public domain.
 
 .. contents::
 
+Release 0.9.1 (2012-06-17)
+==========================
+
+* docutils/setup.py
+
+  - Fix [ 3527842 ]. Under Python 3, converted tests and tools were
+    installed in the PYTHONPATH. Converted tests are now
+    stored in ``test3/``, tools no longer need conversion.
+
+    If you installed one of Docutils versions 0.7 ... 0.9 with
+    ``setup.py install`` under Python 3, remove the spurious
+    ``test/`` and ``tools/`` directories in the site library root.
+
+* docutils/test/
+
+  - Make tests independent from the location of the ``test/`` directory.
+  - Use converted sources (from the ``build/`` directory) for tests under
+    Python 3.
+
+* docutils/tools/
+
+  - Make tools compatible with both, Python 2 and 3 without 2to3-conversion.
+
+* docutils/io.py
+
+  - Fix writing binary data to sys.stdout under Python 3 (allows
+    ``rst2odt.py`` to be used with output redirection).
+
+* docutils/parsers/rst/directives/misc.py
+
+  - Fix [ 3525847 ]. Catch and report UnicodeEncodeError with
+    ``locale == C`` and 8-bit char in path argument of `include` directive.
+
+* docutils/test/alltests.py
+
+  - class `Tee`: catch UnicodeError when writing to "ascii" stream or
+    file under Python 3.
+
 Release 0.9 (2012-05-02)
 ========================
 
 * General:
 
   - New reStructuredText "code" role and directive and "code" option
     of the "include" directive with syntax highlighting by Pygments_.
   - Fix parse_option_marker for option arguments containing ``=``.
+  - Fix [ 2993756 ]: import Python Imaging Library's Image module
+    via ``import PIL`` as starting with PIL 1.2,
+    "PIL lives in the PIL namespace only" (announcement__).
 
 .. _Pygments: http://pygments.org/
+__ http://mail.python.org/pipermail/image-sig/2011-January/006650.html
 
 * setup.py
 
   - Fix [ 2971827 ] and [ 3442827 ]
     extras/roman.py moved to docutils/utils/roman.py
 
 * docutils/frontend.py
@@ -109,15 +151,15 @@
 * General:
 
   - Fix [ 3364658 ] (Change last file with Apache license to BSD-2-Clause)
     and [ 3395920 ] (correct copyright info for rst.el).
 
 * docutils/test/
 
-  -  Apply [ 3303733 ] and [ 3365041 ] to fix tests under py3k.
+  -  Apply [ 3303733 ] and [ 3365041 ] to fix tests under Py3k.
 
 * docutils/writers/latex2e/__init__.py
 
   - Clean up Babel language setting. Restores Sphinx compatibility.
 
 Release 0.8 (2011-07-07)
 ========================
@@ -210,15 +252,15 @@
 
   - Fix [ 1830389 ] Replace not breaking on getting system_messages from
     nested_parse
 
 * docutils/io.py:
 
   - Do not close() sys.stdin, sys.stdout, or sys.stderr. Prevents
-    ``Exception ValueError: 'I/O operation on closed file.'`` with Python 3.
+    ``Exception ValueError: 'I/O operation on closed file.'`` with Python 3.
 
 Release 0.7 (2010-07-07)
 ========================
 
 * General:
 
   - Fix [ 2881769 ] setup configuration.
@@ -278,15 +320,15 @@
 * docutils/nodes.py
 
   - Fix: encoding ``'ascii'`` must be lowercase to prevent problems for
     turkish locale.
 
 * setup.py:
 
-  - Python 3 support: copy test/ and tools/ to the build-dir
+  - Python 3 support: copy test/ and tools/ to the build-dir
     and convert Python sources with 2to3.
 
 
 Release 0.6 (2009-10-11)
 ========================
 
 * General:
```

### Comparing `docutils-0.9/README.txt` & `docutils-0.9.1/README.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 ======================
  README: Docutils 0.9
 ======================
 
 :Author: David Goodger
 :Contact: goodger@python.org
-:Date: $Date: 2012-02-28 17:39:05 +0100 (Die, 28 Feb 2012) $
+:Date: $Date: 2012-06-14 01:27:03 +0200 (Don, 14 Jun 2012) $
 :Web site: http://docutils.sourceforge.net/
 :Copyright: This document has been placed in the public domain.
 
 .. contents::
 
 
 Quick-Start
 ===========
 
-This is for those who want to get up & running quickly.  Read on for
-complete details.
+This is for those who want to get up & running quickly.
 
-1. Get and install the latest release of Python, available from
+1. Docutils requires Python (version 2.3 or later), available from
 
-       http://www.python.org/
+     http://www.python.org/
 
-   Docutils is compatible with Python versions from 2.3 up to 2.6 and
-   version 3.1. (Support for Python 3 is new and might still have some
-   issues.)
+   See Requirements_ below for details.
 
-2. Use the latest Docutils code.  Get the code from Subversion or from
-   the snapshot:
+2. Use the latest Docutils code.  Get the code from the `Subversion
+   repository`_ or from the snapshot:
 
-       http://docutils.svn.sourceforge.net/viewvc/docutils/trunk/docutils/?view=tar
+     http://docutils.svn.sourceforge.net/viewvc/docutils/trunk/docutils/?view=tar
 
    See `Releases & Snapshots`_ below for details.
 
 3. Unpack the tarball in a temporary directory (**not** directly in
-   Python's ``site-packages``) and run ``setup.py install`` or
-   ``install.py`` with admin rights.  On Windows systems it may be
-   sufficient to double-click ``install.py``.  On Unix or Mac OS X,
-   type::
-
-        su
-        (enter admin password)
-        ./setup.py install
-
-   Docutils will only work with Python 3, if installed with a Python
-   version >= 3. If your default Python version is 2.x, also call
-   ``python3 setup.py install`` from the temporary directory.
+   Python's ``site-packages``), go to the directory created by expanding
+   the archive, and run ``setup.py install`` with admin rights. On
+   Windows systems it may be sufficient to double-click ``install.py``.
+
    See Installation_ below for details.
 
-4. Use a front-end tool from the "tools" subdirectory of the same
-   directory as in step 3.  For example::
+4. Use the front-end scripts to convert reStructuredText documents.
+   Try for example::
 
-       cd tools
-       ./rst2html.py ../FAQ.txt ../FAQ.html        (Unix)
-       python rst2html.py ..\FAQ.txt ..\FAQ.html   (Windows)
+       rst2html.py FAQ.txt FAQ.html         (Unix)
+       python tools/rst2html.py FAQ.txt FAQ.html  (Windows)
 
    See Usage_ below for details.
 
 
 Purpose
 =======
 
@@ -99,33 +87,65 @@
 * Snapshot of Docutils code, documentation, front-end tools, and
   tests:
   http://docutils.svn.sourceforge.net/viewvc/docutils/trunk/docutils/?view=tar
 
 * Snapshot of the Sandbox (experimental, contributed code):
   http://docutils.svn.sourceforge.net/viewvc/docutils/trunk/sandbox/?view=tar
 
-To keep up to date on the latest developments, download fresh copies
-of the snapshots regularly.  New functionality is being added weekly,
-sometimes daily.  (There's also the `Subversion repository`_.)
+To keep up to date on the latest developments, download fresh copies of
+the snapshots regularly or use a working copy of the
+`Subversion repository`_.
 
 .. _Subversion repository: docs/dev/repository.html
 
 
 Requirements
 ============
 
-To run the code, Python 2.3 or later must already be installed.
-Python is available from
-http://www.python.org/.
+To run the code, Python_ must be installed.
+Docutils is compatible with Python versions from 2.3 up to 2.7 and
+versions 3.1 and 3.2 (cf. `Python 3 compatibility`_).
+
+Docutils uses the following packages for enhanced functionality, if they are
+installed:
 
-The `Python Imaging Library`, or PIL, is used for some image
-manipulation operations if it is installed.
+* The `Python Imaging Library`_, or PIL, is used for some image
+  manipulation operations.
 
+* The `Pygments`_ syntax highlighter is used for content of `code`
+  directives and roles.
+
+.. _Python: http://www.python.org/.
 .. _Python Imaging Library: http://www.pythonware.com/products/pil/
-.. _Optik: http://optik.sourceforge.net/
+.. _Pygments: http://pygments.org/
+
+
+Python 3 compatibility
+----------------------
+
+The Docutils codebase is written for Python 2 and uses "on-demand"
+translation for `porting to Python 3`_.
+
+* The `setup.py` script generates Python 3 compatible sources in
+  ``build/`` and tests in ``tests3/`` sub-directories during
+  installation_ with Python 3.
+
+* The scripts in the ``tools/`` sub-directory work with all supported
+  Python versions without conversion.
+
+* To convert the sources without installing (e.g. for testing), run
+  ``python3 setup.py build``.
+
+* When editing the source, do changes on the Python 2 versions of the
+  files and re-run the build command.
+
+Using Docutils with Python 3.x is less tested and might still have some
+issues.
+
+.. _porting to Python 3: http://docs.python.org/py3k/howto/pyporting.html
 
 
 Project Files & Directories
 ===========================
 
 * README.txt: You're reading it.
 
@@ -147,18 +167,14 @@
 
 * install.py: Quick & dirty installation script.  Just run it.  For
   any kind of customization or help though, setup.py must be used.
 
 * docutils: The project source directory, installed as a Python
   package.
 
-* extras: Directory for third-party modules that Docutils depends on
-  (roman.py).  These are only installed if
-  they're not already present.
-
 * docs: The project documentation directory.  Read ``docs/index.txt``
   for an overview.
 
 * docs/user: The project user documentation directory.  Contains the
   following documents, among others:
 
   - docs/user/tools.txt: Docutils Front-End Tools
@@ -176,14 +192,20 @@
 * tools: Directory for Docutils front-end tools.  See
   ``docs/user/tools.txt`` for documentation.
 
 * test: Unit tests.  Not required to use the software, but very useful
   if you're planning to modify it.  See `Running the Test Suite`_
   below.
 
+Generated directories when installing under Python 3:
+
+* build: Converted sources.
+
+* test3: Converted tests.
+
 
 Installation
 ============
 
 The first step is to expand the ``.tgz`` archive in a temporary
 directory (**not** directly in Python's ``site-packages``).  It
 contains a distutils setup file "setup.py".  OS-specific installation
@@ -195,27 +217,34 @@
 
 1. Open a shell.
 
 2. Go to the directory created by expanding the archive::
 
        cd <archive_directory_path>
 
-3. Install the package::
+3. Install the package (you may need root permissions to complete this
+   step)::
 
+       su
+       (enter admin password)
        python setup.py install
 
    If the python executable isn't on your path, you'll have to specify
-   the complete path, such as /usr/local/bin/python.  You may need
-   root permissions to complete this step.
+   the complete path, such as ``/usr/local/bin/python``.
 
-   To install for a specific python version, use this version in the
+   To install for a specific Python version, use this version in the
    setup call, e.g. ::
 
        python3.1 setup.py install
 
+   To install for different Python versions, repeat step 3 for every
+   required version. The last installed version will be used in the
+   `shebang line`_ of the ``rst2*.py`` wrapper scripts.
+
+   .. _shebang line: http://en.wikipedia.org/wiki/Shebang_%28Unix%29
 
 Windows
 -------
 
 Just double-click ``install.py``.  If this doesn't work, try the
 following:
 
@@ -229,33 +258,45 @@
 3. Install the package::
 
        <path_to_python.exe>\python setup.py install
 
    To install for a specific python version, specify the Python
    executable for this version.
 
+   To install for different Python versions, repeat step 3 for every
+   required version.
 
-Python 3 peculiarities
-----------------------
+Optional steps:
+
+* `running the test suite`_
 
-If called from Python 3, setup.py, in addition to copying the sources
-to the right place, will also convert them using 2to3 to Python 3
-compatible code.
-
-* If you want to test or develop Docutils, also run ``python3 setup.py
-  build``. This will generate Python 3 compatible sources, tests and
-  developer tools in the build directory.  Do changes on the Python 2
-  versions of the sources and re-run the build command. This works
-  incrementally, so if you change one file it will only reconvert that
-  file the next time you run setup.py build.
+* `converting the documentation`_
 
 
 Usage
 =====
 
+There are many front-end tools in the unpacked "tools" subdirectory.
+Installation under Unix places copies in the PATH.
+You may want to begin with the "rst2html.py" front-end tool.  Most
+tools take up to two arguments, the source path and destination path,
+with STDIN and STDOUT being the defaults.  Use the "--help" option to
+the front-end tools for details on options and arguments.  See
+Docutils Front-End Tools (``docs/user/tools.txt``) for full documentation.
+
+The package modules are continually growing and evolving.  The
+``docutils.statemachine`` module is usable independently.  It contains
+extensive inline documentation (in reStructuredText format of course).
+
+Contributions are welcome!
+
+
+Converting the documentation
+============================
+
 After unpacking and installing the Docutils package, the following
 shell commands will generate HTML for all included documentation::
 
     cd <archive_directory_path>/tools
     ./buildhtml.py ../
 
 On Windows systems, type::
@@ -268,54 +309,39 @@
 called "docutils-X.Y.Z", where "X.Y.Z" is the release version.
 Alternatively::
 
     cd <archive_directory_path>
     tools/buildhtml.py --config=tools/docutils.conf          (Unix)
     python tools\buildhtml.py --config=tools\docutils.conf   (Windows)
 
-With Python 3, call::
-
-    build/<Python-3-subdir>/tools/buildhtml.py --config=tools/docutils.conf
-
 Some files may generate system messages (warnings and errors).  The
 ``docs/user/rst/demo.txt`` file (under the archive directory) contains
 five intentional errors.  (They test the error reporting mechanism!)
 
-There are many front-end tools in the unpacked "tools" subdirectory.
-You may want to begin with the "rst2html.py" front-end tool.  Most
-tools take up to two arguments, the source path and destination path,
-with STDIN and STDOUT being the defaults.  Use the "--help" option to
-the front-end tools for details on options and arguments.  See
-Docutils Front-End Tools (``docs/user/tools.txt``) for full documentation.
-
-The package modules are continually growing and evolving.  The
-``docutils.statemachine`` module is usable independently.  It contains
-extensive inline documentation (in reStructuredText format of course).
-
-Contributions are welcome!
-
 
 Running the Test Suite
 ======================
 
-To run the entire test suite, after installation_ open a shell and use
-the following commands::
+The test suite is documented in `Docutils Testing`_ (docs/dev/testing.txt).
+
+To run the entire test suite, open a shell and use the following
+commands::
 
     cd <archive_directory_path>/test
     ./alltests.py
 
 Under Windows, type::
 
     cd <archive_directory_path>\test
     python alltests.py
 
 For testing with Python 3 use the converted test suite::
 
-    cd <archive_directory_path>/build/<Python-3-subdir>/test
-    python alltests.py
+    cd <archive_directory_path>/test3
+    python3 alltests.py
 
 
 You should see a long line of periods, one for each test, and then a
 summary like this::
 
     Ran 1111 tests in 24.653s
 
@@ -338,17 +364,16 @@
     ./quicktest.py --version
 
 Windows users type these commands::
 
     cd ..\tools
     python quicktest.py --version
 
-Python 3 users must use ``build/<Python-3-subdir>/tools/quicktest.py``.
-
 
+.. _Docutils Testing: http://docutils.sourceforge.net/docs/dev/testing.html
 .. _open a bug report:
    http://sourceforge.net/tracker/?group_id=38414&atid=422030
 .. _send email: mailto:docutils-users@lists.sourceforge.net
    ?subject=Test%20suite%20failure
 .. _web interface: http://post.gmane.org/post.php
    ?group=gmane.text.docutils.user&subject=Test+suite+failure
```

### Comparing `docutils-0.9/RELEASE-NOTES.txt` & `docutils-0.9.1/RELEASE-NOTES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 ========================
  Docutils Release Notes
 ========================
 
 :Contact: grubert@users.sourceforge.net
-:Date: $Date: 2012-05-02 19:13:41 +0200 (Mit, 02 Mai 2012) $
-:Revision: $Revision: 7410 $
+:Date: $Date: 2012-06-18 00:05:00 +0200 (Mon, 18 Jun 2012) $
+:Revision: $Revision: 7452 $
 :Web site: http://docutils.sourceforge.net/
 :Copyright: This document has been placed in the public domain.
 
 
 This document summarizes the major changes in recent releases.  For a
 more detailed list of changes, please see the `Docutils History`_.
 
 .. _Docutils History: HISTORY.html
 
 .. contents::
 
 Future changes
 ==============
 
+* Support for Python 2.3 will be dropped in version 0.10.
+
 * docutils/math, docutils/error_reporting.py, and
   docutils/urischemes.py will move to the utils package
   Code importing these modules needs to adapt, e.g.::
 
     try:
         import docutils.math as math
     except ImportError:
@@ -30,20 +32,39 @@
 
 * docutils.io.FileInput/FileOutput will no longer do a
   system-exit on IOError by default.
 
   Roadmap:
 
   :0.10: change of default behaviour to the equivalent of
-         ``handle_io_errors=False`` and deprecation of the
-         `handle_io_errors` option,
-  :0.11: deprecation warning to stderr if FileInput/FileOutput
-         is called with `handle_io_errors`,
-  :0.12: ignore ``handle_io_errors=True``,
-  :0.13: remove the `handle_io_errors` option.
+         ``handle_io_errors=False``,
+         ignore and deprecate the `handle_io_errors` option.
+         (allows us to clean up Docutils code and remove the error handling
+         code from the FileInput/FileOutput classes)
+  :0.10 + n:   deprecation warning to stderr if FileInput/FileOutput
+               is called with `handle_io_errors`,
+  :0.10 + n+1: remove the `handle_io_errors` option.
+
+
+Release 0.9.1 (2012-06-17)
+==========================
+
+* General:
+
+  Several fixes for Python 3 usage.
+
+* docutils/setup.py
+
+  - Fix [ 3527842 ]. Under Python 3, converted tests and tools were
+    installed in the PYTHONPATH. Converted tests are now
+    stored in ``docutils/test3/``, tools no longer need conversion.
+
+    If you installed one of Docutils versions 0.7 ... 0.9 with
+    ``setup.py install`` under Python 3, remove the spurious
+    ``test/`` and ``tools/`` directories in the site library root.
 
 
 Release 0.9 (2012-05-02)
 =========================
 
 * General:
 
@@ -83,22 +104,19 @@
 ==========================
 
 * General:
 
   - Fix [ 3364658 ] (Change last file with Apache license to BSD-2-Clause)
     and [ 3395920 ] (correct copyright info for rst.el).
 
-* docutils/test/
-
-  -  Apply [ 3303733 ] and [ 3365041 ] to fix tests under py3k.
-
 * docutils/writers/latex2e/__init__.py
 
   - Clean up Babel language setting. Restores Sphinx compatibility.
 
+
 Release 0.8 (2011-07-07)
 ========================
 
 * COPYING:
 
   - Some additions to the Docutils core are released under the 2-Clause BSD
     license.
@@ -148,14 +166,15 @@
 
   - New writer generating LaTeX code for compiling with ``xelatex``.
 
     XeTeX uses unicode and modern font technologies.
 
 * and fixes and enhancements here and there.
 
+
 Release 0.7 (2010-07-07)
 ========================
 
 Components:
 
 * HTML writer:
 
@@ -192,14 +211,15 @@
   (mode "rU", configurable with the new optional argument "mode").
 
 * setup.py:
 
   - Python 3 support: copy test/ and tools/ to the build-dir
     and convert Python sources with 2to3.
 
+
 Release 0.6 (2009-10-11)
 ========================
 
 .. Note::
 
    Docutils 0.5 is the last version supporting Python 2.2.
 
@@ -311,14 +331,15 @@
 * Configuration files are now assumed and required to be
   UTF-8-encoded.
 
 * Added docutils/writers/html4css1/template.txt.
 
 * Enhance emacs support.
 
+
 Release 0.4 (2006-01-09)
 ========================
 
 .. Note::
 
    Docutils 0.4.x is the last version that will support Python 2.1.
    Docutils 0.5 will *not* be compatible with Python 2.1; Python 2.2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `docutils-0.9/THANKS.txt` & `docutils-0.9.1/THANKS.txt`

 * *Files identical despite different names*

### Comparing `docutils-0.9/install.py` & `docutils-0.9.1/install.py`

 * *Files identical despite different names*

### Comparing `docutils-0.9/setup.py` & `docutils-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# $Id: setup.py 7268 2011-12-20 16:39:10Z milde $
+# $Id: setup.py 7446 2012-06-17 20:47:10Z grubert $
 # Copyright: This file has been placed in the public domain.
 
 import sys
 import os
 import glob
 try:
     from distutils.core import setup, Command
@@ -24,16 +24,16 @@
 
 
 if sys.version_info >= (3,):
     # copy-convert auxiliary python sources
     class copy_build_py_2to3(build_py_2to3):
         """Copy/convert Python source files in given directories recursively.
 
-        Build py3k versions of the modules and packages. Also copy
-        'tools/' and 'test/' dirs and run 2to3 on *.py files.
+        Build py3k versions of the modules and packages.
+        Also copy 'test/' suite and run 2to3 on *.py files.
         """
         manifest_in = """\
         exclude *.pyc *~ .DS_Store
         recursive-exclude * *.pyc *~ .DS_Store
         recursive-exclude functional/output *
         include functional/output/README.txt
         prune .svn
@@ -41,19 +41,17 @@
         prune */*/.svn
         prune */*/*/.svn
         prune */*/*/*/.svn
         prune */*/*/*/*/.svn
         """
         def run(self):
             build_py_2to3.run(self)
-            print("copying aux dirs")
+            print("copy/convert test suite")
             loglevel = log.set_threshold(log.ERROR)
-            for source in ['tools', 'test']:
-                dest = os.path.join(self.build_lib, source)
-                copydir_run_2to3(source, dest, template=self.manifest_in)
+            copydir_run_2to3('test', 'test3', template=self.manifest_in)
             log.set_threshold(loglevel)
 
 
 class smart_install_data(install_data):
     # From <http://wiki.python.org/moin/DistutilsInstallDataScattered>,
     # by Pete Shinners.
 
@@ -111,15 +109,15 @@
     'description': 'Docutils -- Python Documentation Utilities',
     'long_description': """\
 Docutils is a modular system for processing documentation
 into useful formats, such as HTML, XML, and LaTeX.  For
 input Docutils supports reStructuredText, an easy-to-read,
 what-you-see-is-what-you-get plaintext markup syntax.""", # wrap at col 60
     'url': 'http://docutils.sourceforge.net/',
-    'version': '0.9',
+    'version': '0.9.1',
     'author': 'David Goodger',
     'author_email': 'goodger@python.org',
     'license': 'public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)',
     'platforms': 'OS-independent',
     'package_dir': {'docutils': 'docutils',
                     'docutils.tools': 'tools'},
     'packages': ['docutils',
@@ -183,37 +181,39 @@
     'Intended Audience :: System Administrators',
     'License :: Public Domain',
     'License :: OSI Approved :: Python Software Foundation License',
     'License :: OSI Approved :: BSD License',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
     'Topic :: Documentation',
     'Topic :: Software Development :: Documentation',
     'Topic :: Text Processing',
     'Natural Language :: English',      # main/default language, keep first
     'Natural Language :: Afrikaans',
-    'Natural Language :: Brazilian Portuguese',
     'Natural Language :: Catalan',
+    'Natural Language :: Chinese (Simplified)',
+    'Natural Language :: Chinese (Traditional)',
     'Natural Language :: Czech',
     'Natural Language :: Dutch',
     'Natural Language :: Esperanto',
     'Natural Language :: Finnish',
     'Natural Language :: French',
     'Natural Language :: Galician',
     'Natural Language :: German',
     'Natural Language :: Italian',
     'Natural Language :: Japanese',
-    'Natural Language :: Lithuanian',
     'Natural Language :: Polish',
+    'Natural Language :: Portuguese (Brazilian)',
     'Natural Language :: Russian',
-    'Natural Language :: Simplified Chinese ',
     'Natural Language :: Slovak',
     'Natural Language :: Spanish',
     'Natural Language :: Swedish',
-    'Natural Language :: Traditional Chinese ',
     ]
+# BUG pypi did not like fllowing languages
+#   'Natural Language :: Lithuanian',
 """Trove classifiers for the Distutils "register" command;
 Python 2.3 and up."""
 
 if __name__ == '__main__' :
     do_setup()
```

### Comparing `docutils-0.9/PKG-INFO` & `docutils-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: docutils
-Version: 0.9
+Version: 0.9.1
 Summary: Docutils -- Python Documentation Utilities
 Home-page: http://docutils.sourceforge.net/
 Author: David Goodger
 Author-email: goodger@python.org
 License: public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
 Description: Docutils is a modular system for processing documentation
         into useful formats, such as HTML, XML, and LaTeX.  For
@@ -19,31 +19,31 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Public Domain
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Afrikaans
-Classifier: Natural Language :: Brazilian Portuguese
 Classifier: Natural Language :: Catalan
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: Czech
 Classifier: Natural Language :: Dutch
 Classifier: Natural Language :: Esperanto
 Classifier: Natural Language :: Finnish
 Classifier: Natural Language :: French
 Classifier: Natural Language :: Galician
 Classifier: Natural Language :: German
 Classifier: Natural Language :: Italian
 Classifier: Natural Language :: Japanese
-Classifier: Natural Language :: Lithuanian
 Classifier: Natural Language :: Polish
+Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Natural Language :: Russian
-Classifier: Natural Language :: Simplified Chinese 
 Classifier: Natural Language :: Slovak
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Swedish
-Classifier: Natural Language :: Traditional Chinese
```

